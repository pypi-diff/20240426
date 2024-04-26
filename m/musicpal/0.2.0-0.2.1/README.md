# Comparing `tmp/musicpal-0.2.0.tar.gz` & `tmp/musicpal-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicpal-0.2.0.tar", last modified: Sun Mar 17 16:09:23 2024, max compression
+gzip compressed data, was "musicpal-0.2.1.tar", last modified: Fri Apr 26 16:07:01 2024, max compression
```

## Comparing `musicpal-0.2.0.tar` & `musicpal-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:09:23.938271 musicpal-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:09:23.934271 musicpal-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:09:23.934271 musicpal-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-17 16:09:19.000000 musicpal-0.2.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-17 16:09:19.000000 musicpal-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-17 16:09:19.000000 musicpal-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-17 16:09:19.000000 musicpal-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-17 16:09:23.938271 musicpal-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-03-17 16:09:19.000000 musicpal-0.2.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-03-17 16:09:19.000000 musicpal-0.2.0/mpal
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:09:23.934271 musicpal-0.2.0/musicpal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 16:09:19.000000 musicpal-0.2.0/musicpal/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10164 2024-03-17 16:09:19.000000 musicpal-0.2.0/musicpal/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:09:23.938271 musicpal-0.2.0/musicpal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-17 16:09:23.000000 musicpal-0.2.0/musicpal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-17 16:09:23.000000 musicpal-0.2.0/musicpal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 16:09:23.000000 musicpal-0.2.0/musicpal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-17 16:09:23.000000 musicpal-0.2.0/musicpal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-17 16:09:23.000000 musicpal-0.2.0/musicpal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-17 16:09:23.000000 musicpal-0.2.0/musicpal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-17 16:09:19.000000 musicpal-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 16:09:23.938271 musicpal-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-17 16:09:19.000000 musicpal-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:07:01.259064 musicpal-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:07:01.259064 musicpal-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:07:01.259064 musicpal-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-26 16:06:56.000000 musicpal-0.2.1/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 16:06:56.000000 musicpal-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-26 16:06:56.000000 musicpal-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 16:06:56.000000 musicpal-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-26 16:07:01.259064 musicpal-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-26 16:06:56.000000 musicpal-0.2.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10164 2024-04-26 16:06:56.000000 musicpal-0.2.1/musicpal
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:07:01.259064 musicpal-0.2.1/musicpal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-26 16:07:01.000000 musicpal-0.2.1/musicpal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-26 16:07:01.000000 musicpal-0.2.1/musicpal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:07:01.000000 musicpal-0.2.1/musicpal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 16:07:01.000000 musicpal-0.2.1/musicpal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:07:01.000000 musicpal-0.2.1/musicpal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-26 16:06:56.000000 musicpal-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:07:01.259064 musicpal-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-26 16:06:56.000000 musicpal-0.2.1/setup.py
```

### Comparing `musicpal-0.2.0/.github/workflows/publish-to-test-pypi.yml` & `musicpal-0.2.1/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `musicpal-0.2.0/LICENSE` & `musicpal-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `musicpal-0.2.0/PKG-INFO` & `musicpal-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicpal
-Version: 0.2.0
+Version: 0.2.1
 Summary: Command line interface for remote controlling a Freecom MusicPal
 Home-page: https://github.com/jmechnich/musicpal
 Author: Joerg Mechnich
 Author-email: joerg.mechnich@gmail.com
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -34,20 +34,14 @@
 
 The last stable firmware version 1.67 sports a 2.6.16 Linux
 kernel. All services are offered by a single application called
 _Nashville_ which, unfortunately, is closed source.
 
 ### Usage
 
-After installation using `pip` or `pipx`, use the command `musicpal`
-will be available.
-
-When running locally from this repository, the wrapper script `mpal`
-in the top-level directory or `python3 -m musicpal` can be used, alternatively.
-
 ```
 usage: musicpal [--help] [-h HOSTNAME] [-u USERNAME] [-p PASSWORD] [-d] [-l]
                 [command] [args ...]
 
 Command line client for the Freecom MusicPal.
 
 positional arguments:
```

### Comparing `musicpal-0.2.0/README.md` & `musicpal-0.2.1/musicpal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: musicpal
+Version: 0.2.1
+Summary: Command line interface for remote controlling a Freecom MusicPal
+Home-page: https://github.com/jmechnich/musicpal
+Author: Joerg Mechnich
+Author-email: joerg.mechnich@gmail.com
+License: GNU GPLv3
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
+Requires-Dist: requests
+
 [![PyPI versio](https://img.shields.io/pypi/v/musicpal)](https://pypi.org/project/musicpal/)
 [![PyPi format](https://img.shields.io/pypi/format/musicpal)](https://pypi.org/project/musicpal/)
 [![PyPI license](https://img.shields.io/pypi/l/musicpal)](https://pypi.org/project/musicpal/)
 [![PyPi weekly downloads](https://img.shields.io/pypi/dw/musicpal)](https://pypi.org/project/musicpal/)
 
 ## musicpal
 
@@ -16,20 +34,14 @@
 
 The last stable firmware version 1.67 sports a 2.6.16 Linux
 kernel. All services are offered by a single application called
 _Nashville_ which, unfortunately, is closed source.
 
 ### Usage
 
-After installation using `pip` or `pipx`, use the command `musicpal`
-will be available.
-
-When running locally from this repository, the wrapper script `mpal`
-in the top-level directory or `python3 -m musicpal` can be used, alternatively.
-
 ```
 usage: musicpal [--help] [-h HOSTNAME] [-u USERNAME] [-p PASSWORD] [-d] [-l]
                 [command] [args ...]
 
 Command line client for the Freecom MusicPal.
 
 positional arguments:
```

### Comparing `musicpal-0.2.0/musicpal/__main__.py` & `musicpal-0.2.1/musicpal`

 * *Files identical despite different names*

### Comparing `musicpal-0.2.0/setup.py` & `musicpal-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,15 @@
     author="Joerg Mechnich",
     author_email="joerg.mechnich@gmail.com",
     license="GNU GPLv3",
     description="Command line interface for remote controlling a Freecom MusicPal",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jmechnich/musicpal",
-    packages=["musicpal"],
-    entry_points={
-        "console_scripts": [
-            "musicpal = musicpal.__main__:main",
-        ]
-    },
+    scripts=["musicpal"],
     use_scm_version={"local_scheme": "no-local-version"},
     setup_requires=["setuptools_scm"],
     install_requires=["beautifulsoup4", "lxml", "requests"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: POSIX :: Linux",
```

