# Comparing `tmp/groqon-0.1.0.tar.gz` & `tmp/groqon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groqon-0.1.0.tar", max compression
+gzip compressed data, was "groqon-0.1.1.tar", max compression
```

## Comparing `groqon-0.1.0.tar` & `groqon-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2395 2024-04-25 18:31:43.241228 groqon-0.1.0/README.md
--rw-r--r--   0        0        0      111 2024-04-25 19:10:06.592737 groqon-0.1.0/groqon/__init__.py
--rw-r--r--   0        0        0     4492 2024-04-25 17:55:15.560946 groqon-0.1.0/groqon/groq.py
--rw-r--r--   0        0        0      177 2024-04-25 12:57:55.515517 groqon-0.1.0/groqon/groq_config.py
--rw-r--r--   0        0        0     4137 2024-04-25 17:30:58.573383 groqon-0.1.0/groqon/groq_utils.py
--rw-r--r--   0        0        0      390 2024-04-25 19:12:26.832374 groqon-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 groqon-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2571 2024-04-25 19:47:18.747816 groqon-0.1.1/README.md
+-rw-r--r--   0        0        0      112 2024-04-25 19:21:55.434929 groqon-0.1.1/groqon/__init__.py
+-rw-r--r--   0        0        0     4746 2024-04-25 19:57:20.288794 groqon-0.1.1/groqon/groq.py
+-rw-r--r--   0        0        0      178 2024-04-25 19:53:54.205780 groqon-0.1.1/groqon/groq_config.py
+-rw-r--r--   0        0        0     4138 2024-04-25 19:22:25.722853 groqon-0.1.1/groqon/groq_utils.py
+-rw-r--r--   0        0        0      390 2024-04-25 19:58:57.424340 groqon-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 groqon-0.1.1/PKG-INFO
```

### Comparing `groqon-0.1.0/README.md` & `groqon-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # GROQ without API
 
-This projects uses playwright to Access [GROQ]('www.groq.com') using python
+This projects uses playwright to Access [GROQ]('https://www.groq.com') using python
 
 ## Inspiration(Story)
 On a long summer evening of april 2023 I was sitting in front of cranky old fan working on my [News-app](https://www.github.com/tikendraw/news-app). I needed a llm api to summarize the news articles. As a poor man I do not have money to buy llm subscription, I chose to use [Gemini]('https://gemini.google.com) (limit 1 req/sec), it took avg 8-9 sec per request to process, felt dissapointed.
 
 At this point I have heard about Groq and its new LPU hardware that outputs insanely fast. 
 There wasn't any free api for poor people like me. So I decided to emulate the user using playwright and can query and get the llm response. Finally as the thousands of seconds passed I could manage to make it work. Now you can too. 
 
@@ -13,14 +13,15 @@
 
 
 ## Working
 
 * It emulates user using playwright and queries the selected model and ouputs the response as a json object.
 * It uses cookie to login.(For the first time you have to login in under 120 seconds(browser will be open for 2 minutes), your cookies will be saved and will be used again next time you query)
 * This code doesn't share your cookie or any kind of data with anyone.
+* One way query.
 
 ## Installation
 ```
 pip install groq-on
 ```
 make sure you have playwright installed, if not do this
 ```
@@ -60,10 +61,16 @@
   --save_output         set true to save the groq output with its query name.json
   --output_dir OUTPUT_DIR
                         Path to save the output file. Defaults to current working directory.
 ```
 
 ## TODO
 
-[ ] Keep updated
-[ ] Add something
-[ ] Use Better parser
+* [ ] Keep updated
+* [ ] Add something
+* [ ] Use Better parser
+* [ ] Use color for better Visual
+* [ ] Multiround chat
+
+## Contribution
+
+Feel free to add features and keep it maintained and do pull requests.
```

### Comparing `groqon-0.1.0/groqon/groq.py` & `groqon-0.1.1/groqon/groq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import argparse
 import json
 import os
-import argparse
 from contextlib import contextmanager
 
-from playwright.sync_api import sync_playwright
-from groq_config import modelindex
-from groq_utils import (
+from playwright.sync_api import Page, sync_playwright
+
+from .groq_config import modelindex
+from .groq_utils import (
     check_element_and_get_text,
     clear_chat,
     file_exists,
     get_content,
     get_cookie,
     get_query,
     save_cookie,
@@ -18,52 +19,54 @@
 
 URL = 'https://groq.com/'
 QUERY_INPUT_SELECTOR = "#chat"
 QUERY_SUBMIT_SELECTOR = ".self-end"
 END_TEXT_SELECTOR = "body > main > div > div.flex.flex-col-reverse.md\:flex-col.md\:relative.w-full.max-w-\[900px\].bg-background.z-10.gap-2.md\:gap-6 > div > a > div > div"
 
 @contextmanager
-def groq_context(cookie_file='groq_cookie.json', model='llama3-70b', headless=False):
+def groq_context(cookie_file:str='groq_cookie.json', model:str='llama3-70b', headless:bool=False):
 
     url = URL
 
     if file_exists(cookie_file):
         cookie = get_cookie(cookie_file)
-
-
-    headless = False if not cookie else headless
+    else:
+        headless=False
+        cookie=None
     
     with sync_playwright() as p:
         browser = p.firefox.launch(headless=headless)
         context = browser.new_context()
         page = context.new_page()
 
         if cookie:
             context.add_cookies(cookie)
             print("Cookie loaded!!!")
         else:
             print("Cookie not loaded!!!", "You have 120 seconds to login to groq.com, Make it quick!!! HEADLESS is set to False")
-            page.wait_for_timeout(1000 * 120)
 
         page.goto(url, timeout=60_000, wait_until='networkidle')
+        
+        if not cookie:
+            page.wait_for_timeout(1000*120) #120 sec to login
+            
         page.screenshot(path="screenshot1.png", full_page=True)
 
         # Set model
         select_model(page, model_choice=model)
 
         try:
             yield page
         finally:
             # Save cookie
             save_cookie(context.cookies(), cookie_file)
-            page.screenshot(path="screenshot3_cleared_chat.png", full_page=True)
             browser.close()
             print("Browser closed!!!")
 
-def get_groq_response(page, query, save_output: bool=False, save_dir=str(os.getcwd())):
+def get_groq_response(page:Page, query:str, save_output:bool=False, save_dir:str=str(os.getcwd())):
     # Add query
     page.locator(QUERY_INPUT_SELECTOR).fill(query)
     # Submit query
     page.locator(QUERY_SUBMIT_SELECTOR).click()
 
     # Check if generation finished if not wait till end and get tok/s
     is_present, end_text = check_element_and_get_text(page, END_TEXT_SELECTOR)
@@ -71,41 +74,45 @@
     if not is_present:
         print("Generation not finished!!!")
         page.screenshot(path="screenshot_generation_not_finished.png", full_page=True)
         return
 
     # Get query and text generated
     query_text, raw_query_html = get_query(page)
-    text_content, raw_text_html = get_content(page)
+    response_content, raw_response_html = get_content(page)
 
     # Screenshot the content (for no reason)
     page.screenshot(path="screenshot2.png", full_page=True)
     clear_chat(page)
 
     output_dict = {
                 "query": query_text,
-                "text": text_content,
+                "response": response_content,
                 "query_html":raw_query_html,
-                "text_content":raw_text_html,
+                "response_html":raw_response_html,
                 "tok/s": end_text
             }
     if save_output:
         with open(os.path.join(save_dir,query_text + '.json'), 'w') as f:
             json.dump(output_dict, f)
 
     return output_dict
     
 
-def groq(query_list, cookie_file='groq_cookie.json', model='llama3-70b', headless=False, save_output=True, save_dir=str(os.getcwd())):
-
+def groq(query_list:list[str], cookie_file:str='groq_cookie.json', model:str='llama3-70b', headless:bool=False, save_output:bool=True, save_dir=str(os.getcwd())):
+    
+    if isinstance(query_list, str):
+        query_list = [query_list]
+        
     with groq_context(cookie_file=cookie_file, model=model, headless=headless) as page:
         for query in query_list:
             response = get_groq_response(page, query, save_output=save_output, save_dir=save_dir)
-            for i in response:
-                print(i, ":", response.get(i, None))
+            print('Query', ":", response.get('query', None))
+            print('Response', ":", response.get('response', None))
+            print('tok/s', ":", response.get('tok/s', None))
     
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('queries', nargs='+', help="one or alot of quoted string like 'what is the purpose of life?' 'why everyone hates meg griffin?'")
     parser.add_argument('--model', default='llama3-70b', help=f"Available models are {" ".join(modelindex)}")
     parser.add_argument('--cookie_file', type=str, default='groq_cookie.json')
@@ -122,8 +129,8 @@
         query_list=args.queries, 
         save_output=args.save_output, 
         save_dir=args.output_dir
     )
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `groqon-0.1.0/groqon/groq_utils.py` & `groqon-0.1.1/groqon/groq_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import re
 from html import unescape
 from pathlib import Path
 
 from playwright.sync_api import Page
 
-from groq_config import modelindex
+from .groq_config import modelindex
 
 CLEAR_CHAT_BUTTON = "body > main > div > div.flex.flex-col-reverse.md\:flex-col.md\:relative.w-full.max-w-\[900px\].bg-background.z-10.gap-2.md\:gap-6 > div > button.inline-flex.items-center.justify-center.whitespace-nowrap.rounded-md.text-sm.font-medium.ring-offset-background.transition-colors.focus-visible\:outline-none.disabled\:pointer-events-none.disabled\:opacity-50.underline-offset-4.h-10.p-0.text-muted-foreground.hover\:text-primaryaccent.hover\:no-underline"
 DROPDOWN_BUTTON = "body > header > div.flex-1.flex.items-center.justify-center.md\:col-span-4.md\:col-start-2 > div > button.flex.h-10.w-full.items-center.justify-between.border.border-input.bg-background.py-2.text-sm.ring-offset-background.placeholder\:text-muted-foreground.focus\:outline-none.focus\:ring-ring.focus\:ring-offset-2.disabled\:cursor-not-allowed.disabled\:opacity-50.\[\&\>span\]\:line-clamp-1.ml-auto.max-w-\[160px\].sm\:max-w-\[190px\].rounded-none.border-none.overflow-hidden.px-2.sm\:px-3.focus\:ring-0"
 QUERY_SELECTOR = "div.break-words"
 RESPONSE_SELECTOR = "div.text-base"
 
 def select_model(page:Page, model_choice):
```

### Comparing `groqon-0.1.0/PKG-INFO` & `groqon-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: groqon
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use Groq.com as llm
 Author: tikendraw
 Author-email: tikendraksahu1029@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # GROQ without API
 
-This projects uses playwright to Access [GROQ]('www.groq.com') using python
+This projects uses playwright to Access [GROQ]('https://www.groq.com') using python
 
 ## Inspiration(Story)
 On a long summer evening of april 2023 I was sitting in front of cranky old fan working on my [News-app](https://www.github.com/tikendraw/news-app). I needed a llm api to summarize the news articles. As a poor man I do not have money to buy llm subscription, I chose to use [Gemini]('https://gemini.google.com) (limit 1 req/sec), it took avg 8-9 sec per request to process, felt dissapointed.
 
 At this point I have heard about Groq and its new LPU hardware that outputs insanely fast. 
 There wasn't any free api for poor people like me. So I decided to emulate the user using playwright and can query and get the llm response. Finally as the thousands of seconds passed I could manage to make it work. Now you can too. 
 
@@ -26,14 +26,15 @@
 
 
 ## Working
 
 * It emulates user using playwright and queries the selected model and ouputs the response as a json object.
 * It uses cookie to login.(For the first time you have to login in under 120 seconds(browser will be open for 2 minutes), your cookies will be saved and will be used again next time you query)
 * This code doesn't share your cookie or any kind of data with anyone.
+* One way query.
 
 ## Installation
 ```
 pip install groq-on
 ```
 make sure you have playwright installed, if not do this
 ```
@@ -73,10 +74,16 @@
   --save_output         set true to save the groq output with its query name.json
   --output_dir OUTPUT_DIR
                         Path to save the output file. Defaults to current working directory.
 ```
 
 ## TODO
 
-[ ] Keep updated
-[ ] Add something
-[ ] Use Better parser
+* [ ] Keep updated
+* [ ] Add something
+* [ ] Use Better parser
+* [ ] Use color for better Visual
+* [ ] Multiround chat
+
+## Contribution
+
+Feel free to add features and keep it maintained and do pull requests.
```

