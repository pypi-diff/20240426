# Comparing `tmp/volcano_base-2.0.2.tar.gz` & `tmp/volcano_base-2.0.3.tar.gz`

## Comparing `volcano_base-2.0.2.tar` & `volcano_base-2.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 volcano_base-2.0.2/.mise.local.toml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 volcano_base-2.0.2/.mise.toml
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 volcano_base-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-2.0.2/.release-please-manifest.json
--rw-r--r--   0        0        0    20123 2020-02-02 00:00:00.000000 volcano_base-2.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-2.0.2/release-please-config.json
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 volcano_base-2.0.2/requirements-dev.lock
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 volcano_base-2.0.2/requirements.lock
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 volcano_base-2.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-2.0.2/.github/release-please/release-please-config.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-2.0.2/.github/release-please/release-please-manifest.json
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 volcano_base-2.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 volcano_base-2.0.2/assets/examples.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/__init__.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/config.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/down/__init__.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/down/cesm2.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/down/historic_so2.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/down/ob16.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/load/__init__.py
--rw-r--r--   0        0        0    24151 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/load/load_c2w_files.py
--rw-r--r--   0        0        0    31646 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/load/load_ob16.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/manipulate/__init__.py
--rw-r--r--   0        0        0    24511 2020-02-02 00:00:00.000000 volcano_base-2.0.2/src/volcano_base/manipulate/time_series.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 volcano_base-2.0.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 volcano_base-2.0.2/LICENSE
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 volcano_base-2.0.2/README.md
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 volcano_base-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 volcano_base-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 volcano_base-2.0.3/.mise.local.toml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 volcano_base-2.0.3/.mise.toml
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 volcano_base-2.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-2.0.3/.release-please-manifest.json
+-rw-r--r--   0        0        0    20537 2020-02-02 00:00:00.000000 volcano_base-2.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-2.0.3/release-please-config.json
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 volcano_base-2.0.3/requirements-dev.lock
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 volcano_base-2.0.3/requirements.lock
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 volcano_base-2.0.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-2.0.3/.github/release-please/release-please-config.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-2.0.3/.github/release-please/release-please-manifest.json
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 volcano_base-2.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 volcano_base-2.0.3/assets/examples.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/__init__.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/config.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/down/__init__.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/down/cesm2.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/down/historic_so2.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/down/ob16.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/load/__init__.py
+-rw-r--r--   0        0        0    24311 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/load/load_c2w_files.py
+-rw-r--r--   0        0        0    31646 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/load/load_ob16.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/manipulate/__init__.py
+-rw-r--r--   0        0        0    24511 2020-02-02 00:00:00.000000 volcano_base-2.0.3/src/volcano_base/manipulate/time_series.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 volcano_base-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 volcano_base-2.0.3/LICENSE
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 volcano_base-2.0.3/README.md
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 volcano_base-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 volcano_base-2.0.3/PKG-INFO
```

### Comparing `volcano_base-2.0.2/.mise.toml` & `volcano_base-2.0.3/.mise.toml`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/.pre-commit-config.yaml` & `volcano_base-2.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/CHANGELOG.md` & `volcano_base-2.0.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## [2.0.3](https://github.com/engeir/volcano-base/compare/v2.0.2...v2.0.3) (2024-04-26)
+
+
+### Bug Fixes
+
+* **FindFiles:** keep most recent was not removing all old files ([ea594a2](https://github.com/engeir/volcano-base/commit/ea594a2f91c62bcdaf151646c186b2bece19a828))
+
+
+### Build System
+
+* **deps:** update all ([8f01131](https://github.com/engeir/volcano-base/commit/8f011314b8b6008c4196823cb6fcdd2634d7f3b6))
+
 ## [2.0.2](https://github.com/engeir/volcano-base/compare/v2.0.1...v2.0.2) (2024-04-19)
 
 
 ### Bug Fixes
 
 * **cesm2 load:** use match group 'ensemble', since this matches with the data attrs ([51579ff](https://github.com/engeir/volcano-base/commit/51579ff59ea0733ed6ef3c8aab3e6210812afde4))
```

### Comparing `volcano_base-2.0.2/release-please-config.json` & `volcano_base-2.0.3/release-please-config.json`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/requirements-dev.lock` & `volcano_base-2.0.3/requirements-dev.lock`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     # via pydoclint
 cloudpickle==3.0.0
     # via dask
 contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
-dask==2024.4.1
+dask==2024.4.2
     # via volcano-base
 datetime==5.5
     # via volcano-base
 distlib==0.3.8
     # via virtualenv
 docstring-parser-fork==0.0.5
     # via pydoclint
@@ -44,15 +44,15 @@
     # via matplotlib
 fsspec==2024.3.1
     # via dask
 h5netcdf==1.3.0
     # via volcano-base
 h5py==3.11.0
     # via h5netcdf
-identify==2.5.35
+identify==2.5.36
     # via pre-commit
 idna==3.7
     # via requests
 iniconfig==2.0.0
     # via pytest
 kiwisolver==1.4.5
     # via matplotlib
@@ -61,15 +61,15 @@
 markdown-it-py==3.0.0
     # via rich
 matplotlib==3.8.4
     # via nc-time-axis
     # via volcano-base
 mdurl==0.1.2
     # via markdown-it-py
-mypy==1.9.0
+mypy==1.10.0
 mypy-extensions==1.0.0
     # via mypy
 nc-time-axis==1.4.1
 nodeenv==1.8.0
     # via pre-commit
 numpy==1.26.4
     # via cftime
@@ -89,23 +89,23 @@
     # via xarray
 pandas==2.2.2
     # via xarray
 partd==1.4.1
     # via dask
 pillow==10.3.0
     # via matplotlib
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 pre-commit==3.7.0
 pre-commit-hooks==4.6.0
-pydantic==2.7.0
+pydantic==2.7.1
     # via volcano-base
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pydoclint==0.4.1
 pydocstringformatter==0.7.3
 pygments==2.17.2
     # via rich
 pyparsing==3.1.2
     # via matplotlib
@@ -131,15 +131,15 @@
     # via volcano-base
 rich==13.7.1
     # via volcano-base
 ruamel-yaml==0.18.6
     # via pre-commit-hooks
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-ruff==0.4.0
+ruff==0.4.2
 scipy==1.13.0
     # via volcano-base
 six==1.16.0
     # via python-dateutil
 soupsieve==2.5
     # via beautifulsoup4
 tokenize-rt==5.2.0
@@ -154,15 +154,15 @@
     # via pydantic-core
     # via returns
 tzdata==2024.1
     # via pandas
 urllib3==2.2.1
     # via requests
     # via types-requests
-virtualenv==20.25.3
+virtualenv==20.26.0
     # via pre-commit
 xarray==2024.3.0
     # via volcano-base
 xdoctest==1.1.3
 zope-interface==6.3
     # via datetime
 setuptools==69.5.1
```

### Comparing `volcano_base-2.0.2/requirements.lock` & `volcano_base-2.0.3/requirements.lock`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # via dask
 cloudpickle==3.0.0
     # via dask
 contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
-dask==2024.4.1
+dask==2024.4.2
     # via volcano-base
 datetime==5.5
     # via volcano-base
 fonttools==4.51.0
     # via matplotlib
 fsspec==2024.3.1
     # via dask
@@ -66,17 +66,17 @@
     # via xarray
 pandas==2.2.2
     # via xarray
 partd==1.4.1
     # via dask
 pillow==10.3.0
     # via matplotlib
-pydantic==2.7.0
+pydantic==2.7.1
     # via volcano-base
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pygments==2.17.2
     # via rich
 pyparsing==3.1.2
     # via matplotlib
 python-dateutil==2.9.0.post0
     # via matplotlib
```

### Comparing `volcano_base-2.0.2/.github/release-please/release-please-config.json` & `volcano_base-2.0.3/.github/release-please/release-please-config.json`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/.github/workflows/release.yml` & `volcano_base-2.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/assets/examples.py` & `volcano_base-2.0.3/assets/examples.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/src/volcano_base/config.py` & `volcano_base-2.0.3/src/volcano_base/config.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/src/volcano_base/down/cesm2.py` & `volcano_base-2.0.3/src/volcano_base/down/cesm2.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/src/volcano_base/down/historic_so2.py` & `volcano_base-2.0.3/src/volcano_base/down/historic_so2.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/src/volcano_base/down/ob16.py` & `volcano_base-2.0.3/src/volcano_base/down/ob16.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/src/volcano_base/load/load_c2w_files.py` & `volcano_base-2.0.3/src/volcano_base/load/load_c2w_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -549,25 +549,30 @@
 
         This assumes that there is a sorting attribute named 'date' that is available.
         """
         if self._matched_files is None:
             return self
         sorting = self._sort_order
         reverse = self._sort_reverse
-        self = self.sort("date", reverse=True)
-        only_recent = []
-        last_file = ("",) * len(self.regex.groups)
-        if self._matched_files is None:
+        local_self = self.sort("date", reverse=True)
+        only_recent: list[tuple[str, ...]] = []
+        if local_self._matched_files is None:
             return self
-        for file in self._matched_files:
-            if last_file[:-1] != file[:-1]:
+        for file in local_self._matched_files:
+            tuple_exists = any(
+                file[:-1] == existing_tuple[:-1] for existing_tuple in only_recent
+            )
+            if not tuple_exists or not only_recent:
                 only_recent.append(file)
-                last_file = file
-        self._matched_files = only_recent
-        return self if sorting is None else self.sort(*sorting, reverse=reverse)
+        local_self._matched_files = only_recent
+        return (
+            local_self
+            if sorting is None
+            else local_self.sort(*sorting, reverse=reverse)
+        )
 
     def _re_create_file_paths(
         self,
         *found_files: tuple[str, ...],
         ft: str | None = None,
         check_existance: bool = True,
     ) -> list[pathlib.Path]:
```

### Comparing `volcano_base-2.0.2/src/volcano_base/load/load_ob16.py` & `volcano_base-2.0.3/src/volcano_base/load/load_ob16.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/src/volcano_base/manipulate/__init__.py` & `volcano_base-2.0.3/src/volcano_base/manipulate/__init__.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/src/volcano_base/manipulate/time_series.py` & `volcano_base-2.0.3/src/volcano_base/manipulate/time_series.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/.gitignore` & `volcano_base-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/LICENSE` & `volcano_base-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.2/README.md` & `volcano_base-2.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Core module for volcanic eruption simulation projects
 
-<sup>Latest version: v2.0.2</sup> <!-- x-release-please-version -->
+<sup>Latest version: v2.0.3</sup> <!-- x-release-please-version -->
 
 > [!WARNING]
 >
 > This README reflects the changes made to the main branch. For the most up to date
 > documentation about the version you are using, see the README at the relevant tag.
 
 This repository contains the core elements used across several independent volcanic
```

### Comparing `volcano_base-2.0.2/pyproject.toml` & `volcano_base-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "volcano-base"
-version = "2.0.2"
+version = "2.0.3"
 description = "Download, find and manipulate volcano and climate related time series"
 authors = [{ name = "engeir", email = "engeir@pm.me" }]
 license = "MIT"
 readme = "README.md"
 requires-python = ">= 3.12"
 dependencies = [
   "returns>=0.22.0",
```

### Comparing `volcano_base-2.0.2/PKG-INFO` & `volcano_base-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: volcano-base
-Version: 2.0.2
+Version: 2.0.3
 Summary: Download, find and manipulate volcano and climate related time series
 Author-email: engeir <engeir@pm.me>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.12
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: cftime>=1.6.3
@@ -19,15 +19,15 @@
 Requires-Dist: rich>=13.7.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: xarray>=2024.1.1
 Description-Content-Type: text/markdown
 
 # Core module for volcanic eruption simulation projects
 
-<sup>Latest version: v2.0.2</sup> <!-- x-release-please-version -->
+<sup>Latest version: v2.0.3</sup> <!-- x-release-please-version -->
 
 > [!WARNING]
 >
 > This README reflects the changes made to the main branch. For the most up to date
 > documentation about the version you are using, see the README at the relevant tag.
 
 This repository contains the core elements used across several independent volcanic
```

