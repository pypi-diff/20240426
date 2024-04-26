# Comparing `tmp/heiwa4126_hello-0.0.6.tar.gz` & `tmp/heiwa4126_hello-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heiwa4126_hello-0.0.6.tar", last modified: Tue Apr 16 08:53:27 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `heiwa4126_hello-0.0.6.tar` & `heiwa4126_hello-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 08:53:27.586609 heiwa4126_hello-0.0.6/
--rw-rw-rw-   0        0        0     1076 2024-04-16 07:47:43.000000 heiwa4126_hello-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3423 2024-04-16 08:53:27.573970 heiwa4126_hello-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-04-16 07:47:43.000000 heiwa4126_hello-0.0.6/README.md
--rw-rw-rw-   0        0        0     1267 2024-04-16 08:36:45.000000 heiwa4126_hello-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 08:53:27.586609 heiwa4126_hello-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 08:53:27.488175 heiwa4126_hello-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 08:53:27.488175 heiwa4126_hello-0.0.6/src/heiwa4126/
-drwxrwxrwx   0        0        0        0 2024-04-16 08:53:27.527567 heiwa4126_hello-0.0.6/src/heiwa4126/hello/
--rw-rw-rw-   0        0        0       62 2024-04-16 07:47:43.000000 heiwa4126_hello-0.0.6/src/heiwa4126/hello/__init__.py
--rw-rw-rw-   0        0        0      156 2024-04-16 07:47:43.000000 heiwa4126_hello-0.0.6/src/heiwa4126/hello/cli.py
--rw-rw-rw-   0        0        0      582 2024-04-16 07:47:43.000000 heiwa4126_hello-0.0.6/src/heiwa4126/hello/hello.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:53:27.563389 heiwa4126_hello-0.0.6/src/heiwa4126.hello.egg-info/
--rw-rw-rw-   0        0        0     3423 2024-04-16 08:53:27.000000 heiwa4126_hello-0.0.6/src/heiwa4126.hello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2024-04-16 08:53:27.000000 heiwa4126_hello-0.0.6/src/heiwa4126.hello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 08:53:27.000000 heiwa4126_hello-0.0.6/src/heiwa4126.hello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-16 08:53:27.000000 heiwa4126_hello-0.0.6/src/heiwa4126.hello.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       46 2024-04-16 08:53:27.000000 heiwa4126_hello-0.0.6/src/heiwa4126.hello.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-16 08:53:27.000000 heiwa4126_hello-0.0.6/src/heiwa4126.hello.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 08:53:27.540396 heiwa4126_hello-0.0.6/tests/
--rw-rw-rw-   0        0        0      712 2024-04-16 07:47:43.000000 heiwa4126_hello-0.0.6/tests/test_hello.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/src/heiwa4126/hello/__about__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/src/heiwa4126/hello/__init__.py
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/src/heiwa4126/hello/cli.py
+-rwxr-xr-x   0        0        0      582 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/src/heiwa4126/hello/hello.py
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/LICENSE
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/README.md
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/PKG-INFO
```

### Comparing `heiwa4126_hello-0.0.6/LICENSE` & `heiwa4126_hello-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `heiwa4126_hello-0.0.6/src/heiwa4126/hello/hello.py` & `heiwa4126_hello-0.0.7/src/heiwa4126/hello/hello.py`

 * *Files identical despite different names*

