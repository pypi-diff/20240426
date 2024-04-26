# Comparing `tmp/fcio-0.2.2.tar.gz` & `tmp/fcio-0.2.4.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcio-0.2.2.tar", last modified: Tue Nov 28 17:00:15 2023, max compression
+gzip compressed data, was "fcio-0.2.4.dev7.tar", last modified: Fri Apr 26 16:26:51 2024, max compression
```

## Comparing `fcio-0.2.2.tar` & `fcio-0.2.4.dev7.tar`

### file list

```diff
@@ -1,87 +1,91 @@
--rw-r--r--   0        0        0     3184 2023-11-28 16:59:06.000000 fcio-0.2.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0       51 2023-11-28 16:59:06.000000 fcio-0.2.2/.gitignore
--rw-r--r--   0        0        0      209 2023-11-28 16:59:06.000000 fcio-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0    16726 2023-11-28 16:59:06.000000 fcio-0.2.2/LICENSE
--rw-r--r--   0        0        0      628 2023-11-28 16:59:06.000000 fcio-0.2.2/Makefile
--rw-r--r--   0        0        0     1961 2023-11-28 16:59:06.000000 fcio-0.2.2/README.md
--rw-r--r--   0        0        0      638 2023-11-28 16:59:06.000000 fcio-0.2.2/docs/Makefile
--rw-r--r--   0        0        0      804 2023-11-28 16:59:06.000000 fcio-0.2.2/docs/make.bat
--rw-r--r--   0        0        0     1511 2023-11-28 16:59:06.000000 fcio-0.2.2/docs/source/conf.py
--rw-r--r--   0        0        0      238 2023-11-28 16:59:06.000000 fcio-0.2.2/docs/source/fcio.rst
--rw-r--r--   0        0        0      223 2023-11-28 16:59:06.000000 fcio-0.2.2/docs/source/index.rst
--rw-r--r--   0        0        0       45 2023-11-28 16:59:06.000000 fcio-0.2.2/docs/source/readme.rst
--rw-r--r--   0        0        0     1200 2023-11-28 16:59:06.000000 fcio-0.2.2/meson.build
--rw-r--r--   0        0        0     2095 2023-11-28 16:59:06.000000 fcio-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      668 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/__init__.py
--rw-r--r--   0        0        0       92 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cmds/__init__.py
--rw-r--r--   0        0        0     3071 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cmds/cmds.py
--rw-r--r--   0        0        0     1943 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cppyy_fcio/config.py
--rw-r--r--   0        0        0     8387 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cppyy_fcio/event.py
--rw-r--r--   0        0        0     4344 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cppyy_fcio/fcio_cppyy.py
--rw-r--r--   0        0        0     2957 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cppyy_fcio/status.py
--rw-r--r--   0        0        0     4591 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cy_fcio/cfcio.pxd
--rw-r--r--   0        0        0     9905 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cy_fcio/cy_fcio.pyx
--rw-r--r--   0        0        0     3740 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cy_fcio/cy_fcio_config.pyx
--rw-r--r--   0        0        0     6335 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cy_fcio/cy_fcio_event.pyx
--rw-r--r--   0        0        0     8088 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cy_fcio/cy_fcio_event_ext.pyx
--rw-r--r--   0        0        0     7069 2023-11-28 16:59:06.000000 fcio-0.2.2/src/fcio/cy_fcio/cy_fcio_status.pyx
--rw-r--r--   0        0        0     1272 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/.drone.star
--rw-r--r--   0        0        0       50 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/.gitignore
--rw-r--r--   0        0        0    16726 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/LICENSE
--rw-r--r--   0        0        0      408 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/Makefile
--rw-r--r--   0        0        0      427 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/README.md
--rw-r--r--   0        0        0     2365 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/examples/bufio_benchmark.c
--rw-r--r--   0        0        0      124 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/examples/meson.build
--rw-r--r--   0        0        0      523 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/meson.build
--rw-r--r--   0        0        0    44851 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/src/bufio.c
--rw-r--r--   0        0        0     3273 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/src/bufio.h
--rw-r--r--   0        0        0      161 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/src/meson.build
--rw-r--r--   0        0        0     1189 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/tests/bufio_test_follow.c
--rw-r--r--   0        0        0     1875 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/tests/bufio_test_follow_chunk.c
--rw-r--r--   0        0        0     1902 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/tests/bufio_test_lockedfile.c
--rw-r--r--   0        0        0     1331 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c
--rw-r--r--   0        0        0     1232 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c
--rw-r--r--   0        0        0     1255 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/tests/meson.build
--rw-r--r--   0        0        0      479 2023-11-28 13:24:18.000000 fcio-0.2.2/subprojects/bufio/tests/test.h
--rw-r--r--   0        0        0      110 2023-11-28 16:59:06.000000 fcio-0.2.2/subprojects/bufio.wrap
--rw-r--r--   0        0        0      965 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/.drone.star
--rw-r--r--   0        0        0       18 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/.gitignore
--rw-r--r--   0        0        0    16726 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/LICENSE
--rw-r--r--   0        0        0      375 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/Makefile
--rw-r--r--   0        0        0      715 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/README.md
--rw-r--r--   0        0        0      589 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/meson.build
--rw-r--r--   0        0        0    57331 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/src/fcio.c
--rw-r--r--   0        0        0    13863 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/src/fcio.h
--rw-r--r--   0        0        0      210 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/src/meson.build
--rw-r--r--   0        0        0     6190 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/src/time_utils.c
--rw-r--r--   0        0        0      778 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/src/time_utils.h
--rw-r--r--   0        0        0      106 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/subprojects/bufio.wrap
--rw-r--r--   0        0        0      104 2023-11-28 13:23:42.000000 fcio-0.2.2/subprojects/fcio/subprojects/tmio.wrap
--rw-r--r--   0        0        0      109 2023-11-28 16:59:06.000000 fcio-0.2.2/subprojects/fcio.wrap
--rw-r--r--   0        0        0      965 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/.drone.star
--rw-r--r--   0        0        0       44 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/.gitignore
--rw-r--r--   0        0        0    16726 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/LICENSE
--rw-r--r--   0        0        0      408 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/Makefile
--rw-r--r--   0        0        0     2650 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/README.md
--rw-r--r--   0        0        0      944 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/meson.build
--rw-r--r--   0        0        0     5929 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/timer.c
--rw-r--r--   0        0        0      637 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/timer.h
--rw-r--r--   0        0        0    10493 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark.c
--rwxr-xr-x   0        0        0      572 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark_disk_read.sh
--rwxr-xr-x   0        0        0      575 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark_disk_write.sh
--rwxr-xr-x   0        0        0      539 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark_pipe.sh
--rw-r--r--   0        0        0     2389 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark_simple.c
--rwxr-xr-x   0        0        0      926 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark_tcp.sh
--rw-r--r--   0        0        0     1620 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/tmio_example_reader.c
--rw-r--r--   0        0        0     1822 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/tmio_example_writer.c
--rw-r--r--   0        0        0     4720 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/examples/tmio_sink.c
--rw-r--r--   0        0        0      520 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/meson.build
--rw-r--r--   0        0        0      182 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/src/meson.build
--rw-r--r--   0        0        0    33908 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/src/tmio.c
--rw-r--r--   0        0        0     3723 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/src/tmio.h
--rw-r--r--   0        0        0      177 2023-11-28 14:52:33.000000 fcio-0.2.2/subprojects/tmio/subprojects/bufio.wrap
--rw-r--r--   0        0        0      108 2023-11-28 16:59:06.000000 fcio-0.2.2/subprojects/tmio.wrap
--rwxr-xr-x   0        0        0      526 2023-11-28 16:59:06.000000 fcio-0.2.2/tests/test_platform.py
--rwxr-xr-x   0        0        0      249 2023-11-28 16:59:06.000000 fcio-0.2.2/tools/create-pxd.sh
--rwxr-xr-x   0        0        0     1353 2023-11-28 16:59:06.000000 fcio-0.2.2/tools/version_util.py
--rw-r--r--   0        0        0     3296 2023-11-28 17:00:15.113301 fcio-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/.github/workflows/gh-pages-static.yml
+-rw-r--r--   0        0        0     1720 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/.github/workflows/main.yml
+-rw-r--r--   0        0        0     3178 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       51 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/.gitignore
+-rw-r--r--   0        0        0      695 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/CHANGELOG.md
+-rw-r--r--   0        0        0    16726 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/LICENSE
+-rw-r--r--   0        0        0      628 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/Makefile
+-rw-r--r--   0        0        0     1961 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/README.md
+-rw-r--r--   0        0        0      638 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/docs/Makefile
+-rw-r--r--   0        0        0      804 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/docs/make.bat
+-rw-r--r--   0        0        0       29 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/docs/requirements.txt
+-rw-r--r--   0        0        0     1729 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/docs/source/conf.py
+-rw-r--r--   0        0        0      238 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/docs/source/fcio.rst
+-rw-r--r--   0        0        0      223 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/docs/source/index.rst
+-rw-r--r--   0        0        0       45 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/docs/source/readme.rst
+-rw-r--r--   0        0        0     1200 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/meson.build
+-rw-r--r--   0        0        0     2178 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/pyproject.toml
+-rw-r--r--   0        0        0      714 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cmds/__init__.py
+-rw-r--r--   0        0        0     3071 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cmds/cmds.py
+-rw-r--r--   0        0        0     1943 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cppyy_fcio/config.py
+-rw-r--r--   0        0        0     8387 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cppyy_fcio/event.py
+-rw-r--r--   0        0        0     4344 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cppyy_fcio/fcio_cppyy.py
+-rw-r--r--   0        0        0     2957 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cppyy_fcio/status.py
+-rw-r--r--   0        0        0     4591 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cy_fcio/cfcio.pxd
+-rw-r--r--   0        0        0    10114 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cy_fcio/cy_fcio.pyx
+-rw-r--r--   0        0        0     3740 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cy_fcio/cy_fcio_config.pyx
+-rw-r--r--   0        0        0     5817 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cy_fcio/cy_fcio_event.pyx
+-rw-r--r--   0        0        0     9216 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cy_fcio/cy_fcio_event_ext.pyx
+-rw-r--r--   0        0        0     6415 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/src/fcio/cy_fcio/cy_fcio_status.pyx
+-rw-r--r--   0        0        0     1272 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/.drone.star
+-rw-r--r--   0        0        0       50 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/LICENSE
+-rw-r--r--   0        0        0      408 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/Makefile
+-rw-r--r--   0        0        0      427 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/README.md
+-rw-r--r--   0        0        0     2365 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/examples/bufio_benchmark.c
+-rw-r--r--   0        0        0      124 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/examples/meson.build
+-rw-r--r--   0        0        0      523 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/meson.build
+-rw-r--r--   0        0        0    45364 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/src/bufio.c
+-rw-r--r--   0        0        0     3273 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/src/bufio.h
+-rw-r--r--   0        0        0      161 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/src/meson.build
+-rw-r--r--   0        0        0      927 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c
+-rw-r--r--   0        0        0     1189 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_follow.c
+-rw-r--r--   0        0        0     1875 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_follow_chunk.c
+-rw-r--r--   0        0        0     1902 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_lockedfile.c
+-rw-r--r--   0        0        0      887 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_tcp_connect.c
+-rw-r--r--   0        0        0     1331 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c
+-rw-r--r--   0        0        0     1232 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c
+-rw-r--r--   0        0        0     1739 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/tests/meson.build
+-rw-r--r--   0        0        0      479 2024-02-09 15:22:16.000000 fcio-0.2.4.dev7/subprojects/bufio/tests/test.h
+-rw-r--r--   0        0        0      110 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/subprojects/bufio.wrap
+-rw-r--r--   0        0        0      965 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/.drone.star
+-rw-r--r--   0        0        0       18 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/LICENSE
+-rw-r--r--   0        0        0      375 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/Makefile
+-rw-r--r--   0        0        0      715 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/README.md
+-rw-r--r--   0        0        0      549 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/meson.build
+-rw-r--r--   0        0        0    57331 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/src/fcio.c
+-rw-r--r--   0        0        0    13863 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/src/fcio.h
+-rw-r--r--   0        0        0      199 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/src/meson.build
+-rw-r--r--   0        0        0     6190 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/src/time_utils.c
+-rw-r--r--   0        0        0      778 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/src/time_utils.h
+-rw-r--r--   0        0        0      104 2024-03-10 11:25:29.000000 fcio-0.2.4.dev7/subprojects/fcio/subprojects/tmio.wrap
+-rw-r--r--   0        0        0      109 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/subprojects/fcio.wrap
+-rw-r--r--   0        0        0      965 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/.drone.star
+-rw-r--r--   0        0        0       44 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/LICENSE
+-rw-r--r--   0        0        0      408 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/Makefile
+-rw-r--r--   0        0        0     2650 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/README.md
+-rw-r--r--   0        0        0      669 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/meson.build
+-rw-r--r--   0        0        0     5929 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/timer.c
+-rw-r--r--   0        0        0      637 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/timer.h
+-rw-r--r--   0        0        0    10493 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark.c
+-rwxr-xr-x   0        0        0      572 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark_disk_read.sh
+-rwxr-xr-x   0        0        0      575 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark_disk_write.sh
+-rwxr-xr-x   0        0        0      539 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark_pipe.sh
+-rw-r--r--   0        0        0     2389 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark_simple.c
+-rwxr-xr-x   0        0        0      926 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark_tcp.sh
+-rw-r--r--   0        0        0     1620 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_example_reader.c
+-rw-r--r--   0        0        0     1822 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_example_writer.c
+-rw-r--r--   0        0        0     4720 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_sink.c
+-rw-r--r--   0        0        0      549 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/meson.build
+-rw-r--r--   0        0        0      182 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/src/meson.build
+-rw-r--r--   0        0        0    33908 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/src/tmio.c
+-rw-r--r--   0        0        0     3723 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/src/tmio.h
+-rw-r--r--   0        0        0      106 2024-03-10 11:24:50.000000 fcio-0.2.4.dev7/subprojects/tmio/subprojects/bufio.wrap
+-rw-r--r--   0        0        0      108 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/subprojects/tmio.wrap
+-rwxr-xr-x   0        0        0      526 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/tests/test_platform.py
+-rwxr-xr-x   0        0        0      249 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/tools/create-pxd.sh
+-rwxr-xr-x   0        0        0     1374 2024-04-26 16:25:28.000000 fcio-0.2.4.dev7/tools/version_util.py
+-rw-r--r--   0        0        0     3386 2024-04-26 16:26:51.871711 fcio-0.2.4.dev7/PKG-INFO
```

### Comparing `fcio-0.2.2/LICENSE` & `fcio-0.2.4.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/Makefile` & `fcio-0.2.4.dev7/Makefile`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/README.md` & `fcio-0.2.4.dev7/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/docs/Makefile` & `fcio-0.2.4.dev7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/docs/make.bat` & `fcio-0.2.4.dev7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/meson.build` & `fcio-0.2.4.dev7/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/pyproject.toml` & `fcio-0.2.4.dev7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -32,20 +32,24 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development ",
 ]
+dependencies = [
+  "numpy"
+]
 
 [project.urls]
 Homepage = "https://github.com/FlashCam/fcio-py"
 Repository = "https://github.com/FlashCam/fcio-py.git"
 Issues = "https://github.com/FlashCam/fcio-py/issues"
 Changelog = "https://github.com/FlashCam/fcio-py/blob/main/CHANGELOG.md"
+Documentation = "https://flashcam.github.io/fcio-py/"
 
 [tool.meson-python.args]
 dist = ['--include-subprojects'] # required to include the c sources in the source distribution
 setup = [
   '-Dbuildtype=release', # already default; here to allow developers quick switching
   '-Db_ndebug=false', # default: if-release. bufio/tmio use asserts in tests.
   ]
```

### Comparing `fcio-0.2.2/src/fcio/__init__.py` & `fcio-0.2.4.dev7/src/fcio/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib.metadata
 __version__ = importlib.metadata.version("fcio")
 
 from .cy_fcio import CyFCIO as FCIO
 from .cy_fcio import CyFCIOTag as FCIOTag
+from .cy_fcio import CyFCIOLimit as FCIOLimit
 
 def fcio_open(filename : str, timeout : int = 0, buffersize : int = 0, debug : int = 0, compression : str = 'auto', extended = True) -> FCIO:
   """
   Opens an fcio data file or tcp stream and returns an FCIO object exposing the data fields as well as interaction (reading) from stream.
   All parameters are passed as is to the FCIO constructor, offering some default values.
   """
   return FCIO(filename=filename, timeout=timeout, buffersize=buffersize, debug=debug, compression=compression, extended = extended)
```

### Comparing `fcio-0.2.2/src/fcio/cmds/cmds.py` & `fcio-0.2.4.dev7/src/fcio/cmds/cmds.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/src/fcio/cppyy_fcio/config.py` & `fcio-0.2.4.dev7/src/fcio/cppyy_fcio/config.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/src/fcio/cppyy_fcio/event.py` & `fcio-0.2.4.dev7/src/fcio/cppyy_fcio/event.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/src/fcio/cppyy_fcio/fcio_cppyy.py` & `fcio-0.2.4.dev7/src/fcio/cppyy_fcio/fcio_cppyy.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/src/fcio/cppyy_fcio/status.py` & `fcio-0.2.4.dev7/src/fcio/cppyy_fcio/status.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/src/fcio/cy_fcio/cfcio.pxd` & `fcio-0.2.4.dev7/src/fcio/cy_fcio/cfcio.pxd`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/src/fcio/cy_fcio/cy_fcio.pyx` & `fcio-0.2.4.dev7/src/fcio/cy_fcio/cy_fcio.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from cfcio cimport FCIOOpen, FCIOClose, FCIODebug, FCIOGetRecord, FCIOTimeout, FCIOData, FCIOTag
+from cfcio cimport FCIOMaxChannels,FCIOMaxSamples,FCIOMaxPulses,FCIOTraceBufferLength
 cimport numpy
 import tempfile, os, subprocess
 
 include "cy_fcio_config.pyx"
 include "cy_fcio_event.pyx"
 include "cy_fcio_status.pyx"
 include "cy_fcio_event_ext.pyx"
@@ -14,14 +15,23 @@
   """
   Config = FCIOTag.FCIOConfig
   Event = FCIOTag.FCIOEvent
   Status = FCIOTag.FCIOStatus
   RecEvent = FCIOTag.FCIORecEvent
   SparseEvent = FCIOTag.FCIOSparseEvent
 
+class CyFCIOLimit:
+  """
+  A wrapper class to expose the compile time defines used in fcio.c
+  """
+  MaxChannels = FCIOMaxChannels
+  MaxSamples = FCIOMaxSamples
+  MaxPulses = FCIOMaxPulses
+  TraceBufferLength = FCIOTraceBufferLength
+
 cdef class CyFCIO:
   """
   The main class providing access to the data fields.
   Interaction mainly by using the get_record() function or CyFCIO's properties.
   
   Parameters
   ----------
@@ -235,20 +245,16 @@
         # config must always be allocated first.
         self.config = CyConfig(self)
         self.status = CyStatus(self)
         if self._extended:
           self.event = CyEventExt(self)
         else:
           self.event = CyEvent(self)
-      elif self._tag == FCIOTag.FCIOEvent or self._tag == FCIOTag.FCIOSparseEvent:
+      elif self._extended and (self._tag == FCIOTag.FCIOEvent or self._tag == FCIOTag.FCIOSparseEvent):
         self.event.update()
-      elif self._tag == FCIOTag.FCIOStatus:
-        self.status.update()
-      elif self._tag == FCIOTag.FCIORecEvent:
-        pass
       elif self._tag <= 0:
         return False
 
       return True
     else:
       raise IOError(f"File {self._filename} not opened.")
```

### Comparing `fcio-0.2.2/src/fcio/cy_fcio/cy_fcio_config.pyx` & `fcio-0.2.4.dev7/src/fcio/cy_fcio/cy_fcio_config.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/src/fcio/cy_fcio/cy_fcio_event.pyx` & `fcio-0.2.4.dev7/src/fcio/cy_fcio/cy_fcio_event.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -63,20 +63,15 @@
 
     self._np_timestamp = numpy.ndarray(shape=(10,), dtype=numpy.int32, offset=0, buffer=timestamp_memview)
     self._np_timeoffset = numpy.ndarray(shape=(10,), dtype=numpy.int32, offset=0, buffer=timeoffset_memview)
     self._np_deadregion = numpy.ndarray(shape=(10,), dtype=numpy.int32, offset=0, buffer=deadregion_memview)
     self._np_trace_list = numpy.ndarray(shape=(FCIOMaxChannels,), dtype=numpy.uint16, offset=0, buffer=trace_list_memview)
 
   cdef update(self):
-    # Call this function if a new event has been read.
-    # This updates the possible size changes
-    self._np_timestamp = numpy.lib.stride_tricks.as_strided(self._np_timestamp, shape=(self.event_ptr.timestamp_size,), writeable=False)
-    self._np_timeoffset = numpy.lib.stride_tricks.as_strided(self._np_timeoffset, shape=(self.event_ptr.timeoffset_size,), writeable=False)
-    self._np_deadregion = numpy.lib.stride_tricks.as_strided(self._np_deadregion, shape=(self.event_ptr.deadregion_size,), writeable=False)
-    self._np_trace_list = numpy.lib.stride_tricks.as_strided(self._np_trace_list, shape=(self.event_ptr.num_traces,), writeable=False)
+    pass
 
   @property
   def type(self):
     """
     the event type
     """
     return numpy.int32(self.event_ptr.type)
@@ -89,30 +84,30 @@
     return numpy.float32(self.event_ptr.pulser)
 
   @property
   def timeoffset(self):
     """
     the offset between master card pps/clock counters and the readout server unix time.
     """
-    return self._np_timeoffset
+    return self._np_timeoffset[:self.event_ptr.timeoffset_size]
 
   @property
   def deadregion(self):
     """
     the pps/clock counters while the readout system buffers are full.
     only updates when the system is 
     """
-    return self._np_deadregion
+    return self._np_deadregion[:self.event_ptr.deadregion_size]
 
   @property
   def timestamp(self):
     """
     contains event counters and pps/clock counters
     """
-    return self._np_timestamp
+    return self._np_timestamp[:self.event_ptr.timestamp_size]
 
   @property
   def num_traces(self):
     """
     the numbers of traces contain in the event.
     Incase of FCIOTag.Event tag, num_traces must be equal to the total number of mapped channels.
     """
@@ -120,15 +115,15 @@
 
   @property
   def trace_list(self):
     """
     Lookup array for the mapped channels, use with trace_buffer or trace attributes to get the
     correct waveforms.
     """
-    return self._np_trace_list
+    return self._np_trace_list[:self.event_ptr.num_traces]
 
   @property
   def timeoffset_size(self):
     """
     Size of the timeoffset array. 
     Must be equal to the shape[0] of the array.
     """
@@ -167,11 +162,11 @@
     shape is (<total number of mapped trace>,<number of samples>)
     """
     return self._np_trace
 
   @property
   def theader(self):
     """
-    2D array of the waveforms headers containing the [0]fpga baseline and [1] fpga energy.
+    2D array of the waveforms headers containing the [0]fpga baseline and [1]fpga energy.
     shape is (<total number of mapped trace>,<2>)
     """
     return self._np_theader
```

### Comparing `fcio-0.2.2/src/fcio/cy_fcio/cy_fcio_event_ext.pyx` & `fcio-0.2.4.dev7/src/fcio/cy_fcio/cy_fcio_event_ext.pyx`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cimport numpy
 import numpy
 
-# unfortunately cython does not allow multiple inheritance
-# therefor we cannot also use CyConfig as a base class
-# and must use composition here
+import sys
+
+import numbers
 
 cdef class CyEventExt(CyEvent):
   """
   Class internal to the fcio library. Do not allocate directly, must be created by using `fcio_open` or 
   FCIO.open().
   Exposes the fcio_event struct fields from the fcio.c library.
   All fields are exposes as numpy scalars or arrays with their corresponsing datatype and size.
@@ -17,71 +17,95 @@
 
   All CyEvent attributes are still available.
   """
 
   cdef numpy.ndarray _card_addresses
   cdef numpy.ndarray _card_channels
 
-  cdef numpy.int32_t _utc_unix_sec
-  cdef numpy.int32_t _utc_unix_nsec
+  
+  cdef numpy.int64_t _utc_unix_ns
   cdef numpy.float64_t _utc_unix
-
-  cdef numpy.int32_t _run_time_sec
-  cdef numpy.int32_t _run_time_nsec
+  
+  cdef numpy.int64_t _run_time_ns
   cdef numpy.float64_t _run_time
 
-  cdef int _check_max_ticks
+  cdef numpy.int32_t _wait_for_first_event
+  
+  cdef numpy.int64_t _start_time_ns
+
+  # cdef numpy.int64_t _dead_time_ns
+  # cdef numpy.int64_t _total_dead_time_ns
+
+  cdef numpy.ndarray _dead_time_ns
+  cdef numpy.ndarray _total_dead_time_ns
+
+  cdef numpy.int32_t _allowed_gps_error_ns
+
+  cdef int _current_dead_time_end_pps
+  cdef int _current_dead_time_end_ticks
 
   cdef numpy.ndarray _tracemap
 
   # def __cinit__(self):
   def __cinit__(self, fcio : CyFCIO):
 
     cdef unsigned int[:] tracemap_view = self.config_ptr.tracemap
     self._tracemap = numpy.ndarray(shape=(self.maxtraces,), dtype=numpy.uint32, offset=0, buffer=tracemap_view)
 
     self._card_addresses = self._tracemap >> 16 # upper 16bit
     self._card_channels = self._tracemap % (1 << 16) # lower 16bit
 
-    self._check_max_ticks = 1 if self.config_ptr.gps in (1,5) else 0
+    self._dead_time_ns = numpy.zeros(shape=(self.config_ptr.adcs,),dtype=numpy.int64)
+    self._total_dead_time_ns = numpy.zeros(shape=(self.config_ptr.adcs,),dtype=numpy.int64)
+
+    self._allowed_gps_error_ns = self.config_ptr.gps
+    self._wait_for_first_event = True
+    self._start_time_ns = 0
 
   cdef update(self):
-    CyEvent.update(self)
+    cdef numpy.int64_t _event_deadtime
 
-    # Check for timestamp consistency
+    if self._wait_for_first_event:
+      self._start_time_ns = self.event_ptr.deadregion[2] * 1000000000L + self.event_ptr.deadregion[3] * 4
+      self._wait_for_first_event = False
+    else:
+      # determine if we have a new dead region end and update the counters
+      if self._current_dead_time_end_pps != self.event_ptr.deadregion[2] or self._current_dead_time_end_ticks != self.event_ptr.deadregion[3]:
+        _event_deadtime = (self.event_ptr.deadregion[2]-self.event_ptr.deadregion[0]) * 1000000000L + (self.event_ptr.deadregion[3]-self.event_ptr.deadregion[1]) * 4
+        self._dead_time_ns[self.event_ptr.deadregion[5] : self.event_ptr.deadregion[5] + self.event_ptr.deadregion[6]] = _event_deadtime
+        self._total_dead_time_ns[self.event_ptr.deadregion[5] : self.event_ptr.deadregion[5] + self.event_ptr.deadregion[6]] += _event_deadtime
+      else:
+        self._dead_time_ns[:] = 0
+    
     cdef expected_max_ticks = 249999999
-    if self._check_max_ticks != 0:
-      if self.timestamp[3] != expected_max_ticks:
-        # replace with logging
-        print(f"Max Ticks field for event {self.timestamp[0]} pps {self.timestamp[1]} is not {expected_max_ticks} but {self.timestamp[3]}.")
-        # raise Exception(f"Max Ticks field for event {self.timestamp[0]} pps {self.timestamp[1]} is not {expected_max_ticks} but {self.timestamp[3]}.")
-
-    # update time information
-    self._run_time_sec = self.timestamp[1]
-    self._run_time_nsec = 4 * self.timestamp[2]
-    self._utc_unix_sec = self._run_time_sec
-    self._utc_unix_nsec = self._run_time_nsec
+    
+    cdef numpy.int64_t _current_clock_offset
+
+    _current_clock_offset = abs(self.timestamp[3] - expected_max_ticks) * 4  
+    
+    if _current_clock_offset > self._allowed_gps_error_ns:
+      print(f"WARNING fcio: max_ticks of last pps cycle {self.timestamp[3]} with { _current_clock_offset } > {self._allowed_gps_error_ns}",file=sys.stderr)
+
+    cdef numpy.int64_t nanoseconds_since_daq_reset
+    # store the current clock cycle information temporarily
+    nanoseconds_since_daq_reset = (1000000000L * self.timestamp[1] + 4 * self.timestamp[2])
+
+    # update relative time information, correct for time until the trigger was enabled in the system
+    self._run_time_ns = nanoseconds_since_daq_reset - self._start_time_ns
+    self._run_time = self._run_time_ns / 1000000000L
 
+    # update absolute time information
     if self.config_ptr.gps != 0:
-      self._utc_unix_sec += self.timeoffset[2]
+      self._utc_unix_ns = nanoseconds_since_daq_reset + self.timeoffset[2] * 1000000000L
     else:
-      self._utc_unix_sec += self.timeoffset[0]
-      self._utc_unix_nsec += 1000 * self.timeoffset[1]
-
-      while self._utc_unix_nsec >= 1000000000L:
-        self._utc_unix_sec += 1
-        self._utc_unix_nsec -= 1000000000L
+      self._utc_unix_ns = nanoseconds_since_daq_reset + 1000000000L * self.timeoffset[0] + 1000 * self.timeoffset[1]
     
-    self._utc_unix = self._utc_unix_sec + 1.0e-9 * self._utc_unix_nsec
-
-    # TODO correct for the delta t between reset of counters and actually enabling the trigger
-    self._run_time = self._run_time_sec + 1.0e-9 * self._run_time_nsec
+    self._utc_unix = self._utc_unix_ns / 1.0e-9
 
   cpdef trace_indices(self, trace_idx = None, trace_map = None, warn_unmapped = False):
-    import numbers
 
     cdef set trace_indices = set()
     cdef unsigned int tracemap_to_check
 
     # convert
     if trace_idx != None:
       if isinstance(trace_idx, numbers.Integral):
@@ -137,14 +161,28 @@
     shape is (<total number of mapped trace>,)
     Contains the fpga energy values.
     """
     if self.config_ptr.adcbits == 12: #250MHz
       return self.config_ptr.sumlength / self.config_ptr.blprecision * (self.theader[self._np_trace_list,1] - self.theader[self._np_trace_list,0])
     elif self.config_ptr.adcbits == 16: #62.5MHz
       return self.theader[self._np_trace_list,1]
+  
+  @property
+  def dead_time_ns(self):
+    """
+    The dead time since the last triggered event in nanoseconds
+    """
+    return self._dead_time_ns[self._np_trace_list]
+
+  @property
+  def total_dead_time_ns(self):
+    """
+    The total dead time since the last DAQ reset (start of run) in nanoseconds
+    """
+    return self._total_dead_time_ns[self._np_trace_list]
 
   @property
   def card_address(self):
     """
     List of corresponding MAC addresses of the FADC Card per channel.
     Display in human readable form as hex(car_address[index])
     """
@@ -179,52 +217,38 @@
     """
     The maximum time difference between fpga pps and readout server second.
     If no external clock is used, this parameter is 0.
     """
     return numpy.int32(self.config_ptr.gps)
 
   @property
-  def run_time_sec(self):
+  def run_time_ns(self):
     """
-    The number of seconds since run start.
+    The number of nanoseconds since trigger enable.
     """
-    return self._run_time_sec
-
-  @property
-  def run_time_nsec(self):
-    """
-    The number of nanoseconds since last second (run_time_sec).
-    """
-    return self._run_time_nsec
+    return self._run_time_ns
 
   @property
   def run_time(self):
     """
-    The time since run start in seconds as floating point, with decimals extracted from run_time_nsec.
+    run_time_ns in seconds as float64.
     """
     return self._run_time
 
   @property
-  def utc_unix_sec(self):
-    """
-    The number of UTC seconds since beginning of unix time (first of January 1970).
-    """
-    return self._utc_unix_sec
-
-  @property
-  def utc_unix_nsec(self):
+  def utc_unix_ns(self):
     """
-    The number of nanoseconds since last utc_unix_sec.
+    The number of nanoseconds since 1970 (UTC unix timestamps).
     """
-    return self._utc_unix_nsec
+    return self._utc_unix_ns
 
   @property
   def utc_unix(self):
     """
-    The time (UTC) since beginning of unix time (first of January 1970) as floating point.
+    utc_unix_ns in seconds as float64.
     Be aware that float64 on your machine probably doesn't allow for better than microsecond precision.
     """
     return self._utc_unix
 
   @property
   def trace(self):
     """
```

### Comparing `fcio-0.2.2/src/fcio/cy_fcio/cy_fcio_status.pyx` & `fcio-0.2.4.dev7/src/fcio/cy_fcio/cy_fcio_status.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,14 @@
     cdef int[:] environment_view = self.card_status.environment
 
     self._linkstates = numpy.ndarray(shape=(256), dtype=numpy.uint32, offset=0, buffer=linkstates_view)
     self._ctilinks = numpy.ndarray(shape=(4), dtype=numpy.uint32, offset=0, buffer=ctilinks_view)
     self._environment = numpy.ndarray(shape=(16), dtype=numpy.int32, offset=0, buffer=environment_view)
     self._othererrors = numpy.ndarray(shape=(5), dtype=numpy.uint32, offset=0, buffer=othererrors_view)
 
-  cdef update(self):
-    self._linkstates = numpy.lib.stride_tricks.as_strided(self._linkstates, shape=(self.status.data[self.index].numlinks,), writeable=False)
-    self._ctilinks = numpy.lib.stride_tricks.as_strided(self._ctilinks, shape=(self.status.data[self.index].numctilinks,), writeable=False)
-    self._environment = numpy.lib.stride_tricks.as_strided(self._environment, shape=(self.status.data[self.index].numenv,), writeable=False)
-
   @property
   def reqid(self):
     """
     Current request id.
     """
     return numpy.uint32(self.card_status.reqid)
 
@@ -148,29 +143,29 @@
     Contains information from the on-board environment sensors in the following order:
     5 temperatures in mDegree
     5 voltages in mV
     1 main current im mA
     1 humidity in o/oo
     2 temperatures in mDegree, only present if adc piggy cards are used (adc card).
     """
-    return self._environment
+    return self._environment[:self.status.data[self.index].numenv]
 
   @property
   def ctilinks(self):
     """
     Contain expert values, see fc250bcommands.h.
     """
-    return self._ctilinks
+    return self._ctilinks[:self.status.data[self.index].numctilinks]
 
   @property
   def linkstates(self):
     """
     Contain expert values, see fc250bcommands.h.
     """
-    return self._linkstates
+    return self._linkstates[:self.status.data[self.index].numlinks]
 
 cdef class CyStatus:
   """
   Class internal to the fcio library. Do not allocate directly, must be created by using `fcio_open` or 
   FCIO.open().
   Exposes the fcio_status struct fields from the fcio.c library.
   All fields are exposes as numpy scalars or arrays with their corresponsing datatype and size.
@@ -190,24 +185,14 @@
     self.num_cards = self.config.mastercards + self.config.triggercards + self.config.adccards
 
     self._data = numpy.array([CyCardStatus(self, index) for index in range(self.num_cards)], dtype=object)
 
     cdef int[:] statustime_view = self.status.statustime
     self._statustime = numpy.ndarray(shape=(10,), dtype=numpy.int32, offset=0, buffer=statustime_view)
 
-  cdef update(self):
-    if self.num_cards != self.status.cards:
-      self.num_cards = self.status.cards
-      self._data = numpy.array([CyCardStatus(self, index) for index in range(self.num_cards)], dtype=object)
-
-    cdef CyCardStatus current_card_status
-    for cs in self._data:
-      current_card_status = cs
-      current_card_status.update()
-
   @property
   def status(self):
     """
     Overall status flag of the system.
     1 : no errors
     0 : errors did occur on some card
     """
@@ -245,8 +230,8 @@
 
   @property
   def data(self):
     """
     An array of CyCardStatus objects. The type of card is ordered as master -> trigger -> adc card and their counts should be taken from the CyConfig attributes.
 
     """
-    return self._data
+    return self._data[:self.status.cards]
```

### Comparing `fcio-0.2.2/subprojects/bufio/.drone.star` & `fcio-0.2.4.dev7/subprojects/bufio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/bufio/LICENSE` & `fcio-0.2.4.dev7/subprojects/bufio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/bufio/examples/bufio_benchmark.c` & `fcio-0.2.4.dev7/subprojects/bufio/examples/bufio_benchmark.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/bufio/meson.build` & `fcio-0.2.4.dev7/subprojects/bufio/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/bufio/src/bufio.c` & `fcio-0.2.4.dev7/subprojects/bufio/src/bufio.c`

 * *Files 0% similar despite different names*

```diff
@@ -633,15 +633,15 @@
   }
 
   // Handle socket connection
   // Set default timeout to blocking
   stream->io_timeout_ms = -1;
 
   // Fill address information
-  static struct sockaddr_in address;
+  struct sockaddr_in address;
   address.sin_addr.s_addr = INADDR_ANY;
   address.sin_family = AF_INET;
   address.sin_port = htons(port);
 
   if (name[0]) {
     struct hostent *hostentry = gethostbyname(name);
     if (hostentry == 0) {
@@ -685,24 +685,33 @@
     loginetadr(info, "server waiting for connections", sa, address.sin_port);
     if (stream->type != BUFIO_LISTEN_SOCKET && accept_socket(stream, timeout, info) != 1)
       goto close_free_and_out;
   } else {
     // Handle client connection
     loginetadr(info, "connecting to", sa, address.sin_port);
 
-    struct sockaddr_in client_address;
-    socklen_t address_size = sizeof(client_address);
-
     int rc = -1;
     while (1) {
-      // TODO: Measure 'connect' time to properly decrease timeout
-      rc = connect(stream->fd, (struct sockaddr *) &address, address_size);
+      // TODO: Measure 'connect' (and 'close'/'socket') time to properly decrease timeout
+      rc = connect(stream->fd, (struct sockaddr *) &address, (socklen_t) sizeof(address));
+      // fprintf(stderr, "bufio_open: connect rc %d errno %d desc %s\n", rc, errno, strerror(errno));
       if (rc == 0 || (timeout >= 0 && timeout < 50))
         break;
 
+      if (rc == -1 && errno == ECONNREFUSED) {
+        // if the peer is not ready and refuses we try again
+        // linux would accept retrying the connect() call directly
+        // apple/bsd require closing and opening the socket again.
+        close(stream->fd);
+        if ( (stream->fd = socket(AF_INET, socket_type, 0)) == -1 ) {
+          logstring(info, "create socket failed");
+          goto free_and_out;
+        }
+        ignore_sigpipe(stream->fd);
+      }
       usleep(50000);
       timeout -= 50;
 #ifdef __APPLE__
       errno = 0;  // On OS X, usleep sets errno even on success
 #endif
     }
```

### Comparing `fcio-0.2.2/subprojects/bufio/src/bufio.h` & `fcio-0.2.4.dev7/subprojects/bufio/src/bufio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/bufio/tests/bufio_test_follow.c` & `fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_follow.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/bufio/tests/bufio_test_follow_chunk.c` & `fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_follow_chunk.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/bufio/tests/bufio_test_lockedfile.c` & `fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_lockedfile.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c` & `fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c` & `fcio-0.2.4.dev7/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/bufio/tests/meson.build` & `fcio-0.2.4.dev7/subprojects/bufio/tests/meson.build`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 bufio_test_follow_chunk = executable('bufio_test_follow_chunk', 'bufio_test_follow_chunk.c', include_directories : bufio_inc, link_with : bufio_lib)
 bufio_test_follow = executable('bufio_test_follow', 'bufio_test_follow.c', include_directories : bufio_inc, link_with : bufio_lib)
+bufio_test_tcp_connect = executable('bufio_test_tcp_connect', 'bufio_test_tcp_connect.c', include_directories : bufio_inc, link_with : bufio_lib)
+bufio_test_delayed_tcp_connect = executable('bufio_test_delayed_tcp_connect', 'bufio_test_delayed_tcp_connect.c', include_directories : bufio_inc, link_with : bufio_lib)
 bufio_test_lockedfile = executable('bufio_test_lockedfile', 'bufio_test_lockedfile.c', include_directories : bufio_inc, link_with : bufio_lib)
 bufio_test_wait_on_tcpclose_with_pending_data = executable('bufio_test_wait_on_tcpclose_with_pending_data', 'bufio_test_wait_on_tcpclose_with_pending_data.c', include_directories : bufio_inc, link_with : bufio_lib)
 bufio_test_wait_on_tcpclose = executable('bufio_test_wait_on_tcpclose', 'bufio_test_wait_on_tcpclose.c', include_directories : bufio_inc, link_with : bufio_lib)
 
 test('bufio_test_follow_chunk', bufio_test_follow_chunk, is_parallel : false)
 test('bufio_test_follow', bufio_test_follow, is_parallel : false)
+test('bufio_test_tcp_connect', bufio_test_tcp_connect, is_parallel : false)
+test('bufio_test_delayed_tcp_connect', bufio_test_delayed_tcp_connect, is_parallel : false)
 test('bufio_test_lockedfile', bufio_test_lockedfile, is_parallel : false)
 test('bufio_test_wait_on_tcpclose', bufio_test_wait_on_tcpclose, is_parallel : false, timeout : 120)
 test('bufio_test_wait_on_tcpclose_with_pending_data', bufio_test_wait_on_tcpclose_with_pending_data, is_parallel : false, timeout : 120)
```

### Comparing `fcio-0.2.2/subprojects/fcio/.drone.star` & `fcio-0.2.4.dev7/subprojects/fcio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/fcio/LICENSE` & `fcio-0.2.4.dev7/subprojects/fcio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/fcio/README.md` & `fcio-0.2.4.dev7/subprojects/fcio/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/fcio/meson.build` & `fcio-0.2.4.dev7/subprojects/tmio/meson.build`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-project('fcio', 'c',
-  version:'1.0.0',
+
+project('tmio', 'c', version:'1.0.0',
   license:'MPL-2.0',
   license_files: 'LICENSE',
-   default_options : [
+  default_options : [
     'warning_level=3',
     'c_std=c99',
     'buildtype=release',
     'default_library=both',
     'prefer_static=true',
-   ]
+  ]
 )
 
 bufio_dep = dependency('bufio', fallback : ['bufio', 'bufio_dep'])
-tmio_dep = dependency('tmio', fallback : ['tmio', 'tmio_dep'])
 
-fcio_inc= include_directories('src')
+tmio_inc = include_directories('src')
 
 subdir('src')
 
-fcio_dep = declare_dependency(include_directories : fcio_inc, link_with : fcio_lib, sources : fcio_sources)
+tmio_dep = declare_dependency(include_directories : tmio_inc, link_with : tmio_lib, dependencies : [bufio_dep])
+
+subdir('examples')
 
 pkg_mod = import('pkgconfig')
-pkg_mod.generate(fcio_lib)
+pkg_mod.generate(tmio_lib)
+
```

### Comparing `fcio-0.2.2/subprojects/fcio/src/fcio.c` & `fcio-0.2.4.dev7/subprojects/fcio/src/fcio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/fcio/src/fcio.h` & `fcio-0.2.4.dev7/subprojects/fcio/src/fcio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/fcio/src/time_utils.c` & `fcio-0.2.4.dev7/subprojects/fcio/src/time_utils.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/fcio/src/time_utils.h` & `fcio-0.2.4.dev7/subprojects/fcio/src/time_utils.h`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/.drone.star` & `fcio-0.2.4.dev7/subprojects/tmio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/LICENSE` & `fcio-0.2.4.dev7/subprojects/tmio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/README.md` & `fcio-0.2.4.dev7/subprojects/tmio/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/timer.c` & `fcio-0.2.4.dev7/subprojects/tmio/examples/timer.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/timer.h` & `fcio-0.2.4.dev7/subprojects/tmio/examples/timer.h`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark.c` & `fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark_disk_read.sh` & `fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark_disk_read.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark_disk_write.sh` & `fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark_disk_write.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark_pipe.sh` & `fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark_pipe.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark_simple.c` & `fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark_simple.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/tmio_benchmark_tcp.sh` & `fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_benchmark_tcp.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/tmio_example_reader.c` & `fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_example_reader.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/tmio_example_writer.c` & `fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_example_writer.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/examples/tmio_sink.c` & `fcio-0.2.4.dev7/subprojects/tmio/examples/tmio_sink.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/meson.build` & `fcio-0.2.4.dev7/subprojects/fcio/meson.build`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-
-project('tmio', 'c', version:'1.0.0',
+project('fcio', 'c',
+  version:'1.0.0',
   license:'MPL-2.0',
   license_files: 'LICENSE',
-  default_options : [
+   default_options : [
     'warning_level=3',
     'c_std=c99',
     'buildtype=release',
     'default_library=both',
     'prefer_static=true',
-  ]
+   ]
 )
 
-bufio_dep = dependency('bufio', fallback : ['bufio', 'bufio_dep'])
+tmio_dep = dependency('tmio', fallback : ['tmio', 'tmio_dep'])
 
-tmio_inc = include_directories('src')
+fcio_inc= include_directories('src')
 
 subdir('src')
 
-tmio_dep = declare_dependency(include_directories : tmio_inc, link_with : tmio_lib)
-subdir('examples')
+fcio_dep = declare_dependency(include_directories : fcio_inc, link_with : fcio_lib, sources : fcio_sources, dependencies : [tmio_dep])
 
 pkg_mod = import('pkgconfig')
-pkg_mod.generate(tmio_lib)
-
+pkg_mod.generate(fcio_lib)
```

### Comparing `fcio-0.2.2/subprojects/tmio/src/tmio.c` & `fcio-0.2.4.dev7/subprojects/tmio/src/tmio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/subprojects/tmio/src/tmio.h` & `fcio-0.2.4.dev7/subprojects/tmio/src/tmio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/tests/test_platform.py` & `fcio-0.2.4.dev7/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.2/tools/version_util.py` & `fcio-0.2.4.dev7/tools/version_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-import os
+
 import subprocess
    
 def run_command(cmd, cwd):
     proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, cwd=cwd)
     out = proc.communicate()[0]
     rc = proc.returncode
     return out, rc
@@ -32,9 +32,10 @@
     else:
         parts = git_describe.split('-')
         if len(parts) == 1:
             git_version = parts[0]
         elif len(parts) == 3:
             git_version = f"{parts[0]}.dev{parts[1]}"
         else:
-            raise KeyError(f"Parsed git version does not conform the expected number of dashes. Got {git_describe}, but only none or 2 dash-separated format is expected from `git describe`.")
+            print("Unkown")
+            # raise KeyError(f"Parsed git version does not conform the expected number of dashes. Got {git_describe}, but only none or 2 dash-separated format is expected from `git describe`.")
         print(git_version)
```

### Comparing `fcio-0.2.2/PKG-INFO` & `fcio-0.2.4.dev7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcio
-Version: 0.2.2
+Version: 0.2.4.dev7
 Summary: FlashCam File Format (FCIO) reader for python.
 Author-Email: Simon Sailer <simon.sailer@mpi-hd.mpg.de>
 License: MPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -21,15 +21,17 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development 
 Project-URL: Homepage, https://github.com/FlashCam/fcio-py
 Project-URL: Repository, https://github.com/FlashCam/fcio-py.git
 Project-URL: Issues, https://github.com/FlashCam/fcio-py/issues
 Project-URL: Changelog, https://github.com/FlashCam/fcio-py/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://flashcam.github.io/fcio-py/
 Requires-Python: >=3.8
+Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 # Installation
 
 Run `python3 -m pip install fcio` to install from the pypi repository.
 
 # Description
```

