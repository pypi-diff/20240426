# Comparing `tmp/focanocodigo-1.0.0.tar.gz` & `tmp/focanocodigo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "focanocodigo-1.0.0.tar", last modified: Fri Apr 26 00:05:20 2024, max compression
+gzip compressed data, was "focanocodigo-1.0.1.tar", last modified: Fri Apr 26 00:25:57 2024, max compression
```

## Comparing `focanocodigo-1.0.0.tar` & `focanocodigo-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 00:05:20.837847 focanocodigo-1.0.0/
--rw-rw-rw-   0        0        0      520 2024-04-25 23:51:35.000000 focanocodigo-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      836 2024-04-26 00:05:20.837847 focanocodigo-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-26 00:05:20.828300 focanocodigo-1.0.0/focanocodigo/
--rw-rw-rw-   0        0        0      520 2024-04-25 23:51:00.000000 focanocodigo-1.0.0/focanocodigo/__init__.py
--rw-rw-rw-   0        0        0      500 2024-04-25 23:48:44.000000 focanocodigo-1.0.0/focanocodigo/calc.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:05:20.834723 focanocodigo-1.0.0/focanocodigo.egg-info/
--rw-rw-rw-   0        0        0      836 2024-04-26 00:05:20.000000 focanocodigo-1.0.0/focanocodigo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-04-26 00:05:20.000000 focanocodigo-1.0.0/focanocodigo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 00:05:20.000000 focanocodigo-1.0.0/focanocodigo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-26 00:05:20.000000 focanocodigo-1.0.0/focanocodigo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2024-04-26 00:05:20.839854 focanocodigo-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      996 2024-04-26 00:02:53.000000 focanocodigo-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:25:57.041105 focanocodigo-1.0.1/
+-rw-rw-rw-   0        0        0      520 2024-04-25 23:51:35.000000 focanocodigo-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      876 2024-04-26 00:25:57.039801 focanocodigo-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 00:25:57.033772 focanocodigo-1.0.1/focanocodigo/
+-rw-rw-rw-   0        0        0      520 2024-04-25 23:51:00.000000 focanocodigo-1.0.1/focanocodigo/__init__.py
+-rw-rw-rw-   0        0        0      500 2024-04-25 23:48:44.000000 focanocodigo-1.0.1/focanocodigo/calc.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:25:57.038803 focanocodigo-1.0.1/focanocodigo.egg-info/
+-rw-rw-rw-   0        0        0      876 2024-04-26 00:25:56.000000 focanocodigo-1.0.1/focanocodigo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-04-26 00:25:56.000000 focanocodigo-1.0.1/focanocodigo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 00:25:56.000000 focanocodigo-1.0.1/focanocodigo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-26 00:25:56.000000 focanocodigo-1.0.1/focanocodigo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2024-04-26 00:25:57.041105 focanocodigo-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2024-04-26 00:20:36.000000 focanocodigo-1.0.1/setup.py
```

### Comparing `focanocodigo-1.0.0/LICENSE.txt` & `focanocodigo-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `focanocodigo-1.0.0/PKG-INFO` & `focanocodigo-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: focanocodigo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Calculadora simples
 Home-page: https://github.com/vagnerasilva
 Author: vagner a silva
 Author-email: vagnerasilva@email.com.br
 License: MIT
-Project-URL: Código fonte, https://github.com/vagnerasilva
-Project-URL: Download, https://github.com/vagnerasilva
+Project-URL: Código fonte, https://github.com/vagnerasilva/pacote_focanocodigo
+Project-URL: Download, https://github.com/vagnerasilva/pacote_focanocodigo
 Keywords: calculadora simples
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Internationalization
```

### Comparing `focanocodigo-1.0.0/focanocodigo/__init__.py` & `focanocodigo-1.0.1/focanocodigo/__init__.py`

 * *Files identical despite different names*

### Comparing `focanocodigo-1.0.0/focanocodigo.egg-info/PKG-INFO` & `focanocodigo-1.0.1/focanocodigo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: focanocodigo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Calculadora simples
 Home-page: https://github.com/vagnerasilva
 Author: vagner a silva
 Author-email: vagnerasilva@email.com.br
 License: MIT
-Project-URL: Código fonte, https://github.com/vagnerasilva
-Project-URL: Download, https://github.com/vagnerasilva
+Project-URL: Código fonte, https://github.com/vagnerasilva/pacote_focanocodigo
+Project-URL: Download, https://github.com/vagnerasilva/pacote_focanocodigo
 Keywords: calculadora simples
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Internationalization
```

### Comparing `focanocodigo-1.0.0/setup.py` & `focanocodigo-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name = 'focanocodigo',
-    version = '1.0.0',
+    version = '1.0.1',
     author = 'vagner a silva',
     author_email = 'vagnerasilva@email.com.br',
     packages = ['focanocodigo'],
     description = 'Calculadora simples',
     long_description = 'Calculadora simples para somar, subtrair, dividir e multiplicar.',
     url = 'https://github.com/vagnerasilva',
     project_urls = {
-        'Código fonte': 'https://github.com/vagnerasilva',
-        'Download': 'https://github.com/vagnerasilva'
+        'Código fonte': 'https://github.com/vagnerasilva/pacote_focanocodigo',
+        'Download': 'https://github.com/vagnerasilva/pacote_focanocodigo'
     },
     license = 'MIT',
     keywords = 'calculadora simples',
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

