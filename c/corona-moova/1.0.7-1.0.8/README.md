# Comparing `tmp/corona-moova-1.0.7.tar.gz` & `tmp/corona-moova-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corona-moova-1.0.7.tar", last modified: Tue Jan 16 03:30:56 2024, max compression
+gzip compressed data, was "corona-moova-1.0.8.tar", last modified: Fri Apr 26 18:12:17 2024, max compression
```

## Comparing `corona-moova-1.0.7.tar` & `corona-moova-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 anderssonvelasquezalvites   (501) staff       (20)        0 2024-01-16 03:30:56.267886 corona-moova-1.0.7/
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)        0 2023-08-05 04:18:54.000000 corona-moova-1.0.7/LICENSE
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     2162 2024-01-16 03:30:56.267745 corona-moova-1.0.7/PKG-INFO
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     1812 2024-01-16 00:32:22.000000 corona-moova-1.0.7/README.rst
-drwxr-xr-x   0 anderssonvelasquezalvites   (501) staff       (20)        0 2024-01-16 03:30:56.266480 corona-moova-1.0.7/corona_moova.egg-info/
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     2162 2024-01-16 03:30:56.000000 corona-moova-1.0.7/corona_moova.egg-info/PKG-INFO
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)      260 2024-01-16 03:30:56.000000 corona-moova-1.0.7/corona_moova.egg-info/SOURCES.txt
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)        1 2024-01-16 03:30:56.000000 corona-moova-1.0.7/corona_moova.egg-info/dependency_links.txt
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)       27 2024-01-16 03:30:56.000000 corona-moova-1.0.7/corona_moova.egg-info/requires.txt
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)        6 2024-01-16 03:30:56.000000 corona-moova-1.0.7/corona_moova.egg-info/top_level.txt
-drwxr-xr-x   0 anderssonvelasquezalvites   (501) staff       (20)        0 2024-01-16 03:30:56.267361 corona-moova-1.0.7/moova/
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     3036 2024-01-12 02:39:49.000000 corona-moova-1.0.7/moova/connector.py
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     6959 2024-01-16 03:18:39.000000 corona-moova-1.0.7/moova/handler.py
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     4639 2024-01-16 00:32:11.000000 corona-moova-1.0.7/moova/settings.py
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)       38 2024-01-16 03:30:56.267946 corona-moova-1.0.7/setup.cfg
--rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)      627 2024-01-16 03:29:11.000000 corona-moova-1.0.7/setup.py
+drwxr-xr-x   0 anderssonvelasquezalvites   (501) staff       (20)        0 2024-04-26 18:12:17.839536 corona-moova-1.0.8/
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)        0 2023-08-05 04:18:54.000000 corona-moova-1.0.8/LICENSE
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     2162 2024-04-26 18:12:17.839316 corona-moova-1.0.8/PKG-INFO
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     1812 2024-01-16 00:32:22.000000 corona-moova-1.0.8/README.rst
+drwxr-xr-x   0 anderssonvelasquezalvites   (501) staff       (20)        0 2024-04-26 18:12:17.837817 corona-moova-1.0.8/corona_moova.egg-info/
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     2162 2024-04-26 18:12:17.000000 corona-moova-1.0.8/corona_moova.egg-info/PKG-INFO
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)      260 2024-04-26 18:12:17.000000 corona-moova-1.0.8/corona_moova.egg-info/SOURCES.txt
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)        1 2024-04-26 18:12:17.000000 corona-moova-1.0.8/corona_moova.egg-info/dependency_links.txt
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)       27 2024-04-26 18:12:17.000000 corona-moova-1.0.8/corona_moova.egg-info/requires.txt
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)        6 2024-04-26 18:12:17.000000 corona-moova-1.0.8/corona_moova.egg-info/top_level.txt
+drwxr-xr-x   0 anderssonvelasquezalvites   (501) staff       (20)        0 2024-04-26 18:12:17.838737 corona-moova-1.0.8/moova/
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     3036 2024-01-12 02:39:49.000000 corona-moova-1.0.8/moova/connector.py
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     6997 2024-04-26 17:54:28.000000 corona-moova-1.0.8/moova/handler.py
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)     4639 2024-01-16 00:32:11.000000 corona-moova-1.0.8/moova/settings.py
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)       38 2024-04-26 18:12:17.839605 corona-moova-1.0.8/setup.cfg
+-rw-r--r--   0 anderssonvelasquezalvites   (501) staff       (20)      627 2024-04-26 17:58:24.000000 corona-moova-1.0.8/setup.py
```

### Comparing `corona-moova-1.0.7/PKG-INFO` & `corona-moova-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corona-moova
-Version: 1.0.7
+Version: 1.0.8
 Summary: Django Moova Integration
 Home-page: https://gitlab.com/linets-projects/python-libraries/django-moova/
 Author: Corona Development Team
 Author-email: rolguin@corona.cl
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `corona-moova-1.0.7/README.rst` & `corona-moova-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `corona-moova-1.0.7/corona_moova.egg-info/PKG-INFO` & `corona-moova-1.0.8/corona_moova.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corona-moova
-Version: 1.0.7
+Version: 1.0.8
 Summary: Django Moova Integration
 Home-page: https://gitlab.com/linets-projects/python-libraries/django-moova/
 Author: Corona Development Team
 Author-email: rolguin@corona.cl
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `corona-moova-1.0.7/moova/connector.py` & `corona-moova-1.0.8/moova/connector.py`

 * *Files identical despite different names*

### Comparing `corona-moova-1.0.7/moova/handler.py` & `corona-moova-1.0.8/moova/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 'email': api_settings.SENDER['EMAIL'],
                 'phone': api_settings.SENDER['PHONE']
             }
         }
 
         payload = {
             'currency': api_settings.MOOVA['CURRENCY'],
-            'type': self.type,
+            'type': getattr(instance.extra_args, 'type', self.type),
             'flow': self.flow,
             'from': from_data,
             'to': {
                 'address': f'{instance.address.street} {instance.address.number}, {instance.commune.name}, {instance.region.name}, Chile',
                 'country': api_settings.SENDER['COUNTRY'],
                 'instructions': instance.address.full_address,
                 'contact': {
```

### Comparing `corona-moova-1.0.7/moova/settings.py` & `corona-moova-1.0.8/moova/settings.py`

 * *Files identical despite different names*

### Comparing `corona-moova-1.0.7/setup.py` & `corona-moova-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, 'README.rst')).read()
 
 setup(
     name='corona-moova',
-    version='1.0.7',
+    version='1.0.8',
     packages=['moova'],
     description='Django Moova Integration',
     long_description=README,
     long_description_content_type="text/markdown",
     author='Corona Development Team',
     author_email='rolguin@corona.cl',
     url='https://gitlab.com/linets-projects/python-libraries/django-moova/',
```

