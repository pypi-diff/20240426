# Comparing `tmp/framelib-0.0.3b2.tar.gz` & `tmp/framelib-0.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framelib-0.0.3b2.tar", last modified: Tue Mar 19 02:33:04 2024, max compression
+gzip compressed data, was "framelib-0.0.4b0.tar", last modified: Fri Apr 26 12:32:19 2024, max compression
```

## Comparing `framelib-0.0.3b2.tar` & `framelib-0.0.4b0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-03-19 02:33:04.112505 framelib-0.0.3b2/
--rw-r--r--   0 devin     (1000) devin     (1000)     1677 2024-03-19 02:33:04.112505 framelib-0.0.3b2/PKG-INFO
--rw-rw-r--   0 devin     (1000) devin     (1000)     1063 2024-03-07 03:10:47.000000 framelib-0.0.3b2/README.md
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-03-19 02:33:04.108505 framelib-0.0.3b2/framelib/
--rw-rw-r--   0 devin     (1000) devin     (1000)      280 2024-03-18 03:26:19.000000 framelib-0.0.3b2/framelib/__init__.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     1778 2024-03-18 03:25:18.000000 framelib-0.0.3b2/framelib/frame.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     2605 2024-03-18 05:25:25.000000 framelib-0.0.3b2/framelib/models.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3367 2024-03-18 05:32:18.000000 framelib-0.0.3b2/framelib/neynar.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-03-19 02:33:04.112505 framelib-0.0.3b2/framelib/templates/
--rw-rw-r--   0 devin     (1000) devin     (1000)     2356 2024-03-07 03:43:55.000000 framelib-0.0.3b2/framelib/templates/frame.html
--rw-rw-r--   0 devin     (1000) devin     (1000)     1578 2024-03-19 02:25:55.000000 framelib-0.0.3b2/framelib/transaction.py
--rw-rw-r--   0 devin     (1000) devin     (1000)      380 2024-03-07 03:10:47.000000 framelib-0.0.3b2/framelib/warpcast.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-03-19 02:33:04.112505 framelib-0.0.3b2/framelib.egg-info/
--rw-r--r--   0 devin     (1000) devin     (1000)     1677 2024-03-19 02:33:04.000000 framelib-0.0.3b2/framelib.egg-info/PKG-INFO
--rw-rw-r--   0 devin     (1000) devin     (1000)      415 2024-03-19 02:33:04.000000 framelib-0.0.3b2/framelib.egg-info/SOURCES.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)        1 2024-03-19 02:33:04.000000 framelib-0.0.3b2/framelib.egg-info/dependency_links.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       83 2024-03-19 02:33:04.000000 framelib-0.0.3b2/framelib.egg-info/requires.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       14 2024-03-19 02:33:04.000000 framelib-0.0.3b2/framelib.egg-info/top_level.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       38 2024-03-19 02:33:04.112505 framelib-0.0.3b2/setup.cfg
--rw-rw-r--   0 devin     (1000) devin     (1000)      917 2024-03-19 02:27:39.000000 framelib-0.0.3b2/setup.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-03-19 02:33:04.112505 framelib-0.0.3b2/test/
--rw-rw-r--   0 devin     (1000) devin     (1000)        0 2024-03-07 03:10:47.000000 framelib-0.0.3b2/test/__init__.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3316 2024-03-18 03:32:04.000000 framelib-0.0.3b2/test/test_render.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     5252 2024-03-19 02:24:43.000000 framelib-0.0.3b2/test/test_transaction.py
--rw-rw-r--   0 devin     (1000) devin     (1000)      906 2024-03-17 16:40:49.000000 framelib-0.0.3b2/test/test_validation.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:32:19.457774 framelib-0.0.4b0/
+-rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 12:32:19.457774 framelib-0.0.4b0/PKG-INFO
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1233 2024-03-20 13:38:58.000000 framelib-0.0.4b0/README.md
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:32:19.457774 framelib-0.0.4b0/framelib/
+-rw-rw-r--   0 devin     (1000) devin     (1000)      381 2024-04-26 12:10:50.000000 framelib-0.0.4b0/framelib/__init__.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1778 2024-03-20 13:38:58.000000 framelib-0.0.4b0/framelib/frame.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3043 2024-04-26 12:14:45.000000 framelib-0.0.4b0/framelib/hub.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3067 2024-04-26 11:37:38.000000 framelib-0.0.4b0/framelib/models.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3195 2024-04-26 12:19:23.000000 framelib-0.0.4b0/framelib/neynar.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:32:19.457774 framelib-0.0.4b0/framelib/templates/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2356 2024-03-13 12:40:19.000000 framelib-0.0.4b0/framelib/templates/frame.html
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1578 2024-03-20 13:38:58.000000 framelib-0.0.4b0/framelib/transaction.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)      380 2024-02-26 15:07:40.000000 framelib-0.0.4b0/framelib/warpcast.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:32:19.457774 framelib-0.0.4b0/framelib.egg-info/
+-rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 12:32:19.000000 framelib-0.0.4b0/framelib.egg-info/PKG-INFO
+-rw-rw-r--   0 devin     (1000) devin     (1000)      431 2024-04-26 12:32:19.000000 framelib-0.0.4b0/framelib.egg-info/SOURCES.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)        1 2024-04-26 12:32:19.000000 framelib-0.0.4b0/framelib.egg-info/dependency_links.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       83 2024-04-26 12:32:19.000000 framelib-0.0.4b0/framelib.egg-info/requires.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       14 2024-04-26 12:32:19.000000 framelib-0.0.4b0/framelib.egg-info/top_level.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       38 2024-04-26 12:32:19.457774 framelib-0.0.4b0/setup.cfg
+-rw-rw-r--   0 devin     (1000) devin     (1000)      917 2024-04-26 12:30:57.000000 framelib-0.0.4b0/setup.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:32:19.457774 framelib-0.0.4b0/test/
+-rw-rw-r--   0 devin     (1000) devin     (1000)        0 2024-02-26 19:53:14.000000 framelib-0.0.4b0/test/__init__.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3316 2024-03-20 13:38:58.000000 framelib-0.0.4b0/test/test_render.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5252 2024-03-20 13:38:58.000000 framelib-0.0.4b0/test/test_transaction.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2673 2024-04-26 11:37:38.000000 framelib-0.0.4b0/test/test_validation.py
```

### Comparing `framelib-0.0.3b2/PKG-INFO` & `framelib-0.0.4b0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framelib
-Version: 0.0.3b2
+Version: 0.0.4b0
 Summary: lightweight library for building farcaster frames using python and flask
 Home-page: https://github.com/devinaconley/python-frames
 Author: Devin A. Conley
 Author-email: devinaconley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,38 +21,41 @@
 lightweight library for building farcaster frames using python and flask
 
 - easily render frames that conform to the farcaster specification
 - configurable frame design
 - parse frame action messages
 - verify the frame action signatures using neynar
 - query user profile info from warpcast
+- on-chain frame transactions
 
 
 ## quickstart
 
 install `framelib` from pip
 ```
 pip install framelib
 ```
 
 simple example
 ```python
 from flask import Flask, url_for
-from framelib import render_frame
+from framelib import frame
 
 app = Flask(__name__)
 
 @app.route('/')
 def home():
-    return render_frame(
+    return frame(
         image='https://opengraph.githubassets.com/0x/devinaconley/python-frames',
         button1='next',
         post_url=url_for('second_page', _external=True),
     )
 ```
 
 ## examples
 
 see a complete example using python + flask + vercel [here](https://github.com/devinaconley/python-frames/tree/main/examples/simple)
 
+for an example that uses on-chain frame transactions, see the [weth frame](https://github.com/devinaconley/python-frames/tree/main/examples/transaction)
+
 and for a more advanced example involving multiplayer games, supabase integration, dynamic image rendering, and more,
 see [rock paper scissors](https://github.com/devinaconley/rock-paper-scissors)
```

### Comparing `framelib-0.0.3b2/README.md` & `framelib-0.0.4b0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,38 +3,41 @@
 lightweight library for building farcaster frames using python and flask
 
 - easily render frames that conform to the farcaster specification
 - configurable frame design
 - parse frame action messages
 - verify the frame action signatures using neynar
 - query user profile info from warpcast
+- on-chain frame transactions
 
 
 ## quickstart
 
 install `framelib` from pip
 ```
 pip install framelib
 ```
 
 simple example
 ```python
 from flask import Flask, url_for
-from framelib import render_frame
+from framelib import frame
 
 app = Flask(__name__)
 
 @app.route('/')
 def home():
-    return render_frame(
+    return frame(
         image='https://opengraph.githubassets.com/0x/devinaconley/python-frames',
         button1='next',
         post_url=url_for('second_page', _external=True),
     )
 ```
 
 ## examples
 
 see a complete example using python + flask + vercel [here](https://github.com/devinaconley/python-frames/tree/main/examples/simple)
 
+for an example that uses on-chain frame transactions, see the [weth frame](https://github.com/devinaconley/python-frames/tree/main/examples/transaction)
+
 and for a more advanced example involving multiplayer games, supabase integration, dynamic image rendering, and more,
 see [rock paper scissors](https://github.com/devinaconley/rock-paper-scissors)
```

### Comparing `framelib-0.0.3b2/framelib/frame.py` & `framelib-0.0.4b0/framelib/frame.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.3b2/framelib/models.py` & `framelib-0.0.4b0/framelib/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,27 +10,31 @@
 # ---- frame message ----
 
 class CastId(BaseModel):
     fid: int
     hash: str
 
 
-class UntrustedData(BaseModel):
-    fid: int
+class FrameAction(BaseModel):
     url: str
-    messageHash: str
-    timestamp: int
-    network: int
     buttonIndex: int
     inputText: Optional[str] = None
     state: Optional[str] = None
     transactionId: Optional[str] = None
     castId: CastId
 
 
+class UntrustedData(FrameAction):
+    # note: this untrusted message seems to collapse the ValidatedDate and FrameAction fields
+    fid: int
+    messageHash: str
+    timestamp: int
+    network: int
+
+
 class TrustedData(BaseModel):
     messageBytes: str
 
 
 class FrameMessage(BaseModel):
     untrustedData: UntrustedData
     trustedData: TrustedData
@@ -47,14 +51,33 @@
 
 class Transaction(BaseModel):
     chainId: str
     method: Literal['eth_sendTransaction']
     params: EthTransactionParams
 
 
+# ---- hub ----
+
+class ValidatedData(BaseModel):
+    type: str
+    fid: int
+    timestamp: datetime.datetime
+    network: str
+    frameActionBody: FrameAction
+
+
+class ValidatedMessage(BaseModel):
+    data: ValidatedData
+    hash: str
+    hashScheme: str
+    signature: str
+    signatureScheme: str
+    signer: str
+
+
 # ---- neynar ----
 
 class NeynarViewer(BaseModel):
     following: bool
     followed_by: bool
 
 
@@ -63,15 +86,15 @@
     mentioned_profiles: Optional[list[str]] = []
 
 
 class NeynarProfile(BaseModel):
     bio: NeynarBio
 
 
-class Interactor(BaseModel):
+class NeynarInteractor(BaseModel):
     object: str
     fid: int
     username: str
     display_name: str
     custody_address: Optional[str] = None
     pfp_url: str
     profile: NeynarProfile
@@ -96,17 +119,17 @@
     serialized: str
 
 
 class NeynarTransaction(BaseModel):
     hash: str
 
 
-class ValidatedMessage(BaseModel):
+class NeynarValidatedMessage(BaseModel):
     object: str
-    interactor: Interactor
+    interactor: NeynarInteractor
     tapped_button: NeynarButton
     input: Optional[NeynarInput] = None
     state: Optional[NeynarState] = None
     url: str
     cast: dict
     timestamp: datetime.datetime
     transaction: Optional[NeynarTransaction] = None
```

### Comparing `framelib-0.0.3b2/framelib/neynar.py` & `framelib-0.0.4b0/framelib/neynar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 methods to call neynar api
 """
-import os
 
+# lib
+import os
 import requests
 
-from .models import FrameMessage, ValidatedMessage, Interactor, NeynarProfile, NeynarBio, NeynarButton, NeynarInput, \
-    NeynarState, NeynarTransaction
+# src
+from .models import FrameMessage, NeynarValidatedMessage, NeynarInteractor, NeynarProfile, NeynarBio, \
+    NeynarButton, NeynarInput, NeynarState, NeynarTransaction
 
 
-def get_frame_action(msg: str, api_key: str) -> ValidatedMessage:
+def get_frame_message(msg: str, api_key: str) -> NeynarValidatedMessage:
     if not api_key:
         raise ValueError('neynar api key not set')
     url = 'https://api.neynar.com/v2/farcaster/frame/validate'
     body = {
         'cast_reaction_context': False,  # TODO
         'follow_context': False,
         'signer_context': False,
@@ -26,21 +28,21 @@
     }
     res = requests.post(url, json=body, headers=headers)
 
     body = res.json()
     if not body['valid']:
         raise ValueError('frame action message is invalid')
 
-    action = ValidatedMessage(**body['action'])
+    action = NeynarValidatedMessage(**body['action'])
 
     return action
 
 
-def validate_message(msg: FrameMessage, api_key: str) -> ValidatedMessage:
-    action = get_frame_action(msg.trustedData.messageBytes, api_key)
+def validate_message(msg: FrameMessage, api_key: str) -> NeynarValidatedMessage:
+    action = get_frame_message(msg.trustedData.messageBytes, api_key)
 
     if msg.untrustedData.fid != action.interactor.fid:
         raise ValueError(f'fid does not match: {msg.untrustedData.fid} {action.interactor.fid}')
 
     if msg.untrustedData.buttonIndex != action.tapped_button.index:
         raise ValueError(f'button index does not match: {msg.untrustedData.buttonIndex} {action.tapped_button.index}')
 
@@ -49,21 +51,21 @@
 
     if msg.untrustedData.state is not None and msg.untrustedData.state != action.state.serialized:
         raise ValueError(f'state does not match: {msg.untrustedData.state} {action.state.serialized}')
 
     return action
 
 
-def validate_message_or_mock(msg: FrameMessage, api_key: str, mock: bool = False) -> ValidatedMessage:
+def validate_message_or_mock(msg: FrameMessage, api_key: str, mock: bool = False) -> NeynarValidatedMessage:
     if mock:
         # mock
         # TODO option to populate with warpcast profile
-        return ValidatedMessage(
+        return NeynarValidatedMessage(
             object='validated_frame_action',
-            interactor=Interactor(
+            interactor=NeynarInteractor(
                 object='user',
                 fid=msg.untrustedData.fid,
                 username=f'username {msg.untrustedData.fid}',
                 display_name=f'display name {msg.untrustedData.fid}',
                 pfp_url='',
                 profile=NeynarProfile(bio=NeynarBio(text='')),
                 follower_count=0,
@@ -77,12 +79,7 @@
             transaction=NeynarTransaction(hash=msg.untrustedData.transactionId or ''),
             url=msg.untrustedData.url,
             timestamp=msg.untrustedData.timestamp,
             cast={}
         )
 
     return validate_message(msg, api_key)
-
-
-def validate_message_or_mock_vercel(msg: FrameMessage, api_key: str) -> ValidatedMessage:
-    vercel_env = os.getenv('VERCEL_ENV')
-    return validate_message_or_mock(msg, api_key, vercel_env is None or vercel_env == 'development')
```

### Comparing `framelib-0.0.3b2/framelib/templates/frame.html` & `framelib-0.0.4b0/framelib/templates/frame.html`

 * *Files identical despite different names*

### Comparing `framelib-0.0.3b2/framelib/transaction.py` & `framelib-0.0.4b0/framelib/transaction.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.3b2/framelib.egg-info/PKG-INFO` & `framelib-0.0.4b0/framelib.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framelib
-Version: 0.0.3b2
+Version: 0.0.4b0
 Summary: lightweight library for building farcaster frames using python and flask
 Home-page: https://github.com/devinaconley/python-frames
 Author: Devin A. Conley
 Author-email: devinaconley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,38 +21,41 @@
 lightweight library for building farcaster frames using python and flask
 
 - easily render frames that conform to the farcaster specification
 - configurable frame design
 - parse frame action messages
 - verify the frame action signatures using neynar
 - query user profile info from warpcast
+- on-chain frame transactions
 
 
 ## quickstart
 
 install `framelib` from pip
 ```
 pip install framelib
 ```
 
 simple example
 ```python
 from flask import Flask, url_for
-from framelib import render_frame
+from framelib import frame
 
 app = Flask(__name__)
 
 @app.route('/')
 def home():
-    return render_frame(
+    return frame(
         image='https://opengraph.githubassets.com/0x/devinaconley/python-frames',
         button1='next',
         post_url=url_for('second_page', _external=True),
     )
 ```
 
 ## examples
 
 see a complete example using python + flask + vercel [here](https://github.com/devinaconley/python-frames/tree/main/examples/simple)
 
+for an example that uses on-chain frame transactions, see the [weth frame](https://github.com/devinaconley/python-frames/tree/main/examples/transaction)
+
 and for a more advanced example involving multiplayer games, supabase integration, dynamic image rendering, and more,
 see [rock paper scissors](https://github.com/devinaconley/rock-paper-scissors)
```

### Comparing `framelib-0.0.3b2/setup.py` & `framelib-0.0.4b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='framelib',
-    version='0.0.3b2',
+    version='0.0.4b0',
     author='Devin A. Conley',
     author_email='devinaconley@gmail.com',
     description='lightweight library for building farcaster frames using python and flask',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/devinaconley/python-frames',
     packages=setuptools.find_packages(),
```

### Comparing `framelib-0.0.3b2/test/test_render.py` & `framelib-0.0.4b0/test/test_render.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.3b2/test/test_transaction.py` & `framelib-0.0.4b0/test/test_transaction.py`

 * *Files identical despite different names*

