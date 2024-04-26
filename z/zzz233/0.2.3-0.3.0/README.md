# Comparing `tmp/zzz233-0.2.3.tar.gz` & `tmp/zzz233-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zzz233-0.2.3.tar", last modified: Tue May 23 11:16:27 2023, max compression
+gzip compressed data, was "zzz233-0.3.0.tar", last modified: Fri Apr 26 03:22:07 2024, max compression
```

## Comparing `zzz233-0.2.3.tar` & `zzz233-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:16:27.687479 zzz233-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:16:27.679479 zzz233-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:16:27.683479 zzz233-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-23 11:16:08.000000 zzz233-0.2.3/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-23 11:16:08.000000 zzz233-0.2.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-23 11:16:08.000000 zzz233-0.2.3/.github/workflows/unittest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 11:16:08.000000 zzz233-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-23 11:16:08.000000 zzz233-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-23 11:16:27.687479 zzz233-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-23 11:16:08.000000 zzz233-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:16:27.683479 zzz233-0.2.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:16:27.683479 zzz233-0.2.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-23 11:16:08.000000 zzz233-0.2.3/docs/api/all-api.md
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 11:16:08.000000 zzz233-0.2.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-23 11:16:08.000000 zzz233-0.2.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-23 11:16:08.000000 zzz233-0.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:16:27.683479 zzz233-0.2.3/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:16:27.683479 zzz233-0.2.3/python/zzz233/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-23 11:16:08.000000 zzz233-0.2.3/python/zzz233/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-23 11:16:08.000000 zzz233-0.2.3/python/zzz233/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 11:16:27.000000 zzz233-0.2.3/python/zzz233/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:16:27.687479 zzz233-0.2.3/python/zzz233.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-23 11:16:27.000000 zzz233-0.2.3/python/zzz233.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-23 11:16:27.000000 zzz233-0.2.3/python/zzz233.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:16:27.000000 zzz233-0.2.3/python/zzz233.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 11:16:27.000000 zzz233-0.2.3/python/zzz233.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-23 11:16:27.000000 zzz233-0.2.3/python/zzz233.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 11:16:27.000000 zzz233-0.2.3/python/zzz233.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:16:27.687479 zzz233-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:16:27.687479 zzz233-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 11:16:08.000000 zzz233-0.2.3/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:22:07.481053 zzz233-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:22:07.473053 zzz233-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:22:07.477053 zzz233-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-26 03:22:02.000000 zzz233-0.3.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-26 03:22:02.000000 zzz233-0.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-26 03:22:02.000000 zzz233-0.3.0/.github/workflows/unittest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-26 03:22:02.000000 zzz233-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-26 03:22:02.000000 zzz233-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-26 03:22:07.481053 zzz233-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-26 03:22:02.000000 zzz233-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:22:07.477053 zzz233-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:22:07.477053 zzz233-0.3.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-26 03:22:02.000000 zzz233-0.3.0/docs/api/all-api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 03:22:02.000000 zzz233-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-26 03:22:02.000000 zzz233-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-26 03:22:02.000000 zzz233-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:22:07.473053 zzz233-0.3.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:22:07.477053 zzz233-0.3.0/python/zzz233/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-26 03:22:02.000000 zzz233-0.3.0/python/zzz233/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-26 03:22:02.000000 zzz233-0.3.0/python/zzz233/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 03:22:07.000000 zzz233-0.3.0/python/zzz233/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:22:07.477053 zzz233-0.3.0/python/zzz233/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 03:22:02.000000 zzz233-0.3.0/python/zzz233/data/data00.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 03:22:02.000000 zzz233-0.3.0/python/zzz233/data/data01.text
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:22:07.477053 zzz233-0.3.0/python/zzz233.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-26 03:22:07.000000 zzz233-0.3.0/python/zzz233.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 03:22:07.000000 zzz233-0.3.0/python/zzz233.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 03:22:07.000000 zzz233-0.3.0/python/zzz233.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 03:22:07.000000 zzz233-0.3.0/python/zzz233.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-26 03:22:07.000000 zzz233-0.3.0/python/zzz233.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 03:22:07.000000 zzz233-0.3.0/python/zzz233.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 03:22:07.481053 zzz233-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:22:07.477053 zzz233-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-26 03:22:02.000000 zzz233-0.3.0/tests/test_basic.py
```

### Comparing `zzz233-0.2.3/.github/workflows/doc.yml` & `zzz233-0.3.0/.github/workflows/doc.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Sample workflow for building and deploying a mkdocs site to GitHub Pages
-name: Deploy mkdocs to Pages
+name: mkdocs-github-page
 
 
 on:
   push:
-    branches: [$default-branch]
+    branches: [master]
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
 permissions:
   contents: read
   pages: write
```

### Comparing `zzz233-0.2.3/.github/workflows/pypi-publish.yml` & `zzz233-0.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `zzz233-0.2.3/.github/workflows/unittest.yml` & `zzz233-0.3.0/.github/workflows/unittest.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: unittest
 
 on:
   push:
-    branches: [$default-branch]
+    branches: [master]
   pull_request:
-    branches: [$default-branch]
+    branches: [master]
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
```

### Comparing `zzz233-0.2.3/LICENSE` & `zzz233-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zzz233-0.2.3/PKG-INFO` & `zzz233-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,23 @@
-Metadata-Version: 2.1
-Name: zzz233
-Version: 0.2.3
-Summary: a minimalistic python package
-Author-email: husisy <donot@mail.me>
-License: MIT
-Project-URL: Homepage, https://github.com/husisy/zzz233
-Project-URL: Documentation, https://husisy.github.io/zzz233/
-Keywords: toy package
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: doc
-License-File: LICENSE
-
 # zzz233
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhusisy%2Fzzz233.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fhusisy%2Fzzz233?ref=badge_shield)
+
 
 A minimal python package.
 
 1. download locally
-   * clone repository: `git clone xxx`
+   * clone repository: `git clone git@github.com:husisy/zzz233.git`
    * download zip: `wget xxx`
    * download released package: TODO
 2. install
+   * install from pypi: `pip install zzz233`
    * install locally: `pip install .`
    * (for developer) install locally: `pip install ".[dev]"`
    * (for documentation developer) install locally: `pip install ".[doc]"`
    * install from github: `pip install git+https://github.com/husisy/zzz233.git`
-   * TODO pypi
 3. uninstall `pip uninstall zzz233`
 4. scrips
    * run in command line: `zzz233`
 5. unittest: download locally
    * `pytest`
    * (require developer install locally) coverage `pytest --cov=python/zzz233`
 6. documentation
@@ -88,7 +75,11 @@
 # --repository-url https://test.pypi.org/legacy/
 pip uninstall zzz233
 pip install --upgrade -i https://test.pypi.org/simple/ zzz233
 
 # pypi
 # --repository-url https://upload.pypi.org/legacy/
 ```
+
+
+## License
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fhusisy%2Fzzz233.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fhusisy%2Fzzz233?ref=badge_large)
```

### Comparing `zzz233-0.2.3/mkdocs.yml` & `zzz233-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `zzz233-0.2.3/pyproject.toml` & `zzz233-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,7 +40,10 @@
 zzz233 = "zzz233:script_print_lucky"
 
 [tool.setuptools.packages.find]
 where = ["python"]
 
 [tool.setuptools_scm]
 write_to = "python/zzz233/_version.py"
+
+[tool.setuptools.package-data]
+zzz233 = ["data/*.txt"]
```

### Comparing `zzz233-0.2.3/python/zzz233/_internal.py` & `zzz233-0.3.0/python/zzz233/_internal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import random
 import pickle
 import urllib.request
 import urllib.error
 import numpy as np
 
 def to_pickle(**kwargs):
     '''save kwargs to tbd00.pkl
@@ -117,7 +118,32 @@
 
     Parameters:
 
     Returns:
         ret (NoneType): None
     '''
     print('[zzz233] I am feelly lucky today!')
+
+
+def load_package_data(file='data00.txt'):
+    path = os.path.join(os.path.dirname(__file__), 'data', file)
+    if os.path.exists(path):
+        with open(path, 'r') as fid:
+            ret = fid.read().strip()
+    else:
+        print(f'package data file "{file}" not exist')
+        ret = None
+    return ret
+
+def next_tbd_dir(dir0='tbd00', maximum_int=100000, tag_create:bool=True):
+    if not os.path.exists(dir0):
+        os.makedirs(dir0)
+    tmp1 = [x for x in os.listdir(dir0) if x[:3]=='tbd']
+    exist_set = {x[3:] for x in tmp1}
+    while True:
+        tmp1 = str(random.randint(1,maximum_int))
+        if tmp1 not in exist_set:
+            break
+    tbd_dir = os.path.join(dir0, 'tbd'+tmp1)
+    if tag_create:
+        os.mkdir(tbd_dir)
+    return tbd_dir
```

