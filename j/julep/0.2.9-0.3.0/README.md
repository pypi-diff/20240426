# Comparing `tmp/julep-0.2.9.tar.gz` & `tmp/julep-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julep-0.2.9.tar", max compression
+gzip compressed data, was "julep-0.3.0.tar", max compression
```

## Comparing `julep-0.2.9.tar` & `julep-0.3.0.tar`

### file list

```diff
@@ -1,105 +1,108 @@
--rw-r--r--   0        0        0      121 2024-02-10 10:42:24.049214 julep-0.2.9/README.md
--rw-r--r--   0        0        0      326 2024-02-29 08:57:18.582002 julep-0.2.9/julep/__init__.py
--rw-r--r--   0        0        0     4077 2024-03-14 08:00:14.081169 julep-0.2.9/julep/api/__init__.py
--rw-r--r--   0        0        0   132894 2024-03-14 08:01:07.660220 julep-0.2.9/julep/api/client.py
--rw-r--r--   0        0        0      519 2024-03-14 07:55:57.885744 julep-0.2.9/julep/api/core/__init__.py
--rw-r--r--   0        0        0      440 2024-03-14 07:56:06.133596 julep-0.2.9/julep/api/core/api_error.py
--rw-r--r--   0        0        0      972 2024-03-14 07:55:57.885744 julep-0.2.9/julep/api/core/client_wrapper.py
--rw-r--r--   0        0        0     1069 2024-03-14 07:56:06.141595 julep-0.2.9/julep/api/core/datetime_utils.py
--rw-r--r--   0        0        0     3825 2024-03-14 07:56:06.213594 julep-0.2.9/julep/api/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-14 07:55:57.885744 julep-0.2.9/julep/api/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      164 2024-03-14 07:55:57.889744 julep-0.2.9/julep/api/environment.py
--rw-r--r--   0        0        0     6258 2024-03-14 08:00:14.085168 julep-0.2.9/julep/api/types/__init__.py
--rw-r--r--   0        0        0     2026 2024-03-14 07:56:06.169595 julep-0.2.9/julep/api/types/agent.py
--rw-r--r--   0        0        0     3189 2024-03-14 07:56:06.169595 julep-0.2.9/julep/api/types/agent_default_settings.py
--rw-r--r--   0        0        0     1883 2024-03-14 07:55:57.909744 julep-0.2.9/julep/api/types/agent_default_settings_preset.py
--rw-r--r--   0        0        0      988 2024-03-14 07:56:06.145595 julep-0.2.9/julep/api/types/agent_metadata.py
--rw-r--r--   0        0        0     1675 2024-03-14 07:56:06.157595 julep-0.2.9/julep/api/types/chat_input_data.py
--rw-r--r--   0        0        0      251 2024-03-14 08:00:14.085168 julep-0.2.9/julep/api/types/chat_input_data_tool_choice.py
--rw-r--r--   0        0        0     1447 2024-03-14 07:56:06.157595 julep-0.2.9/julep/api/types/chat_ml_message.py
--rw-r--r--   0        0        0      901 2024-03-14 07:55:57.913744 julep-0.2.9/julep/api/types/chat_ml_message_role.py
--rw-r--r--   0        0        0     2118 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/chat_response.py
--rw-r--r--   0        0        0     1479 2024-03-14 07:55:57.901744 julep-0.2.9/julep/api/types/chat_response_finish_reason.py
--rw-r--r--   0        0        0     6401 2024-03-14 07:56:06.201594 julep-0.2.9/julep/api/types/chat_settings.py
--rw-r--r--   0        0        0     1787 2024-03-14 07:55:57.913744 julep-0.2.9/julep/api/types/chat_settings_preset.py
--rw-r--r--   0        0        0     2352 2024-03-14 07:56:06.157595 julep-0.2.9/julep/api/types/chat_settings_response_format.py
--rw-r--r--   0        0        0     1037 2024-03-14 07:56:06.129596 julep-0.2.9/julep/api/types/chat_settings_response_format_schema.py
--rw-r--r--   0        0        0      786 2024-03-14 07:55:57.897744 julep-0.2.9/julep/api/types/chat_settings_response_format_type.py
--rw-r--r--   0        0        0      152 2024-03-14 07:55:57.893744 julep-0.2.9/julep/api/types/chat_settings_stop.py
--rw-r--r--   0        0        0     1358 2024-03-14 07:56:06.149595 julep-0.2.9/julep/api/types/completion_usage.py
--rw-r--r--   0        0        0     1001 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/create_agent_request_metadata.py
--rw-r--r--   0        0        0     1295 2024-03-14 07:56:06.153595 julep-0.2.9/julep/api/types/create_doc.py
--rw-r--r--   0        0        0      992 2024-03-14 07:56:06.149595 julep-0.2.9/julep/api/types/create_doc_metadata.py
--rw-r--r--   0        0        0     1003 2024-03-14 07:56:06.149595 julep-0.2.9/julep/api/types/create_session_request_metadata.py
--rw-r--r--   0        0        0     1329 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/create_tool_request.py
--rw-r--r--   0        0        0      646 2024-03-14 07:56:06.141595 julep-0.2.9/julep/api/types/create_tool_request_type.py
--rw-r--r--   0        0        0     1000 2024-03-14 07:56:06.157595 julep-0.2.9/julep/api/types/create_user_request_metadata.py
--rw-r--r--   0        0        0     1399 2024-03-14 07:56:06.169595 julep-0.2.9/julep/api/types/doc.py
--rw-r--r--   0        0        0      986 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/doc_metadata.py
--rw-r--r--   0        0        0     1159 2024-03-14 07:56:06.165595 julep-0.2.9/julep/api/types/function_call_option.py
--rw-r--r--   0        0        0     1493 2024-03-14 07:56:06.177595 julep-0.2.9/julep/api/types/function_def.py
--rw-r--r--   0        0        0      130 2024-03-14 07:55:57.909744 julep-0.2.9/julep/api/types/function_parameters.py
--rw-r--r--   0        0        0      485 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/get_agent_docs_request_order.py
--rw-r--r--   0        0        0      570 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/get_agent_docs_request_sort_by.py
--rw-r--r--   0        0        0     1023 2024-03-14 07:56:06.173595 julep-0.2.9/julep/api/types/get_agent_docs_response.py
--rw-r--r--   0        0        0     1036 2024-03-14 07:56:06.177595 julep-0.2.9/julep/api/types/get_agent_memories_response.py
--rw-r--r--   0        0        0     1027 2024-03-14 07:56:06.177595 julep-0.2.9/julep/api/types/get_agent_tools_response.py
--rw-r--r--   0        0        0     1053 2024-03-14 07:56:06.181595 julep-0.2.9/julep/api/types/get_history_response.py
--rw-r--r--   0        0        0     1046 2024-03-14 07:56:06.185595 julep-0.2.9/julep/api/types/get_suggestions_response.py
--rw-r--r--   0        0        0      482 2024-03-14 07:56:06.173595 julep-0.2.9/julep/api/types/get_user_docs_request_order.py
--rw-r--r--   0        0        0      567 2024-03-14 07:56:06.173595 julep-0.2.9/julep/api/types/get_user_docs_request_sort_by.py
--rw-r--r--   0        0        0     1022 2024-03-14 07:56:06.181595 julep-0.2.9/julep/api/types/get_user_docs_response.py
--rw-r--r--   0        0        0     1511 2024-03-14 07:56:06.201594 julep-0.2.9/julep/api/types/input_chat_ml_message.py
--rw-r--r--   0        0        0     1063 2024-03-14 07:55:57.913744 julep-0.2.9/julep/api/types/input_chat_ml_message_role.py
--rw-r--r--   0        0        0     1224 2024-03-14 07:56:06.185595 julep-0.2.9/julep/api/types/instruction.py
--rw-r--r--   0        0        0     1819 2024-03-14 07:56:06.201594 julep-0.2.9/julep/api/types/job_status.py
--rw-r--r--   0        0        0     1361 2024-03-14 07:55:57.901744 julep-0.2.9/julep/api/types/job_status_state.py
--rw-r--r--   0        0        0      479 2024-03-14 07:56:06.177595 julep-0.2.9/julep/api/types/list_agents_request_order.py
--rw-r--r--   0        0        0      564 2024-03-14 07:56:06.193595 julep-0.2.9/julep/api/types/list_agents_request_sort_by.py
--rw-r--r--   0        0        0     1010 2024-03-14 07:56:06.189595 julep-0.2.9/julep/api/types/list_agents_response.py
--rw-r--r--   0        0        0      485 2024-03-14 07:56:06.181595 julep-0.2.9/julep/api/types/list_sessions_request_order.py
--rw-r--r--   0        0        0      570 2024-03-14 07:56:06.181595 julep-0.2.9/julep/api/types/list_sessions_request_sort_by.py
--rw-r--r--   0        0        0     1018 2024-03-14 07:56:06.193595 julep-0.2.9/julep/api/types/list_sessions_response.py
--rw-r--r--   0        0        0      476 2024-03-14 07:56:06.185595 julep-0.2.9/julep/api/types/list_users_request_order.py
--rw-r--r--   0        0        0      561 2024-03-14 07:56:06.185595 julep-0.2.9/julep/api/types/list_users_request_sort_by.py
--rw-r--r--   0        0        0     1006 2024-03-14 07:56:06.197595 julep-0.2.9/julep/api/types/list_users_response.py
--rw-r--r--   0        0        0     2233 2024-03-14 07:56:06.221594 julep-0.2.9/julep/api/types/memory.py
--rw-r--r--   0        0        0     1231 2024-03-14 08:00:14.085168 julep-0.2.9/julep/api/types/memory_access_options.py
--rw-r--r--   0        0        0     4640 2024-03-14 07:55:57.913744 julep-0.2.9/julep/api/types/memory_emotions_item.py
--rw-r--r--   0        0        0      550 2024-03-14 07:56:06.193595 julep-0.2.9/julep/api/types/memory_type.py
--rw-r--r--   0        0        0     1240 2024-03-14 07:56:06.217594 julep-0.2.9/julep/api/types/named_tool_choice.py
--rw-r--r--   0        0        0     1040 2024-03-14 07:56:06.209594 julep-0.2.9/julep/api/types/named_tool_choice_function.py
--rw-r--r--   0        0        0     1000 2024-03-14 07:56:06.205594 julep-0.2.9/julep/api/types/patch_agent_request_metadata.py
--rw-r--r--   0        0        0     1002 2024-03-14 07:56:06.205594 julep-0.2.9/julep/api/types/patch_session_request_metadata.py
--rw-r--r--   0        0        0      999 2024-03-14 07:56:06.209594 julep-0.2.9/julep/api/types/patch_user_request_metadata.py
--rw-r--r--   0        0        0     1143 2024-03-14 07:56:06.217594 julep-0.2.9/julep/api/types/resource_created_response.py
--rw-r--r--   0        0        0     1000 2024-03-14 08:00:14.085168 julep-0.2.9/julep/api/types/resource_deleted_response.py
--rw-r--r--   0        0        0     1143 2024-03-14 07:56:06.213594 julep-0.2.9/julep/api/types/resource_updated_response.py
--rw-r--r--   0        0        0     1937 2024-03-14 07:56:06.225594 julep-0.2.9/julep/api/types/session.py
--rw-r--r--   0        0        0      990 2024-03-14 07:56:06.217594 julep-0.2.9/julep/api/types/session_metadata.py
--rw-r--r--   0        0        0     1502 2024-03-14 07:56:06.233594 julep-0.2.9/julep/api/types/suggestion.py
--rw-r--r--   0        0        0      546 2024-03-14 07:56:06.213594 julep-0.2.9/julep/api/types/suggestion_target.py
--rw-r--r--   0        0        0     1327 2024-03-14 07:56:06.225594 julep-0.2.9/julep/api/types/tool.py
--rw-r--r--   0        0        0       88 2024-03-14 07:55:57.897744 julep-0.2.9/julep/api/types/tool_choice_option.py
--rw-r--r--   0        0        0      607 2024-03-14 07:56:06.217594 julep-0.2.9/julep/api/types/tool_type.py
--rw-r--r--   0        0        0     1001 2024-03-14 07:56:06.225594 julep-0.2.9/julep/api/types/update_agent_request_metadata.py
--rw-r--r--   0        0        0     1003 2024-03-14 07:56:06.225594 julep-0.2.9/julep/api/types/update_session_request_metadata.py
--rw-r--r--   0        0        0     1000 2024-03-14 07:56:06.229594 julep-0.2.9/julep/api/types/update_user_request_metadata.py
--rw-r--r--   0        0        0     1557 2024-03-14 07:56:06.233594 julep-0.2.9/julep/api/types/user.py
--rw-r--r--   0        0        0      987 2024-03-14 07:56:06.225594 julep-0.2.9/julep/api/types/user_metadata.py
--rw-r--r--   0        0        0    11519 2024-03-14 08:00:32.588841 julep-0.2.9/julep/client.py
--rw-r--r--   0        0        0      277 2024-03-09 05:49:53.102445 julep-0.2.9/julep/env.py
--rw-r--r--   0        0        0        0 2024-02-10 10:42:24.053213 julep-0.2.9/julep/managers/__init__.py
--rw-r--r--   0        0        0    31392 2024-03-14 05:13:36.947764 julep-0.2.9/julep/managers/agent.py
--rw-r--r--   0        0        0     1015 2024-02-10 10:42:24.053213 julep-0.2.9/julep/managers/base.py
--rw-r--r--   0        0        0    20539 2024-03-14 05:13:36.947764 julep-0.2.9/julep/managers/doc.py
--rw-r--r--   0        0        0     7674 2024-02-10 10:42:24.053213 julep-0.2.9/julep/managers/memory.py
--rw-r--r--   0        0        0    43912 2024-03-14 05:13:36.951764 julep-0.2.9/julep/managers/session.py
--rw-r--r--   0        0        0    18487 2024-02-16 12:27:51.553366 julep-0.2.9/julep/managers/tool.py
--rw-r--r--   0        0        0     1297 2024-03-09 05:49:53.102445 julep-0.2.9/julep/managers/types.py
--rw-r--r--   0        0        0    18865 2024-03-14 05:13:36.951764 julep-0.2.9/julep/managers/user.py
--rw-r--r--   0        0        0     1115 2024-03-09 05:49:53.102445 julep-0.2.9/julep/managers/utils.py
--rw-r--r--   0        0        0        0 2024-03-09 05:49:53.102445 julep-0.2.9/julep/utils/__init__.py
--rw-r--r--   0        0        0    12819 2024-03-09 05:49:53.102445 julep-0.2.9/julep/utils/openai_patch.py
--rw-r--r--   0        0        0     1659 2024-03-14 08:33:37.007294 julep-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 julep-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      121 2024-04-09 11:11:10.306527 julep-0.3.0/README.md
+-rw-r--r--   0        0        0      326 2024-04-05 09:31:45.036791 julep-0.3.0/julep/__init__.py
+-rw-r--r--   0        0        0     4325 2024-04-26 05:08:20.800959 julep-0.3.0/julep/api/__init__.py
+-rw-r--r--   0        0        0   134983 2024-04-26 06:24:15.533309 julep-0.3.0/julep/api/client.py
+-rw-r--r--   0        0        0      519 2024-04-26 05:08:20.796959 julep-0.3.0/julep/api/core/__init__.py
+-rw-r--r--   0        0        0      440 2024-04-26 05:08:52.083167 julep-0.3.0/julep/api/core/api_error.py
+-rw-r--r--   0        0        0      972 2024-04-26 05:08:20.796959 julep-0.3.0/julep/api/core/client_wrapper.py
+-rw-r--r--   0        0        0     1069 2024-04-26 05:08:52.087166 julep-0.3.0/julep/api/core/datetime_utils.py
+-rw-r--r--   0        0        0     3825 2024-04-26 05:08:52.159162 julep-0.3.0/julep/api/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-26 05:08:20.796959 julep-0.3.0/julep/api/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      164 2024-04-26 05:08:20.800959 julep-0.3.0/julep/api/environment.py
+-rw-r--r--   0        0        0     6647 2024-04-26 05:08:20.824958 julep-0.3.0/julep/api/types/__init__.py
+-rw-r--r--   0        0        0     2024 2024-04-26 05:08:52.119165 julep-0.3.0/julep/api/types/agent.py
+-rw-r--r--   0        0        0     3189 2024-04-26 05:08:52.123164 julep-0.3.0/julep/api/types/agent_default_settings.py
+-rw-r--r--   0        0        0     1883 2024-04-26 05:08:20.820958 julep-0.3.0/julep/api/types/agent_default_settings_preset.py
+-rw-r--r--   0        0        0      136 2024-04-26 06:24:15.533309 julep-0.3.0/julep/api/types/agent_instructions.py
+-rw-r--r--   0        0        0      988 2024-04-26 05:08:52.095166 julep-0.3.0/julep/api/types/agent_metadata.py
+-rw-r--r--   0        0        0     1675 2024-04-26 05:08:52.107165 julep-0.3.0/julep/api/types/chat_input_data.py
+-rw-r--r--   0        0        0      251 2024-04-26 06:24:15.533309 julep-0.3.0/julep/api/types/chat_input_data_tool_choice.py
+-rw-r--r--   0        0        0     1530 2024-04-26 05:08:52.091166 julep-0.3.0/julep/api/types/chat_ml_message.py
+-rw-r--r--   0        0        0     1062 2024-04-26 05:08:20.824958 julep-0.3.0/julep/api/types/chat_ml_message_role.py
+-rw-r--r--   0        0        0     2118 2024-04-26 05:08:52.111165 julep-0.3.0/julep/api/types/chat_response.py
+-rw-r--r--   0        0        0     1479 2024-04-26 05:08:20.812958 julep-0.3.0/julep/api/types/chat_response_finish_reason.py
+-rw-r--r--   0        0        0     6427 2024-04-26 05:08:52.159162 julep-0.3.0/julep/api/types/chat_settings.py
+-rw-r--r--   0        0        0     1787 2024-04-26 05:08:20.824958 julep-0.3.0/julep/api/types/chat_settings_preset.py
+-rw-r--r--   0        0        0     2352 2024-04-26 05:08:52.111165 julep-0.3.0/julep/api/types/chat_settings_response_format.py
+-rw-r--r--   0        0        0     1037 2024-04-26 05:08:52.115165 julep-0.3.0/julep/api/types/chat_settings_response_format_schema.py
+-rw-r--r--   0        0        0      786 2024-04-26 05:08:20.808958 julep-0.3.0/julep/api/types/chat_settings_response_format_type.py
+-rw-r--r--   0        0        0      152 2024-04-26 05:08:20.804959 julep-0.3.0/julep/api/types/chat_settings_stop.py
+-rw-r--r--   0        0        0     1358 2024-04-26 05:08:52.111165 julep-0.3.0/julep/api/types/completion_usage.py
+-rw-r--r--   0        0        0      149 2024-04-26 06:24:15.533309 julep-0.3.0/julep/api/types/create_agent_request_instructions.py
+-rw-r--r--   0        0        0     1003 2024-04-26 05:08:52.107165 julep-0.3.0/julep/api/types/create_agent_request_metadata.py
+-rw-r--r--   0        0        0     1295 2024-04-26 05:08:52.115165 julep-0.3.0/julep/api/types/create_doc.py
+-rw-r--r--   0        0        0      992 2024-04-26 05:08:52.115165 julep-0.3.0/julep/api/types/create_doc_metadata.py
+-rw-r--r--   0        0        0     1003 2024-04-26 05:08:52.107165 julep-0.3.0/julep/api/types/create_session_request_metadata.py
+-rw-r--r--   0        0        0     1329 2024-04-26 05:08:52.119165 julep-0.3.0/julep/api/types/create_tool_request.py
+-rw-r--r--   0        0        0      646 2024-04-26 05:08:52.103165 julep-0.3.0/julep/api/types/create_tool_request_type.py
+-rw-r--r--   0        0        0     1002 2024-04-26 05:08:52.115165 julep-0.3.0/julep/api/types/create_user_request_metadata.py
+-rw-r--r--   0        0        0     1399 2024-04-26 05:08:52.123164 julep-0.3.0/julep/api/types/doc.py
+-rw-r--r--   0        0        0      986 2024-04-26 05:08:52.123164 julep-0.3.0/julep/api/types/doc_metadata.py
+-rw-r--r--   0        0        0     1159 2024-04-26 05:08:52.143163 julep-0.3.0/julep/api/types/function_call_option.py
+-rw-r--r--   0        0        0     1493 2024-04-26 05:08:52.135164 julep-0.3.0/julep/api/types/function_def.py
+-rw-r--r--   0        0        0      130 2024-04-26 05:08:20.820958 julep-0.3.0/julep/api/types/function_parameters.py
+-rw-r--r--   0        0        0      485 2024-04-26 05:08:52.119165 julep-0.3.0/julep/api/types/get_agent_docs_request_order.py
+-rw-r--r--   0        0        0      570 2024-04-26 05:08:52.123164 julep-0.3.0/julep/api/types/get_agent_docs_request_sort_by.py
+-rw-r--r--   0        0        0     1023 2024-04-26 05:08:52.135164 julep-0.3.0/julep/api/types/get_agent_docs_response.py
+-rw-r--r--   0        0        0     1036 2024-04-26 05:08:52.135164 julep-0.3.0/julep/api/types/get_agent_memories_response.py
+-rw-r--r--   0        0        0     1027 2024-04-26 05:08:52.135164 julep-0.3.0/julep/api/types/get_agent_tools_response.py
+-rw-r--r--   0        0        0     1053 2024-04-26 05:08:52.135164 julep-0.3.0/julep/api/types/get_history_response.py
+-rw-r--r--   0        0        0     1046 2024-04-26 05:08:52.139163 julep-0.3.0/julep/api/types/get_suggestions_response.py
+-rw-r--r--   0        0        0      482 2024-04-26 05:08:52.127164 julep-0.3.0/julep/api/types/get_user_docs_request_order.py
+-rw-r--r--   0        0        0      567 2024-04-26 05:08:52.127164 julep-0.3.0/julep/api/types/get_user_docs_request_sort_by.py
+-rw-r--r--   0        0        0     1022 2024-04-26 05:08:52.143163 julep-0.3.0/julep/api/types/get_user_docs_response.py
+-rw-r--r--   0        0        0     1615 2024-04-26 05:08:52.163162 julep-0.3.0/julep/api/types/input_chat_ml_message.py
+-rw-r--r--   0        0        0     1234 2024-04-26 05:08:20.828957 julep-0.3.0/julep/api/types/input_chat_ml_message_role.py
+-rw-r--r--   0        0        0     1819 2024-04-26 05:08:52.163162 julep-0.3.0/julep/api/types/job_status.py
+-rw-r--r--   0        0        0     1361 2024-04-26 05:08:20.812958 julep-0.3.0/julep/api/types/job_status_state.py
+-rw-r--r--   0        0        0      479 2024-04-26 05:08:52.135164 julep-0.3.0/julep/api/types/list_agents_request_order.py
+-rw-r--r--   0        0        0      564 2024-04-26 05:08:52.135164 julep-0.3.0/julep/api/types/list_agents_request_sort_by.py
+-rw-r--r--   0        0        0     1010 2024-04-26 05:08:52.155162 julep-0.3.0/julep/api/types/list_agents_response.py
+-rw-r--r--   0        0        0      485 2024-04-26 05:08:52.143163 julep-0.3.0/julep/api/types/list_sessions_request_order.py
+-rw-r--r--   0        0        0      570 2024-04-26 05:08:52.143163 julep-0.3.0/julep/api/types/list_sessions_request_sort_by.py
+-rw-r--r--   0        0        0     1018 2024-04-26 05:08:52.155162 julep-0.3.0/julep/api/types/list_sessions_response.py
+-rw-r--r--   0        0        0      476 2024-04-26 05:08:52.155162 julep-0.3.0/julep/api/types/list_users_request_order.py
+-rw-r--r--   0        0        0      561 2024-04-26 05:08:52.147163 julep-0.3.0/julep/api/types/list_users_request_sort_by.py
+-rw-r--r--   0        0        0     1006 2024-04-26 05:08:52.159162 julep-0.3.0/julep/api/types/list_users_response.py
+-rw-r--r--   0        0        0     1907 2024-04-26 05:08:52.179161 julep-0.3.0/julep/api/types/memory.py
+-rw-r--r--   0        0        0     1365 2024-04-26 05:08:52.167162 julep-0.3.0/julep/api/types/memory_access_options.py
+-rw-r--r--   0        0        0      954 2024-04-26 05:08:52.159162 julep-0.3.0/julep/api/types/memory_entities_item.py
+-rw-r--r--   0        0        0     1240 2024-04-26 05:08:52.163162 julep-0.3.0/julep/api/types/named_tool_choice.py
+-rw-r--r--   0        0        0     1040 2024-04-26 05:08:52.167162 julep-0.3.0/julep/api/types/named_tool_choice_function.py
+-rw-r--r--   0        0        0     1534 2024-04-26 05:08:52.171162 julep-0.3.0/julep/api/types/partial_function_def.py
+-rw-r--r--   0        0        0      148 2024-04-26 06:24:15.533309 julep-0.3.0/julep/api/types/patch_agent_request_instructions.py
+-rw-r--r--   0        0        0     1000 2024-04-26 05:08:52.167162 julep-0.3.0/julep/api/types/patch_agent_request_metadata.py
+-rw-r--r--   0        0        0     1002 2024-04-26 05:08:52.167162 julep-0.3.0/julep/api/types/patch_session_request_metadata.py
+-rw-r--r--   0        0        0      999 2024-04-26 05:08:52.167162 julep-0.3.0/julep/api/types/patch_user_request_metadata.py
+-rw-r--r--   0        0        0     1143 2024-04-26 05:08:52.183161 julep-0.3.0/julep/api/types/resource_created_response.py
+-rw-r--r--   0        0        0     1143 2024-04-26 05:08:52.175161 julep-0.3.0/julep/api/types/resource_deleted_response.py
+-rw-r--r--   0        0        0     1143 2024-04-26 05:08:52.183161 julep-0.3.0/julep/api/types/resource_updated_response.py
+-rw-r--r--   0        0        0     2090 2024-04-26 05:08:52.203159 julep-0.3.0/julep/api/types/session.py
+-rw-r--r--   0        0        0      990 2024-04-26 05:08:52.179161 julep-0.3.0/julep/api/types/session_metadata.py
+-rw-r--r--   0        0        0     1502 2024-04-26 05:08:52.191160 julep-0.3.0/julep/api/types/suggestion.py
+-rw-r--r--   0        0        0      546 2024-04-26 05:08:52.171162 julep-0.3.0/julep/api/types/suggestion_target.py
+-rw-r--r--   0        0        0     1327 2024-04-26 05:08:52.187160 julep-0.3.0/julep/api/types/tool.py
+-rw-r--r--   0        0        0       88 2024-04-26 05:08:20.812958 julep-0.3.0/julep/api/types/tool_choice_option.py
+-rw-r--r--   0        0        0      607 2024-04-26 05:08:52.175161 julep-0.3.0/julep/api/types/tool_type.py
+-rw-r--r--   0        0        0      149 2024-04-26 06:24:15.533309 julep-0.3.0/julep/api/types/update_agent_request_instructions.py
+-rw-r--r--   0        0        0     1001 2024-04-26 05:08:52.187160 julep-0.3.0/julep/api/types/update_agent_request_metadata.py
+-rw-r--r--   0        0        0     1003 2024-04-26 05:08:52.187160 julep-0.3.0/julep/api/types/update_session_request_metadata.py
+-rw-r--r--   0        0        0     1000 2024-04-26 05:08:52.187160 julep-0.3.0/julep/api/types/update_user_request_metadata.py
+-rw-r--r--   0        0        0     1559 2024-04-26 05:08:52.203159 julep-0.3.0/julep/api/types/user.py
+-rw-r--r--   0        0        0      989 2024-04-26 05:08:52.191160 julep-0.3.0/julep/api/types/user_metadata.py
+-rw-r--r--   0        0        0    11638 2024-04-16 05:25:00.535880 julep-0.3.0/julep/client.py
+-rw-r--r--   0        0        0      527 2024-04-18 03:57:55.434983 julep-0.3.0/julep/env.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:31:45.040791 julep-0.3.0/julep/managers/__init__.py
+-rw-r--r--   0        0        0    32129 2024-04-18 06:05:18.506024 julep-0.3.0/julep/managers/agent.py
+-rw-r--r--   0        0        0     1249 2024-04-18 06:05:18.506024 julep-0.3.0/julep/managers/base.py
+-rw-r--r--   0        0        0    21222 2024-04-26 06:24:15.533309 julep-0.3.0/julep/managers/doc.py
+-rw-r--r--   0        0        0     7707 2024-04-18 05:08:06.874967 julep-0.3.0/julep/managers/memory.py
+-rw-r--r--   0        0        0    47059 2024-04-18 06:05:18.510024 julep-0.3.0/julep/managers/session.py
+-rw-r--r--   0        0        0    18899 2024-04-26 06:24:15.533309 julep-0.3.0/julep/managers/tool.py
+-rw-r--r--   0        0        0     1758 2024-04-18 06:05:18.510024 julep-0.3.0/julep/managers/types.py
+-rw-r--r--   0        0        0    19731 2024-04-16 05:25:00.535880 julep-0.3.0/julep/managers/user.py
+-rw-r--r--   0        0        0     1628 2024-04-18 06:05:18.510024 julep-0.3.0/julep/managers/utils.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:31:45.040791 julep-0.3.0/julep/utils/__init__.py
+-rw-r--r--   0        0        0    14233 2024-04-18 06:05:18.510024 julep-0.3.0/julep/utils/openai_patch.py
+-rw-r--r--   0        0        0     1668 2024-04-26 08:17:25.642907 julep-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 julep-0.3.0/PKG-INFO
```

### Comparing `julep-0.2.9/julep/api/__init__.py` & `julep-0.3.0/julep/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     Agent,
     AgentDefaultSettings,
     AgentDefaultSettingsPreset,
+    AgentInstructions,
     AgentMetadata,
     ChatInputData,
     ChatInputDataToolChoice,
     ChatMlMessage,
     ChatMlMessageRole,
     ChatResponse,
     ChatResponseFinishReason,
     ChatSettings,
     ChatSettingsPreset,
     ChatSettingsResponseFormat,
     ChatSettingsResponseFormatSchema,
     ChatSettingsResponseFormatType,
     ChatSettingsStop,
     CompletionUsage,
+    CreateAgentRequestInstructions,
     CreateAgentRequestMetadata,
     CreateDoc,
     CreateDocMetadata,
     CreateSessionRequestMetadata,
     CreateToolRequest,
     CreateToolRequestType,
     CreateUserRequestMetadata,
@@ -38,71 +40,74 @@
     GetHistoryResponse,
     GetSuggestionsResponse,
     GetUserDocsRequestOrder,
     GetUserDocsRequestSortBy,
     GetUserDocsResponse,
     InputChatMlMessage,
     InputChatMlMessageRole,
-    Instruction,
     JobStatus,
     JobStatusState,
     ListAgentsRequestOrder,
     ListAgentsRequestSortBy,
     ListAgentsResponse,
     ListSessionsRequestOrder,
     ListSessionsRequestSortBy,
     ListSessionsResponse,
     ListUsersRequestOrder,
     ListUsersRequestSortBy,
     ListUsersResponse,
     Memory,
     MemoryAccessOptions,
-    MemoryEmotionsItem,
-    MemoryType,
+    MemoryEntitiesItem,
     NamedToolChoice,
     NamedToolChoiceFunction,
+    PartialFunctionDef,
+    PatchAgentRequestInstructions,
     PatchAgentRequestMetadata,
     PatchSessionRequestMetadata,
     PatchUserRequestMetadata,
     ResourceCreatedResponse,
     ResourceDeletedResponse,
     ResourceUpdatedResponse,
     Session,
     SessionMetadata,
     Suggestion,
     SuggestionTarget,
     Tool,
     ToolChoiceOption,
     ToolType,
+    UpdateAgentRequestInstructions,
     UpdateAgentRequestMetadata,
     UpdateSessionRequestMetadata,
     UpdateUserRequestMetadata,
     User,
     UserMetadata,
 )
 from .environment import JulepApiEnvironment
 
 __all__ = [
     "Agent",
     "AgentDefaultSettings",
     "AgentDefaultSettingsPreset",
+    "AgentInstructions",
     "AgentMetadata",
     "ChatInputData",
     "ChatInputDataToolChoice",
     "ChatMlMessage",
     "ChatMlMessageRole",
     "ChatResponse",
     "ChatResponseFinishReason",
     "ChatSettings",
     "ChatSettingsPreset",
     "ChatSettingsResponseFormat",
     "ChatSettingsResponseFormatSchema",
     "ChatSettingsResponseFormatType",
     "ChatSettingsStop",
     "CompletionUsage",
+    "CreateAgentRequestInstructions",
     "CreateAgentRequestMetadata",
     "CreateDoc",
     "CreateDocMetadata",
     "CreateSessionRequestMetadata",
     "CreateToolRequest",
     "CreateToolRequestType",
     "CreateUserRequestMetadata",
@@ -119,45 +124,46 @@
     "GetHistoryResponse",
     "GetSuggestionsResponse",
     "GetUserDocsRequestOrder",
     "GetUserDocsRequestSortBy",
     "GetUserDocsResponse",
     "InputChatMlMessage",
     "InputChatMlMessageRole",
-    "Instruction",
     "JobStatus",
     "JobStatusState",
     "JulepApiEnvironment",
     "ListAgentsRequestOrder",
     "ListAgentsRequestSortBy",
     "ListAgentsResponse",
     "ListSessionsRequestOrder",
     "ListSessionsRequestSortBy",
     "ListSessionsResponse",
     "ListUsersRequestOrder",
     "ListUsersRequestSortBy",
     "ListUsersResponse",
     "Memory",
     "MemoryAccessOptions",
-    "MemoryEmotionsItem",
-    "MemoryType",
+    "MemoryEntitiesItem",
     "NamedToolChoice",
     "NamedToolChoiceFunction",
+    "PartialFunctionDef",
+    "PatchAgentRequestInstructions",
     "PatchAgentRequestMetadata",
     "PatchSessionRequestMetadata",
     "PatchUserRequestMetadata",
     "ResourceCreatedResponse",
     "ResourceDeletedResponse",
     "ResourceUpdatedResponse",
     "Session",
     "SessionMetadata",
     "Suggestion",
     "SuggestionTarget",
     "Tool",
     "ToolChoiceOption",
     "ToolType",
+    "UpdateAgentRequestInstructions",
     "UpdateAgentRequestMetadata",
     "UpdateSessionRequestMetadata",
     "UpdateUserRequestMetadata",
     "User",
     "UserMetadata",
 ]
```

### Comparing `julep-0.2.9/julep/api/client.py` & `julep-0.3.0/julep/api/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# type: ignore
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
@@ -15,14 +14,15 @@
 from .types.agent import Agent
 from .types.agent_default_settings import AgentDefaultSettings
 from .types.chat_input_data_tool_choice import ChatInputDataToolChoice
 from .types.chat_response import ChatResponse
 from .types.chat_settings_preset import ChatSettingsPreset
 from .types.chat_settings_response_format import ChatSettingsResponseFormat
 from .types.chat_settings_stop import ChatSettingsStop
+from .types.create_agent_request_instructions import CreateAgentRequestInstructions
 from .types.create_agent_request_metadata import CreateAgentRequestMetadata
 from .types.create_doc import CreateDoc
 from .types.create_session_request_metadata import CreateSessionRequestMetadata
 from .types.create_tool_request import CreateToolRequest
 from .types.create_user_request_metadata import CreateUserRequestMetadata
 from .types.function_def import FunctionDef
 from .types.get_agent_docs_request_order import GetAgentDocsRequestOrder
@@ -32,32 +32,34 @@
 from .types.get_agent_tools_response import GetAgentToolsResponse
 from .types.get_history_response import GetHistoryResponse
 from .types.get_suggestions_response import GetSuggestionsResponse
 from .types.get_user_docs_request_order import GetUserDocsRequestOrder
 from .types.get_user_docs_request_sort_by import GetUserDocsRequestSortBy
 from .types.get_user_docs_response import GetUserDocsResponse
 from .types.input_chat_ml_message import InputChatMlMessage
-from .types.instruction import Instruction
 from .types.job_status import JobStatus
 from .types.list_agents_request_order import ListAgentsRequestOrder
 from .types.list_agents_request_sort_by import ListAgentsRequestSortBy
 from .types.list_agents_response import ListAgentsResponse
 from .types.list_sessions_request_order import ListSessionsRequestOrder
 from .types.list_sessions_request_sort_by import ListSessionsRequestSortBy
 from .types.list_sessions_response import ListSessionsResponse
 from .types.list_users_request_order import ListUsersRequestOrder
 from .types.list_users_request_sort_by import ListUsersRequestSortBy
 from .types.list_users_response import ListUsersResponse
+from .types.partial_function_def import PartialFunctionDef
+from .types.patch_agent_request_instructions import PatchAgentRequestInstructions
 from .types.patch_agent_request_metadata import PatchAgentRequestMetadata
 from .types.patch_session_request_metadata import PatchSessionRequestMetadata
 from .types.patch_user_request_metadata import PatchUserRequestMetadata
 from .types.resource_created_response import ResourceCreatedResponse
 from .types.resource_updated_response import ResourceUpdatedResponse
 from .types.session import Session
 from .types.tool import Tool
+from .types.update_agent_request_instructions import UpdateAgentRequestInstructions
 from .types.update_agent_request_metadata import UpdateAgentRequestMetadata
 from .types.update_session_request_metadata import UpdateSessionRequestMetadata
 from .types.update_user_request_metadata import UpdateUserRequestMetadata
 from .types.user import User
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
@@ -77,17 +79,17 @@
         api_key: str,
         timeout: typing.Optional[float] = 300,
         httpx_client: typing.Optional[httpx.Client] = None,
     ):
         self._client_wrapper = SyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
             api_key=api_key,
-            httpx_client=httpx.Client(timeout=timeout)
-            if httpx_client is None
-            else httpx_client,
+            httpx_client=(
+                httpx.Client(timeout=timeout) if httpx_client is None else httpx_client
+            ),
         )
 
     def list_sessions(
         self,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
@@ -138,49 +140,52 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_session(
         self,
         *,
-        user_id: str,
+        user_id: typing.Optional[str] = OMIT,
         agent_id: str,
         situation: typing.Optional[str] = OMIT,
         metadata: typing.Optional[CreateSessionRequestMetadata] = OMIT,
+        render_templates: typing.Optional[bool] = OMIT,
     ) -> ResourceCreatedResponse:
         """
         Create a session between an agent and a user
 
         Parameters:
-            - user_id: str. User ID of user to associate with this session
+            - user_id: typing.Optional[str]. (Optional) User ID of user to associate with this session
 
             - agent_id: str. Agent ID of agent to associate with this session
 
             - situation: typing.Optional[str]. A specific situation that sets the background for this session
 
             - metadata: typing.Optional[CreateSessionRequestMetadata]. Optional metadata
+
+            - render_templates: typing.Optional[bool]. Render system and assistant message content as jinja templates
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.create_session(
-            user_id="user_id",
             agent_id="agent_id",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {
-            "user_id": user_id,
-            "agent_id": agent_id,
-        }
+        _request: typing.Dict[str, typing.Any] = {"agent_id": agent_id}
+        if user_id is not OMIT:
+            _request["user_id"] = user_id
         if situation is not OMIT:
             _request["situation"] = situation
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if render_templates is not OMIT:
+            _request["render_templates"] = render_templates
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
@@ -259,15 +264,15 @@
         Parameters:
             - name: typing.Optional[str]. Name of the user
 
             - about: typing.Optional[str]. About the user
 
             - docs: typing.Optional[typing.List[CreateDoc]]. List of docs about user
 
-            - metadata: typing.Optional[CreateUserRequestMetadata]. Optional metadata
+            - metadata: typing.Optional[CreateUserRequestMetadata]. (Optional) metadata
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.create_user()
@@ -350,65 +355,65 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_agent(
         self,
         *,
         name: str,
         about: typing.Optional[str] = OMIT,
-        instructions: typing.Optional[typing.List[Instruction]] = OMIT,
         tools: typing.Optional[typing.List[CreateToolRequest]] = OMIT,
         default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
         model: typing.Optional[str] = OMIT,
         docs: typing.Optional[typing.List[CreateDoc]] = OMIT,
         metadata: typing.Optional[CreateAgentRequestMetadata] = OMIT,
+        instructions: typing.Optional[CreateAgentRequestInstructions] = OMIT,
     ) -> ResourceCreatedResponse:
         """
         Create a new agent
 
         Parameters:
             - name: str. Name of the agent
 
             - about: typing.Optional[str]. About the agent
 
-            - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
-
             - tools: typing.Optional[typing.List[CreateToolRequest]]. A list of tools the model may call. Currently, only `function`s are supported as a tool. Use this to provide a list of functions the model may generate JSON inputs for.
 
             - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
 
             - model: typing.Optional[str]. Name of the model that the agent is supposed to use
 
             - docs: typing.Optional[typing.List[CreateDoc]]. List of docs about agent
 
-            - metadata: typing.Optional[CreateAgentRequestMetadata]. Optional metadata
+            - metadata: typing.Optional[CreateAgentRequestMetadata]. (Optional) metadata
+
+            - instructions: typing.Optional[CreateAgentRequestInstructions]. Instructions for the agent
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.create_agent(
             name="name",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if about is not OMIT:
             _request["about"] = about
-        if instructions is not OMIT:
-            _request["instructions"] = instructions
         if tools is not OMIT:
             _request["tools"] = tools
         if default_settings is not OMIT:
             _request["default_settings"] = default_settings
         if model is not OMIT:
             _request["model"] = model
         if docs is not OMIT:
             _request["docs"] = docs
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if instructions is not OMIT:
+            _request["instructions"] = instructions
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
@@ -452,39 +457,38 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_session(
         self,
         session_id: str,
         *,
-        situation: typing.Optional[str] = OMIT,
+        situation: str,
         metadata: typing.Optional[UpdateSessionRequestMetadata] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - session_id: str.
 
-            - situation: typing.Optional[str]. Updated situation for this session
+            - situation: str. Updated situation for this session
 
             - metadata: typing.Optional[UpdateSessionRequestMetadata]. Optional metadata
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.update_session(
             session_id="session_id",
+            situation="situation",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if situation is not OMIT:
-            _request["situation"] = situation
+        _request: typing.Dict[str, typing.Any] = {"situation": situation}
         if metadata is not OMIT:
             _request["metadata"] = metadata
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"sessions/{session_id}"
             ),
@@ -664,14 +668,47 @@
             return pydantic.parse_obj_as(GetHistoryResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def delete_session_history(self, session_id: str) -> None:
+        """
+
+
+        Parameters:
+            - session_id: str.
+        ---
+        from julep.client import JulepApi
+
+        client = JulepApi(
+            api_key="YOUR_API_KEY",
+        )
+        client.delete_session_history(
+            session_id="session_id",
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "DELETE",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"sessions/{session_id}/history",
+            ),
+            headers=self._client_wrapper.get_headers(),
+            timeout=300,
+        )
+        if 200 <= _response.status_code < 300:
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def chat(
         self,
         session_id: str,
         *,
         messages: typing.List[InputChatMlMessage],
         tools: typing.Optional[typing.List[Tool]] = OMIT,
         tool_choice: typing.Optional[ChatInputDataToolChoice] = OMIT,
@@ -686,14 +723,15 @@
         stop: typing.Optional[ChatSettingsStop] = OMIT,
         stream: typing.Optional[bool] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         top_p: typing.Optional[float] = OMIT,
         min_p: typing.Optional[float] = OMIT,
         preset: typing.Optional[ChatSettingsPreset] = OMIT,
         recall: typing.Optional[bool] = OMIT,
+        record: typing.Optional[bool] = OMIT,
         remember: typing.Optional[bool] = OMIT,
     ) -> ChatResponse:
         """
 
 
         Parameters:
             - session_id: str.
@@ -736,15 +774,17 @@
 
             - min_p: typing.Optional[float]. Minimum probability compared to leading token to be considered
 
             - preset: typing.Optional[ChatSettingsPreset]. Generation preset name (problem_solving|conversational|fun|prose|creative|business|deterministic|code|multilingual)
 
             - recall: typing.Optional[bool]. Whether previous memories should be recalled or not
 
-            - remember: typing.Optional[bool]. Whether this interaction should be recorded in memory or not
+            - record: typing.Optional[bool]. Whether this interaction should be recorded in history or not
+
+            - remember: typing.Optional[bool]. Whether this interaction should form memories or not
         ---
         from julep import InputChatMlMessage, InputChatMlMessageRole
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
@@ -787,17 +827,19 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if min_p is not OMIT:
             _request["min_p"] = min_p
         if preset is not OMIT:
-            _request["preset"] = preset.value
+            _request["preset"] = preset.value  # type: ignore
         if recall is not OMIT:
             _request["recall"] = recall
+        if record is not OMIT:
+            _request["record"] = record
         if remember is not OMIT:
             _request["remember"] = remember
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"sessions/{session_id}/chat"
             ),
@@ -816,29 +858,26 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_agent_memories(
         self,
         agent_id: str,
         *,
         query: str,
-        types: typing.Optional[typing.Union[str, typing.List[str]]] = None,
         user_id: typing.Optional[str] = None,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> GetAgentMemoriesResponse:
         """
         Sorted (created_at descending)
 
         Parameters:
             - agent_id: str.
 
             - query: str.
 
-            - types: typing.Optional[typing.Union[str, typing.List[str]]]. episode, belief, entity
-
             - user_id: typing.Optional[str].
 
             - limit: typing.Optional[int].
 
             - offset: typing.Optional[int].
         ---
         from julep.client import JulepApi
@@ -853,21 +892,15 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}/memories"
             ),
             params=remove_none_from_dict(
-                {
-                    "query": query,
-                    "types": types,
-                    "user_id": user_id,
-                    "limit": limit,
-                    "offset": offset,
-                }
+                {"query": query, "user_id": user_id, "limit": limit, "offset": offset}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetAgentMemoriesResponse, _response.json())  # type: ignore
         try:
@@ -908,44 +941,42 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_user(
         self,
         user_id: str,
         *,
-        about: typing.Optional[str] = OMIT,
-        name: typing.Optional[str] = OMIT,
+        about: str,
+        name: str,
         metadata: typing.Optional[UpdateUserRequestMetadata] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - user_id: str.
 
-            - about: typing.Optional[str]. About the user
+            - about: str. About the user
 
-            - name: typing.Optional[str]. Name of the user
+            - name: str. Name of the user
 
             - metadata: typing.Optional[UpdateUserRequestMetadata]. Optional metadata
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.update_user(
             user_id="user_id",
+            about="about",
+            name="name",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if about is not OMIT:
-            _request["about"] = about
-        if name is not OMIT:
-            _request["name"] = name
+        _request: typing.Dict[str, typing.Any] = {"about": about, "name": name}
         if metadata is not OMIT:
             _request["metadata"] = metadata
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}"
             ),
@@ -1078,61 +1109,59 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_agent(
         self,
         agent_id: str,
         *,
-        about: typing.Optional[str] = OMIT,
-        instructions: typing.Optional[typing.List[Instruction]] = OMIT,
-        name: typing.Optional[str] = OMIT,
+        about: str,
+        name: str,
         model: typing.Optional[str] = OMIT,
         default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
         metadata: typing.Optional[UpdateAgentRequestMetadata] = OMIT,
+        instructions: typing.Optional[UpdateAgentRequestInstructions] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - agent_id: str.
 
-            - about: typing.Optional[str]. About the agent
-
-            - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
+            - about: str. About the agent
 
-            - name: typing.Optional[str]. Name of the agent
+            - name: str. Name of the agent
 
             - model: typing.Optional[str]. Name of the model that the agent is supposed to use
 
             - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
 
             - metadata: typing.Optional[UpdateAgentRequestMetadata]. Optional metadata
+
+            - instructions: typing.Optional[UpdateAgentRequestInstructions]. Instructions for the agent
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.update_agent(
             agent_id="agent_id",
+            about="about",
+            name="name",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if about is not OMIT:
-            _request["about"] = about
-        if instructions is not OMIT:
-            _request["instructions"] = instructions
-        if name is not OMIT:
-            _request["name"] = name
+        _request: typing.Dict[str, typing.Any] = {"about": about, "name": name}
         if model is not OMIT:
             _request["model"] = model
         if default_settings is not OMIT:
             _request["default_settings"] = default_settings
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if instructions is not OMIT:
+            _request["instructions"] = instructions
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"
             ),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -1179,60 +1208,60 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def patch_agent(
         self,
         agent_id: str,
         *,
         about: typing.Optional[str] = OMIT,
-        instructions: typing.Optional[typing.List[Instruction]] = OMIT,
         name: typing.Optional[str] = OMIT,
         model: typing.Optional[str] = OMIT,
         default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
         metadata: typing.Optional[PatchAgentRequestMetadata] = OMIT,
+        instructions: typing.Optional[PatchAgentRequestInstructions] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - agent_id: str.
 
             - about: typing.Optional[str]. About the agent
 
-            - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
-
             - name: typing.Optional[str]. Name of the agent
 
             - model: typing.Optional[str]. Name of the model that the agent is supposed to use
 
             - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
 
             - metadata: typing.Optional[PatchAgentRequestMetadata]. Optional metadata
+
+            - instructions: typing.Optional[PatchAgentRequestInstructions]. Instructions for the agent
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.patch_agent(
             agent_id="agent_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if about is not OMIT:
             _request["about"] = about
-        if instructions is not OMIT:
-            _request["instructions"] = instructions
         if name is not OMIT:
             _request["name"] = name
         if model is not OMIT:
             _request["model"] = model
         if default_settings is not OMIT:
             _request["default_settings"] = default_settings
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if instructions is not OMIT:
+            _request["instructions"] = instructions
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"
             ),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -1725,39 +1754,36 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def patch_agent_tool(
-        self, agent_id: str, tool_id: str, *, function: FunctionDef
+        self, agent_id: str, tool_id: str, *, function: PartialFunctionDef
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - agent_id: str.
 
             - tool_id: str.
 
-            - function: FunctionDef. Function definition and parameters
+            - function: PartialFunctionDef. Function definition and parameters
         ---
-        from julep import FunctionDef
+        from julep import PartialFunctionDef
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.patch_agent_tool(
             agent_id="agent_id",
             tool_id="tool_id",
-            function=FunctionDef(
-                name="name",
-                parameters={},
-            ),
+            function=PartialFunctionDef(),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"agents/{agent_id}/tools/{tool_id}",
@@ -1816,17 +1842,19 @@
         api_key: str,
         timeout: typing.Optional[float] = 300,
         httpx_client: typing.Optional[httpx.AsyncClient] = None,
     ):
         self._client_wrapper = AsyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
             api_key=api_key,
-            httpx_client=httpx.AsyncClient(timeout=timeout)
-            if httpx_client is None
-            else httpx_client,
+            httpx_client=(
+                httpx.AsyncClient(timeout=timeout)
+                if httpx_client is None
+                else httpx_client
+            ),
         )
 
     async def list_sessions(
         self,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
@@ -1877,49 +1905,52 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_session(
         self,
         *,
-        user_id: str,
+        user_id: typing.Optional[str] = OMIT,
         agent_id: str,
         situation: typing.Optional[str] = OMIT,
         metadata: typing.Optional[CreateSessionRequestMetadata] = OMIT,
+        render_templates: typing.Optional[bool] = OMIT,
     ) -> ResourceCreatedResponse:
         """
         Create a session between an agent and a user
 
         Parameters:
-            - user_id: str. User ID of user to associate with this session
+            - user_id: typing.Optional[str]. (Optional) User ID of user to associate with this session
 
             - agent_id: str. Agent ID of agent to associate with this session
 
             - situation: typing.Optional[str]. A specific situation that sets the background for this session
 
             - metadata: typing.Optional[CreateSessionRequestMetadata]. Optional metadata
+
+            - render_templates: typing.Optional[bool]. Render system and assistant message content as jinja templates
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.create_session(
-            user_id="user_id",
             agent_id="agent_id",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {
-            "user_id": user_id,
-            "agent_id": agent_id,
-        }
+        _request: typing.Dict[str, typing.Any] = {"agent_id": agent_id}
+        if user_id is not OMIT:
+            _request["user_id"] = user_id
         if situation is not OMIT:
             _request["situation"] = situation
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if render_templates is not OMIT:
+            _request["render_templates"] = render_templates
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
@@ -1998,15 +2029,15 @@
         Parameters:
             - name: typing.Optional[str]. Name of the user
 
             - about: typing.Optional[str]. About the user
 
             - docs: typing.Optional[typing.List[CreateDoc]]. List of docs about user
 
-            - metadata: typing.Optional[CreateUserRequestMetadata]. Optional metadata
+            - metadata: typing.Optional[CreateUserRequestMetadata]. (Optional) metadata
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.create_user()
@@ -2089,65 +2120,65 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_agent(
         self,
         *,
         name: str,
         about: typing.Optional[str] = OMIT,
-        instructions: typing.Optional[typing.List[Instruction]] = OMIT,
         tools: typing.Optional[typing.List[CreateToolRequest]] = OMIT,
         default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
         model: typing.Optional[str] = OMIT,
         docs: typing.Optional[typing.List[CreateDoc]] = OMIT,
         metadata: typing.Optional[CreateAgentRequestMetadata] = OMIT,
+        instructions: typing.Optional[CreateAgentRequestInstructions] = OMIT,
     ) -> ResourceCreatedResponse:
         """
         Create a new agent
 
         Parameters:
             - name: str. Name of the agent
 
             - about: typing.Optional[str]. About the agent
 
-            - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
-
             - tools: typing.Optional[typing.List[CreateToolRequest]]. A list of tools the model may call. Currently, only `function`s are supported as a tool. Use this to provide a list of functions the model may generate JSON inputs for.
 
             - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
 
             - model: typing.Optional[str]. Name of the model that the agent is supposed to use
 
             - docs: typing.Optional[typing.List[CreateDoc]]. List of docs about agent
 
-            - metadata: typing.Optional[CreateAgentRequestMetadata]. Optional metadata
+            - metadata: typing.Optional[CreateAgentRequestMetadata]. (Optional) metadata
+
+            - instructions: typing.Optional[CreateAgentRequestInstructions]. Instructions for the agent
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.create_agent(
             name="name",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if about is not OMIT:
             _request["about"] = about
-        if instructions is not OMIT:
-            _request["instructions"] = instructions
         if tools is not OMIT:
             _request["tools"] = tools
         if default_settings is not OMIT:
             _request["default_settings"] = default_settings
         if model is not OMIT:
             _request["model"] = model
         if docs is not OMIT:
             _request["docs"] = docs
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if instructions is not OMIT:
+            _request["instructions"] = instructions
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
@@ -2191,39 +2222,38 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_session(
         self,
         session_id: str,
         *,
-        situation: typing.Optional[str] = OMIT,
+        situation: str,
         metadata: typing.Optional[UpdateSessionRequestMetadata] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - session_id: str.
 
-            - situation: typing.Optional[str]. Updated situation for this session
+            - situation: str. Updated situation for this session
 
             - metadata: typing.Optional[UpdateSessionRequestMetadata]. Optional metadata
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.update_session(
             session_id="session_id",
+            situation="situation",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if situation is not OMIT:
-            _request["situation"] = situation
+        _request: typing.Dict[str, typing.Any] = {"situation": situation}
         if metadata is not OMIT:
             _request["metadata"] = metadata
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"sessions/{session_id}"
             ),
@@ -2403,14 +2433,47 @@
             return pydantic.parse_obj_as(GetHistoryResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    async def delete_session_history(self, session_id: str) -> None:
+        """
+
+
+        Parameters:
+            - session_id: str.
+        ---
+        from julep.client import AsyncJulepApi
+
+        client = AsyncJulepApi(
+            api_key="YOUR_API_KEY",
+        )
+        await client.delete_session_history(
+            session_id="session_id",
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "DELETE",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"sessions/{session_id}/history",
+            ),
+            headers=self._client_wrapper.get_headers(),
+            timeout=300,
+        )
+        if 200 <= _response.status_code < 300:
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     async def chat(
         self,
         session_id: str,
         *,
         messages: typing.List[InputChatMlMessage],
         tools: typing.Optional[typing.List[Tool]] = OMIT,
         tool_choice: typing.Optional[ChatInputDataToolChoice] = OMIT,
@@ -2425,14 +2488,15 @@
         stop: typing.Optional[ChatSettingsStop] = OMIT,
         stream: typing.Optional[bool] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         top_p: typing.Optional[float] = OMIT,
         min_p: typing.Optional[float] = OMIT,
         preset: typing.Optional[ChatSettingsPreset] = OMIT,
         recall: typing.Optional[bool] = OMIT,
+        record: typing.Optional[bool] = OMIT,
         remember: typing.Optional[bool] = OMIT,
     ) -> ChatResponse:
         """
 
 
         Parameters:
             - session_id: str.
@@ -2475,15 +2539,17 @@
 
             - min_p: typing.Optional[float]. Minimum probability compared to leading token to be considered
 
             - preset: typing.Optional[ChatSettingsPreset]. Generation preset name (problem_solving|conversational|fun|prose|creative|business|deterministic|code|multilingual)
 
             - recall: typing.Optional[bool]. Whether previous memories should be recalled or not
 
-            - remember: typing.Optional[bool]. Whether this interaction should be recorded in memory or not
+            - record: typing.Optional[bool]. Whether this interaction should be recorded in history or not
+
+            - remember: typing.Optional[bool]. Whether this interaction should form memories or not
         ---
         from julep import InputChatMlMessage, InputChatMlMessageRole
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
@@ -2526,17 +2592,19 @@
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if top_p is not OMIT:
             _request["top_p"] = top_p
         if min_p is not OMIT:
             _request["min_p"] = min_p
         if preset is not OMIT:
-            _request["preset"] = preset.value
+            _request["preset"] = preset.value  # type: ignore
         if recall is not OMIT:
             _request["recall"] = recall
+        if record is not OMIT:
+            _request["record"] = record
         if remember is not OMIT:
             _request["remember"] = remember
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"sessions/{session_id}/chat"
             ),
@@ -2555,29 +2623,26 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_agent_memories(
         self,
         agent_id: str,
         *,
         query: str,
-        types: typing.Optional[typing.Union[str, typing.List[str]]] = None,
         user_id: typing.Optional[str] = None,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> GetAgentMemoriesResponse:
         """
         Sorted (created_at descending)
 
         Parameters:
             - agent_id: str.
 
             - query: str.
 
-            - types: typing.Optional[typing.Union[str, typing.List[str]]]. episode, belief, entity
-
             - user_id: typing.Optional[str].
 
             - limit: typing.Optional[int].
 
             - offset: typing.Optional[int].
         ---
         from julep.client import AsyncJulepApi
@@ -2592,21 +2657,15 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}/memories"
             ),
             params=remove_none_from_dict(
-                {
-                    "query": query,
-                    "types": types,
-                    "user_id": user_id,
-                    "limit": limit,
-                    "offset": offset,
-                }
+                {"query": query, "user_id": user_id, "limit": limit, "offset": offset}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetAgentMemoriesResponse, _response.json())  # type: ignore
         try:
@@ -2647,44 +2706,42 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_user(
         self,
         user_id: str,
         *,
-        about: typing.Optional[str] = OMIT,
-        name: typing.Optional[str] = OMIT,
+        about: str,
+        name: str,
         metadata: typing.Optional[UpdateUserRequestMetadata] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - user_id: str.
 
-            - about: typing.Optional[str]. About the user
+            - about: str. About the user
 
-            - name: typing.Optional[str]. Name of the user
+            - name: str. Name of the user
 
             - metadata: typing.Optional[UpdateUserRequestMetadata]. Optional metadata
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.update_user(
             user_id="user_id",
+            about="about",
+            name="name",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if about is not OMIT:
-            _request["about"] = about
-        if name is not OMIT:
-            _request["name"] = name
+        _request: typing.Dict[str, typing.Any] = {"about": about, "name": name}
         if metadata is not OMIT:
             _request["metadata"] = metadata
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}"
             ),
@@ -2817,61 +2874,59 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_agent(
         self,
         agent_id: str,
         *,
-        about: typing.Optional[str] = OMIT,
-        instructions: typing.Optional[typing.List[Instruction]] = OMIT,
-        name: typing.Optional[str] = OMIT,
+        about: str,
+        name: str,
         model: typing.Optional[str] = OMIT,
         default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
         metadata: typing.Optional[UpdateAgentRequestMetadata] = OMIT,
+        instructions: typing.Optional[UpdateAgentRequestInstructions] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - agent_id: str.
 
-            - about: typing.Optional[str]. About the agent
-
-            - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
+            - about: str. About the agent
 
-            - name: typing.Optional[str]. Name of the agent
+            - name: str. Name of the agent
 
             - model: typing.Optional[str]. Name of the model that the agent is supposed to use
 
             - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
 
             - metadata: typing.Optional[UpdateAgentRequestMetadata]. Optional metadata
+
+            - instructions: typing.Optional[UpdateAgentRequestInstructions]. Instructions for the agent
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.update_agent(
             agent_id="agent_id",
+            about="about",
+            name="name",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if about is not OMIT:
-            _request["about"] = about
-        if instructions is not OMIT:
-            _request["instructions"] = instructions
-        if name is not OMIT:
-            _request["name"] = name
+        _request: typing.Dict[str, typing.Any] = {"about": about, "name": name}
         if model is not OMIT:
             _request["model"] = model
         if default_settings is not OMIT:
             _request["default_settings"] = default_settings
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if instructions is not OMIT:
+            _request["instructions"] = instructions
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"
             ),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -2918,60 +2973,60 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def patch_agent(
         self,
         agent_id: str,
         *,
         about: typing.Optional[str] = OMIT,
-        instructions: typing.Optional[typing.List[Instruction]] = OMIT,
         name: typing.Optional[str] = OMIT,
         model: typing.Optional[str] = OMIT,
         default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
         metadata: typing.Optional[PatchAgentRequestMetadata] = OMIT,
+        instructions: typing.Optional[PatchAgentRequestInstructions] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - agent_id: str.
 
             - about: typing.Optional[str]. About the agent
 
-            - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
-
             - name: typing.Optional[str]. Name of the agent
 
             - model: typing.Optional[str]. Name of the model that the agent is supposed to use
 
             - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
 
             - metadata: typing.Optional[PatchAgentRequestMetadata]. Optional metadata
+
+            - instructions: typing.Optional[PatchAgentRequestInstructions]. Instructions for the agent
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.patch_agent(
             agent_id="agent_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if about is not OMIT:
             _request["about"] = about
-        if instructions is not OMIT:
-            _request["instructions"] = instructions
         if name is not OMIT:
             _request["name"] = name
         if model is not OMIT:
             _request["model"] = model
         if default_settings is not OMIT:
             _request["default_settings"] = default_settings
         if metadata is not OMIT:
             _request["metadata"] = metadata
+        if instructions is not OMIT:
+            _request["instructions"] = instructions
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"
             ),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -3464,39 +3519,36 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def patch_agent_tool(
-        self, agent_id: str, tool_id: str, *, function: FunctionDef
+        self, agent_id: str, tool_id: str, *, function: PartialFunctionDef
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - agent_id: str.
 
             - tool_id: str.
 
-            - function: FunctionDef. Function definition and parameters
+            - function: PartialFunctionDef. Function definition and parameters
         ---
-        from julep import FunctionDef
+        from julep import PartialFunctionDef
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.patch_agent_tool(
             agent_id="agent_id",
             tool_id="tool_id",
-            function=FunctionDef(
-                name="name",
-                parameters={},
-            ),
+            function=PartialFunctionDef(),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"agents/{agent_id}/tools/{tool_id}",
```

### Comparing `julep-0.2.9/julep/api/core/__init__.py` & `julep-0.3.0/julep/api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/core/client_wrapper.py` & `julep-0.3.0/julep/api/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/core/datetime_utils.py` & `julep-0.3.0/julep/api/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/core/jsonable_encoder.py` & `julep-0.3.0/julep/api/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/__init__.py` & `julep-0.3.0/julep/api/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .agent import Agent
 from .agent_default_settings import AgentDefaultSettings
 from .agent_default_settings_preset import AgentDefaultSettingsPreset
+from .agent_instructions import AgentInstructions
 from .agent_metadata import AgentMetadata
 from .chat_input_data import ChatInputData
 from .chat_input_data_tool_choice import ChatInputDataToolChoice
 from .chat_ml_message import ChatMlMessage
 from .chat_ml_message_role import ChatMlMessageRole
 from .chat_response import ChatResponse
 from .chat_response_finish_reason import ChatResponseFinishReason
 from .chat_settings import ChatSettings
 from .chat_settings_preset import ChatSettingsPreset
 from .chat_settings_response_format import ChatSettingsResponseFormat
 from .chat_settings_response_format_schema import ChatSettingsResponseFormatSchema
 from .chat_settings_response_format_type import ChatSettingsResponseFormatType
 from .chat_settings_stop import ChatSettingsStop
 from .completion_usage import CompletionUsage
+from .create_agent_request_instructions import CreateAgentRequestInstructions
 from .create_agent_request_metadata import CreateAgentRequestMetadata
 from .create_doc import CreateDoc
 from .create_doc_metadata import CreateDocMetadata
 from .create_session_request_metadata import CreateSessionRequestMetadata
 from .create_tool_request import CreateToolRequest
 from .create_tool_request_type import CreateToolRequestType
 from .create_user_request_metadata import CreateUserRequestMetadata
@@ -37,69 +39,72 @@
 from .get_history_response import GetHistoryResponse
 from .get_suggestions_response import GetSuggestionsResponse
 from .get_user_docs_request_order import GetUserDocsRequestOrder
 from .get_user_docs_request_sort_by import GetUserDocsRequestSortBy
 from .get_user_docs_response import GetUserDocsResponse
 from .input_chat_ml_message import InputChatMlMessage
 from .input_chat_ml_message_role import InputChatMlMessageRole
-from .instruction import Instruction
 from .job_status import JobStatus
 from .job_status_state import JobStatusState
 from .list_agents_request_order import ListAgentsRequestOrder
 from .list_agents_request_sort_by import ListAgentsRequestSortBy
 from .list_agents_response import ListAgentsResponse
 from .list_sessions_request_order import ListSessionsRequestOrder
 from .list_sessions_request_sort_by import ListSessionsRequestSortBy
 from .list_sessions_response import ListSessionsResponse
 from .list_users_request_order import ListUsersRequestOrder
 from .list_users_request_sort_by import ListUsersRequestSortBy
 from .list_users_response import ListUsersResponse
 from .memory import Memory
 from .memory_access_options import MemoryAccessOptions
-from .memory_emotions_item import MemoryEmotionsItem
-from .memory_type import MemoryType
+from .memory_entities_item import MemoryEntitiesItem
 from .named_tool_choice import NamedToolChoice
 from .named_tool_choice_function import NamedToolChoiceFunction
+from .partial_function_def import PartialFunctionDef
+from .patch_agent_request_instructions import PatchAgentRequestInstructions
 from .patch_agent_request_metadata import PatchAgentRequestMetadata
 from .patch_session_request_metadata import PatchSessionRequestMetadata
 from .patch_user_request_metadata import PatchUserRequestMetadata
 from .resource_created_response import ResourceCreatedResponse
 from .resource_deleted_response import ResourceDeletedResponse
 from .resource_updated_response import ResourceUpdatedResponse
 from .session import Session
 from .session_metadata import SessionMetadata
 from .suggestion import Suggestion
 from .suggestion_target import SuggestionTarget
 from .tool import Tool
 from .tool_choice_option import ToolChoiceOption
 from .tool_type import ToolType
+from .update_agent_request_instructions import UpdateAgentRequestInstructions
 from .update_agent_request_metadata import UpdateAgentRequestMetadata
 from .update_session_request_metadata import UpdateSessionRequestMetadata
 from .update_user_request_metadata import UpdateUserRequestMetadata
 from .user import User
 from .user_metadata import UserMetadata
 
 __all__ = [
     "Agent",
     "AgentDefaultSettings",
     "AgentDefaultSettingsPreset",
+    "AgentInstructions",
     "AgentMetadata",
     "ChatInputData",
     "ChatInputDataToolChoice",
     "ChatMlMessage",
     "ChatMlMessageRole",
     "ChatResponse",
     "ChatResponseFinishReason",
     "ChatSettings",
     "ChatSettingsPreset",
     "ChatSettingsResponseFormat",
     "ChatSettingsResponseFormatSchema",
     "ChatSettingsResponseFormatType",
     "ChatSettingsStop",
     "CompletionUsage",
+    "CreateAgentRequestInstructions",
     "CreateAgentRequestMetadata",
     "CreateDoc",
     "CreateDocMetadata",
     "CreateSessionRequestMetadata",
     "CreateToolRequest",
     "CreateToolRequestType",
     "CreateUserRequestMetadata",
@@ -116,44 +121,45 @@
     "GetHistoryResponse",
     "GetSuggestionsResponse",
     "GetUserDocsRequestOrder",
     "GetUserDocsRequestSortBy",
     "GetUserDocsResponse",
     "InputChatMlMessage",
     "InputChatMlMessageRole",
-    "Instruction",
     "JobStatus",
     "JobStatusState",
     "ListAgentsRequestOrder",
     "ListAgentsRequestSortBy",
     "ListAgentsResponse",
     "ListSessionsRequestOrder",
     "ListSessionsRequestSortBy",
     "ListSessionsResponse",
     "ListUsersRequestOrder",
     "ListUsersRequestSortBy",
     "ListUsersResponse",
     "Memory",
     "MemoryAccessOptions",
-    "MemoryEmotionsItem",
-    "MemoryType",
+    "MemoryEntitiesItem",
     "NamedToolChoice",
     "NamedToolChoiceFunction",
+    "PartialFunctionDef",
+    "PatchAgentRequestInstructions",
     "PatchAgentRequestMetadata",
     "PatchSessionRequestMetadata",
     "PatchUserRequestMetadata",
     "ResourceCreatedResponse",
     "ResourceDeletedResponse",
     "ResourceUpdatedResponse",
     "Session",
     "SessionMetadata",
     "Suggestion",
     "SuggestionTarget",
     "Tool",
     "ToolChoiceOption",
     "ToolType",
+    "UpdateAgentRequestInstructions",
     "UpdateAgentRequestMetadata",
     "UpdateSessionRequestMetadata",
     "UpdateUserRequestMetadata",
     "User",
     "UserMetadata",
 ]
```

### Comparing `julep-0.2.9/julep/api/types/agent.py` & `julep-0.3.0/julep/api/types/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .agent_default_settings import AgentDefaultSettings
+from .agent_instructions import AgentInstructions
 from .agent_metadata import AgentMetadata
-from .instruction import Instruction
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class Agent(pydantic.BaseModel):
     name: str = pydantic.Field(description="Name of the agent")
     about: typing.Optional[str] = pydantic.Field(description="About the agent")
-    instructions: typing.Optional[typing.List[Instruction]] = pydantic.Field(
-        description="List of instructions for the agent"
-    )
     created_at: typing.Optional[dt.datetime] = pydantic.Field(
         description="Agent created at (RFC-3339 format)"
     )
     updated_at: typing.Optional[dt.datetime] = pydantic.Field(
         description="Agent updated at (RFC-3339 format)"
     )
     id: str = pydantic.Field(description="Agent id (UUID)")
     default_settings: typing.Optional[AgentDefaultSettings] = pydantic.Field(
         description="Default settings for all sessions created by this agent"
     )
     model: str = pydantic.Field(description="The model to use with this agent")
     metadata: typing.Optional[AgentMetadata] = pydantic.Field(
         description="Optional metadata"
     )
+    instructions: typing.Optional[AgentInstructions] = pydantic.Field(
+        description="Instructions for the agent"
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.9/julep/api/types/agent_default_settings.py` & `julep-0.3.0/julep/api/types/agent_default_settings.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/agent_default_settings_preset.py` & `julep-0.3.0/julep/api/types/agent_default_settings_preset.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/agent_metadata.py` & `julep-0.3.0/julep/api/types/agent_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/chat_input_data.py` & `julep-0.3.0/julep/api/types/chat_input_data.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/chat_ml_message.py` & `julep-0.3.0/julep/api/types/chat_ml_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,21 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class ChatMlMessage(pydantic.BaseModel):
     role: ChatMlMessageRole = pydantic.Field(
-        description=("ChatML role (system\n" "assistant\n" "user\n" "function_call)\n")
+        description=(
+            "ChatML role (system\n"
+            "assistant\n"
+            "user\n"
+            "function_call\n"
+            "function)\n"
+        )
     )
     content: str = pydantic.Field(description="ChatML content")
     name: typing.Optional[str] = pydantic.Field(description="ChatML name")
     created_at: dt.datetime = pydantic.Field(
         description="Message created at (RFC-3339 format)"
     )
     id: str = pydantic.Field(description="Message ID")
```

### Comparing `julep-0.2.9/julep/api/types/chat_ml_message_role.py` & `julep-0.3.0/julep/api/types/input_chat_ml_message_role.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,32 +2,40 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class ChatMlMessageRole(str, enum.Enum):
+class InputChatMlMessageRole(str, enum.Enum):
     """
-    ChatML role (system|assistant|user|function_call)
+    ChatML role (system|assistant|user|function_call|function|auto)
     """
 
     USER = "user"
     ASSISTANT = "assistant"
     SYSTEM = "system"
     FUNCTION_CALL = "function_call"
+    FUNCTION = "function"
+    AUTO = "auto"
 
     def visit(
         self,
         user: typing.Callable[[], T_Result],
         assistant: typing.Callable[[], T_Result],
         system: typing.Callable[[], T_Result],
         function_call: typing.Callable[[], T_Result],
+        function: typing.Callable[[], T_Result],
+        auto: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is ChatMlMessageRole.USER:
+        if self is InputChatMlMessageRole.USER:
             return user()
-        if self is ChatMlMessageRole.ASSISTANT:
+        if self is InputChatMlMessageRole.ASSISTANT:
             return assistant()
-        if self is ChatMlMessageRole.SYSTEM:
+        if self is InputChatMlMessageRole.SYSTEM:
             return system()
-        if self is ChatMlMessageRole.FUNCTION_CALL:
+        if self is InputChatMlMessageRole.FUNCTION_CALL:
             return function_call()
+        if self is InputChatMlMessageRole.FUNCTION:
+            return function()
+        if self is InputChatMlMessageRole.AUTO:
+            return auto()
```

### Comparing `julep-0.2.9/julep/api/types/chat_response.py` & `julep-0.3.0/julep/api/types/chat_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/chat_response_finish_reason.py` & `julep-0.3.0/julep/api/types/chat_response_finish_reason.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/chat_settings.py` & `julep-0.3.0/julep/api/types/chat_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 class ChatSettings(pydantic.BaseModel):
     frequency_penalty: typing.Optional[float] = pydantic.Field(
         description="(OpenAI-like) Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim."
     )
     length_penalty: typing.Optional[float] = pydantic.Field(
         description="(Huggingface-like) Number between 0 and 2.0. 1.0 is neutral and values larger than that penalize number of tokens generated."
     )
-    logit_bias: typing.Optional[
-        typing.Dict[str, typing.Optional[int]]
-    ] = pydantic.Field(
-        description=(
-            "Modify the likelihood of specified tokens appearing in the completion.\n"
-            "\n"
-            "Accepts a JSON object that maps tokens (specified by their token ID in the tokenizer) to an associated bias value from -100 to 100. Mathematically, the bias is added to the logits generated by the model prior to sampling. The exact effect will vary per model, but values between -1 and 1 should decrease or increase likelihood of selection; values like -100 or 100 should result in a ban or exclusive selection of the relevant token.\n"
+    logit_bias: typing.Optional[typing.Dict[str, typing.Optional[int]]] = (
+        pydantic.Field(
+            description=(
+                "Modify the likelihood of specified tokens appearing in the completion.\n"
+                "\n"
+                "Accepts a JSON object that maps tokens (specified by their token ID in the tokenizer) to an associated bias value from -100 to 100. Mathematically, the bias is added to the logits generated by the model prior to sampling. The exact effect will vary per model, but values between -1 and 1 should decrease or increase likelihood of selection; values like -100 or 100 should result in a ban or exclusive selection of the relevant token.\n"
+            )
         )
     )
     max_tokens: typing.Optional[int] = pydantic.Field(
         description=(
             "The maximum number of tokens to generate in the chat completion.\n"
             "\n"
             "The total length of input tokens and generated tokens is limited by the model's context length.\n"
```

### Comparing `julep-0.2.9/julep/api/types/chat_settings_preset.py` & `julep-0.3.0/julep/api/types/chat_settings_preset.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/chat_settings_response_format.py` & `julep-0.3.0/julep/api/types/chat_settings_response_format.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/chat_settings_response_format_schema.py` & `julep-0.3.0/julep/api/types/chat_settings_response_format_schema.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/chat_settings_response_format_type.py` & `julep-0.3.0/julep/api/types/chat_settings_response_format_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/completion_usage.py` & `julep-0.3.0/julep/api/types/completion_usage.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/create_agent_request_metadata.py` & `julep-0.3.0/julep/api/types/patch_user_request_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class CreateAgentRequestMetadata(pydantic.BaseModel):
+class PatchUserRequestMetadata(pydantic.BaseModel):
     """
     Optional metadata
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
```

### Comparing `julep-0.2.9/julep/api/types/create_doc.py` & `julep-0.3.0/julep/api/types/create_doc.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/create_doc_metadata.py` & `julep-0.3.0/julep/api/types/create_doc_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/create_session_request_metadata.py` & `julep-0.3.0/julep/api/types/create_session_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/create_tool_request.py` & `julep-0.3.0/julep/api/types/create_tool_request.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/create_tool_request_type.py` & `julep-0.3.0/julep/api/types/create_tool_request_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/create_user_request_metadata.py` & `julep-0.3.0/julep/api/types/create_user_request_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class CreateUserRequestMetadata(pydantic.BaseModel):
     """
-    Optional metadata
+    (Optional) metadata
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
```

### Comparing `julep-0.2.9/julep/api/types/doc.py` & `julep-0.3.0/julep/api/types/doc.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/doc_metadata.py` & `julep-0.3.0/julep/api/types/doc_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/function_call_option.py` & `julep-0.3.0/julep/api/types/function_call_option.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/function_def.py` & `julep-0.3.0/julep/api/types/function_def.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/get_agent_docs_request_sort_by.py` & `julep-0.3.0/julep/api/types/get_agent_docs_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/get_agent_docs_response.py` & `julep-0.3.0/julep/api/types/get_agent_docs_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/get_agent_memories_response.py` & `julep-0.3.0/julep/api/types/get_agent_memories_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/get_agent_tools_response.py` & `julep-0.3.0/julep/api/types/get_agent_tools_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/get_history_response.py` & `julep-0.3.0/julep/api/types/get_history_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/get_suggestions_response.py` & `julep-0.3.0/julep/api/types/get_suggestions_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/get_user_docs_request_sort_by.py` & `julep-0.3.0/julep/api/types/get_user_docs_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/get_user_docs_response.py` & `julep-0.3.0/julep/api/types/get_user_docs_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/input_chat_ml_message.py` & `julep-0.3.0/julep/api/types/partial_function_def.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .input_chat_ml_message_role import InputChatMlMessageRole
+from .function_parameters import FunctionParameters
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class InputChatMlMessage(pydantic.BaseModel):
-    role: InputChatMlMessageRole = pydantic.Field(
-        description=("ChatML role (system\n" "assistant\n" "user\n" "function_call)\n")
+class PartialFunctionDef(pydantic.BaseModel):
+    description: typing.Optional[str] = pydantic.Field(
+        description="A description of what the function does, used by the model to choose when and how to call the function."
     )
-    content: str = pydantic.Field(description="ChatML content")
-    name: typing.Optional[str] = pydantic.Field(description="ChatML name")
-    continue_: typing.Optional[bool] = pydantic.Field(
-        alias="continue",
-        description="Whether to continue this message or return a new one",
+    name: typing.Optional[str] = pydantic.Field(
+        description="The name of the function to be called. Must be a-z, A-Z, 0-9, or contain underscores and dashes, with a maximum length of 64."
+    )
+    parameters: typing.Optional[FunctionParameters] = pydantic.Field(
+        description="Parameters accepeted by this function"
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
@@ -38,9 +38,8 @@
             **kwargs,
         }
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `julep-0.2.9/julep/api/types/input_chat_ml_message_role.py` & `julep-0.3.0/julep/api/types/chat_ml_message_role.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class InputChatMlMessageRole(str, enum.Enum):
+class ChatMlMessageRole(str, enum.Enum):
     """
-    ChatML role (system|assistant|user|function_call)
+    ChatML role (system|assistant|user|function_call|function)
     """
 
     USER = "user"
     ASSISTANT = "assistant"
     SYSTEM = "system"
     FUNCTION_CALL = "function_call"
-    AUTO = "auto"
+    FUNCTION = "function"
 
     def visit(
         self,
         user: typing.Callable[[], T_Result],
         assistant: typing.Callable[[], T_Result],
         system: typing.Callable[[], T_Result],
         function_call: typing.Callable[[], T_Result],
-        auto: typing.Callable[[], T_Result],
+        function: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is InputChatMlMessageRole.USER:
+        if self is ChatMlMessageRole.USER:
             return user()
-        if self is InputChatMlMessageRole.ASSISTANT:
+        if self is ChatMlMessageRole.ASSISTANT:
             return assistant()
-        if self is InputChatMlMessageRole.SYSTEM:
+        if self is ChatMlMessageRole.SYSTEM:
             return system()
-        if self is InputChatMlMessageRole.FUNCTION_CALL:
+        if self is ChatMlMessageRole.FUNCTION_CALL:
             return function_call()
-        if self is InputChatMlMessageRole.AUTO:
-            return auto()
+        if self is ChatMlMessageRole.FUNCTION:
+            return function()
```

### Comparing `julep-0.2.9/julep/api/types/instruction.py` & `julep-0.3.0/julep/api/types/tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .function_def import FunctionDef
+from .tool_type import ToolType
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class Instruction(pydantic.BaseModel):
-    content: str = pydantic.Field(description="Content of the instruction")
-    important: typing.Optional[bool] = pydantic.Field(
-        description="Whether this instruction should be marked as important (only up to 3 instructions per agent can be marked important)"
+class Tool(pydantic.BaseModel):
+    type: ToolType = pydantic.Field(
+        description="Whether this tool is a `function` or a `webhook` (Only `function` tool supported right now)"
     )
+    function: FunctionDef = pydantic.Field(
+        description="Function definition and parameters"
+    )
+    id: str = pydantic.Field(description="Tool ID")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.9/julep/api/types/job_status.py` & `julep-0.3.0/julep/api/types/job_status.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/job_status_state.py` & `julep-0.3.0/julep/api/types/job_status_state.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/list_agents_request_sort_by.py` & `julep-0.3.0/julep/api/types/list_agents_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/list_agents_response.py` & `julep-0.3.0/julep/api/types/list_agents_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/list_sessions_request_sort_by.py` & `julep-0.3.0/julep/api/types/list_sessions_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/list_sessions_response.py` & `julep-0.3.0/julep/api/types/list_sessions_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/list_users_request_sort_by.py` & `julep-0.3.0/julep/api/types/list_users_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/list_users_response.py` & `julep-0.3.0/julep/api/types/list_users_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/memory.py` & `julep-0.3.0/julep/api/types/user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .memory_emotions_item import MemoryEmotionsItem
-from .memory_type import MemoryType
+from .user_metadata import UserMetadata
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class Memory(pydantic.BaseModel):
-    type: MemoryType = pydantic.Field(
-        description="Type of memory (`episode` or `belief`)"
+class User(pydantic.BaseModel):
+    name: typing.Optional[str] = pydantic.Field(description="Name of the user")
+    about: typing.Optional[str] = pydantic.Field(description="About the user")
+    created_at: typing.Optional[dt.datetime] = pydantic.Field(
+        description="User created at (RFC-3339 format)"
+    )
+    updated_at: typing.Optional[dt.datetime] = pydantic.Field(
+        description="User updated at (RFC-3339 format)"
+    )
+    id: str = pydantic.Field(description="User id (UUID)")
+    metadata: typing.Optional[UserMetadata] = pydantic.Field(
+        description="(Optional) metadata"
     )
-    agent_id: str = pydantic.Field(description="ID of the agent")
-    user_id: str = pydantic.Field(description="ID of the user")
-    content: str = pydantic.Field(description="Content of the memory")
-    weight: typing.Optional[float] = pydantic.Field(
-        description="Weight (importance) of the memory on a scale of 0-100"
-    )
-    created_at: dt.datetime = pydantic.Field(
-        description="Memory created at (RFC-3339 format)"
-    )
-    last_accessed_at: typing.Optional[dt.datetime] = pydantic.Field(
-        description="Memory last accessed at (RFC-3339 format)"
-    )
-    timestamp: typing.Optional[dt.datetime] = pydantic.Field(
-        description="Memory happened at (RFC-3339 format)"
-    )
-    sentiment: typing.Optional[float] = pydantic.Field(
-        description="Sentiment (valence) of the memory on a scale of -1 to 1"
-    )
-    duration: typing.Optional[float] = pydantic.Field(
-        description="Duration of the Memory (in seconds)"
-    )
-    id: str = pydantic.Field(description="Memory id (UUID)")
-    emotions: typing.Optional[typing.List[MemoryEmotionsItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.9/julep/api/types/memory_access_options.py` & `julep-0.3.0/julep/api/types/memory_access_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,19 @@
     import pydantic  # type: ignore
 
 
 class MemoryAccessOptions(pydantic.BaseModel):
     recall: typing.Optional[bool] = pydantic.Field(
         description="Whether previous memories should be recalled or not"
     )
+    record: typing.Optional[bool] = pydantic.Field(
+        description="Whether this interaction should be recorded in history or not"
+    )
     remember: typing.Optional[bool] = pydantic.Field(
-        description="Whether this interaction should be recorded in memory or not"
+        description="Whether this interaction should form memories or not"
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
```

### Comparing `julep-0.2.9/julep/api/types/memory_type.py` & `julep-0.3.0/julep/api/types/tool_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class MemoryType(str, enum.Enum):
+class ToolType(str, enum.Enum):
     """
-    Type of memory (`episode` or `belief`)
+    Whether this tool is a `function` or a `webhook` (Only `function` tool supported right now)
     """
 
-    EPISODE = "episode"
-    BELIEF = "belief"
+    FUNCTION = "function"
+    WEBHOOK = "webhook"
 
     def visit(
         self,
-        episode: typing.Callable[[], T_Result],
-        belief: typing.Callable[[], T_Result],
+        function: typing.Callable[[], T_Result],
+        webhook: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is MemoryType.EPISODE:
-            return episode()
-        if self is MemoryType.BELIEF:
-            return belief()
+        if self is ToolType.FUNCTION:
+            return function()
+        if self is ToolType.WEBHOOK:
+            return webhook()
```

### Comparing `julep-0.2.9/julep/api/types/named_tool_choice.py` & `julep-0.3.0/julep/api/types/named_tool_choice.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/named_tool_choice_function.py` & `julep-0.3.0/julep/api/types/named_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/patch_agent_request_metadata.py` & `julep-0.3.0/julep/api/types/patch_agent_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/patch_session_request_metadata.py` & `julep-0.3.0/julep/api/types/patch_session_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/patch_user_request_metadata.py` & `julep-0.3.0/julep/api/types/update_user_request_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class PatchUserRequestMetadata(pydantic.BaseModel):
+class UpdateUserRequestMetadata(pydantic.BaseModel):
     """
     Optional metadata
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
```

### Comparing `julep-0.2.9/julep/api/types/resource_created_response.py` & `julep-0.3.0/julep/api/types/resource_created_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/resource_deleted_response.py` & `julep-0.3.0/julep/api/types/update_agent_request_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ResourceDeletedResponse(pydantic.BaseModel):
-    id: str
-    deleted_at: dt.datetime
+class UpdateAgentRequestMetadata(pydantic.BaseModel):
+    """
+    Optional metadata
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.9/julep/api/types/resource_updated_response.py` & `julep-0.3.0/julep/api/types/resource_updated_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/session.py` & `julep-0.3.0/julep/api/types/session.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     )
     updated_at: typing.Optional[dt.datetime] = pydantic.Field(
         description="Session updated at (RFC-3339 format)"
     )
     metadata: typing.Optional[SessionMetadata] = pydantic.Field(
         description="Optional metadata"
     )
+    render_templates: typing.Optional[bool] = pydantic.Field(
+        description="Render system and assistant message content as jinja templates"
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.9/julep/api/types/session_metadata.py` & `julep-0.3.0/julep/api/types/session_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/suggestion.py` & `julep-0.3.0/julep/api/types/suggestion.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/suggestion_target.py` & `julep-0.3.0/julep/api/types/suggestion_target.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.9/julep/api/types/tool.py` & `julep-0.3.0/julep/api/types/update_session_request_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .function_def import FunctionDef
-from .tool_type import ToolType
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class Tool(pydantic.BaseModel):
-    type: ToolType = pydantic.Field(
-        description="Whether this tool is a `function` or a `webhook` (Only `function` tool supported right now)"
-    )
-    function: FunctionDef = pydantic.Field(
-        description="Function definition and parameters"
-    )
-    id: str = pydantic.Field(description="Tool ID")
+class UpdateSessionRequestMetadata(pydantic.BaseModel):
+    """
+    Optional metadata
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.9/julep/api/types/update_agent_request_metadata.py` & `julep-0.3.0/julep/api/types/user_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UpdateAgentRequestMetadata(pydantic.BaseModel):
+class UserMetadata(pydantic.BaseModel):
     """
-    Optional metadata
+    (Optional) metadata
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
```

### Comparing `julep-0.2.9/julep/api/types/update_session_request_metadata.py` & `julep-0.3.0/julep/api/types/resource_deleted_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UpdateSessionRequestMetadata(pydantic.BaseModel):
-    """
-    Optional metadata
-    """
+class ResourceDeletedResponse(pydantic.BaseModel):
+    id: str
+    deleted_at: dt.datetime
+    jobs: typing.Optional[typing.List[str]] = pydantic.Field(
+        description="IDs (if any) of jobs created as part of this request"
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.9/julep/api/types/update_user_request_metadata.py` & `julep-0.3.0/julep/api/types/memory_entities_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UpdateUserRequestMetadata(pydantic.BaseModel):
-    """
-    Optional metadata
-    """
-
+class MemoryEntitiesItem(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
         return super().json(**kwargs_with_defaults)
```

### Comparing `julep-0.2.9/julep/api/types/user.py` & `julep-0.3.0/julep/api/types/memory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .user_metadata import UserMetadata
+from .memory_entities_item import MemoryEntitiesItem
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class User(pydantic.BaseModel):
-    name: typing.Optional[str] = pydantic.Field(description="Name of the user")
-    about: typing.Optional[str] = pydantic.Field(description="About the user")
-    created_at: typing.Optional[dt.datetime] = pydantic.Field(
-        description="User created at (RFC-3339 format)"
+class Memory(pydantic.BaseModel):
+    agent_id: str = pydantic.Field(description="ID of the agent")
+    user_id: str = pydantic.Field(description="ID of the user")
+    content: str = pydantic.Field(description="Content of the memory")
+    created_at: dt.datetime = pydantic.Field(
+        description="Memory created at (RFC-3339 format)"
     )
-    updated_at: typing.Optional[dt.datetime] = pydantic.Field(
-        description="User updated at (RFC-3339 format)"
+    last_accessed_at: typing.Optional[dt.datetime] = pydantic.Field(
+        description="Memory last accessed at (RFC-3339 format)"
     )
-    id: str = pydantic.Field(description="User id (UUID)")
-    metadata: typing.Optional[UserMetadata] = pydantic.Field(
-        description="Optional metadata"
+    timestamp: typing.Optional[dt.datetime] = pydantic.Field(
+        description="Memory happened at (RFC-3339 format)"
+    )
+    sentiment: typing.Optional[float] = pydantic.Field(
+        description="Sentiment (valence) of the memory on a scale of -1 to 1"
+    )
+    id: str = pydantic.Field(description="Memory id (UUID)")
+    entities: typing.List[MemoryEntitiesItem] = pydantic.Field(
+        description="List of entities mentioned in the memory"
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
```

### Comparing `julep-0.2.9/julep/api/types/user_metadata.py` & `julep-0.3.0/julep/api/types/create_agent_request_metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UserMetadata(pydantic.BaseModel):
+class CreateAgentRequestMetadata(pydantic.BaseModel):
     """
-    Optional metadata
+    (Optional) metadata
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
```

### Comparing `julep-0.2.9/julep/client.py` & `julep-0.3.0/julep/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Dict, Optional
 from urllib.parse import urlparse
 
 from beartype import beartype
 import httpx
 from openai import AsyncOpenAI, OpenAI
 from openai.resources.chat.chat import AsyncChat, Chat
 from openai.resources.completions import AsyncCompletions, Completions
@@ -77,14 +77,15 @@
 
     @beartype
     def __init__(
         self,
         api_key: Optional[str] = JULEP_API_KEY,
         base_url: Optional[str] = JULEP_API_URL,
         timeout: int = 300,
+        additional_headers: Dict[str, str] = {},
         _httpx_client: Optional[httpx.Client] = None,
         *args,
         **kwargs,
     ):
         """
         Initialize a new client object with the given API key and base URL.
 
@@ -111,19 +112,20 @@
         assert (
             base_url is not None
         ), "base_url must be provided or set as env var JULEP_API_URL"
 
         # Create an httpz client that follows redirects and has a timeout
         httpx_client = _httpx_client or httpx.Client(
             timeout=timeout,
+            headers=additional_headers,
             follow_redirects=True,
         )
 
         self._api_client = JulepApi(
-            api_key=api_key,
+            api_key=f"Bearer {api_key}",
             base_url=base_url,
             httpx_client=httpx_client,
             *args,
             **kwargs,
         )
 
         self.agents = AgentsManager(api_client=self._api_client)
@@ -236,15 +238,15 @@
             api_key is not None
         ), "api_key must be provided or set as env var JULEP_API_KEY"
         assert (
             base_url is not None
         ), "base_url must be provided or set as env var JULEP_API_URL"
 
         self._api_client = AsyncJulepApi(
-            api_key=api_key, base_url=base_url, *args, **kwargs
+            api_key=f"Bearer {api_key}", base_url=base_url, *args, **kwargs
         )
 
         self.agents = AsyncAgentsManager(api_client=self._api_client)
         self.users = AsyncUsersManager(api_client=self._api_client)
         self.sessions = AsyncSessionsManager(api_client=self._api_client)
         self.docs = AsyncDocsManager(api_client=self._api_client)
         self.memories = AsyncMemoriesManager(api_client=self._api_client)
```

### Comparing `julep-0.2.9/julep/managers/agent.py` & `julep-0.3.0/julep/managers/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,60 +6,62 @@
 from beartype.typing import Any, Awaitable, Dict, List, Literal, Union
 
 from ..api.types import (
     Agent,
     AgentDefaultSettings,
     CreateDoc,
     CreateToolRequest,
-    Instruction,
     ResourceCreatedResponse,
     ListAgentsResponse,
     ResourceUpdatedResponse,
 )
 
 from .utils import rewrap_in_class
 
 from .base import BaseManager
-from .utils import is_valid_uuid4
+from .utils import is_valid_uuid4, NotSet
 from .types import (
     ToolDict,
     FunctionDefDict,
     DefaultSettingsDict,
     DocDict,
-    InstructionDict,
 )
 
 
 ###########
 ## TYPES ##
 ###########
 
+
 ModelName = Literal[
     "julep-ai/samantha-1",
     "julep-ai/samantha-1-turbo",
 ]
 
 
 class AgentCreateArgs(TypedDict):
     name: str
-    about: str
-    instructions: Union[List[str], List[InstructionDict]]
+    about: Optional[str]
+    instructions: Optional[List[str]]
     tools: List[ToolDict] = []
     functions: List[FunctionDefDict] = []
     default_settings: DefaultSettingsDict = {}
     model: ModelName = "julep-ai/samantha-1-turbo"
     docs: List[DocDict] = []
+    metadata: Dict[str, Any] = {}
 
 
 class AgentUpdateArgs(TypedDict):
     about: Optional[str] = None
-    instructions: Optional[Union[List[str], List[InstructionDict]]] = None
+    instructions: Optional[List[str]] = None
     name: Optional[str] = None
     model: Optional[str] = None
     default_settings: Optional[DefaultSettingsDict] = None
+    metadata: Optional[Dict[str, Any]] = None
+    overwrite: bool = False
 
 
 class BaseAgentsManager(BaseManager):
     """
     A class responsible for managing agent entities.
 
     This manager handles CRUD operations for agents including retrieving, creating, listing, deleting, and updating agents using an API client.
@@ -71,52 +73,55 @@
         _get(self, id: Union[str, UUID]) -> Union[Agent, Awaitable[Agent]]:
             Retrieves a single agent by its UUID.
             Args:
                 id (Union[str, UUID]): The UUID of the agent to retrieve.
             Returns:
                 The agent object or an awaitable that resolves to the agent object.
 
-        _create(self, name: str, about: str, instructions: Union[List[str], List[InstructionDict]], tools: List[ToolDict] = [], functions: List[FunctionDefDict] = [], default_settings: DefaultSettingsDict = {}, model: ModelName = 'julep-ai/samantha-1-turbo', docs: List[DocDict] = []) -> Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]:
+        _create(self, name: str, about: str, instructions: List[str], tools: List[ToolDict] = [], functions: List[FunctionDefDict] = [], default_settings: DefaultSettingsDict = {}, model: ModelName = 'julep-ai/samantha-1-turbo', docs: List[DocDict] = [], metadata: Dict[str, Any] = {}) -> Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]:
             Creates an agent with the given specifications.
             Args:
                 name (str): The name of the new agent.
                 about (str): Description about the new agent.
-                instructions (Union[List[str], List[InstructionDict]]): List of instructions or instruction dictionaries for the new agent.
+                instructions (List[str]): List of instructions or instruction dictionaries for the new agent.
                 tools (List[ToolDict], optional): List of tool dictionaries. Defaults to an empty list.
                 functions (List[FunctionDefDict], optional): List of function definition dictionaries. Defaults to an empty list.
                 default_settings (DefaultSettingsDict, optional): Dictionary of default settings for the new agent. Defaults to an empty dictionary.
                 model (ModelName, optional): The model name for the new agent. Defaults to 'julep-ai/samantha-1-turbo'.
                 docs (List[DocDict], optional): List of document dictionaries for the new agent. Defaults to an empty list.
+                metadata (Dict[str, Any], optional): Dictionary of metadata for the new agent. Defaults to an empty dictionary.
             Returns:
                 The response indicating creation or an awaitable that resolves to the creation response.
 
-        _list_items(self, limit: Optional[int] = None, offset: Optional[int] = None) -> Union[ListAgentsResponse, Awaitable[ListAgentsResponse]]:
-            Lists agents with pagination support.
+        _list_items(self, limit: Optional[int] = None, offset: Optional[int] = None, metadata_filter: Dict[str, Any] = {}) -> Union[ListAgentsResponse, Awaitable[ListAgentsResponse]]:
+            Lists agents with pagination support and optional metadata filtering.
             Args:
                 limit (Optional[int], optional): The maximum number of agents to list. Defaults to None.
                 offset (Optional[int], optional): The number of agents to skip (for pagination). Defaults to None.
+                metadata_filter (Dict[str, Any], optional): Filters for querying agents based on metadata. Defaults to an empty dictionary.
             Returns:
                 The list of agents or an awaitable that resolves to the list of agents.
 
         _delete(self, agent_id: Union[str, UUID]) -> Union[None, Awaitable[None]]:
             Deletes an agent with the specified UUID.
             Args:
                 agent_id (Union[str, UUID]): The UUID of the agent to delete.
             Returns:
                 None or an awaitable that resolves to None.
 
-        _update(self, agent_id: Union[str, UUID], about: Optional[str] = None, instructions: Optional[Union[List[str], List[InstructionDict]]] = None, name: Optional[str] = None, model: Optional[str] = None, default_settings: Optional[DefaultSettingsDict] = None) -> Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]:
+        _update(self, agent_id: Union[str, UUID], about: Optional[str] = None, instructions: Optional[List[str]] = None, name: Optional[str] = None, model: Optional[str] = None, default_settings: Optional[DefaultSettingsDict] = None, metadata: Dict[str, Any] = {}) -> Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]:
             Updates the specified fields of an agent.
             Args:
                 agent_id (Union[str, UUID]): The UUID of the agent to update.
                 about (Optional[str], optional): The new description about the agent.
-                instructions (Optional[Union[List[str], List[InstructionDict]]], optional): The new list of instructions or instruction dictionaries.
+                instructions (Optional[List[str]], optional): The new list of instructions or instruction dictionaries.
                 name (Optional[str], optional): The new name for the agent.
                 model (Optional[str], optional): The new model name for the agent.
                 default_settings (Optional[DefaultSettingsDict], optional): The new default settings dictionary for the agent.
+                metadata (Dict[str, Any])
             Returns:
                 The response indicating successful update or an awaitable that resolves to the update response.
     """
 
     def _get(self, id: Union[str, UUID]) -> Union[Agent, Awaitable[Agent]]:
         """
         Retrieves an agent based on the provided identifier.
@@ -132,54 +137,49 @@
         """
         assert is_valid_uuid4(id), "id must be a valid UUID v4"
         return self.api_client.get_agent(agent_id=id)
 
     def _create(
         self,
         name: str,
-        about: str,
-        instructions: Union[List[str], List[InstructionDict]],
+        about: str = "",
+        instructions: List[str] = [],
         tools: List[ToolDict] = [],
         functions: List[FunctionDefDict] = [],
         default_settings: DefaultSettingsDict = {},
         model: ModelName = "julep-ai/samantha-1-turbo",
         docs: List[DocDict] = [],
+        metadata: Dict[str, Any] = {},
     ) -> Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]:
-        # Cast instructions to a list of Instruction objects
+        # Instructions are expected to be provided in the correct format
         """
         Create a new agent with the specified configuration.
 
         Args:
             name (str): Name of the agent.
             about (str): Information about the agent.
-            instructions (Union[List[str], List[InstructionDict]]): List of instructions as either string or dictionaries for the agent.
+            instructions (List[str]): List of instructions as either string or dictionaries for the agent.
             tools (List[ToolDict], optional): List of tool configurations for the agent. Defaults to an empty list.
             functions (List[FunctionDefDict], optional): List of function definitions for the agent. Defaults to an empty list.
             default_settings (DefaultSettingsDict, optional): Dictionary of default settings for the agent. Defaults to an empty dict.
             model (ModelName, optional): The model name identifier. Defaults to 'julep-ai/samantha-1-turbo'.
             docs (List[DocDict], optional): List of document configurations for the agent. Defaults to an empty list.
+            metadata (Dict[str, Any])
 
         Returns:
             Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]: The response object indicating the resource has been created or a future of the response object if the creation is being awaited.
 
         Raises:
             AssertionError: If both functions and tools are provided.
 
         Notes:
             The `_create` method is meant to be used internally and should be considered private.
             It assumes the input data for instructions, tools, and docs will have the proper format,
             and items in the 'instructions' list will be converted to Instruction instances.
         """
-        instructions: List[Instruction] = [
-            Instruction(content=content, important=False)
-            if isinstance(content, str)
-            else Instruction(**content)
-            for content in instructions
-        ]
-
         # Ensure that only functions or tools are provided
         assert not (functions and tools), "Only functions or tools can be provided"
 
         # Cast functions/tools to a list of CreateToolRequest objects
         tools: List[CreateToolRequest] = (
             [
                 CreateToolRequest(type="function", function=function)
@@ -201,14 +201,15 @@
             name=name,
             about=about,
             instructions=instructions,
             tools=tools,
             default_settings=default_settings,
             model=model,
             docs=docs,
+            metadata=metadata,
         )
 
     def _list_items(
         self,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         metadata_filter: str = "{}",
@@ -248,64 +249,69 @@
         """
         assert is_valid_uuid4(agent_id), "id must be a valid UUID v4"
         return self.api_client.delete_agent(agent_id=agent_id)
 
     def _update(
         self,
         agent_id: Union[str, UUID],
-        about: Optional[str] = None,
-        instructions: Optional[Union[List[str], List[InstructionDict]]] = None,
-        name: Optional[str] = None,
-        model: Optional[str] = None,
-        default_settings: Optional[DefaultSettingsDict] = None,
+        about: Optional[str] = NotSet,
+        instructions: List[str] = NotSet,
+        name: Optional[str] = NotSet,
+        model: Optional[str] = NotSet,
+        default_settings: Optional[DefaultSettingsDict] = NotSet,
+        metadata: Dict[str, Any] = NotSet,
+        overwrite: bool = False,
     ) -> Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]:
         """
         Update the agent's properties.
 
             Args:
                 agent_id (Union[str, UUID]): The unique identifier for the agent, which can be a string or UUID object.
                 about (Optional[str], optional): A brief description of the agent. Defaults to None.
-                instructions (Optional[Union[List[str], List[InstructionDict]]], optional): A list of either strings or instruction dictionaries that will be converted into Instruction objects. Defaults to None.
+                instructions (Optional[List[str]], optional): A list of either strings or instruction dictionaries that will be converted into Instruction objects. Defaults to None.
                 name (Optional[str], optional): The name of the agent. Defaults to None.
                 model (Optional[str], optional): The model identifier for the agent. Defaults to None.
                 default_settings (Optional[DefaultSettingsDict], optional): A dictionary of default settings to apply to the agent. Defaults to None.
+                metadata (Dict[str, Any])
+                overwrite (bool, optional): Whether to overwrite the existing agent settings. Defaults to False.
 
             Returns:
                 Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]: An object representing the response for the resource updated, which can also be an awaitable in asynchronous contexts.
 
             Raises:
-                AssertionError: If the provided agent_id is not a valid UUID v4.
+                AssertionError: If the provided agent_id is not validated by the is_valid_uuid4 function.
 
             Note:
                 This method asserts that the agent_id must be a valid UUID v4. The instructions and default_settings, if provided, are converted into their respective object types before making the update API call.
         """
         assert is_valid_uuid4(agent_id), "id must be a valid UUID v4"
 
-        if instructions is not None:
-            instructions: List[Instruction] = [
-                Instruction(content=content, important=False)
-                if isinstance(content, str)
-                else Instruction(**content)
-                for content in instructions
-            ]
-
-        if default_settings is not None:
+        if default_settings is not NotSet:
             default_settings: AgentDefaultSettings = AgentDefaultSettings(
                 **default_settings
             )
 
-        return self.api_client.update_agent(
+        updateFn = (
+            self.api_client.update_agent if overwrite else self.api_client.patch_agent
+        )
+
+        update_payload = dict(
             agent_id=agent_id,
             about=about,
             instructions=instructions,
             name=name,
             model=model,
             default_settings=default_settings,
+            metadata=metadata,
         )
 
+        update_payload = {k: v for k, v in update_payload.items() if v is not NotSet}
+
+        return updateFn(**update_payload)
+
 
 class AgentsManager(BaseAgentsManager):
     """
     A class for managing agents, inheriting from `BaseAgentsManager`.
 
     This class provides functionalities to interact with and manage agents, including creating, retrieving, listing, updating, and deleting agents. It utilizes type annotations to ensure type correctness at runtime using the `beartype` decorator.
 
@@ -315,26 +321,27 @@
 
             Args:
                 id (Union[str, UUID]): The unique identifier of the agent, which can be either a string or a UUID.
 
             Returns:
                 Agent: The agent with the corresponding identifier.
 
-        create(*, name: str, about: str, instructions: Union[List[str], List[InstructionDict]], tools: List[ToolDict]=[], functions: List[FunctionDefDict]=[], default_settings: DefaultSettingsDict={}, model: ModelName='julep-ai/samantha-1-turbo', docs: List[DocDict]=[]) -> ResourceCreatedResponse:
+        create(*, name: str, about: str, instructions: List[str], tools: List[ToolDict]=[], functions: List[FunctionDefDict]=[], default_settings: DefaultSettingsDict={}, model: ModelName='julep-ai/samantha-1-turbo', docs: List[DocDict]=[]) -> ResourceCreatedResponse:
             Creates a new agent with the provided details.
 
             Args:
                 name (str): The name of the agent.
                 about (str): A description of the agent.
-                instructions (Union[List[str], List[InstructionDict]]): A list of instructions or dictionaries defining instructions.
+                instructions (List[str]): A list of instructions or dictionaries defining instructions.
                 tools (List[ToolDict], optional): A list of dictionaries defining tools. Defaults to an empty list.
                 functions (List[FunctionDefDict], optional): A list of dictionaries defining functions. Defaults to an empty list.
                 default_settings (DefaultSettingsDict, optional): A dictionary of default settings. Defaults to an empty dictionary.
                 model (ModelName, optional): The model name to be used. Defaults to 'julep-ai/samantha-1-turbo'.
                 docs (List[DocDict], optional): A list of dictionaries defining documentation. Defaults to an empty list.
+                metadata (Dict[str, Any])
 
             Returns:
                 ResourceCreatedResponse: The response indicating the resource (agent) was successfully created.
 
         list(*, limit: Optional[int]=None, offset: Optional[int]=None) -> List[Agent]:
             Lists all agents with pagination support.
 
@@ -347,24 +354,25 @@
 
         delete(agent_id: Union[str, UUID]):
             Deletes an agent by its unique identifier.
 
             Args:
                 agent_id (Union[str, UUID]): The unique identifier of the agent to be deleted.
 
-        update(*, agent_id: Union[str, UUID], about: Optional[str]=None, instructions: Optional[Union[List[str], List[InstructionDict]]]=None, name: Optional[str]=None, model: Optional[str]=None, default_settings: Optional[DefaultSettingsDict]=None) -> ResourceUpdatedResponse:
+        update(*, agent_id: Union[str, UUID], about: Optional[str]=None, instructions: Optional[List[str]]=None, name: Optional[str]=None, model: Optional[str]=None, default_settings: Optional[DefaultSettingsDict]=None) -> ResourceUpdatedResponse:
             Updates an existing agent with new details.
 
             Args:
                 agent_id (Union[str, UUID]): The unique identifier of the agent to be updated.
                 about (Optional[str], optional): A new description of the agent. Defaults to None (no change).
-                instructions (Optional[Union[List[str], List[InstructionDict]]], optional): A new list of instructions or dictionaries defining instructions. Defaults to None (no change).
+                instructions (Optional[List[str]], optional): A new list of instructions or dictionaries defining instructions. Defaults to None (no change).
                 name (Optional[str], optional): A new name for the agent. Defaults to None (no change).
                 model (Optional[str], optional): A new model name to be used. Defaults to None (no change).
                 default_settings (Optional[DefaultSettingsDict], optional): A new dictionary of default settings. Defaults to None (no change).
+                metadata (Dict[str, Any])
 
             Returns:
                 ResourceUpdatedResponse: The response indicating the resource (agent) was successfully updated.
     """
 
     @beartype
     def get(self, id: Union[str, UUID]) -> Agent:
@@ -388,20 +396,21 @@
     def create(self, **kwargs: AgentCreateArgs) -> Agent:
         """
         Creates a new resource with the specified details.
 
         Args:
             name (str): The name of the resource.
             about (str): A description of the resource.
-            instructions (Union[List[str], List[InstructionDict]]): A list of instructions or dictionaries with instruction details.
+            instructions (List[str]): A list of instructions or dictionaries with instruction details.
             tools (List[ToolDict], optional): A list of dictionaries with tool details. Defaults to an empty list.
             functions (List[FunctionDefDict], optional): A list of dictionaries with function definition details. Defaults to an empty list.
             default_settings (DefaultSettingsDict, optional): A dictionary with default settings. Defaults to an empty dictionary.
             model (ModelName, optional): The name of the model to use. Defaults to 'julep-ai/samantha-1-turbo'.
             docs (List[DocDict], optional): A list of dictionaries with documentation details. Defaults to an empty list.
+            metadata (Dict[str, Any])
 
         Returns:
             Agent: An instance of the Agent with the specified details
 
         Note:
             This function is decorated with `@beartype`, which will perform runtime type checking on the arguments.
         """
@@ -465,25 +474,28 @@
         Update the properties of a resource.
 
         This function updates various attributes of an existing resource based on the provided keyword arguments. All updates are optional and are applied only if the corresponding argument is given.
 
         Args:
             agent_id (Union[str, UUID]): The identifier of the agent, either as a string or a UUID object.
             about (Optional[str], optional): A brief description of the agent. Defaults to None.
-            instructions (Optional[Union[List[str], List[InstructionDict]]], optional): A list of instructions or instruction dictionaries to update the agent with. Defaults to None.
+            instructions (Optional[List[str]], optional): A list of instructions or instruction dictionaries to update the agent with. Defaults to None.
             name (Optional[str], optional): The new name to assign to the agent. Defaults to None.
             model (Optional[str], optional): The model identifier to associate with the agent. Defaults to None.
             default_settings (Optional[DefaultSettingsDict], optional): A dictionary of default settings to apply to the agent. Defaults to None.
+            metadata (Dict[str, Any])
+            overwrite (bool, optional): Whether to overwrite the existing agent settings. Defaults to False.
 
         Returns:
             ResourceUpdatedResponse: An object representing the response to the update request.
 
         Note:
             This method is decorated with `beartype`, which means it enforces type annotations at runtime.
         """
+
         result = self._update(agent_id=agent_id, **kwargs)
         return result
 
 
 class AsyncAgentsManager(BaseAgentsManager):
     """
     A class for managing asynchronous agent operations.
@@ -507,53 +519,55 @@
 
         create:
             Creates a new agent with the provided specifications.
 
             Args:
                 name (str): The name of the agent to create.
                 about (str): A description of the agent.
-                instructions (Union[List[str], List[InstructionDict]]): The instructions for operating the agent.
+                instructions (List[str]): The instructions for operating the agent.
                 tools (List[ToolDict], optional): An optional list of tools for the agent.
                 functions (List[FunctionDefDict], optional): An optional list of functions the agent can perform.
                 default_settings (DefaultSettingsDict, optional): Optional default settings for the agent.
                 model (ModelName, optional): The model name to associate with the agent, defaults to 'julep-ai/samantha-1-turbo'.
                 docs (List[DocDict], optional): An optional list of documents associated with the agent.
+                metadata (Dict[str, Any])
 
             Returns:
                 ResourceCreatedResponse: A response indicating the agent was created successfully.
 
         list:
-            Lists agents with optional pagination.
+            Asynchronously lists agents with optional pagination and returns an awaitable object.
 
             Args:
                 limit (Optional[int], optional): The maximum number of agents to retrieve.
                 offset (Optional[int], optional): The number of agents to skip before starting to collect the results.
 
             Returns:
                 List[Agent]: A list of agents.
 
         delete:
-            Deletes an agent by its ID.
+            Asynchronously deletes an agent by its ID and returns an awaitable object.
 
             Args:
                 agent_id (Union[str, UUID]): The unique identifier of the agent to delete.
 
             Returns:
                 The response from the delete operation (specific return type may vary).
 
         update:
-            Updates the specified fields of an agent by its ID.
+            Asynchronously updates the specified fields of an agent by its ID and returns an awaitable object.
 
             Args:
                 agent_id (Union[str, UUID]): The unique identifier of the agent to update.
                 about (Optional[str], optional): An optional new description for the agent.
-                instructions (Optional[Union[List[str], List[InstructionDict]]], optional): Optional new instructions for the agent.
+                instructions (Optional[List[str]], optional): Optional new instructions for the agent.
                 name (Optional[str], optional): An optional new name for the agent.
                 model (Optional[str], optional): Optional new model associated with the agent.
                 default_settings (Optional[DefaultSettingsDict], optional): Optional new default settings for the agent.
+                metadata (Dict[str, Any])
 
             Returns:
                 ResourceUpdatedResponse: A response indicating the agent was updated successfully.
     """
 
     @beartype
     async def get(self, id: Union[UUID, str]) -> Agent:
@@ -581,20 +595,21 @@
         Create a new resource asynchronously with specified details.
 
         This function is decorated with `beartype` to ensure that arguments conform to specified types.
 
         Args:
             name (str): The name of the resource to create.
             about (str): Information or description about the resource.
-            instructions (Union[List[str], List[InstructionDict]]): A list of strings or dictionaries detailing the instructions for the resource.
+            instructions (List[str]): A list of strings or dictionaries detailing the instructions for the resource.
             tools (List[ToolDict], optional): A list of dictionaries representing the tools associated with the resource. Defaults to an empty list.
             functions (List[FunctionDefDict], optional): A list of dictionaries defining functions that can be performed with the resource. Defaults to an empty list.
             default_settings (DefaultSettingsDict, optional): A dictionary with default settings for the resource. Defaults to an empty dictionary.
             model (ModelName, optional): The model identifier to use for the resource. Defaults to 'julep-ai/samantha-1-turbo'.
             docs (List[DocDict], optional): A list of dictionaries containing documentation for the resource. Defaults to an empty list.
+            metadata (Dict[str, Any])
 
         Returns:
             Agent: An instance of the Agent with the specified details
 
         Raises:
             The exceptions that may be raised are not specified in the signature and depend on the implementation of the _create method.
         """
@@ -656,17 +671,19 @@
         Asynchronously update an agent's details.
 
         This function is decorated with `beartype` to enforce the type checking of parameters. It updates the properties of the agent identified by `agent_id`.
 
         Args:
             agent_id (Union[str, UUID]): Unique identifier for the agent. It can be a string or a UUID object.
             about (Optional[str]): Additional information about the agent. Default is None.
-            instructions (Optional[Union[List[str], List[InstructionDict]]]): A list of instructions or instruction dictionaries. Default is None.
+            instructions (Optional[List[str]]): A list of instructions or instruction dictionaries. Default is None.
             name (Optional[str]): The name of the agent. Default is None.
             model (Optional[str]): The model identifier or name. Default is None.
             default_settings (Optional[DefaultSettingsDict]): Dictionary with default settings for the agent. Default is None.
+            metadata (Dict[str, Any])
+            overwrite (bool): Whether to overwrite the existing agent settings. Default is False.
 
         Returns:
             ResourceUpdatedResponse: An object containing the details of the update response.
         """
         result = await self._update(agent_id=agent_id, **kwargs)
         return result
```

### Comparing `julep-0.2.9/julep/managers/doc.py` & `julep-0.3.0/julep/managers/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 from beartype import beartype
 from beartype.typing import Any, Awaitable, Dict, List, Union
 
 from ..api.types import (
     CreateDoc,
     Doc,
     ResourceCreatedResponse,
+    ResourceDeletedResponse,
     GetAgentDocsResponse,
 )
 
 from .utils import rewrap_in_class
 
 from .base import BaseManager
 from .utils import is_valid_uuid4
 from .types import DocDict
 
 
 class DocsCreateArgs(TypedDict):
     agent_id: Optional[Union[str, UUID]]
     user_id: Optional[Union[str, UUID]]
     doc: DocDict
+    metadata: Dict[str, Any] = {}
 
 
 class BaseDocsManager(BaseManager):
     """
-    Manages documents for agents or users by providing methods to get, create, and delete docsrmation.
+    Manages documents for agents or users by providing internal methods to list, create, and delete documents.
 
     The class utilizes an API client to interact with a back-end service that handles the document management operations.
 
     Typical usage example:
 
         docs_manager = BaseDocsManager(api_client)
         agent_docs = docs_manager._list(agent_id="some-agent-uuid")
@@ -74,14 +76,15 @@
         assert an error.
 
         Args:
             agent_id (Optional[Union[str, UUID]]): The UUID v4 of the agent for whom docs is requested, exclusive with `user_id`.
             user_id (Optional[Union[str, UUID]]): The UUID v4 of the user for whom docs is requested, exclusive with `agent_id`.
             limit (Optional[int]): The maximum number of records to return. Defaults to None.
             offset (Optional[int]): The number of records to skip before starting to collect the response set. Defaults to None.
+            metadata_filter (Dict[str, Any]): A dictionary used for filtering documents based on metadata criteria. Defaults to an empty dictionary.
 
         Returns:
             Union[GetAgentDocsResponse, Awaitable[GetAgentDocsResponse]]: The response object containing docsrmation about the agent or user, or a promise of such an object if the call is asynchronous.
 
         Raises:
             AssertionError: If both `agent_id` and `user_id` are provided or neither is provided, or if the provided IDs are not valid UUID v4.
         """
@@ -110,25 +113,27 @@
             )
 
     def _create(
         self,
         doc: DocDict,
         agent_id: Optional[Union[str, UUID]] = None,
         user_id: Optional[Union[str, UUID]] = None,
+        metadata: Dict[str, Any] = {},
     ) -> Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]:
         """
         Create a new resource with docsrmation for either an agent or a user, but not both.
 
             This function asserts that exactly one of `agent_id` or `user_id` is provided and is a valid UUID v4.
             It then creates the appropriate docsrmation based on which ID was provided.
 
             Args:
                 agent_id (Optional[Union[str, UUID]]): The UUID of the agent or None.
                 user_id (Optional[Union[str, UUID]]): The UUID of the user or None.
                 doc (DocDict): A dictionary containing the document data for the resource being created.
+                metadata (Dict[str, Any]): Optional metadata for the document. Defaults to an empty dictionary.
 
             Returns:
                 Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]: The response after creating the resource, which could be immediate or an awaitable for asynchronous execution.
 
             Raises:
                 AssertionError: If both `agent_id` and `user_id` are provided, neither are provided, or if the provided IDs are not valid UUID v4 strings.
 
@@ -157,36 +162,38 @@
             )
 
     def _delete(
         self,
         agent_id: Optional[Union[str, UUID]],
         user_id: Optional[Union[str, UUID]],
         doc_id: Union[str, UUID],
-    ):
+    ) -> Union[ResourceDeletedResponse, Awaitable[ResourceDeletedResponse]]:
         """
         Delete docs based on either an agent_id or a user_id.
 
             This method selects the appropriate deletion operation (agent or user) based on whether an `agent_id` or `user_id` is provided. Only one of these ID types should be valid and provided.
 
             Args:
                 agent_id (Optional[Union[str, UUID]]): A unique identifier of an agent. Either a string or UUID v4, but not both `agent_id` and `user_id`.
                 user_id (Optional[Union[str, UUID]]): A unique identifier of a user. Either a string or UUID v4, but not both `agent_id` and `user_id`.
                 doc_id (Union[str, UUID]): A unique identifier for docsrmation to be deleted, as a string or UUID v4.
 
             Returns:
                 The result of the API deletion request. This can be the response object from the client's delete operation.
 
             Raises:
-                AssertionError: If neither `agent_id` nor `user_id` is valid, if both are provided simultaneously, or if negation logic for valid UUIDs fails.
+                AssertionError: If both `agent_id` and `user_id` are provided, neither are provided, or if the provided IDs are not valid UUID v4 strings.
                 Other exceptions related to the `api_client` operations could potentially be raised and depend on its implementation.
         """
-        assert (
-            (agent_id and is_valid_uuid4(agent_id))
-            or (user_id and is_valid_uuid4(user_id))
-            and not (agent_id and user_id)
+        assert bool(agent_id) ^ bool(
+            user_id
+        ), "One and only one of user_id or agent_id must be given."
+
+        assert (agent_id and is_valid_uuid4(agent_id)) or (
+            user_id and is_valid_uuid4(user_id)
         ), "One and only one of user_id or agent_id must be given and must be valid UUID v4"
 
         if agent_id is not None:
             return self.api_client.delete_agent_doc(
                 agent_id=agent_id,
                 doc_id=doc_id,
             )
@@ -453,12 +460,17 @@
 
         Returns:
             Coroutine[Any]: A coroutine that, when awaited, returns the result of the document deletion process.
 
         Note:
             The `@beartype` decorator is used to enforce type checking on the function arguments.
         """
+
+        # Assert either user_id or agent_id is provided
+        if not agent_id and not user_id:
+            raise ValueError("Either agent_id or user_id must be provided.")
+
         return await self._delete(
             agent_id=agent_id,
             user_id=user_id,
             doc_id=doc_id,
         )
```

### Comparing `julep-0.2.9/julep/managers/memory.py` & `julep-0.3.0/julep/managers/memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from .utils import is_valid_uuid4
 
 
 class BaseMemoriesManager(BaseManager):
     """
     A base manager class for handling agent memories.
 
-        This manager provides an interface to interact with agent memories, allowing
-        for listing and other operations to manage an agent's memories.
+        This manager provides an interface to interact with agent memories, facilitating
+        operations such as listing and retrieving memories based on various criteria.
 
         Methods:
             _list(agent_id, query, types=None, user_id=None, limit=None, offset=None):
                 Retrieves a list of memories for a given agent.
 
         Args:
             agent_id (str): A valid UUID v4 string identifying the agent.
@@ -67,27 +67,26 @@
             AssertionError: If `agent_id` is not a valid UUID v4.
         """
         assert is_valid_uuid4(agent_id), "agent_id must be a valid UUID v4"
 
         return self.api_client.get_agent_memories(
             agent_id=agent_id,
             query=query,
-            types=types,
             user_id=user_id,
             limit=limit,
             offset=offset,
         )
 
 
 class MemoriesManager(BaseMemoriesManager):
     """
     A class for managing memory entities associated with agents.
 
-        This class inherits from `BaseMemoriesManager` and provides
-        an interface to list memory entities for a given agent.
+        Inherits from `BaseMemoriesManager` and extends its functionality to specifically
+        manage and retrieve memory entities for agents based on query parameters.
 
         Attributes:
             Inherited from `BaseMemoriesManager`.
 
         Methods:
             list: Retrieves a list of memory entities based on query parameters.
     """
```

### Comparing `julep-0.2.9/julep/managers/session.py` & `julep-0.3.0/julep/managers/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,25 @@
     ToolDict,
 )
 
 from .utils import is_valid_uuid4
 
 
 class SessionCreateArgs(TypedDict):
-    user_id: Union[str, UUID]
+    user_id: Optional[Union[str, UUID]]
     agent_id: Union[str, UUID]
-    situation: Optional[str]
+    situation: Optional[str] = None
+    metadata: Dict[str, Any] = {}
 
 
 class SessionUpdateArgs(TypedDict):
     session_id: Union[str, UUID]
-    situation: str
+    situation: Optional[str] = None
+    metadata: Optional[Dict[str, Any]] = None
+    overwrite: bool = False
 
 
 class BaseSessionsManager(BaseManager):
     """
     A class to manage sessions using base API client methods.
 
     This manager handles CRUD operations and additional actions on the session data,
@@ -61,20 +64,24 @@
 
             Args:
                 id (Union[str, UUID]): The unique identifier for the session.
 
             Returns:
                 Union[Session, Awaitable[Session]]: The session object or an awaitable yielding it.
 
+            Raises:
+                ValueError: If the `id` is not a valid UUID.
+                NetworkError: If there is an issue communicating with the API.
+
         _create(user_id, agent_id, situation):
             Create a new session with specified user and agent identifiers.
 
             Args:
-                user_id (Union[str, UUID]): The unique identifier for the user.
                 agent_id (Union[str, UUID]): The unique identifier for the agent.
+                user_id (Optional[Union[str, UUID]]): The unique identifier for the user.
                 situation (Optional[str]): An optional description of the situation for the session.
 
             Returns:
                 Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]: The response for the created session or an awaitable yielding it.
 
         _list_items(limit, offset):
             List multiple session items with optional pagination.
@@ -135,14 +142,23 @@
             Args:
                 session_id (Union[str, UUID]): The unique identifier for the session.
                 limit (Optional[int]): The limit on the number of history entries to be retrieved.
                 offset (Optional[int]): The number of history entries to be skipped before starting to collect the result set.
 
             Returns:
                 Union[GetHistoryResponse, Awaitable[GetHistoryResponse]]: The history response for the session or an awaitable yielding it.
+
+        _delete_history(session_id):
+            Delete the history of a session.
+
+            Args:
+                session_id (Union[str, UUID]): The unique identifier for the session.
+
+            Returns:
+                Union[None, Awaitable[None]]: None or an awaitable yielding None if the operation is successful.
     """
 
     def _get(self, id: Union[str, UUID]) -> Union[Session, Awaitable[Session]]:
         """
         Get a session by its ID.
 
         Args:
@@ -155,43 +171,47 @@
             AssertionError: If the id is not a valid UUID v4.
         """
         assert is_valid_uuid4(id), "id must be a valid UUID v4"
         return self.api_client.get_session(session_id=id)
 
     def _create(
         self,
-        user_id: Union[str, UUID],
         agent_id: Union[str, UUID],
+        user_id: Optional[Union[str, UUID]] = None,
         situation: Optional[str] = None,
+        metadata: Dict[str, Any] = {},
     ) -> Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]:
         # Cast instructions to a list of Instruction objects
         """
         Creates a session for a specified user and agent.
 
         This internal method is responsible for creating a session using the API client. It validates that both the user and agent IDs are valid UUID v4 strings before proceeding with session creation.
 
         Args:
-            user_id (Union[str, UUID]): The user's identifier which could be a string or a UUID object.
             agent_id (Union[str, UUID]): The agent's identifier which could be a string or a UUID object.
+            user_id (Optional[Union[str, UUID]]): The user's identifier which could be a string or a UUID object.
             situation (Optional[str], optional): An optional description of the situation.
+            metadata (Dict[str, Any])
 
         Returns:
             Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]: The response from the API client upon successful session creation, which can be a synchronous `ResourceCreatedResponse` or an asynchronous `Awaitable` of it.
 
         Raises:
             AssertionError: If either `user_id` or `agent_id` is not a valid UUID v4.
         """
-        assert is_valid_uuid4(user_id) and is_valid_uuid4(
-            agent_id
-        ), "id must be a valid UUID v4"
+        assert is_valid_uuid4(agent_id), "agent_id must be a valid UUID v4"
+
+        if user_id is not None:
+            assert is_valid_uuid4(user_id), "user_id must be a valid UUID v4"
 
         return self.api_client.create_session(
             user_id=user_id,
             agent_id=agent_id,
             situation=situation,
+            metadata=metadata,
         )
 
     def _list_items(
         self,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         metadata_filter: str = "{}",
@@ -235,34 +255,43 @@
         """
         assert is_valid_uuid4(session_id), "id must be a valid UUID v4"
         return self.api_client.delete_session(session_id=session_id)
 
     def _update(
         self,
         session_id: Union[str, UUID],
-        situation: str,
+        situation: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+        overwrite: bool = False,
     ) -> Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]:
         """
         Update a session with a given situation.
 
         Args:
             session_id (Union[str, UUID]): The session identifier, which can be a string-formatted UUID or an actual UUID object.
             situation (str): A string describing the current situation.
-
+            overwrite (bool, optional): Whether to overwrite the existing situation. Defaults to False.
         Returns:
             Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]: The response from the update operation, which can be either synchronous or asynchronous.
 
         Raises:
             AssertionError: If `session_id` is not a valid UUID v4.
         """
         assert is_valid_uuid4(session_id), "id must be a valid UUID v4"
 
-        return self.api_client.update_session(
+        updateFn = (
+            self.api_client.update_session
+            if overwrite
+            else self.api_client.patch_session
+        )
+
+        return updateFn(
             session_id=session_id,
             situation=situation,
+            metadata=metadata,
         )
 
     def _chat(
         self,
         *,
         session_id: str,
         messages: List[Union[InputChatMlMessageDict, InputChatMlMessage]],
@@ -385,14 +414,35 @@
         """
         return self.api_client.get_history(
             session_id=session_id,
             limit=limit,
             offset=offset,
         )
 
+    def _delete_history(
+        self,
+        session_id: Union[str, UUID],
+    ) -> Union[None, Awaitable[None]]:
+        """
+        Delete the history of a session.
+
+        Args:
+            session_id (Union[str, UUID]): The unique identifier for the session.
+
+        Returns:
+            Union[None, Awaitable[None]]: The result of the delete operation, which can be either
+            None or an Awaitable that resolves to None, depending on whether this is a synchronous
+            or asynchronous call.
+
+        Raises:
+            AssertionError: If the `session_id` is not a valid UUID v4.
+        """
+        assert is_valid_uuid4(session_id), "id must be a valid UUID v4"
+        return self.api_client.delete_session_history(session_id=session_id)
+
 
 class SessionsManager(BaseSessionsManager):
     """
     A class responsible for managing session interactions.
 
     This class extends `BaseSessionsManager` and provides methods to get, create,
     list, delete, and update sessions, as well as to initiate a chat within a session,
@@ -449,14 +499,16 @@
             session_id: Union[str, UUID],
             limit: Optional[int]=None,
             offset: Optional[int]=None
         ) -> List[ChatMlMessage]:
             Retrieves the chat history for a given session, supported by
             optional pagination parameters.
 
+        delete_history (session_id: Union[str, UUID]) -> None:
+
     Each method is decorated with `@beartype` for runtime type enforcement.
     """
 
     @beartype
     def get(self, id: Union[str, UUID]) -> Session:
         """
         Retrieve a Session object based on a given identifier.
@@ -554,14 +606,15 @@
         is either a string or a UUID and that the `situation` parameter is a string. It delegates
         the actual update process to an internal method '_update'.
 
         Args:
             session_id (Union[str, UUID]): The session identifier, which can be a UUID or a
                 string that uniquely identifies the session.
             situation (str): A string that represents the new situation for the resource update.
+            overwrite (bool, optional): A flag to indicate whether to overwrite the existing
 
         Returns:
             Session: The updated Session object.
 
         Note:
             The `@beartype` decorator is used for runtime type checking of the function arguments.
         """
@@ -700,14 +753,30 @@
         """
         return self._history(
             session_id=session_id,
             limit=limit,
             offset=offset,
         ).items
 
+    @beartype
+    def delete_history(self, session_id: Union[str, UUID]) -> None:
+        """
+        Delete the history of a session.
+
+        Args:
+            session_id (Union[str, UUID]): The unique identifier for the session.
+
+        Returns:
+            None: The result of the delete operation.
+
+        Raises:
+            AssertionError: If the `session_id` is not a valid UUID v4.
+        """
+        return self._delete_history(session_id=session_id)
+
 
 class AsyncSessionsManager(BaseSessionsManager):
     """
     A class for managing asynchronous sessions.
 
     This class handles operations related to creating, retrieving, updating,
     deleting, and interacting with sessions asynchronously. It extends the
@@ -737,14 +806,16 @@
 
         async suggestions(*, session_id: Union[str, UUID], limit: Optional[int]=None, offset: Optional[int]=None) -> List[Suggestion]:
             Retrieves suggestions related to a session optionally limited and paginated.
 
         async history(*, session_id: Union[str, UUID], limit: Optional[int]=None, offset: Optional[int]=None) -> List[ChatMlMessage]:
             Retrieves the history of messages in a session, optionally limited and paginated.
 
+        async delete_history(session_id: Union[str, UUID]) -> None:
+
     Note:
         The `@beartype` decorator is used for runtime type checking of the arguments.
 
     Additional methods may be provided by the BaseSessionsManager.
     """
 
     @beartype
@@ -1018,7 +1089,23 @@
         return (
             await self._history(
                 session_id=session_id,
                 limit=limit,
                 offset=offset,
             )
         ).items
+
+    @beartype
+    async def delete_history(self, session_id: Union[str, UUID]) -> None:
+        """
+        Delete the history of a session asynchronously.
+
+        Args:
+            session_id (Union[str, UUID]): The unique identifier for the session.
+
+        Returns:
+            None: The result of the delete operation.
+
+        Raises:
+            AssertionError: If the `session_id` is not a valid UUID v4.
+        """
+        return await self._delete_history(session_id=session_id)
```

### Comparing `julep-0.2.9/julep/managers/tool.py` & `julep-0.3.0/julep/managers/tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,51 +2,48 @@
 
 from typing import Optional
 from beartype import beartype
 from beartype.typing import Awaitable, List, Union
 
 from ..api.types import (
     ResourceCreatedResponse,
+    ResourceDeletedResponse,
     FunctionDef,
     GetAgentToolsResponse,
     CreateToolRequest,
     ResourceUpdatedResponse,
     Tool,
 )
 
 from .base import BaseManager
 from .utils import is_valid_uuid4
 from .types import ToolDict, FunctionDefDict
 
 
 class BaseToolsManager(BaseManager):
     """
-    A class to manage base tools by interacting with an API client.
+    A class to manage tools by interacting with an API client.
 
-    This class provides an interface for creating, reading, updating, and deleting tools, where each tool is associated with an agent.
+    This class provides methods for creating, reading, updating, and deleting tools associated with agents. It ensures the validity of UUIDs for agent_id and tool_id where applicable and handles both synchronous and asynchronous operations.
 
     Attributes:
-        api_client: The API client utilized to send requests to the service.
+        api_client: The API client used to send requests to the service.
 
     Methods:
         _get(self, agent_id: Union[str, UUID], limit: Optional[int]=None, offset: Optional[int]=None) -> Union[GetAgentToolsResponse, Awaitable[GetAgentToolsResponse]]:
-            Retrieve a list of tools associated with the given agent using the API client.
+            Retrieves a list of tools associated with the specified agent. Supports pagination through limit and offset parameters.
 
         _create(self, agent_id: Union[str, UUID], tool: ToolDict) -> Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]:
-            Create a new tool associated with the given agent using the API client.
+            Creates a new tool associated with the specified agent.
 
         _update(self, agent_id: Union[str, UUID], tool_id: Union[str, UUID], function: FunctionDefDict) -> Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]:
-            Update the definition of an existing tool associated with the given agent using the API client.
+            Updates the definition of an existing tool associated with the specified agent.
 
         _delete(self, agent_id: Union[str, UUID], tool_id: Union[str, UUID]):
-            Delete a tool associated with the given agent using the API client.
-
-    Note:
-        All methods assert the validity of UUIDs for agent_id and tool_id when applicable.
-        The _get, _create, and _update methods may return either synchronous or asynchronous responses, indicated by the return type Union[..., Awaitable[...]].
+            Deletes a tool associated with the specified agent.
     """
 
     def _get(
         self,
         agent_id: Union[str, UUID],
         limit: Optional[int] = None,
         offset: Optional[int] = None,
@@ -103,46 +100,54 @@
         )
 
     def _update(
         self,
         agent_id: Union[str, UUID],
         tool_id: Union[str, UUID],
         function: FunctionDefDict,
+        overwrite: bool = False,
     ) -> Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]:
         """
         Update the tool definition for a given agent.
 
             Args:
                 agent_id (Union[str, UUID]): The unique identifier for the agent, either in string or UUID format.
                 tool_id (Union[str, UUID]): The unique identifier for the tool, either in string or UUID format.
                 function (FunctionDefDict): A dictionary containing the function definition that conforms with the required API schema.
+                overwrite (bool): A flag to indicate whether to overwrite the existing function definition. Defaults to False.
 
             Returns:
                 Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]: The updated resource response sync or async.
 
             Raises:
                 AssertionError: If the `agent_id` or `tool_id` is not a valid UUID v4.
         """
         assert is_valid_uuid4(agent_id) and is_valid_uuid4(
             tool_id
         ), "agent_id and tool_id must be a valid UUID v4"
 
         function: FunctionDef = FunctionDef(**function)
 
-        return self.api_client.update_agent_tool(
+        updateFn = (
+            self.api_client.update_agent_tool
+            if overwrite
+            else self.api_client.patch_agent_tool
+        )
+
+        return updateFn(
             agent_id=agent_id,
             tool_id=tool_id,
             function=function,
         )
 
     def _delete(
         self,
         agent_id: Union[str, UUID],
         tool_id: Union[str, UUID],
-    ):
+    ) -> Union[ResourceDeletedResponse, Awaitable[ResourceDeletedResponse]]:
         """
         Delete a tool associated with an agent.
 
             Args:
                 agent_id (Union[str, UUID]): The UUID of the agent.
                 tool_id (Union[str, UUID]): The UUID of the tool to be deleted.
 
@@ -310,22 +315,24 @@
     @beartype
     def update(
         self,
         *,
         agent_id: Union[str, UUID],
         tool_id: Union[str, UUID],
         function: FunctionDefDict,
+        overwrite: bool = False,
     ) -> ResourceUpdatedResponse:
         """
         Update a specific tool definition for an agent.
 
         Args:
             agent_id (Union[str, UUID]): The unique identifier of the agent.
             tool_id (Union[str, UUID]): The unique identifier of the tool to be updated.
             function (FunctionDefDict): A dictionary containing the new definition of the tool.
+            overwrite (bool): A flag indicating whether to overwrite the existing definition.
 
         Returns:
             ResourceUpdatedResponse: An object representing the update operation response.
 
         Note:
             This function is decorated with `beartype` which ensures that the arguments provided
             match the expected types at runtime.
@@ -334,14 +341,15 @@
             BeartypeDecorHintPepParamException: If the type of any parameter does not match the expected type.
             Any exceptions that `self._update` method might raise.
         """
         return self._update(
             agent_id=agent_id,
             tool_id=tool_id,
             function=function,
+            overwrite=overwrite,
         )
 
 
 class AsyncToolsManager(BaseToolsManager):
     """
     A manager for asynchronous tools handling.
 
@@ -421,15 +429,15 @@
 
     @beartype
     async def delete(
         self,
         *,
         agent_id: Union[str, UUID],
         tool_id: Union[str, UUID],
-    ):
+    ) -> Awaitable[ResourceDeletedResponse]:
         """
         Asynchronously delete a specified agent-tool association.
 
             This function is a high-level asynchronous API that delegates to a
             private coroutinal method `_delete` to perform the actual deletion based on
             the provided `agent_id` and `tool_id`.
```

### Comparing `julep-0.2.9/julep/managers/user.py` & `julep-0.3.0/julep/managers/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 from uuid import UUID
 from typing import Optional, TypedDict
-
 from beartype import beartype
 from beartype.typing import Any, Awaitable, Dict, List, Union
 
-from .utils import rewrap_in_class
+from .utils import rewrap_in_class, NotSet
 
 from ..api.types import (
     User,
     CreateDoc,
     ResourceCreatedResponse,
     ResourceUpdatedResponse,
     ListUsersResponse,
@@ -19,20 +18,23 @@
 from .utils import is_valid_uuid4
 from .types import DocDict
 
 
 class UserCreateArgs(TypedDict):
     name: str
     about: str
-    docs: List[str]
+    docs: List[str] = []
+    metadata: Dict[str, Any] = {}
 
 
 class UserUpdateArgs(TypedDict):
-    about: Optional[str] = None
     name: Optional[str] = None
+    metadata: Optional[Dict[str, Any]] = None
+    about: Optional[str] = None
+    overwrite: bool = False
 
 
 class BaseUsersManager(BaseManager):
     """
     A manager class for handling user-related operations through an API client.
 
         This class provides high-level methods to interact with user records,
@@ -75,26 +77,28 @@
         return self.api_client.get_user(user_id=id)
 
     def _create(
         self,
         name: str,
         about: str,
         docs: List[DocDict] = [],
+        metadata: Dict[str, Any] = {},
     ) -> Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]:
         # Cast docs to a list of CreateDoc objects
         """
         Create a new resource with the given name and about information, optionally including additional docs.
 
         This internal method allows for creating a new resource with optional docsrmation.
 
         Args:
             name (str): The name of the new resource.
             about (str): A brief description about the new resource.
             docs (List[DocDict], optional): A list of dictionaries with documentation-related information. Each dictionary
                 must conform to the structure expected by CreateDoc. Defaults to an empty list.
+            metadata (Dict[str, Any])
 
         Returns:
             Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]: The response indicating the resource has been
             created successfully. It can be either a synchronous ResourceCreatedResponse or an asynchronous Awaitable object
             containing a ResourceCreatedResponse.
 
         Note:
@@ -107,14 +111,15 @@
         """
         docs: List[CreateDoc] = [CreateDoc(**doc) for doc in docs]
 
         return self.api_client.create_user(
             name=name,
             about=about,
             docs=docs,
+            metadata=metadata,
         )
 
     def _list_items(
         self,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         metadata_filter: str = "{}",
@@ -152,40 +157,57 @@
         """
         assert is_valid_uuid4(user_id), "id must be a valid UUID v4"
         return self.api_client.delete_user(user_id=user_id)
 
     def _update(
         self,
         user_id: Union[str, UUID],
-        about: Optional[str] = None,
-        name: Optional[str] = None,
+        about: Optional[str] = NotSet,
+        name: Optional[str] = NotSet,
+        metadata: Dict[str, Any] = NotSet,
+        overwrite: bool = False,
     ) -> Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]:
         """
         Update user details for a given user ID.
 
         This method updates the 'about' and/or 'name' fields for the user identified by user_id.
 
         Args:
             user_id (Union[str, UUID]): The ID of the user to be updated. Must be a valid UUID v4.
             about (Optional[str], optional): The new information about the user. Defaults to None.
             name (Optional[str], optional): The new name for the user. Defaults to None.
+            metadata (Dict[str, Any])
+            overwrite (bool, optional): Whether to overwrite the existing user data. Defaults to False.
 
         Returns:
             Union[ResourceUpdatedResponse, Awaitable[ResourceUpdatedResponse]]: The response indicating successful update or an Awaitable that resolves to such a response.
 
         Raises:
             AssertionError: If `user_id` is not a valid UUID v4.
         """
         assert is_valid_uuid4(user_id), "id must be a valid UUID v4"
-        return self.api_client.update_user(
+
+        updateFn = (
+            self.api_client.update_user if overwrite else self.api_client.patch_user
+        )
+
+        update_data = dict(
             user_id=user_id,
             about=about,
             name=name,
+            metadata=metadata,
         )
 
+        update_data = {k: v for k, v in update_data.items() if v is not NotSet}
+
+        if not update_data:
+            raise ValueError("No fields to update")
+
+        return updateFn(**update_data)
+
 
 class UsersManager(BaseUsersManager):
     """
     A class responsible for managing users in a system.
 
     This class is a specialized version of the BaseUsersManager and provides
     methods for retrieving, creating, listing, deleting, and updating users within
@@ -285,15 +307,14 @@
             offset=offset,
             metadata_filter=metadata_filter_string,
         ).items
 
     @beartype
     def delete(
         self,
-        *,
         user_id: Union[str, UUID],
     ) -> None:
         """
         Deletes a user based on the provided user ID.
 
         Args:
             user_id (Union[str, UUID]): Unique identifier of the user.
@@ -321,14 +342,15 @@
 
         This method updates user details such as the `about` text and user's `name` for a given `user_id`.
 
         Args:
             user_id (Union[str, UUID]): The unique identifier for the user, which can be a string or a UUID object.
             about(Optional[str], optional): The descriptive information about the user. Defaults to None, indicating that `about` should not be updated if not provided.
             name(Optional[str], optional): The name of the user. Defaults to None, indicating that `name` should not be updated if not provided.
+            overwrite(bool, optional): Whether to overwrite the existing user data. Defaults to False.
 
         Returns:
             ResourceUpdatedResponse: An object indicating the outcome of the update operation, which typically includes the status of the operation and possibly the updated resource data.
         """
         result = self._update(user_id=user_id, **kwargs)
         return result
 
@@ -435,15 +457,14 @@
                 metadata_filter=metadata_filter_string,
             )
         ).items
 
     @beartype
     async def delete(
         self,
-        *,
         user_id: Union[str, UUID],
     ) -> None:
         """
         Asynchronously deletes a user by their user ID.
 
         Args:
             user_id (Union[str, UUID]): The unique identifier of the user to delete, which can be a string or a UUID.
```

### Comparing `julep-0.2.9/julep/utils/openai_patch.py` & `julep-0.3.0/julep/utils/openai_patch.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,25 @@
     completion_create_params,
 )
 
 from openai._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 
 
 def patch_completions_acreate(client: OpenAI):
+    """
+    Asynchronously patches the `completions.create` method of the OpenAI client.
+
+    This function replaces the original `completions.create` method with a custom asynchronous version that allows for additional parameters and custom behavior.
+
+    Parameters:
+    - client (OpenAI): The OpenAI client instance to be patched.
+
+    Returns:
+    - OpenAI: The patched OpenAI client instance with the modified `completions.create` method.
+    """
     original_completions_create = client.completions.create
 
     async def completions_create(
         *,
         model: Union[
             str, Literal["gpt-3.5-turbo-instruct", "davinci-002", "babbage-002"]
         ] = "julep-ai/samantha-1-turbo",
@@ -78,14 +89,25 @@
 
     client.completions.create = completions_create
 
     return client
 
 
 def patch_chat_acreate(client: OpenAI):
+    """
+    Asynchronously patches the `chat.completions.create` method of the OpenAI client.
+
+    This function updates the `chat.completions.create` method to an asynchronous version, enabling the inclusion of additional parameters and adjustments to its behavior.
+
+    Parameters:
+    - client (OpenAI): The OpenAI client instance to be patched.
+
+    Returns:
+    - OpenAI: The patched OpenAI client instance with the updated `chat.completions.create` method.
+    """
     original_chat_create = client.chat.completions.create
 
     async def chat_create(
         *,
         messages: Iterable[ChatCompletionMessageParam],
         model: Union[
             str,
@@ -167,14 +189,25 @@
 
     client.chat.completions.create = chat_create
 
     return client
 
 
 def patch_completions_create(client: OpenAI):
+    """
+    Patches the `completions.create` method (non-async version) of the OpenAI client.
+
+    This function replaces the original `completions.create` method with a custom version that supports additional parameters and custom behavior, without changing it to an asynchronous function.
+
+    Parameters:
+    - client (OpenAI): The OpenAI client instance to be patched.
+
+    Returns:
+    - OpenAI: The patched OpenAI client instance with the modified `completions.create` method.
+    """
     original_completions_create = client.completions.create
 
     def completions_create(
         *,
         model: Union[
             str, Literal["gpt-3.5-turbo-instruct", "davinci-002", "babbage-002"]
         ] = "julep-ai/samantha-1-turbo",
```

### Comparing `julep-0.2.9/pyproject.toml` & `julep-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "julep"
-version = "0.2.9"
+version = "0.3.0"
 description = "Julep is a platform for creating agents with long-term memory"
 authors = ["Julep Developers <developers@julep.ai>"]
 license = "ISC"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.14"
@@ -13,32 +13,32 @@
 environs = ">=9.0.0,<11.0.0"
 beartype = ">=0.14.0,<1.0.0"
 openai = ">=1.0.1,<2.0.0"
 typing-extensions = ">=4.0.0,<5.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
-pytype = "^2024.1.5"
-black = "^23.12.1"
+pytype = "2024.1.5"
+black = "^24.4.0"
 ward = "^0.68.0b0"
 ruff = "^0.1.13"
-poethepoet = "^0.24.4"
+poethepoet = "^0.25.1"
 ipython = "<8.13"
 pyright = "^1.1.348"
 handsdown = "^2.1.0"
 jupyterlab = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks]
 format = "black ."
-lint = "ruff **/*.py --fix --unsafe-fixes"
-typecheck = "pytype --config=pytype.toml julep"
+lint = "ruff julep/**/*.py tests/**/*.py --fix --unsafe-fixes"
+typecheck = "pytype --config=pytype.toml"
 check = [
     "format",
     "lint",
     "typecheck",
 ]
 start_prism.shell = "prism mock ./tests/mock_openapi.yaml -p 8080 -v fatal 1> /dev/null &"
 kill_prism.shell = "kill $(pgrep -f 'prism .*')"
@@ -47,8 +47,8 @@
     "start_prism",
     { cmd = "echo 'Waiting for prism to start up'" },
     { cmd = "sleep 1" },
     { cmd = "ward" },
     "kill_prism",
 ]
 generate_docstrings = "gpt4docstrings -k $OPENAI_API_KEY -v 1 -w -p -s -n -C -e api/ -m gpt-4-1106-preview julep/"
-doc = "handsdown julep --exclude julep/api/core --exclude julep/api/types --exclude julep/api/environment.py --exclude julep/env.py --exclude julep/managers/base.py --exclude julep/managers/types.py --exclude julep/managers/utils.py --cleanup -n 'Julep Python SDK' --toc-depth 2 -o ../../gitbook/python-sdk-docs"
+doc = "handsdown julep --exclude julep/api/core --exclude julep/api/types --exclude julep/api/environment.py --exclude julep/env.py --exclude julep/managers/base.py --exclude julep/managers/types.py --exclude julep/managers/utils.py --cleanup -n 'Julep Python SDK' --toc-depth 2 -o ../../docs/python-sdk-docs"
```

### Comparing `julep-0.2.9/PKG-INFO` & `julep-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julep
-Version: 0.2.9
+Version: 0.3.0
 Summary: Julep is a platform for creating agents with long-term memory
 License: ISC
 Author: Julep Developers
 Author-email: developers@julep.ai
 Requires-Python: >=3.8,<3.14
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

