# Comparing `tmp/aikicore-1.0.0a3.tar.gz` & `tmp/aikicore-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikicore-1.0.0a3.tar", last modified: Wed Apr 24 22:12:20 2024, max compression
+gzip compressed data, was "aikicore-1.0.0a4.tar", last modified: Thu Apr 25 22:52:31 2024, max compression
```

## Comparing `aikicore-1.0.0a3.tar` & `aikicore-1.0.0a4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-24 22:12:20.629913 aikicore-1.0.0a3/
--rw-r--r--   0 ashatz     (501) staff       (20)     1509 2024-04-23 22:54:22.000000 aikicore-1.0.0a3/LICENSE
--rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-24 22:12:20.629679 aikicore-1.0.0a3/PKG-INFO
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-24 22:12:20.627602 aikicore-1.0.0a3/aikicore/
--rw-r--r--   0 ashatz     (501) staff       (20)     2503 2024-04-24 01:08:35.000000 aikicore-1.0.0a3/aikicore/__init__.py
--rw-r--r--   0 ashatz     (501) staff       (20)       55 2024-04-23 22:57:31.000000 aikicore-1.0.0a3/aikicore/activity.py
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-24 22:12:20.629211 aikicore-1.0.0a3/aikicore/config/
--rw-r--r--   0 ashatz     (501) staff       (20)     3146 2024-04-24 21:33:16.000000 aikicore-1.0.0a3/aikicore/config/__init__.py
--rw-r--r--   0 ashatz     (501) staff       (20)      306 2024-04-23 22:57:31.000000 aikicore-1.0.0a3/aikicore/config/json.py
--rw-r--r--   0 ashatz     (501) staff       (20)      407 2024-04-23 22:57:31.000000 aikicore-1.0.0a3/aikicore/config/yaml.py
--rw-r--r--   0 ashatz     (501) staff       (20)      334 2024-04-23 22:57:31.000000 aikicore-1.0.0a3/aikicore/constants.py
--rw-r--r--   0 ashatz     (501) staff       (20)      575 2024-04-24 01:05:56.000000 aikicore-1.0.0a3/aikicore/containers.py
--rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-23 22:57:31.000000 aikicore-1.0.0a3/aikicore/domain.py
--rw-r--r--   0 ashatz     (501) staff       (20)     1571 2024-04-23 22:57:31.000000 aikicore-1.0.0a3/aikicore/error.py
--rw-r--r--   0 ashatz     (501) staff       (20)     5762 2024-04-24 22:01:58.000000 aikicore-1.0.0a3/aikicore/routing.py
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-24 22:12:20.629438 aikicore-1.0.0a3/aikicore.egg-info/
--rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-24 22:12:20.000000 aikicore-1.0.0a3/aikicore.egg-info/PKG-INFO
--rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-24 22:12:20.000000 aikicore-1.0.0a3/aikicore.egg-info/SOURCES.txt
--rw-r--r--   0 ashatz     (501) staff       (20)        1 2024-04-24 22:12:20.000000 aikicore-1.0.0a3/aikicore.egg-info/dependency_links.txt
--rw-r--r--   0 ashatz     (501) staff       (20)       32 2024-04-24 22:12:20.000000 aikicore-1.0.0a3/aikicore.egg-info/requires.txt
--rw-r--r--   0 ashatz     (501) staff       (20)        9 2024-04-24 22:12:20.000000 aikicore-1.0.0a3/aikicore.egg-info/top_level.txt
--rw-r--r--   0 ashatz     (501) staff       (20)       38 2024-04-24 22:12:20.629960 aikicore-1.0.0a3/setup.cfg
--rw-r--r--   0 ashatz     (501) staff       (20)      657 2024-04-24 22:08:45.000000 aikicore-1.0.0a3/setup.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-25 22:52:31.996775 aikicore-1.0.0a4/
+-rw-r--r--   0 ashatz     (501) staff       (20)     1509 2024-04-23 22:54:22.000000 aikicore-1.0.0a4/LICENSE
+-rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-25 22:52:31.996558 aikicore-1.0.0a4/PKG-INFO
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-25 22:52:31.994487 aikicore-1.0.0a4/aikicore/
+-rw-r--r--   0 ashatz     (501) staff       (20)     2503 2024-04-24 01:08:35.000000 aikicore-1.0.0a4/aikicore/__init__.py
+-rw-r--r--   0 ashatz     (501) staff       (20)       55 2024-04-23 22:57:31.000000 aikicore-1.0.0a4/aikicore/activity.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-25 22:52:31.996160 aikicore-1.0.0a4/aikicore/config/
+-rw-r--r--   0 ashatz     (501) staff       (20)     3115 2024-04-25 22:51:55.000000 aikicore-1.0.0a4/aikicore/config/__init__.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      306 2024-04-23 22:57:31.000000 aikicore-1.0.0a4/aikicore/config/json.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      407 2024-04-23 22:57:31.000000 aikicore-1.0.0a4/aikicore/config/yaml.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      334 2024-04-23 22:57:31.000000 aikicore-1.0.0a4/aikicore/constants.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      575 2024-04-24 01:05:56.000000 aikicore-1.0.0a4/aikicore/containers.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-23 22:57:31.000000 aikicore-1.0.0a4/aikicore/domain.py
+-rw-r--r--   0 ashatz     (501) staff       (20)     1784 2024-04-25 22:40:31.000000 aikicore-1.0.0a4/aikicore/error.py
+-rw-r--r--   0 ashatz     (501) staff       (20)     5762 2024-04-24 22:01:58.000000 aikicore-1.0.0a4/aikicore/routing.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-25 22:52:31.996354 aikicore-1.0.0a4/aikicore.egg-info/
+-rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-25 22:52:31.000000 aikicore-1.0.0a4/aikicore.egg-info/PKG-INFO
+-rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-25 22:52:31.000000 aikicore-1.0.0a4/aikicore.egg-info/SOURCES.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)        1 2024-04-25 22:52:31.000000 aikicore-1.0.0a4/aikicore.egg-info/dependency_links.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)       32 2024-04-25 22:52:31.000000 aikicore-1.0.0a4/aikicore.egg-info/requires.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)        9 2024-04-25 22:52:31.000000 aikicore-1.0.0a4/aikicore.egg-info/top_level.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)       38 2024-04-25 22:52:31.996822 aikicore-1.0.0a4/setup.cfg
+-rw-r--r--   0 ashatz     (501) staff       (20)      657 2024-04-25 22:52:11.000000 aikicore-1.0.0a4/setup.py
```

### Comparing `aikicore-1.0.0a3/LICENSE` & `aikicore-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a3/aikicore/__init__.py` & `aikicore-1.0.0a4/aikicore/__init__.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a3/aikicore/config/__init__.py` & `aikicore-1.0.0a4/aikicore/config/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     status_code = t.IntType(default=400, choices=[400, 401, 403, 404]) # Status codes include Bad Request, Unauthorized, Forbidden, and Not Found
 
 
 class AppConfiguration(Model):
     errors = t.DictType(t.ModelType(ErrorConfiguration), default={})
 
 class InterfaceConfiguration(Model):
-    type = t.StringType(required=True, choices=['cli', 'rest_flask'])
+    type = t.StringType(required=True)
 
 class AppConfiguration(Model):
     errors = t.DictType(t.ModelType(ErrorConfiguration), default={})
     features = t.ModelType(AppFeaturesConfiguration)
     interfaces = t.DictType(t.ModelType(InterfaceConfiguration), default=[])
```

### Comparing `aikicore-1.0.0a3/aikicore/containers.py` & `aikicore-1.0.0a4/aikicore/containers.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a3/aikicore/error.py` & `aikicore-1.0.0a4/aikicore/error.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,22 @@
 
     def add(self, error: Error):
         try:
             self.__errors[error.error_name] = error
             setattr(self, error.error_name, error)
         except:
             return
+        
+class DomainError(Exception):
+
+    def __init__(self, model: str, method: str, code: str, *data):
+        self.model = model
+        self.method = method
+        self.code = code
+        self.data = data
 
 class AppError(Exception):
 
     def __init__(self, error: Error, lang: str = 'en_US'):
         super().__init__(self)
         self.error_code = error.error_code
         self.message = error.message[lang]
```

### Comparing `aikicore-1.0.0a3/aikicore/routing.py` & `aikicore-1.0.0a4/aikicore/routing.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a3/setup.py` & `aikicore-1.0.0a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 config = {
     'description': 'The Core Library for the Spirit of Harmony',
     'author': 'Andrew Shatz',
     'url': r'https://github.com/Great-Strength-Studios/aikicore',
     'download_url': r'https://github.com/Great-Strength-Studios/aikicore',
     'author_email': 'andrew@greatstrength.me',
-    'version': '1.0.0-alpha.3',
+    'version': '1.0.0-alpha.4',
     'license': 'BSD 3',
     'install_requires': [
         'schematics>=2.1.1',
         'pyyaml>=6.0.1'
     ],
     'packages': [
         'aikicore',
```

