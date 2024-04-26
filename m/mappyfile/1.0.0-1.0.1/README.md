# Comparing `tmp/mappyfile-1.0.0.tar.gz` & `tmp/mappyfile-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mappyfile-1.0.0.tar", last modified: Thu Sep 28 09:33:42 2023, max compression
+gzip compressed data, was "mappyfile-1.0.1.tar", last modified: Fri Apr 26 08:39:05 2024, max compression
```

## Comparing `mappyfile-1.0.0.tar` & `mappyfile-1.0.1.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-09-28 09:33:42.721295 mappyfile-1.0.0/
--rw-rw-rw-   0        0        0     1089 2017-07-06 19:50:13.000000 mappyfile-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       78 2017-10-02 08:44:46.000000 mappyfile-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5431 2023-09-28 09:33:42.722296 mappyfile-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4546 2023-09-28 08:55:09.000000 mappyfile-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-09-28 09:33:41.088295 mappyfile-1.0.0/docs/
--rw-rw-rw-   0        0        0        9 2023-08-11 15:22:45.000000 mappyfile-1.0.0/docs/.gitignore
--rw-rw-rw-   0        0        0    16914 2023-09-28 08:36:15.000000 mappyfile-1.0.0/docs/HISTORY.rst
--rw-rw-rw-   0        0        0     7843 2017-07-06 19:50:13.000000 mappyfile-1.0.0/docs/Makefile
--rw-rw-rw-   0        0        0     3354 2020-07-14 05:32:08.000000 mappyfile-1.0.0/docs/client.rst
--rw-rw-rw-   0        0        0     3710 2023-08-13 18:55:15.000000 mappyfile-1.0.0/docs/comments.rst
--rw-rw-rw-   0        0        0    19393 2023-08-11 15:48:40.000000 mappyfile-1.0.0/docs/conf.py
--rw-rw-rw-   0        0        0     2882 2023-09-28 07:25:03.000000 mappyfile-1.0.0/docs/development.rst
--rw-rw-rw-   0        0        0     3237 2023-08-13 18:25:58.000000 mappyfile-1.0.0/docs/editing.rst
--rw-rw-rw-   0        0        0     1655 2018-08-22 22:23:30.000000 mappyfile-1.0.0/docs/format.txt
--rw-rw-rw-   0        0        0     7176 2023-04-20 10:21:52.000000 mappyfile-1.0.0/docs/grammar.rst
--rw-rw-rw-   0        0        0    10113 2023-09-28 07:56:02.000000 mappyfile-1.0.0/docs/index.rst
--rwxrwxrwx   0        0        0     7738 2017-07-06 19:50:13.000000 mappyfile-1.0.0/docs/make.bat
--rw-rw-rw-   0        0        0     6378 2023-08-11 15:31:23.000000 mappyfile-1.0.0/docs/parser.rst
--rw-rw-rw-   0        0        0    12725 2017-07-06 19:50:13.000000 mappyfile-1.0.0/docs/performance.txt
--rw-rw-rw-   0        0        0     5423 2023-08-13 18:28:48.000000 mappyfile-1.0.0/docs/pretty_printing.rst
--rw-rw-rw-   0        0        0     1144 2023-08-11 14:50:51.000000 mappyfile-1.0.0/docs/python_integration.rst
--rw-rw-rw-   0        0        0       13 2023-09-28 07:15:29.000000 mappyfile-1.0.0/docs/requirements.txt
--rw-rw-rw-   0        0        0    10515 2023-08-13 18:15:54.000000 mappyfile-1.0.0/docs/rfc.rst
--rw-rw-rw-   0        0        0     1692 2017-07-06 19:50:13.000000 mappyfile-1.0.0/docs/sample_dict.json
--rw-rw-rw-   0        0        0      879 2017-07-06 19:50:13.000000 mappyfile-1.0.0/docs/sample_map.txt
--rw-rw-rw-   0        0        0     2723 2023-08-11 17:41:30.000000 mappyfile-1.0.0/docs/schemas.rst
--rw-rw-rw-   0        0        0     3497 2023-08-13 18:03:47.000000 mappyfile-1.0.0/docs/testing.rst
--rw-rw-rw-   0        0        0     2268 2023-08-13 18:22:08.000000 mappyfile-1.0.0/docs/transformer.rst
--rw-rw-rw-   0        0        0      923 2018-08-22 22:23:30.000000 mappyfile-1.0.0/docs/validate.txt
--rw-rw-rw-   0        0        0     5919 2023-08-13 08:30:20.000000 mappyfile-1.0.0/docs/validation.rst
--rw-rw-rw-   0        0        0      305 2018-08-22 22:23:30.000000 mappyfile-1.0.0/docs/validation_errors.txt
-drwxrwxrwx   0        0        0        0 2023-09-28 09:33:41.422294 mappyfile-1.0.0/mappyfile/
--rw-rw-rw-   0        0        0     2534 2023-09-28 08:48:29.000000 mappyfile-1.0.0/mappyfile/__init__.py
--rw-rw-rw-   0        0        0     8598 2023-08-13 12:38:53.000000 mappyfile-1.0.0/mappyfile/cli.py
--rw-rw-rw-   0        0        0     8694 2023-08-13 18:01:01.000000 mappyfile-1.0.0/mappyfile/dictutils.py
--rw-rw-rw-   0        0        0     5600 2023-04-25 07:37:14.000000 mappyfile-1.0.0/mappyfile/mapfile.lark
--rw-rw-rw-   0        0        0     5223 2023-08-13 18:01:01.000000 mappyfile-1.0.0/mappyfile/ordereddict.py
--rw-rw-rw-   0        0        0     8626 2023-09-02 14:55:20.000000 mappyfile-1.0.0/mappyfile/parser.py
--rw-rw-rw-   0        0        0    20742 2023-08-13 18:01:01.000000 mappyfile-1.0.0/mappyfile/pprint.py
--rw-rw-rw-   0        0        0        0 2023-08-14 14:48:56.000000 mappyfile-1.0.0/mappyfile/py.typed
--rw-rw-rw-   0        0        0     4021 2023-08-13 12:18:42.000000 mappyfile-1.0.0/mappyfile/quoter.py
-drwxrwxrwx   0        0        0        0 2023-09-28 09:33:42.390296 mappyfile-1.0.0/mappyfile/schemas/
--rw-rw-rw-   0        0        0     3134 2022-02-21 21:03:48.000000 mappyfile-1.0.0/mappyfile/schemas/class.json
--rw-rw-rw-   0        0        0      815 2022-02-21 21:03:48.000000 mappyfile-1.0.0/mappyfile/schemas/cluster.json
--rw-rw-rw-   0        0        0      335 2023-08-02 07:58:46.000000 mappyfile-1.0.0/mappyfile/schemas/color.json
--rw-rw-rw-   0        0        0     1140 2022-06-13 21:01:53.000000 mappyfile-1.0.0/mappyfile/schemas/composite.json
--rw-rw-rw-   0        0        0      128 2020-01-09 23:26:49.000000 mappyfile-1.0.0/mappyfile/schemas/connectionoptions.json
--rw-rw-rw-   0        0        0       51 2017-10-01 10:38:49.000000 mappyfile-1.0.0/mappyfile/schemas/debug.json
--rw-rw-rw-   0        0        0      274 2017-10-01 11:25:03.000000 mappyfile-1.0.0/mappyfile/schemas/expression.json
--rw-rw-rw-   0        0        0      103 2023-08-02 07:58:42.000000 mappyfile-1.0.0/mappyfile/schemas/extent.json
--rw-rw-rw-   0        0        0      668 2018-06-11 10:04:25.000000 mappyfile-1.0.0/mappyfile/schemas/feature.json
--rw-rw-rw-   0        0        0     1015 2022-06-13 21:01:53.000000 mappyfile-1.0.0/mappyfile/schemas/grid.json
--rw-rw-rw-   0        0        0      105 2017-09-20 14:03:32.000000 mappyfile-1.0.0/mappyfile/schemas/hex.json
--rw-rw-rw-   0        0        0      107 2017-09-20 17:48:38.000000 mappyfile-1.0.0/mappyfile/schemas/hex2.json
--rw-rw-rw-   0        0        0     1064 2019-10-06 21:14:50.000000 mappyfile-1.0.0/mappyfile/schemas/join.json
--rw-rw-rw-   0        0        0     8076 2023-08-13 10:02:15.000000 mappyfile-1.0.0/mappyfile/schemas/label.json
--rw-rw-rw-   0        0        0     7362 2023-08-13 10:24:53.000000 mappyfile-1.0.0/mappyfile/schemas/layer.json
--rw-rw-rw-   0        0        0      563 2023-04-20 10:27:46.000000 mappyfile-1.0.0/mappyfile/schemas/leader.json
--rw-rw-rw-   0        0        0     1668 2022-02-21 21:03:48.000000 mappyfile-1.0.0/mappyfile/schemas/legend.json
--rw-rw-rw-   0        0        0     3888 2023-08-13 11:04:08.000000 mappyfile-1.0.0/mappyfile/schemas/map.json
--rw-rw-rw-   0        0        0       82 2017-09-26 10:20:23.000000 mappyfile-1.0.0/mappyfile/schemas/metadata.json
--rw-rw-rw-   0        0        0       51 2017-09-24 22:00:41.000000 mappyfile-1.0.0/mappyfile/schemas/onoff.json
--rw-rw-rw-   0        0        0     1056 2022-06-13 21:01:53.000000 mappyfile-1.0.0/mappyfile/schemas/outputformat.json
--rw-rw-rw-   0        0        0      192 2018-01-16 16:42:03.000000 mappyfile-1.0.0/mappyfile/schemas/points.json
--rw-rw-rw-   0        0        0       72 2017-09-24 21:58:49.000000 mappyfile-1.0.0/mappyfile/schemas/position.json
--rw-rw-rw-   0        0        0      165 2018-02-07 23:07:41.000000 mappyfile-1.0.0/mappyfile/schemas/projection.json
--rw-rw-rw-   0        0        0      795 2022-02-21 21:03:49.000000 mappyfile-1.0.0/mappyfile/schemas/querymap.json
--rw-rw-rw-   0        0        0     1200 2022-02-21 21:03:49.000000 mappyfile-1.0.0/mappyfile/schemas/reference.json
--rw-rw-rw-   0        0        0      143 2017-09-20 14:01:00.000000 mappyfile-1.0.0/mappyfile/schemas/rgb.json
--rw-rw-rw-   0        0        0     2604 2022-02-21 21:03:49.000000 mappyfile-1.0.0/mappyfile/schemas/scalebar.json
--rw-rw-rw-   0        0        0      466 2018-06-11 10:04:25.000000 mappyfile-1.0.0/mappyfile/schemas/scaletoken.json
--rw-rw-rw-   0        0        0       96 2017-09-23 23:25:20.000000 mappyfile-1.0.0/mappyfile/schemas/sizeunits.json
--rw-rw-rw-   0        0        0     6505 2023-06-01 15:35:22.000000 mappyfile-1.0.0/mappyfile/schemas/style.json
--rw-rw-rw-   0        0        0     1620 2022-02-21 21:03:49.000000 mappyfile-1.0.0/mappyfile/schemas/symbol.json
--rw-rw-rw-   0        0        0      323 2021-12-06 13:53:21.000000 mappyfile-1.0.0/mappyfile/schemas/symbolset.json
--rw-rw-rw-   0        0        0       93 2017-10-01 10:10:15.000000 mappyfile-1.0.0/mappyfile/schemas/units.json
--rw-rw-rw-   0        0        0       82 2017-09-26 10:20:23.000000 mappyfile-1.0.0/mappyfile/schemas/validation.json
--rw-rw-rw-   0        0        0     2149 2022-02-21 21:03:49.000000 mappyfile-1.0.0/mappyfile/schemas/web.json
--rw-rw-rw-   0        0        0       52 2018-05-14 10:05:23.000000 mappyfile-1.0.0/mappyfile/schemas/yesno.json
--rw-rw-rw-   0        0        0     6275 2023-08-13 10:25:39.000000 mappyfile-1.0.0/mappyfile/tokens.py
--rw-rw-rw-   0        0        0    23783 2023-08-13 18:01:01.000000 mappyfile-1.0.0/mappyfile/transformer.py
--rw-rw-rw-   0        0        0    14610 2023-08-13 18:01:01.000000 mappyfile-1.0.0/mappyfile/utils.py
--rw-rw-rw-   0        0        0    11983 2023-08-13 18:01:01.000000 mappyfile-1.0.0/mappyfile/validator.py
-drwxrwxrwx   0        0        0        0 2023-09-28 09:33:41.573296 mappyfile-1.0.0/mappyfile.egg-info/
--rw-rw-rw-   0        0        0     5431 2023-09-28 09:33:40.000000 mappyfile-1.0.0/mappyfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2610 2023-09-28 09:33:40.000000 mappyfile-1.0.0/mappyfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-28 09:33:40.000000 mappyfile-1.0.0/mappyfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-09-28 09:33:40.000000 mappyfile-1.0.0/mappyfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-08-14 09:32:10.000000 mappyfile-1.0.0/mappyfile.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       87 2023-09-28 09:33:40.000000 mappyfile-1.0.0/mappyfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-09-28 09:33:40.000000 mappyfile-1.0.0/mappyfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1002 2023-07-27 16:39:13.000000 mappyfile-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      169 2023-09-28 09:33:42.732295 mappyfile-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1697 2023-09-28 08:53:25.000000 mappyfile-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-28 09:33:42.719296 mappyfile-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2017-07-06 19:50:13.000000 mappyfile-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0      485 2023-09-02 14:55:20.000000 mappyfile-1.0.0/tests/test_cli.py
--rw-rw-rw-   0        0        0     8326 2023-08-01 14:59:09.000000 mappyfile-1.0.0/tests/test_comments.py
--rw-rw-rw-   0        0        0     7563 2023-08-13 18:01:01.000000 mappyfile-1.0.0/tests/test_dictutils.py
--rw-rw-rw-   0        0        0     2579 2023-07-27 22:39:55.000000 mappyfile-1.0.0/tests/test_errors.py
--rw-rw-rw-   0        0        0    10925 2023-06-02 06:55:32.000000 mappyfile-1.0.0/tests/test_expressions.py
--rw-rw-rw-   0        0        0     3213 2023-06-02 06:55:32.000000 mappyfile-1.0.0/tests/test_includes.py
--rw-rw-rw-   0        0        0     1933 2023-08-13 10:07:02.000000 mappyfile-1.0.0/tests/test_map_collection.py
--rw-rw-rw-   0        0        0     3220 2023-08-13 10:45:27.000000 mappyfile-1.0.0/tests/test_msautotest.py
--rw-rw-rw-   0        0        0     4634 2023-06-02 06:55:33.000000 mappyfile-1.0.0/tests/test_ordereddict.py
--rw-rw-rw-   0        0        0    12135 2023-08-13 18:01:01.000000 mappyfile-1.0.0/tests/test_pprint.py
--rw-rw-rw-   0        0        0      923 2023-08-13 18:01:01.000000 mappyfile-1.0.0/tests/test_quoter.py
--rw-rw-rw-   0        0        0     4162 2023-08-13 10:00:33.000000 mappyfile-1.0.0/tests/test_sample_maps.py
--rw-rw-rw-   0        0        0    24396 2023-08-13 10:28:11.000000 mappyfile-1.0.0/tests/test_snippets.py
--rw-rw-rw-   0        0        0     2045 2023-06-02 06:55:33.000000 mappyfile-1.0.0/tests/test_symbolset.py
--rw-rw-rw-   0        0        0     8398 2023-08-13 12:59:09.000000 mappyfile-1.0.0/tests/test_transformer.py
--rw-rw-rw-   0        0        0     4262 2023-08-13 18:01:01.000000 mappyfile-1.0.0/tests/test_utils.py
--rw-rw-rw-   0        0        0    14374 2023-08-13 11:04:08.000000 mappyfile-1.0.0/tests/test_validation.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.693572 mappyfile-1.0.1/
+-rw-rw-rw-   0        0        0     1089 2017-07-06 19:50:13.000000 mappyfile-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       78 2017-10-02 08:44:46.000000 mappyfile-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5410 2024-04-26 08:39:05.693572 mappyfile-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4546 2023-09-28 08:55:09.000000 mappyfile-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.386873 mappyfile-1.0.1/docs/
+-rw-rw-rw-   0        0        0        9 2023-08-11 15:22:45.000000 mappyfile-1.0.1/docs/.gitignore
+-rw-rw-rw-   0        0        0    17323 2023-10-05 06:43:32.000000 mappyfile-1.0.1/docs/HISTORY.rst
+-rw-rw-rw-   0        0        0     7843 2017-07-06 19:50:13.000000 mappyfile-1.0.1/docs/Makefile
+-rw-rw-rw-   0        0        0     3354 2020-07-14 05:32:08.000000 mappyfile-1.0.1/docs/client.rst
+-rw-rw-rw-   0        0        0     3710 2023-08-13 18:55:15.000000 mappyfile-1.0.1/docs/comments.rst
+-rw-rw-rw-   0        0        0    19393 2023-08-11 15:48:40.000000 mappyfile-1.0.1/docs/conf.py
+-rw-rw-rw-   0        0        0     2882 2023-09-28 07:25:03.000000 mappyfile-1.0.1/docs/development.rst
+-rw-rw-rw-   0        0        0     3237 2023-08-13 18:25:58.000000 mappyfile-1.0.1/docs/editing.rst
+-rw-rw-rw-   0        0        0     1655 2018-08-22 22:23:30.000000 mappyfile-1.0.1/docs/format.txt
+-rw-rw-rw-   0        0        0     7176 2023-04-20 10:21:52.000000 mappyfile-1.0.1/docs/grammar.rst
+-rw-rw-rw-   0        0        0    10113 2023-09-28 07:56:02.000000 mappyfile-1.0.1/docs/index.rst
+-rwxrwxrwx   0        0        0     7738 2017-07-06 19:50:13.000000 mappyfile-1.0.1/docs/make.bat
+-rw-rw-rw-   0        0        0     6378 2023-08-11 15:31:23.000000 mappyfile-1.0.1/docs/parser.rst
+-rw-rw-rw-   0        0        0    12725 2017-07-06 19:50:13.000000 mappyfile-1.0.1/docs/performance.txt
+-rw-rw-rw-   0        0        0     5423 2023-08-13 18:28:48.000000 mappyfile-1.0.1/docs/pretty_printing.rst
+-rw-rw-rw-   0        0        0     1144 2023-08-11 14:50:51.000000 mappyfile-1.0.1/docs/python_integration.rst
+-rw-rw-rw-   0        0        0       13 2024-04-25 14:10:28.000000 mappyfile-1.0.1/docs/requirements.txt
+-rw-rw-rw-   0        0        0    10515 2023-08-13 18:15:54.000000 mappyfile-1.0.1/docs/rfc.rst
+-rw-rw-rw-   0        0        0     1692 2017-07-06 19:50:13.000000 mappyfile-1.0.1/docs/sample_dict.json
+-rw-rw-rw-   0        0        0      879 2017-07-06 19:50:13.000000 mappyfile-1.0.1/docs/sample_map.txt
+-rw-rw-rw-   0        0        0     2723 2023-08-11 17:41:30.000000 mappyfile-1.0.1/docs/schemas.rst
+-rw-rw-rw-   0        0        0     3497 2023-08-13 18:03:47.000000 mappyfile-1.0.1/docs/testing.rst
+-rw-rw-rw-   0        0        0     2268 2023-08-13 18:22:08.000000 mappyfile-1.0.1/docs/transformer.rst
+-rw-rw-rw-   0        0        0      923 2018-08-22 22:23:30.000000 mappyfile-1.0.1/docs/validate.txt
+-rw-rw-rw-   0        0        0     5919 2023-08-13 08:30:20.000000 mappyfile-1.0.1/docs/validation.rst
+-rw-rw-rw-   0        0        0      305 2018-08-22 22:23:30.000000 mappyfile-1.0.1/docs/validation_errors.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.406803 mappyfile-1.0.1/mappyfile/
+-rw-rw-rw-   0        0        0     2534 2024-03-14 12:58:45.000000 mappyfile-1.0.1/mappyfile/__init__.py
+-rw-rw-rw-   0        0        0     8598 2023-08-13 12:38:53.000000 mappyfile-1.0.1/mappyfile/cli.py
+-rw-rw-rw-   0        0        0     8716 2024-04-25 14:05:28.000000 mappyfile-1.0.1/mappyfile/dictutils.py
+-rw-rw-rw-   0        0        0     5600 2024-01-11 16:05:39.000000 mappyfile-1.0.1/mappyfile/mapfile.lark
+-rw-rw-rw-   0        0        0     5223 2023-08-13 18:01:01.000000 mappyfile-1.0.1/mappyfile/ordereddict.py
+-rw-rw-rw-   0        0        0     8626 2024-01-12 14:23:25.000000 mappyfile-1.0.1/mappyfile/parser.py
+-rw-rw-rw-   0        0        0    20742 2024-01-12 14:23:25.000000 mappyfile-1.0.1/mappyfile/pprint.py
+-rw-rw-rw-   0        0        0        0 2023-08-14 14:48:56.000000 mappyfile-1.0.1/mappyfile/py.typed
+-rw-rw-rw-   0        0        0     4021 2023-08-13 12:18:42.000000 mappyfile-1.0.1/mappyfile/quoter.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.475840 mappyfile-1.0.1/mappyfile/schemas/
+-rw-rw-rw-   0        0        0     3134 2024-01-12 14:40:01.000000 mappyfile-1.0.1/mappyfile/schemas/class.json
+-rw-rw-rw-   0        0        0      815 2022-02-21 21:03:48.000000 mappyfile-1.0.1/mappyfile/schemas/cluster.json
+-rw-rw-rw-   0        0        0      335 2023-08-02 07:58:46.000000 mappyfile-1.0.1/mappyfile/schemas/color.json
+-rw-rw-rw-   0        0        0     1140 2022-06-13 21:01:53.000000 mappyfile-1.0.1/mappyfile/schemas/composite.json
+-rw-rw-rw-   0        0        0      128 2020-01-09 23:26:49.000000 mappyfile-1.0.1/mappyfile/schemas/connectionoptions.json
+-rw-rw-rw-   0        0        0       51 2017-10-01 10:38:49.000000 mappyfile-1.0.1/mappyfile/schemas/debug.json
+-rw-rw-rw-   0        0        0      274 2024-01-12 14:39:15.000000 mappyfile-1.0.1/mappyfile/schemas/expression.json
+-rw-rw-rw-   0        0        0      103 2023-08-02 07:58:42.000000 mappyfile-1.0.1/mappyfile/schemas/extent.json
+-rw-rw-rw-   0        0        0      668 2018-06-11 10:04:25.000000 mappyfile-1.0.1/mappyfile/schemas/feature.json
+-rw-rw-rw-   0        0        0     1015 2022-06-13 21:01:53.000000 mappyfile-1.0.1/mappyfile/schemas/grid.json
+-rw-rw-rw-   0        0        0      105 2017-09-20 14:03:32.000000 mappyfile-1.0.1/mappyfile/schemas/hex.json
+-rw-rw-rw-   0        0        0      107 2017-09-20 17:48:38.000000 mappyfile-1.0.1/mappyfile/schemas/hex2.json
+-rw-rw-rw-   0        0        0     1064 2019-10-06 21:14:50.000000 mappyfile-1.0.1/mappyfile/schemas/join.json
+-rw-rw-rw-   0        0        0     8076 2023-08-13 10:02:15.000000 mappyfile-1.0.1/mappyfile/schemas/label.json
+-rw-rw-rw-   0        0        0     7362 2023-08-13 10:24:53.000000 mappyfile-1.0.1/mappyfile/schemas/layer.json
+-rw-rw-rw-   0        0        0      563 2023-04-20 10:27:46.000000 mappyfile-1.0.1/mappyfile/schemas/leader.json
+-rw-rw-rw-   0        0        0     1668 2022-02-21 21:03:48.000000 mappyfile-1.0.1/mappyfile/schemas/legend.json
+-rw-rw-rw-   0        0        0     3888 2023-08-13 11:04:08.000000 mappyfile-1.0.1/mappyfile/schemas/map.json
+-rw-rw-rw-   0        0        0       82 2017-09-26 10:20:23.000000 mappyfile-1.0.1/mappyfile/schemas/metadata.json
+-rw-rw-rw-   0        0        0       51 2017-09-24 22:00:41.000000 mappyfile-1.0.1/mappyfile/schemas/onoff.json
+-rw-rw-rw-   0        0        0     1056 2022-06-13 21:01:53.000000 mappyfile-1.0.1/mappyfile/schemas/outputformat.json
+-rw-rw-rw-   0        0        0      192 2018-01-16 16:42:03.000000 mappyfile-1.0.1/mappyfile/schemas/points.json
+-rw-rw-rw-   0        0        0       72 2017-09-24 21:58:49.000000 mappyfile-1.0.1/mappyfile/schemas/position.json
+-rw-rw-rw-   0        0        0      165 2018-02-07 23:07:41.000000 mappyfile-1.0.1/mappyfile/schemas/projection.json
+-rw-rw-rw-   0        0        0      795 2022-02-21 21:03:49.000000 mappyfile-1.0.1/mappyfile/schemas/querymap.json
+-rw-rw-rw-   0        0        0     1200 2022-02-21 21:03:49.000000 mappyfile-1.0.1/mappyfile/schemas/reference.json
+-rw-rw-rw-   0        0        0      143 2017-09-20 14:01:00.000000 mappyfile-1.0.1/mappyfile/schemas/rgb.json
+-rw-rw-rw-   0        0        0     2604 2022-02-21 21:03:49.000000 mappyfile-1.0.1/mappyfile/schemas/scalebar.json
+-rw-rw-rw-   0        0        0      466 2018-06-11 10:04:25.000000 mappyfile-1.0.1/mappyfile/schemas/scaletoken.json
+-rw-rw-rw-   0        0        0       96 2017-09-23 23:25:20.000000 mappyfile-1.0.1/mappyfile/schemas/sizeunits.json
+-rw-rw-rw-   0        0        0     6505 2023-06-01 15:35:22.000000 mappyfile-1.0.1/mappyfile/schemas/style.json
+-rw-rw-rw-   0        0        0     1620 2022-02-21 21:03:49.000000 mappyfile-1.0.1/mappyfile/schemas/symbol.json
+-rw-rw-rw-   0        0        0      323 2021-12-06 13:53:21.000000 mappyfile-1.0.1/mappyfile/schemas/symbolset.json
+-rw-rw-rw-   0        0        0       93 2017-10-01 10:10:15.000000 mappyfile-1.0.1/mappyfile/schemas/units.json
+-rw-rw-rw-   0        0        0       82 2017-09-26 10:20:23.000000 mappyfile-1.0.1/mappyfile/schemas/validation.json
+-rw-rw-rw-   0        0        0     2149 2022-02-21 21:03:49.000000 mappyfile-1.0.1/mappyfile/schemas/web.json
+-rw-rw-rw-   0        0        0       52 2018-05-14 10:05:23.000000 mappyfile-1.0.1/mappyfile/schemas/yesno.json
+-rw-rw-rw-   0        0        0     6275 2024-01-12 14:23:25.000000 mappyfile-1.0.1/mappyfile/tokens.py
+-rw-rw-rw-   0        0        0    23783 2024-01-12 14:23:25.000000 mappyfile-1.0.1/mappyfile/transformer.py
+-rw-rw-rw-   0        0        0    14610 2023-08-13 18:01:01.000000 mappyfile-1.0.1/mappyfile/utils.py
+-rw-rw-rw-   0        0        0    11983 2023-08-13 18:01:01.000000 mappyfile-1.0.1/mappyfile/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.421517 mappyfile-1.0.1/mappyfile.egg-info/
+-rw-rw-rw-   0        0        0     5410 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-14 09:32:10.000000 mappyfile-1.0.1/mappyfile.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       87 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1002 2023-07-27 16:39:13.000000 mappyfile-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      169 2024-04-26 08:39:05.696573 mappyfile-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2023-09-28 08:53:25.000000 mappyfile-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.691564 mappyfile-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2017-07-06 19:50:13.000000 mappyfile-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-09-02 14:55:20.000000 mappyfile-1.0.1/tests/test_cli.py
+-rw-rw-rw-   0        0        0     8326 2023-08-01 14:59:09.000000 mappyfile-1.0.1/tests/test_comments.py
+-rw-rw-rw-   0        0        0     1882 2024-01-11 21:03:52.000000 mappyfile-1.0.1/tests/test_config.py
+-rw-rw-rw-   0        0        0     8512 2024-04-26 08:37:25.000000 mappyfile-1.0.1/tests/test_dictutils.py
+-rw-rw-rw-   0        0        0     2579 2023-07-27 22:39:55.000000 mappyfile-1.0.1/tests/test_errors.py
+-rw-rw-rw-   0        0        0    10925 2023-06-02 06:55:32.000000 mappyfile-1.0.1/tests/test_expressions.py
+-rw-rw-rw-   0        0        0     3213 2023-06-02 06:55:32.000000 mappyfile-1.0.1/tests/test_includes.py
+-rw-rw-rw-   0        0        0     1933 2023-08-13 10:07:02.000000 mappyfile-1.0.1/tests/test_map_collection.py
+-rw-rw-rw-   0        0        0     3220 2023-08-13 10:45:27.000000 mappyfile-1.0.1/tests/test_msautotest.py
+-rw-rw-rw-   0        0        0     4634 2023-06-02 06:55:33.000000 mappyfile-1.0.1/tests/test_ordereddict.py
+-rw-rw-rw-   0        0        0    12135 2023-08-13 18:01:01.000000 mappyfile-1.0.1/tests/test_pprint.py
+-rw-rw-rw-   0        0        0      923 2023-08-13 18:01:01.000000 mappyfile-1.0.1/tests/test_quoter.py
+-rw-rw-rw-   0        0        0     4162 2023-08-13 10:00:33.000000 mappyfile-1.0.1/tests/test_sample_maps.py
+-rw-rw-rw-   0        0        0    24723 2024-01-12 14:41:23.000000 mappyfile-1.0.1/tests/test_snippets.py
+-rw-rw-rw-   0        0        0     2045 2023-06-02 06:55:33.000000 mappyfile-1.0.1/tests/test_symbolset.py
+-rw-rw-rw-   0        0        0     8398 2023-08-13 12:59:09.000000 mappyfile-1.0.1/tests/test_transformer.py
+-rw-rw-rw-   0        0        0     4262 2023-08-13 18:01:01.000000 mappyfile-1.0.1/tests/test_utils.py
+-rw-rw-rw-   0        0        0    14374 2024-01-12 14:23:25.000000 mappyfile-1.0.1/tests/test_validation.py
```

### Comparing `mappyfile-1.0.0/LICENSE` & `mappyfile-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/PKG-INFO` & `mappyfile-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: mappyfile
-Version: 1.0.0
+Version: 1.0.1
 Summary: A pure Python MapFile parser for working with MapServer
 Home-page: http://github.com/geographika/mappyfile
 Author: Seth Girvin
 Author-email: sethg@geographika.co.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
@@ -152,8 +151,7 @@
 
 .. |Coveralls| image:: https://coveralls.io/repos/github/geographika/mappyfile/badge.svg?branch=master
     :target: https://coveralls.io/github/geographika/mappyfile?branch=master
 
 .. |Downloads| image:: https://static.pepy.tech/badge/mappyfile
     :target: https://www.pepy.tech/projects/mappyfile
     
-
```

### Comparing `mappyfile-1.0.0/README.rst` & `mappyfile-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/HISTORY.rst` & `mappyfile-1.0.1/docs/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,28 @@
         # replace the following parameter
         # transformerClass=ColorsTransformer,
         transformer_class=ColorsTransformer,
         conversion_type=None,
         include_color_names=True,
     )
 
++ **Breaking Change** - ``LAYER`` ``DATA`` has been changed in the schema from a list to a simple string.
+
+  .. code-block:: python
+
+      layer = {
+          '__type__': 'layer',
+          // pre v1 the data clause had to be in a list
+          // 'data': ['/path/to/data']
+          // in v1 this should now be a string
+          'data': '/path/to/data'
+      }
+
+      mappyfile.dumps(layer)
+
 + Support added for `lark_cython <https://github.com/lark-parser/lark_cython>`_ - see `#178 <https://github.com/geographika/mappyfile/issues/178>`_ - thanks @erezsh.
   To use ``lark_cython`` is as simple as installing the option with ``pip``:
 
   .. code-block:: bash
 
       pip install mappyfile[lark_cython]
```

### Comparing `mappyfile-1.0.0/docs/Makefile` & `mappyfile-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/client.rst` & `mappyfile-1.0.1/docs/client.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/comments.rst` & `mappyfile-1.0.1/docs/comments.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/conf.py` & `mappyfile-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/development.rst` & `mappyfile-1.0.1/docs/development.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/editing.rst` & `mappyfile-1.0.1/docs/editing.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/format.txt` & `mappyfile-1.0.1/docs/format.txt`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/grammar.rst` & `mappyfile-1.0.1/docs/grammar.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/index.rst` & `mappyfile-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/make.bat` & `mappyfile-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/parser.rst` & `mappyfile-1.0.1/docs/parser.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/performance.txt` & `mappyfile-1.0.1/docs/performance.txt`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/pretty_printing.rst` & `mappyfile-1.0.1/docs/pretty_printing.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/python_integration.rst` & `mappyfile-1.0.1/docs/python_integration.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/rfc.rst` & `mappyfile-1.0.1/docs/rfc.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/sample_dict.json` & `mappyfile-1.0.1/docs/sample_dict.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/sample_map.txt` & `mappyfile-1.0.1/docs/sample_map.txt`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/schemas.rst` & `mappyfile-1.0.1/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/testing.rst` & `mappyfile-1.0.1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/transformer.rst` & `mappyfile-1.0.1/docs/transformer.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/validate.txt` & `mappyfile-1.0.1/docs/validate.txt`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/docs/validation.rst` & `mappyfile-1.0.1/docs/validation.rst`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/__init__.py` & `mappyfile-1.0.1/mappyfile/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     findall,
     findkey,
     findunique,
     update,
     dict_move_to_end,
 )
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 __all__ = [
     "open",
     "load",
     "loads",
     "find",
     "findall",
```

### Comparing `mappyfile-1.0.0/mappyfile/cli.py` & `mappyfile-1.0.1/mappyfile/cli.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/dictutils.py` & `mappyfile-1.0.1/mappyfile/dictutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         END
         '''
 
         d = mappyfile.loads(s)
         layers = mappyfile.findall(d["layers"], "group", "test")
         assert len(layers) == 2
     """
-    return [item for item in lst if item[key.lower()] in value]
+    return [item for item in lst if item[key.lower()] and item[key.lower()] in value]
 
 
 def findunique(lst, key):
     """
     Find all unique key values for items in lst. If no
     items with the key are found an empty list is returned.
```

### Comparing `mappyfile-1.0.0/mappyfile/mapfile.lark` & `mappyfile-1.0.1/mappyfile/mapfile.lark`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/ordereddict.py` & `mappyfile-1.0.1/mappyfile/ordereddict.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/parser.py` & `mappyfile-1.0.1/mappyfile/parser.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/pprint.py` & `mappyfile-1.0.1/mappyfile/pprint.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/quoter.py` & `mappyfile-1.0.1/mappyfile/quoter.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/class.json` & `mappyfile-1.0.1/mappyfile/schemas/class.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/cluster.json` & `mappyfile-1.0.1/mappyfile/schemas/cluster.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/composite.json` & `mappyfile-1.0.1/mappyfile/schemas/composite.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/feature.json` & `mappyfile-1.0.1/mappyfile/schemas/feature.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/grid.json` & `mappyfile-1.0.1/mappyfile/schemas/grid.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/join.json` & `mappyfile-1.0.1/mappyfile/schemas/join.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/label.json` & `mappyfile-1.0.1/mappyfile/schemas/label.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/layer.json` & `mappyfile-1.0.1/mappyfile/schemas/layer.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/leader.json` & `mappyfile-1.0.1/mappyfile/schemas/leader.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/legend.json` & `mappyfile-1.0.1/mappyfile/schemas/legend.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/map.json` & `mappyfile-1.0.1/mappyfile/schemas/map.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/outputformat.json` & `mappyfile-1.0.1/mappyfile/schemas/outputformat.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/querymap.json` & `mappyfile-1.0.1/mappyfile/schemas/querymap.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/reference.json` & `mappyfile-1.0.1/mappyfile/schemas/reference.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/scalebar.json` & `mappyfile-1.0.1/mappyfile/schemas/scalebar.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/style.json` & `mappyfile-1.0.1/mappyfile/schemas/style.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/symbol.json` & `mappyfile-1.0.1/mappyfile/schemas/symbol.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/schemas/web.json` & `mappyfile-1.0.1/mappyfile/schemas/web.json`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/tokens.py` & `mappyfile-1.0.1/mappyfile/tokens.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/transformer.py` & `mappyfile-1.0.1/mappyfile/transformer.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/utils.py` & `mappyfile-1.0.1/mappyfile/utils.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile/validator.py` & `mappyfile-1.0.1/mappyfile/validator.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/mappyfile.egg-info/PKG-INFO` & `mappyfile-1.0.1/mappyfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: mappyfile
-Version: 1.0.0
+Version: 1.0.1
 Summary: A pure Python MapFile parser for working with MapServer
 Home-page: http://github.com/geographika/mappyfile
 Author: Seth Girvin
 Author-email: sethg@geographika.co.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
@@ -152,8 +151,7 @@
 
 .. |Coveralls| image:: https://coveralls.io/repos/github/geographika/mappyfile/badge.svg?branch=master
     :target: https://coveralls.io/github/geographika/mappyfile?branch=master
 
 .. |Downloads| image:: https://static.pepy.tech/badge/mappyfile
     :target: https://www.pepy.tech/projects/mappyfile
     
-
```

### Comparing `mappyfile-1.0.0/mappyfile.egg-info/SOURCES.txt` & `mappyfile-1.0.1/mappyfile.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 mappyfile/schemas/units.json
 mappyfile/schemas/validation.json
 mappyfile/schemas/web.json
 mappyfile/schemas/yesno.json
 tests/__init__.py
 tests/test_cli.py
 tests/test_comments.py
+tests/test_config.py
 tests/test_dictutils.py
 tests/test_errors.py
 tests/test_expressions.py
 tests/test_includes.py
 tests/test_map_collection.py
 tests/test_msautotest.py
 tests/test_ordereddict.py
```

### Comparing `mappyfile-1.0.0/pyproject.toml` & `mappyfile-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/setup.py` & `mappyfile-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_comments.py` & `mappyfile-1.0.1/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_dictutils.py` & `mappyfile-1.0.1/tests/test_dictutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,54 @@
 
     d = mappyfile.loads(s)
     layers = mappyfile.findall(d["layers"], "group", "test")
     assert len(layers) == 2
     assert layers[0]["name"] == "Layer1"
 
 
+def test_findall_missing_value():
+    s = """
+    MAP
+        LAYER
+            NAME "Layer1"
+            TYPE POLYGON
+            GROUP "test"
+        END
+        LAYER
+            NAME "Layer2"
+            TYPE POLYGON
+            GROUP "1test"
+        END
+        LAYER
+            NAME "Layer3"
+            TYPE POLYGON
+            GROUP "test2"
+        END
+        LAYER
+            NAME "Layer4"
+            TYPE POLYGON
+            # GROUP "test"
+        END
+    END
+    """
+
+    d = mappyfile.loads(s)
+    layers = mappyfile.findall(d["layers"], "group", "test")
+    assert len(layers) == 1
+    assert layers[0]["name"] == "Layer1"
+
+
+def test_findall_itasca():
+    fn = "./tests/mapfiles/itasca2.map"
+    d = mappyfile.open(fn)
+    layers = mappyfile.findall(d["layers"], "group", "roads")
+    assert len(layers) == 4
+    assert layers[0]["name"] == "ctyrdln3"
+
+
 def test_update():
     s1 = """
     MAP
         LAYER
             NAME "Layer1"
             TYPE POLYGON
         END
@@ -345,10 +385,11 @@
 
 def run_tests():
     pytest.main(["tests/test_dictutils.py"])
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
-    run_tests()
-    # test_findunique()
+    # run_tests()
+    test_findall_missing_value()
+    test_findall_itasca()
     print("Done!")
```

### Comparing `mappyfile-1.0.0/tests/test_errors.py` & `mappyfile-1.0.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_expressions.py` & `mappyfile-1.0.1/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_includes.py` & `mappyfile-1.0.1/tests/test_includes.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_map_collection.py` & `mappyfile-1.0.1/tests/test_map_collection.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_msautotest.py` & `mappyfile-1.0.1/tests/test_msautotest.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_ordereddict.py` & `mappyfile-1.0.1/tests/test_ordereddict.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_pprint.py` & `mappyfile-1.0.1/tests/test_pprint.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_quoter.py` & `mappyfile-1.0.1/tests/test_quoter.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_sample_maps.py` & `mappyfile-1.0.1/tests/test_sample_maps.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_snippets.py` & `mappyfile-1.0.1/tests/test_snippets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1019,23 +1019,38 @@
 END"""
 
     print(output(s, schema_name="layer"))
     exp = "LAYER NAME 'centerline1' TYPE LINE GEOMTRANSFORM (centerline(densify([shape],5))) END"
     assert output(s, schema_name="leader") == exp
 
 
+def test_class_regex_expression():
+    s = """
+CLASS
+    EXPRESSION /*1/
+    STYLE
+        COLOR 0 255 0
+    END
+END"""
+
+    print(output(s, schema_name="class"))
+    exp = "CLASS EXPRESSION /*1/ STYLE COLOR 0 255 0 END END"
+    assert output(s, schema_name="class") == exp
+
+
 def run_tests():
     r"""
     Need to comment out the following line in C:\VirtualEnvs\mappyfile\Lib\site-packages\pep8.py
     #stdin_get_value = sys.stdin.read
     Or get AttributeError: '_ReplInput' object has no attribute 'read'
     """
     # pytest.main(["tests/test_snippets.py::test_style_pattern"])
     pytest.main(["tests/test_snippets.py"])
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.DEBUG)
     # test_multiple_compfilters()
-    test_geomtransform_nested_function()
+    # test_geomtransform_nested_function()
+    test_class_regex_expression()
     # run_tests()
     print("Done!")
```

### Comparing `mappyfile-1.0.0/tests/test_symbolset.py` & `mappyfile-1.0.1/tests/test_symbolset.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_transformer.py` & `mappyfile-1.0.1/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_utils.py` & `mappyfile-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mappyfile-1.0.0/tests/test_validation.py` & `mappyfile-1.0.1/tests/test_validation.py`

 * *Files identical despite different names*

