# Comparing `tmp/variable_local-0.0.90.tar.gz` & `tmp/variable_local-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variable_local-0.0.90.tar", last modified: Tue Apr 16 22:46:35 2024, max compression
+gzip compressed data, was "variable_local-0.0.91.tar", last modified: Fri Apr 26 12:19:19 2024, max compression
```

## Comparing `variable_local-0.0.90.tar` & `variable_local-0.0.91.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:46:35.848099 variable_local-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-16 22:46:35.848099 variable_local-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-16 22:46:04.000000 variable_local-0.0.90/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-16 22:46:04.000000 variable_local-0.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:46:35.848099 variable_local-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-16 22:46:04.000000 variable_local-0.0.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:46:35.844099 variable_local-0.0.90/variable_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:46:35.848099 variable_local-0.0.90/variable_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:46:04.000000 variable_local-0.0.90/variable_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-16 22:46:04.000000 variable_local-0.0.90/variable_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-04-16 22:46:04.000000 variable_local-0.0.90/variable_local/src/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 22:46:04.000000 variable_local-0.0.90/variable_local/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-16 22:46:04.000000 variable_local-0.0.90/variable_local/src/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:46:35.848099 variable_local-0.0.90/variable_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-16 22:46:35.000000 variable_local-0.0.90/variable_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-16 22:46:35.000000 variable_local-0.0.90/variable_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:46:35.000000 variable_local-0.0.90/variable_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-16 22:46:35.000000 variable_local-0.0.90/variable_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 22:46:35.000000 variable_local-0.0.90/variable_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:19:19.275912 variable_local-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 12:19:19.275912 variable_local-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-26 12:18:43.000000 variable_local-0.0.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-26 12:18:43.000000 variable_local-0.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 12:19:19.275912 variable_local-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-26 12:18:43.000000 variable_local-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:19:19.271911 variable_local-0.0.91/variable_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:19:19.275912 variable_local-0.0.91/variable_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:18:43.000000 variable_local-0.0.91/variable_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-26 12:18:43.000000 variable_local-0.0.91/variable_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-26 12:18:43.000000 variable_local-0.0.91/variable_local/src/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 12:18:43.000000 variable_local-0.0.91/variable_local/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-26 12:18:43.000000 variable_local-0.0.91/variable_local/src/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:19:19.275912 variable_local-0.0.91/variable_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 12:19:19.000000 variable_local-0.0.91/variable_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-26 12:19:19.000000 variable_local-0.0.91/variable_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:19:19.000000 variable_local-0.0.91/variable_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 12:19:19.000000 variable_local-0.0.91/variable_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 12:19:19.000000 variable_local-0.0.91/variable_local.egg-info/top_level.txt
```

### Comparing `variable_local-0.0.90/PKG-INFO` & `variable_local-0.0.91/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.90
+Version: 0.0.91
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `variable_local-0.0.90/README.md` & `variable_local-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.90/pyproject.toml` & `variable_local-0.0.91/pyproject.toml`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.90/setup.py` & `variable_local-0.0.91/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = 'variable-local'
 package_dir = PACKAGE_NAME.replace('-', '_')
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.90',  # https://pypi.org/project/variable-local
+    version='0.0.91',  # https://pypi.org/project/variable-local
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles variable Local/Remote Python",
     long_description="PyPI Package for Circles variable Local/Remote Python",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
```

### Comparing `variable_local-0.0.90/variable_local/src/constants.py` & `variable_local-0.0.91/variable_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.90/variable_local/src/template.py` & `variable_local-0.0.91/variable_local/src/template.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from datetime import datetime
 
 from language_local.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 from smartlink_local.smartlink import SmartLinkLocal
 
 from .constants import variable_local_logger_init_object
-from .utils import to_unified
 from .variable import VariablesLocal
 
 logger = Logger.create_logger(object=variable_local_logger_init_object)
 
 LEFT_BRACKETS = '{'
 RIGHT_BRACKETS = '}'
 
@@ -95,36 +94,34 @@
         """Returns:
             1. A list of all variable names that were inside curly braces of message
             2. A string that's a copy of the message but without the variable names inside curly braces,
             and a randomly chosen parameter out of each curly braces options:
             "Hello {First Name}, how are you {feeling|doing}?" --> "Hello {}, how are you doing?" 
         """
         logger.start(object={'kwargs': kwargs})
-        unified_kwargs = {to_unified(name): var_id
-                          for name, var_id in kwargs.get('kwargs', kwargs).items()}
+        kwargs = kwargs.get('kwargs', kwargs)
         variable_names_list = []
         message_without_variable_names = kwargs.get("message", self.message)
 
         pattern = re.compile(r'\${{[^}]*}}')  # ${{vraiable}}
         matches = pattern.findall(message_without_variable_names)
         for exact_match in matches:
             match = exact_match[3:-2].strip()  # remove '${{' and '}}'
-            unified_match = to_unified(match)
             if '|' in match:  # # choose random option from {A|B|C}
                 # pick random choice
                 options = match.split('|')
                 random_option = random.choice(options)
                 message_without_variable_names = message_without_variable_names.replace(
                     exact_match, random_option, 1)
 
-            elif unified_match in unified_kwargs:
+            elif match in kwargs:
                 message_without_variable_names = message_without_variable_names.replace(
-                    exact_match, str(kwargs[match] if match in kwargs else unified_kwargs[unified_match]), 1)
+                    exact_match, str(kwargs[match] if match in kwargs else kwargs[match]), 1)
 
-            elif unified_match in self.variable.clean_name2id_dict.keys():
+            elif match in self.variable.name2id_dict.keys():
                 # replace variable name with '{}' and add variable names to list
                 message_without_variable_names = message_without_variable_names.replace(exact_match, '{}', 1)
                 variable_names_list.append(match)
 
             else:
                 message_without_variable_names = message_without_variable_names.replace(
                     exact_match, self.special_variable(match, **kwargs), 1)
```

### Comparing `variable_local-0.0.90/variable_local/src/variable.py` & `variable_local-0.0.91/variable_local/src/variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,41 +2,37 @@
 
 from database_mysql_local.generic_crud import GenericCRUD
 from language_local.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 from user_context_remote.user_context import UserContext
 
 from .constants import variable_local_logger_init_object, VARIABLE_LOCAL_PYTHON_PACKAGE_COMPONENT_ID
-from .utils import to_unified
 
 logger = Logger.create_logger(object=variable_local_logger_init_object)
 cache_with_timeout = {}
 
 
 class VariablesLocal(GenericCRUD):
     def __init__(self):
         super().__init__(default_schema_name="field", default_table_name="field_table",
                          default_view_table_name="field_view", default_id_column_name="variable_id")
         self.name2id_dict = {}
-        self.clean_name2id_dict = {}
         self.id2name_dict = {}
         self.next_variable_id = 1
         variable_names_dict = self.load_variable_names_dict_from_variable_table()
         for variable_id in variable_names_dict:
             self.add(variable_id=variable_id,
                      variable_name=variable_names_dict[variable_id])
 
     def add(self, variable_id: int, variable_name: str) -> None:
         logger.start(object={'variable_id': variable_id,
                              'variable_name': variable_name})
         try:
             if variable_id is not None and variable_name is not None:
                 self.name2id_dict[variable_name] = variable_id
-                clean_var = to_unified(variable_name)
-                self.clean_name2id_dict[clean_var] = variable_id
                 self.id2name_dict[variable_id] = variable_name
             # TODO: just make bad performance, seems that can be removed
             # self.cursor.execute("""INSERT INTO variable_table(variable_id, name) VALUES (%s, %s)""", [
             #                     variable_id, variable_name])
             # GenericCRUD(schema_name=VARIABLE_LOCAL_SCHEMA_NAME).insert(
             #     table_name='variable_table', json_data={'variable_id': variable_id, 'name': variable_name})
             # self.connector.commit()
@@ -46,19 +42,15 @@
             logger.exception(message, object=exception)
             logger.end()
             raise
         logger.end()
 
     def get_variable_id_by_variable_name(self, variable_name: str) -> int:
         logger.start(object={'variable_name': variable_name})
-        unified_variable_name = to_unified(variable_name)
-        if variable_name in self.name2id_dict:  # just in case it's not there already
-            self.clean_name2id_dict[unified_variable_name] = self.name2id_dict[variable_name]
-
-        variable_id = self.clean_name2id_dict.get(unified_variable_name)
+        variable_id = self.name2id_dict.get(variable_name)
         logger.end(object={'variable_id': variable_id})
         return variable_id
 
     def get_variable_name_by_variable_id(self, variable_id: int) -> str:
         logger.start(object={'variable_id': variable_id})
         variable_name = self.id2name_dict[variable_id]
         logger.end(object={'variable_name': variable_name})
```

### Comparing `variable_local-0.0.90/variable_local.egg-info/PKG-INFO` & `variable_local-0.0.91/variable_local.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.90
+Version: 0.0.91
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

