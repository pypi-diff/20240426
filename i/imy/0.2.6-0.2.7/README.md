# Comparing `tmp/imy-0.2.6.tar.gz` & `tmp/imy-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.2.6.tar", max compression
+gzip compressed data, was "imy-0.2.7.tar", max compression
```

## Comparing `imy-0.2.6.tar` & `imy-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.6/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.6/README.md
--rw-r--r--   0        0        0        0 2024-04-08 18:10:47.446922 imy-0.2.6/imy/__init__.py
--rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.6/imy/assets.py
--rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.6/imy/async_utils.py
--rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.6/imy/config.py
--rw-r--r--   0        0        0       71 2024-04-18 06:50:34.243007 imy-0.2.6/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     5072 2024-04-18 07:34:38.648724 imy-0.2.6/imy/docstrings/data_models.py
--rw-r--r--   0        0        0    16636 2024-04-20 10:16:34.262937 imy-0.2.6/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8572 2024-04-10 14:07:52.133967 imy-0.2.6/imy/inject.py
--rw-r--r--   0        0        0    13613 2024-04-10 14:10:43.230681 imy-0.2.6/imy/logs.py
--rw-r--r--   0        0        0     3185 2024-04-19 18:44:30.576908 imy-0.2.6/imy/package_metadata.py
--rw-r--r--   0        0        0      754 2024-04-20 10:17:16.242959 imy-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.7/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.2.7/imy/__init__.py
+-rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.2.7/imy/assets.py
+-rw-r--r--   0        0        0     6011 2024-04-22 13:27:52.000000 imy-0.2.7/imy/async_utils.py
+-rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.2.7/imy/config.py
+-rw-r--r--   0        0        0       71 2024-04-22 13:27:52.000000 imy-0.2.7/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     6302 2024-04-26 05:51:19.364642 imy-0.2.7/imy/docstrings/data_models.py
+-rw-r--r--   0        0        0    16683 2024-04-25 22:21:42.250990 imy-0.2.7/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.2.7/imy/inject.py
+-rw-r--r--   0        0        0    13613 2024-04-22 13:27:52.000000 imy-0.2.7/imy/logs.py
+-rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.2.7/imy/package_metadata.py
+-rw-r--r--   0        0        0      754 2024-04-26 06:20:20.992955 imy-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.7/PKG-INFO
```

### Comparing `imy-0.2.6/LICENSE` & `imy-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.2.6/imy/assets.py` & `imy-0.2.7/imy/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         """
         Ensures that the given asset is extracted and returns a path to it. This
         is useful for assets that are not opened with `open_asset`. If you want
         to open the file use that function instead.
 
         Returns a path to where the extracted asset is located.
 
-        ## Args
+        ## Parameters
 
         path: The relative path to the asset.
 
         compressed: Whether the asset is compressed. If it is, the function will
             ensure that the asset is extracted before returning the path.
             Uncompressed assets are returned as-is.
 
@@ -151,15 +151,15 @@
         compressed: bool = True,
     ) -> IO:
         """
         Opens an asset file for reading.
 
         Returns a file-like object.
 
-        ## Args
+        ## Parameters
 
         path: The relative path to the asset.
 
         mode: The mode to open the file in. The default is `"r"`.
 
         compressed: Whether the asset is compressed. If it is, the function will
             ensure that the asset is extracted before opening it. Uncompressed
```

### Comparing `imy-0.2.6/imy/async_utils.py` & `imy-0.2.7/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.6/imy/config.py` & `imy-0.2.7/imy/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 __all__ = [
     "ConfigurationError",
     "Config",
 ]
 
 
-_DEFAULTS_BY_TYPE: dict[Type, Any] = {
+_DEFAULTS_BY_TYPE: dict[Type, uniserde.Jsonable] = {
     Any: None,
     bool: False,
     bytes: b"",
-    datetime: datetime.now(),
+    datetime: datetime.now().isoformat(),
     dict: {},
     enum.Enum: "",
     enum.Flag: [],
     float: 0.0,
     int: 0,
     list: [],
     Literal: "",
     set: set(),
     str: "",
-    timedelta: timedelta(),
+    timedelta: 0,
     tuple: tuple(),
     Union: None,
     ObjectId: "",
 }  # type: ignore
 
 
 class ConfigurationError(ValueError):
@@ -97,15 +97,15 @@
             trailing_commas=True,
         )
 
         # Add comments describing the fields
         serialized = serialized.strip()
         lines = serialized.splitlines()
 
-        for ii, line in enumerate(lines[1:-1]):
+        for ii, line in enumerate(lines[1:-1], start=1):
             lines[ii] = "  // " + line.strip()
 
         # Done
         return "\n".join(lines) + "\n"
 
     @classmethod
     def _parse_fields(
```

### Comparing `imy-0.2.6/imy/docstrings/data_models.py` & `imy-0.2.7/imy/docstrings/data_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import introspection.types
 import introspection.typing
 
 from . import parsers
 
 __all__ = [
     "Unset",
+    "UNSET",
     "CommonMetadata",
     "Docstring",
     "FunctionParameter",
     "FunctionDocs",
     "ClassField",
     "ClassDocs",
 ]
@@ -29,16 +30,22 @@
 @dataclass
 class CommonMetadata:
     """
     Some metadata such as whether an object is public or not is shared between
     different types of objects. This class is used to hold that metadata.
     """
 
+    # Whether the object is meant to be used by users of the library, or if it's
+    # an internal implementation detail.
     public: bool
 
+    # If `True`, this object is not yet ready for public use. Its API may change
+    # between even patch releases.
+    experimental: bool
+
     @staticmethod
     def _parse_bool(
         metadata: dict[str, str],
         key_name: str,
         default_value: bool | None,
     ) -> bool:
         """
@@ -66,26 +73,61 @@
         if raw == "False":
             return False
 
         # Invalid value
         raise ValueError(f"Invalid value for `{key_name}` in metadata: {raw}")
 
     @staticmethod
+    def _parse_literal(
+        metadata: dict[str, str],
+        key_name: str,
+        options: Set[str],
+        default_value: str | None,
+    ) -> str:
+        """
+        Attempts to parse a literal value from metadata.
+
+        ## Raises
+
+        `ValueError`: If the key is missing or invalid.
+        """
+
+        # Try to get the value
+        try:
+            raw = metadata[key_name]
+        except KeyError:
+            # No value provided
+            if default_value is None:
+                raise ValueError(f"Missing value for `{key_name}` in metadata")
+
+            return default_value
+
+        # Check if the value is valid
+        if raw not in options:
+            raise ValueError(f"Invalid value for `{key_name}` in metadata: {raw}")
+
+        return raw
+
+    @staticmethod
     def from_dictionary(metadata: dict[str, Any]) -> CommonMetadata:
         """
         Parses a `CommonMetadata` object from a dictionary. This is useful for
         parsing metadata from a docstring key section.
         """
 
         # Parse all values
         public = CommonMetadata._parse_bool(metadata, "public", default_value=True)
+        experimental = CommonMetadata._parse_bool(
+            metadata, "experimental", default_value=False
+        )
 
         # Construct the result
         return CommonMetadata(
             public=public,
+            experimental=experimental,
         )
 
 
 @dataclass
 class FunctionMetadata(CommonMetadata):
     @staticmethod
     def from_dictionary(metadata: dict[str, Any]) -> FunctionMetadata:
```

### Comparing `imy-0.2.6/imy/docstrings/parsers.py` & `imy-0.2.7/imy/docstrings/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     result is the part of the string before the first heading, and a dictionary
     mapping the heading names to the text of the sections ("the summary").
 
     If the docstring starts with a heading it will not create a separate section
     and the text of that section will be considered part of the summary.
     """
     # Drop the title if it exists
-    if docstring.startswith("#"):
+    if docstring.startswith("#") and not docstring.startswith("##"):
         docstring = docstring.split("\n", 1)[1]
 
     # Split the docstring into sections
     sections: dict[str, list[str]] = {}
     details: list[str] = []
     current_section: list[str] = details
 
@@ -324,22 +324,22 @@
         parsed = data_models.Docstring(summary=None, details=None, key_sections={})
         raises = []
         metadata = data_models.FunctionMetadata.from_dictionary({})
     else:
         parsed = parse_docstring(
             docstring,
             key_sections=[
-                "args",
+                "parameters",
                 "raises",
                 "metadata",
             ],
         )
 
         # Add any information learned about parameters from the docstring
-        for param_name, param_details in parsed.key_sections["args"].items():
+        for param_name, param_details in parsed.key_sections["parameters"].items():
             try:
                 result_param = parameters[param_name]
             except KeyError:
                 warnings.warn(
                     f"The docstring for function `{func.__name__}` mentions a parameter `{param_name}` that does not exist in the function signature."
                 )
                 continue
```

### Comparing `imy-0.2.6/imy/inject.py` & `imy-0.2.7/imy/inject.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,26 +167,26 @@
         # Try to find a factory that can create the item
         try:
             factory_param_types, factory = self._factories[key]
         except KeyError:
             raise KeyError(raw_key)
 
         # Get all of the factory's dependencies
-        factory_args: list[Any] = []
+        factory_params: list[Any] = []
 
         for param_type in factory_param_types:
-            factory_args.append(
+            factory_params.append(
                 self._get(
                     param_type,
                     in_flight=in_flight + [key],
                 )
             )
 
         # Create the item, register it and return
-        item = factory(*factory_args)
+        item = factory(*factory_params)
         self._components[key] = item
 
         return item
 
     def __getitem__(self, key: Type[T]) -> T:
         """
         Given an item type, return the component of that type.
```

### Comparing `imy-0.2.6/imy/logs.py` & `imy-0.2.7/imy/logs.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.6/imy/package_metadata.py` & `imy-0.2.7/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.6/pyproject.toml` & `imy-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.2.6"
+version = "0.2.7"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.2.6/PKG-INFO` & `imy-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.2.6
+Version: 0.2.7
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

