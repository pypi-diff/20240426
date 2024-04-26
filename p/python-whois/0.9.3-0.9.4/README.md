# Comparing `tmp/python-whois-0.9.3.tar.gz` & `tmp/python_whois-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-whois-0.9.3.tar", last modified: Sat Mar 23 23:58:30 2024, max compression
+gzip compressed data, was "python_whois-0.9.4.tar", last modified: Fri Apr 26 09:22:05 2024, max compression
```

## Comparing `python-whois-0.9.3.tar` & `python_whois-0.9.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-03-23 23:58:30.558903 python-whois-0.9.3/
--rw-r--r--   0 baron      (501) staff       (20)     1023 2024-03-21 12:43:32.000000 python-whois-0.9.3/LICENSE.txt
--rw-r--r--   0 baron      (501) staff       (20)       73 2024-03-21 12:43:32.000000 python-whois-0.9.3/MANIFEST.in
--rw-r--r--   0 baron      (501) staff       (20)     3155 2024-03-23 23:58:30.558780 python-whois-0.9.3/PKG-INFO
--rw-r--r--   0 baron      (501) staff       (20)     2534 2024-03-22 12:54:30.000000 python-whois-0.9.3/README.rst
-drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-03-23 23:58:30.554585 python-whois-0.9.3/python_whois.egg-info/
--rw-r--r--   0 baron      (501) staff       (20)     3155 2024-03-23 23:58:30.000000 python-whois-0.9.3/python_whois.egg-info/PKG-INFO
--rw-r--r--   0 baron      (501) staff       (20)      440 2024-03-23 23:58:30.000000 python-whois-0.9.3/python_whois.egg-info/SOURCES.txt
--rw-r--r--   0 baron      (501) staff       (20)        1 2024-03-23 23:58:30.000000 python-whois-0.9.3/python_whois.egg-info/dependency_links.txt
--rw-r--r--   0 baron      (501) staff       (20)        1 2024-03-23 23:58:30.000000 python-whois-0.9.3/python_whois.egg-info/not-zip-safe
--rw-r--r--   0 baron      (501) staff       (20)       16 2024-03-23 23:58:30.000000 python-whois-0.9.3/python_whois.egg-info/requires.txt
--rw-r--r--   0 baron      (501) staff       (20)        6 2024-03-23 23:58:30.000000 python-whois-0.9.3/python_whois.egg-info/top_level.txt
--rw-r--r--   0 baron      (501) staff       (20)       38 2024-03-23 23:58:30.558942 python-whois-0.9.3/setup.cfg
--rw-r--r--   0 baron      (501) staff       (20)     1052 2024-03-23 23:58:18.000000 python-whois-0.9.3/setup.py
-drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-03-23 23:58:30.556057 python-whois-0.9.3/test/
--rw-r--r--   0 baron      (501) staff       (20)     1678 2024-03-22 12:45:22.000000 python-whois-0.9.3/test/test_main.py
--rw-r--r--   0 baron      (501) staff       (20)      363 2024-03-22 12:45:14.000000 python-whois-0.9.3/test/test_nicclient.py
--rw-r--r--   0 baron      (501) staff       (20)    30936 2024-03-22 13:20:13.000000 python-whois-0.9.3/test/test_parser.py
--rw-r--r--   0 baron      (501) staff       (20)     1431 2024-03-22 12:45:01.000000 python-whois-0.9.3/test/test_query.py
-drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-03-23 23:58:30.557335 python-whois-0.9.3/whois/
--rw-r--r--   0 baron      (501) staff       (20)     5325 2024-03-22 12:44:47.000000 python-whois-0.9.3/whois/__init__.py
-drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-03-23 23:58:30.557726 python-whois-0.9.3/whois/data/
--rw-r--r--   0 baron      (501) staff       (20)   232589 2024-03-21 12:43:32.000000 python-whois-0.9.3/whois/data/public_suffix_list.dat
--rw-r--r--   0 baron      (501) staff       (20)   138402 2024-03-22 13:04:11.000000 python-whois-0.9.3/whois/parser.py
--rw-r--r--   0 baron      (501) staff       (20)     1275 2024-03-22 12:45:44.000000 python-whois-0.9.3/whois/time_zones.py
--rw-r--r--   0 baron      (501) staff       (20)    19751 2024-03-22 12:35:57.000000 python-whois-0.9.3/whois/whois.py
+drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-04-26 09:22:05.610557 python_whois-0.9.4/
+-rw-r--r--   0 baron      (501) staff       (20)     1023 2024-03-21 12:43:32.000000 python_whois-0.9.4/LICENSE.txt
+-rw-r--r--   0 baron      (501) staff       (20)       72 2024-04-26 09:14:39.000000 python_whois-0.9.4/MANIFEST.in
+-rw-r--r--   0 baron      (501) staff       (20)     2615 2024-04-26 09:22:05.610320 python_whois-0.9.4/PKG-INFO
+-rw-r--r--   0 baron      (501) staff       (20)     1923 2024-04-26 09:13:54.000000 python_whois-0.9.4/README.md
+drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-04-26 09:22:05.610065 python_whois-0.9.4/python_whois.egg-info/
+-rw-r--r--   0 baron      (501) staff       (20)     2615 2024-04-26 09:22:05.000000 python_whois-0.9.4/python_whois.egg-info/PKG-INFO
+-rw-r--r--   0 baron      (501) staff       (20)      439 2024-04-26 09:22:05.000000 python_whois-0.9.4/python_whois.egg-info/SOURCES.txt
+-rw-r--r--   0 baron      (501) staff       (20)        1 2024-04-26 09:22:05.000000 python_whois-0.9.4/python_whois.egg-info/dependency_links.txt
+-rw-r--r--   0 baron      (501) staff       (20)        1 2024-04-26 09:22:05.000000 python_whois-0.9.4/python_whois.egg-info/not-zip-safe
+-rw-r--r--   0 baron      (501) staff       (20)       16 2024-04-26 09:22:05.000000 python_whois-0.9.4/python_whois.egg-info/requires.txt
+-rw-r--r--   0 baron      (501) staff       (20)        6 2024-04-26 09:22:05.000000 python_whois-0.9.4/python_whois.egg-info/top_level.txt
+-rw-r--r--   0 baron      (501) staff       (20)       38 2024-04-26 09:22:05.610605 python_whois-0.9.4/setup.cfg
+-rw-r--r--   0 baron      (501) staff       (20)     1102 2024-04-26 09:21:33.000000 python_whois-0.9.4/setup.py
+drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-04-26 09:22:05.606765 python_whois-0.9.4/test/
+-rw-r--r--   0 baron      (501) staff       (20)     1678 2024-03-22 12:45:22.000000 python_whois-0.9.4/test/test_main.py
+-rw-r--r--   0 baron      (501) staff       (20)      363 2024-03-22 12:45:14.000000 python_whois-0.9.4/test/test_nicclient.py
+-rw-r--r--   0 baron      (501) staff       (20)    30936 2024-03-22 13:20:13.000000 python_whois-0.9.4/test/test_parser.py
+-rw-r--r--   0 baron      (501) staff       (20)     1431 2024-03-22 12:45:01.000000 python_whois-0.9.4/test/test_query.py
+drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-04-26 09:22:05.608506 python_whois-0.9.4/whois/
+-rw-r--r--   0 baron      (501) staff       (20)     5325 2024-03-22 12:44:47.000000 python_whois-0.9.4/whois/__init__.py
+drwxr-xr-x   0 baron      (501) staff       (20)        0 2024-04-26 09:22:05.609017 python_whois-0.9.4/whois/data/
+-rw-r--r--   0 baron      (501) staff       (20)   232589 2024-03-21 12:43:32.000000 python_whois-0.9.4/whois/data/public_suffix_list.dat
+-rw-r--r--   0 baron      (501) staff       (20)   138629 2024-04-26 09:13:54.000000 python_whois-0.9.4/whois/parser.py
+-rw-r--r--   0 baron      (501) staff       (20)     1275 2024-03-22 12:45:44.000000 python_whois-0.9.4/whois/time_zones.py
+-rw-r--r--   0 baron      (501) staff       (20)    19751 2024-03-22 12:35:57.000000 python_whois-0.9.4/whois/whois.py
```

### Comparing `python-whois-0.9.3/LICENSE.txt` & `python_whois-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-whois-0.9.3/PKG-INFO` & `python_whois-0.9.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,105 @@
 Metadata-Version: 2.1
 Name: python-whois
-Version: 0.9.3
+Version: 0.9.4
 Summary: Whois querying and parsing of domain registration information.
 Home-page: https://github.com/richardpenman/whois
 Author: Richard Penman
 Author-email: richard.penman@gmail.com
 License: MIT
 Keywords: whois,python
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: python-dateutil
 
 Goal
 ====
 
 -  Create a simple importable Python module which will produce parsed
    WHOIS data for a given domain.
 -  Able to extract data for all the popular TLDs (com, org, net, ...)
 -  Query a WHOIS server directly instead of going through an
    intermediate web service like many others do.
 
 
 Example
 =======
 
-.. sourcecode:: bash
-
-    >>> import whois
-    >>> w = whois.whois('example.com')
-    >>> w.expiration_date  # dates converted to datetime object
-    datetime.datetime(2022, 8, 13, 4, 0)
-    >>> w.text  # the content downloaded from whois server
-    u'\nDomain Name: EXAMPLE.COM
-    Registry Domain ID: 2336799_DOMAIN_COM-VRSN
-    ...'
-
-    >>> print(w)  # print values of all found attributes    
-    {
-        "creation_date": "1995-08-14 04:00:00",
-        "expiration_date": "2022-08-13 04:00:00",
-        "updated_date": "2021-08-14 07:01:44",
-        "domain_name": "EXAMPLE.COM",
-        "name_servers": [
-            "A.IANA-SERVERS.NET",
-            "B.IANA-SERVERS.NET"
-        ],
-    ...
-
+```python
+>>> import whois
+>>> w = whois.whois('example.com')
+>>> w.expiration_date  # dates converted to datetime object
+datetime.datetime(2022, 8, 13, 4, 0)
+>>> w.text  # the content downloaded from whois server
+u'\nDomain Name: EXAMPLE.COM
+Registry Domain ID: 2336799_DOMAIN_COM-VRSN
+...'
+
+>>> print(w)  # print values of all found attributes    
+{
+  "creation_date": "1995-08-14 04:00:00",
+  "expiration_date": "2022-08-13 04:00:00",
+  "updated_date": "2021-08-14 07:01:44",
+  "domain_name": "EXAMPLE.COM",
+  "name_servers": [
+      "A.IANA-SERVERS.NET",
+      "B.IANA-SERVERS.NET"
+  ],
+  ...
+```
 
 Install
 =======
 
 Install from pypi:
 
-.. sourcecode:: bash
-
-    $ pip install python-whois
+```bash
+pip install python-whois
+```
 
 Or checkout latest version from repository:
 
-.. sourcecode:: bash
-
-    $ git clone git@github.com:richardpenman/whois.git
-
-.. sourcecode:: bash
-
-    $ pip install -r requirements.txt
+```bash
+git clone git@github.com:richardpenman/whois.git
+pip install -r requirements.txt
+```
 
 Run test cases:
 
-.. sourcecode:: bash
-
-    $ python -m unittest discover test
-    .............
-    ----------------------------------------------------------------------
-    Ran 13 tests in 1.431s
-    
-    OK
-
-SOCKS Proxy support requirements:
-
-.. sourcecode:: bash
-
-    $ pip install PySocks
-    ............
-    ---------------------------------------------------------------------
-    $ export SOCKS=socksproxy.someplace.com:8080
-
+```bash
+python -m pytest
+```
 
 Problems?
 =========
 
 Pull requests are welcome! 
 
 Thanks to the many who have sent patches for additional TLDs. If you want to add or fix a TLD it's quite straightforward. 
-See example domains in `whois/parser.py <https://github.com/richardpenman/whois/blob/master/whois/parser.py>`_
+See example domains in [whois/parser.py](https://github.com/richardpenman/whois/blob/master/whois/parser.py)
 
 Basically each TLD has a similar format to the following:
 
-.. sourcecode:: python
+```python
+class WhoisOrg(WhoisEntry):
+  """Whois parser for .org domains
+  """
+  regex = {
+    'domain_name':      'Domain Name: *(.+)',
+    'registrar':        'Registrar: *(.+)',
+    'whois_server':     'Whois Server: *(.+)',
+    ...
+  }
 
-    class WhoisOrg(WhoisEntry):
-    """Whois parser for .org domains
-    """
-    regex = {
-        'domain_name':      'Domain Name: *(.+)',
-        'registrar':        'Registrar: *(.+)',
-        'whois_server':     'Whois Server: *(.+)',
-        ...
-    }
-
-    def __init__(self, domain, text):
-        if text.strip() == 'NOT FOUND':
-            raise PywhoisError(text)
-        else:
-            WhoisEntry.__init__(self, domain, text)
+  def __init__(self, domain, text):
+    if text.strip() == 'NOT FOUND':
+      raise PywhoisError(text)
+    else:
+      WhoisEntry.__init__(self, domain, text)
+```
```

### Comparing `python-whois-0.9.3/python_whois.egg-info/PKG-INFO` & `python_whois-0.9.4/python_whois.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,105 @@
 Metadata-Version: 2.1
 Name: python-whois
-Version: 0.9.3
+Version: 0.9.4
 Summary: Whois querying and parsing of domain registration information.
 Home-page: https://github.com/richardpenman/whois
 Author: Richard Penman
 Author-email: richard.penman@gmail.com
 License: MIT
 Keywords: whois,python
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: python-dateutil
 
 Goal
 ====
 
 -  Create a simple importable Python module which will produce parsed
    WHOIS data for a given domain.
 -  Able to extract data for all the popular TLDs (com, org, net, ...)
 -  Query a WHOIS server directly instead of going through an
    intermediate web service like many others do.
 
 
 Example
 =======
 
-.. sourcecode:: bash
-
-    >>> import whois
-    >>> w = whois.whois('example.com')
-    >>> w.expiration_date  # dates converted to datetime object
-    datetime.datetime(2022, 8, 13, 4, 0)
-    >>> w.text  # the content downloaded from whois server
-    u'\nDomain Name: EXAMPLE.COM
-    Registry Domain ID: 2336799_DOMAIN_COM-VRSN
-    ...'
-
-    >>> print(w)  # print values of all found attributes    
-    {
-        "creation_date": "1995-08-14 04:00:00",
-        "expiration_date": "2022-08-13 04:00:00",
-        "updated_date": "2021-08-14 07:01:44",
-        "domain_name": "EXAMPLE.COM",
-        "name_servers": [
-            "A.IANA-SERVERS.NET",
-            "B.IANA-SERVERS.NET"
-        ],
-    ...
-
+```python
+>>> import whois
+>>> w = whois.whois('example.com')
+>>> w.expiration_date  # dates converted to datetime object
+datetime.datetime(2022, 8, 13, 4, 0)
+>>> w.text  # the content downloaded from whois server
+u'\nDomain Name: EXAMPLE.COM
+Registry Domain ID: 2336799_DOMAIN_COM-VRSN
+...'
+
+>>> print(w)  # print values of all found attributes    
+{
+  "creation_date": "1995-08-14 04:00:00",
+  "expiration_date": "2022-08-13 04:00:00",
+  "updated_date": "2021-08-14 07:01:44",
+  "domain_name": "EXAMPLE.COM",
+  "name_servers": [
+      "A.IANA-SERVERS.NET",
+      "B.IANA-SERVERS.NET"
+  ],
+  ...
+```
 
 Install
 =======
 
 Install from pypi:
 
-.. sourcecode:: bash
-
-    $ pip install python-whois
+```bash
+pip install python-whois
+```
 
 Or checkout latest version from repository:
 
-.. sourcecode:: bash
-
-    $ git clone git@github.com:richardpenman/whois.git
-
-.. sourcecode:: bash
-
-    $ pip install -r requirements.txt
+```bash
+git clone git@github.com:richardpenman/whois.git
+pip install -r requirements.txt
+```
 
 Run test cases:
 
-.. sourcecode:: bash
-
-    $ python -m unittest discover test
-    .............
-    ----------------------------------------------------------------------
-    Ran 13 tests in 1.431s
-    
-    OK
-
-SOCKS Proxy support requirements:
-
-.. sourcecode:: bash
-
-    $ pip install PySocks
-    ............
-    ---------------------------------------------------------------------
-    $ export SOCKS=socksproxy.someplace.com:8080
-
+```bash
+python -m pytest
+```
 
 Problems?
 =========
 
 Pull requests are welcome! 
 
 Thanks to the many who have sent patches for additional TLDs. If you want to add or fix a TLD it's quite straightforward. 
-See example domains in `whois/parser.py <https://github.com/richardpenman/whois/blob/master/whois/parser.py>`_
+See example domains in [whois/parser.py](https://github.com/richardpenman/whois/blob/master/whois/parser.py)
 
 Basically each TLD has a similar format to the following:
 
-.. sourcecode:: python
+```python
+class WhoisOrg(WhoisEntry):
+  """Whois parser for .org domains
+  """
+  regex = {
+    'domain_name':      'Domain Name: *(.+)',
+    'registrar':        'Registrar: *(.+)',
+    'whois_server':     'Whois Server: *(.+)',
+    ...
+  }
 
-    class WhoisOrg(WhoisEntry):
-    """Whois parser for .org domains
-    """
-    regex = {
-        'domain_name':      'Domain Name: *(.+)',
-        'registrar':        'Registrar: *(.+)',
-        'whois_server':     'Whois Server: *(.+)',
-        ...
-    }
-
-    def __init__(self, domain, text):
-        if text.strip() == 'NOT FOUND':
-            raise PywhoisError(text)
-        else:
-            WhoisEntry.__init__(self, domain, text)
+  def __init__(self, domain, text):
+    if text.strip() == 'NOT FOUND':
+      raise PywhoisError(text)
+    else:
+      WhoisEntry.__init__(self, domain, text)
+```
```

### Comparing `python-whois-0.9.3/setup.py` & `python_whois-0.9.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 def read(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 
 setuptools.setup(
     name="python-whois",
-    version="0.9.3",
+    version="0.9.4",
     description="Whois querying and parsing of domain registration information.",
-    long_description=read("README.rst"),
+    long_description=read("README.md"),
+    long_description_content_type='text/markdown',
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Internet :: WWW/HTTP",
```

### Comparing `python-whois-0.9.3/test/test_main.py` & `python_whois-0.9.4/test/test_main.py`

 * *Files identical despite different names*

### Comparing `python-whois-0.9.3/test/test_parser.py` & `python_whois-0.9.4/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `python-whois-0.9.3/test/test_query.py` & `python_whois-0.9.4/test/test_query.py`

 * *Files identical despite different names*

### Comparing `python-whois-0.9.3/whois/__init__.py` & `python_whois-0.9.4/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `python-whois-0.9.3/whois/data/public_suffix_list.dat` & `python_whois-0.9.4/whois/data/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `python-whois-0.9.3/whois/parser.py` & `python_whois-0.9.4/whois/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # This module is part of python-whois and is released under
 # the MIT license: http://www.opensource.org/licenses/mit-license.php
 
 import re
 from datetime import datetime
 import json
 import dateutil.parser as dp
+from dateutil.utils import default_tzinfo
 from .time_zones import tz_data
 
 EMAIL_REGEX = (
     r"[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*@(?:[a-z0-9](?:[a-z0-9-]*["
     r"a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?"
 )
 
@@ -56,14 +57,15 @@
     "%d/%m/%Y %H:%M:%S.%f %Z",  # 23/04/2015 12:00:07.619546 EEST
     "%B %d %Y",  # August 14 2017
     "%d.%m.%Y %H:%M:%S",  # 08.03.2014 10:28:24
     "before %b-%Y",  # before aug-1996
     "before %Y-%m-%d",  # before 1996-01-01
     "before %Y%m%d",  # before 19960821
     "%Y-%m-%d %H:%M:%S (%Z%z)",  # 2017-09-26 11:38:29 (GMT+00:00)
+    "%Y-%b-%d.",  # 2024-Apr-02.
 ]
 
 
 class PywhoisError(Exception):
     pass
 
 
@@ -76,17 +78,17 @@
             pass  # Wrong format, keep trying
     return s
 
 
 def cast_date(s, dayfirst=False, yearfirst=False):
     """Convert any date string found in WHOIS to a datetime object."""
     try:
-        return dp.parse(
+        return default_tzinfo(dp.parse(
             s, tzinfos=tz_data, dayfirst=dayfirst, yearfirst=yearfirst
-        ).replace(tzinfo=None)
+        ), datetime.UTC)
     except Exception:
         return datetime_parse(s)
 
 
 class WhoisEntry(dict):
     """Base class for parsing a Whois entries."""
 
@@ -724,15 +726,15 @@
 
 
 class WhoisPl(WhoisEntry):
     """Whois parser for .pl domains"""
 
     regex = {
         "domain_name": r"DOMAIN NAME: *(.+)\n",
-        "name_servers": r"nameservers:((?:\s+.+\n+)*)",
+        "name_servers": r"nameservers:(?:\s+(\S+)\.[^\n]*\n)(?:\s+(\S+)\.[^\n]*\n)?(?:\s+(\S+)\.[^\n]*\n)?(?:\s+(\S+)\.[^\n]*\n)?", # up to 4
         "registrar": r"REGISTRAR:\s*(.+)",
         "registrar_url": r"URL: *(.+)",  # not available
         "status": r"Registration status:\n\s*(.+)",  # not available
         "registrant_name": r"Registrant:\n\s*(.+)",  # not available
         "creation_date": r"(?<! )created: *(.+)\n",
         "expiration_date": r"renewal date: *(.+)",
         "updated_date": r"last modified: *(.+)\n",
@@ -942,19 +944,19 @@
 
 class WhoisJp(WhoisEntry):
     """Whois parser for .jp domains"""
 
     regex = {
         "domain_name": r".*\[Domain Name\]\s*(.+)",
         "registrant_org": r".*\[(?:Organization|Registrant)\](.+)",
-        "creation_date": r"\[(?:Registered Date|Created on)\]\s*(.+)",
-        "expiration_date": r"\[Expires on\]\s*(.+)",
+        "creation_date": r"\[(?:Registered Date|Created on|登録年月日)\]\s*(.+)",
+        "expiration_date": r"\[(?:Expires on|有効期限)\]\s*(.+)",
         "name_servers": r".*\[Name Server\]\s*(.+)",  # list of name servers
-        "updated_date": r"\[Last Updated?\]\s?(.+)",
-        "status": r"\[(?:State|Status)\]\s*(.+)",  # list of statuses
+        "updated_date": r"\[(?:Last Updated|最終更新)?\]\s?(.+)",
+        "status": r"\[(?:State|Status|状態)\]\s*(.+)",  # list of statuses
     }
 
     def __init__(self, domain, text):
         if "No match!!" in text:
             raise PywhoisError(text)
         else:
             WhoisEntry.__init__(self, domain, text, self.regex)
```

### Comparing `python-whois-0.9.3/whois/time_zones.py` & `python_whois-0.9.4/whois/time_zones.py`

 * *Files identical despite different names*

### Comparing `python-whois-0.9.3/whois/whois.py` & `python_whois-0.9.4/whois/whois.py`

 * *Files identical despite different names*

