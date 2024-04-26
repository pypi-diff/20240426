# Comparing `tmp/cadcutils-1.5.2.1.tar.gz` & `tmp/cadcutils-1.5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadcutils-1.5.2.1.tar", last modified: Mon Apr 22 18:28:31 2024, max compression
+gzip compressed data, was "cadcutils-1.5.2.2.tar", last modified: Fri Apr 26 03:24:14 2024, max compression
```

## Comparing `cadcutils-1.5.2.1.tar` & `cadcutils-1.5.2.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:28:31.317948 cadcutils-1.5.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-22 18:28:31.317948 cadcutils-1.5.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:28:31.309949 cadcutils-1.5.2.1/cadcutils/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:28:31.313948 cadcutils-1.5.2.1/cadcutils/net/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14480 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9055 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:28:31.313948 cadcutils-1.5.2.1/cadcutils/net/group_xml/
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/group_property_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/group_property_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/group_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/group_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/groups_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/groups_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:28:31.317948 cadcutils-1.5.2.1/cadcutils/net/group_xml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/tests/test_group_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/tests/test_groups_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/tests/test_user_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/user_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/group_xml/user_writer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29291 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/groups_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/netutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:28:31.317948 cadcutils-1.5.2.1/cadcutils/net/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/tests/test_groups_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/tests/test_int_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/tests/test_netutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    66649 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/tests/test_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/tests/test_wscapabilities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    56188 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/ws.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12263 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/net/wscapabilities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8457 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/old_get_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:28:31.317948 cadcutils-1.5.2.1/cadcutils/util/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/util/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/cadcutils/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 18:28:30.000000 cadcutils-1.5.2.1/cadcutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:28:31.317948 cadcutils-1.5.2.1/cadcutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-22 18:28:31.000000 cadcutils-1.5.2.1/cadcutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-22 18:28:31.000000 cadcutils-1.5.2.1/cadcutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:28:31.000000 cadcutils-1.5.2.1/cadcutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-22 18:28:31.000000 cadcutils-1.5.2.1/cadcutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:28:31.000000 cadcutils-1.5.2.1/cadcutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 18:28:31.000000 cadcutils-1.5.2.1/cadcutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-22 18:28:31.000000 cadcutils-1.5.2.1/cadcutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-22 18:28:31.317948 cadcutils-1.5.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3082 2024-04-22 18:28:26.000000 cadcutils-1.5.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:24:14.691418 cadcutils-1.5.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-26 03:24:14.691418 cadcutils-1.5.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:24:14.683418 cadcutils-1.5.2.2/cadcutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:24:14.683418 cadcutils-1.5.2.2/cadcutils/net/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14480 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9055 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:24:14.687418 cadcutils-1.5.2.2/cadcutils/net/group_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/group_property_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/group_property_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/group_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/group_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/groups_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/groups_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:24:14.687418 cadcutils-1.5.2.2/cadcutils/net/group_xml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/tests/test_group_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/tests/test_groups_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/tests/test_user_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/user_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/group_xml/user_writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29291 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/groups_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/netutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:24:14.687418 cadcutils-1.5.2.2/cadcutils/net/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/tests/test_groups_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/tests/test_int_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/tests/test_netutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66719 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/tests/test_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/tests/test_wscapabilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57066 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/ws.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12263 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/net/wscapabilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8457 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/old_get_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:24:14.687418 cadcutils-1.5.2.2/cadcutils/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/cadcutils/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 03:24:13.000000 cadcutils-1.5.2.2/cadcutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:24:14.687418 cadcutils-1.5.2.2/cadcutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-26 03:24:14.000000 cadcutils-1.5.2.2/cadcutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-26 03:24:14.000000 cadcutils-1.5.2.2/cadcutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 03:24:14.000000 cadcutils-1.5.2.2/cadcutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-26 03:24:14.000000 cadcutils-1.5.2.2/cadcutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 03:24:14.000000 cadcutils-1.5.2.2/cadcutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-26 03:24:14.000000 cadcutils-1.5.2.2/cadcutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 03:24:14.000000 cadcutils-1.5.2.2/cadcutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-26 03:24:14.691418 cadcutils-1.5.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3082 2024-04-26 03:24:06.000000 cadcutils-1.5.2.2/setup.py
```

### Comparing `cadcutils-1.5.2.1/LICENSE` & `cadcutils-1.5.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/PKG-INFO` & `cadcutils-1.5.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadcutils
-Version: 1.5.2.1
+Version: 1.5.2.2
 Summary: Generic CADC Python libary of utilities
 Home-page: http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca
 Author: Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `cadcutils-1.5.2.1/README.rst` & `cadcutils-1.5.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/exceptions.py` & `cadcutils-1.5.2.2/cadcutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/__init__.py` & `cadcutils-1.5.2.2/cadcutils/net/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/auth.py` & `cadcutils-1.5.2.2/cadcutils/net/auth.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group.py` & `cadcutils-1.5.2.2/cadcutils/net/group.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/__init__.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/group_property_reader.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/group_property_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/group_property_writer.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/group_property_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/group_reader.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/group_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/group_writer.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/group_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/groups_reader.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/groups_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/groups_writer.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/groups_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/tests/test_group_reader_writer.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/tests/test_group_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/tests/test_groups_reader_writer.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/tests/test_groups_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/tests/test_user_reader_writer.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/tests/test_user_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/user_reader.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/user_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/group_xml/user_writer.py` & `cadcutils-1.5.2.2/cadcutils/net/group_xml/user_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/groups_client.py` & `cadcutils-1.5.2.2/cadcutils/net/groups_client.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/netutils.py` & `cadcutils-1.5.2.2/cadcutils/net/netutils.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/tests/test_auth.py` & `cadcutils-1.5.2.2/cadcutils/net/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/tests/test_group.py` & `cadcutils-1.5.2.2/cadcutils/net/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/tests/test_groups_client.py` & `cadcutils-1.5.2.2/cadcutils/net/tests/test_groups_client.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/tests/test_int_groups.py` & `cadcutils-1.5.2.2/cadcutils/net/tests/test_int_groups.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/tests/test_netutils.py` & `cadcutils-1.5.2.2/cadcutils/net/tests/test_netutils.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/tests/test_ws.py` & `cadcutils-1.5.2.2/cadcutils/net/tests/test_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,26 +458,26 @@
         session.put.assert_called_with(target_url, headers=expected_headers,
                                        data=ANY, verify=True)
 
         # pass the md5 in update small file
         session.put.reset_mock()
         rsp = client.upload_file(url=target_url, src=src.name,
                                  md5_checksum=content_md5)
-        assert ('file', content_md5) == rsp
+        assert ('file', content_md5, len(content)) == rsp
         session.put.assert_called_once()
         session.put.assert_called_with(target_url, headers=put_headers,
                                        data=ANY, verify=True)
 
         # make it fail the first attempt but succeed on the next
         session.put.reset_mock()
         session.put.side_effect = [exceptions.PreconditionFailedException,
                                    response]
         rsp = client.upload_file(url=target_url, src=src.name,
                                  md5_checksum=content_md5)
-        assert ('file', content_md5) == rsp
+        assert ('file', content_md5, len(content)) == rsp
         assert session.put.mock_calls == [
             call(target_url, headers=put_headers, data=ANY, verify=True),
             call(target_url, headers=put_headers, data=ANY, verify=True)]
 
         # fail on repeated BadRequests
         session.put.reset_mock()
         session.put.side_effect = [exceptions.PreconditionFailedException] * 4
@@ -532,15 +532,15 @@
             caller_header = {CONTENT_TYPE: TEXT_TYPE}
             # lower the threshold for "large" files so that the current test
             # files becomes large
             ws.MAX_MD5_COMPUTE_SIZE = 10
             # PUT headers do not contain the md5 anymore
             rsp = client.upload_file(url=target_url, src=src.name,
                                      headers=caller_header)
-            assert ('file', content_md5) == rsp
+            assert ('file', content_md5, len(content)) == rsp
             put_headers = {ws.HTTP_LENGTH: str(len(content)),
                            ws.PUT_TXN_OP: ws.PUT_TXN_START}
             commit_headers = {ws.PUT_TXN_ID: '123',
                               ws.PUT_TXN_OP: ws.PUT_TXN_COMMIT,
                               ws.HTTP_LENGTH: '0'}
             expected_put_headers = dict(caller_header)
             expected_put_headers.update(put_headers)
@@ -557,25 +557,25 @@
             del put_headers[ws.PUT_TXN_OP]
             session.put.reset_mock()
             rsp = client.upload_file(
                 url=target_url, src=src.name, md5_checksum=content_md5)
             net.add_md5_header(headers=put_headers, md5_checksum=content_md5)
             session.put.assert_called_with(target_url, headers=put_headers,
                                            data=ANY, verify=True)
-            assert ('file', content_md5) == rsp
+            assert ('file', content_md5, len(content)) == rsp
 
             # mimic a replacement where source and destination are identical
             session.put.reset_mock()
             head_headers = {}
             net.add_md5_header(head_headers, content_md5)
             head_response = Mock(headers=head_headers)
             session.head.return_value = head_response
             rsp = client.upload_file(url=target_url, src=src.name, md5_checksum=content_md5)
             session.put.assert_not_called()
-            assert ('file', content_md5) == rsp
+            assert ('file', content_md5, len(content)) == rsp
 
             # mimic md5 mismatch
             session.put.reset_mock()
             response_headers = {ws.PUT_TXN_ID: '123',
                                 ws.HTTP_LENGTH: str(len(content))}
             net.add_md5_header(response_headers, 'd41d8cd98f00b204e9800998ecf8427e')
             session.put.return_value = Mock(headers=response_headers)
```

### Comparing `cadcutils-1.5.2.1/cadcutils/net/tests/test_wscapabilities.py` & `cadcutils-1.5.2.2/cadcutils/net/tests/test_wscapabilities.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/net/ws.py` & `cadcutils-1.5.2.2/cadcutils/net/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -469,15 +469,15 @@
            at https://github.com/opencadc/storage-inventory/blob/master/minoc/PutTransaction.md
            :param url: URL to upload the file to
            :param src: name of the file to upload
            :param md5_checksum: optional md5 checksum of the file content. If
            available, the caller should set the attribute, otherwise the method
            might compute it (for small files) and introduce overhead.
            :param kwargs: other http attributes
-           :returns (name_of_uploaded_file, md5_checksum)
+           :returns (name_of_uploaded_file, md5_checksum, file_size)
            :throws: HttpExceptions
         """
         stat_info = os.stat(src)
         if stat_info.st_size == 0:
             raise ValueError('Cannot upload empty files')
         if HEADERS not in kwargs:
             kwargs[HEADERS] = {}
@@ -504,44 +504,47 @@
         if src_md5:
             # try a HEAD first on the destination
             try:
                 response = self._get_session().head(url)
                 response.raise_for_status()
                 dest_md5 = net.extract_md5(response.headers)
                 if dest_md5 and (dest_md5 == src_md5):
-                    self.logger.debug(
-                        'Source and destination identical for {}. Skip transfer'.format(src))
-                    return dest_name, dest_md5
+                    self.logger.info(
+                        'Source and destination identical for {}. Skip transfer!'.format(src))
+                    return dest_name, dest_md5, stat_info.st_size
             except Exception:
                 # continue
                 pass
             net.add_md5_header(headers=orig_headers, md5_checksum=src_md5)
             if stat_info.st_size < FILE_SEGMENT_THRESHOLD:
                 # no transactions needed.
                 retries = MD5_MISMATCH_RETRY
+                start = time.time()
                 while retries:
                     try:
                         with open(src, 'rb') as reader:
                             response = self._get_session().put(
                                 url,
                                 data=reader,
                                 verify=self.verify, **kwargs)
                         self.logger.debug('{} uploaded (HTTP {})'.format(
                             src, response.status_code))
                         dest_md5 = net.extract_md5(response.headers)
-                        return dest_name, dest_md5
+                        self._log_upload(src, start, stat_info.st_size)
+                        return dest_name, dest_md5, stat_info.st_size
                     except exceptions.PreconditionFailedException as e:
                         # retry as this is likely caused by md5 mismatch
                         if not retries:
                             raise e
                         retries -= 1
 
         if stat_info.st_size < FILE_SEGMENT_THRESHOLD:
             # one go upload with transaction
             retries = MD5_MISMATCH_RETRY
+            start = time.time()
             while retries:
                 with util.Md5File(src, 'rb') as reader:
                     kwargs[HEADERS] = combine_headers(
                         {PUT_TXN_OP: PUT_TXN_START})
                     response = self._get_session().put(
                         url,
                         data=reader,
@@ -568,15 +571,16 @@
                         raise exceptions.TransferException(msg)
                     # commit tran
                 kwargs[HEADERS] = combine_headers({
                     PUT_TXN_ID: trans_id,
                     PUT_TXN_OP: PUT_TXN_COMMIT,
                     HTTP_LENGTH: '0'})
                 self._get_session().put(url, verify=self.verify, **kwargs)
-                return dest_name, dest_md5
+                self._log_upload(src, start, stat_info.st_size)
+                return dest_name, dest_md5, stat_info.st_size
 
         # large file that requires multiple segments
         kwargs[HEADERS] = combine_headers({
             HTTP_LENGTH: '0',
             PUT_TXN_TOTAL_LENGTH: str(stat_info.st_size),
             PUT_TXN_OP: PUT_TXN_START})
         response = self._get_session().put(url,
@@ -588,14 +592,15 @@
         min_segment = response.headers.get(PUT_TXN_MIN_SEGMENT, None)
         max_segment = response.headers.get(PUT_TXN_MAX_SEGMENT, None)
         seg_size = self._get_segment_size(stat_info.st_size,
                                           min_segment,
                                           max_segment)
         current_size = 0
         last_digest = hashlib.md5()
+        start = time.time()
         try:
             # Obs -(-stat_info.st_size//seg_size) - ceiling division in PYTHON
             for segment in range(0, -(-stat_info.st_size//seg_size)):
                 cur_seg_size = min(seg_size,
                                    stat_info.st_size-segment*seg_size)
                 self.logger.debug('Sending segment {} of size {}'.format(
                     segment, cur_seg_size))
@@ -682,15 +687,24 @@
         # commit tran
         self.logger.debug('Commit transaction')
         kwargs[HEADERS] = combine_headers({
             PUT_TXN_ID: trans_id,
             PUT_TXN_OP: PUT_TXN_COMMIT,
             HTTP_LENGTH: '0'})
         self._get_session().put(url, verify=self.verify, **kwargs)
-        return dest_name, dest_md5
+        self._log_upload(src, start, stat_info.st_size)
+        return dest_name, dest_md5, stat_info.st_size
+
+    def _log_upload(self, src, start, size):
+        duration = time.time() - start
+        self.logger.info(
+            'Successfully uploaded file {} in {}s '
+            '(avg. speed: {}MB/s)'.format(
+                src, round(duration, 2),
+                round(size / 1024 / 1024 / duration, 2)))
 
     @staticmethod
     def _get_segment_size(file_size, min_segment, max_segment):
         segment_size = min(file_size, PREFERRED_SEGMENT_SIZE)
         if min_segment:
             segment_size = max(segment_size, int(min_segment))
         if max_segment:
@@ -727,34 +741,36 @@
            robust.
            :param url: URL to get the file from
            :param dest: name of the file to store it to. If it's the name of
            the directory to save it to, it will use the Content-Disposition for
            the file name. By default, it saves the file in the current
            directory.
            :param kwargs: other http attributes
-           :return: (file_name, md5_checksum)
+           :return: (file_name, md5_checksum, file_size)
            :throws: HttpExceptions
 
         """
         response = self.get(url, stream=True, **kwargs)
         src_md5 = net.extract_md5(response.headers)
         src_size = int(response.headers.get(HTTP_LENGTH, 0))
         content_disp = net.get_header_filename(response.headers)
         if hasattr(dest, 'read'):
             dest.write(response.raw.read())
-            return content_disp, src_md5
+            return content_disp, src_md5, src_size
         else:
             final_dest, temp_dest = self._resolve_destination_file(
                 dest=dest, src_md5=src_md5, default_file_name=content_disp)
             if os.path.isfile(final_dest) and \
                src_size == os.stat(final_dest).st_size and \
                src_md5 == \
                     hashlib.md5(open(final_dest, 'rb').read()).hexdigest():
                 # nothing to be done
-                return os.path.basename(final_dest), src_md5
+                self.logger.info(
+                    'Source and destination identical for {}. Skip transfer!'.format(final_dest))
+                return os.path.basename(final_dest), src_md5, src_size
             if src_md5 and src_size and os.path.isfile(temp_dest):
                 stat_info = os.stat(temp_dest)
                 if not stat_info.st_size or stat_info.st_size >= src_size:
                     # Note: the existence of a complete temporary file should
                     # be a bug. It's more likely that it's corrupted hence the
                     # removal below
                     os.remove(temp_dest)
@@ -780,17 +796,17 @@
                         actual_cr = response.headers.get('Content-Range', '')
                         if actual_cr != exp_cr:
                             self.logger.warning(
                                 'Content-Range expected {} vs '
                                 'received {}'.format(exp_cr, actual_cr))
             # need to send the original file content-length. The Range response
             # contains the content-length of the range.
-            dest_md5 = self._save_bytes(response, src_size, temp_dest, None)
+            dest_md5, dest_size = self._save_bytes(response, src_size, temp_dest, None)
             os.rename(temp_dest, final_dest)
-            return os.path.basename(final_dest), dest_md5
+            return os.path.basename(final_dest), dest_md5, dest_size
 
     def _save_bytes(self, response, src_length, dest_file, process_bytes=None):
         # requests automatically decompresses the data.
         # Tell it to do it only if it had to
         hash_md5 = hashlib.md5()
         src_md5 = net.extract_md5(response.headers)
 
@@ -869,15 +885,15 @@
         else:
             duration = time.time() - start
             self.logger.info(
                 'Successfully downloaded file {} in {}s '
                 '(avg. speed: {}MB/s)'.format(
                     dest_file, round(duration, 2),
                     round(dest_downloaded / 1024 / 1024 / duration, 2)))
-            return dest_md5
+            return dest_md5, dest_length
         if not src_length or not src_md5:
             # clean up the temporary file
             os.remove(dest_file)
         raise exceptions.TransferException(error_msg)
 
 
 def _check_server_version(supported_versions, server_header):
```

### Comparing `cadcutils-1.5.2.1/cadcutils/net/wscapabilities.py` & `cadcutils-1.5.2.2/cadcutils/net/wscapabilities.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/old_get_cert.py` & `cadcutils-1.5.2.2/cadcutils/old_get_cert.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/util/__init__.py` & `cadcutils-1.5.2.2/cadcutils/util/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/util/config.py` & `cadcutils-1.5.2.2/cadcutils/util/config.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils/util/utils.py` & `cadcutils-1.5.2.2/cadcutils/util/utils.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/cadcutils.egg-info/PKG-INFO` & `cadcutils-1.5.2.2/cadcutils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadcutils
-Version: 1.5.2.1
+Version: 1.5.2.2
 Summary: Generic CADC Python libary of utilities
 Home-page: http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca
 Author: Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `cadcutils-1.5.2.1/cadcutils.egg-info/SOURCES.txt` & `cadcutils-1.5.2.2/cadcutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.2.1/setup.cfg` & `cadcutils-1.5.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 long_description = Library of utilities. It includes generic utilities for logging and command line parsing, networking utilities, etc.
 author = Canadian Astronomy Data Centre
 author_email = cadc@nrc-cnrc.gc.ca
 license = AGPLv3
 url = http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca
 edit_on_github = False
 github_project = opencadc/cadctools
-version = 1.5.2.1
+version = 1.5.2.2
 
 [options]
 install_requires = 
 	setuptools>=36.0
 	requests>=2.8
 	lxml>=3.7.0
 	html2text
```

### Comparing `cadcutils-1.5.2.1/setup.py` & `cadcutils-1.5.2.2/setup.py`

 * *Files identical despite different names*

