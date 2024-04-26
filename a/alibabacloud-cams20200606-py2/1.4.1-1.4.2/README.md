# Comparing `tmp/alibabacloud_cams20200606_py2-1.4.1.tar.gz` & `tmp/alibabacloud_cams20200606_py2-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cams20200606_py2-1.4.1.tar", last modified: Wed Apr 10 10:05:06 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cams20200606_py2-1.4.2.tar", last modified: Fri Apr 26 17:08:26 2024, max compression
```

## Comparing `alibabacloud_cams20200606_py2-1.4.1.tar` & `alibabacloud_cams20200606_py2-1.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/
--rw-r--r--   0 root         (0) root         (0)     1561 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   128469 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606/client.py
--rw-r--r--   0 root         (0) root         (0)   509532 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2024-04-10 10:05:06.000000 alibabacloud_cams20200606_py2-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   128469 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606/client.py
+-rw-r--r--   0 root         (0) root         (0)   509532 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-04-26 17:08:26.000000 alibabacloud_cams20200606_py2-1.4.2/setup.py
```

### Comparing `alibabacloud_cams20200606_py2-1.4.1/LICENSE` & `alibabacloud_cams20200606_py2-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606_py2-1.4.1/PKG-INFO` & `alibabacloud_cams20200606_py2-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cams20200606_py2
-Version: 1.4.1
+Version: 1.4.2
 Summary: Alibaba Cloud cams (20200606) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cams20200606_py2-1.4.1/README-CN.md` & `alibabacloud_cams20200606_py2-1.4.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606_py2-1.4.1/README.md` & `alibabacloud_cams20200606_py2-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606/client.py` & `alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606/models.py` & `alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_cams20200606_py2-1.4.1/alibabacloud_cams20200606_py2.egg-info/PKG-INFO` & `alibabacloud_cams20200606_py2-1.4.2/alibabacloud_cams20200606_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cams20200606-py2
-Version: 1.4.1
+Version: 1.4.2
 Summary: Alibaba Cloud cams (20200606) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cams20200606_py2-1.4.1/setup.py` & `alibabacloud_cams20200606_py2-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cams20200606_py2.
 
-Created on 10/04/2024
+Created on 26/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cams20200606"
 NAME = "alibabacloud_cams20200606_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cams (20200606) SDK Library for Python2"
```

