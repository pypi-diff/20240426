# Comparing `tmp/logger_aux-0.0.2.tar.gz` & `tmp/logger_aux-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_aux-0.0.2.tar", last modified: Thu Apr 25 13:57:52 2024, max compression
+gzip compressed data, was "logger_aux-0.0.3.tar", last modified: Fri Apr 26 08:05:18 2024, max compression
```

## Comparing `logger_aux-0.0.2.tar` & `logger_aux-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 13:57:52.178115 logger_aux-0.0.2/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     6665 2024-04-25 13:57:52.178115 logger_aux-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5865 2024-04-25 13:57:27.000000 logger_aux-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 13:57:52.169510 logger_aux-0.0.2/logger_aux/
--rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.2/logger_aux/__init__.py
--rw-rw-rw-   0        0        0     4427 2024-04-25 12:25:02.000000 logger_aux-0.0.2/logger_aux/main.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:57:52.177468 logger_aux-0.0.2/logger_aux.egg-info/
--rw-rw-rw-   0        0        0     6665 2024-04-25 13:57:52.000000 logger_aux-0.0.2/logger_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-25 13:57:52.000000 logger_aux-0.0.2/logger_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 13:57:52.000000 logger_aux-0.0.2/logger_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 13:57:52.000000 logger_aux-0.0.2/logger_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 13:57:52.179150 logger_aux-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 logger_aux-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:05:18.459385 logger_aux-0.0.3/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     8403 2024-04-26 08:05:18.459385 logger_aux-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7603 2024-04-26 08:04:07.000000 logger_aux-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 08:05:18.451516 logger_aux-0.0.3/logger_aux/
+-rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.3/logger_aux/__init__.py
+-rw-rw-rw-   0        0        0     6114 2024-04-26 07:44:47.000000 logger_aux-0.0.3/logger_aux/main.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:05:18.458384 logger_aux-0.0.3/logger_aux.egg-info/
+-rw-rw-rw-   0        0        0     8403 2024-04-26 08:05:18.000000 logger_aux-0.0.3/logger_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-26 08:05:18.000000 logger_aux-0.0.3/logger_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 08:05:18.000000 logger_aux-0.0.3/logger_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 08:05:18.000000 logger_aux-0.0.3/logger_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 08:05:18.460384 logger_aux-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-04-26 07:47:41.000000 logger_aux-0.0.3/setup.py
```

### Comparing `logger_aux-0.0.2/LICENSE` & `logger_aux-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logger_aux-0.0.2/logger_aux/main.py` & `logger_aux-0.0.3/logger_aux/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import *
 import pathlib
 import logging
 from logging.handlers import RotatingFileHandler
 
 
 # =====================================================================================================================
-def _example():
+def _example_zero():
     LEVEL = logging.DEBUG
     PATTERN = '%(asctime)s[%(levelname)s](%(name)s(%(filename)s).%(funcName)s/thread%(thread)s(line%(lineno)d))%(msg)s'
     formatter = logging.Formatter(PATTERN)
 
     logger = logging.getLogger()
     logger.setLevel(LEVEL)
 
@@ -26,95 +26,143 @@
     # logger.log(10, 'ЛОГ10')   #DEBUG=ЛОГ10
     # logger.log(11, 'ЛОГ11')   #Level 11=ЛОГ11
     logger.warning('MSG_DEFAULT')     # 2024-03-19 15:27:21,644[WARNING](root(t001.py).<module>/thread18536(line21))MSG_DEFAULT
 
 
 # =====================================================================================================================
 class Logger:
+    """
+    NOTES:
+        DONT use directly root as secondary logger - use it only as first or it would be applyed automatically!
+    """
+
     # SETTINGS ---------------------------------------
-    NAME: None | str = None     # None="root"
+    LOG_NAME: None | str = None     # None=self "root"="root", if not StrNone=get ClassName!
 
-    LEVEL: int = logging.DEBUG
-    PATTERN: str = '%(asctime)s[%(levelname)s](%(name)s(%(filename)s).%(funcName)s/thread%(thread)s(line%(lineno)d))%(msg)s'
+    LOG_LEVEL: int = logging.DEBUG
+    LOG_PATTERN: str = '%(asctime)s[%(levelname)s]%(name)s(%(filename)s).%(funcName)s(line%(lineno)d)/thread%(thread)s::%(msg)s'
 
-    DIRPATH: None | pathlib.Path = None
+    LOG_DIRPATH: None | pathlib.Path = None
 
-    FILENAME_START: None | str = None
-    FILENAME_EXTENTION: None | str = None
-    FILE_MAXBYTES: int = 1024*100
-    FILE_BACKUPCOUNT: int = 3
+    LOG_FILE_STARTWITH: None | str = None
+    LOG_FILE_EXTENTION: None | str = None
+    LOG_FILE_MAXBYTES: int = 1024 * 100
+    LOG_FILE_BACKUPCOUNT: int = 3
 
-    USE_STREAM: bool = True
-    USE_FILE: bool = True
+    LOG_DISABLE: None | bool = None
+    LOG_USE_STREAM: bool = True
+    LOG_USE_FILE: bool = True
 
     # AUX ---------------------------------------
     _formatter: logging.Formatter
 
     @property
-    def FILENAME(self) -> str:
-        return f"{self.FILENAME_START or 'logger'}__{self.NAME or 'root'}.{self.FILENAME_EXTENTION or 'log'}"
+    def LOG_FILENAME(self) -> str:
+        return f"{self.LOG_FILE_STARTWITH or 'logger'}__{self.LOG_NAME or 'root'}.{self.LOG_FILE_EXTENTION or 'log'}"
 
     @property
-    def FILEPATH(self) -> pathlib.Path:
-        if self.DIRPATH is None:
-            return pathlib.Path(self.FILENAME)
+    def LOG_FILEPATH(self) -> pathlib.Path:
+        if self.LOG_DIRPATH is None:
+            return pathlib.Path(self.LOG_FILENAME)
         else:
-            return self.DIRPATH.joinpath(self.FILENAME)
+            return self.LOG_DIRPATH.joinpath(self.LOG_FILENAME)
 
     def __init__(
             self,
-            name: None | str = None,
-            dirpath: None | str | pathlib.Path = None,
-            level: None | int = None,
-            use_stream: None | bool = None,
-            use_file: None | bool = None,
+            log_name: None | str | Any = None,
+            log_dirpath: None | str | pathlib.Path = None,
+            log_level: None | int = None,
+            log_use_stream: None | bool = None,
+            log_use_file: None | bool = None,
+            log_disable: None | bool = None,
+
+            *args,
+            **kwargs,
     ):
+        super().__init__(*args, **kwargs)
+
         # PARAMS ------------------------------------------
-        if name is not None:
-            self.NAME = name
+        if log_name is not None:
+            self.LOG_NAME = log_name
+
+        if log_dirpath is not None:
+            self.LOG_DIRPATH = pathlib.Path(log_dirpath)
 
-        if dirpath is not None:
-            self.DIRPATH = pathlib.Path(dirpath)
+        if log_level is not None:
+            self.LOG_LEVEL = log_level
 
-        if level is not None:
-            self.LEVEL = level
+        if log_use_stream is not None:
+            self.LOG_USE_STREAM = log_use_stream
 
-        if use_stream is not None:
-            self.USE_STREAM = use_stream
+        if log_use_file is not None:
+            self.LOG_USE_FILE = log_use_file
 
-        if use_file is not None:
-            self.USE_FILE = use_file
+        if log_disable is not None:
+            self.LOG_DISABLE = log_disable
 
         # PREPARE ------------------------------------------
-        # TODO: create DIRPATH
+        if self.LOG_DISABLE:
+            return
+
+        # TODO: create not exists LOG_DIRPATH
+
+        # if log_name as istance!
+        if self.LOG_NAME is None:
+            class_name = self.__class__.__name__
+            if class_name == "Logger":
+                self.LOG_NAME = "root"
+            else:
+                self.LOG_NAME = class_name
+        elif not isinstance(self.LOG_NAME, str):
+            self.LOG_NAME = self.LOG_NAME.__class__.__name__
 
         # INIT ---------------------------------------------
-        self.LOGGER = logging.getLogger(self.NAME)
-        self.LOGGER.setLevel(self.LEVEL)
+        self.LOGGER = logging.getLogger(self.LOG_NAME)
+        self.LOGGER.setLevel(self.LOG_LEVEL)
 
-        self._formatter = logging.Formatter(self.PATTERN)
+        self._formatter = logging.Formatter(self.LOG_PATTERN)
 
         self._handler_stream = None
         self._handler_file = None
 
-        # WORK ---------------------------------------------
-        if self.USE_STREAM:
+        # CONNECT ---------------------------------------------
+        if self.LOG_USE_STREAM:
             self._handler_stream = logging.StreamHandler()
-            # self._handler_stream.setLevel(self.LEVEL)
+            # self._handler_stream.setLevel(self.LOG_LEVEL)
             self._handler_stream.setFormatter(self._formatter)
             self.LOGGER.addHandler(self._handler_stream)
-            self.LOGGER.debug(f"logger STREAM started")
 
-        if self.USE_FILE:
-            self._handler_file = RotatingFileHandler(self.FILEPATH, maxBytes=self.FILE_MAXBYTES, backupCount=self.FILE_BACKUPCOUNT)
-            # self._handler_file.setLevel(self.LEVEL)
+        if self.LOG_USE_FILE:
+            self._handler_file = RotatingFileHandler(self.LOG_FILEPATH, maxBytes=self.LOG_FILE_MAXBYTES, backupCount=self.LOG_FILE_BACKUPCOUNT)
+            # self._handler_file.setLevel(self.LOG_LEVEL)
             self._handler_file.setFormatter(self._formatter)
             self.LOGGER.addHandler(self._handler_file)
-            self.LOGGER.debug("="*100)
-            self.LOGGER.debug(f"logger FILE started {self._handler_file.baseFilename=}")
+
+        # INIT ROOT -----------------------------------------
+        # run always after connects!
+        self._log_init_root()
+
+        # INITIAL MSG -----------------------------------------
+        self.LOGGER.debug("="*100)
+
+        if self.LOG_USE_STREAM:
+            self.LOGGER.debug(f"[Logger.{self.LOG_NAME}] start STREAM")
+
+        if self.LOG_USE_FILE:
+            self.LOGGER.debug(f"[Logger.{self.LOG_NAME}] start FILE=[{self._handler_file.baseFilename}]")
+
+    @classmethod
+    def _log_init_root(cls, *args, **kwargs) -> None:
+        """
+        DONT USE IT DIRECTLY!!!
+        it would used always automated!!!
+        """
+        logger_root = logging.getLogger()
+        if not logger_root.hasHandlers():
+            cls(*args, **kwargs)
 
 
 # =====================================================================================================================
 if __name__ == "__main__":
     pass
```

### Comparing `logger_aux-0.0.2/setup.py` & `logger_aux-0.0.3/setup.py`

 * *Files identical despite different names*

