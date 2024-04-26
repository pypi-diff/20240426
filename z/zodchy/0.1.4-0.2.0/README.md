# Comparing `tmp/zodchy-0.1.4.tar.gz` & `tmp/zodchy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy-0.1.4.tar", max compression
+gzip compressed data, was "zodchy-0.2.0.tar", max compression
```

## Comparing `zodchy-0.1.4.tar` & `zodchy-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,14 @@
--rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy-0.1.4/README.md
--rw-r--r--   0        0        0      503 2024-04-15 10:02:42.485148 zodchy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       43 2024-04-11 07:57:07.719271 zodchy-0.1.4/zodchy/__init__.py
--rw-r--r--   0        0        0      459 2024-04-11 07:57:07.719421 zodchy-0.1.4/zodchy/codex/__init__.py
--rw-r--r--   0        0        0      699 2024-04-14 13:38:37.665427 zodchy-0.1.4/zodchy/codex/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      741 2024-04-14 13:40:59.600989 zodchy-0.1.4/zodchy/codex/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      254 2024-04-14 13:40:59.602373 zodchy-0.1.4/zodchy/codex/__pycache__/base.cpython-312.pyc
--rw-r--r--   0        0        0     1809 2024-04-14 13:40:59.603000 zodchy-0.1.4/zodchy/codex/__pycache__/communication.cpython-312.pyc
--rw-r--r--   0        0        0     1037 2024-04-14 13:40:59.605308 zodchy-0.1.4/zodchy/codex/__pycache__/cqrs.cpython-312.pyc
--rw-r--r--   0        0        0     3490 2024-04-14 13:40:59.604928 zodchy-0.1.4/zodchy/codex/__pycache__/di.cpython-312.pyc
--rw-r--r--   0        0        0      770 2024-04-14 13:40:59.602622 zodchy-0.1.4/zodchy/codex/__pycache__/identity.cpython-312.pyc
--rw-r--r--   0        0        0     5420 2024-04-14 13:38:37.666161 zodchy-0.1.4/zodchy/codex/__pycache__/query.cpython-310.pyc
--rw-r--r--   0        0        0     8275 2024-04-14 17:02:02.243157 zodchy-0.1.4/zodchy/codex/__pycache__/query.cpython-312.pyc
--rw-r--r--   0        0        0       65 2024-04-02 15:23:42.894657 zodchy-0.1.4/zodchy/codex/base.py
--rw-r--r--   0        0        0     1084 2024-04-02 15:23:42.894771 zodchy-0.1.4/zodchy/codex/communication.py
--rw-r--r--   0        0        0      390 2024-04-05 16:20:59.839302 zodchy-0.1.4/zodchy/codex/cqrs.py
--rw-r--r--   0        0        0     1468 2024-04-11 07:57:07.719538 zodchy-0.1.4/zodchy/codex/di.py
--rw-r--r--   0        0        0      161 2024-04-02 15:23:42.895433 zodchy-0.1.4/zodchy/codex/identity.py
--rw-r--r--   0        0        0     2870 2024-04-14 17:02:02.063167 zodchy-0.1.4/zodchy/codex/query.py
--rw-r--r--   0        0        0       19 2024-04-02 15:23:42.895673 zodchy-0.1.4/zodchy/notations/__init__.py
--rw-r--r--   0        0        0      190 2024-04-14 13:40:59.605598 zodchy-0.1.4/zodchy/notations/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    13488 2024-04-14 16:24:03.836275 zodchy-0.1.4/zodchy/notations/__pycache__/math.cpython-312.pyc
--rw-r--r--   0        0        0     7827 2024-04-14 16:24:03.652202 zodchy-0.1.4/zodchy/notations/math.py
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 zodchy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy-0.2.0/README.md
+-rw-r--r--   0        0        0      476 2024-04-26 14:10:51.954708 zodchy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-26 14:09:47.283719 zodchy-0.2.0/zodchy/__init__.py
+-rw-r--r--   0        0        0       60 2024-04-26 14:04:00.386664 zodchy-0.2.0/zodchy/codex/__init__.py
+-rw-r--r--   0        0        0      304 2024-04-26 13:33:12.470259 zodchy-0.2.0/zodchy/codex/cqea/__init__.py
+-rw-r--r--   0        0        0      648 2024-04-26 14:04:00.437433 zodchy-0.2.0/zodchy/codex/cqea/actors.py
+-rw-r--r--   0        0        0     1083 2024-04-26 13:33:12.496006 zodchy-0.2.0/zodchy/codex/cqea/messages.py
+-rw-r--r--   0        0        0     1468 2024-04-11 07:57:07.719538 zodchy-0.2.0/zodchy/codex/di.py
+-rw-r--r--   0        0        0      171 2024-04-26 12:52:44.493427 zodchy-0.2.0/zodchy/codex/identity.py
+-rw-r--r--   0        0        0      271 2024-04-26 14:04:00.427192 zodchy-0.2.0/zodchy/codex/query/__init__.py
+-rw-r--r--   0        0        0     2438 2024-04-26 14:04:00.412260 zodchy-0.2.0/zodchy/codex/query/bits.py
+-rw-r--r--   0        0        0      499 2024-04-26 14:04:00.362265 zodchy-0.2.0/zodchy/codex/query/parsing.py
+-rw-r--r--   0        0        0       53 2024-04-26 14:05:35.505418 zodchy-0.2.0/zodchy/types.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 zodchy-0.2.0/PKG-INFO
```

### Comparing `zodchy-0.1.4/zodchy/codex/communication.py` & `zodchy-0.2.0/zodchy/codex/cqea/messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 Context = dataclasses.make_dataclass('Context', ())
 
 Query = dataclasses.make_dataclass('Query', (), bases=(Message,))
 Command = dataclasses.make_dataclass('Command', (), bases=(Message,))
 Event = dataclasses.make_dataclass('Event', (), bases=(Message,))
 
 Error = dataclasses.make_dataclass('Error', (), bases=(Event,))
-
-IOEvent = dataclasses.make_dataclass('IOE', (), bases=(Event,))
 BDEvent = dataclasses.make_dataclass('BDE', (), bases=(Event,))
+IOEvent = dataclasses.make_dataclass('IOE', (), bases=(Event,))
 
 StorageEvent = dataclasses.make_dataclass('StorageEvent', (), bases=(IOEvent,))
-ResponseEvent = dataclasses.make_dataclass('ResponseEvent', (), bases=(IOEvent,))
-
 ReadEvent = dataclasses.make_dataclass('ReadEvent', (), bases=(StorageEvent,))
 WriteEvent = dataclasses.make_dataclass('WriteEvent', (), bases=(StorageEvent,))
 
+ResponseEvent = dataclasses.make_dataclass('ResponseEvent', (), bases=(IOEvent,))
+
 P = typing.TypeVar('P', bound=Query | Command)
 C = typing.TypeVar('C', bound=Context)
 
 
 class Frame(typing.Generic[P, C]):
     payload: P
     context: C
```

### Comparing `zodchy-0.1.4/zodchy/codex/di.py` & `zodchy-0.2.0/zodchy/codex/di.py`

 * *Files identical despite different names*

### Comparing `zodchy-0.1.4/zodchy/codex/query.py` & `zodchy-0.2.0/zodchy/codex/query/bits.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import typing
 import abc
-import collections.abc
 
 T = typing.TypeVar("T")
 
 
 class ClauseBit(typing.Generic[T]):
     def __init__(self, *data: typing.Self):
         self._data = data
@@ -132,27 +131,7 @@
 
 class ASC(OrderBit):
     pass
 
 
 class DESC(OrderBit):
     pass
-
-
-class Param(typing.Generic[T]):
-    def __init__(self, name: str, value: ClauseBit[T]):
-        self._value = value
-        self._name = name
-
-    @property
-    def value(self) -> ClauseBit:
-        return self._value
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-
-NotationParser = typing.Callable[
-    [str | collections.abc.Mapping[str, str]],
-    collections.abc.Iterable[Param]
-]
```

### Comparing `zodchy-0.1.4/PKG-INFO` & `zodchy-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: zodchy
-Version: 0.1.4
+Version: 0.2.0
 Summary: Collection of contracts and tools for building CQRS applications
 Home-page: https://github.com/smairon/zodchy
 Author: Smairon
 Author-email: man@smairon.ru
 Maintainer: Smairon
 Maintainer-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Project-URL: Repository, https://github.com/smairon/zodchy
 Description-Content-Type: text/markdown
 
 # Hello
```

