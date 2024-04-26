# Comparing `tmp/reconic1-1.6.tar.gz` & `tmp/reconic1-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reconic1-1.6.tar", last modified: Fri Apr 26 18:21:04 2024, max compression
+gzip compressed data, was "reconic1-1.6.1.tar", last modified: Fri Apr 26 18:27:38 2024, max compression
```

## Comparing `reconic1-1.6.tar` & `reconic1-1.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.322428 reconic1-1.6/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1062 2024-04-26 15:39:39.000000 reconic1-1.6/LICENSE
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       95 2024-04-26 17:46:32.000000 reconic1-1.6/MANIFEST.in
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5836 2024-04-26 18:21:04.322428 reconic1-1.6/PKG-INFO
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5349 2024-04-26 15:39:39.000000 reconic1-1.6/README.md
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.319094 reconic1-1.6/reconic1.egg-info/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5836 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/PKG-INFO
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)      553 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/SOURCES.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)        1 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/dependency_links.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       50 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/entry_points.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       68 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/requires.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)        4 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/top_level.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       38 2024-04-26 18:21:04.322428 reconic1-1.6/setup.cfg
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1010 2024-04-26 18:20:41.000000 reconic1-1.6/setup.py
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.322428 reconic1-1.6/src/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 15:39:39.000000 reconic1-1.6/src/__init__.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     4447 2024-04-26 15:39:39.000000 reconic1-1.6/src/directory_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3388 2024-04-26 15:39:39.000000 reconic1-1.6/src/dns_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2439 2024-04-26 15:39:39.000000 reconic1-1.6/src/http_headers.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2883 2024-04-26 15:39:39.000000 reconic1-1.6/src/js_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3802 2024-04-26 15:39:39.000000 reconic1-1.6/src/port_scanner.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2732 2024-04-26 15:39:39.000000 reconic1-1.6/src/report_generator.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3441 2024-04-26 15:39:39.000000 reconic1-1.6/src/ssl_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2676 2024-04-26 15:39:39.000000 reconic1-1.6/src/subdomain_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2349 2024-04-26 15:39:39.000000 reconic1-1.6/src/textwrap.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2530 2024-04-26 15:39:39.000000 reconic1-1.6/src/whois_lookup.py
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.322428 reconic1-1.6/templates/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6552 2024-04-26 15:39:39.000000 reconic1-1.6/templates/report_template.html
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.322428 reconic1-1.6/utils/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)    16860 2024-04-26 15:39:39.000000 reconic1-1.6/utils/ports.json
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3172 2024-04-26 15:39:39.000000 reconic1-1.6/utils/utils.py
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.322428 reconic1-1.6/wordlists/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6685 2024-04-26 15:39:39.000000 reconic1-1.6/wordlists/directories.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)    17271 2024-04-26 17:45:34.000000 reconic1-1.6/wordlists/subdomains.txt
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.340722 reconic1-1.6.1/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1062 2024-04-26 15:39:39.000000 reconic1-1.6.1/LICENSE
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       95 2024-04-26 17:46:32.000000 reconic1-1.6.1/MANIFEST.in
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5838 2024-04-26 18:27:38.340722 reconic1-1.6.1/PKG-INFO
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5349 2024-04-26 15:39:39.000000 reconic1-1.6.1/README.md
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.337388 reconic1-1.6.1/reconic1.egg-info/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5838 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/PKG-INFO
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)      553 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/SOURCES.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)        1 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/dependency_links.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       42 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/entry_points.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       68 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/requires.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)        4 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/top_level.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       38 2024-04-26 18:27:38.340722 reconic1-1.6.1/setup.cfg
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1004 2024-04-26 18:27:36.000000 reconic1-1.6.1/setup.py
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.340722 reconic1-1.6.1/src/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/__init__.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     4447 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/directory_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3388 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/dns_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2439 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/http_headers.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2883 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/js_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3802 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/port_scanner.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2732 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/report_generator.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3441 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/ssl_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2676 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/subdomain_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2349 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/textwrap.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2530 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/whois_lookup.py
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.340722 reconic1-1.6.1/templates/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6552 2024-04-26 15:39:39.000000 reconic1-1.6.1/templates/report_template.html
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.340722 reconic1-1.6.1/utils/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)    16860 2024-04-26 15:39:39.000000 reconic1-1.6.1/utils/ports.json
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3172 2024-04-26 15:39:39.000000 reconic1-1.6.1/utils/utils.py
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.340722 reconic1-1.6.1/wordlists/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6685 2024-04-26 15:39:39.000000 reconic1-1.6.1/wordlists/directories.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)    17271 2024-04-26 17:45:34.000000 reconic1-1.6.1/wordlists/subdomains.txt
```

### Comparing `reconic1-1.6/LICENSE` & `reconic1-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/PKG-INFO` & `reconic1-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reconic1
-Version: 1.6
+Version: 1.6.1
 Summary: All-in-One Reconnaissance Tool for Penetration Testing and Bounty Hunting
 Home-page: https://github.com/fkkarakurt/reconic
 Author: Fatih Küçükkarakurt
 Author-email: fatihkkarakurt128@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `reconic1-1.6/README.md` & `reconic1-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/reconic1.egg-info/PKG-INFO` & `reconic1-1.6.1/reconic1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reconic1
-Version: 1.6
+Version: 1.6.1
 Summary: All-in-One Reconnaissance Tool for Penetration Testing and Bounty Hunting
 Home-page: https://github.com/fkkarakurt/reconic
 Author: Fatih Küçükkarakurt
 Author-email: fatihkkarakurt128@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `reconic1-1.6/reconic1.egg-info/SOURCES.txt` & `reconic1-1.6.1/reconic1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/setup.py` & `reconic1-1.6.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="reconic1",
-    version="1.6",
+    version="1.6.1",
     author="Fatih Küçükkarakurt",
     author_email="fatihkkarakurt128@gmail.com",
     description="All-in-One Reconnaissance Tool for Penetration Testing and Bounty Hunting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fkkarakurt/reconic",
     packages=find_packages(),
@@ -20,15 +20,15 @@
         "rich",
         "python-whois",
         "beautifulsoup4",
         "Jinja2"
     ],
     entry_points={
         'console_scripts': [
-            'reconic1 = reconic.reconic:main'
+            'reconic1 = reconic:main'
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `reconic1-1.6/src/directory_scan.py` & `reconic1-1.6.1/src/directory_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/src/dns_scan.py` & `reconic1-1.6.1/src/dns_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/src/http_headers.py` & `reconic1-1.6.1/src/http_headers.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/src/js_scan.py` & `reconic1-1.6.1/src/js_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/src/port_scanner.py` & `reconic1-1.6.1/src/port_scanner.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/src/report_generator.py` & `reconic1-1.6.1/src/report_generator.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/src/ssl_scan.py` & `reconic1-1.6.1/src/ssl_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/src/subdomain_scan.py` & `reconic1-1.6.1/src/subdomain_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/src/textwrap.py` & `reconic1-1.6.1/src/textwrap.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/src/whois_lookup.py` & `reconic1-1.6.1/src/whois_lookup.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/templates/report_template.html` & `reconic1-1.6.1/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/utils/ports.json` & `reconic1-1.6.1/utils/ports.json`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/utils/utils.py` & `reconic1-1.6.1/utils/utils.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/wordlists/directories.txt` & `reconic1-1.6.1/wordlists/directories.txt`

 * *Files identical despite different names*

### Comparing `reconic1-1.6/wordlists/subdomains.txt` & `reconic1-1.6.1/wordlists/subdomains.txt`

 * *Files identical despite different names*

