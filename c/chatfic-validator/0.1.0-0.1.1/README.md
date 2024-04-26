# Comparing `tmp/chatfic_validator-0.1.0.tar.gz` & `tmp/chatfic_validator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\2-Dev\1-Projects\0-python\chatfic-validator-python\dist\.tmp-od9jl4d8\chatfic_validator-0.1.0.tar", last modified: Tue Apr 23 17:22:17 2024, max compression
+gzip compressed data, was "D:\2-Dev\1-Projects\0-python\chatfic-validator-python\dist\.tmp-ykpbmfp1\chatfic_validator-0.1.1.tar", last modified: Fri Apr 26 07:45:54 2024, max compression
```

## Comparing `chatfic_validator-0.1.0.tar` & `chatfic_validator-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:22:16.993445 chatfic_validator-0.1.0/
--rw-rw-rw-   0        0        0    35821 2024-04-23 16:40:19.000000 chatfic_validator-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2370 2024-04-23 17:22:16.992432 chatfic_validator-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1839 2024-04-23 17:09:49.000000 chatfic_validator-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 17:22:16.975204 chatfic_validator-0.1.0/chatfic_validator/
--rw-rw-rw-   0        0        0      197 2024-04-23 12:18:27.000000 chatfic_validator-0.1.0/chatfic_validator/__init__.py
--rw-rw-rw-   0        0        0      306 2024-04-23 13:05:28.000000 chatfic_validator-0.1.0/chatfic_validator/error.py
--rw-rw-rw-   0        0        0     1129 2024-04-23 12:56:35.000000 chatfic_validator-0.1.0/chatfic_validator/result.py
--rw-rw-rw-   0        0        0    32726 2024-04-23 16:24:09.000000 chatfic_validator-0.1.0/chatfic_validator/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:22:16.990430 chatfic_validator-0.1.0/chatfic_validator.egg-info/
--rw-rw-rw-   0        0        0     2370 2024-04-23 17:22:16.000000 chatfic_validator-0.1.0/chatfic_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2024-04-23 17:22:16.000000 chatfic_validator-0.1.0/chatfic_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:22:16.000000 chatfic_validator-0.1.0/chatfic_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-23 17:22:16.000000 chatfic_validator-0.1.0/chatfic_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 17:22:16.994436 chatfic_validator-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-04-23 17:11:18.000000 chatfic_validator-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:22:16.988430 chatfic_validator-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 15:00:21.000000 chatfic_validator-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     6981 2024-04-23 16:25:30.000000 chatfic_validator-0.1.0/tests/test_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:45:54.940033 chatfic_validator-0.1.1/
+-rw-rw-rw-   0        0        0    35821 2024-04-23 16:40:19.000000 chatfic_validator-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2370 2024-04-26 07:45:54.939032 chatfic_validator-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1839 2024-04-23 17:09:49.000000 chatfic_validator-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 07:45:54.895032 chatfic_validator-0.1.1/chatfic_validator/
+-rw-rw-rw-   0        0        0      197 2024-04-23 12:18:27.000000 chatfic_validator-0.1.1/chatfic_validator/__init__.py
+-rw-rw-rw-   0        0        0      306 2024-04-23 13:05:28.000000 chatfic_validator-0.1.1/chatfic_validator/error.py
+-rw-rw-rw-   0        0        0     1129 2024-04-23 12:56:35.000000 chatfic_validator-0.1.1/chatfic_validator/result.py
+-rw-rw-rw-   0        0        0    32726 2024-04-26 07:44:47.000000 chatfic_validator-0.1.1/chatfic_validator/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:45:54.938077 chatfic_validator-0.1.1/chatfic_validator.egg-info/
+-rw-rw-rw-   0        0        0     2370 2024-04-26 07:45:54.000000 chatfic_validator-0.1.1/chatfic_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2024-04-26 07:45:54.000000 chatfic_validator-0.1.1/chatfic_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 07:45:54.000000 chatfic_validator-0.1.1/chatfic_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-26 07:45:54.000000 chatfic_validator-0.1.1/chatfic_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 07:45:54.940033 chatfic_validator-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      777 2024-04-26 07:40:01.000000 chatfic_validator-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:45:54.935032 chatfic_validator-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 15:00:21.000000 chatfic_validator-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     6981 2024-04-23 16:25:30.000000 chatfic_validator-0.1.1/tests/test_validator.py
```

### Comparing `chatfic_validator-0.1.0/LICENSE` & `chatfic_validator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatfic_validator-0.1.0/PKG-INFO` & `chatfic_validator-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatfic-validator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for validating chatfic-format data
 Home-page: https://github.com/gokhanmeteerturk/chatfic-validator-python
 Author: Gökhan Mete Ertürk
 Author-email: 8rlvjfxsh@mozmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `chatfic_validator-0.1.0/README.md` & `chatfic_validator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chatfic_validator-0.1.0/chatfic_validator/result.py` & `chatfic_validator-0.1.1/chatfic_validator/result.py`

 * *Files identical despite different names*

### Comparing `chatfic_validator-0.1.0/chatfic_validator/validator.py` & `chatfic_validator-0.1.1/chatfic_validator/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                     )
                 )
             else:
                 character_keys.remove("name")
             if "color" in character_keys:
                 character_keys.remove("color")
             if "model" in character_keys:
-                character_keys.remove("color")
+                character_keys.remove("model")
             if character_keys:
                 errors.append(ChatficValidationError(
                     f"Alien fields in character "
                     f"'{character}': {character_keys}"))
         if "player" not in characters:
             errors.append(
                 ChatficValidationError(
```

### Comparing `chatfic_validator-0.1.0/chatfic_validator.egg-info/PKG-INFO` & `chatfic_validator-0.1.1/chatfic_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatfic-validator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for validating chatfic-format data
 Home-page: https://github.com/gokhanmeteerturk/chatfic-validator-python
 Author: Gökhan Mete Ertürk
 Author-email: 8rlvjfxsh@mozmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `chatfic_validator-0.1.0/setup.py` & `chatfic_validator-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="chatfic-validator",
-    version="0.1.0",
+    version="0.1.1",
     author="Gökhan Mete Ertürk",
     author_email="8rlvjfxsh@mozmail.com",
     description="A Python package for validating chatfic-format data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gokhanmeteerturk/chatfic-validator-python",
     packages=find_packages(),
```

### Comparing `chatfic_validator-0.1.0/tests/test_validator.py` & `chatfic_validator-0.1.1/tests/test_validator.py`

 * *Files identical despite different names*

