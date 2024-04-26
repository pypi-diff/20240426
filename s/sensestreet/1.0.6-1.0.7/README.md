# Comparing `tmp/sensestreet-1.0.6.tar.gz` & `tmp/sensestreet-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensestreet-1.0.6.tar", last modified: Wed Apr 24 07:29:32 2024, max compression
+gzip compressed data, was "sensestreet-1.0.7.tar", last modified: Fri Apr 26 12:59:17 2024, max compression
```

## Comparing `sensestreet-1.0.6.tar` & `sensestreet-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-24 07:29:32.518621 sensestreet-1.0.6/
--rw-rw-r--   0 michalg   (1001) michalg   (1001)    11327 2023-06-21 13:47:45.000000 sensestreet-1.0.6/LICENSE
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     4047 2024-04-24 07:29:32.518621 sensestreet-1.0.6/PKG-INFO
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     3778 2024-04-24 07:26:03.000000 sensestreet-1.0.6/README.md
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      103 2024-04-24 07:29:32.518621 sensestreet-1.0.6/setup.cfg
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      649 2024-04-24 07:27:45.000000 sensestreet-1.0.6/setup.py
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-24 07:29:32.514621 sensestreet-1.0.6/src/
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-24 07:29:32.514621 sensestreet-1.0.6/src/sensestreet/
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      108 2024-04-24 07:26:03.000000 sensestreet-1.0.6/src/sensestreet/__init__.py
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     5628 2024-04-24 07:26:03.000000 sensestreet-1.0.6/src/sensestreet/anonymise.py
--rw-rw-r--   0 michalg   (1001) michalg   (1001)    11899 2024-04-24 07:27:45.000000 sensestreet-1.0.6/src/sensestreet/sensestreet_client.py
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-24 07:29:32.518621 sensestreet-1.0.6/src/sensestreet.egg-info/
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     4047 2024-04-24 07:29:32.000000 sensestreet-1.0.6/src/sensestreet.egg-info/PKG-INFO
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      325 2024-04-24 07:29:32.000000 sensestreet-1.0.6/src/sensestreet.egg-info/SOURCES.txt
--rw-rw-r--   0 michalg   (1001) michalg   (1001)        1 2024-04-24 07:29:32.000000 sensestreet-1.0.6/src/sensestreet.egg-info/dependency_links.txt
--rw-rw-r--   0 michalg   (1001) michalg   (1001)       28 2024-04-24 07:29:32.000000 sensestreet-1.0.6/src/sensestreet.egg-info/requires.txt
--rw-rw-r--   0 michalg   (1001) michalg   (1001)       12 2024-04-24 07:29:32.000000 sensestreet-1.0.6/src/sensestreet.egg-info/top_level.txt
+drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-26 12:59:17.351953 sensestreet-1.0.7/
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)    11327 2023-06-21 13:47:45.000000 sensestreet-1.0.7/LICENSE
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)     4047 2024-04-26 12:59:17.351953 sensestreet-1.0.7/PKG-INFO
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)     3778 2024-04-24 07:26:03.000000 sensestreet-1.0.7/README.md
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)      103 2024-04-26 12:59:17.355953 sensestreet-1.0.7/setup.cfg
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)      686 2024-04-26 12:57:22.000000 sensestreet-1.0.7/setup.py
+drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-26 12:59:17.343954 sensestreet-1.0.7/src/
+drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-26 12:59:17.351953 sensestreet-1.0.7/src/sensestreet/
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)      108 2024-04-24 07:26:03.000000 sensestreet-1.0.7/src/sensestreet/__init__.py
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)     5628 2024-04-26 12:54:47.000000 sensestreet-1.0.7/src/sensestreet/anonymise.py
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)    12370 2024-04-26 12:57:22.000000 sensestreet-1.0.7/src/sensestreet/sensestreet_client.py
+drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-26 12:59:17.351953 sensestreet-1.0.7/src/sensestreet.egg-info/
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)     4047 2024-04-26 12:59:17.000000 sensestreet-1.0.7/src/sensestreet.egg-info/PKG-INFO
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)      325 2024-04-26 12:59:17.000000 sensestreet-1.0.7/src/sensestreet.egg-info/SOURCES.txt
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)        1 2024-04-26 12:59:17.000000 sensestreet-1.0.7/src/sensestreet.egg-info/dependency_links.txt
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)       39 2024-04-26 12:59:17.000000 sensestreet-1.0.7/src/sensestreet.egg-info/requires.txt
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)       12 2024-04-26 12:59:17.000000 sensestreet-1.0.7/src/sensestreet.egg-info/top_level.txt
```

### Comparing `sensestreet-1.0.6/LICENSE` & `sensestreet-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sensestreet-1.0.6/PKG-INFO` & `sensestreet-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensestreet
-Version: 1.0.6
+Version: 1.0.7
 Summary: UNKNOWN
 Home-page: https://sensestreet.com
 Author: Sense Street
 Author-email: engineering@sensestreet.com
 License: Apache
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `sensestreet-1.0.6/README.md` & `sensestreet-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sensestreet-1.0.6/setup.py` & `sensestreet-1.0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='sensestreet',
-    version='1.0.6',
+    version='1.0.7',
     license='Apache',
     packages=find_packages('src'),
     author="Sense Street",
     author_email="engineering@sensestreet.com",
     url="https://sensestreet.com",
     package_dir={'': 'src'},
     install_requires=[
           'requests',
           'PyJWT',
-          'cryptography'
+          'cryptography',
+          'lxml',
+          'Faker'
       ],
     long_description=long_description,
     long_description_content_type='text/markdown'
 
 )
```

### Comparing `sensestreet-1.0.6/src/sensestreet/anonymise.py` & `sensestreet-1.0.7/src/sensestreet/anonymise.py`

 * *Files identical despite different names*

### Comparing `sensestreet-1.0.6/src/sensestreet/sensestreet_client.py` & `sensestreet-1.0.7/src/sensestreet/sensestreet_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,211 +27,250 @@
     api_url: str
         Url of the api to use with the client.
     priv_key_path: str, optional
         Path to the private key.
     pub_key_id: str, optional
         Id of the public key.
     server_id: str, optional,
-        Id of the server 
+        Id of the server
     req_timeout_sec: int, optional
-        After how many seconds the request will time out. 
+        After how many seconds the request will time out.
     pub_key_path: str, optional
-        Path to the public key. 
+        Path to the public key.
     extra_headers: dict
         Extra headers to use when making requests.
     request_args: dict
         Extra arguments to use when making requests.
-   
+
 
     Methods
     -------
     ping():
         Sends a ping. Useful for testing network connectivity.
 
     ping_auth():
         Sends an authorised ping.
 
     predict_rfqs(conversation, options):
         Predicts RFQs from input converstaion.
-    
+
     chat_snippet_predict_rfqs(chat_snippet, options):
         Predicts RFQs from chat snippet.
 
     upload_files_with_conversations(files_paths):
         Uploads files with conversations for processing.
 
     upload_file_with_bond_ref_data(file_path):
         Uploads files with information about bonds.
 
     get_processed_conv_file(file_id, output_file_path):
         Download processed conversations.
 
     get_conv_file_status(file_id):
         Check if conversations sent in file with the file_id have already been processed.
-    
-    
+
+
 
     """
-    __version__ = "1.0.6"
 
-    def __init__(self, app_id, api_url, priv_key_path=None, pub_key_id='default.pub', server_id='default', 
-            req_timeout_sec=500, pub_key_path=None, extra_headers=None, request_args=None):
+    __version__ = "1.0.7"
+
+    def __init__(
+        self,
+        app_id,
+        api_url,
+        priv_key_path=None,
+        pub_key_id="default.pub",
+        server_id="default",
+        req_timeout_sec=500,
+        pub_key_path=None,
+        extra_headers=None,
+        request_args=None,
+    ):
         self.api_url = self._prepare_api_url(api_url)
         self.app_id = app_id
         self.server_id = server_id
         self.pub_key_id = pub_key_id
-        self.auth_key = self._load_rsa_private_key(priv_key_path) if priv_key_path else None
+        self.auth_key = (
+            self._load_rsa_private_key(priv_key_path) if priv_key_path else None
+        )
         self.last_token_meta = None
         self.last_token = None
         self.req_timeout_sec = req_timeout_sec
-        self.extra_headers=extra_headers
+        self.extra_headers = extra_headers
         self.pub_key = self._get_pub_key(pub_key_path)
 
         if isinstance(request_args, dict):
-            forbidded_keys = {"url", "timeout", "headers"} 
+            forbidded_keys = {"url", "timeout", "headers"}
             if forbidded_keys_found := forbidded_keys & set(request_args.keys()):
-                raise ValueError(f"Not allowed request arguments found {forbidded_keys_found}")
+                raise ValueError(
+                    f"Not allowed request arguments found {forbidded_keys_found}"
+                )
 
             self.request_args = request_args
         else:
             self.request_args = {}
 
     def ping(self):
-        """ Sends a ping. Useful for testing network connectivity.
-        """
+        """Sends a ping. Useful for testing network connectivity."""
         ping_url = f"{self.api_url}/ping"
-        res = requests.get(url=ping_url, timeout=self.req_timeout_sec, headers=self._get_headers(), **self.request_args)
+        res = requests.get(
+            url=ping_url,
+            timeout=self.req_timeout_sec,
+            headers=self._get_headers(),
+            **self.request_args,
+        )
         res.raise_for_status()
         res_json = json.loads(res.text)
         return res_json
 
     def ping_auth(self):
-        """ Sends an authorised ping.
-            Once bare ping works, it's useful for testing authorisation.
+        """Sends an authorised ping.
+        Once bare ping works, it's useful for testing authorisation.
         """
         ping_auth_url = f"{self.api_url}/ping_auth"
-        res = requests.get(url=ping_auth_url, headers=self._get_headers(), timeout=self.req_timeout_sec, **self.request_args)
+        res = requests.get(
+            url=ping_auth_url,
+            headers=self._get_headers(),
+            timeout=self.req_timeout_sec,
+            **self.request_args,
+        )
         res.raise_for_status()
         res_json = json.loads(res.text)
         return res_json
 
     def predict_rfqs(self, conversation, options=None):
-        """ Predict RFQs from input converstaion.
-            Input must be valid conversation dict.
+        """Predict RFQs from input converstaion.
+        Input must be valid conversation dict.
         """
         predict_rfqs_url = f"{self.api_url}/predict_rfqs"
         flags = options or {}
-        conversation_json = conversation if isinstance(conversation, dict) else json.loads(conversation)
-        json_payload = {
-            "conv": conversation_json,
-            "flags": flags
-        }
-        res = requests.post(json=json_payload, url=predict_rfqs_url, headers=self._get_headers(), timeout=self.req_timeout_sec, **self.request_args)
+        conversation_json = (
+            conversation if isinstance(conversation, dict) else json.loads(conversation)
+        )
+        json_payload = {"conv": conversation_json, "flags": flags}
+        res = requests.post(
+            json=json_payload,
+            url=predict_rfqs_url,
+            headers=self._get_headers(),
+            timeout=self.req_timeout_sec,
+            **self.request_args,
+        )
         res.raise_for_status()
         res_json = json.loads(res.text)
         return res_json
 
     def chat_snippet_predict_rfqs(self, chat_snippet, options=None):
-        """ Predict RFQs from chat snippet.
-            Input must be valid conversation dict.
+        """Predict RFQs from chat snippet.
+        Input must be valid conversation dict.
         """
         predict_rfqs_url = f"{self.api_url}/predict_chat_snippet_rfqs"
         flags = options or {}
-        conversation_json = chat_snippet if isinstance(chat_snippet, dict) else json.loads(chat_snippet)
-        json_payload = {
-            "chat_snippet": conversation_json,
-            "flags": flags
-        }
-        res = requests.post(json=json_payload, url=predict_rfqs_url, headers=self._get_headers(), timeout=self.req_timeout_sec, **self.request_args)
+        conversation_json = (
+            chat_snippet if isinstance(chat_snippet, dict) else json.loads(chat_snippet)
+        )
+        json_payload = {"chat_snippet": conversation_json, "flags": flags}
+        res = requests.post(
+            json=json_payload,
+            url=predict_rfqs_url,
+            headers=self._get_headers(),
+            timeout=self.req_timeout_sec,
+            **self.request_args,
+        )
         res.raise_for_status()
         res_json = json.loads(res.text)
         return res_json
 
     def upload_files_with_conversations(self, files_paths):
-        """ Uploads list of files with conversations to be processed by the server.
-        """
+        """Uploads list of files with conversations to be processed by the server."""
         conv_upload_url = f"{self.api_url}/conversations"
         if not isinstance(files_paths, list):
-            raise RuntimeError("Please provide list of filenames even if you're sending just one file")
+            raise RuntimeError(
+                "Please provide list of filenames even if you're sending just one file"
+            )
             return
         files = []
         auth_headers = self._get_headers(True)
         for file_path in files_paths:
             file = pathlib.Path(file_path)
-            files.append(('files', file.open('rb')))
-        
-        resp = requests.post(url=conv_upload_url, files=files, headers=auth_headers, **self.request_args) 
+            files.append(("files", file.open("rb")))
+
+        resp = requests.post(
+            url=conv_upload_url, files=files, headers=auth_headers, **self.request_args
+        )
         return resp.json()
 
     def upload_file_with_bond_ref_data(self, file_path):
-        """ Uploads file with bond data to be added to the server.
-        """
+        """Uploads file with bond data to be added to the server."""
         bond_upload_url = f"{self.api_url}/bonds"
         file = pathlib.Path(file_path)
-        resp = requests.post(url=bond_upload_url, files={"file": (file.name, file.open('rb'))}, headers=self._get_headers(True), **self.request_args) 
+        resp = requests.post(
+            url=bond_upload_url,
+            files={"file": (file.name, file.open("rb"))},
+            headers=self._get_headers(True),
+            **self.request_args,
+        )
         return resp.json()
 
     def get_processed_conv_file(self, file_id, output_file_path):
-        """ Returns file with processed conversations.
-        """
+        """Returns file with processed conversations."""
         url = f"{self.api_url}/conversations/file/{file_id}"
         get_response = requests.get(url=url, stream=True, headers=self._get_headers())
         if get_response.status_code != 200:
             return get_response.json()
-        file_name  = url.split("/")[-1]
-        with open(output_file_path, 'wb') as f:
+        file_name = url.split("/")[-1]
+        with open(output_file_path, "wb") as f:
             for chunk in get_response.iter_content(chunk_size=1024):
                 if chunk:
                     f.write(chunk)
         return f"File saved under {output_file_path+file_name}.json"
 
     def get_conv_file_status(self, file_id):
-        """ Returns status of the conversations sent in a given file for the processing by the server.
-        """
+        """Returns status of the conversations sent in a given file for the processing by the server."""
         url = f"{self.api_url}/conversations/status/{file_id}"
         resp = requests.get(url=url, headers=self._get_headers(), **self.request_args)
         return resp.json()
 
     def _get_headers(self, is_not_json=False):
         start_time = datetime.now().strftime("%m/%d/%Y, %H:%M:%S")
         head = {}
         if self.auth_key:
             token = self._get_token()
-            head['Authorization'] = 'Bearer {}'.format(token)
+            head["Authorization"] = "Bearer {}".format(token)
         if not is_not_json:
-            head['Content-Type'] = 'application/json'
+            head["Content-Type"] = "application/json"
         if self.pub_key:
-            head['X-key'] = self.pub_key
-        head['X-client-version'] = str(self.__version__)
-        head['Date'] = start_time
+            head["X-key"] = self.pub_key
+        head["X-client-version"] = str(self.__version__)
+        head["Date"] = start_time
         if isinstance(self.extra_headers, dict):
             for key, value in self.extra_headers.items():
                 head[key] = value
         return head
 
     def _get_token(self):
         if self.last_token:
             safe_time = datetime.now() + timedelta(minutes=1)
-            if self.last_token_meta['exp'] > safe_time:
+            if self.last_token_meta["exp"] > safe_time:
                 return self.last_token
         self.last_token, self.last_token_meta = self._generate_token(self.auth_key)
         return self.last_token
 
     def _generate_token(self, private_key):
         token_payload = {
             # JWT claim
-            'exp': datetime.utcnow() + timedelta(minutes=15),  # expiry
-            'nbf': datetime.utcnow() - timedelta(minutes=5),
-            'aud': 'api.sensestreet.com',  # audience
+            "exp": datetime.utcnow() + timedelta(minutes=15),  # expiry
+            "nbf": datetime.utcnow() - timedelta(minutes=5),
+            "aud": "api.sensestreet.com",  # audience
             # Custom fields
-            'application_id': self.app_id,
-            'public_key_id': self.pub_key_id,
-            'server_id': self.server_id,
-            'server_role': 'default',
-            }
+            "application_id": self.app_id,
+            "public_key_id": self.pub_key_id,
+            "server_id": self.server_id,
+            "server_role": "default",
+        }
 
         token = jwt.encode(token_payload, private_key, algorithm="RS256")
         return token, token_payload
 
     def _get_pub_key(self, pub_key_path):
         if pub_key_path:
             try:
@@ -252,66 +291,71 @@
             return url + suffix
 
     @staticmethod
     def _load_rsa_public_key(path):
         """
         Load public key in pem format.
         """
-        with open(path,'rb') as f:
+        with open(path, "rb") as f:
             public_key = f.read()
             decoded_key = public_key.decode()
-            if decoded_key[-1] == '\n':
+            if decoded_key[-1] == "\n":
                 public_key = public_key[:-1]
         return public_key
 
     @staticmethod
     def _load_rsa_private_key(path):
-        """ Load private key in pem format
-        """
-        with open(path, 'rb') as f:
+        """Load private key in pem format"""
+        with open(path, "rb") as f:
             private_key = f.read()
-        if b'BEGIN OPENSSH PRIVATE' in private_key and b'END OPENSSH PRIVATE' in private_key:
+        if (
+            b"BEGIN OPENSSH PRIVATE" in private_key
+            and b"END OPENSSH PRIVATE" in private_key
+        ):
             private_key_openssh = serialization.load_ssh_private_key(private_key, None)
             private_key_rsa = private_key_openssh.private_bytes(
-                    encoding=serialization.Encoding.PEM,
-                    format=serialization.PrivateFormat.TraditionalOpenSSL,
-                    encryption_algorithm=serialization.NoEncryption()
-                    )
+                encoding=serialization.Encoding.PEM,
+                format=serialization.PrivateFormat.TraditionalOpenSSL,
+                encryption_algorithm=serialization.NoEncryption(),
+            )
             return private_key_rsa
-        elif b'BEGIN RSA PRIVATE' in private_key and b'END RSA PRIVATE' in private_key:
+        elif b"BEGIN RSA PRIVATE" in private_key and b"END RSA PRIVATE" in private_key:
             return private_key
-        raise RuntimeError(f"Key in '{path}' is not stored in supported format. Must be either RSA (.pem) or OPENSSH format. ")
-
+        raise RuntimeError(
+            f"Key in '{path}' is not stored in supported format. Must be either RSA (.pem) or OPENSSH format. "
+        )
 
     @staticmethod
     def dict2conv(messages):
-        """ A simple util function for generating a conversation dict from simple list of dicts. 
-        """
+        """A simple util function for generating a conversation dict from simple list of dicts."""
         tstamp = datetime.utcnow().isoformat()
         conv = {
             "chat_id": f"{tstamp}Z_auto",
             "participants": [
                 {
                     "login_name": "CLIENT",
                     "role": "Client",
                     "company_name": "CLIENT FIRM",
                     "first_name": "Client",
-                    "last_name": "One"
+                    "last_name": "One",
                 },
                 {
                     "login_name": "BANK",
                     "role": "Bank",
                     "company_name": "Bank Name",
                     "first_name": "Bank",
-                    "last_name": "One"
-                }
+                    "last_name": "One",
+                },
             ],
             "msgs": [
                 {
                     "msg_id": str(idx),
                     "content": str(list(msg.values())[0]),
                     "message_time_utc": tstamp,
-                    "login_name": "BANK" if str(list(msg.keys())[0]).upper()=="BANK" else "CLIENT"
-                } for idx, msg in enumerate(messages)
+                    "login_name": "BANK"
+                    if str(list(msg.keys())[0]).upper() == "BANK"
+                    else "CLIENT",
+                }
+                for idx, msg in enumerate(messages)
             ],
         }
         return conv
```

### Comparing `sensestreet-1.0.6/src/sensestreet.egg-info/PKG-INFO` & `sensestreet-1.0.7/src/sensestreet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensestreet
-Version: 1.0.6
+Version: 1.0.7
 Summary: UNKNOWN
 Home-page: https://sensestreet.com
 Author: Sense Street
 Author-email: engineering@sensestreet.com
 License: Apache
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

