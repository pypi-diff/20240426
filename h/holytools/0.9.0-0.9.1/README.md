# Comparing `tmp/holytools-0.9.0.tar.gz` & `tmp/holytools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holytools-0.9.0.tar", last modified: Fri Apr 26 07:36:36 2024, max compression
+gzip compressed data, was "holytools-0.9.1.tar", last modified: Fri Apr 26 08:35:02 2024, max compression
```

## Comparing `holytools-0.9.0.tar` & `holytools-0.9.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.330551 holytools-0.9.0/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1072 2024-03-11 20:42:56.000000 holytools-0.9.0/LICENSE.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      675 2024-04-26 07:36:36.326551 holytools-0.9.0/PKG-INFO
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.318551 holytools-0.9.0/holytools/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-03-17 14:55:27.000000 holytools-0.9.0/holytools/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.318551 holytools-0.9.0/holytools/abstract/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       81 2024-04-24 18:54:07.000000 holytools-0.9.0/holytools/abstract/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      704 2024-03-31 21:00:00.000000 holytools-0.9.0/holytools/abstract/enum.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.318551 holytools-0.9.0/holytools/abstract/serialization/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      139 2024-04-19 08:37:49.000000 holytools-0.9.0/holytools/abstract/serialization/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      805 2024-04-25 18:51:31.000000 holytools-0.9.0/holytools/abstract/serialization/dillable.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4388 2024-04-15 18:02:44.000000 holytools-0.9.0/holytools/abstract/serialization/jsondataclass.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      903 2024-04-25 18:51:22.000000 holytools-0.9.0/holytools/abstract/serialization/serializable.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.318551 holytools-0.9.0/holytools/abstract/tree/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       32 2024-03-24 12:59:25.000000 holytools-0.9.0/holytools/abstract/tree/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3393 2024-04-24 19:12:51.000000 holytools-0.9.0/holytools/abstract/tree/node.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.318551 holytools-0.9.0/holytools/configs/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       51 2024-04-26 05:33:16.000000 holytools-0.9.0/holytools/configs/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1851 2024-04-26 07:34:44.000000 holytools-0.9.0/holytools/configs/abstr.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2326 2024-04-26 07:01:18.000000 holytools-0.9.0/holytools/configs/impl.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.318551 holytools-0.9.0/holytools/crypto/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       42 2024-03-17 14:40:51.000000 holytools-0.9.0/holytools/crypto/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.318551 holytools-0.9.0/holytools/crypto/encrypt/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       41 2024-03-17 14:40:51.000000 holytools-0.9.0/holytools/crypto/encrypt/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2117 2024-03-17 14:40:51.000000 holytools-0.9.0/holytools/crypto/encrypt/aes.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      262 2024-03-17 14:40:51.000000 holytools-0.9.0/holytools/crypto/encrypt/algo.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2041 2024-03-17 14:40:51.000000 holytools-0.9.0/holytools/crypto/encrypt/rsa.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.318551 holytools-0.9.0/holytools/crypto/hash/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       20 2024-03-17 14:40:51.000000 holytools-0.9.0/holytools/crypto/hash/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      828 2024-03-17 14:40:51.000000 holytools-0.9.0/holytools/crypto/hash/salt.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      643 2024-03-17 14:40:51.000000 holytools-0.9.0/holytools/crypto/hash/sha.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.318551 holytools-0.9.0/holytools/devtools/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       45 2024-03-17 13:23:34.000000 holytools-0.9.0/holytools/devtools/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.318551 holytools-0.9.0/holytools/devtools/inspection/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       93 2024-03-23 08:22:37.000000 holytools-0.9.0/holytools/devtools/inspection/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2790 2024-03-26 15:44:48.000000 holytools-0.9.0/holytools/devtools/inspection/module_inspect.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1354 2024-03-17 13:37:56.000000 holytools-0.9.0/holytools/devtools/inspection/type_inspect.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.322551 holytools-0.9.0/holytools/devtools/test/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       62 2024-03-17 21:09:21.000000 holytools-0.9.0/holytools/devtools/test/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2065 2024-04-26 05:10:24.000000 holytools-0.9.0/holytools/devtools/test/cases.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      293 2024-03-17 20:52:37.000000 holytools-0.9.0/holytools/devtools/test/configurable_unit.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4783 2024-04-26 05:10:24.000000 holytools-0.9.0/holytools/devtools/test/results.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4066 2024-04-26 05:10:24.000000 holytools-0.9.0/holytools/devtools/test/unit.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.322551 holytools-0.9.0/holytools/events/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      169 2024-04-21 08:55:36.000000 holytools-0.9.0/holytools/events/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1373 2024-04-21 08:51:08.000000 holytools-0.9.0/holytools/events/countdown.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      682 2024-03-17 14:40:51.000000 holytools-0.9.0/holytools/events/input_waiter.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3133 2024-04-21 09:33:11.000000 holytools-0.9.0/holytools/events/task_scheduler.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      463 2024-04-24 18:37:04.000000 holytools-0.9.0/holytools/events/timer.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.322551 holytools-0.9.0/holytools/file/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       64 2024-03-17 13:44:51.000000 holytools-0.9.0/holytools/file/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.322551 holytools-0.9.0/holytools/file/spoof/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-03-17 21:37:28.000000 holytools-0.9.0/holytools/file/spoof/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1567 2024-04-11 01:29:21.000000 holytools-0.9.0/holytools/file/spoof/file_spoofer.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1024 2024-03-15 16:26:58.000000 holytools-0.9.0/holytools/file/spoof/spoof.bin
--rw-rw-r--   0 daniel    (1000) daniel    (1000)   171225 2024-03-15 16:26:58.000000 holytools-0.9.0/holytools/file/spoof/spoof.csv
--rw-rw-r--   0 daniel    (1000) daniel    (1000)   102796 2024-03-15 16:26:58.000000 holytools-0.9.0/holytools/file/spoof/spoof.jpg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    13264 2024-03-15 16:26:58.000000 holytools-0.9.0/holytools/file/spoof/spoof.pdf
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2670 2024-03-15 16:26:58.000000 holytools-0.9.0/holytools/file/spoof/spoof.png
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       89 2024-03-15 16:26:58.000000 holytools-0.9.0/holytools/file/spoof/spoof.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)   775192 2007-04-03 19:33:25.000000 holytools-0.9.0/holytools/file/spoof/spoof.wav
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.322551 holytools-0.9.0/holytools/file/types/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      190 2024-04-17 05:12:51.000000 holytools-0.9.0/holytools/file/types/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1252 2024-03-17 15:00:13.000000 holytools-0.9.0/holytools/file/types/binary.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2152 2024-03-27 10:11:25.000000 holytools-0.9.0/holytools/file/types/file.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4855 2024-03-17 15:07:23.000000 holytools-0.9.0/holytools/file/types/image.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      950 2024-04-11 01:29:21.000000 holytools-0.9.0/holytools/file/types/plaintext.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools/fsys/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      116 2024-03-31 21:37:04.000000 holytools-0.9.0/holytools/fsys/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5213 2024-04-26 05:10:24.000000 holytools-0.9.0/holytools/fsys/fsys_node.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1821 2024-04-24 19:29:49.000000 holytools-0.9.0/holytools/fsys/location_manager.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2516 2024-04-24 19:22:05.000000 holytools-0.9.0/holytools/fsys/resource.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1715 2024-04-25 17:55:24.000000 holytools-0.9.0/holytools/fsys/save_manager.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools/hardware/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       91 2024-03-18 19:01:40.000000 holytools-0.9.0/holytools/hardware/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools/hardware/display/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       82 2024-03-11 20:43:28.000000 holytools-0.9.0/holytools/hardware/display/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2151 2024-03-11 20:43:28.000000 holytools-0.9.0/holytools/hardware/display/display.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3953 2024-03-12 13:51:37.000000 holytools-0.9.0/holytools/hardware/display/grid_draw.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3162 2024-03-17 13:10:54.000000 holytools-0.9.0/holytools/hardware/display/types.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools/hardware/input/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       84 2024-03-11 20:43:28.000000 holytools-0.9.0/holytools/hardware/input/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3207 2024-04-26 05:10:24.000000 holytools-0.9.0/holytools/hardware/input/keyboard.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2137 2024-04-26 05:10:24.000000 holytools-0.9.0/holytools/hardware/input/mouse.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools/hardware/memory/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-03-11 20:43:28.000000 holytools-0.9.0/holytools/hardware/memory/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3265 2024-04-26 05:10:24.000000 holytools-0.9.0/holytools/hardware/memory/drives.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      827 2024-03-17 13:37:56.000000 holytools-0.9.0/holytools/hardware/memory/ram.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2260 2024-03-17 13:29:24.000000 holytools-0.9.0/holytools/hardware/memory/usage.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools/hardware/microphone/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-15 17:13:40.000000 holytools-0.9.0/holytools/hardware/microphone/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1385 2024-04-21 12:42:55.000000 holytools-0.9.0/holytools/hardware/microphone/recorder.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools/logging/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      149 2024-04-17 04:45:07.000000 holytools-0.9.0/holytools/logging/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3546 2024-04-17 04:51:03.000000 holytools-0.9.0/holytools/logging/customlogger.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1825 2024-04-26 07:26:02.000000 holytools-0.9.0/holytools/logging/interface.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      563 2024-03-17 14:40:51.000000 holytools-0.9.0/holytools/logging/log_settings.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools/network/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       87 2024-03-18 01:29:37.000000 holytools-0.9.0/holytools/network/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5058 2024-04-24 19:44:12.000000 holytools-0.9.0/holytools/network/adapter.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      969 2024-03-18 02:16:12.000000 holytools-0.9.0/holytools/network/endpoint.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2221 2024-04-26 05:10:24.000000 holytools-0.9.0/holytools/network/ip.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools/userIO/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       31 2024-03-11 20:43:29.000000 holytools-0.9.0/holytools/userIO/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4140 2024-04-26 05:10:24.000000 holytools-0.9.0/holytools/userIO/cli.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools/web/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-11 07:27:47.000000 holytools-0.9.0/holytools/web/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1293 2024-04-11 08:00:48.000000 holytools-0.9.0/holytools/web/link_soup.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2145 2024-04-06 16:52:16.000000 holytools-0.9.0/holytools/web/search_engine.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3690 2024-04-26 05:10:24.000000 holytools-0.9.0/holytools/web/site_visitor.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:36:36.326551 holytools-0.9.0/holytools.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      675 2024-04-26 07:36:36.000000 holytools-0.9.0/holytools.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2930 2024-04-26 07:36:36.000000 holytools-0.9.0/holytools.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-26 07:36:36.000000 holytools-0.9.0/holytools.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      153 2024-04-26 07:36:36.000000 holytools-0.9.0/holytools.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       10 2024-04-26 07:36:36.000000 holytools-0.9.0/holytools.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      442 2024-04-26 07:36:33.000000 holytools-0.9.0/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      152 2024-04-21 08:50:41.000000 holytools-0.9.0/requirements.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-26 07:36:36.330551 holytools-0.9.0/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.452759 holytools-0.9.1/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1072 2024-04-26 07:43:12.000000 holytools-0.9.1/LICENSE.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      676 2024-04-26 08:35:02.452759 holytools-0.9.1/PKG-INFO
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.440759 holytools-0.9.1/holytools/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.440759 holytools-0.9.1/holytools/abstract/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       81 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/abstract/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      704 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/abstract/enum.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.440759 holytools-0.9.1/holytools/abstract/serialization/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      139 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/abstract/serialization/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      805 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/abstract/serialization/dillable.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4388 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/abstract/serialization/jsondataclass.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      903 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/abstract/serialization/serializable.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.440759 holytools-0.9.1/holytools/abstract/tree/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       32 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/abstract/tree/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3393 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/abstract/tree/node.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.440759 holytools-0.9.1/holytools/configs/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       51 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/configs/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1846 2024-04-26 08:10:43.000000 holytools-0.9.1/holytools/configs/abstr.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2617 2024-04-26 08:29:00.000000 holytools-0.9.1/holytools/configs/impl.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.440759 holytools-0.9.1/holytools/crypto/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       42 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/crypto/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.444759 holytools-0.9.1/holytools/crypto/encrypt/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       41 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/crypto/encrypt/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2117 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/crypto/encrypt/aes.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      262 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/crypto/encrypt/algo.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2041 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/crypto/encrypt/rsa.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.444759 holytools-0.9.1/holytools/crypto/hash/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       20 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/crypto/hash/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      828 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/crypto/hash/salt.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      643 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/crypto/hash/sha.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.444759 holytools-0.9.1/holytools/devtools/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       45 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/devtools/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.444759 holytools-0.9.1/holytools/devtools/inspection/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       93 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/devtools/inspection/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2790 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/devtools/inspection/module_inspect.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1354 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/devtools/inspection/type_inspect.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.444759 holytools-0.9.1/holytools/devtools/test/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       62 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/devtools/test/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2065 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/devtools/test/cases.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      293 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/devtools/test/configurable_unit.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4783 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/devtools/test/results.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4066 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/devtools/test/unit.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.444759 holytools-0.9.1/holytools/events/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      169 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/events/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1373 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/events/countdown.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      682 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/events/input_waiter.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3133 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/events/task_scheduler.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      463 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/events/timer.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.444759 holytools-0.9.1/holytools/file/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       57 2024-04-26 08:19:30.000000 holytools-0.9.1/holytools/file/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.444759 holytools-0.9.1/holytools/file/mock/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/mock/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1557 2024-04-26 08:19:30.000000 holytools-0.9.1/holytools/file/mock/file_mock.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1024 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/mock/mock.bin
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)   171225 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/mock/mock.csv
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)   102796 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/mock/mock.jpg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    13264 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/mock/mock.pdf
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2670 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/mock/mock.png
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       89 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/mock/mock.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)   775192 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/mock/mock.wav
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.448759 holytools-0.9.1/holytools/file/types/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      190 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/types/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1252 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/types/binary.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2152 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/types/file.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4855 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/types/image.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      950 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/file/types/plaintext.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.448759 holytools-0.9.1/holytools/fsys/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      116 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/fsys/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5213 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/fsys/fsys_node.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1821 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/fsys/location_manager.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2516 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/fsys/resource.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1715 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/fsys/save_manager.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.448759 holytools-0.9.1/holytools/hardware/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       91 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.448759 holytools-0.9.1/holytools/hardware/display/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       82 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/display/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2151 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/display/display.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3953 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/display/grid_draw.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3162 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/display/types.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.448759 holytools-0.9.1/holytools/hardware/input/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       84 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/input/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3207 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/input/keyboard.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2137 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/input/mouse.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.448759 holytools-0.9.1/holytools/hardware/memory/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/memory/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3265 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/memory/drives.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      827 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/memory/ram.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2260 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/memory/usage.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.448759 holytools-0.9.1/holytools/hardware/microphone/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/microphone/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1385 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/hardware/microphone/recorder.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.448759 holytools-0.9.1/holytools/logging/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      149 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/logging/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3546 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/logging/customlogger.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1825 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/logging/interface.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      563 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/logging/log_settings.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.448759 holytools-0.9.1/holytools/network/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       87 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/network/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5058 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/network/adapter.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      969 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/network/endpoint.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2221 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/network/ip.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.448759 holytools-0.9.1/holytools/userIO/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       31 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/userIO/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4140 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/userIO/cli.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.452759 holytools-0.9.1/holytools/web/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/web/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1293 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/web/link_soup.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2145 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/web/search_engine.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3690 2024-04-26 07:43:12.000000 holytools-0.9.1/holytools/web/site_visitor.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 08:35:02.452759 holytools-0.9.1/holytools.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      676 2024-04-26 08:35:02.000000 holytools-0.9.1/holytools.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2911 2024-04-26 08:35:02.000000 holytools-0.9.1/holytools.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-26 08:35:02.000000 holytools-0.9.1/holytools.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      153 2024-04-26 08:35:02.000000 holytools-0.9.1/holytools.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       10 2024-04-26 08:35:02.000000 holytools-0.9.1/holytools.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      442 2024-04-26 08:33:24.000000 holytools-0.9.1/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      152 2024-04-26 07:43:12.000000 holytools-0.9.1/requirements.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-26 08:35:02.452759 holytools-0.9.1/setup.cfg
```

### Comparing `holytools-0.9.0/LICENSE.txt` & `holytools-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/PKG-INFO` & `holytools-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: holytools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Collection of general python utilities for future projects
 Author-email: Daniel Hollarek <daniel.hollarek@googlemail.com>
-Project-URL: repository, https://github.com/Somerandomguy10111/hollarek
+Project-URL: repository, https://github.com/Somerandomguy10111/holytools
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: func_timeout
 Requires-Dist: selenium
 Requires-Dist: pathvalidate
 Requires-Dist: psutil
 Requires-Dist: pympler
```

### Comparing `holytools-0.9.0/holytools/abstract/enum.py` & `holytools-0.9.1/holytools/abstract/enum.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/abstract/serialization/dillable.py` & `holytools-0.9.1/holytools/abstract/serialization/dillable.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/abstract/serialization/jsondataclass.py` & `holytools-0.9.1/holytools/abstract/serialization/jsondataclass.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/abstract/serialization/serializable.py` & `holytools-0.9.1/holytools/abstract/serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/abstract/tree/node.py` & `holytools-0.9.1/holytools/abstract/tree/node.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/configs/abstr.py` & `holytools-0.9.1/holytools/configs/abstr.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from holytools.logging import Loggable, LogLevel
 
 DictType = TypeVar(name='DictType', bound=dict)
 ConfigValue = Union[str, int, bool, float]
 
 # ---------------------------------------------------------
 
-class Configs(ABC, Loggable):
+class Configs(Loggable):
     def __init__(self, *args, **kwargs):
         super().__init__()
         self._map : DictType = self._retrieve_map()
 
     @abstractmethod
     def _retrieve_map(self) -> DictType:
         pass
```

### Comparing `holytools-0.9.0/holytools/configs/impl.py` & `holytools-0.9.1/holytools/configs/impl.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 import subprocess
 from typing import Optional
 from holytools.logging import LogLevel
 from holytools.configs.abstr import Configs, DictType
 
 # ---------------------------------------------------------
 
+
 class FileConfigs(Configs):
-    def __init__(self, config_fpath : str = os.path.expanduser('~/.pyconfig')):
-        self._config_fpath: str = config_fpath
+    def __init__(self, config_fpath : str = '~/.pyconfig'):
+        self._config_fpath: str = as_absolute(path=config_fpath)
+        config_dirpath = os.path.dirname(self._config_fpath)
+        os.makedirs(config_dirpath, exist_ok=True)
         super().__init__()
-        # self.log(f'Initialized {self.__class__.__name__} with \"{self._config_fpath}\"')
 
     def _retrieve_map(self) -> ConfigObj:
+        self.log(f'Initialized {self.__class__.__name__} with config file at \"{self._config_fpath}\"')
         return ConfigObj(self._config_fpath)
 
     def update_config_resouce(self, key : str, value : str):
         self._map.write()
 
 
 class PassConfigs(Configs):
-    def __init__(self, pass_dirpath : str):
-        self._pass_dirpath: str = pass_dirpath
+    def __init__(self, pass_dirpath : str = '~/.password-store' ):
+        self._pass_dirpath: str = as_absolute(path=pass_dirpath)
         os.environ['PASSWORD_STORE_DIR'] = pass_dirpath
         super().__init__()
 
     def update_config_resouce(self, key : str, value : str):
         insert_command = f"echo \"{value}\" | pass insert --echo {key}"
         self.try_run_cmd(cmd=insert_command)
 
@@ -52,14 +55,18 @@
 
     def get_keys(self) -> list[str]:
         filenames = os.listdir(path=self._pass_dirpath)
         keys = [os.path.splitext(f)[0] for f in filenames if f.endswith('.gpg')]
         return keys
 
 
+def as_absolute(path : str) -> str:
+    path = os.path.expanduser(path=path)
+    path = os.path.abspath(path)
+    return path
 
 
 if __name__ == "__main__":
     pass_config = PassConfigs(pass_dirpath='/home/daniel/Drive/.password-store')
     pypi_key = pass_config.get(key='pypi')
     # pass_config.set(key='this', value='that')
     print(pypi_key)
```

### Comparing `holytools-0.9.0/holytools/crypto/encrypt/aes.py` & `holytools-0.9.1/holytools/crypto/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/crypto/encrypt/rsa.py` & `holytools-0.9.1/holytools/crypto/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/crypto/hash/salt.py` & `holytools-0.9.1/holytools/crypto/hash/salt.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/crypto/hash/sha.py` & `holytools-0.9.1/holytools/crypto/hash/sha.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/devtools/inspection/module_inspect.py` & `holytools-0.9.1/holytools/devtools/inspection/module_inspect.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/devtools/inspection/type_inspect.py` & `holytools-0.9.1/holytools/devtools/inspection/type_inspect.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/devtools/test/cases.py` & `holytools-0.9.1/holytools/devtools/test/cases.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/devtools/test/results.py` & `holytools-0.9.1/holytools/devtools/test/results.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/devtools/test/unit.py` & `holytools-0.9.1/holytools/devtools/test/unit.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/events/countdown.py` & `holytools-0.9.1/holytools/events/countdown.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/events/input_waiter.py` & `holytools-0.9.1/holytools/events/input_waiter.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/events/task_scheduler.py` & `holytools-0.9.1/holytools/events/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/file/spoof/file_spoofer.py` & `holytools-0.9.1/holytools/file/mock/file_mock.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,45 +12,45 @@
     temp_fd, temp_filepath = tempfile.mkstemp(suffix=os.path.splitext(filename)[1], dir='/tmp')
     os.close(temp_fd)
     shutil.copy2(original_file_path, temp_filepath)
 
     return temp_filepath
 
 
-class FileSpoofer:
+class FileMock:
     @staticmethod
     def lend_png() -> ImageFile:
-        fpath = create_temp_copy('spoof.png')
+        fpath = create_temp_copy('mock.png')
         return ImageFile(fpath=fpath)
 
     @staticmethod
     def lend_jpg() -> ImageFile:
-        fpath = create_temp_copy('spoof.jpg')
+        fpath = create_temp_copy('mock.jpg')
         return ImageFile(fpath=fpath)
 
     @staticmethod
     def lend_pdf() -> PlaintextFile:
-        fpath = create_temp_copy('spoof.pdf')
+        fpath = create_temp_copy('mock.pdf')
         return PlaintextFile(fpath=fpath)
 
     @staticmethod
     def lend_txt() -> PlaintextFile:
-        fpath = create_temp_copy('spoof.txt')
+        fpath = create_temp_copy('mock.txt')
         return PlaintextFile(fpath=fpath)
 
     @staticmethod
     def lend_csv() -> PlaintextFile:
-        fpath = create_temp_copy('spoof.csv')
+        fpath = create_temp_copy('mock.csv')
         return PlaintextFile(fpath=fpath)
 
     @staticmethod
     def lend_bin() -> BinaryFile:
-        fpath = create_temp_copy('spoof.bin')
+        fpath = create_temp_copy('mock.bin')
         return BinaryFile(fpath=fpath)
 
     @staticmethod
     def lend_wav() -> BinaryFile:
-        fpath = create_temp_copy('spoof.wav')
+        fpath = create_temp_copy('mock.wav')
         return BinaryFile(fpath=fpath)
 
 if __name__ == "__main__":
     print(os.path.abspath(__file__))
```

### Comparing `holytools-0.9.0/holytools/file/spoof/spoof.csv` & `holytools-0.9.1/holytools/file/mock/mock.csv`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/file/spoof/spoof.jpg` & `holytools-0.9.1/holytools/file/mock/mock.jpg`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/file/spoof/spoof.pdf` & `holytools-0.9.1/holytools/file/mock/mock.pdf`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/file/spoof/spoof.png` & `holytools-0.9.1/holytools/file/mock/mock.png`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/file/spoof/spoof.wav` & `holytools-0.9.1/holytools/file/mock/mock.wav`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/file/types/binary.py` & `holytools-0.9.1/holytools/file/types/binary.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/file/types/file.py` & `holytools-0.9.1/holytools/file/types/file.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/file/types/image.py` & `holytools-0.9.1/holytools/file/types/image.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/file/types/plaintext.py` & `holytools-0.9.1/holytools/file/types/plaintext.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/fsys/fsys_node.py` & `holytools-0.9.1/holytools/fsys/fsys_node.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/fsys/location_manager.py` & `holytools-0.9.1/holytools/fsys/location_manager.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/fsys/resource.py` & `holytools-0.9.1/holytools/fsys/resource.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/fsys/save_manager.py` & `holytools-0.9.1/holytools/fsys/save_manager.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/hardware/display/display.py` & `holytools-0.9.1/holytools/hardware/display/display.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/hardware/display/grid_draw.py` & `holytools-0.9.1/holytools/hardware/display/grid_draw.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/hardware/display/types.py` & `holytools-0.9.1/holytools/hardware/display/types.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/hardware/input/keyboard.py` & `holytools-0.9.1/holytools/hardware/input/keyboard.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/hardware/input/mouse.py` & `holytools-0.9.1/holytools/hardware/input/mouse.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/hardware/memory/drives.py` & `holytools-0.9.1/holytools/hardware/memory/drives.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/hardware/memory/ram.py` & `holytools-0.9.1/holytools/hardware/memory/ram.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/hardware/memory/usage.py` & `holytools-0.9.1/holytools/hardware/memory/usage.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/hardware/microphone/recorder.py` & `holytools-0.9.1/holytools/hardware/microphone/recorder.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/logging/customlogger.py` & `holytools-0.9.1/holytools/logging/customlogger.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/logging/interface.py` & `holytools-0.9.1/holytools/logging/interface.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/logging/log_settings.py` & `holytools-0.9.1/holytools/logging/log_settings.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/network/adapter.py` & `holytools-0.9.1/holytools/network/adapter.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/network/endpoint.py` & `holytools-0.9.1/holytools/network/endpoint.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/network/ip.py` & `holytools-0.9.1/holytools/network/ip.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/userIO/cli.py` & `holytools-0.9.1/holytools/userIO/cli.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/web/link_soup.py` & `holytools-0.9.1/holytools/web/link_soup.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/web/search_engine.py` & `holytools-0.9.1/holytools/web/search_engine.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools/web/site_visitor.py` & `holytools-0.9.1/holytools/web/site_visitor.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.0/holytools.egg-info/PKG-INFO` & `holytools-0.9.1/holytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: holytools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Collection of general python utilities for future projects
 Author-email: Daniel Hollarek <daniel.hollarek@googlemail.com>
-Project-URL: repository, https://github.com/Somerandomguy10111/hollarek
+Project-URL: repository, https://github.com/Somerandomguy10111/holytools
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: func_timeout
 Requires-Dist: selenium
 Requires-Dist: pathvalidate
 Requires-Dist: psutil
 Requires-Dist: pympler
```

### Comparing `holytools-0.9.0/holytools.egg-info/SOURCES.txt` & `holytools-0.9.1/holytools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 holytools/devtools/test/unit.py
 holytools/events/__init__.py
 holytools/events/countdown.py
 holytools/events/input_waiter.py
 holytools/events/task_scheduler.py
 holytools/events/timer.py
 holytools/file/__init__.py
-holytools/file/spoof/__init__.py
-holytools/file/spoof/file_spoofer.py
-holytools/file/spoof/spoof.bin
-holytools/file/spoof/spoof.csv
-holytools/file/spoof/spoof.jpg
-holytools/file/spoof/spoof.pdf
-holytools/file/spoof/spoof.png
-holytools/file/spoof/spoof.txt
-holytools/file/spoof/spoof.wav
+holytools/file/mock/__init__.py
+holytools/file/mock/file_mock.py
+holytools/file/mock/mock.bin
+holytools/file/mock/mock.csv
+holytools/file/mock/mock.jpg
+holytools/file/mock/mock.pdf
+holytools/file/mock/mock.png
+holytools/file/mock/mock.txt
+holytools/file/mock/mock.wav
 holytools/file/types/__init__.py
 holytools/file/types/binary.py
 holytools/file/types/file.py
 holytools/file/types/image.py
 holytools/file/types/plaintext.py
 holytools/fsys/__init__.py
 holytools/fsys/fsys_node.py
```

