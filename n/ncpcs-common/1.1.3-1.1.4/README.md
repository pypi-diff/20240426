# Comparing `tmp/ncpcs_common-1.1.3.tar.gz` & `tmp/ncpcs_common-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ncpcs_common-1.1.3.tar", last modified: Sun Apr  7 01:50:47 2024, max compression
+gzip compressed data, was "dist/ncpcs_common-1.1.4.tar", last modified: Fri Apr 26 03:10:06 2024, max compression
```

## Comparing `ncpcs_common-1.1.3.tar` & `ncpcs_common-1.1.4.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:50:47.029232 ncpcs_common-1.1.3/
--rw-r--r--   0 chen       (501) staff       (20)      137 2024-04-07 01:50:47.028724 ncpcs_common-1.1.3/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-01 03:19:06.000000 ncpcs_common-1.1.3/README.md
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:50:46.983473 ncpcs_common-1.1.3/common/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.3/common/__init__.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:50:46.984943 ncpcs_common-1.1.3/common/constants/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.3/common/constants/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      296 2024-03-11 01:42:08.000000 ncpcs_common-1.1.3/common/constants/database_config.py
--rw-r--r--   0 chen       (501) staff       (20)    76288 2024-04-07 01:50:32.000000 ncpcs_common-1.1.3/common/constants/level_dict.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:50:46.985689 ncpcs_common-1.1.3/common/entity/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.3/common/entity/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      742 2024-03-14 03:04:23.000000 ncpcs_common-1.1.3/common/entity/relation_key.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:50:46.988048 ncpcs_common-1.1.3/common/service/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.3/common/service/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     1433 2024-02-22 00:30:19.000000 ncpcs_common-1.1.3/common/service/iccc3.py
--rw-r--r--   0 chen       (501) staff       (20)     3502 2024-03-14 03:08:51.000000 ncpcs_common-1.1.3/common/service/medical_text.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:50:47.004520 ncpcs_common-1.1.3/common/tests/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.3/common/tests/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     1621 2024-03-13 00:54:29.000000 ncpcs_common-1.1.3/common/tests/test_date_util.py
--rw-r--r--   0 chen       (501) staff       (20)      493 2024-03-11 01:56:01.000000 ncpcs_common-1.1.3/common/tests/test_encrypt_util.py
--rw-r--r--   0 chen       (501) staff       (20)      990 2024-02-22 00:30:19.000000 ncpcs_common-1.1.3/common/tests/test_iccc3.py
--rw-r--r--   0 chen       (501) staff       (20)      259 2024-03-08 06:32:33.000000 ncpcs_common-1.1.3/common/tests/test_id_card_util.py
--rw-r--r--   0 chen       (501) staff       (20)      238 2024-02-22 00:30:19.000000 ncpcs_common-1.1.3/common/tests/test_list_util.py
--rw-r--r--   0 chen       (501) staff       (20)     1776 2024-03-14 03:09:57.000000 ncpcs_common-1.1.3/common/tests/test_medical_text.py
--rw-r--r--   0 chen       (501) staff       (20)      196 2024-03-08 06:32:33.000000 ncpcs_common-1.1.3/common/tests/test_phone_util.py
--rw-r--r--   0 chen       (501) staff       (20)      248 2024-03-14 03:02:47.000000 ncpcs_common-1.1.3/common/tests/test_relation_key.py
--rw-r--r--   0 chen       (501) staff       (20)     2705 2024-03-27 06:49:32.000000 ncpcs_common-1.1.3/common/tests/test_sql_util.py
--rw-r--r--   0 chen       (501) staff       (20)     4194 2024-03-14 08:10:50.000000 ncpcs_common-1.1.3/common/tests/test_string_util.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:50:47.024401 ncpcs_common-1.1.3/common/util/
--rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.3/common/util/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      316 2024-03-08 07:12:56.000000 ncpcs_common-1.1.3/common/util/csv_util.py
--rw-r--r--   0 chen       (501) staff       (20)     2200 2024-03-11 01:54:24.000000 ncpcs_common-1.1.3/common/util/database_connection_util.py
--rw-r--r--   0 chen       (501) staff       (20)     9442 2024-03-25 08:45:23.000000 ncpcs_common-1.1.3/common/util/date_util.py
--rw-r--r--   0 chen       (501) staff       (20)     1133 2024-03-11 01:01:54.000000 ncpcs_common-1.1.3/common/util/encrypt_util.py
--rw-r--r--   0 chen       (501) staff       (20)      185 2024-03-07 08:57:18.000000 ncpcs_common-1.1.3/common/util/excel_util.py
--rw-r--r--   0 chen       (501) staff       (20)     3829 2024-03-08 06:13:07.000000 ncpcs_common-1.1.3/common/util/id_card_util.py
--rw-r--r--   0 chen       (501) staff       (20)      889 2024-03-20 01:13:40.000000 ncpcs_common-1.1.3/common/util/linux_util.py
--rw-r--r--   0 chen       (501) staff       (20)      131 2024-02-01 05:44:53.000000 ncpcs_common-1.1.3/common/util/list_util.py
--rw-r--r--   0 chen       (501) staff       (20)      238 2024-03-08 06:33:15.000000 ncpcs_common-1.1.3/common/util/phone_util.py
--rw-r--r--   0 chen       (501) staff       (20)     7451 2024-03-27 00:35:28.000000 ncpcs_common-1.1.3/common/util/sql_util.py
--rw-r--r--   0 chen       (501) staff       (20)     3279 2024-03-26 05:24:15.000000 ncpcs_common-1.1.3/common/util/string_util.py
--rw-r--r--   0 chen       (501) staff       (20)      497 2024-02-02 06:22:13.000000 ncpcs_common-1.1.3/common/util/timer_util.py
--rw-r--r--   0 chen       (501) staff       (20)     1315 2024-03-08 06:08:27.000000 ncpcs_common-1.1.3/common/util/zip_util.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-07 01:50:47.027656 ncpcs_common-1.1.3/ncpcs_common.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      137 2024-04-07 01:50:46.000000 ncpcs_common-1.1.3/ncpcs_common.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)     1168 2024-04-07 01:50:46.000000 ncpcs_common-1.1.3/ncpcs_common.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2024-04-07 01:50:46.000000 ncpcs_common-1.1.3/ncpcs_common.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       51 2024-04-07 01:50:46.000000 ncpcs_common-1.1.3/ncpcs_common.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)        7 2024-04-07 01:50:46.000000 ncpcs_common-1.1.3/ncpcs_common.egg-info/top_level.txt
--rw-r--r--   0 chen       (501) staff       (20)       38 2024-04-07 01:50:47.029412 ncpcs_common-1.1.3/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      263 2024-04-07 01:50:32.000000 ncpcs_common-1.1.3/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-26 03:10:06.180822 ncpcs_common-1.1.4/
+-rw-r--r--   0 chen       (501) staff       (20)      137 2024-04-26 03:10:06.179968 ncpcs_common-1.1.4/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-01 03:19:06.000000 ncpcs_common-1.1.4/README.md
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-26 03:10:06.142866 ncpcs_common-1.1.4/common/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.4/common/__init__.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-26 03:10:06.144925 ncpcs_common-1.1.4/common/constants/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.4/common/constants/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      296 2024-03-11 01:42:08.000000 ncpcs_common-1.1.4/common/constants/database_config.py
+-rw-r--r--   0 chen       (501) staff       (20)    76288 2024-04-07 01:50:32.000000 ncpcs_common-1.1.4/common/constants/level_dict.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-26 03:10:06.147090 ncpcs_common-1.1.4/common/entity/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.4/common/entity/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      742 2024-03-14 03:04:23.000000 ncpcs_common-1.1.4/common/entity/relation_key.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-26 03:10:06.153889 ncpcs_common-1.1.4/common/service/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.4/common/service/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     1433 2024-02-22 00:30:19.000000 ncpcs_common-1.1.4/common/service/iccc3.py
+-rw-r--r--   0 chen       (501) staff       (20)     3527 2024-04-19 03:22:09.000000 ncpcs_common-1.1.4/common/service/medical_text.py
+-rw-r--r--   0 chen       (501) staff       (20)      604 2024-04-26 02:21:20.000000 ncpcs_common-1.1.4/common/service/multi_thread.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-26 03:10:06.163756 ncpcs_common-1.1.4/common/tests/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.4/common/tests/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     1621 2024-03-13 00:54:29.000000 ncpcs_common-1.1.4/common/tests/test_date_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      493 2024-03-11 01:56:01.000000 ncpcs_common-1.1.4/common/tests/test_encrypt_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      990 2024-02-22 00:30:19.000000 ncpcs_common-1.1.4/common/tests/test_iccc3.py
+-rw-r--r--   0 chen       (501) staff       (20)      259 2024-03-08 06:32:33.000000 ncpcs_common-1.1.4/common/tests/test_id_card_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      238 2024-02-22 00:30:19.000000 ncpcs_common-1.1.4/common/tests/test_list_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     1776 2024-03-14 03:09:57.000000 ncpcs_common-1.1.4/common/tests/test_medical_text.py
+-rw-r--r--   0 chen       (501) staff       (20)      196 2024-03-08 06:32:33.000000 ncpcs_common-1.1.4/common/tests/test_phone_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      248 2024-03-14 03:02:47.000000 ncpcs_common-1.1.4/common/tests/test_relation_key.py
+-rw-r--r--   0 chen       (501) staff       (20)     2692 2024-04-17 00:47:55.000000 ncpcs_common-1.1.4/common/tests/test_sql_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     4194 2024-03-14 08:10:50.000000 ncpcs_common-1.1.4/common/tests/test_string_util.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-26 03:10:06.177163 ncpcs_common-1.1.4/common/util/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2024-02-21 07:50:07.000000 ncpcs_common-1.1.4/common/util/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      316 2024-03-08 07:12:56.000000 ncpcs_common-1.1.4/common/util/csv_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     2200 2024-03-11 01:54:24.000000 ncpcs_common-1.1.4/common/util/database_connection_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     9442 2024-03-25 08:45:23.000000 ncpcs_common-1.1.4/common/util/date_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     1133 2024-03-11 01:01:54.000000 ncpcs_common-1.1.4/common/util/encrypt_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      185 2024-03-07 08:57:18.000000 ncpcs_common-1.1.4/common/util/excel_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     3829 2024-03-08 06:13:07.000000 ncpcs_common-1.1.4/common/util/id_card_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      889 2024-03-20 01:13:40.000000 ncpcs_common-1.1.4/common/util/linux_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      131 2024-02-01 05:44:53.000000 ncpcs_common-1.1.4/common/util/list_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      238 2024-03-08 06:33:15.000000 ncpcs_common-1.1.4/common/util/phone_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     7451 2024-03-27 00:35:28.000000 ncpcs_common-1.1.4/common/util/sql_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     4692 2024-04-26 02:21:20.000000 ncpcs_common-1.1.4/common/util/string_util.py
+-rw-r--r--   0 chen       (501) staff       (20)      497 2024-02-02 06:22:13.000000 ncpcs_common-1.1.4/common/util/timer_util.py
+-rw-r--r--   0 chen       (501) staff       (20)     1315 2024-03-08 06:08:27.000000 ncpcs_common-1.1.4/common/util/zip_util.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2024-04-26 03:10:06.179282 ncpcs_common-1.1.4/ncpcs_common.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      137 2024-04-26 03:10:06.000000 ncpcs_common-1.1.4/ncpcs_common.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)     1199 2024-04-26 03:10:06.000000 ncpcs_common-1.1.4/ncpcs_common.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2024-04-26 03:10:06.000000 ncpcs_common-1.1.4/ncpcs_common.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       51 2024-04-26 03:10:06.000000 ncpcs_common-1.1.4/ncpcs_common.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)        7 2024-04-26 03:10:06.000000 ncpcs_common-1.1.4/ncpcs_common.egg-info/top_level.txt
+-rw-r--r--   0 chen       (501) staff       (20)       38 2024-04-26 03:10:06.181379 ncpcs_common-1.1.4/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      263 2024-04-26 03:07:23.000000 ncpcs_common-1.1.4/setup.py
```

### Comparing `ncpcs_common-1.1.3/common/constants/level_dict.py` & `ncpcs_common-1.1.4/common/constants/level_dict.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/entity/relation_key.py` & `ncpcs_common-1.1.4/common/entity/relation_key.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/service/iccc3.py` & `ncpcs_common-1.1.4/common/service/iccc3.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/service/medical_text.py` & `ncpcs_common-1.1.4/common/service/medical_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
     }
 }
 
 GET_TEXT_SQL_FORMAT = "select {} from {} where nc_medical_institution_code = '{}' and nc_medical_record_no = '{}' and "\
                      "nc_discharge_time = '{}' and nc_hedge = 0 and nc_data_status != 99"
 
 
-def extract_medical_text(cursor, relation_key):
+def extract_medical_text(cursor, relation_key, column_dict=COLUMN_DICT):
     medical_text = []
-    for table_name, column_list in COLUMN_DICT.items():
+    for table_name, column_list in column_dict.items():
         get_text_sql = GET_TEXT_SQL_FORMAT.format(','.join(column_list), table_name, relation_key.medical_institution_code,
                                                   relation_key.medical_record_no, relation_key.discharge_time)
         page_uuid, get_text_sql = generate_order_sql(get_text_sql)
         cursor.execute(get_text_sql)
         page = 1
         for ele in cursor.fetchall():
             medical_text.extend([
```

### Comparing `ncpcs_common-1.1.3/common/tests/test_date_util.py` & `ncpcs_common-1.1.4/common/tests/test_date_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/tests/test_iccc3.py` & `ncpcs_common-1.1.4/common/tests/test_iccc3.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/tests/test_medical_text.py` & `ncpcs_common-1.1.4/common/tests/test_medical_text.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/tests/test_sql_util.py` & `ncpcs_common-1.1.4/common/tests/test_sql_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         assert transfer_database_name_to_hump("nc_admission_record") == 'ncAdmissionRecord'
 
     def test_transfer_hump_to_database_name(self):
         assert transfer_hump_to_database_name("ncAddTime") == 'nc_add_time'
         assert transfer_hump_to_database_name("ncAdmissionRecord") == 'nc_admission_record'
 
     def test_generate_select_sql(self):
-        print(generate_select_sql('ncpcs_medical_data_analyze', 'nc_tumor_desc'))
+        print(generate_select_sql('ncpcs_all', 'nc_pathology_info'))
 
     def test_generate_insert_sql(self):
         # print(generate_insert_sql('ncpcs_tool', 'nc_report_medical_info'))
         print("select distinct nc_iccc3_code, nc_level from nc_tumor_desc UNION " \
                           "select distinct nc_iccc3_code, nc_level from nc_tumor_gtm union select distinct " \
                           "nc_iccc3_code, nc_level from nc_tumor_subtype UNION select distinct nc_iccc3_code, " \
                           "nc_level from nc_tumor_tnm")
```

### Comparing `ncpcs_common-1.1.3/common/tests/test_string_util.py` & `ncpcs_common-1.1.4/common/tests/test_string_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/util/database_connection_util.py` & `ncpcs_common-1.1.4/common/util/database_connection_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/util/date_util.py` & `ncpcs_common-1.1.4/common/util/date_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/util/encrypt_util.py` & `ncpcs_common-1.1.4/common/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/util/id_card_util.py` & `ncpcs_common-1.1.4/common/util/id_card_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/util/linux_util.py` & `ncpcs_common-1.1.4/common/util/linux_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/util/sql_util.py` & `ncpcs_common-1.1.4/common/util/sql_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/common/util/zip_util.py` & `ncpcs_common-1.1.4/common/util/zip_util.py`

 * *Files identical despite different names*

### Comparing `ncpcs_common-1.1.3/ncpcs_common.egg-info/SOURCES.txt` & `ncpcs_common-1.1.4/ncpcs_common.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 common/constants/database_config.py
 common/constants/level_dict.py
 common/entity/__init__.py
 common/entity/relation_key.py
 common/service/__init__.py
 common/service/iccc3.py
 common/service/medical_text.py
+common/service/multi_thread.py
 common/tests/__init__.py
 common/tests/test_date_util.py
 common/tests/test_encrypt_util.py
 common/tests/test_iccc3.py
 common/tests/test_id_card_util.py
 common/tests/test_list_util.py
 common/tests/test_medical_text.py
```

