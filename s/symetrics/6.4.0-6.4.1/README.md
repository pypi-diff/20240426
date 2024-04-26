# Comparing `tmp/symetrics-6.4.0.tar.gz` & `tmp/symetrics-6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symetrics-6.4.0.tar", last modified: Wed Jan 31 09:20:32 2024, max compression
+gzip compressed data, was "symetrics-6.4.1.tar", last modified: Fri Apr 26 00:42:05 2024, max compression
```

## Comparing `symetrics-6.4.0.tar` & `symetrics-6.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-31 09:20:32.485300 symetrics-6.4.0/
--rw-rw-rw-   0        0        0     1151 2024-01-31 09:20:32.485300 symetrics-6.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-01-31 09:20:32.485300 symetrics-6.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1640 2024-01-31 09:20:17.000000 symetrics-6.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-31 09:20:32.459657 symetrics-6.4.0/symetrics/
--rw-rw-rw-   0        0        0      101 2023-12-09 13:09:42.000000 symetrics-6.4.0/symetrics/__init__.py
--rw-rw-rw-   0        0        0      519 2023-12-09 13:09:33.000000 symetrics-6.4.0/symetrics/dbcontext.py
-drwxrwxrwx   0        0        0        0 2024-01-31 09:20:32.476072 symetrics-6.4.0/symetrics/src/
--rw-rw-rw-   0        0        0       25 2023-10-25 09:08:07.000000 symetrics-6.4.0/symetrics/src/__init__.py
--rw-rw-rw-   0        0        0      967 2024-01-31 08:23:38.000000 symetrics-6.4.0/symetrics/src/datastruct.py
--rw-rw-rw-   0        0        0    20346 2024-01-31 09:19:14.000000 symetrics-6.4.0/symetrics/symetrics_api.py
-drwxrwxrwx   0        0        0        0 2024-01-31 09:20:32.476072 symetrics-6.4.0/symetrics.egg-info/
--rw-rw-rw-   0        0        0     1151 2024-01-31 09:20:32.000000 symetrics-6.4.0/symetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-01-31 09:20:32.000000 symetrics-6.4.0/symetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-31 09:20:32.000000 symetrics-6.4.0/symetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-01-31 09:20:32.000000 symetrics-6.4.0/symetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-31 09:20:32.000000 symetrics-6.4.0/symetrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 00:42:05.135994 symetrics-6.4.1/
+-rw-rw-rw-   0        0        0     1151 2024-04-26 00:42:05.135994 symetrics-6.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-26 00:42:05.135994 symetrics-6.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1640 2024-04-26 00:41:49.000000 symetrics-6.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:42:05.090962 symetrics-6.4.1/symetrics/
+-rw-rw-rw-   0        0        0      101 2023-12-09 13:09:42.000000 symetrics-6.4.1/symetrics/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-12-09 13:09:33.000000 symetrics-6.4.1/symetrics/dbcontext.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:42:05.133987 symetrics-6.4.1/symetrics/src/
+-rw-rw-rw-   0        0        0       25 2023-10-25 09:08:07.000000 symetrics-6.4.1/symetrics/src/__init__.py
+-rw-rw-rw-   0        0        0      967 2024-01-31 08:23:38.000000 symetrics-6.4.1/symetrics/src/datastruct.py
+-rw-rw-rw-   0        0        0    20747 2024-04-26 00:35:20.000000 symetrics-6.4.1/symetrics/symetrics_api.py
+drwxrwxrwx   0        0        0        0 2024-04-26 00:42:05.131347 symetrics-6.4.1/symetrics.egg-info/
+-rw-rw-rw-   0        0        0     1151 2024-04-26 00:42:04.000000 symetrics-6.4.1/symetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-04-26 00:42:04.000000 symetrics-6.4.1/symetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 00:42:04.000000 symetrics-6.4.1/symetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-26 00:42:04.000000 symetrics-6.4.1/symetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-26 00:42:04.000000 symetrics-6.4.1/symetrics.egg-info/top_level.txt
```

### Comparing `symetrics-6.4.0/PKG-INFO` & `symetrics-6.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symetrics
-Version: 6.4.0
+Version: 6.4.1
 Summary: Symetrics API
 Home-page: https://lbundalian.github.io/symetrics/
 Author: Linnaeus Bundalian
 Author-email: linnaeusbundalian@gmail.com
 Keywords: python,synonymous variants
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `symetrics-6.4.0/setup.py` & `symetrics-6.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '6.4.0' 
+VERSION = '6.4.1' 
 DESCRIPTION = 'Symetrics API'
 LONG_DESCRIPTION = '''A package to access SYMETRICS database. 
 SYMETRICS database is a consolidation of metrics for synonymous variants which were derived from a number of computational tools each of which contributing to 
 attribute specific metrics such as SYNVEP for general functional constraints, SpliceAI for splicing effect, SILVA for obtaining GERP++ (phylogenetic related constraints)
 CpG/CpG_Exon, dRSCU/RSCU for codon usage and SURF for rna stability. The package also includes a result of the analysis of the influence of each variants exceeding set threshold
 per metrics defined constituting to a score assigned to a gene'''
 REQUIRED_PACKAGES = [
```

### Comparing `symetrics-6.4.0/symetrics/dbcontext.py` & `symetrics-6.4.1/symetrics/dbcontext.py`

 * *Files identical despite different names*

### Comparing `symetrics-6.4.0/symetrics/src/datastruct.py` & `symetrics-6.4.1/symetrics/src/datastruct.py`

 * *Files identical despite different names*

### Comparing `symetrics-6.4.0/symetrics/symetrics_api.py` & `symetrics-6.4.1/symetrics/symetrics_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,29 +87,33 @@
         """
 
         silva_scores = None
         try:
             # dont forget silva is hg19
             with self._db as dbhandler:
                 silva_cursor = dbhandler._conn.cursor()
-                silva_query = f'SELECT "#chrom" AS CHR,pos AS POS,ref AS REF,alt AS ALT,gene AS GENE,"#RSCU" AS RSCU,dRSCU,"#GERP++" AS GERP,"#CpG?" AS CPG,CpG_exon AS CPGX FROM SILVA WHERE "#chrom" = {variant._chr} AND pos = {variant._pos} AND ref = "{variant._ref}" AND alt = "{variant._alt}"'
+                #silva_query = f'SELECT "#chrom" AS CHR,pos AS POS,ref AS REF,alt AS ALT,gene AS GENE,"#RSCU" AS RSCU,dRSCU,"#GERP++" AS GERP,"#CpG?" AS CPG,CpG_exon AS CPGX FROM SILVA WHERE "#chrom" = {variant._chr} AND pos = {variant._pos} AND ref = "{variant._ref}" AND alt = "{variant._alt}"'
+                #silva_query = f'SELECT * FROM SILVA WHERE "#chrom" = {variant._chr} AND pos = {variant._pos} AND ref = "{variant._ref}" AND alt = "{variant._alt}"'
+                silva_query = f'SELECT * FROM SILVA_SCORE WHERE CHROM = {variant._chr} AND POS = {variant._pos} AND REF = "{variant._ref}" AND ALT = "{variant._alt}"'
+                
                 silva_cursor.execute(silva_query)
                 silva_rows = silva_cursor.fetchall()
                 silva_scores = silva_rows[0]
                 silva_scores = {
                     "CHR": silva_scores[0],
                     "POS": silva_scores[1],
-                    "REF": silva_scores[2],
-                    "ALT": silva_scores[3],
-                    "GENE": silva_scores[4],
-                    "RSCU": silva_scores[5],
-                    "dRSCU": silva_scores[6],
+                    "REF": silva_scores[3],
+                    "ALT": silva_scores[4],
+                    "GENE": silva_scores[5],
+                    "RSCU": silva_scores[8],
+                    "dRSCU": silva_scores[9],
                     "GERP": silva_scores[7],
-                    "CPG": silva_scores[8],
-                    "CPGX": silva_scores[9]
+                    "MES": silva_scores[12],
+                    "CPG": silva_scores[10],
+                    "CPGX": silva_scores[11]
                 }
 
         except Error as e:
             logging.error(f"Connection to {self._db} failed")
```

### Comparing `symetrics-6.4.0/symetrics.egg-info/PKG-INFO` & `symetrics-6.4.1/symetrics.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symetrics
-Version: 6.4.0
+Version: 6.4.1
 Summary: Symetrics API
 Home-page: https://lbundalian.github.io/symetrics/
 Author: Linnaeus Bundalian
 Author-email: linnaeusbundalian@gmail.com
 Keywords: python,synonymous variants
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

