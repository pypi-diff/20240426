# Comparing `tmp/tfrecord_slow-0.4.0.tar.gz` & `tmp/tfrecord_slow-0.5.0.tar.gz`

## Comparing `tfrecord_slow-0.4.0.tar` & `tfrecord_slow-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,34 @@
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/requirements-dev.lock
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/requirements.lock
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/examples/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/examples/bench_reader.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/examples/bench_writer.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/examples/common.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/__init__.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/__main__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/msgpack.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/reader.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/utils/__init__.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/utils/loader.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/src/tfrecord_slow/utils/masked_crc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/tests/test_ndarray.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/tests/test_pickle.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/.gitignore
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 tfrecord_slow-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/requirements-dev.lock
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/requirements.lock
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/__init__.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/bench_fbs_reader.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/bench_fbs_writer.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/bench_flex_reader.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/bench_flex_writer.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/bench_reader.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/bench_writer.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/common.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/message.fbs
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/Data/Message.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/Data/NdArray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/examples/Data/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/__init__.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/__main__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/reader.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/loaders/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/loaders/msgpack_loader.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/loaders/raw_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/utils/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/utils/masked_crc.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/utils/msgpack.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/src/tfrecord_slow/utils/numpy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/tests/test_ndarray.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/tests/test_pickle.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/.gitignore
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.0/PKG-INFO
```

### Comparing `tfrecord_slow-0.4.0/requirements-dev.lock` & `tfrecord_slow-0.5.0/requirements-dev.lock`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 #   features: []
 #   all-features: true
 #   with-sources: false
 
 -e file:.
 asttokens==2.4.1
     # via stack-data
-crc32c==2.3.post0
+crc32c==2.4
     # via tfrecord-slow
 decorator==5.1.1
     # via ipython
 executing==2.0.1
     # via stack-data
+flatbuffers==24.3.25
 iniconfig==2.0.0
     # via pytest
 ipython==8.22.1
 jedi==0.19.1
     # via ipython
 loguru==0.7.2
     # via tfrecord-slow
```

### Comparing `tfrecord_slow-0.4.0/.github/workflows/python-package.yml` & `tfrecord_slow-0.5.0/.github/workflows/python-package.yml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         python-version: ["3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Setup rye
         id: setup-rye
-        uses: eifinger/setup-rye@v1
+        uses: eifinger/setup-rye@v2
         with:
           enable-cache: true
           cache-prefix: "py${{ matrix.python-version }}"
 
       - name: python version
         run: rye pin ${{ matrix.python-version }}
```

### Comparing `tfrecord_slow-0.4.0/.github/workflows/python-publish.yml` & `tfrecord_slow-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.4.0/src/tfrecord_slow/__main__.py` & `tfrecord_slow-0.5.0/src/tfrecord_slow/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Make a new package for it.
 """
 
 import argparse
-import logging
 from pathlib import Path
 from typing import Optional
-from .reader import TfRecordReader
+from .reader import TfrecordReader
 from loguru import logger
-from tqdm import tqdm
+import time
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers()
     add_count_args(subparsers.add_parser("count"))
 
@@ -22,33 +21,38 @@
 def add_count_args(parser: argparse.ArgumentParser):
     parser.set_defaults(func=count)
     parser.add_argument("path", type=Path, help="Path to tfrecord file or directory.")
     parser.add_argument("-m", "--mask", action="store_const", const="*.tfrec")
     parser.add_argument("-c", "--check", action="store_true", help="Check integrity.")
 
 
-def count(args):
-    path: Path = args.path
-    mask: Optional[str] = args.mask
-    check_integrity: bool = args.check
-
+def count(path: Path, mask: Optional[str], check: bool, **kwargs):
     if mask is not None:
         paths = list(path.glob(mask))
     else:
         paths = [path]
 
+    total = 0
+
     for path in paths:
-        with TfRecordReader.open(str(path), check_integrity=check_integrity) as reader:
+        with TfrecordReader.open(str(path), check_integrity=check) as reader:
+            start_time = time.perf_counter()
             num_records = reader.count()
-            print(f"file: {path}, records: {num_records}")
+            end_time = time.perf_counter()
+            records_per_second = num_records / (end_time - start_time)
+            logger.info(
+                f"file: {path}, records: {num_records}, speed: {records_per_second} rec/s"
+            )
+            total += num_records
+
+    logger.info("total records: {}", total)
 
 
 def main():
     args = get_args()
-    print(args)
-
+    logger.debug("{}", args)
     if "func" in args:
-        args.func(args)
+        args.func(**vars(args))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tfrecord_slow-0.4.0/src/tfrecord_slow/msgpack.py` & `tfrecord_slow-0.5.0/src/tfrecord_slow/utils/msgpack.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.4.0/src/tfrecord_slow/reader.py` & `tfrecord_slow-0.5.0/src/tfrecord_slow/reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 import io
 from typing import Optional
 import struct
 import logging
 
+
 logger = logging.getLogger(__name__)
 
 
-class TfRecordReader:
+def _always_return_true(*args, **kwargs):
+    return True
+
+
+class TfrecordReader:
     def __init__(self, file: io.BufferedIOBase, check_integrity: bool = False) -> None:
         self._file = file
-        self._check_integrity = check_integrity
+
+        if check_integrity:
+            from tfrecord_slow.utils.masked_crc import verify_masked_crc
+
+            self._verify_masked_crc32 = verify_masked_crc
+        else:
+            self._verify_masked_crc32 = _always_return_true
 
         self._length_bytes = bytearray(8)
         self._crc_bytes = bytearray(4)
         self._data_bytes = bytearray(1024 * 1024)
 
     @classmethod
     def open(cls, path: str, check_integrity: bool = False):
@@ -29,23 +40,31 @@
             return
         elif bytes_read != 8:
             raise RuntimeError("Invalid tfrecord file: failed to read the record size.")
 
         if self._file.readinto(self._crc_bytes) != 4:
             raise RuntimeError("Invalid tfrecord file: failed to read the start token.")
 
+        if not self._verify_masked_crc32(self._length_bytes, self._crc_bytes):
+            raise RuntimeError("Crc32 check failed.")
+
         (length,) = struct.unpack("<Q", self._length_bytes)
         if length > len(self._data_bytes):
             self._data_bytes = self._data_bytes.zfill(length * 2)
 
         data_bytes_view = memoryview(self._data_bytes)[:length]
+
         if self._file.readinto(data_bytes_view) != length:
             raise RuntimeError("Invalid tfrecord file: failed to read the record.")
         if self._file.readinto(self._crc_bytes) != 4:
             raise RuntimeError("Invalid tfrecord file: failed to read the end token.")
+
+        if not self._verify_masked_crc32(data_bytes_view, self._crc_bytes):
+            raise RuntimeError("Crc32 check failed.")
+
         return data_bytes_view
 
     def __enter__(self):
         return self
 
     def __exit__(self, _exc_type, _exc_value, _traceback):
         self.close()
@@ -54,9 +73,12 @@
         while True:
             data = self.read()
             if data is not None:
                 yield data
             else:
                 break
 
-    def count(self):
-        return sum(1 for _ in self)
+    def count(self) -> int:
+        n = 0
+        for _ in self:
+            n += 1
+        return n
```

### Comparing `tfrecord_slow-0.4.0/src/tfrecord_slow/writer.py` & `tfrecord_slow-0.5.0/src/tfrecord_slow/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import struct
 from io import BufferedIOBase
 from .utils.masked_crc import make_masked_crc
 
 
-class TfRecordWriter:
+class TfrecordWriter:
     def __init__(self, file: BufferedIOBase) -> None:
         self._file = file
 
     @classmethod
     def create(cls, path: str, buffering: int = -1):
         return cls(open(path, mode="wb", buffering=buffering))
```

### Comparing `tfrecord_slow-0.4.0/src/tfrecord_slow/utils/loader.py` & `tfrecord_slow-0.5.0/src/tfrecord_slow/loaders/msgpack_loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,32 @@
-from typing import TypeVar, Iterable, Iterator, Callable, Type
+from typing import TypeVar, Iterable, Iterator, Generic, Type
 from io import BufferedIOBase
-from tfrecord_slow.reader import TfRecordReader
+from tfrecord_slow.reader import TfrecordReader
 import msgspec
 
-T = TypeVar("T")
 
+T = TypeVar("T", bound=msgspec.Struct)
 
-def _default_func(buf: memoryview):
-    return buf.tobytes()
 
-
-class RawTfrecordLoader:
-    def __init__(
-        self,
-        datapipe: Iterable[BufferedIOBase],
-        func: Callable[[memoryview], T] = _default_func,
-        check_integrity: bool = False,
-    ):
-        self.datapipe = datapipe
-        self.check_integrity = check_integrity
-        self.func = func
-
-    def __iter__(self) -> Iterator[T]:
-        for fp in self.datapipe:
-            reader = TfRecordReader(fp, check_integrity=self.check_integrity)
-            for buf in reader:
-                example = self.func(buf)
-                yield example
-
-
-S = TypeVar("S", bound=msgspec.Struct)
-
-
-class MsgpackTfrecordLoader:
+class MsgpackTfrecordLoader(Generic[T]):
     def __init__(
         self,
         datapipe: Iterable[BufferedIOBase],
-        spec: Type[S],
+        spec: Type[T],
         check_integrity: bool = False,
     ):
         """
         Args:
             datapipe: iter of files
             spec: msgspec.Struct, must have owned memory
         """
         self.datapipe = datapipe
         self.check_integrity = check_integrity
         self.spec = spec
 
-    def __iter__(self) -> Iterator[S]:
+    def __iter__(self) -> Iterator[T]:
         decoder = msgspec.msgpack.Decoder(type=self.spec)
         for fp in self.datapipe:
-            reader = TfRecordReader(fp, check_integrity=self.check_integrity)
+            reader = TfrecordReader(fp, check_integrity=self.check_integrity)
             for buf in reader:
                 example = decoder.decode(buf)
                 yield example
```

### Comparing `tfrecord_slow-0.4.0/.gitignore` & `tfrecord_slow-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.4.0/pyproject.toml` & `tfrecord_slow-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 [project]
 name = "tfrecord-slow"
-version = "0.4.0"
+version = "0.5.0"
 description = "Default template for PDM package"
 authors = [
     { name = "SunDoge", email = "triplez0@outlook.com" }
 ]
 dependencies = [
-    "crc32c>=2.3.post0",
-    "numpy>=1",
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 
 [project.scripts]
 hello = "tfrecord_slow:hello"
 
@@ -19,25 +17,30 @@
 msgpack = [
     "msgspec>=0.18.6",
 ]
 cli = [
     "loguru>=0.7.2",
     "tqdm>=4.66.2",
 ]
+crc32c = [
+    "numpy>=1",
+    "crc32c>=2.3.post0",
+]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "safetensors>=0.4.2",
     "pytest>=8.0.1",
     "ipython>=8",
+    "flatbuffers>=24.3.25",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/tfrecord_slow"]
```

### Comparing `tfrecord_slow-0.4.0/PKG-INFO` & `tfrecord_slow-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,48 @@
 Metadata-Version: 2.3
 Name: tfrecord-slow
-Version: 0.4.0
+Version: 0.5.0
 Summary: Default template for PDM package
 Author-email: SunDoge <triplez0@outlook.com>
 Requires-Python: >=3.9
-Requires-Dist: crc32c>=2.3.post0
-Requires-Dist: numpy>=1
 Provides-Extra: cli
 Requires-Dist: loguru>=0.7.2; extra == 'cli'
 Requires-Dist: tqdm>=4.66.2; extra == 'cli'
+Provides-Extra: crc32c
+Requires-Dist: crc32c>=2.3.post0; extra == 'crc32c'
+Requires-Dist: numpy>=1; extra == 'crc32c'
 Provides-Extra: msgpack
 Requires-Dist: msgspec>=0.18.6; extra == 'msgpack'
 Description-Content-Type: text/markdown
 
 # tfrecord-slow
 
 [![Github Actions](https://img.shields.io/github/actions/workflow/status/SunDoge/tfrecord-slow/python-package.yml?branch=main&style=for-the-badge)](https://github.com/SunDoge/tfrecord-slow/actions/workflows/python-package.yml)
 [![Pypi](https://img.shields.io/pypi/v/tfrecord-slow?style=for-the-badge)](https://pypi.org/project/tfrecord-slow/)
 
 TFRecord reader and writer without protobuf.
 
 ## Install
 
+### Reader only (without masked crc32 check support)
+
 ```shell
 pip install tfrecord-slow
 ```
+
+### Reader with masked crc32 check support
+
+```shell
+pip install tfrecord-slow[crc32c]
+```
+
+### Writer (must have crc32c installed)
+
+```shell
+pip install tfrecord-slow[crc32c]
+```
+
+### Use ndarray msgpack support
+
+```shell
+pip install tfrecord-slow[msgpack]
+```
```

