# Comparing `tmp/crawlipt-0.0.2.tar.gz` & `tmp/crawlipt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlipt-0.0.2.tar", last modified: Wed Apr 24 04:13:45 2024, max compression
+gzip compressed data, was "crawlipt-0.0.3.tar", last modified: Fri Apr 26 06:38:04 2024, max compression
```

## Comparing `crawlipt-0.0.2.tar` & `crawlipt-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:45.725271 crawlipt-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 04:13:39.000000 crawlipt-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 04:13:39.000000 crawlipt-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-24 04:13:45.725271 crawlipt-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-24 04:13:39.000000 crawlipt-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:45.721271 crawlipt-0.0.2/crawlipt/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:45.725271 crawlipt-0.0.2/crawlipt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/input.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/slide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/actions/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-24 04:13:39.000000 crawlipt-0.0.2/crawlipt/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:13:45.725271 crawlipt-0.0.2/crawlipt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-24 04:13:45.000000 crawlipt-0.0.2/crawlipt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 04:13:45.000000 crawlipt-0.0.2/crawlipt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:13:45.000000 crawlipt-0.0.2/crawlipt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 04:13:45.000000 crawlipt-0.0.2/crawlipt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 04:13:45.000000 crawlipt-0.0.2/crawlipt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:13:45.725271 crawlipt-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-24 04:13:39.000000 crawlipt-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:04.193247 crawlipt-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-26 06:37:55.000000 crawlipt-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 06:37:55.000000 crawlipt-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-26 06:38:04.193247 crawlipt-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-26 06:37:55.000000 crawlipt-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:04.189247 crawlipt-0.0.3/crawlipt/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:04.193247 crawlipt-0.0.3/crawlipt/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:04.193247 crawlipt-0.0.3/crawlipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-26 06:38:04.000000 crawlipt-0.0.3/crawlipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-26 06:38:04.000000 crawlipt-0.0.3/crawlipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:38:04.000000 crawlipt-0.0.3/crawlipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 06:38:04.000000 crawlipt-0.0.3/crawlipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 06:38:04.000000 crawlipt-0.0.3/crawlipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:38:04.193247 crawlipt-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-26 06:37:55.000000 crawlipt-0.0.3/setup.py
```

### Comparing `crawlipt-0.0.2/LICENSE` & `crawlipt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/PKG-INFO` & `crawlipt-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.2
+Version: 0.0.3
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.0.0
-Requires-Dist: ddddocr
-Requires-Dist: webdriver-manager
 
 
 <!-- markdownlint-disable MD033 MD041 -->
 <p align="center">
   <a href="https://github.com/WwwwwyDev/crawlipt"><img src="https://s2.loli.net/2024/04/19/1T7sZdrjbEfci8W.png" alt="crawlist" style="width:254px; height:208px" ></a>
 </p>
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.2 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.3 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python ::
+Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: selenium>=4.0.0 Requires-
-Dist: ddddocr Requires-Dist: webdriver-manager
+text/markdown License-File: LICENSE Requires-Dist: selenium>=4.0.0
                                   _[_c_r_a_w_l_i_s_t_]
                  # crawlipt The script for selenium in python
                          _[_p_y_p_i_][python]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 ## introduction You can use Crawlipt to driver the selenium by script in
 python.The script adopts JSON format for better cross language operations and
 physical storage. ## installing You can use pip or pip3 to install the
 crawlist\ `pip install crawlipt` or `pip3 install crawlipt` ## quickly start
```

### Comparing `crawlipt-0.0.2/README.md` & `crawlipt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/crawlipt/actions/click.py` & `crawlipt-0.0.3/crawlipt/actions/click.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/crawlipt/actions/get.py` & `crawlipt-0.0.3/crawlipt/actions/get.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/crawlipt/actions/input.py` & `crawlipt-0.0.3/crawlipt/actions/input.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/crawlipt/actions/redirect.py` & `crawlipt-0.0.3/crawlipt/actions/redirect.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/crawlipt/actions/select.py` & `crawlipt-0.0.3/crawlipt/actions/select.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/crawlipt/actions/slide.py` & `crawlipt-0.0.3/crawlipt/actions/slide.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/crawlipt/actions/switch.py` & `crawlipt-0.0.3/crawlipt/actions/switch.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/crawlipt/annotation.py` & `crawlipt-0.0.3/crawlipt/annotation.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/crawlipt/script.py` & `crawlipt-0.0.3/crawlipt/script.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,20 @@
 import random
 import time
 import json
 from inspect import signature
 from typing import Any
 from selenium.webdriver.remote.webdriver import WebDriver
-from webdriver_manager.chrome import ChromeDriverManager
-from selenium import webdriver as wd
-from selenium.webdriver.chrome.service import Service
 from crawlipt.annotation import check, ParamTypeError
 from crawlipt.action import Action
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
 
 
-def getDriver(is_headless=False):
-    option = wd.ChromeOptions()
-    arguments = [
-        "no-sandbox",
-        "--disable-extensions",
-        '--disable-gpu',
-        'User-Agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36"',
-        "window-size=1920x3000",
-        "start-maximized",
-        'cache-control="max-age=0"'
-        "disable-blink-features=AutomationControlled"
-    ]
-    for argument in arguments:
-        option.add_argument(argument)
-    if is_headless:
-        option.add_argument("--headless")
-    option.add_experimental_option('excludeSwitches', ['enable-automation'])
-    webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()), options=option)
-    webdriver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {
-        "source": """
-        Object.defineProperty(navigator, 'webdriver', {
-          get: () => false
-        })
-      """
-    })
-    return webdriver
-
-
 class ScriptError(Exception):
     def __init__(self, e: Exception, method: str, deep: int):
         self.e = e
         self.method = method
         self.deep = deep
 
     def __str__(self):
@@ -93,22 +62,18 @@
             self.script = json.loads(script)
         else:
             self.script = script
         Script.syntax_check(self.script)
         self.interval = interval
 
     @check
-    def process(self, webdriver: WebDriver = None) -> Any:
+    def process(self, webdriver: WebDriver) -> Any:
         """
         process the script
         """
-        is_use_default = False
-        if not webdriver:
-            is_use_default = True
-            webdriver = getDriver(is_headless=True)
         script = self.script
         pre_return = None
         while script:
             temp_args = {"driver": webdriver}
             method = script.get("method")
             for key, value in script.items():
                 if key.lower() not in Script.POP_KEY:
@@ -119,16 +84,14 @@
                         temp_args[key] = pre_return
             if "driver" in temp_args and "xpath" in temp_args:
                 WebDriverWait(temp_args["driver"], 10).until(
                     EC.presence_of_element_located((By.XPATH, temp_args["xpath"])))
             pre_return = Script.ACTIONS[method](**temp_args)
             script = script.get("next")
             time.sleep(random.uniform(self.interval / 2, self.interval))
-        if is_use_default:
-            webdriver.quit()
         return pre_return
 
     @staticmethod
     @check
     def syntax_check(script: dict | str) -> None:
         """
         Script syntax check
@@ -191,9 +154,15 @@
     @check
     def json2dict(scripts_json: str) -> dict:
         """
         generate the scripts(str of json) from dict
         """
         return json.loads(scripts_json)
 
+    @staticmethod
+    def add_action(func: callable) -> None:
+        if not callable(func):
+            raise ParamTypeError("func must be a callable")
+        Script.ACTIONS[func.__name__] = func
+
     def __call__(self, webdriver: WebDriver):
         return self.process(webdriver)
```

### Comparing `crawlipt-0.0.2/crawlipt.egg-info/PKG-INFO` & `crawlipt-0.0.3/crawlipt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.2
+Version: 0.0.3
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.0.0
-Requires-Dist: ddddocr
-Requires-Dist: webdriver-manager
 
 
 <!-- markdownlint-disable MD033 MD041 -->
 <p align="center">
   <a href="https://github.com/WwwwwyDev/crawlipt"><img src="https://s2.loli.net/2024/04/19/1T7sZdrjbEfci8W.png" alt="crawlist" style="width:254px; height:208px" ></a>
 </p>
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.2 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.3 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python ::
+Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: selenium>=4.0.0 Requires-
-Dist: ddddocr Requires-Dist: webdriver-manager
+text/markdown License-File: LICENSE Requires-Dist: selenium>=4.0.0
                                   _[_c_r_a_w_l_i_s_t_]
                  # crawlipt The script for selenium in python
                          _[_p_y_p_i_][python]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 ## introduction You can use Crawlipt to driver the selenium by script in
 python.The script adopts JSON format for better cross language operations and
 physical storage. ## installing You can use pip or pip3 to install the
 crawlist\ `pip install crawlipt` or `pip3 install crawlipt` ## quickly start
```

### Comparing `crawlipt-0.0.2/crawlipt.egg-info/SOURCES.txt` & `crawlipt-0.0.3/crawlipt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.2/setup.py` & `crawlipt-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # Package meta-data.
 NAME = 'crawlipt'
 DESCRIPTION = 'The script for selenium in python'
 URL = 'https://github.com/WwwwwyDev/crawlipt'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwwwwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    "selenium>=4.0.0", "ddddocr",  'webdriver-manager'
+    "selenium>=4.0.0"
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
@@ -116,15 +116,15 @@
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
```

