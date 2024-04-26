# Comparing `tmp/empack-3.3.2.tar.gz` & `tmp/empack-3.3.3.tar.gz`

## Comparing `empack-3.3.2.tar` & `empack-3.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 empack-3.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 empack-3.3.2/CHANGELOG.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 empack-3.3.2/ci_env.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 empack-3.3.2/setup.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 empack-3.3.2/config/empack_config.yaml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 empack-3.3.2/empack/__init__.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 empack-3.3.2/empack/file_patterns.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 empack-3.3.2/empack/filter_env.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 empack-3.3.2/empack/micromamba_wrapper.py
--rw-r--r--   0        0        0    10213 2020-02-02 00:00:00.000000 empack-3.3.2/empack/pack.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 empack-3.3.2/empack/repodata.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 empack-3.3.2/empack/tar_utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 empack-3.3.2/empack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.3.2/empack/cli/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 empack-3.3.2/empack/cli/app.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 empack-3.3.2/empack/cli/err.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 empack-3.3.2/empack/cli/main.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 empack-3.3.2/empack/cli/pack.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 empack-3.3.2/empack/cli/repodata.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 empack-3.3.2/empack/cli/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.3.2/tests/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 empack-3.3.2/tests/conftest.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 empack-3.3.2/tests/empack_test_config.yaml
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 empack-3.3.2/tests/empack_test_extra_config.yaml
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 empack-3.3.2/tests/test_cli.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 empack-3.3.2/tests/test_filter.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 empack-3.3.2/tests/test_integration.py
--rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 empack-3.3.2/tests/test_pack.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 empack-3.3.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 empack-3.3.2/LICENSE
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 empack-3.3.2/README.md
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 empack-3.3.2/pyproject.toml
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 empack-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 empack-3.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 empack-3.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 empack-3.3.3/ci_env.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 empack-3.3.3/setup.py
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 empack-3.3.3/config/empack_config.yaml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 empack-3.3.3/empack/__init__.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 empack-3.3.3/empack/file_patterns.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 empack-3.3.3/empack/filter_env.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 empack-3.3.3/empack/micromamba_wrapper.py
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 empack-3.3.3/empack/pack.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 empack-3.3.3/empack/repodata.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 empack-3.3.3/empack/tar_utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 empack-3.3.3/empack/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/app.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/err.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/main.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/pack.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/repodata.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.3.3/tests/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 empack-3.3.3/tests/conftest.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 empack-3.3.3/tests/empack_test_config.yaml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 empack-3.3.3/tests/empack_test_extra_config.yaml
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 empack-3.3.3/tests/test_cli.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 empack-3.3.3/tests/test_filter.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 empack-3.3.3/tests/test_integration.py
+-rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 empack-3.3.3/tests/test_pack.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 empack-3.3.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 empack-3.3.3/LICENSE
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 empack-3.3.3/README.md
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 empack-3.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 empack-3.3.3/PKG-INFO
```

### Comparing `empack-3.3.2/.pre-commit-config.yaml` & `empack-3.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/CHANGELOG.md` & `empack-3.3.3/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 3.3.3
+
+([Full Changelog](https://github.com/emscripten-forge/empack/compare/v3.3.2...d6ae4fc42fe79aa7a60f4b70fa72245e1e7566a3))
+
+### Enhancements made
+
+- use abspath when comparing dirs [#95](https://github.com/emscripten-forge/empack/pull/95) ([@DerThorsten](https://github.com/DerThorsten))
+
+### Bugs fixed
+
+- Fix rules for pyvis [#96](https://github.com/emscripten-forge/empack/pull/96) ([@martinRenou](https://github.com/martinRenou))
+- use abspath when comparing dirs [#95](https://github.com/emscripten-forge/empack/pull/95) ([@DerThorsten](https://github.com/DerThorsten))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/emscripten-forge/empack/graphs/contributors?from=2024-02-05&to=2024-04-26&type=c))
+
+[@DerThorsten](https://github.com/search?q=repo%3Aemscripten-forge%2Fempack+involves%3ADerThorsten+updated%3A2024-02-05..2024-04-26&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Aemscripten-forge%2Fempack+involves%3AmartinRenou+updated%3A2024-02-05..2024-04-26&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 3.3.2
 
 ([Full Changelog](https://github.com/emscripten-forge/empack/compare/v3.3.1...d742539ef5f7fdf4afb94561d4026a7976ebc629))
 
 ### Enhancements made
 
 - Update config for urllib and certifi [#94](https://github.com/emscripten-forge/empack/pull/94) ([@martinRenou](https://github.com/martinRenou))
@@ -16,16 +37,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/emscripten-forge/empack/graphs/contributors?from=2024-01-29&to=2024-02-05&type=c))
 
 [@martinRenou](https://github.com/search?q=repo%3Aemscripten-forge%2Fempack+involves%3AmartinRenou+updated%3A2024-01-29..2024-02-05&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Aemscripten-forge%2Fempack+involves%3Atrungleduc+updated%3A2024-01-29..2024-02-05&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 3.3.1
 
 ([Full Changelog](https://github.com/emscripten-forge/empack/compare/v3.3.0...d8d48c6779696aac0a695fe162fd7c38f698073e))
 
 ### Enhancements made
 
 - fixes for voici windows build [#90](https://github.com/emscripten-forge/empack/pull/90) ([@pjaggi1](https://github.com/pjaggi1))
```

### Comparing `empack-3.3.2/config/empack_config.yaml` & `empack-3.3.3/config/empack_config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,18 @@
     include_patterns:
       - pattern: '*.py'
       - pattern: '**/contrib/emscripten/emscripten_fetch_worker.js'
   certifi:
     include_patterns:
       - pattern: '*.py'
       - pattern: '*.pem'
+  pyvis:
+    include_patterns:
+      - pattern: '*.py'
+      - pattern: '*.html'
 default:
   include_patterns:
     - pattern: '*.so'
     - pattern: '*.py'
     - pattern: '*.json'
     - pattern: 'share/zoneinfo/**'
     - pattern: '**/*.dist-info/METADATA'
```

### Comparing `empack-3.3.2/empack/file_patterns.py` & `empack-3.3.3/empack/file_patterns.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/empack/filter_env.py` & `empack-3.3.3/empack/filter_env.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/empack/micromamba_wrapper.py` & `empack-3.3.3/empack/micromamba_wrapper.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/empack/pack.py` & `empack-3.3.3/empack/pack.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     env_meta["packages"].append(package_item)
     with open(env_meta_filename, "w") as f:
         json.dump(env_meta, f, indent=4)
 
     # dir of env_meta_filename
     env_meta_dir = Path(env_meta_filename).parent
     # copy tarfile to env_meta_dir if not already there
-    if Path(tarfile).parent != env_meta_dir:
+    if Path(tarfile).parent.resolve() != env_meta_dir.resolve():
         shutil.copy(tarfile, env_meta_dir)
 
 
 def pack_env(
     env_prefix,
     relocate_prefix,
     file_filters,
```

### Comparing `empack-3.3.2/empack/repodata.py` & `empack-3.3.3/empack/repodata.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/empack/tar_utils.py` & `empack-3.3.3/empack/tar_utils.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/empack/cli/pack.py` & `empack-3.3.3/empack/cli/pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/empack/cli/repodata.py` & `empack-3.3.3/empack/cli/repodata.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/tests/conftest.py` & `empack-3.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/tests/empack_test_config.yaml` & `empack-3.3.3/tests/empack_test_config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/tests/test_cli.py` & `empack-3.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/tests/test_filter.py` & `empack-3.3.3/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/tests/test_integration.py` & `empack-3.3.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/tests/test_pack.py` & `empack-3.3.3/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/.gitignore` & `empack-3.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/LICENSE` & `empack-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/README.md` & `empack-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/pyproject.toml` & `empack-3.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `empack-3.3.2/PKG-INFO` & `empack-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: empack
-Version: 3.3.2
+Version: 3.3.3
 Summary: empack emscripten+boa
 Project-URL: Homepage, https://github.com/emscripten-forge/empack
 Author-email: Thorsten Beier <derthorstenbeier@gmail.com>
 License: 
         MIT License
         
         Copyright (c) 2022, Thorsten Beier
```

