# Comparing `tmp/pytgpt_bot-0.0.8.tar.gz` & `tmp/pytgpt_bot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.0.8.tar", last modified: Fri Apr 26 02:28:56 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.0.9.tar", last modified: Fri Apr 26 03:06:32 2024, max compression
```

## Comparing `pytgpt_bot-0.0.8.tar` & `pytgpt_bot-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:28:56.848400 pytgpt_bot-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 02:28:56.848400 pytgpt_bot-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:28:56.848400 pytgpt_bot-0.0.8/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:28:56.848400 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 02:28:56.848400 pytgpt_bot-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:06:32.588867 pytgpt_bot-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 03:06:32.588867 pytgpt_bot-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:06:32.588867 pytgpt_bot-0.0.9/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17267 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/pytgpt_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:06:32.588867 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 03:06:32.000000 pytgpt_bot-0.0.9/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 03:06:32.588867 pytgpt_bot-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-26 03:06:15.000000 pytgpt_bot-0.0.9/setup.py
```

### Comparing `pytgpt_bot-0.0.8/LICENSE` & `pytgpt_bot-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.8/PKG-INFO` & `pytgpt_bot-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.8 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.9 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
```

### Comparing `pytgpt_bot-0.0.8/README.md` & `pytgpt_bot-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.8/pytgpt_bot/cli.py` & `pytgpt_bot-0.0.9/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.8/pytgpt_bot/config.py` & `pytgpt_bot-0.0.9/pytgpt_bot/config.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.8/pytgpt_bot/db.py` & `pytgpt_bot-0.0.9/pytgpt_bot/db.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.8/pytgpt_bot/main.py` & `pytgpt_bot-0.0.9/pytgpt_bot/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import telebot
 import pytgpt.imager as image_generator
 from pytgpt.utils import Audio as audio_generator
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
 from functools import wraps
 import logging
+import json
 
 from .config import (
     bot_token,
     max_tokens,
     timeout,
     loglevel,
     logfile,
@@ -306,20 +307,20 @@
 
 
 @bot.message_handler(commands=["settings"])
 @handler_formatter()
 def check_current_settings(message: telebot.types.Message):
     """Check current user settings"""
     user_record: dict = User(message.from_user.id).record
-    current_user_settings = f"""
-    **Chat Length** : `{len(user_record.get('history'))}`
-    **Speech Voice** : `{user_record.get('voice')}`
-    **Chat provider** : {user_record.get('provider')}
-    **Chat Intro** : `{user_record.get('intro')}`
-    """
+    current_user_settings = (
+        f"Chat Length : `{len(user_record.get('history'))}`\n"
+        f"Speech Voice : `{user_record.get('voice')}`\n"
+        f"Chat Provider : `{user_record.get('provider')}`\n"
+        f"Chat Intro : `{user_record.get('intro')}`"
+    )
     return bot.reply_to(
         message, current_user_settings, reply_markup=make_delete_markup(message)
     )
 
 
 @bot.message_handler(commands=["history"])
 @handler_formatter()
@@ -360,24 +361,27 @@
     )
 
 
 @bot.message_handler(commands=["audio", "aud"])
 @handler_formatter(text=True)
 def text_to_audio(message: telebot.types.Message):
     """Convert text to audio"""
+    voice = User(message.chat.id).chat_voice
     audio_chunk = audio_generator.text_to_audio(
         message=message.text,
-        voice=User(message.chat.id).chat_voice,
+        voice=voice,
         timeout=timeout,
     )
     return bot.send_audio(
         message.chat.id,
         audio=audio_chunk,
         caption=message.text,
         reply_markup=make_delete_markup(message),
+        performer=voice,
+        title="Text-to-Audio",
     )
 
 
 @bot.message_handler(commands=["reset"])
 @handler_formatter()
 def reset_chat(message: telebot.types.Message):
     """Reset current chat thread"""
```

### Comparing `pytgpt_bot-0.0.8/pytgpt_bot/utils.py` & `pytgpt_bot-0.0.9/pytgpt_bot/utils.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.8/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.0.9/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.8 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.9 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
```

### Comparing `pytgpt_bot-0.0.8/setup.py` & `pytgpt_bot-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.0.8",
+    version="0.0.9",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Telegram bot for text generation, text-to-image and text-to-audio conversions.",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
```

