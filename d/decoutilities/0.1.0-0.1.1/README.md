# Comparing `tmp/decoutilities-0.1.0.tar.gz` & `tmp/decoutilities-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.1.0.tar", last modified: Fri Apr 26 13:56:16 2024, max compression
+gzip compressed data, was "decoutilities-0.1.1.tar", last modified: Fri Apr 26 14:45:28 2024, max compression
```

## Comparing `decoutilities-0.1.0.tar` & `decoutilities-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 13:56:16.332088 decoutilities-0.1.0/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      377 2024-04-26 13:56:16.319089 decoutilities-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-26 13:56:16.165091 decoutilities-0.1.0/config/
--rw-rw-rw-   0        0        0       70 2024-04-26 13:18:54.000000 decoutilities-0.1.0/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.0/config/config.py
--rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.0/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-04-26 13:56:16.296089 decoutilities-0.1.0/decoutilities.egg-info/
--rw-rw-rw-   0        0        0      377 2024-04-26 13:56:15.000000 decoutilities-0.1.0/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-04-26 13:56:16.000000 decoutilities-0.1.0/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 13:56:15.000000 decoutilities-0.1.0/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-26 13:56:15.000000 decoutilities-0.1.0/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 13:56:16.333089 decoutilities-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      420 2024-04-25 11:45:26.000000 decoutilities-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:45:28.551296 decoutilities-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3053 2024-04-26 14:45:28.528297 decoutilities-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2024-04-26 14:17:02.000000 decoutilities-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 14:45:28.389265 decoutilities-0.1.1/config/
+-rw-rw-rw-   0        0        0       70 2024-04-26 13:18:54.000000 decoutilities-0.1.1/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.1/config/config.py
+-rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.1/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-04-26 14:45:28.505293 decoutilities-0.1.1/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0     3053 2024-04-26 14:45:28.000000 decoutilities-0.1.1/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-04-26 14:45:28.000000 decoutilities-0.1.1/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 14:45:28.000000 decoutilities-0.1.1/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-26 14:45:28.000000 decoutilities-0.1.1/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 14:45:28.552295 decoutilities-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      636 2024-04-26 14:44:49.000000 decoutilities-0.1.1/setup.py
```

### Comparing `decoutilities-0.1.0/LICENSE` & `decoutilities-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.0/config/config.py` & `decoutilities-0.1.1/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.0/config/configContainer.py` & `decoutilities-0.1.1/config/configContainer.py`

 * *Files identical despite different names*

