# Comparing `tmp/nonebot-plugin-sayoroll-1.0.3.tar.gz` & `tmp/nonebot_plugin_sayoroll-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sayoroll-1.0.3.tar", last modified: Thu Apr 11 09:30:36 2024, max compression
+gzip compressed data, was "nonebot_plugin_sayoroll-1.0.4.tar", last modified: Fri Apr 26 03:07:12 2024, max compression
```

## Comparing `nonebot-plugin-sayoroll-1.0.3.tar` & `nonebot_plugin_sayoroll-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:30:36.769732 nonebot-plugin-sayoroll-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 09:30:33.000000 nonebot-plugin-sayoroll-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-11 09:30:36.769732 nonebot-plugin-sayoroll-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-11 09:30:33.000000 nonebot-plugin-sayoroll-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:30:36.769732 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll/
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-11 09:30:33.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:30:36.769732 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-11 09:30:36.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-11 09:30:36.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:30:36.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 09:30:36.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 09:30:36.000000 nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:30:36.769732 nonebot-plugin-sayoroll-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-11 09:30:33.000000 nonebot-plugin-sayoroll-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:07:12.342231 nonebot_plugin_sayoroll-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-26 03:07:08.000000 nonebot_plugin_sayoroll-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-26 03:07:12.342231 nonebot_plugin_sayoroll-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-26 03:07:08.000000 nonebot_plugin_sayoroll-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:07:12.342231 nonebot_plugin_sayoroll-1.0.4/nonebot_plugin_sayoroll/
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-26 03:07:08.000000 nonebot_plugin_sayoroll-1.0.4/nonebot_plugin_sayoroll/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:07:12.342231 nonebot_plugin_sayoroll-1.0.4/nonebot_plugin_sayoroll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-26 03:07:12.000000 nonebot_plugin_sayoroll-1.0.4/nonebot_plugin_sayoroll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-26 03:07:12.000000 nonebot_plugin_sayoroll-1.0.4/nonebot_plugin_sayoroll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 03:07:12.000000 nonebot_plugin_sayoroll-1.0.4/nonebot_plugin_sayoroll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 03:07:12.000000 nonebot_plugin_sayoroll-1.0.4/nonebot_plugin_sayoroll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 03:07:12.000000 nonebot_plugin_sayoroll-1.0.4/nonebot_plugin_sayoroll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 03:07:12.342231 nonebot_plugin_sayoroll-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-26 03:07:08.000000 nonebot_plugin_sayoroll-1.0.4/setup.py
```

### Comparing `nonebot-plugin-sayoroll-1.0.3/LICENSE` & `nonebot_plugin_sayoroll-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sayoroll-1.0.3/PKG-INFO` & `nonebot_plugin_sayoroll-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sayoroll
-Version: 1.0.3
+Version: 1.0.4
 Summary: 基于NoneBot的高仿以前小夜bot的roll功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 1.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 1.0.4 Summary:
 åºäºNoneBotçé«ä»¿ä»¥åå°å¤botçrollåè½ Home-page: https://
 github.com/mas-alone/nonebot-plugin-sayoroll Author: A M D Author-email:
 mas_alone@qq.com Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-
 adapter-onebot>=2.0.0b1 Requires-Dist: nonebot-plugin-alconna>=0.38.2
```

### Comparing `nonebot-plugin-sayoroll-1.0.3/README.md` & `nonebot_plugin_sayoroll-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll/__init__.py` & `nonebot_plugin_sayoroll-1.0.4/nonebot_plugin_sayoroll/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         args = normalize_str(args)
         args_without_punctuation = args.translate(str.maketrans('', '', string.punctuation))
         if len(args_without_punctuation.split(' ')) == 1:
             msg = '未匹配到参数！'
         else:
             options = [x for x in args.split(' ') if x.strip()]
             if len(options) > 1:
-                similarities = [difflib.SequenceMatcher(None, option1.lower(), option2.lower()).ratio() for option1 in options for option2 in options if option1 != option2]
+                similarities = [difflib.SequenceMatcher(None, option1.lower(), option2.lower()).ratio() for i, option1 in enumerate(options) for option2 in options[i+1:]]
                 if any(similarity > 0.8 for similarity in similarities):
                     msg = '总共就{}个参数..还这么相似..怎么roll都一样啊'.format(len(options))
                 else:
                     msg = '当然是{}咯'.format(random.choice(options))
             else:
                 msg = '未匹配到参数！'
     await UniMessage.text(msg).send(reply_to=True)
```

### Comparing `nonebot-plugin-sayoroll-1.0.3/nonebot_plugin_sayoroll.egg-info/PKG-INFO` & `nonebot_plugin_sayoroll-1.0.4/nonebot_plugin_sayoroll.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sayoroll
-Version: 1.0.3
+Version: 1.0.4
 Summary: 基于NoneBot的高仿以前小夜bot的roll功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 1.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 1.0.4 Summary:
 åºäºNoneBotçé«ä»¿ä»¥åå°å¤botçrollåè½ Home-page: https://
 github.com/mas-alone/nonebot-plugin-sayoroll Author: A M D Author-email:
 mas_alone@qq.com Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-
 adapter-onebot>=2.0.0b1 Requires-Dist: nonebot-plugin-alconna>=0.38.2
```

### Comparing `nonebot-plugin-sayoroll-1.0.3/setup.py` & `nonebot_plugin_sayoroll-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-sayoroll",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.0.3",  # 程序版本
+    version="1.0.4",  # 程序版本
     author="A M D",  # 项目作者
     author_email="mas_alone@qq.com",  # 作者邮件
     description="基于NoneBot的高仿以前小夜bot的roll功能",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/mas-alone/nonebot-plugin-sayoroll",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

