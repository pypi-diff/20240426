# Comparing `tmp/python_ulid-2.4.0.post0.tar.gz` & `tmp/python_ulid-2.5.0.tar.gz`

## Comparing `python_ulid-2.4.0.post0.tar` & `python_ulid-2.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/.readthedocs.yml
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/CHANGELOG.rst
--rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/README.rst
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/logo.png
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/docs/Makefile
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/docs/requirements.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/docs/source/api.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/docs/source/changelog.rst
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/docs/source/conf.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/tests/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/tests/test_base32.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/tests/test_cli.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/tests/test_ulid.py
--rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/ulid/__init__.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/ulid/__main__.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/ulid/base32.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/ulid/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/ulid/py.typed
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/LICENSE
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/hatch.toml
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/pyproject.toml
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 python_ulid-2.4.0.post0/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 python_ulid-2.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 python_ulid-2.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 python_ulid-2.5.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 python_ulid-2.5.0/README.rst
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 python_ulid-2.5.0/logo.png
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 python_ulid-2.5.0/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_ulid-2.5.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/Makefile
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/requirements.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/source/api.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/source/conf.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 python_ulid-2.5.0/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_ulid-2.5.0/tests/test_base32.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 python_ulid-2.5.0/tests/test_cli.py
+-rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 python_ulid-2.5.0/tests/test_ulid.py
+-rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 python_ulid-2.5.0/ulid/__init__.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 python_ulid-2.5.0/ulid/__main__.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 python_ulid-2.5.0/ulid/base32.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 python_ulid-2.5.0/ulid/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.5.0/ulid/py.typed
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 python_ulid-2.5.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 python_ulid-2.5.0/LICENSE
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 python_ulid-2.5.0/hatch.toml
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 python_ulid-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 python_ulid-2.5.0/PKG-INFO
```

### Comparing `python_ulid-2.4.0.post0/CHANGELOG.rst` & `python_ulid-2.5.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 .. _changelog:
 
 Changelog
 =========
 
 Versions follow `Semantic Versioning <http://www.semver.org>`_
 
+`2.5.0`_ - 2024-04-26
+---------------------
+
+Changed
+~~~~~~~
+* Generate a more accurate JSON schema with Pydantic's ``BaseModel.model_json_schema()``. This
+  includes a specification for string and byte representations.
+
 `2.4.0`_ - 2024-04-02
 ---------------------
 
 Added
 ~~~~~
 * :class:`.ULID` objects are now properly serialized when used as Pydantic types `@Avihais12344 <https://github.com/Avihais12344>`_.
 
@@ -147,14 +155,15 @@
     >>> ULID().hex
     '0171caa5459a8631a6894d072c8550a8'
 
 * Equality checks and ordering now also work with ``str``-instances.
 * The package now has no external dependencies.
 * The test-coverage has been raised to 100%.
 
+.. _2.5.0: https://github.com/mdomke/python-ulid/compare/2.4.0...2.5.0
 .. _2.4.0: https://github.com/mdomke/python-ulid/compare/2.3.0...2.4.0
 .. _2.3.0: https://github.com/mdomke/python-ulid/compare/2.2.0...2.3.0
 .. _2.2.0: https://github.com/mdomke/python-ulid/compare/2.1.0...2.2.0
 .. _2.1.0: https://github.com/mdomke/python-ulid/compare/2.0.0...2.1.0
 .. _2.0.0: https://github.com/mdomke/python-ulid/compare/1.1.0...2.0.0
 .. _1.1.0: https://github.com/mdomke/python-ulid/compare/1.0.3...1.1.0
 .. _1.0.3: https://github.com/mdomke/python-ulid/compare/1.0.2...1.0.3
```

### Comparing `python_ulid-2.4.0.post0/README.rst` & `python_ulid-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/logo.png` & `python_ulid-2.5.0/logo.png`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/.github/workflows/lint-and-test.yml` & `python_ulid-2.5.0/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/.github/workflows/publish.yml` & `python_ulid-2.5.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/docs/Makefile` & `python_ulid-2.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/docs/source/conf.py` & `python_ulid-2.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/docs/source/index.rst` & `python_ulid-2.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/tests/test_base32.py` & `python_ulid-2.5.0/tests/test_base32.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/tests/test_cli.py` & `python_ulid-2.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/tests/test_ulid.py` & `python_ulid-2.5.0/tests/test_ulid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import time
 import uuid
 from collections.abc import Callable
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
+from typing import Optional
 from typing import Union
 
 import pytest
 from freezegun import freeze_time
 from pydantic import BaseModel
 from pydantic import ValidationError
 
@@ -164,15 +165,15 @@
         constructor(value)
 
 
 def test_pydantic_protocol() -> None:
     ulid = ULID()
 
     class Model(BaseModel):
-        ulid: ULID
+        ulid: Optional[ULID] = None
 
     for value in [ulid, str(ulid), int(ulid), bytes(ulid)]:
         model = Model(ulid=value)
         assert isinstance(model.ulid, ULID)
         assert model.ulid == ulid
 
     for value in [b"not-enough", "not-enough"]:
@@ -184,7 +185,27 @@
     assert ulid_from_dict == ulid
     assert isinstance(ulid_from_dict, ULID)
     assert Model(**model_dict) == model
 
     model_json = model.model_dump_json()
     assert isinstance(json.loads(model_json)["ulid"], str)
     assert Model.model_validate_json(model_json) == model
+
+    model_json_schema = model.model_json_schema()
+    assert "properties" in model_json_schema
+    assert "ulid" in model_json_schema["properties"]
+    assert "anyOf" in model_json_schema["properties"]["ulid"]
+    assert {
+        "maxLength": 26,
+        "minLength": 26,
+        "pattern": "[A-Z0-9]{26}",
+        "type": "string",
+    } in model_json_schema["properties"]["ulid"]["anyOf"]
+    assert {
+        "maxLength": 16,
+        "minLength": 16,
+        "type": "string",
+        "format": "binary",
+    } in model_json_schema["properties"]["ulid"]["anyOf"]
+    assert {
+        "type": "null",
+    } in model_json_schema["properties"]["ulid"]["anyOf"]
```

### Comparing `python_ulid-2.4.0.post0/ulid/__init__.py` & `python_ulid-2.5.0/ulid/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,16 @@
 
         return core_schema.no_info_wrap_validator_function(
             cls._pydantic_validate,
             core_schema.union_schema(
                 [
                     core_schema.is_instance_schema(ULID),
                     core_schema.no_info_plain_validator_function(ULID),
+                    core_schema.str_schema(pattern=r"[A-Z0-9]{26}", min_length=26, max_length=26),
+                    core_schema.bytes_schema(min_length=16, max_length=16),
                 ]
             ),
             serialization=core_schema.to_string_ser_schema(
                 when_used="json-unless-none",
             ),
         )
```

### Comparing `python_ulid-2.4.0.post0/ulid/__main__.py` & `python_ulid-2.5.0/ulid/__main__.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/ulid/base32.py` & `python_ulid-2.5.0/ulid/base32.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/LICENSE` & `python_ulid-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/hatch.toml` & `python_ulid-2.5.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/pyproject.toml` & `python_ulid-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.4.0.post0/PKG-INFO` & `python_ulid-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-ulid
-Version: 2.4.0.post0
+Version: 2.5.0
 Summary: Universally unique lexicographically sortable identifier
 Project-URL: Homepage, https://github.com/mdomke/python-ulid
 Project-URL: Documentation, https://python-ulid.readthedocs.io
 Project-URL: Changelog, https://python-ulid.readthedocs.io/en/latest/changelog.html
 Project-URL: Issues, https://github.com/mdomke/python-ulid/issues
 Project-URL: CI, https://github.com/mdomke/python-ulid/actions
 Project-URL: Repository, https://github.com/mdomke/python-ulid
```

