# Comparing `tmp/f4-0.9.8.tar.gz` & `tmp/f4-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.9.8.tar", last modified: Wed Apr 24 17:38:37 2024, max compression
+gzip compressed data, was "f4-0.9.9.tar", last modified: Fri Apr 26 01:20:07 2024, max compression
```

## Comparing `f4-0.9.8.tar` & `f4-0.9.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-24 17:38:37.589040 f4-0.9.8/
--rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.8/LICENSE
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-24 17:38:37.588983 f4-0.9.8/PKG-INFO
--rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.8/README.md
--rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.8/pyproject.toml
--rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-24 17:38:37.589328 f4-0.9.8/setup.cfg
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-24 17:38:37.584456 f4-0.9.8/src/
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-24 17:38:37.587180 f4-0.9.8/src/f4/
--rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.8/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.8/src/f4/Parser.py
--rw-r--r--   0 srp33      (503) staff       (20)    16352 2024-04-24 16:31:08.000000 f4-0.9.8/src/f4/Transformer.py
--rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-24 16:31:08.000000 f4-0.9.8/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.8/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-24 17:38:37.588780 f4-0.9.8/src/f4.egg-info/
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-24 17:38:37.000000 f4-0.9.8/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-24 17:38:37.000000 f4-0.9.8/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-24 17:38:37.000000 f4-0.9.8/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-24 17:38:37.000000 f4-0.9.8/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-24 17:38:37.000000 f4-0.9.8/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-24 17:38:37.588061 f4-0.9.8/test/
--rwxr-xr-x   0 srp33      (503) staff       (20)    55960 2024-04-24 17:35:51.000000 f4-0.9.8/test/test.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-26 01:20:07.164749 f4-0.9.9/
+-rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.9/LICENSE
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-26 01:20:07.164693 f4-0.9.9/PKG-INFO
+-rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.9/README.md
+-rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.9/pyproject.toml
+-rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-26 01:20:07.165035 f4-0.9.9/setup.cfg
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-26 01:20:07.159551 f4-0.9.9/src/
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-26 01:20:07.162904 f4-0.9.9/src/f4/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.9/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)    64912 2024-04-25 15:35:56.000000 f4-0.9.9/src/f4/Parser.py
+-rw-r--r--   0 srp33      (503) staff       (20)    16960 2024-04-25 15:36:31.000000 f4-0.9.9/src/f4/Transformer.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)     8669 2024-04-25 22:14:11.000000 f4-0.9.9/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.9/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-26 01:20:07.164482 f4-0.9.9/src/f4.egg-info/
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-26 01:20:07.000000 f4-0.9.9/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-26 01:20:07.000000 f4-0.9.9/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-26 01:20:07.000000 f4-0.9.9/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-26 01:20:07.000000 f4-0.9.9/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-26 01:20:07.000000 f4-0.9.9/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-26 01:20:07.163834 f4-0.9.9/test/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    61472 2024-04-25 20:24:33.000000 f4-0.9.9/test/test.py
```

### Comparing `f4-0.9.8/LICENSE` & `f4-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.9.8/PKG-INFO` & `f4-0.9.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.8/setup.cfg` & `f4-0.9.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.9.8
+version = 0.9.9
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.9.8/src/f4/Builder.py` & `f4-0.9.9/src/f4/Builder.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.8/src/f4/Parser.py` & `f4-0.9.9/src/f4/Parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from .Utilities import *
 
 #####################################################
 # Classes
 #####################################################
 
 class FileData:
-    def __init__(self, data_file_path, file_handle, file_map_dict, cache_dict, version, decompression_type, decompressor):
+    def __init__(self, data_file_path, file_handle, use_memory_mapping, file_map_dict, cache_dict, version, decompression_type, decompressor):
         self.data_file_path = data_file_path
         self.file_handle = file_handle
+        self.use_memory_mapping = use_memory_mapping
         self.file_map_dict = file_map_dict
         self.cache_dict = cache_dict
         self.version = version
         self.decompression_type = decompression_type
         self.decompressor = decompressor
 
 """
@@ -57,23 +58,23 @@
             if row_indices is None:
                 num_rows = file_data.cache_dict["num_rows"]
 
                 if num_rows <= 100 or num_parallel == 1:
                     return self._do_row_indices_pass(file_data, coords, parse_function, range(num_rows))
                 else:
                     return set(chain.from_iterable(joblib.Parallel(n_jobs=num_parallel)(
-                        joblib.delayed(self._do_row_indices_pass_parallel)(file_data.data_file_path, coords, parse_function, chunk_row_indices)
+                        joblib.delayed(self._do_row_indices_pass_parallel)(file_data.data_file_path, file_data.use_memory_mapping, coords, parse_function, chunk_row_indices)
                         for chunk_row_indices in generate_range_chunks(num_rows, 1000001)))
                     )
             else:
                 if len(row_indices) <= 100 or num_parallel == 1:
                     return self._do_row_indices_pass(file_data, coords, parse_function, row_indices)
                 else:
                     return set(chain.from_iterable(joblib.Parallel(n_jobs=num_parallel)(
-                        joblib.delayed(self._do_row_indices_pass_parallel)(file_data.data_file_path, coords, parse_function, chunk_row_indices)
+                        joblib.delayed(self._do_row_indices_pass_parallel)(file_data.data_file_path, file_data.use_memory_mapping, coords, parse_function, chunk_row_indices)
                         for chunk_row_indices in split_list_into_chunks(list(row_indices), 1000001)))
                     )
         else:
             matching_row_indices = self.get_matching_row_indices_indexed(file_data, index_number, 0, 1, 0, file_data.cache_dict["num_rows"], True, num_parallel)
 
             if row_indices is None:
                 return matching_row_indices
@@ -94,18 +95,18 @@
 
         for i in row_indices_to_check:
             if self._passes(parse_function(file_data, "", i, coords)):
                 passing_row_indices.add(i)
 
         return passing_row_indices
 
-    def _do_row_indices_pass_parallel(self, data_file_path, coords, parse_function, row_indices_to_check):
+    def _do_row_indices_pass_parallel(self, data_file_path, use_memory_mapping, coords, parse_function, row_indices_to_check):
         passing_row_indices = set()
 
-        with initialize(data_file_path) as file_data:
+        with initialize(data_file_path, use_memory_mapping) as file_data:
             for i in row_indices_to_check:
                 if self._passes(parse_function(file_data, "", i, coords)):
                     passing_row_indices.add(i)
 
         return passing_row_indices
 
     def _get_conversion_function(self):
@@ -445,15 +446,15 @@
 
         return -1
 
 #####################################################
 # Public function(s)
 #####################################################
 
-def query(data_file_path, fltr=NoFilter(), select_columns=[], out_file_path=None, out_file_type="tsv", num_parallel=1, tmp_dir_path=None):
+def query(data_file_path, fltr=NoFilter(), select_columns=[], out_file_path=None, out_file_type="tsv", num_parallel=1, tmp_dir_path=None, use_memory_mapping=True):
     """
     Query the data file using zero or more filters.
 
     This function accepts filtering criteria, identifies matching rows,
     and writes the output (for select columns) to an output file or standard output.
 
     Args:
@@ -475,15 +476,15 @@
     if out_file_type != "tsv":
         raise Exception("The only out_file_type currently supported is tsv.")
 
     if num_parallel > 1:
         global joblib
         joblib = __import__('joblib', globals(), locals())
 
-    with initialize(data_file_path) as file_data:
+    with initialize(data_file_path, use_memory_mapping) as file_data:
         # Make sure the filters match the column types.
         fltr._check_types(file_data)
 
         # Filter rows based on the data
         keep_row_indices = fltr.get_matching_row_indices(file_data, None, num_parallel)
 
         if keep_row_indices is None:
@@ -516,15 +517,16 @@
             # Save header line
             chunk_size = 1000001
             cn_start = file_data.file_map_dict["cn"][0]
             cn_end = file_data.file_map_dict["cn"][1]
 
             with get_write_object(out_file_path) as write_obj:
                 for chunk_start in range(cn_start, cn_end, chunk_size):
-                    chunk_text = file_data.file_handle[chunk_start:min(chunk_start + chunk_size, cn_end)]
+                    # chunk_text = file_data.file_handle[chunk_start:min(chunk_start + chunk_size, cn_end)]
+                    chunk_text = read_from_file(file_data.file_handle, chunk_start, min(chunk_start + chunk_size, cn_end), use_memory_mapping)
                     write_obj.write(chunk_text.replace(b"\n", b"\t"))
 
                 write_obj.write(b"\n")
 
             # Get select column indices
             max_columns_per_chunk = 1000001
             num_cols = file_data.cache_dict["num_cols"]
@@ -540,30 +542,30 @@
 
         if num_row_index_chunks == 1:
             keep_row_indices = [keep_row_indices]
         else:
             keep_row_indices = list(split_list_into_chunks(keep_row_indices, max_rows_per_chunk))
 
         if num_select_column_chunks == 1 and num_row_index_chunks == 1:
-            save_output_rows(data_file_path, out_file_path, keep_row_indices[0], select_column_index_chunks[0])
+            save_output_rows(data_file_path, use_memory_mapping, out_file_path, keep_row_indices[0], select_column_index_chunks[0])
         else:
             if tmp_dir_path:
                 makedirs(tmp_dir_path, exist_ok=True)
             else:
                 tmp_dir_path = mkdtemp()
 
             tmp_dir_path = fix_dir_path_ending(tmp_dir_path)
 
             if num_parallel == 1:
                 for row_chunk_number, row_chunk_indices in enumerate(keep_row_indices):
                     for column_chunk_number, column_chunk_indices in enumerate(select_column_index_chunks):
-                        save_output_rows(data_file_path, f"{tmp_dir_path}{row_chunk_number}_{column_chunk_number}", row_chunk_indices, column_chunk_indices)
+                        save_output_rows(data_file_path, use_memory_mapping, f"{tmp_dir_path}{row_chunk_number}_{column_chunk_number}", row_chunk_indices, column_chunk_indices)
             else:
                 joblib.Parallel(n_jobs=num_parallel)(
-                    joblib.delayed(save_output_rows)(data_file_path, f"{tmp_dir_path}{row_chunk_number}_{column_chunk_number}", row_chunk_indices, column_chunk_indices)
+                    joblib.delayed(save_output_rows)(data_file_path, use_memory_mapping, f"{tmp_dir_path}{row_chunk_number}_{column_chunk_number}", row_chunk_indices, column_chunk_indices)
                         for row_chunk_number, row_chunk_indices in enumerate(keep_row_indices)
                             for column_chunk_number, column_chunk_indices in enumerate(select_column_index_chunks)
                 )
 
             with get_write_object(out_file_path, "ab") as write_obj:
                 for row_chunk_number, row_indices in enumerate(keep_row_indices):
                     chunk_file_dict = {}
@@ -598,38 +600,38 @@
 def tail(data_file_path, n=10, select_columns=None, out_file_path=None, out_file_type="tsv"):
     if not select_columns:
         select_columns = []
 
     query(data_file_path, TailFilter(n), select_columns, out_file_path=out_file_path, out_file_type=out_file_type)
 
 def get_version(data_file_path):
-    with initialize(data_file_path) as file_data:
+    with initialize(data_file_path, use_memory_mapping=True) as file_data:
         return file_data.version.decode()
 
-def get_num_rows(data_file_path):
-    with initialize(data_file_path) as file_data:
+def get_num_rows(data_file_path, use_memory_mapping=True):
+    with initialize(data_file_path, use_memory_mapping) as file_data:
         return file_data.cache_dict["num_rows"]
 
-def get_num_cols(data_file_path):
-    with initialize(data_file_path) as file_data:
+def get_num_cols(data_file_path, use_memory_mapping=True):
+    with initialize(data_file_path, use_memory_mapping) as file_data:
         return file_data.cache_dict["num_cols"]
 
-def get_column_type_from_name(data_file_path, column_name):
+def get_column_type_from_name(data_file_path, column_name, use_memory_mapping=True):
     try:
-        with initialize(data_file_path) as file_data:
+        with initialize(data_file_path, use_memory_mapping) as file_data:
             column_index = get_column_index_from_name(file_data, column_name.encode())
 
             return get_column_type_from_index(file_data, column_index)
     except:
         raise Exception(f"A column with the name {column_name} does not exist.")
 
-def get_indexes(data_file_path):
+def get_indexes(data_file_path, use_memory_mapping=True):
     indexes = []
 
-    with initialize(data_file_path) as file_data:
+    with initialize(data_file_path, use_memory_mapping) as file_data:
         if "i" in file_data.cache_dict:
             for key, number in file_data.cache_dict["i"].items():
                 if len(key) == 1:
                     column_name = key[0][0]
                     reverse_status = key[0][1]
 
                     if reverse_status:
@@ -655,73 +657,153 @@
     return indexes
 
 ##############################################
 # Non-public functions
 ##############################################
 
 @contextmanager
-def initialize(data_file_path):
-    with open(data_file_path, 'rb') as file_handle:
-        with mmap(file_handle.fileno(), 0, prot=PROT_READ) as mmap_handle:
-            file_map_length_string = mmap_handle.readline()
-            file_map_length = fast_int(file_map_length_string.rstrip(b"\n"))
-            file_map_dict = deserialize(mmap_handle[len(file_map_length_string):(len(file_map_length_string) + file_map_length)])
-
-            cache_dict = {}
-            cache_dict["ccml"] = fast_int(mmap_handle[file_map_dict["ccml"][0]:file_map_dict["ccml"][1]])
-            cache_dict["num_cols"] = fast_int((file_map_dict["cc"][1] - file_map_dict["cc"][0]) / cache_dict["ccml"]) - 1
-
-            decompression_type = None
-            decompressor = None
-
-            if "cmpr" in file_map_dict:
-                decompression_text = mmap_handle[file_map_dict["cmpr"][0]:file_map_dict["cmpr"][1]]
-
-                if decompression_text == b"z":
-                    decompression_type = "zstd"
-                    decompressor = ZstdDecompressor()
-
-                    # TODO: For super tall files, this gets too large to fit in memory.
-                    #       If we continue to support zstd compression, you may need to incorporate
-                    #       the idea of row chunks when building the file and then retrieve
-                    #       the row_starts just for those.
-                    #       However, the custom compression approach would avoid this problem.
-                    # row_lengths = deserialize(mmap_handle[file_map_dict["rl"][0]:file_map_dict["rl"][1]])
-                    # cache_dict["row_starts"] = [file_map_dict[""][0]]
-                    # for i, row_length in enumerate(row_lengths):
-                    #     cache_dict["row_starts"].append(cache_dict["row_starts"][-1] + row_length)
-                    cache_dict["mrel"] = fast_int(mmap_handle[file_map_dict["mrel"][0]:file_map_dict["mrel"][1]])
-
-                    cache_dict["ll"] = fast_int(mmap_handle[file_map_dict["ll"][0]:file_map_dict["ll"][1]])
-                    cache_dict["num_rows"] = fast_int(mmap_handle[file_map_dict["nrow"][0]:file_map_dict["nrow"][1]])
-                # else:
-                #     decompression_type = "dictionary"
-                #     decompressor = deserialize(decompression_text)
-            else:
-                last_cc = file_map_dict["cc"][1]
-                cache_dict["ll"] = fast_int(mmap_handle[(last_cc - cache_dict["ccml"]):last_cc])
-                cache_dict["num_rows"] = fast_int((file_map_dict[""][1] - file_map_dict[""][0]) / cache_dict["ll"])
-
-            # Calculate line length based on last "cnicc" value.
-            cache_dict["cniccml"] = fast_int(mmap_handle[file_map_dict["cniccml"][0]:file_map_dict["cniccml"][1]])
-            cache_dict["cnill"] = fast_int(mmap_handle[(file_map_dict["cnicc"][1] - cache_dict["cniccml"]):file_map_dict["cnicc"][1]])
-
-            if "i" in file_map_dict:
-                cache_dict["i"] = deserialize(mmap_handle[file_map_dict["i"][0]:file_map_dict["i"][1]])
-
-                for key in file_map_dict:
-                    if key.endswith("ccml"):
-                        cache_dict[key] = fast_int(mmap_handle[file_map_dict[key][0]:file_map_dict[key][1]])
-
-                        last_cc = file_map_dict[key[:-2]][1]
-                        cache_dict[key.replace("ccml", "ll")] = fast_int(mmap_handle[(last_cc - cache_dict[key]):last_cc])
-
-            ver = mmap_handle[file_map_dict["ver"][0]:file_map_dict["ver"][1]]
+def initialize(data_file_path, use_memory_mapping):
+    with get_file_handle(data_file_path, use_memory_mapping) as file_handle:
+        file_map_length_string = file_handle.readline()
+        file_map_length = fast_int(file_map_length_string.rstrip(b"\n"))
+        # file_map_dict = deserialize(mmap_handle[len(file_map_length_string):(len(file_map_length_string) + file_map_length)])
+        file_map_dict = deserialize(read_from_file(file_handle, len(file_map_length_string), len(file_map_length_string) + file_map_length, use_memory_mapping))
+
+        cache_dict = {}
+        # cache_dict["ccml"] = fast_int(mmap_handle[file_map_dict["ccml"][0]:file_map_dict["ccml"][1]])
+        cache_dict["ccml"] = fast_int(read_from_file(file_handle, file_map_dict["ccml"][0], file_map_dict["ccml"][1], use_memory_mapping))
+        cache_dict["num_cols"] = fast_int((file_map_dict["cc"][1] - file_map_dict["cc"][0]) / cache_dict["ccml"]) - 1
+
+        decompression_type = None
+        decompressor = None
+
+        if "cmpr" in file_map_dict:
+            # decompression_text = mmap_handle[file_map_dict["cmpr"][0]:file_map_dict["cmpr"][1]]
+            decompression_text = read_from_file(file_handle, file_map_dict["cmpr"][0], file_map_dict["cmpr"][1], use_memory_mapping)
+
+            if decompression_text == b"z":
+                decompression_type = "zstd"
+                decompressor = ZstdDecompressor()
+
+                # TODO: For super tall files, this gets too large to fit in memory.
+                #       If we continue to support zstd compression, you may need to incorporate
+                #       the idea of row chunks when building the file and then retrieve
+                #       the row_starts just for those.
+                #       However, the custom compression approach would avoid this problem.
+                # row_lengths = deserialize(mmap_handle[file_map_dict["rl"][0]:file_map_dict["rl"][1]])
+                # cache_dict["row_starts"] = [file_map_dict[""][0]]
+                # for i, row_length in enumerate(row_lengths):
+                #     cache_dict["row_starts"].append(cache_dict["row_starts"][-1] + row_length)
+                # cache_dict["mrel"] = fast_int(mmap_handle[file_map_dict["mrel"][0]:file_map_dict["mrel"][1]])
+                cache_dict["mrel"] = fast_int(read_from_file(file_handle, file_map_dict["mrel"][0], file_map_dict["mrel"][1], use_memory_mapping))
+
+                # cache_dict["ll"] = fast_int(mmap_handle[file_map_dict["ll"][0]:file_map_dict["ll"][1]])
+                cache_dict["ll"] = fast_int(read_from_file(file_handle, file_map_dict["ll"][0], file_map_dict["ll"][1], use_memory_mapping))
+
+                # cache_dict["num_rows"] = fast_int(mmap_handle[file_map_dict["nrow"][0]:file_map_dict["nrow"][1]])
+                cache_dict["num_rows"] = fast_int(read_from_file(file_handle, file_map_dict["nrow"][0], file_map_dict["nrow"][1], use_memory_mapping))
+            # else:
+            #     decompression_type = "dictionary"
+            #     decompressor = deserialize(decompression_text)
+        else:
+            last_cc = file_map_dict["cc"][1]
+            # cache_dict["ll"] = fast_int(mmap_handle[(last_cc - cache_dict["ccml"]):last_cc])
+            cache_dict["ll"] = fast_int(read_from_file(file_handle, (last_cc - cache_dict["ccml"]), last_cc, use_memory_mapping))
+            cache_dict["num_rows"] = fast_int((file_map_dict[""][1] - file_map_dict[""][0]) / cache_dict["ll"])
+
+        # Calculate line length based on last "cnicc" value.
+        cache_dict["cniccml"] = fast_int(read_from_file(file_handle, file_map_dict["cniccml"][0], file_map_dict["cniccml"][1], use_memory_mapping))
+        cache_dict["cnill"] = fast_int(read_from_file(file_handle, (file_map_dict["cnicc"][1] - cache_dict["cniccml"]), file_map_dict["cnicc"][1], use_memory_mapping))
+
+        if "i" in file_map_dict:
+            # cache_dict["i"] = deserialize(mmap_handle[file_map_dict["i"][0]:file_map_dict["i"][1]])
+            cache_dict["i"] = deserialize(read_from_file(file_handle, file_map_dict["i"][0], file_map_dict["i"][1], use_memory_mapping))
+
+            for key in file_map_dict:
+                if key.endswith("ccml"):
+                    # cache_dict[key] = fast_int(mmap_handle[file_map_dict[key][0]:file_map_dict[key][1]])
+                    cache_dict[key] = fast_int(read_from_file(file_handle, file_map_dict[key][0], file_map_dict[key][1], use_memory_mapping))
+
+                    last_cc = file_map_dict[key[:-2]][1]
+                    # cache_dict[key.replace("ccml", "ll")] = fast_int(mmap_handle[(last_cc - cache_dict[key]):last_cc])
+                    cache_dict[key.replace("ccml", "ll")] = fast_int(read_from_file(file_handle, (last_cc - cache_dict[key]), last_cc, use_memory_mapping))
+
+        # ver = mmap_handle[file_map_dict["ver"][0]:file_map_dict["ver"][1]]
+        ver = read_from_file(file_handle, file_map_dict["ver"][0], file_map_dict["ver"][1], use_memory_mapping)
+
+        yield FileData(data_file_path, file_handle, use_memory_mapping, file_map_dict, cache_dict, ver, decompression_type, decompressor)
+
+# def initialize(data_file_path, use_memory_mapping=True):
+#     with get_file_handle(data_file_path, use_memory_mapping) as file_handle:
+#         file_map_length_string = file_handle.readline()
+#         file_map_length = fast_int(file_map_length_string.rstrip(b"\n"))
+#         file_map_dict = deserialize(mmap_handle[len(file_map_length_string):(len(file_map_length_string) + file_map_length)])
+#
+#         cache_dict = {}
+#         cache_dict["ccml"] = fast_int(mmap_handle[file_map_dict["ccml"][0]:file_map_dict["ccml"][1]])
+#         cache_dict["num_cols"] = fast_int((file_map_dict["cc"][1] - file_map_dict["cc"][0]) / cache_dict["ccml"]) - 1
+#
+#         decompression_type = None
+#         decompressor = None
+#
+#         if "cmpr" in file_map_dict:
+#             decompression_text = mmap_handle[file_map_dict["cmpr"][0]:file_map_dict["cmpr"][1]]
+#
+#             if decompression_text == b"z":
+#                 decompression_type = "zstd"
+#                 decompressor = ZstdDecompressor()
+#
+#                 # TODO: For super tall files, this gets too large to fit in memory.
+#                 #       If we continue to support zstd compression, you may need to incorporate
+#                 #       the idea of row chunks when building the file and then retrieve
+#                 #       the row_starts just for those.
+#                 #       However, the custom compression approach would avoid this problem.
+#                 # row_lengths = deserialize(mmap_handle[file_map_dict["rl"][0]:file_map_dict["rl"][1]])
+#                 # cache_dict["row_starts"] = [file_map_dict[""][0]]
+#                 # for i, row_length in enumerate(row_lengths):
+#                 #     cache_dict["row_starts"].append(cache_dict["row_starts"][-1] + row_length)
+#                 cache_dict["mrel"] = fast_int(mmap_handle[file_map_dict["mrel"][0]:file_map_dict["mrel"][1]])
+#
+#                 cache_dict["ll"] = fast_int(mmap_handle[file_map_dict["ll"][0]:file_map_dict["ll"][1]])
+#                 cache_dict["num_rows"] = fast_int(mmap_handle[file_map_dict["nrow"][0]:file_map_dict["nrow"][1]])
+#             # else:
+#             #     decompression_type = "dictionary"
+#             #     decompressor = deserialize(decompression_text)
+#         else:
+#             last_cc = file_map_dict["cc"][1]
+#             cache_dict["ll"] = fast_int(mmap_handle[(last_cc - cache_dict["ccml"]):last_cc])
+#             cache_dict["num_rows"] = fast_int((file_map_dict[""][1] - file_map_dict[""][0]) / cache_dict["ll"])
+#
+#         # Calculate line length based on last "cnicc" value.
+#         cache_dict["cniccml"] = fast_int(mmap_handle[file_map_dict["cniccml"][0]:file_map_dict["cniccml"][1]])
+#         cache_dict["cnill"] = fast_int(mmap_handle[(file_map_dict["cnicc"][1] - cache_dict["cniccml"]):file_map_dict["cnicc"][1]])
+#
+#         if "i" in file_map_dict:
+#             cache_dict["i"] = deserialize(mmap_handle[file_map_dict["i"][0]:file_map_dict["i"][1]])
+#
+#             for key in file_map_dict:
+#                 if key.endswith("ccml"):
+#                     cache_dict[key] = fast_int(mmap_handle[file_map_dict[key][0]:file_map_dict[key][1]])
+#
+#                     last_cc = file_map_dict[key[:-2]][1]
+#                     cache_dict[key.replace("ccml", "ll")] = fast_int(mmap_handle[(last_cc - cache_dict[key]):last_cc])
+#
+#         ver = mmap_handle[file_map_dict["ver"][0]:file_map_dict["ver"][1]]
+#
+#         yield FileData(data_file_path, mmap_handle, file_map_dict, cache_dict, ver, decompression_type, decompressor)
 
-            yield FileData(data_file_path, mmap_handle, file_map_dict, cache_dict, ver, decompression_type, decompressor)
+@contextmanager
+def get_file_handle(data_file_path, use_memory_mapping):
+    if use_memory_mapping:
+        with open(data_file_path, 'rb') as file_handle:
+            with mmap(file_handle.fileno(), 0, prot=PROT_READ) as mmap_handle:
+                yield mmap_handle
+    else:
+        with open(data_file_path, 'rb') as file_handle:
+            yield file_handle
 
 def get_column_index_from_name(file_data, column_name):
     position = get_identifier_row_index(file_data, "cni", column_name, file_data.cache_dict["num_cols"])
 
     if position < 0:
         raise Exception(f"Could not retrieve index because column named {column_name.decode()} was not found.")
 
@@ -760,17 +842,18 @@
     #     column_name += next_char
     #     cn_current += 1
     # cn_current += 1
 
 def get_column_type_from_index(file_data, column_index):
     return next(parse_data_values_from_file(file_data, "ct", column_index, 1, [[0, 1]])).decode()
 
-def get_value_from_single_column_file(file_handle, content_start_index, segment_length, row_index):
-    start_search_position = content_start_index + row_index * segment_length
-    return file_handle[start_search_position:(start_search_position + segment_length)].rstrip(b" ")
+# def get_value_from_single_column_file(file_handle, content_start_index, segment_length, row_index):
+#     start_search_position = content_start_index + row_index * segment_length
+#     # return file_handle[start_search_position:(start_search_position + segment_length)].rstrip(b" ")
+#     return read_from_file(file_handle, start_search_position, (start_search_position + segment_length), use_memory_mapping).rstrip(b" ")
 
 def parse_data_coord(file_data, data_file_key, index):
     ccml = file_data.cache_dict[data_file_key + "ccml"]
 
     start_pos = index * ccml
     next_start_pos = start_pos + ccml
     further_next_start_pos = next_start_pos + ccml
@@ -812,28 +895,30 @@
 
         data_coords.append([data_start_pos, data_end_pos])
 
     return data_coords
 
 def parse_data_value_from_file(file_data, data_file_key, start_element, segment_length, coords):
     start_pos = start_element * segment_length + file_data.file_map_dict[data_file_key][0]
-    return file_data.file_handle[(start_pos + coords[0]):(start_pos + coords[1])]
+    # return file_data.file_handle[(start_pos + coords[0]):(start_pos + coords[1])]
+    return read_from_file(file_data.file_handle, start_pos + coords[0], start_pos + coords[1], file_data.use_memory_mapping)
 
 def parse_data_value_from_string(coords, string):
     return string[(coords[0]):(coords[1])].rstrip(b" ")
 
 def parse_data_values_from_string(data_coords, string):
     for coords in data_coords:
         yield string[(coords[0]):(coords[1])].rstrip(b" ")
 
 def parse_data_values_from_file(file_data, data_file_key, start_element, segment_length, data_coords):
     start_pos = start_element * segment_length + file_data.file_map_dict[data_file_key][0]
 
     for coords in data_coords:
-        yield file_data.file_handle[(start_pos + coords[0]):(start_pos + coords[1])].rstrip(b" ")
+        # yield file_data.file_handle[(start_pos + coords[0]):(start_pos + coords[1])].rstrip(b" ")
+        yield read_from_file(file_data.file_handle, start_pos + coords[0], start_pos + coords[1], file_data.use_memory_mapping).rstrip(b" ")
 
 def get_parse_row_value_function(file_data):
     if not file_data.decompression_type:
         return parse_row_value
     else:
         return parse_zstd_compressed_row_value
 
@@ -867,22 +952,25 @@
     re_overall_start = file_data.file_map_dict["re"][0]
 
     if row_index == 0:
         row_start = 0
     else:
         row_start_start = re_overall_start + (row_index - 1) * mrel
         row_start_end = row_start_start + mrel
-        row_start = int(file_data.file_handle[row_start_start:row_start_end].rstrip(b' '))
+        # row_start = int(file_data.file_handle[row_start_start:row_start_end].rstrip(b' '))
+        row_start = int(read_from_file(file_data.file_handle, row_start_start, row_start_end, file_data.use_memory_mapping).rstrip(b' '))
 
     row_end_start = re_overall_start + row_index * mrel
     row_end_end = row_end_start + mrel
-    row_end = int(file_data.file_handle[row_end_start:row_end_end].rstrip(b' '))
+    # row_end = int(file_data.file_handle[row_end_start:row_end_end].rstrip(b' '))
+    row_end = int(read_from_file(file_data.file_handle, row_end_start, row_end_end, file_data.use_memory_mapping).rstrip(b' '))
 
     data_start = file_data.file_map_dict[""][0]
-    return file_data.decompressor.decompress(file_data.file_handle[(data_start + row_start):(data_start + row_end)])
+    # return file_data.decompressor.decompress(file_data.file_handle[(data_start + row_start):(data_start + row_end)])
+    return file_data.decompressor.decompress(read_from_file(file_data.file_handle, data_start + row_start, data_start + row_end, file_data.use_memory_mapping))
 
 # def parse_dictionary_compressed_row_value(file_data, data_file_key, row_index, column_coords, bigram_size_dict=None, column_name=None):
 #     value = parse_data_value_from_file(file_data, data_file_key, row_index, file_data.cache_dict["ll"], column_coords).rstrip(b" ")
 #     return decompress(value, file_data.decompressor[column_name], bigram_size_dict[column_name])
 
 def get_parse_row_values_function(file_data):
     if not file_data.decompression_type:
@@ -935,16 +1023,16 @@
         try:
             yield write_obj
         finally:
             write_obj.close()
     else:
         yield sys.stdout.buffer
 
-def save_output_rows(in_file_path, out_file_path, row_indices, column_indices):
-    with initialize(in_file_path) as file_data:
+def save_output_rows(in_file_path, use_memory_mapping, out_file_path, row_indices, column_indices):
+    with initialize(in_file_path, use_memory_mapping) as file_data:
         with get_write_object(out_file_path, "ab") as write_obj:
             select_column_coords = parse_data_coords(file_data, "", column_indices)
             parse_row_values_function = get_parse_row_values_function(file_data)
 
             for row_index in row_indices:
                 write_obj.write(b"\t".join(parse_row_values_function(file_data, "", row_index, select_column_coords)) + b"\n")
 
@@ -1173,16 +1261,16 @@
     for i in range(positions[0], positions[1]):
         matching_row_indices.add(fast_int(parse_row_value(file_data, data_file_key, i, position_coords)))
 
     return matching_row_indices
 
 # This is the same as the function above it, but it needs to pass the file path
 # to work with joblib.
-def find_matching_row_indices_parallel(data_file_path, data_file_key, position_coords, positions):
-    with initialize(data_file_path) as file_data:
+def find_matching_row_indices_parallel(data_file_path, use_memory_mapping, data_file_key, position_coords, positions):
+    with initialize(data_file_path, use_memory_mapping) as file_data:
         matching_row_indices = set()
 
         for i in range(positions[0], positions[1]):
             matching_row_indices.add(fast_int(parse_row_value(file_data, data_file_key, i, position_coords)))
 
         return matching_row_indices
 
@@ -1196,15 +1284,15 @@
         chunk_size = ceil(num_indices / num_parallel)
 
         position_chunks = []
         for i in range(positions[0], positions[1], chunk_size):
             position_chunks.append((i, min(positions[1], i + chunk_size)))
 
         return set(chain.from_iterable(joblib.Parallel(n_jobs=num_parallel)(
-            joblib.delayed(find_matching_row_indices_parallel)(file_data.data_file_path, data_file_key, position_coords, position_chunk)
+            joblib.delayed(find_matching_row_indices_parallel)(file_data.data_file_path, file_data.use_memory_mapping, data_file_key, position_coords, position_chunk)
             for position_chunk in position_chunks))
         )
 
 def find_bounds_for_range(file_data, data_file_key, value_coords, filter1, filter2, start_search_position, end_search_position):
     lower_positions = find_positions_g(file_data, data_file_key, value_coords, filter1, start_search_position, end_search_position, lt)
     upper_positions = find_positions_l(file_data, data_file_key, value_coords, filter2, lower_positions[0], lower_positions[1], le)
```

### Comparing `f4-0.9.8/src/f4/Transformer.py` & `f4-0.9.9/src/f4/Transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from .Builder import *
 from .Parser import *
 
-def transpose(f4_src_file_path, f4_dest_file_path, src_column_for_names, index_columns=[], num_parallel=1, tmp_dir_path=None, verbose=False):
+# FYI: Memory mapping seems to use too much memory in this context with large files, so the default is False.
+def transpose(f4_src_file_path, f4_dest_file_path, src_column_for_names, index_columns=[], num_parallel=1, tmp_dir_path=None, use_memory_mapping=False, verbose=False):
     if src_column_for_names is None or not isinstance(src_column_for_names, str) or len(src_column_for_names) == 0:
         raise Exception(f"The value specified for src_column_for_names was invalid.")
 
     print_message(f"Finding max column width when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
 
-    with initialize(f4_src_file_path) as src_file_data:
+    with initialize(f4_src_file_path, use_memory_mapping) as src_file_data:
         num_cols = src_file_data.cache_dict["num_cols"]
         max_column_width = get_max_column_width(src_file_data)
 
     tmp_dir_path2 = prepare_tmp_dir(tmp_dir_path)
     tmp_tsv_file_path = f"{tmp_dir_path2}transposed.tsv.zstd"
 
     if num_parallel == 1:
-        transpose_column_chunk(f4_src_file_path, src_column_for_names, 0, range(num_cols), max_column_width, tmp_tsv_file_path, verbose)
+        transpose_column_chunk(f4_src_file_path, use_memory_mapping, src_column_for_names, 0, range(num_cols), max_column_width, tmp_tsv_file_path, verbose)
     else:
         max_cols_per_chunk = 10001
 
         global joblib
         joblib = __import__('joblib', globals(), locals())
 
         # Transpose the data in chunks.
         joblib.Parallel(n_jobs=num_parallel)(joblib.delayed(transpose_column_chunk)(
             f4_src_file_path,
+            use_memory_mapping,
             src_column_for_names,
             chunk_number,
             chunk_range,
             max_column_width,
             f"{tmp_dir_path2}transposed_chunk_{chunk_number}.tsv.zstd",
             verbose)
                 for chunk_number, chunk_range in enumerate(generate_column_ranges(max_cols_per_chunk, num_cols, num_parallel))
@@ -72,18 +74,18 @@
         # Find the max width of values.
         column_coords = parse_data_coord(src_file_data, "", column_index)
         column_size = column_coords[1] - column_coords[0]
         max_column_width = max(max_column_width, column_size)
 
     return max_column_width
 
-def transpose_column_chunk(f4_src_file_path, src_column_for_names, chunk_number, column_range, max_column_width, tmp_tsv_file_path, verbose):
+def transpose_column_chunk(f4_src_file_path, use_memory_mapping, src_column_for_names, chunk_number, column_range, max_column_width, tmp_tsv_file_path, verbose):
     tmp_fw_file_path = f"{tmp_tsv_file_path}.fw"
 
-    with initialize(f4_src_file_path) as src_file_data:
+    with initialize(f4_src_file_path, use_memory_mapping) as src_file_data:
         print_message(f"Parsing column coordinates for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
         # Get basic meta information.
         num_rows = src_file_data.cache_dict["num_rows"]
         src_column_for_names_index = get_column_index_from_name(src_file_data, src_column_for_names.encode())
         src_column_for_names_coords = parse_data_coord(src_file_data, "", src_column_for_names_index)
         parse_row_value_function = get_parse_row_value_function(src_file_data)
         parse_row_values_function = get_parse_row_values_function(src_file_data)
@@ -171,46 +173,48 @@
 
 def advance_to_column_names(src_file_data, first_col_index):
     cn_current = src_file_data.file_map_dict["cn"][0]
     cn_end = src_file_data.file_map_dict["cn"][1]
 
     # Advance to the first column name for this chunk range.
     for column_index in range(first_col_index):
-        while src_file_data.file_handle[cn_current:(cn_current + 1)] != b"\n":
+        # while src_file_data.file_handle[cn_current:(cn_current + 1)] != b"\n":
+        while read_from_file(src_file_data.file_handle, cn_current, cn_current + 1, src_file_data.use_memory_mapping) != b"\n":
             cn_current += 1
         cn_current += 1
 
     return cn_current, cn_end
 
 def get_next_column_name(src_file_data, cn_current, cn_end):
     # Parse the column name, one character at a time.
     column_name = b""
-    while cn_current < cn_end and (next_char := src_file_data.file_handle[cn_current:(cn_current + 1)]) != b"\n":
+    # while cn_current < cn_end and (next_char := src_file_data.file_handle[cn_current:(cn_current + 1)]) != b"\n":
+    while cn_current < cn_end and (next_char := read_from_file(src_file_data.file_handle, cn_current, cn_current + 1, src_file_data.use_memory_mapping)) != b"\n":
         column_name += next_char
         cn_current += 1
 
     return cn_current + 1, column_name
 
 #TODO: This function is not yet designed for files with 1000000+ columns.
-def inner_join(f4_left_src_file_path, f4_right_src_file_path, join_column, f4_dest_file_path, index_columns=[], num_parallel=1, tmp_dir_path=None, verbose=False):
+def inner_join(f4_left_src_file_path, f4_right_src_file_path, join_column, f4_dest_file_path, index_columns=[], num_parallel=1, tmp_dir_path=None, use_memory_mapping=True, verbose=False):
     #TODO: Add error checking to make sure join_column is present in left and right.
     print_message(f"Inner joining {f4_left_src_file_path} and {f4_right_src_file_path} based on the {join_column} column, saving to {f4_dest_file_path}.", verbose)
 
     join_column = join_column.encode()
 
     if tmp_dir_path:
         makedirs(tmp_dir_path, exist_ok=True)
     else:
         tmp_dir_path = mkdtemp()
 
     tmp_dir_path = fix_dir_path_ending(tmp_dir_path)
     tmp_tsv_file_path = f"{tmp_dir_path}tmp.tsv.zstd"
 
-    with initialize(f4_left_src_file_path) as left_file_data:
-        with initialize(f4_right_src_file_path) as right_file_data:
+    with initialize(f4_left_src_file_path, use_memory_mapping) as left_file_data:
+        with initialize(f4_right_src_file_path, use_memory_mapping) as right_file_data:
             # Determine which functions are suitable for parsing the join column info.
             left_parse_row_value_function = get_parse_row_value_function(left_file_data)
             right_parse_row_value_function = get_parse_row_value_function(right_file_data)
 
             # Find the index of the join column in each file.
             left_join_column_index = get_column_index_from_name(left_file_data, join_column)
             right_join_column_index = get_column_index_from_name(right_file_data, join_column)
```

### Comparing `f4-0.9.8/src/f4/Utilities.py` & `f4-0.9.9/src/f4/Utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,23 +17,30 @@
 import sqlite3
 import sys
 from tempfile import mkdtemp
 from uuid import uuid4
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 def get_current_version():
-    return "0.9.8"
+    return "0.9.9"
 
 #####################################################
 # Constants
 #####################################################
 
 def get_current_version_major():
     return get_current_version().split(".")[0]
 
+def read_from_file(file_handle, start_position, end_position, use_memory_mapping):
+    if use_memory_mapping:
+        return file_handle[start_position:end_position]
+    else:
+        file_handle.seek(start_position)
+        return file_handle.read(end_position - start_position)
+
 def read_str_from_file(file_path, file_extension=""):
     with open_temp_file_compressed(file_path + file_extension) as the_file:
         return the_file.read()
 
 def write_str_to_file(file_path, the_string):
     with open_temp_file_to_compress(file_path) as the_file:
         the_file.write(the_string)
```

### Comparing `f4-0.9.8/src/f4.egg-info/PKG-INFO` & `f4-0.9.9/src/f4.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

