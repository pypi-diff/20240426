# Comparing `tmp/pytgpt_bot-0.0.7.tar.gz` & `tmp/pytgpt_bot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.0.7.tar", last modified: Fri Apr 26 01:17:19 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.0.8.tar", last modified: Fri Apr 26 02:28:56 2024, max compression
```

## Comparing `pytgpt_bot-0.0.7.tar` & `pytgpt_bot-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:17:19.544592 pytgpt_bot-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 01:17:19.544592 pytgpt_bot-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:17:19.540592 pytgpt_bot-0.0.7/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    18621 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/pytgpt_bot/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:17:19.540592 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 01:17:19.000000 pytgpt_bot-0.0.7/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 01:17:19.544592 pytgpt_bot-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-26 01:17:04.000000 pytgpt_bot-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:28:56.848400 pytgpt_bot-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 02:28:56.848400 pytgpt_bot-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:28:56.848400 pytgpt_bot-0.0.8/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/pytgpt_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:28:56.848400 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 02:28:56.000000 pytgpt_bot-0.0.8/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 02:28:56.848400 pytgpt_bot-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-26 02:28:41.000000 pytgpt_bot-0.0.8/setup.py
```

### Comparing `pytgpt_bot-0.0.7/LICENSE` & `pytgpt_bot-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.7/PKG-INFO` & `pytgpt_bot-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.7
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.7 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.8 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
```

### Comparing `pytgpt_bot-0.0.7/README.md` & `pytgpt_bot-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.7/pytgpt_bot/cli.py` & `pytgpt_bot-0.0.8/pytgpt_bot/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import click
 from pytgpt.utils import Audio
 from pytgpt_bot import __version__
 from os import environ
 import logging
+from pytgpt_bot.utils import provider_keys
+from pytgpt_bot.utils import bot_dir
+from shutil import rmtree
 
 context_settings: dict = dict(auto_envvar_prefix="PYTGPT-BOT")
 
 # bot_token, max_tokens, timeout, voice, loglevel, logfile, admin_id
 
 
 @click.group()
@@ -56,14 +59,21 @@
     "--logfile",
     type=click.Path(),
     help="Path to file for loggging",
 )
 @click.option(
     "-a", "--admin-id", type=click.INT, help="Admin's Telegram user ID", default=12345
 )
+@click.option(
+    "-p",
+    "--provider",
+    type=click.Choice(provider_keys),
+    help="Default tgpt-based llm provider",
+    default="auto",
+)
 @click.help_option("-h", "--help")
 def run(**kwargs):
     """Start the bot"""
     click.secho("[*] Firing up bot - [pytgpt-bot]", fg="cyan")
 
     modded_kwargs: dict = {}
 
@@ -76,15 +86,29 @@
 
         bot.infinity_polling(timeout=kwargs.get("timeout"), skip_pending=True)
     except Exception as e:
         logging.error(e.args[1] if e.args and len(e.args) > 1 else str(e))
         click.secho("[^] Quitting", fg="yellow")
 
 
+@click.command()
+@click.option("-y", "--yes", is_flag=True, help="Okay to confirmations")
+@click.help_option("-h", "--help")
+def clear(yes: bool):
+    """Clear bot's storage directory"""
+    if not yes and not click.confirm(
+        f"Are you sure to clear path '{bot_dir.as_posix()}'."
+    ):
+        return
+    rmtree(bot_dir, ignore_errors=True)
+    click.secho("[*] Path cleared successfully!", fg="yellow")
+
+
 def entry():
     """Cli entrypoint"""
     bot.add_command(run)
+    bot.add_command(clear)
     bot()
 
 
 if __name__ == "__main__":
-    run()
+    entry()
```

### Comparing `pytgpt_bot-0.0.7/pytgpt_bot/db.py` & `pytgpt_bot-0.0.8/pytgpt_bot/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sqlite3
+from .utils import path_to_db
 from .config import admin_id
-from .config import path_to_db
+from .config import provider
+from .config import voice
 from functools import wraps
 import logging
 import typing
 from pytgpt.utils import Conversation
-from pytgpt.utils import Audio
 
 
 def exception_handler(func):
 
     @wraps(func)
     def decorator(*args, **kwargs):
         try:
@@ -30,16 +31,16 @@
         conn = sqlite3.connect(path_to_db)
         conn.execute(
             f"""
         CREATE TABLE IF NOT EXISTS Chat(
             Id INTEGER PRIMARY KEY,
             Intro TEXT DEFAULT "{Conversation.intro}",
             History TEXT DEFAULT "" NOT NULL,
-            Voice TEXT DEFAULT "Brian" NOT NULL,
-            Provider TEXT DEFAULT "auto" NOT NULL
+            Voice TEXT DEFAULT "{voice}" NOT NULL,
+            Provider TEXT DEFAULT "{provider}" NOT NULL
             );
         """
         )
         conn.commit()
 
     @staticmethod
     @exception_handler
```

### Comparing `pytgpt_bot-0.0.7/pytgpt_bot/main.py` & `pytgpt_bot-0.0.8/pytgpt_bot/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,52 +2,28 @@
 import pytgpt.imager as image_generator
 from pytgpt.utils import Audio as audio_generator
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
 from functools import wraps
 import logging
 
-from pytgpt.opengpt import OPENGPT
-from pytgpt.koboldai import KOBOLDAI
-from pytgpt.phind import PHIND
-from pytgpt.llama2 import LLAMA2
-from pytgpt.blackboxai import BLACKBOXAI
-from pytgpt.perplexity import PERPLEXITY
-from pytgpt.yepchat import YEPCHAT
-from pytgpt.auto import AUTO
-
 from .config import (
     bot_token,
     max_tokens,
     timeout,
     loglevel,
     logfile,
     admin_id,
     provider,
 )
 from .db import User, Chat
-from . import __version__
-
-provider_map: dict[str, object] = {
-    "opengpt": OPENGPT,
-    "koboldai": KOBOLDAI,
-    "phind": PHIND,
-    "llama2": LLAMA2,
-    "blackboxai": BLACKBOXAI,
-    "perplexity": PERPLEXITY,
-    "yepchat": YEPCHAT,
-    "auto": AUTO,
-}
+from .utils import provider_keys
+from .utils import provider_map
 
 chosen_provider: str = provider_map.get(provider)
-provider_keys: list = list(provider_map.keys())
-
-assert (
-    chosen_provider
-), f"Provider '{provider}' is not one of {', '.join(provider_keys)}"
 
 log_params = dict(
     format="%(asctime)s : %(levelname)s - %(message)s",
     datefmt="%d-%b-%Y %H:%M:%S",
     level=loglevel,
 )
 
@@ -438,29 +414,29 @@
         f"Total Chats **{total_chats}**",
         reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["drop", "drop_chats"])
 @handler_formatter(admin=True)
-def total_chats_table(message: telebot.types.Message):
+def total_chats_table_and_logs(message: telebot.types.Message):
     """Drop chat table and create new"""
     if logfile:
         with open(logfile, "w") as fh:
             fh.write(
                 f"ADMIN CLEARED LOGS & DROPPED CHAT TABLE [{message.from_user.id}] - ({message.from_user.full_name})\n"
             )
     logging.warning(
         f"Dropping Chat table and reinitialize - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     Chat.query("DROP TABLE CHAT")
     Chat.initialize()
     return bot.reply_to(
         message,
-        f"Chat table dropped and new one created.",
+        f"Chat table and bot logs dropped and new one created.",
         reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["sql"])
 @handler_formatter(admin=True)
 def run_sql_statement(message: telebot.types.Message):
@@ -489,36 +465,14 @@
     if not logfile:
         return bot.reply_to(message, "Logfile not specified!")
     with open(logfile, encoding="utf-8") as fh:
         contents: str = fh.read()
     return send_long_text(message, contents, add_delete=True)
 
 
-@bot.message_handler(content_types=["chat"])
-@handler_formatter(text=True)
-def text_chat(message: telebot.types.Message):
-    """Text generation - provider of choice"""
-    user = User(message.from_user.id)
-    chat_record = user.record
-    conversation = Conversation(max_tokens=max_tokens)
-    conversation.chat_history = chat_record.get("history") or ""
-    conversation_prompt = conversation.gen_complete_prompt(
-        message.text, intro=chat_record.get("intro")
-    )
-    bot.send_chat_action(message.chat.id, "typing")
-    ai_response = text_generator.AUTO(is_conversation=False, timeout=timeout).chat(
-        conversation_prompt
-    )
-    conversation.update_chat_history(
-        prompt=message.text, response=ai_response, force=True
-    )
-    user.update_history(conversation.chat_history)
-    return send_long_text(message, ai_response)
-
-
 @bot.message_handler(content_types=["text"])
 @handler_formatter(text=True)
 def text_chat(message: telebot.types.Message):
     """Text generation"""
     user = User(message.from_user.id)
     chat_record = user.record
     conversation = Conversation(max_tokens=max_tokens)
```

### Comparing `pytgpt_bot-0.0.7/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.0.8/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.7
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.7 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.8 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
```

### Comparing `pytgpt_bot-0.0.7/setup.py` & `pytgpt_bot-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.0.7",
+    version="0.0.8",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Telegram bot for text generation, text-to-image and text-to-audio conversions.",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
```

