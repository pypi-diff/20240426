# Comparing `tmp/eppo-server-sdk-1.3.0.tar.gz` & `tmp/eppo_server_sdk-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eppo-server-sdk-1.3.0.tar", last modified: Thu Oct  5 16:54:38 2023, max compression
+gzip compressed data, was "eppo_server_sdk-3.0.0.tar", last modified: Fri Apr 26 21:33:45 2024, max compression
```

## Comparing `eppo-server-sdk-1.3.0.tar` & `eppo_server_sdk-3.0.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-10-05 16:54:38.282195 eppo-server-sdk-1.3.0/
--rw-r--r--   0 leo        (501) staff       (20)     1071 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/LICENSE
--rw-r--r--   0 leo        (501) staff       (20)       88 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/MANIFEST.in
--rw-r--r--   0 leo        (501) staff       (20)      906 2023-10-05 16:54:38.282113 eppo-server-sdk-1.3.0/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      308 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/README.md
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-10-05 16:54:38.280927 eppo-server-sdk-1.3.0/eppo_client/
--rw-r--r--   0 leo        (501) staff       (20)     2507 2023-10-05 16:53:14.000000 eppo-server-sdk-1.3.0/eppo_client/__init__.py
--rw-r--r--   0 leo        (501) staff       (20)      266 2023-10-05 16:53:14.000000 eppo-server-sdk-1.3.0/eppo_client/assignment_logger.py
--rw-r--r--   0 leo        (501) staff       (20)      202 2023-10-05 16:53:14.000000 eppo-server-sdk-1.3.0/eppo_client/base_model.py
--rw-r--r--   0 leo        (501) staff       (20)     8970 2023-10-05 16:53:14.000000 eppo-server-sdk-1.3.0/eppo_client/client.py
--rw-r--r--   0 leo        (501) staff       (20)      378 2023-10-05 16:53:14.000000 eppo-server-sdk-1.3.0/eppo_client/config.py
--rw-r--r--   0 leo        (501) staff       (20)     1989 2023-10-05 16:53:14.000000 eppo-server-sdk-1.3.0/eppo_client/configuration_requestor.py
--rw-r--r--   0 leo        (501) staff       (20)      868 2023-10-05 04:02:28.000000 eppo-server-sdk-1.3.0/eppo_client/configuration_store.py
--rw-r--r--   0 leo        (501) staff       (20)      249 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/eppo_client/constants.py
--rw-r--r--   0 leo        (501) staff       (20)     2107 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/eppo_client/http_client.py
--rw-r--r--   0 leo        (501) staff       (20)     1130 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/eppo_client/poller.py
--rw-r--r--   0 leo        (501) staff       (20)     1222 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/eppo_client/read_write_lock.py
--rw-r--r--   0 leo        (501) staff       (20)     2207 2023-10-05 16:53:14.000000 eppo-server-sdk-1.3.0/eppo_client/rules.py
--rw-r--r--   0 leo        (501) staff       (20)      618 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/eppo_client/shard.py
--rw-r--r--   0 leo        (501) staff       (20)      193 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/eppo_client/validation.py
--rw-r--r--   0 leo        (501) staff       (20)     1152 2023-10-05 16:53:14.000000 eppo-server-sdk-1.3.0/eppo_client/variation_type.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-10-05 16:54:38.281822 eppo-server-sdk-1.3.0/eppo_server_sdk.egg-info/
--rw-r--r--   0 leo        (501) staff       (20)      906 2023-10-05 16:54:38.000000 eppo-server-sdk-1.3.0/eppo_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      691 2023-10-05 16:54:38.000000 eppo-server-sdk-1.3.0/eppo_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 leo        (501) staff       (20)        1 2023-10-05 16:54:38.000000 eppo-server-sdk-1.3.0/eppo_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 leo        (501) staff       (20)       47 2023-10-05 16:54:38.000000 eppo-server-sdk-1.3.0/eppo_server_sdk.egg-info/requires.txt
--rw-r--r--   0 leo        (501) staff       (20)       12 2023-10-05 16:54:38.000000 eppo-server-sdk-1.3.0/eppo_server_sdk.egg-info/top_level.txt
--rw-r--r--   0 leo        (501) staff       (20)       84 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/pyproject.toml
--rw-r--r--   0 leo        (501) staff       (20)       25 2023-09-08 21:47:05.000000 eppo-server-sdk-1.3.0/requirements-test.txt
--rw-r--r--   0 leo        (501) staff       (20)      123 2023-10-05 16:53:14.000000 eppo-server-sdk-1.3.0/requirements.txt
--rw-r--r--   0 leo        (501) staff       (20)      686 2023-10-05 16:54:38.282532 eppo-server-sdk-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:33:45.977213 eppo_server_sdk-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-26 21:33:45.977213 eppo_server_sdk-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:33:45.973213 eppo_server_sdk-3.0.0/eppo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/assignment_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/configuration_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/configuration_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/read_write_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/sharders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/eppo_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:33:45.977213 eppo_server_sdk-3.0.0/eppo_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-26 21:33:45.000000 eppo_server_sdk-3.0.0/eppo_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-26 21:33:45.000000 eppo_server_sdk-3.0.0/eppo_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:33:45.000000 eppo_server_sdk-3.0.0/eppo_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 21:33:45.000000 eppo_server_sdk-3.0.0/eppo_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 21:33:45.000000 eppo_server_sdk-3.0.0/eppo_server_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 21:33:42.000000 eppo_server_sdk-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 21:33:45.977213 eppo_server_sdk-3.0.0/setup.cfg
```

### Comparing `eppo-server-sdk-1.3.0/LICENSE` & `eppo_server_sdk-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.3.0/PKG-INFO` & `eppo_server_sdk-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 1.3.0
+Version: 3.0.0
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eppo-server-sdk-1.3.0/eppo_client/__init__.py` & `eppo_server_sdk-3.0.0/eppo_client/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Optional
 from eppo_client.client import EppoClient
 from eppo_client.config import Config
 from eppo_client.configuration_requestor import (
-    ExperimentConfigurationDto,
     ExperimentConfigurationRequestor,
 )
 from eppo_client.configuration_store import ConfigurationStore
 from eppo_client.constants import MAX_CACHE_ENTRIES
 from eppo_client.http_client import HttpClient, SdkParams
+from eppo_client.models import Flag
 from eppo_client.read_write_lock import ReadWriteLock
+from eppo_client.version import __version__
 
-__version__ = "1.3.0"
 
 __client: Optional[EppoClient] = None
 __lock = ReadWriteLock()
 
 
 def init(config: Config) -> EppoClient:
     """Initializes a global Eppo client instance
@@ -27,31 +27,33 @@
     :type config: Config
     """
     config._validate()
     sdk_params = SdkParams(
         apiKey=config.api_key, sdkName="python", sdkVersion=__version__
     )
     http_client = HttpClient(base_url=config.base_url, sdk_params=sdk_params)
-    config_store: ConfigurationStore[ExperimentConfigurationDto] = ConfigurationStore(
+    config_store: ConfigurationStore[Flag] = ConfigurationStore(
         max_size=MAX_CACHE_ENTRIES
     )
     config_requestor = ExperimentConfigurationRequestor(
         http_client=http_client, config_store=config_store
     )
     assignment_logger = config.assignment_logger
+    is_graceful_mode = config.is_graceful_mode
     global __client
     global __lock
     try:
         __lock.acquire_write()
         if __client:
             # if a client was already initialized, stop the background processes of the old client
             __client._shutdown()
         __client = EppoClient(
             config_requestor=config_requestor,
             assignment_logger=assignment_logger,
+            is_graceful_mode=is_graceful_mode,
         )
         return __client
     finally:
         __lock.release_write()
 
 
 def get_instance() -> EppoClient:
```

### Comparing `eppo-server-sdk-1.3.0/eppo_client/client.py` & `eppo_server_sdk-3.0.0/eppo_client/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,240 +1,265 @@
-import hashlib
 import datetime
 import logging
+import json
 from typing import Any, Dict, Optional
-from typing_extensions import deprecated
-from numbers import Number
 from eppo_client.assignment_logger import AssignmentLogger
 from eppo_client.configuration_requestor import (
-    ExperimentConfigurationDto,
     ExperimentConfigurationRequestor,
-    VariationDto,
 )
 from eppo_client.constants import POLL_INTERVAL_MILLIS, POLL_JITTER_MILLIS
+from eppo_client.models import VariationType
 from eppo_client.poller import Poller
-from eppo_client.rules import find_matching_rule
-from eppo_client.shard import ShardRange, get_shard, is_in_shard_range
+from eppo_client.sharders import MD5Sharder
+from eppo_client.types import SubjectAttributes, ValueType
 from eppo_client.validation import validate_not_blank
-from eppo_client.variation_type import VariationType
+from eppo_client.eval import FlagEvaluation, Evaluator, none_result
+from eppo_client.version import __version__
+
 
 logger = logging.getLogger(__name__)
 
 
 class EppoClient:
     def __init__(
         self,
         config_requestor: ExperimentConfigurationRequestor,
         assignment_logger: AssignmentLogger,
+        is_graceful_mode: bool = True,
     ):
         self.__config_requestor = config_requestor
         self.__assignment_logger = assignment_logger
+        self.__is_graceful_mode = is_graceful_mode
         self.__poller = Poller(
             interval_millis=POLL_INTERVAL_MILLIS,
             jitter_millis=POLL_JITTER_MILLIS,
             callback=config_requestor.fetch_and_store_configurations,
         )
         self.__poller.start()
+        self.__evaluator = Evaluator(sharder=MD5Sharder())
 
     def get_string_assignment(
-        self, subject_key: str, flag_key: str, subject_attributes=dict()
-    ) -> Optional[str]:
-        assigned_variation = self.get_assignment_variation(
-            subject_key, flag_key, subject_attributes, VariationType.STRING
-        )
-        return (
-            assigned_variation.typed_value
-            if assigned_variation is not None
-            else assigned_variation
+        self,
+        flag_key: str,
+        subject_key: str,
+        subject_attributes: SubjectAttributes,
+        default: str,
+    ) -> str:
+        return self.get_assignment_variation(
+            flag_key,
+            subject_key,
+            subject_attributes,
+            default,
+            VariationType.STRING,
+        )
+
+    def get_integer_assignment(
+        self,
+        flag_key: str,
+        subject_key: str,
+        subject_attributes: SubjectAttributes,
+        default: int,
+    ) -> int:
+        return self.get_assignment_variation(
+            flag_key,
+            subject_key,
+            subject_attributes,
+            default,
+            VariationType.INTEGER,
         )
 
     def get_numeric_assignment(
-        self, subject_key: str, flag_key: str, subject_attributes=dict()
-    ) -> Optional[Number]:
-        assigned_variation = self.get_assignment_variation(
-            subject_key, flag_key, subject_attributes, VariationType.NUMERIC
-        )
-        return (
-            assigned_variation.typed_value
-            if assigned_variation is not None
-            else assigned_variation
+        self,
+        flag_key: str,
+        subject_key: str,
+        subject_attributes: SubjectAttributes,
+        default: float,
+    ) -> float:
+        # convert to float in case we get an int
+        return float(
+            self.get_assignment_variation(
+                flag_key,
+                subject_key,
+                subject_attributes,
+                default,
+                VariationType.NUMERIC,
+            )
         )
 
     def get_boolean_assignment(
-        self, subject_key: str, flag_key: str, subject_attributes=dict()
-    ) -> Optional[bool]:
-        assigned_variation = self.get_assignment_variation(
-            subject_key, flag_key, subject_attributes, VariationType.BOOLEAN
-        )
-        return (
-            assigned_variation.typed_value
-            if assigned_variation is not None
-            else assigned_variation
-        )
-
-    def get_parsed_json_assignment(
-        self, subject_key: str, flag_key: str, subject_attributes=dict()
-    ) -> Optional[Dict[Any, Any]]:
-        assigned_variation = self.get_assignment_variation(
-            subject_key, flag_key, subject_attributes, VariationType.JSON
-        )
-        return (
-            assigned_variation.typed_value
-            if assigned_variation is not None
-            else assigned_variation
-        )
-
-    def get_json_string_assignment(
-        self, subject_key: str, flag_key: str, subject_attributes=dict()
-    ) -> Optional[str]:
-        assigned_variation = self.get_assignment_variation(
-            subject_key, flag_key, subject_attributes, VariationType.JSON
-        )
-        return (
-            assigned_variation.value
-            if assigned_variation is not None
-            else assigned_variation
-        )
-
-    @deprecated(
-        "get_assignment is deprecated in favor of the typed get_<type>_assignment methods"
-    )
-    def get_assignment(
-        self, subject_key: str, flag_key: str, subject_attributes=dict()
-    ) -> Optional[str]:
-        assigned_variation = self.get_assignment_variation(
-            subject_key, flag_key, subject_attributes
-        )
-        return (
-            assigned_variation.value
-            if assigned_variation is not None
-            else assigned_variation
+        self,
+        flag_key: str,
+        subject_key: str,
+        subject_attributes: SubjectAttributes,
+        default: bool,
+    ) -> bool:
+        return self.get_assignment_variation(
+            flag_key,
+            subject_key,
+            subject_attributes,
+            default,
+            VariationType.BOOLEAN,
+        )
+
+    def get_json_assignment(
+        self,
+        flag_key: str,
+        subject_key: str,
+        subject_attributes: SubjectAttributes,
+        default: Dict[Any, Any],
+    ) -> Dict[Any, Any]:
+        json_value = self.get_assignment_variation(
+            flag_key,
+            subject_key,
+            subject_attributes,
+            None,
+            VariationType.JSON,
         )
+        if json_value is None:
+            return default
+
+        return json.loads(json_value)
 
     def get_assignment_variation(
         self,
+        flag_key: str,
         subject_key: str,
+        subject_attributes: SubjectAttributes,
+        default: Optional[ValueType],
+        expected_variation_type: VariationType,
+    ):
+        try:
+            result = self.get_assignment_detail(
+                flag_key, subject_key, subject_attributes, expected_variation_type
+            )
+            if not result or not result.variation:
+                return default
+            return result.variation.value
+        except ValueError as e:
+            # allow ValueError to bubble up as it is a validation error
+            raise e
+        except Exception as e:
+            if self.__is_graceful_mode:
+                logger.error("[Eppo SDK] Error getting assignment: " + str(e))
+                return default
+            raise e
+
+    def get_assignment_detail(
+        self,
         flag_key: str,
-        subject_attributes: Any,
-        expected_variation_type: Optional[str] = None,
-    ) -> Optional[VariationDto]:
-        """Maps a subject to a variation for a given experiment
-        Returns None if the subject is not part of the experiment sample.
+        subject_key: str,
+        subject_attributes: SubjectAttributes,
+        expected_variation_type: VariationType,
+    ) -> FlagEvaluation:
+        """Maps a subject to a variation for a given flag
+        Returns None if the subject is not allocated in the flag
 
-        :param subject_key: an identifier of the experiment subject, for example a user ID.
-        :param flag_key: an experiment or feature flag identifier
+        :param subject_key: an identifier of the subject, for example a user ID.
+        :param flag_key: a feature flag identifier
         :param subject_attributes: optional attributes associated with the subject, for example name and email.
-        The subject attributes are used for evaluating any targeting rules tied to the experiment.
+        The subject attributes are used for evaluating any targeting rules tied
+        to the flag and logged in the logging callback.
         """
         validate_not_blank("subject_key", subject_key)
         validate_not_blank("flag_key", flag_key)
-        experiment_config = self.__config_requestor.get_configuration(flag_key)
-        override = self._get_subject_variation_override(experiment_config, subject_key)
-        if override:
-            if expected_variation_type is not None:
-                variation_is_expected_type = VariationType.is_expected_type(
-                    override, expected_variation_type
-                )
-                if not variation_is_expected_type:
-                    return None
-            return override
+        if subject_attributes is None:
+            subject_attributes = {}
 
-        if experiment_config is None or not experiment_config.enabled:
-            logger.info(
-                "[Eppo SDK] No assigned variation. No active experiment or flag for key: "
-                + flag_key
+        flag = self.__config_requestor.get_configuration(flag_key)
+
+        if flag is None:
+            logger.warning(
+                "[Eppo SDK] No assigned variation. Flag not found: " + flag_key
+            )
+            return none_result(
+                flag_key, expected_variation_type, subject_key, subject_attributes
             )
-            return None
 
-        matched_rule = find_matching_rule(subject_attributes, experiment_config.rules)
-        if matched_rule is None:
-            logger.info(
-                "[Eppo SDK] No assigned variation. Subject attributes do not match targeting rules: {0}".format(
-                    subject_attributes
-                )
+        if not check_type_match(expected_variation_type, flag.variation_type):
+            raise TypeError(
+                f"Variation value does not have the correct type."
+                f" Found: {flag.variation_type} != {expected_variation_type}"
             )
-            return None
 
-        allocation = experiment_config.allocations[matched_rule.allocation_key]
-        if not self._is_in_experiment_sample(
-            subject_key,
-            flag_key,
-            experiment_config.subject_shards,
-            allocation.percent_exposure,
-        ):
+        if not flag.enabled:
             logger.info(
-                "[Eppo SDK] No assigned variation. Subject is not part of experiment sample population"
+                "[Eppo SDK] No assigned variation. Flag is disabled: " + flag_key
+            )
+            return none_result(
+                flag_key, expected_variation_type, subject_key, subject_attributes
             )
-            return None
 
-        shard = get_shard(
-            "assignment-{}-{}".format(subject_key, flag_key),
-            experiment_config.subject_shards,
-        )
-        assigned_variation = next(
-            (
-                variation
-                for variation in allocation.variations
-                if is_in_shard_range(shard, variation.shard_range)
-            ),
-            None,
-        )
+        result = self.__evaluator.evaluate_flag(flag, subject_key, subject_attributes)
 
-        assigned_variation_value_to_log = None
-        if assigned_variation is not None:
-            assigned_variation_value_to_log = assigned_variation.value
-            if expected_variation_type is not None:
-                variation_is_expected_type = VariationType.is_expected_type(
-                    assigned_variation, expected_variation_type
-                )
-                if not variation_is_expected_type:
-                    return None
+        if result.variation and not check_value_type_match(
+            expected_variation_type, result.variation.value
+        ):
+            logger.error(
+                "[Eppo SDK] Variation value does not have the correct type for the flag: "
+                f"{flag_key} and variation key {result.variation.key}"
+            )
+            return none_result(
+                flag_key, flag.variation_type, subject_key, subject_attributes
+            )
 
         assignment_event = {
-            "allocation": matched_rule.allocation_key,
-            "experiment": f"{flag_key}-{matched_rule.allocation_key}",
+            **(result.extra_logging if result else {}),
+            "allocation": result.allocation_key if result else None,
+            "experiment": f"{flag_key}-{result.allocation_key}" if result else None,
             "featureFlag": flag_key,
-            "variation": assigned_variation_value_to_log,
+            "variation": result.variation.key if result and result.variation else None,
             "subject": subject_key,
             "timestamp": datetime.datetime.utcnow().isoformat(),
             "subjectAttributes": subject_attributes,
+            "metaData": {"sdkLanguage": "python", "sdkVersion": __version__},
         }
         try:
-            self.__assignment_logger.log_assignment(assignment_event)
+            if result and result.do_log:
+                self.__assignment_logger.log_assignment(assignment_event)
         except Exception as e:
             logger.error("[Eppo SDK] Error logging assignment event: " + str(e))
-        return assigned_variation
+        return result
+
+    def get_flag_keys(self):
+        """
+        Returns a list of all flag keys that have been initialized.
+        This can be useful to debug the initialization process.
+
+        Note that it is generally not a good idea to pre-load all flag configurations.
+        """
+        return self.__config_requestor.get_flag_keys()
+
+    def is_initialized(self):
+        """
+        Returns True if the client has successfully initialized
+        the flag configuration and is ready to serve requests.
+        """
+        return self.__config_requestor.is_initialized()
 
     def _shutdown(self):
         """Stops all background processes used by the client
         Do not use the client after calling this method.
         """
         self.__poller.stop()
 
-    def _get_subject_variation_override(
-        self, experiment_config: Optional[ExperimentConfigurationDto], subject: str
-    ) -> Optional[VariationDto]:
-        subject_hash = hashlib.md5(subject.encode("utf-8")).hexdigest()
-        if (
-            experiment_config is not None
-            and subject_hash in experiment_config.overrides
-        ):
-            return VariationDto(
-                name="override",
-                value=experiment_config.overrides[subject_hash],
-                typed_value=experiment_config.typed_overrides[subject_hash],
-                shard_range=ShardRange(start=0, end=10000),
-            )
-        return None
-
-    def _is_in_experiment_sample(
-        self,
-        subject: str,
-        experiment_key: str,
-        subject_shards: int,
-        percent_exposure: float,
-    ):
-        shard = get_shard(
-            "exposure-{}-{}".format(subject, experiment_key),
-            subject_shards,
-        )
-        return shard <= percent_exposure * subject_shards
+
+def check_type_match(
+    expected_type: Optional[VariationType], actual_type: VariationType
+):
+    return expected_type is None or actual_type == expected_type
+
+
+def check_value_type_match(
+    expected_type: Optional[VariationType], value: ValueType
+) -> bool:
+    if expected_type is None:
+        return True
+    if expected_type in [VariationType.JSON, VariationType.STRING]:
+        return isinstance(value, str)
+    if expected_type == VariationType.INTEGER:
+        return isinstance(value, int)
+    if expected_type == VariationType.NUMERIC:
+        # we can convert int to float
+        return isinstance(value, float) or isinstance(value, int)
+    if expected_type == VariationType.BOOLEAN:
+        return isinstance(value, bool)
+    return False
```

### Comparing `eppo-server-sdk-1.3.0/eppo_client/configuration_store.py` & `eppo_server_sdk-3.0.0/eppo_client/configuration_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,11 +19,15 @@
             return None  # key does not exist
         finally:
             self.__lock.release_read()
 
     def set_configurations(self, configs: Dict[str, T]):
         try:
             self.__lock.acquire_write()
+            self.__cache.clear()
             for key, config in configs.items():
                 self.__cache[key] = config
         finally:
             self.__lock.release_write()
+
+    def get_keys(self):
+        return list(self.__cache.keys())
```

### Comparing `eppo-server-sdk-1.3.0/eppo_client/http_client.py` & `eppo_server_sdk-3.0.0/eppo_client/http_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any
 from requests.exceptions import Timeout
 from requests.adapters import HTTPAdapter, Retry
 from http import HTTPStatus
 
 import requests
 
-from eppo_client.base_model import SdkBaseModel
+from eppo_client.models import SdkBaseModel
 
 
 class SdkParams(SdkBaseModel):
     # attributes are camelCase because that's what the backend endpoint expects
     apiKey: str
     sdkName: str
     sdkVersion: str
@@ -39,15 +39,15 @@
     def is_unauthorized(self) -> bool:
         return self.__is_unauthorized
 
     def get(self, resource: str) -> Any:
         try:
             response = self.__session.get(
                 self.__base_url + resource,
-                params=self.__sdk_params.dict(),
+                params=self.__sdk_params.model_dump(),
                 timeout=REQUEST_TIMEOUT_SECONDS,
             )
             self.__is_unauthorized = response.status_code == HTTPStatus.UNAUTHORIZED
             if response.status_code != HTTPStatus.OK:
                 raise self._get_http_error(response.status_code, resource)
             return response.json()
         except Timeout:
```

### Comparing `eppo-server-sdk-1.3.0/eppo_client/poller.py` & `eppo_server_sdk-3.0.0/eppo_client/poller.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.3.0/eppo_client/read_write_lock.py` & `eppo_server_sdk-3.0.0/eppo_client/read_write_lock.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def release_read(self):
         """Release a read lock."""
         self._read_ready.acquire()
         try:
             self._readers -= 1
             if not self._readers:
-                self._read_ready.notifyAll()
+                self._read_ready.notify_all()
         finally:
             self._read_ready.release()
 
     def acquire_write(self):
         """Acquire a write lock. Blocks until there are no
         acquired read or write locks."""
         self._read_ready.acquire()
```

### Comparing `eppo-server-sdk-1.3.0/eppo_server_sdk.egg-info/PKG-INFO` & `eppo_server_sdk-3.0.0/eppo_server_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 1.3.0
+Version: 3.0.0
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eppo-server-sdk-1.3.0/eppo_server_sdk.egg-info/SOURCES.txt` & `eppo_server_sdk-3.0.0/eppo_server_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 eppo_client/assignment_logger.py
 eppo_client/base_model.py
 eppo_client/client.py
 eppo_client/config.py
 eppo_client/configuration_requestor.py
 eppo_client/configuration_store.py
 eppo_client/constants.py
+eppo_client/eval.py
 eppo_client/http_client.py
+eppo_client/models.py
 eppo_client/poller.py
 eppo_client/read_write_lock.py
 eppo_client/rules.py
-eppo_client/shard.py
+eppo_client/sharders.py
+eppo_client/types.py
 eppo_client/validation.py
-eppo_client/variation_type.py
+eppo_client/version.py
 eppo_server_sdk.egg-info/PKG-INFO
 eppo_server_sdk.egg-info/SOURCES.txt
 eppo_server_sdk.egg-info/dependency_links.txt
 eppo_server_sdk.egg-info/requires.txt
 eppo_server_sdk.egg-info/top_level.txt
```

### Comparing `eppo-server-sdk-1.3.0/setup.cfg` & `eppo_server_sdk-3.0.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eppo-server-sdk
-version = attr: eppo_client.__version__
+version = attr: eppo_client.version.__version__
 author = Eppo
 author_email = eppo-team@geteppo.com
 description = Eppo SDK for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Eppo-exp/python-sdk
 project_urls =
```

