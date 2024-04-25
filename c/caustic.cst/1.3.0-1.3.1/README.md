# Comparing `tmp/caustic.cst-1.3.0.tar.gz` & `tmp/caustic.cst-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.cst-1.3.0.tar", last modified: Wed Apr 24 18:47:22 2024, max compression
+gzip compressed data, was "caustic.cst-1.3.1.tar", last modified: Wed Apr 24 23:12:20 2024, max compression
```

## Comparing `caustic.cst-1.3.0.tar` & `caustic.cst-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 18:47:22.120438 caustic.cst-1.3.0/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.cst-1.3.0/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     3751 2024-04-24 18:47:22.117105 caustic.cst-1.3.0/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)     2871 2024-04-24 18:11:57.000000 caustic.cst-1.3.0/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)      962 2024-04-24 18:11:29.000000 caustic.cst-1.3.0/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-24 18:47:22.120438 caustic.cst-1.3.0/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 18:47:22.110438 caustic.cst-1.3.0/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 18:47:22.110438 caustic.cst-1.3.0/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 18:47:22.117105 caustic.cst-1.3.0/src/caustic/cst/
--rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-24 18:12:28.000000 caustic.cst-1.3.0/src/caustic/cst/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1248 2024-04-24 01:42:12.000000 caustic.cst-1.3.0/src/caustic/cst/atom.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1664 2024-04-24 18:14:27.000000 caustic.cst-1.3.0/src/caustic/cst/bases.py
--rw-r--r--   0 shae      (1000) shae      (1000)      485 2024-04-24 01:40:40.000000 caustic.cst-1.3.0/src/caustic/cst/block.py
--rw-r--r--   0 shae      (1000) shae      (1000)     4127 2024-04-24 02:01:35.000000 caustic.cst-1.3.0/src/caustic/cst/expression.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 18:47:22.117105 caustic.cst-1.3.0/src/caustic/cst/mods/
--rw-r--r--   0 shae      (1000) shae      (1000)      946 2024-04-24 16:44:17.000000 caustic.cst-1.3.0/src/caustic/cst/mods/m_exception.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1522 2024-04-24 18:46:52.000000 caustic.cst-1.3.0/src/caustic/cst/serialize.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1870 2024-04-24 16:51:20.000000 caustic.cst-1.3.0/src/caustic/cst/statement.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 18:47:22.117105 caustic.cst-1.3.0/src/caustic.cst.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     3751 2024-04-24 18:47:22.000000 caustic.cst-1.3.0/src/caustic.cst.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      414 2024-04-24 18:47:22.000000 caustic.cst-1.3.0/src/caustic.cst.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-24 18:47:22.000000 caustic.cst-1.3.0/src/caustic.cst.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-24 18:47:22.000000 caustic.cst-1.3.0/src/caustic.cst.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 23:12:20.173923 caustic.cst-1.3.1/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.cst-1.3.1/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     3792 2024-04-24 23:12:20.173923 caustic.cst-1.3.1/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     2912 2024-04-24 23:11:54.000000 caustic.cst-1.3.1/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)      962 2024-04-24 23:12:00.000000 caustic.cst-1.3.1/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-24 23:12:20.173923 caustic.cst-1.3.1/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 23:12:20.163923 caustic.cst-1.3.1/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 23:12:20.163923 caustic.cst-1.3.1/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 23:12:20.170589 caustic.cst-1.3.1/src/caustic/cst/
+-rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-24 18:12:28.000000 caustic.cst-1.3.1/src/caustic/cst/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1248 2024-04-24 01:42:12.000000 caustic.cst-1.3.1/src/caustic/cst/atom.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1664 2024-04-24 18:14:27.000000 caustic.cst-1.3.1/src/caustic/cst/bases.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      485 2024-04-24 01:40:40.000000 caustic.cst-1.3.1/src/caustic/cst/block.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     4240 2024-04-24 23:11:22.000000 caustic.cst-1.3.1/src/caustic/cst/expression.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 23:12:20.170589 caustic.cst-1.3.1/src/caustic/cst/mods/
+-rw-r--r--   0 shae      (1000) shae      (1000)      946 2024-04-24 16:44:17.000000 caustic.cst-1.3.1/src/caustic/cst/mods/m_exception.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1522 2024-04-24 18:46:52.000000 caustic.cst-1.3.1/src/caustic/cst/serialize.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1870 2024-04-24 16:51:20.000000 caustic.cst-1.3.1/src/caustic/cst/statement.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 23:12:20.170589 caustic.cst-1.3.1/src/caustic.cst.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     3792 2024-04-24 23:12:20.000000 caustic.cst-1.3.1/src/caustic.cst.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      414 2024-04-24 23:12:20.000000 caustic.cst-1.3.1/src/caustic.cst.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-24 23:12:20.000000 caustic.cst-1.3.1/src/caustic.cst.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-24 23:12:20.000000 caustic.cst-1.3.1/src/caustic.cst.egg-info/top_level.txt
```

### Comparing `caustic.cst-1.3.0/LICENSE` & `caustic.cst-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.3.0/PKG-INFO` & `caustic.cst-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.cst
-Version: 1.3.0
+Version: 1.3.1
 Summary: Caustic's Abstract Syntax Tree, or CST
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticAST
 Project-URL: Issues, https://codeberg.org/Caustic/CausticAST/issues
 Keywords: caustic,language,parser,ast,syntax,tree
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -55,14 +55,15 @@
  │   │   │   ├─ expression.AssignExpr
  │   │   │   ├─ expression.Add
  │   │   │   ├─ expression.Sub
  │   │   │   ├─ expression.Mult
  │   │   │   ├─ expression.Div
  │   │   │   ├─ expression.Mod
  │   │   │   ├─ expression.MMul
+ │   │   │   ├─ expression.Pow
  │   │   │   ├─ expression.Equality [EQ]
  │   │   │   ├─ expression.Inequality [NE]
  │   │   │   ├─ expression.LessThan [LT]
  │   │   │   ├─ expression.GreaterThan [GT]
  │   │   │   ├─ expression.LessThanOrEquality [LE]
  │   │   │   ├─ expression.GreaterThanOrEquality [GE]
  │   │   │   ├─ expression.Nullish
```

### Comparing `caustic.cst-1.3.0/README.md` & `caustic.cst-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
  │   │   │   ├─ expression.AssignExpr
  │   │   │   ├─ expression.Add
  │   │   │   ├─ expression.Sub
  │   │   │   ├─ expression.Mult
  │   │   │   ├─ expression.Div
  │   │   │   ├─ expression.Mod
  │   │   │   ├─ expression.MMul
+ │   │   │   ├─ expression.Pow
  │   │   │   ├─ expression.Equality [EQ]
  │   │   │   ├─ expression.Inequality [NE]
  │   │   │   ├─ expression.LessThan [LT]
  │   │   │   ├─ expression.GreaterThan [GT]
  │   │   │   ├─ expression.LessThanOrEquality [LE]
  │   │   │   ├─ expression.GreaterThanOrEquality [GE]
  │   │   │   ├─ expression.Nullish
```

### Comparing `caustic.cst-1.3.0/pyproject.toml` & `caustic.cst-1.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.cst"
-version = "1.3.0"
+version = "1.3.1"
 dependencies = []
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's Abstract Syntax Tree, or CST"
 readme = "README.md"
 keywords = ['caustic', 'language', 'parser', 'ast', 'syntax', 'tree']
```

### Comparing `caustic.cst-1.3.0/src/caustic/cst/atom.py` & `caustic.cst-1.3.1/src/caustic/cst/atom.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.3.0/src/caustic/cst/bases.py` & `caustic.cst-1.3.1/src/caustic/cst/bases.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.3.0/src/caustic/cst/expression.py` & `caustic.cst-1.3.1/src/caustic/cst/expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 #> Header >/
 __all__ = (# Unary
            'UPlus', 'UMinus', 'Increment', 'Decrement', 'BitInvert', 'LogNot',
            # Binary
            'AssignExpr',
            ## Arithmetic
-           'Add', 'Sub', 'Mult', 'Div', 'Mod', 'MMul',
+           'Add', 'Sub', 'Mult', 'Div', 'Mod', 'MMul', 'Pow',
            ## Comparison
            'Equality', 'Inequality', 'LessThan', 'GreaterThan', 'LessThanOrEquality', 'GreaterThanOrEquality', 'Nullish',
            ### Aliases
            'EQ', 'NE', 'LT', 'GT', 'LE', 'GE',
            ## Logical
            'LogAnd', 'LogOr', 'LogXor',
            ## Bitwise
@@ -66,14 +66,17 @@
     __slots__ = ()
 class Mod(BaseBinaryOperator):
     '''Represents a modulus operator'''
     __slots__ = ()
 class MMul(BaseBinaryOperator):
     '''Represents a matrix-multiplication operator'''
     __slots__ = ()
+class Pow(BaseBinaryOperator):
+    '''Represents a power (exponentiation) operation'''
+    __slots__ = ()
 ## Comparison
 class Equality(BaseBinaryOperator):
     '''Represents an equality comparison operator'''
     __slots__ = ()
 EQ = Equality
 class Inequality(BaseBinaryOperator):
     '''Represents an inequality comparison operator'''
```

### Comparing `caustic.cst-1.3.0/src/caustic/cst/mods/m_exception.py` & `caustic.cst-1.3.1/src/caustic/cst/mods/m_exception.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.3.0/src/caustic/cst/serialize.py` & `caustic.cst-1.3.1/src/caustic/cst/serialize.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.3.0/src/caustic/cst/statement.py` & `caustic.cst-1.3.1/src/caustic/cst/statement.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.3.0/src/caustic.cst.egg-info/PKG-INFO` & `caustic.cst-1.3.1/src/caustic.cst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.cst
-Version: 1.3.0
+Version: 1.3.1
 Summary: Caustic's Abstract Syntax Tree, or CST
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticAST
 Project-URL: Issues, https://codeberg.org/Caustic/CausticAST/issues
 Keywords: caustic,language,parser,ast,syntax,tree
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -55,14 +55,15 @@
  │   │   │   ├─ expression.AssignExpr
  │   │   │   ├─ expression.Add
  │   │   │   ├─ expression.Sub
  │   │   │   ├─ expression.Mult
  │   │   │   ├─ expression.Div
  │   │   │   ├─ expression.Mod
  │   │   │   ├─ expression.MMul
+ │   │   │   ├─ expression.Pow
  │   │   │   ├─ expression.Equality [EQ]
  │   │   │   ├─ expression.Inequality [NE]
  │   │   │   ├─ expression.LessThan [LT]
  │   │   │   ├─ expression.GreaterThan [GT]
  │   │   │   ├─ expression.LessThanOrEquality [LE]
  │   │   │   ├─ expression.GreaterThanOrEquality [GE]
  │   │   │   ├─ expression.Nullish
```

