# Comparing `tmp/nonebot_plugin_userinfo-0.2.2.tar.gz` & `tmp/nonebot_plugin_userinfo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_userinfo-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_userinfo-0.2.3.tar", max compression
```

## Comparing `nonebot_plugin_userinfo-0.2.2.tar` & `nonebot_plugin_userinfo-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1063 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/LICENSE
--rw-r--r--   0        0        0     3916 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/README.md
--rw-r--r--   0        0        0      855 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/__init__.py
--rw-r--r--   0        0        0      351 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/__init__.py
--rw-r--r--   0        0        0      690 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/console.py
--rw-r--r--   0        0        0     1547 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/discord.py
--rw-r--r--   0        0        0     2862 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/dodo.py
--rw-r--r--   0        0        0     2062 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/feishu.py
--rw-r--r--   0        0        0     1887 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/kaiheila.py
--rw-r--r--   0        0        0     2687 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/onebot_v11.py
--rw-r--r--   0        0        0     4709 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/onebot_v12.py
--rw-r--r--   0        0        0     2103 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/qq.py
--rw-r--r--   0        0        0     3247 2024-03-01 02:26:40.555765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/red.py
--rw-r--r--   0        0        0     1376 2024-03-01 02:26:40.559765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/satori.py
--rw-r--r--   0        0        0     3348 2024-03-01 02:26:40.559765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/telegram.py
--rw-r--r--   0        0        0       40 2024-03-01 02:26:40.559765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/exception.py
--rw-r--r--   0        0        0     2405 2024-03-01 02:26:40.559765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/getter.py
--rw-r--r--   0        0        0     2782 2024-03-01 02:26:40.559765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/image_source.py
--rw-r--r--   0        0        0      454 2024-03-01 02:26:40.559765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/user_info.py
--rw-r--r--   0        0        0      565 2024-03-01 02:26:40.559765 nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/utils.py
--rw-r--r--   0        0        0     1851 2024-03-01 02:26:40.559765 nonebot_plugin_userinfo-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 nonebot_plugin_userinfo-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3916 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/README.md
+-rw-r--r--   0        0        0      855 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/__init__.py
+-rw-r--r--   0        0        0      351 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/__init__.py
+-rw-r--r--   0        0        0      690 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/console.py
+-rw-r--r--   0        0        0     1547 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/discord.py
+-rw-r--r--   0        0        0     2862 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/dodo.py
+-rw-r--r--   0        0        0     2062 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/feishu.py
+-rw-r--r--   0        0        0     1887 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/kaiheila.py
+-rw-r--r--   0        0        0     2706 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     4709 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     2103 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/qq.py
+-rw-r--r--   0        0        0     3247 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/red.py
+-rw-r--r--   0        0        0     1880 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/satori.py
+-rw-r--r--   0        0        0     3348 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/telegram.py
+-rw-r--r--   0        0        0       40 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/exception.py
+-rw-r--r--   0        0        0     2405 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/getter.py
+-rw-r--r--   0        0        0     2782 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/image_source.py
+-rw-r--r--   0        0        0      454 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/user_info.py
+-rw-r--r--   0        0        0      660 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/utils.py
+-rw-r--r--   0        0        0     1803 2024-03-19 10:39:42.171471 nonebot_plugin_userinfo-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 nonebot_plugin_userinfo-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_userinfo-0.2.2/LICENSE` & `nonebot_plugin_userinfo-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/README.md` & `nonebot_plugin_userinfo-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/__init__.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/console.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/discord.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/discord.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/dodo.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/dodo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/feishu.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/feishu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/kaiheila.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/onebot_v11.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/onebot_v11.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from nonebot.exception import ActionFailed
 from nonebot.log import logger
 
 from ..getter import UserInfoGetter, register_user_info_getter
 from ..image_source import QQAvatar
 from ..user_info import UserGender, UserInfo
+from ..utils import check_qq_number
 
 try:
     from nonebot.adapters.onebot.v11 import (
         Bot,
         Event,
         GroupAdminNoticeEvent,
         GroupBanNoticeEvent,
@@ -17,14 +18,23 @@
         GroupIncreaseNoticeEvent,
         GroupMessageEvent,
         GroupRecallNoticeEvent,
         GroupRequestEvent,
         GroupUploadNoticeEvent,
     )
 
+    def _sex_to_gender(sex: Optional[str]) -> UserGender:
+        return (
+            UserGender.male
+            if sex == "male"
+            else UserGender.female
+            if sex == "female"
+            else UserGender.unknown
+        )
+
     @register_user_info_getter(Bot, Event)
     class Getter(UserInfoGetter[Bot, Event]):
         async def _get_info(self, user_id: str) -> Optional[UserInfo]:
             info = None
 
             if isinstance(
                 self.event,
@@ -51,30 +61,23 @@
                     info = await self.bot.get_stranger_info(user_id=int(user_id))
                 except ActionFailed as e:
                     logger.warning(f"Error calling get_stranger_info failed: {e}")
 
             if info:
                 qq = info["user_id"]
                 sex = info.get("sex")
-                user_gender = (
-                    UserGender.male
-                    if sex == "male"
-                    else UserGender.female
-                    if sex == "female"
-                    else UserGender.unknown
-                )
                 return UserInfo(
                     user_id=str(qq),
                     user_name=info.get("nickname", ""),
                     user_displayname=info.get("card"),
                     user_avatar=QQAvatar(qq=qq),
-                    user_gender=user_gender,
+                    user_gender=_sex_to_gender(sex),
                 )
 
-            if user_id.isdigit() and 5 <= len(user_id) <= 11:
+            if check_qq_number(user_id):
                 return UserInfo(
                     user_id=user_id,
                     user_name="",
                     user_avatar=QQAvatar(qq=int(user_id)),
                 )
 
 except ImportError:
```

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/onebot_v12.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/qq.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/qq.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/red.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/red.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/adapters/telegram.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/getter.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/getter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/image_source.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/image_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.2.2/nonebot_plugin_userinfo/utils.py` & `nonebot_plugin_userinfo-0.2.3/nonebot_plugin_userinfo/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import re
 
 import httpx
 from nonebot.log import logger
 
 from .exception import NetworkError
 
 
@@ -13,7 +14,11 @@
                 resp = await client.get(url, timeout=10)
                 resp.raise_for_status()
                 return resp.content
             except Exception as e:
                 logger.warning(f"Error downloading {url}, retry {i}/3: {e}")
                 await asyncio.sleep(3)
     raise NetworkError(f"{url} 下载失败！")
+
+
+def check_qq_number(qq: str) -> bool:
+    return bool(re.match(r"^\d{5,11}$", qq))
```

### Comparing `nonebot_plugin_userinfo-0.2.2/pyproject.toml` & `nonebot_plugin_userinfo-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_userinfo"
-version = "0.2.2"
+version = "0.2.3"
 description = "Nonebot2 用户信息获取插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-userinfo"
 repository = "https://github.com/noneplugin/nonebot-plugin-userinfo"
 
@@ -27,15 +27,15 @@
 [tool.poetry.group.adapters]
 optional = true
 
 [tool.poetry.group.adapters.dependencies]
 nonebot-adapter-onebot = "^2.4.0"
 nonebot-adapter-console = "^0.5.0"
 nonebot-adapter-kaiheila = "^0.3.1"
-nonebot-adapter-telegram = { git = "https://github.com/nonebot/adapter-telegram.git" }
+nonebot-adapter-telegram = "^0.1.0b17"
 nonebot-adapter-feishu = "^2.4.0"
 nonebot-adapter-red = "^0.9.0"
 nonebot-adapter-discord = "^0.1.4"
 nonebot-adapter-dodo = "^0.2.0"
 nonebot-adapter-satori = "^0.9.3"
 nonebot-adapter-qq = "^1.4.1"
```

### Comparing `nonebot_plugin_userinfo-0.2.2/PKG-INFO` & `nonebot_plugin_userinfo-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_userinfo
-Version: 0.2.2
+Version: 0.2.3
 Summary: Nonebot2 用户信息获取插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-userinfo
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_userinfo Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_userinfo Version: 0.2.3 Summary:
 Nonebot2 ç¨æ·ä¿¡æ¯è·åæä»¶ Home-page: https://github.com/noneplugin/
 nonebot-plugin-userinfo License: MIT Author: meetwq Author-email:
 meetwq@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

