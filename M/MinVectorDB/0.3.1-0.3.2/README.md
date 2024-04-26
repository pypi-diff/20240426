# Comparing `tmp/minvectordb-0.3.1.tar.gz` & `tmp/minvectordb-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minvectordb-0.3.1.tar", last modified: Wed Apr 24 05:51:40 2024, max compression
+gzip compressed data, was "minvectordb-0.3.2.tar", last modified: Fri Apr 26 10:55:19 2024, max compression
```

## Comparing `minvectordb-0.3.1.tar` & `minvectordb-0.3.2.tar`

### file list

```diff
@@ -1,56 +1,62 @@
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.944385 minvectordb-0.3.1/
--rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.3.1/LICENSE
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.943888 minvectordb-0.3.1/MinVectorDB.egg-info/
--rw-r--r--   0 guobingming   (501) staff       (20)    11386 2024-04-24 05:51:40.000000 minvectordb-0.3.1/MinVectorDB.egg-info/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)     1281 2024-04-24 05:51:40.000000 minvectordb-0.3.1/MinVectorDB.egg-info/SOURCES.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-24 05:51:40.000000 minvectordb-0.3.1/MinVectorDB.egg-info/dependency_links.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       54 2024-04-24 05:51:40.000000 minvectordb-0.3.1/MinVectorDB.egg-info/entry_points.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.3.1/MinVectorDB.egg-info/not-zip-safe
--rw-r--r--   0 guobingming   (501) staff       (20)      200 2024-04-24 05:51:40.000000 minvectordb-0.3.1/MinVectorDB.egg-info/requires.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-24 05:51:40.000000 minvectordb-0.3.1/MinVectorDB.egg-info/top_level.txt
--rw-r--r--   0 guobingming   (501) staff       (20)    11386 2024-04-24 05:51:40.944156 minvectordb-0.3.1/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)    10013 2024-04-24 02:27:10.000000 minvectordb-0.3.1/README.md
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.937264 minvectordb-0.3.1/min_vec/
--rw-r--r--   0 guobingming   (501) staff       (20)      122 2024-04-24 00:48:34.000000 minvectordb-0.3.1/min_vec/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.938152 minvectordb-0.3.1/min_vec/api/
--rw-r--r--   0 guobingming   (501) staff       (20)      273 2024-04-23 05:39:11.000000 minvectordb-0.3.1/min_vec/api/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)      398 2024-04-24 05:46:31.000000 minvectordb-0.3.1/min_vec/api/client_api.py
--rw-r--r--   0 guobingming   (501) staff       (20)    10321 2024-04-24 05:46:31.000000 minvectordb-0.3.1/min_vec/api/high_level.py
--rw-r--r--   0 guobingming   (501) staff       (20)    20874 2024-04-24 04:37:03.000000 minvectordb-0.3.1/min_vec/api/http_api.py
--rw-r--r--   0 guobingming   (501) staff       (20)    14711 2024-04-23 11:06:39.000000 minvectordb-0.3.1/min_vec/api/low_level.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.938542 minvectordb-0.3.1/min_vec/computational_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.3.1/min_vec/computational_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)      890 2024-04-17 08:04:09.000000 minvectordb-0.3.1/min_vec/computational_layer/engines.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.939161 minvectordb-0.3.1/min_vec/configs/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.3.1/min_vec/configs/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2553 2024-04-23 13:22:47.000000 minvectordb-0.3.1/min_vec/configs/config.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3548 2024-04-19 15:33:58.000000 minvectordb-0.3.1/min_vec/configs/parameters_validator.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.940180 minvectordb-0.3.1/min_vec/execution_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.3.1/min_vec/execution_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2328 2024-04-23 10:00:41.000000 minvectordb-0.3.1/min_vec/execution_layer/cluster_worker.py
--rw-r--r--   0 guobingming   (501) staff       (20)    18058 2024-04-23 13:36:51.000000 minvectordb-0.3.1/min_vec/execution_layer/matrix_serializer.py
--rw-r--r--   0 guobingming   (501) staff       (20)     7236 2024-04-23 13:11:40.000000 minvectordb-0.3.1/min_vec/execution_layer/query.py
--rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 minvectordb-0.3.1/min_vec/execution_layer/session.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.940502 minvectordb-0.3.1/min_vec/storage_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.3.1/min_vec/storage_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    14526 2024-04-23 09:08:02.000000 minvectordb-0.3.1/min_vec/storage_layer/storage.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.942410 minvectordb-0.3.1/min_vec/structures/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.3.1/min_vec/structures/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     6256 2024-04-23 13:26:51.000000 minvectordb-0.3.1/min_vec/structures/fields_filter.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4656 2024-04-23 11:07:42.000000 minvectordb-0.3.1/min_vec/structures/filter.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1037 2024-04-23 08:37:07.000000 minvectordb-0.3.1/min_vec/structures/id_checker.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1545 2024-04-12 07:35:09.000000 minvectordb-0.3.1/min_vec/structures/kmeans.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1449 2024-04-18 02:30:25.000000 minvectordb-0.3.1/min_vec/structures/limited_dict.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3150 2024-04-23 05:39:11.000000 minvectordb-0.3.1/min_vec/structures/limited_sort.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3785 2024-04-24 02:25:22.000000 minvectordb-0.3.1/min_vec/structures/scaler.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.942623 minvectordb-0.3.1/min_vec/utils/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.3.1/min_vec/utils/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4021 2024-04-23 09:26:54.000000 minvectordb-0.3.1/min_vec/utils/utils.py
--rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-24 05:51:40.944422 minvectordb-0.3.1/setup.cfg
--rw-r--r--   0 guobingming   (501) staff       (20)     1581 2024-04-24 00:46:19.000000 minvectordb-0.3.1/setup.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-24 05:51:40.943560 minvectordb-0.3.1/test/
--rw-r--r--   0 guobingming   (501) staff       (20)      198 2024-04-23 11:11:07.000000 minvectordb-0.3.1/test/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1557 2024-04-23 11:18:25.000000 minvectordb-0.3.1/test/test_hmvdb_initial.py
--rw-r--r--   0 guobingming   (501) staff       (20)     5305 2024-04-24 04:16:23.000000 minvectordb-0.3.1/test/test_http_api.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1591 2024-04-23 10:40:50.000000 minvectordb-0.3.1/test/test_smvdb_initial.py
--rw-r--r--   0 guobingming   (501) staff       (20)    13195 2024-04-23 11:10:18.000000 minvectordb-0.3.1/test/test_smvdb_save_and_query.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.385584 minvectordb-0.3.2/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.3.2/LICENSE
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.384998 minvectordb-0.3.2/MinVectorDB.egg-info/
+-rw-r--r--   0 guobingming   (501) staff       (20)    12327 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)     1470 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/SOURCES.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/dependency_links.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       54 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/entry_points.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.3.2/MinVectorDB.egg-info/not-zip-safe
+-rw-r--r--   0 guobingming   (501) staff       (20)      240 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/requires.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/top_level.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)    12327 2024-04-26 10:55:19.385294 minvectordb-0.3.2/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)    10961 2024-04-26 10:54:39.000000 minvectordb-0.3.2/README.md
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.376425 minvectordb-0.3.2/min_vec/
+-rw-r--r--   0 guobingming   (501) staff       (20)     1100 2024-04-26 10:04:57.000000 minvectordb-0.3.2/min_vec/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.377261 minvectordb-0.3.2/min_vec/api/
+-rw-r--r--   0 guobingming   (501) staff       (20)      273 2024-04-23 05:39:11.000000 minvectordb-0.3.2/min_vec/api/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    24476 2024-04-26 09:16:06.000000 minvectordb-0.3.2/min_vec/api/client_api.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    11043 2024-04-26 09:49:47.000000 minvectordb-0.3.2/min_vec/api/high_level.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    35323 2024-04-26 10:25:25.000000 minvectordb-0.3.2/min_vec/api/http_api.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    15062 2024-04-26 07:41:58.000000 minvectordb-0.3.2/min_vec/api/low_level.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.377553 minvectordb-0.3.2/min_vec/computational_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.3.2/min_vec/computational_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      890 2024-04-17 08:04:09.000000 minvectordb-0.3.2/min_vec/computational_layer/engines.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.378231 minvectordb-0.3.2/min_vec/configs/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.3.2/min_vec/configs/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2553 2024-04-23 13:22:47.000000 minvectordb-0.3.2/min_vec/configs/config.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3624 2024-04-25 06:47:17.000000 minvectordb-0.3.2/min_vec/configs/parameters_validator.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.379612 minvectordb-0.3.2/min_vec/execution_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.3.2/min_vec/execution_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2710 2024-04-26 08:20:20.000000 minvectordb-0.3.2/min_vec/execution_layer/cluster_worker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    19573 2024-04-26 08:44:04.000000 minvectordb-0.3.2/min_vec/execution_layer/matrix_serializer.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     8031 2024-04-26 08:19:12.000000 minvectordb-0.3.2/min_vec/execution_layer/query.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      409 2024-04-26 02:40:02.000000 minvectordb-0.3.2/min_vec/execution_layer/session.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.380030 minvectordb-0.3.2/min_vec/storage_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.3.2/min_vec/storage_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    15749 2024-04-26 07:59:35.000000 minvectordb-0.3.2/min_vec/storage_layer/storage.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.382139 minvectordb-0.3.2/min_vec/structures/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.3.2/min_vec/structures/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      677 2024-04-26 06:44:38.000000 minvectordb-0.3.2/min_vec/structures/counter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     6280 2024-04-26 05:45:48.000000 minvectordb-0.3.2/min_vec/structures/fields_filter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     5448 2024-04-24 23:46:29.000000 minvectordb-0.3.2/min_vec/structures/filter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      866 2024-04-26 05:45:48.000000 minvectordb-0.3.2/min_vec/structures/id_checker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1642 2024-04-26 08:20:02.000000 minvectordb-0.3.2/min_vec/structures/kmeans.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1449 2024-04-18 02:30:25.000000 minvectordb-0.3.2/min_vec/structures/limited_dict.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3258 2024-04-26 07:02:33.000000 minvectordb-0.3.2/min_vec/structures/limited_sort.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3864 2024-04-25 06:47:17.000000 minvectordb-0.3.2/min_vec/structures/scaler.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.382554 minvectordb-0.3.2/min_vec/utils/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.3.2/min_vec/utils/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4021 2024-04-25 06:40:13.000000 minvectordb-0.3.2/min_vec/utils/utils.py
+-rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-26 10:55:19.385627 minvectordb-0.3.2/setup.cfg
+-rw-r--r--   0 guobingming   (501) staff       (20)     1485 2024-04-26 10:28:05.000000 minvectordb-0.3.2/setup.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.382895 minvectordb-0.3.2/test/
+-rw-r--r--   0 guobingming   (501) staff       (20)      310 2024-04-25 11:00:27.000000 minvectordb-0.3.2/test/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.383106 minvectordb-0.3.2/test/docker_tests/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-04-26 03:04:25.000000 minvectordb-0.3.2/test/docker_tests/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3057 2024-04-26 04:00:27.000000 minvectordb-0.3.2/test/docker_tests/test_docker_api.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.384440 minvectordb-0.3.2/test/standard_tests/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-04-26 03:03:57.000000 minvectordb-0.3.2/test/standard_tests/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1601 2024-04-24 13:16:55.000000 minvectordb-0.3.2/test/standard_tests/test_hmvdb_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     6019 2024-04-26 03:51:59.000000 minvectordb-0.3.2/test/standard_tests/test_http_api.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1591 2024-04-23 10:40:50.000000 minvectordb-0.3.2/test/standard_tests/test_smvdb_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    14141 2024-04-26 08:24:07.000000 minvectordb-0.3.2/test/standard_tests/test_smvdb_save_and_query.py
```

### Comparing `minvectordb-0.3.1/LICENSE` & `minvectordb-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.1/MinVectorDB.egg-info/PKG-INFO` & `minvectordb-0.3.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,10 @@
-Metadata-Version: 2.1
-Name: MinVectorDB
-Version: 0.3.1
-Summary: MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
-Home-page: https://github.com/BirchKwok/MinVectorDB
-Author: Birch Kwok
-Author-email: birchkwok@gmail.com
-Keywords: vector database
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.17.0
-Requires-Dist: spinesUtils>=0.3.13
-Requires-Dist: msgpack>=1.0.2
-Requires-Dist: h5py>=3.4.0
-Requires-Dist: scikit-learn>=1.0.0
-Requires-Dist: cloudpickle>=2.0.0
-Requires-Dist: numexpr>=2.7.3
-Requires-Dist: pyroaring>=0.4.5
-Requires-Dist: jax>=0.4.25
-Requires-Dist: numba>=0.54.0
-Requires-Dist: jaxlib>=0.4.25
-Requires-Dist: flask>=2.0.1
-Requires-Dist: PyYAML>=5.4.1
-
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
-  <h3>A pure Python-implemented, lightweight, serverless, locally deployed vector database.</h3>
+  <h3>A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
     <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
@@ -65,173 +30,160 @@
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
 - **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
 MinVectorDB focuses on achieving 100% recall, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications that require responses within hundreds of milliseconds.
 
 While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
 
-## Install
+## Install Client API package (Mandatory)
 
 ```shell
 pip install MinVectorDB
 ```
 
-## Qucik Start
+## If you wish to use Docker (Optional)
 
-### Environment setup (optional, Each instance can only be set once, and needs to be set before instantiation)
+```shell
+docker pull birchkwok/minvectordb:latest
+```
 
+## Qucik Start
 
-```python
-import os
 
-# logger settings
-# logger level: DEBUG, INFO, WARNING, ERROR, CRITICAL
-os.environ['MVDB_LOG_LEVEL'] = 'INFO'  # default: INFO, Options are 'DEBUG'/'INFO'/'WARNING'/'ERROR'/'CRITICAL'
+```python
+import min_vec
+print("MinVectorDB version is: ", min_vec.__version__)
+```
 
-# log path
-os.environ['MVDB_LOG_PATH'] = './min_vec_db.log'  # default: None
+    MinVectorDB version is:  0.3.2
 
-# whether to truncate log file
-os.environ['MVDB_TRUNCATE_LOG'] = 'True'  # default: True
 
-# whether to add time to log
-os.environ['MVDB_LOG_WITH_TIME'] = 'False'  # default: False
+## Initialize Database
 
-# clustering settings
-# kmeans epochs
-os.environ['MVDB_KMEANS_EPOCHS'] = '500'  # default: 100
+MinVectorDB now supports HTTP API and Python local code API. 
 
-# query cache size
-os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
-# specify the number of chunks in the memory cache
-os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '40', must be integer-like string
+The HTTP API mode requires starting an HTTP server beforehand. You have two options: 
+- start directly.
+  
+  For direct startup, the default port is 7637. You can run the following command in the terminal to start the service:
+```shell
+min_vec run --host 127.0.0.1 --port 7637
 ```
 
-
-```python
-import min_vec
-print("MinVectorDB version is: ", min_vec.__version__)
-print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
+- within Docker
+  
+  In Docker, the default port is 5403. You can run the following command in the terminal to start the service:
+```shell
+docker run -p 5403:7637 birchkwok/minvectordb:latest
 ```
 
-    MinVectorDB version is:  0.3.0
-    MinVectorDB all configs:  
-     - MVDB_LOG_LEVEL: INFO
-     - MVDB_LOG_PATH: ./min_vec_db.log
-     - MVDB_TRUNCATE_LOG: True
-     - MVDB_LOG_WITH_TIME: False
-     - MVDB_KMEANS_EPOCHS: 500
-     - MVDB_QUERY_CACHE_SIZE: 10000
-     - MVDB_DATALOADER_BUFFER_SIZE: 20
+```python
+from min_vec import MinVectorDB
 
+# This method is for the Python local code API, recommended only for CI/CD testing or single-user local use.
+# Specify database root directory
+my_db = MinVectorDB('my_vec_db')  # Judgment condition, root_path does not start with http or https
+# or
+# Use the HTTP API mode, it is suitable for use in production environments.
+# For direct startup
+my_db = MinVectorDB("http://127.0.0.1:7637")
 
-### create a collection
+# within Docker
+my_db = MinVectorDB("http://127.0.0.1:5403")
+```
 
 
 ```python
 from min_vec import MinVectorDB
 
-# Specify database root directory
-my_db = MinVectorDB(root_path='my_vec_db')
+# For direct startup
+my_db = MinVectorDB("http://localhost:5403")
 ```
 
-    MinVectorDB - INFO - Successful initialization of MinVectorDB in root_path: /projects/MinVectorDB/my_vec_db
-
+### create a collection
 
 
 ```python
-collection = my_db.require_collection("test_collection", 4, drop_if_exists=True)
+collection = my_db.require_collection("test_collection", 4, drop_if_exists=True, scaler_bits=8)
 ```
 
-    MinVectorDB - INFO - Creating collection test_collection with: 
-    //    dim=4, collection='test_collection', 
-    //    n_clusters=16, chunk_size=100000,
-    //    distance='cosine', index_mode='IVF-FLAT', 
-    //    dtypes='float32', use_cache=True, 
-    //    scaler_bits=8, n_threads=10
-
-
 ### Add vectors
 
+When inserting vectors, collection requires manually running the `commit` function or inserting within the `insert_session` function context manager, which will run the `commit` function in the background.
+
 
 ```python
 with collection.insert_session():
-    id = collection.add_item(vector=[0.01, 0.34, 0.74, 0.31], id=1, field={'field': 'test_1', 'order': 0})
-    id = collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1})
-    id = collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2})
-    id = collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field': 'test_2', 'order': 3})
-    id = collection.add_item(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4})
-    id = collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field': 'test_3', 'order': 5})
-    id = collection.add_item(vector=[0.18, 0.34, 0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6})
-    id = collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7})
-    id = collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8})
-    id = collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field': 'test_1', 'order': 9})
+    id = collection.add_item(vector=[0.01, 0.34, 0.74, 0.31], id=1, field={'field': 'test_1', 'order': 0})   # id = 0
+    id = collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1})   # id = 1
+    id = collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2})   # id = 2
+    id = collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field': 'test_2', 'order': 3})   # id = 3
+    id = collection.add_item(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4})   # id = 4
+    id = collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field': 'test_3', 'order': 5})   # id = 5
+    id = collection.add_item(vector=[0.18, 0.34, 0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6})   # id = 6
+    id = collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7})   # id = 7
+    id = collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8})   # id = 8
+    id = collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field': 'test_1', 'order': 9})  # id = 9
 
 # If you do not use the insert_session function, you need to manually call the commit function to submit the data
 # collection.commit()
 ```
 
 
 ```python
-print(id)
+# or use the bulk_add_items function
+# with collection.insert_session():
+#     ids = collection.bulk_add_items([([0.01, 0.34, 0.74, 0.31], 0, {'field': 'test_1', 'order': 0}), 
+#                                      ([0.36, 0.43, 0.56, 0.12], 1, {'field': 'test_1', 'order': 1}), 
+#                                      ([0.03, 0.04, 0.10, 0.51], 2, {'field': 'test_2', 'order': 2}),
+#                                      ([0.11, 0.44, 0.23, 0.24], 3, {'field': 'test_2', 'order': 3}), 
+#                                      ([0.91, 0.43, 0.44, 0.67], 4, {'field': 'test_2', 'order': 4}), 
+#                                      ([0.92, 0.12, 0.56, 0.19], 5, {'field': 'test_3', 'order': 5}),
+#                                      ([0.18, 0.34, 0.56, 0.71], 6, {'field': 'test_1', 'order': 6}), 
+#                                      ([0.01, 0.33, 0.14, 0.31], 7, {'field': 'test_2', 'order': 7}), 
+#                                      ([0.71, 0.75, 0.91, 0.82], 8, {'field': 'test_3', 'order': 8}),
+#                                      ([0.75, 0.44, 0.38, 0.75], 9, {'field': 'test_1', 'order': 9})])
+# print(ids)  # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
 ```
 
-    10
-
-
 ### Query
 
 
 ```python
-collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=3)
+collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=10)
 ```
 
 
 
 
-    (array([2, 9, 1]), Array([0.99822044, 0.9201999 , 0.8585187 ], dtype=float32))
+    (array([ 2,  9,  1,  4,  6,  5, 10,  7,  8,  3]),
+     array([1.        , 0.92355633, 0.86097705, 0.85727406, 0.81551266,
+            0.813797  , 0.78595245, 0.7741583 , 0.6871773 , 0.34695023]))
 
 
 
 
 ```python
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
-    | - Database Shape: (10, 4)
-    | - Query Time: 0.00125 s
+    | - Collection Shape: (10, 4)
+    | - Query Time: 0.20518 s
     | - Query Distance: cosine
-    | - Query K: 3
-    | - Top 3 Results ID: [2 9 1]
-    | - Top 3 Results Similarity: [0.99822  0.9202   0.858519]
+    | - Query K: 10
+    | - Top 10 Results ID: [ 2  9  1  4  6  5 10  7  8  3]
+    | - Top 10 Results Similarity: [1.         0.92355633 0.86097705 0.85727406 0.81551266 0.813797
+     0.78595245 0.7741583  0.6871773  0.34695023]
     * - END OF REPORT -
     
 
 
-
-```python
-collection.status_report_['DATABASE STATUS REPORT']
-```
-
-
-
-
-    {'Database shape': (10, 4),
-     'Database last_commit_time': datetime.datetime(2024, 4, 23, 21, 16, 38, 764711),
-     'Database commit status': True,
-     'Database index_mode': 'IVF-FLAT',
-     'Database distance': 'cosine',
-     'Database use_cache': True,
-     'Database status': 'ACTIVE'}
-
-
-
 ### Use Filter
 
 
 ```python
 import operator
 
 from min_vec.structures.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
@@ -253,20 +205,20 @@
 )
 
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
-    | - Database Shape: (10, 4)
-    | - Query Time: 0.00237 s
+    | - Collection Shape: (10, 4)
+    | - Query Time: 0.11985 s
     | - Query Distance: cosine
     | - Query K: 10
     | - Top 10 Results ID: [ 2  1  4  5 10  3]
-    | - Top 10 Results Similarity: [0.99822    0.858519   0.85362    0.812733   0.783597   0.34614798]
+    | - Top 10 Results Similarity: [1.         0.86097705 0.85727406 0.813797   0.78595245 0.34695023]
     * - END OF REPORT -
     
 
 
 ### Drop a collection
 
 
@@ -287,15 +239,27 @@
 my_db.drop_database()
 my_db
 ```
 
 
 
 
-    DELETED MinVectorDB(root_path='/projects/MinVectorDB/my_vec_db')
+    MinVectorDB remote server at http://localhost:5403 does not exist.
+
+
+
+
+```python
+my_db.database_exists()
+```
+
+
+
+
+    {'status': 'success', 'params': {'exists': False}}
 
 
 
 ## What's Next
 
 - [Collection's operations](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/collections.ipynb)
 - [Add vectors to collection](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/add_vectors.ipynb)
```

#### html2text {}

```diff
@@ -1,29 +1,10 @@
-Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.1 Summary: MinVectorDB is
-a pure Python-implemented, lightweight, serverless vector, locally deployed
-databasethat offers clear and concise Python APIs, aimed at lowering the
-barrier to the use of vector databases. Home-page: https://github.com/
-BirchKwok/MinVectorDB Author: Birch Kwok Author-email: birchkwok@gmail.com
-Keywords: vector database Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers Classifier: Topic :: Software
-Development Classifier: Topic :: Scientific/Engineering Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
-Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: numpy>=1.17.0 Requires-Dist: spinesUtils>=0.3.13 Requires-Dist:
-msgpack>=1.0.2 Requires-Dist: h5py>=3.4.0 Requires-Dist: scikit-learn>=1.0.0
-Requires-Dist: cloudpickle>=2.0.0 Requires-Dist: numexpr>=2.7.3 Requires-Dist:
-pyroaring>=0.4.5 Requires-Dist: jax>=0.4.25 Requires-Dist: numba>=0.54.0
-Requires-Dist: jaxlib>=0.4.25 Requires-Dist: flask>=2.0.1 Requires-Dist:
-PyYAML>=5.4.1
                                  _[_M_i_n_V_e_c_t_o_r_D_B_]
-   ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerrlleessss,, llooccaallllyy ddeeppllooyyeedd
-                             vveeccttoorr ddaattaabbaassee.. ********
+    ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerr--ooppttiioonnaall,, mmuullttii--eenndd
+       ccoommppaattiibbllee,, vveeccttoorr ddaattaabbaassee ddeeppllooyyaabbllee llooccaallllyy oorr rreemmootteellyy.. ********
      _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _p_a_c_k_a_g_e_]
 â¡ **Serverless, simple parameters, simple API.** â¡ **Fast, memory-
 efficient, easily scales to millions of vectors.** â¡ **Supports cosine
 similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for
 inverted indexing.** â¡ **Friendly caching technology stores recently queried
 vectors for accelerated access.** â¡ **Based on a generic Python software
 stack, platform-independent, highly versatile.** > **WARNING**: MinVectorDB is
@@ -52,87 +33,94 @@
 focuses on achieving 100% recall, prioritizing recall accuracy over high-speed
 search performance. This approach ensures that users can reliably retrieve all
 relevant vector data, making MinVectorDB particularly suitable for applications
 that require responses within hundreds of milliseconds. While the project has
 not yet been benchmarked against other systems, we believe these planned
 features will significantly enhance MinVectorDB's capabilities in managing and
 retrieving vector data, addressing a wide range of user needs. ## Install
-```shell pip install MinVectorDB ``` ## Qucik Start ### Environment setup
-(optional, Each instance can only be set once, and needs to be set before
-instantiation) ```python import os # logger settings # logger level: DEBUG,
-INFO, WARNING, ERROR, CRITICAL os.environ['MVDB_LOG_LEVEL'] = 'INFO' # default:
-INFO, Options are 'DEBUG'/'INFO'/'WARNING'/'ERROR'/'CRITICAL' # log path
-os.environ['MVDB_LOG_PATH'] = './min_vec_db.log' # default: None # whether to
-truncate log file os.environ['MVDB_TRUNCATE_LOG'] = 'True' # default: True #
-whether to add time to log os.environ['MVDB_LOG_WITH_TIME'] = 'False' #
-default: False # clustering settings # kmeans epochs os.environ
-['MVDB_KMEANS_EPOCHS'] = '500' # default: 100 # query cache size os.environ
-['MVDB_QUERY_CACHE_SIZE'] = '10000' # default: 10000 # specify the number of
-chunks in the memory cache os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20' #
-default to '40', must be integer-like string ``` ```python import min_vec print
-("MinVectorDB version is: ", min_vec.__version__) print("MinVectorDB all
-configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in
-min_vec.get_all_configs().items()])) ``` MinVectorDB version is: 0.3.0
-MinVectorDB all configs: - MVDB_LOG_LEVEL: INFO - MVDB_LOG_PATH: ./
-min_vec_db.log - MVDB_TRUNCATE_LOG: True - MVDB_LOG_WITH_TIME: False -
-MVDB_KMEANS_EPOCHS: 500 - MVDB_QUERY_CACHE_SIZE: 10000 -
-MVDB_DATALOADER_BUFFER_SIZE: 20 ### create a collection ```python from min_vec
-import MinVectorDB # Specify database root directory my_db = MinVectorDB
-(root_path='my_vec_db') ``` MinVectorDB - INFO - Successful initialization of
-MinVectorDB in root_path: /projects/MinVectorDB/my_vec_db ```python collection
-= my_db.require_collection("test_collection", 4, drop_if_exists=True) ```
-MinVectorDB - INFO - Creating collection test_collection with: // dim=4,
-collection='test_collection', // n_clusters=16, chunk_size=100000, /
-/ distance='cosine', index_mode='IVF-FLAT', // dtypes='float32',
-use_cache=True, // scaler_bits=8, n_threads=10 ### Add vectors ```python with
+Client API package (Mandatory) ```shell pip install MinVectorDB ``` ## If you
+wish to use Docker (Optional) ```shell docker pull birchkwok/minvectordb:latest
+``` ## Qucik Start ```python import min_vec print("MinVectorDB version is: ",
+min_vec.__version__) ``` MinVectorDB version is: 0.3.2 ## Initialize Database
+MinVectorDB now supports HTTP API and Python local code API. The HTTP API mode
+requires starting an HTTP server beforehand. You have two options: - start
+directly. For direct startup, the default port is 7637. You can run the
+following command in the terminal to start the service: ```shell min_vec run --
+host 127.0.0.1 --port 7637 ``` - within Docker In Docker, the default port is
+5403. You can run the following command in the terminal to start the service:
+```shell docker run -p 5403:7637 birchkwok/minvectordb:latest ``` ```python
+from min_vec import MinVectorDB # This method is for the Python local code API,
+recommended only for CI/CD testing or single-user local use. # Specify database
+root directory my_db = MinVectorDB('my_vec_db') # Judgment condition, root_path
+does not start with http or https # or # Use the HTTP API mode, it is suitable
+for use in production environments. # For direct startup my_db = MinVectorDB
+("http://127.0.0.1:7637") # within Docker my_db = MinVectorDB("http://
+127.0.0.1:5403") ``` ```python from min_vec import MinVectorDB # For direct
+startup my_db = MinVectorDB("http://localhost:5403") ``` ### create a
+collection ```python collection = my_db.require_collection("test_collection",
+4, drop_if_exists=True, scaler_bits=8) ``` ### Add vectors When inserting
+vectors, collection requires manually running the `commit` function or
+inserting within the `insert_session` function context manager, which will run
+the `commit` function in the background. ```python with
 collection.insert_session(): id = collection.add_item(vector=[0.01, 0.34, 0.74,
-0.31], id=1, field={'field': 'test_1', 'order': 0}) id = collection.add_item
-(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1})
-id = collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field':
-'test_2', 'order': 2}) id = collection.add_item(vector=[0.11, 0.44, 0.23,
-0.24], id=4, field={'field': 'test_2', 'order': 3}) id = collection.add_item
-(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4})
-id = collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field':
-'test_3', 'order': 5}) id = collection.add_item(vector=[0.18, 0.34, 0.56,
-0.71], id=7, field={'field': 'test_1', 'order': 6}) id = collection.add_item
-(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7})
-id = collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field':
-'test_3', 'order': 8}) id = collection.add_item(vector=[0.75, 0.44, 0.38,
-0.75], id=10, field={'field': 'test_1', 'order': 9}) # If you do not use the
-insert_session function, you need to manually call the commit function to
-submit the data # collection.commit() ``` ```python print(id) ``` 10 ### Query
-```python collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=3) ``` (array([2,
-9, 1]), Array([0.99822044, 0.9201999 , 0.8585187 ], dtype=float32)) ```python
-print(collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Database
-Shape: (10, 4) | - Query Time: 0.00125 s | - Query Distance: cosine | - Query
-K: 3 | - Top 3 Results ID: [2 9 1] | - Top 3 Results Similarity: [0.99822
-0.9202 0.858519] * - END OF REPORT - ```python collection.status_report_
-['DATABASE STATUS REPORT'] ``` {'Database shape': (10, 4), 'Database
-last_commit_time': datetime.datetime(2024, 4, 23, 21, 16, 38, 764711),
-'Database commit status': True, 'Database index_mode': 'IVF-FLAT', 'Database
-distance': 'cosine', 'Database use_cache': True, 'Database status': 'ACTIVE'}
-### Use Filter ```python import operator from min_vec.structures.filter import
-Filter, FieldCondition, MatchField, IDCondition, MatchID collection.query
-( vector=[0.36, 0.43, 0.56, 0.12], k=10, query_filter=Filter( must=
-[ FieldCondition(key='field', matcher=MatchField('test_1')), # Support for
-filtering fields ], any=[ FieldCondition(key='order', matcher=MatchField(8,
-comparator=operator.ge)), IDCondition(MatchID([1, 2, 3, 4, 5])), # Support for
-filtering IDs ] ) ) print(collection.query_report_) ``` * - MOST RECENT QUERY
-REPORT - | - Database Shape: (10, 4) | - Query Time: 0.00237 s | - Query
-Distance: cosine | - Query K: 10 | - Top 10 Results ID: [ 2 1 4 5 10 3] | - Top
-10 Results Similarity: [0.99822 0.858519 0.85362 0.812733 0.783597 0.34614798]
-* - END OF REPORT - ### Drop a collection ```python print("Collection list
-before dropping:", my_db.show_collections()) my_db.drop_collection
-("test_collection") print("Collection list after dropped:",
-my_db.show_collections()) ``` Collection list before dropping:
-['test_collection'] Collection list after dropped: [] ## Drop the database
-```python my_db.drop_database() my_db ``` DELETED MinVectorDB(root_path='/
-projects/MinVectorDB/my_vec_db') ## What's Next - [Collection's operations]
-(https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
-collections.ipynb) - [Add vectors to collection](https://github.com/BirchKwok/
-MinVectorDB/blob/main/tutorials/add_vectors.ipynb) - [Using different indexing
-methods](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
+0.31], id=1, field={'field': 'test_1', 'order': 0}) # id = 0 id =
+collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field':
+'test_1', 'order': 1}) # id = 1 id = collection.add_item(vector=[0.03, 0.04,
+0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2}) # id = 2 id =
+collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field':
+'test_2', 'order': 3}) # id = 3 id = collection.add_item(vector=[0.91, 0.43,
+0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4}) # id = 4 id =
+collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field':
+'test_3', 'order': 5}) # id = 5 id = collection.add_item(vector=[0.18, 0.34,
+0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6}) # id = 6 id =
+collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field':
+'test_2', 'order': 7}) # id = 7 id = collection.add_item(vector=[0.71, 0.75,
+0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8}) # id = 8 id =
+collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field':
+'test_1', 'order': 9}) # id = 9 # If you do not use the insert_session
+function, you need to manually call the commit function to submit the data #
+collection.commit() ``` ```python # or use the bulk_add_items function # with
+collection.insert_session(): # ids = collection.bulk_add_items([([0.01, 0.34,
+0.74, 0.31], 0, {'field': 'test_1', 'order': 0}), # ([0.36, 0.43, 0.56, 0.12],
+1, {'field': 'test_1', 'order': 1}), # ([0.03, 0.04, 0.10, 0.51], 2, {'field':
+'test_2', 'order': 2}), # ([0.11, 0.44, 0.23, 0.24], 3, {'field': 'test_2',
+'order': 3}), # ([0.91, 0.43, 0.44, 0.67], 4, {'field': 'test_2', 'order': 4}),
+# ([0.92, 0.12, 0.56, 0.19], 5, {'field': 'test_3', 'order': 5}), # ([0.18,
+0.34, 0.56, 0.71], 6, {'field': 'test_1', 'order': 6}), # ([0.01, 0.33, 0.14,
+0.31], 7, {'field': 'test_2', 'order': 7}), # ([0.71, 0.75, 0.91, 0.82], 8,
+{'field': 'test_3', 'order': 8}), # ([0.75, 0.44, 0.38, 0.75], 9, {'field':
+'test_1', 'order': 9})]) # print(ids) # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9] ``` ###
+Query ```python collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=10) ```
+(array([ 2, 9, 1, 4, 6, 5, 10, 7, 8, 3]), array([1. , 0.92355633, 0.86097705,
+0.85727406, 0.81551266, 0.813797 , 0.78595245, 0.7741583 , 0.6871773 ,
+0.34695023])) ```python print(collection.query_report_) ``` * - MOST RECENT
+QUERY REPORT - | - Collection Shape: (10, 4) | - Query Time: 0.20518 s | -
+Query Distance: cosine | - Query K: 10 | - Top 10 Results ID: [ 2 9 1 4 6 5 10
+7 8 3] | - Top 10 Results Similarity: [1. 0.92355633 0.86097705 0.85727406
+0.81551266 0.813797 0.78595245 0.7741583 0.6871773 0.34695023] * - END OF
+REPORT - ### Use Filter ```python import operator from
+min_vec.structures.filter import Filter, FieldCondition, MatchField,
+IDCondition, MatchID collection.query( vector=[0.36, 0.43, 0.56, 0.12], k=10,
+query_filter=Filter( must=[ FieldCondition(key='field', matcher=MatchField
+('test_1')), # Support for filtering fields ], any=[ FieldCondition
+(key='order', matcher=MatchField(8, comparator=operator.ge)), IDCondition
+(MatchID([1, 2, 3, 4, 5])), # Support for filtering IDs ] ) ) print
+(collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Collection
+Shape: (10, 4) | - Query Time: 0.11985 s | - Query Distance: cosine | - Query
+K: 10 | - Top 10 Results ID: [ 2 1 4 5 10 3] | - Top 10 Results Similarity: [1.
+0.86097705 0.85727406 0.813797 0.78595245 0.34695023] * - END OF REPORT - ###
+Drop a collection ```python print("Collection list before dropping:",
+my_db.show_collections()) my_db.drop_collection("test_collection") print
+("Collection list after dropped:", my_db.show_collections()) ``` Collection
+list before dropping: ['test_collection'] Collection list after dropped: [] ##
+Drop the database ```python my_db.drop_database() my_db ``` MinVectorDB remote
+server at http://localhost:5403 does not exist. ```python my_db.database_exists
+() ``` {'status': 'success', 'params': {'exists': False}} ## What's Next -
+[Collection's operations](https://github.com/BirchKwok/MinVectorDB/blob/main/
+tutorials/collections.ipynb) - [Add vectors to collection](https://github.com/
+BirchKwok/MinVectorDB/blob/main/tutorials/add_vectors.ipynb) - [Using different
+indexing methods](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
 index_mode.ipynb) - [Using different distance metric functions](https://
 github.com/BirchKwok/MinVectorDB/blob/main/tutorials/distance.ipynb) -
 [Diversified queries](https://github.com/BirchKwok/MinVectorDB/blob/main/
 tutorials/queries.ipynb) - [Benchmarks](https://github.com/BirchKwok/
 MinVectorDB/blob/main/tutorials/Benchmarks.ipynb)
```

### Comparing `minvectordb-0.3.1/PKG-INFO` & `minvectordb-0.3.2/MinVectorDB.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.3.1
-Summary: MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
+Version: 0.3.2
+Summary: A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
@@ -18,28 +18,30 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: spinesUtils>=0.3.13
 Requires-Dist: msgpack>=1.0.2
-Requires-Dist: h5py>=3.4.0
 Requires-Dist: scikit-learn>=1.0.0
 Requires-Dist: cloudpickle>=2.0.0
 Requires-Dist: numexpr>=2.7.3
 Requires-Dist: pyroaring>=0.4.5
 Requires-Dist: jax>=0.4.25
 Requires-Dist: numba>=0.54.0
 Requires-Dist: jaxlib>=0.4.25
 Requires-Dist: flask>=2.0.1
 Requires-Dist: PyYAML>=5.4.1
+Requires-Dist: portalocker>=2.3.0
+Requires-Dist: requests>=2.26.0
+Requires-Dist: waitress>=2.0.0
 
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
-  <h3>A pure Python-implemented, lightweight, serverless, locally deployed vector database.</h3>
+  <h3>A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
     <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
@@ -65,173 +67,160 @@
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
 - **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
 MinVectorDB focuses on achieving 100% recall, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications that require responses within hundreds of milliseconds.
 
 While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
 
-## Install
+## Install Client API package (Mandatory)
 
 ```shell
 pip install MinVectorDB
 ```
 
-## Qucik Start
+## If you wish to use Docker (Optional)
 
-### Environment setup (optional, Each instance can only be set once, and needs to be set before instantiation)
+```shell
+docker pull birchkwok/minvectordb:latest
+```
 
+## Qucik Start
 
-```python
-import os
 
-# logger settings
-# logger level: DEBUG, INFO, WARNING, ERROR, CRITICAL
-os.environ['MVDB_LOG_LEVEL'] = 'INFO'  # default: INFO, Options are 'DEBUG'/'INFO'/'WARNING'/'ERROR'/'CRITICAL'
+```python
+import min_vec
+print("MinVectorDB version is: ", min_vec.__version__)
+```
 
-# log path
-os.environ['MVDB_LOG_PATH'] = './min_vec_db.log'  # default: None
+    MinVectorDB version is:  0.3.2
 
-# whether to truncate log file
-os.environ['MVDB_TRUNCATE_LOG'] = 'True'  # default: True
 
-# whether to add time to log
-os.environ['MVDB_LOG_WITH_TIME'] = 'False'  # default: False
+## Initialize Database
 
-# clustering settings
-# kmeans epochs
-os.environ['MVDB_KMEANS_EPOCHS'] = '500'  # default: 100
+MinVectorDB now supports HTTP API and Python local code API. 
 
-# query cache size
-os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
-# specify the number of chunks in the memory cache
-os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '40', must be integer-like string
+The HTTP API mode requires starting an HTTP server beforehand. You have two options: 
+- start directly.
+  
+  For direct startup, the default port is 7637. You can run the following command in the terminal to start the service:
+```shell
+min_vec run --host 127.0.0.1 --port 7637
 ```
 
-
-```python
-import min_vec
-print("MinVectorDB version is: ", min_vec.__version__)
-print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
+- within Docker
+  
+  In Docker, the default port is 5403. You can run the following command in the terminal to start the service:
+```shell
+docker run -p 5403:7637 birchkwok/minvectordb:latest
 ```
 
-    MinVectorDB version is:  0.3.0
-    MinVectorDB all configs:  
-     - MVDB_LOG_LEVEL: INFO
-     - MVDB_LOG_PATH: ./min_vec_db.log
-     - MVDB_TRUNCATE_LOG: True
-     - MVDB_LOG_WITH_TIME: False
-     - MVDB_KMEANS_EPOCHS: 500
-     - MVDB_QUERY_CACHE_SIZE: 10000
-     - MVDB_DATALOADER_BUFFER_SIZE: 20
+```python
+from min_vec import MinVectorDB
 
+# This method is for the Python local code API, recommended only for CI/CD testing or single-user local use.
+# Specify database root directory
+my_db = MinVectorDB('my_vec_db')  # Judgment condition, root_path does not start with http or https
+# or
+# Use the HTTP API mode, it is suitable for use in production environments.
+# For direct startup
+my_db = MinVectorDB("http://127.0.0.1:7637")
 
-### create a collection
+# within Docker
+my_db = MinVectorDB("http://127.0.0.1:5403")
+```
 
 
 ```python
 from min_vec import MinVectorDB
 
-# Specify database root directory
-my_db = MinVectorDB(root_path='my_vec_db')
+# For direct startup
+my_db = MinVectorDB("http://localhost:5403")
 ```
 
-    MinVectorDB - INFO - Successful initialization of MinVectorDB in root_path: /projects/MinVectorDB/my_vec_db
-
+### create a collection
 
 
 ```python
-collection = my_db.require_collection("test_collection", 4, drop_if_exists=True)
+collection = my_db.require_collection("test_collection", 4, drop_if_exists=True, scaler_bits=8)
 ```
 
-    MinVectorDB - INFO - Creating collection test_collection with: 
-    //    dim=4, collection='test_collection', 
-    //    n_clusters=16, chunk_size=100000,
-    //    distance='cosine', index_mode='IVF-FLAT', 
-    //    dtypes='float32', use_cache=True, 
-    //    scaler_bits=8, n_threads=10
-
-
 ### Add vectors
 
+When inserting vectors, collection requires manually running the `commit` function or inserting within the `insert_session` function context manager, which will run the `commit` function in the background.
+
 
 ```python
 with collection.insert_session():
-    id = collection.add_item(vector=[0.01, 0.34, 0.74, 0.31], id=1, field={'field': 'test_1', 'order': 0})
-    id = collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1})
-    id = collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2})
-    id = collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field': 'test_2', 'order': 3})
-    id = collection.add_item(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4})
-    id = collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field': 'test_3', 'order': 5})
-    id = collection.add_item(vector=[0.18, 0.34, 0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6})
-    id = collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7})
-    id = collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8})
-    id = collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field': 'test_1', 'order': 9})
+    id = collection.add_item(vector=[0.01, 0.34, 0.74, 0.31], id=1, field={'field': 'test_1', 'order': 0})   # id = 0
+    id = collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1})   # id = 1
+    id = collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2})   # id = 2
+    id = collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field': 'test_2', 'order': 3})   # id = 3
+    id = collection.add_item(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4})   # id = 4
+    id = collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field': 'test_3', 'order': 5})   # id = 5
+    id = collection.add_item(vector=[0.18, 0.34, 0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6})   # id = 6
+    id = collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7})   # id = 7
+    id = collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8})   # id = 8
+    id = collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field': 'test_1', 'order': 9})  # id = 9
 
 # If you do not use the insert_session function, you need to manually call the commit function to submit the data
 # collection.commit()
 ```
 
 
 ```python
-print(id)
+# or use the bulk_add_items function
+# with collection.insert_session():
+#     ids = collection.bulk_add_items([([0.01, 0.34, 0.74, 0.31], 0, {'field': 'test_1', 'order': 0}), 
+#                                      ([0.36, 0.43, 0.56, 0.12], 1, {'field': 'test_1', 'order': 1}), 
+#                                      ([0.03, 0.04, 0.10, 0.51], 2, {'field': 'test_2', 'order': 2}),
+#                                      ([0.11, 0.44, 0.23, 0.24], 3, {'field': 'test_2', 'order': 3}), 
+#                                      ([0.91, 0.43, 0.44, 0.67], 4, {'field': 'test_2', 'order': 4}), 
+#                                      ([0.92, 0.12, 0.56, 0.19], 5, {'field': 'test_3', 'order': 5}),
+#                                      ([0.18, 0.34, 0.56, 0.71], 6, {'field': 'test_1', 'order': 6}), 
+#                                      ([0.01, 0.33, 0.14, 0.31], 7, {'field': 'test_2', 'order': 7}), 
+#                                      ([0.71, 0.75, 0.91, 0.82], 8, {'field': 'test_3', 'order': 8}),
+#                                      ([0.75, 0.44, 0.38, 0.75], 9, {'field': 'test_1', 'order': 9})])
+# print(ids)  # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
 ```
 
-    10
-
-
 ### Query
 
 
 ```python
-collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=3)
+collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=10)
 ```
 
 
 
 
-    (array([2, 9, 1]), Array([0.99822044, 0.9201999 , 0.8585187 ], dtype=float32))
+    (array([ 2,  9,  1,  4,  6,  5, 10,  7,  8,  3]),
+     array([1.        , 0.92355633, 0.86097705, 0.85727406, 0.81551266,
+            0.813797  , 0.78595245, 0.7741583 , 0.6871773 , 0.34695023]))
 
 
 
 
 ```python
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
-    | - Database Shape: (10, 4)
-    | - Query Time: 0.00125 s
+    | - Collection Shape: (10, 4)
+    | - Query Time: 0.20518 s
     | - Query Distance: cosine
-    | - Query K: 3
-    | - Top 3 Results ID: [2 9 1]
-    | - Top 3 Results Similarity: [0.99822  0.9202   0.858519]
+    | - Query K: 10
+    | - Top 10 Results ID: [ 2  9  1  4  6  5 10  7  8  3]
+    | - Top 10 Results Similarity: [1.         0.92355633 0.86097705 0.85727406 0.81551266 0.813797
+     0.78595245 0.7741583  0.6871773  0.34695023]
     * - END OF REPORT -
     
 
 
-
-```python
-collection.status_report_['DATABASE STATUS REPORT']
-```
-
-
-
-
-    {'Database shape': (10, 4),
-     'Database last_commit_time': datetime.datetime(2024, 4, 23, 21, 16, 38, 764711),
-     'Database commit status': True,
-     'Database index_mode': 'IVF-FLAT',
-     'Database distance': 'cosine',
-     'Database use_cache': True,
-     'Database status': 'ACTIVE'}
-
-
-
 ### Use Filter
 
 
 ```python
 import operator
 
 from min_vec.structures.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
@@ -253,20 +242,20 @@
 )
 
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
-    | - Database Shape: (10, 4)
-    | - Query Time: 0.00237 s
+    | - Collection Shape: (10, 4)
+    | - Query Time: 0.11985 s
     | - Query Distance: cosine
     | - Query K: 10
     | - Top 10 Results ID: [ 2  1  4  5 10  3]
-    | - Top 10 Results Similarity: [0.99822    0.858519   0.85362    0.812733   0.783597   0.34614798]
+    | - Top 10 Results Similarity: [1.         0.86097705 0.85727406 0.813797   0.78595245 0.34695023]
     * - END OF REPORT -
     
 
 
 ### Drop a collection
 
 
@@ -287,15 +276,27 @@
 my_db.drop_database()
 my_db
 ```
 
 
 
 
-    DELETED MinVectorDB(root_path='/projects/MinVectorDB/my_vec_db')
+    MinVectorDB remote server at http://localhost:5403 does not exist.
+
+
+
+
+```python
+my_db.database_exists()
+```
+
+
+
+
+    {'status': 'success', 'params': {'exists': False}}
 
 
 
 ## What's Next
 
 - [Collection's operations](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/collections.ipynb)
 - [Add vectors to collection](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/add_vectors.ipynb)
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.1 Summary: MinVectorDB is
-a pure Python-implemented, lightweight, serverless vector, locally deployed
-databasethat offers clear and concise Python APIs, aimed at lowering the
-barrier to the use of vector databases. Home-page: https://github.com/
+Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.2 Summary: A pure Python-
+implemented, lightweight, server-optional, multi-end compatible, vector
+database deployable locally or remotely. Home-page: https://github.com/
 BirchKwok/MinVectorDB Author: Birch Kwok Author-email: birchkwok@gmail.com
 Keywords: vector database Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development Classifier: Topic :: Scientific/Engineering Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: numpy>=1.17.0 Requires-Dist: spinesUtils>=0.3.13 Requires-Dist:
-msgpack>=1.0.2 Requires-Dist: h5py>=3.4.0 Requires-Dist: scikit-learn>=1.0.0
-Requires-Dist: cloudpickle>=2.0.0 Requires-Dist: numexpr>=2.7.3 Requires-Dist:
+msgpack>=1.0.2 Requires-Dist: scikit-learn>=1.0.0 Requires-Dist:
+cloudpickle>=2.0.0 Requires-Dist: numexpr>=2.7.3 Requires-Dist:
 pyroaring>=0.4.5 Requires-Dist: jax>=0.4.25 Requires-Dist: numba>=0.54.0
 Requires-Dist: jaxlib>=0.4.25 Requires-Dist: flask>=2.0.1 Requires-Dist:
-PyYAML>=5.4.1
+PyYAML>=5.4.1 Requires-Dist: portalocker>=2.3.0 Requires-Dist: requests>=2.26.0
+Requires-Dist: waitress>=2.0.0
                                  _[_M_i_n_V_e_c_t_o_r_D_B_]
-   ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerrlleessss,, llooccaallllyy ddeeppllooyyeedd
-                             vveeccttoorr ddaattaabbaassee.. ********
+    ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerr--ooppttiioonnaall,, mmuullttii--eenndd
+       ccoommppaattiibbllee,, vveeccttoorr ddaattaabbaassee ddeeppllooyyaabbllee llooccaallllyy oorr rreemmootteellyy.. ********
      _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _p_a_c_k_a_g_e_]
 â¡ **Serverless, simple parameters, simple API.** â¡ **Fast, memory-
 efficient, easily scales to millions of vectors.** â¡ **Supports cosine
 similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for
 inverted indexing.** â¡ **Friendly caching technology stores recently queried
 vectors for accelerated access.** â¡ **Based on a generic Python software
 stack, platform-independent, highly versatile.** > **WARNING**: MinVectorDB is
@@ -52,87 +52,94 @@
 focuses on achieving 100% recall, prioritizing recall accuracy over high-speed
 search performance. This approach ensures that users can reliably retrieve all
 relevant vector data, making MinVectorDB particularly suitable for applications
 that require responses within hundreds of milliseconds. While the project has
 not yet been benchmarked against other systems, we believe these planned
 features will significantly enhance MinVectorDB's capabilities in managing and
 retrieving vector data, addressing a wide range of user needs. ## Install
-```shell pip install MinVectorDB ``` ## Qucik Start ### Environment setup
-(optional, Each instance can only be set once, and needs to be set before
-instantiation) ```python import os # logger settings # logger level: DEBUG,
-INFO, WARNING, ERROR, CRITICAL os.environ['MVDB_LOG_LEVEL'] = 'INFO' # default:
-INFO, Options are 'DEBUG'/'INFO'/'WARNING'/'ERROR'/'CRITICAL' # log path
-os.environ['MVDB_LOG_PATH'] = './min_vec_db.log' # default: None # whether to
-truncate log file os.environ['MVDB_TRUNCATE_LOG'] = 'True' # default: True #
-whether to add time to log os.environ['MVDB_LOG_WITH_TIME'] = 'False' #
-default: False # clustering settings # kmeans epochs os.environ
-['MVDB_KMEANS_EPOCHS'] = '500' # default: 100 # query cache size os.environ
-['MVDB_QUERY_CACHE_SIZE'] = '10000' # default: 10000 # specify the number of
-chunks in the memory cache os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20' #
-default to '40', must be integer-like string ``` ```python import min_vec print
-("MinVectorDB version is: ", min_vec.__version__) print("MinVectorDB all
-configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in
-min_vec.get_all_configs().items()])) ``` MinVectorDB version is: 0.3.0
-MinVectorDB all configs: - MVDB_LOG_LEVEL: INFO - MVDB_LOG_PATH: ./
-min_vec_db.log - MVDB_TRUNCATE_LOG: True - MVDB_LOG_WITH_TIME: False -
-MVDB_KMEANS_EPOCHS: 500 - MVDB_QUERY_CACHE_SIZE: 10000 -
-MVDB_DATALOADER_BUFFER_SIZE: 20 ### create a collection ```python from min_vec
-import MinVectorDB # Specify database root directory my_db = MinVectorDB
-(root_path='my_vec_db') ``` MinVectorDB - INFO - Successful initialization of
-MinVectorDB in root_path: /projects/MinVectorDB/my_vec_db ```python collection
-= my_db.require_collection("test_collection", 4, drop_if_exists=True) ```
-MinVectorDB - INFO - Creating collection test_collection with: // dim=4,
-collection='test_collection', // n_clusters=16, chunk_size=100000, /
-/ distance='cosine', index_mode='IVF-FLAT', // dtypes='float32',
-use_cache=True, // scaler_bits=8, n_threads=10 ### Add vectors ```python with
+Client API package (Mandatory) ```shell pip install MinVectorDB ``` ## If you
+wish to use Docker (Optional) ```shell docker pull birchkwok/minvectordb:latest
+``` ## Qucik Start ```python import min_vec print("MinVectorDB version is: ",
+min_vec.__version__) ``` MinVectorDB version is: 0.3.2 ## Initialize Database
+MinVectorDB now supports HTTP API and Python local code API. The HTTP API mode
+requires starting an HTTP server beforehand. You have two options: - start
+directly. For direct startup, the default port is 7637. You can run the
+following command in the terminal to start the service: ```shell min_vec run --
+host 127.0.0.1 --port 7637 ``` - within Docker In Docker, the default port is
+5403. You can run the following command in the terminal to start the service:
+```shell docker run -p 5403:7637 birchkwok/minvectordb:latest ``` ```python
+from min_vec import MinVectorDB # This method is for the Python local code API,
+recommended only for CI/CD testing or single-user local use. # Specify database
+root directory my_db = MinVectorDB('my_vec_db') # Judgment condition, root_path
+does not start with http or https # or # Use the HTTP API mode, it is suitable
+for use in production environments. # For direct startup my_db = MinVectorDB
+("http://127.0.0.1:7637") # within Docker my_db = MinVectorDB("http://
+127.0.0.1:5403") ``` ```python from min_vec import MinVectorDB # For direct
+startup my_db = MinVectorDB("http://localhost:5403") ``` ### create a
+collection ```python collection = my_db.require_collection("test_collection",
+4, drop_if_exists=True, scaler_bits=8) ``` ### Add vectors When inserting
+vectors, collection requires manually running the `commit` function or
+inserting within the `insert_session` function context manager, which will run
+the `commit` function in the background. ```python with
 collection.insert_session(): id = collection.add_item(vector=[0.01, 0.34, 0.74,
-0.31], id=1, field={'field': 'test_1', 'order': 0}) id = collection.add_item
-(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1})
-id = collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field':
-'test_2', 'order': 2}) id = collection.add_item(vector=[0.11, 0.44, 0.23,
-0.24], id=4, field={'field': 'test_2', 'order': 3}) id = collection.add_item
-(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4})
-id = collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field':
-'test_3', 'order': 5}) id = collection.add_item(vector=[0.18, 0.34, 0.56,
-0.71], id=7, field={'field': 'test_1', 'order': 6}) id = collection.add_item
-(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7})
-id = collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field':
-'test_3', 'order': 8}) id = collection.add_item(vector=[0.75, 0.44, 0.38,
-0.75], id=10, field={'field': 'test_1', 'order': 9}) # If you do not use the
-insert_session function, you need to manually call the commit function to
-submit the data # collection.commit() ``` ```python print(id) ``` 10 ### Query
-```python collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=3) ``` (array([2,
-9, 1]), Array([0.99822044, 0.9201999 , 0.8585187 ], dtype=float32)) ```python
-print(collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Database
-Shape: (10, 4) | - Query Time: 0.00125 s | - Query Distance: cosine | - Query
-K: 3 | - Top 3 Results ID: [2 9 1] | - Top 3 Results Similarity: [0.99822
-0.9202 0.858519] * - END OF REPORT - ```python collection.status_report_
-['DATABASE STATUS REPORT'] ``` {'Database shape': (10, 4), 'Database
-last_commit_time': datetime.datetime(2024, 4, 23, 21, 16, 38, 764711),
-'Database commit status': True, 'Database index_mode': 'IVF-FLAT', 'Database
-distance': 'cosine', 'Database use_cache': True, 'Database status': 'ACTIVE'}
-### Use Filter ```python import operator from min_vec.structures.filter import
-Filter, FieldCondition, MatchField, IDCondition, MatchID collection.query
-( vector=[0.36, 0.43, 0.56, 0.12], k=10, query_filter=Filter( must=
-[ FieldCondition(key='field', matcher=MatchField('test_1')), # Support for
-filtering fields ], any=[ FieldCondition(key='order', matcher=MatchField(8,
-comparator=operator.ge)), IDCondition(MatchID([1, 2, 3, 4, 5])), # Support for
-filtering IDs ] ) ) print(collection.query_report_) ``` * - MOST RECENT QUERY
-REPORT - | - Database Shape: (10, 4) | - Query Time: 0.00237 s | - Query
-Distance: cosine | - Query K: 10 | - Top 10 Results ID: [ 2 1 4 5 10 3] | - Top
-10 Results Similarity: [0.99822 0.858519 0.85362 0.812733 0.783597 0.34614798]
-* - END OF REPORT - ### Drop a collection ```python print("Collection list
-before dropping:", my_db.show_collections()) my_db.drop_collection
-("test_collection") print("Collection list after dropped:",
-my_db.show_collections()) ``` Collection list before dropping:
-['test_collection'] Collection list after dropped: [] ## Drop the database
-```python my_db.drop_database() my_db ``` DELETED MinVectorDB(root_path='/
-projects/MinVectorDB/my_vec_db') ## What's Next - [Collection's operations]
-(https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
-collections.ipynb) - [Add vectors to collection](https://github.com/BirchKwok/
-MinVectorDB/blob/main/tutorials/add_vectors.ipynb) - [Using different indexing
-methods](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
+0.31], id=1, field={'field': 'test_1', 'order': 0}) # id = 0 id =
+collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field':
+'test_1', 'order': 1}) # id = 1 id = collection.add_item(vector=[0.03, 0.04,
+0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2}) # id = 2 id =
+collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field':
+'test_2', 'order': 3}) # id = 3 id = collection.add_item(vector=[0.91, 0.43,
+0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4}) # id = 4 id =
+collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field':
+'test_3', 'order': 5}) # id = 5 id = collection.add_item(vector=[0.18, 0.34,
+0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6}) # id = 6 id =
+collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field':
+'test_2', 'order': 7}) # id = 7 id = collection.add_item(vector=[0.71, 0.75,
+0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8}) # id = 8 id =
+collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field':
+'test_1', 'order': 9}) # id = 9 # If you do not use the insert_session
+function, you need to manually call the commit function to submit the data #
+collection.commit() ``` ```python # or use the bulk_add_items function # with
+collection.insert_session(): # ids = collection.bulk_add_items([([0.01, 0.34,
+0.74, 0.31], 0, {'field': 'test_1', 'order': 0}), # ([0.36, 0.43, 0.56, 0.12],
+1, {'field': 'test_1', 'order': 1}), # ([0.03, 0.04, 0.10, 0.51], 2, {'field':
+'test_2', 'order': 2}), # ([0.11, 0.44, 0.23, 0.24], 3, {'field': 'test_2',
+'order': 3}), # ([0.91, 0.43, 0.44, 0.67], 4, {'field': 'test_2', 'order': 4}),
+# ([0.92, 0.12, 0.56, 0.19], 5, {'field': 'test_3', 'order': 5}), # ([0.18,
+0.34, 0.56, 0.71], 6, {'field': 'test_1', 'order': 6}), # ([0.01, 0.33, 0.14,
+0.31], 7, {'field': 'test_2', 'order': 7}), # ([0.71, 0.75, 0.91, 0.82], 8,
+{'field': 'test_3', 'order': 8}), # ([0.75, 0.44, 0.38, 0.75], 9, {'field':
+'test_1', 'order': 9})]) # print(ids) # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9] ``` ###
+Query ```python collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=10) ```
+(array([ 2, 9, 1, 4, 6, 5, 10, 7, 8, 3]), array([1. , 0.92355633, 0.86097705,
+0.85727406, 0.81551266, 0.813797 , 0.78595245, 0.7741583 , 0.6871773 ,
+0.34695023])) ```python print(collection.query_report_) ``` * - MOST RECENT
+QUERY REPORT - | - Collection Shape: (10, 4) | - Query Time: 0.20518 s | -
+Query Distance: cosine | - Query K: 10 | - Top 10 Results ID: [ 2 9 1 4 6 5 10
+7 8 3] | - Top 10 Results Similarity: [1. 0.92355633 0.86097705 0.85727406
+0.81551266 0.813797 0.78595245 0.7741583 0.6871773 0.34695023] * - END OF
+REPORT - ### Use Filter ```python import operator from
+min_vec.structures.filter import Filter, FieldCondition, MatchField,
+IDCondition, MatchID collection.query( vector=[0.36, 0.43, 0.56, 0.12], k=10,
+query_filter=Filter( must=[ FieldCondition(key='field', matcher=MatchField
+('test_1')), # Support for filtering fields ], any=[ FieldCondition
+(key='order', matcher=MatchField(8, comparator=operator.ge)), IDCondition
+(MatchID([1, 2, 3, 4, 5])), # Support for filtering IDs ] ) ) print
+(collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Collection
+Shape: (10, 4) | - Query Time: 0.11985 s | - Query Distance: cosine | - Query
+K: 10 | - Top 10 Results ID: [ 2 1 4 5 10 3] | - Top 10 Results Similarity: [1.
+0.86097705 0.85727406 0.813797 0.78595245 0.34695023] * - END OF REPORT - ###
+Drop a collection ```python print("Collection list before dropping:",
+my_db.show_collections()) my_db.drop_collection("test_collection") print
+("Collection list after dropped:", my_db.show_collections()) ``` Collection
+list before dropping: ['test_collection'] Collection list after dropped: [] ##
+Drop the database ```python my_db.drop_database() my_db ``` MinVectorDB remote
+server at http://localhost:5403 does not exist. ```python my_db.database_exists
+() ``` {'status': 'success', 'params': {'exists': False}} ## What's Next -
+[Collection's operations](https://github.com/BirchKwok/MinVectorDB/blob/main/
+tutorials/collections.ipynb) - [Add vectors to collection](https://github.com/
+BirchKwok/MinVectorDB/blob/main/tutorials/add_vectors.ipynb) - [Using different
+indexing methods](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
 index_mode.ipynb) - [Using different distance metric functions](https://
 github.com/BirchKwok/MinVectorDB/blob/main/tutorials/distance.ipynb) -
 [Diversified queries](https://github.com/BirchKwok/MinVectorDB/blob/main/
 tutorials/queries.ipynb) - [Benchmarks](https://github.com/BirchKwok/
 MinVectorDB/blob/main/tutorials/Benchmarks.ipynb)
```

### Comparing `minvectordb-0.3.1/README.md` & `minvectordb-0.3.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,47 @@
+Metadata-Version: 2.1
+Name: MinVectorDB
+Version: 0.3.2
+Summary: A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.
+Home-page: https://github.com/BirchKwok/MinVectorDB
+Author: Birch Kwok
+Author-email: birchkwok@gmail.com
+Keywords: vector database
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: spinesUtils>=0.3.13
+Requires-Dist: msgpack>=1.0.2
+Requires-Dist: scikit-learn>=1.0.0
+Requires-Dist: cloudpickle>=2.0.0
+Requires-Dist: numexpr>=2.7.3
+Requires-Dist: pyroaring>=0.4.5
+Requires-Dist: jax>=0.4.25
+Requires-Dist: numba>=0.54.0
+Requires-Dist: jaxlib>=0.4.25
+Requires-Dist: flask>=2.0.1
+Requires-Dist: PyYAML>=5.4.1
+Requires-Dist: portalocker>=2.3.0
+Requires-Dist: requests>=2.26.0
+Requires-Dist: waitress>=2.0.0
+
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
-  <h3>A pure Python-implemented, lightweight, serverless, locally deployed vector database.</h3>
+  <h3>A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
     <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
@@ -30,173 +67,160 @@
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
 - **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
 MinVectorDB focuses on achieving 100% recall, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications that require responses within hundreds of milliseconds.
 
 While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
 
-## Install
+## Install Client API package (Mandatory)
 
 ```shell
 pip install MinVectorDB
 ```
 
-## Qucik Start
+## If you wish to use Docker (Optional)
 
-### Environment setup (optional, Each instance can only be set once, and needs to be set before instantiation)
+```shell
+docker pull birchkwok/minvectordb:latest
+```
 
+## Qucik Start
 
-```python
-import os
 
-# logger settings
-# logger level: DEBUG, INFO, WARNING, ERROR, CRITICAL
-os.environ['MVDB_LOG_LEVEL'] = 'INFO'  # default: INFO, Options are 'DEBUG'/'INFO'/'WARNING'/'ERROR'/'CRITICAL'
+```python
+import min_vec
+print("MinVectorDB version is: ", min_vec.__version__)
+```
 
-# log path
-os.environ['MVDB_LOG_PATH'] = './min_vec_db.log'  # default: None
+    MinVectorDB version is:  0.3.2
 
-# whether to truncate log file
-os.environ['MVDB_TRUNCATE_LOG'] = 'True'  # default: True
 
-# whether to add time to log
-os.environ['MVDB_LOG_WITH_TIME'] = 'False'  # default: False
+## Initialize Database
 
-# clustering settings
-# kmeans epochs
-os.environ['MVDB_KMEANS_EPOCHS'] = '500'  # default: 100
+MinVectorDB now supports HTTP API and Python local code API. 
 
-# query cache size
-os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
-# specify the number of chunks in the memory cache
-os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '40', must be integer-like string
+The HTTP API mode requires starting an HTTP server beforehand. You have two options: 
+- start directly.
+  
+  For direct startup, the default port is 7637. You can run the following command in the terminal to start the service:
+```shell
+min_vec run --host 127.0.0.1 --port 7637
 ```
 
-
-```python
-import min_vec
-print("MinVectorDB version is: ", min_vec.__version__)
-print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
+- within Docker
+  
+  In Docker, the default port is 5403. You can run the following command in the terminal to start the service:
+```shell
+docker run -p 5403:7637 birchkwok/minvectordb:latest
 ```
 
-    MinVectorDB version is:  0.3.0
-    MinVectorDB all configs:  
-     - MVDB_LOG_LEVEL: INFO
-     - MVDB_LOG_PATH: ./min_vec_db.log
-     - MVDB_TRUNCATE_LOG: True
-     - MVDB_LOG_WITH_TIME: False
-     - MVDB_KMEANS_EPOCHS: 500
-     - MVDB_QUERY_CACHE_SIZE: 10000
-     - MVDB_DATALOADER_BUFFER_SIZE: 20
+```python
+from min_vec import MinVectorDB
 
+# This method is for the Python local code API, recommended only for CI/CD testing or single-user local use.
+# Specify database root directory
+my_db = MinVectorDB('my_vec_db')  # Judgment condition, root_path does not start with http or https
+# or
+# Use the HTTP API mode, it is suitable for use in production environments.
+# For direct startup
+my_db = MinVectorDB("http://127.0.0.1:7637")
 
-### create a collection
+# within Docker
+my_db = MinVectorDB("http://127.0.0.1:5403")
+```
 
 
 ```python
 from min_vec import MinVectorDB
 
-# Specify database root directory
-my_db = MinVectorDB(root_path='my_vec_db')
+# For direct startup
+my_db = MinVectorDB("http://localhost:5403")
 ```
 
-    MinVectorDB - INFO - Successful initialization of MinVectorDB in root_path: /projects/MinVectorDB/my_vec_db
-
+### create a collection
 
 
 ```python
-collection = my_db.require_collection("test_collection", 4, drop_if_exists=True)
+collection = my_db.require_collection("test_collection", 4, drop_if_exists=True, scaler_bits=8)
 ```
 
-    MinVectorDB - INFO - Creating collection test_collection with: 
-    //    dim=4, collection='test_collection', 
-    //    n_clusters=16, chunk_size=100000,
-    //    distance='cosine', index_mode='IVF-FLAT', 
-    //    dtypes='float32', use_cache=True, 
-    //    scaler_bits=8, n_threads=10
-
-
 ### Add vectors
 
+When inserting vectors, collection requires manually running the `commit` function or inserting within the `insert_session` function context manager, which will run the `commit` function in the background.
+
 
 ```python
 with collection.insert_session():
-    id = collection.add_item(vector=[0.01, 0.34, 0.74, 0.31], id=1, field={'field': 'test_1', 'order': 0})
-    id = collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1})
-    id = collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2})
-    id = collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field': 'test_2', 'order': 3})
-    id = collection.add_item(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4})
-    id = collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field': 'test_3', 'order': 5})
-    id = collection.add_item(vector=[0.18, 0.34, 0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6})
-    id = collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7})
-    id = collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8})
-    id = collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field': 'test_1', 'order': 9})
+    id = collection.add_item(vector=[0.01, 0.34, 0.74, 0.31], id=1, field={'field': 'test_1', 'order': 0})   # id = 0
+    id = collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1})   # id = 1
+    id = collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2})   # id = 2
+    id = collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field': 'test_2', 'order': 3})   # id = 3
+    id = collection.add_item(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4})   # id = 4
+    id = collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field': 'test_3', 'order': 5})   # id = 5
+    id = collection.add_item(vector=[0.18, 0.34, 0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6})   # id = 6
+    id = collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7})   # id = 7
+    id = collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8})   # id = 8
+    id = collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field': 'test_1', 'order': 9})  # id = 9
 
 # If you do not use the insert_session function, you need to manually call the commit function to submit the data
 # collection.commit()
 ```
 
 
 ```python
-print(id)
+# or use the bulk_add_items function
+# with collection.insert_session():
+#     ids = collection.bulk_add_items([([0.01, 0.34, 0.74, 0.31], 0, {'field': 'test_1', 'order': 0}), 
+#                                      ([0.36, 0.43, 0.56, 0.12], 1, {'field': 'test_1', 'order': 1}), 
+#                                      ([0.03, 0.04, 0.10, 0.51], 2, {'field': 'test_2', 'order': 2}),
+#                                      ([0.11, 0.44, 0.23, 0.24], 3, {'field': 'test_2', 'order': 3}), 
+#                                      ([0.91, 0.43, 0.44, 0.67], 4, {'field': 'test_2', 'order': 4}), 
+#                                      ([0.92, 0.12, 0.56, 0.19], 5, {'field': 'test_3', 'order': 5}),
+#                                      ([0.18, 0.34, 0.56, 0.71], 6, {'field': 'test_1', 'order': 6}), 
+#                                      ([0.01, 0.33, 0.14, 0.31], 7, {'field': 'test_2', 'order': 7}), 
+#                                      ([0.71, 0.75, 0.91, 0.82], 8, {'field': 'test_3', 'order': 8}),
+#                                      ([0.75, 0.44, 0.38, 0.75], 9, {'field': 'test_1', 'order': 9})])
+# print(ids)  # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
 ```
 
-    10
-
-
 ### Query
 
 
 ```python
-collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=3)
+collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=10)
 ```
 
 
 
 
-    (array([2, 9, 1]), Array([0.99822044, 0.9201999 , 0.8585187 ], dtype=float32))
+    (array([ 2,  9,  1,  4,  6,  5, 10,  7,  8,  3]),
+     array([1.        , 0.92355633, 0.86097705, 0.85727406, 0.81551266,
+            0.813797  , 0.78595245, 0.7741583 , 0.6871773 , 0.34695023]))
 
 
 
 
 ```python
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
-    | - Database Shape: (10, 4)
-    | - Query Time: 0.00125 s
+    | - Collection Shape: (10, 4)
+    | - Query Time: 0.20518 s
     | - Query Distance: cosine
-    | - Query K: 3
-    | - Top 3 Results ID: [2 9 1]
-    | - Top 3 Results Similarity: [0.99822  0.9202   0.858519]
+    | - Query K: 10
+    | - Top 10 Results ID: [ 2  9  1  4  6  5 10  7  8  3]
+    | - Top 10 Results Similarity: [1.         0.92355633 0.86097705 0.85727406 0.81551266 0.813797
+     0.78595245 0.7741583  0.6871773  0.34695023]
     * - END OF REPORT -
     
 
 
-
-```python
-collection.status_report_['DATABASE STATUS REPORT']
-```
-
-
-
-
-    {'Database shape': (10, 4),
-     'Database last_commit_time': datetime.datetime(2024, 4, 23, 21, 16, 38, 764711),
-     'Database commit status': True,
-     'Database index_mode': 'IVF-FLAT',
-     'Database distance': 'cosine',
-     'Database use_cache': True,
-     'Database status': 'ACTIVE'}
-
-
-
 ### Use Filter
 
 
 ```python
 import operator
 
 from min_vec.structures.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
@@ -218,20 +242,20 @@
 )
 
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
-    | - Database Shape: (10, 4)
-    | - Query Time: 0.00237 s
+    | - Collection Shape: (10, 4)
+    | - Query Time: 0.11985 s
     | - Query Distance: cosine
     | - Query K: 10
     | - Top 10 Results ID: [ 2  1  4  5 10  3]
-    | - Top 10 Results Similarity: [0.99822    0.858519   0.85362    0.812733   0.783597   0.34614798]
+    | - Top 10 Results Similarity: [1.         0.86097705 0.85727406 0.813797   0.78595245 0.34695023]
     * - END OF REPORT -
     
 
 
 ### Drop a collection
 
 
@@ -252,15 +276,27 @@
 my_db.drop_database()
 my_db
 ```
 
 
 
 
-    DELETED MinVectorDB(root_path='/projects/MinVectorDB/my_vec_db')
+    MinVectorDB remote server at http://localhost:5403 does not exist.
+
+
+
+
+```python
+my_db.database_exists()
+```
+
+
+
+
+    {'status': 'success', 'params': {'exists': False}}
 
 
 
 ## What's Next
 
 - [Collection's operations](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/collections.ipynb)
 - [Add vectors to collection](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/add_vectors.ipynb)
```

#### html2text {}

```diff
@@ -1,10 +1,29 @@
+Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.2 Summary: A pure Python-
+implemented, lightweight, server-optional, multi-end compatible, vector
+database deployable locally or remotely. Home-page: https://github.com/
+BirchKwok/MinVectorDB Author: Birch Kwok Author-email: birchkwok@gmail.com
+Keywords: vector database Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers Classifier: Topic :: Software
+Development Classifier: Topic :: Scientific/Engineering Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: numpy>=1.17.0 Requires-Dist: spinesUtils>=0.3.13 Requires-Dist:
+msgpack>=1.0.2 Requires-Dist: scikit-learn>=1.0.0 Requires-Dist:
+cloudpickle>=2.0.0 Requires-Dist: numexpr>=2.7.3 Requires-Dist:
+pyroaring>=0.4.5 Requires-Dist: jax>=0.4.25 Requires-Dist: numba>=0.54.0
+Requires-Dist: jaxlib>=0.4.25 Requires-Dist: flask>=2.0.1 Requires-Dist:
+PyYAML>=5.4.1 Requires-Dist: portalocker>=2.3.0 Requires-Dist: requests>=2.26.0
+Requires-Dist: waitress>=2.0.0
                                  _[_M_i_n_V_e_c_t_o_r_D_B_]
-   ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerrlleessss,, llooccaallllyy ddeeppllooyyeedd
-                             vveeccttoorr ddaattaabbaassee.. ********
+    ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerr--ooppttiioonnaall,, mmuullttii--eenndd
+       ccoommppaattiibbllee,, vveeccttoorr ddaattaabbaassee ddeeppllooyyaabbllee llooccaallllyy oorr rreemmootteellyy.. ********
      _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _p_a_c_k_a_g_e_]
 â¡ **Serverless, simple parameters, simple API.** â¡ **Fast, memory-
 efficient, easily scales to millions of vectors.** â¡ **Supports cosine
 similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for
 inverted indexing.** â¡ **Friendly caching technology stores recently queried
 vectors for accelerated access.** â¡ **Based on a generic Python software
 stack, platform-independent, highly versatile.** > **WARNING**: MinVectorDB is
@@ -33,87 +52,94 @@
 focuses on achieving 100% recall, prioritizing recall accuracy over high-speed
 search performance. This approach ensures that users can reliably retrieve all
 relevant vector data, making MinVectorDB particularly suitable for applications
 that require responses within hundreds of milliseconds. While the project has
 not yet been benchmarked against other systems, we believe these planned
 features will significantly enhance MinVectorDB's capabilities in managing and
 retrieving vector data, addressing a wide range of user needs. ## Install
-```shell pip install MinVectorDB ``` ## Qucik Start ### Environment setup
-(optional, Each instance can only be set once, and needs to be set before
-instantiation) ```python import os # logger settings # logger level: DEBUG,
-INFO, WARNING, ERROR, CRITICAL os.environ['MVDB_LOG_LEVEL'] = 'INFO' # default:
-INFO, Options are 'DEBUG'/'INFO'/'WARNING'/'ERROR'/'CRITICAL' # log path
-os.environ['MVDB_LOG_PATH'] = './min_vec_db.log' # default: None # whether to
-truncate log file os.environ['MVDB_TRUNCATE_LOG'] = 'True' # default: True #
-whether to add time to log os.environ['MVDB_LOG_WITH_TIME'] = 'False' #
-default: False # clustering settings # kmeans epochs os.environ
-['MVDB_KMEANS_EPOCHS'] = '500' # default: 100 # query cache size os.environ
-['MVDB_QUERY_CACHE_SIZE'] = '10000' # default: 10000 # specify the number of
-chunks in the memory cache os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20' #
-default to '40', must be integer-like string ``` ```python import min_vec print
-("MinVectorDB version is: ", min_vec.__version__) print("MinVectorDB all
-configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in
-min_vec.get_all_configs().items()])) ``` MinVectorDB version is: 0.3.0
-MinVectorDB all configs: - MVDB_LOG_LEVEL: INFO - MVDB_LOG_PATH: ./
-min_vec_db.log - MVDB_TRUNCATE_LOG: True - MVDB_LOG_WITH_TIME: False -
-MVDB_KMEANS_EPOCHS: 500 - MVDB_QUERY_CACHE_SIZE: 10000 -
-MVDB_DATALOADER_BUFFER_SIZE: 20 ### create a collection ```python from min_vec
-import MinVectorDB # Specify database root directory my_db = MinVectorDB
-(root_path='my_vec_db') ``` MinVectorDB - INFO - Successful initialization of
-MinVectorDB in root_path: /projects/MinVectorDB/my_vec_db ```python collection
-= my_db.require_collection("test_collection", 4, drop_if_exists=True) ```
-MinVectorDB - INFO - Creating collection test_collection with: // dim=4,
-collection='test_collection', // n_clusters=16, chunk_size=100000, /
-/ distance='cosine', index_mode='IVF-FLAT', // dtypes='float32',
-use_cache=True, // scaler_bits=8, n_threads=10 ### Add vectors ```python with
+Client API package (Mandatory) ```shell pip install MinVectorDB ``` ## If you
+wish to use Docker (Optional) ```shell docker pull birchkwok/minvectordb:latest
+``` ## Qucik Start ```python import min_vec print("MinVectorDB version is: ",
+min_vec.__version__) ``` MinVectorDB version is: 0.3.2 ## Initialize Database
+MinVectorDB now supports HTTP API and Python local code API. The HTTP API mode
+requires starting an HTTP server beforehand. You have two options: - start
+directly. For direct startup, the default port is 7637. You can run the
+following command in the terminal to start the service: ```shell min_vec run --
+host 127.0.0.1 --port 7637 ``` - within Docker In Docker, the default port is
+5403. You can run the following command in the terminal to start the service:
+```shell docker run -p 5403:7637 birchkwok/minvectordb:latest ``` ```python
+from min_vec import MinVectorDB # This method is for the Python local code API,
+recommended only for CI/CD testing or single-user local use. # Specify database
+root directory my_db = MinVectorDB('my_vec_db') # Judgment condition, root_path
+does not start with http or https # or # Use the HTTP API mode, it is suitable
+for use in production environments. # For direct startup my_db = MinVectorDB
+("http://127.0.0.1:7637") # within Docker my_db = MinVectorDB("http://
+127.0.0.1:5403") ``` ```python from min_vec import MinVectorDB # For direct
+startup my_db = MinVectorDB("http://localhost:5403") ``` ### create a
+collection ```python collection = my_db.require_collection("test_collection",
+4, drop_if_exists=True, scaler_bits=8) ``` ### Add vectors When inserting
+vectors, collection requires manually running the `commit` function or
+inserting within the `insert_session` function context manager, which will run
+the `commit` function in the background. ```python with
 collection.insert_session(): id = collection.add_item(vector=[0.01, 0.34, 0.74,
-0.31], id=1, field={'field': 'test_1', 'order': 0}) id = collection.add_item
-(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1})
-id = collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field':
-'test_2', 'order': 2}) id = collection.add_item(vector=[0.11, 0.44, 0.23,
-0.24], id=4, field={'field': 'test_2', 'order': 3}) id = collection.add_item
-(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4})
-id = collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field':
-'test_3', 'order': 5}) id = collection.add_item(vector=[0.18, 0.34, 0.56,
-0.71], id=7, field={'field': 'test_1', 'order': 6}) id = collection.add_item
-(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7})
-id = collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field':
-'test_3', 'order': 8}) id = collection.add_item(vector=[0.75, 0.44, 0.38,
-0.75], id=10, field={'field': 'test_1', 'order': 9}) # If you do not use the
-insert_session function, you need to manually call the commit function to
-submit the data # collection.commit() ``` ```python print(id) ``` 10 ### Query
-```python collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=3) ``` (array([2,
-9, 1]), Array([0.99822044, 0.9201999 , 0.8585187 ], dtype=float32)) ```python
-print(collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Database
-Shape: (10, 4) | - Query Time: 0.00125 s | - Query Distance: cosine | - Query
-K: 3 | - Top 3 Results ID: [2 9 1] | - Top 3 Results Similarity: [0.99822
-0.9202 0.858519] * - END OF REPORT - ```python collection.status_report_
-['DATABASE STATUS REPORT'] ``` {'Database shape': (10, 4), 'Database
-last_commit_time': datetime.datetime(2024, 4, 23, 21, 16, 38, 764711),
-'Database commit status': True, 'Database index_mode': 'IVF-FLAT', 'Database
-distance': 'cosine', 'Database use_cache': True, 'Database status': 'ACTIVE'}
-### Use Filter ```python import operator from min_vec.structures.filter import
-Filter, FieldCondition, MatchField, IDCondition, MatchID collection.query
-( vector=[0.36, 0.43, 0.56, 0.12], k=10, query_filter=Filter( must=
-[ FieldCondition(key='field', matcher=MatchField('test_1')), # Support for
-filtering fields ], any=[ FieldCondition(key='order', matcher=MatchField(8,
-comparator=operator.ge)), IDCondition(MatchID([1, 2, 3, 4, 5])), # Support for
-filtering IDs ] ) ) print(collection.query_report_) ``` * - MOST RECENT QUERY
-REPORT - | - Database Shape: (10, 4) | - Query Time: 0.00237 s | - Query
-Distance: cosine | - Query K: 10 | - Top 10 Results ID: [ 2 1 4 5 10 3] | - Top
-10 Results Similarity: [0.99822 0.858519 0.85362 0.812733 0.783597 0.34614798]
-* - END OF REPORT - ### Drop a collection ```python print("Collection list
-before dropping:", my_db.show_collections()) my_db.drop_collection
-("test_collection") print("Collection list after dropped:",
-my_db.show_collections()) ``` Collection list before dropping:
-['test_collection'] Collection list after dropped: [] ## Drop the database
-```python my_db.drop_database() my_db ``` DELETED MinVectorDB(root_path='/
-projects/MinVectorDB/my_vec_db') ## What's Next - [Collection's operations]
-(https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
-collections.ipynb) - [Add vectors to collection](https://github.com/BirchKwok/
-MinVectorDB/blob/main/tutorials/add_vectors.ipynb) - [Using different indexing
-methods](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
+0.31], id=1, field={'field': 'test_1', 'order': 0}) # id = 0 id =
+collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field':
+'test_1', 'order': 1}) # id = 1 id = collection.add_item(vector=[0.03, 0.04,
+0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2}) # id = 2 id =
+collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field':
+'test_2', 'order': 3}) # id = 3 id = collection.add_item(vector=[0.91, 0.43,
+0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4}) # id = 4 id =
+collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field':
+'test_3', 'order': 5}) # id = 5 id = collection.add_item(vector=[0.18, 0.34,
+0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6}) # id = 6 id =
+collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field':
+'test_2', 'order': 7}) # id = 7 id = collection.add_item(vector=[0.71, 0.75,
+0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8}) # id = 8 id =
+collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field':
+'test_1', 'order': 9}) # id = 9 # If you do not use the insert_session
+function, you need to manually call the commit function to submit the data #
+collection.commit() ``` ```python # or use the bulk_add_items function # with
+collection.insert_session(): # ids = collection.bulk_add_items([([0.01, 0.34,
+0.74, 0.31], 0, {'field': 'test_1', 'order': 0}), # ([0.36, 0.43, 0.56, 0.12],
+1, {'field': 'test_1', 'order': 1}), # ([0.03, 0.04, 0.10, 0.51], 2, {'field':
+'test_2', 'order': 2}), # ([0.11, 0.44, 0.23, 0.24], 3, {'field': 'test_2',
+'order': 3}), # ([0.91, 0.43, 0.44, 0.67], 4, {'field': 'test_2', 'order': 4}),
+# ([0.92, 0.12, 0.56, 0.19], 5, {'field': 'test_3', 'order': 5}), # ([0.18,
+0.34, 0.56, 0.71], 6, {'field': 'test_1', 'order': 6}), # ([0.01, 0.33, 0.14,
+0.31], 7, {'field': 'test_2', 'order': 7}), # ([0.71, 0.75, 0.91, 0.82], 8,
+{'field': 'test_3', 'order': 8}), # ([0.75, 0.44, 0.38, 0.75], 9, {'field':
+'test_1', 'order': 9})]) # print(ids) # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9] ``` ###
+Query ```python collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=10) ```
+(array([ 2, 9, 1, 4, 6, 5, 10, 7, 8, 3]), array([1. , 0.92355633, 0.86097705,
+0.85727406, 0.81551266, 0.813797 , 0.78595245, 0.7741583 , 0.6871773 ,
+0.34695023])) ```python print(collection.query_report_) ``` * - MOST RECENT
+QUERY REPORT - | - Collection Shape: (10, 4) | - Query Time: 0.20518 s | -
+Query Distance: cosine | - Query K: 10 | - Top 10 Results ID: [ 2 9 1 4 6 5 10
+7 8 3] | - Top 10 Results Similarity: [1. 0.92355633 0.86097705 0.85727406
+0.81551266 0.813797 0.78595245 0.7741583 0.6871773 0.34695023] * - END OF
+REPORT - ### Use Filter ```python import operator from
+min_vec.structures.filter import Filter, FieldCondition, MatchField,
+IDCondition, MatchID collection.query( vector=[0.36, 0.43, 0.56, 0.12], k=10,
+query_filter=Filter( must=[ FieldCondition(key='field', matcher=MatchField
+('test_1')), # Support for filtering fields ], any=[ FieldCondition
+(key='order', matcher=MatchField(8, comparator=operator.ge)), IDCondition
+(MatchID([1, 2, 3, 4, 5])), # Support for filtering IDs ] ) ) print
+(collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Collection
+Shape: (10, 4) | - Query Time: 0.11985 s | - Query Distance: cosine | - Query
+K: 10 | - Top 10 Results ID: [ 2 1 4 5 10 3] | - Top 10 Results Similarity: [1.
+0.86097705 0.85727406 0.813797 0.78595245 0.34695023] * - END OF REPORT - ###
+Drop a collection ```python print("Collection list before dropping:",
+my_db.show_collections()) my_db.drop_collection("test_collection") print
+("Collection list after dropped:", my_db.show_collections()) ``` Collection
+list before dropping: ['test_collection'] Collection list after dropped: [] ##
+Drop the database ```python my_db.drop_database() my_db ``` MinVectorDB remote
+server at http://localhost:5403 does not exist. ```python my_db.database_exists
+() ``` {'status': 'success', 'params': {'exists': False}} ## What's Next -
+[Collection's operations](https://github.com/BirchKwok/MinVectorDB/blob/main/
+tutorials/collections.ipynb) - [Add vectors to collection](https://github.com/
+BirchKwok/MinVectorDB/blob/main/tutorials/add_vectors.ipynb) - [Using different
+indexing methods](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
 index_mode.ipynb) - [Using different distance metric functions](https://
 github.com/BirchKwok/MinVectorDB/blob/main/tutorials/distance.ipynb) -
 [Diversified queries](https://github.com/BirchKwok/MinVectorDB/blob/main/
 tutorials/queries.ipynb) - [Benchmarks](https://github.com/BirchKwok/
 MinVectorDB/blob/main/tutorials/Benchmarks.ipynb)
```

### Comparing `minvectordb-0.3.1/min_vec/api/high_level.py` & `minvectordb-0.3.2/min_vec/api/high_level.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """high_level.py - The MinVectorDB API."""
 import json
 from pathlib import Path
 from typing import Union
 
 from spinesUtils.asserts import ParameterTypeAssert
+import portalocker
 
 from min_vec.api.low_level import StandaloneMinVectorDB
 from min_vec.api import logger
 from min_vec.utils.utils import unavailable_if_deleted
 
 
 class _Register:
@@ -23,22 +24,24 @@
         Save the collection name to the local database path.
 
         Parameters:
             collection (str): The name of the collection.
         """
         if not (self.root_path / 'collections.json').exists():
             with open(self.root_path / 'collections.json', 'w') as f:
+                portalocker.lock(f, portalocker.LOCK_EX)  # add lock
                 json.dump({collection: kwargs}, f)
         else:
             collections = self.get_collections_details()
 
             if collection not in collections:
                 collections[collection] = kwargs
 
                 with open(self.root_path / 'collections.json', 'w') as f:
+                    portalocker.lock(f, portalocker.LOCK_EX)  # add lock
                     json.dump(collections, f)
 
     def deregister_collection(self, collection: str):
         """
         Delete the collection name from the local database path.
 
         Parameters:
@@ -49,14 +52,15 @@
 
         collections = self.get_collections_details()
 
         if collection in collections:
             del collections[collection]
 
             with open(self.root_path / 'collections.json', 'w') as f:
+                portalocker.lock(f, portalocker.LOCK_EX)  # add lock
                 json.dump(collections, f)
 
     def get_collections_details(self) -> dict:
         """
         Show the collections in the database.
 
         Returns:
@@ -69,14 +73,15 @@
             collections = json.load(f)
 
         # 遍历collections，如果有不存在的collection，删除
         for collection in list(collections.keys()):
             if not (self.root_path / collection).exists():
                 del collections[collection]
                 with open(self.root_path / 'collections.json', 'w') as f:
+                    portalocker.lock(f, portalocker.LOCK_EX)  # add lock
                     json.dump(collections, f)
 
         return collections
 
     def show_collections(self) -> list:
         """
         Show the collections in the database.
@@ -86,38 +91,49 @@
         """
         return list(self.get_collections_details().keys())
 
     def __contains__(self, item):
         return item in self.get_collections_details()
 
 
-class MinVectorDB:
+class MinVectorDBLocalClient:
     """
-    A class for managing a vector database stored in .mvdb files and computing vectors similarity.
+    A singleton class for the local MinVectorDB client.
     """
+    _instance = None
+    _last_root_path = None
+
+    def __new__(cls, root_path: Union[Path, str]):
+        """
+        Create a new instance or return the existing instance of the class.
+        """
+        if cls._instance is not None and cls._last_root_path != root_path:
+            cls._instance = None
+            cls._last_root_path = root_path
+
+        if cls._instance is None:
+            cls._instance = super(MinVectorDBLocalClient, cls).__new__(cls)
+            cls._instance._init(root_path)
+
+        return cls._instance
 
     @ParameterTypeAssert({
         'root_path': str
     }, func_name='MinVectorDB')
-    def __init__(self, root_path: Union[Path, str]) -> None:
+    def _init(self, root_path: Union[Path, str]):
         """
         Initialize the vector database.
-
-        Parameters:
-            root_path (str): The root path of the database.
-                .. versionadded:: 0.3.0
         """
         self._root_path = Path(root_path).absolute()
         if not self._root_path.exists():
             self._root_path.mkdir(parents=True)
         logger.info(f"Successful initialization of MinVectorDB in root_path: {self._root_path.as_posix()}")
 
         self._register = _Register(root_path)
         self._collections = {}
-
         self.STATUS = 'INITIALIZED'
 
     @unavailable_if_deleted
     def require_collection(
             self, collection: str, dim: int = None,
             n_clusters: int = 16, chunk_size: int = 100_000,
             distance: str = 'cosine', index_mode: str = 'IVF-FLAT', dtypes: str = 'float32',
@@ -255,14 +271,15 @@
                     file.unlink()
                 else:
                     for f in file.iterdir():
                         f.unlink()
                     file.rmdir()
             self._root_path.rmdir()
 
+        MinVectorDBLocalClient._instance = None
         self.STATUS = 'DELETED'
 
     @property
     def root_path(self):
         return self._root_path.as_posix()
 
     def __repr__(self):
```

### Comparing `minvectordb-0.3.1/min_vec/api/http_api.py` & `minvectordb-0.3.2/min_vec/api/http_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,74 @@
 """使用flask实现的http接口, 用于向外部提供服务"""
 import json
 import operator
 import os
+import shutil
 from pathlib import Path
 
 import numpy as np
+import portalocker
 import yaml
 
 from flask import Flask, request, jsonify, Response
+from waitress import serve
 
-from min_vec.api.high_level import MinVectorDB
+from min_vec.api.high_level import MinVectorDBLocalClient
 from min_vec.structures.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
 
+
 os.environ['MVDB_LOG_LEVEL'] = 'ERROR'
 
 app = Flask(__name__)
 
+version = '0.3.2'
+
 # 构建配置文件的路径
 config_path = Path(os.path.expanduser('~/.MinVectorDB/config.yaml'))
 default_root_path = Path(os.path.expanduser('~/.MinVectorDB/data/min_vec_db')).as_posix()
 
 
 def generate_config(root_path: str = default_root_path, config_path: Path = config_path):
     """Generate a default configuration file.
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.3.2
     """
     if root_path is None:
         root_path = default_root_path
 
     if not config_path.exists():
         config_path.parent.mkdir(parents=True, exist_ok=True)
         config = {'root_path': root_path}
 
         with open(config_path, 'w') as file:
+            portalocker.lock(file, portalocker.LOCK_EX)
             yaml.dump(config, file)
     else:
         with open(config_path, 'r') as file:
             config = yaml.load(file, Loader=yaml.FullLoader)
             if 'root_path' not in config or config['root_path'] != root_path:
                 config['root_path'] = root_path
                 with open(config_path, 'w') as file:
+                    portalocker.lock(file, portalocker.LOCK_EX)
                     yaml.dump(config, file)
 
     return config_path, root_path, config
 
 
 root_path, config = 'PlaceholderName', {'root_path': 'PlaceholderName'}
 
 
+@app.route('/', methods=['GET'])
+def index():
+    return Response(json.dumps({'status': 'success', 'message': 'MinVectorDB HTTP API'}), mimetype='application/json')
+
+
 @app.route('/required_collection', methods=['POST'])
 def required_collection():
     """Create a collection in the database.
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.3.2
 
     Example:
         1) use curl
         curl -X POST http://localhost:7637/required_collection \
          -H "Content-Type: application/json" \
          -d '{
               "collection_name": "example_collection",
@@ -117,15 +130,15 @@
         data['n_threads'] = 10
     if 'warm_up' not in data:
         data['warm_up'] = True
     if 'drop_if_exists' not in data:
         data['drop_if_exists'] = False
 
     try:
-        my_vec_db = MinVectorDB(root_path=config['root_path'])
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
         collection = my_vec_db.require_collection(
             collection=data['collection_name'],
             dim=data['dim'],
             n_clusters=data['n_clusters'],
             chunk_size=data['chunk_size'],
             distance=data['distance'],
             index_mode=data['index_mode'],
@@ -154,15 +167,15 @@
     except Exception as e:
         return jsonify({'error': str(e)}), 500
 
 
 @app.route('/drop_collection', methods=['POST'])
 def drop_collection():
     """Drop a collection from the database.
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.3.2
 
     Example:
         1) use curl
         curl -X POST http://localhost:7637/drop_collection \
          -H "Content-Type: application/json" \
          -d '{
               "collection_name": "example_collection"
@@ -182,15 +195,15 @@
         dict: The status of the operation.
     """
     data = request.json
     if not data:
         return jsonify({'error': 'No data provided'}), 400
 
     try:
-        my_vec_db = MinVectorDB(root_path=config['root_path'])
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
         my_vec_db.drop_collection(data['collection_name'])
 
         return Response(json.dumps(
             {
                 'status': 'success', 'params': {
                 'collection_name': data['collection_name']
             }
@@ -203,15 +216,15 @@
     except Exception as e:
         return jsonify({'error': str(e)}), 500
 
 
 @app.route('/drop_database', methods=['GET'])
 def drop_database():
     """Drop the database.
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.3.2
 
     Example:
         1) use curl
         curl -X GET http://localhost:7637/drop_database -w "\n"
 
         2) use python requests
         import requests
@@ -220,29 +233,28 @@
         response = requests.get(url)
         print(response.json())
 
     Returns:
         dict: The status of the operation.
     """
     try:
-        my_vec_db = MinVectorDB(root_path=config['root_path'])
-        my_vec_db.drop_database()
+        shutil.rmtree(config['root_path'])
 
         return Response(json.dumps({
             'status': 'success'
         }, sort_keys=False),
             mimetype='application/json')
     except Exception as e:
         return jsonify({'error': str(e)}), 500
 
 
 @app.route('/database_exists', methods=['GET'])
 def database_exists():
     """Check if the database exists.
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.3.2
 
     Example:
         1) use curl
         curl -X GET http://localhost:7637/database_exists -w "\n"
 
         2) use python requests
         import requests
@@ -251,29 +263,29 @@
         response = requests.get(url)
         print(response.json())
 
     Returns:
         dict: The status of the operation.
     """
     try:
-        my_vec_db = MinVectorDB(root_path=config['root_path'])
+        exists = Path(config['root_path']).exists()
         return Response(json.dumps({
             'status': 'success', 'params': {
-                    'exists': True if my_vec_db.STATUS == 'INITIALIZED' else False
-                }
+                'exists': True if exists else False
+            }
         },
-       sort_keys=False), mimetype='application/json')
+            sort_keys=False), mimetype='application/json')
     except Exception as e:
         return jsonify({'error': str(e)}), 500
 
 
 @app.route('/show_collections', methods=['GET'])
 def show_collections():
     """Show all collections in the database.
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.3.2
 
     Example:
         1) use curl
         curl -X GET http://localhost:7637/show_collections -w "\n"
 
         2) use python requests
         import requests
@@ -282,38 +294,38 @@
         response = requests.get(url)
         print(response.json())
 
     Returns:
         dict: The status of the operation.
     """
     try:
-        my_vec_db = MinVectorDB(root_path=config['root_path'])
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
         collections = my_vec_db.show_collections()
         return Response(json.dumps({'status': 'success', 'params': {'collections': collections}},
                                    sort_keys=False), mimetype='application/json')
 
     except Exception as e:
         return jsonify({'error': str(e)}), 500
 
 
 @app.route('/add_item', methods=['POST'])
 def add_item():
     """Add an item to a collection.
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.3.2
 
     Example:
         1) use curl
         curl -X POST http://localhost:7637/add_item \
          -H "Content-Type: application/json" \
          -d '{
               "collection_name": "example_collection",
               "item": {
                   "vector": [0.1, 0.2, 0.3, 0.4],
                   "id": 1,
-                  "fields": {
+                  "field": {
                       "name": "example",
                       "age": 18
                     }
                 }
             }' -w "\n"
 
         2) use python requests
@@ -321,15 +333,15 @@
 
         url = 'http://localhost:7637/add_item'
         data = {
             "collection_name": "example_collection",
             "item": {
                 "vector": [0.1, 0.2, 0.3, 0.4],
                 "id": 1,
-                "fields": {
+                "field": {
                     "name": "example",
                     "age": 18
                 }
             }
         }
         response = requests.post(url, json=data)
         print(response.json())
@@ -338,95 +350,101 @@
         dict: The status of the operation.
     """
     data = request.json
     if not data:
         return jsonify({'error': 'No data provided'}), 400
 
     try:
-        my_vec_db = MinVectorDB(root_path=config['root_path'])
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
         collection = my_vec_db.get_collection(data['collection_name'])
-        with collection.insert_session():
-            collection.add_item(vector=np.array(data['item']['vector']), id=data['item'].get('id', None),
-                                field=data['item'].get('fields', None))
+        id = collection.add_item(vector=np.array(data['item']['vector']), id=data['item'].get('id', None),
+                                 field=data['item'].get('field', None))
 
         return Response(json.dumps(
             {
-                'status': 'success', 'params': {'collection_name': data['collection_name'], 'item': {
-                        'vector': data['item']['vector'], 'id': data['item'].get('id', None),
-                        'fields': data['item'].get('fields', None)
+                'status': 'success', 'params': {
+                    'collection_name': data['collection_name'], 'item': {
+                        'vector': data['item']['vector'], 'id': id,
+                        'field': data['item'].get('field', None)
                     }
                 }
             }, sort_keys=False),
             mimetype='application/json')
 
     except KeyError as e:
         return jsonify({'error': f'Missing required parameter {e}'}), 400
     except Exception as e:
         return jsonify({'error': str(e)}), 500
 
 
 @app.route('/query', methods=['POST'])
 def query():
     """Query the database for the vectors most similar to the given vector.
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.3.2
 
     Example:
         1) use curl
         curl -X POST http://localhost:7637/query \
          -H "Content-Type: application/json" \
          -d '{
               "collection_name": "example_collection",
               "vector": [0.1, 0.2, 0.3, 0.4],
               "k": 10,
-              'distance': 'cosine',
+              "distance": "cosine",
               "query_filter": {
                   "must": [
                       {
                           "field": "name",
                           "operator": "eq",
                           "value": "example"
+                      },
+                      {
+                          "ids": [1, 2, 3]
                       }
                   ],
                   "any": [
                       {
                           "field": "age",
                           "operator": "gt",
                           "value": 18
                         }
                     ]
                 },
-                return_similarity: true
+                "return_similarity": true
             }' -w "\n"
 
         2) use python requests
         import requests
 
         url = 'http://localhost:7637/query'
         data = {
             "collection_name": "example_collection",
             "vector": [0.1, 0.2, 0.3, 0.4],
             "k": 10,
-            'distance': 'cosine',
+            "distance": "cosine",
             "query_filter": {
                 "must": [
                     {
                         "field": "name",
                         "operator": "eq",
                         "value": "example"
+                    },
+                    {
+                        "ids": [1, 2, 3]
                     }
                 ],
                 "any": [
                     {
                         "field": "age",
                         "operator": "gt",
                         "value": 18
                     }
                 ]
             },
-            return_similarity: true
+            "return_similarity": true
         }
         response = requests.post(url, json=data)
         print(response.json())
 
     Returns:
         dict: The status of the operation.
     """
@@ -434,87 +452,95 @@
     if not data:
         return jsonify({'error': 'No data provided'}), 400
 
     if 'k' not in data:
         data['k'] = 10
 
     try:
-        my_vec_db = MinVectorDB(root_path=config['root_path'])
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
         collection = my_vec_db.get_collection(data['collection_name'])
 
-        query_filter = Filter(
-            must=[
-                FieldCondition(
-                    key=condition['field'],
-                    matcher=MatchField(
-                        value=condition['value'],
-                        comparator=getattr(operator, condition['operator'])
-                    )
-                ) for condition in data['query_filter']['must']
-            ] if 'must' in data['query_filter'] else None,
-            any=[
-                FieldCondition(
-                    key=condition['field'],
-                    matcher=MatchField(
-                        value=condition['value'],
-                        comparator=getattr(operator, condition['operator'])
-                    )
-                ) for condition in data['query_filter']['any']
-            ] if 'any' in data['query_filter'] else None
-        )
+        if data['query_filter'] is None:
+            query_filter = None
+        else:
+            query_filter = Filter(
+                must=[
+                    FieldCondition(
+                        key=condition['field'],
+                        matcher=MatchField(
+                            value=condition['value'],
+                            comparator=getattr(operator, condition['operator'])
+                        )
+                    ) if 'field' in condition and 'operator' in condition
+                    else IDCondition(matcher=MatchID(ids=condition['ids']))
+                    for condition in data['query_filter']['must']
+                ] if data['query_filter']['must'] is not None else None,
+                any=[
+                    FieldCondition(
+                        key=condition['field'],
+                        matcher=MatchField(
+                            value=condition['value'],
+                            comparator=getattr(operator, condition['operator'])
+                        )
+                    ) if 'field' in condition and 'operator' in condition
+                    else IDCondition(matcher=MatchID(ids=condition['ids']))
+                    for condition in data['query_filter']['any']
+                ] if data['query_filter']['any'] is not None else None
+            )
+
         ids, scores = collection.query(vector=data['vector'], k=data['k'],
                                        query_filter=query_filter,
                                        distance=data.get('distance', 'cosine'),
-                                       return_similarity=data.get('return_similarity', False))
+                                       return_similarity=data.get('return_similarity', True))
 
         if ids is not None:
             ids = ids.tolist()
             scores = scores.tolist()
 
         return Response(json.dumps(
             {
                 'status': 'success', 'params': {
-                    'collection_name': data['collection_name'], 'items': {
-                        'k': data['k'], 'ids': ids, 'scores': scores,
-                        'distance': collection.most_recent_query_report['Query Distance'],
-                        'query time': collection.most_recent_query_report['Query Time']
-                    }
+                'collection_name': data['collection_name'], 'items': {
+                    'k': data['k'], 'ids': ids, 'scores': scores,
+                    'distance': collection.most_recent_query_report['Query Distance'],
+                    'query time': collection.most_recent_query_report['Query Time']
+                }
             }
             }, sort_keys=False),
             mimetype='application/json')
     except KeyError as e:
         return jsonify({'error': f'Missing required parameter {e}'}), 400
     except Exception as e:
         return jsonify({'error': str(e)}), 500
 
 
 @app.route('/bulk_add_items', methods=['POST'])
 def bulk_add_items():
     """Bulk add items to a collection.
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.3.2
 
     Example:
         1) use curl
         curl -X POST http://localhost:7637/bulk_add_items \
          -H "Content-Type: application/json" \
          -d '{
               "collection_name": "example_collection",
               "items": [
                   {
                       "vector": [0.1, 0.2, 0.3, 0.4],
                       "id": 1,
-                      "fields": {
+                      "field": {
                           "name": "example",
                           "age": 18
                         }
                     },
                     {
                         "vector": [0.5, 0.6, 0.7, 0.8],
                         "id": 2,
-                        "fields": {
+                        "field": {
                             "name": "example",
                             "age": 20
                         }
                     }
                 ]
             }' -w "\n"
 
@@ -525,23 +551,23 @@
 
         data = {
             "collection_name": "example_collection",
             "items": [
                 {
                     "vector": [0.1, 0.2, 0.3, 0.4],
                     "id": 1,
-                    "fields": {
+                    "field": {
                         "name": "example",
                         "age": 18
                     }
                 },
                 {
                     "vector": [0.5, 0.6, 0.7, 0.8],
                     "id": 2,
-                    "fields": {
+                    "field": {
                         "name": "example",
                         "age": 20
                     }
                 }
             ]
         }
         response = requests.post(url, json=data)
@@ -551,41 +577,86 @@
         dict: The status of the operation.
     """
     data = request.json
     if not data:
         return jsonify({'error': 'No data provided'}), 400
 
     try:
-        my_vec_db = MinVectorDB(root_path=config['root_path'])
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
         collection = my_vec_db.get_collection(data['collection_name'])
         items = []
         for item in data['items']:
-            items.append((item['vector'], item.get('id', None), item.get('fields', None)))
+            items.append((item['vector'], item.get('id', None), item.get('field', None)))
 
-        with collection.insert_session():
-            collection.bulk_add_items(items)
+        ids = collection.bulk_add_items(items)
 
         return Response(json.dumps({
             'status': 'success', 'params': {
                 'collection_name': data['collection_name'], 'items': [
-                    {'vector': item[0], 'id': item[1], 'fields': item[2]} for item in items
-                ]
+                    {'vector': item[0], 'id': item[1], 'field': item[2]} for item in items
+                ], 'ids': ids
             }
         }, sort_keys=False),
             mimetype='application/json')
     except KeyError as e:
         return jsonify({'error': f'Missing required parameter {e}'}), 400
     except Exception as e:
         return jsonify({'error': str(e)}), 500
 
 
+@app.route('/commit', methods=['POST'])
+def commit():
+    """Commit the database.
+        .. versionadded:: 0.3.2
+
+    Example:
+        1) use curl
+        curl -X POST http://localhost:7637/commit \
+         -H "Content-Type: application/json" \
+         -d '{
+              "collection_name": "example_collection"
+             }' -w "\n"
+
+        2) use python requests
+        import requests
+
+        url = 'http://localhost:7637/commit'
+        data = {
+            "collection_name": "example_collection"
+        }
+        response = requests.post(url, json=data)
+        print(response.json())
+
+    Returns:
+        dict: The status of the operation.
+    """
+    data = request.json
+    if not data:
+        return jsonify({'error': 'No data provided'}), 400
+
+    try:
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
+        collection = my_vec_db.get_collection(data['collection_name'])
+        collection.commit()
+
+        return Response(json.dumps({
+            'status': 'success', 'params': {
+                'collection_name': data['collection_name']
+            }
+        }, sort_keys=False), mimetype='application/json')
+    except KeyError as e:
+        return jsonify({'error': f'Missing required parameter {e}'}), 400
+    except Exception as e:
+        return jsonify({'error': str(e)}), 500
+
+
 @app.route('/collection_shape', methods=['POST'])
 def collection_shape():
     """Get the shape of a collection.
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.3.2
 
     Example:
         1) use curl
         curl -X POST http://localhost:7637/collection_shape \
          -H "Content-Type: application/json" \
          -d '{
               "collection_name": "example_collection"
@@ -605,42 +676,404 @@
         dict: The status of the operation.
     """
     data = request.json
     if not data:
         return jsonify({'error': 'No data provided'}), 400
 
     try:
-        my_vec_db = MinVectorDB(root_path=config['root_path'])
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
         collection = my_vec_db.get_collection(data['collection_name'])
         return Response(json.dumps({'status': 'success', 'params': {
             'collection_name': data['collection_name'], 'shape': collection.shape
         }}, sort_keys=False), mimetype='application/json')
     except KeyError as e:
         return jsonify({'error': f'Missing required parameter {e}'}), 400
     except Exception as e:
         return jsonify({'error': str(e)}), 500
 
 
+@app.route('/set_environment', methods=['POST'])
+def set_environment():
+    """Set the environment variables.
+        .. versionadded:: 0.3.2
+
+    Example:
+        1) use curl
+        curl -X POST http://localhost:7637/set_environment \
+         -H "Content-Type: application/json" \
+         -d '{
+              "MVDB_LOG_LEVEL": "ERROR",
+              "MVDB_LOG_PATH": "/path/to/log",
+              "MVDB_TRUNCATE_LOG": "true",
+              "MVDB_LOG_WITH_TIME": "true",
+              "MVDB_KMEANS_EPOCHS": "100",
+              "MVDB_QUERY_CACHE_SIZE": "100",
+              "MVDB_DATALOADER_BUFFER_SIZE": "1000"
+             }' -w "\n"
+
+        2) use python requests
+        import requests
+
+        url = 'http://localhost:7637/set_environment'
+        data = {
+            "MVDB_LOG_LEVEL": "ERROR",
+            "MVDB_LOG_PATH": "/path/to/log",
+            "MVDB_TRUNCATE_LOG": "true",
+            "MVDB_LOG_WITH_TIME": "true",
+            "MVDB_KMEANS_EPOCHS": "100",
+            "MVDB_QUERY_CACHE_SIZE": "100",
+            "MVDB_DATALOADER_BUFFER_SIZE": "1000"
+        }
+
+        response = requests.post(url, json=data)
+        print(response.json())
+
+    Returns:
+        dict: The status of the operation.
+    """
+    data = request.json
+    if not data:
+        return jsonify({'error': 'No data provided'}), 400
+
+    try:
+        for key, value in data.items():
+            os.environ[key] = value
+        return Response(json.dumps({'status': 'success', 'params': data}, sort_keys=False), mimetype='application/json')
+    except Exception as e:
+        return jsonify({'error': str(e)}), 500
+
+
+@app.route('/get_environment', methods=['GET'])
+def get_environment():
+    """Get the environment variables.
+        .. versionadded:: 0.3.2
+
+    Example:
+        1) use curl
+        curl -X GET http://localhost:7637/get_environment -w "\n"
+
+        2) use python requests
+        import requests
+
+        url = 'http://localhost:7637/get_environment'
+        response = requests.get(url)
+        print(response.json())
+
+    Returns:
+        dict: The status of the operation.
+    """
+    env_list = ['MVDB_LOG_LEVEL', 'MVDB_LOG_PATH', 'MVDB_TRUNCATE_LOG', 'MVDB_LOG_WITH_TIME',
+                'MVDB_KMEANS_EPOCHS', 'MVDB_QUERY_CACHE_SIZE', 'MVDB_DATALOADER_BUFFER_SIZE']
+
+    params = {key: eval("global_config.key") for key in env_list}
+    try:
+        return Response(json.dumps({'status': 'success', 'params': params}, sort_keys=False),
+                        mimetype='application/json')
+    except Exception as e:
+        return jsonify({'error': str(e)}), 500
+
+
+@app.route('/get_collection_query_report', methods=['POST'])
+def get_collection_query_report():
+    """Get the query report of a collection.
+        .. versionadded:: 0.3.2
+
+    Example:
+        1) use curl
+        curl -X POST http://localhost:7637/get_collection_query_report \
+         -H "Content-Type: application/json" \
+         -d '{
+              "collection_name": "example_collection"
+             }' -w "\n"
+
+        2) use python requests
+        import requests
+
+        url = 'http://localhost:7637/get_collection_query_report'
+        data = {
+            "collection_name": "example_collection"
+        }
+        response = requests.post(url, json=data)
+        print(response.json())
+
+    Returns:
+        dict: The status of the operation.
+    """
+    data = request.json
+    if not data:
+        return jsonify({'error': 'No data provided'}), 400
+
+    try:
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
+        collection = my_vec_db.get_collection(data['collection_name'])
+
+        return Response(json.dumps({'status': 'success', 'params': {
+            'collection_name': data['collection_name'], 'query_report': collection.query_report_
+        }}, sort_keys=False), mimetype='application/json')
+    except KeyError as e:
+        return jsonify({'error': f'Missing required parameter {e}'}), 400
+    except Exception as e:
+        return jsonify({'error': str(e)}), 500
+
+
+@app.route('/get_collection_status_report', methods=['POST'])
+def get_collection_status_report():
+    """Get the status report of a collection.
+        .. versionadded:: 0.3.2
+
+    Example:
+        1) use curl
+        curl -X POST http://localhost:7637/get_collection_status_report \
+         -H "Content-Type: application/json" \
+         -d '{
+              "collection_name": "example_collection"
+             }' -w "\n"
+
+        2) use python requests
+        import requests
+
+        url = 'http://localhost:7637/get_collection_status_report'
+        data = {
+            "collection_name": "example_collection"
+        }
+        response = requests.post(url, json=data)
+        print(response.json())
+
+    Returns:
+        dict: The status of the operation.
+    """
+    data = request.json
+    if not data:
+        return jsonify({'error': 'No data provided'}), 400
+
+    try:
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
+        collection = my_vec_db.get_collection(data['collection_name'])
+
+        db_report = {'DATABASE STATUS REPORT': {
+            'Database shape': (
+                0, collection._matrix_serializer.dim) if collection._matrix_serializer.IS_DELETED else collection.shape,
+            'Database last_commit_time': collection._matrix_serializer.last_commit_time,
+            'Database commit status': collection._matrix_serializer.COMMIT_FLAG,
+            'Database index_mode': collection._matrix_serializer.index_mode,
+            'Database distance': collection._distance,
+            'Database use_cache': collection._use_cache,
+            'Database status': 'DELETED' if collection._matrix_serializer.IS_DELETED else 'ACTIVE'
+        }}
+
+        return Response(json.dumps({'status': 'success', 'params': {
+            'collection_name': data['collection_name'], 'status_report': db_report
+        }}, sort_keys=False), mimetype='application/json')
+    except KeyError as e:
+        return jsonify({'error': f'Missing required parameter {e}'}), 400
+    except Exception as e:
+        return jsonify({'error': str(e)}), 500
+
+
+@app.route('/is_collection_exists', methods=['POST'])
+def is_collection_exists():
+    """Check if a collection exists.
+        .. versionadded:: 0.3.2
+
+    Example:
+        1) use curl
+        curl -X POST http://localhost:7637/is_collection_exists \
+         -H "Content-Type: application/json" \
+         -d '{
+              "collection_name": "example_collection"
+             }' -w "\n"
+
+        2) use python requests
+        import requests
+
+        url = 'http://localhost:7637/is_collection_exists'
+        data = {
+            "collection_name": "example_collection"
+        }
+        response = requests.post(url, json=data)
+        print(response.json())
+
+    Returns:
+        dict: The status of the operation.
+    """
+    data = request.json
+    if not data:
+        return jsonify({'error': 'No data provided'}), 400
+
+    try:
+        my_vec_db = MinVectorDBLocalClient(root_path=config['root_path'])
+        return Response(json.dumps({'status': 'success', 'params': {
+            'collection_name': data['collection_name'], 'exists': data['collection_name'] in my_vec_db.show_collections()
+        }}, sort_keys=False), mimetype='application/json')
+    except KeyError as e:
+        return jsonify({'error': f'Missing required parameter {e}'}), 400
+    except Exception as e:
+        return jsonify({'error': str(e)}), 500
+
+
+@app.route('/get_collection_config', methods=['POST'])
+def get_collection_config():
+    """Get the configuration of a collection.
+        .. versionadded:: 0.3.2
+
+    Example:
+        1) use curl
+        curl -X POST http://localhost:7637/get_collection_config \
+         -H "Content-Type: application/json" \
+         -d '{
+              "collection_name": "example_collection"
+             }' -w "\n"
+
+        2) use python requests
+        import requests
+
+        url = 'http://localhost:7637/get_collection_config'
+        data = {
+            "collection_name": "example_collection"
+        }
+        response = requests.post(url, json=data)
+        print(response.json())
+
+    Returns:
+        dict: The status of the operation.
+    """
+    data = request.json
+    if not data:
+        return jsonify({'error': 'No data provided'}), 400
+
+    try:
+        config_json_path = Path(config['root_path']) / 'collections.json'
+        with open(config_json_path, 'r') as file:
+            collections = json.load(file)
+            collection_config = collections[data['collection_name']]
+
+        return Response(json.dumps({'status': 'success', 'params': {
+            'collection_name': data['collection_name'], 'config': collection_config
+        }}, sort_keys=False), mimetype='application/json')
+    except KeyError as e:
+        return jsonify({'error': f'Missing required parameter {e}'}), 400
+    except Exception as e:
+        return jsonify({'error': str(e)}), 500
+
+
+@app.route('/update_commit_msg', methods=['POST'])
+def update_commit_msg():
+    """Save the commit message of a collection.
+        .. versionadded:: 0.3.2
+
+    Example:
+        1) use curl
+        curl -X POST http://localhost:7637/save_commit_msg \
+         -H "Content-Type: application/json" \
+         -d '{
+              "collection_name": "example_collection",
+              "last_commit_time": "last_commit_time",
+             }' -w "\n"
+
+        2) use python requests
+        import requests
+
+        url = 'http://localhost:7637/save_commit_msg'
+        data = {
+            "collection_name": "example_collection",
+            "last_commit_time": "last_commit_time",
+        }
+        response = requests.post(url, json=data)
+        print(response.json())
+
+    Returns:
+        dict: The status of the operation.
+    """
+    data = request.json
+    if not data:
+        return jsonify({'error': 'No data provided'}), 400
+
+    try:
+        if (Path(config['root_path']) / 'commit_msg.json').exists():
+            with open(config['root_path'] + '/commit_msg.json', 'r') as file:
+                commit_msg = json.load(file)
+                commit_msg[data['collection_name']] = data
+        else:
+            commit_msg = {data['collection_name']: data}
+
+        with open(config['root_path'] + '/commit_msg.json', 'w') as file:
+            portalocker.lock(file, portalocker.LOCK_EX)
+            json.dump(commit_msg, file)
+
+        return Response(json.dumps({'status': 'success', 'params': {
+            'collection_name': data['collection_name']
+        }}, sort_keys=False), mimetype='application/json')
+    except KeyError as e:
+        return jsonify({'error': f'Missing required parameter {e}'}), 400
+    except Exception as e:
+        return jsonify({'error': str(e)}), 500
+
+
+@app.route('/get_commit_msg', methods=['POST'])
+def get_commit_msg():
+    """Get the commit message of a collection.
+        .. versionadded:: 0.3.2
+
+    Example:
+        1) use curl
+        curl -X POST http://localhost:7637/get_commit_msg \
+         -H "Content-Type: application/json" \
+         -d '{
+              "collection_name": "example_collection"
+             }' -w "\n"
+
+        2) use python requests
+        import requests
+
+        url = 'http://localhost:7637/get_commit_msg'
+        data = {
+            "collection_name": "example_collection"
+        }
+        response = requests.post(url, json=data)
+        print(response.json())
+
+    Returns:
+        dict: The status of the operation.
+    """
+    data = request.json
+    if not data:
+        return jsonify({'error': 'No data provided'}), 400
+
+    try:
+        if (Path(config['root_path']) / 'commit_msg.json').exists():
+            with open(config['root_path'] + '/commit_msg.json', 'r') as file:
+                commit_msg = json.load(file)
+                commit_msg = commit_msg.get(data['collection_name'], None)
+        else:
+            commit_msg = None
+
+        return Response(json.dumps({'status': 'success', 'params': {
+            'collection_name': data['collection_name'], 'commit_msg': commit_msg
+        }}, sort_keys=False), mimetype='application/json')
+    except KeyError as e:
+        return jsonify({'error': f'Missing required parameter {e}'}), 400
+    except Exception as e:
+        return jsonify({'error': str(e)}), 500
+
+
 def main():
     global config_path, default_root_path, config, root_path
     import argparse
-
-    parser = argparse.ArgumentParser(description='Start the MinVec HTTP API server.')
+    parser = argparse.ArgumentParser(description='Start the MinVectorDB HTTP API server.')
     parser.add_argument('--host', default='127.0.0.1', help='The host to bind to.')
     parser.add_argument('--port', default=7637, type=int, help='The port to bind to.')
+    parser.add_argument('--threads', default=4, type=int, help='Number of threads per worker.')
     parser.add_argument('--config', default=config_path, help='The path to the configuration file.')
     parser.add_argument('--root_path', default=default_root_path, help='The path to the database root directory.')
-    parser.add_argument('--debug', action='store_true', help='Enable debug mode.')
-    parser.add_argument('run', help='Run the HTTP API server.')
-
-    version = '0.3.1'
-
-    parser.add_argument('--version', action='version', version=version)
-
+    parser.add_argument('run', help='Run the server.')
     args = parser.parse_args()
 
     config_path = args.config
     root_path = args.root_path
     config_path, root_path, config = generate_config(root_path=root_path, config_path=config_path)
 
     if args.run:
-        app.run(host=args.host, port=args.port, debug=args.debug)
+        serve(app, host=args.host, port=args.port, threads=args.threads)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `minvectordb-0.3.1/min_vec/api/low_level.py` & `minvectordb-0.3.2/min_vec/api/low_level.py`

 * *Files 5% similar despite different names*

```diff
@@ -235,27 +235,30 @@
             raise ValueError('database is empty.')
 
         if k > self._matrix_serializer.shape[0]:
             k = self._matrix_serializer.shape[0]
 
         self.most_recent_query_report = {}
 
+        # update scaler
+        self._query.update_scaler(self._matrix_serializer.scaler)
+
         self._timer.start()
         if self._use_cache:
             res = self._query.query(vector=vector, k=k, query_filter=query_filter, index_mode=self._matrix_serializer.index_mode,
                                     distance=distance, return_similarity=return_similarity)
         else:
             res = self._query.query(vector=vector, k=k, query_filter=query_filter,
                                     index_mode=self._matrix_serializer.index_mode,
                                     now_time=datetime.datetime.now().strftime('%Y%m%d%H%M%S%f'),
                                     distance=distance,
                                     return_similarity=return_similarity)
 
         time_cost = self._timer.last_timestamp_diff()
-        self.most_recent_query_report['Database Shape'] = self.shape
+        self.most_recent_query_report['Collection Shape'] = self.shape
         self.most_recent_query_report['Query Time'] = f"{time_cost :>.5f} s"
         self.most_recent_query_report['Query Distance'] = self._distance if distance is None else distance
         self.most_recent_query_report['Query K'] = k
 
         if res[0] is not None:
             self.most_recent_query_report[f'Top {k} Results ID'] = res[0]
             if return_similarity:
@@ -302,33 +305,40 @@
         """
         Return the most recent query report.
         """
         # print as a pretty string
         # title use bold font
         report = '\n* - MOST RECENT QUERY REPORT -\n'
         for key, value in self.most_recent_query_report.items():
+            if key == 'Collection Shape':
+                value = self.shape
+
             report += f'| - {key}: {value}\n'
 
         report += '* - END OF REPORT -\n'
 
         return report
 
     @property
     def status_report_(self):
         """
         Return the database report.
         """
-        db_report = {'DATABASE STATUS REPORT': {
-            'Database shape': (0, self._matrix_serializer.dim) if self._matrix_serializer.IS_DELETED else self.shape,
-            'Database last_commit_time': self._matrix_serializer.last_commit_time,
-            'Database commit status': self._matrix_serializer.COMMIT_FLAG,
-            'Database index_mode': self._matrix_serializer.index_mode,
-            'Database distance': self._distance,
-            'Database use_cache': self._use_cache,
-            'Database status': 'DELETED' if self._matrix_serializer.IS_DELETED else 'ACTIVE'
+        if self._initialize_as_collection:
+            name = "Collection"
+        else:
+            name = "Database"
+
+        db_report = {f'{name.upper()} STATUS REPORT': {
+            f'{name} shape': (0, self._matrix_serializer.dim) if self._matrix_serializer.IS_DELETED else self.shape,
+            f'{name} last_commit_time': self._matrix_serializer.last_commit_time,
+            f'{name} index_mode': self._matrix_serializer.index_mode,
+            f'{name} distance': self._distance,
+            f'{name} use_cache': self._use_cache,
+            f'{name} status': 'DELETED' if self._matrix_serializer.IS_DELETED else 'ACTIVE'
         }}
 
         return db_report
 
     def __repr__(self):
         if self._matrix_serializer.IS_DELETED:
             if self._initialize_as_collection:
@@ -337,16 +347,21 @@
                 title = "Deleted MinVectorDB object with status: \n"
         else:
             if self._initialize_as_collection:
                 title = "MinVectorDB collection with status: \n"
             else:
                 title = "MinVectorDB object with status: \n"
 
-        report = '\n* - DATABASE STATUS REPORT -\n'
-        for key, value in self.status_report_['DATABASE STATUS REPORT'].items():
+        if self._initialize_as_collection:
+            name = "Collection"
+        else:
+            name = "Database"
+
+        report = f'\n* - {name.upper()} STATUS REPORT -\n'
+        for key, value in self.status_report_[f'{name.upper()} STATUS REPORT'].items():
             report += f'| - {key}: {value}\n'
 
         return title + report
 
     def __str__(self):
         return self.__repr__()
```

### Comparing `minvectordb-0.3.1/min_vec/computational_layer/engines.py` & `minvectordb-0.3.2/min_vec/computational_layer/engines.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.1/min_vec/configs/config.py` & `minvectordb-0.3.2/min_vec/configs/config.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.1/min_vec/configs/parameters_validator.py` & `minvectordb-0.3.2/min_vec/configs/parameters_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from functools import wraps
 from pathlib import Path
 
+import portalocker
 from spinesUtils.asserts import raise_if, generate_function_kwargs
 from spinesUtils.logging import Logger
 
 
 class ParametersValidator:
     """Database configuration, define once and can not be changed.
 
@@ -45,14 +46,15 @@
             self.logger.error(f"Failed to load the MinVectorDB configurations.")
             raise e
 
     def save_configs(self, configs_json: Path, configs: dict):
         """Save the configurations."""
         try:
             with open(configs_json, 'w') as f:
+                portalocker.lock(f, portalocker.LOCK_EX)
                 json.dump(configs, f)
 
             return configs
         except (PermissionError, OSError) as e:
             self.logger.error(f"Failed to save the MinVectorDB configurations.")
             raise e
```

### Comparing `minvectordb-0.3.1/min_vec/execution_layer/matrix_serializer.py` & `minvectordb-0.3.2/min_vec/execution_layer/matrix_serializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from datetime import datetime
 from pathlib import Path
 import shutil
 from typing import Union
 
 import numpy as np
+import portalocker
 from spinesUtils.asserts import raise_if
 from spinesUtils.logging import Logger
 
 from min_vec.structures.id_checker import IDChecker
 from min_vec.utils.utils import io_checker
 from min_vec.configs.config import config
 from min_vec.structures.kmeans import BatchKMeans
 from min_vec.structures.scaler import ScalarQuantization
 from min_vec.structures.fields_filter import FieldIndex
 from min_vec.storage_layer.storage import StorageWorker
 from min_vec.execution_layer.cluster_worker import ClusterWorker
+from min_vec.structures.counter import ThreadSafeCounter
 
 
 class MatrixSerializer:
     """
     The MatrixSerializer class is used to serialize and deserialize the matrix data.
     """
     def __init__(
@@ -87,16 +89,16 @@
         self.scaler = None
         if self.scaler_bits is not None:
             self._initialize_scalar_quantization()
 
         # initialize the storage worker
         self.storage_worker = StorageWorker(self.collections_path_parent, self.dim,
                                             self.chunk_size,
-                                            quantizer=None if self.scaler_bits is None else self.scaler,
                                             warm_up=warm_up)
+        self.counter = ThreadSafeCounter()
 
         # ============== Loading or create one empty collection ==============
         # first of all, initialize a collection
         self.database = []
         self.indices = []
         self.fields = []
 
@@ -178,37 +180,33 @@
     def reset_collection(self):
         """Reset the database to its initial state with zeros."""
         self.database = []
         self.indices = []
         self.fields = []
 
     @io_checker
-    def dataloader(self, filename, mode='eager'):
+    def dataloader(self, filename):
         """
         Generator for loading the database and index.
 
         Parameters:
             filename (str): The name of the file to load.
-            mode (str): The mode of the generator. Options are 'eager' or 'lazy'. Default is 'eager'.
 
         Yields:
             tuple: A tuple of (database, index, field).
 
         Raises:
             FileNotFoundError: If the file does not exist.
             IOError: If the file cannot be read.
             PermissionError: If the file cannot be read due to permission issues.
             UnKnownError: If an unknown error occurs.
         """
         data, indices = self.storage_worker.read(filename=filename)
 
-        if mode == 'lazy':
-            return data, indices
-        else:
-            return data, indices
+        return data, indices
 
     def _is_collection_reset(self):
         """
         Check if the collection is in its reset state (empty list).
 
         Returns:
             bool: True if the collection is reset, False otherwise.
@@ -286,27 +284,60 @@
             self.id_filter.to_file(self._filter_path)
 
             # save fields index
             self.logger.debug('Saving fields index...')
             self.fields_index.save(self.collections_path_parent / 'fields_index.mvdb')
 
             chunk_partition_size = self.storage_worker.get_shape(read_type='chunk')[0]
-            if chunk_partition_size >= 100000 and self.index_mode != 'FLAT':
-                self.logger.debug('Building index...')
-                # build index
-                self.build_index()
+            cluster_partition_size = self.storage_worker.get_shape(read_type='cluster')[0]
+
+            all_partition_size = self.storage_worker.get_shape(read_type='all')[0]
+
+            if all_partition_size >= 100000 and not (self.collections_path_parent / 'scaled_status.json').exists():
+                # only run once
+                self.storage_worker.update_quantizer(self.scaler)
+                filenames = self.storage_worker.get_all_files(read_type='chunk')
+                if filenames:
+                    for filename in filenames:
+                        self.storage_worker.write(filename=filename)
+
+                with open(self.collections_path_parent / 'scaled_status.json', 'w') as f:
+                    portalocker.lock(f, portalocker.LOCK_EX)
+                    import json
+                    json.dump({'status': True}, f)
+
+            if (
+                    cluster_partition_size == 0 and (chunk_partition_size >= 100000 and self.index_mode != 'FLAT')
+            ) or (
+                    cluster_partition_size > 0 and self.index_mode != 'FLAT'
+            ):
+                self.logger.info('Building index...')
+
+                if cluster_partition_size == 0 and (chunk_partition_size >= 100000 and self.index_mode != 'FLAT'):
+                    self.logger.info('Start to fit the index for cluster...')
+                    self.cluster_worker.build_index(refit=True)
+                else:
+                    self.counter.add(chunk_partition_size)
+                    if self.counter.get_value() >= 100000:
+                        self.logger.info('Refitting the index for cluster...')
+                        self.cluster_worker.build_index(refit=True)
+                        self.counter.reset()
+                    else:
+                        self.logger.info('Incrementally building the index for cluster...')
+                        self.cluster_worker.build_index(refit=False)
 
                 # save ivf index and k-means model
                 self.logger.debug('Saving ann model...')
                 self.ann_model.save(self.collections_path_parent / 'ann_model.mvdb')
 
             self.reset_collection()
 
             if self.scaler_bits is not None:
-                self.scaler.save(self.collections_path_parent / 'sq_model.mvdb')
+                if self.scaler.fitted:
+                    self.scaler.save(self.collections_path_parent / 'sq_model.mvdb')
 
             self.COMMIT_FLAG = True
 
             self.last_commit_time = datetime.now()
 
     def _generate_new_id(self):
         """
@@ -363,15 +394,16 @@
                     vector, index = sample
                     field = {}
                 else:
                     raise_if(ValueError, len(sample) != 3,
                              f'vectors must be tuple of (vector, id[optional], field[optional]).')
                     vector, index, field = sample
 
-                    raise_if(TypeError, not isinstance(field, dict), f'field must be dict, got {type(field)}')
+                    raise_if(TypeError, not (isinstance(field, dict) or field is None),
+                             f'field must be dict or None, got {type(field)}')
 
                 if isinstance(vector, list):
                     vector = np.array(vector)
 
                 index = self._generate_new_id() if index is None else index
 
                 raise_if(ValueError, index < 0, f'id must be greater than 0, got {index}')
@@ -459,17 +491,11 @@
         self._initialize_fields_index()
         self._initialize_ann_model()
         self._initialize_id_checker()
 
         # clear cache
         self.storage_worker.clear_cache()
 
-    def build_index(self):
-        """
-        Build the IVF index.
-        """
-        self.cluster_worker.build_index(self.scaler)
-
     @property
     def shape(self):
         self.check_commit()
         return tuple(self.storage_worker.get_shape(read_type='all'))
```

### Comparing `minvectordb-0.3.1/min_vec/execution_layer/query.py` & `minvectordb-0.3.2/min_vec/execution_layer/query.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,31 +33,44 @@
         self.chunk_size = self.matrix_serializer.chunk_size
 
         self.fields_index = self.matrix_serializer.fields_index
 
         self.n_threads = n_threads
 
         self.scaler = getattr(self.matrix_serializer, 'scaler', None)
+        if self.scaler is not None and not self.scaler.fitted:
+            self.scaler = None
 
         self.executors = ThreadPoolExecutor(max_workers=self.n_threads)
         self.limited_sorted = LimitedSorted(dim=self.matrix_serializer.dim, dtype=self.dtypes,
                                             scaler=self.scaler, chunk_size=self.chunk_size)
 
+    def update_scaler(self, scaler):
+        if scaler is not None:
+            self.scaler = scaler
+        else:
+            self.scaler = getattr(self.matrix_serializer, 'scaler', None)
+
+        if self.scaler is not None and not self.scaler.fitted:
+            self.scaler = None
+
+        self.limited_sorted.scaler = self.scaler
+
     def _query_chunk(self, vector, query_filter, dataloader, filename):
         """
         Query a single database chunk for the vectors most similar to the given vector.
 
         Parameters:
             vector (np.ndarray): The query vector.
             query_filter (Filter, optional): The field filter to apply to the query.
 
         Returns:
             Tuple: The indices and similarity scores of the nearest vectors in the chunk.
         """
-        database_chunk, index_chunk = dataloader(filename, mode='lazy')
+        database_chunk, index_chunk = dataloader(filename)
 
         if query_filter is not None:
             subset_indices = []
             field_filters_must = []
             field_filters_any = []
 
             if query_filter.must:
@@ -131,14 +144,15 @@
         if isinstance(vector, list):
             vector = np.array(vector)
 
         vector = vector.astype(self.dtypes) if vector.dtype != self.dtypes else vector
 
         vector = to_normalize(vector)
 
+        # set the number of nearest vectors to return
         self.limited_sorted.set_n(k)
 
         all_index = []
 
         def batch_query(is_ivf=True, cid=None, sort=True):
             nonlocal all_index
 
@@ -167,15 +181,25 @@
         # if the index mode is FLAT, use FLAT
         if not (self.matrix_serializer.ann_model is not None and self.matrix_serializer.ann_model.fitted):
             return batch_query(is_ivf=False)
 
         # otherwise, use IVF-FLAT
         cluster_id_sorted = np.argsort(
             -cosine_distance(vector, self.matrix_serializer.ann_model.cluster_centers_)
-        )
+        ).tolist()
+
+        if self.scaler is not None:
+            d_vector = self.scaler.encode(vector)
+        else:
+            d_vector = vector
+
+        predict_id = self.matrix_serializer.ann_model.predict(d_vector.reshape(1, -1))[0]
+
+        cluster_id_sorted.remove(predict_id)
+        cluster_id_sorted.insert(0, predict_id)
 
         for cluster_id in cluster_id_sorted:
             batch_query(cid=cluster_id, sort=False)
 
             if len(all_index) >= k:
                 break
```

### Comparing `minvectordb-0.3.1/min_vec/storage_layer/storage.py` & `minvectordb-0.3.2/min_vec/storage_layer/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from pathlib import Path
 import json
 
 import numpy as np
+import portalocker
 from spinesUtils.asserts import raise_if
 
 from min_vec.computational_layer.engines import to_normalize
 from min_vec.configs.config import config
 from min_vec.structures.limited_dict import LimitedDict
 
 
 class StorageWorker:
     """The worker class for reading and writing data to the files."""
 
-    def __init__(self, collection_path, dimension, chunk_size, quantizer=None, warm_up=False):
+    def __init__(self, collection_path, dimension, chunk_size, warm_up=False):
         self.collection_path = Path(collection_path)
         self.collection_chunk_path = self.collection_path / 'chunk_data'
         self.collection_chunk_indices_path = self.collection_path / 'chunk_indices_data'
 
         self.collection_cluster_path = self.collection_path / 'cluster_data'
         self.collection_cluster_indices_path = self.collection_path / 'cluster_indices_data'
 
@@ -27,19 +28,22 @@
         self.dimension = dimension
         self.chunk_size = chunk_size
 
         self.cluster_last_file_shape = {}
 
         self.cache = LimitedDict(max_size=config.MVDB_DATALOADER_BUFFER_SIZE)
 
-        self.quantizer = quantizer
+        self.quantizer = None
 
         if warm_up:
             self.warm_up()
 
+    def update_quantizer(self, quantizer):
+        self.quantizer = quantizer
+
     def file_exists(self):
         return ((self.collection_chunk_path / 'chunk_0').exists()
                 or (self.collection_cluster_path / 'cluster_0_0').exists())
 
     def warm_up(self):
         """Load the data from the file to the memory."""
         if not self.file_exists():
@@ -104,34 +108,36 @@
         if filename in self.cache:
             return self._return_if_in_memory(filename)
         else:
             return self._load_data(filename, data_path, indices_path)
 
     def get_last_id(self, contains='chunk', cluster_id=None):
         if contains == 'chunk':
-            ids = [int(str(i).split('_')[-1])
+            ids = [int(i.stem.split('_')[-1])
                    for i in self.collection_chunk_path.glob('chunk_*')]
         else:
-            ids = [int(str(i).split('_')[-1])
+            ids = [int(i.stem.split('_')[-1])
                    for i in self.collection_cluster_path.glob(f'cluster_{cluster_id}_*')]
 
         if len(ids) > 0:
             return max(ids)
 
         return -1
 
     @staticmethod
     def _write_to_disk(data, indices, data_path, indices_path, filename):
         with open(data_path / filename, 'wb') as f:
+            portalocker.lock(f, portalocker.LOCK_EX)
             np.save(f, data)
 
         with open(indices_path / filename, 'wb') as f:
+            portalocker.lock(f, portalocker.LOCK_EX)
             np.save(f, indices)
 
-    def _write(self, data, indices, write_type='chunk', cluster_id=None, normalize=False):
+    def _incremental_write(self, data, indices, write_type='chunk', cluster_id=None, normalize=False):
         if normalize:
             data = to_normalize(np.vstack(data))
 
         if write_type == 'chunk':
             collection_subfile_path = self.collection_chunk_path
             collection_indices_path = self.collection_chunk_indices_path
             file_prefix = 'chunk'
@@ -141,17 +147,19 @@
 
             file_prefix = f'cluster_{cluster_id}'
 
         last_file_id = self.get_last_id(contains=write_type, cluster_id=cluster_id)
         # read info file to get the shape of the data
         # file shape
         if write_type == 'chunk':
+            # save the total shape of the data
             if not (self.collection_path / 'info.json').exists():
                 total_shape = [0, self.dimension]
                 with open(self.collection_path / 'info.json', 'w') as f:
+                    portalocker.lock(f, portalocker.LOCK_EX)
                     json.dump({"total_shape": total_shape}, f)
             else:
                 with open(self.collection_path / 'info.json', 'r') as f:
                     total_shape = json.load(f)['total_shape']
 
             # in this class, we only use the quantizer in chunk_write, after quantization,
             # the disk data and memory data will be changed to quantized data
@@ -226,39 +234,45 @@
                     self._write_to_disk(temp_data, temp_indices, collection_subfile_path,
                                         collection_indices_path, filename)
 
                     self._write_to_memory(filename, temp_data, temp_indices)
 
         if write_type == 'chunk':
             with open(self.collection_path / 'info.json', 'w') as f:
+                portalocker.lock(f, portalocker.LOCK_EX)
                 total_shape[0] += data_shape
                 json.dump({"total_shape": total_shape}, f)
         else:
             self.cluster_last_file_shape[cluster_id] = [data_shape + total_shape[0], self.dimension]
 
-    def cluster_write(self, cluster_id, data, indices, normalize=False):
-        """Write the data to the file."""
-        self._write(data, indices, write_type='cluster', cluster_id=cluster_id, normalize=normalize)
+    def _overwrite(self, filename, normalize=False):
+        """only use in chunk write"""
+        data, indices = self._read(filename)
 
-    def chunk_write(self, data, indices, normalize=False):
-        """Write the data to the file."""
-        self._write(data, indices, write_type='chunk', normalize=normalize)
+        if normalize:
+            data = to_normalize(data)
+
+        if self.quantizer is not None:
+            data = self.quantizer.fit_transform(data)
+
+        self._write_to_disk(data, indices, self.collection_chunk_path, self.collection_chunk_indices_path, filename)
+        self._write_to_memory(filename, data, indices)
 
     def read(self, filename):
         """Read the data from the file."""
         return self._read(filename=filename)
 
-    def write(self, data, indices, write_type='chunk', cluster_id=None, normalize=False):
+    def write(self, data=None, indices=None, write_type='chunk', cluster_id=None, normalize=False, filename=None):
         """Write the data to the file."""
-        if write_type == 'chunk':
-            self.chunk_write(data, indices, normalize=normalize)
-        elif write_type == 'cluster':
-            raise_if(ValueError, not isinstance(cluster_id, str) and not cluster_id.isdigit(),
-                     "cluster_id must be string-type integer.")
-            self.cluster_write(cluster_id, data, indices, normalize=normalize)
+        if write_type in ['chunk', 'cluster']:
+            if filename:
+                self._overwrite(filename, normalize=normalize)
+            else:
+                self._incremental_write(data, indices, write_type=write_type, cluster_id=cluster_id,
+                                        normalize=normalize)
         else:
             raise ValueError('write_type must be "chunk" or "cluster"')
 
     def get_shape(self, read_type='all'):
         """Get the shape of the data.
         parameters:
             read_type (str): The type of data to read. Must be 'chunk' or 'cluster' or 'all'.
@@ -344,14 +358,15 @@
                 continue
 
             index = np.where(indices == by_indices)[0][0]
             _data[index] = data
 
             with open(self.collection_chunk_path / path if read_type == 'chunk'
                       else self.collection_cluster_path / path, 'wb') as f:
+                portalocker.lock(f, portalocker.LOCK_EX)
                 np.save(f, _data)
 
             # delete cache
             self.cache.pop(path, None)
 
             break
 
@@ -361,7 +376,25 @@
         self._modify_data(data, by_indices, read_type='cluster', cluster_id=cluster_id)
 
     def modify_chunk_data(self, data, by_indices):
         self._modify_data(data, by_indices, read_type='chunk')
 
     def clear_cache(self):
         self.cache.clear()
+
+    def move_all_files_to_chunk(self):
+        """Move all files to chunk."""
+        try:
+            last_id = self.get_last_id(contains='chunk')
+            for file in self.collection_cluster_path.glob('*'):
+                last_id += 1
+                new_file_path = self.collection_chunk_path / f'chunk_{last_id}'
+                file.rename(new_file_path)
+
+                indices_file = self.collection_cluster_indices_path / file.name
+                new_indices_path = self.collection_chunk_indices_path / f'chunk_{last_id}'
+                indices_file.rename(new_indices_path)
+
+                self.cache.pop(file.stem, None)
+                self.cluster_last_file_shape = {}
+        except Exception as e:
+            raise IOError(f"Error occurred: {e}")
```

### Comparing `minvectordb-0.3.1/min_vec/structures/fields_filter.py` & `minvectordb-0.3.2/min_vec/structures/fields_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import gzip
 import random
 from pathlib import Path
 
 import msgpack
 import cloudpickle
+import portalocker
 
 
 class SkipListNode:
     def __init__(self, key, level, data=None):
         self.key = key
         self.data = data
         self.forward = [None] * (level + 1)
@@ -145,19 +146,19 @@
             return matched
         else:
             return [(id, self.data_store[self.id_map[id]]) for id in matched]
 
     def save(self, filepath):
         """Save all data to a file with gzip compression."""
         try:
-            # 使用 msgpack 保存基础数据
             with gzip.open(filepath, 'wb') as f:
+                portalocker.lock(f, portalocker.LOCK_EX)
                 f.write(msgpack.packb([self.data_store, self.id_map, self.last_internal_id, self.data_to_internal_id]))
-            # 使用 cloudpickle 和 gzip 保存跳表对象
             with gzip.open(Path(filepath).parent / (Path(filepath).stem + '-obj.mvdb'), 'wb') as f:
+                portalocker.lock(f, portalocker.LOCK_EX)
                 cloudpickle.dump(self.index, f)
         except IOError as e:
             print(f"Error saving to file {filepath}: {e}")
 
     def load(self, filepath):
         """Load all data from a file with gzip decompression."""
         try:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `minvectordb-0.3.1/min_vec/structures/filter.py` & `minvectordb-0.3.2/min_vec/structures/filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,23 +62,23 @@
         return False
 
     def __hash__(self):
         return hash(self.key) + hash(self.matcher)
 
 
 class MatchID:
-    def __init__(self, indices: Union[list, np.ndarray]):
+    def __init__(self, ids: Union[list, np.ndarray]):
         """
         Initialize an MatchID instance.
             .. versionadded:: 0.3.0
 
         Parameters:
-            indices (list or np.ndarray): The indices to filter the numpy array.
+            ids (list or np.ndarray): The indices to filter the numpy array.
         """
-        self.indices = indices
+        self.indices = ids
 
     def match(self, array):
         """
         Filter the numpy array according to the specified indices.
 
         Parameters:
             array (np.ndarray): The numpy array to filter.
@@ -148,9 +148,25 @@
             any_pass = False
         else:
             must_pass = all(condition.evaluate(data) for condition in self.must) if self.must else True
             any_pass = any(condition.evaluate(data) for condition in self.any) if self.any else False
 
         return must_pass and (any_pass or not self.any)
 
+    def to_dict(self):
+        """
+        Convert the filter to a dictionary.
+
+        Returns:
+            dict: A dictionary representation of the filter.
+        """
+        return {
+            'must': [{'field': condition.key, 'operator': condition.matcher.comparator.__name__, 'value': condition.matcher.value}
+                     if isinstance(condition, FieldCondition) else {'ids': condition.matcher.indices}
+                     for condition in self.must] if self.must else None,
+            'any': [{'field': condition.key, 'operator': condition.matcher.comparator.__name__, 'value': condition.matcher.value}
+                    if isinstance(condition, FieldCondition) else {'ids': condition.matcher.indices}
+                    for condition in self.any] if self.any else None
+        }
+
     def __hash__(self):
         return hash((tuple(self.must), tuple(self.any)))
```

### Comparing `minvectordb-0.3.1/min_vec/structures/kmeans.py` & `minvectordb-0.3.2/min_vec/structures/kmeans.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import portalocker
 from sklearn.cluster import MiniBatchKMeans
 
 
 class BatchKMeans:
     def __init__(self, n_clusters, random_state=42, epochs=100, batch_size=1024):
         self.model = MiniBatchKMeans(n_clusters=n_clusters, random_state=random_state, max_iter=epochs,
                                      batch_size=batch_size, n_init='auto', reassignment_ratio=0)
@@ -29,15 +30,17 @@
             raise ValueError('The model is not fitted yet. Please call the fit method first.')
 
         return self.model.predict(X)
 
     def save(self, filename):
         import cloudpickle
 
-        cloudpickle.dump(self.model, open(filename, 'wb'))
+        with open(filename, 'wb') as f:
+            portalocker.lock(f, portalocker.LOCK_EX)
+            cloudpickle.dump(self.model, f)
 
     def load(self, filename):
         import cloudpickle
 
         self.model = cloudpickle.load(open(filename, 'rb'))
 
         return self
```

### Comparing `minvectordb-0.3.1/min_vec/structures/limited_dict.py` & `minvectordb-0.3.2/min_vec/structures/limited_dict.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.1/min_vec/structures/limited_sort.py` & `minvectordb-0.3.2/min_vec/structures/limited_sort.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,27 +51,29 @@
             idx_len = len(idx)
             self.similarities[:idx_len] = self.similarities[idx]
             self.indices[:idx_len] = self.indices[idx]
             self.matrix_subset[:idx_len] = self.matrix_subset[idx]
             self.current_length = idx_len
 
     def get_top_n(self, vector: np.ndarray, distance='cosine'):
-        if distance == 'cosine':
-            distance_func = cosine_distance
-        else:
-            distance_func = euclidean_distance
+        with self.lock:
+            if distance == 'cosine':
+                distance_func = cosine_distance
+            else:
+                distance_func = euclidean_distance
 
-        if self.scaler is None:
-            sim = distance_func(vector, self.matrix_subset[:self.current_length])
-        else:
-            decoded_vectors = self.scaler.decode(self.matrix_subset[:self.current_length])
-            sim = distance_func(vector, decoded_vectors)
+            if self.scaler is None:
+                sim = distance_func(vector, self.matrix_subset[:self.current_length])
+            else:
+                decoded_vectors = self.scaler.decode(self.matrix_subset[:self.current_length])
+                sim = distance_func(vector, decoded_vectors)
 
-        sorted_idx = np.argsort(-sim) if distance == 'cosine' else np.argsort(sim)
+            sorted_idx = np.argsort(-sim) if distance == 'cosine' else np.argsort(sim)
 
-        return self.indices[sorted_idx], sim[sorted_idx]
+            return self.indices[sorted_idx], sim[sorted_idx]
 
     def clear(self):
-        self.current_length = 0
-        self.similarities = np.empty(self.max_length, dtype=self.similarities.dtype)
-        self.indices = np.empty(self.max_length, dtype=self.indices.dtype)
-        self.matrix_subset = np.empty((self.max_length, self.dim), dtype=self.matrix_subset.dtype)
+        with self.lock:
+            self.current_length = 0
+            self.similarities = np.empty(self.max_length, dtype=self.similarities.dtype)
+            self.indices = np.empty(self.max_length, dtype=self.indices.dtype)
+            self.matrix_subset = np.empty((self.max_length, self.dim), dtype=self.matrix_subset.dtype)
```

### Comparing `minvectordb-0.3.1/min_vec/structures/scaler.py` & `minvectordb-0.3.2/min_vec/structures/scaler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """scaler.py - Scalar Quantization module"""
 import numpy as np
 import numexpr as ne
 import cloudpickle
+import portalocker
 
 from spinesUtils.asserts import raise_if
 
 
 class ScalarQuantization:
     bits_map = {8: np.uint8, 16: np.uint16, 32: np.uint32}
 
@@ -86,14 +87,15 @@
 
         return decoded
 
     def save(self, filepath):
         raise_if(ValueError, not self.fitted, 'The model must be fitted before saving.')
         try:
             with open(filepath, 'wb') as file:
+                portalocker.lock(file, portalocker.LOCK_EX)
                 cloudpickle.dump(self, file)
         except IOError as e:
             print(f"Error saving model: {e}")
 
     @staticmethod
     def load(filepath):
         try:
```

### Comparing `minvectordb-0.3.1/min_vec/utils/utils.py` & `minvectordb-0.3.2/min_vec/utils/utils.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.1/setup.py` & `minvectordb-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 reqs = read_requirements(Path('.').parent.joinpath("requirements.txt"))
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='MinVectorDB',
-    version="0.3.1",
-    description='MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed database'
-                'that offers clear and concise Python APIs, aimed at lowering the barrier to '
-                'the use of vector databases.',
+    version="0.3.2",
+    description='A pure Python-implemented, lightweight, server-optional, '
+                'multi-end compatible, vector database deployable locally or remotely.',
     keywords='vector database',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
```

### Comparing `minvectordb-0.3.1/test/test_hmvdb_initial.py` & `minvectordb-0.3.2/test/standard_tests/test_hmvdb_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 
 import numpy as np
 
-from test import MinVectorDB
+from test import MinVectorDBLocalClient
 
 
 def test_create_collection():
-    my_vec_db = MinVectorDB(root_path='my_vec_db')
+    my_vec_db = MinVectorDBLocalClient(root_path='my_vec_db')
     collection = my_vec_db.require_collection('test_collection', dim=4, drop_if_exists=True)
 
     assert Path(collection._database_path).stem == 'test_collection'
     assert collection._matrix_serializer.dim == 4
     assert collection._matrix_serializer.chunk_size == 100000
     assert collection._matrix_serializer.dtypes == np.float32
     assert Path('my_vec_db/test_collection').exists()
@@ -19,27 +19,27 @@
     assert not Path('my_vec_db/test_collection').exists()
 
     my_vec_db.drop_database()
     assert not Path('my_vec_db').exists()
 
 
 def test_show_collections():
-    my_vec_db = MinVectorDB(root_path='my_vec_db')
+    my_vec_db = MinVectorDBLocalClient(root_path='my_vec_db')
     collection = my_vec_db.require_collection('test_collection', dim=4, drop_if_exists=True)
 
     collections = my_vec_db.show_collections()
     assert collections == ['test_collection']
 
     my_vec_db.drop_collection('test_collection')
     my_vec_db.drop_database()
     assert not Path('my_vec_db').exists()
 
 
 def test_get_an_exists_collection():
-    my_vec_db = MinVectorDB(root_path='my_vec_db')
+    my_vec_db = MinVectorDBLocalClient(root_path='my_vec_db')
     collection = my_vec_db.require_collection('test_collection', dim=4, drop_if_exists=True)
 
     collection = my_vec_db.get_collection('test_collection')
     assert Path(collection._database_path).stem == 'test_collection'
 
     my_vec_db.drop_collection('test_collection')
     my_vec_db.drop_database()
```

### Comparing `minvectordb-0.3.1/test/test_http_api.py` & `minvectordb-0.3.2/test/standard_tests/test_http_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,58 +41,82 @@
 def test_add_item(test_client):
     url = 'http://localhost:7637/add_item'
     data = {
         "collection_name": "example_collection",
         "item": {
             "vector": [0.1, 0.2, 0.3, 0.4],
             "id": 1,
-            "fields": {
+            "field": {
                 "name": "example",
                 "age": 18
             }
         }
     }
     response = test_client.post(url, json=data)
     print(response.json)
     assert response.status_code == 200
     assert response.json == {"status": "success", "params":
         {"collection_name": "example_collection", "item":
-            {"vector": [0.1, 0.2, 0.3, 0.4], "id": 1, "fields": {"name": "example", "age": 18}}}}
+            {"vector": [0.1, 0.2, 0.3, 0.4], "id": 1, "field": {"name": "example", "age": 18}}}}
+
+    url = 'http://localhost:7637/commit'
+    data = {
+        "collection_name": "example_collection"
+    }
+    response = test_client.post(url, json=data)
+    assert response.status_code == 200
+    assert response.json == {"status": "success", "params": {"collection_name": "example_collection"}}
 
 
 def test_bulk_add_items(test_client):
     url = 'http://localhost:7637/bulk_add_items'
     data = {
         "collection_name": "example_collection",
         "items": [
             {
                 "vector": [0.1, 0.4, 0.3, 0.6],
                 "id": 2,
-                "fields": {
+                "field": {
                     "name": "example2",
                     "age": 18
                 }
             },
             {
                 "vector": [0.2, 0.3, 0.4, 0.5],
                 "id": 3,
-                "fields": {
+                "field": {
                     "name": "example3",
                     "age": 19
                 }
             }
         ]
     }
     response = test_client.post(url, json=data)
+
     assert response.status_code == 200
-    assert response.json == {"status": "success", "params":
-        {"collection_name": "example_collection", "items": [
-            {"vector": [0.1, 0.4, 0.3, 0.6], "id": 2, "fields": {"name": "example2", "age": 18}},
-            {"vector": [0.2, 0.3, 0.4, 0.5], "id": 3, "fields": {"name": "example3", "age": 19}}
-        ]}}
+    assert response.json == {
+        "status": "success", "params":
+            {
+                "collection_name": "example_collection",
+                "ids": [2, 3],
+                "items": [
+                    {"vector": [0.1, 0.4, 0.3, 0.6], "id": 2, "field": {"name": "example2", "age": 18}},
+                    {"vector": [0.2, 0.3, 0.4, 0.5], "id": 3, "field": {"name": "example3", "age": 19}}
+                ]
+            }
+    }
+
+    url = 'http://localhost:7637/commit'
+    data = {
+        "collection_name": "example_collection"
+    }
+    response = test_client.post(url, json=data)
+    assert response.status_code == 200
+    assert response.json == {"status": "success", "params": {"collection_name": "example_collection"}}
+
 
 
 def test_collection_shape(test_client):
     url = 'http://localhost:7637/collection_shape'
     data = {
         "collection_name": "example_collection"
     }
@@ -166,8 +190,8 @@
     assert response.json == {"status": "success"}
 
 
 def test_database_exists(test_client):
     url = 'http://localhost:7637/database_exists'
     response = test_client.get(url)
     assert response.status_code == 200
-    assert response.json == {"status": "success", "params": {"exists": True}}
+    assert response.json == {"status": "success", "params": {"exists": False}}
```

### Comparing `minvectordb-0.3.1/test/test_smvdb_initial.py` & `minvectordb-0.3.2/test/standard_tests/test_smvdb_initial.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.1/test/test_smvdb_save_and_query.py` & `minvectordb-0.3.2/test/standard_tests/test_smvdb_save_and_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,7 +446,37 @@
 
         index, score = db.query(query, k=10)
 
         assert len(index) == len(score) == 10
         assert index[0] == 0
 
         db.delete()
+
+
+def test_refit(capsys):
+    db = StandaloneMinVectorDB(dim=1024, database_path='test_min_vec', chunk_size=10000, index_mode='IVF-FLAT')
+    with db.insert_session():
+        for i in range(100000):
+            db.add_item(np.random.rand(1024), id=i)
+
+    out, err = capsys.readouterr()
+
+    assert 'Start to fit the index for cluster' in err
+    assert db._matrix_serializer.ann_model.fitted
+
+    with db.insert_session():
+        for i in range(100000, 110000):
+            db.add_item(np.random.rand(1024), id=i)
+
+    out, err = capsys.readouterr()
+    assert 'Incrementally building the index for cluster' in err
+    assert db._matrix_serializer.ann_model.fitted
+
+    with db.insert_session():
+        for i in range(110000, 200000):
+            db.add_item(np.random.rand(1024), id=i)
+
+    out, err = capsys.readouterr()
+    assert 'Refitting the index for cluster' in err
+    assert db._matrix_serializer.ann_model.fitted
+
+    db.delete()
```

