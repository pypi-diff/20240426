# Comparing `tmp/osc_transformer_presteps-0.1.0.tar.gz` & `tmp/osc_transformer_presteps-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc_transformer_presteps-0.1.0.tar", last modified: Fri Jan 19 17:32:25 2024, max compression
+gzip compressed data, was "osc_transformer_presteps-0.1.1.tar", last modified: Fri Apr 26 12:34:19 2024, max compression
```

## Comparing `osc_transformer_presteps-0.1.0.tar` & `osc_transformer_presteps-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,28 @@
--rw-r--r--   0        0        0       89 2024-01-16 19:16:59.486723 osc_transformer_presteps-0.1.0/AUTHORS.rst
--rw-r--r--   0        0        0    11357 2024-01-16 19:16:59.487009 osc_transformer_presteps-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1267 2024-01-19 17:25:52.714159 osc_transformer_presteps-0.1.0/README.rst
--rw-r--r--   0        0        0     2932 2024-01-19 17:32:25.297428 osc_transformer_presteps-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      595 2024-01-19 16:46:43.587426 osc_transformer_presteps-0.1.0/src/osc_data_extractor/__init__.py
--rw-r--r--   0        0        0     4289 2024-01-19 16:46:43.587636 osc_transformer_presteps-0.1.0/src/osc_data_extractor/skeleton.py
--rw-r--r--   0        0        0      292 2024-01-19 16:46:43.587790 osc_transformer_presteps-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      606 2024-01-19 16:46:43.587931 osc_transformer_presteps-0.1.0/tests/test_osc_data_extractor.py
--rw-r--r--   0        0        0    15977 1970-01-01 00:00:00.000000 osc_transformer_presteps-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       89 2024-04-26 12:34:00.714644 osc_transformer_presteps-0.1.1/AUTHORS.rst
+-rw-r--r--   0        0        0    11357 2024-04-26 12:34:00.714644 osc_transformer_presteps-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     3922 2024-04-26 12:34:00.714644 osc_transformer_presteps-0.1.1/README.rst
+-rw-r--r--   0        0        0     3234 2024-04-26 12:34:19.182784 osc_transformer_presteps-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      589 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/api/__init__.py
+-rw-r--r--   0        0        0      884 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/api/api.py
+-rw-r--r--   0        0        0     2883 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/api/extract.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/api/temp_storage/.gitkeep
+-rwxr-xr-x   0        0        0      569 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/cli.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/content_extraction/__init__.py
+-rw-r--r--   0        0        0     1412 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/content_extraction/extraction_factory.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/content_extraction/extractors/__init__.py
+-rw-r--r--   0        0        0     4790 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/content_extraction/extractors/base_extractor.py
+-rw-r--r--   0        0        0     6731 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/content_extraction/extractors/pdf_text_extractor.py
+-rw-r--r--   0        0        0      955 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/content_extraction/extractors/utils.py
+-rw-r--r--   0        0        0     5121 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/run_local_extraction.py
+-rw-r--r--   0        0        0      987 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/settings.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/streamlit/__init__.py
+-rw-r--r--   0        0        0     1533 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/streamlit/app.py
+-rw-r--r--   0        0        0      286 2024-04-26 12:34:00.726644 osc_transformer_presteps-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0  1304038 2024-04-26 12:34:00.730644 osc_transformer_presteps-0.1.1/tests/osc_transformer_presteps/content_extraction/extractors/test.pdf
+-rw-r--r--   0        0        0     2952 2024-04-26 12:34:00.734644 osc_transformer_presteps-0.1.1/tests/osc_transformer_presteps/content_extraction/extractors/test_base_extractor.py
+-rw-r--r--   0        0        0    18382 2024-04-26 12:34:00.734644 osc_transformer_presteps-0.1.1/tests/osc_transformer_presteps/content_extraction/extractors/test_data.json
+-rw-r--r--   0        0        0   814394 2024-04-26 12:34:00.738644 osc_transformer_presteps-0.1.1/tests/osc_transformer_presteps/content_extraction/extractors/test_issue.pdf
+-rw-r--r--   0        0        0     1345 2024-04-26 12:34:00.738644 osc_transformer_presteps-0.1.1/tests/osc_transformer_presteps/content_extraction/extractors/test_pdf_extractor.py
+-rw-r--r--   0        0        0      534 2024-04-26 12:34:00.738644 osc_transformer_presteps-0.1.1/tests/osc_transformer_presteps/content_extraction/test_extraction_factory.py
+-rw-r--r--   0        0        0    19088 1970-01-01 00:00:00.000000 osc_transformer_presteps-0.1.1/PKG-INFO
```

### Comparing `osc_transformer_presteps-0.1.0/LICENSE.txt` & `osc_transformer_presteps-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osc_transformer_presteps-0.1.0/pyproject.toml` & `osc_transformer_presteps-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "osc-transformer-presteps"
-version = "0.1.0"
+version = "v0.1.1"
 description = "OS-Climate Data Extraction Tool"
 authors = [
     { name = "David Besslich", email = "90916810+DaBeIDS@users.noreply.github.com" },
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.9, !=3.9.7"
 readme = "README.rst"
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
@@ -20,54 +20,68 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
     "Topic :: Office/Business :: Financial",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development",
 ]
+dependencies = [
+    "pdfminer>=20191125",
+    "pypdf>=4.0.0",
+    "numpy>=1.26.3",
+    "fastapi>=0.109.0",
+    "uvicorn>=0.27.0.post1",
+    "python-multipart>=0.0.6",
+    "streamlit>=1.12.0",
+    "altair<5",
+    "types-requests>=2.31.0.20240218",
+    "pydantic>=2.6.3",
+    "typer>=0.12.3",
+]
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.urls]
 Homepage = "https://github.com/os-climate/osc-transformer-presteps"
 Repository = "https://github.com/os-climate/osc-transformer-presteps"
 Downloads = "https://github.com/os-climate/osc-transformer-presteps/releases"
 "Bug Tracker" = "https://github.com/os-climate/osc-transformer-presteps/issues"
 Documentation = "https://github.com/os-climate/osc-transformer-presteps/tree/main/docs"
 "Source Code" = "https://github.com/os-climate/osc-transformer-presteps"
 
 [project.scripts]
-osc-transformer-presteps = "osc_transformer_presteps.skeleton:run"
+osc-transformer-presteps = "osc_transformer_presteps.cli:run"
 
 [project.optional-dependencies]
 dev = [
     "pylint",
     "toml",
     "yapf",
     "pdm",
 ]
 test = [
-    "pytest",
-    "pytest-cov",
+    "pytest>=8.1.1",
+    "pytest-cov>=5.0.0",
+]
+lint = [
+    "pre-commit>=3.7.0",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [metadata]
 license-files = [
     "LICENSES.txt",
 ]
 
-[tool.setuptools_scm]
-
 [tool.pdm.scripts]
 pre_release = "scripts/dev-versioning.sh"
 release = "scripts/release-versioning.sh"
 test = "pytest"
 tox = "tox"
 lint = "pre-commit run --all-files"
 
@@ -95,22 +109,21 @@
 ]
 dev = [
     "tox>=4.11.3",
     "tox-pdm>=0.7.0",
 ]
 lint = [
     "pre-commit",
-    "pyproject-flake8",
 ]
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests/",
 ]
-addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 95"
+addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 40"
 
 [tool.coverage.run]
 source = [
     "src",
 ]
 
 [tool.yapf]
```

### Comparing `osc_transformer_presteps-0.1.0/src/osc_data_extractor/__init__.py` & `osc_transformer_presteps-0.1.1/src/osc_transformer_presteps/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,13 +4,13 @@
     # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
     from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 else:
     from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
 
 try:
     # Change here if project is renamed and does not equal the package name
-    dist_name = "osc-transformer-presteps"
+    dist_name = "osc-data-extractor"
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
```

### Comparing `osc_transformer_presteps-0.1.0/PKG-INFO` & `osc_transformer_presteps-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc-transformer-presteps
-Version: 0.1.0
+Version: 0.1.1
 Summary: OS-Climate Data Extraction Tool
 Author-Email: David Besslich <90916810+DaBeIDS@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,61 +221,142 @@
 Classifier: Topic :: Software Development
 Project-URL: Homepage, https://github.com/os-climate/osc-transformer-presteps
 Project-URL: Repository, https://github.com/os-climate/osc-transformer-presteps
 Project-URL: Downloads, https://github.com/os-climate/osc-transformer-presteps/releases
 Project-URL: Bug tracker, https://github.com/os-climate/osc-transformer-presteps/issues
 Project-URL: Documentation, https://github.com/os-climate/osc-transformer-presteps/tree/main/docs
 Project-URL: Source code, https://github.com/os-climate/osc-transformer-presteps
-Requires-Python: >=3.9
-Provides-Extra: dev
-Provides-Extra: test
+Requires-Python: !=3.9.7,>=3.9
+Requires-Dist: pdfminer>=20191125
+Requires-Dist: pypdf>=4.0.0
+Requires-Dist: numpy>=1.26.3
+Requires-Dist: fastapi>=0.109.0
+Requires-Dist: uvicorn>=0.27.0.post1
+Requires-Dist: python-multipart>=0.0.6
+Requires-Dist: streamlit>=1.12.0
+Requires-Dist: altair<5
+Requires-Dist: types-requests>=2.31.0.20240218
+Requires-Dist: pydantic>=2.6.3
+Requires-Dist: typer>=0.12.3
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: toml; extra == "dev"
 Requires-Dist: yapf; extra == "dev"
 Requires-Dist: pdm; extra == "dev"
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest>=8.1.1; extra == "test"
+Requires-Dist: pytest-cov>=5.0.0; extra == "test"
+Requires-Dist: pre-commit>=3.7.0; extra == "lint"
+Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: lint
 Description-Content-Type: text/x-rst
 
+=====================================================================
+OSC Data Extractor Pre-Steps
+=====================================================================
+
+|osc-climate-project| |osc-climate-slack| |osc-climate-github| |pypi| |build-status| |pdm| |PyScaffold|
+
+OS-Climate Data Extraction Tool
+===============================
+
+.. _notes:
+
+This code provides you with an api and a streamlit app to which you
+can provide a pdf document and the output will be the text content in a json format.
+In the backend it is using a python module for extracting text from pdfs, which
+might be extended in the future to other file types.
+The json file is needed for later usage in the context of transformer models
+to extract relevant information, but it can also be used independently.
+
+Quick start
+===========
+
+Install via PyPi
+----------------
+
+You can simply install the package via::
+
+    $ pip install osc-transformer-presteps
+
+Afterwards you can use the tooling as a CLI tool by simply typing::
+
+    $ osc-transformer-presteps
+
+We are using typer to have a nice CLI tool here. All details and help will be shown in the CLI
+tool itself and are not described here in more detail.
+
+
+Install via Github Repository
+-----------------------------
+
+For a quick start with the tool install python and clone the repository to your local environment::
+
+    $ git clone https://github.com/os-climate/osc-transformer-presteps
+
+Afterwards update your python to the requirements (possible for example
+via pdm update) and start a local api server via::
 
-.. image:: https://img.shields.io/badge/OS-Climate-blue
+    $ python ./src/run_server.py
+
+**Note**:
+    * We assume that you are located in the cloned repository.
+    * To check if it is running open "http://localhost:8000/liveness" and you should see the
+      message {"message": "OSC Transformer Pre-Steps Server is running."}.
+
+Finally, run the following code to start a streamlit app which opens up the possibility
+to "upload" a file and extract data from pdf to json via this UI. Note that the UI needs
+the running server so you have to open the streamlit and the server in two different
+terminals.::
+
+    $ streamlit run ./src/osc_transformer_presteps/streamlit/app.py
+
+**Note**: Check also docs/demo. There you can
+find local_extraction_demo.py which will start an extraction
+without any API call and then there is post_request_demo.py
+which will send a file to the API (of course you have to start
+server as above first).
+
+Developer Notes
+===============
+
+For adding new dependencies use pdm. First install via pip::
+
+    $ pip install pdm
+
+And then you could add new packages via pdm add. For example numpy via::
+
+    $ pdm add numpy
+
+For running linting tools just to the following::
+
+    $ pip install tox
+    $ tox -e lint
+    $ tox -e test
+
+
+.. |osc-climate-project| image:: https://img.shields.io/badge/OS-Climate-blue
   :alt: An OS-Climate Project
   :target: https://os-climate.org/
 
-.. image:: https://img.shields.io/badge/slack-osclimate-brightgreen.svg?logo=slack
+.. |osc-climate-slack| image:: https://img.shields.io/badge/slack-osclimate-brightgreen.svg?logo=slack
   :alt: Join OS-Climate on Slack
   :target: https://os-climate.slack.com
 
-.. image:: https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white
+.. |osc-climate-github| image:: https://img.shields.io/badge/GitHub-100000?logo=github&logoColor=white
   :alt: Source code on GitHub
-  :target: https://github.com/ModeSevenIndustrialSolutions/osc-transformer-presteps
+  :target: https://github.com/ModeSevenIndustrialSolutions/osc-data-extractor
 
-.. image:: https://img.shields.io/pypi/v/osc-transformer-presteps.svg
+.. |pypi| image:: https://img.shields.io/pypi/v/osc-data-extractor.svg
   :alt: PyPI package
-  :target: https://pypi.org/project/osc-transformer-presteps/
+  :target: https://pypi.org/project/osc-data-extractor/
 
-.. image:: https://api.cirrus-ci.com/github/os-climate/osc-transformer-presteps.svg?branch=main
+.. |build-status| image:: https://api.cirrus-ci.com/github/os-climate/osc-data-extractor.svg?branch=main
   :alt: Built Status
-  :target: https://cirrus-ci.com/github/os-climate/osc-transformer-presteps
+  :target: https://cirrus-ci.com/github/os-climate/osc-data-extractor
 
-.. image:: https://img.shields.io/badge/PDM-Project-purple
+.. |pdm| image:: https://img.shields.io/badge/PDM-Project-purple
   :alt: Built using PDM
   :target: https://pdm-project.org/latest/
 
-.. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
+.. |PyScaffold| image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
   :alt: Project generated with PyScaffold
   :target: https://pyscaffold.org/
-
-
-
-========================
-osc-transformer-presteps
-========================
-
-OS-Climate Data Extraction Tool
-
-.. _notes:
-
-Notes
-=====
-
-Placeholder notes content
```

