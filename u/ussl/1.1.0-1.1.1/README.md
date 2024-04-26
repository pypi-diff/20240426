# Comparing `tmp/ussl-1.1.0.tar.gz` & `tmp/ussl-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ussl-1.1.0.tar", last modified: Wed Apr 24 13:51:11 2024, max compression
+gzip compressed data, was "dist\ussl-1.1.1.tar", last modified: Fri Apr 26 10:24:44 2024, max compression
```

## Comparing `ussl-1.1.0.tar` & `ussl-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:11.193489 ussl-1.1.0/
--rw-rw-rw-   0        0        0    15143 2024-04-24 13:51:11.189491 ussl-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    14493 2024-03-01 08:27:08.000000 ussl-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 13:51:11.193489 ussl-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1679 2024-04-24 13:51:08.000000 ussl-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:11.146272 ussl-1.1.0/ussl/
--rw-rw-rw-   0        0        0       49 2024-03-01 08:27:08.000000 ussl-1.1.0/ussl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:11.164589 ussl-1.1.0/ussl/exceptions/
--rw-rw-rw-   0        0        0      305 2024-03-01 08:27:08.000000 ussl-1.1.0/ussl/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1369 2024-04-24 10:36:55.000000 ussl-1.1.0/ussl/exceptions/main.py
--rw-rw-rw-   0        0        0     1126 2024-03-01 08:27:08.000000 ussl-1.1.0/ussl/exceptions/protocol_exc.py
--rw-rw-rw-   0        0        0     1084 2024-03-01 08:27:08.000000 ussl-1.1.0/ussl/exceptions/validation_exc.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:11.166596 ussl-1.1.0/ussl/model/
--rw-rw-rw-   0        0        0     4312 2024-04-24 12:40:12.000000 ussl-1.1.0/ussl/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:11.169618 ussl-1.1.0/ussl/postprocessing/
--rw-rw-rw-   0        0        0        0 2024-03-01 08:27:08.000000 ussl-1.1.0/ussl/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     6999 2024-04-24 13:51:08.000000 ussl-1.1.0/ussl/postprocessing/base.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:11.183490 ussl-1.1.0/ussl/protocol/
--rw-rw-rw-   0        0        0      673 2024-04-24 10:42:12.000000 ussl-1.1.0/ussl/protocol/__init__.py
--rw-rw-rw-   0        0        0      562 2024-04-24 12:40:12.000000 ussl-1.1.0/ussl/protocol/base.py
--rw-rw-rw-   0        0        0     1480 2024-04-24 12:40:12.000000 ussl-1.1.0/ussl/protocol/ldap.py
--rw-rw-rw-   0        0        0     3999 2024-04-24 12:46:57.000000 ussl-1.1.0/ussl/protocol/ssh.py
--rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.1.0/ussl/protocol/winexe.py
--rw-rw-rw-   0        0        0     6120 2024-04-24 12:40:12.000000 ussl-1.1.0/ussl/protocol/winrm.py
--rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.1.0/ussl/protocol/wmi.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:11.185486 ussl-1.1.0/ussl/transport/
--rw-rw-rw-   0        0        0     1508 2024-03-01 08:27:08.000000 ussl-1.1.0/ussl/transport/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:11.186486 ussl-1.1.0/ussl/utils/
--rw-rw-rw-   0        0        0     6424 2024-03-01 08:27:08.000000 ussl-1.1.0/ussl/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:11.155589 ussl-1.1.0/ussl.egg-info/
--rw-rw-rw-   0        0        0    15143 2024-04-24 13:51:11.000000 ussl-1.1.0/ussl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2024-04-24 13:51:11.000000 ussl-1.1.0/ussl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 13:51:11.000000 ussl-1.1.0/ussl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-04-24 13:51:11.000000 ussl-1.1.0/ussl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-24 13:51:11.000000 ussl-1.1.0/ussl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.211096 ussl-1.1.1/
+-rw-rw-rw-   0        0        0    15145 2024-04-26 10:24:44.205865 ussl-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14493 2024-03-01 08:27:08.000000 ussl-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 10:24:44.211096 ussl-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1681 2024-04-26 10:24:31.000000 ussl-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.157381 ussl-1.1.1/ussl/
+-rw-rw-rw-   0        0        0       49 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.177040 ussl-1.1.1/ussl/exceptions/
+-rw-rw-rw-   0        0        0      305 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1369 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/exceptions/main.py
+-rw-rw-rw-   0        0        0     1126 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/exceptions/protocol_exc.py
+-rw-rw-rw-   0        0        0     1084 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/exceptions/validation_exc.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.179042 ussl-1.1.1/ussl/model/
+-rw-rw-rw-   0        0        0     4312 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.182945 ussl-1.1.1/ussl/postprocessing/
+-rw-rw-rw-   0        0        0        0 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     6999 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/postprocessing/base.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.198877 ussl-1.1.1/ussl/protocol/
+-rw-rw-rw-   0        0        0      673 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/protocol/__init__.py
+-rw-rw-rw-   0        0        0      562 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/protocol/base.py
+-rw-rw-rw-   0        0        0     1480 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/protocol/ldap.py
+-rw-rw-rw-   0        0        0     3999 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/protocol/ssh.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.1.1/ussl/protocol/winexe.py
+-rw-rw-rw-   0        0        0     6120 2024-04-26 07:05:38.000000 ussl-1.1.1/ussl/protocol/winrm.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.1.1/ussl/protocol/wmi.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.199876 ussl-1.1.1/ussl/transport/
+-rw-rw-rw-   0        0        0     1508 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/transport/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.202448 ussl-1.1.1/ussl/utils/
+-rw-rw-rw-   0        0        0     6424 2024-03-01 08:27:08.000000 ussl-1.1.1/ussl/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:24:44.167336 ussl-1.1.1/ussl.egg-info/
+-rw-rw-rw-   0        0        0    15145 2024-04-26 10:24:44.000000 ussl-1.1.1/ussl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2024-04-26 10:24:44.000000 ussl-1.1.1/ussl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 10:24:44.000000 ussl-1.1.1/ussl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-04-26 10:24:44.000000 ussl-1.1.1/ussl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 10:24:44.000000 ussl-1.1.1/ussl.egg-info/top_level.txt
```

### Comparing `ussl-1.1.0/PKG-INFO` & `ussl-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.1.0
+Version: 1.1.1
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: ==3.8
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: pywinrm==0.4.1
 Requires-Dist: paramiko==2.7.2
 Requires-Dist: marshmallow==3.20.2
 Requires-Dist: python-ldap==3.4.4; platform_system != "Windows"
 
 # USSL - USSC SOAR SCRIPT LIB
```

### Comparing `ussl-1.1.0/README.md` & `ussl-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/setup.py` & `ussl-1.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 setup(
     name='ussl',
     author='ussc soc dev team',
     author_email='iushangaraev@ussc.ru, pbikkuzhina@ussc.ru',
     description='Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.0',
-    python_requires='==3.8',
+    version='1.1.1',
+    python_requires='>=3.8.0',
     packages=[
         'ussl',
         'ussl.model',
         'ussl.postprocessing',
         'ussl.protocol',
         'ussl.transport',
         'ussl.exceptions',
```

### Comparing `ussl-1.1.0/ussl/exceptions/main.py` & `ussl-1.1.1/ussl/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/exceptions/protocol_exc.py` & `ussl-1.1.1/ussl/exceptions/protocol_exc.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/exceptions/validation_exc.py` & `ussl-1.1.1/ussl/exceptions/validation_exc.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/model/__init__.py` & `ussl-1.1.1/ussl/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/postprocessing/base.py` & `ussl-1.1.1/ussl/postprocessing/base.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/protocol/__init__.py` & `ussl-1.1.1/ussl/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/protocol/base.py` & `ussl-1.1.1/ussl/protocol/base.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/protocol/ldap.py` & `ussl-1.1.1/ussl/protocol/ldap.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/protocol/ssh.py` & `ussl-1.1.1/ussl/protocol/ssh.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/protocol/winrm.py` & `ussl-1.1.1/ussl/protocol/winrm.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/transport/__init__.py` & `ussl-1.1.1/ussl/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl/utils/__init__.py` & `ussl-1.1.1/ussl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.1.0/ussl.egg-info/PKG-INFO` & `ussl-1.1.1/ussl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.1.0
+Version: 1.1.1
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: ==3.8
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: pywinrm==0.4.1
 Requires-Dist: paramiko==2.7.2
 Requires-Dist: marshmallow==3.20.2
 Requires-Dist: python-ldap==3.4.4; platform_system != "Windows"
 
 # USSL - USSC SOAR SCRIPT LIB
```

### Comparing `ussl-1.1.0/ussl.egg-info/SOURCES.txt` & `ussl-1.1.1/ussl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

