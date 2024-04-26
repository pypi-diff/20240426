# Comparing `tmp/py12flogging-0.5.0.tar.gz` & `tmp/py12flogging-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py12flogging-0.5.0.tar", last modified: Wed Jan 20 07:28:41 2021, max compression
+gzip compressed data, was "py12flogging-0.6.0.tar", last modified: Fri Apr 26 11:41:21 2024, max compression
```

## Comparing `py12flogging-0.5.0.tar` & `py12flogging-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxr-x   0 optech    (1000) optech    (1000)        0 2021-01-20 07:28:41.000000 py12flogging-0.5.0/
--rw-rw-r--   0 optech    (1000) optech    (1000)       53 2020-09-17 09:16:43.000000 py12flogging-0.5.0/requirements.txt
--rw-rw-r--   0 optech    (1000) optech    (1000)      258 2020-09-17 10:27:26.000000 py12flogging-0.5.0/tox.ini
--rw-rw-r--   0 optech    (1000) optech    (1000)       29 2020-09-17 09:16:43.000000 py12flogging-0.5.0/.pylintrc
--rw-rw-r--   0 optech    (1000) optech    (1000)        6 2021-01-20 07:19:02.000000 py12flogging-0.5.0/VERSION
--rw-rw-r--   0 optech    (1000) optech    (1000)       98 2020-09-17 10:27:26.000000 py12flogging-0.5.0/MANIFEST.in
-drwxrwxr-x   0 optech    (1000) optech    (1000)        0 2021-01-20 07:28:41.000000 py12flogging-0.5.0/py12flogging/
--rw-rw-r--   0 optech    (1000) optech    (1000)    13688 2021-01-20 07:19:02.000000 py12flogging-0.5.0/py12flogging/log_formatter.py
--rw-rw-r--   0 optech    (1000) optech    (1000)     1722 2021-01-20 07:19:02.000000 py12flogging-0.5.0/py12flogging/pprint.py
--rw-rw-r--   0 optech    (1000) optech    (1000)      168 2021-01-20 07:19:02.000000 py12flogging-0.5.0/py12flogging/__init__.py
--rw-rw-r--   0 optech    (1000) optech    (1000)       42 2020-09-17 09:16:43.000000 py12flogging-0.5.0/.coveragerc
--rw-rw-r--   0 optech    (1000) optech    (1000)     1174 2021-01-20 07:19:02.000000 py12flogging-0.5.0/setup.py
--rw-rw-r--   0 optech    (1000) optech    (1000)     2076 2021-01-20 07:19:02.000000 py12flogging-0.5.0/CHANGES.rst
--rw-rw-r--   0 optech    (1000) optech    (1000)    13957 2020-09-17 10:27:26.000000 py12flogging-0.5.0/LICENSE.txt
-drwxrwxr-x   0 optech    (1000) optech    (1000)        0 2021-01-20 07:28:41.000000 py12flogging-0.5.0/py12flogging.egg-info/
--rw-rw-r--   0 optech    (1000) optech    (1000)       13 2021-01-20 07:28:41.000000 py12flogging-0.5.0/py12flogging.egg-info/top_level.txt
--rw-rw-r--   0 optech    (1000) optech    (1000)        1 2021-01-20 07:28:41.000000 py12flogging-0.5.0/py12flogging.egg-info/dependency_links.txt
--rw-rw-r--   0 optech    (1000) optech    (1000)      332 2021-01-20 07:28:41.000000 py12flogging-0.5.0/py12flogging.egg-info/SOURCES.txt
--rw-rw-r--   0 optech    (1000) optech    (1000)     2148 2021-01-20 07:28:41.000000 py12flogging-0.5.0/py12flogging.egg-info/PKG-INFO
--rw-rw-r--   0 optech    (1000) optech    (1000)       38 2021-01-20 07:28:41.000000 py12flogging-0.5.0/setup.cfg
--rw-rw-r--   0 optech    (1000) optech    (1000)     1125 2021-01-20 07:19:02.000000 py12flogging-0.5.0/README.rst
--rw-rw-r--   0 optech    (1000) optech    (1000)     2148 2021-01-20 07:28:41.000000 py12flogging-0.5.0/PKG-INFO
+drwxrwxr-x   0 optech    (1000) optech    (1000)        0 2024-04-26 11:41:21.206852 py12flogging-0.6.0/
+-rw-rw-r--   0 optech    (1000) optech    (1000)       42 2021-04-13 10:20:04.000000 py12flogging-0.6.0/.coveragerc
+-rw-rw-r--   0 optech    (1000) optech    (1000)       29 2021-04-13 10:20:04.000000 py12flogging-0.6.0/.pylintrc
+-rw-rw-r--   0 optech    (1000) optech    (1000)     2464 2024-04-26 11:35:44.000000 py12flogging-0.6.0/CHANGES.rst
+-rw-rw-r--   0 optech    (1000) optech    (1000)    13957 2021-04-13 10:20:05.000000 py12flogging-0.6.0/LICENSE.txt
+-rw-rw-r--   0 optech    (1000) optech    (1000)       98 2021-04-13 10:20:04.000000 py12flogging-0.6.0/MANIFEST.in
+-rw-r--r--   0 optech    (1000) optech    (1000)     1819 2024-04-26 11:41:21.206852 py12flogging-0.6.0/PKG-INFO
+-rw-rw-r--   0 optech    (1000) optech    (1000)     1125 2021-04-13 10:20:05.000000 py12flogging-0.6.0/README.rst
+-rw-rw-r--   0 optech    (1000) optech    (1000)        6 2024-04-26 11:35:44.000000 py12flogging-0.6.0/VERSION
+drwxrwxr-x   0 optech    (1000) optech    (1000)        0 2024-04-26 11:41:21.206852 py12flogging-0.6.0/py12flogging/
+-rw-rw-r--   0 optech    (1000) optech    (1000)      168 2021-04-13 10:20:04.000000 py12flogging-0.6.0/py12flogging/__init__.py
+-rw-rw-r--   0 optech    (1000) optech    (1000)    13688 2021-04-13 10:20:04.000000 py12flogging-0.6.0/py12flogging/log_formatter.py
+-rw-rw-r--   0 optech    (1000) optech    (1000)     1722 2021-04-13 10:20:04.000000 py12flogging-0.6.0/py12flogging/pprint.py
+drwxrwxr-x   0 optech    (1000) optech    (1000)        0 2024-04-26 11:41:21.206852 py12flogging-0.6.0/py12flogging.egg-info/
+-rw-r--r--   0 optech    (1000) optech    (1000)     1819 2024-04-26 11:41:21.000000 py12flogging-0.6.0/py12flogging.egg-info/PKG-INFO
+-rw-rw-r--   0 optech    (1000) optech    (1000)      381 2024-04-26 11:41:21.000000 py12flogging-0.6.0/py12flogging.egg-info/SOURCES.txt
+-rw-rw-r--   0 optech    (1000) optech    (1000)        1 2024-04-26 11:41:21.000000 py12flogging-0.6.0/py12flogging.egg-info/dependency_links.txt
+-rw-rw-r--   0 optech    (1000) optech    (1000)       13 2024-04-26 11:41:21.000000 py12flogging-0.6.0/py12flogging.egg-info/top_level.txt
+-rw-rw-r--   0 optech    (1000) optech    (1000)       83 2024-04-26 11:35:44.000000 py12flogging-0.6.0/requirements.txt
+-rw-rw-r--   0 optech    (1000) optech    (1000)       38 2024-04-26 11:41:21.206852 py12flogging-0.6.0/setup.cfg
+-rw-rw-r--   0 optech    (1000) optech    (1000)     1178 2024-04-26 11:35:44.000000 py12flogging-0.6.0/setup.py
+drwxrwxr-x   0 optech    (1000) optech    (1000)        0 2024-04-26 11:41:21.206852 py12flogging-0.6.0/tests/
+-rw-rw-r--   0 optech    (1000) optech    (1000)    16646 2021-04-13 10:20:04.000000 py12flogging-0.6.0/tests/test_log_formatter.py
+-rw-rw-r--   0 optech    (1000) optech    (1000)     1941 2021-04-13 10:20:04.000000 py12flogging-0.6.0/tests/test_pprint.py
+-rw-rw-r--   0 optech    (1000) optech    (1000)      260 2024-04-26 11:35:44.000000 py12flogging-0.6.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py12flogging-0.5.0/py12flogging/log_formatter.py` & `py12flogging-0.6.0/py12flogging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `py12flogging-0.5.0/py12flogging/pprint.py` & `py12flogging-0.6.0/py12flogging/pprint.py`

 * *Files identical despite different names*

### Comparing `py12flogging-0.5.0/setup.py` & `py12flogging-0.6.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 with open('VERSION', 'r') as fh:
     version = fh.readline().strip()
 
 
 setup(
     name='py12flogging',
     version=version,
-    url='https://bitbucket.org/tietoarkisto/py12flogging',
+    url='https://gitlab.tuni.fi/fsd/py12flogging',
     description='Python logging module for developing microservices '
     'conforming to 12 Factor App methodology.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     license='EUPL v1.2',
     author='Toni Sissala',
-    author_email='toni.sissala@tuni.fi',
+    author_email='support.fsd+py12flogging@tuni.fi',
     packages=find_packages(),
     classifiers=(
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
         "Programming Language :: Python",
```

### Comparing `py12flogging-0.5.0/CHANGES.rst` & `py12flogging-0.6.0/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 Py12fLogging Changelog
 ======================
 
 
+0.6.0 (2024-04-26)
+------------------
+
+* Use 'python-latest' in Jenkinsfile instead of 'python3'. In FSD
+  Jenkins environment the python-latest always points to latest
+  installed Python.
+* Add py39, py310, py311 to tox test environments and use it in Jenkinsfile.
+* Drop py35, py36, py37 from tox test environments and Jenkinsfile.
+* Change project url from bitbucket to gitlab.tuni.
+
+
 0.5.0 (2021-01-20)
 ------------------
 
 * Maintenance release fixes setup.py long_description_content_type to
   make it compatible with PyPI. PyPI expects content type value
   'text/x-rst' for reStructuredText.
 * Remove the step to obtain package from README.rst since pip can
```

### Comparing `py12flogging-0.5.0/LICENSE.txt` & `py12flogging-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py12flogging-0.5.0/py12flogging.egg-info/PKG-INFO` & `py12flogging-0.6.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: py12flogging
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python logging module for developing microservices conforming to 12 Factor App methodology.
-Home-page: https://bitbucket.org/tietoarkisto/py12flogging
+Home-page: https://gitlab.tuni.fi/fsd/py12flogging
 Author: Toni Sissala
-Author-email: toni.sissala@tuni.fi
+Author-email: support.fsd+py12flogging@tuni.fi
 License: EUPL v1.2
-Description: Py12fLogging
-        ============
-        
-        Python logging module for developing microservices conforming to 12 Factor App
-        methodology. Depends only on Python standard lib. However, setuptools may be
-        installed to provide additional functionality.
-        
-        
-        Installation
-        ------------
-        
-        Py12fLogging is available to install from PyPI::
-        
-           pip install py12flogging
-        
-        
-        Usage
-        -----
-        
-        Py12fLogging is a module used for developing microservices. It is not a standalone
-        application. See module documentation for more information.
-        
-        Example use of log_formatter -module::
-        
-           import logging
-           from py12flogging import log_formatter
-           log_formatter.setup_app_logging('my_app')
-           logging.info('all done')
-        
-        
-        PrettyPrint logging output
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        Developers may wish to restructure log output stream of an application while it's
-        under development. This can be achieved by using pprint command line application,
-        which prettyprints the log output stream coming from stdin and flushes immediately
-        to stdout. See module documentation for more information.
-        
-        Pipe application's stdout to pprint-module::
-        
-           ./my_app.py | python -m py12flogging.pprint
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+Py12fLogging
+============
+
+Python logging module for developing microservices conforming to 12 Factor App
+methodology. Depends only on Python standard lib. However, setuptools may be
+installed to provide additional functionality.
+
+
+Installation
+------------
+
+Py12fLogging is available to install from PyPI::
+
+   pip install py12flogging
+
+
+Usage
+-----
+
+Py12fLogging is a module used for developing microservices. It is not a standalone
+application. See module documentation for more information.
+
+Example use of log_formatter -module::
+
+   import logging
+   from py12flogging import log_formatter
+   log_formatter.setup_app_logging('my_app')
+   logging.info('all done')
+
+
+PrettyPrint logging output
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Developers may wish to restructure log output stream of an application while it's
+under development. This can be achieved by using pprint command line application,
+which prettyprints the log output stream coming from stdin and flushes immediately
+to stdout. See module documentation for more information.
+
+Pipe application's stdout to pprint-module::
+
+   ./my_app.py | python -m py12flogging.pprint
```

### Comparing `py12flogging-0.5.0/README.rst` & `py12flogging-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `py12flogging-0.5.0/PKG-INFO` & `py12flogging-0.6.0/py12flogging.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: py12flogging
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python logging module for developing microservices conforming to 12 Factor App methodology.
-Home-page: https://bitbucket.org/tietoarkisto/py12flogging
+Home-page: https://gitlab.tuni.fi/fsd/py12flogging
 Author: Toni Sissala
-Author-email: toni.sissala@tuni.fi
+Author-email: support.fsd+py12flogging@tuni.fi
 License: EUPL v1.2
-Description: Py12fLogging
-        ============
-        
-        Python logging module for developing microservices conforming to 12 Factor App
-        methodology. Depends only on Python standard lib. However, setuptools may be
-        installed to provide additional functionality.
-        
-        
-        Installation
-        ------------
-        
-        Py12fLogging is available to install from PyPI::
-        
-           pip install py12flogging
-        
-        
-        Usage
-        -----
-        
-        Py12fLogging is a module used for developing microservices. It is not a standalone
-        application. See module documentation for more information.
-        
-        Example use of log_formatter -module::
-        
-           import logging
-           from py12flogging import log_formatter
-           log_formatter.setup_app_logging('my_app')
-           logging.info('all done')
-        
-        
-        PrettyPrint logging output
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        Developers may wish to restructure log output stream of an application while it's
-        under development. This can be achieved by using pprint command line application,
-        which prettyprints the log output stream coming from stdin and flushes immediately
-        to stdout. See module documentation for more information.
-        
-        Pipe application's stdout to pprint-module::
-        
-           ./my_app.py | python -m py12flogging.pprint
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+Py12fLogging
+============
+
+Python logging module for developing microservices conforming to 12 Factor App
+methodology. Depends only on Python standard lib. However, setuptools may be
+installed to provide additional functionality.
+
+
+Installation
+------------
+
+Py12fLogging is available to install from PyPI::
+
+   pip install py12flogging
+
+
+Usage
+-----
+
+Py12fLogging is a module used for developing microservices. It is not a standalone
+application. See module documentation for more information.
+
+Example use of log_formatter -module::
+
+   import logging
+   from py12flogging import log_formatter
+   log_formatter.setup_app_logging('my_app')
+   logging.info('all done')
+
+
+PrettyPrint logging output
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Developers may wish to restructure log output stream of an application while it's
+under development. This can be achieved by using pprint command line application,
+which prettyprints the log output stream coming from stdin and flushes immediately
+to stdout. See module documentation for more information.
+
+Pipe application's stdout to pprint-module::
+
+   ./my_app.py | python -m py12flogging.pprint
```

