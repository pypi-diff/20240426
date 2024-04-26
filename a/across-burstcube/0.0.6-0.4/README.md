# Comparing `tmp/across_burstcube-0.0.6.tar.gz` & `tmp/across_burstcube-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "across_burstcube-0.0.6.tar", last modified: Fri Apr 26 21:14:54 2024, max compression
+gzip compressed data, was "across_burstcube-0.4.tar", last modified: Fri Apr 19 18:58:37 2024, max compression
```

## Comparing `across_burstcube-0.0.6.tar` & `across_burstcube-0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:54.739172 across_burstcube-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:54.735172 across_burstcube-0.0.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:54.735172 across_burstcube-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-26 21:14:54.739172 across_burstcube-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:54.739172 across_burstcube-0.0.6/across_burstcube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-26 21:14:54.000000 across_burstcube-0.0.6/across_burstcube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-26 21:14:54.000000 across_burstcube-0.0.6/across_burstcube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:14:54.000000 across_burstcube-0.0.6/across_burstcube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-26 21:14:54.000000 across_burstcube-0.0.6/across_burstcube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 21:14:54.000000 across_burstcube-0.0.6/across_burstcube.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:54.735172 across_burstcube-0.0.6/across_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:54.735172 across_burstcube-0.0.6/across_client/across/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/across/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/across/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/across/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:54.739172 across_burstcube-0.0.6/across_client/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/base/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/base/coords.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/base/daterange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/base/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/base/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:54.739172 across_burstcube-0.0.6/across_client/burstcube/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/burstcube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/burstcube/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/burstcube/fov.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/burstcube/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/burstcube/toorequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/across_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-26 21:14:49.000000 across_burstcube-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:14:54.739172 across_burstcube-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.469876 across_burstcube-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.461876 across_burstcube-0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.461876 across_burstcube-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 18:58:32.000000 across_burstcube-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 18:58:32.000000 across_burstcube-0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 18:58:37.469876 across_burstcube-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-19 18:58:32.000000 across_burstcube-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_burstcube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/across/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/daterange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/burstcube/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/fov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/toorequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-19 18:58:32.000000 across_burstcube-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:58:37.469876 across_burstcube-0.4/setup.cfg
```

### Comparing `across_burstcube-0.0.6/.github/ISSUE_TEMPLATE.md` & `across_burstcube-0.4/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.6/.github/PULL_REQUEST_TEMPLATE.md` & `across_burstcube-0.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.6/.github/workflows/deploy.yml` & `across_burstcube-0.4/.github/workflows/deploy.yml`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
       - name: Checkout the repository
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
           python-version: "3.11"
 
       - name: Git describe
         id: ghd
         uses: proudust/gh-describe@v2
 
@@ -30,15 +30,15 @@
           build
           --user
 
       - name: Build a binary wheel and a source tarball
         run: python3 -m build
 
       - name: Store the distribution packages
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
 
   publish-to-pypi:
     name: >-
       Publish Python 🐍 distribution 📦 to PyPI
@@ -49,13 +49,13 @@
     environment:
       name: pypi
       url: https://pypi.org/p/across-burstcube  # Replace <package-name> with your PyPI project name
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
     steps:
       - name: Download all the dists
-        uses: actions/download-artifact@v4
+        uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
       - name: Publish distribution 📦 to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `across_burstcube-0.0.6/.github/workflows/pylint.yml` & `across_burstcube-0.4/.github/workflows/pylint.yml`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 on: [push]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.9", "3.10", "3.11"]
     steps:
-    - uses: actions/checkout@v4
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v5
+      uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install flake8 mypy
     - name: Lint with flake8
```

### Comparing `across_burstcube-0.0.6/across_burstcube.egg-info/SOURCES.txt` & `across_burstcube-0.4/across_burstcube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.6/across_client/across/resolve.py` & `across_burstcube-0.4/across_client/across/resolve.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from ..base.common import ACROSSBase
 from .schema import ResolveGetSchema, ResolveSchema
 
 
-class Resolve(ACROSSBase, ResolveSchema):
+class Resolve(ACROSSBase):
     """
     Represents a resolver for resolving celestial object coordinates.
 
     Attributes
     ----------
     name : Optional[str]
         The name of the celestial object.
@@ -16,19 +16,30 @@
         The right ascension of the celestial object.
     dec : Optional[float]
         The declination of the celestial object.
     resolver : Optional[str]
         The resolver used for resolving the coordinates.
     """
 
+    # Type hints
+    name: Optional[str] = None
+    ra: Optional[float] = None
+    dec: Optional[float] = None
+    resolver: Optional[str] = None
+
     _mission = "ACROSS"
     _api_name = "Resolve"
     _schema = ResolveSchema
     _get_schema = ResolveGetSchema
 
+    def __init__(self, name: Optional[str] = None, **kwargs):
+        self.name = name
+        for k, a in kwargs.items():
+            setattr(self, k, a)
+
 
 class ACROSSResolveName:
     """_summary_
 
     Returns
     -------
     _type_
```

### Comparing `across_burstcube-0.0.6/across_client/across/schema.py` & `across_burstcube-0.4/across_client/across/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 
 
 class ResolveSchema(BaseSchema):
     """
     A schema for resolving astronomical coordinates.
     """
 
-    name: Optional[str] = None
-    ra: Optional[float] = None
-    dec: Optional[float] = None
-    resolver: Optional[str] = None
+    ra: float
+    dec: float
+    resolver: str
 
 
 class ResolveGetSchema(BaseSchema):
     """Schema defines required parameters for a GET"""
 
     name: str
```

### Comparing `across_burstcube-0.0.6/across_client/base/common.py` & `across_burstcube-0.4/across_client/base/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 class ACROSSBase:
     """
     Base class for ACROSS API Classes including common methods for all API classes.
     """
 
     # Type hints
-    # entries: list
+    entries: list
 
     # API descriptors type hints
     _schema: Type[BaseSchema]
     _get_schema: Type[BaseSchema]
     _put_schema: Type[BaseSchema]
     _post_schema: Type[BaseSchema]
     _del_schema: Type[BaseSchema]
 
     _mission: str
-    _api_name: str
+    _api_name: str = __name__
 
     def __getitem__(self, i):
         return self.entries[i]
 
     def api_url(self, argdict) -> str:
         """
         URL for this API call.
@@ -41,24 +41,24 @@
             URL for API call
         """
         # If arguments has `id` in it, then put this in the path
         if "id" in argdict.keys() and argdict["id"] is not None:
             return f"{API_URL}{self._mission.lower()}/{self._api_name.lower()}/{argdict['id']}"
         return f"{API_URL}{self._mission.lower()}/{self._api_name.lower()}"
 
-    # @property
-    # def schema(self) -> Any:
-    #     """Return pydantic schema for this API class
-
-    #     Returns
-    #     -------
-    #     object
-    #         Pydantic Schema
-    #     """
-    #     return self._schema.model_validate(self)
+    @property
+    def schema(self) -> Any:
+        """Return pydantic schema for this API class
+
+        Returns
+        -------
+        object
+            Pydantic Schema
+        """
+        return self._schema.model_validate(self)
 
     @property
     def parameters(self) -> dict:
         """
         Return parameters as dict
 
         Returns
@@ -105,27 +105,23 @@
         ------
         HTTPError
             Raised if GET doesn't return a 200 response.
         """
         if self.validate_get():
             # Create an array of parameters from the schema
             get_params = {
-                key: value
-                for key, value in self._get_schema.model_validate(self)
-                if key in self._get_schema.model_fields
+                key: value for key, value in self._get_schema.model_validate(self)
             }
-
             # Do the GET request
             req = requests.get(
                 self.api_url(get_params),
                 params=get_params,
                 headers=self.headers,
                 timeout=60,
             )
-            print(req.request.url)
             if req.status_code == 200:
                 # Parse, validate and record values from returned API JSON
                 for k, v in self._schema.model_validate(req.json()):
                     setattr(self, k, v)
                 return True
             elif req.status_code == 404:
                 """Handle 404 errors gracefully, by issuing a warning"""
@@ -237,18 +233,14 @@
             )
 
             if req.status_code == 201:
                 # Parse, validate and record values from returned API JSON
                 for k, v in self._schema.model_validate(req.json()):
                     setattr(self, k, v)
                 return True
-            elif req.status_code == 304:
-                # No changes made
-                warnings.warn("Update identical to values on server. No changes made.")
-                return False
             else:
                 print("ERROR: ", req.status_code, req.json())
                 req.raise_for_status()
         return False
 
     def post(self) -> bool:
         """
```

### Comparing `across_burstcube-0.0.6/across_client/base/coords.py` & `across_burstcube-0.4/across_client/base/coords.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.6/across_client/base/daterange.py` & `across_burstcube-0.4/across_client/base/daterange.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.6/across_client/base/schema.py` & `across_burstcube-0.4/across_client/base/schema.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.6/across_client/burstcube/schema.py` & `across_burstcube-0.4/across_client/burstcube/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,27 +87,25 @@
 
 class BurstCubeTOOSchema(OptionalPositionSchema):
     """
     Schema describing a BurstCube TOO Request.
     """
 
     id: Optional[int] = None
-    created_by: Optional[str] = None
-    created_on: Optional[datetime] = None
+    created_by: str
+    created_on: datetime
     modified_by: Optional[str] = None
     modified_on: Optional[datetime] = None
-    trigger_time: Optional[datetime] = None
-    trigger_info: Optional[BurstCubeTriggerInfo] = None
-    exposure: int = 200
-    offset: int = -50
+    trigger_time: datetime
+    trigger_info: BurstCubeTriggerInfo
+    exposure: int
+    offset: int
     reject_reason: TOOReason = TOOReason.none
     status: TOOStatus = TOOStatus.requested
     too_info: str = ""
-    healpix_filename: Optional[str] = None
-    version: Optional[int] = None
 
 
 class BurstCubeTOODelSchema(BaseSchema):
     """
     Schema for BurstCubeTOO DELETE API call.
 
     Attributes
@@ -159,13 +157,13 @@
     """
 
     duration: Optional[float] = None
     limit: Optional[int] = None
     offset: Optional[int] = None
 
 
-class BurstCubeTOORequestsSchema(BurstCubeTOORequestsGetSchema):
+class BurstCubeTOORequestsSchema(BaseSchema):
     """
     Schema for BurstCube TOO requests.
     """
 
-    entries: List[BurstCubeTOOSchema] = []
+    entries: List[BurstCubeTOOSchema]
```

### Comparing `across_burstcube-0.0.6/across_client/burstcube/toorequest.py` & `across_burstcube-0.4/across_client/burstcube/toorequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-from datetime import datetime
 import io
-from typing import Any, Optional, Union
+from dataclasses import dataclass, field
+from datetime import datetime
+from typing import Optional, Union
 
-from pydantic import model_validator
+from pydantic import FilePath
 
 from ..across.resolve import ACROSSResolveName
 from ..base.common import ACROSSBase
 from .constants import MISSION
 from .schema import (
     BurstCubeTOOGetSchema,
     BurstCubeTOOPostSchema,
     BurstCubeTOOPutSchema,
     BurstCubeTOORequestsGetSchema,
     BurstCubeTOORequestsSchema,
     BurstCubeTOOSchema,
+    BurstCubeTriggerInfo,
+    TOOReason,
+    TOOStatus,
 )
 
 
-class BurstCubeTOO(ACROSSBase, ACROSSResolveName, BurstCubeTOOSchema):
+@dataclass
+class TOO(ACROSSBase, ACROSSResolveName):
     """
     Class representing a Target of Opportunity (TOO) request.
 
     Parameters:
     ----------
     api_token: str
         The api_token for login (optional).
@@ -68,37 +73,55 @@
         The reason for the TOO request being rejected.
     status : str
         The status of the TOO request.
     too_info : str
         The information about the TOO request.
     id : str
         The ID of the TOO request.
-    version : int
-        The version of the TOO request.
     """
 
+    api_token: Optional[str] = None
+    id: Optional[int] = None
+    trigger_time: Optional[datetime] = None
+    created_by: Optional[str] = None
+    created_on: Optional[datetime] = None
+    modified_by: Optional[str] = None
+    modified_on: Optional[datetime] = None
+    trigger_info: BurstCubeTriggerInfo = field(default_factory=BurstCubeTriggerInfo)
+    exposure: float = 200
+    offset: float = -50
+    too_info: str = ""
+    ra: Optional[float] = None
+    dec: Optional[float] = None
+    error_radius: Optional[float] = None
+    healpix_filename: Optional[FilePath] = None
+    healpix_file: Union[io.BytesIO, io.BufferedReader, None] = None
+    reject_reason: TOOReason = TOOReason.none
+    status: TOOStatus = TOOStatus.requested
+
     # API definitions
     _mission = MISSION
     _api_name = "TOO"
     _schema = BurstCubeTOOSchema
     _put_schema = BurstCubeTOOPutSchema
     _post_schema = BurstCubeTOOPostSchema
     _get_schema = BurstCubeTOOGetSchema
     _del_schema = BurstCubeTOOGetSchema
 
-    # Local parameters
-    healpix_file: Union[io.BytesIO, io.BufferedReader, None] = None
-    api_token: Optional[str] = None
-
-    # Aliases
-    def submit(self):
-        self.post()
+    @classmethod
+    def submit_too(cls, **kwargs):
+        """
+        Submit a TOO request.
+        """
+        for k, a in kwargs.items():
+            if k in cls._post_schema.model_fields.keys():
+                setattr(cls, k, a)
 
-    def update(self):
-        self.put()
+        if cls.validate_post():
+            cls.post()
 
     @property
     def _table(self):
         return (
             [
                 "TOO ID",
                 "Submitted",
@@ -122,68 +145,61 @@
                     self.status.value,
                     self.reject_reason.value,
                 ]
             ],
         )
 
 
-class TOORequests(ACROSSBase, BurstCubeTOORequestsSchema):
+class TOORequests(ACROSSBase):
     """
     Represents a Targer of Opportunity (TOO) request.
 
-    Parameters
+    Attributes
     ----------
-    trigger_time : datetime
-        Trigger time of the TOO request.
     begin : datetime
         The start time of the observation.
     end : datetime
         The end time of the observation.
     limit : int
-        The maximum number of TOOs to return.
-    offset : int
-        The limit offset for fetching TOOs.
-
-    Attributes
-    ----------
+        The maximum number of entries for the observation.
+    trigger_time : datetime
+        The time at which the observation should be triggered.
     entries : list
         The list of entries for the observation.
     """
 
-    # API definitions
     _mission = MISSION
     _api_name = "TOO"
     _schema = BurstCubeTOORequestsSchema
     _get_schema = BurstCubeTOORequestsGetSchema
-    # Local parameters
-    trigger_time: Optional[datetime] = None
 
-    def __len__(self):
-        return len(self.entries)
+    def __init__(self, **kwargs):
+        self.entries = []
+        self.begin = None
+        self.end = None
+        self.limit = None
+        for k, a in kwargs.items():
+            if k in self._get_schema.model_fields.keys():
+                setattr(self, k, a)
+
+        # As this is a GET only class, we can validate and get the data
+        if self.validate_get():
+            self.get()
 
-    def __getitem__(self, i):
-        return self.entries[i]
+        # Convert the entries to a list of TOO objects
+        self.entries = [TOO(**entry.__dict__) for entry in self.entries]
 
     def by_id(self, id):
         """
         Get a TOO request by ID.
         """
         for entry in self.entries:
             if entry.id == id:
                 return entry
 
-    @model_validator(mode="before")
-    @classmethod
-    def check_card_number_omitted(cls, data: Any) -> Any:
-        if isinstance(data, dict):
-            if "trigger_time" in data and data["trigger_time"] is not None:
-                data["begin"] = data["trigger_time"]
-                data["end"] = data["trigger_time"]
-        return data
-
     @property
     def _table(self):
         return (
             [
                 "TOO ID",
                 "Submitted",
                 "Submitter",
@@ -206,83 +222,13 @@
                     entry.status.value,
                     entry.reject_reason.value,
                 ]
                 for entry in self.entries
             ],
         )
 
-    @classmethod
-    def get_toos(cls, *args, **kwargs):
-        """
-        Fetch TOOs based on various criteria.
-
-        Parameters
-        ----------
-        trigger_time : datetime
-            Trigger time of the TOO request.
-        begin : datetime
-            Beginning trigger time to search.
-        end : datetime
-            Ending trigger time to search.
-        limit : int
-            The maximum number of TOOs to return.
-        offset : int
-            The limit offset for fetching TOOs.
-
-        Returns
-        ----------
-        TOORequests
-            The list of entries for the observation.
-        """
-        too_requests = cls(*args, **kwargs)
-        too_requests.get()
-        return too_requests
-
-
-def get_too_by_id(id: int) -> BurstCubeTOO:
-    """
-    Get a TOO request by ID.
-
-    Parameters
-    ----------
-    id : int
-        The ID of the TOO request.
-    api_token : str
-        The API token for the user.
-
-    Returns
-    -------
-    BurstCubeTOO
-        The TOO request.
-    """
-    too = BurstCubeTOO(id=id)
-    too.get()
-    return too
-
-
-def get_too_by_trigger_time(trigger_time: datetime) -> Optional[BurstCubeTOO]:
-    """
-    Get a TOO request by timestamp.
-
-    Parameters
-    ----------
-    timestamp : str
-        The timestamp of the TOO request.
-    api_token : str
-        The API token for the user.
-
-    Returns
-    -------
-    BurstCubeTOO
-        The TOO request.
-    """
-    too = TOORequests(trigger_time=trigger_time)
-    too.get()
-    if len(too) > 0:
-        return too[0]
-    return None
-
 
 # Alias
-TOO = BurstCubeTOO
+BurstCubeTOO = TOO
 BurstCubeTOORequests = TOORequests
-get_too_requests = TOORequests.get_toos
+submit_too = TOO.submit_too
+burstcube_submit_too = TOO.submit_too
```

### Comparing `across_burstcube-0.0.6/across_client/functions.py` & `across_burstcube-0.4/across_client/functions.py`

 * *Files identical despite different names*

