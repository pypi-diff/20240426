# Comparing `tmp/tomata-1.0.3.tar.gz` & `tmp/tomata-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomata-1.0.3.tar", max compression
+gzip compressed data, was "tomata-1.1.0.tar", max compression
```

## Comparing `tomata-1.0.3.tar` & `tomata-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-10-27 05:58:49.386531 tomata-1.0.3/LICENSE
--rw-r--r--   0        0        0     8337 2023-10-27 05:58:49.386531 tomata-1.0.3/README.md
--rw-r--r--   0        0        0      542 2023-10-27 05:58:49.386531 tomata-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       96 2023-10-27 05:58:49.386531 tomata-1.0.3/tomata/__init__.py
--rw-r--r--   0        0        0     3552 2023-10-27 05:58:49.386531 tomata-1.0.3/tomata/async_emitter.py
--rw-r--r--   0        0        0     1186 2023-10-27 05:58:49.386531 tomata-1.0.3/tomata/base.py
--rw-r--r--   0        0        0     2801 2023-10-27 05:58:49.386531 tomata-1.0.3/tomata/emitter.py
--rw-r--r--   0        0        0        0 2023-10-27 05:58:49.386531 tomata-1.0.3/tomata/py.typed
--rw-r--r--   0        0        0     8933 1970-01-01 00:00:00.000000 tomata-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-26 03:52:38.651458 tomata-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9049 2024-04-26 03:52:38.651458 tomata-1.1.0/README.md
+-rw-r--r--   0        0        0      542 2024-04-26 03:52:38.651458 tomata-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       96 2024-04-26 03:52:38.651458 tomata-1.1.0/tomata/__init__.py
+-rw-r--r--   0        0        0     3695 2024-04-26 03:52:38.651458 tomata-1.1.0/tomata/async_emitter.py
+-rw-r--r--   0        0        0     1186 2024-04-26 03:52:38.651458 tomata-1.1.0/tomata/base.py
+-rw-r--r--   0        0        0     3012 2024-04-26 03:52:38.651458 tomata-1.1.0/tomata/emitter.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:52:38.651458 tomata-1.1.0/tomata/py.typed
+-rw-r--r--   0        0        0     9696 1970-01-01 00:00:00.000000 tomata-1.1.0/PKG-INFO
```

### Comparing `tomata-1.0.3/LICENSE` & `tomata-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tomata-1.0.3/README.md` & `tomata-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -292,13 +292,49 @@
 To redefine setting fallback handler logic, define your own `set_default(handler)` and `get_default()` methods.
 
 
 ### AsyncEmitter methods
 
 To extend AsyncEmitter, you have to remember two things:
 
-- Some methods (`[get|set]_state`, `get_handler`, `get_default`) are async. This means you have to define them with `async def` even if you don't plan to use await in them. 
+- Some methods (`[get|set]_state`, `get_handler`, `get_default`, `reroute`) are async. This means you have to define them with `async def` even if you don't plan to use await in them. 
     *`emit` is obviously async, but if you don't need an async `emit`, take a look at synchronous `Emitter`*
 
 - In `set_handler` and `set_default`, you have to async-ify the handlers. To do that, use `tomata.async_emitter.make_async` function, which takes any handler and makes it async
 
-Otherwise, the extension process should be just as with `Emitter`.
+Otherwise, the extension process should be just as with `Emitter`.
+
+
+## Reroute 
+
+*new in 1.1.0*
+
+Sometimes you receive an event within one state and want to handle it within another instead. Use `*Emitter.reroute()` for this:
+
+```python
+from time import time
+
+HOUR = 3600
+DAY = 24 * HOUR
+NOON = 12 * HOUR
+
+@handler.on("state1")
+def handle1(event: Event, identity: Identity, state: State):
+    if (time() % DAY) > NOON:
+        return handler.reroute("state2", event, identity)
+        
+    print("it is morning")
+
+
+@handler.on("state2")
+def handle2(event: Event, identity: Identity, state: State):
+    print("it is state2 or afternoon")
+
+```
+
+`.reroute` basically does this:
+
+```python
+handler.set_state(identity, state)
+handler.emit(event, identity)
+return None
+```
```

### Comparing `tomata-1.0.3/pyproject.toml` & `tomata-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomata"
-version = "1.0.3"
+version = "1.1.0"
 description = ""
 authors = ["Dmitry Gritsenko <tomata@evtn.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/evtn/tomata"
 homepage = "https://github.com/evtn/tomata"
 keywords = []
```

### Comparing `tomata-1.0.3/tomata/async_emitter.py` & `tomata-1.1.0/tomata/async_emitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,31 +58,31 @@
         next_state = await handler(event, identity, current_state)
 
         if not next_state:
             return
 
         await self.leave_state(current_state, event, identity)
         await self.set_state(identity, next_state)
-        await self.enter_state(next_state, event, identity, current_state)
+        await self.enter_state(next_state, event, identity)
 
-    async def set_state(self, identity: Id, state: SK):
-        return NotImplemented
+    async def set_state(self, identity: Id, state: SK) -> None:
+        return
 
     async def get_state(self, identity: Id) -> SK:
         return NotImplemented
 
     async def leave_state(self, state: SK, event: Ev, identity: Id):
         leave_handler = await self.get_handler(state, "leave")
 
         if not leave_handler:
             return
 
         return await leave_handler(event, identity, state)
 
-    async def enter_state(self, state: SK, event: Ev, identity: Id, prev_state: SK):
+    async def enter_state(self, state: SK, event: Ev, identity: Id):
         enter_handler = await self.get_handler(state, "enter")
 
         if not enter_handler:
             return
 
         await enter_handler(event, identity, state)
 
@@ -102,14 +102,19 @@
 
     async def get_default(self) -> AsyncHandler[Ev, Id, SK] | None:
         return self.handlers["default"]
 
     def set_default(self, handler: Handler[Ev, Id, SK]):
         self.handlers["default"] = make_async(handler)
 
+    async def reroute(self, state: SK, event: Ev, identity: Id) -> None:
+        await self.set_state(identity, state)
+        await self.emit(event, identity)
+        return None
+
 
 class AsyncOn(Generic[Ev, SK, Id]):
     def __init__(self, emitter: AsyncEmitter[Ev, SK, Id]):
         self.emitter = emitter
 
     def __call__(self, state: SK, handler_type: HandlerType = "event"):
         def decorator(handler: Handler[Ev, Id, SK]) -> Handler[Ev, Id, SK]:
```

### Comparing `tomata-1.0.3/tomata/base.py` & `tomata-1.1.0/tomata/base.py`

 * *Files identical despite different names*

### Comparing `tomata-1.0.3/tomata/emitter.py` & `tomata-1.1.0/tomata/emitter.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,58 +33,74 @@
         next_state = handler(event, identity, current_state)
 
         if not next_state:
             return
 
         self.leave_state(current_state, event, identity)
         self.set_state(identity, next_state)
-        self.enter_state(next_state, event, identity, current_state)
+        self.enter_state(next_state, event, identity)
 
-    def set_state(self, identity: Id, state: SK):
-        return NotImplemented
+    def set_state(self, identity: Id, state: SK) -> None:
+        return
 
     def get_state(self, identity: Id) -> SK:
         return NotImplemented
 
-    def leave_state(self, state: SK, event: Ev, identity: Id):
+    def leave_state(
+        self,
+        state: SK,
+        event: Ev,
+        identity: Id,
+    ):
         leave_handler = self.get_handler(state, "leave")
 
         if not leave_handler:
             return
 
         leave_handler(event, identity, state)
 
-    def enter_state(self, state: SK, event: Ev, identity: Id, prev_state: SK):
+    def enter_state(
+        self,
+        state: SK,
+        event: Ev,
+        identity: Id,
+    ):
         enter_handler = self.get_handler(state, "enter")
 
         if not enter_handler:
             return
 
         enter_handler(event, identity, state)
 
     def get_handler(
-        self, state: SK, handler_type: HandlerType
+        self,
+        state: SK,
+        handler_type: HandlerType,
     ) -> SyncHandler[Ev, Id, SK] | None:
         store = self.handlers[handler_type]
         return store.get(state)
 
     def set_handler(
         self,
         state: SK,
         handler_type: HandlerType,
         handler: SyncHandler[Ev, Id, SK],
     ):
         self.handlers[handler_type][state] = handler
 
     def get_default(self) -> SyncHandler[Ev, Id, SK] | None:
-        return self.handlers["default"]
+        return self.handlers.get("default")
 
     def set_default(self, handler: SyncHandler[Ev, Id, SK]):
         self.handlers["default"] = handler
 
+    def reroute(self, state: SK, event: Ev, identity: Id) -> None:
+        self.set_state(identity, state)
+        return self.emit(event, identity)
+
 
 class On(Generic[Ev, SK, Id]):
     def __init__(self, emitter: Emitter[Ev, SK, Id]):
         self.emitter = emitter
 
     def __call__(self, state: SK, handler_type: HandlerType = "event"):
         def decorator(handler: SyncHandler[Ev, Id, SK]):
```

### Comparing `tomata-1.0.3/PKG-INFO` & `tomata-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tomata
-Version: 1.0.3
+Version: 1.1.0
 Summary: 
 Home-page: https://github.com/evtn/tomata
 License: MIT
 Author: Dmitry Gritsenko
 Author-email: tomata@evtn.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/evtn/tomata
 Description-Content-Type: text/markdown
 
 # Welcome to `tomata` readme!
 
 This is a generic state automata-ish module allowing you to build an typed event-driven stateful flow with minimal setup.
 
@@ -310,13 +311,49 @@
 To redefine setting fallback handler logic, define your own `set_default(handler)` and `get_default()` methods.
 
 
 ### AsyncEmitter methods
 
 To extend AsyncEmitter, you have to remember two things:
 
-- Some methods (`[get|set]_state`, `get_handler`, `get_default`) are async. This means you have to define them with `async def` even if you don't plan to use await in them. 
+- Some methods (`[get|set]_state`, `get_handler`, `get_default`, `reroute`) are async. This means you have to define them with `async def` even if you don't plan to use await in them. 
     *`emit` is obviously async, but if you don't need an async `emit`, take a look at synchronous `Emitter`*
 
 - In `set_handler` and `set_default`, you have to async-ify the handlers. To do that, use `tomata.async_emitter.make_async` function, which takes any handler and makes it async
 
 Otherwise, the extension process should be just as with `Emitter`.
+
+
+## Reroute 
+
+*new in 1.1.0*
+
+Sometimes you receive an event within one state and want to handle it within another instead. Use `*Emitter.reroute()` for this:
+
+```python
+from time import time
+
+HOUR = 3600
+DAY = 24 * HOUR
+NOON = 12 * HOUR
+
+@handler.on("state1")
+def handle1(event: Event, identity: Identity, state: State):
+    if (time() % DAY) > NOON:
+        return handler.reroute("state2", event, identity)
+        
+    print("it is morning")
+
+
+@handler.on("state2")
+def handle2(event: Event, identity: Identity, state: State):
+    print("it is state2 or afternoon")
+
+```
+
+`.reroute` basically does this:
+
+```python
+handler.set_state(identity, state)
+handler.emit(event, identity)
+return None
+```
```

