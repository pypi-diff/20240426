# Comparing `tmp/gllogger-0.0.4.tar.gz` & `tmp/gllogger-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gllogger-0.0.4.tar", last modified: Sun Apr 14 12:00:33 2024, max compression
+gzip compressed data, was "gllogger-0.0.5.tar", last modified: Fri Apr 26 10:47:30 2024, max compression
```

## Comparing `gllogger-0.0.4.tar` & `gllogger-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 12:00:33.847736 gllogger-0.0.4/
--rw-rw-rw-   0        0        0     1674 2024-04-14 12:00:33.846428 gllogger-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2024-04-14 11:55:13.000000 gllogger-0.0.4/README.md
--rw-rw-rw-   0        0        0      384 2024-04-14 11:55:13.000000 gllogger-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 12:00:33.848447 gllogger-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 12:00:33.821378 gllogger-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-14 12:00:33.844382 gllogger-0.0.4/src/gllogger.egg-info/
--rw-rw-rw-   0        0        0     1674 2024-04-14 12:00:33.000000 gllogger-0.0.4/src/gllogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-14 12:00:33.000000 gllogger-0.0.4/src/gllogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 12:00:33.000000 gllogger-0.0.4/src/gllogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 12:00:33.000000 gllogger-0.0.4/src/gllogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    19750 2024-04-14 11:55:13.000000 gllogger-0.0.4/src/gllogger.py
-drwxrwxrwx   0        0        0        0 2024-04-14 12:00:33.842351 gllogger-0.0.4/test/
--rw-rw-rw-   0        0        0     5005 2024-04-14 11:55:13.000000 gllogger-0.0.4/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:47:30.651988 gllogger-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-26 10:47:30.651988 gllogger-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-26 10:47:26.000000 gllogger-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-26 10:47:26.000000 gllogger-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:47:30.651988 gllogger-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:47:30.647988 gllogger-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:47:30.651988 gllogger-0.0.5/src/gllogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-26 10:47:30.000000 gllogger-0.0.5/src/gllogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 10:47:30.000000 gllogger-0.0.5/src/gllogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:47:30.000000 gllogger-0.0.5/src/gllogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 10:47:30.000000 gllogger-0.0.5/src/gllogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 10:47:30.000000 gllogger-0.0.5/src/gllogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19750 2024-04-26 10:47:26.000000 gllogger-0.0.5/src/gllogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:47:30.647988 gllogger-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-26 10:47:26.000000 gllogger-0.0.5/test/test.py
```

### Comparing `gllogger-0.0.4/PKG-INFO` & `gllogger-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,75 @@
-Metadata-Version: 2.1
-Name: gllogger
-Version: 0.0.4
-Summary: gllogger
-Author-email: calm51 <calm51@protonmail.com>
-Project-URL: Homepage, https://github.com/calm51/gllogger
-Project-URL: Issues, https://github.com/calm51/gllogger/issues
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-```python3
-# NOTE: You should import gllogger before executing any other code.
-from gllogger import gL
-
-gL.getLogger(__name__)
-gL.setGlobalLevel(logging.DEBUG)
-
-...
-```
-
-```python3
-# You can log into the console,
-gL.init(gL.OT_console)
-
-# or you can pass logs into a function,
-def gL_function(text):
-    print(text)
-gL.setFunction(gL_function)
-gL.init(gL.OT_function)
-
-# or you can write logs to files.
-import os
-gL.setLogDir(os.path.join(os.getcwd(), "log", ))
-gL.init(gL.OT_logging)
-
-
-# Then, use the following function anywhere to log.
-gL.debugs("a", 1, True, )
-gL.infos()
-gL.warns()
-gL.errors()
-
-"""
-[DEBUG 00:00:00 main[15].<module>] a 1 True
-"""
-
-```
-
-```python3
-# You can use 'gL(Exception)' to enable logging of complete exception tracebacks,
-# and if you have 'better_exceptions' installed, the tracebacks will be even more detailed.
-# $ pip install better_exceptions
-
-try:
-    def f(a, b):
-        return a / b
-    f(1, 0)
-except ZeroDivisionError as e:
-    gL.warns(gL(e))
-
-"""
-[WARNING 00:00:00 main[10].<module>] Traceback (most recent call last):
-  File "/tmp/main.py", line 8, in <module>
-    f(1, 0)
-    └ <function f at 0x04E264A8>
-  File "/tmp/main.py", line 6, in f
-    return a / b
-           │   └ 0
-           └ 1
-"""
-
-```
+Metadata-Version: 2.1
+Name: gllogger
+Version: 0.0.5
+Summary: gllogger
+Author-email: calm51 <calm51@protonmail.com>
+Project-URL: Homepage, https://github.com/calm510/gllogger
+Project-URL: Issues, https://github.com/calm510/gllogger/issues
+Keywords: logger,global logger,logger hook,easy logger
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: better_exceptions
+
+```python3
+# NOTE: You should import gllogger before executing any other code.
+from gllogger import gL
+
+gL.getLogger(__name__)
+gL.setGlobalLevel(logging.DEBUG)
+
+...
+```
+
+```python3
+# You can log into the console,
+gL.init(gL.OT_console)
+
+# or you can pass logs into a function,
+def gL_function(text):
+    print(text)
+gL.setFunction(gL_function)
+gL.init(gL.OT_function)
+
+# or you can write logs to files.
+import os
+gL.setLogDir(os.path.join(os.getcwd(), "log", ))
+gL.init(gL.OT_logging)
+
+
+# Then, use the following function anywhere to log.
+gL.debugs("a", 1, True, )
+gL.infos()
+gL.warns()
+gL.errors()
+
+"""
+[DEBUG 00:00:00 main[15].<module>] a 1 True
+"""
+
+```
+
+```python3
+# You can use 'gL(Exception)' to enable logging of complete exception tracebacks,
+# and if you have 'better_exceptions' installed, the tracebacks will be even more detailed.
+# $ pip install better_exceptions
+
+try:
+    def f(a, b):
+        return a / b
+    f(1, 0)
+except ZeroDivisionError as e:
+    gL.warns(gL(e))
+
+"""
+[WARNING 00:00:00 main[10].<module>] Traceback (most recent call last):
+  File "/tmp/main.py", line 8, in <module>
+    f(1, 0)
+    └ <function f at 0x04E264A8>
+  File "/tmp/main.py", line 6, in f
+    return a / b
+           │   └ 0
+           └ 1
+"""
+
+```
```

### Comparing `gllogger-0.0.4/README.md` & `gllogger-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gllogger-0.0.4/src/gllogger.egg-info/PKG-INFO` & `gllogger-0.0.5/src/gllogger.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,75 @@
-Metadata-Version: 2.1
-Name: gllogger
-Version: 0.0.4
-Summary: gllogger
-Author-email: calm51 <calm51@protonmail.com>
-Project-URL: Homepage, https://github.com/calm51/gllogger
-Project-URL: Issues, https://github.com/calm51/gllogger/issues
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-```python3
-# NOTE: You should import gllogger before executing any other code.
-from gllogger import gL
-
-gL.getLogger(__name__)
-gL.setGlobalLevel(logging.DEBUG)
-
-...
-```
-
-```python3
-# You can log into the console,
-gL.init(gL.OT_console)
-
-# or you can pass logs into a function,
-def gL_function(text):
-    print(text)
-gL.setFunction(gL_function)
-gL.init(gL.OT_function)
-
-# or you can write logs to files.
-import os
-gL.setLogDir(os.path.join(os.getcwd(), "log", ))
-gL.init(gL.OT_logging)
-
-
-# Then, use the following function anywhere to log.
-gL.debugs("a", 1, True, )
-gL.infos()
-gL.warns()
-gL.errors()
-
-"""
-[DEBUG 00:00:00 main[15].<module>] a 1 True
-"""
-
-```
-
-```python3
-# You can use 'gL(Exception)' to enable logging of complete exception tracebacks,
-# and if you have 'better_exceptions' installed, the tracebacks will be even more detailed.
-# $ pip install better_exceptions
-
-try:
-    def f(a, b):
-        return a / b
-    f(1, 0)
-except ZeroDivisionError as e:
-    gL.warns(gL(e))
-
-"""
-[WARNING 00:00:00 main[10].<module>] Traceback (most recent call last):
-  File "/tmp/main.py", line 8, in <module>
-    f(1, 0)
-    └ <function f at 0x04E264A8>
-  File "/tmp/main.py", line 6, in f
-    return a / b
-           │   └ 0
-           └ 1
-"""
-
-```
+Metadata-Version: 2.1
+Name: gllogger
+Version: 0.0.5
+Summary: gllogger
+Author-email: calm51 <calm51@protonmail.com>
+Project-URL: Homepage, https://github.com/calm510/gllogger
+Project-URL: Issues, https://github.com/calm510/gllogger/issues
+Keywords: logger,global logger,logger hook,easy logger
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: better_exceptions
+
+```python3
+# NOTE: You should import gllogger before executing any other code.
+from gllogger import gL
+
+gL.getLogger(__name__)
+gL.setGlobalLevel(logging.DEBUG)
+
+...
+```
+
+```python3
+# You can log into the console,
+gL.init(gL.OT_console)
+
+# or you can pass logs into a function,
+def gL_function(text):
+    print(text)
+gL.setFunction(gL_function)
+gL.init(gL.OT_function)
+
+# or you can write logs to files.
+import os
+gL.setLogDir(os.path.join(os.getcwd(), "log", ))
+gL.init(gL.OT_logging)
+
+
+# Then, use the following function anywhere to log.
+gL.debugs("a", 1, True, )
+gL.infos()
+gL.warns()
+gL.errors()
+
+"""
+[DEBUG 00:00:00 main[15].<module>] a 1 True
+"""
+
+```
+
+```python3
+# You can use 'gL(Exception)' to enable logging of complete exception tracebacks,
+# and if you have 'better_exceptions' installed, the tracebacks will be even more detailed.
+# $ pip install better_exceptions
+
+try:
+    def f(a, b):
+        return a / b
+    f(1, 0)
+except ZeroDivisionError as e:
+    gL.warns(gL(e))
+
+"""
+[WARNING 00:00:00 main[10].<module>] Traceback (most recent call last):
+  File "/tmp/main.py", line 8, in <module>
+    f(1, 0)
+    └ <function f at 0x04E264A8>
+  File "/tmp/main.py", line 6, in f
+    return a / b
+           │   └ 0
+           └ 1
+"""
+
+```
```

### Comparing `gllogger-0.0.4/src/gllogger.py` & `gllogger-0.0.5/src/gllogger.py`

 * *Files identical despite different names*

