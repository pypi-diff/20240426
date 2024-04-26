# Comparing `tmp/hello_world_suraj_test-1.0.0.tar.gz` & `tmp/hello_world_suraj_test-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_world_suraj_test-1.0.0.tar", last modified: Fri Apr 26 07:20:40 2024, max compression
+gzip compressed data, was "hello_world_suraj_test-1.1.0.tar", last modified: Fri Apr 26 07:28:37 2024, max compression
```

## Comparing `hello_world_suraj_test-1.0.0.tar` & `hello_world_suraj_test-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-04-26 07:20:40.291483 hello_world_suraj_test-1.0.0/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       66 2024-04-26 07:20:40.291483 hello_world_suraj_test-1.0.0/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)       66 2024-04-26 07:08:31.000000 hello_world_suraj_test-1.0.0/hello-world.py
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-04-26 07:20:40.271483 hello_world_suraj_test-1.0.0/hello_world_suraj_test.egg-info/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       66 2024-04-26 07:20:40.000000 hello_world_suraj_test-1.0.0/hello_world_suraj_test.egg-info/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)      207 2024-04-26 07:20:40.000000 hello_world_suraj_test-1.0.0/hello_world_suraj_test.egg-info/SOURCES.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-04-26 07:20:40.000000 hello_world_suraj_test-1.0.0/hello_world_suraj_test.egg-info/dependency_links.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-04-26 07:20:40.000000 hello_world_suraj_test-1.0.0/hello_world_suraj_test.egg-info/top_level.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-26 07:20:40.291483 hello_world_suraj_test-1.0.0/setup.cfg
--rw-r--r--   0 surajram  (1000) surajram  (1000)      127 2024-04-26 07:20:36.000000 hello_world_suraj_test-1.0.0/setup.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-04-26 07:28:37.481488 hello_world_suraj_test-1.1.0/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       66 2024-04-26 07:28:37.481488 hello_world_suraj_test-1.1.0/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      129 2024-04-26 07:27:39.000000 hello_world_suraj_test-1.1.0/hello-world.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-04-26 07:28:37.481488 hello_world_suraj_test-1.1.0/hello_world_suraj_test.egg-info/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       66 2024-04-26 07:28:37.000000 hello_world_suraj_test-1.1.0/hello_world_suraj_test.egg-info/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      207 2024-04-26 07:28:37.000000 hello_world_suraj_test-1.1.0/hello_world_suraj_test.egg-info/SOURCES.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-04-26 07:28:37.000000 hello_world_suraj_test-1.1.0/hello_world_suraj_test.egg-info/dependency_links.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-04-26 07:28:37.000000 hello_world_suraj_test-1.1.0/hello_world_suraj_test.egg-info/top_level.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-26 07:28:37.481488 hello_world_suraj_test-1.1.0/setup.cfg
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      127 2024-04-26 07:28:32.000000 hello_world_suraj_test-1.1.0/setup.py
```

