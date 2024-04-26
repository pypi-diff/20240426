# Comparing `tmp/fedops-1.1.8.tar.gz` & `tmp/fedops-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedops-1.1.8.tar", last modified: Fri Dec  1 05:05:33 2023, max compression
+gzip compressed data, was "fedops-1.1.9.tar", last modified: Fri Dec  1 05:38:57 2023, max compression
```

## Comparing `fedops-1.1.8.tar` & `fedops-1.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:05:33.305528 fedops-1.1.8/
--rw-rw-r--   0 ccl       (1001) ccl       (1001)      647 2023-12-01 05:05:33.305528 fedops-1.1.8/PKG-INFO
-drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:05:33.305528 fedops-1.1.8/fedops/
--rw-rw-r--   0 ccl       (1001) ccl       (1001)      872 2023-08-23 06:40:49.000000 fedops-1.1.8/fedops/__init__.py
-drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:05:33.305528 fedops-1.1.8/fedops/client/
--rw-rw-r--   0 ccl       (1001) ccl       (1001)      987 2023-08-23 07:42:40.000000 fedops-1.1.8/fedops/client/__init__.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     9452 2023-12-01 05:02:05.000000 fedops-1.1.8/fedops/client/app.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     2813 2023-11-30 11:13:52.000000 fedops-1.1.8/fedops/client/client_api.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)    11737 2023-12-01 05:03:22.000000 fedops-1.1.8/fedops/client/client_fl.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     3591 2023-12-01 05:04:29.000000 fedops-1.1.8/fedops/client/client_utils.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     2501 2023-12-01 05:05:22.000000 fedops-1.1.8/fedops/client/client_wandb.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)        0 2023-08-23 06:40:49.000000 fedops-1.1.8/fedops/client/test.py
-drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:05:33.305528 fedops-1.1.8/fedops/server/
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     1107 2023-11-29 10:09:59.000000 fedops-1.1.8/fedops/server/__init__.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)    10147 2023-12-01 04:58:41.000000 fedops-1.1.8/fedops/server/app.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     4782 2023-12-01 05:00:11.000000 fedops-1.1.8/fedops/server/mobile_app.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     3921 2023-11-29 10:09:44.000000 fedops-1.1.8/fedops/server/mobile_strategy.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     1283 2023-09-01 02:00:16.000000 fedops-1.1.8/fedops/server/server_api.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     4793 2023-12-01 04:56:29.000000 fedops-1.1.8/fedops/server/server_utils.py
-drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:05:33.305528 fedops-1.1.8/fedops/simulation/
--rw-rw-r--   0 ccl       (1001) ccl       (1001)      801 2023-11-29 12:11:59.000000 fedops-1.1.8/fedops/simulation/__init__.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     3763 2023-11-29 14:10:42.000000 fedops-1.1.8/fedops/simulation/app.py
-drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:05:33.305528 fedops-1.1.8/fedops/simulation/fl_strategy/
--rw-rw-r--   0 ccl       (1001) ccl       (1001)      926 2023-11-29 11:47:29.000000 fedops-1.1.8/fedops/simulation/fl_strategy/__init__.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     7265 2023-11-30 02:48:10.000000 fedops-1.1.8/fedops/simulation/fl_strategy/aggregation.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     4557 2023-11-30 04:47:16.000000 fedops-1.1.8/fedops/simulation/fl_strategy/client.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     2211 2023-11-29 11:44:12.000000 fedops-1.1.8/fedops/simulation/fl_strategy/selection.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)    10335 2023-11-30 04:46:45.000000 fedops-1.1.8/fedops/simulation/fl_strategy/server.py
-drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:05:33.305528 fedops-1.1.8/fedops/utils/
--rw-rw-r--   0 ccl       (1001) ccl       (1001)        0 2023-08-24 04:23:10.000000 fedops-1.1.8/fedops/utils/__init__.py
--rw-rw-r--   0 ccl       (1001) ccl       (1001)      832 2023-08-23 06:40:49.000000 fedops-1.1.8/fedops/utils/version.py
-drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:05:33.305528 fedops-1.1.8/fedops.egg-info/
--rw-rw-r--   0 ccl       (1001) ccl       (1001)      647 2023-12-01 05:05:33.000000 fedops-1.1.8/fedops.egg-info/PKG-INFO
--rw-rw-r--   0 ccl       (1001) ccl       (1001)      840 2023-12-01 05:05:33.000000 fedops-1.1.8/fedops.egg-info/SOURCES.txt
--rw-rw-r--   0 ccl       (1001) ccl       (1001)        1 2023-12-01 05:05:33.000000 fedops-1.1.8/fedops.egg-info/dependency_links.txt
--rw-rw-r--   0 ccl       (1001) ccl       (1001)      195 2023-12-01 05:05:33.000000 fedops-1.1.8/fedops.egg-info/requires.txt
--rw-rw-r--   0 ccl       (1001) ccl       (1001)        7 2023-12-01 05:05:33.000000 fedops-1.1.8/fedops.egg-info/top_level.txt
--rw-rw-r--   0 ccl       (1001) ccl       (1001)       38 2023-12-01 05:05:33.305528 fedops-1.1.8/setup.cfg
--rw-rw-r--   0 ccl       (1001) ccl       (1001)     1161 2023-12-01 05:05:30.000000 fedops-1.1.8/setup.py
+drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:38:57.668611 fedops-1.1.9/
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)      647 2023-12-01 05:38:57.668611 fedops-1.1.9/PKG-INFO
+drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:38:57.664611 fedops-1.1.9/fedops/
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)      872 2023-08-23 06:40:49.000000 fedops-1.1.9/fedops/__init__.py
+drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:38:57.664611 fedops-1.1.9/fedops/client/
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)      987 2023-08-23 07:42:40.000000 fedops-1.1.9/fedops/client/__init__.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     9452 2023-12-01 05:02:05.000000 fedops-1.1.9/fedops/client/app.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     2813 2023-11-30 11:13:52.000000 fedops-1.1.9/fedops/client/client_api.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)    11737 2023-12-01 05:03:22.000000 fedops-1.1.9/fedops/client/client_fl.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     3591 2023-12-01 05:04:29.000000 fedops-1.1.9/fedops/client/client_utils.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     2501 2023-12-01 05:05:22.000000 fedops-1.1.9/fedops/client/client_wandb.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)        0 2023-08-23 06:40:49.000000 fedops-1.1.9/fedops/client/test.py
+drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:38:57.664611 fedops-1.1.9/fedops/server/
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     1107 2023-11-29 10:09:59.000000 fedops-1.1.9/fedops/server/__init__.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)    10142 2023-12-01 05:37:32.000000 fedops-1.1.9/fedops/server/app.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     4763 2023-12-01 05:38:46.000000 fedops-1.1.9/fedops/server/mobile_app.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     3921 2023-11-29 10:09:44.000000 fedops-1.1.9/fedops/server/mobile_strategy.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     1283 2023-09-01 02:00:16.000000 fedops-1.1.9/fedops/server/server_api.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     4793 2023-12-01 04:56:29.000000 fedops-1.1.9/fedops/server/server_utils.py
+drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:38:57.664611 fedops-1.1.9/fedops/simulation/
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)      801 2023-11-29 12:11:59.000000 fedops-1.1.9/fedops/simulation/__init__.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     3763 2023-11-29 14:10:42.000000 fedops-1.1.9/fedops/simulation/app.py
+drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:38:57.668611 fedops-1.1.9/fedops/simulation/fl_strategy/
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)      926 2023-11-29 11:47:29.000000 fedops-1.1.9/fedops/simulation/fl_strategy/__init__.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     7265 2023-11-30 02:48:10.000000 fedops-1.1.9/fedops/simulation/fl_strategy/aggregation.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     4557 2023-11-30 04:47:16.000000 fedops-1.1.9/fedops/simulation/fl_strategy/client.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     2211 2023-11-29 11:44:12.000000 fedops-1.1.9/fedops/simulation/fl_strategy/selection.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)    10335 2023-11-30 04:46:45.000000 fedops-1.1.9/fedops/simulation/fl_strategy/server.py
+drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:38:57.668611 fedops-1.1.9/fedops/utils/
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)        0 2023-08-24 04:23:10.000000 fedops-1.1.9/fedops/utils/__init__.py
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)      832 2023-08-23 06:40:49.000000 fedops-1.1.9/fedops/utils/version.py
+drwxrwxr-x   0 ccl       (1001) ccl       (1001)        0 2023-12-01 05:38:57.664611 fedops-1.1.9/fedops.egg-info/
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)      647 2023-12-01 05:38:57.000000 fedops-1.1.9/fedops.egg-info/PKG-INFO
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)      840 2023-12-01 05:38:57.000000 fedops-1.1.9/fedops.egg-info/SOURCES.txt
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)        1 2023-12-01 05:38:57.000000 fedops-1.1.9/fedops.egg-info/dependency_links.txt
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)      195 2023-12-01 05:38:57.000000 fedops-1.1.9/fedops.egg-info/requires.txt
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)        7 2023-12-01 05:38:57.000000 fedops-1.1.9/fedops.egg-info/top_level.txt
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)       38 2023-12-01 05:38:57.668611 fedops-1.1.9/setup.cfg
+-rw-rw-r--   0 ccl       (1001) ccl       (1001)     1161 2023-12-01 05:37:39.000000 fedops-1.1.9/setup.py
```

### Comparing `fedops-1.1.8/PKG-INFO` & `fedops-1.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 1.1.8
+Version: 1.1.9
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-1.1.8/fedops/__init__.py` & `fedops-1.1.9/fedops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/client/__init__.py` & `fedops-1.1.9/fedops/client/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/client/app.py` & `fedops-1.1.9/fedops/client/app.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/client/client_api.py` & `fedops-1.1.9/fedops/client/client_api.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/client/client_fl.py` & `fedops-1.1.9/fedops/client/client_fl.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/client/client_utils.py` & `fedops-1.1.9/fedops/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/client/client_wandb.py` & `fedops-1.1.9/fedops/client/client_wandb.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/server/__init__.py` & `fedops-1.1.9/fedops/server/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/server/app.py` & `fedops-1.1.9/fedops/server/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         def evaluate(
                 server_round: int,
                 parameters_ndarrays: fl.common.NDArrays,
                 config: Dict[str, fl.common.Scalar],
         ) -> Optional[Tuple[float, Dict[str, fl.common.Scalar]]]:
                         
             # model path for saving local model
-            gl_model_path = f'./{model_name}_gl_model_V{self.server.next_gl_model_v}'
+            gl_model_path = f'./{model_name}_gl_model_V{self.server.gl_model_v}'
             
             metrics = None
             
             if self.model_type == "Tensorflow":
                 # loss, accuracy, precision, recall, auc, auprc = model.evaluate(x_val, y_val)
                 loss, accuracy = model.evaluate(self.x_val, self.y_val)
```

### Comparing `fedops-1.1.8/fedops/server/mobile_app.py` & `fedops-1.1.9/fedops/server/mobile_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,18 @@
         )
 
 
     def start(self):
 
         today_time = datetime.datetime.today().strftime('%Y-%m-%d %H-%M-%S')
 
-        # self.next_model, self.next_model_name, self.server.latest_gl_model_v = server_utils.model_download_s3(self.task_id, self.model_type, self.init_model)
+        # self.next_model, self.next_model_name, self.server.last_gl_model_v = server_utils.model_download_s3(self.task_id, self.model_type, self.init_model)
 
         # New Global Model Version
-        # self.server.next_gl_model_v = self.server.latest_gl_model_v + 1
+        # self.server.gl_model_v = self.server.last_gl_model_v + 1
 
         # API that sends server status to server manager
         inform_Payload = {
             'S3_bucket': None,  # bucket name
             'Last_GL_Model': None,  # Model Weight File Name
             'FLServer_start': today_time,
             'FLSeReady': True,  # server ready status
@@ -97,17 +97,17 @@
             json_all_time_result = json.dumps(server_all_time_result)
             logging.info(f'server_operation_time - {json_all_time_result}')
             # Send server time result to performance pod
             server_api.ServerAPI(self.task_id).put_server_time_result(json_all_time_result)
             
             # # # upload global model
             # # if self.model_type == "Tensorflow":
-            # #     global_model_file_name = f"{gl_model_name}_gl_model_V{self.server.next_gl_model_v}.h5"
+            # #     global_model_file_name = f"{gl_model_name}_gl_model_V{self.server.gl_model_v}.h5"
             # # elif self.model_type =="Pytorch":
-            # #     global_model_file_name = f"{gl_model_name}_gl_model_V{self.server.next_gl_model_v}.pth"
+            # #     global_model_file_name = f"{gl_model_name}_gl_model_V{self.server.gl_model_v}.pth"
             # # server_utils.upload_model_to_bucket(self.task_id, global_model_file_name)
 
             # logging.info(f'upload {global_model_file_name} model in s3')
 
         # server_status error
         except Exception as e:
             logging.error('error: ', e)
```

### Comparing `fedops-1.1.8/fedops/server/mobile_strategy.py` & `fedops-1.1.9/fedops/server/mobile_strategy.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/server/server_api.py` & `fedops-1.1.9/fedops/server/server_api.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/server/server_utils.py` & `fedops-1.1.9/fedops/server/server_utils.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/simulation/__init__.py` & `fedops-1.1.9/fedops/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/simulation/app.py` & `fedops-1.1.9/fedops/simulation/app.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/simulation/fl_strategy/__init__.py` & `fedops-1.1.9/fedops/simulation/fl_strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/simulation/fl_strategy/aggregation.py` & `fedops-1.1.9/fedops/simulation/fl_strategy/aggregation.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/simulation/fl_strategy/client.py` & `fedops-1.1.9/fedops/simulation/fl_strategy/client.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/simulation/fl_strategy/selection.py` & `fedops-1.1.9/fedops/simulation/fl_strategy/selection.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/simulation/fl_strategy/server.py` & `fedops-1.1.9/fedops/simulation/fl_strategy/server.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops/utils/version.py` & `fedops-1.1.9/fedops/utils/version.py`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/fedops.egg-info/PKG-INFO` & `fedops-1.1.9/fedops.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedops
-Version: 1.1.8
+Version: 1.1.9
 Summary: FL Lifecycle Operations Management Platform
 Home-page: https://github.com/gachon-CCLab/FedOps.git
 Author: Semo Yang
 Author-email: tpah20@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fedops-1.1.8/fedops.egg-info/SOURCES.txt` & `fedops-1.1.9/fedops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedops-1.1.8/setup.py` & `fedops-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fedops',
-    version='1.1.8',
+    version='1.1.9',
     author='Semo Yang',
     author_email='tpah20@gmail.com',
     description='FL Lifecycle Operations Management Platform',
     long_description='Long description of your library',
     url='https://github.com/gachon-CCLab/FedOps.git',
     packages=find_packages(),
     install_requires=[
```

