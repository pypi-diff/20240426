# Comparing `tmp/redhat_assisted_installer-0.0.4.tar.gz` & `tmp/redhat_assisted_installer-0.0.5.tar.gz`

## Comparing `redhat_assisted_installer-0.0.4.tar` & `redhat_assisted_installer-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/__init__.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/assistedinstaller.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/logging.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/schema/__init__.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/schema/createParams.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/clusters/createanddelete.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/clusters/createcluster.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/clusters/deleteclusters.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/clusters/getcluster.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/infra-envs/createInfraEnvs.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/infra-envs/deleteInfraEnvs.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/infra-envs/getInfraEnv.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/__init__.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/assistedinstaller.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/logging.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/schema/__init__.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/schema/createParams.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/clusters/createanddelete.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/clusters/createcluster.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/clusters/deleteclusters.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/clusters/getcluster.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/infra-envs/createInfraEnvs.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/infra-envs/deleteInfraEnvs.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/infra-envs/getInfraEnv.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/PKG-INFO
```

### Comparing `redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/assistedinstaller.py` & `redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/assistedinstaller.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,20 +84,20 @@
                 logging.errorMessage(f"getInfrastructureEnvironments() method did not recieve a 200 status code, recieved {response.status_code} instead")
                 logging.errorMessage(f"{response.text}")  
                 return False     
         except Exception as e:
             logging.errorMessage(f"getInfrastructureEnvironments() method errored on request.get() with the following error: {e}")
 
 
-    def postInfrastructureEnvironment(self, name, version=None):
+    def postInfrastructureEnvironment(self, name, cpuarchitecture="x86_64", version=None, clusterid=None):
         url = self.apiBase + "infra-envs"
 
         headers = self.__getHeaders()
 
-        infraparams = createParams.infraEnvCreateParams(name, self.pullSecret, version=version)
+        infraparams = createParams.infraEnvCreateParams(name, self.pullSecret, cpuarchitecture=cpuarchitecture, version=version, clusterid=clusterid)
 
         data = infraparams.getParams()
 
         try:
             response = requests.post(url, headers=headers, json=data)
 
             if response.status_code == 201:
```

### Comparing `redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/tools.py` & `redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/tools.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/schema/createParams.py` & `redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/schema/createParams.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.4/PKG-INFO` & `redhat_assisted_installer-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: redhat-assisted-installer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python module to implement the RedHat Assisted Installer API
 Project-URL: Homepage, https://github.com/JustinBatchelor/red-hat-assisted-installer
 Project-URL: Issues, https://github.com/JustinBatchelor/red-hat-assisted-installer/issues
 Author-email: Justin Batchelor <justinrossbatchelor@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

