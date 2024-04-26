# Comparing `tmp/lindi-0.3.0.tar.gz` & `tmp/lindi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lindi-0.3.0.tar", max compression
+gzip compressed data, was "lindi-0.3.1.tar", max compression
```

## Comparing `lindi-0.3.0.tar` & `lindi-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,39 @@
--rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.0/LICENSE
--rw-r--r--   0        0        0     5269 2024-04-19 19:44:06.440621 lindi-0.3.0/README.md
--rw-r--r--   0        0        0    28820 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
--rw-r--r--   0        0        0      136 2024-03-21 11:16:09.352672 lindi-0.3.0/lindi/LindiH5ZarrStore/__init__.py
--rw-r--r--   0        0        0     3112 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5ZarrStore/_util.py
--rw-r--r--   0        0        0     3710 2024-04-04 18:56:02.142012 lindi-0.3.0/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py
--rw-r--r--   0        0        0     1045 2024-03-21 18:16:58.794258 lindi-0.3.0/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py
--rw-r--r--   0        0        0        0 2024-03-21 18:16:58.794258 lindi-0.3.0/lindi/LindiH5pyFile/FileSegmentReader/__init__.py
--rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyAttributes.py
--rw-r--r--   0        0        0    11685 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyDataset.py
--rw-r--r--   0        0        0    15606 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyFile.py
--rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyGroup.py
--rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyLink.py
--rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyReference.py
--rw-r--r--   0        0        0    10388 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
--rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.0/lindi/LindiH5pyFile/__init__.py
--rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
--rw-r--r--   0        0        0     1941 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
--rw-r--r--   0        0        0     6651 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.0/lindi/LindiH5pyFile/writers/__init__.py
--rw-r--r--   0        0        0    10625 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiStagingStore/LindiStagingStore.py
--rw-r--r--   0        0        0     2915 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiStagingStore/StagingArea.py
--rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiStagingStore/__init__.py
--rw-r--r--   0        0        0      286 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.0/lindi/conversion/__init__.py
--rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.0/lindi/conversion/_util.py
--rw-r--r--   0        0        0     5907 2024-04-18 21:52:00.325839 lindi-0.3.0/lindi/conversion/attr_conversion.py
--rw-r--r--   0        0        0    10819 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/conversion/create_zarr_dataset_from_h5_data.py
--rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.0/lindi/conversion/decode_references.py
--rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.0/lindi/conversion/h5_filters_to_codecs.py
--rw-r--r--   0        0        0     2041 2024-04-19 14:03:48.185150 lindi-0.3.0/lindi/conversion/h5_ref_to_zarr_attr.py
--rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.0/lindi/conversion/nan_inf_ninf.py
--rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.0/lindi/conversion/reformat_json.py
--rw-r--r--   0        0        0      748 2024-04-19 19:44:21.692431 lindi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5969 1970-01-01 00:00:00.000000 lindi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5697 2024-04-25 13:07:47.575992 lindi-0.3.1/README.md
+-rw-r--r--   0        0        0     1314 2024-04-25 20:36:30.815997 lindi-0.3.1/lindi/File/File.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:30:55.955999 lindi-0.3.1/lindi/File/__init__.py
+-rw-r--r--   0        0        0    29801 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
+-rw-r--r--   0        0        0      529 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
+-rw-r--r--   0        0        0      169 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiH5ZarrStore/__init__.py
+-rw-r--r--   0        0        0     3112 2024-04-22 18:53:12.519957 lindi-0.3.1/lindi/LindiH5ZarrStore/_util.py
+-rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyAttributes.py
+-rw-r--r--   0        0        0    11776 2024-04-25 18:34:46.019872 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyDataset.py
+-rw-r--r--   0        0        0    24528 2024-04-25 13:36:35.223981 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyFile.py
+-rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyGroup.py
+-rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyLink.py
+-rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyReference.py
+-rw-r--r--   0        0        0    11183 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
+-rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.1/lindi/LindiH5pyFile/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
+-rw-r--r--   0        0        0     1941 2024-04-19 19:44:06.440621 lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
+-rw-r--r--   0        0        0     6651 2024-04-24 16:16:12.091927 lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.1/lindi/LindiH5pyFile/writers/__init__.py
+-rw-r--r--   0        0        0    16420 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiRemfile/LindiRemfile.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiRemfile/__init__.py
+-rw-r--r--   0        0        0     8848 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiStagingStore/LindiStagingStore.py
+-rw-r--r--   0        0        0     3506 2024-04-25 13:16:02.363988 lindi-0.3.1/lindi/LindiStagingStore/StagingArea.py
+-rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.1/lindi/LindiStagingStore/__init__.py
+-rw-r--r--   0        0        0     2299 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LocalCache/LocalCache.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LocalCache/__init__.py
+-rw-r--r--   0        0        0      388 2024-04-25 20:32:45.831998 lindi-0.3.1/lindi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.1/lindi/conversion/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.1/lindi/conversion/_util.py
+-rw-r--r--   0        0        0     5907 2024-04-24 16:16:12.091927 lindi-0.3.1/lindi/conversion/attr_conversion.py
+-rw-r--r--   0        0        0    10819 2024-04-24 16:16:12.091927 lindi-0.3.1/lindi/conversion/create_zarr_dataset_from_h5_data.py
+-rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.1/lindi/conversion/decode_references.py
+-rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.1/lindi/conversion/h5_filters_to_codecs.py
+-rw-r--r--   0        0        0     2041 2024-04-24 16:16:12.091927 lindi-0.3.1/lindi/conversion/h5_ref_to_zarr_attr.py
+-rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.1/lindi/conversion/nan_inf_ninf.py
+-rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.1/lindi/conversion/reformat_json.py
+-rw-r--r--   0        0        0      729 2024-04-26 14:55:53.451922 lindi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6357 1970-01-01 00:00:00.000000 lindi-0.3.1/PKG-INFO
```

### Comparing `lindi-0.3.0/LICENSE` & `lindi-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/README.md` & `lindi-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 - A specification for representing arbitrary HDF5 files as Zarr stores. This handles scalar datasets, references, soft links, and compound data types for datasets.
 - A Zarr wrapper for remote or local HDF5 files (LindiH5ZarrStore).
 - A mechanism for creating .lindi.json (or .nwb.lindi.json) files that reference data chunks in external files, inspired by [kerchunk](https://github.com/fsspec/kerchunk).
 - An h5py-like interface for reading from and writing to these data sources that can be used with [pynwb](https://pynwb.readthedocs.io/en/stable/).
 - A mechanism for uploading and downloading these data sources to and from cloud storage, including DANDI.
 
-This project was inspired by [kerchunk](https://github.com/fsspec/kerchunk) and [hdmf-zarr](https://hdmf-zarr.readthedocs.io/en/latest/index.html) and depends on [zarr](https://zarr.readthedocs.io/en/stable/), [h5py](https://www.h5py.org/), [remfile](https://github.com/magland/remfile) and [numcodecs](https://numcodecs.readthedocs.io/en/stable/).
+This project was inspired by [kerchunk](https://github.com/fsspec/kerchunk) and [hdmf-zarr](https://hdmf-zarr.readthedocs.io/en/latest/index.html) and depends on [zarr](https://zarr.readthedocs.io/en/stable/), [h5py](https://www.h5py.org/) and [numcodecs](https://numcodecs.readthedocs.io/en/stable/).
 
 ## Installation
 
 ```bash
 pip install lindi
 ```
 
@@ -31,60 +31,77 @@
 ```bash
 cd lindi
 pip install -e .
 ```
 
 ## Use cases
 
+* Lazy-load a remote NWB/HDF5 file for efficient access to metadata and data.
 * Represent a remote NWB/HDF5 file as a .nwb.lindi.json file.
 * Read a local or remote .nwb.lindi.json file using pynwb or other tools.
 * Edit a .nwb.lindi.json file using pynwb or other tools.
 * Add datasets to a .nwb.lindi.json file using a local staging area.
-* Upload a .nwb.lindi.json file to a cloud storage service such as DANDI.
+* Upload a .nwb.lindi.json file with staged datasets to a cloud storage service such as DANDI.
+
+### Lazy-load a remote NWB/HDF5 file for efficient access to metadata and data
+
+```python
+import pynwb
+import lindi
+
+# URL of the remote NWB file
+h5_url = "https://api.dandiarchive.org/api/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/download/"
+
+# Set up a local cache
+local_cache = lindi.LocalCache(cache_dir='lindi_cache')
+
+# Create the h5py-like client
+client = lindi.LindiH5pyFile.from_hdf5_file(h5_url, local_cache=local_cache)
+
+# Open using pynwb
+with pynwb.NWBHDF5IO(file=client, mode="r") as io:
+    nwbfile = io.read()
+    print(nwbfile)
+
+# The downloaded data will be cached locally, so subsequent reads will be faster
+```
 
 ### Represent a remote NWB/HDF5 file as a .nwb.lindi.json file
 
 ```python
 import json
-import pynwb
 import lindi
 
 # URL of the remote NWB file
 h5_url = "https://api.dandiarchive.org/api/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/download/"
 
-# Create a read-only Zarr store as a wrapper for the h5 file
-store = lindi.LindiH5ZarrStore.from_file(h5_url)
+# Create the h5py-like client
+client = lindi.LindiH5pyFile.from_hdf5_file(h5_url)
 
 # Generate a reference file system
-rfs = store.to_reference_file_system()
+rfs = client.to_reference_file_system()
 
 # Save it to a file for later use
 with open("example.lindi.json", "w") as f:
     json.dump(rfs, f, indent=2)
 
-# Create an h5py-like client from the reference file system
-client = lindi.LindiH5pyFile.from_reference_file_system(rfs)
-
-# Open using pynwb
-with pynwb.NWBHDF5IO(file=client, mode="r") as io:
-    nwbfile = io.read()
-    print(nwbfile)
+# See the next example for how to read this file
 ```
 
 ### Read a local or remote .nwb.lindi.json file using pynwb or other tools
 
 ```python
 import pynwb
 import lindi
 
 # URL of the remote .nwb.lindi.json file
 url = 'https://kerchunk.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
 
-# Load the h5py-like client for the reference file system
-client = lindi.LindiH5pyFile.from_reference_file_system(url)
+# Load the h5py-like client
+client = lindi.LindiH5pyFile.from_lindi_file(url)
 
 # Open using pynwb
 with pynwb.NWBHDF5IO(file=client, mode="r") as io:
     nwbfile = io.read()
     print(nwbfile)
 ```
 
@@ -117,24 +134,24 @@
 
 # URL of the remote .nwb.lindi.json file
 url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
 
 # Load the h5py-like client for the reference file system
 # in read-write mode with a staging area
 with lindi.StagingArea.create(base_dir='lindi_staging') as staging_area:
-    client = lindi.LindiH5pyFile.from_reference_file_system(
+    client = lindi.LindiH5pyFile.from_lindi_file(
         url,
         mode="r+",
         staging_area=staging_area
     )
     # add datasets to client using pynwb or other tools
     # upload the changes to the remote .nwb.lindi.json file
 ```
 
-### Upload a .nwb.lindi.json file to a cloud storage service such as DANDI
+### Upload a .nwb.lindi.json file with staged datasets to a cloud storage service such as DANDI
 
 See [this example](https://github.com/magland/lindi-dandi/blob/main/devel/lindi_test_2.py).
 
 ## For developers
 
 [Special Zarr annotations used by LINDI](docs/special_zarr_annotations.md)
```

### Comparing `lindi-0.3.0/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py` & `lindi-0.3.1/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import json
 import base64
 from typing import Union, List, IO, Any, Dict
-from dataclasses import dataclass
 import numpy as np
 import zarr
-import remfile
 from zarr.storage import Store, MemoryStore
 import h5py
 from ._util import (
     _read_bytes,
     _get_chunk_byte_range,
     _get_byte_range_for_contiguous_dataset,
     _join,
@@ -16,28 +14,17 @@
     _write_rfs_to_file,
 )
 from ..conversion.attr_conversion import h5_to_zarr_attr
 from ..conversion.reformat_json import reformat_json
 from ..conversion.h5_filters_to_codecs import h5_filters_to_codecs
 from ..conversion.create_zarr_dataset_from_h5_data import create_zarr_dataset_from_h5_data
 from ..LindiH5pyFile.LindiReferenceFileSystemStore import LindiReferenceFileSystemStore
-
-
-@dataclass
-class LindiH5ZarrStoreOpts:
-    """
-    Options for the LindiH5ZarrStore class.
-
-    Attributes:
-        num_dataset_chunks_threshold (Union[int, None]): For each dataset in the
-        HDF5 file, if the number of chunks is greater than this threshold, then
-        the dataset will be represented as an external array link. If None, then
-        the threshold is not used. Default is 1000.
-    """
-    num_dataset_chunks_threshold: Union[int, None] = 1000
+from ..LocalCache.LocalCache import LocalCache
+from ..LindiRemfile.LindiRemfile import LindiRemfile
+from .LindiH5ZarrStoreOpts import LindiH5ZarrStoreOpts
 
 
 class LindiH5ZarrStore(Store):
     """A zarr store that provides a read-only view of an HDF5 file.
 
     Do not call the constructor directly. Instead do one of the following:
 
@@ -53,24 +40,26 @@
 
     def __init__(
         self,
         *,
         _file: Union[IO, Any],
         _opts: LindiH5ZarrStoreOpts,
         _url: Union[str, None] = None,
-        _entities_to_close: List[Any]
+        _entities_to_close: List[Any],
+        _local_cache: Union[LocalCache, None] = None
     ):
         """
         Do not call the constructor directly. Instead, use the from_file class
         method.
         """
         self._file: Union[IO, Any, None] = _file
         self._h5f: Union[h5py.File, None] = h5py.File(_file, "r")
         self._url = _url
         self._opts = _opts
+        self._local_cache = _local_cache
         self._entities_to_close = _entities_to_close + [self._h5f]
 
         # Some datasets do not correspond to traditional chunked datasets. For
         # those datasets, we need to store the inline data so that we can return
         # it when the chunk is requested.
         self._inline_arrays: Dict[str, InlineArray] = {}
 
@@ -78,14 +67,15 @@
 
     @staticmethod
     def from_file(
         hdf5_file_name_or_url: str,
         *,
         opts: LindiH5ZarrStoreOpts = LindiH5ZarrStoreOpts(),
         url: Union[str, None] = None,
+        local_cache: Union[LocalCache, None] = None
     ):
         """
         Create a LindiH5ZarrStore from a file or url pointing to an HDF5 file.
 
         Parameters
         ----------
         hdf5_file_name_or_url : str
@@ -95,22 +85,27 @@
         url : str or None
             If hdf5_file_name_or_url is a local file name, then this can
             optionally be set to the URL of the remote file to be used when
             creating references. If None, and the hdf5_file_name_or_url is a
             local file name, then you will need to set
             opts.num_dataset_chunks_threshold to None, and you will not be able
             to use the to_reference_file_system method.
+        local_cache : LocalCache or None
+            A local cache to use when reading chunks from a remote file. If None,
+            then no local cache is used.
         """
         if hdf5_file_name_or_url.startswith(
             "http://"
         ) or hdf5_file_name_or_url.startswith("https://"):
             # note that the remfile.File object does not need to be closed
-            remf = remfile.File(hdf5_file_name_or_url, verbose=False)
-            return LindiH5ZarrStore(_file=remf, _url=hdf5_file_name_or_url, _opts=opts, _entities_to_close=[])
+            remf = LindiRemfile(hdf5_file_name_or_url, verbose=False, local_cache=local_cache)
+            return LindiH5ZarrStore(_file=remf, _url=hdf5_file_name_or_url, _opts=opts, _entities_to_close=[], _local_cache=local_cache)
         else:
+            if local_cache is not None:
+                raise Exception("local_cache cannot be used with a local file")
             f = open(hdf5_file_name_or_url, "rb")
             return LindiH5ZarrStore(_file=f, _url=url, _opts=opts, _entities_to_close=[f])
 
     def close(self):
         """Close the store."""
         for e in self._entities_to_close:
             e.close()
@@ -330,15 +325,32 @@
             key_parent, key_name
         )
         if inline_data is not None:
             return inline_data
         else:
             assert byte_offset is not None
             assert byte_count is not None
+            if self._local_cache is not None:
+                assert self._url is not None, "Unexpected: url is None but local_cache is not None"
+                ch = self._local_cache.get_remote_chunk(
+                    url=self._url,
+                    offset=byte_offset,
+                    size=byte_count
+                )
+                if ch is not None:
+                    return ch
             buf = _read_bytes(self._file, byte_offset, byte_count)
+            if self._local_cache is not None:
+                assert self._url is not None, "Unexpected: url is None but local_cache is not None"
+                self._local_cache.put_remote_chunk(
+                    url=self._url,
+                    offset=byte_offset,
+                    size=byte_count,
+                    data=buf
+                )
             return buf
 
     def _get_chunk_file_bytes_data(self, key_parent: str, key_name: str):
         if self._h5f is None:
             raise Exception("Store is closed")
         h5_item = self._h5f.get('/' + key_parent, None)
         if not isinstance(h5_item, h5py.Dataset):
@@ -460,15 +472,15 @@
             return []
         else:
             return []
 
     def write_reference_file_system(self, output_file_name: str):
         """Write a reference file system corresponding to this store to a file.
 
-        This can then be loaded using LindiH5pyFile.from_reference_file_system(file_name)
+        This can then be loaded using LindiH5pyFile.from_lindi_file(file_name)
         """
 
         if not output_file_name.endswith(".lindi.json"):
             raise Exception("The output file name must end with .lindi.json")
 
         rfs = self.to_reference_file_system()
         _write_rfs_to_file(rfs=rfs, output_file_name=output_file_name)
@@ -588,15 +600,18 @@
     def __init__(self, h5_dataset: h5py.Dataset):
         self._additional_zarr_attributes = {}
         if h5_dataset.shape == ():
             self._additional_zarr_attributes["_SCALAR"] = True
             self._is_inline = True
             ...
         elif h5_dataset.dtype.kind in ['i', 'u', 'f']:  # integer or float
-            self._is_inline = False
+            if h5_dataset.size and h5_dataset.size < 1000:
+                self._is_inline = True
+            else:
+                self._is_inline = False
         else:
             self._is_inline = True
             if h5_dataset.dtype.kind == "V" and h5_dataset.dtype.fields is not None:  # compound type
                 compound_dtype = []
                 for name in h5_dataset.dtype.names:
                     tt = h5_dataset.dtype[name]
                     if tt == h5py.special_dtype(ref=h5py.Reference):
```

### Comparing `lindi-0.3.0/lindi/LindiH5ZarrStore/_util.py` & `lindi-0.3.1/lindi/LindiH5ZarrStore/_util.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyAttributes.py` & `lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyAttributes.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyDataset.py` & `lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyDataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import TYPE_CHECKING, Any, Dict
 import numpy as np
 import h5py
 import zarr
-import remfile
 
 from .LindiH5pyAttributes import LindiH5pyAttributes
 from .LindiH5pyReference import LindiH5pyReference
+from ..LindiRemfile.LindiRemfile import LindiRemfile
 
 from ..conversion.decode_references import decode_references
 
 
 if TYPE_CHECKING:
     from .LindiH5pyFile import LindiH5pyFile  # pragma: no cover
 
@@ -112,15 +112,15 @@
                 #     else:
                 #         received = received.name
                 # ------------------------------------------
                 # I don't know how to figure out when vlen should be str or bytes
                 # but validate seems to work only when I put in vlen = bytes
                 #
                 vlen = bytes
-                ret = np.dtype(str(ret), metadata={'vlen': vlen})
+                ret = np.dtype(str(ret), metadata={'vlen': vlen})  # type: ignore
         return ret
 
     @property
     def nbytes(self):
         return self._zarr_array.nbytes
 
     @property
@@ -215,15 +215,15 @@
                 raise TypeError(f'Cannot slice a scalar dataset with {selection}')
             return zarr_array[0]
         return decode_references(zarr_array[selection])
 
     def _get_external_hdf5_client(self, url: str) -> h5py.File:
         if url not in _external_hdf5_clients:
             if url.startswith("http://") or url.startswith("https://"):
-                ff = remfile.File(url)
+                ff = LindiRemfile(url, local_cache=self._file._local_cache)
             else:
                 ff = open(url, "rb")  # this never gets closed
             _external_hdf5_clients[url] = h5py.File(ff, "r")
         return _external_hdf5_clients[url]
 
     @property
     def ref(self):
```

### Comparing `lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyGroup.py` & `lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyGroup.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py` & `lindi-0.3.1/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Literal, Dict
+from typing import Literal, Dict, Union
 import json
 import base64
+import requests
 from zarr.storage import Store as ZarrStore
-from .FileSegmentReader.FileSegmentReader import FileSegmentReader
-from .FileSegmentReader.DandiFileSegmentReader import DandiFileSegmentReader
+
+from ..LocalCache.LocalCache import LocalCache
 
 
 class LindiReferenceFileSystemStore(ZarrStore):
     """
     A Zarr store that reads data from a reference file system.
 
     The reference file system is based on the ReferenceFileSystem of fsspec, but
@@ -61,24 +62,27 @@
     In this case, the "{{u1}}" will be replaced with the value of the "u1"
     template string.
 
     It is okay for rfs to be modified outside of this class, and the changes
     will be reflected immediately in the store. This can be used by experimental
     tools such as lindi-cloud.
     """
-    def __init__(self, rfs: dict, mode: Literal["r", "r+"] = "r+"):
+    def __init__(self, rfs: dict, *, mode: Literal["r", "r+"] = "r+", local_cache: Union[LocalCache, None] = None):
         """
         Create a LindiReferenceFileSystemStore.
 
         Parameters
         ----------
         rfs : dict
             The reference file system (see class docstring for details).
         mode : str
             The mode to open the store in. Only "r" is supported at this time.
+        local_cache : LocalCache, optional
+            The local cache to use for caching data chunks read from the
+            remote URLs. If None, no caching is done.
         """
         if "refs" not in rfs:
             raise Exception("rfs must contain a 'refs' key")
 
         # validate rfs['refs']
         for k, v in rfs["refs"].items():
             if isinstance(v, str):
@@ -102,14 +106,15 @@
         if "templates" in rfs:
             for k, v in rfs["templates"].items():
                 if not isinstance(v, str):
                     raise Exception(f"Problem with templates: value for {k} must be a string")
 
         self.rfs = rfs
         self.mode = mode
+        self.local_cache = local_cache
 
     # These methods are overridden from MutableMapping
     def __getitem__(self, key: str):
         if key not in self.rfs["refs"]:
             raise KeyError(key)
         x = self.rfs["refs"][key]
         if isinstance(x, str):
@@ -121,18 +126,24 @@
             return json.dumps(x).encode("utf-8")
         elif isinstance(x, list):
             if len(x) != 3:
                 raise Exception("list must have 3 elements")  # pragma: no cover
             url = x[0]
             offset = x[1]
             length = x[2]
-            if '{{' in url and 'templates' in self.rfs:
+            if '{{' in url and '}}' in url and 'templates' in self.rfs:
                 for k, v in self.rfs["templates"].items():
                     url = url.replace("{{" + k + "}}", v)
-            val = _read_bytes_from_url(url, offset, length)
+            if self.local_cache is not None:
+                x = self.local_cache.get_remote_chunk(url=url, offset=offset, size=length)
+                if x is not None:
+                    return x
+            val = _read_bytes_from_url_or_path(url, offset, length)
+            if self.local_cache is not None:
+                self.local_cache.put_remote_chunk(url=url, offset=offset, size=length, data=val)
             return val
         else:
             # should not happen given checks in __init__, but self.rfs is mutable
             # and contains mutable lists
             raise Exception(f"Problem with {key}: value {x} must be a string or a list")
 
     def __setitem__(self, key: str, value: bytes):
@@ -198,41 +209,47 @@
             if isinstance(v, list):
                 url = v[0]
                 if '{{' not in url:
                     url_counts[url] = url_counts.get(url, 0) + 1
         urls_with_many_occurrences = sorted([url for url, count in url_counts.items() if count >= 5])
         new_templates = rfs.get('templates', {})
         template_names_for_urls: Dict[str, str] = {}
+        for template_name, url in new_templates.items():
+            template_names_for_urls[url] = template_name
         for url in urls_with_many_occurrences:
+            if url in template_names_for_urls:
+                continue
             i = 1
             while f'u{i}' in new_templates:
                 i += 1
             new_templates[f'u{i}'] = url
             template_names_for_urls[url] = f'u{i}'
         if new_templates:
             rfs['templates'] = new_templates
         for k, v in rfs['refs'].items():
             if isinstance(v, list):
                 url = v[0]
                 if url in template_names_for_urls:
                     v[0] = '{{' + template_names_for_urls[url] + '}}'
 
 
-# Keep a global cache of file segment readers that apply to all instances of
-# LindiReferenceFileSystemStore. The key is the URL of the file.
-_file_segment_readers: Dict[str, FileSegmentReader] = {}
-
-
-def _read_bytes_from_url(url: str, offset: int, length: int):
+def _read_bytes_from_url_or_path(url_or_path: str, offset: int, length: int):
     """
     Read a range of bytes from a URL.
     """
-    if url not in _file_segment_readers:
-        if DandiFileSegmentReader.is_dandi_url(url):
-            # This is a DANDI URL, so it needs to be handled specially
-            # see the docstring for DandiFileSegmentReader for details
-            file_segment_reader = DandiFileSegmentReader(url)
-        else:
-            # This is a non-DANDI URL or local file path
-            file_segment_reader = FileSegmentReader(url)
-        _file_segment_readers[url] = file_segment_reader
-    return _file_segment_readers[url].read(offset, length)
+    from ..LindiRemfile.LindiRemfile import _resolve_url
+    if url_or_path.startswith('http://') or url_or_path.startswith('https://'):
+        url_resolved = _resolve_url(url_or_path)  # handle DANDI auth
+        range_start = offset
+        range_end = offset + length - 1
+        range_header = f"bytes={range_start}-{range_end}"
+        headers = {
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
+            "Range": range_header
+        }
+        response = requests.get(url_resolved, headers=headers)
+        response.raise_for_status()
+        return response.content
+    else:
+        with open(url_or_path, 'rb') as f:
+            f.seek(offset)
+            return f.read(length)
```

### Comparing `lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py` & `lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py` & `lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py` & `lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/LindiStagingStore/LindiStagingStore.py` & `lindi-0.3.1/lindi/LindiStagingStore/LindiStagingStore.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,11 @@
-from typing import Callable
-import json
-import tempfile
 import os
 from zarr.storage import Store as ZarrStore
 from ..LindiH5pyFile.LindiReferenceFileSystemStore import LindiReferenceFileSystemStore
 from .StagingArea import StagingArea, _random_str
-from ..LindiH5ZarrStore._util import _write_rfs_to_file
-
-
-# Accepts a string path to a file, uploads (or copies) it somewhere, and returns a string URL
-# (or local path)
-UploadFileFunc = Callable[[str], str]
 
 
 class LindiStagingStore(ZarrStore):
     """
     A Zarr store that allows supplementing a base LindiReferenceFileSystemStore
     where the large data blobs are stored in a staging area. After writing new
     data to the store, the data blobs can be consolidated into larger files and
@@ -90,64 +81,14 @@
             rfs['refs'] = {}
         rfs['refs'][key] = [
             filename,
             offset,
             size
         ]
 
-    def upload(
-        self,
-        *,
-        on_upload_blob: UploadFileFunc,
-        on_upload_main: UploadFileFunc,
-        consolidate_chunks: bool = True
-    ):
-        """
-        Consolidate the chunks in the staging area, upload them to a storage
-        system, updating the references in the base store, and then upload the
-        updated reference file system .json file.
-
-        Parameters
-        ----------
-        on_upload_blob : StoreFileFunc
-            A function that takes a string path to a blob file, uploads or copies it
-            somewhere, and returns a string URL (or local path).
-        on_upload_main : StoreFileFunc
-            A function that takes a string path to the main .json file, stores
-            it somewhere, and returns a string URL (or local path).
-        consolidate_chunks : bool
-            If True (the default), consolidate the chunks in the staging area
-            before uploading.
-
-        Returns
-        -------
-        str
-            The URL (or local path) of the uploaded reference file system .json
-            file.
-        """
-        if consolidate_chunks:
-            self.consolidate_chunks()
-        rfs = self._base_store.rfs
-        rfs = json.loads(json.dumps(rfs))  # deep copy
-        LindiReferenceFileSystemStore.replace_meta_file_contents_with_dicts_in_rfs(rfs)
-        blob_mapping = _upload_directory_of_blobs(self._staging_area.directory, on_upload_blob=on_upload_blob)
-        for k, v in rfs['refs'].items():
-            if isinstance(v, list) and len(v) == 3:
-                url1 = v[0]
-                if url1.startswith(self._staging_area.directory + '/'):
-                    url2 = blob_mapping.get(url1, None)
-                    if url2 is None:
-                        raise ValueError(f"Could not find url in blob mapping: {url1}")
-                    rfs['refs'][k][0] = url2
-        with tempfile.TemporaryDirectory() as tmpdir:
-            rfs_fname = f"{tmpdir}/rfs.lindi.json"
-            LindiReferenceFileSystemStore.use_templates_in_rfs(rfs)
-            _write_rfs_to_file(rfs=rfs, output_file_name=rfs_fname)
-            return on_upload_main(rfs_fname)
-
     def consolidate_chunks(self):
         """
         Consolidate the chunks in the staging area.
 
         This method is called by `upload` if `consolidate_chunks` is True.
         """
         rfs = self._base_store.rfs
@@ -205,14 +146,53 @@
                     continue
                 consolidated_fname, new_offset = offset_maps[filename]
                 rfs['refs'][key] = [consolidated_fname, new_offset + old_offset, old_size]
             # remove the old files
             for fname in files:
                 os.remove(f"{root}/{fname}")
 
+    def copy_chunks_to_staging_area(self, *, download_remote: bool):
+        """
+        Copy the chunks in the base store to the staging area. This is done
+        in preparation for uploading to a storage system.
+
+        Parameters
+        ----------
+        download_remote : bool
+            If True, download the remote chunks to the staging area. If False,
+            just copy the local chunks.
+        """
+        if download_remote:
+            raise NotImplementedError("Downloading remote chunks not yet implemented")
+        rfs = self._base_store.rfs
+        templates = rfs.get('templates', {})
+        for k, v in rfs['refs'].items():
+            if isinstance(v, list) and len(v) == 3:
+                url = _apply_templates(v[0], templates)
+                if url.startswith('http://') or url.startswith('https://'):
+                    if download_remote:
+                        raise NotImplementedError("Downloading remote chunks not yet implemented")
+                    continue
+                elif url.startswith(self._staging_area.directory + '/'):
+                    # already in the staging area
+                    continue
+                else:
+                    # copy the local file to the staging area
+                    path0 = url
+                    chunk_data = _read_chunk_data(path0, v[1], v[2])
+                    stored_file_path = self._staging_area.store_file(k, chunk_data)
+                    self._set_ref_reference(k, stored_file_path, 0, v[2])
+
+
+def _apply_templates(x: str, templates: dict) -> str:
+    if '{{' in x and '}}' in x:
+        for key, val in templates.items():
+            x = x.replace('{{' + key + '}}', val)
+    return x
+
 
 def _sort_by_chunk_key(files: list) -> list:
     # first verify that all the files have the same number of parts
     num_parts = None
     for fname in files:
         parts = fname.split('.')
         if num_parts is None:
@@ -230,39 +210,11 @@
 
     def _chunk_key(fname: str) -> tuple:
         parts = fname.split('.')
         return tuple(int(p) for p in parts)
     return sorted(files, key=_chunk_key)
 
 
-def _upload_directory_of_blobs(
-    staging_dir: str,
-    on_upload_blob: UploadFileFunc
-) -> dict:
-    """
-    Upload all the files in a directory to a storage system and return a mapping
-    from the original file paths to the URLs of the uploaded files.
-    """
-    all_files = []
-    for root, dirs, files in os.walk(staging_dir):
-        for fname in files:
-            full_fname = f"{root}/{fname}"
-            all_files.append(full_fname)
-    blob_mapping = {}
-    for i, full_fname in enumerate(all_files):
-        relative_fname = full_fname[len(staging_dir):]
-        size_bytes = os.path.getsize(full_fname)
-        print(f'Uploading blob {i + 1} of {len(all_files)} {relative_fname} ({_format_size_bytes(size_bytes)})')
-        blob_url = on_upload_blob(full_fname)
-        blob_mapping[full_fname] = blob_url
-    return blob_mapping
-
-
-def _format_size_bytes(size_bytes: int) -> str:
-    if size_bytes < 1024:
-        return f"{size_bytes} bytes"
-    elif size_bytes < 1024 * 1024:
-        return f"{size_bytes / 1024:.1f} KB"
-    elif size_bytes < 1024 * 1024 * 1024:
-        return f"{size_bytes / 1024 / 1024:.1f} MB"
-    else:
-        return f"{size_bytes / 1024 / 1024 / 1024:.1f} GB"
+def _read_chunk_data(filename: str, offset: int, size: int) -> bytes:
+    with open(filename, "rb") as f:
+        f.seek(offset)
+        return f.read(size)
```

### Comparing `lindi-0.3.0/lindi/LindiStagingStore/StagingArea.py` & `lindi-0.3.1/lindi/LindiStagingStore/StagingArea.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Union
 import os
 import random
 import string
 import datetime
 import shutil
 
 
@@ -17,25 +18,35 @@
         """
         Do not call this constructor directly. Instead, use the `create` method
         to create a new staging area.
         """
         self._directory = os.path.abspath(_directory)
 
     @staticmethod
-    def create(base_dir: str) -> 'StagingArea':
+    def create(*, base_dir: Union[str, None] = None, dir: Union[str, None] = None) -> 'StagingArea':
         """
-        Create a new staging area.
+        Create a new staging area. Provide either `base_dir` or `dir`, but not
+        both.
 
         Parameters
         ----------
-        base_dir : str
-            The base directory where the staging area will be created. The
-            staging directory will be a subdirectory of this directory.
+        base_dir : str or None
+            If provided, the base directory where the staging area will be
+            created. The staging directory will be a subdirectory of this
+            directory.
+        dir : str or None
+            If provided, the exact directory where the staging area will be
+            created. It is okay if this directory already exists.
         """
-        dir = os.path.join(base_dir, _create_random_id())
+        if base_dir is not None and dir is not None:
+            raise ValueError("Provide either base_dir or dir, but not both")
+        if base_dir is not None:
+            dir = os.path.join(base_dir, _create_random_id())
+        if dir is None:
+            raise ValueError("Provide either base_dir or dir")
         return StagingArea(_directory=dir)
 
     def cleanup(self) -> None:
         """
         Clean up the staging area, deleting all files in it. This method is
         called automatically when the staging area is used as a context manager
         in a `with` statement.
```

### Comparing `lindi-0.3.0/lindi/conversion/attr_conversion.py` & `lindi-0.3.1/lindi/conversion/attr_conversion.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/conversion/create_zarr_dataset_from_h5_data.py` & `lindi-0.3.1/lindi/conversion/create_zarr_dataset_from_h5_data.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/conversion/decode_references.py` & `lindi-0.3.1/lindi/conversion/decode_references.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/conversion/h5_filters_to_codecs.py` & `lindi-0.3.1/lindi/conversion/h5_filters_to_codecs.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/conversion/h5_ref_to_zarr_attr.py` & `lindi-0.3.1/lindi/conversion/h5_ref_to_zarr_attr.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/lindi/conversion/nan_inf_ninf.py` & `lindi-0.3.1/lindi/conversion/nan_inf_ninf.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.0/pyproject.toml` & `lindi-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "lindi"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = [
     "Jeremy Magland <jmagland@flatironinstitute.org>",
     "Ryan Ly <rly@lbl.gov>",
     "Oliver Ruebel <oruebel@lbl.gov>"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numcodecs = "^0.12.1"
 zarr = "^2.16.1"
 h5py = "^3.10.0"
-remfile = "^0.1.9"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 pynwb = "^2.6.0"
 pytest = "^7.4.4"
 pytest-cov = "^4.1.0"
 ruff = "^0.3.3"
```

### Comparing `lindi-0.3.0/PKG-INFO` & `lindi-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: lindi
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: h5py (>=3.10.0,<4.0.0)
 Requires-Dist: numcodecs (>=0.12.1,<0.13.0)
-Requires-Dist: remfile (>=0.1.9,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: zarr (>=2.16.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # LINDI - Linked Data Interface
 
 [![latest-release](https://img.shields.io/pypi/v/lindi.svg)](https://pypi.org/project/lindi)
@@ -34,15 +33,15 @@
 
 - A specification for representing arbitrary HDF5 files as Zarr stores. This handles scalar datasets, references, soft links, and compound data types for datasets.
 - A Zarr wrapper for remote or local HDF5 files (LindiH5ZarrStore).
 - A mechanism for creating .lindi.json (or .nwb.lindi.json) files that reference data chunks in external files, inspired by [kerchunk](https://github.com/fsspec/kerchunk).
 - An h5py-like interface for reading from and writing to these data sources that can be used with [pynwb](https://pynwb.readthedocs.io/en/stable/).
 - A mechanism for uploading and downloading these data sources to and from cloud storage, including DANDI.
 
-This project was inspired by [kerchunk](https://github.com/fsspec/kerchunk) and [hdmf-zarr](https://hdmf-zarr.readthedocs.io/en/latest/index.html) and depends on [zarr](https://zarr.readthedocs.io/en/stable/), [h5py](https://www.h5py.org/), [remfile](https://github.com/magland/remfile) and [numcodecs](https://numcodecs.readthedocs.io/en/stable/).
+This project was inspired by [kerchunk](https://github.com/fsspec/kerchunk) and [hdmf-zarr](https://hdmf-zarr.readthedocs.io/en/latest/index.html) and depends on [zarr](https://zarr.readthedocs.io/en/stable/), [h5py](https://www.h5py.org/) and [numcodecs](https://numcodecs.readthedocs.io/en/stable/).
 
 ## Installation
 
 ```bash
 pip install lindi
 ```
 
@@ -51,60 +50,77 @@
 ```bash
 cd lindi
 pip install -e .
 ```
 
 ## Use cases
 
+* Lazy-load a remote NWB/HDF5 file for efficient access to metadata and data.
 * Represent a remote NWB/HDF5 file as a .nwb.lindi.json file.
 * Read a local or remote .nwb.lindi.json file using pynwb or other tools.
 * Edit a .nwb.lindi.json file using pynwb or other tools.
 * Add datasets to a .nwb.lindi.json file using a local staging area.
-* Upload a .nwb.lindi.json file to a cloud storage service such as DANDI.
+* Upload a .nwb.lindi.json file with staged datasets to a cloud storage service such as DANDI.
+
+### Lazy-load a remote NWB/HDF5 file for efficient access to metadata and data
+
+```python
+import pynwb
+import lindi
+
+# URL of the remote NWB file
+h5_url = "https://api.dandiarchive.org/api/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/download/"
+
+# Set up a local cache
+local_cache = lindi.LocalCache(cache_dir='lindi_cache')
+
+# Create the h5py-like client
+client = lindi.LindiH5pyFile.from_hdf5_file(h5_url, local_cache=local_cache)
+
+# Open using pynwb
+with pynwb.NWBHDF5IO(file=client, mode="r") as io:
+    nwbfile = io.read()
+    print(nwbfile)
+
+# The downloaded data will be cached locally, so subsequent reads will be faster
+```
 
 ### Represent a remote NWB/HDF5 file as a .nwb.lindi.json file
 
 ```python
 import json
-import pynwb
 import lindi
 
 # URL of the remote NWB file
 h5_url = "https://api.dandiarchive.org/api/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/download/"
 
-# Create a read-only Zarr store as a wrapper for the h5 file
-store = lindi.LindiH5ZarrStore.from_file(h5_url)
+# Create the h5py-like client
+client = lindi.LindiH5pyFile.from_hdf5_file(h5_url)
 
 # Generate a reference file system
-rfs = store.to_reference_file_system()
+rfs = client.to_reference_file_system()
 
 # Save it to a file for later use
 with open("example.lindi.json", "w") as f:
     json.dump(rfs, f, indent=2)
 
-# Create an h5py-like client from the reference file system
-client = lindi.LindiH5pyFile.from_reference_file_system(rfs)
-
-# Open using pynwb
-with pynwb.NWBHDF5IO(file=client, mode="r") as io:
-    nwbfile = io.read()
-    print(nwbfile)
+# See the next example for how to read this file
 ```
 
 ### Read a local or remote .nwb.lindi.json file using pynwb or other tools
 
 ```python
 import pynwb
 import lindi
 
 # URL of the remote .nwb.lindi.json file
 url = 'https://kerchunk.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
 
-# Load the h5py-like client for the reference file system
-client = lindi.LindiH5pyFile.from_reference_file_system(url)
+# Load the h5py-like client
+client = lindi.LindiH5pyFile.from_lindi_file(url)
 
 # Open using pynwb
 with pynwb.NWBHDF5IO(file=client, mode="r") as io:
     nwbfile = io.read()
     print(nwbfile)
 ```
 
@@ -137,24 +153,24 @@
 
 # URL of the remote .nwb.lindi.json file
 url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
 
 # Load the h5py-like client for the reference file system
 # in read-write mode with a staging area
 with lindi.StagingArea.create(base_dir='lindi_staging') as staging_area:
-    client = lindi.LindiH5pyFile.from_reference_file_system(
+    client = lindi.LindiH5pyFile.from_lindi_file(
         url,
         mode="r+",
         staging_area=staging_area
     )
     # add datasets to client using pynwb or other tools
     # upload the changes to the remote .nwb.lindi.json file
 ```
 
-### Upload a .nwb.lindi.json file to a cloud storage service such as DANDI
+### Upload a .nwb.lindi.json file with staged datasets to a cloud storage service such as DANDI
 
 See [this example](https://github.com/magland/lindi-dandi/blob/main/devel/lindi_test_2.py).
 
 ## For developers
 
 [Special Zarr annotations used by LINDI](docs/special_zarr_annotations.md)
```

