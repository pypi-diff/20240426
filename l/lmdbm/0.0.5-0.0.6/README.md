# Comparing `tmp/lmdbm-0.0.5.tar.gz` & `tmp/lmdbm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmdbm-0.0.5.tar", last modified: Thu Sep 30 09:38:45 2021, max compression
+gzip compressed data, was "lmdbm-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lmdbm-0.0.5.tar` & `lmdbm-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 09:38:45.471104 lmdbm-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     4849 2021-09-30 09:38:45.471104 lmdbm-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 09:38:45.471104 lmdbm-0.0.5/lmdbm/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-09-30 09:38:43.000000 lmdbm-0.0.5/lmdbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9330 2021-09-30 09:38:43.000000 lmdbm-0.0.5/lmdbm/lmdbm.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 09:38:43.000000 lmdbm-0.0.5/lmdbm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 09:38:45.471104 lmdbm-0.0.5/lmdbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4849 2021-09-30 09:38:45.000000 lmdbm-0.0.5/lmdbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      249 2021-09-30 09:38:45.000000 lmdbm-0.0.5/lmdbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-30 09:38:45.000000 lmdbm-0.0.5/lmdbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-09-30 09:38:45.000000 lmdbm-0.0.5/lmdbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-30 09:38:45.000000 lmdbm-0.0.5/lmdbm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-30 09:38:45.000000 lmdbm-0.0.5/lmdbm.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      190 2021-09-30 09:38:43.000000 lmdbm-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      753 2021-09-30 09:38:45.471104 lmdbm-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-09-30 09:38:43.000000 lmdbm-0.0.5/setup.py
+-rw-r--r--   0        0        0      213 2024-04-26 15:11:02.586946 lmdbm-0.0.6/lmdbm/__init__.py
+-rw-r--r--   0        0        0     9026 2024-04-26 15:11:02.586946 lmdbm-0.0.6/lmdbm/lmdbm.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:11:02.586946 lmdbm-0.0.6/lmdbm/py.typed
+-rw-r--r--   0        0        0     1294 2024-04-26 15:11:02.586946 lmdbm-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3729 2024-04-26 15:11:02.586946 lmdbm-0.0.6/readme.md
+-rw-r--r--   0        0        0     5151 1970-01-01 00:00:00.000000 lmdbm-0.0.6/PKG-INFO
```

### Comparing `lmdbm-0.0.5/PKG-INFO` & `lmdbm-0.0.6/readme.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,68 @@
-Metadata-Version: 2.1
-Name: lmdbm
-Version: 0.0.5
-Summary: Python DBM style wrapper around LMDB (Lightning Memory-Mapped Database)
-Home-page: https://github.com/Dobatymo/lmdb-python-dbm
-Author: Dobatymo
-License: UNKNOWN
-Description: # lmdbm
-        
-        This is a Python DBM interface style wrapper around [LMDB](http://www.lmdb.tech/doc/) (Lightning Memory-Mapped Database).
-        It uses the existing lower level Python bindings [py-lmdb](https://lmdb.readthedocs.io).
-        This is especially useful on Windows, where otherwise `dbm.dumb` is the default `dbm` database.
-        
-        ## Install
-        - `pip install lmdbm`
-        
-        ## Example
-        ```python
-        from lmdbm import Lmdb
-        with Lmdb.open("test.db", "c") as db:
-          db[b"key"] = b"value"
-          db.update({b"key1": b"value1", b"key2": b"value2"})  # batch insert, uses a single transaction
-        ```
-        
-        ### Use inheritance to store Python objects using json serialization
-        
-        ```python
-        import json
-        from lmdbm import Lmdb
-        
-        class JsonLmdb(Lmdb):
-          def _pre_key(self, value):
-            return value.encode("utf-8")
-          def _post_key(self, value):
-            return value.decode("utf-8")
-          def _pre_value(self, value):
-            return json.dumps(value).encode("utf-8")
-          def _post_value(self, value):
-            return json.loads(value.decode("utf-8"))
-        
-        with JsonLmdb.open("test.db", "c") as db:
-          db["key"] = {"some": "object"}
-          obj = db["key"]
-          print(obj["some"])  # prints "object"
-        ```
-        
-        ## Warning
-        
-        As of `lmdb==1.2.1` the docs say that calling `lmdb.Environment.set_mapsize` from multiple processes "may cause catastrophic loss of data". If `lmdbm` is used in write mode from multiple processes, set `autogrow=False` and map_size to a large enough value: `Lmdb.open(..., map_size=2**30, autogrow=False)`.
-        
-        ## Benchmarks
-        
-        See `benchmark.py` and `requirements-bench.txt`. Other storage engines which could be tested: `wiredtiger`, `berkeleydb`.
-        Storage engines not benchmarked:
-        	- `tinydb` (because it doesn't have built-in str/bytes keys)
-        
-        ### continuous writes in seconds (best of 3)
-        | items | lmdbm  |lmdbm-batch|pysos |sqlitedict|sqlitedict-batch|dbm.dumb|semidbm|vedis |vedis-batch|unqlite|unqlite-batch|
-        |------:|-------:|----------:|-----:|---------:|---------------:|-------:|------:|-----:|----------:|------:|------------:|
-        |     10|   0.000|      0.015| 0.000|     0.031|           0.000|   0.016|  0.000| 0.000|      0.000|  0.000|        0.000|
-        |    100|   0.094|      0.000| 0.000|     0.265|           0.016|   0.188|  0.000| 0.000|      0.000|  0.000|        0.000|
-        |   1000|   1.684|      0.016| 0.015|     3.885|           0.124|   2.387|  0.016| 0.015|      0.015|  0.016|        0.000|
-        |  10000|  16.895|      0.093| 0.265|    45.334|           1.326|  25.350|  0.156| 0.093|      0.094|  0.094|        0.093|
-        | 100000| 227.106|      1.030| 2.698|   461.638|          12.964| 238.400|  1.623| 1.388|      1.467|  1.466|        1.357|
-        |1000000|3482.520|     13.104|27.815|  5851.239|         133.396|2432.945| 16.411|15.693|     15.709| 14.508|       14.103|
-        
-        ### random reads in seconds (best of 3)
-        | items |lmdbm |lmdbm-batch|pysos |sqlitedict|sqlitedict-batch|dbm.dumb|semidbm| vedis |vedis-batch|unqlite|unqlite-batch|
-        |------:|-----:|-----------|-----:|---------:|----------------|-------:|------:|------:|-----------|------:|-------------|
-        |     10| 0.000|           | 0.000|     0.000|                |   0.000|  0.000|  0.000|           |  0.000|             |
-        |    100| 0.000|           | 0.000|     0.031|                |   0.000|  0.000|  0.000|           |  0.000|             |
-        |   1000| 0.016|           | 0.015|     0.250|                |   0.109|  0.016|  0.015|           |  0.000|             |
-        |  10000| 0.109|           | 0.156|     2.558|                |   1.123|  0.171|  0.109|           |  0.109|             |
-        | 100000| 1.014|           | 2.137|    27.769|                |  11.419|  2.090|  1.170|           |  1.170|             |
-        |1000000|10.390|           |24.258|   447.613|                | 870.580| 22.838|214.486|           |211.319|             |
-        
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Database
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: dev
+# lmdbm
+
+This is a Python DBM interface style wrapper around [LMDB](http://www.lmdb.tech/doc/) (Lightning Memory-Mapped Database).
+It uses the existing lower level Python bindings [py-lmdb](https://lmdb.readthedocs.io).
+This is especially useful on Windows, where otherwise `dbm.dumb` is the default `dbm` database.
+
+## Install
+- `pip install lmdbm`
+
+## Example
+```python
+from lmdbm import Lmdb
+with Lmdb.open("test.db", "c") as db:
+  db[b"key"] = b"value"
+  db.update({b"key1": b"value1", b"key2": b"value2"})  # batch insert, uses a single transaction
+```
+
+### Use inheritance to store Python objects using json serialization
+
+```python
+import json
+from lmdbm import Lmdb
+
+class JsonLmdb(Lmdb):
+  def _pre_key(self, value):
+    return value.encode("utf-8")
+  def _post_key(self, value):
+    return value.decode("utf-8")
+  def _pre_value(self, value):
+    return json.dumps(value).encode("utf-8")
+  def _post_value(self, value):
+    return json.loads(value.decode("utf-8"))
+
+with JsonLmdb.open("test.db", "c") as db:
+  db["key"] = {"some": "object"}
+  obj = db["key"]
+  print(obj["some"])  # prints "object"
+```
+
+## Warning
+
+As of `lmdb==1.2.1` the docs say that calling `lmdb.Environment.set_mapsize` from multiple processes "may cause catastrophic loss of data". If `lmdbm` is used in write mode from multiple processes, set `autogrow=False` and map_size to a large enough value: `Lmdb.open(..., map_size=2**30, autogrow=False)`.
+
+## Benchmarks
+
+See `benchmark.py` and `requirements-bench.txt`. Other storage engines which could be tested: `wiredtiger`, `berkeleydb`.
+Storage engines not benchmarked:
+	- `tinydb` (because it doesn't have built-in str/bytes keys)
+
+### continuous writes in seconds (best of 3)
+| items | lmdbm  |lmdbm-batch|pysos |sqlitedict|sqlitedict-batch|dbm.dumb|semidbm|vedis |vedis-batch|unqlite|unqlite-batch|
+|------:|-------:|----------:|-----:|---------:|---------------:|-------:|------:|-----:|----------:|------:|------------:|
+|     10|   0.000|      0.015| 0.000|     0.031|           0.000|   0.016|  0.000| 0.000|      0.000|  0.000|        0.000|
+|    100|   0.094|      0.000| 0.000|     0.265|           0.016|   0.188|  0.000| 0.000|      0.000|  0.000|        0.000|
+|   1000|   1.684|      0.016| 0.015|     3.885|           0.124|   2.387|  0.016| 0.015|      0.015|  0.016|        0.000|
+|  10000|  16.895|      0.093| 0.265|    45.334|           1.326|  25.350|  0.156| 0.093|      0.094|  0.094|        0.093|
+| 100000| 227.106|      1.030| 2.698|   461.638|          12.964| 238.400|  1.623| 1.388|      1.467|  1.466|        1.357|
+|1000000|3482.520|     13.104|27.815|  5851.239|         133.396|2432.945| 16.411|15.693|     15.709| 14.508|       14.103|
+
+### random reads in seconds (best of 3)
+| items |lmdbm |lmdbm-batch|pysos |sqlitedict|sqlitedict-batch|dbm.dumb|semidbm| vedis |vedis-batch|unqlite|unqlite-batch|
+|------:|-----:|-----------|-----:|---------:|----------------|-------:|------:|------:|-----------|------:|-------------|
+|     10| 0.000|           | 0.000|     0.000|                |   0.000|  0.000|  0.000|           |  0.000|             |
+|    100| 0.000|           | 0.000|     0.031|                |   0.000|  0.000|  0.000|           |  0.000|             |
+|   1000| 0.016|           | 0.015|     0.250|                |   0.109|  0.016|  0.015|           |  0.000|             |
+|  10000| 0.109|           | 0.156|     2.558|                |   1.123|  0.171|  0.109|           |  0.109|             |
+| 100000| 1.014|           | 2.137|    27.769|                |  11.419|  2.090|  1.170|           |  1.170|             |
+|1000000|10.390|           |24.258|   447.613|                | 870.580| 22.838|214.486|           |211.319|             |
```

### Comparing `lmdbm-0.0.5/lmdbm/lmdbm.py` & `lmdbm-0.0.6/lmdbm/lmdbm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,238 +1,197 @@
 import logging
 from collections.abc import Mapping, MutableMapping
 from gzip import compress, decompress
 from pathlib import Path
 from sys import exit
-from typing import TYPE_CHECKING
+from typing import Any, Generic, Iterator, List, Optional, Tuple, TypeVar, Union
 
 import lmdb
+from typing_extensions import Self
 
-if TYPE_CHECKING:
-    from typing import Any, Iterator, List, Optional, Tuple, TypeVar, Union
-
-    T = TypeVar("T")
-    KT = Union[bytes, str]  # TypeVar("KT")
-    VT = Union[bytes, str]  # TypeVar("VT")
+T = TypeVar("T")
+KT = TypeVar("KT")
+VT = TypeVar("VT")
 
 logger = logging.getLogger(__name__)
 
+_DEFAULT = object()
+
 
 class error(Exception):
     pass
 
 
-class MissingOk(object):
-
+class MissingOk:
     # for python < 3.8 compatibility
 
-    def __init__(self, ok):
-        # type: (bool, ) -> None
-
+    def __init__(self, ok: bool) -> None:
         self.ok = ok
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         if isinstance(exc_value, FileNotFoundError) and self.ok:
             return True
 
 
-def remove_lmdbm(file, missing_ok=True):
-    # type: (str, bool) -> None
-
+def remove_lmdbm(file: str, missing_ok: bool = True) -> None:
     base = Path(file)
     with MissingOk(missing_ok):
         (base / "data.mdb").unlink()
     with MissingOk(missing_ok):
         (base / "lock.mdb").unlink()
     with MissingOk(missing_ok):
         base.rmdir()
 
 
-class Lmdb(MutableMapping):
-
+class Lmdb(MutableMapping, Generic[KT, VT]):
     autogrow_error = "Failed to grow LMDB ({}). Is there enough disk space available?"
     autogrow_msg = "Grew database (%s) map size to %s"
 
-    def __init__(self, env, autogrow):
-        # type: (lmdb.Environment, bool) -> None
-
+    def __init__(self, env: lmdb.Environment, autogrow: bool) -> None:
         self.env = env
         self.autogrow = autogrow
 
     @classmethod
-    def open(cls, file, flag="r", mode=0o755, map_size=2 ** 20, autogrow=True):
-        # type: (str, str, int, int, bool) -> Lmdb
-
+    def open(
+        cls, file: str, flag: str = "r", mode: int = 0o755, map_size: int = 2**20, autogrow: bool = True, **kwargs
+    ) -> "Lmdb":
         """
         Opens the database `file`.
         `flag`: r (read only, existing), w (read and write, existing),
                 c (read, write, create if not exists), n (read, write, overwrite existing)
         `map_size`: Initial database size. Defaults to 2**20 (1MB).
         `autogrow`: Automatically grow the database size when `map_size` is exceeded.
                 WARNING: Set this to `False` for multi-process write access.
+        `**kwargs`: All other keyword arguments are passed through to `lmdb.open`.
         """
 
         if flag == "r":  # Open existing database for reading only (default)
-            env = lmdb.open(file, map_size=map_size, max_dbs=1, readonly=True, create=False, mode=mode)
+            env = lmdb.open(file, map_size=map_size, max_dbs=1, readonly=True, create=False, mode=mode, **kwargs)
         elif flag == "w":  # Open existing database for reading and writing
-            env = lmdb.open(file, map_size=map_size, max_dbs=1, readonly=False, create=False, mode=mode)
+            env = lmdb.open(file, map_size=map_size, max_dbs=1, readonly=False, create=False, mode=mode, **kwargs)
         elif flag == "c":  # Open database for reading and writing, creating it if it doesn't exist
-            env = lmdb.open(file, map_size=map_size, max_dbs=1, readonly=False, create=True, mode=mode)
+            env = lmdb.open(file, map_size=map_size, max_dbs=1, readonly=False, create=True, mode=mode, **kwargs)
         elif flag == "n":  # Always create a new, empty database, open for reading and writing
             remove_lmdbm(file)
-            env = lmdb.open(file, map_size=map_size, max_dbs=1, readonly=False, create=True, mode=mode)
+            env = lmdb.open(file, map_size=map_size, max_dbs=1, readonly=False, create=True, mode=mode, **kwargs)
         else:
             raise ValueError("Invalid flag")
 
         return cls(env, autogrow)
 
     @property
-    def map_size(self):
-        # type: () -> int
-
+    def map_size(self) -> int:
         return self.env.info()["map_size"]
 
     @map_size.setter
-    def map_size(self, value):
-        # type: (int, ) -> None
-
+    def map_size(self, value: int) -> None:
         self.env.set_mapsize(value)
 
-    def _pre_key(self, key):
-        # type: (object, ) -> bytes
-
+    def _pre_key(self, key: KT) -> bytes:
         if isinstance(key, bytes):
             return key
         elif isinstance(key, str):
             return key.encode("Latin-1")
 
-        raise TypeError
-
-    def _post_key(self, key):
-        # type: (bytes, ) -> KT
+        raise TypeError(key)
 
+    def _post_key(self, key: bytes) -> KT:
         return key
 
-    def _pre_value(self, value):
-        # type: (VT, ) -> bytes
-
+    def _pre_value(self, value: VT) -> bytes:
         if isinstance(value, bytes):
             return value
         elif isinstance(value, str):
             return value.encode("Latin-1")
 
-        raise TypeError
-
-    def _post_value(self, value):
-        # type: (bytes, ) -> VT
+        raise TypeError(value)
 
+    def _post_value(self, value: bytes) -> VT:
         return value
 
-    def __getitem__(self, key):
-        # type: (KT, ) -> VT
-
+    def __getitem__(self, key: KT) -> VT:
         with self.env.begin() as txn:
             value = txn.get(self._pre_key(key))
         if value is None:
             raise KeyError(key)
         return self._post_value(value)
 
-    def __setitem__(self, key, value):
-        # type: (KT, VT) -> None
-
+    def __setitem__(self, key: KT, value: VT) -> None:
         k = self._pre_key(key)
         v = self._pre_value(value)
-        for i in range(12):
+        for _i in range(12):
             try:
                 with self.env.begin(write=True) as txn:
                     txn.put(k, v)
                     return
             except lmdb.MapFullError:
                 if not self.autogrow:
                     raise
                 new_map_size = self.map_size * 2
                 self.map_size = new_map_size
                 logger.info(self.autogrow_msg, self.env.path(), new_map_size)
 
         exit(self.autogrow_error.format(self.env.path()))
 
-    def __delitem__(self, key):
-        # type: (KT, ) -> None
-
+    def __delitem__(self, key: KT) -> None:
         with self.env.begin(write=True) as txn:
             txn.delete(self._pre_key(key))
 
-    def keys(self):
-        # type: () -> Iterator[KT]
-
+    def keys(self) -> Iterator[KT]:
         with self.env.begin() as txn:
             for key in txn.cursor().iternext(keys=True, values=False):
                 yield self._post_key(key)
 
-    def items(self):
-        # type: () -> Iterator[Tuple[KT, VT]]
-
+    def items(self) -> Iterator[Tuple[KT, VT]]:
         with self.env.begin() as txn:
             for key, value in txn.cursor().iternext(keys=True, values=True):
                 yield (self._post_key(key), self._post_value(value))
 
-    def values(self):
-        # type: () -> Iterator[VT]
-
+    def values(self) -> Iterator[VT]:
         with self.env.begin() as txn:
             for value in txn.cursor().iternext(keys=False, values=True):
                 yield self._post_value(value)
 
-    def __contains__(self, key):
-        # type: (object, ) -> bool
-
+    def __contains__(self, key: KT) -> bool:
         with self.env.begin() as txn:
             value = txn.get(self._pre_key(key))
         return value is not None
 
-    def __iter__(self):
-        # type: () -> Iterator[KT]
-
+    def __iter__(self) -> Iterator[KT]:
         return self.keys()
 
-    def __len__(self):
-        # type: () -> int
-
+    def __len__(self) -> int:
         with self.env.begin() as txn:
             return txn.stat()["entries"]
 
-    def pop(self, key, default=object()):
-        # type: (KT, Union[VT, T]) -> Union[VT, T]
-
+    def pop(self, key: KT, default: Union[VT, T] = _DEFAULT) -> Union[VT, T]:
         with self.env.begin(write=True) as txn:
             value = txn.pop(self._pre_key(key))
         if value is None:
             return default
         return self._post_value(value)
 
-    def update(self, __other=(), **kwds):  # python3.8 only: update(self, other=(), /, **kwds)
-        # type: (Any, **VT) -> None
-
+    def update(self, __other: Any = (), **kwds: VT) -> None:  # python3.8 only: update(self, other=(), /, **kwds)
         # fixme: `kwds`
 
         # note: benchmarking showed that there is no real difference between using lists or iterables
         # as input to `putmulti`.
         # lists: Finished 14412594 in 253496 seconds.
         # iter:  Finished 14412594 in 256315 seconds.
 
         # save generated lists in case the insert fails and needs to be retried
         # for performance reasons, but mostly because `__other` could be an iterable
         # which would already be exhausted on the second try
-        pairs_other = None  # type: Optional[List[Tuple[bytes, bytes]]]
-        pairs_kwds = None  # type: Optional[List[Tuple[bytes, bytes]]]
+        pairs_other: Optional[List[Tuple[bytes, bytes]]] = None
+        pairs_kwds: Optional[List[Tuple[bytes, bytes]]] = None
 
-        for i in range(12):
+        for _i in range(12):
             try:
                 with self.env.begin(write=True) as txn:
                     with txn.cursor() as curs:
                         if isinstance(__other, Mapping):
                             pairs_other = pairs_other or [
                                 (self._pre_key(key), self._pre_value(__other[key])) for key in __other
                             ]
@@ -259,43 +218,35 @@
                     raise
                 new_map_size = self.map_size * 2
                 self.map_size = new_map_size
                 logger.info(self.autogrow_msg, self.env.path(), new_map_size)
 
         exit(self.autogrow_error.format(self.env.path()))
 
-    def sync(self):
-        # type: () -> None
-
+    def sync(self) -> None:
         self.env.sync()
 
-    def close(self):
-        # type: () -> None
-
+    def close(self) -> None:
         self.env.close()
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         return self
 
     def __exit__(self, *args):
         self.close()
 
 
 class LmdbGzip(Lmdb):
-    def __init__(self, env, compresslevel=9):
-        Lmdb.__init__(self, env)
+    def __init__(self, env, autogrow: bool, compresslevel: int = 9):
+        Lmdb.__init__(self, env, autogrow)
         self.compresslevel = compresslevel
 
-    def _pre_value(self, value):
-        # type: (VT, ) -> bytes
-
+    def _pre_value(self, value: VT) -> bytes:
         value = Lmdb._pre_value(self, value)
         return compress(value, self.compresslevel)
 
-    def _post_value(self, value):
-        # type: (bytes, ) -> VT
-
+    def _post_value(self, value: bytes) -> VT:
         return decompress(value)
 
 
-def open(file, flag="r", mode=0o755):
-    return Lmdb.open(file, flag, mode)
+def open(file, flag="r", mode=0o755, **kwargs):
+    return Lmdb.open(file, flag, mode, **kwargs)
```

