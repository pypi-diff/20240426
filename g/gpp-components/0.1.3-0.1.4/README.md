# Comparing `tmp/gpp_components-0.1.3.tar.gz` & `tmp/gpp_components-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpp_components-0.1.3.tar", last modified: Wed Apr 17 06:43:32 2024, max compression
+gzip compressed data, was "gpp_components-0.1.4.tar", last modified: Fri Apr 26 02:55:11 2024, max compression
```

## Comparing `gpp_components-0.1.3.tar` & `gpp_components-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:43:32.665585 gpp_components-0.1.3/
--rw-rw-rw-   0        0        0     1097 2024-01-24 04:54:41.000000 gpp_components-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      412 2024-04-17 06:43:32.657586 gpp_components-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       58 2024-01-24 04:54:41.000000 gpp_components-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 06:43:32.470559 gpp_components-0.1.3/gpp_components/
--rw-rw-rw-   0        0        0       19 2024-01-24 04:54:41.000000 gpp_components-0.1.3/gpp_components/__init__.py
--rw-rw-rw-   0        0        0     1076 2024-01-24 04:54:41.000000 gpp_components-0.1.3/gpp_components/aes.py
--rw-rw-rw-   0        0        0      239 2024-01-26 05:10:34.000000 gpp_components-0.1.3/gpp_components/constant.py
--rw-rw-rw-   0        0        0     4442 2024-01-24 04:54:41.000000 gpp_components-0.1.3/gpp_components/dbConfig.py
--rw-rw-rw-   0        0        0     2535 2024-04-02 12:30:35.000000 gpp_components-0.1.3/gpp_components/decorator.py
--rw-rw-rw-   0        0        0     9366 2024-04-17 06:41:00.000000 gpp_components-0.1.3/gpp_components/fileImporter.py
--rw-rw-rw-   0        0        0     7692 2024-04-17 06:42:48.000000 gpp_components-0.1.3/gpp_components/handleData.py
--rw-rw-rw-   0        0        0     1629 2024-01-24 04:54:41.000000 gpp_components-0.1.3/gpp_components/lazyImport.py
--rw-rw-rw-   0        0        0     1422 2024-03-04 01:22:22.000000 gpp_components-0.1.3/gpp_components/response.py
--rw-rw-rw-   0        0        0     5115 2024-04-17 06:41:00.000000 gpp_components-0.1.3/gpp_components/runOracle.py
--rw-rw-rw-   0        0        0     2880 2024-01-24 04:54:41.000000 gpp_components-0.1.3/gpp_components/sendMail.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:43:32.622683 gpp_components-0.1.3/gpp_components.egg-info/
--rw-rw-rw-   0        0        0      412 2024-04-17 06:43:31.000000 gpp_components-0.1.3/gpp_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2024-04-17 06:43:31.000000 gpp_components-0.1.3/gpp_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:43:31.000000 gpp_components-0.1.3/gpp_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-17 06:43:31.000000 gpp_components-0.1.3/gpp_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-17 06:43:31.000000 gpp_components-0.1.3/gpp_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 06:43:32.669591 gpp_components-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-04-17 06:42:48.000000 gpp_components-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:55:11.067385 gpp_components-0.1.4/
+-rw-rw-rw-   0        0        0     1097 2024-01-24 04:54:41.000000 gpp_components-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      412 2024-04-26 02:55:11.061618 gpp_components-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2024-01-24 04:54:41.000000 gpp_components-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 02:55:10.976572 gpp_components-0.1.4/gpp_components/
+-rw-rw-rw-   0        0        0       19 2024-01-24 04:54:41.000000 gpp_components-0.1.4/gpp_components/__init__.py
+-rw-rw-rw-   0        0        0     1076 2024-01-24 04:54:41.000000 gpp_components-0.1.4/gpp_components/aes.py
+-rw-rw-rw-   0        0        0      239 2024-01-26 05:10:34.000000 gpp_components-0.1.4/gpp_components/constant.py
+-rw-rw-rw-   0        0        0     4442 2024-01-24 04:54:41.000000 gpp_components-0.1.4/gpp_components/dbConfig.py
+-rw-rw-rw-   0        0        0     2535 2024-04-02 12:30:35.000000 gpp_components-0.1.4/gpp_components/decorator.py
+-rw-rw-rw-   0        0        0     9440 2024-04-26 02:54:25.000000 gpp_components-0.1.4/gpp_components/fileImporter.py
+-rw-rw-rw-   0        0        0     7692 2024-04-17 06:42:48.000000 gpp_components-0.1.4/gpp_components/handleData.py
+-rw-rw-rw-   0        0        0     1629 2024-01-24 04:54:41.000000 gpp_components-0.1.4/gpp_components/lazyImport.py
+-rw-rw-rw-   0        0        0     1422 2024-03-04 01:22:22.000000 gpp_components-0.1.4/gpp_components/response.py
+-rw-rw-rw-   0        0        0     5115 2024-04-17 06:41:00.000000 gpp_components-0.1.4/gpp_components/runOracle.py
+-rw-rw-rw-   0        0        0     2880 2024-01-24 04:54:41.000000 gpp_components-0.1.4/gpp_components/sendMail.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:55:11.053330 gpp_components-0.1.4/gpp_components.egg-info/
+-rw-rw-rw-   0        0        0      412 2024-04-26 02:55:09.000000 gpp_components-0.1.4/gpp_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2024-04-26 02:55:09.000000 gpp_components-0.1.4/gpp_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 02:55:09.000000 gpp_components-0.1.4/gpp_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-26 02:55:09.000000 gpp_components-0.1.4/gpp_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-26 02:55:09.000000 gpp_components-0.1.4/gpp_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 02:55:11.068381 gpp_components-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-04-26 02:54:40.000000 gpp_components-0.1.4/setup.py
```

### Comparing `gpp_components-0.1.3/LICENSE` & `gpp_components-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.3/gpp_components/aes.py` & `gpp_components-0.1.4/gpp_components/aes.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.3/gpp_components/dbConfig.py` & `gpp_components-0.1.4/gpp_components/dbConfig.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.3/gpp_components/decorator.py` & `gpp_components-0.1.4/gpp_components/decorator.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.3/gpp_components/fileImporter.py` & `gpp_components-0.1.4/gpp_components/fileImporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,17 @@
         "lob_group":"Client"
       }
     }
     """
 
     def importData(self):
         table_data = self.loadFile(self.jsonStr)
-        # DB 操作
-        res = self.executeDB(self.jsonStr, table_data)
+        if not table_data.empty:
+            # DB 操作
+            res = self.executeDB(self.jsonStr, table_data)
         if res:
             return Response(success=False, msg=str(res), data=[])
         else:
             return Response(success=True, data=[])
 
     def executeDB(self, obj, table_data):
         """
@@ -121,15 +122,17 @@
         if db_type == "Oracle":
             if dsn:
                 conn = odb.connect(user=user_name, password=password, dsn=dsn)
             else:
                 conn_str = f"{user_name}/{password}@{host_name}/{service_name}"
                 conn = odb.connect(conn_str)
         elif db_type == "SQL":
-            conn = sqla.create_engine(f"mssql+pymssql://{user_name}:{password}@{host_name}/{service_name}?charset=utf8").connect()
+            conn = sqla.create_engine(
+                f"mssql+pymssql://{user_name}:{password}@{host_name}/{service_name}?charset=utf8"
+            ).connect()
 
         return conn
 
     def rebuildSQL(self, table_name, columns, db_type):
         """
         table_name:
         columns:['ORDERNUM', 'QTY']
```

### Comparing `gpp_components-0.1.3/gpp_components/handleData.py` & `gpp_components-0.1.4/gpp_components/handleData.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.3/gpp_components/lazyImport.py` & `gpp_components-0.1.4/gpp_components/lazyImport.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.3/gpp_components/response.py` & `gpp_components-0.1.4/gpp_components/response.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.3/gpp_components/runOracle.py` & `gpp_components-0.1.4/gpp_components/runOracle.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.3/gpp_components/sendMail.py` & `gpp_components-0.1.4/gpp_components/sendMail.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.3/gpp_components.egg-info/SOURCES.txt` & `gpp_components-0.1.4/gpp_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.3/setup.py` & `gpp_components-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gpp_components",
-    version = '0.1.3',
+    version = '0.1.4',
     # version="0.0.36", # last version for Py310
     #
     author="L",
     description="for internal use",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT Licence",
```

