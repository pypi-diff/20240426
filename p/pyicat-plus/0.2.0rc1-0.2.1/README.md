# Comparing `tmp/pyicat_plus-0.2.0rc1.tar.gz` & `tmp/pyicat_plus-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyicat_plus-0.2.0rc1.tar", last modified: Fri Apr 19 11:39:30 2024, max compression
+gzip compressed data, was "pyicat_plus-0.2.1.tar", last modified: Fri Apr 26 15:29:10 2024, max compression
```

## Comparing `pyicat_plus-0.2.0rc1.tar` & `pyicat_plus-0.2.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.350351 pyicat_plus-0.2.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     7560 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     3672 2024-04-19 11:39:30.350351 pyicat_plus-0.2.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1636 2024-04-19 11:39:30.350351 pyicat_plus-0.2.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.342352 pyicat_plus-0.2.0rc1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.342352 pyicat_plus-0.2.0rc1/src/pyicat_plus/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-19 11:37:04.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.342352 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2879 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/icat_as_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_from_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2728 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_raw.py
--rw-rw-rw-   0 root         (0) root         (0)    17512 2024-04-03 00:21:24.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/sync_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1138 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/add_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/archive.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      647 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     7708 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/elogbook.py
--rw-rw-rw-   0 root         (0) root         (0)     6376 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/interface.py
--rw-rw-rw-   0 root         (0) root         (0)    14265 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/investigation.py
--rw-rw-rw-   0 root         (0) root         (0)    19360 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/main.py
--rw-rw-rw-   0 root         (0) root         (0)     4049 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/messaging.py
--rw-rw-rw-   0 root         (0) root         (0)     2723 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/null.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/update_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     2763 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/client/xmlns.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11075 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2024-04-19 05:17:41.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/hdf5_cfg.xml
--rw-rw-rw-   0 root         (0) root         (0)     2168 2024-04-18 15:13:55.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/namespace_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/nexus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11429 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/icat.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/proc.py
--rw-rw-rw-   0 root         (0) root         (0)     3117 2024-03-24 19:22:59.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/tcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2858 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/activemq_rest_server.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/icat_db.py
--rw-rw-rw-   0 root         (0) root         (0)     9204 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/icatplus_server.py
--rw-rw-rw-   0 root         (0) root         (0)     2386 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/stomp_publisher.py
--rw-rw-rw-   0 root         (0) root         (0)     6660 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/stomp_subscriber.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4054 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     4316 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_elogbook.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_add_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1560 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     3806 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    15798 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_investigations.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_mockup.py
--rw-rw-rw-   0 root         (0) root         (0)     3800 2024-04-08 07:20:19.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)    21005 2024-04-03 00:12:57.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_sync.py
--rw-rw-rw-   0 root         (0) root         (0)     4548 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_update_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_maxsizedict.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2024-04-07 16:03:54.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_url_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/compare.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.346351 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 11:39:26.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1253 2024-04-02 10:49:31.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/log_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/maxsizedict.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/path_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6944 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/raw_data.py
--rw-rw-rw-   0 root         (0) root         (0)    12868 2024-04-03 00:21:24.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/sync_store.py
--rw-rw-rw-   0 root         (0) root         (0)    12546 2024-04-02 17:52:39.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/sync_types.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2024-03-07 17:03:13.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 11:39:30.350351 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3672 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2916 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-19 11:39:30.000000 pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.744470 pyicat_plus-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7560 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     3669 2024-04-26 15:29:10.744470 pyicat_plus-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2024-04-26 15:29:10.744470 pyicat_plus-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.728469 pyicat_plus-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.728469 pyicat_plus-0.2.1/src/pyicat_plus/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-26 15:27:49.000000 pyicat_plus-0.2.1/src/pyicat_plus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.732469 pyicat_plus-0.2.1/src/pyicat_plus/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 15:29:05.000000 pyicat_plus-0.2.1/src/pyicat_plus/apps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2879 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/apps/icat_as_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/apps/store_from_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/apps/store_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/apps/store_raw.py
+-rw-rw-rw-   0 root         (0) root         (0)    18012 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/apps/sync_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.732469 pyicat_plus-0.2.1/src/pyicat_plus/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 15:29:05.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/add_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     7708 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/elogbook.py
+-rw-rw-rw-   0 root         (0) root         (0)     6376 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/interface.py
+-rw-rw-rw-   0 root         (0) root         (0)    14265 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/investigation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19360 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     4049 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/messaging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/null.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/update_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2763 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/client/xmlns.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.736469 pyicat_plus-0.2.1/src/pyicat_plus/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 15:29:05.000000 pyicat_plus-0.2.1/src/pyicat_plus/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11075 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/metadata/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/metadata/hdf5_cfg.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2168 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/metadata/namespace_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/metadata/nexus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.736469 pyicat_plus-0.2.1/src/pyicat_plus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 15:29:05.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.736469 pyicat_plus-0.2.1/src/pyicat_plus/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 15:29:05.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11429 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/fixtures/icat.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/fixtures/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/fixtures/proc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/fixtures/tcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.740469 pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 15:29:05.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2858 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/activemq_rest_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/icat_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     9204 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/icatplus_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/stomp_publisher.py
+-rw-rw-rw-   0 root         (0) root         (0)     6660 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/stomp_subscriber.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4054 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     4316 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_elogbook.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_add_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3806 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15798 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_investigations.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_mockup.py
+-rw-rw-rw-   0 root         (0) root         (0)     3800 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)    21005 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_sync.py
+-rw-rw-rw-   0 root         (0) root         (0)     4548 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_update_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_maxsizedict.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/test_url_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.740469 pyicat_plus-0.2.1/src/pyicat_plus/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 15:29:05.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/utils/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/tests/utils/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.740469 pyicat_plus-0.2.1/src/pyicat_plus/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 15:29:05.000000 pyicat_plus-0.2.1/src/pyicat_plus/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/utils/log_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/utils/maxsizedict.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/utils/path_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6944 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/utils/raw_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    13068 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/utils/sync_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    13015 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/utils/sync_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-04-26 14:18:18.000000 pyicat_plus-0.2.1/src/pyicat_plus/utils/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:29:10.740469 pyicat_plus-0.2.1/src/pyicat_plus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3669 2024-04-26 15:29:10.000000 pyicat_plus-0.2.1/src/pyicat_plus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2916 2024-04-26 15:29:10.000000 pyicat_plus-0.2.1/src/pyicat_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 15:29:10.000000 pyicat_plus-0.2.1/src/pyicat_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-26 15:29:10.000000 pyicat_plus-0.2.1/src/pyicat_plus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-26 15:29:10.000000 pyicat_plus-0.2.1/src/pyicat_plus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-26 15:29:10.000000 pyicat_plus-0.2.1/src/pyicat_plus.egg-info/top_level.txt
```

### Comparing `pyicat_plus-0.2.0rc1/LICENSE.md` & `pyicat_plus-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/PKG-INFO` & `pyicat_plus-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyicat-plus
-Version: 0.2.0rc1
+Version: 0.2.1
 Summary: Python client to ICAT+
 Home-page: https://gitlab.esrf.fr/icat/pyicat-plus/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/pyicat-plus/
 Project-URL: Documentation, https://pyicat-plus.readthedocs.io/
```

### Comparing `pyicat_plus-0.2.0rc1/README.md` & `pyicat_plus-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/setup.cfg` & `pyicat_plus-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/icat_as_nexus.py` & `pyicat_plus-0.2.1/src/pyicat_plus/apps/icat_as_nexus.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_from_file.py` & `pyicat_plus-0.2.1/src/pyicat_plus/apps/store_from_file.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_processed.py` & `pyicat_plus-0.2.1/src/pyicat_plus/apps/store_processed.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/store_raw.py` & `pyicat_plus-0.2.1/src/pyicat_plus/apps/store_raw.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/apps/sync_raw.py` & `pyicat_plus-0.2.1/src/pyicat_plus/apps/sync_raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import logging
 import argparse
 import datetime
 from tqdm import tqdm
 from time import sleep
 from glob import glob
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Generator
 
 from ..utils import raw_data
 from ..utils import path_utils
 from ..utils import sync_types
 from ..client.main import IcatClient
 from ..client.bliss import get_icat_client
 from ..utils.log_utils import basic_config
@@ -23,14 +23,15 @@
 def sync_raw(
     icat_client: IcatClient,
     beamline: Optional[str] = None,
     proposal: Optional[str] = None,
     session: Optional[str] = None,
     root_dir: Optional[str] = None,
     dry_run: bool = True,
+    unsupervised: bool = False,
     raw_data_format: str = "esrfv3",
     save_dir: Optional[str] = None,
     cache_dir: Optional[str] = None,
     invalidate_cache: bool = False,
 ) -> None:
     with ExperimentalSessionStore(
         cache_dir=cache_dir,
@@ -71,14 +72,15 @@
             try:
                 _ = sync_session(
                     icat_client,
                     proposal_from_dir,
                     beamline_from_dir,
                     session_from_dir,
                     dry_run=dry_run,
+                    unsupervised=unsupervised,
                     raw_data_format=raw_data_format,
                     exp_session_store=exp_session_store,
                 )
             except Exception as e:
                 raise RuntimeError(
                     f"Failed syncing beamline={beamline_from_dir}, proposal={proposal_from_dir}, session={session_from_dir}"
                 ) from e
@@ -88,14 +90,15 @@
 def sync_session(
     icat_client: IcatClient,
     proposal: str,
     beamline: str,
     session: str,
     root_dir: Optional[str] = None,
     dry_run: bool = True,
+    unsupervised: bool = False,
     allow_open_ended: bool = True,
     raw_data_format: str = "esrfv3",
     exp_session_store: Optional[ExperimentalSessionStore] = None,
 ) -> Optional[sync_types.ExperimentalSession]:
     remove_from_cache_afterwards = False
     exp_session = None
     try:
@@ -134,77 +137,94 @@
                 raw_data_format=raw_data_format,
             )
 
         # Print summary of the experimental session
         exp_session.pprint()
 
         # Register datasets that failed to be registered
-        datasets = exp_session.datasets["not_uploaded"]
-        if datasets:
-            action = 'Upload "not uploaded" dataset'
-            execute = not dry_run and _ask_execute_confirmation(
-                exp_session, action + "s"
-            )
-            if not execute:
-                datasets = []
-            for dataset in datasets:
-                _print_dataset_details(dataset, action)
-                if execute:
-                    remove_from_cache_afterwards = True
-                    icat_client.store_dataset_from_file(dataset.metadata_file)
-                    sleep(0.1)  # do not overload ICAT
+        for dataset in _iter_datasets_to_upload(
+            exp_session, "not_uploaded", dry_run, unsupervised
+        ):
+            remove_from_cache_afterwards = True
+            icat_client.store_dataset_from_file(dataset.metadata_file)
+            sleep(0.1)  # do not overload ICAT
 
         # Register datasets that were not even attempted to be registered
-        datasets = exp_session.datasets["unregistered"]
-        if datasets:
-            action = 'Upload "unregistered" dataset'
-            execute = not dry_run and _ask_execute_confirmation(
-                exp_session, action + "s"
+        for dataset in _iter_datasets_to_upload(
+            exp_session, "unregistered", dry_run, unsupervised
+        ):
+            remove_from_cache_afterwards = True
+            icat_client.store_dataset(
+                beamline=dataset.beamline,
+                proposal=dataset.proposal,
+                dataset=dataset.name,
+                path=dataset.path,
+                metadata=dataset.metadata,
             )
-            if not execute:
-                datasets = []
-            for dataset in datasets:
-                _print_dataset_details(dataset, action)
-                if execute:
-                    remove_from_cache_afterwards = True
-                    icat_client.store_dataset(
-                        beamline=dataset.beamline,
-                        proposal=dataset.proposal,
-                        dataset=dataset.name,
-                        path=dataset.path,
-                        metadata=dataset.metadata,
-                    )
-                    sleep(0.1)  # do not overload ICAT
+            sleep(0.1)  # do not overload ICAT
 
         # Add missing data files for registered datasets without data
-        datasets = exp_session.datasets["registered_without_files"]
-        if datasets:
-            action = 'Upload "registered without files" dataset'
-            execute = not dry_run and _ask_execute_confirmation(
-                exp_session, action + "s"
-            )
-            if not execute:
-                datasets = []
-            for dataset in datasets:
-                _print_dataset_details(dataset, action)
-                if execute:
-                    remove_from_cache_afterwards = True
-                    icat_client.add_files(dataset.icat_dataset.icat_dataset_id)
-                    sleep(0.1)  # do not overload ICAT
+        for dataset in _iter_datasets_to_upload(
+            exp_session, "registered_without_files", dry_run, unsupervised
+        ):
+            remove_from_cache_afterwards = True
+            icat_client.add_files(dataset.icat_dataset.icat_dataset_id)
+            sleep(0.1)  # do not overload ICAT
 
     finally:
         if exp_session_store and exp_session:
             if remove_from_cache_afterwards:
                 exp_session_store.remove_session(exp_session)
             else:
                 exp_session_store.add_session(exp_session)
 
     return exp_session
 
 
+def _iter_datasets_to_upload(
+    exp_session: sync_types.ExperimentalSession,
+    dataset_status: str,
+    dry_run: bool,
+    unsupervised: bool,
+    verbose: bool = False,
+) -> Generator[sync_types.Dataset, None, None]:
+    datasets = exp_session.datasets[dataset_status]
+    if not datasets:
+        return
+
+    action = f'Upload "{dataset_status}" dataset'
+
+    if dry_run:
+        do_yield = False
+        do_print = verbose
+    elif unsupervised:
+        if exp_session.allow_unsupervised_upload(dataset_status):
+            do_yield = True
+            do_print = True
+        else:
+            do_yield = False
+            do_print = verbose
+    else:
+        if _ask_execute_confirmation(exp_session, action + "s"):
+            do_yield = True
+            do_print = True
+        else:
+            do_yield = False
+            do_print = verbose
+
+    if not do_yield and not do_print:
+        return
+
+    for dataset in datasets:
+        if do_print:
+            _print_dataset_details(dataset, action)
+        if do_yield:
+            yield dataset
+
+
 def _ask_execute_confirmation(
     exp_session: sync_types.ExperimentalSession, action: str
 ) -> bool:
     logger.info("Search URL: %s", exp_session.icat_investigation.search_url)
     result = input(f"{action}? (y/[n])")
     return result.lower() in ("y", "yes")
 
@@ -472,15 +492,21 @@
     parser.add_argument(
         "--session", required=False, help="Session name (e.g. 20231028)"
     )
     parser.add_argument(
         "--register",
         action="store_true",
         required=False,
-        help="Register dataset with ICAT when needed",
+        help="Register datasets with ICAT when needed (prompts for confirmation)",
+    )
+    parser.add_argument(
+        "--auto-register",
+        action="store_true",
+        required=False,
+        help="Register datasets with ICAT when needed without confirmation (only when it is safe to do so)",
     )
     parser.add_argument(
         "--format",
         required=False,
         choices=["esrfv1", "esrfv2", "esrfv3", "id16bspec"],
         default="esrfv3",
         help="Raw data structure",
@@ -513,20 +539,24 @@
         logger=logger,
         level=logging.INFO if args.no_print else logging.DEBUG,
         format="%(message)s",
     )
 
     icat_client = get_icat_client(timeout=600)
 
+    dry_run = not args.register and not args.auto_register
+    unsupervised = args.auto_register
+
     sync_raw(
         icat_client,
         beamline=args.beamline,
         proposal=args.proposal,
         session=args.session,
-        dry_run=not args.register,
+        dry_run=dry_run,
+        unsupervised=unsupervised,
         raw_data_format=args.format,
         save_dir=args.save_dir,
         cache_dir=args.cache_dir,
         invalidate_cache=args.invalidate_cache,
     )
 
     icat_client.disconnect()
```

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/add_files.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/add_files.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/archive.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/archive.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/bliss.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/bliss.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/defaults.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/defaults.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/elogbook.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/elogbook.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/interface.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/interface.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/investigation.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/investigation.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/main.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/main.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/messaging.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/messaging.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/metadata.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/metadata.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/null.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/null.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/serialize.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/serialize.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/update_metadata.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/update_metadata.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/client/xmlns.py` & `pyicat_plus-0.2.1/src/pyicat_plus/client/xmlns.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/concurrency.py` & `pyicat_plus-0.2.1/src/pyicat_plus/concurrency.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/definitions.py` & `pyicat_plus-0.2.1/src/pyicat_plus/metadata/definitions.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/namespace_wrapper.py` & `pyicat_plus-0.2.1/src/pyicat_plus/metadata/namespace_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/metadata/nexus.py` & `pyicat_plus-0.2.1/src/pyicat_plus/metadata/nexus.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/icat.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/fixtures/icat.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/proc.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/fixtures/proc.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/fixtures/tcp.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/fixtures/tcp.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/activemq_rest_server.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/activemq_rest_server.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/icat_db.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/icat_db.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/icatplus_server.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/icatplus_server.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/stomp_publisher.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/stomp_publisher.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/servers/stomp_subscriber.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/servers/stomp_subscriber.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_cli.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_elogbook.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_elogbook.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_add_files.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_add_files.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_archive.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_archive.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_datasets.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_datasets.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_definitions.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_definitions.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_investigations.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_investigations.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_nexus.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_nexus.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_serialize.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_serialize.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_sync.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_sync.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_icat_update_metadata.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_icat_update_metadata.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_namespace.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/test_url_utils.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/test_url_utils.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/compare.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/utils/compare.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/tests/utils/message.py` & `pyicat_plus-0.2.1/src/pyicat_plus/tests/utils/message.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/log_utils.py` & `pyicat_plus-0.2.1/src/pyicat_plus/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/maxsizedict.py` & `pyicat_plus-0.2.1/src/pyicat_plus/utils/maxsizedict.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/path_utils.py` & `pyicat_plus-0.2.1/src/pyicat_plus/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/raw_data.py` & `pyicat_plus-0.2.1/src/pyicat_plus/utils/raw_data.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/sync_store.py` & `pyicat_plus-0.2.1/src/pyicat_plus/utils/sync_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,25 +141,28 @@
         ]
 
         register_cmd_params = ""
         if self._save_dir:
             register_cmd_params += f"--save-dir {self._save_dir} "
         if self._cache_dir:
             register_cmd_params += f"--cache-dir {self._cache_dir} "
-        register_cmd_params += "--register"
+        register_cmd_params += '"$@"'
 
         with concurrent.futures.ThreadPoolExecutor() as executor:
             # Clear CSV files and add header
             stats_files = dict(
                 (s, os.path.join(self._save_subdir, s + ".csv")) for s in save_category
             )
 
             def _init_csv(filename):
                 _save_csv_line(filename, save_columns, clear=True)
-                os.chmod(filename, 0o0664)
+                try:
+                    os.chmod(filename, 0o0664)
+                except PermissionError:
+                    pass
 
             _ = list(executor.map(_init_csv, stats_files.values()))
 
             # Clear bash files and add header
             cmd_files = dict(
                 (s, os.path.join(self._save_subdir, s + ".sh")) for s in save_category
             )
@@ -174,20 +177,24 @@
                 _save_file_line(filename, 'if [ -z "$SCRIPT_CACHED" ]; then')
                 _save_file_line(filename, '    SCRIPT_CACHED=$(<"$0")')
                 _save_file_line(filename, '    script_name=$(basename "$0")')
                 _save_file_line(
                     filename, '    echo "$SCRIPT_CACHED" > /tmp/cached_$script_name'
                 )
                 _save_file_line(
-                    filename, "    SCRIPT_CACHED=1 /bin/bash /tmp/cached_$script_name"
+                    filename,
+                    '    SCRIPT_CACHED=1 /bin/bash /tmp/cached_$script_name "$@"',
                 )
                 _save_file_line(filename, "    exit $?")
                 _save_file_line(filename, "fi")
                 _save_file_line(filename, "")
-                os.chmod(filename, 0o0774)
+                try:
+                    os.chmod(filename, 0o0774)
+                except PermissionError:
+                    pass
 
             _ = list(executor.map(_init_cmd, cmd_files.values()))
 
             # Add sessions CSV and BASH files
             def _save_session_line(exp_session):
                 icat_investigation = exp_session.icat_investigation
                 if not icat_investigation:
```

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/sync_types.py` & `pyicat_plus-0.2.1/src/pyicat_plus/utils/sync_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,16 @@
         return self.enddate is None
 
     @property
     def started(self) -> bool:
         if not self.has_timeslot:
             return False
         now = datetime.datetime.now().astimezone()
-        return now >= self.startdate
+        startdate = self.startdate - datetime.timedelta(days=2)
+        return now >= startdate
 
     def _start_from_now(self) -> str:
         if not self.has_timeslot:
             return ""
         now = datetime.datetime.now().astimezone()
         if now >= self.startdate:
             return f"(Started {now-self.startdate} ago)"
@@ -133,15 +134,16 @@
             return f"(Will start in {self.startdate-now})"
 
     @property
     def ended(self) -> bool:
         if self.open_ended:
             return False
         now = datetime.datetime.now().astimezone()
-        return now >= self.enddate
+        enddate = self.enddate + datetime.timedelta(days=2)
+        return now >= enddate
 
     def _end_from_now(self) -> str:
         if self.open_ended:
             return ""
         now = datetime.datetime.now().astimezone()
         if now >= self.enddate:
             return f"(Ended {now-self.enddate} ago)"
@@ -203,16 +205,16 @@
         "registered",
         "invalid",
         "registered_without_files",
     )
 
     def __post_init__(self) -> None:
         self.datasets = {
-            dset_type: self.datasets.get(dset_type, list())
-            for dset_type in self.DATASET_STATUSES
+            status: self.datasets.get(status, list())
+            for status in self.DATASET_STATUSES
         }
         self.session_dir = path_utils.markdir(self.session_dir)
         self.raw_root_dir = path_utils.markdir(self.raw_root_dir)
 
     def as_dict(self) -> Dict[str, Any]:
         return dataclasses.asdict(self)
 
@@ -227,14 +229,22 @@
 
         icat_investigation = data.get("icat_investigation")
         if icat_investigation is not None:
             data["icat_investigation"] = IcatInvestigation.from_dict(icat_investigation)
 
         return cls(**data)
 
+    @classmethod
+    def allow_unsupervised_upload(cls, dataset_status: str) -> bool:
+        if dataset_status not in cls.DATASET_STATUSES:
+            raise ValueError(
+                f"'{dataset_status}' is not as valid dataset status. Valid statuses are {list(cls.DATASET_STATUSES)}"
+            )
+        return dataset_status == "registered_without_files"
+
     @property
     def in_icat_investigation(self) -> Optional[bool]:
         if self.icat_investigation is None:
             return
         if not self.icat_investigation.has_timeslot:
             return False
         inside_timeslot = self.startdate >= self.icat_investigation.startdate.date()
```

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus/utils/url.py` & `pyicat_plus-0.2.1/src/pyicat_plus/utils/url.py`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/PKG-INFO` & `pyicat_plus-0.2.1/src/pyicat_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyicat-plus
-Version: 0.2.0rc1
+Version: 0.2.1
 Summary: Python client to ICAT+
 Home-page: https://gitlab.esrf.fr/icat/pyicat-plus/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/pyicat-plus/
 Project-URL: Documentation, https://pyicat-plus.readthedocs.io/
```

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/SOURCES.txt` & `pyicat_plus-0.2.1/src/pyicat_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyicat_plus-0.2.0rc1/src/pyicat_plus.egg-info/requires.txt` & `pyicat_plus-0.2.1/src/pyicat_plus.egg-info/requires.txt`

 * *Files identical despite different names*

