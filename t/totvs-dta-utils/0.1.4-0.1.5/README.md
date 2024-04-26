# Comparing `tmp/totvs-dta-utils-0.1.4.tar.gz` & `tmp/totvs-dta-utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totvs-dta-utils-0.1.4.tar", last modified: Thu Apr 25 17:29:44 2024, max compression
+gzip compressed data, was "totvs-dta-utils-0.1.5.tar", last modified: Fri Apr 26 14:43:27 2024, max compression
```

## Comparing `totvs-dta-utils-0.1.4.tar` & `totvs-dta-utils-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/dta_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/dta_utils/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/services/dta_chat_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/services/dta_observer_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/services/dta_proxy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/services/dta_tracer_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 17:29:43.000000 totvs-dta-utils-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-25 17:29:43.000000 totvs-dta-utils-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-25 17:29:44.000000 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-25 17:29:44.000000 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:29:44.000000 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 17:29:44.000000 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 17:29:44.000000 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:43:27.130700 totvs-dta-utils-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-26 14:43:27.130700 totvs-dta-utils-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-26 14:43:25.000000 totvs-dta-utils-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:43:27.126700 totvs-dta-utils-0.1.5/dta_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-26 14:43:25.000000 totvs-dta-utils-0.1.5/dta_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:43:27.126700 totvs-dta-utils-0.1.5/dta_utils/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:43:25.000000 totvs-dta-utils-0.1.5/dta_utils/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-26 14:43:25.000000 totvs-dta-utils-0.1.5/dta_utils/services/dta_chat_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-26 14:43:25.000000 totvs-dta-utils-0.1.5/dta_utils/services/dta_observer_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-26 14:43:25.000000 totvs-dta-utils-0.1.5/dta_utils/services/dta_proxy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-26 14:43:25.000000 totvs-dta-utils-0.1.5/dta_utils/services/dta_tracer_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 14:43:25.000000 totvs-dta-utils-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:43:27.130700 totvs-dta-utils-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-26 14:43:25.000000 totvs-dta-utils-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:43:27.130700 totvs-dta-utils-0.1.5/totvs_dta_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-26 14:43:27.000000 totvs-dta-utils-0.1.5/totvs_dta_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-26 14:43:27.000000 totvs-dta-utils-0.1.5/totvs_dta_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:43:27.000000 totvs-dta-utils-0.1.5/totvs_dta_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 14:43:27.000000 totvs-dta-utils-0.1.5/totvs_dta_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 14:43:27.000000 totvs-dta-utils-0.1.5/totvs_dta_utils.egg-info/top_level.txt
```

### Comparing `totvs-dta-utils-0.1.4/PKG-INFO` & `totvs-dta-utils-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totvs-dta-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Lib for integration with DTA services
 Home-page: https://github.com/totvs-ai/dta-utils-python
 Author: TotvsLabs
 Author-email: info@totvs.ai
 Keywords: dta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `totvs-dta-utils-0.1.4/README.md` & `totvs-dta-utils-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `totvs-dta-utils-0.1.4/dta_utils/services/dta_chat_service.py` & `totvs-dta-utils-0.1.5/dta_utils/services/dta_chat_service.py`

 * *Files identical despite different names*

### Comparing `totvs-dta-utils-0.1.4/dta_utils/services/dta_observer_service.py` & `totvs-dta-utils-0.1.5/dta_utils/services/dta_observer_service.py`

 * *Files identical despite different names*

### Comparing `totvs-dta-utils-0.1.4/dta_utils/services/dta_proxy_service.py` & `totvs-dta-utils-0.1.5/dta_utils/services/dta_proxy_service.py`

 * *Files identical despite different names*

### Comparing `totvs-dta-utils-0.1.4/dta_utils/services/dta_tracer_service.py` & `totvs-dta-utils-0.1.5/dta_utils/services/dta_tracer_service.py`

 * *Files identical despite different names*

### Comparing `totvs-dta-utils-0.1.4/setup.py` & `totvs-dta-utils-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = rf.read()
 
 requirements = ["langfuse==2.*"]
 
 setup(
     name="totvs-dta-utils",
     author="TotvsLabs",
-    version="0.1.4",
+    version="0.1.5",
     author_email="info@totvs.ai",
     python_requires=">=3.10",
     description="Lib for integration with DTA services",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     include_package_data=True,
```

### Comparing `totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/PKG-INFO` & `totvs-dta-utils-0.1.5/totvs_dta_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totvs-dta-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Lib for integration with DTA services
 Home-page: https://github.com/totvs-ai/dta-utils-python
 Author: TotvsLabs
 Author-email: info@totvs.ai
 Keywords: dta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

