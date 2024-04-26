# Comparing `tmp/psyaitools-0.1.3.dev1.tar.gz` & `tmp/psyaitools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyaitools-0.1.3.dev1.tar", max compression
+gzip compressed data, was "psyaitools-0.1.4.tar", max compression
```

## Comparing `psyaitools-0.1.3.dev1.tar` & `psyaitools-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2024-04-19 18:30:19.184238 psyaitools-0.1.3.dev1/LICENSE
--rw-r--r--   0        0        0      928 2024-04-26 16:26:27.686146 psyaitools-0.1.3.dev1/README.md
--rw-r--r--   0        0        0     6148 2024-04-26 16:27:46.412536 psyaitools-0.1.3.dev1/psyaitools/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-26 17:38:19.164142 psyaitools-0.1.3.dev1/psyaitools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 09:29:19.590033 psyaitools-0.1.3.dev1/psyaitools/functional/IOs/__init__.py
--rw-r--r--   0        0        0     1680 2024-04-26 14:53:49.167989 psyaitools-0.1.3.dev1/psyaitools/functional/IOs/base64_wav.py
--rw-r--r--   0        0        0      434 2024-04-26 18:59:09.524676 psyaitools-0.1.3.dev1/psyaitools/functional/IOs/base64_xfccs.py
--rw-r--r--   0        0        0      234 2024-04-26 18:59:02.994265 psyaitools-0.1.3.dev1/psyaitools/functional/IOs/readFiles.py
--rw-r--r--   0        0        0        0 2024-04-26 17:36:54.161932 psyaitools-0.1.3.dev1/psyaitools/functional/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 17:37:47.798436 psyaitools-0.1.3.dev1/psyaitools/functional/ext/__init__.py
--rw-r--r--   0        0        0      997 2024-04-26 15:06:50.275222 psyaitools-0.1.3.dev1/psyaitools/functional/ext/shInst.py
--rw-r--r--   0        0        0        0 2024-04-26 17:37:24.367135 psyaitools-0.1.3.dev1/psyaitools/functional/representation/__init__.py
--rw-r--r--   0        0        0     1527 2024-04-26 16:28:20.020756 psyaitools-0.1.3.dev1/psyaitools/functional/representation/factDecomMachine.py
--rw-r--r--   0        0        0     1075 2024-04-26 17:47:56.028505 psyaitools-0.1.3.dev1/psyaitools/functional/representation/xfccs.py
--rw-r--r--   0        0        0       23 2024-04-19 18:36:31.305642 psyaitools-0.1.3.dev1/psyaitools/res/res.py
--rw-r--r--   0        0        0      437 2024-04-26 18:55:21.717263 psyaitools-0.1.3.dev1/pyproject.toml
--rw-r--r--   0        0        0     1578 1970-01-01 00:00:00.000000 psyaitools-0.1.3.dev1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-19 18:30:19.184238 psyaitools-0.1.4/LICENSE
+-rw-r--r--   0        0        0      928 2024-04-26 16:26:27.686146 psyaitools-0.1.4/README.md
+-rw-r--r--   0        0        0     6148 2024-04-26 16:27:46.412536 psyaitools-0.1.4/psyaitools/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-26 17:38:19.164142 psyaitools-0.1.4/psyaitools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:29:19.590033 psyaitools-0.1.4/psyaitools/functional/IOs/__init__.py
+-rw-r--r--   0        0        0     1680 2024-04-26 14:53:49.167989 psyaitools-0.1.4/psyaitools/functional/IOs/base64_wav.py
+-rw-r--r--   0        0        0      434 2024-04-26 18:59:09.524676 psyaitools-0.1.4/psyaitools/functional/IOs/base64_xfccs.py
+-rw-r--r--   0        0        0      234 2024-04-26 18:59:02.994265 psyaitools-0.1.4/psyaitools/functional/IOs/readFiles.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:36:54.161932 psyaitools-0.1.4/psyaitools/functional/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:37:47.798436 psyaitools-0.1.4/psyaitools/functional/ext/__init__.py
+-rw-r--r--   0        0        0      997 2024-04-26 15:06:50.275222 psyaitools-0.1.4/psyaitools/functional/ext/shInst.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:37:24.367135 psyaitools-0.1.4/psyaitools/functional/representation/__init__.py
+-rw-r--r--   0        0        0     1527 2024-04-26 16:28:20.020756 psyaitools-0.1.4/psyaitools/functional/representation/factDecomMachine.py
+-rw-r--r--   0        0        0     1075 2024-04-26 17:47:56.028505 psyaitools-0.1.4/psyaitools/functional/representation/xfccs.py
+-rw-r--r--   0        0        0       23 2024-04-19 18:36:31.305642 psyaitools-0.1.4/psyaitools/res/res.py
+-rw-r--r--   0        0        0      432 2024-04-26 19:01:17.765092 psyaitools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 psyaitools-0.1.4/PKG-INFO
```

### Comparing `psyaitools-0.1.3.dev1/LICENSE` & `psyaitools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.3.dev1/README.md` & `psyaitools-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.3.dev1/psyaitools/.DS_Store` & `psyaitools-0.1.4/psyaitools/.DS_Store`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.3.dev1/psyaitools/functional/IOs/base64_wav.py` & `psyaitools-0.1.4/psyaitools/functional/IOs/base64_wav.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.3.dev1/psyaitools/functional/ext/shInst.py` & `psyaitools-0.1.4/psyaitools/functional/ext/shInst.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.3.dev1/psyaitools/functional/representation/factDecomMachine.py` & `psyaitools-0.1.4/psyaitools/functional/representation/factDecomMachine.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.3.dev1/psyaitools/functional/representation/xfccs.py` & `psyaitools-0.1.4/psyaitools/functional/representation/xfccs.py`

 * *Files identical despite different names*

### Comparing `psyaitools-0.1.3.dev1/PKG-INFO` & `psyaitools-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyaitools
-Version: 0.1.3.dev1
+Version: 0.1.4
 Summary: Minor issues fixed
 Author: moomoofarm1
 Author-email: 46774289+moomoofarm1@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

