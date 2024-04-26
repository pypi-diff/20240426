# Comparing `tmp/groqon-0.1.2.tar.gz` & `tmp/groqon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groqon-0.1.2.tar", max compression
+gzip compressed data, was "groqon-0.1.3.tar", max compression
```

## Comparing `groqon-0.1.2.tar` & `groqon-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3218 2024-04-26 06:48:23.791166 groqon-0.1.2/README.md
--rw-r--r--   0        0        0      112 2024-04-25 19:21:55.434929 groqon-0.1.2/groqon/__init__.py
--rw-r--r--   0        0        0     7987 2024-04-26 06:39:48.642772 groqon-0.1.2/groqon/groq.py
--rw-r--r--   0        0        0      178 2024-04-25 19:53:54.205780 groqon-0.1.2/groqon/groq_config.py
--rw-r--r--   0        0        0     9253 2024-04-26 06:18:39.760558 groqon-0.1.2/groqon/groq_utils.py
--rw-r--r--   0        0        0      390 2024-04-26 06:42:04.999894 groqon-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 groqon-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3396 2024-04-26 08:37:30.417926 groqon-0.1.3/README.md
+-rw-r--r--   0        0        0      112 2024-04-26 08:37:30.417926 groqon-0.1.3/groqon/__init__.py
+-rw-r--r--   0        0        0     8236 2024-04-26 08:37:30.417926 groqon-0.1.3/groqon/groq.py
+-rw-r--r--   0        0        0      178 2024-04-26 08:37:30.417926 groqon-0.1.3/groqon/groq_config.py
+-rw-r--r--   0        0        0     9221 2024-04-26 08:37:30.417926 groqon-0.1.3/groqon/groq_utils.py
+-rw-r--r--   0        0        0      446 2024-04-26 08:37:30.417926 groqon-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3800 1970-01-01 00:00:00.000000 groqon-0.1.3/PKG-INFO
```

### Comparing `groqon-0.1.2/README.md` & `groqon-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# GROQ without API
+# GROQ without API : GroqOn
 
 This projects uses playwright to Access [GROQ](https://www.groq.com) using python
 
 ## Inspiration(Story)
-On a long summer evening of april 2023 I was sitting in front of cranky old fan working on my [News-app](https://www.github.com/tikendraw/news-app). I needed a llm api to summarize the news articles. As a poor man I do not have money to buy llm subscription, I chose to use [Gemini](https://gemini.google.com) (limit 1 req/sec), it took avg 8-9 sec per request to process, felt dissapointed.
+On a long summer evening of april 2024 I was sitting in front of cranky old fan working on my [News-app](https://www.github.com/tikendraw/news-app). I needed a llm api to summarize the news articles. As a poor man I do not have money to buy llm subscription, I chose to use [Gemini](https://gemini.google.com) (limit 1 req/sec), it took avg 8-9 sec per request to process, felt dissapointed.
 
 At this point I have heard about Groq and its new LPU hardware that outputs insanely fast. 
 There wasn't any free api for poor people like me. So I decided to emulate the user using playwright and can query and get the llm response. Finally as the thousands of seconds passed I could manage to make it work. Now you can use groq.com as llm too. I did it for poor people. 
 
 ## Working
 
 * It emulates user using playwright and queries the selected model and ouputs the response as a json object.
@@ -76,20 +76,24 @@
   --cookie_file COOKIE_FILE
   --headless            set true to not see the browser
   --save_output         set true to save the groq output with its query name.json
   --output_dir OUTPUT_DIR
                         Path to save the output file. Defaults to current working directory.
 ```
 
-## TODO
+## TODO (Need Help)
 
 * [x] Set System Prompt
 * [ ] Keep updated
 * [ ] Add something
 * [ ] Use Better parser
-* [ ] Use color for better Visual /Rich text formatting
+* [ ] Use color for better Visual / Rich text formatting
 * [ ] Add logger
 * [ ] Multiround chat
 
 ## Contribution
 
-Feel free to add features and keep it maintained and do pull requests.
+Feel free to add features and keep it maintained and do pull requests.
+
+## Buy me a Coffee/Chai
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoffee.com/tikendraw)
+
```

### Comparing `groqon-0.1.2/groqon/groq.py` & `groqon-0.1.3/groqon/groq.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,27 @@
     save_cookie,
     select_model,
     set_system_prompt,
 )
 from pathlib import Path
 
 
-URL = 'https://groq.com/'
+URL = "https://groq.com/"
 QUERY_INPUT_SELECTOR = "#chat"
 QUERY_SUBMIT_SELECTOR = ".self-end"
 END_TEXT_SELECTOR = r"body > main > div > div.flex.flex-col-reverse.md\:flex-col.md\:relative.w-full.max-w-\[900px\].bg-background.z-10.gap-2.md\:gap-6 > div > a > div > div"
 
 
 @contextmanager
-def groq_context(cookie_file:str='groq_cookie.json', model:str='llama3-70b', headless:bool=False, system_prompt:str=None) -> Page:
+def groq_context(
+    cookie_file: str = "groq_cookie.json",
+    model: str = "llama3-70b",
+    headless: bool = False,
+    system_prompt: str = None,
+) -> Page:
     """
     Context manager for creating a Groq context.
 
     Args:
         cookie_file (str, optional): The path to the cookie file. Defaults to 'groq_cookie.json'.
         model (str, optional): The model to use. Defaults to 'llama3-70b'.
         headless (bool, optional): Whether to run the browser in headless mode. Defaults to False.
@@ -45,33 +50,36 @@
     """
 
     url = URL
 
     if file_exists(cookie_file):
         cookie = get_cookie(cookie_file)
     else:
-        headless=False
-        cookie=None
-    
+        headless = False
+        cookie = None
+
     with sync_playwright() as p:
         browser = p.firefox.launch(headless=headless)
         context = browser.new_context()
         page = context.new_page()
 
         if cookie:
             context.add_cookies(cookie)
             print("Cookie loaded!!!")
         else:
-            print("Cookie not loaded!!!", "You have 120 seconds to login to groq.com, Make it quick!!! HEADLESS is set to False")
+            print(
+                "Cookie not loaded!!!",
+                "You have 120 seconds to login to groq.com, Make it quick!!! HEADLESS is set to False",
+            )
+
+        page.goto(url, timeout=60_000, wait_until="networkidle")
 
-        page.goto(url, timeout=60_000, wait_until='networkidle')
-        
         if not cookie:
-            page.wait_for_timeout(1000*120) #120 sec to login
-            
+            page.wait_for_timeout(1000 * 120)  # 120 sec to login
+
         page.screenshot(path="screenshot1.png", full_page=True)
 
         # Set model
         select_model(page, model_choice=model)
 
         # Set system prompt
         if system_prompt:
@@ -81,15 +89,18 @@
             yield page
         finally:
             # Save cookie
             save_cookie(context.cookies(), cookie_file)
             browser.close()
             print("Browser closed!!!")
 
-def get_groq_response(page:Page, query:str, save_output:bool=False, save_dir:str=os.getcwd()) -> dict:
+
+def get_groq_response(
+    page: Page, query: str, save_output: bool = False, save_dir: str = os.getcwd()
+) -> dict:
     """
     Retrieves the response to a given query using the specified page object.
 
     Args:
         page (Page): The page object for interacting with the browser.
         query (str): The query string to be filled in the input field.
         save_output (bool, optional): A flag indicating whether to save the output as a JSON file. Defaults to False.
@@ -116,42 +127,42 @@
     response_content, raw_response_html = get_content_text(page)
 
     # Screenshot the content (for no reason)
     page.screenshot(path="screenshot2.png", full_page=True)
     clear_chat(page)
 
     output_dict = {
-                "query": query_text,
-                "response": response_content,
-                # "query_html":raw_query_html,
-                # "response_html":raw_response_html,
-                "token/s": end_text
-            }
+        "query": query_text,
+        "response": response_content,
+        # "query_html":raw_query_html,
+        # "response_html":raw_response_html,
+        "token/s": end_text,
+    }
     if save_output:
         save_dir = Path(save_dir)
         save_dir.mkdir(parents=True, exist_ok=True)
-        
-        json_file = save_dir / f'{query_text}.json'
 
-        with open(json_file, 'w') as f:
+        json_file = save_dir / f"{query_text}.json"
+
+        with open(json_file, "w") as f:
             json.dump(output_dict, f)
 
     return output_dict
-    
+
 
 def groq(
-    query_list:list[str], 
-    cookie_file:str='groq_cookie.json', 
-    model:str='llama3-70b', 
-    headless:bool=False, 
-    save_output:bool=True, 
-    save_dir:str=os.getcwd(),
-    system_prompt:str=None,
-    print_output=True
-    ) -> list[dict]:
+    query_list: list[str],
+    cookie_file: str = "groq_cookie.json",
+    model: str = "llama3-70b",
+    headless: bool = False,
+    save_output: bool = True,
+    save_dir: str = os.getcwd(),
+    system_prompt: str = None,
+    print_output=True,
+) -> list[dict]:
     """
     Executes a list of Groq queries and returns a list of dictionaries containing the query, response, and token/s value.
 
     Args:
         query_list (list[str]): A list of Groq queries to execute.
         cookie_file (str, optional): The path to the cookie file. Defaults to 'groq_cookie.json'.
         model (str, optional): The model to use. Defaults to 'llama3-70b'.
@@ -164,46 +175,79 @@
     Returns:
         list[dict]: A list of dictionaries containing the query, response, and token/s value for each executed query.
     """
 
     if isinstance(query_list, str):
         query_list = [query_list]
 
-    with groq_context(cookie_file=cookie_file, model=model, headless=headless, system_prompt=system_prompt) as page:
+    with groq_context(
+        cookie_file=cookie_file,
+        model=model,
+        headless=headless,
+        system_prompt=system_prompt,
+    ) as page:
         response_list = []
         for query in query_list:
-            response = get_groq_response(page, query, save_output=save_output, save_dir=save_dir)
+            response = get_groq_response(
+                page, query, save_output=save_output, save_dir=save_dir
+            )
             response_list.append(response)
-            
+
             if print_output:
-                print('Query', ":", response.get('query', None))
-                print('Response', ":", response.get('response', None))
-                print('token/s', ":", response.get('token/s', None))
+                print("Query", ":", response.get("query", None))
+                print("Response", ":", response.get("response", None))
+                print("token/s", ":", response.get("token/s", None))
 
         return response_list
 
+
 def main() -> None:
     parser = argparse.ArgumentParser()
-    parser.add_argument('queries', nargs='+', help="one or more quoted string like 'what is the purpose of life?' 'why everyone hates meg griffin?'")
-    parser.add_argument('--model', default='llama3-70b', help=f"Available models are {" ".join(modelindex)}")
-    parser.add_argument('--cookie_file', type=str, default='groq_cookie.json', help="looks in current directory by default for groq_cookie.json. If not found, You will have to login when the browswer opens under 120 seconds. It's one time thing")
-    parser.add_argument('--system_prompt', type=str, help="System prompt to be given to the llm model. Its like 'you are samuel l jackson as my assistant'. Default is None.")
-    parser.add_argument('--headless', action='store_true', help= "set true to not see the browser")
-    parser.add_argument('--save_output', action='store_true', help="set true to save the groq output with its query name.json")
-    parser.add_argument('--output_dir', default=os.getcwd(), help="Path to save the output file. Defaults to current working directory.")
+    parser.add_argument(
+        "queries",
+        nargs="+",
+        help="one or more quoted string like 'what is the purpose of life?' 'why everyone hates meg griffin?'",
+    )
+    parser.add_argument(
+        "--model",
+        default="llama3-70b",
+        help=f"Available models are {' '.join(modelindex)}",
+    )
+    parser.add_argument(
+        "--cookie_file",
+        type=str,
+        default="groq_cookie.json",
+        help="looks in current directory by default for groq_cookie.json. If not found, You will have to login when the browswer opens under 120 seconds. It's one time thing",
+    )
+    parser.add_argument(
+        "--system_prompt",
+        type=str,
+        help="System prompt to be given to the llm model. Its like 'you are samuel l jackson as my assistant'. Default is None.",
+    )
+    parser.add_argument(
+        "--headless", action="store_true", help="set true to not see the browser"
+    )
+    parser.add_argument(
+        "--save_output",
+        action="store_true",
+        help="set true to save the groq output with its query name.json",
+    )
+    parser.add_argument(
+        "--output_dir",
+        default=os.getcwd(),
+        help="Path to save the output file. Defaults to current working directory.",
+    )
 
     args = parser.parse_args()
-    
+
     groq(
-        cookie_file=args.cookie_file, 
-        model=args.model, 
+        cookie_file=args.cookie_file,
+        model=args.model,
         headless=args.headless,
-        query_list=args.queries, 
-        save_output=args.save_output, 
+        query_list=args.queries,
+        save_output=args.save_output,
         save_dir=args.output_dir,
         system_prompt=args.system_prompt,
-        print_output=True
+        print_output=True,
     )
 
 
-if __name__ == '__main__':
-    main()
```

### Comparing `groqon-0.1.2/groqon/groq_utils.py` & `groqon-0.1.3/groqon/groq_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,37 +12,37 @@
 QUERY_SELECTOR = "div.break-words"
 RESPONSE_SELECTOR = "div.text-base"
 PROMPT_SETTER_SELETOR = r"body > header > div.flex-1.flex.items-center.justify-center.md\:col-span-4.md\:col-start-2 > div > button.flex.gap-1.items-center.ml-1.px-2.sm\:px-3"
 PROMPT_TEXTAREA_SELECTOR = r"#radix-\:r3\: > textarea"
 PROMPT_SAVE_BUTTON_SELECTOR = r"#radix-\:r3\: > div.flex.justify-end.gap-5 > button.inline-flex.items-center.justify-center.whitespace-nowrap.rounded-md.text-sm.font-medium.ring-offset-background.transition-colors.focus-visible\:outline-none.disabled\:pointer-events-none.disabled\:opacity-50.hover\:bg-gray-600.dark\:hover\:bg-slate-200.h-10.px-4.py-2.text-background.bg-foreground"
 
 
-def set_system_prompt(page:Page, system_prompt:str) -> None:
+def set_system_prompt(page: Page, system_prompt: str) -> None:
     """
     Sets the system prompt on the page for interaction.
 
     Args:
         page (Page): The page object for interacting with the browser.
         system_prompt (str): The system prompt text to set.
 
     Returns:
         None
     """
     try:
         page.locator(PROMPT_SETTER_SELETOR).click()
         text_area = page.locator(PROMPT_TEXTAREA_SELECTOR)
         text_area.fill(system_prompt)
-        
+
         page.locator(PROMPT_SAVE_BUTTON_SELECTOR).click()
         print("Set System prompt!")
     except Exception as e:
-        print("Exception occured while setting System Prompt:: ",e)    
-    
-    
-def select_model(page:Page, model_choice) -> None:
+        print("Exception occured while setting System Prompt:: ", e)
+
+
+def select_model(page: Page, model_choice) -> None:
     """
     Selects a model from a dropdown button on a page.
 
     Args:
         page (Page): The page object for interacting with the browser.
         model_choice (str): The name of the model to select.
 
@@ -58,25 +58,27 @@
         the Enter key to select the model. If an error occurs during the process, it prints an error message.
     """
     try:
         # dropdown_button
         page.locator(DROPDOWN_BUTTON).click()
 
         downpress = modelindex.index(model_choice)
-        
+
         for _ in range(downpress):
             page.keyboard.press("ArrowDown")
         page.keyboard.press("Enter")
 
-        print(f'Model set to : {model_choice}')
+        print(f"Model set to : {model_choice}")
     except Exception as e:
-        print("Exception occured while selecting model:: ",e)
-        
-        
-def check_element_and_get_text(page:Page, selector, max_retries=100, retry_delay=1) -> [bool, str|None]:
+        print("Exception occured while selecting model:: ", e)
+
+
+def check_element_and_get_text(
+    page: Page, selector, max_retries=100, retry_delay=1
+) -> [bool, str | None]:
     """
     Checks if an element with the given selector exists on the page and retrieves its inner text.
 
     Args:
         page (Page): The page object for interacting with the browser.
         selector (str): The CSS selector of the element to check.
         max_retries (int, optional): The maximum number of times to retry checking the element. Defaults to 100.
@@ -88,39 +90,40 @@
     """
     retries = 0
     while retries < max_retries:
         element = page.locator(selector)
         if element:
             return True, element.inner_text()
         retries += 1
-        print('Waiting 1 second...')
-        page.wait_for_timeout(1000*retry_delay)
+        print("Waiting 1 second...")
+        page.wait_for_timeout(1000 * retry_delay)
     return False, None
 
 
-def clear_chat(page:Page) -> None:
+def clear_chat(page: Page) -> None:
     """
     Clears the chat on the given page.
 
     Args:
         page (Page): The page object representing the chat interface.
 
     Returns:
         None
 
     Raises:
         Exception: If an error occurs while clearing the chat.
     """
     try:
         page.locator(CLEAR_CHAT_BUTTON).click()
-        print('Chat cleared')
+        print("Chat cleared")
     except Exception as e:
-        print("Exception occured while clearing chat:: ",e)
+        print("Exception occured while clearing chat:: ", e)
 
-def get_text_by_selector(page:Page, selector) -> str:
+
+def get_text_by_selector(page: Page, selector) -> str:
     """
     Retrieves the text content from the element specified by the given selector on the given page.
 
     Args:
         page (Page): The page object for interacting with the browser.
         selector (str): The CSS selector of the element to retrieve the text from.
 
@@ -128,46 +131,48 @@
         tuple: A tuple containing two elements:
                 - The extracted text from the element, converted to markdown format.
                 - The raw HTML content of the element.
     """
     html = page.query_selector(selector).inner_html()
     return extract_to_markdown(html), html
 
+
 # Get the text from the desired elements
-def get_query_text(page:Page) -> str:
+def get_query_text(page: Page) -> str:
     """
     Retrieves the text content from the element specified by the given selector on the given page.
 
     Args:
         page (Page): The page object for interacting with the browser.
 
     Returns:
         tuple: A tuple containing two elements:
                 - The extracted text from the element, converted to markdown format.
                 - The raw HTML content of the element.
     """
-    return get_text_by_selector(page,QUERY_SELECTOR)
+    return get_text_by_selector(page, QUERY_SELECTOR)
 
-def get_content_text(page:Page) -> str:
+
+def get_content_text(page: Page) -> str:
     """
     Retrieves the content from the specified page using the given selector.
 
     Args:
         page (Page): The page object for interacting with the browser.
 
     Returns:
         tuple: A tuple containing two elements:
                 - The extracted content from the element, converted to markdown format.
                 - The raw HTML content of the element.
     """
-    return get_text_by_selector(page,RESPONSE_SELECTOR)
-    
-    
-#load the cookie
-def get_cookie(file_name:str) -> dict|None:
+    return get_text_by_selector(page, RESPONSE_SELECTOR)
+
+
+# load the cookie
+def get_cookie(file_name: str) -> dict | None:
     """
     Retrieves the cookie from the specified file.
 
     Parameters:
         file_name (str): The name of the file containing the cookie.
 
     Returns:
@@ -176,73 +181,75 @@
     Raises:
         FileNotFoundError: If the specified file does not exist.
     """
     with open(file_name) as f:
         return json.load(f)
     return None
 
-def file_exists(file:str) -> bool:
+
+def file_exists(file: str) -> bool:
     """
     Checks if a file exists using pathlib.
 
     Args:
         file (str): The path of the file to check.
 
     Returns:
         bool: True if the file exists, False otherwise.
     """
     path = Path(file)
     return path.exists()
 
-#save the cookie
-def save_cookie(cookie:Any,filename:str="cookies.json") -> None:
+
+# save the cookie
+def save_cookie(cookie: Any, filename: str = "cookies.json") -> None:
     """
     saves the cookie
     Parameters:
         cookie: The cookie data to be saved.
         filename (optional): The name of the file to save the cookie to. Defaults to 'cookies.json'.
     Returns:
         None
     """
-    with open(filename, 'w') as output:
+    with open(filename, "w") as output:
         json.dump(cookie, output)
-        
 
-def extract_to_markdown(html_source:str) -> str:
+
+def extract_to_markdown(html_source: str) -> str:
     """
     Extracts markdown content from the given HTML source.
-    
+
     Args:
         html_source (str): The HTML source code from which to extract markdown content.
-        
+
     Returns:
         str: The extracted markdown content from the HTML source.
     """
     output = []
     in_table = False
     code_block = []
-    for line in html_source.split('\n'):
+    for line in html_source.split("\n"):
         line = line.strip()
-        if line.startswith('<pre>'):
-            output.append('```\n')
+        if line.startswith("<pre>"):
+            output.append("```\n")
             code_block = []
-        elif line.startswith('</pre>'):
-            code_block.append(line.replace('</pre>', ''))
-            code = unescape('\n'.join(code_block))
-            output.append(code + '\n')
-            output.append('```\n\n')
+        elif line.startswith("</pre>"):
+            code_block.append(line.replace("</pre>", ""))
+            code = unescape("\n".join(code_block))
+            output.append(code + "\n")
+            output.append("```\n\n")
             code_block = []
-        elif line.startswith('<table'):
+        elif line.startswith("<table"):
             table_lines = [line]
             in_table = True
-        elif in_table and line.startswith('</table>'):
+        elif in_table and line.startswith("</table>"):
             table_lines.append(line)
-            table = '\n'.join(table_lines)
-            output.append(table + '\n\n')
+            table = "\n".join(table_lines)
+            output.append(table + "\n\n")
             in_table = False
         elif in_table:
             table_lines.append(line)
         else:
-            text = re.sub(r'<[^>]+>', '', line)
+            text = re.sub(r"<[^>]+>", "", line)
             if text:
-                output.append(text + '\n')
-    return ''.join(output).strip().strip(r'\n')
+                output.append(text + "\n")
+    return "".join(output).strip().strip(r"\n")
```

### Comparing `groqon-0.1.2/PKG-INFO` & `groqon-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: groqon
-Version: 0.1.2
+Version: 0.1.3
 Summary: Use Groq.com as llm
 Author: tikendraw
 Author-email: tikendraksahu1029@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Description-Content-Type: text/markdown
 
-# GROQ without API
+# GROQ without API : GroqOn
 
 This projects uses playwright to Access [GROQ](https://www.groq.com) using python
 
 ## Inspiration(Story)
-On a long summer evening of april 2023 I was sitting in front of cranky old fan working on my [News-app](https://www.github.com/tikendraw/news-app). I needed a llm api to summarize the news articles. As a poor man I do not have money to buy llm subscription, I chose to use [Gemini](https://gemini.google.com) (limit 1 req/sec), it took avg 8-9 sec per request to process, felt dissapointed.
+On a long summer evening of april 2024 I was sitting in front of cranky old fan working on my [News-app](https://www.github.com/tikendraw/news-app). I needed a llm api to summarize the news articles. As a poor man I do not have money to buy llm subscription, I chose to use [Gemini](https://gemini.google.com) (limit 1 req/sec), it took avg 8-9 sec per request to process, felt dissapointed.
 
 At this point I have heard about Groq and its new LPU hardware that outputs insanely fast. 
 There wasn't any free api for poor people like me. So I decided to emulate the user using playwright and can query and get the llm response. Finally as the thousands of seconds passed I could manage to make it work. Now you can use groq.com as llm too. I did it for poor people. 
 
 ## Working
 
 * It emulates user using playwright and queries the selected model and ouputs the response as a json object.
@@ -89,20 +89,25 @@
   --cookie_file COOKIE_FILE
   --headless            set true to not see the browser
   --save_output         set true to save the groq output with its query name.json
   --output_dir OUTPUT_DIR
                         Path to save the output file. Defaults to current working directory.
 ```
 
-## TODO
+## TODO (Need Help)
 
 * [x] Set System Prompt
 * [ ] Keep updated
 * [ ] Add something
 * [ ] Use Better parser
-* [ ] Use color for better Visual /Rich text formatting
+* [ ] Use color for better Visual / Rich text formatting
 * [ ] Add logger
 * [ ] Multiround chat
 
 ## Contribution
 
 Feel free to add features and keep it maintained and do pull requests.
+
+## Buy me a Coffee/Chai
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoffee.com/tikendraw)
+
+
```

