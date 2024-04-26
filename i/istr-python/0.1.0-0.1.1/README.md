# Comparing `tmp/istr_python-0.1.0.tar.gz` & `tmp/istr_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.1.0.tar", last modified: Wed Apr 24 16:01:57 2024, max compression
+gzip compressed data, was "istr_python-0.1.1.tar", last modified: Fri Apr 26 12:45:20 2024, max compression
```

## Comparing `istr_python-0.1.0.tar` & `istr_python-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 16:01:57.723514 istr_python-0.1.0/
--rw-rw-rw-   0        0        0    10346 2024-04-24 16:01:57.720511 istr_python-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9419 2024-04-24 14:54:22.000000 istr_python-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 16:01:57.666693 istr_python-0.1.0/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.0/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.0/istr/install istr.py
--rw-rw-rw-   0        0        0    15553 2024-04-24 12:19:57.000000 istr_python-0.1.0/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:01:57.713932 istr_python-0.1.0/istr_python.egg-info/
--rw-rw-rw-   0        0        0    10346 2024-04-24 16:01:57.000000 istr_python-0.1.0/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-24 16:01:57.000000 istr_python-0.1.0/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 16:01:57.000000 istr_python-0.1.0/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-24 16:01:57.000000 istr_python-0.1.0/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      744 2024-04-24 16:01:50.000000 istr_python-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-24 16:01:57.724954 istr_python-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-24 16:01:57.706870 istr_python-0.1.0/tests/
--rw-rw-rw-   0        0        0    11213 2024-04-23 14:50:53.000000 istr_python-0.1.0/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:45:20.410875 istr_python-0.1.1/
+-rw-rw-rw-   0        0        0    10334 2024-04-26 12:45:20.408875 istr_python-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9420 2024-04-26 11:01:42.000000 istr_python-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 12:45:20.376413 istr_python-0.1.1/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.1/istr/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.1/istr/install istr.py
+-rw-rw-rw-   0        0        0    15477 2024-04-26 12:43:24.000000 istr_python-0.1.1/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:45:20.406571 istr_python-0.1.1/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    10334 2024-04-26 12:45:20.000000 istr_python-0.1.1/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-26 12:45:20.000000 istr_python-0.1.1/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 12:45:20.000000 istr_python-0.1.1/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 12:45:20.000000 istr_python-0.1.1/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      616 2024-04-26 12:45:13.000000 istr_python-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 12:45:20.411875 istr_python-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 12:45:20.403564 istr_python-0.1.1/tests/
+-rw-rw-rw-   0        0        0    11418 2024-04-25 11:05:24.000000 istr_python-0.1.1/tests/test_istr.py
```

### Comparing `istr_python-0.1.0/PKG-INFO` & `istr_python-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.0
-Summary: istr is a module to use strings as if they were integers.
+Version: 0.1.1
+Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-<img src="https://www.salabim.org/istr.png" width=500>
+<img src="https://www.salabim.org/istr1.png" width=500>
 
 # Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
```

### Comparing `istr_python-0.1.0/README.md` & `istr_python-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="https://www.salabim.org/istr.png" width=500>
+<img src="https://www.salabim.org/istr1.png" width=500>
 
 # Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
```

### Comparing `istr_python-0.1.0/istr/install istr.py` & `istr_python-0.1.1/istr/install istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.1.0/istr/istr.py` & `istr_python-0.1.1/istr/istr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import functools
 import math
 
+#     _       _
+#    (_) ___ | |_  _ __
+#    | |/ __|| __|| '__|
+#    | |\__ \| |_ | |
+#    |_||___/ \__||_|
+# strings you can count on
 
-#   _       _
-#  (_) ___ | |_  _ __
-#  | |/ __|| __|| '__|
-#  | |\__ \| |_ | |
-#  |_||___/ \__||_|    use strings as integers
-
-__version__ = "0.1.0"
+__version__ = "0.1.1"
+import functools
+import math
 
 """
 changelog
 
 version 0.1.0  2024-04-22  
 -------------------------
 Changed the way istr.range is implemenented.
@@ -252,15 +254,15 @@
                 return map(functools.partial(cls), value)
             return type(value)(map(functools.partial(cls), value))
         if value == "":
             as_str = ""
             as_int = 0
         else:
             as_int = cls._to_int(value)
-            if cls._format == "" or cls._base != 10:
+            if (cls._format == "" or cls._base != 10) and not isinstance(value,istr):
                 if isinstance(value, str):
                     as_str = value
                 else:
                     if cls._base == 10:
                         as_str = str(as_int)
                     else:
                         as_str = istr._to_base(as_int, cls._base)
@@ -487,23 +489,17 @@
     @classmethod
     def range(cls, start,stop=None,step=1):
         return _range(cls,start,stop,step) 
 
 
 
 def main():
-    print(repr(istr("  12")))
     with istr.base(16):
-        print(repr(istr("  12")))
-
-
-    with istr.format("05"):
-        print(repr(istr("  12")))
-        print(repr(istr(12)))
-        with istr.base(16):
-            print(repr(istr("   12")))
-
+        a = istr(15)
+    b = a * a
+    print(b)
+    c=istr(a)
+    print(repr(c))
 
 
 if __name__ == "__main__":
-    main()
-
+    main()
```

### Comparing `istr_python-0.1.0/istr_python.egg-info/PKG-INFO` & `istr_python-0.1.1/istr_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.0
-Summary: istr is a module to use strings as if they were integers.
+Version: 0.1.1
+Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-<img src="https://www.salabim.org/istr.png" width=500>
+<img src="https://www.salabim.org/istr1.png" width=500>
 
 # Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
```

### Comparing `istr_python-0.1.0/tests/test_istr.py` & `istr_python-0.1.1/tests/test_istr.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,14 +435,24 @@
     with pytest.raises(ValueError):
         istr.base(37)
 
     with pytest.raises(ValueError):
         with istr.base(16):
             istr(-1)
 
+    with istr.base(16):
+        a = istr(15)
+    with istr.base(10):
+        assert a * a == 225
+    with pytest.raises(ValueError):
+        assert a | a # FF can't be converted to base 10
+        
+    
+
+
 
 def test_subclassing():
     class jstr(istr):
         ...
 
     assert jstr(5).equals(jstr(5))
     assert repr(jstr(*range(3))) == "(jstr('0'), jstr('1'), jstr('2'))"
```

