# Comparing `tmp/r4ven_utils-0.0.4.tar.gz` & `tmp/r4ven_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r4ven_utils-0.0.4.tar", last modified: Fri Jan 12 22:23:18 2024, max compression
+gzip compressed data, was "r4ven_utils-0.0.5.tar", last modified: Fri Apr 26 14:32:19 2024, max compression
```

## Comparing `r4ven_utils-0.0.4.tar` & `r4ven_utils-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-01-12 22:23:18.084077 r4ven_utils-0.0.4/
--rwxrwxrwx   0 victor    (1000) victor    (1000)    35149 2022-11-07 06:44:00.000000 r4ven_utils-0.0.4/LICENSE
--rw-r--r--   0 victor    (1000) victor    (1000)     3809 2024-01-12 22:23:18.084077 r4ven_utils-0.0.4/PKG-INFO
--rwxrwxrwx   0 victor    (1000) victor    (1000)     2980 2022-11-07 07:50:32.000000 r4ven_utils-0.0.4/README.md
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-01-12 22:23:18.084077 r4ven_utils-0.0.4/r4ven_utils/
--rwxrwxrwx   0 victor    (1000) victor    (1000)        0 2022-11-07 06:44:00.000000 r4ven_utils-0.0.4/r4ven_utils/__init__.py
--rwxrwxrwx   0 victor    (1000) victor    (1000)      691 2022-11-24 11:06:45.000000 r4ven_utils-0.0.4/r4ven_utils/exceptions.py
--rwxrwxrwx   0 victor    (1000) victor    (1000)     4389 2024-01-12 22:05:03.000000 r4ven_utils-0.0.4/r4ven_utils/log4me.py
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-01-12 22:23:18.084077 r4ven_utils-0.0.4/r4ven_utils.egg-info/
--rw-r--r--   0 victor    (1000) victor    (1000)     3809 2024-01-12 22:23:18.000000 r4ven_utils-0.0.4/r4ven_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 victor    (1000) victor    (1000)      269 2024-01-12 22:23:18.000000 r4ven_utils-0.0.4/r4ven_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 victor    (1000) victor    (1000)        1 2024-01-12 22:23:18.000000 r4ven_utils-0.0.4/r4ven_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 victor    (1000) victor    (1000)       12 2024-01-12 22:23:18.000000 r4ven_utils-0.0.4/r4ven_utils.egg-info/top_level.txt
--rwxrwxrwx   0 victor    (1000) victor    (1000)      350 2024-01-12 22:23:18.084077 r4ven_utils-0.0.4/setup.cfg
--rwxrwxrwx   0 victor    (1000) victor    (1000)     1454 2023-05-03 18:55:13.000000 r4ven_utils-0.0.4/setup.py
-drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-01-12 22:23:18.084077 r4ven_utils-0.0.4/tests/
--rwxrwxrwx   0 victor    (1000) victor    (1000)     5470 2024-01-12 22:09:03.000000 r4ven_utils-0.0.4/tests/test_log4me.py
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 14:32:19.103107 r4ven_utils-0.0.5/
+-rw-rw-r--   0 victor    (1000) victor    (1000)    35149 2022-11-07 06:44:00.000000 r4ven_utils-0.0.5/LICENSE
+-rw-r--r--   0 victor    (1000) victor    (1000)     3209 2024-04-26 14:32:19.103107 r4ven_utils-0.0.5/PKG-INFO
+-rw-rw-r--   0 victor    (1000) victor    (1000)     2380 2024-04-26 14:24:30.000000 r4ven_utils-0.0.5/README.md
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 14:32:19.103107 r4ven_utils-0.0.5/r4ven_utils/
+-rw-rw-r--   0 victor    (1000) victor    (1000)        0 2022-11-07 06:44:00.000000 r4ven_utils-0.0.5/r4ven_utils/__init__.py
+-rw-rw-r--   0 victor    (1000) victor    (1000)      691 2022-11-24 11:06:45.000000 r4ven_utils-0.0.5/r4ven_utils/exceptions.py
+-rw-rw-r--   0 victor    (1000) victor    (1000)     4373 2024-04-26 13:48:19.000000 r4ven_utils-0.0.5/r4ven_utils/log4me.py
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 14:32:19.103107 r4ven_utils-0.0.5/r4ven_utils.egg-info/
+-rw-r--r--   0 victor    (1000) victor    (1000)     3209 2024-04-26 14:32:19.000000 r4ven_utils-0.0.5/r4ven_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 victor    (1000) victor    (1000)      269 2024-04-26 14:32:19.000000 r4ven_utils-0.0.5/r4ven_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)        1 2024-04-26 14:32:19.000000 r4ven_utils-0.0.5/r4ven_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)       12 2024-04-26 14:32:19.000000 r4ven_utils-0.0.5/r4ven_utils.egg-info/top_level.txt
+-rw-rw-r--   0 victor    (1000) victor    (1000)      350 2024-04-26 14:32:19.107107 r4ven_utils-0.0.5/setup.cfg
+-rw-rw-r--   0 victor    (1000) victor    (1000)     1454 2024-04-26 14:30:48.000000 r4ven_utils-0.0.5/setup.py
+drwxrwxr-x   0 victor    (1000) victor    (1000)        0 2024-04-26 14:32:19.103107 r4ven_utils-0.0.5/tests/
+-rw-rw-r--   0 victor    (1000) victor    (1000)     5162 2024-04-26 13:42:22.000000 r4ven_utils-0.0.5/tests/test_log4me.py
```

### Comparing `r4ven_utils-0.0.4/LICENSE` & `r4ven_utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `r4ven_utils-0.0.4/PKG-INFO` & `r4ven_utils-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: r4ven_utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: The companion that holds your grab-bag of utility functions and objects
 Home-page: https://github.com/VictorFantucci/r4ven_utils_dev
-Download-URL: https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.4.tar.gz
+Download-URL: https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.5.tar.gz
 Author: Victor Vinci Fantucci
 Author-email: victor.v.fantucci@gmail.com
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/VictorFantucci/r4ven_utils_dev/issues
 Keywords: r4ven_utils,utils,logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -32,38 +32,29 @@
 ## What is it?
 
 **r4ven_utils** is all of those of utilities you keep reimplementing across your Python projects, that all got together and decided to live in harmony.
 
 ## Main Features
 Here are some of the utilities that r4ven keep under it's wings:
 
-  - [**log4me**][log-4-me] - Creation of a logger object specific to the function in which it's called.
+  - [**log4me**][log-4-me] - convenient way to implement logging in Python applications, ensuring that logs are organized and execution times are recorded accurately.
 
    [log-4-me]: r4ven_utils/log4me.py
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/VictorFantucci/r4ven_utils_dev
 
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/r4ven_utils).
 ```sh
 # or PyPI
 pip install r4ven-utils
 ```
 
-## Dependencies
-- [**os**][os-module] - This module provides a portable way of using operating system dependent functionality.
-- [**sys**][sys-module] - This module provides access to some variables used or maintained by the interpreter and to functions that interact strongly with the interpreter.
-- [**logging**][logging-module]- This module defines functions and classes which implement a flexible event logging system for applications and libraries.
-
-[os-module]: https://docs.python.org/3/library/os.html
-[sys-module]: https://docs.python.org/3/library/sys.html
-[logging-module]: https://docs.python.org/3/library/logging.htmlhttps://github.com/stub42/pytz
-
 ## License
 [GPLv3](LICENSE)
 
 ## Documentation
 All my scripts have very detailed docstrings and comments that make their use intuitive and simple. As the project grows and takes shape I plan to write a  proper documentation for it.
 
 ## Background
```

### Comparing `r4ven_utils-0.0.4/README.md` & `r4ven_utils-0.0.5/r4ven_utils.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: r4ven_utils
+Version: 0.0.5
+Summary: The companion that holds your grab-bag of utility functions and objects
+Home-page: https://github.com/VictorFantucci/r4ven_utils_dev
+Download-URL: https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.5.tar.gz
+Author: Victor Vinci Fantucci
+Author-email: victor.v.fantucci@gmail.com
+License: GPLv3
+Project-URL: Bug Tracker, https://github.com/VictorFantucci/r4ven_utils_dev/issues
+Keywords: r4ven_utils,utils,logs
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Documentation
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
   <img src="imgs/r4ven_logo.png"><br>
 </div>
 
 -----------------
 
 # r4ven: The companion that holds your grab-bag of utility functions and objects
@@ -13,38 +32,29 @@
 ## What is it?
 
 **r4ven_utils** is all of those of utilities you keep reimplementing across your Python projects, that all got together and decided to live in harmony.
 
 ## Main Features
 Here are some of the utilities that r4ven keep under it's wings:
 
-  - [**log4me**][log-4-me] - Creation of a logger object specific to the function in which it's called.
+  - [**log4me**][log-4-me] - convenient way to implement logging in Python applications, ensuring that logs are organized and execution times are recorded accurately.
 
    [log-4-me]: r4ven_utils/log4me.py
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/VictorFantucci/r4ven_utils_dev
 
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/r4ven_utils).
 ```sh
 # or PyPI
 pip install r4ven-utils
 ```
 
-## Dependencies
-- [**os**][os-module] - This module provides a portable way of using operating system dependent functionality.
-- [**sys**][sys-module] - This module provides access to some variables used or maintained by the interpreter and to functions that interact strongly with the interpreter.
-- [**logging**][logging-module]- This module defines functions and classes which implement a flexible event logging system for applications and libraries.
-
-[os-module]: https://docs.python.org/3/library/os.html
-[sys-module]: https://docs.python.org/3/library/sys.html
-[logging-module]: https://docs.python.org/3/library/logging.htmlhttps://github.com/stub42/pytz
-
 ## License
 [GPLv3](LICENSE)
 
 ## Documentation
 All my scripts have very detailed docstrings and comments that make their use intuitive and simple. As the project grows and takes shape I plan to write a  proper documentation for it.
 
 ## Background
```

### Comparing `r4ven_utils-0.0.4/r4ven_utils/exceptions.py` & `r4ven_utils-0.0.5/r4ven_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `r4ven_utils-0.0.4/setup.py` & `r4ven_utils-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # Package Information:
     name='r4ven_utils',
     packages=['r4ven_utils'], # Should match the package folder.
-    version='0.0.4',
+    version='0.0.5',
     license='GPLv3',
 
     # Description Information:
     description='The companion that holds your grab-bag of utility functions and objects',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
@@ -39,9 +39,9 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Documentation',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
     ],
 
-    download_url="https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.4.tar.gz",
+    download_url="https://github.com/VictorFantucci/r4ven_utils_dev/archive/refs/tag/0.0.5.tar.gz",
 )
```

### Comparing `r4ven_utils-0.0.4/tests/test_log4me.py` & `r4ven_utils-0.0.5/tests/test_log4me.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 # Adding the parent directory to the sys.path.
 sys.path.append(parent_directory)
 
 # Import the main function [function_logger()] from function_logger.py
 from r4ven_utils.log4me import function_logger
 
-# Get the base name of the script file (excluding the '.py' extension) using os.path.basename
-# and remove the '.py' suffix from the obtained base name.
-script_name = os.path.basename(__file__).removesuffix(".py")
-
 # Import logging module to get the logging.levels constants.
 import logging
 
 def get_logging_levels(file_level: int) -> list:
     """
     Get the list of logging levels that are greater or equal than file_level
     parameter of the function_logger() function.
@@ -56,31 +52,30 @@
 
     Args:
         function_name (str): The name of the function that's calling the function
         function_logger.
     """
     logs_directory = os.getcwd()
     logs_directory = os.path.join(logs_directory, "logs")
-    function_log_path = logs_directory + "/log4me/{}.log".format(function_name)
+    function_log_path = os.path.join(logs_directory, "logs", f"log4me/{function_name}.log")
 
     # Get file object reference for the file.
     with open (file = function_log_path, mode = "r") as file:
         # Read the content of the file to string.
         file_to_be_inspected = file.read()
 
         logging_levels = get_logging_levels(file_level)
 
         if all(logging_level in file_to_be_inspected for logging_level in logging_levels):
-            print("For {}: ".format(function_name))
+            print(f"For {function_name}: ")
             print("All logging levels with a priority greater or equal" +\
-                  " {} are present in the {}.log file. \n".format(file_level, function_name))
+                  f" {file_level} are present in the {function_name}.log file. \n")
         else:
             sys.exit()
 
-
 def f1() -> None:
     """
     Function that test a specific case of the function_logger(), from src.function_logger.
 
     Case 01:
 
         Args:
@@ -91,15 +86,15 @@
 
             > console_level (str, optional): Logging level that will be displayed
             at the console.
                 > console_level = None;
                 The function shouldn't write any message to the console, because there isn't any
                 logging level assigned to the console_level variable.
     """
-    f1_logger = function_logger(script_name = script_name, file_level = logging.DEBUG)
+    f1_logger = function_logger(file_level = logging.DEBUG)
     f1_logger.debug("f1 Debug message")
     f1_logger.info("f1 Information message")
     f1_logger.warning("f1 Warning message")
     f1_logger.error("f1 Error message")
     f1_logger.critical("f1 Critical message")
 
 def f2() -> None:
@@ -116,16 +111,15 @@
 
             > console_level (str, optional): Logging level that will be displayed
             at the console.
                 > console_level = None;
                 The function should write all logging levels with priority equal or above INFO
                 to the console.
     """
-    f2_logger = function_logger(script_name = script_name,
-                                file_mode = "a",
+    f2_logger = function_logger(file_mode = "a",
                                 file_level = logging.WARNING,
                                 console_level = logging.INFO)
     f2_logger.debug("f2 Debug message")
     f2_logger.info("f2 Information message")
     f2_logger.warning("f2 Warning message")
     f2_logger.error("f2 Error message")
     f2_logger.critical("f2 Critical message")
```

