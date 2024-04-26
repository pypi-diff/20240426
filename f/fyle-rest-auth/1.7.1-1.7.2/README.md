# Comparing `tmp/fyle-rest-auth-1.7.1.tar.gz` & `tmp/fyle_rest_auth-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyle-rest-auth-1.7.1.tar", last modified: Fri Feb 23 08:00:18 2024, max compression
+gzip compressed data, was "fyle_rest_auth-1.7.2.tar", last modified: Fri Apr 26 15:27:20 2024, max compression
```

## Comparing `fyle-rest-auth-1.7.1.tar` & `fyle_rest_auth-1.7.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:00:18.574890 fyle-rest-auth-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-02-23 08:00:18.574890 fyle-rest-auth-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:00:18.570891 fyle-rest-auth-1.7.1/fyle_rest_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:00:18.574890 fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/0002_auto_20200101_1205.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/0003_auto_20200107_0921.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/0004_auto_20200107_1345.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/0005_remove_authtoken_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/0006_auto_20201221_0849.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/fyle_rest_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:00:18.574890 fyle-rest-auth-1.7.1/fyle_rest_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-02-23 08:00:18.000000 fyle-rest-auth-1.7.1/fyle_rest_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-23 08:00:18.000000 fyle-rest-auth-1.7.1/fyle_rest_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 08:00:18.000000 fyle-rest-auth-1.7.1/fyle_rest_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-23 08:00:18.000000 fyle-rest-auth-1.7.1/fyle_rest_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-23 08:00:18.000000 fyle-rest-auth-1.7.1/fyle_rest_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 08:00:18.574890 fyle-rest-auth-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-23 08:00:08.000000 fyle-rest-auth-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:27:20.227999 fyle_rest_auth-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-26 15:27:20.227999 fyle_rest_auth-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:27:20.223999 fyle_rest_auth-1.7.2/fyle_rest_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:27:20.227999 fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/0002_auto_20200101_1205.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/0003_auto_20200107_0921.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/0004_auto_20200107_1345.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/0005_remove_authtoken_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/0006_auto_20201221_0849.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/fyle_rest_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:27:20.227999 fyle_rest_auth-1.7.2/fyle_rest_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-26 15:27:20.000000 fyle_rest_auth-1.7.2/fyle_rest_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-26 15:27:20.000000 fyle_rest_auth-1.7.2/fyle_rest_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:27:20.000000 fyle_rest_auth-1.7.2/fyle_rest_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-26 15:27:20.000000 fyle_rest_auth-1.7.2/fyle_rest_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 15:27:20.000000 fyle_rest_auth-1.7.2/fyle_rest_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:27:20.227999 fyle_rest_auth-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-26 15:27:12.000000 fyle_rest_auth-1.7.2/setup.py
```

### Comparing `fyle-rest-auth-1.7.1/LICENSE` & `fyle_rest_auth-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fyle-rest-auth-1.7.1/PKG-INFO` & `fyle_rest_auth-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyle-rest-auth
-Version: 1.7.1
+Version: 1.7.2
 Summary: Django application to implement OAuth 2.0 using Fyle in Django rest framework
 Home-page: https://github.com/fylein/fyle-rest-auth
 Author: Shwetabh Kumar
 Author-email: shwetabh.kumar@fyle.in
 License: MIT
 Keywords: fyle,rest,django-rest-framework,api,python,oauth 2
 Classifier: Framework :: Django
```

### Comparing `fyle-rest-auth-1.7.1/README.md` & `fyle_rest_auth-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `fyle-rest-auth-1.7.1/fyle_rest_auth/authentication.py` & `fyle_rest_auth-1.7.2/fyle_rest_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `fyle-rest-auth-1.7.1/fyle_rest_auth/helpers.py` & `fyle_rest_auth-1.7.2/fyle_rest_auth/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,18 +52,21 @@
 
         tokens = auth.generate_fyle_refresh_token(authorization_code=authorization_code)
 
         employee_info = get_fyle_admin(tokens['access_token'], auth.get_origin_address(request))
         users = get_user_model()
 
         user, _ = users.objects.get_or_create(
-            user_id=employee_info['data']['user']['id'],
-            email=employee_info['data']['user']['email']
+            user_id=employee_info['data']['user']['id']
         )
 
+        if user and user.email != employee_info['data']['user']['email']:
+            user.email = employee_info['data']['user']['email']
+            user.save()
+
         AuthToken.objects.update_or_create(
             user=user,
             defaults={
                 'refresh_token': tokens['refresh_token']
             }
         )
 
@@ -71,15 +74,15 @@
         tokens['user'] = serializer(user).data
         tokens['user']['full_name'] = employee_info['data']['user']['full_name']
         tokens['user']['org_id'] = employee_info['data']['org']['id']
         tokens['user']['org_name'] = employee_info['data']['org']['name']
 
         # Update Fyle Credentials with latest healthy token
         if 'async_update_user' in settings.FYLE_REST_AUTH_SETTINGS \
-             and settings.FYLE_REST_AUTH_SETTINGS['async_update_user']:
+            and settings.FYLE_REST_AUTH_SETTINGS['async_update_user']:
             async_task(
                 'apps.workspaces.tasks.async_update_fyle_credentials',
                 employee_info['data']['org']['id'], tokens['refresh_token']
             )
 
         return tokens
 
@@ -107,18 +110,21 @@
 
         tokens = auth.refresh_access_token(refresh_token)
 
         employee_info = get_fyle_admin(tokens['access_token'], auth.get_origin_address(request))
         users = get_user_model()
 
         user, _ = users.objects.get_or_create(
-            user_id=employee_info['data']['user']['id'],
-            email=employee_info['data']['user']['email']
+            user_id=employee_info['data']['user']['id']
         )
 
+        if user and user.email != employee_info['data']['user']['email']:
+            user.email = employee_info['data']['user']['email']
+            user.save()
+
         AuthToken.objects.update_or_create(
             user=user,
             defaults={
                 'refresh_token': refresh_token
             }
         )
 
@@ -126,15 +132,15 @@
         tokens['user'] = serializer(user).data
         tokens['user']['full_name'] = employee_info['data']['user']['full_name']
         tokens['user']['org_id'] = employee_info['data']['org']['id']
         tokens['user']['org_name'] = employee_info['data']['org']['name']
 
         # Update Fyle Credentials with latest healthy token
         if 'async_update_user' in settings.FYLE_REST_AUTH_SETTINGS \
-             and settings.FYLE_REST_AUTH_SETTINGS['async_update_user']:
+            and settings.FYLE_REST_AUTH_SETTINGS['async_update_user']:
             async_task(
                 'apps.workspaces.tasks.async_update_fyle_credentials',
                 employee_info['data']['org']['id'], tokens['refresh_token']
             )
 
         if 'async_update_user_settings_api' in settings.FYLE_REST_AUTH_SETTINGS \
             and settings.FYLE_REST_AUTH_SETTINGS['async_update_user_settings_api']:
```

### Comparing `fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/0001_initial.py` & `fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/0002_auto_20200101_1205.py` & `fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/0002_auto_20200101_1205.py`

 * *Files identical despite different names*

### Comparing `fyle-rest-auth-1.7.1/fyle_rest_auth/migrations/0003_auto_20200107_0921.py` & `fyle_rest_auth-1.7.2/fyle_rest_auth/migrations/0003_auto_20200107_0921.py`

 * *Files identical despite different names*

### Comparing `fyle-rest-auth-1.7.1/fyle_rest_auth/urls.py` & `fyle_rest_auth-1.7.2/fyle_rest_auth/urls.py`

 * *Files identical despite different names*

### Comparing `fyle-rest-auth-1.7.1/fyle_rest_auth/utils.py` & `fyle_rest_auth-1.7.2/fyle_rest_auth/utils.py`

 * *Files identical despite different names*

### Comparing `fyle-rest-auth-1.7.1/fyle_rest_auth/views.py` & `fyle_rest_auth-1.7.2/fyle_rest_auth/views.py`

 * *Files identical despite different names*

### Comparing `fyle-rest-auth-1.7.1/fyle_rest_auth.egg-info/PKG-INFO` & `fyle_rest_auth-1.7.2/fyle_rest_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyle-rest-auth
-Version: 1.7.1
+Version: 1.7.2
 Summary: Django application to implement OAuth 2.0 using Fyle in Django rest framework
 Home-page: https://github.com/fylein/fyle-rest-auth
 Author: Shwetabh Kumar
 Author-email: shwetabh.kumar@fyle.in
 License: MIT
 Keywords: fyle,rest,django-rest-framework,api,python,oauth 2
 Classifier: Framework :: Django
```

### Comparing `fyle-rest-auth-1.7.1/fyle_rest_auth.egg-info/SOURCES.txt` & `fyle_rest_auth-1.7.2/fyle_rest_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fyle-rest-auth-1.7.1/setup.py` & `fyle_rest_auth-1.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='fyle-rest-auth',
-    version='1.7.1',
+    version='1.7.2',
     author='Shwetabh Kumar',
     author_email='shwetabh.kumar@fyle.in',
     description='Django application to implement OAuth 2.0 using Fyle in Django rest framework',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['fyle', 'rest', 'django-rest-framework', 'api', 'python', 'oauth 2'],
```

