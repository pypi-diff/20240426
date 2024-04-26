# Comparing `tmp/rich_split-0.1.0.tar.gz` & `tmp/rich_split-0.1.1.tar.gz`

## Comparing `rich_split-0.1.0.tar` & `rich_split-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/__init__.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/exceptions.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/cutters/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/cutters/base_cutter.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/cutters/markdown_cutter.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/cutters/text_cutter.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/joiners/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/joiners/base_joiner.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/joiners/markdown_joiner.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/joiners/text_joiner.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/splitters/__init__.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/splitters/base_splitter.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/splitters/markdown_splitter.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/splitters/text_splitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/utils/__init__.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 rich_split-0.1.0/rich_split/utils/markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rich_split-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 rich_split-0.1.0/tests/test_cutters.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 rich_split-0.1.0/tests/test_joiners.py
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 rich_split-0.1.0/tests/test_splitters.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 rich_split-0.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rich_split-0.1.0/LICENSE
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 rich_split-0.1.0/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 rich_split-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 rich_split-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/__init__.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/exceptions.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/cutters/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/cutters/base_cutter.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/cutters/markdown_cutter.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/cutters/text_cutter.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/joiners/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/joiners/base_joiner.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/joiners/markdown_joiner.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/joiners/text_joiner.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/splitters/__init__.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/splitters/base_splitter.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/splitters/markdown_splitter.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/splitters/text_splitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/utils/__init__.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 rich_split-0.1.1/rich_split/utils/markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rich_split-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 rich_split-0.1.1/tests/test_cutters.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 rich_split-0.1.1/tests/test_joiners.py
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 rich_split-0.1.1/tests/test_splitters.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 rich_split-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rich_split-0.1.1/LICENSE
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 rich_split-0.1.1/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 rich_split-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 rich_split-0.1.1/PKG-INFO
```

### Comparing `rich_split-0.1.0/rich_split/cutters/markdown_cutter.py` & `rich_split-0.1.1/rich_split/cutters/markdown_cutter.py`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/rich_split/cutters/text_cutter.py` & `rich_split-0.1.1/rich_split/cutters/text_cutter.py`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/rich_split/joiners/markdown_joiner.py` & `rich_split-0.1.1/rich_split/joiners/markdown_joiner.py`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/rich_split/joiners/text_joiner.py` & `rich_split-0.1.1/rich_split/joiners/text_joiner.py`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/rich_split/splitters/base_splitter.py` & `rich_split-0.1.1/rich_split/splitters/base_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
         max_part_length,
         cutter_config=None,
         joiner_config=None,
         part_header_config=None,
         not_process_if_only_one_part=True,
     ):
         self.max_part_length = max_part_length
-        self.cutter_config = (self.cutter_config or {}) | (cutter_config or {})
+        self.cutter_config = (cutter_config or {}) | (self.cutter_config or {})
         self.cutter_config = copy.deepcopy(self.cutter_config)
-        self.joiner_config = (self.joiner_config or {}) | (joiner_config or {})
+        self.joiner_config = (joiner_config or {}) | (self.joiner_config or {})
         self.joiner_config = copy.deepcopy(self.joiner_config)
-        self.part_header_config = (self.part_header_config or {}) | (
-            part_header_config or {}
+        self.part_header_config = (part_header_config or {}) | (
+            self.part_header_config or {}
         )
         self.part_header_config = copy.deepcopy(self.part_header_config)
         self.not_process_if_only_one_part = not_process_if_only_one_part
         cutter_config = dict(self.cutter_config)
         cls = cutter_config.pop("class")
         self.cutter = cls(**cutter_config)
         joiner_config = dict(self.joiner_config)
```

### Comparing `rich_split-0.1.0/rich_split/splitters/markdown_splitter.py` & `rich_split-0.1.1/rich_split/splitters/markdown_splitter.py`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/rich_split/splitters/text_splitter.py` & `rich_split-0.1.1/rich_split/splitters/text_splitter.py`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/rich_split/utils/markdown.py` & `rich_split-0.1.1/rich_split/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/tests/test_cutters.py` & `rich_split-0.1.1/tests/test_cutters.py`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/tests/test_joiners.py` & `rich_split-0.1.1/tests/test_joiners.py`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/tests/test_splitters.py` & `rich_split-0.1.1/tests/test_splitters.py`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/.gitignore` & `rich_split-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/LICENSE` & `rich_split-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_split-0.1.0/pyproject.toml` & `rich_split-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   "rich_split",
   "tests",
   "LICENSE",
 ]
 
 [project]
 name = "rich_split"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Danstiv", email="danstiv@yandex.ru" },
 ]
 description = "Library for splitting simple strings and markdown"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `rich_split-0.1.0/PKG-INFO` & `rich_split-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rich_split
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for splitting simple strings and markdown
 Project-URL: Homepage, https://github.com/Danstiv/rich_split
 Project-URL: Bug Tracker, https://github.com/Danstiv/rich_split/issues
 Author-email: Danstiv <danstiv@yandex.ru>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

