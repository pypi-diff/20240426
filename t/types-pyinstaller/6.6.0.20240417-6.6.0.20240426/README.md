# Comparing `tmp/types-pyinstaller-6.6.0.20240417.tar.gz` & `tmp/types-pyinstaller-6.6.0.20240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyinstaller-6.6.0.20240417.tar", last modified: Wed Apr 17 02:17:22 2024, max compression
+gzip compressed data, was "types-pyinstaller-6.6.0.20240426.tar", last modified: Fri Apr 26 02:17:52 2024, max compression
```

## Comparing `types-pyinstaller-6.6.0.20240417.tar` & `types-pyinstaller-6.6.0.20240426.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.561383 types-pyinstaller-6.6.0.20240417/
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-17 02:17:22.561383 types-pyinstaller-6.6.0.20240417/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.557383 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/__main__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.557383 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/building/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/building/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/building/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/building/build_main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/building/datastruct.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/building/splash.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.557383 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/depend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/depend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/depend/analysis.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/depend/imphookapi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.557383 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/isolated/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/isolated/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/isolated/_parent.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.557383 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/lib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.561383 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/lib/modulegraph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/lib/modulegraph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.561383 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.561383 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/utils/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/utils/hooks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/utils/hooks/conda.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.561383 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/utils/win32/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/utils/win32/versioninfo.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.561383 types-pyinstaller-6.6.0.20240417/pyi_splash-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/pyi_splash-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-17 02:16:41.000000 types-pyinstaller-6.6.0.20240417/pyi_splash-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/pyi_splash-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:17:22.561383 types-pyinstaller-6.6.0.20240417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:22.561383 types-pyinstaller-6.6.0.20240417/types_pyinstaller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/types_pyinstaller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/types_pyinstaller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/types_pyinstaller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/types_pyinstaller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 02:17:22.000000 types-pyinstaller-6.6.0.20240417/types_pyinstaller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.728155 types-pyinstaller-6.6.0.20240426/
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-26 02:17:51.000000 types-pyinstaller-6.6.0.20240426/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 02:17:51.000000 types-pyinstaller-6.6.0.20240426/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-26 02:17:52.728155 types-pyinstaller-6.6.0.20240426/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.724156 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-26 02:17:51.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/__main__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.724156 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/building/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/building/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/building/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/building/build_main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/building/datastruct.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/building/splash.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.724156 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/depend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/depend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/depend/analysis.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/depend/imphookapi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.724156 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/isolated/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/isolated/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/isolated/_parent.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.724156 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/lib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.728155 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/lib/modulegraph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/lib/modulegraph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:51.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.728155 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.728155 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/utils/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/utils/hooks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/utils/hooks/conda.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.728155 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/utils/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/utils/win32/versioninfo.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.728155 types-pyinstaller-6.6.0.20240426/pyi_splash-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-26 02:17:51.000000 types-pyinstaller-6.6.0.20240426/pyi_splash-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-26 02:17:42.000000 types-pyinstaller-6.6.0.20240426/pyi_splash-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:51.000000 types-pyinstaller-6.6.0.20240426/pyi_splash-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 02:17:52.728155 types-pyinstaller-6.6.0.20240426/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-26 02:17:51.000000 types-pyinstaller-6.6.0.20240426/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:17:52.728155 types-pyinstaller-6.6.0.20240426/types_pyinstaller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-26 02:17:52.000000 types-pyinstaller-6.6.0.20240426/types_pyinstaller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-26 02:17:52.000000 types-pyinstaller-6.6.0.20240426/types_pyinstaller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 02:17:52.000000 types-pyinstaller-6.6.0.20240426/types_pyinstaller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 02:17:52.000000 types-pyinstaller-6.6.0.20240426/types_pyinstaller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-26 02:17:52.000000 types-pyinstaller-6.6.0.20240426/types_pyinstaller.egg-info/top_level.txt
```

### Comparing `types-pyinstaller-6.6.0.20240417/CHANGELOG.md` & `types-pyinstaller-6.6.0.20240426/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 6.6.0.20240426 (2024-04-26)
+
+pyinstaller: allow `Splash(text_pos = None)` (#11835)
+
 ## 6.6.0.20240417 (2024-04-17)
 
 Remove remaining bare `Incomplete`s (#11768)
 
 Enable Y065
 
 ## 6.6.0.20240415 (2024-04-15)
```

### Comparing `types-pyinstaller-6.6.0.20240417/PKG-INFO` & `types-pyinstaller-6.6.0.20240426/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyinstaller
-Version: 6.6.0.20240417
+Version: 6.6.0.20240426
 Summary: Typing stubs for pyinstaller
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyinstaller.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-pyinstaller` aims to provide accurate annotations
 for `pyinstaller==6.6.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyinstaller. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `48a68f521ee1cb23a2aea43951a5000d2600d824` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
```

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/building/api.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/building/api.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/building/build_main.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/building/build_main.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/building/datastruct.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/building/datastruct.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/building/splash.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/building/splash.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     binaries: list[_TOCTuple]
     def __init__(
         self,
         image_file: StrPath,
         binaries: list[_TOCTuple],
         datas: list[_TOCTuple],
         *,
-        text_pos: tuple[int, int] = ...,
+        text_pos: tuple[int, int] | None = ...,
         text_size: int = 12,
         text_font: str = ...,
         text_color: str = "black",
         text_default: str = "Initializing",
         full_tk: bool = False,
         minify_script: bool = True,
         rundir: str = "__splash",
```

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/compat.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/depend/analysis.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/depend/analysis.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/depend/imphookapi.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/depend/imphookapi.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/isolated/_parent.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/isolated/_parent.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/utils/hooks/__init__.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/utils/hooks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/utils/hooks/conda.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/utils/hooks/conda.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/PyInstaller-stubs/utils/win32/versioninfo.pyi` & `types-pyinstaller-6.6.0.20240426/PyInstaller-stubs/utils/win32/versioninfo.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.6.0.20240417/setup.py` & `types-pyinstaller-6.6.0.20240426/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-pyinstaller` aims to provide accurate annotations
 for `pyinstaller==6.6.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyinstaller. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `48a68f521ee1cb23a2aea43951a5000d2600d824` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="6.6.0.20240417",
+      version="6.6.0.20240426",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyinstaller.md",
```

### Comparing `types-pyinstaller-6.6.0.20240417/types_pyinstaller.egg-info/PKG-INFO` & `types-pyinstaller-6.6.0.20240426/types_pyinstaller.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyinstaller
-Version: 6.6.0.20240417
+Version: 6.6.0.20240426
 Summary: Typing stubs for pyinstaller
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyinstaller.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-pyinstaller` aims to provide accurate annotations
 for `pyinstaller==6.6.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyinstaller. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `48a68f521ee1cb23a2aea43951a5000d2600d824` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
```

### Comparing `types-pyinstaller-6.6.0.20240417/types_pyinstaller.egg-info/SOURCES.txt` & `types-pyinstaller-6.6.0.20240426/types_pyinstaller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

