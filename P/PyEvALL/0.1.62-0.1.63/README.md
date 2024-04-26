# Comparing `tmp/PyEvALL-0.1.62.tar.gz` & `tmp/PyEvALL-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEvALL-0.1.62.tar", last modified: Sun Apr  7 13:17:03 2024, max compression
+gzip compressed data, was "PyEvALL-0.1.63.tar", last modified: Fri Apr 26 18:13:56 2024, max compression
```

## Comparing `PyEvALL-0.1.62.tar` & `PyEvALL-0.1.63.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.027772 PyEvALL-0.1.62/
--rw-rw-rw-   0        0        0       24 2024-03-13 22:18:07.000000 PyEvALL-0.1.62/MANIFEST.in
--rw-rw-rw-   0        0        0      447 2024-04-07 13:17:03.027772 PyEvALL-0.1.62/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.004140 PyEvALL-0.1.62/PyEvALL.egg-info/
--rw-rw-rw-   0        0        0      447 2024-04-07 13:17:02.000000 PyEvALL-0.1.62/PyEvALL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2024-04-07 13:17:02.000000 PyEvALL-0.1.62/PyEvALL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 13:17:02.000000 PyEvALL-0.1.62/PyEvALL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-04-07 13:17:02.000000 PyEvALL-0.1.62/PyEvALL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 13:17:02.000000 PyEvALL-0.1.62/PyEvALL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    26380 2024-04-07 13:15:19.000000 PyEvALL-0.1.62/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.004140 PyEvALL-0.1.62/pyevall/
--rw-rw-rw-   0        0        0        0 2023-02-07 00:42:14.000000 PyEvALL-0.1.62/pyevall/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.004140 PyEvALL-0.1.62/pyevall/comparators/
--rw-rw-rw-   0        0        0        0 2022-08-28 10:43:21.000000 PyEvALL-0.1.62/pyevall/comparators/__init__.py
--rw-rw-rw-   0        0        0    15325 2024-04-07 06:02:05.000000 PyEvALL-0.1.62/pyevall/comparators/comparators.py
--rw-rw-rw-   0        0        0    21114 2024-04-07 13:08:09.000000 PyEvALL-0.1.62/pyevall/comparators/formats.py
--rw-rw-rw-   0        0        0     9855 2024-04-03 09:08:55.000000 PyEvALL-0.1.62/pyevall/evaluation.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.019763 PyEvALL-0.1.62/pyevall/metrics/
--rw-rw-rw-   0        0        0        0 2022-08-28 10:42:54.000000 PyEvALL-0.1.62/pyevall/metrics/__init__.py
--rw-rw-rw-   0        0        0     4187 2024-04-03 09:09:44.000000 PyEvALL-0.1.62/pyevall/metrics/metricfactory.py
--rw-rw-rw-   0        0        0    55383 2024-04-05 22:08:18.000000 PyEvALL-0.1.62/pyevall/metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.019763 PyEvALL-0.1.62/pyevall/reports/
--rw-rw-rw-   0        0        0        0 2022-08-28 10:42:12.000000 PyEvALL-0.1.62/pyevall/reports/__init__.py
--rw-rw-rw-   0        0        0    27269 2024-04-04 10:04:56.000000 PyEvALL-0.1.62/pyevall/reports/reports.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.019763 PyEvALL-0.1.62/pyevall/utils/
--rw-rw-rw-   0        0        0      479 2024-03-06 07:06:10.000000 PyEvALL-0.1.62/pyevall/utils/file.conf
--rw-rw-rw-   0        0        0     2459 2024-04-04 10:28:07.000000 PyEvALL-0.1.62/pyevall/utils/pyevall_keys_texts_reports.rep
--rw-rw-rw-   0        0        0     8000 2024-04-03 13:16:56.000000 PyEvALL-0.1.62/pyevall/utils/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-07 13:17:03.027772 PyEvALL-0.1.62/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-04-07 06:35:30.000000 PyEvALL-0.1.62/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:17:03.019763 PyEvALL-0.1.62/test/
--rw-rw-rw-   0        0        0    10405 2024-04-03 16:37:42.000000 PyEvALL-0.1.62/test/testformats.py
--rw-rw-rw-   0        0        0    11154 2024-04-03 20:01:38.000000 PyEvALL-0.1.62/test/testmetrics.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:13:56.982170 PyEvALL-0.1.63/
+-rw-rw-rw-   0        0        0       24 2024-03-13 22:18:07.000000 PyEvALL-0.1.63/MANIFEST.in
+-rw-rw-rw-   0        0        0     1254 2024-04-26 18:13:56.981170 PyEvALL-0.1.63/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 18:13:56.925051 PyEvALL-0.1.63/PyEvALL.egg-info/
+-rw-rw-rw-   0        0        0     1254 2024-04-26 18:13:56.000000 PyEvALL-0.1.63/PyEvALL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2024-04-26 18:13:56.000000 PyEvALL-0.1.63/PyEvALL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 18:13:56.000000 PyEvALL-0.1.63/PyEvALL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-04-26 18:13:56.000000 PyEvALL-0.1.63/PyEvALL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 18:13:56.000000 PyEvALL-0.1.63/PyEvALL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    26380 2024-04-07 13:15:19.000000 PyEvALL-0.1.63/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 18:13:56.934147 PyEvALL-0.1.63/pyevall/
+-rw-rw-rw-   0        0        0        0 2023-02-07 00:42:14.000000 PyEvALL-0.1.63/pyevall/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:13:56.944151 PyEvALL-0.1.63/pyevall/comparators/
+-rw-rw-rw-   0        0        0        0 2022-08-28 10:43:21.000000 PyEvALL-0.1.63/pyevall/comparators/__init__.py
+-rw-rw-rw-   0        0        0    15325 2024-04-20 16:40:21.000000 PyEvALL-0.1.63/pyevall/comparators/comparators.py
+-rw-rw-rw-   0        0        0    21114 2024-04-07 13:08:09.000000 PyEvALL-0.1.63/pyevall/comparators/formats.py
+-rw-rw-rw-   0        0        0     9855 2024-04-03 09:08:55.000000 PyEvALL-0.1.63/pyevall/evaluation.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:13:56.954151 PyEvALL-0.1.63/pyevall/metrics/
+-rw-rw-rw-   0        0        0        0 2022-08-28 10:42:54.000000 PyEvALL-0.1.63/pyevall/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4187 2024-04-03 09:09:44.000000 PyEvALL-0.1.63/pyevall/metrics/metricfactory.py
+-rw-rw-rw-   0        0        0    55383 2024-04-20 16:15:32.000000 PyEvALL-0.1.63/pyevall/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:13:56.962164 PyEvALL-0.1.63/pyevall/reports/
+-rw-rw-rw-   0        0        0        0 2022-08-28 10:42:12.000000 PyEvALL-0.1.63/pyevall/reports/__init__.py
+-rw-rw-rw-   0        0        0    27269 2024-04-04 10:04:56.000000 PyEvALL-0.1.63/pyevall/reports/reports.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:13:56.971165 PyEvALL-0.1.63/pyevall/utils/
+-rw-rw-rw-   0        0        0      479 2024-04-20 16:15:18.000000 PyEvALL-0.1.63/pyevall/utils/file.conf
+-rw-rw-rw-   0        0        0     2459 2024-04-04 10:28:07.000000 PyEvALL-0.1.63/pyevall/utils/pyevall_keys_texts_reports.rep
+-rw-rw-rw-   0        0        0     8014 2024-04-23 11:25:03.000000 PyEvALL-0.1.63/pyevall/utils/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-26 18:13:56.982170 PyEvALL-0.1.63/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2024-04-26 18:13:20.000000 PyEvALL-0.1.63/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:13:56.980171 PyEvALL-0.1.63/test/
+-rw-rw-rw-   0        0        0    10405 2024-04-03 16:37:42.000000 PyEvALL-0.1.63/test/testformats.py
+-rw-rw-rw-   0        0        0    11154 2024-04-03 20:01:38.000000 PyEvALL-0.1.63/test/testmetrics.py
```

### Comparing `PyEvALL-0.1.62/PyEvALL.egg-info/SOURCES.txt` & `PyEvALL-0.1.63/PyEvALL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.62/README.md` & `PyEvALL-0.1.63/README.md`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.62/pyevall/comparators/comparators.py` & `PyEvALL-0.1.63/pyevall/comparators/comparators.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.62/pyevall/comparators/formats.py` & `PyEvALL-0.1.63/pyevall/comparators/formats.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.62/pyevall/evaluation.py` & `PyEvALL-0.1.63/pyevall/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.62/pyevall/metrics/metricfactory.py` & `PyEvALL-0.1.63/pyevall/metrics/metricfactory.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.62/pyevall/metrics/metrics.py` & `PyEvALL-0.1.63/pyevall/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.62/pyevall/reports/reports.py` & `PyEvALL-0.1.63/pyevall/reports/reports.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.62/pyevall/utils/pyevall_keys_texts_reports.rep` & `PyEvALL-0.1.63/pyevall/utils/pyevall_keys_texts_reports.rep`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.62/pyevall/utils/utils.py` & `PyEvALL-0.1.63/pyevall/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             "type": "object",
             "properties": {
                 "test_case": {"type": "string"},
                 "id":{"type": "string"},
                 "value": {
                     "anyOf": [
                         {"type": "string"},
-                        {"type": "array", "items": {"type": "string"}},
+                        {"type": "array", "items": {"type": "string"},"minItems": 1},
                         {"type": "integer"},
                         {
                             "type": "object",
                             "patternProperties": {
                             "^.*$": {"type": "number"},    }
                         },
                     ]
```

### Comparing `PyEvALL-0.1.62/test/testformats.py` & `PyEvALL-0.1.63/test/testformats.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.62/test/testmetrics.py` & `PyEvALL-0.1.63/test/testmetrics.py`

 * *Files identical despite different names*

