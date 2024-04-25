# Comparing `tmp/dir2prompt-1.0.8.tar.gz` & `tmp/dir2prompt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dir2prompt-1.0.8.tar", last modified: Thu Apr 25 18:49:59 2024, max compression
+gzip compressed data, was "dir2prompt-1.0.9.tar", last modified: Thu Apr 25 19:02:24 2024, max compression
```

## Comparing `dir2prompt-1.0.8.tar` & `dir2prompt-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 18:49:59.735705 dir2prompt-1.0.8/
--rw-r--r--   0 mkieffer   (501) staff       (20)     1069 2024-04-02 23:08:45.000000 dir2prompt-1.0.8/LICENSE
--rw-r--r--   0 mkieffer   (501) staff       (20)     6550 2024-04-25 18:49:59.735471 dir2prompt-1.0.8/PKG-INFO
--rw-r--r--   0 mkieffer   (501) staff       (20)     4322 2024-04-25 15:53:20.000000 dir2prompt-1.0.8/README.md
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 18:49:59.734146 dir2prompt-1.0.8/dir2prompt/
--rw-r--r--   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:44:25.000000 dir2prompt-1.0.8/dir2prompt/__init__.py
--rw-r--r--   0 mkieffer   (501) staff       (20)      978 2024-04-02 23:57:47.000000 dir2prompt-1.0.8/dir2prompt/config.json
--rw-r--r--   0 mkieffer   (501) staff       (20)     7923 2024-04-25 18:46:36.000000 dir2prompt-1.0.8/dir2prompt/d2p.py
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 18:49:59.735175 dir2prompt-1.0.8/dir2prompt.egg-info/
--rw-r--r--   0 mkieffer   (501) staff       (20)     6550 2024-04-25 18:49:59.000000 dir2prompt-1.0.8/dir2prompt.egg-info/PKG-INFO
--rw-r--r--   0 mkieffer   (501) staff       (20)      269 2024-04-25 18:49:59.000000 dir2prompt-1.0.8/dir2prompt.egg-info/SOURCES.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)        1 2024-04-25 18:49:59.000000 dir2prompt-1.0.8/dir2prompt.egg-info/dependency_links.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)       44 2024-04-25 18:49:59.000000 dir2prompt-1.0.8/dir2prompt.egg-info/entry_points.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)       11 2024-04-25 18:49:59.000000 dir2prompt-1.0.8/dir2prompt.egg-info/top_level.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)     1271 2024-04-25 17:32:20.000000 dir2prompt-1.0.8/pyproject.toml
--rw-r--r--   0 mkieffer   (501) staff       (20)       38 2024-04-25 18:49:59.735753 dir2prompt-1.0.8/setup.cfg
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 19:02:24.402701 dir2prompt-1.0.9/
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1069 2024-04-02 23:08:45.000000 dir2prompt-1.0.9/LICENSE
+-rw-r--r--   0 mkieffer   (501) staff       (20)     6550 2024-04-25 19:02:24.402489 dir2prompt-1.0.9/PKG-INFO
+-rw-r--r--   0 mkieffer   (501) staff       (20)     4322 2024-04-25 18:54:42.000000 dir2prompt-1.0.9/README.md
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 19:02:24.401246 dir2prompt-1.0.9/dir2prompt/
+-rw-r--r--   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:44:25.000000 dir2prompt-1.0.9/dir2prompt/__init__.py
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1129 2024-04-25 19:01:33.000000 dir2prompt-1.0.9/dir2prompt/config.json
+-rw-r--r--   0 mkieffer   (501) staff       (20)     7923 2024-04-25 18:59:07.000000 dir2prompt-1.0.9/dir2prompt/d2p.py
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 19:02:24.402191 dir2prompt-1.0.9/dir2prompt.egg-info/
+-rw-r--r--   0 mkieffer   (501) staff       (20)     6550 2024-04-25 19:02:24.000000 dir2prompt-1.0.9/dir2prompt.egg-info/PKG-INFO
+-rw-r--r--   0 mkieffer   (501) staff       (20)      269 2024-04-25 19:02:24.000000 dir2prompt-1.0.9/dir2prompt.egg-info/SOURCES.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)        1 2024-04-25 19:02:24.000000 dir2prompt-1.0.9/dir2prompt.egg-info/dependency_links.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)       44 2024-04-25 19:02:24.000000 dir2prompt-1.0.9/dir2prompt.egg-info/entry_points.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)       11 2024-04-25 19:02:24.000000 dir2prompt-1.0.9/dir2prompt.egg-info/top_level.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1271 2024-04-25 19:02:08.000000 dir2prompt-1.0.9/pyproject.toml
+-rw-r--r--   0 mkieffer   (501) staff       (20)       38 2024-04-25 19:02:24.402748 dir2prompt-1.0.9/setup.cfg
```

### Comparing `dir2prompt-1.0.8/LICENSE` & `dir2prompt-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.8/PKG-INFO` & `dir2prompt-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir2prompt
-Version: 1.0.8
+Version: 1.0.9
 Summary: Generate prompts for long-context LLMs using the content in your directory
 Author-email: Max Kieffer <wkieffer@ufl.edu>
 License: MIT License
         
         Copyright (c) 2024 mkieffer1107
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dir2prompt-1.0.8/README.md` & `dir2prompt-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.8/dir2prompt/config.json` & `dir2prompt-1.0.9/dir2prompt/config.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9423076923076923%*

 * *Differences: {"'IGNORE_FILES'": "{insert: [(30, '*.zip'), (31, '*.gz'), (32, '*.bz2'), (33, '*.tar'), (34, "*

 * *                   "'*.tgz'), (35, '*.7z'), (36, '*.rar'), (37, '*.iso'), (38, '*.dmg')]}"}*

```diff
@@ -45,10 +45,19 @@
         "*.dll",
         "*.exe",
         "*.o",
         "*.obj",
         "*.so",
         "*.a",
         "*.lib",
-        "*.pdb"
+        "*.pdb",
+        "*.zip",
+        "*.gz",
+        "*.bz2",
+        "*.tar",
+        "*.tgz",
+        "*.7z",
+        "*.rar",
+        "*.iso",
+        "*.dmg"
     ]
 }
```

### Comparing `dir2prompt-1.0.8/dir2prompt/d2p.py` & `dir2prompt-1.0.9/dir2prompt/d2p.py`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.8/dir2prompt.egg-info/PKG-INFO` & `dir2prompt-1.0.9/dir2prompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir2prompt
-Version: 1.0.8
+Version: 1.0.9
 Summary: Generate prompts for long-context LLMs using the content in your directory
 Author-email: Max Kieffer <wkieffer@ufl.edu>
 License: MIT License
         
         Copyright (c) 2024 mkieffer1107
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dir2prompt-1.0.8/pyproject.toml` & `dir2prompt-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dir2prompt"
-version = "1.0.8"
+version = "1.0.9"
 license = {file = "LICENSE"}
 authors = [
   { name="Max Kieffer", email="wkieffer@ufl.edu" },
 ]
 description = "Generate prompts for long-context LLMs using the content in your directory"
 readme = "README.md"
 requires-python = ">=3.6"
```

