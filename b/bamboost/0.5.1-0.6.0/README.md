# Comparing `tmp/bamboost-0.5.1.tar.gz` & `tmp/bamboost-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/florez/work/code/bamboost/dist/.tmp-4t89408s/bamboost-0.5.1.tar", last modified: Wed Mar  6 08:42:10 2024, max compression
+gzip compressed data, was "bamboost-0.6.0.tar", last modified: Thu Apr 25 22:26:45 2024, max compression
```

## Comparing `bamboost-0.5.1.tar` & `bamboost-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,57 @@
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-03-06 08:42:10.939704 bamboost-0.5.1/
--rw-r--r--   0 florez    (1000) florez    (1000)     1060 2024-01-29 08:07:36.000000 bamboost-0.5.1/LICENSE
--rw-r--r--   0 florez    (1000) florez    (1000)       62 2024-03-05 17:53:33.000000 bamboost-0.5.1/MANIFEST.in
--rw-r--r--   0 florez    (1000) florez    (1000)    13793 2024-03-06 08:42:10.939704 bamboost-0.5.1/PKG-INFO
--rw-r--r--   0 florez    (1000) florez    (1000)    11755 2024-03-05 17:53:33.000000 bamboost-0.5.1/README.md
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-03-06 08:42:10.936370 bamboost-0.5.1/bamboost/
--rw-r--r--   0 florez    (1000) florez    (1000)      489 2024-03-06 08:41:32.000000 bamboost-0.5.1/bamboost/__init__.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-03-06 08:42:10.939704 bamboost-0.5.1/bamboost/accessors/
--rw-r--r--   0 florez    (1000) florez    (1000)       67 2024-03-05 17:53:33.000000 bamboost-0.5.1/bamboost/accessors/__init__.py
--rw-r--r--   0 florez    (1000) florez    (1000)     6210 2024-03-06 08:14:53.000000 bamboost-0.5.1/bamboost/accessors/fielddata.py
--rw-r--r--   0 florez    (1000) florez    (1000)      932 2024-03-05 17:53:33.000000 bamboost-0.5.1/bamboost/accessors/globals.py
--rw-r--r--   0 florez    (1000) florez    (1000)     1481 2024-03-06 08:41:32.000000 bamboost-0.5.1/bamboost/accessors/meshes.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-03-06 08:42:10.939704 bamboost-0.5.1/bamboost/common/
--rw-r--r--   0 florez    (1000) florez    (1000)      181 2024-03-06 08:31:51.000000 bamboost-0.5.1/bamboost/common/__init__.py
--rw-r--r--   0 florez    (1000) florez    (1000)     3045 2024-03-05 18:19:15.000000 bamboost-0.5.1/bamboost/common/_mock_mpi.py
--rw-r--r--   0 florez    (1000) florez    (1000)     5291 2024-03-06 08:31:51.000000 bamboost-0.5.1/bamboost/common/file_handler.py
--rw-r--r--   0 florez    (1000) florez    (1000)     1474 2024-03-05 17:53:33.000000 bamboost-0.5.1/bamboost/common/git_utility.py
--rw-r--r--   0 florez    (1000) florez    (1000)     8985 2024-03-06 08:31:51.000000 bamboost-0.5.1/bamboost/common/hdf_pointer.py
--rw-r--r--   0 florez    (1000) florez    (1000)     3432 2024-03-06 08:33:52.000000 bamboost-0.5.1/bamboost/common/job.py
--rw-r--r--   0 florez    (1000) florez    (1000)      899 2024-03-06 08:41:32.000000 bamboost-0.5.1/bamboost/common/mpi.py
--rw-r--r--   0 florez    (1000) florez    (1000)     3618 2024-03-05 17:53:33.000000 bamboost-0.5.1/bamboost/common/utilities.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-03-06 08:42:10.939704 bamboost-0.5.1/bamboost/html/
--rw-r--r--   0 florez    (1000) florez    (1000)     3771 2024-03-05 17:53:33.000000 bamboost-0.5.1/bamboost/html/hdf5_group.html
--rw-r--r--   0 florez    (1000) florez    (1000)    58161 2024-03-05 17:53:33.000000 bamboost-0.5.1/bamboost/html/icon.png
--rw-r--r--   0 florez    (1000) florez    (1000)    77548 2024-03-05 17:53:33.000000 bamboost-0.5.1/bamboost/html/icon.txt
--rw-r--r--   0 florez    (1000) florez    (1000)     1353 2024-03-05 17:53:33.000000 bamboost-0.5.1/bamboost/html/manager.html
--rw-r--r--   0 florez    (1000) florez    (1000)     3471 2024-03-05 17:53:33.000000 bamboost-0.5.1/bamboost/html/simulation.html
--rw-r--r--   0 florez    (1000) florez    (1000)     5119 2024-03-05 17:53:33.000000 bamboost-0.5.1/bamboost/index.py
--rw-r--r--   0 florez    (1000) florez    (1000)    17649 2024-03-06 08:41:32.000000 bamboost-0.5.1/bamboost/manager.py
--rw-r--r--   0 florez    (1000) florez    (1000)    16498 2024-03-06 08:41:32.000000 bamboost-0.5.1/bamboost/simulation.py
--rw-r--r--   0 florez    (1000) florez    (1000)    11098 2024-03-06 08:41:32.000000 bamboost-0.5.1/bamboost/simulation_writer.py
--rw-r--r--   0 florez    (1000) florez    (1000)     6388 2024-03-06 08:41:32.000000 bamboost-0.5.1/bamboost/xdmf.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-03-06 08:42:10.939704 bamboost-0.5.1/bamboost.egg-info/
--rw-r--r--   0 florez    (1000) florez    (1000)    13793 2024-03-06 08:42:10.000000 bamboost-0.5.1/bamboost.egg-info/PKG-INFO
--rw-r--r--   0 florez    (1000) florez    (1000)      886 2024-03-06 08:42:10.000000 bamboost-0.5.1/bamboost.egg-info/SOURCES.txt
--rw-r--r--   0 florez    (1000) florez    (1000)        1 2024-03-06 08:42:10.000000 bamboost-0.5.1/bamboost.egg-info/dependency_links.txt
--rw-r--r--   0 florez    (1000) florez    (1000)       89 2024-03-06 08:42:10.000000 bamboost-0.5.1/bamboost.egg-info/requires.txt
--rw-r--r--   0 florez    (1000) florez    (1000)        9 2024-03-06 08:42:10.000000 bamboost-0.5.1/bamboost.egg-info/top_level.txt
--rw-r--r--   0 florez    (1000) florez    (1000)     1019 2024-03-06 08:31:51.000000 bamboost-0.5.1/pyproject.toml
--rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-03-06 08:42:10.939704 bamboost-0.5.1/setup.cfg
--rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-02-02 10:38:32.000000 bamboost-0.5.1/setup.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-03-06 08:42:10.939704 bamboost-0.5.1/tests/
--rw-r--r--   0 florez    (1000) florez    (1000)     1247 2024-03-06 08:29:02.000000 bamboost-0.5.1/tests/test_manager.py
--rw-r--r--   0 florez    (1000) florez    (1000)       64 2024-03-05 17:46:44.000000 bamboost-0.5.1/tests/test_reader.py
--rw-r--r--   0 florez    (1000) florez    (1000)     3324 2024-03-05 17:53:33.000000 bamboost-0.5.1/tests/test_writer.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-25 22:26:45.369233 bamboost-0.6.0/
+-rw-r--r--   0 florez    (1000) florez    (1000)     1060 2024-01-29 08:07:36.000000 bamboost-0.6.0/LICENSE
+-rw-r--r--   0 florez    (1000) florez    (1000)       62 2024-03-05 17:53:33.000000 bamboost-0.6.0/MANIFEST.in
+-rw-r--r--   0 florez    (1000) florez    (1000)    13793 2024-04-25 22:26:45.369233 bamboost-0.6.0/PKG-INFO
+-rw-r--r--   0 florez    (1000) florez    (1000)    11755 2024-03-05 17:53:33.000000 bamboost-0.6.0/README.md
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-25 22:26:45.365899 bamboost-0.6.0/bamboost/
+-rw-r--r--   0 florez    (1000) florez    (1000)      552 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/__init__.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     2421 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/_config.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     5057 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/_sqlite_database.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-25 22:26:45.365899 bamboost-0.6.0/bamboost/accessors/
+-rw-r--r--   0 florez    (1000) florez    (1000)       78 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/accessors/__init__.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     6456 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/accessors/fielddata.py
+-rw-r--r--   0 florez    (1000) florez    (1000)      932 2024-03-05 17:53:33.000000 bamboost-0.6.0/bamboost/accessors/globals.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     1570 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/accessors/meshes.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-25 22:26:45.365899 bamboost-0.6.0/bamboost/common/
+-rw-r--r--   0 florez    (1000) florez    (1000)      181 2024-04-17 13:09:34.000000 bamboost-0.6.0/bamboost/common/__init__.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     3045 2024-04-17 13:09:34.000000 bamboost-0.6.0/bamboost/common/_mock_mpi.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     5291 2024-04-17 13:09:34.000000 bamboost-0.6.0/bamboost/common/file_handler.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     1474 2024-03-05 17:53:33.000000 bamboost-0.6.0/bamboost/common/git_utility.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     8985 2024-04-17 13:09:34.000000 bamboost-0.6.0/bamboost/common/hdf_pointer.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     3553 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/common/job.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     1075 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/common/mpi.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     5902 2024-04-25 21:48:38.000000 bamboost-0.6.0/bamboost/common/utilities.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-25 22:26:45.365899 bamboost-0.6.0/bamboost/extensions/
+-rw-r--r--   0 florez    (1000) florez    (1000)      754 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/extensions/__init__.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     7332 2024-04-25 21:44:53.000000 bamboost-0.6.0/bamboost/extensions/fenics.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     8381 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/extensions/remote_manager.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     2352 2024-04-25 22:03:07.000000 bamboost-0.6.0/bamboost/extensions/slurm.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-25 22:26:45.369233 bamboost-0.6.0/bamboost/html/
+-rw-r--r--   0 florez    (1000) florez    (1000)     3741 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/html/hdf5_group.html
+-rw-r--r--   0 florez    (1000) florez    (1000)    58161 2024-03-05 17:53:33.000000 bamboost-0.6.0/bamboost/html/icon.png
+-rw-r--r--   0 florez    (1000) florez    (1000)    77548 2024-03-05 17:53:33.000000 bamboost-0.6.0/bamboost/html/icon.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)     1353 2024-03-05 17:53:33.000000 bamboost-0.6.0/bamboost/html/manager.html
+-rw-r--r--   0 florez    (1000) florez    (1000)     3471 2024-03-05 17:53:33.000000 bamboost-0.6.0/bamboost/html/simulation.html
+-rw-r--r--   0 florez    (1000) florez    (1000)    19535 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/index.py
+-rw-r--r--   0 florez    (1000) florez    (1000)    20664 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/manager.py
+-rw-r--r--   0 florez    (1000) florez    (1000)    19113 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/simulation.py
+-rw-r--r--   0 florez    (1000) florez    (1000)    11163 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/simulation_writer.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     6577 2024-04-25 22:22:13.000000 bamboost-0.6.0/bamboost/xdmf.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-25 22:26:45.369233 bamboost-0.6.0/bamboost.egg-info/
+-rw-r--r--   0 florez    (1000) florez    (1000)    13793 2024-04-25 22:26:45.000000 bamboost-0.6.0/bamboost.egg-info/PKG-INFO
+-rw-r--r--   0 florez    (1000) florez    (1000)     1147 2024-04-25 22:26:45.000000 bamboost-0.6.0/bamboost.egg-info/SOURCES.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)        1 2024-04-25 22:26:45.000000 bamboost-0.6.0/bamboost.egg-info/dependency_links.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)       41 2024-04-25 22:26:45.000000 bamboost-0.6.0/bamboost.egg-info/entry_points.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)       89 2024-04-25 22:26:45.000000 bamboost-0.6.0/bamboost.egg-info/requires.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)       13 2024-04-25 22:26:45.000000 bamboost-0.6.0/bamboost.egg-info/top_level.txt
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-25 22:26:45.369233 bamboost-0.6.0/cli/
+-rw-r--r--   0 florez    (1000) florez    (1000)       64 2024-04-25 22:22:13.000000 bamboost-0.6.0/cli/__init__.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     4413 2024-04-25 22:22:13.000000 bamboost-0.6.0/cli/main.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     1099 2024-04-25 22:22:13.000000 bamboost-0.6.0/pyproject.toml
+-rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-04-25 22:26:45.369233 bamboost-0.6.0/setup.cfg
+-rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-02-02 10:38:32.000000 bamboost-0.6.0/setup.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-25 22:26:45.369233 bamboost-0.6.0/tests/
+-rw-r--r--   0 florez    (1000) florez    (1000)     4643 2024-04-25 22:22:13.000000 bamboost-0.6.0/tests/test_index.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     3200 2024-04-25 22:22:13.000000 bamboost-0.6.0/tests/test_manager.py
+-rw-r--r--   0 florez    (1000) florez    (1000)      502 2024-04-25 22:22:13.000000 bamboost-0.6.0/tests/test_reader.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     3324 2024-04-17 13:14:35.000000 bamboost-0.6.0/tests/test_writer.py
```

### Comparing `bamboost-0.5.1/LICENSE` & `bamboost-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/PKG-INFO` & `bamboost-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamboost
-Version: 0.5.1
+Version: 0.6.0
 Summary: A light weight database manager using HDF5
 Author-email: Flavio Lorez <florez@ethz.ch>
 License: Copyright (c) 2023 CMBM, ETH Zurich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bamboost Version: 0.5.1 Summary: A light weight
+Metadata-Version: 2.1 Name: bamboost Version: 0.6.0 Summary: A light weight
 database manager using HDF5 Author-email: Flavio Lorez
 ethz.ch> License: Copyright (c) 2023 CMBM, ETH Zurich Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `bamboost-0.5.1/README.md` & `bamboost-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/bamboost/accessors/fielddata.py` & `bamboost-0.6.0/bamboost/accessors/fielddata.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,20 +90,25 @@
         self._name = path_to_data.split("/")[-1]
 
     @with_file_open("r")
     def __getitem__(self, key) -> np.ndarray:
         return self._get_full_data()[key]
 
     def _get_full_data(self) -> h5py.Dataset:
-        try:
+        if self._vds_key not in self.keys():
+            self._create_vds()
             return self.obj[self._vds_key]
-        except KeyError:
+
+        if len(self) > self.obj.attrs.get("virtual_dataset_length", 0):
             self._create_vds()
+            self._create_times()
             return self.obj[self._vds_key]
 
+        return self.obj[self._vds_key]
+
     @with_file_open("r")
     def __len__(self) -> int:
         non_field_keys = set({self._vds_key, self._times_key})
         return len(self.keys() - non_field_keys)
 
     @property
     @with_file_open("r")
@@ -201,8 +206,9 @@
             for step in range(length):
                 vsource = h5py.VirtualSource(self.obj[str(step)])
                 layout[step] = vsource
 
         with self._file("r+"):
             if self._vds_key in self.obj.keys():
                 del self.obj[self._vds_key]
+            self.obj.attrs["virtual_dataset_length"] = length
             self.obj.create_virtual_dataset(self._vds_key, layout)
```

### Comparing `bamboost-0.5.1/bamboost/accessors/globals.py` & `bamboost-0.6.0/bamboost/accessors/globals.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/bamboost/accessors/meshes.py` & `bamboost-0.6.0/bamboost/accessors/meshes.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,15 +41,18 @@
 class Mesh(hdf_pointer.Group):
     def __init__(self, file_handler: FileHandler, path_to_data: str) -> None:
         super().__init__(file_handler, path_to_data)
 
     @property
     @with_file_open("r")
     def coordinates(self):
-        return self.obj["geometry"][()]
+        try:
+            return self.obj["geometry"][()]
+        except KeyError:
+            return self.obj["coordinates"][()]
 
     @property
     @with_file_open("r")
     def connectivity(self):
         return self.obj["topology"][()]
 
     @with_file_open("r")
```

### Comparing `bamboost-0.5.1/bamboost/common/_mock_mpi.py` & `bamboost-0.6.0/bamboost/common/_mock_mpi.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/bamboost/common/file_handler.py` & `bamboost-0.6.0/bamboost/common/file_handler.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/bamboost/common/git_utility.py` & `bamboost-0.6.0/bamboost/common/git_utility.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/bamboost/common/hdf_pointer.py` & `bamboost-0.6.0/bamboost/common/hdf_pointer.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/bamboost/common/job.py` & `bamboost-0.6.0/bamboost/common/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 # Copyright 2023 Flavio Lorez and contributors
 #
 # There is no warranty for this code
 
 import argparse
 import os
 
+from bamboost._config import paths
+
 __all__ = ["Job"]
 
 
 class Job:
     def __init__(self):
         pass
 
     def create_sbatch_script(
         self,
         commands: list,
         path: str,
         uid: str = None,
+        db_id: str = None,
         nnodes: int = 1,
         ntasks: int = 4,
         ncpus: int = 1,
         time: str = "04:00:00",
         mem_per_cpu: int = 2048,
         tmp: int = 8000,
     ) -> None:
@@ -49,15 +52,16 @@
         script += f"#SBATCH --job-name={uid}\n"
         script += f"#SBATCH --mem-per-cpu={mem_per_cpu}\n"
         if tmp:
             script += f"#SBATCH --tmp={tmp}\n"
         script += f"#SBATCH --output={os.path.join(path, uid)}/{uid}.out\n"
 
         # add SCRIPT_DIR as environment variable
-        script += 'SCRIPT_DIR=$( cd -- "$( dirname -- "${BASH_SOURCE[0]}" )" &> /dev/null && pwd )\n\n'
+        script += f"""path=$(sqlite3 {paths['DATABASE_FILE']} "SELECT path FROM dbindex WHERE id='{db_id}'")\n"""
+        script += f"SCRIPT_DIR=$path/{uid}\n\n"
 
         # user defined commands
         script += "\n"
         for cmd in commands:
             script += cmd.format(MPI=mpicommand) + "\n"
 
         # write to submission file
```

### Comparing `bamboost-0.5.1/bamboost/common/mpi.py` & `bamboost-0.6.0/bamboost/common/mpi.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,26 +8,36 @@
 # There is no warranty for this code
 import logging
 import os
 from typing import Any, Union
 
 log = logging.getLogger(__name__)
 
+from bamboost._config import config
+
 from ._mock_mpi import MockMPI
 
-MPI_ON: bool = False if os.environ.get("BAMBOOST_NO_MPI", "0") == "1" else True
-"""Indicates the use of `mpi4py.MPI`. If `False`, the `MockMPI` class is used
-instead. Is set by reading the environment variable `BAMBOOST_NO_MPI` [0 or 1].
+MPIType = Union[MockMPI, Any]
+
+MPI_ON = config.get("options", {}).get("mpi", True)
+ENV_BAMBOOST_MPI: bool = os.environ.get("BAMBOOST_MPI", None)
+"""Indicates the use of `mpi4py.MPI`. If `0`, the `MockMPI` class is used
+instead. Is set by reading the environment variable `BAMBOOST_MPI` [0 or 1].
 """
+if ENV_BAMBOOST_MPI is not None:
+    MPI_ON = ENV_BAMBOOST_MPI == "1"
+
 
 def _get_mpi_module():
     if not MPI_ON:
         return MockMPI
 
     try:
         from mpi4py import MPI
+
         return MPI
     except ImportError:
-        log.warning("MPI is not available, using MockMPI")
+        log.info("`mpi4py` unavailable [using a mock MPI module]")
         return MockMPI
 
+
 MPI: Union[MockMPI, Any] = _get_mpi_module()
```

### Comparing `bamboost-0.5.1/bamboost/html/hdf5_group.html` & `bamboost-0.6.0/bamboost/html/hdf5_group.html`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,14 @@
         background-color: var(--bb-bg50);
       }
 
       .jp-RenderedHTMLCommon tbody tr:hover {
         background-color: var(--bb-bg50);
       }
 
-      table th {
-        font-style: italic;
-        background-color: var(--bb-bg50);
-      }
-
       .info_container {
         position: relative;
         display: inline-flex;
         justify-content: flex-start;
         gap: 1.5rem;
         align-items: flex-start;
         height: 100%;
@@ -102,14 +97,20 @@
         padding: var(--head-padding);
         font-style: normal;
         font-size: larger;
         font-weight: bold;
         text-align: right;
         background-color: transparent;
       }
+
+      table.content-table th {
+        font-style: italic;
+        background-color: var(--bb-bg50);
+      }
+
     </style>
   </head>
 
   <body>
     <div class="info_container">
       <div class="name-logo">
         <div class="first-col-header">
@@ -117,26 +118,24 @@
           <div id="title">$NAME</div>
         </div>
         <div class="logobox">
           <img class="logo" src="data:image/png;base64,$ICON" alt="Icon" />
           <div>bamboost $version</div>
         </div>
       </div>
-      <div class="content-table">
-        <table>
-          <tbody>
-            <th colspan="2" class="head">Attributes</th>
-            <tr>
-              <th>Attribute</th>
-              <th>Value</th>
-            </tr>
-            $attrs
-          </tbody>
-        </table>
-      </div>
+      <table class="content-table">
+        <tbody>
+          <th colspan="2" class="head">Attributes</th>
+          <tr>
+            <th>Attribute</th>
+            <th>Value</th>
+          </tr>
+          $attrs
+        </tbody>
+      </table>
       <table class="content-table">
         <tbody>
           <th colspan="2" class="head">Groups</th>
           <tr>
             <th>Name</th>
             <th>Members</th>
           </tr>
```

### Comparing `bamboost-0.5.1/bamboost/html/icon.png` & `bamboost-0.6.0/bamboost/html/icon.png`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/bamboost/html/icon.txt` & `bamboost-0.6.0/bamboost/html/icon.txt`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/bamboost/html/manager.html` & `bamboost-0.6.0/bamboost/html/manager.html`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/bamboost/html/simulation.html` & `bamboost-0.6.0/bamboost/html/simulation.html`

 * *Files identical despite different names*

### Comparing `bamboost-0.5.1/bamboost/manager.py` & `bamboost-0.6.0/bamboost/manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,67 +11,61 @@
 import logging
 import numbers
 import os
 import pkgutil
 import shutil
 import uuid
 from ctypes import ArgumentError
-from typing import Union
+from typing import Generator, Union
 
 import h5py
 import pandas as pd
 
+
+# forward declaration
+class Manager:
+    pass
+
+
 from . import index
 from .common.file_handler import open_h5file
 from .common.mpi import MPI
+from .index import DatabaseTable, IndexAPI, config
 from .simulation import Simulation
 from .simulation_writer import SimulationWriter
 
 __all__ = ["Manager", "ManagerFromUID", "ManagerFromName"]
 
 log = logging.getLogger(__name__)
 
 
-META_INFO = """
-This database has been created using `bamboost`, a python package developed at
-the CMBM group of ETH zurich. It has been built for data management using the
-HDF5 file format.
-
-https://gitlab.ethz.ch/compmechmat/research/libs/dbmanager
-"""
-
-# Setup Manager getters
-# ---------------------
-
-
 class ManagerFromUID(object):
     """Get a database by its UID. This is used for autocompletion in ipython."""
 
     def __init__(self) -> None:
-        ids = index.get_index_dict()
+        # or [] to circumvent Null type (MPI)
+        ids = IndexAPI().fetch(f"SELECT id, path FROM dbindex") or []
         self.completion_keys = tuple(
-            [
-                f'{key} - {"..."+val[-25:] if len(val)>=25 else val}'
-                for key, val in ids.items()
-            ]
+            [f'{key} - {"..."+val[-25:] if len(val)>=25 else val}' for key, val in ids]
         )
 
     def _ipython_key_completions_(self):
         return self.completion_keys
 
     def __getitem__(self, key) -> Manager:
         key = key.split()[0]  # take only uid
         return Manager(uid=key, create_if_not_exist=False)
 
 
 class ManagerFromName(object):
     """Get a database by its path/name. This is used for autocompletion in ipython."""
 
     def __init__(self) -> None:
-        self.completion_keys = tuple(index.get_index_dict().values())
+        paths = IndexAPI().fetch("SELECT path FROM dbindex") or []
+        self.completion_keys = tuple(paths)
 
     def _ipython_key_completions_(self):
         return self.completion_keys
 
     def __getitem__(self, key) -> Manager:
         return Manager(key, create_if_not_exist=False)
 
@@ -86,43 +80,57 @@
         uid: UID of the database
 
     Attributes:
         FIX_DF: If False, the dataframe of the database is reconstructed every
             time it is accessed.
         fromUID: Access a database by its UID
         fromName: Access a database by its path/name
+
+    Example:
+        >>> db = Manager("path/to/db")
+        >>> db.df # DataFrame of the database
     """
 
     FIX_DF = True
     fromUID: ManagerFromUID = ManagerFromUID()
     fromName: ManagerFromName = ManagerFromName()
 
     def __init__(
         self,
         path: str = None,
         comm: MPI.Comm = MPI.COMM_WORLD,
         uid: str = None,
         create_if_not_exist: bool = True,
     ):
+        # provided uid has precedence
         if uid is not None:
-            path = index.get_path(uid.upper())
+            path = self._index.get_path(uid.upper())
+            path = comm.bcast(path, root=0)
         self.path = path
         self.comm = comm
 
         # check if path exists
         if not os.path.isdir(path):
             if not create_if_not_exist:
                 raise NotADirectoryError("Specified path is not a valid path.")
             log.info(f"Created new database ({path})")
             self._make_new(path)
-        self.UID = self._retrieve_uid()
-        # self._store_uid_in_index()
-        self._all_uids = self._get_uids()
-        self._dataframe: pd.DataFrame = None
-        self._meta_folder = os.path.join(path, ".database")
+
+        # retrieve the UID of the database from the id file
+        # if not found, a new one is generated
+        self.UID = uid or self._retrieve_uid()
+
+        # Update the SQL table for the database
+        try:
+            with self._index.open():
+                self._index.insert_path(self.UID, self.path)
+                self._table.create_database_table()
+                self._table.sync()
+        except index.Error as e:
+            log.warning(f"index error: {e}")
 
     def __getitem__(self, key: Union[str, int]) -> Simulation:
         """Returns the simulation in the specified row of the dataframe.
 
         Args:
             key: The simulation identifier (`str`) or the row index (`int`).
         Returns:
@@ -145,26 +153,38 @@
             .replace("$db_uid", self.UID)
             .replace("$db_size", str(len(self)))
         )
 
     def __len__(self) -> int:
         return len(self.all_uids)
 
-    def __iter__(self) -> Simulation:
+    def __iter__(self) -> Generator[Simulation]:
         for sim in self.sims():
             yield sim
 
     def _ipython_key_completions_(self):
         return self.all_uids
 
+    @property
+    def _index(self) -> IndexAPI:
+        """The index which contains this database."""
+        return IndexAPI()
+
+    @property
+    def _table(self) -> DatabaseTable:
+        """The table in the sql database for this database."""
+        return self._index.get_database_table(self.UID)
+
     def _retrieve_uid(self) -> str:
         """Get the UID of this database from the file tree."""
-        for file in os.listdir(self.path):
-            if file.startswith(".BAMBOOST"):
-                return file.split("-")[1]
+        try:
+            return index.get_uid_from_path(self.path)
+        except FileNotFoundError:
+            pass
+
         log.warning("Database exists but no UID found. Generating new UID.")
         return self._make_new(self.path)
 
     def _make_new(self, path) -> str:
         """Initialize a new database."""
         from datetime import datetime
 
@@ -174,73 +194,137 @@
         # Assign a unique id to the database
         self.UID = f"{uuid.uuid4().hex[:10]}".upper()
         uid_file = os.path.join(path, f".BAMBOOST-{self.UID}")
         with open(uid_file, "a") as f:
             f.write(self.UID + "\n")
             f.write(f'Date of creation: {datetime.now().strftime("%d/%m/%Y %H:%M:%S")}')
         os.chmod(uid_file, 0o444)  # read only for uid file
+
         log.info(f"Registered new database (uid = {self.UID})")
-        self._store_uid_in_index()
+        self._index.insert_path(self.UID, path)
         return self.UID
 
-    def _store_uid_in_index(self) -> None:
-        """Stores the UID of this database with the current path."""
-        index.record_database(self.UID, os.path.abspath(self.path))
-
-    def _init_meta_folder(self) -> None:
-        os.makedirs(self._meta_folder, exist_ok=True)
-        with open(os.path.join(self._meta_folder, "README.txt"), "w") as f:
-            f.write(META_INFO)
-
     @property
-    def all_uids(self) -> set:
-        if self.FIX_DF:
-            return self._all_uids
-        return self._get_uids()
+    def all_uids(self) -> list:
+        if not self.FIX_DF or not hasattr(self, "_all_uids"):
+            self._all_uids = self._get_uids()
+        return self._all_uids
+
+    @all_uids.setter
+    def all_uids(self, value: set | list):
+        self._all_uids = value
+
+    def _get_uids(self) -> list:
+        """Get all simulation names in the database."""
+        all_uids = list()
+        for dir in os.listdir(self.path):
+            if not os.path.isdir(os.path.join(self.path, dir)):
+                continue
+            if any(
+                [i.endswith(".h5") for i in os.listdir(os.path.join(self.path, dir))]
+            ):
+                all_uids.append(dir)
+        return all_uids
 
     @property
     def df(self) -> pd.DataFrame:
         """View of the database and its parametric space.
 
         Returns:
             :class:`pd.DataFrame`
         """
+        if not hasattr(self, "_dataframe"):
+            return self.get_view()
         if self.FIX_DF and self._dataframe is not None:
             return self._dataframe
         return self.get_view()
 
+    def _get_parameters_for_uid(
+        self, uid: str, include_linked_sims: bool = False
+    ) -> dict:
+        """Get the parameters for a given uid.
+
+        Args:
+            uid (`str`): uid of the simulation
+            include_linked_sims (`bool`): if True, include the parameters of linked sims
+        """
+        h5file_for_uid = os.path.join(self.path, uid, f"{uid}.h5")
+        tmp_dict = dict()
+
+        with open_h5file(h5file_for_uid, "r") as f:
+            if "parameters" in f.keys():
+                tmp_dict.update(f["parameters"].attrs)
+            if "additionals" in f.keys():
+                tmp_dict.update({"additionals": dict(f["additionals"].attrs)})
+            tmp_dict.update(f.attrs)
+
+        if include_linked_sims:
+            for linked, full_uid in self.sim(uid).links.attrs.items():
+                sim = Simulation.fromUID(full_uid)
+                tmp_dict.update(
+                    {f"{linked}.{key}": val for key, val in sim.parameters.items()}
+                )
+        return tmp_dict
+
     def get_view(self, include_linked_sims: bool = False) -> pd.DataFrame:
-        """View of the database and its parametric space.
+        """View of the database and its parametric space. Read from the sql
+        database. If `include_linked_sims` is True, the individual h5 files are
+        scanned.
 
         Args:
             include_linked_sims: if True, include the parameters of linked sims
 
-        Returns:
-            :class:`pd.DataFrame`
+        Examples:
+            >>> db.get_view()
+            >>> db.get_view(include_linked_sims=True)
         """
-        all_uids = self.all_uids
+        if include_linked_sims:
+            return self.get_view_from_hdf_files(include_linked_sims=include_linked_sims)
+
+        try:
+            with self._table.open():
+                self._table.sync()
+                df = self._table.read_table()
+        except index.Error as e:
+            log.warning(f"index error: {e}")
+            return self.get_view_from_hdf_files(include_linked_sims=include_linked_sims)
+
+        if df.empty:
+            return df
+        df["time_stamp"] = pd.to_datetime(df["time_stamp"])
+
+        # Sort dataframe columns
+        columns_start = ["id", "notes", "status", "time_stamp"]
+        self._dataframe = df[[*columns_start, *df.columns.difference(columns_start)]]
+
+        opts = config.get("options", {})
+        if "sort_table_key" in opts:
+            self._dataframe.sort_values(
+                opts.get("sort_table_key", "id"),
+                ascending=opts.get("sort_table_order", "asc") == "asc",
+                inplace=True,
+            )
+        return self._dataframe
+
+    def get_view_from_hdf_files(
+        self, include_linked_sims: bool = False
+    ) -> pd.DataFrame:
+        """View of the database and its parametric space. Read from the h5
+        files metadata.
+
+        Args:
+            include_linked_sims: if True, include the parameters of linked sims
+        """
+        all_uids = self._get_uids()
         data = list()
 
         for uid in all_uids:
-            h5file_for_uid = os.path.join(self.path, uid, f"{uid}.h5")
-            tmp_dict = dict()
-
-            with open_h5file(h5file_for_uid, "r") as f:
-                if "parameters" in f.keys():
-                    tmp_dict.update(f["parameters"].attrs)
-                if "additionals" in f.keys():
-                    tmp_dict.update({"additionals": dict(f["additionals"].attrs)})
-                tmp_dict.update(f.attrs)
-
-            if include_linked_sims:
-                for linked, full_uid in self.sim(uid).links.attrs.items():
-                    sim = Simulation.fromUID(full_uid)
-                    tmp_dict.update(
-                        {f"{linked}.{key}": val for key, val in sim.parameters.items()}
-                    )
+            tmp_dict = self._get_parameters_for_uid(
+                uid, include_linked_sims=include_linked_sims
+            )
             data.append(tmp_dict)
 
         df = pd.DataFrame.from_records(data)
         if df.empty:
             return df
         df["time_stamp"] = pd.to_datetime(df["time_stamp"])
 
@@ -256,41 +340,49 @@
         Returns:
             :class:`pd.DataFrame`
         """
         data = list()
         for uid in self.all_uids:
             h5file_for_uid = os.path.join(self.path, uid, f"{uid}.h5")
             with open_h5file(h5file_for_uid, "r") as file:
-                tmp_dict = dict()
-                tmp_dict = {
-                    key: (
-                        len(file[f"data/{key}"]),
-                        file[f"data/{key}/0"].shape,
-                        file[f"data/{key}/0"].dtype,
-                    )
-                    for key in file["data"].keys()
-                }
+                try:
+                    tmp_dict = dict()
+                    tmp_dict = {
+                        key: (
+                            len(file[f"data/{key}"]),
+                            file[f"data/{key}/0"].shape,
+                            file[f"data/{key}/0"].dtype,
+                        )
+                        for key in file["data"].keys()
+                    }
+                except KeyError:
+                    tmp_dict = dict()
                 data.append(tmp_dict)
         return pd.DataFrame.from_records(data)
 
-    def sim(self, uid, return_writer: bool = False) -> Simulation:
+    def sim(
+        self,
+        uid,
+        return_writer: bool = False,
+        writer_type: SimulationWriter = SimulationWriter,
+    ) -> Simulation:
         """Get an existing simulation with uid. Same as accessing with `db[uid]` directly.
 
         Args:
             uid (`str`): unique identifier
             return_writer: if true, return `SimulationWriter`, otherwise
                 return `Simulation`
+            writer_type: Optionally, you can specify a custom writer type to return.
+
         Returns:
             :class:`~bamboost.simulation.Simulation`
         """
-        if uid not in self.all_uids:
-            raise KeyError("The simulation id is not valid.")
         if return_writer:
-            return SimulationWriter(uid, self.path, self.comm)
-        return Simulation(uid, self.path, self.comm)
+            return writer_type(uid, self.path, self.comm)
+        return Simulation(uid, self.path, self.comm, _db_id=self.UID)
 
     def sims(
         self,
         select: pd.Series = None,
         sort: str = None,
         reverse: bool = False,
         exclude: set = None,
@@ -302,16 +394,20 @@
         Args:
             select (`pd.Series`): pandas boolean series
             sort (`str`): Optionally sort the list with this keyword
             reverse (`bool`): swap sort direction
             exclude (`list[str]`): sims to exclude
             return_writer: if true, return `SimulationWriter`, otherwise
                 return `Simulation`
+
         Returns:
             A list of `:class:~bamboost.simulation.Simulation` objects
+
+        Examples:
+            >>> db.sims(select=db.df["status"] == "finished", sort="time_stamp")
         """
         if select is not None:
             id_list = self.df[select]["id"].values
         else:
             id_list = self.all_uids
         if exclude is not None:
             exclude = list([exclude]) if isinstance(exclude, str) else exclude
@@ -341,16 +437,23 @@
             uid (`str`): The name/uid for the simulation. If not specified, a random id
                 will be assigned.
             parameters (`dict`): Parameter dictionary. If provided, the parameters will be
                 checked against the existing sims for duplication. Otherwise, they may be
                 specified later with :func:`~bamboost.simulation.SimulationWriter.add_parameters`.
             skip_duplicate_check (`bool`): if True, the duplicate check is skipped.
             prefix (`str`): Prefix for the uid. If not specified, no prefix is used.
+
         Returns:
             sim (:class:`~bamboost.simulation.SimulationWriter`)
+
+        Examples:
+            >>> db.create_simulation(parameters={"a": 1, "b": 2})
+            apple
+
+            >>> db.create_simulation(uid="my_sim", parameters={"a": 1, "b": 2}, prefix="test")
         """
         if parameters and not skip_duplicate_check:
             go_on, uid = self._check_duplicate(parameters, uid)
             if not go_on:
                 print("Aborting by user desire...")
                 return None
 
@@ -367,38 +470,29 @@
             path_to_h5_file = os.path.join(self.path, uid, f"{uid}.h5")
             if os.path.exists(path_to_h5_file):
                 os.remove(path_to_h5_file)
             h5py.File(path_to_h5_file, "a").close()  # create file
 
         new_sim = SimulationWriter(uid, self.path, self.comm)
         new_sim.initialize()  # sets metadata and status
-        self.all_uids.append(new_sim.uid)
-        if parameters is None:
-            parameters = dict()
-        new_sim.add_parameters(parameters)
+        # add the id to the (fixed) _all_uids list
+        if hasattr(self, "_all_uids"):
+            self._all_uids.append(new_sim.uid)
+        if parameters:
+            new_sim.add_parameters(parameters)
         return new_sim
 
     def remove(self, uid: str) -> None:
         """CAUTION, DELETING DATA. Remove the data of a simulation.
 
         Args:
             uid (`str`): uid
         """
         shutil.rmtree(os.path.join(self.path, uid))
 
-    def _get_uids(self) -> list:
-        """Get all simulation names in the database."""
-        all_uids = list()
-        for dir in [i for i in os.listdir(self.path) if not i.startswith(".")]:
-            if any(
-                [i.endswith(".h5") for i in os.listdir(os.path.join(self.path, dir))]
-            ):
-                all_uids.append(dir)
-        return all_uids
-
     def _check_duplicate(self, parameters: dict, uid: str) -> tuple:
         """Checking whether the parameters dictionary exists already.
         May need to be improved...
 
         Args:
             parameters (`dict`): parameter dictionary to check for
             uid (`str`): uid
```

### Comparing `bamboost-0.5.1/bamboost/simulation.py` & `bamboost-0.6.0/bamboost/simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import subprocess
 from typing import Any, Iterable, Tuple
 
 import numpy as np
 import pandas as pd
 from typing_extensions import Self, deprecated
 
+from bamboost._config import config
+
 from . import index
 from .accessors.fielddata import DataGroup
 from .accessors.globals import GlobalGroup
 from .accessors.meshes import MeshGroup
 from .common import hdf_pointer, utilities
 from .common.file_handler import FileHandler, with_file_open
 from .common.job import Job
@@ -92,23 +94,29 @@
 
     def __init__(
         self,
         uid: str,
         path: str,
         comm: MPI.Comm = MPI.COMM_WORLD,
         create_if_not_exists: bool = False,
+        *,
+        _db_id: str = None,
     ):
         self.uid: str = uid
+        path = comm.bcast(path, root=0)
         self.path_database: str = os.path.abspath(path)
+        self.database_id = _db_id or index.get_uid_from_path(self.path_database)
         self.path: str = os.path.abspath(os.path.join(path, uid))
         self.h5file: str = os.path.join(self.path, f"{self.uid}.h5")
         self.xdmffile: str = os.path.join(self.path, f"{self.uid}.xdmf")
 
         if not os.path.exists(self.h5file) and not create_if_not_exists:
-            raise FileNotFoundError(f"Simulation {self.uid} does not exist in {self.path}.")
+            raise FileNotFoundError(
+                f"Simulation {self.uid} does not exist in {self.path}."
+            )
 
         os.makedirs(self.path, exist_ok=True)
 
         # MPI information
         self._comm = comm
         self._psize = self._comm.size
         self._prank = self._comm.rank
@@ -129,16 +137,16 @@
     def fromUID(cls, full_uid: str) -> Self:
         """Return the `Simulation` with given UID.
 
         Args:
             full_uid: the full id (Database uid : simulation uid)
         """
         db_uid, sim_uid = full_uid.split(":")
-        db_path = index.get_path(db_uid)
-        return cls(sim_uid, db_path)
+        db_path = index.IndexAPI().get_path(db_uid)
+        return cls(sim_uid, db_path, create_if_not_exists=False)
 
     @with_file_open()
     def __getitem__(self, key) -> hdf_pointer.BasePointer:
         """Direct access to HDF5 file.
 
         Returns:
             :class:`~bamboost.common.file_handler.BasePointer`
@@ -196,19 +204,35 @@
                 ),
             )
             .replace("$SUBMITTED", submitted_options[metadata.get("submitted", False)])
             .replace("$TIMESTAMP", metadata["time_stamp"])
         )
         return html_string
 
+    def _push_update_to_sqlite(self, update_dict: dict) -> None:
+        """Push update to sqlite database.
+
+        Args:
+            - update_dict (dict): key value pair to push
+        """
+        if not config["options"].get("sync_table", True):
+            return
+        try:
+            index.DatabaseTable(self.database_id).update_entry(self.uid, update_dict)
+        except index.Error as e:
+            log.warning(f"Could not update sqlite database: {e}")
+
     @property
     def parameters(self) -> dict:
         tmp_dict = dict()
         if self._prank == 0:
             with self._file("r"):
+                # return if parameters is not in the file
+                if "parameters" not in self._file.keys():
+                    return {}
                 tmp_dict.update(self._file["parameters"].attrs)
                 for key in self._file["parameters"].keys():
                     tmp_dict.update({key: self._file[f"parameters/{key}"][()]})
 
         tmp_dict = utilities.unflatten_dict(tmp_dict)
 
         tmp_dict = self._comm.bcast(tmp_dict, root=0)
@@ -216,14 +240,16 @@
 
     @property
     def metadata(self) -> dict:
         tmp_dict = dict()
         if self._prank == 0:
             with self._file("r") as file:
                 tmp_dict.update(file.attrs)
+
+        tmp_dict = utilities.unflatten_dict(tmp_dict)
         tmp_dict = self._comm.bcast(tmp_dict, root=0)
         return tmp_dict
 
     def files(self, filename: str) -> str:
         """Get the path to the file.
 
         Args:
@@ -252,14 +278,18 @@
     def open_in_file_explorer(self) -> None:
         """Open the simulation directory. Uses `xdg-open` on linux systems."""
         if os.name == "nt":  # should work on Windows
             os.startfile(self.path)
         else:
             subprocess.run(["xdg-open", self.path])
 
+    def open_in_paraview(self) -> None:
+        """Open the xdmf file in paraview."""
+        subprocess.Popen(["paraview", self.xdmffile])
+
     def get_full_uid(self) -> str:
         """Returns the full uid of the simulation (including the one of the database)"""
         database_uid = index.get_uid_from_path(self.path_database)
         return f"{database_uid}:{self.uid}"
 
     def change_status(self, status: str) -> None:
         """Change status of simulation.
@@ -268,72 +298,92 @@
             status (str): new status
         """
         if self._prank == 0:
             self._file.open("a")
             self._file.attrs["status"] = status
             self._file.close()
 
+        self._push_update_to_sqlite({"status": status})
+
     def update_metadata(self, update_dict: dict) -> None:
         """Update the metadata attributes.
 
         Args:
             update_dict: dictionary to push
         """
-        with self._file("a") as file:
-            file.attrs.update(update_dict)
+        if self._prank == 0:
+            update_dict = utilities.flatten_dict(update_dict)
+            with self._file("a") as file:
+                file.attrs.update(update_dict)
+
+            self._push_update_to_sqlite(update_dict)
 
     def update_parameters(self, update_dict: dict) -> None:
         """Update the parameters dictionary.
 
         Args:
             update_dict: dictionary to push
         """
         if self._prank == 0:
+            update_dict = utilities.flatten_dict(update_dict)
             with self._file("a") as file:
-                file["parameters"].attrs.update(utilities.flatten_dict(update_dict))
+                file["parameters"].attrs.update(update_dict)
+
+            self._push_update_to_sqlite(update_dict)
 
     def create_xdmf_file(self, fields: list = None, nb_steps: int = None) -> None:
         """Create the xdmf file to read in paraview.
 
         Args:
             fields (list[str]): fields for which to write timeseries information,
                 if not specified, all fields in data are written.
             nb_steps (int): number of steps the simulation has
         """
 
         if self._prank == 0:
             with self._file("r") as f:
-                if not fields:
+                if "data" not in f.keys():
+                    fields, nb_steps = [], 0
+                if fields is None:
                     fields = list(f["data"].keys())
 
-                if not nb_steps:
+                if nb_steps is None:
                     grp_name = list(f["data"].keys())[0]
                     nb_steps = list(f[f"data/{grp_name}"].keys())
                     nb_steps = max(
                         [int(step) for step in nb_steps if not step.startswith("__")]
                     )
 
+                # temporary fix to load coordinates/geometry
+                coords_name = (
+                    "geometry"
+                    if "geometry"
+                    in f[f"{self._mesh_location}/{self._default_mesh}"].keys()
+                    else "coordinates"
+                )
+
             xdmf_writer = XDMFWriter(self.xdmffile, self.h5file)
             xdmf_writer.write_points_cells(
-                f"{self._mesh_location}/{self._default_mesh}/geometry",
+                f"{self._mesh_location}/{self._default_mesh}/{coords_name}",
                 f"{self._mesh_location}/{self._default_mesh}/topology",
             )
 
-            xdmf_writer.add_timeseries(nb_steps + 1, fields)
+            if fields:
+                xdmf_writer.add_timeseries(nb_steps + 1, fields)
             xdmf_writer.write_file()
 
     def create_batch_script(
         self,
         commands: list = None,
         nnodes=1,
         ntasks=4,
         ncpus=1,
         time="04:00:00",
         mem_per_cpu=2048,
-        tmp=8000,
+        tmp=None,
         euler=True,
     ) -> None:
         """Create a batch job and put it into the folder.
 
         Args:
             commands: A list of strings being the user defined commands to run
             nnodes: nb of nodes (default=1)
@@ -360,14 +410,15 @@
                 )
 
         if euler:
             job.create_sbatch_script(
                 commands,
                 path=os.path.abspath(self.path_database),
                 uid=self.uid,
+                db_id=self.database_id,
                 nnodes=nnodes,
                 ntasks=ntasks,
                 ncpus=ncpus,
                 time=time,
                 mem_per_cpu=mem_per_cpu,
                 tmp=tmp,
             )
@@ -383,27 +434,40 @@
 
     def submit(self) -> None:
         """Submit the job for this simulation."""
         if f"sbatch_{self.uid}.sh" in os.listdir(self.path):
             batch_script = os.path.abspath(
                 os.path.join(self.path, f"sbatch_{self.uid}.sh")
             )
-            subprocess.Popen(["sbatch", f"{batch_script}"])
-        if f"{self.uid}.sh" in os.listdir(self.path):
+            env = os.environ.copy()
+            _ = env.pop("BAMBOOST_MPI", None)
+            subprocess.run(["sbatch", f"{batch_script}"], env=env)
+        elif f"{self.uid}.sh" in os.listdir(self.path):
             bash_script = os.path.abspath(os.path.join(self.path, f"{self.uid}.sh"))
-            subprocess.Popen(["bash", f"{bash_script}"])
+            env = os.environ.copy()
+            _ = env.pop("BAMBOOST_MPI", None)
+            subprocess.run(["bash", f"{bash_script}"], env=env)
+        else:
+            raise FileNotFoundError(
+                f"Could not find a batch script for simulation {self.uid}."
+            )
+        
 
-        print(f"Simulation {self.uid} submitted!")
+        log.info(f"Simulation {self.uid} submitted!")
 
         with self._file("a") as file:
             file.attrs.update({"submitted": True})
 
+        self._push_update_to_sqlite({"submitted": True})
+
     @with_file_open("a")
     def change_note(self, note) -> None:
-        self._file.attrs["notes"] = note
+        if self._prank == 0:
+            self._file.attrs["notes"] = note
+            self._push_update_to_sqlite({"notes": note})
 
     # Ex-Simulation reader methods
     # ----------------------------
 
     def open(self, mode: str = "r", driver=None, comm=None) -> FileHandler:
         """Use this as a context manager in a `with` statement.
         Purpose: keeping the file open to directly access/edit something in the
@@ -433,14 +497,20 @@
             mesh_name (`str`): optional, name of mesh to read (default = mesh)
         Returns:
             Tuple of np.arrays (coordinates, connectivity)
         """
         if mesh_name is None:
             mesh_name = self._default_mesh
 
+        # Raise an error if the mesh is not found
+        if (self._mesh_location.split("/")[0] not in self._file.keys()) or (
+            mesh_name not in self._file[self._mesh_location].keys()
+        ):
+            raise KeyError(f"Mesh location {self._mesh_location} not found in file.")
+
         mesh = self.meshes[mesh_name]
         return mesh.coordinates, mesh.connectivity
 
     @property
     @deprecated("Use `data.info` instead")
     @with_file_open("r")
     def data_info(self) -> pd.DataFrame:
```

### Comparing `bamboost-0.5.1/bamboost/simulation_writer.py` & `bamboost-0.6.0/bamboost/simulation_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,20 +73,22 @@
         return self
 
     def add_metadata(self) -> None:
         """Add metadata to h5 file."""
         nb_proc = self._comm.Get_size()
         if self._prank == 0:
             with self._file("a"):
-                self._file.attrs["time_stamp"] = str(
-                    datetime.datetime.now().replace(microsecond=0)
-                )
-                self._file.attrs["id"] = self.uid
-                self._file.attrs["processors"] = nb_proc
-                self._file.attrs["notes"] = self._file.attrs.get("notes", "")
+                data = {
+                    "time_stamp": str(datetime.datetime.now().replace(microsecond=0)),
+                    "id": self.uid,
+                    "processors": nb_proc,
+                    "notes": self._file.attrs.get("notes", ""),
+                }
+                self._file.attrs.update(data)
+            self._push_update_to_sqlite(data)
 
     def add_parameters(self, parameters: dict) -> None:
         """Add parameters to simulation.
 
         Args:
             parameters: Dictionary with parameters.
         """
@@ -99,16 +101,15 @@
                     del self._file["parameters"]
                 grp = self._file.create_group("/parameters")
                 for key, val in parameters.items():
                     if isinstance(val, np.ndarray):
                         grp.create_dataset(key, data=val)
                     elif val is not None:
                         grp.attrs[key] = val
-                    else:
-                        pass
+            self._push_update_to_sqlite(parameters)
 
     def add_mesh(
         self, coordinates: np.ndarray, connectivity: np.ndarray, mesh_name: str = None
     ) -> None:
         """Add the mesh to file. Currently only 2d meshes.
 
         Args:
@@ -146,16 +147,16 @@
         idx_end_cells = idx_start_cells + nb_cells_local
         connectivity = connectivity + idx_start
 
         with self._file("a", driver="mpio", comm=self._comm) as f:
             if mesh_location in self._file.file_object:
                 del self._file.file_object[mesh_location]
             grp = f.require_group(mesh_location)
-            coord = grp.require_dataset("geometry", shape=coord_shape, dtype="f")
-            conn = grp.require_dataset("topology", shape=conn_shape, dtype="i")
+            coord = grp.require_dataset("geometry", shape=coord_shape, dtype=coordinates.dtype)
+            conn = grp.require_dataset("topology", shape=conn_shape, dtype=connectivity.dtype)
 
             coord[idx_start:idx_end] = coordinates
             conn[idx_start_cells:idx_end_cells] = connectivity
 
     def add_field(
         self,
         name: str,
@@ -173,42 +174,40 @@
             mesh: Optional. Linked mesh for this data
             dtype: Optional. Numpy style datatype, see h5py documentation,
                 defaults to the dtype of the vector.
         """
         if mesh is None:
             mesh = self._default_mesh
 
-        # Get dimension of vector
-        if vector.ndim <= 1:
-            vector = vector.reshape((-1, 1))
-        dim = vector.shape[1]
+        dim = vector.shape[1:] if vector.ndim > 1 else None
 
         if time is None:
             time = self.step
 
         length_local = vector.shape[0]
         length_p = np.array(self._comm.allgather(length_local))
+
         length = np.sum(length_p)
 
         # global indices
         idx_start = np.sum(length_p[self._ranks < self._prank])
         idx_end = idx_start + length_local
 
         # open file
         with self._file("a", driver="mpio", comm=self._comm) as f:
             data = f.require_group(
                 "data"
             )  # Require group data to store all point data in
             grp = data.require_group(name)
             vec = grp.require_dataset(
                 str(self.step),
-                shape=(length, dim),
+                shape=(length, *dim) if dim else (length,),
                 dtype=dtype if dtype else vector.dtype,
             )
-            vec[idx_start:idx_end, :] = vector
+            vec[idx_start:idx_end] = vector
 
         if self._prank == 0:
             with self._file("a"):
                 vec = self._file["data"][name][str(self.step)]
                 vec.attrs["t"] = time  # add time as attribute to dataset
                 vec.attrs["mesh"] = mesh  # add link to mesh as attribute
 
@@ -224,20 +223,21 @@
         """
         if self._prank == 0:
             with self._file("a") as f:
                 grp = f.require_group("globals")
                 if name not in grp.keys():
                     vec = grp.create_dataset(
                         name,
-                        shape=(1,),
+                        shape=(self.step + 1,),
                         dtype=dtype if dtype else np.array(value).dtype,
                         chunks=True,
                         maxshape=(None,),
+                        fillvalue=np.nan,
                     )
-                    vec[0] = value
+                    vec[-1] = value
                 else:
                     vec = grp[name]
                     vec.resize((self.step + 1,))
                     vec[-1] = value
 
     @deprecated("Use `copy_file` instead.")
     def add_additional(self, name: str, file: str) -> None:
```

### Comparing `bamboost-0.5.1/bamboost/xdmf.py` & `bamboost-0.6.0/bamboost/xdmf.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 # There is no warranty for this code
 
 import os
 import xml.etree.ElementTree as ET
 
 import h5py
+import numpy as np
 
 __all__ = ["XDMFWriter"]
 
 # `numpy_to_xdmf_dtype` from `meshio.xdmf.common`
 numpy_to_xdmf_dtype = {
     "int8": ("Int", "1"),
     "int16": ("Int", "2"),
@@ -154,33 +155,38 @@
 
     def write_attribute(
         self, grid: ET.Element, field_name: str, name: str, step: int
     ) -> None:
         """Write an attribute/field."""
         with h5py.File(self.h5file, "r") as f:
             data = f[f"data/{field_name}/{step}"]
-            try:
-                shape = data.shape[1]
-            except IndexError:
-                shape = 1
-            att_type = {1: "Scalar", 2: "Vector", 3: "Tensor"}.get(shape, "Scalar")
+            
+            if data.ndim == 1 or data.shape[1] <= 1:
+                att_type = "Scalar"
+            elif data.ndim == 2:
+                att_type = "Vector"
+            elif data.ndim == 3 and len(set(data.shape[1:])) == 1:
+                # Square shape -> Tensor
+                att_type = "Tensor"
+            else:
+                att_type = "Matrix"
+
+            # Cell or Node data
+            center = data.attrs.get("center", "Node")
 
             att = ET.SubElement(
                 grid,
                 "Attribute",
                 Name=name,
                 AttributeType=att_type,
-                Center="Node",
+                Center=center,
             )
 
             dt, prec = numpy_to_xdmf_dtype[data.dtype.name]
-            try:
-                dim = "{} {}".format(*data.shape)
-            except IndexError:
-                dim = "{}".format(data.shape[0])
+            dim = " ".join([str(i) for i in data.shape])
 
             data_item = ET.SubElement(
                 att,
                 "DataItem",
                 DataType=dt,
                 Dimensions=dim,
                 Format="HDF",
```

### Comparing `bamboost-0.5.1/bamboost.egg-info/PKG-INFO` & `bamboost-0.6.0/bamboost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamboost
-Version: 0.5.1
+Version: 0.6.0
 Summary: A light weight database manager using HDF5
 Author-email: Flavio Lorez <florez@ethz.ch>
 License: Copyright (c) 2023 CMBM, ETH Zurich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bamboost Version: 0.5.1 Summary: A light weight
+Metadata-Version: 2.1 Name: bamboost Version: 0.6.0 Summary: A light weight
 database manager using HDF5 Author-email: Flavio Lorez
 ethz.ch> License: Copyright (c) 2023 CMBM, ETH Zurich Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `bamboost-0.5.1/bamboost.egg-info/SOURCES.txt` & `bamboost-0.6.0/bamboost.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 bamboost/__init__.py
+bamboost/_config.py
+bamboost/_sqlite_database.py
 bamboost/index.py
 bamboost/manager.py
 bamboost/simulation.py
 bamboost/simulation_writer.py
 bamboost/xdmf.py
 bamboost.egg-info/PKG-INFO
 bamboost.egg-info/SOURCES.txt
 bamboost.egg-info/dependency_links.txt
+bamboost.egg-info/entry_points.txt
 bamboost.egg-info/requires.txt
 bamboost.egg-info/top_level.txt
 bamboost/accessors/__init__.py
 bamboost/accessors/fielddata.py
 bamboost/accessors/globals.py
 bamboost/accessors/meshes.py
 bamboost/common/__init__.py
 bamboost/common/_mock_mpi.py
 bamboost/common/file_handler.py
 bamboost/common/git_utility.py
 bamboost/common/hdf_pointer.py
 bamboost/common/job.py
 bamboost/common/mpi.py
 bamboost/common/utilities.py
+bamboost/extensions/__init__.py
+bamboost/extensions/fenics.py
+bamboost/extensions/remote_manager.py
+bamboost/extensions/slurm.py
 bamboost/html/hdf5_group.html
 bamboost/html/icon.png
 bamboost/html/icon.txt
 bamboost/html/manager.html
 bamboost/html/simulation.html
+cli/__init__.py
+cli/main.py
+tests/test_index.py
 tests/test_manager.py
 tests/test_reader.py
 tests/test_writer.py
```

### Comparing `bamboost-0.5.1/pyproject.toml` & `bamboost-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bamboost"
-version = "0.5.1"
+version = "0.6.0"
 description = "A light weight database manager using HDF5"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [{ name = "Flavio Lorez", email = "florez@ethz.ch" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -27,14 +27,17 @@
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 mpi = [
     "mpi4py",
 ]
 
+[project.entry-points.console_scripts]
+bamboostcli = "cli:main"
+
 [project.urls]
 Homepage = "https://bamboost.ch/"
 repository = "https://gitlab.com/cmbm-ethz/bamboost"
 changelog = "https://gitlab.com/cmbm-ethz/bamboost/-/tree/main/CHANGELOG.md"
 
 [tool.setuptools.packages.find]
-include = ["bamboost", "bamboost*"]
+include = ["bamboost", "bamboost*", "cli", "cli*"]
```

### Comparing `bamboost-0.5.1/tests/test_writer.py` & `bamboost-0.6.0/tests/test_writer.py`

 * *Files identical despite different names*

