# Comparing `tmp/django-paypal-plus-1.0.1.tar.gz` & `tmp/django-paypal-plus-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-paypal-plus-1.0.1.tar", last modified: Thu Mar 21 10:52:19 2024, max compression
+gzip compressed data, was "django-paypal-plus-1.1.0.tar", last modified: Fri Apr 26 10:25:21 2024, max compression
```

## Comparing `django-paypal-plus-1.0.1.tar` & `django-paypal-plus-1.1.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-03-21 10:52:19.066117 django-paypal-plus-1.0.1/
--rw-r--r--   0 timtam     (502) staff       (20)     1113 2024-01-30 03:41:51.000000 django-paypal-plus-1.0.1/LICENSE
--rw-r--r--   0 timtam     (502) staff       (20)       23 2024-01-30 03:41:51.000000 django-paypal-plus-1.0.1/MANIFEST.in
--rw-r--r--   0 timtam     (502) staff       (20)      975 2024-03-21 10:52:19.065874 django-paypal-plus-1.0.1/PKG-INFO
--rw-r--r--   0 timtam     (502) staff       (20)     2341 2024-02-20 08:14:41.000000 django-paypal-plus-1.0.1/README.md
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-03-21 10:52:19.055868 django-paypal-plus-1.0.1/django_paypal/
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-03-21 10:52:19.056338 django-paypal-plus-1.0.1/django_paypal/.ruff_cache/
--rw-r--r--   0 timtam     (502) staff       (20)        1 2024-01-30 05:07:59.000000 django-paypal-plus-1.0.1/django_paypal/.ruff_cache/.gitignore
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-03-21 10:52:19.056528 django-paypal-plus-1.0.1/django_paypal/.ruff_cache/0.1.15/
--rw-r--r--   0 timtam     (502) staff       (20)    24879 2024-02-06 06:48:19.000000 django-paypal-plus-1.0.1/django_paypal/.ruff_cache/0.1.15/10239535276270870560
--rw-r--r--   0 timtam     (502) staff       (20)       43 2024-01-30 05:07:59.000000 django-paypal-plus-1.0.1/django_paypal/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0 timtam     (502) staff       (20)       22 2024-03-21 10:48:34.000000 django-paypal-plus-1.0.1/django_paypal/__init__.py
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-03-21 10:52:19.061913 django-paypal-plus-1.0.1/django_paypal/__pycache__/
--rw-r--r--   0 timtam     (502) staff       (20)      193 2024-02-05 06:09:00.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      205 2024-02-02 07:31:19.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      667 2024-02-06 06:48:48.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/admin.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)    22441 2024-02-05 07:54:49.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/api_types.cpython-311.pyc
--rw-r--r--   0 timtam     (502) staff       (20)    15871 2024-02-07 05:49:27.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/api_types.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      692 2024-02-05 09:12:15.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/exceptions.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     8411 2024-02-07 05:29:21.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     1614 2024-02-05 06:09:00.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     1097 2024-02-06 06:48:48.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      348 2024-02-06 02:49:18.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/signals.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      362 2024-02-02 06:09:52.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      447 2024-01-31 06:16:42.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     2374 2024-02-07 05:43:42.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/webhooks.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)    15560 2024-02-05 07:54:18.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/wrappers.cpython-311.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     8464 2024-02-07 08:27:09.000000 django-paypal-plus-1.0.1/django_paypal/__pycache__/wrappers.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      315 2024-02-06 06:48:04.000000 django-paypal-plus-1.0.1/django_paypal/admin.py
--rw-r--r--   0 timtam     (502) staff       (20)     9971 2024-02-07 05:49:26.000000 django-paypal-plus-1.0.1/django_paypal/api_types.py
--rw-r--r--   0 timtam     (502) staff       (20)      207 2024-02-05 09:12:13.000000 django-paypal-plus-1.0.1/django_paypal/exceptions.py
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-03-21 10:52:19.063356 django-paypal-plus-1.0.1/django_paypal/migrations/
--rw-r--r--   0 timtam     (502) staff       (20)     7840 2024-01-30 03:41:51.000000 django-paypal-plus-1.0.1/django_paypal/migrations/0001_initial.py
--rw-r--r--   0 timtam     (502) staff       (20)     1495 2024-01-30 03:41:51.000000 django-paypal-plus-1.0.1/django_paypal/migrations/0002_auto_20171002_1551.py
--rw-r--r--   0 timtam     (502) staff       (20)     1573 2024-01-30 03:42:26.000000 django-paypal-plus-1.0.1/django_paypal/migrations/0003_auto_20200124_1528.py
--rw-r--r--   0 timtam     (502) staff       (20)     1446 2024-01-30 03:42:26.000000 django-paypal-plus-1.0.1/django_paypal/migrations/0004_paypalpayment_related_resource_state.py
--rw-r--r--   0 timtam     (502) staff       (20)     4611 2024-02-07 05:30:57.000000 django-paypal-plus-1.0.1/django_paypal/migrations/0005_auto_20240207_0630.py
--rw-r--r--   0 timtam     (502) staff       (20)        0 2024-01-30 03:41:51.000000 django-paypal-plus-1.0.1/django_paypal/migrations/__init__.py
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-03-21 10:52:19.064464 django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/
--rw-r--r--   0 timtam     (502) staff       (20)     4088 2024-01-31 07:22:43.000000 django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/0001_initial.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     1162 2024-01-31 07:22:43.000000 django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/0002_auto_20171002_1551.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     1319 2024-01-31 07:22:43.000000 django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/0003_auto_20200124_1528.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     1347 2024-01-31 07:22:43.000000 django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/0004_paypalpayment_related_resource_state.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     2713 2024-02-07 05:40:35.000000 django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/0005_auto_20240207_0630.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      195 2024-01-31 07:22:43.000000 django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     9481 2024-02-07 05:29:19.000000 django-paypal-plus-1.0.1/django_paypal/models.py
--rw-r--r--   0 timtam     (502) staff       (20)     1304 2024-01-30 05:07:08.000000 django-paypal-plus-1.0.1/django_paypal/ruff.toml
--rw-r--r--   0 timtam     (502) staff       (20)     1281 2024-02-06 06:48:04.000000 django-paypal-plus-1.0.1/django_paypal/settings.py
--rw-r--r--   0 timtam     (502) staff       (20)      192 2024-02-06 02:48:11.000000 django-paypal-plus-1.0.1/django_paypal/signals.py
--rw-r--r--   0 timtam     (502) staff       (20)      174 2024-02-02 06:09:49.000000 django-paypal-plus-1.0.1/django_paypal/urls.py
--rw-r--r--   0 timtam     (502) staff       (20)      213 2024-01-30 03:41:51.000000 django-paypal-plus-1.0.1/django_paypal/utils.py
--rw-r--r--   0 timtam     (502) staff       (20)     2430 2024-03-21 10:46:38.000000 django-paypal-plus-1.0.1/django_paypal/webhooks.py
--rw-r--r--   0 timtam     (502) staff       (20)    10412 2024-02-07 08:27:06.000000 django-paypal-plus-1.0.1/django_paypal/wrappers.py
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-03-21 10:52:19.065592 django-paypal-plus-1.0.1/django_paypal_plus.egg-info/
--rw-r--r--   0 timtam     (502) staff       (20)      975 2024-03-21 10:52:19.000000 django-paypal-plus-1.0.1/django_paypal_plus.egg-info/PKG-INFO
--rw-r--r--   0 timtam     (502) staff       (20)     2215 2024-03-21 10:52:19.000000 django-paypal-plus-1.0.1/django_paypal_plus.egg-info/SOURCES.txt
--rw-r--r--   0 timtam     (502) staff       (20)        1 2024-03-21 10:52:19.000000 django-paypal-plus-1.0.1/django_paypal_plus.egg-info/dependency_links.txt
--rw-r--r--   0 timtam     (502) staff       (20)        1 2024-02-20 08:20:44.000000 django-paypal-plus-1.0.1/django_paypal_plus.egg-info/not-zip-safe
--rw-r--r--   0 timtam     (502) staff       (20)       73 2024-03-21 10:52:19.000000 django-paypal-plus-1.0.1/django_paypal_plus.egg-info/requires.txt
--rw-r--r--   0 timtam     (502) staff       (20)       39 2024-03-21 10:52:19.000000 django-paypal-plus-1.0.1/django_paypal_plus.egg-info/top_level.txt
--rw-r--r--   0 timtam     (502) staff       (20)       38 2024-03-21 10:52:19.066158 django-paypal-plus-1.0.1/setup.cfg
--rwxr-xr-x   0 timtam     (502) staff       (20)     2698 2024-02-06 06:48:04.000000 django-paypal-plus-1.0.1/setup.py
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.502114 django-paypal-plus-1.1.0/
+-rw-r--r--   0 timtam     (502) staff       (20)     1113 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/LICENSE
+-rw-r--r--   0 timtam     (502) staff       (20)       23 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/MANIFEST.in
+-rw-r--r--   0 timtam     (502) staff       (20)      975 2024-04-26 10:25:21.501831 django-paypal-plus-1.1.0/PKG-INFO
+-rw-r--r--   0 timtam     (502) staff       (20)     2341 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/README.md
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.492431 django-paypal-plus-1.1.0/django_paypal/
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.492783 django-paypal-plus-1.1.0/django_paypal/.ruff_cache/
+-rw-r--r--   0 timtam     (502) staff       (20)        1 2024-01-30 05:07:59.000000 django-paypal-plus-1.1.0/django_paypal/.ruff_cache/.gitignore
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.493025 django-paypal-plus-1.1.0/django_paypal/.ruff_cache/0.1.15/
+-rw-r--r--   0 timtam     (502) staff       (20)      740 2024-04-24 05:35:37.000000 django-paypal-plus-1.1.0/django_paypal/.ruff_cache/0.1.15/10239535276270870560
+-rw-r--r--   0 timtam     (502) staff       (20)       43 2024-01-30 05:07:59.000000 django-paypal-plus-1.1.0/django_paypal/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0 timtam     (502) staff       (20)       22 2024-04-26 10:23:00.000000 django-paypal-plus-1.1.0/django_paypal/__init__.py
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.497383 django-paypal-plus-1.1.0/django_paypal/__pycache__/
+-rw-r--r--   0 timtam     (502) staff       (20)      193 2024-02-05 06:09:00.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      205 2024-04-26 04:51:50.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      667 2024-04-24 03:34:05.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/admin.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)    22441 2024-02-05 07:54:49.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/api_types.cpython-311.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)    15871 2024-04-24 03:34:04.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/api_types.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      692 2024-04-24 03:34:05.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/exceptions.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     8411 2024-04-26 04:51:50.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     1614 2024-02-05 06:09:00.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     1097 2024-04-26 04:51:51.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      348 2024-04-24 03:34:05.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/signals.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      362 2024-02-02 06:09:52.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      447 2024-01-31 06:16:42.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     2588 2024-04-26 05:07:15.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/webhooks.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)    15560 2024-02-05 07:54:18.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/wrappers.cpython-311.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     8464 2024-04-26 04:51:51.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/wrappers.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      315 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/admin.py
+-rw-r--r--   0 timtam     (502) staff       (20)     9971 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/api_types.py
+-rw-r--r--   0 timtam     (502) staff       (20)      207 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/exceptions.py
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.498825 django-paypal-plus-1.1.0/django_paypal/migrations/
+-rw-r--r--   0 timtam     (502) staff       (20)     7840 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0001_initial.py
+-rw-r--r--   0 timtam     (502) staff       (20)     1495 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0002_auto_20171002_1551.py
+-rw-r--r--   0 timtam     (502) staff       (20)     1573 2024-01-30 03:42:26.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0003_auto_20200124_1528.py
+-rw-r--r--   0 timtam     (502) staff       (20)     1446 2024-01-30 03:42:26.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0004_paypalpayment_related_resource_state.py
+-rw-r--r--   0 timtam     (502) staff       (20)     4611 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0005_auto_20240207_0630.py
+-rw-r--r--   0 timtam     (502) staff       (20)      755 2024-04-26 10:20:15.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0006_auto_20240424_0727.py
+-rw-r--r--   0 timtam     (502) staff       (20)        0 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__init__.py
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.500497 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/
+-rw-r--r--   0 timtam     (502) staff       (20)     4088 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0001_initial.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     1162 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0002_auto_20171002_1551.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     1319 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0003_auto_20200124_1528.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     1347 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0004_paypalpayment_related_resource_state.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     2713 2024-04-24 03:34:09.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0005_auto_20240207_0630.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      835 2024-04-24 05:27:44.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0006_auto_20240424_0727.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      195 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     9617 2024-04-26 10:20:15.000000 django-paypal-plus-1.1.0/django_paypal/models.py
+-rw-r--r--   0 timtam     (502) staff       (20)     1304 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/ruff.toml
+-rw-r--r--   0 timtam     (502) staff       (20)     1293 2024-04-26 10:20:15.000000 django-paypal-plus-1.1.0/django_paypal/settings.py
+-rw-r--r--   0 timtam     (502) staff       (20)      192 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/signals.py
+-rw-r--r--   0 timtam     (502) staff       (20)      174 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/urls.py
+-rw-r--r--   0 timtam     (502) staff       (20)      213 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/django_paypal/utils.py
+-rw-r--r--   0 timtam     (502) staff       (20)     2383 2024-04-26 10:20:15.000000 django-paypal-plus-1.1.0/django_paypal/webhooks.py
+-rw-r--r--   0 timtam     (502) staff       (20)    11435 2024-04-26 10:20:15.000000 django-paypal-plus-1.1.0/django_paypal/wrappers.py
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.501460 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/
+-rw-r--r--   0 timtam     (502) staff       (20)      975 2024-04-26 10:25:21.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/PKG-INFO
+-rw-r--r--   0 timtam     (502) staff       (20)     2343 2024-04-26 10:25:21.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 timtam     (502) staff       (20)        1 2024-04-26 10:25:21.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 timtam     (502) staff       (20)        1 2024-02-20 08:20:44.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/not-zip-safe
+-rw-r--r--   0 timtam     (502) staff       (20)       73 2024-04-26 10:25:21.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/requires.txt
+-rw-r--r--   0 timtam     (502) staff       (20)       39 2024-04-26 10:25:21.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/top_level.txt
+-rw-r--r--   0 timtam     (502) staff       (20)       38 2024-04-26 10:25:21.502159 django-paypal-plus-1.1.0/setup.cfg
+-rwxr-xr-x   0 timtam     (502) staff       (20)     2698 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/setup.py
```

### Comparing `django-paypal-plus-1.0.1/LICENSE` & `django-paypal-plus-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/PKG-INFO` & `django-paypal-plus-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-paypal-plus
-Version: 1.0.1
+Version: 1.1.0
 Summary: Django integration of PayPal's Orders v2 API
 Home-page: https://github.com/ParticulateSolutions/django-paypal-plus
 Author: Particulate Solutions GmbH
 Author-email: tech@particulate.me
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-paypal-plus-1.0.1/README.md` & `django-paypal-plus-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/__pycache__/admin.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/__pycache__/admin.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Feb  6 06:48:04 2024 UTC, .py size: 315 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 24d6 c165 3b01 0000  U.......$..e;...
+00000000: 550d 0d0a 0000 0000 b33b 2766 3b01 0000  U........;'f;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000050: 8400 6405 6501 6a05 8303 5a06 6501 6a07  ..d.e.j...Z.e.j.
 00000060: a008 6503 6506 a102 0100 4700 6406 6407  ..e.e.....G.d.d.
 00000070: 8400 6407 6501 6a05 8303 5a09 6501 6a07  ..d.e.j...Z.e.j.
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/__pycache__/api_types.cpython-311.pyc` & `django-paypal-plus-1.1.0/django_paypal/__pycache__/api_types.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/__pycache__/api_types.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/__pycache__/api_types.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Feb  7 05:49:26 2024 UTC, .py size: 9971 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 e619 c365 f326 0000  U..........e.&..
+00000000: 550d 0d0a 0000 0000 b33b 2766 f326 0000  U........;'f.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e203 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6505 6404 1900 5a0b 6505  m.Z...e.d...Z.e.
 00000070: 6405 1900 5a0c 6505 6406 1900 5a0d 6501  d...Z.e.d...Z.e.
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/__pycache__/exceptions.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/__pycache__/exceptions.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Feb  5 09:12:13 2024 UTC, .py size: 207 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6da6 c065 cf00 0000  U.......m..e....
+00000000: 550d 0d0a 0000 0000 b33b 2766 cf00 0000  U........;'f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 4700 6404 6405  ..d.e...Z.G.d.d.
 00000050: 8400 6405 6501 8303 5a03 4700 6406 6407  ..d.e...Z.G.d.d.
 00000060: 8400 6407 6504 8303 5a05 6408 5300 2909  ..d.e...Z.d.S.).
 00000070: e900 0000 0029 01da 1052 6571 7565 7374  .....)...Request
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/__pycache__/models.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/__pycache__/models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Feb  7 05:29:19 2024 UTC, .py size: 9481 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2f15 c365 0925 0000  U......./..e.%..
+00000000: 550d 0d0a 0000 0000 cd31 2b66 0925 0000  U........1+f.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 1e01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0c 0100 6400 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/__pycache__/settings.cpython-311.pyc` & `django-paypal-plus-1.1.0/django_paypal/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/__pycache__/settings.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/__pycache__/settings.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Feb  6 06:48:04 2024 UTC, .py size: 1281 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 24d6 c165 0105 0000  U.......$..e....
+00000000: 550d 0d0a 0000 0000 cd31 2b66 0105 0000  U........1+f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6503 5a04 6505 6501 6403  m.Z...e.Z.e.e.d.
 00000050: 6404 8303 5a06 6505 6501 6405 6404 8303  d...Z.e.e.d.d...
 00000060: 5a07 6505 6501 6406 6407 8303 5a08 6505  Z.e.e.d.d...Z.e.
 00000070: 6501 6408 6409 8303 5a09 6505 6501 640a  e.d.d...Z.e.e.d.
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/__pycache__/webhooks.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/__pycache__/webhooks.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Feb  7 05:43:39 2024 UTC, .py size: 2251 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,149 +1,162 @@
-00000000: 550d 0d0a 0000 0000 8b18 c365 cb08 0000  U..........e....
+00000000: 550d 0d0a 0000 0000 8036 2b66 2a0a 0000  U........6+f*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6400 6407 6c0d  d.l.m.Z...d.d.l.
 00000080: 6d0e 5a0e 0100 6408 6409 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
 00000090: 0100 6408 640a 6c11 6d12 5a12 6d13 5a13  ..d.d.l.m.Z.m.Z.
-000000a0: 0100 6408 640b 6c14 6d15 5a15 6d16 5a16  ..d.d.l.m.Z.m.Z.
-000000b0: 0100 6408 640c 6c17 6d18 5a18 0100 6400  ..d.d.l.m.Z...d.
-000000c0: 6403 6c19 6d05 5a1a 0100 4700 640d 640e  d.l.m.Z...G.d.d.
-000000d0: 8400 640e 8302 5a1b 6508 6518 6503 651c  ..d...Z.e.e.e.e.
-000000e0: 6502 6602 1900 640f 9c03 6410 6411 8404  e.f...d...d.d...
-000000f0: 5a1d 650a 650c 6412 6413 8d02 4700 6414  Z.e.e.d.d...G.d.
-00000100: 6415 8400 6415 650e 8303 8301 5a1e 6401  d...d.e.....Z.d.
-00000110: 5300 2916 e900 0000 004e 2902 da03 416e  S.)......N)...An
-00000120: 79da 0444 6963 7429 01da 0873 6574 7469  y..Dict)...setti
-00000130: 6e67 7329 02da 0c48 7474 7052 6573 706f  ngs)...HttpRespo
-00000140: 6e73 65da 0b48 7474 7052 6571 7565 7374  nse..HttpRequest
-00000150: 2901 da10 6d65 7468 6f64 5f64 6563 6f72  )...method_decor
-00000160: 6174 6f72 2901 da0b 6373 7266 5f65 7865  ator)...csrf_exe
-00000170: 6d70 7429 01da 0456 6965 77e9 0100 0000  mpt)...View.....
-00000180: 2901 da12 4150 4941 7574 6843 7265 6465  )...APIAuthCrede
-00000190: 6e74 6961 6c73 2902 da0d 5061 7970 616c  ntials)...Paypal
-000001a0: 5765 6268 6f6f 6bda 1250 6179 7061 6c57  Webhook..PaypalW
-000001b0: 6562 686f 6f6b 4576 656e 7429 02da 0e6f  ebhookEvent)...o
-000001c0: 7264 6572 5f61 7070 726f 7665 64da 0f6f  rder_approved..o
-000001d0: 7264 6572 5f63 6f6d 706c 6574 6564 2901  rder_completed).
-000001e0: da0d 5061 7970 616c 5772 6170 7065 7263  ..PaypalWrapperc
-000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0300 0000 4000 0000 7316 0000 0065 005a  ....@...s....e.Z
-00000210: 0164 005a 0264 0164 0264 0367 035a 0364  .d.Z.d.d.d.g.Z.d
-00000220: 0453 0029 05da 0d57 6562 686f 6f6b 4576  .S.)...WebhookEv
-00000230: 656e 7473 fa18 4348 4543 4b4f 5554 2e4f  ents..CHECKOUT.O
-00000240: 5244 4552 2e43 4f4d 504c 4554 4544 fa17  RDER.COMPLETED..
-00000250: 4348 4543 4b4f 5554 2e4f 5244 4552 2e41  CHECKOUT.ORDER.A
-00000260: 5050 524f 5645 447a 2243 4845 434b 4f55  PPROVEDz"CHECKOU
-00000270: 542e 5041 594d 454e 542d 4150 5052 4f56  T.PAYMENT-APPROV
-00000280: 414c 2e52 4556 4552 5345 444e 2904 da08  AL.REVERSEDN)...
-00000290: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000002a0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000002b0: 5f5f da06 4f52 4445 5253 a900 7218 0000  __..ORDERS..r...
-000002c0: 0072 1800 0000 fa5d 2f55 7365 7273 2f74  .r.....]/Users/t
-000002d0: 696d 7461 6d2f 2e70 7965 6e76 2f76 6572  imtam/.pyenv/ver
-000002e0: 7369 6f6e 732f 7366 2d33 2e38 2e31 322f  sions/sf-3.8.12/
-000002f0: 6c69 622f 7079 7468 6f6e 332e 382f 7369  lib/python3.8/si
-00000300: 7465 2d70 6163 6b61 6765 732f 646a 616e  te-packages/djan
-00000310: 676f 5f70 6179 7061 6c2f 7765 6268 6f6f  go_paypal/webhoo
-00000320: 6b73 2e70 7972 1100 0000 1100 0000 7302  ks.pyr........s.
-00000330: 0000 0008 0172 1100 0000 2903 da07 7265  .....r....)...re
-00000340: 7175 6573 74da 0e70 6179 7061 6c5f 7772  quest..paypal_wr
-00000350: 6170 7065 72da 0770 6179 6c6f 6164 6303  apper..payloadc.
-00000360: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-00000370: 0000 0043 0000 0073 5a00 0000 7400 6a01  ...C...sZ...t.j.
-00000380: 7356 7402 6a03 6a04 7c00 a005 a100 6401  sVt.j.j.|.....d.
-00000390: 8d01 7d03 7c01 a006 7c00 7c03 6a07 a102  ..}.|...|.|.j...
-000003a0: 0100 7c02 7c03 7c02 a004 6402 a101 7240  ..|.|.|...d...r@
-000003b0: 7c02 6402 1900 6403 1900 6e02 6400 6404  |.d...d...n.d.d.
-000003c0: 9c03 7d04 7408 6a03 6a09 6600 7c04 8e01  ..}.t.j.j.f.|...
-000003d0: 0100 6400 5300 2905 4e29 01da 0375 726c  ..d.S.).N)...url
-000003e0: da08 7265 736f 7572 6365 da02 6964 2903  ..resource..id).
-000003f0: 721c 0000 00da 0777 6562 686f 6f6b da08  r......webhook..
-00000400: 6f72 6465 725f 6964 290a 7204 0000 00da  order_id).r.....
-00000410: 0544 4542 5547 720c 0000 00da 076f 626a  .DEBUGr......obj
-00000420: 6563 7473 da03 6765 74da 1262 7569 6c64  ects..get..build
-00000430: 5f61 6273 6f6c 7574 655f 7572 69da 1476  _absolute_uri..v
-00000440: 6572 6966 795f 7765 6268 6f6f 6b5f 6576  erify_webhook_ev
-00000450: 656e 74da 0a77 6562 686f 6f6b 5f69 6472  ent..webhook_idr
-00000460: 0d00 0000 da06 6372 6561 7465 2905 721a  ......create).r.
-00000470: 0000 0072 1b00 0000 721c 0000 00da 0e70  ...r....r......p
-00000480: 6179 7061 6c5f 7765 6268 6f6f 6b5a 0a65  aypal_webhookZ.e
-00000490: 7665 6e74 5f64 6174 6172 1800 0000 7218  vent_datar....r.
-000004a0: 0000 0072 1900 0000 da1d 7665 7269 6679  ...r......verify
-000004b0: 5f61 6e64 5f73 6176 655f 7765 6268 6f6f  _and_save_webhoo
-000004c0: 6b5f 6576 656e 7415 0000 0073 1000 0000  k_event....s....
-000004d0: 0001 0601 1201 0e02 0201 0201 18fd 0605  ................
-000004e0: 722a 0000 00da 0864 6973 7061 7463 6829  r*.....dispatch)
-000004f0: 01da 046e 616d 6563 0000 0000 0000 0000  ...namec........
-00000500: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-00000510: 7314 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
-00000520: 0284 005a 0364 0353 0029 04da 1150 6179  ...Z.d.S.)...Pay
-00000530: 7061 6c57 6562 686f 6f6b 5669 6577 6302  palWebhookViewc.
-00000540: 0000 0000 0000 0000 0000 0007 0000 0005  ................
-00000550: 0000 004f 0000 0073 b000 0000 7400 a001  ...O...s....t...
-00000560: 7c01 6a02 a003 6401 a101 a101 7d04 7c04  |.j...d.....}.|.
-00000570: a004 6402 a101 7d05 7c05 7405 6a06 6b07  ..d...}.|.t.j.k.
-00000580: 7230 7407 6403 6404 8d01 5300 7408 7409  r0t.d.d...S.t.t.
-00000590: 740a 6a0b 740a 6a0c 6405 8d02 6406 8d01  t.j.t.j.d...d...
-000005a0: 7d06 740d 7c01 7c06 7c04 6407 8d03 0100  }.t.|.|.|.d.....
-000005b0: 7c05 6408 6b02 7288 740e 6a0f 7c00 6a10  |.d.k.r.t.j.|.j.
-000005c0: 7c04 a004 6409 a101 640a 8d02 0100 7c06  |...d...d.....|.
-000005d0: a011 7c04 a004 6409 a101 a004 640b a101  ..|...d.....d...
-000005e0: a101 0100 7c05 640c 6b02 72a6 7412 6a0f  ....|.d.k.r.t.j.
-000005f0: 7c00 6a10 7c04 a004 6409 a101 640a 8d02  |.j.|...d...d...
-00000600: 0100 7407 640d 6404 8d01 5300 290e 4e7a  ..t.d.d...S.).Nz
-00000610: 0575 7466 2d38 da0a 6576 656e 745f 7479  .utf-8..event_ty
-00000620: 7065 6990 0100 0029 01da 0673 7461 7475  pei....)...statu
-00000630: 7329 02da 0963 6c69 656e 745f 6964 da0d  s)...client_id..
-00000640: 636c 6965 6e74 5f73 6563 7265 7429 01da  client_secret)..
-00000650: 0461 7574 6829 0172 1c00 0000 7213 0000  .auth).r....r...
-00000660: 0072 1e00 0000 2902 da06 7365 6e64 6572  .r....)...sender
-00000670: 721e 0000 0072 1f00 0000 7212 0000 00e9  r....r....r.....
-00000680: c800 0000 2913 da04 6a73 6f6e da05 6c6f  ....)...json..lo
-00000690: 6164 73da 0462 6f64 79da 0664 6563 6f64  ads..body..decod
-000006a0: 6572 2400 0000 7211 0000 0072 1700 0000  er$...r....r....
-000006b0: 7205 0000 0072 1000 0000 720b 0000 00da  r....r....r.....
-000006c0: 1664 6a61 6e67 6f5f 7061 7970 616c 5f73  .django_paypal_s
-000006d0: 6574 7469 6e67 73da 1450 4159 5041 4c5f  ettings..PAYPAL_
-000006e0: 4150 495f 434c 4945 4e54 5f49 44da 1150  API_CLIENT_ID..P
-000006f0: 4159 5041 4c5f 4150 495f 5345 4352 4554  AYPAL_API_SECRET
-00000700: 722a 0000 0072 0e00 0000 da04 7365 6e64  r*...r......send
-00000710: da09 5f5f 636c 6173 735f 5fda 0d63 6170  ..__class__..cap
-00000720: 7475 7265 5f6f 7264 6572 720f 0000 0029  ture_orderr....)
-00000730: 07da 0473 656c 6672 1a00 0000 da04 6172  ...selfr......ar
-00000740: 6773 da06 6b77 6172 6773 da09 706f 7374  gs..kwargs..post
-00000750: 5f64 6963 7472 2e00 0000 721b 0000 0072  _dictr....r....r
-00000760: 1800 0000 7218 0000 0072 1900 0000 da04  ....r....r......
-00000770: 706f 7374 2300 0000 7322 0000 0000 0112  post#...s"......
-00000780: 010a 010a 010a 0202 0102 0104 0004 ff04  ................
-00000790: ff06 060e 0208 0116 0116 0108 0116 027a  ...............z
-000007a0: 1650 6179 7061 6c57 6562 686f 6f6b 5669  .PaypalWebhookVi
-000007b0: 6577 2e70 6f73 744e 2904 7214 0000 0072  ew.postN).r....r
-000007c0: 1500 0000 7216 0000 0072 4300 0000 7218  ....r....rC...r.
-000007d0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-000007e0: 0000 722d 0000 0021 0000 0073 0200 0000  ..r-...!...s....
-000007f0: 0802 722d 0000 0029 1f72 3500 0000 da06  ..r-...).r5.....
-00000800: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00000810: da0b 646a 616e 676f 2e63 6f6e 6672 0400  ..django.confr..
-00000820: 0000 da0b 646a 616e 676f 2e68 7474 7072  ....django.httpr
-00000830: 0500 0000 7206 0000 00da 1764 6a61 6e67  ....r......djang
-00000840: 6f2e 7574 696c 732e 6465 636f 7261 746f  o.utils.decorato
-00000850: 7273 7207 0000 00da 1c64 6a61 6e67 6f2e  rsr......django.
-00000860: 7669 6577 732e 6465 636f 7261 746f 7273  views.decorators
-00000870: 2e63 7372 6672 0800 0000 da14 646a 616e  .csrfr......djan
-00000880: 676f 2e76 6965 7773 2e67 656e 6572 6963  go.views.generic
-00000890: 7209 0000 00da 0961 7069 5f74 7970 6573  r......api_types
-000008a0: 720b 0000 00da 066d 6f64 656c 7372 0c00  r......modelsr..
-000008b0: 0000 720d 0000 00da 0773 6967 6e61 6c73  ..r......signals
-000008c0: 720e 0000 0072 0f00 0000 da08 7772 6170  r....r......wrap
-000008d0: 7065 7273 7210 0000 00da 0d64 6a61 6e67  persr......djang
-000008e0: 6f5f 7061 7970 616c 7239 0000 0072 1100  o_paypalr9...r..
-000008f0: 0000 da03 7374 7272 2a00 0000 722d 0000  ....strr*...r-..
-00000900: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-00000910: 7219 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000920: 0000 0073 1e00 0000 0801 1002 0c01 1001  ...s............
-00000930: 0c01 0c01 0c02 0c01 1001 1001 0c01 0c03  ................
-00000940: 0e04 1a0c 0a01                           ......
+000000a0: 6d14 5a14 0100 6408 640b 6c15 6d16 5a16  m.Z...d.d.l.m.Z.
+000000b0: 6d17 5a17 0100 6408 640c 6c18 6d19 5a19  m.Z...d.d.l.m.Z.
+000000c0: 0100 6400 6403 6c1a 6d05 5a1b 0100 4700  ..d.d.l.m.Z...G.
+000000d0: 640d 640e 8400 640e 8302 5a1c 6508 6519  d.d...d...Z.e.e.
+000000e0: 6503 651d 6502 6602 1900 640f 9c03 6410  e.e.e.f...d...d.
+000000f0: 6411 8404 5a1e 650a 650c 6412 6413 8d02  d...Z.e.e.d.d...
+00000100: 4700 6414 6415 8400 6415 650e 8303 8301  G.d.d...d.e.....
+00000110: 5a1f 6401 5300 2916 e900 0000 004e 2902  Z.d.S.)......N).
+00000120: da03 416e 79da 0444 6963 7429 01da 0873  ..Any..Dict)...s
+00000130: 6574 7469 6e67 7329 02da 0c48 7474 7052  ettings)...HttpR
+00000140: 6573 706f 6e73 65da 0b48 7474 7052 6571  esponse..HttpReq
+00000150: 7565 7374 2901 da10 6d65 7468 6f64 5f64  uest)...method_d
+00000160: 6563 6f72 6174 6f72 2901 da0b 6373 7266  ecorator)...csrf
+00000170: 5f65 7865 6d70 7429 01da 0456 6965 77e9  _exempt)...View.
+00000180: 0100 0000 2901 da12 4150 4941 7574 6843  ....)...APIAuthC
+00000190: 7265 6465 6e74 6961 6c73 2903 da0d 5061  redentials)...Pa
+000001a0: 7970 616c 5765 6268 6f6f 6bda 1250 6179  ypalWebhook..Pay
+000001b0: 7061 6c57 6562 686f 6f6b 4576 656e 74da  palWebhookEvent.
+000001c0: 0b50 6179 7061 6c4f 7264 6572 2902 da0e  .PaypalOrder)...
+000001d0: 6f72 6465 725f 6170 7072 6f76 6564 da0f  order_approved..
+000001e0: 6f72 6465 725f 636f 6d70 6c65 7465 6429  order_completed)
+000001f0: 01da 0d50 6179 7061 6c57 7261 7070 6572  ...PaypalWrapper
+00000200: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000210: 0003 0000 0040 0000 0073 1600 0000 6500  .....@...s....e.
+00000220: 5a01 6400 5a02 6401 6402 6403 6703 5a03  Z.d.Z.d.d.d.g.Z.
+00000230: 6404 5300 2905 da0d 5765 6268 6f6f 6b45  d.S.)...WebhookE
+00000240: 7665 6e74 73fa 1843 4845 434b 4f55 542e  vents..CHECKOUT.
+00000250: 4f52 4445 522e 434f 4d50 4c45 5445 44fa  ORDER.COMPLETED.
+00000260: 1743 4845 434b 4f55 542e 4f52 4445 522e  .CHECKOUT.ORDER.
+00000270: 4150 5052 4f56 4544 7a22 4348 4543 4b4f  APPROVEDz"CHECKO
+00000280: 5554 2e50 4159 4d45 4e54 2d41 5050 524f  UT.PAYMENT-APPRO
+00000290: 5641 4c2e 5245 5645 5253 4544 4e29 04da  VAL.REVERSEDN)..
+000002a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000002b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000002c0: 655f 5fda 064f 5244 4552 53a9 0072 1900  e__..ORDERS..r..
+000002d0: 0000 7219 0000 00fa 5d2f 5573 6572 732f  ..r.....]/Users/
+000002e0: 7469 6d74 616d 2f2e 7079 656e 762f 7665  timtam/.pyenv/ve
+000002f0: 7273 696f 6e73 2f73 662d 332e 382e 3132  rsions/sf-3.8.12
+00000300: 2f6c 6962 2f70 7974 686f 6e33 2e38 2f73  /lib/python3.8/s
+00000310: 6974 652d 7061 636b 6167 6573 2f64 6a61  ite-packages/dja
+00000320: 6e67 6f5f 7061 7970 616c 2f77 6562 686f  ngo_paypal/webho
+00000330: 6f6b 732e 7079 7212 0000 0011 0000 0073  oks.pyr........s
+00000340: 0200 0000 0801 7212 0000 0029 03da 0772  ......r....)...r
+00000350: 6571 7565 7374 da0e 7061 7970 616c 5f77  equest..paypal_w
+00000360: 7261 7070 6572 da07 7061 796c 6f61 6463  rapper..payloadc
+00000370: 0300 0000 0000 0000 0000 0000 0800 0000  ................
+00000380: 0900 0000 4300 0000 73b6 0000 0074 0064  ....C...s....t.d
+00000390: 017c 0283 0201 0074 0064 027c 0264 0319  .|.....t.d.|.d..
+000003a0: 0064 0419 0083 0201 0064 0564 066c 016d  .d.......d.d.l.m
+000003b0: 017d 0301 007c 037c 006a 0283 0101 0074  .}...|.|.j.....t
+000003c0: 036a 0473 b27c 0264 0319 0064 0419 007d  .j.s.|.d...d...}
+000003d0: 0474 056a 066a 077c 0464 078d 017d 057c  .t.j.j.|.d...}.|
+000003e0: 01a0 087c 007c 056a 09a1 0201 007a 1a74  ...|.|.j.....z.t
+000003f0: 0a6a 066a 077c 0264 0319 0064 0419 0064  .j.j.|.d...d...d
+00000400: 088d 017d 0657 006e 1c04 0074 0b74 0c66  ...}.W.n...t.t.f
+00000410: 026b 0a72 9601 0001 0001 0064 007d 0659  .k.r.......d.}.Y
+00000420: 006e 0258 007c 027c 057c 0664 099c 037d  .n.X.|.|.|.d...}
+00000430: 0774 0d6a 066a 0e66 007c 078e 0101 0064  .t.j.j.f.|.....d
+00000440: 0053 0029 0a4e 721d 0000 00da 0a77 6562  .S.).Nr......web
+00000450: 686f 6f6b 5f69 64da 0872 6573 6f75 7263  hook_id..resourc
+00000460: 65da 0269 6472 0100 0000 2901 da06 7070  e..idr....)...pp
+00000470: 7269 6e74 2901 721e 0000 0029 01da 086f  rint).r....)...o
+00000480: 7264 6572 5f69 6429 0372 1d00 0000 da07  rder_id).r......
+00000490: 7765 6268 6f6f 6bda 056f 7264 6572 290f  webhook..order).
+000004a0: da05 7072 696e 7472 2100 0000 da04 4d45  ..printr!.....ME
+000004b0: 5441 7204 0000 00da 0544 4542 5547 720c  TAr......DEBUGr.
+000004c0: 0000 00da 076f 626a 6563 7473 da03 6765  .....objects..ge
+000004d0: 74da 1476 6572 6966 795f 7765 6268 6f6f  t..verify_webhoo
+000004e0: 6b5f 6576 656e 7472 1e00 0000 720e 0000  k_eventr....r...
+000004f0: 00da 084b 6579 4572 726f 72da 0954 7970  ...KeyError..Typ
+00000500: 6545 7272 6f72 720d 0000 00da 0663 7265  eErrorr......cre
+00000510: 6174 6529 0872 1b00 0000 721c 0000 0072  ate).r....r....r
+00000520: 1d00 0000 7221 0000 0072 1e00 0000 da0e  ....r!...r......
+00000530: 7061 7970 616c 5f77 6562 686f 6f6b da0c  paypal_webhook..
+00000540: 7061 7970 616c 5f6f 7264 6572 5a0a 6576  paypal_orderZ.ev
+00000550: 656e 745f 6461 7461 7219 0000 0072 1900  ent_datar....r..
+00000560: 0000 721a 0000 00da 1d76 6572 6966 795f  ..r......verify_
+00000570: 616e 645f 7361 7665 5f77 6562 686f 6f6b  and_save_webhook
+00000580: 5f65 7665 6e74 1500 0000 7322 0000 0000  _event....s"....
+00000590: 010a 0112 010c 010a 0106 010c 010e 010e  ................
+000005a0: 0102 011a 0112 010a 0202 0102 0102 fd06  ................
+000005b0: 0572 3000 0000 da08 6469 7370 6174 6368  .r0.....dispatch
+000005c0: 2901 da04 6e61 6d65 6300 0000 0000 0000  )...namec.......
+000005d0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
+000005e0: 0073 1400 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+000005f0: 6402 8400 5a03 6403 5300 2904 da11 5061  d...Z.d.S.)...Pa
+00000600: 7970 616c 5765 6268 6f6f 6b56 6965 7763  ypalWebhookViewc
+00000610: 0200 0000 0000 0000 0000 0000 0700 0000  ................
+00000620: 0500 0000 4f00 0000 73b0 0000 0074 00a0  ....O...s....t..
+00000630: 017c 016a 02a0 0364 01a1 01a1 017d 047c  .|.j...d.....}.|
+00000640: 04a0 0464 02a1 017d 057c 0574 056a 066b  ...d...}.|.t.j.k
+00000650: 0772 3074 0764 0364 048d 0153 0074 0874  .r0t.d.d...S.t.t
+00000660: 0974 0a6a 0b74 0a6a 0c64 058d 0264 068d  .t.j.t.j.d...d..
+00000670: 017d 0674 0d7c 017c 067c 0464 078d 0301  .}.t.|.|.|.d....
+00000680: 007c 0564 086b 0272 8874 0e6a 0f7c 006a  .|.d.k.r.t.j.|.j
+00000690: 107c 04a0 0464 09a1 0164 0a8d 0201 007c  .|...d...d.....|
+000006a0: 06a0 117c 04a0 0464 09a1 01a0 0464 0ba1  ...|...d.....d..
+000006b0: 01a1 0101 007c 0564 0c6b 0272 a674 126a  .....|.d.k.r.t.j
+000006c0: 0f7c 006a 107c 04a0 0464 09a1 0164 0a8d  .|.j.|...d...d..
+000006d0: 0201 0074 0764 0d64 048d 0153 0029 0e4e  ...t.d.d...S.).N
+000006e0: 7a05 7574 662d 38da 0a65 7665 6e74 5f74  z.utf-8..event_t
+000006f0: 7970 6569 9001 0000 2901 da06 7374 6174  ypei....)...stat
+00000700: 7573 2902 da09 636c 6965 6e74 5f69 64da  us)...client_id.
+00000710: 0d63 6c69 656e 745f 7365 6372 6574 2901  .client_secret).
+00000720: da04 6175 7468 2901 721d 0000 0072 1400  ..auth).r....r..
+00000730: 0000 721f 0000 0029 02da 0673 656e 6465  ..r....)...sende
+00000740: 7272 1f00 0000 7220 0000 0072 1300 0000  rr....r ...r....
+00000750: e9c8 0000 0029 13da 046a 736f 6eda 056c  .....)...json..l
+00000760: 6f61 6473 da04 626f 6479 da06 6465 636f  oads..body..deco
+00000770: 6465 7229 0000 0072 1200 0000 7218 0000  der)...r....r...
+00000780: 0072 0500 0000 7211 0000 0072 0b00 0000  .r....r....r....
+00000790: da16 646a 616e 676f 5f70 6179 7061 6c5f  ..django_paypal_
+000007a0: 7365 7474 696e 6773 da14 5041 5950 414c  settings..PAYPAL
+000007b0: 5f41 5049 5f43 4c49 454e 545f 4944 da11  _API_CLIENT_ID..
+000007c0: 5041 5950 414c 5f41 5049 5f53 4543 5245  PAYPAL_API_SECRE
+000007d0: 5472 3000 0000 720f 0000 00da 0473 656e  Tr0...r......sen
+000007e0: 64da 095f 5f63 6c61 7373 5f5f da0d 6361  d..__class__..ca
+000007f0: 7074 7572 655f 6f72 6465 7272 1000 0000  pture_orderr....
+00000800: 2907 da04 7365 6c66 721b 0000 00da 0461  )...selfr......a
+00000810: 7267 73da 066b 7761 7267 73da 0970 6f73  rgs..kwargs..pos
+00000820: 745f 6469 6374 7234 0000 0072 1c00 0000  t_dictr4...r....
+00000830: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00000840: 0470 6f73 742c 0000 0073 2200 0000 0001  .post,...s".....
+00000850: 1201 0a01 0a01 0a02 0201 0201 0400 04ff  ................
+00000860: 04ff 0606 0e02 0801 1601 1601 0801 1602  ................
+00000870: 7a16 5061 7970 616c 5765 6268 6f6f 6b56  z.PaypalWebhookV
+00000880: 6965 772e 706f 7374 4e29 0472 1500 0000  iew.postN).r....
+00000890: 7216 0000 0072 1700 0000 7249 0000 0072  r....r....rI...r
+000008a0: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
+000008b0: 0000 0072 3300 0000 2a00 0000 7302 0000  ...r3...*...s...
+000008c0: 0008 0272 3300 0000 2920 723b 0000 00da  ...r3...) r;....
+000008d0: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
+000008e0: 00da 0b64 6a61 6e67 6f2e 636f 6e66 7204  ...django.confr.
+000008f0: 0000 00da 0b64 6a61 6e67 6f2e 6874 7470  .....django.http
+00000900: 7205 0000 0072 0600 0000 da17 646a 616e  r....r......djan
+00000910: 676f 2e75 7469 6c73 2e64 6563 6f72 6174  go.utils.decorat
+00000920: 6f72 7372 0700 0000 da1c 646a 616e 676f  orsr......django
+00000930: 2e76 6965 7773 2e64 6563 6f72 6174 6f72  .views.decorator
+00000940: 732e 6373 7266 7208 0000 00da 1464 6a61  s.csrfr......dja
+00000950: 6e67 6f2e 7669 6577 732e 6765 6e65 7269  ngo.views.generi
+00000960: 6372 0900 0000 da09 6170 695f 7479 7065  cr......api_type
+00000970: 7372 0b00 0000 da06 6d6f 6465 6c73 720c  sr......modelsr.
+00000980: 0000 0072 0d00 0000 720e 0000 00da 0773  ...r....r......s
+00000990: 6967 6e61 6c73 720f 0000 0072 1000 0000  ignalsr....r....
+000009a0: da08 7772 6170 7065 7273 7211 0000 00da  ..wrappersr.....
+000009b0: 0d64 6a61 6e67 6f5f 7061 7970 616c 723f  .django_paypalr?
+000009c0: 0000 0072 1200 0000 da03 7374 7272 3000  ...r......strr0.
+000009d0: 0000 7233 0000 0072 1900 0000 7219 0000  ..r3...r....r...
+000009e0: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
+000009f0: 6475 6c65 3e01 0000 0073 1e00 0000 0801  dule>....s......
+00000a00: 1002 0c01 1001 0c01 0c01 0c02 0c01 1401  ................
+00000a10: 1001 0c01 0c03 0e04 1a15 0a01            ............
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/__pycache__/wrappers.cpython-311.pyc` & `django-paypal-plus-1.1.0/django_paypal/__pycache__/wrappers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/__pycache__/wrappers.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/__pycache__/wrappers.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Feb  7 08:27:06 2024 UTC, .py size: 10412 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 da3e c365 ac28 0000  U........>.e.(..
+00000000: 550d 0d0a 0000 0000 cd31 2b66 ac28 0000  U........1+f.(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 f400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6404 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6402 6c0b 5a0b 6400 6405 6c0c 6d0d 5a0d  d.l.Z.d.d.l.m.Z.
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/api_types.py` & `django-paypal-plus-1.1.0/django_paypal/api_types.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/migrations/0001_initial.py` & `django-paypal-plus-1.1.0/django_paypal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/migrations/0002_auto_20171002_1551.py` & `django-paypal-plus-1.1.0/django_paypal/migrations/0002_auto_20171002_1551.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/migrations/0003_auto_20200124_1528.py` & `django-paypal-plus-1.1.0/django_paypal/migrations/0003_auto_20200124_1528.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/migrations/0004_paypalpayment_related_resource_state.py` & `django-paypal-plus-1.1.0/django_paypal/migrations/0004_paypalpayment_related_resource_state.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/migrations/0005_auto_20240207_0630.py` & `django-paypal-plus-1.1.0/django_paypal/migrations/0005_auto_20240207_0630.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/0001_initial.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0001_initial.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/0002_auto_20171002_1551.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0002_auto_20171002_1551.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/0003_auto_20200124_1528.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0003_auto_20200124_1528.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/0004_paypalpayment_related_resource_state.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0004_paypalpayment_related_resource_state.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/migrations/__pycache__/0005_auto_20240207_0630.cpython-38.pyc` & `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0005_auto_20240207_0630.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Feb  7 05:30:57 2024 UTC, .py size: 4611 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9115 c365 0312 0000  U..........e....
+00000000: 550d 0d0a 0000 0000 b33b 2766 0312 0000  U........;'f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6400 6401 6c05 5a01 4700  m.Z...d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6503 6a06 8303 5a06  d.d...d.e.j...Z.
 00000060: 6401 5300 2905 e900 0000 004e 2902 da0a  d.S.)......N)...
 00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
@@ -45,33 +45,33 @@
 000002c0: 6a06 6a14 6a15 643b 6433 6434 8d03 6602  j.j.j.d;d3d4..f.
 000002d0: 643c 6506 6a12 6404 6509 6a13 6a06 6a14  d<e.j.d.e.j.j.j.
 000002e0: 6a15 643d 643e 643f 8d04 6602 6706 6411  j.d=d>d?..f.g.d.
 000002f0: 8d02 6504 6a16 6440 6431 6506 6a12 6509  ..e.j.d@d1e.j.e.
 00000300: 6a13 6a06 6a14 6a15 6441 6433 6434 8d03  j.j.j.j.dAd3d4..
 00000310: 6442 8d03 670c 5a17 6443 5300 2944 da09  dB..g.Z.dCS.)D..
 00000320: 4d69 6772 6174 696f 6e29 02da 0d64 6a61  Migration)...dja
-00000330: 6e67 6f5f 7061 7970 616c 5a29 3030 3034  ngo_paypalZ)0004
+00000330: 6e67 6f5f 7061 7970 616c da29 3030 3034  ngo_paypal.)0004
 00000340: 5f70 6179 7061 6c70 6179 6d65 6e74 5f72  _paypalpayment_r
 00000350: 656c 6174 6564 5f72 6573 6f75 7263 655f  elated_resource_
 00000360: 7374 6174 65da 1150 6179 7061 6c41 5049  state..PaypalAPI
 00000370: 506f 7374 4461 7461 da02 6964 5446 da02  PostData..idTF..
 00000380: 4944 2904 da0c 6175 746f 5f63 7265 6174  ID)...auto_creat
 00000390: 6564 da0b 7072 696d 6172 795f 6b65 79da  ed..primary_key.
 000003a0: 0973 6572 6961 6c69 7a65 da0c 7665 7262  .serialize..verb
 000003b0: 6f73 655f 6e61 6d65 da03 7572 6ce9 ff00  ose_name..url...
 000003c0: 0000 da03 5552 4c29 03da 0562 6c61 6e6b  ....URL)...blank
-000003d0: da0a 6d61 785f 6c65 6e67 7468 720c 0000  ..max_lengthr...
+000003d0: da0a 6d61 785f 6c65 6e67 7468 720d 0000  ..max_lengthr...
 000003e0: 00da 0970 6f73 745f 6461 7461 7a09 506f  ...post_dataz.Po
-000003f0: 7374 2044 6174 6129 0172 0c00 0000 da0a  st Data).r......
+000003f0: 7374 2044 6174 6129 0172 0d00 0000 da0a  st Data).r......
 00000400: 6372 6561 7465 645f 6174 2901 da0c 6175  created_at)...au
 00000410: 746f 5f6e 6f77 5f61 6464 2902 da04 6e61  to_now_add)...na
 00000420: 6d65 da06 6669 656c 6473 da0b 5061 7970  me..fields..Payp
 00000430: 616c 4f72 6465 72da 086f 7264 6572 5f69  alOrder..order_i
-00000440: 647a 084f 7264 6572 2049 4429 0372 1100  dz.Order ID).r..
-00000450: 0000 da06 756e 6971 7565 720c 0000 00da  ....uniquer.....
+00000440: 647a 084f 7264 6572 2049 4429 0372 1200  dz.Order ID).r..
+00000450: 0000 da06 756e 6971 7565 720d 0000 00da  ....uniquer.....
 00000460: 0673 7461 7475 73da 0653 7461 7475 73da  .status..Status.
 00000470: 0d50 6179 7061 6c57 6562 686f 6f6b da0a  .PaypalWebhook..
 00000480: 7765 6268 6f6f 6b5f 6964 7a0a 5765 6268  webhook_idz.Webh
 00000490: 6f6f 6b20 4944 da0b 6576 656e 745f 7479  ook ID..event_ty
 000004a0: 7065 737a 1541 6374 6976 6520 5765 6268  pesz.Active Webh
 000004b0: 6f6f 6b20 4576 656e 7473 5a0a 5061 7970  ook EventsZ.Payp
 000004c0: 616c 4974 656d da10 4c65 6761 6379 5061  alItem..LegacyPa
@@ -81,17 +81,17 @@
 00000500: 6567 6163 7950 6179 7061 6c50 6179 6d65  egacyPaypalPayme
 00000510: 6e74 5a11 5061 7970 616c 5472 616e 7361  ntZ.PaypalTransa
 00000520: 6374 696f 6eda 174c 6567 6163 7950 6179  ction..LegacyPay
 00000530: 7061 6c54 7261 6e73 6163 7469 6f6e 5a10  palTransactionZ.
 00000540: 6c65 6761 6379 7061 7970 616c 6974 656d  legacypaypalitem
 00000550: 7a24 4c65 6761 6379 2050 6179 7061 6c20  z$Legacy Paypal 
 00000560: 4974 656d 2028 7061 796d 656e 7473 2076  Item (payments v
-00000570: 3120 4150 4929 2902 720c 0000 00da 1376  1 API)).r......v
+00000570: 3120 4150 4929 2902 720d 0000 00da 1376  1 API)).r......v
 00000580: 6572 626f 7365 5f6e 616d 655f 706c 7572  erbose_name_plur
-00000590: 616c 2902 7215 0000 00da 076f 7074 696f  al).r......optio
+00000590: 616c 2902 7216 0000 00da 076f 7074 696f  al).r......optio
 000005a0: 6e73 5a13 6c65 6761 6379 7061 7970 616c  nsZ.legacypaypal
 000005b0: 7061 796d 656e 747a 274c 6567 6163 7920  paymentz'Legacy 
 000005c0: 5061 7970 616c 2050 6179 6d65 6e74 2028  Paypal Payment (
 000005d0: 7061 796d 656e 7473 2076 3120 4150 4929  payments v1 API)
 000005e0: 7a28 4c65 6761 6379 2050 6179 7061 6c20  z(Legacy Paypal 
 000005f0: 5061 796d 656e 7473 2028 7061 796d 656e  Payments (paymen
 00000600: 7473 2076 3120 4150 4929 5a17 6c65 6761  ts v1 API)Z.lega
@@ -115,36 +115,36 @@
 00000720: 6f6f 6bda 1150 6179 7061 6c41 5049 5265  ook..PaypalAPIRe
 00000730: 7370 6f6e 7365 da0d 7265 7370 6f6e 7365  sponse..response
 00000740: 5f64 6174 617a 0d52 6573 706f 6e73 6520  _dataz.Response 
 00000750: 4461 7461 da0d 6170 695f 7265 7370 6f6e  Data..api_respon
 00000760: 7365 73da 0470 6f73 74da 0972 6573 706f  ses..post..respo
 00000770: 6e73 6573 7a1f 646a 616e 676f 5f70 6179  nsesz.django_pay
 00000780: 7061 6c2e 5061 7970 616c 4150 4950 6f73  pal.PaypalAPIPos
-00000790: 7444 6174 6129 04da 046e 756c 6c72 2c00  tData)...nullr,.
-000007a0: 0000 722d 0000 0072 2e00 0000 5a11 7061  ..r-...r....Z.pa
+00000790: 7444 6174 6129 04da 046e 756c 6c72 2d00  tData)...nullr-.
+000007a0: 0000 722e 0000 0072 2f00 0000 5a11 7061  ..r....r/...Z.pa
 000007b0: 7970 616c 6170 6970 6f73 7464 6174 61da  ypalapipostdata.
 000007c0: 0961 7069 5f70 6f73 7473 2903 da0a 6d6f  .api_posts)...mo
-000007d0: 6465 6c5f 6e61 6d65 7215 0000 00da 0566  del_namer......f
+000007d0: 6465 6c5f 6e61 6d65 7216 0000 00da 0566  del_namer......f
 000007e0: 6965 6c64 4e29 18da 085f 5f6e 616d 655f  ieldN)...__name_
 000007f0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000800: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
 00000810: 656e 6465 6e63 6965 7372 0200 0000 da0b  endenciesr......
 00000820: 4372 6561 7465 4d6f 6465 6c72 0300 0000  CreateModelr....
 00000830: da09 4175 746f 4669 656c 64da 0943 6861  ..AutoField..Cha
 00000840: 7246 6965 6c64 da06 646a 616e 676f da07  rField..django..
 00000850: 636f 6e74 7269 62da 0870 6f73 7467 7265  contrib..postgre
-00000860: 7372 1600 0000 da05 6a73 6f6e 62da 094a  sr......jsonb..J
+00000860: 7372 1700 0000 da05 6a73 6f6e 62da 094a  sr......jsonb..J
 00000870: 534f 4e46 6965 6c64 da0d 4461 7465 5469  SONField..DateTi
 00000880: 6d65 4669 656c 64da 0b52 656e 616d 654d  meField..RenameM
 00000890: 6f64 656c da11 416c 7465 724d 6f64 656c  odel..AlterModel
 000008a0: 4f70 7469 6f6e 73da 0a46 6f72 6569 676e  Options..Foreign
 000008b0: 4b65 79da 0264 62da 0864 656c 6574 696f  Key..db..deletio
 000008c0: 6eda 0743 4153 4341 4445 da08 4164 6446  n..CASCADE..AddF
 000008d0: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-000008e0: a900 724f 0000 0072 4f00 0000 fa77 2f55  ..rO...rO....w/U
+000008e0: a900 7250 0000 0072 5000 0000 fa77 2f55  ..rP...rP....w/U
 000008f0: 7365 7273 2f74 696d 7461 6d2f 2e70 7965  sers/timtam/.pye
 00000900: 6e76 2f76 6572 7369 6f6e 732f 7366 2d33  nv/versions/sf-3
 00000910: 2e38 2e31 322f 6c69 622f 7079 7468 6f6e  .8.12/lib/python
 00000920: 332e 382f 7369 7465 2d70 6163 6b61 6765  3.8/site-package
 00000930: 732f 646a 616e 676f 5f70 6179 7061 6c2f  s/django_paypal/
 00000940: 6d69 6772 6174 696f 6e73 2f30 3030 355f  migrations/0005_
 00000950: 6175 746f 5f32 3032 3430 3230 375f 3036  auto_20240207_06
@@ -157,14 +157,14 @@
 000009c0: 0102 0108 fe04 0404 0102 0108 fe04 0404  ................
 000009d0: 0102 0108 fe04 0404 0102 0214 0116 011a  ................
 000009e0: 011a fc02 fe04 0904 0102 0214 0112 0116  ................
 000009f0: 010e 011a 011c fa02 fe04 0b04 0102 0102  ................
 00000a00: 0116 fd04 b972 0400 0000 2907 5a24 646a  .....r....).Z$dj
 00000a10: 616e 676f 2e63 6f6e 7472 6962 2e70 6f73  ango.contrib.pos
 00000a20: 7467 7265 732e 6669 656c 6473 2e6a 736f  tgres.fields.jso
-00000a30: 6e62 7241 0000 00da 0964 6a61 6e67 6f2e  nbrA.....django.
+00000a30: 6e62 7242 0000 00da 0964 6a61 6e67 6f2e  nbrB.....django.
 00000a40: 6462 7202 0000 0072 0300 0000 da19 646a  dbr....r......dj
 00000a50: 616e 676f 2e64 622e 6d6f 6465 6c73 2e64  ango.db.models.d
-00000a60: 656c 6574 696f 6e72 0400 0000 724f 0000  eletionr....rO..
-00000a70: 0072 4f00 0000 724f 0000 0072 5000 0000  .rO...rO...rP...
+00000a60: 656c 6574 696f 6e72 0400 0000 7250 0000  eletionr....rP..
+00000a70: 0072 5000 0000 7250 0000 0072 5100 0000  .rP...rP...rQ...
 00000a80: da08 3c6d 6f64 756c 653e 0300 0000 7306  ..<module>....s.
 00000a90: 0000 0008 0110 0108 03                   .........
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/models.py` & `django-paypal-plus-1.1.0/django_paypal/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from decimal import Decimal
 from typing import List
 
 from dataclass_wizard import fromdict
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
-from django_paypal.api_types import SellerReceivableBreakdown, Capture
+from django_paypal.api_types import Capture
 
 try:
     # Django 3.1 and newer
     from django.db.models import JSONField
 except ImportError:
     # Django 2.2
     from django.contrib.postgres.fields import JSONField
@@ -48,17 +48,24 @@
     url = models.CharField(_('URL'), max_length=255, blank=True)
     response_data = JSONField(_('Response Data'))
     created_at = models.DateTimeField(auto_now_add=True)
 
 
 class PaypalWebhook(models.Model):
     webhook_id = models.CharField(_('Webhook ID'), max_length=255, unique=True)
-    url = models.CharField('URL', max_length=255, unique=True)
+    auth_hash = models.CharField(_('Auth Hash'), max_length=255, default='')
+    url = models.CharField('URL', max_length=255)
     event_types = JSONField(_('Active Webhook Events'))
 
+    class Meta:
+        unique_together = (
+            'url',
+            'auth_hash',
+        )
+
 
 class PaypalWebhookEvent(models.Model):
     payload = JSONField(_('Payload'))
     order = models.ForeignKey(PaypalOrder, related_name='webhook_events', on_delete=models.CASCADE)
     webhook = models.ForeignKey(PaypalWebhook, related_name='events', on_delete=models.CASCADE)
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/ruff.toml` & `django-paypal-plus-1.1.0/django_paypal/ruff.toml`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.0.1/django_paypal/settings.py` & `django-paypal-plus-1.1.0/django_paypal/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 PAYPAL_API_URL = getattr(settings, 'PAYPAL_API_URL', 'https://api-m.paypal.com')
 PAYPAL_SANDBOX_API_URL = getattr(settings, 'PAYPAL_SANDBOX_API_URL', 'https://api-m.sandbox.paypal.com')
 PAYPAL_SANDBOX = getattr(settings, 'PAYPAL_SANDBOX', True)
 
 PAYPAL_AUTH_URL = getattr(settings, 'PAYPAL_AUTH_URL', '/v1/oauth2/token')
 PAYPAL_AUTH_CACHE_TIMEOUT = getattr(settings, 'PAYPAL_AUTH_CACHE_TIMEOUT', 600)  # 10 minutes
-PAYPAL_AUTH_CACHE_KEY = getattr(settings, 'PAYPAL_AUTH_CACHE_KEY', 'django-paypal-auth')
+PAYPAL_AUTH_CACHE_KEY = getattr(settings, 'PAYPAL_AUTH_CACHE_KEY', 'django-paypal-auth-{auth_hash}')
 PAYPAL_ORDERS_API_ENDPOINT = getattr(settings, 'PAYPAL_ORDERS_API_ENDPOINT', '/v2/checkout/orders')
 PAYPAL_WEBHOOK_LISTENER = getattr(settings, 'PAYPAL_WEBHOOK_LISTENER', None)
 
 # checkout urls
 PAYPAL_SUCCESS_URL = getattr(settings, 'PAYPAL_SUCCESS_URL', '/')
 PAYPAL_CANCELLATION_URL = getattr(settings, 'PAYDIREKT_CANCELLATION_URL', '/')
 PAYPAL_NOTIFICATION_URL = getattr(settings, 'PAYDIREKT_NOTIFICATION_URL', '/paypal/notify/')
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/webhooks.py` & `django-paypal-plus-1.1.0/django_paypal/webhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,17 @@
 
 def verify_and_save_webhook_event(request: HttpRequest, paypal_wrapper: PaypalWrapper, payload: Dict[str, Any]):
     if not settings.DEBUG:
         paypal_webhook = PaypalWebhook.objects.get(url=request.build_absolute_uri())
         paypal_wrapper.verify_webhook_event(request, paypal_webhook.webhook_id)
         try:
             paypal_order = PaypalOrder.objects.get(order_id=payload['resource']['id'])
-        except (KeyError, TypeError):   # if the payload does not contain the order id
+        except (KeyError, TypeError):  # if the payload does not contain the order id
             paypal_order = None
-        event_data = {
-            'payload': payload,
-            'webhook': paypal_webhook,
-            'order': paypal_order
-        }
+        event_data = {'payload': payload, 'webhook': paypal_webhook, 'order': paypal_order}
         PaypalWebhookEvent.objects.create(**event_data)
 
 
 @method_decorator(csrf_exempt, name='dispatch')
 class PaypalWebhookView(View):
     def post(self, request, *args, **kwargs):
         post_dict = json.loads(request.body.decode('utf-8'))
```

### Comparing `django-paypal-plus-1.0.1/django_paypal/wrappers.py` & `django-paypal-plus-1.1.0/django_paypal/wrappers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import unicode_literals
 
+import hashlib
 import json
 import warnings
 from typing import Literal, List, Any, Dict
 
 from django.core.cache import cache
 import requests
 from django.http import HttpRequest
@@ -100,66 +101,85 @@
 
     def get_order_details(self, order_id: str) -> OrderDetailAPIResponse:
         order = PaypalOrder.objects.get(order_id=order_id)
         url = f'{self.api_url}{self.orders_api_endpoint}/{order.order_id}'
         order_details_response = self.call_api(url=url, method='GET')
         return OrderDetailAPIResponse.from_dict(order_details_response)
 
-    def call_api(self, url: str, method: Literal['GET', 'POST', 'PATCH'], data=None) -> Dict[str, Any]:
+    def call_api(self, url: str, method: Literal['GET', 'POST', 'PATCH', 'DELETE'], data=None) -> Dict[str, Any]:
         headers = {'Authorization': f'Bearer {self._get_access_token()}', 'Content-Type': 'application/json'}
 
         try:
             if method == 'GET':
                 response = requests.get(url, headers=headers)
             elif method == 'POST':
                 response = requests.post(url, headers=headers, json=data)
             elif method == 'PATCH':
                 response = requests.patch(url, headers=headers, json=data)
+            elif method == 'DELETE':
+                response = requests.delete(url, headers=headers)
+                response.raise_for_status()
+                return {'deleted': True}
             else:
                 raise ValueError('Invalid method')
             response.raise_for_status()
             response_json = response.json()
             return response_json
         except requests.HTTPError as e:
             raise PaypalAPIError(str(e), response=e.response)
 
     def setup_webhooks(self, webhook_listener: str) -> PaypalWebhook:
-        if PaypalWebhook.objects.filter(url=webhook_listener).exists():
+        if PaypalWebhook.objects.filter(url=webhook_listener, auth_hash=self.api_auth_hash).exists():
             raise ValueError(f'Webhook listener ({webhook_listener}) already exists')
         from django_paypal.webhooks import WebhookEvents
 
         data = {'url': webhook_listener, 'event_types': [{'name': event} for event in WebhookEvents.ORDERS]}
         webhook_api = '{0}{1}'.format(self.api_url, '/v1/notifications/webhooks')
         try:
             response_dict = self.call_api(url=webhook_api, method='POST', data=data)
             return PaypalWebhook.objects.create(
-                webhook_id=response_dict['id'], url=response_dict['url'], event_types=response_dict['event_types']
+                webhook_id=response_dict['id'],
+                auth_hash=self.api_auth_hash,
+                url=response_dict['url'],
+                event_types=response_dict['event_types'],
             )
         except PaypalAPIError as e:
             response_json = e.response.json()
             if response_json.get('name') == 'WEBHOOK_URL_ALREADY_EXISTS':
                 webhook_list = self.call_api(url=webhook_api, method='GET')
                 for webhook in webhook_list.get('webhooks', []):
                     if webhook['url'] == webhook_listener:
-                        return PaypalWebhook.objects.create(webhook_id=webhook['id'], url=webhook['url'], event_types=webhook['event_types'])
+                        return PaypalWebhook.objects.create(
+                            webhook_id=webhook['id'], url=webhook['url'], event_types=webhook['event_types'], auth_hash=self.api_auth_hash
+                        )
             raise e
 
     def patch_webhook(self, webhook_id: str, patch_data: List[Dict]) -> PaypalWebhook:
         try:
             paypal_webhook = PaypalWebhook.objects.get(webhook_id=webhook_id)
         except PaypalWebhook.DoesNotExist as e:
             warnings.warn(f'Webhook with id {webhook_id} does not exist in the database. Set up webhooks by calling "setup_webhooks"')
             raise e
-        url = '{0}{1}'.format(self.api_url, f'/v1/notifications/webhooks/{webhook_id}')
+        url = '{0}{1}'.format(self.api_url, f'/v1/notifications/webhooks/{paypal_webhook.webhook_id}')
         webhook_response_dict = self.call_api(url=url, method='PATCH', data=patch_data)
         paypal_webhook.url = webhook_response_dict['url']
         paypal_webhook.event_types = webhook_response_dict['event_types']
         paypal_webhook.save()
         return paypal_webhook
 
+    def delete_webhook(self, webhook_listener: str) -> bool:
+        try:
+            paypal_webhook = PaypalWebhook.objects.get(url=webhook_listener, auth_hash=self.api_auth_hash)
+        except PaypalWebhook.DoesNotExist as e:
+            raise e
+        url = '{0}{1}'.format(self.api_url, f'/v1/notifications/webhooks/{paypal_webhook.webhook_id}')
+        self.call_api(url=url, method='DELETE')
+        paypal_webhook.delete()
+        return True
+
     def verify_webhook_event(self, request: HttpRequest, webhook_id: str) -> bool:
         headers = request.headers
         auth_algo = headers.get('Paypal-Auth-Algo')
         cert_url = headers.get('Paypal-Cert-Url')
         transmission_id = headers.get('Paypal-Transmission-Id')
         transmission_time = headers.get('Paypal-Transmission-Time')
         transmission_sig = headers.get('Paypal-Transmission-Sig')
@@ -175,24 +195,29 @@
         }
         url = f'{self.api_url}/v1/notifications/verify-webhook-signature'
         res = self.call_api(url=url, method='POST', data=verification_payload)
         if res.get('verification_status') == 'SUCCESS':
             return True
         raise PaypalWebhookVerificationError('Webhook verification failed', res)
 
+    def verify_api_keys(self) -> bool:
+        self._get_access_token()
+        return True
+
     def _get_access_token(self) -> str:
         if not self.auth_cache_timeout:
             auth_response = self._authorize_client()
             return auth_response.access_token
         else:
-            access_token = cache.get(self.auth_cache_key)
+            cache_key = self.auth_cache_key.format(auth_hash=self.api_auth_hash)
+            access_token = cache.get(cache_key)
             if not access_token:
                 auth_response = self._authorize_client()
                 access_token = auth_response.access_token
-                cache.set(self.auth_cache_key, access_token, self.auth_cache_timeout)
+                cache.set(cache_key, access_token, self.auth_cache_timeout)
             return access_token
 
     def _authorize_client(self) -> OAuthResponse:
         # preparing request
         url = f'{self.api_url}{self.auth_url}'
 
         api_auth = HTTPBasicAuth(self.auth.client_id, self.auth.client_secret)
@@ -201,11 +226,12 @@
 
         try:
             response = requests.post(url, headers=headers, data=data, auth=api_auth)
             response.raise_for_status()  # Raise an exception for HTTP errors
             response_json = response.json()
             return OAuthResponse(**response_json)
         except requests.HTTPError as e:
-            print(e.response.json(), url)
-            print("Client id", self.auth.client_id)
-            print("Client secret", self.auth.client_secret)
             raise PaypalAuthFailure(str(e), response=e.response)
+
+    @property
+    def api_auth_hash(self) -> str:
+        return hashlib.md5(f'{self.auth.client_id}{self.auth.client_secret}'.encode()).hexdigest()
```

### Comparing `django-paypal-plus-1.0.1/django_paypal_plus.egg-info/PKG-INFO` & `django-paypal-plus-1.1.0/django_paypal_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-paypal-plus
-Version: 1.0.1
+Version: 1.1.0
 Summary: Django integration of PayPal's Orders v2 API
 Home-page: https://github.com/ParticulateSolutions/django-paypal-plus
 Author: Particulate Solutions GmbH
 Author-email: tech@particulate.me
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-paypal-plus-1.0.1/django_paypal_plus.egg-info/SOURCES.txt` & `django-paypal-plus-1.1.0/django_paypal_plus.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -33,20 +33,22 @@
 django_paypal/__pycache__/wrappers.cpython-311.pyc
 django_paypal/__pycache__/wrappers.cpython-38.pyc
 django_paypal/migrations/0001_initial.py
 django_paypal/migrations/0002_auto_20171002_1551.py
 django_paypal/migrations/0003_auto_20200124_1528.py
 django_paypal/migrations/0004_paypalpayment_related_resource_state.py
 django_paypal/migrations/0005_auto_20240207_0630.py
+django_paypal/migrations/0006_auto_20240424_0727.py
 django_paypal/migrations/__init__.py
 django_paypal/migrations/__pycache__/0001_initial.cpython-38.pyc
 django_paypal/migrations/__pycache__/0002_auto_20171002_1551.cpython-38.pyc
 django_paypal/migrations/__pycache__/0003_auto_20200124_1528.cpython-38.pyc
 django_paypal/migrations/__pycache__/0004_paypalpayment_related_resource_state.cpython-38.pyc
 django_paypal/migrations/__pycache__/0005_auto_20240207_0630.cpython-38.pyc
+django_paypal/migrations/__pycache__/0006_auto_20240424_0727.cpython-38.pyc
 django_paypal/migrations/__pycache__/__init__.cpython-38.pyc
 django_paypal_plus.egg-info/PKG-INFO
 django_paypal_plus.egg-info/SOURCES.txt
 django_paypal_plus.egg-info/dependency_links.txt
 django_paypal_plus.egg-info/not-zip-safe
 django_paypal_plus.egg-info/requires.txt
 django_paypal_plus.egg-info/top_level.txt
```

### Comparing `django-paypal-plus-1.0.1/setup.py` & `django-paypal-plus-1.1.0/setup.py`

 * *Files identical despite different names*

