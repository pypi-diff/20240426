# Comparing `tmp/great_expectations_cloud-20240425.0.tar.gz` & `tmp/great_expectations_cloud-20240426.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240425.0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240426.0.tar", max compression
```

## Comparing `great_expectations_cloud-20240425.0.tar` & `great_expectations_cloud-20240426.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2084 2024-04-25 18:18:38.263824 great_expectations_cloud-20240425.0/LICENSE
--rw-r--r--   0        0        0     9269 2024-04-25 18:18:38.263824 great_expectations_cloud-20240425.0/README.md
--rw-r--r--   0        0        0      150 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      733 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     2993 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      739 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    16116 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0      362 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/agent_warnings.py
--rw-r--r--   0        0        0     2851 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4598 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0     1762 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     5395 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9457 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/pyproject.toml
--rw-r--r--   0        0        0    10598 1970-01-01 00:00:00.000000 great_expectations_cloud-20240425.0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-04-26 18:57:19.775872 great_expectations_cloud-20240426.0/LICENSE
+-rw-r--r--   0        0        0     9269 2024-04-26 18:57:19.775872 great_expectations_cloud-20240426.0/README.md
+-rw-r--r--   0        0        0      150 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     2993 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      739 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    17084 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0      362 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/agent_warnings.py
+-rw-r--r--   0        0        0     2851 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4598 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0     1762 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     5918 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9457 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/pyproject.toml
+-rw-r--r--   0        0        0    10598 1970-01-01 00:00:00.000000 great_expectations_cloud-20240426.0/PKG-INFO
```

### Comparing `great_expectations_cloud-20240425.0/LICENSE` & `great_expectations_cloud-20240426.0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/README.md` & `great_expectations_cloud-20240426.0/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/run_metric_list_action.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/unknown.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,14 +51,16 @@
     import requests
     from great_expectations.data_context import CloudDataContext
     from typing_extensions import Self
 
     from great_expectations_cloud.agent.actions.agent_action import ActionResult
 
 LOGGER: Final[logging.Logger] = logging.getLogger(__name__)
+# TODO Set in log dict
+LOGGER.setLevel(logging.INFO)
 HandlerMap = Dict[str, OnMessageCallback]
 
 
 class GXAgentConfig(AgentBaseModel):
     """GXAgent configuration.
     Attributes:
         queue: name of queue
@@ -197,14 +199,21 @@
 
         Args:
             event_context: event with related properties and actions.
         """
         # warning:  this method will not be executed in the main thread
         self._update_status(job_id=event_context.correlation_id, status=JobStarted())
         print(f"Starting job {event_context.event.type} ({event_context.correlation_id}) ")
+        LOGGER.info(
+            "Starting job",
+            extra={
+                "event_type": event_context.event.type,
+                "correlation_id": event_context.correlation_id,
+            },
+        )
         handler = EventHandler(context=self._context)
         # This method might raise an exception. Allow it and handle in _handle_event_as_thread_exit
         result = handler.handle_event(event=event_context.event, id=event_context.correlation_id)
         return result
 
     def _handle_event_as_thread_exit(
         self, future: Future[ActionResult], event_context: EventContext
@@ -224,28 +233,42 @@
 
             if result.type == UnknownEvent().type:
                 status = JobCompleted(
                     success=False,
                     created_resources=[],
                     error_stack_trace="The version of the GX Agent you are using does not support this functionality. Please upgrade to latest.",
                 )
-                print(
-                    f"Job completed with error: {event_context.event.type} ({event_context.correlation_id}). Ensure agent is up-to-date."
+                LOGGER.error(
+                    "Job completed with error. Ensure agent is up-to-date.",
+                    extra={
+                        "event_type": event_context.event.type,
+                        "id": event_context.correlation_id,
+                    },
                 )
             else:
                 status = JobCompleted(
                     success=True,
                     created_resources=result.created_resources,
                 )
-                print(f"Completed job: {event_context.event.type} ({event_context.correlation_id})")
+                LOGGER.info(
+                    "Completed job",
+                    extra={
+                        "event_type": event_context.event.type,
+                        "correlation_id": event_context.correlation_id,
+                    },
+                )
         else:
             status = build_failed_job_completed_status(error)
-            print(traceback.format_exc())
-            print(
-                f"Job completed with error: {event_context.event.type} ({event_context.correlation_id})"
+            LOGGER.info(traceback.format_exc())
+            LOGGER.info(
+                "Job completed with error",
+                extra={
+                    "event_type": event_context.event.type,
+                    "correlation_id": event_context.correlation_id,
+                },
             )
 
         self._update_status(job_id=event_context.correlation_id, status=status)
 
         # ack message and cleanup resources
         event_context.processed_successfully()
         self._current_task = None
@@ -318,15 +341,15 @@
     def _update_status(self, job_id: str, status: JobStatus) -> None:
         """Update GX Cloud on the status of a job.
 
         Args:
             job_id: job identifier, also known as correlation_id
             status: pydantic model encapsulating the current status
         """
-        LOGGER.info(f"Updating status: {job_id} - {status}")
+        LOGGER.info("Updating status", extra={"job_id": job_id, "status": str(status)})
         agent_sessions_url = (
             f"{self._config.gx_cloud_base_url}/organizations/{self._config.gx_cloud_organization_id}"
             + f"/agent-jobs/{job_id}"
         )
         session = create_session(access_token=self._config.gx_cloud_access_token)
         data = status.json()
         session.patch(agent_sessions_url, data=data)
@@ -345,21 +368,31 @@
         from great_expectations.data_context.store.gx_cloud_store_backend import GXCloudStoreBackend
 
         if Version(__version__) > Version(
             "0.19"  # using 0.19 instead of 1.0 to account for pre-releases
         ):
             # TODO: public API should be available in v1
             LOGGER.info(
-                f"Unable to set {HeaderName.USER_AGENT} or {HeaderName.AGENT_JOB_ID} header for requests to GX Cloud"
+                "Unable to set header for requests to GX Cloud",
+                extra={
+                    "user_agent": HeaderName.USER_AGENT,
+                    "agent_job_id": HeaderName.AGENT_JOB_ID,
+                },
             )
             return
 
         agent_version = self.get_current_gx_agent_version()
         LOGGER.debug(
-            f"Setting session headers for GX Cloud. {HeaderName.USER_AGENT}:{agent_version} {HeaderName.AGENT_JOB_ID}:{correlation_id}"
+            "Setting session headers for GX Cloud",
+            extra={
+                "user_agent": HeaderName.USER_AGENT,
+                "agent_version": agent_version,
+                "job_id": HeaderName.AGENT_JOB_ID,
+                "correlation_id": correlation_id,
+            },
         )
 
         if correlation_id:
             # OSS doesn't use the same session for all requests, so we need to set the header for each store
             for store in self._context.stores.values():
                 backend = store._store_backend
                 if isinstance(backend, GXCloudStoreBackend):
```

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/event_handler.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240426.0/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240425.0/great_expectations_cloud/logging/logging_cfg.py` & `great_expectations_cloud-20240426.0/great_expectations_cloud/logging/logging_cfg.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import enum
 import json
 import logging
 import logging.config
 import logging.handlers
 import pathlib
 from datetime import datetime, timezone
-from typing import Any, Final, Literal
+from typing import Any, ClassVar, Final, Literal
 
 from typing_extensions import override
 
 LOGGER = logging.getLogger(__name__)
 
 DEFAULT_LOG_FILE: Final[str] = "logfile"
 DEFAULT_LOG_DIR = "logs"
@@ -133,16 +133,33 @@
     LOGGER.info(f"Configured logging from file {log_cfg_file}")
 
 
 class JSONFormatter(logging.Formatter):
     """
     All custom formatting is done through subclassing this Formatter class
     Note: Defined within fn bc parametrization of Formatters is not supported by dictConfig
+
     """
 
+    _SKIP_KEYS: ClassVar[frozenset[str]] = frozenset(
+        [
+            "exc_text",
+            "levelno",
+            "lineno",
+            "msecs",
+            "msg",
+            "name",
+            "pathname",
+            "process",
+            "processName",
+            "thread",
+            "threadName",
+        ]
+    )
+
     def __init__(
         self,
         fmt: str | None = None,
         datefmt: str | None = None,
         style: Literal["%", "{", "$"] = "%",
         validate: bool = True,
         **kwargs: dict[str, Any],
@@ -151,23 +168,32 @@
         if custom_tags := kwargs.get("custom_tags"):
             self.custom_tags = custom_tags
         else:
             self.custom_tags = {}
 
     @override
     def format(self, record: logging.LogRecord) -> str:
-        optionals = {}
+        log_full = record.__dict__
+
+        log_full["event"] = record.msg
+        log_full["level"] = record.levelname
+        log_full["logger"] = record.name
+        log_full["timestamp"] = datetime.fromtimestamp(record.created, tz=timezone.utc).isoformat()
 
-        base_tags = {
-            "event": record.msg,
-            "level": record.levelname,
-            "logger": record.name,
-            "timestamp": datetime.fromtimestamp(record.created, tz=timezone.utc).isoformat(),
-        }
         if record.exc_info:
-            optionals["exc_info"] = str(record.exc_info)
-        if record.stack_info:
-            optionals["stack_info"] = record.stack_info
+            log_full["exc_info"] = str(record.exc_info)
 
-        complete_dict = {**base_tags, **self.custom_tags, **optionals}
+        if record.args:
+            log_full["args"] = str(record.args)
+
+        log_subset = {
+            key: value
+            for key, value in log_full.items()
+            if key is not None and key not in self._SKIP_KEYS
+        }
+
+        complete_dict = {
+            **log_subset,
+            **self.custom_tags,
+        }
 
         return json.dumps(complete_dict)
```

### Comparing `great_expectations_cloud-20240425.0/pyproject.toml` & `great_expectations_cloud-20240426.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240425.0"
+version = "20240426.0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
```

### Comparing `great_expectations_cloud-20240425.0/PKG-INFO` & `great_expectations_cloud-20240426.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240425.0
+Version: 20240426.0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
```

