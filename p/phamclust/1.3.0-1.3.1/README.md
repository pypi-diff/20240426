# Comparing `tmp/phamclust-1.3.0.tar.gz` & `tmp/phamclust-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phamclust-1.3.0.tar", last modified: Thu Apr 25 20:39:38 2024, max compression
+gzip compressed data, was "phamclust-1.3.1.tar", last modified: Fri Apr 26 13:35:40 2024, max compression
```

## Comparing `phamclust-1.3.0.tar` & `phamclust-1.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-25 20:39:38.194760 phamclust-1.3.0/
--rw-r--r--   0 cgauthier   (501) staff       (20)    35148 2024-01-30 13:49:10.000000 phamclust-1.3.0/LICENSE
--rw-r--r--   0 cgauthier   (501) staff       (20)    10739 2024-04-25 20:39:38.194611 phamclust-1.3.0/PKG-INFO
--rw-r--r--   0 cgauthier   (501) staff       (20)     9457 2024-04-25 20:17:00.000000 phamclust-1.3.0/README.md
--rw-r--r--   0 cgauthier   (501) staff       (20)       89 2024-01-30 13:49:10.000000 phamclust-1.3.0/pyproject.toml
--rw-r--r--   0 cgauthier   (501) staff       (20)     1400 2024-04-25 20:39:38.195264 phamclust-1.3.0/setup.cfg
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-25 20:39:38.179794 phamclust-1.3.0/src/
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-25 20:39:38.189913 phamclust-1.3.0/src/phamclust/
--rw-r--r--   0 cgauthier   (501) staff       (20)       69 2024-01-30 13:49:10.000000 phamclust-1.3.0/src/phamclust/__init__.py
--rw-r--r--   0 cgauthier   (501) staff       (20)      130 2024-03-05 13:51:35.000000 phamclust-1.3.0/src/phamclust/__main__.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     5478 2024-04-25 20:19:39.000000 phamclust-1.3.0/src/phamclust/blastn.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     6397 2024-04-25 18:43:50.000000 phamclust-1.3.0/src/phamclust/cli.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     1911 2024-02-21 18:41:57.000000 phamclust-1.3.0/src/phamclust/clustering.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     2409 2024-01-30 13:49:10.000000 phamclust-1.3.0/src/phamclust/fasta.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     6803 2024-01-30 15:25:50.000000 phamclust-1.3.0/src/phamclust/genome.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     4534 2024-04-25 20:00:07.000000 phamclust-1.3.0/src/phamclust/heatmap.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)    23449 2024-04-21 20:44:13.000000 phamclust-1.3.0/src/phamclust/matrix.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     8292 2024-01-30 13:49:10.000000 phamclust-1.3.0/src/phamclust/metrics.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     2630 2024-01-30 13:49:10.000000 phamclust-1.3.0/src/phamclust/parallel_process.py
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-25 20:39:38.193623 phamclust-1.3.0/src/phamclust/scripts/
--rw-r--r--   0 cgauthier   (501) staff       (20)        0 2024-03-05 13:49:45.000000 phamclust-1.3.0/src/phamclust/scripts/__init__.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     3657 2024-03-06 21:02:43.000000 phamclust-1.3.0/src/phamclust/scripts/benchmark.py
--rw-r--r--   0 cgauthier   (501) staff       (20)    21143 2024-04-25 20:17:04.000000 phamclust-1.3.0/src/phamclust/scripts/phamclust.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     2831 2024-01-30 13:49:10.000000 phamclust-1.3.0/src/phamclust/statistics.py
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-25 20:39:38.193998 phamclust-1.3.0/src/phamclust.egg-info/
--rw-r--r--   0 cgauthier   (501) staff       (20)    10739 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/PKG-INFO
--rw-r--r--   0 cgauthier   (501) staff       (20)      678 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/SOURCES.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)        1 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/dependency_links.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)      109 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/entry_points.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)      136 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/requires.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)       10 2024-04-25 20:39:38.000000 phamclust-1.3.0/src/phamclust.egg-info/top_level.txt
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-26 13:35:40.576348 phamclust-1.3.1/
+-rw-r--r--   0 cgauthier   (501) staff       (20)    35148 2024-01-30 13:49:10.000000 phamclust-1.3.1/LICENSE
+-rw-r--r--   0 cgauthier   (501) staff       (20)    10739 2024-04-26 13:35:40.576188 phamclust-1.3.1/PKG-INFO
+-rw-r--r--   0 cgauthier   (501) staff       (20)     9457 2024-04-25 20:17:00.000000 phamclust-1.3.1/README.md
+-rw-r--r--   0 cgauthier   (501) staff       (20)       89 2024-01-30 13:49:10.000000 phamclust-1.3.1/pyproject.toml
+-rw-r--r--   0 cgauthier   (501) staff       (20)     1400 2024-04-26 13:35:40.576966 phamclust-1.3.1/setup.cfg
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-26 13:35:40.560994 phamclust-1.3.1/src/
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-26 13:35:40.571431 phamclust-1.3.1/src/phamclust/
+-rw-r--r--   0 cgauthier   (501) staff       (20)       69 2024-01-30 13:49:10.000000 phamclust-1.3.1/src/phamclust/__init__.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)      130 2024-03-05 13:51:35.000000 phamclust-1.3.1/src/phamclust/__main__.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     5478 2024-04-25 20:19:39.000000 phamclust-1.3.1/src/phamclust/blastn.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     6379 2024-04-26 13:30:21.000000 phamclust-1.3.1/src/phamclust/cli.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     1911 2024-02-21 18:41:57.000000 phamclust-1.3.1/src/phamclust/clustering.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     2409 2024-01-30 13:49:10.000000 phamclust-1.3.1/src/phamclust/fasta.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     6803 2024-01-30 15:25:50.000000 phamclust-1.3.1/src/phamclust/genome.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     4534 2024-04-25 20:00:07.000000 phamclust-1.3.1/src/phamclust/heatmap.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)    23449 2024-04-21 20:44:13.000000 phamclust-1.3.1/src/phamclust/matrix.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     8292 2024-01-30 13:49:10.000000 phamclust-1.3.1/src/phamclust/metrics.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     2630 2024-01-30 13:49:10.000000 phamclust-1.3.1/src/phamclust/parallel_process.py
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-26 13:35:40.575231 phamclust-1.3.1/src/phamclust/scripts/
+-rw-r--r--   0 cgauthier   (501) staff       (20)        0 2024-03-05 13:49:45.000000 phamclust-1.3.1/src/phamclust/scripts/__init__.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     3657 2024-03-06 21:02:43.000000 phamclust-1.3.1/src/phamclust/scripts/benchmark.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)    21143 2024-04-25 20:17:04.000000 phamclust-1.3.1/src/phamclust/scripts/phamclust.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     2831 2024-01-30 13:49:10.000000 phamclust-1.3.1/src/phamclust/statistics.py
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2024-04-26 13:35:40.575680 phamclust-1.3.1/src/phamclust.egg-info/
+-rw-r--r--   0 cgauthier   (501) staff       (20)    10739 2024-04-26 13:35:40.000000 phamclust-1.3.1/src/phamclust.egg-info/PKG-INFO
+-rw-r--r--   0 cgauthier   (501) staff       (20)      678 2024-04-26 13:35:40.000000 phamclust-1.3.1/src/phamclust.egg-info/SOURCES.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)        1 2024-04-26 13:35:40.000000 phamclust-1.3.1/src/phamclust.egg-info/dependency_links.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)      109 2024-04-26 13:35:40.000000 phamclust-1.3.1/src/phamclust.egg-info/entry_points.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)      136 2024-04-26 13:35:40.000000 phamclust-1.3.1/src/phamclust.egg-info/requires.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)       10 2024-04-26 13:35:40.000000 phamclust-1.3.1/src/phamclust.egg-info/top_level.txt
```

### Comparing `phamclust-1.3.0/LICENSE` & `phamclust-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/PKG-INFO` & `phamclust-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phamclust
-Version: 1.3.0
+Version: 1.3.1
 Summary: Cluster genomes based on gene phamily data
 Home-page: https://github.com/chg60/phamclust
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
 Project-URL: Source, https://github.com/chg60/phamclust
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `phamclust-1.3.0/README.md` & `phamclust-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/setup.cfg` & `phamclust-1.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 license_files = LICENSE
 name = phamclust
-version = 1.3.0
+version = 1.3.1
 author = Christian Gauthier
 author_email = chg60@pitt.edu
 description = Cluster genomes based on gene phamily data
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/chg60/phamclust
 project_urls =
```

### Comparing `phamclust-1.3.0/src/phamclust/blastn.py` & `phamclust-1.3.1/src/phamclust/blastn.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust/cli.py` & `phamclust-1.3.1/src/phamclust/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,17 +120,17 @@
 
     h = p.add_argument_group("heatmap arguments:")
     h.add_argument("-hc", "--heatmap-colors",
                    type=str, default=COLORS, metavar="",
                    help=f"comma-separated list of 2 or 3 colors to use in "
                         f"heatmaps [default: %(default)s]")
     h.add_argument("-hm", "--heatmap-midpoint",
-                   type=float, default=None, metavar="",
+                   type=float, default=0.5, metavar="",
                    help=f"midpoint to use for color gradient in heatmaps "
-                        f"[default: same as clustering threshold]")
+                        f"[default: %(default)s]")
 
     p.add_argument("-d", "--debug", action="store_true",
                    help=f"increase verbosity of logging for debug purposes")
     p.add_argument("-n", "--no-sub", action="store_true",
                    help="do not perform sub-clustering")
     p.add_argument("-r", "--remove-tmp", action="store_true",
                    help=f"remove temporary files (not recommended if repeated "
```

### Comparing `phamclust-1.3.0/src/phamclust/clustering.py` & `phamclust-1.3.1/src/phamclust/clustering.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust/fasta.py` & `phamclust-1.3.1/src/phamclust/fasta.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust/genome.py` & `phamclust-1.3.1/src/phamclust/genome.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust/heatmap.py` & `phamclust-1.3.1/src/phamclust/heatmap.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust/matrix.py` & `phamclust-1.3.1/src/phamclust/matrix.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust/metrics.py` & `phamclust-1.3.1/src/phamclust/metrics.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust/parallel_process.py` & `phamclust-1.3.1/src/phamclust/parallel_process.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust/scripts/benchmark.py` & `phamclust-1.3.1/src/phamclust/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust/scripts/phamclust.py` & `phamclust-1.3.1/src/phamclust/scripts/phamclust.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust/statistics.py` & `phamclust-1.3.1/src/phamclust/statistics.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.3.0/src/phamclust.egg-info/PKG-INFO` & `phamclust-1.3.1/src/phamclust.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phamclust
-Version: 1.3.0
+Version: 1.3.1
 Summary: Cluster genomes based on gene phamily data
 Home-page: https://github.com/chg60/phamclust
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
 Project-URL: Source, https://github.com/chg60/phamclust
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `phamclust-1.3.0/src/phamclust.egg-info/SOURCES.txt` & `phamclust-1.3.1/src/phamclust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

