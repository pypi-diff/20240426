# Comparing `tmp/ccs-digitalmarketplace-frontend-jinja-2.1.1.tar.gz` & `tmp/ccs-digitalmarketplace-frontend-jinja-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-2.1.1.tar", last modified: Wed Apr 24 13:38:00 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-2.2.0.tar", last modified: Fri Apr 26 09:51:05 2024, max compression
```

## Comparing `ccs-digitalmarketplace-frontend-jinja-2.1.1.tar` & `ccs-digitalmarketplace-frontend-jinja-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:38:00.250293 ccs-digitalmarketplace-frontend-jinja-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-24 13:37:47.000000 ccs-digitalmarketplace-frontend-jinja-2.1.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 13:38:00.250293 ccs-digitalmarketplace-frontend-jinja-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-24 13:37:47.000000 ccs-digitalmarketplace-frontend-jinja-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:38:00.250293 ccs-digitalmarketplace-frontend-jinja-2.1.1/app/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-24 13:37:47.000000 ccs-digitalmarketplace-frontend-jinja-2.1.1/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:38:00.250293 ccs-digitalmarketplace-frontend-jinja-2.1.1/ccs_digitalmarketplace_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 13:38:00.000000 ccs-digitalmarketplace-frontend-jinja-2.1.1/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-24 13:38:00.000000 ccs-digitalmarketplace-frontend-jinja-2.1.1/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:38:00.000000 ccs-digitalmarketplace-frontend-jinja-2.1.1/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 13:38:00.000000 ccs-digitalmarketplace-frontend-jinja-2.1.1/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:38:00.000000 ccs-digitalmarketplace-frontend-jinja-2.1.1/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:38:00.250293 ccs-digitalmarketplace-frontend-jinja-2.1.1/digitalmarketplace_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 13:37:47.000000 ccs-digitalmarketplace-frontend-jinja-2.1.1/digitalmarketplace_frontend_jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:38:00.250293 ccs-digitalmarketplace-frontend-jinja-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-24 13:37:47.000000 ccs-digitalmarketplace-frontend-jinja-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-26 09:50:57.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-04-26 09:50:57.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-26 09:50:57.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-26 09:51:05.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-26 09:51:05.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:51:05.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 09:51:05.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:51:05.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/digitalmarketplace_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 09:50:57.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/digitalmarketplace_frontend_jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-26 09:50:57.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/setup.py
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.1.1/LICENCE` & `ccs-digitalmarketplace-frontend-jinja-2.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.1.1/README.md` & `ccs-digitalmarketplace-frontend-jinja-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 ## Compatibility
 
 The following table shows the version of Digital Marketplace Frontend Jinja that you should use for your targeted version of CCS Digital Marketplace GOV.UK Frontend:
 
 | Digital Marketplace Frontend Jinja Version | Target CCS Digital Marketplace GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [2.2.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/2.2.0) | [6.2.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/6.2.0) |
 | [2.1.1](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/2.1.1) | [6.1.1](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/6.1.1) |
 | [2.1.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/2.1.0) | [6.1.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/6.1.0) |
 | [2.0.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/2.0.0) | [6.0.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/6.0.0) |
 | [1.4.1](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.4.1) | [5.5.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.5.0) |
 | [1.4.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.4.0) | [5.5.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.5.0) |
 | [1.3.3](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.3) | [5.4.3](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.3) |
 | [1.3.2](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.2) | [5.4.2](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.2) |
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.1.1/app/__init__.py` & `ccs-digitalmarketplace-frontend-jinja-2.2.0/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.1.1/setup.py` & `ccs-digitalmarketplace-frontend-jinja-2.2.0/setup.py`

 * *Files identical despite different names*

