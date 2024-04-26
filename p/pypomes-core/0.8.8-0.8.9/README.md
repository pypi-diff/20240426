# Comparing `tmp/pypomes_core-0.8.8.tar.gz` & `tmp/pypomes_core-0.8.9.tar.gz`

## Comparing `pypomes_core-0.8.8.tar` & `pypomes_core-0.8.9.tar`

### file list

```diff
@@ -1,20 +1,45 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    23887 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/make.bat
+-rw-r--r--   0        0        0    18730 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/index.html
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/search.html
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/source/conf.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/docs/source/index.rst
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    23887 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.9/PKG-INFO
```

### Comparing `pypomes_core-0.8.8/src/pypomes_core/.ruff.toml` & `pypomes_core-0.8.9/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/__init__.py` & `pypomes_core-0.8.9/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/dict_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -663,15 +663,16 @@
 
     This insertion will happen only if such a value is not itself a list.
     All lists eventually found, up to the penultimate key in the chain, will be processed recursively.
 
     :param target: the dictionary to be modified
     :param key_chain: the chain of nested keys pointing to the item in question
     """
-    def items_listify(in_targets: list, in_keys: list[str]) -> None:
+    def items_listify(in_targets: list,
+                      in_keys: list[str]) -> None:
 
         # traverse the list
         for in_target in in_targets:
             # is the element a dictionary ?
             if isinstance(in_target, dict):
                 # yes, process it
                 dict_listify(in_target, in_keys)
```

### Comparing `pypomes_core-0.8.8/src/pypomes_core/email_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/env_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/file_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/json_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/list_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/str_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.8.9/src/pypomes_core/validation_msgs.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,22 @@
         "en": "Attribute not applicable for {}",
         "pt": "Atributo não se aplica a {}",
     },
     114: {
         "en": "Attribute applicable only for {}",
         "pt": "Atributo se aplica apenas a {}",
     },
+    115: {
+        "en": "A value has not yet been assigned",
+        "pt": "Valor ainda não foi atribuído",
+    },
+    116: {
+        "en": "Value {} cannot be assigned for attributes {} at the same time",
+        "pt": "Valor {} não pode ser atribuído aos atributos {} ao mesmo tempo",
+    },
     121: {
         "en": "Invalid value {}",
         "pt": "Valor {} inválido",
     },
     122: {
         "en": "Invalid value {}: length shorter than {}",
         "pt": "Valor {} inválido: comprimento menor que {}",
```

### Comparing `pypomes_core-0.8.8/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.8.9/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/LICENSE` & `pypomes_core-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.8/pyproject.toml` & `pypomes_core-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.8.8"
+version = "0.8.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.8.8/PKG-INFO` & `pypomes_core-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.8.8
+Version: 0.8.9
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

