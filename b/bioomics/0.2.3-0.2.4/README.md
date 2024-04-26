# Comparing `tmp/bioomics-0.2.3.tar.gz` & `tmp/bioomics-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioomics-0.2.3.tar", last modified: Mon Apr 22 17:36:41 2024, max compression
+gzip compressed data, was "bioomics-0.2.4.tar", last modified: Fri Apr 26 20:07:24 2024, max compression
```

## Comparing `bioomics-0.2.3.tar` & `bioomics-0.2.4.tar`

### file list

```diff
@@ -1,43 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:36:41.002068 bioomics-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 17:36:33.000000 bioomics-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-22 17:36:41.002068 bioomics-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-22 17:36:33.000000 bioomics-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 17:36:41.002068 bioomics-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-22 17:36:33.000000 bioomics-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:36:40.994068 bioomics-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:36:40.998068 bioomics-0.2.3/src/bioomics/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:36:40.998068 bioomics-0.2.3/src/bioomics/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/connector/conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/connector/conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/connector/conn_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/connector/conn_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:36:41.002068 bioomics-0.2.3/src/bioomics/constants/
--rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/constants/IEDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/iedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/iedb_antigen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/iedb_epitope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/integrate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 17:36:33.000000 bioomics-0.2.3/src/bioomics/rnacentral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:36:41.002068 bioomics-0.2.3/src/bioomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-22 17:36:40.000000 bioomics-0.2.3/src/bioomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-22 17:36:40.000000 bioomics-0.2.3/src/bioomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:36:40.000000 bioomics-0.2.3/src/bioomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 17:36:40.000000 bioomics-0.2.3/src/bioomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 17:36:40.000000 bioomics-0.2.3/src/bioomics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:36:41.002068 bioomics-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_conn_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_conn_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_iedb.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_iedb_antigen.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_iedb_epitope.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-22 17:36:33.000000 bioomics-0.2.3/tests/test_rnacentral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.984609 bioomics-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 20:07:18.000000 bioomics-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-26 20:07:24.984609 bioomics-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 20:07:18.000000 bioomics-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:07:24.984609 bioomics-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 20:07:18.000000 bioomics-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.976609 bioomics-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.980609 bioomics-0.2.4/src/bioomics/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.980609 bioomics-0.2.4/src/bioomics/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/connector/conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/connector/conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/connector/conn_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/connector/conn_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.980609 bioomics-0.2.4/src/bioomics/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/constants/IEDB.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.980609 bioomics-0.2.4/src/bioomics/immune/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/immune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/immune/iedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/immune/iedb_antigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/immune/iedb_epitope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/integrate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/ncbi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.980609 bioomics-0.2.4/src/bioomics/protein/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/protein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/protein/expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/protein/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/protein/uniprot_sprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/protein/uniprot_trembl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/rnacentral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.984609 bioomics-0.2.4/src/bioomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-26 20:07:24.000000 bioomics-0.2.4/src/bioomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-26 20:07:24.000000 bioomics-0.2.4/src/bioomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:07:24.000000 bioomics-0.2.4/src/bioomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 20:07:24.000000 bioomics-0.2.4/src/bioomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 20:07:24.000000 bioomics-0.2.4/src/bioomics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.984609 bioomics-0.2.4/src/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/pipelines/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/pipelines/retrieve_epitopes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.984609 bioomics-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_conn_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_conn_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_iedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_iedb_antigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_iedb_epitope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_rnacentral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_uniprot_sprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_uniprot_trembl.py
```

### Comparing `bioomics-0.2.3/LICENSE` & `bioomics-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/PKG-INFO` & `bioomics-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.2.3
+Version: 0.2.4
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -19,18 +19,19 @@
 Requires-Dist: lxml
 Requires-Dist: redis
 Requires-Dist: sh
 
 \n# bio_omics
 Download, retrieve and process omics data, or biological informatics data from public database
 
-Comprehensive databases
-- NCBI
+Comprehensive Databases
+- NCBI: genome database, 
+- UniProt: protein database, https://www.expasy.org/resources/uniprotkb-swiss-prot
 
-Sepecific databases
+Sepecific Databases
 - miRBase: mircoRNA database, https://www.mirbase.org/
 - RNACentral: non-coding RNA squence database, https://rnacentral.org/
 - IEDB: immune epitope database, https://www.iedb.org/
 
 
 See the help documents of example coding at https://www.fbridges.com/pipeline/bio_omics.
```

### Comparing `bioomics-0.2.3/README.md` & `bioomics-0.2.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # bio_omics
 Download, retrieve and process omics data, or biological informatics data from public database
 
-Comprehensive databases
-- NCBI
+Comprehensive Databases
+- NCBI: genome database, 
+- UniProt: protein database, https://www.expasy.org/resources/uniprotkb-swiss-prot
 
-Sepecific databases
+Sepecific Databases
 - miRBase: mircoRNA database, https://www.mirbase.org/
 - RNACentral: non-coding RNA squence database, https://rnacentral.org/
 - IEDB: immune epitope database, https://www.iedb.org/
 
 
 See the help documents of example coding at https://www.fbridges.com/pipeline/bio_omics.
```

### Comparing `bioomics-0.2.3/setup.py` & `bioomics-0.2.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="bioomics",
-    version='0.2.3',
+    version='0.2.4',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="Download, retrieve and process omics data for further bioinformatics",
     url = "https://github.com/Tiezhengyuan/bio_omics",
     long_description_content_type="text/markdown",
     long_description=long_description,
     package_dir={"": "src"},
```

### Comparing `bioomics-0.2.3/src/bioomics/connector/conn_ftp.py` & `bioomics-0.2.4/src/bioomics/connector/conn_ftp.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,39 +65,42 @@
         one download one connection avoiding timeout
         '''
         if run_gunzip is None: run_gunzip = True
         Dir(local_path).init_dir()
         local_file = os.path.join(local_path, file_name)
         unzip_file = local_file.replace('.gz', '')
         # doesn't download if file exists and overwrite is False
-        if os.path.isfile(unzip_file) and self.overwrite is False:
-            return unzip_file
+        if self.overwrite is False:
+            if os.path.isfile(unzip_file):
+                return unzip_file
+            elif os.path.isfile(local_file):
+                return local_file
         
         # connect FTP
         ftp = FTP(self.url)
         ftp.login()
         if endpoint:
             ftp.cwd(endpoint)
         ftp_file = f"{self.url}/{endpoint}/{file_name}"
         
         # download
         try:
             with open(local_file, 'wb') as f:
                 ftp.retrbinary(f"RETR {file_name}", f.write)
                 print(f"Download {ftp_file}")
-            # unzip .gz file
-            if run_gunzip and local_file.endswith('gz'):
-                print(f"decompress {local_file} to {unzip_file}")
-                gunzip(local_file, '-f')
-                return unzip_file
-            return local_file
         except Exception as e:
             print('Failure: download data from FTP, error=', e)
             os.remove(local_file)
-        return None
+            local_file = None
+        # unzip .gz file
+        if run_gunzip and local_file and local_file.endswith('gz'):
+            print(f"decompress {local_file} to {unzip_file}")
+            gunzip(local_file, '-f')
+            return unzip_file
+        return local_file
     
     def download_files(self,
             endpoint:str=None,
             match:str=None,
             local_path:str=None,
         ):
         '''
```

### Comparing `bioomics-0.2.3/src/bioomics/connector/conn_ftplib.py` & `bioomics-0.2.4/src/bioomics/connector/conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/src/bioomics/connector/conn_http.py` & `bioomics-0.2.4/src/bioomics/connector/conn_http.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/src/bioomics/connector/conn_redis.py` & `bioomics-0.2.4/src/bioomics/connector/conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/src/bioomics/constants/IEDB.py` & `bioomics-0.2.4/src/bioomics/constants/IEDB.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/src/bioomics/expasy.py` & `bioomics-0.2.4/src/bioomics/protein/expasy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 FTP of ExPASy: ftp.expasy.org
 """
 import os
-from .connector.conn_ftp import ConnFTP
+from ..connector.conn_ftp import ConnFTP
 
 class Expasy(ConnFTP):
     url = "ftp.expasy.org"
 
     def __init__(self, local_dir:str, overwrite:bool=None):
         super().__init__(url=self.url, overwrite=overwrite)
         self.local_dir = os.path.join(local_dir, 'ExPASy')
```

### Comparing `bioomics-0.2.3/src/bioomics/iedb.py` & `bioomics-0.2.4/src/bioomics/immune/iedb.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 '''
 from biosequtils import Dir
 import json
 import os
 import pandas as pd
 import numpy as np
 
-from .connector.conn_http import ConnHTTP
+from ..connector.conn_http import ConnHTTP
 
 
 class IEDB:
     url = "https://www.iedb.org"
     source = "IEDB"
     meta_file_name = 'IEDB_meta.json'
 
     def __init__(self, local_path:str, version:str=None, overwrite:bool=None):
+        '''
+        args: mode: normal(default), debug, update
+        '''
         self.local_path = local_path
         Dir(self.local_path).init_dir()
         self.version = 'v3' if version is None else version
         self.overwrite = overwrite
         self.get_meta()
     
     def get_meta(self):
@@ -369,14 +372,15 @@
     def convert_data(self, data_list:list, unique_key:str) -> dict:
         '''
         convert list to dict
         detect duplicates and invalid identifier
         '''
         entity_data = {}
         for data in data_list:
+            data['source'] = self.source
             ids = self.retrieve_ids(data)
             data.update(ids)
             # detect unique key
             if unique_key in data:
                 key = ids[unique_key]
                 entity_data[key] = data
             else:
```

### Comparing `bioomics-0.2.3/src/bioomics/iedb_antigen.py` & `bioomics-0.2.4/src/bioomics/immune/iedb_antigen.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 antigen --- eptope --- BCR/TCR/BCell/TCell/MHC
 '''
 from biosequtils import Dir
 import os
 import json
 from .iedb import IEDB
-from .integrate_data import IntegrateData
+from ..integrate_data import IntegrateData
 
 class IEDBAntigen(IEDB):
     key = 'accession'
 
     def __init__(self, local_path:str):
         super().__init__(local_path, None, False)
         self.meta['entity'] = 'antigen'
```

### Comparing `bioomics-0.2.3/src/bioomics/iedb_epitope.py` & `bioomics-0.2.4/src/bioomics/immune/iedb_epitope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 '''
-build data mapping of antigen from IEDB
+build data mapping of epitopes from IEDB
+entity is proteins with epitopes
 '''
 from biosequtils import Dir
 import os
-import json
+
 from .iedb import IEDB
-from .integrate_data import IntegrateData
+from ..integrate_data import IntegrateData
 
 class IEDBEpitope(IEDB):
     key = 'accession'
 
-    def __init__(self, local_path:str):
+    def __init__(self, local_path:str, entity_path:str=None):
         super().__init__(local_path, None, False)
         self.meta['entity'] = 'epitope'
-        self.meta['entity_path'] = os.path.join(self.meta['local_path'], 'epitope')
+        self.meta['entity_path'] = entity_path if entity_path \
+            else os.path.join(self.meta['local_path'], 'epitope')
         Dir(self.meta['entity_path']).init_dir()
         self.integrate = None
     
     def process(self):
         self.integrate = IntegrateData(self.meta['entity_path'])
 
         print("Process epitopes")
```

### Comparing `bioomics-0.2.3/src/bioomics/integrate_data.py` & `bioomics-0.2.4/src/bioomics/integrate_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,39 +3,70 @@
 from biosequtils import Dir
 import os
 import json
 import math
 from typing import Iterable
 
 class IntegrateData:
-    def __init__(self, local_path:str):
-        self.local_path = local_path
+    def __init__(self, entity_path:str):
+        '''
+        args: entity_path: store integrated data.
+        '''
+        self.entity_path = entity_path
+        Dir(self.entity_path).init_dir()
         self.index_meta = self.get_index_meta()
 
     def get_index_meta(self) -> dict:
         '''
+        self.index_meta
         key: a certain accession
         value: dictionary
         '''
-        self.index_meta_file = os.path.join(self.local_path, 'index_meta.json')
+        self.index_meta_file = os.path.join(self.entity_path, 'index_meta.json')
         if os.path.isfile(self.index_meta_file):
             with open(self.index_meta_file, 'r') as f:
                 index_meta = json.load(f)
                 return index_meta
         return {}
 
     def save_index_meta(self, input:dict=None) -> bool:
         if isinstance(input, dict):
             self.index_meta.update(input)
         if self.index_meta:
             with open(self.index_meta_file, 'w') as f:
                 json.dump(self.index_meta, f, indent=4)
             return True
         return False
-    
+
+    def get_meta(self, updated_meta:dict):
+        '''
+        meta varies by database
+        '''
+        meta = {}
+        source = meta.get('source', '')
+        meta_file = os.path.join(self.entity_path, f"{source}_meta.json")
+        if os.path.isfile(meta_file):
+            print('get meta.')
+            with open(meta_file, 'r') as f:
+                meta = json.load(f)
+        else:
+            meta = {
+                'entity_path': self.entity_path,
+                'index_meta_file': self.index_meta_file,
+                'meta_file': meta_file,
+            }
+        # update meta
+        meta.update(updated_meta)
+        return meta
+
+    def save_meta(self, meta:dict):
+        with open(meta['meta_file'], 'w') as f:
+            json.dump(meta, f, indent=4)
+        return meta['meta_file']
+        
     def scan(self) -> Iterable:
         '''
         Note: self.index_meta could be updated
         ?? memroy leak
         '''
         files = [i['json_file'] for i in self.index_meta.values() if 'json_file' in i]
         for file in files:
@@ -53,15 +84,15 @@
     def new_json_path(self, new_id:str) -> str:
         '''
         id = '1234'
         path: ./12/34/1234.json
         '''
         id_prefix = str(math.floor(int(new_id)/1000))
         sub_dirs = [id_prefix[i:i+2] for i in range(0, len(id_prefix), 2)]
-        path = os.path.join(self.local_path, *sub_dirs)
+        path = os.path.join(self.entity_path, *sub_dirs)
         Dir(path).init_dir()
         json_file = os.path.join(path, f'{new_id}.json')
         return json_file
     
     def add_data(self, data:dict, key_value:str=None):
         '''
         'key' and 'ID' are added into new data
```

### Comparing `bioomics-0.2.3/src/bioomics/mirbase.py` & `bioomics-0.2.4/src/bioomics/mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/src/bioomics/ncbi.py` & `bioomics-0.2.4/src/bioomics/ncbi.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/src/bioomics/rnacentral.py` & `bioomics-0.2.4/src/bioomics/rnacentral.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/src/bioomics.egg-info/PKG-INFO` & `bioomics-0.2.4/src/bioomics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.2.3
+Version: 0.2.4
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -19,18 +19,19 @@
 Requires-Dist: lxml
 Requires-Dist: redis
 Requires-Dist: sh
 
 \n# bio_omics
 Download, retrieve and process omics data, or biological informatics data from public database
 
-Comprehensive databases
-- NCBI
+Comprehensive Databases
+- NCBI: genome database, 
+- UniProt: protein database, https://www.expasy.org/resources/uniprotkb-swiss-prot
 
-Sepecific databases
+Sepecific Databases
 - miRBase: mircoRNA database, https://www.mirbase.org/
 - RNACentral: non-coding RNA squence database, https://rnacentral.org/
 - IEDB: immune epitope database, https://www.iedb.org/
 
 
 See the help documents of example coding at https://www.fbridges.com/pipeline/bio_omics.
```

### Comparing `bioomics-0.2.3/tests/test_conn_ftp.py` & `bioomics-0.2.4/tests/test_conn_ftp.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/tests/test_conn_ftplib.py` & `bioomics-0.2.4/tests/test_conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/tests/test_conn_http.py` & `bioomics-0.2.4/tests/test_conn_http.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/tests/test_conn_redis.py` & `bioomics-0.2.4/tests/test_conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/tests/test_iedb.py` & `bioomics-0.2.4/tests/test_iedb.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/tests/test_mirbase.py` & `bioomics-0.2.4/tests/test_mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/tests/test_ncbi.py` & `bioomics-0.2.4/tests/test_ncbi.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.3/tests/test_rnacentral.py` & `bioomics-0.2.4/tests/test_rnacentral.py`

 * *Files identical despite different names*

