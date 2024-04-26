# Comparing `tmp/PyQt6_NetworkAuth-6.6.0.tar.gz` & `tmp/PyQt6_NetworkAuth-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_NetworkAuth-6.6.0.tar", last modified: Wed Oct 25 10:24:16 2023, max compression
+gzip compressed data, was "PyQt6_NetworkAuth-6.7.0.tar", last modified: Sat Apr 20 16:02:48 2024, max compression
```

## Comparing `PyQt6_NetworkAuth-6.6.0.tar` & `PyQt6_NetworkAuth-6.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:24:16.028172 PyQt6_NetworkAuth-6.6.0/
--rw-r--r--   0 phil       (501) staff       (20)     5441 2023-10-25 10:24:15.555321 PyQt6_NetworkAuth-6.6.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2023-10-25 10:24:15.332440 PyQt6_NetworkAuth-6.6.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      744 2023-10-25 10:23:49.612040 PyQt6_NetworkAuth-6.6.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1663 2023-10-25 10:24:16.028390 PyQt6_NetworkAuth-6.6.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1315 2023-10-25 10:24:15.556802 PyQt6_NetworkAuth-6.6.0/README
--rw-r--r--   0 phil       (501) staff       (20)      852 2023-10-25 10:24:15.557282 PyQt6_NetworkAuth-6.6.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:24:16.024564 PyQt6_NetworkAuth-6.6.0/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:24:16.027929 PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/
--rw-r--r--   0 phil       (501) staff       (20)     2608 2023-10-25 10:24:15.829358 PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/QtNetworkAuthmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     8253 2023-10-25 10:24:15.826459 PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qabstractoauth.sip
--rw-r--r--   0 phil       (501) staff       (20)     3807 2023-10-25 10:24:15.827774 PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qabstractoauth2.sip
--rw-r--r--   0 phil       (501) staff       (20)     1693 2023-10-25 10:24:15.828303 PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qabstractoauthreplyhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     4170 2023-10-25 10:24:15.824247 PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qoauth1.sip
--rw-r--r--   0 phil       (501) staff       (20)     2829 2023-10-25 10:24:15.824944 PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qoauth1signature.sip
--rw-r--r--   0 phil       (501) staff       (20)     2386 2023-10-25 10:24:15.827017 PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qoauth2authorizationcodeflow.sip
--rw-r--r--   0 phil       (501) staff       (20)     1967 2023-10-25 10:24:15.829906 PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qoauthhttpserverreplyhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     1289 2023-10-25 10:24:15.828791 PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qoauthoobreplyhandler.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:48.546630 PyQt6_NetworkAuth-6.7.0/
+-rw-r--r--   0 phil       (501) staff       (20)     6242 2024-04-20 16:02:48.377769 PyQt6_NetworkAuth-6.7.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2024-04-20 16:02:48.282633 PyQt6_NetworkAuth-6.7.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      798 2024-04-20 16:02:32.386901 PyQt6_NetworkAuth-6.7.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1592 2024-04-20 16:02:48.546692 PyQt6_NetworkAuth-6.7.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1198 2024-04-20 16:02:48.378365 PyQt6_NetworkAuth-6.7.0/README.md
+-rw-r--r--   0 phil       (501) staff       (20)      820 2024-04-20 16:02:48.378579 PyQt6_NetworkAuth-6.7.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:48.545056 PyQt6_NetworkAuth-6.7.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:48.546498 PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/
+-rw-r--r--   0 phil       (501) staff       (20)     2628 2024-04-20 16:02:48.447375 PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/QtNetworkAuthmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8260 2024-04-20 16:02:48.445948 PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qabstractoauth.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3814 2024-04-20 16:02:48.446631 PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qabstractoauth2.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1700 2024-04-20 16:02:48.446885 PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qabstractoauthreplyhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4177 2024-04-20 16:02:48.444679 PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qoauth1.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2829 2024-04-20 16:02:48.445089 PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qoauth1signature.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2393 2024-04-20 16:02:48.446246 PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qoauth2authorizationcodeflow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1974 2024-04-20 16:02:48.447637 PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qoauthhttpserverreplyhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1296 2024-04-20 16:02:48.447100 PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qoauthoobreplyhandler.sip
```

### Comparing `PyQt6_NetworkAuth-6.6.0/ChangeLog` & `PyQt6_NetworkAuth-6.7.0/ChangeLog`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+2024-04-04  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS:
+	Updated for Qt v6.7.0.
+	[686cca14f4f0] [6.7.0]
+
+2024-03-17  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-NetworkAuth.msp:
+	Added support for Qt v6.7.
+	[e821a4224d36]
+
+2024-02-18  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* README, README.md, pyproject.toml:
+	Migrated from [tool.sip.metadata] to [project] in pyproject.toml.
+	[2ab86f3f05f4]
+
+	* NEWS:
+	Updated the NEWS file.
+	[98a66d7a068d]
+
+	* Merged the 6.6-maint branch.
+	[4341bead3405]
+
+2024-01-02  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, rb-product.toml:
+	Removed the product file.
+	[d5c83b6d20ac] <6.6-maint>
+
+2023-10-25  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* .hgtags:
+	Added tag 6.6.0 for changeset dc9c78d01cb5
+	[c4b8af0f94e3]
+
 2023-10-22  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, PyQt6-NetworkAuth.msp:
 	Updated for Qt v6.6.
 	[dc9c78d01cb5] [6.6.0]
 
 2023-04-04  Phil Thompson  <phil@riverbankcomputing.com>
```

### Comparing `PyQt6_NetworkAuth-6.6.0/LICENSE` & `PyQt6_NetworkAuth-6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_NetworkAuth-6.6.0/NEWS` & `PyQt6_NetworkAuth-6.7.0/NEWS`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+v6.7.0 4th April 2024
+  - Added support for Qt v6.7.
+
 v6.6.0 22nd October 2023
   - Added support for Qt v6.6.
 
 v6.5.0 31st March 2023
   - Added support for Qt v6.5.
 
 v6.4.0 30th September 2022
```

### Comparing `PyQt6_NetworkAuth-6.6.0/PKG-INFO` & `PyQt6_NetworkAuth-6.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 Metadata-Version: 2.1
 Name: PyQt6-NetworkAuth
-Version: 6.6.0
-Requires-Python: >=3.7
+Version: 6.7.0
+Requires-Python: >=3.8
 Summary: Python bindings for the Qt Network Authorization library
-Home-Page: https://www.riverbankcomputing.com/software/pyqtnetworkauth/
-Author: Riverbank Computing Limited
-Author-Email: info@riverbankcomputing.com
-License: GPL v3
+Description-Content-Type: text/markdown
+Project-Url: homepage, https://www.riverbankcomputing.com/software/pyqtnetworkauth/
 Requires-Dist: PyQt6 (>=6.2.0)
+License: GPL v3
+Author-Email: Riverbank Computing Limited <info@riverbankcomputing.com>
 
-PyQt6-NetworkAuth - Python Bindings for the Qt Network Authorization Library
-============================================================================
+# PyQt6-NetworkAuth - Python Bindings for the Qt Network Authorization Library
 
 PyQt6-NetworkAuth is a set of Python bindings for The Qt Company's Qt Network
 Authorisation library.  The bindings sit on top of PyQt6 and are implemented as
 a single module.
 
 
-Author
-------
+## Author
 
 PyQt6-NetworkAuth is copyright (c) Riverbank Computing Limited.  Its homepage
 is https://www.riverbankcomputing.com/software/pyqtnetworkauth/.
 
 Support may be obtained from the PyQt mailing list at
 https://www.riverbankcomputing.com/mailman/listinfo/pyqt/.
 
 
-License
--------
+## License
 
 PyQt6-NetworkAuth is released under the GPL v3 license and under a commercial
 license that allows for the development of proprietary applications.
 
 
-Documentation
--------------
+## Documentation
 
 The documentation for the latest release can be found
-`here <https://www.riverbankcomputing.com/static/Docs/PyQt6/>`__.
+[here](https://www.riverbankcomputing.com/static/Docs/PyQt6/).
 
 
-Installation
-------------
+## Installation
 
-The GPL version of PyQt6-NetworkAuth can be installed from PyPI::
+The GPL version of PyQt6-NetworkAuth can be installed from PyPI:
 
     pip install PyQt6-NetworkAuth
 
-``pip`` will also build and install the bindings from the sdist package but
-Qt's ``qmake`` tool must be on ``PATH``.
+`pip` will also build and install the bindings from the sdist package but Qt's
+`qmake` tool must be on `PATH`.
 
-The ``sip-install`` tool will also install the bindings from the sdist package
+The `sip-install` tool will also install the bindings from the sdist package
 but will allow you to configure many aspects of the installation.
```

### Comparing `PyQt6_NetworkAuth-6.6.0/README` & `PyQt6_NetworkAuth-6.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-PyQt6-NetworkAuth - Python Bindings for the Qt Network Authorization Library
-============================================================================
+# PyQt6-NetworkAuth - Python Bindings for the Qt Network Authorization Library
 
 PyQt6-NetworkAuth is a set of Python bindings for The Qt Company's Qt Network
 Authorisation library.  The bindings sit on top of PyQt6 and are implemented as
 a single module.
 
 
-Author
-------
+## Author
 
 PyQt6-NetworkAuth is copyright (c) Riverbank Computing Limited.  Its homepage
 is https://www.riverbankcomputing.com/software/pyqtnetworkauth/.
 
 Support may be obtained from the PyQt mailing list at
 https://www.riverbankcomputing.com/mailman/listinfo/pyqt/.
 
 
-License
--------
+## License
 
 PyQt6-NetworkAuth is released under the GPL v3 license and under a commercial
 license that allows for the development of proprietary applications.
 
 
-Documentation
--------------
+## Documentation
 
 The documentation for the latest release can be found
-`here <https://www.riverbankcomputing.com/static/Docs/PyQt6/>`__.
+[here](https://www.riverbankcomputing.com/static/Docs/PyQt6/).
 
 
-Installation
-------------
+## Installation
 
-The GPL version of PyQt6-NetworkAuth can be installed from PyPI::
+The GPL version of PyQt6-NetworkAuth can be installed from PyPI:
 
     pip install PyQt6-NetworkAuth
 
-``pip`` will also build and install the bindings from the sdist package but
-Qt's ``qmake`` tool must be on ``PATH``.
+`pip` will also build and install the bindings from the sdist package but Qt's
+`qmake` tool must be on `PATH`.
 
-The ``sip-install`` tool will also install the bindings from the sdist package
+The `sip-install` tool will also install the bindings from the sdist package
 but will allow you to configure many aspects of the installation.
```

### Comparing `PyQt6_NetworkAuth-6.6.0/pyproject.toml` & `PyQt6_NetworkAuth-6.7.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Specify the build system for the project.
 [build-system]
-requires = ["sip >=6, <7", "PyQt-builder >=1.9, <2"]
+requires = ["sip >=6.8, <7", "PyQt-builder >=1.9, <2"]
 build-backend = "sipbuild.api"
 
-# Specify the PEP 566 metadata for the project.
-[tool.sip.metadata]
+[project]
 name = "PyQt6-NetworkAuth"
-version = "6.6.0"
-summary = "Python bindings for the Qt Network Authorization library"
-home-page = "https://www.riverbankcomputing.com/software/pyqtnetworkauth/"
-author = "Riverbank Computing Limited"
-author-email = "info@riverbankcomputing.com"
-license = "GPL v3"
-description-file = "README"
-requires-dist = "PyQt6 (>=6.2.0)"
+version = "6.7.0"
+description = "Python bindings for the Qt Network Authorization library"
+readme = "README.md"
+urls.homepage = "https://www.riverbankcomputing.com/software/pyqtnetworkauth/"
+dependencies = ["PyQt6 (>=6.2.0)"]
+license = {text = "GPL v3"}
+
+[[project.authors]]
+name = "Riverbank Computing Limited"
+email = "info@riverbankcomputing.com"
+
 
 # Specify a PyQt-based project.
 [tool.sip]
 project-factory = "pyqtbuild:PyQtProject"
 
 # Configure the project.
 [tool.sip.project]
```

### Comparing `PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/QtNetworkAuthmod.sip` & `PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/QtNetworkAuthmod.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtNetworkAuthmod.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -21,18 +21,18 @@
 
 
 %Module(name=PyQt6.QtNetworkAuth, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtCore/QtCoremod.sip
 %Import QtNetwork/QtNetworkmod.sip
 
-%Timeline {QtNetworkAuth_6_0_0 QtNetworkAuth_6_1_0 QtNetworkAuth_6_2_0 QtNetworkAuth_6_3_0 QtNetworkAuth_6_4_0 QtNetworkAuth_6_5_0 QtNetworkAuth_6_6_0}
+%Timeline {QtNetworkAuth_6_0_0 QtNetworkAuth_6_1_0 QtNetworkAuth_6_2_0 QtNetworkAuth_6_3_0 QtNetworkAuth_6_4_0 QtNetworkAuth_6_5_0 QtNetworkAuth_6_6_0 QtNetworkAuth_6_7_0}
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-NetworkAuth.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
@@ -48,16 +48,16 @@
 
 %DefaultSupertype PyQt6.sip.simplewrapper
 
 int PYQT_NETWORKAUTH_VERSION;
 const char *PYQT_NETWORKAUTH_VERSION_STR;
 
 %ModuleCode
-static int PYQT_NETWORKAUTH_VERSION = 0x060600;
-static const char *PYQT_NETWORKAUTH_VERSION_STR = "6.6.0";
+static int PYQT_NETWORKAUTH_VERSION = 0x060700;
+static const char *PYQT_NETWORKAUTH_VERSION_STR = "6.7.0";
 %End
 
 %Include qabstractoauth.sip
 %Include qabstractoauth2.sip
 %Include qabstractoauthreplyhandler.sip
 %Include qoauth1.sip
 %Include qoauth1signature.sip
```

### Comparing `PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qabstractoauth.sip` & `PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qabstractoauth.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractoauth.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAbstractOAuth : QObject /NoDefaultCtors/
+class QAbstractOAuth : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qabstractoauth.h>
 %End
 
 %ConvertToSubClassCode
     static struct class_graph {
```

### Comparing `PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qabstractoauth2.sip` & `PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qabstractoauth2.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractoauth2.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAbstractOAuth2 : QAbstractOAuth
+class QAbstractOAuth2 : public QAbstractOAuth
 {
 %TypeHeaderCode
 #include <qabstractoauth2.h>
 %End
 
 public:
     explicit QAbstractOAuth2(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qabstractoauthreplyhandler.sip` & `PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qabstractoauthreplyhandler.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractoauthreplyhandler.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAbstractOAuthReplyHandler : QObject
+class QAbstractOAuthReplyHandler : public QObject
 {
 %TypeHeaderCode
 #include <qabstractoauthreplyhandler.h>
 %End
 
 public:
     explicit QAbstractOAuthReplyHandler(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qoauth1.sip` & `PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qoauth1.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qoauth1.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QOAuth1 : QAbstractOAuth
+class QOAuth1 : public QAbstractOAuth
 {
 %TypeHeaderCode
 #include <qoauth1.h>
 %End
 
 public:
     enum class SignatureMethod
```

### Comparing `PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qoauth1signature.sip` & `PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qoauth1signature.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qoauth1signature.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qoauth2authorizationcodeflow.sip` & `PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qoauth2authorizationcodeflow.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qoauth2authorizationcodeflow.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QOAuth2AuthorizationCodeFlow : QAbstractOAuth2
+class QOAuth2AuthorizationCodeFlow : public QAbstractOAuth2
 {
 %TypeHeaderCode
 #include <qoauth2authorizationcodeflow.h>
 %End
 
 public:
     explicit QOAuth2AuthorizationCodeFlow(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qoauthhttpserverreplyhandler.sip` & `PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qoauthhttpserverreplyhandler.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qoauthhttpserverreplyhandler.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QOAuthHttpServerReplyHandler : QOAuthOobReplyHandler
+class QOAuthHttpServerReplyHandler : public QOAuthOobReplyHandler
 {
 %TypeHeaderCode
 #include <qoauthhttpserverreplyhandler.h>
 %End
 
 public:
     explicit QOAuthHttpServerReplyHandler(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_NetworkAuth-6.6.0/sip/QtNetworkAuth/qoauthoobreplyhandler.sip` & `PyQt6_NetworkAuth-6.7.0/sip/QtNetworkAuth/qoauthoobreplyhandler.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qoauthoobreplyhandler.sip generated by MetaSIP
 //
 // This file is part of the QtNetworkAuth Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-NetworkAuth.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QOAuthOobReplyHandler : QAbstractOAuthReplyHandler
+class QOAuthOobReplyHandler : public QAbstractOAuthReplyHandler
 {
 %TypeHeaderCode
 #include <qoauthoobreplyhandler.h>
 %End
 
 public:
     explicit QOAuthOobReplyHandler(QObject *parent /TransferThis/ = 0);
```

