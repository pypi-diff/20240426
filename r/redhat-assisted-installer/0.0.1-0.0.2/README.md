# Comparing `tmp/redhat_assisted_installer-0.0.1.tar.gz` & `tmp/redhat_assisted_installer-0.0.2.tar.gz`

## Comparing `redhat_assisted_installer-0.0.1.tar` & `redhat_assisted_installer-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/src/redhat_assisted_installer/__init__.py
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/src/redhat_assisted_installer/assistedinstaller.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/src/redhat_assisted_installer/lib/logging.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/src/redhat_assisted_installer/lib/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/src/redhat_assisted_installer/lib/schema/__init__.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/src/redhat_assisted_installer/lib/schema/createParams.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/tests/createInfraEnvs.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/tests/deleteInfraEnvs.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/tests/getInfraEnv.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/README.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/src/redhat_assisted_installer/__init__.py
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/src/redhat_assisted_installer/assistedinstaller.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/src/redhat_assisted_installer/lib/logging.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/src/redhat_assisted_installer/lib/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/src/redhat_assisted_installer/lib/schema/__init__.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/src/redhat_assisted_installer/lib/schema/createParams.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/tests/createInfraEnvs.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/tests/deleteInfraEnvs.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/tests/getInfraEnv.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 redhat_assisted_installer-0.0.2/PKG-INFO
```

### Comparing `redhat_assisted_installer-0.0.1/src/redhat_assisted_installer/assistedinstaller.py` & `redhat_assisted_installer-0.0.2/src/redhat_assisted_installer/assistedinstaller.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.1/src/redhat_assisted_installer/lib/tools.py` & `redhat_assisted_installer-0.0.2/src/redhat_assisted_installer/lib/tools.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.1/src/redhat_assisted_installer/lib/schema/createParams.py` & `redhat_assisted_installer-0.0.2/src/redhat_assisted_installer/lib/schema/createParams.py`

 * *Files identical despite different names*

### Comparing `redhat_assisted_installer-0.0.1/pyproject.toml` & `redhat_assisted_installer-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "redhat-assisted-installer"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Justin Batchelor", email="justinrossbatchelor@gmail.com" },
 ]
 description = "Python module to implement the RedHat Assisted Installer API"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `redhat_assisted_installer-0.0.1/PKG-INFO` & `redhat_assisted_installer-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: redhat-assisted-installer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python module to implement the RedHat Assisted Installer API
 Project-URL: Homepage, https://github.com/JustinBatchelor/red-hat-assisted-installer
 Project-URL: Issues, https://github.com/JustinBatchelor/red-hat-assisted-installer/issues
 Author-email: Justin Batchelor <justinrossbatchelor@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

