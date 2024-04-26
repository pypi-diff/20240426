# Comparing `tmp/chat_bot_sea-0.0.0.tar.gz` & `tmp/chat_bot_sea-0.0.1.tar.gz`

## Comparing `chat_bot_sea-0.0.0.tar` & `chat_bot_sea-0.0.1.tar`

### file list

```diff
@@ -1,39 +1,30 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/__init__.py
--rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/config/__init__.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/config/asgi.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/config/settings.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/config/urls.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/config/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/bot_read_url.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/download_drive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/__init__.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/func.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/gcp.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/matching_v1.py
--rw-r--r--   0        0        0    10411 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/matching_v2.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/testing/__init__.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/testing/adhoc_v1.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/read_news/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/read_news/news.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/read_news/rag_web_vi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/admin.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/apps.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/function_interactive.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/function_user.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/models.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/services.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/views.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/migrations/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/requirements.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/__init__.py
+-rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/manage.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/config/asgi.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/config/settings.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/config/urls.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/config/wsgi.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/bot_read_url.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/download_drive.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/build_index/func.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/build_index/gcp.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/build_index/matching_v1.py
+-rw-r--r--   0        0        0    10411 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/build_index/matching_v2.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/build_index/model.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/testing/adhoc_v1.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/read_news/news.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/read_news/rag_web_vi.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/admin.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/apps.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/function_interactive.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/function_user.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/models.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/services.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/views.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/README.md
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 chat_bot_sea-0.0.1/PKG-INFO
```

### Comparing `chat_bot_sea-0.0.0/src/manage.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/manage.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/config/settings.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/config/settings.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/download_drive.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/download_drive.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/func.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/build_index/func.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/gcp.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/build_index/gcp.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/matching_v1.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/build_index/matching_v1.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/matching_v2.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/build_index/matching_v2.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/build_index/model.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/build_index/model.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/item_match/testing/adhoc_v1.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/item_match/testing/adhoc_v1.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/read_news/news.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/read_news/news.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/request_functions/read_news/rag_web_vi.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/request_functions/read_news/rag_web_vi.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/function_interactive.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/function_interactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,53 +4,54 @@
     button_list = ['Read News', 'Search News', 'BD']
 
     return [
         {'element_type': 'button',
          'button': {
              'button_type': 'callback',
              'text': button,
+             'value': button
          }} for button in button_list]
 
 
 # class BotFunction:
 #     def __init__(self, group_id: str):
 
-        # def message_template(self, content: str = ''):
-        #     return {
-        #         'group_id': self.group_id,
-        #         'message': {
-        #             'tag': 'text',
-        #             'text': {
-        #                 'format': 1,  # markdown
-        #                 'content': content,
-        #             },
-        #         }
-        #     }
-
-        # def post(self, message_body: dict = None):
-        #     r = requests.post(self.end_point, json=message_body, headers=self.header)
-        #     return r
-
-        # def interact_button(self, name: str) -> dict:
-        #     return {
-        #         'element_type': 'button',
-        #         'button': {
-        #             'button_type': 'callback',
-        #             'text': name,
-        #             'value': str({
-        #                 'group_id': self.group_id,
-        #                 'type': name
-        #             })
-        #         }
-        #     }
-
-        # def interact_info(self, title: str = None, description: str = None) -> dict:
-        #     if title:
-        #         return {
-        #             'element_type': 'title',
-        #             'title': {'text': title}
-        #         }
-        #     if description:
-        #         return {
-        #             'element_type': 'description',
-        #             'description': {'text': description}
-        #         }
+    # def message_template(self, content: str = ''):
+    #     return {
+    #         'group_id': self.group_id,
+    #         'message': {
+    #             'tag': 'text',
+    #             'text': {
+    #                 'format': 1,  # markdown
+    #                 'content': content,
+    #             },
+    #         }
+    #     }
+
+    # def post(self, message_body: dict = None):
+    #     r = requests.post(self.end_point, json=message_body, headers=self.header)
+    #     return r
+
+    # def interact_button(self, name: str) -> dict:
+    #     return {
+    #         'element_type': 'button',
+    #         'button': {
+    #             'button_type': 'callback',
+    #             'text': name,
+    #             'value': str({
+    #                 'group_id': self.group_id,
+    #                 'type': name
+    #             })
+    #         }
+    #     }
+
+    # def interact_info(self, title: str = None, description: str = None) -> dict:
+    #     if title:
+    #         return {
+    #             'element_type': 'title',
+    #             'title': {'text': title}
+    #         }
+    #     if description:
+    #         return {
+    #             'element_type': 'description',
+    #             'description': {'text': description}
+    #         }
```

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/function_user.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/function_user.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/services.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/services.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,23 +26,25 @@
 
     def text(self, content: str):
         self.json = {
             **self.json,
             "message": {"tag": "text", "text": {"format": 1, "content": content}},
         }
 
-        requests.post(
+        response = requests.post(
             url=self.end_point,
             json=self.json,
             headers={
                 "Authorization": f"Bearer {self.access_token}",
                 "Content-Type": "application/json",
             },
         )
 
+        print(response.text)
+
     def interactive(self, content: [], title: str = "", description: str = "",):
         self.json = {
             **self.json,
             "message": {"tag": "interactive_message", "interactive_message": {
                 "elements": [
                     {
                         "element_type": "title",
@@ -56,23 +58,27 @@
                             "text": description
                         }
                     }if description else None,
                 ] + content
             }},
         }
 
-        requests.post(
+        print(self.json)
+
+        response = requests.post(
             url=self.end_point,
             json=self.json,
             headers={
                 "Authorization": f"Bearer {self.access_token}",
                 "Content-Type": "application/json",
             },
         )
 
+        print(response.text)
+
 
 def image_to_base64(image: str):
     with open(image, "rb") as f:
         image_byte: bytes = f.read()
 
         return base64.b64encode(image_byte).decode("utf-8")
```

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/views.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
                     # react
                     if '/start' in message:
                         send_to_group_though_app(app_name="Gau Gau", group_id=group_id).interactive(
                             title='🐶 Hello, may I can assist you today?', description='Please select your tools:', content=start_interactive())
 
                     # elif '/match' in user_message:
                     #     read_url(user_message)
+                    return Response(status=HTTP_200_OK)
                 else:
                     return Response(
                         data={'message': 'Event type not exist. Abort'}, status=HTTP_400_BAD_REQUEST)
             else:
                 return Response(
                     data={'message': 'Failed to validate the signature. Aborted'}, status=HTTP_400_BAD_REQUEST)
         else:
```

### Comparing `chat_bot_sea-0.0.0/src/chat_bot_sea/seatalk/migrations/0001_initial.py` & `chat_bot_sea-0.0.1/src/chat_bot_sea/seatalk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/.gitignore` & `chat_bot_sea-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/LICENSE` & `chat_bot_sea-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_bot_sea-0.0.0/pyproject.toml` & `chat_bot_sea-0.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chat_bot_sea"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Kevin Khang", email="kevinkhang2909@gmail.com" },
 ]
 description = "A chatbot package"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
@@ -16,12 +16,16 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["Django, chatbot"]
 dependencies = [
     'Django',
+    'djangorestframework',
+    'django-cors-headers',
+    'loguru',
+    'requests',
 ]
 
 [project.urls]
 "Homepage" = "https://git.vndev.shopee.io/xuankhang.do/chatbot"
 "Bug Tracker" = "https://git.vndev.shopee.io/xuankhang.do/chatbot/-/issues"
```

### Comparing `chat_bot_sea-0.0.0/PKG-INFO` & `chat_bot_sea-0.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: chat_bot_sea
-Version: 0.0.0
+Version: 0.0.1
 Summary: A chatbot package
 Project-URL: Homepage, https://git.vndev.shopee.io/xuankhang.do/chatbot
 Project-URL: Bug Tracker, https://git.vndev.shopee.io/xuankhang.do/chatbot/-/issues
 Author-email: Kevin Khang <kevinkhang2909@gmail.com>
 License: Copyright (c) 2023 Kevin Khang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,11 +27,15 @@
 License-File: LICENSE
 Keywords: Django, chatbot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: django
+Requires-Dist: django-cors-headers
+Requires-Dist: djangorestframework
+Requires-Dist: loguru
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # chatbot
```

