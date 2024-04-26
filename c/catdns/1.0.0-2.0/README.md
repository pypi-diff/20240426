# Comparing `tmp/catdns-1.0.0.tar.gz` & `tmp/catdns-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catdns-1.0.0.tar", last modified: Fri Apr 26 13:17:17 2024, max compression
+gzip compressed data, was "catdns-2.0.tar", last modified: Fri Apr 26 16:03:25 2024, max compression
```

## Comparing `catdns-1.0.0.tar` & `catdns-2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 13:17:17.821146 catdns-1.0.0/
--rw-rw-rw-   0        0        0     1080 2024-04-26 11:05:33.000000 catdns-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      906 2024-04-26 13:17:17.816155 catdns-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-26 13:11:17.000000 catdns-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 13:17:17.740818 catdns-1.0.0/catdns/
--rw-rw-rw-   0        0        0      387 2024-04-26 13:04:02.000000 catdns-1.0.0/catdns/__init__.py
--rw-rw-rw-   0        0        0     1347 2024-04-26 13:01:53.000000 catdns-1.0.0/catdns/async_session.py
--rw-rw-rw-   0        0        0      386 2024-04-26 13:00:16.000000 catdns-1.0.0/catdns/asyncio.py
--rw-rw-rw-   0        0        0     1508 2024-04-26 13:02:38.000000 catdns-1.0.0/catdns/session.py
--rw-rw-rw-   0        0        0     3265 2024-04-26 12:49:43.000000 catdns-1.0.0/catdns/types.py
-drwxrwxrwx   0        0        0        0 2024-04-26 13:17:17.814174 catdns-1.0.0/catdns.egg-info/
--rw-rw-rw-   0        0        0      906 2024-04-26 13:17:17.000000 catdns-1.0.0/catdns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-04-26 13:17:17.000000 catdns-1.0.0/catdns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 13:17:17.000000 catdns-1.0.0/catdns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-26 13:17:17.000000 catdns-1.0.0/catdns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-26 13:17:17.000000 catdns-1.0.0/catdns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 13:17:17.823135 catdns-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1075 2024-04-26 13:16:51.000000 catdns-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:03:25.302048 catdns-2.0/
+-rw-rw-rw-   0        0        0     1080 2024-04-26 11:05:33.000000 catdns-2.0/LICENSE
+-rw-rw-rw-   0        0        0      850 2024-04-26 16:03:25.300053 catdns-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-26 13:11:17.000000 catdns-2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 16:03:25.244680 catdns-2.0/catdns/
+-rw-rw-rw-   0        0        0      385 2024-04-26 16:02:46.000000 catdns-2.0/catdns/__init__.py
+-rw-rw-rw-   0        0        0     1347 2024-04-26 13:01:53.000000 catdns-2.0/catdns/async_session.py
+-rw-rw-rw-   0        0        0      386 2024-04-26 13:00:16.000000 catdns-2.0/catdns/asyncio.py
+-rw-rw-rw-   0        0        0     1508 2024-04-26 13:02:38.000000 catdns-2.0/catdns/session.py
+-rw-rw-rw-   0        0        0     3398 2024-04-26 15:26:48.000000 catdns-2.0/catdns/types.py
+drwxrwxrwx   0        0        0        0 2024-04-26 16:03:25.298060 catdns-2.0/catdns.egg-info/
+-rw-rw-rw-   0        0        0      850 2024-04-26 16:03:25.000000 catdns-2.0/catdns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-26 16:03:25.000000 catdns-2.0/catdns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 16:03:25.000000 catdns-2.0/catdns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-26 16:03:25.000000 catdns-2.0/catdns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 16:03:25.000000 catdns-2.0/catdns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      554 2024-04-26 16:02:39.000000 catdns-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 16:03:25.303046 catdns-2.0/setup.cfg
```

### Comparing `catdns-1.0.0/LICENSE` & `catdns-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `catdns-1.0.0/catdns/async_session.py` & `catdns-2.0/catdns/async_session.py`

 * *Files identical despite different names*

### Comparing `catdns-1.0.0/catdns/session.py` & `catdns-2.0/catdns/session.py`

 * *Files identical despite different names*

### Comparing `catdns-1.0.0/catdns/types.py` & `catdns-2.0/catdns/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,24 +54,27 @@
 
         return state
 
 class MailData(Parser):
     def __init__(
             self,
             content: str = None,
-            type: str = None
+            type: str = None,
+            html: str = None
         ):
             self.content = content
             self.type = type
+            self.html = html
 
     @staticmethod
     def from_json(_d: Dict) -> "MailData":
         return MailData(
             content=_d.get("content"),
-            type=_d.get("type")
+            type=_d.get("type"),
+            html=_d.get("textAsHtml")
         )
 
 class Mail(Parser):
     def __init__(
         self,
         data: "MailData" = None,
         date: str = None,
@@ -116,10 +119,10 @@
         ):
             self.mail_data = mail_data
             self.message = message
 
     @staticmethod
     def from_json(_d: Dict) -> "FullMail":
         return FullMail(
-            mail_data=[Mail.from_json(i) for i in _d.get("mailData")],
+            mail_data=[Mail.from_json(i) for i in _d.get("mailData")] if _d.get("mailData") else None,
             message=_d.get("message")
         )
```

