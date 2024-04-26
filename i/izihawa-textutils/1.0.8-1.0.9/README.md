# Comparing `tmp/izihawa_textutils-1.0.8.tar.gz` & `tmp/izihawa_textutils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_textutils-1.0.8.tar", max compression
+gzip compressed data, was "izihawa_textutils-1.0.9.tar", max compression
```

## Comparing `izihawa_textutils-1.0.8.tar` & `izihawa_textutils-1.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       54 2023-11-27 07:20:26.275666 izihawa_textutils-1.0.8/README.md
--rw-r--r--   0        0        0        0 2023-11-27 07:15:02.405382 izihawa_textutils-1.0.8/izihawa_textutils/__init__.py
--rw-r--r--   0        0        0     1152 2023-11-27 07:20:26.278155 izihawa_textutils-1.0.8/izihawa_textutils/html_processing.py
--rw-r--r--   0        0        0     1458 2023-11-27 07:17:37.826198 izihawa_textutils-1.0.8/izihawa_textutils/regex.py
--rw-r--r--   0        0        0     4576 2023-11-27 09:45:43.053713 izihawa_textutils-1.0.8/izihawa_textutils/utils.py
--rw-r--r--   0        0        0      276 2023-11-27 09:45:50.523985 izihawa_textutils-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 izihawa_textutils-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-11-27 07:20:26.275666 izihawa_textutils-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-11-27 07:15:02.405382 izihawa_textutils-1.0.9/izihawa_textutils/__init__.py
+-rw-r--r--   0        0        0     1152 2023-11-27 07:20:26.278155 izihawa_textutils-1.0.9/izihawa_textutils/html_processing.py
+-rw-r--r--   0        0        0     1458 2023-11-27 07:17:37.826198 izihawa_textutils-1.0.9/izihawa_textutils/regex.py
+-rw-r--r--   0        0        0     4569 2023-11-27 09:47:19.851061 izihawa_textutils-1.0.9/izihawa_textutils/utils.py
+-rw-r--r--   0        0        0      276 2023-11-27 09:47:23.609880 izihawa_textutils-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 izihawa_textutils-1.0.9/PKG-INFO
```

### Comparing `izihawa_textutils-1.0.8/izihawa_textutils/html_processing.py` & `izihawa_textutils-1.0.9/izihawa_textutils/html_processing.py`

 * *Files identical despite different names*

### Comparing `izihawa_textutils-1.0.8/izihawa_textutils/regex.py` & `izihawa_textutils-1.0.9/izihawa_textutils/regex.py`

 * *Files identical despite different names*

### Comparing `izihawa_textutils-1.0.8/izihawa_textutils/utils.py` & `izihawa_textutils-1.0.9/izihawa_textutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     text = re.sub(r"\[\s*(.*?)(\s*)]\([^)]+", r"\g<1>\g<2>", text, flags=re.MULTILINE)
     return text
 
 
 def convert_markdown_to_telegram_markdown(text: str):
     text = re.sub(r"^#{1,6}\s*([^\n$]*)", r"**\g<1>**", text, flags=re.MULTILINE)
     text = re.sub(r"~([^~\n]+)~", r"\g<1>", text)
-    text = re.sub(r"!\[(.*)]\([^)]+\)", r"🖼️[\g<1>]", text)
+    text = re.sub(r"!\[(.*)]\([^)]+\)", r"🖼️", text)
     text = re.sub(r"\[(.*)]\([^)]+\)", r"\g<1>", text)
     text = re.sub(r'^(\|.*\|)+$', '🔢', text, flags=re.MULTILINE | re.DOTALL)
     text = re.sub(r"\^([^\^\n]+)\^", r"\g<1>", text)
     return text
 
 
 def remove_emails(text: str):
```

### Comparing `izihawa_textutils-1.0.8/PKG-INFO` & `izihawa_textutils-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa-textutils
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

