# Comparing `tmp/hypermedia-2.0.0.tar.gz` & `tmp/hypermedia-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypermedia-2.0.0.tar", max compression
+gzip compressed data, was "hypermedia-2.0.1.tar", max compression
```

## Comparing `hypermedia-2.0.0.tar` & `hypermedia-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1080 2024-04-17 17:19:24.803724 hypermedia-2.0.0/LICENSE
--rw-r--r--   0        0        0     1439 2024-04-17 17:19:24.803873 hypermedia-2.0.0/README.md
--rw-r--r--   0        0        0     4952 2024-04-17 19:20:13.717395 hypermedia-2.0.0/hypermedia/__init__.py
--rw-r--r--   0        0        0      516 2024-04-17 19:17:59.497657 hypermedia-2.0.0/hypermedia/audio_and_video.py
--rw-r--r--   0        0        0     2051 2024-04-17 19:20:13.717812 hypermedia-2.0.0/hypermedia/basic.py
--rw-r--r--   0        0        0     4712 2024-04-17 19:17:59.498633 hypermedia-2.0.0/hypermedia/formatting.py
--rw-r--r--   0        0        0     1369 2024-04-17 19:17:59.498990 hypermedia-2.0.0/hypermedia/forms_and_input.py
--rw-r--r--   0        0        0      131 2024-04-17 19:17:59.499322 hypermedia-2.0.0/hypermedia/frames.py
--rw-r--r--   0        0        0     2448 2024-04-17 19:17:59.499658 hypermedia-2.0.0/hypermedia/htmx.py
--rw-r--r--   0        0        0      973 2024-04-17 19:17:59.499939 hypermedia-2.0.0/hypermedia/images.py
--rw-r--r--   0        0        0      440 2024-04-17 19:17:59.500223 hypermedia-2.0.0/hypermedia/links.py
--rw-r--r--   0        0        0     1017 2024-04-17 19:17:59.500527 hypermedia-2.0.0/hypermedia/lists.py
--rw-r--r--   0        0        0      270 2024-04-17 19:17:59.500801 hypermedia-2.0.0/hypermedia/meta_info.py
--rw-r--r--   0        0        0     5670 2024-04-17 19:17:59.501060 hypermedia-2.0.0/hypermedia/models.py
--rw-r--r--   0        0        0      500 2024-04-17 19:17:59.501352 hypermedia-2.0.0/hypermedia/programming.py
--rw-r--r--   0        0        0        0 2024-04-17 17:19:24.805780 hypermedia-2.0.0/hypermedia/py.typed
--rw-r--r--   0        0        0     1645 2024-04-17 19:17:59.501607 hypermedia-2.0.0/hypermedia/styles_and_semantics.py
--rw-r--r--   0        0        0     1485 2024-04-17 19:17:59.501834 hypermedia-2.0.0/hypermedia/tables.py
--rw-r--r--   0        0        0     2999 2024-04-17 19:21:11.408899 hypermedia-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 hypermedia-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-17 17:19:24.803724 hypermedia-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1439 2024-04-17 17:19:24.803873 hypermedia-2.0.1/README.md
+-rw-r--r--   0        0        0     4952 2024-04-17 19:20:13.717395 hypermedia-2.0.1/hypermedia/__init__.py
+-rw-r--r--   0        0        0      516 2024-04-17 19:17:59.497657 hypermedia-2.0.1/hypermedia/audio_and_video.py
+-rw-r--r--   0        0        0     2051 2024-04-17 19:20:13.717812 hypermedia-2.0.1/hypermedia/basic.py
+-rw-r--r--   0        0        0     4712 2024-04-17 19:17:59.498633 hypermedia-2.0.1/hypermedia/formatting.py
+-rw-r--r--   0        0        0     1369 2024-04-17 19:17:59.498990 hypermedia-2.0.1/hypermedia/forms_and_input.py
+-rw-r--r--   0        0        0      131 2024-04-17 19:17:59.499322 hypermedia-2.0.1/hypermedia/frames.py
+-rw-r--r--   0        0        0     2254 2024-04-26 17:51:13.966308 hypermedia-2.0.1/hypermedia/htmx.py
+-rw-r--r--   0        0        0      973 2024-04-17 19:17:59.499939 hypermedia-2.0.1/hypermedia/images.py
+-rw-r--r--   0        0        0      440 2024-04-17 19:17:59.500223 hypermedia-2.0.1/hypermedia/links.py
+-rw-r--r--   0        0        0     1017 2024-04-17 19:17:59.500527 hypermedia-2.0.1/hypermedia/lists.py
+-rw-r--r--   0        0        0      270 2024-04-17 19:17:59.500801 hypermedia-2.0.1/hypermedia/meta_info.py
+-rw-r--r--   0        0        0     5670 2024-04-17 19:17:59.501060 hypermedia-2.0.1/hypermedia/models.py
+-rw-r--r--   0        0        0      500 2024-04-17 19:17:59.501352 hypermedia-2.0.1/hypermedia/programming.py
+-rw-r--r--   0        0        0        0 2024-04-17 17:19:24.805780 hypermedia-2.0.1/hypermedia/py.typed
+-rw-r--r--   0        0        0     1645 2024-04-17 19:17:59.501607 hypermedia-2.0.1/hypermedia/styles_and_semantics.py
+-rw-r--r--   0        0        0     1485 2024-04-17 19:17:59.501834 hypermedia-2.0.1/hypermedia/tables.py
+-rw-r--r--   0        0        0     2999 2024-04-26 17:51:13.966736 hypermedia-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 hypermedia-2.0.1/PKG-INFO
```

### Comparing `hypermedia-2.0.0/LICENSE` & `hypermedia-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/README.md` & `hypermedia-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/hypermedia/__init__.py` & `hypermedia-2.0.1/hypermedia/__init__.py`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/hypermedia/audio_and_video.py` & `hypermedia-2.0.1/hypermedia/audio_and_video.py`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/hypermedia/basic.py` & `hypermedia-2.0.1/hypermedia/basic.py`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/hypermedia/formatting.py` & `hypermedia-2.0.1/hypermedia/formatting.py`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/hypermedia/forms_and_input.py` & `hypermedia-2.0.1/hypermedia/forms_and_input.py`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/hypermedia/htmx.py` & `hypermedia-2.0.1/hypermedia/htmx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 from functools import wraps
 from typing import (
     Any,
     Callable,
     Coroutine,
-    Mapping,
     ParamSpec,
     Protocol,
     TypeVar,
 )
 
 from hypermedia.models import Element
 
 Param = ParamSpec("Param")
 ReturnType = TypeVar("ReturnType")
 
 
-class RequestWithHeaders(Protocol):
-    """Protocol for FastAPI's Request class."""
-
-    headers: Mapping[str, str]
-
-
 class RequestPartialAndFull(Protocol):
     """Requires, `request`, `partial` and `full` args on decorated function."""
 
     def __call__(  # noqa: D102
-        self, request: RequestWithHeaders, partial: Element, full: Element
+        self, request: Any, partial: Element, full: Element
     ) -> Coroutine[Any, Any, None]: ...
 
 
 class RequestAndPartial(Protocol):
     """Requires, `request` and `partial` args on decorated function."""
 
     def __call__(  # noqa: D102
-        self, request: RequestWithHeaders, partial: Element
+        self, request: Any, partial: Element
     ) -> Coroutine[Any, Any, None]: ...
 
 
 def htmx(
     func: RequestPartialAndFull | RequestAndPartial,
 ) -> Callable[..., str]:
     """
@@ -54,26 +47,28 @@
     Make sure to use the `@full` decorator on the full renderer to prevent
     it from being evaluated before it is needed.
     """
 
     @wraps(func)
     async def wrapper(
         *,
-        request: RequestWithHeaders,
+        request: Any,
         partial: Element,
         full: None | Callable[..., Element] = None,
     ) -> str:
         """Wrap function."""
         hx_request = "HX-Request" in request.headers
         if hx_request:
             return partial.dump()
 
-        # should probably return some http error if user tries to get a
-        # full page load when its not expected.
-        return full().dump() if full else ""
+        # Return partial if full render is not available.
+        if full is None:
+            return partial.dump()
+
+        return full().dump()
 
     return wrapper  # type: ignore
 
 
 def full(
     func: Callable[Param, ReturnType],
 ) -> Callable[Param, Coroutine[Any, Any, Callable[[], ReturnType]]]:
```

### Comparing `hypermedia-2.0.0/hypermedia/images.py` & `hypermedia-2.0.1/hypermedia/images.py`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/hypermedia/lists.py` & `hypermedia-2.0.1/hypermedia/lists.py`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/hypermedia/models.py` & `hypermedia-2.0.1/hypermedia/models.py`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/hypermedia/styles_and_semantics.py` & `hypermedia-2.0.1/hypermedia/styles_and_semantics.py`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/hypermedia/tables.py` & `hypermedia-2.0.1/hypermedia/tables.py`

 * *Files identical despite different names*

### Comparing `hypermedia-2.0.0/pyproject.toml` & `hypermedia-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hypermedia"
-version = "2.0.0"
+version = "2.0.1"
 description = "An opinionated way to work with html in pure python with htmx support."
 authors = ["Thomas Borgen <thomasborgen91@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/thomasborgen/hypermedia"
 repository = "https://github.com/thomasborgen/hypermedia"
 keywords = ["HTML", "HTMX", "Extendable", "Partial HTML", "HTML Templating", "FastAPI"]
```

### Comparing `hypermedia-2.0.0/PKG-INFO` & `hypermedia-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypermedia
-Version: 2.0.0
+Version: 2.0.1
 Summary: An opinionated way to work with html in pure python with htmx support.
 Home-page: https://github.com/thomasborgen/hypermedia
 License: MIT
 Keywords: HTML,HTMX,Extendable,Partial HTML,HTML Templating,FastAPI
 Author: Thomas Borgen
 Author-email: thomasborgen91@gmail.com
 Requires-Python: >=3.10,<4.0
```

