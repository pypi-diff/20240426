# Comparing `tmp/coinanalyse-1.0.1.tar.gz` & `tmp/coinanalyse-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinanalyse-1.0.1.tar", last modified: Fri Apr 26 09:35:26 2024, max compression
+gzip compressed data, was "coinanalyse-1.0.2.tar", last modified: Fri Apr 26 10:50:20 2024, max compression
```

## Comparing `coinanalyse-1.0.1.tar` & `coinanalyse-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 09:36:09.644942 coinanalyse-1.0.1/
--rw-rw-rw-   0        0        0     1068 2024-03-28 10:30:36.000000 coinanalyse-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      221 2024-04-26 09:36:09.642995 coinanalyse-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-26 09:36:09.644942 coinanalyse-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      373 2024-04-26 09:35:03.000000 coinanalyse-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:36:09.607955 coinanalyse-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 09:36:09.635217 coinanalyse-1.0.1/src/coinanalyse.egg-info/
--rw-rw-rw-   0        0        0      221 2024-04-26 09:36:09.000000 coinanalyse-1.0.1/src/coinanalyse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-26 09:36:09.000000 coinanalyse-1.0.1/src/coinanalyse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 09:36:09.000000 coinanalyse-1.0.1/src/coinanalyse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-26 09:36:09.000000 coinanalyse-1.0.1/src/coinanalyse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-26 09:36:09.000000 coinanalyse-1.0.1/src/coinanalyse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 10:50:52.730694 coinanalyse-1.0.2/
+-rw-rw-rw-   0        0        0     1068 2024-03-28 10:30:36.000000 coinanalyse-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      242 2024-04-26 10:50:52.728747 coinanalyse-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 10:50:52.696627 coinanalyse-1.0.2/coinanalyse/
+-rw-rw-rw-   0        0        0      877 2019-07-26 16:30:47.000000 coinanalyse-1.0.2/coinanalyse/colors.py
+-rw-rw-rw-   0        0        0      955 2019-07-26 16:30:47.000000 coinanalyse-1.0.2/coinanalyse/exporter.py
+-rw-rw-rw-   0        0        0      564 2019-07-26 16:30:47.000000 coinanalyse-1.0.2/coinanalyse/getQuark.py
+-rw-rw-rw-   0        0        0      764 2019-07-26 16:30:47.000000 coinanalyse-1.0.2/coinanalyse/getTransactions.py
+-rw-rw-rw-   0        0        0      535 2019-07-26 16:30:47.000000 coinanalyse-1.0.2/coinanalyse/prepareGraph.py
+-rw-rw-rw-   0        0        0      104 2019-07-26 16:30:47.000000 coinanalyse-1.0.2/coinanalyse/requester.py
+-rw-rw-rw-   0        0        0     1187 2019-07-26 16:30:47.000000 coinanalyse-1.0.2/coinanalyse/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 10:50:52.722906 coinanalyse-1.0.2/coinanalyse.egg-info/
+-rw-rw-rw-   0        0        0      242 2024-04-26 10:50:52.000000 coinanalyse-1.0.2/coinanalyse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-04-26 10:50:52.000000 coinanalyse-1.0.2/coinanalyse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 10:50:52.000000 coinanalyse-1.0.2/coinanalyse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-26 10:50:52.000000 coinanalyse-1.0.2/coinanalyse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-26 10:50:52.000000 coinanalyse-1.0.2/coinanalyse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 10:50:52.731667 coinanalyse-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      383 2024-04-26 10:50:51.000000 coinanalyse-1.0.2/setup.py
```

### Comparing `coinanalyse-1.0.1/LICENSE.txt` & `coinanalyse-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

