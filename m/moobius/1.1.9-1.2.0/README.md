# Comparing `tmp/moobius-1.1.9.tar.gz` & `tmp/moobius-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moobius-1.1.9.tar", last modified: Mon Apr 22 05:00:33 2024, max compression
+gzip compressed data, was "moobius-1.2.0.tar", last modified: Fri Apr 26 06:14:47 2024, max compression
```

## Comparing `moobius-1.1.9.tar` & `moobius-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.307537 moobius-1.1.9/
--rw-rw-rw-   0        0        0     8910 2024-04-22 05:00:33.307537 moobius-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.1.9/license.md
--rw-rw-rw-   0        0        0      647 2024-04-22 02:34:33.000000 moobius-1.1.9/pyproject.toml
--rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.1.9/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-22 05:00:33.307537 moobius-1.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.287603 moobius-1.1.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.289596 moobius-1.1.9/src/moobius/
--rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.1.9/src/moobius/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.297570 moobius-1.1.9/src/moobius/core/
--rw-rw-rw-   0        0        0    57654 2024-04-22 00:12:14.000000 moobius-1.1.9/src/moobius/core/sdk.py
--rw-rw-rw-   0        0        0     4170 2024-04-01 21:02:47.000000 moobius-1.1.9/src/moobius/core/wand.py
-drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.302554 moobius-1.1.9/src/moobius/database/
--rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.1.9/src/moobius/database/database_interface.py
--rw-rw-rw-   0        0        0     4098 2024-04-16 23:52:13.000000 moobius-1.1.9/src/moobius/database/json_database.py
--rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.1.9/src/moobius/database/null_database.py
--rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.1.9/src/moobius/database/redis_database.py
--rw-rw-rw-   0        0        0     9559 2024-03-26 23:06:54.000000 moobius-1.1.9/src/moobius/database/storage.py
-drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.305543 moobius-1.1.9/src/moobius/network/
--rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.1.9/src/moobius/network/asserts.py
--rw-rw-rw-   0        0        0    45076 2024-04-22 00:04:45.000000 moobius-1.1.9/src/moobius/network/http_api_wrapper.py
--rw-rw-rw-   0        0        0    25652 2024-04-10 03:05:43.000000 moobius-1.1.9/src/moobius/network/ws_client.py
--rw-rw-rw-   0        0        0     7154 2024-04-08 21:51:19.000000 moobius-1.1.9/src/moobius/types.py
--rw-rw-rw-   0        0        0     7399 2024-03-29 15:46:12.000000 moobius-1.1.9/src/moobius/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.306539 moobius-1.1.9/src/moobius.egg-info/
--rw-rw-rw-   0        0        0     8910 2024-04-22 05:00:33.000000 moobius-1.1.9/src/moobius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2024-04-22 05:00:33.000000 moobius-1.1.9/src/moobius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 05:00:33.000000 moobius-1.1.9/src/moobius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-04-22 05:00:33.000000 moobius-1.1.9/src/moobius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-22 05:00:33.000000 moobius-1.1.9/src/moobius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.1.9/src/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.241967 moobius-1.2.0/
+-rw-rw-rw-   0        0        0     8910 2024-04-26 06:14:47.240970 moobius-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.2.0/license.md
+-rw-rw-rw-   0        0        0      647 2024-04-26 06:06:56.000000 moobius-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.2.0/readme.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 06:14:47.241967 moobius-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.220204 moobius-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.223898 moobius-1.2.0/src/moobius/
+-rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.2.0/src/moobius/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.231846 moobius-1.2.0/src/moobius/core/
+-rw-rw-rw-   0        0        0    57654 2024-04-24 21:24:30.000000 moobius-1.2.0/src/moobius/core/sdk.py
+-rw-rw-rw-   0        0        0     4170 2024-04-01 21:02:47.000000 moobius-1.2.0/src/moobius/core/wand.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.235837 moobius-1.2.0/src/moobius/database/
+-rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.2.0/src/moobius/database/database_interface.py
+-rw-rw-rw-   0        0        0     4435 2024-04-26 04:20:23.000000 moobius-1.2.0/src/moobius/database/json_database.py
+-rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.2.0/src/moobius/database/null_database.py
+-rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.2.0/src/moobius/database/redis_database.py
+-rw-rw-rw-   0        0        0     9708 2024-04-26 05:53:24.000000 moobius-1.2.0/src/moobius/database/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.238977 moobius-1.2.0/src/moobius/network/
+-rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.2.0/src/moobius/network/asserts.py
+-rw-rw-rw-   0        0        0    45076 2024-04-24 18:33:19.000000 moobius-1.2.0/src/moobius/network/http_api_wrapper.py
+-rw-rw-rw-   0        0        0    25652 2024-04-10 03:05:43.000000 moobius-1.2.0/src/moobius/network/ws_client.py
+-rw-rw-rw-   0        0        0     7154 2024-04-08 21:51:19.000000 moobius-1.2.0/src/moobius/types.py
+-rw-rw-rw-   0        0        0     7399 2024-04-23 19:30:39.000000 moobius-1.2.0/src/moobius/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.239979 moobius-1.2.0/src/moobius.egg-info/
+-rw-rw-rw-   0        0        0     8910 2024-04-26 06:14:47.000000 moobius-1.2.0/src/moobius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2024-04-26 06:14:47.000000 moobius-1.2.0/src/moobius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 06:14:47.000000 moobius-1.2.0/src/moobius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-04-26 06:14:47.000000 moobius-1.2.0/src/moobius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-26 06:14:47.000000 moobius-1.2.0/src/moobius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.2.0/src/setup.py
```

### Comparing `moobius-1.1.9/PKG-INFO` & `moobius-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.1.9
+Version: 1.2.0
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.1.9/license.md` & `moobius-1.2.0/license.md`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/pyproject.toml` & `moobius-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "moobius"
-version = "1.1.9"
+version = "1.2.0"
 authors = [
   { name="Kevin Kostlan", email="sdk@moobius.app"},
 ]
 description = "Moobius Platform SDK"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `moobius-1.1.9/readme.md` & `moobius-1.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius/core/sdk.py` & `moobius-1.2.0/src/moobius/core/sdk.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius/core/wand.py` & `moobius-1.2.0/src/moobius/core/wand.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius/database/database_interface.py` & `moobius-1.2.0/src/moobius/database/database_interface.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius/database/json_database.py` & `moobius-1.2.0/src/moobius/database/json_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # json_database.py
 
-import json
+import json, dataclasses
 import os
 from pydoc import locate
 
 from dacite import from_dict
 from loguru import logger
 
 from moobius.utils import EnhancedJSONEncoder
 from moobius import types
 from .database_interface import DatabaseInterface
 
+DTYPE = '_type' # Used to indicate the class name.
 
 # TODO: 
 # 1. validity check for key (must be str)
 # 2. json serializable check
 # 3. rolling back when error occurs
 class JSONDatabase(DatabaseInterface):
     # key: name of the database json file
@@ -38,15 +39,14 @@
           Note: This should not be called directly. Users should config the database in the config file, and call MoobiusStorage to initialize the database.
           >>> database = JSONDatabase(domain='service_1.channel_1', root_dir='data')
         """
 
         super().__init__()
 
         self.path = os.path.join(root_dir, domain.replace('.', os.sep))
-        self.ref_module = types
         os.makedirs(self.path, exist_ok=True)
 
     def get_value(self, key):
         """
         Gets the value (which is a dict) of a string-valued key. Returns (is_success, the_value).
         Note: This function should not be called directly.
 
@@ -56,39 +56,40 @@
         filename = os.path.join(self.path, key + '.json')
 
         if not os.path.exists(filename):
             return False, f'No json file found for {key}.'
         with open(filename, 'r', encoding='utf-8') as f:
             data = json.load(f)
 
-            if data['_type'] == 'NoneType':
+            if data[DTYPE] == 'NoneType':
                 return True, None   # You can't use NoneType(None) to construct a NoneType object, so we have to return None directly
             else:
-                class_name = data['_type']
-                data_type = locate(f'{self.ref_module.__name__}.{class_name}')
-
-                if data_type:   # dataclass
-                    return True, from_dict(data_class=data_type, data=data[key])
-
-                else:   # possible built-in type, attempt to construct the object from the value
-                    data_type = locate(class_name)
+                class_name_fullpath = data[DTYPE]
+                data_type = locate(class_name_fullpath)
 
+                if not data_type: # Legacy backwards compat. Remove this if block after enough time has passed.
+                    data_type = locate(f'{types.__name__}.{class_name_fullpath}')
                     if data_type:
-                        return True, data_type(data[key])
+                        logger.warning('Legacy compat JSONDatabase type system. This warning should disappear on save+load of the database.')
 
+                if data_type:
+                    if dataclasses.is_dataclass(data_type):
+                        return True, from_dict(data_class=data_type, data=data[key])
                     else:
-                        raise TypeError(f'Unknown type: {class_name}')
+                        return True, data_type(data[key])
+                else:
+                    raise TypeError(f'Unknown type: {class_name_fullpath}')
 
     def set_value(self, key, value):
         """Set the value (a dict) of a key (a string). Returns (is_success, the_key).
            Note: This function should not be called directly."""
         filename = os.path.join(self.path, key + '.json')
 
         with open(filename, 'w', encoding='utf-8') as f:
-            data = {key: value, '_type': type(value).__name__}
+            data = {key: value, DTYPE: type(value).__module__+'.'+type(value).__name__} # Fullpath is package.module.name.
             json.dump(data, f, indent=4, cls=EnhancedJSONEncoder, ensure_ascii=False)
             return True, key
 
     def delete_key(self, key):
         """Delete a (string-valued) key. Returns (is_success, key)
            Note: This function should not be called directly."""
         filename = os.path.join(self.path, key + '.json')
```

### Comparing `moobius-1.1.9/src/moobius/database/null_database.py` & `moobius-1.2.0/src/moobius/database/null_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius/database/redis_database.py` & `moobius-1.2.0/src/moobius/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius/database/storage.py` & `moobius-1.2.0/src/moobius/database/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,19 @@
         if dict.__contains__(self, key):
             out = self.__getitem__(key)
             self.__delitem__(key)
             return out
         else:
             return default
 
+    def clear(self):
+        """Clears everything in both this file and on the disk."""
+        for k in list(self.keys()):
+            self.pop(k)
+
     def __str__(self):
         kys = list(self.keys())
         vs = [self.get(k) for k in kys]
         return f'moobius.CachedDict({dict(zip(kys, vs))})'
     def __repr__(self):
         return self.__str__()
```

### Comparing `moobius-1.1.9/src/moobius/network/asserts.py` & `moobius-1.2.0/src/moobius/network/asserts.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius/network/http_api_wrapper.py` & `moobius-1.2.0/src/moobius/network/http_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius/network/ws_client.py` & `moobius-1.2.0/src/moobius/network/ws_client.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius/types.py` & `moobius-1.2.0/src/moobius/types.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius/utils.py` & `moobius-1.2.0/src/moobius/utils.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.9/src/moobius.egg-info/PKG-INFO` & `moobius-1.2.0/src/moobius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.1.9
+Version: 1.2.0
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.1.9/src/moobius.egg-info/SOURCES.txt` & `moobius-1.2.0/src/moobius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

