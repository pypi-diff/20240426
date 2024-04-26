# Comparing `tmp/lfdfiles-2024.3.4.tar.gz` & `tmp/lfdfiles-2024.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfdfiles-2024.3.4.tar", last modified: Tue Mar  5 02:08:13 2024, max compression
+gzip compressed data, was "lfdfiles-2024.4.24.tar", last modified: Fri Apr 26 02:00:50 2024, max compression
```

## Comparing `lfdfiles-2024.3.4.tar` & `lfdfiles-2024.4.24.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 02:08:13.249606 lfdfiles-2024.3.4/
-drwxrwxrwx   0        0        0        0 2024-03-05 02:08:13.234067 lfdfiles-2024.3.4/.github/
-drwxrwxrwx   0        0        0        0 2024-03-05 02:08:13.249606 lfdfiles-2024.3.4/.github/workflows/
--rw-rw-rw-   0        0        0     1105 2024-03-05 02:00:23.000000 lfdfiles-2024.3.4/.github/workflows/wheel.yml
--rw-rw-rw-   0        0        0     3898 2024-03-05 02:08:12.000000 lfdfiles-2024.3.4/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2024-03-05 02:08:12.000000 lfdfiles-2024.3.4/LICENSE
--rw-rw-rw-   0        0        0      567 2023-08-11 03:00:09.000000 lfdfiles-2024.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     8510 2024-03-05 02:08:13.249606 lfdfiles-2024.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     7192 2024-03-05 02:08:12.000000 lfdfiles-2024.3.4/README.rst
--rw-rw-rw-   0        0        0     2812 2023-09-23 02:25:22.000000 lfdfiles-2024.3.4/fbdfix.py
-drwxrwxrwx   0        0        0        0 2024-03-05 02:08:13.249606 lfdfiles-2024.3.4/lfdfiles/
--rw-rw-rw-   0        0        0      104 2023-12-17 16:49:54.000000 lfdfiles-2024.3.4/lfdfiles/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:24:17.000000 lfdfiles-2024.3.4/lfdfiles/__main__.py
--rw-rw-rw-   0        0        0  2079138 2024-03-05 02:07:51.000000 lfdfiles-2024.3.4/lfdfiles/_lfdfiles.c
--rw-rw-rw-   0        0        0    23139 2024-03-05 02:03:39.000000 lfdfiles-2024.3.4/lfdfiles/_lfdfiles.pyx
--rw-rw-rw-   0        0        0     6486 2023-08-30 05:53:08.000000 lfdfiles-2024.3.4/lfdfiles/fbd2b64.py
--rw-rw-rw-   0        0        0   231816 2024-03-05 01:54:54.000000 lfdfiles-2024.3.4/lfdfiles/lfdfiles.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 lfdfiles-2024.3.4/lfdfiles/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-05 02:08:13.249606 lfdfiles-2024.3.4/lfdfiles.egg-info/
--rw-rw-rw-   0        0        0     8510 2024-03-05 02:08:12.000000 lfdfiles-2024.3.4/lfdfiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2024-03-05 02:08:13.000000 lfdfiles-2024.3.4/lfdfiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 02:08:12.000000 lfdfiles-2024.3.4/lfdfiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-03-05 02:08:12.000000 lfdfiles-2024.3.4/lfdfiles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-05 02:08:12.000000 lfdfiles-2024.3.4/lfdfiles.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       78 2024-03-05 02:08:12.000000 lfdfiles-2024.3.4/lfdfiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-05 02:08:12.000000 lfdfiles-2024.3.4/lfdfiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-05 02:08:13.249606 lfdfiles-2024.3.4/setup.cfg
--rw-rw-rw-   0        0        0     5015 2023-12-17 16:50:02.000000 lfdfiles-2024.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:00:50.778662 lfdfiles-2024.4.24/
+drwxrwxrwx   0        0        0        0 2024-04-26 02:00:50.763034 lfdfiles-2024.4.24/.github/
+drwxrwxrwx   0        0        0        0 2024-04-26 02:00:50.763034 lfdfiles-2024.4.24/.github/workflows/
+-rw-rw-rw-   0        0        0     1115 2024-04-25 19:20:45.000000 lfdfiles-2024.4.24/.github/workflows/wheel.yml
+-rw-rw-rw-   0        0        0     3933 2024-04-26 02:00:49.000000 lfdfiles-2024.4.24/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2024-04-26 02:00:49.000000 lfdfiles-2024.4.24/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-08-11 03:00:09.000000 lfdfiles-2024.4.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     8548 2024-04-26 02:00:50.778662 lfdfiles-2024.4.24/PKG-INFO
+-rw-rw-rw-   0        0        0     7229 2024-04-26 02:00:49.000000 lfdfiles-2024.4.24/README.rst
+-rw-rw-rw-   0        0        0     2812 2023-09-23 02:25:22.000000 lfdfiles-2024.4.24/fbdfix.py
+drwxrwxrwx   0        0        0        0 2024-04-26 02:00:50.763034 lfdfiles-2024.4.24/lfdfiles/
+-rw-rw-rw-   0        0        0      104 2023-12-17 16:49:54.000000 lfdfiles-2024.4.24/lfdfiles/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:24:17.000000 lfdfiles-2024.4.24/lfdfiles/__main__.py
+-rw-rw-rw-   0        0        0  2077776 2024-04-26 02:00:30.000000 lfdfiles-2024.4.24/lfdfiles/_lfdfiles.c
+-rw-rw-rw-   0        0        0    23134 2024-04-11 16:24:16.000000 lfdfiles-2024.4.24/lfdfiles/_lfdfiles.pyx
+-rw-rw-rw-   0        0        0     6486 2023-08-30 05:53:08.000000 lfdfiles-2024.4.24/lfdfiles/fbd2b64.py
+-rw-rw-rw-   0        0        0   231900 2024-04-26 01:39:47.000000 lfdfiles-2024.4.24/lfdfiles/lfdfiles.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 lfdfiles-2024.4.24/lfdfiles/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-26 02:00:50.778662 lfdfiles-2024.4.24/lfdfiles.egg-info/
+-rw-rw-rw-   0        0        0     8548 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       78 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-26 02:00:50.000000 lfdfiles-2024.4.24/lfdfiles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 02:00:50.778662 lfdfiles-2024.4.24/setup.cfg
+-rw-rw-rw-   0        0        0     5015 2023-12-17 16:50:02.000000 lfdfiles-2024.4.24/setup.py
```

### Comparing `lfdfiles-2024.3.4/.github/workflows/wheel.yml` & `lfdfiles-2024.4.24/.github/workflows/wheel.yml`

 * *Files 7% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04, macos-12, windows-2019]
     steps:
       - uses: actions/checkout@v4
-      - uses: pypa/cibuildwheel@v2.16.5
+      - uses: pypa/cibuildwheel@v2.17.0
         env:
           CIBW_SKIP: "pp* cp37* cp38* *musllinux* *i686 *ppc64le *s390x cp39*win*arm64 cp310*win*arm64"
           CIBW_BEFORE_ALL_MACOS: curl -O https://mac.r-project.org/openmp/openmp-14.0.6-darwin20-Release.tar.gz && sudo tar fvxz openmp-14.0.6-darwin20-Release.tar.gz -C /
-          CIBW_BEFORE_BUILD: python -m pip install numpy Cython
+          CIBW_BEFORE_BUILD: python -m pip install numpy>=2.0.0rc1 Cython
           # CIBW_ARCHS_LINUX: auto aarch64
           CIBW_ARCHS_LINUX: auto
           CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_ARCHS_WINDOWS: AMD64 ARM64 x86
           CIBW_TEST_REQUIRES: numpy tifffile
           CIBW_TEST_COMMAND: python -c "import lfdfiles;from lfdfiles import _lfdfiles;print(lfdfiles.__version__)"
       - uses: actions/upload-artifact@v4
```

### Comparing `lfdfiles-2024.3.4/CHANGES.rst` & `lfdfiles-2024.4.24/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2024.3.4
 
 - Fix decoding 32-bit, 16 windows, 4 channels Spartan6 FBD files (#1).
 
 2023.9.26
 
 - Remove phasor and lifetime methods from VistaIfli (breaking).
```

### Comparing `lfdfiles-2024.3.4/LICENSE` & `lfdfiles-2024.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `lfdfiles-2024.3.4/MANIFEST.in` & `lfdfiles-2024.4.24/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lfdfiles-2024.3.4/PKG-INFO` & `lfdfiles-2024.4.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfdfiles
-Version: 2024.3.4
+Version: 2024.4.24
 Summary: Laboratory for Fluorescence Dynamics (LFD) file formats
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/lfdfiles/issues
 Project-URL: Source Code, https://github.com/cgohlke/lfdfiles
@@ -49,15 +49,15 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.3.4
+:Version: 2024.4.24
 :DOI: `10.5281/zenodo.8384166 <https://doi.org/10.5281/zenodo.8384166>`_
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
@@ -77,29 +77,33 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
-- `Cython <https://pypi.org/project/cython/>`_ 3.0.8 (build)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Cython <https://pypi.org/project/cython/>`_ 3.0.10 (build)
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.4.24 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile/>`_ 2023.8.30 (optional)
 - `Netpbmfile <https://pypi.org/project/netpbmfile/>`_ 2023.8.30 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (optional, for plotting)
 - `Click <https://pypi.python.org/pypi/click>`_ 8.1.7
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2024.3.4
 
 - Fix decoding 32-bit, 16 windows, 4 channels Spartan6 FBD files (#1).
 
 2023.9.26
 
 - Remove phasor and lifetime methods from VistaIfli (breaking).
```

### Comparing `lfdfiles-2024.3.4/README.rst` & `lfdfiles-2024.4.24/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.3.4
+:Version: 2024.4.24
 :DOI: `10.5281/zenodo.8384166 <https://doi.org/10.5281/zenodo.8384166>`_
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
@@ -42,29 +42,33 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
-- `Cython <https://pypi.org/project/cython/>`_ 3.0.8 (build)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Cython <https://pypi.org/project/cython/>`_ 3.0.10 (build)
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.4.24 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile/>`_ 2023.8.30 (optional)
 - `Netpbmfile <https://pypi.org/project/netpbmfile/>`_ 2023.8.30 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (optional, for plotting)
 - `Click <https://pypi.python.org/pypi/click>`_ 8.1.7
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2024.3.4
 
 - Fix decoding 32-bit, 16 windows, 4 channels Spartan6 FBD files (#1).
 
 2023.9.26
 
 - Remove phasor and lifetime methods from VistaIfli (breaking).
```

### Comparing `lfdfiles-2024.3.4/fbdfix.py` & `lfdfiles-2024.4.24/fbdfix.py`

 * *Files identical despite different names*

### Comparing `lfdfiles-2024.3.4/lfdfiles/_lfdfiles.c` & `lfdfiles-2024.4.24/lfdfiles/_lfdfiles.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -43,18 +43,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -138,14 +138,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -199,14 +201,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -260,60 +264,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -396,14 +423,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -739,16 +769,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1092,15 +1127,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1179,15 +1214,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1287,32 +1322,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -3210,15 +3228,14 @@
 static const char __pyx_k_datasize[] = "datasize";
 static const char __pyx_k_defaults[] = "defaults";
 static const char __pyx_k_framelen[] = "framelen";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_hist_out[] = "hist_out";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_nchannel[] = "nchannel";
-static const char __pyx_k_nwindows[] = "nwindows";
 static const char __pyx_k_pcc_mask[] = "pcc_mask";
 static const char __pyx_k_pmax_win[] = "pmax_win";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_register[] = "register";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_tcc_mask[] = "tcc_mask";
 static const char __pyx_k_uint16_t[] = "uint16_t";
@@ -3595,15 +3612,14 @@
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_n_s_nframes;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
   PyObject *__pyx_kp_u_no_start_of_frame_found_for_addr;
   PyObject *__pyx_n_s_np;
   PyObject *__pyx_n_s_numpy;
   PyObject *__pyx_n_s_numthreads;
-  PyObject *__pyx_n_s_nwindows;
   PyObject *__pyx_n_s_obj;
   PyObject *__pyx_n_s_pack;
   PyObject *__pyx_n_s_pcc;
   PyObject *__pyx_n_s_pcc_mask;
   PyObject *__pyx_n_s_pcc_shr;
   PyObject *__pyx_n_s_pdiv;
   PyObject *__pyx_n_s_photons;
@@ -3926,15 +3942,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_n_s_nframes);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_CLEAR(clear_module_state->__pyx_kp_u_no_start_of_frame_found_for_addr);
   Py_CLEAR(clear_module_state->__pyx_n_s_np);
   Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
   Py_CLEAR(clear_module_state->__pyx_n_s_numthreads);
-  Py_CLEAR(clear_module_state->__pyx_n_s_nwindows);
   Py_CLEAR(clear_module_state->__pyx_n_s_obj);
   Py_CLEAR(clear_module_state->__pyx_n_s_pack);
   Py_CLEAR(clear_module_state->__pyx_n_s_pcc);
   Py_CLEAR(clear_module_state->__pyx_n_s_pcc_mask);
   Py_CLEAR(clear_module_state->__pyx_n_s_pcc_shr);
   Py_CLEAR(clear_module_state->__pyx_n_s_pdiv);
   Py_CLEAR(clear_module_state->__pyx_n_s_photons);
@@ -4235,15 +4250,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_n_s_nframes);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_VISIT(traverse_module_state->__pyx_kp_u_no_start_of_frame_found_for_addr);
   Py_VISIT(traverse_module_state->__pyx_n_s_np);
   Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
   Py_VISIT(traverse_module_state->__pyx_n_s_numthreads);
-  Py_VISIT(traverse_module_state->__pyx_n_s_nwindows);
   Py_VISIT(traverse_module_state->__pyx_n_s_obj);
   Py_VISIT(traverse_module_state->__pyx_n_s_pack);
   Py_VISIT(traverse_module_state->__pyx_n_s_pcc);
   Py_VISIT(traverse_module_state->__pyx_n_s_pcc_mask);
   Py_VISIT(traverse_module_state->__pyx_n_s_pcc_shr);
   Py_VISIT(traverse_module_state->__pyx_n_s_pdiv);
   Py_VISIT(traverse_module_state->__pyx_n_s_photons);
@@ -4558,15 +4572,14 @@
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_n_s_nframes __pyx_mstate_global->__pyx_n_s_nframes
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
 #define __pyx_kp_u_no_start_of_frame_found_for_addr __pyx_mstate_global->__pyx_kp_u_no_start_of_frame_found_for_addr
 #define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
 #define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
 #define __pyx_n_s_numthreads __pyx_mstate_global->__pyx_n_s_numthreads
-#define __pyx_n_s_nwindows __pyx_mstate_global->__pyx_n_s_nwindows
 #define __pyx_n_s_obj __pyx_mstate_global->__pyx_n_s_obj
 #define __pyx_n_s_pack __pyx_mstate_global->__pyx_n_s_pack
 #define __pyx_n_s_pcc __pyx_mstate_global->__pyx_n_s_pcc
 #define __pyx_n_s_pcc_mask __pyx_mstate_global->__pyx_n_s_pcc_mask
 #define __pyx_n_s_pcc_shr __pyx_mstate_global->__pyx_n_s_pcc_shr
 #define __pyx_n_s_pdiv __pyx_mstate_global->__pyx_n_s_pdiv
 #define __pyx_n_s_photons __pyx_mstate_global->__pyx_n_s_photons
@@ -20438,15 +20451,15 @@
       __pyx_v_swap_words = __Pyx_PyObject_IsTrue(values[16]); if (unlikely((__pyx_v_swap_words == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
     } else {
 
       /* "lfdfiles/_lfdfiles.pyx":88
  *     data_t win_mask,
  *     uint32_t win_shr,
  *     bint swap_words = False,             # <<<<<<<<<<<<<<
- *     ):
+ * ):
  *     """Decode FLIMbox data stream.
  */
       __pyx_v_swap_words = ((int)((int)((int)0)));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
@@ -20934,15 +20947,15 @@
                                 }
 
                                 /* "lfdfiles/_lfdfiles.pyx":173
  *                     )
  *                 else:
  *                     bins_out[c, i] = -1  # no event             # <<<<<<<<<<<<<<
  *             else:
- *                bins_out[c, i] = -2  # should never happen
+ *                 bins_out[c, i] = -2  # should never happen
  */
                                 /*else*/ {
                                   __pyx_t_12 = __pyx_v_c;
                                   __pyx_t_13 = __pyx_v_i;
                                   *((int8_t *) ( /* dim=1 */ ((char *) (((int8_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_12 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_13)) )) = -1;
                                 }
                                 __pyx_L23:;
@@ -20956,15 +20969,15 @@
  */
                                 goto __pyx_L22;
                               }
 
                               /* "lfdfiles/_lfdfiles.pyx":175
  *                     bins_out[c, i] = -1  # no event
  *             else:
- *                bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
+ *                 bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
  * 
  *     # record up-markers and absolute time
  */
                               /*else*/ {
                                 __pyx_t_13 = __pyx_v_c;
                                 __pyx_t_12 = __pyx_v_i;
                                 *((int8_t *) ( /* dim=1 */ ((char *) (((int8_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_13 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_12)) )) = -2;
@@ -21621,15 +21634,15 @@
       __pyx_v_swap_words = __Pyx_PyObject_IsTrue(values[16]); if (unlikely((__pyx_v_swap_words == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
     } else {
 
       /* "lfdfiles/_lfdfiles.pyx":88
  *     data_t win_mask,
  *     uint32_t win_shr,
  *     bint swap_words = False,             # <<<<<<<<<<<<<<
- *     ):
+ * ):
  *     """Decode FLIMbox data stream.
  */
       __pyx_v_swap_words = ((int)((int)((int)0)));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
@@ -22117,15 +22130,15 @@
                                 }
 
                                 /* "lfdfiles/_lfdfiles.pyx":173
  *                     )
  *                 else:
  *                     bins_out[c, i] = -1  # no event             # <<<<<<<<<<<<<<
  *             else:
- *                bins_out[c, i] = -2  # should never happen
+ *                 bins_out[c, i] = -2  # should never happen
  */
                                 /*else*/ {
                                   __pyx_t_12 = __pyx_v_c;
                                   __pyx_t_13 = __pyx_v_i;
                                   *((int8_t *) ( /* dim=1 */ ((char *) (((int8_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_12 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_13)) )) = -1;
                                 }
                                 __pyx_L23:;
@@ -22139,15 +22152,15 @@
  */
                                 goto __pyx_L22;
                               }
 
                               /* "lfdfiles/_lfdfiles.pyx":175
  *                     bins_out[c, i] = -1  # no event
  *             else:
- *                bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
+ *                 bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
  * 
  *     # record up-markers and absolute time
  */
                               /*else*/ {
                                 __pyx_t_13 = __pyx_v_c;
                                 __pyx_t_12 = __pyx_v_i;
                                 *((int8_t *) ( /* dim=1 */ ((char *) (((int8_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_13 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_12)) )) = -2;
@@ -22804,15 +22817,15 @@
       __pyx_v_swap_words = __Pyx_PyObject_IsTrue(values[16]); if (unlikely((__pyx_v_swap_words == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
     } else {
 
       /* "lfdfiles/_lfdfiles.pyx":88
  *     data_t win_mask,
  *     uint32_t win_shr,
  *     bint swap_words = False,             # <<<<<<<<<<<<<<
- *     ):
+ * ):
  *     """Decode FLIMbox data stream.
  */
       __pyx_v_swap_words = ((int)((int)((int)0)));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
@@ -23300,15 +23313,15 @@
                                 }
 
                                 /* "lfdfiles/_lfdfiles.pyx":173
  *                     )
  *                 else:
  *                     bins_out[c, i] = -1  # no event             # <<<<<<<<<<<<<<
  *             else:
- *                bins_out[c, i] = -2  # should never happen
+ *                 bins_out[c, i] = -2  # should never happen
  */
                                 /*else*/ {
                                   __pyx_t_12 = __pyx_v_c;
                                   __pyx_t_13 = __pyx_v_i;
                                   *((int16_t *) ( /* dim=1 */ ((char *) (((int16_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_12 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_13)) )) = -1;
                                 }
                                 __pyx_L23:;
@@ -23322,15 +23335,15 @@
  */
                                 goto __pyx_L22;
                               }
 
                               /* "lfdfiles/_lfdfiles.pyx":175
  *                     bins_out[c, i] = -1  # no event
  *             else:
- *                bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
+ *                 bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
  * 
  *     # record up-markers and absolute time
  */
                               /*else*/ {
                                 __pyx_t_13 = __pyx_v_c;
                                 __pyx_t_12 = __pyx_v_i;
                                 *((int16_t *) ( /* dim=1 */ ((char *) (((int16_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_13 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_12)) )) = -2;
@@ -23987,15 +24000,15 @@
       __pyx_v_swap_words = __Pyx_PyObject_IsTrue(values[16]); if (unlikely((__pyx_v_swap_words == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
     } else {
 
       /* "lfdfiles/_lfdfiles.pyx":88
  *     data_t win_mask,
  *     uint32_t win_shr,
  *     bint swap_words = False,             # <<<<<<<<<<<<<<
- *     ):
+ * ):
  *     """Decode FLIMbox data stream.
  */
       __pyx_v_swap_words = ((int)((int)((int)0)));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
@@ -24483,15 +24496,15 @@
                                 }
 
                                 /* "lfdfiles/_lfdfiles.pyx":173
  *                     )
  *                 else:
  *                     bins_out[c, i] = -1  # no event             # <<<<<<<<<<<<<<
  *             else:
- *                bins_out[c, i] = -2  # should never happen
+ *                 bins_out[c, i] = -2  # should never happen
  */
                                 /*else*/ {
                                   __pyx_t_12 = __pyx_v_c;
                                   __pyx_t_13 = __pyx_v_i;
                                   *((int16_t *) ( /* dim=1 */ ((char *) (((int16_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_12 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_13)) )) = -1;
                                 }
                                 __pyx_L23:;
@@ -24505,15 +24518,15 @@
  */
                                 goto __pyx_L22;
                               }
 
                               /* "lfdfiles/_lfdfiles.pyx":175
  *                     bins_out[c, i] = -1  # no event
  *             else:
- *                bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
+ *                 bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
  * 
  *     # record up-markers and absolute time
  */
                               /*else*/ {
                                 __pyx_t_13 = __pyx_v_c;
                                 __pyx_t_12 = __pyx_v_i;
                                 *((int16_t *) ( /* dim=1 */ ((char *) (((int16_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_13 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_12)) )) = -2;
@@ -25170,15 +25183,15 @@
       __pyx_v_swap_words = __Pyx_PyObject_IsTrue(values[16]); if (unlikely((__pyx_v_swap_words == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
     } else {
 
       /* "lfdfiles/_lfdfiles.pyx":88
  *     data_t win_mask,
  *     uint32_t win_shr,
  *     bint swap_words = False,             # <<<<<<<<<<<<<<
- *     ):
+ * ):
  *     """Decode FLIMbox data stream.
  */
       __pyx_v_swap_words = ((int)((int)((int)0)));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
@@ -25666,15 +25679,15 @@
                                 }
 
                                 /* "lfdfiles/_lfdfiles.pyx":173
  *                     )
  *                 else:
  *                     bins_out[c, i] = -1  # no event             # <<<<<<<<<<<<<<
  *             else:
- *                bins_out[c, i] = -2  # should never happen
+ *                 bins_out[c, i] = -2  # should never happen
  */
                                 /*else*/ {
                                   __pyx_t_12 = __pyx_v_c;
                                   __pyx_t_13 = __pyx_v_i;
                                   *((int8_t *) ( /* dim=1 */ ((char *) (((int8_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_12 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_13)) )) = -1;
                                 }
                                 __pyx_L23:;
@@ -25688,15 +25701,15 @@
  */
                                 goto __pyx_L22;
                               }
 
                               /* "lfdfiles/_lfdfiles.pyx":175
  *                     bins_out[c, i] = -1  # no event
  *             else:
- *                bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
+ *                 bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
  * 
  *     # record up-markers and absolute time
  */
                               /*else*/ {
                                 __pyx_t_13 = __pyx_v_c;
                                 __pyx_t_12 = __pyx_v_i;
                                 *((int8_t *) ( /* dim=1 */ ((char *) (((int8_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_13 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_12)) )) = -2;
@@ -26353,15 +26366,15 @@
       __pyx_v_swap_words = __Pyx_PyObject_IsTrue(values[16]); if (unlikely((__pyx_v_swap_words == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
     } else {
 
       /* "lfdfiles/_lfdfiles.pyx":88
  *     data_t win_mask,
  *     uint32_t win_shr,
  *     bint swap_words = False,             # <<<<<<<<<<<<<<
- *     ):
+ * ):
  *     """Decode FLIMbox data stream.
  */
       __pyx_v_swap_words = ((int)((int)((int)0)));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
@@ -26849,15 +26862,15 @@
                                 }
 
                                 /* "lfdfiles/_lfdfiles.pyx":173
  *                     )
  *                 else:
  *                     bins_out[c, i] = -1  # no event             # <<<<<<<<<<<<<<
  *             else:
- *                bins_out[c, i] = -2  # should never happen
+ *                 bins_out[c, i] = -2  # should never happen
  */
                                 /*else*/ {
                                   __pyx_t_12 = __pyx_v_c;
                                   __pyx_t_13 = __pyx_v_i;
                                   *((int8_t *) ( /* dim=1 */ ((char *) (((int8_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_12 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_13)) )) = -1;
                                 }
                                 __pyx_L23:;
@@ -26871,15 +26884,15 @@
  */
                                 goto __pyx_L22;
                               }
 
                               /* "lfdfiles/_lfdfiles.pyx":175
  *                     bins_out[c, i] = -1  # no event
  *             else:
- *                bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
+ *                 bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
  * 
  *     # record up-markers and absolute time
  */
                               /*else*/ {
                                 __pyx_t_13 = __pyx_v_c;
                                 __pyx_t_12 = __pyx_v_i;
                                 *((int8_t *) ( /* dim=1 */ ((char *) (((int8_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_13 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_12)) )) = -2;
@@ -27536,15 +27549,15 @@
       __pyx_v_swap_words = __Pyx_PyObject_IsTrue(values[16]); if (unlikely((__pyx_v_swap_words == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
     } else {
 
       /* "lfdfiles/_lfdfiles.pyx":88
  *     data_t win_mask,
  *     uint32_t win_shr,
  *     bint swap_words = False,             # <<<<<<<<<<<<<<
- *     ):
+ * ):
  *     """Decode FLIMbox data stream.
  */
       __pyx_v_swap_words = ((int)((int)((int)0)));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
@@ -28032,15 +28045,15 @@
                                 }
 
                                 /* "lfdfiles/_lfdfiles.pyx":173
  *                     )
  *                 else:
  *                     bins_out[c, i] = -1  # no event             # <<<<<<<<<<<<<<
  *             else:
- *                bins_out[c, i] = -2  # should never happen
+ *                 bins_out[c, i] = -2  # should never happen
  */
                                 /*else*/ {
                                   __pyx_t_12 = __pyx_v_c;
                                   __pyx_t_13 = __pyx_v_i;
                                   *((int16_t *) ( /* dim=1 */ ((char *) (((int16_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_12 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_13)) )) = -1;
                                 }
                                 __pyx_L23:;
@@ -28054,15 +28067,15 @@
  */
                                 goto __pyx_L22;
                               }
 
                               /* "lfdfiles/_lfdfiles.pyx":175
  *                     bins_out[c, i] = -1  # no event
  *             else:
- *                bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
+ *                 bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
  * 
  *     # record up-markers and absolute time
  */
                               /*else*/ {
                                 __pyx_t_13 = __pyx_v_c;
                                 __pyx_t_12 = __pyx_v_i;
                                 *((int16_t *) ( /* dim=1 */ ((char *) (((int16_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_13 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_12)) )) = -2;
@@ -28719,15 +28732,15 @@
       __pyx_v_swap_words = __Pyx_PyObject_IsTrue(values[16]); if (unlikely((__pyx_v_swap_words == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
     } else {
 
       /* "lfdfiles/_lfdfiles.pyx":88
  *     data_t win_mask,
  *     uint32_t win_shr,
  *     bint swap_words = False,             # <<<<<<<<<<<<<<
- *     ):
+ * ):
  *     """Decode FLIMbox data stream.
  */
       __pyx_v_swap_words = ((int)((int)((int)0)));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
@@ -29215,15 +29228,15 @@
                                 }
 
                                 /* "lfdfiles/_lfdfiles.pyx":173
  *                     )
  *                 else:
  *                     bins_out[c, i] = -1  # no event             # <<<<<<<<<<<<<<
  *             else:
- *                bins_out[c, i] = -2  # should never happen
+ *                 bins_out[c, i] = -2  # should never happen
  */
                                 /*else*/ {
                                   __pyx_t_12 = __pyx_v_c;
                                   __pyx_t_13 = __pyx_v_i;
                                   *((int16_t *) ( /* dim=1 */ ((char *) (((int16_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_12 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_13)) )) = -1;
                                 }
                                 __pyx_L23:;
@@ -29237,15 +29250,15 @@
  */
                                 goto __pyx_L22;
                               }
 
                               /* "lfdfiles/_lfdfiles.pyx":175
  *                     bins_out[c, i] = -1  # no event
  *             else:
- *                bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
+ *                 bins_out[c, i] = -2  # should never happen             # <<<<<<<<<<<<<<
  * 
  *     # record up-markers and absolute time
  */
                               /*else*/ {
                                 __pyx_t_13 = __pyx_v_c;
                                 __pyx_t_12 = __pyx_v_i;
                                 *((int16_t *) ( /* dim=1 */ ((char *) (((int16_t *) ( /* dim=0 */ (__pyx_v_bins_out.data + __pyx_t_13 * __pyx_v_bins_out.strides[0]) )) + __pyx_t_12)) )) = -2;
@@ -31056,15 +31069,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_26flimbox_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out) {
   Py_ssize_t __pyx_v_nframes;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nchannels;
   Py_ssize_t __pyx_v_framelen;
-  CYTHON_UNUSED Py_ssize_t __pyx_v_nwindows;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_f;
   Py_ssize_t __pyx_v_c;
   Py_ssize_t __pyx_v_idx;
   uint32_t __pyx_v_t0;
@@ -31107,36 +31119,27 @@
   __pyx_v_nframes = (__pyx_v_hist_out.shape[0]);
 
   /* "lfdfiles/_lfdfiles.pyx":241
  *     cdef:
  *         ssize_t nframes = hist_out.shape[0]
  *         ssize_t nchannels = hist_out.shape[1]             # <<<<<<<<<<<<<<
  *         ssize_t framelen = hist_out.shape[2]
- *         ssize_t nwindows = hist_out.shape[3]
+ *         # ssize_t nwindows = hist_out.shape[3]
  */
   __pyx_v_nchannels = (__pyx_v_hist_out.shape[1]);
 
   /* "lfdfiles/_lfdfiles.pyx":242
  *         ssize_t nframes = hist_out.shape[0]
  *         ssize_t nchannels = hist_out.shape[1]
  *         ssize_t framelen = hist_out.shape[2]             # <<<<<<<<<<<<<<
- *         ssize_t nwindows = hist_out.shape[3]
+ *         # ssize_t nwindows = hist_out.shape[3]
  *         ssize_t i, j, k, f, c, idx
  */
   __pyx_v_framelen = (__pyx_v_hist_out.shape[2]);
 
-  /* "lfdfiles/_lfdfiles.pyx":243
- *         ssize_t nchannels = hist_out.shape[1]
- *         ssize_t framelen = hist_out.shape[2]
- *         ssize_t nwindows = hist_out.shape[3]             # <<<<<<<<<<<<<<
- *         ssize_t i, j, k, f, c, idx
- *         times_t t0
- */
-  __pyx_v_nwindows = (__pyx_v_hist_out.shape[3]);
-
   /* "lfdfiles/_lfdfiles.pyx":248
  *         bins_t w
  * 
  *     if bins.shape[0] != hist_out.shape[1]:             # <<<<<<<<<<<<<<
  *         raise ValueError('shape mismatch between bins and hist_out')
  *     if bins.shape[1] != times.shape[0]:
  */
@@ -31709,15 +31712,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_28flimbox_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out) {
   Py_ssize_t __pyx_v_nframes;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nchannels;
   Py_ssize_t __pyx_v_framelen;
-  CYTHON_UNUSED Py_ssize_t __pyx_v_nwindows;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_f;
   Py_ssize_t __pyx_v_c;
   Py_ssize_t __pyx_v_idx;
   uint64_t __pyx_v_t0;
@@ -31760,36 +31762,27 @@
   __pyx_v_nframes = (__pyx_v_hist_out.shape[0]);
 
   /* "lfdfiles/_lfdfiles.pyx":241
  *     cdef:
  *         ssize_t nframes = hist_out.shape[0]
  *         ssize_t nchannels = hist_out.shape[1]             # <<<<<<<<<<<<<<
  *         ssize_t framelen = hist_out.shape[2]
- *         ssize_t nwindows = hist_out.shape[3]
+ *         # ssize_t nwindows = hist_out.shape[3]
  */
   __pyx_v_nchannels = (__pyx_v_hist_out.shape[1]);
 
   /* "lfdfiles/_lfdfiles.pyx":242
  *         ssize_t nframes = hist_out.shape[0]
  *         ssize_t nchannels = hist_out.shape[1]
  *         ssize_t framelen = hist_out.shape[2]             # <<<<<<<<<<<<<<
- *         ssize_t nwindows = hist_out.shape[3]
+ *         # ssize_t nwindows = hist_out.shape[3]
  *         ssize_t i, j, k, f, c, idx
  */
   __pyx_v_framelen = (__pyx_v_hist_out.shape[2]);
 
-  /* "lfdfiles/_lfdfiles.pyx":243
- *         ssize_t nchannels = hist_out.shape[1]
- *         ssize_t framelen = hist_out.shape[2]
- *         ssize_t nwindows = hist_out.shape[3]             # <<<<<<<<<<<<<<
- *         ssize_t i, j, k, f, c, idx
- *         times_t t0
- */
-  __pyx_v_nwindows = (__pyx_v_hist_out.shape[3]);
-
   /* "lfdfiles/_lfdfiles.pyx":248
  *         bins_t w
  * 
  *     if bins.shape[0] != hist_out.shape[1]:             # <<<<<<<<<<<<<<
  *         raise ValueError('shape mismatch between bins and hist_out')
  *     if bins.shape[1] != times.shape[0]:
  */
@@ -32362,15 +32355,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_30flimbox_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out) {
   Py_ssize_t __pyx_v_nframes;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nchannels;
   Py_ssize_t __pyx_v_framelen;
-  CYTHON_UNUSED Py_ssize_t __pyx_v_nwindows;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_f;
   Py_ssize_t __pyx_v_c;
   Py_ssize_t __pyx_v_idx;
   uint32_t __pyx_v_t0;
@@ -32413,36 +32405,27 @@
   __pyx_v_nframes = (__pyx_v_hist_out.shape[0]);
 
   /* "lfdfiles/_lfdfiles.pyx":241
  *     cdef:
  *         ssize_t nframes = hist_out.shape[0]
  *         ssize_t nchannels = hist_out.shape[1]             # <<<<<<<<<<<<<<
  *         ssize_t framelen = hist_out.shape[2]
- *         ssize_t nwindows = hist_out.shape[3]
+ *         # ssize_t nwindows = hist_out.shape[3]
  */
   __pyx_v_nchannels = (__pyx_v_hist_out.shape[1]);
 
   /* "lfdfiles/_lfdfiles.pyx":242
  *         ssize_t nframes = hist_out.shape[0]
  *         ssize_t nchannels = hist_out.shape[1]
  *         ssize_t framelen = hist_out.shape[2]             # <<<<<<<<<<<<<<
- *         ssize_t nwindows = hist_out.shape[3]
+ *         # ssize_t nwindows = hist_out.shape[3]
  *         ssize_t i, j, k, f, c, idx
  */
   __pyx_v_framelen = (__pyx_v_hist_out.shape[2]);
 
-  /* "lfdfiles/_lfdfiles.pyx":243
- *         ssize_t nchannels = hist_out.shape[1]
- *         ssize_t framelen = hist_out.shape[2]
- *         ssize_t nwindows = hist_out.shape[3]             # <<<<<<<<<<<<<<
- *         ssize_t i, j, k, f, c, idx
- *         times_t t0
- */
-  __pyx_v_nwindows = (__pyx_v_hist_out.shape[3]);
-
   /* "lfdfiles/_lfdfiles.pyx":248
  *         bins_t w
  * 
  *     if bins.shape[0] != hist_out.shape[1]:             # <<<<<<<<<<<<<<
  *         raise ValueError('shape mismatch between bins and hist_out')
  *     if bins.shape[1] != times.shape[0]:
  */
@@ -33015,15 +32998,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_32flimbox_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out) {
   Py_ssize_t __pyx_v_nframes;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nchannels;
   Py_ssize_t __pyx_v_framelen;
-  CYTHON_UNUSED Py_ssize_t __pyx_v_nwindows;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_f;
   Py_ssize_t __pyx_v_c;
   Py_ssize_t __pyx_v_idx;
   uint64_t __pyx_v_t0;
@@ -33066,36 +33048,27 @@
   __pyx_v_nframes = (__pyx_v_hist_out.shape[0]);
 
   /* "lfdfiles/_lfdfiles.pyx":241
  *     cdef:
  *         ssize_t nframes = hist_out.shape[0]
  *         ssize_t nchannels = hist_out.shape[1]             # <<<<<<<<<<<<<<
  *         ssize_t framelen = hist_out.shape[2]
- *         ssize_t nwindows = hist_out.shape[3]
+ *         # ssize_t nwindows = hist_out.shape[3]
  */
   __pyx_v_nchannels = (__pyx_v_hist_out.shape[1]);
 
   /* "lfdfiles/_lfdfiles.pyx":242
  *         ssize_t nframes = hist_out.shape[0]
  *         ssize_t nchannels = hist_out.shape[1]
  *         ssize_t framelen = hist_out.shape[2]             # <<<<<<<<<<<<<<
- *         ssize_t nwindows = hist_out.shape[3]
+ *         # ssize_t nwindows = hist_out.shape[3]
  *         ssize_t i, j, k, f, c, idx
  */
   __pyx_v_framelen = (__pyx_v_hist_out.shape[2]);
 
-  /* "lfdfiles/_lfdfiles.pyx":243
- *         ssize_t nchannels = hist_out.shape[1]
- *         ssize_t framelen = hist_out.shape[2]
- *         ssize_t nwindows = hist_out.shape[3]             # <<<<<<<<<<<<<<
- *         ssize_t i, j, k, f, c, idx
- *         times_t t0
- */
-  __pyx_v_nwindows = (__pyx_v_hist_out.shape[3]);
-
   /* "lfdfiles/_lfdfiles.pyx":248
  *         bins_t w
  * 
  *     if bins.shape[0] != hist_out.shape[1]:             # <<<<<<<<<<<<<<
  *         raise ValueError('shape mismatch between bins and hist_out')
  *     if bins.shape[1] != times.shape[0]:
  */
@@ -40147,15 +40120,14 @@
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_n_s_nframes, __pyx_k_nframes, sizeof(__pyx_k_nframes), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
     {&__pyx_kp_u_no_start_of_frame_found_for_addr, __pyx_k_no_start_of_frame_found_for_addr, sizeof(__pyx_k_no_start_of_frame_found_for_addr), 0, 1, 0, 0},
     {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
     {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
     {&__pyx_n_s_numthreads, __pyx_k_numthreads, sizeof(__pyx_k_numthreads), 0, 0, 1, 1},
-    {&__pyx_n_s_nwindows, __pyx_k_nwindows, sizeof(__pyx_k_nwindows), 0, 0, 1, 1},
     {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
     {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
     {&__pyx_n_s_pcc, __pyx_k_pcc, sizeof(__pyx_k_pcc), 0, 0, 1, 1},
     {&__pyx_n_s_pcc_mask, __pyx_k_pcc_mask, sizeof(__pyx_k_pcc_mask), 0, 0, 1, 1},
     {&__pyx_n_s_pcc_shr, __pyx_k_pcc_shr, sizeof(__pyx_k_pcc_shr), 0, 0, 1, 1},
     {&__pyx_n_s_pdiv, __pyx_k_pdiv, sizeof(__pyx_k_pdiv), 0, 0, 1, 1},
     {&__pyx_n_s_photons, __pyx_k_photons, sizeof(__pyx_k_photons), 0, 0, 1, 1},
@@ -40500,18 +40472,18 @@
   /* "lfdfiles/_lfdfiles.pyx":209
  * 
  * 
  * def flimbox_histogram(             # <<<<<<<<<<<<<<
  *     bins_t[:, ::1] bins,
  *     times_t[::1] times,
  */
-  __pyx_tuple__33 = PyTuple_Pack(18, __pyx_n_s_bins, __pyx_n_s_times, __pyx_n_s_frame_markers, __pyx_n_s_units_per_sample, __pyx_n_s_scanner_frame_start, __pyx_n_s_hist_out, __pyx_n_s_nframes, __pyx_n_s_nchannels, __pyx_n_s_framelen, __pyx_n_s_nwindows, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_f, __pyx_n_s_c, __pyx_n_s_idx, __pyx_n_s_t0, __pyx_n_s_w); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(17, __pyx_n_s_bins, __pyx_n_s_times, __pyx_n_s_frame_markers, __pyx_n_s_units_per_sample, __pyx_n_s_scanner_frame_start, __pyx_n_s_hist_out, __pyx_n_s_nframes, __pyx_n_s_nchannels, __pyx_n_s_framelen, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_f, __pyx_n_s_c, __pyx_n_s_idx, __pyx_n_s_t0, __pyx_n_s_w); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lfdfiles__lfdfiles_pyx, __pyx_n_s_flimbox_histogram, 209, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lfdfiles__lfdfiles_pyx, __pyx_n_s_flimbox_histogram, 209, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 209, __pyx_L1_error)
 
   /* "lfdfiles/_lfdfiles.pyx":294
  * 
  * 
  * def sflim_decode(             # <<<<<<<<<<<<<<
  *     const uint32_t[::1] data,
  *     sflim_t[:, :, :, ::1] sflim,
@@ -46549,15 +46521,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `lfdfiles-2024.3.4/lfdfiles/_lfdfiles.pyx` & `lfdfiles-2024.4.24/lfdfiles/_lfdfiles.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     data_t pcc_mask,
     uint32_t pcc_shr,
     data_t marker_mask,
     uint32_t marker_shr,
     data_t win_mask,
     uint32_t win_shr,
     bint swap_words = False,
-    ):
+):
     """Decode FLIMbox data stream.
 
     Parameters:
         data (numpy.ndarray):
             FLIMbox data stream without header.
             An `uint16` (16-bit FLIMbox) or `uint32` (32-bit FLIMbox) array.
         bins_out (numpy.ndarray):
@@ -168,15 +168,15 @@
                 if win >= 0:
                     bins_out[c, i] = <bins_t>(
                         (pmax-1 - (pcc + win * pmax_win) % pmax) // pdiv
                     )
                 else:
                     bins_out[c, i] = -1  # no event
             else:
-               bins_out[c, i] = -2  # should never happen
+                bins_out[c, i] = -2  # should never happen
 
     # record up-markers and absolute time
     tcc_max = (tcc_mask >> tcc_shr) + 1
     j = 0
     d = data[0]
     if swap_words:
         d = (d >> 16) | (d << 16)
@@ -209,15 +209,15 @@
 def flimbox_histogram(
     bins_t[:, ::1] bins,
     times_t[::1] times,
     frame_markers,
     double units_per_sample,
     double scanner_frame_start,
     uint16_t[:, :, :, ::1] hist_out
-    ):
+):
     """Calculate histograms from decoded FLIMbox data and frame markers.
 
     Parameters:
         bins (numpy.ndarray):
             Cross correlation phase index for all channels and data points.
             A `int8` or `int16` array of shape `(channels, data.size)`.
             A value of -1 means no photon was counted.
@@ -236,15 +236,15 @@
             where computed histogram will be stored.
 
     """
     cdef:
         ssize_t nframes = hist_out.shape[0]
         ssize_t nchannels = hist_out.shape[1]
         ssize_t framelen = hist_out.shape[2]
-        ssize_t nwindows = hist_out.shape[3]
+        # ssize_t nwindows = hist_out.shape[3]
         ssize_t i, j, k, f, c, idx
         times_t t0
         bins_t w
 
     if bins.shape[0] != hist_out.shape[1]:
         raise ValueError('shape mismatch between bins and hist_out')
     if bins.shape[1] != times.shape[0]:
```

### Comparing `lfdfiles-2024.3.4/lfdfiles/fbd2b64.py` & `lfdfiles-2024.4.24/lfdfiles/fbd2b64.py`

 * *Files identical despite different names*

### Comparing `lfdfiles-2024.3.4/lfdfiles/lfdfiles.py` & `lfdfiles-2024.4.24/lfdfiles/lfdfiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.3.4
+:Version: 2024.4.24
 :DOI: `10.5281/zenodo.8384166 <https://doi.org/10.5281/zenodo.8384166>`_
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
@@ -72,29 +72,33 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
-- `Cython <https://pypi.org/project/cython/>`_ 3.0.8 (build)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Cython <https://pypi.org/project/cython/>`_ 3.0.10 (build)
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.4.24 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile/>`_ 2023.8.30 (optional)
 - `Netpbmfile <https://pypi.org/project/netpbmfile/>`_ 2023.8.30 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (optional, for plotting)
 - `Click <https://pypi.python.org/pypi/click>`_ 8.1.7
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2024.3.4
 
 - Fix decoding 32-bit, 16 windows, 4 channels Spartan6 FBD files (#1).
 
 2023.9.26
 
 - Remove phasor and lifetime methods from VistaIfli (breaking).
@@ -237,15 +241,15 @@
 >>> with BioradPic('_biorad.pic') as f:
 ...     f.totiff('_biorad.tif', compression='zlib')
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.3.4'
+__version__ = '2024.4.24'
 
 __all__ = [
     'LfdFile',
     'LfdFileSequence',
     'LfdFileError',
     'RawPal',
     'SimfcsVpl',
@@ -328,16 +332,16 @@
     parse_kwargs,
     product,
     stripnull,
     update_kwargs,
 )
 
 if TYPE_CHECKING:
-    from collections.abc import Iterator, Sequence
-    from typing import Any, Callable, ClassVar, Literal, TypeVar
+    from collections.abc import Callable, Iterator, Sequence
+    from typing import Any, ClassVar, Literal, TypeVar
 
     from numpy.typing import ArrayLike, DTypeLike, NDArray
 
 # delay import optional modules
 pyplot = None
 cycler = None
 
@@ -833,17 +837,16 @@
 
         """
         if not self._filepattern or self._filepattern == r'.*':
             return
         if re.search(self._filepattern, self._filename, re.IGNORECASE) is None:
             raise LfdFileError(
                 self,
-                ".\n    File name '{}' does not match '{}')".format(
-                    self._filename, self._filepattern
-                ),
+                f'.\n    File name {self._filename!r}'
+                f' does not match {self._filepattern!r}',
             )
 
     def _decompress_header(
         self, max_length: int, /, max_read: int = 256
     ) -> bytes:
         """Return first uncompressed bytes of Zlib compressed file."""
         data = self._fh.read(max_read)
@@ -2624,15 +2627,15 @@
         >>> with FlimboxFbd('flimbox$CBCO.fbd') as f:
         ...     bins, times, markers = f.decode(
         ...         word_count=500000, skip_words=1900000
         ... )
         >>> print(bins[0, :2], times[:2], markers)
         [53 51] [ 0 42] [ 44097 124815]
         >>> hist = [numpy.bincount(b[b>=0]) for b in bins]
-        >>> numpy.argmax(hist[0])
+        >>> int(numpy.argmax(hist[0]))
         53
 
     """
 
     _filepattern = r'.*\.fbd$'
     _figureargs = {'figsize': (6, 5)}
 
@@ -4195,17 +4198,17 @@
 
     _filepattern = r'.*\.lif$'
 
     _records: list[Record]
     _record_t = numpy.dtype(
         [
             ('_title_len', 'u1'),
-            ('title', 'a80'),
+            ('title', 'S80'),
             ('number', 'i2'),
-            ('frequency', [('_len', 'u1'), ('str', 'a6')], 25),
+            ('frequency', [('_len', 'u1'), ('str', 'S6')], 25),
             ('phase', 'i2', 25),
             ('modulation', 'i2', 25),
             ('deltap', 'i2', 25),
             ('deltam', 'i2', 25),
             ('nanal', 'i2'),
             ('date', 'i2', 3),
             ('time', 'i2', 3),
@@ -4483,15 +4486,15 @@
 
     header: numpy.recarray
     """File header."""
 
     _header_t = numpy.dtype(
         [
             # undocumented file header
-            ('signature', 'a10'),  # 'VISTAIMAGE'
+            ('signature', 'S10'),  # 'VISTAIMAGE'
             ('version', 'u2'),
             ('channel_bits', 'u2'),
             ('dimensions', 'u2', 3),  # XYZ
             ('boundaries', 'f4', 6),
             ('dwelltime', 'f4'),
         ]
     )
@@ -4819,15 +4822,18 @@
         return indent(
             'header:',
             *(
                 f'{name}: {value}'
                 for name, value in self.header.items()
                 if name != 'Comments'
             ),
-            *(f'{name}Offset: {value}' for name, value in self.offsets.items()),
+            *(
+                f'{name}Offset: {value}'
+                for name, value in self.offsets.items()
+            ),
             (
                 f'Comments:\n{self.header["Comments"]}'
                 if 'Comments' in self.header
                 else ''
             ),
         )
 
@@ -4842,19 +4848,19 @@
 
     Parameters:
         filename: Name of file to open.
 
     Examples:
         >>> f = FlimfastFlif('flimfast.flif')
         >>> data = f.asarray()
-        >>> f.header.frequency
-        80.652
-        >>> f.records['phase'][31]
+        >>> float(f.header.frequency)
+        80.652...
+        >>> float(f.records['phase'][31])
         348.75
-        >>> data[31, 219, 299]
+        >>> int(data[31, 219, 299])
         366
         >>> f.totiff('_flimfast.flif.tif')
         >>> f.close()
         >>> with TiffFile('_flimfast.flif.tif') as f:
         ...     assert_array_equal(f.asarray(), data)
 
     """
@@ -4866,18 +4872,18 @@
     """File header."""
 
     records: numpy.recarray
     """Frame header."""
 
     _header_t = numpy.dtype(
         [
-            ('magic', 'a8'),  # '\211FLF\r\n0\n'
-            ('creator', 'a120'),
-            ('date', 'a32'),
-            ('comments', 'a351'),
+            ('magic', 'S8'),  # '\211FLF\r\n0\n'
+            ('creator', 'S120'),
+            ('date', 'S32'),
+            ('comments', 'S351'),
             ('_', 'u1'),
             ('fileprec', '<u2'),
             ('records', '<u2'),
             ('phases', '<i4'),
             ('width', '<i4'),
             ('height', '<i4'),
             ('dataprec', '<i4'),
```

### Comparing `lfdfiles-2024.3.4/lfdfiles.egg-info/PKG-INFO` & `lfdfiles-2024.4.24/lfdfiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfdfiles
-Version: 2024.3.4
+Version: 2024.4.24
 Summary: Laboratory for Fluorescence Dynamics (LFD) file formats
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/lfdfiles/issues
 Project-URL: Source Code, https://github.com/cgohlke/lfdfiles
@@ -49,15 +49,15 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.3.4
+:Version: 2024.4.24
 :DOI: `10.5281/zenodo.8384166 <https://doi.org/10.5281/zenodo.8384166>`_
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
@@ -77,29 +77,33 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
-- `Cython <https://pypi.org/project/cython/>`_ 3.0.8 (build)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
+- `Cython <https://pypi.org/project/cython/>`_ 3.0.10 (build)
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.4.24 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile/>`_ 2023.8.30 (optional)
 - `Netpbmfile <https://pypi.org/project/netpbmfile/>`_ 2023.8.30 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (optional, for plotting)
 - `Click <https://pypi.python.org/pypi/click>`_ 8.1.7
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2024.4.24
+
+- Support NumPy 2.
+
 2024.3.4
 
 - Fix decoding 32-bit, 16 windows, 4 channels Spartan6 FBD files (#1).
 
 2023.9.26
 
 - Remove phasor and lifetime methods from VistaIfli (breaking).
```

### Comparing `lfdfiles-2024.3.4/setup.py` & `lfdfiles-2024.4.24/setup.py`

 * *Files identical despite different names*

