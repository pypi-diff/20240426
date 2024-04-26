# Comparing `tmp/checksum_dict-1.1.3.tar.gz` & `tmp/checksum_dict-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checksum_dict-1.1.3.tar", last modified: Wed Feb 21 18:20:07 2024, max compression
+gzip compressed data, was "checksum_dict-1.1.4.tar", last modified: Fri Apr 26 18:35:01 2024, max compression
```

## Comparing `checksum_dict-1.1.3.tar` & `checksum_dict-1.1.4.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:20:07.684466 checksum_dict-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:20:07.684466 checksum_dict-1.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:20:07.684466 checksum_dict-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-21 18:20:07.684466 checksum_dict-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:20:07.684466 checksum_dict-1.1.3/checksum_dict/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/checksum_dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/checksum_dict/_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/checksum_dict/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/checksum_dict/default.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/checksum_dict/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/checksum_dict/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:20:07.684466 checksum_dict-1.1.3/checksum_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-21 18:20:07.000000 checksum_dict-1.1.3/checksum_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-21 18:20:07.000000 checksum_dict-1.1.3/checksum_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 18:20:07.000000 checksum_dict-1.1.3/checksum_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-21 18:20:07.000000 checksum_dict-1.1.3/checksum_dict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 18:20:07.000000 checksum_dict-1.1.3/checksum_dict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 18:20:07.684466 checksum_dict-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-21 18:19:53.000000 checksum_dict-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:35:01.887369 checksum_dict-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:35:01.883370 checksum_dict-1.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:35:01.883370 checksum_dict-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 18:35:01.887369 checksum_dict-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:35:01.883370 checksum_dict-1.1.4/checksum_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/checksum_dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/checksum_dict/_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/checksum_dict/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/checksum_dict/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/checksum_dict/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/checksum_dict/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/checksum_dict/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:35:01.887369 checksum_dict-1.1.4/checksum_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 18:35:01.000000 checksum_dict-1.1.4/checksum_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-26 18:35:01.000000 checksum_dict-1.1.4/checksum_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:35:01.000000 checksum_dict-1.1.4/checksum_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 18:35:01.000000 checksum_dict-1.1.4/checksum_dict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 18:35:01.000000 checksum_dict-1.1.4/checksum_dict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:35:01.887369 checksum_dict-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-26 18:34:51.000000 checksum_dict-1.1.4/setup.py
```

### Comparing `checksum_dict-1.1.3/.github/workflows/release.yaml` & `checksum_dict-1.1.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `checksum_dict-1.1.3/README.md` & `checksum_dict-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `checksum_dict-1.1.3/checksum_dict/_key.py` & `checksum_dict-1.1.4/checksum_dict/_key.py`

 * *Files identical despite different names*

### Comparing `checksum_dict-1.1.3/checksum_dict/base.py` & `checksum_dict-1.1.4/checksum_dict/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+
 from typing import TYPE_CHECKING, Dict, Iterable, Tuple, TypeVar, Union
 
+from checksum_dict import exceptions
 from checksum_dict._key import EthAddressKey
 
 if TYPE_CHECKING:
     from checksum_dict._key import AnyAddressOrContract
 else:
     from eth_typing import AnyAddress as AnyAddressOrContract
 
@@ -31,15 +33,21 @@
         return f"ChecksumAddressDict({str(dict(self))})"
     
     def __getitem__(self, key: AnyAddressOrContract) -> T:
         try:
             # It is ~700x faster to perform this check and then skip the checksum if we find a result for this key
             return super().__getitem__(key)
         except KeyError:
+            # NOTE: passing instead of checksumming here lets us keep a clean exc chain
+            pass
+            
+        try:
             return super().__getitem__(EthAddressKey(key))
+        except KeyError as e:
+            raise exceptions.KeyError(*e.args) from None
 
     def __setitem__(self, key: AnyAddressOrContract, value: T) -> None:
         if key in self:
             # It is ~700x faster to perform this check and then skip the checksum if we find a result for this key
             super().__setitem__(key, value)
         else:
             super().__setitem__(EthAddressKey(key), value)
```

### Comparing `checksum_dict-1.1.3/checksum_dict/default.py` & `checksum_dict-1.1.4/checksum_dict/default.py`

 * *Files identical despite different names*

### Comparing `checksum_dict-1.1.3/checksum_dict/singleton.py` & `checksum_dict-1.1.4/checksum_dict/singleton.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import threading
 from collections import defaultdict
 from typing import Any, DefaultDict, Dict, Generic, Tuple
 
+from checksum_dict import exceptions
 from checksum_dict.base import AnyAddressOrContract, ChecksumAddressDict, T
 
 
 _LocksDict = DefaultDict[AnyAddressOrContract, threading.Lock]
 
 class ChecksumAddressSingletonMeta(type, Generic[T]):
     def __init__(cls, name: str, bases: Tuple[type, ...], namespace: Dict[str, Any]) -> None:
@@ -13,24 +14,28 @@
         cls.__instances: ChecksumAddressDict[T] = ChecksumAddressDict()
         cls.__locks: _LocksDict = defaultdict(threading.Lock)
         cls.__locks_lock: threading.Lock = threading.Lock()
 
     def __call__(cls, address: AnyAddressOrContract, *args: Any, **kwargs: Any) -> T:  # type: ignore
         address = str(address)
         try:
-            instance = cls.__instances[address]
-        except KeyError:
-            with cls.__get_address_lock(address):
-                # Try to get the instance again, in case it was added while waiting for the lock
-                try:
-                    instance =  cls.__instances[address]
-                except KeyError:
-                    instance = super().__call__(address, *args, **kwargs)
-                    cls.__instances[address] = instance
-            cls.__delete_address_lock(address)
+            return cls.__instances[address]
+        except exceptions.KeyError:
+            pass  # NOTE: passing instead of proceeding lets helps us keep a clean exc chain
+            
+        with cls.__get_address_lock(address):
+            # Try to get the instance again, in case it was added while waiting for the lock
+            try:
+                return cls.__instances[address]
+            except exceptions.KeyError:
+                pass  # NOTE: passing instead of proceeding here lets us keep a clean exc chain
+            
+            instance = super().__call__(address, *args, **kwargs)
+            cls.__instances[address] = instance
+        cls.__delete_address_lock(address)
         return instance
     
     def __get_address_lock(cls, address: AnyAddressOrContract) -> threading.Lock:
         """ Makes sure the singleton is actually a singleton. """
         with cls.__locks_lock:
             return cls.__locks[address]
```

### Comparing `checksum_dict-1.1.3/setup.py` & `checksum_dict-1.1.4/setup.py`

 * *Files identical despite different names*

