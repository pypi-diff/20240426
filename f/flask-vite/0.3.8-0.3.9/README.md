# Comparing `tmp/flask_vite-0.3.8.tar.gz` & `tmp/flask_vite-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_vite-0.3.8.tar", max compression
+gzip compressed data, was "flask_vite-0.3.9.tar", max compression
```

## Comparing `flask_vite-0.3.8.tar` & `flask_vite-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      144 2023-10-27 14:41:44.670623 flask_vite-0.3.8/AUTHORS.rst
--rw-r--r--   0        0        0     1074 2023-10-27 14:31:08.285369 flask_vite-0.3.8/LICENSE
--rw-r--r--   0        0        0     4335 2023-10-27 14:33:46.572110 flask_vite-0.3.8/README.md
--rw-r--r--   0        0        0     1401 2024-03-28 20:22:36.311900 flask_vite-0.3.8/pyproject.toml
--rw-r--r--   0        0        0       48 2022-09-02 18:03:03.970225 flask_vite-0.3.8/src/flask_vite/__init__.py
--rw-r--r--   0        0        0     1545 2024-02-01 14:55:12.742635 flask_vite-0.3.8/src/flask_vite/cli.py
--rw-r--r--   0        0        0     1877 2023-09-19 16:48:29.779804 flask_vite-0.3.8/src/flask_vite/extension.py
--rw-r--r--   0        0        0     1142 2023-09-19 17:13:20.292046 flask_vite-0.3.8/src/flask_vite/npm.py
--rw-r--r--   0        0        0       50 2023-07-04 09:13:43.637994 flask_vite-0.3.8/src/flask_vite/starter/.gitignore
--rwxr-xr-t   0        0        0    52227 2024-01-10 18:30:13.543461 flask_vite-0.3.8/src/flask_vite/starter/bun.lockb
--rw-r--r--   0        0        0      280 2023-07-04 08:57:59.573627 flask_vite-0.3.8/src/flask_vite/starter/index.html
--rw-r--r--   0        0        0       27 2023-07-04 09:14:53.281846 flask_vite-0.3.8/src/flask_vite/starter/main.js
--rw-r--r--   0        0        0      360 2024-01-10 18:30:05.609248 flask_vite-0.3.8/src/flask_vite/starter/package.json
--rw-r--r--   0        0        0       82 2023-07-04 09:05:39.738914 flask_vite-0.3.8/src/flask_vite/starter/postcss.config.js
--rw-r--r--   0        0        0       59 2023-07-04 08:17:31.233442 flask_vite-0.3.8/src/flask_vite/starter/src/styles.css
--rw-r--r--   0        0        0      157 2023-07-04 09:03:39.209131 flask_vite-0.3.8/src/flask_vite/starter/tailwind.config.js
--rw-r--r--   0        0        0      131 2023-07-04 08:17:31.234222 flask_vite-0.3.8/src/flask_vite/starter/vite.config.js
--rw-r--r--   0        0        0      902 2023-01-04 10:16:52.879813 flask_vite-0.3.8/src/flask_vite/tags.py
--rw-r--r--   0        0        0       40 2022-04-08 07:28:14.665349 flask_vite-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0     1287 2023-10-27 14:33:51.316229 flask_vite-0.3.8/tests/test_flask_vite.py
--rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 flask_vite-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      144 2023-10-27 14:41:44.670623 flask_vite-0.3.9/AUTHORS.rst
+-rw-r--r--   0        0        0     1074 2023-10-27 14:31:08.285369 flask_vite-0.3.9/LICENSE
+-rw-r--r--   0        0        0     4335 2023-10-27 14:33:46.572110 flask_vite-0.3.9/README.md
+-rw-r--r--   0        0        0      999 2024-04-26 16:36:34.001504 flask_vite-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      157 2024-04-26 16:16:57.467495 flask_vite-0.3.9/src/flask_vite/__init__.py
+-rw-r--r--   0        0        0     1653 2024-04-26 16:25:38.956462 flask_vite-0.3.9/src/flask_vite/cli.py
+-rw-r--r--   0        0        0     1974 2024-04-26 16:31:01.388966 flask_vite-0.3.9/src/flask_vite/extension.py
+-rw-r--r--   0        0        0     1263 2024-04-26 16:34:32.184328 flask_vite-0.3.9/src/flask_vite/npm.py
+-rw-r--r--   0        0        0       50 2023-07-04 09:13:43.637994 flask_vite-0.3.9/src/flask_vite/starter/.gitignore
+-rwxr-xr-t   0        0        0    52227 2024-01-10 18:30:13.543461 flask_vite-0.3.9/src/flask_vite/starter/bun.lockb
+-rw-r--r--   0        0        0      280 2023-07-04 08:57:59.573627 flask_vite-0.3.9/src/flask_vite/starter/index.html
+-rw-r--r--   0        0        0       27 2023-07-04 09:14:53.281846 flask_vite-0.3.9/src/flask_vite/starter/main.js
+-rw-r--r--   0        0        0      360 2024-01-10 18:30:05.609248 flask_vite-0.3.9/src/flask_vite/starter/package.json
+-rw-r--r--   0        0        0       82 2023-07-04 09:05:39.738914 flask_vite-0.3.9/src/flask_vite/starter/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-07-04 08:17:31.233442 flask_vite-0.3.9/src/flask_vite/starter/src/styles.css
+-rw-r--r--   0        0        0      157 2023-07-04 09:03:39.209131 flask_vite-0.3.9/src/flask_vite/starter/tailwind.config.js
+-rw-r--r--   0        0        0      131 2023-07-04 08:17:31.234222 flask_vite-0.3.9/src/flask_vite/starter/vite.config.js
+-rw-r--r--   0        0        0     1014 2024-04-26 16:27:24.908127 flask_vite-0.3.9/src/flask_vite/tags.py
+-rw-r--r--   0        0        0      113 2024-04-26 16:14:35.052843 flask_vite-0.3.9/tests/__init__.py
+-rw-r--r--   0        0        0     1317 2024-04-26 16:35:17.584356 flask_vite-0.3.9/tests/test_flask_vite.py
+-rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 flask_vite-0.3.9/PKG-INFO
```

### Comparing `flask_vite-0.3.8/LICENSE` & `flask_vite-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_vite-0.3.8/README.md` & `flask_vite-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `flask_vite-0.3.8/src/flask_vite/cli.py` & `flask_vite-0.3.9/src/flask_vite/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+# Copyright (c) 2022-2024, Abilian SAS
+#
+# SPDX-License-Identifier: MIT
 """Console script for flask_vite."""
 
+from __future__ import annotations
+
 import shutil
 import sys
 from pathlib import Path
 
 import click
 from click import secho
 from flask import current_app
```

### Comparing `flask_vite-0.3.8/src/flask_vite/extension.py` & `flask_vite-0.3.9/src/flask_vite/extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+# Copyright (c) 2022-2024, Abilian SAS
+#
+# SPDX-License-Identifier: MIT
 """Main module."""
 
+from __future__ import annotations
+
 import os
+from http.client import OK
 from pathlib import Path
-from typing import Optional
 
 from flask import Flask, Response, send_from_directory
 
 from .npm import NPM
 from .tags import make_tag
 
 ONE_YEAR = 60 * 60 * 24 * 365
 
 
 class Vite:
-    app: Optional[Flask] = None
-    npm: Optional[NPM] = None
+    app: Flask | None = None
+    npm: NPM | None = None
 
-    def __init__(self, app: Optional[Flask] = None):
+    def __init__(self, app: Flask | None = None):
         self.app = app
 
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app: Flask):
         if "vite" in app.extensions:
@@ -37,15 +42,15 @@
         npm_bin_path = config.get("VITE_NPM_BIN_PATH", "npm")
         self.npm = NPM(cwd=str(self._get_root()), npm_bin_path=npm_bin_path)
 
         app.route("/_vite/<path:filename>")(self.vite_static)
         app.template_global("vite_tags")(make_tag)
 
     def after_request(self, response: Response):
-        if response.status_code != 200:
+        if response.status_code != OK:
             return response
 
         mimetype = response.mimetype or ""
         if not mimetype.startswith("text/html"):
             return response
 
         if not isinstance(response.response, list):
```

### Comparing `flask_vite-0.3.8/src/flask_vite/npm.py` & `flask_vite-0.3.9/src/flask_vite/npm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# Copyright (c) 2022-2024, Abilian SAS
+#
+# SPDX-License-Identifier: MIT
+
+from __future__ import annotations
+
 import subprocess
 from dataclasses import dataclass
 from textwrap import dedent
 
 # Assume npm is in the path for now.
 NPM_BIN_PATH = "npm"
 
@@ -13,16 +19,16 @@
 @dataclass
 class NPM:
     cwd: str = ""
     npm_bin_path: str = NPM_BIN_PATH
 
     def run(self, *args):
         try:
-            _args = [self.npm_bin_path] + list(args)
-            subprocess.run(_args, cwd=self.cwd)
+            _args = [self.npm_bin_path, *list(args)]
+            subprocess.run(_args, cwd=self.cwd, check=True)
         except OSError as e:
             if e.filename == self.npm_bin_path:
                 msg = """
                 It looks like node.js and/or npm is not installed or cannot be found.
                 Visit https://nodejs.org to download and install node.js for your system.
                 """
             elif e.filename == self.cwd:
```

### Comparing `flask_vite-0.3.8/src/flask_vite/starter/bun.lockb` & `flask_vite-0.3.9/src/flask_vite/starter/bun.lockb`

 * *Files identical despite different names*

### Comparing `flask_vite-0.3.8/src/flask_vite/tags.py` & `flask_vite-0.3.9/src/flask_vite/tags.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+# Copyright (c) 2022-2024, Abilian SAS
+#
+# SPDX-License-Identifier: MIT
+
+from __future__ import annotations
+
 import glob
 from textwrap import dedent
 
 from flask import current_app
 
 
-def make_tag(static: bool = False):
+def make_tag(*, static: bool = False):
     if static or not current_app.debug:
         return make_static_tag()
     else:
         return make_debug_tag()
 
 
 def make_static_tag():
```

### Comparing `flask_vite-0.3.8/tests/test_flask_vite.py` & `flask_vite-0.3.9/tests/test_flask_vite.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-#!/usr/bin/env python
+# Copyright (c) 2022-2024, Abilian SAS
+#
+# SPDX-License-Identifier: MIT
 
 """Tests for `flask_vite` package."""
 from pathlib import Path
 
 import pytest
 from click.testing import CliRunner
 from flask import Flask
@@ -36,16 +38,15 @@
     vite = Vite(app)
     npm = vite.npm
     assert npm.npm_bin_path == "npm"
 
     Path("vite").mkdir(exist_ok=True)
 
     with app.app_context():
-        npm.run()
-        npm.run("--help")
+        npm.run("help")
 
 
 def test_npm_alt_path():
     app = Flask(__name__)
     app.config["VITE_NPM_BIN_PATH"] = "xxx"
     vite = Vite(app)
     npm = vite.npm
```

### Comparing `flask_vite-0.3.8/PKG-INFO` & `flask_vite-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-vite
-Version: 0.3.8
+Version: 0.3.9
 Summary: Flask+Vite integration.
 Home-page: https://github.com/abilian/flask-vite
 Author: Abilian SAS
 Author-email: contact@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

