# Comparing `tmp/llm_monitoring_sascha-0.0.6.tar.gz` & `tmp/llm_monitoring_sascha-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_monitoring_sascha-0.0.6.tar", last modified: Fri Apr 26 08:46:53 2024, max compression
+gzip compressed data, was "llm_monitoring_sascha-0.0.7.tar", last modified: Fri Apr 26 08:55:01 2024, max compression
```

## Comparing `llm_monitoring_sascha-0.0.6.tar` & `llm_monitoring_sascha-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:46:53.199233 llm_monitoring_sascha-0.0.6/
--rw-r--r--   0 sascha     (501) staff       (20)        8 2024-04-26 07:51:08.000000 llm_monitoring_sascha-0.0.6/LICENSE
--rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:46:53.198881 llm_monitoring_sascha-0.0.6/PKG-INFO
--rw-r--r--   0 sascha     (501) staff       (20)       10 2023-12-21 09:09:33.000000 llm_monitoring_sascha-0.0.6/README.md
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:46:53.198356 llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/
--rw-r--r--   0 sascha     (501) staff       (20)      526 2024-04-26 08:46:53.000000 llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/PKG-INFO
--rw-r--r--   0 sascha     (501) staff       (20)      276 2024-04-26 08:46:53.000000 llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/SOURCES.txt
--rw-r--r--   0 sascha     (501) staff       (20)        1 2024-04-26 08:46:53.000000 llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/dependency_links.txt
--rw-r--r--   0 sascha     (501) staff       (20)       11 2024-04-26 08:46:53.000000 llm_monitoring_sascha-0.0.6/llm_monitoring_sascha.egg-info/top_level.txt
-drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:46:53.197929 llm_monitoring_sascha-0.0.6/monitoring/
--rw-r--r--   0 sascha     (501) staff       (20)     2113 2024-04-25 14:07:28.000000 llm_monitoring_sascha-0.0.6/monitoring/__init__.py
--rw-r--r--   0 sascha     (501) staff       (20)     4629 2024-04-26 07:28:16.000000 llm_monitoring_sascha-0.0.6/monitoring/client.py
--rw-r--r--   0 sascha     (501) staff       (20)      204 2024-04-26 08:42:20.000000 llm_monitoring_sascha-0.0.6/monitoring/setup.py
--rw-r--r--   0 sascha     (501) staff       (20)      601 2024-04-26 08:46:44.000000 llm_monitoring_sascha-0.0.6/pyproject.toml
--rw-r--r--   0 sascha     (501) staff       (20)       38 2024-04-26 08:46:53.199319 llm_monitoring_sascha-0.0.6/setup.cfg
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:55:01.109447 llm_monitoring_sascha-0.0.7/
+-rw-r--r--   0 sascha     (501) staff       (20)        8 2024-04-26 07:51:08.000000 llm_monitoring_sascha-0.0.7/LICENSE
+-rw-r--r--   0 sascha     (501) staff       (20)      561 2024-04-26 08:55:01.109072 llm_monitoring_sascha-0.0.7/PKG-INFO
+-rw-r--r--   0 sascha     (501) staff       (20)       10 2023-12-21 09:09:33.000000 llm_monitoring_sascha-0.0.7/README.md
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:55:01.108516 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/
+-rw-r--r--   0 sascha     (501) staff       (20)      561 2024-04-26 08:55:01.000000 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/PKG-INFO
+-rw-r--r--   0 sascha     (501) staff       (20)      320 2024-04-26 08:55:01.000000 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/SOURCES.txt
+-rw-r--r--   0 sascha     (501) staff       (20)        1 2024-04-26 08:55:01.000000 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/dependency_links.txt
+-rw-r--r--   0 sascha     (501) staff       (20)       20 2024-04-26 08:55:01.000000 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/requires.txt
+-rw-r--r--   0 sascha     (501) staff       (20)       11 2024-04-26 08:55:01.000000 llm_monitoring_sascha-0.0.7/llm_monitoring_sascha.egg-info/top_level.txt
+drwxr-xr-x   0 sascha     (501) staff       (20)        0 2024-04-26 08:55:01.108183 llm_monitoring_sascha-0.0.7/monitoring/
+-rw-r--r--   0 sascha     (501) staff       (20)     2113 2024-04-25 14:07:28.000000 llm_monitoring_sascha-0.0.7/monitoring/__init__.py
+-rw-r--r--   0 sascha     (501) staff       (20)     4629 2024-04-26 07:28:16.000000 llm_monitoring_sascha-0.0.7/monitoring/client.py
+-rw-r--r--   0 sascha     (501) staff       (20)      186 2024-04-26 08:54:10.000000 llm_monitoring_sascha-0.0.7/monitoring/setup.py
+-rw-r--r--   0 sascha     (501) staff       (20)      644 2024-04-26 08:54:56.000000 llm_monitoring_sascha-0.0.7/pyproject.toml
+-rw-r--r--   0 sascha     (501) staff       (20)       38 2024-04-26 08:55:01.109549 llm_monitoring_sascha-0.0.7/setup.cfg
```

### Comparing `llm_monitoring_sascha-0.0.6/monitoring/__init__.py` & `llm_monitoring_sascha-0.0.7/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_monitoring_sascha-0.0.6/monitoring/client.py` & `llm_monitoring_sascha-0.0.7/monitoring/client.py`

 * *Files identical despite different names*

### Comparing `llm_monitoring_sascha-0.0.6/pyproject.toml` & `llm_monitoring_sascha-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm_monitoring_sascha"
-version = "0.0.6"
+dependencies = [
+  'google-cloud-pubsub'
+]
+version = "0.0.7"
 authors = [
   { name="Sascha Heyer", email="mail@saschaheyer.de" },
   { name="Sascha Heyer", email="sascha@doit.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 classifiers = [
```

