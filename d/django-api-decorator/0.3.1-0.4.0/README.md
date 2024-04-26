# Comparing `tmp/django_api_decorator-0.3.1.tar.gz` & `tmp/django_api_decorator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_api_decorator-0.3.1.tar", max compression
+gzip compressed data, was "django_api_decorator-0.4.0.tar", max compression
```

## Comparing `django_api_decorator-0.3.1.tar` & `django_api_decorator-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1076 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/LICENSE
--rw-r--r--   0        0        0     2697 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/__init__.py
--rw-r--r--   0        0        0      390 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/apps.py
--rw-r--r--   0        0        0    12735 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/decorators.py
--rw-r--r--   0        0        0        0 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/management/commands/__init__.py
--rw-r--r--   0        0        0      920 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/management/commands/generate_api_schemas.py
--rw-r--r--   0        0        0     9675 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/openapi.py
--rw-r--r--   0        0        0        0 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/py.typed
--rw-r--r--   0        0        0     1552 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/schema_file.py
--rw-r--r--   0        0        0     1037 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/types.py
--rw-r--r--   0        0        0     1993 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/utils.py
--rw-r--r--   0        0        0     1077 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 django_api_decorator-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-26 15:57:17.740021 django_api_decorator-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2697 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/__init__.py
+-rw-r--r--   0        0        0      390 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/apps.py
+-rw-r--r--   0        0        0    13393 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/decorators.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/management/commands/__init__.py
+-rw-r--r--   0        0        0      920 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/management/commands/generate_api_schemas.py
+-rw-r--r--   0        0        0     9675 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/openapi.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/py.typed
+-rw-r--r--   0        0        0     1552 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/schema_file.py
+-rw-r--r--   0        0        0     1037 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/types.py
+-rw-r--r--   0        0        0     2850 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/django_api_decorator/utils.py
+-rw-r--r--   0        0        0     1077 2024-04-26 15:57:17.744021 django_api_decorator-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 django_api_decorator-0.4.0/PKG-INFO
```

### Comparing `django_api_decorator-0.3.1/LICENSE` & `django_api_decorator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.1/README.md` & `django_api_decorator-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.1/django_api_decorator/decorators.py` & `django_api_decorator-0.4.0/django_api_decorator/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from django.http import Http404, HttpRequest, HttpResponse, JsonResponse
 from django.views.decorators.http import require_http_methods
 from pydantic.fields import FieldInfo
 from pydantic.functional_validators import BeforeValidator
 from pydantic_core import PydanticUndefined
 
 from .types import ApiMeta, FieldError, PublicAPIError
+from .utils import get_list_fields, parse_form_encoded_body
 
 P = typing.ParamSpec("P")
 T = typing.TypeVar("T")
 
 Annotation = Any
 ExceptionHandler = Callable[
     [HttpRequest, ValidationError | pydantic.ValidationError], HttpResponse
@@ -97,17 +98,17 @@
         # the requests query parameters.
         query_params_model = _get_query_params_model(
             parameters=signature.parameters, query_params=query_params or []
         )
 
         # If the method has a "body" argument, get a function to call to parse
         # the request body into the type expected by the view.
-        body_adapter = None
-        if "body" in signature.parameters:
-            body_adapter = _get_body_adapter(parameter=signature.parameters["body"])
+        list_fields, body_adapter = set[str](), None
+        if body_annotation := signature.parameters.get("body"):
+            list_fields, body_adapter = _get_body_adapter(body_annotation)
 
         # Get a function to use for encoding the value returned from the view
         # into a request we can return to the client.
         response_adapter = _get_response_adapter(
             type_annotation=signature.return_annotation
         )
 
@@ -122,15 +123,22 @@
 
             try:
                 extra_kwargs = {}
 
                 # Parse the request body if the request method allows a body and the
                 # view has requested that we should parse the body.
                 if _can_have_body(request.method) and body_adapter:
-                    extra_kwargs["body"] = body_adapter.validate_json(request.body)
+                    if request.content_type in {
+                        "application/x-www-form-urlencoded",
+                        "multipart/form-data",
+                    }:
+                        data = parse_form_encoded_body(request, list_fields)
+                        extra_kwargs["body"] = body_adapter.validate_python(data)
+                    else:
+                        extra_kwargs["body"] = body_adapter.validate_json(request.body)
 
                 # Parse query params and add them to the parameters given to the view.
                 raw_query_params: dict[str, Any] = {}
                 for key in request.GET:
                     if value := request.GET.getlist(key):
                         raw_query_params[key] = value[0] if len(value) == 1 else value
                     else:
@@ -257,20 +265,26 @@
 ################
 
 
 def _can_have_body(method: str | None) -> bool:
     return method in ("POST", "PATCH", "PUT")
 
 
-def _get_body_adapter(*, parameter: inspect.Parameter) -> pydantic.TypeAdapter[Any]:
+def _get_body_adapter(
+    parameter: inspect.Parameter,
+) -> tuple[set[str], pydantic.TypeAdapter[Any]]:
     annotation = parameter.annotation
     if annotation is inspect.Parameter.empty:
         raise TypeError("The body parameter must have a type annotation")
 
-    return pydantic.TypeAdapter(annotation)
+    list_fields = set()
+    if isinstance(annotation, type) and issubclass(annotation, pydantic.BaseModel):
+        list_fields = get_list_fields(annotation)
+
+    return list_fields, pydantic.TypeAdapter(annotation)
 
 
 #####################
 # Response encoding #
 #####################
```

### Comparing `django_api_decorator-0.3.1/django_api_decorator/management/commands/generate_api_schemas.py` & `django_api_decorator-0.4.0/django_api_decorator/management/commands/generate_api_schemas.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.1/django_api_decorator/openapi.py` & `django_api_decorator-0.4.0/django_api_decorator/openapi.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.1/django_api_decorator/schema_file.py` & `django_api_decorator-0.4.0/django_api_decorator/schema_file.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.1/django_api_decorator/types.py` & `django_api_decorator-0.4.0/django_api_decorator/types.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.1/django_api_decorator/utils.py` & `django_api_decorator-0.4.0/django_api_decorator/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from typing import Callable, ParamSpec, cast
+from types import UnionType
+from typing import Any, Callable, List, ParamSpec, Set, Tuple, Union, cast, get_origin
 
 from django.http import HttpRequest, HttpResponse, HttpResponseNotAllowed
+from pydantic import BaseModel
 
 P = ParamSpec("P")
 
 
 def method_router(
     csrf_exempt: bool | None = None,
     **views: Callable[..., HttpResponse],
@@ -54,7 +56,37 @@
         return view(request, *args, **kwargs)
 
     call_view.csrf_exempt = csrf_exempt  # type: ignore[attr-defined]
 
     call_view._method_router_views = views  # type: ignore[attr-defined]
 
     return cast(Callable[..., HttpResponse], call_view)
+
+
+def is_list_type(annotation: Any) -> bool:
+    """
+    Check if the given annotation is a collection type.
+    """
+
+    origin = get_origin(annotation)
+    return origin in (Union, UnionType, List, Tuple, Set, list, set, tuple)
+
+
+def get_list_fields(model: type[BaseModel]) -> set[str]:
+    return {
+        name
+        for name, field in model.model_fields.items()
+        if is_list_type(field.annotation)
+    }
+
+
+def parse_form_encoded_body(
+    request: HttpRequest, list_fields: set[str]
+) -> dict[str, str | list[str] | None]:
+    """
+    Convert request.POST to a format pydantic can take as input
+    """
+
+    return {
+        key: request.POST.getlist(key) if key in list_fields else request.POST.get(key)
+        for key in request.POST
+    }
```

### Comparing `django_api_decorator-0.3.1/pyproject.toml` & `django_api_decorator-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "django-api-decorator"
-version = "0.3.1"
+version = "0.4.0"
 description = "A collection of tools to build function based Django APIs"
 authors = ["Oda <tech@oda.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/django-api-decorator"
 repository = "https://github.com/kolonialno/django-api-decorator"
 packages = [{include = "django_api_decorator"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 Django = ">=3"
 pydantic = "^2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 black = ">=23.3,<25.0"
```

### Comparing `django_api_decorator-0.3.1/PKG-INFO` & `django_api_decorator-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: django-api-decorator
-Version: 0.3.1
+Version: 0.4.0
 Summary: A collection of tools to build function based Django APIs
 Home-page: https://github.com/kolonialno/django-api-decorator
 License: MIT
 Author: Oda
 Author-email: tech@oda.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=3)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Repository, https://github.com/kolonialno/django-api-decorator
 Description-Content-Type: text/markdown
```

