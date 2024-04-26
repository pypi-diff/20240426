# Comparing `tmp/aitelegrambot-0.5.0.tar.gz` & `tmp/aitelegrambot-0.5.1.tar.gz`

## Comparing `aitelegrambot-0.5.0.tar` & `aitelegrambot-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,33 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/.env.example
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/Makefile
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/Makefile.venv
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/docs/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/docs/commands.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/docs/setup.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/src/aitelegrambot/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/src/aitelegrambot/__main__.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/src/aitelegrambot/bot.py
--rw-r--r--   0        0        0     8256 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/src/aitelegrambot/commandhandlers.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/src/aitelegrambot/constants.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/.gitignore
--rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/LICENSE.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aitelegrambot-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/.env.example
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/Makefile
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/Makefile.venv
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/.env.example
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/.gitignore
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/CHANGELOG.md
+-rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/LICENSE.md
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/Makefile
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/Makefile.venv
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/pyproject.toml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/docs/README.md
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/docs/commands.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/docs/setup.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/src/aitelegrambot/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/src/aitelegrambot/__main__.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/src/aitelegrambot/bot.py
+-rw-r--r--   0        0        0     8256 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/src/aitelegrambot/commandhandlers.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/aitelegrambot/src/aitelegrambot/constants.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/docs/README.md
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/docs/commands.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/docs/setup.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/src/aitelegrambot/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/src/aitelegrambot/__main__.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/src/aitelegrambot/bot.py
+-rw-r--r--   0        0        0     8256 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/src/aitelegrambot/commandhandlers.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/src/aitelegrambot/constants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/.gitignore
+-rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.5.1/PKG-INFO
```

### Comparing `aitelegrambot-0.5.0/CHANGELOG.md` & `aitelegrambot-0.5.1/aitelegrambot/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.0/Makefile.venv` & `aitelegrambot-0.5.1/Makefile.venv`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.0/docs/commands.md` & `aitelegrambot-0.5.1/aitelegrambot/docs/commands.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.0/docs/setup.md` & `aitelegrambot-0.5.1/aitelegrambot/docs/setup.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.0/src/aitelegrambot/__main__.py` & `aitelegrambot-0.5.1/aitelegrambot/src/aitelegrambot/__main__.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.0/src/aitelegrambot/bot.py` & `aitelegrambot-0.5.1/aitelegrambot/src/aitelegrambot/bot.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.0/src/aitelegrambot/commandhandlers.py` & `aitelegrambot-0.5.1/aitelegrambot/src/aitelegrambot/commandhandlers.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.0/LICENSE.md` & `aitelegrambot-0.5.1/aitelegrambot/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.0/pyproject.toml` & `aitelegrambot-0.5.1/aitelegrambot/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.0/PKG-INFO` & `aitelegrambot-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.3
 Name: aitelegrambot
-Version: 0.5.0
+Version: 0.5.1
 Summary: aitelegrambot is a Telegram bot that uses the Ollama backend to run the LLM rationalAI (by default).
 Author-email: tusharhero <tusharhero@sdf.org>, alokosx <alokosx@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: ollama
 Requires-Dist: python-dotenv
 Requires-Dist: python-telegram-bot
 Description-Content-Type: text/markdown
 
+**HELP NEEDED, if you think you can help me maintain this project, please create a issue.**
+
 # Introduction
 
 aitelegrambot is a Telegram bot that uses the
 [Ollama](http://ollama.com/) backend to run the LLM
 [rationalAI](https://ollama.com/tusharhero/rationalai)(by
 default). This bot is designed to provide access to the full
 capabilities of Ollama through Telegram, allowing users to interact
```

