# Comparing `tmp/audplot-1.4.6.tar.gz` & `tmp/audplot-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audplot-1.4.6.tar", last modified: Wed Dec 21 16:02:08 2022, max compression
+gzip compressed data, was "audplot-1.4.7.tar", last modified: Fri Apr 26 07:07:45 2024, max compression
```

## Comparing `audplot-1.4.6.tar` & `audplot-1.4.7.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.764629 audplot-1.4.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.760629 audplot-1.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.760629 audplot-1.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2022-12-21 16:01:47.000000 audplot-1.4.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2022-12-21 16:01:47.000000 audplot-1.4.6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-21 16:01:47.000000 audplot-1.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2022-12-21 16:01:47.000000 audplot-1.4.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2022-12-21 16:01:47.000000 audplot-1.4.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-21 16:01:47.000000 audplot-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2022-12-21 16:02:08.764629 audplot-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2022-12-21 16:01:47.000000 audplot-1.4.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.760629 audplot-1.4.6/audplot/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-21 16:01:47.000000 audplot-1.4.6/audplot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.760629 audplot-1.4.6/audplot/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 16:01:47.000000 audplot-1.4.6/audplot/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25568 2022-12-21 16:01:47.000000 audplot-1.4.6/audplot/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.760629 audplot-1.4.6/audplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2022-12-21 16:02:08.000000 audplot-1.4.6/audplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2022-12-21 16:02:08.000000 audplot-1.4.6/audplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 16:02:08.000000 audplot-1.4.6/audplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-21 16:02:08.000000 audplot-1.4.6/audplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-21 16:02:08.000000 audplot-1.4.6/audplot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.764629 audplot-1.4.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.760629 audplot-1.4.6/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.764629 audplot-1.4.6/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.764629 audplot-1.4.6/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/api-src/audplot.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2022-12-21 16:01:47.000000 audplot-1.4.6/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-21 16:01:47.000000 audplot-1.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2022-12-21 16:02:08.764629 audplot-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-21 16:01:47.000000 audplot-1.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 16:02:08.764629 audplot-1.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-21 16:01:47.000000 audplot-1.4.6/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2022-12-21 16:01:47.000000 audplot-1.4.6/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.069120 audplot-1.4.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.061119 audplot-1.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.065119 audplot-1.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-26 07:07:23.000000 audplot-1.4.7/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-26 07:07:23.000000 audplot-1.4.7/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-26 07:07:23.000000 audplot-1.4.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-26 07:07:23.000000 audplot-1.4.7/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 07:07:23.000000 audplot-1.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-26 07:07:23.000000 audplot-1.4.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-26 07:07:23.000000 audplot-1.4.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-26 07:07:23.000000 audplot-1.4.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-26 07:07:23.000000 audplot-1.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-26 07:07:45.069120 audplot-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-26 07:07:23.000000 audplot-1.4.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.065119 audplot-1.4.7/audplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-26 07:07:23.000000 audplot-1.4.7/audplot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.065119 audplot-1.4.7/audplot/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:23.000000 audplot-1.4.7/audplot/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25873 2024-04-26 07:07:23.000000 audplot-1.4.7/audplot/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.069120 audplot-1.4.7/audplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-26 07:07:45.000000 audplot-1.4.7/audplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-26 07:07:45.000000 audplot-1.4.7/audplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:07:45.000000 audplot-1.4.7/audplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 07:07:45.000000 audplot-1.4.7/audplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 07:07:45.000000 audplot-1.4.7/audplot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.069120 audplot-1.4.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.061119 audplot-1.4.7/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.069120 audplot-1.4.7/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.069120 audplot-1.4.7/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/api-src/audplot.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-26 07:07:23.000000 audplot-1.4.7/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-26 07:07:23.000000 audplot-1.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 07:07:23.000000 audplot-1.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 07:07:45.069120 audplot-1.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:07:45.069120 audplot-1.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 07:07:23.000000 audplot-1.4.7/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-26 07:07:23.000000 audplot-1.4.7/tests/test_api.py
```

### Comparing `audplot-1.4.6/.github/workflows/publish.yml` & `audplot-1.4.7/.github/workflows/publish.yml`

 * *Files 15% similar despite different names*

```diff
@@ -4,44 +4,49 @@
   push:
     tags:
       - 'v*' # Push events to matching v*, i.e. v1.0, v20.15.10
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      contents: write
+      id-token: write
+    concurrency:
+      group: ${{ github.workflow }}-${{ github.ref }}
+
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 2
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
-        python-version: '3.8'
+        python-version: '3.10'
 
     - name: Setup Ubuntu
       run: |
         sudo apt-get update
         sudo apt-get -y install libsndfile1
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install setuptools wheel twine
+        pip install build twine virtualenv
 
     # PyPI package
-    - name: Build and publish
-      env:
-        TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
-        TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-      run: |
-        python setup.py sdist bdist_wheel
-        python -m twine upload dist/*
+    - name: Build Python package
+      run: python -m build
 
-    # Docuemntation
+    - name: Publish Python package to PyPI
+      uses: pypa/gh-action-pypi-publish@release/v1
+
+    # Documentation
     - name: Install doc dependencies
       run: |
         pip install -r requirements.txt
         pip install -r docs/requirements.txt
 
     - name: Build documentation
       run: |
@@ -55,24 +60,25 @@
 
     # Github release
     - name: Read CHANGELOG
       id: changelog
       run: |
         # Get bullet points from last CHANGELOG entry
         CHANGELOG=$(git diff -U0 HEAD^ HEAD | grep '^[+][\* ]' | sed 's/\+//')
-        # Support for multiline, see
-        # https://github.com/actions/create-release/pull/11#issuecomment-640071918
-        CHANGELOG="${CHANGELOG//'%'/'%25'}"
-        CHANGELOG="${CHANGELOG//$'\n'/'%0A'}"
-        CHANGELOG="${CHANGELOG//$'\r'/'%0D'}"
         echo "Got changelog: $CHANGELOG"
-        echo "::set-output name=body::$CHANGELOG"
+        # Support for multiline, see
+        # https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#multiline-strings
+        {
+          echo 'body<<EOF'
+          echo "$CHANGELOG"
+          echo EOF
+        } >> "$GITHUB_OUTPUT"
 
     - name: Create release on Github
       id: create_release
-      uses: softprops/action-gh-release@v1
+      uses: softprops/action-gh-release@v2
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag_name: ${{ github.ref }}
         name: Release ${{ github.ref_name }}
         body: ${{ steps.changelog.outputs.body }}
```

### Comparing `audplot-1.4.6/.github/workflows/test.yml` & `audplot-1.4.7/.github/workflows/test.yml`

 * *Files 23% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-latest, windows-latest, macos-latest ]
-        python-version: [ '3.7', '3.8', '3.9', '3.10' ]
+        python-version: [ '3.8', '3.9', '3.10', '3.11', '3.12' ]
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Setup Ubuntu
       run: |
         sudo apt-get update
         sudo apt-get -y install libsndfile1
       if: matrix.os == 'ubuntu-latest'
@@ -32,17 +32,12 @@
         pip install -r requirements.txt
         pip install -r docs/requirements.txt
         pip install -r tests/requirements.txt
     - name: Test with pytest
       run: |
         python -m pytest
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
       if: matrix.os == 'ubuntu-latest'
-    - name: Test building documentation
-      run: |
-        python -m sphinx docs/ docs/_build/ -b html -W
-        python -m sphinx docs/ docs/_build/ -b linkcheck -W
-      if: matrix.os == 'ubuntu-latest'
```

### Comparing `audplot-1.4.6/CHANGELOG.rst` & `audplot-1.4.7/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,29 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.4.7 (2024-04-26)
+--------------------------
+
+* Added: support for Python 3.11
+* Added: support for Python 3.12
+* Fixed: avoid ``pandas`` future warning
+  for ``pandas.DataFrame.applymap()``
+* Fixed: avoid deprecation warning
+  by replacing
+  ``pkg_resources``
+  internally with
+  ``importlib.metadata``
+* Removed: support for Python 3.7
+
+
 Version 1.4.6 (2022-12-21)
 --------------------------
 
 * Changed: split API documentation into sub-pages
   for each function
```

### Comparing `audplot-1.4.6/CONTRIBUTING.rst` & `audplot-1.4.7/CONTRIBUTING.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,122 @@
 Contributing
 ============
 
 Everyone is invited to contribute to this project.
 Feel free to create a `pull request`_ .
-If you find errors, omissions, inconsistencies or other things
-that need improvement, please create an issue_.
+If you find errors,
+omissions,
+inconsistencies,
+or other things
+that need improvement,
+please create an issue_.
 
 .. _issue: https://github.com/audeering/audplot/issues/new/
 .. _pull request: https://github.com/audeering/audplot/compare/
 
 
 Development Installation
 ------------------------
 
-Instead of pip-installing the latest release from PyPI,
+Instead of pip-installing the latest release from PyPI_,
 you should get the newest development version from Github_::
 
-    git clone https://github.com/audeering/audplot/
-    cd audplot
-    # Create virutal environment for this project
-    # e.g.
-    # virtualenv --python="python3"  $HOME/.envs/audplot
-    # source $HOME/.envs/audplot/bin/activate
-    pip install -r requirements.txt
+   git clone https://github.com/audeering/audplot/
+   cd audplot
+   # Create virtual environment for this project
+   # e.g.
+   # virtualenv --python="python3"  $HOME/.envs/audplot
+   # source $HOME/.envs/audplot/bin/activate
+   pip install -r requirements.txt
 
-.. _Github: https://github.com/audeering/audplot
 
-This way, your installation always stays up-to-date,
+This way,
+your installation always stays up-to-date,
 even if you pull new changes from the Github repository.
 
+.. _PyPI: https://pypi.org/project/audplot/
+.. _Github: https://github.com/audeering/audplot/
+
+
+Coding Convention
+-----------------
+
+We follow the PEP8_ convention for Python code
+and use ruff_ as a linter and code formatter.
+In addition,
+we check for common spelling errors with codespell_.
+Both tools and possible exceptions
+are defined in :file:`pyproject.toml`.
+
+The checks are executed in the CI using `pre-commit`_.
+You can enable those checks locally by executing::
+
+    pip install pre-commit  # consider system wide installation
+    pre-commit install
+    pre-commit run --all-files
+
+Afterwards ruff_ and codespell_ are executed
+every time you create a commit.
+
+You can also install ruff_ and codespell_
+and call it directly::
+
+    pip install ruff codespell  # consider system wide installation
+    ruff check --fix .  # lint all Python files, and fix any fixable errors
+    ruff format .  # format code of all Python files
+    codespell
+
+It can be restricted to specific folders::
+
+    ruff check audplot/ tests/
+    codespell audplot/ tests/
+
+
+.. _codespell: https://github.com/codespell-project/codespell/
+.. _PEP8: http://www.python.org/dev/peps/pep-0008/
+.. _pre-commit: https://pre-commit.com
+.. _ruff: https://beta.ruff.rs
+
 
 Building the Documentation
 --------------------------
 
 If you make changes to the documentation,
 you can re-create the HTML pages using Sphinx_.
 You can install it and a few other necessary packages with::
 
-    pip install -r requirements.txt
-    pip install -r docs/requirements.txt
+   pip install -r docs/requirements.txt
 
 To create the HTML pages, use::
 
-	python -m sphinx docs/ build/sphinx/html -b html
+   python -m sphinx docs/ build/sphinx/html -b html
 
 The generated files will be available
 in the directory :file:`build/sphinx/html/`.
 
 It is also possible to automatically check if all links are still valid::
 
-    python -m sphinx docs/ build/sphinx/linkcheck -b linkcheck
+   python -m sphinx docs/ build/sphinx/html -b linkcheck
 
-.. _Sphinx: http://sphinx-doc.org/
+.. _Sphinx: http://sphinx-doc.org
 
 
 Running the Tests
 -----------------
 
 You'll need pytest_ for that.
 It can be installed with::
 
-    pip install -r tests/requirements.txt
+   pip install -r tests/requirements.txt
 
 To execute the tests, simply run::
 
-    python -m pytest
+   python -m pytest
 
-.. _pytest: https://pytest.org/
+.. _pytest: https://pytest.org
 
 
 Creating a New Release
 ----------------------
 
 New releases are made using the following steps:
```

### Comparing `audplot-1.4.6/LICENSE` & `audplot-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `audplot-1.4.6/README.rst` & `audplot-1.4.7/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 and machine learning problems (e.g. confusion matrix).
 
 
 .. badges images and links:
 .. |tests| image:: https://github.com/audeering/audplot/workflows/Test/badge.svg
     :target: https://github.com/audeering/audplot/actions?query=workflow%3ATest
     :alt: Test status
-.. |coverage| image:: https://codecov.io/gh/audeering/audplot/branch/master/graph/badge.svg?token=t5c5Ky64Ch
+.. |coverage| image:: https://codecov.io/gh/audeering/audplot/branch/main/graph/badge.svg?token=t5c5Ky64Ch
     :target: https://codecov.io/gh/audeering/audplot/
     :alt: code coverage
 .. |docs| image:: https://img.shields.io/pypi/v/audplot?label=docs
     :target: https://audeering.github.io/audplot/
     :alt: audplot's documentation
 .. |license| image:: https://img.shields.io/badge/license-MIT-green.svg
-    :target: https://github.com/audeering/audplot/blob/master/LICENSE
+    :target: https://github.com/audeering/audplot/blob/main/LICENSE
     :alt: audplot's MIT license
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/audplot.svg
     :target: https://pypi.org/project/audplot/
     :alt: audplot's supported Python versions
```

### Comparing `audplot-1.4.6/audplot/core/api.py` & `audplot-1.4.7/audplot/core/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import math
 import typing
+import warnings
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
+
 # The scipy implementation is faster,
 # but scipy is not an official dependency of audplot
 try:
     from scipy.special import ndtri as inverse_normal_distribution
 except ModuleNotFoundError:  # pragma: nocover
     from audmath import inverse_normal_distribution
 
 import audmetric
 
 
 def cepstrum(
-        cc_matrix: np.ndarray,
-        hop_duration: float,
-        *,
-        channel: int = 0,
-        ax: matplotlib.axes._axes.Axes = None,
-        cmap: str = 'magma',
+    cc_matrix: np.ndarray,
+    hop_duration: float,
+    *,
+    channel: int = 0,
+    ax: matplotlib.axes._axes.Axes = None,
+    cmap: str = "magma",
 ) -> matplotlib.image.AxesImage:
     r"""Cepstrum.
 
     Args:
         cc_matrix: cepstral coefficients matrix with magnitude values
         hop_duration: hop duration in seconds
         channel: channel index
@@ -46,39 +48,38 @@
             from audplot import cepstrum
 
         .. plot::
             :context: close-figs
 
             >>> import librosa
             >>> import matplotlib.pyplot as plt
-            >>> x, sr = librosa.load(librosa.ex('trumpet'))
+            >>> x, sr = librosa.load(librosa.ex("trumpet"))
             >>> y = librosa.feature.mfcc(y=x, sr=sr)
             >>> hop_dur = 512 / sr  # default hop length is 512
             >>> image = cepstrum(y, hop_dur)
             >>> cb = plt.colorbar(image)
             >>> cb.outline.set_visible(False)
             >>> plt.tight_layout()
 
     """
-
     ax = ax or plt.gca()
     cc_matrix = cc_matrix[channel] if cc_matrix.ndim == 3 else cc_matrix
 
     n_cc, n_cepstra = cc_matrix.shape
     extent = [0, n_cepstra * hop_duration, -0.5, n_cc - 0.5]
-    ax.set_ylabel('Cepstral Coefficients')
-    ax.set_xlabel('Time / s')
+    ax.set_ylabel("Cepstral Coefficients")
+    ax.set_xlabel("Time / s")
 
     ax.margins(x=0)
     image = ax.imshow(
         cc_matrix,
-        aspect='auto',
-        origin='lower',
+        aspect="auto",
+        origin="lower",
         cmap=cmap,
-        interpolation='none',
+        interpolation="none",
         extent=extent,
     )
 
     # Adjust yticks to be located at real cepstral coefficient steps
     locs = ax.get_yticks()
     yticks_spacing = int(np.round(n_cc / len(locs)))
     locs = list(range(0, n_cc - 1, yticks_spacing))
@@ -87,22 +88,22 @@
     # Remove axis lines
     sns.despine(ax=ax, left=True, bottom=True)
 
     return image
 
 
 def confusion_matrix(
-        truth: typing.Union[typing.Sequence, pd.Series],
-        prediction: typing.Union[typing.Sequence, pd.Series],
-        *,
-        labels: typing.Sequence = None,
-        label_aliases: typing.Dict = None,
-        percentage: bool = False,
-        show_both: bool = False,
-        ax: matplotlib.axes.Axes = None,
+    truth: typing.Union[typing.Sequence, pd.Series],
+    prediction: typing.Union[typing.Sequence, pd.Series],
+    *,
+    labels: typing.Sequence = None,
+    label_aliases: typing.Dict = None,
+    percentage: bool = False,
+    show_both: bool = False,
+    ax: matplotlib.axes.Axes = None,
 ):
     r"""Confusion matrix between ground truth and prediction.
 
     The confusion matrix is calculated by :mod:`audmetric.confusion_matrix`.
 
     Args:
         truth: truth values
@@ -154,90 +155,98 @@
             :context: close-figs
 
             >>> confusion_matrix(truth, prediction, labels=[0, 1, 2, 3])
 
         .. plot::
             :context: close-figs
 
-            >>> confusion_matrix(truth, prediction, label_aliases={0: 'A', 1: 'B', 2: 'C'})
+            >>> confusion_matrix(truth, prediction, label_aliases={0: "A", 1: "B", 2: "C"})
 
-    """  # noqa: 501
+    """  # noqa: E501
     ax = ax or plt.gca()
     if labels is None:
         labels = audmetric.utils.infer_labels(truth, prediction)
 
     cm = audmetric.confusion_matrix(
         truth,
         prediction,
         labels=labels,
         normalize=percentage,
     )
     cm = pd.DataFrame(cm, index=labels)
 
     # Set format of first row labels in confusion matrix
-    if percentage:
-        annot = cm.applymap(lambda x: f'{100 * x:.0f}%')
-    else:
-        annot = cm.applymap(lambda x: human_format(x))
+    with warnings.catch_warnings():
+        # Catch warning,
+        # to still support older pandas versions.
+        # See https://github.com/audeering/audplot/pull/69
+        warnings.simplefilter(action="ignore", category=FutureWarning)
+        if percentage:
+            annot = cm.applymap(lambda x: f"{100 * x:.0f}%")
+        else:
+            annot = cm.applymap(lambda x: human_format(x))
 
     # Add a second row of annotations if requested
     if show_both:
         cm2 = audmetric.confusion_matrix(
             truth,
             prediction,
             labels=labels,
             normalize=not percentage,
         )
         cm2 = pd.DataFrame(cm2, index=labels)
-        if percentage:
-            annot2 = cm2.applymap(lambda x: human_format(x))
-        else:
-            annot2 = cm2.applymap(lambda x: f'{100 * x:.0f}%')
+
+        with warnings.catch_warnings():
+            # Catch warning,
+            # to still support older pandas versions.
+            # See https://github.com/audeering/audplot/pull/69
+            warnings.simplefilter(action="ignore", category=FutureWarning)
+            if percentage:
+                annot2 = cm2.applymap(lambda x: human_format(x))
+            else:
+                annot2 = cm2.applymap(lambda x: f"{100 * x:.0f}%")
 
         # Combine strings from two dataframes
         # by vectorizing the underlying function.
         # See: https://stackoverflow.com/a/42277839
 
         def combine_string(x, y):
-            return f'{x}\n({y})'
+            return f"{x}\n({y})"
 
         combine_string = np.vectorize(combine_string)
         annot = pd.DataFrame(combine_string(annot, annot2), index=labels)
 
     # Get label names to present on x- and y-axis
     if label_aliases is not None:
-        labels = [
-            label_aliases.get(label, label)
-            for label in labels
-        ]
+        labels = [label_aliases.get(label, label) for label in labels]
 
     sns.heatmap(
         cm,
         annot=annot,
         xticklabels=labels,
         yticklabels=labels,
         cbar=False,
-        fmt='',
-        cmap='Blues',
+        fmt="",
+        cmap="Blues",
         ax=ax,
     )
-    ax.tick_params(axis='y', rotation=0)
-    ax.set_xlabel('Prediction')
-    ax.set_ylabel('Truth')
+    ax.tick_params(axis="y", rotation=0)
+    ax.set_xlabel("Prediction")
+    ax.set_ylabel("Truth")
 
 
 def detection_error_tradeoff(
-        x: typing.Union[typing.Sequence, pd.Series],
-        y: typing.Union[typing.Sequence, pd.Series],
-        *,
-        error_rates: bool = False,
-        xlim: typing.Sequence = [0.001, 0.5],
-        ylim: typing.Sequence = [0.001, 0.5],
-        label: str = None,
-        ax: matplotlib.axes.Axes = None,
+    x: typing.Union[typing.Sequence, pd.Series],
+    y: typing.Union[typing.Sequence, pd.Series],
+    *,
+    error_rates: bool = False,
+    xlim: typing.Sequence = [0.001, 0.5],
+    ylim: typing.Sequence = [0.001, 0.5],
+    label: str = None,
+    ax: matplotlib.axes.Axes = None,
 ) -> typing.Callable:
     r"""Detection error tradeoff curve.
 
     A `detection error tradeoff (DET)`_ curve
     is a graphical plot of error rates for binary classification systems,
     plotting the false non-match rate (FNMR)
     against the false match rate (FMR).
@@ -294,29 +303,31 @@
         .. plot::
             :context: close-figs
 
             >>> truth = np.array([1] * 1000 + [0] * 1000)
             >>> # Random prediction
             >>> pred1 = np.random.random_sample(2000)
             >>> # Better than random prediction
-            >>> pred2 = np.zeros(2000,)
+            >>> pred2 = np.zeros(
+            ...     2000,
+            ... )
             >>> pred2[:1000] = np.random.normal(loc=0.6, scale=0.1, size=1000)
             >>> pred2[1000:] = np.random.normal(loc=0.4, scale=0.1, size=1000)
             >>> pred2 = np.clip(pred2, 0, 1)
             >>> transform = detection_error_tradeoff(
             ...     truth,
             ...     pred1,
             ...     xlim=[0.01, 0.99],  # use large limits for random
             ...     ylim=[0.01, 0.99],
-            ...     label='pred1',
+            ...     label="pred1",
             ... )
             >>> # Add pred2 to plot using transformed FMR and FNMR values
             >>> import audmetric
             >>> fmr, fnmr, _ = audmetric.detection_error_tradeoff(truth, pred2)
-            >>> _ = plt.plot(transform(fmr), transform(fnmr), label='pred2')
+            >>> _ = plt.plot(transform(fmr), transform(fnmr), label="pred2")
             >>> _ = plt.legend()
             >>> plt.tight_layout()
 
     """  # noqa: E501
     ax = ax or plt.gca()
 
     if not error_rates:
@@ -326,40 +337,37 @@
     transform = inverse_normal_distribution
 
     g = sns.lineplot(
         x=transform(x),
         y=transform(y),
         label=label,
     )
-    ax.set_title('Detection Error Tradeoff (DET) Curve')
-    ax.set_xlabel('False Match Rate')
-    ax.set_ylabel('False Non-Match Rate')
+    ax.set_title("Detection Error Tradeoff (DET) Curve")
+    ax.set_xlabel("False Match Rate")
+    ax.set_ylabel("False Non-Match Rate")
     ax.grid(alpha=0.4)
 
     ticks = [0.001, 0.01, 0.05, 0.2, 0.4, 0.6, 0.8, 0.95, 0.99]
     tick_locations = transform(ticks)
-    tick_labels = [
-        f'{t:.0%}' if (100 * t).is_integer() else f'{t:.1%}'
-        for t in ticks
-    ]
+    tick_labels = [f"{t:.0%}" if (100 * t).is_integer() else f"{t:.1%}" for t in ticks]
     g.set(xticks=tick_locations, xticklabels=tick_labels)
     g.set(yticks=tick_locations, yticklabels=tick_labels)
     ax.set_xlim(transform(xlim[0]), transform(xlim[1]))
     ax.set_ylim(transform(ylim[0]), transform(ylim[1]))
 
     sns.despine(ax=ax)
 
     return transform
 
 
 def distribution(
-        truth: typing.Union[typing.Sequence, pd.Series],
-        prediction: typing.Union[typing.Sequence, pd.Series],
-        *,
-        ax: matplotlib.axes.Axes = None,
+    truth: typing.Union[typing.Sequence, pd.Series],
+    prediction: typing.Union[typing.Sequence, pd.Series],
+    *,
+    ax: matplotlib.axes.Axes = None,
 ):
     r"""Distribution of truth and predicted values.
 
     Args:
         truth: truth values
         prediction: predicted values
         ax: pre-existing axes for the plot.
@@ -381,33 +389,33 @@
             >>> prediction = np.random.normal(loc=0.05, scale=0.5, size=1000)
             >>> distribution(truth, prediction)
 
     """
     ax = ax or plt.gca()
     data = pd.DataFrame(
         data=np.array([truth, prediction]).T,
-        columns=['Truth', 'Prediction'],
+        columns=["Truth", "Prediction"],
     )
     sns.histplot(
         data,
         common_bins=False,
-        stat='frequency',
+        stat="frequency",
         kde=True,
         edgecolor=None,
-        kde_kws={'cut': 3},  # hard code like in distplot()
+        kde_kws={"cut": 3},  # hard code like in distplot()
         ax=ax,
     )
     ax.grid(alpha=0.4)
     sns.despine(ax=ax)
     # Force y ticks at integer locations
     ax.yaxis.set_major_locator(matplotlib.ticker.MaxNLocator(integer=True))
 
 
 def human_format(
-        number: typing.Union[int, float],
+    number: typing.Union[int, float],
 ) -> str:
     r"""Display large or small numbers in a human readable way.
 
     It replaces large or small numbers
     by no more than 3 significant digits
     and no more than 1 fractional digit.
     Instead it adds a string indicating the base,
@@ -453,56 +461,56 @@
         '123u'
         >>> human_format(0)
         '0'
         >>> human_format(-1000)
         '-1k'
 
     """
-    sign = ''
+    sign = ""
     if number == 0:
-        return '0'
+        return "0"
     if number < 0:
-        sign = '-'
+        sign = "-"
         number = -1 * number
     units = [
-        'n',  # 10^-9  nano
-        'u',  # 10^-6  micro
-        'm',  # 10^-3  milli
-        '',   # 0
-        'k',  # 10^3   thousand
-        'M',  # 10^6   Million      Mega
-        'B',  # 10^9   Billion      Giga
-        'T',  # 10^12  Trillion     Tera
-        'P',  # 10^15  Quadrillion  Peta
-        'E',  # 10^18  Quintillion  Exa
-        'Z',  # 10^21  Sextillion   Zetta
-        'Y',  # 10^24  Septillion   Yotta
+        "n",  # 10^-9  nano
+        "u",  # 10^-6  micro
+        "m",  # 10^-3  milli
+        "",  # 0
+        "k",  # 10^3   thousand
+        "M",  # 10^6   Million      Mega
+        "B",  # 10^9   Billion      Giga
+        "T",  # 10^12  Trillion     Tera
+        "P",  # 10^15  Quadrillion  Peta
+        "E",  # 10^18  Quintillion  Exa
+        "Z",  # 10^21  Sextillion   Zetta
+        "Y",  # 10^24  Septillion   Yotta
     ]
     k = 1000.0
     magnitude = int(math.floor(math.log(number, k)))
-    number = f'{number / k**magnitude:.1f}'
+    number = f"{number / k**magnitude:.1f}"
     if magnitude >= 9:
-        raise ValueError('Only magnitudes < 1000 ** 9 are supported.')
+        raise ValueError("Only magnitudes < 1000 ** 9 are supported.")
     if magnitude <= -4:
-        raise ValueError('Only magnitudes > 1000 ** -4 are supported.')
+        raise ValueError("Only magnitudes > 1000 ** -4 are supported.")
     # Make sure we show only up to 3 significant digits
     if len(number) > 4:
         number = number[:-2]
-    if number.endswith('.0'):
+    if number.endswith(".0"):
         number = number[:-2]
-    return f'{sign}{number}{units[magnitude + 3]}'
+    return f"{sign}{number}{units[magnitude + 3]}"
 
 
 def scatter(
-        truth: typing.Union[typing.Sequence, pd.Series],
-        prediction: typing.Union[typing.Sequence, pd.Series],
-        *,
-        fit: bool = False,
-        order: int = 1,
-        ax: matplotlib.axes.Axes = None,
+    truth: typing.Union[typing.Sequence, pd.Series],
+    prediction: typing.Union[typing.Sequence, pd.Series],
+    *,
+    fit: bool = False,
+    order: int = 1,
+    ax: matplotlib.axes.Axes = None,
 ):
     r"""Scatter plot of truth and predicted values.
 
     Args:
         truth: truth values
         prediction: predicted values
         fit: if ``True``,
@@ -528,30 +536,30 @@
 
     """
     ax = ax or plt.gca()
     sns.regplot(
         x=truth,
         y=prediction,
         fit_reg=fit,
-        line_kws={'color': 'r'},
+        line_kws={"color": "r"},
         order=order,
         ax=ax,
         seed=0,
     )
-    ax.set_xlabel('Truth')
-    ax.set_ylabel('Prediction')
+    ax.set_xlabel("Truth")
+    ax.set_ylabel("Prediction")
     ax.grid(alpha=0.4)
     sns.despine(ax=ax)
 
 
 def series(
-        truth: typing.Union[typing.Sequence, pd.Series],
-        prediction: typing.Union[typing.Sequence, pd.Series],
-        *,
-        ax: matplotlib.axes.Axes = None,
+    truth: typing.Union[typing.Sequence, pd.Series],
+    prediction: typing.Union[typing.Sequence, pd.Series],
+    *,
+    ax: matplotlib.axes.Axes = None,
 ):
     r"""Time series plot of truth and predicted values.
 
     Args:
         truth: truth values
         prediction: predicted values
         ax: pre-existing axes for the plot.
@@ -574,25 +582,25 @@
     """
     ax = ax or plt.gca()
     minimum = min([min(truth), min(prediction)])
     maximum = max([max(truth), max(prediction)])
     ax.plot(truth)
     ax.plot(prediction)
     ax.set_ylim(minimum, maximum)
-    ax.legend(['Truth', 'Prediction'])
+    ax.legend(["Truth", "Prediction"])
     ax.grid(alpha=0.4)
     sns.despine(ax=ax)
 
 
 def signal(
-        x: np.ndarray,
-        sampling_rate: float,
-        *,
-        channel: int = 0,
-        ax: plt.Axes = None,
+    x: np.ndarray,
+    sampling_rate: float,
+    *,
+    channel: int = 0,
+    ax: plt.Axes = None,
 ):
     r"""Time signal.
 
     Args:
         x: array with signal values
         sampling_rate: sampling rate in Hz
         channel: channel index
@@ -606,38 +614,38 @@
 
             from audplot import signal
 
         .. plot::
             :context: close-figs
 
             >>> import librosa
-            >>> x, sr = librosa.load(librosa.ex('trumpet'))
+            >>> x, sr = librosa.load(librosa.ex("trumpet"))
             >>> signal(x, sr)
 
     """
     ax = ax or plt.gca()
     x = x[channel] if x.ndim == 2 else x
 
     time = np.arange(len(x)) / sampling_rate
-    ax.set_xlabel('Time / s')
+    ax.set_xlabel("Time / s")
 
     ax.margins(x=0)
     ax.plot(time, x)
     ax.grid(alpha=0.4)
     sns.despine(ax=ax)
 
 
 def spectrum(
-        magnitude: np.ndarray,
-        hop_duration: float,
-        centers: np.ndarray,
-        *,
-        channel: int = 0,
-        cmap: str = 'magma',
-        ax: matplotlib.axes.Axes = None,
+    magnitude: np.ndarray,
+    hop_duration: float,
+    centers: np.ndarray,
+    *,
+    channel: int = 0,
+    cmap: str = "magma",
+    ax: matplotlib.axes.Axes = None,
 ) -> matplotlib.image.AxesImage:
     r"""Plot spectrum.
 
     Args:
         magnitude: matrix with magnitude values
         hop_duration: hop duration in seconds
         centers: array with center frequencies
@@ -658,40 +666,40 @@
             import numpy as np
 
         .. plot::
             :context: close-figs
 
             >>> import librosa
             >>> import matplotlib.pyplot as plt
-            >>> x, sr = librosa.load(librosa.ex('trumpet'))
+            >>> x, sr = librosa.load(librosa.ex("trumpet"))
             >>> y = librosa.feature.melspectrogram(y=x, sr=sr, n_mels=40, fmax=4000)
             >>> y_db = librosa.power_to_db(y, ref=np.max)
             >>> hop_dur = 512 / sr  # default hop length is 512
             >>> centers = librosa.mel_frequencies(n_mels=40, fmax=4000)
             >>> image = spectrum(y_db, hop_dur, centers)
-            >>> cb = plt.colorbar(image, format='%+2.0f dB')
+            >>> cb = plt.colorbar(image, format="%+2.0f dB")
             >>> cb.outline.set_visible(False)
             >>> plt.tight_layout()
 
     """  # noqa: E501
     ax = ax or plt.gca()
     magnitude = magnitude[channel] if magnitude.ndim == 3 else magnitude
 
     frequencies, times = magnitude.shape
     extent = [0, times * hop_duration, -0.5, frequencies - 0.5]
-    ax.set_ylabel('Frequency / Hz')
-    ax.set_xlabel('Time / s')
+    ax.set_ylabel("Frequency / Hz")
+    ax.set_xlabel("Time / s")
 
     ax.margins(x=0)
     image = ax.imshow(
         magnitude,
-        aspect='auto',
-        origin='lower',
+        aspect="auto",
+        origin="lower",
         cmap=cmap,
-        interpolation='none',
+        interpolation="none",
         extent=extent,
     )
 
     # Add center frequencies as yticks labels
     formatter = matplotlib.ticker.FuncFormatter(
         lambda val, pos: round(centers[min(int(val), len(centers) - 1)], 1)
     )
@@ -705,22 +713,22 @@
     # Remove axis lines
     sns.despine(ax=ax, left=True, bottom=True)
 
     return image
 
 
 def waveform(
-        x: np.ndarray,
-        *,
-        text: str = None,
-        color: typing.Union[str, typing.Sequence[float]] = '#E13B41',
-        background: typing.Union[str, typing.Sequence[float]] = '#FFFFFF00',
-        linewidth: float = 1.5,
-        ylim: typing.Sequence[float] = (-1, 1),
-        ax: matplotlib.axes.Axes = None,
+    x: np.ndarray,
+    *,
+    text: str = None,
+    color: typing.Union[str, typing.Sequence[float]] = "#E13B41",
+    background: typing.Union[str, typing.Sequence[float]] = "#FFFFFF00",
+    linewidth: float = 1.5,
+    ylim: typing.Sequence[float] = (-1, 1),
+    ax: matplotlib.axes.Axes = None,
 ):
     r"""Plot waveform of a mono signal.
 
     Shows only the outline of a time signal
     without showing any axis or values.
 
     Args:
@@ -744,65 +752,65 @@
 
             from audplot import waveform
 
         .. plot::
             :context: close-figs
 
             >>> import librosa
-            >>> x, _ = librosa.load(librosa.ex('trumpet'))
-            >>> waveform(x, text='Trumpet')
+            >>> x, _ = librosa.load(librosa.ex("trumpet"))
+            >>> waveform(x, text="Trumpet")
 
         .. plot::
             :context: close-figs
 
             >>> import librosa
-            >>> x, _ = librosa.load(librosa.ex('trumpet'))
-            >>> waveform(x, background='#363636', color='#f6f6f6')
+            >>> x, _ = librosa.load(librosa.ex("trumpet"))
+            >>> waveform(x, background="#363636", color="#f6f6f6")
 
         .. plot::
             :context: close-figs
 
             >>> import librosa
             >>> import matplotlib.pyplot as plt
-            >>> x, _ = librosa.load(librosa.ex('trumpet', hq=True), mono=False)
+            >>> x, _ = librosa.load(librosa.ex("trumpet", hq=True), mono=False)
             >>> _, axs = plt.subplots(2, figsize=(8, 3))
             >>> plt.subplots_adjust(hspace=0)
             >>> waveform(
             ...     x[0, :],
-            ...     text='Left ',  # empty space for same size as 'Right'
+            ...     text="Left ",  # empty space for same size as 'Right'
             ...     linewidth=0.5,
-            ...     background='#389DCD',
-            ...     color='#1B5975',
+            ...     background="#389DCD",
+            ...     color="#1B5975",
             ...     ax=axs[0],
             ... )
             >>> waveform(
             ...     x[1, :],
-            ...     text='Right',
+            ...     text="Right",
             ...     linewidth=0.5,
-            ...     background='#CA5144',
-            ...     color='#742A23',
+            ...     background="#CA5144",
+            ...     color="#742A23",
             ...     ax=axs[1],
             ... )
 
     """
     # Setting the figsize has to be done first
     # before requesting axis or figure.
     # If axis/figure exist already it will have no effect
 
     # Set default figsize if no existing figure is used
-    default_figsize = plt.rcParams['figure.figsize']
-    plt.rcParams['figure.figsize'] = (8, 1)
+    default_figsize = plt.rcParams["figure.figsize"]
+    plt.rcParams["figure.figsize"] = (8, 1)
 
     fig = plt.gcf()
     ax = ax or plt.gca()
 
     x = np.atleast_2d(x)
     channels, samples = x.shape
     if channels > 1:
-        raise RuntimeError('Only mono signals are supported.')
+        raise RuntimeError("Only mono signals are supported.")
     x = x[0]
 
     # Set colors
     ax.grid(False)
     ax.set_facecolor(background)
 
     # Downsample long signals
@@ -845,25 +853,25 @@
     # Add text before waveform
     if text is not None and len(text) > 0:
         space_around_text = 0.02 * samples
         text = ax.text(
             -space_around_text,
             0,
             text,
-            fontsize='large',
-            fontweight='semibold',
+            fontsize="large",
+            fontweight="semibold",
             color=color,
-            horizontalalignment='right',
-            verticalalignment='center',
+            horizontalalignment="right",
+            verticalalignment="center",
         )
         # Get left position of text and adjust xlim accordingly
         fig = ax.get_figure()
         bb = text.get_window_extent(renderer=fig.canvas.get_renderer())
         transform = ax.transData.inverted()
         bb = bb.transformed(transform)
         xlim = (bb.x0 - 1.5 * space_around_text, samples)
     else:
         xlim = (0, samples)
     ax.set(xlim=xlim)
 
     # Restore default figure size
-    plt.rcParams['figure.figsize'] = default_figsize
+    plt.rcParams["figure.figsize"] = default_figsize
```

### Comparing `audplot-1.4.6/audplot.egg-info/SOURCES.txt` & `audplot-1.4.7/audplot.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 .gitignore
+.pre-commit-config.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 README.rst
+pyproject.toml
 requirements.txt
-setup.cfg
-setup.py
+.github/workflows/doc.yml
+.github/workflows/linter.yml
 .github/workflows/publish.yml
 .github/workflows/test.yml
 audplot/__init__.py
 audplot.egg-info/PKG-INFO
 audplot.egg-info/SOURCES.txt
 audplot.egg-info/dependency_links.txt
 audplot.egg-info/requires.txt
```

### Comparing `audplot-1.4.6/docs/_templates/autosummary/class.rst` & `audplot-1.4.7/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audplot-1.4.6/docs/conf.py` & `audplot-1.4.7/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import configparser
 from datetime import date
 import os
 import shutil
 
+import toml
+
 import audeer
 
 
-config = configparser.ConfigParser()
-config.read(os.path.join('..', 'setup.cfg'))
+config = toml.load(audeer.path("..", "pyproject.toml"))
+
 
 # Project -----------------------------------------------------------------
-author = config['metadata']['author']
-copyright = f'2020-{date.today().year} audEERING GmbH'
-project = config['metadata']['name']
+author = ", ".join(author["name"] for author in config["project"]["authors"])
+copyright = f"2020-{date.today().year} audEERING GmbH"
+project = config["project"]["name"]
 version = audeer.git_repo_version()
-title = f'{project} Documentation'
+title = "Documentation"
 
 
 # General -----------------------------------------------------------------
-master_doc = 'index'
-source_suffix = '.rst'
+master_doc = "index"
+source_suffix = ".rst"
 exclude_patterns = [
-    'api-src',
-    'build',
-    'tests',
-    'Thumbs.db',
-    '.DS_Store',
+    "api-src",
+    "build",
+    "tests",
+    "Thumbs.db",
+    ".DS_Store",
 ]
-templates_path = ['_templates']
+templates_path = ["_templates"]
 pygments_style = None
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.napoleon',  # support for Google-style docstrings
-    'sphinx.ext.autosummary',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.intersphinx',
-    'sphinx_autodoc_typehints',
-    'sphinx_copybutton',  # for "copy to clipboard" buttons
-    'sphinxcontrib.katex',  # has to be before jupyter_sphinx
-    'matplotlib.sphinxext.plot_directive',  # include resulting figures in doc
+    "sphinx.ext.autodoc",
+    "sphinx.ext.napoleon",  # support for Google-style docstrings
+    "sphinx.ext.autosummary",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.intersphinx",
+    "sphinx_autodoc_typehints",
+    "sphinx_copybutton",  # for "copy to clipboard" buttons
+    "sphinxcontrib.katex",  # has to be before jupyter_sphinx
+    "matplotlib.sphinxext.plot_directive",  # include resulting figures in doc
 ]
 
 # Do not copy prompot output
-copybutton_prompt_text = r'>>> |\.\.\. '
+copybutton_prompt_text = r">>> |\.\.\. "
 copybutton_prompt_is_regexp = True
 
 # Mapping to external documentation
 intersphinx_mapping = {
-    'audmath': ('https://audeering.github.io/audmath/', None),
-    'audmetric': ('https://audeering.github.io/audmetric/', None),
-    'matplotlib': ('https://matplotlib.org/stable/', None),
-    'numpy': ('https://docs.scipy.org/doc/numpy/', None),
-    'pandas': ('https://pandas.pydata.org/pandas-docs/stable/', None),
-    'python': ('https://docs.python.org/3/', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/', None),
+    "audmath": ("https://audeering.github.io/audmath/", None),
+    "audmetric": ("https://audeering.github.io/audmetric/", None),
+    "matplotlib": ("https://matplotlib.org/stable/", None),
+    "numpy": ("https://docs.scipy.org/doc/numpy/", None),
+    "pandas": ("https://pandas.pydata.org/pandas-docs/stable/", None),
+    "python": ("https://docs.python.org/3/", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/", None),
 }
 
 # Disable Gitlab as we need to sign in
 linkcheck_ignore = [
-    'https://gitlab.audeering.com',
+    "https://gitlab.audeering.com",
 ]
 
 # Plotting
 plot_include_source = True
 plot_html_show_source_link = False
 plot_html_show_formats = False
-plot_pre_code = ''
+plot_pre_code = ""
 plot_rcparams = {
-    'figure.figsize': '5, 3.8',  # inch
+    "figure.figsize": "5, 3.8",  # inch
 }
-plot_formats = ['svg']
+plot_formats = ["svg"]
 
 # Disable auto-generation of TOC entries in the API
 # https://github.com/sphinx-doc/sphinx/issues/6316
 toc_object_entries = False
 
 
 # HTML --------------------------------------------------------------------
-html_theme = 'sphinx_audeering_theme'
+html_theme = "sphinx_audeering_theme"
 html_theme_options = {
-    'display_version': True,
-    'logo_only': False,
-    'footer_links': False,
+    "display_version": True,
+    "logo_only": False,
+    "footer_links": False,
 }
 html_context = {
-    'display_github': True,
+    "display_github": True,
 }
 html_title = title
 
 
 # Copy API (sub-)module RST files to docs/api/ folder ---------------------
-audeer.rmdir('api')
-audeer.mkdir('api')
-api_src_files = audeer.list_file_names('api-src')
+audeer.rmdir("api")
+audeer.mkdir("api")
+api_src_files = audeer.list_file_names("api-src")
 api_dst_files = [
-    audeer.path('api', os.path.basename(src_file))
-    for src_file in api_src_files
+    audeer.path("api", os.path.basename(src_file)) for src_file in api_src_files
 ]
 for src_file, dst_file in zip(api_src_files, api_dst_files):
     shutil.copyfile(src_file, dst_file)
```

### Comparing `audplot-1.4.6/docs/index.rst` & `audplot-1.4.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audplot-1.4.6/docs/usage.rst` & `audplot-1.4.7/docs/usage.rst`

 * *Files 23% similar despite different names*

```diff
@@ -16,20 +16,20 @@
     import audplot
     import matplotlib.pyplot as plt
     import seaborn as sns
 
 
     sns.set()  # get prettier plots
 
-    truth = ['A', 'A', 'A', 'B', 'B', 'B', 'C', 'C', 'C']
-    prediction = ['A', 'A', 'B', 'B', 'C', 'C', 'A', 'A', 'C']
-    label_aliases = {'A': 'c1', 'B': 'c2', 'C': 'c3'}
+    truth = ["A", "A", "A", "B", "B", "B", "C", "C", "C"]
+    prediction = ["A", "A", "B", "B", "C", "C", "A", "A", "C"]
+    label_aliases = {"A": "c1", "B": "c2", "C": "c3"}
 
     plt.figure(figsize=[2.8, 2.5])
-    plt.title('Confusion Matrix')
+    plt.title("Confusion Matrix")
     audplot.confusion_matrix(truth, prediction, label_aliases=label_aliases)
 
     plt.tight_layout()
 
 To show multiple graphs in one figure
 you can specify the axes to draw on.
 
@@ -46,12 +46,12 @@
 
     plot_funcs = [
         audplot.distribution,
         audplot.scatter,
         audplot.series,
     ]
     fig, axs = plt.subplots(1, len(plot_funcs), figsize=[12, 3])
-    plt.suptitle('Multiple plots in one figure')
+    plt.suptitle("Multiple plots in one figure")
     for plot_func, ax in zip(plot_funcs, axs):
         plot_func(truth, prediction, ax=ax)
 
     plt.tight_layout()
```

### Comparing `audplot-1.4.6/tests/test_api.py` & `audplot-1.4.7/tests/test_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,43 +5,43 @@
 import audplot
 
 
 np.random.seed(1)
 
 
 @pytest.mark.parametrize(
-    'number, expected_string',
+    "number, expected_string",
     [
-        (0, '0'),
-        (1, '1'),
-        (10, '10'),
-        (100, '100'),
-        (1000, '1k'),
-        (10000, '10k'),
-        (100000, '100k'),
-        (1000000, '1M'),
-        (0.1, '100m'),
-        (0.01, '10m'),
-        (0.001, '1m'),
-        (0.0015, '1.5m'),
-        (0.0001, '100u'),
-        (-1, '-1'),
-        (-0.001, '-1m'),
-        (-0.0015, '-1.5m'),
+        (0, "0"),
+        (1, "1"),
+        (10, "10"),
+        (100, "100"),
+        (1000, "1k"),
+        (10000, "10k"),
+        (100000, "100k"),
+        (1000000, "1M"),
+        (0.1, "100m"),
+        (0.01, "10m"),
+        (0.001, "1m"),
+        (0.0015, "1.5m"),
+        (0.0001, "100u"),
+        (-1, "-1"),
+        (-0.001, "-1m"),
+        (-0.0015, "-1.5m"),
         pytest.param(
-            1000 ** 9,
-            '',
+            1000**9,
+            "",
             marks=pytest.mark.xfail(raises=ValueError),
         ),
         pytest.param(
-            1000 ** -4,
-            '',
+            1000**-4,
+            "",
             marks=pytest.mark.xfail(raises=ValueError),
         ),
-    ]
+    ],
 )
 def test_human_format(number, expected_string):
     string = audplot.human_format(number)
     assert string == expected_string
 
 
 def test_waveform():
```

