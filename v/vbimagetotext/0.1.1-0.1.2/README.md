# Comparing `tmp/vbimagetotext-0.1.1.tar.gz` & `tmp/vbimagetotext-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbimagetotext-0.1.1.tar", max compression
+gzip compressed data, was "vbimagetotext-0.1.2.tar", max compression
```

## Comparing `vbimagetotext-0.1.1.tar` & `vbimagetotext-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.1/README.md
--rw-r--r--   0        0        0      588 2024-04-21 17:37:37.224832 vbimagetotext-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.1/vbimagetotext/__init__.py
--rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.1/vbimagetotext/__main__.py
--rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.1/vbimagetotext/choice_option.py
--rw-r--r--   0        0        0     2805 2024-04-21 17:37:29.390242 vbimagetotext-0.1.1/vbimagetotext/functions.py
--rw-r--r--   0        0        0     2160 2024-04-18 21:14:46.243588 vbimagetotext-0.1.1/vbimagetotext/geminivision.py
--rw-r--r--   0        0        0     1611 2024-04-18 21:36:33.615000 vbimagetotext-0.1.1/vbimagetotext/gptvision.py
--rw-r--r--   0        0        0      306 2024-04-16 09:07:05.481819 vbimagetotext-0.1.1/vbimagetotext/main.py
--rw-r--r--   0        0        0     7791 2024-04-21 17:36:53.778457 vbimagetotext-0.1.1/vbimagetotext/prompts.py
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.2/README.md
+-rw-r--r--   0        0        0      588 2024-04-26 07:27:24.529673 vbimagetotext-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.2/vbimagetotext/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.2/vbimagetotext/__main__.py
+-rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.2/vbimagetotext/choice_option.py
+-rw-r--r--   0        0        0     3388 2024-04-26 07:17:08.395521 vbimagetotext-0.1.2/vbimagetotext/functions.py
+-rw-r--r--   0        0        0     2776 2024-04-26 07:27:12.309253 vbimagetotext-0.1.2/vbimagetotext/geminivision.py
+-rw-r--r--   0        0        0     1611 2024-04-18 21:36:33.615000 vbimagetotext-0.1.2/vbimagetotext/gptvision.py
+-rw-r--r--   0        0        0      306 2024-04-16 09:07:05.481819 vbimagetotext-0.1.2/vbimagetotext/main.py
+-rw-r--r--   0        0        0     7791 2024-04-21 17:36:53.778457 vbimagetotext-0.1.2/vbimagetotext/prompts.py
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.2/PKG-INFO
```

### Comparing `vbimagetotext-0.1.1/pyproject.toml` & `vbimagetotext-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vbimagetotext"
-version = "0.1.1"
+version = "0.1.2"
 description = "A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API"
 authors = ["vaibhavblayer <vaibhavblayer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 click = "^8.1.7"
```

### Comparing `vbimagetotext-0.1.1/vbimagetotext/choice_option.py` & `vbimagetotext-0.1.2/vbimagetotext/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.1/vbimagetotext/functions.py` & `vbimagetotext-0.1.2/vbimagetotext/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -76,25 +76,38 @@
                     *image_dicts
                 ]
             }
         ],
         "max_tokens": max_tokens
     }
 
+    message = ""
+
     response = requests.post(
         "https://api.openai.com/v1/chat/completions", headers=headers, json=payload)
 
-    message = response.json()["choices"][0]["message"]["content"]
+    if response.status_code == 200:
+        response_json = response.json()
+
+        if 'choices' in response_json and 'message' in response_json["choices"][0]:
+            message = response_json["choices"][0]["message"]["content"]
+        else:
+            console = Console()
+            console.print(
+                "Error: 'choices' or 'message' not found in the API response.", style="bold red")
+            return "Error: 'choices' or 'message' not found in the API response."
+    else:
+        console = Console()
+        console.print(
+            f"Error: API request failed with status code {response.status_code}.", style="bold red")
+        return f"Error: API request failed with status code {response.status_code}."
+
     pattern = r"```latex(.*?)```"
     matches = re.findall(pattern, message, re.DOTALL)
 
-    try:
-        pyperclip.copy(matches[0])
-    except Exception as e:
-        print(f"Error copying to clipboard: {e}")
-
     Console().print(message, style="deep_pink3")
 
-    if matches[0] is not None:
+    if matches:
+        pyperclip.copy(matches[0])
         return matches[0]
     else:
-        return f"Match not found in the response."
+        return "Match not found in the response."
```

### Comparing `vbimagetotext-0.1.1/vbimagetotext/geminivision.py` & `vbimagetotext-0.1.2/vbimagetotext/geminivision.py`

 * *Files 14% similar despite different names*

```diff
@@ -67,19 +67,37 @@
     if prompt == "prompt":
         prompt = click.prompt("Please enter your custom prompt", type=str)
 
     prompt = switch_prompt(prompt)
 
     model = genai.GenerativeModel('gemini-pro-vision')
 
-    images = [PIL.Image.open(image_name) for image_name in image]
-    response = model.generate_content(
-        [prompt, *images], stream=True, max_tokens=1000)
-    response.resolve()
+    try:
+        images = [PIL.Image.open(image_name) for image_name in image]
+    except FileNotFoundError as e:
+        console = Console()
+        console.print(
+            f"Error: Image file not found: {str(e)}", style="bold red")
+        return
 
     try:
-        pyperclip.copy(response.text)
+        response = model.generate_content(
+            [prompt, *images], stream=True)
+        response.resolve()
     except Exception as e:
-        print(
-            f"An error occurred while copying the text to clipboard: {str(e)}")
+        console = Console()
+        console.print(
+            f"Error: Failed to generate content: {str(e)}", style="bold red")
+        return
 
-    Console().print(response.text, style="deep_pink3")
+    try:
+        if hasattr(response, 'text'):
+            pyperclip.copy(response.text)
+            Console().print(response.text, style="deep_pink3")
+        else:
+            console = Console()
+            console.print(
+                "Error: 'text' not found in the response.", style="bold red")
+    except Exception as e:
+        console = Console()
+        console.print(
+            f"An error occurred while copying the text to clipboard: {str(e)}", style="bold red")
```

### Comparing `vbimagetotext-0.1.1/vbimagetotext/gptvision.py` & `vbimagetotext-0.1.2/vbimagetotext/gptvision.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.1/vbimagetotext/prompts.py` & `vbimagetotext-0.1.2/vbimagetotext/prompts.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.1/PKG-INFO` & `vbimagetotext-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbimagetotext
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API
 Author: vaibhavblayer
 Author-email: vaibhavblayer@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

