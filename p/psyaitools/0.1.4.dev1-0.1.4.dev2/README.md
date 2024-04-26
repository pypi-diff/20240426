# Comparing `tmp/psyaitools-0.1.4.dev1.tar.gz` & `tmp/psyaitools-0.1.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyaitools-0.1.4.dev1.tar", max compression
+gzip compressed data, was "psyaitools-0.1.4.dev2.tar", max compression
```

## Comparing `psyaitools-0.1.4.dev1.tar` & `psyaitools-0.1.4.dev2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2024-04-19 18:30:19.184238 psyaitools-0.1.4.dev1/LICENSE
--rw-r--r--   0        0        0      928 2024-04-26 16:26:27.686146 psyaitools-0.1.4.dev1/README.md
--rw-r--r--   0        0        0     6148 2024-04-26 16:27:46.412536 psyaitools-0.1.4.dev1/psyaitools/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-26 17:38:19.164142 psyaitools-0.1.4.dev1/psyaitools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 09:29:19.590033 psyaitools-0.1.4.dev1/psyaitools/functional/IOs/__init__.py
--rw-r--r--   0        0        0     1731 2024-04-26 19:14:25.227467 psyaitools-0.1.4.dev1/psyaitools/functional/IOs/base64_wav.py
--rw-r--r--   0        0        0      593 2024-04-26 19:07:57.053996 psyaitools-0.1.4.dev1/psyaitools/functional/IOs/base64_xfccs.py
--rw-r--r--   0        0        0      218 2024-04-26 19:09:46.876182 psyaitools-0.1.4.dev1/psyaitools/functional/IOs/readFiles.py
--rw-r--r--   0        0        0        0 2024-04-26 17:36:54.161932 psyaitools-0.1.4.dev1/psyaitools/functional/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 17:37:47.798436 psyaitools-0.1.4.dev1/psyaitools/functional/ext/__init__.py
--rw-r--r--   0        0        0      997 2024-04-26 15:06:50.275222 psyaitools-0.1.4.dev1/psyaitools/functional/ext/shInst.py
--rw-r--r--   0        0        0        0 2024-04-26 17:37:24.367135 psyaitools-0.1.4.dev1/psyaitools/functional/representation/__init__.py
--rw-r--r--   0        0        0     1527 2024-04-26 16:28:20.020756 psyaitools-0.1.4.dev1/psyaitools/functional/representation/factDecomMachine.py
--rw-r--r--   0        0        0     1075 2024-04-26 17:47:56.028505 psyaitools-0.1.4.dev1/psyaitools/functional/representation/xfccs.py
--rw-r--r--   0        0        0       23 2024-04-19 18:36:31.305642 psyaitools-0.1.4.dev1/psyaitools/res/res.py
--rw-r--r--   0        0        0      437 2024-04-26 19:09:25.115995 psyaitools-0.1.4.dev1/pyproject.toml
--rw-r--r--   0        0        0     1578 1970-01-01 00:00:00.000000 psyaitools-0.1.4.dev1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-19 18:30:19.184238 psyaitools-0.1.4.dev2/LICENSE
+-rw-r--r--   0        0        0      928 2024-04-26 16:26:27.686146 psyaitools-0.1.4.dev2/README.md
+-rw-r--r--   0        0        0     6148 2024-04-26 16:27:46.412536 psyaitools-0.1.4.dev2/psyaitools/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-26 17:38:19.164142 psyaitools-0.1.4.dev2/psyaitools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:29:19.590033 psyaitools-0.1.4.dev2/psyaitools/functional/IOs/__init__.py
+-rw-r--r--   0        0        0     1741 2024-04-26 19:22:07.922883 psyaitools-0.1.4.dev2/psyaitools/functional/IOs/base64_wav.py
+-rw-r--r--   0        0        0      593 2024-04-26 19:07:57.053996 psyaitools-0.1.4.dev2/psyaitools/functional/IOs/base64_xfccs.py
+-rw-r--r--   0        0        0      218 2024-04-26 19:09:46.876182 psyaitools-0.1.4.dev2/psyaitools/functional/IOs/readFiles.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:36:54.161932 psyaitools-0.1.4.dev2/psyaitools/functional/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:37:47.798436 psyaitools-0.1.4.dev2/psyaitools/functional/ext/__init__.py
+-rw-r--r--   0        0        0      997 2024-04-26 15:06:50.275222 psyaitools-0.1.4.dev2/psyaitools/functional/ext/shInst.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:37:24.367135 psyaitools-0.1.4.dev2/psyaitools/functional/representation/__init__.py
+-rw-r--r--   0        0        0     1527 2024-04-26 16:28:20.020756 psyaitools-0.1.4.dev2/psyaitools/functional/representation/factDecomMachine.py
+-rw-r--r--   0        0        0     1075 2024-04-26 17:47:56.028505 psyaitools-0.1.4.dev2/psyaitools/functional/representation/xfccs.py
+-rw-r--r--   0        0        0       23 2024-04-19 18:36:31.305642 psyaitools-0.1.4.dev2/psyaitools/res/res.py
+-rw-r--r--   0        0        0      437 2024-04-26 19:22:56.066793 psyaitools-0.1.4.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1578 1970-01-01 00:00:00.000000 psyaitools-0.1.4.dev2/PKG-INFO
```

### Comparing `psyaitools-0.1.4.dev1/LICENSE` & `psyaitools-0.1.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.4.dev1/README.md` & `psyaitools-0.1.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.4.dev1/psyaitools/.DS_Store` & `psyaitools-0.1.4.dev2/psyaitools/.DS_Store`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.4.dev1/psyaitools/functional/IOs/base64_wav.py` & `psyaitools-0.1.4.dev2/psyaitools/functional/IOs/base64_wav.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         lenx = lens - (lens % 4 if lens % 4 else 4)
         decode_string = base64.b64decode(wavStr[:lenx])
     elif method == 3:
         decode_string = base64.urlsafe_b64decode(wavStr)
     else:
         pass
     
-    with open(fileName, "wb") as wavFile:
+    with open(fileName + ".webm", "wb") as wavFile:
         wavFile.write(decode_string)
     print("The file has been converted to .webm format.")
         
 def webm2Wav(fileName, sampling_rate=None):
     
     assert isinstance(fileName, str)
     #assert isinstance(sampling_rate, int)
```

### Comparing `psyaitools-0.1.4.dev1/psyaitools/functional/IOs/base64_xfccs.py` & `psyaitools-0.1.4.dev2/psyaitools/functional/IOs/base64_xfccs.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.4.dev1/psyaitools/functional/ext/shInst.py` & `psyaitools-0.1.4.dev2/psyaitools/functional/ext/shInst.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.4.dev1/psyaitools/functional/representation/factDecomMachine.py` & `psyaitools-0.1.4.dev2/psyaitools/functional/representation/factDecomMachine.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.4.dev1/psyaitools/functional/representation/xfccs.py` & `psyaitools-0.1.4.dev2/psyaitools/functional/representation/xfccs.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.4.dev1/PKG-INFO` & `psyaitools-0.1.4.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyaitools
-Version: 0.1.4.dev1
+Version: 0.1.4.dev2
 Summary: Minor issues fixed
 Author: moomoofarm1
 Author-email: 46774289+moomoofarm1@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

