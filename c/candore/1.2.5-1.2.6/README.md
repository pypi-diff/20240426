# Comparing `tmp/candore-1.2.5.tar.gz` & `tmp/candore-1.2.6.tar.gz`

## Comparing `candore-1.2.5.tar` & `candore-1.2.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.5/apix/__init__.py
--rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 candore-1.2.5/apix/diff.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 candore-1.2.5/apix/explore.py
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 candore-1.2.5/apix/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.5/apix/parsers/__init__.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 candore-1.2.5/apix/parsers/apipie.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 candore-1.2.5/apix/parsers/test.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 candore-1.2.5/candore/__init__.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 candore-1.2.5/candore/cli.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 candore-1.2.5/candore/config.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 candore-1.2.5/candore/errors.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 candore-1.2.5/candore/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/api_lister.py
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/comparator.py
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/extractor.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/finder.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/report.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/variations.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/webapp.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/templates/table.html
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 candore-1.2.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 candore-1.2.5/LICENSE
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 candore-1.2.5/README.md
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 candore-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 candore-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.6/apix/__init__.py
+-rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 candore-1.2.6/apix/diff.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 candore-1.2.6/apix/explore.py
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 candore-1.2.6/apix/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.6/apix/parsers/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 candore-1.2.6/apix/parsers/apipie.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 candore-1.2.6/apix/parsers/test.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 candore-1.2.6/candore/__init__.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 candore-1.2.6/candore/cli.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 candore-1.2.6/candore/config.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 candore-1.2.6/candore/errors.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 candore-1.2.6/candore/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.6/candore/modules/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 candore-1.2.6/candore/modules/api_lister.py
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 candore-1.2.6/candore/modules/comparator.py
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 candore-1.2.6/candore/modules/extractor.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 candore-1.2.6/candore/modules/finder.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 candore-1.2.6/candore/modules/report.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 candore-1.2.6/candore/modules/variations.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 candore-1.2.6/candore/modules/webapp.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 candore-1.2.6/candore/modules/templates/table.html
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 candore-1.2.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 candore-1.2.6/LICENSE
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 candore-1.2.6/README.md
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 candore-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 candore-1.2.6/PKG-INFO
```

### Comparing `candore-1.2.5/apix/diff.py` & `candore-1.2.6/apix/diff.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/apix/explore.py` & `candore-1.2.6/apix/explore.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/apix/helpers.py` & `candore-1.2.6/apix/helpers.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/apix/parsers/apipie.py` & `candore-1.2.6/apix/parsers/apipie.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/apix/parsers/test.py` & `candore-1.2.6/apix/parsers/test.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/candore/__init__.py` & `candore-1.2.6/candore/__init__.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/candore/cli.py` & `candore-1.2.6/candore/cli.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/candore/config.py` & `candore-1.2.6/candore/config.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/candore/utils.py` & `candore-1.2.6/candore/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 
 def is_list_contains_dict(_list):
     contains_dict = any(isinstance(element, dict) for element in _list)
     return contains_dict
 
 
 def yaml_reader(file_path=None):
+    if not file_path:
+        return None
     templates_path = Path(file_path)
     if not templates_path.exists():
-        print(f"The file {templates_path} does not exist.")
+        print(f"Warning! The file {templates_path} does not exist.")
+        return None
     with templates_path.open() as yaml_file:
         yaml_data = yaml.safe_load(yaml_file)
     return yaml_data
 
 
 def get_yaml_paths(yaml_data, prefix="", separator="/"):
     paths = []
-    if isinstance(yaml_data, dict):
-        for key, value in yaml_data.items():
-            paths.extend(get_yaml_paths(value, f"{prefix}{key}{separator}"))
-    elif isinstance(yaml_data, list):
-        for item in yaml_data:
-            paths.extend(get_yaml_paths(item, prefix, separator))
-    else:
-        paths.append(f"{prefix}{yaml_data}")
+    if yaml_data:
+        if isinstance(yaml_data, dict):
+            for key, value in yaml_data.items():
+                paths.extend(get_yaml_paths(value, f"{prefix}{key}{separator}"))
+        elif isinstance(yaml_data, list):
+            for item in yaml_data:
+                paths.extend(get_yaml_paths(item, prefix, separator))
+        else:
+            paths.append(f"{prefix}{yaml_data}")
     return paths
```

### Comparing `candore-1.2.5/candore/modules/api_lister.py` & `candore-1.2.6/candore/modules/api_lister.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/candore/modules/comparator.py` & `candore-1.2.6/candore/modules/comparator.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,20 +8,14 @@
     def __init__(self, settings):
         self.big_key = []
         self.big_diff = {}
         self.big_constant = {}
         self.record_evs = False
         self.variations = Variations(settings)
         self.constants = Constants(settings)
-        self.expected_variations = self.variations.expected_variations
-        self.skipped_variations = self.variations.skipped_variations
-        self.expected_constants = self.constants.expected_constants
-        self.skipped_constants = self.constants.skipped_constants
-
-
 
     def remove_verifed_key(self, key):
         reversed_bk = self.big_key[::-1]
         if key in reversed_bk:
             reversed_bk.remove(key)
         self.big_key = reversed_bk[::-1]
 
@@ -31,44 +25,44 @@
             return
         self.big_key = self.big_key[:id_index]
 
     def record_variation(self, pre, post, var_details=None):
         big_key = [str(itm) for itm in self.big_key]
         full_path = "/".join(big_key)
         var_full_path = "/".join([itm for itm in self.big_key if not isinstance(itm, int)])
-        if var_full_path in self.expected_variations or var_full_path in self.skipped_variations:
+        if var_full_path in self.variations.expected_variations or var_full_path in self.variations.skipped_variations:
             if self.record_evs:
                 variation = {
                     "pre": pre,
                     "post": post,
                     "variation": var_details or "Expected(A)",
                 }
                 self.big_diff.update({full_path: variation})
         elif (
-            var_full_path not in self.expected_variations
-            and var_full_path not in self.skipped_variations
+            var_full_path not in self.variations.expected_variations
+            and var_full_path not in self.variations.skipped_variations
         ):
             variation = {"pre": pre, "post": post, "variation": var_details or ""}
             self.big_diff.update({full_path: variation})
 
     def record_constants(self, pre, post, var_details=None):
         big_key = [str(itm) for itm in self.big_key]
         full_path = "/".join(big_key)
         var_full_path = "/".join([itm for itm in self.big_key if not isinstance(itm, int)])
-        if var_full_path in self.expected_constants or var_full_path in self.skipped_constants:
+        if var_full_path in self.constants.expected_constants or var_full_path in self.constants.skipped_constants:
             if self.record_evs:
                 variation = {
                     "pre": pre,
                     "post": post,
                     "constant": var_details or "Expected(A)",
                 }
                 self.big_constant.update({full_path: variation})
         elif (
-            var_full_path not in self.expected_constants
-            and var_full_path not in self.skipped_constants
+            var_full_path not in self.constants.expected_constants
+            and var_full_path not in self.constants.skipped_constants
         ):
             variation = {"pre": pre, "post": post, "constant": var_details or ""}
             self.big_constant.update({full_path: variation})
 
     def _is_data_type_dict(self, pre, post, unique_key=""):
         if (pre and 'id' in pre) and (post and 'id' in post):
             # Dont compare the entities if the ids are not the same
```

### Comparing `candore-1.2.5/candore/modules/extractor.py` & `candore-1.2.6/candore/modules/extractor.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/candore/modules/finder.py` & `candore-1.2.6/candore/modules/finder.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/candore/modules/report.py` & `candore-1.2.6/candore/modules/report.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/candore/modules/variations.py` & `candore-1.2.6/candore/modules/variations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 """
 A module responsible for calculating expected and skipped variations from
 `conf/variations` yaml file and convert them into processable list
 """
 from functools import cached_property
 from candore.utils import yaml_reader, get_yaml_paths
 
-import yaml
-
 
 class Variations:
     def __init__(self, settings):
         self.settings = settings
 
     @cached_property
     def variations(self):
-        yaml_data = yaml_reader(file_path=self.settings.candore.var_file)
+        yaml_data = yaml_reader(file_path=getattr(self.settings.candore, "var_file", None))
         return yaml_data
 
     @cached_property
     def expected_variations(self):
-        return get_yaml_paths(yaml_data=self.variations.get("expected_variations"))
+        yaml_data = self.variations.get("expected_variations") if self.variations else None
+        return get_yaml_paths(yaml_data=yaml_data)
+
 
     @cached_property
     def skipped_variations(self):
-        return get_yaml_paths(yaml_data=self.variations.get("skipped_variations"))
+        yaml_data = self.variations.get("skipped_variations") if self.variations else None
+        return get_yaml_paths(yaml_data=yaml_data)
 
 
 class Constants:
     def __init__(self, settings):
         self.settings = settings
 
     @cached_property
     def constants(self):
-        yaml_data = yaml_reader(file_path=self.settings.candore.constant_file)
+        yaml_data = yaml_reader(file_path=getattr(self.settings.candore, "constant_file", None))
         return yaml_data
 
     @cached_property
     def expected_constants(self):
-        return get_yaml_paths(yaml_data=self.constants.get("expected_constants"))
+        yaml_data = self.constants.get("expected_constants") if self.constants else None
+        return get_yaml_paths(yaml_data=yaml_data)
 
     @cached_property
     def skipped_constants(self):
-        return get_yaml_paths(yaml_data=self.constants.get("skipped_constants"))
+        yaml_data = self.constants.get("skipped_constants") if self.constants else None
+        return get_yaml_paths(yaml_data=yaml_data)
```

### Comparing `candore-1.2.5/candore/modules/templates/table.html` & `candore-1.2.6/candore/modules/templates/table.html`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/LICENSE` & `candore-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/README.md` & `candore-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/pyproject.toml` & `candore-1.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `candore-1.2.5/PKG-INFO` & `candore-1.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: candore
-Version: 1.2.5
+Version: 1.2.6
 Author: Jitendra Yejare
 Maintainer: Jitendra Yejare
 License-File: LICENSE
 Keywords: api,data,distutils,hatch,upgrades,validation
 Requires-Dist: aiohttp
 Requires-Dist: asyncio
 Requires-Dist: click
```

