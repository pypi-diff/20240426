# Comparing `tmp/pylegendmeta-0.9.0a1.tar.gz` & `tmp/pylegendmeta-0.9.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylegendmeta-0.9.0a1.tar", last modified: Thu Dec 21 16:25:22 2023, max compression
+gzip compressed data, was "pylegendmeta-0.9.0a2.tar", last modified: Sat Dec 30 15:35:57 2023, max compression
```

## Comparing `pylegendmeta-0.9.0a1.tar` & `pylegendmeta-0.9.0a2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 16:25:22.394183 pylegendmeta-0.9.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2023-12-21 16:25:22.394183 pylegendmeta-0.9.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 16:25:22.394183 pylegendmeta-0.9.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 16:25:22.386183 pylegendmeta-0.9.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 16:25:22.386183 pylegendmeta-0.9.0a1/src/legendmeta/
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-21 16:25:22.000000 pylegendmeta-0.9.0a1/src/legendmeta/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    16666 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/jsondb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/police.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/scdb_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/slowcontrol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 16:25:22.390183 pylegendmeta-0.9.0a1/src/legendmeta/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/templates/bege-detector.json
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/templates/coax-detector.json
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/templates/geds-channel.json
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/templates/icpc-detector.json
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/templates/ppc-detector.json
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/src/legendmeta/templates/spms-channel.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 16:25:22.394183 pylegendmeta-0.9.0a1/src/pylegendmeta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2023-12-21 16:25:22.000000 pylegendmeta-0.9.0a1/src/pylegendmeta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-12-21 16:25:22.000000 pylegendmeta-0.9.0a1/src/pylegendmeta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 16:25:22.000000 pylegendmeta-0.9.0a1/src/pylegendmeta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-21 16:25:22.000000 pylegendmeta-0.9.0a1/src/pylegendmeta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 16:25:22.000000 pylegendmeta-0.9.0a1/src/pylegendmeta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-21 16:25:22.000000 pylegendmeta-0.9.0a1/src/pylegendmeta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-21 16:25:22.000000 pylegendmeta-0.9.0a1/src/pylegendmeta.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 16:25:22.390183 pylegendmeta-0.9.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7526 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/test_jsondb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/test_lmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/test_police.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/test_slowcontroldb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 16:25:22.390183 pylegendmeta-0.9.0a1/tests/testdb/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/testdb/arrays.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 16:25:22.394183 pylegendmeta-0.9.0a1/tests/testdb/dir1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 16:25:22.394183 pylegendmeta-0.9.0a1/tests/testdb/dir1/dir2/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/testdb/dir1/dir2/file4.json
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/testdb/dir1/file3.json
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/testdb/dir1/file5.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/testdb/dir1/validity.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 16:25:22.394183 pylegendmeta-0.9.0a1/tests/testdb/dir2/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/testdb/dir2/file7.json
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/testdb/dir2/file8.json
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/testdb/file1.json
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/testdb/file2.json
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-21 16:25:15.000000 pylegendmeta-0.9.0a1/tests/testdb/file3.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 15:35:57.260479 pylegendmeta-0.9.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2023-12-30 15:35:57.260479 pylegendmeta-0.9.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-30 15:35:57.260479 pylegendmeta-0.9.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 15:35:57.248479 pylegendmeta-0.9.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 15:35:57.252479 pylegendmeta-0.9.0a2/src/legendmeta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-30 15:35:57.000000 pylegendmeta-0.9.0a2/src/legendmeta/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/police.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/scdb_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/slowcontrol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 15:35:57.252479 pylegendmeta-0.9.0a2/src/legendmeta/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/templates/bege-detector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/templates/coax-detector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/templates/geds-channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/templates/icpc-detector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/templates/ppc-detector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/templates/spms-channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19407 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/textdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/src/legendmeta/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 15:35:57.256479 pylegendmeta-0.9.0a2/src/pylegendmeta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2023-12-30 15:35:57.000000 pylegendmeta-0.9.0a2/src/pylegendmeta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2023-12-30 15:35:57.000000 pylegendmeta-0.9.0a2/src/pylegendmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-30 15:35:57.000000 pylegendmeta-0.9.0a2/src/pylegendmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-30 15:35:57.000000 pylegendmeta-0.9.0a2/src/pylegendmeta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-30 15:35:57.000000 pylegendmeta-0.9.0a2/src/pylegendmeta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-30 15:35:57.000000 pylegendmeta-0.9.0a2/src/pylegendmeta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-30 15:35:57.000000 pylegendmeta-0.9.0a2/src/pylegendmeta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 15:35:57.256479 pylegendmeta-0.9.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7841 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/test_jsondb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/test_lmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/test_police.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/test_slowcontroldb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 15:35:57.256479 pylegendmeta-0.9.0a2/tests/testdb/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/testdb/arrays.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 15:35:57.256479 pylegendmeta-0.9.0a2/tests/testdb/dir1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 15:35:57.256479 pylegendmeta-0.9.0a2/tests/testdb/dir1/dir2/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/testdb/dir1/dir2/file4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/testdb/dir1/file3.json
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/testdb/dir1/file5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/testdb/dir1/validity.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 15:35:57.256479 pylegendmeta-0.9.0a2/tests/testdb/dir2/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/testdb/dir2/file7.json
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/testdb/dir2/file8.json
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/testdb/file1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/testdb/file2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-30 15:35:50.000000 pylegendmeta-0.9.0a2/tests/testdb/file3.json
```

### Comparing `pylegendmeta-0.9.0a1/LICENSE` & `pylegendmeta-0.9.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.9.0a1/PKG-INFO` & `pylegendmeta-0.9.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylegendmeta
-Version: 0.9.0a1
+Version: 0.9.0a2
 Summary: Python LEGEND-metadata implementation
 Author-email: Luigi Pertoldi <gipert@pm.me>
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/legend-exp/pylegendmeta
 Project-URL: Bug Tracker, https://github.com/legend-exp/pylegedmeta/issues
 Project-URL: Discussions, https://github.com/legend-exp/pylegedmeta/discussions
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: GitPython
 Requires-Dist: pandas
+Requires-Dist: pyyaml
 Requires-Dist: psycopg2-binary
 Requires-Dist: sqlalchemy>=2
 Provides-Extra: all
 Requires-Dist: pylegendmeta[docs,test]; extra == "all"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
```

### Comparing `pylegendmeta-0.9.0a1/README.md` & `pylegendmeta-0.9.0a2/README.md`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.9.0a1/pyproject.toml` & `pylegendmeta-0.9.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "GitPython",
     "pandas",
+    "pyyaml",
     "psycopg2-binary",
     "sqlalchemy>=2",
 ]
 dynamic = [
     "version",
 ]
```

### Comparing `pylegendmeta-0.9.0a1/src/legendmeta/__init__.py` & `pylegendmeta-0.9.0a2/src/legendmeta/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """A package to access `legend-metadata <https://github.com/legend-exp/legend-metadata>`_ in Python."""
 from __future__ import annotations
 
-from legendmeta._version import version as __version__
-from legendmeta.catalog import to_datetime
-from legendmeta.core import LegendMetadata
-from legendmeta.jsondb import AttrsDict, JsonDB
-from legendmeta.slowcontrol import LegendSlowControlDB
+from ._version import version as __version__
+from .catalog import to_datetime
+from .core import LegendMetadata
+from .slowcontrol import LegendSlowControlDB
+from .textdb import AttrsDict, JsonDB, TextDB
 
 __all__ = [
     "__version__",
     "LegendMetadata",
     "LegendSlowControlDB",
     "JsonDB",
+    "TextDB",
     "AttrsDict",
     "to_datetime",
 ]
```

### Comparing `pylegendmeta-0.9.0a1/src/legendmeta/catalog.py` & `pylegendmeta-0.9.0a2/src/legendmeta/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 import json
 import types
 from collections import namedtuple
 from datetime import datetime
 from pathlib import Path
 from string import Template
 
+from . import utils
+
 
 def to_datetime(value):
     """Convert a LEGEND timestamp (or key) to :class:`datetime.datetime`."""
     return datetime.strptime(value, "%Y%m%dT%H%M%SZ")
 
 
 def unix_time(value):
@@ -130,32 +132,31 @@
 
 class Props:
     @staticmethod
     def read_from(sources, subst_pathvar=False, trim_null=False):
         def read_impl(sources):
             if isinstance(sources, str):
                 file_name = sources
-                with Path(file_name).open() as file:
-                    result = json.load(file)
-                    if subst_pathvar:
-                        Props.subst_vars(
-                            result,
-                            var_values={"_": Path(file_name).parent},
-                            ignore_missing=True,
-                        )
-                    return result
+                result = utils.load_dict(file_name)
+                if subst_pathvar:
+                    Props.subst_vars(
+                        result,
+                        var_values={"_": Path(file_name).parent},
+                        ignore_missing=True,
+                    )
+                return result
 
-            elif isinstance(sources, list):
+            if isinstance(sources, list):
                 result = {}
                 for p in map(read_impl, sources):
                     Props.add_to(result, p)
                 return result
-            else:
-                msg = f"Can't run Props.read_from on sources-value of type {type(sources)}"
-                raise ValueError(msg)
+
+            msg = f"Can't run Props.read_from on sources-value of type {type(sources)}"
+            raise ValueError(msg)
 
         result = read_impl(sources)
         if trim_null:
             Props.trim_null(result)
         return result
 
     @staticmethod
```

### Comparing `pylegendmeta-0.9.0a1/src/legendmeta/core.py` & `pylegendmeta-0.9.0a2/src/legendmeta/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 from datetime import datetime
 from getpass import getuser
 from pathlib import Path
 from tempfile import gettempdir
 
 from git import GitCommandError, InvalidGitRepositoryError, Repo
 
-from .jsondb import AttrsDict, JsonDB
+from .textdb import AttrsDict, TextDB
 
 log = logging.getLogger(__name__)
 
 
-class LegendMetadata(JsonDB):
+class LegendMetadata(TextDB):
     """LEGEND metadata.
 
     Class representing the LEGEND metadata repository with utilities for fast
     access.
 
     Parameters
     ----------
     path
         path to legend-metadata repository. If not existing, will attempt a
         git-clone through SSH. If ``None``, legend-metadata will be cloned
         in a temporary directory (see :func:`tempfile.gettempdir`).
     **kwargs
-        further keyword arguments forwarded to :math:`JsonDB.__init__`.
+        further keyword arguments forwarded to :math:`TextDB.__init__`.
     """
 
     def __init__(self, path: str | None = None, **kwargs) -> None:
         self._default_git_ref = "main"
 
         if isinstance(path, str):
             self._repo_path = path
@@ -117,15 +117,15 @@
         >>> channel.geometry.mass_in_g
         2362.0
         >>> channel.analysis.usability
         'on'
 
         See Also
         --------
-        .jsondb.JsonDB.on
+        .textdb.TextDB.on
         """
         if on is None:
             on = datetime.now()
 
         chmap = self.hardware.configuration.channelmaps.on(
             on, pattern=None, system="all"
         )
```

### Comparing `pylegendmeta-0.9.0a1/src/legendmeta/jsondb.py` & `pylegendmeta-0.9.0a2/src/legendmeta/textdb.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,29 +20,34 @@
 import re
 import sys
 from collections.abc import Iterator
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 
-from legendmeta.catalog import Catalog, Props
+import yaml
+
+from . import utils
+from .catalog import Catalog, Props
 
 log = logging.getLogger(__name__)
 
 
 class AttrsDict(dict):
     """Access dictionary items as attributes.
 
     Examples
     --------
     >>> d = AttrsDict({"key1": {"key2": 1}})
-    >>> d.key1.key2 # == 1
+    >>> d.key1.key2
+    1
     >>> d1 = AttrsDict()
     >>> d1["a"] = 1
-    >>> d1.a # == 1
+    >>> d1.a
+    1
     """
 
     def __init__(self, value: dict | None = None) -> None:
         """Construct an :class:`.AttrsDict` object.
 
         Note
         ----
@@ -191,57 +196,115 @@
             msg = f"could not find '{label}' anywhere in the dictionary"
             raise ValueError(msg)
 
         # cache it
         self.__cached_remaps__[label] = newmap
         return newmap
 
+    def group(self, label: str) -> AttrsDict:
+        """Group dictionary according to a `label`.
+
+        This is equivalent to :meth:`.map` with `unique` set to ``False``.
+
+        Parameters
+        ----------
+        label
+            name (key) at which the new label can be found. If nested in
+            dictionaries, use ``.`` to separate levels, e.g.
+            ``level1.level2.label``.
+
+        Examples
+        --------
+        >>> d = AttrsDict({
+        ...   "a": {
+        ...     "type": "A",
+        ...     "data": 1
+        ...   },
+        ...   "b": {
+        ...     "type": "A",
+        ...     "data": 2
+        ...   },
+        ...   "c": {
+        ...     "type": "B",
+        ...     "data": 3
+        ...   },
+        ... })
+        >>> d.group("type").keys()
+        dict_keys(['A', 'B'])
+        >>> d.group("type").A.values()
+        dict_values([{'type': 'A', 'data': 1}, {'type': 'A', 'data': 2}])
+        >>> d.group("type").B.values()
+        dict_values([{'type': 'B', 'data': 3}])
+        >>> d.group("type").A.map("data")[1]
+        {'type': 'A', 'data': 1}
+
+        See Also
+        --------
+        map
+        """
+        return self.map(label, unique=False)
+
     # d |= other_d should still produce a valid AttrsDict
     def __ior__(self, other: dict | AttrsDict) -> AttrsDict:
         return AttrsDict(super().__ior__(other))
 
     # d1 | d2 should still produce a valid AttrsDict
     def __or__(self, other: dict | AttrsDict) -> AttrsDict:
         return AttrsDict(super().__or__(other))
 
 
-class JsonDB:
-    """Bare-bones JSON database.
+def JsonDB(*args, **kwargs):
+    import warnings
+
+    warnings.warn(
+        "The JsonDB class has been renamed to TextDB. "
+        "Please update your code, as JsonDB will be removed in a future release.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return TextDB(*args, **kwargs)
 
-    The database is represented on disk by a collection of JSON files
+
+class TextDB:
+    """A simple text file database.
+
+    The database is represented on disk by a collection of text files
     arbitrarily scattered in a filesystem. Subdirectories are also
-    :class:`.JsonDB` objects. In memory, the database is represented as an
+    :class:`.TextDB` objects. In memory, the database is represented as an
     :class:`AttrsDict`.
 
+    Currently supported file formats are JSON and YAML.
+
     Tip
     ---
     For large databases, a basic "lazy" mode is available. In this case, no
     global scan of the filesystem is performed at initialization time. Once a
     file is queried, it is also cached in the internal store for faster access.
     Caution, this option is for advanced use (see warning message below).
 
     Warning
     -------
     A manual call to :meth:`scan` is needed before most class methods (e.g.
     iterating on the database files) can be properly used.
 
     Examples
     --------
-    >>> from legendmeta.jsondb import JsonDB
-    >>> jdb = JsonDB("path/to/dir")
+    >>> from legendmeta.jsondb import TextDB
+    >>> jdb = TextDB("path/to/dir")
     >>> jdb["file1.json"]  # is a dict
+    >>> jdb["file1.yaml"]  # is a dict
     >>> jdb["file1"]  # also works
-    >>> jdb["dir1"]  # JsonDB instance
-    >>> jdb["dir1"]["file1"]  # nested JSON file
+    >>> jdb["dir1"]  # TextDB instance
+    >>> jdb["dir1"]["file1"]  # nested file
     >>> jdb["dir1/file1"]  # also works
     >>> jdb.dir1.file # keys can be accessed as attributes
     """
 
     def __init__(self, path: str | Path, lazy: str | bool = False) -> None:
-        """Construct a :class:`.JsonDB` object.
+        """Construct a :class:`.TextDB` object.
 
         Parameters
         ----------
         path
             path to the directory containing the database.
         lazy
             whether a database scan should be performed at initialization time.
@@ -249,54 +312,66 @@
             session.
         """
         if isinstance(lazy, bool):
             self.__lazy__ = lazy
         elif lazy == "auto":
             self.__lazy__ = not hasattr(sys, "ps1")
         else:
-            msg = f"unrecognized value lazy={lazy}"
+            msg = f"unrecognized value {lazy=}"
             raise ValueError(msg)
 
         self.__path__ = Path(path).expanduser().resolve()
 
         if not self.__path__.is_dir():
             msg = "input path is not a valid directory"
             raise ValueError(msg)
 
         self.__store__ = AttrsDict()
+        self.__ftypes__ = {"json", "yaml"}
 
         if not self.__lazy__:
             self.scan()
 
+    @property
+    def __extensions__(self) -> set:
+        # determine list of supported file extensions
+        return set().union(
+            *[
+                exts
+                for ft, exts in utils.__file_extensions__.items()
+                if ft in self.__ftypes__
+            ]
+        )
+
     def scan(self, recursive: bool = True, subdir: str = ".") -> None:
         """Populate the database by walking the filesystem.
 
         Parameters
         ----------
         recursive
             if ``True``, recurse subdirectories.
         subdir
             restrict scan to path relative to the database location.
         """
-        if recursive:
-            flist = self.__path__.rglob(f"{subdir}/*.json")
-        else:
-            flist = self.__path__.glob(f"{subdir}/*.json")
+        # recursive search or not?
+        _fcn = self.__path__.rglob if recursive else self.__path__.glob
+        # build file list
+        flist = (p for p in _fcn(f"{subdir}/*") if p.suffix in self.__extensions__)
 
         for j in flist:
             try:
-                self[j]
-            except (json.JSONDecodeError, ValueError) as e:
+                self[j.with_suffix("")]
+            except (json.JSONDecodeError, yaml.YAMLError, ValueError) as e:
                 msg = f"could not scan file {j}, reason {e}"
                 log.warning(msg)
 
     def keys(self) -> list[str]:
         return self.__store__.keys()
 
-    def items(self) -> Iterator[(str, JsonDB | AttrsDict | list)]:
+    def items(self) -> Iterator[(str, TextDB | AttrsDict | list)]:
         return self.__store__.items()
 
     def on(
         self, timestamp: str | datetime, pattern: str | None = None, system: str = "all"
     ) -> AttrsDict | list:
         """Query database in `time[, file pattern, system]`.
 
@@ -304,29 +379,29 @@
         to specify a validity mapping. This functionality relies on the
         :class:`.catalog.Catalog` class.
 
         The JSONL specification is documented at `this link
         <https://legend-exp.github.io/legend-data-format-specs/dev/metadata/#Specifying-metadata-validity-in-time-(and-system)>`_.
 
         The special ``$_`` string is expanded to the directory containing the
-        JSON files.
+        text files.
 
         Parameters
         ----------
         timestamp
             a :class:`~datetime.datetime` object or a string matching the
             pattern ``YYYYmmddTHHMMSSZ``.
         pattern
             query by filename pattern.
         system: 'all', 'phy', 'cal', 'lar', ...
             query only a data taking "system".
         """
         jsonl = self.__path__ / "validity.jsonl"
         if not jsonl.is_file():
-            msg = f"no validity.jsonl file found in {self.__path__}"
+            msg = f"no validity.jsonl file found in {self.__path__!s}"
             raise RuntimeError(msg)
 
         file_list = Catalog.get_files(str(jsonl), timestamp, system)
         # select only files matching pattern if specified
         if pattern is not None:
             c = re.compile(pattern)
             out_files = []
@@ -349,107 +424,129 @@
         else:
             fp = self.__path__.rglob(file)
             db_ptr = db_ptr[next(iter(fp))]
         Props.subst_vars(db_ptr, var_values={"_": self.__path__})
         return db_ptr
 
     def map(self, label: str, unique: bool = True) -> AttrsDict:
-        """Remap dictionary according to a second unique `key`.
+        """Remap dictionary according to a second unique `label`.
 
         See Also
         --------
         AttrsDict.map
 
         Warning
         -------
         If the database is lazy, you must call :meth:`.scan` in advance to
         populate it, otherwise mappings cannot be created.
         """
         return self.__store__.map(label, unique=unique)
 
-    def __getitem__(self, item: str | Path) -> JsonDB | AttrsDict | list:
+    def group(self, label: str) -> AttrsDict:
+        """Group dictionary according to a second unique `label`.
+
+        See Also
+        --------
+        AttrsDict.group
+
+        Warning
+        -------
+        If the database is lazy, you must call :meth:`.scan` in advance to
+        populate it, otherwise groupings cannot be created.
+        """
+        return self.__store__.group(label)
+
+    def __getitem__(self, item: str | Path) -> TextDB | AttrsDict | list:
         """Access files or directories in the database."""
         # resolve relative paths / links, but keep it relative to self.__path__
         item = Path(item)
 
         if item.is_absolute() and item.is_relative_to(self.__path__):
             item = item.expanduser().resolve().relative_to(self.__path__)
         elif not item.is_absolute():
             item = (
                 (self.__path__ / item).expanduser().resolve().relative_to(self.__path__)
             )
         else:
-            msg = f"{item} lies outside the database root path {self.__path__}"
+            msg = f"{item} lies outside the database root path {self.__path__!s}"
             raise ValueError(msg)
 
         # now call this very function recursively to walk the directories to the file
         db_ptr = self
         for d in item.parts[0:-1]:
             db_ptr = db_ptr[d]
 
         # item_id should not contain any / at this point
-        # store JSON file names without extension
+        # store file names without extension
         item_id = item.stem
         # skip if object is already in the store
         if item_id not in db_ptr.__store__:
             obj = db_ptr.__path__ / item.name
-            # if directory, construct another JsonDB object
+            # if directory, construct another TextDB object
             if obj.is_dir():
-                db_ptr.__store__[item_id] = JsonDB(obj, lazy=self.__lazy__)
+                db_ptr.__store__[item_id] = TextDB(obj, lazy=self.__lazy__)
+
             else:
-                # try to attach .json extension if file cannot be found
+                # try to attach an extension if file cannot be found
+                # but check if there are multiple files that only differ in extension (unsupported)
+                found = True
                 if not obj.is_file():
-                    obj = Path(str(obj) + ".json")
+                    found = False
+                    for ext in self.__extensions__:
+                        if obj.with_suffix(ext).is_file():
+                            if found:
+                                msg = "the database cannot contain files that differ only in the extension"
+                                raise RuntimeError(msg)
+
+                            obj = obj.with_suffix(ext)
+                            found = True
 
-                # if it's a valid JSON file, construct an AttrsDict object
-                if obj.is_file():
-                    with obj.open() as f:
-                        loaded = json.load(f)
-                        if isinstance(loaded, dict):
-                            loaded = AttrsDict(loaded)
-                            Props.subst_vars(loaded, var_values={"_": self.__path__})
-                        else:  # must be a list, check if there are dicts inside to convert
-                            for i, el in enumerate(loaded):
-                                if isinstance(el, dict):
-                                    loaded[i] = AttrsDict(el)
-                                    Props.subst_vars(
-                                        loaded[i], var_values={"_": self.__path__}
-                                    )
-
-                        db_ptr.__store__[item_id] = loaded
-                else:
-                    msg = f"{str(obj).replace('.json.json', '.json')} is not a valid file or directory"
+                if not found:
+                    msg = f"{obj.with_stem('.(json|yaml|yml)')} is not a valid file or directory"
                     raise FileNotFoundError(msg)
 
+                # if it's a valid file, construct an AttrsDict object
+                loaded = utils.load_dict(obj)
+                if isinstance(loaded, dict):
+                    loaded = AttrsDict(loaded)
+                    Props.subst_vars(loaded, var_values={"_": self.__path__})
+                else:  # must be a list, check if there are dicts inside to convert
+                    for i, el in enumerate(loaded):
+                        if isinstance(el, dict):
+                            loaded[i] = AttrsDict(el)
+                            Props.subst_vars(loaded[i], var_values={"_": self.__path__})
+
+                db_ptr.__store__[item_id] = loaded
+
             # set also an attribute, if possible
             if item_id.isidentifier():
                 db_ptr.__setattr__(item_id, db_ptr.__store__[item_id])
 
         return db_ptr.__store__[item_id]
 
-    def __getattr__(self, name: str) -> JsonDB | AttrsDict | list:
+    def __getattr__(self, name: str) -> TextDB | AttrsDict | list:
         try:
             return object.__getattribute__(self, name)
         except AttributeError:
             try:
                 return self.__getitem__(name)
             except AttributeError as exc:
-                msg = f"JSON database does not contain '{name}'"
+                msg = f"file database does not contain '{name}'"
                 raise AttributeError(msg) from exc
 
-    # NOTE: self cannot stay a JsonDB, since the class is characterized by a
+    # NOTE: self cannot stay a TextDB, since the class is characterized by a
     # (unique) root directory. What would be the root directory of the merged
-    # JsonDB?
-    def __ior__(self, other: JsonDB) -> AttrsDict:
-        msg = "cannot merge JsonDB in-place"
+    # TextDB?
+    def __ior__(self, other: TextDB) -> AttrsDict:
+        msg = "cannot merge TextDB in-place"
         raise TypeError(msg)
 
-    # NOTE: returning a JsonDB does not make much sense, see above
-    def __or__(self, other: JsonDB) -> AttrsDict:
-        if isinstance(other, JsonDB):
+    # NOTE: returning a TextDB does not make much sense, see above
+    def __or__(self, other: TextDB) -> AttrsDict:
+        if isinstance(other, TextDB):
             return self.__store__ | other.__store__
 
         return self.__store__ | other
 
     def __contains__(self, value: str) -> bool:
         return self.__store__.__contains__(value)
```

### Comparing `pylegendmeta-0.9.0a1/src/legendmeta/police.py` & `pylegendmeta-0.9.0a2/src/legendmeta/police.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,94 +18,92 @@
 import argparse
 import json
 import re
 import sys
 from importlib import resources
 from pathlib import Path
 
-from .jsondb import JsonDB
+from . import utils
+from .textdb import TextDB
 
 templates = resources.files("legendmeta") / "templates"
 
 
 def validate_legend_detector_db() -> bool:
     """Validate LEGEND detector database.
 
     Invoked in CLI.
     """
     parser = argparse.ArgumentParser(
         prog="validate-legend-detdb", description="Validate LEGEND detector database"
     )
 
-    parser.add_argument("files", nargs="+", help="JSON files")
+    parser.add_argument("files", nargs="+", help="files")
 
     args = parser.parse_args()
 
     dict_temp = {}
     for typ in ("bege", "ppc", "coax", "icpc"):
-        with (templates / f"{typ}-detector.json").open() as f:
-            dict_temp[typ] = json.load(f)
+        dict_temp[typ] = utils.load_dict(templates / f"{typ}-detector.yaml")
 
     for file in args.files:
         valid = True
 
-        with Path(file).open() as f:
-            entry = json.load(f)
+        entry = utils.load_dict(file)
 
-            if "type" not in entry:
-                print(  # noqa: T201
-                    f"ERROR: '{file}' entry does not contain 'type' key"
-                )
-                valid *= False
-                continue
-
-            if entry["type"] not in dict_temp:
-                print(  # noqa: T201
-                    f"WARNING: '{file}': no template for type '{entry['type']}' detector"
-                )
-                continue
-
-            valid *= validate_dict_schema(
-                entry,
-                dict_temp[entry["type"]],
-                greedy=False,
-                typecheck=True,
-                root_obj=file,
+        if "type" not in entry:
+            print(  # noqa: T201
+                f"ERROR: '{file}' entry does not contain 'type' key"
             )
+            valid *= False
+            continue
+
+        if entry["type"] not in dict_temp:
+            print(  # noqa: T201
+                f"WARNING: '{file}': no template for type '{entry['type']}' detector"
+            )
+            continue
+
+        valid *= validate_dict_schema(
+            entry,
+            dict_temp[entry["type"]],
+            greedy=False,
+            typecheck=True,
+            root_obj=file,
+        )
 
         if not valid:
             sys.exit(1)
 
 
 def validate_legend_channel_map() -> bool:
     """Validate list of LEGEND channel map files.
 
     Invoked in CLI.
     """
     parser = argparse.ArgumentParser(
         prog="validate-legend-chmaps", description="Validate LEGEND channel map files"
     )
 
-    parser.add_argument("files", nargs="+", help="JSON channel maps files")
+    parser.add_argument("files", nargs="+", help="channel maps files")
 
     args = parser.parse_args()
 
     dict_temp = {}
     for typ in ("geds", "spms"):
-        with (templates / f"{typ}-channel.json").open() as f:
-            dict_temp[typ] = json.load(f)
+        dict_temp[typ] = utils.load_dict(templates / f"{typ}-channel.yaml")
 
     for d in {Path(f).parent for f in args.files}:
-        db = JsonDB(d)
+        db = TextDB(d)
         valid = True
 
         with Path(f"{d}/validity.jsonl").open() as f:
             for line in f.readlines():
                 ts = json.loads(line)["valid_from"]
-                sy = json.loads(line)["category"]
+                sy = json.loads(line)["select"]
                 chmap = db.on(ts, system=sy)
 
                 for k, v in chmap.items():
                     if "system" not in v:
                         print(  # noqa: T201
                             f"ERROR: '{k}' entry does not contain 'system' key"
                         )
```

### Comparing `pylegendmeta-0.9.0a1/src/legendmeta/scdb_tables.py` & `pylegendmeta-0.9.0a2/src/legendmeta/scdb_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from dataclasses import dataclass
 from datetime import datetime
 
 import sqlalchemy as db
 from sqlalchemy.orm import DeclarativeBase, Mapped
 
-from .jsondb import AttrsDict
+from .textdb import AttrsDict
 
 
 class Base(DeclarativeBase):
     pass
 
 
 @dataclass
```

### Comparing `pylegendmeta-0.9.0a1/src/legendmeta/slowcontrol.py` & `pylegendmeta-0.9.0a2/src/legendmeta/slowcontrol.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.9.0a1/src/pylegendmeta.egg-info/PKG-INFO` & `pylegendmeta-0.9.0a2/src/pylegendmeta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylegendmeta
-Version: 0.9.0a1
+Version: 0.9.0a2
 Summary: Python LEGEND-metadata implementation
 Author-email: Luigi Pertoldi <gipert@pm.me>
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/legend-exp/pylegendmeta
 Project-URL: Bug Tracker, https://github.com/legend-exp/pylegedmeta/issues
 Project-URL: Discussions, https://github.com/legend-exp/pylegedmeta/discussions
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: GitPython
 Requires-Dist: pandas
+Requires-Dist: pyyaml
 Requires-Dist: psycopg2-binary
 Requires-Dist: sqlalchemy>=2
 Provides-Extra: all
 Requires-Dist: pylegendmeta[docs,test]; extra == "all"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
```

### Comparing `pylegendmeta-0.9.0a1/src/pylegendmeta.egg-info/SOURCES.txt` & `pylegendmeta-0.9.0a2/src/pylegendmeta.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 LICENSE
 README.md
 pyproject.toml
 src/legendmeta/__init__.py
 src/legendmeta/_version.py
 src/legendmeta/catalog.py
 src/legendmeta/core.py
-src/legendmeta/jsondb.py
 src/legendmeta/police.py
 src/legendmeta/scdb_tables.py
 src/legendmeta/slowcontrol.py
-src/legendmeta/templates/bege-detector.json
-src/legendmeta/templates/coax-detector.json
-src/legendmeta/templates/geds-channel.json
-src/legendmeta/templates/icpc-detector.json
-src/legendmeta/templates/ppc-detector.json
-src/legendmeta/templates/spms-channel.json
+src/legendmeta/textdb.py
+src/legendmeta/utils.py
+src/legendmeta/templates/bege-detector.yaml
+src/legendmeta/templates/coax-detector.yaml
+src/legendmeta/templates/geds-channel.yaml
+src/legendmeta/templates/icpc-detector.yaml
+src/legendmeta/templates/ppc-detector.yaml
+src/legendmeta/templates/spms-channel.yaml
 src/pylegendmeta.egg-info/PKG-INFO
 src/pylegendmeta.egg-info/SOURCES.txt
 src/pylegendmeta.egg-info/dependency_links.txt
 src/pylegendmeta.egg-info/entry_points.txt
 src/pylegendmeta.egg-info/not-zip-safe
 src/pylegendmeta.egg-info/requires.txt
 src/pylegendmeta.egg-info/top_level.txt
 tests/test_catalog.py
 tests/test_jsondb.py
 tests/test_lmeta.py
 tests/test_police.py
 tests/test_slowcontroldb.py
-tests/testdb/arrays.json
+tests/testdb/arrays.yaml
 tests/testdb/file1.json
-tests/testdb/file2.json
+tests/testdb/file2.yaml
 tests/testdb/file3.json
 tests/testdb/dir1/file3.json
 tests/testdb/dir1/file5.json
 tests/testdb/dir1/validity.jsonl
-tests/testdb/dir1/dir2/file4.json
+tests/testdb/dir1/dir2/file4.yaml
 tests/testdb/dir2/file7.json
 tests/testdb/dir2/file8.json
```

### Comparing `pylegendmeta-0.9.0a1/tests/test_jsondb.py` & `pylegendmeta-0.9.0a2/tests/test_jsondb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 from datetime import datetime, timezone
 from pathlib import Path
 
 import pytest
 
-from legendmeta import AttrsDict, JsonDB
+from legendmeta import AttrsDict, TextDB
 from legendmeta.catalog import Props
 
 testdb = Path(__file__).parent / "testdb"
 
 
 def test_props():
     # test read_from
-    test_dict = Props.read_from(str(Path(__file__).parent / "testdb/file2.json"))
+    test_dict = Props.read_from(str(Path(__file__).parent / "testdb/file2.yaml"))
     assert test_dict["data"] == 2
 
     # test subst_vars
     Props.subst_vars(test_dict, var_values={"_": str(Path(__file__).parent / "testdb")})
     assert test_dict["filepath"] == str(
         Path(__file__).parent / "testdb/dir1/file3.json"
     )
@@ -31,46 +31,46 @@
     # test trim null
     Props.trim_null(test_dict)
     with pytest.raises(KeyError):
         test_dict["null_key"]
 
     test_dict = Props.read_from(
         [
-            str(Path(__file__).parent / "testdb/file2.json"),
+            str(Path(__file__).parent / "testdb/file2.yaml"),
             str(Path(__file__).parent / "testdb/file3.json"),
         ],
         subst_pathvar=True,
         trim_null=True,
     )
     assert test_dict["data"] == 3
     assert test_dict["filepath"] == str(
         Path(__file__).parent / "testdb/dir1/file3.json"
     )
     with pytest.raises(KeyError):
         test_dict["null_key"]
 
 
 def test_access():
-    jdb = JsonDB(testdb)
+    jdb = TextDB(testdb)
     assert isinstance(jdb["file1.json"], AttrsDict)
-    assert isinstance(jdb["file2.json"], AttrsDict)
+    assert isinstance(jdb["file2.yaml"], AttrsDict)
     assert isinstance(jdb["file1"], AttrsDict)
-    assert isinstance(jdb["dir1"], JsonDB)
+    assert isinstance(jdb["dir1"], TextDB)
     assert isinstance(jdb["dir1"]["file3.json"], AttrsDict)
     assert isinstance(jdb["dir1"]["file3"], AttrsDict)
     assert isinstance(jdb["dir1/file3.json"], AttrsDict)
-    assert isinstance(jdb["dir1"]["dir2"], JsonDB)
+    assert isinstance(jdb["dir1"]["dir2"], TextDB)
     assert isinstance(jdb["dir1"]["dir2"]["file4.json"], AttrsDict)
     assert isinstance(jdb["dir1/dir2/file4.json"], AttrsDict)
     assert jdb["file1.json"]["data"] == 1
     assert isinstance(jdb["file1"]["group"], AttrsDict)
 
     assert isinstance(jdb.file1, AttrsDict)
     assert isinstance(jdb.file1.group, AttrsDict)
-    assert isinstance(jdb.dir1, JsonDB)
+    assert isinstance(jdb.dir1, TextDB)
     assert isinstance(jdb.dir1.file3, AttrsDict)
     assert jdb.file1.data == 1
     assert jdb.file2.data == 2
     assert jdb.dir1.file3.data == 1
     assert jdb.file1.group.data1 == 1
 
     assert isinstance(jdb.arrays, list)
@@ -81,85 +81,88 @@
     assert isinstance(jdb.arrays[1].array[1], AttrsDict)
     assert jdb.arrays[1].array[0] == 1
     assert jdb.arrays[1].array[1].data == 2
 
     assert jdb.file2.filepath == str(Path(__file__).parent / "testdb/dir1/file3.json")
 
     with pytest.raises(ValueError):
-        JsonDB("non-existent-db")
+        TextDB("non-existent-db")
     with pytest.raises(FileNotFoundError):
         jdb["non-existent-file"]
     with pytest.raises(FileNotFoundError):
         assert jdb.non_existent_file
 
     with pytest.raises(AttributeError):
         assert jdb.dir1.file3.non_existent_key
 
 
 def test_keys():
-    jdb = JsonDB(testdb, lazy=False)
+    jdb = TextDB(testdb, lazy=False)
     assert sorted(jdb.keys()) == ["arrays", "dir1", "dir2", "file1", "file2", "file3"]
     assert sorted(jdb.dir1.keys()) == ["dir2", "file3", "file5"]
 
     assert "arrays" in jdb
 
 
 def test_items():
-    jdb = JsonDB(testdb, lazy=False)
+    jdb = TextDB(testdb, lazy=False)
     items = sorted(jdb.items())
     assert items[0][0] == "arrays"
     assert isinstance(items[0][1], list)
     assert items[1][0] == "dir1"
-    assert isinstance(items[1][1], JsonDB)
+    assert isinstance(items[1][1], TextDB)
     assert items[3][0] == "file1"
     assert isinstance(items[3][1], AttrsDict)
 
 
 def test_scan():
-    jdb = JsonDB(testdb, lazy=True)
+    jdb = TextDB(testdb, lazy=True)
     jdb.scan(recursive=True)
 
     assert sorted(jdb.__dict__.keys()) == [
+        "__ftypes__",
         "__lazy__",
         "__path__",
         "__store__",
         "arrays",
         "dir1",
         "dir2",
         "file1",
         "file2",
         "file3",
     ]
 
-    jdb = JsonDB(testdb, lazy=True)
+    jdb = TextDB(testdb, lazy=True)
     jdb.scan(recursive=False)
 
     assert sorted(jdb.__dict__.keys()) == [
+        "__ftypes__",
         "__lazy__",
         "__path__",
         "__store__",
         "arrays",
         "file1",
         "file2",
         "file3",
     ]
 
-    jdb = JsonDB(testdb, lazy=True)
+    jdb = TextDB(testdb, lazy=True)
     jdb.scan(recursive=False, subdir="dir1")
 
     assert sorted(jdb.__dict__.keys()) == [
+        "__ftypes__",
         "__lazy__",
         "__path__",
         "__store__",
         "dir1",
     ]
 
 
 def test_time_validity():
-    jdb = JsonDB(testdb)
+    jdb = TextDB(testdb)
     assert isinstance(jdb["dir1"].on("20220628T221955Z"), AttrsDict)
 
     assert jdb["dir1"].on("20220628T221955Z")["data"] == 1
     assert jdb.dir1.on("20220629T221955Z").data == 2
     # time point in between
     assert jdb["dir1"].on("20220628T233500Z")["data"] == 1
     # time point after
@@ -182,29 +185,32 @@
     assert jdb.dir1.on(tstamp, r"^file3.*", "all").data == 1
 
     assert jdb.dir1.on(tstamp, system="phy").data == 1
     assert jdb.dir1.on(tstamp, system="cal").data == 1
 
 
 def test_mapping():
-    jdb = JsonDB(testdb)
+    jdb = TextDB(testdb)
 
     assert isinstance(jdb.map("label"), AttrsDict)
     assert jdb.map("label")[3].data == 2
     assert jdb.map("key.label")[3].data == 2
     assert isinstance(jdb.file1.group.map("label"), AttrsDict)
     assert jdb.file1.group.map("label")["a"].data == 1
     assert jdb.file1.group.map("label")["b"].data == 2
 
     with pytest.raises(RuntimeError):
         jdb.map("system", unique=True)
 
     assert jdb.map("system", unique=False)[2].map("label")[1].data == 3
     assert jdb.map("system", unique=False)[1].map("label")[2].data == 1
 
+    assert jdb.group("system")[2].map("label")[1].data == 3
+    assert jdb.group("system")[1].map("label")[2].data == 1
+
     with pytest.raises(ValueError):
         jdb.map("non-existent-label")
 
 
 def test_modification():
     d = AttrsDict()
     d["a"] = 1
@@ -225,37 +231,48 @@
     d2 = d | {"c": 3}
     assert isinstance(d2, AttrsDict)
     assert d2 == {"a": 1, "b": 2, "c": 3}
     assert hasattr(d2, "a")
     assert hasattr(d2, "b")
     assert hasattr(d2, "c")
 
-    jdb = JsonDB(testdb, lazy=False)
+    jdb = TextDB(testdb, lazy=False)
     j = jdb.dir1 | jdb.dir2
     assert isinstance(j, AttrsDict)
     assert sorted(j.keys()) == ["dir2", "file3", "file5", "file7", "file8"]
     assert hasattr(j, "dir2")
     assert hasattr(j, "file8")
 
     with pytest.raises(TypeError):
         jdb |= jdb.dir1
 
 
 def test_lazyness():
-    jdb = JsonDB(testdb, lazy="auto")
+    jdb = TextDB(testdb, lazy="auto")
     assert jdb.__lazy__ is True
-    assert sorted(jdb.__dict__.keys()) == ["__lazy__", "__path__", "__store__"]
+    assert sorted(jdb.__dict__.keys()) == [
+        "__ftypes__",
+        "__lazy__",
+        "__path__",
+        "__store__",
+    ]
 
-    jdb = JsonDB(testdb, lazy=True)
+    jdb = TextDB(testdb, lazy=True)
     assert jdb.__lazy__ is True
-    assert sorted(jdb.__dict__.keys()) == ["__lazy__", "__path__", "__store__"]
+    assert sorted(jdb.__dict__.keys()) == [
+        "__ftypes__",
+        "__lazy__",
+        "__path__",
+        "__store__",
+    ]
 
-    jdb = JsonDB(testdb, lazy=False)
+    jdb = TextDB(testdb, lazy=False)
     assert jdb.__lazy__ is False
     assert sorted(jdb.__dict__.keys()) == [
+        "__ftypes__",
         "__lazy__",
         "__path__",
         "__store__",
         "arrays",
         "dir1",
         "dir2",
         "file1",
```

### Comparing `pylegendmeta-0.9.0a1/tests/test_lmeta.py` & `pylegendmeta-0.9.0a2/tests/test_lmeta.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from datetime import datetime
 
 import pytest
 from git import GitCommandError
 
 from legendmeta import LegendMetadata
-from legendmeta.jsondb import AttrsDict
+from legendmeta.textdb import AttrsDict
 
 pytestmark = pytest.mark.xfail(run=True, reason="requires access to legend-metadata")
 
 
 @pytest.fixture(scope="module")
 def metadb():
     mdata = LegendMetadata()
```

### Comparing `pylegendmeta-0.9.0a1/tests/test_police.py` & `pylegendmeta-0.9.0a2/tests/test_police.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.9.0a1/tests/test_slowcontroldb.py` & `pylegendmeta-0.9.0a2/tests/test_slowcontroldb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import pytest
 import sqlalchemy as sql
 
 from legendmeta import LegendMetadata, LegendSlowControlDB
-from legendmeta.jsondb import AttrsDict
 from legendmeta.slowcontrol import DiodeSnap
+from legendmeta.textdb import AttrsDict
 
 pytestmark = pytest.mark.xfail(
     run=True, reason="requires access to LEGEND slow control database"
 )
 
 
 @pytest.fixture(scope="session")
```

