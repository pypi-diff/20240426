# Comparing `tmp/gbnf-0.0.4.tar.gz` & `tmp/gbnf-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbnf-0.0.4.tar", last modified: Sun Apr 14 19:32:21 2024, max compression
+gzip compressed data, was "gbnf-0.0.5.tar", last modified: Fri Apr 26 12:32:17 2024, max compression
```

## Comparing `gbnf-0.0.4.tar` & `gbnf-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 thekevinscott   (501) staff       (20)        0 2024-04-14 19:32:21.794930 gbnf-0.0.4/
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1068 2024-04-14 19:32:19.000000 gbnf-0.0.4/LICENSE
--rw-r--r--   0 thekevinscott   (501) staff       (20)       55 2024-04-14 19:08:10.000000 gbnf-0.0.4/MANIFEST.in
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1593 2024-04-14 19:32:21.794659 gbnf-0.0.4/PKG-INFO
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1092 2024-04-14 19:08:10.000000 gbnf-0.0.4/README.md
-drwxr-xr-x   0 thekevinscott   (501) staff       (20)        0 2024-04-14 19:32:21.790818 gbnf-0.0.4/gbnf/
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1648 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/GBNF.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)       31 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/__init__.py
-drwxr-xr-x   0 thekevinscott   (501) staff       (20)        0 2024-04-14 19:32:21.794100 gbnf-0.0.4/gbnf/rules_builder/
--rw-r--r--   0 thekevinscott   (501) staff       (20)       68 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/__init__.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1891 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/errors.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1901 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/errors_test.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)       95 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/is_word_char.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)      599 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/is_word_char_test.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)      841 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/parse_char.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1489 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/parse_char_test.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)      498 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/parse_name.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)      691 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/parse_name_test.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)      416 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/parse_space.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)     2020 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/parse_space_test.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)     8577 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/rules_builder.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)    62881 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/rules_builder_test.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)     2089 2024-04-14 19:08:10.000000 gbnf-0.0.4/gbnf/rules_builder/types.py
-drwxr-xr-x   0 thekevinscott   (501) staff       (20)        0 2024-04-14 19:32:21.794369 gbnf-0.0.4/gbnf.egg-info/
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1593 2024-04-14 19:32:21.000000 gbnf-0.0.4/gbnf.egg-info/PKG-INFO
--rw-r--r--   0 thekevinscott   (501) staff       (20)      675 2024-04-14 19:32:21.000000 gbnf-0.0.4/gbnf.egg-info/SOURCES.txt
--rw-r--r--   0 thekevinscott   (501) staff       (20)        1 2024-04-14 19:32:21.000000 gbnf-0.0.4/gbnf.egg-info/dependency_links.txt
--rw-r--r--   0 thekevinscott   (501) staff       (20)        5 2024-04-14 19:32:21.000000 gbnf-0.0.4/gbnf.egg-info/top_level.txt
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1733 2024-04-14 19:08:10.000000 gbnf-0.0.4/pyproject.toml
--rw-r--r--   0 thekevinscott   (501) staff       (20)       38 2024-04-14 19:32:21.794979 gbnf-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:17.827558 gbnf-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 12:32:16.000000 gbnf-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-26 12:32:11.000000 gbnf-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-26 12:32:17.827558 gbnf-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-26 12:32:11.000000 gbnf-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:17.823558 gbnf-0.0.5/gbnf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/GBNF.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:17.827558 gbnf-0.0.5/gbnf/rules_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/is_word_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/is_word_char_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/parse_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/parse_char_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/parse_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/parse_name_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/parse_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/parse_space_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/rules_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62881 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/rules_builder_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-26 12:32:11.000000 gbnf-0.0.5/gbnf/rules_builder/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:17.827558 gbnf-0.0.5/gbnf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-26 12:32:17.000000 gbnf-0.0.5/gbnf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-26 12:32:17.000000 gbnf-0.0.5/gbnf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:32:17.000000 gbnf-0.0.5/gbnf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 12:32:17.000000 gbnf-0.0.5/gbnf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-26 12:32:11.000000 gbnf-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 12:32:17.827558 gbnf-0.0.5/setup.cfg
```

### Comparing `gbnf-0.0.4/LICENSE` & `gbnf-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/PKG-INFO` & `gbnf-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbnf
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for parsing GBNF grammars
 Author-email: Kevin Scott <kevin@gbnf.dev>
 Project-URL: Homepage, https://github.com/thekevinscott/gbnf
 Project-URL: Bug Tracker, https://github.com/thekevinscott/gbnf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gbnf Version: 0.0.4 Summary: A library for parsing
+Metadata-Version: 2.1 Name: gbnf Version: 0.0.5 Summary: A library for parsing
 GBNF grammars Author-email: Kevin Scott
 gbnf.dev> Project-URL: Homepage, https://github.com/thekevinscott/gbnf Project-
 URL: Bug Tracker, https://github.com/thekevinscott/gbnf/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE # GBNF _[_L_a_t_e_s_t
 _G_B_N_F_ _P_y_P_I_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_ _f_o_r_ _g_b_n_f_]_[_D_o_w_n_l_o_a_d_s_ _p_e_r_ _w_e_e_k_ _o_n_ _P_y_P_I_ _f_o_r_ _g_b_n_f_]
```

### Comparing `gbnf-0.0.4/README.md` & `gbnf-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/GBNF.py` & `gbnf-0.0.5/gbnf/GBNF.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/rules_builder/errors.py` & `gbnf-0.0.5/gbnf/rules_builder/errors.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/rules_builder/errors_test.py` & `gbnf-0.0.5/gbnf/rules_builder/errors_test.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/rules_builder/is_word_char_test.py` & `gbnf-0.0.5/gbnf/rules_builder/is_word_char_test.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/rules_builder/parse_char.py` & `gbnf-0.0.5/gbnf/rules_builder/parse_char.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/rules_builder/parse_char_test.py` & `gbnf-0.0.5/gbnf/rules_builder/parse_char_test.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/rules_builder/parse_name_test.py` & `gbnf-0.0.5/gbnf/rules_builder/parse_name_test.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/rules_builder/parse_space_test.py` & `gbnf-0.0.5/gbnf/rules_builder/parse_space_test.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/rules_builder/rules_builder.py` & `gbnf-0.0.5/gbnf/rules_builder/rules_builder.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/rules_builder/rules_builder_test.py` & `gbnf-0.0.5/gbnf/rules_builder/rules_builder_test.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf/rules_builder/types.py` & `gbnf-0.0.5/gbnf/rules_builder/types.py`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/gbnf.egg-info/PKG-INFO` & `gbnf-0.0.5/gbnf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbnf
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for parsing GBNF grammars
 Author-email: Kevin Scott <kevin@gbnf.dev>
 Project-URL: Homepage, https://github.com/thekevinscott/gbnf
 Project-URL: Bug Tracker, https://github.com/thekevinscott/gbnf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gbnf Version: 0.0.4 Summary: A library for parsing
+Metadata-Version: 2.1 Name: gbnf Version: 0.0.5 Summary: A library for parsing
 GBNF grammars Author-email: Kevin Scott
 gbnf.dev> Project-URL: Homepage, https://github.com/thekevinscott/gbnf Project-
 URL: Bug Tracker, https://github.com/thekevinscott/gbnf/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE # GBNF _[_L_a_t_e_s_t
 _G_B_N_F_ _P_y_P_I_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_ _f_o_r_ _g_b_n_f_]_[_D_o_w_n_l_o_a_d_s_ _p_e_r_ _w_e_e_k_ _o_n_ _P_y_P_I_ _f_o_r_ _g_b_n_f_]
```

### Comparing `gbnf-0.0.4/gbnf.egg-info/SOURCES.txt` & `gbnf-0.0.5/gbnf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.4/pyproject.toml` & `gbnf-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gbnf"
-version = "0.0.4"
+version = "0.0.5"
 # Notes
 authors = [{ name = "Kevin Scott", email = "kevin@gbnf.dev" }]
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
 ]
 description = "A library for parsing GBNF grammars"
```

