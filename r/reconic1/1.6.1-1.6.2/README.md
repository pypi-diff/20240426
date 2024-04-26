# Comparing `tmp/reconic1-1.6.1.tar.gz` & `tmp/reconic1-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reconic1-1.6.1.tar", last modified: Fri Apr 26 18:27:38 2024, max compression
+gzip compressed data, was "reconic1-1.6.2.tar", last modified: Fri Apr 26 19:57:47 2024, max compression
```

## Comparing `reconic1-1.6.1.tar` & `reconic1-1.6.2.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.340722 reconic1-1.6.1/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1062 2024-04-26 15:39:39.000000 reconic1-1.6.1/LICENSE
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       95 2024-04-26 17:46:32.000000 reconic1-1.6.1/MANIFEST.in
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5838 2024-04-26 18:27:38.340722 reconic1-1.6.1/PKG-INFO
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5349 2024-04-26 15:39:39.000000 reconic1-1.6.1/README.md
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.337388 reconic1-1.6.1/reconic1.egg-info/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5838 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/PKG-INFO
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)      553 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/SOURCES.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)        1 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/dependency_links.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       42 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/entry_points.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       68 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/requires.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)        4 2024-04-26 18:27:37.000000 reconic1-1.6.1/reconic1.egg-info/top_level.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)       38 2024-04-26 18:27:38.340722 reconic1-1.6.1/setup.cfg
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1004 2024-04-26 18:27:36.000000 reconic1-1.6.1/setup.py
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.340722 reconic1-1.6.1/src/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/__init__.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     4447 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/directory_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3388 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/dns_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2439 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/http_headers.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2883 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/js_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3802 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/port_scanner.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2732 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/report_generator.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3441 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/ssl_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2676 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/subdomain_scan.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2349 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/textwrap.py
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2530 2024-04-26 15:39:39.000000 reconic1-1.6.1/src/whois_lookup.py
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.340722 reconic1-1.6.1/templates/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6552 2024-04-26 15:39:39.000000 reconic1-1.6.1/templates/report_template.html
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.340722 reconic1-1.6.1/utils/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)    16860 2024-04-26 15:39:39.000000 reconic1-1.6.1/utils/ports.json
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3172 2024-04-26 15:39:39.000000 reconic1-1.6.1/utils/utils.py
-drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 18:27:38.340722 reconic1-1.6.1/wordlists/
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6685 2024-04-26 15:39:39.000000 reconic1-1.6.1/wordlists/directories.txt
--rw-r--r--   0 fatsec    (1000) fatsec    (1000)    17271 2024-04-26 17:45:34.000000 reconic1-1.6.1/wordlists/subdomains.txt
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 19:57:47.031000 reconic1-1.6.2/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1062 2024-04-26 15:39:39.000000 reconic1-1.6.2/LICENSE
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)      121 2024-04-26 19:52:37.000000 reconic1-1.6.2/MANIFEST.in
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6152 2024-04-26 19:57:47.031000 reconic1-1.6.2/PKG-INFO
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     5349 2024-04-26 15:39:39.000000 reconic1-1.6.2/README.md
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 19:57:47.031000 reconic1-1.6.2/reconic1.egg-info/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6152 2024-04-26 19:57:46.000000 reconic1-1.6.2/reconic1.egg-info/PKG-INFO
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)      593 2024-04-26 19:57:47.000000 reconic1-1.6.2/reconic1.egg-info/SOURCES.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)        1 2024-04-26 19:57:46.000000 reconic1-1.6.2/reconic1.egg-info/dependency_links.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       41 2024-04-26 19:57:46.000000 reconic1-1.6.2/reconic1.egg-info/entry_points.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       68 2024-04-26 19:57:46.000000 reconic1-1.6.2/reconic1.egg-info/requires.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)        4 2024-04-26 19:57:46.000000 reconic1-1.6.2/reconic1.egg-info/top_level.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)       38 2024-04-26 19:57:47.031000 reconic1-1.6.2/setup.cfg
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     1316 2024-04-26 19:57:35.000000 reconic1-1.6.2/setup.py
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 19:57:47.031000 reconic1-1.6.2/src/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/__init__.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     4447 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/directory_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3388 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/dns_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2439 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/http_headers.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2883 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/js_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3802 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/port_scanner.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2732 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/report_generator.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3441 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/ssl_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2676 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/subdomain_scan.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2349 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/textwrap.py
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     2530 2024-04-26 15:39:39.000000 reconic1-1.6.2/src/whois_lookup.py
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 19:57:47.031000 reconic1-1.6.2/templates/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6552 2024-04-26 15:39:39.000000 reconic1-1.6.2/templates/report_template.html
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 19:57:47.031000 reconic1-1.6.2/utils/
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 19:57:47.031000 reconic1-1.6.2/utils/__pycache__/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     4410 2024-04-26 18:33:56.000000 reconic1-1.6.2/utils/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)    16860 2024-04-26 15:39:39.000000 reconic1-1.6.2/utils/ports.json
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     3172 2024-04-26 15:39:39.000000 reconic1-1.6.2/utils/utils.py
+drwxr-xr-x   0 fatsec    (1000) fatsec    (1000)        0 2024-04-26 19:57:47.031000 reconic1-1.6.2/wordlists/
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)     6685 2024-04-26 15:39:39.000000 reconic1-1.6.2/wordlists/directories.txt
+-rw-r--r--   0 fatsec    (1000) fatsec    (1000)    17271 2024-04-26 17:45:34.000000 reconic1-1.6.2/wordlists/subdomains.txt
```

### Comparing `reconic1-1.6.1/LICENSE` & `reconic1-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/PKG-INFO` & `reconic1-1.6.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: reconic1
-Version: 1.6.1
-Summary: All-in-One Reconnaissance Tool for Penetration Testing and Bounty Hunting
-Home-page: https://github.com/fkkarakurt/reconic
-Author: Fatih Küçükkarakurt
-Author-email: fatihkkarakurt128@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 <p align="center">
   <img src="https://github.com/fkkarakurt/reconic/blob/main/assets/reconicLogo.png?raw=true" alt="Logo">
 </p>
 
 # Reconic | All-in-One Reconnaissance Tool
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `reconic1-1.6.1/README.md` & `reconic1-1.6.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: reconic1
+Version: 1.6.2
+Summary: All-in-One Reconnaissance Tool for Penetration Testing and Bounty Hunting
+Home-page: https://github.com/fkkarakurt/reconic
+Author: Fatih Küçükkarakurt
+Author-email: fatihkkarakurt128@gmail.com
+Keywords: recon tool
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Security
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 <p align="center">
   <img src="https://github.com/fkkarakurt/reconic/blob/main/assets/reconicLogo.png?raw=true" alt="Logo">
 </p>
 
 # Reconic | All-in-One Reconnaissance Tool
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reconic1-1.6.1/reconic1.egg-info/PKG-INFO` & `reconic1-1.6.2/reconic1.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: reconic1
-Version: 1.6.1
+Version: 1.6.2
 Summary: All-in-One Reconnaissance Tool for Penetration Testing and Bounty Hunting
 Home-page: https://github.com/fkkarakurt/reconic
 Author: Fatih Küçükkarakurt
 Author-email: fatihkkarakurt128@gmail.com
+Keywords: recon tool
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Security
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <p align="center">
   <img src="https://github.com/fkkarakurt/reconic/blob/main/assets/reconicLogo.png?raw=true" alt="Logo">
```

### Comparing `reconic1-1.6.1/reconic1.egg-info/SOURCES.txt` & `reconic1-1.6.2/reconic1.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 src/ssl_scan.py
 src/subdomain_scan.py
 src/textwrap.py
 src/whois_lookup.py
 templates/report_template.html
 utils/ports.json
 utils/utils.py
+utils/__pycache__/utils.cpython-311.pyc
 wordlists/directories.txt
 wordlists/subdomains.txt
```

### Comparing `reconic1-1.6.1/setup.py` & `reconic1-1.6.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="reconic1",
-    version="1.6.1",
+    version="1.6.2",
     author="Fatih Küçükkarakurt",
     author_email="fatihkkarakurt128@gmail.com",
     description="All-in-One Reconnaissance Tool for Penetration Testing and Bounty Hunting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fkkarakurt/reconic",
     packages=find_packages(),
@@ -19,18 +19,25 @@
         "requests",
         "rich",
         "python-whois",
         "beautifulsoup4",
         "Jinja2"
     ],
     entry_points={
-        'console_scripts': [
-            'reconic1 = reconic:main'
+        "console_scripts": [
+            "reconic = reconic:main"
         ]
     },
     classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Console",
+        "Intended Audience :: Information Technology",
+        "Intended Audience :: System Administrators",
+        "Intended Audience :: Telecommunications Industry",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
+        "Operating System :: POSIX :: Linux",
+        "Topic :: Security"
     ],
+    keywords="recon tool",
     python_requires=">=3.8",
 )
```

### Comparing `reconic1-1.6.1/src/directory_scan.py` & `reconic1-1.6.2/src/directory_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/src/dns_scan.py` & `reconic1-1.6.2/src/dns_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/src/http_headers.py` & `reconic1-1.6.2/src/http_headers.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/src/js_scan.py` & `reconic1-1.6.2/src/js_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/src/port_scanner.py` & `reconic1-1.6.2/src/port_scanner.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/src/report_generator.py` & `reconic1-1.6.2/src/report_generator.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/src/ssl_scan.py` & `reconic1-1.6.2/src/ssl_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/src/subdomain_scan.py` & `reconic1-1.6.2/src/subdomain_scan.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/src/textwrap.py` & `reconic1-1.6.2/src/textwrap.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/src/whois_lookup.py` & `reconic1-1.6.2/src/whois_lookup.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/templates/report_template.html` & `reconic1-1.6.2/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/utils/ports.json` & `reconic1-1.6.2/utils/ports.json`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/utils/utils.py` & `reconic1-1.6.2/utils/utils.py`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/wordlists/directories.txt` & `reconic1-1.6.2/wordlists/directories.txt`

 * *Files identical despite different names*

### Comparing `reconic1-1.6.1/wordlists/subdomains.txt` & `reconic1-1.6.2/wordlists/subdomains.txt`

 * *Files identical despite different names*

