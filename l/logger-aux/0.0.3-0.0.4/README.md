# Comparing `tmp/logger_aux-0.0.3.tar.gz` & `tmp/logger_aux-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_aux-0.0.3.tar", last modified: Fri Apr 26 08:05:18 2024, max compression
+gzip compressed data, was "logger_aux-0.0.4.tar", last modified: Fri Apr 26 09:24:36 2024, max compression
```

## Comparing `logger_aux-0.0.3.tar` & `logger_aux-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 08:05:18.459385 logger_aux-0.0.3/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     8403 2024-04-26 08:05:18.459385 logger_aux-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7603 2024-04-26 08:04:07.000000 logger_aux-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 08:05:18.451516 logger_aux-0.0.3/logger_aux/
--rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.3/logger_aux/__init__.py
--rw-rw-rw-   0        0        0     6114 2024-04-26 07:44:47.000000 logger_aux-0.0.3/logger_aux/main.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:05:18.458384 logger_aux-0.0.3/logger_aux.egg-info/
--rw-rw-rw-   0        0        0     8403 2024-04-26 08:05:18.000000 logger_aux-0.0.3/logger_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-26 08:05:18.000000 logger_aux-0.0.3/logger_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 08:05:18.000000 logger_aux-0.0.3/logger_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 08:05:18.000000 logger_aux-0.0.3/logger_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 08:05:18.460384 logger_aux-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-04-26 07:47:41.000000 logger_aux-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:24:36.029356 logger_aux-0.0.4/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     8484 2024-04-26 09:24:36.029356 logger_aux-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7684 2024-04-26 09:23:58.000000 logger_aux-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 09:24:36.021229 logger_aux-0.0.4/logger_aux/
+-rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.4/logger_aux/__init__.py
+-rw-rw-rw-   0        0        0     6108 2024-04-26 09:12:24.000000 logger_aux-0.0.4/logger_aux/main.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:24:36.028131 logger_aux-0.0.4/logger_aux.egg-info/
+-rw-rw-rw-   0        0        0     8484 2024-04-26 09:24:35.000000 logger_aux-0.0.4/logger_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-26 09:24:36.000000 logger_aux-0.0.4/logger_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 09:24:36.000000 logger_aux-0.0.4/logger_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 09:24:36.000000 logger_aux-0.0.4/logger_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 09:24:36.031503 logger_aux-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-04-26 07:47:41.000000 logger_aux-0.0.4/setup.py
```

### Comparing `logger_aux-0.0.3/LICENSE` & `logger_aux-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `logger_aux-0.0.3/PKG-INFO` & `logger_aux-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,8 @@
-Metadata-Version: 2.1
-Name: logger_aux
-Version: 0.0.3
-Summary: simple logging
-Home-page: https://github.com/centroid457/
-Author: Andrei Starichenko
-Author-email: centroid@mail.ru
-Project-URL: Source, https://github.com/centroid457/logger_aux
-Keywords: logger
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Typing :: Typed
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# logger_aux (v0.0.3)
+# logger_aux (v0.0.4)
 
 ## DESCRIPTION_SHORT
 simple logging
 
 ## DESCRIPTION_LONG
 designed for DRY simple/easy usage logging
 
@@ -61,15 +39,15 @@
 ------------------------------
 ### 1. example1.py
 ```python
 from logger_aux import *
 from object_info import ObjectInfo
 
 
-# NAMES -----------------------
+# USAGE-1=DIRECT ===================================
 logger0 = Logger()
 # ObjectInfo(logger0.LOGGER).print()
 
 # logger0.LOGGER.debug()    # TypeError: Logger.debug() missing 1 required positional argument: 'msg'
 logger0.LOGGER.debug(None)  # OK
 logger0.LOGGER.debug(True)  # OK
 logger0.LOGGER.debug("")    # OK
@@ -89,15 +67,15 @@
 logger_dir = Logger("logger_dir", "c:\\1")
 logger_dir.LOGGER.debug("hello_dir")
 
 print(f"{logger_dir.LOG_DIRPATH=}")
 print(f"{logger_dir.LOG_FILEPATH=}")
 
 
-# NESTING -----------------------
+# USAGE-2=NESTING ===================================
 class Example(Logger):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def meth(self):
         self.LOGGER.debug("hello123")
 
@@ -106,65 +84,65 @@
 
 # ObjectInfo(logger0.LOGGER).print()
 ```
 
 ------------------------------
 ### 2. logger__Example.log
 ```
-2024-04-26 10:49:39,602[DEBUG]Example(main.py).__init__(line145)/thread6888::====================================================================================================
-2024-04-26 10:49:39,602[DEBUG]Example(main.py).__init__(line148)/thread6888::[Logger.Example] start STREAM
-2024-04-26 10:49:39,603[DEBUG]Example(main.py).__init__(line151)/thread6888::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
-2024-04-26 10:49:39,604[DEBUG]Example(example1.py).meth(line39)/thread6888::hello123
+2024-04-26 12:12:34,977[DEBUG]Example(main.py).__init__(line145)/thread21536::====================================================================================================
+2024-04-26 12:12:34,977[DEBUG]Example(main.py).__init__(line148)/thread21536::[Logger.Example] start STREAM
+2024-04-26 12:12:34,977[DEBUG]Example(main.py).__init__(line151)/thread21536::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
+2024-04-26 12:12:34,977[DEBUG]Example(example1.py).meth(line39)/thread21536::hello123
 ```
 
 ------------------------------
 ### 3. logger__logger_first.log
 ```
-2024-04-26 10:49:39,589[DEBUG]logger_first(main.py).__init__(line145)/thread6888::====================================================================================================
-2024-04-26 10:49:39,589[DEBUG]logger_first(main.py).__init__(line148)/thread6888::[Logger.logger_first] start STREAM
-2024-04-26 10:49:39,589[DEBUG]logger_first(main.py).__init__(line151)/thread6888::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
-2024-04-26 10:49:39,589[DEBUG]logger_first(example1.py).<module>(line16)/thread6888::hello1-1
-2024-04-26 10:49:39,594[DEBUG]logger_first(example1.py).<module>(line22)/thread6888::hello1-2
+2024-04-26 12:12:34,970[DEBUG]logger_first(main.py).__init__(line145)/thread21536::====================================================================================================
+2024-04-26 12:12:34,970[DEBUG]logger_first(main.py).__init__(line148)/thread21536::[Logger.logger_first] start STREAM
+2024-04-26 12:12:34,971[DEBUG]logger_first(main.py).__init__(line151)/thread21536::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
+2024-04-26 12:12:34,971[DEBUG]logger_first(example1.py).<module>(line16)/thread21536::hello1-1
+2024-04-26 12:12:34,974[DEBUG]logger_first(example1.py).<module>(line22)/thread21536::hello1-2
 ```
 
 ------------------------------
 ### 4. logger__logger_second.log
 ```
-2024-04-26 10:49:39,592[DEBUG]logger_second(main.py).__init__(line145)/thread6888::====================================================================================================
-2024-04-26 10:49:39,592[DEBUG]logger_second(main.py).__init__(line148)/thread6888::[Logger.logger_second] start STREAM
-2024-04-26 10:49:39,593[DEBUG]logger_second(main.py).__init__(line151)/thread6888::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
-2024-04-26 10:49:39,593[DEBUG]logger_second(example1.py).<module>(line19)/thread6888::hello2-1
-2024-04-26 10:49:39,595[DEBUG]logger_second(example1.py).<module>(line23)/thread6888::hello2-2
+2024-04-26 12:12:34,972[DEBUG]logger_second(main.py).__init__(line145)/thread21536::====================================================================================================
+2024-04-26 12:12:34,973[DEBUG]logger_second(main.py).__init__(line148)/thread21536::[Logger.logger_second] start STREAM
+2024-04-26 12:12:34,973[DEBUG]logger_second(main.py).__init__(line151)/thread21536::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
+2024-04-26 12:12:34,973[DEBUG]logger_second(example1.py).<module>(line19)/thread21536::hello2-1
+2024-04-26 12:12:34,974[DEBUG]logger_second(example1.py).<module>(line23)/thread21536::hello2-2
 ```
 
 ------------------------------
 ### 5. logger__root.log
 ```
-2024-04-26 10:49:39,583[DEBUG]root(main.py).__init__(line145)/thread6888::====================================================================================================
-2024-04-26 10:49:39,584[DEBUG]root(main.py).__init__(line148)/thread6888::[Logger.root] start STREAM
-2024-04-26 10:49:39,587[DEBUG]root(main.py).__init__(line151)/thread6888::[Logger.root] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__root.log]
-2024-04-26 10:49:39,587[DEBUG]root(example1.py).<module>(line10)/thread6888::None
-2024-04-26 10:49:39,587[DEBUG]root(example1.py).<module>(line11)/thread6888::True
-2024-04-26 10:49:39,588[DEBUG]root(example1.py).<module>(line12)/thread6888::
-2024-04-26 10:49:39,588[DEBUG]root(example1.py).<module>(line13)/thread6888::hello0-1
-2024-04-26 10:49:39,589[DEBUG]logger_first(main.py).__init__(line145)/thread6888::====================================================================================================
-2024-04-26 10:49:39,589[DEBUG]logger_first(main.py).__init__(line148)/thread6888::[Logger.logger_first] start STREAM
-2024-04-26 10:49:39,589[DEBUG]logger_first(main.py).__init__(line151)/thread6888::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
-2024-04-26 10:49:39,589[DEBUG]logger_first(example1.py).<module>(line16)/thread6888::hello1-1
-2024-04-26 10:49:39,592[DEBUG]logger_second(main.py).__init__(line145)/thread6888::====================================================================================================
-2024-04-26 10:49:39,592[DEBUG]logger_second(main.py).__init__(line148)/thread6888::[Logger.logger_second] start STREAM
-2024-04-26 10:49:39,593[DEBUG]logger_second(main.py).__init__(line151)/thread6888::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
-2024-04-26 10:49:39,593[DEBUG]logger_second(example1.py).<module>(line19)/thread6888::hello2-1
-2024-04-26 10:49:39,594[DEBUG]root(example1.py).<module>(line21)/thread6888::hello0-2
-2024-04-26 10:49:39,594[DEBUG]logger_first(example1.py).<module>(line22)/thread6888::hello1-2
-2024-04-26 10:49:39,595[DEBUG]logger_second(example1.py).<module>(line23)/thread6888::hello2-2
-2024-04-26 10:49:39,596[DEBUG]logger_dir(main.py).__init__(line145)/thread6888::====================================================================================================
-2024-04-26 10:49:39,596[DEBUG]logger_dir(main.py).__init__(line148)/thread6888::[Logger.logger_dir] start STREAM
-2024-04-26 10:49:39,598[DEBUG]logger_dir(main.py).__init__(line151)/thread6888::[Logger.logger_dir] start FILE=[c:\1\logger__logger_dir.log]
-2024-04-26 10:49:39,599[DEBUG]logger_dir(example1.py).<module>(line27)/thread6888::hello_dir
-2024-04-26 10:49:39,602[DEBUG]Example(main.py).__init__(line145)/thread6888::====================================================================================================
-2024-04-26 10:49:39,602[DEBUG]Example(main.py).__init__(line148)/thread6888::[Logger.Example] start STREAM
-2024-04-26 10:49:39,603[DEBUG]Example(main.py).__init__(line151)/thread6888::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
-2024-04-26 10:49:39,604[DEBUG]Example(example1.py).meth(line39)/thread6888::hello123
+2024-04-26 12:12:34,965[DEBUG]root(main.py).__init__(line145)/thread21536::====================================================================================================
+2024-04-26 12:12:34,965[DEBUG]root(main.py).__init__(line148)/thread21536::[Logger.root] start STREAM
+2024-04-26 12:12:34,965[DEBUG]root(main.py).__init__(line151)/thread21536::[Logger.root] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__root.log]
+2024-04-26 12:12:34,965[DEBUG]root(example1.py).<module>(line10)/thread21536::None
+2024-04-26 12:12:34,965[DEBUG]root(example1.py).<module>(line11)/thread21536::True
+2024-04-26 12:12:34,968[DEBUG]root(example1.py).<module>(line12)/thread21536::
+2024-04-26 12:12:34,968[DEBUG]root(example1.py).<module>(line13)/thread21536::hello0-1
+2024-04-26 12:12:34,970[DEBUG]logger_first(main.py).__init__(line145)/thread21536::====================================================================================================
+2024-04-26 12:12:34,970[DEBUG]logger_first(main.py).__init__(line148)/thread21536::[Logger.logger_first] start STREAM
+2024-04-26 12:12:34,971[DEBUG]logger_first(main.py).__init__(line151)/thread21536::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
+2024-04-26 12:12:34,971[DEBUG]logger_first(example1.py).<module>(line16)/thread21536::hello1-1
+2024-04-26 12:12:34,972[DEBUG]logger_second(main.py).__init__(line145)/thread21536::====================================================================================================
+2024-04-26 12:12:34,973[DEBUG]logger_second(main.py).__init__(line148)/thread21536::[Logger.logger_second] start STREAM
+2024-04-26 12:12:34,973[DEBUG]logger_second(main.py).__init__(line151)/thread21536::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
+2024-04-26 12:12:34,973[DEBUG]logger_second(example1.py).<module>(line19)/thread21536::hello2-1
+2024-04-26 12:12:34,974[DEBUG]root(example1.py).<module>(line21)/thread21536::hello0-2
+2024-04-26 12:12:34,974[DEBUG]logger_first(example1.py).<module>(line22)/thread21536::hello1-2
+2024-04-26 12:12:34,974[DEBUG]logger_second(example1.py).<module>(line23)/thread21536::hello2-2
+2024-04-26 12:12:34,975[DEBUG]logger_dir(main.py).__init__(line145)/thread21536::====================================================================================================
+2024-04-26 12:12:34,975[DEBUG]logger_dir(main.py).__init__(line148)/thread21536::[Logger.logger_dir] start STREAM
+2024-04-26 12:12:34,976[DEBUG]logger_dir(main.py).__init__(line151)/thread21536::[Logger.logger_dir] start FILE=[c:\1\logger__logger_dir.log]
+2024-04-26 12:12:34,976[DEBUG]logger_dir(example1.py).<module>(line27)/thread21536::hello_dir
+2024-04-26 12:12:34,977[DEBUG]Example(main.py).__init__(line145)/thread21536::====================================================================================================
+2024-04-26 12:12:34,977[DEBUG]Example(main.py).__init__(line148)/thread21536::[Logger.Example] start STREAM
+2024-04-26 12:12:34,977[DEBUG]Example(main.py).__init__(line151)/thread21536::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
+2024-04-26 12:12:34,977[DEBUG]Example(example1.py).meth(line39)/thread21536::hello123
 ```
 
 ********************************************************************************
```

### Comparing `logger_aux-0.0.3/logger_aux/main.py` & `logger_aux-0.0.4/logger_aux/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,32 +137,32 @@
             self._handler_file.setFormatter(self._formatter)
             self.LOGGER.addHandler(self._handler_file)
 
         # INIT ROOT -----------------------------------------
         # run always after connects!
         self._log_init_root()
 
-        # INITIAL MSG -----------------------------------------
+        # INITIAL MSG ---------------------------------------
         self.LOGGER.debug("="*100)
 
         if self.LOG_USE_STREAM:
             self.LOGGER.debug(f"[Logger.{self.LOG_NAME}] start STREAM")
 
         if self.LOG_USE_FILE:
             self.LOGGER.debug(f"[Logger.{self.LOG_NAME}] start FILE=[{self._handler_file.baseFilename}]")
 
-    @classmethod
-    def _log_init_root(cls, *args, **kwargs) -> None:
+    @staticmethod
+    def _log_init_root() -> None:
         """
         DONT USE IT DIRECTLY!!!
         it would used always automated!!!
         """
         logger_root = logging.getLogger()
         if not logger_root.hasHandlers():
-            cls(*args, **kwargs)
+            Logger()        # DONT USE cls()!!!
 
 
 # =====================================================================================================================
 if __name__ == "__main__":
     pass
```

### Comparing `logger_aux-0.0.3/setup.py` & `logger_aux-0.0.4/setup.py`

 * *Files identical despite different names*

