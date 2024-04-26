# Comparing `tmp/blastpipe-2024.1.2.tar.gz` & `tmp/blastpipe-2024.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.1.2.tar", last modified: Wed Apr 24 21:23:24 2024, max compression
+gzip compressed data, was "blastpipe-2024.1.3.tar", last modified: Fri Apr 26 17:18:23 2024, max compression
```

## Comparing `blastpipe-2024.1.2.tar` & `blastpipe-2024.1.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:23:24.128316 blastpipe-2024.1.2/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5868 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)    82121 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-24 21:23:24.128316 blastpipe-2024.1.2/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/mixin.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      121 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-24 21:17:33.000000 blastpipe-2024.1.2/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:18:23.549308 blastpipe-2024.1.3/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5868 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    83194 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-26 17:18:23.549308 blastpipe-2024.1.3/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/mixin.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      121 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.1.2/.github/workflows/codeql.yml` & `blastpipe-2024.1.3/.github/workflows/codeql.yml`

 * *Files 10% similar despite different names*

```diff
@@ -46,33 +46,33 @@
           egress-policy: audit
 
       - name: Checkout repository
         uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
-        uses: github/codeql-action/init@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
+        uses: github/codeql-action/init@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
         with:
           languages: ${{ matrix.language }}
           # If you wish to specify custom queries, you can do so here or in a config file.
           # By default, queries listed here will override any specified in a config file.
           # Prefix the list here with "+" to use these queries and those in the config file.
 
       # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
       # If this step fails, then you should remove it and run the build manually (see below)
       - name: Autobuild
-        uses: github/codeql-action/autobuild@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
+        uses: github/codeql-action/autobuild@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
 
       # ℹ️ Command-line programs to run using the OS shell.
       # 📚 See https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepsrun
 
       #   If the Autobuild fails above, remove it and uncomment the following three lines.
       #   modify them (or add more) to build your code if your project, please refer to the EXAMPLE below for guidance.
 
       # - run: |
       #   echo "Run, Build Application using script"
       #   ./location_of_script_within_repo/buildscript.sh
 
       - name: Perform CodeQL Analysis
-        uses: github/codeql-action/analyze@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
+        uses: github/codeql-action/analyze@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
         with:
           category: "/language:${{matrix.language}}"
```

### Comparing `blastpipe-2024.1.2/.github/workflows/dependency-review.yml` & `blastpipe-2024.1.3/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/.github/workflows/ozi.yml` & `blastpipe-2024.1.3/.github/workflows/ozi.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/.github/workflows/scorecards.yml` & `blastpipe-2024.1.3/.github/workflows/scorecards.yml`

 * *Files 10% similar despite different names*

```diff
@@ -67,10 +67,10 @@
         with:
           name: SARIF file
           path: results.sarif
           retention-days: 5
 
       # Upload the results to GitHub's code scanning dashboard.
       - name: "Upload to code-scanning"
-        uses: github/codeql-action/upload-sarif@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
+        uses: github/codeql-action/upload-sarif@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
         with:
           sarif_file: results.sarif
```

### Comparing `blastpipe-2024.1.2/.gitignore` & `blastpipe-2024.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/CHANGELOG.md` & `blastpipe-2024.1.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,38 @@
 # CHANGELOG
 
 
 
+## v2024.1.3 (2024-04-26)
+
+### :arrow_up:
+
+* :arrow_up: Bump github/codeql-action from 3.25.2 to 3.25.3
+
+Bumps [github/codeql-action](https://github.com/github/codeql-action) from 3.25.2 to 3.25.3.
+- [Release notes](https://github.com/github/codeql-action/releases)
+- [Changelog](https://github.com/github/codeql-action/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/github/codeql-action/compare/8f596b4ae3cb3c588a5c46780b86dd53fef16c52...d39d31e687223d841ef683f52467bd88e9b21c14)
+
+---
+updated-dependencies:
+- dependency-name: github/codeql-action
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`9ba3bcb`](https://github.com/OZI-Project/blastpipe/commit/9ba3bcbbafb32db7b5d292fef20f80b9b787209c))
+
+### Other
+
+* Merge pull request #69 from OZI-Project/dependabot/github_actions/github/codeql-action-3.25.3
+
+⬆️ Bump github/codeql-action from 3.25.2 to 3.25.3 ([`a69420e`](https://github.com/OZI-Project/blastpipe/commit/a69420eb4fd8cfb47649fe7be0a9ddea0ddc2b5b))
+
+
 ## v2024.1.2 (2024-04-24)
 
 ### :arrow_up:
 
 * :arrow_up: Bump actions/checkout from 4.1.3 to 4.1.4
 
 Bumps [actions/checkout](https://github.com/actions/checkout) from 4.1.3 to 4.1.4.
```

### Comparing `blastpipe-2024.1.2/LICENSE.txt` & `blastpipe-2024.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/NOTICE.md` & `blastpipe-2024.1.3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/PKG-INFO` & `blastpipe-2024.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.1.2
+Version: 2024.1.3
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.1.2.tar.gz
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.1.3.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `blastpipe-2024.1.2/README.rst` & `blastpipe-2024.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/blastpipe/__init__.py` & `blastpipe-2024.1.3/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/blastpipe/backports.py` & `blastpipe-2024.1.3/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/blastpipe/backports.pyi` & `blastpipe-2024.1.3/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/blastpipe/buffer.py` & `blastpipe-2024.1.3/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/blastpipe/loop.py` & `blastpipe-2024.1.3/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/blastpipe/malloc.py` & `blastpipe-2024.1.3/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/blastpipe/meson.build` & `blastpipe-2024.1.3/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/blastpipe/mixin.py` & `blastpipe-2024.1.3/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/blastpipe/sequence.py` & `blastpipe-2024.1.3/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/blastpipe/tailcall.py` & `blastpipe-2024.1.3/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/meson.build` & `blastpipe-2024.1.3/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/meson.options` & `blastpipe-2024.1.3/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/pyproject.toml` & `blastpipe-2024.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/subprojects/docs/LICENSE.txt` & `blastpipe-2024.1.3/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.1.3/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.1.3/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/subprojects/docs/_static/meson.build` & `blastpipe-2024.1.3/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/subprojects/docs/_templates/layout.html` & `blastpipe-2024.1.3/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/subprojects/docs/_templates/meson.build` & `blastpipe-2024.1.3/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/subprojects/docs/conf.cfg` & `blastpipe-2024.1.3/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/subprojects/docs/index.rst` & `blastpipe-2024.1.3/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/subprojects/docs/meson.build` & `blastpipe-2024.1.3/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/subprojects/docs/meson.options` & `blastpipe-2024.1.3/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/tests/meson.build` & `blastpipe-2024.1.3/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/tests/test_backports.py` & `blastpipe-2024.1.3/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/tests/test_fuzz.py` & `blastpipe-2024.1.3/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.2/tests/test_tailcall.py` & `blastpipe-2024.1.3/tests/test_tailcall.py`

 * *Files identical despite different names*

