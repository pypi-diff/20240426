# Comparing `tmp/copy-spotter-0.1.2.tar.gz` & `tmp/copy-spotter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copy-spotter-0.1.2.tar", last modified: Wed Apr 24 20:13:06 2024, max compression
+gzip compressed data, was "copy-spotter-0.1.3.tar", last modified: Fri Apr 26 17:54:11 2024, max compression
```

## Comparing `copy-spotter-0.1.2.tar` & `copy-spotter-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:06.688352 copy-spotter-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 20:13:06.688352 copy-spotter-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:06.684352 copy-spotter-0.1.2/copy_spotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 20:13:06.000000 copy-spotter-0.1.2/copy_spotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-24 20:13:06.000000 copy-spotter-0.1.2/copy_spotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:13:06.000000 copy-spotter-0.1.2/copy_spotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 20:13:06.000000 copy-spotter-0.1.2/copy_spotter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-24 20:13:06.000000 copy-spotter-0.1.2/copy_spotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 20:13:06.000000 copy-spotter-0.1.2/copy_spotter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:06.684352 copy-spotter-0.1.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/scripts/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/scripts/html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/scripts/processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/scripts/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-24 20:13:06.688352 copy-spotter-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:06.684352 copy-spotter-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:06.688352 copy-spotter-0.1.2/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/tests/scripts/test_html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/tests/scripts/test_html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/tests/scripts/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/tests/scripts/test_processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/tests/scripts/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-24 20:12:51.000000 copy-spotter-0.1.2/tests/scripts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/copy_spotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 17:54:11.000000 copy-spotter-0.1.3/copy_spotter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:11.756621 copy-spotter-0.1.3/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-26 17:53:55.000000 copy-spotter-0.1.3/tests/scripts/test_utils.py
```

### Comparing `copy-spotter-0.1.2/LICENSE` & `copy-spotter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.2/README.md` & `copy-spotter-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,95 @@
+Metadata-Version: 2.1
+Name: copy-spotter
+Version: 0.1.3
+Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
+Home-page: https://github.com/Wazzabeee/copy-spotter
+Author: Clément Delteil
+Author-email: clement45.delteil45@gmail.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: dev
+License-File: LICENSE
+
 # Copy Spotter
+
+![PyPI - Version](https://img.shields.io/pypi/v/copy-spotter) ![PyPI - License](https://img.shields.io/pypi/l/copy-spotter)
+![Python](https://img.shields.io/badge/python-3.11-blue)
+
+
 ![GIF demo](data/img/example.gif)
 
 ## About
-This program will proccess pdf, txt, docx, and txt files that can be found in the given input directory, find similar sentences, calculate similarity percentage, display a similarity table with links to side by side comparison where similar sentences are highlighted.
-
-This project was made part of my internship at the "Human Computer Humans Interacting with Computers at University of Primorska" lab (HICUP Lab).
+This program will process pdf, txt, docx, and txt files that can be found in the given input directory, find similar sentences, calculate similarity percentage, display a similarity table with links to side by side comparison where similar sentences are highlighted.
 
 **Usage**
 ---
 
+```bash
+$ pip install copy-spotter
+$ copy-spotter [-s] [-o] [-h] input_directory
 ```
-Usage: python -m scripts.main.py input_directory [OPTIONS]
+***Positional Arguments:***
+* `input_directory`: Directory that contains one folder per pdf file (see `data/pdf/plagiarism` for example)
+
+***Optional Arguments:***
+* `-s`, `--block-size`: Set minimum number of consecutive and similar words detected. (Default is 2)
+* `-o`, `--out_dir`: Set the output directory for html files. (Default is creating a new directory called results)
+* `-h`, `--help`: Show this message and exit.
 
-  Performs a similarity analysis of all text files available in given input directory.
-  Developed by Clément Delteil -> (Github: Wazzabeee)
+**Examples**
+---
+```bash
+# Analyze documents in 'data/pdf/plagiarism', with default settings
+$ copy-spotter data/pdf/plagiarism
 
-Options:
-  -block_size, -s  Set minimum number of consecutive and similar words detected. (Default is 2)
-  -out_dir, -o     Set the output directory for html files. (Default is creating a new directory)
-  -help, -h        Show this message and exit.
+# Analyze with custom block size and specify output directory
+$ copy-spotter data/pdf/plagiarism -s 5 -o results/output
 ```
 
-**How to use**
+**Development Setup:**
 ---
 
 ```bash
 # Clone this repository
 $ git clone https://github.com/Wazzabeee/copy_spotter
 
 # Go into the repository
 $ cd copy_spotter
 
 # Install requirements
 $ pip install -r requirements.txt
+$ pip install -r requirements_lint.txt
 
-# Run the app
-$ python -m scripts.main.py data/pdf/plagiarism -s 2
-```
-**First run**
----
-On the first run you might get :
-- an ImportError from pdfminer library 
-``` 
-ImportError: cannot import name 'uint_value' from 'pdfminer.pdftypes' (C:/.../pdfminer/pdftypes.py)
-```
-To fix this, please uninstall pdfminer3k and pdfminer.six via 
-``` pip uninstall pdfminer3k ```
-``` pip uninstall pdfminer.six ```
-Then install them again via 
-``` pip install pdfminer3k ```
-``` pip install pdfminer.six ```
-
+# Install precommit
+$ pip install pre-commit
+$ pre-commit install
+
+# Run tests
+$ pip install pytest
+$ pytest tests/
 
-- a TypeError from Slate3k library 
-```
-TypeError __init__() missing 1 required positional arg 'parser' in "C:/.../slate3k/classes.py
+# Run package locally
+$ python -m scripts.main.py [-s] [-o] [-h] input_directory
 ```
-To fix this you'll need to modify `class PDF(list):` in `C:/.../slate3k/classes.py`. In `def __init__()` change both `if PYTHON 3:` <br/> to `if not PYTHON 3:` on lines 58 and 72.
 
 **Recommandations**
 ---
 - Please make sure that all text files are closed before running the program.
 - In order to get the best results please provide text files of the same languages.
 - Pdf files that are made from scanned images won't be processed correctly.
+- Ensure you have writing access when using the package 
 - If a specific file is not processed correctly feel free to [contact me](mailto:<clement45.delteil45@gmail.com>) so that I can address the issue.
 
 **TODO**
 ---
-- Add more tests
+- Add more tests on existing functions
+- Implement OCR with tesseract for scanned documents
 - Add info in console for timing (tqdm)
-- Add CSS to HTML Template
-- Add support for other folder structures
-- Fix Slate3k by installing custom fork
+- Add CSS to HTML Template to make the results better looking
+- Add support for other folder structures (right now the package is expecting one pdf files per folder)
+- Add custom naming option for pdf files
+- Fix Slate3k by installing custom fork (check if still relevant)
```

### Comparing `copy-spotter-0.1.2/copy_spotter.egg-info/SOURCES.txt` & `copy-spotter-0.1.3/copy_spotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.2/scripts/html_utils.py` & `copy-spotter-0.1.3/scripts/html_utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.2/scripts/html_writing.py` & `copy-spotter-0.1.3/scripts/html_writing.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.2/scripts/main.py` & `copy-spotter-0.1.3/scripts/main.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.2/scripts/processing_files.py` & `copy-spotter-0.1.3/scripts/processing_files.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.2/scripts/similarity.py` & `copy-spotter-0.1.3/scripts/similarity.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.2/scripts/utils.py` & `copy-spotter-0.1.3/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.2/setup.py` & `copy-spotter-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.2/tests/scripts/test_utils.py` & `copy-spotter-0.1.3/tests/scripts/test_utils.py`

 * *Files identical despite different names*

