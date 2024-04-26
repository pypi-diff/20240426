# Comparing `tmp/django-darthmail-0.3.0.tar.gz` & `tmp/django_darthmail-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-darthmail-0.3.0.tar", last modified: Thu Sep 14 09:50:18 2023, max compression
+gzip compressed data, was "django_darthmail-0.4.0.tar", last modified: Fri Apr 26 13:41:02 2024, max compression
```

## Comparing `django-darthmail-0.3.0.tar` & `django_darthmail-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-14 09:50:18.128550 django-darthmail-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1465 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       64 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1456 2023-09-14 09:50:18.128550 django-darthmail-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      593 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-14 09:50:18.128550 django-darthmail-0.3.0/django_darthmail/
--rw-r--r--   0 root         (0) root         (0)      463 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/django_darthmail/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/django_darthmail/apps.py
--rw-r--r--   0 root         (0) root         (0)     2200 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/django_darthmail/backends.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/django_darthmail/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-14 09:50:18.128550 django-darthmail-0.3.0/django_darthmail/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/django_darthmail/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-14 09:50:18.128550 django-darthmail-0.3.0/django_darthmail/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/django_darthmail/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/django_darthmail/management/commands/sendtestdarthmail.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/django_darthmail/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-14 09:50:18.128550 django-darthmail-0.3.0/django_darthmail/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/django_darthmail/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3747 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/django_darthmail/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-14 09:50:18.128550 django-darthmail-0.3.0/django_darthmail.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1456 2023-09-14 09:50:18.000000 django-darthmail-0.3.0/django_darthmail.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      604 2023-09-14 09:50:18.000000 django-darthmail-0.3.0/django_darthmail.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-14 09:50:18.000000 django-darthmail-0.3.0/django_darthmail.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-09-14 09:50:18.000000 django-darthmail-0.3.0/django_darthmail.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-09-14 09:50:18.000000 django-darthmail-0.3.0/django_darthmail.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      406 2023-09-14 09:50:18.128550 django-darthmail-0.3.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1876 2023-09-14 09:50:07.000000 django-darthmail-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1456 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/django_darthmail/
+-rw-r--r--   0 root         (0) root         (0)      463 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/backends.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/django_darthmail/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/django_darthmail/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      823 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/management/commands/sendtestdarthmail.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/django_darthmail/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3747 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/django_darthmail.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1456 2024-04-26 13:41:02.000000 django_darthmail-0.4.0/django_darthmail.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-26 13:41:02.000000 django_darthmail-0.4.0/django_darthmail.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 13:41:02.000000 django_darthmail-0.4.0/django_darthmail.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-26 13:41:02.000000 django_darthmail-0.4.0/django_darthmail.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-26 13:41:02.000000 django_darthmail-0.4.0/django_darthmail.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1876 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/setup.py
```

### Comparing `django-darthmail-0.3.0/LICENSE` & `django_darthmail-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-darthmail-0.3.0/PKG-INFO` & `django_darthmail-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-darthmail
-Version: 0.3.0
+Version: 0.4.0
 Summary: Client for the DarthMail project
 Home-page: https://github.com/regiohelden/django-darthmail
 Author: RegioHelden GmbH
 Author-email: entwicklung@regiohelden.de
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
```

### Comparing `django-darthmail-0.3.0/README.md` & `django_darthmail-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django-darthmail-0.3.0/django_darthmail/backends.py` & `django_darthmail-0.4.0/django_darthmail/backends.py`

 * *Files identical despite different names*

### Comparing `django-darthmail-0.3.0/django_darthmail/client.py` & `django_darthmail-0.4.0/django_darthmail/client.py`

 * *Files identical despite different names*

### Comparing `django-darthmail-0.3.0/django_darthmail/management/commands/sendtestdarthmail.py` & `django_darthmail-0.4.0/django_darthmail/management/commands/sendtestdarthmail.py`

 * *Files identical despite different names*

### Comparing `django-darthmail-0.3.0/django_darthmail/message.py` & `django_darthmail-0.4.0/django_darthmail/message.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import os
 import mimetypes
 from email.mime.image import MIMEImage
+from pathlib import Path
+from typing import IO
 
 from django.core.mail import EmailMultiAlternatives as DjangoEmailMultiAlternatives
+from PIL import Image
 
 
 class EmailMultiAlternatives(DjangoEmailMultiAlternatives):
     def __init__(self, *args, **kwargs):
         """
         Extension of django's EmailMultiAlternatives supporting the following extra parameters: metadata, send_at,
         unique_hash and force_send
@@ -19,25 +21,29 @@
         self.metadata = kwargs.pop('metadata', dict())
         self.send_at = kwargs.pop('send_at', None)
         self.force_send = kwargs.pop('force_send', False)
         self.unique_hash = kwargs.pop('unique_hash', None)
 
         super(EmailMultiAlternatives, self).__init__(*args, **kwargs)
 
-    def attach_inline_image(self, filepath, cid):
-        if not os.path.exists(filepath):
+    def attach_inline_image(self, filepath: str, cid: str) -> None:
+        if not Path(filepath).exists():
             # TODO: shouldn't we raise something?
             return
-        with open(filepath, 'rb') as fp:
-            msg_img = MIMEImage(fp.read())
+        with Path(filepath).open(mode='rb') as fp:
+            image_data = fp.read()
+            image = Image.open(fp)
+            _, mime_format = image.get_format_mimetype().split('/')
+            msg_img = MIMEImage(image_data, _subtype=mime_format)
             msg_img.add_header('Content-ID', '<{}>'.format(cid))
             self.attach(msg_img)
 
-    def add_image(self, directory, filename, alias):
+    def add_image(self, directory: str, filename: str, alias: str) -> None:
         '''
         Wrapper for backward-compat with notification.models.EmailMultiAlternativesWithImages
         '''
-        self.attach_inline_image(os.path.join(directory, filename), alias)
+        filepath = Path(directory, filename)
+        self.attach_inline_image(filepath.as_posix(), alias)
 
-    def add_attachment(self, _file):
+    def add_attachment(self, _file: IO) -> None:
         content_type, encoding = mimetypes.guess_type(_file.name)
-        self.attach(os.path.basename(_file.name), _file.read(), content_type)
+        self.attach(Path(_file.name).name, _file.read(), content_type)
```

### Comparing `django-darthmail-0.3.0/django_darthmail/serializers.py` & `django_darthmail-0.4.0/django_darthmail/serializers.py`

 * *Files identical despite different names*

### Comparing `django-darthmail-0.3.0/django_darthmail.egg-info/PKG-INFO` & `django_darthmail-0.4.0/django_darthmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-darthmail
-Version: 0.3.0
+Version: 0.4.0
 Summary: Client for the DarthMail project
 Home-page: https://github.com/regiohelden/django-darthmail
 Author: RegioHelden GmbH
 Author-email: entwicklung@regiohelden.de
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
```

### Comparing `django-darthmail-0.3.0/django_darthmail.egg-info/SOURCES.txt` & `django_darthmail-0.4.0/django_darthmail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-darthmail-0.3.0/setup.py` & `django_darthmail-0.4.0/setup.py`

 * *Files identical despite different names*

