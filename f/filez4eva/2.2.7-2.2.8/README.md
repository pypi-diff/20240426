# Comparing `tmp/filez4eva-2.2.7.tar.gz` & `tmp/filez4eva-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filez4eva-2.2.7.tar", max compression
+gzip compressed data, was "filez4eva-2.2.8.tar", max compression
```

## Comparing `filez4eva-2.2.7.tar` & `filez4eva-2.2.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1616 2024-03-18 00:40:04.806631 filez4eva-2.2.7/README.md
--rw-r--r--   0        0        0      168 2024-03-18 00:40:04.806631 filez4eva-2.2.7/filez4eva/__init__.py
--rw-r--r--   0        0        0       48 2024-03-18 00:40:04.806631 filez4eva-2.2.7/filez4eva/__main__.py
--rw-r--r--   0        0        0      288 2024-03-18 00:40:04.806631 filez4eva-2.2.7/filez4eva/command/__init__.py
--rw-r--r--   0        0        0      654 2024-03-18 00:40:04.806631 filez4eva-2.2.7/filez4eva/command/scan_command.py
--rw-r--r--   0        0        0     2067 2024-03-18 00:40:04.806631 filez4eva-2.2.7/filez4eva/command/stow_command.py
--rw-r--r--   0        0        0      730 2024-03-18 00:40:04.806631 filez4eva-2.2.7/filez4eva/directory_scanner.py
--rw-r--r--   0        0        0       42 2024-03-18 00:40:04.806631 filez4eva-2.2.7/filez4eva/error.py
--rw-r--r--   0        0        0     2487 2024-03-18 00:40:04.806631 filez4eva-2.2.7/filez4eva/file_mover.py
--rw-r--r--   0        0        0      586 2024-03-18 00:40:14.883530 filez4eva-2.2.7/pyproject.toml
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 filez4eva-2.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1616 2024-04-26 04:48:22.060644 filez4eva-2.2.8/README.md
+-rw-r--r--   0        0        0      168 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/__main__.py
+-rw-r--r--   0        0        0      288 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/command/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/command/scan_command.py
+-rw-r--r--   0        0        0     3261 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/command/stow_command.py
+-rw-r--r--   0        0        0      730 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/directory_scanner.py
+-rw-r--r--   0        0        0       42 2024-04-26 04:48:22.061644 filez4eva-2.2.8/filez4eva/error.py
+-rw-r--r--   0        0        0     2487 2024-04-26 04:48:22.061644 filez4eva-2.2.8/filez4eva/file_mover.py
+-rw-r--r--   0        0        0      585 2024-04-26 04:48:32.205571 filez4eva-2.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 filez4eva-2.2.8/PKG-INFO
```

### Comparing `filez4eva-2.2.7/README.md` & `filez4eva-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `filez4eva-2.2.7/filez4eva/command/scan_command.py` & `filez4eva-2.2.8/filez4eva/command/scan_command.py`

 * *Files identical despite different names*

### Comparing `filez4eva-2.2.7/filez4eva/directory_scanner.py` & `filez4eva-2.2.8/filez4eva/directory_scanner.py`

 * *Files identical despite different names*

### Comparing `filez4eva-2.2.7/filez4eva/file_mover.py` & `filez4eva-2.2.8/filez4eva/file_mover.py`

 * *Files identical despite different names*

### Comparing `filez4eva-2.2.7/pyproject.toml` & `filez4eva-2.2.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "filez4eva"
 description = "Shift scans, photos, and other files into structured folders for permanent safekeeping"
 authors = ["Francis Potter <francis@steampunkwizard.ca>"]
 license = "MIT"
 readme = "README.md"
-version = "2.2.7"
+version = "2.2.8"
 
 [tool.poetry.dependencies]
 python = "~3.11"
-wizlib = "^2.0.12"
 watchdog = "^3.0.0"
+wizlib = "2.0.18"
 
 [tool.poetry.group.dev.dependencies]
 pycodestyle = "^2.11.0"
 coverage = "^7.3.0"
 autopep8 = "^2.0.4"
 
 [build-system]
```

### Comparing `filez4eva-2.2.7/PKG-INFO` & `filez4eva-2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: filez4eva
-Version: 2.2.7
+Version: 2.2.8
 Summary: Shift scans, photos, and other files into structured folders for permanent safekeeping
 License: MIT
 Author: Francis Potter
 Author-email: francis@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
-Requires-Dist: wizlib (>=2.0.12,<3.0.0)
+Requires-Dist: wizlib (==2.0.18)
 Description-Content-Type: text/markdown
 
 # Filez4Eva
 
 Shift scans, photos, and other files into structured folders for permanent safekeeping
 ---
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: filez4eva Version: 2.2.7 Summary: Shift scans,
+Metadata-Version: 2.1 Name: filez4eva Version: 2.2.8 Summary: Shift scans,
 photos, and other files into structured folders for permanent safekeeping
 License: MIT Author: Francis Potter Author-email: francis@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: watchdog (>=3.0.0,<4.0.0) Requires-
-Dist: wizlib (>=2.0.12,<3.0.0) Description-Content-Type: text/markdown #
-Filez4Eva Shift scans, photos, and other files into structured folders for
-permanent safekeeping --- _E_l_e_p_h_a_n_t_ _i_c_o_n_ _c_r_e_a_t_e_d_ _b_y_ _F_l_a_t_ _I_c_o_n_s_ _-_ _F_l_a_t_i_c_o_n I keep
-files named and organized in a certain way in DropBox. This tool names new
-files correctly and puts them in the right directory. ## Installation It's best
-to install using `pipx`. See [the pipx site](https://pypa.github.io/pipx/) if
-you need it. Then: ```bash pipx install filez4eva ``` ## Usage The directory
+Dist: wizlib (==2.0.18) Description-Content-Type: text/markdown # Filez4Eva
+Shift scans, photos, and other files into structured folders for permanent
+safekeeping --- _E_l_e_p_h_a_n_t_ _i_c_o_n_ _c_r_e_a_t_e_d_ _b_y_ _F_l_a_t_ _I_c_o_n_s_ _-_ _F_l_a_t_i_c_o_n I keep files
+named and organized in a certain way in DropBox. This tool names new files
+correctly and puts them in the right directory. ## Installation It's best to
+install using `pipx`. See [the pipx site](https://pypa.github.io/pipx/) if you
+need it. Then: ```bash pipx install filez4eva ``` ## Usage The directory
 pattern for account documents is: ``` ~/Dropbox/accounts///-. ``` Where: -
 `year` is the year of the document, typically from the date - `account` is the
 name of the account, all lower case, hyphen separated - `date` is the date on
 the document in `YYYYMMDD` format - `part` is the textual part of the name of
 the document, often starting with the account name, all lower case, hyphen
 separated - `extension` is the original filename extension, often `pdf` I have
 my browsers etc. set to download new files to Desktop, then it's easy to run
```

