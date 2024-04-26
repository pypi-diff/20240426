# Comparing `tmp/pypomes_http-0.1.4.tar.gz` & `tmp/pypomes_http-0.1.5.tar.gz`

## Comparing `pypomes_http-0.1.4.tar` & `pypomes_http-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/src/pypomes_http/__init__.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/src/pypomes_http/http_async.py
--rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/src/pypomes_http/http_pomes.py
--rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/src/pypomes_http/http_statuses.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pypomes_http-0.1.5/src/pypomes_http/__init__.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pypomes_http-0.1.5/src/pypomes_http/http_async.py
+-rw-r--r--   0        0        0    16862 2020-02-02 00:00:00.000000 pypomes_http-0.1.5/src/pypomes_http/http_pomes.py
+-rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 pypomes_http-0.1.5/src/pypomes_http/http_statuses.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.5/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.5/PKG-INFO
```

### Comparing `pypomes_http-0.1.4/src/pypomes_http/__init__.py` & `pypomes_http-0.1.5/src/pypomes_http/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 )
 from .http_pomes import (
     HTTP_DELETE_TIMEOUT, HTTP_GET_TIMEOUT, HTTP_PATCH_TIMEOUT, HTTP_POST_TIMEOUT, HTTP_PUT_TIMEOUT,
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
     http_status_code, http_status_name, http_status_description,
-    http_get_parameter, http_get_parameters,
+    http_get_parameter, http_get_parameters, http_get_parameter_as_list,
     http_delete, http_get, http_patch, http_post, http_put,
 )
 
 __all__ = [
     # http_async
     "HttpAsync",
     # http_pomes
     "HTTP_DELETE_TIMEOUT", "HTTP_GET_TIMEOUT", "HTTP_PATCH_TIMEOUT", "HTTP_POST_TIMEOUT", "HTTP_PUT_TIMEOUT",
     "MIMETYPE_BINARY", "MIMETYPE_CSS", "MIMETYPE_CSV", "MIMETYPE_HTML", "MIMETYPE_JAVASCRIPT",
     "MIMETYPE_JSON", "MIMETYPE_MULTIPART", "MIMETYPE_PDF", "MIMETYPE_PKCS7", "MIMETYPE_SOAP",
     "MIMETYPE_TEXT", "MIMETYPE_URLENCODED", "MIMETYPE_XML", "MIMETYPE_ZIP",
     "http_status_code", "http_status_name", "http_status_description",
-    "http_get_parameter", "http_get_parameters",
+    "http_get_parameter", "http_get_parameters", "http_get_parameter_as_list",
     "http_delete", "http_get", "http_patch", "http_post", "http_put",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_http")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_http-0.1.4/src/pypomes_http/http_async.py` & `pypomes_http-0.1.5/src/pypomes_http/http_async.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.4/src/pypomes_http/http_pomes.py` & `pypomes_http-0.1.5/src/pypomes_http/http_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     item: dict = _HTTP_STATUSES.get(status_code)
     return (item or {"en": "Unknown status code", "pt": "Status desconhecido"}).get(lang)
 
 
 def http_get_parameter(request: Request,
                        param: str) -> Any:
     """
-    Obtain the *request*'s input parameter name *param_name*.
+    Obtain the *request*'s input parameter named *param_name*.
 
     Until *param* is found, the following are sequentially attempted:
         - elements in a HTML form
         - parameters in the URL's query part
         - key/value pairs in a *JSON* structure in the request's body
 
     :param request: the Request object
@@ -139,14 +139,46 @@
 
     # obtain parameters in form
     result.update(request.form)
 
     return result
 
 
+def http_get_parameter_as_list(request: Request,
+                               param: str) -> list[Any]:
+    """
+    Obtain the *request*'s input parameter named *param_name* as a list.
+
+    Until *param* is found, the following are sequentially attempted:
+        - elements in a HTML form
+        - parameters in the URL's query part
+        - key/value pairs in a *JSON* structure in the request's body
+
+    :param request: the Request object
+    :param param: name of parameter to retrieve
+    :return: the parameter's value as a list, or 'None' if not found
+    """
+    # initialize the return variable
+    result: list[Any] | None = None
+
+    # obtain the parameter's raw valuw
+    value: Any = http_get_parameter(request, param)
+
+    # is 'value' a list ?
+    if isinstance(value, list):
+        # yes, return it
+        result = value
+    # is 'value' a string ?
+    elif isinstance(value, str):
+        # yes, split it into a list
+        result = value.split(sep=",")
+
+    return result
+
+
 def http_delete(errors: list[str] | None,
                 url: str,
                 headers: dict = None,
                 params: dict = None,
                 data: dict = None,
                 json: dict = None, auth: str = None,
                 timeout: int | None = HTTP_DELETE_TIMEOUT,
```

### Comparing `pypomes_http-0.1.4/src/pypomes_http/http_statuses.py` & `pypomes_http-0.1.5/src/pypomes_http/http_statuses.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.4/LICENSE` & `pypomes_http-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.4/pyproject.toml` & `pypomes_http-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_http"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (HTTP modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes_core>=0.8.7",
+    "pypomes_core>=0.8.9",
     "pypomes_security>=0.1.3",
     "requests>=2.31.0",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
```

### Comparing `pypomes_http-0.1.4/PKG-INFO` & `pypomes_http-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_http
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of Python pomes, pennyeach (HTTP modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-HTTP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-HTTP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.8.7
+Requires-Dist: pypomes-core>=0.8.9
 Requires-Dist: pypomes-security>=0.1.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

