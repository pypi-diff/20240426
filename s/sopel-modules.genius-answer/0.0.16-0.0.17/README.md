# Comparing `tmp/sopel_modules.genius-answer-0.0.16.tar.gz` & `tmp/sopel_modules_genius_answer-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_modules.genius-answer-0.0.16.tar", last modified: Thu Oct  6 19:57:12 2022, max compression
+gzip compressed data, was "sopel_modules_genius_answer-0.0.17.tar", last modified: Fri Apr 26 16:33:58 2024, max compression
```

## Comparing `sopel_modules.genius-answer-0.0.16.tar` & `sopel_modules_genius_answer-0.0.17.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:57:12.771935 sopel_modules.genius-answer-0.0.16/
--rw-rw-r--   0 user      (1000) user      (1000)      702 2022-10-06 08:06:57.000000 sopel_modules.genius-answer-0.0.16/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)      111 2022-10-06 09:42:43.000000 sopel_modules.genius-answer-0.0.16/NOTE.md
--rw-rw-r--   0 user      (1000) user      (1000)      743 2022-10-06 19:57:12.771935 sopel_modules.genius-answer-0.0.16/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      419 2022-10-06 09:31:11.000000 sopel_modules.genius-answer-0.0.16/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      625 2022-10-06 09:47:55.000000 sopel_modules.genius-answer-0.0.16/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-10-06 19:57:12.771935 sopel_modules.genius-answer-0.0.16/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:57:12.770935 sopel_modules.genius-answer-0.0.16/sopel_modules/
--rw-rw-r--   0 user      (1000) user      (1000)       56 2022-10-06 09:37:05.000000 sopel_modules.genius-answer-0.0.16/sopel_modules/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:57:12.771935 sopel_modules.genius-answer-0.0.16/sopel_modules/genius-answer/
--rw-rw-r--   0 user      (1000) user      (1000)     1988 2022-10-06 19:56:50.000000 sopel_modules.genius-answer-0.0.16/sopel_modules/genius-answer/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-10-06 19:57:12.771935 sopel_modules.genius-answer-0.0.16/sopel_modules.genius_answer.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      743 2022-10-06 19:57:12.000000 sopel_modules.genius-answer-0.0.16/sopel_modules.genius_answer.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      363 2022-10-06 19:57:12.000000 sopel_modules.genius-answer-0.0.16/sopel_modules.genius_answer.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-10-06 19:57:12.000000 sopel_modules.genius-answer-0.0.16/sopel_modules.genius_answer.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       37 2022-10-06 19:57:12.000000 sopel_modules.genius-answer-0.0.16/sopel_modules.genius_answer.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       14 2022-10-06 19:57:12.000000 sopel_modules.genius-answer-0.0.16/sopel_modules.genius_answer.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 16:33:58.917505 sopel_modules_genius_answer-0.0.17/
+-rw-rw-r--   0 user      (1000) user      (1000)      702 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.17/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)      111 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.17/NOTE.md
+-rw-r--r--   0 user      (1000) user      (1000)     1000 2024-04-26 16:33:58.916505 sopel_modules_genius_answer-0.0.17/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      592 2024-04-26 15:48:30.000000 sopel_modules_genius_answer-0.0.17/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      674 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.17/TODO
+-rw-rw-r--   0 user      (1000) user      (1000)      642 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.17/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-26 16:33:58.917505 sopel_modules_genius_answer-0.0.17/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 16:33:58.915505 sopel_modules_genius_answer-0.0.17/sopel_modules/
+-rw-rw-r--   0 user      (1000) user      (1000)       56 2024-04-26 15:08:23.000000 sopel_modules_genius_answer-0.0.17/sopel_modules/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 16:33:58.916505 sopel_modules_genius_answer-0.0.17/sopel_modules/genius-answer/
+-rw-rw-r--   0 user      (1000) user      (1000)     2180 2024-04-26 16:28:27.000000 sopel_modules_genius_answer-0.0.17/sopel_modules/genius-answer/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-26 16:33:58.916505 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1000 2024-04-26 16:33:58.000000 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      368 2024-04-26 16:33:58.000000 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-26 16:33:58.000000 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-26 16:33:58.000000 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       14 2024-04-26 16:33:58.000000 sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/top_level.txt
```

### Comparing `sopel_modules.genius-answer-0.0.16/.gitignore` & `sopel_modules_genius_answer-0.0.17/.gitignore`

 * *Files identical despite different names*

### Comparing `sopel_modules.genius-answer-0.0.16/PKG-INFO` & `sopel_modules_genius_answer-0.0.17/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: sopel_modules.genius-answer
-Version: 0.0.16
-Summary: A microframework for network oriented applications
+Version: 0.0.17
+Summary: A sopel plugin (irc-bot) to answer with a quote from rapgenius.com 
 Author-email: eoli3n <eoli3n@runbox.com>
 License: WTFPL
 Project-URL: Source code, https://github.com/eoli3n/sopel-genius-answer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: sopel<8,>=7.1
+Requires-Dist: lyricsgenius<4,>=3.0.1
 
 # sopel-genius-answer
 A sopel plugin (irc-bot) to answer with a quote from rapgenius.com
 
 ### Install genius-answer plugin
 
 ```bash
@@ -22,7 +24,16 @@
 To create the genius token, see https://github.com/johnwmillr/lyricsgenius#setup  
 In ``default.cfg`` config file, add a ``[genius]`` section with ``api_key`` as
 
 ```ini
 [genius]
 api_key = xxxxxxxxxxxxxxxxx
 ```
+
+### Configure per channel fallback answers
+Bot will ``say``, not ``answer``.
+
+```ini
+[fallback]
+default="I don't know dude."
+channel="#channel is such a great place !"
+```
```

### Comparing `sopel_modules.genius-answer-0.0.16/pyproject.toml` & `sopel_modules_genius_answer-0.0.17/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 61",
     "setuptools_scm >= 6.4"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sopel_modules.genius-answer"
-description = "A microframework for network oriented applications"
+description = "A sopel plugin (irc-bot) to answer with a quote from rapgenius.com "
 readme = "README.md"
 authors = [{name = "eoli3n", email = "eoli3n@runbox.com"}]
 license = {text = "WTFPL"}
 requires-python = ">=3.8"
 dependencies = [
     "sopel>=7.1,<8",
     "lyricsgenius>=3.0.1,<4"
```

### Comparing `sopel_modules.genius-answer-0.0.16/sopel_modules/genius-answer/__init__.py` & `sopel_modules_genius_answer-0.0.17/sopel_modules/genius-answer/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,27 +41,34 @@
     }
     return result
 
 def search_line_by_song(sid):
     text = genius.lyrics(song_id=sid)
     text_list = text.split('\n')
     text_length = len(text_list) 
-    randomnum = randomnum = random.randrange(text_length - 1)
+    randomnum = random.randrange(text_length - 1)
     line = text_list[randomnum]
     return line
 
 def genius_bot_answer(line):
-    words = get_two_words_in_text(line)
-    result = search_song_by_text(words)
-    answer = search_line_by_song(result['song_id'])
+    try:
+        words = get_two_words_in_text(line)
+        result = search_song_by_text(words)
+        answer = search_line_by_song(result['song_id'])
+    except:
+        return False
     return answer
 
 @plugin.rule(r'(.*\b)($nickname)[ :,](.*)')
 
 def sentence_responder(bot, trigger):
     message = trigger.group(1) + trigger.group(3)
     response = genius_bot_answer(message)
-    fallback = "J'ai pas le moral là... je crois que je suis amoureux d'arch_ange et elle ignore mes query"
+    channel = bot.channels[trigger.sender].name.replace('#','')
+    if getattr(bot.config.fallback, channel):
+        fallback = getattr(bot.config.fallback, channel)
+    elif bot.config.fallback.default:
+        fallback = bot.config.fallback.default
     if response:
         bot.reply(response)
-    else:
-        bot.reply(fallback)
+    elif fallback:
+        bot.say(fallback)
```

### Comparing `sopel_modules.genius-answer-0.0.16/sopel_modules.genius_answer.egg-info/PKG-INFO` & `sopel_modules_genius_answer-0.0.17/sopel_modules.genius_answer.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
-Name: sopel-modules.genius-answer
-Version: 0.0.16
-Summary: A microframework for network oriented applications
+Name: sopel_modules.genius-answer
+Version: 0.0.17
+Summary: A sopel plugin (irc-bot) to answer with a quote from rapgenius.com 
 Author-email: eoli3n <eoli3n@runbox.com>
 License: WTFPL
 Project-URL: Source code, https://github.com/eoli3n/sopel-genius-answer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: sopel<8,>=7.1
+Requires-Dist: lyricsgenius<4,>=3.0.1
 
 # sopel-genius-answer
 A sopel plugin (irc-bot) to answer with a quote from rapgenius.com
 
 ### Install genius-answer plugin
 
 ```bash
@@ -22,7 +24,16 @@
 To create the genius token, see https://github.com/johnwmillr/lyricsgenius#setup  
 In ``default.cfg`` config file, add a ``[genius]`` section with ``api_key`` as
 
 ```ini
 [genius]
 api_key = xxxxxxxxxxxxxxxxx
 ```
+
+### Configure per channel fallback answers
+Bot will ``say``, not ``answer``.
+
+```ini
+[fallback]
+default="I don't know dude."
+channel="#channel is such a great place !"
+```
```

