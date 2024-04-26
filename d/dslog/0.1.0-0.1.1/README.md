# Comparing `tmp/dslog-0.1.0.tar.gz` & `tmp/dslog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dslog-0.1.0.tar", last modified: Sat Apr 20 07:51:22 2024, max compression
+gzip compressed data, was "dslog-0.1.1.tar", last modified: Fri Apr 26 12:13:15 2024, max compression
```

## Comparing `dslog-0.1.0.tar` & `dslog-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 07:51:22.824982 dslog-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      679 2024-04-20 07:51:22.824982 dslog-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      399 2024-04-20 07:49:44.000000 dslog-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      530 2024-04-20 05:22:41.000000 dslog-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-20 07:51:22.824982 dslog-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 07:51:22.814982 dslog-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 07:51:22.824982 dslog-0.1.0/src/dslog/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      468 2024-04-20 07:42:14.000000 dslog-0.1.0/src/dslog/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1511 2024-04-20 07:48:00.000000 dslog-0.1.0/src/dslog/logger.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 07:51:22.824982 dslog-0.1.0/src/dslog/loggers/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-20 06:37:47.000000 dslog-0.1.0/src/dslog/loggers/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      502 2024-04-20 06:38:28.000000 dslog-0.1.0/src/dslog/loggers/loggers.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      543 2024-04-20 07:41:22.000000 dslog-0.1.0/src/dslog/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 07:51:22.824982 dslog-0.1.0/src/dslog/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-20 05:24:05.000000 dslog-0.1.0/src/dslog/util/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-04-20 05:23:58.000000 dslog-0.1.0/src/dslog/util/uvicorn.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 07:51:22.824982 dslog-0.1.0/src/dslog.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      679 2024-04-20 07:51:22.000000 dslog-0.1.0/src/dslog.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      329 2024-04-20 07:51:22.000000 dslog-0.1.0/src/dslog.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-20 07:51:22.000000 dslog-0.1.0/src/dslog.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-04-20 07:51:22.000000 dslog-0.1.0/src/dslog.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.084415 dslog-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-04-26 12:13:15.074415 dslog-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      399 2024-04-20 07:49:44.000000 dslog-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      544 2024-04-26 12:13:11.000000 dslog-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-26 12:13:15.084415 dslog-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.074415 dslog-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.074415 dslog-0.1.1/src/dslog/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      468 2024-04-20 07:42:14.000000 dslog-0.1.1/src/dslog/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1604 2024-04-26 12:12:47.000000 dslog-0.1.1/src/dslog/logger.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.074415 dslog-0.1.1/src/dslog/loggers/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-20 06:37:47.000000 dslog-0.1.1/src/dslog/loggers/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      502 2024-04-20 06:38:28.000000 dslog-0.1.1/src/dslog/loggers/loggers.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      543 2024-04-20 07:41:22.000000 dslog-0.1.1/src/dslog/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.074415 dslog-0.1.1/src/dslog/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-20 05:24:05.000000 dslog-0.1.1/src/dslog/util/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1018 2024-04-20 08:13:09.000000 dslog-0.1.1/src/dslog/util/uvicorn.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 12:13:15.074415 dslog-0.1.1/src/dslog.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-04-26 12:13:15.000000 dslog-0.1.1/src/dslog.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      361 2024-04-26 12:13:15.000000 dslog-0.1.1/src/dslog.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-26 12:13:15.000000 dslog-0.1.1/src/dslog.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       13 2024-04-26 12:13:15.000000 dslog-0.1.1/src/dslog.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-04-26 12:13:15.000000 dslog-0.1.1/src/dslog.egg-info/top_level.txt
```

### Comparing `dslog-0.1.0/pyproject.toml` & `dslog-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dslog"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Dead-simple logging: just function composition"
 dependencies = [
   
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/REPO.git"
 
-# [project.optional-dependencies]
+[project.optional-dependencies]
+rich = ["rich"]
 # test = [
 #   "pytest < 5.0.0",
 #   "pytest-cov[all]"
 # ]
```

### Comparing `dslog-0.1.0/src/dslog/logger.py` & `dslog-0.1.1/src/dslog/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,19 @@
   @abstractmethod
   def __call__(self, *objs, level: Level = 'INFO'):
     ...
 
   @classmethod
   def of(cls, handler: Handler) -> 'Logger':
     return LoggerOf(handler)
+
+  @classmethod
+  def rich(cls) -> 'Logger':
+    import rich
+    return LoggerOf(rich.print)
   
   @classmethod
   def empty(cls) -> 'Logger':
     """A logger that doesn't do anything"""
     return LoggerOf(lambda *_, **_kw: None)
 
   def limit(self, min_level: Level) -> 'Logger':
```

### Comparing `dslog-0.1.0/src/dslog/types.py` & `dslog-0.1.1/src/dslog/types.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.0/src/dslog/util/uvicorn.py` & `dslog-0.1.1/src/dslog/util/uvicorn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 def uvicorn_logconfig(prefix: str):
   return {
-  "version": 1,
-  "disable_existing_loggers": True,
-  "formatters": {
-    "custom": {
-      "()": "uvicorn.logging.DefaultFormatter",
-      "fmt": f"{prefix}%(levelprefix)s %(message)s",
-      "use_colors": True
+    "version": 1,
+    "disable_existing_loggers": False,
+    "formatters": {
+      "default": {
+        "()": "uvicorn.logging.DefaultFormatter",
+        "fmt": f"{prefix}%(levelprefix)s %(message)s",
+        "use_colors": None,
+      },
+      "access": {
+        "()": "uvicorn.logging.AccessFormatter",
+        "fmt": f'{prefix}%(levelprefix)s %(client_addr)s - "%(request_line)s" %(status_code)s',  # noqa: E501
+      },
     },
-  },
-  "handlers": {
-    "default": {
-      "formatter": "custom",
-      "class": "logging.StreamHandler",
-      "stream": "ext://sys.stdout",
+    "handlers": {
+      "default": {
+        "formatter": "default",
+        "class": "logging.StreamHandler",
+        "stream": "ext://sys.stderr",
+      },
+      "access": {
+        "formatter": "access",
+        "class": "logging.StreamHandler",
+        "stream": "ext://sys.stdout",
+      },
+    },
+    "loggers": {
+      "uvicorn": {"handlers": ["default"], "level": "INFO", "propagate": False},
+      "uvicorn.error": {"level": "INFO"},
+      "uvicorn.access": {"handlers": ["access"], "level": "INFO", "propagate": False},
     },
-  },
-  "loggers": {
-    "uvicorn": {"handlers": ["default"], "level": "INFO", "propagate": False },
-    "uvicorn.error": {"handlers": ["default"], "level": "INFO", "propagate": False },
-    "uvicorn.access": {"handlers": ["default"], "level": "INFO", "propagate": False },
-  }
   }
```

