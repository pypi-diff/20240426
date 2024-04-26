# Comparing `tmp/framelib-0.0.4b0.tar.gz` & `tmp/framelib-0.0.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framelib-0.0.4b0.tar", last modified: Fri Apr 26 12:32:19 2024, max compression
+gzip compressed data, was "framelib-0.0.4b1.tar", last modified: Fri Apr 26 12:49:48 2024, max compression
```

## Comparing `framelib-0.0.4b0.tar` & `framelib-0.0.4b1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:32:19.457774 framelib-0.0.4b0/
--rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 12:32:19.457774 framelib-0.0.4b0/PKG-INFO
--rw-rw-r--   0 devin     (1000) devin     (1000)     1233 2024-03-20 13:38:58.000000 framelib-0.0.4b0/README.md
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:32:19.457774 framelib-0.0.4b0/framelib/
--rw-rw-r--   0 devin     (1000) devin     (1000)      381 2024-04-26 12:10:50.000000 framelib-0.0.4b0/framelib/__init__.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     1778 2024-03-20 13:38:58.000000 framelib-0.0.4b0/framelib/frame.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3043 2024-04-26 12:14:45.000000 framelib-0.0.4b0/framelib/hub.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3067 2024-04-26 11:37:38.000000 framelib-0.0.4b0/framelib/models.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3195 2024-04-26 12:19:23.000000 framelib-0.0.4b0/framelib/neynar.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:32:19.457774 framelib-0.0.4b0/framelib/templates/
--rw-rw-r--   0 devin     (1000) devin     (1000)     2356 2024-03-13 12:40:19.000000 framelib-0.0.4b0/framelib/templates/frame.html
--rw-rw-r--   0 devin     (1000) devin     (1000)     1578 2024-03-20 13:38:58.000000 framelib-0.0.4b0/framelib/transaction.py
--rw-rw-r--   0 devin     (1000) devin     (1000)      380 2024-02-26 15:07:40.000000 framelib-0.0.4b0/framelib/warpcast.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:32:19.457774 framelib-0.0.4b0/framelib.egg-info/
--rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 12:32:19.000000 framelib-0.0.4b0/framelib.egg-info/PKG-INFO
--rw-rw-r--   0 devin     (1000) devin     (1000)      431 2024-04-26 12:32:19.000000 framelib-0.0.4b0/framelib.egg-info/SOURCES.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)        1 2024-04-26 12:32:19.000000 framelib-0.0.4b0/framelib.egg-info/dependency_links.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       83 2024-04-26 12:32:19.000000 framelib-0.0.4b0/framelib.egg-info/requires.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       14 2024-04-26 12:32:19.000000 framelib-0.0.4b0/framelib.egg-info/top_level.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       38 2024-04-26 12:32:19.457774 framelib-0.0.4b0/setup.cfg
--rw-rw-r--   0 devin     (1000) devin     (1000)      917 2024-04-26 12:30:57.000000 framelib-0.0.4b0/setup.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:32:19.457774 framelib-0.0.4b0/test/
--rw-rw-r--   0 devin     (1000) devin     (1000)        0 2024-02-26 19:53:14.000000 framelib-0.0.4b0/test/__init__.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3316 2024-03-20 13:38:58.000000 framelib-0.0.4b0/test/test_render.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     5252 2024-03-20 13:38:58.000000 framelib-0.0.4b0/test/test_transaction.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     2673 2024-04-26 11:37:38.000000 framelib-0.0.4b0/test/test_validation.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:49:48.463480 framelib-0.0.4b1/
+-rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 12:49:48.463480 framelib-0.0.4b1/PKG-INFO
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1233 2024-03-20 13:38:58.000000 framelib-0.0.4b1/README.md
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:49:48.459480 framelib-0.0.4b1/framelib/
+-rw-rw-r--   0 devin     (1000) devin     (1000)      381 2024-04-26 12:10:50.000000 framelib-0.0.4b1/framelib/__init__.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1778 2024-03-20 13:38:58.000000 framelib-0.0.4b1/framelib/frame.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3208 2024-04-26 12:47:44.000000 framelib-0.0.4b1/framelib/hub.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3067 2024-04-26 11:37:38.000000 framelib-0.0.4b1/framelib/models.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3195 2024-04-26 12:19:23.000000 framelib-0.0.4b1/framelib/neynar.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:49:48.459480 framelib-0.0.4b1/framelib/templates/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2356 2024-03-13 12:40:19.000000 framelib-0.0.4b1/framelib/templates/frame.html
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1578 2024-03-20 13:38:58.000000 framelib-0.0.4b1/framelib/transaction.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)      380 2024-02-26 15:07:40.000000 framelib-0.0.4b1/framelib/warpcast.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:49:48.463480 framelib-0.0.4b1/framelib.egg-info/
+-rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 12:49:48.000000 framelib-0.0.4b1/framelib.egg-info/PKG-INFO
+-rw-rw-r--   0 devin     (1000) devin     (1000)      431 2024-04-26 12:49:48.000000 framelib-0.0.4b1/framelib.egg-info/SOURCES.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)        1 2024-04-26 12:49:48.000000 framelib-0.0.4b1/framelib.egg-info/dependency_links.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       83 2024-04-26 12:49:48.000000 framelib-0.0.4b1/framelib.egg-info/requires.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       14 2024-04-26 12:49:48.000000 framelib-0.0.4b1/framelib.egg-info/top_level.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       38 2024-04-26 12:49:48.463480 framelib-0.0.4b1/setup.cfg
+-rw-rw-r--   0 devin     (1000) devin     (1000)      917 2024-04-26 12:48:13.000000 framelib-0.0.4b1/setup.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:49:48.463480 framelib-0.0.4b1/test/
+-rw-rw-r--   0 devin     (1000) devin     (1000)        0 2024-02-26 19:53:14.000000 framelib-0.0.4b1/test/__init__.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3316 2024-03-20 13:38:58.000000 framelib-0.0.4b1/test/test_render.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5252 2024-03-20 13:38:58.000000 framelib-0.0.4b1/test/test_transaction.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2675 2024-04-26 12:48:58.000000 framelib-0.0.4b1/test/test_validation.py
```

### Comparing `framelib-0.0.4b0/PKG-INFO` & `framelib-0.0.4b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framelib
-Version: 0.0.4b0
+Version: 0.0.4b1
 Summary: lightweight library for building farcaster frames using python and flask
 Home-page: https://github.com/devinaconley/python-frames
 Author: Devin A. Conley
 Author-email: devinaconley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `framelib-0.0.4b0/README.md` & `framelib-0.0.4b1/README.md`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b0/framelib/frame.py` & `framelib-0.0.4b1/framelib/frame.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b0/framelib/hub.py` & `framelib-0.0.4b1/framelib/hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,23 +56,30 @@
 
     if msg.untrustedData.state is not None and msg.untrustedData.state != action.data.frameActionBody.state:
         raise ValueError(f'state does not match: {msg.untrustedData.state} {action.data.frameActionBody.state}')
 
     return action
 
 
-def validate_message_or_mock(msg: FrameMessage, api_key: str, mock: bool = False) -> ValidatedMessage:
+def validate_message_or_mock(
+        msg: FrameMessage,
+        hub: str,
+        username: str = None,
+        password: str = None,
+        api_key: str = None,
+        mock: bool = False
+) -> ValidatedMessage:
     if mock:
         # mock
         return ValidatedMessage(
             data=ValidatedData(
                 type='MESSAGE_TYPE_FRAME_ACTION',
                 fid=msg.untrustedData.fid,
                 timestamp=msg.untrustedData.timestamp,
-                network=msg.untrustedData.network,
+                network=str(msg.untrustedData.network),
                 frameActionBody=FrameAction(
                     url=msg.untrustedData.url,
                     buttonIndex=msg.untrustedData.buttonIndex,
                     castId=msg.untrustedData.castId,
                     inputTest=msg.untrustedData.inputText,
                     state=msg.untrustedData.state,
                     transactionId=msg.untrustedData.transactionId
@@ -81,10 +88,8 @@
             hash=msg.untrustedData.hash,
             hashScheme='HASH_SCHEME_BLAKE',
             signature='',
             signature_scheme='SIGNATURE_SCHEME_ED25519',
             signer=''
         )
 
-    return validate_message(msg, api_key)
-
-
+    return validate_message(msg, hub, username=username, password=password, api_key=api_key)
```

### Comparing `framelib-0.0.4b0/framelib/models.py` & `framelib-0.0.4b1/framelib/models.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b0/framelib/neynar.py` & `framelib-0.0.4b1/framelib/neynar.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b0/framelib/templates/frame.html` & `framelib-0.0.4b1/framelib/templates/frame.html`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b0/framelib/transaction.py` & `framelib-0.0.4b1/framelib/transaction.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b0/framelib.egg-info/PKG-INFO` & `framelib-0.0.4b1/framelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framelib
-Version: 0.0.4b0
+Version: 0.0.4b1
 Summary: lightweight library for building farcaster frames using python and flask
 Home-page: https://github.com/devinaconley/python-frames
 Author: Devin A. Conley
 Author-email: devinaconley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `framelib-0.0.4b0/setup.py` & `framelib-0.0.4b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='framelib',
-    version='0.0.4b0',
+    version='0.0.4b1',
     author='Devin A. Conley',
     author_email='devinaconley@gmail.com',
     description='lightweight library for building farcaster frames using python and flask',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/devinaconley/python-frames',
     packages=setuptools.find_packages(),
```

### Comparing `framelib-0.0.4b0/test/test_render.py` & `framelib-0.0.4b1/test/test_render.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b0/test/test_transaction.py` & `framelib-0.0.4b1/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b0/test/test_validation.py` & `framelib-0.0.4b1/test/test_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 """
 
 # lib
 import pytest
 
 # src
 from framelib import validate_message
-from framelib.neynar import get_frame_action
+from framelib.neynar import get_frame_message
 from framelib.hub import get_message
 
 
 class TestValidateMessageNeynar(object):
 
     def test_button_1(self):
         # example signed message from fid 8268 clicking button 1
         msg = '0a4e080d10cc4018cbe1a230200182013f0a2068747470733a2f2f707974686f6e2d6672616d652e76657263656c2e6170702f10011a1908cc401214000000000000000000000000000000000000000112140101bf04a2e61cb24c9a66c047ac5ed175e1bed8180122403feee9d0c1392c1e5bc7bca49850f83735c53b4f60c88959ffc271123e333a196e963d15619125e6034acda36076c709182daa5625e4affe6df21866c204830828013220ad4520314a78bc4317c604a3324ebc25bd8215c3ac38342fd790b7905c291bd1'
-        action = get_frame_action(msg, 'NEYNAR_API_DOCS')
+        action = get_frame_message(msg, 'NEYNAR_API_DOCS')
         assert action.tapped_button.index == 1
         assert action.interactor.fid == 8268
         assert action.input is None
 
 
 class TestValidateMessageHub(object):
```

