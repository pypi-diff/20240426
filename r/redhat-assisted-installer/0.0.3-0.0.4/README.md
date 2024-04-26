# Comparing `tmp/redhat_assisted_installer-0.0.3.tar.gz` & `tmp/redhat_assisted_installer-0.0.4.tar.gz`

## Comparing `redhat_assisted_installer-0.0.3.tar` & `redhat_assisted_installer-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/src/redhat_assisted_installer/__init__.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/src/redhat_assisted_installer/assistedinstaller.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/src/redhat_assisted_installer/lib/logging.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/src/redhat_assisted_installer/lib/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/src/redhat_assisted_installer/lib/schema/__init__.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/src/redhat_assisted_installer/lib/schema/createParams.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/tests/createInfraEnvs.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/tests/deleteInfraEnvs.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/tests/getInfraEnv.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/__init__.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/assistedinstaller.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/logging.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/schema/__init__.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/schema/createParams.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/clusters/createanddelete.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/clusters/createcluster.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/clusters/deleteclusters.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/clusters/getcluster.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/infra-envs/createInfraEnvs.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/infra-envs/deleteInfraEnvs.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/tests/infra-envs/getInfraEnv.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.4/PKG-INFO
```

### Comparing `redhat_assisted_installer-0.0.3/src/redhat_assisted_installer/lib/tools.py` & `redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/tools.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.3/src/redhat_assisted_installer/lib/schema/createParams.py` & `redhat_assisted_installer-0.0.4/src/redhat_assisted_installer/lib/schema/createParams.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 
 class clusterCreateParams:
     def __init__(self, name, pullsecret, version, hamode="None", cpuarchitecture='x86_64'):
         self.params = {}
         self.params['name'] = name + "infra-env"
         self.params['pull_secret'] = pullsecret
         self.params['openshift_version'] = version
-        self.params['high_availablity_mode'] = hamode
+        self.params['high_availability_mode'] = hamode
         self.params['cpu_architecture'] = cpuarchitecture
 
     def getParams(self):
+    
         return self.params
```

### Comparing `redhat_assisted_installer-0.0.3/PKG-INFO` & `redhat_assisted_installer-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: redhat-assisted-installer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python module to implement the RedHat Assisted Installer API
 Project-URL: Homepage, https://github.com/JustinBatchelor/red-hat-assisted-installer
 Project-URL: Issues, https://github.com/JustinBatchelor/red-hat-assisted-installer/issues
 Author-email: Justin Batchelor <justinrossbatchelor@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

