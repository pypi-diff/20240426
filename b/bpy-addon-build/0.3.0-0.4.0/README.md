# Comparing `tmp/bpy_addon_build-0.3.0.tar.gz` & `tmp/bpy_addon_build-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpy_addon_build-0.3.0.tar", max compression
+gzip compressed data, was "bpy_addon_build-0.4.0.tar", max compression
```

## Comparing `bpy_addon_build-0.3.0.tar` & `bpy_addon_build-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,14 @@
--rw-r--r--   0        0        0     1048 2023-12-24 21:29:15.929958 bpy_addon_build-0.3.0/bpy_addon_build/__init__.py
--rw-r--r--   0        0        0     4339 2023-12-26 21:34:44.895579 bpy_addon_build-0.3.0/bpy_addon_build/args.py
--rw-r--r--   0        0        0     5466 2024-01-12 15:11:59.203231 bpy_addon_build-0.3.0/bpy_addon_build/build_context.py
--rw-r--r--   0        0        0     1296 2023-12-26 21:15:30.886065 bpy_addon_build-0.3.0/bpy_addon_build/config.py
--rw-r--r--   0        0        0      608 2023-12-24 21:34:36.857883 bpy_addon_build-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 bpy_addon_build-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1499 2024-04-18 13:43:17.154076 bpy_addon_build-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2931 2024-04-26 18:27:46.167616 bpy_addon_build-0.4.0/bpy_addon_build/__init__.py
+-rw-r--r--   0        0        0     2421 2024-04-26 18:27:46.167616 bpy_addon_build-0.4.0/bpy_addon_build/api/__init__.py
+-rw-r--r--   0        0        0     4362 2024-04-26 18:27:46.167616 bpy_addon_build-0.4.0/bpy_addon_build/args.py
+-rw-r--r--   0        0        0        1 2024-04-18 13:43:17.154076 bpy_addon_build-0.4.0/bpy_addon_build/build_context/__init__.py
+-rw-r--r--   0        0        0     2095 2024-04-26 18:27:46.167616 bpy_addon_build-0.4.0/bpy_addon_build/build_context/build.py
+-rw-r--r--   0        0        0     1083 2024-04-26 18:27:46.167616 bpy_addon_build-0.4.0/bpy_addon_build/build_context/core.py
+-rw-r--r--   0        0        0     6783 2024-04-26 18:27:46.167616 bpy_addon_build-0.4.0/bpy_addon_build/build_context/hook_definitions.py
+-rw-r--r--   0        0        0     1595 2024-04-26 18:27:46.167616 bpy_addon_build-0.4.0/bpy_addon_build/build_context/hooks.py
+-rw-r--r--   0        0        0     1706 2024-04-26 18:27:46.167616 bpy_addon_build-0.4.0/bpy_addon_build/build_context/install.py
+-rw-r--r--   0        0        0     1296 2024-04-26 18:27:46.167616 bpy_addon_build-0.4.0/bpy_addon_build/config.py
+-rw-r--r--   0        0        0      491 2024-04-26 18:27:46.167616 bpy_addon_build-0.4.0/bpy_addon_build/util.py
+-rw-r--r--   0        0        0      658 2024-04-26 18:34:21.615079 bpy_addon_build-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 bpy_addon_build-0.4.0/PKG-INFO
```

### Comparing `bpy_addon_build-0.3.0/bpy_addon_build/args.py` & `bpy_addon_build-0.4.0/bpy_addon_build/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import argparse
 from pathlib import Path
 from typing import List, Optional, cast
 from attrs import define, field, Attribute
 
 
 # Must be ignored to pass Mypy as this has
 # an expression of Any, likely due to how
@@ -37,35 +36,35 @@
     path: Path = field(default=Path("bpy-build.yaml"))
     versions: List[float] = field(default=[])
     actions: List[str] = field(default=["default"])
     debug_mode: bool = field(default=False)
     supress_messages: bool = field(default=False)
 
     @path.validator
-    def path_validate(self, _: Attribute, value: Path) -> None:
+    def path_validate(self, _: Attribute, value: Optional[Path]) -> None:
         # Assume the user did not pass
         # a path in
         if value is None:
             return
         if not value.exists():
-            raise FileNotFoundError("File does not exist!")
+            raise FileNotFoundError(f"File {value} does not exist!")
         if value.is_dir():
             raise IsADirectoryError("Expected a file, got a direcory!")
 
     @versions.validator
-    def version_validate(self, _: Attribute, value: List[float]) -> None:
+    def version_validate(self, _: Attribute, value: Optional[List[float]]) -> None:
         if value is None:
             self.versions = []
         else:
             for ver in value:
                 if not isinstance(ver, float):
                     raise ValueError("Expected List of floating point values!")
 
     @actions.validator
-    def actions_validate(self, _: Attribute, value: List[str]) -> None:
+    def actions_validate(self, _: Attribute, value: Optional[List[str]]) -> None:
         if value is None:
             self.actions = ["default"]
         else:
             for act in value:
                 if not isinstance(act, str):
                     raise ValueError("Expect List of strings!")
```

### Comparing `bpy_addon_build-0.3.0/bpy_addon_build/config.py` & `bpy_addon_build-0.4.0/bpy_addon_build/config.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.3.0/pyproject.toml` & `bpy_addon_build-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "bpy-addon-build"
-version = "0.3.0"
+version = "0.4.0"
 description = "A build system to make building and testing Blender addons 10 times easier"
 authors = ["StandingPad"]
-license = "MIT"
+license = "BSD-3-Clause"
 homepage = "https://github.com/StandingPadAnimations/bpy-build"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 attrs = "^23.1.0"
 pyyaml = "^6.0.1"
 cattrs = "^23.2.3"
 rich = "^13.7.0"
+typeguard = "^4.1.5"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
 mypy = "^1.4.1"
 types-pyyaml = "^6.0.12.11"
+ruff = "^0.3.4"
+gitpython = "^3.1.43"
 
 [tool.poetry.scripts]
 bab = "bpy_addon_build:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bpy_addon_build-0.3.0/PKG-INFO` & `bpy_addon_build-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: bpy-addon-build
-Version: 0.3.0
+Version: 0.4.0
 Summary: A build system to make building and testing Blender addons 10 times easier
 Home-page: https://github.com/StandingPadAnimations/bpy-build
-License: MIT
+License: BSD-3-Clause
 Author: StandingPad
 Requires-Python: >=3.8
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: cattrs (>=23.2.3,<24.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: typeguard (>=4.1.5,<5.0.0)
```

