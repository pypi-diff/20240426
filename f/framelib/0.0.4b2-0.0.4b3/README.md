# Comparing `tmp/framelib-0.0.4b2.tar.gz` & `tmp/framelib-0.0.4b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framelib-0.0.4b2.tar", last modified: Fri Apr 26 12:51:52 2024, max compression
+gzip compressed data, was "framelib-0.0.4b3.tar", last modified: Fri Apr 26 12:54:35 2024, max compression
```

## Comparing `framelib-0.0.4b2.tar` & `framelib-0.0.4b3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:51:52.116510 framelib-0.0.4b2/
--rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 12:51:52.116510 framelib-0.0.4b2/PKG-INFO
--rw-rw-r--   0 devin     (1000) devin     (1000)     1233 2024-03-20 13:38:58.000000 framelib-0.0.4b2/README.md
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:51:52.116510 framelib-0.0.4b2/framelib/
--rw-rw-r--   0 devin     (1000) devin     (1000)      381 2024-04-26 12:10:50.000000 framelib-0.0.4b2/framelib/__init__.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     1778 2024-03-20 13:38:58.000000 framelib-0.0.4b2/framelib/frame.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3215 2024-04-26 12:51:26.000000 framelib-0.0.4b2/framelib/hub.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3067 2024-04-26 11:37:38.000000 framelib-0.0.4b2/framelib/models.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3195 2024-04-26 12:19:23.000000 framelib-0.0.4b2/framelib/neynar.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:51:52.116510 framelib-0.0.4b2/framelib/templates/
--rw-rw-r--   0 devin     (1000) devin     (1000)     2356 2024-03-13 12:40:19.000000 framelib-0.0.4b2/framelib/templates/frame.html
--rw-rw-r--   0 devin     (1000) devin     (1000)     1578 2024-03-20 13:38:58.000000 framelib-0.0.4b2/framelib/transaction.py
--rw-rw-r--   0 devin     (1000) devin     (1000)      380 2024-02-26 15:07:40.000000 framelib-0.0.4b2/framelib/warpcast.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:51:52.116510 framelib-0.0.4b2/framelib.egg-info/
--rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 12:51:52.000000 framelib-0.0.4b2/framelib.egg-info/PKG-INFO
--rw-rw-r--   0 devin     (1000) devin     (1000)      431 2024-04-26 12:51:52.000000 framelib-0.0.4b2/framelib.egg-info/SOURCES.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)        1 2024-04-26 12:51:52.000000 framelib-0.0.4b2/framelib.egg-info/dependency_links.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       83 2024-04-26 12:51:52.000000 framelib-0.0.4b2/framelib.egg-info/requires.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       14 2024-04-26 12:51:52.000000 framelib-0.0.4b2/framelib.egg-info/top_level.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       38 2024-04-26 12:51:52.116510 framelib-0.0.4b2/setup.cfg
--rw-rw-r--   0 devin     (1000) devin     (1000)      917 2024-04-26 12:51:45.000000 framelib-0.0.4b2/setup.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:51:52.116510 framelib-0.0.4b2/test/
--rw-rw-r--   0 devin     (1000) devin     (1000)        0 2024-02-26 19:53:14.000000 framelib-0.0.4b2/test/__init__.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     3316 2024-03-20 13:38:58.000000 framelib-0.0.4b2/test/test_render.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     5252 2024-03-20 13:38:58.000000 framelib-0.0.4b2/test/test_transaction.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     2675 2024-04-26 12:48:58.000000 framelib-0.0.4b2/test/test_validation.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:54:35.853853 framelib-0.0.4b3/
+-rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 12:54:35.853853 framelib-0.0.4b3/PKG-INFO
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1233 2024-03-20 13:38:58.000000 framelib-0.0.4b3/README.md
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:54:35.853853 framelib-0.0.4b3/framelib/
+-rw-rw-r--   0 devin     (1000) devin     (1000)      381 2024-04-26 12:10:50.000000 framelib-0.0.4b3/framelib/__init__.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1778 2024-03-20 13:38:58.000000 framelib-0.0.4b3/framelib/frame.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3214 2024-04-26 12:53:55.000000 framelib-0.0.4b3/framelib/hub.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3067 2024-04-26 11:37:38.000000 framelib-0.0.4b3/framelib/models.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3195 2024-04-26 12:19:23.000000 framelib-0.0.4b3/framelib/neynar.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:54:35.853853 framelib-0.0.4b3/framelib/templates/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2356 2024-03-13 12:40:19.000000 framelib-0.0.4b3/framelib/templates/frame.html
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1578 2024-03-20 13:38:58.000000 framelib-0.0.4b3/framelib/transaction.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)      380 2024-02-26 15:07:40.000000 framelib-0.0.4b3/framelib/warpcast.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:54:35.853853 framelib-0.0.4b3/framelib.egg-info/
+-rw-r--r--   0 devin     (1000) devin     (1000)     1847 2024-04-26 12:54:35.000000 framelib-0.0.4b3/framelib.egg-info/PKG-INFO
+-rw-rw-r--   0 devin     (1000) devin     (1000)      431 2024-04-26 12:54:35.000000 framelib-0.0.4b3/framelib.egg-info/SOURCES.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)        1 2024-04-26 12:54:35.000000 framelib-0.0.4b3/framelib.egg-info/dependency_links.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       83 2024-04-26 12:54:35.000000 framelib-0.0.4b3/framelib.egg-info/requires.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       14 2024-04-26 12:54:35.000000 framelib-0.0.4b3/framelib.egg-info/top_level.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       38 2024-04-26 12:54:35.853853 framelib-0.0.4b3/setup.cfg
+-rw-rw-r--   0 devin     (1000) devin     (1000)      917 2024-04-26 12:54:29.000000 framelib-0.0.4b3/setup.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-26 12:54:35.853853 framelib-0.0.4b3/test/
+-rw-rw-r--   0 devin     (1000) devin     (1000)        0 2024-02-26 19:53:14.000000 framelib-0.0.4b3/test/__init__.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3316 2024-03-20 13:38:58.000000 framelib-0.0.4b3/test/test_render.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5252 2024-03-20 13:38:58.000000 framelib-0.0.4b3/test/test_transaction.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2675 2024-04-26 12:48:58.000000 framelib-0.0.4b3/test/test_validation.py
```

### Comparing `framelib-0.0.4b2/PKG-INFO` & `framelib-0.0.4b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framelib
-Version: 0.0.4b2
+Version: 0.0.4b3
 Summary: lightweight library for building farcaster frames using python and flask
 Home-page: https://github.com/devinaconley/python-frames
 Author: Devin A. Conley
 Author-email: devinaconley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `framelib-0.0.4b2/README.md` & `framelib-0.0.4b3/README.md`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b2/framelib/frame.py` & `framelib-0.0.4b3/framelib/frame.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b2/framelib/hub.py` & `framelib-0.0.4b3/framelib/hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,12 +84,12 @@
                     state=msg.untrustedData.state,
                     transactionId=msg.untrustedData.transactionId
                 )
             ),
             hash=msg.untrustedData.messageHash,
             hashScheme='HASH_SCHEME_BLAKE',
             signature='',
-            signature_scheme='SIGNATURE_SCHEME_ED25519',
+            signatureScheme='SIGNATURE_SCHEME_ED25519',
             signer=''
         )
 
     return validate_message(msg, hub, username=username, password=password, api_key=api_key)
```

### Comparing `framelib-0.0.4b2/framelib/models.py` & `framelib-0.0.4b3/framelib/models.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b2/framelib/neynar.py` & `framelib-0.0.4b3/framelib/neynar.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b2/framelib/templates/frame.html` & `framelib-0.0.4b3/framelib/templates/frame.html`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b2/framelib/transaction.py` & `framelib-0.0.4b3/framelib/transaction.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b2/framelib.egg-info/PKG-INFO` & `framelib-0.0.4b3/framelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framelib
-Version: 0.0.4b2
+Version: 0.0.4b3
 Summary: lightweight library for building farcaster frames using python and flask
 Home-page: https://github.com/devinaconley/python-frames
 Author: Devin A. Conley
 Author-email: devinaconley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `framelib-0.0.4b2/setup.py` & `framelib-0.0.4b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='framelib',
-    version='0.0.4b2',
+    version='0.0.4b3',
     author='Devin A. Conley',
     author_email='devinaconley@gmail.com',
     description='lightweight library for building farcaster frames using python and flask',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/devinaconley/python-frames',
     packages=setuptools.find_packages(),
```

### Comparing `framelib-0.0.4b2/test/test_render.py` & `framelib-0.0.4b3/test/test_render.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b2/test/test_transaction.py` & `framelib-0.0.4b3/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `framelib-0.0.4b2/test/test_validation.py` & `framelib-0.0.4b3/test/test_validation.py`

 * *Files identical despite different names*

