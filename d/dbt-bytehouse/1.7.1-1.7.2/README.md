# Comparing `tmp/dbt-bytehouse-1.7.1.tar.gz` & `tmp/dbt-bytehouse-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-bytehouse-1.7.1.tar", last modified: Mon Apr 22 06:29:25 2024, max compression
+gzip compressed data, was "dbt-bytehouse-1.7.2.tar", last modified: Fri Apr 26 06:38:39 2024, max compression
```

## Comparing `dbt-bytehouse-1.7.1.tar` & `dbt-bytehouse-1.7.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.554251 dbt-bytehouse-1.7.1/
--rw-r--r--   0 bytedance   (501) staff       (20)    11451 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/LICENSE
--rw-r--r--   0 bytedance   (501) staff       (20)    20624 2024-04-22 06:29:25.553814 dbt-bytehouse-1.7.1/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)    19501 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/README.md
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.532251 dbt-bytehouse-1.7.1/dbt/
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.531889 dbt-bytehouse-1.7.1/dbt/adapters/
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.540881 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/
--rw-r--r--   0 bytedance   (501) staff       (20)     1229 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      681 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/__version__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4847 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/column.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5147 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/connections.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2819 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/credentials.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3042 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/dbclient.py
--rw-r--r--   0 bytedance   (501) staff       (20)    14888 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/impl.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11128 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/nativeclient.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2325 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/relation.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.532492 dbt-bytehouse-1.7.1/dbt/include/
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.542031 dbt-bytehouse-1.7.1/dbt/include/bytehouse/
--rw-r--r--   0 bytedance   (501) staff       (20)      715 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)       80 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/dbt_project.yml
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.544041 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.545243 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters/
--rw-r--r--   0 bytedance   (501) staff       (20)     1120 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters/apply_grants.sql
--rw-r--r--   0 bytedance   (501) staff       (20)     1534 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters/relation.sql
--rw-r--r--   0 bytedance   (501) staff       (20)     4956 2024-04-18 02:42:07.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters.sql
--rw-r--r--   0 bytedance   (501) staff       (20)     1686 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/catalog.sql
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.548554 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/
--rw-r--r--   0 bytedance   (501) staff       (20)     8057 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/incremental.sql
--rw-r--r--   0 bytedance   (501) staff       (20)     2137 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/seed.sql
--rw-r--r--   0 bytedance   (501) staff       (20)     3834 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/snapshot.sql
--rw-r--r--   0 bytedance   (501) staff       (20)     7180 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/table.sql
--rw-r--r--   0 bytedance   (501) staff       (20)     1111 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/test.sql
--rw-r--r--   0 bytedance   (501) staff       (20)     3315 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/view.sql
--rw-r--r--   0 bytedance   (501) staff       (20)     1537 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/persist_docs.sql
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.549250 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/schema_tests/
--rw-r--r--   0 bytedance   (501) staff       (20)     1095 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/schema_tests/relationships.sql
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.550525 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/utils/
--rw-r--r--   0 bytedance   (501) staff       (20)      660 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/utils/datatypes.sql
--rw-r--r--   0 bytedance   (501) staff       (20)     2223 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/utils/utils.sql
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.553211 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)    20624 2024-04-22 06:29:25.000000 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)     1350 2024-04-22 06:29:25.000000 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2024-04-22 06:29:25.000000 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       49 2024-04-22 06:29:25.000000 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/requires.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        4 2024-04-22 06:29:25.000000 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)      367 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/pyproject.toml
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2024-04-22 06:29:25.554302 dbt-bytehouse-1.7.1/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)     3203 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.220895 dbt-bytehouse-1.7.2/
+-rw-r--r--   0 bytedance   (501) staff       (20)    11451 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/LICENSE
+-rw-r--r--   0 bytedance   (501) staff       (20)    19115 2024-04-26 06:38:39.220519 dbt-bytehouse-1.7.2/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)    18086 2024-04-22 08:52:27.000000 dbt-bytehouse-1.7.2/README.md
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.192993 dbt-bytehouse-1.7.2/dbt/
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.192682 dbt-bytehouse-1.7.2/dbt/adapters/
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.208343 dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1229 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      681 2024-04-26 06:36:46.000000 dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/__version__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4847 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/column.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5147 2024-04-25 06:59:45.000000 dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/connections.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2819 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/credentials.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3042 2024-04-25 06:59:45.000000 dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/dbclient.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    13557 2024-04-26 06:36:46.000000 dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/impl.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6454 2024-04-26 06:36:46.000000 dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/nativeclient.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2325 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/relation.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.193216 dbt-bytehouse-1.7.2/dbt/include/
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.209307 dbt-bytehouse-1.7.2/dbt/include/bytehouse/
+-rw-r--r--   0 bytedance   (501) staff       (20)      715 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)       80 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/dbt_project.yml
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.210979 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.212245 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/adapters/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1120 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/adapters/apply_grants.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     1787 2024-04-26 06:36:46.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/adapters/relation.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     5476 2024-04-26 06:36:46.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/adapters.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     1968 2024-04-26 06:36:46.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/catalog.sql
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.216359 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/
+-rw-r--r--   0 bytedance   (501) staff       (20)     8061 2024-04-26 06:36:46.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/incremental.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     2134 2024-04-26 06:36:46.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/seed.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     3834 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/snapshot.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     7188 2024-04-26 06:36:46.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/table.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     1111 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/test.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     3315 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/view.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     1537 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/persist_docs.sql
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.216881 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/schema_tests/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1095 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/schema_tests/relationships.sql
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.217817 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/utils/
+-rw-r--r--   0 bytedance   (501) staff       (20)      660 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/utils/datatypes.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     2227 2024-04-26 06:36:46.000000 dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/utils/utils.sql
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-26 06:38:39.220039 dbt-bytehouse-1.7.2/dbt_bytehouse.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)    19115 2024-04-26 06:38:39.000000 dbt-bytehouse-1.7.2/dbt_bytehouse.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)     1350 2024-04-26 06:38:39.000000 dbt-bytehouse-1.7.2/dbt_bytehouse.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2024-04-26 06:38:39.000000 dbt-bytehouse-1.7.2/dbt_bytehouse.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       49 2024-04-26 06:38:39.000000 dbt-bytehouse-1.7.2/dbt_bytehouse.egg-info/requires.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        4 2024-04-26 06:38:39.000000 dbt-bytehouse-1.7.2/dbt_bytehouse.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)      367 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.2/pyproject.toml
+-rw-r--r--   0 bytedance   (501) staff       (20)       38 2024-04-26 06:38:39.220953 dbt-bytehouse-1.7.2/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)     3203 2024-04-24 11:24:12.000000 dbt-bytehouse-1.7.2/setup.py
```

### Comparing `dbt-bytehouse-1.7.1/LICENSE` & `dbt-bytehouse-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/PKG-INFO` & `dbt-bytehouse-1.7.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,1289 +1,1131 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6462 742d  : 2.1.Name: dbt-
-00000020: 6279 7465 686f 7573 650a 5665 7273 696f  bytehouse.Versio
-00000030: 6e3a 2031 2e37 2e31 0a53 756d 6d61 7279  n: 1.7.1.Summary
-00000040: 3a20 5468 6520 4279 7465 486f 7573 6520  : The ByteHouse 
-00000050: 706c 7567 696e 2066 6f72 2064 6274 2028  plugin for dbt (
-00000060: 6461 7461 2062 7569 6c64 2074 6f6f 6c29  data build tool)
-00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
-00000080: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-00000090: 7974 6568 6f75 7365 2d63 6c6f 7564 2f62  ytehouse-cloud/b
-000000a0: 7974 6568 6f75 7365 2d64 6274 0a41 7574  ytehouse-dbt.Aut
-000000b0: 686f 723a 2052 6166 7361 6e20 4d61 7a75  hor: Rafsan Mazu
-000000c0: 6d64 6572 0a41 7574 686f 722d 656d 6169  mder.Author-emai
-000000d0: 6c3a 2072 6166 7361 6e2e 6d61 7a75 6d64  l: rafsan.mazumd
-000000e0: 6572 4062 7974 6564 616e 6365 2e63 6f6d  er@bytedance.com
-000000f0: 0a4c 6963 656e 7365 3a20 4d49 540a 5072  .License: MIT.Pr
-00000100: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
-00000110: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
-00000120: 2f2f 6769 7468 7562 2e63 6f6d 2f62 7974  //github.com/byt
-00000130: 6568 6f75 7365 2d63 6c6f 7564 2f62 7974  ehouse-cloud/byt
-00000140: 6568 6f75 7365 2d64 6274 0a50 726f 6a65  ehouse-dbt.Proje
-00000150: 6374 2d55 524c 3a20 4368 616e 6765 732c  ct-URL: Changes,
-00000160: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000170: 636f 6d2f 6279 7465 686f 7573 652d 636c  com/bytehouse-cl
-00000180: 6f75 642f 6279 7465 686f 7573 652d 6462  oud/bytehouse-db
-00000190: 742f 626c 6f62 2f6d 6169 6e2f 4348 414e  t/blob/main/CHAN
-000001a0: 4745 4c4f 472e 6d64 0a4b 6579 776f 7264  GELOG.md.Keyword
-000001b0: 733a 2042 7974 6548 6f75 7365 2064 6274  s: ByteHouse dbt
-000001c0: 2063 6f6e 6e65 6374 6f72 0a50 6c61 7466   connector.Platf
-000001d0: 6f72 6d3a 2061 6e79 0a43 6c61 7373 6966  orm: any.Classif
-000001e0: 6965 723a 2044 6576 656c 6f70 6d65 6e74  ier: Development
-000001f0: 2053 7461 7475 7320 3a3a 2035 202d 2050   Status :: 5 - P
-00000200: 726f 6475 6374 696f 6e2f 5374 6162 6c65  roduction/Stable
-00000210: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
-00000220: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000230: 6f76 6564 203a 3a20 4170 6163 6865 2053  oved :: Apache S
-00000240: 6f66 7477 6172 6520 4c69 6365 6e73 650a  oftware License.
-00000250: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000260: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000270: 4d69 6372 6f73 6f66 7420 3a3a 2057 696e  Microsoft :: Win
-00000280: 646f 7773 0a43 6c61 7373 6966 6965 723a  dows.Classifier:
-00000290: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000002a0: 6d20 3a3a 204d 6163 4f53 203a 3a20 4d61  m :: MacOS :: Ma
-000002b0: 634f 5320 580a 436c 6173 7369 6669 6572  cOS X.Classifier
-000002c0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-000002d0: 656d 203a 3a20 504f 5349 5820 3a3a 204c  em :: POSIX :: L
-000002e0: 696e 7578 0a43 6c61 7373 6966 6965 723a  inux.Classifier:
-000002f0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000300: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000310: 3a3a 2033 2e37 0a43 6c61 7373 6966 6965  :: 3.7.Classifie
-00000320: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000330: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000340: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
-00000350: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000360: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000370: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
-00000380: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000390: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000003a0: 7974 686f 6e20 3a3a 2033 2e31 300a 5265  ython :: 3.10.Re
-000003b0: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
-000003c0: 3d33 2e37 0a44 6573 6372 6970 7469 6f6e  =3.7.Description
-000003d0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-000003e0: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
-000003f0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-00000400: 5345 0a52 6571 7569 7265 732d 4469 7374  SE.Requires-Dist
-00000410: 3a20 6462 742d 636f 7265 7e3d 312e 372e  : dbt-core~=1.7.
-00000420: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
-00000430: 2062 7974 6568 6f75 7365 2d64 7269 7665   bytehouse-drive
-00000440: 720a 5265 7175 6972 6573 2d44 6973 743a  r.Requires-Dist:
-00000450: 2070 7974 686f 6e2d 6461 7465 7574 696c   python-dateutil
-00000460: 0a0a 2320 496e 7472 6f64 7563 7469 6f6e  ..# Introduction
-00000470: 0a60 6462 7460 2028 4461 7461 2042 7569  .`dbt` (Data Bui
-00000480: 6c64 696e 6720 546f 6f6c 2920 6973 2061  lding Tool) is a
-00000490: 6e20 6f70 656e 2073 6f75 7263 6520 746f  n open source to
-000004a0: 6f6c 2074 6861 7420 656e 6162 6c65 7320  ol that enables 
-000004b0: 6461 7461 2061 6e61 6c79 7374 7320 616e  data analysts an
-000004c0: 6420 656e 6769 6e65 6572 7320 746f 2074  d engineers to t
-000004d0: 7261 6e73 666f 726d 0a64 6174 6120 696e  ransform.data in
-000004e0: 2074 6865 6972 2077 6172 6568 6f75 7365   their warehouse
-000004f0: 7320 7369 6d70 6c79 2062 7920 7772 6974  s simply by writ
-00000500: 696e 6720 7365 6c65 6374 2073 7461 7465  ing select state
-00000510: 6d65 6e74 732e 2060 6462 7460 2070 6572  ments. `dbt` per
-00000520: 666f 726d 7320 7468 6520 5420 2854 7261  forms the T (Tra
-00000530: 6e73 666f 726d 2920 6f66 2045 544c 2061  nsform) of ETL a
-00000540: 6e64 0a61 6c6c 6f77 7320 636f 6d70 616e  nd.allows compan
-00000550: 6965 7320 746f 2077 7269 7465 2074 7261  ies to write tra
-00000560: 6e73 666f 726d 6174 696f 6e73 2061 7320  nsformations as 
-00000570: 7175 6572 6965 7320 616e 6420 6f72 6368  queries and orch
-00000580: 6573 7472 6174 6520 7468 656d 2069 6e20  estrate them in 
-00000590: 6120 6d6f 7265 2065 6666 6963 6965 6e74  a more efficient
-000005a0: 2077 6179 2e20 0a42 7974 6548 6f75 7365   way. .ByteHouse
-000005b0: 2064 6274 2063 6f6e 6e65 6374 6f72 2069   dbt connector i
-000005c0: 7320 6120 706c 7567 696e 2065 6e61 626c  s a plugin enabl
-000005d0: 696e 6720 7573 6572 7320 746f 2062 7569  ing users to bui
-000005e0: 6c64 2074 6865 6972 2064 6174 6120 7761  ld their data wa
-000005f0: 7265 686f 7573 6520 6563 6f73 7973 7465  rehouse ecosyste
-00000600: 6d20 7769 7468 2064 6274 200a 616e 6420  m with dbt .and 
-00000610: 4279 7465 486f 7573 652e 200a 2320 5461  ByteHouse. .# Ta
-00000620: 626c 6520 6f66 2043 6f6e 7465 6e74 730a  ble of Contents.
-00000630: 2d20 5b49 6e74 726f 6475 6374 696f 6e5d  - [Introduction]
-00000640: 2823 696e 7472 6f64 7563 7469 6f6e 290a  (#introduction).
-00000650: 2d20 5b52 6571 7569 7265 6d65 6e74 735d  - [Requirements]
-00000660: 2823 7265 7175 6972 656d 656e 7473 290a  (#requirements).
-00000670: 2d20 5b43 7265 6174 696e 6720 4279 7465  - [Creating Byte
-00000680: 486f 7573 6520 4163 636f 756e 745d 2823  House Account](#
-00000690: 6372 6561 7469 6e67 2d62 7974 6568 6f75  creating-bytehou
-000006a0: 7365 2d61 6363 6f75 6e74 290a 2d20 5b49  se-account).- [I
-000006b0: 6e73 7461 6c6c 6174 696f 6e5d 2823 696e  nstallation](#in
-000006c0: 7374 616c 6c61 7469 6f6e 290a 2d20 5b64  stallation).- [d
-000006d0: 6274 2050 726f 6a65 6374 2053 6574 7570  bt Project Setup
-000006e0: 5d28 2364 6274 2d70 726f 6a65 6374 2d73  ](#dbt-project-s
-000006f0: 6574 7570 290a 2020 2a20 5b64 6274 5f70  etup).  * [dbt_p
-00000700: 726f 6a65 6374 2e79 6d6c 5d28 2364 6274  roject.yml](#dbt
-00000710: 2d70 726f 6a65 6374 796d 6c29 0a20 202a  -projectyml).  *
-00000720: 205b 7072 6f66 696c 6573 2e79 6d6c 5d28   [profiles.yml](
-00000730: 2370 726f 6669 6c65 7379 6d6c 290a 2020  #profilesyml).  
-00000740: 2a20 5b43 6f6e 6e65 6374 696f 6e20 2620  * [Connection & 
-00000750: 4175 7468 656e 7469 6361 7469 6f6e 2043  Authentication C
-00000760: 6f6e 6669 6775 7261 7469 6f6e 735d 2823  onfigurations](#
-00000770: 636f 6e6e 6563 7469 6f6e 2d2d 2d61 7574  connection---aut
-00000780: 6865 6e74 6963 6174 696f 6e2d 636f 6e66  hentication-conf
-00000790: 6967 7572 6174 696f 6e73 290a 2020 2020  igurations).    
-000007a0: 2b20 5b42 7974 6548 6f75 7365 2052 6567  + [ByteHouse Reg
-000007b0: 696f 6e73 5d28 2362 7974 6568 6f75 7365  ions](#bytehouse
-000007c0: 2d72 6567 696f 6e73 290a 2020 2020 2b20  -regions).    + 
-000007d0: 5b52 6567 696f 6e20 2620 5061 7373 776f  [Region & Passwo
-000007e0: 7264 2043 6f6e 6669 6775 7261 7469 6f6e  rd Configuration
-000007f0: 5d28 2372 6567 696f 6e2d 2d2d 7061 7373  ](#region---pass
-00000800: 776f 7264 2d63 6f6e 6669 6775 7261 7469  word-configurati
-00000810: 6f6e 290a 2020 2020 2b20 5b52 6567 696f  on).    + [Regio
-00000820: 6e20 2620 4150 4920 4b65 7920 436f 6e66  n & API Key Conf
-00000830: 6967 7572 6174 696f 6e5d 2823 7265 6769  iguration](#regi
-00000840: 6f6e 2d2d 2d61 7069 2d6b 6579 2d63 6f6e  on---api-key-con
-00000850: 6669 6775 7261 7469 6f6e 290a 2020 2020  figuration).    
-00000860: 2b20 5b48 6f73 7420 4164 6472 6573 7320  + [Host Address 
-00000870: 2620 5061 7373 776f 7264 2043 6f6e 6669  & Password Confi
-00000880: 6775 7261 7469 6f6e 5d28 2368 6f73 742d  guration](#host-
-00000890: 6164 6472 6573 732d 2d2d 7061 7373 776f  address---passwo
-000008a0: 7264 2d63 6f6e 6669 6775 7261 7469 6f6e  rd-configuration
-000008b0: 290a 2020 2020 2b20 5b48 6f73 7420 4164  ).    + [Host Ad
-000008c0: 6472 6573 7320 2620 4150 4920 4b65 7920  dress & API Key 
-000008d0: 436f 6e66 6967 7572 6174 696f 6e5d 2823  Configuration](#
-000008e0: 686f 7374 2d61 6464 7265 7373 2d2d 2d61  host-address---a
-000008f0: 7069 2d6b 6579 2d63 6f6e 6669 6775 7261  pi-key-configura
-00000900: 7469 6f6e 290a 2020 2a20 5b50 726f 6a65  tion).  * [Proje
-00000910: 6374 2049 6e69 7469 616c 697a 6174 696f  ct Initializatio
-00000920: 6e5d 2823 7072 6f6a 6563 742d 696e 6974  n](#project-init
-00000930: 6961 6c69 7a61 7469 6f6e 290a 2020 2a20  ialization).  * 
-00000940: 5b54 6573 7420 5761 7265 686f 7573 6520  [Test Warehouse 
-00000950: 436f 6e6e 6563 7469 6f6e 5d28 2374 6573  Connection](#tes
-00000960: 742d 7761 7265 686f 7573 652d 636f 6e6e  t-warehouse-conn
-00000970: 6563 7469 6f6e 290a 2d20 5b44 6174 6173  ection).- [Datas
-00000980: 6574 2049 6e67 6573 7469 6f6e 5d28 2364  et Ingestion](#d
-00000990: 6174 6173 6574 2d69 6e67 6573 7469 6f6e  ataset-ingestion
-000009a0: 290a 2d20 5b64 6274 204d 6f64 656c 735d  ).- [dbt Models]
-000009b0: 2823 6462 742d 6d6f 6465 6c73 290a 2d20  (#dbt-models).- 
-000009c0: 5b73 6368 656d 612e 796d 6c5d 2823 7363  [schema.yml](#sc
-000009d0: 6865 6d61 796d 6c29 0a2d 205b 4d61 7465  hemayml).- [Mate
-000009e0: 7269 616c 697a 6174 696f 6e20 7479 7065  rialization type
-000009f0: 7320 6f66 204d 6f64 656c 735d 2823 6d61  s of Models](#ma
-00000a00: 7465 7269 616c 697a 6174 696f 6e2d 7479  terialization-ty
-00000a10: 7065 732d 6f66 2d6d 6f64 656c 7329 0a20  pes-of-models). 
-00000a20: 202a 205b 5669 6577 204d 6174 6572 6961   * [View Materia
-00000a30: 6c69 7a61 7469 6f6e 735d 2823 7669 6577  lizations](#view
-00000a40: 2d6d 6174 6572 6961 6c69 7a61 7469 6f6e  -materialization
-00000a50: 7329 0a20 202a 205b 5461 626c 6520 4d61  s).  * [Table Ma
-00000a60: 7465 7269 616c 697a 6174 696f 6e73 5d28  terializations](
-00000a70: 2374 6162 6c65 2d6d 6174 6572 6961 6c69  #table-materiali
-00000a80: 7a61 7469 6f6e 7329 0a20 202a 205b 496e  zations).  * [In
-00000a90: 6372 656d 656e 7461 6c20 4d61 7465 7269  cremental Materi
-00000aa0: 616c 697a 6174 696f 6e73 5d28 2369 6e63  alizations](#inc
-00000ab0: 7265 6d65 6e74 616c 2d6d 6174 6572 6961  remental-materia
-00000ac0: 6c69 7a61 7469 6f6e 7329 0a20 2020 202b  lizations).    +
-00000ad0: 205b 486f 7720 6974 2077 6f72 6b73 5d28   [How it works](
-00000ae0: 2368 6f77 2d69 742d 776f 726b 7329 0a2d  #how-it-works).-
-00000af0: 205b 5072 6f6a 6563 7420 446f 6375 6d65   [Project Docume
-00000b00: 6e74 6174 696f 6e5d 2823 7072 6f6a 6563  ntation](#projec
-00000b10: 742d 646f 6375 6d65 6e74 6174 696f 6e29  t-documentation)
-00000b20: 0a2d 205b 4c6f 6361 6c20 4465 7665 6c6f  .- [Local Develo
-00000b30: 706d 656e 745d 2823 6c6f 6361 6c2d 6465  pment](#local-de
-00000b40: 7665 6c6f 706d 656e 7429 0a2d 205b 4f72  velopment).- [Or
-00000b50: 6967 696e 616c 2041 7574 686f 725d 2823  iginal Author](#
-00000b60: 6f72 6967 696e 616c 2d61 7574 686f 7229  original-author)
-00000b70: 0a2d 205b 4c69 6365 6e73 655d 2823 6c69  .- [License](#li
-00000b80: 6365 6e73 6529 0a23 2052 6571 7569 7265  cense).# Require
-00000b90: 6d65 6e74 730a 4d61 6b65 2073 7572 6520  ments.Make sure 
-00000ba0: 796f 7520 6861 7665 2060 6462 7460 2026  you have `dbt` &
-00000bb0: 2060 7079 7468 6f6e 6020 696e 7374 616c   `python` instal
-00000bc0: 6c65 6420 6f6e 2079 6f75 7220 6d61 6368  led on your mach
-00000bd0: 696e 652e 2049 6620 6e6f 742c 2074 6865  ine. If not, the
-00000be0: 6e20 796f 7520 6361 6e20 666f 6c6c 6f77  n you can follow
-00000bf0: 2074 6869 7320 6775 6964 6520 6874 7470   this guide http
-00000c00: 733a 2f2f 646f 6373 2e67 6574 6462 742e  s://docs.getdbt.
-00000c10: 636f 6d2f 646f 6373 2f67 6574 2d73 7461  com/docs/get-sta
-00000c20: 7274 6564 2f69 6e73 7461 6c6c 6174 696f  rted/installatio
-00000c30: 6e0a 2d20 6462 7420 7631 2e37 2e30 206f  n.- dbt v1.7.0 o
-00000c40: 7220 6772 6561 7465 720a 2d20 7079 7468  r greater.- pyth
-00000c50: 6f6e 2076 332e 3720 6f72 2067 7265 6174  on v3.7 or great
-00000c60: 6572 0a23 2043 7265 6174 696e 6720 4279  er.# Creating By
-00000c70: 7465 486f 7573 6520 4163 636f 756e 740a  teHouse Account.
-00000c80: 596f 7520 6e65 6564 2074 6f20 6372 6561  You need to crea
-00000c90: 7465 2042 7974 6548 6f75 7365 2061 6363  te ByteHouse acc
-00000ca0: 6f75 6e74 2069 6e20 6f72 6465 7220 746f  ount in order to
-00000cb0: 2075 7365 2062 7974 6568 6f75 7365 2d64   use bytehouse-d
-00000cc0: 6274 2063 6f6e 6e65 6374 6f72 2e20 596f  bt connector. Yo
-00000cd0: 7520 6361 6e20 7369 6d70 6c79 2063 7265  u can simply cre
-00000ce0: 6174 6520 6120 6672 6565 2061 6363 6f75  ate a free accou
-00000cf0: 6e74 2077 6974 680a 7468 6520 7072 6f63  nt with.the proc
-00000d00: 6573 7320 6d65 6e74 696f 6e65 6420 696e  ess mentioned in
-00000d10: 206f 7572 206f 6666 6963 6961 6c20 7765   our official we
-00000d20: 6273 6974 6520 646f 6375 6d65 6e74 6174  bsite documentat
-00000d30: 696f 6e3a 2068 7474 7073 3a2f 2f64 6f63  ion: https://doc
-00000d40: 732e 6279 7465 686f 7573 652e 636c 6f75  s.bytehouse.clou
-00000d50: 642f 656e 2f64 6f63 732f 7175 6963 6b2d  d/en/docs/quick-
-00000d60: 7374 6172 7420 3c62 722f 3e0a 0a59 6f75  start <br/>..You
-00000d70: 2063 616e 2061 6c73 6f20 6372 6561 7465   can also create
-00000d80: 2042 7974 6548 6f75 7365 2061 6363 6f75   ByteHouse accou
-00000d90: 6e74 2074 6872 6f75 6768 2056 6f6c 6361  nt through Volca
-00000da0: 6e6f 2045 6e67 696e 6520 6279 2042 7974  no Engine by Byt
-00000db0: 6544 616e 6365 3a20 0a68 7474 7073 3a2f  eDance: .https:/
-00000dc0: 2f77 7777 2e76 6f6c 6365 6e67 696e 652e  /www.volcengine.
-00000dd0: 636f 6d2f 7072 6f64 7563 742f 6279 7465  com/product/byte
-00000de0: 686f 7573 652d 636c 6f75 6420 0a23 2049  house-cloud .# I
-00000df0: 6e73 7461 6c6c 6174 696f 6e0a 4372 6561  nstallation.Crea
-00000e00: 7465 2061 206e 6577 2072 6570 6f73 6974  te a new reposit
-00000e10: 6f72 7920 7768 6572 6520 7765 2077 696c  ory where we wil
-00000e20: 6c20 696e 7374 616e 7469 6174 6520 6120  l instantiate a 
-00000e30: 6050 7974 686f 6e60 2076 6972 7475 616c  `Python` virtual
-00000e40: 2065 6e76 6972 6f6e 6d65 6e74 2e0a 6060   environment..``
-00000e50: 6063 6f6d 6d61 6e64 6c69 6e65 0a6d 6b64  `commandline.mkd
-00000e60: 6972 2064 6274 5f62 7974 6568 6f75 7365  ir dbt_bytehouse
-00000e70: 5f64 656d 6f0a 6364 2064 6274 5f62 7974  _demo.cd dbt_byt
-00000e80: 6568 6f75 7365 5f64 656d 6f0a 0a70 7974  ehouse_demo..pyt
-00000e90: 686f 6e20 2d6d 2076 656e 7620 7665 6e76  hon -m venv venv
-00000ea0: 0a73 6f75 7263 6520 7665 6e76 2f62 696e  .source venv/bin
-00000eb0: 2f61 6374 6976 6174 650a 6060 600a 4c61  /activate.```.La
-00000ec0: 7465 7374 2072 656c 6561 7365 2076 6572  test release ver
-00000ed0: 7369 6f6e 2063 616e 2062 6520 696e 7374  sion can be inst
-00000ee0: 616c 6c65 6420 6672 6f6d 2068 6572 653a  alled from here:
-00000ef0: 0a60 6060 636f 6d6d 616e 646c 696e 650a  .```commandline.
-00000f00: 7069 7020 696e 7374 616c 6c20 6462 742d  pip install dbt-
-00000f10: 6279 7465 686f 7573 650a 6060 600a 4375  bytehouse.```.Cu
-00000f20: 7272 656e 7420 6465 7665 6c6f 706d 656e  rrent developmen
-00000f30: 7420 7665 7273 696f 6e20 6361 6e20 6265  t version can be
-00000f40: 2069 6e73 7461 6c6c 6564 2066 726f 6d20   installed from 
-00000f50: 6865 7265 3a0a 6060 6063 6f6d 6d61 6e64  here:.```command
-00000f60: 6c69 6e65 0a70 6970 2069 6e73 7461 6c6c  line.pip install
-00000f70: 2067 6974 2b68 7474 7073 3a2f 2f67 6974   git+https://git
-00000f80: 6875 622e 636f 6d2f 6279 7465 686f 7573  hub.com/bytehous
-00000f90: 652d 636c 6f75 642f 6279 7465 686f 7573  e-cloud/bytehous
-00000fa0: 652d 6462 7440 6d61 7374 6572 2365 6767  e-dbt@master#egg
-00000fb0: 3d62 7974 6568 6f75 7365 2d64 7269 7665  =bytehouse-drive
-00000fc0: 720a 6060 600a 4368 6563 6b20 7768 6574  r.```.Check whet
-00000fd0: 6865 7220 696e 7374 616c 6c61 7469 6f6e  her installation
-00000fe0: 2069 7320 7375 6363 6573 7366 756c 2062   is successful b
-00000ff0: 7920 7665 7269 6679 696e 6720 6279 7465  y verifying byte
-00001000: 686f 7573 6520 6973 2061 7661 696c 6162  house is availab
-00001010: 6c65 2075 6e64 6572 2050 6c75 6769 6e73  le under Plugins
-00001020: 2e0a 6060 6063 6f6d 6d61 6e64 6c69 6e65  ..```commandline
-00001030: 0a64 6274 202d 2d76 6572 7369 6f6e 0a60  .dbt --version.`
-00001040: 6060 0a21 5b56 6572 7369 6f6e 5d28 2e2f  ``.![Version](./
-00001050: 6578 616d 706c 6573 2f31 5f76 6572 7369  examples/1_versi
-00001060: 6f6e 2e70 6e67 290a 2320 6462 7420 5072  on.png).# dbt Pr
-00001070: 6f6a 6563 7420 5365 7475 700a 2323 2064  oject Setup.## d
-00001080: 6274 5f70 726f 6a65 6374 2e79 6d6c 0a45  bt_project.yml.E
-00001090: 7665 7279 2060 6462 7460 2070 726f 6a65  very `dbt` proje
-000010a0: 6374 206e 6565 6473 2061 2060 6462 745f  ct needs a `dbt_
-000010b0: 7072 6f6a 6563 742e 796d 6c60 2066 696c  project.yml` fil
-000010c0: 6520 e280 9420 7468 6973 2069 7320 686f  e ... this is ho
-000010d0: 7720 6064 6274 6020 6b6e 6f77 7320 6120  w `dbt` knows a 
-000010e0: 6469 7265 6374 6f72 7920 6973 2061 2060  directory is a `
-000010f0: 6462 7460 2070 726f 6a65 6374 2e20 6064  dbt` project. `d
-00001100: 6274 5f70 726f 6a65 6374 2e79 6d6c 600a  bt_project.yml`.
-00001110: 6669 6c65 2068 6f6c 6473 2074 6865 2063  file holds the c
-00001120: 6f6e 7465 7874 206f 6620 796f 7572 2070  ontext of your p
-00001130: 726f 6a65 6374 2061 6e64 2074 656c 6c73  roject and tells
-00001140: 2060 6462 7460 2068 6f77 2074 6f20 6275   `dbt` how to bu
-00001150: 696c 6420 796f 7572 2064 6174 6120 7365  ild your data se
-00001160: 7473 2e20 536f 6d65 2063 6f6d 6d6f 6e20  ts. Some common 
-00001170: 636f 6e66 6967 7572 6174 696f 6e73 0a66  configurations.f
-00001180: 6f72 2060 6462 745f 7072 6f6a 6563 742e  or `dbt_project.
-00001190: 796d 6c60 2061 7265 3a0a 3c74 6162 6c65  yml` are:.<table
-000011a0: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-000011b0: 2020 203c 7464 3e59 414d 4c20 6b65 793c     <td>YAML key<
-000011c0: 2f74 643e 0a20 2020 2020 2020 203c 7464  /td>.        <td
-000011d0: 3e56 616c 7565 3c2f 7464 3e0a 2020 2020  >Value</td>.    
-000011e0: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
-000011f0: 2020 2020 2020 203c 7464 3e6e 616d 653c         <td>name<
-00001200: 2f74 643e 0a20 2020 2020 2020 203c 7464  /td>.        <td
-00001210: 3e59 6f75 7220 7072 6f6a 6563 74e2 8099  >Your project...
-00001220: 7320 6e61 6d65 2069 6e20 736e 616b 6520  s name in snake 
-00001230: 6361 7365 3c2f 7464 3e0a 2020 2020 3c2f  case</td>.    </
-00001240: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
-00001250: 2020 2020 203c 7464 3e76 6572 7369 6f6e       <td>version
-00001260: 3c2f 7464 3e0a 2020 2020 2020 2020 3c74  </td>.        <t
-00001270: 643e 5665 7273 696f 6e20 6f66 2079 6f75  d>Version of you
-00001280: 7220 7072 6f6a 6563 743c 2f74 643e 0a20  r project</td>. 
-00001290: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
-000012a0: 3e0a 2020 2020 2020 2020 3c74 643e 7072  >.        <td>pr
-000012b0: 6f66 696c 653c 2f74 643e 0a20 2020 2020  ofile</td>.     
-000012c0: 2020 203c 7464 3e54 6865 2070 726f 6669     <td>The profi
-000012d0: 6c65 2064 6274 2075 7365 7320 746f 2063  le dbt uses to c
-000012e0: 6f6e 6e65 6374 2074 6f20 4279 7465 486f  onnect to ByteHo
-000012f0: 7573 653c 2f74 643e 0a20 2020 203c 2f74  use</td>.    </t
-00001300: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
-00001310: 2020 2020 3c74 643e 6d6f 6465 6c2d 7061      <td>model-pa
-00001320: 7468 733c 2f74 643e 0a20 2020 2020 2020  ths</td>.       
-00001330: 203c 7464 3e44 6972 6563 746f 7269 6573   <td>Directories
-00001340: 2074 6f20 7768 6572 6520 796f 7572 206d   to where your m
-00001350: 6f64 656c 2061 6e64 2073 6f75 7263 6520  odel and source 
-00001360: 6669 6c65 7320 6c69 7665 3c2f 7464 3e0a  files live</td>.
-00001370: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
-00001380: 723e 0a20 2020 2020 2020 203c 7464 3e73  r>.        <td>s
-00001390: 6565 642d 7061 7468 733c 2f74 643e 0a20  eed-paths</td>. 
-000013a0: 2020 2020 2020 203c 7464 3e44 6972 6563         <td>Direc
-000013b0: 746f 7269 6573 2074 6f20 7768 6572 6520  tories to where 
-000013c0: 796f 7572 2073 6565 6420 6669 6c65 7320  your seed files 
-000013d0: 6c69 7665 3c2f 7464 3e0a 2020 2020 3c2f  live</td>.    </
-000013e0: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
-000013f0: 2020 2020 203c 7464 3e74 6573 742d 7061       <td>test-pa
-00001400: 7468 733c 2f74 643e 0a20 2020 2020 2020  ths</td>.       
-00001410: 203c 7464 3e44 6972 6563 746f 7269 6573   <td>Directories
-00001420: 2074 6f20 7768 6572 6520 796f 7572 2074   to where your t
-00001430: 6573 7420 6669 6c65 7320 6c69 7665 3c2f  est files live</
-00001440: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
-00001450: 2020 3c74 723e 0a20 2020 2020 2020 203c    <tr>.        <
-00001460: 7464 3e73 6e61 7073 686f 742d 7061 7468  td>snapshot-path
-00001470: 733c 2f74 643e 0a20 2020 2020 2020 203c  s</td>.        <
-00001480: 7464 3e44 6972 6563 746f 7269 6573 2074  td>Directories t
-00001490: 6f20 7768 6572 6520 796f 7572 2073 6e61  o where your sna
-000014a0: 7073 686f 7473 206c 6976 653c 2f74 643e  pshots live</td>
-000014b0: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
-000014c0: 7472 3e0a 2020 2020 2020 2020 3c74 643e  tr>.        <td>
-000014d0: 646f 6373 2d70 6174 6873 3c2f 7464 3e0a  docs-paths</td>.
-000014e0: 2020 2020 2020 2020 3c74 643e 4469 7265          <td>Dire
-000014f0: 6374 6f72 6965 7320 746f 2077 6865 7265  ctories to where
-00001500: 2079 6f75 7220 646f 6373 2062 6c6f 636b   your docs block
-00001510: 7320 6c69 7665 3c2f 7464 3e0a 2020 2020  s live</td>.    
-00001520: 3c2f 7472 3e0a 3c2f 7461 626c 653e 0a0a  </tr>.</table>..
-00001530: 2323 2070 726f 6669 6c65 732e 796d 6c0a  ## profiles.yml.
-00001540: 5768 656e 2079 6f75 2069 6e76 6f6b 6520  When you invoke 
-00001550: 6064 6274 6020 6672 6f6d 2074 6865 2063  `dbt` from the c
-00001560: 6f6d 6d61 6e64 206c 696e 652c 2060 6462  ommand line, `db
-00001570: 7460 2070 6172 7365 7320 796f 7572 2060  t` parses your `
-00001580: 6462 745f 7072 6f6a 6563 742e 796d 6c60  dbt_project.yml`
-00001590: 2061 6e64 206f 6274 6169 6e73 2074 6865   and obtains the
-000015a0: 2070 726f 6669 6c65 206e 616d 652e 2060   profile name. `
-000015b0: 6462 7460 2074 6865 6e20 0a63 6865 636b  dbt` then .check
-000015c0: 7320 796f 7572 2060 7072 6f66 696c 6573  s your `profiles
-000015d0: 2e79 6d6c 6020 6669 6c65 2066 6f72 2061  .yml` file for a
-000015e0: 2070 726f 6669 6c65 2077 6974 6820 7468   profile with th
-000015f0: 6520 7361 6d65 206e 616d 652e 2041 2070  e same name. A p
-00001600: 726f 6669 6c65 2063 6f6e 7461 696e 7320  rofile contains 
-00001610: 616c 6c20 7468 6520 6465 7461 696c 732f  all the details/
-00001620: 6372 6564 656e 7469 616c 7320 0a72 6571  credentials .req
-00001630: 7569 7265 6420 746f 2063 6f6e 6e65 6374  uired to connect
-00001640: 2074 6f20 4279 7465 486f 7573 652e 2060   to ByteHouse. `
-00001650: 6462 7460 2077 696c 6c20 7365 6172 6368  dbt` will search
-00001660: 2074 6865 2063 7572 7265 6e74 2077 6f72   the current wor
-00001670: 6b69 6e67 2064 6972 6563 746f 7279 2066  king directory f
-00001680: 6f72 2074 6865 2060 7072 6f66 696c 6573  or the `profiles
-00001690: 2e79 6d6c 6020 6669 6c65 2061 6e64 2077  .yml` file and w
-000016a0: 696c 6c0a 6465 6661 756c 7420 746f 2074  ill.default to t
-000016b0: 6865 2060 7e2f 2e64 6274 2f20 6469 7265  he `~/.dbt/ dire
-000016c0: 6374 6f72 7960 2069 6620 6e6f 7420 666f  ctory` if not fo
-000016d0: 756e 642e 0a60 6060 7961 6d6c 0a3c 7072  und..```yaml.<pr
-000016e0: 6f66 696c 652d 6e61 6d65 3e3a 0a20 2074  ofile-name>:.  t
-000016f0: 6172 6765 743a 203c 7461 7267 6574 2d6e  arget: <target-n
-00001700: 616d 653e 0a20 206f 7574 7075 7473 3a0a  ame>.  outputs:.
-00001710: 2020 2020 3c74 6172 6765 742d 6e61 6d65      <target-name
-00001720: 3e3a 0a20 2020 2020 2074 7970 653a 2062  >:.      type: b
-00001730: 7974 6568 6f75 7365 0a20 2020 2020 2073  ytehouse.      s
-00001740: 6368 656d 613a 203c 6461 7461 6261 7365  chema: <database
-00001750: 2d6e 616d 653e 0a20 2020 2020 2075 7365  -name>.      use
-00001760: 723a 203c 7573 6572 6e61 6d65 3e0a 2020  r: <username>.  
-00001770: 2020 2020 7061 7373 776f 7264 3a20 3c70      password: <p
-00001780: 6173 7377 6f72 643e 0a20 2020 2020 2064  assword>.      d
-00001790: 7269 7665 723a 206e 6174 6976 650a 2020  river: native.  
-000017a0: 2020 2020 236f 7074 696f 6e61 6c20 6669      #optional fi
-000017b0: 656c 6473 0a20 2020 2020 2068 6f73 743a  elds.      host:
-000017c0: 203c 686f 7374 6e61 6d65 3e0a 2020 2020   <hostname>.    
-000017d0: 2020 706f 7274 3a20 3c70 6f72 743e 0a20    port: <port>. 
-000017e0: 2020 2020 2072 6567 696f 6e3a 203c 7265       region: <re
-000017f0: 6769 6f6e 2d6e 616d 653e 0a20 2020 2020  gion-name>.     
-00001800: 2061 6363 6f75 6e74 3a20 3c61 6363 6f75   account: <accou
-00001810: 6e74 2d6e 616d 653e 0a20 2020 2020 2077  nt-name>.      w
-00001820: 6172 6568 6f75 7365 3a20 3c77 6172 6568  arehouse: <wareh
-00001830: 6f75 7365 2d6e 616d 653e 0a20 2020 2020  ouse-name>.     
-00001840: 2072 6574 7269 6573 3a20 310a 2020 2020   retries: 1.    
-00001850: 2020 7365 6375 7265 3a20 5472 7565 0a20    secure: True. 
-00001860: 2020 2020 2063 6f6e 6e65 6374 5f74 696d       connect_tim
-00001870: 656f 7574 3a20 3130 0a20 2020 2020 2073  eout: 10.      s
-00001880: 656e 645f 7265 6365 6976 655f 7469 6d65  end_receive_time
-00001890: 6f75 743a 2033 3030 0a20 2020 2020 2063  out: 300.      c
-000018a0: 7573 746f 6d5f 7365 7474 696e 6773 3a20  ustom_settings: 
-000018b0: 3c65 6d70 7479 3e0a 6060 600a 3c74 6162  <empty>.```.<tab
-000018c0: 6c65 3e0a 2020 2020 3c74 723e 0a20 2020  le>.    <tr>.   
-000018d0: 2020 2020 203c 7464 3e59 414d 4c20 6b65       <td>YAML ke
-000018e0: 793c 2f74 643e 0a20 2020 2020 2020 203c  y</td>.        <
-000018f0: 7464 3e56 616c 7565 3c2f 7464 3e0a 2020  td>Value</td>.  
-00001900: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
-00001910: 0a20 2020 2020 2020 203c 7464 3e26 6c74  .        <td>&lt
-00001920: 3b70 726f 6669 6c65 2d6e 616d 6526 6774  ;profile-name&gt
-00001930: 3b3c 2f74 643e 0a20 2020 2020 2020 203c  ;</td>.        <
-00001940: 7464 3e4e 616d 6520 6f66 2074 6865 2070  td>Name of the p
-00001950: 726f 6669 6c65 2e20 4861 7320 746f 2062  rofile. Has to b
-00001960: 6520 7468 6520 7361 6d65 206e 616d 6520  e the same name 
-00001970: 6173 2074 6865 2070 726f 6669 6c65 2069  as the profile i
-00001980: 6e64 6963 6174 6564 2069 6e20 796f 7572  ndicated in your
-00001990: 2064 6274 5f70 726f 6a65 6374 2e79 6d6c   dbt_project.yml
-000019a0: 2066 696c 653c 2f74 643e 0a20 2020 203c   file</td>.    <
-000019b0: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
-000019c0: 2020 2020 2020 3c74 643e 7461 7267 6574        <td>target
-000019d0: 3c2f 7464 3e0a 2020 2020 2020 2020 3c74  </td>.        <t
-000019e0: 643e 4465 6661 756c 7420 7461 7267 6574  d>Default target
-000019f0: 2079 6f75 7220 6462 7420 7072 6f6a 6563   your dbt projec
-00001a00: 7420 7769 6c6c 2075 7365 2e20 4974 206d  t will use. It m
-00001a10: 7573 7420 6265 206f 6e65 206f 6620 7468  ust be one of th
-00001a20: 6520 7461 7267 6574 7320 796f 7520 6465  e targets you de
-00001a30: 6669 6e65 2069 6e20 796f 7572 2070 726f  fine in your pro
-00001a40: 6669 6c65 3c2f 7464 3e0a 2020 2020 3c2f  file</td>.    </
-00001a50: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
-00001a60: 2020 2020 203c 7464 3e74 7970 653c 2f74       <td>type</t
-00001a70: 643e 0a20 2020 2020 2020 203c 7464 3e4d  d>.        <td>M
-00001a80: 7573 7420 6265 2073 6574 2074 6f20 6279  ust be set to by
-00001a90: 7465 686f 7573 653c 2f74 643e 0a20 2020  tehouse</td>.   
-00001aa0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
-00001ab0: 2020 2020 2020 2020 3c74 643e 7363 6865          <td>sche
-00001ac0: 6d61 3c2f 7464 3e0a 2020 2020 2020 2020  ma</td>.        
-00001ad0: 3c74 643e 4461 7461 6261 7365 206e 616d  <td>Database nam
-00001ae0: 653c 2f74 643e 0a20 2020 203c 2f74 723e  e</td>.    </tr>
-00001af0: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
-00001b00: 2020 3c74 643e 7573 6572 3c2f 7464 3e0a    <td>user</td>.
-00001b10: 2020 2020 2020 2020 3c74 643e 5573 6572          <td>User
-00001b20: 6e61 6d65 2077 6974 6820 6164 6571 7561  name with adequa
-00001b30: 7465 2070 6572 6d69 7373 696f 6e73 2074  te permissions t
-00001b40: 6f20 6163 6365 7373 2074 6865 2073 7065  o access the spe
-00001b50: 6369 6669 6564 2073 6368 656d 612e 2046  cified schema. F
-00001b60: 6f72 2041 5049 204b 6579 2061 7574 6865  or API Key authe
-00001b70: 6e74 6963 6174 696f 6e2c 2075 7365 7220  ntication, user 
-00001b80: 6d75 7374 2062 6520 7365 7420 746f 2062  must be set to b
-00001b90: 7974 6568 6f75 7365 3c2f 7464 3e0a 2020  ytehouse</td>.  
-00001ba0: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
-00001bb0: 0a20 2020 2020 2020 203c 7464 3e70 6173  .        <td>pas
-00001bc0: 7377 6f72 643c 2f74 643e 0a20 2020 2020  sword</td>.     
-00001bd0: 2020 203c 7464 3e54 6865 2070 6173 7377     <td>The passw
-00001be0: 6f72 6420 6173 736f 6369 6174 6564 2077  ord associated w
-00001bf0: 6974 6820 7468 6520 7370 6563 6966 6965  ith the specifie
-00001c00: 6420 7573 6572 3c2f 7464 3e0a 2020 2020  d user</td>.    
-00001c10: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
-00001c20: 2020 2020 2020 203c 7464 3e64 7269 7665         <td>drive
-00001c30: 723c 2f74 643e 0a20 2020 2020 2020 203c  r</td>.        <
-00001c40: 7464 3e4d 7573 7420 6265 2073 6574 2074  td>Must be set t
-00001c50: 6f20 6e61 7469 7665 3c2f 7464 3e0a 2020  o native</td>.  
-00001c60: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
-00001c70: 0a20 2020 2020 2020 203c 7464 3e68 6f73  .        <td>hos
-00001c80: 743c 2f74 643e 0a20 2020 2020 2020 203c  t</td>.        <
-00001c90: 7464 3e5b 4f70 7469 6f6e 616c 5d20 5468  td>[Optional] Th
-00001ca0: 6520 686f 7374 206e 616d 6520 6f66 2074  e host name of t
-00001cb0: 6865 2063 6f6e 6e65 6374 696f 6e3c 2f74  he connection</t
-00001cc0: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
-00001cd0: 203c 7472 3e0a 2020 2020 2020 2020 3c74   <tr>.        <t
-00001ce0: 643e 706f 7274 203c 2f74 643e 0a20 2020  d>port </td>.   
-00001cf0: 2020 2020 203c 7464 3e5b 4f70 7469 6f6e       <td>[Option
-00001d00: 616c 5d20 5468 6520 706f 7274 206e 756d  al] The port num
-00001d10: 6265 7220 6f66 2074 6865 2068 6f73 7420  ber of the host 
-00001d20: 7365 7276 6572 3c2f 7464 3e0a 2020 2020  server</td>.    
-00001d30: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
-00001d40: 2020 2020 2020 203c 7464 3e72 6567 696f         <td>regio
-00001d50: 6e3c 2f74 643e 0a20 2020 2020 2020 203c  n</td>.        <
-00001d60: 7464 3e5b 4f70 7469 6f6e 616c 5d20 416c  td>[Optional] Al
-00001d70: 6961 7320 666f 7220 686f 7374 2026 616d  ias for host &am
-00001d80: 703b 2070 6f72 7420 3c2f 7464 3e0a 2020  p; port </td>.  
-00001d90: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
-00001da0: 0a20 2020 2020 2020 203c 7464 3e61 6363  .        <td>acc
-00001db0: 6f75 6e74 3c2f 7464 3e0a 2020 2020 2020  ount</td>.      
-00001dc0: 2020 3c74 643e 5b4f 7074 696f 6e61 6c5d    <td>[Optional]
-00001dd0: 2042 7974 6548 6f75 7365 2061 6363 6f75   ByteHouse accou
-00001de0: 6e74 206e 756d 6265 723c 2f74 643e 0a20  nt number</td>. 
-00001df0: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
-00001e00: 3e0a 2020 2020 2020 2020 3c74 643e 7761  >.        <td>wa
-00001e10: 7265 686f 7573 653c 2f74 643e 0a20 2020  rehouse</td>.   
-00001e20: 2020 2020 203c 7464 3e5b 4f70 7469 6f6e       <td>[Option
-00001e30: 616c 5d20 5468 6520 6e61 6d65 206f 6620  al] The name of 
-00001e40: 7468 6520 7669 7274 7561 6c20 7761 7265  the virtual ware
-00001e50: 686f 7573 6520 7468 6174 2079 6f75 2077  house that you w
-00001e60: 616e 7420 746f 2075 7365 2066 6f72 2074  ant to use for t
-00001e70: 6869 7320 7365 7373 696f 6e3c 2f74 643e  his session</td>
-00001e80: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
-00001e90: 7472 3e0a 2020 2020 2020 2020 3c74 643e  tr>.        <td>
-00001ea0: 7265 7472 6965 733c 2f74 643e 0a20 2020  retries</td>.   
-00001eb0: 2020 2020 203c 7464 3e5b 4f70 7469 6f6e       <td>[Option
-00001ec0: 616c 5d20 4e75 6d62 6572 206f 6620 7469  al] Number of ti
-00001ed0: 6d65 7320 746f 2072 6574 7279 2074 6865  mes to retry the
-00001ee0: 2069 6e69 7469 616c 2063 6f6e 6e65 6374   initial connect
-00001ef0: 696f 6e20 6174 7465 6d70 7420 6966 2074  ion attempt if t
-00001f00: 6865 2065 7272 6f72 2061 7070 6561 7273  he error appears
-00001f10: 2074 6f20 6265 2072 6563 6f76 6572 6162   to be recoverab
-00001f20: 6c65 3c2f 7464 3e0a 2020 2020 3c2f 7472  le</td>.    </tr
-00001f30: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00001f40: 2020 203c 7464 3e73 6563 7572 653c 2f74     <td>secure</t
-00001f50: 643e 0a20 2020 2020 2020 203c 7464 3e5b  d>.        <td>[
-00001f60: 4f70 7469 6f6e 616c 5d20 5768 6574 6865  Optional] Whethe
-00001f70: 7220 7468 6520 636f 6e6e 6563 7469 6f6e  r the connection
-00001f80: 2069 7320 7365 6375 7265 6420 6279 2054   is secured by T
-00001f90: 4c53 2e20 5375 6767 6573 7465 6420 746f  LS. Suggested to
-00001fa0: 2073 6574 2069 7420 746f 2054 7275 653c   set it to True<
-00001fb0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
-00001fc0: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
-00001fd0: 3c74 643e 636f 6e6e 6563 745f 7469 6d65  <td>connect_time
-00001fe0: 6f75 743c 2f74 643e 0a20 2020 2020 2020  out</td>.       
-00001ff0: 203c 7464 3e5b 4f70 7469 6f6e 616c 5d20   <td>[Optional] 
-00002000: 436f 6e6e 6563 7469 6f6e 2074 696d 656f  Connection timeo
-00002010: 7574 2069 6e20 7365 636f 6e64 732e 2044  ut in seconds. D
-00002020: 6566 6175 6c74 2069 7320 3130 2073 6563  efault is 10 sec
-00002030: 6f6e 6473 3c2f 7464 3e0a 2020 2020 3c2f  onds</td>.    </
-00002040: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
-00002050: 2020 2020 203c 7464 3e73 656e 645f 7265       <td>send_re
-00002060: 6365 6976 655f 7469 6d65 6f75 743c 2f74  ceive_timeout</t
-00002070: 643e 0a20 2020 2020 2020 203c 7464 3e5b  d>.        <td>[
-00002080: 4f70 7469 6f6e 616c 5d20 5469 6d65 6f75  Optional] Timeou
-00002090: 7420 666f 7220 7265 6365 6976 696e 6720  t for receiving 
-000020a0: 6461 7461 2066 726f 6d20 6f72 2073 656e  data from or sen
-000020b0: 6469 6e67 2064 6174 6120 746f 2042 7974  ding data to Byt
-000020c0: 6548 6f75 7365 2e20 4465 6661 756c 7420  eHouse. Default 
-000020d0: 6973 2035 206d 696e 7574 6573 2028 3330  is 5 minutes (30
-000020e0: 3020 7365 636f 6e64 7329 3c2f 7464 3e0a  0 seconds)</td>.
-000020f0: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
-00002100: 723e 0a20 2020 2020 2020 203c 7464 3e63  r>.        <td>c
-00002110: 7573 746f 6d5f 7365 7474 696e 6773 3c2f  ustom_settings</
-00002120: 7464 3e0a 2020 2020 2020 2020 3c74 643e  td>.        <td>
-00002130: 5b4f 7074 696f 6e61 6c5d 2041 206d 6170  [Optional] A map
-00002140: 7069 6e67 206f 6620 4279 7465 486f 7573  ping of ByteHous
-00002150: 6520 7370 6563 6966 6963 2075 7365 7220  e specific user 
-00002160: 7365 7474 696e 6773 2074 6f20 7573 6520  settings to use 
-00002170: 7769 7468 2074 6865 2063 6f6e 6e65 6374  with the connect
-00002180: 696f 6e3c 2f74 643e 0a20 2020 203c 2f74  ion</td>.    </t
-00002190: 723e 0a3c 2f74 6162 6c65 3e0a 0a23 2320  r>.</table>..## 
-000021a0: 436f 6e6e 6563 7469 6f6e 2026 2041 7574  Connection & Aut
-000021b0: 6865 6e74 6963 6174 696f 6e20 436f 6e66  hentication Conf
-000021c0: 6967 7572 6174 696f 6e73 0a23 2323 2042  igurations.### B
-000021d0: 7974 6548 6f75 7365 2052 6567 696f 6e73  yteHouse Regions
-000021e0: 0a43 7572 7265 6e74 6c79 2c20 7468 6520  .Currently, the 
-000021f0: 6472 6976 6572 2073 7570 706f 7274 7320  driver supports 
-00002200: 7468 6520 666f 6c6c 6f77 696e 6720 7265  the following re
-00002210: 6769 6f6e 206e 616d 6573 2061 6372 6f73  gion names acros
-00002220: 7320 6469 6666 6572 656e 7420 636c 6f75  s different clou
-00002230: 6420 7072 6f76 6964 6572 732e 2041 6c74  d providers. Alt
-00002240: 6572 6e61 7469 7665 6c79 2c20 6966 2079  ernatively, if y
-00002250: 6f75 206b 6e6f 770a 7468 6520 686f 7374  ou know.the host
-00002260: 2061 6464 7265 7373 206f 6620 4279 7465   address of Byte
-00002270: 486f 7573 6520 7365 7276 6572 2c20 796f  House server, yo
-00002280: 7520 6361 6e20 6469 7265 6374 6c79 2075  u can directly u
-00002290: 7365 2068 6f73 7420 6164 6472 6573 7320  se host address 
-000022a0: 2620 6f6d 6974 2072 6567 696f 6e20 6e61  & omit region na
-000022b0: 6d65 2e0a 3c74 6162 6c65 3e0a 2020 2020  me..<table>.    
-000022c0: 3c74 723e 0a20 2020 2020 2020 203c 7464  <tr>.        <td
-000022d0: 3e52 6567 696f 6e20 4e61 6d65 3c2f 7464  >Region Name</td
-000022e0: 3e0a 2020 2020 2020 2020 3c74 643e 5461  >.        <td>Ta
-000022f0: 7267 6574 2053 6572 7665 723c 2f74 643e  rget Server</td>
-00002300: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
-00002310: 7472 3e0a 2020 2020 2020 2020 3c74 643e  tr>.        <td>
-00002320: 4150 2d53 4f55 5448 4541 5354 2d31 3c2f  AP-SOUTHEAST-1</
-00002330: 7464 3e0a 2020 2020 2020 2020 3c74 643e  td>.        <td>
-00002340: 6761 7465 7761 792e 6177 732d 6170 2d73  gateway.aws-ap-s
-00002350: 6f75 7468 6561 7374 2d31 2e62 7974 6568  outheast-1.byteh
-00002360: 6f75 7365 2e63 6c6f 7564 3a31 3930 3030  ouse.cloud:19000
-00002370: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
-00002380: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
-00002390: 203c 7464 3e56 4f4c 4341 4e4f 2d43 4e2d   <td>VOLCANO-CN-
-000023a0: 4e4f 5254 482d 313c 2f74 643e 0a20 2020  NORTH-1</td>.   
-000023b0: 2020 2020 203c 7464 3e62 7974 6568 6f75       <td>bytehou
-000023c0: 7365 2d63 6e2d 6265 696a 696e 672e 766f  se-cn-beijing.vo
-000023d0: 6c63 6573 2e63 6f6d 3a31 3930 3030 3c2f  lces.com:19000</
-000023e0: 7464 3e0a 2020 2020 3c2f 7472 3e0a 3c2f  td>.    </tr>.</
-000023f0: 7461 626c 653e 0a0a 2323 2320 5265 6769  table>..### Regi
-00002400: 6f6e 2026 2050 6173 7377 6f72 6420 436f  on & Password Co
-00002410: 6e66 6967 7572 6174 696f 6e0a 5265 7175  nfiguration.Requ
-00002420: 6972 6564 2070 6172 616d 6574 6572 733a  ired parameters:
-00002430: 2060 6163 636f 756e 7460 2060 7573 6572   `account` `user
-00002440: 6020 6070 6173 7377 6f72 6460 2060 7265  ` `password` `re
-00002450: 6769 6f6e 600a 6060 6079 616d 6c0a 6279  gion`.```yaml.by
-00002460: 7465 686f 7573 655f 7072 6f66 696c 653a  tehouse_profile:
-00002470: 0a20 2074 6172 6765 743a 2064 6576 0a20  .  target: dev. 
-00002480: 206f 7574 7075 7473 3a0a 2020 2020 6465   outputs:.    de
-00002490: 763a 0a20 2020 2020 2074 7970 653a 2062  v:.      type: b
-000024a0: 7974 6568 6f75 7365 0a20 2020 2020 2064  ytehouse.      d
-000024b0: 7269 7665 723a 206e 6174 6976 650a 0a20  river: native.. 
-000024c0: 2020 2020 2023 2064 6174 6162 6173 650a       # database.
-000024d0: 2020 2020 2020 7363 6865 6d61 3a20 2444        schema: $D
-000024e0: 4154 4142 4153 455f 4e41 4d45 0a0a 2020  ATABASE_NAME..  
-000024f0: 2020 2020 2320 7461 7267 6574 2073 6572      # target ser
-00002500: 7665 7220 6164 6472 6573 730a 2020 2020  ver address.    
-00002510: 2020 7265 6769 6f6e 3a20 2452 4547 494f    region: $REGIO
-00002520: 4e5f 4e41 4d45 0a0a 2020 2020 2020 2320  N_NAME..      # 
-00002530: 6163 636f 756e 7420 6372 6564 656e 7469  account credenti
-00002540: 616c 730a 2020 2020 2020 6163 636f 756e  als.      accoun
-00002550: 743a 2024 4143 434f 554e 545f 4e41 4d45  t: $ACCOUNT_NAME
-00002560: 0a20 2020 2020 2075 7365 723a 2024 5553  .      user: $US
-00002570: 4552 5f4e 414d 450a 2020 2020 2020 7061  ER_NAME.      pa
-00002580: 7373 776f 7264 3a20 2450 4153 5357 4f52  ssword: $PASSWOR
-00002590: 440a 0a20 2020 2020 2023 2061 6464 6974  D..      # addit
-000025a0: 696f 6e61 6c20 7365 7474 696e 6773 0a20  ional settings. 
-000025b0: 2020 2020 2073 6563 7572 653a 2054 7275       secure: Tru
-000025c0: 650a 6060 600a 2323 2320 5265 6769 6f6e  e.```.### Region
-000025d0: 2026 2041 5049 204b 6579 2043 6f6e 6669   & API Key Confi
-000025e0: 6775 7261 7469 6f6e 0a52 6571 7569 7265  guration.Require
-000025f0: 6420 7061 7261 6d65 7465 7273 3a20 6072  d parameters: `r
-00002600: 6567 696f 6e60 2060 7573 6572 6020 6070  egion` `user` `p
-00002610: 6173 7377 6f72 6460 0a60 6060 7961 6d6c  assword`.```yaml
-00002620: 0a62 7974 6568 6f75 7365 5f70 726f 6669  .bytehouse_profi
-00002630: 6c65 3a0a 2020 7461 7267 6574 3a20 6465  le:.  target: de
-00002640: 760a 2020 6f75 7470 7574 733a 0a20 2020  v.  outputs:.   
-00002650: 2064 6576 3a0a 2020 2020 2020 7479 7065   dev:.      type
-00002660: 3a20 6279 7465 686f 7573 650a 2020 2020  : bytehouse.    
-00002670: 2020 6472 6976 6572 3a20 6e61 7469 7665    driver: native
-00002680: 0a0a 2020 2020 2020 2320 6461 7461 6261  ..      # databa
-00002690: 7365 0a20 2020 2020 2073 6368 656d 613a  se.      schema:
-000026a0: 2024 4441 5441 4241 5345 5f4e 414d 450a   $DATABASE_NAME.
-000026b0: 0a20 2020 2020 2023 2074 6172 6765 7420  .      # target 
-000026c0: 7365 7276 6572 2061 6464 7265 7373 0a20  server address. 
-000026d0: 2020 2020 2072 6567 696f 6e3a 2024 5245       region: $RE
-000026e0: 4749 4f4e 5f4e 414d 450a 0a20 2020 2020  GION_NAME..     
-000026f0: 2023 2061 6363 6f75 6e74 2063 7265 6465   # account crede
-00002700: 6e74 6961 6c73 0a20 2020 2020 2075 7365  ntials.      use
-00002710: 723a 2062 7974 6568 6f75 7365 0a20 2020  r: bytehouse.   
-00002720: 2020 2070 6173 7377 6f72 643a 2024 4150     password: $AP
-00002730: 495f 4b45 590a 0a20 2020 2020 2023 2061  I_KEY..      # a
-00002740: 6464 6974 696f 6e61 6c20 7365 7474 696e  dditional settin
-00002750: 6773 0a20 2020 2020 2073 6563 7572 653a  gs.      secure:
-00002760: 2054 7275 650a 6060 600a 2323 2320 486f   True.```.### Ho
-00002770: 7374 2041 6464 7265 7373 2026 2050 6173  st Address & Pas
-00002780: 7377 6f72 6420 436f 6e66 6967 7572 6174  sword Configurat
-00002790: 696f 6e0a 5265 7175 6972 6564 2070 6172  ion.Required par
-000027a0: 616d 6574 6572 733a 2060 686f 7374 6020  ameters: `host` 
-000027b0: 6070 6f72 7460 2060 6163 636f 756e 7460  `port` `account`
-000027c0: 2060 7573 6572 6020 6070 6173 7377 6f72   `user` `passwor
-000027d0: 6460 0a60 6060 7961 6d6c 0a62 7974 6568  d`.```yaml.byteh
-000027e0: 6f75 7365 5f70 726f 6669 6c65 3a0a 2020  ouse_profile:.  
-000027f0: 7461 7267 6574 3a20 6465 760a 2020 6f75  target: dev.  ou
-00002800: 7470 7574 733a 0a20 2020 2064 6576 3a0a  tputs:.    dev:.
-00002810: 2020 2020 2020 7479 7065 3a20 6279 7465        type: byte
-00002820: 686f 7573 650a 2020 2020 2020 6472 6976  house.      driv
-00002830: 6572 3a20 6e61 7469 7665 0a0a 2020 2020  er: native..    
-00002840: 2020 2320 6461 7461 6261 7365 0a20 2020    # database.   
-00002850: 2020 2073 6368 656d 613a 2024 4441 5441     schema: $DATA
-00002860: 4241 5345 5f4e 414d 450a 0a20 2020 2020  BASE_NAME..     
-00002870: 2023 2074 6172 6765 7420 7365 7276 6572   # target server
-00002880: 2061 6464 7265 7373 0a20 2020 2020 2068   address.      h
-00002890: 6f73 743a 2024 484f 5354 5f41 4444 5245  ost: $HOST_ADDRE
-000028a0: 5353 2020 0a20 2020 2020 2070 6f72 743a  SS  .      port:
-000028b0: 2024 504f 5254 5f4e 554d 4245 520a 0a20   $PORT_NUMBER.. 
-000028c0: 2020 2020 2023 2061 6363 6f75 6e74 2063       # account c
-000028d0: 7265 6465 6e74 6961 6c73 0a20 2020 2020  redentials.     
-000028e0: 2061 6363 6f75 6e74 3a20 2441 4343 4f55   account: $ACCOU
-000028f0: 4e54 5f4e 414d 450a 2020 2020 2020 7573  NT_NAME.      us
-00002900: 6572 3a20 2455 5345 525f 4e41 4d45 0a20  er: $USER_NAME. 
-00002910: 2020 2020 2070 6173 7377 6f72 643a 2024       password: $
-00002920: 5041 5353 574f 5244 0a0a 2020 2020 2020  PASSWORD..      
-00002930: 2320 6164 6469 7469 6f6e 616c 2073 6574  # additional set
-00002940: 7469 6e67 730a 2020 2020 2020 7365 6375  tings.      secu
-00002950: 7265 3a20 5472 7565 0a60 6060 0a23 2323  re: True.```.###
-00002960: 2048 6f73 7420 4164 6472 6573 7320 2620   Host Address & 
-00002970: 4150 4920 4b65 7920 436f 6e66 6967 7572  API Key Configur
-00002980: 6174 696f 6e0a 5265 7175 6972 6564 2070  ation.Required p
-00002990: 6172 616d 6574 6572 733a 2060 686f 7374  arameters: `host
-000029a0: 6020 6070 6f72 7460 2060 7573 6572 6020  ` `port` `user` 
-000029b0: 6070 6173 7377 6f72 6460 0a60 6060 7961  `password`.```ya
-000029c0: 6d6c 0a62 7974 6568 6f75 7365 5f70 726f  ml.bytehouse_pro
-000029d0: 6669 6c65 3a0a 2020 7461 7267 6574 3a20  file:.  target: 
-000029e0: 6465 760a 2020 6f75 7470 7574 733a 0a20  dev.  outputs:. 
-000029f0: 2020 2064 6576 3a0a 2020 2020 2020 7479     dev:.      ty
-00002a00: 7065 3a20 6279 7465 686f 7573 650a 2020  pe: bytehouse.  
-00002a10: 2020 2020 6472 6976 6572 3a20 6e61 7469      driver: nati
-00002a20: 7665 0a0a 2020 2020 2020 2320 6461 7461  ve..      # data
-00002a30: 6261 7365 0a20 2020 2020 2073 6368 656d  base.      schem
-00002a40: 613a 2024 4441 5441 4241 5345 5f4e 414d  a: $DATABASE_NAM
-00002a50: 450a 0a20 2020 2020 2023 2074 6172 6765  E..      # targe
-00002a60: 7420 7365 7276 6572 2061 6464 7265 7373  t server address
-00002a70: 0a20 2020 2020 2068 6f73 743a 2024 484f  .      host: $HO
-00002a80: 5354 5f41 4444 5245 5353 2020 0a20 2020  ST_ADDRESS  .   
-00002a90: 2020 2070 6f72 743a 2024 504f 5254 5f4e     port: $PORT_N
-00002aa0: 554d 4245 520a 0a20 2020 2020 2023 2061  UMBER..      # a
-00002ab0: 6363 6f75 6e74 2063 7265 6465 6e74 6961  ccount credentia
-00002ac0: 6c73 0a20 2020 2020 2075 7365 723a 2062  ls.      user: b
-00002ad0: 7974 6568 6f75 7365 0a20 2020 2020 2070  ytehouse.      p
-00002ae0: 6173 7377 6f72 643a 2024 4150 495f 4b45  assword: $API_KE
-00002af0: 590a 0a20 2020 2020 2023 2061 6464 6974  Y..      # addit
-00002b00: 696f 6e61 6c20 7365 7474 696e 6773 0a20  ional settings. 
-00002b10: 2020 2020 2073 6563 7572 653a 2054 7275       secure: Tru
-00002b20: 650a 6060 600a 2323 2050 726f 6a65 6374  e.```.## Project
-00002b30: 2049 6e69 7469 616c 697a 6174 696f 6e0a   Initialization.
-00002b40: 6064 6274 2069 6e69 7460 2063 6f6d 6d61  `dbt init` comma
-00002b50: 6e64 2077 696c 6c20 7072 6f6d 7074 2066  nd will prompt f
-00002b60: 6f72 2070 726f 6a65 6374 206e 616d 6520  or project name 
-00002b70: 2620 6461 7461 6261 7365 2061 6461 7074  & database adapt
-00002b80: 6572 732c 2077 6865 7265 2079 6f75 2068  ers, where you h
-00002b90: 6176 6520 746f 2073 656c 6563 7420 6279  ave to select by
-00002ba0: 7465 686f 7573 652e 2054 6869 7320 7769  tehouse. This wi
-00002bb0: 6c6c 2063 7265 6174 650a 6120 6e65 7720  ll create.a new 
-00002bc0: 666f 6c64 6572 2077 6974 6820 796f 7572  folder with your
-00002bd0: 2070 726f 6a65 6374 206e 616d 652c 2073   project name, s
-00002be0: 616d 706c 6520 6669 6c65 7320 2620 6064  ample files & `d
-00002bf0: 6274 5f70 726f 6a65 6374 2e79 6d6c 6020  bt_project.yml` 
-00002c00: 636f 6e66 6967 2066 696c 652c 2065 6e6f  config file, eno
-00002c10: 7567 6820 746f 2067 6574 2079 6f75 2073  ugh to get you s
-00002c20: 7461 7274 6564 2077 6974 6820 6462 742e  tarted with dbt.
-00002c30: 0a60 6060 636f 6d6d 616e 646c 696e 650a  .```commandline.
-00002c40: 6462 7420 696e 6974 0a60 6060 0a21 5b49  dbt init.```.![I
-00002c50: 6e69 745d 282e 2f65 7861 6d70 6c65 732f  nit](./examples/
-00002c60: 325f 7072 6f66 696c 6573 2e70 6e67 290a  2_profiles.png).
-00002c70: 5570 6461 7465 2079 6f75 7220 7072 6f66  Update your prof
-00002c80: 696c 6573 2e79 6d6c 2077 6974 6820 7265  iles.yml with re
-00002c90: 7175 6972 6564 2061 7574 6865 6e74 6963  quired authentic
-00002ca0: 6174 696f 6e20 2620 7461 7267 6574 2073  ation & target s
-00002cb0: 6572 7665 7220 6372 6564 656e 7469 616c  erver credential
-00002cc0: 732e 200a 6060 6063 6f6d 6d61 6e64 6c69  s. .```commandli
-00002cd0: 6e65 0a6e 616e 6f20 7e2f 2e64 6274 2f70  ne.nano ~/.dbt/p
-00002ce0: 726f 6669 6c65 732e 796d 6c0a 6060 600a  rofiles.yml.```.
-00002cf0: 4173 2060 6462 7460 2068 6173 2063 7265  As `dbt` has cre
-00002d00: 6174 6564 2061 206e 6577 2066 6f6c 6465  ated a new folde
-00002d10: 7220 7769 7468 2074 6865 2073 616d 6520  r with the same 
-00002d20: 6e61 6d65 2061 7320 796f 7572 2070 726f  name as your pro
-00002d30: 6a65 6374 206e 616d 652c 2063 6861 6e67  ject name, chang
-00002d40: 6520 796f 7572 2063 7572 7265 6e74 200a  e your current .
-00002d50: 6469 7265 6374 6f72 7920 746f 2074 6865  directory to the
-00002d60: 2070 726f 6a65 6374 2066 6f6c 6465 722e   project folder.
-00002d70: 200a 6060 6063 6f6d 6d61 6e64 6c69 6e65   .```commandline
-00002d80: 0a63 6420 6462 745f 6279 7465 686f 7573  .cd dbt_bytehous
-00002d90: 655f 6465 6d6f 0a60 6060 0a55 7064 6174  e_demo.```.Updat
-00002da0: 6520 796f 7572 2060 6462 745f 7072 6f6a  e your `dbt_proj
-00002db0: 6563 742e 796d 6c60 2066 696c 6520 746f  ect.yml` file to
-00002dc0: 2068 6176 6520 7468 6520 7361 6d65 2070   have the same p
-00002dd0: 726f 6669 6c65 5f6e 616d 6520 6173 2060  rofile_name as `
-00002de0: 7e2f 2e64 6274 2f70 726f 6669 6c65 732e  ~/.dbt/profiles.
-00002df0: 796d 6c60 2e0a 6060 6063 6f6d 6d61 6e64  yml`..```command
-00002e00: 6c69 6e65 0a6e 616e 6f20 6462 745f 7072  line.nano dbt_pr
-00002e10: 6f6a 6563 742e 796d 6c0a 6060 600a 215b  oject.yml.```.![
-00002e20: 5072 6f6a 6563 745d 282e 2f65 7861 6d70  Project](./examp
-00002e30: 6c65 732f 335f 7072 6f6a 6563 742e 706e  les/3_project.pn
-00002e40: 6729 0a23 2320 5465 7374 2057 6172 6568  g).## Test Wareh
-00002e50: 6f75 7365 2043 6f6e 6e65 6374 696f 6e0a  ouse Connection.
-00002e60: 5573 6520 6064 6274 2064 6562 7567 6020  Use `dbt debug` 
-00002e70: 636f 6d6d 616e 6420 746f 2076 6572 6966  command to verif
-00002e80: 7920 7265 7175 6972 6564 2064 6570 656e  y required depen
-00002e90: 6465 6e63 6965 7320 2620 7761 7265 686f  dencies & wareho
-00002ea0: 7573 6520 636f 6e6e 6563 7469 6f6e 2e20  use connection. 
-00002eb0: 496e 2063 6173 6520 6f66 2073 7563 6365  In case of succe
-00002ec0: 7373 2c20 6974 2077 696c 6c20 7368 6f77  ss, it will show
-00002ed0: 2079 6f75 200a 2241 6c6c 2063 6865 636b   you ."All check
-00002ee0: 7320 7061 7373 6564 2122 0a60 6060 636f  s passed!".```co
-00002ef0: 6d6d 616e 646c 696e 650a 6462 7420 6465  mmandline.dbt de
-00002f00: 6275 670a 6060 600a 215b 4465 6275 675d  bug.```.![Debug]
-00002f10: 282e 2f65 7861 6d70 6c65 732f 345f 6465  (./examples/4_de
-00002f20: 6275 672e 706e 6729 0a23 2044 6174 6173  bug.png).# Datas
-00002f30: 6574 2049 6e67 6573 7469 6f6e 0a54 6f20  et Ingestion.To 
-00002f40: 7368 6f77 6361 7365 2064 6966 6665 7265  showcase differe
-00002f50: 6e74 2060 6462 7460 2066 756e 6374 696f  nt `dbt` functio
-00002f60: 6e61 6c69 7469 6573 2c20 7765 2077 696c  nalities, we wil
-00002f70: 6c20 696e 6765 7374 2061 2073 6d61 6c6c  l ingest a small
-00002f80: 2069 6d64 6220 6d6f 7669 6520 6461 7461   imdb movie data
-00002f90: 7365 742c 2077 6974 6820 7468 6520 666f  set, with the fo
-00002fa0: 6c6c 6f77 696e 6720 7363 6865 6d61 2e20  llowing schema. 
-00002fb0: 0a54 6865 2044 444c 2026 2069 6e73 6572  .The DDL & inser
-00002fc0: 7469 6f6e 2071 7565 7269 6573 2063 616e  tion queries can
-00002fd0: 2062 6520 666f 756e 6420 6865 7265 2068   be found here h
-00002fe0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002ff0: 6d2f 6279 7465 686f 7573 652d 636c 6f75  m/bytehouse-clou
-00003000: 642f 6279 7465 686f 7573 652d 6462 742f  d/bytehouse-dbt/
-00003010: 6578 616d 706c 6573 2f64 6174 615f 6c6f  examples/data_lo
-00003020: 6164 696e 672e 7371 6c2e 200a 596f 7520  ading.sql. .You 
-00003030: 6361 6e20 7573 6520 4279 7465 486f 7573  can use ByteHous
-00003040: 6520 5351 4c20 776f 726b 7368 6565 7420  e SQL worksheet 
-00003050: 746f 2063 7265 6174 6520 7468 6520 7363  to create the sc
-00003060: 6865 6d61 2026 2069 6e73 6572 7420 7468  hema & insert th
-00003070: 6520 6461 7461 7365 742e 200a 215b 5363  e dataset. .![Sc
-00003080: 6865 6d61 5d28 2e2f 6578 616d 706c 6573  hema](./examples
-00003090: 2f35 5f73 6368 656d 612e 706e 6729 0a54  /5_schema.png).T
-000030a0: 6f20 7665 7269 6679 2074 6861 7420 6461  o verify that da
-000030b0: 7461 7365 7420 7072 6570 6172 6174 696f  taset preparatio
-000030c0: 6e20 7761 7320 7375 6363 6573 7366 756c  n was successful
-000030d0: 2c20 7765 2077 696c 6c20 6578 6563 7574  , we will execut
-000030e0: 6520 7468 6973 2066 6f6c 6c6f 7769 6e67  e this following
-000030f0: 2071 7565 7279 2074 6f20 7375 6d6d 6172   query to summar
-00003100: 697a 6520 6561 6368 2061 6374 6f72 2061  ize each actor a
-00003110: 6c6f 6e67 200a 7769 7468 2074 6865 6972  long .with their
-00003120: 2074 6f74 616c 206e 756d 6265 7220 6f66   total number of
-00003130: 206d 6f76 6965 2061 7070 6561 7261 6e63   movie appearanc
-00003140: 6573 2e20 0a60 6060 0a53 454c 4543 5420  es. .```.SELECT 
-00003150: 6964 2c0a 2020 616e 7928 6163 746f 725f  id,.  any(actor_
-00003160: 6e61 6d65 2920 6173 206e 616d 652c 0a20  name) as name,. 
-00003170: 2075 6e69 7145 7861 6374 286d 6f76 6965   uniqExact(movie
-00003180: 5f69 6429 2020 2020 6173 206e 756d 5f6d  _id)    as num_m
-00003190: 6f76 6965 732c 0a20 2061 7667 2872 6174  ovies,.  avg(rat
-000031a0: 696e 6729 2020 2020 2020 2020 2020 2020  ing)            
-000031b0: 2020 2020 6173 2061 7667 5f72 6174 696e      as avg_ratin
-000031c0: 672c 0a20 206d 6178 2863 7265 6174 6564  g,.  max(created
-000031d0: 5f61 7429 2061 7320 7570 6461 7465 645f  _at) as updated_
-000031e0: 6174 0a46 524f 4d20 280a 2020 5345 4c45  at.FROM (.  SELE
-000031f0: 4354 2061 6374 6f72 732e 6964 2061 7320  CT actors.id as 
-00003200: 6964 2c0a 2020 2020 2020 2063 6f6e 6361  id,.       conca
-00003210: 7428 6163 746f 7273 2e66 6972 7374 5f6e  t(actors.first_n
-00003220: 616d 652c 2027 2027 2c20 6163 746f 7273  ame, ' ', actors
-00003230: 2e6c 6173 745f 6e61 6d65 2920 6173 2061  .last_name) as a
-00003240: 6374 6f72 5f6e 616d 652c 0a20 2020 2020  ctor_name,.     
-00003250: 2020 6d6f 7669 6573 2e69 6420 6173 206d    movies.id as m
-00003260: 6f76 6965 5f69 642c 0a20 2020 2020 2020  ovie_id,.       
-00003270: 6d6f 7669 6573 2e72 6174 696e 6720 6173  movies.rating as
-00003280: 2072 6174 696e 672c 0a20 2020 2020 2020   rating,.       
-00003290: 6372 6561 7465 645f 6174 0a20 2046 524f  created_at.  FRO
-000032a0: 4d20 2069 6d64 622e 6163 746f 7273 0a20  M  imdb.actors. 
-000032b0: 2020 2020 2020 204a 4f49 4e20 696d 6462         JOIN imdb
-000032c0: 2e72 6f6c 6573 204f 4e20 726f 6c65 732e  .roles ON roles.
-000032d0: 6163 746f 725f 6964 203d 2061 6374 6f72  actor_id = actor
-000032e0: 732e 6964 0a20 2020 2020 2020 204c 4546  s.id.        LEF
-000032f0: 5420 4f55 5445 5220 4a4f 494e 2069 6d64  T OUTER JOIN imd
-00003300: 622e 6d6f 7669 6573 204f 4e20 6d6f 7669  b.movies ON movi
-00003310: 6573 2e69 6420 3d20 726f 6c65 732e 6d6f  es.id = roles.mo
-00003320: 7669 655f 6964 0a29 0a47 524f 5550 2042  vie_id.).GROUP B
-00003330: 5920 6964 0a60 6060 0a54 6865 2072 6573  Y id.```.The res
-00003340: 756c 7473 6574 2073 686f 756c 6420 6265  ultset should be
-00003350: 206c 696b 6520 7468 6973 3a0a 215b 5363   like this:.![Sc
-00003360: 6865 6d61 2043 6f6e 6669 726d 5d28 2e2f  hema Confirm](./
-00003370: 6578 616d 706c 6573 2f36 5f73 6368 656d  examples/6_schem
-00003380: 615f 636f 6e66 6972 6d2e 706e 6729 0a23  a_confirm.png).#
-00003390: 2064 6274 204d 6f64 656c 7320 0a49 6e20   dbt Models .In 
-000033a0: 6120 6064 6274 6020 7072 6f6a 6563 742c  a `dbt` project,
-000033b0: 2061 206d 6f64 656c 2069 7320 6120 7371   a model is a sq
-000033c0: 6c20 6669 6c65 206c 6f63 6174 6564 2069  l file located i
-000033d0: 6e73 6964 6520 606d 6f64 656c 732f 6020  nside `models/` 
-000033e0: 6469 7265 6374 6f72 7920 7768 6963 6820  directory which 
-000033f0: 7769 6c6c 2063 6f6e 7461 696e 2061 2060  will contain a `
-00003400: 5345 4c45 4354 6020 7374 6174 656d 656e  SELECT` statemen
-00003410: 7420 0a72 6566 6572 7269 6e67 2074 6f20  t .referring to 
-00003420: 6120 7472 616e 7366 6f72 6d61 7469 6f6e  a transformation
-00003430: 2e20 5468 6520 6e61 6d65 206f 6620 7468  . The name of th
-00003440: 6520 6d6f 6465 6c20 6669 6c65 2077 696c  e model file wil
-00003450: 6c20 7265 6665 7220 746f 2074 6865 206e  l refer to the n
-00003460: 616d 6520 6f66 2066 7574 7572 6520 7461  ame of future ta
-00003470: 626c 652f 7669 6577 2061 6674 6572 0a60  ble/view after.`
-00003480: 6462 7460 2065 7865 6375 7469 6f6e 2e20  dbt` execution. 
-00003490: 5768 656e 2077 6520 6578 6563 7574 6520  When we execute 
-000034a0: 6064 6274 2072 756e 6020 636f 6d6d 616e  `dbt run` comman
-000034b0: 642c 2060 6462 7460 2077 696c 6c20 6275  d, `dbt` will bu
-000034c0: 696c 6420 7468 6973 206d 6f64 656c 2064  ild this model d
-000034d0: 6972 6563 746c 7920 696e 746f 2042 7974  irectly into Byt
-000034e0: 6548 6f75 7365 2062 7920 7772 6170 7069  eHouse by wrappi
-000034f0: 6e67 0a69 7420 696e 2061 2063 7265 6174  ng.it in a creat
-00003500: 6520 7461 626c 6520 2f20 7669 6577 206d  e table / view m
-00003510: 6174 6572 6961 6c69 7a61 7469 6f6e 2e20  aterialization. 
-00003520: 4d61 7465 7269 616c 697a 6174 696f 6e20  Materialization 
-00003530: 7479 7065 206f 6620 796f 7572 206d 6f64  type of your mod
-00003540: 656c 2077 696c 6c20 6465 7465 726d 696e  el will determin
-00003550: 6520 7468 6520 6163 7475 616c 2053 514c  e the actual SQL
-00003560: 0a74 6861 7420 6064 6274 6020 7769 6c6c  .that `dbt` will
-00003570: 2075 7365 2074 6f20 6372 6561 7465 206d   use to create m
-00003580: 6f64 656c 2069 6e20 7468 6520 7761 7265  odel in the ware
-00003590: 686f 7573 652e 0a23 2073 6368 656d 612e  house..# schema.
-000035a0: 796d 6c0a 5468 6520 6073 6368 656d 612e  yml.The `schema.
-000035b0: 796d 6c60 2066 696c 6520 7769 6c6c 2064  yml` file will d
-000035c0: 6566 696e 6520 6f75 7220 7461 626c 6573  efine our tables
-000035d0: 2026 2063 6f6c 756d 6e73 2062 7920 7265   & columns by re
-000035e0: 6665 7272 696e 6720 7468 726f 7567 6820  ferring through 
-000035f0: 616c 6961 7320 6e61 6d65 2e20 5468 6973  alias name. This
-00003600: 2073 6368 656d 6173 2063 616e 206c 6174   schemas can lat
-00003610: 6572 2062 650a 7573 6564 2069 6e20 6469  er be.used in di
-00003620: 6666 6572 656e 7420 6d6f 6465 6c73 2f6d  fferent models/m
-00003630: 6163 726f 7320 7669 6120 6073 6f75 7263  acros via `sourc
-00003640: 6528 2960 2066 756e 6374 696f 6e2e 0a43  e()` function..C
-00003650: 7265 6174 6520 6073 6368 656d 612e 796d  reate `schema.ym
-00003660: 6c60 2066 696c 6520 756e 6465 7220 606d  l` file under `m
-00003670: 6f64 656c 732f 6020 6469 7265 6374 6f72  odels/` director
-00003680: 790a 6060 6063 6f6d 6d61 6e64 6c69 6e65  y.```commandline
-00003690: 0a74 6f75 6368 206d 6f64 656c 732f 7363  .touch models/sc
-000036a0: 6865 6d61 2e79 6d6c 0a60 6060 0a44 6566  hema.yml.```.Def
-000036b0: 696e 6520 6f75 7220 6d6f 6465 6c20 7363  ine our model sc
-000036c0: 6865 6d61 206c 696b 6520 7468 6973 0a60  hema like this.`
-000036d0: 6060 7961 6d6c 0a76 6572 7369 6f6e 3a20  ``yaml.version: 
-000036e0: 320a 0a73 6f75 7263 6573 3a0a 2d20 6e61  2..sources:.- na
-000036f0: 6d65 3a20 696d 6462 0a20 2074 6162 6c65  me: imdb.  table
-00003700: 733a 0a20 202d 206e 616d 653a 2061 6374  s:.  - name: act
-00003710: 6f72 730a 2020 2d20 6e61 6d65 3a20 726f  ors.  - name: ro
-00003720: 6c65 730a 2020 2d20 6e61 6d65 3a20 6d6f  les.  - name: mo
-00003730: 7669 6573 0a60 6060 0a23 204d 6174 6572  vies.```.# Mater
-00003740: 6961 6c69 7a61 7469 6f6e 2074 7970 6573  ialization types
-00003750: 206f 6620 4d6f 6465 6c73 0a23 2320 5669   of Models.## Vi
-00003760: 6577 204d 6174 6572 6961 6c69 7a61 7469  ew Materializati
-00003770: 6f6e 730a 496e 2063 6173 6520 6f66 2076  ons.In case of v
-00003780: 6965 7720 6d61 7465 7269 616c 697a 6174  iew materializat
-00003790: 696f 6e2c 2061 206d 6f64 656c 2069 7320  ion, a model is 
-000037a0: 7472 616e 7366 6f72 6d65 6420 746f 2061  transformed to a
-000037b0: 2076 6965 7720 6f6e 2065 6163 6820 7369   view on each si
-000037c0: 6e67 6c65 2072 756e 2062 7920 6043 5245  ngle run by `CRE
-000037d0: 4154 4520 5649 4557 6020 4153 2073 7461  ATE VIEW` AS sta
-000037e0: 7465 6d65 6e74 2069 6e20 0a42 7974 6548  tement in .ByteH
-000037f0: 6f75 7365 2e20 5669 6577 206d 6174 6572  ouse. View mater
-00003800: 6961 6c69 7a61 7469 6f6e 7320 776f 6e27  ializations won'
-00003810: 7420 7374 6f72 6520 7468 6520 6163 7475  t store the actu
-00003820: 616c 2064 6174 612c 2073 6f20 6974 2077  al data, so it w
-00003830: 6f75 6c64 2062 6520 736c 6f77 6572 2074  ould be slower t
-00003840: 6f20 7175 6572 7920 7468 616e 2074 6162  o query than tab
-00003850: 6c65 206d 6174 6572 6961 6c69 7a61 7469  le materializati
-00003860: 6f6e 732e 0a4c 6574 2773 2063 7265 6174  ons..Let's creat
-00003870: 6520 606d 6f64 656c 732f 6163 746f 725f  e `models/actor_
-00003880: 696e 7369 6768 742e 7371 6c60 2061 7320  insight.sql` as 
-00003890: 7669 6577 206d 6174 6572 6961 6c69 7a61  view materializa
-000038a0: 7469 6f6e 2e20 0a60 6060 636f 6d6d 616e  tion. .```comman
-000038b0: 646c 696e 650a 746f 7563 6820 6d6f 6465  dline.touch mode
-000038c0: 6c73 2f61 6374 6f72 735f 696e 7369 6768  ls/actors_insigh
-000038d0: 742e 7371 6c0a 6060 600a 6060 600a 7b7b  t.sql.```.```.{{
-000038e0: 2063 6f6e 6669 6728 6d61 7465 7269 616c   config(material
-000038f0: 697a 6564 3d27 7669 6577 2729 207d 7d0a  ized='view') }}.
-00003900: 0a53 454c 4543 5420 6964 2c0a 2020 616e  .SELECT id,.  an
-00003910: 7928 6163 746f 725f 6e61 6d65 2920 6173  y(actor_name) as
-00003920: 206e 616d 652c 0a20 2075 6e69 7145 7861   name,.  uniqExa
-00003930: 6374 286d 6f76 6965 5f69 6429 2020 2020  ct(movie_id)    
-00003940: 6173 206e 756d 5f6d 6f76 6965 732c 0a20  as num_movies,. 
-00003950: 2061 7667 2872 6174 696e 6729 2020 2020   avg(rating)    
-00003960: 2020 2020 2020 2020 2020 2020 6173 2061              as a
-00003970: 7667 5f72 6174 696e 672c 0a20 206d 6178  vg_rating,.  max
-00003980: 2863 7265 6174 6564 5f61 7429 2061 7320  (created_at) as 
-00003990: 7570 6461 7465 645f 6174 0a46 524f 4d20  updated_at.FROM 
-000039a0: 280a 2020 5345 4c45 4354 2061 6374 6f72  (.  SELECT actor
-000039b0: 732e 6964 2061 7320 6964 2c0a 2020 2020  s.id as id,.    
-000039c0: 2020 2063 6f6e 6361 7428 6163 746f 7273     concat(actors
-000039d0: 2e66 6972 7374 5f6e 616d 652c 2027 2027  .first_name, ' '
-000039e0: 2c20 6163 746f 7273 2e6c 6173 745f 6e61  , actors.last_na
-000039f0: 6d65 2920 6173 2061 6374 6f72 5f6e 616d  me) as actor_nam
-00003a00: 652c 0a20 2020 2020 2020 6d6f 7669 6573  e,.       movies
-00003a10: 2e69 6420 6173 206d 6f76 6965 5f69 642c  .id as movie_id,
-00003a20: 0a20 2020 2020 2020 6d6f 7669 6573 2e72  .       movies.r
-00003a30: 6174 696e 6720 6173 2072 6174 696e 672c  ating as rating,
-00003a40: 0a20 2020 2020 2020 6372 6561 7465 645f  .       created_
-00003a50: 6174 0a20 2046 524f 4d20 207b 7b20 736f  at.  FROM  {{ so
-00003a60: 7572 6365 2827 696d 6462 272c 2027 6163  urce('imdb', 'ac
-00003a70: 746f 7273 2729 207d 7d0a 2020 2020 2020  tors') }}.      
-00003a80: 2020 4a4f 494e 207b 7b20 736f 7572 6365    JOIN {{ source
-00003a90: 2827 696d 6462 272c 2027 726f 6c65 7327  ('imdb', 'roles'
-00003aa0: 2920 7d7d 204f 4e20 726f 6c65 732e 6163  ) }} ON roles.ac
-00003ab0: 746f 725f 6964 203d 2061 6374 6f72 732e  tor_id = actors.
-00003ac0: 6964 0a20 2020 2020 2020 204c 4546 5420  id.        LEFT 
-00003ad0: 4f55 5445 5220 4a4f 494e 207b 7b20 736f  OUTER JOIN {{ so
-00003ae0: 7572 6365 2827 696d 6462 272c 2027 6d6f  urce('imdb', 'mo
-00003af0: 7669 6573 2729 207d 7d20 4f4e 206d 6f76  vies') }} ON mov
-00003b00: 6965 732e 6964 203d 2072 6f6c 6573 2e6d  ies.id = roles.m
-00003b10: 6f76 6965 5f69 640a 290a 4752 4f55 5020  ovie_id.).GROUP 
-00003b20: 4259 2069 640a 6060 600a 4c65 7427 7320  BY id.```.Let's 
-00003b30: 6578 6563 7574 6520 6064 6274 2072 756e  execute `dbt run
-00003b40: 6020 636f 6d6d 616e 6420 746f 2062 7569  ` command to bui
-00003b50: 6c64 2074 6869 7320 6d6f 6465 6c20 696e  ld this model in
-00003b60: 2042 7974 6548 6f75 7365 2e20 0a21 5b43   ByteHouse. .![C
-00003b70: 6f6e 6669 726d 5d28 2e2f 6578 616d 706c  onfirm](./exampl
-00003b80: 6573 2f37 5f61 6374 6f72 5f69 6e73 6967  es/7_actor_insig
-00003b90: 6874 5f63 6f6e 6669 726d 2e70 6e67 290a  ht_confirm.png).
-00003ba0: 5175 6572 7969 6e67 2074 6869 7320 7669  Querying this vi
-00003bb0: 6577 2c20 7765 2063 616e 2072 6570 6c69  ew, we can repli
-00003bc0: 6361 7465 2074 6865 2072 6573 756c 7473  cate the results
-00003bd0: 206f 6620 6f75 7220 6561 726c 6965 7220   of our earlier 
-00003be0: 7175 6572 7920 7769 7468 2061 2073 696d  query with a sim
-00003bf0: 706c 6572 2073 796e 7461 783a 0a60 6060  pler syntax:.```
-00003c00: 0a53 454c 4543 5420 2a20 4652 4f4d 2069  .SELECT * FROM i
-00003c10: 6d64 622e 6163 746f 7273 5f69 6e73 6967  mdb.actors_insig
-00003c20: 6874 204f 5244 4552 2042 5920 6e75 6d5f  ht ORDER BY num_
-00003c30: 6d6f 7669 6573 2044 4553 433b 0a60 6060  movies DESC;.```
-00003c40: 0a21 5b43 6f6e 6669 726d 325d 282e 2f65  .![Confirm2](./e
-00003c50: 7861 6d70 6c65 732f 385f 6d61 7465 7269  xamples/8_materi
-00003c60: 616c 697a 6564 5f76 6965 775f 7275 6e5f  alized_view_run_
-00003c70: 636f 6e66 6972 6d2e 706e 6729 0a23 2320  confirm.png).## 
-00003c80: 5461 626c 6520 4d61 7465 7269 616c 697a  Table Materializ
-00003c90: 6174 696f 6e73 0a49 6e20 6361 7365 206f  ations.In case o
-00003ca0: 6620 7461 626c 6520 6d61 7465 7269 616c  f table material
-00003cb0: 697a 6174 696f 6e2c 2079 6f75 7220 6d6f  ization, your mo
-00003cc0: 6465 6c20 776f 756c 6420 6265 2072 6562  del would be reb
-00003cd0: 7569 6c74 2061 7320 6120 7461 626c 6520  uilt as a table 
-00003ce0: 6f6e 2065 6163 6820 7369 6e67 6c65 2060  on each single `
-00003cf0: 6462 7420 7275 6e60 200a 7669 6120 6120  dbt run` .via a 
-00003d00: 6043 5245 4154 4520 5441 424c 4560 2041  `CREATE TABLE` A
-00003d10: 5320 7374 6174 656d 656e 742e 200a 6060  S statement. .``
-00003d20: 6063 6f6d 6d61 6e64 6c69 6e65 0a74 6f75  `commandline.tou
-00003d30: 6368 206d 6f64 656c 732f 6163 746f 7273  ch models/actors
-00003d40: 5f69 6e73 6967 6874 5f74 6162 6c65 2e73  _insight_table.s
-00003d50: 716c 0a60 6060 0a57 6520 6361 6e20 7573  ql.```.We can us
-00003d60: 6520 6f75 7220 7072 6576 696f 7573 2076  e our previous v
-00003d70: 6965 7720 6d61 7465 7269 616c 697a 6174  iew materializat
-00003d80: 696f 6e20 7371 6c20 7769 7468 2063 6f6e  ion sql with con
-00003d90: 6669 6720 6368 616e 6765 2066 6f72 2074  fig change for t
-00003da0: 6162 6c65 206d 6174 6572 6961 6c69 7a61  able materializa
-00003db0: 7469 6f6e 2073 716c 2e20 0a60 6060 0a7b  tion sql. .```.{
-00003dc0: 7b20 636f 6e66 6967 286f 7264 6572 5f62  { config(order_b
-00003dd0: 793d 2728 7570 6461 7465 645f 6174 2c20  y='(updated_at, 
-00003de0: 6964 2c20 6e61 6d65 2927 2c20 6d61 7465  id, name)', mate
-00003df0: 7269 616c 697a 6564 3d27 7461 626c 6527  rialized='table'
-00003e00: 2920 7d7d 0a60 6060 0a57 6520 6361 6e20  ) }}.```.We can 
-00003e10: 7665 7269 6679 2074 6861 7420 626f 7468  verify that both
-00003e20: 2076 6965 7720 2620 7461 626c 6520 6d61   view & table ma
-00003e30: 7465 7269 616c 697a 6174 696f 6e73 2067  terializations g
-00003e40: 656e 6572 6174 6520 7468 6520 7361 6d65  enerate the same
-00003e50: 2072 6573 706f 6e73 652e 200a 6060 600a   response. .```.
-00003e60: 2053 454c 4543 5420 2a20 4652 4f4d 2069   SELECT * FROM i
-00003e70: 6d64 622e 6163 746f 7273 5f69 6e73 6967  mdb.actors_insig
-00003e80: 6874 5f74 6162 6c65 204f 5244 4552 2042  ht_table ORDER B
-00003e90: 5920 6e75 6d5f 6d6f 7669 6573 2044 4553  Y num_movies DES
-00003ea0: 433b 0a60 6060 0a23 2320 496e 6372 656d  C;.```.## Increm
-00003eb0: 656e 7461 6c20 4d61 7465 7269 616c 697a  ental Materializ
-00003ec0: 6174 696f 6e73 0a46 6f72 206f 7572 2070  ations.For our p
-00003ed0: 7265 7669 6f75 7320 7461 626c 6520 6d61  revious table ma
-00003ee0: 7465 7269 616c 697a 6174 696f 6e2c 2060  terialization, `
-00003ef0: 6462 7460 2077 696c 6c20 636f 6e73 7472  dbt` will constr
-00003f00: 7563 7420 6120 7461 626c 6520 6576 6572  uct a table ever
-00003f10: 7920 7469 6d65 2074 6f20 6d61 7465 7269  y time to materi
-00003f20: 616c 697a 6520 7468 6520 6d6f 6465 6c2e  alize the model.
-00003f30: 2046 6f72 206c 6172 6765 720a 6f72 2063   For larger.or c
-00003f40: 6f6d 706c 6578 2074 7261 6e73 666f 726d  omplex transform
-00003f50: 6174 696f 6e73 2c20 7468 6973 2077 6f75  ations, this wou
-00003f60: 6c64 2062 6520 7265 6475 6e64 616e 7420  ld be redundant 
-00003f70: 616e 6420 636f 7374 6c79 2069 6e20 7465  and costly in te
-00003f80: 726d 7320 6f66 2063 6f6d 7075 7469 6e67  rms of computing
-00003f90: 2070 6f77 6572 2e20 496e 6372 656d 656e   power. Incremen
-00003fa0: 7461 6c20 0a6d 6174 6572 6961 6c69 7a61  tal .materializa
-00003fb0: 7469 6f6e 7320 736f 6c76 6520 7468 6973  tions solve this
-00003fc0: 2070 726f 626c 656d 2e3c 6272 2f3e 0a54   problem.<br/>.T
-00003fd0: 6865 2066 6972 7374 2074 696d 6520 6120  he first time a 
-00003fe0: 6d6f 6465 6c20 6973 2072 756e 2c20 7468  model is run, th
-00003ff0: 6520 7461 626c 6520 6973 2062 7569 6c74  e table is built
-00004000: 2062 7920 7472 616e 7366 6f72 6d69 6e67   by transforming
-00004010: 2061 6c6c 2072 6f77 7320 6f66 2073 6f75   all rows of sou
-00004020: 7263 6520 6461 7461 2e20 4f6e 2073 7562  rce data. On sub
-00004030: 7365 7175 656e 7420 7275 6e73 2c20 0a60  sequent runs, .`
-00004040: 6462 7460 2074 7261 6e73 666f 726d 7320  dbt` transforms 
-00004050: 6f6e 6c79 2074 6865 2072 6f77 7320 696e  only the rows in
-00004060: 2079 6f75 7220 736f 7572 6365 2064 6174   your source dat
-00004070: 6120 7468 6174 2079 6f75 2074 656c 6c20  a that you tell 
-00004080: 6064 6274 6020 746f 2066 696c 7465 7220  `dbt` to filter 
-00004090: 666f 722c 2069 6e73 6572 7469 6e67 2074  for, inserting t
-000040a0: 6865 6d20 696e 746f 2074 6865 2074 6172  hem into the tar
-000040b0: 6765 7420 0a74 6162 6c65 2077 6869 6368  get .table which
-000040c0: 2069 7320 7468 6520 7461 626c 6520 7468   is the table th
-000040d0: 6174 2068 6173 2061 6c72 6561 6479 2062  at has already b
-000040e0: 6565 6e20 6275 696c 742e 3c62 722f 3e0a  een built.<br/>.
-000040f0: 546f 2074 656c 6c20 6064 6274 6020 7768  To tell `dbt` wh
-00004100: 6963 6820 726f 7773 2069 7420 7368 6f75  ich rows it shou
-00004110: 6c64 2074 7261 6e73 666f 726d 206f 6e20  ld transform on 
-00004120: 616e 2069 6e63 7265 6d65 6e74 616c 2072  an incremental r
-00004130: 756e 2c20 7772 6170 2076 616c 6964 2053  un, wrap valid S
-00004140: 514c 2074 6861 7420 6669 6c74 6572 7320  QL that filters 
-00004150: 666f 7220 7468 6573 6520 726f 7773 200a  for these rows .
-00004160: 696e 2074 6865 2060 6973 5f69 6e63 7265  in the `is_incre
-00004170: 6d65 6e74 616c 2829 6020 6d61 6372 6f2e  mental()` macro.
-00004180: 2059 6f75 7220 6069 735f 696e 6372 656d   Your `is_increm
-00004190: 656e 7461 6c28 2960 2063 6f64 6520 7769  ental()` code wi
-000041a0: 6c6c 2063 6865 636b 2066 6f72 2072 6f77  ll check for row
-000041b0: 7320 6372 6561 7465 6420 6f72 206d 6f64  s created or mod
-000041c0: 6966 6965 6420 7369 6e63 6520 7468 6520  ified since the 
-000041d0: 0a6c 6173 7420 7469 6d65 2060 6462 7460  .last time `dbt`
-000041e0: 2072 616e 2074 6869 7320 6d6f 6465 6c2e   ran this model.
-000041f0: 0a60 6060 636f 6d6d 616e 646c 696e 650a  .```commandline.
-00004200: 746f 7563 6820 6d6f 6465 6c73 2f61 6374  touch models/act
-00004210: 6f72 735f 696e 7369 6768 745f 696e 6372  ors_insight_incr
-00004220: 656d 656e 7461 6c2e 7371 6c0a 6060 600a  emental.sql.```.
-00004230: 6060 600a 7b7b 2063 6f6e 6669 6728 6f72  ```.{{ config(or
-00004240: 6465 725f 6279 3d27 2875 7064 6174 6564  der_by='(updated
-00004250: 5f61 742c 2069 642c 206e 616d 6529 272c  _at, id, name)',
-00004260: 206d 6174 6572 6961 6c69 7a65 643d 2769   materialized='i
-00004270: 6e63 7265 6d65 6e74 616c 2729 207d 7d0a  ncremental') }}.
-00004280: 0a53 454c 4543 5420 6964 2c0a 2020 616e  .SELECT id,.  an
-00004290: 7928 6163 746f 725f 6e61 6d65 2920 6173  y(actor_name) as
-000042a0: 206e 616d 652c 0a20 2075 6e69 7145 7861   name,.  uniqExa
-000042b0: 6374 286d 6f76 6965 5f69 6429 2020 2020  ct(movie_id)    
-000042c0: 6173 206e 756d 5f6d 6f76 6965 732c 0a20  as num_movies,. 
-000042d0: 2061 7667 2872 6174 696e 6729 2020 2020   avg(rating)    
-000042e0: 2020 2020 2020 2020 2020 2020 6173 2061              as a
-000042f0: 7667 5f72 6174 696e 672c 0a20 206d 6178  vg_rating,.  max
-00004300: 2863 7265 6174 6564 5f61 7429 2061 7320  (created_at) as 
-00004310: 7570 6461 7465 645f 6174 0a46 524f 4d20  updated_at.FROM 
-00004320: 280a 2020 5345 4c45 4354 2061 6374 6f72  (.  SELECT actor
-00004330: 732e 6964 2061 7320 6964 2c0a 2020 2020  s.id as id,.    
-00004340: 2020 2063 6f6e 6361 7428 6163 746f 7273     concat(actors
-00004350: 2e66 6972 7374 5f6e 616d 652c 2027 2027  .first_name, ' '
-00004360: 2c20 6163 746f 7273 2e6c 6173 745f 6e61  , actors.last_na
-00004370: 6d65 2920 6173 2061 6374 6f72 5f6e 616d  me) as actor_nam
-00004380: 652c 0a20 2020 2020 2020 6d6f 7669 6573  e,.       movies
-00004390: 2e69 6420 6173 206d 6f76 6965 5f69 642c  .id as movie_id,
-000043a0: 0a20 2020 2020 2020 6d6f 7669 6573 2e72  .       movies.r
-000043b0: 6174 696e 6720 6173 2072 6174 696e 672c  ating as rating,
-000043c0: 0a20 2020 2020 2020 6372 6561 7465 645f  .       created_
-000043d0: 6174 0a20 2046 524f 4d20 207b 7b20 736f  at.  FROM  {{ so
-000043e0: 7572 6365 2827 696d 6462 272c 2027 6163  urce('imdb', 'ac
-000043f0: 746f 7273 2729 207d 7d0a 2020 2020 2020  tors') }}.      
-00004400: 2020 4a4f 494e 207b 7b20 736f 7572 6365    JOIN {{ source
-00004410: 2827 696d 6462 272c 2027 726f 6c65 7327  ('imdb', 'roles'
-00004420: 2920 7d7d 204f 4e20 726f 6c65 732e 6163  ) }} ON roles.ac
-00004430: 746f 725f 6964 203d 2061 6374 6f72 732e  tor_id = actors.
-00004440: 6964 0a20 2020 2020 2020 204c 4546 5420  id.        LEFT 
-00004450: 4f55 5445 5220 4a4f 494e 207b 7b20 736f  OUTER JOIN {{ so
-00004460: 7572 6365 2827 696d 6462 272c 2027 6d6f  urce('imdb', 'mo
-00004470: 7669 6573 2729 207d 7d20 4f4e 206d 6f76  vies') }} ON mov
-00004480: 6965 732e 6964 203d 2072 6f6c 6573 2e6d  ies.id = roles.m
-00004490: 6f76 6965 5f69 640a 290a 4752 4f55 5020  ovie_id.).GROUP 
-000044a0: 4259 2069 640a 0a7b 2520 6966 2069 735f  BY id..{% if is_
-000044b0: 696e 6372 656d 656e 7461 6c28 2920 257d  incremental() %}
-000044c0: 0a0a 2d2d 2074 6869 7320 6669 6c74 6572  ..-- this filter
-000044d0: 2077 696c 6c20 6f6e 6c79 2062 6520 6170   will only be ap
-000044e0: 706c 6965 6420 6f6e 2061 6e20 696e 6372  plied on an incr
-000044f0: 656d 656e 7461 6c20 7275 6e0a 7768 6572  emental run.wher
-00004500: 6520 6964 203e 2028 7365 6c65 6374 206d  e id > (select m
-00004510: 6178 2869 6429 2066 726f 6d20 7b7b 2074  ax(id) from {{ t
-00004520: 6869 7320 7d7d 2920 6f72 2075 7064 6174  his }}) or updat
-00004530: 6564 5f61 7420 3e20 2873 656c 6563 7420  ed_at > (select 
-00004540: 6d61 7828 7570 6461 7465 645f 6174 2920  max(updated_at) 
-00004550: 6672 6f6d 207b 7b74 6869 737d 7d29 0a0a  from {{this}})..
-00004560: 7b25 2065 6e64 6966 2025 7d0a 6060 600a  {% endif %}.```.
-00004570: 5765 2063 616e 2076 6572 6966 7920 7468  We can verify th
-00004580: 6174 2076 6965 772c 2074 6162 6c65 2026  at view, table &
-00004590: 2069 6e63 7265 6d65 6e74 616c 206d 6174   incremental mat
-000045a0: 6572 6961 6c69 7a61 7469 6f6e 732c 2061  erializations, a
-000045b0: 6c6c 2067 656e 6572 6174 6520 7468 6520  ll generate the 
-000045c0: 7361 6d65 2072 6573 706f 6e73 652e 200a  same response. .
-000045d0: 6060 600a 2053 454c 4543 5420 2a20 4652  ```. SELECT * FR
-000045e0: 4f4d 2069 6d64 622e 6163 746f 7273 5f69  OM imdb.actors_i
-000045f0: 6e73 6967 6874 5f74 6162 6c65 204f 5244  nsight_table ORD
-00004600: 4552 2042 5920 6e75 6d5f 6d6f 7669 6573  ER BY num_movies
-00004610: 2044 4553 433b 0a60 6060 0a60 6060 636f   DESC;.```.```co
-00004620: 6d6d 616e 646c 696e 650a 6462 7420 7275  mmandline.dbt ru
-00004630: 6e20 2d6d 206d 6f64 656c 732f 6163 746f  n -m models/acto
-00004640: 7273 5f69 6e73 6967 6874 5f69 6e63 7265  rs_insight_incre
-00004650: 6d65 6e74 616c 2e73 716c 0a60 6060 0a4c  mental.sql.```.L
-00004660: 6574 2773 2069 6e73 6572 7420 6120 6665  et's insert a fe
-00004670: 7720 6d6f 7265 2072 6f77 7320 746f 2064  w more rows to d
-00004680: 656d 6f6e 7374 7261 7465 2074 6865 2070  emonstrate the p
-00004690: 6f77 6572 206f 6620 696e 6372 656d 656e  ower of incremen
-000046a0: 7461 6c20 6d61 7465 7269 616c 697a 6174  tal materializat
-000046b0: 696f 6e73 2e20 4e6f 7720 7468 6520 6d6f  ions. Now the mo
-000046c0: 7374 200a 6170 7065 6172 6564 2061 6374  st .appeared act
-000046d0: 6f72 2073 686f 756c 6420 6265 2027 4368  or should be 'Ch
-000046e0: 7269 7320 5072 6174 7427 2e20 0a60 6060  ris Pratt'. .```
-000046f0: 0a49 4e53 4552 5420 494e 544f 2069 6d64  .INSERT INTO imd
-00004700: 622e 6d6f 7669 6573 2056 414c 5545 5320  b.movies VALUES 
-00004710: 2839 2c20 2750 6173 7365 6e67 6572 7327  (9, 'Passengers'
-00004720: 2c20 3230 3136 2c20 3729 3b0a 494e 5345  , 2016, 7);.INSE
-00004730: 5254 2049 4e54 4f20 696d 6462 2e6d 6f76  RT INTO imdb.mov
-00004740: 6965 7320 5641 4c55 4553 2028 3130 2c20  ies VALUES (10, 
-00004750: 2754 6865 2054 6f6d 6f72 726f 7720 5761  'The Tomorrow Wa
-00004760: 7227 2c20 3230 3231 2c20 362e 3529 3b0a  r', 2021, 6.5);.
-00004770: 0a49 4e53 4552 5420 494e 544f 2069 6d64  .INSERT INTO imd
-00004780: 622e 726f 6c65 7320 2861 6374 6f72 5f69  b.roles (actor_i
-00004790: 642c 206d 6f76 6965 5f69 642c 2072 6f6c  d, movie_id, rol
-000047a0: 655f 6e61 6d65 2920 5641 4c55 4553 2834  e_name) VALUES(4
-000047b0: 2c20 392c 2027 4a69 6d20 5072 6573 746f  , 9, 'Jim Presto
-000047c0: 6e27 293b 0a49 4e53 4552 5420 494e 544f  n');.INSERT INTO
-000047d0: 2069 6d64 622e 726f 6c65 7320 2861 6374   imdb.roles (act
-000047e0: 6f72 5f69 642c 206d 6f76 6965 5f69 642c  or_id, movie_id,
-000047f0: 2072 6f6c 655f 6e61 6d65 2920 5641 4c55   role_name) VALU
-00004800: 4553 2834 2c20 3130 2c20 2744 616e 2046  ES(4, 10, 'Dan F
-00004810: 6f72 6573 7465 7227 293b 0a60 6060 0a60  orester');.```.`
-00004820: 6060 636f 6d6d 616e 646c 696e 650a 6462  ``commandline.db
-00004830: 7420 7275 6e20 2d6d 206d 6f64 656c 732f  t run -m models/
-00004840: 6163 746f 7273 5f69 6e73 6967 6874 5f69  actors_insight_i
-00004850: 6e63 7265 6d65 6e74 616c 2e73 716c 0a60  ncremental.sql.`
-00004860: 6060 0a60 6060 0a53 454c 4543 5420 2a20  ``.```.SELECT * 
-00004870: 4652 4f4d 2069 6d64 622e 6163 746f 7273  FROM imdb.actors
-00004880: 5f69 6e73 6967 6874 5f69 6e63 7265 6d65  _insight_increme
-00004890: 6e74 616c 204f 5244 4552 2042 5920 6e75  ntal ORDER BY nu
-000048a0: 6d5f 6d6f 7669 6573 2044 4553 433b 0a60  m_movies DESC;.`
-000048b0: 6060 0a21 5b43 6f6e 6669 726d 335d 282e  ``.![Confirm3](.
-000048c0: 2f65 7861 6d70 6c65 732f 395f 696e 6372  /examples/9_incr
-000048d0: 656d 656e 7461 6c5f 636f 6e66 6972 6d2e  emental_confirm.
-000048e0: 706e 6729 0a23 2323 2048 6f77 2069 7420  png).### How it 
-000048f0: 776f 726b 730a 312e 2060 6462 7460 2077  works.1. `dbt` w
-00004900: 696c 6c20 6669 7273 7420 6372 6561 7465  ill first create
-00004910: 2061 2074 656d 706f 7261 7279 2074 6162   a temporary tab
-00004920: 6c65 206e 616d 6564 2060 6163 746f 7273  le named `actors
-00004930: 5f69 6e73 6967 6874 5f69 6e63 7265 6d65  _insight_increme
-00004940: 6e74 616c 5f74 6d70 6020 2620 696e 7365  ntal_tmp` & inse
-00004950: 7274 2061 6c6c 2074 686f 7365 2072 6f77  rt all those row
-00004960: 7320 7768 6963 6820 0a70 6173 7320 6f75  s which .pass ou
-00004970: 7220 6069 735f 696e 6372 656d 656e 7461  r `is_incrementa
-00004980: 6c28 2960 2066 696c 7465 722e 0a32 2e20  l()` filter..2. 
-00004990: 4120 6e65 7720 7461 626c 6520 6061 6374  A new table `act
-000049a0: 6f72 735f 696e 7369 6768 745f 696e 6372  ors_insight_incr
-000049b0: 656d 656e 7461 6c5f 6e65 7760 2077 696c  emental_new` wil
-000049c0: 6c20 6265 2063 7265 6174 6564 2026 2072  l be created & r
-000049d0: 6f77 7320 6672 6f6d 2074 6865 206f 6c64  ows from the old
-000049e0: 2074 6162 6c65 2060 6163 746f 7273 5f69   table `actors_i
-000049f0: 6e73 6967 6874 5f69 6e63 7265 6d65 6e74  nsight_increment
-00004a00: 616c 6020 0a77 696c 6c20 6265 2069 6e67  al` .will be ing
-00004a10: 6573 7465 6420 6865 7265 2e20 6064 6274  ested here. `dbt
-00004a20: 6020 7769 6c6c 206d 616b 6520 7375 7265  ` will make sure
-00004a30: 2074 6861 7420 6075 6e69 7175 655f 6b65   that `unique_ke
-00004a40: 7960 2028 6966 2061 6e79 2064 6563 6c61  y` (if any decla
-00004a50: 7265 6420 696e 2063 6f6e 6669 6729 2063  red in config) c
-00004a60: 6f6e 7374 7261 696e 7420 6973 206d 6169  onstraint is mai
-00004a70: 6e74 6169 6e65 642c 200a 6279 206e 6f74  ntained, .by not
-00004a80: 2061 6c6c 6f77 696e 6720 7468 6f73 6520   allowing those 
-00004a90: 726f 7773 2077 6869 6368 2068 6176 6520  rows which have 
-00004aa0: 7468 6520 7361 6d65 2060 756e 6971 7565  the same `unique
-00004ab0: 5f6b 6579 6020 6173 2074 6865 2070 7265  _key` as the pre
-00004ac0: 7669 6f75 7320 7465 6d70 6f72 6172 7920  vious temporary 
-00004ad0: 7461 626c 652e 200a 332e 2054 6865 2072  table. .3. The r
-00004ae0: 6f77 7320 6672 6f6d 2074 6865 2074 656d  ows from the tem
-00004af0: 706f 7261 7279 2074 6162 6c65 2077 6f75  porary table wou
-00004b00: 6c64 2062 6520 696e 6765 7374 6564 2069  ld be ingested i
-00004b10: 6e74 6f20 7468 6520 6e65 7720 7461 626c  nto the new tabl
-00004b20: 652e 0a34 2e20 4f75 7220 7072 6576 696f  e..4. Our previo
-00004b30: 7573 2074 6162 6c65 2028 6061 6374 6f72  us table (`actor
-00004b40: 735f 696e 7369 6768 745f 696e 6372 656d  s_insight_increm
-00004b50: 656e 7461 6c60 2920 2620 6e65 7720 7461  ental`) & new ta
-00004b60: 626c 6520 2860 6163 746f 7273 5f69 6e73  ble (`actors_ins
-00004b70: 6967 6874 5f6e 6577 6029 2077 696c 6c20  ight_new`) will 
-00004b80: 6265 2065 7863 6861 6e67 6564 2e20 0a23  be exchanged. .#
-00004b90: 2050 726f 6a65 6374 2044 6f63 756d 656e   Project Documen
-00004ba0: 7461 7469 6f6e 0a60 6462 7460 2070 726f  tation.`dbt` pro
-00004bb0: 7669 6465 7320 6120 7761 7920 746f 2067  vides a way to g
-00004bc0: 656e 6572 6174 6520 646f 6375 6d65 6e74  enerate document
-00004bd0: 6174 696f 6e20 666f 7220 796f 7572 2064  ation for your d
-00004be0: 6274 2070 726f 6a65 6374 2061 6e64 2072  bt project and r
-00004bf0: 656e 6465 7220 6974 2061 7320 6120 7765  ender it as a we
-00004c00: 6273 6974 652e 200a 4372 6561 7465 2060  bsite. .Create `
-00004c10: 6d6f 6465 6c73 2f61 6374 6f72 735f 696e  models/actors_in
-00004c20: 7369 6768 745f 696e 6372 656d 656e 7461  sight_incrementa
-00004c30: 6c2e 796d 6c60 2074 6f20 6765 6e65 7261  l.yml` to genera
-00004c40: 7465 2064 6f63 756d 656e 7461 7469 6f6e  te documentation
-00004c50: 2066 6f72 206f 7572 206d 6f64 656c 732e   for our models.
-00004c60: 200a 6060 6079 616d 6c0a 7665 7273 696f   .```yaml.versio
-00004c70: 6e3a 2032 0a0a 6d6f 6465 6c73 3a0a 2020  n: 2..models:.  
-00004c80: 2d20 6e61 6d65 3a20 6163 746f 7273 5f69  - name: actors_i
-00004c90: 6e73 6967 6874 5f69 6e63 7265 6d65 6e74  nsight_increment
-00004ca0: 616c 0a20 2020 2064 6573 6372 6970 7469  al.    descripti
-00004cb0: 6f6e 3a20 4163 746f 7220 6170 7065 6172  on: Actor appear
-00004cc0: 616e 6365 2073 756d 6d61 7279 2062 6173  ance summary bas
-00004cd0: 6564 206f 6e20 726f 6c65 730a 2020 2020  ed on roles.    
-00004ce0: 636f 6c75 6d6e 733a 200a 2020 2020 2020  columns: .      
-00004cf0: 2d20 6e61 6d65 3a20 6964 0a20 2020 2020  - name: id.     
-00004d00: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-00004d10: 5468 6520 6964 206e 756d 6265 7220 6f66  The id number of
-00004d20: 2061 6374 6f72 0a20 2020 2020 202d 206e   actor.      - n
-00004d30: 616d 653a 206e 616d 650a 2020 2020 2020  ame: name.      
-00004d40: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
-00004d50: 6865 206e 616d 6520 6f66 2061 6374 6f72  he name of actor
-00004d60: 0a20 2020 2020 202d 206e 616d 653a 206e  .      - name: n
-00004d70: 756d 5f6d 6f76 6965 730a 2020 2020 2020  um_movies.      
-00004d80: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
-00004d90: 6865 206e 756d 6265 7220 6f66 206d 6f76  he number of mov
-00004da0: 6965 7320 6163 746f 7220 6861 7320 6170  ies actor has ap
-00004db0: 7065 6172 6564 200a 2020 2020 2020 2d20  peared .      - 
-00004dc0: 6e61 6d65 3a20 6176 675f 7261 7469 6e67  name: avg_rating
-00004dd0: 0a20 2020 2020 2020 2064 6573 6372 6970  .        descrip
-00004de0: 7469 6f6e 3a20 4176 6572 6167 6520 7261  tion: Average ra
-00004df0: 7469 6e67 0a20 2020 2020 202d 206e 616d  ting.      - nam
-00004e00: 653a 2075 7064 6174 6564 5f61 740a 2020  e: updated_at.  
-00004e10: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00004e20: 6e3a 204c 6174 6573 7420 7570 6461 7465  n: Latest update
-00004e30: 2074 696d 650a 6060 600a 5573 6520 6064   time.```.Use `d
-00004e40: 6274 2064 6f63 7320 6765 6e65 7261 7465  bt docs generate
-00004e50: 6020 746f 2067 656e 6572 6174 6520 7468  ` to generate th
-00004e60: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
-00004e70: 666f 7220 796f 7572 206d 6f64 656c 7320  for your models 
-00004e80: 2620 6064 6274 2064 6f63 7320 7365 7276  & `dbt docs serv
-00004e90: 6560 2074 6f20 7365 7276 6520 7468 6520  e` to serve the 
-00004ea0: 646f 6375 6d65 6e74 6174 696f 6e20 696e  documentation in
-00004eb0: 200a 796f 7572 206c 6f63 616c 2062 726f   .your local bro
-00004ec0: 7773 6572 206f 6e20 706f 7274 2038 3030  wser on port 800
-00004ed0: 302e 0a21 5b44 6f63 5d28 2e2f 6578 616d  0..![Doc](./exam
-00004ee0: 706c 6573 2f31 305f 646f 6373 2e70 6e67  ples/10_docs.png
-00004ef0: 290a 2320 4c6f 6361 6c20 4465 7665 6c6f  ).# Local Develo
-00004f00: 706d 656e 740a 5570 6461 7465 2060 7465  pment.Update `te
-00004f10: 7374 732f 696e 7465 6772 6174 696f 6e2f  sts/integration/
-00004f20: 636f 6e66 6573 742e 7079 6020 6669 6c65  confest.py` file
-00004f30: 2074 6f20 696e 636c 7564 6520 796f 7572   to include your
-00004f40: 2063 6f6e 6e65 6374 696f 6e20 6372 6564   connection cred
-00004f50: 656e 7469 616c 732e 2046 6f72 2072 756e  entials. For run
-00004f60: 6e69 6e67 2074 6573 7473 206c 6f63 616c  ning tests local
-00004f70: 6c79 2c20 666f 6c6c 6f77 200a 7468 6573  ly, follow .thes
-00004f80: 6520 7374 6570 733a 0a60 6060 636f 6d6d  e steps:.```comm
-00004f90: 616e 646c 696e 650a 7069 7020 696e 7374  andline.pip inst
-00004fa0: 616c 6c20 2d72 2064 6576 5f72 6571 7569  all -r dev_requi
-00004fb0: 7265 6d65 6e74 732e 7478 740a 7079 7468  rements.txt.pyth
-00004fc0: 6f6e 202d 6d20 7079 7465 7374 0a60 6060  on -m pytest.```
-00004fd0: 0a23 204f 7269 6769 6e61 6c20 4175 7468  .# Original Auth
-00004fe0: 6f72 0a42 7974 6548 6f75 7365 2077 616e  or.ByteHouse wan
-00004ff0: 7473 2074 6f20 7468 616e 6b20 436c 6963  ts to thank Clic
-00005000: 6b48 6f75 7365 2066 6f72 206f 7269 6769  kHouse for origi
-00005010: 6e61 6c20 636f 6e74 7269 6275 7469 6f6e  nal contribution
-00005020: 2074 6f20 7468 6973 2063 6f6e 6e65 6374   to this connect
-00005030: 6f72 2e0a 0a23 204c 6963 656e 7365 0a54  or...# License.T
-00005040: 6869 7320 7072 6f6a 6563 7420 6973 2064  his project is d
-00005050: 6973 7472 6962 7574 6564 2075 6e64 6572  istributed under
-00005060: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
-00005070: 6520 4170 6163 6865 204c 6963 656e 7365  e Apache License
-00005080: 2028 5665 7273 696f 6e20 322e 3029 2e0a   (Version 2.0)..
+00000000: 2320 496e 7472 6f64 7563 7469 6f6e 0a60  # Introduction.`
+00000010: 6462 7460 2028 4461 7461 2042 7569 6c64  dbt` (Data Build
+00000020: 696e 6720 546f 6f6c 2920 6973 2061 6e20  ing Tool) is an 
+00000030: 6f70 656e 2073 6f75 7263 6520 746f 6f6c  open source tool
+00000040: 2074 6861 7420 656e 6162 6c65 7320 6461   that enables da
+00000050: 7461 2061 6e61 6c79 7374 7320 616e 6420  ta analysts and 
+00000060: 656e 6769 6e65 6572 7320 746f 2074 7261  engineers to tra
+00000070: 6e73 666f 726d 0a64 6174 6120 696e 2074  nsform.data in t
+00000080: 6865 6972 2077 6172 6568 6f75 7365 7320  heir warehouses 
+00000090: 7369 6d70 6c79 2062 7920 7772 6974 696e  simply by writin
+000000a0: 6720 7365 6c65 6374 2073 7461 7465 6d65  g select stateme
+000000b0: 6e74 732e 2060 6462 7460 2070 6572 666f  nts. `dbt` perfo
+000000c0: 726d 7320 7468 6520 5420 2854 7261 6e73  rms the T (Trans
+000000d0: 666f 726d 2920 6f66 2045 544c 2061 6e64  form) of ETL and
+000000e0: 0a61 6c6c 6f77 7320 636f 6d70 616e 6965  .allows companie
+000000f0: 7320 746f 2077 7269 7465 2074 7261 6e73  s to write trans
+00000100: 666f 726d 6174 696f 6e73 2061 7320 7175  formations as qu
+00000110: 6572 6965 7320 616e 6420 6f72 6368 6573  eries and orches
+00000120: 7472 6174 6520 7468 656d 2069 6e20 6120  trate them in a 
+00000130: 6d6f 7265 2065 6666 6963 6965 6e74 2077  more efficient w
+00000140: 6179 2e20 0a42 7974 6548 6f75 7365 2064  ay. .ByteHouse d
+00000150: 6274 2063 6f6e 6e65 6374 6f72 2069 7320  bt connector is 
+00000160: 6120 706c 7567 696e 2065 6e61 626c 696e  a plugin enablin
+00000170: 6720 7573 6572 7320 746f 2062 7569 6c64  g users to build
+00000180: 2074 6865 6972 2064 6174 6120 7761 7265   their data ware
+00000190: 686f 7573 6520 6563 6f73 7973 7465 6d20  house ecosystem 
+000001a0: 7769 7468 2064 6274 200a 616e 6420 4279  with dbt .and By
+000001b0: 7465 486f 7573 652e 200a 2320 5461 626c  teHouse. .# Tabl
+000001c0: 6520 6f66 2043 6f6e 7465 6e74 730a 2d20  e of Contents.- 
+000001d0: 5b49 6e74 726f 6475 6374 696f 6e5d 2823  [Introduction](#
+000001e0: 696e 7472 6f64 7563 7469 6f6e 290a 2d20  introduction).- 
+000001f0: 5b52 6571 7569 7265 6d65 6e74 735d 2823  [Requirements](#
+00000200: 7265 7175 6972 656d 656e 7473 290a 2d20  requirements).- 
+00000210: 5b43 7265 6174 696e 6720 4279 7465 486f  [Creating ByteHo
+00000220: 7573 6520 4163 636f 756e 745d 2823 6372  use Account](#cr
+00000230: 6561 7469 6e67 2d62 7974 6568 6f75 7365  eating-bytehouse
+00000240: 2d61 6363 6f75 6e74 290a 2d20 5b49 6e73  -account).- [Ins
+00000250: 7461 6c6c 6174 696f 6e5d 2823 696e 7374  tallation](#inst
+00000260: 616c 6c61 7469 6f6e 290a 2d20 5b64 6274  allation).- [dbt
+00000270: 2050 726f 6a65 6374 2053 6574 7570 5d28   Project Setup](
+00000280: 2364 6274 2d70 726f 6a65 6374 2d73 6574  #dbt-project-set
+00000290: 7570 290a 2020 2a20 5b64 6274 5f70 726f  up).  * [dbt_pro
+000002a0: 6a65 6374 2e79 6d6c 5d28 2364 6274 2d70  ject.yml](#dbt-p
+000002b0: 726f 6a65 6374 796d 6c29 0a20 202a 205b  rojectyml).  * [
+000002c0: 7072 6f66 696c 6573 2e79 6d6c 5d28 2370  profiles.yml](#p
+000002d0: 726f 6669 6c65 7379 6d6c 290a 2020 2a20  rofilesyml).  * 
+000002e0: 5b43 6f6e 6e65 6374 696f 6e20 2620 4175  [Connection & Au
+000002f0: 7468 656e 7469 6361 7469 6f6e 2043 6f6e  thentication Con
+00000300: 6669 6775 7261 7469 6f6e 735d 2823 636f  figurations](#co
+00000310: 6e6e 6563 7469 6f6e 2d2d 2d61 7574 6865  nnection---authe
+00000320: 6e74 6963 6174 696f 6e2d 636f 6e66 6967  ntication-config
+00000330: 7572 6174 696f 6e73 290a 2020 2020 2b20  urations).    + 
+00000340: 5b42 7974 6548 6f75 7365 2052 6567 696f  [ByteHouse Regio
+00000350: 6e73 5d28 2362 7974 6568 6f75 7365 2d72  ns](#bytehouse-r
+00000360: 6567 696f 6e73 290a 2020 2020 2b20 5b52  egions).    + [R
+00000370: 6567 696f 6e20 2620 5061 7373 776f 7264  egion & Password
+00000380: 2043 6f6e 6669 6775 7261 7469 6f6e 5d28   Configuration](
+00000390: 2372 6567 696f 6e2d 2d2d 7061 7373 776f  #region---passwo
+000003a0: 7264 2d63 6f6e 6669 6775 7261 7469 6f6e  rd-configuration
+000003b0: 290a 2020 2020 2b20 5b52 6567 696f 6e20  ).    + [Region 
+000003c0: 2620 4150 4920 4b65 7920 436f 6e66 6967  & API Key Config
+000003d0: 7572 6174 696f 6e5d 2823 7265 6769 6f6e  uration](#region
+000003e0: 2d2d 2d61 7069 2d6b 6579 2d63 6f6e 6669  ---api-key-confi
+000003f0: 6775 7261 7469 6f6e 290a 2020 2020 2b20  guration).    + 
+00000400: 5b48 6f73 7420 4164 6472 6573 7320 2620  [Host Address & 
+00000410: 5061 7373 776f 7264 2043 6f6e 6669 6775  Password Configu
+00000420: 7261 7469 6f6e 5d28 2368 6f73 742d 6164  ration](#host-ad
+00000430: 6472 6573 732d 2d2d 7061 7373 776f 7264  dress---password
+00000440: 2d63 6f6e 6669 6775 7261 7469 6f6e 290a  -configuration).
+00000450: 2020 2020 2b20 5b48 6f73 7420 4164 6472      + [Host Addr
+00000460: 6573 7320 2620 4150 4920 4b65 7920 436f  ess & API Key Co
+00000470: 6e66 6967 7572 6174 696f 6e5d 2823 686f  nfiguration](#ho
+00000480: 7374 2d61 6464 7265 7373 2d2d 2d61 7069  st-address---api
+00000490: 2d6b 6579 2d63 6f6e 6669 6775 7261 7469  -key-configurati
+000004a0: 6f6e 290a 2020 2a20 5b50 726f 6a65 6374  on).  * [Project
+000004b0: 2049 6e69 7469 616c 697a 6174 696f 6e5d   Initialization]
+000004c0: 2823 7072 6f6a 6563 742d 696e 6974 6961  (#project-initia
+000004d0: 6c69 7a61 7469 6f6e 290a 2020 2a20 5b54  lization).  * [T
+000004e0: 6573 7420 5761 7265 686f 7573 6520 436f  est Warehouse Co
+000004f0: 6e6e 6563 7469 6f6e 5d28 2374 6573 742d  nnection](#test-
+00000500: 7761 7265 686f 7573 652d 636f 6e6e 6563  warehouse-connec
+00000510: 7469 6f6e 290a 2d20 5b44 6174 6173 6574  tion).- [Dataset
+00000520: 2049 6e67 6573 7469 6f6e 5d28 2364 6174   Ingestion](#dat
+00000530: 6173 6574 2d69 6e67 6573 7469 6f6e 290a  aset-ingestion).
+00000540: 2d20 5b64 6274 204d 6f64 656c 735d 2823  - [dbt Models](#
+00000550: 6462 742d 6d6f 6465 6c73 290a 2d20 5b73  dbt-models).- [s
+00000560: 6368 656d 612e 796d 6c5d 2823 7363 6865  chema.yml](#sche
+00000570: 6d61 796d 6c29 0a2d 205b 4d61 7465 7269  mayml).- [Materi
+00000580: 616c 697a 6174 696f 6e20 7479 7065 7320  alization types 
+00000590: 6f66 204d 6f64 656c 735d 2823 6d61 7465  of Models](#mate
+000005a0: 7269 616c 697a 6174 696f 6e2d 7479 7065  rialization-type
+000005b0: 732d 6f66 2d6d 6f64 656c 7329 0a20 202a  s-of-models).  *
+000005c0: 205b 5669 6577 204d 6174 6572 6961 6c69   [View Materiali
+000005d0: 7a61 7469 6f6e 735d 2823 7669 6577 2d6d  zations](#view-m
+000005e0: 6174 6572 6961 6c69 7a61 7469 6f6e 7329  aterializations)
+000005f0: 0a20 202a 205b 5461 626c 6520 4d61 7465  .  * [Table Mate
+00000600: 7269 616c 697a 6174 696f 6e73 5d28 2374  rializations](#t
+00000610: 6162 6c65 2d6d 6174 6572 6961 6c69 7a61  able-materializa
+00000620: 7469 6f6e 7329 0a20 202a 205b 496e 6372  tions).  * [Incr
+00000630: 656d 656e 7461 6c20 4d61 7465 7269 616c  emental Material
+00000640: 697a 6174 696f 6e73 5d28 2369 6e63 7265  izations](#incre
+00000650: 6d65 6e74 616c 2d6d 6174 6572 6961 6c69  mental-materiali
+00000660: 7a61 7469 6f6e 7329 0a20 2020 202b 205b  zations).    + [
+00000670: 486f 7720 6974 2077 6f72 6b73 5d28 2368  How it works](#h
+00000680: 6f77 2d69 742d 776f 726b 7329 0a2d 205b  ow-it-works).- [
+00000690: 5072 6f6a 6563 7420 446f 6375 6d65 6e74  Project Document
+000006a0: 6174 696f 6e5d 2823 7072 6f6a 6563 742d  ation](#project-
+000006b0: 646f 6375 6d65 6e74 6174 696f 6e29 0a2d  documentation).-
+000006c0: 205b 4c6f 6361 6c20 4465 7665 6c6f 706d   [Local Developm
+000006d0: 656e 745d 2823 6c6f 6361 6c2d 6465 7665  ent](#local-deve
+000006e0: 6c6f 706d 656e 7429 0a2d 205b 4f72 6967  lopment).- [Orig
+000006f0: 696e 616c 2041 7574 686f 725d 2823 6f72  inal Author](#or
+00000700: 6967 696e 616c 2d61 7574 686f 7229 0a2d  iginal-author).-
+00000710: 205b 4c69 6365 6e73 655d 2823 6c69 6365   [License](#lice
+00000720: 6e73 6529 0a23 2052 6571 7569 7265 6d65  nse).# Requireme
+00000730: 6e74 730a 4d61 6b65 2073 7572 6520 796f  nts.Make sure yo
+00000740: 7520 6861 7665 2060 6462 7460 2026 2060  u have `dbt` & `
+00000750: 7079 7468 6f6e 6020 696e 7374 616c 6c65  python` installe
+00000760: 6420 6f6e 2079 6f75 7220 6d61 6368 696e  d on your machin
+00000770: 652e 2049 6620 6e6f 742c 2074 6865 6e20  e. If not, then 
+00000780: 796f 7520 6361 6e20 666f 6c6c 6f77 2074  you can follow t
+00000790: 6869 7320 6775 6964 6520 6874 7470 733a  his guide https:
+000007a0: 2f2f 646f 6373 2e67 6574 6462 742e 636f  //docs.getdbt.co
+000007b0: 6d2f 646f 6373 2f67 6574 2d73 7461 7274  m/docs/get-start
+000007c0: 6564 2f69 6e73 7461 6c6c 6174 696f 6e0a  ed/installation.
+000007d0: 2d20 6462 7420 7631 2e37 2e30 206f 7220  - dbt v1.7.0 or 
+000007e0: 6772 6561 7465 720a 2d20 7079 7468 6f6e  greater.- python
+000007f0: 2076 332e 3720 6f72 2067 7265 6174 6572   v3.7 or greater
+00000800: 0a23 2043 7265 6174 696e 6720 4279 7465  .# Creating Byte
+00000810: 486f 7573 6520 4163 636f 756e 740a 596f  House Account.Yo
+00000820: 7520 6e65 6564 2074 6f20 6372 6561 7465  u need to create
+00000830: 2042 7974 6548 6f75 7365 2061 6363 6f75   ByteHouse accou
+00000840: 6e74 2069 6e20 6f72 6465 7220 746f 2075  nt in order to u
+00000850: 7365 2062 7974 6568 6f75 7365 2d64 6274  se bytehouse-dbt
+00000860: 2063 6f6e 6e65 6374 6f72 2e20 596f 7520   connector. You 
+00000870: 6361 6e20 7369 6d70 6c79 2063 7265 6174  can simply creat
+00000880: 6520 6120 6672 6565 2061 6363 6f75 6e74  e a free account
+00000890: 2077 6974 680a 7468 6520 7072 6f63 6573   with.the proces
+000008a0: 7320 6d65 6e74 696f 6e65 6420 696e 206f  s mentioned in o
+000008b0: 7572 206f 6666 6963 6961 6c20 7765 6273  ur official webs
+000008c0: 6974 6520 646f 6375 6d65 6e74 6174 696f  ite documentatio
+000008d0: 6e3a 2068 7474 7073 3a2f 2f64 6f63 732e  n: https://docs.
+000008e0: 6279 7465 686f 7573 652e 636c 6f75 642f  bytehouse.cloud/
+000008f0: 656e 2f64 6f63 732f 7175 6963 6b2d 7374  en/docs/quick-st
+00000900: 6172 7420 3c62 722f 3e0a 0a59 6f75 2063  art <br/>..You c
+00000910: 616e 2061 6c73 6f20 6372 6561 7465 2042  an also create B
+00000920: 7974 6548 6f75 7365 2061 6363 6f75 6e74  yteHouse account
+00000930: 2074 6872 6f75 6768 2056 6f6c 6361 6e6f   through Volcano
+00000940: 2045 6e67 696e 6520 6279 2042 7974 6544   Engine by ByteD
+00000950: 616e 6365 3a20 0a68 7474 7073 3a2f 2f77  ance: .https://w
+00000960: 7777 2e76 6f6c 6365 6e67 696e 652e 636f  ww.volcengine.co
+00000970: 6d2f 7072 6f64 7563 742f 6279 7465 686f  m/product/byteho
+00000980: 7573 652d 636c 6f75 6420 0a23 2049 6e73  use-cloud .# Ins
+00000990: 7461 6c6c 6174 696f 6e0a 4372 6561 7465  tallation.Create
+000009a0: 2061 206e 6577 2072 6570 6f73 6974 6f72   a new repositor
+000009b0: 7920 7768 6572 6520 7765 2077 696c 6c20  y where we will 
+000009c0: 696e 7374 616e 7469 6174 6520 6120 6050  instantiate a `P
+000009d0: 7974 686f 6e60 2076 6972 7475 616c 2065  ython` virtual e
+000009e0: 6e76 6972 6f6e 6d65 6e74 2e0a 6060 6063  nvironment..```c
+000009f0: 6f6d 6d61 6e64 6c69 6e65 0a6d 6b64 6972  ommandline.mkdir
+00000a00: 2064 6274 5f62 7974 6568 6f75 7365 5f64   dbt_bytehouse_d
+00000a10: 656d 6f0a 6364 2064 6274 5f62 7974 6568  emo.cd dbt_byteh
+00000a20: 6f75 7365 5f64 656d 6f0a 0a70 7974 686f  ouse_demo..pytho
+00000a30: 6e20 2d6d 2076 656e 7620 7665 6e76 0a73  n -m venv venv.s
+00000a40: 6f75 7263 6520 7665 6e76 2f62 696e 2f61  ource venv/bin/a
+00000a50: 6374 6976 6174 650a 6060 600a 4c61 7465  ctivate.```.Late
+00000a60: 7374 2072 656c 6561 7365 2076 6572 7369  st release versi
+00000a70: 6f6e 2063 616e 2062 6520 696e 7374 616c  on can be instal
+00000a80: 6c65 6420 6672 6f6d 2068 6572 653a 0a60  led from here:.`
+00000a90: 6060 636f 6d6d 616e 646c 696e 650a 7069  ``commandline.pi
+00000aa0: 7020 696e 7374 616c 6c20 6462 742d 6279  p install dbt-by
+00000ab0: 7465 686f 7573 650a 6060 600a 4375 7272  tehouse.```.Curr
+00000ac0: 656e 7420 6465 7665 6c6f 706d 656e 7420  ent development 
+00000ad0: 7665 7273 696f 6e20 6361 6e20 6265 2069  version can be i
+00000ae0: 6e73 7461 6c6c 6564 2066 726f 6d20 6865  nstalled from he
+00000af0: 7265 3a0a 6060 6063 6f6d 6d61 6e64 6c69  re:.```commandli
+00000b00: 6e65 0a70 6970 2069 6e73 7461 6c6c 2067  ne.pip install g
+00000b10: 6974 2b68 7474 7073 3a2f 2f67 6974 6875  it+https://githu
+00000b20: 622e 636f 6d2f 6279 7465 686f 7573 652d  b.com/bytehouse-
+00000b30: 636c 6f75 642f 6279 7465 686f 7573 652d  cloud/bytehouse-
+00000b40: 6462 7440 6d61 7374 6572 2365 6767 3d62  dbt@master#egg=b
+00000b50: 7974 6568 6f75 7365 2d64 7269 7665 720a  ytehouse-driver.
+00000b60: 6060 600a 4368 6563 6b20 7768 6574 6865  ```.Check whethe
+00000b70: 7220 696e 7374 616c 6c61 7469 6f6e 2069  r installation i
+00000b80: 7320 7375 6363 6573 7366 756c 2062 7920  s successful by 
+00000b90: 7665 7269 6679 696e 6720 6279 7465 686f  verifying byteho
+00000ba0: 7573 6520 6973 2061 7661 696c 6162 6c65  use is available
+00000bb0: 2075 6e64 6572 2050 6c75 6769 6e73 2e0a   under Plugins..
+00000bc0: 6060 6063 6f6d 6d61 6e64 6c69 6e65 0a64  ```commandline.d
+00000bd0: 6274 202d 2d76 6572 7369 6f6e 0a60 6060  bt --version.```
+00000be0: 0a21 5b56 6572 7369 6f6e 5d28 2e2f 6578  .![Version](./ex
+00000bf0: 616d 706c 6573 2f31 5f76 6572 7369 6f6e  amples/1_version
+00000c00: 2e70 6e67 290a 2320 6462 7420 5072 6f6a  .png).# dbt Proj
+00000c10: 6563 7420 5365 7475 700a 2323 2064 6274  ect Setup.## dbt
+00000c20: 5f70 726f 6a65 6374 2e79 6d6c 0a45 7665  _project.yml.Eve
+00000c30: 7279 2060 6462 7460 2070 726f 6a65 6374  ry `dbt` project
+00000c40: 206e 6565 6473 2061 2060 6462 745f 7072   needs a `dbt_pr
+00000c50: 6f6a 6563 742e 796d 6c60 2066 696c 6520  oject.yml` file 
+00000c60: e280 9420 7468 6973 2069 7320 686f 7720  ... this is how 
+00000c70: 6064 6274 6020 6b6e 6f77 7320 6120 6469  `dbt` knows a di
+00000c80: 7265 6374 6f72 7920 6973 2061 2060 6462  rectory is a `db
+00000c90: 7460 2070 726f 6a65 6374 2e20 6064 6274  t` project. `dbt
+00000ca0: 5f70 726f 6a65 6374 2e79 6d6c 600a 6669  _project.yml`.fi
+00000cb0: 6c65 2068 6f6c 6473 2074 6865 2063 6f6e  le holds the con
+00000cc0: 7465 7874 206f 6620 796f 7572 2070 726f  text of your pro
+00000cd0: 6a65 6374 2061 6e64 2074 656c 6c73 2060  ject and tells `
+00000ce0: 6462 7460 2068 6f77 2074 6f20 6275 696c  dbt` how to buil
+00000cf0: 6420 796f 7572 2064 6174 6120 7365 7473  d your data sets
+00000d00: 2e20 536f 6d65 2063 6f6d 6d6f 6e20 636f  . Some common co
+00000d10: 6e66 6967 7572 6174 696f 6e73 0a66 6f72  nfigurations.for
+00000d20: 2060 6462 745f 7072 6f6a 6563 742e 796d   `dbt_project.ym
+00000d30: 6c60 2061 7265 3a0a 3c74 6162 6c65 3e0a  l` are:.<table>.
+00000d40: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+00000d50: 203c 7464 3e59 414d 4c20 6b65 793c 2f74   <td>YAML key</t
+00000d60: 643e 0a20 2020 2020 2020 203c 7464 3e56  d>.        <td>V
+00000d70: 616c 7565 3c2f 7464 3e0a 2020 2020 3c2f  alue</td>.    </
+00000d80: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+00000d90: 2020 2020 203c 7464 3e6e 616d 653c 2f74       <td>name</t
+00000da0: 643e 0a20 2020 2020 2020 203c 7464 3e59  d>.        <td>Y
+00000db0: 6f75 7220 7072 6f6a 6563 74e2 8099 7320  our project...s 
+00000dc0: 6e61 6d65 2069 6e20 736e 616b 6520 6361  name in snake ca
+00000dd0: 7365 3c2f 7464 3e0a 2020 2020 3c2f 7472  se</td>.    </tr
+00000de0: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00000df0: 2020 203c 7464 3e76 6572 7369 6f6e 3c2f     <td>version</
+00000e00: 7464 3e0a 2020 2020 2020 2020 3c74 643e  td>.        <td>
+00000e10: 5665 7273 696f 6e20 6f66 2079 6f75 7220  Version of your 
+00000e20: 7072 6f6a 6563 743c 2f74 643e 0a20 2020  project</td>.   
+00000e30: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+00000e40: 2020 2020 2020 2020 3c74 643e 7072 6f66          <td>prof
+00000e50: 696c 653c 2f74 643e 0a20 2020 2020 2020  ile</td>.       
+00000e60: 203c 7464 3e54 6865 2070 726f 6669 6c65   <td>The profile
+00000e70: 2064 6274 2075 7365 7320 746f 2063 6f6e   dbt uses to con
+00000e80: 6e65 6374 2074 6f20 4279 7465 486f 7573  nect to ByteHous
+00000e90: 653c 2f74 643e 0a20 2020 203c 2f74 723e  e</td>.    </tr>
+00000ea0: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+00000eb0: 2020 3c74 643e 6d6f 6465 6c2d 7061 7468    <td>model-path
+00000ec0: 733c 2f74 643e 0a20 2020 2020 2020 203c  s</td>.        <
+00000ed0: 7464 3e44 6972 6563 746f 7269 6573 2074  td>Directories t
+00000ee0: 6f20 7768 6572 6520 796f 7572 206d 6f64  o where your mod
+00000ef0: 656c 2061 6e64 2073 6f75 7263 6520 6669  el and source fi
+00000f00: 6c65 7320 6c69 7665 3c2f 7464 3e0a 2020  les live</td>.  
+00000f10: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+00000f20: 0a20 2020 2020 2020 203c 7464 3e73 6565  .        <td>see
+00000f30: 642d 7061 7468 733c 2f74 643e 0a20 2020  d-paths</td>.   
+00000f40: 2020 2020 203c 7464 3e44 6972 6563 746f       <td>Directo
+00000f50: 7269 6573 2074 6f20 7768 6572 6520 796f  ries to where yo
+00000f60: 7572 2073 6565 6420 6669 6c65 7320 6c69  ur seed files li
+00000f70: 7665 3c2f 7464 3e0a 2020 2020 3c2f 7472  ve</td>.    </tr
+00000f80: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00000f90: 2020 203c 7464 3e74 6573 742d 7061 7468     <td>test-path
+00000fa0: 733c 2f74 643e 0a20 2020 2020 2020 203c  s</td>.        <
+00000fb0: 7464 3e44 6972 6563 746f 7269 6573 2074  td>Directories t
+00000fc0: 6f20 7768 6572 6520 796f 7572 2074 6573  o where your tes
+00000fd0: 7420 6669 6c65 7320 6c69 7665 3c2f 7464  t files live</td
+00000fe0: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+00000ff0: 3c74 723e 0a20 2020 2020 2020 203c 7464  <tr>.        <td
+00001000: 3e73 6e61 7073 686f 742d 7061 7468 733c  >snapshot-paths<
+00001010: 2f74 643e 0a20 2020 2020 2020 203c 7464  /td>.        <td
+00001020: 3e44 6972 6563 746f 7269 6573 2074 6f20  >Directories to 
+00001030: 7768 6572 6520 796f 7572 2073 6e61 7073  where your snaps
+00001040: 686f 7473 206c 6976 653c 2f74 643e 0a20  hots live</td>. 
+00001050: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+00001060: 3e0a 2020 2020 2020 2020 3c74 643e 646f  >.        <td>do
+00001070: 6373 2d70 6174 6873 3c2f 7464 3e0a 2020  cs-paths</td>.  
+00001080: 2020 2020 2020 3c74 643e 4469 7265 6374        <td>Direct
+00001090: 6f72 6965 7320 746f 2077 6865 7265 2079  ories to where y
+000010a0: 6f75 7220 646f 6373 2062 6c6f 636b 7320  our docs blocks 
+000010b0: 6c69 7665 3c2f 7464 3e0a 2020 2020 3c2f  live</td>.    </
+000010c0: 7472 3e0a 3c2f 7461 626c 653e 0a0a 2323  tr>.</table>..##
+000010d0: 2070 726f 6669 6c65 732e 796d 6c0a 5768   profiles.yml.Wh
+000010e0: 656e 2079 6f75 2069 6e76 6f6b 6520 6064  en you invoke `d
+000010f0: 6274 6020 6672 6f6d 2074 6865 2063 6f6d  bt` from the com
+00001100: 6d61 6e64 206c 696e 652c 2060 6462 7460  mand line, `dbt`
+00001110: 2070 6172 7365 7320 796f 7572 2060 6462   parses your `db
+00001120: 745f 7072 6f6a 6563 742e 796d 6c60 2061  t_project.yml` a
+00001130: 6e64 206f 6274 6169 6e73 2074 6865 2070  nd obtains the p
+00001140: 726f 6669 6c65 206e 616d 652e 2060 6462  rofile name. `db
+00001150: 7460 2074 6865 6e20 0a63 6865 636b 7320  t` then .checks 
+00001160: 796f 7572 2060 7072 6f66 696c 6573 2e79  your `profiles.y
+00001170: 6d6c 6020 6669 6c65 2066 6f72 2061 2070  ml` file for a p
+00001180: 726f 6669 6c65 2077 6974 6820 7468 6520  rofile with the 
+00001190: 7361 6d65 206e 616d 652e 2041 2070 726f  same name. A pro
+000011a0: 6669 6c65 2063 6f6e 7461 696e 7320 616c  file contains al
+000011b0: 6c20 7468 6520 6465 7461 696c 732f 6372  l the details/cr
+000011c0: 6564 656e 7469 616c 7320 0a72 6571 7569  edentials .requi
+000011d0: 7265 6420 746f 2063 6f6e 6e65 6374 2074  red to connect t
+000011e0: 6f20 4279 7465 486f 7573 652e 2060 6462  o ByteHouse. `db
+000011f0: 7460 2077 696c 6c20 7365 6172 6368 2074  t` will search t
+00001200: 6865 2063 7572 7265 6e74 2077 6f72 6b69  he current worki
+00001210: 6e67 2064 6972 6563 746f 7279 2066 6f72  ng directory for
+00001220: 2074 6865 2060 7072 6f66 696c 6573 2e79   the `profiles.y
+00001230: 6d6c 6020 6669 6c65 2061 6e64 2077 696c  ml` file and wil
+00001240: 6c0a 6465 6661 756c 7420 746f 2074 6865  l.default to the
+00001250: 2060 7e2f 2e64 6274 2f20 6469 7265 6374   `~/.dbt/ direct
+00001260: 6f72 7960 2069 6620 6e6f 7420 666f 756e  ory` if not foun
+00001270: 642e 0a60 6060 7961 6d6c 0a3c 7072 6f66  d..```yaml.<prof
+00001280: 696c 652d 6e61 6d65 3e3a 0a20 2074 6172  ile-name>:.  tar
+00001290: 6765 743a 203c 7461 7267 6574 2d6e 616d  get: <target-nam
+000012a0: 653e 0a20 206f 7574 7075 7473 3a0a 2020  e>.  outputs:.  
+000012b0: 2020 3c74 6172 6765 742d 6e61 6d65 3e3a    <target-name>:
+000012c0: 0a20 2020 2020 2074 7970 653a 2062 7974  .      type: byt
+000012d0: 6568 6f75 7365 0a20 2020 2020 2073 6368  ehouse.      sch
+000012e0: 656d 613a 203c 6461 7461 6261 7365 2d6e  ema: <database-n
+000012f0: 616d 653e 0a20 2020 2020 2075 7365 723a  ame>.      user:
+00001300: 2062 7974 6568 6f75 7365 0a20 2020 2020   bytehouse.     
+00001310: 2070 6173 7377 6f72 643a 203c 6279 7465   password: <byte
+00001320: 686f 7573 652d 6170 692d 6b65 793e 0a20  house-api-key>. 
+00001330: 2020 2020 2064 7269 7665 723a 206e 6174       driver: nat
+00001340: 6976 650a 2020 2020 2020 236f 7074 696f  ive.      #optio
+00001350: 6e61 6c20 6669 656c 6473 0a20 2020 2020  nal fields.     
+00001360: 2068 6f73 743a 203c 686f 7374 6e61 6d65   host: <hostname
+00001370: 3e0a 2020 2020 2020 706f 7274 3a20 3c70  >.      port: <p
+00001380: 6f72 743e 0a20 2020 2020 2072 6567 696f  ort>.      regio
+00001390: 6e3a 203c 7265 6769 6f6e 2d6e 616d 653e  n: <region-name>
+000013a0: 0a20 2020 2020 2077 6172 6568 6f75 7365  .      warehouse
+000013b0: 3a20 3c77 6172 6568 6f75 7365 2d6e 616d  : <warehouse-nam
+000013c0: 653e 0a20 2020 2020 2072 6574 7269 6573  e>.      retries
+000013d0: 3a20 310a 2020 2020 2020 7365 6375 7265  : 1.      secure
+000013e0: 3a20 5472 7565 0a20 2020 2020 2063 6f6e  : True.      con
+000013f0: 6e65 6374 5f74 696d 656f 7574 3a20 3130  nect_timeout: 10
+00001400: 0a20 2020 2020 2073 656e 645f 7265 6365  .      send_rece
+00001410: 6976 655f 7469 6d65 6f75 743a 2033 3030  ive_timeout: 300
+00001420: 0a20 2020 2020 2063 7573 746f 6d5f 7365  .      custom_se
+00001430: 7474 696e 6773 3a20 3c65 6d70 7479 3e0a  ttings: <empty>.
+00001440: 6060 600a 3c74 6162 6c65 3e0a 2020 2020  ```.<table>.    
+00001450: 3c74 723e 0a20 2020 2020 2020 203c 7464  <tr>.        <td
+00001460: 3e59 414d 4c20 6b65 793c 2f74 643e 0a20  >YAML key</td>. 
+00001470: 2020 2020 2020 203c 7464 3e56 616c 7565         <td>Value
+00001480: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+00001490: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+000014a0: 203c 7464 3e26 6c74 3b70 726f 6669 6c65   <td>&lt;profile
+000014b0: 2d6e 616d 6526 6774 3b3c 2f74 643e 0a20  -name&gt;</td>. 
+000014c0: 2020 2020 2020 203c 7464 3e4e 616d 6520         <td>Name 
+000014d0: 6f66 2074 6865 2070 726f 6669 6c65 2e20  of the profile. 
+000014e0: 4861 7320 746f 2062 6520 7468 6520 7361  Has to be the sa
+000014f0: 6d65 206e 616d 6520 6173 2074 6865 2070  me name as the p
+00001500: 726f 6669 6c65 2069 6e64 6963 6174 6564  rofile indicated
+00001510: 2069 6e20 796f 7572 2064 6274 5f70 726f   in your dbt_pro
+00001520: 6a65 6374 2e79 6d6c 2066 696c 653c 2f74  ject.yml file</t
+00001530: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+00001540: 203c 7472 3e0a 2020 2020 2020 2020 3c74   <tr>.        <t
+00001550: 643e 7461 7267 6574 3c2f 7464 3e0a 2020  d>target</td>.  
+00001560: 2020 2020 2020 3c74 643e 4465 6661 756c        <td>Defaul
+00001570: 7420 7461 7267 6574 2079 6f75 7220 6462  t target your db
+00001580: 7420 7072 6f6a 6563 7420 7769 6c6c 2075  t project will u
+00001590: 7365 2e20 4974 206d 7573 7420 6265 206f  se. It must be o
+000015a0: 6e65 206f 6620 7468 6520 7461 7267 6574  ne of the target
+000015b0: 7320 796f 7520 6465 6669 6e65 2069 6e20  s you define in 
+000015c0: 796f 7572 2070 726f 6669 6c65 3c2f 7464  your profile</td
+000015d0: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+000015e0: 3c74 723e 0a20 2020 2020 2020 203c 7464  <tr>.        <td
+000015f0: 3e74 7970 653c 2f74 643e 0a20 2020 2020  >type</td>.     
+00001600: 2020 203c 7464 3e4d 7573 7420 6265 2073     <td>Must be s
+00001610: 6574 2074 6f20 6279 7465 686f 7573 653c  et to bytehouse<
+00001620: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+00001630: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
+00001640: 3c74 643e 7363 6865 6d61 3c2f 7464 3e0a  <td>schema</td>.
+00001650: 2020 2020 2020 2020 3c74 643e 4461 7461          <td>Data
+00001660: 6261 7365 206e 616d 653c 2f74 643e 0a20  base name</td>. 
+00001670: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+00001680: 3e0a 2020 2020 2020 2020 3c74 643e 7573  >.        <td>us
+00001690: 6572 3c2f 7464 3e0a 2020 2020 2020 2020  er</td>.        
+000016a0: 3c74 643e 4d75 7374 2062 6520 7365 7420  <td>Must be set 
+000016b0: 746f 2062 7974 6568 6f75 7365 3c2f 7464  to bytehouse</td
+000016c0: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+000016d0: 3c74 723e 0a20 2020 2020 2020 203c 7464  <tr>.        <td
+000016e0: 3e70 6173 7377 6f72 643c 2f74 643e 0a20  >password</td>. 
+000016f0: 2020 2020 2020 203c 7464 3e42 7974 6548         <td>ByteH
+00001700: 6f75 7365 2041 5049 2054 6f6b 656e 3c2f  ouse API Token</
+00001710: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+00001720: 2020 3c74 723e 0a20 2020 2020 2020 203c    <tr>.        <
+00001730: 7464 3e64 7269 7665 723c 2f74 643e 0a20  td>driver</td>. 
+00001740: 2020 2020 2020 203c 7464 3e4d 7573 7420         <td>Must 
+00001750: 6265 2073 6574 2074 6f20 6e61 7469 7665  be set to native
+00001760: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+00001770: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+00001780: 203c 7464 3e68 6f73 743c 2f74 643e 0a20   <td>host</td>. 
+00001790: 2020 2020 2020 203c 7464 3e5b 4f70 7469         <td>[Opti
+000017a0: 6f6e 616c 5d20 5468 6520 686f 7374 206e  onal] The host n
+000017b0: 616d 6520 6f66 2074 6865 2063 6f6e 6e65  ame of the conne
+000017c0: 6374 696f 6e3c 2f74 643e 0a20 2020 203c  ction</td>.    <
+000017d0: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
+000017e0: 2020 2020 2020 3c74 643e 706f 7274 203c        <td>port <
+000017f0: 2f74 643e 0a20 2020 2020 2020 203c 7464  /td>.        <td
+00001800: 3e5b 4f70 7469 6f6e 616c 5d20 5468 6520  >[Optional] The 
+00001810: 706f 7274 206e 756d 6265 7220 6f66 2074  port number of t
+00001820: 6865 2068 6f73 7420 7365 7276 6572 3c2f  he host server</
+00001830: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+00001840: 2020 3c74 723e 0a20 2020 2020 2020 203c    <tr>.        <
+00001850: 7464 3e77 6172 6568 6f75 7365 3c2f 7464  td>warehouse</td
+00001860: 3e0a 2020 2020 2020 2020 3c74 643e 5b4f  >.        <td>[O
+00001870: 7074 696f 6e61 6c5d 2054 6865 206e 616d  ptional] The nam
+00001880: 6520 6f66 2074 6865 2076 6972 7475 616c  e of the virtual
+00001890: 2077 6172 6568 6f75 7365 2074 6861 7420   warehouse that 
+000018a0: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
+000018b0: 666f 7220 7468 6973 2073 6573 7369 6f6e  for this session
+000018c0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000018d0: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+000018e0: 203c 7464 3e72 6574 7269 6573 3c2f 7464   <td>retries</td
+000018f0: 3e0a 2020 2020 2020 2020 3c74 643e 5b4f  >.        <td>[O
+00001900: 7074 696f 6e61 6c5d 204e 756d 6265 7220  ptional] Number 
+00001910: 6f66 2074 696d 6573 2074 6f20 7265 7472  of times to retr
+00001920: 7920 7468 6520 696e 6974 6961 6c20 636f  y the initial co
+00001930: 6e6e 6563 7469 6f6e 2061 7474 656d 7074  nnection attempt
+00001940: 2069 6620 7468 6520 6572 726f 7220 6170   if the error ap
+00001950: 7065 6172 7320 746f 2062 6520 7265 636f  pears to be reco
+00001960: 7665 7261 626c 653c 2f74 643e 0a20 2020  verable</td>.   
+00001970: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+00001980: 2020 2020 2020 2020 3c74 643e 7365 6375          <td>secu
+00001990: 7265 3c2f 7464 3e0a 2020 2020 2020 2020  re</td>.        
+000019a0: 3c74 643e 5b4f 7074 696f 6e61 6c5d 2057  <td>[Optional] W
+000019b0: 6865 7468 6572 2074 6865 2063 6f6e 6e65  hether the conne
+000019c0: 6374 696f 6e20 6973 2073 6563 7572 6564  ction is secured
+000019d0: 2062 7920 544c 532e 2053 7567 6765 7374   by TLS. Suggest
+000019e0: 6564 2074 6f20 7365 7420 6974 2074 6f20  ed to set it to 
+000019f0: 5472 7565 3c2f 7464 3e0a 2020 2020 3c2f  True</td>.    </
+00001a00: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+00001a10: 2020 2020 203c 7464 3e63 6f6e 6e65 6374       <td>connect
+00001a20: 5f74 696d 656f 7574 3c2f 7464 3e0a 2020  _timeout</td>.  
+00001a30: 2020 2020 2020 3c74 643e 5b4f 7074 696f        <td>[Optio
+00001a40: 6e61 6c5d 2043 6f6e 6e65 6374 696f 6e20  nal] Connection 
+00001a50: 7469 6d65 6f75 7420 696e 2073 6563 6f6e  timeout in secon
+00001a60: 6473 2e20 4465 6661 756c 7420 6973 2031  ds. Default is 1
+00001a70: 3020 7365 636f 6e64 733c 2f74 643e 0a20  0 seconds</td>. 
+00001a80: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+00001a90: 3e0a 2020 2020 2020 2020 3c74 643e 7365  >.        <td>se
+00001aa0: 6e64 5f72 6563 6569 7665 5f74 696d 656f  nd_receive_timeo
+00001ab0: 7574 3c2f 7464 3e0a 2020 2020 2020 2020  ut</td>.        
+00001ac0: 3c74 643e 5b4f 7074 696f 6e61 6c5d 2054  <td>[Optional] T
+00001ad0: 696d 656f 7574 2066 6f72 2072 6563 6569  imeout for recei
+00001ae0: 7669 6e67 2064 6174 6120 6672 6f6d 206f  ving data from o
+00001af0: 7220 7365 6e64 696e 6720 6461 7461 2074  r sending data t
+00001b00: 6f20 4279 7465 486f 7573 652e 2044 6566  o ByteHouse. Def
+00001b10: 6175 6c74 2069 7320 3520 6d69 6e75 7465  ault is 5 minute
+00001b20: 7320 2833 3030 2073 6563 6f6e 6473 293c  s (300 seconds)<
+00001b30: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+00001b40: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
+00001b50: 3c74 643e 6375 7374 6f6d 5f73 6574 7469  <td>custom_setti
+00001b60: 6e67 733c 2f74 643e 0a20 2020 2020 2020  ngs</td>.       
+00001b70: 203c 7464 3e5b 4f70 7469 6f6e 616c 5d20   <td>[Optional] 
+00001b80: 4120 6d61 7070 696e 6720 6f66 2042 7974  A mapping of Byt
+00001b90: 6548 6f75 7365 2073 7065 6369 6669 6320  eHouse specific 
+00001ba0: 7573 6572 2073 6574 7469 6e67 7320 746f  user settings to
+00001bb0: 2075 7365 2077 6974 6820 7468 6520 636f   use with the co
+00001bc0: 6e6e 6563 7469 6f6e 3c2f 7464 3e0a 2020  nnection</td>.  
+00001bd0: 2020 3c2f 7472 3e0a 3c2f 7461 626c 653e    </tr>.</table>
+00001be0: 0a0a 2323 2043 6f6e 6e65 6374 696f 6e20  ..## Connection 
+00001bf0: 2620 4175 7468 656e 7469 6361 7469 6f6e  & Authentication
+00001c00: 2043 6f6e 6669 6775 7261 7469 6f6e 730a   Configurations.
+00001c10: 2323 2320 486f 7374 2041 6464 7265 7373  ### Host Address
+00001c20: 2026 2041 5049 204b 6579 2043 6f6e 6669   & API Key Confi
+00001c30: 6775 7261 7469 6f6e 0a52 6571 7569 7265  guration.Require
+00001c40: 6420 7061 7261 6d65 7465 7273 3a20 6068  d parameters: `h
+00001c50: 6f73 7460 2060 706f 7274 6020 6075 7365  ost` `port` `use
+00001c60: 7260 2060 7061 7373 776f 7264 600a 6060  r` `password`.``
+00001c70: 6079 616d 6c0a 6279 7465 686f 7573 655f  `yaml.bytehouse_
+00001c80: 7072 6f66 696c 653a 0a20 2074 6172 6765  profile:.  targe
+00001c90: 743a 2064 6576 0a20 206f 7574 7075 7473  t: dev.  outputs
+00001ca0: 3a0a 2020 2020 6465 763a 0a20 2020 2020  :.    dev:.     
+00001cb0: 2074 7970 653a 2062 7974 6568 6f75 7365   type: bytehouse
+00001cc0: 0a20 2020 2020 2064 7269 7665 723a 206e  .      driver: n
+00001cd0: 6174 6976 650a 0a20 2020 2020 2023 2064  ative..      # d
+00001ce0: 6174 6162 6173 650a 2020 2020 2020 7363  atabase.      sc
+00001cf0: 6865 6d61 3a20 2444 4154 4142 4153 455f  hema: $DATABASE_
+00001d00: 4e41 4d45 0a0a 2020 2020 2020 2320 7461  NAME..      # ta
+00001d10: 7267 6574 2073 6572 7665 7220 6164 6472  rget server addr
+00001d20: 6573 730a 2020 2020 2020 686f 7374 3a20  ess.      host: 
+00001d30: 2448 4f53 545f 4144 4452 4553 5320 200a  $HOST_ADDRESS  .
+00001d40: 2020 2020 2020 706f 7274 3a20 2450 4f52        port: $POR
+00001d50: 545f 4e55 4d42 4552 0a0a 2020 2020 2020  T_NUMBER..      
+00001d60: 2320 6163 636f 756e 7420 6372 6564 656e  # account creden
+00001d70: 7469 616c 730a 2020 2020 2020 7573 6572  tials.      user
+00001d80: 3a20 6279 7465 686f 7573 650a 2020 2020  : bytehouse.    
+00001d90: 2020 7061 7373 776f 7264 3a20 2441 5049    password: $API
+00001da0: 5f4b 4559 0a0a 2020 2020 2020 2320 6164  _KEY..      # ad
+00001db0: 6469 7469 6f6e 616c 2073 6574 7469 6e67  ditional setting
+00001dc0: 730a 2020 2020 2020 7365 6375 7265 3a20  s.      secure: 
+00001dd0: 5472 7565 0a60 6060 0a23 2320 5072 6f6a  True.```.## Proj
+00001de0: 6563 7420 496e 6974 6961 6c69 7a61 7469  ect Initializati
+00001df0: 6f6e 0a60 6462 7420 696e 6974 6020 636f  on.`dbt init` co
+00001e00: 6d6d 616e 6420 7769 6c6c 2070 726f 6d70  mmand will promp
+00001e10: 7420 666f 7220 7072 6f6a 6563 7420 6e61  t for project na
+00001e20: 6d65 2026 2064 6174 6162 6173 6520 6164  me & database ad
+00001e30: 6170 7465 7273 2c20 7768 6572 6520 796f  apters, where yo
+00001e40: 7520 6861 7665 2074 6f20 7365 6c65 6374  u have to select
+00001e50: 2062 7974 6568 6f75 7365 2e20 5468 6973   bytehouse. This
+00001e60: 2077 696c 6c20 6372 6561 7465 0a61 206e   will create.a n
+00001e70: 6577 2066 6f6c 6465 7220 7769 7468 2079  ew folder with y
+00001e80: 6f75 7220 7072 6f6a 6563 7420 6e61 6d65  our project name
+00001e90: 2c20 7361 6d70 6c65 2066 696c 6573 2026  , sample files &
+00001ea0: 2060 6462 745f 7072 6f6a 6563 742e 796d   `dbt_project.ym
+00001eb0: 6c60 2063 6f6e 6669 6720 6669 6c65 2c20  l` config file, 
+00001ec0: 656e 6f75 6768 2074 6f20 6765 7420 796f  enough to get yo
+00001ed0: 7520 7374 6172 7465 6420 7769 7468 2064  u started with d
+00001ee0: 6274 2e0a 6060 6063 6f6d 6d61 6e64 6c69  bt..```commandli
+00001ef0: 6e65 0a64 6274 2069 6e69 740a 6060 600a  ne.dbt init.```.
+00001f00: 215b 496e 6974 5d28 2e2f 6578 616d 706c  ![Init](./exampl
+00001f10: 6573 2f32 5f70 726f 6669 6c65 732e 706e  es/2_profiles.pn
+00001f20: 6729 0a55 7064 6174 6520 796f 7572 2070  g).Update your p
+00001f30: 726f 6669 6c65 732e 796d 6c20 7769 7468  rofiles.yml with
+00001f40: 2072 6571 7569 7265 6420 6175 7468 656e   required authen
+00001f50: 7469 6361 7469 6f6e 2026 2074 6172 6765  tication & targe
+00001f60: 7420 7365 7276 6572 2063 7265 6465 6e74  t server credent
+00001f70: 6961 6c73 2e20 0a60 6060 636f 6d6d 616e  ials. .```comman
+00001f80: 646c 696e 650a 6e61 6e6f 207e 2f2e 6462  dline.nano ~/.db
+00001f90: 742f 7072 6f66 696c 6573 2e79 6d6c 0a60  t/profiles.yml.`
+00001fa0: 6060 0a41 7320 6064 6274 6020 6861 7320  ``.As `dbt` has 
+00001fb0: 6372 6561 7465 6420 6120 6e65 7720 666f  created a new fo
+00001fc0: 6c64 6572 2077 6974 6820 7468 6520 7361  lder with the sa
+00001fd0: 6d65 206e 616d 6520 6173 2079 6f75 7220  me name as your 
+00001fe0: 7072 6f6a 6563 7420 6e61 6d65 2c20 6368  project name, ch
+00001ff0: 616e 6765 2079 6f75 7220 6375 7272 656e  ange your curren
+00002000: 7420 0a64 6972 6563 746f 7279 2074 6f20  t .directory to 
+00002010: 7468 6520 7072 6f6a 6563 7420 666f 6c64  the project fold
+00002020: 6572 2e20 0a60 6060 636f 6d6d 616e 646c  er. .```commandl
+00002030: 696e 650a 6364 2064 6274 5f62 7974 6568  ine.cd dbt_byteh
+00002040: 6f75 7365 5f64 656d 6f0a 6060 600a 5570  ouse_demo.```.Up
+00002050: 6461 7465 2079 6f75 7220 6064 6274 5f70  date your `dbt_p
+00002060: 726f 6a65 6374 2e79 6d6c 6020 6669 6c65  roject.yml` file
+00002070: 2074 6f20 6861 7665 2074 6865 2073 616d   to have the sam
+00002080: 6520 7072 6f66 696c 655f 6e61 6d65 2061  e profile_name a
+00002090: 7320 607e 2f2e 6462 742f 7072 6f66 696c  s `~/.dbt/profil
+000020a0: 6573 2e79 6d6c 602e 0a60 6060 636f 6d6d  es.yml`..```comm
+000020b0: 616e 646c 696e 650a 6e61 6e6f 2064 6274  andline.nano dbt
+000020c0: 5f70 726f 6a65 6374 2e79 6d6c 0a60 6060  _project.yml.```
+000020d0: 0a21 5b50 726f 6a65 6374 5d28 2e2f 6578  .![Project](./ex
+000020e0: 616d 706c 6573 2f33 5f70 726f 6a65 6374  amples/3_project
+000020f0: 2e70 6e67 290a 2323 2054 6573 7420 5761  .png).## Test Wa
+00002100: 7265 686f 7573 6520 436f 6e6e 6563 7469  rehouse Connecti
+00002110: 6f6e 0a55 7365 2060 6462 7420 6465 6275  on.Use `dbt debu
+00002120: 6760 2063 6f6d 6d61 6e64 2074 6f20 7665  g` command to ve
+00002130: 7269 6679 2072 6571 7569 7265 6420 6465  rify required de
+00002140: 7065 6e64 656e 6369 6573 2026 2077 6172  pendencies & war
+00002150: 6568 6f75 7365 2063 6f6e 6e65 6374 696f  ehouse connectio
+00002160: 6e2e 2049 6e20 6361 7365 206f 6620 7375  n. In case of su
+00002170: 6363 6573 732c 2069 7420 7769 6c6c 2073  ccess, it will s
+00002180: 686f 7720 796f 7520 0a22 416c 6c20 6368  how you ."All ch
+00002190: 6563 6b73 2070 6173 7365 6421 220a 6060  ecks passed!".``
+000021a0: 6063 6f6d 6d61 6e64 6c69 6e65 0a64 6274  `commandline.dbt
+000021b0: 2064 6562 7567 0a60 6060 0a21 5b44 6562   debug.```.![Deb
+000021c0: 7567 5d28 2e2f 6578 616d 706c 6573 2f34  ug](./examples/4
+000021d0: 5f64 6562 7567 2e70 6e67 290a 2320 4461  _debug.png).# Da
+000021e0: 7461 7365 7420 496e 6765 7374 696f 6e0a  taset Ingestion.
+000021f0: 546f 2073 686f 7763 6173 6520 6469 6666  To showcase diff
+00002200: 6572 656e 7420 6064 6274 6020 6675 6e63  erent `dbt` func
+00002210: 7469 6f6e 616c 6974 6965 732c 2077 6520  tionalities, we 
+00002220: 7769 6c6c 2069 6e67 6573 7420 6120 736d  will ingest a sm
+00002230: 616c 6c20 696d 6462 206d 6f76 6965 2064  all imdb movie d
+00002240: 6174 6173 6574 2c20 7769 7468 2074 6865  ataset, with the
+00002250: 2066 6f6c 6c6f 7769 6e67 2073 6368 656d   following schem
+00002260: 612e 200a 5468 6520 4444 4c20 2620 696e  a. .The DDL & in
+00002270: 7365 7274 696f 6e20 7175 6572 6965 7320  sertion queries 
+00002280: 6361 6e20 6265 2066 6f75 6e64 2068 6572  can be found her
+00002290: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
+000022a0: 2e63 6f6d 2f62 7974 6568 6f75 7365 2d63  .com/bytehouse-c
+000022b0: 6c6f 7564 2f62 7974 6568 6f75 7365 2d64  loud/bytehouse-d
+000022c0: 6274 2f65 7861 6d70 6c65 732f 6461 7461  bt/examples/data
+000022d0: 5f6c 6f61 6469 6e67 2e73 716c 2e20 0a59  _loading.sql. .Y
+000022e0: 6f75 2063 616e 2075 7365 2042 7974 6548  ou can use ByteH
+000022f0: 6f75 7365 2053 514c 2077 6f72 6b73 6865  ouse SQL workshe
+00002300: 6574 2074 6f20 6372 6561 7465 2074 6865  et to create the
+00002310: 2073 6368 656d 6120 2620 696e 7365 7274   schema & insert
+00002320: 2074 6865 2064 6174 6173 6574 2e20 0a21   the dataset. .!
+00002330: 5b53 6368 656d 615d 282e 2f65 7861 6d70  [Schema](./examp
+00002340: 6c65 732f 355f 7363 6865 6d61 2e70 6e67  les/5_schema.png
+00002350: 290a 546f 2076 6572 6966 7920 7468 6174  ).To verify that
+00002360: 2064 6174 6173 6574 2070 7265 7061 7261   dataset prepara
+00002370: 7469 6f6e 2077 6173 2073 7563 6365 7373  tion was success
+00002380: 6675 6c2c 2077 6520 7769 6c6c 2065 7865  ful, we will exe
+00002390: 6375 7465 2074 6869 7320 666f 6c6c 6f77  cute this follow
+000023a0: 696e 6720 7175 6572 7920 746f 2073 756d  ing query to sum
+000023b0: 6d61 7269 7a65 2065 6163 6820 6163 746f  marize each acto
+000023c0: 7220 616c 6f6e 6720 0a77 6974 6820 7468  r along .with th
+000023d0: 6569 7220 746f 7461 6c20 6e75 6d62 6572  eir total number
+000023e0: 206f 6620 6d6f 7669 6520 6170 7065 6172   of movie appear
+000023f0: 616e 6365 732e 200a 6060 600a 5345 4c45  ances. .```.SELE
+00002400: 4354 2069 642c 0a20 2061 6e79 2861 6374  CT id,.  any(act
+00002410: 6f72 5f6e 616d 6529 2061 7320 6e61 6d65  or_name) as name
+00002420: 2c0a 2020 756e 6971 4578 6163 7428 6d6f  ,.  uniqExact(mo
+00002430: 7669 655f 6964 2920 2020 2061 7320 6e75  vie_id)    as nu
+00002440: 6d5f 6d6f 7669 6573 2c0a 2020 6176 6728  m_movies,.  avg(
+00002450: 7261 7469 6e67 2920 2020 2020 2020 2020  rating)         
+00002460: 2020 2020 2020 2061 7320 6176 675f 7261         as avg_ra
+00002470: 7469 6e67 2c0a 2020 6d61 7828 6372 6561  ting,.  max(crea
+00002480: 7465 645f 6174 2920 6173 2075 7064 6174  ted_at) as updat
+00002490: 6564 5f61 740a 4652 4f4d 2028 0a20 2053  ed_at.FROM (.  S
+000024a0: 454c 4543 5420 6163 746f 7273 2e69 6420  ELECT actors.id 
+000024b0: 6173 2069 642c 0a20 2020 2020 2020 636f  as id,.       co
+000024c0: 6e63 6174 2861 6374 6f72 732e 6669 7273  ncat(actors.firs
+000024d0: 745f 6e61 6d65 2c20 2720 272c 2061 6374  t_name, ' ', act
+000024e0: 6f72 732e 6c61 7374 5f6e 616d 6529 2061  ors.last_name) a
+000024f0: 7320 6163 746f 725f 6e61 6d65 2c0a 2020  s actor_name,.  
+00002500: 2020 2020 206d 6f76 6965 732e 6964 2061       movies.id a
+00002510: 7320 6d6f 7669 655f 6964 2c0a 2020 2020  s movie_id,.    
+00002520: 2020 206d 6f76 6965 732e 7261 7469 6e67     movies.rating
+00002530: 2061 7320 7261 7469 6e67 2c0a 2020 2020   as rating,.    
+00002540: 2020 2063 7265 6174 6564 5f61 740a 2020     created_at.  
+00002550: 4652 4f4d 2020 696d 6462 2e61 6374 6f72  FROM  imdb.actor
+00002560: 730a 2020 2020 2020 2020 4a4f 494e 2069  s.        JOIN i
+00002570: 6d64 622e 726f 6c65 7320 4f4e 2072 6f6c  mdb.roles ON rol
+00002580: 6573 2e61 6374 6f72 5f69 6420 3d20 6163  es.actor_id = ac
+00002590: 746f 7273 2e69 640a 2020 2020 2020 2020  tors.id.        
+000025a0: 4c45 4654 204f 5554 4552 204a 4f49 4e20  LEFT OUTER JOIN 
+000025b0: 696d 6462 2e6d 6f76 6965 7320 4f4e 206d  imdb.movies ON m
+000025c0: 6f76 6965 732e 6964 203d 2072 6f6c 6573  ovies.id = roles
+000025d0: 2e6d 6f76 6965 5f69 640a 290a 4752 4f55  .movie_id.).GROU
+000025e0: 5020 4259 2069 640a 6060 600a 5468 6520  P BY id.```.The 
+000025f0: 7265 7375 6c74 7365 7420 7368 6f75 6c64  resultset should
+00002600: 2062 6520 6c69 6b65 2074 6869 733a 0a21   be like this:.!
+00002610: 5b53 6368 656d 6120 436f 6e66 6972 6d5d  [Schema Confirm]
+00002620: 282e 2f65 7861 6d70 6c65 732f 365f 7363  (./examples/6_sc
+00002630: 6865 6d61 5f63 6f6e 6669 726d 2e70 6e67  hema_confirm.png
+00002640: 290a 2320 6462 7420 4d6f 6465 6c73 200a  ).# dbt Models .
+00002650: 496e 2061 2060 6462 7460 2070 726f 6a65  In a `dbt` proje
+00002660: 6374 2c20 6120 6d6f 6465 6c20 6973 2061  ct, a model is a
+00002670: 2073 716c 2066 696c 6520 6c6f 6361 7465   sql file locate
+00002680: 6420 696e 7369 6465 2060 6d6f 6465 6c73  d inside `models
+00002690: 2f60 2064 6972 6563 746f 7279 2077 6869  /` directory whi
+000026a0: 6368 2077 696c 6c20 636f 6e74 6169 6e20  ch will contain 
+000026b0: 6120 6053 454c 4543 5460 2073 7461 7465  a `SELECT` state
+000026c0: 6d65 6e74 200a 7265 6665 7272 696e 6720  ment .referring 
+000026d0: 746f 2061 2074 7261 6e73 666f 726d 6174  to a transformat
+000026e0: 696f 6e2e 2054 6865 206e 616d 6520 6f66  ion. The name of
+000026f0: 2074 6865 206d 6f64 656c 2066 696c 6520   the model file 
+00002700: 7769 6c6c 2072 6566 6572 2074 6f20 7468  will refer to th
+00002710: 6520 6e61 6d65 206f 6620 6675 7475 7265  e name of future
+00002720: 2074 6162 6c65 2f76 6965 7720 6166 7465   table/view afte
+00002730: 720a 6064 6274 6020 6578 6563 7574 696f  r.`dbt` executio
+00002740: 6e2e 2057 6865 6e20 7765 2065 7865 6375  n. When we execu
+00002750: 7465 2060 6462 7420 7275 6e60 2063 6f6d  te `dbt run` com
+00002760: 6d61 6e64 2c20 6064 6274 6020 7769 6c6c  mand, `dbt` will
+00002770: 2062 7569 6c64 2074 6869 7320 6d6f 6465   build this mode
+00002780: 6c20 6469 7265 6374 6c79 2069 6e74 6f20  l directly into 
+00002790: 4279 7465 486f 7573 6520 6279 2077 7261  ByteHouse by wra
+000027a0: 7070 696e 670a 6974 2069 6e20 6120 6372  pping.it in a cr
+000027b0: 6561 7465 2074 6162 6c65 202f 2076 6965  eate table / vie
+000027c0: 7720 6d61 7465 7269 616c 697a 6174 696f  w materializatio
+000027d0: 6e2e 204d 6174 6572 6961 6c69 7a61 7469  n. Materializati
+000027e0: 6f6e 2074 7970 6520 6f66 2079 6f75 7220  on type of your 
+000027f0: 6d6f 6465 6c20 7769 6c6c 2064 6574 6572  model will deter
+00002800: 6d69 6e65 2074 6865 2061 6374 7561 6c20  mine the actual 
+00002810: 5351 4c0a 7468 6174 2060 6462 7460 2077  SQL.that `dbt` w
+00002820: 696c 6c20 7573 6520 746f 2063 7265 6174  ill use to creat
+00002830: 6520 6d6f 6465 6c20 696e 2074 6865 2077  e model in the w
+00002840: 6172 6568 6f75 7365 2e0a 2320 7363 6865  arehouse..# sche
+00002850: 6d61 2e79 6d6c 0a54 6865 2060 7363 6865  ma.yml.The `sche
+00002860: 6d61 2e79 6d6c 6020 6669 6c65 2077 696c  ma.yml` file wil
+00002870: 6c20 6465 6669 6e65 206f 7572 2074 6162  l define our tab
+00002880: 6c65 7320 2620 636f 6c75 6d6e 7320 6279  les & columns by
+00002890: 2072 6566 6572 7269 6e67 2074 6872 6f75   referring throu
+000028a0: 6768 2061 6c69 6173 206e 616d 652e 2054  gh alias name. T
+000028b0: 6869 7320 7363 6865 6d61 7320 6361 6e20  his schemas can 
+000028c0: 6c61 7465 7220 6265 0a75 7365 6420 696e  later be.used in
+000028d0: 2064 6966 6665 7265 6e74 206d 6f64 656c   different model
+000028e0: 732f 6d61 6372 6f73 2076 6961 2060 736f  s/macros via `so
+000028f0: 7572 6365 2829 6020 6675 6e63 7469 6f6e  urce()` function
+00002900: 2e0a 4372 6561 7465 2060 7363 6865 6d61  ..Create `schema
+00002910: 2e79 6d6c 6020 6669 6c65 2075 6e64 6572  .yml` file under
+00002920: 2060 6d6f 6465 6c73 2f60 2064 6972 6563   `models/` direc
+00002930: 746f 7279 0a60 6060 636f 6d6d 616e 646c  tory.```commandl
+00002940: 696e 650a 746f 7563 6820 6d6f 6465 6c73  ine.touch models
+00002950: 2f73 6368 656d 612e 796d 6c0a 6060 600a  /schema.yml.```.
+00002960: 4465 6669 6e65 206f 7572 206d 6f64 656c  Define our model
+00002970: 2073 6368 656d 6120 6c69 6b65 2074 6869   schema like thi
+00002980: 730a 6060 6079 616d 6c0a 7665 7273 696f  s.```yaml.versio
+00002990: 6e3a 2032 0a0a 736f 7572 6365 733a 0a2d  n: 2..sources:.-
+000029a0: 206e 616d 653a 2069 6d64 620a 2020 7461   name: imdb.  ta
+000029b0: 626c 6573 3a0a 2020 2d20 6e61 6d65 3a20  bles:.  - name: 
+000029c0: 6163 746f 7273 0a20 202d 206e 616d 653a  actors.  - name:
+000029d0: 2072 6f6c 6573 0a20 202d 206e 616d 653a   roles.  - name:
+000029e0: 206d 6f76 6965 730a 6060 600a 2320 4d61   movies.```.# Ma
+000029f0: 7465 7269 616c 697a 6174 696f 6e20 7479  terialization ty
+00002a00: 7065 7320 6f66 204d 6f64 656c 730a 2323  pes of Models.##
+00002a10: 2056 6965 7720 4d61 7465 7269 616c 697a   View Materializ
+00002a20: 6174 696f 6e73 0a49 6e20 6361 7365 206f  ations.In case o
+00002a30: 6620 7669 6577 206d 6174 6572 6961 6c69  f view materiali
+00002a40: 7a61 7469 6f6e 2c20 6120 6d6f 6465 6c20  zation, a model 
+00002a50: 6973 2074 7261 6e73 666f 726d 6564 2074  is transformed t
+00002a60: 6f20 6120 7669 6577 206f 6e20 6561 6368  o a view on each
+00002a70: 2073 696e 676c 6520 7275 6e20 6279 2060   single run by `
+00002a80: 4352 4541 5445 2056 4945 5760 2041 5320  CREATE VIEW` AS 
+00002a90: 7374 6174 656d 656e 7420 696e 200a 4279  statement in .By
+00002aa0: 7465 486f 7573 652e 2056 6965 7720 6d61  teHouse. View ma
+00002ab0: 7465 7269 616c 697a 6174 696f 6e73 2077  terializations w
+00002ac0: 6f6e 2774 2073 746f 7265 2074 6865 2061  on't store the a
+00002ad0: 6374 7561 6c20 6461 7461 2c20 736f 2069  ctual data, so i
+00002ae0: 7420 776f 756c 6420 6265 2073 6c6f 7765  t would be slowe
+00002af0: 7220 746f 2071 7565 7279 2074 6861 6e20  r to query than 
+00002b00: 7461 626c 6520 6d61 7465 7269 616c 697a  table materializ
+00002b10: 6174 696f 6e73 2e0a 4c65 7427 7320 6372  ations..Let's cr
+00002b20: 6561 7465 2060 6d6f 6465 6c73 2f61 6374  eate `models/act
+00002b30: 6f72 5f69 6e73 6967 6874 2e73 716c 6020  or_insight.sql` 
+00002b40: 6173 2076 6965 7720 6d61 7465 7269 616c  as view material
+00002b50: 697a 6174 696f 6e2e 200a 6060 6063 6f6d  ization. .```com
+00002b60: 6d61 6e64 6c69 6e65 0a74 6f75 6368 206d  mandline.touch m
+00002b70: 6f64 656c 732f 6163 746f 7273 5f69 6e73  odels/actors_ins
+00002b80: 6967 6874 2e73 716c 0a60 6060 0a60 6060  ight.sql.```.```
+00002b90: 0a7b 7b20 636f 6e66 6967 286d 6174 6572  .{{ config(mater
+00002ba0: 6961 6c69 7a65 643d 2776 6965 7727 2920  ialized='view') 
+00002bb0: 7d7d 0a0a 5345 4c45 4354 2069 642c 0a20  }}..SELECT id,. 
+00002bc0: 2061 6e79 2861 6374 6f72 5f6e 616d 6529   any(actor_name)
+00002bd0: 2061 7320 6e61 6d65 2c0a 2020 756e 6971   as name,.  uniq
+00002be0: 4578 6163 7428 6d6f 7669 655f 6964 2920  Exact(movie_id) 
+00002bf0: 2020 2061 7320 6e75 6d5f 6d6f 7669 6573     as num_movies
+00002c00: 2c0a 2020 6176 6728 7261 7469 6e67 2920  ,.  avg(rating) 
+00002c10: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00002c20: 7320 6176 675f 7261 7469 6e67 2c0a 2020  s avg_rating,.  
+00002c30: 6d61 7828 6372 6561 7465 645f 6174 2920  max(created_at) 
+00002c40: 6173 2075 7064 6174 6564 5f61 740a 4652  as updated_at.FR
+00002c50: 4f4d 2028 0a20 2053 454c 4543 5420 6163  OM (.  SELECT ac
+00002c60: 746f 7273 2e69 6420 6173 2069 642c 0a20  tors.id as id,. 
+00002c70: 2020 2020 2020 636f 6e63 6174 2861 6374        concat(act
+00002c80: 6f72 732e 6669 7273 745f 6e61 6d65 2c20  ors.first_name, 
+00002c90: 2720 272c 2061 6374 6f72 732e 6c61 7374  ' ', actors.last
+00002ca0: 5f6e 616d 6529 2061 7320 6163 746f 725f  _name) as actor_
+00002cb0: 6e61 6d65 2c0a 2020 2020 2020 206d 6f76  name,.       mov
+00002cc0: 6965 732e 6964 2061 7320 6d6f 7669 655f  ies.id as movie_
+00002cd0: 6964 2c0a 2020 2020 2020 206d 6f76 6965  id,.       movie
+00002ce0: 732e 7261 7469 6e67 2061 7320 7261 7469  s.rating as rati
+00002cf0: 6e67 2c0a 2020 2020 2020 2063 7265 6174  ng,.       creat
+00002d00: 6564 5f61 740a 2020 4652 4f4d 2020 7b7b  ed_at.  FROM  {{
+00002d10: 2073 6f75 7263 6528 2769 6d64 6227 2c20   source('imdb', 
+00002d20: 2761 6374 6f72 7327 2920 7d7d 0a20 2020  'actors') }}.   
+00002d30: 2020 2020 204a 4f49 4e20 7b7b 2073 6f75       JOIN {{ sou
+00002d40: 7263 6528 2769 6d64 6227 2c20 2772 6f6c  rce('imdb', 'rol
+00002d50: 6573 2729 207d 7d20 4f4e 2072 6f6c 6573  es') }} ON roles
+00002d60: 2e61 6374 6f72 5f69 6420 3d20 6163 746f  .actor_id = acto
+00002d70: 7273 2e69 640a 2020 2020 2020 2020 4c45  rs.id.        LE
+00002d80: 4654 204f 5554 4552 204a 4f49 4e20 7b7b  FT OUTER JOIN {{
+00002d90: 2073 6f75 7263 6528 2769 6d64 6227 2c20   source('imdb', 
+00002da0: 276d 6f76 6965 7327 2920 7d7d 204f 4e20  'movies') }} ON 
+00002db0: 6d6f 7669 6573 2e69 6420 3d20 726f 6c65  movies.id = role
+00002dc0: 732e 6d6f 7669 655f 6964 0a29 0a47 524f  s.movie_id.).GRO
+00002dd0: 5550 2042 5920 6964 0a60 6060 0a4c 6574  UP BY id.```.Let
+00002de0: 2773 2065 7865 6375 7465 2060 6462 7420  's execute `dbt 
+00002df0: 7275 6e60 2063 6f6d 6d61 6e64 2074 6f20  run` command to 
+00002e00: 6275 696c 6420 7468 6973 206d 6f64 656c  build this model
+00002e10: 2069 6e20 4279 7465 486f 7573 652e 200a   in ByteHouse. .
+00002e20: 215b 436f 6e66 6972 6d5d 282e 2f65 7861  ![Confirm](./exa
+00002e30: 6d70 6c65 732f 375f 6163 746f 725f 696e  mples/7_actor_in
+00002e40: 7369 6768 745f 636f 6e66 6972 6d2e 706e  sight_confirm.pn
+00002e50: 6729 0a51 7565 7279 696e 6720 7468 6973  g).Querying this
+00002e60: 2076 6965 772c 2077 6520 6361 6e20 7265   view, we can re
+00002e70: 706c 6963 6174 6520 7468 6520 7265 7375  plicate the resu
+00002e80: 6c74 7320 6f66 206f 7572 2065 6172 6c69  lts of our earli
+00002e90: 6572 2071 7565 7279 2077 6974 6820 6120  er query with a 
+00002ea0: 7369 6d70 6c65 7220 7379 6e74 6178 3a0a  simpler syntax:.
+00002eb0: 6060 600a 5345 4c45 4354 202a 2046 524f  ```.SELECT * FRO
+00002ec0: 4d20 696d 6462 2e61 6374 6f72 735f 696e  M imdb.actors_in
+00002ed0: 7369 6768 7420 4f52 4445 5220 4259 206e  sight ORDER BY n
+00002ee0: 756d 5f6d 6f76 6965 7320 4445 5343 3b0a  um_movies DESC;.
+00002ef0: 6060 600a 215b 436f 6e66 6972 6d32 5d28  ```.![Confirm2](
+00002f00: 2e2f 6578 616d 706c 6573 2f38 5f6d 6174  ./examples/8_mat
+00002f10: 6572 6961 6c69 7a65 645f 7669 6577 5f72  erialized_view_r
+00002f20: 756e 5f63 6f6e 6669 726d 2e70 6e67 290a  un_confirm.png).
+00002f30: 2323 2054 6162 6c65 204d 6174 6572 6961  ## Table Materia
+00002f40: 6c69 7a61 7469 6f6e 730a 496e 2063 6173  lizations.In cas
+00002f50: 6520 6f66 2074 6162 6c65 206d 6174 6572  e of table mater
+00002f60: 6961 6c69 7a61 7469 6f6e 2c20 796f 7572  ialization, your
+00002f70: 206d 6f64 656c 2077 6f75 6c64 2062 6520   model would be 
+00002f80: 7265 6275 696c 7420 6173 2061 2074 6162  rebuilt as a tab
+00002f90: 6c65 206f 6e20 6561 6368 2073 696e 676c  le on each singl
+00002fa0: 6520 6064 6274 2072 756e 6020 0a76 6961  e `dbt run` .via
+00002fb0: 2061 2060 4352 4541 5445 2054 4142 4c45   a `CREATE TABLE
+00002fc0: 6020 4153 2073 7461 7465 6d65 6e74 2e20  ` AS statement. 
+00002fd0: 0a60 6060 636f 6d6d 616e 646c 696e 650a  .```commandline.
+00002fe0: 746f 7563 6820 6d6f 6465 6c73 2f61 6374  touch models/act
+00002ff0: 6f72 735f 696e 7369 6768 745f 7461 626c  ors_insight_tabl
+00003000: 652e 7371 6c0a 6060 600a 5765 2063 616e  e.sql.```.We can
+00003010: 2075 7365 206f 7572 2070 7265 7669 6f75   use our previou
+00003020: 7320 7669 6577 206d 6174 6572 6961 6c69  s view materiali
+00003030: 7a61 7469 6f6e 2073 716c 2077 6974 6820  zation sql with 
+00003040: 636f 6e66 6967 2063 6861 6e67 6520 666f  config change fo
+00003050: 7220 7461 626c 6520 6d61 7465 7269 616c  r table material
+00003060: 697a 6174 696f 6e20 7371 6c2e 200a 6060  ization sql. .``
+00003070: 600a 7b7b 2063 6f6e 6669 6728 6f72 6465  `.{{ config(orde
+00003080: 725f 6279 3d27 2875 7064 6174 6564 5f61  r_by='(updated_a
+00003090: 742c 2069 642c 206e 616d 6529 272c 206d  t, id, name)', m
+000030a0: 6174 6572 6961 6c69 7a65 643d 2774 6162  aterialized='tab
+000030b0: 6c65 2729 207d 7d0a 6060 600a 5765 2063  le') }}.```.We c
+000030c0: 616e 2076 6572 6966 7920 7468 6174 2062  an verify that b
+000030d0: 6f74 6820 7669 6577 2026 2074 6162 6c65  oth view & table
+000030e0: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
+000030f0: 7320 6765 6e65 7261 7465 2074 6865 2073  s generate the s
+00003100: 616d 6520 7265 7370 6f6e 7365 2e20 0a60  ame response. .`
+00003110: 6060 0a20 5345 4c45 4354 202a 2046 524f  ``. SELECT * FRO
+00003120: 4d20 696d 6462 2e61 6374 6f72 735f 696e  M imdb.actors_in
+00003130: 7369 6768 745f 7461 626c 6520 4f52 4445  sight_table ORDE
+00003140: 5220 4259 206e 756d 5f6d 6f76 6965 7320  R BY num_movies 
+00003150: 4445 5343 3b0a 6060 600a 2323 2049 6e63  DESC;.```.## Inc
+00003160: 7265 6d65 6e74 616c 204d 6174 6572 6961  remental Materia
+00003170: 6c69 7a61 7469 6f6e 730a 466f 7220 6f75  lizations.For ou
+00003180: 7220 7072 6576 696f 7573 2074 6162 6c65  r previous table
+00003190: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
+000031a0: 2c20 6064 6274 6020 7769 6c6c 2063 6f6e  , `dbt` will con
+000031b0: 7374 7275 6374 2061 2074 6162 6c65 2065  struct a table e
+000031c0: 7665 7279 2074 696d 6520 746f 206d 6174  very time to mat
+000031d0: 6572 6961 6c69 7a65 2074 6865 206d 6f64  erialize the mod
+000031e0: 656c 2e20 466f 7220 6c61 7267 6572 0a6f  el. For larger.o
+000031f0: 7220 636f 6d70 6c65 7820 7472 616e 7366  r complex transf
+00003200: 6f72 6d61 7469 6f6e 732c 2074 6869 7320  ormations, this 
+00003210: 776f 756c 6420 6265 2072 6564 756e 6461  would be redunda
+00003220: 6e74 2061 6e64 2063 6f73 746c 7920 696e  nt and costly in
+00003230: 2074 6572 6d73 206f 6620 636f 6d70 7574   terms of comput
+00003240: 696e 6720 706f 7765 722e 2049 6e63 7265  ing power. Incre
+00003250: 6d65 6e74 616c 200a 6d61 7465 7269 616c  mental .material
+00003260: 697a 6174 696f 6e73 2073 6f6c 7665 2074  izations solve t
+00003270: 6869 7320 7072 6f62 6c65 6d2e 3c62 722f  his problem.<br/
+00003280: 3e0a 5468 6520 6669 7273 7420 7469 6d65  >.The first time
+00003290: 2061 206d 6f64 656c 2069 7320 7275 6e2c   a model is run,
+000032a0: 2074 6865 2074 6162 6c65 2069 7320 6275   the table is bu
+000032b0: 696c 7420 6279 2074 7261 6e73 666f 726d  ilt by transform
+000032c0: 696e 6720 616c 6c20 726f 7773 206f 6620  ing all rows of 
+000032d0: 736f 7572 6365 2064 6174 612e 204f 6e20  source data. On 
+000032e0: 7375 6273 6571 7565 6e74 2072 756e 732c  subsequent runs,
+000032f0: 200a 6064 6274 6020 7472 616e 7366 6f72   .`dbt` transfor
+00003300: 6d73 206f 6e6c 7920 7468 6520 726f 7773  ms only the rows
+00003310: 2069 6e20 796f 7572 2073 6f75 7263 6520   in your source 
+00003320: 6461 7461 2074 6861 7420 796f 7520 7465  data that you te
+00003330: 6c6c 2060 6462 7460 2074 6f20 6669 6c74  ll `dbt` to filt
+00003340: 6572 2066 6f72 2c20 696e 7365 7274 696e  er for, insertin
+00003350: 6720 7468 656d 2069 6e74 6f20 7468 6520  g them into the 
+00003360: 7461 7267 6574 200a 7461 626c 6520 7768  target .table wh
+00003370: 6963 6820 6973 2074 6865 2074 6162 6c65  ich is the table
+00003380: 2074 6861 7420 6861 7320 616c 7265 6164   that has alread
+00003390: 7920 6265 656e 2062 7569 6c74 2e3c 6272  y been built.<br
+000033a0: 2f3e 0a54 6f20 7465 6c6c 2060 6462 7460  />.To tell `dbt`
+000033b0: 2077 6869 6368 2072 6f77 7320 6974 2073   which rows it s
+000033c0: 686f 756c 6420 7472 616e 7366 6f72 6d20  hould transform 
+000033d0: 6f6e 2061 6e20 696e 6372 656d 656e 7461  on an incrementa
+000033e0: 6c20 7275 6e2c 2077 7261 7020 7661 6c69  l run, wrap vali
+000033f0: 6420 5351 4c20 7468 6174 2066 696c 7465  d SQL that filte
+00003400: 7273 2066 6f72 2074 6865 7365 2072 6f77  rs for these row
+00003410: 7320 0a69 6e20 7468 6520 6069 735f 696e  s .in the `is_in
+00003420: 6372 656d 656e 7461 6c28 2960 206d 6163  cremental()` mac
+00003430: 726f 2e20 596f 7572 2060 6973 5f69 6e63  ro. Your `is_inc
+00003440: 7265 6d65 6e74 616c 2829 6020 636f 6465  remental()` code
+00003450: 2077 696c 6c20 6368 6563 6b20 666f 7220   will check for 
+00003460: 726f 7773 2063 7265 6174 6564 206f 7220  rows created or 
+00003470: 6d6f 6469 6669 6564 2073 696e 6365 2074  modified since t
+00003480: 6865 200a 6c61 7374 2074 696d 6520 6064  he .last time `d
+00003490: 6274 6020 7261 6e20 7468 6973 206d 6f64  bt` ran this mod
+000034a0: 656c 2e0a 6060 6063 6f6d 6d61 6e64 6c69  el..```commandli
+000034b0: 6e65 0a74 6f75 6368 206d 6f64 656c 732f  ne.touch models/
+000034c0: 6163 746f 7273 5f69 6e73 6967 6874 5f69  actors_insight_i
+000034d0: 6e63 7265 6d65 6e74 616c 2e73 716c 0a60  ncremental.sql.`
+000034e0: 6060 0a60 6060 0a7b 7b20 636f 6e66 6967  ``.```.{{ config
+000034f0: 286f 7264 6572 5f62 793d 2728 7570 6461  (order_by='(upda
+00003500: 7465 645f 6174 2c20 6964 2c20 6e61 6d65  ted_at, id, name
+00003510: 2927 2c20 6d61 7465 7269 616c 697a 6564  )', materialized
+00003520: 3d27 696e 6372 656d 656e 7461 6c27 2920  ='incremental') 
+00003530: 7d7d 0a0a 5345 4c45 4354 2069 642c 0a20  }}..SELECT id,. 
+00003540: 2061 6e79 2861 6374 6f72 5f6e 616d 6529   any(actor_name)
+00003550: 2061 7320 6e61 6d65 2c0a 2020 756e 6971   as name,.  uniq
+00003560: 4578 6163 7428 6d6f 7669 655f 6964 2920  Exact(movie_id) 
+00003570: 2020 2061 7320 6e75 6d5f 6d6f 7669 6573     as num_movies
+00003580: 2c0a 2020 6176 6728 7261 7469 6e67 2920  ,.  avg(rating) 
+00003590: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000035a0: 7320 6176 675f 7261 7469 6e67 2c0a 2020  s avg_rating,.  
+000035b0: 6d61 7828 6372 6561 7465 645f 6174 2920  max(created_at) 
+000035c0: 6173 2075 7064 6174 6564 5f61 740a 4652  as updated_at.FR
+000035d0: 4f4d 2028 0a20 2053 454c 4543 5420 6163  OM (.  SELECT ac
+000035e0: 746f 7273 2e69 6420 6173 2069 642c 0a20  tors.id as id,. 
+000035f0: 2020 2020 2020 636f 6e63 6174 2861 6374        concat(act
+00003600: 6f72 732e 6669 7273 745f 6e61 6d65 2c20  ors.first_name, 
+00003610: 2720 272c 2061 6374 6f72 732e 6c61 7374  ' ', actors.last
+00003620: 5f6e 616d 6529 2061 7320 6163 746f 725f  _name) as actor_
+00003630: 6e61 6d65 2c0a 2020 2020 2020 206d 6f76  name,.       mov
+00003640: 6965 732e 6964 2061 7320 6d6f 7669 655f  ies.id as movie_
+00003650: 6964 2c0a 2020 2020 2020 206d 6f76 6965  id,.       movie
+00003660: 732e 7261 7469 6e67 2061 7320 7261 7469  s.rating as rati
+00003670: 6e67 2c0a 2020 2020 2020 2063 7265 6174  ng,.       creat
+00003680: 6564 5f61 740a 2020 4652 4f4d 2020 7b7b  ed_at.  FROM  {{
+00003690: 2073 6f75 7263 6528 2769 6d64 6227 2c20   source('imdb', 
+000036a0: 2761 6374 6f72 7327 2920 7d7d 0a20 2020  'actors') }}.   
+000036b0: 2020 2020 204a 4f49 4e20 7b7b 2073 6f75       JOIN {{ sou
+000036c0: 7263 6528 2769 6d64 6227 2c20 2772 6f6c  rce('imdb', 'rol
+000036d0: 6573 2729 207d 7d20 4f4e 2072 6f6c 6573  es') }} ON roles
+000036e0: 2e61 6374 6f72 5f69 6420 3d20 6163 746f  .actor_id = acto
+000036f0: 7273 2e69 640a 2020 2020 2020 2020 4c45  rs.id.        LE
+00003700: 4654 204f 5554 4552 204a 4f49 4e20 7b7b  FT OUTER JOIN {{
+00003710: 2073 6f75 7263 6528 2769 6d64 6227 2c20   source('imdb', 
+00003720: 276d 6f76 6965 7327 2920 7d7d 204f 4e20  'movies') }} ON 
+00003730: 6d6f 7669 6573 2e69 6420 3d20 726f 6c65  movies.id = role
+00003740: 732e 6d6f 7669 655f 6964 0a29 0a47 524f  s.movie_id.).GRO
+00003750: 5550 2042 5920 6964 0a0a 7b25 2069 6620  UP BY id..{% if 
+00003760: 6973 5f69 6e63 7265 6d65 6e74 616c 2829  is_incremental()
+00003770: 2025 7d0a 0a2d 2d20 7468 6973 2066 696c   %}..-- this fil
+00003780: 7465 7220 7769 6c6c 206f 6e6c 7920 6265  ter will only be
+00003790: 2061 7070 6c69 6564 206f 6e20 616e 2069   applied on an i
+000037a0: 6e63 7265 6d65 6e74 616c 2072 756e 0a77  ncremental run.w
+000037b0: 6865 7265 2069 6420 3e20 2873 656c 6563  here id > (selec
+000037c0: 7420 6d61 7828 6964 2920 6672 6f6d 207b  t max(id) from {
+000037d0: 7b20 7468 6973 207d 7d29 206f 7220 7570  { this }}) or up
+000037e0: 6461 7465 645f 6174 203e 2028 7365 6c65  dated_at > (sele
+000037f0: 6374 206d 6178 2875 7064 6174 6564 5f61  ct max(updated_a
+00003800: 7429 2066 726f 6d20 7b7b 7468 6973 7d7d  t) from {{this}}
+00003810: 290a 0a7b 2520 656e 6469 6620 257d 0a60  )..{% endif %}.`
+00003820: 6060 0a57 6520 6361 6e20 7665 7269 6679  ``.We can verify
+00003830: 2074 6861 7420 7669 6577 2c20 7461 626c   that view, tabl
+00003840: 6520 2620 696e 6372 656d 656e 7461 6c20  e & incremental 
+00003850: 6d61 7465 7269 616c 697a 6174 696f 6e73  materializations
+00003860: 2c20 616c 6c20 6765 6e65 7261 7465 2074  , all generate t
+00003870: 6865 2073 616d 6520 7265 7370 6f6e 7365  he same response
+00003880: 2e20 0a60 6060 0a20 5345 4c45 4354 202a  . .```. SELECT *
+00003890: 2046 524f 4d20 696d 6462 2e61 6374 6f72   FROM imdb.actor
+000038a0: 735f 696e 7369 6768 745f 7461 626c 6520  s_insight_table 
+000038b0: 4f52 4445 5220 4259 206e 756d 5f6d 6f76  ORDER BY num_mov
+000038c0: 6965 7320 4445 5343 3b0a 6060 600a 6060  ies DESC;.```.``
+000038d0: 6063 6f6d 6d61 6e64 6c69 6e65 0a64 6274  `commandline.dbt
+000038e0: 2072 756e 202d 6d20 6d6f 6465 6c73 2f61   run -m models/a
+000038f0: 6374 6f72 735f 696e 7369 6768 745f 696e  ctors_insight_in
+00003900: 6372 656d 656e 7461 6c2e 7371 6c0a 6060  cremental.sql.``
+00003910: 600a 4c65 7427 7320 696e 7365 7274 2061  `.Let's insert a
+00003920: 2066 6577 206d 6f72 6520 726f 7773 2074   few more rows t
+00003930: 6f20 6465 6d6f 6e73 7472 6174 6520 7468  o demonstrate th
+00003940: 6520 706f 7765 7220 6f66 2069 6e63 7265  e power of incre
+00003950: 6d65 6e74 616c 206d 6174 6572 6961 6c69  mental materiali
+00003960: 7a61 7469 6f6e 732e 204e 6f77 2074 6865  zations. Now the
+00003970: 206d 6f73 7420 0a61 7070 6561 7265 6420   most .appeared 
+00003980: 6163 746f 7220 7368 6f75 6c64 2062 6520  actor should be 
+00003990: 2743 6872 6973 2050 7261 7474 272e 200a  'Chris Pratt'. .
+000039a0: 6060 600a 494e 5345 5254 2049 4e54 4f20  ```.INSERT INTO 
+000039b0: 696d 6462 2e6d 6f76 6965 7320 5641 4c55  imdb.movies VALU
+000039c0: 4553 2028 392c 2027 5061 7373 656e 6765  ES (9, 'Passenge
+000039d0: 7273 272c 2032 3031 362c 2037 293b 0a49  rs', 2016, 7);.I
+000039e0: 4e53 4552 5420 494e 544f 2069 6d64 622e  NSERT INTO imdb.
+000039f0: 6d6f 7669 6573 2056 414c 5545 5320 2831  movies VALUES (1
+00003a00: 302c 2027 5468 6520 546f 6d6f 7272 6f77  0, 'The Tomorrow
+00003a10: 2057 6172 272c 2032 3032 312c 2036 2e35   War', 2021, 6.5
+00003a20: 293b 0a0a 494e 5345 5254 2049 4e54 4f20  );..INSERT INTO 
+00003a30: 696d 6462 2e72 6f6c 6573 2028 6163 746f  imdb.roles (acto
+00003a40: 725f 6964 2c20 6d6f 7669 655f 6964 2c20  r_id, movie_id, 
+00003a50: 726f 6c65 5f6e 616d 6529 2056 414c 5545  role_name) VALUE
+00003a60: 5328 342c 2039 2c20 274a 696d 2050 7265  S(4, 9, 'Jim Pre
+00003a70: 7374 6f6e 2729 3b0a 494e 5345 5254 2049  ston');.INSERT I
+00003a80: 4e54 4f20 696d 6462 2e72 6f6c 6573 2028  NTO imdb.roles (
+00003a90: 6163 746f 725f 6964 2c20 6d6f 7669 655f  actor_id, movie_
+00003aa0: 6964 2c20 726f 6c65 5f6e 616d 6529 2056  id, role_name) V
+00003ab0: 414c 5545 5328 342c 2031 302c 2027 4461  ALUES(4, 10, 'Da
+00003ac0: 6e20 466f 7265 7374 6572 2729 3b0a 6060  n Forester');.``
+00003ad0: 600a 6060 6063 6f6d 6d61 6e64 6c69 6e65  `.```commandline
+00003ae0: 0a64 6274 2072 756e 202d 6d20 6d6f 6465  .dbt run -m mode
+00003af0: 6c73 2f61 6374 6f72 735f 696e 7369 6768  ls/actors_insigh
+00003b00: 745f 696e 6372 656d 656e 7461 6c2e 7371  t_incremental.sq
+00003b10: 6c0a 6060 600a 6060 600a 5345 4c45 4354  l.```.```.SELECT
+00003b20: 202a 2046 524f 4d20 696d 6462 2e61 6374   * FROM imdb.act
+00003b30: 6f72 735f 696e 7369 6768 745f 696e 6372  ors_insight_incr
+00003b40: 656d 656e 7461 6c20 4f52 4445 5220 4259  emental ORDER BY
+00003b50: 206e 756d 5f6d 6f76 6965 7320 4445 5343   num_movies DESC
+00003b60: 3b0a 6060 600a 215b 436f 6e66 6972 6d33  ;.```.![Confirm3
+00003b70: 5d28 2e2f 6578 616d 706c 6573 2f39 5f69  ](./examples/9_i
+00003b80: 6e63 7265 6d65 6e74 616c 5f63 6f6e 6669  ncremental_confi
+00003b90: 726d 2e70 6e67 290a 2323 2320 486f 7720  rm.png).### How 
+00003ba0: 6974 2077 6f72 6b73 0a31 2e20 6064 6274  it works.1. `dbt
+00003bb0: 6020 7769 6c6c 2066 6972 7374 2063 7265  ` will first cre
+00003bc0: 6174 6520 6120 7465 6d70 6f72 6172 7920  ate a temporary 
+00003bd0: 7461 626c 6520 6e61 6d65 6420 6061 6374  table named `act
+00003be0: 6f72 735f 696e 7369 6768 745f 696e 6372  ors_insight_incr
+00003bf0: 656d 656e 7461 6c5f 746d 7060 2026 2069  emental_tmp` & i
+00003c00: 6e73 6572 7420 616c 6c20 7468 6f73 6520  nsert all those 
+00003c10: 726f 7773 2077 6869 6368 200a 7061 7373  rows which .pass
+00003c20: 206f 7572 2060 6973 5f69 6e63 7265 6d65   our `is_increme
+00003c30: 6e74 616c 2829 6020 6669 6c74 6572 2e0a  ntal()` filter..
+00003c40: 322e 2041 206e 6577 2074 6162 6c65 2060  2. A new table `
+00003c50: 6163 746f 7273 5f69 6e73 6967 6874 5f69  actors_insight_i
+00003c60: 6e63 7265 6d65 6e74 616c 5f6e 6577 6020  ncremental_new` 
+00003c70: 7769 6c6c 2062 6520 6372 6561 7465 6420  will be created 
+00003c80: 2620 726f 7773 2066 726f 6d20 7468 6520  & rows from the 
+00003c90: 6f6c 6420 7461 626c 6520 6061 6374 6f72  old table `actor
+00003ca0: 735f 696e 7369 6768 745f 696e 6372 656d  s_insight_increm
+00003cb0: 656e 7461 6c60 200a 7769 6c6c 2062 6520  ental` .will be 
+00003cc0: 696e 6765 7374 6564 2068 6572 652e 2060  ingested here. `
+00003cd0: 6462 7460 2077 696c 6c20 6d61 6b65 2073  dbt` will make s
+00003ce0: 7572 6520 7468 6174 2060 756e 6971 7565  ure that `unique
+00003cf0: 5f6b 6579 6020 2869 6620 616e 7920 6465  _key` (if any de
+00003d00: 636c 6172 6564 2069 6e20 636f 6e66 6967  clared in config
+00003d10: 2920 636f 6e73 7472 6169 6e74 2069 7320  ) constraint is 
+00003d20: 6d61 696e 7461 696e 6564 2c20 0a62 7920  maintained, .by 
+00003d30: 6e6f 7420 616c 6c6f 7769 6e67 2074 686f  not allowing tho
+00003d40: 7365 2072 6f77 7320 7768 6963 6820 6861  se rows which ha
+00003d50: 7665 2074 6865 2073 616d 6520 6075 6e69  ve the same `uni
+00003d60: 7175 655f 6b65 7960 2061 7320 7468 6520  que_key` as the 
+00003d70: 7072 6576 696f 7573 2074 656d 706f 7261  previous tempora
+00003d80: 7279 2074 6162 6c65 2e20 0a33 2e20 5468  ry table. .3. Th
+00003d90: 6520 726f 7773 2066 726f 6d20 7468 6520  e rows from the 
+00003da0: 7465 6d70 6f72 6172 7920 7461 626c 6520  temporary table 
+00003db0: 776f 756c 6420 6265 2069 6e67 6573 7465  would be ingeste
+00003dc0: 6420 696e 746f 2074 6865 206e 6577 2074  d into the new t
+00003dd0: 6162 6c65 2e0a 342e 204f 7572 2070 7265  able..4. Our pre
+00003de0: 7669 6f75 7320 7461 626c 6520 2860 6163  vious table (`ac
+00003df0: 746f 7273 5f69 6e73 6967 6874 5f69 6e63  tors_insight_inc
+00003e00: 7265 6d65 6e74 616c 6029 2026 206e 6577  remental`) & new
+00003e10: 2074 6162 6c65 2028 6061 6374 6f72 735f   table (`actors_
+00003e20: 696e 7369 6768 745f 6e65 7760 2920 7769  insight_new`) wi
+00003e30: 6c6c 2062 6520 6578 6368 616e 6765 642e  ll be exchanged.
+00003e40: 200a 0a23 2044 6972 6563 7420 5772 6974   ..# Direct Writ
+00003e50: 6520 746f 2043 4e43 4820 556e 6971 7565  e to CNCH Unique
+00003e60: 204b 6579 2054 6162 6c65 0a23 2320 5265   Key Table.## Re
+00003e70: 7175 6972 656d 656e 740a 312e 2060 6462  quirement.1. `db
+00003e80: 742d 6279 7465 686f 7573 6560 2063 6f6e  t-bytehouse` con
+00003e90: 6e65 6374 6f72 2076 6572 7369 6f6e 2074  nector version t
+00003ea0: 6f20 6265 2061 7420 6c65 6173 7420 6031  o be at least `1
+00003eb0: 2e37 2e31 602e 200a 322e 204e 6565 6473  .7.1`. .2. Needs
+00003ec0: 2074 6f20 7365 7420 636f 6e66 6967 206e   to set config n
+00003ed0: 616d 6520 6063 6e63 685f 756e 6971 7565  ame `cnch_unique
+00003ee0: 5f6b 6579 6020 696e 7374 6561 6420 6f66  _key` instead of
+00003ef0: 2060 756e 6971 7565 5f6b 6579 600a 332e   `unique_key`.3.
+00003f00: 204e 6565 6473 2074 6f20 7365 7420 636f   Needs to set co
+00003f10: 6e66 6967 2060 696e 6372 656d 656e 7461  nfig `incrementa
+00003f20: 6c5f 7374 7261 7465 6779 6020 6173 2060  l_strategy` as `
+00003f30: 6170 7065 6e64 600a 342e 2057 7269 7465  append`.4. Write
+00003f40: 2061 2053 514c 2065 7870 7265 7373 696f   a SQL expressio
+00003f50: 6e20 746f 2061 7070 656e 6420 7468 6520  n to append the 
+00003f60: 7669 7274 7561 6c20 7761 7265 686f 7573  virtual warehous
+00003f70: 6520 6964 2061 7420 7468 6520 656e 6420  e id at the end 
+00003f80: 6f66 2044 4254 206d 6f64 656c 2c20 6578  of DBT model, ex
+00003f90: 616d 706c 650a 6053 4554 5449 4e47 5320  ample.`SETTINGS 
+00003fa0: 7669 7274 7561 6c5f 7761 7265 686f 7573  virtual_warehous
+00003fb0: 653d 2776 772d 6964 272c 2076 6972 7475  e='vw-id', virtu
+00003fc0: 616c 5f77 6172 6568 6f75 7365 5f77 7269  al_warehouse_wri
+00003fd0: 7465 3d27 7677 2d69 6427 600a 2323 2045  te='vw-id'`.## E
+00003fe0: 7861 6d70 6c65 0a60 6060 0a7b 7b0a 2020  xample.```.{{.  
+00003ff0: 2020 636f 6e66 6967 280a 2020 2020 2020    config(.      
+00004000: 2020 6d61 7465 7269 616c 697a 6564 3d27    materialized='
+00004010: 696e 6372 656d 656e 7461 6c27 2c0a 2020  incremental',.  
+00004020: 2020 2020 2020 636e 6368 5f75 6e69 7175        cnch_uniqu
+00004030: 655f 6b65 793d 2769 6427 2c0a 2020 2020  e_key='id',.    
+00004040: 2020 2020 696e 6372 656d 656e 7461 6c5f      incremental_
+00004050: 7374 7261 7465 6779 3d27 6170 7065 6e64  strategy='append
+00004060: 2720 2020 200a 2020 2020 290a 7d7d 0a0a  '    .    ).}}..
+00004070: 5345 4c45 4354 0a20 2020 2069 642c 0a20  SELECT.    id,. 
+00004080: 2020 2074 7261 6e73 6163 7469 6f6e 5f64     transaction_d
+00004090: 6174 652c 0a20 2020 2075 7365 725f 6964  ate,.    user_id
+000040a0: 2c0a 2020 2020 616d 6f75 6e74 2c0a 2020  ,.    amount,.  
+000040b0: 2020 7374 6174 7573 0a46 524f 4d20 0a20    status.FROM . 
+000040c0: 2020 2064 6274 5f75 6e69 7175 652e 7472     dbt_unique.tr
+000040d0: 616e 7361 6374 696f 6e73 200a 0a7b 2520  ansactions ..{% 
+000040e0: 6966 2069 735f 696e 6372 656d 656e 7461  if is_incrementa
+000040f0: 6c28 2920 257d 0a0a 2020 5748 4552 4520  l() %}..  WHERE 
+00004100: 7472 616e 7361 6374 696f 6e5f 6461 7465  transaction_date
+00004110: 203e 3d20 2853 454c 4543 5420 6d61 7828   >= (SELECT max(
+00004120: 7472 616e 7361 6374 696f 6e5f 6461 7465  transaction_date
+00004130: 2920 4652 4f4d 2064 6274 5f75 6e69 7175  ) FROM dbt_uniqu
+00004140: 652e 7472 616e 7361 6374 696f 6e73 290a  e.transactions).
+00004150: 0a7b 2520 656e 6469 6620 257d 0a0a 5345  .{% endif %}..SE
+00004160: 5454 494e 4753 2076 6972 7475 616c 5f77  TTINGS virtual_w
+00004170: 6172 6568 6f75 7365 3d27 7677 2d69 6427  arehouse='vw-id'
+00004180: 2c20 7669 7274 7561 6c5f 7761 7265 686f  , virtual_wareho
+00004190: 7573 655f 7772 6974 653d 2776 772d 6964  use_write='vw-id
+000041a0: 270a 6060 600a 2320 5072 6f6a 6563 7420  '.```.# Project 
+000041b0: 446f 6375 6d65 6e74 6174 696f 6e0a 6064  Documentation.`d
+000041c0: 6274 6020 7072 6f76 6964 6573 2061 2077  bt` provides a w
+000041d0: 6179 2074 6f20 6765 6e65 7261 7465 2064  ay to generate d
+000041e0: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
+000041f0: 2079 6f75 7220 6462 7420 7072 6f6a 6563   your dbt projec
+00004200: 7420 616e 6420 7265 6e64 6572 2069 7420  t and render it 
+00004210: 6173 2061 2077 6562 7369 7465 2e20 0a43  as a website. .C
+00004220: 7265 6174 6520 606d 6f64 656c 732f 6163  reate `models/ac
+00004230: 746f 7273 5f69 6e73 6967 6874 5f69 6e63  tors_insight_inc
+00004240: 7265 6d65 6e74 616c 2e79 6d6c 6020 746f  remental.yml` to
+00004250: 2067 656e 6572 6174 6520 646f 6375 6d65   generate docume
+00004260: 6e74 6174 696f 6e20 666f 7220 6f75 7220  ntation for our 
+00004270: 6d6f 6465 6c73 2e20 0a60 6060 7961 6d6c  models. .```yaml
+00004280: 0a76 6572 7369 6f6e 3a20 320a 0a6d 6f64  .version: 2..mod
+00004290: 656c 733a 0a20 202d 206e 616d 653a 2061  els:.  - name: a
+000042a0: 6374 6f72 735f 696e 7369 6768 745f 696e  ctors_insight_in
+000042b0: 6372 656d 656e 7461 6c0a 2020 2020 6465  cremental.    de
+000042c0: 7363 7269 7074 696f 6e3a 2041 6374 6f72  scription: Actor
+000042d0: 2061 7070 6561 7261 6e63 6520 7375 6d6d   appearance summ
+000042e0: 6172 7920 6261 7365 6420 6f6e 2072 6f6c  ary based on rol
+000042f0: 6573 0a20 2020 2063 6f6c 756d 6e73 3a20  es.    columns: 
+00004300: 0a20 2020 2020 202d 206e 616d 653a 2069  .      - name: i
+00004310: 640a 2020 2020 2020 2020 6465 7363 7269  d.        descri
+00004320: 7074 696f 6e3a 2054 6865 2069 6420 6e75  ption: The id nu
+00004330: 6d62 6572 206f 6620 6163 746f 720a 2020  mber of actor.  
+00004340: 2020 2020 2d20 6e61 6d65 3a20 6e61 6d65      - name: name
+00004350: 0a20 2020 2020 2020 2064 6573 6372 6970  .        descrip
+00004360: 7469 6f6e 3a20 5468 6520 6e61 6d65 206f  tion: The name o
+00004370: 6620 6163 746f 720a 2020 2020 2020 2d20  f actor.      - 
+00004380: 6e61 6d65 3a20 6e75 6d5f 6d6f 7669 6573  name: num_movies
+00004390: 0a20 2020 2020 2020 2064 6573 6372 6970  .        descrip
+000043a0: 7469 6f6e 3a20 5468 6520 6e75 6d62 6572  tion: The number
+000043b0: 206f 6620 6d6f 7669 6573 2061 6374 6f72   of movies actor
+000043c0: 2068 6173 2061 7070 6561 7265 6420 0a20   has appeared . 
+000043d0: 2020 2020 202d 206e 616d 653a 2061 7667       - name: avg
+000043e0: 5f72 6174 696e 670a 2020 2020 2020 2020  _rating.        
+000043f0: 6465 7363 7269 7074 696f 6e3a 2041 7665  description: Ave
+00004400: 7261 6765 2072 6174 696e 670a 2020 2020  rage rating.    
+00004410: 2020 2d20 6e61 6d65 3a20 7570 6461 7465    - name: update
+00004420: 645f 6174 0a20 2020 2020 2020 2064 6573  d_at.        des
+00004430: 6372 6970 7469 6f6e 3a20 4c61 7465 7374  cription: Latest
+00004440: 2075 7064 6174 6520 7469 6d65 0a60 6060   update time.```
+00004450: 0a55 7365 2060 6462 7420 646f 6373 2067  .Use `dbt docs g
+00004460: 656e 6572 6174 6560 2074 6f20 6765 6e65  enerate` to gene
+00004470: 7261 7465 2074 6865 2064 6f63 756d 656e  rate the documen
+00004480: 7461 7469 6f6e 2066 6f72 2079 6f75 7220  tation for your 
+00004490: 6d6f 6465 6c73 2026 2060 6462 7420 646f  models & `dbt do
+000044a0: 6373 2073 6572 7665 6020 746f 2073 6572  cs serve` to ser
+000044b0: 7665 2074 6865 2064 6f63 756d 656e 7461  ve the documenta
+000044c0: 7469 6f6e 2069 6e20 0a79 6f75 7220 6c6f  tion in .your lo
+000044d0: 6361 6c20 6272 6f77 7365 7220 6f6e 2070  cal browser on p
+000044e0: 6f72 7420 3830 3030 2e0a 215b 446f 635d  ort 8000..![Doc]
+000044f0: 282e 2f65 7861 6d70 6c65 732f 3130 5f64  (./examples/10_d
+00004500: 6f63 732e 706e 6729 0a23 204c 6f63 616c  ocs.png).# Local
+00004510: 2044 6576 656c 6f70 6d65 6e74 0a55 7064   Development.Upd
+00004520: 6174 6520 6074 6573 7473 2f69 6e74 6567  ate `tests/integ
+00004530: 7261 7469 6f6e 2f63 6f6e 6665 7374 2e70  ration/confest.p
+00004540: 7960 2066 696c 6520 746f 2069 6e63 6c75  y` file to inclu
+00004550: 6465 2079 6f75 7220 636f 6e6e 6563 7469  de your connecti
+00004560: 6f6e 2063 7265 6465 6e74 6961 6c73 2e20  on credentials. 
+00004570: 466f 7220 7275 6e6e 696e 6720 7465 7374  For running test
+00004580: 7320 6c6f 6361 6c6c 792c 2066 6f6c 6c6f  s locally, follo
+00004590: 7720 0a74 6865 7365 2073 7465 7073 3a0a  w .these steps:.
+000045a0: 6060 6063 6f6d 6d61 6e64 6c69 6e65 0a70  ```commandline.p
+000045b0: 6970 2069 6e73 7461 6c6c 202d 7220 6465  ip install -r de
+000045c0: 765f 7265 7175 6972 656d 656e 7473 2e74  v_requirements.t
+000045d0: 7874 0a70 7974 686f 6e20 2d6d 2070 7974  xt.python -m pyt
+000045e0: 6573 740a 6060 600a 2320 4f72 6967 696e  est.```.# Origin
+000045f0: 616c 2041 7574 686f 720a 4279 7465 486f  al Author.ByteHo
+00004600: 7573 6520 7761 6e74 7320 746f 2074 6861  use wants to tha
+00004610: 6e6b 2043 6c69 636b 486f 7573 6520 666f  nk ClickHouse fo
+00004620: 7220 6f72 6967 696e 616c 2063 6f6e 7472  r original contr
+00004630: 6962 7574 696f 6e20 746f 2074 6869 7320  ibution to this 
+00004640: 636f 6e6e 6563 746f 722e 0a0a 2320 4c69  connector...# Li
+00004650: 6365 6e73 650a 5468 6973 2070 726f 6a65  cense.This proje
+00004660: 6374 2069 7320 6469 7374 7269 6275 7465  ct is distribute
+00004670: 6420 756e 6465 7220 7468 6520 7465 726d  d under the term
+00004680: 7320 6f66 2074 6865 2041 7061 6368 6520  s of the Apache 
+00004690: 4c69 6365 6e73 6520 2856 6572 7369 6f6e  License (Version
+000046a0: 2032 2e30 292e                            2.0).
```

### Comparing `dbt-bytehouse-1.7.1/README.md` & `dbt-bytehouse-1.7.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,1219 +1,1195 @@
-00000000: 2320 496e 7472 6f64 7563 7469 6f6e 0a60  # Introduction.`
-00000010: 6462 7460 2028 4461 7461 2042 7569 6c64  dbt` (Data Build
-00000020: 696e 6720 546f 6f6c 2920 6973 2061 6e20  ing Tool) is an 
-00000030: 6f70 656e 2073 6f75 7263 6520 746f 6f6c  open source tool
-00000040: 2074 6861 7420 656e 6162 6c65 7320 6461   that enables da
-00000050: 7461 2061 6e61 6c79 7374 7320 616e 6420  ta analysts and 
-00000060: 656e 6769 6e65 6572 7320 746f 2074 7261  engineers to tra
-00000070: 6e73 666f 726d 0a64 6174 6120 696e 2074  nsform.data in t
-00000080: 6865 6972 2077 6172 6568 6f75 7365 7320  heir warehouses 
-00000090: 7369 6d70 6c79 2062 7920 7772 6974 696e  simply by writin
-000000a0: 6720 7365 6c65 6374 2073 7461 7465 6d65  g select stateme
-000000b0: 6e74 732e 2060 6462 7460 2070 6572 666f  nts. `dbt` perfo
-000000c0: 726d 7320 7468 6520 5420 2854 7261 6e73  rms the T (Trans
-000000d0: 666f 726d 2920 6f66 2045 544c 2061 6e64  form) of ETL and
-000000e0: 0a61 6c6c 6f77 7320 636f 6d70 616e 6965  .allows companie
-000000f0: 7320 746f 2077 7269 7465 2074 7261 6e73  s to write trans
-00000100: 666f 726d 6174 696f 6e73 2061 7320 7175  formations as qu
-00000110: 6572 6965 7320 616e 6420 6f72 6368 6573  eries and orches
-00000120: 7472 6174 6520 7468 656d 2069 6e20 6120  trate them in a 
-00000130: 6d6f 7265 2065 6666 6963 6965 6e74 2077  more efficient w
-00000140: 6179 2e20 0a42 7974 6548 6f75 7365 2064  ay. .ByteHouse d
-00000150: 6274 2063 6f6e 6e65 6374 6f72 2069 7320  bt connector is 
-00000160: 6120 706c 7567 696e 2065 6e61 626c 696e  a plugin enablin
-00000170: 6720 7573 6572 7320 746f 2062 7569 6c64  g users to build
-00000180: 2074 6865 6972 2064 6174 6120 7761 7265   their data ware
-00000190: 686f 7573 6520 6563 6f73 7973 7465 6d20  house ecosystem 
-000001a0: 7769 7468 2064 6274 200a 616e 6420 4279  with dbt .and By
-000001b0: 7465 486f 7573 652e 200a 2320 5461 626c  teHouse. .# Tabl
-000001c0: 6520 6f66 2043 6f6e 7465 6e74 730a 2d20  e of Contents.- 
-000001d0: 5b49 6e74 726f 6475 6374 696f 6e5d 2823  [Introduction](#
-000001e0: 696e 7472 6f64 7563 7469 6f6e 290a 2d20  introduction).- 
-000001f0: 5b52 6571 7569 7265 6d65 6e74 735d 2823  [Requirements](#
-00000200: 7265 7175 6972 656d 656e 7473 290a 2d20  requirements).- 
-00000210: 5b43 7265 6174 696e 6720 4279 7465 486f  [Creating ByteHo
-00000220: 7573 6520 4163 636f 756e 745d 2823 6372  use Account](#cr
-00000230: 6561 7469 6e67 2d62 7974 6568 6f75 7365  eating-bytehouse
-00000240: 2d61 6363 6f75 6e74 290a 2d20 5b49 6e73  -account).- [Ins
-00000250: 7461 6c6c 6174 696f 6e5d 2823 696e 7374  tallation](#inst
-00000260: 616c 6c61 7469 6f6e 290a 2d20 5b64 6274  allation).- [dbt
-00000270: 2050 726f 6a65 6374 2053 6574 7570 5d28   Project Setup](
-00000280: 2364 6274 2d70 726f 6a65 6374 2d73 6574  #dbt-project-set
-00000290: 7570 290a 2020 2a20 5b64 6274 5f70 726f  up).  * [dbt_pro
-000002a0: 6a65 6374 2e79 6d6c 5d28 2364 6274 2d70  ject.yml](#dbt-p
-000002b0: 726f 6a65 6374 796d 6c29 0a20 202a 205b  rojectyml).  * [
-000002c0: 7072 6f66 696c 6573 2e79 6d6c 5d28 2370  profiles.yml](#p
-000002d0: 726f 6669 6c65 7379 6d6c 290a 2020 2a20  rofilesyml).  * 
-000002e0: 5b43 6f6e 6e65 6374 696f 6e20 2620 4175  [Connection & Au
-000002f0: 7468 656e 7469 6361 7469 6f6e 2043 6f6e  thentication Con
-00000300: 6669 6775 7261 7469 6f6e 735d 2823 636f  figurations](#co
-00000310: 6e6e 6563 7469 6f6e 2d2d 2d61 7574 6865  nnection---authe
-00000320: 6e74 6963 6174 696f 6e2d 636f 6e66 6967  ntication-config
-00000330: 7572 6174 696f 6e73 290a 2020 2020 2b20  urations).    + 
-00000340: 5b42 7974 6548 6f75 7365 2052 6567 696f  [ByteHouse Regio
-00000350: 6e73 5d28 2362 7974 6568 6f75 7365 2d72  ns](#bytehouse-r
-00000360: 6567 696f 6e73 290a 2020 2020 2b20 5b52  egions).    + [R
-00000370: 6567 696f 6e20 2620 5061 7373 776f 7264  egion & Password
-00000380: 2043 6f6e 6669 6775 7261 7469 6f6e 5d28   Configuration](
-00000390: 2372 6567 696f 6e2d 2d2d 7061 7373 776f  #region---passwo
-000003a0: 7264 2d63 6f6e 6669 6775 7261 7469 6f6e  rd-configuration
-000003b0: 290a 2020 2020 2b20 5b52 6567 696f 6e20  ).    + [Region 
-000003c0: 2620 4150 4920 4b65 7920 436f 6e66 6967  & API Key Config
-000003d0: 7572 6174 696f 6e5d 2823 7265 6769 6f6e  uration](#region
-000003e0: 2d2d 2d61 7069 2d6b 6579 2d63 6f6e 6669  ---api-key-confi
-000003f0: 6775 7261 7469 6f6e 290a 2020 2020 2b20  guration).    + 
-00000400: 5b48 6f73 7420 4164 6472 6573 7320 2620  [Host Address & 
-00000410: 5061 7373 776f 7264 2043 6f6e 6669 6775  Password Configu
-00000420: 7261 7469 6f6e 5d28 2368 6f73 742d 6164  ration](#host-ad
-00000430: 6472 6573 732d 2d2d 7061 7373 776f 7264  dress---password
-00000440: 2d63 6f6e 6669 6775 7261 7469 6f6e 290a  -configuration).
-00000450: 2020 2020 2b20 5b48 6f73 7420 4164 6472      + [Host Addr
-00000460: 6573 7320 2620 4150 4920 4b65 7920 436f  ess & API Key Co
-00000470: 6e66 6967 7572 6174 696f 6e5d 2823 686f  nfiguration](#ho
-00000480: 7374 2d61 6464 7265 7373 2d2d 2d61 7069  st-address---api
-00000490: 2d6b 6579 2d63 6f6e 6669 6775 7261 7469  -key-configurati
-000004a0: 6f6e 290a 2020 2a20 5b50 726f 6a65 6374  on).  * [Project
-000004b0: 2049 6e69 7469 616c 697a 6174 696f 6e5d   Initialization]
-000004c0: 2823 7072 6f6a 6563 742d 696e 6974 6961  (#project-initia
-000004d0: 6c69 7a61 7469 6f6e 290a 2020 2a20 5b54  lization).  * [T
-000004e0: 6573 7420 5761 7265 686f 7573 6520 436f  est Warehouse Co
-000004f0: 6e6e 6563 7469 6f6e 5d28 2374 6573 742d  nnection](#test-
-00000500: 7761 7265 686f 7573 652d 636f 6e6e 6563  warehouse-connec
-00000510: 7469 6f6e 290a 2d20 5b44 6174 6173 6574  tion).- [Dataset
-00000520: 2049 6e67 6573 7469 6f6e 5d28 2364 6174   Ingestion](#dat
-00000530: 6173 6574 2d69 6e67 6573 7469 6f6e 290a  aset-ingestion).
-00000540: 2d20 5b64 6274 204d 6f64 656c 735d 2823  - [dbt Models](#
-00000550: 6462 742d 6d6f 6465 6c73 290a 2d20 5b73  dbt-models).- [s
-00000560: 6368 656d 612e 796d 6c5d 2823 7363 6865  chema.yml](#sche
-00000570: 6d61 796d 6c29 0a2d 205b 4d61 7465 7269  mayml).- [Materi
-00000580: 616c 697a 6174 696f 6e20 7479 7065 7320  alization types 
-00000590: 6f66 204d 6f64 656c 735d 2823 6d61 7465  of Models](#mate
-000005a0: 7269 616c 697a 6174 696f 6e2d 7479 7065  rialization-type
-000005b0: 732d 6f66 2d6d 6f64 656c 7329 0a20 202a  s-of-models).  *
-000005c0: 205b 5669 6577 204d 6174 6572 6961 6c69   [View Materiali
-000005d0: 7a61 7469 6f6e 735d 2823 7669 6577 2d6d  zations](#view-m
-000005e0: 6174 6572 6961 6c69 7a61 7469 6f6e 7329  aterializations)
-000005f0: 0a20 202a 205b 5461 626c 6520 4d61 7465  .  * [Table Mate
-00000600: 7269 616c 697a 6174 696f 6e73 5d28 2374  rializations](#t
-00000610: 6162 6c65 2d6d 6174 6572 6961 6c69 7a61  able-materializa
-00000620: 7469 6f6e 7329 0a20 202a 205b 496e 6372  tions).  * [Incr
-00000630: 656d 656e 7461 6c20 4d61 7465 7269 616c  emental Material
-00000640: 697a 6174 696f 6e73 5d28 2369 6e63 7265  izations](#incre
-00000650: 6d65 6e74 616c 2d6d 6174 6572 6961 6c69  mental-materiali
-00000660: 7a61 7469 6f6e 7329 0a20 2020 202b 205b  zations).    + [
-00000670: 486f 7720 6974 2077 6f72 6b73 5d28 2368  How it works](#h
-00000680: 6f77 2d69 742d 776f 726b 7329 0a2d 205b  ow-it-works).- [
-00000690: 5072 6f6a 6563 7420 446f 6375 6d65 6e74  Project Document
-000006a0: 6174 696f 6e5d 2823 7072 6f6a 6563 742d  ation](#project-
-000006b0: 646f 6375 6d65 6e74 6174 696f 6e29 0a2d  documentation).-
-000006c0: 205b 4c6f 6361 6c20 4465 7665 6c6f 706d   [Local Developm
-000006d0: 656e 745d 2823 6c6f 6361 6c2d 6465 7665  ent](#local-deve
-000006e0: 6c6f 706d 656e 7429 0a2d 205b 4f72 6967  lopment).- [Orig
-000006f0: 696e 616c 2041 7574 686f 725d 2823 6f72  inal Author](#or
-00000700: 6967 696e 616c 2d61 7574 686f 7229 0a2d  iginal-author).-
-00000710: 205b 4c69 6365 6e73 655d 2823 6c69 6365   [License](#lice
-00000720: 6e73 6529 0a23 2052 6571 7569 7265 6d65  nse).# Requireme
-00000730: 6e74 730a 4d61 6b65 2073 7572 6520 796f  nts.Make sure yo
-00000740: 7520 6861 7665 2060 6462 7460 2026 2060  u have `dbt` & `
-00000750: 7079 7468 6f6e 6020 696e 7374 616c 6c65  python` installe
-00000760: 6420 6f6e 2079 6f75 7220 6d61 6368 696e  d on your machin
-00000770: 652e 2049 6620 6e6f 742c 2074 6865 6e20  e. If not, then 
-00000780: 796f 7520 6361 6e20 666f 6c6c 6f77 2074  you can follow t
-00000790: 6869 7320 6775 6964 6520 6874 7470 733a  his guide https:
-000007a0: 2f2f 646f 6373 2e67 6574 6462 742e 636f  //docs.getdbt.co
-000007b0: 6d2f 646f 6373 2f67 6574 2d73 7461 7274  m/docs/get-start
-000007c0: 6564 2f69 6e73 7461 6c6c 6174 696f 6e0a  ed/installation.
-000007d0: 2d20 6462 7420 7631 2e37 2e30 206f 7220  - dbt v1.7.0 or 
-000007e0: 6772 6561 7465 720a 2d20 7079 7468 6f6e  greater.- python
-000007f0: 2076 332e 3720 6f72 2067 7265 6174 6572   v3.7 or greater
-00000800: 0a23 2043 7265 6174 696e 6720 4279 7465  .# Creating Byte
-00000810: 486f 7573 6520 4163 636f 756e 740a 596f  House Account.Yo
-00000820: 7520 6e65 6564 2074 6f20 6372 6561 7465  u need to create
-00000830: 2042 7974 6548 6f75 7365 2061 6363 6f75   ByteHouse accou
-00000840: 6e74 2069 6e20 6f72 6465 7220 746f 2075  nt in order to u
-00000850: 7365 2062 7974 6568 6f75 7365 2d64 6274  se bytehouse-dbt
-00000860: 2063 6f6e 6e65 6374 6f72 2e20 596f 7520   connector. You 
-00000870: 6361 6e20 7369 6d70 6c79 2063 7265 6174  can simply creat
-00000880: 6520 6120 6672 6565 2061 6363 6f75 6e74  e a free account
-00000890: 2077 6974 680a 7468 6520 7072 6f63 6573   with.the proces
-000008a0: 7320 6d65 6e74 696f 6e65 6420 696e 206f  s mentioned in o
-000008b0: 7572 206f 6666 6963 6961 6c20 7765 6273  ur official webs
-000008c0: 6974 6520 646f 6375 6d65 6e74 6174 696f  ite documentatio
-000008d0: 6e3a 2068 7474 7073 3a2f 2f64 6f63 732e  n: https://docs.
-000008e0: 6279 7465 686f 7573 652e 636c 6f75 642f  bytehouse.cloud/
-000008f0: 656e 2f64 6f63 732f 7175 6963 6b2d 7374  en/docs/quick-st
-00000900: 6172 7420 3c62 722f 3e0a 0a59 6f75 2063  art <br/>..You c
-00000910: 616e 2061 6c73 6f20 6372 6561 7465 2042  an also create B
-00000920: 7974 6548 6f75 7365 2061 6363 6f75 6e74  yteHouse account
-00000930: 2074 6872 6f75 6768 2056 6f6c 6361 6e6f   through Volcano
-00000940: 2045 6e67 696e 6520 6279 2042 7974 6544   Engine by ByteD
-00000950: 616e 6365 3a20 0a68 7474 7073 3a2f 2f77  ance: .https://w
-00000960: 7777 2e76 6f6c 6365 6e67 696e 652e 636f  ww.volcengine.co
-00000970: 6d2f 7072 6f64 7563 742f 6279 7465 686f  m/product/byteho
-00000980: 7573 652d 636c 6f75 6420 0a23 2049 6e73  use-cloud .# Ins
-00000990: 7461 6c6c 6174 696f 6e0a 4372 6561 7465  tallation.Create
-000009a0: 2061 206e 6577 2072 6570 6f73 6974 6f72   a new repositor
-000009b0: 7920 7768 6572 6520 7765 2077 696c 6c20  y where we will 
-000009c0: 696e 7374 616e 7469 6174 6520 6120 6050  instantiate a `P
-000009d0: 7974 686f 6e60 2076 6972 7475 616c 2065  ython` virtual e
-000009e0: 6e76 6972 6f6e 6d65 6e74 2e0a 6060 6063  nvironment..```c
-000009f0: 6f6d 6d61 6e64 6c69 6e65 0a6d 6b64 6972  ommandline.mkdir
-00000a00: 2064 6274 5f62 7974 6568 6f75 7365 5f64   dbt_bytehouse_d
-00000a10: 656d 6f0a 6364 2064 6274 5f62 7974 6568  emo.cd dbt_byteh
-00000a20: 6f75 7365 5f64 656d 6f0a 0a70 7974 686f  ouse_demo..pytho
-00000a30: 6e20 2d6d 2076 656e 7620 7665 6e76 0a73  n -m venv venv.s
-00000a40: 6f75 7263 6520 7665 6e76 2f62 696e 2f61  ource venv/bin/a
-00000a50: 6374 6976 6174 650a 6060 600a 4c61 7465  ctivate.```.Late
-00000a60: 7374 2072 656c 6561 7365 2076 6572 7369  st release versi
-00000a70: 6f6e 2063 616e 2062 6520 696e 7374 616c  on can be instal
-00000a80: 6c65 6420 6672 6f6d 2068 6572 653a 0a60  led from here:.`
-00000a90: 6060 636f 6d6d 616e 646c 696e 650a 7069  ``commandline.pi
-00000aa0: 7020 696e 7374 616c 6c20 6462 742d 6279  p install dbt-by
-00000ab0: 7465 686f 7573 650a 6060 600a 4375 7272  tehouse.```.Curr
-00000ac0: 656e 7420 6465 7665 6c6f 706d 656e 7420  ent development 
-00000ad0: 7665 7273 696f 6e20 6361 6e20 6265 2069  version can be i
-00000ae0: 6e73 7461 6c6c 6564 2066 726f 6d20 6865  nstalled from he
-00000af0: 7265 3a0a 6060 6063 6f6d 6d61 6e64 6c69  re:.```commandli
-00000b00: 6e65 0a70 6970 2069 6e73 7461 6c6c 2067  ne.pip install g
-00000b10: 6974 2b68 7474 7073 3a2f 2f67 6974 6875  it+https://githu
-00000b20: 622e 636f 6d2f 6279 7465 686f 7573 652d  b.com/bytehouse-
-00000b30: 636c 6f75 642f 6279 7465 686f 7573 652d  cloud/bytehouse-
-00000b40: 6462 7440 6d61 7374 6572 2365 6767 3d62  dbt@master#egg=b
-00000b50: 7974 6568 6f75 7365 2d64 7269 7665 720a  ytehouse-driver.
-00000b60: 6060 600a 4368 6563 6b20 7768 6574 6865  ```.Check whethe
-00000b70: 7220 696e 7374 616c 6c61 7469 6f6e 2069  r installation i
-00000b80: 7320 7375 6363 6573 7366 756c 2062 7920  s successful by 
-00000b90: 7665 7269 6679 696e 6720 6279 7465 686f  verifying byteho
-00000ba0: 7573 6520 6973 2061 7661 696c 6162 6c65  use is available
-00000bb0: 2075 6e64 6572 2050 6c75 6769 6e73 2e0a   under Plugins..
-00000bc0: 6060 6063 6f6d 6d61 6e64 6c69 6e65 0a64  ```commandline.d
-00000bd0: 6274 202d 2d76 6572 7369 6f6e 0a60 6060  bt --version.```
-00000be0: 0a21 5b56 6572 7369 6f6e 5d28 2e2f 6578  .![Version](./ex
-00000bf0: 616d 706c 6573 2f31 5f76 6572 7369 6f6e  amples/1_version
-00000c00: 2e70 6e67 290a 2320 6462 7420 5072 6f6a  .png).# dbt Proj
-00000c10: 6563 7420 5365 7475 700a 2323 2064 6274  ect Setup.## dbt
-00000c20: 5f70 726f 6a65 6374 2e79 6d6c 0a45 7665  _project.yml.Eve
-00000c30: 7279 2060 6462 7460 2070 726f 6a65 6374  ry `dbt` project
-00000c40: 206e 6565 6473 2061 2060 6462 745f 7072   needs a `dbt_pr
-00000c50: 6f6a 6563 742e 796d 6c60 2066 696c 6520  oject.yml` file 
-00000c60: e280 9420 7468 6973 2069 7320 686f 7720  ... this is how 
-00000c70: 6064 6274 6020 6b6e 6f77 7320 6120 6469  `dbt` knows a di
-00000c80: 7265 6374 6f72 7920 6973 2061 2060 6462  rectory is a `db
-00000c90: 7460 2070 726f 6a65 6374 2e20 6064 6274  t` project. `dbt
-00000ca0: 5f70 726f 6a65 6374 2e79 6d6c 600a 6669  _project.yml`.fi
-00000cb0: 6c65 2068 6f6c 6473 2074 6865 2063 6f6e  le holds the con
-00000cc0: 7465 7874 206f 6620 796f 7572 2070 726f  text of your pro
-00000cd0: 6a65 6374 2061 6e64 2074 656c 6c73 2060  ject and tells `
-00000ce0: 6462 7460 2068 6f77 2074 6f20 6275 696c  dbt` how to buil
-00000cf0: 6420 796f 7572 2064 6174 6120 7365 7473  d your data sets
-00000d00: 2e20 536f 6d65 2063 6f6d 6d6f 6e20 636f  . Some common co
-00000d10: 6e66 6967 7572 6174 696f 6e73 0a66 6f72  nfigurations.for
-00000d20: 2060 6462 745f 7072 6f6a 6563 742e 796d   `dbt_project.ym
-00000d30: 6c60 2061 7265 3a0a 3c74 6162 6c65 3e0a  l` are:.<table>.
-00000d40: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
-00000d50: 203c 7464 3e59 414d 4c20 6b65 793c 2f74   <td>YAML key</t
-00000d60: 643e 0a20 2020 2020 2020 203c 7464 3e56  d>.        <td>V
-00000d70: 616c 7565 3c2f 7464 3e0a 2020 2020 3c2f  alue</td>.    </
-00000d80: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
-00000d90: 2020 2020 203c 7464 3e6e 616d 653c 2f74       <td>name</t
-00000da0: 643e 0a20 2020 2020 2020 203c 7464 3e59  d>.        <td>Y
-00000db0: 6f75 7220 7072 6f6a 6563 74e2 8099 7320  our project...s 
-00000dc0: 6e61 6d65 2069 6e20 736e 616b 6520 6361  name in snake ca
-00000dd0: 7365 3c2f 7464 3e0a 2020 2020 3c2f 7472  se</td>.    </tr
-00000de0: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00000df0: 2020 203c 7464 3e76 6572 7369 6f6e 3c2f     <td>version</
-00000e00: 7464 3e0a 2020 2020 2020 2020 3c74 643e  td>.        <td>
-00000e10: 5665 7273 696f 6e20 6f66 2079 6f75 7220  Version of your 
-00000e20: 7072 6f6a 6563 743c 2f74 643e 0a20 2020  project</td>.   
-00000e30: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
-00000e40: 2020 2020 2020 2020 3c74 643e 7072 6f66          <td>prof
-00000e50: 696c 653c 2f74 643e 0a20 2020 2020 2020  ile</td>.       
-00000e60: 203c 7464 3e54 6865 2070 726f 6669 6c65   <td>The profile
-00000e70: 2064 6274 2075 7365 7320 746f 2063 6f6e   dbt uses to con
-00000e80: 6e65 6374 2074 6f20 4279 7465 486f 7573  nect to ByteHous
-00000e90: 653c 2f74 643e 0a20 2020 203c 2f74 723e  e</td>.    </tr>
-00000ea0: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
-00000eb0: 2020 3c74 643e 6d6f 6465 6c2d 7061 7468    <td>model-path
-00000ec0: 733c 2f74 643e 0a20 2020 2020 2020 203c  s</td>.        <
-00000ed0: 7464 3e44 6972 6563 746f 7269 6573 2074  td>Directories t
-00000ee0: 6f20 7768 6572 6520 796f 7572 206d 6f64  o where your mod
-00000ef0: 656c 2061 6e64 2073 6f75 7263 6520 6669  el and source fi
-00000f00: 6c65 7320 6c69 7665 3c2f 7464 3e0a 2020  les live</td>.  
-00000f10: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
-00000f20: 0a20 2020 2020 2020 203c 7464 3e73 6565  .        <td>see
-00000f30: 642d 7061 7468 733c 2f74 643e 0a20 2020  d-paths</td>.   
-00000f40: 2020 2020 203c 7464 3e44 6972 6563 746f       <td>Directo
-00000f50: 7269 6573 2074 6f20 7768 6572 6520 796f  ries to where yo
-00000f60: 7572 2073 6565 6420 6669 6c65 7320 6c69  ur seed files li
-00000f70: 7665 3c2f 7464 3e0a 2020 2020 3c2f 7472  ve</td>.    </tr
-00000f80: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00000f90: 2020 203c 7464 3e74 6573 742d 7061 7468     <td>test-path
-00000fa0: 733c 2f74 643e 0a20 2020 2020 2020 203c  s</td>.        <
-00000fb0: 7464 3e44 6972 6563 746f 7269 6573 2074  td>Directories t
-00000fc0: 6f20 7768 6572 6520 796f 7572 2074 6573  o where your tes
-00000fd0: 7420 6669 6c65 7320 6c69 7665 3c2f 7464  t files live</td
-00000fe0: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
-00000ff0: 3c74 723e 0a20 2020 2020 2020 203c 7464  <tr>.        <td
-00001000: 3e73 6e61 7073 686f 742d 7061 7468 733c  >snapshot-paths<
-00001010: 2f74 643e 0a20 2020 2020 2020 203c 7464  /td>.        <td
-00001020: 3e44 6972 6563 746f 7269 6573 2074 6f20  >Directories to 
-00001030: 7768 6572 6520 796f 7572 2073 6e61 7073  where your snaps
-00001040: 686f 7473 206c 6976 653c 2f74 643e 0a20  hots live</td>. 
-00001050: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
-00001060: 3e0a 2020 2020 2020 2020 3c74 643e 646f  >.        <td>do
-00001070: 6373 2d70 6174 6873 3c2f 7464 3e0a 2020  cs-paths</td>.  
-00001080: 2020 2020 2020 3c74 643e 4469 7265 6374        <td>Direct
-00001090: 6f72 6965 7320 746f 2077 6865 7265 2079  ories to where y
-000010a0: 6f75 7220 646f 6373 2062 6c6f 636b 7320  our docs blocks 
-000010b0: 6c69 7665 3c2f 7464 3e0a 2020 2020 3c2f  live</td>.    </
-000010c0: 7472 3e0a 3c2f 7461 626c 653e 0a0a 2323  tr>.</table>..##
-000010d0: 2070 726f 6669 6c65 732e 796d 6c0a 5768   profiles.yml.Wh
-000010e0: 656e 2079 6f75 2069 6e76 6f6b 6520 6064  en you invoke `d
-000010f0: 6274 6020 6672 6f6d 2074 6865 2063 6f6d  bt` from the com
-00001100: 6d61 6e64 206c 696e 652c 2060 6462 7460  mand line, `dbt`
-00001110: 2070 6172 7365 7320 796f 7572 2060 6462   parses your `db
-00001120: 745f 7072 6f6a 6563 742e 796d 6c60 2061  t_project.yml` a
-00001130: 6e64 206f 6274 6169 6e73 2074 6865 2070  nd obtains the p
-00001140: 726f 6669 6c65 206e 616d 652e 2060 6462  rofile name. `db
-00001150: 7460 2074 6865 6e20 0a63 6865 636b 7320  t` then .checks 
-00001160: 796f 7572 2060 7072 6f66 696c 6573 2e79  your `profiles.y
-00001170: 6d6c 6020 6669 6c65 2066 6f72 2061 2070  ml` file for a p
-00001180: 726f 6669 6c65 2077 6974 6820 7468 6520  rofile with the 
-00001190: 7361 6d65 206e 616d 652e 2041 2070 726f  same name. A pro
-000011a0: 6669 6c65 2063 6f6e 7461 696e 7320 616c  file contains al
-000011b0: 6c20 7468 6520 6465 7461 696c 732f 6372  l the details/cr
-000011c0: 6564 656e 7469 616c 7320 0a72 6571 7569  edentials .requi
-000011d0: 7265 6420 746f 2063 6f6e 6e65 6374 2074  red to connect t
-000011e0: 6f20 4279 7465 486f 7573 652e 2060 6462  o ByteHouse. `db
-000011f0: 7460 2077 696c 6c20 7365 6172 6368 2074  t` will search t
-00001200: 6865 2063 7572 7265 6e74 2077 6f72 6b69  he current worki
-00001210: 6e67 2064 6972 6563 746f 7279 2066 6f72  ng directory for
-00001220: 2074 6865 2060 7072 6f66 696c 6573 2e79   the `profiles.y
-00001230: 6d6c 6020 6669 6c65 2061 6e64 2077 696c  ml` file and wil
-00001240: 6c0a 6465 6661 756c 7420 746f 2074 6865  l.default to the
-00001250: 2060 7e2f 2e64 6274 2f20 6469 7265 6374   `~/.dbt/ direct
-00001260: 6f72 7960 2069 6620 6e6f 7420 666f 756e  ory` if not foun
-00001270: 642e 0a60 6060 7961 6d6c 0a3c 7072 6f66  d..```yaml.<prof
-00001280: 696c 652d 6e61 6d65 3e3a 0a20 2074 6172  ile-name>:.  tar
-00001290: 6765 743a 203c 7461 7267 6574 2d6e 616d  get: <target-nam
-000012a0: 653e 0a20 206f 7574 7075 7473 3a0a 2020  e>.  outputs:.  
-000012b0: 2020 3c74 6172 6765 742d 6e61 6d65 3e3a    <target-name>:
-000012c0: 0a20 2020 2020 2074 7970 653a 2062 7974  .      type: byt
-000012d0: 6568 6f75 7365 0a20 2020 2020 2073 6368  ehouse.      sch
-000012e0: 656d 613a 203c 6461 7461 6261 7365 2d6e  ema: <database-n
-000012f0: 616d 653e 0a20 2020 2020 2075 7365 723a  ame>.      user:
-00001300: 203c 7573 6572 6e61 6d65 3e0a 2020 2020   <username>.    
-00001310: 2020 7061 7373 776f 7264 3a20 3c70 6173    password: <pas
-00001320: 7377 6f72 643e 0a20 2020 2020 2064 7269  sword>.      dri
-00001330: 7665 723a 206e 6174 6976 650a 2020 2020  ver: native.    
-00001340: 2020 236f 7074 696f 6e61 6c20 6669 656c    #optional fiel
-00001350: 6473 0a20 2020 2020 2068 6f73 743a 203c  ds.      host: <
-00001360: 686f 7374 6e61 6d65 3e0a 2020 2020 2020  hostname>.      
-00001370: 706f 7274 3a20 3c70 6f72 743e 0a20 2020  port: <port>.   
-00001380: 2020 2072 6567 696f 6e3a 203c 7265 6769     region: <regi
-00001390: 6f6e 2d6e 616d 653e 0a20 2020 2020 2061  on-name>.      a
-000013a0: 6363 6f75 6e74 3a20 3c61 6363 6f75 6e74  ccount: <account
-000013b0: 2d6e 616d 653e 0a20 2020 2020 2077 6172  -name>.      war
-000013c0: 6568 6f75 7365 3a20 3c77 6172 6568 6f75  ehouse: <warehou
-000013d0: 7365 2d6e 616d 653e 0a20 2020 2020 2072  se-name>.      r
-000013e0: 6574 7269 6573 3a20 310a 2020 2020 2020  etries: 1.      
-000013f0: 7365 6375 7265 3a20 5472 7565 0a20 2020  secure: True.   
-00001400: 2020 2063 6f6e 6e65 6374 5f74 696d 656f     connect_timeo
-00001410: 7574 3a20 3130 0a20 2020 2020 2073 656e  ut: 10.      sen
-00001420: 645f 7265 6365 6976 655f 7469 6d65 6f75  d_receive_timeou
-00001430: 743a 2033 3030 0a20 2020 2020 2063 7573  t: 300.      cus
-00001440: 746f 6d5f 7365 7474 696e 6773 3a20 3c65  tom_settings: <e
-00001450: 6d70 7479 3e0a 6060 600a 3c74 6162 6c65  mpty>.```.<table
-00001460: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00001470: 2020 203c 7464 3e59 414d 4c20 6b65 793c     <td>YAML key<
-00001480: 2f74 643e 0a20 2020 2020 2020 203c 7464  /td>.        <td
-00001490: 3e56 616c 7565 3c2f 7464 3e0a 2020 2020  >Value</td>.    
-000014a0: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
-000014b0: 2020 2020 2020 203c 7464 3e26 6c74 3b70         <td>&lt;p
-000014c0: 726f 6669 6c65 2d6e 616d 6526 6774 3b3c  rofile-name&gt;<
-000014d0: 2f74 643e 0a20 2020 2020 2020 203c 7464  /td>.        <td
-000014e0: 3e4e 616d 6520 6f66 2074 6865 2070 726f  >Name of the pro
-000014f0: 6669 6c65 2e20 4861 7320 746f 2062 6520  file. Has to be 
-00001500: 7468 6520 7361 6d65 206e 616d 6520 6173  the same name as
-00001510: 2074 6865 2070 726f 6669 6c65 2069 6e64   the profile ind
-00001520: 6963 6174 6564 2069 6e20 796f 7572 2064  icated in your d
-00001530: 6274 5f70 726f 6a65 6374 2e79 6d6c 2066  bt_project.yml f
-00001540: 696c 653c 2f74 643e 0a20 2020 203c 2f74  ile</td>.    </t
-00001550: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
-00001560: 2020 2020 3c74 643e 7461 7267 6574 3c2f      <td>target</
-00001570: 7464 3e0a 2020 2020 2020 2020 3c74 643e  td>.        <td>
-00001580: 4465 6661 756c 7420 7461 7267 6574 2079  Default target y
-00001590: 6f75 7220 6462 7420 7072 6f6a 6563 7420  our dbt project 
-000015a0: 7769 6c6c 2075 7365 2e20 4974 206d 7573  will use. It mus
-000015b0: 7420 6265 206f 6e65 206f 6620 7468 6520  t be one of the 
-000015c0: 7461 7267 6574 7320 796f 7520 6465 6669  targets you defi
-000015d0: 6e65 2069 6e20 796f 7572 2070 726f 6669  ne in your profi
-000015e0: 6c65 3c2f 7464 3e0a 2020 2020 3c2f 7472  le</td>.    </tr
-000015f0: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00001600: 2020 203c 7464 3e74 7970 653c 2f74 643e     <td>type</td>
-00001610: 0a20 2020 2020 2020 203c 7464 3e4d 7573  .        <td>Mus
-00001620: 7420 6265 2073 6574 2074 6f20 6279 7465  t be set to byte
-00001630: 686f 7573 653c 2f74 643e 0a20 2020 203c  house</td>.    <
-00001640: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
-00001650: 2020 2020 2020 3c74 643e 7363 6865 6d61        <td>schema
-00001660: 3c2f 7464 3e0a 2020 2020 2020 2020 3c74  </td>.        <t
-00001670: 643e 4461 7461 6261 7365 206e 616d 653c  d>Database name<
-00001680: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
-00001690: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
-000016a0: 3c74 643e 7573 6572 3c2f 7464 3e0a 2020  <td>user</td>.  
-000016b0: 2020 2020 2020 3c74 643e 5573 6572 6e61        <td>Userna
-000016c0: 6d65 2077 6974 6820 6164 6571 7561 7465  me with adequate
-000016d0: 2070 6572 6d69 7373 696f 6e73 2074 6f20   permissions to 
-000016e0: 6163 6365 7373 2074 6865 2073 7065 6369  access the speci
-000016f0: 6669 6564 2073 6368 656d 612e 2046 6f72  fied schema. For
-00001700: 2041 5049 204b 6579 2061 7574 6865 6e74   API Key authent
-00001710: 6963 6174 696f 6e2c 2075 7365 7220 6d75  ication, user mu
-00001720: 7374 2062 6520 7365 7420 746f 2062 7974  st be set to byt
-00001730: 6568 6f75 7365 3c2f 7464 3e0a 2020 2020  ehouse</td>.    
-00001740: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
-00001750: 2020 2020 2020 203c 7464 3e70 6173 7377         <td>passw
-00001760: 6f72 643c 2f74 643e 0a20 2020 2020 2020  ord</td>.       
-00001770: 203c 7464 3e54 6865 2070 6173 7377 6f72   <td>The passwor
-00001780: 6420 6173 736f 6369 6174 6564 2077 6974  d associated wit
-00001790: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
-000017a0: 7573 6572 3c2f 7464 3e0a 2020 2020 3c2f  user</td>.    </
-000017b0: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
-000017c0: 2020 2020 203c 7464 3e64 7269 7665 723c       <td>driver<
-000017d0: 2f74 643e 0a20 2020 2020 2020 203c 7464  /td>.        <td
-000017e0: 3e4d 7573 7420 6265 2073 6574 2074 6f20  >Must be set to 
-000017f0: 6e61 7469 7665 3c2f 7464 3e0a 2020 2020  native</td>.    
-00001800: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
-00001810: 2020 2020 2020 203c 7464 3e68 6f73 743c         <td>host<
-00001820: 2f74 643e 0a20 2020 2020 2020 203c 7464  /td>.        <td
-00001830: 3e5b 4f70 7469 6f6e 616c 5d20 5468 6520  >[Optional] The 
-00001840: 686f 7374 206e 616d 6520 6f66 2074 6865  host name of the
-00001850: 2063 6f6e 6e65 6374 696f 6e3c 2f74 643e   connection</td>
-00001860: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
-00001870: 7472 3e0a 2020 2020 2020 2020 3c74 643e  tr>.        <td>
-00001880: 706f 7274 203c 2f74 643e 0a20 2020 2020  port </td>.     
-00001890: 2020 203c 7464 3e5b 4f70 7469 6f6e 616c     <td>[Optional
-000018a0: 5d20 5468 6520 706f 7274 206e 756d 6265  ] The port numbe
-000018b0: 7220 6f66 2074 6865 2068 6f73 7420 7365  r of the host se
-000018c0: 7276 6572 3c2f 7464 3e0a 2020 2020 3c2f  rver</td>.    </
-000018d0: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
-000018e0: 2020 2020 203c 7464 3e72 6567 696f 6e3c       <td>region<
-000018f0: 2f74 643e 0a20 2020 2020 2020 203c 7464  /td>.        <td
-00001900: 3e5b 4f70 7469 6f6e 616c 5d20 416c 6961  >[Optional] Alia
-00001910: 7320 666f 7220 686f 7374 2026 616d 703b  s for host &amp;
-00001920: 2070 6f72 7420 3c2f 7464 3e0a 2020 2020   port </td>.    
-00001930: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
-00001940: 2020 2020 2020 203c 7464 3e61 6363 6f75         <td>accou
-00001950: 6e74 3c2f 7464 3e0a 2020 2020 2020 2020  nt</td>.        
-00001960: 3c74 643e 5b4f 7074 696f 6e61 6c5d 2042  <td>[Optional] B
-00001970: 7974 6548 6f75 7365 2061 6363 6f75 6e74  yteHouse account
-00001980: 206e 756d 6265 723c 2f74 643e 0a20 2020   number</td>.   
-00001990: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
-000019a0: 2020 2020 2020 2020 3c74 643e 7761 7265          <td>ware
-000019b0: 686f 7573 653c 2f74 643e 0a20 2020 2020  house</td>.     
-000019c0: 2020 203c 7464 3e5b 4f70 7469 6f6e 616c     <td>[Optional
-000019d0: 5d20 5468 6520 6e61 6d65 206f 6620 7468  ] The name of th
-000019e0: 6520 7669 7274 7561 6c20 7761 7265 686f  e virtual wareho
-000019f0: 7573 6520 7468 6174 2079 6f75 2077 616e  use that you wan
-00001a00: 7420 746f 2075 7365 2066 6f72 2074 6869  t to use for thi
-00001a10: 7320 7365 7373 696f 6e3c 2f74 643e 0a20  s session</td>. 
-00001a20: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
-00001a30: 3e0a 2020 2020 2020 2020 3c74 643e 7265  >.        <td>re
-00001a40: 7472 6965 733c 2f74 643e 0a20 2020 2020  tries</td>.     
-00001a50: 2020 203c 7464 3e5b 4f70 7469 6f6e 616c     <td>[Optional
-00001a60: 5d20 4e75 6d62 6572 206f 6620 7469 6d65  ] Number of time
-00001a70: 7320 746f 2072 6574 7279 2074 6865 2069  s to retry the i
-00001a80: 6e69 7469 616c 2063 6f6e 6e65 6374 696f  nitial connectio
-00001a90: 6e20 6174 7465 6d70 7420 6966 2074 6865  n attempt if the
-00001aa0: 2065 7272 6f72 2061 7070 6561 7273 2074   error appears t
-00001ab0: 6f20 6265 2072 6563 6f76 6572 6162 6c65  o be recoverable
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6462 742d  : 2.1.Name: dbt-
+00000020: 6279 7465 686f 7573 650a 5665 7273 696f  bytehouse.Versio
+00000030: 6e3a 2031 2e37 2e32 0a53 756d 6d61 7279  n: 1.7.2.Summary
+00000040: 3a20 5468 6520 4279 7465 486f 7573 6520  : The ByteHouse 
+00000050: 706c 7567 696e 2066 6f72 2064 6274 2028  plugin for dbt (
+00000060: 6461 7461 2062 7569 6c64 2074 6f6f 6c29  data build tool)
+00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
+00000080: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+00000090: 7974 6568 6f75 7365 2d63 6c6f 7564 2f62  ytehouse-cloud/b
+000000a0: 7974 6568 6f75 7365 2d64 6274 0a41 7574  ytehouse-dbt.Aut
+000000b0: 686f 723a 2052 6166 7361 6e20 4d61 7a75  hor: Rafsan Mazu
+000000c0: 6d64 6572 0a41 7574 686f 722d 656d 6169  mder.Author-emai
+000000d0: 6c3a 2072 6166 7361 6e2e 6d61 7a75 6d64  l: rafsan.mazumd
+000000e0: 6572 4062 7974 6564 616e 6365 2e63 6f6d  er@bytedance.com
+000000f0: 0a4c 6963 656e 7365 3a20 4d49 540a 5072  .License: MIT.Pr
+00000100: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
+00000110: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
+00000120: 2f2f 6769 7468 7562 2e63 6f6d 2f62 7974  //github.com/byt
+00000130: 6568 6f75 7365 2d63 6c6f 7564 2f62 7974  ehouse-cloud/byt
+00000140: 6568 6f75 7365 2d64 6274 0a50 726f 6a65  ehouse-dbt.Proje
+00000150: 6374 2d55 524c 3a20 4368 616e 6765 732c  ct-URL: Changes,
+00000160: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000170: 636f 6d2f 6279 7465 686f 7573 652d 636c  com/bytehouse-cl
+00000180: 6f75 642f 6279 7465 686f 7573 652d 6462  oud/bytehouse-db
+00000190: 742f 626c 6f62 2f6d 6169 6e2f 4348 414e  t/blob/main/CHAN
+000001a0: 4745 4c4f 472e 6d64 0a4b 6579 776f 7264  GELOG.md.Keyword
+000001b0: 733a 2042 7974 6548 6f75 7365 2064 6274  s: ByteHouse dbt
+000001c0: 2063 6f6e 6e65 6374 6f72 0a50 6c61 7466   connector.Platf
+000001d0: 6f72 6d3a 2061 6e79 0a43 6c61 7373 6966  orm: any.Classif
+000001e0: 6965 723a 2044 6576 656c 6f70 6d65 6e74  ier: Development
+000001f0: 2053 7461 7475 7320 3a3a 2035 202d 2050   Status :: 5 - P
+00000200: 726f 6475 6374 696f 6e2f 5374 6162 6c65  roduction/Stable
+00000210: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000220: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000230: 6f76 6564 203a 3a20 4170 6163 6865 2053  oved :: Apache S
+00000240: 6f66 7477 6172 6520 4c69 6365 6e73 650a  oftware License.
+00000250: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
+00000260: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000270: 4d69 6372 6f73 6f66 7420 3a3a 2057 696e  Microsoft :: Win
+00000280: 646f 7773 0a43 6c61 7373 6966 6965 723a  dows.Classifier:
+00000290: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
+000002a0: 6d20 3a3a 204d 6163 4f53 203a 3a20 4d61  m :: MacOS :: Ma
+000002b0: 634f 5320 580a 436c 6173 7369 6669 6572  cOS X.Classifier
+000002c0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+000002d0: 656d 203a 3a20 504f 5349 5820 3a3a 204c  em :: POSIX :: L
+000002e0: 696e 7578 0a43 6c61 7373 6966 6965 723a  inux.Classifier:
+000002f0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000300: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000310: 3a3a 2033 2e37 0a43 6c61 7373 6966 6965  :: 3.7.Classifie
+00000320: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000330: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000340: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
+00000350: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000360: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000370: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
+00000380: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000390: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000003a0: 7974 686f 6e20 3a3a 2033 2e31 300a 5265  ython :: 3.10.Re
+000003b0: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+000003c0: 3d33 2e37 0a44 6573 6372 6970 7469 6f6e  =3.7.Description
+000003d0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000003e0: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
+000003f0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+00000400: 5345 0a0a 2320 496e 7472 6f64 7563 7469  SE..# Introducti
+00000410: 6f6e 0a60 6462 7460 2028 4461 7461 2042  on.`dbt` (Data B
+00000420: 7569 6c64 696e 6720 546f 6f6c 2920 6973  uilding Tool) is
+00000430: 2061 6e20 6f70 656e 2073 6f75 7263 6520   an open source 
+00000440: 746f 6f6c 2074 6861 7420 656e 6162 6c65  tool that enable
+00000450: 7320 6461 7461 2061 6e61 6c79 7374 7320  s data analysts 
+00000460: 616e 6420 656e 6769 6e65 6572 7320 746f  and engineers to
+00000470: 2074 7261 6e73 666f 726d 0a64 6174 6120   transform.data 
+00000480: 696e 2074 6865 6972 2077 6172 6568 6f75  in their warehou
+00000490: 7365 7320 7369 6d70 6c79 2062 7920 7772  ses simply by wr
+000004a0: 6974 696e 6720 7365 6c65 6374 2073 7461  iting select sta
+000004b0: 7465 6d65 6e74 732e 2060 6462 7460 2070  tements. `dbt` p
+000004c0: 6572 666f 726d 7320 7468 6520 5420 2854  erforms the T (T
+000004d0: 7261 6e73 666f 726d 2920 6f66 2045 544c  ransform) of ETL
+000004e0: 2061 6e64 0a61 6c6c 6f77 7320 636f 6d70   and.allows comp
+000004f0: 616e 6965 7320 746f 2077 7269 7465 2074  anies to write t
+00000500: 7261 6e73 666f 726d 6174 696f 6e73 2061  ransformations a
+00000510: 7320 7175 6572 6965 7320 616e 6420 6f72  s queries and or
+00000520: 6368 6573 7472 6174 6520 7468 656d 2069  chestrate them i
+00000530: 6e20 6120 6d6f 7265 2065 6666 6963 6965  n a more efficie
+00000540: 6e74 2077 6179 2e20 0a42 7974 6548 6f75  nt way. .ByteHou
+00000550: 7365 2064 6274 2063 6f6e 6e65 6374 6f72  se dbt connector
+00000560: 2069 7320 6120 706c 7567 696e 2065 6e61   is a plugin ena
+00000570: 626c 696e 6720 7573 6572 7320 746f 2062  bling users to b
+00000580: 7569 6c64 2074 6865 6972 2064 6174 6120  uild their data 
+00000590: 7761 7265 686f 7573 6520 6563 6f73 7973  warehouse ecosys
+000005a0: 7465 6d20 7769 7468 2064 6274 200a 616e  tem with dbt .an
+000005b0: 6420 4279 7465 486f 7573 652e 200a 2320  d ByteHouse. .# 
+000005c0: 5461 626c 6520 6f66 2043 6f6e 7465 6e74  Table of Content
+000005d0: 730a 2d20 5b49 6e74 726f 6475 6374 696f  s.- [Introductio
+000005e0: 6e5d 2823 696e 7472 6f64 7563 7469 6f6e  n](#introduction
+000005f0: 290a 2d20 5b52 6571 7569 7265 6d65 6e74  ).- [Requirement
+00000600: 735d 2823 7265 7175 6972 656d 656e 7473  s](#requirements
+00000610: 290a 2d20 5b43 7265 6174 696e 6720 4279  ).- [Creating By
+00000620: 7465 486f 7573 6520 4163 636f 756e 745d  teHouse Account]
+00000630: 2823 6372 6561 7469 6e67 2d62 7974 6568  (#creating-byteh
+00000640: 6f75 7365 2d61 6363 6f75 6e74 290a 2d20  ouse-account).- 
+00000650: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2823  [Installation](#
+00000660: 696e 7374 616c 6c61 7469 6f6e 290a 2d20  installation).- 
+00000670: 5b64 6274 2050 726f 6a65 6374 2053 6574  [dbt Project Set
+00000680: 7570 5d28 2364 6274 2d70 726f 6a65 6374  up](#dbt-project
+00000690: 2d73 6574 7570 290a 2020 2a20 5b64 6274  -setup).  * [dbt
+000006a0: 5f70 726f 6a65 6374 2e79 6d6c 5d28 2364  _project.yml](#d
+000006b0: 6274 2d70 726f 6a65 6374 796d 6c29 0a20  bt-projectyml). 
+000006c0: 202a 205b 7072 6f66 696c 6573 2e79 6d6c   * [profiles.yml
+000006d0: 5d28 2370 726f 6669 6c65 7379 6d6c 290a  ](#profilesyml).
+000006e0: 2020 2a20 5b43 6f6e 6e65 6374 696f 6e20    * [Connection 
+000006f0: 2620 4175 7468 656e 7469 6361 7469 6f6e  & Authentication
+00000700: 2043 6f6e 6669 6775 7261 7469 6f6e 735d   Configurations]
+00000710: 2823 636f 6e6e 6563 7469 6f6e 2d2d 2d61  (#connection---a
+00000720: 7574 6865 6e74 6963 6174 696f 6e2d 636f  uthentication-co
+00000730: 6e66 6967 7572 6174 696f 6e73 290a 2020  nfigurations).  
+00000740: 2020 2b20 5b42 7974 6548 6f75 7365 2052    + [ByteHouse R
+00000750: 6567 696f 6e73 5d28 2362 7974 6568 6f75  egions](#bytehou
+00000760: 7365 2d72 6567 696f 6e73 290a 2020 2020  se-regions).    
+00000770: 2b20 5b52 6567 696f 6e20 2620 5061 7373  + [Region & Pass
+00000780: 776f 7264 2043 6f6e 6669 6775 7261 7469  word Configurati
+00000790: 6f6e 5d28 2372 6567 696f 6e2d 2d2d 7061  on](#region---pa
+000007a0: 7373 776f 7264 2d63 6f6e 6669 6775 7261  ssword-configura
+000007b0: 7469 6f6e 290a 2020 2020 2b20 5b52 6567  tion).    + [Reg
+000007c0: 696f 6e20 2620 4150 4920 4b65 7920 436f  ion & API Key Co
+000007d0: 6e66 6967 7572 6174 696f 6e5d 2823 7265  nfiguration](#re
+000007e0: 6769 6f6e 2d2d 2d61 7069 2d6b 6579 2d63  gion---api-key-c
+000007f0: 6f6e 6669 6775 7261 7469 6f6e 290a 2020  onfiguration).  
+00000800: 2020 2b20 5b48 6f73 7420 4164 6472 6573    + [Host Addres
+00000810: 7320 2620 5061 7373 776f 7264 2043 6f6e  s & Password Con
+00000820: 6669 6775 7261 7469 6f6e 5d28 2368 6f73  figuration](#hos
+00000830: 742d 6164 6472 6573 732d 2d2d 7061 7373  t-address---pass
+00000840: 776f 7264 2d63 6f6e 6669 6775 7261 7469  word-configurati
+00000850: 6f6e 290a 2020 2020 2b20 5b48 6f73 7420  on).    + [Host 
+00000860: 4164 6472 6573 7320 2620 4150 4920 4b65  Address & API Ke
+00000870: 7920 436f 6e66 6967 7572 6174 696f 6e5d  y Configuration]
+00000880: 2823 686f 7374 2d61 6464 7265 7373 2d2d  (#host-address--
+00000890: 2d61 7069 2d6b 6579 2d63 6f6e 6669 6775  -api-key-configu
+000008a0: 7261 7469 6f6e 290a 2020 2a20 5b50 726f  ration).  * [Pro
+000008b0: 6a65 6374 2049 6e69 7469 616c 697a 6174  ject Initializat
+000008c0: 696f 6e5d 2823 7072 6f6a 6563 742d 696e  ion](#project-in
+000008d0: 6974 6961 6c69 7a61 7469 6f6e 290a 2020  itialization).  
+000008e0: 2a20 5b54 6573 7420 5761 7265 686f 7573  * [Test Warehous
+000008f0: 6520 436f 6e6e 6563 7469 6f6e 5d28 2374  e Connection](#t
+00000900: 6573 742d 7761 7265 686f 7573 652d 636f  est-warehouse-co
+00000910: 6e6e 6563 7469 6f6e 290a 2d20 5b44 6174  nnection).- [Dat
+00000920: 6173 6574 2049 6e67 6573 7469 6f6e 5d28  aset Ingestion](
+00000930: 2364 6174 6173 6574 2d69 6e67 6573 7469  #dataset-ingesti
+00000940: 6f6e 290a 2d20 5b64 6274 204d 6f64 656c  on).- [dbt Model
+00000950: 735d 2823 6462 742d 6d6f 6465 6c73 290a  s](#dbt-models).
+00000960: 2d20 5b73 6368 656d 612e 796d 6c5d 2823  - [schema.yml](#
+00000970: 7363 6865 6d61 796d 6c29 0a2d 205b 4d61  schemayml).- [Ma
+00000980: 7465 7269 616c 697a 6174 696f 6e20 7479  terialization ty
+00000990: 7065 7320 6f66 204d 6f64 656c 735d 2823  pes of Models](#
+000009a0: 6d61 7465 7269 616c 697a 6174 696f 6e2d  materialization-
+000009b0: 7479 7065 732d 6f66 2d6d 6f64 656c 7329  types-of-models)
+000009c0: 0a20 202a 205b 5669 6577 204d 6174 6572  .  * [View Mater
+000009d0: 6961 6c69 7a61 7469 6f6e 735d 2823 7669  ializations](#vi
+000009e0: 6577 2d6d 6174 6572 6961 6c69 7a61 7469  ew-materializati
+000009f0: 6f6e 7329 0a20 202a 205b 5461 626c 6520  ons).  * [Table 
+00000a00: 4d61 7465 7269 616c 697a 6174 696f 6e73  Materializations
+00000a10: 5d28 2374 6162 6c65 2d6d 6174 6572 6961  ](#table-materia
+00000a20: 6c69 7a61 7469 6f6e 7329 0a20 202a 205b  lizations).  * [
+00000a30: 496e 6372 656d 656e 7461 6c20 4d61 7465  Incremental Mate
+00000a40: 7269 616c 697a 6174 696f 6e73 5d28 2369  rializations](#i
+00000a50: 6e63 7265 6d65 6e74 616c 2d6d 6174 6572  ncremental-mater
+00000a60: 6961 6c69 7a61 7469 6f6e 7329 0a20 2020  ializations).   
+00000a70: 202b 205b 486f 7720 6974 2077 6f72 6b73   + [How it works
+00000a80: 5d28 2368 6f77 2d69 742d 776f 726b 7329  ](#how-it-works)
+00000a90: 0a2d 205b 5072 6f6a 6563 7420 446f 6375  .- [Project Docu
+00000aa0: 6d65 6e74 6174 696f 6e5d 2823 7072 6f6a  mentation](#proj
+00000ab0: 6563 742d 646f 6375 6d65 6e74 6174 696f  ect-documentatio
+00000ac0: 6e29 0a2d 205b 4c6f 6361 6c20 4465 7665  n).- [Local Deve
+00000ad0: 6c6f 706d 656e 745d 2823 6c6f 6361 6c2d  lopment](#local-
+00000ae0: 6465 7665 6c6f 706d 656e 7429 0a2d 205b  development).- [
+00000af0: 4f72 6967 696e 616c 2041 7574 686f 725d  Original Author]
+00000b00: 2823 6f72 6967 696e 616c 2d61 7574 686f  (#original-autho
+00000b10: 7229 0a2d 205b 4c69 6365 6e73 655d 2823  r).- [License](#
+00000b20: 6c69 6365 6e73 6529 0a23 2052 6571 7569  license).# Requi
+00000b30: 7265 6d65 6e74 730a 4d61 6b65 2073 7572  rements.Make sur
+00000b40: 6520 796f 7520 6861 7665 2060 6462 7460  e you have `dbt`
+00000b50: 2026 2060 7079 7468 6f6e 6020 696e 7374   & `python` inst
+00000b60: 616c 6c65 6420 6f6e 2079 6f75 7220 6d61  alled on your ma
+00000b70: 6368 696e 652e 2049 6620 6e6f 742c 2074  chine. If not, t
+00000b80: 6865 6e20 796f 7520 6361 6e20 666f 6c6c  hen you can foll
+00000b90: 6f77 2074 6869 7320 6775 6964 6520 6874  ow this guide ht
+00000ba0: 7470 733a 2f2f 646f 6373 2e67 6574 6462  tps://docs.getdb
+00000bb0: 742e 636f 6d2f 646f 6373 2f67 6574 2d73  t.com/docs/get-s
+00000bc0: 7461 7274 6564 2f69 6e73 7461 6c6c 6174  tarted/installat
+00000bd0: 696f 6e0a 2d20 6462 7420 7631 2e37 2e30  ion.- dbt v1.7.0
+00000be0: 206f 7220 6772 6561 7465 720a 2d20 7079   or greater.- py
+00000bf0: 7468 6f6e 2076 332e 3720 6f72 2067 7265  thon v3.7 or gre
+00000c00: 6174 6572 0a23 2043 7265 6174 696e 6720  ater.# Creating 
+00000c10: 4279 7465 486f 7573 6520 4163 636f 756e  ByteHouse Accoun
+00000c20: 740a 596f 7520 6e65 6564 2074 6f20 6372  t.You need to cr
+00000c30: 6561 7465 2042 7974 6548 6f75 7365 2061  eate ByteHouse a
+00000c40: 6363 6f75 6e74 2069 6e20 6f72 6465 7220  ccount in order 
+00000c50: 746f 2075 7365 2062 7974 6568 6f75 7365  to use bytehouse
+00000c60: 2d64 6274 2063 6f6e 6e65 6374 6f72 2e20  -dbt connector. 
+00000c70: 596f 7520 6361 6e20 7369 6d70 6c79 2063  You can simply c
+00000c80: 7265 6174 6520 6120 6672 6565 2061 6363  reate a free acc
+00000c90: 6f75 6e74 2077 6974 680a 7468 6520 7072  ount with.the pr
+00000ca0: 6f63 6573 7320 6d65 6e74 696f 6e65 6420  ocess mentioned 
+00000cb0: 696e 206f 7572 206f 6666 6963 6961 6c20  in our official 
+00000cc0: 7765 6273 6974 6520 646f 6375 6d65 6e74  website document
+00000cd0: 6174 696f 6e3a 2068 7474 7073 3a2f 2f64  ation: https://d
+00000ce0: 6f63 732e 6279 7465 686f 7573 652e 636c  ocs.bytehouse.cl
+00000cf0: 6f75 642f 656e 2f64 6f63 732f 7175 6963  oud/en/docs/quic
+00000d00: 6b2d 7374 6172 7420 3c62 722f 3e0a 0a59  k-start <br/>..Y
+00000d10: 6f75 2063 616e 2061 6c73 6f20 6372 6561  ou can also crea
+00000d20: 7465 2042 7974 6548 6f75 7365 2061 6363  te ByteHouse acc
+00000d30: 6f75 6e74 2074 6872 6f75 6768 2056 6f6c  ount through Vol
+00000d40: 6361 6e6f 2045 6e67 696e 6520 6279 2042  cano Engine by B
+00000d50: 7974 6544 616e 6365 3a20 0a68 7474 7073  yteDance: .https
+00000d60: 3a2f 2f77 7777 2e76 6f6c 6365 6e67 696e  ://www.volcengin
+00000d70: 652e 636f 6d2f 7072 6f64 7563 742f 6279  e.com/product/by
+00000d80: 7465 686f 7573 652d 636c 6f75 6420 0a23  tehouse-cloud .#
+00000d90: 2049 6e73 7461 6c6c 6174 696f 6e0a 4372   Installation.Cr
+00000da0: 6561 7465 2061 206e 6577 2072 6570 6f73  eate a new repos
+00000db0: 6974 6f72 7920 7768 6572 6520 7765 2077  itory where we w
+00000dc0: 696c 6c20 696e 7374 616e 7469 6174 6520  ill instantiate 
+00000dd0: 6120 6050 7974 686f 6e60 2076 6972 7475  a `Python` virtu
+00000de0: 616c 2065 6e76 6972 6f6e 6d65 6e74 2e0a  al environment..
+00000df0: 6060 6063 6f6d 6d61 6e64 6c69 6e65 0a6d  ```commandline.m
+00000e00: 6b64 6972 2064 6274 5f62 7974 6568 6f75  kdir dbt_bytehou
+00000e10: 7365 5f64 656d 6f0a 6364 2064 6274 5f62  se_demo.cd dbt_b
+00000e20: 7974 6568 6f75 7365 5f64 656d 6f0a 0a70  ytehouse_demo..p
+00000e30: 7974 686f 6e20 2d6d 2076 656e 7620 7665  ython -m venv ve
+00000e40: 6e76 0a73 6f75 7263 6520 7665 6e76 2f62  nv.source venv/b
+00000e50: 696e 2f61 6374 6976 6174 650a 6060 600a  in/activate.```.
+00000e60: 4c61 7465 7374 2072 656c 6561 7365 2076  Latest release v
+00000e70: 6572 7369 6f6e 2063 616e 2062 6520 696e  ersion can be in
+00000e80: 7374 616c 6c65 6420 6672 6f6d 2068 6572  stalled from her
+00000e90: 653a 0a60 6060 636f 6d6d 616e 646c 696e  e:.```commandlin
+00000ea0: 650a 7069 7020 696e 7374 616c 6c20 6462  e.pip install db
+00000eb0: 742d 6279 7465 686f 7573 650a 6060 600a  t-bytehouse.```.
+00000ec0: 4375 7272 656e 7420 6465 7665 6c6f 706d  Current developm
+00000ed0: 656e 7420 7665 7273 696f 6e20 6361 6e20  ent version can 
+00000ee0: 6265 2069 6e73 7461 6c6c 6564 2066 726f  be installed fro
+00000ef0: 6d20 6865 7265 3a0a 6060 6063 6f6d 6d61  m here:.```comma
+00000f00: 6e64 6c69 6e65 0a70 6970 2069 6e73 7461  ndline.pip insta
+00000f10: 6c6c 2067 6974 2b68 7474 7073 3a2f 2f67  ll git+https://g
+00000f20: 6974 6875 622e 636f 6d2f 6279 7465 686f  ithub.com/byteho
+00000f30: 7573 652d 636c 6f75 642f 6279 7465 686f  use-cloud/byteho
+00000f40: 7573 652d 6462 7440 6d61 7374 6572 2365  use-dbt@master#e
+00000f50: 6767 3d62 7974 6568 6f75 7365 2d64 7269  gg=bytehouse-dri
+00000f60: 7665 720a 6060 600a 4368 6563 6b20 7768  ver.```.Check wh
+00000f70: 6574 6865 7220 696e 7374 616c 6c61 7469  ether installati
+00000f80: 6f6e 2069 7320 7375 6363 6573 7366 756c  on is successful
+00000f90: 2062 7920 7665 7269 6679 696e 6720 6279   by verifying by
+00000fa0: 7465 686f 7573 6520 6973 2061 7661 696c  tehouse is avail
+00000fb0: 6162 6c65 2075 6e64 6572 2050 6c75 6769  able under Plugi
+00000fc0: 6e73 2e0a 6060 6063 6f6d 6d61 6e64 6c69  ns..```commandli
+00000fd0: 6e65 0a64 6274 202d 2d76 6572 7369 6f6e  ne.dbt --version
+00000fe0: 0a60 6060 0a21 5b56 6572 7369 6f6e 5d28  .```.![Version](
+00000ff0: 2e2f 6578 616d 706c 6573 2f31 5f76 6572  ./examples/1_ver
+00001000: 7369 6f6e 2e70 6e67 290a 2320 6462 7420  sion.png).# dbt 
+00001010: 5072 6f6a 6563 7420 5365 7475 700a 2323  Project Setup.##
+00001020: 2064 6274 5f70 726f 6a65 6374 2e79 6d6c   dbt_project.yml
+00001030: 0a45 7665 7279 2060 6462 7460 2070 726f  .Every `dbt` pro
+00001040: 6a65 6374 206e 6565 6473 2061 2060 6462  ject needs a `db
+00001050: 745f 7072 6f6a 6563 742e 796d 6c60 2066  t_project.yml` f
+00001060: 696c 6520 e280 9420 7468 6973 2069 7320  ile ... this is 
+00001070: 686f 7720 6064 6274 6020 6b6e 6f77 7320  how `dbt` knows 
+00001080: 6120 6469 7265 6374 6f72 7920 6973 2061  a directory is a
+00001090: 2060 6462 7460 2070 726f 6a65 6374 2e20   `dbt` project. 
+000010a0: 6064 6274 5f70 726f 6a65 6374 2e79 6d6c  `dbt_project.yml
+000010b0: 600a 6669 6c65 2068 6f6c 6473 2074 6865  `.file holds the
+000010c0: 2063 6f6e 7465 7874 206f 6620 796f 7572   context of your
+000010d0: 2070 726f 6a65 6374 2061 6e64 2074 656c   project and tel
+000010e0: 6c73 2060 6462 7460 2068 6f77 2074 6f20  ls `dbt` how to 
+000010f0: 6275 696c 6420 796f 7572 2064 6174 6120  build your data 
+00001100: 7365 7473 2e20 536f 6d65 2063 6f6d 6d6f  sets. Some commo
+00001110: 6e20 636f 6e66 6967 7572 6174 696f 6e73  n configurations
+00001120: 0a66 6f72 2060 6462 745f 7072 6f6a 6563  .for `dbt_projec
+00001130: 742e 796d 6c60 2061 7265 3a0a 3c74 6162  t.yml` are:.<tab
+00001140: 6c65 3e0a 2020 2020 3c74 723e 0a20 2020  le>.    <tr>.   
+00001150: 2020 2020 203c 7464 3e59 414d 4c20 6b65       <td>YAML ke
+00001160: 793c 2f74 643e 0a20 2020 2020 2020 203c  y</td>.        <
+00001170: 7464 3e56 616c 7565 3c2f 7464 3e0a 2020  td>Value</td>.  
+00001180: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+00001190: 0a20 2020 2020 2020 203c 7464 3e6e 616d  .        <td>nam
+000011a0: 653c 2f74 643e 0a20 2020 2020 2020 203c  e</td>.        <
+000011b0: 7464 3e59 6f75 7220 7072 6f6a 6563 74e2  td>Your project.
+000011c0: 8099 7320 6e61 6d65 2069 6e20 736e 616b  ..s name in snak
+000011d0: 6520 6361 7365 3c2f 7464 3e0a 2020 2020  e case</td>.    
+000011e0: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+000011f0: 2020 2020 2020 203c 7464 3e76 6572 7369         <td>versi
+00001200: 6f6e 3c2f 7464 3e0a 2020 2020 2020 2020  on</td>.        
+00001210: 3c74 643e 5665 7273 696f 6e20 6f66 2079  <td>Version of y
+00001220: 6f75 7220 7072 6f6a 6563 743c 2f74 643e  our project</td>
+00001230: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+00001240: 7472 3e0a 2020 2020 2020 2020 3c74 643e  tr>.        <td>
+00001250: 7072 6f66 696c 653c 2f74 643e 0a20 2020  profile</td>.   
+00001260: 2020 2020 203c 7464 3e54 6865 2070 726f       <td>The pro
+00001270: 6669 6c65 2064 6274 2075 7365 7320 746f  file dbt uses to
+00001280: 2063 6f6e 6e65 6374 2074 6f20 4279 7465   connect to Byte
+00001290: 486f 7573 653c 2f74 643e 0a20 2020 203c  House</td>.    <
+000012a0: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
+000012b0: 2020 2020 2020 3c74 643e 6d6f 6465 6c2d        <td>model-
+000012c0: 7061 7468 733c 2f74 643e 0a20 2020 2020  paths</td>.     
+000012d0: 2020 203c 7464 3e44 6972 6563 746f 7269     <td>Directori
+000012e0: 6573 2074 6f20 7768 6572 6520 796f 7572  es to where your
+000012f0: 206d 6f64 656c 2061 6e64 2073 6f75 7263   model and sourc
+00001300: 6520 6669 6c65 7320 6c69 7665 3c2f 7464  e files live</td
+00001310: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+00001320: 3c74 723e 0a20 2020 2020 2020 203c 7464  <tr>.        <td
+00001330: 3e73 6565 642d 7061 7468 733c 2f74 643e  >seed-paths</td>
+00001340: 0a20 2020 2020 2020 203c 7464 3e44 6972  .        <td>Dir
+00001350: 6563 746f 7269 6573 2074 6f20 7768 6572  ectories to wher
+00001360: 6520 796f 7572 2073 6565 6420 6669 6c65  e your seed file
+00001370: 7320 6c69 7665 3c2f 7464 3e0a 2020 2020  s live</td>.    
+00001380: 3c2f 7472 3e0a 2020 2020 3c74 723e 0a20  </tr>.    <tr>. 
+00001390: 2020 2020 2020 203c 7464 3e74 6573 742d         <td>test-
+000013a0: 7061 7468 733c 2f74 643e 0a20 2020 2020  paths</td>.     
+000013b0: 2020 203c 7464 3e44 6972 6563 746f 7269     <td>Directori
+000013c0: 6573 2074 6f20 7768 6572 6520 796f 7572  es to where your
+000013d0: 2074 6573 7420 6669 6c65 7320 6c69 7665   test files live
+000013e0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000013f0: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+00001400: 203c 7464 3e73 6e61 7073 686f 742d 7061   <td>snapshot-pa
+00001410: 7468 733c 2f74 643e 0a20 2020 2020 2020  ths</td>.       
+00001420: 203c 7464 3e44 6972 6563 746f 7269 6573   <td>Directories
+00001430: 2074 6f20 7768 6572 6520 796f 7572 2073   to where your s
+00001440: 6e61 7073 686f 7473 206c 6976 653c 2f74  napshots live</t
+00001450: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+00001460: 203c 7472 3e0a 2020 2020 2020 2020 3c74   <tr>.        <t
+00001470: 643e 646f 6373 2d70 6174 6873 3c2f 7464  d>docs-paths</td
+00001480: 3e0a 2020 2020 2020 2020 3c74 643e 4469  >.        <td>Di
+00001490: 7265 6374 6f72 6965 7320 746f 2077 6865  rectories to whe
+000014a0: 7265 2079 6f75 7220 646f 6373 2062 6c6f  re your docs blo
+000014b0: 636b 7320 6c69 7665 3c2f 7464 3e0a 2020  cks live</td>.  
+000014c0: 2020 3c2f 7472 3e0a 3c2f 7461 626c 653e    </tr>.</table>
+000014d0: 0a0a 2323 2070 726f 6669 6c65 732e 796d  ..## profiles.ym
+000014e0: 6c0a 5768 656e 2079 6f75 2069 6e76 6f6b  l.When you invok
+000014f0: 6520 6064 6274 6020 6672 6f6d 2074 6865  e `dbt` from the
+00001500: 2063 6f6d 6d61 6e64 206c 696e 652c 2060   command line, `
+00001510: 6462 7460 2070 6172 7365 7320 796f 7572  dbt` parses your
+00001520: 2060 6462 745f 7072 6f6a 6563 742e 796d   `dbt_project.ym
+00001530: 6c60 2061 6e64 206f 6274 6169 6e73 2074  l` and obtains t
+00001540: 6865 2070 726f 6669 6c65 206e 616d 652e  he profile name.
+00001550: 2060 6462 7460 2074 6865 6e20 0a63 6865   `dbt` then .che
+00001560: 636b 7320 796f 7572 2060 7072 6f66 696c  cks your `profil
+00001570: 6573 2e79 6d6c 6020 6669 6c65 2066 6f72  es.yml` file for
+00001580: 2061 2070 726f 6669 6c65 2077 6974 6820   a profile with 
+00001590: 7468 6520 7361 6d65 206e 616d 652e 2041  the same name. A
+000015a0: 2070 726f 6669 6c65 2063 6f6e 7461 696e   profile contain
+000015b0: 7320 616c 6c20 7468 6520 6465 7461 696c  s all the detail
+000015c0: 732f 6372 6564 656e 7469 616c 7320 0a72  s/credentials .r
+000015d0: 6571 7569 7265 6420 746f 2063 6f6e 6e65  equired to conne
+000015e0: 6374 2074 6f20 4279 7465 486f 7573 652e  ct to ByteHouse.
+000015f0: 2060 6462 7460 2077 696c 6c20 7365 6172   `dbt` will sear
+00001600: 6368 2074 6865 2063 7572 7265 6e74 2077  ch the current w
+00001610: 6f72 6b69 6e67 2064 6972 6563 746f 7279  orking directory
+00001620: 2066 6f72 2074 6865 2060 7072 6f66 696c   for the `profil
+00001630: 6573 2e79 6d6c 6020 6669 6c65 2061 6e64  es.yml` file and
+00001640: 2077 696c 6c0a 6465 6661 756c 7420 746f   will.default to
+00001650: 2074 6865 2060 7e2f 2e64 6274 2f20 6469   the `~/.dbt/ di
+00001660: 7265 6374 6f72 7960 2069 6620 6e6f 7420  rectory` if not 
+00001670: 666f 756e 642e 0a60 6060 7961 6d6c 0a3c  found..```yaml.<
+00001680: 7072 6f66 696c 652d 6e61 6d65 3e3a 0a20  profile-name>:. 
+00001690: 2074 6172 6765 743a 203c 7461 7267 6574   target: <target
+000016a0: 2d6e 616d 653e 0a20 206f 7574 7075 7473  -name>.  outputs
+000016b0: 3a0a 2020 2020 3c74 6172 6765 742d 6e61  :.    <target-na
+000016c0: 6d65 3e3a 0a20 2020 2020 2074 7970 653a  me>:.      type:
+000016d0: 2062 7974 6568 6f75 7365 0a20 2020 2020   bytehouse.     
+000016e0: 2073 6368 656d 613a 203c 6461 7461 6261   schema: <databa
+000016f0: 7365 2d6e 616d 653e 0a20 2020 2020 2075  se-name>.      u
+00001700: 7365 723a 2062 7974 6568 6f75 7365 0a20  ser: bytehouse. 
+00001710: 2020 2020 2070 6173 7377 6f72 643a 203c       password: <
+00001720: 6279 7465 686f 7573 652d 6170 692d 6b65  bytehouse-api-ke
+00001730: 793e 0a20 2020 2020 2064 7269 7665 723a  y>.      driver:
+00001740: 206e 6174 6976 650a 2020 2020 2020 236f   native.      #o
+00001750: 7074 696f 6e61 6c20 6669 656c 6473 0a20  ptional fields. 
+00001760: 2020 2020 2068 6f73 743a 203c 686f 7374       host: <host
+00001770: 6e61 6d65 3e0a 2020 2020 2020 706f 7274  name>.      port
+00001780: 3a20 3c70 6f72 743e 0a20 2020 2020 2072  : <port>.      r
+00001790: 6567 696f 6e3a 203c 7265 6769 6f6e 2d6e  egion: <region-n
+000017a0: 616d 653e 0a20 2020 2020 2077 6172 6568  ame>.      wareh
+000017b0: 6f75 7365 3a20 3c77 6172 6568 6f75 7365  ouse: <warehouse
+000017c0: 2d6e 616d 653e 0a20 2020 2020 2072 6574  -name>.      ret
+000017d0: 7269 6573 3a20 310a 2020 2020 2020 7365  ries: 1.      se
+000017e0: 6375 7265 3a20 5472 7565 0a20 2020 2020  cure: True.     
+000017f0: 2063 6f6e 6e65 6374 5f74 696d 656f 7574   connect_timeout
+00001800: 3a20 3130 0a20 2020 2020 2073 656e 645f  : 10.      send_
+00001810: 7265 6365 6976 655f 7469 6d65 6f75 743a  receive_timeout:
+00001820: 2033 3030 0a20 2020 2020 2063 7573 746f   300.      custo
+00001830: 6d5f 7365 7474 696e 6773 3a20 3c65 6d70  m_settings: <emp
+00001840: 7479 3e0a 6060 600a 3c74 6162 6c65 3e0a  ty>.```.<table>.
+00001850: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+00001860: 203c 7464 3e59 414d 4c20 6b65 793c 2f74   <td>YAML key</t
+00001870: 643e 0a20 2020 2020 2020 203c 7464 3e56  d>.        <td>V
+00001880: 616c 7565 3c2f 7464 3e0a 2020 2020 3c2f  alue</td>.    </
+00001890: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+000018a0: 2020 2020 203c 7464 3e26 6c74 3b70 726f       <td>&lt;pro
+000018b0: 6669 6c65 2d6e 616d 6526 6774 3b3c 2f74  file-name&gt;</t
+000018c0: 643e 0a20 2020 2020 2020 203c 7464 3e4e  d>.        <td>N
+000018d0: 616d 6520 6f66 2074 6865 2070 726f 6669  ame of the profi
+000018e0: 6c65 2e20 4861 7320 746f 2062 6520 7468  le. Has to be th
+000018f0: 6520 7361 6d65 206e 616d 6520 6173 2074  e same name as t
+00001900: 6865 2070 726f 6669 6c65 2069 6e64 6963  he profile indic
+00001910: 6174 6564 2069 6e20 796f 7572 2064 6274  ated in your dbt
+00001920: 5f70 726f 6a65 6374 2e79 6d6c 2066 696c  _project.yml fil
+00001930: 653c 2f74 643e 0a20 2020 203c 2f74 723e  e</td>.    </tr>
+00001940: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+00001950: 2020 3c74 643e 7461 7267 6574 3c2f 7464    <td>target</td
+00001960: 3e0a 2020 2020 2020 2020 3c74 643e 4465  >.        <td>De
+00001970: 6661 756c 7420 7461 7267 6574 2079 6f75  fault target you
+00001980: 7220 6462 7420 7072 6f6a 6563 7420 7769  r dbt project wi
+00001990: 6c6c 2075 7365 2e20 4974 206d 7573 7420  ll use. It must 
+000019a0: 6265 206f 6e65 206f 6620 7468 6520 7461  be one of the ta
+000019b0: 7267 6574 7320 796f 7520 6465 6669 6e65  rgets you define
+000019c0: 2069 6e20 796f 7572 2070 726f 6669 6c65   in your profile
+000019d0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000019e0: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+000019f0: 203c 7464 3e74 7970 653c 2f74 643e 0a20   <td>type</td>. 
+00001a00: 2020 2020 2020 203c 7464 3e4d 7573 7420         <td>Must 
+00001a10: 6265 2073 6574 2074 6f20 6279 7465 686f  be set to byteho
+00001a20: 7573 653c 2f74 643e 0a20 2020 203c 2f74  use</td>.    </t
+00001a30: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+00001a40: 2020 2020 3c74 643e 7363 6865 6d61 3c2f      <td>schema</
+00001a50: 7464 3e0a 2020 2020 2020 2020 3c74 643e  td>.        <td>
+00001a60: 4461 7461 6261 7365 206e 616d 653c 2f74  Database name</t
+00001a70: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+00001a80: 203c 7472 3e0a 2020 2020 2020 2020 3c74   <tr>.        <t
+00001a90: 643e 7573 6572 3c2f 7464 3e0a 2020 2020  d>user</td>.    
+00001aa0: 2020 2020 3c74 643e 4d75 7374 2062 6520      <td>Must be 
+00001ab0: 7365 7420 746f 2062 7974 6568 6f75 7365  set to bytehouse
 00001ac0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
 00001ad0: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
-00001ae0: 203c 7464 3e73 6563 7572 653c 2f74 643e   <td>secure</td>
-00001af0: 0a20 2020 2020 2020 203c 7464 3e5b 4f70  .        <td>[Op
-00001b00: 7469 6f6e 616c 5d20 5768 6574 6865 7220  tional] Whether 
-00001b10: 7468 6520 636f 6e6e 6563 7469 6f6e 2069  the connection i
-00001b20: 7320 7365 6375 7265 6420 6279 2054 4c53  s secured by TLS
-00001b30: 2e20 5375 6767 6573 7465 6420 746f 2073  . Suggested to s
-00001b40: 6574 2069 7420 746f 2054 7275 653c 2f74  et it to True</t
-00001b50: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
-00001b60: 203c 7472 3e0a 2020 2020 2020 2020 3c74   <tr>.        <t
-00001b70: 643e 636f 6e6e 6563 745f 7469 6d65 6f75  d>connect_timeou
-00001b80: 743c 2f74 643e 0a20 2020 2020 2020 203c  t</td>.        <
-00001b90: 7464 3e5b 4f70 7469 6f6e 616c 5d20 436f  td>[Optional] Co
-00001ba0: 6e6e 6563 7469 6f6e 2074 696d 656f 7574  nnection timeout
-00001bb0: 2069 6e20 7365 636f 6e64 732e 2044 6566   in seconds. Def
-00001bc0: 6175 6c74 2069 7320 3130 2073 6563 6f6e  ault is 10 secon
-00001bd0: 6473 3c2f 7464 3e0a 2020 2020 3c2f 7472  ds</td>.    </tr
-00001be0: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00001bf0: 2020 203c 7464 3e73 656e 645f 7265 6365     <td>send_rece
-00001c00: 6976 655f 7469 6d65 6f75 743c 2f74 643e  ive_timeout</td>
-00001c10: 0a20 2020 2020 2020 203c 7464 3e5b 4f70  .        <td>[Op
-00001c20: 7469 6f6e 616c 5d20 5469 6d65 6f75 7420  tional] Timeout 
-00001c30: 666f 7220 7265 6365 6976 696e 6720 6461  for receiving da
-00001c40: 7461 2066 726f 6d20 6f72 2073 656e 6469  ta from or sendi
-00001c50: 6e67 2064 6174 6120 746f 2042 7974 6548  ng data to ByteH
-00001c60: 6f75 7365 2e20 4465 6661 756c 7420 6973  ouse. Default is
-00001c70: 2035 206d 696e 7574 6573 2028 3330 3020   5 minutes (300 
-00001c80: 7365 636f 6e64 7329 3c2f 7464 3e0a 2020  seconds)</td>.  
-00001c90: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
-00001ca0: 0a20 2020 2020 2020 203c 7464 3e63 7573  .        <td>cus
-00001cb0: 746f 6d5f 7365 7474 696e 6773 3c2f 7464  tom_settings</td
-00001cc0: 3e0a 2020 2020 2020 2020 3c74 643e 5b4f  >.        <td>[O
-00001cd0: 7074 696f 6e61 6c5d 2041 206d 6170 7069  ptional] A mappi
-00001ce0: 6e67 206f 6620 4279 7465 486f 7573 6520  ng of ByteHouse 
-00001cf0: 7370 6563 6966 6963 2075 7365 7220 7365  specific user se
-00001d00: 7474 696e 6773 2074 6f20 7573 6520 7769  ttings to use wi
-00001d10: 7468 2074 6865 2063 6f6e 6e65 6374 696f  th the connectio
-00001d20: 6e3c 2f74 643e 0a20 2020 203c 2f74 723e  n</td>.    </tr>
-00001d30: 0a3c 2f74 6162 6c65 3e0a 0a23 2320 436f  .</table>..## Co
-00001d40: 6e6e 6563 7469 6f6e 2026 2041 7574 6865  nnection & Authe
-00001d50: 6e74 6963 6174 696f 6e20 436f 6e66 6967  ntication Config
-00001d60: 7572 6174 696f 6e73 0a23 2323 2042 7974  urations.### Byt
-00001d70: 6548 6f75 7365 2052 6567 696f 6e73 0a43  eHouse Regions.C
-00001d80: 7572 7265 6e74 6c79 2c20 7468 6520 6472  urrently, the dr
-00001d90: 6976 6572 2073 7570 706f 7274 7320 7468  iver supports th
-00001da0: 6520 666f 6c6c 6f77 696e 6720 7265 6769  e following regi
-00001db0: 6f6e 206e 616d 6573 2061 6372 6f73 7320  on names across 
-00001dc0: 6469 6666 6572 656e 7420 636c 6f75 6420  different cloud 
-00001dd0: 7072 6f76 6964 6572 732e 2041 6c74 6572  providers. Alter
-00001de0: 6e61 7469 7665 6c79 2c20 6966 2079 6f75  natively, if you
-00001df0: 206b 6e6f 770a 7468 6520 686f 7374 2061   know.the host a
-00001e00: 6464 7265 7373 206f 6620 4279 7465 486f  ddress of ByteHo
-00001e10: 7573 6520 7365 7276 6572 2c20 796f 7520  use server, you 
-00001e20: 6361 6e20 6469 7265 6374 6c79 2075 7365  can directly use
-00001e30: 2068 6f73 7420 6164 6472 6573 7320 2620   host address & 
-00001e40: 6f6d 6974 2072 6567 696f 6e20 6e61 6d65  omit region name
-00001e50: 2e0a 3c74 6162 6c65 3e0a 2020 2020 3c74  ..<table>.    <t
-00001e60: 723e 0a20 2020 2020 2020 203c 7464 3e52  r>.        <td>R
-00001e70: 6567 696f 6e20 4e61 6d65 3c2f 7464 3e0a  egion Name</td>.
-00001e80: 2020 2020 2020 2020 3c74 643e 5461 7267          <td>Targ
-00001e90: 6574 2053 6572 7665 723c 2f74 643e 0a20  et Server</td>. 
-00001ea0: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
-00001eb0: 3e0a 2020 2020 2020 2020 3c74 643e 4150  >.        <td>AP
-00001ec0: 2d53 4f55 5448 4541 5354 2d31 3c2f 7464  -SOUTHEAST-1</td
-00001ed0: 3e0a 2020 2020 2020 2020 3c74 643e 6761  >.        <td>ga
-00001ee0: 7465 7761 792e 6177 732d 6170 2d73 6f75  teway.aws-ap-sou
-00001ef0: 7468 6561 7374 2d31 2e62 7974 6568 6f75  theast-1.bytehou
-00001f00: 7365 2e63 6c6f 7564 3a31 3930 3030 3c2f  se.cloud:19000</
-00001f10: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
-00001f20: 2020 3c74 723e 0a20 2020 2020 2020 203c    <tr>.        <
-00001f30: 7464 3e56 4f4c 4341 4e4f 2d43 4e2d 4e4f  td>VOLCANO-CN-NO
-00001f40: 5254 482d 313c 2f74 643e 0a20 2020 2020  RTH-1</td>.     
-00001f50: 2020 203c 7464 3e62 7974 6568 6f75 7365     <td>bytehouse
-00001f60: 2d63 6e2d 6265 696a 696e 672e 766f 6c63  -cn-beijing.volc
-00001f70: 6573 2e63 6f6d 3a31 3930 3030 3c2f 7464  es.com:19000</td
-00001f80: 3e0a 2020 2020 3c2f 7472 3e0a 3c2f 7461  >.    </tr>.</ta
-00001f90: 626c 653e 0a0a 2323 2320 5265 6769 6f6e  ble>..### Region
-00001fa0: 2026 2050 6173 7377 6f72 6420 436f 6e66   & Password Conf
-00001fb0: 6967 7572 6174 696f 6e0a 5265 7175 6972  iguration.Requir
-00001fc0: 6564 2070 6172 616d 6574 6572 733a 2060  ed parameters: `
-00001fd0: 6163 636f 756e 7460 2060 7573 6572 6020  account` `user` 
-00001fe0: 6070 6173 7377 6f72 6460 2060 7265 6769  `password` `regi
-00001ff0: 6f6e 600a 6060 6079 616d 6c0a 6279 7465  on`.```yaml.byte
-00002000: 686f 7573 655f 7072 6f66 696c 653a 0a20  house_profile:. 
-00002010: 2074 6172 6765 743a 2064 6576 0a20 206f   target: dev.  o
-00002020: 7574 7075 7473 3a0a 2020 2020 6465 763a  utputs:.    dev:
-00002030: 0a20 2020 2020 2074 7970 653a 2062 7974  .      type: byt
-00002040: 6568 6f75 7365 0a20 2020 2020 2064 7269  ehouse.      dri
-00002050: 7665 723a 206e 6174 6976 650a 0a20 2020  ver: native..   
-00002060: 2020 2023 2064 6174 6162 6173 650a 2020     # database.  
-00002070: 2020 2020 7363 6865 6d61 3a20 2444 4154      schema: $DAT
-00002080: 4142 4153 455f 4e41 4d45 0a0a 2020 2020  ABASE_NAME..    
-00002090: 2020 2320 7461 7267 6574 2073 6572 7665    # target serve
-000020a0: 7220 6164 6472 6573 730a 2020 2020 2020  r address.      
-000020b0: 7265 6769 6f6e 3a20 2452 4547 494f 4e5f  region: $REGION_
-000020c0: 4e41 4d45 0a0a 2020 2020 2020 2320 6163  NAME..      # ac
-000020d0: 636f 756e 7420 6372 6564 656e 7469 616c  count credential
-000020e0: 730a 2020 2020 2020 6163 636f 756e 743a  s.      account:
-000020f0: 2024 4143 434f 554e 545f 4e41 4d45 0a20   $ACCOUNT_NAME. 
-00002100: 2020 2020 2075 7365 723a 2024 5553 4552       user: $USER
-00002110: 5f4e 414d 450a 2020 2020 2020 7061 7373  _NAME.      pass
-00002120: 776f 7264 3a20 2450 4153 5357 4f52 440a  word: $PASSWORD.
-00002130: 0a20 2020 2020 2023 2061 6464 6974 696f  .      # additio
-00002140: 6e61 6c20 7365 7474 696e 6773 0a20 2020  nal settings.   
-00002150: 2020 2073 6563 7572 653a 2054 7275 650a     secure: True.
-00002160: 6060 600a 2323 2320 5265 6769 6f6e 2026  ```.### Region &
-00002170: 2041 5049 204b 6579 2043 6f6e 6669 6775   API Key Configu
-00002180: 7261 7469 6f6e 0a52 6571 7569 7265 6420  ration.Required 
-00002190: 7061 7261 6d65 7465 7273 3a20 6072 6567  parameters: `reg
-000021a0: 696f 6e60 2060 7573 6572 6020 6070 6173  ion` `user` `pas
-000021b0: 7377 6f72 6460 0a60 6060 7961 6d6c 0a62  sword`.```yaml.b
-000021c0: 7974 6568 6f75 7365 5f70 726f 6669 6c65  ytehouse_profile
-000021d0: 3a0a 2020 7461 7267 6574 3a20 6465 760a  :.  target: dev.
-000021e0: 2020 6f75 7470 7574 733a 0a20 2020 2064    outputs:.    d
-000021f0: 6576 3a0a 2020 2020 2020 7479 7065 3a20  ev:.      type: 
-00002200: 6279 7465 686f 7573 650a 2020 2020 2020  bytehouse.      
-00002210: 6472 6976 6572 3a20 6e61 7469 7665 0a0a  driver: native..
-00002220: 2020 2020 2020 2320 6461 7461 6261 7365        # database
-00002230: 0a20 2020 2020 2073 6368 656d 613a 2024  .      schema: $
-00002240: 4441 5441 4241 5345 5f4e 414d 450a 0a20  DATABASE_NAME.. 
-00002250: 2020 2020 2023 2074 6172 6765 7420 7365       # target se
-00002260: 7276 6572 2061 6464 7265 7373 0a20 2020  rver address.   
-00002270: 2020 2072 6567 696f 6e3a 2024 5245 4749     region: $REGI
-00002280: 4f4e 5f4e 414d 450a 0a20 2020 2020 2023  ON_NAME..      #
-00002290: 2061 6363 6f75 6e74 2063 7265 6465 6e74   account credent
-000022a0: 6961 6c73 0a20 2020 2020 2075 7365 723a  ials.      user:
-000022b0: 2062 7974 6568 6f75 7365 0a20 2020 2020   bytehouse.     
-000022c0: 2070 6173 7377 6f72 643a 2024 4150 495f   password: $API_
-000022d0: 4b45 590a 0a20 2020 2020 2023 2061 6464  KEY..      # add
-000022e0: 6974 696f 6e61 6c20 7365 7474 696e 6773  itional settings
-000022f0: 0a20 2020 2020 2073 6563 7572 653a 2054  .      secure: T
-00002300: 7275 650a 6060 600a 2323 2320 486f 7374  rue.```.### Host
-00002310: 2041 6464 7265 7373 2026 2050 6173 7377   Address & Passw
-00002320: 6f72 6420 436f 6e66 6967 7572 6174 696f  ord Configuratio
-00002330: 6e0a 5265 7175 6972 6564 2070 6172 616d  n.Required param
-00002340: 6574 6572 733a 2060 686f 7374 6020 6070  eters: `host` `p
-00002350: 6f72 7460 2060 6163 636f 756e 7460 2060  ort` `account` `
-00002360: 7573 6572 6020 6070 6173 7377 6f72 6460  user` `password`
-00002370: 0a60 6060 7961 6d6c 0a62 7974 6568 6f75  .```yaml.bytehou
-00002380: 7365 5f70 726f 6669 6c65 3a0a 2020 7461  se_profile:.  ta
-00002390: 7267 6574 3a20 6465 760a 2020 6f75 7470  rget: dev.  outp
-000023a0: 7574 733a 0a20 2020 2064 6576 3a0a 2020  uts:.    dev:.  
-000023b0: 2020 2020 7479 7065 3a20 6279 7465 686f      type: byteho
-000023c0: 7573 650a 2020 2020 2020 6472 6976 6572  use.      driver
-000023d0: 3a20 6e61 7469 7665 0a0a 2020 2020 2020  : native..      
-000023e0: 2320 6461 7461 6261 7365 0a20 2020 2020  # database.     
-000023f0: 2073 6368 656d 613a 2024 4441 5441 4241   schema: $DATABA
-00002400: 5345 5f4e 414d 450a 0a20 2020 2020 2023  SE_NAME..      #
-00002410: 2074 6172 6765 7420 7365 7276 6572 2061   target server a
-00002420: 6464 7265 7373 0a20 2020 2020 2068 6f73  ddress.      hos
-00002430: 743a 2024 484f 5354 5f41 4444 5245 5353  t: $HOST_ADDRESS
-00002440: 2020 0a20 2020 2020 2070 6f72 743a 2024    .      port: $
-00002450: 504f 5254 5f4e 554d 4245 520a 0a20 2020  PORT_NUMBER..   
-00002460: 2020 2023 2061 6363 6f75 6e74 2063 7265     # account cre
-00002470: 6465 6e74 6961 6c73 0a20 2020 2020 2061  dentials.      a
-00002480: 6363 6f75 6e74 3a20 2441 4343 4f55 4e54  ccount: $ACCOUNT
-00002490: 5f4e 414d 450a 2020 2020 2020 7573 6572  _NAME.      user
-000024a0: 3a20 2455 5345 525f 4e41 4d45 0a20 2020  : $USER_NAME.   
-000024b0: 2020 2070 6173 7377 6f72 643a 2024 5041     password: $PA
-000024c0: 5353 574f 5244 0a0a 2020 2020 2020 2320  SSWORD..      # 
-000024d0: 6164 6469 7469 6f6e 616c 2073 6574 7469  additional setti
-000024e0: 6e67 730a 2020 2020 2020 7365 6375 7265  ngs.      secure
-000024f0: 3a20 5472 7565 0a60 6060 0a23 2323 2048  : True.```.### H
-00002500: 6f73 7420 4164 6472 6573 7320 2620 4150  ost Address & AP
-00002510: 4920 4b65 7920 436f 6e66 6967 7572 6174  I Key Configurat
-00002520: 696f 6e0a 5265 7175 6972 6564 2070 6172  ion.Required par
-00002530: 616d 6574 6572 733a 2060 686f 7374 6020  ameters: `host` 
-00002540: 6070 6f72 7460 2060 7573 6572 6020 6070  `port` `user` `p
-00002550: 6173 7377 6f72 6460 0a60 6060 7961 6d6c  assword`.```yaml
-00002560: 0a62 7974 6568 6f75 7365 5f70 726f 6669  .bytehouse_profi
-00002570: 6c65 3a0a 2020 7461 7267 6574 3a20 6465  le:.  target: de
-00002580: 760a 2020 6f75 7470 7574 733a 0a20 2020  v.  outputs:.   
-00002590: 2064 6576 3a0a 2020 2020 2020 7479 7065   dev:.      type
-000025a0: 3a20 6279 7465 686f 7573 650a 2020 2020  : bytehouse.    
-000025b0: 2020 6472 6976 6572 3a20 6e61 7469 7665    driver: native
-000025c0: 0a0a 2020 2020 2020 2320 6461 7461 6261  ..      # databa
-000025d0: 7365 0a20 2020 2020 2073 6368 656d 613a  se.      schema:
-000025e0: 2024 4441 5441 4241 5345 5f4e 414d 450a   $DATABASE_NAME.
-000025f0: 0a20 2020 2020 2023 2074 6172 6765 7420  .      # target 
-00002600: 7365 7276 6572 2061 6464 7265 7373 0a20  server address. 
-00002610: 2020 2020 2068 6f73 743a 2024 484f 5354       host: $HOST
-00002620: 5f41 4444 5245 5353 2020 0a20 2020 2020  _ADDRESS  .     
-00002630: 2070 6f72 743a 2024 504f 5254 5f4e 554d   port: $PORT_NUM
-00002640: 4245 520a 0a20 2020 2020 2023 2061 6363  BER..      # acc
-00002650: 6f75 6e74 2063 7265 6465 6e74 6961 6c73  ount credentials
-00002660: 0a20 2020 2020 2075 7365 723a 2062 7974  .      user: byt
-00002670: 6568 6f75 7365 0a20 2020 2020 2070 6173  ehouse.      pas
-00002680: 7377 6f72 643a 2024 4150 495f 4b45 590a  sword: $API_KEY.
-00002690: 0a20 2020 2020 2023 2061 6464 6974 696f  .      # additio
-000026a0: 6e61 6c20 7365 7474 696e 6773 0a20 2020  nal settings.   
-000026b0: 2020 2073 6563 7572 653a 2054 7275 650a     secure: True.
-000026c0: 6060 600a 2323 2050 726f 6a65 6374 2049  ```.## Project I
-000026d0: 6e69 7469 616c 697a 6174 696f 6e0a 6064  nitialization.`d
-000026e0: 6274 2069 6e69 7460 2063 6f6d 6d61 6e64  bt init` command
-000026f0: 2077 696c 6c20 7072 6f6d 7074 2066 6f72   will prompt for
-00002700: 2070 726f 6a65 6374 206e 616d 6520 2620   project name & 
-00002710: 6461 7461 6261 7365 2061 6461 7074 6572  database adapter
-00002720: 732c 2077 6865 7265 2079 6f75 2068 6176  s, where you hav
-00002730: 6520 746f 2073 656c 6563 7420 6279 7465  e to select byte
-00002740: 686f 7573 652e 2054 6869 7320 7769 6c6c  house. This will
-00002750: 2063 7265 6174 650a 6120 6e65 7720 666f   create.a new fo
-00002760: 6c64 6572 2077 6974 6820 796f 7572 2070  lder with your p
-00002770: 726f 6a65 6374 206e 616d 652c 2073 616d  roject name, sam
-00002780: 706c 6520 6669 6c65 7320 2620 6064 6274  ple files & `dbt
-00002790: 5f70 726f 6a65 6374 2e79 6d6c 6020 636f  _project.yml` co
-000027a0: 6e66 6967 2066 696c 652c 2065 6e6f 7567  nfig file, enoug
-000027b0: 6820 746f 2067 6574 2079 6f75 2073 7461  h to get you sta
-000027c0: 7274 6564 2077 6974 6820 6462 742e 0a60  rted with dbt..`
-000027d0: 6060 636f 6d6d 616e 646c 696e 650a 6462  ``commandline.db
-000027e0: 7420 696e 6974 0a60 6060 0a21 5b49 6e69  t init.```.![Ini
-000027f0: 745d 282e 2f65 7861 6d70 6c65 732f 325f  t](./examples/2_
-00002800: 7072 6f66 696c 6573 2e70 6e67 290a 5570  profiles.png).Up
-00002810: 6461 7465 2079 6f75 7220 7072 6f66 696c  date your profil
-00002820: 6573 2e79 6d6c 2077 6974 6820 7265 7175  es.yml with requ
-00002830: 6972 6564 2061 7574 6865 6e74 6963 6174  ired authenticat
-00002840: 696f 6e20 2620 7461 7267 6574 2073 6572  ion & target ser
-00002850: 7665 7220 6372 6564 656e 7469 616c 732e  ver credentials.
-00002860: 200a 6060 6063 6f6d 6d61 6e64 6c69 6e65   .```commandline
-00002870: 0a6e 616e 6f20 7e2f 2e64 6274 2f70 726f  .nano ~/.dbt/pro
-00002880: 6669 6c65 732e 796d 6c0a 6060 600a 4173  files.yml.```.As
-00002890: 2060 6462 7460 2068 6173 2063 7265 6174   `dbt` has creat
-000028a0: 6564 2061 206e 6577 2066 6f6c 6465 7220  ed a new folder 
-000028b0: 7769 7468 2074 6865 2073 616d 6520 6e61  with the same na
-000028c0: 6d65 2061 7320 796f 7572 2070 726f 6a65  me as your proje
-000028d0: 6374 206e 616d 652c 2063 6861 6e67 6520  ct name, change 
-000028e0: 796f 7572 2063 7572 7265 6e74 200a 6469  your current .di
-000028f0: 7265 6374 6f72 7920 746f 2074 6865 2070  rectory to the p
-00002900: 726f 6a65 6374 2066 6f6c 6465 722e 200a  roject folder. .
-00002910: 6060 6063 6f6d 6d61 6e64 6c69 6e65 0a63  ```commandline.c
-00002920: 6420 6462 745f 6279 7465 686f 7573 655f  d dbt_bytehouse_
-00002930: 6465 6d6f 0a60 6060 0a55 7064 6174 6520  demo.```.Update 
-00002940: 796f 7572 2060 6462 745f 7072 6f6a 6563  your `dbt_projec
-00002950: 742e 796d 6c60 2066 696c 6520 746f 2068  t.yml` file to h
-00002960: 6176 6520 7468 6520 7361 6d65 2070 726f  ave the same pro
-00002970: 6669 6c65 5f6e 616d 6520 6173 2060 7e2f  file_name as `~/
-00002980: 2e64 6274 2f70 726f 6669 6c65 732e 796d  .dbt/profiles.ym
-00002990: 6c60 2e0a 6060 6063 6f6d 6d61 6e64 6c69  l`..```commandli
-000029a0: 6e65 0a6e 616e 6f20 6462 745f 7072 6f6a  ne.nano dbt_proj
-000029b0: 6563 742e 796d 6c0a 6060 600a 215b 5072  ect.yml.```.![Pr
-000029c0: 6f6a 6563 745d 282e 2f65 7861 6d70 6c65  oject](./example
-000029d0: 732f 335f 7072 6f6a 6563 742e 706e 6729  s/3_project.png)
-000029e0: 0a23 2320 5465 7374 2057 6172 6568 6f75  .## Test Warehou
-000029f0: 7365 2043 6f6e 6e65 6374 696f 6e0a 5573  se Connection.Us
-00002a00: 6520 6064 6274 2064 6562 7567 6020 636f  e `dbt debug` co
-00002a10: 6d6d 616e 6420 746f 2076 6572 6966 7920  mmand to verify 
-00002a20: 7265 7175 6972 6564 2064 6570 656e 6465  required depende
-00002a30: 6e63 6965 7320 2620 7761 7265 686f 7573  ncies & warehous
-00002a40: 6520 636f 6e6e 6563 7469 6f6e 2e20 496e  e connection. In
-00002a50: 2063 6173 6520 6f66 2073 7563 6365 7373   case of success
-00002a60: 2c20 6974 2077 696c 6c20 7368 6f77 2079  , it will show y
-00002a70: 6f75 200a 2241 6c6c 2063 6865 636b 7320  ou ."All checks 
-00002a80: 7061 7373 6564 2122 0a60 6060 636f 6d6d  passed!".```comm
-00002a90: 616e 646c 696e 650a 6462 7420 6465 6275  andline.dbt debu
-00002aa0: 670a 6060 600a 215b 4465 6275 675d 282e  g.```.![Debug](.
-00002ab0: 2f65 7861 6d70 6c65 732f 345f 6465 6275  /examples/4_debu
-00002ac0: 672e 706e 6729 0a23 2044 6174 6173 6574  g.png).# Dataset
-00002ad0: 2049 6e67 6573 7469 6f6e 0a54 6f20 7368   Ingestion.To sh
-00002ae0: 6f77 6361 7365 2064 6966 6665 7265 6e74  owcase different
-00002af0: 2060 6462 7460 2066 756e 6374 696f 6e61   `dbt` functiona
-00002b00: 6c69 7469 6573 2c20 7765 2077 696c 6c20  lities, we will 
-00002b10: 696e 6765 7374 2061 2073 6d61 6c6c 2069  ingest a small i
-00002b20: 6d64 6220 6d6f 7669 6520 6461 7461 7365  mdb movie datase
-00002b30: 742c 2077 6974 6820 7468 6520 666f 6c6c  t, with the foll
-00002b40: 6f77 696e 6720 7363 6865 6d61 2e20 0a54  owing schema. .T
-00002b50: 6865 2044 444c 2026 2069 6e73 6572 7469  he DDL & inserti
-00002b60: 6f6e 2071 7565 7269 6573 2063 616e 2062  on queries can b
-00002b70: 6520 666f 756e 6420 6865 7265 2068 7474  e found here htt
-00002b80: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002b90: 6279 7465 686f 7573 652d 636c 6f75 642f  bytehouse-cloud/
-00002ba0: 6279 7465 686f 7573 652d 6462 742f 6578  bytehouse-dbt/ex
-00002bb0: 616d 706c 6573 2f64 6174 615f 6c6f 6164  amples/data_load
-00002bc0: 696e 672e 7371 6c2e 200a 596f 7520 6361  ing.sql. .You ca
-00002bd0: 6e20 7573 6520 4279 7465 486f 7573 6520  n use ByteHouse 
-00002be0: 5351 4c20 776f 726b 7368 6565 7420 746f  SQL worksheet to
-00002bf0: 2063 7265 6174 6520 7468 6520 7363 6865   create the sche
-00002c00: 6d61 2026 2069 6e73 6572 7420 7468 6520  ma & insert the 
-00002c10: 6461 7461 7365 742e 200a 215b 5363 6865  dataset. .![Sche
-00002c20: 6d61 5d28 2e2f 6578 616d 706c 6573 2f35  ma](./examples/5
-00002c30: 5f73 6368 656d 612e 706e 6729 0a54 6f20  _schema.png).To 
-00002c40: 7665 7269 6679 2074 6861 7420 6461 7461  verify that data
-00002c50: 7365 7420 7072 6570 6172 6174 696f 6e20  set preparation 
-00002c60: 7761 7320 7375 6363 6573 7366 756c 2c20  was successful, 
-00002c70: 7765 2077 696c 6c20 6578 6563 7574 6520  we will execute 
-00002c80: 7468 6973 2066 6f6c 6c6f 7769 6e67 2071  this following q
-00002c90: 7565 7279 2074 6f20 7375 6d6d 6172 697a  uery to summariz
-00002ca0: 6520 6561 6368 2061 6374 6f72 2061 6c6f  e each actor alo
-00002cb0: 6e67 200a 7769 7468 2074 6865 6972 2074  ng .with their t
-00002cc0: 6f74 616c 206e 756d 6265 7220 6f66 206d  otal number of m
-00002cd0: 6f76 6965 2061 7070 6561 7261 6e63 6573  ovie appearances
-00002ce0: 2e20 0a60 6060 0a53 454c 4543 5420 6964  . .```.SELECT id
-00002cf0: 2c0a 2020 616e 7928 6163 746f 725f 6e61  ,.  any(actor_na
-00002d00: 6d65 2920 6173 206e 616d 652c 0a20 2075  me) as name,.  u
-00002d10: 6e69 7145 7861 6374 286d 6f76 6965 5f69  niqExact(movie_i
-00002d20: 6429 2020 2020 6173 206e 756d 5f6d 6f76  d)    as num_mov
-00002d30: 6965 732c 0a20 2061 7667 2872 6174 696e  ies,.  avg(ratin
-00002d40: 6729 2020 2020 2020 2020 2020 2020 2020  g)              
-00002d50: 2020 6173 2061 7667 5f72 6174 696e 672c    as avg_rating,
-00002d60: 0a20 206d 6178 2863 7265 6174 6564 5f61  .  max(created_a
-00002d70: 7429 2061 7320 7570 6461 7465 645f 6174  t) as updated_at
-00002d80: 0a46 524f 4d20 280a 2020 5345 4c45 4354  .FROM (.  SELECT
-00002d90: 2061 6374 6f72 732e 6964 2061 7320 6964   actors.id as id
-00002da0: 2c0a 2020 2020 2020 2063 6f6e 6361 7428  ,.       concat(
-00002db0: 6163 746f 7273 2e66 6972 7374 5f6e 616d  actors.first_nam
-00002dc0: 652c 2027 2027 2c20 6163 746f 7273 2e6c  e, ' ', actors.l
-00002dd0: 6173 745f 6e61 6d65 2920 6173 2061 6374  ast_name) as act
-00002de0: 6f72 5f6e 616d 652c 0a20 2020 2020 2020  or_name,.       
-00002df0: 6d6f 7669 6573 2e69 6420 6173 206d 6f76  movies.id as mov
-00002e00: 6965 5f69 642c 0a20 2020 2020 2020 6d6f  ie_id,.       mo
-00002e10: 7669 6573 2e72 6174 696e 6720 6173 2072  vies.rating as r
-00002e20: 6174 696e 672c 0a20 2020 2020 2020 6372  ating,.       cr
-00002e30: 6561 7465 645f 6174 0a20 2046 524f 4d20  eated_at.  FROM 
-00002e40: 2069 6d64 622e 6163 746f 7273 0a20 2020   imdb.actors.   
-00002e50: 2020 2020 204a 4f49 4e20 696d 6462 2e72       JOIN imdb.r
-00002e60: 6f6c 6573 204f 4e20 726f 6c65 732e 6163  oles ON roles.ac
-00002e70: 746f 725f 6964 203d 2061 6374 6f72 732e  tor_id = actors.
-00002e80: 6964 0a20 2020 2020 2020 204c 4546 5420  id.        LEFT 
-00002e90: 4f55 5445 5220 4a4f 494e 2069 6d64 622e  OUTER JOIN imdb.
-00002ea0: 6d6f 7669 6573 204f 4e20 6d6f 7669 6573  movies ON movies
-00002eb0: 2e69 6420 3d20 726f 6c65 732e 6d6f 7669  .id = roles.movi
-00002ec0: 655f 6964 0a29 0a47 524f 5550 2042 5920  e_id.).GROUP BY 
-00002ed0: 6964 0a60 6060 0a54 6865 2072 6573 756c  id.```.The resul
-00002ee0: 7473 6574 2073 686f 756c 6420 6265 206c  tset should be l
-00002ef0: 696b 6520 7468 6973 3a0a 215b 5363 6865  ike this:.![Sche
-00002f00: 6d61 2043 6f6e 6669 726d 5d28 2e2f 6578  ma Confirm](./ex
-00002f10: 616d 706c 6573 2f36 5f73 6368 656d 615f  amples/6_schema_
-00002f20: 636f 6e66 6972 6d2e 706e 6729 0a23 2064  confirm.png).# d
-00002f30: 6274 204d 6f64 656c 7320 0a49 6e20 6120  bt Models .In a 
-00002f40: 6064 6274 6020 7072 6f6a 6563 742c 2061  `dbt` project, a
-00002f50: 206d 6f64 656c 2069 7320 6120 7371 6c20   model is a sql 
-00002f60: 6669 6c65 206c 6f63 6174 6564 2069 6e73  file located ins
-00002f70: 6964 6520 606d 6f64 656c 732f 6020 6469  ide `models/` di
-00002f80: 7265 6374 6f72 7920 7768 6963 6820 7769  rectory which wi
-00002f90: 6c6c 2063 6f6e 7461 696e 2061 2060 5345  ll contain a `SE
-00002fa0: 4c45 4354 6020 7374 6174 656d 656e 7420  LECT` statement 
-00002fb0: 0a72 6566 6572 7269 6e67 2074 6f20 6120  .referring to a 
-00002fc0: 7472 616e 7366 6f72 6d61 7469 6f6e 2e20  transformation. 
-00002fd0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-00002fe0: 6d6f 6465 6c20 6669 6c65 2077 696c 6c20  model file will 
-00002ff0: 7265 6665 7220 746f 2074 6865 206e 616d  refer to the nam
-00003000: 6520 6f66 2066 7574 7572 6520 7461 626c  e of future tabl
-00003010: 652f 7669 6577 2061 6674 6572 0a60 6462  e/view after.`db
-00003020: 7460 2065 7865 6375 7469 6f6e 2e20 5768  t` execution. Wh
-00003030: 656e 2077 6520 6578 6563 7574 6520 6064  en we execute `d
-00003040: 6274 2072 756e 6020 636f 6d6d 616e 642c  bt run` command,
-00003050: 2060 6462 7460 2077 696c 6c20 6275 696c   `dbt` will buil
-00003060: 6420 7468 6973 206d 6f64 656c 2064 6972  d this model dir
-00003070: 6563 746c 7920 696e 746f 2042 7974 6548  ectly into ByteH
-00003080: 6f75 7365 2062 7920 7772 6170 7069 6e67  ouse by wrapping
-00003090: 0a69 7420 696e 2061 2063 7265 6174 6520  .it in a create 
-000030a0: 7461 626c 6520 2f20 7669 6577 206d 6174  table / view mat
-000030b0: 6572 6961 6c69 7a61 7469 6f6e 2e20 4d61  erialization. Ma
-000030c0: 7465 7269 616c 697a 6174 696f 6e20 7479  terialization ty
-000030d0: 7065 206f 6620 796f 7572 206d 6f64 656c  pe of your model
-000030e0: 2077 696c 6c20 6465 7465 726d 696e 6520   will determine 
-000030f0: 7468 6520 6163 7475 616c 2053 514c 0a74  the actual SQL.t
-00003100: 6861 7420 6064 6274 6020 7769 6c6c 2075  hat `dbt` will u
-00003110: 7365 2074 6f20 6372 6561 7465 206d 6f64  se to create mod
-00003120: 656c 2069 6e20 7468 6520 7761 7265 686f  el in the wareho
-00003130: 7573 652e 0a23 2073 6368 656d 612e 796d  use..# schema.ym
-00003140: 6c0a 5468 6520 6073 6368 656d 612e 796d  l.The `schema.ym
-00003150: 6c60 2066 696c 6520 7769 6c6c 2064 6566  l` file will def
-00003160: 696e 6520 6f75 7220 7461 626c 6573 2026  ine our tables &
-00003170: 2063 6f6c 756d 6e73 2062 7920 7265 6665   columns by refe
-00003180: 7272 696e 6720 7468 726f 7567 6820 616c  rring through al
-00003190: 6961 7320 6e61 6d65 2e20 5468 6973 2073  ias name. This s
-000031a0: 6368 656d 6173 2063 616e 206c 6174 6572  chemas can later
-000031b0: 2062 650a 7573 6564 2069 6e20 6469 6666   be.used in diff
-000031c0: 6572 656e 7420 6d6f 6465 6c73 2f6d 6163  erent models/mac
-000031d0: 726f 7320 7669 6120 6073 6f75 7263 6528  ros via `source(
-000031e0: 2960 2066 756e 6374 696f 6e2e 0a43 7265  )` function..Cre
-000031f0: 6174 6520 6073 6368 656d 612e 796d 6c60  ate `schema.yml`
-00003200: 2066 696c 6520 756e 6465 7220 606d 6f64   file under `mod
-00003210: 656c 732f 6020 6469 7265 6374 6f72 790a  els/` directory.
-00003220: 6060 6063 6f6d 6d61 6e64 6c69 6e65 0a74  ```commandline.t
-00003230: 6f75 6368 206d 6f64 656c 732f 7363 6865  ouch models/sche
-00003240: 6d61 2e79 6d6c 0a60 6060 0a44 6566 696e  ma.yml.```.Defin
-00003250: 6520 6f75 7220 6d6f 6465 6c20 7363 6865  e our model sche
-00003260: 6d61 206c 696b 6520 7468 6973 0a60 6060  ma like this.```
-00003270: 7961 6d6c 0a76 6572 7369 6f6e 3a20 320a  yaml.version: 2.
-00003280: 0a73 6f75 7263 6573 3a0a 2d20 6e61 6d65  .sources:.- name
-00003290: 3a20 696d 6462 0a20 2074 6162 6c65 733a  : imdb.  tables:
-000032a0: 0a20 202d 206e 616d 653a 2061 6374 6f72  .  - name: actor
-000032b0: 730a 2020 2d20 6e61 6d65 3a20 726f 6c65  s.  - name: role
-000032c0: 730a 2020 2d20 6e61 6d65 3a20 6d6f 7669  s.  - name: movi
-000032d0: 6573 0a60 6060 0a23 204d 6174 6572 6961  es.```.# Materia
-000032e0: 6c69 7a61 7469 6f6e 2074 7970 6573 206f  lization types o
-000032f0: 6620 4d6f 6465 6c73 0a23 2320 5669 6577  f Models.## View
-00003300: 204d 6174 6572 6961 6c69 7a61 7469 6f6e   Materialization
-00003310: 730a 496e 2063 6173 6520 6f66 2076 6965  s.In case of vie
-00003320: 7720 6d61 7465 7269 616c 697a 6174 696f  w materializatio
-00003330: 6e2c 2061 206d 6f64 656c 2069 7320 7472  n, a model is tr
-00003340: 616e 7366 6f72 6d65 6420 746f 2061 2076  ansformed to a v
-00003350: 6965 7720 6f6e 2065 6163 6820 7369 6e67  iew on each sing
-00003360: 6c65 2072 756e 2062 7920 6043 5245 4154  le run by `CREAT
-00003370: 4520 5649 4557 6020 4153 2073 7461 7465  E VIEW` AS state
-00003380: 6d65 6e74 2069 6e20 0a42 7974 6548 6f75  ment in .ByteHou
-00003390: 7365 2e20 5669 6577 206d 6174 6572 6961  se. View materia
-000033a0: 6c69 7a61 7469 6f6e 7320 776f 6e27 7420  lizations won't 
-000033b0: 7374 6f72 6520 7468 6520 6163 7475 616c  store the actual
-000033c0: 2064 6174 612c 2073 6f20 6974 2077 6f75   data, so it wou
-000033d0: 6c64 2062 6520 736c 6f77 6572 2074 6f20  ld be slower to 
-000033e0: 7175 6572 7920 7468 616e 2074 6162 6c65  query than table
-000033f0: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
-00003400: 732e 0a4c 6574 2773 2063 7265 6174 6520  s..Let's create 
-00003410: 606d 6f64 656c 732f 6163 746f 725f 696e  `models/actor_in
-00003420: 7369 6768 742e 7371 6c60 2061 7320 7669  sight.sql` as vi
-00003430: 6577 206d 6174 6572 6961 6c69 7a61 7469  ew materializati
-00003440: 6f6e 2e20 0a60 6060 636f 6d6d 616e 646c  on. .```commandl
-00003450: 696e 650a 746f 7563 6820 6d6f 6465 6c73  ine.touch models
-00003460: 2f61 6374 6f72 735f 696e 7369 6768 742e  /actors_insight.
-00003470: 7371 6c0a 6060 600a 6060 600a 7b7b 2063  sql.```.```.{{ c
-00003480: 6f6e 6669 6728 6d61 7465 7269 616c 697a  onfig(materializ
-00003490: 6564 3d27 7669 6577 2729 207d 7d0a 0a53  ed='view') }}..S
-000034a0: 454c 4543 5420 6964 2c0a 2020 616e 7928  ELECT id,.  any(
-000034b0: 6163 746f 725f 6e61 6d65 2920 6173 206e  actor_name) as n
-000034c0: 616d 652c 0a20 2075 6e69 7145 7861 6374  ame,.  uniqExact
-000034d0: 286d 6f76 6965 5f69 6429 2020 2020 6173  (movie_id)    as
-000034e0: 206e 756d 5f6d 6f76 6965 732c 0a20 2061   num_movies,.  a
-000034f0: 7667 2872 6174 696e 6729 2020 2020 2020  vg(rating)      
-00003500: 2020 2020 2020 2020 2020 6173 2061 7667            as avg
-00003510: 5f72 6174 696e 672c 0a20 206d 6178 2863  _rating,.  max(c
-00003520: 7265 6174 6564 5f61 7429 2061 7320 7570  reated_at) as up
-00003530: 6461 7465 645f 6174 0a46 524f 4d20 280a  dated_at.FROM (.
-00003540: 2020 5345 4c45 4354 2061 6374 6f72 732e    SELECT actors.
-00003550: 6964 2061 7320 6964 2c0a 2020 2020 2020  id as id,.      
-00003560: 2063 6f6e 6361 7428 6163 746f 7273 2e66   concat(actors.f
-00003570: 6972 7374 5f6e 616d 652c 2027 2027 2c20  irst_name, ' ', 
-00003580: 6163 746f 7273 2e6c 6173 745f 6e61 6d65  actors.last_name
-00003590: 2920 6173 2061 6374 6f72 5f6e 616d 652c  ) as actor_name,
-000035a0: 0a20 2020 2020 2020 6d6f 7669 6573 2e69  .       movies.i
-000035b0: 6420 6173 206d 6f76 6965 5f69 642c 0a20  d as movie_id,. 
-000035c0: 2020 2020 2020 6d6f 7669 6573 2e72 6174        movies.rat
-000035d0: 696e 6720 6173 2072 6174 696e 672c 0a20  ing as rating,. 
-000035e0: 2020 2020 2020 6372 6561 7465 645f 6174        created_at
-000035f0: 0a20 2046 524f 4d20 207b 7b20 736f 7572  .  FROM  {{ sour
-00003600: 6365 2827 696d 6462 272c 2027 6163 746f  ce('imdb', 'acto
-00003610: 7273 2729 207d 7d0a 2020 2020 2020 2020  rs') }}.        
-00003620: 4a4f 494e 207b 7b20 736f 7572 6365 2827  JOIN {{ source('
-00003630: 696d 6462 272c 2027 726f 6c65 7327 2920  imdb', 'roles') 
-00003640: 7d7d 204f 4e20 726f 6c65 732e 6163 746f  }} ON roles.acto
-00003650: 725f 6964 203d 2061 6374 6f72 732e 6964  r_id = actors.id
-00003660: 0a20 2020 2020 2020 204c 4546 5420 4f55  .        LEFT OU
-00003670: 5445 5220 4a4f 494e 207b 7b20 736f 7572  TER JOIN {{ sour
-00003680: 6365 2827 696d 6462 272c 2027 6d6f 7669  ce('imdb', 'movi
-00003690: 6573 2729 207d 7d20 4f4e 206d 6f76 6965  es') }} ON movie
-000036a0: 732e 6964 203d 2072 6f6c 6573 2e6d 6f76  s.id = roles.mov
-000036b0: 6965 5f69 640a 290a 4752 4f55 5020 4259  ie_id.).GROUP BY
-000036c0: 2069 640a 6060 600a 4c65 7427 7320 6578   id.```.Let's ex
-000036d0: 6563 7574 6520 6064 6274 2072 756e 6020  ecute `dbt run` 
-000036e0: 636f 6d6d 616e 6420 746f 2062 7569 6c64  command to build
-000036f0: 2074 6869 7320 6d6f 6465 6c20 696e 2042   this model in B
-00003700: 7974 6548 6f75 7365 2e20 0a21 5b43 6f6e  yteHouse. .![Con
-00003710: 6669 726d 5d28 2e2f 6578 616d 706c 6573  firm](./examples
-00003720: 2f37 5f61 6374 6f72 5f69 6e73 6967 6874  /7_actor_insight
-00003730: 5f63 6f6e 6669 726d 2e70 6e67 290a 5175  _confirm.png).Qu
-00003740: 6572 7969 6e67 2074 6869 7320 7669 6577  erying this view
-00003750: 2c20 7765 2063 616e 2072 6570 6c69 6361  , we can replica
-00003760: 7465 2074 6865 2072 6573 756c 7473 206f  te the results o
-00003770: 6620 6f75 7220 6561 726c 6965 7220 7175  f our earlier qu
-00003780: 6572 7920 7769 7468 2061 2073 696d 706c  ery with a simpl
-00003790: 6572 2073 796e 7461 783a 0a60 6060 0a53  er syntax:.```.S
-000037a0: 454c 4543 5420 2a20 4652 4f4d 2069 6d64  ELECT * FROM imd
-000037b0: 622e 6163 746f 7273 5f69 6e73 6967 6874  b.actors_insight
-000037c0: 204f 5244 4552 2042 5920 6e75 6d5f 6d6f   ORDER BY num_mo
-000037d0: 7669 6573 2044 4553 433b 0a60 6060 0a21  vies DESC;.```.!
-000037e0: 5b43 6f6e 6669 726d 325d 282e 2f65 7861  [Confirm2](./exa
-000037f0: 6d70 6c65 732f 385f 6d61 7465 7269 616c  mples/8_material
-00003800: 697a 6564 5f76 6965 775f 7275 6e5f 636f  ized_view_run_co
-00003810: 6e66 6972 6d2e 706e 6729 0a23 2320 5461  nfirm.png).## Ta
-00003820: 626c 6520 4d61 7465 7269 616c 697a 6174  ble Materializat
-00003830: 696f 6e73 0a49 6e20 6361 7365 206f 6620  ions.In case of 
-00003840: 7461 626c 6520 6d61 7465 7269 616c 697a  table materializ
-00003850: 6174 696f 6e2c 2079 6f75 7220 6d6f 6465  ation, your mode
-00003860: 6c20 776f 756c 6420 6265 2072 6562 7569  l would be rebui
-00003870: 6c74 2061 7320 6120 7461 626c 6520 6f6e  lt as a table on
-00003880: 2065 6163 6820 7369 6e67 6c65 2060 6462   each single `db
-00003890: 7420 7275 6e60 200a 7669 6120 6120 6043  t run` .via a `C
-000038a0: 5245 4154 4520 5441 424c 4560 2041 5320  REATE TABLE` AS 
-000038b0: 7374 6174 656d 656e 742e 200a 6060 6063  statement. .```c
-000038c0: 6f6d 6d61 6e64 6c69 6e65 0a74 6f75 6368  ommandline.touch
-000038d0: 206d 6f64 656c 732f 6163 746f 7273 5f69   models/actors_i
-000038e0: 6e73 6967 6874 5f74 6162 6c65 2e73 716c  nsight_table.sql
-000038f0: 0a60 6060 0a57 6520 6361 6e20 7573 6520  .```.We can use 
-00003900: 6f75 7220 7072 6576 696f 7573 2076 6965  our previous vie
-00003910: 7720 6d61 7465 7269 616c 697a 6174 696f  w materializatio
-00003920: 6e20 7371 6c20 7769 7468 2063 6f6e 6669  n sql with confi
-00003930: 6720 6368 616e 6765 2066 6f72 2074 6162  g change for tab
-00003940: 6c65 206d 6174 6572 6961 6c69 7a61 7469  le materializati
-00003950: 6f6e 2073 716c 2e20 0a60 6060 0a7b 7b20  on sql. .```.{{ 
-00003960: 636f 6e66 6967 286f 7264 6572 5f62 793d  config(order_by=
-00003970: 2728 7570 6461 7465 645f 6174 2c20 6964  '(updated_at, id
-00003980: 2c20 6e61 6d65 2927 2c20 6d61 7465 7269  , name)', materi
-00003990: 616c 697a 6564 3d27 7461 626c 6527 2920  alized='table') 
-000039a0: 7d7d 0a60 6060 0a57 6520 6361 6e20 7665  }}.```.We can ve
-000039b0: 7269 6679 2074 6861 7420 626f 7468 2076  rify that both v
-000039c0: 6965 7720 2620 7461 626c 6520 6d61 7465  iew & table mate
-000039d0: 7269 616c 697a 6174 696f 6e73 2067 656e  rializations gen
-000039e0: 6572 6174 6520 7468 6520 7361 6d65 2072  erate the same r
-000039f0: 6573 706f 6e73 652e 200a 6060 600a 2053  esponse. .```. S
-00003a00: 454c 4543 5420 2a20 4652 4f4d 2069 6d64  ELECT * FROM imd
-00003a10: 622e 6163 746f 7273 5f69 6e73 6967 6874  b.actors_insight
-00003a20: 5f74 6162 6c65 204f 5244 4552 2042 5920  _table ORDER BY 
-00003a30: 6e75 6d5f 6d6f 7669 6573 2044 4553 433b  num_movies DESC;
-00003a40: 0a60 6060 0a23 2320 496e 6372 656d 656e  .```.## Incremen
-00003a50: 7461 6c20 4d61 7465 7269 616c 697a 6174  tal Materializat
-00003a60: 696f 6e73 0a46 6f72 206f 7572 2070 7265  ions.For our pre
-00003a70: 7669 6f75 7320 7461 626c 6520 6d61 7465  vious table mate
-00003a80: 7269 616c 697a 6174 696f 6e2c 2060 6462  rialization, `db
-00003a90: 7460 2077 696c 6c20 636f 6e73 7472 7563  t` will construc
-00003aa0: 7420 6120 7461 626c 6520 6576 6572 7920  t a table every 
-00003ab0: 7469 6d65 2074 6f20 6d61 7465 7269 616c  time to material
-00003ac0: 697a 6520 7468 6520 6d6f 6465 6c2e 2046  ize the model. F
-00003ad0: 6f72 206c 6172 6765 720a 6f72 2063 6f6d  or larger.or com
-00003ae0: 706c 6578 2074 7261 6e73 666f 726d 6174  plex transformat
-00003af0: 696f 6e73 2c20 7468 6973 2077 6f75 6c64  ions, this would
-00003b00: 2062 6520 7265 6475 6e64 616e 7420 616e   be redundant an
-00003b10: 6420 636f 7374 6c79 2069 6e20 7465 726d  d costly in term
-00003b20: 7320 6f66 2063 6f6d 7075 7469 6e67 2070  s of computing p
-00003b30: 6f77 6572 2e20 496e 6372 656d 656e 7461  ower. Incrementa
-00003b40: 6c20 0a6d 6174 6572 6961 6c69 7a61 7469  l .materializati
-00003b50: 6f6e 7320 736f 6c76 6520 7468 6973 2070  ons solve this p
-00003b60: 726f 626c 656d 2e3c 6272 2f3e 0a54 6865  roblem.<br/>.The
-00003b70: 2066 6972 7374 2074 696d 6520 6120 6d6f   first time a mo
-00003b80: 6465 6c20 6973 2072 756e 2c20 7468 6520  del is run, the 
-00003b90: 7461 626c 6520 6973 2062 7569 6c74 2062  table is built b
-00003ba0: 7920 7472 616e 7366 6f72 6d69 6e67 2061  y transforming a
-00003bb0: 6c6c 2072 6f77 7320 6f66 2073 6f75 7263  ll rows of sourc
-00003bc0: 6520 6461 7461 2e20 4f6e 2073 7562 7365  e data. On subse
-00003bd0: 7175 656e 7420 7275 6e73 2c20 0a60 6462  quent runs, .`db
-00003be0: 7460 2074 7261 6e73 666f 726d 7320 6f6e  t` transforms on
-00003bf0: 6c79 2074 6865 2072 6f77 7320 696e 2079  ly the rows in y
-00003c00: 6f75 7220 736f 7572 6365 2064 6174 6120  our source data 
-00003c10: 7468 6174 2079 6f75 2074 656c 6c20 6064  that you tell `d
-00003c20: 6274 6020 746f 2066 696c 7465 7220 666f  bt` to filter fo
-00003c30: 722c 2069 6e73 6572 7469 6e67 2074 6865  r, inserting the
-00003c40: 6d20 696e 746f 2074 6865 2074 6172 6765  m into the targe
-00003c50: 7420 0a74 6162 6c65 2077 6869 6368 2069  t .table which i
-00003c60: 7320 7468 6520 7461 626c 6520 7468 6174  s the table that
-00003c70: 2068 6173 2061 6c72 6561 6479 2062 6565   has already bee
-00003c80: 6e20 6275 696c 742e 3c62 722f 3e0a 546f  n built.<br/>.To
-00003c90: 2074 656c 6c20 6064 6274 6020 7768 6963   tell `dbt` whic
-00003ca0: 6820 726f 7773 2069 7420 7368 6f75 6c64  h rows it should
-00003cb0: 2074 7261 6e73 666f 726d 206f 6e20 616e   transform on an
-00003cc0: 2069 6e63 7265 6d65 6e74 616c 2072 756e   incremental run
-00003cd0: 2c20 7772 6170 2076 616c 6964 2053 514c  , wrap valid SQL
-00003ce0: 2074 6861 7420 6669 6c74 6572 7320 666f   that filters fo
-00003cf0: 7220 7468 6573 6520 726f 7773 200a 696e  r these rows .in
-00003d00: 2074 6865 2060 6973 5f69 6e63 7265 6d65   the `is_increme
-00003d10: 6e74 616c 2829 6020 6d61 6372 6f2e 2059  ntal()` macro. Y
-00003d20: 6f75 7220 6069 735f 696e 6372 656d 656e  our `is_incremen
-00003d30: 7461 6c28 2960 2063 6f64 6520 7769 6c6c  tal()` code will
-00003d40: 2063 6865 636b 2066 6f72 2072 6f77 7320   check for rows 
-00003d50: 6372 6561 7465 6420 6f72 206d 6f64 6966  created or modif
-00003d60: 6965 6420 7369 6e63 6520 7468 6520 0a6c  ied since the .l
-00003d70: 6173 7420 7469 6d65 2060 6462 7460 2072  ast time `dbt` r
-00003d80: 616e 2074 6869 7320 6d6f 6465 6c2e 0a60  an this model..`
-00003d90: 6060 636f 6d6d 616e 646c 696e 650a 746f  ``commandline.to
-00003da0: 7563 6820 6d6f 6465 6c73 2f61 6374 6f72  uch models/actor
-00003db0: 735f 696e 7369 6768 745f 696e 6372 656d  s_insight_increm
-00003dc0: 656e 7461 6c2e 7371 6c0a 6060 600a 6060  ental.sql.```.``
-00003dd0: 600a 7b7b 2063 6f6e 6669 6728 6f72 6465  `.{{ config(orde
-00003de0: 725f 6279 3d27 2875 7064 6174 6564 5f61  r_by='(updated_a
-00003df0: 742c 2069 642c 206e 616d 6529 272c 206d  t, id, name)', m
-00003e00: 6174 6572 6961 6c69 7a65 643d 2769 6e63  aterialized='inc
-00003e10: 7265 6d65 6e74 616c 2729 207d 7d0a 0a53  remental') }}..S
-00003e20: 454c 4543 5420 6964 2c0a 2020 616e 7928  ELECT id,.  any(
-00003e30: 6163 746f 725f 6e61 6d65 2920 6173 206e  actor_name) as n
-00003e40: 616d 652c 0a20 2075 6e69 7145 7861 6374  ame,.  uniqExact
-00003e50: 286d 6f76 6965 5f69 6429 2020 2020 6173  (movie_id)    as
-00003e60: 206e 756d 5f6d 6f76 6965 732c 0a20 2061   num_movies,.  a
-00003e70: 7667 2872 6174 696e 6729 2020 2020 2020  vg(rating)      
-00003e80: 2020 2020 2020 2020 2020 6173 2061 7667            as avg
-00003e90: 5f72 6174 696e 672c 0a20 206d 6178 2863  _rating,.  max(c
-00003ea0: 7265 6174 6564 5f61 7429 2061 7320 7570  reated_at) as up
-00003eb0: 6461 7465 645f 6174 0a46 524f 4d20 280a  dated_at.FROM (.
-00003ec0: 2020 5345 4c45 4354 2061 6374 6f72 732e    SELECT actors.
-00003ed0: 6964 2061 7320 6964 2c0a 2020 2020 2020  id as id,.      
-00003ee0: 2063 6f6e 6361 7428 6163 746f 7273 2e66   concat(actors.f
-00003ef0: 6972 7374 5f6e 616d 652c 2027 2027 2c20  irst_name, ' ', 
-00003f00: 6163 746f 7273 2e6c 6173 745f 6e61 6d65  actors.last_name
-00003f10: 2920 6173 2061 6374 6f72 5f6e 616d 652c  ) as actor_name,
-00003f20: 0a20 2020 2020 2020 6d6f 7669 6573 2e69  .       movies.i
-00003f30: 6420 6173 206d 6f76 6965 5f69 642c 0a20  d as movie_id,. 
-00003f40: 2020 2020 2020 6d6f 7669 6573 2e72 6174        movies.rat
-00003f50: 696e 6720 6173 2072 6174 696e 672c 0a20  ing as rating,. 
-00003f60: 2020 2020 2020 6372 6561 7465 645f 6174        created_at
-00003f70: 0a20 2046 524f 4d20 207b 7b20 736f 7572  .  FROM  {{ sour
-00003f80: 6365 2827 696d 6462 272c 2027 6163 746f  ce('imdb', 'acto
-00003f90: 7273 2729 207d 7d0a 2020 2020 2020 2020  rs') }}.        
-00003fa0: 4a4f 494e 207b 7b20 736f 7572 6365 2827  JOIN {{ source('
-00003fb0: 696d 6462 272c 2027 726f 6c65 7327 2920  imdb', 'roles') 
-00003fc0: 7d7d 204f 4e20 726f 6c65 732e 6163 746f  }} ON roles.acto
-00003fd0: 725f 6964 203d 2061 6374 6f72 732e 6964  r_id = actors.id
-00003fe0: 0a20 2020 2020 2020 204c 4546 5420 4f55  .        LEFT OU
-00003ff0: 5445 5220 4a4f 494e 207b 7b20 736f 7572  TER JOIN {{ sour
-00004000: 6365 2827 696d 6462 272c 2027 6d6f 7669  ce('imdb', 'movi
-00004010: 6573 2729 207d 7d20 4f4e 206d 6f76 6965  es') }} ON movie
-00004020: 732e 6964 203d 2072 6f6c 6573 2e6d 6f76  s.id = roles.mov
-00004030: 6965 5f69 640a 290a 4752 4f55 5020 4259  ie_id.).GROUP BY
-00004040: 2069 640a 0a7b 2520 6966 2069 735f 696e   id..{% if is_in
-00004050: 6372 656d 656e 7461 6c28 2920 257d 0a0a  cremental() %}..
-00004060: 2d2d 2074 6869 7320 6669 6c74 6572 2077  -- this filter w
-00004070: 696c 6c20 6f6e 6c79 2062 6520 6170 706c  ill only be appl
-00004080: 6965 6420 6f6e 2061 6e20 696e 6372 656d  ied on an increm
-00004090: 656e 7461 6c20 7275 6e0a 7768 6572 6520  ental run.where 
-000040a0: 6964 203e 2028 7365 6c65 6374 206d 6178  id > (select max
-000040b0: 2869 6429 2066 726f 6d20 7b7b 2074 6869  (id) from {{ thi
-000040c0: 7320 7d7d 2920 6f72 2075 7064 6174 6564  s }}) or updated
-000040d0: 5f61 7420 3e20 2873 656c 6563 7420 6d61  _at > (select ma
-000040e0: 7828 7570 6461 7465 645f 6174 2920 6672  x(updated_at) fr
-000040f0: 6f6d 207b 7b74 6869 737d 7d29 0a0a 7b25  om {{this}})..{%
-00004100: 2065 6e64 6966 2025 7d0a 6060 600a 5765   endif %}.```.We
-00004110: 2063 616e 2076 6572 6966 7920 7468 6174   can verify that
-00004120: 2076 6965 772c 2074 6162 6c65 2026 2069   view, table & i
-00004130: 6e63 7265 6d65 6e74 616c 206d 6174 6572  ncremental mater
-00004140: 6961 6c69 7a61 7469 6f6e 732c 2061 6c6c  ializations, all
-00004150: 2067 656e 6572 6174 6520 7468 6520 7361   generate the sa
-00004160: 6d65 2072 6573 706f 6e73 652e 200a 6060  me response. .``
-00004170: 600a 2053 454c 4543 5420 2a20 4652 4f4d  `. SELECT * FROM
-00004180: 2069 6d64 622e 6163 746f 7273 5f69 6e73   imdb.actors_ins
-00004190: 6967 6874 5f74 6162 6c65 204f 5244 4552  ight_table ORDER
-000041a0: 2042 5920 6e75 6d5f 6d6f 7669 6573 2044   BY num_movies D
-000041b0: 4553 433b 0a60 6060 0a60 6060 636f 6d6d  ESC;.```.```comm
-000041c0: 616e 646c 696e 650a 6462 7420 7275 6e20  andline.dbt run 
-000041d0: 2d6d 206d 6f64 656c 732f 6163 746f 7273  -m models/actors
-000041e0: 5f69 6e73 6967 6874 5f69 6e63 7265 6d65  _insight_increme
-000041f0: 6e74 616c 2e73 716c 0a60 6060 0a4c 6574  ntal.sql.```.Let
-00004200: 2773 2069 6e73 6572 7420 6120 6665 7720  's insert a few 
-00004210: 6d6f 7265 2072 6f77 7320 746f 2064 656d  more rows to dem
-00004220: 6f6e 7374 7261 7465 2074 6865 2070 6f77  onstrate the pow
-00004230: 6572 206f 6620 696e 6372 656d 656e 7461  er of incrementa
-00004240: 6c20 6d61 7465 7269 616c 697a 6174 696f  l materializatio
-00004250: 6e73 2e20 4e6f 7720 7468 6520 6d6f 7374  ns. Now the most
-00004260: 200a 6170 7065 6172 6564 2061 6374 6f72   .appeared actor
-00004270: 2073 686f 756c 6420 6265 2027 4368 7269   should be 'Chri
-00004280: 7320 5072 6174 7427 2e20 0a60 6060 0a49  s Pratt'. .```.I
-00004290: 4e53 4552 5420 494e 544f 2069 6d64 622e  NSERT INTO imdb.
-000042a0: 6d6f 7669 6573 2056 414c 5545 5320 2839  movies VALUES (9
-000042b0: 2c20 2750 6173 7365 6e67 6572 7327 2c20  , 'Passengers', 
-000042c0: 3230 3136 2c20 3729 3b0a 494e 5345 5254  2016, 7);.INSERT
-000042d0: 2049 4e54 4f20 696d 6462 2e6d 6f76 6965   INTO imdb.movie
-000042e0: 7320 5641 4c55 4553 2028 3130 2c20 2754  s VALUES (10, 'T
-000042f0: 6865 2054 6f6d 6f72 726f 7720 5761 7227  he Tomorrow War'
-00004300: 2c20 3230 3231 2c20 362e 3529 3b0a 0a49  , 2021, 6.5);..I
-00004310: 4e53 4552 5420 494e 544f 2069 6d64 622e  NSERT INTO imdb.
-00004320: 726f 6c65 7320 2861 6374 6f72 5f69 642c  roles (actor_id,
-00004330: 206d 6f76 6965 5f69 642c 2072 6f6c 655f   movie_id, role_
-00004340: 6e61 6d65 2920 5641 4c55 4553 2834 2c20  name) VALUES(4, 
-00004350: 392c 2027 4a69 6d20 5072 6573 746f 6e27  9, 'Jim Preston'
-00004360: 293b 0a49 4e53 4552 5420 494e 544f 2069  );.INSERT INTO i
-00004370: 6d64 622e 726f 6c65 7320 2861 6374 6f72  mdb.roles (actor
-00004380: 5f69 642c 206d 6f76 6965 5f69 642c 2072  _id, movie_id, r
-00004390: 6f6c 655f 6e61 6d65 2920 5641 4c55 4553  ole_name) VALUES
-000043a0: 2834 2c20 3130 2c20 2744 616e 2046 6f72  (4, 10, 'Dan For
-000043b0: 6573 7465 7227 293b 0a60 6060 0a60 6060  ester');.```.```
-000043c0: 636f 6d6d 616e 646c 696e 650a 6462 7420  commandline.dbt 
-000043d0: 7275 6e20 2d6d 206d 6f64 656c 732f 6163  run -m models/ac
-000043e0: 746f 7273 5f69 6e73 6967 6874 5f69 6e63  tors_insight_inc
-000043f0: 7265 6d65 6e74 616c 2e73 716c 0a60 6060  remental.sql.```
-00004400: 0a60 6060 0a53 454c 4543 5420 2a20 4652  .```.SELECT * FR
-00004410: 4f4d 2069 6d64 622e 6163 746f 7273 5f69  OM imdb.actors_i
-00004420: 6e73 6967 6874 5f69 6e63 7265 6d65 6e74  nsight_increment
-00004430: 616c 204f 5244 4552 2042 5920 6e75 6d5f  al ORDER BY num_
-00004440: 6d6f 7669 6573 2044 4553 433b 0a60 6060  movies DESC;.```
-00004450: 0a21 5b43 6f6e 6669 726d 335d 282e 2f65  .![Confirm3](./e
-00004460: 7861 6d70 6c65 732f 395f 696e 6372 656d  xamples/9_increm
-00004470: 656e 7461 6c5f 636f 6e66 6972 6d2e 706e  ental_confirm.pn
-00004480: 6729 0a23 2323 2048 6f77 2069 7420 776f  g).### How it wo
-00004490: 726b 730a 312e 2060 6462 7460 2077 696c  rks.1. `dbt` wil
-000044a0: 6c20 6669 7273 7420 6372 6561 7465 2061  l first create a
-000044b0: 2074 656d 706f 7261 7279 2074 6162 6c65   temporary table
-000044c0: 206e 616d 6564 2060 6163 746f 7273 5f69   named `actors_i
-000044d0: 6e73 6967 6874 5f69 6e63 7265 6d65 6e74  nsight_increment
-000044e0: 616c 5f74 6d70 6020 2620 696e 7365 7274  al_tmp` & insert
-000044f0: 2061 6c6c 2074 686f 7365 2072 6f77 7320   all those rows 
-00004500: 7768 6963 6820 0a70 6173 7320 6f75 7220  which .pass our 
-00004510: 6069 735f 696e 6372 656d 656e 7461 6c28  `is_incremental(
-00004520: 2960 2066 696c 7465 722e 0a32 2e20 4120  )` filter..2. A 
-00004530: 6e65 7720 7461 626c 6520 6061 6374 6f72  new table `actor
-00004540: 735f 696e 7369 6768 745f 696e 6372 656d  s_insight_increm
-00004550: 656e 7461 6c5f 6e65 7760 2077 696c 6c20  ental_new` will 
-00004560: 6265 2063 7265 6174 6564 2026 2072 6f77  be created & row
-00004570: 7320 6672 6f6d 2074 6865 206f 6c64 2074  s from the old t
-00004580: 6162 6c65 2060 6163 746f 7273 5f69 6e73  able `actors_ins
-00004590: 6967 6874 5f69 6e63 7265 6d65 6e74 616c  ight_incremental
-000045a0: 6020 0a77 696c 6c20 6265 2069 6e67 6573  ` .will be inges
-000045b0: 7465 6420 6865 7265 2e20 6064 6274 6020  ted here. `dbt` 
-000045c0: 7769 6c6c 206d 616b 6520 7375 7265 2074  will make sure t
-000045d0: 6861 7420 6075 6e69 7175 655f 6b65 7960  hat `unique_key`
-000045e0: 2028 6966 2061 6e79 2064 6563 6c61 7265   (if any declare
-000045f0: 6420 696e 2063 6f6e 6669 6729 2063 6f6e  d in config) con
-00004600: 7374 7261 696e 7420 6973 206d 6169 6e74  straint is maint
-00004610: 6169 6e65 642c 200a 6279 206e 6f74 2061  ained, .by not a
-00004620: 6c6c 6f77 696e 6720 7468 6f73 6520 726f  llowing those ro
-00004630: 7773 2077 6869 6368 2068 6176 6520 7468  ws which have th
-00004640: 6520 7361 6d65 2060 756e 6971 7565 5f6b  e same `unique_k
-00004650: 6579 6020 6173 2074 6865 2070 7265 7669  ey` as the previ
-00004660: 6f75 7320 7465 6d70 6f72 6172 7920 7461  ous temporary ta
-00004670: 626c 652e 200a 332e 2054 6865 2072 6f77  ble. .3. The row
-00004680: 7320 6672 6f6d 2074 6865 2074 656d 706f  s from the tempo
-00004690: 7261 7279 2074 6162 6c65 2077 6f75 6c64  rary table would
-000046a0: 2062 6520 696e 6765 7374 6564 2069 6e74   be ingested int
-000046b0: 6f20 7468 6520 6e65 7720 7461 626c 652e  o the new table.
-000046c0: 0a34 2e20 4f75 7220 7072 6576 696f 7573  .4. Our previous
-000046d0: 2074 6162 6c65 2028 6061 6374 6f72 735f   table (`actors_
-000046e0: 696e 7369 6768 745f 696e 6372 656d 656e  insight_incremen
-000046f0: 7461 6c60 2920 2620 6e65 7720 7461 626c  tal`) & new tabl
-00004700: 6520 2860 6163 746f 7273 5f69 6e73 6967  e (`actors_insig
-00004710: 6874 5f6e 6577 6029 2077 696c 6c20 6265  ht_new`) will be
-00004720: 2065 7863 6861 6e67 6564 2e20 0a23 2050   exchanged. .# P
-00004730: 726f 6a65 6374 2044 6f63 756d 656e 7461  roject Documenta
-00004740: 7469 6f6e 0a60 6462 7460 2070 726f 7669  tion.`dbt` provi
-00004750: 6465 7320 6120 7761 7920 746f 2067 656e  des a way to gen
-00004760: 6572 6174 6520 646f 6375 6d65 6e74 6174  erate documentat
-00004770: 696f 6e20 666f 7220 796f 7572 2064 6274  ion for your dbt
-00004780: 2070 726f 6a65 6374 2061 6e64 2072 656e   project and ren
-00004790: 6465 7220 6974 2061 7320 6120 7765 6273  der it as a webs
-000047a0: 6974 652e 200a 4372 6561 7465 2060 6d6f  ite. .Create `mo
-000047b0: 6465 6c73 2f61 6374 6f72 735f 696e 7369  dels/actors_insi
-000047c0: 6768 745f 696e 6372 656d 656e 7461 6c2e  ght_incremental.
-000047d0: 796d 6c60 2074 6f20 6765 6e65 7261 7465  yml` to generate
-000047e0: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
-000047f0: 6f72 206f 7572 206d 6f64 656c 732e 200a  or our models. .
-00004800: 6060 6079 616d 6c0a 7665 7273 696f 6e3a  ```yaml.version:
-00004810: 2032 0a0a 6d6f 6465 6c73 3a0a 2020 2d20   2..models:.  - 
-00004820: 6e61 6d65 3a20 6163 746f 7273 5f69 6e73  name: actors_ins
-00004830: 6967 6874 5f69 6e63 7265 6d65 6e74 616c  ight_incremental
-00004840: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
-00004850: 3a20 4163 746f 7220 6170 7065 6172 616e  : Actor appearan
-00004860: 6365 2073 756d 6d61 7279 2062 6173 6564  ce summary based
-00004870: 206f 6e20 726f 6c65 730a 2020 2020 636f   on roles.    co
-00004880: 6c75 6d6e 733a 200a 2020 2020 2020 2d20  lumns: .      - 
-00004890: 6e61 6d65 3a20 6964 0a20 2020 2020 2020  name: id.       
-000048a0: 2064 6573 6372 6970 7469 6f6e 3a20 5468   description: Th
-000048b0: 6520 6964 206e 756d 6265 7220 6f66 2061  e id number of a
-000048c0: 6374 6f72 0a20 2020 2020 202d 206e 616d  ctor.      - nam
-000048d0: 653a 206e 616d 650a 2020 2020 2020 2020  e: name.        
-000048e0: 6465 7363 7269 7074 696f 6e3a 2054 6865  description: The
-000048f0: 206e 616d 6520 6f66 2061 6374 6f72 0a20   name of actor. 
-00004900: 2020 2020 202d 206e 616d 653a 206e 756d       - name: num
-00004910: 5f6d 6f76 6965 730a 2020 2020 2020 2020  _movies.        
-00004920: 6465 7363 7269 7074 696f 6e3a 2054 6865  description: The
-00004930: 206e 756d 6265 7220 6f66 206d 6f76 6965   number of movie
-00004940: 7320 6163 746f 7220 6861 7320 6170 7065  s actor has appe
-00004950: 6172 6564 200a 2020 2020 2020 2d20 6e61  ared .      - na
-00004960: 6d65 3a20 6176 675f 7261 7469 6e67 0a20  me: avg_rating. 
-00004970: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00004980: 6f6e 3a20 4176 6572 6167 6520 7261 7469  on: Average rati
-00004990: 6e67 0a20 2020 2020 202d 206e 616d 653a  ng.      - name:
-000049a0: 2075 7064 6174 6564 5f61 740a 2020 2020   updated_at.    
-000049b0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-000049c0: 204c 6174 6573 7420 7570 6461 7465 2074   Latest update t
-000049d0: 696d 650a 6060 600a 5573 6520 6064 6274  ime.```.Use `dbt
-000049e0: 2064 6f63 7320 6765 6e65 7261 7465 6020   docs generate` 
-000049f0: 746f 2067 656e 6572 6174 6520 7468 6520  to generate the 
-00004a00: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
-00004a10: 7220 796f 7572 206d 6f64 656c 7320 2620  r your models & 
-00004a20: 6064 6274 2064 6f63 7320 7365 7276 6560  `dbt docs serve`
-00004a30: 2074 6f20 7365 7276 6520 7468 6520 646f   to serve the do
-00004a40: 6375 6d65 6e74 6174 696f 6e20 696e 200a  cumentation in .
-00004a50: 796f 7572 206c 6f63 616c 2062 726f 7773  your local brows
-00004a60: 6572 206f 6e20 706f 7274 2038 3030 302e  er on port 8000.
-00004a70: 0a21 5b44 6f63 5d28 2e2f 6578 616d 706c  .![Doc](./exampl
-00004a80: 6573 2f31 305f 646f 6373 2e70 6e67 290a  es/10_docs.png).
-00004a90: 2320 4c6f 6361 6c20 4465 7665 6c6f 706d  # Local Developm
-00004aa0: 656e 740a 5570 6461 7465 2060 7465 7374  ent.Update `test
-00004ab0: 732f 696e 7465 6772 6174 696f 6e2f 636f  s/integration/co
-00004ac0: 6e66 6573 742e 7079 6020 6669 6c65 2074  nfest.py` file t
-00004ad0: 6f20 696e 636c 7564 6520 796f 7572 2063  o include your c
-00004ae0: 6f6e 6e65 6374 696f 6e20 6372 6564 656e  onnection creden
-00004af0: 7469 616c 732e 2046 6f72 2072 756e 6e69  tials. For runni
-00004b00: 6e67 2074 6573 7473 206c 6f63 616c 6c79  ng tests locally
-00004b10: 2c20 666f 6c6c 6f77 200a 7468 6573 6520  , follow .these 
-00004b20: 7374 6570 733a 0a60 6060 636f 6d6d 616e  steps:.```comman
-00004b30: 646c 696e 650a 7069 7020 696e 7374 616c  dline.pip instal
-00004b40: 6c20 2d72 2064 6576 5f72 6571 7569 7265  l -r dev_require
-00004b50: 6d65 6e74 732e 7478 740a 7079 7468 6f6e  ments.txt.python
-00004b60: 202d 6d20 7079 7465 7374 0a60 6060 0a23   -m pytest.```.#
-00004b70: 204f 7269 6769 6e61 6c20 4175 7468 6f72   Original Author
-00004b80: 0a42 7974 6548 6f75 7365 2077 616e 7473  .ByteHouse wants
-00004b90: 2074 6f20 7468 616e 6b20 436c 6963 6b48   to thank ClickH
-00004ba0: 6f75 7365 2066 6f72 206f 7269 6769 6e61  ouse for origina
-00004bb0: 6c20 636f 6e74 7269 6275 7469 6f6e 2074  l contribution t
-00004bc0: 6f20 7468 6973 2063 6f6e 6e65 6374 6f72  o this connector
-00004bd0: 2e0a 0a23 204c 6963 656e 7365 0a54 6869  ...# License.Thi
-00004be0: 7320 7072 6f6a 6563 7420 6973 2064 6973  s project is dis
-00004bf0: 7472 6962 7574 6564 2075 6e64 6572 2074  tributed under t
-00004c00: 6865 2074 6572 6d73 206f 6620 7468 6520  he terms of the 
-00004c10: 4170 6163 6865 204c 6963 656e 7365 2028  Apache License (
-00004c20: 5665 7273 696f 6e20 322e 3029 2e         Version 2.0).
+00001ae0: 203c 7464 3e70 6173 7377 6f72 643c 2f74   <td>password</t
+00001af0: 643e 0a20 2020 2020 2020 203c 7464 3e42  d>.        <td>B
+00001b00: 7974 6548 6f75 7365 2041 5049 2054 6f6b  yteHouse API Tok
+00001b10: 656e 3c2f 7464 3e0a 2020 2020 3c2f 7472  en</td>.    </tr
+00001b20: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00001b30: 2020 203c 7464 3e64 7269 7665 723c 2f74     <td>driver</t
+00001b40: 643e 0a20 2020 2020 2020 203c 7464 3e4d  d>.        <td>M
+00001b50: 7573 7420 6265 2073 6574 2074 6f20 6e61  ust be set to na
+00001b60: 7469 7665 3c2f 7464 3e0a 2020 2020 3c2f  tive</td>.    </
+00001b70: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+00001b80: 2020 2020 203c 7464 3e68 6f73 743c 2f74       <td>host</t
+00001b90: 643e 0a20 2020 2020 2020 203c 7464 3e5b  d>.        <td>[
+00001ba0: 4f70 7469 6f6e 616c 5d20 5468 6520 686f  Optional] The ho
+00001bb0: 7374 206e 616d 6520 6f66 2074 6865 2063  st name of the c
+00001bc0: 6f6e 6e65 6374 696f 6e3c 2f74 643e 0a20  onnection</td>. 
+00001bd0: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+00001be0: 3e0a 2020 2020 2020 2020 3c74 643e 706f  >.        <td>po
+00001bf0: 7274 203c 2f74 643e 0a20 2020 2020 2020  rt </td>.       
+00001c00: 203c 7464 3e5b 4f70 7469 6f6e 616c 5d20   <td>[Optional] 
+00001c10: 5468 6520 706f 7274 206e 756d 6265 7220  The port number 
+00001c20: 6f66 2074 6865 2068 6f73 7420 7365 7276  of the host serv
+00001c30: 6572 3c2f 7464 3e0a 2020 2020 3c2f 7472  er</td>.    </tr
+00001c40: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00001c50: 2020 203c 7464 3e77 6172 6568 6f75 7365     <td>warehouse
+00001c60: 3c2f 7464 3e0a 2020 2020 2020 2020 3c74  </td>.        <t
+00001c70: 643e 5b4f 7074 696f 6e61 6c5d 2054 6865  d>[Optional] The
+00001c80: 206e 616d 6520 6f66 2074 6865 2076 6972   name of the vir
+00001c90: 7475 616c 2077 6172 6568 6f75 7365 2074  tual warehouse t
+00001ca0: 6861 7420 796f 7520 7761 6e74 2074 6f20  hat you want to 
+00001cb0: 7573 6520 666f 7220 7468 6973 2073 6573  use for this ses
+00001cc0: 7369 6f6e 3c2f 7464 3e0a 2020 2020 3c2f  sion</td>.    </
+00001cd0: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+00001ce0: 2020 2020 203c 7464 3e72 6574 7269 6573       <td>retries
+00001cf0: 3c2f 7464 3e0a 2020 2020 2020 2020 3c74  </td>.        <t
+00001d00: 643e 5b4f 7074 696f 6e61 6c5d 204e 756d  d>[Optional] Num
+00001d10: 6265 7220 6f66 2074 696d 6573 2074 6f20  ber of times to 
+00001d20: 7265 7472 7920 7468 6520 696e 6974 6961  retry the initia
+00001d30: 6c20 636f 6e6e 6563 7469 6f6e 2061 7474  l connection att
+00001d40: 656d 7074 2069 6620 7468 6520 6572 726f  empt if the erro
+00001d50: 7220 6170 7065 6172 7320 746f 2062 6520  r appears to be 
+00001d60: 7265 636f 7665 7261 626c 653c 2f74 643e  recoverable</td>
+00001d70: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+00001d80: 7472 3e0a 2020 2020 2020 2020 3c74 643e  tr>.        <td>
+00001d90: 7365 6375 7265 3c2f 7464 3e0a 2020 2020  secure</td>.    
+00001da0: 2020 2020 3c74 643e 5b4f 7074 696f 6e61      <td>[Optiona
+00001db0: 6c5d 2057 6865 7468 6572 2074 6865 2063  l] Whether the c
+00001dc0: 6f6e 6e65 6374 696f 6e20 6973 2073 6563  onnection is sec
+00001dd0: 7572 6564 2062 7920 544c 532e 2053 7567  ured by TLS. Sug
+00001de0: 6765 7374 6564 2074 6f20 7365 7420 6974  gested to set it
+00001df0: 2074 6f20 5472 7565 3c2f 7464 3e0a 2020   to True</td>.  
+00001e00: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+00001e10: 0a20 2020 2020 2020 203c 7464 3e63 6f6e  .        <td>con
+00001e20: 6e65 6374 5f74 696d 656f 7574 3c2f 7464  nect_timeout</td
+00001e30: 3e0a 2020 2020 2020 2020 3c74 643e 5b4f  >.        <td>[O
+00001e40: 7074 696f 6e61 6c5d 2043 6f6e 6e65 6374  ptional] Connect
+00001e50: 696f 6e20 7469 6d65 6f75 7420 696e 2073  ion timeout in s
+00001e60: 6563 6f6e 6473 2e20 4465 6661 756c 7420  econds. Default 
+00001e70: 6973 2031 3020 7365 636f 6e64 733c 2f74  is 10 seconds</t
+00001e80: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+00001e90: 203c 7472 3e0a 2020 2020 2020 2020 3c74   <tr>.        <t
+00001ea0: 643e 7365 6e64 5f72 6563 6569 7665 5f74  d>send_receive_t
+00001eb0: 696d 656f 7574 3c2f 7464 3e0a 2020 2020  imeout</td>.    
+00001ec0: 2020 2020 3c74 643e 5b4f 7074 696f 6e61      <td>[Optiona
+00001ed0: 6c5d 2054 696d 656f 7574 2066 6f72 2072  l] Timeout for r
+00001ee0: 6563 6569 7669 6e67 2064 6174 6120 6672  eceiving data fr
+00001ef0: 6f6d 206f 7220 7365 6e64 696e 6720 6461  om or sending da
+00001f00: 7461 2074 6f20 4279 7465 486f 7573 652e  ta to ByteHouse.
+00001f10: 2044 6566 6175 6c74 2069 7320 3520 6d69   Default is 5 mi
+00001f20: 6e75 7465 7320 2833 3030 2073 6563 6f6e  nutes (300 secon
+00001f30: 6473 293c 2f74 643e 0a20 2020 203c 2f74  ds)</td>.    </t
+00001f40: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+00001f50: 2020 2020 3c74 643e 6375 7374 6f6d 5f73      <td>custom_s
+00001f60: 6574 7469 6e67 733c 2f74 643e 0a20 2020  ettings</td>.   
+00001f70: 2020 2020 203c 7464 3e5b 4f70 7469 6f6e       <td>[Option
+00001f80: 616c 5d20 4120 6d61 7070 696e 6720 6f66  al] A mapping of
+00001f90: 2042 7974 6548 6f75 7365 2073 7065 6369   ByteHouse speci
+00001fa0: 6669 6320 7573 6572 2073 6574 7469 6e67  fic user setting
+00001fb0: 7320 746f 2075 7365 2077 6974 6820 7468  s to use with th
+00001fc0: 6520 636f 6e6e 6563 7469 6f6e 3c2f 7464  e connection</td
+00001fd0: 3e0a 2020 2020 3c2f 7472 3e0a 3c2f 7461  >.    </tr>.</ta
+00001fe0: 626c 653e 0a0a 2323 2043 6f6e 6e65 6374  ble>..## Connect
+00001ff0: 696f 6e20 2620 4175 7468 656e 7469 6361  ion & Authentica
+00002000: 7469 6f6e 2043 6f6e 6669 6775 7261 7469  tion Configurati
+00002010: 6f6e 730a 2323 2320 486f 7374 2041 6464  ons.### Host Add
+00002020: 7265 7373 2026 2041 5049 204b 6579 2043  ress & API Key C
+00002030: 6f6e 6669 6775 7261 7469 6f6e 0a52 6571  onfiguration.Req
+00002040: 7569 7265 6420 7061 7261 6d65 7465 7273  uired parameters
+00002050: 3a20 6068 6f73 7460 2060 706f 7274 6020  : `host` `port` 
+00002060: 6075 7365 7260 2060 7061 7373 776f 7264  `user` `password
+00002070: 600a 6060 6079 616d 6c0a 6279 7465 686f  `.```yaml.byteho
+00002080: 7573 655f 7072 6f66 696c 653a 0a20 2074  use_profile:.  t
+00002090: 6172 6765 743a 2064 6576 0a20 206f 7574  arget: dev.  out
+000020a0: 7075 7473 3a0a 2020 2020 6465 763a 0a20  puts:.    dev:. 
+000020b0: 2020 2020 2074 7970 653a 2062 7974 6568       type: byteh
+000020c0: 6f75 7365 0a20 2020 2020 2064 7269 7665  ouse.      drive
+000020d0: 723a 206e 6174 6976 650a 0a20 2020 2020  r: native..     
+000020e0: 2023 2064 6174 6162 6173 650a 2020 2020   # database.    
+000020f0: 2020 7363 6865 6d61 3a20 2444 4154 4142    schema: $DATAB
+00002100: 4153 455f 4e41 4d45 0a0a 2020 2020 2020  ASE_NAME..      
+00002110: 2320 7461 7267 6574 2073 6572 7665 7220  # target server 
+00002120: 6164 6472 6573 730a 2020 2020 2020 686f  address.      ho
+00002130: 7374 3a20 2448 4f53 545f 4144 4452 4553  st: $HOST_ADDRES
+00002140: 5320 200a 2020 2020 2020 706f 7274 3a20  S  .      port: 
+00002150: 2450 4f52 545f 4e55 4d42 4552 0a0a 2020  $PORT_NUMBER..  
+00002160: 2020 2020 2320 6163 636f 756e 7420 6372      # account cr
+00002170: 6564 656e 7469 616c 730a 2020 2020 2020  edentials.      
+00002180: 7573 6572 3a20 6279 7465 686f 7573 650a  user: bytehouse.
+00002190: 2020 2020 2020 7061 7373 776f 7264 3a20        password: 
+000021a0: 2441 5049 5f4b 4559 0a0a 2020 2020 2020  $API_KEY..      
+000021b0: 2320 6164 6469 7469 6f6e 616c 2073 6574  # additional set
+000021c0: 7469 6e67 730a 2020 2020 2020 7365 6375  tings.      secu
+000021d0: 7265 3a20 5472 7565 0a60 6060 0a23 2320  re: True.```.## 
+000021e0: 5072 6f6a 6563 7420 496e 6974 6961 6c69  Project Initiali
+000021f0: 7a61 7469 6f6e 0a60 6462 7420 696e 6974  zation.`dbt init
+00002200: 6020 636f 6d6d 616e 6420 7769 6c6c 2070  ` command will p
+00002210: 726f 6d70 7420 666f 7220 7072 6f6a 6563  rompt for projec
+00002220: 7420 6e61 6d65 2026 2064 6174 6162 6173  t name & databas
+00002230: 6520 6164 6170 7465 7273 2c20 7768 6572  e adapters, wher
+00002240: 6520 796f 7520 6861 7665 2074 6f20 7365  e you have to se
+00002250: 6c65 6374 2062 7974 6568 6f75 7365 2e20  lect bytehouse. 
+00002260: 5468 6973 2077 696c 6c20 6372 6561 7465  This will create
+00002270: 0a61 206e 6577 2066 6f6c 6465 7220 7769  .a new folder wi
+00002280: 7468 2079 6f75 7220 7072 6f6a 6563 7420  th your project 
+00002290: 6e61 6d65 2c20 7361 6d70 6c65 2066 696c  name, sample fil
+000022a0: 6573 2026 2060 6462 745f 7072 6f6a 6563  es & `dbt_projec
+000022b0: 742e 796d 6c60 2063 6f6e 6669 6720 6669  t.yml` config fi
+000022c0: 6c65 2c20 656e 6f75 6768 2074 6f20 6765  le, enough to ge
+000022d0: 7420 796f 7520 7374 6172 7465 6420 7769  t you started wi
+000022e0: 7468 2064 6274 2e0a 6060 6063 6f6d 6d61  th dbt..```comma
+000022f0: 6e64 6c69 6e65 0a64 6274 2069 6e69 740a  ndline.dbt init.
+00002300: 6060 600a 215b 496e 6974 5d28 2e2f 6578  ```.![Init](./ex
+00002310: 616d 706c 6573 2f32 5f70 726f 6669 6c65  amples/2_profile
+00002320: 732e 706e 6729 0a55 7064 6174 6520 796f  s.png).Update yo
+00002330: 7572 2070 726f 6669 6c65 732e 796d 6c20  ur profiles.yml 
+00002340: 7769 7468 2072 6571 7569 7265 6420 6175  with required au
+00002350: 7468 656e 7469 6361 7469 6f6e 2026 2074  thentication & t
+00002360: 6172 6765 7420 7365 7276 6572 2063 7265  arget server cre
+00002370: 6465 6e74 6961 6c73 2e20 0a60 6060 636f  dentials. .```co
+00002380: 6d6d 616e 646c 696e 650a 6e61 6e6f 207e  mmandline.nano ~
+00002390: 2f2e 6462 742f 7072 6f66 696c 6573 2e79  /.dbt/profiles.y
+000023a0: 6d6c 0a60 6060 0a41 7320 6064 6274 6020  ml.```.As `dbt` 
+000023b0: 6861 7320 6372 6561 7465 6420 6120 6e65  has created a ne
+000023c0: 7720 666f 6c64 6572 2077 6974 6820 7468  w folder with th
+000023d0: 6520 7361 6d65 206e 616d 6520 6173 2079  e same name as y
+000023e0: 6f75 7220 7072 6f6a 6563 7420 6e61 6d65  our project name
+000023f0: 2c20 6368 616e 6765 2079 6f75 7220 6375  , change your cu
+00002400: 7272 656e 7420 0a64 6972 6563 746f 7279  rrent .directory
+00002410: 2074 6f20 7468 6520 7072 6f6a 6563 7420   to the project 
+00002420: 666f 6c64 6572 2e20 0a60 6060 636f 6d6d  folder. .```comm
+00002430: 616e 646c 696e 650a 6364 2064 6274 5f62  andline.cd dbt_b
+00002440: 7974 6568 6f75 7365 5f64 656d 6f0a 6060  ytehouse_demo.``
+00002450: 600a 5570 6461 7465 2079 6f75 7220 6064  `.Update your `d
+00002460: 6274 5f70 726f 6a65 6374 2e79 6d6c 6020  bt_project.yml` 
+00002470: 6669 6c65 2074 6f20 6861 7665 2074 6865  file to have the
+00002480: 2073 616d 6520 7072 6f66 696c 655f 6e61   same profile_na
+00002490: 6d65 2061 7320 607e 2f2e 6462 742f 7072  me as `~/.dbt/pr
+000024a0: 6f66 696c 6573 2e79 6d6c 602e 0a60 6060  ofiles.yml`..```
+000024b0: 636f 6d6d 616e 646c 696e 650a 6e61 6e6f  commandline.nano
+000024c0: 2064 6274 5f70 726f 6a65 6374 2e79 6d6c   dbt_project.yml
+000024d0: 0a60 6060 0a21 5b50 726f 6a65 6374 5d28  .```.![Project](
+000024e0: 2e2f 6578 616d 706c 6573 2f33 5f70 726f  ./examples/3_pro
+000024f0: 6a65 6374 2e70 6e67 290a 2323 2054 6573  ject.png).## Tes
+00002500: 7420 5761 7265 686f 7573 6520 436f 6e6e  t Warehouse Conn
+00002510: 6563 7469 6f6e 0a55 7365 2060 6462 7420  ection.Use `dbt 
+00002520: 6465 6275 6760 2063 6f6d 6d61 6e64 2074  debug` command t
+00002530: 6f20 7665 7269 6679 2072 6571 7569 7265  o verify require
+00002540: 6420 6465 7065 6e64 656e 6369 6573 2026  d dependencies &
+00002550: 2077 6172 6568 6f75 7365 2063 6f6e 6e65   warehouse conne
+00002560: 6374 696f 6e2e 2049 6e20 6361 7365 206f  ction. In case o
+00002570: 6620 7375 6363 6573 732c 2069 7420 7769  f success, it wi
+00002580: 6c6c 2073 686f 7720 796f 7520 0a22 416c  ll show you ."Al
+00002590: 6c20 6368 6563 6b73 2070 6173 7365 6421  l checks passed!
+000025a0: 220a 6060 6063 6f6d 6d61 6e64 6c69 6e65  ".```commandline
+000025b0: 0a64 6274 2064 6562 7567 0a60 6060 0a21  .dbt debug.```.!
+000025c0: 5b44 6562 7567 5d28 2e2f 6578 616d 706c  [Debug](./exampl
+000025d0: 6573 2f34 5f64 6562 7567 2e70 6e67 290a  es/4_debug.png).
+000025e0: 2320 4461 7461 7365 7420 496e 6765 7374  # Dataset Ingest
+000025f0: 696f 6e0a 546f 2073 686f 7763 6173 6520  ion.To showcase 
+00002600: 6469 6666 6572 656e 7420 6064 6274 6020  different `dbt` 
+00002610: 6675 6e63 7469 6f6e 616c 6974 6965 732c  functionalities,
+00002620: 2077 6520 7769 6c6c 2069 6e67 6573 7420   we will ingest 
+00002630: 6120 736d 616c 6c20 696d 6462 206d 6f76  a small imdb mov
+00002640: 6965 2064 6174 6173 6574 2c20 7769 7468  ie dataset, with
+00002650: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
+00002660: 6368 656d 612e 200a 5468 6520 4444 4c20  chema. .The DDL 
+00002670: 2620 696e 7365 7274 696f 6e20 7175 6572  & insertion quer
+00002680: 6965 7320 6361 6e20 6265 2066 6f75 6e64  ies can be found
+00002690: 2068 6572 6520 6874 7470 733a 2f2f 6769   here https://gi
+000026a0: 7468 7562 2e63 6f6d 2f62 7974 6568 6f75  thub.com/bytehou
+000026b0: 7365 2d63 6c6f 7564 2f62 7974 6568 6f75  se-cloud/bytehou
+000026c0: 7365 2d64 6274 2f65 7861 6d70 6c65 732f  se-dbt/examples/
+000026d0: 6461 7461 5f6c 6f61 6469 6e67 2e73 716c  data_loading.sql
+000026e0: 2e20 0a59 6f75 2063 616e 2075 7365 2042  . .You can use B
+000026f0: 7974 6548 6f75 7365 2053 514c 2077 6f72  yteHouse SQL wor
+00002700: 6b73 6865 6574 2074 6f20 6372 6561 7465  ksheet to create
+00002710: 2074 6865 2073 6368 656d 6120 2620 696e   the schema & in
+00002720: 7365 7274 2074 6865 2064 6174 6173 6574  sert the dataset
+00002730: 2e20 0a21 5b53 6368 656d 615d 282e 2f65  . .![Schema](./e
+00002740: 7861 6d70 6c65 732f 355f 7363 6865 6d61  xamples/5_schema
+00002750: 2e70 6e67 290a 546f 2076 6572 6966 7920  .png).To verify 
+00002760: 7468 6174 2064 6174 6173 6574 2070 7265  that dataset pre
+00002770: 7061 7261 7469 6f6e 2077 6173 2073 7563  paration was suc
+00002780: 6365 7373 6675 6c2c 2077 6520 7769 6c6c  cessful, we will
+00002790: 2065 7865 6375 7465 2074 6869 7320 666f   execute this fo
+000027a0: 6c6c 6f77 696e 6720 7175 6572 7920 746f  llowing query to
+000027b0: 2073 756d 6d61 7269 7a65 2065 6163 6820   summarize each 
+000027c0: 6163 746f 7220 616c 6f6e 6720 0a77 6974  actor along .wit
+000027d0: 6820 7468 6569 7220 746f 7461 6c20 6e75  h their total nu
+000027e0: 6d62 6572 206f 6620 6d6f 7669 6520 6170  mber of movie ap
+000027f0: 7065 6172 616e 6365 732e 200a 6060 600a  pearances. .```.
+00002800: 5345 4c45 4354 2069 642c 0a20 2061 6e79  SELECT id,.  any
+00002810: 2861 6374 6f72 5f6e 616d 6529 2061 7320  (actor_name) as 
+00002820: 6e61 6d65 2c0a 2020 756e 6971 4578 6163  name,.  uniqExac
+00002830: 7428 6d6f 7669 655f 6964 2920 2020 2061  t(movie_id)    a
+00002840: 7320 6e75 6d5f 6d6f 7669 6573 2c0a 2020  s num_movies,.  
+00002850: 6176 6728 7261 7469 6e67 2920 2020 2020  avg(rating)     
+00002860: 2020 2020 2020 2020 2020 2061 7320 6176             as av
+00002870: 675f 7261 7469 6e67 2c0a 2020 6d61 7828  g_rating,.  max(
+00002880: 6372 6561 7465 645f 6174 2920 6173 2075  created_at) as u
+00002890: 7064 6174 6564 5f61 740a 4652 4f4d 2028  pdated_at.FROM (
+000028a0: 0a20 2053 454c 4543 5420 6163 746f 7273  .  SELECT actors
+000028b0: 2e69 6420 6173 2069 642c 0a20 2020 2020  .id as id,.     
+000028c0: 2020 636f 6e63 6174 2861 6374 6f72 732e    concat(actors.
+000028d0: 6669 7273 745f 6e61 6d65 2c20 2720 272c  first_name, ' ',
+000028e0: 2061 6374 6f72 732e 6c61 7374 5f6e 616d   actors.last_nam
+000028f0: 6529 2061 7320 6163 746f 725f 6e61 6d65  e) as actor_name
+00002900: 2c0a 2020 2020 2020 206d 6f76 6965 732e  ,.       movies.
+00002910: 6964 2061 7320 6d6f 7669 655f 6964 2c0a  id as movie_id,.
+00002920: 2020 2020 2020 206d 6f76 6965 732e 7261         movies.ra
+00002930: 7469 6e67 2061 7320 7261 7469 6e67 2c0a  ting as rating,.
+00002940: 2020 2020 2020 2063 7265 6174 6564 5f61         created_a
+00002950: 740a 2020 4652 4f4d 2020 696d 6462 2e61  t.  FROM  imdb.a
+00002960: 6374 6f72 730a 2020 2020 2020 2020 4a4f  ctors.        JO
+00002970: 494e 2069 6d64 622e 726f 6c65 7320 4f4e  IN imdb.roles ON
+00002980: 2072 6f6c 6573 2e61 6374 6f72 5f69 6420   roles.actor_id 
+00002990: 3d20 6163 746f 7273 2e69 640a 2020 2020  = actors.id.    
+000029a0: 2020 2020 4c45 4654 204f 5554 4552 204a      LEFT OUTER J
+000029b0: 4f49 4e20 696d 6462 2e6d 6f76 6965 7320  OIN imdb.movies 
+000029c0: 4f4e 206d 6f76 6965 732e 6964 203d 2072  ON movies.id = r
+000029d0: 6f6c 6573 2e6d 6f76 6965 5f69 640a 290a  oles.movie_id.).
+000029e0: 4752 4f55 5020 4259 2069 640a 6060 600a  GROUP BY id.```.
+000029f0: 5468 6520 7265 7375 6c74 7365 7420 7368  The resultset sh
+00002a00: 6f75 6c64 2062 6520 6c69 6b65 2074 6869  ould be like thi
+00002a10: 733a 0a21 5b53 6368 656d 6120 436f 6e66  s:.![Schema Conf
+00002a20: 6972 6d5d 282e 2f65 7861 6d70 6c65 732f  irm](./examples/
+00002a30: 365f 7363 6865 6d61 5f63 6f6e 6669 726d  6_schema_confirm
+00002a40: 2e70 6e67 290a 2320 6462 7420 4d6f 6465  .png).# dbt Mode
+00002a50: 6c73 200a 496e 2061 2060 6462 7460 2070  ls .In a `dbt` p
+00002a60: 726f 6a65 6374 2c20 6120 6d6f 6465 6c20  roject, a model 
+00002a70: 6973 2061 2073 716c 2066 696c 6520 6c6f  is a sql file lo
+00002a80: 6361 7465 6420 696e 7369 6465 2060 6d6f  cated inside `mo
+00002a90: 6465 6c73 2f60 2064 6972 6563 746f 7279  dels/` directory
+00002aa0: 2077 6869 6368 2077 696c 6c20 636f 6e74   which will cont
+00002ab0: 6169 6e20 6120 6053 454c 4543 5460 2073  ain a `SELECT` s
+00002ac0: 7461 7465 6d65 6e74 200a 7265 6665 7272  tatement .referr
+00002ad0: 696e 6720 746f 2061 2074 7261 6e73 666f  ing to a transfo
+00002ae0: 726d 6174 696f 6e2e 2054 6865 206e 616d  rmation. The nam
+00002af0: 6520 6f66 2074 6865 206d 6f64 656c 2066  e of the model f
+00002b00: 696c 6520 7769 6c6c 2072 6566 6572 2074  ile will refer t
+00002b10: 6f20 7468 6520 6e61 6d65 206f 6620 6675  o the name of fu
+00002b20: 7475 7265 2074 6162 6c65 2f76 6965 7720  ture table/view 
+00002b30: 6166 7465 720a 6064 6274 6020 6578 6563  after.`dbt` exec
+00002b40: 7574 696f 6e2e 2057 6865 6e20 7765 2065  ution. When we e
+00002b50: 7865 6375 7465 2060 6462 7420 7275 6e60  xecute `dbt run`
+00002b60: 2063 6f6d 6d61 6e64 2c20 6064 6274 6020   command, `dbt` 
+00002b70: 7769 6c6c 2062 7569 6c64 2074 6869 7320  will build this 
+00002b80: 6d6f 6465 6c20 6469 7265 6374 6c79 2069  model directly i
+00002b90: 6e74 6f20 4279 7465 486f 7573 6520 6279  nto ByteHouse by
+00002ba0: 2077 7261 7070 696e 670a 6974 2069 6e20   wrapping.it in 
+00002bb0: 6120 6372 6561 7465 2074 6162 6c65 202f  a create table /
+00002bc0: 2076 6965 7720 6d61 7465 7269 616c 697a   view materializ
+00002bd0: 6174 696f 6e2e 204d 6174 6572 6961 6c69  ation. Materiali
+00002be0: 7a61 7469 6f6e 2074 7970 6520 6f66 2079  zation type of y
+00002bf0: 6f75 7220 6d6f 6465 6c20 7769 6c6c 2064  our model will d
+00002c00: 6574 6572 6d69 6e65 2074 6865 2061 6374  etermine the act
+00002c10: 7561 6c20 5351 4c0a 7468 6174 2060 6462  ual SQL.that `db
+00002c20: 7460 2077 696c 6c20 7573 6520 746f 2063  t` will use to c
+00002c30: 7265 6174 6520 6d6f 6465 6c20 696e 2074  reate model in t
+00002c40: 6865 2077 6172 6568 6f75 7365 2e0a 2320  he warehouse..# 
+00002c50: 7363 6865 6d61 2e79 6d6c 0a54 6865 2060  schema.yml.The `
+00002c60: 7363 6865 6d61 2e79 6d6c 6020 6669 6c65  schema.yml` file
+00002c70: 2077 696c 6c20 6465 6669 6e65 206f 7572   will define our
+00002c80: 2074 6162 6c65 7320 2620 636f 6c75 6d6e   tables & column
+00002c90: 7320 6279 2072 6566 6572 7269 6e67 2074  s by referring t
+00002ca0: 6872 6f75 6768 2061 6c69 6173 206e 616d  hrough alias nam
+00002cb0: 652e 2054 6869 7320 7363 6865 6d61 7320  e. This schemas 
+00002cc0: 6361 6e20 6c61 7465 7220 6265 0a75 7365  can later be.use
+00002cd0: 6420 696e 2064 6966 6665 7265 6e74 206d  d in different m
+00002ce0: 6f64 656c 732f 6d61 6372 6f73 2076 6961  odels/macros via
+00002cf0: 2060 736f 7572 6365 2829 6020 6675 6e63   `source()` func
+00002d00: 7469 6f6e 2e0a 4372 6561 7465 2060 7363  tion..Create `sc
+00002d10: 6865 6d61 2e79 6d6c 6020 6669 6c65 2075  hema.yml` file u
+00002d20: 6e64 6572 2060 6d6f 6465 6c73 2f60 2064  nder `models/` d
+00002d30: 6972 6563 746f 7279 0a60 6060 636f 6d6d  irectory.```comm
+00002d40: 616e 646c 696e 650a 746f 7563 6820 6d6f  andline.touch mo
+00002d50: 6465 6c73 2f73 6368 656d 612e 796d 6c0a  dels/schema.yml.
+00002d60: 6060 600a 4465 6669 6e65 206f 7572 206d  ```.Define our m
+00002d70: 6f64 656c 2073 6368 656d 6120 6c69 6b65  odel schema like
+00002d80: 2074 6869 730a 6060 6079 616d 6c0a 7665   this.```yaml.ve
+00002d90: 7273 696f 6e3a 2032 0a0a 736f 7572 6365  rsion: 2..source
+00002da0: 733a 0a2d 206e 616d 653a 2069 6d64 620a  s:.- name: imdb.
+00002db0: 2020 7461 626c 6573 3a0a 2020 2d20 6e61    tables:.  - na
+00002dc0: 6d65 3a20 6163 746f 7273 0a20 202d 206e  me: actors.  - n
+00002dd0: 616d 653a 2072 6f6c 6573 0a20 202d 206e  ame: roles.  - n
+00002de0: 616d 653a 206d 6f76 6965 730a 6060 600a  ame: movies.```.
+00002df0: 2320 4d61 7465 7269 616c 697a 6174 696f  # Materializatio
+00002e00: 6e20 7479 7065 7320 6f66 204d 6f64 656c  n types of Model
+00002e10: 730a 2323 2056 6965 7720 4d61 7465 7269  s.## View Materi
+00002e20: 616c 697a 6174 696f 6e73 0a49 6e20 6361  alizations.In ca
+00002e30: 7365 206f 6620 7669 6577 206d 6174 6572  se of view mater
+00002e40: 6961 6c69 7a61 7469 6f6e 2c20 6120 6d6f  ialization, a mo
+00002e50: 6465 6c20 6973 2074 7261 6e73 666f 726d  del is transform
+00002e60: 6564 2074 6f20 6120 7669 6577 206f 6e20  ed to a view on 
+00002e70: 6561 6368 2073 696e 676c 6520 7275 6e20  each single run 
+00002e80: 6279 2060 4352 4541 5445 2056 4945 5760  by `CREATE VIEW`
+00002e90: 2041 5320 7374 6174 656d 656e 7420 696e   AS statement in
+00002ea0: 200a 4279 7465 486f 7573 652e 2056 6965   .ByteHouse. Vie
+00002eb0: 7720 6d61 7465 7269 616c 697a 6174 696f  w materializatio
+00002ec0: 6e73 2077 6f6e 2774 2073 746f 7265 2074  ns won't store t
+00002ed0: 6865 2061 6374 7561 6c20 6461 7461 2c20  he actual data, 
+00002ee0: 736f 2069 7420 776f 756c 6420 6265 2073  so it would be s
+00002ef0: 6c6f 7765 7220 746f 2071 7565 7279 2074  lower to query t
+00002f00: 6861 6e20 7461 626c 6520 6d61 7465 7269  han table materi
+00002f10: 616c 697a 6174 696f 6e73 2e0a 4c65 7427  alizations..Let'
+00002f20: 7320 6372 6561 7465 2060 6d6f 6465 6c73  s create `models
+00002f30: 2f61 6374 6f72 5f69 6e73 6967 6874 2e73  /actor_insight.s
+00002f40: 716c 6020 6173 2076 6965 7720 6d61 7465  ql` as view mate
+00002f50: 7269 616c 697a 6174 696f 6e2e 200a 6060  rialization. .``
+00002f60: 6063 6f6d 6d61 6e64 6c69 6e65 0a74 6f75  `commandline.tou
+00002f70: 6368 206d 6f64 656c 732f 6163 746f 7273  ch models/actors
+00002f80: 5f69 6e73 6967 6874 2e73 716c 0a60 6060  _insight.sql.```
+00002f90: 0a60 6060 0a7b 7b20 636f 6e66 6967 286d  .```.{{ config(m
+00002fa0: 6174 6572 6961 6c69 7a65 643d 2776 6965  aterialized='vie
+00002fb0: 7727 2920 7d7d 0a0a 5345 4c45 4354 2069  w') }}..SELECT i
+00002fc0: 642c 0a20 2061 6e79 2861 6374 6f72 5f6e  d,.  any(actor_n
+00002fd0: 616d 6529 2061 7320 6e61 6d65 2c0a 2020  ame) as name,.  
+00002fe0: 756e 6971 4578 6163 7428 6d6f 7669 655f  uniqExact(movie_
+00002ff0: 6964 2920 2020 2061 7320 6e75 6d5f 6d6f  id)    as num_mo
+00003000: 7669 6573 2c0a 2020 6176 6728 7261 7469  vies,.  avg(rati
+00003010: 6e67 2920 2020 2020 2020 2020 2020 2020  ng)             
+00003020: 2020 2061 7320 6176 675f 7261 7469 6e67     as avg_rating
+00003030: 2c0a 2020 6d61 7828 6372 6561 7465 645f  ,.  max(created_
+00003040: 6174 2920 6173 2075 7064 6174 6564 5f61  at) as updated_a
+00003050: 740a 4652 4f4d 2028 0a20 2053 454c 4543  t.FROM (.  SELEC
+00003060: 5420 6163 746f 7273 2e69 6420 6173 2069  T actors.id as i
+00003070: 642c 0a20 2020 2020 2020 636f 6e63 6174  d,.       concat
+00003080: 2861 6374 6f72 732e 6669 7273 745f 6e61  (actors.first_na
+00003090: 6d65 2c20 2720 272c 2061 6374 6f72 732e  me, ' ', actors.
+000030a0: 6c61 7374 5f6e 616d 6529 2061 7320 6163  last_name) as ac
+000030b0: 746f 725f 6e61 6d65 2c0a 2020 2020 2020  tor_name,.      
+000030c0: 206d 6f76 6965 732e 6964 2061 7320 6d6f   movies.id as mo
+000030d0: 7669 655f 6964 2c0a 2020 2020 2020 206d  vie_id,.       m
+000030e0: 6f76 6965 732e 7261 7469 6e67 2061 7320  ovies.rating as 
+000030f0: 7261 7469 6e67 2c0a 2020 2020 2020 2063  rating,.       c
+00003100: 7265 6174 6564 5f61 740a 2020 4652 4f4d  reated_at.  FROM
+00003110: 2020 7b7b 2073 6f75 7263 6528 2769 6d64    {{ source('imd
+00003120: 6227 2c20 2761 6374 6f72 7327 2920 7d7d  b', 'actors') }}
+00003130: 0a20 2020 2020 2020 204a 4f49 4e20 7b7b  .        JOIN {{
+00003140: 2073 6f75 7263 6528 2769 6d64 6227 2c20   source('imdb', 
+00003150: 2772 6f6c 6573 2729 207d 7d20 4f4e 2072  'roles') }} ON r
+00003160: 6f6c 6573 2e61 6374 6f72 5f69 6420 3d20  oles.actor_id = 
+00003170: 6163 746f 7273 2e69 640a 2020 2020 2020  actors.id.      
+00003180: 2020 4c45 4654 204f 5554 4552 204a 4f49    LEFT OUTER JOI
+00003190: 4e20 7b7b 2073 6f75 7263 6528 2769 6d64  N {{ source('imd
+000031a0: 6227 2c20 276d 6f76 6965 7327 2920 7d7d  b', 'movies') }}
+000031b0: 204f 4e20 6d6f 7669 6573 2e69 6420 3d20   ON movies.id = 
+000031c0: 726f 6c65 732e 6d6f 7669 655f 6964 0a29  roles.movie_id.)
+000031d0: 0a47 524f 5550 2042 5920 6964 0a60 6060  .GROUP BY id.```
+000031e0: 0a4c 6574 2773 2065 7865 6375 7465 2060  .Let's execute `
+000031f0: 6462 7420 7275 6e60 2063 6f6d 6d61 6e64  dbt run` command
+00003200: 2074 6f20 6275 696c 6420 7468 6973 206d   to build this m
+00003210: 6f64 656c 2069 6e20 4279 7465 486f 7573  odel in ByteHous
+00003220: 652e 200a 215b 436f 6e66 6972 6d5d 282e  e. .![Confirm](.
+00003230: 2f65 7861 6d70 6c65 732f 375f 6163 746f  /examples/7_acto
+00003240: 725f 696e 7369 6768 745f 636f 6e66 6972  r_insight_confir
+00003250: 6d2e 706e 6729 0a51 7565 7279 696e 6720  m.png).Querying 
+00003260: 7468 6973 2076 6965 772c 2077 6520 6361  this view, we ca
+00003270: 6e20 7265 706c 6963 6174 6520 7468 6520  n replicate the 
+00003280: 7265 7375 6c74 7320 6f66 206f 7572 2065  results of our e
+00003290: 6172 6c69 6572 2071 7565 7279 2077 6974  arlier query wit
+000032a0: 6820 6120 7369 6d70 6c65 7220 7379 6e74  h a simpler synt
+000032b0: 6178 3a0a 6060 600a 5345 4c45 4354 202a  ax:.```.SELECT *
+000032c0: 2046 524f 4d20 696d 6462 2e61 6374 6f72   FROM imdb.actor
+000032d0: 735f 696e 7369 6768 7420 4f52 4445 5220  s_insight ORDER 
+000032e0: 4259 206e 756d 5f6d 6f76 6965 7320 4445  BY num_movies DE
+000032f0: 5343 3b0a 6060 600a 215b 436f 6e66 6972  SC;.```.![Confir
+00003300: 6d32 5d28 2e2f 6578 616d 706c 6573 2f38  m2](./examples/8
+00003310: 5f6d 6174 6572 6961 6c69 7a65 645f 7669  _materialized_vi
+00003320: 6577 5f72 756e 5f63 6f6e 6669 726d 2e70  ew_run_confirm.p
+00003330: 6e67 290a 2323 2054 6162 6c65 204d 6174  ng).## Table Mat
+00003340: 6572 6961 6c69 7a61 7469 6f6e 730a 496e  erializations.In
+00003350: 2063 6173 6520 6f66 2074 6162 6c65 206d   case of table m
+00003360: 6174 6572 6961 6c69 7a61 7469 6f6e 2c20  aterialization, 
+00003370: 796f 7572 206d 6f64 656c 2077 6f75 6c64  your model would
+00003380: 2062 6520 7265 6275 696c 7420 6173 2061   be rebuilt as a
+00003390: 2074 6162 6c65 206f 6e20 6561 6368 2073   table on each s
+000033a0: 696e 676c 6520 6064 6274 2072 756e 6020  ingle `dbt run` 
+000033b0: 0a76 6961 2061 2060 4352 4541 5445 2054  .via a `CREATE T
+000033c0: 4142 4c45 6020 4153 2073 7461 7465 6d65  ABLE` AS stateme
+000033d0: 6e74 2e20 0a60 6060 636f 6d6d 616e 646c  nt. .```commandl
+000033e0: 696e 650a 746f 7563 6820 6d6f 6465 6c73  ine.touch models
+000033f0: 2f61 6374 6f72 735f 696e 7369 6768 745f  /actors_insight_
+00003400: 7461 626c 652e 7371 6c0a 6060 600a 5765  table.sql.```.We
+00003410: 2063 616e 2075 7365 206f 7572 2070 7265   can use our pre
+00003420: 7669 6f75 7320 7669 6577 206d 6174 6572  vious view mater
+00003430: 6961 6c69 7a61 7469 6f6e 2073 716c 2077  ialization sql w
+00003440: 6974 6820 636f 6e66 6967 2063 6861 6e67  ith config chang
+00003450: 6520 666f 7220 7461 626c 6520 6d61 7465  e for table mate
+00003460: 7269 616c 697a 6174 696f 6e20 7371 6c2e  rialization sql.
+00003470: 200a 6060 600a 7b7b 2063 6f6e 6669 6728   .```.{{ config(
+00003480: 6f72 6465 725f 6279 3d27 2875 7064 6174  order_by='(updat
+00003490: 6564 5f61 742c 2069 642c 206e 616d 6529  ed_at, id, name)
+000034a0: 272c 206d 6174 6572 6961 6c69 7a65 643d  ', materialized=
+000034b0: 2774 6162 6c65 2729 207d 7d0a 6060 600a  'table') }}.```.
+000034c0: 5765 2063 616e 2076 6572 6966 7920 7468  We can verify th
+000034d0: 6174 2062 6f74 6820 7669 6577 2026 2074  at both view & t
+000034e0: 6162 6c65 206d 6174 6572 6961 6c69 7a61  able materializa
+000034f0: 7469 6f6e 7320 6765 6e65 7261 7465 2074  tions generate t
+00003500: 6865 2073 616d 6520 7265 7370 6f6e 7365  he same response
+00003510: 2e20 0a60 6060 0a20 5345 4c45 4354 202a  . .```. SELECT *
+00003520: 2046 524f 4d20 696d 6462 2e61 6374 6f72   FROM imdb.actor
+00003530: 735f 696e 7369 6768 745f 7461 626c 6520  s_insight_table 
+00003540: 4f52 4445 5220 4259 206e 756d 5f6d 6f76  ORDER BY num_mov
+00003550: 6965 7320 4445 5343 3b0a 6060 600a 2323  ies DESC;.```.##
+00003560: 2049 6e63 7265 6d65 6e74 616c 204d 6174   Incremental Mat
+00003570: 6572 6961 6c69 7a61 7469 6f6e 730a 466f  erializations.Fo
+00003580: 7220 6f75 7220 7072 6576 696f 7573 2074  r our previous t
+00003590: 6162 6c65 206d 6174 6572 6961 6c69 7a61  able materializa
+000035a0: 7469 6f6e 2c20 6064 6274 6020 7769 6c6c  tion, `dbt` will
+000035b0: 2063 6f6e 7374 7275 6374 2061 2074 6162   construct a tab
+000035c0: 6c65 2065 7665 7279 2074 696d 6520 746f  le every time to
+000035d0: 206d 6174 6572 6961 6c69 7a65 2074 6865   materialize the
+000035e0: 206d 6f64 656c 2e20 466f 7220 6c61 7267   model. For larg
+000035f0: 6572 0a6f 7220 636f 6d70 6c65 7820 7472  er.or complex tr
+00003600: 616e 7366 6f72 6d61 7469 6f6e 732c 2074  ansformations, t
+00003610: 6869 7320 776f 756c 6420 6265 2072 6564  his would be red
+00003620: 756e 6461 6e74 2061 6e64 2063 6f73 746c  undant and costl
+00003630: 7920 696e 2074 6572 6d73 206f 6620 636f  y in terms of co
+00003640: 6d70 7574 696e 6720 706f 7765 722e 2049  mputing power. I
+00003650: 6e63 7265 6d65 6e74 616c 200a 6d61 7465  ncremental .mate
+00003660: 7269 616c 697a 6174 696f 6e73 2073 6f6c  rializations sol
+00003670: 7665 2074 6869 7320 7072 6f62 6c65 6d2e  ve this problem.
+00003680: 3c62 722f 3e0a 5468 6520 6669 7273 7420  <br/>.The first 
+00003690: 7469 6d65 2061 206d 6f64 656c 2069 7320  time a model is 
+000036a0: 7275 6e2c 2074 6865 2074 6162 6c65 2069  run, the table i
+000036b0: 7320 6275 696c 7420 6279 2074 7261 6e73  s built by trans
+000036c0: 666f 726d 696e 6720 616c 6c20 726f 7773  forming all rows
+000036d0: 206f 6620 736f 7572 6365 2064 6174 612e   of source data.
+000036e0: 204f 6e20 7375 6273 6571 7565 6e74 2072   On subsequent r
+000036f0: 756e 732c 200a 6064 6274 6020 7472 616e  uns, .`dbt` tran
+00003700: 7366 6f72 6d73 206f 6e6c 7920 7468 6520  sforms only the 
+00003710: 726f 7773 2069 6e20 796f 7572 2073 6f75  rows in your sou
+00003720: 7263 6520 6461 7461 2074 6861 7420 796f  rce data that yo
+00003730: 7520 7465 6c6c 2060 6462 7460 2074 6f20  u tell `dbt` to 
+00003740: 6669 6c74 6572 2066 6f72 2c20 696e 7365  filter for, inse
+00003750: 7274 696e 6720 7468 656d 2069 6e74 6f20  rting them into 
+00003760: 7468 6520 7461 7267 6574 200a 7461 626c  the target .tabl
+00003770: 6520 7768 6963 6820 6973 2074 6865 2074  e which is the t
+00003780: 6162 6c65 2074 6861 7420 6861 7320 616c  able that has al
+00003790: 7265 6164 7920 6265 656e 2062 7569 6c74  ready been built
+000037a0: 2e3c 6272 2f3e 0a54 6f20 7465 6c6c 2060  .<br/>.To tell `
+000037b0: 6462 7460 2077 6869 6368 2072 6f77 7320  dbt` which rows 
+000037c0: 6974 2073 686f 756c 6420 7472 616e 7366  it should transf
+000037d0: 6f72 6d20 6f6e 2061 6e20 696e 6372 656d  orm on an increm
+000037e0: 656e 7461 6c20 7275 6e2c 2077 7261 7020  ental run, wrap 
+000037f0: 7661 6c69 6420 5351 4c20 7468 6174 2066  valid SQL that f
+00003800: 696c 7465 7273 2066 6f72 2074 6865 7365  ilters for these
+00003810: 2072 6f77 7320 0a69 6e20 7468 6520 6069   rows .in the `i
+00003820: 735f 696e 6372 656d 656e 7461 6c28 2960  s_incremental()`
+00003830: 206d 6163 726f 2e20 596f 7572 2060 6973   macro. Your `is
+00003840: 5f69 6e63 7265 6d65 6e74 616c 2829 6020  _incremental()` 
+00003850: 636f 6465 2077 696c 6c20 6368 6563 6b20  code will check 
+00003860: 666f 7220 726f 7773 2063 7265 6174 6564  for rows created
+00003870: 206f 7220 6d6f 6469 6669 6564 2073 696e   or modified sin
+00003880: 6365 2074 6865 200a 6c61 7374 2074 696d  ce the .last tim
+00003890: 6520 6064 6274 6020 7261 6e20 7468 6973  e `dbt` ran this
+000038a0: 206d 6f64 656c 2e0a 6060 6063 6f6d 6d61   model..```comma
+000038b0: 6e64 6c69 6e65 0a74 6f75 6368 206d 6f64  ndline.touch mod
+000038c0: 656c 732f 6163 746f 7273 5f69 6e73 6967  els/actors_insig
+000038d0: 6874 5f69 6e63 7265 6d65 6e74 616c 2e73  ht_incremental.s
+000038e0: 716c 0a60 6060 0a60 6060 0a7b 7b20 636f  ql.```.```.{{ co
+000038f0: 6e66 6967 286f 7264 6572 5f62 793d 2728  nfig(order_by='(
+00003900: 7570 6461 7465 645f 6174 2c20 6964 2c20  updated_at, id, 
+00003910: 6e61 6d65 2927 2c20 6d61 7465 7269 616c  name)', material
+00003920: 697a 6564 3d27 696e 6372 656d 656e 7461  ized='incrementa
+00003930: 6c27 2920 7d7d 0a0a 5345 4c45 4354 2069  l') }}..SELECT i
+00003940: 642c 0a20 2061 6e79 2861 6374 6f72 5f6e  d,.  any(actor_n
+00003950: 616d 6529 2061 7320 6e61 6d65 2c0a 2020  ame) as name,.  
+00003960: 756e 6971 4578 6163 7428 6d6f 7669 655f  uniqExact(movie_
+00003970: 6964 2920 2020 2061 7320 6e75 6d5f 6d6f  id)    as num_mo
+00003980: 7669 6573 2c0a 2020 6176 6728 7261 7469  vies,.  avg(rati
+00003990: 6e67 2920 2020 2020 2020 2020 2020 2020  ng)             
+000039a0: 2020 2061 7320 6176 675f 7261 7469 6e67     as avg_rating
+000039b0: 2c0a 2020 6d61 7828 6372 6561 7465 645f  ,.  max(created_
+000039c0: 6174 2920 6173 2075 7064 6174 6564 5f61  at) as updated_a
+000039d0: 740a 4652 4f4d 2028 0a20 2053 454c 4543  t.FROM (.  SELEC
+000039e0: 5420 6163 746f 7273 2e69 6420 6173 2069  T actors.id as i
+000039f0: 642c 0a20 2020 2020 2020 636f 6e63 6174  d,.       concat
+00003a00: 2861 6374 6f72 732e 6669 7273 745f 6e61  (actors.first_na
+00003a10: 6d65 2c20 2720 272c 2061 6374 6f72 732e  me, ' ', actors.
+00003a20: 6c61 7374 5f6e 616d 6529 2061 7320 6163  last_name) as ac
+00003a30: 746f 725f 6e61 6d65 2c0a 2020 2020 2020  tor_name,.      
+00003a40: 206d 6f76 6965 732e 6964 2061 7320 6d6f   movies.id as mo
+00003a50: 7669 655f 6964 2c0a 2020 2020 2020 206d  vie_id,.       m
+00003a60: 6f76 6965 732e 7261 7469 6e67 2061 7320  ovies.rating as 
+00003a70: 7261 7469 6e67 2c0a 2020 2020 2020 2063  rating,.       c
+00003a80: 7265 6174 6564 5f61 740a 2020 4652 4f4d  reated_at.  FROM
+00003a90: 2020 7b7b 2073 6f75 7263 6528 2769 6d64    {{ source('imd
+00003aa0: 6227 2c20 2761 6374 6f72 7327 2920 7d7d  b', 'actors') }}
+00003ab0: 0a20 2020 2020 2020 204a 4f49 4e20 7b7b  .        JOIN {{
+00003ac0: 2073 6f75 7263 6528 2769 6d64 6227 2c20   source('imdb', 
+00003ad0: 2772 6f6c 6573 2729 207d 7d20 4f4e 2072  'roles') }} ON r
+00003ae0: 6f6c 6573 2e61 6374 6f72 5f69 6420 3d20  oles.actor_id = 
+00003af0: 6163 746f 7273 2e69 640a 2020 2020 2020  actors.id.      
+00003b00: 2020 4c45 4654 204f 5554 4552 204a 4f49    LEFT OUTER JOI
+00003b10: 4e20 7b7b 2073 6f75 7263 6528 2769 6d64  N {{ source('imd
+00003b20: 6227 2c20 276d 6f76 6965 7327 2920 7d7d  b', 'movies') }}
+00003b30: 204f 4e20 6d6f 7669 6573 2e69 6420 3d20   ON movies.id = 
+00003b40: 726f 6c65 732e 6d6f 7669 655f 6964 0a29  roles.movie_id.)
+00003b50: 0a47 524f 5550 2042 5920 6964 0a0a 7b25  .GROUP BY id..{%
+00003b60: 2069 6620 6973 5f69 6e63 7265 6d65 6e74   if is_increment
+00003b70: 616c 2829 2025 7d0a 0a2d 2d20 7468 6973  al() %}..-- this
+00003b80: 2066 696c 7465 7220 7769 6c6c 206f 6e6c   filter will onl
+00003b90: 7920 6265 2061 7070 6c69 6564 206f 6e20  y be applied on 
+00003ba0: 616e 2069 6e63 7265 6d65 6e74 616c 2072  an incremental r
+00003bb0: 756e 0a77 6865 7265 2069 6420 3e20 2873  un.where id > (s
+00003bc0: 656c 6563 7420 6d61 7828 6964 2920 6672  elect max(id) fr
+00003bd0: 6f6d 207b 7b20 7468 6973 207d 7d29 206f  om {{ this }}) o
+00003be0: 7220 7570 6461 7465 645f 6174 203e 2028  r updated_at > (
+00003bf0: 7365 6c65 6374 206d 6178 2875 7064 6174  select max(updat
+00003c00: 6564 5f61 7429 2066 726f 6d20 7b7b 7468  ed_at) from {{th
+00003c10: 6973 7d7d 290a 0a7b 2520 656e 6469 6620  is}})..{% endif 
+00003c20: 257d 0a60 6060 0a57 6520 6361 6e20 7665  %}.```.We can ve
+00003c30: 7269 6679 2074 6861 7420 7669 6577 2c20  rify that view, 
+00003c40: 7461 626c 6520 2620 696e 6372 656d 656e  table & incremen
+00003c50: 7461 6c20 6d61 7465 7269 616c 697a 6174  tal materializat
+00003c60: 696f 6e73 2c20 616c 6c20 6765 6e65 7261  ions, all genera
+00003c70: 7465 2074 6865 2073 616d 6520 7265 7370  te the same resp
+00003c80: 6f6e 7365 2e20 0a60 6060 0a20 5345 4c45  onse. .```. SELE
+00003c90: 4354 202a 2046 524f 4d20 696d 6462 2e61  CT * FROM imdb.a
+00003ca0: 6374 6f72 735f 696e 7369 6768 745f 7461  ctors_insight_ta
+00003cb0: 626c 6520 4f52 4445 5220 4259 206e 756d  ble ORDER BY num
+00003cc0: 5f6d 6f76 6965 7320 4445 5343 3b0a 6060  _movies DESC;.``
+00003cd0: 600a 6060 6063 6f6d 6d61 6e64 6c69 6e65  `.```commandline
+00003ce0: 0a64 6274 2072 756e 202d 6d20 6d6f 6465  .dbt run -m mode
+00003cf0: 6c73 2f61 6374 6f72 735f 696e 7369 6768  ls/actors_insigh
+00003d00: 745f 696e 6372 656d 656e 7461 6c2e 7371  t_incremental.sq
+00003d10: 6c0a 6060 600a 4c65 7427 7320 696e 7365  l.```.Let's inse
+00003d20: 7274 2061 2066 6577 206d 6f72 6520 726f  rt a few more ro
+00003d30: 7773 2074 6f20 6465 6d6f 6e73 7472 6174  ws to demonstrat
+00003d40: 6520 7468 6520 706f 7765 7220 6f66 2069  e the power of i
+00003d50: 6e63 7265 6d65 6e74 616c 206d 6174 6572  ncremental mater
+00003d60: 6961 6c69 7a61 7469 6f6e 732e 204e 6f77  ializations. Now
+00003d70: 2074 6865 206d 6f73 7420 0a61 7070 6561   the most .appea
+00003d80: 7265 6420 6163 746f 7220 7368 6f75 6c64  red actor should
+00003d90: 2062 6520 2743 6872 6973 2050 7261 7474   be 'Chris Pratt
+00003da0: 272e 200a 6060 600a 494e 5345 5254 2049  '. .```.INSERT I
+00003db0: 4e54 4f20 696d 6462 2e6d 6f76 6965 7320  NTO imdb.movies 
+00003dc0: 5641 4c55 4553 2028 392c 2027 5061 7373  VALUES (9, 'Pass
+00003dd0: 656e 6765 7273 272c 2032 3031 362c 2037  engers', 2016, 7
+00003de0: 293b 0a49 4e53 4552 5420 494e 544f 2069  );.INSERT INTO i
+00003df0: 6d64 622e 6d6f 7669 6573 2056 414c 5545  mdb.movies VALUE
+00003e00: 5320 2831 302c 2027 5468 6520 546f 6d6f  S (10, 'The Tomo
+00003e10: 7272 6f77 2057 6172 272c 2032 3032 312c  rrow War', 2021,
+00003e20: 2036 2e35 293b 0a0a 494e 5345 5254 2049   6.5);..INSERT I
+00003e30: 4e54 4f20 696d 6462 2e72 6f6c 6573 2028  NTO imdb.roles (
+00003e40: 6163 746f 725f 6964 2c20 6d6f 7669 655f  actor_id, movie_
+00003e50: 6964 2c20 726f 6c65 5f6e 616d 6529 2056  id, role_name) V
+00003e60: 414c 5545 5328 342c 2039 2c20 274a 696d  ALUES(4, 9, 'Jim
+00003e70: 2050 7265 7374 6f6e 2729 3b0a 494e 5345   Preston');.INSE
+00003e80: 5254 2049 4e54 4f20 696d 6462 2e72 6f6c  RT INTO imdb.rol
+00003e90: 6573 2028 6163 746f 725f 6964 2c20 6d6f  es (actor_id, mo
+00003ea0: 7669 655f 6964 2c20 726f 6c65 5f6e 616d  vie_id, role_nam
+00003eb0: 6529 2056 414c 5545 5328 342c 2031 302c  e) VALUES(4, 10,
+00003ec0: 2027 4461 6e20 466f 7265 7374 6572 2729   'Dan Forester')
+00003ed0: 3b0a 6060 600a 6060 6063 6f6d 6d61 6e64  ;.```.```command
+00003ee0: 6c69 6e65 0a64 6274 2072 756e 202d 6d20  line.dbt run -m 
+00003ef0: 6d6f 6465 6c73 2f61 6374 6f72 735f 696e  models/actors_in
+00003f00: 7369 6768 745f 696e 6372 656d 656e 7461  sight_incrementa
+00003f10: 6c2e 7371 6c0a 6060 600a 6060 600a 5345  l.sql.```.```.SE
+00003f20: 4c45 4354 202a 2046 524f 4d20 696d 6462  LECT * FROM imdb
+00003f30: 2e61 6374 6f72 735f 696e 7369 6768 745f  .actors_insight_
+00003f40: 696e 6372 656d 656e 7461 6c20 4f52 4445  incremental ORDE
+00003f50: 5220 4259 206e 756d 5f6d 6f76 6965 7320  R BY num_movies 
+00003f60: 4445 5343 3b0a 6060 600a 215b 436f 6e66  DESC;.```.![Conf
+00003f70: 6972 6d33 5d28 2e2f 6578 616d 706c 6573  irm3](./examples
+00003f80: 2f39 5f69 6e63 7265 6d65 6e74 616c 5f63  /9_incremental_c
+00003f90: 6f6e 6669 726d 2e70 6e67 290a 2323 2320  onfirm.png).### 
+00003fa0: 486f 7720 6974 2077 6f72 6b73 0a31 2e20  How it works.1. 
+00003fb0: 6064 6274 6020 7769 6c6c 2066 6972 7374  `dbt` will first
+00003fc0: 2063 7265 6174 6520 6120 7465 6d70 6f72   create a tempor
+00003fd0: 6172 7920 7461 626c 6520 6e61 6d65 6420  ary table named 
+00003fe0: 6061 6374 6f72 735f 696e 7369 6768 745f  `actors_insight_
+00003ff0: 696e 6372 656d 656e 7461 6c5f 746d 7060  incremental_tmp`
+00004000: 2026 2069 6e73 6572 7420 616c 6c20 7468   & insert all th
+00004010: 6f73 6520 726f 7773 2077 6869 6368 200a  ose rows which .
+00004020: 7061 7373 206f 7572 2060 6973 5f69 6e63  pass our `is_inc
+00004030: 7265 6d65 6e74 616c 2829 6020 6669 6c74  remental()` filt
+00004040: 6572 2e0a 322e 2041 206e 6577 2074 6162  er..2. A new tab
+00004050: 6c65 2060 6163 746f 7273 5f69 6e73 6967  le `actors_insig
+00004060: 6874 5f69 6e63 7265 6d65 6e74 616c 5f6e  ht_incremental_n
+00004070: 6577 6020 7769 6c6c 2062 6520 6372 6561  ew` will be crea
+00004080: 7465 6420 2620 726f 7773 2066 726f 6d20  ted & rows from 
+00004090: 7468 6520 6f6c 6420 7461 626c 6520 6061  the old table `a
+000040a0: 6374 6f72 735f 696e 7369 6768 745f 696e  ctors_insight_in
+000040b0: 6372 656d 656e 7461 6c60 200a 7769 6c6c  cremental` .will
+000040c0: 2062 6520 696e 6765 7374 6564 2068 6572   be ingested her
+000040d0: 652e 2060 6462 7460 2077 696c 6c20 6d61  e. `dbt` will ma
+000040e0: 6b65 2073 7572 6520 7468 6174 2060 756e  ke sure that `un
+000040f0: 6971 7565 5f6b 6579 6020 2869 6620 616e  ique_key` (if an
+00004100: 7920 6465 636c 6172 6564 2069 6e20 636f  y declared in co
+00004110: 6e66 6967 2920 636f 6e73 7472 6169 6e74  nfig) constraint
+00004120: 2069 7320 6d61 696e 7461 696e 6564 2c20   is maintained, 
+00004130: 0a62 7920 6e6f 7420 616c 6c6f 7769 6e67  .by not allowing
+00004140: 2074 686f 7365 2072 6f77 7320 7768 6963   those rows whic
+00004150: 6820 6861 7665 2074 6865 2073 616d 6520  h have the same 
+00004160: 6075 6e69 7175 655f 6b65 7960 2061 7320  `unique_key` as 
+00004170: 7468 6520 7072 6576 696f 7573 2074 656d  the previous tem
+00004180: 706f 7261 7279 2074 6162 6c65 2e20 0a33  porary table. .3
+00004190: 2e20 5468 6520 726f 7773 2066 726f 6d20  . The rows from 
+000041a0: 7468 6520 7465 6d70 6f72 6172 7920 7461  the temporary ta
+000041b0: 626c 6520 776f 756c 6420 6265 2069 6e67  ble would be ing
+000041c0: 6573 7465 6420 696e 746f 2074 6865 206e  ested into the n
+000041d0: 6577 2074 6162 6c65 2e0a 342e 204f 7572  ew table..4. Our
+000041e0: 2070 7265 7669 6f75 7320 7461 626c 6520   previous table 
+000041f0: 2860 6163 746f 7273 5f69 6e73 6967 6874  (`actors_insight
+00004200: 5f69 6e63 7265 6d65 6e74 616c 6029 2026  _incremental`) &
+00004210: 206e 6577 2074 6162 6c65 2028 6061 6374   new table (`act
+00004220: 6f72 735f 696e 7369 6768 745f 6e65 7760  ors_insight_new`
+00004230: 2920 7769 6c6c 2062 6520 6578 6368 616e  ) will be exchan
+00004240: 6765 642e 200a 0a23 2044 6972 6563 7420  ged. ..# Direct 
+00004250: 5772 6974 6520 746f 2043 4e43 4820 556e  Write to CNCH Un
+00004260: 6971 7565 204b 6579 2054 6162 6c65 0a23  ique Key Table.#
+00004270: 2320 5265 7175 6972 656d 656e 740a 312e  # Requirement.1.
+00004280: 2060 6462 742d 6279 7465 686f 7573 6560   `dbt-bytehouse`
+00004290: 2063 6f6e 6e65 6374 6f72 2076 6572 7369   connector versi
+000042a0: 6f6e 2074 6f20 6265 2061 7420 6c65 6173  on to be at leas
+000042b0: 7420 6031 2e37 2e31 602e 200a 322e 204e  t `1.7.1`. .2. N
+000042c0: 6565 6473 2074 6f20 7365 7420 636f 6e66  eeds to set conf
+000042d0: 6967 206e 616d 6520 6063 6e63 685f 756e  ig name `cnch_un
+000042e0: 6971 7565 5f6b 6579 6020 696e 7374 6561  ique_key` instea
+000042f0: 6420 6f66 2060 756e 6971 7565 5f6b 6579  d of `unique_key
+00004300: 600a 332e 204e 6565 6473 2074 6f20 7365  `.3. Needs to se
+00004310: 7420 636f 6e66 6967 2060 696e 6372 656d  t config `increm
+00004320: 656e 7461 6c5f 7374 7261 7465 6779 6020  ental_strategy` 
+00004330: 6173 2060 6170 7065 6e64 600a 342e 2057  as `append`.4. W
+00004340: 7269 7465 2061 2053 514c 2065 7870 7265  rite a SQL expre
+00004350: 7373 696f 6e20 746f 2061 7070 656e 6420  ssion to append 
+00004360: 7468 6520 7669 7274 7561 6c20 7761 7265  the virtual ware
+00004370: 686f 7573 6520 6964 2061 7420 7468 6520  house id at the 
+00004380: 656e 6420 6f66 2044 4254 206d 6f64 656c  end of DBT model
+00004390: 2c20 6578 616d 706c 650a 6053 4554 5449  , example.`SETTI
+000043a0: 4e47 5320 7669 7274 7561 6c5f 7761 7265  NGS virtual_ware
+000043b0: 686f 7573 653d 2776 772d 6964 272c 2076  house='vw-id', v
+000043c0: 6972 7475 616c 5f77 6172 6568 6f75 7365  irtual_warehouse
+000043d0: 5f77 7269 7465 3d27 7677 2d69 6427 600a  _write='vw-id'`.
+000043e0: 2323 2045 7861 6d70 6c65 0a60 6060 0a7b  ## Example.```.{
+000043f0: 7b0a 2020 2020 636f 6e66 6967 280a 2020  {.    config(.  
+00004400: 2020 2020 2020 6d61 7465 7269 616c 697a        materializ
+00004410: 6564 3d27 696e 6372 656d 656e 7461 6c27  ed='incremental'
+00004420: 2c0a 2020 2020 2020 2020 636e 6368 5f75  ,.        cnch_u
+00004430: 6e69 7175 655f 6b65 793d 2769 6427 2c0a  nique_key='id',.
+00004440: 2020 2020 2020 2020 696e 6372 656d 656e          incremen
+00004450: 7461 6c5f 7374 7261 7465 6779 3d27 6170  tal_strategy='ap
+00004460: 7065 6e64 2720 2020 200a 2020 2020 290a  pend'    .    ).
+00004470: 7d7d 0a0a 5345 4c45 4354 0a20 2020 2069  }}..SELECT.    i
+00004480: 642c 0a20 2020 2074 7261 6e73 6163 7469  d,.    transacti
+00004490: 6f6e 5f64 6174 652c 0a20 2020 2075 7365  on_date,.    use
+000044a0: 725f 6964 2c0a 2020 2020 616d 6f75 6e74  r_id,.    amount
+000044b0: 2c0a 2020 2020 7374 6174 7573 0a46 524f  ,.    status.FRO
+000044c0: 4d20 0a20 2020 2064 6274 5f75 6e69 7175  M .    dbt_uniqu
+000044d0: 652e 7472 616e 7361 6374 696f 6e73 200a  e.transactions .
+000044e0: 0a7b 2520 6966 2069 735f 696e 6372 656d  .{% if is_increm
+000044f0: 656e 7461 6c28 2920 257d 0a0a 2020 5748  ental() %}..  WH
+00004500: 4552 4520 7472 616e 7361 6374 696f 6e5f  ERE transaction_
+00004510: 6461 7465 203e 3d20 2853 454c 4543 5420  date >= (SELECT 
+00004520: 6d61 7828 7472 616e 7361 6374 696f 6e5f  max(transaction_
+00004530: 6461 7465 2920 4652 4f4d 2064 6274 5f75  date) FROM dbt_u
+00004540: 6e69 7175 652e 7472 616e 7361 6374 696f  nique.transactio
+00004550: 6e73 290a 0a7b 2520 656e 6469 6620 257d  ns)..{% endif %}
+00004560: 0a0a 5345 5454 494e 4753 2076 6972 7475  ..SETTINGS virtu
+00004570: 616c 5f77 6172 6568 6f75 7365 3d27 7677  al_warehouse='vw
+00004580: 2d69 6427 2c20 7669 7274 7561 6c5f 7761  -id', virtual_wa
+00004590: 7265 686f 7573 655f 7772 6974 653d 2776  rehouse_write='v
+000045a0: 772d 6964 270a 6060 600a 2320 5072 6f6a  w-id'.```.# Proj
+000045b0: 6563 7420 446f 6375 6d65 6e74 6174 696f  ect Documentatio
+000045c0: 6e0a 6064 6274 6020 7072 6f76 6964 6573  n.`dbt` provides
+000045d0: 2061 2077 6179 2074 6f20 6765 6e65 7261   a way to genera
+000045e0: 7465 2064 6f63 756d 656e 7461 7469 6f6e  te documentation
+000045f0: 2066 6f72 2079 6f75 7220 6462 7420 7072   for your dbt pr
+00004600: 6f6a 6563 7420 616e 6420 7265 6e64 6572  oject and render
+00004610: 2069 7420 6173 2061 2077 6562 7369 7465   it as a website
+00004620: 2e20 0a43 7265 6174 6520 606d 6f64 656c  . .Create `model
+00004630: 732f 6163 746f 7273 5f69 6e73 6967 6874  s/actors_insight
+00004640: 5f69 6e63 7265 6d65 6e74 616c 2e79 6d6c  _incremental.yml
+00004650: 6020 746f 2067 656e 6572 6174 6520 646f  ` to generate do
+00004660: 6375 6d65 6e74 6174 696f 6e20 666f 7220  cumentation for 
+00004670: 6f75 7220 6d6f 6465 6c73 2e20 0a60 6060  our models. .```
+00004680: 7961 6d6c 0a76 6572 7369 6f6e 3a20 320a  yaml.version: 2.
+00004690: 0a6d 6f64 656c 733a 0a20 202d 206e 616d  .models:.  - nam
+000046a0: 653a 2061 6374 6f72 735f 696e 7369 6768  e: actors_insigh
+000046b0: 745f 696e 6372 656d 656e 7461 6c0a 2020  t_incremental.  
+000046c0: 2020 6465 7363 7269 7074 696f 6e3a 2041    description: A
+000046d0: 6374 6f72 2061 7070 6561 7261 6e63 6520  ctor appearance 
+000046e0: 7375 6d6d 6172 7920 6261 7365 6420 6f6e  summary based on
+000046f0: 2072 6f6c 6573 0a20 2020 2063 6f6c 756d   roles.    colum
+00004700: 6e73 3a20 0a20 2020 2020 202d 206e 616d  ns: .      - nam
+00004710: 653a 2069 640a 2020 2020 2020 2020 6465  e: id.        de
+00004720: 7363 7269 7074 696f 6e3a 2054 6865 2069  scription: The i
+00004730: 6420 6e75 6d62 6572 206f 6620 6163 746f  d number of acto
+00004740: 720a 2020 2020 2020 2d20 6e61 6d65 3a20  r.      - name: 
+00004750: 6e61 6d65 0a20 2020 2020 2020 2064 6573  name.        des
+00004760: 6372 6970 7469 6f6e 3a20 5468 6520 6e61  cription: The na
+00004770: 6d65 206f 6620 6163 746f 720a 2020 2020  me of actor.    
+00004780: 2020 2d20 6e61 6d65 3a20 6e75 6d5f 6d6f    - name: num_mo
+00004790: 7669 6573 0a20 2020 2020 2020 2064 6573  vies.        des
+000047a0: 6372 6970 7469 6f6e 3a20 5468 6520 6e75  cription: The nu
+000047b0: 6d62 6572 206f 6620 6d6f 7669 6573 2061  mber of movies a
+000047c0: 6374 6f72 2068 6173 2061 7070 6561 7265  ctor has appeare
+000047d0: 6420 0a20 2020 2020 202d 206e 616d 653a  d .      - name:
+000047e0: 2061 7667 5f72 6174 696e 670a 2020 2020   avg_rating.    
+000047f0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00004800: 2041 7665 7261 6765 2072 6174 696e 670a   Average rating.
+00004810: 2020 2020 2020 2d20 6e61 6d65 3a20 7570        - name: up
+00004820: 6461 7465 645f 6174 0a20 2020 2020 2020  dated_at.       
+00004830: 2064 6573 6372 6970 7469 6f6e 3a20 4c61   description: La
+00004840: 7465 7374 2075 7064 6174 6520 7469 6d65  test update time
+00004850: 0a60 6060 0a55 7365 2060 6462 7420 646f  .```.Use `dbt do
+00004860: 6373 2067 656e 6572 6174 6560 2074 6f20  cs generate` to 
+00004870: 6765 6e65 7261 7465 2074 6865 2064 6f63  generate the doc
+00004880: 756d 656e 7461 7469 6f6e 2066 6f72 2079  umentation for y
+00004890: 6f75 7220 6d6f 6465 6c73 2026 2060 6462  our models & `db
+000048a0: 7420 646f 6373 2073 6572 7665 6020 746f  t docs serve` to
+000048b0: 2073 6572 7665 2074 6865 2064 6f63 756d   serve the docum
+000048c0: 656e 7461 7469 6f6e 2069 6e20 0a79 6f75  entation in .you
+000048d0: 7220 6c6f 6361 6c20 6272 6f77 7365 7220  r local browser 
+000048e0: 6f6e 2070 6f72 7420 3830 3030 2e0a 215b  on port 8000..![
+000048f0: 446f 635d 282e 2f65 7861 6d70 6c65 732f  Doc](./examples/
+00004900: 3130 5f64 6f63 732e 706e 6729 0a23 204c  10_docs.png).# L
+00004910: 6f63 616c 2044 6576 656c 6f70 6d65 6e74  ocal Development
+00004920: 0a55 7064 6174 6520 6074 6573 7473 2f69  .Update `tests/i
+00004930: 6e74 6567 7261 7469 6f6e 2f63 6f6e 6665  ntegration/confe
+00004940: 7374 2e70 7960 2066 696c 6520 746f 2069  st.py` file to i
+00004950: 6e63 6c75 6465 2079 6f75 7220 636f 6e6e  nclude your conn
+00004960: 6563 7469 6f6e 2063 7265 6465 6e74 6961  ection credentia
+00004970: 6c73 2e20 466f 7220 7275 6e6e 696e 6720  ls. For running 
+00004980: 7465 7374 7320 6c6f 6361 6c6c 792c 2066  tests locally, f
+00004990: 6f6c 6c6f 7720 0a74 6865 7365 2073 7465  ollow .these ste
+000049a0: 7073 3a0a 6060 6063 6f6d 6d61 6e64 6c69  ps:.```commandli
+000049b0: 6e65 0a70 6970 2069 6e73 7461 6c6c 202d  ne.pip install -
+000049c0: 7220 6465 765f 7265 7175 6972 656d 656e  r dev_requiremen
+000049d0: 7473 2e74 7874 0a70 7974 686f 6e20 2d6d  ts.txt.python -m
+000049e0: 2070 7974 6573 740a 6060 600a 2320 4f72   pytest.```.# Or
+000049f0: 6967 696e 616c 2041 7574 686f 720a 4279  iginal Author.By
+00004a00: 7465 486f 7573 6520 7761 6e74 7320 746f  teHouse wants to
+00004a10: 2074 6861 6e6b 2043 6c69 636b 486f 7573   thank ClickHous
+00004a20: 6520 666f 7220 6f72 6967 696e 616c 2063  e for original c
+00004a30: 6f6e 7472 6962 7574 696f 6e20 746f 2074  ontribution to t
+00004a40: 6869 7320 636f 6e6e 6563 746f 722e 0a0a  his connector...
+00004a50: 2320 4c69 6365 6e73 650a 5468 6973 2070  # License.This p
+00004a60: 726f 6a65 6374 2069 7320 6469 7374 7269  roject is distri
+00004a70: 6275 7465 6420 756e 6465 7220 7468 6520  buted under the 
+00004a80: 7465 726d 7320 6f66 2074 6865 2041 7061  terms of the Apa
+00004a90: 6368 6520 4c69 6365 6e73 6520 2856 6572  che License (Ver
+00004aa0: 7369 6f6e 2032 2e30 292e 0a              sion 2.0)..
```

### Comparing `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/__init__.py` & `dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/__version__.py` & `dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 
-version = '1.7.1'
+version = '1.7.2'
```

### Comparing `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/column.py` & `dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/column.py`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/connections.py` & `dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/credentials.py` & `dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/dbclient.py` & `dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/dbclient.py`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/impl.py` & `dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/impl.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,14 @@
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 
-import csv
-import io
 from concurrent.futures import Future
 from dataclasses import dataclass
 from typing import Callable, Dict, List, Optional, Set, Union
 
 import agate
 import dbt.exceptions
 from dbt.adapters.base import AdapterConfig, available
@@ -40,15 +38,15 @@
 
 GET_CATALOG_MACRO_NAME = 'get_catalog'
 LIST_SCHEMAS_MACRO_NAME = 'list_schemas'
 
 
 @dataclass
 class ByteHouseConfig(AdapterConfig):
-    engine: str = 'MergeTree()'
+    engine: str = 'CnchMergeTree()'
     order_by: Optional[Union[List[str], str]] = 'tuple()'
     partition_by: Optional[Union[List[str], str]] = None
 
 
 class ByteHouseAdapter(SQLAdapter):
     Relation = ByteHouseRelation
     Column = ByteHouseColumn
@@ -175,30 +173,18 @@
             results = self.execute_macro('bytehouse__get_database', kwargs={'database': schema})
             if len(results.rows):
                 return ByteHouseDatabase(**results.rows[0])
             return None
         except dbt.exceptions.DbtRuntimeError:
             return None
 
-    def parse_bytehouse_columns(
-        self, relation: ByteHouseRelation, raw_rows: List[agate.Row]
-    ) -> List[ByteHouseColumn]:
-        rows = [dict(zip(row._keys, row._values)) for row in raw_rows]
-
-        return [
-            ByteHouseColumn(
-                column=column['name'],
-                dtype=column['type'],
-            )
-            for column in rows
-        ]
-
-    def get_columns_in_relation(self, relation: ByteHouseRelation) -> List[ByteHouseColumn]:
-        rows: List[agate.Row] = super().get_columns_in_relation(relation)
-        return self.parse_bytehouse_columns(relation, rows)
+    @available
+    def create_agate_table(self, data, column_names) -> agate.Table:
+        agate_table = dbt.clients.agate_helper.table_from_data_flat(data, column_names)
+        return agate_table
 
     def get_catalog(self, manifest):
         schema_map = self._get_catalog_schemas(manifest)
 
         with executor(self.config) as tpe:
             futures: List[Future[agate.Table]] = []
             for info, schemas in schema_map.items():
@@ -282,48 +268,26 @@
     ) -> str:
         clause = f'alter table {dst_name} update {dst_column} = {clause}'
         if where_clause is not None:
             clause += f' where {where_clause}'
         return clause
 
     @available
-    def get_csv_data(self, table):
-        # TODO: Consider passing table to macro
-        row_count = len(table.rows)
-        column_count = 0
-        if row_count > 0:
-            column_count = len(table.rows[0])
-
-        # TODO: Use hashmap for conversion
-        # TODO: Implement all datatypes
-        datatypes = []
-        for c in table._column_types:
-            if isinstance(c, dbt.clients.agate_helper.Number):
-                datatypes.append("Int")
-            elif isinstance(c, dbt.clients.agate_helper.ISODateTime):
-                datatypes.append("Datetime")
-            elif isinstance(c, agate.data_types.boolean.Boolean):
-                datatypes.append("BooleanInt")
-            elif isinstance(c, agate.data_types.date_time.DateTime):
-                datatypes.append("Datetime")
-            elif isinstance(c, agate.data_types.number.Number):
-                datatypes.append("Int")
-            elif isinstance(c, agate.data_types.text.Text):
-                datatypes.append("String")
-            else:
-                datatypes.append("NotImplemented")
+    def get_sql_select_query_data(self, table):
+        sql_queries = []
 
-        data = "|" + str(row_count)
-        data += "|" + str(column_count)
-        for datatype in datatypes:
-            data += "|" + datatype
         for row in table.rows:
-            for datatype, val in enumerate(row):
-                data += "|" + str(val)
-        return data
+            # Prepare the SQL SELECT statement for each row
+            select_query = "SELECT " + ', '.join(f"'{c.csvify(d)}'" for c, d in zip(table._column_types, row))
+            sql_queries.append(select_query)
+
+        # Combine all SELECT statements with UNION ALL
+        combined_sql = " UNION ALL ".join(sql_queries) + ";"
+
+        return combined_sql
 
     def run_sql_for_tests(self, sql, fetch, conn):
         client = conn.handle
         try:
             if fetch:
                 result = client.query(sql).result_set
             else:
```

### Comparing `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/relation.py` & `dbt-bytehouse-1.7.2/dbt/adapters/bytehouse/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/__init__.py` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters/apply_grants.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters/relation.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/adapters/relation.sql`

 * *Files 19% similar despite different names*

```diff
@@ -30,14 +30,27 @@
       type=type,
       can_exchange=can_exchange
   ) -%}
   {% do return([false, new_relation]) %}
 {% endmacro %}
 
 {% macro bytehouse__get_database(database) %}
-    {% call statement('get_database', fetch_result=True) %}
-        select name, engine, comment
-        from system_meta.databases
-        where name = '{{ database }}'
-   {% endcall %}
-   {% do return(load_result('get_database').table) %}
+  {%- set sql -%}
+    show databases
+  {%- endset -%}
+  {%- set result = run_query(sql) -%}
+
+  {% set data = [] %}
+  {% for row in result %}
+    {% set database_metadata = {
+          'name': row[0],
+          'engine': row[8],
+          'comment': row[7]
+        }
+    %}
+    {% do data.append(database_metadata) %}
+  {% endfor %}
+
+  {% set column_names = ['name', 'engine', 'comment'] %}
+  {% set agate_table = adapter.create_agate_table(data, column_names) %}
+  {% do return(agate_table) %}
 {% endmacro %}
```

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/catalog.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/catalog.sql`

 * *Files 24% similar despite different names*

```diff
@@ -13,32 +13,40 @@
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 */
 
 {% macro bytehouse__get_catalog(information_schema, schemas) -%}
-  {%- call statement('catalog', fetch_result=True) -%}
-    select
-      null as table_database,
-      columns.database as table_schema,
-      columns.table as table_name,
-      if(tables.engine not in ('MaterializedView', 'View'), 'table', 'view') as table_type,
-      tables.comment as table_comment,
-      columns.name as column_name,
-      columns.position as column_index,
-      columns.type as column_type,
-      columns.comment as column_comment,
-      null as table_owner
-    from system_meta.columns as columns
-    join system_meta.tables as tables on tables.database = columns.database and tables.name = columns.table
-    where database != 'system_meta' and
-    (
-    {%- for schema in schemas -%}
-      columns.database = '{{ schema }}'
-      {%- if not loop.last %} or {% endif -%}
-    {%- endfor -%}
-    )
-    order by columns.database, columns.table, columns.position
-  {%- endcall -%}
-  {{ return(load_result('catalog').table) }}
+  {% set data = [] %}
+  {%- for schema in schemas -%}
+    {%- set sql -%}
+      show tables from {{ schema }}
+    {%- endset -%}
+    {%- set tables = run_query(sql) -%}
+    {%- for table in tables -%}
+      {%- set describe_sql -%}
+        describe table {{ schema }}.{{ table[0] }}
+      {%- endset -%}
+      {%- set result = run_query(describe_sql) -%}
+      {% for row in result %}
+        {% set table_type = 'view' if table[8] == 'VIEW' else 'table' %}
+        {% set metadata = {
+          'table_database': null,
+          'table_schema': schema,
+          'table_name': table[0],
+          'table_type': table_type,
+          'table_comment': table[7],
+          'column_name': row[0],
+          'column_index': loop.index,
+          'column_type': row[1],
+          'column_comment': row[4],
+          'table_owner': null
+        } %}
+        {% do data.append(metadata) %}
+      {% endfor %}
+    {%- endfor %}
+  {%- endfor %}
+  {% set column_names = ['table_database', 'table_schema', 'table_name', 'table_type', 'table_comment', 'column_name', 'column_index', 'column_type', 'column_comment', 'table_owner'] %}
+  {% set agate_table = adapter.create_agate_table(data, column_names) %}
+  {% do return(agate_table) %}
 {%- endmacro %}
```

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/incremental.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/incremental.sql`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,14 @@
       {% set fail_msg %}
           The source and target schemas on this incremental model are out of sync!
           They can be reconciled in several ways:
             - set the `on_schema_change` config to either append_new_columns or sync_all_columns, depending on your situation.
             - Re-run the incremental model with `full_refresh: True` to update the target schema.
             - update the schema manually and re-run the process.
       {% endset %}
-      {% do exceptions.CompilationError(fail_msg) %}
+      {% do exceptions.raise_compiler_error(fail_msg) %}
       {{ return }}
     {% endif %}
 
     {% do sync_column_schemas(on_schema_change, target_relation, schema_changes_dict) %}
 
 {% endmacro %}
```

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/seed.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/seed.sql`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,20 @@
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 */
 
 {% macro bytehouse__load_csv_rows(model, agate_table) %}
   {% set cols_sql = get_seed_column_quoted_csv(model, agate_table.column_names) %}
-  {% set data_sql = adapter.get_csv_data(agate_table) %}
+  {% set data_sql = adapter.get_sql_select_query_data(agate_table) %}
 
   {% set sql -%}
-    ByteHouseCustomCSV|insert into {{ this.render() }} ({{ cols_sql }}){{ adapter.get_model_settings(model) }} VALUES{{ data_sql }}
+    insert into {{ this.render() }} ({{ cols_sql }})
+    {{ adapter.get_model_settings(model) }}
+    {{ data_sql }}
   {%- endset %}
 
   {% do adapter.add_query(sql, bindings=agate_table, abridge_sql_log=True) %}
 {% endmacro %}
 
 {% macro bytehouse__create_csv_table(model, agate_table) %}
   {%- set column_override = model['config'].get('column_types', {}) -%}
```

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/snapshot.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/table.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/table.sql`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 {% endmaterialization %}
 
 {% macro engine_clause(label) %}
   {%- set engine = config.get('engine', validator=validation.any[basestring]) -%}
   {%- if engine is not none %}
     {{ label }} = {{ engine }}
   {%- else %}
-    {{ label }} = MergeTree()
+    {{ label }} = CnchMergeTree()
   {%- endif %}
 {%- endmacro -%}
 
 {% macro partition_cols(label) %}
   {%- set cols = config.get('partition_by', validator=validation.any[list, basestring]) -%}
   {%- if cols is not none %}
     {%- if cols is string -%}
@@ -123,15 +123,15 @@
     'HDFS',
     'MaterializedPostgreSQL',
     'S3',
     'EmbeddedRocksDB',
     'Hive'
   ] -%}
 
-  {%- if engine is none or 'MergeTree' in engine or engine in supported %}
+  {%- if engine is none or 'CnchMergeTree' in engine or engine in supported %}
     {%- if cols is not none %}
       {%- if cols is string -%}
         {%- set cols = [cols] -%}
       {%- endif -%}
       {{ label }} (
       {%- for item in cols -%}
         {{ item }}
```

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/test.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/view.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/persist_docs.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/schema_tests/relationships.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/schema_tests/relationships.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/utils/datatypes.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/utils/datatypes.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/utils/utils.sql` & `dbt-bytehouse-1.7.2/dbt/include/bytehouse/macros/utils/utils.sql`

 * *Files 15% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 {% macro bytehouse__replace(field, old_chars, new_chars) %}
    replaceAll({{ field }},'{{ old_chars }}','{{ new_chars }}')
 {% endmacro %}
 
 
 {% macro bytehouse__listagg(measure, delimiter_text, order_by_clause, limit_num) %}
-  {{ exceptions.CompilationError(
+  {{ exceptions.raise_compiler_error(
     'bytehouse does not support the listagg function.  See the groupArray function instead')
     }}
 {% endmacro %}
 
 
 {% macro bytehouse__array_construct(inputs, data_type) -%}
     {% if inputs|length > 0 %}
```

### Comparing `dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/PKG-INFO` & `dbt-bytehouse-1.7.2/dbt_bytehouse.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bytehouse
-Version: 1.7.1
+Version: 1.7.2
 Summary: The ByteHouse plugin for dbt (data build tool)
 Home-page: https://github.com/bytehouse-cloud/bytehouse-dbt
 Author: Rafsan Mazumder
 Author-email: rafsan.mazumder@bytedance.com
 License: MIT
 Project-URL: Documentation, https://github.com/bytehouse-cloud/bytehouse-dbt
 Project-URL: Changes, https://github.com/bytehouse-cloud/bytehouse-dbt/blob/main/CHANGELOG.md
@@ -18,17 +18,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.7.0
-Requires-Dist: bytehouse-driver
-Requires-Dist: python-dateutil
 
 # Introduction
 `dbt` (Data Building Tool) is an open source tool that enables data analysts and engineers to transform
 data in their warehouses simply by writing select statements. `dbt` performs the T (Transform) of ETL and
 allows companies to write transformations as queries and orchestrate them in a more efficient way. 
 ByteHouse dbt connector is a plugin enabling users to build their data warehouse ecosystem with dbt 
 and ByteHouse. 
@@ -144,22 +141,21 @@
 ```yaml
 <profile-name>:
   target: <target-name>
   outputs:
     <target-name>:
       type: bytehouse
       schema: <database-name>
-      user: <username>
-      password: <password>
+      user: bytehouse
+      password: <bytehouse-api-key>
       driver: native
       #optional fields
       host: <hostname>
       port: <port>
       region: <region-name>
-      account: <account-name>
       warehouse: <warehouse-name>
       retries: 1
       secure: True
       connect_timeout: 10
       send_receive_timeout: 300
       custom_settings: <empty>
 ```
@@ -182,41 +178,33 @@
     </tr>
     <tr>
         <td>schema</td>
         <td>Database name</td>
     </tr>
     <tr>
         <td>user</td>
-        <td>Username with adequate permissions to access the specified schema. For API Key authentication, user must be set to bytehouse</td>
+        <td>Must be set to bytehouse</td>
     </tr>
     <tr>
         <td>password</td>
-        <td>The password associated with the specified user</td>
+        <td>ByteHouse API Token</td>
     </tr>
     <tr>
         <td>driver</td>
         <td>Must be set to native</td>
     </tr>
     <tr>
         <td>host</td>
         <td>[Optional] The host name of the connection</td>
     </tr>
     <tr>
         <td>port </td>
         <td>[Optional] The port number of the host server</td>
     </tr>
     <tr>
-        <td>region</td>
-        <td>[Optional] Alias for host &amp; port </td>
-    </tr>
-    <tr>
-        <td>account</td>
-        <td>[Optional] ByteHouse account number</td>
-    </tr>
-    <tr>
         <td>warehouse</td>
         <td>[Optional] The name of the virtual warehouse that you want to use for this session</td>
     </tr>
     <tr>
         <td>retries</td>
         <td>[Optional] Number of times to retry the initial connection attempt if the error appears to be recoverable</td>
     </tr>
@@ -235,104 +223,14 @@
     <tr>
         <td>custom_settings</td>
         <td>[Optional] A mapping of ByteHouse specific user settings to use with the connection</td>
     </tr>
 </table>
 
 ## Connection & Authentication Configurations
-### ByteHouse Regions
-Currently, the driver supports the following region names across different cloud providers. Alternatively, if you know
-the host address of ByteHouse server, you can directly use host address & omit region name.
-<table>
-    <tr>
-        <td>Region Name</td>
-        <td>Target Server</td>
-    </tr>
-    <tr>
-        <td>AP-SOUTHEAST-1</td>
-        <td>gateway.aws-ap-southeast-1.bytehouse.cloud:19000</td>
-    </tr>
-    <tr>
-        <td>VOLCANO-CN-NORTH-1</td>
-        <td>bytehouse-cn-beijing.volces.com:19000</td>
-    </tr>
-</table>
-
-### Region & Password Configuration
-Required parameters: `account` `user` `password` `region`
-```yaml
-bytehouse_profile:
-  target: dev
-  outputs:
-    dev:
-      type: bytehouse
-      driver: native
-
-      # database
-      schema: $DATABASE_NAME
-
-      # target server address
-      region: $REGION_NAME
-
-      # account credentials
-      account: $ACCOUNT_NAME
-      user: $USER_NAME
-      password: $PASSWORD
-
-      # additional settings
-      secure: True
-```
-### Region & API Key Configuration
-Required parameters: `region` `user` `password`
-```yaml
-bytehouse_profile:
-  target: dev
-  outputs:
-    dev:
-      type: bytehouse
-      driver: native
-
-      # database
-      schema: $DATABASE_NAME
-
-      # target server address
-      region: $REGION_NAME
-
-      # account credentials
-      user: bytehouse
-      password: $API_KEY
-
-      # additional settings
-      secure: True
-```
-### Host Address & Password Configuration
-Required parameters: `host` `port` `account` `user` `password`
-```yaml
-bytehouse_profile:
-  target: dev
-  outputs:
-    dev:
-      type: bytehouse
-      driver: native
-
-      # database
-      schema: $DATABASE_NAME
-
-      # target server address
-      host: $HOST_ADDRESS  
-      port: $PORT_NUMBER
-
-      # account credentials
-      account: $ACCOUNT_NAME
-      user: $USER_NAME
-      password: $PASSWORD
-
-      # additional settings
-      secure: True
-```
 ### Host Address & API Key Configuration
 Required parameters: `host` `port` `user` `password`
 ```yaml
 bytehouse_profile:
   target: dev
   outputs:
     dev:
@@ -548,14 +446,49 @@
 1. `dbt` will first create a temporary table named `actors_insight_incremental_tmp` & insert all those rows which 
 pass our `is_incremental()` filter.
 2. A new table `actors_insight_incremental_new` will be created & rows from the old table `actors_insight_incremental` 
 will be ingested here. `dbt` will make sure that `unique_key` (if any declared in config) constraint is maintained, 
 by not allowing those rows which have the same `unique_key` as the previous temporary table. 
 3. The rows from the temporary table would be ingested into the new table.
 4. Our previous table (`actors_insight_incremental`) & new table (`actors_insight_new`) will be exchanged. 
+
+# Direct Write to CNCH Unique Key Table
+## Requirement
+1. `dbt-bytehouse` connector version to be at least `1.7.1`. 
+2. Needs to set config name `cnch_unique_key` instead of `unique_key`
+3. Needs to set config `incremental_strategy` as `append`
+4. Write a SQL expression to append the virtual warehouse id at the end of DBT model, example
+`SETTINGS virtual_warehouse='vw-id', virtual_warehouse_write='vw-id'`
+## Example
+```
+{{
+    config(
+        materialized='incremental',
+        cnch_unique_key='id',
+        incremental_strategy='append'    
+    )
+}}
+
+SELECT
+    id,
+    transaction_date,
+    user_id,
+    amount,
+    status
+FROM 
+    dbt_unique.transactions 
+
+{% if is_incremental() %}
+
+  WHERE transaction_date >= (SELECT max(transaction_date) FROM dbt_unique.transactions)
+
+{% endif %}
+
+SETTINGS virtual_warehouse='vw-id', virtual_warehouse_write='vw-id'
+```
 # Project Documentation
 `dbt` provides a way to generate documentation for your dbt project and render it as a website. 
 Create `models/actors_insight_incremental.yml` to generate documentation for our models. 
 ```yaml
 version: 2
 
 models:
```

### Comparing `dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/SOURCES.txt` & `dbt-bytehouse-1.7.2/dbt_bytehouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.7.1/setup.py` & `dbt-bytehouse-1.7.2/setup.py`

 * *Files identical despite different names*

