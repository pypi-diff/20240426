# Comparing `tmp/nonebot_plugin_sticker_saver-0.1.0.tar.gz` & `tmp/nonebot_plugin_sticker_saver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sticker_saver-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_sticker_saver-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_sticker_saver-0.1.0.tar` & `nonebot_plugin_sticker_saver-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1085 2024-04-26 12:55:23.804448 nonebot_plugin_sticker_saver-0.1.0/LICENSE
--rw-r--r--   0        0        0     2177 2024-04-26 13:21:30.188146 nonebot_plugin_sticker_saver-0.1.0/nonebot_plugin_sticker_saver/__init__.py
--rw-r--r--   0        0        0      757 2024-04-26 13:27:11.449851 nonebot_plugin_sticker_saver-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2527 2024-04-26 13:11:20.843562 nonebot_plugin_sticker_saver-0.1.0/README.md
--rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 nonebot_plugin_sticker_saver-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-26 13:36:16.367526 nonebot_plugin_sticker_saver-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2438 2024-04-26 13:36:16.367526 nonebot_plugin_sticker_saver-0.1.2/README.md
+-rw-r--r--   0        0        0     2137 2024-04-26 13:36:16.367526 nonebot_plugin_sticker_saver-0.1.2/nonebot_plugin_sticker_saver/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-26 13:36:16.371526 nonebot_plugin_sticker_saver-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 nonebot_plugin_sticker_saver-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_sticker_saver-0.1.0/LICENSE` & `nonebot_plugin_sticker_saver-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Colanns
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Colanns
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nonebot_plugin_sticker_saver-0.1.0/nonebot_plugin_sticker_saver/__init__.py` & `nonebot_plugin_sticker_saver-0.1.2/nonebot_plugin_sticker_saver/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from nonebot.plugin import on_command, PluginMetadata
-from nonebot import on_message, logger
-from nonebot.adapters.onebot.v11 import Bot, Message, MessageEvent, MessageSegment
-from httpx import AsyncClient
-
-__plugin_meta__ = PluginMetadata(
-    name="表情包保存器",
-    description="一款很简单的，用于保存已经不提供保存选项的 QQ 表情包的 Nonebot 插件",
-    usage="以 .save 命令回复表情包即可.\n机器人回复的静态表情可以直接保存，动态表情可以通过短链接保存。",
-    type="application",
-    homepage="https://github.com/colasama/nonebot-plugin-sticker-saver",
-    supported_adapters={"~onebot.v11"}
-)
-
-face_extractor = on_command('save', aliases={'保存图片', '保存表情', '保存'}, priority=10, block=True)
-
-@face_extractor.handle()
-async def handle_face_extraction(bot: Bot, event: MessageEvent):
-    if event.reply:
-        # 获取被回复的消息内容
-        original_message = event.reply.message
-        # 提取表情包并发送回去，静态表情包可以直接被保存
-        for seg in original_message:
-            logger.debug("seg: " + seg + " type: " + str(seg.type))
-            if seg.type == "image":
-                content = MessageSegment.text("表情：") + MessageSegment.image(seg.data["url"], type_=0)
-                async with AsyncClient() as client:
-                    # 用于 .gif 格式的表情包保存，加上一层短链接防止可能的检测，可以修改不同的 API
-                    url = "https://t.apii.cn/?url=" + str(seg.data["url"])
-                    try:
-                        req = await client.get(url=url)
-                        result = req.json()
-                        data = result.get("url")
-                    except Exception as e:
-                        await bot.send(event, "获取短链接失败")
-                await bot.send(event, content + "原始链接：" + data)
-                return
-        await bot.send(event, "未在回复内容中检测到表情...")
-    # 如果没有回复消息
-    else:
+from nonebot.plugin import on_command, PluginMetadata
+from nonebot import on_message, logger
+from nonebot.adapters.onebot.v11 import Bot, Message, MessageEvent, MessageSegment
+from httpx import AsyncClient
+
+__plugin_meta__ = PluginMetadata(
+    name="表情包保存器",
+    description="一款很简单的，用于保存已经不提供保存选项的 QQ 表情包的 Nonebot 插件",
+    usage="以 .save 命令回复表情包即可.\n机器人回复的静态表情可以直接保存，动态表情可以通过短链接保存。",
+    type="application",
+    homepage="https://github.com/colasama/nonebot-plugin-sticker-saver",
+    supported_adapters={"~onebot.v11"}
+)
+
+face_extractor = on_command('save', aliases={'保存图片', '保存表情', '保存'}, priority=10, block=True)
+
+@face_extractor.handle()
+async def handle_face_extraction(bot: Bot, event: MessageEvent):
+    if event.reply:
+        # 获取被回复的消息内容
+        original_message = event.reply.message
+        # 提取表情包并发送回去，静态表情包可以直接被保存
+        for seg in original_message:
+            logger.debug("seg: " + seg + " type: " + str(seg.type))
+            if seg.type == "image":
+                content = MessageSegment.text("表情：") + MessageSegment.image(seg.data["url"], type_=0)
+                async with AsyncClient() as client:
+                    # 用于 .gif 格式的表情包保存，加上一层短链接防止可能的检测，可以修改不同的 API
+                    url = "https://t.apii.cn/?url=" + str(seg.data["url"])
+                    try:
+                        req = await client.get(url=url)
+                        result = req.json()
+                        data = result.get("url")
+                    except Exception as e:
+                        await bot.send(event, "获取短链接失败")
+                await bot.send(event, content + "原始链接：" + data)
+                return
+        await bot.send(event, "未在回复内容中检测到表情...")
+    # 如果没有回复消息
+    else:
         await bot.send(event, "只有回复表情才可以用捏")
```

### Comparing `nonebot_plugin_sticker_saver-0.1.0/pyproject.toml` & `nonebot_plugin_sticker_saver-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-[tool.poetry]
-name = "nonebot-plugin-sticker-saver"
-version = "0.1.0"
-description = "A very simple Nonebot plugin for saving QQ emoticons that no longer have a save option."
-authors = ["Colanns <mycolands@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://github.com/colasama/nonebot-plugin-sticker-saver"
-repository = "https://github.com/colasama/nonebot-plugin-sticker-saver"
-documentation = "https://github.com/colasama/nonebot-plugin-sticker-saver"
-keywords = ["nonebot2", "表情包", "sticker"]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-nonebot2 = "^2.0.0-beta.4"
-httpx = ">=0.20.0"
-nonebot-adapter-onebot = "^2.0.0-beta.1"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonebot-plugin-sticker-saver"
+version = "0.1.2"
+description = "A very simple Nonebot plugin for saving QQ emoticons that no longer have a save option."
+authors = ["Colanns <mycolands@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/colasama/nonebot-plugin-sticker-saver"
+repository = "https://github.com/colasama/nonebot-plugin-sticker-saver"
+documentation = "https://github.com/colasama/nonebot-plugin-sticker-saver"
+keywords = ["nonebot2", "表情包", "sticker"]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+nonebot2 = "^2.0.0-beta.4"
+httpx = ">=0.20.0"
+nonebot-adapter-onebot = "^2.0.0-beta.1"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_sticker_saver-0.1.0/PKG-INFO` & `nonebot_plugin_sticker_saver-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sticker-saver
-Version: 0.1.0
+Version: 0.1.2
 Summary: A very simple Nonebot plugin for saving QQ emoticons that no longer have a save option.
 Home-page: https://github.com/colasama/nonebot-plugin-sticker-saver
 License: MIT
 Keywords: nonebot2,表情包,sticker
 Author: Colanns
 Author-email: mycolands@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -19,17 +19,17 @@
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0-beta.4,<3.0.0)
 Project-URL: Documentation, https://github.com/colasama/nonebot-plugin-sticker-saver
 Project-URL: Repository, https://github.com/colasama/nonebot-plugin-sticker-saver
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-sticker-saver/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-sticker-saver/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-sticker-saver
 
 _✨ 一款很简单的，用于保存已经不提供保存选项的 QQ 表情包的 Nonebot 插件 ✨_
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sticker-saver Version: 0.1.0
+Metadata-Version: 2.1 Name: nonebot-plugin-sticker-saver Version: 0.1.2
 Summary: A very simple Nonebot plugin for saving QQ emoticons that no longer
 have a save option. Home-page: https://github.com/colasama/nonebot-plugin-
 sticker-saver License: MIT Keywords: nonebot2,è¡¨æå,sticker Author: Colanns
 Author-email: mycolands@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

