# Comparing `tmp/lukasdata-1.2.1.tar.gz` & `tmp/lukasdata-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.2.1.tar", last modified: Thu Apr 25 13:10:45 2024, max compression
+gzip compressed data, was "lukasdata-1.2.2.tar", last modified: Thu Apr 25 13:17:00 2024, max compression
```

## Comparing `lukasdata-1.2.1.tar` & `lukasdata-1.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 13:10:45.139777 lukasdata-1.2.1/
--rw-rw-rw-   0        0        0      128 2024-04-25 13:10:45.136780 lukasdata-1.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 13:10:45.095804 lukasdata-1.2.1/lukasdata/
--rw-rw-rw-   0        0        0        0 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/__init__.py
--rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/change_directory.py
--rw-rw-rw-   0        0        0      198 2024-04-23 22:24:46.000000 lukasdata-1.2.1/lukasdata/concat_dfs.py
--rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/count_nans.py
--rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/create_mask.py
--rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/del_jpg.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/determine_file_type.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/dict_to_json.py
--rw-rw-rw-   0        0        0      380 2024-04-25 13:07:11.000000 lukasdata-1.2.1/lukasdata/get_list_intersection.py
--rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/get_number_columns.py
--rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/json_to_dict.py
--rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/list_to_string.py
--rw-rw-rw-   0        0        0     1182 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/plot_metric_history.py
--rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.2.1/lukasdata/string_to_text.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:10:45.134779 lukasdata-1.2.1/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      128 2024-04-25 13:10:44.000000 lukasdata-1.2.1/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2024-04-25 13:10:44.000000 lukasdata-1.2.1/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 13:10:44.000000 lukasdata-1.2.1/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-25 13:10:44.000000 lukasdata-1.2.1/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-25 13:10:44.000000 lukasdata-1.2.1/lukasdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 13:10:45.139777 lukasdata-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-04-25 13:08:59.000000 lukasdata-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:17:00.374429 lukasdata-1.2.2/
+-rw-rw-rw-   0        0        0      128 2024-04-25 13:17:00.372431 lukasdata-1.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 13:17:00.353442 lukasdata-1.2.2/lukasdata/
+-rw-rw-rw-   0        0        0        0 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/change_directory.py
+-rw-rw-rw-   0        0        0      198 2024-04-23 22:24:46.000000 lukasdata-1.2.2/lukasdata/concat_dfs.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/count_nans.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/create_mask.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/dict_to_json.py
+-rw-rw-rw-   0        0        0      380 2024-04-25 13:07:11.000000 lukasdata-1.2.2/lukasdata/get_list_intersection.py
+-rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/get_number_columns.py
+-rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/json_to_dict.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/list_to_string.py
+-rw-rw-rw-   0        0        0     1182 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/plot_metric_history.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.2.2/lukasdata/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:17:00.370433 lukasdata-1.2.2/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-04-25 13:17:00.000000 lukasdata-1.2.2/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2024-04-25 13:17:00.000000 lukasdata-1.2.2/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 13:17:00.000000 lukasdata-1.2.2/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-25 13:17:00.000000 lukasdata-1.2.2/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 13:17:00.000000 lukasdata-1.2.2/lukasdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 13:17:00.375430 lukasdata-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      192 2024-04-25 13:16:28.000000 lukasdata-1.2.2/setup.py
```

### Comparing `lukasdata-1.2.1/lukasdata/change_directory.py` & `lukasdata-1.2.2/lukasdata/change_directory.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.2.1/lukasdata/plot_metric_history.py` & `lukasdata-1.2.2/lukasdata/plot_metric_history.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.2.1/lukasdata.egg-info/SOURCES.txt` & `lukasdata-1.2.2/lukasdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

