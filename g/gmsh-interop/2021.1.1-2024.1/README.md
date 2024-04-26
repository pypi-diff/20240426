# Comparing `tmp/gmsh_interop-2021.1.1.tar.gz` & `tmp/gmsh_interop-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmsh_interop-2021.1.1.tar", last modified: Sun Dec 26 17:28:37 2021, max compression
+gzip compressed data, was "gmsh_interop-2024.1.tar", last modified: Fri Apr 26 19:05:50 2024, max compression
```

## Comparing `gmsh_interop-2021.1.1.tar` & `gmsh_interop-2024.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2021-12-26 17:28:37.271728 gmsh_interop-2021.1.1/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1152 2020-08-26 20:55:05.000000 gmsh_interop-2021.1.1/LICENSE
--rw-r--r--   0 andreas   (1000) andreas   (1000)      150 2021-03-10 19:49:54.000000 gmsh_interop-2021.1.1/MANIFEST.in
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2524 2021-12-26 17:28:37.271728 gmsh_interop-2021.1.1/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1189 2021-03-08 06:42:12.000000 gmsh_interop-2021.1.1/README.rst
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2021-12-26 17:28:37.271728 gmsh_interop-2021.1.1/doc/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      634 2020-08-26 20:55:05.000000 gmsh_interop-2021.1.1/doc/Makefile
--rw-r--r--   0 andreas   (1000) andreas   (1000)      694 2021-08-18 18:34:30.000000 gmsh_interop-2021.1.1/doc/conf.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)      662 2020-12-02 03:59:39.000000 gmsh_interop-2021.1.1/doc/index.rst
--rw-r--r--   0 andreas   (1000) andreas   (1000)      795 2020-08-26 20:55:05.000000 gmsh_interop-2021.1.1/doc/make.bat
--rw-r--r--   0 andreas   (1000) andreas   (1000)      404 2020-08-26 20:55:05.000000 gmsh_interop-2021.1.1/doc/misc.rst
--rw-r--r--   0 andreas   (1000) andreas   (1000)       77 2020-08-26 20:55:05.000000 gmsh_interop-2021.1.1/doc/reader.rst
--rw-r--r--   0 andreas   (1000) andreas   (1000)       89 2020-08-26 20:55:05.000000 gmsh_interop-2021.1.1/doc/runner.rst
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2021-12-26 17:28:37.271728 gmsh_interop-2021.1.1/gmsh_interop/
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2019-10-01 22:43:51.000000 gmsh_interop-2021.1.1/gmsh_interop/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)   112921 2020-11-12 00:28:08.000000 gmsh_interop-2021.1.1/gmsh_interop/node_tuples.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    21405 2021-11-05 17:01:12.000000 gmsh_interop-2021.1.1/gmsh_interop/reader.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    11895 2021-12-26 17:27:26.000000 gmsh_interop-2021.1.1/gmsh_interop/runner.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)      109 2021-12-26 17:27:43.000000 gmsh_interop-2021.1.1/gmsh_interop/version.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2021-12-26 17:28:37.271728 gmsh_interop-2021.1.1/gmsh_interop.egg-info/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2524 2021-12-26 17:28:37.000000 gmsh_interop-2021.1.1/gmsh_interop.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)      464 2021-12-26 17:28:37.000000 gmsh_interop-2021.1.1/gmsh_interop.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2021-12-26 17:28:37.000000 gmsh_interop-2021.1.1/gmsh_interop.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)       21 2021-12-26 17:28:37.000000 gmsh_interop-2021.1.1/gmsh_interop.egg-info/requires.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)       13 2021-12-26 17:28:37.000000 gmsh_interop-2021.1.1/gmsh_interop.egg-info/top_level.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)      278 2021-12-26 17:28:37.271728 gmsh_interop-2021.1.1/setup.cfg
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1640 2020-11-09 17:36:08.000000 gmsh_interop-2021.1.1/setup.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2021-12-26 17:28:37.271728 gmsh_interop-2021.1.1/test/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4956 2020-11-12 00:28:08.000000 gmsh_interop-2021.1.1/test/test_gmsh.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-26 19:05:50.955294 gmsh_interop-2024.1/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1152 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/LICENSE
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      150 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/MANIFEST.in
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2363 2024-04-26 19:05:50.955294 gmsh_interop-2024.1/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1189 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/README.rst
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-26 19:05:50.955294 gmsh_interop-2024.1/doc/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      634 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/doc/Makefile
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      728 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/doc/conf.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      662 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/doc/index.rst
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      795 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/doc/make.bat
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      404 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/doc/misc.rst
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       77 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/doc/reader.rst
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       89 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/doc/runner.rst
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-26 19:05:50.955294 gmsh_interop-2024.1/gmsh_interop/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/gmsh_interop/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)   112921 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/gmsh_interop/node_tuples.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    21573 2024-04-26 18:03:43.000000 gmsh_interop-2024.1/gmsh_interop/reader.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    12543 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/gmsh_interop/runner.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      106 2024-04-26 19:01:41.000000 gmsh_interop-2024.1/gmsh_interop/version.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-26 19:05:50.955294 gmsh_interop-2024.1/gmsh_interop.egg-info/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2363 2024-04-26 19:05:50.000000 gmsh_interop-2024.1/gmsh_interop.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      464 2024-04-26 19:05:50.000000 gmsh_interop-2024.1/gmsh_interop.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2024-04-26 19:05:50.000000 gmsh_interop-2024.1/gmsh_interop.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       37 2024-04-26 19:05:50.000000 gmsh_interop-2024.1/gmsh_interop.egg-info/requires.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       13 2024-04-26 19:05:50.000000 gmsh_interop-2024.1/gmsh_interop.egg-info/top_level.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      374 2024-04-26 19:05:50.955294 gmsh_interop-2024.1/setup.cfg
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1669 2023-10-07 06:23:07.000000 gmsh_interop-2024.1/setup.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-26 19:05:50.955294 gmsh_interop-2024.1/test/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     5642 2024-04-26 18:03:43.000000 gmsh_interop-2024.1/test/test_gmsh.py
```

### Comparing `gmsh_interop-2021.1.1/LICENSE` & `gmsh_interop-2024.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmsh_interop-2021.1.1/PKG-INFO` & `gmsh_interop-2024.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: gmsh_interop
-Version: 2021.1.1
+Version: 2024.1
 Summary: A parser for GMSH's .msh format
 Home-page: http://github.com/inducer/gmsh_interop
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
-Description: Interoperability between Python and Gmsh
-        ========================================
-        
-        .. image:: https://gitlab.tiker.net/inducer/gmsh_interop/badges/main/pipeline.svg
-            :alt: Gitlab Build Status
-            :target: https://gitlab.tiker.net/inducer/gmsh_interop/commits/main
-        .. image:: https://github.com/inducer/gmsh_interop/workflows/CI/badge.svg
-            :alt: Github Build Status
-            :target: https://github.com/inducer/gmsh_interop/actions?query=branch%3Amain+workflow%3ACI
-        .. image:: https://badge.fury.io/py/gmsh_interop.png
-            :alt: Python Package Index Release Page
-            :target: https://pypi.org/project/gmsh_interop/
-        
-        This package allows Python to interoperate with the `gmsh <http://gmsh.info/>`_
-        mesh generator.
-        
-        This package contains:
-        
-        * ``gmsh_interop.reader`` to read gmsh's ``.msh`` file format.
-        * ``gmsh_interop.runner`` to run gmsh under program control and process its output.
-        
-        Its contents was extracted from `meshpy <https://github.com/inducer/meshpy>`__
-        to escape its obnoxious licensing.
-        
-        Links:
-        
-        * `Github <https://github.com/inducer/gmsh_interop>`_
-        * `Python package index <https://pypi.org/project/gmsh_interop/>`_
-        * `Documentation <https://documen.tician.de/gmsh_interop>`_
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
@@ -50,8 +19,42 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.6
+Requires-Python: ~=3.8
+License-File: LICENSE
+Requires-Dist: numpy>=1.6.0
+Requires-Dist: pytools
+Requires-Dist: packaging>=20.0
+
+Interoperability between Python and Gmsh
+========================================
+
+.. image:: https://gitlab.tiker.net/inducer/gmsh_interop/badges/main/pipeline.svg
+    :alt: Gitlab Build Status
+    :target: https://gitlab.tiker.net/inducer/gmsh_interop/commits/main
+.. image:: https://github.com/inducer/gmsh_interop/workflows/CI/badge.svg
+    :alt: Github Build Status
+    :target: https://github.com/inducer/gmsh_interop/actions?query=branch%3Amain+workflow%3ACI
+.. image:: https://badge.fury.io/py/gmsh_interop.png
+    :alt: Python Package Index Release Page
+    :target: https://pypi.org/project/gmsh_interop/
+
+This package allows Python to interoperate with the `gmsh <http://gmsh.info/>`_
+mesh generator.
+
+This package contains:
+
+* ``gmsh_interop.reader`` to read gmsh's ``.msh`` file format.
+* ``gmsh_interop.runner`` to run gmsh under program control and process its output.
+
+Its contents was extracted from `meshpy <https://github.com/inducer/meshpy>`__
+to escape its obnoxious licensing.
+
+Links:
+
+* `Github <https://github.com/inducer/gmsh_interop>`_
+* `Python package index <https://pypi.org/project/gmsh_interop/>`_
+* `Documentation <https://documen.tician.de/gmsh_interop>`_
```

### Comparing `gmsh_interop-2021.1.1/README.rst` & `gmsh_interop-2024.1/README.rst`

 * *Files identical despite different names*

### Comparing `gmsh_interop-2021.1.1/doc/Makefile` & `gmsh_interop-2024.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gmsh_interop-2021.1.1/doc/index.rst` & `gmsh_interop-2024.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `gmsh_interop-2021.1.1/doc/make.bat` & `gmsh_interop-2024.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gmsh_interop-2021.1.1/gmsh_interop/node_tuples.py` & `gmsh_interop-2024.1/gmsh_interop/node_tuples.py`

 * *Files identical despite different names*

### Comparing `gmsh_interop-2021.1.1/gmsh_interop/reader.py` & `gmsh_interop-2024.1/gmsh_interop/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,20 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-from functools import reduce
-
 import numpy as np
-#import numpy.linalg as la
-from pytools import memoize_method, Record
-from gmsh_interop.runner import (  # noqa
-        ScriptSource, LiteralSource, FileSource, ScriptWithFilesSource)
+
+from pytools import memoize_method
+
+from gmsh_interop.runner import (  # noqa: F401
+    FileSource, LiteralSource, ScriptSource, ScriptWithFilesSource)
 
 
 __doc__ = """
 .. exception:: GmshFileFormatError
 
 Element types
 -------------
@@ -100,16 +99,15 @@
 def generate_triangle_volume_tuples(order):
     for i in range(1, order):
         for j in range(1, order-i):
             yield (j, i)
 
 
 def generate_quad_vertex_tuples(dim, order):
-    from pytools import \
-            generate_nonnegative_integer_tuples_below
+    from pytools import generate_nonnegative_integer_tuples_below
     for tup in generate_nonnegative_integer_tuples_below(2, dim):
         yield tuple(order * i for i in tup)
 
 
 class LineFeeder:
     def __init__(self, line_iterable):
         self.line_iterable = iter(line_iterable)
@@ -191,24 +189,25 @@
 class GmshSimplexElementBase(GmshElementBase):
     def vertex_count(self):
         return self.dimensions + 1
 
     @memoize_method
     def node_count(self):
         """Return the number of interpolation nodes in this element."""
-        d = self.dimensions
-        o = self.order
+        import math
+        from functools import reduce
         from operator import mul
-        from pytools import factorial
-        return int(reduce(mul, (o + 1 + i for i in range(d)), 1) / factorial(d))
+        return (
+                reduce(mul, (self.order + 1 + i for i in range(self.dimensions)), 1)
+                // math.factorial(self.dimensions))
 
     @memoize_method
     def lexicographic_node_tuples(self):
-        from pytools import \
-                generate_nonnegative_integer_tuples_summing_to_at_most as gnitstam
+        from pytools import (
+            generate_nonnegative_integer_tuples_summing_to_at_most as gnitstam)
         result = list(gnitstam(self.order, self.dimensions))
 
         assert len(result) == self.node_count()
         return result
 
 
 class GmshPoint(GmshSimplexElementBase):
@@ -304,15 +303,19 @@
     def lexicographic_node_tuples(self):
         """Generate tuples enumerating the node indices present
         in this element. Each tuple has a length equal to the dimension
         of the element. The tuples constituents are non-negative integers
         whose sum is less than or equal to the order of the element.
         """
         from pytools import generate_nonnegative_integer_tuples_below as gnitb
-        result = list(gnitb(self.order + 1, self.dimensions))
+
+        # gnitb(2, 2) gives [(0, 0), (0, 1), (1, 0), (1, 1)]
+        # We want the x-coordinate to increase first, so reverse.
+        # (This is also consistent with gnitstam.)
+        result = [tup[::-1] for tup in gnitb(self.order + 1, self.dimensions)]
 
         assert len(result) == self.node_count()
         return result
 
 
 class GmshQuadrilateralElement(GmshTensorProductElementBase):
     dimensions = 2
@@ -491,25 +494,26 @@
         mesh_file.close()
 
     return result
 
 
 def generate_gmsh(receiver, source, dimensions=None, order=None, other_options=(),
             extension="geo", gmsh_executable="gmsh", force_dimension=None,
-            output_file_name=None, save_tmp_files_in=None):
+            target_unit=None, output_file_name=None, save_tmp_files_in=None):
     """Run gmsh and feed the output to *receiver*.
 
     :arg receiver: a class that implements the :class:`GmshMeshReceiverBase`
         interface.
     :arg source: an instance of :class:`ScriptSource` or :class:`FileSource`.
     """
     from gmsh_interop.runner import GmshRunner
     runner = GmshRunner(source, dimensions, order=order,
             other_options=other_options, extension=extension,
             gmsh_executable=gmsh_executable,
+            target_unit=target_unit,
             output_file_name=output_file_name,
             save_tmp_files_in=save_tmp_files_in)
 
     runner.__enter__()
     try:
         result = parse_gmsh(receiver, runner.output_file,
                 force_dimension=force_dimension)
@@ -524,22 +528,18 @@
     :arg receiver: this object will be fed the entities encountered in
         reading the GMSH file. See :class:`GmshMeshReceiverBase` for the
         interface this object needs to conform to.
     :arg line_iterable: an iterable that generates the lines of the GMSH file.
     :arg force_dimension: if not *None*, truncate point coordinates to this
         many dimensions.
     """
-
     feeder = LineFeeder(line_iterable)
 
     # collect the mesh information
 
-    class ElementInfo(Record):
-        pass
-
     while feeder.has_next_line():
         next_line = feeder.get_next_line()
         if not next_line.startswith("$"):
             raise GmshFileFormatError(
                     f"expected start of section, '{next_line}' found instead")
 
         section_name = next_line[1:]
```

### Comparing `gmsh_interop-2021.1.1/gmsh_interop/runner.py` & `gmsh_interop-2024.1/gmsh_interop/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,25 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-from pytools import memoize_method
+try:
+    from packaging.version import Version
+except ImportError:
+    from distutils.version import Version
 
 import logging
+from typing import Optional
+
+from pytools import memoize_method
+
+
 logger = logging.getLogger(__name__)
 
 
 __doc__ = """
 .. exception:: GmshError
 .. autoclass:: ScriptSource
 .. autoclass:: FileSource
@@ -42,15 +50,15 @@
 class GmshError(RuntimeError):
     pass
 
 
 # {{{ tools
 
 def _erase_dir(dir):
-    from os import listdir, unlink, rmdir
+    from os import listdir, rmdir, unlink
     from os.path import join
     for name in listdir(dir):
         unlink(join(dir, name))
     rmdir(dir)
 
 
 class _TempDirManager:
@@ -113,14 +121,41 @@
     """
     def __init__(self, source, filenames, source_name="temp.geo"):
         self.source = source
         self.source_name = source_name
         self.filenames = filenames
 
 
+def get_gmsh_version(executable: str = "gmsh") -> Optional[Version]:
+    import re
+    re_version = re.compile(r"[0-9]+.[0-9]+.[0-9]+")
+
+    def get_gmsh_version_from_string(output: str) -> Optional[Version]:
+        result = re_version.search(output)
+
+        try_version = None
+        if result is not None:
+            try_version = Version(result.group())
+
+        return try_version
+
+    from pytools.prefork import call_capture_output
+    retcode, stdout, stderr = call_capture_output([executable, "-version"])
+
+    # NOTE: gmsh has changed how it displays its version over the years, with
+    # it being displayed both on stderr and stdout -- so we try to cover it all!
+    version = None
+    if retcode == 0:
+        version = get_gmsh_version_from_string(stdout.decode().strip())
+        if version is None:
+            version = get_gmsh_version_from_string(stderr.decode().strip())
+
+    return version
+
+
 class GmshRunner:
     def __init__(self, source, dimensions=None, order=None,
             incomplete_elements=None, other_options=(),
             extension="geo", gmsh_executable="gmsh",
             output_file_name=None,
             target_unit=None,
             save_tmp_files_in=None):
@@ -156,39 +191,26 @@
 
         if self.target_unit not in ["M", "MM"]:
             raise RuntimeError("units must be 'M' (meters) or 'MM' (millimeters)")
 
     @property
     @memoize_method
     def version(self):
-        from distutils.version import LooseVersion
-        cmdline = [
-                self.gmsh_executable,
-                "-version"
-                ]
-
-        from pytools.prefork import call_capture_output
-        retcode, stdout, stderr = call_capture_output(cmdline)
-
-        if stderr:
-            output = stderr.decode().strip()
-        else:
-            output = stdout.decode().strip()
-
-        # stderr can contain irregular info
-        import re
-        version = re.search(r"[0-9]+.[0-9]+.[0-9]+", output).group()
-        return LooseVersion(version)
+        result = get_gmsh_version(self.gmsh_executable)
+        if result is None:
+            raise AttributeError("version")
+
+        return result
 
     def __enter__(self):
         self.temp_dir_mgr = None
         temp_dir_mgr = _TempDirManager()
         try:
             working_dir = temp_dir_mgr.path
-            from os.path import join, abspath, exists
+            from os.path import abspath, exists, join
 
             if isinstance(self.source, ScriptSource):
                 source_file_name = join(
                         working_dir, "temp."+self.source.extension)
                 with open(source_file_name, "w") as source_file:
                     source_file.write(self.source.source)
 
@@ -227,15 +249,15 @@
                     "-o", self.output_file_name,
                     "-nopopup",
                     "-format", "msh2",
                     ]
 
             # NOTE: handle unit incompatibility introduced in GMSH4
             # https://gitlab.onelab.info/gmsh/gmsh/issues/397
-            if self.version < "4.0.0":
+            if self.version < Version("4.0.0"):
                 if self.target_unit == "M":
                     cmdline.extend(["-setnumber", "Geometry.OCCScaling", "1000"])
             else:
                 cmdline.extend(["-setstring",
                     "Geometry.OCCTargetUnit", self.target_unit])
 
             if self.dimensions is not None:
@@ -292,16 +314,16 @@
                     msg += stdout+"\n"
                 msg += stderr+"\n"
                 warn(msg)
 
             self.output_file = open(output_file_name)
 
             if self.save_tmp_files_in:
-                import shutil
                 import errno
+                import shutil
                 try:
                     shutil.copytree(working_dir, self.save_tmp_files_in)
                 except FileExistsError:
                     import select
                     import sys
                     print(f"{self.save_tmp_files_in} exists! "
                         "Overwrite? (Y/N, will default to Y in 10sec).")
```

### Comparing `gmsh_interop-2021.1.1/gmsh_interop.egg-info/PKG-INFO` & `gmsh_interop-2024.1/gmsh_interop.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,15 @@
-Metadata-Version: 1.2
-Name: gmsh-interop
-Version: 2021.1.1
+Metadata-Version: 2.1
+Name: gmsh_interop
+Version: 2024.1
 Summary: A parser for GMSH's .msh format
 Home-page: http://github.com/inducer/gmsh_interop
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
-Description: Interoperability between Python and Gmsh
-        ========================================
-        
-        .. image:: https://gitlab.tiker.net/inducer/gmsh_interop/badges/main/pipeline.svg
-            :alt: Gitlab Build Status
-            :target: https://gitlab.tiker.net/inducer/gmsh_interop/commits/main
-        .. image:: https://github.com/inducer/gmsh_interop/workflows/CI/badge.svg
-            :alt: Github Build Status
-            :target: https://github.com/inducer/gmsh_interop/actions?query=branch%3Amain+workflow%3ACI
-        .. image:: https://badge.fury.io/py/gmsh_interop.png
-            :alt: Python Package Index Release Page
-            :target: https://pypi.org/project/gmsh_interop/
-        
-        This package allows Python to interoperate with the `gmsh <http://gmsh.info/>`_
-        mesh generator.
-        
-        This package contains:
-        
-        * ``gmsh_interop.reader`` to read gmsh's ``.msh`` file format.
-        * ``gmsh_interop.runner`` to run gmsh under program control and process its output.
-        
-        Its contents was extracted from `meshpy <https://github.com/inducer/meshpy>`__
-        to escape its obnoxious licensing.
-        
-        Links:
-        
-        * `Github <https://github.com/inducer/gmsh_interop>`_
-        * `Python package index <https://pypi.org/project/gmsh_interop/>`_
-        * `Documentation <https://documen.tician.de/gmsh_interop>`_
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
@@ -50,8 +19,42 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.6
+Requires-Python: ~=3.8
+License-File: LICENSE
+Requires-Dist: numpy>=1.6.0
+Requires-Dist: pytools
+Requires-Dist: packaging>=20.0
+
+Interoperability between Python and Gmsh
+========================================
+
+.. image:: https://gitlab.tiker.net/inducer/gmsh_interop/badges/main/pipeline.svg
+    :alt: Gitlab Build Status
+    :target: https://gitlab.tiker.net/inducer/gmsh_interop/commits/main
+.. image:: https://github.com/inducer/gmsh_interop/workflows/CI/badge.svg
+    :alt: Github Build Status
+    :target: https://github.com/inducer/gmsh_interop/actions?query=branch%3Amain+workflow%3ACI
+.. image:: https://badge.fury.io/py/gmsh_interop.png
+    :alt: Python Package Index Release Page
+    :target: https://pypi.org/project/gmsh_interop/
+
+This package allows Python to interoperate with the `gmsh <http://gmsh.info/>`_
+mesh generator.
+
+This package contains:
+
+* ``gmsh_interop.reader`` to read gmsh's ``.msh`` file format.
+* ``gmsh_interop.runner`` to run gmsh under program control and process its output.
+
+Its contents was extracted from `meshpy <https://github.com/inducer/meshpy>`__
+to escape its obnoxious licensing.
+
+Links:
+
+* `Github <https://github.com/inducer/gmsh_interop>`_
+* `Python package index <https://pypi.org/project/gmsh_interop/>`_
+* `Documentation <https://documen.tician.de/gmsh_interop>`_
```

### Comparing `gmsh_interop-2021.1.1/setup.py` & `gmsh_interop-2024.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,18 +29,19 @@
           "Topic :: Scientific/Engineering :: Information Analysis",
           "Topic :: Scientific/Engineering :: Mathematics",
           "Topic :: Scientific/Engineering :: Visualization",
           "Topic :: Software Development :: Libraries",
           "Topic :: Utilities",
           ],
 
-      python_requires="~=3.6",
+      python_requires="~=3.8",
       install_requires=[
           "numpy>=1.6.0",
           "pytools",
+          "packaging>=20.0",
           ],
 
       author="Andreas Kloeckner",
       url="http://github.com/inducer/gmsh_interop",
       author_email="inform@tiker.net",
       license="MIT",
       packages=find_packages())
```

### Comparing `gmsh_interop-2021.1.1/test/test_gmsh.py` & `gmsh_interop-2024.1/test/test_gmsh.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 # {{{ gmsh
 
 def search_on_path(filenames):
     """Find file on system path."""
     # http://aspn.activestate.com/ASPN/Cookbook/Python/Recipe/52224
 
-    from os.path import exists, abspath, join
-    from os import pathsep, environ
+    from os import environ, pathsep
+    from os.path import abspath, exists, join
 
     search_path = environ["PATH"]
 
     paths = search_path.split(pathsep)
     for path in paths:
         for filename in filenames:
             if exists(join(path, filename)):
@@ -106,49 +106,67 @@
         pytest.skip("gmsh executable not found")
 
     if visualize:
         save_tmp_files_in = f"simplex_{order}_{dim}d"
     else:
         save_tmp_files_in = None
 
-    from gmsh_interop.reader import generate_gmsh, GmshMeshReceiverBase
+    from gmsh_interop.reader import GmshMeshReceiverBase, generate_gmsh
     from gmsh_interop.runner import ScriptSource
 
     mr = GmshMeshReceiverBase()
     source = ScriptSource(GMSH_SPHERE, "geo")
-    generate_gmsh(mr, source, dimensions=dim, order=order,
+    generate_gmsh(mr, source, dimensions=dim, order=order, target_unit="MM",
             save_tmp_files_in=save_tmp_files_in)
 
 
 @pytest.mark.parametrize("dim", [2, 3])
 @pytest.mark.parametrize("order", [1, 3])
 def test_quad_gmsh(dim, order, visualize=False):
     if search_on_path(["gmsh"]) is None:
         pytest.skip("gmsh executable not found")
 
     if visualize:
         save_tmp_files_in = f"simplex_{order}_{dim}d"
     else:
         save_tmp_files_in = None
 
-    from gmsh_interop.reader import generate_gmsh, GmshMeshReceiverBase
+    from gmsh_interop.reader import GmshMeshReceiverBase, generate_gmsh
     from gmsh_interop.runner import ScriptSource
 
     if dim == 2:
         source = ScriptSource(GMSH_QUAD_SPHERE, "geo")
     else:
         source = ScriptSource(GMSH_QUAD_CUBE, "geo")
 
     mr = GmshMeshReceiverBase()
     generate_gmsh(mr, source, dimensions=dim, order=order,
             save_tmp_files_in=save_tmp_files_in)
 
 # }}}
 
 
+def test_lex_node_ordering():
+    """Check that lex nodes go through axes 'in order', i.e. that the
+    r-axis is the first one to become non-zero, then s, then t.
+    """
+    from gmsh_interop.reader import _gmsh_supported_element_type_map
+
+    for el in _gmsh_supported_element_type_map().values():
+        axis_nonzero_order = []
+
+        for node in el.lexicographic_node_tuples():
+            nonzero_axes = {i for i, ni in enumerate(node) if ni}
+            for nzax in sorted(nonzero_axes):
+                if nzax not in axis_nonzero_order:
+                    axis_nonzero_order.append(nzax)
+
+        assert axis_nonzero_order == list(range(el.dimensions))
+
+
 if __name__ == "__main__":
     import sys
     if len(sys.argv) > 1:
         exec(sys.argv[1])
     else:
         pytest.main([__file__])
```

