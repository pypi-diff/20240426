# Comparing `tmp/dev_assistant_client-0.2.51.tar.gz` & `tmp/dev_assistant_client-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev_assistant_client-0.2.51.tar", max compression
+gzip compressed data, was "dev_assistant_client-0.2.7.tar", max compression
```

## Comparing `dev_assistant_client-0.2.51.tar` & `dev_assistant_client-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,17 @@
--rw-r--r--   0        0        0     1091 2024-04-26 08:12:29.895088 dev_assistant_client-0.2.51/LICENSE
--rw-r--r--   0        0        0     5264 2024-04-26 08:12:29.895088 dev_assistant_client-0.2.51/README.md
--rw-r--r--   0        0        0       56 2024-04-26 08:12:29.895088 dev_assistant_client-0.2.51/dev_assistant_client/__init__.py
--rw-r--r--   0        0        0     5430 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/ably_handler.py
--rw-r--r--   0        0        0     2288 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/api_client.py
--rw-r--r--   0        0        0     2775 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/cli.py
--rw-r--r--   0        0        0     2887 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/client.py
--rw-r--r--   0        0        0     1879 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/client_auth.py
--rw-r--r--   0        0        0      140 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/config.py
--rw-r--r--   0        0        0     3672 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/dev_assistant_client.py
--rw-r--r--   0        0        0   108867 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/icon.ico
--rw-r--r--   0        0        0     6160 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/io.py
--rw-r--r--   0        0        0     8885 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/modules/files.py
--rw-r--r--   0        0        0     3228 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/modules/files_test.py
--rw-r--r--   0        0        0     6946 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/modules/git.py
--rw-r--r--   0        0        0     6881 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/modules/terminal.py
--rw-r--r--   0        0        0     5043 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/dev_assistant_client/utils.py
--rw-r--r--   0        0        0      957 2024-04-26 08:12:29.899088 dev_assistant_client-0.2.51/pyproject.toml
--rw-r--r--   0        0        0     6476 1970-01-01 00:00:00.000000 dev_assistant_client-0.2.51/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3919 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/README.md
+-rw-r--r--   0        0        0       20 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/__init__.py
+-rw-r--r--   0        0        0     2277 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/ably_handler.py
+-rw-r--r--   0        0        0     1709 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/api_client.py
+-rw-r--r--   0        0        0     1405 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/auth.py
+-rw-r--r--   0        0        0     1891 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/cli.py
+-rw-r--r--   0        0        0      380 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/config.py
+-rw-r--r--   0        0        0     1677 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/dev_assistant_client.py
+-rw-r--r--   0        0        0     3226 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/device.py
+-rw-r--r--   0        0        0     5052 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/io.py
+-rw-r--r--   0        0        0     3761 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/modules/files.py
+-rw-r--r--   0        0        0     4314 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/modules/git.py
+-rw-r--r--   0        0        0      736 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/modules/terminal.py
+-rw-r--r--   0        0        0     2012 2023-09-12 04:15:59.843905 dev_assistant_client-0.2.7/dev_assistant_client/utils.py
+-rw-r--r--   0        0        0      725 2023-09-12 04:15:59.847905 dev_assistant_client-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     4643 1970-01-01 00:00:00.000000 dev_assistant_client-0.2.7/PKG-INFO
```

### Comparing `dev_assistant_client-0.2.51/README.md` & `dev_assistant_client-0.2.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,118 +1,107 @@
+Metadata-Version: 2.1
+Name: dev-assistant-client
+Version: 0.2.7
+Summary: Dev Assistant client
+Author: Luciano T.
+Author-email: tonetlds@gmail.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ably (>=2.0.1,<3.0.0)
+Requires-Dist: asyncio (>=3.4.3,<4.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: gitpython (>=3.1.35,<4.0.0)
+Requires-Dist: inquirer (>=3.1.3,<4.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: rich (>=13.5.2,<14.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: unidiff (>=0.7.5,<0.8.0)
+Description-Content-Type: text/markdown
+
 # Dev Assistant
 
-Welcome to the [Dev Assistant](https://devassistant.tonet.dev) project.
+Welcome to the [Dev Assistant](https://devassistant.tonet.dev) plugin for ChatGPT.
 
 ## What is it?
 
-[Dev Assistant](https://devassistant.tonet.dev) is a *GPTs*, a ([tailored version of ChatGPT](https://openai.com/chatgpt#do-more-with-gpts)) that can assist developers by executing tasks directly in our development environment. GPTs are a new way for anyone to create a tailored version of ChatGPT to be more helpful in their daily life, at specific tasks, at work, or at home. For more information about GPTs, please refer to [OpenAI's blog post](https://openai.com/blog/introducing-gpts).
+[Dev Assistant](https://devassistant.tonet.dev) is a plugin for ChatGPT that assists us developers by executing tasks directly on our devices.
 
-This repository contains the Dev Assistant CLI, a Python package that serves as the core component of the project. It receives instructions from Dev Assistant GPT, executes them locally, and sends the response back.
+Dev Assistant Client (this repo) is a Python package that is basically the core component of the project. It receives instructions from ChatGPT via Dev Assistant plugin, executes it on any of your devices and send the response back.
 
 ## Features
 
-Dev Assistant CLI is designed to streamline your development process by offering a range of functionalities:
+The Dev Assistant Local Client is designed to streamline your development process by offering a range of functionalities:
 
-- **File Management**: Create, read, update, and delete files. List the contents of a directory. You can manage your files without leaving your conversation with Dev Assistant GPT.
+- **File Management**: Create, read, update, and delete files. List the contents of a directory. You can manage your files without leaving your conversation with ChatGPT.
 
-- **Git Version Control**: Initialize a Git repository, add changes to the staging area, commit changes, and push changes to a remote repository. Get the status of the Git repository. You can manage your Git repositories directly through Dev Assistant GPT.
+- **Git Version Control**: Initialize a Git repository, add changes to the staging area, commit changes, and push changes to a remote repository. Get the status of the Git repository. You can manage your Git repositories directly through ChatGPT.
 
-- **Terminal Commands Execution**: Execute commands directly in the terminal. You can run any command in your terminal directly from Dev Assistant GPT.
+- **Terminal Commands Execution**: Execute commands directly in the terminal. You can run any command in your terminal directly from ChatGPT.
 
 ## Requirements
 
-- 📓 Python 3.10+
-- 📓 Pip and Poetry
-- 💸 ChatGPT Plus subscription _(for custom GPTs access)_
-- ⭐ [Dev Assistant account](https://devassistant.tonet.dev)
+- 👌🏼 Python 3.6+
+- 👌🏼 pip
+- 💸 ChatGPT Plus subscription _(for plugins store access)_
 
 ## Installation
 
 - Create a Dev Assistant account at [devassistant.tonet.dev](https://devassistant.tonet.dev)
-- Generate a token at [https://devassistant.tonet.dev/user/api-tokens](https://devassistant.tonet.dev/user/api-tokens) for Dev Assistant GPT and save it. You will need it later.
+- Generate a token at [https://devassistant.tonet.dev/user/api-tokens](https://devassistant.tonet.dev/user/api-tokens) for ChatGPT and save it. You'll need it later.
 - Install the local client:
   - [Install Python](https://www.python.org/downloads/)
-  - Run `pip install dev-assistant-client` in your terminal
+  - [Install pip](https://pip.pypa.io/en/stable/)
+  - Run `pip install dev-assistant-client` in your terminal  
+- Install the ChatGPT plugin:
+  - On the [ChatGPT Plugins Store](https://chat.openai.com/plugins), click in the **"Install an unverified plugin"** at bottom of Plugin store dialog window, paste the <https://devassistant.tonet.dev> and click on "Find plugin".
+  - ChatGPT will ask you to enter your credentials. Insert the token generated in the second step and click "Install plugin".
+  - Enable the plugin in the list of installed plugins and you're good to go!
 
 ## Usage
 
 Once installed, just run the following:
 
 ```bash
 dev-assistant
 ```
 
-If the CLI is not already authenticated, it will open a browser window where you will be provided with a token. Copy the token including the pipe, and return to the terminal.
+You will be prompted to enter your email and password, if you're not already logged in. Once authenticated, the client will automatically establish a connection with the server.
 
-If everything runs well, you will see the Dev Assistant CLI presentation and a unique _CLIENT ID_, like this:
+If everything runs well, you will see the Dev Assistant CLI presentation and a exclusive _Device ID_, like this:
 
 ```
+# dev-assistant
 
-        ╭─────╮   Dev Assistant
-        │ >_< │   v0.2.46
-        ╰─────╯   https://devassistant.tonet.dev
-
-›       Connecting...           Connected!
-›       CLIENT ID:              6a35a11c-f34e-4e30-be46-a9ac4d0f5ac7
-›       WebSockets...           Connected!
-›       Private channel...      Connected!
-›       Ready!  Listening for instructions...
-›       
-
+    .-----.   Dev Assistant
+    | >_< |   v0.1.28
+    '-----'   https://devassistant.tonet.dev
+
+31/07/2023 00:43:19     Connecting...
+31/07/2023 00:43:20     Connected.      Device ID 654c5jf7-7993-4b44-ae92-ec51t88339cd
+...
 ```
 
-You can stop the client just doing a `CRTL+C` in the terminal at any time.
-
-## Commands
-
-Go to [Dev Assistant GPT](https://chat.openai.com/g/g-Qa01WfuKG-dev-assistant) and start a conversation. You can ask for help with the commands, or just let Dev Assistant GPT discover it by itself. It will ask you to login if you are not already logged in.
-
-You can now ask Dev Assistant GPT to do things like:
-
-- Create a new file called `my-file.txt` on my Desktop
-- Read a file called `other-file.yml`
-- Update a file
-- Delete a file
-- List the contents of a directory
-- Initialize a Git repository
-- Add changes to the staging area
-- Commit changes
-- Push changes to a remote repository
-- Get the status of the Git repository
-- Execute a command in the terminal
-... and more!
+You can now ask ChatGPT to help you directly on that device.
 
-## Versioning
+You can do `CRTL+C` to stop the client at any time.
 
-To update the version of the package, follow these steps:
+To log out, use:
 
-1. Commit your changes with a descriptive message.
-2. Create a git tag with the format `vX.Y.Z` where `X.Y.Z` is the new version number.
-3. Push your changes and the new tag to the repository.
+```bash
+dev-assistant logout
+```
 
-The GitHub Actions workflow will automatically deploy the new version to PyPi when a new tag is detected.
+This command will remove your saved authentication token, ensuring your security.
 
 ## Contributing
 
 We welcome contributions! If you have an idea for an improvement or have found a bug, please open an issue. Feel free to fork the repository and submit a pull request if you'd like to contribute code. Please follow the code style and conventions used in the existing codebase.
 
-## Development
-
-- Fork the repository
-- Clone your fork
-- Go to the project folder
-- Install Dev Assistant Client in local mode with `pip install -e .` or `poetry install`
-- Run `dev-assistant` in your terminal to start the CLI. You can use poetry to run the CLI with `poetry run dev-assistant`
-- Make your changes
-- Test your changes
-- Commit your changes
-- Push your changes
-- Open a pull request
-- 🎉
-
 ## License
 
 The Dev Assistant Local Client is open-source software, licensed under the [MIT license](LICENSE).
 
 ## Support
 
 If you encounter any problems or have any questions, don't hesitate to open an issue on GitHub. We're here to help!
@@ -121,8 +110,9 @@
 
 A big thank you to all contributors and users for your support! We couldn't do it without you.
 
 ## Authors
 
 - [Luciano T.](https://github.com/lucianotonet)
 - [ChatGPT](https://chat.openai.com/)
-- [Cursor.so](https://cursor.so/)
+- [GitHub Copilot](https://copilot.github.com/)
+
```

### Comparing `dev_assistant_client-0.2.51/dev_assistant_client/api_client.py` & `dev_assistant_client-0.2.7/dev_assistant_client/api_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,47 @@
-import os
-import requests
-import json
-from urllib.parse import urlparse
-
-from .utils import read_token
-
-class APIClient:
-    def __init__(self, base_url, cert_file=None, key_file=None, token=None, verify=None):
-        parsed_url = urlparse(base_url)
-        self.host = parsed_url.hostname
-        self.port = parsed_url.port
-        self.base_url = base_url.rstrip('/')  # Remove trailing slash if present
-        self.cert_file = cert_file
-        self.key_file = key_file
-        self.token = token or read_token()
-        self.headers = {
-            "Content-type": "application/json",
-            "Accept": "application/json",
-            "User-Agent": "DevAssistantCLI",
-            "Authorization": f"Bearer {self.token}" if self.token else None
-        }
-        app_env = os.environ.get("APP_ENV")
-        self.verify = verify if verify is not None else (False if app_env and app_env.lower() != "production" else True)
-    
-    def _make_request(self, method, endpoint, data=None) -> requests.Response | None:
-        
-        # if endpoint starts with https:// or http://, use that as the base url
-        if endpoint.startswith("https://") or endpoint.startswith("http://"):
-            self.base_url = endpoint
-            endpoint = ""
-               
-        url = self.base_url + endpoint
-        payload = json.dumps(data) if data else None
-        
-        cert = (self.cert_file, self.key_file) if self.cert_file and self.key_file else None
-        response = None
-        try:
-            response = requests.request(method, url, data=payload, headers=self.headers, cert=cert, verify=self.verify)
-        except Exception as e:
-            print(e)
-            return None
-        
-        return response   
-            
-    def get(self, endpoint) -> requests.Response | None:
-        return self._make_request("GET", endpoint)
-    
-    def post(self, endpoint, data=None) -> requests.Response | None:
-        return self._make_request("POST", endpoint, data)
-    
-    def put(self, endpoint, data=None) -> requests.Response | None:
-        return self._make_request("PUT", endpoint, data)
-    
-    def delete(self, endpoint) -> requests.Response | None:
-        return self._make_request("DELETE", endpoint)
+import requests
+import json
+from urllib.parse import urlparse
+
+from dev_assistant_client.utils import dd
+
+class APIClient:
+    def __init__(self, base_url, cert_file=None, key_file=None, token=None):
+        parsed_url = urlparse(base_url)
+        self.host = parsed_url.hostname
+        self.port = parsed_url.port
+        self.base_url = base_url.rstrip('/')  # Remove trailing slash if present
+        self.cert_file = cert_file
+        self.key_file = key_file
+        self.token = token
+        self.headers = {
+            "Content-type": "application/json",
+            "Accept": "application/json",
+            "User-Agent": "DevAssistantClient/0.2",
+            "Authorization": f"Bearer {self.token}" if self.token else None
+        }
+    
+    def _make_request(self, method, endpoint, data=None):
+        
+        # if endpoint starts with https:// or http://, use that as the base url
+        if endpoint.startswith("https://") or endpoint.startswith("http://"):
+            self.base_url = endpoint
+            endpoint = ""
+               
+        url = self.base_url + endpoint
+        payload = json.dumps(data) if data else None
+        
+        response = requests.request(method, url, data=payload, headers=self.headers, cert=(self.cert_file, self.key_file))
+        
+        return response        
+            
+    def get(self, endpoint):
+        return self._make_request("GET", endpoint)
+    
+    def post(self, endpoint, data=None):
+        return self._make_request("POST", endpoint, data)
+    
+    def put(self, endpoint, data=None):
+        return self._make_request("PUT", endpoint, data)
+    
+    def delete(self, endpoint):
+        return self._make_request("DELETE", endpoint)
```

