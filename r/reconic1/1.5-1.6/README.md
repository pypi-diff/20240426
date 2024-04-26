# Comparing `tmp/reconic1-1.5.tar.gz` & `tmp/reconic1-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reconic1-1.5.tar", last modified: Fri Apr 26 17:59:36 2024, max compression
+gzip compressed data, was "reconic1-1.6.tar", last modified: Fri Apr 26 18:21:04 2024, max compression
```

## Comparing `reconic1-1.5.tar` & `reconic1-1.6.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 17:59:36.906707 reconic1-1.5/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1062 2024-04-26 15:39:39.000000 reconic1-1.5/LICENSE
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       95 2024-04-26 17:46:32.000000 reconic1-1.5/MANIFEST.in
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5836 2024-04-26 17:59:36.906707 reconic1-1.5/PKG-INFO
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5349 2024-04-26 15:39:39.000000 reconic1-1.5/README.md
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 17:59:36.903374 reconic1-1.5/reconic1.egg-info/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5836 2024-04-26 17:59:36.000000 reconic1-1.5/reconic1.egg-info/PKG-INFO
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)      518 2024-04-26 17:59:36.000000 reconic1-1.5/reconic1.egg-info/SOURCES.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)        1 2024-04-26 17:59:36.000000 reconic1-1.5/reconic1.egg-info/dependency_links.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       68 2024-04-26 17:59:36.000000 reconic1-1.5/reconic1.egg-info/requires.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)        4 2024-04-26 17:59:36.000000 reconic1-1.5/reconic1.egg-info/top_level.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       38 2024-04-26 17:59:36.906707 reconic1-1.5/setup.cfg
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)      930 2024-04-26 17:59:27.000000 reconic1-1.5/setup.py
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 17:59:36.903374 reconic1-1.5/src/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 15:39:39.000000 reconic1-1.5/src/__init__.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     4447 2024-04-26 15:39:39.000000 reconic1-1.5/src/directory_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3388 2024-04-26 15:39:39.000000 reconic1-1.5/src/dns_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2439 2024-04-26 15:39:39.000000 reconic1-1.5/src/http_headers.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2883 2024-04-26 15:39:39.000000 reconic1-1.5/src/js_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3802 2024-04-26 15:39:39.000000 reconic1-1.5/src/port_scanner.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2732 2024-04-26 15:39:39.000000 reconic1-1.5/src/report_generator.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3441 2024-04-26 15:39:39.000000 reconic1-1.5/src/ssl_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2676 2024-04-26 15:39:39.000000 reconic1-1.5/src/subdomain_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2349 2024-04-26 15:39:39.000000 reconic1-1.5/src/textwrap.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2530 2024-04-26 15:39:39.000000 reconic1-1.5/src/whois_lookup.py
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 17:59:36.903374 reconic1-1.5/templates/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6552 2024-04-26 15:39:39.000000 reconic1-1.5/templates/report_template.html
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 17:59:36.903374 reconic1-1.5/utils/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)    16860 2024-04-26 15:39:39.000000 reconic1-1.5/utils/ports.json
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3172 2024-04-26 15:39:39.000000 reconic1-1.5/utils/utils.py
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 17:59:36.903374 reconic1-1.5/wordlists/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6685 2024-04-26 15:39:39.000000 reconic1-1.5/wordlists/directories.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)    17271 2024-04-26 17:45:34.000000 reconic1-1.5/wordlists/subdomains.txt
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.322428 reconic1-1.6/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1062 2024-04-26 15:39:39.000000 reconic1-1.6/LICENSE
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       95 2024-04-26 17:46:32.000000 reconic1-1.6/MANIFEST.in
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5836 2024-04-26 18:21:04.322428 reconic1-1.6/PKG-INFO
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5349 2024-04-26 15:39:39.000000 reconic1-1.6/README.md
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.319094 reconic1-1.6/reconic1.egg-info/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5836 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/PKG-INFO
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)      553 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/SOURCES.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)        1 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/dependency_links.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       50 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/entry_points.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       68 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/requires.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)        4 2024-04-26 18:21:03.000000 reconic1-1.6/reconic1.egg-info/top_level.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       38 2024-04-26 18:21:04.322428 reconic1-1.6/setup.cfg
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1010 2024-04-26 18:20:41.000000 reconic1-1.6/setup.py
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.322428 reconic1-1.6/src/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 15:39:39.000000 reconic1-1.6/src/__init__.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     4447 2024-04-26 15:39:39.000000 reconic1-1.6/src/directory_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3388 2024-04-26 15:39:39.000000 reconic1-1.6/src/dns_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2439 2024-04-26 15:39:39.000000 reconic1-1.6/src/http_headers.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2883 2024-04-26 15:39:39.000000 reconic1-1.6/src/js_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3802 2024-04-26 15:39:39.000000 reconic1-1.6/src/port_scanner.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2732 2024-04-26 15:39:39.000000 reconic1-1.6/src/report_generator.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3441 2024-04-26 15:39:39.000000 reconic1-1.6/src/ssl_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2676 2024-04-26 15:39:39.000000 reconic1-1.6/src/subdomain_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2349 2024-04-26 15:39:39.000000 reconic1-1.6/src/textwrap.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2530 2024-04-26 15:39:39.000000 reconic1-1.6/src/whois_lookup.py
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.322428 reconic1-1.6/templates/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6552 2024-04-26 15:39:39.000000 reconic1-1.6/templates/report_template.html
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.322428 reconic1-1.6/utils/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)    16860 2024-04-26 15:39:39.000000 reconic1-1.6/utils/ports.json
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3172 2024-04-26 15:39:39.000000 reconic1-1.6/utils/utils.py
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:21:04.322428 reconic1-1.6/wordlists/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6685 2024-04-26 15:39:39.000000 reconic1-1.6/wordlists/directories.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)    17271 2024-04-26 17:45:34.000000 reconic1-1.6/wordlists/subdomains.txt
```

### Comparing `reconic1-1.5/LICENSE` & `reconic1-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/PKG-INFO` & `reconic1-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reconic1
-Version: 1.5
+Version: 1.6
 Summary: All-in-One Reconnaissance Tool for Penetration Testing and Bounty Hunting
 Home-page: https://github.com/fkkarakurt/reconic
 Author: Fatih Küçükkarakurt
 Author-email: fatihkkarakurt128@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `reconic1-1.5/README.md` & `reconic1-1.6/README.md`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/reconic1.egg-info/PKG-INFO` & `reconic1-1.6/reconic1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reconic1
-Version: 1.5
+Version: 1.6
 Summary: All-in-One Reconnaissance Tool for Penetration Testing and Bounty Hunting
 Home-page: https://github.com/fkkarakurt/reconic
 Author: Fatih Küçükkarakurt
 Author-email: fatihkkarakurt128@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `reconic1-1.5/reconic1.egg-info/SOURCES.txt` & `reconic1-1.6/reconic1.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 reconic1.egg-info/PKG-INFO
 reconic1.egg-info/SOURCES.txt
 reconic1.egg-info/dependency_links.txt
+reconic1.egg-info/entry_points.txt
 reconic1.egg-info/requires.txt
 reconic1.egg-info/top_level.txt
 src/__init__.py
 src/directory_scan.py
 src/dns_scan.py
 src/http_headers.py
 src/js_scan.py
```

### Comparing `reconic1-1.5/setup.py` & `reconic1-1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="reconic1",
-    version="1.5",
+    version="1.6",
     author="Fatih Küçükkarakurt",
     author_email="fatihkkarakurt128@gmail.com",
     description="All-in-One Reconnaissance Tool for Penetration Testing and Bounty Hunting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fkkarakurt/reconic",
     packages=find_packages(),
-    include_package_data=True,
     install_requires=[
         "dnspython",
         "pyfiglet",
         "requests",
         "rich",
         "python-whois",
         "beautifulsoup4",
         "Jinja2"
     ],
+    entry_points={
+        'console_scripts': [
+            'reconic1 = reconic.reconic:main'
+        ]
+    },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
 )
```

### Comparing `reconic1-1.5/src/directory_scan.py` & `reconic1-1.6/src/directory_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/src/dns_scan.py` & `reconic1-1.6/src/dns_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/src/http_headers.py` & `reconic1-1.6/src/http_headers.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/src/js_scan.py` & `reconic1-1.6/src/js_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/src/port_scanner.py` & `reconic1-1.6/src/port_scanner.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/src/report_generator.py` & `reconic1-1.6/src/report_generator.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/src/ssl_scan.py` & `reconic1-1.6/src/ssl_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/src/subdomain_scan.py` & `reconic1-1.6/src/subdomain_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/src/textwrap.py` & `reconic1-1.6/src/textwrap.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/src/whois_lookup.py` & `reconic1-1.6/src/whois_lookup.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/templates/report_template.html` & `reconic1-1.6/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/utils/ports.json` & `reconic1-1.6/utils/ports.json`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/utils/utils.py` & `reconic1-1.6/utils/utils.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/wordlists/directories.txt` & `reconic1-1.6/wordlists/directories.txt`

 * *Files identical despite different names*

### Comparing `reconic1-1.5/wordlists/subdomains.txt` & `reconic1-1.6/wordlists/subdomains.txt`

 * *Files identical despite different names*

