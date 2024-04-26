# Comparing `tmp/schorle-0.0.8.tar.gz` & `tmp/schorle-0.0.9.tar.gz`

## Comparing `schorle-0.0.8.tar` & `schorle-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,51 @@
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 schorle-0.0.8/Makefile
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 schorle-0.0.8/.github/workflows/onrelease.yml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 schorle-0.0.8/docs/Dockerfile.docs
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 schorle-0.0.8/docs/landing.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 schorle-0.0.8/docs/deployment/main.tf
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 schorle-0.0.8/examples/async_counter.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 schorle-0.0.8/examples/counter.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 schorle-0.0.8/examples/counter_shared_state.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 schorle-0.0.8/examples/todo_list.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 schorle-0.0.8/raw/logo.svg
--rw-r--r--   0        0        0    63256 2020-02-02 00:00:00.000000 schorle-0.0.8/raw/with_text.png
--rw-r--r--   0        0        0   119656 2020-02-02 00:00:00.000000 schorle-0.0.8/raw/with_text.svg
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/__about__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/__init__.py
--rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/app.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/attribute.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/button.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/classes.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/component.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/document.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/effector.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/element.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/emitter.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/icon.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/img.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/inputs.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/models.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/on.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/page.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/render_controller.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/state.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/tags.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/text.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/theme.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/types.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/utils.py
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/assets/bundle.js
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 schorle-0.0.8/src/schorle/assets/favicon.svg
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 schorle-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 schorle-0.0.8/tests/test_context_rendering.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 schorle-0.0.8/tests/test_doc.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 schorle-0.0.8/tests/test_nested_rendering.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 schorle-0.0.8/tests/test_reactive.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 schorle-0.0.8/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 schorle-0.0.8/LICENSE.md
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 schorle-0.0.8/README.md
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 schorle-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 schorle-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 schorle-0.0.9/Makefile
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 schorle-0.0.9/.github/workflows/onpush.yml
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 schorle-0.0.9/.github/workflows/onrelease.yml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 schorle-0.0.9/docs/Dockerfile.docs
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 schorle-0.0.9/docs/landing.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 schorle-0.0.9/docs/deployment/main.tf
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 schorle-0.0.9/examples/counter.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 schorle-0.0.9/examples/counter_shared_state.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 schorle-0.0.9/examples/counter_with_loading.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 schorle-0.0.9/examples/todo_list.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 schorle-0.0.9/raw/logo.svg
+-rw-r--r--   0        0        0    63256 2020-02-02 00:00:00.000000 schorle-0.0.9/raw/with_text.png
+-rw-r--r--   0        0        0   119656 2020-02-02 00:00:00.000000 schorle-0.0.9/raw/with_text.svg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/__about__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/__init__.py
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/app.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/attribute.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/button.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/classes.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/component.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/document.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/effector.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/element.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/emitter.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/icon.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/img.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/inputs.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/loading.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/models.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/on.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/page.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/render_controller.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/state.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/suspense.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/tags.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/text.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/theme.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/types.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/utils.py
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/assets/bundle.js
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 schorle-0.0.9/src/schorle/assets/favicon.svg
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 schorle-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 schorle-0.0.9/tests/test_context_rendering.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 schorle-0.0.9/tests/test_doc.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 schorle-0.0.9/tests/test_nested_rendering.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 schorle-0.0.9/tests/test_reactive.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 schorle-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 schorle-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 schorle-0.0.9/README.md
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 schorle-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 schorle-0.0.9/PKG-INFO
```

### Comparing `schorle-0.0.8/.github/workflows/onrelease.yml` & `schorle-0.0.9/.github/workflows/onrelease.yml`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/docs/Dockerfile.docs` & `schorle-0.0.9/docs/Dockerfile.docs`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/docs/landing.py` & `schorle-0.0.9/docs/landing.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/docs/deployment/main.tf` & `schorle-0.0.9/docs/deployment/main.tf`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/examples/async_counter.py` & `schorle-0.0.9/examples/counter_shared_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 from __future__ import annotations
 
-import asyncio
-
-from pydantic import Field
-
 from schorle.app import Schorle
+from schorle.button import Button
 from schorle.classes import Classes
-from schorle.component import Component
 from schorle.effector import effector
-from schorle.element import button, div, span
+from schorle.element import div, p
 from schorle.on import On
 from schorle.page import Page
 from schorle.state import ReactiveModel
 from schorle.text import text
 
 app = Schorle()
 
 
 class Counter(ReactiveModel):
-    count: int = 0
+    value: int = 0
 
     @effector
     async def increment(self):
-        await asyncio.sleep(1)
-        self.count += 1
-
-
-class Button(Component):
-    counter: Counter
-
-    def render(self):
-        with button(on=On("click", self.counter.increment), classes=Classes("btn btn-primary")):
-            with span(classes=Classes("htmx-indicator")):
-                with span(classes=Classes("loading loading-infinity")):
-                    text("")
-
-            with div():
-                text("Click me" if self.counter.count == 0 else f"Clicked {self.counter.count} times")
+        self.value += 1
 
-    def initialize(self):
-        self.bind(self.counter)
+    @effector
+    async def decrement(self):
+        self.value -= 1
 
 
 class PageWithButton(Page):
-    counter: Counter = Field(default_factory=Counter)
+    counter: Counter = Counter.factory()
 
     def render(self):
         with div(classes=Classes("flex flex-col justify-center items-center h-screen")):
-            Button(counter=self.counter)
+            with div(classes=Classes("flex flex-row justify-center items-center space-x-4")):
+                with Button(on=On("click", self.counter.increment), modifier="primary"):
+                    text("Increment")
+                with Button(
+                    on=On("click", self.counter.decrement),
+                    modifier="secondary",
+                    disabled=self.counter.value <= 0,
+                ):
+                    text("Decrement")
+            with p(classes=Classes("text-2xl")):
+                text(f"Counter: {self.counter.value}")
+
+    def initialize(self):
+        self.bind(self.counter)
 
 
 @app.get("/")
 def get_page():
     return PageWithButton()
```

### Comparing `schorle-0.0.8/examples/counter.py` & `schorle-0.0.9/examples/counter.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/examples/counter_shared_state.py` & `schorle-0.0.9/examples/counter_with_loading.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 from __future__ import annotations
 
+import asyncio
+
 from schorle.app import Schorle
 from schorle.button import Button
 from schorle.classes import Classes
+from schorle.component import Component
 from schorle.effector import effector
-from schorle.element import div, p
+from schorle.element import div
+from schorle.loading import Loading
 from schorle.on import On
 from schorle.page import Page
 from schorle.state import ReactiveModel
+from schorle.suspense import Suspense
 from schorle.text import text
 
 app = Schorle()
 
 
 class Counter(ReactiveModel):
-    value: int = 0
+    count: int = 0
 
     @effector
     async def increment(self):
-        self.value += 1
-
-    @effector
-    async def decrement(self):
-        self.value -= 1
+        await asyncio.sleep(1)
+        self.count += 1
 
 
-class PageWithButton(Page):
+class StatefulButton(Component):
     counter: Counter = Counter.factory()
+    modifier: str | None = None
 
     def render(self):
-        with div(classes=Classes("flex flex-col justify-center items-center h-screen")):
-            with div(classes=Classes("flex flex-row justify-center items-center space-x-4")):
-                with Button(on=On("click", self.counter.increment), modifier="primary"):
-                    text("Increment")
-                with Button(
-                    on=On("click", self.counter.decrement),
-                    modifier="secondary",
-                    disabled=self.counter.value <= 0,
-                ):
-                    text("Decrement")
-            with p(classes=Classes("text-2xl")):
-                text(f"Counter: {self.counter.value}")
+        with Button(
+            on=On("click", self.counter.increment),
+            suspense=Suspense(on=self.counter.increment, fallback=Loading()),
+            classes=self.classes.append("w-48"),
+            modifier=self.modifier,
+        ):
+            text("Click me" if self.counter.count == 0 else f"Clicked {self.counter.count} times")
 
     def initialize(self):
         self.bind(self.counter)
 
 
+class PageWithButton(Page):
+
+    def render(self):
+        with div(classes=Classes("flex flex-col justify-center items-center h-screen")):
+            with div(classes=Classes("space-y-2")):
+                StatefulButton(modifier="primary")
+                StatefulButton(modifier="secondary")
+
+
 @app.get("/")
 def get_page():
     return PageWithButton()
```

### Comparing `schorle-0.0.8/raw/logo.svg` & `schorle-0.0.9/raw/logo.svg`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/raw/with_text.png` & `schorle-0.0.9/raw/with_text.png`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/raw/with_text.svg` & `schorle-0.0.9/raw/with_text.svg`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/src/schorle/app.py` & `schorle-0.0.9/src/schorle/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,15 +75,14 @@
             extra_assets=self.extra_assets,
             lang=self.lang,
         )
         logger.debug(f"Rendering page: {page} with theme: {self.theme}...")
 
         lxml_element = render_in_context(doc)
         rendered = etree.tostring(lxml_element, pretty_print=True, doctype="<!DOCTYPE html>").decode("utf-8")
-        logger.debug(f"Page rendered into: {rendered}")
         response = HTMLResponse(rendered, status_code=200)
 
         logger.info(f"Adding page to cache with token: {doc.csrf_token}")
 
         self._pages[str(doc.csrf_token)] = page
 
         logger.debug("Page rendered.")
@@ -134,19 +133,21 @@
                 logger.debug(f"Events found reactive: {reactive}")
                 _callback = reactive.get(message.headers.trigger_type)
                 if _callback:
                     logger.debug(f"Events found callback: {_callback}")
 
                     if message.headers.trigger_name is not None:
                         _value = getattr(message, message.headers.trigger_name)
-                        await _callback(_value)
+                        _cb = partial(_callback, _value)
                     else:
-                        await _callback()
+                        _cb = _callback
+
+                    # TODO: catch exceptions in _cb
+                    asyncio.ensure_future(_cb())  # noqa: RUF006
 
-                    logger.debug("Events callback executed.")
                 else:
                     logger.error(f"Events no callback found for type: {message.headers.trigger_type}")
             else:
                 logger.error(f"Events no reactive found for id: {message.headers.trigger_element_id}")
 
         else:
             logger.error("No page found, closing websocket...")
```

### Comparing `schorle-0.0.8/src/schorle/button.py` & `schorle-0.0.9/src/schorle/button.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from schorle.classes import Classes
 from schorle.element import button
 from schorle.on import On
+from schorle.suspense import Suspense
 
 
 def Button(  # noqa: N802
     element_id: str | None = None,
     modifier: str | None = None,
     disabled: bool | None = None,
     classes: Classes | None = None,
     style: dict[str, str] | None = None,
     on: list[On] | On | None = None,
+    suspense: Suspense | None = None,
     **attributes,
 ) -> None:
     _classes = Classes("btn")
     if modifier:
         _classes.append(f"btn-{modifier}")
     if disabled:
         _classes.append("btn-disabled")
     if classes:
         _classes.append(classes)
 
-    return button(element_id=element_id, classes=_classes, style=style, on=on, **attributes)
+    return button(element_id=element_id, classes=_classes, style=style, on=on, suspense=suspense, **attributes)
```

### Comparing `schorle-0.0.8/src/schorle/classes.py` & `schorle-0.0.9/src/schorle/classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,20 +30,23 @@
     def __init__(self, *args: RawClassesPayload):
         super().__init__()
         self._value = parse_args(*args)
 
     def append(self, *args: RawClassesPayload):
         new_value = self._value + parse_args(*args)
         self._value = new_value
+        return self
 
     def remove(self, *args: RawClassesPayload):
         new_value = [x for x in self._value if x not in parse_args(*args)]
         self._value = new_value
+        return self
 
     def toggle(self, class_name: str):
         if class_name in self._value:
             self.remove(class_name)
         else:
             self.append(class_name)
+        return self
 
     def render(self) -> str:
         return "" if not self._value else " ".join(set(self._value)).strip()
```

### Comparing `schorle-0.0.8/src/schorle/component.py` & `schorle-0.0.9/src/schorle/component.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     tag: HTMLTag = HTMLTag.DIV
     classes: Classes = Field(default_factory=Classes)
     style: dict[str, str] = Field(default_factory=dict)
     element_id: str | None = None
     attributes: dict[str, str] = Field(default_factory=dict)
     on: list[On] | On = Field(default_factory=list)
     _page_ref: Any | None = None
+    lazy_append: bool = False
 
     def add(self):
         pre_previous = self.controller.previous
         pre_current = self.controller.current
         self._page_ref = self.controller.page
 
         with Element(self.tag, self.element_id, classes=self.classes, style=self.style, on=self.on, **self.attributes):
@@ -34,15 +35,15 @@
 
     def model_post_init(self, __context: Any) -> None:
         if not self.element_id and self.tag not in [HTMLTag.HTML, HTMLTag.BODY]:
             self.element_id = f"sle-{self.tag}-{str(uuid4())[:8]}"
 
         self.initialize()
 
-        if self.controller.page:
+        if self.controller.page and not self.lazy_append:
             self.add()
 
     def initialize(self):
         pass
 
     @abstractmethod
     def render(self):
```

### Comparing `schorle-0.0.8/src/schorle/document.py` & `schorle-0.0.9/src/schorle/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,37 +16,45 @@
     title: str = "Schorle"
     csrf_token: UUID = Field(default_factory=uuid4)
     theme: Theme = Theme.DARK
     page: Page | None = None
     with_dev_meta: bool = False
     extra_assets: list | None = None
     lang: str = "en"
+    with_tailwind: bool = True
+    with_daisyui: bool = True
+    with_htmx: bool = True
+    daisyui_version: str = "4.7.2"
 
     def model_post_init(self, __context: Any) -> None:
         self.attributes["lang"] = self.lang
         super().model_post_init(__context)
 
     def render(self):
         with head():
             meta(charset="utf-8")
             meta(name="viewport", content="width=device-width, initial-scale=1.0")
             meta(name="schorle-csrf-token", content=str(self.csrf_token))
             if self.with_dev_meta:
                 meta(name="schorle-dev", content="true")
             link(href="/favicon.svg", rel="icon", type="image/svg+xml")
-            script(src="https://cdn.tailwindcss.com")
-            script(src="https://unpkg.com/htmx.org@1.9.10", crossorigin="anonymous")
-            script(src="https://unpkg.com/htmx.org@1.9.10/dist/ext/ws.js")
-            script(src="https://unpkg.com/idiomorph@0.3.0")
-            script(src="https://unpkg.com/htmx.org/dist/ext/event-header.js")
-            link(
-                href="https://cdn.jsdelivr.net/npm/daisyui@4.7.0/dist/full.min.css",
-                rel="stylesheet",
-                type="text/css",
-            )
+            if self.with_tailwind:
+                script(src="https://cdn.tailwindcss.com")
+            if self.with_daisyui:
+                link(
+                    href=f"https://cdn.jsdelivr.net/npm/daisyui@{self.daisyui_version}/dist/full.min.css",
+                    rel="stylesheet",
+                    type="text/css",
+                )
+            if self.with_htmx:
+                script(src="https://unpkg.com/htmx.org@1.9.10", crossorigin="anonymous")
+                script(src="https://unpkg.com/htmx.org@1.9.10/dist/ext/ws.js")
+                script(src="https://unpkg.com/idiomorph@0.3.0")
+                script(src="https://unpkg.com/htmx.org/dist/ext/event-header.js")
+
             script(src="/_schorle/assets/bundle.js", crossorigin="anonymous")
             if self.extra_assets:
                 for asset in self.extra_assets:
                     asset()
 
             with title():
                 text(self.title)
```

### Comparing `schorle-0.0.8/src/schorle/effector.py` & `schorle-0.0.9/src/schorle/effector.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,55 +8,63 @@
 from typing import Callable
 
 from pydantic import BaseModel
 
 
 class Effector:
     def __init__(self, bounded_method: MethodType):
+        self.pre_actions: list[Callable] = []
         self.bounded_method = bounded_method
         self.subscribers: list[Callable] = []
 
     async def __call__(self, *args, **kwargs):
+        _tasks = [asyncio.create_task(_pre_action()) for _pre_action in self.pre_actions]
+        await asyncio.gather(*_tasks)
+
         if asyncio.iscoroutinefunction(self.bounded_method):
             await self.bounded_method(*args[1:], **kwargs)
         else:
             self.bounded_method(*args[1:], **kwargs)
 
         for subscriber in self.subscribers:
             subscriber()
 
     def subscribe(self, callback):
         self.subscribers.append(callback)
 
+    def prepend(self, _pre_action):
+        self.pre_actions.append(_pre_action)
+
 
 class EffectorProtocol(Protocol):
-    async def subscribe(self, callback, *, trigger: bool = True):
-        ...
+    def subscribe(self, callback, *, trigger: bool = True): ...
 
-    async def __call__(self, *args, **kwargs):
-        ...
+    async def __call__(self, *args, **kwargs): ...
+
+    def prepend(self, _pre_action): ...
 
 
 def create_emitter(func: MethodType) -> EffectorProtocol:
     _emitter_instance = Effector(func)
 
     async def _wrapper(*args, **kwargs):
         await _emitter_instance(*args, **kwargs)
 
-    wrapper: EffectorProtocol = wraps(func)(_wrapper)
-    wrapper.subscribe = _emitter_instance.subscribe
+    wrapper: EffectorProtocol = wraps(func)(_wrapper)  # type: ignore[assignment]
+    wrapper.subscribe = _emitter_instance.subscribe  # type: ignore[method-assign, assignment]
+    wrapper.prepend = _emitter_instance.prepend  # type: ignore[method-assign, assignment]
     return wrapper
 
 
 def effector(func: Callable) -> EffectorProtocol:
     if not asyncio.iscoroutinefunction(func):
         msg = f"Effector must be a coroutine function. {func.__name__} is not a coroutine function"
         raise ValueError(msg)
-    func.is_emitter = True
-    return func  # type: ignore
+    func.is_emitter = True  # type: ignore[attr-defined]
+    return func  # type: ignore[return-value]
 
 
 @dataclass
 class EffectorInfo:
     method: MethodType
     attr: str
```

### Comparing `schorle-0.0.8/src/schorle/element.py` & `schorle-0.0.9/src/schorle/element.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import hashlib
 
 from lxml import etree
 
 from schorle.classes import Classes
 from schorle.on import On
 from schorle.render_controller import RenderControllerMixin
+from schorle.suspense import Suspense
 from schorle.tags import HTMLTag
 
 
 class Element(RenderControllerMixin):
     def __init__(
         self,
         tag: HTMLTag,
         element_id: str | None = None,
         classes: Classes | None = None,
         style: dict[str, str] | None = None,
         on: list[On] | On | None = None,
+        suspense: Suspense | None = None,
         **attributes,
     ):
         self.tag = tag.value
         self._element_id = element_id
         self._element = self.get_element()
 
         if attributes:
@@ -35,25 +37,32 @@
 
         if element_id:
             self._element.set("id", self._element_id)
 
         if self.controller.page:
             self._element.set("hx-swap-oob", "morph")
 
-        if on and self.controller.page:
-            on = [on] if isinstance(on, On) else on
-            self._element.set("ws-send", "")
-            _triggers = ",".join([o.trigger for o in on])
-            self._element.set("hx-trigger", _triggers)
-
-            if not self._element_id:
-                self._element_id = self._generate_hash("|".join(str(id(_on.callback)) for _on in on))[:8]
-                self._element.set("id", self._element_id)
-
-            self.controller.page.reactives[self._element_id] = {_on.trigger: _on.callback for _on in on}
+        if self.controller.page:
+            if on:
+                on = [on] if isinstance(on, On) else on
+                self._element.set("ws-send", "")
+                _triggers = ",".join([o.trigger for o in on])
+                self._element.set("hx-trigger", _triggers)
+
+                if not self._element_id:
+                    self._element_id = "sle-" + self._generate_hash("|".join(str(id(_on.callback)) for _on in on))[:8]
+                    self._element.set("id", self._element_id)
+
+                self.controller.page.reactives[self._element_id] = {_on.trigger: _on.callback for _on in on}
+
+            if suspense:
+                if not self._element_id:
+                    self._element_id = "sle-" + self._generate_hash(f"suspense-{id(suspense.on)}")[:8]
+                    self._element.set("id", self._element_id)
+                suspense._parent = self._element
 
     @staticmethod
     def _generate_hash(string: str) -> str:
         return hashlib.sha256(string.encode("utf-8")).hexdigest()
 
     def get_element(self):
         elem = etree.SubElement(self.controller.current, self.tag)
@@ -85,17 +94,18 @@
 
 def element_function_factory(tag: HTMLTag):
     def func(
         element_id: str | None = None,
         classes: Classes | None = None,
         style: dict[str, str] | None = None,
         on: list[On] | On | None = None,
+        suspense: Suspense | None = None,
         **attributes,
     ):
-        return Element(tag, element_id, classes, style, on, **attributes)
+        return Element(tag, element_id, classes, style, on, suspense, **attributes)
 
     return func
 
 
 div = element_function_factory(HTMLTag.DIV)
 span = element_function_factory(HTMLTag.SPAN)
 button = element_function_factory(HTMLTag.BUTTON)
```

### Comparing `schorle-0.0.8/src/schorle/emitter.py` & `schorle-0.0.9/src/schorle/emitter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import asyncio
 
 from loguru import logger
 from lxml import etree
 from starlette.websockets import WebSocket
 
+from schorle.component import Component
 from schorle.page import Page
+from schorle.types import LXMLElement
 from schorle.utils import render_in_context
 
 
 class PageEmitter:
     def __init__(self, page: Page) -> None:
         self._page = page
 
     async def emit(self, ws: WebSocket) -> None:
         while True:
             try:
                 await asyncio.sleep(0.0001)
-                component = await self._page._render_queue.get()
-                with self._page:
-                    rendered = render_in_context(component, self._page)
-                    _html = etree.tostring(rendered, pretty_print=True).decode()
-                    await ws.send_text(_html)
+                renderable = await self._page._render_queue.get()
+                if isinstance(renderable, LXMLElement):
+                    _html = etree.tostring(renderable, pretty_print=True).decode()
+                elif isinstance(renderable, Component):
+                    with self._page:
+                        rendered = render_in_context(renderable, self._page)
+                        _html = etree.tostring(rendered, pretty_print=True).decode()
+                await ws.send_text(_html)
             except Exception as e:
                 logger.error(f"Error while emitting: {e}")
                 break
```

### Comparing `schorle-0.0.8/src/schorle/icon.py` & `schorle-0.0.9/src/schorle/icon.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/src/schorle/img.py` & `schorle-0.0.9/src/schorle/img.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/src/schorle/inputs.py` & `schorle-0.0.9/src/schorle/inputs.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/src/schorle/models.py` & `schorle-0.0.9/src/schorle/models.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/src/schorle/page.py` & `schorle-0.0.9/src/schorle/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from schorle.tags import HTMLTag
 
 
 class Page(Component):
     tag: HTMLTag = HTMLTag.DIV
     element_id: str = "schorle-page"
     reactives: dict[str, Any] = Field(default_factory=dict)
+    suspense: dict[str, Any] = Field(default_factory=dict)
     _render_queue: Queue[Component] = PrivateAttr(default_factory=Queue)
 
     def append_to_queue(self, component: Component):
         self._render_queue.put_nowait(component)
 
     @abstractmethod
     def render(self):
```

### Comparing `schorle-0.0.8/src/schorle/render_controller.py` & `schorle-0.0.9/src/schorle/render_controller.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/src/schorle/state.py` & `schorle-0.0.9/src/schorle/state.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/src/schorle/tags.py` & `schorle-0.0.9/src/schorle/tags.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/src/schorle/theme.py` & `schorle-0.0.9/src/schorle/theme.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/src/schorle/utils.py` & `schorle-0.0.9/src/schorle/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 from enum import Enum
+from typing import Any
 
-from schorle.component import Component
-from schorle.page import Page
 from schorle.render_controller import RENDER_CONTROLLER, RenderController
 from schorle.types import LXMLElement
 
 
 class RunningMode(str, Enum):
     DEV = "dev"
     PRODUCTION = "production"
@@ -17,14 +16,14 @@
     _joined_argv = " ".join(sys.argv)
     if "uvicorn" in _joined_argv and "--reload" in _joined_argv:
         return RunningMode.DEV
     else:
         return RunningMode.PRODUCTION
 
 
-def render_in_context(component: Component, page: Page | None = None) -> LXMLElement:
+def render_in_context(component: Any, page: Any | None = None) -> LXMLElement:
     token = RENDER_CONTROLLER.set(RenderController(page=page))
     try:
         component()
-        return RENDER_CONTROLLER.get().get_root().getchildren()[0]
+        return RENDER_CONTROLLER.get().get_root().getchildren()[0]  # type: ignore[attr-defined]
     finally:
         RENDER_CONTROLLER.reset(token)
```

### Comparing `schorle-0.0.8/src/schorle/assets/bundle.js` & `schorle-0.0.9/src/schorle/assets/bundle.js`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/src/schorle/assets/favicon.svg` & `schorle-0.0.9/src/schorle/assets/favicon.svg`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/tests/test_context_rendering.py` & `schorle-0.0.9/tests/test_context_rendering.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/tests/test_doc.py` & `schorle-0.0.9/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/tests/test_nested_rendering.py` & `schorle-0.0.9/tests/test_nested_rendering.py`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/tests/test_reactive.py` & `schorle-0.0.9/tests/test_reactive.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,45 +7,49 @@
 from schorle.page import Page
 from schorle.state import ReactiveModel
 from schorle.text import text
 from schorle.types import LXMLElement
 from schorle.utils import render_in_context
 
 
-def test_reactive():
-    class Sample(ReactiveModel):
-        count: int = 0
+class Sample(ReactiveModel):
+    count: int = 0
+
+    @effector
+    async def increment(self):
+        self.count += 1
+
+
+class Another(Component):
+    def render(self):
+        with span():
+            text("Something")
+
+
+class View(Component):
+    counter: Sample
 
-        @effector
-        async def increment(self):
-            self.count += 1
-
-    class Another(Component):
-        def render(self):
-            with span():
-                text("Something")
-
-    class View(Component):
-        counter: Sample
-
-        def render(self):
-            with button(classes=Classes("btn btn-primary")):
-                text(f"Clicked {self.counter.count} times")
-            Another()
-
-        def __init__(self, **data):
-            super().__init__(**data)
-            self.bind(self.counter)
-
-    class ViewPage(Page):
-        counter: Sample = Field(default_factory=Sample)
-
-        def render(self):
-            with div(classes=Classes("flex justify-center items-center h-screen")):
-                View(counter=self.counter, element_id="v1")
-            View(counter=self.counter)
+    def render(self):
+        with button(classes=Classes("btn btn-primary")):
+            text(f"Clicked {self.counter.count} times")
+        Another()
 
+    def __init__(self, **data):
+        super().__init__(**data)
+        self.bind(self.counter)
+
+
+class ViewPage(Page):
+    counter: Sample = Field(default_factory=Sample)
+
+    def render(self):
+        with div(classes=Classes("flex justify-center items-center h-screen")):
+            View(counter=self.counter, element_id="v1")
+        View(counter=self.counter)
+
+
+def test_reactive():
     vp = ViewPage()
 
     with vp:
         r1 = render_in_context(vp)
         assert isinstance(r1, LXMLElement)
```

### Comparing `schorle-0.0.8/.gitignore` & `schorle-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/LICENSE.md` & `schorle-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/README.md` & `schorle-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `schorle-0.0.8/pyproject.toml` & `schorle-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,19 @@
 cov = ["test-cov", "cov-report"]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
-dependencies = ["black>=23.1.0", "mypy>=1.0.0", "ruff>=0.0.243"]
+dependencies = [
+    "black>=24.2.0,<25.0.0",
+    "mypy>=1.0.0,<2.0.0",
+    "ruff>=0.2.2,<0.3.0",
+]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/schorle tests}"
 style = ["ruff {args:.}", "black --check --diff {args:.}"]
 fmt = ["black {args:.}", "ruff --fix {args:.}", "style"]
 all = ["style", "typing"]
 
 [tool.black]
@@ -132,14 +136,15 @@
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
+"examples/**/*" = ["S311"]
 
 [tool.coverage.run]
 source_pkgs = ["schorle", "tests"]
 source = ["src/schorle"]
 branch = true
 parallel = true
 omit = ["src/schorle/__about__.py"]
```

### Comparing `schorle-0.0.8/PKG-INFO` & `schorle-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schorle
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Documentation, https://github.com/renardeinside/schorle#readme
 Project-URL: Issues, https://github.com/renardeinside/schorle/issues
 Project-URL: Source, https://github.com/renardeinside/schorle
 Author-email: renardeinside <polarpersonal@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: async,python,server-driven-ui,ui
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: schorle Version: 0.0.8 Project-URL: Documentation,
+Metadata-Version: 2.1 Name: schorle Version: 0.0.9 Project-URL: Documentation,
 https://github.com/renardeinside/schorle#readme Project-URL: Issues, https://
 github.com/renardeinside/schorle/issues Project-URL: Source, https://
 github.com/renardeinside/schorle Author-email: renardeinside
 gmail.com> License-Expression: MIT License-File: LICENSE.md Keywords:
 async,python,server-driven-ui,ui Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

