# Comparing `tmp/ipyaggrid-0.5.2.tar.gz` & `tmp/ipyaggrid-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyaggrid-0.5.2.tar", last modified: Fri Feb  9 15:38:55 2024, max compression
+gzip compressed data, was "ipyaggrid-0.5.3.tar", last modified: Fri Apr 26 12:59:25 2024, max compression
```

## Comparing `ipyaggrid-0.5.2.tar` & `ipyaggrid-0.5.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:38:55.720911 ipyaggrid-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-09 15:38:55.720911 ipyaggrid-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/install.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:38:55.680911 ipyaggrid-0.5.2/ipyaggrid/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/builder_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/community.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:38:55.684911 ipyaggrid-0.5.2/ipyaggrid/flexbox/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/flexbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/flexbox/flexbox_css.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/flexbox/flexbox_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/ipyaggrid.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:38:55.684911 ipyaggrid-0.5.2/ipyaggrid/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/js/helpersBuiltin.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:38:55.684911 ipyaggrid-0.5.2/ipyaggrid/labextension/
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:38:55.696911 ipyaggrid-0.5.2/ipyaggrid/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (127)   175470 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/155.ccf00f68124641941798.js
--rw-r--r--   0 runner    (1001) docker     (127)    70486 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4235646 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/590.9cfdf03ea39f42c7dd54.js
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/590.9cfdf03ea39f42c7dd54.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44173 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/591.89fd4c700b5e9bf9a04d.js
--rw-r--r--   0 runner    (1001) docker     (127)   286990 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/628.a876a22b5bf4766eb88f.js
--rw-r--r--   0 runner    (1001) docker     (127)  1057676 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/680.9780c99311f6aacd0551.js
--rw-r--r--   0 runner    (1001) docker     (127)  1089011 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/731.0e661d2646511263a3f4.js
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/731.0e661d2646511263a3f4.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1281803 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/remoteEntry.7ee9081c423d7172ffb0.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-09 15:38:02.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (127)   153234 2024-02-09 15:38:23.000000 ipyaggrid-0.5.2/ipyaggrid/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:38:55.696911 ipyaggrid-0.5.2/ipyaggrid/magics/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/magics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/magics/custom_magics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:38:55.708911 ipyaggrid-0.5.2/ipyaggrid/nbextension/
--rw-r--r--   0 runner    (1001) docker     (127)  1287139 2024-02-09 15:38:00.000000 ipyaggrid-0.5.2/ipyaggrid/nbextension/906.index.js
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-09 15:38:00.000000 ipyaggrid-0.5.2/ipyaggrid/nbextension/906.index.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4236943 2024-02-09 15:38:00.000000 ipyaggrid-0.5.2/ipyaggrid/nbextension/906.index.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-09 15:37:31.000000 ipyaggrid-0.5.2/ipyaggrid/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (127)  4234161 2024-02-09 15:38:00.000000 ipyaggrid-0.5.2/ipyaggrid/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-09 15:38:00.000000 ipyaggrid-0.5.2/ipyaggrid/nbextension/index.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  8922638 2024-02-09 15:38:00.000000 ipyaggrid-0.5.2/ipyaggrid/nbextension/index.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    21470 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/ipyaggrid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:38:55.680911 ipyaggrid-0.5.2/ipyaggrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-09 15:38:55.000000 ipyaggrid-0.5.2/ipyaggrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-09 15:38:55.000000 ipyaggrid-0.5.2/ipyaggrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 15:38:55.000000 ipyaggrid-0.5.2/ipyaggrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 15:38:55.000000 ipyaggrid-0.5.2/ipyaggrid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-09 15:38:55.000000 ipyaggrid-0.5.2/ipyaggrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-09 15:38:55.000000 ipyaggrid-0.5.2/ipyaggrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-09 15:38:55.720911 ipyaggrid-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-09 15:37:01.000000 ipyaggrid-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:59:25.766302 ipyaggrid-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-26 12:59:25.766302 ipyaggrid-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/install.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:59:25.730301 ipyaggrid-0.5.3/ipyaggrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/builder_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/community.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:59:25.730301 ipyaggrid-0.5.3/ipyaggrid/flexbox/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/flexbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/flexbox/flexbox_css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/flexbox/flexbox_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/ipyaggrid.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:59:25.730301 ipyaggrid-0.5.3/ipyaggrid/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/js/helpersBuiltin.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:59:25.730301 ipyaggrid-0.5.3/ipyaggrid/labextension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:59:25.742302 ipyaggrid-0.5.3/ipyaggrid/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   175499 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/155.07e25d30287801138a06.js
+-rw-r--r--   0 runner    (1001) docker     (127)    70486 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4235646 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/590.cf2e9e3d8c2dac69f6c1.js
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/590.cf2e9e3d8c2dac69f6c1.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    44173 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/591.89fd4c700b5e9bf9a04d.js
+-rw-r--r--   0 runner    (1001) docker     (127)   286990 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/628.a876a22b5bf4766eb88f.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1057676 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/680.9780c99311f6aacd0551.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1089011 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/731.0e661d2646511263a3f4.js
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/731.0e661d2646511263a3f4.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1281803 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/remoteEntry.661c44866aeaa5c5cfbc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-26 12:58:32.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (127)   153234 2024-04-26 12:58:53.000000 ipyaggrid-0.5.3/ipyaggrid/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:59:25.742302 ipyaggrid-0.5.3/ipyaggrid/magics/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/magics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/magics/custom_magics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:59:25.758302 ipyaggrid-0.5.3/ipyaggrid/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (127)  1287139 2024-04-26 12:58:29.000000 ipyaggrid-0.5.3/ipyaggrid/nbextension/906.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-26 12:58:29.000000 ipyaggrid-0.5.3/ipyaggrid/nbextension/906.index.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4236943 2024-04-26 12:58:29.000000 ipyaggrid-0.5.3/ipyaggrid/nbextension/906.index.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-26 12:58:00.000000 ipyaggrid-0.5.3/ipyaggrid/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4234161 2024-04-26 12:58:29.000000 ipyaggrid-0.5.3/ipyaggrid/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-26 12:58:29.000000 ipyaggrid-0.5.3/ipyaggrid/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  8922638 2024-04-26 12:58:29.000000 ipyaggrid-0.5.3/ipyaggrid/nbextension/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    21470 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/ipyaggrid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:59:25.730301 ipyaggrid-0.5.3/ipyaggrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-26 12:59:25.000000 ipyaggrid-0.5.3/ipyaggrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-26 12:59:25.000000 ipyaggrid-0.5.3/ipyaggrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:59:25.000000 ipyaggrid-0.5.3/ipyaggrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:59:25.000000 ipyaggrid-0.5.3/ipyaggrid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-26 12:59:25.000000 ipyaggrid-0.5.3/ipyaggrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 12:59:25.000000 ipyaggrid-0.5.3/ipyaggrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-26 12:59:25.766302 ipyaggrid-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-26 12:57:23.000000 ipyaggrid-0.5.3/setup.py
```

### Comparing `ipyaggrid-0.5.2/LICENSE` & `ipyaggrid-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/PKG-INFO` & `ipyaggrid-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ipyaggrid
-Version: 0.5.2
+Version: 0.5.3
 Summary: Jupyter widget - ag-grid in the notebook
 Home-page: https://github.com/widgetti/ipyaggrid
 Author: Mario Buikhuizen, Maarten Breddels, DGothrek
 Author-email: mariobuikhuizen@gmail.com, maartenbreddels@gmail.com
 License: MIT
-Download-URL: https://github.com/widgetti/ipyaggrid/archive/refs/tags/v0.5.2.zip
+Download-URL: https://github.com/widgetti/ipyaggrid/archive/refs/tags/v0.5.3.zip
 Description: # ipyaggrid
         
         [![Latest Version](https://img.shields.io/pypi/v/ipyaggrid.svg)](https://pypi.python.org/pypi/ipyaggrid/)
         [![Downloads](https://img.shields.io/pypi/dm/ipyaggrid.svg)](https://pypi.python.org/pypi/ipyaggrid/)
         [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gl/DGothrek%2Fipyaggrid/binder-demo)
         
         ### Doc
```

### Comparing `ipyaggrid-0.5.2/README.md` & `ipyaggrid-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/__init__.py` & `ipyaggrid-0.5.3/ipyaggrid/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/__meta__.py` & `ipyaggrid-0.5.3/ipyaggrid/__meta__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     return version
 
 
 # meta data
 
 __name__ = 'ipyaggrid'
 name_url = __name__.replace('_', '-')
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 __version_js__ = __version__
 
 
 __description__ = 'Jupyter widget - ag-grid in the notebook'
 __long_description__ = 'See repo README'
 __author__ = 'Mario Buikhuizen, Maarten Breddels, DGothrek'
 __author_email__ = 'mariobuikhuizen@gmail.com, maartenbreddels@gmail.com'
```

### Comparing `ipyaggrid-0.5.2/ipyaggrid/builder_params.py` & `ipyaggrid-0.5.3/ipyaggrid/builder_params.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/community.py` & `ipyaggrid-0.5.3/ipyaggrid/community.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/display.py` & `ipyaggrid-0.5.3/ipyaggrid/display.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/flexbox/flexbox_css.py` & `ipyaggrid-0.5.3/ipyaggrid/flexbox/flexbox_css.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/flexbox/flexbox_standard.py` & `ipyaggrid-0.5.3/ipyaggrid/flexbox/flexbox_standard.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/grid.py` & `ipyaggrid-0.5.3/ipyaggrid/grid.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/js/helpersBuiltin.js` & `ipyaggrid-0.5.3/ipyaggrid/js/helpersBuiltin.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/package.json` & `ipyaggrid-0.5.3/ipyaggrid/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9603365384615384%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.661c44866aeaa5c5cfbc.js'}}",*

 * * "'version'": "'0.5.3'"}*

```diff
@@ -35,15 +35,15 @@
         "dist/*.js",
         "src/styles/**/*.css",
         "src/styles/icons/*.svg"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.7ee9081c423d7172ffb0.js"
+            "load": "static/remoteEntry.661c44866aeaa5c5cfbc.js"
         },
         "extension": "src/labplugin",
         "outputDir": "../ipyaggrid/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -72,9 +72,9 @@
         "dev": "webpack --mode=development && npm run build:labextension:dev",
         "format": "prettier --write '**/*.{js,jsx}'",
         "lint": "eslint '**/*.{js,jsx}' --quiet",
         "prepare": "webpack --mode production",
         "test": "echo \"Error: no test specified\"",
         "watch": "watch 'webpack --mode development' src/"
     },
-    "version": "0.5.2"
+    "version": "0.5.3"
 }
```

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/static/155.ccf00f68124641941798.js` & `ipyaggrid-0.5.3/ipyaggrid/labextension/static/155.07e25d30287801138a06.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -190,15 +190,15 @@
             t.r(a), t.d(a, {
                 AgGridModel: () => I,
                 AgGridView: () => _
             });
             var i = t(2390),
                 c = (t(8174), t(1987), t(9832), t(5783), t(988), t(6743), t(9771), t(7211), t(1014), t(194)),
                 o = t(5106);
-            const l = "0.5.2";
+            const l = "0.5.3";
             var g = t(3379),
                 r = t.n(g),
                 d = t(7795),
                 p = t.n(d),
                 s = t(569),
                 h = t.n(s),
                 x = t(3565),
@@ -312,16 +312,16 @@
                         this.model.get("_is_grid_options_multi") ? c.D(this, o, this.model.get("_grid_options_multi_down"), n, i) : c.q(this, o, this.model.get("_grid_options_mono_down"), n, i), console.log("end ipyaggrid render")
                     })()
                 }
             }
             const E = document.querySelector("body").getAttribute("data-base-url");
             t.p = `${E}nbextensions/ipyaggrid/`;
             const U = [i.IJupyterWidgetRegistry],
-                R = JSON.parse(document.getElementById("jupyter-config-data").textContent).baseUrl;
-            t.p = `${R}lab/extensions/ipyaggrid/static/`;
+                R = JSON.parse(document.getElementById("jupyter-config-data").textContent);
+            t.p = (R.fullLabextensionsUrl || `${R.baseUrl}lab/extensions`) + "/ipyaggrid/static/";
             const S = {
                 id: "ipyaggrid:plugin",
                 requires: U,
                 activate: (e, n) => {
                     console.log("JupyterLab extension ipyaggrid is activated!"), n.registerWidget({
                         name: "ipyaggrid",
                         version: l,
```

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js` & `ipyaggrid-0.5.3/ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/static/590.9cfdf03ea39f42c7dd54.js` & `ipyaggrid-0.5.3/ipyaggrid/labextension/static/590.cf2e9e3d8c2dac69f6c1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 590.9cfdf03ea39f42c7dd54.js.LICENSE.txt */
+/*! For license information please see 590.cf2e9e3d8c2dac69f6c1.js.LICENSE.txt */
 (self.webpackChunkipyaggrid = self.webpackChunkipyaggrid || []).push([
     [590], {
         5590: (module, exports, __webpack_require__) => {
             var __WEBPACK_AMD_DEFINE_ARRAY__, __WEBPACK_AMD_DEFINE_RESULT__;
             __WEBPACK_AMD_DEFINE_ARRAY__ = [__webpack_require__(2390)], __WEBPACK_AMD_DEFINE_RESULT__ = (__WEBPACK_EXTERNAL_MODULE__9146__ => (() => {
                 var __webpack_modules__ = {
                         1731: (e, n, t) => {
@@ -50222,15 +50222,15 @@
                     }
                 }, __nested_webpack_require_4225595__.r = e => {
                     "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
                         value: "Module"
                     }), Object.defineProperty(e, "__esModule", {
                         value: !0
                     })
-                }, __nested_webpack_require_4225595__.nmd = e => (e.paths = [], e.children || (e.children = []), e), __nested_webpack_require_4225595__.p = "https://unpkg.com/ipyaggrid@0.5.2/dist/", (() => {
+                }, __nested_webpack_require_4225595__.nmd = e => (e.paths = [], e.children || (e.children = []), e), __nested_webpack_require_4225595__.p = "https://unpkg.com/ipyaggrid@0.5.3/dist/", (() => {
                     __nested_webpack_require_4225595__.b = document.baseURI || self.location.href;
                     var e = {
                         179: 0
                     };
                     __nested_webpack_require_4225595__.f.j = (n, t) => {
                         var a = __nested_webpack_require_4225595__.o(e, n) ? e[n] : void 0;
                         if (0 !== a)
@@ -50305,15 +50305,15 @@
                     y.styleTagTransform = c(), y.setAttributes = l(), y.insert = g().bind(null, "head"), y.domAPI = r(), y.insertStyleElement = p(), t()(k.Z, y), k.Z && k.Z.locals && k.Z.locals;
                     var I = __nested_webpack_require_4225595__(2557),
                         D = {};
                     D.styleTagTransform = c(), D.setAttributes = l(), D.insert = g().bind(null, "head"), D.domAPI = r(), D.insertStyleElement = p(), t()(I.Z, D), I.Z && I.Z.locals && I.Z.locals;
                     var S = __nested_webpack_require_4225595__(194),
                         _ = __nested_webpack_require_4225595__(5106);
                     const R = {
-                        i8: "0.5.2"
+                        i8: "0.5.3"
                     };
                     var O = __nested_webpack_require_4225595__(890),
                         T = {};
                     T.styleTagTransform = c(), T.setAttributes = l(), T.insert = g().bind(null, "head"), T.domAPI = r(), T.insertStyleElement = p(), t()(O.Z, T), O.Z && O.Z.locals && O.Z.locals;
                     var M = __nested_webpack_require_4225595__(4643),
                         P = {};
                     P.styleTagTransform = c(), P.setAttributes = l(), P.insert = g().bind(null, "head"), P.domAPI = r(), P.insertStyleElement = p(), t()(M.Z, P), M.Z && M.Z.locals && M.Z.locals;
```

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/static/591.89fd4c700b5e9bf9a04d.js` & `ipyaggrid-0.5.3/ipyaggrid/labextension/static/591.89fd4c700b5e9bf9a04d.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/static/628.a876a22b5bf4766eb88f.js` & `ipyaggrid-0.5.3/ipyaggrid/labextension/static/628.a876a22b5bf4766eb88f.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/static/680.9780c99311f6aacd0551.js` & `ipyaggrid-0.5.3/ipyaggrid/labextension/static/680.9780c99311f6aacd0551.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/static/731.0e661d2646511263a3f4.js` & `ipyaggrid-0.5.3/ipyaggrid/labextension/static/731.0e661d2646511263a3f4.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js` & `ipyaggrid-0.5.3/ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/static/remoteEntry.7ee9081c423d7172ffb0.js` & `ipyaggrid-0.5.3/ipyaggrid/labextension/static/remoteEntry.661c44866aeaa5c5cfbc.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, f, d, c, u, l, s, p, h, b, g, v, m, y, w, P, S = {
+    var e, r, t, n, o, a, i, d, f, c, u, l, s, p, h, b, g, v, m, y, w, P, S = {
             7329: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(390), t.e(590)]).then((() => () => t(5590))),
                         "./extension": () => Promise.all([t.e(680), t.e(390), t.e(155)]).then((() => () => t(782)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
         j = {};
 
     function E(e) {
         var r = j[e];
@@ -43,216 +43,216 @@
         }), r
     }, r = Object.getPrototypeOf ? e => Object.getPrototypeOf(e) : e => e.__proto__, E.t = function(t, n) {
         if (1 & n && (t = this(t)), 8 & n) return t;
         if ("object" == typeof t && t) {
             if (4 & n && t.__esModule) return t;
             if (16 & n && "function" == typeof t.then) return t
         }
-        var a = Object.create(null);
-        E.r(a);
-        var o = {};
+        var o = Object.create(null);
+        E.r(o);
+        var a = {};
         e = e || [null, r({}), r([]), r(r)];
         for (var i = 2 & n && t;
-            "object" == typeof i && !~e.indexOf(i); i = r(i)) Object.getOwnPropertyNames(i).forEach((e => o[e] = () => t[e]));
-        return o.default = () => t, E.d(a, o), a
+            "object" == typeof i && !~e.indexOf(i); i = r(i)) Object.getOwnPropertyNames(i).forEach((e => a[e] = () => t[e]));
+        return a.default = () => t, E.d(o, a), o
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
         86: "cf8771b6c6c768b9105b",
-        155: "ccf00f68124641941798",
+        155: "07e25d30287801138a06",
         324: "ddc31b9c6bf66967f205",
         390: "cadb0c6efe054e519894",
         486: "9a102cac74aa3af2b7b8",
-        590: "9cfdf03ea39f42c7dd54",
+        590: "cf2e9e3d8c2dac69f6c1",
         591: "89fd4c700b5e9bf9a04d",
         628: "a876a22b5bf4766eb88f",
         680: "9780c99311f6aacd0551",
         731: "0e661d2646511263a3f4",
         906: "95bbf22d029b842482b2"
     } [e] + ".js?v=" + {
         86: "cf8771b6c6c768b9105b",
-        155: "ccf00f68124641941798",
+        155: "07e25d30287801138a06",
         324: "ddc31b9c6bf66967f205",
         390: "cadb0c6efe054e519894",
         486: "9a102cac74aa3af2b7b8",
-        590: "9cfdf03ea39f42c7dd54",
+        590: "cf2e9e3d8c2dac69f6c1",
         591: "89fd4c700b5e9bf9a04d",
         628: "a876a22b5bf4766eb88f",
         680: "9780c99311f6aacd0551",
         731: "0e661d2646511263a3f4",
         906: "95bbf22d029b842482b2"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, n = "ipyaggrid:", E.l = (e, r, a, o) => {
+    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, n = "ipyaggrid:", E.l = (e, r, o, a) => {
         if (t[e]) t[e].push(r);
         else {
-            var i, f;
-            if (void 0 !== a)
-                for (var d = document.getElementsByTagName("script"), c = 0; c < d.length; c++) {
-                    var u = d[c];
-                    if (u.getAttribute("src") == e || u.getAttribute("data-webpack") == n + a) {
+            var i, d;
+            if (void 0 !== o)
+                for (var f = document.getElementsByTagName("script"), c = 0; c < f.length; c++) {
+                    var u = f[c];
+                    if (u.getAttribute("src") == e || u.getAttribute("data-webpack") == n + o) {
                         i = u;
                         break
                     }
                 }
-            i || (f = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", n + a), i.src = e), t[e] = [r];
+            i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", n + o), i.src = e), t[e] = [r];
             var l = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(s);
-                    var a = t[e];
-                    if (delete t[e], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+                    var o = t[e];
+                    if (delete t[e], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 s = setTimeout(l.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = l.bind(null, i.onerror), i.onload = l.bind(null, i.onload), f && document.head.appendChild(i)
+            i.onerror = l.bind(null, i.onerror), i.onload = l.bind(null, i.onload), d && document.head.appendChild(i)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, E.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         E.S = {};
         var e = {},
             r = {};
         E.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 E.o(E.S, t) || (E.S[t] = {});
-                var o = E.S[t],
+                var a = E.S[t],
                     i = "ipyaggrid",
-                    f = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            f = a[r];
-                        (!f || !f.loaded && (!n != !f.eager ? n : i > f.from)) && (a[r] = {
+                    d = (e, r, t, n) => {
+                        var o = a[e] = a[e] || {},
+                            d = o[r];
+                        (!d || !d.loaded && (!n != !d.eager ? n : i > d.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
-                    d = [];
-                return "default" === t && (f("ag-grid-community", "28.1.1", (() => E.e(731).then((() => () => E(1731))))), f("ag-grid-enterprise", "28.1.1", (() => Promise.all([E.e(906), E.e(324)]).then((() => () => E(1906))))), f("d3", "7.8.5", (() => E.e(628).then((() => () => E(1628))))), f("ipyaggrid", "0.5.2", (() => Promise.all([E.e(390), E.e(590)]).then((() => () => E(5590))))), f("lodash", "4.17.21", (() => E.e(486).then((() => () => E(6486))))), f("pako", "1.0.11", (() => E.e(591).then((() => () => E(9591)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (d("ag-grid-community", "28.1.1", (() => E.e(731).then((() => () => E(1731))))), d("ag-grid-enterprise", "28.1.1", (() => Promise.all([E.e(906), E.e(324)]).then((() => () => E(1906))))), d("d3", "7.8.5", (() => E.e(628).then((() => () => E(1628))))), d("ipyaggrid", "0.5.3", (() => Promise.all([E.e(390), E.e(590)]).then((() => () => E(5590))))), d("lodash", "4.17.21", (() => E.e(486).then((() => () => E(6486))))), d("pako", "1.0.11", (() => E.e(591).then((() => () => E(9591)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
                 for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), E.p = e
-    })(), a = e => {
+    })(), o = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
-    }, o = (e, r) => {
-        e = a(e), r = a(r);
+    }, a = (e, r) => {
+        e = o(e), r = o(r);
         for (var t = 0;;) {
             if (t >= e.length) return t < r.length && "u" != (typeof r[t])[0];
             var n = e[t],
-                o = (typeof n)[0];
-            if (t >= r.length) return "u" == o;
+                a = (typeof n)[0];
+            if (t >= r.length) return "u" == a;
             var i = r[t],
-                f = (typeof i)[0];
-            if (o != f) return "o" == o && "n" == f || "s" == f || "u" == o;
-            if ("o" != o && "u" != o && n != i) return n < i;
+                d = (typeof i)[0];
+            if (a != d) return "o" == a && "n" == d || "s" == d || "u" == a;
+            if ("o" != a && "u" != a && n != i) return n < i;
             t++
         }
     }, i = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(f = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, f);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
             return t
         }
-        var o = [];
-        for (a = 1; a < e.length; a++) {
-            var f = e[a];
-            o.push(0 === f ? "not(" + d() + ")" : 1 === f ? "(" + d() + " || " + d() + ")" : 2 === f ? o.pop() + " " + o.pop() : i(f))
+        var a = [];
+        for (o = 1; o < e.length; o++) {
+            var d = e[o];
+            a.push(0 === d ? "not(" + f() + ")" : 1 === d ? "(" + f() + " || " + f() + ")" : 2 === d ? a.pop() + " " + a.pop() : i(d))
         }
-        return d();
+        return f();
 
-        function d() {
-            return o.pop().replace(/^\((.+)\)$/, "$1")
+        function f() {
+            return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, f = (e, r) => {
+    }, d = (e, r) => {
         if (0 in e) {
-            r = a(r);
+            r = o(r);
             var t = e[0],
                 n = t < 0;
             n && (t = -t - 1);
-            for (var o = 0, i = 1, d = !0;; i++, o++) {
+            for (var a = 0, i = 1, f = !0;; i++, a++) {
                 var c, u, l = i < e.length ? (typeof e[i])[0] : "";
-                if (o >= r.length || "o" == (u = (typeof(c = r[o]))[0])) return !d || ("u" == l ? i > t && !n : "" == l != n);
+                if (a >= r.length || "o" == (u = (typeof(c = r[a]))[0])) return !f || ("u" == l ? i > t && !n : "" == l != n);
                 if ("u" == u) {
-                    if (!d || "u" != l) return !1
-                } else if (d)
+                    if (!f || "u" != l) return !1
+                } else if (f)
                     if (l == u)
                         if (i <= t) {
                             if (c != e[i]) return !1
                         } else {
                             if (n ? c > e[i] : c < e[i]) return !1;
-                            c != e[i] && (d = !1)
+                            c != e[i] && (f = !1)
                         }
                 else if ("s" != l && "n" != l) {
                     if (n || i <= t) return !1;
-                    d = !1, i--
+                    f = !1, i--
                 } else {
                     if (i <= t || u < l != n) return !1;
-                    d = !1
-                } else "s" != l && "n" != l && (d = !1, i--)
+                    f = !1
+                } else "s" != l && "n" != l && (f = !1, i--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
-        for (o = 1; o < e.length; o++) {
-            var h = e[o];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? f(h, r) : !p())
+        for (a = 1; a < e.length; a++) {
+            var h = e[a];
+            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? d(h, r) : !p())
         }
         return !!p()
-    }, d = (e, r) => {
+    }, f = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, c = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", l = (e, r, t, n) => {
-        var a = c(e, t);
-        return f(n, a) || p(u(e, t, a, n)), h(e[t][a])
+        var o = c(e, t);
+        return d(n, o) || p(u(e, t, o, n)), h(e[t][o])
     }, s = (e, r, t) => {
         var n = e[r];
-        return (r = Object.keys(n).reduce(((e, r) => !f(t, r) || e && !o(e, r) ? e : r), 0)) && n[r]
+        return (r = Object.keys(n).reduce(((e, r) => !d(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, h = e => (e.loaded = 1, e.get()), g = (b = e => function(r, t, n, a) {
-        var o = E.I(r);
-        return o && o.then ? o.then(e.bind(e, r, E.S[r], t, n, a)) : e(r, E.S[r], t, n, a)
-    })(((e, r, t, n) => (d(e, t), l(r, 0, t, n)))), v = b(((e, r, t, n, a) => {
-        var o = r && E.o(r, t) && s(r, t, n);
-        return o ? h(o) : a()
+    }, h = e => (e.loaded = 1, e.get()), g = (b = e => function(r, t, n, o) {
+        var a = E.I(r);
+        return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
+    })(((e, r, t, n) => (f(e, t), l(r, 0, t, n)))), v = b(((e, r, t, n, o) => {
+        var a = r && E.o(r, t) && s(r, t, n);
+        return a ? h(a) : o()
     })), m = {}, y = {
         2390: () => g("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3, 0, 0], 1, 1
         ]),
         6289: () => v("default", "d3", [1, 7, 8, 5], (() => E.e(628).then((() => () => E(1628))))),
         6405: () => v("default", "ag-grid-community", [4, 28, 1, 1], (() => E.e(731).then((() => () => E(1731))))),
@@ -277,16 +277,16 @@
                 P[e] = !0;
                 var n = r => {
                     delete m[e], E.m[e] = t => {
                         throw delete E.c[e], r
                     }
                 };
                 try {
-                    var a = y[e]();
-                    a.then ? r.push(m[e] = a.then(t).catch(n)) : t(a)
+                    var o = y[e]();
+                    o.then ? r.push(m[e] = o.then(t).catch(n)) : t(o)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         E.b = document.baseURI || self.location.href;
@@ -295,35 +295,35 @@
         };
         E.f.j = (r, t) => {
             var n = E.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (/^(324|390|86)$/.test(r)) e[r] = 0;
             else {
-                var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                t.push(n[2] = a);
-                var o = E.p + E.u(r),
+                var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                t.push(n[2] = o);
+                var a = E.p + E.u(r),
                     i = new Error;
-                E.l(o, (t => {
+                E.l(a, (t => {
                     if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var a = t && ("load" === t.type ? "missing" : t.type),
-                            o = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                        var o = t && ("load" === t.type ? "missing" : t.type),
+                            a = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var n, a, [o, i, f] = t,
-                    d = 0;
-                if (o.some((r => 0 !== e[r]))) {
+                var n, o, [a, i, d] = t,
+                    f = 0;
+                if (a.some((r => 0 !== e[r]))) {
                     for (n in i) E.o(i, n) && (E.m[n] = i[n]);
-                    f && f(E)
+                    d && d(E)
                 }
-                for (r && r(t); d < o.length; d++) a = o[d], E.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); f < a.length; f++) o = a[f], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkipyaggrid = self.webpackChunkipyaggrid || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var O = E(7329);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyaggrid = O
 })();
```

### Comparing `ipyaggrid-0.5.2/ipyaggrid/labextension/static/third-party-licenses.json` & `ipyaggrid-0.5.3/ipyaggrid/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/magics/custom_magics.py` & `ipyaggrid-0.5.3/ipyaggrid/magics/custom_magics.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/nbextension/906.index.js` & `ipyaggrid-0.5.3/ipyaggrid/nbextension/906.index.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/nbextension/906.index.js.map` & `ipyaggrid-0.5.3/ipyaggrid/nbextension/906.index.js.map`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/nbextension/extension.js` & `ipyaggrid-0.5.3/ipyaggrid/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/nbextension/index.js` & `ipyaggrid-0.5.3/ipyaggrid/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -50312,15 +50312,15 @@
         y.styleTagTransform = c(), y.setAttributes = l(), y.insert = g().bind(null, "head"), y.domAPI = r(), y.insertStyleElement = p(), t()(k.Z, y), k.Z && k.Z.locals && k.Z.locals;
         var I = __webpack_require__(2557),
             D = {};
         D.styleTagTransform = c(), D.setAttributes = l(), D.insert = g().bind(null, "head"), D.domAPI = r(), D.insertStyleElement = p(), t()(I.Z, D), I.Z && I.Z.locals && I.Z.locals;
         var S = __webpack_require__(194),
             R = __webpack_require__(5106);
         const _ = {
-            i8: "0.5.2"
+            i8: "0.5.3"
         };
         var O = __webpack_require__(890),
             T = {};
         T.styleTagTransform = c(), T.setAttributes = l(), T.insert = g().bind(null, "head"), T.domAPI = r(), T.insertStyleElement = p(), t()(O.Z, T), O.Z && O.Z.locals && O.Z.locals;
         var M = __webpack_require__(4643),
             P = {};
         P.styleTagTransform = c(), P.setAttributes = l(), P.insert = g().bind(null, "head"), P.domAPI = r(), P.insertStyleElement = p(), t()(M.Z, P), M.Z && M.Z.locals && M.Z.locals;
```

### Comparing `ipyaggrid-0.5.2/ipyaggrid/nbextension/index.js.LICENSE.txt` & `ipyaggrid-0.5.3/ipyaggrid/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/nbextension/index.js.map` & `ipyaggrid-0.5.3/ipyaggrid/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid/util.py` & `ipyaggrid-0.5.3/ipyaggrid/util.py`

 * *Files identical despite different names*

### Comparing `ipyaggrid-0.5.2/ipyaggrid.egg-info/PKG-INFO` & `ipyaggrid-0.5.3/ipyaggrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ipyaggrid
-Version: 0.5.2
+Version: 0.5.3
 Summary: Jupyter widget - ag-grid in the notebook
 Home-page: https://github.com/widgetti/ipyaggrid
 Author: Mario Buikhuizen, Maarten Breddels, DGothrek
 Author-email: mariobuikhuizen@gmail.com, maartenbreddels@gmail.com
 License: MIT
-Download-URL: https://github.com/widgetti/ipyaggrid/archive/refs/tags/v0.5.2.zip
+Download-URL: https://github.com/widgetti/ipyaggrid/archive/refs/tags/v0.5.3.zip
 Description: # ipyaggrid
         
         [![Latest Version](https://img.shields.io/pypi/v/ipyaggrid.svg)](https://pypi.python.org/pypi/ipyaggrid/)
         [![Downloads](https://img.shields.io/pypi/dm/ipyaggrid.svg)](https://pypi.python.org/pypi/ipyaggrid/)
         [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gl/DGothrek%2Fipyaggrid/binder-demo)
         
         ### Doc
```

### Comparing `ipyaggrid-0.5.2/ipyaggrid.egg-info/SOURCES.txt` & `ipyaggrid-0.5.3/ipyaggrid.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 ipyaggrid.egg-info/requires.txt
 ipyaggrid.egg-info/top_level.txt
 ipyaggrid/flexbox/__init__.py
 ipyaggrid/flexbox/flexbox_css.py
 ipyaggrid/flexbox/flexbox_standard.py
 ipyaggrid/js/helpersBuiltin.js
 ipyaggrid/labextension/package.json
-ipyaggrid/labextension/static/155.ccf00f68124641941798.js
+ipyaggrid/labextension/static/155.07e25d30287801138a06.js
 ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js
 ipyaggrid/labextension/static/486.9a102cac74aa3af2b7b8.js.LICENSE.txt
-ipyaggrid/labextension/static/590.9cfdf03ea39f42c7dd54.js
-ipyaggrid/labextension/static/590.9cfdf03ea39f42c7dd54.js.LICENSE.txt
+ipyaggrid/labextension/static/590.cf2e9e3d8c2dac69f6c1.js
+ipyaggrid/labextension/static/590.cf2e9e3d8c2dac69f6c1.js.LICENSE.txt
 ipyaggrid/labextension/static/591.89fd4c700b5e9bf9a04d.js
 ipyaggrid/labextension/static/628.a876a22b5bf4766eb88f.js
 ipyaggrid/labextension/static/680.9780c99311f6aacd0551.js
 ipyaggrid/labextension/static/731.0e661d2646511263a3f4.js
 ipyaggrid/labextension/static/731.0e661d2646511263a3f4.js.LICENSE.txt
 ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js
 ipyaggrid/labextension/static/906.95bbf22d029b842482b2.js.LICENSE.txt
-ipyaggrid/labextension/static/remoteEntry.7ee9081c423d7172ffb0.js
+ipyaggrid/labextension/static/remoteEntry.661c44866aeaa5c5cfbc.js
 ipyaggrid/labextension/static/style.js
 ipyaggrid/labextension/static/third-party-licenses.json
 ipyaggrid/magics/__init__.py
 ipyaggrid/magics/custom_magics.py
 ipyaggrid/nbextension/906.index.js
 ipyaggrid/nbextension/906.index.js.LICENSE.txt
 ipyaggrid/nbextension/906.index.js.map
```

### Comparing `ipyaggrid-0.5.2/setup.py` & `ipyaggrid-0.5.3/setup.py`

 * *Files identical despite different names*

