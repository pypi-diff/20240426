# Comparing `tmp/emdbg-1.5.1.tar.gz` & `tmp/emdbg-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emdbg-1.5.1.tar", last modified: Mon Apr 22 13:24:58 2024, max compression
+gzip compressed data, was "emdbg-1.5.2.tar", last modified: Fri Apr 26 15:35:51 2024, max compression
```

## Comparing `emdbg-1.5.1.tar` & `emdbg-1.5.2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.535442 emdbg-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-22 13:24:49.000000 emdbg-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-22 13:24:58.535442 emdbg-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-22 13:24:49.000000 emdbg-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-22 13:24:49.000000 emdbg-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:24:58.535442 emdbg-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.507442 emdbg-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.511442 emdbg-1.5.1/src/emdbg/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.515442 emdbg-1.5.1/src/emdbg/analyze/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/analyze/backtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/analyze/callgraph.md
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/analyze/callgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/analyze/calltrace.md
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/analyze/calltrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/analyze/hardfault.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/analyze/priority.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/analyze/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.515442 emdbg-1.5.1/src/emdbg/bench/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.515442 emdbg-1.5.1/src/emdbg/bench/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/data/fmu.gdb
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/data/fmu_v5x_orbtrace.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/data/fmu_v5x_stlink.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/data/fmu_v6x.jlinkscript
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/data/fmu_v6x_orbtrace.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/data/fmu_v6x_stlink.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/fmu.md
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/fmu.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/skynode.md
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/bench/skynode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.515442 emdbg-1.5.1/src/emdbg/debug/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/crashdebug.md
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/crashdebug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.527442 emdbg-1.5.1/src/emdbg/debug/data/
--rw-r--r--   0 runner    (1001) docker     (127)  2342565 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/data/STM32F765.svd
--rw-r--r--   0 runner    (1001) docker     (127)  4154518 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/data/STM32H753.svd
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/data/cortex_m.gdb
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/data/jlink.gdb
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/data/openocd.gdb
--rw-r--r--   0 runner    (1001) docker     (127)    42517 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/data/orbuculum.gdb
--rw-r--r--   0 runner    (1001) docker     (127)    48273 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/gdb.md
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/gdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/jlink.md
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/jlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/openocd.md
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/openocd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.527442 emdbg-1.5.1/src/emdbg/debug/px4/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12206 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21076 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/perf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/system_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    16361 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/px4/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.527442 emdbg-1.5.1/src/emdbg/debug/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/remote/gdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/remote/gdb_api_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/remote/mi.py
--rw-r--r--   0 runner    (1001) docker     (127)    16823 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/remote/px4.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/remote/rpyc.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/debug/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.527442 emdbg-1.5.1/src/emdbg/io/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/io/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/io/digilent.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.531442 emdbg-1.5.1/src/emdbg/patch/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.531442 emdbg-1.5.1/src/emdbg/patch/data/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/disable_uavcan_v5x.patch
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/itm.h
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/itm_Make.defs
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/itm_nuttx_Makefile.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/malloc_return_null.patch
--rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/nuttx_tracing_itm.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/nuttx_tracing_itm_uart4.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/nuttx_tracing_itm_v10.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/nuttx_tracing_itm_v11.patch
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/sdmmc_no_inline.patch
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/sem_boostlog.c
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/semaphore_boostlog.h
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/data/semaphore_boostlog.patch
--rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/patch/set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.531442 emdbg-1.5.1/src/emdbg/power/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/power/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/power/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/power/yocto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.531442 emdbg-1.5.1/src/emdbg/serial/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/serial/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/serial/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/serial/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-22 13:24:49.000000 emdbg-1.5.1/src/emdbg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:24:58.535442 emdbg-1.5.1/src/emdbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-22 13:24:58.000000 emdbg-1.5.1/src/emdbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-22 13:24:58.000000 emdbg-1.5.1/src/emdbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:24:58.000000 emdbg-1.5.1/src/emdbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:24:58.000000 emdbg-1.5.1/src/emdbg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-22 13:24:58.000000 emdbg-1.5.1/src/emdbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 13:24:58.000000 emdbg-1.5.1/src/emdbg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.822668 emdbg-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-26 15:35:44.000000 emdbg-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-26 15:35:51.822668 emdbg-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-26 15:35:44.000000 emdbg-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-26 15:35:44.000000 emdbg-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:35:51.822668 emdbg-1.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.794668 emdbg-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.798668 emdbg-1.5.2/src/emdbg/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.802668 emdbg-1.5.2/src/emdbg/analyze/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/analyze/backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/analyze/callgraph.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/analyze/callgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/analyze/calltrace.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/analyze/calltrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/analyze/hardfault.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/analyze/priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/analyze/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.802668 emdbg-1.5.2/src/emdbg/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.802668 emdbg-1.5.2/src/emdbg/bench/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/data/fmu.gdb
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/data/fmu_v5x_orbtrace.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/data/fmu_v5x_stlink.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/data/fmu_v6x.jlinkscript
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/data/fmu_v6x_orbtrace.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/data/fmu_v6x_stlink.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/fmu.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/fmu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/skynode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/bench/skynode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.802668 emdbg-1.5.2/src/emdbg/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/crashdebug.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/crashdebug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.814668 emdbg-1.5.2/src/emdbg/debug/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  2342565 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/data/STM32F765.svd
+-rw-r--r--   0 runner    (1001) docker     (127)  4154518 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/data/STM32H753.svd
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/data/cortex_m.gdb
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/data/jlink.gdb
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/data/openocd.gdb
+-rw-r--r--   0 runner    (1001) docker     (127)    42517 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/data/orbuculum.gdb
+-rw-r--r--   0 runner    (1001) docker     (127)    48273 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/gdb.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/jlink.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/jlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/openocd.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/openocd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.814668 emdbg-1.5.2/src/emdbg/debug/px4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12206 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21076 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/system_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16361 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/px4/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.814668 emdbg-1.5.2/src/emdbg/debug/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/remote/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/remote/gdb_api_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/remote/mi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16823 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/remote/px4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/remote/rpyc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/debug/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.814668 emdbg-1.5.2/src/emdbg/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/io/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/io/digilent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.818668 emdbg-1.5.2/src/emdbg/patch/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.818668 emdbg-1.5.2/src/emdbg/patch/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/disable_uavcan_v5x.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/itm.h
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/itm_Make.defs
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/itm_nuttx_Makefile.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/malloc_return_null.patch
+-rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/nuttx_tracing_itm.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/nuttx_tracing_itm_uart4.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/nuttx_tracing_itm_v10.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/nuttx_tracing_itm_v11.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/sdmmc_no_inline.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/sem_boostlog.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/semaphore_boostlog.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/data/semaphore_boostlog.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/patch/set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.818668 emdbg-1.5.2/src/emdbg/power/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/power/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/power/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/power/yocto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.822668 emdbg-1.5.2/src/emdbg/serial/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/serial/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/serial/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/serial/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-26 15:35:44.000000 emdbg-1.5.2/src/emdbg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:35:51.822668 emdbg-1.5.2/src/emdbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-26 15:35:51.000000 emdbg-1.5.2/src/emdbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-26 15:35:51.000000 emdbg-1.5.2/src/emdbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:35:51.000000 emdbg-1.5.2/src/emdbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:35:51.000000 emdbg-1.5.2/src/emdbg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-26 15:35:51.000000 emdbg-1.5.2/src/emdbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 15:35:51.000000 emdbg-1.5.2/src/emdbg.egg-info/top_level.txt
```

### Comparing `emdbg-1.5.1/LICENSE` & `emdbg-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/PKG-INFO` & `emdbg-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emdbg
-Version: 1.5.1
+Version: 1.5.2
 Summary: Embedded Debug Tools
 Author-email: Auterion <success@auterion.com>
 License: BSD-3-Clause
 Project-URL: GitHub, https://github.com/auterion/embedded-debug-tools
 Project-URL: Changelog, https://github.com/auterion/embedded-debug-tools/blob/main/CHANGELOG.md
 Keywords: embedded,debug,gdb,stm32,px4
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `emdbg-1.5.1/README.md` & `emdbg-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/pyproject.toml` & `emdbg-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/__init__.py` & `emdbg-1.5.2/src/emdbg/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/analyze/backtrace.py` & `emdbg-1.5.2/src/emdbg/analyze/backtrace.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/analyze/callgraph.md` & `emdbg-1.5.2/src/emdbg/analyze/callgraph.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/analyze/callgraph.py` & `emdbg-1.5.2/src/emdbg/analyze/callgraph.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/analyze/calltrace.md` & `emdbg-1.5.2/src/emdbg/analyze/calltrace.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/analyze/calltrace.py` & `emdbg-1.5.2/src/emdbg/analyze/calltrace.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/analyze/hardfault.py` & `emdbg-1.5.2/src/emdbg/analyze/hardfault.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/analyze/priority.py` & `emdbg-1.5.2/src/emdbg/analyze/priority.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/bench/data/fmu.gdb` & `emdbg-1.5.2/src/emdbg/bench/data/fmu.gdb`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/bench/data/fmu_v6x.jlinkscript` & `emdbg-1.5.2/src/emdbg/bench/data/fmu_v6x.jlinkscript`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/bench/fmu.md` & `emdbg-1.5.2/src/emdbg/bench/fmu.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/bench/fmu.py` & `emdbg-1.5.2/src/emdbg/bench/fmu.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/bench/skynode.md` & `emdbg-1.5.2/src/emdbg/bench/skynode.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/bench/skynode.py` & `emdbg-1.5.2/src/emdbg/bench/skynode.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/__init__.py` & `emdbg-1.5.2/src/emdbg/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/backend.py` & `emdbg-1.5.2/src/emdbg/debug/backend.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/crashdebug.md` & `emdbg-1.5.2/src/emdbg/debug/crashdebug.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/crashdebug.py` & `emdbg-1.5.2/src/emdbg/debug/crashdebug.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/data/STM32F765.svd` & `emdbg-1.5.2/src/emdbg/debug/data/STM32F765.svd`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/data/STM32H753.svd` & `emdbg-1.5.2/src/emdbg/debug/data/STM32H753.svd`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/data/cortex_m.gdb` & `emdbg-1.5.2/src/emdbg/debug/data/cortex_m.gdb`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/data/jlink.gdb` & `emdbg-1.5.2/src/emdbg/debug/data/jlink.gdb`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/data/openocd.gdb` & `emdbg-1.5.2/src/emdbg/debug/data/openocd.gdb`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/data/orbuculum.gdb` & `emdbg-1.5.2/src/emdbg/debug/data/orbuculum.gdb`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/gdb.md` & `emdbg-1.5.2/src/emdbg/debug/gdb.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/gdb.py` & `emdbg-1.5.2/src/emdbg/debug/gdb.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/jlink.md` & `emdbg-1.5.2/src/emdbg/debug/jlink.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/jlink.py` & `emdbg-1.5.2/src/emdbg/debug/jlink.py`

 * *Files 10% similar despite different names*

```diff
@@ -141,14 +141,43 @@
             try:
                 tn.interact()
             except KeyboardInterrupt:
                 pass
     return 0
 
 # -----------------------------------------------------------------------------
+def erase(device: str, speed: int, address_range: tuple[int, int] = None,
+          serial: str = None) -> int:
+    """
+    Erases (part of) the device via JLink.
+
+    :param device: part name of the microcontroller to program. You can
+                   overwrite the default binary by exporting an alternative in
+                   your environment:
+                   ```sh
+                   export PX4_JLINK=path/to/JLinkExe
+                   ```
+    :param speed: SWD connection baudrate in kHz.
+    :param address_range: Optional [start, end] address to erase only part of device.
+    :param serial: Serial number of J-Link for selection.
+
+    :return: the process return code of JLink
+    """
+    binary = os.environ.get("PX4_JLINK", "JLinkExe")
+    if address_range is not None:
+        address_range = f"{address_range[0]} {address_range[1]}"
+    with tempfile.NamedTemporaryFile() as fcmd:
+        commands = f"Erase {address_range or ''}\nExit"
+        Path(fcmd.name).write_text(commands)
+        jcmd = f"{binary} -device {device} -speed {speed} -ExitOnError 1 " \
+               f"-if swd -autoconnect 1 -nogui 1 -commandfile {fcmd.name}"
+        if serial: jcmd += f" -SelectEmuBySN {serial}"
+        LOGGER.debug(f"{jcmd}\n{commands}")
+        return subprocess.call(jcmd, shell=True)
+
 def program(source: Path, device: str, speed: int, serial: str = None, load_addr: int = None) -> int:
     """
     Loads the source file into the microcontroller and resets the device. You can
     overwrite the default binary by exporting an alternative in your environment:
 
     ```sh
     export PX4_JLINK=path/to/JLinkExe
@@ -250,14 +279,20 @@
 
     subparsers = parser.add_subparsers(title="Command", dest="command")
 
     subparsers.add_parser("reset", help="Reset the device.")
 
     subparsers.add_parser("run", help="Run JLinkGDBServer.")
 
+    erase_parser = subparsers.add_parser("erase", help="Erase devices.")
+    erase_parser.add_argument(
+        "--range",
+        help="The range of addresses to erase as a tuple separated by comma. "
+             "For example: --range 0x0800_0000,0x0800_1000")
+
     upload_parser = subparsers.add_parser("upload", help="Upload firmware.")
     upload_parser.add_argument(
         "--source",
         required=True,
         help="The firmware to upload: `.bin`, `.hex`, or `.elf` file")
     upload_parser.add_argument(
         "--load-addr",
@@ -285,14 +320,18 @@
 
     if args.command == "reset":
         exit(reset(args.device, args.speed, args.serial))
 
     if args.command == "run":
         exit(call(args.device, args.speed, args.serial, blocking=True))
 
+    if args.command == "erase":
+        addr_range = [int(a, 0) for a in args.range.split(",")] if args.range else None
+        exit(erase(args.device, args.speed, addr_range, args.serial))
+
     if args.command == "upload":
         exit(program(os.path.abspath(args.source), args.device, args.speed, args.serial))
 
     if args.command == "rtt":
         backend = JLinkBackend(args.device, args.speed, args.serial)
         exit(rtt(backend, args.channel))
```

### Comparing `emdbg-1.5.1/src/emdbg/debug/openocd.md` & `emdbg-1.5.2/src/emdbg/debug/openocd.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/openocd.py` & `emdbg-1.5.2/src/emdbg/debug/openocd.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/__init__.py` & `emdbg-1.5.2/src/emdbg/debug/px4/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/base.py` & `emdbg-1.5.2/src/emdbg/debug/px4/base.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/buffer.py` & `emdbg-1.5.2/src/emdbg/debug/px4/buffer.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         used = head - tail if (tail <= head) else size - tail + head
         header = f"ConsoleBuffer({used}B/{size}B: "
         if tail <= head: header += f"[{tail} -> {head}]) =\n"
         else: header += f"{head}] <- [{tail}) =\n"
         if used:
             if (tail <= head):
                 # [tail, head]
-                memories = [self.read_memory(ptr + tail, used).tobytes()]
+                memories = [self.read_memory(ptr + tail, used)]
             else:
                 # head], [tail
-                memories = [self.read_memory(ptr + tail, size - tail).tobytes(),
-                            self.read_memory(ptr, head).tobytes()]
-            header += "".join(chr(v) if chr(v).isprintable() else f"\\{v:02x}"
+                memories = [self.read_memory(ptr + tail, size - tail),
+                            self.read_memory(ptr, head)]
+            header += "".join(chr(v)
                               for memory in memories
                               for v in memory.tobytes())
         return header
```

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/data.py` & `emdbg-1.5.2/src/emdbg/debug/px4/data.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/device.py` & `emdbg-1.5.2/src/emdbg/debug/px4/device.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/perf.py` & `emdbg-1.5.2/src/emdbg/debug/px4/perf.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/semaphore.py` & `emdbg-1.5.2/src/emdbg/debug/px4/semaphore.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/svd.py` & `emdbg-1.5.2/src/emdbg/debug/px4/svd.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/system_load.py` & `emdbg-1.5.2/src/emdbg/debug/px4/system_load.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/task.py` & `emdbg-1.5.2/src/emdbg/debug/px4/task.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/px4/utils.py` & `emdbg-1.5.2/src/emdbg/debug/px4/utils.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/remote/__init__.py` & `emdbg-1.5.2/src/emdbg/debug/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/remote/gdb.py` & `emdbg-1.5.2/src/emdbg/debug/remote/gdb.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/remote/gdb_api_bridge.py` & `emdbg-1.5.2/src/emdbg/debug/remote/gdb_api_bridge.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/remote/mi.py` & `emdbg-1.5.2/src/emdbg/debug/remote/mi.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/remote/px4.py` & `emdbg-1.5.2/src/emdbg/debug/remote/px4.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/remote/rpyc.py` & `emdbg-1.5.2/src/emdbg/debug/remote/rpyc.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/debug/utils.py` & `emdbg-1.5.2/src/emdbg/debug/utils.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/io/digilent.py` & `emdbg-1.5.2/src/emdbg/io/digilent.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/logger.py` & `emdbg-1.5.2/src/emdbg/logger.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/README.md` & `emdbg-1.5.2/src/emdbg/patch/README.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/__main__.py` & `emdbg-1.5.2/src/emdbg/patch/__main__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/disable_uavcan_v5x.patch` & `emdbg-1.5.2/src/emdbg/patch/data/disable_uavcan_v5x.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/itm.h` & `emdbg-1.5.2/src/emdbg/patch/data/itm.h`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/itm_nuttx_Makefile.patch` & `emdbg-1.5.2/src/emdbg/patch/data/itm_nuttx_Makefile.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/malloc_return_null.patch` & `emdbg-1.5.2/src/emdbg/patch/data/malloc_return_null.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/nuttx_tracing_itm.patch` & `emdbg-1.5.2/src/emdbg/patch/data/nuttx_tracing_itm.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/nuttx_tracing_itm_uart4.patch` & `emdbg-1.5.2/src/emdbg/patch/data/nuttx_tracing_itm_uart4.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/nuttx_tracing_itm_v10.patch` & `emdbg-1.5.2/src/emdbg/patch/data/nuttx_tracing_itm_v10.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/nuttx_tracing_itm_v11.patch` & `emdbg-1.5.2/src/emdbg/patch/data/nuttx_tracing_itm_v11.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/sdmmc_no_inline.patch` & `emdbg-1.5.2/src/emdbg/patch/data/sdmmc_no_inline.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/sem_boostlog.c` & `emdbg-1.5.2/src/emdbg/patch/data/sem_boostlog.c`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/semaphore_boostlog.h` & `emdbg-1.5.2/src/emdbg/patch/data/semaphore_boostlog.h`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/data/semaphore_boostlog.patch` & `emdbg-1.5.2/src/emdbg/patch/data/semaphore_boostlog.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/operation.py` & `emdbg-1.5.2/src/emdbg/patch/operation.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/patch/set.py` & `emdbg-1.5.2/src/emdbg/patch/set.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/power/README.md` & `emdbg-1.5.2/src/emdbg/power/README.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/power/base.py` & `emdbg-1.5.2/src/emdbg/power/base.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/power/yocto.py` & `emdbg-1.5.2/src/emdbg/power/yocto.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/serial/protocol.py` & `emdbg-1.5.2/src/emdbg/serial/protocol.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg/serial/utils.py` & `emdbg-1.5.2/src/emdbg/serial/utils.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.5.1/src/emdbg.egg-info/PKG-INFO` & `emdbg-1.5.2/src/emdbg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emdbg
-Version: 1.5.1
+Version: 1.5.2
 Summary: Embedded Debug Tools
 Author-email: Auterion <success@auterion.com>
 License: BSD-3-Clause
 Project-URL: GitHub, https://github.com/auterion/embedded-debug-tools
 Project-URL: Changelog, https://github.com/auterion/embedded-debug-tools/blob/main/CHANGELOG.md
 Keywords: embedded,debug,gdb,stm32,px4
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `emdbg-1.5.1/src/emdbg.egg-info/SOURCES.txt` & `emdbg-1.5.2/src/emdbg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

