# Comparing `tmp/nstudypy-0.0.3.tar.gz` & `tmp/nstudypy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nstudypy-0.0.3.tar", last modified: Thu Apr 25 03:22:08 2024, max compression
+gzip compressed data, was "nstudypy-0.0.4.tar", last modified: Thu Apr 25 06:17:53 2024, max compression
```

## Comparing `nstudypy-0.0.3.tar` & `nstudypy-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:08.392665 nstudypy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 03:21:57.000000 nstudypy-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 03:22:08.392665 nstudypy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-25 03:21:57.000000 nstudypy-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 03:21:57.000000 nstudypy-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:57.000000 nstudypy-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:22:08.392665 nstudypy-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:08.392665 nstudypy-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:08.392665 nstudypy-0.0.3/src/NStudyPy/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-25 03:21:57.000000 nstudypy-0.0.3/src/NStudyPy/PyTools.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 03:21:57.000000 nstudypy-0.0.3/src/NStudyPy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:08.392665 nstudypy-0.0.3/src/NStudyPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 03:22:08.000000 nstudypy-0.0.3/src/NStudyPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 03:22:08.000000 nstudypy-0.0.3/src/NStudyPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:22:08.000000 nstudypy-0.0.3/src/NStudyPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 03:22:08.000000 nstudypy-0.0.3/src/NStudyPy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:53.515572 nstudypy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 06:17:40.000000 nstudypy-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 06:17:53.515572 nstudypy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-25 06:17:40.000000 nstudypy-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-25 06:17:40.000000 nstudypy-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 06:17:40.000000 nstudypy-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:17:53.515572 nstudypy-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:53.515572 nstudypy-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:53.515572 nstudypy-0.0.4/src/NStudyPy/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 06:17:40.000000 nstudypy-0.0.4/src/NStudyPy/PyShape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-25 06:17:40.000000 nstudypy-0.0.4/src/NStudyPy/PyString.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-25 06:17:40.000000 nstudypy-0.0.4/src/NStudyPy/PyTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 06:17:40.000000 nstudypy-0.0.4/src/NStudyPy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:53.515572 nstudypy-0.0.4/src/NStudyPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 06:17:53.000000 nstudypy-0.0.4/src/NStudyPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-25 06:17:53.000000 nstudypy-0.0.4/src/NStudyPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:17:53.000000 nstudypy-0.0.4/src/NStudyPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 06:17:53.000000 nstudypy-0.0.4/src/NStudyPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 06:17:53.000000 nstudypy-0.0.4/src/NStudyPy.egg-info/top_level.txt
```

### Comparing `nstudypy-0.0.3/LICENSE` & `nstudypy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nstudypy-0.0.3/PKG-INFO` & `nstudypy-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 Metadata-Version: 2.1
 Name: NStudyPy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A NStudyPy useful tools
 Author-email: Jack Li <lizhq08@gmail.com>
+Maintainer: Jack Li contributors
 Project-URL: Homepage, https://nstudy.org
+Project-URL: Documentation, https://hub.nstudy.org
 Project-URL: Bug Tracker, https://github.com/lizhq/NStudyPy/issues
-Classifier: Programming Language :: Python :: 3
+Keywords: NStudyPy,tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: shapely~=2.0.4
 
 # NStudyPy 
 NStudyPy 工具包
 
 
 ## 使用方法
 ```bash
 pip install -U NStudyPy -i https://pypi.org/simple
 ```
 
 ## 版本更新历史
 
-## version 0.0.1
-- 初始化项目
+## version 0.0.4
+- Python 升级到 3.9+
+- 添加 `PyShape` `PyString` 工具
+
+## version 0.0.3
+- 更改包名
 
 ## version 0.0.2
 - 添加一些方法 `from NStudyPy import PyTools`
 
-## version 0.0.3
-- 更改包名
+## version 0.0.1
+- 初始化项目
```

### Comparing `nstudypy-0.0.3/src/NStudyPy/PyTools.py` & `nstudypy-0.0.4/src/NStudyPy/PyTools.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
     初始化项目测试
     :return:
     """
     return "hello world!"
 
 
-def getEnv(key: str, default=None, value_type=None):
+def get_env(key: str, default=None, value_type=None):
     """
         Returns the value from the key.
         check environment variables
     """
     value = default
 
     if key in environ:
@@ -35,15 +35,15 @@
 
     if value_type == bool:
         return value == "True"
 
     return value_type(value)
 
 
-def getHostIp() -> str:
+def get_host_ip() -> str:
     """
         Returns the host ip.
     """
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     s.connect(('114.114.114.114', 80))
     return s.getsockname()[0]
```

### Comparing `nstudypy-0.0.3/src/NStudyPy.egg-info/PKG-INFO` & `nstudypy-0.0.4/src/NStudyPy.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 Metadata-Version: 2.1
 Name: NStudyPy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A NStudyPy useful tools
 Author-email: Jack Li <lizhq08@gmail.com>
+Maintainer: Jack Li contributors
 Project-URL: Homepage, https://nstudy.org
+Project-URL: Documentation, https://hub.nstudy.org
 Project-URL: Bug Tracker, https://github.com/lizhq/NStudyPy/issues
-Classifier: Programming Language :: Python :: 3
+Keywords: NStudyPy,tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: shapely~=2.0.4
 
 # NStudyPy 
 NStudyPy 工具包
 
 
 ## 使用方法
 ```bash
 pip install -U NStudyPy -i https://pypi.org/simple
 ```
 
 ## 版本更新历史
 
-## version 0.0.1
-- 初始化项目
+## version 0.0.4
+- Python 升级到 3.9+
+- 添加 `PyShape` `PyString` 工具
+
+## version 0.0.3
+- 更改包名
 
 ## version 0.0.2
 - 添加一些方法 `from NStudyPy import PyTools`
 
-## version 0.0.3
-- 更改包名
+## version 0.0.1
+- 初始化项目
```

