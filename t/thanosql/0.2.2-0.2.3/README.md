# Comparing `tmp/thanosql-0.2.2.tar.gz` & `tmp/thanosql-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thanosql-0.2.2.tar", last modified: Tue Apr 23 06:20:33 2024, max compression
+gzip compressed data, was "thanosql-0.2.3.tar", last modified: Fri Apr 26 06:41:19 2024, max compression
```

## Comparing `thanosql-0.2.2.tar` & `thanosql-0.2.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.085106 thanosql-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 06:20:27.000000 thanosql-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-23 06:20:33.085106 thanosql-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-23 06:20:27.000000 thanosql-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:27.000000 thanosql-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 06:20:33.085106 thanosql-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-23 06:20:27.000000 thanosql-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.077106 thanosql-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_table_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.077106 thanosql-0.2.2/thanosql/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.081106 thanosql-0.2.2/thanosql/magic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/magic/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/magic/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/magic/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/magic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.081106 thanosql-0.2.2/thanosql/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.081106 thanosql-0.2.2/thanosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-23 06:20:33.000000 thanosql-0.2.2/thanosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 06:20:33.000000 thanosql-0.2.2/thanosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:20:33.000000 thanosql-0.2.2/thanosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:20:32.000000 thanosql-0.2.2/thanosql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-23 06:20:33.000000 thanosql-0.2.2/thanosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 06:20:33.000000 thanosql-0.2.2/thanosql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:41:19.716823 thanosql-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-26 06:41:15.000000 thanosql-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-26 06:41:19.716823 thanosql-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-26 06:41:15.000000 thanosql-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 06:41:15.000000 thanosql-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:41:19.716823 thanosql-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-26 06:41:15.000000 thanosql-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:41:19.712823 thanosql-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-26 06:41:15.000000 thanosql-0.2.3/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-04-26 06:41:15.000000 thanosql-0.2.3/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-26 06:41:15.000000 thanosql-0.2.3/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-26 06:41:15.000000 thanosql-0.2.3/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-26 06:41:15.000000 thanosql-0.2.3/tests/test_table_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-26 06:41:15.000000 thanosql-0.2.3/tests/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:41:19.712823 thanosql-0.2.3/thanosql/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:41:19.712823 thanosql-0.2.3/thanosql/magic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/magic/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/magic/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/magic/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/magic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:41:19.716823 thanosql-0.2.3/thanosql/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/resources/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/resources/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/resources/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/resources/_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/resources/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24077 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/resources/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-26 06:41:15.000000 thanosql-0.2.3/thanosql/resources/_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:41:19.716823 thanosql-0.2.3/thanosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-26 06:41:19.000000 thanosql-0.2.3/thanosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-26 06:41:19.000000 thanosql-0.2.3/thanosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:41:19.000000 thanosql-0.2.3/thanosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:41:19.000000 thanosql-0.2.3/thanosql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-26 06:41:19.000000 thanosql-0.2.3/thanosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 06:41:19.000000 thanosql-0.2.3/thanosql.egg-info/top_level.txt
```

### Comparing `thanosql-0.2.2/LICENSE` & `thanosql-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/PKG-INFO` & `thanosql-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: thanosql
-Version: 0.2.2
+Version: 0.2.3
 Summary: ThanoSQL SDK for Python
 Home-page: https://github.com/smartmind-team/thanosql-python
 Author: SmartMind
 Author-email: dev@smartmind.team
 License: MIT
 Keywords: smartmind thanosql sdk
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: pydantic>=2.0
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: urllib3
 Provides-Extra: dev
@@ -26,15 +27,14 @@
 Requires-Dist: myst-nb; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Provides-Extra: magic
 Requires-Dist: ipython; extra == "magic"
 Requires-Dist: sqlalchemy; extra == "magic"
 Requires-Dist: matplotlib; extra == "magic"
-Requires-Dist: numpy; extra == "magic"
 Requires-Dist: websocket-client; extra == "magic"
 Requires-Dist: pglast; extra == "magic"
 
 # ThanoSQL Python Library
 
 The ThanoSQL Python library provides convenient access to the ThanoSQL API from any Python 3.8+ application. The library covers all ThanoSQL operations that users can do, such as querying, editing tables, and much more.
```

### Comparing `thanosql-0.2.2/README.md` & `thanosql-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/setup.py` & `thanosql-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,28 +27,28 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords="smartmind thanosql sdk",
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=[
+        "numpy",
         "openpyxl",
         "pandas",
         "pydantic>=2.0",
         "requests",
         "tqdm",
         "urllib3",
     ],
     extras_require={
         "dev": ["faker", "pytest", "myst-nb", "sphinx-autoapi", "sphinx-rtd-theme"],
         "magic": [
             "ipython",
             "sqlalchemy",
             "matplotlib",
-            "numpy",
             "websocket-client",
             "pglast",
         ],
     },
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `thanosql-0.2.2/tests/test_file.py` & `thanosql-0.2.3/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/tests/test_query.py` & `thanosql-0.2.3/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/tests/test_schema.py` & `thanosql-0.2.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/tests/test_table.py` & `thanosql-0.2.3/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/tests/test_table_template.py` & `thanosql-0.2.3/tests/test_table_template.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/tests/test_view.py` & `thanosql-0.2.3/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/_base_client.py` & `thanosql-0.2.3/thanosql/_base_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -128,16 +128,18 @@
                     raise thanosql_error.ThanoSQLValueError(message=message)
                 elif code in {401, 403}:
                     raise thanosql_error.ThanoSQLPermissionError(message=message)
                 elif code == 404:
                     raise thanosql_error.ThanoSQLNotFoundError(message=message)
                 elif code == 409:
                     raise thanosql_error.ThanoSQLAlreadyExistsError(message=message)
-                elif code == 500:
-                    raise thanosql_error.ThanoSQLInternalError(message=message)
+                # includes 413 and 500, among many others
+                # will show up as ThanoSQLInternalError with the message from raise_for_status
+                else:
+                    response.raise_for_status()
 
             if stream:
                 filename = response.headers.get(
                     "Content-Disposition", "filename=output.bin"
                 ).split("filename=")[1]
                 with open(filename, "wb") as handle:
                     for data in tqdm(response.iter_content()):
```

### Comparing `thanosql-0.2.2/thanosql/_client.py` & `thanosql-0.2.3/thanosql/_client.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/_error.py` & `thanosql-0.2.3/thanosql/_error.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/_service.py` & `thanosql-0.2.3/thanosql/_service.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/magic/magic.py` & `thanosql-0.2.3/thanosql/magic/magic.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/magic/parse.py` & `thanosql-0.2.3/thanosql/magic/parse.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/magic/util.py` & `thanosql-0.2.3/thanosql/magic/util.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/resources/__init__.py` & `thanosql-0.2.3/thanosql/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/resources/_file.py` & `thanosql-0.2.3/thanosql/resources/_file.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/resources/_query.py` & `thanosql-0.2.3/thanosql/resources/_query.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/resources/_record.py` & `thanosql-0.2.3/thanosql/resources/_record.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/resources/_schema.py` & `thanosql-0.2.3/thanosql/resources/_schema.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql/resources/_table.py` & `thanosql-0.2.3/thanosql/resources/_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import enum
 import os
 from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Union
 
 import pandas as pd
+from numpy import nan
 from pydantic import Field, TypeAdapter
 
 from thanosql._error import ThanoSQLValueError
 from thanosql._service import ThanoSQLService
 from thanosql.resources._model import BaseModel
 from thanosql.resources._record import Records
 
@@ -289,15 +290,15 @@
         ----------
         name : str
             The name of the table created from the file or DataFrame.
         file : str or PathLike, optional
             CSV or Excel-like file containing tabulated data to be uploaded
             to the specified table.
         df : DataFrame, optional
-            Pandas DataFrame containing data to be uploaded to the specified 
+            Pandas DataFrame containing data to be uploaded to the specified
             table.
         schema : str, optional
             The schema to save the created table in. If not specified, the table
             will be saved to "public".
         table : TableObject, optional
             TableObject containing the columns and constraints of the table
             to be created. If specified, the created table will follow the object
@@ -376,14 +377,15 @@
             )
 
             return self._parse_table_response(raw_response)
 
         elif df is not None:
             path = f"/{self.tag}/{name}/upload/json"
 
+            df = df.replace({nan: None})
             df_json = df.to_dict(orient="records")
             query_params = self._create_input_dict(
                 schema=schema, if_exists=if_exists_enum.value
             )
             payload = self._create_input_dict(table=table, data=df_json)
 
             raw_response = self.client._request(
```

### Comparing `thanosql-0.2.2/thanosql/resources/_view.py` & `thanosql-0.2.3/thanosql/resources/_view.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.2/thanosql.egg-info/PKG-INFO` & `thanosql-0.2.3/thanosql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: thanosql
-Version: 0.2.2
+Version: 0.2.3
 Summary: ThanoSQL SDK for Python
 Home-page: https://github.com/smartmind-team/thanosql-python
 Author: SmartMind
 Author-email: dev@smartmind.team
 License: MIT
 Keywords: smartmind thanosql sdk
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: pydantic>=2.0
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: urllib3
 Provides-Extra: dev
@@ -26,15 +27,14 @@
 Requires-Dist: myst-nb; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Provides-Extra: magic
 Requires-Dist: ipython; extra == "magic"
 Requires-Dist: sqlalchemy; extra == "magic"
 Requires-Dist: matplotlib; extra == "magic"
-Requires-Dist: numpy; extra == "magic"
 Requires-Dist: websocket-client; extra == "magic"
 Requires-Dist: pglast; extra == "magic"
 
 # ThanoSQL Python Library
 
 The ThanoSQL Python library provides convenient access to the ThanoSQL API from any Python 3.8+ application. The library covers all ThanoSQL operations that users can do, such as querying, editing tables, and much more.
```

### Comparing `thanosql-0.2.2/thanosql.egg-info/SOURCES.txt` & `thanosql-0.2.3/thanosql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

