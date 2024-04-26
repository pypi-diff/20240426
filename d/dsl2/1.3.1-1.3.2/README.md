# Comparing `tmp/dsl2-1.3.1.tar.gz` & `tmp/dsl2-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsl2-1.3.1.tar", max compression
+gzip compressed data, was "dsl2-1.3.2.tar", max compression
```

## Comparing `dsl2-1.3.1.tar` & `dsl2-1.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-12-31 06:15:27.466138 dsl2-1.3.1/LICENSE
--rw-r--r--   0        0        0       77 2023-12-31 06:15:27.466138 dsl2-1.3.1/README.md
--rw-r--r--   0        0        0        0 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/__init__.py
--rw-r--r--   0        0        0       28 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/config.default.yml
--rw-r--r--   0        0        0      725 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/config.py
--rw-r--r--   0        0        0     9152 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/dsl.py
--rw-r--r--   0        0        0       96 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/feature_extraction/__init__.py
--rw-r--r--   0        0        0       96 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/feature_extraction/column_base/__init__.py
--rw-r--r--   0        0        0      874 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/feature_extraction/column_base/column_name.py
--rw-r--r--   0        0        0     1882 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/feature_extraction/column_base/numeric.py
--rw-r--r--   0        0        0     1521 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/feature_extraction/column_base/textual.py
--rw-r--r--   0        0        0     3770 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/generate_train_data.py
--rw-r--r--   0        0        0     7099 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/input.py
--rw-r--r--   0        0        0     9240 2023-12-31 06:15:27.634138 dsl2-1.3.1/dsl/sm_type_db.py
--rw-r--r--   0        0        0      662 2023-12-31 06:15:27.634138 dsl2-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 dsl2-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-26 18:49:41.215866 dsl2-1.3.2/LICENSE
+-rw-r--r--   0        0        0       77 2024-04-26 18:49:41.215866 dsl2-1.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/config.default.yml
+-rw-r--r--   0        0        0      725 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/config.py
+-rw-r--r--   0        0        0     9152 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/dsl.py
+-rw-r--r--   0        0        0       96 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/feature_extraction/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/feature_extraction/column_base/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/feature_extraction/column_base/column_name.py
+-rw-r--r--   0        0        0     1882 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/feature_extraction/column_base/numeric.py
+-rw-r--r--   0        0        0     1521 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/feature_extraction/column_base/textual.py
+-rw-r--r--   0        0        0     3770 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/generate_train_data.py
+-rw-r--r--   0        0        0     7099 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/input.py
+-rw-r--r--   0        0        0     9240 2024-04-26 18:49:41.379867 dsl2-1.3.2/dsl/sm_type_db.py
+-rw-r--r--   0        0        0      662 2024-04-26 18:49:41.379867 dsl2-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 dsl2-1.3.2/PKG-INFO
```

### Comparing `dsl2-1.3.1/LICENSE` & `dsl2-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsl2-1.3.1/dsl/config.py` & `dsl2-1.3.2/dsl/config.py`

 * *Files identical despite different names*

### Comparing `dsl2-1.3.1/dsl/dsl.py` & `dsl2-1.3.2/dsl/dsl.py`

 * *Files identical despite different names*

### Comparing `dsl2-1.3.1/dsl/feature_extraction/column_base/column_name.py` & `dsl2-1.3.2/dsl/feature_extraction/column_base/column_name.py`

 * *Files identical despite different names*

### Comparing `dsl2-1.3.1/dsl/feature_extraction/column_base/numeric.py` & `dsl2-1.3.2/dsl/feature_extraction/column_base/numeric.py`

 * *Files identical despite different names*

### Comparing `dsl2-1.3.1/dsl/feature_extraction/column_base/textual.py` & `dsl2-1.3.2/dsl/feature_extraction/column_base/textual.py`

 * *Files identical despite different names*

### Comparing `dsl2-1.3.1/dsl/generate_train_data.py` & `dsl2-1.3.2/dsl/generate_train_data.py`

 * *Files identical despite different names*

### Comparing `dsl2-1.3.1/dsl/input.py` & `dsl2-1.3.2/dsl/input.py`

 * *Files identical despite different names*

### Comparing `dsl2-1.3.1/dsl/sm_type_db.py` & `dsl2-1.3.2/dsl/sm_type_db.py`

 * *Files identical despite different names*

### Comparing `dsl2-1.3.1/pyproject.toml` & `dsl2-1.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "dsl2"
-version = "1.3.1"
+version = "1.3.2"
 description = "An implementation of Semantic labeling: A domain-independent approach"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/binh-vu/dsl"
 packages = [{ include = "dsl" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-sem-desc = "^6.0.0"
+sem-desc = "^6.7.2"
 fastnumbers = "^5.0.1"
 ftfy = "^6.1.3"
 spacy = "^3.7.2"
 tqdm = "^4.66.1"
 serde2 = "^1.6.0"
 scipy = "^1.11.4"
 numpy = "^1.26.2"
-kgdata = "^6.0.0"
+kgdata = "^7.0.0"
 scikit-learn = "^1.3.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `dsl2-1.3.1/PKG-INFO` & `dsl2-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: dsl2
-Version: 1.3.1
+Version: 1.3.2
 Summary: An implementation of Semantic labeling: A domain-independent approach
 Home-page: https://github.com/binh-vu/dsl
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastnumbers (>=5.0.1,<6.0.0)
 Requires-Dist: ftfy (>=6.1.3,<7.0.0)
-Requires-Dist: kgdata (>=6.0.0,<7.0.0)
+Requires-Dist: kgdata (>=7.0.0,<8.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
-Requires-Dist: sem-desc (>=6.0.0,<7.0.0)
+Requires-Dist: sem-desc (>=6.7.2,<7.0.0)
 Requires-Dist: serde2 (>=1.6.0,<2.0.0)
 Requires-Dist: spacy (>=3.7.2,<4.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/binh-vu/dsl
 Description-Content-Type: text/markdown
 
 # dsl
```

