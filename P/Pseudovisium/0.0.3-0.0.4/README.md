# Comparing `tmp/Pseudovisium-0.0.3.tar.gz` & `tmp/Pseudovisium-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pseudovisium-0.0.3.tar", last modified: Tue Apr 23 09:38:37 2024, max compression
+gzip compressed data, was "Pseudovisium-0.0.4.tar", last modified: Fri Apr 26 08:27:19 2024, max compression
```

## Comparing `Pseudovisium-0.0.3.tar` & `Pseudovisium-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-23 09:38:37.308315 Pseudovisium-0.0.3/
--rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-04-08 13:33:17.000000 Pseudovisium-0.0.3/LICENSE
--rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-23 09:38:37.308100 Pseudovisium-0.0.3/PKG-INFO
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-23 09:38:37.306480 Pseudovisium-0.0.3/Pseudovisium/
--rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-04-18 09:05:07.000000 Pseudovisium-0.0.3/Pseudovisium/__init__.py
--rw-r--r--   0 k23030440   (504) staff       (20)    59722 2024-04-22 10:42:50.000000 Pseudovisium-0.0.3/Pseudovisium/pseudovisium_generate.py
--rw-r--r--   0 k23030440   (504) staff       (20)    14626 2024-04-16 20:47:21.000000 Pseudovisium-0.0.3/Pseudovisium/pseudovisium_merge.py
--rw-r--r--   0 k23030440   (504) staff       (20)    58609 2024-04-23 09:35:07.000000 Pseudovisium-0.0.3/Pseudovisium/pseudovisium_qc.py
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-23 09:38:37.307826 Pseudovisium-0.0.3/Pseudovisium.egg-info/
--rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-23 09:38:37.000000 Pseudovisium-0.0.3/Pseudovisium.egg-info/PKG-INFO
--rw-r--r--   0 k23030440   (504) staff       (20)      335 2024-04-23 09:38:37.000000 Pseudovisium-0.0.3/Pseudovisium.egg-info/SOURCES.txt
--rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-04-23 09:38:37.000000 Pseudovisium-0.0.3/Pseudovisium.egg-info/dependency_links.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       39 2024-04-23 09:38:37.000000 Pseudovisium-0.0.3/Pseudovisium.egg-info/requires.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       13 2024-04-23 09:38:37.000000 Pseudovisium-0.0.3/Pseudovisium.egg-info/top_level.txt
--rw-r--r--   0 k23030440   (504) staff       (20)     3058 2024-04-23 09:35:49.000000 Pseudovisium-0.0.3/README.md
--rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-04-23 09:38:37.308377 Pseudovisium-0.0.3/setup.cfg
--rw-r--r--   0 k23030440   (504) staff       (20)      911 2024-04-23 09:38:13.000000 Pseudovisium-0.0.3/setup.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-26 08:27:19.515593 Pseudovisium-0.0.4/
+-rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-04-08 13:33:17.000000 Pseudovisium-0.0.4/LICENSE
+-rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-26 08:27:19.515320 Pseudovisium-0.0.4/PKG-INFO
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-26 08:27:19.513405 Pseudovisium-0.0.4/Pseudovisium/
+-rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-04-18 09:05:07.000000 Pseudovisium-0.0.4/Pseudovisium/__init__.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    56091 2024-04-26 08:05:45.000000 Pseudovisium-0.0.4/Pseudovisium/pseudovisium_generate.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    14501 2024-04-23 21:00:08.000000 Pseudovisium-0.0.4/Pseudovisium/pseudovisium_merge.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    68606 2024-04-24 16:52:07.000000 Pseudovisium-0.0.4/Pseudovisium/pseudovisium_qc.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-26 08:27:19.514935 Pseudovisium-0.0.4/Pseudovisium.egg-info/
+-rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-26 08:27:19.000000 Pseudovisium-0.0.4/Pseudovisium.egg-info/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)      335 2024-04-26 08:27:19.000000 Pseudovisium-0.0.4/Pseudovisium.egg-info/SOURCES.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-04-26 08:27:19.000000 Pseudovisium-0.0.4/Pseudovisium.egg-info/dependency_links.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       39 2024-04-26 08:27:19.000000 Pseudovisium-0.0.4/Pseudovisium.egg-info/requires.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       13 2024-04-26 08:27:19.000000 Pseudovisium-0.0.4/Pseudovisium.egg-info/top_level.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)     3637 2024-04-26 08:21:23.000000 Pseudovisium-0.0.4/README.md
+-rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-04-26 08:27:19.515658 Pseudovisium-0.0.4/setup.cfg
+-rw-r--r--   0 k23030440   (504) staff       (20)      911 2024-04-26 08:25:03.000000 Pseudovisium-0.0.4/setup.py
```

### Comparing `Pseudovisium-0.0.3/LICENSE` & `Pseudovisium-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.3/PKG-INFO` & `Pseudovisium-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pseudovisium
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for hexagonal binning of high-resolution spatial transcriptomic data
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: spatial,transcriptomics,visium,xenium,cosmx
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Pseudovisium-0.0.3/Pseudovisium/pseudovisium_generate.py` & `Pseudovisium-0.0.4/Pseudovisium/pseudovisium_generate.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,41 +2,29 @@
 from collections import defaultdict
 import numpy as np
 import math
 import pandas as pd
 import cv2
 import json
 import gzip
-import csv
 import concurrent.futures
 import os
 import shutil
 import tempfile
 from tqdm import tqdm
 import itertools
-import psutil
 import argparse
 import tifffile
-import imagecodecs
 import multiprocessing
 import time
 import scanpy as sc
-from scipy.sparse import csr_matrix
-import concurrent.futures
-import itertools
-import csv
-import multiprocessing
-from tqdm import tqdm
-from scipy.io import mmwrite
-
-
-##Changes
-#Save Fov information if provided
-#Save quality score information if provided
-
+import scipy.io
+import h5py
+import scipy.sparse
+from pathlib import Path
 
 def closest_hex(x,y,hexagon_size):
     """
     closest_hex(x, y, hexagon_size)
     Calculates the closest hexagon centroid to the given (x, y) coordinates.
 
     Args:
@@ -86,51 +74,14 @@
         closest = [option_1_hexagon,option_2_hexagon,option_3_hexagon][np.argmin([distance_1,distance_2,distance_3])]
 
     closest = (round(closest[0], 0), round(closest[1], 1))
     return closest
 
 
 
-def initialize_hexagons(hexagon_size, field_size):
-    """
-    initialize_hexagons(hexagon_size, field_size)
-    Initializes a dictionary of hexagon centroids for a given hexagon size and field size.
-
-    Args:
-    hexagon_size (float): The size of the hexagon.
-    field_size (tuple): The size of the field as (field_size_x, field_size_y).
-
-    Returns:
-        dict: A dictionary where the keys are the hexagon centroid coordinates (x, y) and the values are the same coordinates.
-    """
-
-
-
-    print('initializing hexagons')
-    # given an initial x and y coordinate, this function will create a zig-zag hexagonal lattice, where
-    # hexagon size is the distance from the centroid to the vertex
-    hexagons = {(0, 0): (0, 0)}
-    # create hexagon centroids
-    field_size_x, field_size_y = field_size
-    for dy, i in zip(np.arange(-field_size_y * (1.732050807 * hexagon_size), (field_size_y) * (1.732050807 * hexagon_size), 1.732050807 * hexagon_size), [1, 2] * field_size_y):
-        if i == 1:
-            for dx in range((-field_size_x + 1) * hexagon_size, (field_size_x + 1) * hexagon_size, 2 * hexagon_size):
-
-                hexagons[(dx, dy)] = (dx, dy)
-        else:
-            for dx in range((-field_size_x) * hexagon_size, (field_size_x) * hexagon_size, 2 * hexagon_size):
-                
-                hexagons[(dx, dy)] = (dx, dy)
-    min_x = min([x for x, y in hexagons.keys()])
-    min_y = min([y for x, y in hexagons.keys()])
-    # rename hexagons both keys and values
-    hexagons = {(round(x - min_x, 0), round(y - min_y, 1)): (round(x - min_x, 0), round(y - min_y, 1)) for (x, y) in hexagons.keys()}
-    
-    return hexagons
-
 
 def preprocess_csv(csv_file, batch_size, fieldnames):
     """
     preprocess_csv(csv_file, batch_size, fieldnames)
     Preprocesses a CSV file by splitting it into smaller batches.
 
     Args:
@@ -145,14 +96,15 @@
 
 
     tmp_dir = tempfile.mkdtemp(prefix="tmp_hexa")
     print(f"Created temporary directory {tmp_dir}")
     #if csv_file is .gz, then open it with gzip
     if csv_file.endswith('.gz'):
         with gzip.open(csv_file, 'rt') as file:
+            print("Now creating batches")
             reader = csv.DictReader(file)
             header = next(reader)  # Read the header row
             batch_num = 0
 
             while True:
                 batch = list(itertools.islice(reader, batch_size))
                 if not batch:
@@ -194,15 +146,15 @@
     return tmp_dir, batch_num
 
 
 def default_factory():
 
     return defaultdict(int)
 
-def process_batch(batch_file, hexagon_size, feature_colname, x_colname, y_colname, cell_id_colname, quality_colname=None, quality_filter=False, count_colname="NA",smoothing=False, quality_per_hexagon=False, quality_per_probe=False):
+def process_batch(batch_file, hexagon_size, feature_colname, x_colname, y_colname, cell_id_colname, quality_colname=None, quality_filter=False, count_colname="NA",smoothing=False, quality_per_hexagon=False, quality_per_probe=False,move_x=0,move_y=0):
     """
     process_batch(batch_file, hexagon_size, feature_colname, x_colname, y_colname, cell_id_colname, quality_colname=None, quality_filter=False, count_colname="NA", smoothing=False)
     Processes a batch CSV file to calculate hexagon counts and cell counts.
 
     Args:
     batch_file (str): The path to the batch CSV file.
     hexagon_size (float): The size of the hexagon.
@@ -217,34 +169,31 @@
 
     Returns:
         dict or tuple: If cell_id_colname is not "None", returns a tuple containing the hexagon counts and hexagon cell counts.
                     Otherwise, returns the hexagon counts dictionary.
 
     """
     
-    
-    hexagon_counts = {}
+    hexagon_counts = defaultdict(default_factory)
     if cell_id_colname != "None":
-        hexagon_cell_counts = {}
+        hexagon_cell_counts = defaultdict(default_factory)
     if quality_per_hexagon==True:
-        hexagon_quality = {}
+        hexagon_quality = defaultdict(default_factory)
     if quality_per_probe==True:
-        probe_quality = {}
+        probe_quality = defaultdict(default_factory)
     if count_colname == "NA":
-        print(f"Quality filter is set to {quality_filter}")
-        print(f"Quality counting per hexagon is set to {quality_per_hexagon}")
-        print(f"Quality counting per probe is set to {quality_per_probe}")
+        
 
         ##########Xenium with quality filter scenario
         with open(batch_file, 'r') as file:
             reader = csv.DictReader(file)
             for row in reader:
                 try:
-                    x = float(row[x_colname])
-                    y = float(row[y_colname])
+                    x = float(row[x_colname]) + move_x
+                    y = float(row[y_colname]) + move_y
                     closest_hexagon = closest_hex(x, y, hexagon_size)
                     if quality_per_hexagon==True:
                         if closest_hexagon not in hexagon_quality:
                             hexagon_quality[closest_hexagon] = {"mean":float(row[quality_colname]),"count":1}
                         else:
                             hexagon_quality[closest_hexagon]["mean"] = (hexagon_quality[closest_hexagon]["mean"]*hexagon_quality[closest_hexagon]["count"]+float(row[quality_colname]))/(hexagon_quality[closest_hexagon]["count"]+1)
                             hexagon_quality[closest_hexagon]["count"]+=1
@@ -254,76 +203,52 @@
                         else:
                             probe_quality[row[feature_colname]]["mean"] = (probe_quality[row[feature_colname]]["mean"]*probe_quality[row[feature_colname]]["count"]+float(row[quality_colname]))/(probe_quality[row[feature_colname]]["count"]+1)
                             probe_quality[row[feature_colname]]["count"]+=1
 
                     if quality_filter==True and float(row[quality_colname]) < 20:
                         continue
                     else:
-                        if closest_hexagon not in hexagon_counts:
-                            hexagon_counts[closest_hexagon] = {}
-                        if row[feature_colname] not in hexagon_counts[closest_hexagon]:
-                            hexagon_counts[closest_hexagon][row[feature_colname]] = 0
                         hexagon_counts[closest_hexagon][row[feature_colname]] += 1
                         if cell_id_colname != "None":
-                            if closest_hexagon not in hexagon_cell_counts:
-                                hexagon_cell_counts[closest_hexagon] = {}
-                            if row[cell_id_colname] not in hexagon_cell_counts[closest_hexagon]:
-                                hexagon_cell_counts[closest_hexagon][row[cell_id_colname]] = 0
                             hexagon_cell_counts[closest_hexagon][row[cell_id_colname]] += 1
                     
 
                 except ValueError:
-                    print(f"Skipping row due to invalid coordinates: {row}")
+                    print(f"Skipping row")
         
     else:
         if smoothing!=False:
             print("Smoothing is on. Counts will be spread into four neighboring squares")
             with open(batch_file, 'r') as file:
                 ##########Visium HD with smoothing scenario
                 reader = csv.DictReader(file)
                 for row in reader:
                     try:
-                        x = float(row[x_colname])
-                        y = float(row[y_colname])
+                        x = float(row[x_colname])+move_x
+                        y = float(row[y_colname])+move_y
                         for x_new,y_new in [(x+smoothing,y+smoothing),(x-smoothing,y-smoothing),(x-smoothing,y+smoothing),(x+smoothing,y-smoothing)]:
                             closest_hexagon = closest_hex(x_new, y_new, hexagon_size)
-                            if closest_hexagon not in hexagon_counts:
-                                hexagon_counts[closest_hexagon] = {}
-                            if row[feature_colname] not in hexagon_counts[closest_hexagon]:
-                                hexagon_counts[closest_hexagon][row[feature_colname]] = 0
                             hexagon_counts[closest_hexagon][row[feature_colname]] += float(row[count_colname])/4
                             if cell_id_colname != "None":
-                                if closest_hexagon not in hexagon_cell_counts:
-                                    hexagon_cell_counts[closest_hexagon] = {}
-                                if row[cell_id_colname] not in hexagon_cell_counts[closest_hexagon]:
-                                    hexagon_cell_counts[closest_hexagon][row[cell_id_colname]] = 0
                                 hexagon_cell_counts[closest_hexagon][row[cell_id_colname]] += float(row[count_colname])/4
                     except ValueError:
                         print(f"Skipping row due to invalid coordinates: {row}")
         else:
             print("No smoothing")
             with open(batch_file, 'r') as file:
                 ##########Visium HD scenario without smoothing
                 
                 reader = csv.DictReader(file)
                 for row in reader:
                     try:
-                        x = float(row[x_colname])
-                        y = float(row[y_colname])
+                        x = float(row[x_colname])+move_x
+                        y = float(row[y_colname])+move_y
                         closest_hexagon = closest_hex(x, y, hexagon_size)
-                        if closest_hexagon not in hexagon_counts:
-                            hexagon_counts[closest_hexagon] = {}
-                        if row[feature_colname] not in hexagon_counts[closest_hexagon]:
-                            hexagon_counts[closest_hexagon][row[feature_colname]] = 0
                         hexagon_counts[closest_hexagon][row[feature_colname]] += float(row[count_colname])
                         if cell_id_colname != "None":
-                            if closest_hexagon not in hexagon_cell_counts:
-                                hexagon_cell_counts[closest_hexagon] = {}
-                            if row[cell_id_colname] not in hexagon_cell_counts[closest_hexagon]:
-                                hexagon_cell_counts[closest_hexagon][row[cell_id_colname]] = 0
                             hexagon_cell_counts[closest_hexagon][row[cell_id_colname]] += float(row[count_colname])
                     except ValueError:
                         print(f"Skipping row due to invalid coordinates: {row}")
 
     returning_items = [hexagon_counts]
 
     if cell_id_colname != "None":
@@ -332,32 +257,27 @@
         returning_items.append(hexagon_quality)
     if quality_per_probe==True:
         returning_items.append(probe_quality)
     return tuple(returning_items)
 
 
 
-from concurrent.futures import ThreadPoolExecutor
-from tqdm import tqdm
+
 def process_batch_hexagons(batch,hexagon_counts,hexagon_names,features):
         batch_matrix_data = []
         for hexagon in batch:
             count_dict = hexagon_counts.get(hexagon, {})
             if sum(count_dict.values()) > 0:
                 hexagon_index = hexagon_names.index(hexagon)
                 for feature, count in count_dict.items():
                     feature_index = features.index(feature)
                     batch_matrix_data.append([feature_index+1, hexagon_index+1, count])
         return batch_matrix_data
 
 
-import h5py
-import numpy as np
-from scipy.sparse import csr_matrix
-from pathlib import Path
 def write_10X_h5(adata, file):
     """Writes adata to a 10X-formatted h5 file.
     
     Note that this function is not fully tested and may not work for all cases.
     It will not write the following keys to the h5 file compared to 10X:
     '_all_tag_keys', 'pattern', 'read', 'sequence'
 
@@ -405,16 +325,16 @@
     ftrs.create_dataset("name", data=adata.var.index.values.astype('|S'))
     
     w.close()
 
     
 
 
-def process_csv_file(csv_file, hexagon_size, field_size, batch_size=1000000, technology="Xenium", feature_colname="feature_name", x_colname="x_location", y_colname="y_location", cell_id_colname="None", quality_colname="qv", max_workers=min(2, multiprocessing.cpu_count()),
-                     quality_filter=False, count_colname="NA",smoothing=False,quality_per_hexagon=False,quality_per_probe=False,h5_x_colname="x",h5_y_colname="y"):
+def process_csv_file(csv_file, hexagon_size, batch_size=1000000, technology="Xenium", feature_colname="feature_name", x_colname="x_location", y_colname="y_location", cell_id_colname="None", quality_colname="qv", max_workers=min(2, multiprocessing.cpu_count()),
+                     quality_filter=False, count_colname="NA",smoothing=False,quality_per_hexagon=False,quality_per_probe=False,h5_x_colname="x",h5_y_colname="y",move_x=0,move_y=0):
     """
     process_csv_file(csv_file, hexagon_size, field_size, batch_size=1000000, technology="Xenium", feature_colname="feature_name", x_colname="x_location", y_colname="y_location", cell_id_colname="None", quality_colname="qv", max_workers=min(2, multiprocessing.cpu_count()), quality_filter=False, count_colname="NA", smoothing=False)
     Processes a CSV file to calculate hexagon counts and cell counts using parallel processing.
 
     Args:
     csv_file (str): The path to the CSV file.
     hexagon_size (float): The size of the hexagon.
@@ -431,23 +351,22 @@
     count_colname (str, optional): The name of the count column. Defaults to "NA".
     smoothing (bool, optional): Whether to apply smoothing to the counts. Defaults to False.
 
     Returns:
         tuple: A tuple containing the hexagon counts, hexagons dictionary, and hexagon cell counts.
     """
 
-
-
-
-
-    hexagons = initialize_hexagons(hexagon_size, field_size)
-    hexagon_counts = {hexagon: defaultdict(int) for hexagon in hexagons}
-    hexagon_cell_counts = {hexagon: defaultdict(int) for hexagon in hexagons}
-    hexagon_quality = {hexagon: defaultdict(int) for hexagon in hexagons}
-    probe_quality = {}
+    print(f"Quality filter is set to {quality_filter}")
+    print(f"Quality counting per hexagon is set to {quality_per_hexagon}")
+    print(f"Quality counting per probe is set to {quality_per_probe}")
+
+    hexagon_counts = defaultdict(default_factory)
+    hexagon_cell_counts = defaultdict(default_factory)
+    hexagon_quality = defaultdict(default_factory)
+    probe_quality = defaultdict(default_factory)
     #create a nested dict called hexagon quality, with two keys for each hexagon, one for the quality score and one for the count
     
     if technology == "Xenium":
         print("Technology is Xenium. Going forward with default column names.")
         x_colname = "x_location"
         y_colname = "y_location"
         feature_colname = "feature_name"
@@ -507,51 +426,55 @@
     if count_colname!="NA":
         fieldnames.append(count_colname)
 
 
 
     tmp_dir, num_batches = preprocess_csv(csv_file, batch_size, fieldnames)
     batch_files = [os.path.join(tmp_dir, f"batch_{i}.csv") for i in range(num_batches)]
-    with concurrent.futures.ProcessPoolExecutor(max_workers=min(max_workers, multiprocessing.cpu_count())) as executor:
-        futures = [executor.submit(process_batch, batch_file, hexagon_size, feature_colname, x_colname, y_colname, cell_id_colname, quality_colname, quality_filter, count_colname,smoothing,quality_per_hexagon,quality_per_probe) for batch_file in batch_files]
+    n_threads = min(max_workers, multiprocessing.cpu_count())
+    print(f"Processing batches using {n_threads} threads")
+    with concurrent.futures.ThreadPoolExecutor(max_workers=n_threads) as executor:
+        futures = [executor.submit(process_batch, batch_file, hexagon_size, feature_colname, x_colname, y_colname, cell_id_colname, quality_colname, quality_filter, count_colname,smoothing,quality_per_hexagon,quality_per_probe, move_x,move_y) for batch_file in batch_files]
         
         with tqdm(total=len(batch_files), desc="Processing batches", unit="batch") as progress_bar:
             for future in concurrent.futures.as_completed(futures):
                 all_res = future.result()
                 batch_hexagon_counts = all_res[0]
                 for hexagon_counts_hex, counts in batch_hexagon_counts.items():
                     for feature_name, count in counts.items():
                         try:
                             hexagon_counts[hexagon_counts_hex][feature_name] += count
+                            
+                                
                         except KeyError:
-                            print(f"Feature {feature_name} not found in hexagon_counts")
+                            print(f"Error in trying to add to hexagon_counts")
 
                 if cell_id_colname != "None":
                     batch_hexagon_cell_counts = all_res[1]
                     for hexagon_cell_counts_hex, cell_counts in batch_hexagon_cell_counts.items():
                         for cell_id, cell_count in cell_counts.items():
                             try:
                                 hexagon_cell_counts[hexagon_cell_counts_hex][cell_id] += cell_count
                             except KeyError:
-                                print(f"Cell ID {cell_id} not found in hexagon_cell_counts")
+                                print(f"Error in trying to add to hexagon_cell_counts")
 
                 if quality_per_hexagon==True:
                     if cell_id_colname != "None":
                         batch_hexagon_quality = all_res[2]
                     else:
                         batch_hexagon_quality = all_res[1]
                     for hexagon_quality_hex, quality_dict in batch_hexagon_quality.items():
                         try:
                             if hexagon_quality_hex not in hexagon_quality:
                                 hexagon_quality[hexagon_quality_hex] = quality_dict
                             else:
                                 hexagon_quality[hexagon_quality_hex]["mean"] = (float(hexagon_quality[hexagon_quality_hex]["mean"]) * hexagon_quality[hexagon_quality_hex]["count"] + float(quality_dict["mean"]) * quality_dict["count"]) / (hexagon_quality[hexagon_quality_hex]["count"] + quality_dict["count"])
                                 hexagon_quality[hexagon_quality_hex]["count"] += quality_dict["count"]
                         except KeyError:
-                            print(f"Quality not found in hexagon_quality for hexagon {hexagon_quality_hex}")
+                            print(f"Error in trying to add to hexagon_quality")
                 
                 if quality_per_probe==True:
                     if cell_id_colname != "None" and quality_per_hexagon==True:
                         batch_probe_quality = all_res[3]
                     elif cell_id_colname != "None" and quality_per_hexagon==False:
                         batch_probe_quality = all_res[2]
                     elif cell_id_colname == "None" and quality_per_hexagon==True:
@@ -564,44 +487,34 @@
                         try:
                             if probe not in probe_quality:
                                 probe_quality[probe] = quality_dict
                             else:
                                 probe_quality[probe]["mean"] = (float(probe_quality[probe]["mean"]) * probe_quality[probe]["count"] + float(quality_dict["mean"]) * quality_dict["count"]) / (probe_quality[probe]["count"] + quality_dict["count"])
                                 probe_quality[probe]["count"] += quality_dict["count"]
                         except KeyError:
-                            print(f"Quality not found in probe_quality for probe {probe}")
+                            print(f"Error in trying to add to probe_quality")
                 progress_bar.update(1)
 
     shutil.rmtree(tmp_dir)  # Remove temporary directory and files
 
-    return hexagon_counts, hexagons, hexagon_cell_counts, hexagon_quality, probe_quality
+    return hexagon_counts, hexagon_cell_counts, hexagon_quality, probe_quality
 
-from concurrent.futures import ThreadPoolExecutor
-from tqdm import tqdm
 
-def hex_to_rows(hexagon_batch, hexagon_indices, features, hexagon_counts):
-    """
-    hex_to_rows(hexagon_batch, hexagon_indices, features, hexagon_counts)
-    Converts a batch of hexagons to matrix rows.
-
-    Args:
-        hexagon_batch (list): A list of hexagon coordinates.
-        hexagon_indices (list): A list of hexagon indices.
-        features (list): A list of feature names.
-        hexagon_counts (dict): A dictionary of hexagon counts.
-
-    Returns:
-        list: A list of matrix rows, where each row contains the feature index, hexagon index, and count.
-    """
-    def process_hexagon(hexagon, hexagon_index):
+def process_hexagon(hexagon, hexagon_index, features, hexagon_counts):
         return [[features.index(feature) + 1, hexagon_index + 1, count]
                 for feature, count in hexagon_counts[hexagon].items()]
 
-    matrix_data = [item for hexagon, hexagon_index in zip(hexagon_batch, hexagon_indices)
-                   for item in process_hexagon(hexagon, hexagon_index)]
+def hex_to_rows(hexagon_batch, start_index, features, hexagon_counts):
+    matrix_data = []
+    for hexagon_index, hexagon in enumerate(hexagon_batch, start=start_index):
+        count_dict = hexagon_counts.get(hexagon, {})
+        for feature, count in count_dict.items():
+            feature_index = features.index(feature)
+            matrix_data.append([feature_index + 1, hexagon_index + 1, count])
+    print(f"Batch total count: {sum(row[2] for row in matrix_data)}")
     return matrix_data
 
 def create_pseudovisium(path,hexagon_counts,hexagon_cell_counts,hexagon_quality, probe_quality,
                         img_file_path=None,  project_name="project",
                          alignment_matrix_file=None,image_pixels_per_um=1/0.2125,hexagon_size=100,tissue_hires_scalef=0.2,
                          pixel_to_micron=False,max_workers=min(2, multiprocessing.cpu_count())):
     """
@@ -683,55 +596,55 @@
                                       'pxl_row_in_fullres', 'pxl_col_in_fullres'])
     
     print("Creating tissue_positions_list.csv file in spatial folder.")
     hexagon_table.to_csv(folderpath +'/spatial/tissue_positions_list.csv',index=False,header=False)
 
  ############################################## ##############################################
     #if hexagon_cell_counts is empty, then skip
-    if hexagon_cell_counts == {}:
+    if hexagon_cell_counts == defaultdict(default_factory):
         print("No cell information provided. Skipping cell information files.")
     else:
         print("Creating pv_cell_hex.csv file in spatial folder.")
         with open(folderpath + '/spatial/pv_cell_hex.csv', 'w', newline='') as f:
             writer = csv.writer(f)
             for hexagon, cell_count_dict in hexagon_cell_counts.items():
                 if sum(cell_count_dict.values()) > 0:
                     hexagon_index = hexagon_names.index(hexagon)
                     for cell, count in cell_count_dict.items():
                         writer.writerow([cell, hexagon_index + 1, count])
 
  ############################################## ##############################################
-    if hexagon_quality == {}:
+    if hexagon_quality == defaultdict(default_factory):
         print("No quality information provided. Skipping quality information files.")
     else:
         print("Creating quality_per_hexagon.csv file in spatial folder.")
         with open(folderpath + '/spatial/quality_per_hexagon.csv', 'w', newline='') as f:
             writer = csv.writer(f)
             for hexagon, quality_dict in hexagon_quality.items():
-                hexagon_index = hexagon_names.index(hexagon)
-                writer.writerow([hexagon_index + 1, quality_dict["mean"], quality_dict["count"]])
+                try:
+                    hexagon_index = hexagon_names.index(hexagon)
+                    writer.writerow([hexagon_index + 1, quality_dict["mean"], quality_dict["count"]])
+                except ValueError:
+                    print(f"""One hexagon quality measurement skipped, with mean {quality_dict['mean']} and count {quality_dict['count']}, as no
+                          actual counts were found for this hexagon.""")
 
  ############################################## ##############################################
-    if probe_quality == {}:
+    if probe_quality == defaultdict(default_factory):
         print("No quality information provided. Skipping quality information files.")
     else:
         print("Creating quality_per_probe.csv file in spatial folder.")
         with open(folderpath + '/spatial/quality_per_probe.csv', 'w', newline='') as f:
             writer = csv.writer(f)
             for probe, quality_dict in probe_quality.items():
                 writer.writerow([probe, quality_dict["mean"], quality_dict["count"]])
 
-
-
-
  ############################################## ##############################################
 
-    #get all unique feature_names
-    features = list(set(feature for hexagon_counts in hexagon_counts.values() for feature in hexagon_counts))
-
+    
+    features = list(set(feature for hexagon_counts in hexagon_counts.values() for feature in hexagon_counts)) 
     # Create a list of rows with repeated features and 'Gene Expression' column
     rows = [[feature, feature, 'Gene Expression'] for feature in features]
 
     print("Creating features.tsv.gz file in spatial folder.")
     with open(folderpath + '/features.tsv', 'wt', newline='', encoding='utf-8') as f_out:
         writer = csv.writer(f_out, delimiter='\t')
         writer.writerows(rows)
@@ -740,64 +653,71 @@
     with open(folderpath + '/features.tsv', 'rb') as f_in, gzip.open(folderpath + '/features.tsv.gz', 'wb') as f_out:
         f_out.writelines(f_in)
         
 
  ############################################## ##############################################
     
 
+    # Assuming hexagon_counts is your dictionary
+    ordered_hexagon_counts = dict(sorted(hexagon_counts.items()))
+
     print("Putting together the matrix.mtx file")
     matrix_data = []
-    batch_size_n_hexagons = 500
-    hexagon_names = list(hexagon_counts.keys())  # Convert hexagon_names to a list
-    hexagon_indices = list(range(len(hexagon_names)))  # Create an array of hexagon indices
-    n_total_hexagons = len(hexagon_names)
-    n_batches = n_total_hexagons // batch_size_n_hexagons
-    n_leftover = n_total_hexagons % batch_size_n_hexagons
-
-    # Create batches of hexagon names and indices
-    hexagon_batches = [hexagon_names[i*batch_size_n_hexagons:(i+1)*batch_size_n_hexagons] for i in range(n_batches)]
-    index_batches = [hexagon_indices[i*batch_size_n_hexagons:(i+1)*batch_size_n_hexagons] for i in range(n_batches)]
-    if n_leftover > 0:
-        hexagon_batches.append(hexagon_names[-n_leftover:])
-        index_batches.append(hexagon_indices[-n_leftover:])
 
-    with ThreadPoolExecutor(max_workers=max_workers) as executor:
+    n_total_hexagons = len(ordered_hexagon_counts)
+
+    total_count = 0
+    n_processes = min(max_workers, multiprocessing.cpu_count())
+    batch_size_n_hexagons = n_total_hexagons // (n_processes * 2)
+    print(f"Using {n_processes} processes")
+    print(f"Processing {n_total_hexagons} hexagons in batches of {batch_size_n_hexagons} hexagons")
+    with concurrent.futures.ProcessPoolExecutor(max_workers=n_processes) as executor:
         futures = []
-        for hexagon_batch, index_batch in zip(hexagon_batches, index_batches):
-            future = executor.submit(hex_to_rows, hexagon_batch, index_batch, features, hexagon_counts)
+        hexagon_names = list(ordered_hexagon_counts.keys())
+        for i in range(0, n_total_hexagons, batch_size_n_hexagons):
+            hexagon_batch = hexagon_names[i:i + batch_size_n_hexagons]
+            future = executor.submit(hex_to_rows, hexagon_batch, i, features, ordered_hexagon_counts)
             futures.append(future)
 
-        with tqdm(total=len(hexagon_batches), desc="Processing batches") as pbar:
-            for future in futures:
-                matrix_data.extend(future.result())
+        with tqdm(total=len(futures), desc="Processing batches") as pbar:
+            for future in concurrent.futures.as_completed(futures):
+                batch_matrix_data = future.result()
+                matrix_data.extend(batch_matrix_data)
+                total_count += sum(row[2] for row in batch_matrix_data)
                 pbar.update(1)
+
+    print(f"Total matrix count: {total_count}")
+    unique_hexagons = len(set(hexagon_names))
+    print(f"Number of unique hexagons: {unique_hexagons}")
+    print(f"Number of hexagons in ordered_hexagon_counts: {len(ordered_hexagon_counts)}")
+
     
 
     data = np.array(matrix_data)[:, 2]
     row_indices = np.array(matrix_data)[:, 0] - 1
     col_indices = np.array(matrix_data)[:, 1] - 1
 
-    sparse_matrix = csr_matrix((data, (row_indices, col_indices)), shape=(len(features), len(barcodes)))
+    sparse_matrix = scipy.sparse.csr_matrix((data, (row_indices, col_indices)), shape=(len(features), len(barcodes)))
 
     print("Creating matrix.mtx.gz file in spatial folder.")
     with open(folderpath + '/matrix.mtx', 'wb') as f:
-        mmwrite(f, sparse_matrix, comment='metadata_json: {"software_version": "Pseudovisium", "format_version": 1}\n')
+        scipy.io.mmwrite(f, sparse_matrix, comment='metadata_json: {"software_version": "Pseudovisium", "format_version": 1}\n')
 
     with open(folderpath +'/matrix.mtx', 'rb') as f_in, gzip.open(folderpath + '/matrix.mtx.gz', 'wb') as f_out:
         f_out.writelines(f_in)
     
  ############################################## ##############################################
 
 
 
     print("Putting together the filtered_feature_bc_matrix.h5 file")
     data = np.array(matrix_data)[:, 2]
     row_indices = np.array(matrix_data)[:, 1] - 1  # Use hexagon indices for rows
     col_indices = np.array(matrix_data)[:, 0] - 1  # Use feature indices for columns
-    sparse_matrix = csr_matrix((data, (row_indices, col_indices)), shape=(len(barcodes), len(features)))
+    sparse_matrix = scipy.sparse.csr_matrix((data, (row_indices, col_indices)), shape=(len(barcodes), len(features)))
 
     # Create AnnData object from sparse matrix and barcodes/features
     adata = sc.AnnData(X=sparse_matrix, obs=pd.DataFrame(index=barcodes), var=pd.DataFrame(index=features))
 
     # Write AnnData object to 10X-formatted h5 file
     write_10X_h5(adata, folderpath + '/filtered_feature_bc_matrix.h5')
 
@@ -934,15 +854,15 @@
         #get image resolution of the hires image
         image_resolution = scalefactors["microns_per_pixel"]/scalefactors["tissue_hires_scalef"]
         #change to pixel per micron
         image_resolution = 1/image_resolution
         #tissue_pos keep barcode, pxl_row_in_fullres, pxl_col_in_fullres
         tissue_pos = tissue_pos[["barcode","pxl_row_in_fullres","pxl_col_in_fullres"]]
         # Convert the AnnData matrix to a sparse matrix (CSR format)
-        X = csr_matrix(adata.X)
+        X = scipy.sparse.csr_matrix(adata.X)
 
         # Get the row and column indices of non-zero elements
         row_indices, col_indices = X.nonzero()
 
         # Create a DataFrame with the row names, column names, and counts
         df = pd.DataFrame({
             'barcode': adata.obs_names[row_indices],
@@ -969,15 +889,15 @@
         #keep only the columns x,y
         obs = adata.obs[[x_col,y_col]]
         #rename these cols to x and y
         obs.columns = ["x","y"]
         scale = np.round(min([abs(x1 - x2) for x1 in obs["y"] for x2 in [obs["y"][500]] if x1!=x2]),3) #should be 10um
         
         obs["barcode"] = obs.index
-        X = csr_matrix(adata.X)
+        X = scipy.sparse.csr_matrix(adata.X)
 
         # Get the row and column indices of non-zero elements
         row_indices, col_indices = X.nonzero()
         genes = adata.var.index if (adata.var.index[0] != 0) and (adata.var.index[0] != "0") else adata.var[adata.var.columns[0]]
         genes = genes[col_indices]
         # Create a DataFrame with the row names, column names, and counts
         df = pd.DataFrame({
@@ -999,37 +919,36 @@
     output (str): The path to save the transcripts CSV file.
 
     Returns:
         float: The image resolution (pixels per micrometer).
     """
 
     if technology == "Visium_HD":
-        scalefactors,tissue_pos,fb_matrix = read_files(folder)
-        df,image_resolution  = anndata_to_df(fb_matrix,tissue_pos,scalefactors)
+        scalefactors,tissue_pos,fb_matrix = read_files(folder,technology)
+        df,image_resolution  = anndata_to_df(adata=fb_matrix,technology=technology,tissue_pos=tissue_pos,scalefactors=scalefactors)
         df.to_csv(output,index=False)
         return image_resolution 
     elif technology == "Curio":
         adata = read_files(folder,technology)
-        df,scale = anndata_to_df(adata,technology,x_col=x_col,y_col=y_col)
+        df,scale = anndata_to_df(adata=adata,technology=technology,x_col=x_col,y_col=y_col)
         df.to_csv(output,index=False)
         return scale
 
 
 
 
 
 ######### Main function to generate pseudovisium output ############################################################################################################
     
-def generate_pv(csv_file,img_file_path=None, hexagon_size=100, field_size_x=1000, 
-                field_size_y=1000, output_path=None, batch_size=1000000, alignment_matrix_file=None, project_name='project',
+def generate_pv(csv_file,img_file_path=None, hexagon_size=100,  output_path=None, batch_size=1000000, alignment_matrix_file=None, project_name='project',
                 image_pixels_per_um=1/0.85, tissue_hires_scalef=0.2,technology="Xenium", 
                 feature_colname="feature_name", x_colname="x_location", y_colname="y_location",
                 cell_id_colname="None", quality_colname="qv",
                 pixel_to_micron=False, max_workers=min(2, multiprocessing.cpu_count()), quality_filter=False, count_colname="NA",visium_hd_folder=None,
-                smoothing=False,quality_per_hexagon=False,quality_per_probe=False,h5_x_colname = "x", h5_y_colname = "y"):
+                smoothing=False,quality_per_hexagon=False,quality_per_probe=False,h5_x_colname = "x", h5_y_colname = "y",move_x=0,move_y=0):
     """
     generate_pv(csv_file, img_file_path=None, hexagon_size=100, field_size_x=1000, field_size_y=1000, output_path=None, 
     batch_size=1000000, alignment_matrix_file=None, project_name='project', image_pixels_per_um=1/0.85, tissue_hires_scalef=0.2, 
     technology="Xenium", feature_colname="feature_name", x_colname="x_location", y_colname="y_location", cell_id_colname="None", 
     quality_colname="qv", pixel_to_micron=False, max_workers=min(2, multiprocessing.cpu_count()), quality_filter=False, 
     count_colname="NA", visium_hd_folder=None, smoothing=False)
 
@@ -1074,38 +993,39 @@
         print("Technology is Curio. Generating transcripts.csv file from Curio files.")
         smoothing_scale = visium_hd_curio_to_transcripts(visium_hd_folder,visium_hd_folder+"/transcripts.csv",technology,x_col=h5_x_colname,y_col=h5_y_colname)
         csv_file = visium_hd_folder+"/transcripts.csv"
         print("Smoothing defaults to : {0}".format(smoothing_scale/4))
         smoothing = smoothing_scale/4
         
         # Process CSV file to generate hexagon counts and hexagon information
-    field_size = (field_size_x, field_size_y)
-    hexagon_counts, hexagons, hexagon_cell_counts, hexagon_quality, probe_quality= process_csv_file(csv_file, hexagon_size, field_size, batch_size, 
+    
+    hexagon_counts, hexagon_cell_counts, hexagon_quality, probe_quality= process_csv_file(csv_file, hexagon_size,  batch_size, 
              technology, feature_colname, x_colname, y_colname,cell_id_colname, quality_colname=quality_colname,
                max_workers=max_workers, quality_filter=quality_filter, count_colname=count_colname,smoothing=smoothing,
-               quality_per_hexagon=quality_per_hexagon,quality_per_probe=quality_per_probe,h5_x_colname=h5_x_colname,h5_y_colname=h5_y_colname)
+               quality_per_hexagon=quality_per_hexagon,quality_per_probe=quality_per_probe,h5_x_colname=h5_x_colname,h5_y_colname=h5_y_colname,move_x=move_x,move_y=move_y)
         
     # Create Pseudovisium output
-    create_pseudovisium(path=output_path,hexagon_counts=hexagon_counts,hexagon_cell_counts=hexagon_cell_counts, probe_quality=probe_quality,
-                        img_file_path=img_file_path, hexagon_quality =hexagon_quality , 
+    create_pseudovisium(path=output_path,hexagon_counts=hexagon_counts, hexagon_cell_counts=hexagon_cell_counts, probe_quality=probe_quality,
+                        img_file_path=img_file_path, hexagon_quality =hexagon_quality,
                           project_name=project_name, alignment_matrix_file=alignment_matrix_file,
                           image_pixels_per_um=image_pixels_per_um,hexagon_size=hexagon_size,
                           tissue_hires_scalef=tissue_hires_scalef,pixel_to_micron=pixel_to_micron,max_workers=max_workers)
 
     #save all arguments in a json file called arguments.json
     print("Creating arguments.json file in output path.")
     arguments = {"csv_file":csv_file,"img_file_path":img_file_path,"hexagon_size":hexagon_size,
-                    "field_size_x":field_size_x,"field_size_y":field_size_y,"output_path":output_path,
+                    "output_path":output_path,
                     "batch_size":batch_size,"alignment_matrix_file":alignment_matrix_file,"project_name":project_name,
                     "image_pixels_per_um":image_pixels_per_um,"tissue_hires_scalef":tissue_hires_scalef,
                     "technology":technology,"feature_colname":feature_colname,"x_colname":x_colname,
                     "y_colname":y_colname,"cell_id_colname":cell_id_colname,"pixel_to_micron":pixel_to_micron,
                     "quality_colname":quality_colname,"quality_filter":quality_filter,"count_colname":count_colname,
                     "smoothing":smoothing,"quality_per_hexagon":quality_per_hexagon,"quality_per_probe":quality_per_probe,
-                    "max_workers":max_workers,"visium_hd_folder":visium_hd_folder,"h5_x_colname":h5_x_colname,"h5_y_colname":h5_y_colname}
+                    "max_workers":max_workers,"visium_hd_folder":visium_hd_folder,"h5_x_colname":h5_x_colname,"h5_y_colname":h5_y_colname,
+                    "move_x":move_x,"move_y":move_y}
 
     with open(output_path + '/pseudovisium/' + project_name + '/arguments.json', 'w') as f:
         json.dump(arguments, f)
 
     end = time.time()
     print(f"Time taken: {end - start} seconds")
 
@@ -1117,16 +1037,14 @@
     main()
     The main function that parses command-line arguments and calls the generate_pv function.
     """
     parser = argparse.ArgumentParser(description="Process parameters.")
     parser.add_argument("--csv_file", "-c", type=str, help="CSV file path", default=None)
     parser.add_argument("--output_path", "-o", type=str, help="Output path", default='.')
     parser.add_argument("--hexagon_size", "-hs", type=int, help="Hexagon size", default=100)
-    parser.add_argument("--field_size_x", "-fsx", type=int, help="Field size x", default=1000)
-    parser.add_argument("--field_size_y", "-fsy", type=int, help="Field size y", default=1000)
     parser.add_argument("--img_file_path", "-i", type=str, help="Image file path", default=None)
     parser.add_argument("--alignment_matrix_file", "-am", type=str, help="Alignment matrix file path", default=None)
     parser.add_argument("--batch_size", "-b", type=int, help="Batch size", default=1000000)
     parser.add_argument("--project_name", "-p", type=str, help="Project name", default='project')
     parser.add_argument("--image_pixels_per_um", "-ppu", type=float, help="Image pixels per um", default=1/0.2125)#change!
     parser.add_argument("--tissue_hires_scalef", "-ths", type=float, help="Tissue hires scale factor", default=0.2)
     parser.add_argument("--technology", "-t", type=str, help="Technology", default="Xenium")
@@ -1141,14 +1059,16 @@
     parser.add_argument("--visium_hd_folder", "-vhf", type=str, help="Visium HD folder", default=None)
     parser.add_argument("--mw", "--max_workers", type=int, help="Max workers", default=min(2, multiprocessing.cpu_count()))
     parser.add_argument("--quality_filter", "-qf", action="store_true", help="Filter out rows with quality score less than 20")
     parser.add_argument("--quality_per_hexagon", "-qph", action="store_true", help="Calculate quality per hexagon")
     parser.add_argument("--quality_per_probe", "-qpp", action="store_true", help="Calculate quality per probe")
     parser.add_argument("--h5_x_colname", "-h5x", type=str, help="X column name in h5ad file", default="x")
     parser.add_argument("--h5_y_colname", "-h5y", type=str, help="Y column name in h5ad file", default="y")
+    parser.add_argument("--move_x","-mx", type=int, help="Move x", default=0)
+    parser.add_argument("--move_y","-my", type=int, help="Move y", default=0)
     parser.add_argument("-v", "--verbose", action="store_true", help="Print out script purpose and parameters")
     
     
     #make sure to add verbose as well
     parser.add_argument("-help", action="store_true", help="Print out script purpose and parameters")
     args = parser.parse_args()
 
@@ -1158,29 +1078,29 @@
         sys.exit(0)
 
     #print value of quality filter
     print(f"Quality filter is set to {args.quality_filter}")
     
 
     generate_pv(csv_file=args.csv_file,img_file_path=args.img_file_path,
-                hexagon_size=args.hexagon_size, field_size_x=args.field_size_x, 
-                field_size_y=args.field_size_y, output_path=args.output_path, 
+                hexagon_size=args.hexagon_size, output_path=args.output_path, 
                 batch_size=args.batch_size,
                 alignment_matrix_file=args.alignment_matrix_file, 
                 project_name=args.project_name,image_pixels_per_um=args.image_pixels_per_um, 
                 tissue_hires_scalef=args.tissue_hires_scalef,technology=args.technology, 
                 feature_colname=args.feature_colname, x_colname=args.x_colname, 
                 y_colname=args.y_colname,cell_id_colname=args.cell_id_colname,
                 pixel_to_micron=args.pixel_to_micron,max_workers=args.mw,
                 quality_colname=args.quality_colname,quality_filter=args.quality_filter,
                 count_colname=args.count_colname,
                 smoothing=args.smoothing,
                 quality_per_hexagon=args.quality_per_hexagon,
                 quality_per_probe=args.quality_per_probe,
                 h5_x_colname=args.h5_x_colname,h5_y_colname=args.h5_y_colname,
+                move_x=args.move_x,move_y=args.move_y,
                 visium_hd_folder=args.visium_hd_folder)
                 
     print("Pseudovisium output generated successfully.")
```

### Comparing `Pseudovisium-0.0.3/Pseudovisium/pseudovisium_merge.py` & `Pseudovisium-0.0.4/Pseudovisium/pseudovisium_merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 import argparse
 import json
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import geopandas as gpd
-import shapely
 from shapely.geometry import Point
-import seaborn as sns
 import matplotlib.pyplot as plt
-from io import BytesIO
-import base64
 import scipy.stats as stats
-from concurrent.futures import ProcessPoolExecutor
 from tqdm import tqdm
 import os
 import shutil
 import gzip
 import cv2
 import scanpy as sc
 import scipy.io
```

### Comparing `Pseudovisium-0.0.3/Pseudovisium/pseudovisium_qc.py` & `Pseudovisium-0.0.4/Pseudovisium/pseudovisium_qc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import argparse
 import json
 import matplotlib.pyplot as plt
 from matplotlib.patches import RegularPolygon
 import numpy as np
-import mpld3
 import pandas as pd
 from pysal.lib import weights
 from pysal.explore import esda
 import geopandas as gpd
-import shapely
-from shapely.geometry import Point
 import seaborn as sns
-import matplotlib.pyplot as plt
-from io import BytesIO
-import base64
 import scipy.stats as stats
 from concurrent.futures import ProcessPoolExecutor
 from tqdm import tqdm
 import os
 import datetime
-import matplotlib.pyplot as plt
-from matplotlib.collections import PathCollection
+import base64
+from shapely.geometry import Point
+from libpysal import weights
+from esda import Moran
 from adjustText import adjust_text
 from io import BytesIO
 import base64
 
 
-def generate_qc_report(folders, output_folder="/Users/k23030440/", gene_names=["RYR3", "AQP4", "THBS1"], include_morans_i=False,max_workers=4):
+
+def generate_qc_report(folders, output_folder="/Users/k23030440/", gene_names=["RYR3", "AQP4", "THBS1"], include_morans_i=False,max_workers=4,normalisation=False):
     #if any entry in folders lacks final /, then add
     folders = [folder if folder[-1]=="/" else folder + "/" for folder in folders]
     #same with output_folder
     output_folder = output_folder if output_folder[-1]=="/" else output_folder + "/"
 
     replicates_data = []
-    for folder in folders:
+    for folder in tqdm(folders, desc="Processing folders"):
         # Extract the dataset name from the folder path
         dataset_name = folder.split("/")[-2]
 
         # Load files
         tissue_positions_list = pd.read_csv(folder + "spatial/tissue_positions_list.csv", header=None)
         tissue_positions_list.columns = ["barcode", "in_tissue", "tissue_col", "tissue_row", "x", "y"]
         matrix = pd.read_csv(folder + "matrix.mtx", header=3, sep=" ")
@@ -115,15 +112,17 @@
         median_counts = np.median(grouped_matrix)
         cv_counts = np.std(grouped_matrix) / np.mean(grouped_matrix)
 
         grouped_matrix = matrix_joined.groupby("Barcode_ID")["Gene_ID_y"].count()
         median_features = np.median(grouped_matrix)
         cv_features = np.std(grouped_matrix) / np.mean(grouped_matrix)
 
+        number_of_probes = len(features)
         number_of_genes = len(features[~features["Gene_ID"].str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")])
+        
 
         neg_control_probes = features[features["Gene_ID"].str.contains("Probe")].index + 1
         neg_control_counts = np.sum(matrix[matrix["Gene_ID"].isin(neg_control_probes)]["Counts"])
         total_counts = np.sum(matrix["Counts"])
         prop_neg_control = neg_control_counts / total_counts
         if cell_info:
             pv_cell_hex_assigned = pv_cell_hex[(pv_cell_hex["Cell_ID"] != "UNASSIGNED") & (pv_cell_hex["Cell_ID"] != -1)]
@@ -170,21 +169,22 @@
         replicate_data = {
             "dataset_name": dataset_name,
             "metrics_table_data": {
                 "Number of hexagons with at least 100 counts": int(number_of_hex_above_100),
                 "Number of genes in at least 5% of hexagons": int(pct5_plex),
                 "Median counts per hexagon": int(median_counts),
                 "Median features per hexagon": int(median_features),
+                "Total number of probes (inc. ctrl)": int(number_of_probes),
                 "Number of genes": int(number_of_genes),
-                "Proportion of neg_control probes": np.round(prop_neg_control, 3),
+                "Proportion of neg_control probes": np.round(prop_neg_control, 5),
                 "Number of bad probes (Sum)": n_probes_not_working,
-                "Features CV": np.round(cv_features, 3),
-                "Counts CV": np.round(cv_counts, 3),
-                "Features Morans I": np.round(get_morans_i("features", matrix_joined, tissue_positions_list,max_workers=max_workers),3),
-                "Counts Morans I": np.round(get_morans_i("counts", matrix_joined, tissue_positions_list,max_workers=max_workers),3)
+                "Features CV": np.round(cv_features, 5),
+                "Counts CV": np.round(cv_counts, 5),
+                "Features Morans I": np.round(get_morans_i("features", matrix_joined, tissue_positions_list,max_workers=max_workers),5),
+                "Counts Morans I": np.round(get_morans_i("counts", matrix_joined, tissue_positions_list,max_workers=max_workers),5)
             },
             "matrix_joined": matrix_joined,
             "features": features,
             "tissue_positions_list": tissue_positions_list,
             "hexagon_size": hexagon_size,
             "image_pixels_per_um": image_pixels_per_um,
             "barcodes": barcodes,
@@ -197,38 +197,39 @@
             not_working_probes = plot_df_morans_i[plot_df_morans_i["Probe category"]=="Bad"].index.values
             n_probes_not_working = len(not_working_probes)
             #add to replicate_data metrics_table_data
             replicate_data["metrics_table_data"]["Number of bad probes (Morans I)"] = n_probes_not_working
             replicate_data["morans_i_stripplot_df"] = plot_df_morans_i
 
         if cell_info:
-            replicate_data["metrics_table_data"]["Median cells per hexagon"] = int(median_cells_per_hex)
+            replicate_data["metrics_table_data"]["Median density (cells per hexagon)"] = int(median_cells_per_hex)
             replicate_data["metrics_table_data"]["Median counts per cell"] = int(median_counts_per_cell)
-            replicate_data["metrics_table_data"]["Median pct unassigned"] = np.round(median_unassigned_pct, 3)
+            replicate_data["metrics_table_data"]["Median pct unassigned"] = np.round(median_unassigned_pct, 5)
             replicate_data["merged_assigned_unassigned"] = merged_assigned_unassigned
             replicate_data["cell_density_df"] = tissue_positions_pv_cell_hex_sum
 
-            replicate_data["metrics_table_data"]["Density CV"] = np.round(density_cv, 3)
-            replicate_data["metrics_table_data"]["Density Morans I"] = np.round(density_morans_i, 3)
+            replicate_data["metrics_table_data"]["Density (cells per hexagon) CV"] = np.round(density_cv, 5)
+            replicate_data["metrics_table_data"]["Density (cells per hexagon) Morans I"] = np.round(density_morans_i, 5)
 
         if quality_per_hexagon:
-            replicate_data["metrics_table_data"]["Pct hexagons with quality below 20"] = np.round(pct_hexagons_q_below_20, 3)
+            replicate_data["metrics_table_data"]["Pct hexagons with quality below 20"] = np.round(pct_hexagons_q_below_20, 5)
             replicate_data["hexagon_quality"] = hexagon_quality
-            replicate_data["metrics_table_data"]["Quality Morans I"] = np.round(get_morans_i("Quality", matrix_joined, tissue_positions_list,max_workers=max_workers),3)
+            replicate_data["metrics_table_data"]["Quality Morans I"] = np.round(get_morans_i("Quality", matrix_joined, tissue_positions_list,max_workers=max_workers),5)
+            replicate_data["metrics_table_data"]["Median hexagon quality"] = np.round(hexagon_quality["Quality"].median(), 5)
 
 
         if quality_per_probe:
-            replicate_data["metrics_table_data"]["Pct non-ctrl probes with quality below 20"] = np.round(pct_non_ctrl_probes_q_below_20, 3)
+            replicate_data["metrics_table_data"]["Pct non-ctrl probes with quality below 20"] = np.round(pct_non_ctrl_probes_q_below_20, 5)
             replicate_data["probe_quality"] = probe_quality
             plot_df_quality_per_probe = not_working_probe_based_on_quality(probe_quality, sample_id=dataset_name)
             replicate_data["probe_quality_stripplot_df"] = plot_df_quality_per_probe
 
         replicates_data.append(replicate_data)
 
-    html_code = generate_dashboard_html(replicates_data, gene_names, include_morans_i,quality_per_hexagon,quality_per_probe,cell_info)
+    html_code = generate_dashboard_html(replicates_data, gene_names, include_morans_i,quality_per_hexagon,quality_per_probe,cell_info,normalisation=normalisation)
 
     # Save HTML code to a file
     with open(output_folder + "metrics_dashboard.html", "w", encoding="utf-8") as html_file:
         html_file.write(html_code)
         print("HTML file generated successfully!")
     
     #in the same output folder generate a folder called pv_qc_ date
@@ -258,60 +259,332 @@
 
     #save sum of probes stripplot
     sum_stripplot = pd.concat([replicate_data["probe_sum_stripplot_df"] for replicate_data in replicates_data])
     sum_stripplot.to_csv(data_output_folder + "/sum_stripplot.csv", index=False)
 
 
 
-def generate_dashboard_html(replicates_data, gene_names, include_morans_i,quality_per_hexagon,quality_per_probe,cell_info):
+def generate_dashboard_html(replicates_data, gene_names, include_morans_i,quality_per_hexagon,quality_per_probe,cell_info,normalisation=False):
     metrics_html = """
         <div id="metric-details">
+            <h2>Counts Table</h2>
             <table>
                 <thead>
                     <tr>
                         <th>Metric</th>
     """
     for replicate_data in replicates_data:
         metrics_html += f"""
                         <th>{replicate_data['dataset_name']}</th>
         """
     metrics_html += """
                     </tr>
                 </thead>
                 <tbody>
+                    <tr>
+                        <td>Median counts per hexagon</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Median counts per hexagon']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Number of hexagons with at least 100 counts</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Number of hexagons with at least 100 counts']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Proportion of neg_control probes</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Proportion of neg_control probes']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Counts Morans I</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Counts Morans I']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Counts CV</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Counts CV']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                </tbody>
+            </table>
+
+            <h2>Features Table</h2>
+            <table>
+                <thead>
+                    <tr>
+                        <th>Metric</th>
     """
-    for metric in replicates_data[0]['metrics_table_data']:
+    for replicate_data in replicates_data:
         metrics_html += f"""
+                        <th>{replicate_data['dataset_name']}</th>
+        """
+    metrics_html += """
+                    </tr>
+                </thead>
+                <tbody>
                     <tr>
-                        <td>{metric}</td>
+                        <td>Total number of probes (inc. ctrl)</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Total number of probes (inc. ctrl)']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Number of genes</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Number of genes']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Median features per hexagon</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Median features per hexagon']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Number of genes in at least 5% of hexagons</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Number of genes in at least 5% of hexagons']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Features Morans I</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Features Morans I']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Features CV</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Features CV']}</td>
+        """
+    metrics_html += """
+                    </tr>
+                </tbody>
+            </table>
+
+            <h2>Uninformative Probes Table</h2>
+            <table>
+                <thead>
+                    <tr>
+                        <th>Metric</th>
+    """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <th>{replicate_data['dataset_name']}</th>
+        """
+    metrics_html += """
+                    </tr>
+                </thead>
+                <tbody>
+                    <tr>
+                        <td>Number of bad probes (Sum)</td>
+        """
+    for replicate_data in replicates_data:
+        metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data']['Number of bad probes (Sum)']}</td>
+        """
+    metrics_html += """
+                    </tr>
+    """
+    if include_morans_i:
+        metrics_html += """
+                    <tr>
+                        <td>Number of bad probes (Morans I)</td>
         """
         for replicate_data in replicates_data:
             metrics_html += f"""
-                        <td>{replicate_data['metrics_table_data'][metric]}</td>
+                        <td>{replicate_data['metrics_table_data'].get('Number of bad probes (Morans I)', 'N/A')}</td>
             """
         metrics_html += """
                     </tr>
         """
     metrics_html += """
                 </tbody>
             </table>
+    """
+
+    if cell_info:
+        metrics_html += """
+            <h2>Cell Info Table</h2>
+            <table>
+                <thead>
+                    <tr>
+                        <th>Metric</th>
+        """
+        for replicate_data in replicates_data:
+            metrics_html += f"""
+                        <th>{replicate_data['dataset_name']}</th>
+            """
+        metrics_html += """
+                    </tr>
+                </thead>
+                <tbody>
+                    <tr>
+                        <td>Median counts per cell</td>
+        """
+        for replicate_data in replicates_data:
+            metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data'].get('Median counts per cell', 'N/A')}</td>
+            """
+        metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Median pct unassigned</td>
+        """
+        for replicate_data in replicates_data:
+            metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data'].get('Median pct unassigned', 'N/A')}</td>
+            """
+        metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Median density (cells per hexagon)</td>
+        """
+        for replicate_data in replicates_data:
+            metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data'].get('Median density (cells per hexagon)', 'N/A')}</td>
+            """
+        metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Density (cells per hexagon) CV</td>
+        """
+        for replicate_data in replicates_data:
+            metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data'].get('Density (cells per hexagon) CV', 'N/A')}</td>
+            """
+        metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Density (cells per hexagon) Morans I</td>
+        """
+        for replicate_data in replicates_data:
+            metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data'].get('Density (cells per hexagon) Morans I', 'N/A')}</td>
+            """
+        metrics_html += """
+                    </tr>
+                </tbody>
+            </table>
+        """
+
+    if quality_per_hexagon:
+        metrics_html += """
+            <h2>Quality Table</h2>
+            <table>
+                <thead>
+                    <tr>
+                        <th>Metric</th>
+        """
+        for replicate_data in replicates_data:
+            metrics_html += f"""
+                        <th>{replicate_data['dataset_name']}</th>
+            """
+        metrics_html += """
+                    </tr>
+                </thead>
+                <tbody>
+                    <tr>
+                        <td>Median hexagon quality</td>
+        """
+        for replicate_data in replicates_data:
+            metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data'].get('Median hexagon quality', 'N/A')}</td>
+            """
+        metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Quality Morans I</td>
+        """
+        for replicate_data in replicates_data:
+            metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data'].get('Quality Morans I', 'N/A')}</td>
+            """
+        metrics_html += """
+                    </tr>
+                    <tr>
+                        <td>Pct hexagons with quality below 20</td>
+        """
+        for replicate_data in replicates_data:
+            metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data'].get('Pct hexagons with quality below 20', 'N/A')}</td>
+            """
+        metrics_html += """
+                    </tr>
+        """
+        if quality_per_probe:
+            metrics_html += """
+                    <tr>
+                        <td>Pct non-ctrl probes with quality below 20</td>
+            """
+            for replicate_data in replicates_data:
+                metrics_html += f"""
+                        <td>{replicate_data['metrics_table_data'].get('Pct non-ctrl probes with quality below 20', 'N/A')}</td>
+                """
+            metrics_html += """
+                    </tr>
+            """
+        metrics_html += """
+                </tbody>
+            </table>
+        """
+
+    metrics_html += """
         </div>
     """
 
     hexagon_plots_html = ""
     for i, gene_name in enumerate(gene_names):
         if i % 3 == 0:
             hexagon_plots_html += f"""
             <div class="row">
             """
         gene_found = False
         for replicate_data in replicates_data:
             if gene_name in replicate_data['features']['Gene_Name'].tolist():
                 gene_found = True
-                hexagon_df = get_df_for_gene(replicate_data['matrix_joined'], replicate_data['tissue_positions_list'], gene_name)
+                hexagon_df = get_df_for_gene(replicate_data['matrix_joined'], replicate_data['tissue_positions_list'], gene_name,normalisation)
                 hexagon_html = hexagon_plot_to_html(hexagon_df, replicate_data['hexagon_size'], replicate_data['image_pixels_per_um'], gene_name, replicate_data['dataset_name'])
                 hexagon_plots_html += f"""
                 <div class="col">
                     {hexagon_html}
                 </div>
                 """
             else:
@@ -355,15 +628,15 @@
         cell_density_hexagon_plots_html = ""
         for i, replicate_data in enumerate(replicates_data):
             if i % 3 == 0:
                 cell_density_hexagon_plots_html += f"""
                 <div class="row">
                 """
             cell_density_df= replicate_data["cell_density_df"]
-            hexagon_html = hexagon_plot_to_html(cell_density_df, replicate_data['hexagon_size'], replicate_data['image_pixels_per_um'], "Density", replicate_data['dataset_name'],replicate_data['metrics_table_data']["Density Morans I"])
+            hexagon_html = hexagon_plot_to_html(cell_density_df, replicate_data['hexagon_size'], replicate_data['image_pixels_per_um'], "Density", replicate_data['dataset_name'],replicate_data['metrics_table_data']["Density (cells per hexagon) Morans I"])
             cell_density_hexagon_plots_html += f"""
             <div class="col">
                 <h3>{replicate_data['dataset_name']}</h3>
                 {hexagon_html}
             </div>
             """
             if (i + 1) % 3 == 0 or i == len(replicates_data) - 1:
@@ -526,22 +799,24 @@
         <style>
             body {{
                 font-family: Arial, sans-serif;
             }}
             table {{
                 border-collapse: collapse;
                 width: 100%;
+                font-size: 12px;
             }}
             th, td {{
-                padding: 8px;
+                padding: 6px;
                 text-align: left;
                 border-bottom: 1px solid #ddd;
             }}
             th {{
                 background-color: #f2f2f2;
+                white-space: nowrap;
             }}
             .row {{
                 display: flex;
                 flex-wrap: wrap;
                 margin: 0 -20px;
             }}
             .col {{
@@ -559,26 +834,26 @@
         <h1 style="text-align:center;">Pseudovisium QC</h1>
         <p style="text-align:center;">Written by Bence Kover (2024)</p>
         <div class="container">
             <div class="dropdown">
                 <label for="metrics-select">Select Metric:</label>
                 <select id="metrics-select">
                     <option value="table">Table of Key Metrics</option>
-                    <option value="plot">Hexagon Plots</option>
-                    <option value="sums-comparison">Sums Comparison</option>
                     <option value="abundance-correlation-heatmap">Abundance Correlation Heatmap</option>
-                    {'<option value="morans-i-heatmap">Morans I Heatmap</option>' if include_morans_i else ""}
+                    <option value="sums-comparison">Abundance Comparison</option>
+                    <option value="sums-i-stripplot">Abundance Stripplot</option>
+                    {'<option value="morans-i-heatmap">Morans I Correlation Heatmap</option>' if include_morans_i else ""}
+                    {'<option value="morans-i-comparison">Morans I Comparison</option>' if include_morans_i else ""}
                     {'<option value="morans-i-stripplot">Morans I Stripplot</option>' if include_morans_i else ""}
-                    <option value="sums-i-stripplot">Sums I Stripplot</option>
-                    <option value="nfeature_hexagon_plots">nFeature hexagon plots</option>
-                    {'<option value="quality_hexagon_plots">Quality hexagon plots</option>' if quality_per_hexagon else ""}
-                    <option value="total_hexagon_plots">Total hexagon plots</option>
-                    {'<option value="morans-i-comparison">Pairwise Morans I Plots</option>' if include_morans_i else ""}
-                    {'<option value="probe_quality_stripplot">Probe Quality Stripplot</option>' if quality_per_probe else ""}
+                    <option value="plot">Hexagon Plots for Genes of Interest</option>
+                    <option value="nfeature_hexagon_plots">Number of Features per Hexagon Plots</option>
+                    <option value="total_hexagon_plots">Total Hexagon Plots</option>
                     {'<option value="cell_density_hexagon_plots">Cell Density Hexagon Plots</option>' if cell_info else ""}
+                    {'<option value="quality_hexagon_plots">Quality Hexagon Plots</option>' if quality_per_hexagon else ""}
+                    {'<option value="probe_quality_stripplot">Probe Quality Stripplot</option>' if quality_per_probe else ""}
                 </select>
             </div>
             <div id="metric-details-container">
                 {metrics_html}
             </div>
             <div id="plot" class="plot-container">
                 {hexagon_plots_html}
@@ -689,16 +964,16 @@
     """
     return html_code
 
 
 def not_working_probe_based_on_sum(matrix_joined,sample_id="Sample1"):
     grouped_matrix = matrix_joined.groupby("Gene_ID_y")["Counts"].sum()
     #where index has control|blank|Control|Blank|BLANK in it
-    grouped_matrix_neg_probes = grouped_matrix[grouped_matrix.index.str.contains("control|blank|Control|Blank|BLANK")]
-    grouped_matrix_true_probes = grouped_matrix[~grouped_matrix.index.str.contains("control|blank|Control|Blank|BLANK")]     
+    grouped_matrix_neg_probes = grouped_matrix[grouped_matrix.index.str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
+    grouped_matrix_true_probes = grouped_matrix[~grouped_matrix.index.str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]     
 
     #create a plot_df that is grouped_matrix and a column specifying whether the gene is a neg control or not
     plot_df = pd.DataFrame(grouped_matrix)
     plot_df["Probe category"] = [1 if gene in grouped_matrix_neg_probes.index.values else 0 for gene in plot_df.index.values]
     plot_df["gene"] = plot_df.index.values
     plot_df["log_counts"] = np.log10(plot_df["Counts"])
 
@@ -718,19 +993,15 @@
     plot_df["Sample"] = sample_id
     #order based on probe category
     plot_df = plot_df.sort_values("Probe category")
     return plot_df
 
 
 
-import numpy as np
-import matplotlib.pyplot as plt
-from adjustText import adjust_text
-from io import BytesIO
-import base64
+
 
 
 def probe_stripplot(plot_df, col_to_plot="log_counts", sample_id="Sample 1", legend=False):
     fig, ax = plt.subplots(figsize=(2, 2.5))
     # Define jitter amount
     jitter = 0.1
 
@@ -744,15 +1015,15 @@
         y = row[col_to_plot]
         points["x"].append(x)
         points["y"].append(y)
         points["cat"].append(cat)
         points["index"].append(index)
 
     # Plot the points for each category
-    for cat in ["Neg_control", "Good", "Bad"]:
+    for cat in [ "Good", "Bad","Neg_control"]:
         mask = [c == cat for c in points["cat"]]
         ax.scatter([x for x, m in zip(points["x"], mask) if m],
                    [y for y, m in zip(points["y"], mask) if m],
                    alpha=0.8, label=cat)
 
     # Draw a straight line at the mean of the neg controls
     neg_control_mean = np.mean(plot_df[plot_df["Probe category"] == "Neg_control"][col_to_plot])
@@ -787,16 +1058,16 @@
     img_str = base64.b64encode(img_buffer.getvalue()).decode()
     html_fig = f'<img src="data:image/png;base64,{img_str}"/>'
 
     plt.close(fig)
     return html_fig
 
 def not_working_probe_based_on_quality(probe_quality, sample_id="Sample1"):
-    probe_quality_neg_probes = probe_quality[probe_quality["Probe_ID"].str.contains("control|blank|Control|Blank|BLANK")]
-    probe_quality_true_probes = probe_quality[~probe_quality["Probe_ID"].str.contains("control|blank|Control|Blank|BLANK")]
+    probe_quality_neg_probes = probe_quality[probe_quality["Probe_ID"].str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
+    probe_quality_true_probes = probe_quality[~probe_quality["Probe_ID"].str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
     plot_df = probe_quality.reset_index(drop=True)
     plot_df["Probe category"] = [1 if gene in probe_quality_neg_probes.Probe_ID.values else 0 for gene in plot_df.Probe_ID.values]
 
     #iterate through the true probes and see whether they are significantly outside of the distribution of the neg probes
     for gene in probe_quality_true_probes.Probe_ID.values:
         plot_df_gene_index = plot_df[plot_df["Probe_ID"]==gene].index[0]
         quality = plot_df[plot_df["Probe_ID"]==gene]["Quality"]
@@ -813,34 +1084,37 @@
     plot_df = plot_df.sort_values("Probe category")
     return plot_df
 
 
 
 
 def not_working_probe_based_on_morans_i(morans_table, sample_id="Sample1"):
-    morans_table_neg_probes = morans_table[morans_table.gene.str.contains("control|blank|Control|Blank|BLANK")]
-    morans_table_true_probes = morans_table[~morans_table.gene.str.contains("control|blank|Control|Blank|BLANK")]     
+    
+    morans_table_neg_probes = morans_table[morans_table.gene.str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
+    morans_table_true_probes = morans_table[~morans_table.gene.str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]     
 
     #create a plot_df that is grouped_matrix and a column specifying whether the gene is a neg control or not
     plot_df = morans_table.reset_index(drop=True)
     plot_df["Probe category"] = [1 if gene in morans_table_neg_probes.gene.values else 0 for gene in plot_df.gene.values]
 
+    neg_probes_morans_i_s = plot_df[plot_df["Probe category"]==1]["Morans_I"]
+    mean = np.mean(neg_probes_morans_i_s)
+    std = np.std(neg_probes_morans_i_s)
+
     #iterate through the true probes and see whether they are significantly outside of the distribution of the neg probes
     for gene in morans_table_true_probes.gene.values:
         plot_df_gene_index = plot_df[plot_df["gene"]==gene].index[0]
         morans_i_s = plot_df[plot_df["gene"]==gene]["Morans_I"]
-        neg_probes_morans_i_s = plot_df[plot_df["Probe category"]==1]["Morans_I"]
-        mean = np.mean(neg_probes_morans_i_s)
-        std = np.std(neg_probes_morans_i_s)
         p_val = stats.norm.cdf(morans_i_s, loc=mean, scale=std)
         p_val = 1-p_val
         if p_val*len(morans_table_true_probes)<0.05:
             plot_df.loc[plot_df_gene_index,"Probe category"] = 2
+    
     #save the name of those genes with 0
-    plot_df["Probe category"] = ["Neg_control" if x==1 else "Bad" if x==0 else "Good" for x in plot_df["Probe category"]]
+    plot_df["Probe category"] = ["Neg_control" if x==1 else "Good" if x==2 else "Bad" for x in plot_df["Probe category"]]
     plot_df["Sample"] = sample_id
     plot_df = plot_df.sort_values("Probe category")
     return plot_df
 
 
 
 def get_unique_features_per_hexagon(matrix_joined):
@@ -858,21 +1132,14 @@
     hexagon_quality = matrix_joined.groupby("Barcode_ID").agg({"Quality":"first","x":"first","y":"first"})
     hexagon_quality = hexagon_quality.reset_index()
     #rename Quality to counts
     hexagon_quality = hexagon_quality.rename(columns={"Quality": "counts"})
     return hexagon_quality
 
 
-from shapely.geometry import Point
-import geopandas as gpd
-from libpysal import weights
-from esda import Moran
-import numpy as np
-import pandas as pd
-
 # Functions used in generate_qc_report
 def get_df_for_gene(matrix_joined, tissue_positions_list, gene_name, normalised=False):
     matrix_subset = matrix_joined[matrix_joined["Gene_ID_y"] == gene_name]
     matrix_subset.reset_index(drop=True, inplace=True)
     x = tissue_positions_list["x"]
     y = tissue_positions_list["y"]
     counts = np.zeros(len(tissue_positions_list))
@@ -892,14 +1159,15 @@
 
 
 
 def hexagon_plot_to_html(hexagon_df, hexagon_size, image_pixels_per_um, gene_name, dataset_name,morans_i=None):
     fig, ax = plt.subplots(figsize=(3, 2.5))
     sc = ax.scatter(hexagon_df["x"], hexagon_df["y"], c=hexagon_df["counts"], cmap="viridis", s=2, alpha=0.6)
     for hx, hy in zip(hexagon_df["x"], hexagon_df["y"]):
+        #Double check this and why there is the 0.865 division
         hexagon = RegularPolygon((hx, hy), numVertices=6, radius=hexagon_size * image_pixels_per_um / 0.865, alpha=0.2, edgecolor='k', orientation=np.pi / 2)
         ax.add_patch(hexagon)
     ax.set_xlim(0, max(hexagon_df["x"]))
     ax.set_ylim(0, max(hexagon_df["y"]))
     aspect = hexagon_df["x"].max() / hexagon_df["y"].max()
     ax.set_aspect(aspect)
     ax.set_xticks([])
@@ -961,22 +1229,22 @@
 
         sums_df = pd.merge(sums1, sums2, on="Gene_ID_y", suffixes=("_1", "_2"))
         fig, ax = plt.subplots(figsize=(4, 4))
         ax.scatter(sums_df["Counts_1"], sums_df["Counts_2"], alpha=0.3, s=20)
         ax.set_xlabel(f"Log10 Total expression {dataset1_name}", fontsize=8)
         ax.set_ylabel(f"Log10 Total expression {dataset2_name}", fontsize=8)
         ax.set_title(f"{dataset1_name} vs {dataset2_name}", fontsize=10)
-        corr = sums_df["Counts_1"].corr(sums_df["Counts_2"])
-        ax.text(np.quantile(sums_df["Counts_1"], 0.3), np.quantile(sums_df["Counts_2"], 0.95),
-                f"Pearson correlation: {corr:.2f}", fontsize=8)
 
         sums_df["diff"] = np.abs(sums_df["Counts_1"] - sums_df["Counts_2"])
         sums_df = sums_df.sort_values("diff", ascending=False)
 
-        texts = []
+        corr = sums_df["Counts_1"].corr(sums_df["Counts_2"])
+        corr_text = ax.text(np.quantile(sums_df["Counts_1"], 0.3), np.quantile(sums_df["Counts_2"], 0.95),
+                            f"Pearson correlation: {corr:.2f}", fontsize=8)
+        texts = [corr_text]
         for i in range(10):
             x = sums_df["Counts_1"].iloc[i]
             y = sums_df["Counts_2"].iloc[i]
             txt = sums_df["Gene_ID_y"].iloc[i]
             texts.append(ax.text(x, y, txt, fontsize=10))
 
         adjust_text(texts, arrowprops=dict(arrowstyle="-", color='black', lw=0.5))
@@ -1004,32 +1272,32 @@
     
     corr_matrix = pd.DataFrame(index=replicate_names, columns=replicate_names, dtype=float)
     min_common_probes = 20
     for i in range(len(sums_data)):
         for j in range(i + 1, len(sums_data)):
             common_probes = list(set(sums_data[i]["Gene_ID_y"]) & set(sums_data[j]["Gene_ID_y"]))
             if len(common_probes) >= min_common_probes:
-                #filter dataframes only for common probes then reorder them to have the same order
-                sums_data[i] = sums_data[i][sums_data[i]["Gene_ID_y"].isin(common_probes)]
-                sums_data[j] = sums_data[j][sums_data[j]["Gene_ID_y"].isin(common_probes)]
-                sums_data[i].sort_values("Gene_ID_y", inplace=True)
-                sums_data[j].sort_values("Gene_ID_y", inplace=True)
-                corr = sums_data[i]["Counts"].corr(sums_data[j]["Counts"])
-                corr=round(corr,3)
+                # Filter dataframes only for common probes then reorder them to have the same order
+                sums1 = sums_data[i][sums_data[i]["Gene_ID_y"].isin(common_probes)]
+                sums2 = sums_data[j][sums_data[j]["Gene_ID_y"].isin(common_probes)]
+                sums1 = sums1.sort_values("Gene_ID_y")
+                sums2 = sums2.sort_values("Gene_ID_y")
+                sums_df = pd.merge(sums1, sums2, on="Gene_ID_y", suffixes=("_1", "_2"))
+                corr = sums_df["Counts_1"].corr(sums_df["Counts_2"])
+                corr = round(corr, 3)
                 corr_matrix.iloc[i, j] = corr
                 corr_matrix.iloc[j, i] = corr
             else:
                 corr_matrix.iloc[i, j] = 0.0
                 corr_matrix.iloc[j, i] = 0.0
             
-    #make diagonal 1
+    # Make diagonal 1
     np.fill_diagonal(corr_matrix.values, 1)
     
     fig_dimension = len(replicates_data)
-
     clustermap = sns.clustermap(corr_matrix, cmap='coolwarm', annot=True, fmt='.2f', figsize=(fig_dimension, fig_dimension))
 
     # Convert the plot to HTML
     img_buffer = BytesIO()
     clustermap.savefig(img_buffer, format='png')
     img_str = base64.b64encode(img_buffer.getvalue()).decode()
     html_fig = f'<img src="data:image/png;base64,{img_str}"/>'
@@ -1059,120 +1327,127 @@
     return df.sort_values("counts", ascending=False).drop_duplicates(subset=["x", "y"])
 
 
 def process_gene(gene, matrix_joined, tissue_positions_list):
     gene_df = get_df_for_gene(matrix_joined, tissue_positions_list, gene, normalised=True)
     points = [Point(xy) for xy in zip(gene_df['x'], gene_df['y'])]
     gene_gdf = gpd.GeoDataFrame(gene_df, geometry=points)
-    w = weights.KNN.from_dataframe(gene_gdf, k=6)
+    w = weights.KNN.from_dataframe(gene_gdf, k=18)
     w.transform = 'R'
     mi = Moran(gene_df["counts"], w, permutations=0)
     return {"gene": gene, "Morans_I": mi.I}
 
 def get_morans_i(gene_name, matrix_joined, tissue_positions_list, max_workers=4):
     if gene_name == "all":
         unique_genes = matrix_joined["Gene_ID_y"].unique()
         #remove those unique genes which have less than total 100 counts
-        lowly_expressed_genes = matrix_joined.groupby("Gene_ID_y")["Counts"].sum()
-        lowly_expressed_genes = lowly_expressed_genes[lowly_expressed_genes<100].index.values
-        unique_genes = [gene for gene in unique_genes if gene not in lowly_expressed_genes]
+        #lowly_expressed_genes = matrix_joined.groupby("Gene_ID_y")["Counts"].sum()
+        #lowly_expressed_genes = lowly_expressed_genes[lowly_expressed_genes<100].index.values
+        unique_genes = [gene for gene in unique_genes] #if gene not in lowly_expressed_genes]
         with ProcessPoolExecutor(max_workers=max_workers) as executor:
             results = list(tqdm(executor.map(process_gene, unique_genes, [matrix_joined]*len(unique_genes), [tissue_positions_list]*len(unique_genes)), total=len(unique_genes), desc="Processing genes"))
         
         res_df = pd.DataFrame(results)
         #append the lowly expressed genes to the end of the dataframe with a morans i of 0
-        res_df = pd.concat([res_df,pd.DataFrame({"gene":lowly_expressed_genes,"Morans_I":0})],axis=0)
+        #res_df = pd.concat([res_df,pd.DataFrame({"gene":lowly_expressed_genes,"Morans_I":0})],axis=0)
         
         return res_df
     
     elif gene_name == "features":
         mat = matrix_joined.groupby("Barcode_ID").count()
         mat["x"] = mat.index.to_series().apply(lambda barcode: matrix_joined[matrix_joined["Barcode_ID"]==barcode]["x"].values[0])
         mat["y"] = mat.index.to_series().apply(lambda barcode: matrix_joined[matrix_joined["Barcode_ID"]==barcode]["y"].values[0])
         points = [Point(xy) for xy in zip(mat['x'], mat['y'])]
         gene_gdf = gpd.GeoDataFrame(mat, geometry=points)
-        w = weights.KNN.from_dataframe(gene_gdf, k=6)
+        w = weights.KNN.from_dataframe(gene_gdf, k=18)
         w.transform = 'R'
         mi = esda.Moran(mat["Gene_ID_y"], w, permutations=0)
         return mi.I
     
     elif gene_name == "density":
         mat = matrix_joined.copy()
         points = [Point(xy) for xy in zip(mat['x'], mat['y'])]
         gene_gdf = gpd.GeoDataFrame(mat, geometry=points)
-        w = weights.KNN.from_dataframe(gene_gdf, k=6)
+        w = weights.KNN.from_dataframe(gene_gdf, k=18)
         w.transform = 'R'
         mi = esda.Moran(mat["counts"], w, permutations=0)
         return mi.I
     
     elif gene_name == "counts":
         mat = matrix_joined.groupby("Barcode_ID").sum()
         mat["x"] = mat.index.to_series().apply(lambda barcode: matrix_joined[matrix_joined["Barcode_ID"]==barcode]["x"].values[0])
         mat["y"] = mat.index.to_series().apply(lambda barcode: matrix_joined[matrix_joined["Barcode_ID"]==barcode]["y"].values[0])
         points = [Point(xy) for xy in zip(mat['x'], mat['y'])]
         gene_gdf = gpd.GeoDataFrame(mat, geometry=points)
-        w = weights.KNN.from_dataframe(gene_gdf, k=6)
+        w = weights.KNN.from_dataframe(gene_gdf, k=18)
         w.transform = 'R'
         mi = esda.Moran(mat["Counts"], w, permutations=0)
         return mi.I
 
     elif gene_name == "Quality":
         mat = matrix_joined.groupby("Barcode_ID").agg({"Quality":"mean"})
         mat["x"] = mat.index.to_series().apply(lambda barcode: matrix_joined[matrix_joined["Barcode_ID"]==barcode]["x"].values[0])
         mat["y"] = mat.index.to_series().apply(lambda barcode: matrix_joined[matrix_joined["Barcode_ID"]==barcode]["y"].values[0])
         points = [Point(xy) for xy in zip(mat['x'], mat['y'])]
         gene_gdf = gpd.GeoDataFrame(mat, geometry=points)
-        w = weights.KNN.from_dataframe(gene_gdf, k=6)
+        w = weights.KNN.from_dataframe(gene_gdf, k=18)
         w.transform = 'R'
         mi = esda.Moran(mat["Quality"], w, permutations=0)
         return mi.I
     
     else:
         gene_df = get_df_for_gene(matrix_joined, tissue_positions_list, gene_name, normalised=True)
         points = [Point(xy) for xy in zip(gene_df['x'], gene_df['y'])]
         gene_gdf = gpd.GeoDataFrame(gene_df, geometry=points)
-        w = weights.KNN.from_dataframe(gene_gdf, k=6)
+        w = weights.KNN.from_dataframe(gene_gdf, k=18)
         w.transform = 'R'
         mi = esda.Moran(gene_df["counts"], w, permutations=0)
         return mi.I
 
 
 
 def plot_morans_i_to_html(morans_i1, morans_i2, dataset1_name, dataset2_name):
     common_probes = list(set(morans_i1["gene"]) & set(morans_i2["gene"]))
-    #print length of common_probes "in scatter plot"
-    print("In scatterplot, number of common probes: ",len(common_probes))
     if len(common_probes) < 20:
         fig, ax = plt.subplots(figsize=(4, 4))
         ax.text(0.5, 0.5, "Not enough overlapping probes", fontsize=12, ha='center')
         ax.axis('off')
 
         # Convert the plot to HTML
         img_buffer = BytesIO()
         fig.savefig(img_buffer, format='png')
         img_str = base64.b64encode(img_buffer.getvalue()).decode()
         html_fig = f'<img src="data:image/png;base64,{img_str}"/>'
-        
+
         plt.close(fig)  # Close the plot to free memory
 
         return html_fig
     else:
         morans_i_df = pd.merge(morans_i1, morans_i2, on="gene", suffixes=("_1", "_2"))
         morans_i_df = morans_i_df[morans_i_df["gene"].isin(common_probes)]
         fig, ax = plt.subplots(figsize=(4, 4))
         ax.scatter(morans_i_df["Morans_I_1"], morans_i_df["Morans_I_2"], alpha=0.3, s=20)
         ax.set_xlabel(f"Moran's I {dataset1_name}", fontsize=8)
         ax.set_ylabel(f"Moran's I {dataset2_name}", fontsize=8)
         ax.set_title(f"{dataset1_name} vs {dataset2_name}", fontsize=10)
-        corr = morans_i_df["Morans_I_1"].corr(morans_i_df["Morans_I_2"])
-        ax.text(0.5, 0.1, f"Pearson correlation: {corr:.2f}", fontsize=8, ha='center')
+
         morans_i_df["diff"] = np.abs(morans_i_df["Morans_I_1"] - morans_i_df["Morans_I_2"])
         morans_i_df = morans_i_df.sort_values("diff", ascending=False)
+
+        corr = morans_i_df["Morans_I_1"].corr(morans_i_df["Morans_I_2"])
+        corr_text = ax.text(0.5, 0.1, f"Pearson correlation: {corr:.2f}", fontsize=8, ha='center')
+
+        texts = [corr_text]
         for i in range(10):
-            ax.text(morans_i_df["Morans_I_1"].iloc[i], morans_i_df["Morans_I_2"].iloc[i], morans_i_df["gene"].iloc[i], fontsize=10)
+            x = morans_i_df["Morans_I_1"].iloc[i]
+            y = morans_i_df["Morans_I_2"].iloc[i]
+            txt = morans_i_df["gene"].iloc[i]
+            texts.append(ax.text(x, y, txt, fontsize=10))
+
+        adjust_text(texts, arrowprops=dict(arrowstyle="-", color='black', lw=0.5))
 
         # Convert the plot to HTML
         img_buffer = BytesIO()
         fig.savefig(img_buffer, format='png')
         img_str = base64.b64encode(img_buffer.getvalue()).decode()
         html_fig = f'<img src="data:image/png;base64,{img_str}"/>'
 
@@ -1191,30 +1466,28 @@
         replicate_names.append(replicate_data['dataset_name'])
     
     corr_matrix = pd.DataFrame(index=replicate_names, columns=replicate_names, dtype=float)
     min_common_probes = 20
     for i in range(len(morans_i_data)):
         for j in range(i + 1, len(morans_i_data)):
             common_probes = list(set(morans_i_data[i]["gene"]) & set(morans_i_data[j]["gene"]))
-            print("In heatmap, number of common probes: ",len(common_probes))
             if len(common_probes) >= min_common_probes:
                 #filter dataframes only for common probes then reorder them to have the same order
                 morans_i_df = pd.merge(morans_i_data[i], morans_i_data[j], on="gene", suffixes=("_1", "_2"))
                 morans_i_df = morans_i_df[morans_i_df["gene"].isin(common_probes)]
                 corr = morans_i_df["Morans_I_1"].corr(morans_i_df["Morans_I_2"])
                 corr=round(corr,3)
                 corr_matrix.iloc[i, j] = corr
                 corr_matrix.iloc[j, i] = corr
             else:
                 corr_matrix.iloc[i, j] = 0.0
                 corr_matrix.iloc[j, i] = 0.0
 
     #make diagonal 1
     np.fill_diagonal(corr_matrix.values, 1)
-    print(corr_matrix)
     fig_dimension = len(replicates_data) 
     clustermap = sns.clustermap(corr_matrix, cmap='coolwarm', annot=True, fmt='.2f', figsize=(fig_dimension, fig_dimension))
 
     # Convert the plot to HTML
     img_buffer = BytesIO()
     clustermap.savefig(img_buffer, format='png')
     img_str = base64.b64encode(img_buffer.getvalue()).decode()
@@ -1228,14 +1501,16 @@
 def main():
     parser = argparse.ArgumentParser(description="Generate QC report for Pseudovisium output.")
     parser.add_argument("--folders", "-f", nargs="+", help="List of folders containing Pseudovisium output", required=True)
     parser.add_argument("--output_folder", "-o", default="/Users/k23030440/", help="Output folder path")
     parser.add_argument("--gene_names", "-g", nargs="+", default=["RYR3", "AQP4", "THBS1"], help="List of gene names to plot")
     parser.add_argument("--include_morans_i", "-m", action="store_true", help="Include Moran's I features tab")
     parser.add_argument("-max_workers", "--mw", type=int, default=4, help="Number of workers to use for parallel processing")
+    parser.add_argument("-normalisation","--n",action="store_true",help="Normalise the counts by the total counts per cell")
+
     args = parser.parse_args()
 
-    generate_qc_report(args.folders, args.output_folder, args.gene_names, args.include_morans_i, max_workers=args.mw)
+    generate_qc_report(args.folders, args.output_folder, args.gene_names, args.include_morans_i, max_workers=args.mw,normalisation=args.n)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `Pseudovisium-0.0.3/Pseudovisium.egg-info/PKG-INFO` & `Pseudovisium-0.0.4/Pseudovisium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pseudovisium
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for hexagonal binning of high-resolution spatial transcriptomic data
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: spatial,transcriptomics,visium,xenium,cosmx
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Pseudovisium-0.0.3/README.md` & `Pseudovisium-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 # 🛑 Pseudovisium
-Pseudovisium is a powerful Python software package designed to streamline the processing and analysis of imaging-based spatial transcriptomics data. By leveraging hexagonal binning, Pseudovisium enables efficient compression and visualization of spatial data, making it easier to extract meaningful insights from your experiments.
+Pseudovisium is a Python software package designed to democratize the analysis of spatial transcriptomics data. By leveraging hexagonal binning, Pseudovisium enables efficient compression and visualization of spatial data, making exploratory analysis and quality control faster and more memory efficient. The goal of this tool is not to increase accuracy, but to make spatial data analysis more accessible, regardless of computing environment. Additionally, this package facilitates simulating low-res/Visium spatial experiments both for practical (e.g. experimental design) and theoretical (e.g. studying the impact of resolution) purposes.
 
 ## 🚀 Key Features
-1. generate_pv: Effortless Data Compression 📊
+### 1. generate_pv:   Data Compression 📊
+
 The generate_pv command takes your spatial transcriptomics data in CSV format and performs hexagonal binning to compress the data while preserving spatial information. It calculates hexagon counts and cell counts, and creates a well-structured output directory with all the necessary files for downstream analysis.
 
-2. merge_visium: Seamless Data Integration 🧩
-With the merge_visium command, you can easily merge multiple Pseudovisium or Visium format files. This feature allows you to combine data from different datasets, stitch images together, and generate a merged output directory. Pseudovisium makes it effortless to integrate data from multiple spatial transcriptomics experiments, enabling comprehensive analysis across datasets.
 
-3. generate_qc_report: Comprehensive Quality Control 📈
-Pseudovisium's generate_qc_report command generates a detailed quality control (QC) report for your Pseudovisium output. It calculates a wide range of metrics, including the number of hexagons with a minimum count threshold, the number of genes present in a certain percentage of hexagons, and the median counts and features per hexagon. The report also showcases interactive hexagon plots for selected genes and provides comparison plots between different datasets, allowing you to assess the quality and consistency of your data.
+### 2. qc:   Quality Control 📈
+
+Pseudovisium's qc command generates a detailed quality control (QC) report for a set of Pseudovisium/Visium formatted replicates. It calculates a wide range of metrics, including the number of hexagons with a minimum count threshold, the number of genes present in a certain percentage of hexagons, and the median counts and features per hexagon. The report also showcases hexagon plots for selected genes and provides comparison plots between different datasets, allowing you to assess the quality and consistency of your data.
+
+### 3. merge:   Data Merging 🧩
+
+With the merge command, you can easily merge multiple Pseudovisium or Visium format files. This feature allows you to combine data from different datasets, merge images together, and generate a merged output directory in the Pseudovisium/Visium format. Pseudovisium makes it effortless to merge data from multiple spatial transcriptomics experiments, enabling comprehensive analysis across datasets.
+
 
 ## 🎯 Flexibility and Compatibility
-Pseudovisium is designed to be flexible and compatible with various spatial transcriptomics technologies. It supports data from different platforms and offers customizable output formats, ensuring seamless integration with other analysis tools and workflows.
+
+Pseudovisium is designed to be flexible and compatible with various spatial transcriptomics technologies. It supports data from different platforms and offers customizable output formats, ensuring seamless integration with other analysis tools and workflows. Input files range from transcripts.csv, to .h5 as well as 10X feature-barcode-matrix directories.
 Technologies tried include:
 
 #### Vizgen
 #### Xenium
 #### CosMx
 #### Curio
 #### seqFISH
 #### VisiumHD
 
 
-🚀 Get Started with Pseudovisium
+## 🚀 Get Started with Pseudovisium
+
 To start using Pseudovisium, simply install the package and explore the documentation and examples provided. Pseudovisium is open-source and actively maintained, ensuring continuous improvements and support for the spatial transcriptomics community.
 
 Pseudovisium is available on PyPI and can be easily installed using pip:
 
 ###### pip install Pseudovisium
 
 For more information and the latest version, visit the Pseudovisium PyPI page https://pypi.org/project/Pseudovisium/.
 
+## Examples
+See the example Google Colab on converting 10X Xenium Mouse pup data to Pseudovisium format:
+https://github.com/BKover99/Pseudovisium/blob/main/pseudovisium_mouse_pup.ipynb
 
-### Goals
+## Goals
 
 - [x] Releasing the repo with minimal working capabilities - Apr 20, 2024
 - [ ] Adding supporting Colab notebooks
 - [ ] Releasing all data used in this work on OneDrive
 - [ ] Tidying up all code
 - [ ] Posting pre-print to Biorxiv
 - [ ] Publication of peer-reviewed research article
```

### Comparing `Pseudovisium-0.0.3/setup.py` & `Pseudovisium-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #this is a setup.py file
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Python package for hexagonal binning of high-resolution spatial transcriptomic data'
 LONG_DESCRIPTION = 'Python package for hexagonal binning of high-resolution spatial transcriptomic data, for more information see https://github.com/BKover99/pseudovisium'
 
 
 setup(
     name="Pseudovisium",
     version=VERSION,
```

