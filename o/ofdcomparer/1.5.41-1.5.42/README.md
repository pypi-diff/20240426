# Comparing `tmp/ofdcomparer-1.5.41.tar.gz` & `tmp/ofdcomparer-1.5.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofdcomparer-1.5.41.tar", last modified: Thu Apr 11 15:38:06 2024, max compression
+gzip compressed data, was "ofdcomparer-1.5.42.tar", last modified: Fri Apr 26 16:04:32 2024, max compression
```

## Comparing `ofdcomparer-1.5.41.tar` & `ofdcomparer-1.5.42.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:38:06.792370 ofdcomparer-1.5.41/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-20 08:16:51.000000 ofdcomparer-1.5.41/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1567 2024-04-11 15:38:06.792370 ofdcomparer-1.5.41/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-06 21:06:45.000000 ofdcomparer-1.5.41/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:38:06.790370 ofdcomparer-1.5.41/ofdcomparer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-20 08:16:51.000000 ofdcomparer-1.5.41/ofdcomparer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-12 07:39:03.000000 ofdcomparer-1.5.41/ofdcomparer/allure_helper.py
--rw-rw-rw-   0 root         (0) root         (0)    21525 2024-04-11 05:15:32.000000 ofdcomparer-1.5.41/ofdcomparer/compare_ffd.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-11 05:15:32.000000 ofdcomparer-1.5.41/ofdcomparer/configs.py
--rw-rw-rw-   0 root         (0) root         (0)    13995 2024-04-11 05:15:32.000000 ofdcomparer-1.5.41/ofdcomparer/convert.py
--rw-rw-rw-   0 root         (0) root         (0)    39684 2024-04-11 15:37:51.000000 ofdcomparer-1.5.41/ofdcomparer/dto10.py
--rw-rw-rw-   0 root         (0) root         (0)    38192 2024-04-11 05:15:32.000000 ofdcomparer-1.5.41/ofdcomparer/dto_error_descriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8301 2024-01-25 10:39:56.000000 ofdcomparer-1.5.41/ofdcomparer/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-11 15:37:51.000000 ofdcomparer-1.5.41/ofdcomparer/ofd_cri_atol.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-12 14:13:15.000000 ofdcomparer-1.5.41/ofdcomparer/ofd_taxcom.py
--rw-rw-rw-   0 root         (0) root         (0)    40219 2024-04-11 05:15:32.000000 ofdcomparer-1.5.41/ofdcomparer/tags_fn.py
--rw-rw-rw-   0 root         (0) root         (0)    10168 2024-04-11 05:15:32.000000 ofdcomparer-1.5.41/ofdcomparer/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:38:06.791370 ofdcomparer-1.5.41/ofdcomparer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2024-04-11 15:38:06.000000 ofdcomparer-1.5.41/ofdcomparer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2024-04-11 15:38:06.000000 ofdcomparer-1.5.41/ofdcomparer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 15:38:06.000000 ofdcomparer-1.5.41/ofdcomparer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-11 15:38:06.000000 ofdcomparer-1.5.41/ofdcomparer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-11 15:38:06.000000 ofdcomparer-1.5.41/ofdcomparer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-11 15:38:06.792370 ofdcomparer-1.5.41/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-11 15:37:51.000000 ofdcomparer-1.5.41/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:04:32.066263 ofdcomparer-1.5.42/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 22:27:07.000000 ofdcomparer-1.5.42/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-04-26 16:04:32.066263 ofdcomparer-1.5.42/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-15 14:23:23.000000 ofdcomparer-1.5.42/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:04:32.065263 ofdcomparer-1.5.42/ofdcomparer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 22:27:07.000000 ofdcomparer-1.5.42/ofdcomparer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-20 12:23:39.000000 ofdcomparer-1.5.42/ofdcomparer/allure_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    21525 2024-04-04 19:15:02.000000 ofdcomparer-1.5.42/ofdcomparer/compare_ffd.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/configs.py
+-rw-rw-rw-   0 root         (0) root         (0)    13995 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)    39684 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/dto10.py
+-rw-rw-rw-   0 root         (0) root         (0)    38192 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/dto_error_descriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8301 2024-03-06 23:14:00.000000 ofdcomparer-1.5.42/ofdcomparer/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/ofd_cri_atol.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-20 12:23:39.000000 ofdcomparer-1.5.42/ofdcomparer/ofd_taxcom.py
+-rw-rw-rw-   0 root         (0) root         (0)    40745 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/tags_fn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10168 2024-04-04 19:15:02.000000 ofdcomparer-1.5.42/ofdcomparer/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:04:32.066263 ofdcomparer-1.5.42/ofdcomparer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-04-26 16:04:32.000000 ofdcomparer-1.5.42/ofdcomparer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2024-04-26 16:04:32.000000 ofdcomparer-1.5.42/ofdcomparer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 16:04:32.000000 ofdcomparer-1.5.42/ofdcomparer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-26 16:04:32.000000 ofdcomparer-1.5.42/ofdcomparer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-26 16:04:32.000000 ofdcomparer-1.5.42/ofdcomparer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-26 16:04:32.067263 ofdcomparer-1.5.42/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/setup.py
```

### Comparing `ofdcomparer-1.5.41/PKG-INFO` & `ofdcomparer-1.5.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.41
+Version: 1.5.42
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.41/README.md` & `ofdcomparer-1.5.42/README.md`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.41/ofdcomparer/compare_ffd.py` & `ofdcomparer-1.5.42/ofdcomparer/compare_ffd.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.41/ofdcomparer/convert.py` & `ofdcomparer-1.5.42/ofdcomparer/convert.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.41/ofdcomparer/dto10.py` & `ofdcomparer-1.5.42/ofdcomparer/dto10.py`

 * *Files 0% similar despite different names*

```diff
@@ -562,15 +562,15 @@
         if ofdExchangeStatus is not None:
             not_sent_fd_qty = ofdExchangeStatus["status"]["notSentCount"]
             logging.debug(f"get_not_sent_fd_qty() %s", not_sent_fd_qty)
             return not_sent_fd_qty
         logging.debug(f"get_not_sent_fd_qty() None")
         return None
 
-    def wait_for_sent_all_fd(self, timeout: int = 300):
+    def wait_for_sent_all_fd(self, timeout: int = 180):
         logging.debug(f"wait_for_sent_all_fd() timeout %s", timeout)
         start_time = time.time()
         while self.get_not_sent_fd_qty() != 0:
             if (time.time() - start_time) == (timeout/2):
                 self.print_document_copy()
             elif time.time() - start_time > timeout:
                 logging.debug(f"get_not_sent_fd_qty() False")
```

### Comparing `ofdcomparer-1.5.41/ofdcomparer/dto_error_descriptions.py` & `ofdcomparer-1.5.42/ofdcomparer/dto_error_descriptions.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.41/ofdcomparer/helpers.py` & `ofdcomparer-1.5.42/ofdcomparer/helpers.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.41/ofdcomparer/ofd_cri_atol.py` & `ofdcomparer-1.5.42/ofdcomparer/ofd_cri_atol.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.41/ofdcomparer/ofd_taxcom.py` & `ofdcomparer-1.5.42/ofdcomparer/ofd_taxcom.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.41/ofdcomparer/tags_fn.py` & `ofdcomparer-1.5.42/ofdcomparer/tags_fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -802,14 +802,34 @@
         "Name": "признак осуществления страховой деятельности",
     },
     "1260": {
         "Type": STLV,
         "Head": "отраслевой реквизит предмета расчета",
         "Name": "отраслевой реквизит предмета расчета",
     },
+    "1262": {
+        "Type": STRING,
+        "Head": "",
+        "Name": "идентификатор ФОИВ",
+    },
+    "1263": {
+        "Type": STRING,
+        "Head": "",
+        "Name": "дата документа основания",
+    },
+    "1264": {
+        "Type": STRING,
+        "Head": "",
+        "Name": "номер докумена основания",
+    },
+    "1265": {
+        "Type": STRING,
+        "Head": "",
+        "Name": "значение отраслевого реквизита",
+    },
     "1290": {
         "Type": BITS,
         "Head": "",
         "Name": "признаки условий применения ККТ",
         "BIT1": "ПРИНТЕР В АВТОМАТЕ",
         "BIT2": "АС БСО",
         "BIT5": "ККТ ДЛЯ ИНТЕРНЕТ",
@@ -932,7 +952,8 @@
     },
     "short": {
         "Type": STRING,
         "Head": "",
         "Name": "Признак того, что документ считался из архива и содержит неполный набор данных",
     },
 }
+
```

### Comparing `ofdcomparer-1.5.41/ofdcomparer/utils.py` & `ofdcomparer-1.5.42/ofdcomparer/utils.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.41/ofdcomparer.egg-info/PKG-INFO` & `ofdcomparer-1.5.42/ofdcomparer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.41
+Version: 1.5.42
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.41/ofdcomparer.egg-info/SOURCES.txt` & `ofdcomparer-1.5.42/ofdcomparer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.41/setup.py` & `ofdcomparer-1.5.42/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ofdcomparer",
-    version="1.5.41",
+    version="1.5.42",
     long_description=long_description,
     description="Библиотека для сравнивания ФД из ФН и ОФД",
     packages=["ofdcomparer"],
     author_email="k.kabisova@atol.ru",
     install_requires=[
         "requests==2.31.0",
         "requests-toolbelt==1.0.0",
```

