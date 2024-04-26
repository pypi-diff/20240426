# Comparing `tmp/fosslight_source-1.7.6.tar.gz` & `tmp/fosslight_source-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fosslight_source-1.7.6.tar", last modified: Thu Feb 29 08:04:13 2024, max compression
+gzip compressed data, was "fosslight_source-1.7.7.tar", last modified: Fri Apr 26 06:38:26 2024, max compression
```

## Comparing `fosslight_source-1.7.6.tar` & `fosslight_source-1.7.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:04:13.190995 fosslight_source-1.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-02-29 08:04:13.190995 fosslight_source-1.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 08:04:13.190995 fosslight_source-1.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:04:13.186995 fosslight_source-1.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:04:13.190995 fosslight_source-1.7.6/src/fosslight_source/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/src/fosslight_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/src/fosslight_source/_help.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2046 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/src/fosslight_source/_license_matched.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13177 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/src/fosslight_source/_parsing_scancode_file_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/src/fosslight_source/_parsing_scanoss_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/src/fosslight_source/_scan_item.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12235 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/src/fosslight_source/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5610 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/src/fosslight_source/run_scancode.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3630 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/src/fosslight_source/run_scanoss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-02-29 08:04:04.000000 fosslight_source-1.7.6/src/fosslight_source/run_spdx_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:04:13.190995 fosslight_source-1.7.6/src/fosslight_source.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-02-29 08:04:12.000000 fosslight_source-1.7.6/src/fosslight_source.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-29 08:04:13.000000 fosslight_source-1.7.6/src/fosslight_source.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 08:04:12.000000 fosslight_source-1.7.6/src/fosslight_source.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-29 08:04:12.000000 fosslight_source-1.7.6/src/fosslight_source.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-29 08:04:12.000000 fosslight_source-1.7.6/src/fosslight_source.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 08:04:12.000000 fosslight_source-1.7.6/src/fosslight_source.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:26.094636 fosslight_source-1.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-26 06:38:26.094636 fosslight_source-1.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:38:26.094636 fosslight_source-1.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:26.090635 fosslight_source-1.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:26.090635 fosslight_source-1.7.7/src/fosslight_source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/src/fosslight_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/src/fosslight_source/_help.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2046 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/src/fosslight_source/_license_matched.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13245 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/src/fosslight_source/_parsing_scancode_file_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/src/fosslight_source/_parsing_scanoss_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/src/fosslight_source/_scan_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12275 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/src/fosslight_source/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5610 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/src/fosslight_source/run_scancode.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3630 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/src/fosslight_source/run_scanoss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-26 06:38:18.000000 fosslight_source-1.7.7/src/fosslight_source/run_spdx_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:26.094636 fosslight_source-1.7.7/src/fosslight_source.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-26 06:38:25.000000 fosslight_source-1.7.7/src/fosslight_source.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-26 06:38:26.000000 fosslight_source-1.7.7/src/fosslight_source.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:38:25.000000 fosslight_source-1.7.7/src/fosslight_source.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 06:38:25.000000 fosslight_source-1.7.7/src/fosslight_source.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-26 06:38:25.000000 fosslight_source-1.7.7/src/fosslight_source.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 06:38:25.000000 fosslight_source-1.7.7/src/fosslight_source.egg-info/top_level.txt
```

### Comparing `fosslight_source-1.7.6/LICENSE` & `fosslight_source-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.7.6/PKG-INFO` & `fosslight_source-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_source
-Version: 1.7.6
+Version: 1.7.7
 Summary: FOSSLight Source Scanner
 Home-page: https://github.com/fosslight/fosslight_source_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_source_scanner
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight_source Version: 1.7.6 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight_source Version: 1.7.7 Summary: FOSSLight
 Source Scanner Home-page: https://github.com/fosslight/fosslight_source_scanner
 Author: LG Electronics License: Apache-2.0 Download-URL: https://github.com/
 fosslight/fosslight_source_scanner Description:
                                                                        _[_K_o_r_e_a_n_]
 # FOSSLight Source Scanner [FOSSLight Source Scanner is released under the
 Apache-2.0 License.][Current python package version.][https://img.shields.io/
 pypi/pyversions/fosslight_source][![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_source-1.7.6/README.md` & `fosslight_source-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.7.6/setup.py` & `fosslight_source-1.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('requirements.txt', 'r', 'utf-8') as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_source',
-        version='1.7.6',
+        version='1.7.7',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Source Scanner',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_source-1.7.6/src/fosslight_source/_help.py` & `fosslight_source-1.7.7/src/fosslight_source/_help.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.7.6/src/fosslight_source/_license_matched.py` & `fosslight_source-1.7.7/src/fosslight_source/_license_matched.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.7.6/src/fosslight_source/_parsing_scancode_file_item.py` & `fosslight_source-1.7.7/src/fosslight_source/_parsing_scancode_file_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import re
 import fosslight_util.constant as constant
 from ._license_matched import MatchedLicense
 from ._scan_item import ScanItem
 from ._scan_item import is_exclude_dir
 from ._scan_item import is_exclude_file
 from ._scan_item import replace_word
+from ._scan_item import is_notice_file
 
 logger = logging.getLogger(constant.LOGGER_NAME)
 _exclude_directory = ["test", "tests", "doc", "docs"]
 _exclude_directory = [os.path.sep + dir_name +
                       os.path.sep for dir_name in _exclude_directory]
 _exclude_directory.append("/.")
 REMOVE_LICENSE = ["warranty-disclaimer"]
@@ -261,15 +262,15 @@
                     license_expression = file.get("detected_license_expression", "")
                     if license_expression_spdx:
                         license_expression = license_expression_spdx
                     if license_expression:
                         result_item.comment = license_expression
 
                 result_item.exclude = is_exclude_file(file_path)
-                result_item.is_license_text = file.get("percentage_of_license_text", 0) > 90
+                result_item.is_license_text = file.get("percentage_of_license_text", 0) > 90 or is_notice_file(file_path)
                 scancode_file_item.append(result_item)
             except Exception as ex:
                 msg.append(f"Error Parsing item: {ex}")
                 rc = False
 
     return rc, scancode_file_item, msg, license_list
```

### Comparing `fosslight_source-1.7.6/src/fosslight_source/_parsing_scanoss_file.py` & `fosslight_source-1.7.7/src/fosslight_source/_parsing_scanoss_file.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.7.6/src/fosslight_source/_scan_item.py` & `fosslight_source-1.7.7/src/fosslight_source/_scan_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020 LG Electronics Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 import logging
+import re
 import fosslight_util.constant as constant
 
 logger = logging.getLogger(constant.LOGGER_NAME)
 replace_word = ["-only", "-old-style", "-or-later", "licenseref-scancode-", "licenseref-"]
+_notice_filename = ['licen[cs]e[s]?', 'notice[s]?', 'legal', 'copyright[s]?', 'copying*', 'patent[s]?', 'unlicen[cs]e', 'eula',
+                    '[a,l]?gpl[-]?[1-3]?[.,-,_]?[0-1]?', 'mit', 'bsd[-]?[0-4]?', 'bsd[-]?[0-4][-]?clause[s]?',
+                    'apache[-,_]?[1-2]?[.,-,_]?[0-2]?']
 _exclude_filename = ["changelog", "config.guess", "config.sub", "changes", "ltmain.sh",
                      "configure", "configure.ac", "depcomp", "compile", "missing", "makefile"]
 _exclude_extension = [".m4", ".in", ".po"]
 _exclude_directory = ["test", "tests", "doc", "docs"]
 _exclude_directory = [os.path.sep + dir_name +
                       os.path.sep for dir_name in _exclude_directory]
 _exclude_directory.append("/.")
@@ -115,7 +119,14 @@
             # There will be no execution of this else statement.
             # Because scancode json output results are sorted by path,
             # most of them will match the previous if statement.
             return is_exclude_dir(dir_path)
     else:  # running SCANOSS
         return is_exclude_dir(dir_path)
     return False
+
+
+def is_notice_file(file_path):
+    pattern = r"({})(?<!w)".format("|".join(_notice_filename))
+    file_path = file_path.lower()
+    filename = os.path.basename(file_path)
+    return bool(re.match(pattern, filename))
```

### Comparing `fosslight_source-1.7.6/src/fosslight_source/cli.py` & `fosslight_source-1.7.7/src/fosslight_source/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .run_scancode import run_scan
 from .run_scanoss import run_scanoss_py
 from .run_scanoss import get_scanoss_extra_info
 import yaml
 import argparse
 from .run_spdx_extractor import get_spdx_downloads
 from ._scan_item import ScanItem
+from fosslight_util.cover import CoverItem
 
 SRC_SHEET_NAME = 'SRC_FL_Source'
 SCANOSS_HEADER = {SRC_SHEET_NAME: ['ID', 'Source Name or Path', 'OSS Name',
                                    'OSS Version', 'License', 'Download Location',
                                    'Homepage', 'Copyright Text', 'Exclude', 'Comment']}
 MERGED_HEADER = {SRC_SHEET_NAME: ['ID', 'Source Name or Path', 'OSS Name',
                                   'OSS Version', 'License', 'Download Location',
@@ -139,33 +140,34 @@
 
     if output_file == "":
         if output_extension == _json_ext:
             output_file = f"fosslight_opossum_src_{_start_time}"
         else:
             output_file = f"fosslight_report_src_{_start_time}"
 
+    cover = CoverItem(tool_name=_PKG_NAME,
+                      start_time=_start_time,
+                      input_path=path_to_scan)
+    files_count = sum([len(files) for r, d, files in os.walk(path_to_scan)])
+    cover.comment = f"Total number of files: {files_count} "
+    if len(merged_result) == 0:
+        if files_count < 1:
+            cover.comment += "(No file detected.)"
+        else:
+            cover.comment += "(No OSS detected.)"
+
+    sheet_list[SRC_SHEET_NAME] = []
     if merged_result:
-        if selected_scanner == 'scancode' or output_extension == _json_ext:
-            sheet_list[SRC_SHEET_NAME] = []
-            for scan_item in merged_result:
-                for row in scan_item.get_row_to_print():
-                    sheet_list[SRC_SHEET_NAME].append(row)
-
-        elif selected_scanner == 'scanoss':
-            sheet_list[SRC_SHEET_NAME] = []
-            for scan_item in merged_result:
-                for row in scan_item.get_row_to_print():
-                    sheet_list[SRC_SHEET_NAME].append(row)
-            extended_header = SCANOSS_HEADER
+        for scan_item in merged_result:
+            for row in scan_item.get_row_to_print():
+                sheet_list[SRC_SHEET_NAME].append(row)
 
+        if selected_scanner == 'scanoss':
+            extended_header = SCANOSS_HEADER
         else:
-            sheet_list[SRC_SHEET_NAME] = []
-            for scan_item in merged_result:
-                for row in scan_item.get_row_to_print():
-                    sheet_list[SRC_SHEET_NAME].append(row)
             extended_header = MERGED_HEADER
 
         if need_license:
             if selected_scanner == 'scancode' or output_extension == _json_ext:
                 sheet_list["scancode_reference"] = get_license_list_to_print(license_list)
             elif selected_scanner == 'scanoss':
                 sheet_list["scanoss_reference"] = get_scanoss_extra_info(scanoss_result)
@@ -179,18 +181,19 @@
             logger.info(f"No correction with yaml: {msg_correct}")
         else:
             sheet_list = correct_list
             logger.info("Success to correct with yaml.")
 
     output_file_without_ext = os.path.join(output_path, output_file)
     success_to_write, writing_msg, result_file = write_output_file(output_file_without_ext, output_extension,
-                                                                   sheet_list, extended_header)
+                                                                   sheet_list, extended_header, "", cover)
     if success_to_write:
         if result_file:
             logger.info(f"Output file:{result_file}")
+            logger.info(f'{cover.comment}')
         else:
             logger.warning(f"{writing_msg}")
     else:
         logger.error(f"Fail to generate result file. msg:({writing_msg})")
 
 
 def merge_results(scancode_result=[], scanoss_result=[], spdx_downloads={}):
@@ -260,15 +263,14 @@
                                                                                       print_matched_text, format, called_by_cli,
                                                                                       time_out, correct_mode, correct_filepath)
         if selected_scanner == 'scanoss' or selected_scanner == 'all' or selected_scanner == '':
             scanoss_result = run_scanoss_py(path_to_scan, output_file_name, format, True, write_json_file, num_cores)
         if selected_scanner in SCANNER_TYPE:
             spdx_downloads = get_spdx_downloads(path_to_scan)
             merged_result = merge_results(scancode_result, scanoss_result, spdx_downloads)
-
             create_report_file(start_time, merged_result, license_list, scanoss_result, selected_scanner, print_matched_text,
                                output_path, output_file, output_extension, correct_mode, correct_filepath, path_to_scan)
         else:
             print_help_msg_source_scanner()
             result_log[RESULT_KEY] = "Unsupported scanner"
             success = False
     else:
```

### Comparing `fosslight_source-1.7.6/src/fosslight_source/run_scancode.py` & `fosslight_source-1.7.7/src/fosslight_source/run_scancode.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.7.6/src/fosslight_source/run_scanoss.py` & `fosslight_source-1.7.7/src/fosslight_source/run_scanoss.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.7.6/src/fosslight_source/run_spdx_extractor.py` & `fosslight_source-1.7.7/src/fosslight_source/run_spdx_extractor.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.7.6/src/fosslight_source.egg-info/PKG-INFO` & `fosslight_source-1.7.7/src/fosslight_source.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-source
-Version: 1.7.6
+Version: 1.7.7
 Summary: FOSSLight Source Scanner
 Home-page: https://github.com/fosslight/fosslight_source_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_source_scanner
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight-source Version: 1.7.6 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight-source Version: 1.7.7 Summary: FOSSLight
 Source Scanner Home-page: https://github.com/fosslight/fosslight_source_scanner
 Author: LG Electronics License: Apache-2.0 Download-URL: https://github.com/
 fosslight/fosslight_source_scanner Description:
                                                                        _[_K_o_r_e_a_n_]
 # FOSSLight Source Scanner [FOSSLight Source Scanner is released under the
 Apache-2.0 License.][Current python package version.][https://img.shields.io/
 pypi/pyversions/fosslight_source][![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_source-1.7.6/src/fosslight_source.egg-info/SOURCES.txt` & `fosslight_source-1.7.7/src/fosslight_source.egg-info/SOURCES.txt`

 * *Files identical despite different names*

