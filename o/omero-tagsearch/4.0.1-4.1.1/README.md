# Comparing `tmp/omero-tagsearch-4.0.1.tar.gz` & `tmp/omero-tagsearch-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-tagsearch-4.0.1.tar", last modified: Mon Sep  4 14:56:13 2023, max compression
+gzip compressed data, was "omero-tagsearch-4.1.1.tar", last modified: Fri Apr 26 13:34:40 2024, max compression
```

## Comparing `omero-tagsearch-4.0.1.tar` & `omero-tagsearch-4.1.1.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.489821 omero-tagsearch-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (999)    34520 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (999)       95 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     5754 2023-09-04 14:56:13.489821 omero-tagsearch-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4370 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (999)        6 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.485821 omero-tagsearch-4.0.1/omero_tagsearch/
--rw-r--r--   0 runner    (1001) docker     (999)       63 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      179 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/apps.py
--rw-r--r--   0 runner    (1001) docker     (999)      423 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.485821 omero-tagsearch-4.0.1/omero_tagsearch/static/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.485821 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.485821 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.485821 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/
--rw-r--r--   0 runner    (1001) docker     (999)     3998 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.js
--rw-r--r--   0 runner    (1001) docker     (999)     1459 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.min.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.485821 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/
--rwxr-xr-x   0 runner    (1001) docker     (999)      646 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite.png
--rwxr-xr-x   0 runner    (1001) docker     (999)      872 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite@2x.png
--rwxr-xr-x   0 runner    (1001) docker     (999)    12936 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.css
--rwxr-xr-x   0 runner    (1001) docker     (999)    42443 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.js
--rwxr-xr-x   0 runner    (1001) docker     (999)    26966 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.min.js
--rwxr-xr-x   0 runner    (1001) docker     (999)    10751 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.min.css
--rwxr-xr-x   0 runner    (1001) docker     (999)    42886 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.js
--rwxr-xr-x   0 runner    (1001) docker     (999)    27375 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.min.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.489821 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/
--rwxr-xr-x   0 runner    (1001) docker     (999)     3467 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/chosen.png
--rwxr-xr-x   0 runner    (1001) docker     (999)     6709 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/oss-credit.png
--rwxr-xr-x   0 runner    (1001) docker     (999)     1492 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.css
--rwxr-xr-x   0 runner    (1001) docker     (999)     6659 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.js
--rwxr-xr-x   0 runner    (1001) docker     (999)     6928 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/style.css
--rwxr-xr-x   0 runner    (1001) docker     (999)    85742 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.html
--rwxr-xr-x   0 runner    (1001) docker     (999)    86196 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.proto.html
--rwxr-xr-x   0 runner    (1001) docker     (999)    12053 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/options.html
--rw-r--r--   0 runner    (1001) docker     (999)     6591 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen.order.jquery.js
--rw-r--r--   0 runner    (1001) docker     (999)    43811 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/jquery.form.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.489821 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/css/
--rw-r--r--   0 runner    (1001) docker     (999)     9604 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (999)     1679 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/css/webtagging_search.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.489821 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/
--rw-r--r--   0 runner    (1001) docker     (999)     1205 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/folder16.png
--rw-r--r--   0 runner    (1001) docker     (999)     1187 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/folder_image16.png
--rw-r--r--   0 runner    (1001) docker     (999)      382 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/folder_plate16.png
--rw-r--r--   0 runner    (1001) docker     (999)     1289 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/folder_screen16.png
--rw-r--r--   0 runner    (1001) docker     (999)      219 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/image16.png
--rw-r--r--   0 runner    (1001) docker     (999)     1197 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/run16.png
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.485821 omero-tagsearch-4.0.1/omero_tagsearch/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.489821 omero-tagsearch-4.0.1/omero_tagsearch/templates/omero_tagsearch/
--rw-r--r--   0 runner    (1001) docker     (999)       84 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/templates/omero_tagsearch/index.html
--rw-r--r--   0 runner    (1001) docker     (999)     9651 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/templates/omero_tagsearch/search_details.html
--rw-r--r--   0 runner    (1001) docker     (999)    10592 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/templates/omero_tagsearch/tagnav.html
--rw-r--r--   0 runner    (1001) docker     (999)     4344 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/templates/omero_tagsearch/tagnav_init.js.html
--rw-r--r--   0 runner    (1001) docker     (999)      282 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/urls.py
--rw-r--r--   0 runner    (1001) docker     (999)    15863 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/omero_tagsearch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 14:56:13.485821 omero-tagsearch-4.0.1/omero_tagsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     5754 2023-09-04 14:56:13.000000 omero-tagsearch-4.0.1/omero_tagsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2475 2023-09-04 14:56:13.000000 omero-tagsearch-4.0.1/omero_tagsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 14:56:13.000000 omero-tagsearch-4.0.1/omero_tagsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 14:56:13.000000 omero-tagsearch-4.0.1/omero_tagsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)       17 2023-09-04 14:56:13.000000 omero-tagsearch-4.0.1/omero_tagsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       16 2023-09-04 14:56:13.000000 omero-tagsearch-4.0.1/omero_tagsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      147 2023-09-04 14:56:13.489821 omero-tagsearch-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     2188 2023-09-04 14:56:12.000000 omero-tagsearch-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.090764 omero-tagsearch-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-26 13:34:40.090764 omero-tagsearch-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.082764 omero-tagsearch-4.1.1/omero_tagsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.078764 omero-tagsearch-4.1.1/omero_tagsearch/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.078764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.082764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.082764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.086764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      646 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      872 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite@2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12936 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42443 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26966 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10751 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42886 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27375 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.086764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3467 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/chosen.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6709 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/oss-credit.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6659 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6928 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/style.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    85742 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86196 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.proto.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12053 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/options.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen.order.jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43811 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/jquery.form.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.086764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/css/webtagging_search.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.086764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder_image16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder_plate16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder_screen16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/icon_user.png
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/image16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/run16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/well16.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.078764 omero-tagsearch-4.1.1/omero_tagsearch/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.090764 omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/search_details.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14273 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/tagnav.html
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/tagnav_init.js.html
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18192 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.082764 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-26 13:34:39.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-26 13:34:40.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:34:39.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:34:39.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 13:34:39.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 13:34:39.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-26 13:34:40.090764 omero-tagsearch-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/setup.py
```

### Comparing `omero-tagsearch-4.0.1/LICENSE.txt` & `omero-tagsearch-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/PKG-INFO` & `omero-tagsearch-4.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: omero-tagsearch
-Version: 4.0.1
+Version: 4.1.1
 Summary: OMERO webtagging tagsearch app
 Home-page: https://github.com/German-BioImaging/omero-tagsearch
 Author: D.P.W. Russell
 Author-email: dpwrussell@gmail.com
 Maintainer: Tom Boissonnet
 Maintainer-email: tom.boissonnet@hhu.de
 License: AGPL-3.0
-Download-URL: https://github.com/German-BioImaging/omero-tagsearch/archive/v4.0.1.tar.gz
+Download-URL: https://github.com/German-BioImaging/omero-tagsearch/archive/v4.1.1.tar.gz
 Keywords: OMERO.web,webtagging,tagsearch
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
@@ -24,34 +24,41 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Obsoletes: omero_webtagging_tagsearch
-Requires-Python: ~=3.5
+Requires-Python: >=3
 License-File: LICENSE.txt
 
+.. image:: https://github.com/German-BioImaging/omero-tagsearch/workflows/PyPI/badge.svg
+   :target: https://github.com/German-BioImaging/omero-tagsearch/actions
+
+.. image:: https://badge.fury.io/py/omero-tagsearch.svg
+    :target: https://badge.fury.io/py/omero-tagsearch
+
+
 OMERO.tagsearch
-================
+===============
 OMERO.tagsearch is a plugin for `OMERO.web <https://github.com/ome/omero-web>`_ that enables searching of data using tags, with the search continuously refined as available search terms are entered and further term suggestions based on the entered terms are offered. 
 This can be used in a way that is similar to navigating a file system hierarchy.
 
 This was formerly part of `OMERO.webtagging <https://github.com/German-BioImaging/webtagging>`_, the umbrella name for tools developed to enhance use of text annotations (tags) in OMERO.
 
 Requirements
 ============
 
 As Python 2 has now reached end-of-life, OMERO 5.6 now
 requires Python 3. With release 3.1.0 of tagsearch, the following are now required. To use tagsearch on older OMERO systems (running Python 2),
 please use versions older than 3.1.0.
 
-* Python 3.5 or later
+* Python 3.8 or later
 * omero-web 5.6 or later
-* django 1.11 or later
+* django 4.2 or later
 
 User Documentation
 ==================
 
 http://help.openmicroscopy.org/web-tagging.html
 
 
@@ -138,20 +145,20 @@
 
 OMERO.webtagging was created by Douglas P. W. Russell
 (dpwrussell@gmail.com) while at Oxford University and
 Harvard Medical School, then later extended by DPWR
 Consulting Ltd.
 
 These plugins were developed originally with the
-support of [Micron Advanced Bioimaging Unit](https://micronoxford.com/)
+support of `Micron Advanced Bioimaging Unit <https://micronoxford.com/>`_
 funded by the Wellcome Trust Strategic Award 091911,
-and [Open Microscopy](https://www.openmicroscopy.org/).
+and `Open Microscopy <https://www.openmicroscopy.org/>`_.
 
-Continued development was supported by [The Laboratory
-of Systems Pharmacology, Harvard Medical School](https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/research-program/) and
-[Research Computing, Harvard Medical School](https://it.hms.harvard.edu/our-services/research-computing).
+Continued development was supported by `The Laboratory
+of Systems Pharmacology, Harvard Medical School <https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/research-program/>`_ and
+`Research Computing, Harvard Medical School <https://it.hms.harvard.edu/our-services/research-computing>`_.
 
 Continued development was sponsored by
-[Micron Advanced Bioimaging Unit](https://micronoxford.com/)
+`Micron Advanced Bioimaging Unit <https://micronoxford.com/>`_
 funded by the Wellcome Trust Strategic Award 107457.
```

### Comparing `omero-tagsearch-4.0.1/README.rst` & `omero-tagsearch-4.1.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,31 @@
+.. image:: https://github.com/German-BioImaging/omero-tagsearch/workflows/PyPI/badge.svg
+   :target: https://github.com/German-BioImaging/omero-tagsearch/actions
+
+.. image:: https://badge.fury.io/py/omero-tagsearch.svg
+    :target: https://badge.fury.io/py/omero-tagsearch
+
+
 OMERO.tagsearch
-================
+===============
 OMERO.tagsearch is a plugin for `OMERO.web <https://github.com/ome/omero-web>`_ that enables searching of data using tags, with the search continuously refined as available search terms are entered and further term suggestions based on the entered terms are offered. 
 This can be used in a way that is similar to navigating a file system hierarchy.
 
 This was formerly part of `OMERO.webtagging <https://github.com/German-BioImaging/webtagging>`_, the umbrella name for tools developed to enhance use of text annotations (tags) in OMERO.
 
 Requirements
 ============
 
 As Python 2 has now reached end-of-life, OMERO 5.6 now
 requires Python 3. With release 3.1.0 of tagsearch, the following are now required. To use tagsearch on older OMERO systems (running Python 2),
 please use versions older than 3.1.0.
 
-* Python 3.5 or later
+* Python 3.8 or later
 * omero-web 5.6 or later
-* django 1.11 or later
+* django 4.2 or later
 
 User Documentation
 ==================
 
 http://help.openmicroscopy.org/web-tagging.html
 
 
@@ -105,18 +112,18 @@
 
 OMERO.webtagging was created by Douglas P. W. Russell
 (dpwrussell@gmail.com) while at Oxford University and
 Harvard Medical School, then later extended by DPWR
 Consulting Ltd.
 
 These plugins were developed originally with the
-support of [Micron Advanced Bioimaging Unit](https://micronoxford.com/)
+support of `Micron Advanced Bioimaging Unit <https://micronoxford.com/>`_
 funded by the Wellcome Trust Strategic Award 091911,
-and [Open Microscopy](https://www.openmicroscopy.org/).
+and `Open Microscopy <https://www.openmicroscopy.org/>`_.
 
-Continued development was supported by [The Laboratory
-of Systems Pharmacology, Harvard Medical School](https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/research-program/) and
-[Research Computing, Harvard Medical School](https://it.hms.harvard.edu/our-services/research-computing).
+Continued development was supported by `The Laboratory
+of Systems Pharmacology, Harvard Medical School <https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/research-program/>`_ and
+`Research Computing, Harvard Medical School <https://it.hms.harvard.edu/our-services/research-computing>`_.
 
 Continued development was sponsored by
-[Micron Advanced Bioimaging Unit](https://micronoxford.com/)
+`Micron Advanced Bioimaging Unit <https://micronoxford.com/>`_
 funded by the Wellcome Trust Strategic Award 107457.
```

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.js` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.min.js` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.min.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite.png` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite@2x.png` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.css` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.js` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.min.js` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.min.css` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.min.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.js` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.min.js` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.min.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/chosen.png` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/chosen.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/oss-credit.png` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/oss-credit.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.css` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.js` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/style.css` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/style.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.html` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.html`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.proto.html` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.proto.html`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/options.html` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/options.html`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/chosen.order.jquery.js` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen.order.jquery.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/3rd-party/jquery.form.js` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/jquery.form.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/css/bootstrap.css` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/folder16.png` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder16.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/folder_image16.png` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder_image16.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/folder_screen16.png` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder_screen16.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/static/tagsearch/image/run16.png` & `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/run16.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/templates/omero_tagsearch/search_details.html` & `omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/search_details.html`

 * *Files 14% similar despite different names*

```diff
@@ -49,21 +49,17 @@
                     var selected = $('tr.ui-selected', this);
                     OME.table_selection_changed(selected);
                 },
                 start: function(){
                 }
             });
 
-            // We init sorting (not cols 0 & 3) but don't sort by default
-            $("#dataTable").tablesorter({headers: { 0: { sorter: false}, 4: {sorter: false} } });
+            // We init sorting (not cols 0 & 5) but don't sort by default
+            $("#dataTable").tablesorter({headers: { 0: { sorter: false}, 5: {sorter: false} } });
 
-            $('input#id_search').quicksearch('table#dataTable tbody tr', {
-                'delay': 300,
-                'loader': 'span.loading'
-            });
         });
     </script>
 
     <style type="text/css">
         .search_thumb {
             max-width: 32px;
             max-height: 32px;
@@ -86,14 +82,15 @@
 
         <table id="dataTable" class="tablesorter">
             <thead>
                 <tr>
                     <th class="table_images">{% trans "Object" %}</th>
                     <th class="table_desc">{% trans "Name" %}</th>
                     <th class="table_date">{% trans "Import Date" %}</th>
+                    <th>{% trans "Owner" %}</th>
                     <th>{% trans "Group" %}</th>
                     <th>{% trans "Link" %}</th>
                 </tr>
             </thead>
             <tbody>
             <!-- NB: E.g. "#project-123 td.desc a" etc is used to update names if edited in right-panel 'editinplace.js' -->
             {% for byId in foundById %}
@@ -107,93 +104,114 @@
                         {% endif %}
                     </td>
                     <td class="desc">
                         <span style="color:red">ID: {{ c.id }}</span>
                         <a>{{ c.name|truncatebefor:"65" }}</a>
                     </td>
                     <td class="date">{{ c.creationEventDate }}</td>
+                    <td class="owner">{{ c.getOwnerFullName }}</td>
                     <td class="group">{{ c.getDetails.group.name.val }}</td>
                     <td><a href="{% url 'webindex' %}?show={{ byId.otype }}-{{ c.id }}" title="{% trans 'Show in hierarchy view' %}">
                         {% trans "Browse" %}
                     </a></td>
                 </tr>
                 {% endwith %}
             {% endfor %}
             {% for c in manager.containers.project %}
-                <tr id="project-{{ c.id }}" class="{{ c.getPermsCss }}">
+                <tr id="project-{{ c.id }}" class="{{ c.getPermsCss }} project_row">
                     <td class="image">
                         <img id="{{ c.id }}" src="{% static "webgateway/img/folder16.png" %}" alt="project" title="{{ c.name }}"/>
                     </td>
                     <td class="desc"><a>{{ c.name|truncatebefor:"65" }}</a></td>
                     <td class="date">{{ c.creationEventDate }}</td>
+                    <td class="owner">{{ c.getOwnerFullName }}</td>
                     <td class="group">{{ c.getDetails.group.name.val }}</td>
                     <td><a href="{% url 'webindex' %}?show=project-{{ c.id }}" title="{% trans 'Show in hierarchy view' %}">
                         {% trans "Browse" %}
                     </a></td>
                 </tr>
             {% endfor %}
             {% for c in manager.containers.screen %}
-                <tr id="screen-{{ c.id }}" class="{{ c.getPermsCss }}">
+                <tr id="screen-{{ c.id }}" class="{{ c.getPermsCss }} screen_row">
                     <td class="image">
                         <img id="{{ c.id }}" src="{% static "webclient/image/folder_screen16.png" %}" alt="screen" title="{{ c.name }}"/>
                     </td>
                     <td class="desc"><a>{{ c.name|truncatebefor:"65" }}</a></td>
                     <td class="date">{{ c.creationEventDate }}</td>
+                    <td class="owner">{{ c.getOwnerFullName }}</td>
                     <td class="group">{{ c.getDetails.group.name.val }}</td>
                     <td><a href="{% url 'webindex' %}?show=screen-{{ c.id }}" title="{% trans 'Show in hierarchy view' %}">
                         {% trans "Browse" %}
                     </a></td>
                 </tr>
             {% endfor %}
             {% for c in manager.containers.dataset %}
-                <tr id="dataset-{{ c.id }}" class="{{ c.getPermsCss }}">
+                <tr id="dataset-{{ c.id }}" class="{{ c.getPermsCss }} dataset_row">
                     <td class="image">
                         <img id="{{ c.id }}" src="{% static "webgateway/img/folder_image16.png" %}" alt="dataset" title="{{ c.name }}"/>
                     </td>
                     <td class="desc"><a>{{ c.name|truncatebefor:"65" }}</a></td>
                     <td class="date">{{ c.creationEventDate }}</td>
+                    <td class="owner">{{ c.getOwnerFullName }}</td>
                     <td class="group">{{ c.getDetails.group.name.val }}</td>
                     <td><a href="{% url 'webindex' %}?show=dataset-{{ c.id }}" title="{% trans 'Show in hierarchy view' %}">
                         {% trans "Browse" %}
                     </a></td>
                 </tr>
             {% endfor %}
             {% for c in manager.containers.plate %}
-                <tr id="plate-{{ c.id }}" class="{{ c.getPermsCss }}">
+                <tr id="plate-{{ c.id }}" class="{{ c.getPermsCss }} plate_row">
                     <td class="image">
                         <img id="{{ c.id }}" src="{% static "webclient/image/folder_plate16.png" %}" alt="plate" title="{{ c.name }}"/>
                     </td>
                     <td class="desc"><a>{{ c.name|truncatebefor:"65" }}</a></td>
                     <td class="date">{{ c.creationEventDate }}</td>
+                    <td class="owner">{{ c.getOwnerFullName }}</td>
                     <td class="group">{{ c.getDetails.group.name.val }}</td>
                     <td><a href="{% url 'webindex' %}?show=plate-{{ c.id }}" title="{% trans 'Show in hierarchy view' %}">
                         {% trans "Browse" %}
                     </a></td>
                 </tr>
             {% endfor %}
             {% for c in manager.containers.acquisition %}
-                <tr id="acquisition-{{ c.id }}" class="{{ c.getPermsCss }}">
+                <tr id="acquisition-{{ c.id }}" class="{{ c.getPermsCss }} acquisition_row">
                     <td class="image">
                         <img id="{{ c.id }}" src="{% static "webclient/image/run16.png" %}" alt="acquisition" title="{{ c.name }}"/>
                     </td>
                     <td class="desc"><a>{{ c.name|truncatebefor:"65" }}</a></td>
                     <td class="date">{{ c.creationEventDate }}</td>
+                    <td class="owner">{{ c.getOwnerFullName }}</td>
                     <td class="group">{{ c.getDetails.group.name.val }}</td>
                     <td><a href="{% url 'webindex' %}?show=acquisition-{{ c.id }}" title="{% trans 'Show in hierarchy view' %}">
                         {% trans "Browse" %}
                     </a></td>
                 </tr>
             {% endfor %}
+            {% for c in manager.containers.well %}
+                <tr id="well-{{ c.id }}" class="{{ c.getPermsCss }} well_row">
+                    <td class="image">
+                        <img id="{{ c.id }}" src="{% static "webclient/image/well16.png" %}" alt="well" title="{{ c.name }}"/>
+                    </td>
+                    <td class="desc"><a>{{ c.name|truncatebefor:"65" }}</a></td>
+                    <td class="date">{{ c.creationEventDate }}</td>
+                    <td class="owner">{{ c.getOwnerFullName }}</td>
+                    <td class="group">{{ c.getDetails.group.name.val }}</td>
+                    <td><a href="{% url 'webindex' %}?show=well-{{ c.id }}" title="{% trans 'Show in hierarchy view' %}">
+                        {% trans "Browse" %}
+                    </a></td>
+                </tr>
+            {% endfor %}
             {% for c in manager.containers.image %}
-                <tr id="image-{{ c.id }}" class="{{ c.getPermsCss }}">
+                <tr id="image-{{ c.id }}" class="{{ c.getPermsCss }} image_row">
                     <td class="image">
                         <img class="search_thumb" id="{{ c.id }}" src="{% url 'render_thumbnail_resize' 96 c.id  %}" alt="image" title="{{ c.name }}"/>
                     </td>
                     <td class="desc"><a>{{ c.name|truncatebefor:"65" }}</a></td>
                     <td class="date">{{ c.creationEventDate }}</td>
+                    <td class="owner">{{ c.getOwnerFullName }}</td>
                     <td class="group">{{ c.getDetails.group.name.val }}</td>
                     <td><a href="{% url 'webindex' %}?show=image-{{ c.id }}" title="{% trans 'Show in hierarchy view' %}">
                         {% trans "Browse" %}
                     </a></td>
                 </tr>
             {% endfor %}
             </tbody>
```

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/templates/omero_tagsearch/tagnav.html` & `omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/tagnav.html`

 * *Files 21% similar despite different names*

```diff
@@ -34,154 +34,181 @@
   <![endif]-->
 
 
 {% endblock %}
 
 {% block script %}
     {{ block.super }}
-    <script type="text/javascript" src="{% static "3rdparty/jquery.tooltip/jquery.tooltip.pack.js" %}"></script>
     <script src="{% static 'webclient/javascript/jquery.infieldlabel-0.1.js' %}" type="text/javascript"></script>
     <script type="text/javascript" src="{% static "3rdparty/jquery.tablesorter-2.0.3/jquery.tablesorter.js" %}"></script>
     <script type="text/javascript" src="{% static "3rdparty/jquery.quicksearch-1.0.js" %}"></script>
 
-    {# Different chosen than used elsewhere in OMERO because ordering needs a more recent version #}
+    <!-- Different chosen than used elsewhere in OMERO because ordering needs a more recent version -->
     <script src="{% static "tagsearch/3rd-party/chosen/chosen.jquery.js" %}"></script>
     <script src="{% static "tagsearch/3rd-party/chosen.order.jquery.js" %}"></script>
 
     <script type="text/javascript">
         $(document).ready(function()
             {
+
+                var objTypes = ['project', 'dataset', 'image', 'screen', 'plate', 'acquisition', 'well']
                 $("#id_selectedTags").chosen({placeholder_text:'Choose tags'});
+                $("#id_excludedTags").chosen({placeholder_text:'Choose tags to exclude'});
 
                 $(".searching_info").tooltip({
                     track: true,
                     delay: 0,
                     showURL: false,
                     opacity: 1,
                     fixPNG: true,
                     showBody: " - ",
                     top: -15,
                     left: 5
                 });
 
+                function change_row_display(checked, rowClass) {
+                    if (checked) {
+                        $(rowClass).show();
+                        $(rowClass).removeClass('hidfromcheckbox');
+                    } else {
+                        $(rowClass).hide();
+                        $(rowClass).addClass('hidfromcheckbox');
+                    }
+                }
+
                 // Form Submission
                 $("#tagSearchForm").ajaxForm({
                   beforeSubmit: function() {
                     // prevent submitting the form again while waiting
                     $("div#content_details").html('<p>{% trans "Loading data... please wait" %} <img src ="{% static "webgateway/img/spinner.gif" %}"/></p>');
                   },
                   success: function(data) {
                     $("div#content_details").html(data.html);
 
-                      if (data.project_count > 0) {
-                        $("#tagnav-project span").html(data.project_count);
-                      } else {
-                          $("#tagnav-project span").html('0');
-                      }
-
-                      if (data.dataset_count > 0) {
-                        $(".tagnav-dataset span").html(data.dataset_count);
-                      } else {
-                        $(".tagnav-dataset span").html('0');
-                      }
-
-                      if (data.screen_count > 0) {
-                        $(".tagnav-screen span").html(data.screen_count);
-                      } else {
-                        $(".tagnav-screen span").html('0');
-                      }
-
-                      if (data.plate_count > 0) {
-                        $(".tagnav-plate span").html(data.plate_count);
-                      } else {
-                        $(".tagnav-plate span").html('0');
-                      }
-
-                      if (data.acquisition_count > 0) {
-                        $(".tagnav-acquisition span").html(data.acquisition_count);
-                      } else {
-                        $(".tagnav-acquisition span").html('0');
-                      }
-
-                      if (data.image_count > 0) {
-                        $(".tagnav-image span").html(data.image_count);
-                      } else {
-                        $(".tagnav-image span").html('0');
-                      }
-
-                      if (data.preview) {
-                        $("#filtersearch").removeClass('hidden');
-                        OME.table_selection_changed();
-                      } else {
-                        $("#filtersearch").addClass('hidden');
-                      }
+                    objTypes.forEach(function(objtype) {
+                      $(".tagnav-"+objtype+" span").html(data.count[objtype]);
+                    });
 
+                    $("#filtersearch").removeClass('hidden');
+                    OME.table_selection_changed();
 
                     // Hide any options that are no longer possible and
                     // show any that have become possible
                     $("#id_selectedTags option").each(function() {
                       if (($.inArray(parseInt(this.value), data.navdata) == -1) && (data.navdata.length != 0)) {
                         $(this).hide();
                       } else {
                         $(this).css('display', '');
                       }
                     });
 
+                    $("#id_excludedTags option").each(function() {
+                      if (($.inArray(parseInt(this.value), data.navdata) == -1) && (data.navdata.length != 0)) {
+                        $(this).hide();
+                      } else {
+                        $(this).css('display', '');
+                      }
+                    });
+
                     // Preserve the order of the select because otherwise Chosen will show the same order as
                     // the underlying select. i.e. the original option ordering
-                    var selection = $('#id_selectedTags').getSelectionOrder();
-
+                    var selection_incl = $('#id_selectedTags').getSelectionOrder();
+                    var selection_excl = $('#id_excludedTags').getSelectionOrder();
                     // Update the chosen selector
                     $("#id_selectedTags").trigger("chosen:updated");
-                    // Old style chosen update
-                    // $("#id_selectedTags").trigger("liszt:updated");
-
+                    $("#id_excludedTags").trigger("chosen:updated");
                     // Restore the ordering
-                    $('#id_selectedTags').setSelectionOrder(selection);
+                    $('#id_selectedTags').setSelectionOrder(selection_incl);
+                    $("#id_excludedTags").setSelectionOrder(selection_excl);
 
+                    $('#id_search').quicksearch('table#dataTable tbody tr', {
+                        'delay': 300,
+                        'loader': 'span.loading',
+                        'show': function(){
+                          if (!$(this).hasClass('hidfromcheckbox')){
+                            $(this).show();
+                          }
+                        },
+                        'hide': function(){
+                          if (!$(this).hasClass('hidfromcheckbox')){
+                            $(this).hide();
+                          }
+                        }
+                    });
+
+                    objTypes.forEach(function(objtype) {
+                      change_row_display($('#id_view_'+objtype).is(":checked"), "."+objtype+"_row");
+                    });
+
+                    // Triggering the search and setting the delay
+                    $('#id_search').trigger('keyup');
+                  },
+                });
+
+                $('#id_operation').change(function() {
+                  if ($('#enableCheckbox').is(':checked')) {
+                    $("#tagSearchForm").submit();
                   }
                 });
 
-                // Selection change
                 $( "#id_selectedTags" ).chosen().change(function(event, params) {
-
-                  // Selection made
-                  if (params.selected) {
-                    // Instead of submitting, serialize the input data and load the url
+                  // Tag selection or deselection made
+                  if ((params.selected || params.deselected) && $('#enableCheckbox').is(':checked')) {
                     $("#tagSearchForm").submit();
-
-                  // Deselection made
-                  } else if (params.deselected) {
+                  }
+                });
+                $( "#id_excludedTags" ).chosen().change(function(event, params) {
+                  if ((params.selected || params.deselected) && $('#enableCheckbox').is(':checked')) {
                     $("#tagSearchForm").submit();
                   }
+                });
 
+                $('#enableCheckbox').change(function() {
+                  if ($(this).is(':checked')) {
+                    $('#tagSearchForm').submit();
+                  }
+                });
 
+                objTypes.forEach(function(objtype) {
+                  $('#id_view_'+objtype).change(function() {change_row_display($(this).is(":checked"), "."+objtype+"_row");});
                 });
 
-                // Preview change
-                $('#id_results_preview').change(function() {
-                    if($(this).is(":checked")) {
-                        // Check if there is anything to submit
-                        // Above Success should be able to handle no results though
-                        if ($("#id_selectedTags option:selected").length) {
-                          $("#tagSearchForm").submit();
-                        }
+                $("#filtersearch label").inFieldLabels();
 
-                    } else {
-                        $("div#content_details").empty();
-                        $("#filtersearch").addClass('hidden');
-                        // TODO Hide filter
+                OME.table_selection_changed();     // clear selection (hides acquisition & preview tabs)
+
+                $(".searching_info").tooltip({
+                    track: true,
+                    show: false,
+                    hide: false,
+                    items: '[data-content]',
+                    content: function() {
+                        return $(this).data('content');
                     }
                 });
 
+                $("#selectall_btn").click(function(){
+                    var do_select = $("#selectall_btn").text() === "Select all";
+                    objTypes.forEach(function(objtype) {
+                      _objclass = '#id_view_'+objtype
+                      if ($(_objclass).is(":checked") != do_select) {
+                        $(_objclass).prop("checked", do_select);
+                        change_row_display($(_objclass).is(":checked"), "."+objtype+"_row");
+                      }
+                    });
+
+                    if (do_select) {
+                      $("#selectall_btn").text("Deselect all");
+                    } else {
+                      $("#selectall_btn").text("Select all");
+                    }
 
-                $("#filtersearch label").inFieldLabels();
+                });
 
-                OME.table_selection_changed();     // clear selection (hides acquisition & preview tabs)
-        })
+            });
     </script>
 
 {% endblock %}
 
 {% block left %}
 
 
@@ -194,38 +221,74 @@
 
 <div id="searching">
   <div class="left_panel_inner">
       <form id="tagSearchForm" action="{% url 'wtsimages' %}" method="post" class="standard_form">{% csrf_token %}
           <h2>{% trans "Tag Search" %}</h2>
           {# {{ tagnav_form.as_p }} #}
           {{ tagnav_form.non_field_errors }}
+
+          {% if user_name %}
+            <div id="id_userName" class="tagnav-user">
+              <div class="tagnav-icon">&nbsp;</div>
+              &nbsp;<span>{{ user_name }}</span>
+            </div>
+          {% endif %}
+
           <div class="fieldWrapper">
-              <div class="tagSearchDivider">
-                  {{ tagnav_form.selectedTags.errors }}
-                  <label for="id_selectedTags">Selected Tags:</label>
-                  {{ tagnav_form.selectedTags }}
-                  <span class="searching_info"
-                    title="Tag Search - <small>Perform a query for Projects, Datasets and Images based on the tag specified. The query gets all Projects, Datasets and Images which have <b>all</b> of the specified tags.
-                    Each time a tag is added, the list of potential tags to add is reduced to those that overlap with the tags already specified.
-                    A count of results is shown in the search panel and at any time it is possible to show the Projects, Datasets and Images that match by turning on the <b>Preview<b></small>">
-                    <img src="{% static 'webgateway/img/help16.png' %}" />
-                  </span>
+                <div class="tagSearchDivider">
+                  <div class="field">
+                    {{ tagnav_form.selectedTags.errors }}
+                    <label for="id_selectedTags">Selected Tags:</label>
+                    {{ tagnav_form.selectedTags }}&nbsp;
+                    <span class="searching_info"
+                    data-content="Search objects annotated with selected tags.</br>Only the tags of the selected group & user are listed.</br>Multiple tags are combined according to the joining method.">
+                      <img class="search_tips__tag" src="{% static 'webgateway/img/help16.png' %}" />
+                    </span>
+                  </div><br/>
+                  <div class="field">
+                    {{ tagnav_form.excludedTags.errors }}
+                    <label for="id_excludedTags">Excluded Tags:</label>
+                    {{ tagnav_form.excludedTags }}&nbsp;
+                    <span class="searching_info"
+                    data-content="Remove from the results the objects annotated with excluded tags.</br>Only the tags of the selected group & user are listed.">
+                      <img class="search_tips__tag" src="{% static 'webgateway/img/help16.png' %}" />
+                    </span>
+                  </div><br/><br/>
+                  <div>
+                    <label for="id_operation">Joining method:</label>
+                    <span class="searching_info"
+                    data-content="AND: Get the objects with all selected tags.</br>OR: Get the objects with at least one selected tag.">
+                      <img class="search_tips__join" src="{% static 'webgateway/img/help16.png' %}" />
+                    </span>
+                    {{ tagnav_form.operation }}
+                  </div><br/>
               </div>
 
-              {{ tagnav_form.results_preview.errors }}
-              <label for="id_results_preview">Preview:</label>
-              {{ tagnav_form.results_preview }}
               <h2>Results</h2>
-              <ul>
-                  <li class="tagnav-project"><div class="tagnav-icon">&nbsp;</div>Project:&nbsp;<span>0</span></li>
-                  <li class="tagnav-dataset"><div class="tagnav-icon">&nbsp;</div>Dataset:&nbsp;<span>0</span></li>
-                  <li class="tagnav-screen"><div class="tagnav-icon">&nbsp;</div>Screen:&nbsp;<span>0</span></li>
-                  <li class="tagnav-plate"><div class="tagnav-icon">&nbsp;</div>Plate:&nbsp;<span>0</span></li>
-                  <li class="tagnav-acquisition"><div class="tagnav-icon">&nbsp;</div>Plate Acquisition/Run:&nbsp;<span>0</span></li>
-                  <li class="tagnav-image"><div class="tagnav-icon">&nbsp;</div>Image:&nbsp;<span>0</span></li>
+              <ul id="counts_list">
+                  <li class="tagnav-project">{{ tagnav_form.view_project }}<div class="tagnav-icon">&nbsp;</div>Project:&nbsp;<span>0</span></li>
+                  <li class="tagnav-dataset">{{ tagnav_form.view_dataset }}<div class="tagnav-icon">&nbsp;</div>Dataset:&nbsp;<span>0</span></li>
+                  <li class="tagnav-screen">{{ tagnav_form.view_screen }}<div class="tagnav-icon">&nbsp;</div>Screen:&nbsp;<span>0</span></li>
+                  <li class="tagnav-plate">{{ tagnav_form.view_plate }}<div class="tagnav-icon">&nbsp;</div>Plate:&nbsp;<span>0</span></li>
+                  <li class="tagnav-acquisition">{{ tagnav_form.view_acquisition }}<div class="tagnav-icon">&nbsp;</div>Run:&nbsp;<span>0</span></li>
+                  <li class="tagnav-well">{{ tagnav_form.view_well }}<div class="tagnav-icon">&nbsp;</div>Well:&nbsp;<span>0</span></li>
+                  <li class="tagnav-image">{{ tagnav_form.view_image }}<div class="tagnav-icon">&nbsp;</div>Image:&nbsp;<span>0</span></li>
+                  <li><button id="selectall_btn" type="button">Deselect all</button>&nbsp
+                     <span class="searching_info" data-content="Deselect object types to filter them out of the result view. This has no effect on the query sent to the server.">
+                       <img class="search_tips__join" src="{% static 'webgateway/img/help16.png' %}" />
+                     </span>
+                  </li>
+                  <li><br/><br/>
+                      <label>
+                        <input type="checkbox" id="enableCheckbox" checked> <span>Preview</span>
+                      </label>
+                      <span class="searching_info" data-content="Prevent queries from being sent to the server, thereby disabling the updating of the tag selection fields and results.">
+                        <img class="search_tips__join" src="{% static 'webgateway/img/help16.png' %}" />
+                      </span>
+                  </li>
               </ul>
 
           </div>
 
 
       </form>
```

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch/views.py` & `omero-tagsearch-4.1.1/omero_tagsearch/views.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import absolute_import
 from builtins import str
 import json
 import logging
+from collections import defaultdict
 from django.http import HttpResponse, HttpResponseRedirect
 from django.urls import reverse
 from django.template.loader import render_to_string
 from omeroweb.webclient.decorators import render_response, login_required
 from omero.sys import Parameters
 from omero.rtypes import rlong, rlist
 from omeroweb.webclient.views import switch_active_group
@@ -22,22 +23,23 @@
 
     # TODO Hardcode menu as search until I figure out what to do with menu
     menu = "search"
     template = "omero_tagsearch/tagnav.html"
 
     # tree support
     init = {"initially_open": None, "initially_select": []}
-    first_sel = None
+    selected = None
     initially_open_owner = None
 
     # E.g. backwards compatible support for
     # path=project=51|dataset=502|image=607 (select the image)
     path = request.GET.get("path", "")
     i = path.split("|")[-1]
-    if i.split("=")[0] in ("project", "dataset", "image", "screen", "plate", "tag"):
+    if i.split("=")[0] in ("project", "dataset", "image", "screen",
+                           "plate", "tag", "acquisition", "run", "well"):
         init["initially_select"].append(str(i).replace("=", "-"))
 
     # Now we support show=image-607|image-123  (multi-objects selected)
     show = request.GET.get("show", "")
     for i in show.split("|"):
         if i.split("-")[0] in (
             "project",
@@ -67,63 +69,65 @@
                 + init["initially_select"][0]
             )
 
         try:
             # set context to 'cross-group'
             conn.SERVICE_OPTS.setOmeroGroup("-1")
             if first_obj == "tag":
-                first_sel = conn.getObject("TagAnnotation", int(first_id))
+                selected = conn.getObject("TagAnnotation", int(first_id))
             else:
-                first_sel = conn.getObject(first_obj, int(first_id))
-                initially_open_owner = first_sel.details.owner.id.val
+                selected = conn.getObject(first_obj, int(first_id))
+                initially_open_owner = selected.details.owner.id.val
                 # Wells aren't in the tree, so we need parent...
                 if first_obj == "well":
-                    parentNode = first_sel.getWellSample().getPlateAcquisition()
+                    ws = selected.getWellSample()
+                    parent_node = ws.getPlateAcquisition()
                     ptype = "acquisition"
                     # No Acquisition for this well, use Plate instead
-                    if parentNode is None:
-                        parentNode = first_sel.getParent()
+                    if parent_node is None:
+                        parent_node = selected.getParent()
                         ptype = "plate"
-                    first_sel = parentNode
-                    init["initially_open"] = ["%s-%s" % (ptype, parentNode.getId())]
+                    selected = parent_node
+                    init["initially_open"] = [f"{ptype}-{parent_node.getId()}"]
                     init["initially_select"] = init["initially_open"][:]
-        except:
+        except Exception:
             # invalid id
             pass
         if first_obj not in ("project", "screen"):
             # need to see if first item has parents
-            if first_sel is not None:
-                for p in first_sel.getAncestry():
+            if selected is not None:
+                for p in selected.getAncestry():
                     # parents of tags must be tags (no OMERO_CLASS)
                     if first_obj == "tag":
                         init["initially_open"].insert(0, "tag-%s" % p.getId())
                     else:
                         init["initially_open"].insert(
                             0, "%s-%s" % (p.OMERO_CLASS.lower(), p.getId())
                         )
                         initially_open_owner = p.details.owner.id.val
                 if init["initially_open"][0].split("-")[0] == "image":
                     init["initially_open"].insert(0, "orphaned-0")
 
     # need to be sure that tree will be correct omero.group
-    if first_sel is not None:
-        switch_active_group(request, first_sel.details.group.id.val)
+    if selected is not None:
+        switch_active_group(request, selected.details.group.id.val)
 
     # search support
     global_search_form = GlobalSearchForm(data=request.GET.copy())
     if menu == "search":
         if global_search_form.is_valid():
             init["query"] = global_search_form.cleaned_data["search_query"]
 
     # get url without request string - used to refresh page after switch
     # user/group etc
     url = reverse(viewname="tagsearch")
 
     # validate experimenter is in the active group
-    active_group = request.session.get("active_group") or conn.getEventContext().groupId
+    active_group = (request.session.get("active_group")
+                    or conn.getEventContext().groupId)
     # prepare members of group...
     s = conn.groupSummary(active_group)
     leaders = s["leaders"]
     members = s["colleagues"]
     userIds = [u.id for u in leaders]
     userIds.extend([u.id for u in members])
     users = []
@@ -137,20 +141,21 @@
     user_id = request.GET.get("experimenter")
     if initially_open_owner is not None:
         # if we're not already showing 'All Members'...
         if request.session.get("user_id", None) != -1:
             user_id = initially_open_owner
     try:
         user_id = int(user_id)
-    except:
+    except Exception:
         user_id = None
 
     # Check is user_id is in a current group
     if (
-        user_id not in (set([x.id for x in leaders]) | set([x.id for x in members]))
+        user_id not in (set([x.id for x in leaders])
+                        | set([x.id for x in members]))
         and user_id != -1
     ):
         # All users in group is allowed
         user_id = None
 
     if user_id is None:
         # ... or check that current user is valid in active group
@@ -168,72 +173,108 @@
             if g.getName() not in ("user", "guest")
         ]
     else:
         myGroups = list(conn.getGroupsMemberOf())
     myGroups.sort(key=lambda x: x.getName().lower())
     new_container_form = ContainerForm()
 
+    fullname_d = {exp.getId(): exp for exp in leaders + members}
+    user_name = ""
+    if user_id != -1:
+        user_name = fullname_d[user_id].getFullName()
+
     # Create and set the form
 
-    params = Parameters()
     qs = conn.getQueryService()
     service_opts = conn.SERVICE_OPTS.copy()
     service_opts.setOmeroGroup(active_group)
 
-    def get_tags(obj):
+    def get_tagsets():
+        # Get tagsets for tag_ids
+        # Do not filter tagsets on user, as it's meant to be
+        # information added to tags
+
+        params = Parameters()
+        hql = (
+            """
+            SELECT DISTINCT link.child.id, tagset.textValue
+            FROM Annotation tagset
+            JOIN tagset.annotationLinks link
+            WHERE tagset.class IS TagAnnotation
+            """
+        )
+
+        return {
+            result[0].val: f" [{result[1].val}]"
+            for result in qs.projection(hql, params, service_opts)
+        }
 
+    def get_tags(obj, tagset_d):
         # Get tags
         # It is not sufficient to simply get the objects as there may be tags
         # which are not applied which don't really make sense to display
         # tags = list(self.conn.getObjects("TagAnnotation"))
+
+        params = Parameters()
         hql = (
             """
-            SELECT DISTINCT link.child.id, link.child.textValue
+            SELECT DISTINCT ann.id, ann.textValue
             FROM %sAnnotationLink link
-            WHERE link.child.class IS TagAnnotation
-            ORDER BY link.child.textValue
+            JOIN link.child ann
+            WHERE ann.class IS TagAnnotation
         """
             % obj
         )
 
+        if user_id != -1:
+            hql += " AND ann.details.owner.id = (:uid)"
+            params.map = {"uid": rlong(user_id)}
+
         return [
-            (result[0].val, result[1].val)
+            (result[0].val, result[1].val, tagset_d[result[0].val])
             for result in qs.projection(hql, params, service_opts)
         ]
 
+    tagset_d = defaultdict(str)
+    tagset_d.update(get_tagsets())
+
     # List of tuples (id, value)
-    tags = set(get_tags("Image"))
-    tags.update(get_tags("Dataset"))
-    tags.update(get_tags("Project"))
-    tags.update(get_tags("Plate"))
-    tags.update(get_tags("PlateAcquisition"))
-    tags.update(get_tags("Screen"))
+    tags = set(get_tags("Image", tagset_d))
+    tags.update(get_tags("Dataset", tagset_d))
+    tags.update(get_tags("Project", tagset_d))
+    tags.update(get_tags("Plate", tagset_d))
+    tags.update(get_tags("PlateAcquisition", tagset_d))
+    tags.update(get_tags("Screen", tagset_d))
+    tags.update(get_tags("Well", tagset_d))
 
     # Convert back to an ordered list and sort
     tags = list(tags)
-    tags.sort(key=lambda x: x[1].lower())
+    tags.sort(key=lambda x: (x[2].lower(), x[1].lower()))
+    tags = list(map(lambda t: (t[0], t[1] + t[2]), tags))
 
-    form = TagSearchForm(tags, conn, initial={"results_preview": True})
+    form = TagSearchForm(tags, conn, use_required_attribute=False)
 
     context = {
         "init": init,
         "myGroups": myGroups,
         "new_container_form": new_container_form,
         "global_search_form": global_search_form,
     }
     context["groups"] = myGroups
-    context["active_group"] = conn.getObject("ExperimenterGroup", int(active_group))
+    context["active_group"] = conn.getObject("ExperimenterGroup",
+                                             int(active_group))
     for g in context["groups"]:
         g.groupSummary()  # load leaders / members
     context["active_user"] = conn.getObject("Experimenter", int(user_id))
 
     context["isLeader"] = conn.isLeader()
     context["current_url"] = url
     context["template"] = template
     context["tagnav_form"] = form
+    context["user_name"] = user_name
 
     return context
 
 
 @login_required(setGroupContext=True)
 # TODO Figure out what happened to render_response as it wasn't working on
 # production
@@ -241,138 +282,146 @@
 def tag_image_search(request, conn=None, **kwargs):
     import time
 
     start = time.time()
     if request.method == "POST":
 
         selected_tags = [int(x) for x in request.POST.getlist("selectedTags")]
-        results_preview = bool(request.POST.get("results_preview"))
+        excluded_tags = [int(x) for x in request.POST.getlist("excludedTags")]
+        operation = request.POST.get("operation")
 
         # validate experimenter is in the active group
         active_group = (
-            request.session.get("active_group") or conn.getEventContext().groupId
+            request.session.get("active_group")
+            or conn.getEventContext().groupId
         )
         service_opts = conn.SERVICE_OPTS.copy()
         service_opts.setOmeroGroup(active_group)
 
-        def getObjectsWithAllAnnotations(obj_type, annids):
+        def get_annotated_obj(obj_type, in_ids, excl_ids):
             # Get the images that match
-            hql = (
-                "select link.parent.id from %sAnnotationLink link "
-                "where link.child.id in (:oids) "
-                "group by link.parent.id "
-                "having count (distinct link.child) = %s" % (obj_type, len(annids))
-            )
             params = Parameters()
             params.map = {}
-            params.map["oids"] = rlist([rlong(o) for o in set(annids)])
+            params.map["in_ids"] = rlist([rlong(o) for o in set(in_ids)])
+
+            hql = ("select link.parent.id from %sAnnotationLink link "
+                   "where link.child.id in (:in_ids) " % (obj_type))
+            if len(excl_ids) > 0:
+                params.map["ex_ids"] = rlist([rlong(o) for o in set(excl_ids)])
+                hql += (" and link.parent.id not in "
+                        "(select link.parent.id from %sAnnotationLink link "
+                        "where link.child.id in (:ex_ids)) " % (obj_type))
+
+            hql += "group by link.parent.id"
+            if operation == "AND":
+                hql += f" having count (distinct link.child) = {len(in_ids)}"
 
             qs = conn.getQueryService()
-            return [x[0].getValue() for x in qs.projection(hql, params, service_opts)]
+            return [x[0].getValue() for x in qs.projection(hql,
+                                                           params,
+                                                           service_opts)]
 
         context = {}
         html_response = ""
         remaining = set([])
 
         manager = {"containers": {}}
         preview = False
-        project_count = 0
-        dataset_count = 0
-        screen_count = 0
-        plate_count = 0
-        acquisition_count = 0
-        image_count = 0
-
+        count_d = {}
         if selected_tags:
-            image_ids = getObjectsWithAllAnnotations("Image", selected_tags)
-            context["image_count"] = len(image_ids)
-            image_count = len(image_ids)
-
-            dataset_ids = getObjectsWithAllAnnotations("Dataset", selected_tags)
-            context["dataset_count"] = len(dataset_ids)
-            dataset_count = len(dataset_ids)
-
-            project_ids = getObjectsWithAllAnnotations("Project", selected_tags)
-            context["project_count"] = len(project_ids)
-            project_count = len(project_ids)
-
-            screen_ids = getObjectsWithAllAnnotations("Screen", selected_tags)
-            context["screen_count"] = len(screen_ids)
-            screen_count = len(screen_ids)
-
-            plate_ids = getObjectsWithAllAnnotations("Plate", selected_tags)
-            context["plate_count"] = len(plate_ids)
-            plate_count = len(plate_ids)
+            image_ids = get_annotated_obj("Image", selected_tags,
+                                          excluded_tags)
+            count_d["image"] = len(image_ids)
+
+            dataset_ids = get_annotated_obj("Dataset", selected_tags,
+                                            excluded_tags)
+            count_d["dataset"] = len(dataset_ids)
+
+            project_ids = get_annotated_obj("Project", selected_tags,
+                                            excluded_tags)
+            count_d["project"] = len(project_ids)
+
+            screen_ids = get_annotated_obj("Screen", selected_tags,
+                                           excluded_tags)
+            count_d["screen"] = len(screen_ids)
+
+            plate_ids = get_annotated_obj("Plate", selected_tags,
+                                          excluded_tags)
+            count_d["plate"] = len(plate_ids)
+
+            well_ids = get_annotated_obj("Well", selected_tags,
+                                         excluded_tags)
+            count_d["well"] = len(well_ids)
+
+            acquisition_ids = get_annotated_obj("PlateAcquisition",
+                                                selected_tags, excluded_tags)
+            count_d["acquisition"] = len(acquisition_ids)
 
-            acquisition_ids = getObjectsWithAllAnnotations(
-                "PlateAcquisition", selected_tags
-            )
-            context["acquisition_count"] = len(acquisition_ids)
-            acquisition_count = len(acquisition_ids)
+            if image_ids:
+                images = conn.getObjects("Image", ids=image_ids)
+                manager["containers"]["image"] = list(images)
 
-            if results_preview:
-                if image_ids:
-                    images = conn.getObjects("Image", ids=image_ids)
-                    manager["containers"]["image"] = list(images)
+            if dataset_ids:
+                datasets = conn.getObjects("Dataset", ids=dataset_ids)
+                manager["containers"]["dataset"] = list(datasets)
 
-                if dataset_ids:
-                    datasets = conn.getObjects("Dataset", ids=dataset_ids)
-                    manager["containers"]["dataset"] = list(datasets)
+            if project_ids:
+                projects = conn.getObjects("Project", ids=project_ids)
+                manager["containers"]["project"] = list(projects)
 
-                if project_ids:
-                    projects = conn.getObjects("Project", ids=project_ids)
-                    manager["containers"]["project"] = list(projects)
+            if screen_ids:
+                screens = conn.getObjects("Screen", ids=screen_ids)
+                manager["containers"]["screen"] = list(screens)
 
-                if screen_ids:
-                    screens = conn.getObjects("Screen", ids=screen_ids)
-                    manager["containers"]["screen"] = list(screens)
+            if plate_ids:
+                plates = conn.getObjects("Plate", ids=plate_ids)
+                manager["containers"]["plate"] = list(plates)
 
-                if plate_ids:
-                    plates = conn.getObjects("Plate", ids=plate_ids)
-                    manager["containers"]["plate"] = list(plates)
+            if well_ids:
+                wells = []
+                for w in conn.getObjects("Well", ids=well_ids):
+                    w.name = f"{w.getParent().name} - {w.getWellPos()}"
+                    wells.append(w)
+                manager["containers"]["well"] = wells
 
-                if acquisition_ids:
-                    acquisitions = conn.getObjects(
-                        "PlateAcquisition", ids=acquisition_ids
-                    )
-                    manager["containers"]["acquisition"] = list(acquisitions)
-
-                manager["c_size"] = (
-                    len(image_ids)
-                    + len(dataset_ids)
-                    + len(project_ids)
-                    + len(screen_ids)
-                    + len(plate_ids)
-                    + len(acquisition_ids)
+            if acquisition_ids:
+                acquisitions = conn.getObjects(
+                    "PlateAcquisition", ids=acquisition_ids
                 )
-                if manager["c_size"] > 0:
-                    preview = True
+                manager["containers"]["acquisition"] = list(acquisitions)
+
+            manager["c_size"] = sum(count_d.values())
+            if manager["c_size"] > 0:
+                preview = True
 
             context["manager"] = manager
 
             html_response = render_to_string(
                 "omero_tagsearch/search_details.html", context
             )
 
             middle = time.time()
 
-            def getAnnotationsForObjects(obj_type, oids):
+            def get_objects_annotations(obj_type, oids):
                 # Get the images that match
-                hql = (
-                    "select distinct link.child.id from %sAnnotationLink link "
-                    "where link.parent.id in (:oids)" % obj_type
-                )
-
                 params = Parameters()
                 params.map = {}
-                params.map["oids"] = rlist([rlong(o) for o in oids])
+                hql = (
+                    "select distinct link.child.id " +
+                    "from %sAnnotationLink link " % obj_type
+                )
+                if operation == "AND":
+                    hql += "where link.parent.id in (:oids)"
+                    params.map["oids"] = rlist([rlong(o) for o in oids])
 
                 qs = conn.getQueryService()
                 return [
-                    result[0].val for result in qs.projection(hql, params, service_opts)
+                    result[0].val for result in qs.projection(hql,
+                                                              params,
+                                                              service_opts)
                 ]
 
             # Calculate remaining possible tag navigations
             # TODO Compare subquery to pass-in performance
             # sub_hql = """
             #     SELECT link.parent.id
             #     FROM ImageAnnotationLink link
@@ -382,46 +431,50 @@
             # """ % len(selected_tags)
             # hql = """
             #     SELECT DISTINCT link.child.id
             #     FROM ImageAnnotationLink link
             #     WHERE link.parent.id IN (%s)
             # """ % sub_hql
 
-            if image_ids:
-                remaining.update(getAnnotationsForObjects("Image", image_ids))
-            if dataset_ids:
-                remaining.update(getAnnotationsForObjects("Dataset", dataset_ids))
-            if project_ids:
-                remaining.update(getAnnotationsForObjects("Project", project_ids))
-            if acquisition_ids:
-                remaining.update(
-                    getAnnotationsForObjects("PlateAcquisition", acquisition_ids)
-                )
-            if plate_ids:
-                remaining.update(getAnnotationsForObjects("Plate", plate_ids))
-            if screen_ids:
-                remaining.update(getAnnotationsForObjects("Screen", screen_ids))
+            if operation == "AND":
+                if image_ids:
+                    remaining.update(get_objects_annotations("Image",
+                                                             image_ids))
+                if dataset_ids:
+                    remaining.update(get_objects_annotations("Dataset",
+                                                             dataset_ids))
+                if project_ids:
+                    remaining.update(get_objects_annotations("Project",
+                                                             project_ids))
+                if well_ids:
+                    remaining.update(get_objects_annotations("Well",
+                                                             well_ids))
+                if acquisition_ids:
+                    remaining.update(
+                        get_objects_annotations("PlateAcquisition",
+                                                acquisition_ids))
+                if plate_ids:
+                    remaining.update(get_objects_annotations("Plate",
+                                                             plate_ids))
+                if screen_ids:
+                    remaining.update(get_objects_annotations("Screen",
+                                                             screen_ids))
 
             end = time.time()
             logger.info(
                 "Tag Query Times. Preview: %ss, Remaining: %ss, Total:%ss"
                 % ((middle - start), (end - middle), (end - start))
             )
 
         # Return the navigation data and the html preview for display
         # return {"navdata": list(remaining), "html": html_response}
         return HttpResponse(
             json.dumps(
                 {
                     "navdata": list(remaining),
                     "preview": preview,
-                    "project_count": project_count,
-                    "dataset_count": dataset_count,
-                    "screen_count": screen_count,
-                    "plate_count": plate_count,
-                    "acquisition_count": acquisition_count,
-                    "image_count": image_count,
+                    "count": count_d,
                     "html": html_response,
                 }
             ),
             content_type="application/json",
         )
```

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch.egg-info/PKG-INFO` & `omero-tagsearch-4.1.1/omero_tagsearch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: omero-tagsearch
-Version: 4.0.1
+Version: 4.1.1
 Summary: OMERO webtagging tagsearch app
 Home-page: https://github.com/German-BioImaging/omero-tagsearch
 Author: D.P.W. Russell
 Author-email: dpwrussell@gmail.com
 Maintainer: Tom Boissonnet
 Maintainer-email: tom.boissonnet@hhu.de
 License: AGPL-3.0
-Download-URL: https://github.com/German-BioImaging/omero-tagsearch/archive/v4.0.1.tar.gz
+Download-URL: https://github.com/German-BioImaging/omero-tagsearch/archive/v4.1.1.tar.gz
 Keywords: OMERO.web,webtagging,tagsearch
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
@@ -24,34 +24,41 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Obsoletes: omero_webtagging_tagsearch
-Requires-Python: ~=3.5
+Requires-Python: >=3
 License-File: LICENSE.txt
 
+.. image:: https://github.com/German-BioImaging/omero-tagsearch/workflows/PyPI/badge.svg
+   :target: https://github.com/German-BioImaging/omero-tagsearch/actions
+
+.. image:: https://badge.fury.io/py/omero-tagsearch.svg
+    :target: https://badge.fury.io/py/omero-tagsearch
+
+
 OMERO.tagsearch
-================
+===============
 OMERO.tagsearch is a plugin for `OMERO.web <https://github.com/ome/omero-web>`_ that enables searching of data using tags, with the search continuously refined as available search terms are entered and further term suggestions based on the entered terms are offered. 
 This can be used in a way that is similar to navigating a file system hierarchy.
 
 This was formerly part of `OMERO.webtagging <https://github.com/German-BioImaging/webtagging>`_, the umbrella name for tools developed to enhance use of text annotations (tags) in OMERO.
 
 Requirements
 ============
 
 As Python 2 has now reached end-of-life, OMERO 5.6 now
 requires Python 3. With release 3.1.0 of tagsearch, the following are now required. To use tagsearch on older OMERO systems (running Python 2),
 please use versions older than 3.1.0.
 
-* Python 3.5 or later
+* Python 3.8 or later
 * omero-web 5.6 or later
-* django 1.11 or later
+* django 4.2 or later
 
 User Documentation
 ==================
 
 http://help.openmicroscopy.org/web-tagging.html
 
 
@@ -138,20 +145,20 @@
 
 OMERO.webtagging was created by Douglas P. W. Russell
 (dpwrussell@gmail.com) while at Oxford University and
 Harvard Medical School, then later extended by DPWR
 Consulting Ltd.
 
 These plugins were developed originally with the
-support of [Micron Advanced Bioimaging Unit](https://micronoxford.com/)
+support of `Micron Advanced Bioimaging Unit <https://micronoxford.com/>`_
 funded by the Wellcome Trust Strategic Award 091911,
-and [Open Microscopy](https://www.openmicroscopy.org/).
+and `Open Microscopy <https://www.openmicroscopy.org/>`_.
 
-Continued development was supported by [The Laboratory
-of Systems Pharmacology, Harvard Medical School](https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/research-program/) and
-[Research Computing, Harvard Medical School](https://it.hms.harvard.edu/our-services/research-computing).
+Continued development was supported by `The Laboratory
+of Systems Pharmacology, Harvard Medical School <https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/research-program/>`_ and
+`Research Computing, Harvard Medical School <https://it.hms.harvard.edu/our-services/research-computing>`_.
 
 Continued development was sponsored by
-[Micron Advanced Bioimaging Unit](https://micronoxford.com/)
+`Micron Advanced Bioimaging Unit <https://micronoxford.com/>`_
 funded by the Wellcome Trust Strategic Award 107457.
```

### Comparing `omero-tagsearch-4.0.1/omero_tagsearch.egg-info/SOURCES.txt` & `omero-tagsearch-4.1.1/omero_tagsearch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,13 +37,15 @@
 omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/style.css
 omero_tagsearch/static/tagsearch/css/bootstrap.css
 omero_tagsearch/static/tagsearch/css/webtagging_search.css
 omero_tagsearch/static/tagsearch/image/folder16.png
 omero_tagsearch/static/tagsearch/image/folder_image16.png
 omero_tagsearch/static/tagsearch/image/folder_plate16.png
 omero_tagsearch/static/tagsearch/image/folder_screen16.png
+omero_tagsearch/static/tagsearch/image/icon_user.png
 omero_tagsearch/static/tagsearch/image/image16.png
 omero_tagsearch/static/tagsearch/image/run16.png
+omero_tagsearch/static/tagsearch/image/well16.png
 omero_tagsearch/templates/omero_tagsearch/index.html
 omero_tagsearch/templates/omero_tagsearch/search_details.html
 omero_tagsearch/templates/omero_tagsearch/tagnav.html
 omero_tagsearch/templates/omero_tagsearch/tagnav_init.js.html
```

### Comparing `omero-tagsearch-4.0.1/setup.py` & `omero-tagsearch-4.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,37 +30,38 @@
 setup(
     name="omero-tagsearch",
     packages=find_packages(exclude=["ez_setup"]),
     version=VERSION,
     description=DESCRIPTION,
     long_description=read_file("README.rst"),
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Web Environment",
-        "Framework :: Django",
-        "Intended Audience :: End Users/Desktop",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: GNU Affero General Public License v3",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: JavaScript",
-        "Programming Language :: Python :: 3",
-        "Topic :: Internet :: WWW/HTTP",
-        "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
-        "Topic :: Internet :: WWW/HTTP :: WSGI",
-        "Topic :: Scientific/Engineering :: Visualization",
-        "Topic :: Software Development :: Libraries :: " "Application Frameworks",
-        "Topic :: Text Processing :: Markup :: HTML",
+        'Development Status :: 5 - Production/Stable',
+        'Environment :: Web Environment',
+        'Framework :: Django',
+        'Intended Audience :: End Users/Desktop',
+        'Intended Audience :: Science/Research',
+        'License :: OSI Approved :: GNU Affero General Public License v3',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: JavaScript',
+        'Programming Language :: Python :: 3',
+        'Topic :: Internet :: WWW/HTTP',
+        'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
+        'Topic :: Internet :: WWW/HTTP :: WSGI',
+        'Topic :: Scientific/Engineering :: Visualization',
+        'Topic :: Software Development :: Libraries :: ' +
+        'Application Frameworks',
+        'Topic :: Text Processing :: Markup :: HTML'
     ],
     author=AUTHOR,
     author_email="dpwrussell@gmail.com",
     maintainer=MAINTAINER,
     maintainer_email="tom.boissonnet@hhu.de",
     license=LICENSE,
     url=HOMEPAGE,
     download_url="%s/archive/v%s.tar.gz" % (HOMEPAGE, VERSION),
     keywords=["OMERO.web", "webtagging", "tagsearch"],
     install_requires=REQUIREMENTS,
-    python_requires="~=3.5",
+    python_requires=">=3",
     include_package_data=True,
     zip_safe=False,
 )
```

