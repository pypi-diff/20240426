# Comparing `tmp/loggerk-0.0.3.tar.gz` & `tmp/loggerk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerk-0.0.3.tar", last modified: Thu Apr 25 15:45:27 2024, max compression
+gzip compressed data, was "loggerk-0.0.4.tar", last modified: Thu Apr 25 22:09:11 2024, max compression
```

## Comparing `loggerk-0.0.3.tar` & `loggerk-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.134089 loggerk-0.0.3/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     7048 2024-04-22 22:17:13.000000 loggerk-0.0.3/LICENSE
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3296 2024-04-25 15:45:27.133890 loggerk-0.0.3/PKG-INFO
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.132545 loggerk-0.0.3/loggerk/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     5620 2024-04-25 15:39:00.000000 loggerk-0.0.3/loggerk/__init__.py
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.133243 loggerk-0.0.3/loggerk/config/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3015 2024-04-25 14:37:20.000000 loggerk-0.0.3/loggerk/config/__init__.py
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.133377 loggerk-0.0.3/loggerk/formatters/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      311 2024-04-23 15:13:03.000000 loggerk-0.0.3/loggerk/formatters/__init__.py
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.133505 loggerk-0.0.3/loggerk/handlers/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     4777 2024-04-25 14:38:13.000000 loggerk-0.0.3/loggerk/handlers/__init__.py
-drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 15:45:27.133663 loggerk-0.0.3/loggerk.egg-info/
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3296 2024-04-25 15:45:27.000000 loggerk-0.0.3/loggerk.egg-info/PKG-INFO
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      277 2024-04-25 15:45:27.000000 loggerk-0.0.3/loggerk.egg-info/SOURCES.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        1 2024-04-25 15:45:27.000000 loggerk-0.0.3/loggerk.egg-info/dependency_links.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        6 2024-04-25 15:45:27.000000 loggerk-0.0.3/loggerk.egg-info/requires.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        8 2024-04-25 15:45:27.000000 loggerk-0.0.3/loggerk.egg-info/top_level.txt
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)       38 2024-04-25 15:45:27.134124 loggerk-0.0.3/setup.cfg
--rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     1016 2024-04-25 15:45:10.000000 loggerk-0.0.3/setup.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 22:09:11.259747 loggerk-0.0.4/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     7048 2024-04-22 22:17:13.000000 loggerk-0.0.4/LICENSE
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     4131 2024-04-25 22:09:11.259565 loggerk-0.0.4/PKG-INFO
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 22:09:11.257969 loggerk-0.0.4/loggerk/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     5627 2024-04-25 21:59:10.000000 loggerk-0.0.4/loggerk/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 22:09:11.258687 loggerk-0.0.4/loggerk/config/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     3015 2024-04-25 21:57:19.000000 loggerk-0.0.4/loggerk/config/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 22:09:11.259044 loggerk-0.0.4/loggerk/formatters/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      311 2024-04-23 15:13:03.000000 loggerk-0.0.4/loggerk/formatters/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 22:09:11.259176 loggerk-0.0.4/loggerk/handlers/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     4777 2024-04-25 14:38:13.000000 loggerk-0.0.4/loggerk/handlers/__init__.py
+drwxr-xr-x   0 angeldejesussanchezmorales   (501) staff       (20)        0 2024-04-25 22:09:11.259354 loggerk-0.0.4/loggerk.egg-info/
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     4131 2024-04-25 22:09:11.000000 loggerk-0.0.4/loggerk.egg-info/PKG-INFO
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)      277 2024-04-25 22:09:11.000000 loggerk-0.0.4/loggerk.egg-info/SOURCES.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        1 2024-04-25 22:09:11.000000 loggerk-0.0.4/loggerk.egg-info/dependency_links.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        6 2024-04-25 22:09:11.000000 loggerk-0.0.4/loggerk.egg-info/requires.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)        8 2024-04-25 22:09:11.000000 loggerk-0.0.4/loggerk.egg-info/top_level.txt
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)       38 2024-04-25 22:09:11.259785 loggerk-0.0.4/setup.cfg
+-rw-r--r--   0 angeldejesussanchezmorales   (501) staff       (20)     1016 2024-04-25 22:08:37.000000 loggerk-0.0.4/setup.py
```

### Comparing `loggerk-0.0.3/LICENSE` & `loggerk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerk-0.0.3/PKG-INFO` & `loggerk-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerk
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a custom logger module for Python
 Author: Kuantik DataJump
 Author-email: master@kuantik.mx
 Maintainer: Angel de Jesús Sanchez Morales
 Maintainer-email: angel.sanchez@kuantik.mx
 Keywords: python,logging
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 # loggerk
 This is a custom logger module for Python
 
 Enviroment variables required:
 
 - `LOGGER_APP_NAME`: The name of the App
 - `LOGGER_URLS`: a list of URLS to send the log requests to. Separated by commas.
-- `LOGGER_CREDENTIALS`: If needed, the credentials to send the log resuests with.
+- `LOGGER_CREDENTIALS`: If needed, the credentials sent in the authorization header of the log request.
 
 
 ## Usage
 Import LoggerK from the `loggerk` mdoule 
 
 ```python
 from loggerk import LoggerK
@@ -52,28 +52,14 @@
 * `app_name: str`
 * `level: str | int`
 * `config: ConfigDict`
 * `file_path: str`
 
 The only required argument is `name`. The rest of the arguments are Optional.
 
-### Note:
-Initializing two `LoggerK` instances with the same name will behave as a Singleton, so any new configuration to the new instance will affect all existing instances with the same name.
-
-#### Example:
-```python
-logger_1 = LoggerK("my_new_logger")
-
-logger_2 = LoggerK(
-    "my_new_logger", 
-    config=SOME_CUSTOM_CONFIG,
-)
-
-# The new config on logger_2 will apply also for the logger_1 as they share the same name.
-```
 
 ### `app_name`
 
 Represents the name of the application in which the logger instance is being created. If it is not provided, it will be extracted from the environment as `LOGGER_APP_NAME`.
 
 ### `level`
 
@@ -98,7 +84,43 @@
 - An `StreamingHandler` to the standar output.
 - A `RotatingFileHandler` that defaults to `"logs/app.log"`
 - A `CustomHttpHandler` that will make a post request for every log message to the first URL that returns a succesful response within the given URLs  in the `LOGGER_URLS` env variable.
 
 ### `file_path`
 
 When given a value, will override every FileHandler inside the `config` dictionary.
+
+
+### Note:
+Initializing two `LoggerK` instances with the same name will behave as a Singleton, so any new configuration to the new instance will affect all existing instances with the same name.
+
+#### Example:
+```python
+logger_1 = LoggerK("my_new_logger")
+
+logger_2 = LoggerK(
+    "my_new_logger", 
+    config=SOME_CUSTOM_CONFIG,
+)
+
+# The new config on logger_2 will apply also for the logger_1 as they share the same name.
+```
+
+## Configuring the log instance
+
+If needed, the log instance can be configured after initialization by updating the `ConfigDict` in the  `Loggerk.config` attribute.
+
+#### Example:
+
+```python
+logger = LoggerK(__name__)
+
+current_config = logger.config # accessing the current configuration of the looger instance. This returns a copy of the config dictionary, so updating directly will have no efect on the actual configuration of the logger instance.
+
+# updating the configuration
+new_config = current_configuration["handlers"]["file"]["level"] = "ERROR" #changing the debug level of the file handler
+
+# setting the new configuration to the logger instance
+logger.config = new_configuration
+```
+
+Every time the value of `config` is set, the instance will be reconfigured, so all new configurations are applied.
```

### Comparing `loggerk-0.0.3/loggerk/__init__.py` & `loggerk-0.0.4/loggerk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self._config = config
 
         self.app_name = app_name
         self._set_up_handlers()
 
     @property
     def config(self) -> ConfigDict:
-        return self._config
+        return self._config.copy()
 
     @config.setter
     def config(self, new_config: ConfigDict):
         self._prepare_handlers(new_config)
         self._config = new_config
 
     def _set_up_handlers(self):
```

### Comparing `loggerk-0.0.3/loggerk/config/__init__.py` & `loggerk-0.0.4/loggerk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerk-0.0.3/loggerk/handlers/__init__.py` & `loggerk-0.0.4/loggerk/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerk-0.0.3/loggerk.egg-info/PKG-INFO` & `loggerk-0.0.4/loggerk.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerk
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a custom logger module for Python
 Author: Kuantik DataJump
 Author-email: master@kuantik.mx
 Maintainer: Angel de Jesús Sanchez Morales
 Maintainer-email: angel.sanchez@kuantik.mx
 Keywords: python,logging
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 # loggerk
 This is a custom logger module for Python
 
 Enviroment variables required:
 
 - `LOGGER_APP_NAME`: The name of the App
 - `LOGGER_URLS`: a list of URLS to send the log requests to. Separated by commas.
-- `LOGGER_CREDENTIALS`: If needed, the credentials to send the log resuests with.
+- `LOGGER_CREDENTIALS`: If needed, the credentials sent in the authorization header of the log request.
 
 
 ## Usage
 Import LoggerK from the `loggerk` mdoule 
 
 ```python
 from loggerk import LoggerK
@@ -52,28 +52,14 @@
 * `app_name: str`
 * `level: str | int`
 * `config: ConfigDict`
 * `file_path: str`
 
 The only required argument is `name`. The rest of the arguments are Optional.
 
-### Note:
-Initializing two `LoggerK` instances with the same name will behave as a Singleton, so any new configuration to the new instance will affect all existing instances with the same name.
-
-#### Example:
-```python
-logger_1 = LoggerK("my_new_logger")
-
-logger_2 = LoggerK(
-    "my_new_logger", 
-    config=SOME_CUSTOM_CONFIG,
-)
-
-# The new config on logger_2 will apply also for the logger_1 as they share the same name.
-```
 
 ### `app_name`
 
 Represents the name of the application in which the logger instance is being created. If it is not provided, it will be extracted from the environment as `LOGGER_APP_NAME`.
 
 ### `level`
 
@@ -98,7 +84,43 @@
 - An `StreamingHandler` to the standar output.
 - A `RotatingFileHandler` that defaults to `"logs/app.log"`
 - A `CustomHttpHandler` that will make a post request for every log message to the first URL that returns a succesful response within the given URLs  in the `LOGGER_URLS` env variable.
 
 ### `file_path`
 
 When given a value, will override every FileHandler inside the `config` dictionary.
+
+
+### Note:
+Initializing two `LoggerK` instances with the same name will behave as a Singleton, so any new configuration to the new instance will affect all existing instances with the same name.
+
+#### Example:
+```python
+logger_1 = LoggerK("my_new_logger")
+
+logger_2 = LoggerK(
+    "my_new_logger", 
+    config=SOME_CUSTOM_CONFIG,
+)
+
+# The new config on logger_2 will apply also for the logger_1 as they share the same name.
+```
+
+## Configuring the log instance
+
+If needed, the log instance can be configured after initialization by updating the `ConfigDict` in the  `Loggerk.config` attribute.
+
+#### Example:
+
+```python
+logger = LoggerK(__name__)
+
+current_config = logger.config # accessing the current configuration of the looger instance. This returns a copy of the config dictionary, so updating directly will have no efect on the actual configuration of the logger instance.
+
+# updating the configuration
+new_config = current_configuration["handlers"]["file"]["level"] = "ERROR" #changing the debug level of the file handler
+
+# setting the new configuration to the logger instance
+logger.config = new_configuration
+```
+
+Every time the value of `config` is set, the instance will be reconfigured, so all new configurations are applied.
```

### Comparing `loggerk-0.0.3/setup.py` & `loggerk-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 here: pathlib.Path = pathlib.Path(__file__).parent.resolve()
 
 long_description: str = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "This is a custom logger module for Python"
 
 # Setting up
 setup(
     name="loggerk",
     version=VERSION,
     author="Kuantik DataJump",
```

