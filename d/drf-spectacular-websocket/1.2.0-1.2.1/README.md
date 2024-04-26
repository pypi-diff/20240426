# Comparing `tmp/drf_spectacular_websocket-1.2.0.tar.gz` & `tmp/drf_spectacular_websocket-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_spectacular_websocket-1.2.0.tar", last modified: Thu Apr 25 18:41:11 2024, max compression
+gzip compressed data, was "drf_spectacular_websocket-1.2.1.tar", last modified: Fri Apr 26 18:08:09 2024, max compression
```

## Comparing `drf_spectacular_websocket-1.2.0.tar` & `drf_spectacular_websocket-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:41:11.778108 drf_spectacular_websocket-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-25 18:41:11.778108 drf_spectacular_websocket-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:41:11.778108 drf_spectacular_websocket-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:41:11.774108 drf_spectacular_websocket-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:41:11.774108 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:41:11.778108 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/consumer_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-25 18:41:01.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:41:11.778108 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-25 18:41:11.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 18:41:11.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:41:11.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-25 18:41:11.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 18:41:11.000000 drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.153668 drf_spectacular_websocket-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-26 18:08:09.153668 drf_spectacular_websocket-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:08:09.153668 drf_spectacular_websocket-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.145668 drf_spectacular_websocket-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.149668 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.149668 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/consumer_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.149668 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-26 18:08:09.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 18:08:09.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:08:09.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 18:08:09.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 18:08:09.000000 drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:08:09.149668 drf_spectacular_websocket-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 18:08:05.000000 drf_spectacular_websocket-1.2.1/tests/test_schema.py
```

### Comparing `drf_spectacular_websocket-1.2.0/LICENSE` & `drf_spectacular_websocket-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.0/PKG-INFO` & `drf_spectacular_websocket-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: drf_spectacular_websocket
-Version: 1.2.0
-Summary: Extend schema decorator for Channels
+Version: 1.2.1
+Summary: Extend websocket schema decorator for Django Channels
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -35,39 +35,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Code Generators
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=4.2.11
 Requires-Dist: djangorestframework>=3.14.0
 Requires-Dist: drf-spectacular>=0.27.2
 Requires-Dist: drf-spectacular-sidecar>=2024.4.1
-Requires-Dist: channels>=4.1.0
+Requires-Dist: channels>=4.0.0
+Provides-Extra: dev
+Requires-Dist: pre-commit>=3.5.0; extra == "dev"
+Requires-Dist: ruff==0.4.1; extra == "dev"
+Requires-Dist: pytest>=7.0.1; extra == "dev"
+Provides-Extra: ci
+Requires-Dist: ruff==0.4.1; extra == "ci"
+Requires-Dist: pytest>=7.0.1; extra == "ci"
 
-# Extend schema decorator for Channels
+# Extend websocket schema decorator for Django Channels
 
 
 > Provides [extend_ws_schema](#About-decorator) decorator to documentation [Cunsumer](https://channels.readthedocs.io/en/latest/topics/consumers.html) methods from [channels](https://github.com/django/channels) just like it does [drf-spectacular](https://github.com/tfranzel/drf-spectacular)
 
 
-## Requirements
-- django>=4.2.11
-- djangorestframework>=3.14.0
-- drf-spectacular>=0.27.2
-- drf-spectacular-sidecar>=2024.4.1
-- channels>=4.1.0
-
-
 ## Install
 1. `pip install drf-spectacular-websocket`
 2. `python manage.py collectstatic` for sidecar static
 3. Add app name to `INSTALLED_APPS`
 ```python
 INSTALLED_APPS = [
     # drf_spectacular_websocket must be higher than drf_spectacular
```

### Comparing `drf_spectacular_websocket-1.2.0/README.md` & `drf_spectacular_websocket-1.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,13 @@
-# Extend schema decorator for Channels
+# Extend websocket schema decorator for Django Channels
 
 
 > Provides [extend_ws_schema](#About-decorator) decorator to documentation [Cunsumer](https://channels.readthedocs.io/en/latest/topics/consumers.html) methods from [channels](https://github.com/django/channels) just like it does [drf-spectacular](https://github.com/tfranzel/drf-spectacular)
 
 
-## Requirements
-- django>=4.2.11
-- djangorestframework>=3.14.0
-- drf-spectacular>=0.27.2
-- drf-spectacular-sidecar>=2024.4.1
-- channels>=4.1.0
-
-
 ## Install
 1. `pip install drf-spectacular-websocket`
 2. `python manage.py collectstatic` for sidecar static
 3. Add app name to `INSTALLED_APPS`
 ```python
 INSTALLED_APPS = [
     # drf_spectacular_websocket must be higher than drf_spectacular
```

### Comparing `drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/decorators.py` & `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/decorators.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/consumer_schema.py` & `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/consumer_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from drf_spectacular.openapi import AutoSchema
 from drf_spectacular.plumbing import (
     build_media_type_object,
     force_instance,
     is_list_serializer,
     is_serializer,
 )
```

### Comparing `drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/schemas/schema.py` & `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/schemas/schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-from collections.abc import Callable
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 from channels.routing import URLRouter
 from django.conf import settings
 from django.contrib.admindocs.views import simplify_regex
 from django.utils.module_loading import import_string
 from drf_spectacular.generators import SchemaGenerator
 
 from .consumer_schema import NotReadyError
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
 
 class WsSchemaGenerator(SchemaGenerator):
     """"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.prepared = {'request': {}, 'response': {}}
```

### Comparing `drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket/settings.py` & `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket/settings.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/PKG-INFO` & `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: drf_spectacular_websocket
-Version: 1.2.0
-Summary: Extend schema decorator for Channels
+Version: 1.2.1
+Summary: Extend websocket schema decorator for Django Channels
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -35,39 +35,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Code Generators
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=4.2.11
 Requires-Dist: djangorestframework>=3.14.0
 Requires-Dist: drf-spectacular>=0.27.2
 Requires-Dist: drf-spectacular-sidecar>=2024.4.1
-Requires-Dist: channels>=4.1.0
+Requires-Dist: channels>=4.0.0
+Provides-Extra: dev
+Requires-Dist: pre-commit>=3.5.0; extra == "dev"
+Requires-Dist: ruff==0.4.1; extra == "dev"
+Requires-Dist: pytest>=7.0.1; extra == "dev"
+Provides-Extra: ci
+Requires-Dist: ruff==0.4.1; extra == "ci"
+Requires-Dist: pytest>=7.0.1; extra == "ci"
 
-# Extend schema decorator for Channels
+# Extend websocket schema decorator for Django Channels
 
 
 > Provides [extend_ws_schema](#About-decorator) decorator to documentation [Cunsumer](https://channels.readthedocs.io/en/latest/topics/consumers.html) methods from [channels](https://github.com/django/channels) just like it does [drf-spectacular](https://github.com/tfranzel/drf-spectacular)
 
 
-## Requirements
-- django>=4.2.11
-- djangorestframework>=3.14.0
-- drf-spectacular>=0.27.2
-- drf-spectacular-sidecar>=2024.4.1
-- channels>=4.1.0
-
-
 ## Install
 1. `pip install drf-spectacular-websocket`
 2. `python manage.py collectstatic` for sidecar static
 3. Add app name to `INSTALLED_APPS`
 ```python
 INSTALLED_APPS = [
     # drf_spectacular_websocket must be higher than drf_spectacular
```

### Comparing `drf_spectacular_websocket-1.2.0/src/drf_spectacular_websocket.egg-info/SOURCES.txt` & `drf_spectacular_websocket-1.2.1/src/drf_spectacular_websocket.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 src/drf_spectacular_websocket.egg-info/PKG-INFO
 src/drf_spectacular_websocket.egg-info/SOURCES.txt
 src/drf_spectacular_websocket.egg-info/dependency_links.txt
 src/drf_spectacular_websocket.egg-info/requires.txt
 src/drf_spectacular_websocket.egg-info/top_level.txt
 src/drf_spectacular_websocket/schemas/__init__.py
 src/drf_spectacular_websocket/schemas/consumer_schema.py
-src/drf_spectacular_websocket/schemas/schema.py
+src/drf_spectacular_websocket/schemas/schema.py
+tests/test_schema.py
```

