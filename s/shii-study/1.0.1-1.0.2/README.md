# Comparing `tmp/shii_study-1.0.1-py2.py3-none-any.whl.zip` & `tmp/shii_study-1.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3172 bytes, number of entries: 7
+Zip file size: 3255 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      204 b- defN 80-Jan-01 00:00 shii/__init__.py
 -rw-r--r--  2.0 unx       17 b- defN 80-Jan-01 00:00 shii/src/__init__.py
--rw-r--r--  2.0 unx     3178 b- defN 80-Jan-01 00:00 shii/src/study.py
--rw-r--r--  2.0 unx      800 b- defN 80-Jan-01 00:00 shii_study-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 shii_study-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 shii_study-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      530 b- defN 80-Jan-01 00:00 shii_study-1.0.1.dist-info/RECORD
-7 files, 4844 bytes uncompressed, 2232 bytes compressed:  53.9%
+-rw-r--r--  2.0 unx     3472 b- defN 80-Jan-01 00:00 shii/src/study.py
+-rw-r--r--  2.0 unx      800 b- defN 80-Jan-01 00:00 shii_study-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 shii_study-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 shii_study-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      530 b- defN 80-Jan-01 00:00 shii_study-1.0.2.dist-info/RECORD
+7 files, 5138 bytes uncompressed, 2315 bytes compressed:  54.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: shii/src/__init__.py
 Comment: 
 
 Filename: shii/src/study.py
 Comment: 
 
-Filename: shii_study-1.0.1.dist-info/METADATA
+Filename: shii_study-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: shii_study-1.0.1.dist-info/WHEEL
+Filename: shii_study-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: shii_study-1.0.1.dist-info/top_level.txt
+Filename: shii_study-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: shii_study-1.0.1.dist-info/RECORD
+Filename: shii_study-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shii/__init__.py

```diff
@@ -1,3 +1,3 @@
 from shii.src.study import study, study_return_text, no_study_return_text, study_say, del_study
 __all__ = ['study', 'study_return_text', 'study_say', 'no_study_return_text', 'del_study']
-version = '1.0.1'
+version = '1.0.2'
```

## shii/src/__init__.py

```diff
@@ -1 +1 @@
-version = '1.0.1'
+version = '1.0.2'
```

## shii/src/study.py

```diff
@@ -1,29 +1,33 @@
 # Part of Shii (
 #
 # Description: Shii is a discord bot that can be taught to respond to certain keywords.
-from logging import Logger
-import json
+import logging
+import json
 
+logger: logging.Logger = logging.getLogger(__name__)
 study_return = None
-no_study_return = None
+no_study_return = None
+  
 
 def study_return_text(text):
     '''Sets the text returned when training is complete.'''
     ''':study_return_text ex): study_return_text("네! 알았어요!")'''
     '''학습 성공시 리턴되는 텍스트를 정의 합니다.'''
     global study_return
     study_return = text
+    logging.info(f"Study return text set to {study_return}")
 
 
 def no_study_return_text(text):
   '''Sets the text returned when training is not complete.'''
   ''':no_study_return_text ex): no_study_return_text("으에?")"'''
   global no_study_return
-  no_study_return = text
+  no_study_return = text
+  logging.info(f"No study return text set to {no_study_return}")
 
 
 def load_bot_info():
     try:
         with open('bot_info.json', 'r', encoding='utf-8') as f:
             bot_info = json.load(f)
     except FileNotFoundError:
@@ -53,29 +57,33 @@
     if keyword not in bot_info:
         bot_info[keyword] = {
             'description': description,
             'author_nickname': user_id
         }
         save_bot_info(bot_info)
         if study_return == None:
+          logging.info(f"Study comleted. {keyword} added.")
           return f"'{keyword}'를 학습하였습니다."
-        else:
+        else:
+          logging.info(f"Study comleted. {keyword} added.")
           return study_return
     else:
         return f"`{keyword}`는 이미 알고 있어요!"
 
 
 def study_say(keyword: str):
     '''Returns the description of the keyword.'''
     ''':return ex): 안녕하세요'''
     bot_info = load_bot_info()
-    info = bot_info.get(keyword)
+    info = bot_info.get(keyword)
+  
     word = {
-        'shii': f"`pip install -U shii`",
-    }
+          'shii': f"`pip install -U shii`",
+    }
+  
     if keyword in word.keys():
         return f'{word[keyword]}'
     else:
         if info:
             author_nickname = info['author_nickname']
             description = info['description']
             return f"{description}\n`{author_nickname} 님이 알려주셨어요!`"
```

## Comparing `shii_study-1.0.1.dist-info/METADATA` & `shii_study-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shii_study
-Version: 1.0.1
+Version: 1.0.2
 Summary: PYPI tutorial package creation written by Boran
 Home-page: https://github.com/boranloves/shii
 Author: boran
 Author-email: boran <boran@shii.me>
 Project-URL: Homepage, https://github.com/boranloves/shii
 Project-URL: Issues, https://github.com/boranloves/shii
 Classifier: Programming Language :: Python :: 3
```

## Comparing `shii_study-1.0.1.dist-info/RECORD` & `shii_study-1.0.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-shii/__init__.py,sha256=MFbY2UAz0hN4_9FzO-R1hZ2-DQYkTKe-S-2e2j11_hM,204
-shii/src/__init__.py,sha256=ZrxVG_1EyOtJGZv5TksXAOwRZof1WpD_EEEOOXzcZko,17
-shii/src/study.py,sha256=q1V-yD79ER2GUvSPA-r8QcoPEDF5rdvJA7l4E34U6GU,3178
-shii_study-1.0.1.dist-info/METADATA,sha256=n_i2-CGZLFfj8vVK5TsOB-z8XwuYyEHuGybfaPVQIJ8,800
-shii_study-1.0.1.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-shii_study-1.0.1.dist-info/top_level.txt,sha256=xSjQX0HJSMT8sgtMRf6vWT1kRi8g03W9l-ttA6Mmbgk,5
-shii_study-1.0.1.dist-info/RECORD,,
+shii/__init__.py,sha256=vxiyurUM77ugZY065rg7ag1IMkWIz9P1bcSTQhYpwk4,204
+shii/src/__init__.py,sha256=VQKfdd_ofogkXNr4epD-N2TOkX1WVYa49SS8-W-q5Os,17
+shii/src/study.py,sha256=CeXJBSp1ZfcUn7KvXribmsiiXhYOC9PpQy3lPvPIMIg,3472
+shii_study-1.0.2.dist-info/METADATA,sha256=e4i5WVxXvE59oTYEqxIC27w8_BZQ50WzUQCma_tsd6o,800
+shii_study-1.0.2.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+shii_study-1.0.2.dist-info/top_level.txt,sha256=xSjQX0HJSMT8sgtMRf6vWT1kRi8g03W9l-ttA6Mmbgk,5
+shii_study-1.0.2.dist-info/RECORD,,
```

