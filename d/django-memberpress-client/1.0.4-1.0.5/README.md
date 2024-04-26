# Comparing `tmp/django-memberpress-client-1.0.4.tar.gz` & `tmp/django_memberpress_client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-memberpress-client-1.0.4.tar", last modified: Fri Nov 10 18:27:48 2023, max compression
+gzip compressed data, was "django_memberpress_client-1.0.5.tar", last modified: Fri Apr 26 19:17:09 2024, max compression
```

## Comparing `django-memberpress-client-1.0.4.tar` & `django_memberpress_client-1.0.5.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:27:48.245853 django-memberpress-client-1.0.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/LICENSE.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7326 2023-11-10 18:27:48.245853 django-memberpress-client-1.0.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6230 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:27:48.241853 django-memberpress-client-1.0.4/django_memberpress_client.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7326 2023-11-10 18:27:48.000000 django-memberpress-client-1.0.4/django_memberpress_client.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1724 2023-11-10 18:27:48.000000 django-memberpress-client-1.0.4/django_memberpress_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-11-10 18:27:48.000000 django-memberpress-client-1.0.4/django_memberpress_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2023-11-10 18:27:48.000000 django-memberpress-client-1.0.4/django_memberpress_client.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-11-10 18:27:48.000000 django-memberpress-client-1.0.4/django_memberpress_client.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2023-11-10 18:27:48.000000 django-memberpress-client-1.0.4/django_memberpress_client.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-11-10 18:27:48.000000 django-memberpress-client-1.0.4/django_memberpress_client.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:27:48.241853 django-memberpress-client-1.0.4/memberpress_client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      529 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/admin.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:27:48.241853 django-memberpress-client-1.0.4/memberpress_client/api/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/api/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:27:48.241853 django-memberpress-client-1.0.4/memberpress_client/api/v1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/api/v1/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      191 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/api/v1/urls.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      972 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/api/v1/views.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2048 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/apps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4566 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:27:48.245853 django-memberpress-client-1.0.4/memberpress_client/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      224 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/config/api_router.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1688 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/config/wsgi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14869 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4179 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/decorators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36960 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/events.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11901 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/member.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4320 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/memberpress.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7735 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/membership.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:27:48.245853 django-memberpress-client-1.0.4/memberpress_client/migrations/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6967 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/migrations/0001_initial.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      613 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/migrations/0002_auto_20221219_0316.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/migrations/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1880 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1854 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/receivers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:27:48.245853 django-memberpress-client-1.0.4/memberpress_client/settings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/settings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/settings/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8317 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/settings/local.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/settings/production.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4468 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/subscription.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:27:48.245853 django-memberpress-client-1.0.4/memberpress_client/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2061 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7298 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/tests/test_events.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2900 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/tests/test_member_nosubscription.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12976 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/tests/test_member_offline.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3649 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/tests/test_member_online.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3404 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/transaction.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      614 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/urls.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4312 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/memberpress_client/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1937 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-11-10 18:27:48.245853 django-memberpress-client-1.0.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3426 2023-11-10 18:24:43.000000 django-memberpress-client-1.0.4/setup.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2024-04-26 19:17:09.166452 django_memberpress_client-1.0.5/
+-rw-r--r--   0 travis     (501) staff       (20)     1074 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/LICENSE.txt
+-rw-r--r--   0 travis     (501) staff       (20)       18 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/MANIFEST.in
+-rw-r--r--   0 travis     (501) staff       (20)     7326 2024-04-26 19:17:09.166349 django_memberpress_client-1.0.5/PKG-INFO
+-rw-r--r--   0 travis     (501) staff       (20)     6230 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/README.md
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2024-04-26 19:17:09.165847 django_memberpress_client-1.0.5/django_memberpress_client.egg-info/
+-rw-r--r--   0 travis     (501) staff       (20)     7326 2024-04-26 19:17:09.000000 django_memberpress_client-1.0.5/django_memberpress_client.egg-info/PKG-INFO
+-rw-r--r--   0 travis     (501) staff       (20)     1791 2024-04-26 19:17:09.000000 django_memberpress_client-1.0.5/django_memberpress_client.egg-info/SOURCES.txt
+-rw-r--r--   0 travis     (501) staff       (20)        1 2024-04-26 19:17:09.000000 django_memberpress_client-1.0.5/django_memberpress_client.egg-info/dependency_links.txt
+-rw-r--r--   0 travis     (501) staff       (20)       85 2024-04-26 19:17:09.000000 django_memberpress_client-1.0.5/django_memberpress_client.egg-info/entry_points.txt
+-rw-r--r--   0 travis     (501) staff       (20)        1 2024-04-26 19:17:09.000000 django_memberpress_client-1.0.5/django_memberpress_client.egg-info/not-zip-safe
+-rw-r--r--   0 travis     (501) staff       (20)       85 2024-04-26 19:17:09.000000 django_memberpress_client-1.0.5/django_memberpress_client.egg-info/requires.txt
+-rw-r--r--   0 travis     (501) staff       (20)       19 2024-04-26 19:17:09.000000 django_memberpress_client-1.0.5/django_memberpress_client.egg-info/top_level.txt
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2024-04-26 19:17:09.163046 django_memberpress_client-1.0.5/memberpress_client/
+-rw-r--r--   0 travis     (501) staff       (20)       71 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)      529 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/admin.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2024-04-26 19:17:09.163170 django_memberpress_client-1.0.5/memberpress_client/api/
+-rw-r--r--   0 travis     (501) staff       (20)        0 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/api/__init__.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2024-04-26 19:17:09.163488 django_memberpress_client-1.0.5/memberpress_client/api/v1/
+-rw-r--r--   0 travis     (501) staff       (20)        0 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/api/v1/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)      191 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/api/v1/urls.py
+-rw-r--r--   0 travis     (501) staff       (20)      972 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/api/v1/views.py
+-rw-r--r--   0 travis     (501) staff       (20)     2048 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/apps.py
+-rw-r--r--   0 travis     (501) staff       (20)     4522 2024-04-25 14:22:41.000000 django_memberpress_client-1.0.5/memberpress_client/client.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2024-04-26 19:17:09.163880 django_memberpress_client-1.0.5/memberpress_client/config/
+-rw-r--r--   0 travis     (501) staff       (20)        0 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/config/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)      224 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/config/api_router.py
+-rw-r--r--   0 travis     (501) staff       (20)     1688 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/config/wsgi.py
+-rw-r--r--   0 travis     (501) staff       (20)    14869 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/constants.py
+-rw-r--r--   0 travis     (501) staff       (20)     4179 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/decorators.py
+-rw-r--r--   0 travis     (501) staff       (20)    36960 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/events.py
+-rw-r--r--   0 travis     (501) staff       (20)    11901 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/member.py
+-rw-r--r--   0 travis     (501) staff       (20)     4320 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/memberpress.py
+-rw-r--r--   0 travis     (501) staff       (20)     7735 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/membership.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2024-04-26 19:17:09.164375 django_memberpress_client-1.0.5/memberpress_client/migrations/
+-rw-r--r--   0 travis     (501) staff       (20)     6967 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/migrations/0001_initial.py
+-rw-r--r--   0 travis     (501) staff       (20)      613 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/migrations/0002_auto_20221219_0316.py
+-rw-r--r--   0 travis     (501) staff       (20)      468 2024-04-26 19:09:09.000000 django_memberpress_client-1.0.5/memberpress_client/migrations/0003_alter_memberpresseventlog_id.py
+-rw-r--r--   0 travis     (501) staff       (20)        0 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/migrations/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)     1880 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/models.py
+-rw-r--r--   0 travis     (501) staff       (20)     1854 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/receivers.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2024-04-26 19:17:09.164797 django_memberpress_client-1.0.5/memberpress_client/settings/
+-rw-r--r--   0 travis     (501) staff       (20)        0 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/settings/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)     1738 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/settings/common.py
+-rw-r--r--   0 travis     (501) staff       (20)     8317 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/settings/local.py
+-rw-r--r--   0 travis     (501) staff       (20)      291 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/settings/production.py
+-rw-r--r--   0 travis     (501) staff       (20)     4468 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/subscription.py
+drwxr-xr-x   0 travis     (501) staff       (20)        0 2024-04-26 19:17:09.165681 django_memberpress_client-1.0.5/memberpress_client/tests/
+-rw-r--r--   0 travis     (501) staff       (20)        0 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/tests/__init__.py
+-rw-r--r--   0 travis     (501) staff       (20)     2727 2024-04-26 19:09:09.000000 django_memberpress_client-1.0.5/memberpress_client/tests/test_client.py
+-rw-r--r--   0 travis     (501) staff       (20)     7298 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/tests/test_events.py
+-rw-r--r--   0 travis     (501) staff       (20)     2900 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/tests/test_member_nosubscription.py
+-rw-r--r--   0 travis     (501) staff       (20)    12976 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/tests/test_member_offline.py
+-rw-r--r--   0 travis     (501) staff       (20)     3649 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/tests/test_member_online.py
+-rw-r--r--   0 travis     (501) staff       (20)     3404 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/transaction.py
+-rw-r--r--   0 travis     (501) staff       (20)      614 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/urls.py
+-rw-r--r--   0 travis     (501) staff       (20)     4312 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/memberpress_client/utils.py
+-rw-r--r--   0 travis     (501) staff       (20)     1937 2024-04-26 19:16:35.000000 django_memberpress_client-1.0.5/pyproject.toml
+-rw-r--r--   0 travis     (501) staff       (20)       67 2024-04-26 19:17:09.166678 django_memberpress_client-1.0.5/setup.cfg
+-rw-r--r--   0 travis     (501) staff       (20)     3426 2024-04-24 19:03:59.000000 django_memberpress_client-1.0.5/setup.py
```

### Comparing `django-memberpress-client-1.0.4/LICENSE.txt` & `django_memberpress_client-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/PKG-INFO` & `django_memberpress_client-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-memberpress-client
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Django plugin to add Memberpress REST API and Webhook integrations.
 Home-page: https://github.com/lpm0073/django-memberpress-client
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Project-URL: Homepage, https://github.com/lpm0073/django-memberpress-client
 Project-URL: Bug Tracker, https://github.com/lpm0073/django-memberpress-client/issues
 Project-URL: Repository, https://github.com/lpm0073/django-memberpress-client
```

### Comparing `django-memberpress-client-1.0.4/README.md` & `django_memberpress_client-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/django_memberpress_client.egg-info/PKG-INFO` & `django_memberpress_client-1.0.5/django_memberpress_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-memberpress-client
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Django plugin to add Memberpress REST API and Webhook integrations.
 Home-page: https://github.com/lpm0073/django-memberpress-client
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Project-URL: Homepage, https://github.com/lpm0073/django-memberpress-client
 Project-URL: Bug Tracker, https://github.com/lpm0073/django-memberpress-client/issues
 Project-URL: Repository, https://github.com/lpm0073/django-memberpress-client
```

### Comparing `django-memberpress-client-1.0.4/django_memberpress_client.egg-info/SOURCES.txt` & `django_memberpress_client-1.0.5/django_memberpress_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 memberpress_client/api/v1/urls.py
 memberpress_client/api/v1/views.py
 memberpress_client/config/__init__.py
 memberpress_client/config/api_router.py
 memberpress_client/config/wsgi.py
 memberpress_client/migrations/0001_initial.py
 memberpress_client/migrations/0002_auto_20221219_0316.py
+memberpress_client/migrations/0003_alter_memberpresseventlog_id.py
 memberpress_client/migrations/__init__.py
 memberpress_client/settings/__init__.py
 memberpress_client/settings/common.py
 memberpress_client/settings/local.py
 memberpress_client/settings/production.py
 memberpress_client/tests/__init__.py
 memberpress_client/tests/test_client.py
```

### Comparing `django-memberpress-client-1.0.4/memberpress_client/admin.py` & `django_memberpress_client-1.0.5/memberpress_client/admin.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/api/v1/views.py` & `django_memberpress_client-1.0.5/memberpress_client/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/apps.py` & `django_memberpress_client-1.0.5/memberpress_client/apps.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/client.py` & `django_memberpress_client-1.0.5/memberpress_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,25 +42,25 @@
     @property
     def headers(self) -> dict:
         return {
             f"{settings.MEMBERPRESS_API_KEY_NAME}": f"{settings.MEMBERPRESS_API_KEY}",
         }
 
     @request_manager
-    def post(self, path, data=None, host=None, operation="") -> json:
-        url = self.get_url(path, host=host)
+    def post(self, path, data=None, operation="") -> json:
+        url = self.get_url(path)
         log_pretrip(caller=inspect.currentframe().f_code.co_name, url=url, data=data, operation=operation)
         response = requests.post(url, data=data, headers=self.headers)
         log_postrip(caller=inspect.currentframe().f_code.co_name, path=url, response=response, operation=operation)
         response.raise_for_status()
         return response.json()
 
     @request_manager
-    def patch(self, path, data=None, host=None, headers=None, json=True, operation=""):
-        url = self.get_url(path, host=host)
+    def patch(self, path, data=None, headers=None, json=True, operation=""):
+        url = self.get_url(path)
         if not headers:
             headers = self.headers
 
         log_pretrip(caller=inspect.currentframe().f_code.co_name, url=url, data=data, operation=operation)
         response = requests.patch(url, json=data, headers=headers)
         log_postrip(caller=inspect.currentframe().f_code.co_name, path=url, response=response, operation=operation)
         response.raise_for_status()
```

### Comparing `django-memberpress-client-1.0.4/memberpress_client/config/wsgi.py` & `django_memberpress_client-1.0.5/memberpress_client/config/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/constants.py` & `django_memberpress_client-1.0.5/memberpress_client/constants.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/decorators.py` & `django_memberpress_client-1.0.5/memberpress_client/decorators.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/events.py` & `django_memberpress_client-1.0.5/memberpress_client/events.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/member.py` & `django_memberpress_client-1.0.5/memberpress_client/member.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/memberpress.py` & `django_memberpress_client-1.0.5/memberpress_client/memberpress.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/membership.py` & `django_memberpress_client-1.0.5/memberpress_client/membership.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/migrations/0001_initial.py` & `django_memberpress_client-1.0.5/memberpress_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/migrations/0002_auto_20221219_0316.py` & `django_memberpress_client-1.0.5/memberpress_client/migrations/0002_auto_20221219_0316.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/models.py` & `django_memberpress_client-1.0.5/memberpress_client/models.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/receivers.py` & `django_memberpress_client-1.0.5/memberpress_client/receivers.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/settings/common.py` & `django_memberpress_client-1.0.5/memberpress_client/settings/common.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/settings/local.py` & `django_memberpress_client-1.0.5/memberpress_client/settings/local.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/subscription.py` & `django_memberpress_client-1.0.5/memberpress_client/subscription.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/tests/test_client.py` & `django_memberpress_client-1.0.5/memberpress_client/tests/test_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from unittest import TestCase
 from unittest.mock import patch
 
 from django.core.cache import cache
 
 from memberpress_client.client import MemberpressAPIClient
 
+
 class MockResponse:
     def __init__(self, json_data, status_code):
         self.json_data = json_data
         self.status_code = status_code
 
     def json(self):
         return self.json_data
-    
+
     def raise_for_status(self):
         pass
 
 
 class TestClient(TestCase):
 
     def setUp(self):
         cache.clear()
 
+    @patch("memberpress_client.client.requests.patch", return_value=MockResponse({"foo": "bar"}, 200))
+    @patch("memberpress_client.client.requests.post", return_value=MockResponse({"foo": "bar"}, 200))
     @patch("memberpress_client.client.requests.get", return_value=MockResponse({"foo": "bar"}, 200))
-    def test_response_caching(self, mock_get):
+    def test_response_caching(self, mock_get, mock_post, mock_patch):
         client = MemberpressAPIClient()
         assert mock_get.call_count == 0
         # first call should make a request
         client.get("test")
         assert mock_get.call_count == 1
         # second call should retrieve from cache
         client.get("test")
@@ -46,8 +49,19 @@
         assert mock_get.call_count == 3
         # third call with same params but different values should make a request
         client.get("test", params={"param_1": "value_1", "param_2": "value_3"})
         assert mock_get.call_count == 4
         # call again with same params but caching disabled should make a request
         client.get("test", params={"param_1": "value_1", "param_2": "value_3"}, enable_caching=False)
         assert mock_get.call_count == 5
-        
+        client.post("test-post", {"input": "post data"})
+        mock_post.assert_called_with(
+            client.get_url("test-post"),
+            data={"input": "post data"},
+            headers=client.headers
+        )
+        client.patch("test-patch", {"input": "patch data"})
+        mock_patch.assert_called_with(
+            client.get_url("test-patch"),
+            json={"input": "patch data"},
+            headers=client.headers
+        )
```

### Comparing `django-memberpress-client-1.0.4/memberpress_client/tests/test_events.py` & `django_memberpress_client-1.0.5/memberpress_client/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/tests/test_member_nosubscription.py` & `django_memberpress_client-1.0.5/memberpress_client/tests/test_member_nosubscription.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/tests/test_member_offline.py` & `django_memberpress_client-1.0.5/memberpress_client/tests/test_member_offline.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/tests/test_member_online.py` & `django_memberpress_client-1.0.5/memberpress_client/tests/test_member_online.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/transaction.py` & `django_memberpress_client-1.0.5/memberpress_client/transaction.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/urls.py` & `django_memberpress_client-1.0.5/memberpress_client/urls.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/memberpress_client/utils.py` & `django_memberpress_client-1.0.5/memberpress_client/utils.py`

 * *Files identical despite different names*

### Comparing `django-memberpress-client-1.0.4/pyproject.toml` & `django_memberpress_client-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 #------------------------------------------------------------------------------
 # PyPi meta data
 #------------------------------------------------------------------------------
 [project]
 name = "django-memberpress-client"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Lawrence McDaniel", email="lpm0073@gmail.com" }
 ]
 description = "A Django plugin to add Memberpress REST API and Webhook integrations."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `django-memberpress-client-1.0.4/setup.py` & `django_memberpress_client-1.0.5/setup.py`

 * *Files identical despite different names*

