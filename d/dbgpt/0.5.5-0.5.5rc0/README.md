# Comparing `tmp/dbgpt-0.5.5.tar.gz` & `tmp/dbgpt-0.5.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbgpt-0.5.5.tar", last modified: Fri Apr 26 06:29:52 2024, max compression
+gzip compressed data, was "dbgpt-0.5.5rc0.tar", last modified: Thu Apr 18 03:05:22 2024, max compression
```

## Comparing `dbgpt-0.5.5.tar` & `dbgpt-0.5.5rc0.tar`

### file list

```diff
@@ -1,465 +1,462 @@
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.677514 dbgpt-0.5.5/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1067 2023-06-21 06:41:58.000000 dbgpt-0.5.5/LICENSE
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       59 2023-12-05 02:13:48.000000 dbgpt-0.5.5/MANIFEST.in
--rw-r--r--   0 staneyffer  (1000) staneyffer  (1000)    31236 2024-04-26 06:29:52.677514 dbgpt-0.5.5/PKG-INFO
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    12350 2024-04-23 06:52:33.000000 dbgpt-0.5.5/README.md
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.525515 dbgpt-0.5.5/dbgpt/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      638 2024-01-22 13:19:20.000000 dbgpt-0.5.5/dbgpt/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.529515 dbgpt-0.5.5/dbgpt/_private/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       83 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/_private/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    14757 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/_private/config.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1693 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/_private/llm_metadata.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2234 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/_private/pydantic.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       18 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/_version.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.529515 dbgpt-0.5.5/dbgpt/agent/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1125 2024-04-15 06:23:33.000000 dbgpt-0.5.5/dbgpt/agent/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.529515 dbgpt-0.5.5/dbgpt/agent/actions/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       24 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/actions/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5354 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/actions/action.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      890 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/actions/blank_action.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3746 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/actions/chart_action.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5097 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/actions/code_action.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4461 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/actions/dashboard_action.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5443 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/actions/indicator_action.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5491 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/actions/plugin_action.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.533515 dbgpt-0.5.5/dbgpt/agent/core/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       33 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/core/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9497 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/core/agent.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5364 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/core/agent_manage.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    35815 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/core/base_agent.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5544 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/core/base_team.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.533515 dbgpt-0.5.5/dbgpt/agent/core/llm/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       22 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/core/llm/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3473 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/core/llm/llm.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6745 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/core/llm/llm_client.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.533515 dbgpt-0.5.5/dbgpt/agent/core/llm/strategy/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       27 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/core/llm/strategy/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1291 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/core/llm/strategy/priority.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3715 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/core/role.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      456 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/core/schema.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      466 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/core/user_proxy_agent.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.533515 dbgpt-0.5.5/dbgpt/agent/expand/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1675 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/expand/Indicator_assistant_agent.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       26 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/expand/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7025 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/expand/code_assistant_agent.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2207 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/expand/dashboard_assistant_agent.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5415 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/expand/data_scientist_agent.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2715 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/expand/plugin_assistant_agent.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    22055 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1685 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/expand/summary_assistant_agent.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.537515 dbgpt-0.5.5/dbgpt/agent/memory/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       32 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/memory/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6850 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/memory/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5803 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/memory/default_gpts_memory.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7170 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/memory/gpts_memory.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.537515 dbgpt-0.5.5/dbgpt/agent/plan/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      914 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plan/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.537515 dbgpt-0.5.5/dbgpt/agent/plan/awel/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       60 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plan/awel/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    10852 2024-04-15 06:23:33.000000 dbgpt-0.5.5/dbgpt/agent/plan/awel/agent_operator.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6014 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/plan/awel/agent_operator_resource.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8258 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/plan/awel/team_awel_layout.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4732 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plan/plan_action.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7582 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/plan/planner_agent.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    12459 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plan/team_auto_plan.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.537515 dbgpt-0.5.5/dbgpt/agent/plugin/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      214 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.541515 dbgpt-0.5.5/dbgpt/agent/plugin/commands/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       23 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/commands/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.541515 dbgpt-0.5.5/dbgpt/agent/plugin/commands/built_in/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       36 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/commands/built_in/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.541515 dbgpt-0.5.5/dbgpt/agent/plugin/commands/built_in/display_type/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       88 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    10775 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      687 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1188 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5226 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/commands/command.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    22485 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/plugin/commands/command_manage.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1166 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/commands/exceptions.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4438 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/generator.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1240 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/loader.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7625 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/plugin/plugins_util.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.541515 dbgpt-0.5.5/dbgpt/agent/resource/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      665 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/resource/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3721 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/agent/resource/resource_api.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4443 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/resource/resource_db_api.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      782 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/resource/resource_knowledge_api.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1350 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/resource/resource_loader.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3224 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/resource/resource_plugin_api.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.541515 dbgpt-0.5.5/dbgpt/agent/util/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      114 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/util/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      850 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/agent/util/cmp.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.541515 dbgpt-0.5.5/dbgpt/cli/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        0 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/cli/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5794 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/cli/cli_scripts.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.545515 dbgpt-0.5.5/dbgpt/client/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      154 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/client/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7280 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/client/_cli.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1413 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/client/app.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    14335 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/client/client.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3784 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/client/datasource.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3568 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/client/flow.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7003 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/client/knowledge.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9487 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/client/schema.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    10759 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/component.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.545515 dbgpt-0.5.5/dbgpt/configs/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      530 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/configs/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    10760 2024-04-23 06:52:33.000000 dbgpt-0.5.5/dbgpt/configs/model_config.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.545515 dbgpt-0.5.5/dbgpt/core/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2672 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.545515 dbgpt-0.5.5/dbgpt/core/_private/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        0 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/core/_private/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1225 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/core/_private/example_base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3753 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/core/_private/prompt_registry.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.545515 dbgpt-0.5.5/dbgpt/core/awel/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6061 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/awel/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.549515 dbgpt-0.5.5/dbgpt/core/awel/dag/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       26 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/core/awel/dag/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    29536 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/dag/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4143 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/awel/dag/dag_manager.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3309 2024-02-29 10:48:49.000000 dbgpt-0.5.5/dbgpt/core/awel/dag/loader.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.549515 dbgpt-0.5.5/dbgpt/core/awel/flow/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      752 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/flow/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    33942 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/awel/flow/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1084 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/flow/compat.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1577 2024-02-21 03:05:44.000000 dbgpt-0.5.5/dbgpt/core/awel/flow/exceptions.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    29039 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/awel/flow/flow_factory.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.549515 dbgpt-0.5.5/dbgpt/core/awel/operators/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       30 2024-01-23 06:56:58.000000 dbgpt-0.5.5/dbgpt/core/awel/operators/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    11174 2024-04-20 02:09:18.000000 dbgpt-0.5.5/dbgpt/core/awel/operators/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    11132 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/operators/common_operator.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4262 2024-02-23 04:07:33.000000 dbgpt-0.5.5/dbgpt/core/awel/operators/stream_operator.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.549515 dbgpt-0.5.5/dbgpt/core/awel/resource/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       58 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/core/awel/resource/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      413 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/core/awel/resource/base.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.549515 dbgpt-0.5.5/dbgpt/core/awel/runner/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      118 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/core/awel/runner/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4203 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/runner/job_manager.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7648 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/runner/local_runner.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.553515 dbgpt-0.5.5/dbgpt/core/awel/task/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       26 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/core/awel/task/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    14271 2024-04-20 02:09:18.000000 dbgpt-0.5.5/dbgpt/core/awel/task/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    20591 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/task/task_impl.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.553515 dbgpt-0.5.5/dbgpt/core/awel/trigger/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       34 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/core/awel/trigger/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      519 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/trigger/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6462 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/trigger/ext_http_trigger.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    37988 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/awel/trigger/http_trigger.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6040 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/trigger/iterator_trigger.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7886 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/awel/trigger/trigger_manager.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.553515 dbgpt-0.5.5/dbgpt/core/awel/util/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       22 2024-02-21 03:05:44.000000 dbgpt-0.5.5/dbgpt/core/awel/util/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      228 2024-02-21 03:05:44.000000 dbgpt-0.5.5/dbgpt/core/awel/util/_typing_util.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      500 2024-02-21 03:05:44.000000 dbgpt-0.5.5/dbgpt/core/awel/util/http_util.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2328 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/awel/util/parameter_util.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.557515 dbgpt-0.5.5/dbgpt/core/interface/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      102 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/core/interface/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3546 2024-01-29 10:49:25.000000 dbgpt-0.5.5/dbgpt/core/interface/cache.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1018 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/interface/embeddings.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7410 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/interface/evaluation.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3818 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/interface/knowledge.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    31110 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/interface/llm.py
--rwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)    42803 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/interface/message.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.557515 dbgpt-0.5.5/dbgpt/core/interface/operators/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       55 2024-01-23 06:56:58.000000 dbgpt-0.5.5/dbgpt/core/interface/operators/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4438 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/interface/operators/composer_operator.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    18962 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/interface/operators/llm_operator.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    23685 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/interface/operators/message_operator.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    16465 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/interface/operators/prompt_operator.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      767 2024-01-23 06:56:58.000000 dbgpt-0.5.5/dbgpt/core/interface/operators/retriever.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    10805 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/interface/output_parser.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    26575 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/interface/prompt.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1748 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/interface/serialization.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    15126 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/interface/storage.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.557515 dbgpt-0.5.5/dbgpt/core/operators/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1509 2024-02-21 03:05:44.000000 dbgpt-0.5.5/dbgpt/core/operators/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.557515 dbgpt-0.5.5/dbgpt/core/operators/flow/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      340 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/operators/flow/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9546 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/operators/flow/composer_operator.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2601 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/operators/flow/dict_operator.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.561514 dbgpt-0.5.5/dbgpt/core/schema/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       33 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/core/schema/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8246 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/core/schema/api.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.561514 dbgpt-0.5.5/dbgpt/datasource/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      412 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6802 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/datasource/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3909 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/conn_spark.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4454 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/datasource/conn_tugraph.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      923 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/db_conn_info.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.561514 dbgpt-0.5.5/dbgpt/datasource/manages/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      157 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/manages/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9173 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/manages/connect_config_db.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8623 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/datasource/manages/connector_manager.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.561514 dbgpt-0.5.5/dbgpt/datasource/nosql/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       33 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/nosql/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.561514 dbgpt-0.5.5/dbgpt/datasource/operators/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      128 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/operators/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      770 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/operators/datasource_operator.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.565515 dbgpt-0.5.5/dbgpt/datasource/rdbms/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       30 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    23230 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    12710 2024-04-23 06:52:33.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_clickhouse.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6407 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_doris.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2473 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_duckdb.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1417 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_hive.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1329 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_mssql.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      295 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_mysql.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8185 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_postgresql.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9677 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_sqlite.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5681 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_starrocks.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.565515 dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       33 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.565515 dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/starrocks/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      648 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.565515 dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      820 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3186 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7507 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      116 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/datasource/redis.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.565515 dbgpt-0.5.5/dbgpt/model/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      320 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.569515 dbgpt-0.5.5/dbgpt/model/adapter/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        0 2023-12-22 17:31:06.000000 dbgpt-0.5.5/dbgpt/model/adapter/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    19868 2024-01-16 06:29:48.000000 dbgpt-0.5.5/dbgpt/model/adapter/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3071 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/adapter/embeddings_loader.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8687 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/model/adapter/fschat_adapter.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    11521 2024-04-23 06:52:33.000000 dbgpt-0.5.5/dbgpt/model/adapter/hf_adapter.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    15595 2024-01-22 13:19:20.000000 dbgpt-0.5.5/dbgpt/model/adapter/loader.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5520 2024-01-16 06:29:48.000000 dbgpt-0.5.5/dbgpt/model/adapter/model_adapter.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    17037 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/adapter/old_adapter.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9783 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/adapter/proxy_adapter.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3587 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/model/adapter/template.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3495 2024-01-13 14:22:44.000000 dbgpt-0.5.5/dbgpt/model/adapter/vllm_adapter.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3050 2024-02-29 10:48:49.000000 dbgpt-0.5.5/dbgpt/model/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    13971 2024-01-13 14:22:45.000000 dbgpt-0.5.5/dbgpt/model/cli.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.569515 dbgpt-0.5.5/dbgpt/model/operators/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      341 2024-01-23 06:56:58.000000 dbgpt-0.5.5/dbgpt/model/operators/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4981 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/operators/llm_operator.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    18163 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/parameter.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.569515 dbgpt-0.5.5/dbgpt/model/proxy/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1013 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/proxy/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7967 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/model/proxy/base.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.573515 dbgpt-0.5.5/dbgpt/model/proxy/llms/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      306 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3077 2024-01-16 06:29:48.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/baichuan.py
--rwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)     2325 2024-01-16 06:29:48.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/bard.py
--rwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)    10636 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/chatgpt.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      200 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/claude.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6485 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/gemini.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3336 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/moonshot.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1350 2024-01-16 06:29:48.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/proxy_model.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7602 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/spark.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3720 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/tongyi.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7011 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/wenxin.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2859 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/yi.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3796 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/model/proxy/llms/zhipu.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.573515 dbgpt-0.5.5/dbgpt/model/utils/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        0 2023-12-23 08:34:19.000000 dbgpt-0.5.5/dbgpt/model/utils/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9274 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/model/utils/chatgpt_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2365 2024-01-22 13:19:20.000000 dbgpt-0.5.5/dbgpt/model/utils/llm_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3101 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/model/utils/token_utils.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.573515 dbgpt-0.5.5/dbgpt/rag/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      200 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.577515 dbgpt-0.5.5/dbgpt/rag/assembler/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      431 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/assembler/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2648 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/assembler/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4815 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/assembler/db_schema.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4199 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/assembler/embedding.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4611 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/assembler/summary.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6792 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/chunk_manager.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.577515 dbgpt-0.5.5/dbgpt/rag/embedding/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      725 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/embedding/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1167 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/embedding/_wrapped.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8826 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/embedding/embedding_factory.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    24993 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/rag/embedding/embeddings.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.577515 dbgpt-0.5.5/dbgpt/rag/evaluation/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      271 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/evaluation/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8772 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/rag/evaluation/retriever.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.577515 dbgpt-0.5.5/dbgpt/rag/extractor/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      152 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/extractor/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1314 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/extractor/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6352 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/extractor/summary.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.577515 dbgpt-0.5.5/dbgpt/rag/graph/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       28 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/graph/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.581514 dbgpt-0.5.5/dbgpt/rag/knowledge/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1338 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5582 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3541 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/csv.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2389 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/datasource.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2580 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/docx.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6600 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/factory.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3024 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/html.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       22 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/json.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2600 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/markdown.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3378 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/pdf.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2886 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/pptx.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1807 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/string.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2504 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/txt.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2143 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/knowledge/url.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.585514 dbgpt-0.5.5/dbgpt/rag/operators/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      971 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      654 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/assembler.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      743 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/datasource.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2956 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/db_schema.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6584 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/embedding.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2085 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/evaluation.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4534 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/knowledge.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1268 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/rerank.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3199 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/rewrite.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1466 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/schema_linking.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4156 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/operators/summary.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.585514 dbgpt-0.5.5/dbgpt/rag/retriever/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      503 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/retriever/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4107 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/retriever/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7270 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/retriever/db_schema.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8548 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/retriever/embedding.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7113 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/rag/retriever/rerank.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5223 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/retriever/rewrite.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.585514 dbgpt-0.5.5/dbgpt/rag/schemalinker/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       30 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/schemalinker/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1624 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/schemalinker/base_linker.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3392 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/schemalinker/schema_linking.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.589515 dbgpt-0.5.5/dbgpt/rag/summary/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      420 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/summary/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1226 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/summary/db_summary.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5210 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/rag/summary/db_summary_client.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4575 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/rag/summary/gdbms_db_summary.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4443 2024-04-13 17:42:32.000000 dbgpt-0.5.5/dbgpt/rag/summary/rdbms_db_summary.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.589515 dbgpt-0.5.5/dbgpt/rag/text_splitter/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      539 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/text_splitter/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1497 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/rag/text_splitter/pre_text_splitter.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    32461 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/rag/text_splitter/text_splitter.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6913 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/rag/text_splitter/token_splitter.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.589515 dbgpt-0.5.5/dbgpt/storage/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       67 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.589515 dbgpt-0.5.5/dbgpt/storage/cache/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      384 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/cache/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       24 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/cache/embedding_cache.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6185 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/cache/llm_cache.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4472 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/cache/manager.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9995 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/cache/operators.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.589515 dbgpt-0.5.5/dbgpt/storage/cache/protocol/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       27 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/cache/protocol/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.589515 dbgpt-0.5.5/dbgpt/storage/cache/storage/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       47 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/cache/storage/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8913 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/cache/storage/base.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.593515 dbgpt-0.5.5/dbgpt/storage/cache/storage/disk/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       41 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/cache/storage/disk/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3254 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/cache/storage/disk/disk_storage.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.593515 dbgpt-0.5.5/dbgpt/storage/chat_history/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      438 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/chat_history/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4736 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/chat_history/chat_history_db.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5829 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/chat_history/storage_adapter.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.593515 dbgpt-0.5.5/dbgpt/storage/metadata/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      476 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/metadata/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9345 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/storage/metadata/_base_dao.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1041 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/metadata/db_factory.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    18854 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/metadata/db_manager.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5503 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/metadata/db_storage.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1892 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/storage/schema.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.597514 dbgpt-0.5.5/dbgpt/storage/vector_store/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1173 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/storage/vector_store/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7923 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/storage/vector_store/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8233 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/storage/vector_store/chroma_store.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6622 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/storage/vector_store/connector.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1234 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/storage/vector_store/filters.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    21293 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/storage/vector_store/milvus_store.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    29140 2024-04-26 06:17:48.000000 dbgpt-0.5.5/dbgpt/storage/vector_store/oceanbase_store.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3440 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/storage/vector_store/pgvector_store.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     6727 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/storage/vector_store/weaviate_store.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.605514 dbgpt-0.5.5/dbgpt/util/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      413 2024-01-13 14:22:45.000000 dbgpt-0.5.5/dbgpt/util/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    14058 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/_db_migration_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2868 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/util/annotations.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     4659 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/api_utils.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.605514 dbgpt-0.5.5/dbgpt/util/benchmarks/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        0 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/util/benchmarks/__init__.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.605514 dbgpt-0.5.5/dbgpt/util/benchmarks/llm/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        0 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/util/benchmarks/llm/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    10778 2024-01-13 14:22:45.000000 dbgpt-0.5.5/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9317 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/util/benchmarks/llm/llm_benchmarks.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1703 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/chat_util.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    19203 2023-12-27 13:40:23.000000 dbgpt-0.5.5/dbgpt/util/code_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5840 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/command_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1791 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/util/config_utils.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.605514 dbgpt-0.5.5/dbgpt/util/console/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       70 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/console/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1827 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/console/console.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      780 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/custom_data_structure.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      247 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/date_utils.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.605514 dbgpt-0.5.5/dbgpt/util/dbgpts/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        0 2024-02-21 03:05:44.000000 dbgpt-0.5.5/dbgpt/util/dbgpts/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1936 2024-02-29 10:48:49.000000 dbgpt-0.5.5/dbgpt/util/dbgpts/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5982 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/dbgpts/cli.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    11198 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/util/dbgpts/loader.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    11883 2024-04-15 06:23:33.000000 dbgpt-0.5.5/dbgpt/util/dbgpts/repo.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    10560 2024-04-15 06:23:33.000000 dbgpt-0.5.5/dbgpt/util/dbgpts/template.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      533 2023-12-27 13:40:23.000000 dbgpt-0.5.5/dbgpt/util/error_types.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2886 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/executor_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3929 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/util/fastapi.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1807 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/util/formatting.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3340 2024-02-23 04:07:33.000000 dbgpt-0.5.5/dbgpt/util/function_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    12937 2024-01-13 14:22:45.000000 dbgpt-0.5.5/dbgpt/util/global_helper.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1976 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/i18n_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3673 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/json_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      238 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/memory_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2679 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/model_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      893 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/module_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      704 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/net_utils.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.605514 dbgpt-0.5.5/dbgpt/util/network/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/network/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     9818 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/util/network/_cli.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3488 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/openai_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      618 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/util/pagination_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    27652 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/parameter_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      105 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/util/path_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      629 2024-02-29 10:48:49.000000 dbgpt-0.5.5/dbgpt/util/pd_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     8747 2024-04-20 06:22:55.000000 dbgpt-0.5.5/dbgpt/util/prompt_util.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1676 2024-04-16 08:18:45.000000 dbgpt-0.5.5/dbgpt/util/retry.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.609514 dbgpt-0.5.5/dbgpt/util/serialization/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        0 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/util/serialization/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1859 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/serialization/json_serialization.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1219 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/similarity_util.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      697 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/util/singleton.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.609514 dbgpt-0.5.5/dbgpt/util/speech/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        0 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/util/speech/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1119 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/util/speech/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1180 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/util/speech/brian.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2985 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/speech/eleven_labs.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      467 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/util/speech/gtts.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      523 2023-12-08 06:49:37.000000 dbgpt-0.5.5/dbgpt/util/speech/macos_tts.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1441 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/speech/say.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     2526 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/splitter_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3006 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/string_utils.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7537 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/system_utils.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.609514 dbgpt-0.5.5/dbgpt/util/tracer/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      723 2024-01-13 14:22:45.000000 dbgpt-0.5.5/dbgpt/util/tracer/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7264 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/tracer/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5743 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/tracer/span_storage.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    18465 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/tracer/tracer_cli.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     7846 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/util/tracer/tracer_impl.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1504 2024-01-10 02:49:00.000000 dbgpt-0.5.5/dbgpt/util/tracer/tracer_middleware.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5246 2024-01-17 03:48:33.000000 dbgpt-0.5.5/dbgpt/util/utils.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.609514 dbgpt-0.5.5/dbgpt/vis/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      602 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1050 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/base.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1220 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/client.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.613515 dbgpt-0.5.5/dbgpt/vis/tags/
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       16 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/tags/__init__.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      284 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/tags/vis_agent_message.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      257 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/tags/vis_agent_plans.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     3080 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/tags/vis_chart.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      256 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/tags/vis_code.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     1957 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/tags/vis_dashboard.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      258 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/tags/vis_gpts_execution.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      311 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/tags/vis_gpts_result.py
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)      253 2024-04-13 17:42:28.000000 dbgpt-0.5.5/dbgpt/vis/tags/vis_plugin.py
-drwxrwxr-x   0 staneyffer  (1000) staneyffer  (1000)        0 2024-04-26 06:29:52.525515 dbgpt-0.5.5/dbgpt.egg-info/
--rw-r--r--   0 staneyffer  (1000) staneyffer  (1000)    31236 2024-04-26 06:29:52.000000 dbgpt-0.5.5/dbgpt.egg-info/PKG-INFO
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    12775 2024-04-26 06:29:52.000000 dbgpt-0.5.5/dbgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        1 2024-04-26 06:29:52.000000 dbgpt-0.5.5/dbgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       53 2024-04-26 06:29:52.000000 dbgpt-0.5.5/dbgpt.egg-info/entry_points.txt
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)     5103 2024-04-26 06:29:52.000000 dbgpt-0.5.5/dbgpt.egg-info/requires.txt
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)        6 2024-04-26 06:29:52.000000 dbgpt-0.5.5/dbgpt.egg-info/top_level.txt
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)       38 2024-04-26 06:29:52.677514 dbgpt-0.5.5/setup.cfg
--rw-rw-r--   0 staneyffer  (1000) staneyffer  (1000)    24277 2024-04-26 06:29:46.000000 dbgpt-0.5.5/setup.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.085496 dbgpt-0.5.5rc0/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.5rc0/LICENSE
+-rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.5rc0/MANIFEST.in
+-rw-r--r--   0 staneyffer   (501) staff       (20)    30253 2024-04-18 03:05:22.084796 dbgpt-0.5.5rc0/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11946 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/README.md
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.797715 dbgpt-0.5.5rc0/dbgpt/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.801427 dbgpt-0.5.5rc0/dbgpt/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14183 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/_private/config.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1693 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/_private/llm_metadata.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2234 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/_private/pydantic.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-04-10 15:09:52.000000 dbgpt-0.5.5rc0/dbgpt/_version.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.801728 dbgpt-0.5.5rc0/dbgpt/agent/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1125 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/agent/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.806821 dbgpt-0.5.5rc0/dbgpt/agent/actions/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5354 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      890 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/blank_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3746 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/chart_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5097 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/code_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4461 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/dashboard_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5443 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/indicator_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5491 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/plugin_action.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.810930 dbgpt-0.5.5rc0/dbgpt/agent/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9497 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5364 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/agent_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    35815 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/base_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5544 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/base_team.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.812142 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3473 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6745 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm_client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.813235 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1291 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/priority.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3715 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/role.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      456 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      466 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/user_proxy_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.817278 dbgpt-0.5.5rc0/dbgpt/agent/expand/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1675 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/Indicator_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7025 2024-04-16 17:14:04.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/code_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2207 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/dashboard_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5415 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/data_scientist_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2715 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/plugin_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22055 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1685 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/summary_assistant_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.819411 dbgpt-0.5.5rc0/dbgpt/agent/memory/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       32 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6850 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5803 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/default_gpts_memory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7170 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/gpts_memory.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.821740 dbgpt-0.5.5rc0/dbgpt/agent/plan/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      914 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.823998 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       60 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10852 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6014 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator_resource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8258 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/team_awel_layout.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4732 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/plan_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7582 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/planner_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12459 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/team_auto_plan.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.825803 dbgpt-0.5.5rc0/dbgpt/agent/plugin/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      214 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.827682 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       23 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.828088 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       36 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.830121 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       88 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10775 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      687 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1188 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5226 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22485 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1166 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/generator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1240 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7625 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/plugins_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.832787 dbgpt-0.5.5rc0/dbgpt/agent/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      665 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3721 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_db_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      782 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_knowledge_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3224 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_plugin_api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.834142 dbgpt-0.5.5rc0/dbgpt/agent/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      114 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/agent/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      850 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/util/cmp.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.835035 dbgpt-0.5.5rc0/dbgpt/cli/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/cli/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5794 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/cli/cli_scripts.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.838920 dbgpt-0.5.5rc0/dbgpt/client/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.5rc0/dbgpt/client/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-04-17 10:27:40.000000 dbgpt-0.5.5rc0/dbgpt/client/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.5rc0/dbgpt/client/app.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14335 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3784 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3568 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/flow.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7003 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9487 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10759 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/component.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.839908 dbgpt-0.5.5rc0/dbgpt/configs/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/configs/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10186 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/configs/model_config.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.840591 dbgpt-0.5.5rc0/dbgpt/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2672 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.842026 dbgpt-0.5.5rc0/dbgpt/core/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/_private/example_base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/_private/prompt_registry.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.842690 dbgpt-0.5.5rc0/dbgpt/core/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6061 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.845836 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4143 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/dag_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3309 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/loader.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.849896 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    33942 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1084 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/compat.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29039 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/flow_factory.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.852865 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11154 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11132 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/common_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/stream_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.854341 dbgpt-0.5.5rc0/dbgpt/core/awel/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/resource/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.856561 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/job_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/local_runner.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.859147 dbgpt-0.5.5rc0/dbgpt/core/awel/task/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/task/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14193 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/task/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/task/task_impl.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.863491 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6462 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/ext_http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    37988 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/iterator_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/trigger_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.866415 dbgpt-0.5.5rc0/dbgpt/core/awel/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/_typing_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/http_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2328 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/parameter_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.873538 dbgpt-0.5.5rc0/dbgpt/core/interface/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1018 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/embeddings.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3818 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31110 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/llm.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    42803 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/message.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.878118 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/message_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    16465 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/prompt_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/retriever.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10805 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/output_parser.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    26575 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/prompt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1748 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15126 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.878848 dbgpt-0.5.5rc0/dbgpt/core/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.881201 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/dict_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.882453 dbgpt-0.5.5rc0/dbgpt/core/schema/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/schema/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8246 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/schema/api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.885625 dbgpt-0.5.5rc0/dbgpt/datasource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6653 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/conn_spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/db_conn_info.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.887735 dbgpt-0.5.5rc0/dbgpt/datasource/manages/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/manages/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9173 2024-03-28 01:32:30.000000 dbgpt-0.5.5rc0/dbgpt/datasource/manages/connect_config_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8392 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/manages/connector_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.888451 dbgpt-0.5.5rc0/dbgpt/datasource/nosql/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/nosql/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.889918 dbgpt-0.5.5rc0/dbgpt/datasource/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-28 01:32:23.000000 dbgpt-0.5.5rc0/dbgpt/datasource/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/operators/datasource_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.897610 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12585 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_clickhouse.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_doris.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_duckdb.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_hive.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_mssql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_mysql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_postgresql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9677 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_sqlite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_starrocks.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.898231 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.898831 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.900469 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/redis.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.903268 dbgpt-0.5.5rc0/dbgpt/model/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.912503 dbgpt-0.5.5rc0/dbgpt/model/adapter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19868 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3071 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/embeddings_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/fschat_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9327 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/hf_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5520 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/model_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    17037 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/old_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9783 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/proxy_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/vllm_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/cli.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.914015 dbgpt-0.5.5rc0/dbgpt/model/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/model/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18163 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/parameter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.915211 dbgpt-0.5.5rc0/dbgpt/model/proxy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1013 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.923920 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/baichuan.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/bard.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    10636 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/chatgpt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/claude.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/gemini.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3336 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/moonshot.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/proxy_model.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/tongyi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/wenxin.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/yi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/zhipu.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.926322 dbgpt-0.5.5rc0/dbgpt/model/utils/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/chatgpt_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/llm_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/token_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.927912 dbgpt-0.5.5rc0/dbgpt/rag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.931570 dbgpt-0.5.5rc0/dbgpt/rag/assembler/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2648 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4199 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/chunk_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.934462 dbgpt-0.5.5rc0/dbgpt/rag/embedding/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      725 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1167 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/_wrapped.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8826 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/embedding_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    24261 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/embeddings.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.935766 dbgpt-0.5.5rc0/dbgpt/rag/evaluation/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/evaluation/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/evaluation/retriever.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.938265 dbgpt-0.5.5rc0/dbgpt/rag/extractor/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/extractor/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/extractor/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/extractor/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.938914 dbgpt-0.5.5rc0/dbgpt/rag/graph/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/graph/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.947645 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1338 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5582 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3541 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/csv.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2131 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2580 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/docx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6600 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3024 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/html.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/json.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2600 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/markdown.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3378 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pdf.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pptx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/string.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2504 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/txt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2143 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/url.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.953454 dbgpt-0.5.5rc0/dbgpt/rag/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/assembler.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-28 01:32:23.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/rewrite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/schema_linking.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.957440 dbgpt-0.5.5rc0/dbgpt/rag/retriever/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4107 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7270 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8548 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4242 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/rewrite.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.959293 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/base_linker.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/schema_linking.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.961655 dbgpt-0.5.5rc0/dbgpt/rag/summary/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4057 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary_client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-13 17:38:21.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/rdbms_db_summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.964496 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/pre_text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31787 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/token_splitter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.965560 dbgpt-0.5.5rc0/dbgpt/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.973084 dbgpt-0.5.5rc0/dbgpt/storage/cache/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/embedding_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/llm_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-04-17 10:41:53.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/operators.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.973881 dbgpt-0.5.5rc0/dbgpt/storage/cache/protocol/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/protocol/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.975078 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.976473 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/disk_storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.978356 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/chat_history_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/storage_adapter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.982178 dbgpt-0.5.5rc0/dbgpt/storage/metadata/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9345 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/_base_dao.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1860 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/schema.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.986115 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      960 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7923 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8233 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/chroma_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6622 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/connector.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1234 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/filters.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    21288 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/milvus_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3440 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/pgvector_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6727 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/weaviate_store.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.010463 dbgpt-0.5.5rc0/dbgpt/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/_db_migration_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2868 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/annotations.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/api_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.011350 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.013055 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9317 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/chat_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19203 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/code_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-04-12 06:30:46.000000 dbgpt-0.5.5rc0/dbgpt/util/command_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/config_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.014455 dbgpt-0.5.5rc0/dbgpt/util/console/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/util/console/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/util/console/console.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/custom_data_structure.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      247 2024-04-09 19:22:04.000000 dbgpt-0.5.5rc0/dbgpt/util/date_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.019006 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1936 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11198 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11883 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/repo.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10560 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/error_types.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/executor_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3929 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/fastapi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/formatting.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3340 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/function_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/global_helper.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/util/i18n_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3673 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/util/json_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/memory_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/model_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/module_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/net_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.020208 dbgpt-0.5.5rc0/dbgpt/util/network/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/util/network/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9818 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/network/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/openai_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      618 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/pagination_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    27652 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/parameter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/path_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/pd_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8747 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/prompt_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1676 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/retry.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.021012 dbgpt-0.5.5rc0/dbgpt/util/serialization/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/serialization/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-04-17 10:39:42.000000 dbgpt-0.5.5rc0/dbgpt/util/serialization/json_serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/similarity_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/singleton.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.025755 dbgpt-0.5.5rc0/dbgpt/util/speech/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/brian.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/eleven_labs.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/gtts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/macos_tts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/say.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/splitter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3006 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/util/string_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/util/system_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.030555 dbgpt-0.5.5rc0/dbgpt/util/tracer/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7264 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5743 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/span_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7846 2024-04-17 04:06:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_impl.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_middleware.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.032504 dbgpt-0.5.5rc0/dbgpt/vis/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      602 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/vis/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1050 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.038159 dbgpt-0.5.5rc0/dbgpt/vis/tags/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       16 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      284 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_agent_message.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      257 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_agent_plans.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3080 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_chart.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      256 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_code.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1957 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_dashboard.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      258 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_gpts_execution.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      311 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_gpts_result.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      253 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_plugin.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.799891 dbgpt-0.5.5rc0/dbgpt.egg-info/
+-rw-r--r--   0 staneyffer   (501) staff       (20)    30253 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12658 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/entry_points.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4987 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/requires.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/top_level.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-04-18 03:05:22.085629 dbgpt-0.5.5rc0/setup.cfg
+-rw-r--r--   0 staneyffer   (501) staff       (20)    24009 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/setup.py
```

### Comparing `dbgpt-0.5.5/LICENSE` & `dbgpt-0.5.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/PKG-INFO` & `dbgpt-0.5.5rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.5
+Version: 0.5.5rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -13,406 +13,393 @@
 Requires-Dist: chardet==5.1.0
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: cachetools
 Requires-Dist: pydantic>=2.6.0
 Requires-Dist: typeguard
 Provides-Extra: core
+Requires-Dist: chardet==5.1.0; extra == "core"
+Requires-Dist: importlib-resources==5.12.0; extra == "core"
 Requires-Dist: cachetools; extra == "core"
+Requires-Dist: typeguard; extra == "core"
 Requires-Dist: aiohttp==3.8.4; extra == "core"
 Requires-Dist: python-dotenv==1.0.0; extra == "core"
 Requires-Dist: pydantic>=2.6.0; extra == "core"
-Requires-Dist: importlib-resources==5.12.0; extra == "core"
-Requires-Dist: chardet==5.1.0; extra == "core"
-Requires-Dist: typeguard; extra == "core"
 Provides-Extra: client
+Requires-Dist: chardet==5.1.0; extra == "client"
+Requires-Dist: httpx; extra == "client"
+Requires-Dist: importlib-resources==5.12.0; extra == "client"
 Requires-Dist: fastapi>=0.100.0; extra == "client"
 Requires-Dist: cachetools; extra == "client"
-Requires-Dist: httpx; extra == "client"
+Requires-Dist: typeguard; extra == "client"
 Requires-Dist: aiohttp==3.8.4; extra == "client"
 Requires-Dist: python-dotenv==1.0.0; extra == "client"
 Requires-Dist: pydantic>=2.6.0; extra == "client"
-Requires-Dist: importlib-resources==5.12.0; extra == "client"
-Requires-Dist: chardet==5.1.0; extra == "client"
-Requires-Dist: typeguard; extra == "client"
 Provides-Extra: cli
-Requires-Dist: fastapi>=0.100.0; extra == "cli"
-Requires-Dist: cachetools; extra == "cli"
-Requires-Dist: colorama==0.4.6; extra == "cli"
+Requires-Dist: click; extra == "cli"
+Requires-Dist: chardet==5.1.0; extra == "cli"
 Requires-Dist: httpx; extra == "cli"
 Requires-Dist: tomlkit; extra == "cli"
+Requires-Dist: importlib-resources==5.12.0; extra == "cli"
+Requires-Dist: fastapi>=0.100.0; extra == "cli"
+Requires-Dist: prettytable; extra == "cli"
+Requires-Dist: cachetools; extra == "cli"
+Requires-Dist: typeguard; extra == "cli"
+Requires-Dist: rich; extra == "cli"
+Requires-Dist: psutil==5.9.4; extra == "cli"
 Requires-Dist: aiohttp==3.8.4; extra == "cli"
+Requires-Dist: colorama==0.4.6; extra == "cli"
 Requires-Dist: python-dotenv==1.0.0; extra == "cli"
-Requires-Dist: psutil==5.9.4; extra == "cli"
-Requires-Dist: click; extra == "cli"
-Requires-Dist: rich; extra == "cli"
 Requires-Dist: pydantic>=2.6.0; extra == "cli"
-Requires-Dist: importlib-resources==5.12.0; extra == "cli"
-Requires-Dist: chardet==5.1.0; extra == "cli"
-Requires-Dist: typeguard; extra == "cli"
-Requires-Dist: prettytable; extra == "cli"
 Provides-Extra: agent
-Requires-Dist: fastapi>=0.100.0; extra == "agent"
-Requires-Dist: cachetools; extra == "agent"
-Requires-Dist: colorama==0.4.6; extra == "agent"
+Requires-Dist: click; extra == "agent"
+Requires-Dist: chardet==5.1.0; extra == "agent"
 Requires-Dist: httpx; extra == "agent"
 Requires-Dist: tomlkit; extra == "agent"
-Requires-Dist: aiohttp==3.8.4; extra == "agent"
-Requires-Dist: python-dotenv==1.0.0; extra == "agent"
 Requires-Dist: termcolor; extra == "agent"
+Requires-Dist: importlib-resources==5.12.0; extra == "agent"
+Requires-Dist: fastapi>=0.100.0; extra == "agent"
+Requires-Dist: prettytable; extra == "agent"
+Requires-Dist: cachetools; extra == "agent"
+Requires-Dist: typeguard; extra == "agent"
 Requires-Dist: pandas==2.0.3; extra == "agent"
-Requires-Dist: psutil==5.9.4; extra == "agent"
-Requires-Dist: click; extra == "agent"
 Requires-Dist: rich; extra == "agent"
+Requires-Dist: psutil==5.9.4; extra == "agent"
+Requires-Dist: aiohttp==3.8.4; extra == "agent"
+Requires-Dist: colorama==0.4.6; extra == "agent"
+Requires-Dist: python-dotenv==1.0.0; extra == "agent"
 Requires-Dist: pydantic>=2.6.0; extra == "agent"
-Requires-Dist: importlib-resources==5.12.0; extra == "agent"
-Requires-Dist: chardet==5.1.0; extra == "agent"
-Requires-Dist: typeguard; extra == "agent"
-Requires-Dist: prettytable; extra == "agent"
 Provides-Extra: simple-framework
+Requires-Dist: click; extra == "simple-framework"
 Requires-Dist: fschat; extra == "simple-framework"
-Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
 Requires-Dist: msgpack; extra == "simple-framework"
-Requires-Dist: duckdb; extra == "simple-framework"
-Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
 Requires-Dist: uvicorn; extra == "simple-framework"
+Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
+Requires-Dist: typeguard; extra == "simple-framework"
+Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: duckdb-engine; extra == "simple-framework"
+Requires-Dist: colorama==0.4.6; extra == "simple-framework"
+Requires-Dist: pympler; extra == "simple-framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
+Requires-Dist: jinja2; extra == "simple-framework"
+Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
 Requires-Dist: schedule; extra == "simple-framework"
-Requires-Dist: shortuuid; extra == "simple-framework"
-Requires-Dist: prettytable; extra == "simple-framework"
-Requires-Dist: tomlkit; extra == "simple-framework"
+Requires-Dist: chardet==5.1.0; extra == "simple-framework"
 Requires-Dist: httpx; extra == "simple-framework"
+Requires-Dist: tomlkit; extra == "simple-framework"
+Requires-Dist: cachetools; extra == "simple-framework"
+Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
 Requires-Dist: psutil==5.9.4; extra == "simple-framework"
 Requires-Dist: termcolor; extra == "simple-framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
-Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
-Requires-Dist: click; extra == "simple-framework"
-Requires-Dist: chardet==5.1.0; extra == "simple-framework"
+Requires-Dist: prettytable; extra == "simple-framework"
 Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
-Requires-Dist: cachetools; extra == "simple-framework"
-Requires-Dist: jinja2; extra == "simple-framework"
-Requires-Dist: colorama==0.4.6; extra == "simple-framework"
 Requires-Dist: pandas==2.0.3; extra == "simple-framework"
-Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
-Requires-Dist: duckdb-engine; extra == "simple-framework"
-Requires-Dist: pympler; extra == "simple-framework"
-Requires-Dist: typeguard; extra == "simple-framework"
-Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
+Requires-Dist: duckdb; extra == "simple-framework"
+Requires-Dist: shortuuid; extra == "simple-framework"
 Provides-Extra: framework
+Requires-Dist: click; extra == "framework"
 Requires-Dist: fschat; extra == "framework"
-Requires-Dist: fastapi>=0.100.0; extra == "framework"
 Requires-Dist: msgpack; extra == "framework"
-Requires-Dist: duckdb; extra == "framework"
-Requires-Dist: aiohttp==3.8.4; extra == "framework"
-Requires-Dist: aiofiles; extra == "framework"
 Requires-Dist: uvicorn; extra == "framework"
-Requires-Dist: schedule; extra == "framework"
-Requires-Dist: GitPython; extra == "framework"
-Requires-Dist: shortuuid; extra == "framework"
+Requires-Dist: importlib-resources==5.12.0; extra == "framework"
+Requires-Dist: typeguard; extra == "framework"
+Requires-Dist: rich; extra == "framework"
+Requires-Dist: duckdb-engine; extra == "framework"
 Requires-Dist: pymysql; extra == "framework"
-Requires-Dist: prettytable; extra == "framework"
-Requires-Dist: graphviz; extra == "framework"
-Requires-Dist: tomlkit; extra == "framework"
-Requires-Dist: httpx; extra == "framework"
-Requires-Dist: psutil==5.9.4; extra == "framework"
-Requires-Dist: termcolor; extra == "framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "framework"
+Requires-Dist: colorama==0.4.6; extra == "framework"
+Requires-Dist: pympler; extra == "framework"
+Requires-Dist: alembic==1.12.0; extra == "framework"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
-Requires-Dist: transformers>=4.34.0; extra == "framework"
 Requires-Dist: coloredlogs; extra == "framework"
+Requires-Dist: aiofiles; extra == "framework"
+Requires-Dist: seaborn; extra == "framework"
+Requires-Dist: openpyxl==3.1.2; extra == "framework"
+Requires-Dist: jinja2; extra == "framework"
+Requires-Dist: fastapi>=0.100.0; extra == "framework"
+Requires-Dist: GitPython; extra == "framework"
+Requires-Dist: schedule; extra == "framework"
+Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: httpx; extra == "framework"
+Requires-Dist: tomlkit; extra == "framework"
+Requires-Dist: gTTS==2.3.1; extra == "framework"
+Requires-Dist: cachetools; extra == "framework"
 Requires-Dist: auto-gpt-plugin-template; extra == "framework"
-Requires-Dist: jsonschema; extra == "framework"
+Requires-Dist: transformers>=4.34.0; extra == "framework"
 Requires-Dist: pydantic>=2.6.0; extra == "framework"
-Requires-Dist: click; extra == "framework"
-Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: psutil==5.9.4; extra == "framework"
+Requires-Dist: termcolor; extra == "framework"
+Requires-Dist: prettytable; extra == "framework"
 Requires-Dist: sqlparse==0.4.4; extra == "framework"
-Requires-Dist: cachetools; extra == "framework"
-Requires-Dist: jinja2; extra == "framework"
-Requires-Dist: colorama==0.4.6; extra == "framework"
-Requires-Dist: gTTS==2.3.1; extra == "framework"
-Requires-Dist: seaborn; extra == "framework"
-Requires-Dist: alembic==1.12.0; extra == "framework"
 Requires-Dist: pandas==2.0.3; extra == "framework"
+Requires-Dist: graphviz; extra == "framework"
+Requires-Dist: aiohttp==3.8.4; extra == "framework"
+Requires-Dist: jsonschema; extra == "framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "framework"
 Requires-Dist: xlrd==2.0.1; extra == "framework"
-Requires-Dist: importlib-resources==5.12.0; extra == "framework"
-Requires-Dist: duckdb-engine; extra == "framework"
-Requires-Dist: pympler; extra == "framework"
-Requires-Dist: openpyxl==3.1.2; extra == "framework"
-Requires-Dist: typeguard; extra == "framework"
-Requires-Dist: rich; extra == "framework"
+Requires-Dist: duckdb; extra == "framework"
+Requires-Dist: shortuuid; extra == "framework"
 Provides-Extra: torch
-Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchvision==0.17.1; extra == "torch"
+Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchaudio==2.2.1; extra == "torch"
 Provides-Extra: torch-cpu
-Requires-Dist: torch==2.2.1; extra == "torch-cpu"
 Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
+Requires-Dist: torch==2.2.1; extra == "torch-cpu"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cpu"
 Provides-Extra: torch-cuda
-Requires-Dist: torch==2.2.1; extra == "torch-cuda"
 Requires-Dist: torchvision==0.17.1; extra == "torch-cuda"
+Requires-Dist: torch==2.2.1; extra == "torch-cuda"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cuda"
 Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python; extra == "llama-cpp"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes; extra == "bitsandbytes"
 Provides-Extra: quantization
-Requires-Dist: autoawq; extra == "quantization"
-Requires-Dist: optimum; extra == "quantization"
-Requires-Dist: bitsandbytes; extra == "quantization"
-Requires-Dist: auto-gptq; extra == "quantization"
 Requires-Dist: cpm_kernels; extra == "quantization"
 Provides-Extra: vstore
 Requires-Dist: chromadb>=0.4.22; extra == "vstore"
 Provides-Extra: vstore-weaviate
-Requires-Dist: weaviate-client; extra == "vstore-weaviate"
 Requires-Dist: chromadb>=0.4.22; extra == "vstore-weaviate"
+Requires-Dist: weaviate-client; extra == "vstore-weaviate"
 Provides-Extra: vstore-milvus
-Requires-Dist: chromadb>=0.4.22; extra == "vstore-milvus"
 Requires-Dist: pymilvus; extra == "vstore-milvus"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-milvus"
 Provides-Extra: vstore-all
-Requires-Dist: weaviate-client; extra == "vstore-all"
-Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
 Requires-Dist: pymilvus; extra == "vstore-all"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
+Requires-Dist: weaviate-client; extra == "vstore-all"
 Provides-Extra: datasource
 Requires-Dist: pymysql; extra == "datasource"
 Provides-Extra: datasource-all
 Requires-Dist: pymssql; extra == "datasource-all"
 Requires-Dist: pyspark; extra == "datasource-all"
+Requires-Dist: clickhouse-connect; extra == "datasource-all"
 Requires-Dist: thrift_sasl; extra == "datasource-all"
-Requires-Dist: psycopg2; extra == "datasource-all"
 Requires-Dist: mysqlclient==2.1.0; extra == "datasource-all"
 Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "datasource-all"
 Requires-Dist: pyhive; extra == "datasource-all"
-Requires-Dist: clickhouse-connect; extra == "datasource-all"
 Requires-Dist: pymysql; extra == "datasource-all"
 Requires-Dist: thrift; extra == "datasource-all"
-Requires-Dist: neo4j; extra == "datasource-all"
+Requires-Dist: psycopg2; extra == "datasource-all"
 Provides-Extra: rag
+Requires-Dist: pypdf; extra == "rag"
+Requires-Dist: python-pptx; extra == "rag"
 Requires-Dist: python-docx; extra == "rag"
+Requires-Dist: spacy>=3.7; extra == "rag"
+Requires-Dist: markdown; extra == "rag"
 Requires-Dist: python-multipart; extra == "rag"
+Requires-Dist: sentence-transformers; extra == "rag"
 Requires-Dist: langchain>=0.0.286; extra == "rag"
-Requires-Dist: chromadb>=0.4.22; extra == "rag"
-Requires-Dist: pypdf; extra == "rag"
-Requires-Dist: spacy>=3.7; extra == "rag"
 Requires-Dist: bs4; extra == "rag"
-Requires-Dist: sentence-transformers; extra == "rag"
-Requires-Dist: markdown; extra == "rag"
-Requires-Dist: python-pptx; extra == "rag"
+Requires-Dist: chromadb>=0.4.22; extra == "rag"
 Provides-Extra: openai
+Requires-Dist: click; extra == "openai"
 Requires-Dist: fschat; extra == "openai"
-Requires-Dist: fastapi>=0.100.0; extra == "openai"
 Requires-Dist: msgpack; extra == "openai"
-Requires-Dist: python-multipart; extra == "openai"
-Requires-Dist: duckdb; extra == "openai"
-Requires-Dist: aiohttp==3.8.4; extra == "openai"
-Requires-Dist: aiofiles; extra == "openai"
 Requires-Dist: uvicorn; extra == "openai"
-Requires-Dist: schedule; extra == "openai"
-Requires-Dist: GitPython; extra == "openai"
-Requires-Dist: shortuuid; extra == "openai"
+Requires-Dist: importlib-resources==5.12.0; extra == "openai"
+Requires-Dist: typeguard; extra == "openai"
+Requires-Dist: rich; extra == "openai"
+Requires-Dist: duckdb-engine; extra == "openai"
+Requires-Dist: spacy>=3.7; extra == "openai"
 Requires-Dist: pymysql; extra == "openai"
-Requires-Dist: python-pptx; extra == "openai"
-Requires-Dist: prettytable; extra == "openai"
-Requires-Dist: python-docx; extra == "openai"
-Requires-Dist: graphviz; extra == "openai"
-Requires-Dist: tomlkit; extra == "openai"
-Requires-Dist: httpx; extra == "openai"
-Requires-Dist: chromadb>=0.4.22; extra == "openai"
-Requires-Dist: pypdf; extra == "openai"
-Requires-Dist: psutil==5.9.4; extra == "openai"
-Requires-Dist: tiktoken; extra == "openai"
-Requires-Dist: bs4; extra == "openai"
-Requires-Dist: sentence-transformers; extra == "openai"
 Requires-Dist: markdown; extra == "openai"
-Requires-Dist: termcolor; extra == "openai"
-Requires-Dist: python-dotenv==1.0.0; extra == "openai"
+Requires-Dist: colorama==0.4.6; extra == "openai"
+Requires-Dist: langchain>=0.0.286; extra == "openai"
+Requires-Dist: pympler; extra == "openai"
+Requires-Dist: alembic==1.12.0; extra == "openai"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
-Requires-Dist: transformers>=4.34.0; extra == "openai"
 Requires-Dist: coloredlogs; extra == "openai"
+Requires-Dist: aiofiles; extra == "openai"
+Requires-Dist: pypdf; extra == "openai"
+Requires-Dist: seaborn; extra == "openai"
+Requires-Dist: openpyxl==3.1.2; extra == "openai"
+Requires-Dist: jinja2; extra == "openai"
+Requires-Dist: fastapi>=0.100.0; extra == "openai"
+Requires-Dist: python-multipart; extra == "openai"
+Requires-Dist: bs4; extra == "openai"
+Requires-Dist: GitPython; extra == "openai"
+Requires-Dist: schedule; extra == "openai"
+Requires-Dist: chromadb>=0.4.22; extra == "openai"
+Requires-Dist: chardet==5.1.0; extra == "openai"
+Requires-Dist: httpx; extra == "openai"
+Requires-Dist: tomlkit; extra == "openai"
+Requires-Dist: gTTS==2.3.1; extra == "openai"
+Requires-Dist: python-docx; extra == "openai"
+Requires-Dist: cachetools; extra == "openai"
 Requires-Dist: auto-gpt-plugin-template; extra == "openai"
-Requires-Dist: jsonschema; extra == "openai"
+Requires-Dist: transformers>=4.34.0; extra == "openai"
 Requires-Dist: pydantic>=2.6.0; extra == "openai"
+Requires-Dist: psutil==5.9.4; extra == "openai"
+Requires-Dist: sentence-transformers; extra == "openai"
+Requires-Dist: python-pptx; extra == "openai"
+Requires-Dist: termcolor; extra == "openai"
 Requires-Dist: openai; extra == "openai"
-Requires-Dist: click; extra == "openai"
-Requires-Dist: chardet==5.1.0; extra == "openai"
+Requires-Dist: prettytable; extra == "openai"
 Requires-Dist: sqlparse==0.4.4; extra == "openai"
-Requires-Dist: cachetools; extra == "openai"
-Requires-Dist: jinja2; extra == "openai"
-Requires-Dist: colorama==0.4.6; extra == "openai"
-Requires-Dist: gTTS==2.3.1; extra == "openai"
-Requires-Dist: langchain>=0.0.286; extra == "openai"
-Requires-Dist: seaborn; extra == "openai"
-Requires-Dist: alembic==1.12.0; extra == "openai"
 Requires-Dist: pandas==2.0.3; extra == "openai"
+Requires-Dist: graphviz; extra == "openai"
+Requires-Dist: tiktoken; extra == "openai"
+Requires-Dist: aiohttp==3.8.4; extra == "openai"
+Requires-Dist: jsonschema; extra == "openai"
+Requires-Dist: python-dotenv==1.0.0; extra == "openai"
 Requires-Dist: xlrd==2.0.1; extra == "openai"
-Requires-Dist: spacy>=3.7; extra == "openai"
-Requires-Dist: importlib-resources==5.12.0; extra == "openai"
-Requires-Dist: duckdb-engine; extra == "openai"
-Requires-Dist: pympler; extra == "openai"
-Requires-Dist: openpyxl==3.1.2; extra == "openai"
-Requires-Dist: typeguard; extra == "openai"
-Requires-Dist: rich; extra == "openai"
+Requires-Dist: duckdb; extra == "openai"
+Requires-Dist: shortuuid; extra == "openai"
 Provides-Extra: gpt4all
 Requires-Dist: gpt4all; extra == "gpt4all"
 Provides-Extra: vllm
 Requires-Dist: vllm; extra == "vllm"
 Provides-Extra: cache
 Requires-Dist: rocksdict; extra == "cache"
 Provides-Extra: default
+Requires-Dist: click; extra == "default"
 Requires-Dist: fschat; extra == "default"
-Requires-Dist: fastapi>=0.100.0; extra == "default"
+Requires-Dist: torchaudio==2.2.1; extra == "default"
 Requires-Dist: msgpack; extra == "default"
-Requires-Dist: python-multipart; extra == "default"
-Requires-Dist: zhipuai; extra == "default"
-Requires-Dist: autoawq; extra == "default"
-Requires-Dist: duckdb; extra == "default"
+Requires-Dist: uvicorn; extra == "default"
+Requires-Dist: importlib-resources==5.12.0; extra == "default"
+Requires-Dist: sentencepiece; extra == "default"
+Requires-Dist: typeguard; extra == "default"
+Requires-Dist: rich; extra == "default"
+Requires-Dist: duckdb-engine; extra == "default"
+Requires-Dist: spacy>=3.7; extra == "default"
+Requires-Dist: pymysql; extra == "default"
+Requires-Dist: markdown; extra == "default"
+Requires-Dist: colorama==0.4.6; extra == "default"
 Requires-Dist: rocksdict; extra == "default"
-Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: langchain>=0.0.286; extra == "default"
+Requires-Dist: pympler; extra == "default"
+Requires-Dist: alembic==1.12.0; extra == "default"
+Requires-Dist: torch==2.2.1; extra == "default"
+Requires-Dist: chardet; extra == "default"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
+Requires-Dist: coloredlogs; extra == "default"
 Requires-Dist: aiofiles; extra == "default"
-Requires-Dist: uvicorn; extra == "default"
+Requires-Dist: pypdf; extra == "default"
+Requires-Dist: seaborn; extra == "default"
+Requires-Dist: openpyxl==3.1.2; extra == "default"
+Requires-Dist: jinja2; extra == "default"
+Requires-Dist: fastapi>=0.100.0; extra == "default"
+Requires-Dist: python-multipart; extra == "default"
+Requires-Dist: bs4; extra == "default"
+Requires-Dist: tokenizers>=0.14; extra == "default"
 Requires-Dist: schedule; extra == "default"
 Requires-Dist: GitPython; extra == "default"
-Requires-Dist: bitsandbytes; extra == "default"
-Requires-Dist: shortuuid; extra == "default"
-Requires-Dist: pymysql; extra == "default"
-Requires-Dist: python-pptx; extra == "default"
-Requires-Dist: tokenizers>=0.14; extra == "default"
-Requires-Dist: chardet; extra == "default"
-Requires-Dist: prettytable; extra == "default"
-Requires-Dist: python-docx; extra == "default"
-Requires-Dist: graphviz; extra == "default"
-Requires-Dist: tomlkit; extra == "default"
-Requires-Dist: httpx; extra == "default"
-Requires-Dist: optimum; extra == "default"
 Requires-Dist: chromadb>=0.4.22; extra == "default"
-Requires-Dist: pypdf; extra == "default"
+Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: httpx; extra == "default"
+Requires-Dist: tomlkit; extra == "default"
+Requires-Dist: gTTS==2.3.1; extra == "default"
+Requires-Dist: python-docx; extra == "default"
+Requires-Dist: cachetools; extra == "default"
+Requires-Dist: auto-gpt-plugin-template; extra == "default"
+Requires-Dist: dashscope; extra == "default"
+Requires-Dist: pydantic>=2.6.0; extra == "default"
 Requires-Dist: psutil==5.9.4; extra == "default"
-Requires-Dist: bs4; extra == "default"
-Requires-Dist: auto-gptq; extra == "default"
+Requires-Dist: transformers>=4.34.0; extra == "default"
 Requires-Dist: sentence-transformers; extra == "default"
-Requires-Dist: markdown; extra == "default"
-Requires-Dist: accelerate>=0.20.3; extra == "default"
-Requires-Dist: dashscope; extra == "default"
-Requires-Dist: sentencepiece; extra == "default"
+Requires-Dist: zhipuai; extra == "default"
+Requires-Dist: python-pptx; extra == "default"
+Requires-Dist: cpm_kernels; extra == "default"
 Requires-Dist: termcolor; extra == "default"
-Requires-Dist: python-dotenv==1.0.0; extra == "default"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
-Requires-Dist: transformers>=4.34.0; extra == "default"
-Requires-Dist: coloredlogs; extra == "default"
-Requires-Dist: auto-gpt-plugin-template; extra == "default"
-Requires-Dist: jsonschema; extra == "default"
-Requires-Dist: pydantic>=2.6.0; extra == "default"
-Requires-Dist: click; extra == "default"
-Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: prettytable; extra == "default"
 Requires-Dist: sqlparse==0.4.4; extra == "default"
-Requires-Dist: cachetools; extra == "default"
-Requires-Dist: jinja2; extra == "default"
-Requires-Dist: colorama==0.4.6; extra == "default"
-Requires-Dist: gTTS==2.3.1; extra == "default"
-Requires-Dist: langchain>=0.0.286; extra == "default"
-Requires-Dist: seaborn; extra == "default"
-Requires-Dist: alembic==1.12.0; extra == "default"
+Requires-Dist: accelerate>=0.20.3; extra == "default"
 Requires-Dist: pandas==2.0.3; extra == "default"
-Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: graphviz; extra == "default"
 Requires-Dist: torchvision==0.17.1; extra == "default"
-Requires-Dist: spacy>=3.7; extra == "default"
-Requires-Dist: torchaudio==2.2.1; extra == "default"
-Requires-Dist: cpm_kernels; extra == "default"
-Requires-Dist: torch==2.2.1; extra == "default"
-Requires-Dist: importlib-resources==5.12.0; extra == "default"
-Requires-Dist: duckdb-engine; extra == "default"
-Requires-Dist: pympler; extra == "default"
-Requires-Dist: openpyxl==3.1.2; extra == "default"
-Requires-Dist: typeguard; extra == "default"
-Requires-Dist: rich; extra == "default"
+Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: jsonschema; extra == "default"
+Requires-Dist: python-dotenv==1.0.0; extra == "default"
+Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: duckdb; extra == "default"
+Requires-Dist: shortuuid; extra == "default"
 Provides-Extra: all
-Requires-Dist: fastapi>=0.100.0; extra == "all"
-Requires-Dist: python-multipart; extra == "all"
-Requires-Dist: pyspark; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: rocksdict; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: shortuuid; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: tomlkit; extra == "all"
-Requires-Dist: pypdf; extra == "all"
-Requires-Dist: bs4; extra == "all"
-Requires-Dist: auto-gptq; extra == "all"
-Requires-Dist: markdown; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
-Requires-Dist: openai; extra == "all"
 Requires-Dist: click; extra == "all"
-Requires-Dist: neo4j; extra == "all"
-Requires-Dist: torchvision==0.17.1; extra == "all"
-Requires-Dist: torchaudio==2.2.1; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
-Requires-Dist: thrift; extra == "all"
+Requires-Dist: fschat; extra == "all"
 Requires-Dist: importlib-resources==5.12.0; extra == "all"
+Requires-Dist: typeguard; extra == "all"
+Requires-Dist: thrift; extra == "all"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
 Requires-Dist: gpt4all; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: gTTS==2.3.1; extra == "all"
+Requires-Dist: clickhouse-connect; extra == "all"
+Requires-Dist: dashscope; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: cpm_kernels; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: sqlparse==0.4.4; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
 Requires-Dist: duckdb; extra == "all"
-Requires-Dist: aiohttp==3.8.4; extra == "all"
-Requires-Dist: aiofiles; extra == "all"
+Requires-Dist: shortuuid; extra == "all"
+Requires-Dist: torchaudio==2.2.1; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: markdown; extra == "all"
 Requires-Dist: pymysql; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: python-docx; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: vllm; extra == "all"
-Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: rocksdict; extra == "all"
+Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: pypdf; extra == "all"
+Requires-Dist: openpyxl==3.1.2; extra == "all"
+Requires-Dist: bs4; extra == "all"
 Requires-Dist: chromadb>=0.4.22; extra == "all"
-Requires-Dist: tiktoken; extra == "all"
-Requires-Dist: pymssql; extra == "all"
-Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: pyspark; extra == "all"
 Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: langchain>=0.0.286; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
-Requires-Dist: openpyxl==3.1.2; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: autoawq; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: bitsandbytes; extra == "all"
-Requires-Dist: chardet; extra == "all"
 Requires-Dist: httpx; extra == "all"
-Requires-Dist: optimum; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
+Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: cachetools; extra == "all"
 Requires-Dist: transformers>=4.34.0; extra == "all"
-Requires-Dist: jsonschema; extra == "all"
+Requires-Dist: pymssql; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
+Requires-Dist: aiohttp==3.8.4; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
+Requires-Dist: spacy>=3.7; extra == "all"
+Requires-Dist: pympler; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: fastapi>=0.100.0; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: python-docx; extra == "all"
+Requires-Dist: pyhive; extra == "all"
 Requires-Dist: pydantic>=2.6.0; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: gTTS==2.3.1; extra == "all"
-Requires-Dist: seaborn; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
+Requires-Dist: pandas==2.0.3; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
+Requires-Dist: tiktoken; extra == "all"
 Requires-Dist: xlrd==2.0.1; extra == "all"
-Requires-Dist: schedule; extra == "all"
-Requires-Dist: rich; extra == "all"
-Requires-Dist: fschat; extra == "all"
 Requires-Dist: msgpack; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: termcolor; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
-Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: cachetools; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: rich; extra == "all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
 Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: pyhive; extra == "all"
-Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: spacy>=3.7; extra == "all"
+Requires-Dist: langchain>=0.0.286; extra == "all"
 Requires-Dist: torch==2.2.1; extra == "all"
-Requires-Dist: pympler; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
+Requires-Dist: aiofiles; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: python-multipart; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
+Requires-Dist: vllm; extra == "all"
 Requires-Dist: auto-gpt-plugin-template; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: weaviate-client; extra == "all"
+Requires-Dist: jsonschema; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
 
@@ -566,18 +553,14 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
-    - 🔥🔥🔥  [Qwen1.5-MoE-A2.7B-Chat](https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat)
-    - 🔥🔥🔥  [Meta-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct)
-    - 🔥🔥🔥  [Meta-Llama-3-8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct)
-    - 🔥🔥🔥  [CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat)
     - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
     - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
     - 🔥🔥🔥  [gemma-7b-it](https://huggingface.co/google/gemma-7b-it)
     - 🔥🔥🔥  [gemma-2b-it](https://huggingface.co/google/gemma-2b-it)
     - 🔥🔥🔥  [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)
     - 🔥🔥🔥  [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1)
     - 🔥🔥🔥  [Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)
```

### Comparing `dbgpt-0.5.5/README.md` & `dbgpt-0.5.5rc0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -154,18 +154,14 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
-    - 🔥🔥🔥  [Qwen1.5-MoE-A2.7B-Chat](https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat)
-    - 🔥🔥🔥  [Meta-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct)
-    - 🔥🔥🔥  [Meta-Llama-3-8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct)
-    - 🔥🔥🔥  [CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat)
     - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
     - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
     - 🔥🔥🔥  [gemma-7b-it](https://huggingface.co/google/gemma-7b-it)
     - 🔥🔥🔥  [gemma-2b-it](https://huggingface.co/google/gemma-2b-it)
     - 🔥🔥🔥  [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)
     - 🔥🔥🔥  [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1)
     - 🔥🔥🔥  [Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)
```

#### html2text {}

```diff
@@ -99,45 +99,40 @@
 tuning lightweight framework centred on large language models (LLMs), Text2SQL
 datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework
 simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly
 line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub) - **SMMF
 (Service-oriented Multi-model Management Framework)** We offer extensive model
 support, including dozens of large language models (LLMs) from both open-source
 and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu,
-and many more. - News - ð¥ð¥ð¥ [Qwen1.5-MoE-A2.7B-Chat](https://
-huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat) - ð¥ð¥ð¥ [Meta-Llama-3-70B-
-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct) -
-ð¥ð¥ð¥ [Meta-Llama-3-8B-Instruct](https://huggingface.co/meta-llama/Meta-
-Llama-3-8B-Instruct) - ð¥ð¥ð¥ [CodeQwen1.5-7B-Chat](https://
-huggingface.co/Qwen/CodeQwen1.5-7B-Chat) - ð¥ð¥ð¥ [Qwen1.5-32B-Chat]
-(https://huggingface.co/Qwen/Qwen1.5-32B-Chat) - ð¥ð¥ð¥ [Starling-LM-7B-
-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta) - ð¥ð¥ð¥
-[gemma-7b-it](https://huggingface.co/google/gemma-7b-it) - ð¥ð¥ð¥ [gemma-
-2b-it](https://huggingface.co/google/gemma-2b-it) - ð¥ð¥ð¥ [SOLAR-10.7B]
-(https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0) - ð¥ð¥ð¥
-[Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) -
-ð¥ð¥ð¥ [Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat) -
-ð¥ð¥ð¥ [Yi-34B-Chat](https://huggingface.co/01-ai/Yi-34B-Chat) - [More
-Supported LLMs](http://docs.dbgpt.site/docs/modules/smmf) - **Privacy and
-Security** We ensure the privacy and security of data through the
-implementation of various technologies, including privatized large models and
-proxy desensitization. - Support Datasources - [Datasources](http://
-docs.dbgpt.site/docs/modules/connections) ## Image ð [AutoDL Image](https://
-www.codewithgpu.com/i/eosphoros-ai/DB-GPT/dbgpt) ### Language Switching In the
-.env configuration file, modify the LANGUAGE parameter to switch to different
-languages. The default is English (Chinese: zh, English: en, other languages to
-be added later). ## Contribution - To check detailed guidelines for new
-contributions, please refer [how to contribute](https://github.com/eosphoros-
-ai/DB-GPT/blob/main/CONTRIBUTING.md) ### Contributors Wall _[_h_t_t_p_s_:_/_/
-_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_e_o_s_p_h_o_r_o_s_-_a_i_/_D_B_-_G_P_T_&_m_a_x_=_2_0_0_]## Licence The MIT License
-(MIT) ## Citation If you find `DB-GPT` useful for your research or development,
-please cite the following _p_a_p_e_r: ```bibtex @article{xue2023dbgpt, title={DB-
-GPT: Empowering Database Interactions with Private Large Language Models},
-author={Siqiao Xue and Caigao Jiang and Wenhui Shi and Fangyin Cheng and Keting
-Chen and Hongjun Yang and Zhiping Zhang and Jianshan He and Hongyang Zhang and
+and many more. - News - ð¥ð¥ð¥ [Qwen1.5-32B-Chat](https://huggingface.co/
+Qwen/Qwen1.5-32B-Chat) - ð¥ð¥ð¥ [Starling-LM-7B-beta](https://
+huggingface.co/Nexusflow/Starling-LM-7B-beta) - ð¥ð¥ð¥ [gemma-7b-it]
+(https://huggingface.co/google/gemma-7b-it) - ð¥ð¥ð¥ [gemma-2b-it](https:
+//huggingface.co/google/gemma-2b-it) - ð¥ð¥ð¥ [SOLAR-10.7B](https://
+huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0) - ð¥ð¥ð¥ [Mixtral-8x7B]
+(https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) - ð¥ð¥ð¥
+[Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat) - ð¥ð¥ð¥ [Yi-
+34B-Chat](https://huggingface.co/01-ai/Yi-34B-Chat) - [More Supported LLMs]
+(http://docs.dbgpt.site/docs/modules/smmf) - **Privacy and Security** We ensure
+the privacy and security of data through the implementation of various
+technologies, including privatized large models and proxy desensitization. -
+Support Datasources - [Datasources](http://docs.dbgpt.site/docs/modules/
+connections) ## Image ð [AutoDL Image](https://www.codewithgpu.com/i/
+eosphoros-ai/DB-GPT/dbgpt) ### Language Switching In the .env configuration
+file, modify the LANGUAGE parameter to switch to different languages. The
+default is English (Chinese: zh, English: en, other languages to be added
+later). ## Contribution - To check detailed guidelines for new contributions,
+please refer [how to contribute](https://github.com/eosphoros-ai/DB-GPT/blob/
+main/CONTRIBUTING.md) ### Contributors Wall _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_e_o_s_p_h_o_r_o_s_-_a_i_/_D_B_-_G_P_T_&_m_a_x_=_2_0_0_]## Licence The MIT License (MIT) ##
+Citation If you find `DB-GPT` useful for your research or development, please
+cite the following _p_a_p_e_r: ```bibtex @article{xue2023dbgpt, title={DB-GPT:
+Empowering Database Interactions with Private Large Language Models}, author=
+{Siqiao Xue and Caigao Jiang and Wenhui Shi and Fangyin Cheng and Keting Chen
+and Hongjun Yang and Zhiping Zhang and Jianshan He and Hongyang Zhang and
 Ganglin Wei and Wang Zhao and Fan Zhou and Danrui Qi and Hong Yi and Shaodong
 Liu and Faqiang Chen}, year={2023}, journal={arXiv preprint arXiv:2312.17449},
 url={https://arxiv.org/abs/2312.17449} } ``` ## Contact Information We are
 working on building a community, if you have any ideas for building the
 community, feel free to contact us. [![](https://dcbadge.vercel.app/api/server/
 7uQnPuveTY?compact=true&style=flat)](https://discord.gg/7uQnPuveTY) [![Star
 History Chart](https://api.star-history.com/svg?repos=csunny/DB-GPT&type=Date)]
```

### Comparing `dbgpt-0.5.5/dbgpt/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/_private/config.py` & `dbgpt-0.5.5rc0/dbgpt/_private/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,26 +234,14 @@
         ### Vector Store Configuration
         self.VECTOR_STORE_TYPE = os.getenv("VECTOR_STORE_TYPE", "Chroma")
         self.MILVUS_URL = os.getenv("MILVUS_URL", "127.0.0.1")
         self.MILVUS_PORT = os.getenv("MILVUS_PORT", "19530")
         self.MILVUS_USERNAME = os.getenv("MILVUS_USERNAME", None)
         self.MILVUS_PASSWORD = os.getenv("MILVUS_PASSWORD", None)
 
-        ## OceanBase Configuration
-        self.OB_HOST = os.getenv("OB_HOST", "127.0.0.1")
-        self.OB_PORT = int(os.getenv("OB_PORT", "2881"))
-        self.OB_USER = os.getenv("OB_USER", "root")
-        self.OB_PASSWORD = os.getenv("OB_PASSWORD", "")
-        self.OB_DATABASE = os.getenv("OB_DATABASE", "test")
-        self.OB_SQL_DBG_LOG_PATH = os.getenv("OB_SQL_DBG_LOG_PATH", "")
-        self.OB_ENABLE_NORMALIZE_VECTOR = bool(
-            os.getenv("OB_ENABLE_NORMALIZE_VECTOR", "")
-        )
-        self.OB_ENABLE_INDEX = bool(os.getenv("OB_ENABLE_INDEX", ""))
-
         # QLoRA
         self.QLoRA = os.getenv("QUANTIZE_QLORA", "True")
         self.IS_LOAD_8BIT = os.getenv("QUANTIZE_8bit", "True").lower() == "true"
         self.IS_LOAD_4BIT = os.getenv("QUANTIZE_4bit", "False").lower() == "true"
         if self.IS_LOAD_8BIT and self.IS_LOAD_4BIT:
             self.IS_LOAD_8BIT = False
         # In order to be compatible with the new and old model parameter design
```

### Comparing `dbgpt-0.5.5/dbgpt/_private/llm_metadata.py` & `dbgpt-0.5.5rc0/dbgpt/_private/llm_metadata.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/_private/pydantic.py` & `dbgpt-0.5.5rc0/dbgpt/_private/pydantic.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/actions/action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/actions/blank_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/blank_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/actions/chart_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/chart_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/actions/code_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/code_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/actions/dashboard_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/dashboard_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/actions/indicator_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/indicator_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/actions/plugin_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/plugin_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/core/agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/core/agent_manage.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/agent_manage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/core/base_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/base_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/core/base_team.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/base_team.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/core/llm/llm.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/core/llm/llm_client.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm_client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/core/llm/strategy/priority.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/priority.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/core/role.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/role.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/expand/Indicator_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/Indicator_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/expand/code_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/code_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/expand/dashboard_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/dashboard_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/expand/data_scientist_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/data_scientist_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/expand/plugin_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/plugin_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/expand/retrieve_summary_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/expand/summary_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/summary_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/memory/base.py` & `dbgpt-0.5.5rc0/dbgpt/agent/memory/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/memory/default_gpts_memory.py` & `dbgpt-0.5.5rc0/dbgpt/agent/memory/default_gpts_memory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/memory/gpts_memory.py` & `dbgpt-0.5.5rc0/dbgpt/agent/memory/gpts_memory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plan/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plan/awel/agent_operator.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plan/awel/agent_operator_resource.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator_resource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plan/awel/team_awel_layout.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/team_awel_layout.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plan/plan_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/plan_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plan/planner_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/planner_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plan/team_auto_plan.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/team_auto_plan.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plugin/commands/command.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plugin/commands/command_manage.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command_manage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plugin/commands/exceptions.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plugin/generator.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/generator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plugin/loader.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/plugin/plugins_util.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/plugins_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/resource/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/resource/resource_api.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/resource/resource_db_api.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_db_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/resource/resource_knowledge_api.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_knowledge_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/resource/resource_loader.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/resource/resource_plugin_api.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_plugin_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/agent/util/cmp.py` & `dbgpt-0.5.5rc0/dbgpt/agent/util/cmp.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/cli/cli_scripts.py` & `dbgpt-0.5.5rc0/dbgpt/cli/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/client/_cli.py` & `dbgpt-0.5.5rc0/dbgpt/client/_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/client/app.py` & `dbgpt-0.5.5rc0/dbgpt/client/app.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/client/client.py` & `dbgpt-0.5.5rc0/dbgpt/client/client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/client/datasource.py` & `dbgpt-0.5.5rc0/dbgpt/client/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/client/flow.py` & `dbgpt-0.5.5rc0/dbgpt/client/flow.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/client/knowledge.py` & `dbgpt-0.5.5rc0/dbgpt/client/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/client/schema.py` & `dbgpt-0.5.5rc0/dbgpt/client/schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/component.py` & `dbgpt-0.5.5rc0/dbgpt/component.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/configs/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/configs/model_config.py` & `dbgpt-0.5.5rc0/dbgpt/configs/model_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,18 +68,14 @@
     # https://platform.lingyiwanwu.com/docs/
     "yi_proxyllm": "yi_proxyllm",
     # https://platform.moonshot.cn/docs/
     "moonshot_proxyllm": "moonshot_proxyllm",
     "llama-2-7b": os.path.join(MODEL_PATH, "Llama-2-7b-chat-hf"),
     "llama-2-13b": os.path.join(MODEL_PATH, "Llama-2-13b-chat-hf"),
     "llama-2-70b": os.path.join(MODEL_PATH, "Llama-2-70b-chat-hf"),
-    # https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct
-    "meta-llama-3-8b-instruct": os.path.join(MODEL_PATH, "Meta-Llama-3-8B-Instruct"),
-    # https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct
-    "meta-llama-3-70b-instruct": os.path.join(MODEL_PATH, "Meta-Llama-3-70B-Instruct"),
     "baichuan-13b": os.path.join(MODEL_PATH, "Baichuan-13B-Chat"),
     # please rename "fireballoon/baichuan-vicuna-chinese-7b" to "baichuan-7b"
     "baichuan-7b": os.path.join(MODEL_PATH, "baichuan-7b"),
     "baichuan2-7b": os.path.join(MODEL_PATH, "Baichuan2-7B-Chat"),
     "baichuan2-13b": os.path.join(MODEL_PATH, "Baichuan2-13B-Chat"),
     # https://huggingface.co/Qwen/Qwen-7B-Chat
     "qwen-7b-chat": os.path.join(MODEL_PATH, "Qwen-7B-Chat"),
@@ -108,18 +104,14 @@
     # https://huggingface.co/Qwen/Qwen1.5-1.8B-Chat
     "qwen1.5-1.8b-chat": os.path.join(MODEL_PATH, "Qwen1.5-1.8B-Chat"),
     "qwen1.5-7b-chat": os.path.join(MODEL_PATH, "Qwen1.5-7B-Chat"),
     "qwen1.5-14b-chat": os.path.join(MODEL_PATH, "Qwen1.5-14B-Chat"),
     # https://huggingface.co/Qwen/Qwen1.5-32B-Chat
     "qwen1.5-32b-chat": os.path.join(MODEL_PATH, "Qwen1.5-32B-Chat"),
     "qwen1.5-72b-chat": os.path.join(MODEL_PATH, "Qwen1.5-72B-Chat"),
-    # https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat
-    "codeqwen1.5-7b-chat": os.path.join(MODEL_PATH, "CodeQwen1.5-7B-Chat"),
-    # https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat
-    "qwen1.5-moe-a2.7b-chat": os.path.join(MODEL_PATH, "Qwen1.5-MoE-A2.7B-Chat"),
     # (Llama2 based) We only support WizardLM-13B-V1.2 for now, which is trained from Llama-2 13b, see https://huggingface.co/WizardLM/WizardLM-13B-V1.2
     "wizardlm-13b": os.path.join(MODEL_PATH, "WizardLM-13B-V1.2"),
     # wget https://huggingface.co/TheBloke/vicuna-13B-v1.5-GGUF/resolve/main/vicuna-13b-v1.5.Q4_K_M.gguf -O models/ggml-model-q4_0.gguf
     "llama-cpp": os.path.join(MODEL_PATH, "ggml-model-q4_0.gguf"),
     # https://huggingface.co/internlm/internlm-chat-7b-v1_1, 7b vs 7b-v1.1: https://github.com/InternLM/InternLM/issues/288
     "internlm-7b": os.path.join(MODEL_PATH, "internlm-chat-7b"),
     "internlm-7b-8k": os.path.join(MODEL_PATH, "internlm-chat-7b-8k"),
```

### Comparing `dbgpt-0.5.5/dbgpt/core/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/_private/example_base.py` & `dbgpt-0.5.5rc0/dbgpt/core/_private/example_base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/_private/prompt_registry.py` & `dbgpt-0.5.5rc0/dbgpt/core/_private/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/dag/base.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/dag/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/dag/dag_manager.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/dag/dag_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/dag/loader.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/dag/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/flow/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/flow/base.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/flow/compat.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/compat.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/flow/exceptions.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/flow/flow_factory.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/flow_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/operators/base.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/operators/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     AsyncToSyncIterator,
     BlockingFunction,
     DefaultExecutorFactory,
     blocking_func_to_async,
 )
 
 from ..dag.base import DAG, DAGContext, DAGNode, DAGVar
-from ..task.base import EMPTY_DATA, OUT, T, TaskOutput, is_empty_data
+from ..task.base import EMPTY_DATA, OUT, T, TaskOutput
 
 F = TypeVar("F", bound=FunctionType)
 
 CALL_DATA = Union[Dict[str, Any], Any]
 CURRENT_DAG_CONTEXT: ContextVar[Optional[DAGContext]] = ContextVar(
     "current_dag_context", default=None
 )
@@ -209,15 +209,15 @@
         Args:
             call_data (CALL_DATA): The data pass to root operator node.
             dag_ctx (DAGContext): The context of the DAG when this node is run,
                 Defaults to None.
         Returns:
             OUT: The output of the node after execution.
         """
-        if not is_empty_data(call_data):
+        if call_data != EMPTY_DATA:
             call_data = {"data": call_data}
         out_ctx = await self._runner.execute_workflow(
             self, call_data, exist_dag_ctx=dag_ctx
         )
         return out_ctx.current_task_context.task_output.output
 
     def _blocking_call(
```

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/operators/common_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/operators/common_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/operators/stream_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/operators/stream_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/runner/job_manager.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/runner/job_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/runner/local_runner.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/runner/local_runner.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/task/base.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/task/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,14 @@
 PLACEHOLDER_DATA = _EMPTY_DATA_TYPE("PLACEHOLDER_DATA")
 
 
 def is_empty_data(data: Any):
     """Check if the data is empty."""
     if isinstance(data, _EMPTY_DATA_TYPE):
         return data in (EMPTY_DATA, SKIP_DATA)
-    elif hasattr(data, "empty"):
-        return getattr(data, "empty", False)
     return False
 
 
 MapFunc = Union[Callable[[IN], OUT], Callable[[IN], Awaitable[OUT]]]
 ReduceFunc = Union[Callable[[IN, IN], OUT], Callable[[IN, IN], Awaitable[OUT]]]
 StreamFunc = Callable[[IN], Awaitable[AsyncIterator[OUT]]]
 UnStreamFunc = Callable[[AsyncIterator[IN]], OUT]
```

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/task/task_impl.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/task/task_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/trigger/base.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/trigger/ext_http_trigger.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/ext_http_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/trigger/http_trigger.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/http_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/trigger/iterator_trigger.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/iterator_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/trigger/trigger_manager.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/trigger_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/awel/util/parameter_util.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/util/parameter_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/cache.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/embeddings.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/embeddings.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/evaluation.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/knowledge.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/llm.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/llm.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/message.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/message.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/operators/composer_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/operators/llm_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/operators/message_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/message_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/operators/prompt_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/prompt_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/operators/retriever.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/retriever.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/output_parser.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/output_parser.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/prompt.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/prompt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/serialization.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/interface/storage.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/operators/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/operators/flow/composer_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/operators/flow/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/operators/flow/dict_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/operators/flow/dict_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/core/schema/api.py` & `dbgpt-0.5.5rc0/dbgpt/core/schema/api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/base.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,12 +212,7 @@
         """
         raise NotImplementedError("Current connector does not support get_indexes")
 
     @classmethod
     def is_normal_type(cls) -> bool:
         """Return whether the connector is a normal type."""
         return True
-
-    @classmethod
-    def is_graph_type(cls) -> bool:
-        """Return whether the connector is a graph database connector."""
-        return False
```

### Comparing `dbgpt-0.5.5/dbgpt/datasource/conn_spark.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/conn_spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/db_conn_info.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/db_conn_info.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/manages/connect_config_db.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/manages/connect_config_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/manages/connector_manager.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/manages/connector_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
     def on_init(self):
         """Execute on init.
 
         Load all connector classes.
         """
         from dbgpt.datasource.conn_spark import SparkConnector  # noqa: F401
-        from dbgpt.datasource.conn_tugraph import TuGraphConnector  # noqa: F401
         from dbgpt.datasource.rdbms.base import RDBMSConnector  # noqa: F401
         from dbgpt.datasource.rdbms.conn_clickhouse import (  # noqa: F401
             ClickhouseConnector,
         )
         from dbgpt.datasource.rdbms.conn_doris import DorisConnector  # noqa: F401
         from dbgpt.datasource.rdbms.conn_duckdb import DuckDbConnector  # noqa: F401
         from dbgpt.datasource.rdbms.conn_hive import HiveConnector  # noqa: F401
@@ -182,19 +181,16 @@
             db_info.db_user,
             db_info.db_pwd,
             db_info.comment,
         )
 
     async def async_db_summary_embedding(self, db_name, db_type):
         """Async db summary embedding."""
-        executor = self.system_app.get_component(
-            ComponentType.EXECUTOR_DEFAULT, ExecutorFactory
-        ).create()  # type: ignore
-        executor.submit(self.db_summary_client.db_summary_embedding, db_name, db_type)
-        return True
+        # TODO: async embedding
+        self.db_summary_client.db_summary_embedding(db_name, db_type)
 
     def add_db(self, db_info: DBConfig):
         """Add db connect info.
 
         Args:
             db_info (DBConfig): db connect info.
         """
```

### Comparing `dbgpt-0.5.5/dbgpt/datasource/operators/datasource_operator.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/operators/datasource_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/base.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_clickhouse.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_clickhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,19 +146,14 @@
         """
         fields = self.get_fields(table_name)
         return [
             {"name": name, "comment": comment, "type": column_type}
             for name, column_type, _, _, comment in fields[0]
         ]
 
-    @property
-    def dialect(self) -> str:
-        """Return string representation of dialect to use."""
-        return ""
-
     def get_fields(self, table_name) -> List[Tuple]:
         """Get column fields about specified table."""
         session = self.client
 
         _query_sql = f"""
             SELECT name, type, default_expression, is_in_primary_key, comment
                 from system.columns where table='{table_name}'
```

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_doris.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_doris.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_duckdb.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_duckdb.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_hive.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_hive.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_mssql.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_mssql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_postgresql.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_postgresql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_sqlite.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_sqlite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/conn_starrocks.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_starrocks.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/adapter/base.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/adapter/embeddings_loader.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/embeddings_loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/adapter/fschat_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/fschat_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/adapter/hf_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/hf_adapter.py`

 * *Files 11% similar despite different names*

```diff
@@ -263,83 +263,16 @@
             )
 
     def do_match(self, lower_model_name_or_path: Optional[str] = None):
         return (
             lower_model_name_or_path
             and "qwen" in lower_model_name_or_path
             and "1.5" in lower_model_name_or_path
-            and "moe" not in lower_model_name_or_path
         )
 
 
-class QwenMoeAdapter(NewHFChatModelAdapter):
-    """
-    https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B
-
-    TODO: There are problems with quantization.
-    """
-
-    support_4bit: bool = False
-    support_8bit: bool = False
-
-    def check_transformer_version(self, current_version: str) -> None:
-        print(f"Checking version: Current version {current_version}")
-        if not current_version >= "4.40.0":
-            raise ValueError(
-                "Qwen 1.5 Moe require transformers.__version__>=4.40.0, please upgrade your transformers package."
-            )
-
-    def do_match(self, lower_model_name_or_path: Optional[str] = None):
-        return (
-            lower_model_name_or_path
-            and "qwen" in lower_model_name_or_path
-            and "1.5" in lower_model_name_or_path
-            and "moe" in lower_model_name_or_path
-        )
-
-
-class Llama3Adapter(NewHFChatModelAdapter):
-    """
-    https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct
-    https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct
-    """
-
-    support_4bit: bool = True
-    support_8bit: bool = True
-
-    def do_match(self, lower_model_name_or_path: Optional[str] = None):
-        return lower_model_name_or_path and "llama-3" in lower_model_name_or_path
-
-    def get_str_prompt(
-        self,
-        params: Dict,
-        messages: List[ModelMessage],
-        tokenizer: Any,
-        prompt_template: str = None,
-        convert_to_compatible_format: bool = False,
-    ) -> Optional[str]:
-        str_prompt = super().get_str_prompt(
-            params,
-            messages,
-            tokenizer,
-            prompt_template,
-            convert_to_compatible_format,
-        )
-        terminators = [
-            tokenizer.eos_token_id,
-            tokenizer.convert_tokens_to_ids("<|eot_id|>"),
-        ]
-        exist_token_ids = params.get("stop_token_ids", [])
-        terminators.extend(exist_token_ids)
-        # TODO(fangyinc): We should modify the params in the future
-        params["stop_token_ids"] = terminators
-        return str_prompt
-
-
 register_model_adapter(YiAdapter)
 register_model_adapter(Mixtral8x7BAdapter)
 register_model_adapter(SOLARAdapter)
 register_model_adapter(GemmaAdapter)
 register_model_adapter(StarlingLMAdapter)
 register_model_adapter(QwenAdapter)
-register_model_adapter(QwenMoeAdapter)
-register_model_adapter(Llama3Adapter)
```

### Comparing `dbgpt-0.5.5/dbgpt/model/adapter/loader.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/adapter/model_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/model_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/adapter/old_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/old_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/adapter/proxy_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/proxy_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/adapter/template.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/template.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/adapter/vllm_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/vllm_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/base.py` & `dbgpt-0.5.5rc0/dbgpt/model/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/cli.py` & `dbgpt-0.5.5rc0/dbgpt/model/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/operators/llm_operator.py` & `dbgpt-0.5.5rc0/dbgpt/model/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/parameter.py` & `dbgpt-0.5.5rc0/dbgpt/model/parameter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/base.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/baichuan.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/baichuan.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/bard.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/bard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/chatgpt.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/chatgpt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/gemini.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/gemini.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/moonshot.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/moonshot.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/proxy_model.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/proxy_model.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/spark.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/tongyi.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/wenxin.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/wenxin.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/yi.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/yi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/proxy/llms/zhipu.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/zhipu.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/utils/chatgpt_utils.py` & `dbgpt-0.5.5rc0/dbgpt/model/utils/chatgpt_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/utils/llm_utils.py` & `dbgpt-0.5.5rc0/dbgpt/model/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/model/utils/token_utils.py` & `dbgpt-0.5.5rc0/dbgpt/model/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/assembler/base.py` & `dbgpt-0.5.5rc0/dbgpt/rag/assembler/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/assembler/db_schema.py` & `dbgpt-0.5.5rc0/dbgpt/rag/assembler/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/assembler/embedding.py` & `dbgpt-0.5.5rc0/dbgpt/rag/assembler/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/assembler/summary.py` & `dbgpt-0.5.5rc0/dbgpt/rag/assembler/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/chunk_manager.py` & `dbgpt-0.5.5rc0/dbgpt/rag/chunk_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/embedding/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/rag/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/embedding/_wrapped.py` & `dbgpt-0.5.5rc0/dbgpt/rag/embedding/_wrapped.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/embedding/embedding_factory.py` & `dbgpt-0.5.5rc0/dbgpt/rag/embedding/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/embedding/embeddings.py` & `dbgpt-0.5.5rc0/dbgpt/rag/embedding/embeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,41 +65,39 @@
     """
 
     model_config = ConfigDict(extra=EXTRA_FORBID, protected_namespaces=())
 
     client: Any  #: :meta private:
     model_name: str = DEFAULT_MODEL_NAME
     """Model name to use."""
-    cache_folder: Optional[str] = Field(None, description="Path of the cache folder.")
+    cache_folder: Optional[str] = None
     """Path to store models. Can be also set by SENTENCE_TRANSFORMERS_HOME
     environment variable."""
     model_kwargs: Dict[str, Any] = Field(default_factory=dict)
     """Keyword arguments to pass to the model."""
     encode_kwargs: Dict[str, Any] = Field(default_factory=dict)
     """Keyword arguments to pass when calling the `encode` method of the model."""
     multi_process: bool = False
     """Run encode() on multiple GPUs."""
 
     def __init__(self, **kwargs: Any):
         """Initialize the sentence_transformer."""
+        super().__init__(**kwargs)
         try:
             import sentence_transformers
 
         except ImportError as exc:
             raise ImportError(
                 "Could not import sentence_transformers python package. "
                 "Please install it with `pip install sentence-transformers`."
             ) from exc
 
-        kwargs["client"] = sentence_transformers.SentenceTransformer(
-            kwargs.get("model_name"),
-            cache_folder=kwargs.get("cache_folder"),
-            **kwargs.get("model_kwargs"),
+        self.client = sentence_transformers.SentenceTransformer(
+            self.model_name, cache_folder=self.cache_folder, **self.model_kwargs
         )
-        super().__init__(**kwargs)
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Compute doc embeddings using a HuggingFace transformer model.
 
         Args:
             texts: The list of texts to embed.
 
@@ -198,27 +196,24 @@
     embed_instruction: str = DEFAULT_EMBED_INSTRUCTION
     """Instruction to use for embedding documents."""
     query_instruction: str = DEFAULT_QUERY_INSTRUCTION
     """Instruction to use for embedding query."""
 
     def __init__(self, **kwargs: Any):
         """Initialize the sentence_transformer."""
+        super().__init__(**kwargs)
         try:
             from InstructorEmbedding import INSTRUCTOR
 
-            kwargs["client"] = INSTRUCTOR(
-                kwargs.get("model_name"),
-                cache_folder=kwargs.get("cache_folder"),
-                **kwargs.get("model_kwargs"),
+            self.client = INSTRUCTOR(
+                self.model_name, cache_folder=self.cache_folder, **self.model_kwargs
             )
         except ImportError as e:
             raise ImportError("Dependencies for InstructorEmbedding not found.") from e
 
-        super().__init__(**kwargs)
-
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Compute doc embeddings using a HuggingFace instruct model.
 
         Args:
             texts: The list of texts to embed.
 
         Returns:
@@ -279,30 +274,27 @@
     encode_kwargs: Dict[str, Any] = Field(default_factory=dict)
     """Keyword arguments to pass when calling the `encode` method of the model."""
     query_instruction: str = DEFAULT_QUERY_BGE_INSTRUCTION_EN
     """Instruction to use for embedding query."""
 
     def __init__(self, **kwargs: Any):
         """Initialize the sentence_transformer."""
+        super().__init__(**kwargs)
         try:
             import sentence_transformers
 
         except ImportError as exc:
             raise ImportError(
                 "Could not import sentence_transformers python package. "
                 "Please install it with `pip install sentence_transformers`."
             ) from exc
 
-        kwargs["client"] = sentence_transformers.SentenceTransformer(
-            kwargs.get("model_name"),
-            cache_folder=kwargs.get("cache_folder"),
-            **kwargs.get("model_kwargs"),
+        self.client = sentence_transformers.SentenceTransformer(
+            self.model_name, cache_folder=self.cache_folder, **self.model_kwargs
         )
-
-        super().__init__(**kwargs)
         if "-zh" in self.model_name:
             self.query_instruction = DEFAULT_QUERY_BGE_INSTRUCTION_ZH
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Compute doc embeddings using a HuggingFace transformer model.
 
         Args:
@@ -484,38 +476,27 @@
     """API key for the Jina AI API.."""
     model_name: str = "jina-embeddings-v2-base-en"
     """The name of the model to use for text embeddings. Defaults to
     "jina-embeddings-v2-base-en"."""
 
     def __init__(self, **kwargs):
         """Create a new JinaEmbeddings instance."""
+        super().__init__(**kwargs)
         try:
             import requests
         except ImportError:
             raise ValueError(
                 "The requests python package is not installed. Please install it with "
                 "`pip install requests`"
             )
-        if "api_url" not in kwargs:
-            kwargs["api_url"] = "https://api.jina.ai/v1/embeddings"
-        if "session" not in kwargs:  # noqa: SIM401
-            session = requests.Session()
-        else:
-            session = kwargs["session"]
-        api_key = kwargs.get("api_key")
-        if api_key:
-            session.headers.update(
-                {
-                    "Authorization": f"Bearer {api_key}",
-                    "Accept-Encoding": "identity",
-                }
-            )
-        kwargs["session"] = session
-
-        super().__init__(**kwargs)
+        self.api_url = "https://api.jina.ai/v1/embeddings"
+        self.session = requests.Session()
+        self.session.headers.update(
+            {"Authorization": f"Bearer {self.api_key}", "Accept-Encoding": "identity"}
+        )
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Get the embeddings for a list of texts.
 
         Args:
             texts (Documents): A list of texts to get embeddings for.
 
@@ -657,30 +638,24 @@
         default=60, description="The timeout for the request in seconds."
     )
 
     session: Optional[requests.Session] = None
 
     def __init__(self, **kwargs):
         """Initialize the OpenAPIEmbeddings."""
+        super().__init__(**kwargs)
         try:
             import requests
         except ImportError:
             raise ValueError(
                 "The requests python package is not installed. "
                 "Please install it with `pip install requests`"
             )
-        if "session" not in kwargs:  # noqa: SIM401
-            session = requests.Session()
-        else:
-            session = kwargs["session"]
-        api_key = kwargs.get("api_key")
-        if api_key:
-            session.headers.update({"Authorization": f"Bearer {api_key}"})
-        kwargs["session"] = session
-        super().__init__(**kwargs)
+        self.session = requests.Session()
+        self.session.headers.update({"Authorization": f"Bearer {self.api_key}"})
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Get the embeddings for a list of texts.
 
         Args:
             texts (Documents): A list of texts to get embeddings for.
```

### Comparing `dbgpt-0.5.5/dbgpt/rag/extractor/base.py` & `dbgpt-0.5.5rc0/dbgpt/rag/extractor/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/extractor/summary.py` & `dbgpt-0.5.5rc0/dbgpt/rag/extractor/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/base.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/csv.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/csv.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/datasource.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/markdown.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,80 @@
-"""Datasource Knowledge."""
+"""Markdown Knowledge."""
 from typing import Any, Dict, List, Optional, Union
 
 from dbgpt.core import Document
-from dbgpt.datasource import BaseConnector
+from dbgpt.rag.knowledge.base import (
+    ChunkStrategy,
+    DocumentType,
+    Knowledge,
+    KnowledgeType,
+)
 
-from ..summary.gdbms_db_summary import _parse_db_summary as _parse_gdb_summary
-from ..summary.rdbms_db_summary import _parse_db_summary
-from .base import ChunkStrategy, DocumentType, Knowledge, KnowledgeType
 
-
-class DatasourceKnowledge(Knowledge):
-    """Datasource Knowledge."""
+class MarkdownKnowledge(Knowledge):
+    """Markdown Knowledge."""
 
     def __init__(
         self,
-        connector: BaseConnector,
-        summary_template: str = "{table_name}({columns})",
-        knowledge_type: Optional[KnowledgeType] = KnowledgeType.DOCUMENT,
+        file_path: Optional[str] = None,
+        knowledge_type: KnowledgeType = KnowledgeType.DOCUMENT,
+        encoding: Optional[str] = "utf-8",
+        loader: Optional[Any] = None,
         metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
-        """Create Datasource Knowledge with Knowledge arguments.
+        """Create Markdown Knowledge with Knowledge arguments.
 
         Args:
-            connector(BaseConnector): connector
-            summary_template(str, optional): summary template
+            file_path(str,  optional): file path
             knowledge_type(KnowledgeType, optional): knowledge type
-            metadata(Dict[str, Union[str, List[str]], optional): metadata
+            encoding(str, optional): csv encoding
+            loader(Any, optional): loader
         """
-        self._connector = connector
-        self._summary_template = summary_template
-        super().__init__(knowledge_type=knowledge_type, metadata=metadata, **kwargs)
+        super().__init__(
+            path=file_path,
+            knowledge_type=knowledge_type,
+            data_loader=loader,
+            metadata=metadata,
+            **kwargs,
+        )
+        self._encoding = encoding
 
     def _load(self) -> List[Document]:
-        """Load datasource document from data_loader."""
-        docs = []
-        if self._connector.is_graph_type():
-            db_summary = _parse_gdb_summary(self._connector, self._summary_template)
+        """Load markdown document from loader."""
+        if self._loader:
+            documents = self._loader.load()
         else:
-            db_summary = _parse_db_summary(self._connector, self._summary_template)
-        for table_summary in db_summary:
-            metadata = {"source": "database"}
-            if self._metadata:
-                metadata.update(self._metadata)  # type: ignore
-            docs.append(Document(content=table_summary, metadata=metadata))
-        return docs
+            if not self._path:
+                raise ValueError("file path is required")
+            with open(self._path, encoding=self._encoding, errors="ignore") as f:
+                markdown_text = f.read()
+                metadata = {"source": self._path}
+                if self._metadata:
+                    metadata.update(self._metadata)  # type: ignore
+                documents = [Document(content=markdown_text, metadata=metadata)]
+                return documents
+        return [Document.langchain2doc(lc_document) for lc_document in documents]
 
     @classmethod
     def support_chunk_strategy(cls) -> List[ChunkStrategy]:
         """Return support chunk strategy."""
         return [
             ChunkStrategy.CHUNK_BY_SIZE,
+            ChunkStrategy.CHUNK_BY_MARKDOWN_HEADER,
             ChunkStrategy.CHUNK_BY_SEPARATOR,
         ]
 
     @classmethod
+    def default_chunk_strategy(cls) -> ChunkStrategy:
+        """Return default chunk strategy."""
+        return ChunkStrategy.CHUNK_BY_MARKDOWN_HEADER
+
+    @classmethod
     def type(cls) -> KnowledgeType:
-        """Knowledge type of Datasource."""
+        """Return knowledge type."""
         return KnowledgeType.DOCUMENT
 
     @classmethod
     def document_type(cls) -> DocumentType:
         """Return document type."""
-        return DocumentType.DATASOURCE
+        return DocumentType.MARKDOWN
```

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/docx.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/docx.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/factory.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/html.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/html.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/markdown.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/txt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,83 @@
-"""Markdown Knowledge."""
+"""TXT Knowledge."""
 from typing import Any, Dict, List, Optional, Union
 
+import chardet
+
 from dbgpt.core import Document
 from dbgpt.rag.knowledge.base import (
     ChunkStrategy,
     DocumentType,
     Knowledge,
     KnowledgeType,
 )
 
 
-class MarkdownKnowledge(Knowledge):
-    """Markdown Knowledge."""
+class TXTKnowledge(Knowledge):
+    """TXT Knowledge."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         knowledge_type: KnowledgeType = KnowledgeType.DOCUMENT,
-        encoding: Optional[str] = "utf-8",
         loader: Optional[Any] = None,
         metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
-        """Create Markdown Knowledge with Knowledge arguments.
+        """Create TXT Knowledge with Knowledge arguments.
 
         Args:
             file_path(str,  optional): file path
             knowledge_type(KnowledgeType, optional): knowledge type
-            encoding(str, optional): csv encoding
             loader(Any, optional): loader
         """
         super().__init__(
             path=file_path,
             knowledge_type=knowledge_type,
             data_loader=loader,
             metadata=metadata,
             **kwargs,
         )
-        self._encoding = encoding
 
     def _load(self) -> List[Document]:
-        """Load markdown document from loader."""
+        """Load txt document from loader."""
         if self._loader:
             documents = self._loader.load()
         else:
             if not self._path:
                 raise ValueError("file path is required")
-            with open(self._path, encoding=self._encoding, errors="ignore") as f:
-                markdown_text = f.read()
-                metadata = {"source": self._path}
-                if self._metadata:
-                    metadata.update(self._metadata)  # type: ignore
-                documents = [Document(content=markdown_text, metadata=metadata)]
-                return documents
+            with open(self._path, "rb") as f:
+                raw_text = f.read()
+                result = chardet.detect(raw_text)
+                if result["encoding"] is None:
+                    text = raw_text.decode("utf-8")
+                else:
+                    text = raw_text.decode(result["encoding"])
+            metadata = {"source": self._path}
+            if self._metadata:
+                metadata.update(self._metadata)  # type: ignore
+            return [Document(content=text, metadata=metadata)]
+
         return [Document.langchain2doc(lc_document) for lc_document in documents]
 
     @classmethod
-    def support_chunk_strategy(cls) -> List[ChunkStrategy]:
+    def support_chunk_strategy(cls):
         """Return support chunk strategy."""
         return [
             ChunkStrategy.CHUNK_BY_SIZE,
-            ChunkStrategy.CHUNK_BY_MARKDOWN_HEADER,
             ChunkStrategy.CHUNK_BY_SEPARATOR,
         ]
 
     @classmethod
     def default_chunk_strategy(cls) -> ChunkStrategy:
         """Return default chunk strategy."""
-        return ChunkStrategy.CHUNK_BY_MARKDOWN_HEADER
+        return ChunkStrategy.CHUNK_BY_SIZE
 
     @classmethod
     def type(cls) -> KnowledgeType:
         """Return knowledge type."""
         return KnowledgeType.DOCUMENT
 
     @classmethod
     def document_type(cls) -> DocumentType:
         """Return document type."""
-        return DocumentType.MARKDOWN
+        return DocumentType.TXT
```

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/pdf.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pdf.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/pptx.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pptx.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/string.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/string.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/txt.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/datasource.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,60 @@
-"""TXT Knowledge."""
+"""Datasource Knowledge."""
 from typing import Any, Dict, List, Optional, Union
 
-import chardet
-
 from dbgpt.core import Document
-from dbgpt.rag.knowledge.base import (
-    ChunkStrategy,
-    DocumentType,
-    Knowledge,
-    KnowledgeType,
-)
+from dbgpt.datasource import BaseConnector
+
+from ..summary.rdbms_db_summary import _parse_db_summary
+from .base import ChunkStrategy, DocumentType, Knowledge, KnowledgeType
 
 
-class TXTKnowledge(Knowledge):
-    """TXT Knowledge."""
+class DatasourceKnowledge(Knowledge):
+    """Datasource Knowledge."""
 
     def __init__(
         self,
-        file_path: Optional[str] = None,
-        knowledge_type: KnowledgeType = KnowledgeType.DOCUMENT,
-        loader: Optional[Any] = None,
+        connector: BaseConnector,
+        summary_template: str = "{table_name}({columns})",
+        knowledge_type: Optional[KnowledgeType] = KnowledgeType.DOCUMENT,
         metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
-        """Create TXT Knowledge with Knowledge arguments.
+        """Create Datasource Knowledge with Knowledge arguments.
 
         Args:
-            file_path(str,  optional): file path
+            connector(BaseConnector): connector
+            summary_template(str, optional): summary template
             knowledge_type(KnowledgeType, optional): knowledge type
-            loader(Any, optional): loader
+            metadata(Dict[str, Union[str, List[str]], optional): metadata
         """
-        super().__init__(
-            path=file_path,
-            knowledge_type=knowledge_type,
-            data_loader=loader,
-            metadata=metadata,
-            **kwargs,
-        )
+        self._connector = connector
+        self._summary_template = summary_template
+        super().__init__(knowledge_type=knowledge_type, metadata=metadata, **kwargs)
 
     def _load(self) -> List[Document]:
-        """Load txt document from loader."""
-        if self._loader:
-            documents = self._loader.load()
-        else:
-            if not self._path:
-                raise ValueError("file path is required")
-            with open(self._path, "rb") as f:
-                raw_text = f.read()
-                result = chardet.detect(raw_text)
-                if result["encoding"] is None:
-                    text = raw_text.decode("utf-8")
-                else:
-                    text = raw_text.decode(result["encoding"])
-            metadata = {"source": self._path}
+        """Load datasource document from data_loader."""
+        docs = []
+        for table_summary in _parse_db_summary(self._connector, self._summary_template):
+            metadata = {"source": "database"}
             if self._metadata:
                 metadata.update(self._metadata)  # type: ignore
-            return [Document(content=text, metadata=metadata)]
-
-        return [Document.langchain2doc(lc_document) for lc_document in documents]
+            docs.append(Document(content=table_summary, metadata=metadata))
+        return docs
 
     @classmethod
-    def support_chunk_strategy(cls):
+    def support_chunk_strategy(cls) -> List[ChunkStrategy]:
         """Return support chunk strategy."""
         return [
             ChunkStrategy.CHUNK_BY_SIZE,
             ChunkStrategy.CHUNK_BY_SEPARATOR,
         ]
 
     @classmethod
-    def default_chunk_strategy(cls) -> ChunkStrategy:
-        """Return default chunk strategy."""
-        return ChunkStrategy.CHUNK_BY_SIZE
-
-    @classmethod
     def type(cls) -> KnowledgeType:
-        """Return knowledge type."""
+        """Knowledge type of Datasource."""
         return KnowledgeType.DOCUMENT
 
     @classmethod
     def document_type(cls) -> DocumentType:
         """Return document type."""
-        return DocumentType.TXT
+        return DocumentType.DATASOURCE
```

### Comparing `dbgpt-0.5.5/dbgpt/rag/knowledge/url.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/url.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/assembler.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/assembler.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/datasource.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/db_schema.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/embedding.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/evaluation.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/knowledge.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/rerank.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/rerank.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/rewrite.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/schema_linking.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/operators/summary.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/retriever/base.py` & `dbgpt-0.5.5rc0/dbgpt/rag/retriever/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/retriever/db_schema.py` & `dbgpt-0.5.5rc0/dbgpt/rag/retriever/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/retriever/embedding.py` & `dbgpt-0.5.5rc0/dbgpt/rag/retriever/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/retriever/rerank.py` & `dbgpt-0.5.5rc0/dbgpt/rag/retriever/rerank.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,27 +20,26 @@
             topk: int
             rank_fn: Optional[callable]
         """
         self.topk = topk
         self.rank_fn = rank_fn
 
     @abstractmethod
-    def rank(
-        self, candidates_with_scores: List[Chunk], query: Optional[str] = None
-    ) -> List[Chunk]:
+    def rank(self, candidates_with_scores: List) -> List[Chunk]:
         """Return top k chunks after ranker.
 
         Rank algorithm implementation return topk documents by candidates
         similarity score
 
         Args:
             candidates_with_scores: List[Tuple]
-            query: Optional[str]
+            topk: int
+
         Return:
-            List[Chunk]
+            List[Document]
         """
 
     def _filter(self, candidates_with_scores: List) -> List[Chunk]:
         """Filter duplicate candidates documents."""
         candidates_with_scores = sorted(
             candidates_with_scores, key=lambda x: x.score, reverse=True
         )
@@ -74,25 +73,19 @@
         #     default=None,
         # ),
     ],
 )
 class DefaultRanker(Ranker):
     """Default Ranker."""
 
-    def __init__(
-        self,
-        topk: int = 4,
-        rank_fn: Optional[RANK_FUNC] = None,
-    ):
+    def __init__(self, topk: int, rank_fn: Optional[RANK_FUNC] = None):
         """Create Default Ranker with topk and rank_fn."""
         super().__init__(topk, rank_fn)
 
-    def rank(
-        self, candidates_with_scores: List[Chunk], query: Optional[str] = None
-    ) -> List[Chunk]:
+    def rank(self, candidates_with_scores: List[Chunk]) -> List[Chunk]:
         """Return top k chunks after ranker.
 
         Return top k documents by candidates similarity score
 
         Args:
             candidates_with_scores: List[Tuple]
 
@@ -108,25 +101,19 @@
             )
         return candidates_with_scores[: self.topk]
 
 
 class RRFRanker(Ranker):
     """RRF(Reciprocal Rank Fusion) Ranker."""
 
-    def __init__(
-        self,
-        topk: int = 4,
-        rank_fn: Optional[RANK_FUNC] = None,
-    ):
+    def __init__(self, topk: int, rank_fn: Optional[RANK_FUNC] = None):
         """RRF rank algorithm implementation."""
         super().__init__(topk, rank_fn)
 
-    def rank(
-        self, candidates_with_scores: List[Chunk], query: Optional[str] = None
-    ) -> List[Chunk]:
+    def rank(self, candidates_with_scores: List[Chunk]) -> List[Chunk]:
         """RRF rank algorithm implementation.
 
         This code implements an algorithm called Reciprocal Rank Fusion (RRF), is a
         method for combining multiple result sets with different relevance indicators
         into a single result set. RRF requires no tuning, and the different relevance
         indicators do not have to be related to each other to achieve high-quality
         results.
@@ -137,91 +124,7 @@
             if d in result(q):
                 score += 1.0 / ( k + rank( result(q), d ) )
         return score
         reference:https://www.elastic.co/guide/en/elasticsearch/reference/current/rrf.html
         """
         # it will be implemented soon when multi recall is implemented
         return candidates_with_scores
-
-
-@register_resource(
-    _("CrossEncoder Rerank"),
-    "cross_encoder_ranker",
-    category=ResourceCategory.RAG,
-    description=_("CrossEncoder ranker."),
-    parameters=[
-        Parameter.build_from(
-            _("Top k"),
-            "topk",
-            int,
-            description=_("The number of top k documents."),
-        ),
-        Parameter.build_from(
-            _("Rerank Model"),
-            "model",
-            str,
-            description=_("rerank model name, e.g., 'BAAI/bge-reranker-base'."),
-        ),
-        Parameter.build_from(
-            _("device"),
-            "device",
-            str,
-            description=_("device name, e.g., 'cpu'."),
-        ),
-    ],
-)
-class CrossEncoderRanker(Ranker):
-    """CrossEncoder Ranker."""
-
-    def __init__(
-        self,
-        topk: int = 4,
-        model: str = "BAAI/bge-reranker-base",
-        device: str = "cpu",
-        rank_fn: Optional[RANK_FUNC] = None,
-    ):
-        """Cross Encoder rank algorithm implementation.
-
-        Args:
-            topk: int - The number of top k documents.
-            model: str - rerank model name, e.g., 'BAAI/bge-reranker-base'.
-            device: str - device name, e.g., 'cpu'.
-            rank_fn: Optional[callable] - The rank function.
-        Refer: https://www.sbert.net/examples/applications/cross-encoder/README.html
-        """
-        try:
-            from sentence_transformers import CrossEncoder
-        except ImportError:
-            raise ImportError(
-                "please `pip install sentence-transformers`",
-            )
-        self._model = CrossEncoder(model, max_length=512, device=device)
-        super().__init__(topk, rank_fn)
-
-    def rank(
-        self, candidates_with_scores: List[Chunk], query: Optional[str] = None
-    ) -> List[Chunk]:
-        """Cross Encoder rank algorithm implementation.
-
-        Args:
-            candidates_with_scores: List[Chunk], candidates with scores
-            query: Optional[str], query text
-        Returns:
-            List[Chunk], reranked candidates
-        """
-        contents = [candidate.content for candidate in candidates_with_scores]
-        query_content_pairs = [
-            [
-                query,
-                content,
-            ]
-            for content in contents
-        ]
-        rank_scores = self._model.predict(sentences=query_content_pairs)
-
-        for candidate, score in zip(candidates_with_scores, rank_scores):
-            candidate.score = score
-
-        new_candidates_with_scores = sorted(
-            candidates_with_scores, key=lambda x: x.score, reverse=True
-        )
-        return new_candidates_with_scores[: self.topk]
```

### Comparing `dbgpt-0.5.5/dbgpt/rag/retriever/rewrite.py` & `dbgpt-0.5.5rc0/dbgpt/rag/retriever/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/schemalinker/base_linker.py` & `dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/base_linker.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/schemalinker/schema_linking.py` & `dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/summary/db_summary.py` & `dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/summary/db_summary_client.py` & `dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import logging
 import traceback
 
 from dbgpt._private.config import Config
 from dbgpt.component import SystemApp
 from dbgpt.configs.model_config import EMBEDDING_MODEL_CONFIG
-from dbgpt.rag.summary.gdbms_db_summary import GdbmsSummary
 from dbgpt.rag.summary.rdbms_db_summary import RdbmsSummary
 
 logger = logging.getLogger(__name__)
 
 CFG = Config()
 
 
@@ -36,15 +35,15 @@
         )
         self.embeddings = embedding_factory.create(
             model_name=EMBEDDING_MODEL_CONFIG[CFG.EMBEDDING_MODEL]
         )
 
     def db_summary_embedding(self, dbname, db_type):
         """Put db profile and table profile summary into vector store."""
-        db_summary_client = self.create_summary_client(dbname, db_type)
+        db_summary_client = RdbmsSummary(dbname, db_type)
 
         self.init_db_profile(db_summary_client, dbname)
 
         logger.info("db summary embedding success")
 
     def get_db_summary(self, dbname, query, topk):
         """Get user query related tables info."""
@@ -104,36 +103,7 @@
                 connector=db_summary_client.db, vector_store_connector=vector_connector
             )
             if len(db_assembler.get_chunks()) > 0:
                 db_assembler.persist()
         else:
             logger.info(f"Vector store name {vector_store_name} exist")
         logger.info("initialize db summary profile success...")
-
-    def delete_db_profile(self, dbname):
-        """Delete db profile."""
-        vector_store_name = dbname + "_profile"
-        from dbgpt.storage.vector_store.base import VectorStoreConfig
-        from dbgpt.storage.vector_store.connector import VectorStoreConnector
-
-        vector_store_config = VectorStoreConfig(name=vector_store_name)
-        vector_connector = VectorStoreConnector.from_default(
-            CFG.VECTOR_STORE_TYPE,
-            self.embeddings,
-            vector_store_config=vector_store_config,
-        )
-        vector_connector.delete_vector_name(vector_store_name)
-        logger.info(f"delete db profile {dbname} success")
-
-    @staticmethod
-    def create_summary_client(dbname: str, db_type: str):
-        """
-        Create a summary client based on the database type.
-
-        Args:
-            dbname (str): The name of the database.
-            db_type (str): The type of the database.
-        """
-        if "graph" in db_type:
-            return GdbmsSummary(dbname, db_type)
-        else:
-            return RdbmsSummary(dbname, db_type)
```

### Comparing `dbgpt-0.5.5/dbgpt/rag/summary/gdbms_db_summary.py` & `dbgpt-0.5.5rc0/dbgpt/rag/summary/rdbms_db_summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """Summary for rdbms database."""
-
-from typing import TYPE_CHECKING, Dict, List, Optional
+import re
+from typing import TYPE_CHECKING, List, Optional
 
 from dbgpt._private.config import Config
 from dbgpt.datasource import BaseConnector
-from dbgpt.datasource.conn_tugraph import TuGraphConnector
 from dbgpt.rag.summary.db_summary import DBSummary
 
 if TYPE_CHECKING:
     from dbgpt.datasource.manages import ConnectorManager
 
 CFG = Config()
 
 
-class GdbmsSummary(DBSummary):
-    """Get graph db table summary template."""
+class RdbmsSummary(DBSummary):
+    """Get rdbms db table summary template.
+
+    Summary example:
+        table_name(column1(column1 comment),column2(column2 comment),
+        column3(column3 comment) and index keys, and table comment is {table_comment})
+    """
 
     def __init__(
         self, name: str, type: str, manager: Optional["ConnectorManager"] = None
     ):
         """Create a new RdbmsSummary."""
         self.name = name
         self.type = type
         self.summary_template = "{table_name}({columns})"
-        # self.v_summary_template = "{table_name}({columns})"
         self.tables = {}
         # self.tables_info = []
         # self.vector_tables_info = []
 
         # TODO: Don't use the global variable.
         db_manager = manager or CFG.local_db_manager
         if not db_manager:
@@ -38,97 +41,89 @@
         collation:{collation}""".format(
             users=self.db.get_users(),
             grant=self.db.get_grants(),
             charset=self.db.get_charset(),
             collation=self.db.get_collation(),
         )
         tables = self.db.get_table_names()
-        self.table_info_summaries = {
-            "vertex_tables": [
-                self.get_table_summary(table_name, "vertex")
-                for table_name in tables["vertex_tables"]
-            ],
-            "edge_tables": [
-                self.get_table_summary(table_name, "edge")
-                for table_name in tables["edge_tables"]
-            ],
-        }
+        self.table_info_summaries = [
+            self.get_table_summary(table_name) for table_name in tables
+        ]
 
-    def get_table_summary(self, table_name, table_type):
+    def get_table_summary(self, table_name):
         """Get table summary for table.
 
         example:
             table_name(column1(column1 comment),column2(column2 comment),
             column3(column3 comment) and index keys, and table comment: {table_comment})
         """
-        return _parse_table_summary(
-            self.db, self.summary_template, table_name, table_type
-        )
+        return _parse_table_summary(self.db, self.summary_template, table_name)
 
     def table_summaries(self):
         """Get table summaries."""
         return self.table_info_summaries
 
 
 def _parse_db_summary(
     conn: BaseConnector, summary_template: str = "{table_name}({columns})"
 ) -> List[str]:
-    """Get db summary for database."""
-    table_info_summaries = None
-    if isinstance(conn, TuGraphConnector):
-        table_names = conn.get_table_names()
-        v_tables = table_names.get("vertex_tables", [])
-        e_tables = table_names.get("edge_tables", [])
-        table_info_summaries = [
-            _parse_table_summary(conn, summary_template, table_name, "vertex")
-            for table_name in v_tables
-        ] + [
-            _parse_table_summary(conn, summary_template, table_name, "edge")
-            for table_name in e_tables
-        ]
-    else:
-        table_info_summaries = []
+    """Get db summary for database.
 
+    Args:
+        conn (BaseConnector): database connection
+        summary_template (str): summary template
+    """
+    tables = conn.get_table_names()
+    table_info_summaries = [
+        _parse_table_summary(conn, summary_template, table_name)
+        for table_name in tables
+    ]
     return table_info_summaries
 
 
-def _format_column(column: Dict) -> str:
-    """Format a single column's summary."""
-    comment = column.get("comment", "")
-    if column.get("is_in_primary_key"):
-        comment += " Primary Key" if comment else "Primary Key"
-    return f"{column['name']} ({comment})" if comment else column["name"]
-
-
-def _format_indexes(indexes: List[Dict]) -> str:
-    """Format index keys for table summary."""
-    return ", ".join(
-        f"{index['name']}(`{', '.join(index['column_names'])}`)" for index in indexes
-    )
-
-
 def _parse_table_summary(
-    conn: TuGraphConnector, summary_template: str, table_name: str, table_type: str
+    conn: BaseConnector, summary_template: str, table_name: str
 ) -> str:
-    """Enhanced table summary function."""
-    columns = [
-        _format_column(column) for column in conn.get_columns(table_name, table_type)
-    ]
-    column_str = ", ".join(columns)
+    """Get table summary for table.
 
-    indexes = conn.get_indexes(table_name, table_type)
-    index_str = _format_indexes(indexes) if indexes else ""
+    Args:
+        conn (BaseConnector): database connection
+        summary_template (str): summary template
+        table_name (str): table name
+
+    Examples:
+        table_name(column1(column1 comment),column2(column2 comment),
+        column3(column3 comment) and index keys, and table comment: {table_comment})
+    """
+    columns = []
+    for column in conn.get_columns(table_name):
+        if column.get("comment"):
+            columns.append(f"{column['name']} ({column.get('comment')})")
+        else:
+            columns.append(f"{column['name']}")
 
+    column_str = ", ".join(columns)
+    # Obtain index information
+    index_keys = []
+    raw_indexes = conn.get_indexes(table_name)
+    for index in raw_indexes:
+        if isinstance(index, tuple):  # Process tuple type index information
+            index_name, index_creation_command = index
+            # Extract column names using re
+            matched_columns = re.findall(r"\(([^)]+)\)", index_creation_command)
+            if matched_columns:
+                key_str = ", ".join(matched_columns)
+                index_keys.append(f"{index_name}(`{key_str}`) ")
+        else:
+            key_str = ", ".join(index["column_names"])
+            index_keys.append(f"{index['name']}(`{key_str}`) ")
     table_str = summary_template.format(table_name=table_name, columns=column_str)
-    if index_str:
-        table_str += f", and index keys: {index_str}"
+    if len(index_keys) > 0:
+        index_key_str = ", ".join(index_keys)
+        table_str += f", and index keys: {index_key_str}"
     try:
         comment = conn.get_table_comment(table_name)
     except Exception:
         comment = dict(text=None)
     if comment.get("text"):
-        table_str += (
-            f", and table comment: {comment.get('text')}, this is a {table_type} table"
-        )
-    else:
-        table_str += f", and table comment: this is a {table_type} table"
+        table_str += f", and table comment: {comment.get('text')}"
     return table_str
```

### Comparing `dbgpt-0.5.5/dbgpt/rag/text_splitter/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/text_splitter/pre_text_splitter.py` & `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/pre_text_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/rag/text_splitter/text_splitter.py` & `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/text_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -511,16 +511,15 @@
             ):
                 # If the last line in the aggregated list
                 # has the same metadata as the current line,
                 # append the current content to the last lines's content
                 aggregated_chunks[-1]["content"] += "  \n" + line["content"]
             else:
                 # Otherwise, append the current line to the aggregated list
-                subtitles = "-".join((list(line["metadata"].values())))
-                line["content"] = f'"{subtitles}": ' + line["content"]
+                line["content"] = f"{line['metadata']}, " + line["content"]
                 aggregated_chunks.append(line)
 
         return [
             Chunk(content=chunk["content"], metadata=chunk["metadata"])
             for chunk in aggregated_chunks
         ]
 
@@ -554,36 +553,24 @@
         # Content and metadata of the chunk currently being processed
         current_content: List[str] = []
         current_metadata: Dict[str, str] = {}
         # Keep track of the nested header structure
         # header_stack: List[Dict[str, Union[int, str]]] = []
         header_stack: List[HeaderType] = []
         initial_metadata: Dict[str, str] = {}
-        # Determine whether a line is within a markdown code block.
-        in_code_block = False
         for line in lines:
             stripped_line = line.strip()
-            # A code frame starts with "```"
-            with_code_frame = stripped_line.startswith("```") and (
-                stripped_line != "```"
-            )
-            if (not in_code_block) and with_code_frame:
-                in_code_block = True
             # Check each line against each of the header types (e.g., #, ##)
             for sep, name in self.headers_to_split_on:
                 # Check if line starts with a header that we intend to split on
-                if (
-                    (not in_code_block)
-                    and stripped_line.startswith(sep)
-                    and (
-                        # Header with no text OR header is followed by space
-                        # Both are valid conditions that sep is being used a header
-                        len(stripped_line) == len(sep)
-                        or stripped_line[len(sep)] == " "
-                    )
+                if stripped_line.startswith(sep) and (
+                    # Header with no text OR header is followed by space
+                    # Both are valid conditions that sep is being used a header
+                    len(stripped_line) == len(sep)
+                    or stripped_line[len(sep)] == " "
                 ):
                     # Ensure we are tracking the header as metadata
                     if name is not None:
                         # Get the current header level
                         current_header_level = sep.count("#")
 
                         # Pop out headers of lower or same level from the stack
@@ -629,18 +616,14 @@
                         {
                             "content": separator.join(current_content),
                             "metadata": current_metadata.copy(),
                         }
                     )
                     current_content.clear()
 
-            # Code block ends
-            if in_code_block and stripped_line == "```":
-                in_code_block = False
-
             current_metadata = initial_metadata.copy()
         if current_content:
             lines_with_metadata.append(
                 {
                     "content": separator.join(current_content),
                     "metadata": current_metadata,
                 }
```

### Comparing `dbgpt-0.5.5/dbgpt/rag/text_splitter/token_splitter.py` & `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/token_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/cache/llm_cache.py` & `dbgpt-0.5.5rc0/dbgpt/storage/cache/llm_cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/cache/manager.py` & `dbgpt-0.5.5rc0/dbgpt/storage/cache/manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/cache/operators.py` & `dbgpt-0.5.5rc0/dbgpt/storage/cache/operators.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/cache/storage/base.py` & `dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/cache/storage/disk/disk_storage.py` & `dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/disk_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/chat_history/chat_history_db.py` & `dbgpt-0.5.5rc0/dbgpt/storage/chat_history/chat_history_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/chat_history/storage_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/storage/chat_history/storage_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/metadata/_base_dao.py` & `dbgpt-0.5.5rc0/dbgpt/storage/metadata/_base_dao.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/metadata/db_factory.py` & `dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/metadata/db_manager.py` & `dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/metadata/db_storage.py` & `dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/schema.py` & `dbgpt-0.5.5rc0/dbgpt/storage/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     MSSQL = DbInfo("mssql")
     Postgresql = DbInfo("postgresql")
     Clickhouse = DbInfo("clickhouse")
     StarRocks = DbInfo("starrocks")
     Spark = DbInfo("spark", True)
     Doris = DbInfo("doris")
     Hive = DbInfo("hive")
-    TuGraph = DbInfo("tugraph")
 
     def value(self) -> str:
         """Return the name of the database type."""
         return self._value_.name
 
     def is_file_db(self) -> bool:
         """Return whether the database is a file database."""
```

### Comparing `dbgpt-0.5.5/dbgpt/storage/vector_store/base.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/vector_store/chroma_store.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/chroma_store.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/vector_store/connector.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/connector.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/vector_store/filters.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/filters.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/vector_store/milvus_store.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/milvus_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
 
         if score_threshold is not None:
             docs_and_scores = [
                 Chunk(
                     metadata=doc.metadata,
                     content=doc.content,
                     score=score,
-                    chunk_id=str(id),
+                    chunk_id=id,
                 )
                 for doc, score, id in docs_and_scores
                 if score >= score_threshold
             ]
             if len(docs_and_scores) == 0:
                 logger.warning(
                     "No relevant docs were retrieved using the relevance score"
```

### Comparing `dbgpt-0.5.5/dbgpt/storage/vector_store/pgvector_store.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/pgvector_store.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/storage/vector_store/weaviate_store.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/weaviate_store.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/_db_migration_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/_db_migration_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/annotations.py` & `dbgpt-0.5.5rc0/dbgpt/util/annotations.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/api_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/api_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py` & `dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/benchmarks/llm/llm_benchmarks.py` & `dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/chat_util.py` & `dbgpt-0.5.5rc0/dbgpt/util/chat_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/code_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/code_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/command_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/command_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/config_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/config_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/console/console.py` & `dbgpt-0.5.5rc0/dbgpt/util/console/console.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/custom_data_structure.py` & `dbgpt-0.5.5rc0/dbgpt/util/custom_data_structure.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/dbgpts/base.py` & `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/dbgpts/cli.py` & `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/dbgpts/loader.py` & `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/dbgpts/repo.py` & `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/repo.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/dbgpts/template.py` & `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/template.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/error_types.py` & `dbgpt-0.5.5rc0/dbgpt/util/error_types.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/executor_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/executor_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/fastapi.py` & `dbgpt-0.5.5rc0/dbgpt/util/fastapi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/formatting.py` & `dbgpt-0.5.5rc0/dbgpt/util/formatting.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/function_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/function_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/global_helper.py` & `dbgpt-0.5.5rc0/dbgpt/util/global_helper.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/i18n_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/i18n_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/json_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/json_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/model_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/model_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/module_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/module_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/net_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/net_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/network/_cli.py` & `dbgpt-0.5.5rc0/dbgpt/util/network/_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/openai_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/openai_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/pagination_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/pagination_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/parameter_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/parameter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/pd_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/prompt_util.py` & `dbgpt-0.5.5rc0/dbgpt/util/prompt_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/retry.py` & `dbgpt-0.5.5rc0/dbgpt/util/retry.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/serialization/json_serialization.py` & `dbgpt-0.5.5rc0/dbgpt/util/serialization/json_serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/similarity_util.py` & `dbgpt-0.5.5rc0/dbgpt/util/similarity_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/singleton.py` & `dbgpt-0.5.5rc0/dbgpt/util/singleton.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/speech/base.py` & `dbgpt-0.5.5rc0/dbgpt/util/speech/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/speech/brian.py` & `dbgpt-0.5.5rc0/dbgpt/util/speech/brian.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/speech/eleven_labs.py` & `dbgpt-0.5.5rc0/dbgpt/util/speech/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/speech/macos_tts.py` & `dbgpt-0.5.5rc0/dbgpt/util/speech/macos_tts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/speech/say.py` & `dbgpt-0.5.5rc0/dbgpt/util/speech/say.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/splitter_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/splitter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/string_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/system_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/system_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/tracer/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/tracer/base.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/tracer/span_storage.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/span_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/tracer/tracer_cli.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/tracer/tracer_impl.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/tracer/tracer_middleware.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_middleware.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/util/utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/vis/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/vis/base.py` & `dbgpt-0.5.5rc0/dbgpt/vis/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/vis/client.py` & `dbgpt-0.5.5rc0/dbgpt/vis/client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/vis/tags/vis_chart.py` & `dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_chart.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt/vis/tags/vis_dashboard.py` & `dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_dashboard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5/dbgpt.egg-info/PKG-INFO` & `dbgpt-0.5.5rc0/dbgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.5
+Version: 0.5.5rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -13,406 +13,393 @@
 Requires-Dist: chardet==5.1.0
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: cachetools
 Requires-Dist: pydantic>=2.6.0
 Requires-Dist: typeguard
 Provides-Extra: core
+Requires-Dist: chardet==5.1.0; extra == "core"
+Requires-Dist: importlib-resources==5.12.0; extra == "core"
 Requires-Dist: cachetools; extra == "core"
+Requires-Dist: typeguard; extra == "core"
 Requires-Dist: aiohttp==3.8.4; extra == "core"
 Requires-Dist: python-dotenv==1.0.0; extra == "core"
 Requires-Dist: pydantic>=2.6.0; extra == "core"
-Requires-Dist: importlib-resources==5.12.0; extra == "core"
-Requires-Dist: chardet==5.1.0; extra == "core"
-Requires-Dist: typeguard; extra == "core"
 Provides-Extra: client
+Requires-Dist: chardet==5.1.0; extra == "client"
+Requires-Dist: httpx; extra == "client"
+Requires-Dist: importlib-resources==5.12.0; extra == "client"
 Requires-Dist: fastapi>=0.100.0; extra == "client"
 Requires-Dist: cachetools; extra == "client"
-Requires-Dist: httpx; extra == "client"
+Requires-Dist: typeguard; extra == "client"
 Requires-Dist: aiohttp==3.8.4; extra == "client"
 Requires-Dist: python-dotenv==1.0.0; extra == "client"
 Requires-Dist: pydantic>=2.6.0; extra == "client"
-Requires-Dist: importlib-resources==5.12.0; extra == "client"
-Requires-Dist: chardet==5.1.0; extra == "client"
-Requires-Dist: typeguard; extra == "client"
 Provides-Extra: cli
-Requires-Dist: fastapi>=0.100.0; extra == "cli"
-Requires-Dist: cachetools; extra == "cli"
-Requires-Dist: colorama==0.4.6; extra == "cli"
+Requires-Dist: click; extra == "cli"
+Requires-Dist: chardet==5.1.0; extra == "cli"
 Requires-Dist: httpx; extra == "cli"
 Requires-Dist: tomlkit; extra == "cli"
+Requires-Dist: importlib-resources==5.12.0; extra == "cli"
+Requires-Dist: fastapi>=0.100.0; extra == "cli"
+Requires-Dist: prettytable; extra == "cli"
+Requires-Dist: cachetools; extra == "cli"
+Requires-Dist: typeguard; extra == "cli"
+Requires-Dist: rich; extra == "cli"
+Requires-Dist: psutil==5.9.4; extra == "cli"
 Requires-Dist: aiohttp==3.8.4; extra == "cli"
+Requires-Dist: colorama==0.4.6; extra == "cli"
 Requires-Dist: python-dotenv==1.0.0; extra == "cli"
-Requires-Dist: psutil==5.9.4; extra == "cli"
-Requires-Dist: click; extra == "cli"
-Requires-Dist: rich; extra == "cli"
 Requires-Dist: pydantic>=2.6.0; extra == "cli"
-Requires-Dist: importlib-resources==5.12.0; extra == "cli"
-Requires-Dist: chardet==5.1.0; extra == "cli"
-Requires-Dist: typeguard; extra == "cli"
-Requires-Dist: prettytable; extra == "cli"
 Provides-Extra: agent
-Requires-Dist: fastapi>=0.100.0; extra == "agent"
-Requires-Dist: cachetools; extra == "agent"
-Requires-Dist: colorama==0.4.6; extra == "agent"
+Requires-Dist: click; extra == "agent"
+Requires-Dist: chardet==5.1.0; extra == "agent"
 Requires-Dist: httpx; extra == "agent"
 Requires-Dist: tomlkit; extra == "agent"
-Requires-Dist: aiohttp==3.8.4; extra == "agent"
-Requires-Dist: python-dotenv==1.0.0; extra == "agent"
 Requires-Dist: termcolor; extra == "agent"
+Requires-Dist: importlib-resources==5.12.0; extra == "agent"
+Requires-Dist: fastapi>=0.100.0; extra == "agent"
+Requires-Dist: prettytable; extra == "agent"
+Requires-Dist: cachetools; extra == "agent"
+Requires-Dist: typeguard; extra == "agent"
 Requires-Dist: pandas==2.0.3; extra == "agent"
-Requires-Dist: psutil==5.9.4; extra == "agent"
-Requires-Dist: click; extra == "agent"
 Requires-Dist: rich; extra == "agent"
+Requires-Dist: psutil==5.9.4; extra == "agent"
+Requires-Dist: aiohttp==3.8.4; extra == "agent"
+Requires-Dist: colorama==0.4.6; extra == "agent"
+Requires-Dist: python-dotenv==1.0.0; extra == "agent"
 Requires-Dist: pydantic>=2.6.0; extra == "agent"
-Requires-Dist: importlib-resources==5.12.0; extra == "agent"
-Requires-Dist: chardet==5.1.0; extra == "agent"
-Requires-Dist: typeguard; extra == "agent"
-Requires-Dist: prettytable; extra == "agent"
 Provides-Extra: simple-framework
+Requires-Dist: click; extra == "simple-framework"
 Requires-Dist: fschat; extra == "simple-framework"
-Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
 Requires-Dist: msgpack; extra == "simple-framework"
-Requires-Dist: duckdb; extra == "simple-framework"
-Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
 Requires-Dist: uvicorn; extra == "simple-framework"
+Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
+Requires-Dist: typeguard; extra == "simple-framework"
+Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: duckdb-engine; extra == "simple-framework"
+Requires-Dist: colorama==0.4.6; extra == "simple-framework"
+Requires-Dist: pympler; extra == "simple-framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
+Requires-Dist: jinja2; extra == "simple-framework"
+Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
 Requires-Dist: schedule; extra == "simple-framework"
-Requires-Dist: shortuuid; extra == "simple-framework"
-Requires-Dist: prettytable; extra == "simple-framework"
-Requires-Dist: tomlkit; extra == "simple-framework"
+Requires-Dist: chardet==5.1.0; extra == "simple-framework"
 Requires-Dist: httpx; extra == "simple-framework"
+Requires-Dist: tomlkit; extra == "simple-framework"
+Requires-Dist: cachetools; extra == "simple-framework"
+Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
 Requires-Dist: psutil==5.9.4; extra == "simple-framework"
 Requires-Dist: termcolor; extra == "simple-framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
-Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
-Requires-Dist: click; extra == "simple-framework"
-Requires-Dist: chardet==5.1.0; extra == "simple-framework"
+Requires-Dist: prettytable; extra == "simple-framework"
 Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
-Requires-Dist: cachetools; extra == "simple-framework"
-Requires-Dist: jinja2; extra == "simple-framework"
-Requires-Dist: colorama==0.4.6; extra == "simple-framework"
 Requires-Dist: pandas==2.0.3; extra == "simple-framework"
-Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
-Requires-Dist: duckdb-engine; extra == "simple-framework"
-Requires-Dist: pympler; extra == "simple-framework"
-Requires-Dist: typeguard; extra == "simple-framework"
-Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
+Requires-Dist: duckdb; extra == "simple-framework"
+Requires-Dist: shortuuid; extra == "simple-framework"
 Provides-Extra: framework
+Requires-Dist: click; extra == "framework"
 Requires-Dist: fschat; extra == "framework"
-Requires-Dist: fastapi>=0.100.0; extra == "framework"
 Requires-Dist: msgpack; extra == "framework"
-Requires-Dist: duckdb; extra == "framework"
-Requires-Dist: aiohttp==3.8.4; extra == "framework"
-Requires-Dist: aiofiles; extra == "framework"
 Requires-Dist: uvicorn; extra == "framework"
-Requires-Dist: schedule; extra == "framework"
-Requires-Dist: GitPython; extra == "framework"
-Requires-Dist: shortuuid; extra == "framework"
+Requires-Dist: importlib-resources==5.12.0; extra == "framework"
+Requires-Dist: typeguard; extra == "framework"
+Requires-Dist: rich; extra == "framework"
+Requires-Dist: duckdb-engine; extra == "framework"
 Requires-Dist: pymysql; extra == "framework"
-Requires-Dist: prettytable; extra == "framework"
-Requires-Dist: graphviz; extra == "framework"
-Requires-Dist: tomlkit; extra == "framework"
-Requires-Dist: httpx; extra == "framework"
-Requires-Dist: psutil==5.9.4; extra == "framework"
-Requires-Dist: termcolor; extra == "framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "framework"
+Requires-Dist: colorama==0.4.6; extra == "framework"
+Requires-Dist: pympler; extra == "framework"
+Requires-Dist: alembic==1.12.0; extra == "framework"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
-Requires-Dist: transformers>=4.34.0; extra == "framework"
 Requires-Dist: coloredlogs; extra == "framework"
+Requires-Dist: aiofiles; extra == "framework"
+Requires-Dist: seaborn; extra == "framework"
+Requires-Dist: openpyxl==3.1.2; extra == "framework"
+Requires-Dist: jinja2; extra == "framework"
+Requires-Dist: fastapi>=0.100.0; extra == "framework"
+Requires-Dist: GitPython; extra == "framework"
+Requires-Dist: schedule; extra == "framework"
+Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: httpx; extra == "framework"
+Requires-Dist: tomlkit; extra == "framework"
+Requires-Dist: gTTS==2.3.1; extra == "framework"
+Requires-Dist: cachetools; extra == "framework"
 Requires-Dist: auto-gpt-plugin-template; extra == "framework"
-Requires-Dist: jsonschema; extra == "framework"
+Requires-Dist: transformers>=4.34.0; extra == "framework"
 Requires-Dist: pydantic>=2.6.0; extra == "framework"
-Requires-Dist: click; extra == "framework"
-Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: psutil==5.9.4; extra == "framework"
+Requires-Dist: termcolor; extra == "framework"
+Requires-Dist: prettytable; extra == "framework"
 Requires-Dist: sqlparse==0.4.4; extra == "framework"
-Requires-Dist: cachetools; extra == "framework"
-Requires-Dist: jinja2; extra == "framework"
-Requires-Dist: colorama==0.4.6; extra == "framework"
-Requires-Dist: gTTS==2.3.1; extra == "framework"
-Requires-Dist: seaborn; extra == "framework"
-Requires-Dist: alembic==1.12.0; extra == "framework"
 Requires-Dist: pandas==2.0.3; extra == "framework"
+Requires-Dist: graphviz; extra == "framework"
+Requires-Dist: aiohttp==3.8.4; extra == "framework"
+Requires-Dist: jsonschema; extra == "framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "framework"
 Requires-Dist: xlrd==2.0.1; extra == "framework"
-Requires-Dist: importlib-resources==5.12.0; extra == "framework"
-Requires-Dist: duckdb-engine; extra == "framework"
-Requires-Dist: pympler; extra == "framework"
-Requires-Dist: openpyxl==3.1.2; extra == "framework"
-Requires-Dist: typeguard; extra == "framework"
-Requires-Dist: rich; extra == "framework"
+Requires-Dist: duckdb; extra == "framework"
+Requires-Dist: shortuuid; extra == "framework"
 Provides-Extra: torch
-Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchvision==0.17.1; extra == "torch"
+Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchaudio==2.2.1; extra == "torch"
 Provides-Extra: torch-cpu
-Requires-Dist: torch==2.2.1; extra == "torch-cpu"
 Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
+Requires-Dist: torch==2.2.1; extra == "torch-cpu"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cpu"
 Provides-Extra: torch-cuda
-Requires-Dist: torch==2.2.1; extra == "torch-cuda"
 Requires-Dist: torchvision==0.17.1; extra == "torch-cuda"
+Requires-Dist: torch==2.2.1; extra == "torch-cuda"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cuda"
 Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python; extra == "llama-cpp"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes; extra == "bitsandbytes"
 Provides-Extra: quantization
-Requires-Dist: autoawq; extra == "quantization"
-Requires-Dist: optimum; extra == "quantization"
-Requires-Dist: bitsandbytes; extra == "quantization"
-Requires-Dist: auto-gptq; extra == "quantization"
 Requires-Dist: cpm_kernels; extra == "quantization"
 Provides-Extra: vstore
 Requires-Dist: chromadb>=0.4.22; extra == "vstore"
 Provides-Extra: vstore-weaviate
-Requires-Dist: weaviate-client; extra == "vstore-weaviate"
 Requires-Dist: chromadb>=0.4.22; extra == "vstore-weaviate"
+Requires-Dist: weaviate-client; extra == "vstore-weaviate"
 Provides-Extra: vstore-milvus
-Requires-Dist: chromadb>=0.4.22; extra == "vstore-milvus"
 Requires-Dist: pymilvus; extra == "vstore-milvus"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-milvus"
 Provides-Extra: vstore-all
-Requires-Dist: weaviate-client; extra == "vstore-all"
-Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
 Requires-Dist: pymilvus; extra == "vstore-all"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
+Requires-Dist: weaviate-client; extra == "vstore-all"
 Provides-Extra: datasource
 Requires-Dist: pymysql; extra == "datasource"
 Provides-Extra: datasource-all
 Requires-Dist: pymssql; extra == "datasource-all"
 Requires-Dist: pyspark; extra == "datasource-all"
+Requires-Dist: clickhouse-connect; extra == "datasource-all"
 Requires-Dist: thrift_sasl; extra == "datasource-all"
-Requires-Dist: psycopg2; extra == "datasource-all"
 Requires-Dist: mysqlclient==2.1.0; extra == "datasource-all"
 Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "datasource-all"
 Requires-Dist: pyhive; extra == "datasource-all"
-Requires-Dist: clickhouse-connect; extra == "datasource-all"
 Requires-Dist: pymysql; extra == "datasource-all"
 Requires-Dist: thrift; extra == "datasource-all"
-Requires-Dist: neo4j; extra == "datasource-all"
+Requires-Dist: psycopg2; extra == "datasource-all"
 Provides-Extra: rag
+Requires-Dist: pypdf; extra == "rag"
+Requires-Dist: python-pptx; extra == "rag"
 Requires-Dist: python-docx; extra == "rag"
+Requires-Dist: spacy>=3.7; extra == "rag"
+Requires-Dist: markdown; extra == "rag"
 Requires-Dist: python-multipart; extra == "rag"
+Requires-Dist: sentence-transformers; extra == "rag"
 Requires-Dist: langchain>=0.0.286; extra == "rag"
-Requires-Dist: chromadb>=0.4.22; extra == "rag"
-Requires-Dist: pypdf; extra == "rag"
-Requires-Dist: spacy>=3.7; extra == "rag"
 Requires-Dist: bs4; extra == "rag"
-Requires-Dist: sentence-transformers; extra == "rag"
-Requires-Dist: markdown; extra == "rag"
-Requires-Dist: python-pptx; extra == "rag"
+Requires-Dist: chromadb>=0.4.22; extra == "rag"
 Provides-Extra: openai
+Requires-Dist: click; extra == "openai"
 Requires-Dist: fschat; extra == "openai"
-Requires-Dist: fastapi>=0.100.0; extra == "openai"
 Requires-Dist: msgpack; extra == "openai"
-Requires-Dist: python-multipart; extra == "openai"
-Requires-Dist: duckdb; extra == "openai"
-Requires-Dist: aiohttp==3.8.4; extra == "openai"
-Requires-Dist: aiofiles; extra == "openai"
 Requires-Dist: uvicorn; extra == "openai"
-Requires-Dist: schedule; extra == "openai"
-Requires-Dist: GitPython; extra == "openai"
-Requires-Dist: shortuuid; extra == "openai"
+Requires-Dist: importlib-resources==5.12.0; extra == "openai"
+Requires-Dist: typeguard; extra == "openai"
+Requires-Dist: rich; extra == "openai"
+Requires-Dist: duckdb-engine; extra == "openai"
+Requires-Dist: spacy>=3.7; extra == "openai"
 Requires-Dist: pymysql; extra == "openai"
-Requires-Dist: python-pptx; extra == "openai"
-Requires-Dist: prettytable; extra == "openai"
-Requires-Dist: python-docx; extra == "openai"
-Requires-Dist: graphviz; extra == "openai"
-Requires-Dist: tomlkit; extra == "openai"
-Requires-Dist: httpx; extra == "openai"
-Requires-Dist: chromadb>=0.4.22; extra == "openai"
-Requires-Dist: pypdf; extra == "openai"
-Requires-Dist: psutil==5.9.4; extra == "openai"
-Requires-Dist: tiktoken; extra == "openai"
-Requires-Dist: bs4; extra == "openai"
-Requires-Dist: sentence-transformers; extra == "openai"
 Requires-Dist: markdown; extra == "openai"
-Requires-Dist: termcolor; extra == "openai"
-Requires-Dist: python-dotenv==1.0.0; extra == "openai"
+Requires-Dist: colorama==0.4.6; extra == "openai"
+Requires-Dist: langchain>=0.0.286; extra == "openai"
+Requires-Dist: pympler; extra == "openai"
+Requires-Dist: alembic==1.12.0; extra == "openai"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
-Requires-Dist: transformers>=4.34.0; extra == "openai"
 Requires-Dist: coloredlogs; extra == "openai"
+Requires-Dist: aiofiles; extra == "openai"
+Requires-Dist: pypdf; extra == "openai"
+Requires-Dist: seaborn; extra == "openai"
+Requires-Dist: openpyxl==3.1.2; extra == "openai"
+Requires-Dist: jinja2; extra == "openai"
+Requires-Dist: fastapi>=0.100.0; extra == "openai"
+Requires-Dist: python-multipart; extra == "openai"
+Requires-Dist: bs4; extra == "openai"
+Requires-Dist: GitPython; extra == "openai"
+Requires-Dist: schedule; extra == "openai"
+Requires-Dist: chromadb>=0.4.22; extra == "openai"
+Requires-Dist: chardet==5.1.0; extra == "openai"
+Requires-Dist: httpx; extra == "openai"
+Requires-Dist: tomlkit; extra == "openai"
+Requires-Dist: gTTS==2.3.1; extra == "openai"
+Requires-Dist: python-docx; extra == "openai"
+Requires-Dist: cachetools; extra == "openai"
 Requires-Dist: auto-gpt-plugin-template; extra == "openai"
-Requires-Dist: jsonschema; extra == "openai"
+Requires-Dist: transformers>=4.34.0; extra == "openai"
 Requires-Dist: pydantic>=2.6.0; extra == "openai"
+Requires-Dist: psutil==5.9.4; extra == "openai"
+Requires-Dist: sentence-transformers; extra == "openai"
+Requires-Dist: python-pptx; extra == "openai"
+Requires-Dist: termcolor; extra == "openai"
 Requires-Dist: openai; extra == "openai"
-Requires-Dist: click; extra == "openai"
-Requires-Dist: chardet==5.1.0; extra == "openai"
+Requires-Dist: prettytable; extra == "openai"
 Requires-Dist: sqlparse==0.4.4; extra == "openai"
-Requires-Dist: cachetools; extra == "openai"
-Requires-Dist: jinja2; extra == "openai"
-Requires-Dist: colorama==0.4.6; extra == "openai"
-Requires-Dist: gTTS==2.3.1; extra == "openai"
-Requires-Dist: langchain>=0.0.286; extra == "openai"
-Requires-Dist: seaborn; extra == "openai"
-Requires-Dist: alembic==1.12.0; extra == "openai"
 Requires-Dist: pandas==2.0.3; extra == "openai"
+Requires-Dist: graphviz; extra == "openai"
+Requires-Dist: tiktoken; extra == "openai"
+Requires-Dist: aiohttp==3.8.4; extra == "openai"
+Requires-Dist: jsonschema; extra == "openai"
+Requires-Dist: python-dotenv==1.0.0; extra == "openai"
 Requires-Dist: xlrd==2.0.1; extra == "openai"
-Requires-Dist: spacy>=3.7; extra == "openai"
-Requires-Dist: importlib-resources==5.12.0; extra == "openai"
-Requires-Dist: duckdb-engine; extra == "openai"
-Requires-Dist: pympler; extra == "openai"
-Requires-Dist: openpyxl==3.1.2; extra == "openai"
-Requires-Dist: typeguard; extra == "openai"
-Requires-Dist: rich; extra == "openai"
+Requires-Dist: duckdb; extra == "openai"
+Requires-Dist: shortuuid; extra == "openai"
 Provides-Extra: gpt4all
 Requires-Dist: gpt4all; extra == "gpt4all"
 Provides-Extra: vllm
 Requires-Dist: vllm; extra == "vllm"
 Provides-Extra: cache
 Requires-Dist: rocksdict; extra == "cache"
 Provides-Extra: default
+Requires-Dist: click; extra == "default"
 Requires-Dist: fschat; extra == "default"
-Requires-Dist: fastapi>=0.100.0; extra == "default"
+Requires-Dist: torchaudio==2.2.1; extra == "default"
 Requires-Dist: msgpack; extra == "default"
-Requires-Dist: python-multipart; extra == "default"
-Requires-Dist: zhipuai; extra == "default"
-Requires-Dist: autoawq; extra == "default"
-Requires-Dist: duckdb; extra == "default"
+Requires-Dist: uvicorn; extra == "default"
+Requires-Dist: importlib-resources==5.12.0; extra == "default"
+Requires-Dist: sentencepiece; extra == "default"
+Requires-Dist: typeguard; extra == "default"
+Requires-Dist: rich; extra == "default"
+Requires-Dist: duckdb-engine; extra == "default"
+Requires-Dist: spacy>=3.7; extra == "default"
+Requires-Dist: pymysql; extra == "default"
+Requires-Dist: markdown; extra == "default"
+Requires-Dist: colorama==0.4.6; extra == "default"
 Requires-Dist: rocksdict; extra == "default"
-Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: langchain>=0.0.286; extra == "default"
+Requires-Dist: pympler; extra == "default"
+Requires-Dist: alembic==1.12.0; extra == "default"
+Requires-Dist: torch==2.2.1; extra == "default"
+Requires-Dist: chardet; extra == "default"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
+Requires-Dist: coloredlogs; extra == "default"
 Requires-Dist: aiofiles; extra == "default"
-Requires-Dist: uvicorn; extra == "default"
+Requires-Dist: pypdf; extra == "default"
+Requires-Dist: seaborn; extra == "default"
+Requires-Dist: openpyxl==3.1.2; extra == "default"
+Requires-Dist: jinja2; extra == "default"
+Requires-Dist: fastapi>=0.100.0; extra == "default"
+Requires-Dist: python-multipart; extra == "default"
+Requires-Dist: bs4; extra == "default"
+Requires-Dist: tokenizers>=0.14; extra == "default"
 Requires-Dist: schedule; extra == "default"
 Requires-Dist: GitPython; extra == "default"
-Requires-Dist: bitsandbytes; extra == "default"
-Requires-Dist: shortuuid; extra == "default"
-Requires-Dist: pymysql; extra == "default"
-Requires-Dist: python-pptx; extra == "default"
-Requires-Dist: tokenizers>=0.14; extra == "default"
-Requires-Dist: chardet; extra == "default"
-Requires-Dist: prettytable; extra == "default"
-Requires-Dist: python-docx; extra == "default"
-Requires-Dist: graphviz; extra == "default"
-Requires-Dist: tomlkit; extra == "default"
-Requires-Dist: httpx; extra == "default"
-Requires-Dist: optimum; extra == "default"
 Requires-Dist: chromadb>=0.4.22; extra == "default"
-Requires-Dist: pypdf; extra == "default"
+Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: httpx; extra == "default"
+Requires-Dist: tomlkit; extra == "default"
+Requires-Dist: gTTS==2.3.1; extra == "default"
+Requires-Dist: python-docx; extra == "default"
+Requires-Dist: cachetools; extra == "default"
+Requires-Dist: auto-gpt-plugin-template; extra == "default"
+Requires-Dist: dashscope; extra == "default"
+Requires-Dist: pydantic>=2.6.0; extra == "default"
 Requires-Dist: psutil==5.9.4; extra == "default"
-Requires-Dist: bs4; extra == "default"
-Requires-Dist: auto-gptq; extra == "default"
+Requires-Dist: transformers>=4.34.0; extra == "default"
 Requires-Dist: sentence-transformers; extra == "default"
-Requires-Dist: markdown; extra == "default"
-Requires-Dist: accelerate>=0.20.3; extra == "default"
-Requires-Dist: dashscope; extra == "default"
-Requires-Dist: sentencepiece; extra == "default"
+Requires-Dist: zhipuai; extra == "default"
+Requires-Dist: python-pptx; extra == "default"
+Requires-Dist: cpm_kernels; extra == "default"
 Requires-Dist: termcolor; extra == "default"
-Requires-Dist: python-dotenv==1.0.0; extra == "default"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
-Requires-Dist: transformers>=4.34.0; extra == "default"
-Requires-Dist: coloredlogs; extra == "default"
-Requires-Dist: auto-gpt-plugin-template; extra == "default"
-Requires-Dist: jsonschema; extra == "default"
-Requires-Dist: pydantic>=2.6.0; extra == "default"
-Requires-Dist: click; extra == "default"
-Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: prettytable; extra == "default"
 Requires-Dist: sqlparse==0.4.4; extra == "default"
-Requires-Dist: cachetools; extra == "default"
-Requires-Dist: jinja2; extra == "default"
-Requires-Dist: colorama==0.4.6; extra == "default"
-Requires-Dist: gTTS==2.3.1; extra == "default"
-Requires-Dist: langchain>=0.0.286; extra == "default"
-Requires-Dist: seaborn; extra == "default"
-Requires-Dist: alembic==1.12.0; extra == "default"
+Requires-Dist: accelerate>=0.20.3; extra == "default"
 Requires-Dist: pandas==2.0.3; extra == "default"
-Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: graphviz; extra == "default"
 Requires-Dist: torchvision==0.17.1; extra == "default"
-Requires-Dist: spacy>=3.7; extra == "default"
-Requires-Dist: torchaudio==2.2.1; extra == "default"
-Requires-Dist: cpm_kernels; extra == "default"
-Requires-Dist: torch==2.2.1; extra == "default"
-Requires-Dist: importlib-resources==5.12.0; extra == "default"
-Requires-Dist: duckdb-engine; extra == "default"
-Requires-Dist: pympler; extra == "default"
-Requires-Dist: openpyxl==3.1.2; extra == "default"
-Requires-Dist: typeguard; extra == "default"
-Requires-Dist: rich; extra == "default"
+Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: jsonschema; extra == "default"
+Requires-Dist: python-dotenv==1.0.0; extra == "default"
+Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: duckdb; extra == "default"
+Requires-Dist: shortuuid; extra == "default"
 Provides-Extra: all
-Requires-Dist: fastapi>=0.100.0; extra == "all"
-Requires-Dist: python-multipart; extra == "all"
-Requires-Dist: pyspark; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: rocksdict; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: shortuuid; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: tomlkit; extra == "all"
-Requires-Dist: pypdf; extra == "all"
-Requires-Dist: bs4; extra == "all"
-Requires-Dist: auto-gptq; extra == "all"
-Requires-Dist: markdown; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
-Requires-Dist: openai; extra == "all"
 Requires-Dist: click; extra == "all"
-Requires-Dist: neo4j; extra == "all"
-Requires-Dist: torchvision==0.17.1; extra == "all"
-Requires-Dist: torchaudio==2.2.1; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
-Requires-Dist: thrift; extra == "all"
+Requires-Dist: fschat; extra == "all"
 Requires-Dist: importlib-resources==5.12.0; extra == "all"
+Requires-Dist: typeguard; extra == "all"
+Requires-Dist: thrift; extra == "all"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
 Requires-Dist: gpt4all; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: gTTS==2.3.1; extra == "all"
+Requires-Dist: clickhouse-connect; extra == "all"
+Requires-Dist: dashscope; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: cpm_kernels; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: sqlparse==0.4.4; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
 Requires-Dist: duckdb; extra == "all"
-Requires-Dist: aiohttp==3.8.4; extra == "all"
-Requires-Dist: aiofiles; extra == "all"
+Requires-Dist: shortuuid; extra == "all"
+Requires-Dist: torchaudio==2.2.1; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: markdown; extra == "all"
 Requires-Dist: pymysql; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: python-docx; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: vllm; extra == "all"
-Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: rocksdict; extra == "all"
+Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: pypdf; extra == "all"
+Requires-Dist: openpyxl==3.1.2; extra == "all"
+Requires-Dist: bs4; extra == "all"
 Requires-Dist: chromadb>=0.4.22; extra == "all"
-Requires-Dist: tiktoken; extra == "all"
-Requires-Dist: pymssql; extra == "all"
-Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: pyspark; extra == "all"
 Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: langchain>=0.0.286; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
-Requires-Dist: openpyxl==3.1.2; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: autoawq; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: bitsandbytes; extra == "all"
-Requires-Dist: chardet; extra == "all"
 Requires-Dist: httpx; extra == "all"
-Requires-Dist: optimum; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
+Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: cachetools; extra == "all"
 Requires-Dist: transformers>=4.34.0; extra == "all"
-Requires-Dist: jsonschema; extra == "all"
+Requires-Dist: pymssql; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
+Requires-Dist: aiohttp==3.8.4; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
+Requires-Dist: spacy>=3.7; extra == "all"
+Requires-Dist: pympler; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: fastapi>=0.100.0; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: python-docx; extra == "all"
+Requires-Dist: pyhive; extra == "all"
 Requires-Dist: pydantic>=2.6.0; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: gTTS==2.3.1; extra == "all"
-Requires-Dist: seaborn; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
+Requires-Dist: pandas==2.0.3; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
+Requires-Dist: tiktoken; extra == "all"
 Requires-Dist: xlrd==2.0.1; extra == "all"
-Requires-Dist: schedule; extra == "all"
-Requires-Dist: rich; extra == "all"
-Requires-Dist: fschat; extra == "all"
 Requires-Dist: msgpack; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: termcolor; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
-Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: cachetools; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: rich; extra == "all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
 Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: pyhive; extra == "all"
-Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: spacy>=3.7; extra == "all"
+Requires-Dist: langchain>=0.0.286; extra == "all"
 Requires-Dist: torch==2.2.1; extra == "all"
-Requires-Dist: pympler; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
+Requires-Dist: aiofiles; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: python-multipart; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
+Requires-Dist: vllm; extra == "all"
 Requires-Dist: auto-gpt-plugin-template; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: weaviate-client; extra == "all"
+Requires-Dist: jsonschema; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
 
@@ -566,18 +553,14 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
-    - 🔥🔥🔥  [Qwen1.5-MoE-A2.7B-Chat](https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat)
-    - 🔥🔥🔥  [Meta-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct)
-    - 🔥🔥🔥  [Meta-Llama-3-8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct)
-    - 🔥🔥🔥  [CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat)
     - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
     - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
     - 🔥🔥🔥  [gemma-7b-it](https://huggingface.co/google/gemma-7b-it)
     - 🔥🔥🔥  [gemma-2b-it](https://huggingface.co/google/gemma-2b-it)
     - 🔥🔥🔥  [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)
     - 🔥🔥🔥  [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1)
     - 🔥🔥🔥  [Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)
```

### Comparing `dbgpt-0.5.5/dbgpt.egg-info/SOURCES.txt` & `dbgpt-0.5.5rc0/dbgpt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,14 @@
 dbgpt/core/operators/flow/composer_operator.py
 dbgpt/core/operators/flow/dict_operator.py
 dbgpt/core/schema/__init__.py
 dbgpt/core/schema/api.py
 dbgpt/datasource/__init__.py
 dbgpt/datasource/base.py
 dbgpt/datasource/conn_spark.py
-dbgpt/datasource/conn_tugraph.py
 dbgpt/datasource/db_conn_info.py
 dbgpt/datasource/redis.py
 dbgpt/datasource/manages/__init__.py
 dbgpt/datasource/manages/connect_config_db.py
 dbgpt/datasource/manages/connector_manager.py
 dbgpt/datasource/nosql/__init__.py
 dbgpt/datasource/operators/__init__.py
@@ -263,15 +262,14 @@
 dbgpt/rag/retriever/rewrite.py
 dbgpt/rag/schemalinker/__init__.py
 dbgpt/rag/schemalinker/base_linker.py
 dbgpt/rag/schemalinker/schema_linking.py
 dbgpt/rag/summary/__init__.py
 dbgpt/rag/summary/db_summary.py
 dbgpt/rag/summary/db_summary_client.py
-dbgpt/rag/summary/gdbms_db_summary.py
 dbgpt/rag/summary/rdbms_db_summary.py
 dbgpt/rag/text_splitter/__init__.py
 dbgpt/rag/text_splitter/pre_text_splitter.py
 dbgpt/rag/text_splitter/text_splitter.py
 dbgpt/rag/text_splitter/token_splitter.py
 dbgpt/storage/__init__.py
 dbgpt/storage/schema.py
@@ -295,15 +293,14 @@
 dbgpt/storage/metadata/db_storage.py
 dbgpt/storage/vector_store/__init__.py
 dbgpt/storage/vector_store/base.py
 dbgpt/storage/vector_store/chroma_store.py
 dbgpt/storage/vector_store/connector.py
 dbgpt/storage/vector_store/filters.py
 dbgpt/storage/vector_store/milvus_store.py
-dbgpt/storage/vector_store/oceanbase_store.py
 dbgpt/storage/vector_store/pgvector_store.py
 dbgpt/storage/vector_store/weaviate_store.py
 dbgpt/util/__init__.py
 dbgpt/util/_db_migration_utils.py
 dbgpt/util/annotations.py
 dbgpt/util/api_utils.py
 dbgpt/util/chat_util.py
```

### Comparing `dbgpt-0.5.5/dbgpt.egg-info/requires.txt` & `dbgpt-0.5.5rc0/dbgpt.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,423 +3,410 @@
 importlib-resources==5.12.0
 python-dotenv==1.0.0
 cachetools
 pydantic>=2.6.0
 typeguard
 
 [agent]
-fastapi>=0.100.0
-cachetools
-colorama==0.4.6
+click
+chardet==5.1.0
 httpx
 tomlkit
-aiohttp==3.8.4
-python-dotenv==1.0.0
 termcolor
+importlib-resources==5.12.0
+fastapi>=0.100.0
+prettytable
+cachetools
+typeguard
 pandas==2.0.3
-psutil==5.9.4
-click
 rich
+psutil==5.9.4
+aiohttp==3.8.4
+colorama==0.4.6
+python-dotenv==1.0.0
 pydantic>=2.6.0
-importlib-resources==5.12.0
-chardet==5.1.0
-typeguard
-prettytable
 
 [all]
-fastapi>=0.100.0
-python-multipart
-pyspark
-zhipuai
-rocksdict
-uvicorn
-shortuuid
-python-pptx
-tomlkit
-pypdf
-bs4
-auto-gptq
-markdown
-sentencepiece
-coloredlogs
-openai
 click
-neo4j
-torchvision==0.17.1
-torchaudio==2.2.1
-cpm_kernels
-thrift
+fschat
 importlib-resources==5.12.0
+typeguard
+thrift
+SQLAlchemy<2.0.29,>=2.0.25
 gpt4all
+pymilvus
+GitPython
+gTTS==2.3.1
+clickhouse-connect
+dashscope
+sentence-transformers
+cpm_kernels
+openai
+sqlparse==0.4.4
+graphviz
+python-dotenv==1.0.0
 duckdb
-aiohttp==3.8.4
-aiofiles
+shortuuid
+torchaudio==2.2.1
+duckdb-engine
+markdown
 pymysql
-tokenizers>=0.14
-python-docx
-graphviz
-vllm
-psycopg2
+rocksdict
+bitsandbytes
+pypdf
+openpyxl==3.1.2
+bs4
 chromadb>=0.4.22
-tiktoken
-pymssql
-thrift_sasl
+pyspark
 chardet==5.1.0
-langchain>=0.0.286
-alembic==1.12.0
-duckdb-engine
-openpyxl==3.1.2
-typeguard
-autoawq
-mysqlclient==2.1.0
-GitPython
-bitsandbytes
-chardet
 httpx
-optimum
-psutil==5.9.4
-pydoris<2.0.0,>=1.0.2
-llama-cpp-python
-dashscope
-SQLAlchemy<2.0.29,>=2.0.25
+tomlkit
+cachetools
 transformers>=4.34.0
-jsonschema
+pymssql
+termcolor
+accelerate>=0.20.3
+aiohttp==3.8.4
+uvicorn
+sentencepiece
+spacy>=3.7
+pympler
+alembic==1.12.0
+chardet
+psycopg2
+fastapi>=0.100.0
+schedule
+python-docx
+pyhive
 pydantic>=2.6.0
-jinja2
-gTTS==2.3.1
-seaborn
+python-pptx
+zhipuai
+pandas==2.0.3
+torchvision==0.17.1
+tiktoken
 xlrd==2.0.1
-schedule
-rich
-fschat
 msgpack
-pymilvus
-prettytable
-weaviate-client
-clickhouse-connect
-sentence-transformers
-accelerate>=0.20.3
-termcolor
-python-dotenv==1.0.0
-sqlparse==0.4.4
-cachetools
+mysqlclient==2.1.0
+rich
+pydoris<2.0.0,>=1.0.2
 colorama==0.4.6
-pyhive
-pandas==2.0.3
-spacy>=3.7
+langchain>=0.0.286
 torch==2.2.1
-pympler
+coloredlogs
+aiofiles
+llama-cpp-python
+seaborn
+jinja2
+python-multipart
+tokenizers>=0.14
+vllm
 auto-gpt-plugin-template
+psutil==5.9.4
+thrift_sasl
+prettytable
+weaviate-client
+jsonschema
 
 [bitsandbytes]
 bitsandbytes
 
 [cache]
 rocksdict
 
 [cli]
-fastapi>=0.100.0
-cachetools
-colorama==0.4.6
+click
+chardet==5.1.0
 httpx
 tomlkit
+importlib-resources==5.12.0
+fastapi>=0.100.0
+prettytable
+cachetools
+typeguard
+rich
+psutil==5.9.4
 aiohttp==3.8.4
+colorama==0.4.6
 python-dotenv==1.0.0
-psutil==5.9.4
-click
-rich
 pydantic>=2.6.0
-importlib-resources==5.12.0
-chardet==5.1.0
-typeguard
-prettytable
 
 [client]
+chardet==5.1.0
+httpx
+importlib-resources==5.12.0
 fastapi>=0.100.0
 cachetools
-httpx
+typeguard
 aiohttp==3.8.4
 python-dotenv==1.0.0
 pydantic>=2.6.0
-importlib-resources==5.12.0
-chardet==5.1.0
-typeguard
 
 [core]
+chardet==5.1.0
+importlib-resources==5.12.0
 cachetools
+typeguard
 aiohttp==3.8.4
 python-dotenv==1.0.0
 pydantic>=2.6.0
-importlib-resources==5.12.0
-chardet==5.1.0
-typeguard
 
 [datasource]
 pymysql
 
 [datasource_all]
 pymssql
 pyspark
+clickhouse-connect
 thrift_sasl
-psycopg2
 mysqlclient==2.1.0
 pydoris<2.0.0,>=1.0.2
 pyhive
-clickhouse-connect
 pymysql
 thrift
-neo4j
+psycopg2
 
 [default]
+click
 fschat
-fastapi>=0.100.0
+torchaudio==2.2.1
 msgpack
-python-multipart
-zhipuai
-autoawq
-duckdb
+uvicorn
+importlib-resources==5.12.0
+sentencepiece
+typeguard
+rich
+duckdb-engine
+spacy>=3.7
+pymysql
+markdown
+colorama==0.4.6
 rocksdict
-aiohttp==3.8.4
+langchain>=0.0.286
+pympler
+alembic==1.12.0
+torch==2.2.1
+chardet
+SQLAlchemy<2.0.29,>=2.0.25
+coloredlogs
 aiofiles
-uvicorn
+pypdf
+seaborn
+openpyxl==3.1.2
+jinja2
+fastapi>=0.100.0
+python-multipart
+bs4
+tokenizers>=0.14
 schedule
 GitPython
-bitsandbytes
-shortuuid
-pymysql
-python-pptx
-tokenizers>=0.14
-chardet
-prettytable
-python-docx
-graphviz
-tomlkit
-httpx
-optimum
 chromadb>=0.4.22
-pypdf
+chardet==5.1.0
+httpx
+tomlkit
+gTTS==2.3.1
+python-docx
+cachetools
+auto-gpt-plugin-template
+dashscope
+pydantic>=2.6.0
 psutil==5.9.4
-bs4
-auto-gptq
+transformers>=4.34.0
 sentence-transformers
-markdown
-accelerate>=0.20.3
-dashscope
-sentencepiece
+zhipuai
+python-pptx
+cpm_kernels
 termcolor
-python-dotenv==1.0.0
-SQLAlchemy<2.0.29,>=2.0.25
-transformers>=4.34.0
-coloredlogs
-auto-gpt-plugin-template
-jsonschema
-pydantic>=2.6.0
-click
-chardet==5.1.0
+prettytable
 sqlparse==0.4.4
-cachetools
-jinja2
-colorama==0.4.6
-gTTS==2.3.1
-langchain>=0.0.286
-seaborn
-alembic==1.12.0
+accelerate>=0.20.3
 pandas==2.0.3
-xlrd==2.0.1
+graphviz
 torchvision==0.17.1
-spacy>=3.7
-torchaudio==2.2.1
-cpm_kernels
-torch==2.2.1
-importlib-resources==5.12.0
-duckdb-engine
-pympler
-openpyxl==3.1.2
-typeguard
-rich
+aiohttp==3.8.4
+jsonschema
+python-dotenv==1.0.0
+xlrd==2.0.1
+duckdb
+shortuuid
 
 [framework]
+click
 fschat
-fastapi>=0.100.0
 msgpack
-duckdb
-aiohttp==3.8.4
-aiofiles
 uvicorn
-schedule
-GitPython
-shortuuid
+importlib-resources==5.12.0
+typeguard
+rich
+duckdb-engine
 pymysql
-prettytable
-graphviz
-tomlkit
-httpx
-psutil==5.9.4
-termcolor
-python-dotenv==1.0.0
+colorama==0.4.6
+pympler
+alembic==1.12.0
 SQLAlchemy<2.0.29,>=2.0.25
-transformers>=4.34.0
 coloredlogs
+aiofiles
+seaborn
+openpyxl==3.1.2
+jinja2
+fastapi>=0.100.0
+GitPython
+schedule
+chardet==5.1.0
+httpx
+tomlkit
+gTTS==2.3.1
+cachetools
 auto-gpt-plugin-template
-jsonschema
+transformers>=4.34.0
 pydantic>=2.6.0
-click
-chardet==5.1.0
+psutil==5.9.4
+termcolor
+prettytable
 sqlparse==0.4.4
-cachetools
-jinja2
-colorama==0.4.6
-gTTS==2.3.1
-seaborn
-alembic==1.12.0
 pandas==2.0.3
+graphviz
+aiohttp==3.8.4
+jsonschema
+python-dotenv==1.0.0
 xlrd==2.0.1
-importlib-resources==5.12.0
-duckdb-engine
-pympler
-openpyxl==3.1.2
-typeguard
-rich
+duckdb
+shortuuid
 
 [gpt4all]
 gpt4all
 
 [llama_cpp]
 llama-cpp-python
 
 [openai]
+click
 fschat
-fastapi>=0.100.0
 msgpack
-python-multipart
-duckdb
-aiohttp==3.8.4
-aiofiles
 uvicorn
-schedule
-GitPython
-shortuuid
+importlib-resources==5.12.0
+typeguard
+rich
+duckdb-engine
+spacy>=3.7
 pymysql
-python-pptx
-prettytable
-python-docx
-graphviz
-tomlkit
-httpx
-chromadb>=0.4.22
-pypdf
-psutil==5.9.4
-tiktoken
-bs4
-sentence-transformers
 markdown
-termcolor
-python-dotenv==1.0.0
+colorama==0.4.6
+langchain>=0.0.286
+pympler
+alembic==1.12.0
 SQLAlchemy<2.0.29,>=2.0.25
-transformers>=4.34.0
 coloredlogs
+aiofiles
+pypdf
+seaborn
+openpyxl==3.1.2
+jinja2
+fastapi>=0.100.0
+python-multipart
+bs4
+GitPython
+schedule
+chromadb>=0.4.22
+chardet==5.1.0
+httpx
+tomlkit
+gTTS==2.3.1
+python-docx
+cachetools
 auto-gpt-plugin-template
-jsonschema
+transformers>=4.34.0
 pydantic>=2.6.0
+psutil==5.9.4
+sentence-transformers
+python-pptx
+termcolor
 openai
-click
-chardet==5.1.0
+prettytable
 sqlparse==0.4.4
-cachetools
-jinja2
-colorama==0.4.6
-gTTS==2.3.1
-langchain>=0.0.286
-seaborn
-alembic==1.12.0
 pandas==2.0.3
+graphviz
+tiktoken
+aiohttp==3.8.4
+jsonschema
+python-dotenv==1.0.0
 xlrd==2.0.1
-spacy>=3.7
-importlib-resources==5.12.0
-duckdb-engine
-pympler
-openpyxl==3.1.2
-typeguard
-rich
+duckdb
+shortuuid
 
 [quantization]
-autoawq
-optimum
-bitsandbytes
-auto-gptq
 cpm_kernels
 
 [rag]
+pypdf
+python-pptx
 python-docx
+spacy>=3.7
+markdown
 python-multipart
+sentence-transformers
 langchain>=0.0.286
-chromadb>=0.4.22
-pypdf
-spacy>=3.7
 bs4
-sentence-transformers
-markdown
-python-pptx
+chromadb>=0.4.22
 
 [simple_framework]
+click
 fschat
-fastapi>=0.100.0
 msgpack
-duckdb
-aiohttp==3.8.4
 uvicorn
+importlib-resources==5.12.0
+typeguard
+rich
+duckdb-engine
+colorama==0.4.6
+pympler
+SQLAlchemy<2.0.29,>=2.0.25
+jinja2
+fastapi>=0.100.0
 schedule
-shortuuid
-prettytable
-tomlkit
+chardet==5.1.0
 httpx
+tomlkit
+cachetools
+pydantic>=2.6.0
 psutil==5.9.4
 termcolor
-python-dotenv==1.0.0
-SQLAlchemy<2.0.29,>=2.0.25
-pydantic>=2.6.0
-click
-chardet==5.1.0
+prettytable
 sqlparse==0.4.4
-cachetools
-jinja2
-colorama==0.4.6
 pandas==2.0.3
-importlib-resources==5.12.0
-duckdb-engine
-pympler
-typeguard
-rich
+aiohttp==3.8.4
+python-dotenv==1.0.0
+duckdb
+shortuuid
 
 [torch]
-torch==2.2.1
 torchvision==0.17.1
+torch==2.2.1
 torchaudio==2.2.1
 
 [torch_cpu]
-torch==2.2.1
 torchvision==0.17.1
+torch==2.2.1
 torchaudio==2.2.1
 
 [torch_cuda]
-torch==2.2.1
 torchvision==0.17.1
+torch==2.2.1
 torchaudio==2.2.1
 
 [vllm]
 vllm
 
 [vstore]
 chromadb>=0.4.22
 
 [vstore_all]
-weaviate-client
-chromadb>=0.4.22
 pymilvus
+chromadb>=0.4.22
+weaviate-client
 
 [vstore_milvus]
-chromadb>=0.4.22
 pymilvus
+chromadb>=0.4.22
 
 [vstore_weaviate]
-weaviate-client
 chromadb>=0.4.22
+weaviate-client
```

### Comparing `dbgpt-0.5.5/setup.py` & `dbgpt-0.5.5rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,25 @@
 
 with open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 IS_DEV_MODE = os.getenv("IS_DEV_MODE", "true").lower() == "true"
 # If you modify the version, please modify the version in the following files:
 # dbgpt/_version.py
-DB_GPT_VERSION = os.getenv("DB_GPT_VERSION", "0.5.5")
+DB_GPT_VERSION = os.getenv("DB_GPT_VERSION", "0.5.4")
 
 BUILD_NO_CACHE = os.getenv("BUILD_NO_CACHE", "true").lower() == "true"
 LLAMA_CPP_GPU_ACCELERATION = (
     os.getenv("LLAMA_CPP_GPU_ACCELERATION", "true").lower() == "true"
 )
 BUILD_FROM_SOURCE = os.getenv("BUILD_FROM_SOURCE", "false").lower() == "true"
 BUILD_FROM_SOURCE_URL_FAST_CHAT = os.getenv(
     "BUILD_FROM_SOURCE_URL_FAST_CHAT", "git+https://github.com/lm-sys/FastChat.git"
 )
 BUILD_VERSION_OPENAI = os.getenv("BUILD_VERSION_OPENAI")
-INCLUDE_QUANTIZATION = os.getenv("INCLUDE_QUANTIZATION", "true").lower() == "true"
 
 
 def parse_requirements(file_name: str) -> List[str]:
     with open(file_name) as f:
         return [
             require.strip()
             for require in f
@@ -342,24 +341,24 @@
             "torchvision",
             torchvision_version,
             base_url_func=base_url_func,
             supported_cuda_versions=supported_versions,
         )
 
         # Cache and add CUDA-dependent packages if URLs are available
-        # if torch_url:
-        #     torch_url_cached = cache_package(
-        #         torch_url, "torch", os_type == OSType.WINDOWS
-        #     )
-        #     torch_cuda_pkgs[0] = f"torch @ {torch_url_cached}"
-        # if torchvision_url:
-        #     torchvision_url_cached = cache_package(
-        #         torchvision_url, "torchvision", os_type == OSType.WINDOWS
-        #     )
-        #     torch_cuda_pkgs[1] = f"torchvision @ {torchvision_url_cached}"
+        if torch_url:
+            torch_url_cached = cache_package(
+                torch_url, "torch", os_type == OSType.WINDOWS
+            )
+            torch_cuda_pkgs[0] = f"torch @ {torch_url_cached}"
+        if torchvision_url:
+            torchvision_url_cached = cache_package(
+                torchvision_url, "torchvision", os_type == OSType.WINDOWS
+            )
+            torch_cuda_pkgs[1] = f"torchvision @ {torchvision_url_cached}"
 
     # Assuming 'setup_spec' is a dictionary where we're adding these dependencies
     setup_spec.extras["torch"] = torch_pkgs
     setup_spec.extras["torch_cpu"] = torch_pkgs
     setup_spec.extras["torch_cuda"] = torch_cuda_pkgs
 
 
@@ -396,15 +395,15 @@
     llama_cpp_version = "0.2.26"
     py_version = "cp310"
     os_pkg_name = "manylinux_2_31_x86_64" if os_type == OSType.LINUX else "win_amd64"
     extra_index_url = f"{base_url}/llama_cpp_python_cuda-{llama_cpp_version}+{device}-{py_version}-{py_version}-{os_pkg_name}.whl"
     extra_index_url, _ = encode_url(extra_index_url)
     print(f"Install llama_cpp_python_cuda from {extra_index_url}")
 
-    # setup_spec.extras["llama_cpp"].append(f"llama_cpp_python_cuda @ {extra_index_url}")
+    setup_spec.extras["llama_cpp"].append(f"llama_cpp_python_cuda @ {extra_index_url}")
 
 
 def core_requires():
     """
     pip install dbgpt or pip install "dbgpt[core]"
     """
     setup_spec.extras["core"] = [
@@ -549,17 +548,15 @@
         autoawq_latest_version = get_latest_version("autoawq", "", "0.2.4")
         if cuda_version is None or cuda_version == "12.1":
             quantization_pkgs.extend(["autoawq", _build_autoawq_requires(), "optimum"])
         else:
             # TODO(yyhhyy): Add autoawq install method for CUDA version 11.8
             quantization_pkgs.extend(["autoawq", _build_autoawq_requires(), "optimum"])
 
-    setup_spec.extras["quantization"] = (
-        ["cpm_kernels"] + quantization_pkgs + setup_spec.extras["bitsandbytes"]
-    )
+    setup_spec.extras["quantization"] = ["cpm_kernels"] + quantization_pkgs
 
 
 def all_vector_store_requires():
     """
     pip install "dbgpt[vstore]"
     """
     setup_spec.extras["vstore"] = [
@@ -602,15 +599,14 @@
         "mysqlclient==2.1.0",
         # pydoris is too old, we should find a new package to replace it.
         "pydoris>=1.0.2,<2.0.0",
         "clickhouse-connect",
         "pyhive",
         "thrift",
         "thrift_sasl",
-        "neo4j",
     ]
 
 
 def openai_requires():
     """
     pip install "dbgpt[openai]"
     """
@@ -659,17 +655,15 @@
         "chardet",
         "sentencepiece",
     ]
     setup_spec.extras["default"] += setup_spec.extras["framework"]
     setup_spec.extras["default"] += setup_spec.extras["rag"]
     setup_spec.extras["default"] += setup_spec.extras["datasource"]
     setup_spec.extras["default"] += setup_spec.extras["torch"]
-    if INCLUDE_QUANTIZATION:
-        # Add quantization extra to default, default is True
-        setup_spec.extras["default"] += setup_spec.extras["quantization"]
+    setup_spec.extras["default"] += setup_spec.extras["quantization"]
     setup_spec.extras["default"] += setup_spec.extras["cache"]
 
 
 def all_requires():
     requires = set()
     for _, pkgs in setup_spec.extras.items():
         for pkg in pkgs:
```

