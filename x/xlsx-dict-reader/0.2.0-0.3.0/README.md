# Comparing `tmp/xlsx_dict_reader-0.2.0.tar.gz` & `tmp/xlsx_dict_reader-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlsx_dict_reader-0.2.0.tar", max compression
+gzip compressed data, was "xlsx_dict_reader-0.3.0.tar", max compression
```

## Comparing `xlsx_dict_reader-0.2.0.tar` & `xlsx_dict_reader-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1130 2024-03-24 12:10:30.531644 xlsx_dict_reader-0.2.0/LICENSE
--rw-r--r--   0        0        0      673 2024-03-24 12:14:44.066841 xlsx_dict_reader-0.2.0/README.md
--rw-r--r--   0        0        0      695 2024-03-25 02:13:52.418986 xlsx_dict_reader-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       36 2024-03-24 10:18:00.358925 xlsx_dict_reader-0.2.0/xlsx_dict_reader/__init__.py
--rw-r--r--   0        0        0     2463 2024-03-24 11:39:58.591255 xlsx_dict_reader-0.2.0/xlsx_dict_reader/dict_reader.py
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 xlsx_dict_reader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1130 2024-03-24 12:10:30.531644 xlsx_dict_reader-0.3.0/LICENSE
+-rw-r--r--   0        0        0      673 2024-03-24 12:14:44.066841 xlsx_dict_reader-0.3.0/README.md
+-rw-r--r--   0        0        0      695 2024-04-26 14:21:48.052929 xlsx_dict_reader-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-03-24 10:18:00.358925 xlsx_dict_reader-0.3.0/xlsx_dict_reader/__init__.py
+-rw-r--r--   0        0        0     2657 2024-04-26 14:20:28.321492 xlsx_dict_reader-0.3.0/xlsx_dict_reader/dict_reader.py
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 xlsx_dict_reader-0.3.0/PKG-INFO
```

### Comparing `xlsx_dict_reader-0.2.0/LICENSE` & `xlsx_dict_reader-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xlsx_dict_reader-0.2.0/README.md` & `xlsx_dict_reader-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xlsx_dict_reader-0.2.0/pyproject.toml` & `xlsx_dict_reader-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xlsx-dict-reader"
-version = "0.2.0"
+version = "0.3.0"
 description = "An interface similar to csv.DictReader for openpyxl WorkSheet objects"
 authors = ["Geoff Beier <geoff@tuxpup.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://git.sr.ht/~tuxpup/xlsx-dict-reader"
 
 [tool.poetry.dependencies]
```

### Comparing `xlsx_dict_reader-0.2.0/xlsx_dict_reader/dict_reader.py` & `xlsx_dict_reader-0.3.0/xlsx_dict_reader/dict_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,24 @@
         min_row: int = None,
         max_row: int = None,
         min_col: int = None,
         max_col: int = None,
         headers: List[str] = None,
         values_only=True,
         skip_blank_rows=False,
+        strip_whitespace_in_headers=True,
     ):
         self.worksheet = worksheet
         self.min_row = min_row
         self.max_row = max_row
         self.min_col = min_col
         self.max_col = max_col
         self.values_only = values_only
         self.skip_blank_rows = skip_blank_rows
+        self.strip_whitespace_in_headers = strip_whitespace_in_headers
         self.curr_row = 1
 
         if headers:
             self.headers = headers
             self.min_col = self.min_col or 1
             self.max_col = self.min_col + len(headers) - 1
         else:
@@ -39,14 +41,16 @@
         max_col = self.max_col or self.worksheet.max_column
         for col in self.worksheet.iter_cols(
             min_row=row, max_row=row, min_col=min_col, max_col=max_col
         ):
             hv = col[0].value
             if not hv:
                 break
+            if self.strip_whitespace_in_headers:
+                hv = hv.strip()
             if hv in headers:
                 raise ValueError(f"Duplicate header found: {hv}: {headers}")
             headers.append(hv)
         if self.max_col is not None:
             if len(headers) != max_col + 1 - min_col:
                 raise ValueError(
                     f"Number of headers ({len(headers)}) does not match "
```

### Comparing `xlsx_dict_reader-0.2.0/PKG-INFO` & `xlsx_dict_reader-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlsx-dict-reader
-Version: 0.2.0
+Version: 0.3.0
 Summary: An interface similar to csv.DictReader for openpyxl WorkSheet objects
 Home-page: https://git.sr.ht/~tuxpup/xlsx-dict-reader
 License: MIT
 Author: Geoff Beier
 Author-email: geoff@tuxpup.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

