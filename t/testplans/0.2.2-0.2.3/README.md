# Comparing `tmp/testplans-0.2.2.tar.gz` & `tmp/testplans-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testplans-0.2.2.tar", last modified: Wed Apr 24 09:56:02 2024, max compression
+gzip compressed data, was "testplans-0.2.3.tar", last modified: Fri Apr 26 12:21:18 2024, max compression
```

## Comparing `testplans-0.2.2.tar` & `testplans-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 09:56:02.925351 testplans-0.2.2/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     5494 2024-04-24 09:56:02.925210 testplans-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4584 2024-04-22 15:10:50.000000 testplans-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 09:56:02.925702 testplans-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:56:02.917649 testplans-0.2.2/testplans/
--rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.2/testplans/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.2/testplans/_results.py
--rw-rw-rw-   0        0        0     3845 2024-04-22 15:01:51.000000 testplans-0.2.2/testplans/api.py
--rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.2/testplans/devices.py
--rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.2/testplans/gui.py
--rw-rw-rw-   0        0        0    10511 2024-04-22 15:01:51.000000 testplans-0.2.2/testplans/main.py
--rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.2/testplans/models.py
--rw-rw-rw-   0        0        0    10986 2024-04-24 09:53:50.000000 testplans-0.2.2/testplans/tc.py
--rw-rw-rw-   0        0        0     8911 2024-03-29 14:14:49.000000 testplans-0.2.2/testplans/tm.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:56:02.923679 testplans-0.2.2/testplans.egg-info/
--rw-rw-rw-   0        0        0     5494 2024-04-24 09:56:02.000000 testplans-0.2.2/testplans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-04-24 09:56:02.000000 testplans-0.2.2/testplans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 09:56:02.000000 testplans-0.2.2/testplans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-24 09:56:02.000000 testplans-0.2.2/testplans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 12:21:18.909757 testplans-0.2.3/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     5494 2024-04-26 12:21:18.909757 testplans-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4584 2024-04-26 12:20:33.000000 testplans-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 12:21:18.911266 testplans-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:21:18.900800 testplans-0.2.3/testplans/
+-rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.3/testplans/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.3/testplans/_results.py
+-rw-rw-rw-   0        0        0     3845 2024-04-22 15:01:51.000000 testplans-0.2.3/testplans/api.py
+-rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.3/testplans/devices.py
+-rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.3/testplans/gui.py
+-rw-rw-rw-   0        0        0    10511 2024-04-22 15:01:51.000000 testplans-0.2.3/testplans/main.py
+-rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.3/testplans/models.py
+-rw-rw-rw-   0        0        0    10986 2024-04-24 09:53:50.000000 testplans-0.2.3/testplans/tc.py
+-rw-rw-rw-   0        0        0     8975 2024-04-26 12:19:02.000000 testplans-0.2.3/testplans/tm.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:21:18.908499 testplans-0.2.3/testplans.egg-info/
+-rw-rw-rw-   0        0        0     5494 2024-04-26 12:21:18.000000 testplans-0.2.3/testplans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-04-26 12:21:18.000000 testplans-0.2.3/testplans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 12:21:18.000000 testplans-0.2.3/testplans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-26 12:21:18.000000 testplans-0.2.3/testplans.egg-info/top_level.txt
```

### Comparing `testplans-0.2.2/LICENSE` & `testplans-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `testplans-0.2.2/PKG-INFO` & `testplans-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.2
+Version: 0.2.3
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.2.1)
+# testplans (v0.2.3)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.2/README.md` & `testplans-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# testplans (v0.2.1)
+# testplans (v0.2.3)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.2/setup.py` & `testplans-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.2/testplans/_results.py` & `testplans-0.2.3/testplans/_results.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.2/testplans/api.py` & `testplans-0.2.3/testplans/api.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.2/testplans/devices.py` & `testplans-0.2.3/testplans/devices.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.2/testplans/gui.py` & `testplans-0.2.3/testplans/gui.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.2/testplans/main.py` & `testplans-0.2.3/testplans/main.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.2/testplans/models.py` & `testplans-0.2.3/testplans/models.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.2/testplans/tc.py` & `testplans-0.2.3/testplans/tc.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.2/testplans/tm.py` & `testplans-0.2.3/testplans/tm.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,33 @@
 from pyqt_templates import TableModelTemplate
 from funcs_aux import NamesIndexed_Base, NamesIndexed_Templated
 
 # from .tp import TpMultyDutBase
 
 
 # =====================================================================================================================
-class Headers(NamesIndexed_Base):
-    TESTCASE = 0
-    ASYNC = 1
-    STARTUP = 2
-    DUTS = NamesIndexed_Templated(3, 10)
-    # FIXME: need resolve COUNT over DevicesIndexed!!!
-
-
-# =====================================================================================================================
 class TpTableModel(TableModelTemplate):
     DATA: "TpMultyDutBase"
-    HEADERS: Headers = Headers()
+    HEADERS: "Headers"
 
     # AUX -------------------------------------------
     open__settings: Optional[bool] = None
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        class Headers(NamesIndexed_Base):
+            TESTCASE = 0
+            ASYNC = 1
+            STARTUP = 2
+            DUTS = NamesIndexed_Templated(3, self.DATA.DEVICES__CLS.COUNT)
+            # FIXME: need resolve COUNT over DevicesIndexed!!!
+
+        self.HEADERS = Headers()
+
     def rowCount(self, parent: QModelIndex = None, *args, **kwargs) -> int:
         return len(self.DATA.TCS__CLS)
 
     def columnCount(self, parent: QModelIndex = None, *args, **kwargs) -> int:
         return self.HEADERS.count()
 
     # def headerData(self, section: Any, orientation: Qt.Orientation, role: int = Qt.DisplayRole) -> str:
```

### Comparing `testplans-0.2.2/testplans.egg-info/PKG-INFO` & `testplans-0.2.3/testplans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.2
+Version: 0.2.3
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.2.1)
+# testplans (v0.2.3)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

