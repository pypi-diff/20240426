# Comparing `tmp/logger_aux-0.0.1.tar.gz` & `tmp/logger_aux-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_aux-0.0.1.tar", last modified: Thu Apr 25 12:43:54 2024, max compression
+gzip compressed data, was "logger_aux-0.0.2.tar", last modified: Thu Apr 25 13:57:52 2024, max compression
```

## Comparing `logger_aux-0.0.1.tar` & `logger_aux-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 12:43:54.959790 logger_aux-0.0.1/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6213 2024-04-25 12:43:54.958789 logger_aux-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5413 2024-04-25 12:43:29.000000 logger_aux-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 12:43:54.952747 logger_aux-0.0.1/logger_aux/
--rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.1/logger_aux/__init__.py
--rw-rw-rw-   0        0        0     4427 2024-04-25 12:25:02.000000 logger_aux-0.0.1/logger_aux/main.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:43:54.958789 logger_aux-0.0.1/logger_aux.egg-info/
--rw-rw-rw-   0        0        0     6213 2024-04-25 12:43:54.000000 logger_aux-0.0.1/logger_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-25 12:43:54.000000 logger_aux-0.0.1/logger_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 12:43:54.000000 logger_aux-0.0.1/logger_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 12:43:54.000000 logger_aux-0.0.1/logger_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 12:43:54.959790 logger_aux-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 logger_aux-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:57:52.178115 logger_aux-0.0.2/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6665 2024-04-25 13:57:52.178115 logger_aux-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5865 2024-04-25 13:57:27.000000 logger_aux-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 13:57:52.169510 logger_aux-0.0.2/logger_aux/
+-rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.2/logger_aux/__init__.py
+-rw-rw-rw-   0        0        0     4427 2024-04-25 12:25:02.000000 logger_aux-0.0.2/logger_aux/main.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:57:52.177468 logger_aux-0.0.2/logger_aux.egg-info/
+-rw-rw-rw-   0        0        0     6665 2024-04-25 13:57:52.000000 logger_aux-0.0.2/logger_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-25 13:57:52.000000 logger_aux-0.0.2/logger_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 13:57:52.000000 logger_aux-0.0.2/logger_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 13:57:52.000000 logger_aux-0.0.2/logger_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 13:57:52.179150 logger_aux-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 logger_aux-0.0.2/setup.py
```

### Comparing `logger_aux-0.0.1/LICENSE` & `logger_aux-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logger_aux-0.0.1/logger_aux/main.py` & `logger_aux-0.0.2/logger_aux/main.py`

 * *Files identical despite different names*

### Comparing `logger_aux-0.0.1/setup.py` & `logger_aux-0.0.2/setup.py`

 * *Files identical despite different names*

