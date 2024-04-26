# Comparing `tmp/redhat_assisted_installer-0.0.5.tar.gz` & `tmp/redhat_assisted_installer-0.0.6.tar.gz`

## Comparing `redhat_assisted_installer-0.0.5.tar` & `redhat_assisted_installer-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/__init__.py
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/assistedinstaller.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/logging.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/schema/__init__.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/schema/createParams.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/clusters/createanddelete.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/clusters/createcluster.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/clusters/deleteclusters.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/clusters/getcluster.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/infra-envs/createInfraEnvs.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/infra-envs/deleteInfraEnvs.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/tests/infra-envs/getInfraEnv.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/src/redhat_assisted_installer/__init__.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/src/redhat_assisted_installer/assistedinstaller.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/src/redhat_assisted_installer/lib/logging.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/src/redhat_assisted_installer/lib/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/src/redhat_assisted_installer/lib/schema/__init__.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/src/redhat_assisted_installer/lib/schema/createParams.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/tests/clusters/createanddelete.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/tests/clusters/createcluster.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/tests/clusters/deleteclusters.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/tests/clusters/getcluster.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/tests/infra-envs/createInfraEnvs.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/tests/infra-envs/deleteInfraEnvs.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/tests/infra-envs/getInfraEnv.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.6/PKG-INFO
```

### Comparing `redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/assistedinstaller.py` & `redhat_assisted_installer-0.0.6/src/redhat_assisted_installer/assistedinstaller.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,20 +159,20 @@
             else: 
                 logging.errorMessage(f"getClusters() method did not recieve a 200 status code, recieved {response.status_code} instead")
                 logging.errorMessage(f"{response.text}")  
                 return False     
         except Exception as e:
             logging.errorMessage(f"getClusters() method errored on request.get() with the following error: {e}")
 
-    def postCluster(self, name, version, hamode="None", cpuarchitecture='x86_64'):
+    def postCluster(self, name, version, basedomain, hamode="None", cpuarchitecture='x86_64'):
         url = self.apiBase + "clusters"
 
         headers = self.__getHeaders()
 
-        clusterparamas = createParams.clusterCreateParams(name, self.pullSecret, version=version, hamode=hamode, cpuarchitecture=cpuarchitecture)
+        clusterparamas = createParams.clusterCreateParams(name, self.pullSecret, version=version, basedomain=basedomain, hamode=hamode, cpuarchitecture=cpuarchitecture)
 
         data = clusterparamas.getParams()
 
         try:
             response = requests.post(url, headers=headers, json=data)
 
             if response.status_code == 201:
```

### Comparing `redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/tools.py` & `redhat_assisted_installer-0.0.6/src/redhat_assisted_installer/lib/tools.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.5/src/redhat_assisted_installer/lib/schema/createParams.py` & `redhat_assisted_installer-0.0.6/src/redhat_assisted_installer/lib/schema/createParams.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
     def getParams(self):
         return self.params
     
     
 
 class clusterCreateParams:
-    def __init__(self, name, pullsecret, version, hamode="None", cpuarchitecture='x86_64'):
+    def __init__(self, name, pullsecret, version, basedomain, hamode="None", cpuarchitecture='x86_64'):
         self.params = {}
         self.params['name'] = name + "infra-env"
         self.params['pull_secret'] = pullsecret
         self.params['openshift_version'] = version
         self.params['high_availability_mode'] = hamode
+        self.params['base_dns_domain'] = basedomain
         self.params['cpu_architecture'] = cpuarchitecture
 
     def getParams(self):
-    
         return self.params
```

### Comparing `redhat_assisted_installer-0.0.5/pyproject.toml` & `redhat_assisted_installer-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "redhat-assisted-installer"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Justin Batchelor", email="justinrossbatchelor@gmail.com" },
 ]
 description = "Python module to implement the RedHat Assisted Installer API"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `redhat_assisted_installer-0.0.5/PKG-INFO` & `redhat_assisted_installer-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: redhat-assisted-installer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python module to implement the RedHat Assisted Installer API
 Project-URL: Homepage, https://github.com/JustinBatchelor/red-hat-assisted-installer
 Project-URL: Issues, https://github.com/JustinBatchelor/red-hat-assisted-installer/issues
 Author-email: Justin Batchelor <justinrossbatchelor@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

