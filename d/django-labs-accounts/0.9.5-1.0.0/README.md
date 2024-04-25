# Comparing `tmp/django_labs_accounts-0.9.5.tar.gz` & `tmp/django_labs_accounts-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_labs_accounts-0.9.5.tar", max compression
+gzip compressed data, was "django_labs_accounts-1.0.0.tar", max compression
```

## Comparing `django_labs_accounts-0.9.5.tar` & `django_labs_accounts-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0     2757 2024-03-03 03:03:29.470227 django_labs_accounts-0.9.5/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/LICENSE
--rw-r--r--   0        0        0     6206 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/README.md
--rw-r--r--   0        0        0        0 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/__init__.py
--rw-r--r--   0        0        0     1402 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/admin.py
--rw-r--r--   0        0        0      138 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/apps.py
--rw-r--r--   0        0        0     2751 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/authentication.py
--rw-r--r--   0        0        0     2958 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/backends.py
--rw-r--r--   0        0        0     3292 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/ipc.py
--rw-r--r--   0        0        0     1860 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/migrations/__init__.py
--rw-r--r--   0        0        0      899 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/migrations/rename_groups.py
--rw-r--r--   0        0        0      587 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/models.py
--rw-r--r--   0        0        0     1124 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/settings.py
--rw-r--r--   0        0        0      380 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/urls.py
--rw-r--r--   0        0        0     6090 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/accounts/views.py
--rw-r--r--   0        0        0        0 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/identity/__init__.py
--rw-r--r--   0        0        0      263 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/identity/apps.py
--rw-r--r--   0        0        0     4415 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/identity/identity.py
--rw-r--r--   0        0        0     1556 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/identity/permissions.py
--rw-r--r--   0        0        0      971 2024-03-03 03:03:29.474227 django_labs_accounts-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     7055 1970-01-01 00:00:00.000000 django_labs_accounts-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     2825 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6206 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/__init__.py
+-rw-r--r--   0        0        0     1402 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/admin.py
+-rw-r--r--   0        0        0      138 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/apps.py
+-rw-r--r--   0        0        0     2751 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/authentication.py
+-rw-r--r--   0        0        0     2958 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/backends.py
+-rw-r--r--   0        0        0     3292 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/ipc.py
+-rw-r--r--   0        0        0     1860 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/migrations/__init__.py
+-rw-r--r--   0        0        0      899 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/migrations/rename_groups.py
+-rw-r--r--   0        0        0      587 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/models.py
+-rw-r--r--   0        0        0     1124 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/settings.py
+-rw-r--r--   0        0        0      380 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/urls.py
+-rw-r--r--   0        0        0     6090 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/accounts/views.py
+-rw-r--r--   0        0        0        0 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/analytics/__init__.py
+-rw-r--r--   0        0        0     2594 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/analytics/analytics.py
+-rw-r--r--   0        0        0      141 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/analytics/apps.py
+-rw-r--r--   0        0        0        0 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/identity/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/identity/apps.py
+-rw-r--r--   0        0        0     4415 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/identity/identity.py
+-rw-r--r--   0        0        0     1556 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/identity/permissions.py
+-rw-r--r--   0        0        0     1002 2024-04-25 23:26:42.210401 django_labs_accounts-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7055 1970-01-01 00:00:00.000000 django_labs_accounts-1.0.0/PKG-INFO
```

### Comparing `django_labs_accounts-0.9.5/CHANGELOG.md` & `django_labs_accounts-1.0.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Changelog
 =========
 
 x.y.z (UNRELEASED)
 ------------------
 * Changes
 
+1.0.0 (2024-04-25)
+------------------
+* Introducing Labs Analytics
+
 0.9.5 (2024-03-02)
 ------------------
 * Mandate Python 3.11 and Django 5.0.2
 
 0.9.4 (2023-08-27)
 ------------------
 * Authenticate user in TokenView for mobile users
```

### Comparing `django_labs_accounts-0.9.5/LICENSE` & `django_labs_accounts-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/README.md` & `django_labs_accounts-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/accounts/admin.py` & `django_labs_accounts-1.0.0/accounts/admin.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/accounts/authentication.py` & `django_labs_accounts-1.0.0/accounts/authentication.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/accounts/backends.py` & `django_labs_accounts-1.0.0/accounts/backends.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/accounts/ipc.py` & `django_labs_accounts-1.0.0/accounts/ipc.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/accounts/migrations/0001_initial.py` & `django_labs_accounts-1.0.0/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/accounts/migrations/rename_groups.py` & `django_labs_accounts-1.0.0/accounts/migrations/rename_groups.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/accounts/models.py` & `django_labs_accounts-1.0.0/accounts/models.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/accounts/settings.py` & `django_labs_accounts-1.0.0/accounts/settings.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/accounts/views.py` & `django_labs_accounts-1.0.0/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/identity/identity.py` & `django_labs_accounts-1.0.0/identity/identity.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/identity/permissions.py` & `django_labs_accounts-1.0.0/identity/permissions.py`

 * *Files identical despite different names*

### Comparing `django_labs_accounts-0.9.5/pyproject.toml` & `django_labs_accounts-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "django-labs-accounts"
-version = "0.9.5"
+version = "1.0.0"
 description = "Reusable Django app for Penn Labs accounts"
 authors = ["Penn Labs <contact@pennlabs.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pennlabs/django-labs-accounts"
 repository = "https://github.com/pennlabs/django-labs-accounts"
 include = ["CHANGELOG.md", "LICENSE"]
 exclude = ["tox.ini"]
 packages = [
     { include = "accounts" },
     { include = "identity" },
+    { include = "analytics" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 Django = "^5.0.2"
 requests-oauthlib = "^1.3.1"
 requests = "^2.0.0"
```

### Comparing `django_labs_accounts-0.9.5/PKG-INFO` & `django_labs_accounts-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-labs-accounts
-Version: 0.9.5
+Version: 1.0.0
 Summary: Reusable Django app for Penn Labs accounts
 Home-page: https://github.com/pennlabs/django-labs-accounts
 License: MIT
 Author: Penn Labs
 Author-email: contact@pennlabs.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

