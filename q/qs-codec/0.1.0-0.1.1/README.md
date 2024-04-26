# Comparing `tmp/qs_codec-0.1.0.tar.gz` & `tmp/qs_codec-0.1.1.tar.gz`

## Comparing `qs_codec-0.1.0.tar` & `qs_codec-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 qs_codec-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.1.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qs_codec-0.1.0/requirements_dev.txt
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/__init__.py
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/decode.py
--rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/encode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/enums/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/enums/charset.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/enums/duplicates.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/enums/format.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/enums/list_format.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/enums/sentinel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/models/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/models/decode_options.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/models/encode_options.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/models/undefined.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/models/weak_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/utils/__init__.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/utils/decode_utils.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/utils/encode_utils.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/utils/str_utils.py
--rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 qs_codec-0.1.0/src/qs_codec/utils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.0/tests/e2e/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 qs_codec-0.1.0/tests/e2e/e2e_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.0/tests/unit/__init__.py
--rw-r--r--   0        0        0    29989 2020-02-02 00:00:00.000000 qs_codec-0.1.0/tests/unit/decode_test.py
--rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 qs_codec-0.1.0/tests/unit/encode_test.py
--rw-r--r--   0        0        0    21897 2020-02-02 00:00:00.000000 qs_codec-0.1.0/tests/unit/example_test.py
--rw-r--r--   0        0        0    14896 2020-02-02 00:00:00.000000 qs_codec-0.1.0/tests/unit/utils_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.1.0/tests/unit/weakref_test.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.1.0/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.1.0/LICENSE
--rw-r--r--   0        0        0    24399 2020-02-02 00:00:00.000000 qs_codec-0.1.0/README.md
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 qs_codec-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    25804 2020-02-02 00:00:00.000000 qs_codec-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 qs_codec-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.1.1/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qs_codec-0.1.1/requirements_dev.txt
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/__init__.py
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/decode.py
+-rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/encode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/enums/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/enums/charset.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/enums/duplicates.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/enums/format.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/enums/list_format.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/enums/sentinel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/models/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/models/decode_options.py
+-rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/models/encode_options.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/models/undefined.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/models/weak_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/utils/__init__.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/utils/decode_utils.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/utils/encode_utils.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/utils/str_utils.py
+-rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 qs_codec-0.1.1/src/qs_codec/utils/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.1/tests/e2e/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 qs_codec-0.1.1/tests/e2e/e2e_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0    29989 2020-02-02 00:00:00.000000 qs_codec-0.1.1/tests/unit/decode_test.py
+-rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 qs_codec-0.1.1/tests/unit/encode_test.py
+-rw-r--r--   0        0        0    21897 2020-02-02 00:00:00.000000 qs_codec-0.1.1/tests/unit/example_test.py
+-rw-r--r--   0        0        0    14896 2020-02-02 00:00:00.000000 qs_codec-0.1.1/tests/unit/utils_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.1.1/tests/unit/weakref_test.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.1.1/LICENSE
+-rw-r--r--   0        0        0    24736 2020-02-02 00:00:00.000000 qs_codec-0.1.1/README.md
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 qs_codec-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    26141 2020-02-02 00:00:00.000000 qs_codec-0.1.1/PKG-INFO
```

### Comparing `qs_codec-0.1.0/CODE-OF-CONDUCT.md` & `qs_codec-0.1.1/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/decode.py` & `qs_codec-0.1.1/src/qs_codec/decode.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/encode.py` & `qs_codec-0.1.1/src/qs_codec/encode.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/enums/format.py` & `qs_codec-0.1.1/src/qs_codec/enums/format.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/enums/list_format.py` & `qs_codec-0.1.1/src/qs_codec/enums/list_format.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/enums/sentinel.py` & `qs_codec-0.1.1/src/qs_codec/enums/sentinel.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/models/decode_options.py` & `qs_codec-0.1.1/src/qs_codec/models/decode_options.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/models/encode_options.py` & `qs_codec-0.1.1/src/qs_codec/models/encode_options.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/models/weak_wrapper.py` & `qs_codec-0.1.1/src/qs_codec/models/weak_wrapper.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/utils/decode_utils.py` & `qs_codec-0.1.1/src/qs_codec/utils/decode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/utils/encode_utils.py` & `qs_codec-0.1.1/src/qs_codec/utils/encode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/utils/str_utils.py` & `qs_codec-0.1.1/src/qs_codec/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/src/qs_codec/utils/utils.py` & `qs_codec-0.1.1/src/qs_codec/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/tests/e2e/e2e_test.py` & `qs_codec-0.1.1/tests/e2e/e2e_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/tests/unit/decode_test.py` & `qs_codec-0.1.1/tests/unit/decode_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/tests/unit/encode_test.py` & `qs_codec-0.1.1/tests/unit/encode_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/tests/unit/example_test.py` & `qs_codec-0.1.1/tests/unit/example_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/tests/unit/utils_test.py` & `qs_codec-0.1.1/tests/unit/utils_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/tests/unit/weakref_test.py` & `qs_codec-0.1.1/tests/unit/weakref_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/.gitignore` & `qs_codec-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/LICENSE` & `qs_codec-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/README.md` & `qs_codec-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,51 @@
+Metadata-Version: 2.3
+Name: qs-codec
+Version: 0.1.1
+Summary: A query string encoding and decoding library for Python. Ported from qs for JavaScript.
+Project-URL: Source, https://github.com/techouse/qs_codec
+Project-URL: Changelog, https://github.com/techouse/qs_codec/blob/master/CHANGELOG.md
+Project-URL: Sponsor, https://github.com/sponsors/techouse
+Project-URL: PayPal, https://paypal.me/ktusar
+Author-email: Klemen Tusar <techouse@gmail.com>
+License: BSD-3-Clause
+License-File: LICENSE
+Keywords: codec,qs,query,query-string,querystring,url
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 from typing import Listfrom re import Matchfrom typing import List
 
 # qs_codec
 
 A query string encoding and decoding library for Python.
 
 Ported from [qs](https://www.npmjs.com/package/qs) for JavaScript.
 
+![PyPI - Version](https://img.shields.io/pypi/v/qs_codec)
+![PyPI - Status](https://img.shields.io/pypi/status/qs_codec)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qs_codec)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/qs_codec)
+![PyPI - Format](https://img.shields.io/pypi/format/qs_codec)
 [![Test](https://github.com/techouse/qs_codec/actions/workflows/test.yml/badge.svg)](https://github.com/techouse/qs_codec/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/techouse/qs_codec/graph/badge.svg?token=Vp0z05yj2l)](https://codecov.io/gh/techouse/qs_codec)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/7ead208221ae4f6785631043064647e4)](https://app.codacy.com/gh/techouse/qs_codec/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![GitHub](https://img.shields.io/github/license/techouse/qs_codec)](LICENSE)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/techouse)](https://github.com/sponsors/techouse)
 [![GitHub Repo stars](https://img.shields.io/github/stars/techouse/qs_codec)](https://github.com/techouse/qs_codec/stargazers)
 
@@ -30,18 +66,20 @@
 ### Decoding dictionaries
 
 ```python
 import qs_codec, typing as t
 
 
 def decode(
-        value: t.Optional[t.Union[str, t.Mapping]],
-        options: qs_codec.DecodeOptions = qs_codec.DecodeOptions(),
+    value: t.Optional[t.Union[str, t.Mapping]],
+    options: qs_codec.DecodeOptions = qs_codec.DecodeOptions(),
 ) -> dict:
-    """Decodes a str or Mapping into a Dict. Providing custom DecodeOptions will override the default behavior."""
+    """Decodes a str or Mapping into a Dict. 
+    
+    Providing custom DecodeOptions will override the default behavior."""
     pass
 ```
 
 **qs** allows you to create nested `dict`s within your query strings, by surrounding the name of sub-keys with 
 square brackets `[]`. For example, the string `'foo[bar]=baz'` converts to:
 
 ```python
@@ -354,18 +392,20 @@
 ### Encoding
 
 ```python
 import qs_codec, typing as t
 
 
 def encode(
-        value: t.Any,
-        options: qs_codec.EncodeOptions = qs_codec.EncodeOptions()
+    value: t.Any,
+    options: qs_codec.EncodeOptions = qs_codec.EncodeOptions()
 ) -> str:
-    """Encodes an object into a query string. Providing custom EncodeOptions will override the default behavior."""
+    """Encodes an object into a query string.
+    
+    Providing custom EncodeOptions will override the default behavior."""
     pass
 ```
 
 When encoding, **qs** by default URI encodes output. `dict`s are encoded as you would expect:
 
 ```python
 import qs_codec
```

### Comparing `qs_codec-0.1.0/pyproject.toml` & `qs_codec-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.0/PKG-INFO` & `qs_codec-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,20 @@
-Metadata-Version: 2.3
-Name: qs-codec
-Version: 0.1.0
-Summary: A query string encoding and decoding library for Python. Ported from qs for JavaScript.
-Project-URL: Source, https://github.com/techouse/qs_codec
-Project-URL: Changelog, https://github.com/techouse/qs_codec/blob/master/CHANGELOG.md
-Project-URL: Sponsor, https://github.com/sponsors/techouse
-Project-URL: PayPal, https://paypal.me/ktusar
-Author-email: Klemen Tusar <techouse@gmail.com>
-License: BSD-3-Clause
-License-File: LICENSE
-Keywords: codec,qs,query,query-string,querystring,url
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 from typing import Listfrom re import Matchfrom typing import List
 
 # qs_codec
 
 A query string encoding and decoding library for Python.
 
 Ported from [qs](https://www.npmjs.com/package/qs) for JavaScript.
 
+![PyPI - Version](https://img.shields.io/pypi/v/qs_codec)
+![PyPI - Status](https://img.shields.io/pypi/status/qs_codec)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qs_codec)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/qs_codec)
+![PyPI - Format](https://img.shields.io/pypi/format/qs_codec)
 [![Test](https://github.com/techouse/qs_codec/actions/workflows/test.yml/badge.svg)](https://github.com/techouse/qs_codec/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/techouse/qs_codec/graph/badge.svg?token=Vp0z05yj2l)](https://codecov.io/gh/techouse/qs_codec)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/7ead208221ae4f6785631043064647e4)](https://app.codacy.com/gh/techouse/qs_codec/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![GitHub](https://img.shields.io/github/license/techouse/qs_codec)](LICENSE)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/techouse)](https://github.com/sponsors/techouse)
 [![GitHub Repo stars](https://img.shields.io/github/stars/techouse/qs_codec)](https://github.com/techouse/qs_codec/stargazers)
 
@@ -61,18 +35,20 @@
 ### Decoding dictionaries
 
 ```python
 import qs_codec, typing as t
 
 
 def decode(
-        value: t.Optional[t.Union[str, t.Mapping]],
-        options: qs_codec.DecodeOptions = qs_codec.DecodeOptions(),
+    value: t.Optional[t.Union[str, t.Mapping]],
+    options: qs_codec.DecodeOptions = qs_codec.DecodeOptions(),
 ) -> dict:
-    """Decodes a str or Mapping into a Dict. Providing custom DecodeOptions will override the default behavior."""
+    """Decodes a str or Mapping into a Dict. 
+    
+    Providing custom DecodeOptions will override the default behavior."""
     pass
 ```
 
 **qs** allows you to create nested `dict`s within your query strings, by surrounding the name of sub-keys with 
 square brackets `[]`. For example, the string `'foo[bar]=baz'` converts to:
 
 ```python
@@ -385,18 +361,20 @@
 ### Encoding
 
 ```python
 import qs_codec, typing as t
 
 
 def encode(
-        value: t.Any,
-        options: qs_codec.EncodeOptions = qs_codec.EncodeOptions()
+    value: t.Any,
+    options: qs_codec.EncodeOptions = qs_codec.EncodeOptions()
 ) -> str:
-    """Encodes an object into a query string. Providing custom EncodeOptions will override the default behavior."""
+    """Encodes an object into a query string.
+    
+    Providing custom EncodeOptions will override the default behavior."""
     pass
 ```
 
 When encoding, **qs** by default URI encodes output. `dict`s are encoded as you would expect:
 
 ```python
 import qs_codec
```

