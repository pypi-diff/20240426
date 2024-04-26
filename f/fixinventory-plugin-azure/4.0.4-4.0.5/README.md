# Comparing `tmp/fixinventory_plugin_azure-4.0.4.tar.gz` & `tmp/fixinventory_plugin_azure-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory_plugin_azure-4.0.4.tar", last modified: Wed Apr 24 19:31:43 2024, max compression
+gzip compressed data, was "fixinventory_plugin_azure-4.0.5.tar", last modified: Fri Apr 26 20:31:11 2024, max compression
```

## Comparing `fixinventory_plugin_azure-4.0.4.tar` & `fixinventory_plugin_azure-4.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:43.433275 fixinventory_plugin_azure-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-24 19:31:43.433275 fixinventory_plugin_azure-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:43.429275 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11410 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/azure_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:43.433275 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32066 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)   308884 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    81717 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/containerservice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11954 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)   443396 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/fix_plugin_azure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:31:43.433275 fixinventory_plugin_azure-4.0.4/fixinventory_plugin_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-24 19:31:43.000000 fixinventory_plugin_azure-4.0.4/fixinventory_plugin_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 19:31:43.000000 fixinventory_plugin_azure-4.0.4/fixinventory_plugin_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:31:43.000000 fixinventory_plugin_azure-4.0.4/fixinventory_plugin_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 19:31:43.000000 fixinventory_plugin_azure-4.0.4/fixinventory_plugin_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:28:19.000000 fixinventory_plugin_azure-4.0.4/fixinventory_plugin_azure.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 19:31:43.000000 fixinventory_plugin_azure-4.0.4/fixinventory_plugin_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 19:31:43.000000 fixinventory_plugin_azure-4.0.4/fixinventory_plugin_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-24 19:27:17.000000 fixinventory_plugin_azure-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 19:31:43.433275 fixinventory_plugin_azure-4.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:31:11.403431 fixinventory_plugin_azure-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-26 20:31:11.403431 fixinventory_plugin_azure-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:31:11.399431 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/azure_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:31:11.399431 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   308884 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81717 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/containerservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11954 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)   443396 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/fix_plugin_azure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:31:11.403431 fixinventory_plugin_azure-4.0.5/fixinventory_plugin_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-26 20:31:11.000000 fixinventory_plugin_azure-4.0.5/fixinventory_plugin_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 20:31:11.000000 fixinventory_plugin_azure-4.0.5/fixinventory_plugin_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:31:11.000000 fixinventory_plugin_azure-4.0.5/fixinventory_plugin_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-26 20:31:11.000000 fixinventory_plugin_azure-4.0.5/fixinventory_plugin_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:27:39.000000 fixinventory_plugin_azure-4.0.5/fixinventory_plugin_azure.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-26 20:31:11.000000 fixinventory_plugin_azure-4.0.5/fixinventory_plugin_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 20:31:11.000000 fixinventory_plugin_azure-4.0.5/fixinventory_plugin_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-26 20:26:34.000000 fixinventory_plugin_azure-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-26 20:31:11.403431 fixinventory_plugin_azure-4.0.5/setup.cfg
```

### Comparing `fixinventory_plugin_azure-4.0.4/PKG-INFO` & `fixinventory_plugin_azure-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-azure
-Version: 4.0.4
+Version: 4.0.5
 Summary: Runs collector plugins and sends the result to fixcore.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/azure
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: retrying
 Requires-Dist: azure-identity
 Requires-Dist: azure-mgmt-resource
 
 # fix-plugin-azure
 An Azure collector plugin for Fix.
```

### Comparing `fixinventory_plugin_azure-4.0.4/fix_plugin_azure/__init__.py` & `fixinventory_plugin_azure-4.0.5/fix_plugin_azure/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 cloud,
                 evolve(subscription, account_name=name),
                 ac,
                 self.core_feedback.with_context(cloud.id, subscription.safe_name),
                 self.task_data,
             )
             for name, ac in account_configs.items()
-            for subscription in AzureSubscription.list_subscriptions(ac.credentials())
+            for subscription in AzureSubscription.list_subscriptions(config, ac.credentials())
             if ac.allowed(subscription.subscription_id)
         }
         args = list(args_by_subscription_id.values())
 
         # Send initial progress
         progress = ProgressTree(self.cloud)
         for sub in args:
```

### Comparing `fixinventory_plugin_azure-4.0.4/fix_plugin_azure/azure_client.py` & `fixinventory_plugin_azure-4.0.5/fix_plugin_azure/azure_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from azure.core.rest import HttpRequest
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.resource import ResourceManagementClient
 from azure.mgmt.resource.resources._serialization import Serializer
 from azure.mgmt.resource.resources.models import GenericResource
 
-from fix_plugin_azure.config import AzureCredentials
+from fix_plugin_azure.config import AzureConfig, AzureCredentials
 from fixlib.core.actions import CoreFeedback, ErrorAccumulator
 from fixlib.types import Json
 
 log = logging.getLogger("fix.plugins.azure")
 
 
 class MetricRequestError(HttpResponseError):
@@ -78,36 +78,39 @@
 
     @abstractmethod
     def delete_resource_tag(self, tag_name: str, resource_id: str) -> bool:
         pass
 
     @staticmethod
     def __create_management_client(
+        config: AzureConfig,
         credential: AzureCredentials,
         subscription_id: str,
         core_feedback: Optional[CoreFeedback] = None,
         error_accumulator: Optional[ErrorAccumulator] = None,
         resource_group: Optional[str] = None,
     ) -> AzureClient:
         return AzureResourceManagementClient(
-            credential, subscription_id, resource_group, core_feedback, error_accumulator
+            config, credential, subscription_id, resource_group, core_feedback, error_accumulator
         )
 
     create = __create_management_client
 
 
 class AzureResourceManagementClient(AzureClient):
     def __init__(
         self,
+        config: AzureConfig,
         credential: AzureCredentials,
         subscription_id: str,
         location: Optional[str] = None,
         core_feedback: Optional[CoreFeedback] = None,
         accumulator: Optional[ErrorAccumulator] = None,
     ) -> None:
+        self.config = config
         self.credential = credential
         self.subscription_id = subscription_id
         self.location = location
         self.core_feedback = core_feedback
         self.accumulator = accumulator or ErrorAccumulator()
         self.client = ResourceManagementClient(self.credential, self.subscription_id)
 
@@ -117,18 +120,24 @@
             return []
         return result  # type: ignore
 
     def delete(self, resource_id: str) -> bool:
         try:
             self.client.resources.begin_delete_by_id(resource_id=resource_id, api_version="2021-04-01")
         except HttpResponseError as e:
-            if e.error and e.error.code == "ResourceNotFoundError":
-                return False  # Resource not found to delete
-            else:
-                raise e
+            if error := e.error:
+                error_code = error.code or "Unknown"
+                if error_code == "ResourceNotFoundError":
+                    return False  # Resource not found to delete
+                else:
+                    msg = f"An Azure API error occurred during the deletion of a resource: {e}"
+                    self.accumulator.add_error(False, error_code, "Resource deletion", "service_resource", msg)
+                    if self.config.discard_account_on_resource_error:
+                        raise
+                    return False
 
         return True
 
     def update_resource_tag(self, tag_name: str, tag_value: str, resource_id: str) -> bool:
         return self._update_or_delete_tag(
             tag_name=tag_name, tag_value=tag_value, resource_id=resource_id, is_update=True
         )
@@ -156,34 +165,45 @@
                     return True
 
             # Create or update the resource to reflect the removal of the tag
             updated_resource = GenericResource(location=resource.location, tags=resource.tags)
             self.client.resources.begin_create_or_update_by_id(resource_id, "2021-04-01", updated_resource)
 
         except HttpResponseError as e:
-            if e.error and e.error.code == "ResourceNotFoundError":
-                return False  # Resource not found
-            elif e.error and e.error.code == "ResourceExistsError":
-                return False  # Tag for update/delete does not exist
-            else:
-                raise e
+            if error := e.error:
+                error_code = error.code or "Unknown"
+                if error_code == "ResourceNotFoundError":
+                    return False  # Resource not found
+                elif error_code == "ResourceExistsError":
+                    return False  # Tag for update/delete does not exist
+                else:
+                    msg = f"An Azure API error occurred during the updating or deletion tag of a resource: {e}"
+                    self.accumulator.add_error(
+                        False, error_code, "Resource updating or deletion", "service_resource", msg
+                    )
+                    if self.config.discard_account_on_resource_error:
+                        raise
+                    return False
 
         return True
 
     @retry(  # type: ignore
         stop_max_attempt_number=10,  # 10 attempts: 1000 max 60000: max wait time is 5 minutes
         wait_exponential_multiplier=1000,
         wait_exponential_max=60000,
         retry_on_exception=is_retryable_exception,
     )
     def _list_with_retry(self, spec: AzureApiSpec, **kwargs: Any) -> Optional[List[Json]]:
         try:
             return self._call(spec, **kwargs)
         except ClientAuthenticationError as e:
-            log.error(f"[Azure] Call to Azure API is not authorized!: {e}")
+            log.warning(f"[Azure] Call to Azure API is not authorized!: {e}")
+            if (error := e.error) and (error_code := error.code):
+                msg = "Call to Azure API is not authorized!"
+                self.accumulator.add_error(False, error_code, spec.service, spec.path, msg, self.location)
             return None
         except HttpResponseError as e:
             if error := e.error:
                 if error.code == "NoRegisteredProviderFound":
                     return None  # API not available in this region
                 elif error.code in spec.expected_error_codes:
                     return None
@@ -191,14 +211,16 @@
                     raise MetricRequestError from e
                 code = error.code or "Unknown"
                 self.accumulator.add_error(False, code, spec.service, spec.path, str(e), self.location)
             log.warning(f"[Azure] Client Error: status={e.status_code}, error={e.error}, message={e}")
             return None
         except Exception as e:
             log.warning(f"[Azure] called service={spec.service}: hit unexpected error: {e}", exc_info=e)
+            if self.config.discard_account_on_resource_error:
+                raise
             return None
 
     # noinspection PyProtectedMember
     def _call(self, spec: AzureApiSpec, **kwargs: Any) -> List[Json]:
         ser = Serializer()
 
         error_map = {
@@ -281,8 +303,10 @@
         request = HttpRequest(method="GET", url=url, params=params, headers=headers)
         pipeline_response: PipelineResponse = self.client._client._pipeline.run(request, stream=False)  # type: ignore
         response = pipeline_response.http_response
 
         return response
 
     def for_location(self, location: str) -> AzureClient:
-        return AzureClient.create(self.credential, self.subscription_id, self.core_feedback, self.accumulator, location)
+        return AzureClient.create(
+            self.config, self.credential, self.subscription_id, self.core_feedback, self.accumulator, location
+        )
```

### Comparing `fixinventory_plugin_azure-4.0.4/fix_plugin_azure/collector.py` & `fixinventory_plugin_azure-4.0.5/fix_plugin_azure/collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
             thread_name_prefix=f"azure_{self.subscription.subscription_id}",
             max_workers=self.config.resource_pool_size,
         ) as executor:
             self.core_feedback.progress_done(self.subscription.subscription_id, 0, 1, context=[self.cloud.id])
             queue = ExecutorQueue(executor, "azure_collector")
             error_accumulator = ErrorAccumulator()
             client = AzureClient.create(
+                self.config,
                 self.credentials,
                 self.subscription.subscription_id,
                 core_feedback=self.core_feedback,
                 error_accumulator=error_accumulator,
             )
 
             def get_last_run() -> Optional[datetime]:
```

### Comparing `fixinventory_plugin_azure-4.0.4/fix_plugin_azure/config.py` & `fixinventory_plugin_azure-4.0.5/fix_plugin_azure/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,11 +64,19 @@
     )
 
     accounts: Optional[Dict[str, AzureAccountConfig]] = field(
         factory=lambda: {"default": AzureAccountConfig()},
         metadata={"description": "Configure accounts to collect subscriptions. You can define multiple accounts here."},
     )
 
+    discard_account_on_resource_error: bool = field(
+        default=False,
+        metadata={
+            "description": "Fail the whole account if collecting a resource fails. "
+            "If false, the error is logged and the resource is skipped."
+        },
+    )
+
     collect_usage_metrics: Optional[bool] = field(
         default=True,
         metadata={"description": "Collect resource usage metrics via Azure Metric, enabled by default"},
     )
```

### Comparing `fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/base.py` & `fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     config = current_config()
     azure_config = cast(AzureConfig, config.azure)
     #  Taking credentials from the config if access through the environment cannot be provided
     if azure_config.accounts and (account := azure_config.accounts.get(subscription_id)):
         credential = account.credentials()
     else:
         credential = DefaultAzureCredential()
-    return AzureClient.create(credential=credential, subscription_id=subscription_id)
+    return AzureClient.create(config=azure_config, credential=credential, subscription_id=subscription_id)
 
 
 T = TypeVar("T")
 
 
 class AzureResource(BaseResource):
     kind: ClassVar[str] = "azure_resource"
@@ -151,23 +151,28 @@
     @classmethod
     def collect_resources(
         cls: Type[AzureResourceType], builder: GraphBuilder, **kwargs: Any
     ) -> List[AzureResourceType]:
         # Default behavior: in case the class has an ApiSpec, call the api and call collect.
         log.debug(f"[Azure:{builder.subscription.id}] Collecting {cls.__name__} with ({kwargs})")
         if spec := cls.api_spec:
-            # TODO: add error handling
-            items = builder.client.list(spec, **kwargs)
-            collected = cls.collect(items, builder)
-            if builder.config.collect_usage_metrics:
-                try:
-                    cls.collect_usage_metrics(builder, collected)
-                except Exception as e:
-                    log.warning(f"Failed to collect usage metrics for {cls.__name__}: {e}")
-            return collected
+            try:
+                items = builder.client.list(spec, **kwargs)
+                collected = cls.collect(items, builder)
+                if builder.config.collect_usage_metrics:
+                    try:
+                        cls.collect_usage_metrics(builder, collected)
+                    except Exception as e:
+                        log.warning(f"Failed to collect usage metrics for {cls.__name__}: {e}")
+                return collected
+            except Exception as e:
+                msg = f"Error while collecting {cls.__name__} with service {spec.service} and location: {builder.location}: {e}"
+                builder.core_feedback.info(msg, log)
+                raise
+
         return []
 
     @classmethod
     def collect(
         cls: Type[AzureResourceType],
         raw: List[Json],
         builder: GraphBuilder,
@@ -402,16 +407,16 @@
     state: Optional[str] = field(default=None, metadata={'description': 'The subscription state. Possible values are enabled, warned, pastdue, disabled, and deleted.'})  # fmt: skip
     subscription_id: str = field(default="", metadata={"description": "The subscription id."})
     subscription_policies: Optional[AzureSubscriptionPolicies] = field(default=None, metadata={'description': 'Subscription policies.'})  # fmt: skip
     tenant_id: Optional[str] = field(default=None, metadata={"description": "The subscription tenant id."})
     account_name: Optional[str] = field(default=None, metadata={"description": "The account used to collect this subscription."})  # fmt: skip
 
     @classmethod
-    def list_subscriptions(cls, credentials: AzureCredentials) -> List[AzureSubscription]:
-        client = AzureClient.create(credentials, "global")
+    def list_subscriptions(cls, config: AzureConfig, credentials: AzureCredentials) -> List[AzureSubscription]:
+        client = AzureClient.create(config, credentials, "global")
         return [cls.from_api(js) for js in client.list(cls.api_spec)]
 
 
 @define(eq=False, slots=False)
 class AzureSubResource:
     kind: ClassVar[str] = "azure_sub_resource"
     mapping: ClassVar[Dict[str, Bender]] = {"id": S("id")}
```

### Comparing `fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/compute.py` & `fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/compute.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/containerservice.py` & `fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/containerservice.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/metrics.py` & `fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/metrics.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_azure-4.0.4/fix_plugin_azure/resource/network.py` & `fixinventory_plugin_azure-4.0.5/fix_plugin_azure/resource/network.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_azure-4.0.4/fix_plugin_azure/utils.py` & `fixinventory_plugin_azure-4.0.5/fix_plugin_azure/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_azure-4.0.4/fixinventory_plugin_azure.egg-info/PKG-INFO` & `fixinventory_plugin_azure-4.0.5/fixinventory_plugin_azure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-azure
-Version: 4.0.4
+Version: 4.0.5
 Summary: Runs collector plugins and sends the result to fixcore.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/azure
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.4
+Requires-Dist: fixinventorylib==4.0.5
 Requires-Dist: retrying
 Requires-Dist: azure-identity
 Requires-Dist: azure-mgmt-resource
 
 # fix-plugin-azure
 An Azure collector plugin for Fix.
```

### Comparing `fixinventory_plugin_azure-4.0.4/fixinventory_plugin_azure.egg-info/SOURCES.txt` & `fixinventory_plugin_azure-4.0.5/fixinventory_plugin_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_azure-4.0.4/pyproject.toml` & `fixinventory_plugin_azure-4.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixinventory-plugin-azure"
-version = "4.0.4"
+version = "4.0.5"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to fixcore."
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.4",
+    "fixinventorylib==4.0.5",
     "retrying",
     "azure-identity",
     "azure-mgmt-resource"
 ]
 
 [project.entry-points."fix.plugins"]
 azure = "fix_plugin_azure:AzureCollectorPlugin"
```

