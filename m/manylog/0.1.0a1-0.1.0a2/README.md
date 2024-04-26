# Comparing `tmp/manylog-0.1.0a1.tar.gz` & `tmp/manylog-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manylog-0.1.0a1.tar", last modified: Fri Apr 26 19:57:50 2024, max compression
+gzip compressed data, was "manylog-0.1.0a2.tar", last modified: Fri Apr 26 20:24:25 2024, max compression
```

## Comparing `manylog-0.1.0a1.tar` & `manylog-0.1.0a2.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:50.481716 manylog-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 19:57:46.000000 manylog-0.1.0a1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 19:57:46.000000 manylog-0.1.0a1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 19:57:46.000000 manylog-0.1.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 19:57:46.000000 manylog-0.1.0a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 19:57:46.000000 manylog-0.1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-26 19:57:50.481716 manylog-0.1.0a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:50.473716 manylog-0.1.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-26 19:57:46.000000 manylog-0.1.0a1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-26 19:57:46.000000 manylog-0.1.0a1/justfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:50.473716 manylog-0.1.0a1/manylog/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-26 19:57:46.000000 manylog-0.1.0a1/manylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-26 19:57:46.000000 manylog-0.1.0a1/manylog/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-26 19:57:46.000000 manylog-0.1.0a1/manylog/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-26 19:57:46.000000 manylog-0.1.0a1/manylog/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:50.477716 manylog-0.1.0a1/manylog/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-26 19:57:46.000000 manylog-0.1.0a1/manylog/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-26 19:57:46.000000 manylog-0.1.0a1/manylog/worker/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-26 19:57:46.000000 manylog-0.1.0a1/manylog/worker/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-26 19:57:46.000000 manylog-0.1.0a1/manylog/worker/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:50.477716 manylog-0.1.0a1/manylog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-26 19:57:50.000000 manylog-0.1.0a1/manylog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-26 19:57:50.000000 manylog-0.1.0a1/manylog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:57:50.000000 manylog-0.1.0a1/manylog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-26 19:57:50.000000 manylog-0.1.0a1/manylog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 19:57:50.000000 manylog-0.1.0a1/manylog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-26 19:57:46.000000 manylog-0.1.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:57:50.481716 manylog-0.1.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:50.477716 manylog-0.1.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-26 19:57:46.000000 manylog-0.1.0a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-26 19:57:46.000000 manylog-0.1.0a1/tests/test_sp_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-26 19:57:46.000000 manylog-0.1.0a1/tests/test_sp_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:25.679014 manylog-0.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 20:24:19.000000 manylog-0.1.0a2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 20:24:19.000000 manylog-0.1.0a2/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 20:24:19.000000 manylog-0.1.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 20:24:19.000000 manylog-0.1.0a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 20:24:19.000000 manylog-0.1.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-26 20:24:25.679014 manylog-0.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-26 20:24:19.000000 manylog-0.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:25.671013 manylog-0.1.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-26 20:24:19.000000 manylog-0.1.0a2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-26 20:24:19.000000 manylog-0.1.0a2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-26 20:24:19.000000 manylog-0.1.0a2/docs/parent.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-26 20:24:19.000000 manylog-0.1.0a2/docs/worker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-26 20:24:19.000000 manylog-0.1.0a2/justfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:25.671013 manylog-0.1.0a2/manylog/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-26 20:24:19.000000 manylog-0.1.0a2/manylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-26 20:24:19.000000 manylog-0.1.0a2/manylog/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-26 20:24:19.000000 manylog-0.1.0a2/manylog/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-26 20:24:19.000000 manylog-0.1.0a2/manylog/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:25.675013 manylog-0.1.0a2/manylog/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-26 20:24:19.000000 manylog-0.1.0a2/manylog/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-26 20:24:19.000000 manylog-0.1.0a2/manylog/worker/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-26 20:24:19.000000 manylog-0.1.0a2/manylog/worker/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-26 20:24:19.000000 manylog-0.1.0a2/manylog/worker/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:25.675013 manylog-0.1.0a2/manylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-26 20:24:25.000000 manylog-0.1.0a2/manylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-26 20:24:25.000000 manylog-0.1.0a2/manylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:24:25.000000 manylog-0.1.0a2/manylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-26 20:24:25.000000 manylog-0.1.0a2/manylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 20:24:25.000000 manylog-0.1.0a2/manylog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-26 20:24:19.000000 manylog-0.1.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:24:25.679014 manylog-0.1.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:24:25.675013 manylog-0.1.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-26 20:24:19.000000 manylog-0.1.0a2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-26 20:24:19.000000 manylog-0.1.0a2/tests/test_sp_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-26 20:24:19.000000 manylog-0.1.0a2/tests/test_sp_progress.py
```

### Comparing `manylog-0.1.0a1/.gitignore` & `manylog-0.1.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a1/LICENSE.md` & `manylog-0.1.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a1/docs/conf.py` & `manylog-0.1.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a1/justfile` & `manylog-0.1.0a2/justfile`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a1/manylog/listener.py` & `manylog-0.1.0a2/manylog/listener.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,69 +5,96 @@
 from __future__ import annotations
 
 import logging
 import os
 import warnings
 from tempfile import TemporaryDirectory
 from threading import Thread
-from typing import Optional
+from typing import Any, Optional
 from uuid import UUID
 
 import zmq
 from progress_api.api import Progress
 from progress_api.backends import ProgressBarSpec
 from progress_api.config import get_backend
 
 import manylog.connection as x
 import manylog.messages as m
 
 _log = logging.getLogger(__name__)
 
 
 class LogListener:
+    """
+    Class that listens for logging messages and reinjects them in the parent.
+
+    The listener is not listening for messages until :meth:`start` is called. It
+    must be properly shut down with :meth:`close`.  The log listener can be used
+    as a context manager, in which case `start` and `close` will be
+    automatically called.  If the process terminates without calling `close`,
+    log messages may be lost.
+
+    Args:
+        ctx: A ZeroMQ context to use.
+    """
+
     address: str | None = None
+    "The address where the socket is listening for log messages."
     context: x.Context
     thread: ListenThread | None = None
     _tmpdir: TemporaryDirectory[str]
 
     def __init__(self, ctx: Optional[x.Context] = None):
         if ctx is None:
             self.context = zmq.Context.instance()
         else:
             self.context = ctx
 
     def start(self):
+        """
+        Start the log listener.
+        """
         rt_dir = os.environ.get("XDG_RUNTIME_DIR", None)
         self._tmpdir = TemporaryDirectory(prefix="manylog-", dir=rt_dir)
         try:
             socket = self.context.socket(zmq.PULL, zmq.Socket)
             self.address = f"ipc://{self._tmpdir.name}/logging.ipc"
             socket.bind(self.address)
             self.thread = ListenThread(socket)
             self.thread.start()
         except Exception as e:
             self._tmpdir.cleanup()
             raise e
 
     def close(self):
+        """
+        Shut down the log listener.
+        """
         if not self.thread:
             warnings.warn("listener thread not running")
             return
         self.thread.shutdown()
         self.thread = None
         self._tmpdir.cleanup()
 
+    def __begin__(self):
+        self.start()
+        return self
+
+    def __end__(self, *args: Any):
+        self.close()
+
 
 class ListenThread(Thread):
     socket: x.Socket
     _shutdown_wanted: bool = False
     active_pbs: dict[UUID, Progress]
 
     def __init__(self, socket: x.Socket):
-        super().__init__(name="manylog-listener")
+        super().__init__(name="manylog-listener", daemon=True)
         self.socket = socket
         self.active_pbs = {}
 
     def run(self):
         while True:
             # we poll for 250ms, to allow shutdown signals
             evt = self.socket.poll(250)
```

### Comparing `manylog-0.1.0a1/manylog/messages.py` & `manylog-0.1.0a2/manylog/messages.py`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a1/manylog/worker/logging.py` & `manylog-0.1.0a2/manylog/worker/logging.py`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a1/manylog/worker/progress.py` & `manylog-0.1.0a2/manylog/worker/progress.py`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a1/manylog/worker/setup.py` & `manylog-0.1.0a2/manylog/worker/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,24 @@
 
 from ..connection import Context
 from .logging import ZMQLogHandler
 from .progress import ZMQProgressBackend
 
 
 def init_worker_logging(address: str, level: int = logging.INFO):
+    """
+    Initialize logging in the worker.
+
+    Args:
+        address:
+            The address of the socket to connect to.  This can be
+            obtained from :attr:`manylog.LogListener.address`.
+        level:
+            The maximum logging level to forward.
+    """
     ctx: Context = zmq.Context.instance()
     sock = ctx.socket(zmq.PUSH)
     sock.connect(address)
 
     h = ZMQLogHandler(sock)
     h.setLevel(level)
     root = logging.getLogger()
```

### Comparing `manylog-0.1.0a1/pyproject.toml` & `manylog-0.1.0a2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 doc = [
   "sphinx >=4.2",
   "sphinxext-opengraph >= 0.5",
   "furo",
 ]
 
 [project.urls]
-Homepage = "https://manylog.lenksit.org"
+Documentation = "https://manylog.readthedocs.io/"
 GitHub = "https://github.com/lenskit/manylog"
 
 # configure build tools
 [tool.setuptools.packages.find]
 include = ["manylog"]
 
 [tool.setuptools_scm]
```

### Comparing `manylog-0.1.0a1/tests/test_sp_log.py` & `manylog-0.1.0a2/tests/test_sp_log.py`

 * *Files identical despite different names*

### Comparing `manylog-0.1.0a1/tests/test_sp_progress.py` & `manylog-0.1.0a2/tests/test_sp_progress.py`

 * *Files identical despite different names*

