# Comparing `tmp/george_walrus-0.1.5.tar.gz` & `tmp/george-walrus-0.1.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "george_walrus-0.1.5.tar", last modified: Fri Apr 26 08:59:22 2024, max compression
+gzip compressed data, was "george-walrus-0.1.5rc1.tar", last modified: Sat Jan  7 05:36:05 2023, max compression
```

## Comparing `george_walrus-0.1.5.tar` & `george-walrus-0.1.5rc1.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxr-x   0 george    (1007) george    (1007)        0 2024-04-26 08:59:22.721360 george_walrus-0.1.5/
--rw-rw-r--   0 george    (1007) george    (1007)     1099 2024-04-25 07:46:16.000000 george_walrus-0.1.5/LICENSE
--rw-rw-r--   0 george    (1007) george    (1007)       32 2024-04-25 07:46:16.000000 george_walrus-0.1.5/MANIFEST.in
--rw-r--r--   0 george    (1007) george    (1007)     4238 2024-04-26 08:59:22.721360 george_walrus-0.1.5/PKG-INFO
--rw-rw-r--   0 george    (1007) george    (1007)     2334 2024-04-26 08:57:05.000000 george_walrus-0.1.5/README.md
-drwxrwxr-x   0 george    (1007) george    (1007)        0 2024-04-26 08:59:22.721360 george_walrus-0.1.5/george_walrus.egg-info/
--rw-r--r--   0 george    (1007) george    (1007)     4238 2024-04-26 08:59:22.000000 george_walrus-0.1.5/george_walrus.egg-info/PKG-INFO
--rw-rw-r--   0 george    (1007) george    (1007)      335 2024-04-26 08:59:22.000000 george_walrus-0.1.5/george_walrus.egg-info/SOURCES.txt
--rw-rw-r--   0 george    (1007) george    (1007)        1 2024-04-26 08:59:22.000000 george_walrus-0.1.5/george_walrus.egg-info/dependency_links.txt
--rw-rw-r--   0 george    (1007) george    (1007)       39 2024-04-26 08:59:22.000000 george_walrus-0.1.5/george_walrus.egg-info/entry_points.txt
--rw-rw-r--   0 george    (1007) george    (1007)      306 2024-04-26 08:59:22.000000 george_walrus-0.1.5/george_walrus.egg-info/requires.txt
--rw-rw-r--   0 george    (1007) george    (1007)        7 2024-04-26 08:59:22.000000 george_walrus-0.1.5/george_walrus.egg-info/top_level.txt
--rw-rw-r--   0 george    (1007) george    (1007)      233 2024-04-25 07:46:16.000000 george_walrus-0.1.5/pyproject.toml
-drwxrwxr-x   0 george    (1007) george    (1007)        0 2024-04-26 08:59:22.721360 george_walrus-0.1.5/scripts/
--rw-rw-r--   0 george    (1007) george    (1007)      497 2024-04-25 07:46:16.000000 george_walrus-0.1.5/scripts/find_version.py
--rw-rw-r--   0 george    (1007) george    (1007)      102 2024-04-26 08:59:22.721360 george_walrus-0.1.5/setup.cfg
--rw-rw-r--   0 george    (1007) george    (1007)     2594 2024-04-26 08:57:05.000000 george_walrus-0.1.5/setup.py
-drwxrwxr-x   0 george    (1007) george    (1007)        0 2024-04-26 08:59:22.721360 george_walrus-0.1.5/tests/
--rw-rw-r--   0 george    (1007) george    (1007)     6723 2024-04-25 07:46:16.000000 george_walrus-0.1.5/tests/test.py
--rw-rw-r--   0 george    (1007) george    (1007)    80510 2024-04-26 08:57:02.000000 george_walrus-0.1.5/walrus.py
+drwxrwxr-x   0 george    (1007) george    (1007)        0 2023-01-07 05:36:05.074579 george-walrus-0.1.5rc1/
+-rw-rw-r--   0 george    (1007) george    (1007)     1099 2023-01-07 03:43:58.000000 george-walrus-0.1.5rc1/LICENSE
+-rw-rw-r--   0 george    (1007) george    (1007)       32 2023-01-07 03:43:58.000000 george-walrus-0.1.5rc1/MANIFEST.in
+-rw-rw-r--   0 george    (1007) george    (1007)     3456 2023-01-07 05:36:05.074579 george-walrus-0.1.5rc1/PKG-INFO
+-rw-rw-r--   0 george    (1007) george    (1007)     2334 2023-01-07 03:53:01.000000 george-walrus-0.1.5rc1/README.md
+drwxrwxr-x   0 george    (1007) george    (1007)        0 2023-01-07 05:36:05.074579 george-walrus-0.1.5rc1/george_walrus.egg-info/
+-rw-rw-r--   0 george    (1007) george    (1007)     3456 2023-01-07 05:36:05.000000 george-walrus-0.1.5rc1/george_walrus.egg-info/PKG-INFO
+-rw-rw-r--   0 george    (1007) george    (1007)      321 2023-01-07 05:36:05.000000 george-walrus-0.1.5rc1/george_walrus.egg-info/SOURCES.txt
+-rw-rw-r--   0 george    (1007) george    (1007)        1 2023-01-07 05:36:05.000000 george-walrus-0.1.5rc1/george_walrus.egg-info/dependency_links.txt
+-rw-rw-r--   0 george    (1007) george    (1007)       39 2023-01-07 05:36:05.000000 george-walrus-0.1.5rc1/george_walrus.egg-info/entry_points.txt
+-rw-rw-r--   0 george    (1007) george    (1007)      302 2023-01-07 05:36:05.000000 george-walrus-0.1.5rc1/george_walrus.egg-info/requires.txt
+-rw-rw-r--   0 george    (1007) george    (1007)        7 2023-01-07 05:36:05.000000 george-walrus-0.1.5rc1/george_walrus.egg-info/top_level.txt
+-rw-rw-r--   0 george    (1007) george    (1007)      233 2023-01-07 03:43:58.000000 george-walrus-0.1.5rc1/pyproject.toml
+drwxrwxr-x   0 george    (1007) george    (1007)        0 2023-01-07 05:36:05.074579 george-walrus-0.1.5rc1/scripts/
+-rw-rw-r--   0 george    (1007) george    (1007)      497 2023-01-07 03:43:58.000000 george-walrus-0.1.5rc1/scripts/find_version.py
+-rw-rw-r--   0 george    (1007) george    (1007)      102 2023-01-07 05:36:05.078579 george-walrus-0.1.5rc1/setup.cfg
+-rw-rw-r--   0 george    (1007) george    (1007)     2594 2023-01-07 05:35:57.000000 george-walrus-0.1.5rc1/setup.py
+-rw-rw-r--   0 george    (1007) george    (1007)    80338 2023-01-07 03:43:58.000000 george-walrus-0.1.5rc1/walrus.py
```

### Comparing `george_walrus-0.1.5/LICENSE` & `george-walrus-0.1.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `george_walrus-0.1.5/README.md` & `george-walrus-0.1.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `george_walrus-0.1.5/setup.py` & `george-walrus-0.1.5rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     ],
     keywords=['walrus operator', 'assignment expression', 'back-port compiler'],
     py_modules=[module_name],
     python_requires='>=3.4',
     install_requires=[
         'parso>=0.6.0',         # universal AST support
         'tbtrim>=0.2.1',        # traceback trim support
-        'bpc-f2format',         # bpc-f2format
+        'f2format',             # bpc-f2format
         'bpc-utils~=0.10.0',    # utility library
         'typing;python_version<"3.5"',
         'typing_extensions',
     ],
     extras_require={
         'lint': [
             'flake8',
```

### Comparing `george_walrus-0.1.5/walrus.py` & `george-walrus-0.1.5rc1/walrus.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                        recover_files)
 from bpc_utils import Linesep
 from typing_extensions import Literal, TypedDict, final
 
 __all__ = ['main', 'walrus', 'convert']
 
 # version string
-__version__ = '0.1.5'
+__version__ = '0.1.5rc1'
 
 ###############################################################################
 # Types for annotation
 
 ScopeKeyword = Literal['global', 'nonlocal']
 
 
@@ -272,23 +272,17 @@
 
 tbtrim.set_trim_rule(predicate, strict=True, target=BPCSyntaxError)
 
 ###############################################################################
 # Main Conversion Implementation
 
 # walrus wrapper template
-
-# NAME_TEMPLATE = '''\
-# if False:
-# %(indentation)s%(name_list)s = NotImplemented
-# '''.splitlines()  # `str.splitlines` will remove trailing newline
-# make it Cython compilable
 NAME_TEMPLATE = '''\
-if '%(name)s' not in dir():
-%(indentation)s%(name)s = NotImplemented
+if False:
+%(indentation)s%(name_list)s = NotImplemented
 '''.splitlines()  # `str.splitlines` will remove trailing newline
 CALL_TEMPLATE = '_walrus_wrapper_%(name)s_%(uuid)s(%(expr)s)'
 FUNC_TEMPLATE = '''\
 def _walrus_wrapper_%(name)s_%(uuid)s(expr):
 %(indentation)s"""Wrapper function for assignment expression."""
 %(indentation)s%(scope_keyword)s %(name)s
 %(indentation)s%(name)s = expr
@@ -1019,18 +1013,18 @@
         # then, the variables and functions
         indent = self._indentation * self._indent_level
         if self._pep8:
             linesep = self._linesep * (1 if self._indent_level > 0 else 2)
         else:
             linesep = ''
         if self._vars:
-            for name in sorted(set(self._vars)):
-                self._buffer += indent + (
-                    '%s%s' % (self._linesep, indent)
-                ).join(NAME_TEMPLATE) % dict(indentation=self._indentation, name=name) + self._linesep
+            name_list = ' = '.join(sorted(set(self._vars)))
+            self._buffer += indent + (
+                '%s%s' % (self._linesep, indent)
+            ).join(NAME_TEMPLATE) % dict(indentation=self._indentation, name_list=name_list) + self._linesep
         for func in sorted(self._func, key=lambda func: func['name']):
             if self._buffer:
                 self._buffer += linesep
             self._buffer += indent + (
                 '%s%s' % (self._linesep, indent)
             ).join(FUNC_TEMPLATE) % dict(indentation=self._indentation, **func) + self._linesep
         for lamb in self._lamb:
@@ -1207,18 +1201,18 @@
         # first, the variables and functions
         indent = self._indentation * self._indent_level
         if self._pep8:
             linesep = self._linesep * (1 if self._indent_level > 0 else 2)
         else:
             linesep = ''
         if self._vars:
-            for name in sorted(set(self._vars)):
-                self._buffer += indent + (
-                    '%s%s' % (self._linesep, indent)
-                ).join(NAME_TEMPLATE) % dict(indentation=self._indentation, name=name) + self._linesep
+            name_list = ' = '.join(sorted(set(self._vars)))
+            self._buffer += indent + (
+                '%s%s' % (self._linesep, indent)
+            ).join(NAME_TEMPLATE) % dict(indentation=self._indentation, name_list=name_list) + self._linesep
         for func in sorted(self._func, key=lambda func: func['name']):
             if self._buffer:
                 self._buffer += linesep
             self._buffer += indent + (
                 '%s%s' % (self._linesep, indent)
             ).join(FUNC_TEMPLATE) % dict(indentation=self._indentation, **func) + self._linesep
         for lamb in self._lamb:
```

