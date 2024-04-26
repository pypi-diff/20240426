# Comparing `tmp/DXEntity-0.1.7.tar.gz` & `tmp/dxentity-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXEntity-0.1.7.tar", last modified: Wed Jan 24 19:14:25 2024, max compression
+gzip compressed data, was "dxentity-0.1.8.tar", last modified: Fri Apr 26 01:56:19 2024, max compression
```

## Comparing `DXEntity-0.1.7.tar` & `dxentity-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-01-24 19:14:25.008027 DXEntity-0.1.7/
--rw-r--r--   0 fred       (501) staff       (20)       56 2023-12-26 00:53:47.000000 DXEntity-0.1.7/.flake8
--rw-r--r--   0 fred       (501) staff       (20)      125 2023-12-22 01:56:16.000000 DXEntity-0.1.7/.git_archival.txt
--rw-r--r--   0 fred       (501) staff       (20)       31 2023-12-22 01:56:54.000000 DXEntity-0.1.7/.gitattributes
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-01-24 19:14:25.005444 DXEntity-0.1.7/.github/
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-01-24 19:14:25.006675 DXEntity-0.1.7/.github/workflows/
--rw-r--r--   0 fred       (501) staff       (20)      574 2023-12-21 23:11:31.000000 DXEntity-0.1.7/.github/workflows/pylint.yml
--rw-r--r--   0 fred       (501) staff       (20)     1920 2023-12-22 01:57:12.000000 DXEntity-0.1.7/.gitignore
--rw-r--r--   0 fred       (501) staff       (20)      611 2024-01-24 15:22:40.000000 DXEntity-0.1.7/.pre-commit-config.yaml
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-01-24 19:14:25.007100 DXEntity-0.1.7/DXEntity/
--rw-r--r--   0 fred       (501) staff       (20)      360 2023-12-26 00:59:06.000000 DXEntity-0.1.7/DXEntity/__init__.py
--rw-r--r--   0 fred       (501) staff       (20)     4018 2024-01-24 19:01:13.000000 DXEntity-0.1.7/DXEntity/_dxentity.py
--rw-r--r--   0 fred       (501) staff       (20)      411 2024-01-24 19:14:24.000000 DXEntity-0.1.7/DXEntity/_version.py
--rw-r--r--   0 fred       (501) staff       (20)        0 2023-12-26 02:02:25.000000 DXEntity-0.1.7/DXEntity/py.typed
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-01-24 19:14:25.007645 DXEntity-0.1.7/DXEntity.egg-info/
--rw-r--r--   0 fred       (501) staff       (20)     2831 2024-01-24 19:14:24.000000 DXEntity-0.1.7/DXEntity.egg-info/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)      356 2024-01-24 19:14:25.000000 DXEntity-0.1.7/DXEntity.egg-info/SOURCES.txt
--rw-r--r--   0 fred       (501) staff       (20)        1 2024-01-24 19:14:24.000000 DXEntity-0.1.7/DXEntity.egg-info/dependency_links.txt
--rw-r--r--   0 fred       (501) staff       (20)        9 2024-01-24 19:14:24.000000 DXEntity-0.1.7/DXEntity.egg-info/top_level.txt
--rw-r--r--   0 fred       (501) staff       (20)     1498 2023-12-21 19:25:15.000000 DXEntity-0.1.7/LICENSE
--rw-r--r--   0 fred       (501) staff       (20)     2831 2024-01-24 19:14:25.007857 DXEntity-0.1.7/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)      321 2023-12-22 00:27:53.000000 DXEntity-0.1.7/README.md
--rw-r--r--   0 fred       (501) staff       (20)    20257 2023-12-21 19:20:49.000000 DXEntity-0.1.7/pylintrc
--rw-r--r--   0 fred       (501) staff       (20)     1040 2023-12-25 23:40:01.000000 DXEntity-0.1.7/pyproject.toml
--rw-r--r--   0 fred       (501) staff       (20)       38 2024-01-24 19:14:25.008065 DXEntity-0.1.7/setup.cfg
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-26 01:56:19.101929 dxentity-0.1.8/
+-rw-r--r--   0 fred       (501) staff       (20)       56 2023-12-26 00:53:47.000000 dxentity-0.1.8/.flake8
+-rw-r--r--   0 fred       (501) staff       (20)      125 2023-12-22 01:56:16.000000 dxentity-0.1.8/.git_archival.txt
+-rw-r--r--   0 fred       (501) staff       (20)       31 2023-12-22 01:56:54.000000 dxentity-0.1.8/.gitattributes
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-26 01:56:19.098300 dxentity-0.1.8/.github/
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-26 01:56:19.100353 dxentity-0.1.8/.github/workflows/
+-rw-r--r--   0 fred       (501) staff       (20)      794 2024-04-26 01:31:07.000000 dxentity-0.1.8/.github/workflows/main.yaml
+-rw-r--r--   0 fred       (501) staff       (20)     1920 2024-02-15 17:05:04.000000 dxentity-0.1.8/.gitignore
+-rw-r--r--   0 fred       (501) staff       (20)      611 2024-04-26 01:31:07.000000 dxentity-0.1.8/.pre-commit-config.yaml
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-26 01:56:19.101052 dxentity-0.1.8/DXEntity/
+-rw-r--r--   0 fred       (501) staff       (20)      360 2023-12-26 00:59:06.000000 dxentity-0.1.8/DXEntity/__init__.py
+-rw-r--r--   0 fred       (501) staff       (20)     4208 2024-04-26 01:44:38.000000 dxentity-0.1.8/DXEntity/_dxentity.py
+-rw-r--r--   0 fred       (501) staff       (20)      411 2024-04-26 01:56:19.000000 dxentity-0.1.8/DXEntity/_version.py
+-rw-r--r--   0 fred       (501) staff       (20)        0 2023-12-26 02:02:25.000000 dxentity-0.1.8/DXEntity/py.typed
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-26 01:56:19.101539 dxentity-0.1.8/DXEntity.egg-info/
+-rw-r--r--   0 fred       (501) staff       (20)     2831 2024-04-26 01:56:19.000000 dxentity-0.1.8/DXEntity.egg-info/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)      355 2024-04-26 01:56:19.000000 dxentity-0.1.8/DXEntity.egg-info/SOURCES.txt
+-rw-r--r--   0 fred       (501) staff       (20)        1 2024-04-26 01:56:19.000000 dxentity-0.1.8/DXEntity.egg-info/dependency_links.txt
+-rw-r--r--   0 fred       (501) staff       (20)        9 2024-04-26 01:56:19.000000 dxentity-0.1.8/DXEntity.egg-info/top_level.txt
+-rw-r--r--   0 fred       (501) staff       (20)     1498 2023-12-21 19:25:15.000000 dxentity-0.1.8/LICENSE
+-rw-r--r--   0 fred       (501) staff       (20)     2831 2024-04-26 01:56:19.101749 dxentity-0.1.8/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)      321 2023-12-22 00:27:53.000000 dxentity-0.1.8/README.md
+-rw-r--r--   0 fred       (501) staff       (20)    20257 2023-12-21 19:20:49.000000 dxentity-0.1.8/pylintrc
+-rw-r--r--   0 fred       (501) staff       (20)     1039 2024-04-26 01:31:26.000000 dxentity-0.1.8/pyproject.toml
+-rw-r--r--   0 fred       (501) staff       (20)       38 2024-04-26 01:56:19.101964 dxentity-0.1.8/setup.cfg
```

### Comparing `DXEntity-0.1.7/.github/workflows/pylint.yml` & `dxentity-0.1.8/.github/workflows/main.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-name: Pylint
+name: Check code
 
 on: [push]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.10"]
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install pylint
-    - name: Analysing the code with pylint
+        pip install pylint isort flake8
+    - name: Lint check
+      continue-on-error: false
       run: |
-        pylint DXEntity/__init__.py
-        pylint DXEntity/_dxentity.py
+        pylint $(git ls-files "*.py")
+    - name: Running flake8
+      continue-on-error: false
+      run: |
+        flake8 $(git ls-files "*.py")
+    - name: Checking imports
+      continue-on-error: false
+      run: |
+        isort --check $(git ls-files "*.py")
```

### Comparing `DXEntity-0.1.7/.gitignore` & `dxentity-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `DXEntity-0.1.7/.pre-commit-config.yaml` & `dxentity-0.1.8/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -11,11 +11,11 @@
       - id: check-yaml
       - id: debug-statements
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 7.0.0
     hooks:
       - id: flake8
         args: [--max-line-length=100, --indent-size=2, --ignore=E231]
```

### Comparing `DXEntity-0.1.7/DXEntity/_dxentity.py` & `dxentity-0.1.8/DXEntity/_dxentity.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,29 @@
 # pylint: disable=invalid-name
 
 import dbm
 import logging
 import marshal
 import plistlib
 import time
-import urllib
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import _CacheInfo, _lru_cache_wrapper, lru_cache
 from pathlib import Path
-from typing import Callable, DefaultDict, Dict
+from typing import Callable, DefaultDict, TypeAlias, cast
+from urllib import request
+
+Buffer: TypeAlias = bytes
 
 CTY_URL: str = "https://www.country-files.com/cty/cty.plist"
-CTY_DB: str = Path.home() / ".local/cty"
+CTY_DB: Path = Path.home() / ".local/cty"
 CTY_EXPIRE: int = 86400 * 7          # One week
 
+ZERO = b'\xe9\x00\x00\x00\x00'
+
 LRU_CACHE_SIZE: int = 2048
 TRANSLATOR = ''.maketrans(
   'abcdefghijklmnopqrstuvwxyz',
   'ABCDEFGHIJKLMNOPQRSTUVWXYZ',
   ' !"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
 )
 
@@ -58,20 +62,20 @@
 
   def __init__(self, db_path: Path = CTY_DB, cache_size: int = LRU_CACHE_SIZE,
                cache_expire: int = CTY_EXPIRE) -> None:
     if not db_path.parent.exists():
       db_path.parent.mkdir(parents=True)
 
     self._max_len: int = 0
-    self.lookup: CACHE_TYPE = lru_cache(maxsize=cache_size)(self._get_prefix)
+    self._lookup: CACHE_TYPE = lru_cache(maxsize=cache_size)(self._get_prefix)
     self._db: str = str(db_path)
 
     try:
       with dbm.open(self._db, 'r') as cdb:
-        age = marshal.loads(cdb.get('__age__', 0))
+        age = marshal.loads(cdb.get('__age__', ZERO))
     except dbm.error:
       age = 0
       logging.error('DXEntity cache not found or expired')
 
     if age + cache_expire > time.time():
       try:
         logging.info('Using DXCC cache %s', self._db)
@@ -79,15 +83,15 @@
           self._max_len = marshal.loads(cdb['__max_len__'])
         return
       except dbm.error as err:
         logging.error('DXEntity cache error: %s', err)
 
     logging.info('Download %s', CTY_URL)
 
-    with urllib.request.urlopen(CTY_URL) as result:
+    with request.urlopen(CTY_URL) as result:
       raw_data = result.read()
       cty_data = plistlib.loads(raw_data)
     self._max_len = max(len(k) for k in cty_data)
 
     logging.info('Create cty cache: %s', self._db)
     entities: DefaultDict[str, set] = defaultdict(set)
     with dbm.open(self._db, 'c') as cdb:
@@ -95,38 +99,42 @@
         cdb[key] = marshal.dumps(val)
         country = val['Country'].translate(TRANSLATOR)
         entities[country].add(key)
       cdb['__age__'] = marshal.dumps(int(time.time()))
       cdb['__max_len__'] = marshal.dumps(self._max_len)
       cdb['__entities__'] = marshal.dumps(dict(entities))
 
-  def _get_prefix(self, call: str) -> DXCCRecord:
+  def lookup(self, call: str) -> DXCCRecord:
     call = call.upper()
+    return self._lookup(call)
+
+  def _get_prefix(self, call: str) -> DXCCRecord:
     prefixes = list({call[:c] for c in range(self._max_len, 0, -1)})
     prefixes.sort(key=lambda x: -len(x))
     with dbm.open(self._db, 'r') as cdb:
       for prefix in prefixes:
         if prefix in cdb:
           return DXCCRecord(**marshal.loads(cdb[prefix]))
     raise KeyError(f"{call} not found")
 
   def cache_info(self) -> CacheInfo:
     # pylint: disable=no-member
-    return self.lookup.cache_info()  # type: ignore
+    return self._lookup.cache_info()  # type: ignore
 
   def isentity(self, country: str) -> bool:
     country = country.translate(TRANSLATOR)
     if country in self.entities:
       return True
     return False
 
   @property
-  def entities(self) -> Dict[str, set]:
+  def entities(self) -> dict[str, set]:
     with dbm.open(self._db, 'r') as cdb:
-      return marshal.loads(cdb.get('__entities__'))
+      ret = cdb.get('__entities__')
+      return marshal.loads(cast('Buffer', ret))
 
   def get_entity(self, key: str) -> set:
     _entities = self.entities
     _key = key.translate(TRANSLATOR)
     if _key in _entities:
       return _entities[_key]
     raise KeyError(f'Entity {key} not found')
```

### Comparing `DXEntity-0.1.7/DXEntity.egg-info/PKG-INFO` & `dxentity-0.1.8/DXEntity.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DXEntity
-Version: 0.1.7
+Version: 0.1.8
 Summary: The DXEntity API return location information for an amateur radio call sign.
 Author: Fred C.
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Fred Cirera
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `DXEntity-0.1.7/LICENSE` & `dxentity-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `DXEntity-0.1.7/PKG-INFO` & `dxentity-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DXEntity
-Version: 0.1.7
+Version: 0.1.8
 Summary: The DXEntity API return location information for an amateur radio call sign.
 Author: Fred C.
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Fred Cirera
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `DXEntity-0.1.7/pylintrc` & `dxentity-0.1.8/pylintrc`

 * *Files identical despite different names*

### Comparing `DXEntity-0.1.7/pyproject.toml` & `dxentity-0.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -24,11 +24,10 @@
         "Programming Language :: Python",
         "Topic :: Communications :: Ham Radio",
     ]
 
 [tool.setuptools_scm]
     write_to = "DXEntity/_version.py"
 
-
 [project.urls]
     Source = "https://github.com/0x9900/DXEntity"
     Tracker = "https://github.com/0x9900/DXEntity/issues"
```

