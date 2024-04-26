# Comparing `tmp/zg_crawl_tools-0.0.1.tar.gz` & `tmp/zg_crawl_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zg_crawl_tools-0.0.1.tar", last modified: Fri Apr 12 02:47:20 2024, max compression
+gzip compressed data, was "zg_crawl_tools-0.0.2.tar", last modified: Fri Apr 26 07:12:01 2024, max compression
```

## Comparing `zg_crawl_tools-0.0.1.tar` & `zg_crawl_tools-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-12 02:47:20.953797 zg_crawl_tools-0.0.1/
--rw-r--r--   0 zhiboyuan   (501) staff       (20)     1073 2024-04-12 02:45:56.000000 zg_crawl_tools-0.0.1/LICENSE
--rw-r--r--   0 zhiboyuan   (501) staff       (20)      589 2024-04-12 02:47:20.953538 zg_crawl_tools-0.0.1/PKG-INFO
--rw-r--r--   0 zhiboyuan   (501) staff       (20)      170 2024-04-12 02:45:48.000000 zg_crawl_tools-0.0.1/README.md
--rw-r--r--   0 zhiboyuan   (501) staff       (20)      408 2024-04-12 02:47:17.000000 zg_crawl_tools-0.0.1/pyproject.toml
--rw-r--r--   0 zhiboyuan   (501) staff       (20)       38 2024-04-12 02:47:20.953850 zg_crawl_tools-0.0.1/setup.cfg
-drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-12 02:47:20.950557 zg_crawl_tools-0.0.1/src/
-drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-12 02:47:20.952234 zg_crawl_tools-0.0.1/src/zg_crawl_tools/
--rw-r--r--   0 zhiboyuan   (501) staff       (20)      111 2024-04-12 02:41:26.000000 zg_crawl_tools-0.0.1/src/zg_crawl_tools/__init__.py
--rw-r--r--   0 zhiboyuan   (501) staff       (20)     1787 2024-04-12 02:24:43.000000 zg_crawl_tools-0.0.1/src/zg_crawl_tools/zg_extract_response.py
--rw-r--r--   0 zhiboyuan   (501) staff       (20)      956 2024-04-12 02:45:15.000000 zg_crawl_tools-0.0.1/src/zg_crawl_tools/zg_request.py
-drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-12 02:47:20.953257 zg_crawl_tools-0.0.1/src/zg_crawl_tools.egg-info/
--rw-r--r--   0 zhiboyuan   (501) staff       (20)      589 2024-04-12 02:47:20.000000 zg_crawl_tools-0.0.1/src/zg_crawl_tools.egg-info/PKG-INFO
--rw-r--r--   0 zhiboyuan   (501) staff       (20)      347 2024-04-12 02:47:20.000000 zg_crawl_tools-0.0.1/src/zg_crawl_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zhiboyuan   (501) staff       (20)        1 2024-04-12 02:47:20.000000 zg_crawl_tools-0.0.1/src/zg_crawl_tools.egg-info/dependency_links.txt
--rw-r--r--   0 zhiboyuan   (501) staff       (20)       14 2024-04-12 02:47:20.000000 zg_crawl_tools-0.0.1/src/zg_crawl_tools.egg-info/requires.txt
--rw-r--r--   0 zhiboyuan   (501) staff       (20)       15 2024-04-12 02:47:20.000000 zg_crawl_tools-0.0.1/src/zg_crawl_tools.egg-info/top_level.txt
+drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-26 07:12:01.035100 zg_crawl_tools-0.0.2/
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)     1073 2024-04-12 02:45:56.000000 zg_crawl_tools-0.0.2/LICENSE
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      643 2024-04-26 07:12:01.034865 zg_crawl_tools-0.0.2/PKG-INFO
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      170 2024-04-12 02:45:48.000000 zg_crawl_tools-0.0.2/README.md
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      446 2024-04-26 06:57:50.000000 zg_crawl_tools-0.0.2/pyproject.toml
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)       38 2024-04-26 07:12:01.035166 zg_crawl_tools-0.0.2/setup.cfg
+drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-26 07:12:01.030199 zg_crawl_tools-0.0.2/src/
+drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-26 07:12:01.031350 zg_crawl_tools-0.0.2/src/zg_crawl_tools/
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      338 2024-04-26 06:54:03.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools/__init__.py
+drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-26 07:12:01.032654 zg_crawl_tools-0.0.2/src/zg_crawl_tools/bloomfilter_module/
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      114 2024-04-26 06:47:33.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools/bloomfilter_module/__init__.py
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      537 2024-04-26 06:50:52.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools/bloomfilter_module/bloom_check.py
+drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-26 07:12:01.033286 zg_crawl_tools-0.0.2/src/zg_crawl_tools/cipher_moudle/
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      114 2024-04-24 08:33:54.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools/cipher_moudle/__init__.py
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)     1991 2024-04-26 06:54:03.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools/cipher_moudle/cipher_calculate.py
+drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-26 07:12:01.034275 zg_crawl_tools-0.0.2/src/zg_crawl_tools/requests_moudle/
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      114 2024-04-26 06:52:46.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools/requests_moudle/__init__.py
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)     1787 2024-04-12 02:24:43.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools/requests_moudle/zg_extract_response.py
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      956 2024-04-12 02:45:15.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools/requests_moudle/zg_request.py
+drwxr-xr-x   0 zhiboyuan   (501) staff       (20)        0 2024-04-26 07:12:01.034590 zg_crawl_tools-0.0.2/src/zg_crawl_tools.egg-info/
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      643 2024-04-26 07:12:01.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)      627 2024-04-26 07:12:01.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)        1 2024-04-26 07:12:01.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)       38 2024-04-26 07:12:01.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools.egg-info/requires.txt
+-rw-r--r--   0 zhiboyuan   (501) staff       (20)       15 2024-04-26 07:12:01.000000 zg_crawl_tools-0.0.2/src/zg_crawl_tools.egg-info/top_level.txt
```

### Comparing `zg_crawl_tools-0.0.1/LICENSE` & `zg_crawl_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zg_crawl_tools-0.0.1/PKG-INFO` & `zg_crawl_tools-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: zg_crawl_tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: by_yuanyuan <zhiboyuan666@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: lxml
+Requires-Dist: redisbloom
+Requires-Dist: pycryptodome
 
 # Example Package
 
 This is a simple example package. You can use
 [GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
```

### Comparing `zg_crawl_tools-0.0.1/src/zg_crawl_tools/zg_extract_response.py` & `zg_crawl_tools-0.0.2/src/zg_crawl_tools/requests_moudle/zg_extract_response.py`

 * *Files identical despite different names*

### Comparing `zg_crawl_tools-0.0.1/src/zg_crawl_tools/zg_request.py` & `zg_crawl_tools-0.0.2/src/zg_crawl_tools/requests_moudle/zg_request.py`

 * *Files identical despite different names*

### Comparing `zg_crawl_tools-0.0.1/src/zg_crawl_tools.egg-info/PKG-INFO` & `zg_crawl_tools-0.0.2/src/zg_crawl_tools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: zg_crawl_tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: by_yuanyuan <zhiboyuan666@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: lxml
+Requires-Dist: redisbloom
+Requires-Dist: pycryptodome
 
 # Example Package
 
 This is a simple example package. You can use
 [GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
```

