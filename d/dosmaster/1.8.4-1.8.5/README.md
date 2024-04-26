# Comparing `tmp/dosmaster-1.8.4.tar.gz` & `tmp/dosmaster-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.8.4.tar", last modified: Wed Apr 24 18:13:33 2024, max compression
+gzip compressed data, was "dist/dosmaster-1.8.5.tar", last modified: Fri Apr 26 15:28:43 2024, max compression
```

## Comparing `dosmaster-1.8.4.tar` & `dosmaster-1.8.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1069 2024-04-24 17:32:35.000000 dosmaster-1.8.4/LICENSE
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      214 2024-03-11 04:31:06.000000 dosmaster-1.8.4/MANIFEST.in
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      719 2024-04-24 18:13:33.000000 dosmaster-1.8.4/PKG-INFO
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2944 2024-04-24 18:11:32.000000 dosmaster-1.8.4/README.md
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/__init__.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/base/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/base/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3535 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/base/data_generation.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5276 2024-03-11 04:39:50.000000 dosmaster-1.8.4/dosmaster/base/printer.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/custom_setting/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      288 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/custom_setting/example_default.yaml
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/custom_setting/example_figure_size_up.yaml
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/custom_setting/example_font_size_up.yaml
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/features/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4281 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/a_add_atom_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11865 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/b_dos_projection.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2128 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/c_dos_sum.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3189 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/d_average_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2404 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/e_remove_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/f_change_sign.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    12152 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/g_graph_editor.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5897 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/h_axis_optimization.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2061 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/i_import_custom_setting.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1241 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/j_save_custom_setting.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1963 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/k_import_dosmaster_data.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      961 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/l_save_dosmaster_data.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/fileparser/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/fileparser/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4777 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/fileparser/doscar_split.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/fileparser/procar_parser.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/fileparser/structure_parser.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/main/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2024-04-24 17:38:45.000000 dosmaster-1.8.4/dosmaster/main/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7598 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/main/dosmaster.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/mainplotter/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/mainplotter/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11921 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/mainplotter/dosplot.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/subplotter/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/subplotter/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/subplotter/colors.csv
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/subplotter/colortable.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7081 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/subplotter/dosplot_manager.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/subplotter/make_color_list.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster.egg-info/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      719 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/PKG-INFO
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1453 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/SOURCES.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/dependency_links.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/entry_points.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       66 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/requires.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/top_level.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2024-04-24 18:13:33.000000 dosmaster-1.8.4/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1403 2024-04-24 17:41:51.000000 dosmaster-1.8.4/setup.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-26 15:28:43.000000 dosmaster-1.8.5/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1069 2024-04-24 17:32:35.000000 dosmaster-1.8.5/LICENSE
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      214 2024-03-11 04:31:06.000000 dosmaster-1.8.5/MANIFEST.in
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      719 2024-04-26 15:28:43.000000 dosmaster-1.8.5/PKG-INFO
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2980 2024-04-26 15:26:24.000000 dosmaster-1.8.5/README.md
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/__init__.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster/base/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/base/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3535 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/base/data_generation.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5322 2024-04-26 15:25:24.000000 dosmaster-1.8.5/dosmaster/base/printer.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster/custom_setting/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      288 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/custom_setting/example_default.yaml
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/custom_setting/example_figure_size_up.yaml
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/custom_setting/example_font_size_up.yaml
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster/features/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4281 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/a_add_atom_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11865 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/b_dos_projection.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2128 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/c_dos_sum.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3189 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/d_average_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2404 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/e_remove_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/f_change_sign.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    12152 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/g_graph_editor.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5897 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/h_axis_optimization.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2061 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/i_import_custom_setting.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1241 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/j_save_custom_setting.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1963 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/k_import_dosmaster_data.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      961 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/features/l_save_dosmaster_data.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster/fileparser/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/fileparser/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4777 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/fileparser/doscar_split.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/fileparser/procar_parser.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/fileparser/structure_parser.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster/main/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2024-04-26 15:27:08.000000 dosmaster-1.8.5/dosmaster/main/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7598 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/main/dosmaster.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster/mainplotter/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/mainplotter/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11921 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/mainplotter/dosplot.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster/subplotter/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/subplotter/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/subplotter/colors.csv
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/subplotter/colortable.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7081 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/subplotter/dosplot_manager.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2024-03-11 04:33:19.000000 dosmaster-1.8.5/dosmaster/subplotter/make_color_list.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster.egg-info/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      719 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster.egg-info/PKG-INFO
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1453 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster.egg-info/entry_points.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       66 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster.egg-info/requires.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2024-04-26 15:28:43.000000 dosmaster-1.8.5/dosmaster.egg-info/top_level.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2024-04-26 15:28:43.000000 dosmaster-1.8.5/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1403 2024-04-24 17:41:51.000000 dosmaster-1.8.5/setup.py
```

### Comparing `dosmaster-1.8.4/LICENSE` & `dosmaster-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/PKG-INFO` & `dosmaster-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.8.4
+Version: 1.8.5
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim in CNMD
 Author-email: yjpark29@postech.ac.kr
 License: MIT
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.8.4/README.md` & `dosmaster-1.8.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
 ver 1.8.1 : Label 버그 수정, 각종 버그 수정, Setting 저장 및 불러오기 기능 구현, DOS plot 저장 및 불러오기 기능 구현, shift_x_axis 구현, 연속된 숫자 입력 기능 확장, legend display 여부 선택 가능
 
 ver 1.8.3 : ISPIN = 1 calculation 지원 및 각종 버그 수정
 
 ver 1.8.4 : Lisence 수정
 
+ver 1.8.5 : f orbital error 수정
+
 
 ## Features
 1) Add Atom DOS : 원하는 atom의 DOS를 추가합니다.
 2) DOS Projection : 특정 DOS를 원하는 orbital로 projection 시킵니다.
 3) Sum DOS : 특정 DOS들의 기여분을 합칩니다.
 4) Average DOS : 특정 DOS들의 기여분을 평균화합니다.
 5) Remove DOS : 특정 DOS를 지웁니다.
```

### Comparing `dosmaster-1.8.4/dosmaster/base/data_generation.py` & `dosmaster-1.8.5/dosmaster/base/data_generation.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/base/printer.py` & `dosmaster-1.8.5/dosmaster/base/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     else:
         print('                                                    ...                                                            ')
         #0. Run split_dos function
         dos_data_total, dos_data, is_spin = split_dos()
     
         if path.exists("PROCAR") == False:
             print('PROCAR file cannot be found. Now Dosmaster uses basic orbital list.')
-            orbital_list = ['s', 'py', 'pz', 'px', 'dxy', 'dyz', 'dz2', 'dxz', 'x2-y2']
+            orbital_list = ['s', 'py', 'pz', 'px', 'dxy', 'dyz', 'dz2', 'dxz', 'x2-y2', 'fxyz', 'fyz2', 'fz3', 'fxz2', 'fzx3', 'fx3']
     
         else:
             #1. Get orbital_list from PROCAR
             orbital_list = PROCAR_Parser('./PROCAR')
 
         #2. Convert to 2D list
         dos_data_total_list=[[dos_temp.e_f] + dos_temp.dos_values for dos_temp in dos_data_total]
```

### Comparing `dosmaster-1.8.4/dosmaster/features/a_add_atom_dos.py` & `dosmaster-1.8.5/dosmaster/features/a_add_atom_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/b_dos_projection.py` & `dosmaster-1.8.5/dosmaster/features/b_dos_projection.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/c_dos_sum.py` & `dosmaster-1.8.5/dosmaster/features/c_dos_sum.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/d_average_dos.py` & `dosmaster-1.8.5/dosmaster/features/d_average_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/e_remove_dos.py` & `dosmaster-1.8.5/dosmaster/features/e_remove_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/f_change_sign.py` & `dosmaster-1.8.5/dosmaster/features/f_change_sign.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/g_graph_editor.py` & `dosmaster-1.8.5/dosmaster/features/g_graph_editor.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/h_axis_optimization.py` & `dosmaster-1.8.5/dosmaster/features/h_axis_optimization.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/i_import_custom_setting.py` & `dosmaster-1.8.5/dosmaster/features/i_import_custom_setting.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/j_save_custom_setting.py` & `dosmaster-1.8.5/dosmaster/features/j_save_custom_setting.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/k_import_dosmaster_data.py` & `dosmaster-1.8.5/dosmaster/features/k_import_dosmaster_data.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/features/l_save_dosmaster_data.py` & `dosmaster-1.8.5/dosmaster/features/l_save_dosmaster_data.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/fileparser/doscar_split.py` & `dosmaster-1.8.5/dosmaster/fileparser/doscar_split.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/fileparser/structure_parser.py` & `dosmaster-1.8.5/dosmaster/fileparser/structure_parser.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/main/dosmaster.py` & `dosmaster-1.8.5/dosmaster/main/dosmaster.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/mainplotter/dosplot.py` & `dosmaster-1.8.5/dosmaster/mainplotter/dosplot.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/subplotter/colors.csv` & `dosmaster-1.8.5/dosmaster/subplotter/colors.csv`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/subplotter/colortable.py` & `dosmaster-1.8.5/dosmaster/subplotter/colortable.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/subplotter/dosplot_manager.py` & `dosmaster-1.8.5/dosmaster/subplotter/dosplot_manager.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster/subplotter/make_color_list.py` & `dosmaster-1.8.5/dosmaster/subplotter/make_color_list.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/dosmaster.egg-info/PKG-INFO` & `dosmaster-1.8.5/dosmaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.8.4
+Version: 1.8.5
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim in CNMD
 Author-email: yjpark29@postech.ac.kr
 License: MIT
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.8.4/dosmaster.egg-info/SOURCES.txt` & `dosmaster-1.8.5/dosmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.4/setup.py` & `dosmaster-1.8.5/setup.py`

 * *Files identical despite different names*

