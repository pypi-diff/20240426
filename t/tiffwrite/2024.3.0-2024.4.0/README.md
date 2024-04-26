# Comparing `tmp/tiffwrite-2024.3.0.tar.gz` & `tmp/tiffwrite-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiffwrite-2024.3.0.tar", max compression
+gzip compressed data, was "tiffwrite-2024.4.0.tar", max compression
```

## Comparing `tiffwrite-2024.3.0.tar` & `tiffwrite-2024.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2022-05-12 07:11:33.746847 tiffwrite-2024.3.0/LICENSE
--rw-r--r--   0        0        0     4492 2024-03-27 14:52:29.020886 tiffwrite-2024.3.0/README.md
--rw-r--r--   0        0        0      854 2024-03-27 14:56:38.832900 tiffwrite-2024.3.0/pyproject.toml
--rwxr-xr-x   0        0        0    27519 2024-03-27 14:46:22.500865 tiffwrite-2024.3.0/tiffwrite/__init__.py
--rw-r--r--   0        0        0     5398 1970-01-01 00:00:00.000000 tiffwrite-2024.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-05-12 07:11:33.746847 tiffwrite-2024.4.0/LICENSE
+-rw-r--r--   0        0        0     4492 2024-03-27 15:03:27.356924 tiffwrite-2024.4.0/README.md
+-rw-r--r--   0        0        0      895 2024-04-26 12:05:39.947361 tiffwrite-2024.4.0/pyproject.toml
+-rwxr-xr-x   0        0        0    27588 2024-04-26 12:04:53.199390 tiffwrite-2024.4.0/tiffwrite/__init__.py
+-rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 tiffwrite-2024.4.0/PKG-INFO
```

### Comparing `tiffwrite-2024.3.0/LICENSE` & `tiffwrite-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiffwrite-2024.3.0/README.md` & `tiffwrite-2024.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Mypy](https://github.com/wimpomp/tiffwrite/actions/workflows/mypy.yml/badge.svg)](https://github.com/wimpomp/tiffwrite/actions/workflows/mypy.yml)
+[![mypy](https://github.com/wimpomp/tiffwrite/actions/workflows/mypy.yml/badge.svg)](https://github.com/wimpomp/tiffwrite/actions/workflows/mypy.yml)
 [![pytest](https://github.com/wimpomp/tiffwrite/actions/workflows/pytest.yml/badge.svg)](https://github.com/wimpomp/tiffwrite/actions/workflows/pytest.yml)
 
 # Tiffwrite
 Exploiting [tifffile](https://pypi.org/project/tifffile/) in parallel to write BioFormats/ImageJ compatible tiffs with
 good compression.
 
 ## Features
```

### Comparing `tiffwrite-2024.3.0/pyproject.toml` & `tiffwrite-2024.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tiffwrite"
-version = "2024.3.0"
+version = "2024.4.0"
 description = "Parallel tiff writer compatible with ImageJ."
 authors = ["Wim Pomp, Lenstra lab NKI <w.pomp@nki.nl>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "tiffwrite"}]
 repository = "https://github.com/wimpomp/tiffwrite"
 
@@ -12,16 +12,17 @@
 python = "^3.10"
 tifffile = "*"
 imagecodecs = "*"
 numpy = "*"
 tqdm = "*"
 colorcet = "*"
 matplotlib = "*"
-parfor = ">=2023.10.1"
+parfor = ">=2024.3.0"
 pytest = { version = "*", optional = true }
+mypy = { version = "*", optional = true }
 
 [tool.poetry.extras]
 test = ["pytest", "mypy"]
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore:::(?!tiffwrite)"]
```

### Comparing `tiffwrite-2024.3.0/tiffwrite/__init__.py` & `tiffwrite-2024.4.0/tiffwrite/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,15 @@
         desc_bytes = [bytes(d, 'ascii') for d in desc]
         if self.comment is not None:
             desc_bytes.append(b'')
             if isinstance(self.comment, bytes):
                 desc_bytes.append(self.comment)
             else:
                 desc_bytes.append(bytes(self.comment, 'ascii'))
-        return b'\n'.join(desc_bytes)
+        return b'\n'.join(desc_bytes) + b'\0'
 
     @cached_property
     def colormap_bytes(self) -> Optional[bytes]:
         if self.colormap:
             colormap = getattr(colorcet, self.colormap)
             colormap[0] = '#ffffff'
             colormap[-1] = '#000000'
@@ -481,21 +481,22 @@
                 ifds[framenr], strips[(framenr, channel)] = self.pool[n]
 
             self.pool.close()
             with self.fh.lock() as fh:  # noqa
                 for n, tags in self.frame_extra_tags.items():
                     framenr, channel = self.get_frame_number(n)
                     ifds[framenr].update(tags)
-                if self.colormap is not None:
+                if 0 in ifds and self.colormap is not None:
                     ifds[0][320] = Tag('SHORT', self.colormap_bytes)
                     ifds[0][262] = Tag('SHORT', 3)
                 if self.colors is not None:
                     for c, color in enumerate(self.colors_bytes):
-                        ifds[c][320] = Tag('SHORT', color)
-                        ifds[c][262] = Tag('SHORT', 3)
+                        if c in ifds:
+                            ifds[c][320] = Tag('SHORT', color)
+                            ifds[c][262] = Tag('SHORT', 3)
                 if 0 in ifds and 306 not in ifds[0]:
                     ifds[0][306] = Tag('ASCII', datetime.now().strftime('%Y:%m:%d %H:%M:%S'))
                 wrn = False
                 for framenr in range(self.nframes):
                     if framenr in ifds and all([(framenr, channel) in strips for channel in range(self.spp)]):
                         stripbyteoffsets, stripbytecounts = zip(*[strips[(framenr, channel)]
                                                                   for channel in range(self.spp)])
@@ -514,15 +515,15 @@
                             ifds[framenr].write_offset(ifds[framenr - 1].where_to_write_next_ifd_offset)
                         else:
                             ifds[framenr].write_offset(self.header.offset - self.header.offsetsize)
                     else:
                         wrn = True
                 if wrn:
                     warnings.warn('Some frames were not added to the tif file, either you forgot them, '
-                                  'or an error occured and the tif file was closed prematurely.')
+                                  'or an error occurred and the tif file was closed prematurely.')
 
     def __enter__(self) -> IJTiffFile:
         return self
 
     def __exit__(self, *args: Any, **kwargs: Any) -> None:
         self.close()
```

### Comparing `tiffwrite-2024.3.0/PKG-INFO` & `tiffwrite-2024.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiffwrite
-Version: 2024.3.0
+Version: 2024.4.0
 Summary: Parallel tiff writer compatible with ImageJ.
 Home-page: https://github.com/wimpomp/tiffwrite
 License: GPL-3.0-or-later
 Author: Wim Pomp, Lenstra lab NKI
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -12,23 +12,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: test
 Requires-Dist: colorcet
 Requires-Dist: imagecodecs
 Requires-Dist: matplotlib
+Requires-Dist: mypy ; extra == "test"
 Requires-Dist: numpy
-Requires-Dist: parfor (>=2023.10.1)
+Requires-Dist: parfor (>=2024.3.0)
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: tifffile
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/wimpomp/tiffwrite
 Description-Content-Type: text/markdown
 
-[![Mypy](https://github.com/wimpomp/tiffwrite/actions/workflows/mypy.yml/badge.svg)](https://github.com/wimpomp/tiffwrite/actions/workflows/mypy.yml)
+[![mypy](https://github.com/wimpomp/tiffwrite/actions/workflows/mypy.yml/badge.svg)](https://github.com/wimpomp/tiffwrite/actions/workflows/mypy.yml)
 [![pytest](https://github.com/wimpomp/tiffwrite/actions/workflows/pytest.yml/badge.svg)](https://github.com/wimpomp/tiffwrite/actions/workflows/pytest.yml)
 
 # Tiffwrite
 Exploiting [tifffile](https://pypi.org/project/tifffile/) in parallel to write BioFormats/ImageJ compatible tiffs with
 good compression.
 
 ## Features
```

