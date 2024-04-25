# Comparing `tmp/django_unfold_admin_list_filter_dropdown-1.0.0.tar.gz` & `tmp/django_unfold_admin_list_filter_dropdown-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_unfold_admin_list_filter_dropdown-1.0.0.tar", last modified: Wed Apr 24 21:48:18 2024, max compression
+gzip compressed data, was "django_unfold_admin_list_filter_dropdown-1.0.2.tar", last modified: Thu Apr 25 23:24:02 2024, max compression
```

## Comparing `django_unfold_admin_list_filter_dropdown-1.0.0.tar` & `django_unfold_admin_list_filter_dropdown-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:48:18.048224 django_unfold_admin_list_filter_dropdown-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 21:48:14.000000 django_unfold_admin_list_filter_dropdown-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 21:48:14.000000 django_unfold_admin_list_filter_dropdown-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-24 21:48:18.048224 django_unfold_admin_list_filter_dropdown-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-24 21:48:14.000000 django_unfold_admin_list_filter_dropdown-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:48:18.048224 django_unfold_admin_list_filter_dropdown-1.0.0/django_unfold_admin_list_filter_dropdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-24 21:48:18.000000 django_unfold_admin_list_filter_dropdown-1.0.0/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-24 21:48:18.000000 django_unfold_admin_list_filter_dropdown-1.0.0/django_unfold_admin_list_filter_dropdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:48:18.000000 django_unfold_admin_list_filter_dropdown-1.0.0/django_unfold_admin_list_filter_dropdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 21:48:18.000000 django_unfold_admin_list_filter_dropdown-1.0.0/django_unfold_admin_list_filter_dropdown.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:48:18.048224 django_unfold_admin_list_filter_dropdown-1.0.0/django_unfold_admin_listfilter_dropdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:48:14.000000 django_unfold_admin_list_filter_dropdown-1.0.0/django_unfold_admin_listfilter_dropdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 21:48:14.000000 django_unfold_admin_list_filter_dropdown-1.0.0/django_unfold_admin_listfilter_dropdown/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 21:48:18.048224 django_unfold_admin_list_filter_dropdown-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 21:48:14.000000 django_unfold_admin_list_filter_dropdown-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:24:02.983619 django_unfold_admin_list_filter_dropdown-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 23:23:59.000000 django_unfold_admin_list_filter_dropdown-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-25 23:23:59.000000 django_unfold_admin_list_filter_dropdown-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-25 23:24:02.983619 django_unfold_admin_list_filter_dropdown-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-25 23:23:59.000000 django_unfold_admin_list_filter_dropdown-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:24:02.983619 django_unfold_admin_list_filter_dropdown-1.0.2/django_unfold_admin_list_filter_dropdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-25 23:24:02.000000 django_unfold_admin_list_filter_dropdown-1.0.2/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-25 23:24:02.000000 django_unfold_admin_list_filter_dropdown-1.0.2/django_unfold_admin_list_filter_dropdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 23:24:02.000000 django_unfold_admin_list_filter_dropdown-1.0.2/django_unfold_admin_list_filter_dropdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 23:24:02.000000 django_unfold_admin_list_filter_dropdown-1.0.2/django_unfold_admin_list_filter_dropdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:24:02.983619 django_unfold_admin_list_filter_dropdown-1.0.2/django_unfold_admin_listfilter_dropdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 23:23:59.000000 django_unfold_admin_list_filter_dropdown-1.0.2/django_unfold_admin_listfilter_dropdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-25 23:23:59.000000 django_unfold_admin_list_filter_dropdown-1.0.2/django_unfold_admin_listfilter_dropdown/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 23:24:02.983619 django_unfold_admin_list_filter_dropdown-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-25 23:23:59.000000 django_unfold_admin_list_filter_dropdown-1.0.2/setup.py
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.0/LICENSE` & `django_unfold_admin_list_filter_dropdown-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.0/PKG-INFO` & `django_unfold_admin_list_filter_dropdown-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,13 @@
-Metadata-Version: 2.1
-Name: django-unfold-admin-list-filter-dropdown
-Version: 1.0.0
-Summary: Use dropdowns in Django admin list filter
-Home-page: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdown
-Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.0.zip
-Author: Franco Borrelli
-Author-email: francoborrelli96@gmail.com
-License: MIT License
-Keywords: django,admin,filter,dropdown,unfold,django-unfold
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # django-unfold-admin-list-filter-dropdown
 
-This version is compatible with [django-unfold](https://github.com/unfoldadmin/django-unfold).
+[![PyPI version](https://badge.fury.io/py/django-unfold-admin-list-filter-dropdown.svg)](https://badge.fury.io/py/django-unfold-admin-list-filter-dropdown)
+
+> [!NOTE]  
+> This version is compatible with [django-unfold](https://github.com/unfoldadmin/django-unfold).
 
 A Django admin filter implementation that renders as a dropdown.
 
 If you have more than ten values for a field that you want to filter by in
 Django admin, the filtering sidebar gets long, cluttered and hard to use.
 
 This app contains the `DropdownFilter` class that renders as a drop-down in the
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.0/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO` & `django_unfold_admin_list_filter_dropdown-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-unfold-admin-list-filter-dropdown
-Version: 1.0.0
+Version: 1.0.2
 Summary: Use dropdowns in Django admin list filter
 Home-page: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdown
-Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.0.zip
+Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.2.zip
 Author: Franco Borrelli
 Author-email: francoborrelli96@gmail.com
 License: MIT License
 Keywords: django,admin,filter,dropdown,unfold,django-unfold
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,18 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-unfold-admin-list-filter-dropdown
 
-This version is compatible with [django-unfold](https://github.com/unfoldadmin/django-unfold).
+[![PyPI version](https://badge.fury.io/py/django-unfold-admin-list-filter-dropdown.svg)](https://badge.fury.io/py/django-unfold-admin-list-filter-dropdown)
+
+> [!NOTE]  
+> This version is compatible with [django-unfold](https://github.com/unfoldadmin/django-unfold).
 
 A Django admin filter implementation that renders as a dropdown.
 
 If you have more than ten values for a field that you want to filter by in
 Django admin, the filtering sidebar gets long, cluttered and hard to use.
 
 This app contains the `DropdownFilter` class that renders as a drop-down in the
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.0/django_unfold_admin_listfilter_dropdown/filters.py` & `django_unfold_admin_list_filter_dropdown-1.0.2/django_unfold_admin_listfilter_dropdown/filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,24 @@
     ChoicesFieldListFilter,
     RelatedFieldListFilter,
     RelatedOnlyFieldListFilter
 )
 
 
 class SimpleDropdownFilter(SimpleListFilter):
-    template = 'django_unfold_admin_listfilter_dropdown/dropdown_filter.html'
+    template = 'django_unfold_admin_listfilter_dropdown/templates/dropdown_filter.html'
 
 
 class DropdownFilter(AllValuesFieldListFilter):
-    template = 'django_unfold_admin_listfilter_dropdown/dropdown_filter.html'
+    template = 'django_unfold_admin_listfilter_dropdown/templates/dropdown_filter.html'
 
 
 class ChoiceDropdownFilter(ChoicesFieldListFilter):
-    template = 'django_unfold_admin_listfilter_dropdown/dropdown_filter.html'
+    template = 'django_unfold_admin_listfilter_dropdown/templates/dropdown_filter.html'
 
 
 class RelatedDropdownFilter(RelatedFieldListFilter):
-    template = 'django_unfold_admin_listfilter_dropdown/dropdown_filter.html'
+    template = 'django_unfold_admin_listfilter_dropdown/templates/dropdown_filter.html'
 
 
 class RelatedOnlyDropdownFilter(RelatedOnlyFieldListFilter):
-    template = 'django_unfold_admin_listfilter_dropdown/dropdown_filter.html'
+    template = 'django_unfold_admin_listfilter_dropdown/templates/dropdown_filter.html'
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.0/setup.py` & `django_unfold_admin_list_filter_dropdown-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # encoding: utf-8
 
 import os
 from setuptools import find_packages, setup
 
-VERSION = '1.0.0'
+VERSION = '1.0.2'
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 description = 'Use dropdowns in Django admin list filter'
 
 setup(
```

