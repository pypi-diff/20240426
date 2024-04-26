# Comparing `tmp/PyQt6_WebEngine-6.6.0.tar.gz` & `tmp/PyQt6_WebEngine-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_WebEngine-6.6.0.tar", last modified: Wed Oct 25 10:26:54 2023, max compression
+gzip compressed data, was "PyQt6_WebEngine-6.7.0.tar", last modified: Sat Apr 20 16:04:26 2024, max compression
```

## Comparing `PyQt6_WebEngine-6.6.0.tar` & `PyQt6_WebEngine-6.7.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:26:54.697210 PyQt6_WebEngine-6.6.0/
--rw-r--r--   0 phil       (501) staff       (20)     4655 2023-10-25 10:26:54.015344 PyQt6_WebEngine-6.6.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2023-10-25 10:26:53.806290 PyQt6_WebEngine-6.6.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      515 2023-10-25 10:24:17.227279 PyQt6_WebEngine-6.6.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1787 2023-10-25 10:26:54.697385 PyQt6_WebEngine-6.6.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1453 2023-10-25 10:26:54.016675 PyQt6_WebEngine-6.6.0/README
--rw-r--r--   0 phil       (501) staff       (20)      959 2023-10-25 10:26:54.017134 PyQt6_WebEngine-6.6.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:26:54.683315 PyQt6_WebEngine-6.6.0/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:26:54.696855 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/
--rw-r--r--   0 phil       (501) staff       (20)     3502 2023-10-25 10:26:54.460937 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/QtWebEngineCoremod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1440 2023-10-25 10:26:54.471652 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qtwebenginecoreglobal.sip
--rw-r--r--   0 phil       (501) staff       (20)     2140 2023-10-25 10:26:54.461552 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginecertificateerror.sip
--rw-r--r--   0 phil       (501) staff       (20)     1425 2023-10-25 10:26:54.458565 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineclientcertificateselection.sip
--rw-r--r--   0 phil       (501) staff       (20)     1397 2023-10-25 10:26:54.450241 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineclientcertificatestore.sip
--rw-r--r--   0 phil       (501) staff       (20)     2535 2023-10-25 10:26:54.467954 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginecontextmenurequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     4428 2023-10-25 10:26:54.464670 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginecookiestore.sip
--rw-r--r--   0 phil       (501) staff       (20)     3408 2023-10-25 10:26:54.453475 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginedownloadrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2069 2023-10-25 10:26:54.457454 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginefilesystemaccessrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1282 2023-10-25 10:26:54.459069 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginefindtextresult.sip
--rw-r--r--   0 phil       (501) staff       (20)     1296 2023-10-25 10:26:54.468919 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginefullscreenrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1415 2023-10-25 10:26:54.469471 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineglobalsettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     2995 2023-10-25 10:26:54.455083 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginehistory.sip
--rw-r--r--   0 phil       (501) staff       (20)     2156 2023-10-25 10:26:54.463104 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginehttprequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2576 2023-10-25 10:26:54.470176 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineloadinginfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1741 2023-10-25 10:26:54.455667 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginenavigationrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1495 2023-10-25 10:26:54.456218 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginenewwindowrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1526 2023-10-25 10:26:54.463638 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginenotification.sip
--rw-r--r--   0 phil       (501) staff       (20)    14877 2023-10-25 10:26:54.467186 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginepage.sip
--rw-r--r--   0 phil       (501) staff       (20)     8472 2023-10-25 10:26:54.452499 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineprofile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1333 2023-10-25 10:26:54.460245 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginequotarequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1435 2023-10-25 10:26:54.462540 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineregisterprotocolhandlerrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2015 2023-10-25 10:26:54.456831 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginescript.sip
--rw-r--r--   0 phil       (501) staff       (20)     1522 2023-10-25 10:26:54.462050 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginescriptcollection.sip
--rw-r--r--   0 phil       (501) staff       (20)     3766 2023-10-25 10:26:54.471067 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginesettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     2692 2023-10-25 10:26:54.454241 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineurlrequestinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1349 2023-10-25 10:26:54.450787 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineurlrequestinterceptor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1759 2023-10-25 10:26:54.458040 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineurlrequestjob.sip
--rw-r--r--   0 phil       (501) staff       (20)     2396 2023-10-25 10:26:54.459746 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineurlscheme.sip
--rw-r--r--   0 phil       (501) staff       (20)     1277 2023-10-25 10:26:54.468422 PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineurlschemehandler.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:26:54.682868 PyQt6_WebEngine-6.6.0/sip/QtWebEngineQuick/
--rw-r--r--   0 phil       (501) staff       (20)     2077 2023-10-25 10:26:54.447982 PyQt6_WebEngine-6.6.0/sip/QtWebEngineQuick/QtWebEngineQuickmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     4597 2023-10-25 10:26:54.449082 PyQt6_WebEngine-6.6.0/sip/QtWebEngineQuick/qquickwebengineprofile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1094 2023-10-25 10:26:54.449583 PyQt6_WebEngine-6.6.0/sip/QtWebEngineQuick/qtwebenginequickglobal.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:26:54.680013 PyQt6_WebEngine-6.6.0/sip/QtWebEngineWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2225 2023-10-25 10:26:54.447385 PyQt6_WebEngine-6.6.0/sip/QtWebEngineWidgets/QtWebEngineWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     7637 2023-10-25 10:26:54.446753 PyQt6_WebEngine-6.6.0/sip/QtWebEngineWidgets/qwebengineview.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:04:26.502966 PyQt6_WebEngine-6.7.0/
+-rw-r--r--   0 phil       (501) staff       (20)     5452 2024-04-20 16:04:26.300186 PyQt6_WebEngine-6.7.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2024-04-20 16:04:26.205870 PyQt6_WebEngine-6.7.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      569 2024-04-20 16:02:49.714136 PyQt6_WebEngine-6.7.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1728 2024-04-20 16:04:26.503033 PyQt6_WebEngine-6.7.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1348 2024-04-20 16:04:26.300837 PyQt6_WebEngine-6.7.0/README.md
+-rw-r--r--   0 phil       (501) staff       (20)      927 2024-04-20 16:04:26.301065 PyQt6_WebEngine-6.7.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:04:26.497171 PyQt6_WebEngine-6.7.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:04:26.502848 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/
+-rw-r--r--   0 phil       (501) staff       (20)     3603 2024-04-20 16:04:26.392469 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/QtWebEngineCoremod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1440 2024-04-20 16:04:26.398302 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qtwebenginecoreglobal.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2140 2024-04-20 16:04:26.392755 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginecertificateerror.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1425 2024-04-20 16:04:26.391109 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineclientcertificateselection.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1397 2024-04-20 16:04:26.387141 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineclientcertificatestore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2542 2024-04-20 16:04:26.396548 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginecontextmenurequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3450 2024-04-20 16:04:26.394651 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginecookiestore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1416 2024-04-20 16:04:26.392120 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginedesktopmediarequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3415 2024-04-20 16:04:26.388687 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginedownloadrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2069 2024-04-20 16:04:26.390600 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginefilesystemaccessrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1282 2024-04-20 16:04:26.391329 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginefindtextresult.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1296 2024-04-20 16:04:26.396982 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginefullscreenrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1415 2024-04-20 16:04:26.397239 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineglobalsettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3009 2024-04-20 16:04:26.389482 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginehistory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2156 2024-04-20 16:04:26.393934 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginehttprequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2576 2024-04-20 16:04:26.397575 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineloadinginfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1748 2024-04-20 16:04:26.389760 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginenavigationrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1502 2024-04-20 16:04:26.390009 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginenewwindowrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1533 2024-04-20 16:04:26.394189 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginenotification.sip
+-rw-r--r--   0 phil       (501) staff       (20)    15100 2024-04-20 16:04:26.396153 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginepage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8713 2024-04-20 16:04:26.388211 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineprofile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1333 2024-04-20 16:04:26.391887 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginequotarequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1435 2024-04-20 16:04:26.393655 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineregisterprotocolhandlerrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2015 2024-04-20 16:04:26.390301 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginescript.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1522 2024-04-20 16:04:26.392990 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginescriptcollection.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3820 2024-04-20 16:04:26.398051 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginesettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2759 2024-04-20 16:04:26.389078 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineurlrequestinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1356 2024-04-20 16:04:26.387362 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineurlrequestinterceptor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1833 2024-04-20 16:04:26.390884 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineurlrequestjob.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2396 2024-04-20 16:04:26.391666 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineurlscheme.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1284 2024-04-20 16:04:26.396762 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineurlschemehandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2904 2024-04-20 16:04:26.393423 PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginewebauthuxrequest.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:04:26.496979 PyQt6_WebEngine-6.7.0/sip/QtWebEngineQuick/
+-rw-r--r--   0 phil       (501) staff       (20)     2077 2024-04-20 16:04:26.386064 PyQt6_WebEngine-6.7.0/sip/QtWebEngineQuick/QtWebEngineQuickmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4671 2024-04-20 16:04:26.386633 PyQt6_WebEngine-6.7.0/sip/QtWebEngineQuick/qquickwebengineprofile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1094 2024-04-20 16:04:26.386854 PyQt6_WebEngine-6.7.0/sip/QtWebEngineQuick/qtwebenginequickglobal.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:04:26.496410 PyQt6_WebEngine-6.7.0/sip/QtWebEngineWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2225 2024-04-20 16:04:26.385805 PyQt6_WebEngine-6.7.0/sip/QtWebEngineWidgets/QtWebEngineWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7644 2024-04-20 16:04:26.385480 PyQt6_WebEngine-6.7.0/sip/QtWebEngineWidgets/qwebengineview.sip
```

### Comparing `PyQt6_WebEngine-6.6.0/ChangeLog` & `PyQt6_WebEngine-6.7.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,44 @@
+2024-04-04  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-WebEngine.msp:
+	Updated for Qt v6.7.0.
+	[cb8b0faaaac7] [6.7.0]
+
+2024-03-17  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-WebEngine.msp, mksccode/QtWebEngineCore.versions:
+	Added support for Qt v6.7.
+	[10ef78663bab]
+
+2024-02-18  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* README, README.md, pyproject.toml:
+	Migrated from [tool.sip.metadata] to [project] in pyproject.toml.
+	[44c8b10a047b]
+
+	* NEWS:
+	Updated the NEWS file.
+	[dfeb66ea536b]
+
+	* Merged the 6.6-maint branch.
+	[4ff980ee9851]
+
+2024-01-02  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, rb-product.toml:
+	Removed the product file.
+	[b7be550b308f] <6.6-maint>
+
 2023-10-25  Phil Thompson  <phil@riverbankcomputing.com>
 
+	* .hgtags:
+	Added tag 6.6.0 for changeset 6b4eda057dbf
+	[35b28a4bc972]
+
 	* NEWS, rb-product.toml:
 	Removed an out of date entry in the product file.
 	[6b4eda057dbf] [6.6.0]
 
 2023-10-22  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, PyQt6-WebEngine.msp:
```

### Comparing `PyQt6_WebEngine-6.6.0/LICENSE` & `PyQt6_WebEngine-6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_WebEngine-6.6.0/NEWS` & `PyQt6_WebEngine-6.7.0/NEWS`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+v6.7.0 4th April 2024
+  - Added support for Qt v6.7.
+
 v6.6.0 25th October 2023
   - Added support for Qt v6.6.
 
 v6.5.0 31st March 2023
   - Added support for Qt v6.5.
 
 v6.4.0 30th September 2022
```

### Comparing `PyQt6_WebEngine-6.6.0/PKG-INFO` & `PyQt6_WebEngine-6.7.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,41 @@
-Metadata-Version: 2.1
-Name: PyQt6-WebEngine
-Version: 6.6.0
-Requires-Python: >=3.7
-Summary: Python bindings for the Qt WebEngine framework
-Home-Page: https://www.riverbankcomputing.com/software/pyqtwebengine/
-Author: Riverbank Computing Limited
-Author-Email: info@riverbankcomputing.com
-License: GPL v3
-Requires-Dist: PyQt6 (>=6.2.0)
-
-PyQt6-WebEngine - Python Bindings for the Qt WebEngine Framework
-================================================================
+# PyQt6-WebEngine - Python Bindings for the Qt WebEngine Framework
 
 PyQt6-WebEngine is a set of Python bindings for The Qt Company's Qt WebEngine
 framework.  The framework provides the ability to embed web content in
 applications and is based on the Chrome browser.  The bindings sit on top of
 PyQt6 and are implemented as three separate modules corresponding to the
 different libraries that make up the framework.
 
 
-Author
-------
+## Author
 
 PyQt6-WebEngine is copyright (c) Riverbank Computing Limited.  Its homepage is
 https://www.riverbankcomputing.com/software/pyqtwebengine/.
 
 Support may be obtained from the PyQt mailing list at
 https://www.riverbankcomputing.com/mailman/listinfo/pyqt/.
 
 
-License
--------
+## License
 
 PyQt6-WebEngine is released under the GPL v3 license and under a commercial
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
 
-The GPL version of PyQt6-WebEngine can be installed from PyPI::
+The GPL version of PyQt6-WebEngine can be installed from PyPI:
 
     pip install PyQt6-WebEngine
 
-``pip`` will also build and install the bindings from the sdist package but
-Qt's ``qmake`` tool must be on ``PATH``.
+`pip` will also build and install the bindings from the sdist package but Qt's
+`qmake` tool must be on `PATH`.
 
-The ``sip-install`` tool will also install the bindings from the sdist package
+The `sip-install` tool will also install the bindings from the sdist package
 but will allow you to configure many aspects of the installation.
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/QtWebEngineCoremod.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/QtWebEngineCoremod.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtWebEngineCoremod.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -23,18 +23,18 @@
 %Module(name=PyQt6.QtWebEngineCore, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtCore/QtCoremod.sip
 %Import QtGui/QtGuimod.sip
 %Import QtNetwork/QtNetworkmod.sip
 %Import QtWebChannel/QtWebChannelmod.sip
 
-%Timeline {QtWebEngine_6_0_0 QtWebEngine_6_1_0 QtWebEngine_6_2_0 QtWebEngine_6_3_0 QtWebEngine_6_4_0 QtWebEngine_6_5_0 QtWebEngine_6_6_0}
+%Timeline {QtWebEngine_6_0_0 QtWebEngine_6_1_0 QtWebEngine_6_2_0 QtWebEngine_6_3_0 QtWebEngine_6_4_0 QtWebEngine_6_5_0 QtWebEngine_6_6_0 QtWebEngine_6_7_0}
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-WebEngine.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
@@ -50,24 +50,25 @@
 
 %DefaultSupertype PyQt6.sip.simplewrapper
 
 int PYQT_WEBENGINE_VERSION;
 const char *PYQT_WEBENGINE_VERSION_STR;
 
 %ModuleCode
-static int PYQT_WEBENGINE_VERSION = 0x060600;
-static const char *PYQT_WEBENGINE_VERSION_STR = "6.6.0";
+static int PYQT_WEBENGINE_VERSION = 0x060700;
+static const char *PYQT_WEBENGINE_VERSION_STR = "6.7.0";
 %End
 
 %Include qtwebenginecoreglobal.sip
 %Include qwebenginecertificateerror.sip
 %Include qwebengineclientcertificateselection.sip
 %Include qwebengineclientcertificatestore.sip
 %Include qwebenginecontextmenurequest.sip
 %Include qwebenginecookiestore.sip
+%Include qwebenginedesktopmediarequest.sip
 %Include qwebenginedownloadrequest.sip
 %Include qwebenginefilesystemaccessrequest.sip
 %Include qwebenginefindtextresult.sip
 %Include qwebenginefullscreenrequest.sip
 %Include qwebengineglobalsettings.sip
 %Include qwebenginehistory.sip
 %Include qwebenginehttprequest.sip
@@ -83,7 +84,8 @@
 %Include qwebenginescriptcollection.sip
 %Include qwebenginesettings.sip
 %Include qwebengineurlrequestinfo.sip
 %Include qwebengineurlrequestinterceptor.sip
 %Include qwebengineurlrequestjob.sip
 %Include qwebengineurlscheme.sip
 %Include qwebengineurlschemehandler.sip
+%Include qwebenginewebauthuxrequest.sip
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qtwebenginecoreglobal.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qtwebenginecoreglobal.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtwebenginecoreglobal.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginecertificateerror.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginecertificateerror.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginecertificateerror.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineclientcertificateselection.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineclientcertificateselection.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineclientcertificateselection.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineclientcertificatestore.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineclientcertificatestore.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineclientcertificatestore.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginecontextmenurequest.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginecontextmenurequest.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginecontextmenurequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEngineContextMenuRequest : QObject /NoDefaultCtors/
+class QWebEngineContextMenuRequest : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qwebenginecontextmenurequest.h>
 %End
 
 public:
     enum MediaType
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginedownloadrequest.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginedownloadrequest.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginedownloadrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEngineDownloadRequest : QObject /NoDefaultCtors/
+class QWebEngineDownloadRequest : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qwebenginedownloadrequest.h>
 %End
 
 public:
     virtual ~QWebEngineDownloadRequest();
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginefilesystemaccessrequest.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginefilesystemaccessrequest.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginefilesystemaccessrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginefindtextresult.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginefindtextresult.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginefindtextresult.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginefullscreenrequest.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginefullscreenrequest.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginefullscreenrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineglobalsettings.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineglobalsettings.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineglobalsettings.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginehistory.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginehistory.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginehistory.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -37,15 +37,15 @@
     bool isValid() const;
     void swap(QWebEngineHistoryItem &other /Constrained/);
 };
 
 QDataStream &operator<<(QDataStream &, const QWebEngineHistory &) /ReleaseGIL/;
 QDataStream &operator>>(QDataStream &, QWebEngineHistory & /Constrained/) /ReleaseGIL/;
 
-class QWebEngineHistoryModel : QAbstractListModel /NoDefaultCtors/
+class QWebEngineHistoryModel : public QAbstractListModel /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qwebenginehistory.h>
 %End
 
 public:
     enum Roles
@@ -61,15 +61,15 @@
     virtual QHash<int, QByteArray> roleNames() const;
     void reset();
 
 private:
     virtual ~QWebEngineHistoryModel();
 };
 
-class QWebEngineHistory : QObject /NoDefaultCtors/
+class QWebEngineHistory : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qwebenginehistory.h>
 %End
 
 public:
     void clear();
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginehttprequest.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginehttprequest.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginehttprequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineloadinginfo.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineloadinginfo.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineloadinginfo.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginenavigationrequest.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginenavigationrequest.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginenavigationrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEngineNavigationRequest : QObject
+class QWebEngineNavigationRequest : public QObject
 {
 %TypeHeaderCode
 #include <qwebenginenavigationrequest.h>
 %End
 
 public:
     enum NavigationType
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginenewwindowrequest.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginenewwindowrequest.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginenewwindowrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEngineNewWindowRequest : QObject /NoDefaultCtors/
+class QWebEngineNewWindowRequest : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qwebenginenewwindowrequest.h>
 %End
 
 public:
     enum DestinationType
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginenotification.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginenotification.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginenotification.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEngineNotification : QObject /NoDefaultCtors/
+class QWebEngineNotification : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qwebenginenotification.h>
 %End
 
 public:
     virtual ~QWebEngineNotification();
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginepage.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginepage.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginepage.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEnginePage : QObject
+class QWebEnginePage : public QObject
 {
 %TypeHeaderCode
 #include <qwebenginepage.h>
 %End
 
 public:
     enum WebAction
@@ -463,8 +463,16 @@
     void fileSystemAccessRequested(QWebEngineFileSystemAccessRequest request);
 %End
 
 public:
 %If (QtWebEngine_6_6_0 -)
     QString devToolsId() const;
 %End
+
+signals:
+%If (QtWebEngine_6_7_0 -)
+    void desktopMediaRequested(const QWebEngineDesktopMediaRequest &request);
+%End
+%If (QtWebEngine_6_7_0 -)
+    void webAuthUxRequested(QWebEngineWebAuthUxRequest *request);
+%End
 };
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineprofile.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineprofile.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineprofile.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEngineProfile : QObject
+class QWebEngineProfile : public QObject
 {
 %TypeHeaderCode
 #include <qwebengineprofile.h>
 %End
 
 %TypeCode
 // Needed by handwritten code.
@@ -46,15 +46,20 @@
         {sipName_QWebEngineNavigationRequest, &sipType_QWebEngineNavigationRequest, -1, 6},
         {sipName_QWebEngineNewWindowRequest, &sipType_QWebEngineNewWindowRequest, -1, 7},
         {sipName_QWebEngineNotification, &sipType_QWebEngineNotification, -1, 8},
         {sipName_QWebEnginePage, &sipType_QWebEnginePage, -1, 9},
         {sipName_QWebEngineProfile, &sipType_QWebEngineProfile, -1, 10},
         {sipName_QWebEngineUrlRequestInterceptor, &sipType_QWebEngineUrlRequestInterceptor, -1, 11},
         {sipName_QWebEngineUrlRequestJob, &sipType_QWebEngineUrlRequestJob, -1, 12},
-        {sipName_QWebEngineUrlSchemeHandler, &sipType_QWebEngineUrlSchemeHandler, -1, -1},
+        {sipName_QWebEngineUrlSchemeHandler, &sipType_QWebEngineUrlSchemeHandler, -1, 13},
+    #if QT_VERSION >= 0x060700
+        {sipName_QWebEngineWebAuthUxRequest, &sipType_QWebEngineWebAuthUxRequest, -1, -1},
+    #else
+        {0, 0, -1, -1},
+    #endif
     };
     
     int i = 0;
     
     sipType = NULL;
     
     do
@@ -110,14 +115,17 @@
     bool visitedLinksContainsUrl(const QUrl &url) const;
     QWebEngineSettings *settings() const;
     QWebEngineScriptCollection *scripts() const;
     static QWebEngineProfile *defaultProfile() /Transfer/;
 
 signals:
     void downloadRequested(QWebEngineDownloadRequest *download);
+%If (QtWebEngine_6_7_0 -)
+    void clearHttpCacheCompleted();
+%End
 
 public:
     void setHttpAcceptLanguage(const QString &httpAcceptLanguage);
     QString httpAcceptLanguage() const;
     QWebEngineCookieStore *cookieStore() /Transfer/;
     void setUrlRequestInterceptor(QWebEngineUrlRequestInterceptor *interceptor);
     const QWebEngineUrlSchemeHandler *urlSchemeHandler(const QByteArray &) const;
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginequotarequest.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginequotarequest.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginequotarequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineregisterprotocolhandlerrequest.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineregisterprotocolhandlerrequest.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineregisterprotocolhandlerrequest.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginescript.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginescript.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginescript.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginescriptcollection.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginescriptcollection.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginescriptcollection.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebenginesettings.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebenginesettings.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebenginesettings.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -73,14 +73,17 @@
         PdfViewerEnabled,
 %If (QtWebEngine_6_4_0 -)
         NavigateOnDropEnabled,
 %End
 %If (QtWebEngine_6_6_0 -)
         ReadingFromCanvasEnabled,
 %End
+%If (QtWebEngine_6_7_0 -)
+        ForceDarkMode,
+%End
     };
 
     enum FontSize
     {
         MinimumFontSize,
         MinimumLogicalFontSize,
         DefaultFontSize,
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineurlrequestinfo.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineurlrequestinfo.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineurlrequestinfo.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -74,12 +74,15 @@
     void block(bool shouldBlock);
     void redirect(const QUrl &url);
     void setHttpHeader(const QByteArray &name, const QByteArray &value);
     QUrl initiator() const;
 %If (QtWebEngine_6_5_0 -)
     QHash<QByteArray, QByteArray> httpHeaders() const;
 %End
+%If (QtWebEngine_6_7_0 -)
+    QIODevice *requestBody() const;
+%End
 
 private:
     QWebEngineUrlRequestInfo();
     ~QWebEngineUrlRequestInfo();
 };
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineurlrequestinterceptor.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineurlrequestinterceptor.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineurlrequestinterceptor.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEngineUrlRequestInterceptor : QObject
+class QWebEngineUrlRequestInterceptor : public QObject
 {
 %TypeHeaderCode
 #include <qwebengineurlrequestinterceptor.h>
 %End
 
 public:
     explicit QWebEngineUrlRequestInterceptor(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineurlrequestjob.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineurlrequestjob.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineurlrequestjob.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEngineUrlRequestJob : QObject /NoDefaultCtors/
+class QWebEngineUrlRequestJob : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qwebengineurlrequestjob.h>
 %End
 
 public:
     virtual ~QWebEngineUrlRequestJob();
@@ -45,8 +45,11 @@
     void fail(QWebEngineUrlRequestJob::Error error);
     void redirect(const QUrl &url);
     QUrl initiator() const;
     QMap<QByteArray, QByteArray> requestHeaders() const;
 %If (QtWebEngine_6_6_0 -)
     void setAdditionalResponseHeaders(const QMultiMap<QByteArray, QByteArray> &additionalResponseHeaders) const;
 %End
+%If (QtWebEngine_6_7_0 -)
+    QIODevice *requestBody() const;
+%End
 };
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineurlscheme.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineurlscheme.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineurlscheme.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineCore/qwebengineurlschemehandler.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineCore/qwebengineurlschemehandler.sip`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineurlschemehandler.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEngineUrlSchemeHandler : QObject
+class QWebEngineUrlSchemeHandler : public QObject
 {
 %TypeHeaderCode
 #include <qwebengineurlschemehandler.h>
 %End
 
 public:
     QWebEngineUrlSchemeHandler(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineQuick/QtWebEngineQuickmod.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineQuick/QtWebEngineQuickmod.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtWebEngineQuickmod.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineQuick Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 %Module(name=PyQt6.QtWebEngineQuick, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtQml/QtQmlmod.sip
 %Import QtWebEngineCore/QtWebEngineCoremod.sip
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-WebEngine.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineQuick/qquickwebengineprofile.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineQuick/qquickwebengineprofile.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qquickwebengineprofile.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineQuick Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QQuickWebEngineProfile : QObject
+class QQuickWebEngineProfile : public QObject
 {
 %TypeHeaderCode
 #include <qquickwebengineprofile.h>
 %End
 
 %ConvertToSubClassCode
     static struct class_graph {
@@ -140,8 +140,11 @@
     void setPushServiceEnabled(bool enable);
 %End
 
 signals:
 %If (QtWebEngine_6_5_0 -)
     void pushServiceEnabledChanged();
 %End
+%If (QtWebEngine_6_7_0 -)
+    void clearHttpCacheCompleted();
+%End
 };
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineQuick/qtwebenginequickglobal.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineQuick/qtwebenginequickglobal.sip`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtwebenginequickglobal.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineQuick Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineWidgets/QtWebEngineWidgetsmod.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineWidgets/QtWebEngineWidgetsmod.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtWebEngineWidgetsmod.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineWidgets Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -25,15 +25,15 @@
 %Import QtCore/QtCoremod.sip
 %Import QtNetwork/QtNetworkmod.sip
 %Import QtPrintSupport/QtPrintSupportmod.sip
 %Import QtWebEngineCore/QtWebEngineCoremod.sip
 %Import QtWidgets/QtWidgetsmod.sip
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-WebEngine.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_WebEngine-6.6.0/sip/QtWebEngineWidgets/qwebengineview.sip` & `PyQt6_WebEngine-6.7.0/sip/QtWebEngineWidgets/qwebengineview.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qwebengineview.sip generated by MetaSIP
 //
 // This file is part of the QtWebEngineWidgets Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-WebEngine.
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
 
 
-class QWebEngineView : QWidget
+class QWebEngineView : public QWidget
 {
 %TypeHeaderCode
 #include <qwebengineview.h>
 %End
 
 %TypeCode
 // For QWebEngineView.findText().
```

