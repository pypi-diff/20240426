# Comparing `tmp/cabinet-2024.4.15.2.tar.gz` & `tmp/cabinet-2024.4.25.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2024.4.15.2.tar", last modified: Tue Apr 16 03:17:40 2024, max compression
+gzip compressed data, was "cabinet-2024.4.25.1.tar", last modified: Fri Apr 26 06:21:58 2024, max compression
```

## Comparing `cabinet-2024.4.15.2.tar` & `cabinet-2024.4.25.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:17:40.814808 cabinet-2024.4.15.2/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.15.2/LICENSE
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-16 03:17:40.814808 cabinet-2024.4.15.2/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:14:18.000000 cabinet-2024.4.15.2/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.15.2/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-16 03:17:40.814808 cabinet-2024.4.15.2/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:17:40.810808 cabinet-2024.4.15.2/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:17:40.814808 cabinet-2024.4.15.2/src/cabinet/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.15.2/src/cabinet/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.15.2/src/cabinet/__main__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    37122 2024-04-16 00:09:36.000000 cabinet-2024.4.15.2/src/cabinet/cabinet.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.15.2/src/cabinet/constants.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     4894 2024-04-16 03:15:43.000000 cabinet-2024.4.15.2/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:17:40.814808 cabinet-2024.4.15.2/src/cabinet.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-16 03:17:40.000000 cabinet-2024.4.15.2/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      358 2024-04-16 03:17:40.000000 cabinet-2024.4.15.2/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-16 03:17:40.000000 cabinet-2024.4.15.2/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-16 03:17:40.000000 cabinet-2024.4.15.2/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-16 03:17:40.000000 cabinet-2024.4.15.2/src/cabinet.egg-info/top_level.txt
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:17:40.814808 cabinet-2024.4.15.2/test/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1730 2024-01-29 08:09:41.000000 cabinet-2024.4.15.2/test/test___init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-26 06:21:58.675914 cabinet-2024.4.25.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.25.1/LICENSE
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-26 06:21:58.675914 cabinet-2024.4.25.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.4.25.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.25.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-26 06:21:58.675914 cabinet-2024.4.25.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-26 06:21:58.671914 cabinet-2024.4.25.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-26 06:21:58.675914 cabinet-2024.4.25.1/src/cabinet/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.25.1/src/cabinet/__init__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.25.1/src/cabinet/__main__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)    37937 2024-04-26 06:03:05.000000 cabinet-2024.4.25.1/src/cabinet/cabinet.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.25.1/src/cabinet/constants.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-26 04:02:59.000000 cabinet-2024.4.25.1/src/cabinet/helpers.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     4894 2024-04-16 03:19:05.000000 cabinet-2024.4.25.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-26 06:21:58.675914 cabinet-2024.4.25.1/src/cabinet.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-26 06:21:58.000000 cabinet-2024.4.25.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-04-26 06:21:58.000000 cabinet-2024.4.25.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-26 06:21:58.000000 cabinet-2024.4.25.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-26 06:21:58.000000 cabinet-2024.4.25.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-26 06:21:58.000000 cabinet-2024.4.25.1/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2024.4.15.2/LICENSE` & `cabinet-2024.4.25.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.15.2/PKG-INFO` & `cabinet-2024.4.25.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.15.2
+Version: 2024.4.25.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2024.4.15.2/README.md` & `cabinet-2024.4.25.1/README.md`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.15.2/setup.cfg` & `cabinet-2024.4.25.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2024.04.15.2
+version = 2024.04.25.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2024.4.15.2/src/cabinet/cabinet.py` & `cabinet-2024.4.25.1/src/cabinet/cabinet.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 import time
 import logging
 import getpass
 import pathlib
 import argparse
 import subprocess
 import importlib.metadata
-from typing import Optional
 from datetime import date, datetime
+from typing import Any, Type, Optional, TypeVar
 import pymongo.errors
 from pymongo.mongo_client import MongoClient
 from pymongo.server_api import ServerApi
 from bson import json_util, ObjectId
+from . import helpers
 from .constants import (
     NEW_SETUP_MSG_INTRO,
     NEW_SETUP_MSG_MONGODB_INSTRUCTIONS,
     CONFIG_MONGODB_USERNAME,
     CONFIG_MONGODB_PASSWORD,
     CONFIG_MONGODB_CLUSTER_NAME,
     CONFIG_MONGODB_DB_NAME,
@@ -58,15 +59,15 @@
     client: MongoClient | None = None
     database = None
     new_setup: bool = False
     path_config_dir = str(pathlib.Path(
         __file__).resolve().parent)
     path_config_file = f"{path_config_dir}/cabinet_config.json"
     path_cabinet: str | None = None
-    path_log: str | None = None
+    path_log: str = ''
 
     def _get_config(self, key=None):
         """
         Retrieves the value associated with the specified key from the configuration file.
 
         Args:
             key (str): The key to retrieve the corresponding value.
@@ -123,15 +124,15 @@
             with open(self.path_config_file, 'r+', encoding="utf8") as file:
                 return json.load(file)[key]
         except FileNotFoundError:
             # setup
             self.new_setup = True
 
             # make .cabinet directory, if needed
-            path_cabinet = self._expand_aliases("~/.cabinet")
+            path_cabinet = helpers.resolve_path("~/.cabinet")
             path_cabinet_slash = os.path.join(path_cabinet, '')
             if not os.path.exists(path_cabinet_slash):
                 os.makedirs(path_cabinet_slash)
 
             has_mongodb = input(NEW_SETUP_MSG_INTRO)
 
             if not has_mongodb.lower().startswith('y'):
@@ -212,27 +213,14 @@
             if is_print:
                 print(json.dumps(message, indent=2))
         except json.JSONDecodeError:
             if is_print:
                 print(message)
             return message
 
-    def _expand_aliases(self, string):
-        """
-        Expands environment variables and user aliases in a string.
-
-        Args:
-            - string (str): the string to expand
-
-        Returns:
-            - The expanded string.
-        """
-        return string.replace("$HOME", os.environ.get("HOME",
-            "")).replace("~", os.environ.get("HOME", ""))
-
     def __init__(self, path_cabinet: str | None = None):
         """
         Initializes the Cabinet instance with the provided or default configuration.
 
         Args:
             path_cabinet (str, optional): The path to the cabinet directory. Defaults to None.
 
@@ -244,15 +232,15 @@
             - The attributes of the Cabinet instance are set based on the configuration values.
 
         """
 
         if path_cabinet is not None:
             self.path_cabinet = path_cabinet
         else:
-            self.path_cabinet = self._expand_aliases(self._get_config('path_cabinet'))
+            self.path_cabinet = helpers.resolve_path(self._get_config('path_cabinet'))
 
         # these should match class attributes above
         keys = ["mongodb_username", "mongodb_password",
                 "mongodb_cluster_name", "mongodb_db_name", "path_cabinet"]
 
         for key in keys:
             if key == 'path_cabinet' and path_cabinet is not None:
@@ -283,15 +271,15 @@
             sys.exit(-1)
         except pymongo.errors.ConfigurationError as error:
             print(ERROR_MONGODB_DNS)
             print(error)
             sys.exit(-1)
 
 
-        path_log = self._expand_aliases(self.get('path', 'log') or '~/.cabinet/log')
+        path_log = helpers.resolve_path(self.get('path', 'log', returnType=str) or '~/.cabinet/log')
         path_log_slash = os.path.join(path_log, '')
 
         # Create the directory if it doesn't exist
         if not os.path.exists(path_log_slash):
             os.makedirs(path_log_slash)
 
         self.path_log = path_log_slash
@@ -575,85 +563,99 @@
         if is_print:
             print(f"Modified {result.modified_count} item(s)")
             print(
                 f"{' -> '.join(attribute[:-1])} set to {value}\n")
 
         return value
 
-    def get(self, *attributes, warn_missing=False, is_print=False, no_cache=False):
+    T = TypeVar('T', bound=Any)  # Generic type variable for returnType
+    def get(self, *attributes, warn_missing: bool = False, is_print: bool = False,
+            no_cache: bool = False, returnType: Optional[Type[T]] = None) -> Optional[T]:
         """
-        Returns a property or properties from MongoDB based on the input attributes,
-        using a cache file to improve performance.
+            Returns a property or properties from MongoDB based on the input attributes,
+            using a cache file to improve performance.
 
-        Args:
-            - *attributes (str): a sequence of strings representing nested attributes
-            - warn_missing (bool, optional): whether to warn if an attribute is missing
-            - is_print (bool, optional): whether to print the return value
-            - no_cache (bool, optional): whether to force a fresh MongoDB call
-                - by default, if cache is over 1 hour old,
-                    update will be called and cache will be updated
+            Args:
+                *attributes (str): A sequence of strings representing nested attributes.
+                warn_missing (bool, optional): Whether to warn if an attribute is missing.
+                is_print (bool, optional): Whether to print the return value.
+                no_cache (bool, optional): Whether to force a fresh MongoDB call.
+                returnType (Type[T], optional): The expected return type of the result.
+                    Defaults to object, which includes any type.
 
-        Returns:
-            - The value of the attribute if it exists in the cache or MongoDB, otherwise None.
+            Returns:
+                The value of the attribute if it exists in the cache or MongoDB,
+                cast to returnType, otherwise None.
 
-        Usage:
-            - get('person', 'tyler', 'salary') returns the value of person -> tyler -> salary
-        """
+            Usage:
+                get('person', 'tyler', 'salary')  # Returns the value of person -> tyler -> salary
+            """
 
         path_cache_file = f"{self.path_config_dir}/cache.json"
         cache_update_needed = no_cache
 
         # Check if cache file exists and is less than 1 hour old
         if os.path.exists(path_cache_file):
             last_modified = os.path.getmtime(path_cache_file)
             if (time.time() - last_modified) / 3600 > 1:
                 cache_update_needed = True
         else:
             cache_update_needed = True
 
         if cache_update_needed:
-            self.update_cache()  # Update the cache file
+            self.update_cache()
 
         # Read from cache
         try:
             with open(path_cache_file, "r", encoding="utf-8") as file:
                 cached_data = json.load(file)
         except FileNotFoundError:
             self.log(f"Cache file not found at {path_cache_file}", level="warn")
             return None
         except json.decoder.JSONDecodeError:
-            self.log(f"Could not read Cabinet cache at {path_cache_file}. Clearing.",
-                     level="warn")
+            self.log(f"Could not read Cabinet cache at {path_cache_file}. Clearing.", level="warn")
             try:
                 os.remove(path_cache_file)
                 print(f"File removed successfully: {path_cache_file}")
                 print("Please retry your last command.")
                 sys.exit(0)
             except PermissionError:
                 self.log(f"Permission denied: Unable to delete the file at {path_cache_file}",
-                         level="critical")
+                         level="error")
+            return None
 
         # Process the cached data
         for document in cached_data:
             result = document
             for attribute in attributes:
                 if isinstance(result, dict) and attribute in result:
                     result = result[attribute]
                 else:
                     if warn_missing:
                         self.log(f"Attribute '{attribute}' is missing", level="warn")
                     return None
 
             if isinstance(result, str):
-                result = self._expand_aliases(result)
+                result = helpers.resolve_path(result)
+
+            if is_print:
+                print(result)
 
             if is_print:
                 print(result)
 
-            return result
+            # Handle returnType if specified
+            if returnType is not None:
+                try:
+                    return returnType(result)
+                except (ValueError, TypeError) as e:
+                    self.log(f"Error casting result to {returnType}: {str(e)}", level="error")
+                    return None
+            else:
+                return result  # Return as is if no specific returnType is needed
 
         if warn_missing:
             self.log("No document found in cache or MongoDB", level="warn")
         return None
 
     def remove(self, *attribute, is_print: bool = False):
         """
@@ -820,70 +822,80 @@
 
             return content.split('\n')
         except FileNotFoundError as error:
             if not ignore_not_found:
                 self.log(f"get_file_as_array: {error}", level="error")
             return None
 
-    def write_file(self, file_name: str, file_path: Optional[str] = None,
+    def write_file(self, file_name: str, path_file: str = '',
                    content: Optional[str] = None, append: bool = False,
                    is_quiet: bool = False) -> bool:
         """
-        Writes a file to the specified path and creates subfolders if necessary.
+        writes a file to the specified path, creating necessary subfolders.
+        resolves aliases in paths.
 
-        Args:
-            - file_name (str): The name of the file to write.
-            - file_path (str, optional): The path to the directory where the file should be written.
-                If None, path_log is used.
-            - content (str, optional): The contents to write to the file.
-                If None, an empty file is created.
-            - append (bool, optional): Whether to append to the file instead of overwriting it.
-                Default: False
-            - is_quiet (bool, optional): Whether to skip printing status messages.
-                Default: False
-
-        Return:
-            True if the file was written successfully
-            False otherwise.
-        """
+        args:
+            file_name (str): the name of the file to write.
+            path_file (str, optional): the directory path for the file.
+                uses default log path if empty.
+                use 'notes' for cabinet -> path -> notes
+            content (str, optional): the content to write to the file.
+                creates an empty file if none.
+            append (bool, optional): set to true to append to the file instead of overwriting.
+                defaults to false.
+            is_quiet (bool, optional): set to true to suppress status messages.
+                defaults to false.
 
+        returns:
+            true if the file was successfully written, false otherwise.
+        """
         try:
-            if file_path is None:
-                file_path = self.path_log.rstrip("/")
-            elif file_path == "notes":
-                file_path = self.get('path', 'notes')
-            os.makedirs(file_path, exist_ok=True)
-            with open(f"{file_path}/{file_name}", 'a+' if append else 'w', encoding="utf8") as file:
+            # handle default file path and notes alias
+            if not path_file:
+                path_file = helpers.resolve_path(self.path_log or '~/.cabinet/log')
+            elif path_file == "notes":
+                path_notes: str = self.get('path', 'notes', returnType=str) or ''
+                path_file = helpers.resolve_path(path_notes or self.path_log or '~/.cabinet/notes')
+
+            # create directory if it does not exist
+            os.makedirs(path_file, exist_ok=True)
+
+            # write content to file
+            mode = 'a+' if append else 'w'
+            with open(os.path.join(path_file, file_name), mode, encoding="utf8") as file:
                 file.write(content or "")
+
+            # optionally print status message
             if not is_quiet:
-                print(f"Wrote to '{file_path}/{file_name}'")
+                print(f"wrote to '{os.path.join(path_file, file_name)}'")
+
             return True
         except (OSError, IOError) as error:
             self.log(f"write_file: {error}", level="error")
             return False
 
     def export(self):
         """
         Exports all data in MongoDB to JSON
         """
         cache = self.update_cache()
 
-        path_export = self._expand_aliases('~/.cabinet/export')
+        path_export = helpers.resolve_path('~/.cabinet/export')
         path_export_slash = os.path.join(path_export, '')
 
         # Create the directory if it doesn't exist
         if not os.path.exists(path_export_slash):
             os.makedirs(path_export_slash)
 
         current_datetime = datetime.now()
         formatted_datetime = current_datetime.strftime("%Y-%m-%d %H:%M:%S")
         file_name = f"cabinet export {formatted_datetime}"
 
         with open(file_name, 'w', encoding='utf-8') as file:
-            file.write(cache)
+            file.write(cache or '')
 
 
 def main():
     """
     Main function for running Cabinet.
 
     Args:
```

### Comparing `cabinet-2024.4.15.2/src/cabinet/constants.py` & `cabinet-2024.4.25.1/src/cabinet/constants.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.15.2/src/cabinet/mail.py` & `cabinet-2024.4.25.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.15.2/src/cabinet.egg-info/PKG-INFO` & `cabinet-2024.4.25.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.15.2
+Version: 2024.4.25.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

