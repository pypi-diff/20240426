# Comparing `tmp/sanctify-1.4.0.tar.gz` & `tmp/sanctify-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctify-1.4.0.tar", last modified: Tue Apr  2 09:27:27 2024, max compression
+gzip compressed data, was "sanctify-1.4.1.tar", last modified: Fri Apr 26 08:58:00 2024, max compression
```

## Comparing `sanctify-1.4.0.tar` & `sanctify-1.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-02 09:27:27.301941 sanctify-1.4.0/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11349 2023-07-24 05:34:49.000000 sanctify-1.4.0/LICENSE
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-04-02 09:27:27.301638 sanctify-1.4.0/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18062 2023-09-20 08:58:16.000000 sanctify-1.4.0/README.md
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1814 2024-04-02 09:27:08.000000 sanctify-1.4.0/pyproject.toml
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-02 09:27:27.299127 sanctify-1.4.0/sanctify/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1286 2024-04-02 09:24:44.000000 sanctify-1.4.0/sanctify/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18219 2024-04-02 09:27:08.000000 sanctify-1.4.0/sanctify/cleanser.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2805 2024-03-08 13:21:10.000000 sanctify-1.4.0/sanctify/constants.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-02 09:27:27.300948 sanctify-1.4.0/sanctify/examples/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      329 2024-04-02 09:24:44.000000 sanctify-1.4.0/sanctify/examples/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2155 2024-03-09 16:56:05.000000 sanctify-1.4.0/sanctify/examples/column_mapping_schema.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3238 2023-10-16 06:12:09.000000 sanctify-1.4.0/sanctify/examples/data_type_schema.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      332 2023-08-07 05:30:23.000000 sanctify-1.4.0/sanctify/exception.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    14964 2024-04-02 09:24:45.000000 sanctify-1.4.0/sanctify/processor.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4145 2023-08-07 05:30:23.000000 sanctify-1.4.0/sanctify/serializer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13067 2024-04-02 09:24:45.000000 sanctify-1.4.0/sanctify/transformer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4922 2024-03-12 11:16:48.000000 sanctify-1.4.0/sanctify/utils.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13172 2024-04-02 09:24:45.000000 sanctify-1.4.0/sanctify/validator.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-02 09:27:27.301270 sanctify-1.4.0/sanctify.egg-info/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-04-02 09:27:27.000000 sanctify-1.4.0/sanctify.egg-info/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      497 2024-04-02 09:27:27.000000 sanctify-1.4.0/sanctify.egg-info/SOURCES.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2024-04-02 09:27:27.000000 sanctify-1.4.0/sanctify.egg-info/dependency_links.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      256 2024-04-02 09:27:27.000000 sanctify-1.4.0/sanctify.egg-info/requires.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2024-04-02 09:27:27.000000 sanctify-1.4.0/sanctify.egg-info/top_level.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2024-04-02 09:27:27.301980 sanctify-1.4.0/setup.cfg
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-26 08:58:00.953573 sanctify-1.4.1/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11349 2023-07-24 05:34:49.000000 sanctify-1.4.1/LICENSE
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-04-26 08:58:00.953195 sanctify-1.4.1/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18062 2023-09-20 08:58:16.000000 sanctify-1.4.1/README.md
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1814 2024-04-26 08:56:53.000000 sanctify-1.4.1/pyproject.toml
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-26 08:58:00.940561 sanctify-1.4.1/sanctify/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1286 2024-04-26 08:57:18.000000 sanctify-1.4.1/sanctify/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18219 2024-04-26 08:49:28.000000 sanctify-1.4.1/sanctify/cleanser.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2805 2024-03-08 13:21:10.000000 sanctify-1.4.1/sanctify/constants.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-26 08:58:00.950364 sanctify-1.4.1/sanctify/examples/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      329 2024-04-26 08:57:18.000000 sanctify-1.4.1/sanctify/examples/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2155 2024-03-09 16:56:05.000000 sanctify-1.4.1/sanctify/examples/column_mapping_schema.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3238 2023-10-16 06:12:09.000000 sanctify-1.4.1/sanctify/examples/data_type_schema.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      332 2023-08-07 05:30:23.000000 sanctify-1.4.1/sanctify/exception.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    14964 2024-04-26 08:57:18.000000 sanctify-1.4.1/sanctify/processor.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4145 2023-08-07 05:30:23.000000 sanctify-1.4.1/sanctify/serializer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12902 2024-04-26 08:57:18.000000 sanctify-1.4.1/sanctify/transformer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4922 2024-03-12 11:16:48.000000 sanctify-1.4.1/sanctify/utils.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13172 2024-04-26 08:57:18.000000 sanctify-1.4.1/sanctify/validator.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-26 08:58:00.952337 sanctify-1.4.1/sanctify.egg-info/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-04-26 08:58:00.000000 sanctify-1.4.1/sanctify.egg-info/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      497 2024-04-26 08:58:00.000000 sanctify-1.4.1/sanctify.egg-info/SOURCES.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2024-04-26 08:58:00.000000 sanctify-1.4.1/sanctify.egg-info/dependency_links.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      256 2024-04-26 08:58:00.000000 sanctify-1.4.1/sanctify.egg-info/requires.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2024-04-26 08:58:00.000000 sanctify-1.4.1/sanctify.egg-info/top_level.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2024-04-26 08:58:00.953740 sanctify-1.4.1/setup.cfg
```

### Comparing `sanctify-1.4.0/LICENSE` & `sanctify-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/PKG-INFO` & `sanctify-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.4.0
+Version: 1.4.1
 Summary: Column Mapping based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sanctify-1.4.0/README.md` & `sanctify-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/pyproject.toml` & `sanctify-1.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 [tool.pytest.ini_options]
 log_cli=true
 log_cli_level='DEBUG'
 
 [project]
 name = "sanctify"
-version = "1.4.0"
+version = "1.4.1"
 authors = [{name = "Avijeet Diwaker", email = "avijeetdiwaker@gmail.com"}]
 description = "Column Mapping based cleansing and validations for a given pandas dataframe"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `sanctify-1.4.0/sanctify/__init__.py` & `sanctify-1.4.1/sanctify/__init__.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/sanctify/cleanser.py` & `sanctify-1.4.1/sanctify/cleanser.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/sanctify/constants.py` & `sanctify-1.4.1/sanctify/constants.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/sanctify/examples/column_mapping_schema.py` & `sanctify-1.4.1/sanctify/examples/column_mapping_schema.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/sanctify/examples/data_type_schema.py` & `sanctify-1.4.1/sanctify/examples/data_type_schema.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/sanctify/processor.py` & `sanctify-1.4.1/sanctify/processor.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/sanctify/serializer.py` & `sanctify-1.4.1/sanctify/serializer.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/sanctify/transformer.py` & `sanctify-1.4.1/sanctify/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,21 +272,16 @@
         Args:
             value (str): The input amount string.
 
         Returns:
             str: The amount string with currency symbols and separators removed.
             ValidationError: if amount is invalid or negative
         """
+        # Use regex to remove everything except digits, decimal point, and minus sign
         _amount = re.sub(r"[^\d.-]", "", str(value))
-        match = re.search(r"(-)?0*([1-9])", _amount)
-
-        if match:
-            hyphen = match.group(1) if match.group(1) else ""
-            non_zero_digit = match.group(2)
-            _amount = f"{hyphen}{non_zero_digit}{_amount[match.end():]}"
 
         try:
             amount = float(_amount)
             if amount > 0:
                 return str(amount)
             else:
                 raise ValidationError(f"Amount {str(amount)} should not be negative")
```

### Comparing `sanctify-1.4.0/sanctify/utils.py` & `sanctify-1.4.1/sanctify/utils.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/sanctify/validator.py` & `sanctify-1.4.1/sanctify/validator.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.0/sanctify.egg-info/PKG-INFO` & `sanctify-1.4.1/sanctify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.4.0
+Version: 1.4.1
 Summary: Column Mapping based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

