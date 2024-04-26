# Comparing `tmp/ifes_apt_tc_data_modeling-0.2.1.tar.gz` & `tmp/ifes_apt_tc_data_modeling-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifes_apt_tc_data_modeling-0.2.1.tar", last modified: Thu Mar 21 13:44:24 2024, max compression
+gzip compressed data, was "ifes_apt_tc_data_modeling-0.2.2.tar", last modified: Fri Apr 26 12:34:52 2024, max compression
```

## Comparing `ifes_apt_tc_data_modeling-0.2.1.tar` & `ifes_apt_tc_data_modeling-0.2.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11358 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/LICENSE.txt
--rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)    24838 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/PKG-INFO
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    10566 2024-03-21 10:55:35.000000 ifes_apt_tc_data_modeling-0.2.1/README.md
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.921803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/__init__.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.921803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4098 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/apt6_headers.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9966 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/apt6_reader.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    19518 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/apt6_sections.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    34047 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1581 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/apt6_utils.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/ato/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/ato/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7231 2024-03-21 13:06:21.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/ato/ato_reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/csv/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/csv/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2810 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/csv/csv_reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/env/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/env/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     5181 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/env/env_reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/epos/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/epos/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7320 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/epos/epos_reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/fig/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/fig/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4358 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/fig/fig_reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/imago/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/imago/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8777 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/imago/imago_reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/nexus/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/nexus/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1206 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/nexus/nx_field.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8928 2024-03-21 11:16:02.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/nexus/nx_ion.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/pos/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/pos/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3202 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/pos/pos_reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/pyccapt/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/pyccapt/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9597 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/pyccapt/pyccapt_reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/rng/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/rng/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7191 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/rng/rng_reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/rrng/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/rrng/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9076 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/rrng/rrng_reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1991 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/definitions.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1388 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/mmapped_io.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    16238 2024-03-21 11:19:42.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/molecular_ions.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)   211717 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      916 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/string_handling.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    12818 2024-03-21 10:53:00.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/utils.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling.egg-info/
--rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)    24838 2024-03-21 13:44:24.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling.egg-info/PKG-INFO
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1944 2024-03-21 13:44:24.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        1 2024-03-21 13:44:24.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling.egg-info/dependency_links.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      171 2024-03-21 13:44:24.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling.egg-info/requires.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       26 2024-03-21 13:44:24.000000 ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling.egg-info/top_level.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1302 2024-03-21 13:42:13.000000 ifes_apt_tc_data_modeling-0.2.1/pyproject.toml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       38 2024-03-21 13:44:24.925803 ifes_apt_tc_data_modeling-0.2.1/setup.cfg
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11358 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/LICENSE.txt
+-rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)    24706 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/PKG-INFO
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    10443 2024-04-26 12:30:16.000000 ifes_apt_tc_data_modeling-0.2.2/README.md
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.518282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/__init__.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.518282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4098 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/apt6_headers.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9966 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/apt6_reader.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    19518 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/apt6_sections.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    34047 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1581 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/apt6_utils.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.518282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/ato/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/ato/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7231 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/ato/ato_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.518282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/csv/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/csv/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2810 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/csv/csv_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.518282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/env/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/env/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     5181 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/env/env_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.518282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/epos/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/epos/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7320 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/epos/epos_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/fig/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/fig/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     4358 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/fig/fig_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/imago/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/imago/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8777 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/imago/imago_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/nexus/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/nexus/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1206 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/nexus/nx_field.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    12361 2024-04-26 12:30:16.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/nexus/nx_ion.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/pos/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/pos/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3202 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/pos/pos_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/pyccapt/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/pyccapt/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9597 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/pyccapt/pyccapt_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/rng/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/rng/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7191 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/rng/rng_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/rrng/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/rrng/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9842 2024-04-26 12:30:16.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/rrng/rrng_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      656 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1991 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/definitions.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1388 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/mmapped_io.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    16238 2024-04-26 09:20:29.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/molecular_ions.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)   211717 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      916 2024-04-26 07:35:24.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/string_handling.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    12819 2024-04-26 12:30:16.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/utils.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling.egg-info/
+-rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)    24706 2024-04-26 12:34:52.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling.egg-info/PKG-INFO
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1944 2024-04-26 12:34:52.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        1 2024-04-26 12:34:52.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      179 2024-04-26 12:34:52.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling.egg-info/requires.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       26 2024-04-26 12:34:52.000000 ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling.egg-info/top_level.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1317 2024-04-26 12:32:06.000000 ifes_apt_tc_data_modeling-0.2.2/pyproject.toml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       38 2024-04-26 12:34:52.522282 ifes_apt_tc_data_modeling-0.2.2/setup.cfg
```

### Comparing `ifes_apt_tc_data_modeling-0.2.1/LICENSE.txt` & `ifes_apt_tc_data_modeling-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/PKG-INFO` & `ifes_apt_tc_data_modeling-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifes_apt_tc_data_modeling
-Version: 0.2.1
+Version: 0.2.2
 Summary: Foster exchange about data models and work towards clear specifications of file formats and data models in the research fields of atom probe tomography and related field-ion microscopy (atom probe microscopy).
 Author: The NOMAD Authors
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -214,25 +214,26 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: h5py>=3.6.0
 Requires-Dist: numpy>=1.21.2
-Requires-Dist: pandas
-Requires-Dist: tables
 Requires-Dist: ase>=3.19.0
 Requires-Dist: radioactivedecay>=0.4.16
+Requires-Dist: pandas
+Requires-Dist: tables
 Requires-Dist: flatdict
 Requires-Dist: xmltodict
+Requires-Dist: jupyter
+Requires-Dist: jupyterlab
+Requires-Dist: jupyterlab_h5web
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: twine; extra == "dev"
-Requires-Dist: jupyterlab_h5web; extra == "dev"
-Requires-Dist: jupyterlab; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pycodestyle; extra == "dev"
 
 # ifes_apt_tc_data_modeling
 
 ## Mission:
@@ -268,48 +269,40 @@
 
 In some cases when using Python3.8, it was necessary to install python-numpy.
 Please consider this if you run into issues when continuing with this manual.
 
 ### Install the ifes_apt_tc_data_modeling modules as a user
 
 ```
-git clone git@github.com:atomprobe-tc/ifes_apt_tc_data_modeling.git
+git clone https://www.github.com/atomprobe-tc/ifes_apt_tc_data_modeling.git
 cd ifes_apt_tc_data_modeling
 python -m pip install --upgrade pip
-python -m pip install pip-tools
 python -m pip install -e .
 python -m pip install -e ".[dev]"
 python -m pip list
-```
-
-### Additional steps to perform when you are a developer
-
-```
-python -m pip install -e ".[dev]"
-python -m pip list
 jupyter-lab
 ```
 
 ## Context, status quo, file formats used for atom probe research
 A lack of detailed technical specifications of the file formats and a lack of usage of magic numbers as identifiers for specific file formats
 are a key blocker to parsing and semantic interpretation of information content stored in current file formats within the research field of
 atom probe microscopy.
 
 A practical solution to raise at least awareness of this problem has been that scientists collect examples (instances)
 of files in respective formats. Pieces of information about the content and formatting of atom probe file formats were reported in the literature
 (e.g. in the books by D. Larson et al. https://doi.org/10.1007/978-1-4614-8721-0 or B. Gault et al. http://dx.doi.org/10.1007/978-1-4614-3436-8 ).
 Atom probers like D. Haley have contributed substantially through raising awareness of the issue within the community.
 
-AMETEK/Cameca is the key technology partner in atom probe. AMETEK has developed an open file format called APT which has improved
+AMETEK/Cameca is the key technology partner in atom probe. AMETEK/Cameca has developed an open file format called APT which has improved
 the accessibility of specific numerical data and some metadata. Individuals like M. Kühbach have driven the implementation and
-communication of parsers for this APT file format. There are ongoing efforts by both AMETEK and the scientific community to extent the APT file format
+communication of parsers for this APT file format. There are ongoing efforts by both AMETEK/Cameca and the scientific community to extent the APT file format
 with additional metadata. The main motivation behind these newer efforts is to improve the interoperability between research data collected
 within the IVAS/APSuite software and third-party software including research data management systems.
 Currently, most metadata have to be entered manually via e.g. electronic lab notebooks if one were to use or register atom probe
-data in solutions other than those developed by AMETEK.
+data in solutions other than those developed by AMETEK/Cameca.
 
 Nowadays, there is a global desire, a push by research funding agencies, and an increased interest of atom probers
 to make their research data and knowledge generation process better matching and more completely aligned to the aims
 and practices of the F.A.I.R. principles of research data stewardship and FAIR4RS research software development.
 
 Therefore, it is useful to exchange more details about data models and file formats. Otherwise, it is not foreseeable
 how atom probe data can be made really interoperable with electronic lab notebooks, research data management
```

### Comparing `ifes_apt_tc_data_modeling-0.2.1/README.md` & `ifes_apt_tc_data_modeling-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,48 +33,40 @@
 
 In some cases when using Python3.8, it was necessary to install python-numpy.
 Please consider this if you run into issues when continuing with this manual.
 
 ### Install the ifes_apt_tc_data_modeling modules as a user
 
 ```
-git clone git@github.com:atomprobe-tc/ifes_apt_tc_data_modeling.git
+git clone https://www.github.com/atomprobe-tc/ifes_apt_tc_data_modeling.git
 cd ifes_apt_tc_data_modeling
 python -m pip install --upgrade pip
-python -m pip install pip-tools
 python -m pip install -e .
 python -m pip install -e ".[dev]"
 python -m pip list
-```
-
-### Additional steps to perform when you are a developer
-
-```
-python -m pip install -e ".[dev]"
-python -m pip list
 jupyter-lab
 ```
 
 ## Context, status quo, file formats used for atom probe research
 A lack of detailed technical specifications of the file formats and a lack of usage of magic numbers as identifiers for specific file formats
 are a key blocker to parsing and semantic interpretation of information content stored in current file formats within the research field of
 atom probe microscopy.
 
 A practical solution to raise at least awareness of this problem has been that scientists collect examples (instances)
 of files in respective formats. Pieces of information about the content and formatting of atom probe file formats were reported in the literature
 (e.g. in the books by D. Larson et al. https://doi.org/10.1007/978-1-4614-8721-0 or B. Gault et al. http://dx.doi.org/10.1007/978-1-4614-3436-8 ).
 Atom probers like D. Haley have contributed substantially through raising awareness of the issue within the community.
 
-AMETEK/Cameca is the key technology partner in atom probe. AMETEK has developed an open file format called APT which has improved
+AMETEK/Cameca is the key technology partner in atom probe. AMETEK/Cameca has developed an open file format called APT which has improved
 the accessibility of specific numerical data and some metadata. Individuals like M. Kühbach have driven the implementation and
-communication of parsers for this APT file format. There are ongoing efforts by both AMETEK and the scientific community to extent the APT file format
+communication of parsers for this APT file format. There are ongoing efforts by both AMETEK/Cameca and the scientific community to extent the APT file format
 with additional metadata. The main motivation behind these newer efforts is to improve the interoperability between research data collected
 within the IVAS/APSuite software and third-party software including research data management systems.
 Currently, most metadata have to be entered manually via e.g. electronic lab notebooks if one were to use or register atom probe
-data in solutions other than those developed by AMETEK.
+data in solutions other than those developed by AMETEK/Cameca.
 
 Nowadays, there is a global desire, a push by research funding agencies, and an increased interest of atom probers
 to make their research data and knowledge generation process better matching and more completely aligned to the aims
 and practices of the F.A.I.R. principles of research data stewardship and FAIR4RS research software development.
 
 Therefore, it is useful to exchange more details about data models and file formats. Otherwise, it is not foreseeable
 how atom probe data can be made really interoperable with electronic lab notebooks, research data management
```

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/apt6_headers.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/apt6_headers.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/apt6_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/apt6_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/apt6_sections.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/apt6_sections.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/apt/apt6_utils.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/apt/apt6_utils.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/ato/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/ato/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/ato/ato_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/ato/ato_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/csv/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/csv/csv_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/csv/csv_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/env/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/env/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/env/env_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/env/env_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/epos/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/epos/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/epos/epos_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/epos/epos_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/fig/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/fig/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/fig/fig_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/fig/fig_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/imago/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/imago/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/imago/imago_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/imago/imago_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/nexus/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/nexus/nx_field.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/nexus/nx_field.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/nexus/nx_ion.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/nexus/nx_ion.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,14 +30,80 @@
 from ifes_apt_tc_data_modeling.utils.molecular_ions import \
     MolecularIonCandidate, MolecularIonBuilder, \
     PRACTICAL_ABUNDANCE, PRACTICAL_ABUNDANCE_PRODUCT, \
     PRACTICAL_MIN_HALF_LIFE, VERBOSE, SACRIFICE_ISOTOPIC_UNIQUENESS
 from ifes_apt_tc_data_modeling.nexus.nx_field import NxField
 
 
+def try_to_reduce_to_unique_definitions(inp: list) -> list:
+    """Try to reduce a set of (molecular) ion definitions to unique."""
+    for entry in inp:
+        if isinstance(entry, NxIon):
+            continue
+        else:
+            raise ValueError(f"Argument inp to try_to_reduce_to_unique_definitions needs to list of NxIon!")
+    unique = []
+    # unique if mqival does not overlap (but can touch) either side
+    # extrema of ranging definition and ivec is different or all 0
+    # from a scientific point of view we would like iontypes to be
+    # unique and ranges at most touching numerically but not overlapping
+    # as then for a given mass-to-charge-state value an ion can qualify
+    # to be an instance more than one iontype thus making the ranging
+    # ambiguous
+    visited = np.asarray(np.zeros(len(inp,)), bool)
+    for idx in np.arange(0, len(inp)):
+        if not visited[idx]:
+            # find all ranging definition value intersections with other ions
+            isect = []  # 
+            for jdx in np.concatenate((np.arange(0, idx), np.arange(idx + 1, len(inp)))):
+                if not visited[jdx]:
+                    if inp[idx].ranges.values[0, 1] < inp[jdx].ranges.values[0, 0] \
+                        or inp[idx].ranges.values[0, 0] > inp[jdx].ranges.values[0, 1]:
+                        continue
+                    else:
+                        # append only if exactly the same ivec
+                        idx_jdx_are_equal = True  # try to falsify
+                        for i in np.arange(0, MAX_NUMBER_OF_ATOMS_PER_ION):
+                            if inp[idx].nuclide_hash.values[i] != inp[jdx].nuclide_hash.values[i]:
+                                idx_jdx_are_equal = False
+                                break
+                        if idx_jdx_are_equal:
+                            isect.append(jdx)
+                            # that nuclide_hashes are the same is necessary for subsequent
+                            # processing of the range for these ions
+                        """
+                        else:
+                            print(f"Overlapping or exactly numerically aligned ranges for different ion types {idx}, {jdx}!")
+                            inp[idx].report()
+                            inp[jdx].report()
+                        """
+            # print(f"isect {isect}")
+            # if there are none accept this candidate for sure
+            visited[idx] = True
+            if len(isect) == 0:
+                # inp[idx].report()
+                unique.append(inp[idx])
+            else:
+                # combine range of isect candidates with the same nuclide_hash
+                mqmin = inp[idx].ranges.values[0, 0]
+                mqmax = inp[idx].ranges.values[0, 1]
+                for ids in isect:
+                    visited[ids] = True
+                    if inp[ids].ranges.values[0, 0] <= mqmin:
+                        mqmin = inp[ids].ranges.values[0, 0]
+                    if inp[ids].ranges.values[0, 1] >= mqmax:
+                        mqmax = inp[ids].ranges.values[0, 1]
+                joined_ion = NxIon(nuclide_hash=inp[idx].nuclide_hash.values, charge_state=0)
+                joined_ion.add_range(mqmin, mqmax)
+                joined_ion.comment.values = f"{inp[idx].comment.values} was combined with {isect}"
+                # joined_ion.report()
+                unique.append(joined_ion)
+    return unique
+
+
 class NxIon():
     """Representative of a NeXus base class NXion."""
 
     def __init__(self, *args, **kwargs):
         self.comment = NxField("", "")  # comment, use e.g. for label of custom ion types
         self.color = NxField("", "")  # color used by software which created the dataset
         self.volume = NxField("", "")  # volume value in range files
```

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/pos/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/pos/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/pos/pos_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/pos/pos_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/pyccapt/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/pyccapt/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/pyccapt/pyccapt_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/pyccapt/pyccapt_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/rng/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/rng/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/rng/rng_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/rng/rng_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/rrng/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/rrng/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/rrng/rrng_reader.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/rrng/rrng_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 """RRNG range file reader used by atom probe microscopists."""
 
 # pylint: disable=too-many-branches,too-many-statements,duplicate-code
 
 import re
 import numpy as np
 
-from ase.data import chemical_symbols
-from ifes_apt_tc_data_modeling.nexus.nx_ion import NxField, NxIon
+from ifes_apt_tc_data_modeling.nexus.nx_ion import NxField, NxIon, \
+    try_to_reduce_to_unique_definitions
 from ifes_apt_tc_data_modeling.utils.utils import \
     create_nuclide_hash, is_range_significant
 from ifes_apt_tc_data_modeling.utils.definitions import MQ_EPSILON
+from ifes_apt_tc_data_modeling.utils.molecular_ions import \
+    get_chemical_symbols
 
 
 def evaluate_rrng_range_line(i: int, line: str) -> dict:
     """Evaluate information content of a single range line."""
     # example line "Range7 = 42.8160 43.3110 vol:0.04543
     #     Al:1 O:1 Name: AlO Color:00FFFF"
     # according to DOI: 10.1007/978-1-4614-8721-0
@@ -43,21 +45,18 @@
                   "volume": np.float64(0.),
                   "color": "",
                   "name": ""}
 
     tmp = re.split(r"[\s=]+", line)
     if len(tmp) < 6:
         # raise ValueError(f"Line {line} does not contain all required fields {len(tmp)}!")
-        return info
-    if tmp[0] != f"Range{i}":
-        # raise ValueError(f"Line {line} has inconsistent line prefix {tmp[0]}!")
-        return info
+        return None
     if is_range_significant(np.float64(tmp[1]), np.float64(tmp[2])) is False:
         # raise ValueError(f"Line {line} insignificant range!")
-        return info
+        return None
     info["range"] = np.asarray([tmp[1], tmp[2]], np.float64)
 
     if tmp[3].lower().startswith("vol:"):
         info["volume"] = np.float64(re.split(r":", tmp[3])[1])
     if (tmp[-1].lower().startswith("color:")) and \
        (len(re.split(r":", tmp[-1])[1]) == 6):
         info["color"] = "#" + re.split(r":", tmp[-1])[1]
@@ -77,15 +76,15 @@
             # this captures properly formatted ranges with keyword
             # name whose name value is then however not a chemical
             # symbol but some user-defined string
             # this is a common habit to define custom names
         elif element_multiplicity[0].lower() not in ["vol", "color"]:
             # pick up what is an element name
             symbol = element_multiplicity[0]
-            if (symbol not in chemical_symbols) or (symbol == "X"):
+            if symbol not in get_chemical_symbols():
                 # raise ValueError(f"WARNING::Line {line} contains an invalid chemical symbol {symbol}!")
                 return info
             # if np.uint32(element_multiplicity[1]) <= 0:
                 # raise ValueError(f"Line {line} zero or negative multiplicity !")
             if np.uint32(element_multiplicity[1]) >= 256:
                 # raise ValueError(f"Line {line} unsupported high multiplicity "
                 #                  f"{np.uint32(element_multiplicity)}!")
@@ -94,23 +93,25 @@
                                       [symbol] * int(element_multiplicity[1]))
     return info
 
 
 class ReadRrngFileFormat():
     """Read *.rrng file format."""
 
-    def __init__(self, file_path: str):
+    def __init__(self, file_path: str, unique=False, verbose=False):
         """Initialize the class."""
         if (len(file_path) <= 5) or (file_path.lower().endswith(".rrng") is False):
             raise ImportError("WARNING::RRNG file incorrect file_path ending or file type!")
         self.file_path = file_path
         self.rrng: dict = {"ionnames": [],
                            "ranges": {},
                            "ions": {},
                            "molecular_ions": []}
+        self.unique = unique
+        self.verbose = verbose
         self.read_rrng()
 
     def read_rrng(self):
         """Read content of an RRNG range file."""
         with open(self.file_path, mode="r", encoding="utf8") as rrngf:
             txt = rrngf.read()
 
@@ -174,21 +175,35 @@
         if tmp[1].isnumeric() is False:
             raise ValueError(f"Line {txt_stripped[current_line_id]} [Ranges]/Number not a number!")
         number_of_ranges = int(tmp[1])
         if number_of_ranges <= 0:
             raise ValueError(f"Line {txt_stripped[current_line_id]}  No ranges defined!")
         current_line_id += 1
 
+        m_ions = []
         for jdx in np.arange(0, number_of_ranges):
+            if self.verbose:
+                print(f"{txt_stripped[current_line_id + jdx]}")
             dct = evaluate_rrng_range_line(jdx + 1, txt_stripped[current_line_id + jdx])
             if dct is None:
                 print(f"WARNING::RRNG line {txt_stripped[current_line_id + jdx]} is corrupted!")
                 continue
 
             m_ion = NxIon(nuclide_hash=create_nuclide_hash(dct["atoms"]), charge_state=0)
             m_ion.add_range(dct["range"][0], dct["range"][1])
             m_ion.comment = NxField(dct["name"], "")
+            m_ions.append(m_ion)
+            # this set may contain duplicates or overlapping ranges if ranging definitions are ambiguous like here https://doi.org/10.5281/zenodo.7788883
+
+        if self.unique:
+            unique_m_ions = try_to_reduce_to_unique_definitions(m_ions)
+            print(f"Found {len(m_ions)} ranging definitions, performed reduction to {len(unique_m_ions)} unique ones")
+        else:
+            unique_m_ions = m_ions.copy()
+            print(f"Found {len(m_ions)} ranging definitions, no reduction, {len(unique_m_ions)} remain.")
+        del m_ions
+
+        for m_ion in unique_m_ions:
             m_ion.apply_combinatorics()
             # m_ion.report()
-
             self.rrng["molecular_ions"].append(m_ion)
         print(f"{self.file_path} parsed successfully")
```

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/__init__.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/definitions.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/mmapped_io.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/mmapped_io.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/molecular_ions.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/molecular_ions.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/string_handling.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/string_handling.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling/utils/utils.py` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         return True
     return False
 
 
 def is_range_significant(left: np.float64, right: np.float64) -> bool:
     """Check if inclusive interval bounds [left, right] span a finite range."""
     if (np.float64(0.) <= left) and (np.float64(0.) <= right):
-        if (right - left) > MQ_EPSILON:
+        if (right - left) >= MQ_EPSILON:
             return True
     return False
 
 
 def is_convertible_to_isotope_hash(symbol: str):
     """Check if human_readable symbol is convertible into nuclide hash tribool."""
     case = re.search("^([A-Z])([a-z])?(-)([0-9]+)$", symbol)
```

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling.egg-info/PKG-INFO` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifes_apt_tc_data_modeling
-Version: 0.2.1
+Version: 0.2.2
 Summary: Foster exchange about data models and work towards clear specifications of file formats and data models in the research fields of atom probe tomography and related field-ion microscopy (atom probe microscopy).
 Author: The NOMAD Authors
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -214,25 +214,26 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: h5py>=3.6.0
 Requires-Dist: numpy>=1.21.2
-Requires-Dist: pandas
-Requires-Dist: tables
 Requires-Dist: ase>=3.19.0
 Requires-Dist: radioactivedecay>=0.4.16
+Requires-Dist: pandas
+Requires-Dist: tables
 Requires-Dist: flatdict
 Requires-Dist: xmltodict
+Requires-Dist: jupyter
+Requires-Dist: jupyterlab
+Requires-Dist: jupyterlab_h5web
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: twine; extra == "dev"
-Requires-Dist: jupyterlab_h5web; extra == "dev"
-Requires-Dist: jupyterlab; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pycodestyle; extra == "dev"
 
 # ifes_apt_tc_data_modeling
 
 ## Mission:
@@ -268,48 +269,40 @@
 
 In some cases when using Python3.8, it was necessary to install python-numpy.
 Please consider this if you run into issues when continuing with this manual.
 
 ### Install the ifes_apt_tc_data_modeling modules as a user
 
 ```
-git clone git@github.com:atomprobe-tc/ifes_apt_tc_data_modeling.git
+git clone https://www.github.com/atomprobe-tc/ifes_apt_tc_data_modeling.git
 cd ifes_apt_tc_data_modeling
 python -m pip install --upgrade pip
-python -m pip install pip-tools
 python -m pip install -e .
 python -m pip install -e ".[dev]"
 python -m pip list
-```
-
-### Additional steps to perform when you are a developer
-
-```
-python -m pip install -e ".[dev]"
-python -m pip list
 jupyter-lab
 ```
 
 ## Context, status quo, file formats used for atom probe research
 A lack of detailed technical specifications of the file formats and a lack of usage of magic numbers as identifiers for specific file formats
 are a key blocker to parsing and semantic interpretation of information content stored in current file formats within the research field of
 atom probe microscopy.
 
 A practical solution to raise at least awareness of this problem has been that scientists collect examples (instances)
 of files in respective formats. Pieces of information about the content and formatting of atom probe file formats were reported in the literature
 (e.g. in the books by D. Larson et al. https://doi.org/10.1007/978-1-4614-8721-0 or B. Gault et al. http://dx.doi.org/10.1007/978-1-4614-3436-8 ).
 Atom probers like D. Haley have contributed substantially through raising awareness of the issue within the community.
 
-AMETEK/Cameca is the key technology partner in atom probe. AMETEK has developed an open file format called APT which has improved
+AMETEK/Cameca is the key technology partner in atom probe. AMETEK/Cameca has developed an open file format called APT which has improved
 the accessibility of specific numerical data and some metadata. Individuals like M. Kühbach have driven the implementation and
-communication of parsers for this APT file format. There are ongoing efforts by both AMETEK and the scientific community to extent the APT file format
+communication of parsers for this APT file format. There are ongoing efforts by both AMETEK/Cameca and the scientific community to extent the APT file format
 with additional metadata. The main motivation behind these newer efforts is to improve the interoperability between research data collected
 within the IVAS/APSuite software and third-party software including research data management systems.
 Currently, most metadata have to be entered manually via e.g. electronic lab notebooks if one were to use or register atom probe
-data in solutions other than those developed by AMETEK.
+data in solutions other than those developed by AMETEK/Cameca.
 
 Nowadays, there is a global desire, a push by research funding agencies, and an increased interest of atom probers
 to make their research data and knowledge generation process better matching and more completely aligned to the aims
 and practices of the F.A.I.R. principles of research data stewardship and FAIR4RS research software development.
 
 Therefore, it is useful to exchange more details about data models and file formats. Otherwise, it is not foreseeable
 how atom probe data can be made really interoperable with electronic lab notebooks, research data management
```

### Comparing `ifes_apt_tc_data_modeling-0.2.1/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt` & `ifes_apt_tc_data_modeling-0.2.2/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.2.1/pyproject.toml` & `ifes_apt_tc_data_modeling-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifes_apt_tc_data_modeling"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name = "The NOMAD Authors" },
 ]
 description = "Foster exchange about data models and work towards clear specifications of file formats and data models in the research fields of atom probe tomography and related field-ion microscopy (atom probe microscopy)."
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.8"
@@ -20,28 +20,29 @@
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "h5py>=3.6.0",
     "numpy>=1.21.2",
-    "pandas",
-    "tables",
     "ase>=3.19.0",
     "radioactivedecay>=0.4.16",
+    "pandas",
+    "tables",
     "flatdict",
-    "xmltodict"
+    "xmltodict",
+    "jupyter",
+    "jupyterlab",
+    "jupyterlab_h5web"
 ]
 
 [project.optional-dependencies]
 dev = [
     "pip-tools",
     "twine",
-    "jupyterlab_h5web",
-    "jupyterlab",
     "mypy",
     "pylint",
     "pycodestyle"
 ]
 
 # [tool.setuptools]
 # packages = ["apt", "ato", "epos", "fig", "imago", "nexus", "pos", "pyccapt", "rng", "rrng", "utils"]
```

