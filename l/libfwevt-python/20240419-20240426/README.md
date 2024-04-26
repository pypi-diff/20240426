# Comparing `tmp/libfwevt-python-20240419.tar.gz` & `tmp/libfwevt-python-20240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwevt-python-20240419.tar", last modified: Sun Apr 21 10:42:11 2024, max compression
+gzip compressed data, was "libfwevt-python-20240426.tar", last modified: Fri Apr 26 17:19:22 2024, max compression
```

## Comparing `libfwevt-python-20240419.tar` & `libfwevt-python-20240426.tar`

### file list

```diff
@@ -1,651 +1,656 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-19 04:00:11.000000 libfwevt-20240419/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-21 10:11:46.000000 libfwevt-20240419/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-19 04:00:11.000000 libfwevt-20240419/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-21 10:11:47.000000 libfwevt-20240419/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26023 2024-04-21 10:11:47.000000 libfwevt-20240419/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 10:11:32.000000 libfwevt-20240419/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-11 04:37:20.000000 libfwevt-20240419/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-21 10:11:42.000000 libfwevt-20240419/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-21 10:11:41.000000 libfwevt-20240419/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-21 10:11:41.000000 libfwevt-20240419/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-21 10:11:42.000000 libfwevt-20240419/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-21 10:11:41.000000 libfwevt-20240419/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-19 04:00:15.000000 libfwevt-20240419/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-16 16:00:57.000000 libfwevt-20240419/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:11.000000 libfwevt-20240419/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-11 04:37:20.000000 libfwevt-20240419/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29416 2024-04-19 04:00:13.000000 libfwevt-20240419/include/libfwevt.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      402 2024-04-19 04:00:11.000000 libfwevt-20240419/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/include/libfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5124 2024-04-19 04:46:36.000000 libfwevt-20240419/include/libfwevt/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5122 2024-04-21 10:12:02.000000 libfwevt-20240419/include/libfwevt/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5439 2024-04-19 04:00:13.000000 libfwevt-20240419/include/libfwevt/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5308 2024-04-21 10:12:02.000000 libfwevt-20240419/include/libfwevt/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-19 04:01:00.000000 libfwevt-20240419/include/libfwevt/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-04-19 04:00:13.000000 libfwevt-20240419/include/libfwevt/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-19 04:00:13.000000 libfwevt-20240419/include/libfwevt/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-21 10:12:02.000000 libfwevt-20240419/include/libfwevt/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29416 2024-04-21 10:12:02.000000 libfwevt-20240419/include/libfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24376 2024-04-21 10:11:47.000000 libfwevt-20240419/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-19 04:00:13.000000 libfwevt-20240419/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-19 04:00:13.000000 libfwevt-20240419/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-19 04:00:13.000000 libfwevt-20240419/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-19 04:00:13.000000 libfwevt-20240419/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-19 04:00:13.000000 libfwevt-20240419/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-19 04:00:13.000000 libfwevt-20240419/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-19 04:00:13.000000 libfwevt-20240419/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-19 04:00:11.000000 libfwevt-20240419/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-19 04:00:13.000000 libfwevt-20240419/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-04-21 10:12:02.000000 libfwevt-20240419/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11564 2024-04-21 10:11:46.000000 libfwevt-20240419/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12255 2024-04-19 05:59:01.000000 libfwevt-20240419/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-19 04:00:13.000000 libfwevt-20240419/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-19 04:00:13.000000 libfwevt-20240419/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-19 04:00:13.000000 libfwevt-20240419/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21433 2024-04-21 10:11:47.000000 libfwevt-20240419/common/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1667 2024-04-16 16:38:33.000000 libfwevt-20240419/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:08:57.000000 libfwevt-20240419/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-21 10:11:46.000000 libfwevt-20240419/config.guess
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2539 2024-04-19 04:00:11.000000 libfwevt-20240419/libfwevt.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-04-19 04:00:15.000000 libfwevt-20240419/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/libfwevt-dev.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      709 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-04-21 10:12:02.000000 libfwevt-20240419/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/libfwevt-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-19 04:00:11.000000 libfwevt-20240419/dpkg/libfwevt.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-04-21 10:12:02.000000 libfwevt-20240419/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-19 04:00:11.000000 libfwevt-20240419/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1610631 2024-04-21 10:11:45.000000 libfwevt-20240419/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-21 10:11:46.000000 libfwevt-20240419/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-21 10:11:46.000000 libfwevt-20240419/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_level.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16103 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_channel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2024-04-21 10:12:02.000000 libfwevt-20240419/libfwevt/libfwevt.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7898 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_provider.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1845 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   169078 2024-04-19 05:49:03.000000 libfwevt-20240419/libfwevt/libfwevt_xml_document.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9032 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_tag.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19153 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_manifest.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12233 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_event.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_task.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_task.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21455 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_template_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2478 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_manifest.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-16 16:37:54.000000 libfwevt-20240419/libfwevt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5790 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_map.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    99778 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_provider.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1095 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_template_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5677 2024-04-19 04:46:23.000000 libfwevt-20240419/libfwevt/libfwevt_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9600 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_document.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8479 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_opcode.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2719 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_channel.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4562 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_template.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2755 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5675 2024-04-21 10:12:02.000000 libfwevt-20240419/libfwevt/libfwevt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2717 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_event.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8583 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_keyword.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_map.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3740 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_template_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   151450 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_tag.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8346 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_level.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_token.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9575 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/fwevt_template.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_opcode.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5976 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_token.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33751 2024-04-21 10:11:47.000000 libfwevt-20240419/libfwevt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_keyword.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12331 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10922 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_xml_template_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38484 2024-04-19 04:00:14.000000 libfwevt-20240419/libfwevt/libfwevt_template.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/pyfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12785 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_template.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9264 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_tasks.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5543 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_level.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2631 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_template_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_providers.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_providers.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52868 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_provider.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_map.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_maps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2391 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_tasks.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1358 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2433 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_opcodes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_channels.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_event.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5702 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_opcode.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-04-16 16:37:34.000000 libfwevt-20240419/pyfwevt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9236 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_levels.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2438 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_template.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2021 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_channel.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9390 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_opcodes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_keywords.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9206 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_maps.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_level.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1313 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_events.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9328 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_events.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11485 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6236 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_provider.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_keywords.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14294 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_manifest.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_keyword.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5566 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_task.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_map.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14900 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_template_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_templates.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_keyword.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1716 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_task.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2580 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_template_items.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1758 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_opcode.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_levels.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9780 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_template_items.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66258 2024-04-21 10:11:47.000000 libfwevt-20240419/pyfwevt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2506 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_manifest.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1175 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9783 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_channel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11339 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_event.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_templates.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2024-04-19 04:01:00.000000 libfwevt-20240419/pyfwevt/pyfwevt_channels.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2862 2024-04-19 04:00:14.000000 libfwevt-20240419/pyfwevt/pyfwevt_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-19 04:00:15.000000 libfwevt-20240419/pyfwevt/pyfwevt_libfwevt.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_level/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_level/fwevt_test_level.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_tag/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5568 2024-04-19 04:00:48.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_provider/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_template_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5436 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_document/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5503 2024-04-19 04:00:48.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1296 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_event/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_event/fwevt_test_event.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8947 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libfwevt/libfwevt.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21121 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libfwevt.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/pyfwevt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8862 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/pyfwevt/pyfwevt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_template/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_template/fwevt_test_template.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_keyword/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_opcode/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_manifest/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_template_item/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5421 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_template_item/fwevt_test_template_item.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_channel/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5151 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_error/fwevt_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_task/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5394 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_task/fwevt_test_task.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5238 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_notify/fwevt_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_token/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19719 2024-04-21 10:11:47.000000 libfwevt-20240419/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_map/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_map/fwevt_test_map.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/msvscpp/fwevt_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5157 2024-04-19 04:00:28.000000 libfwevt-20240419/msvscpp/fwevt_test_support/fwevt_test_support.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-04-19 04:00:13.000000 libfwevt-20240419/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      308 2024-04-19 04:00:11.000000 libfwevt-20240419/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-21 10:11:46.000000 libfwevt-20240419/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29377 2024-04-21 10:11:47.000000 libfwevt-20240419/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-21 10:11:26.000000 libfwevt-20240419/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-19 04:00:11.000000 libfwevt-20240419/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      536 2024-04-19 04:00:11.000000 libfwevt-20240419/libfwevt.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-04-19 04:00:11.000000 libfwevt-20240419/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-21 10:11:46.000000 libfwevt-20240419/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-19 04:00:11.000000 libfwevt-20240419/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      759 2024-04-19 04:01:00.000000 libfwevt-20240419/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:08:57.000000 libfwevt-20240419/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29816 2024-04-21 10:11:47.000000 libfwevt-20240419/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-21 10:11:30.000000 libfwevt-20240419/libcthreads/libcthreads_queue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2019 2024-04-21 10:12:02.000000 libfwevt-20240419/libfwevt.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-21 10:11:47.000000 libfwevt-20240419/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      408 2023-12-31 13:44:14.000000 libfwevt-20240419/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14490 2024-04-19 04:00:15.000000 libfwevt-20240419/manuals/libfwevt.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       99 2024-04-16 16:37:12.000000 libfwevt-20240419/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21632 2024-04-21 10:11:47.000000 libfwevt-20240419/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/pyfwevt_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71222 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_xml_tag.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11439 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_keyword.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7762 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_template_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12655 2024-04-19 04:01:21.000000 libfwevt-20240419/tests/pyfwevt_test_provider.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10018 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_map.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20604 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_xml_template_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5947 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11335 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_channel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15846 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_event.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9238 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_xml_token.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7299 2024-04-19 04:01:21.000000 libfwevt-20240419/tests/pyfwevt_test_event.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11188 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_level.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4425 2024-04-19 04:01:51.000000 libfwevt-20240419/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   422118 2024-04-19 04:45:38.000000 libfwevt-20240419/tests/fwevt_test_xml_document.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20972 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_manifest.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6010 2024-04-19 04:01:21.000000 libfwevt-20240419/tests/pyfwevt_test_manifest.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_libfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    89615 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_provider.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2074 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11198 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_opcode.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11384 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_task.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57856 2024-04-21 10:11:47.000000 libfwevt-20240419/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23465 2024-04-19 04:00:48.000000 libfwevt-20240419/tests/fwevt_test_template.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2024-04-19 04:00:15.000000 libfwevt-20240419/tests/fwevt_test_libfvalue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4151 2024-04-19 04:01:37.000000 libfwevt-20240419/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2024-04-19 04:00:14.000000 libfwevt-20240419/ossfuzz/xml_document_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2024-04-19 04:00:14.000000 libfwevt-20240419/ossfuzz/manifest_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      866 2024-04-16 16:36:54.000000 libfwevt-20240419/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-04-19 04:00:14.000000 libfwevt-20240419/ossfuzz/ossfuzz_libfwevt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29382 2024-04-21 10:11:47.000000 libfwevt-20240419/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-21 10:11:41.000000 libfwevt-20240419/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:10.000000 libfwevt-20240419/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:11.000000 libfwevt-20240419/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:11.000000 libfwevt-20240419/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:12.000000 libfwevt-20240419/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:12.000000 libfwevt-20240419/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:11.000000 libfwevt-20240419/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:12.000000 libfwevt-20240419/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:12.000000 libfwevt-20240419/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:12.000000 libfwevt-20240419/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:11.000000 libfwevt-20240419/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-04-21 10:12:02.000000 libfwevt-20240419/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:12.000000 libfwevt-20240419/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:11.000000 libfwevt-20240419/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53143 2024-04-21 10:11:47.000000 libfwevt-20240419/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-21 10:11:36.000000 libfwevt-20240419/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36939 2024-04-21 10:11:47.000000 libfwevt-20240419/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-21 10:11:33.000000 libfwevt-20240419/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32452 2024-04-21 10:11:47.000000 libfwevt-20240419/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-21 10:11:34.000000 libfwevt-20240419/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26500 2024-04-21 10:11:47.000000 libfwevt-20240419/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-21 10:11:28.000000 libfwevt-20240419/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:08.000000 libfwevt-20240419/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-21 10:11:27.000000 libfwevt-20240419/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25967 2024-04-21 10:11:47.000000 libfwevt-20240419/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-21 10:42:09.000000 libfwevt-20240419/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29551 2024-04-21 10:11:47.000000 libfwevt-20240419/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-21 10:11:31.000000 libfwevt-20240419/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56622 2024-04-21 10:11:44.000000 libfwevt-20240419/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5368 2024-04-19 04:00:11.000000 libfwevt-20240419/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-04-21 10:42:11.440078 libfwevt-20240419/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-26 03:46:20.000000 libfwevt-20240426/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-26 17:04:53.000000 libfwevt-20240426/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 03:46:20.000000 libfwevt-20240426/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-26 17:04:53.000000 libfwevt-20240426/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:20.000000 libfwevt-20240426/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26023 2024-04-26 17:04:53.000000 libfwevt-20240426/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-26 17:04:38.000000 libfwevt-20240426/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:18.000000 libfwevt-20240426/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-16 16:00:57.000000 libfwevt-20240426/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-16 16:00:57.000000 libfwevt-20240426/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-16 16:00:57.000000 libfwevt-20240426/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-11 04:37:20.000000 libfwevt-20240426/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-16 16:00:57.000000 libfwevt-20240426/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-26 17:04:48.000000 libfwevt-20240426/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-26 17:04:48.000000 libfwevt-20240426/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-26 17:04:47.000000 libfwevt-20240426/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-16 16:00:57.000000 libfwevt-20240426/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-16 16:00:57.000000 libfwevt-20240426/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-16 16:00:57.000000 libfwevt-20240426/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-26 17:04:48.000000 libfwevt-20240426/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-26 17:04:47.000000 libfwevt-20240426/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-19 04:00:15.000000 libfwevt-20240426/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-16 16:00:57.000000 libfwevt-20240426/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:11.000000 libfwevt-20240426/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-11 04:37:20.000000 libfwevt-20240426/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:18.000000 libfwevt-20240426/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32854 2024-04-26 04:32:56.000000 libfwevt-20240426/include/libfwevt.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      402 2024-04-26 03:46:20.000000 libfwevt-20240426/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:18.000000 libfwevt-20240426/include/libfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5124 2024-04-26 03:46:22.000000 libfwevt-20240426/include/libfwevt/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5122 2024-04-26 17:05:07.000000 libfwevt-20240426/include/libfwevt/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5478 2024-04-26 03:46:22.000000 libfwevt-20240426/include/libfwevt/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5347 2024-04-26 17:05:07.000000 libfwevt-20240426/include/libfwevt/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-26 03:47:49.000000 libfwevt-20240426/include/libfwevt/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-04-26 03:46:22.000000 libfwevt-20240426/include/libfwevt/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-26 03:46:22.000000 libfwevt-20240426/include/libfwevt/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-26 17:05:07.000000 libfwevt-20240426/include/libfwevt/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32854 2024-04-26 17:05:07.000000 libfwevt-20240426/include/libfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24376 2024-04-26 17:04:53.000000 libfwevt-20240426/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:18.000000 libfwevt-20240426/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-26 03:46:21.000000 libfwevt-20240426/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-26 03:46:21.000000 libfwevt-20240426/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-26 03:46:21.000000 libfwevt-20240426/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-26 03:46:21.000000 libfwevt-20240426/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-26 03:46:21.000000 libfwevt-20240426/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-26 03:46:21.000000 libfwevt-20240426/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-26 03:46:21.000000 libfwevt-20240426/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-26 03:46:20.000000 libfwevt-20240426/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-26 03:46:21.000000 libfwevt-20240426/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-04-26 17:05:07.000000 libfwevt-20240426/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11564 2024-04-26 17:04:52.000000 libfwevt-20240426/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12255 2024-04-26 17:05:07.000000 libfwevt-20240426/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-26 03:46:21.000000 libfwevt-20240426/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-26 03:46:21.000000 libfwevt-20240426/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-26 03:46:21.000000 libfwevt-20240426/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21433 2024-04-26 17:04:53.000000 libfwevt-20240426/common/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1667 2024-04-16 16:38:33.000000 libfwevt-20240426/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:08:57.000000 libfwevt-20240426/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-26 17:04:53.000000 libfwevt-20240426/config.guess
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2539 2024-04-26 03:46:20.000000 libfwevt-20240426/libfwevt.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:18.000000 libfwevt-20240426/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-04-26 03:46:24.000000 libfwevt-20240426/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-26 03:46:20.000000 libfwevt-20240426/dpkg/libfwevt-dev.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:18.000000 libfwevt-20240426/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-26 03:46:20.000000 libfwevt-20240426/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-26 03:46:20.000000 libfwevt-20240426/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      709 2024-04-26 03:46:20.000000 libfwevt-20240426/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-04-26 03:46:20.000000 libfwevt-20240426/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-04-26 17:05:07.000000 libfwevt-20240426/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-26 03:46:20.000000 libfwevt-20240426/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-26 03:46:20.000000 libfwevt-20240426/dpkg/libfwevt-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-26 03:46:20.000000 libfwevt-20240426/dpkg/libfwevt.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-04-26 17:05:07.000000 libfwevt-20240426/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-26 03:46:20.000000 libfwevt-20240426/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1610631 2024-04-26 17:04:51.000000 libfwevt-20240426/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-26 17:04:53.000000 libfwevt-20240426/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-26 17:04:53.000000 libfwevt-20240426/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:20.000000 libfwevt-20240426/libfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_level.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16103 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_channel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2024-04-26 17:05:07.000000 libfwevt-20240426/libfwevt/libfwevt.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7898 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_provider.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1873 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   169452 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_xml_document.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27691 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_xml_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5444 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_xml_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9259 2024-04-26 04:14:50.000000 libfwevt-20240426/libfwevt/libfwevt_xml_tag.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19153 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_manifest.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12233 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_event.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_task.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_task.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21455 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_template_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2478 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_manifest.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2122 2024-04-24 04:21:39.000000 libfwevt-20240426/libfwevt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5790 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_map.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    99778 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_provider.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1095 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_xml_template_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5677 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9600 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_xml_document.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8479 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_opcode.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2719 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_channel.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4562 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_template.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2854 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5675 2024-04-26 17:05:07.000000 libfwevt-20240426/libfwevt/libfwevt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2717 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_event.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8583 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_keyword.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_map.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3740 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_template_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   153739 2024-04-26 04:15:00.000000 libfwevt-20240426/libfwevt/libfwevt_xml_tag.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8346 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_level.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_xml_token.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9575 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/fwevt_template.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_opcode.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5976 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_xml_token.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34049 2024-04-26 17:04:53.000000 libfwevt-20240426/libfwevt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_keyword.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12345 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10922 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_xml_template_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38484 2024-04-26 03:46:22.000000 libfwevt-20240426/libfwevt/libfwevt_template.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/pyfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12785 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_template.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9264 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_tasks.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5543 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_level.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2631 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_template_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_providers.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_providers.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52868 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_provider.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_map.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_maps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2391 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_tasks.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1358 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2433 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_opcodes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_channels.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_event.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5702 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_opcode.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-04-16 16:37:34.000000 libfwevt-20240426/pyfwevt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9236 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_levels.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2438 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_template.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2021 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_channel.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9390 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_opcodes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_keywords.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9206 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_maps.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_level.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1313 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_events.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9328 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_events.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11485 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6236 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_provider.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2454 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_keywords.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14294 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_manifest.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_keyword.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5566 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_task.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_map.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14900 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_template_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2475 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_templates.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_keyword.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1716 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_task.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2580 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_template_items.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1758 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_opcode.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2412 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_levels.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9780 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_template_items.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66258 2024-04-26 17:04:53.000000 libfwevt-20240426/pyfwevt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2506 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_manifest.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1175 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9783 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_channel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11339 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_event.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_templates.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9450 2024-04-26 03:47:07.000000 libfwevt-20240426/pyfwevt/pyfwevt_channels.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2862 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-26 03:46:23.000000 libfwevt-20240426/pyfwevt/pyfwevt_libfwevt.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_level/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_level/fwevt_test_level.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_xml_tag/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5568 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_provider/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_xml_template_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5436 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_xml_document/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5503 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_event/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_event/fwevt_test_event.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/libfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9117 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/libfwevt/libfwevt.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21865 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/libfwevt.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/pyfwevt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8862 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/pyfwevt/pyfwevt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_template/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_template/fwevt_test_template.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_keyword/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_opcode/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_manifest/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_xml_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5574 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_xml_value/fwevt_test_xml_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_template_item/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5421 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_template_item/fwevt_test_template_item.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_channel/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5151 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_error/fwevt_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_task/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5394 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_task/fwevt_test_task.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5238 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_notify/fwevt_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_xml_token/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19771 2024-04-26 17:04:53.000000 libfwevt-20240426/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_map/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_map/fwevt_test_map.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/msvscpp/fwevt_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5157 2024-04-26 03:52:14.000000 libfwevt-20240426/msvscpp/fwevt_test_support/fwevt_test_support.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-04-26 03:46:21.000000 libfwevt-20240426/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      308 2024-04-26 03:46:20.000000 libfwevt-20240426/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-26 17:04:53.000000 libfwevt-20240426/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:19.000000 libfwevt-20240426/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29377 2024-04-26 17:04:53.000000 libfwevt-20240426/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-26 17:04:32.000000 libfwevt-20240426/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-26 03:46:20.000000 libfwevt-20240426/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      536 2024-04-26 03:46:20.000000 libfwevt-20240426/libfwevt.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-04-26 03:46:20.000000 libfwevt-20240426/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-26 17:04:53.000000 libfwevt-20240426/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-26 03:46:20.000000 libfwevt-20240426/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      759 2024-04-26 03:47:49.000000 libfwevt-20240426/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:08:57.000000 libfwevt-20240426/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:19.000000 libfwevt-20240426/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29816 2024-04-26 17:04:53.000000 libfwevt-20240426/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-26 17:04:36.000000 libfwevt-20240426/libcthreads/libcthreads_queue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2019 2024-04-26 17:05:07.000000 libfwevt-20240426/libfwevt.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-26 17:04:53.000000 libfwevt-20240426/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-04-26 17:04:26.000000 libfwevt-20240426/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15518 2024-04-26 04:33:28.000000 libfwevt-20240426/manuals/libfwevt.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       99 2024-04-16 16:37:12.000000 libfwevt-20240426/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21632 2024-04-26 17:04:53.000000 libfwevt-20240426/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/pyfwevt_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73331 2024-04-26 04:23:37.000000 libfwevt-20240426/tests/fwevt_test_xml_tag.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11439 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_keyword.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7762 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_template_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12655 2024-04-26 03:47:49.000000 libfwevt-20240426/tests/pyfwevt_test_provider.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10018 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_map.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20604 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_xml_template_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6297 2024-04-26 03:51:34.000000 libfwevt-20240426/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11335 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_channel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15846 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_event.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9238 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_xml_token.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7299 2024-04-26 03:47:49.000000 libfwevt-20240426/tests/pyfwevt_test_event.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11188 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_level.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-26 03:46:23.000000 libfwevt-20240426/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4425 2024-04-26 03:47:54.000000 libfwevt-20240426/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   422096 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_xml_document.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20972 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_manifest.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6010 2024-04-26 03:47:49.000000 libfwevt-20240426/tests/pyfwevt_test_manifest.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_libfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13479 2024-04-26 04:10:40.000000 libfwevt-20240426/tests/fwevt_test_xml_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    89615 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_provider.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2074 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11198 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_opcode.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11384 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_task.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59010 2024-04-26 17:04:53.000000 libfwevt-20240426/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23465 2024-04-26 03:46:51.000000 libfwevt-20240426/tests/fwevt_test_template.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2024-04-26 03:46:24.000000 libfwevt-20240426/tests/fwevt_test_libfvalue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4161 2024-04-26 03:51:51.000000 libfwevt-20240426/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2024-04-26 03:46:22.000000 libfwevt-20240426/ossfuzz/xml_document_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2024-04-26 03:46:22.000000 libfwevt-20240426/ossfuzz/manifest_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      866 2024-04-16 16:36:54.000000 libfwevt-20240426/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-04-26 03:46:22.000000 libfwevt-20240426/ossfuzz/ossfuzz_libfwevt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29382 2024-04-26 17:04:53.000000 libfwevt-20240426/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-26 17:04:47.000000 libfwevt-20240426/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:21.000000 libfwevt-20240426/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:11.000000 libfwevt-20240426/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:11.000000 libfwevt-20240426/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:12.000000 libfwevt-20240426/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:12.000000 libfwevt-20240426/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:11.000000 libfwevt-20240426/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:12.000000 libfwevt-20240426/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:12.000000 libfwevt-20240426/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:12.000000 libfwevt-20240426/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:11.000000 libfwevt-20240426/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-04-26 17:05:07.000000 libfwevt-20240426/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:12.000000 libfwevt-20240426/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:11.000000 libfwevt-20240426/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:20.000000 libfwevt-20240426/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53143 2024-04-26 17:04:53.000000 libfwevt-20240426/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-26 17:04:43.000000 libfwevt-20240426/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36939 2024-04-26 17:04:53.000000 libfwevt-20240426/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:20.000000 libfwevt-20240426/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32452 2024-04-26 17:04:53.000000 libfwevt-20240426/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-26 17:04:40.000000 libfwevt-20240426/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:19.000000 libfwevt-20240426/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26500 2024-04-26 17:04:53.000000 libfwevt-20240426/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-26 17:04:34.000000 libfwevt-20240426/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:19.000000 libfwevt-20240426/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-26 17:04:33.000000 libfwevt-20240426/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25967 2024-04-26 17:04:53.000000 libfwevt-20240426/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 17:19:20.000000 libfwevt-20240426/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29551 2024-04-26 17:04:53.000000 libfwevt-20240426/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-26 17:04:37.000000 libfwevt-20240426/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56622 2024-04-26 17:04:50.000000 libfwevt-20240426/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5368 2024-04-26 03:46:20.000000 libfwevt-20240426/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-04-26 17:19:22.649715 libfwevt-20240426/PKG-INFO
```

### Comparing `libfwevt-20240419/COPYING` & `libfwevt-20240426/COPYING`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/install-sh` & `libfwevt-20240426/install-sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/depcomp` & `libfwevt-20240426/depcomp`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_error.c` & `libfwevt-20240426/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_support.h` & `libfwevt-20240426/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_identifier.h` & `libfwevt-20240426/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_libcerror.h` & `libfwevt-20240426/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/Makefile.am` & `libfwevt-20240426/libfguid/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_unused.h` & `libfwevt-20240426/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_extern.h` & `libfwevt-20240426/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_types.h` & `libfwevt-20240426/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_identifier.c` & `libfwevt-20240426/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_support.c` & `libfwevt-20240426/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_definitions.h` & `libfwevt-20240426/libfguid/libfguid_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/Makefile.in` & `libfwevt-20240426/libfguid/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfguid/libfguid_error.h` & `libfwevt-20240426/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/libfdatetime.m4` & `libfwevt-20240426/m4/libfdatetime.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/tests.m4` & `libfwevt-20240426/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/lib-prefix.m4` & `libfwevt-20240426/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/progtest.m4` & `libfwevt-20240426/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/libuna.m4` & `libfwevt-20240426/m4/libuna.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/gettext.m4` & `libfwevt-20240426/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/lib-ld.m4` & `libfwevt-20240426/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/libcdata.m4` & `libfwevt-20240426/m4/libcdata.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/common.m4` & `libfwevt-20240426/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/libcthreads.m4` & `libfwevt-20240426/m4/libcthreads.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/ltversion.m4` & `libfwevt-20240426/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/ltsugar.m4` & `libfwevt-20240426/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/host-cpu-c-abi.m4` & `libfwevt-20240426/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/libtool.m4` & `libfwevt-20240426/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/po.m4` & `libfwevt-20240426/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/libcerror.m4` & `libfwevt-20240426/m4/libcerror.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/libcnotify.m4` & `libfwevt-20240426/m4/libcnotify.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/libfguid.m4` & `libfwevt-20240426/m4/libfguid.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/intlmacosx.m4` & `libfwevt-20240426/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/lt~obsolete.m4` & `libfwevt-20240426/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/lib-link.m4` & `libfwevt-20240426/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/iconv.m4` & `libfwevt-20240426/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/ltoptions.m4` & `libfwevt-20240426/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/nls.m4` & `libfwevt-20240426/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/python.m4` & `libfwevt-20240426/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/libfvalue.m4` & `libfwevt-20240426/m4/libfvalue.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/types.m4` & `libfwevt-20240426/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/m4/pthread.m4` & `libfwevt-20240426/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/include/libfwevt.h.in` & `libfwevt-20240426/include/libfwevt.h.in`

 * *Files 4% similar despite different names*

```diff
@@ -854,14 +854,22 @@
 
 #endif /* #if defined( HAVE_DEBUG_OUTPUT ) */
 
 /* -------------------------------------------------------------------------
  * XML tag functions
  * ------------------------------------------------------------------------- */
 
+/* Frees a XML tag
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_tag_free(
+     libfwevt_xml_tag_t **xml_tag,
+     libfwevt_error_t **error );
+
 /* Retrieves the size of the UTF-8 formatted name
  * Returns 1 if successful or -1 on error
  */
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf8_name_size(
      libfwevt_xml_tag_t *xml_tag,
      size_t *utf8_string_size,
@@ -892,45 +900,58 @@
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf16_name(
      libfwevt_xml_tag_t *xml_tag,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libfwevt_error_t **error );
 
+/* Retrieves the XML value
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_tag_get_value(
+     libfwevt_xml_tag_t *xml_tag,
+     libfwevt_xml_value_t **xml_value,
+     libfwevt_error_t **error );
+
 /* Retrieves the size of the UTF-8 formatted value
  * Returns 1 if successful or -1 on error
  */
+LIBFWEVT_DEPRECATED \
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf8_value_size(
      libfwevt_xml_tag_t *xml_tag,
      size_t *utf8_string_size,
      libfwevt_error_t **error );
 
 /* Retrieves the UTF-8 formatted value
  * Returns 1 if successful or -1 on error
  */
+LIBFWEVT_DEPRECATED \
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf8_value(
      libfwevt_xml_tag_t *xml_tag,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libfwevt_error_t **error );
 
 /* Retrieves the size of the UTF-16 formatted value
  * Returns 1 if successful or -1 on error
  */
+LIBFWEVT_DEPRECATED \
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf16_value_size(
      libfwevt_xml_tag_t *xml_tag,
      size_t *utf16_string_size,
      libfwevt_error_t **error );
 
 /* Retrieves the UTF-16 formatted value
  * Returns 1 if successful or -1 on error
  */
+LIBFWEVT_DEPRECATED \
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf16_value(
      libfwevt_xml_tag_t *xml_tag,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libfwevt_error_t **error );
 
@@ -1021,13 +1042,109 @@
  */
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_flags(
      libfwevt_xml_tag_t *xml_tag,
      uint8_t *flags,
      libfwevt_error_t **error );
 
+/* -------------------------------------------------------------------------
+ * XML value functions
+ * ------------------------------------------------------------------------- */
+
+/* Frees a XML value
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_free(
+     libfwevt_xml_value_t **xml_value,
+     libfwevt_error_t **error );
+
+/* Retrieves the data size
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_get_data_size(
+     libfwevt_xml_value_t *xml_value,
+     size_t *data_size,
+     libfwevt_error_t **error );
+
+/* Copies the data
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_data(
+     libfwevt_xml_value_t *xml_value,
+     uint8_t *data,
+     size_t data_size,
+     libfwevt_error_t **error );
+
+/* Copies the value data to an 8-bit value
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_to_8bit(
+     libfwevt_xml_value_t *xml_value,
+     uint8_t *value_8bit,
+     libfwevt_error_t **error );
+
+/* Copies the value data to an 32-bit value
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_to_32bit(
+     libfwevt_xml_value_t *xml_value,
+     uint32_t *value_32bit,
+     libfwevt_error_t **error );
+
+/* Copies the value data to an 64-bit value
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_to_64bit(
+     libfwevt_xml_value_t *xml_value,
+     uint64_t *value_64bit,
+     libfwevt_error_t **error );
+
+/* Retrieves the size of an UTF-8 encoded string of the value data
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_get_utf8_string_size(
+     libfwevt_xml_value_t *xml_value,
+     size_t *utf8_string_size,
+     libfwevt_error_t **error );
+
+/* Copies the value data to an UTF-8 encoded string
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_to_utf8_string(
+     libfwevt_xml_value_t *xml_value,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libfwevt_error_t **error );
+
+/* Retrieves the size of an UTF-16 encoded string of the value data
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_get_utf16_string_size(
+     libfwevt_xml_value_t *xml_value,
+     size_t *utf16_string_size,
+     libfwevt_error_t **error );
+
+/* Copies the value data to an UTF-16 encoded string
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_to_utf16_string(
+     libfwevt_xml_value_t *xml_value,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libfwevt_error_t **error );
+
 #if defined( __cplusplus )
 }
 #endif
 
 #endif /* !defined( _LIBFWEVT_H ) */
```

### Comparing `libfwevt-20240419/include/libfwevt/definitions.h.in` & `libfwevt-20240426/include/libfwevt/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/include/libfwevt/definitions.h` & `libfwevt-20240426/include/libfwevt/definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFWEVT_DEFINITIONS_H )
 #define _LIBFWEVT_DEFINITIONS_H
 
 #include <libfwevt/types.h>
 
-#define LIBFWEVT_VERSION						20240419
+#define LIBFWEVT_VERSION						20240426
 
 /* The version string
  */
-#define LIBFWEVT_VERSION_STRING						"20240419"
+#define LIBFWEVT_VERSION_STRING						"20240426"
 
 /* The byte order definitions
  */
 enum LIBFWEVT_ENDIAN
 {
 	LIBFWEVT_ENDIAN_BIG						= (int) 'b',
 	LIBFWEVT_ENDIAN_LITTLE						= (int) 'l'
```

### Comparing `libfwevt-20240419/include/libfwevt/types.h.in` & `libfwevt-20240426/include/libfwevt/types.h.in`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,15 @@
 typedef intptr_t libfwevt_provider_t;
 typedef intptr_t libfwevt_task_t;
 typedef intptr_t libfwevt_template_t;
 typedef intptr_t libfwevt_template_item_t;
 typedef intptr_t libfwevt_xml_document_t;
 typedef intptr_t libfwevt_xml_tag_t;
 typedef intptr_t libfwevt_xml_template_value_t;
+typedef intptr_t libfwevt_xml_value_t;
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* !defined( _LIBFWEVT_TYPES_H ) */
```

### Comparing `libfwevt-20240419/include/libfwevt/types.h` & `libfwevt-20240426/include/libfwevt/types.h`

 * *Files 0% similar despite different names*

```diff
@@ -211,14 +211,15 @@
 typedef intptr_t libfwevt_provider_t;
 typedef intptr_t libfwevt_task_t;
 typedef intptr_t libfwevt_template_t;
 typedef intptr_t libfwevt_template_item_t;
 typedef intptr_t libfwevt_xml_document_t;
 typedef intptr_t libfwevt_xml_tag_t;
 typedef intptr_t libfwevt_xml_template_value_t;
+typedef intptr_t libfwevt_xml_value_t;
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* !defined( _LIBFWEVT_TYPES_H ) */
```

### Comparing `libfwevt-20240419/include/libfwevt/features.h.in` & `libfwevt-20240426/include/libfwevt/features.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/include/libfwevt/error.h` & `libfwevt-20240426/include/libfwevt/error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/include/libfwevt/extern.h` & `libfwevt-20240426/include/libfwevt/extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/include/libfwevt/features.h` & `libfwevt-20240426/include/libfwevt/features.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/include/libfwevt.h` & `libfwevt-20240426/include/libfwevt.h`

 * *Files 4% similar despite different names*

```diff
@@ -854,14 +854,22 @@
 
 #endif /* #if defined( HAVE_DEBUG_OUTPUT ) */
 
 /* -------------------------------------------------------------------------
  * XML tag functions
  * ------------------------------------------------------------------------- */
 
+/* Frees a XML tag
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_tag_free(
+     libfwevt_xml_tag_t **xml_tag,
+     libfwevt_error_t **error );
+
 /* Retrieves the size of the UTF-8 formatted name
  * Returns 1 if successful or -1 on error
  */
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf8_name_size(
      libfwevt_xml_tag_t *xml_tag,
      size_t *utf8_string_size,
@@ -892,45 +900,58 @@
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf16_name(
      libfwevt_xml_tag_t *xml_tag,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libfwevt_error_t **error );
 
+/* Retrieves the XML value
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_tag_get_value(
+     libfwevt_xml_tag_t *xml_tag,
+     libfwevt_xml_value_t **xml_value,
+     libfwevt_error_t **error );
+
 /* Retrieves the size of the UTF-8 formatted value
  * Returns 1 if successful or -1 on error
  */
+LIBFWEVT_DEPRECATED \
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf8_value_size(
      libfwevt_xml_tag_t *xml_tag,
      size_t *utf8_string_size,
      libfwevt_error_t **error );
 
 /* Retrieves the UTF-8 formatted value
  * Returns 1 if successful or -1 on error
  */
+LIBFWEVT_DEPRECATED \
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf8_value(
      libfwevt_xml_tag_t *xml_tag,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libfwevt_error_t **error );
 
 /* Retrieves the size of the UTF-16 formatted value
  * Returns 1 if successful or -1 on error
  */
+LIBFWEVT_DEPRECATED \
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf16_value_size(
      libfwevt_xml_tag_t *xml_tag,
      size_t *utf16_string_size,
      libfwevt_error_t **error );
 
 /* Retrieves the UTF-16 formatted value
  * Returns 1 if successful or -1 on error
  */
+LIBFWEVT_DEPRECATED \
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf16_value(
      libfwevt_xml_tag_t *xml_tag,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libfwevt_error_t **error );
 
@@ -1021,13 +1042,109 @@
  */
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_flags(
      libfwevt_xml_tag_t *xml_tag,
      uint8_t *flags,
      libfwevt_error_t **error );
 
+/* -------------------------------------------------------------------------
+ * XML value functions
+ * ------------------------------------------------------------------------- */
+
+/* Frees a XML value
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_free(
+     libfwevt_xml_value_t **xml_value,
+     libfwevt_error_t **error );
+
+/* Retrieves the data size
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_get_data_size(
+     libfwevt_xml_value_t *xml_value,
+     size_t *data_size,
+     libfwevt_error_t **error );
+
+/* Copies the data
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_data(
+     libfwevt_xml_value_t *xml_value,
+     uint8_t *data,
+     size_t data_size,
+     libfwevt_error_t **error );
+
+/* Copies the value data to an 8-bit value
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_to_8bit(
+     libfwevt_xml_value_t *xml_value,
+     uint8_t *value_8bit,
+     libfwevt_error_t **error );
+
+/* Copies the value data to an 32-bit value
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_to_32bit(
+     libfwevt_xml_value_t *xml_value,
+     uint32_t *value_32bit,
+     libfwevt_error_t **error );
+
+/* Copies the value data to an 64-bit value
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_to_64bit(
+     libfwevt_xml_value_t *xml_value,
+     uint64_t *value_64bit,
+     libfwevt_error_t **error );
+
+/* Retrieves the size of an UTF-8 encoded string of the value data
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_get_utf8_string_size(
+     libfwevt_xml_value_t *xml_value,
+     size_t *utf8_string_size,
+     libfwevt_error_t **error );
+
+/* Copies the value data to an UTF-8 encoded string
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_to_utf8_string(
+     libfwevt_xml_value_t *xml_value,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libfwevt_error_t **error );
+
+/* Retrieves the size of an UTF-16 encoded string of the value data
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_get_utf16_string_size(
+     libfwevt_xml_value_t *xml_value,
+     size_t *utf16_string_size,
+     libfwevt_error_t **error );
+
+/* Copies the value data to an UTF-16 encoded string
+ * Returns 1 if successful, 0 if size value not be retrieved or -1 on error
+ */
+LIBFWEVT_EXTERN \
+int libfwevt_xml_value_copy_to_utf16_string(
+     libfwevt_xml_value_t *xml_value,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libfwevt_error_t **error );
+
 #if defined( __cplusplus )
 }
 #endif
 
 #endif /* !defined( _LIBFWEVT_H ) */
```

### Comparing `libfwevt-20240419/include/Makefile.in` & `libfwevt-20240426/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/config_borlandc.h` & `libfwevt-20240426/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/file_stream.h` & `libfwevt-20240426/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/memory.h` & `libfwevt-20240426/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/byte_stream.h` & `libfwevt-20240426/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/common.h` & `libfwevt-20240426/common/common.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/config_winapi.h` & `libfwevt-20240426/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/system_string.h` & `libfwevt-20240426/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/types.h.in` & `libfwevt-20240426/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/types.h` & `libfwevt-20240426/common/types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/config.h.in` & `libfwevt-20240426/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/config.h` & `libfwevt-20240426/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -364,24 +364,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfwevt"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfwevt 20240419"
+#define PACKAGE_STRING "libfwevt 20240426"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfwevt"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240419"
+#define PACKAGE_VERSION "20240426"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -399,15 +399,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240419"
+#define VERSION "20240426"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfwevt-20240419/common/wide_string.h` & `libfwevt-20240426/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/narrow_string.h` & `libfwevt-20240426/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/config_msc.h` & `libfwevt-20240426/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/common/Makefile.in` & `libfwevt-20240426/common/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/Makefile.am` & `libfwevt-20240426/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/config.guess` & `libfwevt-20240426/config.guess`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt.spec.in` & `libfwevt-20240426/libfwevt.spec.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/dpkg/copyright` & `libfwevt-20240426/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/dpkg/control` & `libfwevt-20240426/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/dpkg/rules` & `libfwevt-20240426/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/COPYING.LESSER` & `libfwevt-20240426/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/configure` & `libfwevt-20240426/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfwevt 20240419.
+# Generated by GNU Autoconf 2.71 for libfwevt 20240426.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libfwevt'
 PACKAGE_TARNAME='libfwevt'
-PACKAGE_VERSION='20240419'
-PACKAGE_STRING='libfwevt 20240419'
+PACKAGE_VERSION='20240426'
+PACKAGE_STRING='libfwevt 20240426'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfwevt.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1552,15 +1552,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfwevt 20240419 to adapt to many kinds of systems.
+\`configure' configures libfwevt 20240426 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1623,15 +1623,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfwevt 20240419:";;
+     short | recursive ) echo "Configuration of libfwevt 20240426:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1822,15 +1822,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfwevt configure 20240419
+libfwevt configure 20240426
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2543,15 +2543,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfwevt $as_me 20240419, which was
+It was created by libfwevt $as_me 20240426, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4032,15 +4032,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfwevt'
- VERSION='20240419'
+ VERSION='20240426'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -48640,15 +48640,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfwevt $as_me 20240419, which was
+This file was extended by libfwevt $as_me 20240426, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -48708,15 +48708,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfwevt config.status 20240419
+libfwevt config.status 20240426
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfwevt-20240419/compile` & `libfwevt-20240426/compile`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/missing` & `libfwevt-20240426/missing`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_level.h` & `libfwevt-20240426/libfwevt/libfwevt_level.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_channel.c` & `libfwevt-20240426/libfwevt/libfwevt_channel.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt.rc` & `libfwevt-20240426/libfwevt/libfwevt.rc`

 * *Files 11% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support the Windows XML Event Log (EVTX) data types\0"
-      VALUE "FileVersion",		"20240419" "\0"
+      VALUE "FileVersion",		"20240426" "\0"
       VALUE "InternalName",		"libfwevt.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfwevt.dll\0"
       VALUE "ProductName",		"libfwevt\0"
-      VALUE "ProductVersion",		"20240419" "\0"
+      VALUE "ProductVersion",		"20240426" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfwevt/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfwevt-20240419/libfwevt/libfwevt_provider.h` & `libfwevt-20240426/libfwevt/libfwevt_provider.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_debug.h` & `libfwevt-20240426/libfwevt/libfwevt_debug.h`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 #if !defined( _LIBFWEVT_DEBUG_H )
 #define _LIBFWEVT_DEBUG_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libfwevt_libcerror.h"
+#include "libfwevt_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 #if defined( HAVE_DEBUG_OUTPUT )
```

### Comparing `libfwevt-20240419/libfwevt/libfwevt_xml_document.c` & `libfwevt-20240426/libfwevt/libfwevt_xml_document.c`

 * *Files 0% similar despite different names*

```diff
@@ -137,16 +137,16 @@
 	if( *xml_document != NULL )
 	{
 		internal_xml_document = (libfwevt_internal_xml_document_t *) *xml_document;
 		*xml_document         = NULL;
 
 		if( internal_xml_document->root_xml_tag != NULL )
 		{
-			if( libfwevt_xml_tag_free(
-			     &( internal_xml_document->root_xml_tag ),
+			if( libfwevt_internal_xml_tag_free(
+			     (libfwevt_internal_xml_tag_t **) &( internal_xml_document->root_xml_tag ),
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
 				 "%s: unable to free root XML tag.",
@@ -919,16 +919,16 @@
 	}
 	while( template_value_offset > 0 );
 
 	xml_token->size = xml_document_data_offset;
 
 	if( attribute_xml_tag != NULL )
 	{
-		if( libfwevt_xml_tag_free(
-		     &attribute_xml_tag,
+		if( libfwevt_internal_xml_tag_free(
+		     (libfwevt_internal_xml_tag_t **) &attribute_xml_tag,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
 			 "%s: unable to free attribute XML tag.",
@@ -951,16 +951,16 @@
 		goto on_error;
 	}
 	return( 1 );
 
 on_error:
 	if( attribute_xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &attribute_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &attribute_xml_tag,
 		 NULL );
 	}
 	if( xml_sub_token != NULL )
 	{
 		libfwevt_xml_token_free(
 		 &xml_sub_token,
 		 NULL );
@@ -1535,16 +1535,16 @@
 			 function,
 			 value_entry_index );
 
 			goto on_error;
 		}
 	}
 #endif
-	if( libfwevt_xml_tag_free(
-	     &character_xml_tag,
+	if( libfwevt_internal_xml_tag_free(
+	     (libfwevt_internal_xml_tag_t **) &character_xml_tag,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
 		 "%s: unable to free character XML tag.",
@@ -1563,16 +1563,16 @@
 	if( character_value_string != NULL )
 	{
 		memory_free(
 		 character_value_string );
 	}
 	if( character_xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &character_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &character_xml_tag,
 		 NULL );
 	}
 	return( -1 );
 }
 
 /* Reads an element from a binary XML document
  * Returns 1 if successful or -1 on error
@@ -2499,16 +2499,16 @@
 	}
 	while( template_value_offset > 0 );
 
 	xml_token->size = xml_document_data_offset;
 
 	if( element_xml_tag != NULL )
 	{
-		if( libfwevt_xml_tag_free(
-		     &element_xml_tag,
+		if( libfwevt_internal_xml_tag_free(
+		     (libfwevt_internal_xml_tag_t **) &element_xml_tag,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
 			 "%s: unable to free element XML tag.",
@@ -2532,16 +2532,16 @@
 	}
 	return( 1 );
 
 on_error:
 	if( ( element_xml_tag != NULL )
 	 && ( element_xml_tag != internal_xml_document->root_xml_tag ) )
 	{
-		libfwevt_xml_tag_free(
-		 &element_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &element_xml_tag,
 		 NULL );
 	}
 	if( xml_sub_token != NULL )
 	{
 		libfwevt_xml_token_free(
 		 &xml_sub_token,
 		 NULL );
@@ -3012,16 +3012,16 @@
 			 value_entry_index );
 
 			goto on_error;
 		}
 	}
 #endif /* defined( HAVE_DEBUG_OUTPUT ) */
 
-	if( libfwevt_xml_tag_free(
-	     &entity_xml_tag,
+	if( libfwevt_internal_xml_tag_free(
+	     (libfwevt_internal_xml_tag_t **) &entity_xml_tag,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
 		 "%s: unable to free entity XML tag.",
@@ -3040,16 +3040,16 @@
 	if( entity_name != NULL )
 	{
 		memory_free(
 		 entity_name );
 	}
 	if( entity_xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &entity_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &entity_xml_tag,
 		 NULL );
 	}
 	return( -1 );
 }
 
 /* Reads a fragment from a binary XML document
  * Returns 1 if successful or -1 on error
@@ -3590,15 +3590,14 @@
 		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 	}
 #endif
 	if( libfwevt_xml_tag_set_name_data(
 	     xml_tag,
 	     &( xml_document_data[ xml_document_data_offset ] ),
 	     name_size,
-	     LIBFVALUE_CODEPAGE_UTF16_LITTLE_ENDIAN,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
 		 "%s: unable to set name data.",
@@ -4606,16 +4605,16 @@
 	{
 		libfwevt_xml_token_free(
 		 &xml_sub_token,
 		 NULL );
 	}
 	if( pi_xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &pi_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &pi_xml_tag,
 		 NULL );
 	}
 	return( -1 );
 }
 
 /* Reads a template instance from a binary XML document
  * Returns 1 if successful or -1 on error
```

### Comparing `libfwevt-20240419/libfwevt/libfwevt_unused.h` & `libfwevt-20240426/libfwevt/libfwevt_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_libuna.h` & `libfwevt-20240426/libfwevt/libfwevt_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_xml_tag.h` & `libfwevt-20240426/libfwevt/libfwevt_xml_tag.h`

 * *Files 2% similar despite different names*

```diff
@@ -24,40 +24,39 @@
 
 #include <common.h>
 #include <types.h>
 
 #include "libfwevt_extern.h"
 #include "libfwevt_libcdata.h"
 #include "libfwevt_libcerror.h"
-#include "libfwevt_libfvalue.h"
 #include "libfwevt_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 typedef struct libfwevt_internal_xml_tag libfwevt_internal_xml_tag_t;
 
 struct libfwevt_internal_xml_tag
 {
 	/* The type
 	 */
 	uint8_t type;
 
-	/* The name (value)
+	/* The name
 	 */
-	libfvalue_value_t *name;
+	uint8_t *name;
 
-	/* The value type
+	/* The name size
 	 */
-	int value_type;
+	size_t name_size;
 
-	/* The value (value)
+	/* The value
 	 */
-	libfvalue_value_t *value;
+	libfwevt_xml_value_t *value;
 
 	/* The attributes array
 	 */
 	libcdata_array_t *attributes_array;
 
 	/* The elements array
 	 */
@@ -68,33 +67,32 @@
 	uint8_t flags;
 };
 
 int libfwevt_xml_tag_initialize(
      libfwevt_xml_tag_t **xml_tag,
      libcerror_error_t **error );
 
+LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_free(
      libfwevt_xml_tag_t **xml_tag,
      libcerror_error_t **error );
 
+int libfwevt_internal_xml_tag_free(
+     libfwevt_internal_xml_tag_t **internal_xml_tag,
+     libcerror_error_t **error );
+
 int libfwevt_xml_tag_set_type(
      libfwevt_xml_tag_t *xml_tag,
      uint8_t type,
      libcerror_error_t **error );
 
 int libfwevt_xml_tag_set_name_data(
      libfwevt_xml_tag_t *xml_tag,
      const uint8_t *data,
      size_t data_size,
-     int encoding,
-     libcerror_error_t **error );
-
-int libfwevt_xml_tag_get_value(
-     libfwevt_xml_tag_t *xml_tag,
-     libfvalue_value_t **value,
      libcerror_error_t **error );
 
 int libfwevt_xml_tag_set_value_type(
      libfwevt_xml_tag_t *xml_tag,
      int value_type,
      libcerror_error_t **error );
 
@@ -158,14 +156,20 @@
 int libfwevt_xml_tag_get_utf16_name(
      libfwevt_xml_tag_t *xml_tag,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libcerror_error_t **error );
 
 LIBFWEVT_EXTERN \
+int libfwevt_xml_tag_get_value(
+     libfwevt_xml_tag_t *xml_tag,
+     libfwevt_xml_value_t **xml_value,
+     libcerror_error_t **error );
+
+LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf8_value_size(
      libfwevt_xml_tag_t *xml_tag,
      size_t *utf8_string_size,
      libcerror_error_t **error );
 
 LIBFWEVT_EXTERN \
 int libfwevt_xml_tag_get_utf8_value(
@@ -306,14 +310,18 @@
      uint16_t *utf16_string,
      size_t utf16_string_size,
      size_t *utf16_string_index,
      libcerror_error_t **error );
 
 #if defined( HAVE_DEBUG_OUTPUT )
 
+int libfwevt_xml_tag_debug_print_name_string(
+     libfwevt_internal_xml_tag_t *internal_xml_tag,
+     libcerror_error_t **error );
+
 int libfwevt_xml_tag_debug_print_value_string(
      libfwevt_internal_xml_tag_t *internal_xml_tag,
      libcerror_error_t **error );
 
 int libfwevt_xml_tag_debug_print(
      libfwevt_xml_tag_t *xml_tag,
      int xml_tag_level,
```

### Comparing `libfwevt-20240419/libfwevt/libfwevt_manifest.c` & `libfwevt-20240426/libfwevt/libfwevt_manifest.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_event.c` & `libfwevt-20240426/libfwevt/libfwevt_event.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_task.h` & `libfwevt-20240426/libfwevt/libfwevt_task.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_task.c` & `libfwevt-20240426/libfwevt/libfwevt_task.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_template_item.c` & `libfwevt-20240426/libfwevt/libfwevt_template_item.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_manifest.h` & `libfwevt-20240426/libfwevt/libfwevt_manifest.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_support.h` & `libfwevt-20240426/libfwevt/libfwevt_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/Makefile.am` & `libfwevt-20240426/libfwevt/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 	libfwevt_template.c libfwevt_template.h \
 	libfwevt_template_item.c libfwevt_template_item.h \
 	libfwevt_types.h \
 	libfwevt_unused.h \
 	libfwevt_xml_document.c libfwevt_xml_document.h \
 	libfwevt_xml_tag.c libfwevt_xml_tag.h \
 	libfwevt_xml_template_value.c libfwevt_xml_template_value.h \
-	libfwevt_xml_token.c libfwevt_xml_token.h
+	libfwevt_xml_token.c libfwevt_xml_token.h \
+	libfwevt_xml_value.c libfwevt_xml_value.h
 
 libfwevt_la_LIBADD = \
 	@LIBCERROR_LIBADD@ \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBUNA_LIBADD@ \
```

### Comparing `libfwevt-20240419/libfwevt/libfwevt_map.c` & `libfwevt-20240426/libfwevt/libfwevt_map.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_libfvalue.h` & `libfwevt-20240426/libfwevt/libfwevt_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_provider.c` & `libfwevt-20240426/libfwevt/libfwevt_provider.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt.rc.in` & `libfwevt-20240426/libfwevt/libfwevt.rc.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_xml_template_value.h` & `libfwevt-20240426/libfwevt/libfwevt_xml_template_value.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_definitions.h.in` & `libfwevt-20240426/libfwevt/libfwevt_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_xml_document.h` & `libfwevt-20240426/libfwevt/libfwevt_xml_document.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_notify.c` & `libfwevt-20240426/libfwevt/libfwevt_notify.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_opcode.c` & `libfwevt-20240426/libfwevt/libfwevt_opcode.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_channel.h` & `libfwevt-20240426/libfwevt/libfwevt_channel.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_template.h` & `libfwevt-20240426/libfwevt/libfwevt_template.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_types.h` & `libfwevt-20240426/libfwevt/libfwevt_types.h`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 typedef struct libfwevt_provider {}		libfwevt_provider_t;
 typedef struct libfwevt_task {}			libfwevt_task_t;
 typedef struct libfwevt_template {}		libfwevt_template_t;
 typedef struct libfwevt_template_item {}	libfwevt_template_item_t;
 typedef struct libfwevt_xml_document {}		libfwevt_xml_document_t;
 typedef struct libfwevt_xml_tag {}		libfwevt_xml_tag_t;
 typedef struct libfwevt_xml_template_value {}	libfwevt_xml_template_value_t;
+typedef struct libfwevt_xml_value {}		libfwevt_xml_value_t;
 
 #else
 typedef intptr_t libfwevt_channel_t;
 typedef intptr_t libfwevt_event_t;
 typedef intptr_t libfwevt_keyword_t;
 typedef intptr_t libfwevt_level_t;
 typedef intptr_t libfwevt_manifest_t;
@@ -60,14 +61,15 @@
 typedef intptr_t libfwevt_provider_t;
 typedef intptr_t libfwevt_task_t;
 typedef intptr_t libfwevt_template_t;
 typedef intptr_t libfwevt_template_item_t;
 typedef intptr_t libfwevt_xml_document_t;
 typedef intptr_t libfwevt_xml_tag_t;
 typedef intptr_t libfwevt_xml_template_value_t;
+typedef intptr_t libfwevt_xml_value_t;
 
 #endif /* defined( HAVE_DEBUG_OUTPUT ) && !defined( WINAPI ) */
 
 #endif /* defined( HAVE_LOCAL_LIBFWEVT ) */
 
 #endif /* !defined( _LIBFWEVT_INTERNAL_TYPES_H ) */
```

### Comparing `libfwevt-20240419/libfwevt/libfwevt_definitions.h` & `libfwevt-20240426/libfwevt/libfwevt_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwevt/definitions.h> are copied here
  * for local use of libfwevt
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWEVT_VERSION						20240419
+#define LIBFWEVT_VERSION						20240426
 
 /* The version string
  */
-#define LIBFWEVT_VERSION_STRING						"20240419"
+#define LIBFWEVT_VERSION_STRING						"20240426"
 
 /* The byte order definitions
  */
 #define LIBFWEVT_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWEVT_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The binary XML document read flags
```

### Comparing `libfwevt-20240419/libfwevt/libfwevt_event.h` & `libfwevt-20240426/libfwevt/libfwevt_event.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_support.c` & `libfwevt-20240426/libfwevt/libfwevt_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_keyword.c` & `libfwevt-20240426/libfwevt/libfwevt_keyword.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_map.h` & `libfwevt-20240426/libfwevt/libfwevt_map.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_template_item.h` & `libfwevt-20240426/libfwevt/libfwevt_template_item.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_xml_tag.c` & `libfwevt-20240426/libfwevt/libfwevt_xml_tag.c`

 * *Files 14% similar despite different names*

```diff
@@ -26,22 +26,23 @@
 #include <types.h>
 #include <wide_string.h>
 
 #if defined( HAVE_WCTYPE_H )
 #include <wctype.h>
 #endif
 
+#include "libfwevt_debug.h"
 #include "libfwevt_definitions.h"
 #include "libfwevt_libcdata.h"
 #include "libfwevt_libcerror.h"
 #include "libfwevt_libcnotify.h"
-#include "libfwevt_libfvalue.h"
 #include "libfwevt_libuna.h"
 #include "libfwevt_types.h"
 #include "libfwevt_xml_tag.h"
+#include "libfwevt_xml_value.h"
 
 /* Creates a XML tag
  * Make sure the value xml_tag is referencing, is set to NULL
  * Returns 1 if successful or -1 on error
  */
 int libfwevt_xml_tag_initialize(
      libfwevt_xml_tag_t **xml_tag,
@@ -154,96 +155,110 @@
 /* Frees a XML tag
  * Returns 1 if successful or -1 on error
  */
 int libfwevt_xml_tag_free(
      libfwevt_xml_tag_t **xml_tag,
      libcerror_error_t **error )
 {
-	libfwevt_internal_xml_tag_t *internal_xml_tag = NULL;
-	static char *function                         = "libfwevt_xml_tag_free";
-	int result                                    = 1;
+	static char *function = "libfwevt_xml_tag_free";
 
 	if( xml_tag == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	if( *xml_tag != NULL )
 	{
-		internal_xml_tag = (libfwevt_internal_xml_tag_t *) *xml_tag;
-		*xml_tag         = NULL;
+		*xml_tag = NULL;
+	}
+	return( 1 );
+}
+
+/* Frees a XML tag
+ * Returns 1 if successful or -1 on error
+ */
+int libfwevt_internal_xml_tag_free(
+     libfwevt_internal_xml_tag_t **internal_xml_tag,
+     libcerror_error_t **error )
+{
+	static char *function = "libfwevt_internal_xml_tag_free";
+	int result            = 1;
+
+	if( internal_xml_tag == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid XML tag.",
+		 function );
 
+		return( -1 );
+	}
+	if( *internal_xml_tag != NULL )
+	{
 		if( libcdata_array_free(
-		     &( internal_xml_tag->elements_array ),
-		     (int (*)(intptr_t **, libcerror_error_t **)) &libfwevt_xml_tag_free,
+		     &( ( *internal_xml_tag )->elements_array ),
+		     (int (*)(intptr_t **, libcerror_error_t **)) &libfwevt_internal_xml_tag_free,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
 			 "%s: unable to free elements array.",
 			 function );
 
 			result = -1;
 		}
 		if( libcdata_array_free(
-		     &( internal_xml_tag->attributes_array ),
-		     (int (*)(intptr_t **, libcerror_error_t **)) &libfwevt_xml_tag_free,
+		     &( ( *internal_xml_tag )->attributes_array ),
+		     (int (*)(intptr_t **, libcerror_error_t **)) &libfwevt_internal_xml_tag_free,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
 			 "%s: unable to free attributes array.",
 			 function );
 
 			result = -1;
 		}
-		if( internal_xml_tag->value != NULL )
+		if( ( *internal_xml_tag )->value != NULL )
 		{
-			if( libfvalue_value_free(
-			     &( internal_xml_tag->value ),
+			if( libfwevt_internal_xml_value_free(
+			     (libfwevt_internal_xml_value_t **) &( ( *internal_xml_tag )->value ),
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
 				 "%s: unable to free value.",
 				 function );
 
 				result = -1;
 			}
 		}
-		if( internal_xml_tag->name != NULL )
+		if( ( *internal_xml_tag )->name != NULL )
 		{
-			if( libfvalue_value_free(
-			     &( internal_xml_tag->name ),
-			     error ) != 1 )
-			{
-				libcerror_error_set(
-				 error,
-				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
-				 "%s: unable to free name.",
-				 function );
-
-				result = -1;
-			}
+			memory_free(
+			 ( *internal_xml_tag )->name );
 		}
 		memory_free(
-		 internal_xml_tag );
+		 *internal_xml_tag );
+
+		*internal_xml_tag = NULL;
 	}
 	return( result );
 }
 
 /* Appends an attribute
  * Returns 1 if successful or -1 on error
  */
@@ -312,22 +327,21 @@
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
 	internal_xml_tag->type = type;
 
 	return( 1 );
 }
 
-/* Sets the name data
+/* Sets UTF-16 little-endian encoded name data
  * Returns 1 if successful or -1 on error
  */
 int libfwevt_xml_tag_set_name_data(
      libfwevt_xml_tag_t *xml_tag,
      const uint8_t *data,
      size_t data_size,
-     int encoding,
      libcerror_error_t **error )
 {
 	libfwevt_internal_xml_tag_t *internal_xml_tag = NULL;
 	static char *function                         = "libfwevt_xml_tag_set_name_data";
 
 	if( xml_tag == NULL )
 	{
@@ -338,107 +352,106 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	if( libfvalue_value_type_initialize(
-	     &( internal_xml_tag->name ),
-	     LIBFVALUE_VALUE_TYPE_STRING_UTF16,
-	     error ) != 1 )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
-		 "%s: unable to create name.",
-		 function );
-
-		goto on_error;
-	}
-	if( libfvalue_value_set_data(
-	     internal_xml_tag->name,
-	     data,
-	     data_size,
-	     encoding,
-	     LIBFVALUE_VALUE_DATA_FLAG_NON_MANAGED,
-	     error ) != 1 )
+	if( internal_xml_tag->name != NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
-		 "%s: unable to set name data.",
+		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
+		 "%s: invalid XML tag - name value already set.",
 		 function );
 
-		goto on_error;
-	}
-	return( 1 );
-
-on_error:
-	if( internal_xml_tag->name != NULL )
-	{
-		libfvalue_value_free(
-		 &( internal_xml_tag->name ),
-		 NULL );
+		return( -1 );
 	}
-	return( -1 );
-}
-
-/* Retrieves the value
- * Returns 1 if successful or -1 on error
- */
-int libfwevt_xml_tag_get_value(
-     libfwevt_xml_tag_t *xml_tag,
-     libfvalue_value_t **value,
-     libcerror_error_t **error )
-{
-	libfwevt_internal_xml_tag_t *internal_xml_tag = NULL;
-	static char *function                         = "libfwevt_xml_tag_get_value";
-
-	if( xml_tag == NULL )
+	if( data == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid XML tag.",
+		 "%s: invalid data.",
 		 function );
 
 		return( -1 );
 	}
-	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
-
-	if( value == NULL )
+	if( data_size > (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid value.",
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid data size value exceeds maximum.",
 		 function );
 
 		return( -1 );
 	}
-	*value = internal_xml_tag->value;
+	if( data_size > 0 )
+	{
+		internal_xml_tag->name = (uint8_t *) memory_allocate(
+		                                      sizeof( uint8_t ) * data_size );
 
+		if( internal_xml_tag->name == NULL )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_MEMORY,
+			 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+			 "%s: unable to create name.",
+			 function );
+
+			goto on_error;
+		}
+		internal_xml_tag->name_size = data_size;
+
+		if( memory_copy(
+		     internal_xml_tag->name,
+		     data,
+		     data_size ) == NULL )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_MEMORY,
+			 LIBCERROR_MEMORY_ERROR_COPY_FAILED,
+			 "%s: unable to copy name.",
+			 function );
+
+			goto on_error;
+		}
+	}
 	return( 1 );
+
+on_error:
+	if( internal_xml_tag->name != NULL )
+	{
+		memory_free(
+		 internal_xml_tag->name );
+
+		internal_xml_tag->name = NULL;
+	}
+	internal_xml_tag->name_size = 0;
+
+	return( -1 );
 }
 
 /* Sets the value type
  * Returns 1 if successful or -1 on error
  */
 int libfwevt_xml_tag_set_value_type(
      libfwevt_xml_tag_t *xml_tag,
      int value_type,
      libcerror_error_t **error )
 {
 	libfwevt_internal_xml_tag_t *internal_xml_tag = NULL;
 	static char *function                         = "libfwevt_xml_tag_set_value_type";
+	int current_value_type                        = 0;
 
 	if( xml_tag == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -447,40 +460,56 @@
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
 	if( internal_xml_tag->value == NULL )
 	{
-		if( libfvalue_value_type_initialize(
+		if( libfwevt_xml_value_initialize(
 		     &( internal_xml_tag->value ),
 		     value_type,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
 			 "%s: unable to create value.",
 			 function );
 
 			return( -1 );
 		}
-		 internal_xml_tag->value_type = value_type;
 	}
-	else if( internal_xml_tag->value_type != value_type )
+	else
 	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-		 "%s: invalid value type value mismatch.",
-		 function );
+		if( libfwevt_xml_value_get_type(
+		     internal_xml_tag->value,
+		     &current_value_type,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+			 "%s: unable to retrieve value type.",
+			 function );
 
-		return( -1 );
+			return( -1 );
+		}
+		if( value_type != current_value_type )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid value type value mismatch.",
+			 function );
+
+			return( -1 );
+		}
 	}
 	return( 1 );
 }
 
 /* Sets the value format flags
  * Returns 1 if successful or -1 on error
  */
@@ -501,15 +530,15 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	if( libfvalue_value_set_format_flags(
+	if( libfwevt_xml_value_set_format_flags(
 	     internal_xml_tag->value,
 	     format_flags,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -544,15 +573,15 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	if( libfvalue_value_set_data(
+	if( libfwevt_xml_value_set_data(
 	     internal_xml_tag->value,
 	     data,
 	     data_size,
 	     encoding,
 	     LIBFVALUE_VALUE_DATA_FLAG_NON_MANAGED,
 	     error ) != 1 )
 	{
@@ -591,15 +620,15 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	if( libfvalue_value_append_entry_data(
+	if( libfwevt_xml_value_append_data(
 	     internal_xml_tag->value,
 	     value_entry_index,
 	     data,
 	     data_size,
 	     encoding,
 	     error ) != 1 )
 	{
@@ -638,15 +667,15 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	read_count = libfvalue_value_type_set_data_string(
+	read_count = libfwevt_xml_value_type_set_data_string(
 		      internal_xml_tag->value,
 		      strings_array_data,
 		      strings_array_data_size,
 		      encoding,
 		      LIBFVALUE_VALUE_DATA_FLAG_NON_MANAGED,
 		      error );
 
@@ -727,25 +756,26 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	if( libfvalue_value_get_utf8_string_size(
+	if( libuna_utf8_string_size_from_utf16_stream(
 	     internal_xml_tag->name,
-	     0,
+	     internal_xml_tag->name_size,
+	     LIBUNA_ENDIAN_LITTLE,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-		 "%s: unable to retrieve size of UTF-8 string of name.",
+		 "%s: unable to retrieve UTF-8 string size.",
 		 function );
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
@@ -770,26 +800,27 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	if( libfvalue_value_copy_to_utf8_string(
-	     internal_xml_tag->name,
-	     0,
+	if( libuna_utf8_string_copy_from_utf16_stream(
 	     utf8_string,
 	     utf8_string_size,
+	     internal_xml_tag->name,
+	     internal_xml_tag->name_size,
+	     LIBUNA_ENDIAN_LITTLE,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-		 "%s: unable to copy name to UTF-8 string.",
+		 "%s: unable to retrieve UTF-8 string.",
 		 function );
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
@@ -813,25 +844,26 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	if( libfvalue_value_get_utf16_string_size(
+	if( libuna_utf16_string_size_from_utf16_stream(
 	     internal_xml_tag->name,
-	     0,
+	     internal_xml_tag->name_size,
+	     LIBUNA_ENDIAN_LITTLE,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-		 "%s: unable to retrieve size of UTF-16 string of name.",
+		 "%s: unable to retrieve UTF-16 string size.",
 		 function );
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
@@ -856,90 +888,112 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	if( libfvalue_value_copy_to_utf16_string(
-	     internal_xml_tag->name,
-	     0,
+	if( libuna_utf16_string_copy_from_utf16_stream(
 	     utf16_string,
 	     utf16_string_size,
+	     internal_xml_tag->name,
+	     internal_xml_tag->name_size,
+	     LIBUNA_ENDIAN_LITTLE,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-		 "%s: unable to copy name to UTF-16 string.",
+		 "%s: unable to retrieve UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the value
+ * Returns 1 if successful or -1 on error
+ */
+int libfwevt_xml_tag_get_value(
+     libfwevt_xml_tag_t *xml_tag,
+     libfwevt_xml_value_t **xml_value,
+     libcerror_error_t **error )
+{
+	libfwevt_internal_xml_tag_t *internal_xml_tag = NULL;
+	static char *function                         = "libfwevt_xml_tag_get_value";
+
+	if( xml_tag == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
+	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
+
+	if( xml_value == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid XML value.",
+		 function );
+
+		return( -1 );
+	}
+	*xml_value = internal_xml_tag->value;
+
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 formatted value
  * Returns 1 if successful or -1 on error
  */
 int libfwevt_xml_tag_get_utf8_value_size(
      libfwevt_xml_tag_t *xml_tag,
      size_t *utf8_string_size,
      libcerror_error_t **error )
 {
 	libfwevt_internal_xml_tag_t *internal_xml_tag = NULL;
 	static char *function                         = "libfwevt_xml_tag_get_utf8_value_size";
-	int result                                    = 0;
 
 	if( xml_tag == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	result = libfvalue_value_get_utf8_string_size(
-	          internal_xml_tag->value,
-	          0,
-	          utf8_string_size,
-	          error );
-
-	if( result == -1 )
+	if( libfwevt_xml_value_get_utf8_string_size(
+	     internal_xml_tag->value,
+	     utf8_string_size,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve size of UTF-8 string of value.",
 		 function );
 
 		return( -1 );
 	}
-	else if( result == 0 )
-	{
-		if( utf8_string_size == NULL )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-			 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-			 "%s: invalid UTF-8 string size.",
-			 function );
-
-			return( -1 );
-		}
-		*utf8_string_size = 0;
-	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 formatted value
  * Returns 1 if successful or -1 on error
  */
 int libfwevt_xml_tag_get_utf8_value(
@@ -960,17 +1014,16 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	if( libfvalue_value_copy_to_utf8_string(
+	if( libfwevt_xml_value_copy_to_utf8_string(
 	     internal_xml_tag->value,
-	     0,
 	     utf8_string,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -989,61 +1042,42 @@
 int libfwevt_xml_tag_get_utf16_value_size(
      libfwevt_xml_tag_t *xml_tag,
      size_t *utf16_string_size,
      libcerror_error_t **error )
 {
 	libfwevt_internal_xml_tag_t *internal_xml_tag = NULL;
 	static char *function                         = "libfwevt_xml_tag_get_utf16_value_size";
-	int result                                    = 0;
 
 	if( xml_tag == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	result = libfvalue_value_get_utf16_string_size(
-	          internal_xml_tag->value,
-	          0,
-	          utf16_string_size,
-	          error );
-
-	if( result == -1 )
+	if( libfwevt_xml_value_get_utf16_string_size(
+	     internal_xml_tag->value,
+	     utf16_string_size,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve size of UTF-16 string of value.",
 		 function );
 
 		return( -1 );
 	}
-	else if( result == 0 )
-	{
-		if( utf16_string_size == NULL )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-			 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-			 "%s: invalid UTF-16 string size.",
-			 function );
-
-			return( -1 );
-		}
-		*utf16_string_size = 0;
-	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 formatted value
  * Returns 1 if successful or -1 on error
  */
 int libfwevt_xml_tag_get_utf16_value(
@@ -1064,17 +1098,16 @@
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
-	if( libfvalue_value_copy_to_utf16_string(
+	if( libfwevt_xml_value_copy_to_utf16_string(
 	     internal_xml_tag->value,
-	     0,
 	     utf16_string,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -1188,17 +1221,15 @@
 	static char *function                                   = "libfwevt_xml_tag_get_attribute_by_utf8_name";
 	libuna_unicode_character_t name_character               = 0;
 	libuna_unicode_character_t string_character             = 0;
 	size_t name_index                                       = 0;
 	size_t utf8_string_index                                = 0;
 	size_t value_entry_data_size                            = 0;
 	int attribute_index                                     = 0;
-	int encoding                                            = 0;
 	int number_of_attributes                                = 0;
-	int value_type                                          = 0;
 
 	if( xml_tag == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1299,57 +1330,18 @@
 			 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
 			 "%s: missing attribute: %d.",
 			 function,
 			 attribute_index );
 
 			return( -1 );
 		}
-		if( libfvalue_value_get_type(
-		     internal_attribute_xml_tag->name,
-		     &value_type,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve attribute name value type.",
-			 function );
+/* TODO bounds check and clean up */
+		value_entry_data      = internal_attribute_xml_tag->name;
+		value_entry_data_size = internal_attribute_xml_tag->name_size;
 
-			return( -1 );
-		}
-		if( value_type != LIBFVALUE_VALUE_TYPE_STRING_UTF16 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-			 "%s: unsupported attribute name value type: %d.",
-			 function,
-			 value_type );
-
-			return( -1 );
-		}
-		if( libfvalue_value_get_entry_data(
-		     internal_attribute_xml_tag->name,
-		     0,
-		     &value_entry_data,
-		     &value_entry_data_size,
-		     &encoding,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve attribute name value type.",
-			 function );
-
-			return( -1 );
-		}
 		if( ( value_entry_data[ value_entry_data_size - 2 ] == 0 )
 		 && ( value_entry_data[ value_entry_data_size - 1 ] == 0 ) )
 		{
 			value_entry_data_size -= 2;
 		}
 		name_index        = 0;
 		utf8_string_index = 0;
@@ -1426,17 +1418,15 @@
 	static char *function                                   = "libfwevt_xml_tag_get_attribute_by_utf16_name";
 	libuna_unicode_character_t name_character               = 0;
 	libuna_unicode_character_t string_character             = 0;
 	size_t name_index                                       = 0;
 	size_t utf16_string_index                               = 0;
 	size_t value_entry_data_size                            = 0;
 	int attribute_index                                     = 0;
-	int encoding                                            = 0;
 	int number_of_attributes                                = 0;
-	int value_type                                          = 0;
 
 	if( xml_tag == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1537,57 +1527,18 @@
 			 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
 			 "%s: missing attribute: %d.",
 			 function,
 			 attribute_index );
 
 			return( -1 );
 		}
-		if( libfvalue_value_get_type(
-		     internal_attribute_xml_tag->name,
-		     &value_type,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve attribute name value type.",
-			 function );
-
-			return( -1 );
-		}
-		if( value_type != LIBFVALUE_VALUE_TYPE_STRING_UTF16 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-			 "%s: unsupported attribute name value type: %d.",
-			 function,
-			 value_type );
-
-			return( -1 );
-		}
-		if( libfvalue_value_get_entry_data(
-		     internal_attribute_xml_tag->name,
-		     0,
-		     &value_entry_data,
-		     &value_entry_data_size,
-		     &encoding,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve attribute name value type.",
-			 function );
+/* TODO bounds check and clean up */
+		value_entry_data      = internal_attribute_xml_tag->name;
+		value_entry_data_size = internal_attribute_xml_tag->name_size;
 
-			return( -1 );
-		}
 		if( ( value_entry_data[ value_entry_data_size - 2 ] == 0 )
 		 && ( value_entry_data[ value_entry_data_size - 1 ] == 0 ) )
 		{
 			value_entry_data_size -= 2;
 		}
 		name_index         = 0;
 		utf16_string_index = 0;
@@ -1749,17 +1700,15 @@
 	static char *function                                 = "libfwevt_xml_tag_get_element_by_utf8_name";
 	libuna_unicode_character_t name_character             = 0;
 	libuna_unicode_character_t string_character           = 0;
 	size_t name_index                                     = 0;
 	size_t utf8_string_index                              = 0;
 	size_t value_entry_data_size                          = 0;
 	int element_index                                     = 0;
-	int encoding                                          = 0;
 	int number_of_elements                                = 0;
-	int value_type                                        = 0;
 
 	if( xml_tag == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1860,57 +1809,18 @@
 			 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
 			 "%s: missing element: %d.",
 			 function,
 			 element_index );
 
 			return( -1 );
 		}
-		if( libfvalue_value_get_type(
-		     internal_element_xml_tag->name,
-		     &value_type,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve element name value type.",
-			 function );
-
-			return( -1 );
-		}
-		if( value_type != LIBFVALUE_VALUE_TYPE_STRING_UTF16 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-			 "%s: unsupported element name value type: %d.",
-			 function,
-			 value_type );
-
-			return( -1 );
-		}
-		if( libfvalue_value_get_entry_data(
-		     internal_element_xml_tag->name,
-		     0,
-		     &value_entry_data,
-		     &value_entry_data_size,
-		     &encoding,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve element name value type.",
-			 function );
+/* TODO bounds check and clean up */
+		value_entry_data      = internal_element_xml_tag->name;
+		value_entry_data_size = internal_element_xml_tag->name_size;
 
-			return( -1 );
-		}
 		if( ( value_entry_data[ value_entry_data_size - 2 ] == 0 )
 		 && ( value_entry_data[ value_entry_data_size - 1 ] == 0 ) )
 		{
 			value_entry_data_size -= 2;
 		}
 		name_index        = 0;
 		utf8_string_index = 0;
@@ -1987,17 +1897,15 @@
 	static char *function                                 = "libfwevt_xml_tag_get_element_by_utf16_name";
 	libuna_unicode_character_t name_character             = 0;
 	libuna_unicode_character_t string_character           = 0;
 	size_t name_index                                     = 0;
 	size_t utf16_string_index                             = 0;
 	size_t value_entry_data_size                          = 0;
 	int element_index                                     = 0;
-	int encoding                                          = 0;
 	int number_of_elements                                = 0;
-	int value_type                                        = 0;
 
 	if( xml_tag == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2098,57 +2006,18 @@
 			 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
 			 "%s: missing element: %d.",
 			 function,
 			 element_index );
 
 			return( -1 );
 		}
-		if( libfvalue_value_get_type(
-		     internal_element_xml_tag->name,
-		     &value_type,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve element name value type.",
-			 function );
-
-			return( -1 );
-		}
-		if( value_type != LIBFVALUE_VALUE_TYPE_STRING_UTF16 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-			 "%s: unsupported element name value type: %d.",
-			 function,
-			 value_type );
-
-			return( -1 );
-		}
-		if( libfvalue_value_get_entry_data(
-		     internal_element_xml_tag->name,
-		     0,
-		     &value_entry_data,
-		     &value_entry_data_size,
-		     &encoding,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve element name value type.",
-			 function );
+/* TODO bounds check and clean up */
+		value_entry_data      = internal_element_xml_tag->name;
+		value_entry_data_size = internal_element_xml_tag->name_size;
 
-			return( -1 );
-		}
 		if( ( value_entry_data[ value_entry_data_size - 2 ] == 0 )
 		 && ( value_entry_data[ value_entry_data_size - 1 ] == 0 ) )
 		{
 			value_entry_data_size -= 2;
 		}
 		name_index         = 0;
 		utf16_string_index = 0;
@@ -2299,22 +2168,23 @@
 int libfwevt_xml_tag_get_utf8_xml_value_string_size(
      libfwevt_internal_xml_tag_t *internal_xml_tag,
      size_t *utf8_string_size,
      libcerror_error_t **error )
 {
 	uint8_t static_value_string[ 2 ];
 
-	uint8_t *value_string       = NULL;
-	static char *function       = "libfwevt_xml_tag_get_utf8_xml_value_string_size";
-	size_t value_string_index   = 0;
-	size_t value_string_size    = 0;
-	int number_of_value_entries = 0;
-	int result                  = 0;
-	int value_entry_index       = 0;
-	int value_type              = 0;
+	uint8_t *value_string        = NULL;
+	static char *function        = "libfwevt_xml_tag_get_utf8_xml_value_string_size";
+	size_t safe_utf8_string_size = 0;
+	size_t value_string_index    = 0;
+	size_t value_string_size     = 0;
+	int number_of_value_entries  = 0;
+	int result                   = 0;
+	int value_entry_index        = 0;
+	int value_type               = 0;
 
 	if( internal_xml_tag == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2330,49 +2200,47 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-8 string size.",
 		 function );
 
 		return( -1 );
 	}
-	if( libfvalue_value_get_type(
+	if( libfwevt_xml_value_get_type(
 	     internal_xml_tag->value,
 	     &value_type,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve element value type.",
 		 function );
 
 		goto on_error;
 	}
-	if( libfvalue_value_get_number_of_value_entries(
+	if( libfwevt_xml_value_get_number_of_value_entries(
 	     internal_xml_tag->value,
 	     &number_of_value_entries,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve element value number of value entries.",
 		 function );
 
 		goto on_error;
 	}
-	*utf8_string_size = 0;
-
 	for( value_entry_index = 0;
 	     value_entry_index < number_of_value_entries;
 	     value_entry_index++ )
 	{
-		result = libfvalue_value_get_utf8_string_size(
+		result = libfwevt_xml_value_get_utf8_string_size_with_index(
 			  internal_xml_tag->value,
 			  value_entry_index,
 			  &value_string_size,
 			  error );
 
 		if( result == -1 )
 		{
@@ -2400,19 +2268,22 @@
 			goto on_error;
 		}
 		if( result != 0 )
 		{
 			if( ( number_of_value_entries == 1 )
 			 && ( value_string_size == 2 ) )
 			{
-				if( libfvalue_value_copy_to_utf8_string(
+				value_string_index = 0;
+
+				if( libfwevt_xml_value_copy_to_utf8_string_with_index(
 				     internal_xml_tag->value,
 				     0,
 				     static_value_string,
 				     2,
+				     &value_string_index,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 					 "%s: unable to copy element value: 0 to UTF-8 string.",
@@ -2451,19 +2322,22 @@
 					 LIBCERROR_ERROR_DOMAIN_MEMORY,
 					 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
 					 "%s: unable to create value string.",
 					 function );
 
 					goto on_error;
 				}
-				if( libfvalue_value_copy_to_utf8_string(
+				value_string_index = 0;
+
+				if( libfwevt_xml_value_copy_to_utf8_string_with_index(
 				     internal_xml_tag->value,
 				     value_entry_index,
 				     value_string,
 				     value_string_size,
+				     &value_string_index,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 					 "%s: unable to copy element value: %d to UTF-8 string.",
@@ -2476,28 +2350,28 @@
 				     value_string_index < ( value_string_size - 1 );
 				     value_string_index++ )
 				{
 					switch( value_string[ value_string_index ] )
 					{
 						/* Replace & by &amp; */
 						case (uint8_t) '&':
-							*utf8_string_size += 4;
+							safe_utf8_string_size += 4;
 							break;
 
 						/* Replace < by &lt; and > by &gt; */
 						case (uint8_t) '<':
 						case (uint8_t) '>':
-							*utf8_string_size += 3;
+							safe_utf8_string_size += 3;
 							break;
 
 						/* Replace ' by &apos; and " by &quot; */
 /* TODO disabled for now since Event Viewer does not uses it
 						case (uint8_t) '\'':
 						case (uint8_t) '"':
-							*utf8_string_size += 5;
+							safe_utf8_string_size += 5;
 							break;
 */
 
 						default:
 							break;
 					}
 				}
@@ -2507,25 +2381,27 @@
 				value_string = NULL;
 			}
 			if( value_string_size > 1 )
 			{
 				/* The size of:
 				 *   value formatted as a string
 				 */
-				*utf8_string_size += value_string_size - 1;
+				safe_utf8_string_size += value_string_size - 1;
 			}
 		}
 	}
-	if( *utf8_string_size != 0 )
+	if( safe_utf8_string_size != 0 )
 	{
 		/* The size of:
 		 *   end-of-string character
 		 */
-		*utf8_string_size += 1;
+		safe_utf8_string_size += 1;
 	}
+	*utf8_string_size = safe_utf8_string_size;
+
 	return( 1 );
 
 on_error:
 	if( value_string != NULL )
 	{
 		memory_free(
 		 value_string );
@@ -2595,29 +2471,29 @@
 		 "%s: invalid UTF-8 string index.",
 		 function );
 
 		return( -1 );
 	}
 	string_index = *utf8_string_index;
 
-	if( libfvalue_value_get_type(
+	if( libfwevt_xml_value_get_type(
 	     internal_xml_tag->value,
 	     &value_type,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve element value type.",
 		 function );
 
 		goto on_error;
 	}
-	if( libfvalue_value_get_number_of_value_entries(
+	if( libfwevt_xml_value_get_number_of_value_entries(
 	     internal_xml_tag->value,
 	     &number_of_value_entries,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -2627,15 +2503,15 @@
 
 		goto on_error;
 	}
 	for( value_entry_index = 0;
 	     value_entry_index < number_of_value_entries;
 	     value_entry_index++ )
 	{
-		result = libfvalue_value_get_utf8_string_size(
+		result = libfwevt_xml_value_get_utf8_string_size_with_index(
 			  internal_xml_tag->value,
 			  value_entry_index,
 			  &value_string_size,
 			  error );
 
 		if( result == -1 )
 		{
@@ -2689,19 +2565,22 @@
 					 LIBCERROR_ERROR_DOMAIN_MEMORY,
 					 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
 					 "%s: unable to create value string.",
 					 function );
 
 					goto on_error;
 				}
-				if( libfvalue_value_copy_to_utf8_string(
+				value_string_index = 0;
+
+				if( libfwevt_xml_value_copy_to_utf8_string_with_index(
 				     internal_xml_tag->value,
 				     value_entry_index,
 				     value_string,
 				     value_string_size,
+				     &value_string_index,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 					 "%s: unable to copy element value: %d to UTF-8 string.",
@@ -2845,15 +2724,15 @@
 				memory_free(
 				 value_string );
 
 				value_string = NULL;
 			}
 			else
 			{
-				if( libfvalue_value_copy_to_utf8_string_with_index(
+				if( libfwevt_xml_value_copy_to_utf8_string_with_index(
 				     internal_xml_tag->value,
 				     value_entry_index,
 				     utf8_string,
 				     utf8_string_size,
 				     &string_index,
 				     error ) != 1 )
 				{
@@ -2905,15 +2784,17 @@
      size_t *utf8_string_size,
      libcerror_error_t **error )
 {
 	libfwevt_internal_xml_tag_t *internal_attribute_xml_tag = NULL;
 	libfwevt_internal_xml_tag_t *internal_xml_tag           = NULL;
 	libfwevt_xml_tag_t *element_xml_tag                     = NULL;
 	static char *function                                   = "libfwevt_xml_tag_get_utf8_xml_string_size";
-	size_t name_size                                        = 0;
+	size_t attribute_name_size                              = 0;
+	size_t element_name_size                                = 0;
+	size_t safe_utf8_string_size                            = 0;
 	size_t string_size                                      = 0;
 	size_t value_string_size                                = 0;
 	int attribute_index                                     = 0;
 	int element_index                                       = 0;
 	int number_of_attributes                                = 0;
 	int number_of_elements                                  = 0;
 	int value_type                                          = 0;
@@ -2956,15 +2837,15 @@
 
 		return( -1 );
 	}
 	/* The size of:
 	 *   2 x ' ' character per indentation level
 	 *   1 x '<' character
 	 */
-	*utf8_string_size = ( xml_tag_level * 2 ) + 1;
+	safe_utf8_string_size = ( xml_tag_level * 2 ) + 1;
 
 	if( internal_xml_tag->type == LIBFWEVT_XML_TAG_TYPE_NODE )
 	{
 		if( libcdata_array_get_number_of_entries(
 		     internal_xml_tag->elements_array,
 		     &number_of_elements,
 		     error ) != 1 )
@@ -2974,33 +2855,34 @@
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 			 "%s: unable to retrieve number of elements.",
 			 function );
 
 			return( -1 );
 		}
-		if( libfvalue_value_get_utf8_string_size(
+		if( libuna_utf8_string_size_from_utf16_stream(
 		     internal_xml_tag->name,
-		     0,
-		     &name_size,
+		     internal_xml_tag->name_size,
+		     LIBUNA_ENDIAN_LITTLE,
+		     &element_name_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve size of UTF-8 string of name.",
+			 "%s: unable to retrieve UTF-8 string size of element name.",
 			 function );
 
 			return( -1 );
 		}
 		/* The size of:
 		 *   element name
 		 */
-		*utf8_string_size += name_size - 1;
+		safe_utf8_string_size += element_name_size - 1;
 
 		if( number_of_attributes > 0 )
 		{
 			for( attribute_index = 0;
 			     attribute_index < number_of_attributes;
 			     attribute_index++ )
 			{
@@ -3028,18 +2910,19 @@
 					 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
 					 "%s: missing attribute: %d.",
 					 function,
 					 attribute_index );
 
 					return( -1 );
 				}
-				if( libfvalue_value_get_utf8_string_size(
+				if( libuna_utf8_string_size_from_utf16_stream(
 				     internal_attribute_xml_tag->name,
-				     0,
-				     &string_size,
+				     internal_attribute_xml_tag->name_size,
+				     LIBUNA_ENDIAN_LITTLE,
+				     &attribute_name_size,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 					 "%s: unable to retrieve UTF-8 string size of attribute: %d name.",
@@ -3050,31 +2933,31 @@
 				}
 				/* The size of:
 				 *   1 x ' ' character
 				 *   attribute name
 				 *   1 x '=' character
 				 *   1 x '"' character
 				 */
-				*utf8_string_size += string_size + 2;
+				safe_utf8_string_size += attribute_name_size + 2;
 
-				if( libfvalue_value_get_type(
+				if( libfwevt_xml_value_get_type(
 				     internal_attribute_xml_tag->value,
 				     &value_type,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 					 "%s: unable to retrieve attribute value type.",
 					 function );
 
 					return( -1 );
 				}
-				if( libfvalue_value_get_utf8_string_size(
+				if( libfwevt_xml_value_get_utf8_string_size_with_index(
 				     internal_attribute_xml_tag->value,
 				     0,
 				     &string_size,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
@@ -3086,15 +2969,15 @@
 
 					return( -1 );
 				}
 				/* The size of:
 				 *   attribute value formatted as a string
 				 *   1 x '"' character
 				 */
-				*utf8_string_size += string_size;
+				safe_utf8_string_size += string_size;
 			}
 		}
 		if( internal_xml_tag->value != NULL )
 		{
 			if( libfwevt_xml_tag_get_utf8_xml_value_string_size(
 			     internal_xml_tag,
 			     &value_string_size,
@@ -3114,22 +2997,22 @@
 				/* The size of:
 				 *   1 x '>' character
 				 *   value formatted as a string
 				 *   1 x '<' character
 				 *   1 x '/' character
 				 *   element name
 				 */
-				*utf8_string_size += value_string_size + name_size + 1;
+				safe_utf8_string_size += value_string_size + element_name_size + 1;
 			}
 			else
 			{
 				/* The size of:
 				 *   1 x '/' character
 				 */
-				*utf8_string_size += 1;
+				safe_utf8_string_size += 1;
 			}
 		}
 		else if( number_of_elements > 0 )
 		{
 			for( element_index = 0;
 			     element_index < number_of_elements;
 			     element_index++ )
@@ -3165,37 +3048,37 @@
 					 element_index );
 
 					return( -1 );
 				}
 				/* The size of:
 				 *   sub element formatted as a string
 				 */
-				*utf8_string_size += string_size - 1;
+				safe_utf8_string_size += string_size - 1;
 			}
 			/* The size of:
 			 *   1 x '>' character
 			 *   1 x '\n' character
 			 *   2 x ' ' character per indentation level
 			 *   1 x '<' character
 			 *   1 x '/' character
 			 *   element name
 			 */
-			*utf8_string_size += ( xml_tag_level * 2 ) + name_size + 3;
+			safe_utf8_string_size += ( xml_tag_level * 2 ) + element_name_size + 3;
 		}
 		else
 		{
 			/* The size of:
 			 *   1 x '/' character
 			 */
-			*utf8_string_size += 1;
+			safe_utf8_string_size += 1;
 		}
 	}
 	else if( internal_xml_tag->type == LIBFWEVT_XML_TAG_TYPE_CDATA )
 	{
-		if( libfvalue_value_get_utf8_string_size(
+		if( libfwevt_xml_value_get_utf8_string_size_with_index(
 		     internal_xml_tag->value,
 		     0,
 		     &string_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
@@ -3207,40 +3090,41 @@
 			return( -1 );
 		}
 		/* The size of:
 		 *   1 x "![CDATA["
 		 *   value formatted as a string
 		 *   1 x "]]"
 		 */
-		*utf8_string_size += string_size + 9;
+		safe_utf8_string_size += string_size + 9;
 	}
 	else if( internal_xml_tag->type == LIBFWEVT_XML_TAG_TYPE_PI )
 	{
-		if( libfvalue_value_get_utf8_string_size(
+		if( libuna_utf8_string_size_from_utf16_stream(
 		     internal_xml_tag->name,
-		     0,
-		     &name_size,
+		     internal_xml_tag->name_size,
+		     LIBUNA_ENDIAN_LITTLE,
+		     &element_name_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve UTF-8 string size of name.",
+			 "%s: unable to retrieve UTF-8 string size of element name.",
 			 function );
 
 			return( -1 );
 		}
 		/* The size of:
 		 *   1 x '?' character
 		 *   element name
 		 */
-		*utf8_string_size += name_size;
+		safe_utf8_string_size += element_name_size;
 
-		if( libfvalue_value_get_utf8_string_size(
+		if( libfwevt_xml_value_get_utf8_string_size_with_index(
 		     internal_xml_tag->value,
 		     0,
 		     &string_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
@@ -3252,22 +3136,24 @@
 			return( -1 );
 		}
 		/* The size of:
 		 *   1 x ' ' character
 		 *   element name
 		 *   1 x '?' character
 		 */
-		*utf8_string_size += string_size + 1;
+		safe_utf8_string_size += string_size + 1;
 	}
 	/* The size of:
 	 *   1 x '>' character
 	 *   1 x '\n' character
 	 *   1 x '\0' character
 	 */
-	*utf8_string_size += 3;
+	safe_utf8_string_size += 3;
+
+	*utf8_string_size = safe_utf8_string_size;
 
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 formatted string of the XML tag
  * Returns 1 if successful or -1 on error
  */
@@ -3386,20 +3272,21 @@
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 			 "%s: unable to retrieve number of elements.",
 			 function );
 
 			return( -1 );
 		}
-		if( libfvalue_value_copy_to_utf8_string_with_index(
-		     internal_xml_tag->name,
-		     0,
+		if( libuna_utf8_string_with_index_copy_from_utf16_stream(
 		     utf8_string,
 		     utf8_string_size,
 		     &string_index,
+		     internal_xml_tag->name,
+		     internal_xml_tag->name_size,
+		     LIBUNA_ENDIAN_LITTLE,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 			 "%s: unable to copy name to UTF-8 string.",
@@ -3452,20 +3339,21 @@
 					 "%s: UTF-8 string size too small.",
 					 function );
 
 					return( -1 );
 				}
 				utf8_string[ string_index++ ] = (uint8_t) ' ';
 
-				if( libfvalue_value_copy_to_utf8_string_with_index(
-				     internal_attribute_xml_tag->name,
-				     0,
+				if( libuna_utf8_string_with_index_copy_from_utf16_stream(
 				     utf8_string,
 				     utf8_string_size,
 				     &string_index,
+				     internal_attribute_xml_tag->name,
+				     internal_attribute_xml_tag->name_size,
+				     LIBUNA_ENDIAN_LITTLE,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 					 "%s: unable to copy attribute: %d name to UTF-8 string.",
@@ -3486,29 +3374,29 @@
 					 function );
 
 					return( -1 );
 				}
 				utf8_string[ string_index++ ] = (uint8_t) '=';
 				utf8_string[ string_index++ ] = (uint8_t) '"';
 
-				if( libfvalue_value_get_type(
+				if( libfwevt_xml_value_get_type(
 				     internal_attribute_xml_tag->value,
 				     &value_type,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 					 "%s: unable to retrieve attribute value type.",
 					 function );
 
 					return( -1 );
 				}
-				if( libfvalue_value_copy_to_utf8_string_with_index(
+				if( libfwevt_xml_value_copy_to_utf8_string_with_index(
 				     internal_attribute_xml_tag->value,
 				     0,
 				     utf8_string,
 				     utf8_string_size,
 				     &string_index,
 				     error ) != 1 )
 				{
@@ -3597,20 +3485,21 @@
 					 function );
 
 					return( -1 );
 				}
 				utf8_string[ string_index++ ] = (uint8_t) '<';
 				utf8_string[ string_index++ ] = (uint8_t) '/';
 
-				if( libfvalue_value_copy_to_utf8_string_with_index(
-				     internal_xml_tag->name,
-				     0,
+				if( libuna_utf8_string_with_index_copy_from_utf16_stream(
 				     utf8_string,
 				     utf8_string_size,
 				     &string_index,
+				     internal_xml_tag->name,
+				     internal_xml_tag->name_size,
+				     LIBUNA_ENDIAN_LITTLE,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 					 "%s: unable to copy name to UTF-8 string.",
@@ -3720,20 +3609,21 @@
 				 function );
 
 				return( -1 );
 			}
 			utf8_string[ string_index++ ] = (uint8_t) '<';
 			utf8_string[ string_index++ ] = (uint8_t) '/';
 
-			if( libfvalue_value_copy_to_utf8_string_with_index(
-			     internal_xml_tag->name,
-			     0,
+			if( libuna_utf8_string_with_index_copy_from_utf16_stream(
 			     utf8_string,
 			     utf8_string_size,
 			     &string_index,
+			     internal_xml_tag->name,
+			     internal_xml_tag->name_size,
+			     LIBUNA_ENDIAN_LITTLE,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 				 "%s: unable to copy name to UTF-8 string.",
@@ -3788,15 +3678,15 @@
 		utf8_string[ string_index++ ] = (uint8_t) 'C';
 		utf8_string[ string_index++ ] = (uint8_t) 'D';
 		utf8_string[ string_index++ ] = (uint8_t) 'A';
 		utf8_string[ string_index++ ] = (uint8_t) 'T';
 		utf8_string[ string_index++ ] = (uint8_t) 'A';
 		utf8_string[ string_index++ ] = (uint8_t) '[';
 
-		if( libfvalue_value_copy_to_utf8_string_with_index(
+		if( libfwevt_xml_value_copy_to_utf8_string_with_index(
 		     internal_xml_tag->value,
 		     0,
 		     utf8_string,
 		     utf8_string_size,
 		     &string_index,
 		     error ) != 1 )
 		{
@@ -3836,20 +3726,21 @@
 			 "%s: UTF-8 string size too small.",
 			 function );
 
 			return( -1 );
 		}
 		utf8_string[ string_index++ ] = (uint8_t) '?';
 
-		if( libfvalue_value_copy_to_utf8_string_with_index(
-		     internal_xml_tag->name,
-		     0,
+		if( libuna_utf8_string_with_index_copy_from_utf16_stream(
 		     utf8_string,
 		     utf8_string_size,
 		     &string_index,
+		     internal_xml_tag->name,
+		     internal_xml_tag->name_size,
+		     LIBUNA_ENDIAN_LITTLE,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 			 "%s: unable to copy name to UTF-8 string.",
@@ -3868,15 +3759,15 @@
 			 "%s: UTF-8 string size too small.",
 			 function );
 
 			return( -1 );
 		}
 		utf8_string[ string_index++ ] = (uint8_t) ' ';
 
-		if( libfvalue_value_copy_to_utf8_string_with_index(
+		if( libfwevt_xml_value_copy_to_utf8_string_with_index(
 		     internal_xml_tag->value,
 		     0,
 		     utf8_string,
 		     utf8_string_size,
 		     &string_index,
 		     error ) != 1 )
 		{
@@ -3919,22 +3810,23 @@
 int libfwevt_xml_tag_get_utf16_xml_value_string_size(
      libfwevt_internal_xml_tag_t *internal_xml_tag,
      size_t *utf16_string_size,
      libcerror_error_t **error )
 {
 	uint16_t static_value_string[ 2 ];
 
-	uint16_t *value_string      = NULL;
-	static char *function       = "libfwevt_xml_tag_get_utf16_xml_value_string_size";
-	size_t value_string_index   = 0;
-	size_t value_string_size    = 0;
-	int number_of_value_entries = 0;
-	int result                  = 0;
-	int value_entry_index       = 0;
-	int value_type              = 0;
+	uint16_t *value_string        = NULL;
+	static char *function         = "libfwevt_xml_tag_get_utf16_xml_value_string_size";
+	size_t safe_utf16_string_size = 0;
+	size_t value_string_index     = 0;
+	size_t value_string_size      = 0;
+	int number_of_value_entries   = 0;
+	int result                    = 0;
+	int value_entry_index         = 0;
+	int value_type                = 0;
 
 	if( internal_xml_tag == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -3950,49 +3842,47 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-16 string size.",
 		 function );
 
 		return( -1 );
 	}
-	if( libfvalue_value_get_type(
+	if( libfwevt_xml_value_get_type(
 	     internal_xml_tag->value,
 	     &value_type,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve element value type.",
 		 function );
 
 		goto on_error;
 	}
-	if( libfvalue_value_get_number_of_value_entries(
+	if( libfwevt_xml_value_get_number_of_value_entries(
 	     internal_xml_tag->value,
 	     &number_of_value_entries,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve element value number of value entries.",
 		 function );
 
 		goto on_error;
 	}
-	*utf16_string_size = 0;
-
 	for( value_entry_index = 0;
 	     value_entry_index < number_of_value_entries;
 	     value_entry_index++ )
 	{
-		result = libfvalue_value_get_utf16_string_size(
+		result = libfwevt_xml_value_get_utf16_string_size_with_index(
 			  internal_xml_tag->value,
 			  value_entry_index,
 			  &value_string_size,
 			  error );
 
 		if( result == -1 )
 		{
@@ -4020,19 +3910,22 @@
 			goto on_error;
 		}
 		if( result != 0 )
 		{
 			if( ( number_of_value_entries == 1 )
 			 && ( value_string_size == 2 ) )
 			{
-				if( libfvalue_value_copy_to_utf16_string(
+				value_string_index = 0;
+
+				if( libfwevt_xml_value_copy_to_utf16_string_with_index(
 				     internal_xml_tag->value,
 				     0,
 				     static_value_string,
 				     2,
+				     &value_string_index,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 					 "%s: unable to copy element value: 0 to UTF-16 string.",
@@ -4071,19 +3964,22 @@
 					 LIBCERROR_ERROR_DOMAIN_MEMORY,
 					 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
 					 "%s: unable to create value string.",
 					 function );
 
 					goto on_error;
 				}
-				if( libfvalue_value_copy_to_utf16_string(
+				value_string_index = 0;
+
+				if( libfwevt_xml_value_copy_to_utf16_string_with_index(
 				     internal_xml_tag->value,
 				     value_entry_index,
 				     value_string,
 				     value_string_size,
+				     &value_string_index,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 					 "%s: unable to copy element value: %d to UTF-16 string.",
@@ -4096,28 +3992,28 @@
 				     value_string_index < value_string_size;
 				     value_string_index++ )
 				{
 					switch( value_string[ value_string_index ] )
 					{
 						/* Replace & by &amp; */
 						case (uint16_t) '&':
-							*utf16_string_size += 4;
+							safe_utf16_string_size += 4;
 							break;
 
 						/* Replace < by &lt; and > by &gt; */
 						case (uint16_t) '<':
 						case (uint16_t) '>':
-							*utf16_string_size += 3;
+							safe_utf16_string_size += 3;
 							break;
 
 						/* Replace ' by &apos; and " by &quot; */
 /* TODO disabled for now since Event Viewer does not uses it
 						case (uint16_t) '\'':
 						case (uint16_t) '"':
-							*utf16_string_size += 5;
+							safe_utf16_string_size += 5;
 							break;
 */
 
 						default:
 							break;
 					}
 				}
@@ -4127,25 +4023,27 @@
 				value_string = NULL;
 			}
 			if( value_string_size > 1 )
 			{
 				/* The size of:
 				 *   value formatted as a string
 				 */
-				*utf16_string_size += value_string_size - 1;
+				safe_utf16_string_size += value_string_size - 1;
 			}
 		}
 	}
-	if( *utf16_string_size != 0 )
+	if( safe_utf16_string_size != 0 )
 	{
 		/* The size of:
 		 *   end-of-string character
 		 */
-		*utf16_string_size += 1;
+		safe_utf16_string_size += 1;
 	}
+	*utf16_string_size = safe_utf16_string_size;
+
 	return( 1 );
 
 on_error:
 	if( value_string != NULL )
 	{
 		memory_free(
 		 value_string );
@@ -4215,29 +4113,29 @@
 		 "%s: invalid UTF-16 string index.",
 		 function );
 
 		return( -1 );
 	}
 	string_index = *utf16_string_index;
 
-	if( libfvalue_value_get_type(
+	if( libfwevt_xml_value_get_type(
 	     internal_xml_tag->value,
 	     &value_type,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve element value type.",
 		 function );
 
 		goto on_error;
 	}
-	if( libfvalue_value_get_number_of_value_entries(
+	if( libfwevt_xml_value_get_number_of_value_entries(
 	     internal_xml_tag->value,
 	     &number_of_value_entries,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -4247,15 +4145,15 @@
 
 		goto on_error;
 	}
 	for( value_entry_index = 0;
 	     value_entry_index < number_of_value_entries;
 	     value_entry_index++ )
 	{
-		result = libfvalue_value_get_utf16_string_size(
+		result = libfwevt_xml_value_get_utf16_string_size_with_index(
 			  internal_xml_tag->value,
 			  value_entry_index,
 			  &value_string_size,
 			  error );
 
 		if( result == -1 )
 		{
@@ -4309,19 +4207,22 @@
 					 LIBCERROR_ERROR_DOMAIN_MEMORY,
 					 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
 					 "%s: unable to create value string.",
 					 function );
 
 					goto on_error;
 				}
-				if( libfvalue_value_copy_to_utf16_string(
+				value_string_index = 0;
+
+				if( libfwevt_xml_value_copy_to_utf16_string_with_index(
 				     internal_xml_tag->value,
 				     value_entry_index,
 				     value_string,
 				     value_string_size,
+				     &value_string_index,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 					 "%s: unable to copy element value: %d to UTF-16 string.",
@@ -4465,15 +4366,15 @@
 				memory_free(
 				 value_string );
 
 				value_string = NULL;
 			}
 			else
 			{
-				if( libfvalue_value_copy_to_utf16_string_with_index(
+				if( libfwevt_xml_value_copy_to_utf16_string_with_index(
 				     internal_xml_tag->value,
 				     value_entry_index,
 				     utf16_string,
 				     utf16_string_size,
 				     &string_index,
 				     error ) != 1 )
 				{
@@ -4525,15 +4426,17 @@
      size_t *utf16_string_size,
      libcerror_error_t **error )
 {
 	libfwevt_internal_xml_tag_t *internal_attribute_xml_tag = NULL;
 	libfwevt_internal_xml_tag_t *internal_xml_tag           = NULL;
 	libfwevt_xml_tag_t *element_xml_tag                     = NULL;
 	static char *function                                   = "libfwevt_xml_tag_get_utf16_xml_string_size";
-	size_t name_size                                        = 0;
+	size_t attribute_name_size                              = 0;
+	size_t element_name_size                                = 0;
+	size_t safe_utf16_string_size                           = 0;
 	size_t string_size                                      = 0;
 	size_t value_string_size                                = 0;
 	int attribute_index                                     = 0;
 	int element_index                                       = 0;
 	int number_of_attributes                                = 0;
 	int number_of_elements                                  = 0;
 	int value_type                                          = 0;
@@ -4576,15 +4479,15 @@
 
 		return( -1 );
 	}
 	/* The size of:
 	 *   2 x ' ' character per indentation level
 	 *   1 x '<' character
 	 */
-	*utf16_string_size = ( xml_tag_level * 2 ) + 1;
+	safe_utf16_string_size = ( xml_tag_level * 2 ) + 1;
 
 	if( internal_xml_tag->type == LIBFWEVT_XML_TAG_TYPE_NODE )
 	{
 		if( libcdata_array_get_number_of_entries(
 		     internal_xml_tag->elements_array,
 		     &number_of_elements,
 		     error ) != 1 )
@@ -4594,33 +4497,34 @@
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 			 "%s: unable to retrieve number of elements.",
 			 function );
 
 			return( -1 );
 		}
-		if( libfvalue_value_get_utf16_string_size(
+		if( libuna_utf16_string_size_from_utf16_stream(
 		     internal_xml_tag->name,
-		     0,
-		     &name_size,
+		     internal_xml_tag->name_size,
+		     LIBUNA_ENDIAN_LITTLE,
+		     &element_name_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve size of UTF-16 string of name.",
+			 "%s: unable to retrieve size of UTF-16 string of element name.",
 			 function );
 
 			return( -1 );
 		}
 		/* The size of:
 		 *   element name
 		 */
-		*utf16_string_size += name_size - 1;
+		safe_utf16_string_size += element_name_size - 1;
 
 		if( number_of_attributes > 0 )
 		{
 			for( attribute_index = 0;
 			     attribute_index < number_of_attributes;
 			     attribute_index++ )
 			{
@@ -4648,18 +4552,19 @@
 					 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
 					 "%s: missing attribute: %d.",
 					 function,
 					 attribute_index );
 
 					return( -1 );
 				}
-				if( libfvalue_value_get_utf16_string_size(
+				if( libuna_utf16_string_size_from_utf16_stream(
 				     internal_attribute_xml_tag->name,
-				     0,
-				     &string_size,
+				     internal_attribute_xml_tag->name_size,
+				     LIBUNA_ENDIAN_LITTLE,
+				     &attribute_name_size,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 					 "%s: unable to retrieve UTF-16 string size of attribute: %d name.",
@@ -4670,31 +4575,31 @@
 				}
 				/* The size of:
 				 *   1 x ' ' character
 				 *   attribute name
 				 *   1 x '=' character
 				 *   1 x '"' character
 				 */
-				*utf16_string_size += string_size + 2;
+				safe_utf16_string_size += attribute_name_size + 2;
 
-				if( libfvalue_value_get_type(
+				if( libfwevt_xml_value_get_type(
 				     internal_attribute_xml_tag->value,
 				     &value_type,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 					 "%s: unable to retrieve attribute value type.",
 					 function );
 
 					return( -1 );
 				}
-				if( libfvalue_value_get_utf16_string_size(
+				if( libfwevt_xml_value_get_utf16_string_size_with_index(
 				     internal_attribute_xml_tag->value,
 				     0,
 				     &string_size,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
@@ -4706,15 +4611,15 @@
 
 					return( -1 );
 				}
 				/* The size of:
 				 *   attribute value formatted as a string
 				 *   1 x '"' character
 				 */
-				*utf16_string_size += string_size;
+				safe_utf16_string_size += string_size;
 			}
 		}
 		if( internal_xml_tag->value != NULL )
 		{
 			if( libfwevt_xml_tag_get_utf16_xml_value_string_size(
 			     internal_xml_tag,
 			     &value_string_size,
@@ -4734,22 +4639,22 @@
 				/* The size of:
 				 *   1 x '>' character
 				 *   value formatted as a string
 				 *   1 x '<' character
 				 *   1 x '/' character
 				 *   element name
 				 */
-				*utf16_string_size += value_string_size + name_size + 1;
+				safe_utf16_string_size += value_string_size + element_name_size + 1;
 			}
 			else
 			{
 				/* The size of:
 				 *   1 x '/' character
 				 */
-				*utf16_string_size += 1;
+				safe_utf16_string_size += 1;
 			}
 		}
 		else if( number_of_elements > 0 )
 		{
 			for( element_index = 0;
 			     element_index < number_of_elements;
 			     element_index++ )
@@ -4785,37 +4690,37 @@
 					 element_index );
 
 					return( -1 );
 				}
 				/* The size of:
 				 *   sub element formatted as a string
 				 */
-				*utf16_string_size += string_size - 1;
+				safe_utf16_string_size += string_size - 1;
 			}
 			/* The size of:
 			 *   1 x '>' character
 			 *   1 x '\n' character
 			 *   2 x ' ' character per indentation level
 			 *   1 x '<' character
 			 *   1 x '/' character
 			 *   element name
 			 */
-			*utf16_string_size += ( xml_tag_level * 2 ) + name_size + 3;
+			safe_utf16_string_size += ( xml_tag_level * 2 ) + element_name_size + 3;
 		}
 		else
 		{
 			/* The size of:
 			 *   1 x '/' character
 			 */
-			*utf16_string_size += 1;
+			safe_utf16_string_size += 1;
 		}
 	}
 	else if( internal_xml_tag->type == LIBFWEVT_XML_TAG_TYPE_CDATA )
 	{
-		if( libfvalue_value_get_utf16_string_size(
+		if( libfwevt_xml_value_get_utf16_string_size_with_index(
 		     internal_xml_tag->value,
 		     0,
 		     &string_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
@@ -4827,40 +4732,41 @@
 			return( -1 );
 		}
 		/* The size of:
 		 *   1 x "![CDATA["
 		 *   value formatted as a string
 		 *   1 x "]]"
 		 */
-		*utf16_string_size += string_size + 9;
+		safe_utf16_string_size += string_size + 9;
 	}
 	else if( internal_xml_tag->type == LIBFWEVT_XML_TAG_TYPE_PI )
 	{
-		if( libfvalue_value_get_utf16_string_size(
+		if( libuna_utf16_string_size_from_utf16_stream(
 		     internal_xml_tag->name,
-		     0,
-		     &name_size,
+		     internal_xml_tag->name_size,
+		     LIBUNA_ENDIAN_LITTLE,
+		     &element_name_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-			 "%s: unable to retrieve UTF-16 string size of name.",
+			 "%s: unable to retrieve UTF-16 string size of element name.",
 			 function );
 
 			return( -1 );
 		}
 		/* The size of:
 		 *   1 x '?' character
 		 *   element name
 		 */
-		*utf16_string_size += name_size;
+		safe_utf16_string_size += element_name_size;
 
-		if( libfvalue_value_get_utf16_string_size(
+		if( libfwevt_xml_value_get_utf16_string_size_with_index(
 		     internal_xml_tag->value,
 		     0,
 		     &string_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
@@ -4872,22 +4778,24 @@
 			return( -1 );
 		}
 		/* The size of:
 		 *   1 x ' ' character
 		 *   element name
 		 *   1 x '?' character
 		 */
-		*utf16_string_size += string_size + 1;
+		safe_utf16_string_size += string_size + 1;
 	}
 	/* The size of:
 	 *   1 x '>' character
 	 *   1 x '\n' character
 	 *   1 x '\0' character
 	 */
-	*utf16_string_size += 3;
+	safe_utf16_string_size += 3;
+
+	*utf16_string_size = safe_utf16_string_size;
 
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 formatted string of the XML tag
  * Returns 1 if successful or -1 on error
  */
@@ -5006,20 +4914,21 @@
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 			 "%s: unable to retrieve number of elements.",
 			 function );
 
 			return( -1 );
 		}
-		if( libfvalue_value_copy_to_utf16_string_with_index(
-		     internal_xml_tag->name,
-		     0,
+		if( libuna_utf16_string_with_index_copy_from_utf16_stream(
 		     utf16_string,
 		     utf16_string_size,
 		     &string_index,
+		     internal_xml_tag->name,
+		     internal_xml_tag->name_size,
+		     LIBUNA_ENDIAN_LITTLE,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 			 "%s: unable to copy name to UTF-16 string.",
@@ -5072,20 +4981,21 @@
 					 "%s: UTF-16 string size too small.",
 					 function );
 
 					return( -1 );
 				}
 				utf16_string[ string_index++ ] = (uint16_t) ' ';
 
-				if( libfvalue_value_copy_to_utf16_string_with_index(
-				     internal_attribute_xml_tag->name,
-				     0,
+				if( libuna_utf16_string_with_index_copy_from_utf16_stream(
 				     utf16_string,
 				     utf16_string_size,
 				     &string_index,
+				     internal_attribute_xml_tag->name,
+				     internal_attribute_xml_tag->name_size,
+				     LIBUNA_ENDIAN_LITTLE,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 					 "%s: unable to copy attribute: %d name to UTF-16 string.",
@@ -5106,29 +5016,29 @@
 					 function );
 
 					return( -1 );
 				}
 				utf16_string[ string_index++ ] = (uint16_t) '=';
 				utf16_string[ string_index++ ] = (uint16_t) '"';
 
-				if( libfvalue_value_get_type(
+				if( libfwevt_xml_value_get_type(
 				     internal_attribute_xml_tag->value,
 				     &value_type,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 					 "%s: unable to retrieve attribute value type.",
 					 function );
 
 					return( -1 );
 				}
-				if( libfvalue_value_copy_to_utf16_string_with_index(
+				if( libfwevt_xml_value_copy_to_utf16_string_with_index(
 				     internal_attribute_xml_tag->value,
 				     0,
 				     utf16_string,
 				     utf16_string_size,
 				     &string_index,
 				     error ) != 1 )
 				{
@@ -5217,20 +5127,21 @@
 					 function );
 
 					return( -1 );
 				}
 				utf16_string[ string_index++ ] = (uint16_t) '<';
 				utf16_string[ string_index++ ] = (uint16_t) '/';
 
-				if( libfvalue_value_copy_to_utf16_string_with_index(
-				     internal_xml_tag->name,
-				     0,
+				if( libuna_utf16_string_with_index_copy_from_utf16_stream(
 				     utf16_string,
 				     utf16_string_size,
 				     &string_index,
+				     internal_xml_tag->name,
+				     internal_xml_tag->name_size,
+				     LIBUNA_ENDIAN_LITTLE,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 					 "%s: unable to copy name to UTF-16 string.",
@@ -5340,20 +5251,21 @@
 				 function );
 
 				return( -1 );
 			}
 			utf16_string[ string_index++ ] = (uint16_t) '<';
 			utf16_string[ string_index++ ] = (uint16_t) '/';
 
-			if( libfvalue_value_copy_to_utf16_string_with_index(
-			     internal_xml_tag->name,
-			     0,
+			if( libuna_utf16_string_with_index_copy_from_utf16_stream(
 			     utf16_string,
 			     utf16_string_size,
 			     &string_index,
+			     internal_xml_tag->name,
+			     internal_xml_tag->name_size,
+			     LIBUNA_ENDIAN_LITTLE,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 				 "%s: unable to copy name to UTF-16 string.",
@@ -5408,15 +5320,15 @@
 		utf16_string[ string_index++ ] = (uint16_t) 'C';
 		utf16_string[ string_index++ ] = (uint16_t) 'D';
 		utf16_string[ string_index++ ] = (uint16_t) 'A';
 		utf16_string[ string_index++ ] = (uint16_t) 'T';
 		utf16_string[ string_index++ ] = (uint16_t) 'A';
 		utf16_string[ string_index++ ] = (uint16_t) '[';
 
-		if( libfvalue_value_copy_to_utf16_string_with_index(
+		if( libfwevt_xml_value_copy_to_utf16_string_with_index(
 		     internal_xml_tag->value,
 		     0,
 		     utf16_string,
 		     utf16_string_size,
 		     &string_index,
 		     error ) != 1 )
 		{
@@ -5456,20 +5368,21 @@
 			 "%s: UTF-16 string size too small.",
 			 function );
 
 			return( -1 );
 		}
 		utf16_string[ string_index++ ] = (uint16_t) '?';
 
-		if( libfvalue_value_copy_to_utf16_string_with_index(
-		     internal_xml_tag->name,
-		     0,
+		if( libuna_utf16_string_with_index_copy_from_utf16_stream(
 		     utf16_string,
 		     utf16_string_size,
 		     &string_index,
+		     internal_xml_tag->name,
+		     internal_xml_tag->name_size,
+		     LIBUNA_ENDIAN_LITTLE,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
 			 "%s: unable to copy name to UTF-16 string.",
@@ -5488,15 +5401,15 @@
 			 "%s: UTF-16 string size too small.",
 			 function );
 
 			return( -1 );
 		}
 		utf16_string[ string_index++ ] = (uint16_t) ' ';
 
-		if( libfvalue_value_copy_to_utf16_string_with_index(
+		if( libfwevt_xml_value_copy_to_utf16_string_with_index(
 		     internal_xml_tag->value,
 		     0,
 		     utf16_string,
 		     utf16_string_size,
 		     &string_index,
 		     error ) != 1 )
 		{
@@ -5531,14 +5444,134 @@
 	*utf16_string_index = string_index;
 
 	return( 1 );
 }
 
 #if defined( HAVE_DEBUG_OUTPUT )
 
+/* Debug prints the name
+ * Returns 1 if successful or -1 on error
+ */
+int libfwevt_xml_tag_debug_print_name_string(
+     libfwevt_internal_xml_tag_t *internal_xml_tag,
+     libcerror_error_t **error )
+{
+	system_character_t *name_string = NULL;
+	static char *function           = "libfwevt_xml_tag_debug_print_name_string";
+	size_t name_string_size         = 0;
+	int result                      = 0;
+
+	if( internal_xml_tag == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid XML tag.",
+		 function );
+
+		return( -1 );
+	}
+#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+	result = libuna_utf16_string_size_from_utf16_stream(
+		  internal_xml_tag->name,
+		  internal_xml_tag->name_size,
+		  LIBUNA_ENDIAN_LITTLE,
+		  &name_string_size,
+		  error );
+#else
+	result = libuna_utf8_string_size_from_utf16_stream(
+		  internal_xml_tag->name,
+		  internal_xml_tag->name_size,
+		  LIBUNA_ENDIAN_LITTLE,
+		  &name_string_size,
+		  error );
+#endif
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to determine size of name string.",
+		 function );
+
+		goto on_error;
+	}
+	if( name_string_size > (size_t) ( SSIZE_MAX / sizeof( system_character_t ) ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid name string size value exceeds maximum.",
+		 function );
+
+		goto on_error;
+	}
+	name_string = system_string_allocate(
+	               name_string_size );
+
+	if( name_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_MEMORY,
+		 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+		 "%s: unable to create name string.",
+		 function );
+
+		goto on_error;
+	}
+#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+	result = libuna_utf16_string_copy_from_utf16_stream(
+		  (libuna_utf16_character_t *) name_string,
+		  name_string_size,
+		  internal_xml_tag->name,
+		  internal_xml_tag->name_size,
+		  LIBUNA_ENDIAN_LITTLE,
+		  error );
+#else
+	result = libuna_utf8_string_copy_from_utf16_stream(
+		  (libuna_utf8_character_t *) name_string,
+		  name_string_size,
+		  internal_xml_tag->name,
+		  internal_xml_tag->name_size,
+		  LIBUNA_ENDIAN_LITTLE,
+		  error );
+#endif
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+		 "%s: unable to set name string.",
+		 function );
+
+		goto on_error;
+	}
+	libcnotify_printf(
+	 "%" PRIs_SYSTEM "",
+	 name_string );
+
+	memory_free(
+	 name_string );
+
+	return( 1 );
+
+on_error:
+	if( name_string != NULL )
+	{
+		memory_free(
+		 name_string );
+	}
+	return( -1 );
+}
+
 /* Debug prints the XML value
  * Returns 1 if successful or -1 on error
  */
 int libfwevt_xml_tag_debug_print_value_string(
      libfwevt_internal_xml_tag_t *internal_xml_tag,
      libcerror_error_t **error )
 {
@@ -5558,29 +5591,29 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid XML tag.",
 		 function );
 
 		return( -1 );
 	}
-	if( libfvalue_value_get_type(
+	if( libfwevt_xml_value_get_type(
 	     internal_xml_tag->value,
 	     &value_type,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve element value type.",
 		 function );
 
 		goto on_error;
 	}
-	if( libfvalue_value_get_number_of_value_entries(
+	if( libfwevt_xml_value_get_number_of_value_entries(
 	     internal_xml_tag->value,
 	     &number_of_value_entries,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -5591,21 +5624,21 @@
 		goto on_error;
 	}
 	for( value_entry_index = 0;
 	     value_entry_index < number_of_value_entries;
 	     value_entry_index++ )
 	{
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-		result = libfvalue_value_get_utf16_string_size(
+		result = libfwevt_xml_value_get_utf16_string_size_with_index(
 			  internal_xml_tag->value,
 			  value_entry_index,
 			  &value_string_size,
 			  error );
 #else
-		result = libfvalue_value_get_utf8_string_size(
+		result = libfwevt_xml_value_get_utf8_string_size_with_index(
 			  internal_xml_tag->value,
 			  value_entry_index,
 			  &value_string_size,
 			  error );
 #endif
 		if( result == -1 )
 		{
@@ -5646,27 +5679,31 @@
 					 LIBCERROR_ERROR_DOMAIN_MEMORY,
 					 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
 					 "%s: unable to create value string.",
 					 function );
 
 					goto on_error;
 				}
+				value_string_index = 0;
+
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-				result = libfvalue_value_copy_to_utf16_string(
+				result = libfwevt_xml_value_copy_to_utf16_string_with_index(
 				          internal_xml_tag->value,
 				          value_entry_index,
 				          (uint16_t *) value_string,
 				          value_string_size,
+				          &value_string_index,
 				          error );
 #else
-				result = libfvalue_value_copy_to_utf8_string(
+				result = libfwevt_xml_value_copy_to_utf8_string_with_index(
 				          internal_xml_tag->value,
 				          value_entry_index,
 				          (uint8_t *) value_string,
 				          value_string_size,
+				          &value_string_index,
 				          error );
 #endif
 				if( result != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -5733,15 +5770,15 @@
 				memory_free(
 				 value_string );
 
 				value_string = NULL;
 			}
 			else
 			{
-				if( libfvalue_value_print(
+				if( libfwevt_debug_print_xml_value(
 				     internal_xml_tag->value,
 				     value_entry_index,
 				     0,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
@@ -5835,18 +5872,16 @@
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 			 "%s: unable to retrieve number of elements.",
 			 function );
 
 			return( -1 );
 		}
-		if( libfvalue_value_print(
-		     internal_xml_tag->name,
-		     0,
-		     0,
+		if( libfwevt_xml_tag_debug_print_name_string(
+		     internal_xml_tag,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
 			 "%s: unable to print name.",
@@ -5887,47 +5922,45 @@
 					 attribute_index );
 
 					return( -1 );
 				}
 				libcnotify_printf(
 				 " " );
 
-				if( libfvalue_value_print(
-				     internal_attribute_xml_tag->name,
-				     0,
-				     0,
+				if( libfwevt_xml_tag_debug_print_name_string(
+				     internal_attribute_xml_tag,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
 					 "%s: unable to print attribute name.",
 					 function );
 
 					return( -1 );
 				}
 				libcnotify_printf(
 				 "=\"" );
 
-				if( libfvalue_value_get_type(
+				if( libfwevt_xml_value_get_type(
 				     internal_attribute_xml_tag->value,
 				     &value_type,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 					 "%s: unable to retrieve attribute value type.",
 					 function );
 
 					return( -1 );
 				}
-				if( libfvalue_value_print(
+				if( libfwevt_debug_print_xml_value(
 				     internal_attribute_xml_tag->value,
 				     0,
 				     0,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
@@ -5975,18 +6008,16 @@
 					 function );
 
 					return( -1 );
 				}
 				libcnotify_printf(
 				 "</" );
 
-				if( libfvalue_value_print(
-				     internal_xml_tag->name,
-				     0,
-				     0,
+				if( libfwevt_xml_tag_debug_print_name_string(
+				     internal_xml_tag,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
 					 "%s: unable to print name.",
@@ -6048,18 +6079,16 @@
 			{
 				libcnotify_printf(
 				 "  " );
 			}
 			libcnotify_printf(
 			 "</" );
 
-			if( libfvalue_value_print(
-			     internal_xml_tag->name,
-			     0,
-			     0,
+			if( libfwevt_xml_tag_debug_print_name_string(
+			     internal_xml_tag,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
 				 "%s: unable to print name.",
@@ -6075,15 +6104,15 @@
 		}
 	}
 	else if( internal_xml_tag->type == LIBFWEVT_XML_TAG_TYPE_CDATA )
 	{
 		libcnotify_printf(
 		 "![CDATA[" );
 
-		if( libfvalue_value_print(
+		if( libfwevt_debug_print_xml_value(
 		     internal_xml_tag->value,
 		     0,
 		     0,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
@@ -6098,33 +6127,31 @@
 		 "]]" );
 	}
 	else if( internal_xml_tag->type == LIBFWEVT_XML_TAG_TYPE_PI )
 	{
 		libcnotify_printf(
 		 "?" );
 
-		if( libfvalue_value_print(
-		     internal_xml_tag->name,
-		     0,
-		     0,
+		if( libfwevt_xml_tag_debug_print_name_string(
+		     internal_xml_tag,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
 			 "%s: unable to print name.",
 			 function );
 
 			return( -1 );
 		}
 		libcnotify_printf(
 		 " " );
 
-		if( libfvalue_value_print(
+		if( libfwevt_debug_print_xml_value(
 		     internal_xml_tag->value,
 		     0,
 		     0,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
@@ -6167,18 +6194,16 @@
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
 	libcnotify_printf(
 	 "%s: name\t\t\t\t\t: ",
 	 function );
 
-	if( libfvalue_value_print(
-	     internal_xml_tag->name,
-	     0,
-	     0,
+	if( libfwevt_xml_tag_debug_print_name_string(
+	     internal_xml_tag,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
 		 "%s: unable to print name.",
@@ -6219,15 +6244,15 @@
 	}
 	internal_xml_tag = (libfwevt_internal_xml_tag_t *) xml_tag;
 
 	libcnotify_printf(
 	 "%s: value\t\t\t\t: ",
 	 function );
 
-	if( libfvalue_value_print(
+	if( libfwevt_debug_print_xml_value(
 	     internal_xml_tag->value,
 	     value_entry_index,
 	     0,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
```

### Comparing `libfwevt-20240419/libfwevt/libfwevt_libcnotify.h` & `libfwevt-20240426/libfwevt/libfwevt_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_level.c` & `libfwevt-20240426/libfwevt/libfwevt_level.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_notify.h` & `libfwevt-20240426/libfwevt/libfwevt_notify.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_libfguid.h` & `libfwevt-20240426/libfwevt/libfwevt_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_libcdata.h` & `libfwevt-20240426/libfwevt/libfwevt_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_xml_token.h` & `libfwevt-20240426/libfwevt/libfwevt_xml_token.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_error.h` & `libfwevt-20240426/libfwevt/libfwevt_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/fwevt_template.h` & `libfwevt-20240426/libfwevt/fwevt_template.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_opcode.h` & `libfwevt-20240426/libfwevt/libfwevt_opcode.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt.c` & `libfwevt-20240426/libfwevt/libfwevt.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_xml_token.c` & `libfwevt-20240426/libfwevt/libfwevt_xml_token.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/Makefile.in` & `libfwevt-20240426/libfwevt/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,16 @@
 am_libfwevt_la_OBJECTS = libfwevt.lo libfwevt_channel.lo \
 	libfwevt_debug.lo libfwevt_error.lo libfwevt_event.lo \
 	libfwevt_keyword.lo libfwevt_level.lo libfwevt_manifest.lo \
 	libfwevt_map.lo libfwevt_notify.lo libfwevt_opcode.lo \
 	libfwevt_provider.lo libfwevt_support.lo libfwevt_task.lo \
 	libfwevt_template.lo libfwevt_template_item.lo \
 	libfwevt_xml_document.lo libfwevt_xml_tag.lo \
-	libfwevt_xml_template_value.lo libfwevt_xml_token.lo
+	libfwevt_xml_template_value.lo libfwevt_xml_token.lo \
+	libfwevt_xml_value.lo
 libfwevt_la_OBJECTS = $(am_libfwevt_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
 libfwevt_la_LINK = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=link $(CCLD) $(AM_CFLAGS) $(CFLAGS) \
@@ -186,15 +187,16 @@
 	./$(DEPDIR)/libfwevt_provider.Plo \
 	./$(DEPDIR)/libfwevt_support.Plo ./$(DEPDIR)/libfwevt_task.Plo \
 	./$(DEPDIR)/libfwevt_template.Plo \
 	./$(DEPDIR)/libfwevt_template_item.Plo \
 	./$(DEPDIR)/libfwevt_xml_document.Plo \
 	./$(DEPDIR)/libfwevt_xml_tag.Plo \
 	./$(DEPDIR)/libfwevt_xml_template_value.Plo \
-	./$(DEPDIR)/libfwevt_xml_token.Plo
+	./$(DEPDIR)/libfwevt_xml_token.Plo \
+	./$(DEPDIR)/libfwevt_xml_value.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
 	$(AM_CFLAGS) $(CFLAGS)
@@ -533,15 +535,16 @@
 	libfwevt_template.c libfwevt_template.h \
 	libfwevt_template_item.c libfwevt_template_item.h \
 	libfwevt_types.h \
 	libfwevt_unused.h \
 	libfwevt_xml_document.c libfwevt_xml_document.h \
 	libfwevt_xml_tag.c libfwevt_xml_tag.h \
 	libfwevt_xml_template_value.c libfwevt_xml_template_value.h \
-	libfwevt_xml_token.c libfwevt_xml_token.h
+	libfwevt_xml_token.c libfwevt_xml_token.h \
+	libfwevt_xml_value.c libfwevt_xml_value.h
 
 libfwevt_la_LIBADD = \
 	@LIBCERROR_LIBADD@ \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBUNA_LIBADD@ \
@@ -660,14 +663,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwevt_task.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwevt_template.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwevt_template_item.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwevt_xml_document.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwevt_xml_tag.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwevt_xml_template_value.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwevt_xml_token.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwevt_xml_value.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
 
@@ -844,14 +848,15 @@
 	-rm -f ./$(DEPDIR)/libfwevt_task.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_template.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_template_item.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_xml_document.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_xml_tag.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_xml_template_value.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_xml_token.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_xml_value.Plo
 	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
@@ -909,14 +914,15 @@
 	-rm -f ./$(DEPDIR)/libfwevt_task.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_template.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_template_item.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_xml_document.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_xml_tag.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_xml_template_value.Plo
 	-rm -f ./$(DEPDIR)/libfwevt_xml_token.Plo
+	-rm -f ./$(DEPDIR)/libfwevt_xml_value.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
 	mostlyclean-libtool
```

### Comparing `libfwevt-20240419/libfwevt/libfwevt_libcerror.h` & `libfwevt-20240426/libfwevt/libfwevt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_extern.h` & `libfwevt-20240426/libfwevt/libfwevt_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_keyword.h` & `libfwevt-20240426/libfwevt/libfwevt_keyword.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_debug.c` & `libfwevt-20240426/libfwevt/libfwevt_debug.c`

 * *Files 1% similar despite different names*

```diff
@@ -662,15 +662,15 @@
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
 		 "%s: unable to set string.",
 		 function );
 
 		goto on_error;
 	}
 	libcnotify_printf(
-	 "%s: %s: %s\n",
+	 "%s: %s: %" PRIs_SYSTEM "\n",
 	 function_name,
 	 value_name,
 	 string );
 
 	memory_free(
 	 string );
```

### Comparing `libfwevt-20240419/libfwevt/libfwevt_error.c` & `libfwevt-20240426/libfwevt/libfwevt_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_xml_template_value.c` & `libfwevt-20240426/libfwevt/libfwevt_xml_template_value.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt/libfwevt_template.c` & `libfwevt-20240426/libfwevt/libfwevt_template.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_template.c` & `libfwevt-20240426/pyfwevt/pyfwevt_template.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_tasks.c` & `libfwevt-20240426/pyfwevt/pyfwevt_tasks.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_level.c` & `libfwevt-20240426/pyfwevt/pyfwevt_level.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_template_item.h` & `libfwevt-20240426/pyfwevt/pyfwevt_template_item.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_providers.c` & `libfwevt-20240426/pyfwevt/pyfwevt_providers.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_providers.h` & `libfwevt-20240426/pyfwevt/pyfwevt_providers.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_provider.c` & `libfwevt-20240426/pyfwevt/pyfwevt_provider.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_map.c` & `libfwevt-20240426/pyfwevt/pyfwevt_map.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_maps.h` & `libfwevt-20240426/pyfwevt/pyfwevt_maps.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_tasks.h` & `libfwevt-20240426/pyfwevt/pyfwevt_tasks.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_libfguid.h` & `libfwevt-20240426/pyfwevt/pyfwevt_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_integer.h` & `libfwevt-20240426/pyfwevt/pyfwevt_integer.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_unused.h` & `libfwevt-20240426/pyfwevt/pyfwevt_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_error.c` & `libfwevt-20240426/pyfwevt/pyfwevt_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_opcodes.h` & `libfwevt-20240426/pyfwevt/pyfwevt_opcodes.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_channels.h` & `libfwevt-20240426/pyfwevt/pyfwevt_channels.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_event.h` & `libfwevt-20240426/pyfwevt/pyfwevt_event.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_opcode.c` & `libfwevt-20240426/pyfwevt/pyfwevt_opcode.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/Makefile.am` & `libfwevt-20240426/pyfwevt/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_python.h` & `libfwevt-20240426/pyfwevt/pyfwevt_python.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_levels.c` & `libfwevt-20240426/pyfwevt/pyfwevt_levels.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_template.h` & `libfwevt-20240426/pyfwevt/pyfwevt_template.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_channel.h` & `libfwevt-20240426/pyfwevt/pyfwevt_channel.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_opcodes.c` & `libfwevt-20240426/pyfwevt/pyfwevt_opcodes.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_keywords.c` & `libfwevt-20240426/pyfwevt/pyfwevt_keywords.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_libcerror.h` & `libfwevt-20240426/pyfwevt/pyfwevt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_maps.c` & `libfwevt-20240426/pyfwevt/pyfwevt_maps.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_level.h` & `libfwevt-20240426/pyfwevt/pyfwevt_level.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt.h` & `libfwevt-20240426/pyfwevt/pyfwevt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_events.h` & `libfwevt-20240426/pyfwevt/pyfwevt_events.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_events.c` & `libfwevt-20240426/pyfwevt/pyfwevt_events.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt.c` & `libfwevt-20240426/pyfwevt/pyfwevt.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_provider.h` & `libfwevt-20240426/pyfwevt/pyfwevt_provider.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_keywords.h` & `libfwevt-20240426/pyfwevt/pyfwevt_keywords.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_manifest.c` & `libfwevt-20240426/pyfwevt/pyfwevt_manifest.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_keyword.h` & `libfwevt-20240426/pyfwevt/pyfwevt_keyword.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_task.c` & `libfwevt-20240426/pyfwevt/pyfwevt_task.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_error.h` & `libfwevt-20240426/pyfwevt/pyfwevt_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_map.h` & `libfwevt-20240426/pyfwevt/pyfwevt_map.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_template_item.c` & `libfwevt-20240426/pyfwevt/pyfwevt_template_item.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_templates.h` & `libfwevt-20240426/pyfwevt/pyfwevt_templates.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_keyword.c` & `libfwevt-20240426/pyfwevt/pyfwevt_keyword.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_task.h` & `libfwevt-20240426/pyfwevt/pyfwevt_task.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_template_items.h` & `libfwevt-20240426/pyfwevt/pyfwevt_template_items.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_opcode.h` & `libfwevt-20240426/pyfwevt/pyfwevt_opcode.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_levels.h` & `libfwevt-20240426/pyfwevt/pyfwevt_levels.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_template_items.c` & `libfwevt-20240426/pyfwevt/pyfwevt_template_items.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/Makefile.in` & `libfwevt-20240426/pyfwevt/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_manifest.h` & `libfwevt-20240426/pyfwevt/pyfwevt_manifest.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_guid.h` & `libfwevt-20240426/pyfwevt/pyfwevt_guid.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_channel.c` & `libfwevt-20240426/pyfwevt/pyfwevt_channel.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_event.c` & `libfwevt-20240426/pyfwevt/pyfwevt_event.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_templates.c` & `libfwevt-20240426/pyfwevt/pyfwevt_templates.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_channels.c` & `libfwevt-20240426/pyfwevt/pyfwevt_channels.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_integer.c` & `libfwevt-20240426/pyfwevt/pyfwevt_integer.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_guid.c` & `libfwevt-20240426/pyfwevt/pyfwevt_guid.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/pyfwevt/pyfwevt_libfwevt.h` & `libfwevt-20240426/pyfwevt/pyfwevt_libfwevt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_level/fwevt_test_level.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_level/fwevt_test_level.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_provider/fwevt_test_provider.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/libfguid/libfguid.vcproj` & `libfwevt-20240426/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_xml_document/fwevt_test_xml_document.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/Makefile.am` & `libfwevt-20240426/msvscpp/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	fwevt_test_task/fwevt_test_task.vcproj \
 	fwevt_test_template/fwevt_test_template.vcproj \
 	fwevt_test_template_item/fwevt_test_template_item.vcproj \
 	fwevt_test_xml_document/fwevt_test_xml_document.vcproj \
 	fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj \
 	fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj \
 	fwevt_test_xml_token/fwevt_test_xml_token.vcproj \
+	fwevt_test_xml_value/fwevt_test_xml_value.vcproj \
 	libcdata/libcdata.vcproj \
 	libcerror/libcerror.vcproj \
 	libcnotify/libcnotify.vcproj \
 	libcthreads/libcthreads.vcproj \
 	libfdatetime/libfdatetime.vcproj \
 	libfguid/libfguid.vcproj \
 	libfvalue/libfvalue.vcproj \
```

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_event/fwevt_test_event.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_event/fwevt_test_event.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/libfwevt/libfwevt.vcproj` & `libfwevt-20240426/msvscpp/libfwevt/libfwevt.vcproj`

 * *Files 2% similar despite different names*

#### Comparing `libfwevt-20240419/msvscpp/libfwevt/libfwevt.vcproj` & `libfwevt-20240426/msvscpp/libfwevt/libfwevt.vcproj`

```diff
@@ -63,14 +63,15 @@
       <File RelativePath="..\..\libfwevt\libfwevt_task.c"/>
       <File RelativePath="..\..\libfwevt\libfwevt_template.c"/>
       <File RelativePath="..\..\libfwevt\libfwevt_template_item.c"/>
       <File RelativePath="..\..\libfwevt\libfwevt_xml_document.c"/>
       <File RelativePath="..\..\libfwevt\libfwevt_xml_tag.c"/>
       <File RelativePath="..\..\libfwevt\libfwevt_xml_template_value.c"/>
       <File RelativePath="..\..\libfwevt\libfwevt_xml_token.c"/>
+      <File RelativePath="..\..\libfwevt\libfwevt_xml_value.c"/>
     </Filter>
     <Filter Name="Header Files" Filter="h;hpp;hxx;hm;inl;inc;xsd" UniqueIdentifier="{93995380-89BD-4b04-88EB-625FBE52EBFB}">
       <File RelativePath="..\..\libfwevt\fwevt_template.h"/>
       <File RelativePath="..\..\libfwevt\libfwevt_channel.h"/>
       <File RelativePath="..\..\libfwevt\libfwevt_debug.h"/>
       <File RelativePath="..\..\libfwevt\libfwevt_definitions.h"/>
       <File RelativePath="..\..\libfwevt\libfwevt_error.h"/>
@@ -95,14 +96,15 @@
       <File RelativePath="..\..\libfwevt\libfwevt_template_item.h"/>
       <File RelativePath="..\..\libfwevt\libfwevt_types.h"/>
       <File RelativePath="..\..\libfwevt\libfwevt_unused.h"/>
       <File RelativePath="..\..\libfwevt\libfwevt_xml_document.h"/>
       <File RelativePath="..\..\libfwevt\libfwevt_xml_tag.h"/>
       <File RelativePath="..\..\libfwevt\libfwevt_xml_template_value.h"/>
       <File RelativePath="..\..\libfwevt\libfwevt_xml_token.h"/>
+      <File RelativePath="..\..\libfwevt\libfwevt_xml_value.h"/>
     </Filter>
     <Filter Name="Resource Files" Filter="rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav" UniqueIdentifier="{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}">
       <File RelativePath="..\..\libfwevt\libfwevt.rc"/>
     </Filter>
   </Files>
   <Globals/>
 </VisualStudioProject>
```

### Comparing `libfwevt-20240419/msvscpp/libfwevt.sln` & `libfwevt-20240426/msvscpp/libfwevt.sln`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,20 @@
 EndProject
 Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "fwevt_test_xml_token", "fwevt_test_xml_token\fwevt_test_xml_token.vcproj", "{6AEB4E37-792D-490D-95A5-1A855C166C1B}"
 	ProjectSection(ProjectDependencies) = postProject
 		{B97706AC-46E5-4C2A-836E-582A74DC6A68} = {B97706AC-46E5-4C2A-836E-582A74DC6A68}
 		{C5D33EBC-535D-474C-870A-B96A4B30850D} = {C5D33EBC-535D-474C-870A-B96A4B30850D}
 	EndProjectSection
 EndProject
+Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "fwevt_test_xml_value", "fwevt_test_xml_value\fwevt_test_xml_value.vcproj", "{703A33A3-1A6A-4D9C-B25F-F84BE52BAEA3}"
+	ProjectSection(ProjectDependencies) = postProject
+		{B97706AC-46E5-4C2A-836E-582A74DC6A68} = {B97706AC-46E5-4C2A-836E-582A74DC6A68}
+		{C5D33EBC-535D-474C-870A-B96A4B30850D} = {C5D33EBC-535D-474C-870A-B96A4B30850D}
+	EndProjectSection
+EndProject
 Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "libuna", "libuna\libuna.vcproj", "{5C6EAD13-CCA8-4B03-8495-EEE2E3092468}"
 	ProjectSection(ProjectDependencies) = postProject
 		{C5D33EBC-535D-474C-870A-B96A4B30850D} = {C5D33EBC-535D-474C-870A-B96A4B30850D}
 	EndProjectSection
 EndProject
 Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "libfvalue", "libfvalue\libfvalue.vcproj", "{4A81A573-8E94-4C37-96C6-AAB627CA2D9B}"
 	ProjectSection(ProjectDependencies) = postProject
@@ -265,14 +271,18 @@
 		{87326EB9-F85E-43C8-A8D0-8138CF9B8712}.Release|Win32.Build.0 = Release|Win32
 		{87326EB9-F85E-43C8-A8D0-8138CF9B8712}.VSDebug|Win32.ActiveCfg = VSDebug|Win32
 		{87326EB9-F85E-43C8-A8D0-8138CF9B8712}.VSDebug|Win32.Build.0 = VSDebug|Win32
 		{6AEB4E37-792D-490D-95A5-1A855C166C1B}.Release|Win32.ActiveCfg = Release|Win32
 		{6AEB4E37-792D-490D-95A5-1A855C166C1B}.Release|Win32.Build.0 = Release|Win32
 		{6AEB4E37-792D-490D-95A5-1A855C166C1B}.VSDebug|Win32.ActiveCfg = VSDebug|Win32
 		{6AEB4E37-792D-490D-95A5-1A855C166C1B}.VSDebug|Win32.Build.0 = VSDebug|Win32
+		{703A33A3-1A6A-4D9C-B25F-F84BE52BAEA3}.Release|Win32.ActiveCfg = Release|Win32
+		{703A33A3-1A6A-4D9C-B25F-F84BE52BAEA3}.Release|Win32.Build.0 = Release|Win32
+		{703A33A3-1A6A-4D9C-B25F-F84BE52BAEA3}.VSDebug|Win32.ActiveCfg = VSDebug|Win32
+		{703A33A3-1A6A-4D9C-B25F-F84BE52BAEA3}.VSDebug|Win32.Build.0 = VSDebug|Win32
 		{5C6EAD13-CCA8-4B03-8495-EEE2E3092468}.Release|Win32.ActiveCfg = Release|Win32
 		{5C6EAD13-CCA8-4B03-8495-EEE2E3092468}.Release|Win32.Build.0 = Release|Win32
 		{5C6EAD13-CCA8-4B03-8495-EEE2E3092468}.VSDebug|Win32.ActiveCfg = VSDebug|Win32
 		{5C6EAD13-CCA8-4B03-8495-EEE2E3092468}.VSDebug|Win32.Build.0 = VSDebug|Win32
 		{4A81A573-8E94-4C37-96C6-AAB627CA2D9B}.Release|Win32.ActiveCfg = Release|Win32
 		{4A81A573-8E94-4C37-96C6-AAB627CA2D9B}.Release|Win32.Build.0 = Release|Win32
 		{4A81A573-8E94-4C37-96C6-AAB627CA2D9B}.VSDebug|Win32.ActiveCfg = VSDebug|Win32
```

### Comparing `libfwevt-20240419/msvscpp/pyfwevt/pyfwevt.vcproj` & `libfwevt-20240426/msvscpp/pyfwevt/pyfwevt.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_template/fwevt_test_template.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_template/fwevt_test_template.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_keyword/fwevt_test_keyword.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_opcode/fwevt_test_opcode.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_manifest/fwevt_test_manifest.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_template_item/fwevt_test_template_item.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_template_item/fwevt_test_template_item.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/libcdata/libcdata.vcproj` & `libfwevt-20240426/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_channel/fwevt_test_channel.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_error/fwevt_test_error.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_error/fwevt_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_task/fwevt_test_task.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_task/fwevt_test_task.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/libcthreads/libcthreads.vcproj` & `libfwevt-20240426/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_notify/fwevt_test_notify.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_notify/fwevt_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_xml_token/fwevt_test_xml_token.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/libuna/libuna.vcproj` & `libfwevt-20240426/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/Makefile.in` & `libfwevt-20240426/msvscpp/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -403,14 +403,15 @@
 	fwevt_test_task/fwevt_test_task.vcproj \
 	fwevt_test_template/fwevt_test_template.vcproj \
 	fwevt_test_template_item/fwevt_test_template_item.vcproj \
 	fwevt_test_xml_document/fwevt_test_xml_document.vcproj \
 	fwevt_test_xml_tag/fwevt_test_xml_tag.vcproj \
 	fwevt_test_xml_template_value/fwevt_test_xml_template_value.vcproj \
 	fwevt_test_xml_token/fwevt_test_xml_token.vcproj \
+	fwevt_test_xml_value/fwevt_test_xml_value.vcproj \
 	libcdata/libcdata.vcproj \
 	libcerror/libcerror.vcproj \
 	libcnotify/libcnotify.vcproj \
 	libcthreads/libcthreads.vcproj \
 	libfdatetime/libfdatetime.vcproj \
 	libfguid/libfguid.vcproj \
 	libfvalue/libfvalue.vcproj \
```

### Comparing `libfwevt-20240419/msvscpp/libfvalue/libfvalue.vcproj` & `libfwevt-20240426/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/libcnotify/libcnotify.vcproj` & `libfwevt-20240426/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/libcerror/libcerror.vcproj` & `libfwevt-20240426/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfwevt-20240426/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_map/fwevt_test_map.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_map/fwevt_test_map.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/msvscpp/fwevt_test_support/fwevt_test_support.vcproj` & `libfwevt-20240426/msvscpp/fwevt_test_support/fwevt_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/INSTALL` & `libfwevt-20240426/INSTALL`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_list_element.h` & `libfwevt-20240426/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_array.h` & `libfwevt-20240426/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_definitions.h` & `libfwevt-20240426/libcdata/libcdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_libcerror.h` & `libfwevt-20240426/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_unused.h` & `libfwevt-20240426/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_btree.h` & `libfwevt-20240426/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_btree.c` & `libfwevt-20240426/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_support.c` & `libfwevt-20240426/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_list.c` & `libfwevt-20240426/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_extern.h` & `libfwevt-20240426/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_list.h` & `libfwevt-20240426/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_btree_values_list.h` & `libfwevt-20240426/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/Makefile.am` & `libfwevt-20240426/libcdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_btree_node.h` & `libfwevt-20240426/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_range_list_value.h` & `libfwevt-20240426/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_range_list.h` & `libfwevt-20240426/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_range_list.c` & `libfwevt-20240426/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_array.c` & `libfwevt-20240426/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_list_element.c` & `libfwevt-20240426/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_libcthreads.h` & `libfwevt-20240426/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_tree_node.h` & `libfwevt-20240426/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_error.h` & `libfwevt-20240426/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_types.h` & `libfwevt-20240426/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_btree_node.c` & `libfwevt-20240426/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_tree_node.c` & `libfwevt-20240426/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_support.h` & `libfwevt-20240426/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/Makefile.in` & `libfwevt-20240426/libcdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_range_list_value.c` & `libfwevt-20240426/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_btree_values_list.c` & `libfwevt-20240426/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcdata/libcdata_error.c` & `libfwevt-20240426/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt.pc.in` & `libfwevt-20240426/libfwevt.pc.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/config.sub` & `libfwevt-20240426/config.sub`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/setup.py` & `libfwevt-20240426/setup.py`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/acinclude.m4` & `libfwevt-20240426/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/config.rpath` & `libfwevt-20240426/config.rpath`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_thread.h` & `libfwevt-20240426/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_read_write_lock.h` & `libfwevt-20240426/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_thread.c` & `libfwevt-20240426/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_thread_pool.h` & `libfwevt-20240426/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_support.h` & `libfwevt-20240426/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_lock.h` & `libfwevt-20240426/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_unused.h` & `libfwevt-20240426/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_lock.c` & `libfwevt-20240426/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_condition.h` & `libfwevt-20240426/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_repeating_thread.h` & `libfwevt-20240426/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/Makefile.am` & `libfwevt-20240426/libcthreads/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_support.c` & `libfwevt-20240426/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_mutex.c` & `libfwevt-20240426/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_queue.c` & `libfwevt-20240426/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_mutex.h` & `libfwevt-20240426/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_types.h` & `libfwevt-20240426/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_thread_attributes.h` & `libfwevt-20240426/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_condition.c` & `libfwevt-20240426/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_error.c` & `libfwevt-20240426/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_read_write_lock.c` & `libfwevt-20240426/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_libcerror.h` & `libfwevt-20240426/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_definitions.h` & `libfwevt-20240426/libcthreads/libcthreads_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_thread_pool.c` & `libfwevt-20240426/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_error.h` & `libfwevt-20240426/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_thread_attributes.c` & `libfwevt-20240426/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_extern.h` & `libfwevt-20240426/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_repeating_thread.c` & `libfwevt-20240426/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/Makefile.in` & `libfwevt-20240426/libcthreads/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcthreads/libcthreads_queue.h` & `libfwevt-20240426/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfwevt.spec` & `libfwevt-20240426/libfwevt.spec`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfwevt
-Version: 20240419
+Version: 20240426
 Release: 1
 Summary: Library to support the Windows XML Event Log (EVTX) data types
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwevt
         
@@ -76,10 +76,10 @@
 %files -n libfwevt-python3
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Sun Apr 21 2024 Joachim Metz <joachim.metz@gmail.com> 20240419-1
+* Fri Apr 26 2024 Joachim Metz <joachim.metz@gmail.com> 20240426-1
 - Auto-generated
```

### Comparing `libfwevt-20240419/test-driver` & `libfwevt-20240426/test-driver`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/manuals/libfwevt.3` & `libfwevt-20240426/manuals/libfwevt.3`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.Dd December 30, 2023
+.Dd April 26, 2024
 .Dt libfwevt 3
 .Os libfwevt
 .Sh NAME
 .Nm libfwevt.h
 .Nd Library to support the Windows XML Event Log (EVTX) data types
 .Sh SYNOPSIS
 .In libfwevt.h
@@ -197,29 +197,25 @@
 .Ft int
 .Fn libfwevt_xml_document_get_utf16_xml_string_size "libfwevt_xml_document_t *xml_document" "size_t *utf16_string_size" "libfwevt_error_t **error"
 .Ft int
 .Fn libfwevt_xml_document_get_utf16_xml_string "libfwevt_xml_document_t *xml_document" "uint16_t *utf16_string" "size_t utf16_string_size" "libfwevt_error_t **error"
 .Pp
 XML tag functions
 .Ft int
+.Fn libfwevt_xml_tag_free "libfwevt_xml_tag_t **xml_tag" "libfwevt_error_t **error"
+.Ft int
 .Fn libfwevt_xml_tag_get_utf8_name_size "libfwevt_xml_tag_t *xml_tag" "size_t *utf8_string_size" "libfwevt_error_t **error"
 .Ft int
 .Fn libfwevt_xml_tag_get_utf8_name "libfwevt_xml_tag_t *xml_tag" "uint8_t *utf8_string" "size_t utf8_string_size" "libfwevt_error_t **error"
 .Ft int
 .Fn libfwevt_xml_tag_get_utf16_name_size "libfwevt_xml_tag_t *xml_tag" "size_t *utf16_string_size" "libfwevt_error_t **error"
 .Ft int
 .Fn libfwevt_xml_tag_get_utf16_name "libfwevt_xml_tag_t *xml_tag" "uint16_t *utf16_string" "size_t utf16_string_size" "libfwevt_error_t **error"
 .Ft int
-.Fn libfwevt_xml_tag_get_utf8_value_size "libfwevt_xml_tag_t *xml_tag" "size_t *utf8_string_size" "libfwevt_error_t **error"
-.Ft int
-.Fn libfwevt_xml_tag_get_utf8_value "libfwevt_xml_tag_t *xml_tag" "uint8_t *utf8_string" "size_t utf8_string_size" "libfwevt_error_t **error"
-.Ft int
-.Fn libfwevt_xml_tag_get_utf16_value_size "libfwevt_xml_tag_t *xml_tag" "size_t *utf16_string_size" "libfwevt_error_t **error"
-.Ft int
-.Fn libfwevt_xml_tag_get_utf16_value "libfwevt_xml_tag_t *xml_tag" "uint16_t *utf16_string" "size_t utf16_string_size" "libfwevt_error_t **error"
+.Fn libfwevt_xml_tag_get_value "libfwevt_xml_tag_t *xml_tag" "libfwevt_xml_value_t **xml_value" "libfwevt_error_t **error"
 .Ft int
 .Fn libfwevt_xml_tag_get_number_of_attributes "libfwevt_xml_tag_t *xml_tag" "int *number_of_attributes" "libfwevt_error_t **error"
 .Ft int
 .Fn libfwevt_xml_tag_get_attribute_by_index "libfwevt_xml_tag_t *xml_tag" "int attribute_index" "libfwevt_xml_tag_t **attribute_xml_tag" "libfwevt_error_t **error"
 .Ft int
 .Fn libfwevt_xml_tag_get_attribute_by_utf8_name "libfwevt_xml_tag_t *xml_tag" "const uint8_t *utf8_string" "size_t utf8_string_length" "libfwevt_xml_tag_t **attribute_xml_tag" "libfwevt_error_t **error"
 .Ft int
@@ -230,14 +226,36 @@
 .Fn libfwevt_xml_tag_get_element_by_index "libfwevt_xml_tag_t *xml_tag" "int element_index" "libfwevt_xml_tag_t **element_xml_tag" "libfwevt_error_t **error"
 .Ft int
 .Fn libfwevt_xml_tag_get_element_by_utf8_name "libfwevt_xml_tag_t *xml_tag" "const uint8_t *utf8_string" "size_t utf8_string_length" "libfwevt_xml_tag_t **element_xml_tag" "libfwevt_error_t **error"
 .Ft int
 .Fn libfwevt_xml_tag_get_element_by_utf16_name "libfwevt_xml_tag_t *xml_tag" "const uint16_t *utf16_string" "size_t utf16_string_length" "libfwevt_xml_tag_t **element_xml_tag" "libfwevt_error_t **error"
 .Ft int
 .Fn libfwevt_xml_tag_get_flags "libfwevt_xml_tag_t *xml_tag" "uint8_t *flags" "libfwevt_error_t **error"
+.Pp
+XML value functions
+.Ft int
+.Fn libfwevt_xml_value_free "libfwevt_xml_value_t **xml_value" "libfwevt_error_t **error"
+.Ft int
+.Fn libfwevt_xml_value_get_data_size "libfwevt_xml_value_t *xml_value" "size_t *data_size" "libfwevt_error_t **error"
+.Ft int
+.Fn libfwevt_xml_value_copy_data "libfwevt_xml_value_t *xml_value" "uint8_t *data" "size_t data_size" "libfwevt_error_t **error"
+.Ft int
+.Fn libfwevt_xml_value_copy_to_8bit "libfwevt_xml_value_t *xml_value" "uint8_t *value_8bit" "libfwevt_error_t **error"
+.Ft int
+.Fn libfwevt_xml_value_copy_to_32bit "libfwevt_xml_value_t *xml_value" "uint32_t *value_32bit" "libfwevt_error_t **error"
+.Ft int
+.Fn libfwevt_xml_value_copy_to_64bit "libfwevt_xml_value_t *xml_value" "uint64_t *value_64bit" "libfwevt_error_t **error"
+.Ft int
+.Fn libfwevt_xml_value_get_utf8_string_size "libfwevt_xml_value_t *xml_value" "size_t *utf8_string_size" "libfwevt_error_t **error"
+.Ft int
+.Fn libfwevt_xml_value_copy_to_utf8_string "libfwevt_xml_value_t *xml_value" "uint8_t *utf8_string" "size_t utf8_string_size" "libfwevt_error_t **error"
+.Ft int
+.Fn libfwevt_xml_value_get_utf16_string_size "libfwevt_xml_value_t *xml_value" "size_t *utf16_string_size" "libfwevt_error_t **error"
+.Ft int
+.Fn libfwevt_xml_value_copy_to_utf16_string "libfwevt_xml_value_t *xml_value" "uint16_t *utf16_string" "size_t utf16_string_size" "libfwevt_error_t **error"
 .Sh DESCRIPTION
 The
 .Fn libfwevt_get_version
 function is used to retrieve the library version.
 .Sh RETURN VALUES
 Most of the functions return NULL or \-1 on error, dependent on the return type.
 For the actual return values see "libfwevt.h".
```

### Comparing `libfwevt-20240419/manuals/Makefile.in` & `libfwevt-20240426/manuals/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/pyfwevt_test_support.py` & `libfwevt-20240426/tests/pyfwevt_test_support.py`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_xml_tag.c` & `libfwevt-20240426/tests/fwevt_test_xml_tag.c`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 #include "fwevt_test_libfwevt.h"
 #include "fwevt_test_libuna.h"
 #include "fwevt_test_macros.h"
 #include "fwevt_test_memory.h"
 #include "fwevt_test_unused.h"
 
 #include "../libfwevt/libfwevt_xml_tag.h"
+#include "../libfwevt/libfwevt_xml_value.h"
 
 #if defined( __GNUC__ ) && !defined( LIBFWEVT_DLL_IMPORT )
 
 /* Tests the libfwevt_xml_tag_initialize function
  * Returns 1 if successful or 0 if not
  */
 int fwevt_test_xml_tag_initialize(
@@ -71,16 +72,16 @@
 	 "xml_tag",
 	 xml_tag );
 
 	FWEVT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
-	result = libfwevt_xml_tag_free(
-	          &xml_tag,
+	result = libfwevt_internal_xml_tag_free(
+	          (libfwevt_internal_xml_tag_t **) &xml_tag,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -146,16 +147,16 @@
 
 		if( fwevt_test_malloc_attempts_before_fail != -1 )
 		{
 			fwevt_test_malloc_attempts_before_fail = -1;
 
 			if( xml_tag != NULL )
 			{
-				libfwevt_xml_tag_free(
-				 &xml_tag,
+				libfwevt_internal_xml_tag_free(
+				 (libfwevt_internal_xml_tag_t **) &xml_tag,
 				 NULL );
 			}
 		}
 		else
 		{
 			FWEVT_TEST_ASSERT_EQUAL_INT(
 			 "result",
@@ -188,16 +189,16 @@
 
 		if( fwevt_test_memset_attempts_before_fail != -1 )
 		{
 			fwevt_test_memset_attempts_before_fail = -1;
 
 			if( xml_tag != NULL )
 			{
-				libfwevt_xml_tag_free(
-				 &xml_tag,
+				libfwevt_internal_xml_tag_free(
+				 (libfwevt_internal_xml_tag_t **) &xml_tag,
 				 NULL );
 			}
 		}
 		else
 		{
 			FWEVT_TEST_ASSERT_EQUAL_INT(
 			 "result",
@@ -224,16 +225,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_free function
  * Returns 1 if successful or 0 if not
@@ -335,16 +336,16 @@
 	 error );
 
 	libcerror_error_free(
 	 &error );
 
 	/* Clean up
 	 */
-	result = libfwevt_xml_tag_free(
-	          &xml_tag,
+	result = libfwevt_internal_xml_tag_free(
+	          (libfwevt_internal_xml_tag_t **) &xml_tag,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -362,27 +363,28 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_set_name_data function
  * Returns 1 if successful or 0 if not
  */
 int fwevt_test_xml_tag_set_name_data(
      void )
 {
+	uint8_t name_data[ 10 ]     = { 'n', 0, 'a', 0, 'm', 0, 'e', 0, 0 };
 	libcerror_error_t *error    = NULL;
 	libfwevt_xml_tag_t *xml_tag = NULL;
 	int result                  = 0;
 
 	/* Initialize test
 	 */
 	result = libfwevt_xml_tag_initialize(
@@ -402,17 +404,16 @@
 	 "error",
 	 error );
 
 	/* Test regular cases
 	 */
 	result = libfwevt_xml_tag_set_name_data(
 	          xml_tag,
-	          (uint8_t *) "name",
-	          4,
-	          LIBUNA_CODEPAGE_ASCII,
+	          name_data,
+	          10,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -420,17 +421,16 @@
 	 "error",
 	 error );
 
 	/* Test error cases
 	 */
 	result = libfwevt_xml_tag_set_name_data(
 	          NULL,
-	          (uint8_t *) "name",
-	          4,
-	          LIBUNA_CODEPAGE_ASCII,
+	          name_data,
+	          10,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -440,16 +440,15 @@
 
 	libcerror_error_free(
 	 &error );
 
 	result = libfwevt_xml_tag_set_name_data(
 	          xml_tag,
 	          NULL,
-	          4,
-	          LIBUNA_CODEPAGE_ASCII,
+	          10,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -458,135 +457,16 @@
 	 error );
 
 	libcerror_error_free(
 	 &error );
 
 	result = libfwevt_xml_tag_set_name_data(
 	          xml_tag,
-	          (uint8_t *) "name",
+	          name_data,
 	          (size_t) SSIZE_MAX + 1,
-	          LIBUNA_CODEPAGE_ASCII,
-	          &error );
-
-	FWEVT_TEST_ASSERT_EQUAL_INT(
-	 "result",
-	 result,
-	 -1 );
-
-	FWEVT_TEST_ASSERT_IS_NOT_NULL(
-	 "error",
-	 error );
-
-	libcerror_error_free(
-	 &error );
-
-	/* Clean up
-	 */
-	result = libfwevt_xml_tag_free(
-	          &xml_tag,
-	          &error );
-
-	FWEVT_TEST_ASSERT_EQUAL_INT(
-	 "result",
-	 result,
-	 1 );
-
-	FWEVT_TEST_ASSERT_IS_NULL(
-	 "xml_tag",
-	 xml_tag );
-
-	FWEVT_TEST_ASSERT_IS_NULL(
-	 "error",
-	 error );
-
-	return( 1 );
-
-on_error:
-	if( error != NULL )
-	{
-		libcerror_error_free(
-		 &error );
-	}
-	if( xml_tag != NULL )
-	{
-		libfwevt_xml_tag_free(
-		 &xml_tag,
-		 NULL );
-	}
-	return( 0 );
-}
-
-/* Tests the libfwevt_xml_tag_get_value function
- * Returns 1 if successful or 0 if not
- */
-int fwevt_test_xml_tag_get_value(
-     void )
-{
-	libcerror_error_t *error    = NULL;
-	libfvalue_value_t *value    = 0;
-	libfwevt_xml_tag_t *xml_tag = NULL;
-	int result                  = 0;
-
-	/* Initialize test
-	 */
-	result = libfwevt_xml_tag_initialize(
-	          &xml_tag,
-	          &error );
-
-	FWEVT_TEST_ASSERT_EQUAL_INT(
-	 "result",
-	 result,
-	 1 );
-
-	FWEVT_TEST_ASSERT_IS_NOT_NULL(
-	 "xml_tag",
-	 xml_tag );
-
-	FWEVT_TEST_ASSERT_IS_NULL(
-	 "error",
-	 error );
-
-	/* Test regular cases
-	 */
-	result = libfwevt_xml_tag_get_value(
-	          xml_tag,
-	          &value,
-	          &error );
-
-	FWEVT_TEST_ASSERT_EQUAL_INT(
-	 "result",
-	 result,
-	 1 );
-
-	FWEVT_TEST_ASSERT_IS_NULL(
-	 "error",
-	 error );
-
-	/* Test error cases
-	 */
-	result = libfwevt_xml_tag_get_value(
-	          NULL,
-	          &value,
-	          &error );
-
-	FWEVT_TEST_ASSERT_EQUAL_INT(
-	 "result",
-	 result,
-	 -1 );
-
-	FWEVT_TEST_ASSERT_IS_NOT_NULL(
-	 "error",
-	 error );
-
-	libcerror_error_free(
-	 &error );
-
-	result = libfwevt_xml_tag_get_value(
-	          xml_tag,
-	          NULL,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -595,16 +475,16 @@
 	 error );
 
 	libcerror_error_free(
 	 &error );
 
 	/* Clean up
 	 */
-	result = libfwevt_xml_tag_free(
-	          &xml_tag,
+	result = libfwevt_internal_xml_tag_free(
+	          (libfwevt_internal_xml_tag_t **) &xml_tag,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -622,16 +502,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_set_value_type function
  * Returns 1 if successful or 0 if not
@@ -712,16 +592,16 @@
 	 error );
 
 	libcerror_error_free(
 	 &error );
 
 	/* Clean up
 	 */
-	result = libfwevt_xml_tag_free(
-	          &xml_tag,
+	result = libfwevt_internal_xml_tag_free(
+	          (libfwevt_internal_xml_tag_t **) &xml_tag,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -739,16 +619,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_set_value_format_flags function
  * Returns 1 if successful or 0 if not
@@ -826,16 +706,16 @@
 	 error );
 
 	libcerror_error_free(
 	 &error );
 
 	/* Clean up
 	 */
-	result = libfwevt_xml_tag_free(
-	          &xml_tag,
+	result = libfwevt_internal_xml_tag_free(
+	          (libfwevt_internal_xml_tag_t **) &xml_tag,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -853,16 +733,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_set_value_data function
  * Returns 1 if successful or 0 if not
@@ -982,16 +862,16 @@
 	 error );
 
 	libcerror_error_free(
 	 &error );
 
 	/* Clean up
 	 */
-	result = libfwevt_xml_tag_free(
-	          &xml_tag,
+	result = libfwevt_internal_xml_tag_free(
+	          (libfwevt_internal_xml_tag_t **) &xml_tag,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -1009,16 +889,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_get_utf8_name_size function
  * Returns 1 if successful or 0 if not
@@ -1448,14 +1328,114 @@
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	return( 0 );
 }
 
+/* Tests the libfwevt_xml_tag_get_value function
+ * Returns 1 if successful or 0 if not
+ */
+int fwevt_test_xml_tag_get_value(
+     libfwevt_xml_tag_t *xml_tag )
+{
+	libcerror_error_t *error        = NULL;
+	libfwevt_xml_value_t *xml_value = NULL;
+	int result                      = 0;
+
+	/* Test regular cases
+	 */
+	result = libfwevt_xml_tag_get_value(
+	          xml_tag,
+	          &xml_value,
+	          &error );
+
+	FWEVT_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 1 );
+
+	FWEVT_TEST_ASSERT_IS_NOT_NULL(
+	 "xml_value",
+	 xml_value );
+
+	FWEVT_TEST_ASSERT_IS_NULL(
+	 "error",
+	 error );
+
+	result = libfwevt_xml_value_free(
+	          &xml_value,
+	          &error );
+
+	FWEVT_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 1 );
+
+	FWEVT_TEST_ASSERT_IS_NULL(
+	 "xml_value",
+	 xml_value );
+
+	FWEVT_TEST_ASSERT_IS_NULL(
+	 "error",
+	 error );
+
+	/* Test error cases
+	 */
+	result = libfwevt_xml_tag_get_value(
+	          NULL,
+	          &xml_value,
+	          &error );
+
+	FWEVT_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 -1 );
+
+	FWEVT_TEST_ASSERT_IS_NOT_NULL(
+	 "error",
+	 error );
+
+	libcerror_error_free(
+	 &error );
+
+	result = libfwevt_xml_tag_get_value(
+	          xml_tag,
+	          NULL,
+	          &error );
+
+	FWEVT_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 -1 );
+
+	FWEVT_TEST_ASSERT_IS_NOT_NULL(
+	 "error",
+	 error );
+
+	libcerror_error_free(
+	 &error );
+
+	return( 1 );
+
+on_error:
+	if( error != NULL )
+	{
+		libcerror_error_free(
+		 &error );
+	}
+	if( xml_value != NULL )
+	{
+		libfwevt_internal_xml_value_free(
+		 (libfwevt_internal_xml_value_t **) &xml_value,
+		 NULL );
+	}
+	return( 0 );
+}
+
 /* Tests the libfwevt_xml_tag_get_utf8_value_size function
  * Returns 1 if successful or 0 if not
  */
 int fwevt_test_xml_tag_get_utf8_value_size(
      libfwevt_xml_tag_t *xml_tag )
 {
 	libcerror_error_t *error = NULL;
@@ -2005,16 +1985,16 @@
 
 		FWEVT_TEST_ASSERT_IS_NULL(
 		 "error",
 		 error );
 
 		/* Clean up
 		 */
-		result = libfwevt_xml_tag_free(
-		          &attribute_xml_tag,
+		result = libfwevt_internal_xml_tag_free(
+		          (libfwevt_internal_xml_tag_t **) &attribute_xml_tag,
 		          &error );
 
 		FWEVT_TEST_ASSERT_EQUAL_INT(
 		 "result",
 		 result,
 		 1 );
 
@@ -2088,16 +2068,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( attribute_xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &attribute_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &attribute_xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_get_attribute_by_utf8_name function
  * Returns 1 if successful or 0 if not
@@ -2132,16 +2112,16 @@
 	 "error",
 	 error );
 
 	if( result != 0 )
 	{
 		/* Clean up
 		 */
-		result = libfwevt_xml_tag_free(
-		          &attribute_xml_tag,
+		result = libfwevt_internal_xml_tag_free(
+		          (libfwevt_internal_xml_tag_t **) &attribute_xml_tag,
 		          &error );
 
 		FWEVT_TEST_ASSERT_EQUAL_INT(
 		 "result",
 		 result,
 		 1 );
 
@@ -2237,16 +2217,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( attribute_xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &attribute_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &attribute_xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_get_attribute_by_utf16_name function
  * Returns 1 if successful or 0 if not
@@ -2281,16 +2261,16 @@
 	 "error",
 	 error );
 
 	if( result != 0 )
 	{
 		/* Clean up
 		 */
-		result = libfwevt_xml_tag_free(
-		          &attribute_xml_tag,
+		result = libfwevt_internal_xml_tag_free(
+		          (libfwevt_internal_xml_tag_t **) &attribute_xml_tag,
 		          &error );
 
 		FWEVT_TEST_ASSERT_EQUAL_INT(
 		 "result",
 		 result,
 		 1 );
 
@@ -2386,16 +2366,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( attribute_xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &attribute_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &attribute_xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_get_number_of_elements function
  * Returns 1 if successful or 0 if not
@@ -2518,16 +2498,16 @@
 
 		FWEVT_TEST_ASSERT_IS_NULL(
 		 "error",
 		 error );
 
 		/* Clean up
 		 */
-		result = libfwevt_xml_tag_free(
-		          &element_xml_tag,
+		result = libfwevt_internal_xml_tag_free(
+		          (libfwevt_internal_xml_tag_t **) &element_xml_tag,
 		          &error );
 
 		FWEVT_TEST_ASSERT_EQUAL_INT(
 		 "result",
 		 result,
 		 1 );
 
@@ -2601,16 +2581,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( element_xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &element_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &element_xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_get_element_by_utf8_name function
  * Returns 1 if successful or 0 if not
@@ -2645,16 +2625,16 @@
 	 "error",
 	 error );
 
 	if( result != 0 )
 	{
 		/* Clean up
 		 */
-		result = libfwevt_xml_tag_free(
-		          &element_xml_tag,
+		result = libfwevt_internal_xml_tag_free(
+		          (libfwevt_internal_xml_tag_t **) &element_xml_tag,
 		          &error );
 
 		FWEVT_TEST_ASSERT_EQUAL_INT(
 		 "result",
 		 result,
 		 1 );
 
@@ -2750,16 +2730,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( element_xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &element_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &element_xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_get_element_by_utf16_name function
  * Returns 1 if successful or 0 if not
@@ -2794,16 +2774,16 @@
 	 "error",
 	 error );
 
 	if( result != 0 )
 	{
 		/* Clean up
 		 */
-		result = libfwevt_xml_tag_free(
-		          &element_xml_tag,
+		result = libfwevt_internal_xml_tag_free(
+		          (libfwevt_internal_xml_tag_t **) &element_xml_tag,
 		          &error );
 
 		FWEVT_TEST_ASSERT_EQUAL_INT(
 		 "result",
 		 result,
 		 1 );
 
@@ -2899,16 +2879,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( element_xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &element_xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &element_xml_tag,
 		 NULL );
 	}
 	return( 0 );
 }
 
 /* Tests the libfwevt_xml_tag_get_flags function
  * Returns 1 if successful or 0 if not
@@ -3194,14 +3174,19 @@
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
+	FWEVT_TEST_ASSERT_EQUAL_SIZE(
+	 "utf8_xml_string_size",
+	 utf8_xml_string_size,
+	 (size_t) 23 );
+
 	FWEVT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
 	/* Test error cases
 	 */
 	result = libfwevt_xml_tag_get_utf8_xml_string_size(
@@ -3253,14 +3238,18 @@
 
 /* Tests the libfwevt_xml_tag_get_utf8_xml_string_with_index function
  * Returns 1 if successful or 0 if not
  */
 int fwevt_test_xml_tag_get_utf8_xml_string_with_index(
      libfwevt_xml_tag_t *xml_tag )
 {
+	uint8_t expected_utf8_string[ 23 ] = {
+		'<', 'n', 'a', 'm', 'e', '>', '6', '4', '6', '1', '7', '4', '6', '1', '<', '/',
+		'n', 'a', 'm', 'e', '>', '\n', 0 };
+
 	uint8_t utf8_string[ 32 ];
 
 	libcerror_error_t *error = NULL;
 	size_t utf8_string_index = 0;
 	int result               = 0;
 
 	/* Test regular cases
@@ -3274,18 +3263,33 @@
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
+	FWEVT_TEST_ASSERT_EQUAL_SIZE(
+	 "utf8_string_index",
+	 utf8_string_index,
+	 (size_t) 23 );
+
 	FWEVT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
+	result = memory_compare(
+	          expected_utf8_string,
+	          utf8_string,
+	          23 );
+
+	FWEVT_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 0 );
+
 	/* Test error cases
 	 */
 	result = libfwevt_xml_tag_get_utf8_xml_string_with_index(
 	          NULL,
 	          0,
 	          utf8_string,
 	          32,
@@ -3586,14 +3590,19 @@
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
+	FWEVT_TEST_ASSERT_EQUAL_SIZE(
+	 "utf16_xml_string_size",
+	 utf16_xml_string_size,
+	 (size_t) 23 );
+
 	FWEVT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
 	/* Test error cases
 	 */
 	result = libfwevt_xml_tag_get_utf16_xml_string_size(
@@ -3645,14 +3654,18 @@
 
 /* Tests the libfwevt_xml_tag_get_utf16_xml_string_with_index function
  * Returns 1 if successful or 0 if not
  */
 int fwevt_test_xml_tag_get_utf16_xml_string_with_index(
      libfwevt_xml_tag_t *xml_tag )
 {
+	uint16_t expected_utf16_string[ 23 ] = {
+		'<', 'n', 'a', 'm', 'e', '>', '6', '4', '6', '1', '7', '4', '6', '1', '<', '/',
+		'n', 'a', 'm', 'e', '>', '\n', 0 };
+
 	uint16_t utf16_string[ 32 ];
 
 	libcerror_error_t *error  = NULL;
 	size_t utf16_string_index = 0;
 	int result                = 0;
 
 	/* Test regular cases
@@ -3666,18 +3679,33 @@
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
+	FWEVT_TEST_ASSERT_EQUAL_SIZE(
+	 "utf16_string_index",
+	 utf16_string_index,
+	 (size_t) 23 );
+
 	FWEVT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
+	result = memory_compare(
+	          expected_utf16_string,
+	          utf16_string,
+	          23 );
+
+	FWEVT_TEST_ASSERT_EQUAL_INT(
+	 "result",
+	 result,
+	 0 );
+
 	/* Test error cases
 	 */
 	result = libfwevt_xml_tag_get_utf16_xml_string_with_index(
 	          NULL,
 	          0,
 	          utf16_string,
 	          32,
@@ -3779,14 +3807,15 @@
 int main(
      int argc FWEVT_TEST_ATTRIBUTE_UNUSED,
      char * const argv[] FWEVT_TEST_ATTRIBUTE_UNUSED )
 #endif
 {
 #if defined( __GNUC__ ) && !defined( LIBFWEVT_DLL_IMPORT )
 
+	uint8_t name_data[ 10 ]     = { 'n', 0, 'a', 0, 'm', 0, 'e', 0, 0 };
 	libcerror_error_t *error    = NULL;
 	libfwevt_xml_tag_t *xml_tag = NULL;
 	int result                  = 0;
 
 #endif /* defined( __GNUC__ ) && !defined( LIBFWEVT_DLL_IMPORT ) */
 
 	FWEVT_TEST_UNREFERENCED_PARAMETER( argc )
@@ -3798,27 +3827,25 @@
 	 "libfwevt_xml_tag_initialize",
 	 fwevt_test_xml_tag_initialize );
 
 	FWEVT_TEST_RUN(
 	 "libfwevt_xml_tag_free",
 	 fwevt_test_xml_tag_free );
 
+	/* TODO: add tests for libfwevt_internal_xml_tag_free */
+
 	FWEVT_TEST_RUN(
 	 "libfwevt_xml_tag_set_type",
 	 fwevt_test_xml_tag_set_type );
 
 	FWEVT_TEST_RUN(
 	 "libfwevt_xml_tag_set_name_data",
 	 fwevt_test_xml_tag_set_name_data );
 
 	FWEVT_TEST_RUN(
-	 "libfwevt_xml_tag_get_value",
-	 fwevt_test_xml_tag_get_value );
-
-	FWEVT_TEST_RUN(
 	 "libfwevt_xml_tag_set_value_type",
 	 fwevt_test_xml_tag_set_value_type );
 
 	FWEVT_TEST_RUN(
 	 "libfwevt_xml_tag_set_value_format_flags",
 	 fwevt_test_xml_tag_set_value_format_flags );
 
@@ -3853,17 +3880,16 @@
 
 	FWEVT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
 	result = libfwevt_xml_tag_set_name_data(
 	          xml_tag,
-	          (uint8_t *) "name",
-	          4,
-	          LIBUNA_CODEPAGE_ASCII,
+	          name_data,
+	          10,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -3932,14 +3958,19 @@
 
 	FWEVT_TEST_RUN_WITH_ARGS(
 	 "libfwevt_xml_tag_get_utf16_name",
 	 fwevt_test_xml_tag_get_utf16_name,
 	 xml_tag );
 
 	FWEVT_TEST_RUN_WITH_ARGS(
+	 "libfwevt_xml_tag_get_value",
+	 fwevt_test_xml_tag_get_value,
+	 xml_tag );
+
+	FWEVT_TEST_RUN_WITH_ARGS(
 	 "libfwevt_xml_tag_get_utf8_value_size",
 	 fwevt_test_xml_tag_get_utf8_value_size,
 	 xml_tag );
 
 	FWEVT_TEST_RUN_WITH_ARGS(
 	 "libfwevt_xml_tag_get_utf8_value",
 	 fwevt_test_xml_tag_get_utf8_value,
@@ -4052,16 +4083,16 @@
 
 	/* TODO: add tests for libfwevt_xml_tag_value_debug_print */
 
 #endif /* defined( HAVE_DEBUG_OUTPUT ) */
 
 	/* Clean up
 	 */
-	result = libfwevt_xml_tag_free(
-	          &xml_tag,
+	result = libfwevt_internal_xml_tag_free(
+	          (libfwevt_internal_xml_tag_t **) &xml_tag,
 	          &error );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -4085,16 +4116,16 @@
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
 	if( xml_tag != NULL )
 	{
-		libfwevt_xml_tag_free(
-		 &xml_tag,
+		libfwevt_internal_xml_tag_free(
+		 (libfwevt_internal_xml_tag_t **) &xml_tag,
 		 NULL );
 	}
 	return( EXIT_FAILURE );
 
 #endif /* defined( __GNUC__ ) && !defined( LIBFWEVT_DLL_IMPORT ) */
 }
```

### Comparing `libfwevt-20240419/tests/fwevt_test_keyword.c` & `libfwevt-20240426/tests/fwevt_test_keyword.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_template_item.c` & `libfwevt-20240426/tests/fwevt_test_template_item.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/pyfwevt_test_provider.py` & `libfwevt-20240426/tests/pyfwevt_test_provider.py`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_libuna.h` & `libfwevt-20240426/tests/fwevt_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_map.c` & `libfwevt-20240426/tests/fwevt_test_map.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_memory.h` & `libfwevt-20240426/tests/fwevt_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_xml_template_value.c` & `libfwevt-20240426/tests/fwevt_test_xml_template_value.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/Makefile.am` & `libfwevt-20240426/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 	fwevt_test_support \
 	fwevt_test_task \
 	fwevt_test_template \
 	fwevt_test_template_item \
 	fwevt_test_xml_document \
 	fwevt_test_xml_tag \
 	fwevt_test_xml_template_value \
-	fwevt_test_xml_token
+	fwevt_test_xml_token \
+	fwevt_test_xml_value
 
 fwevt_test_channel_SOURCES = \
 	fwevt_test_channel.c \
 	fwevt_test_libcerror.h \
 	fwevt_test_libfwevt.h \
 	fwevt_test_macros.h \
 	fwevt_test_memory.c fwevt_test_memory.h \
@@ -262,12 +263,26 @@
 	fwevt_test_unused.h \
 	fwevt_test_xml_token.c
 
 fwevt_test_xml_token_LDADD = \
 	../libfwevt/libfwevt.la \
 	@LIBCERROR_LIBADD@
 
+fwevt_test_xml_value_SOURCES = \
+	fwevt_test_libcerror.h \
+	fwevt_test_libfvalue.h \
+	fwevt_test_libfwevt.h \
+	fwevt_test_libuna.h \
+	fwevt_test_macros.h \
+	fwevt_test_memory.c fwevt_test_memory.h \
+	fwevt_test_unused.h \
+	fwevt_test_xml_value.c
+
+fwevt_test_xml_value_LDADD = \
+	../libfwevt/libfwevt.la \
+	@LIBCERROR_LIBADD@
+
 DISTCLEANFILES = \
 	Makefile \
 	Makefile.in \
 	notify_stream.log
```

### Comparing `libfwevt-20240419/tests/fwevt_test_channel.c` & `libfwevt-20240426/tests/fwevt_test_channel.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_event.c` & `libfwevt-20240426/tests/fwevt_test_event.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_xml_token.c` & `libfwevt-20240426/tests/fwevt_test_xml_token.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/pyfwevt_test_event.py` & `libfwevt-20240426/tests/pyfwevt_test_event.py`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_macros.h` & `libfwevt-20240426/tests/fwevt_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_level.c` & `libfwevt-20240426/tests/fwevt_test_level.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/test_manpage.sh` & `libfwevt-20240426/tests/test_manpage.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/test_python_module.sh` & `libfwevt-20240426/tests/test_python_module.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_libcerror.h` & `libfwevt-20240426/tests/fwevt_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_notify.c` & `libfwevt-20240426/tests/fwevt_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_memory.c` & `libfwevt-20240426/tests/fwevt_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_xml_document.c` & `libfwevt-20240426/tests/fwevt_test_xml_document.c`

 * *Files 0% similar despite different names*

```diff
@@ -4401,15 +4401,14 @@
 	 "root_xml_tag",
 	 root_xml_tag );
 
 	FWEVT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
-/* TODO
 	result = libfwevt_xml_tag_free(
 	          &root_xml_tag,
 	          NULL );
 
 	FWEVT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -4418,15 +4417,14 @@
 	FWEVT_TEST_ASSERT_IS_NULL(
 	 "root_xml_tag",
 	 root_xml_tag );
 
 	FWEVT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
-*/
 
 	/* Test error cases
 	 */
 	result = libfwevt_xml_document_get_root_xml_tag(
 	          NULL,
 	          &root_xml_tag,
 	          &error );
@@ -4464,22 +4462,20 @@
 
 on_error:
 	if( error != NULL )
 	{
 		libcerror_error_free(
 		 &error );
 	}
-/* TODO
 	if( root_xml_tag != NULL )
 	{
 		libfwevt_xml_tag_free(
 		 &root_xml_tag,
 		 NULL );
 	}
-*/
 	return( 0 );
 }
 
 #endif /* !defined( LIBFWEVT_DLL_IMPORT ) */
 
 /* Tests the libfwevt_xml_document_read function
  * Returns 1 if successful or 0 if not
```

### Comparing `libfwevt-20240419/tests/fwevt_test_manifest.c` & `libfwevt-20240426/tests/fwevt_test_manifest.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/pyfwevt_test_manifest.py` & `libfwevt-20240426/tests/pyfwevt_test_manifest.py`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_libfwevt.h` & `libfwevt-20240426/tests/fwevt_test_libfwevt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/test_runner.sh` & `libfwevt-20240426/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_provider.c` & `libfwevt-20240426/tests/fwevt_test_provider.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_support.c` & `libfwevt-20240426/tests/fwevt_test_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_libcnotify.h` & `libfwevt-20240426/tests/fwevt_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_opcode.c` & `libfwevt-20240426/tests/fwevt_test_opcode.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_task.c` & `libfwevt-20240426/tests/fwevt_test_task.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/Makefile.in` & `libfwevt-20240426/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 	fwevt_test_level$(EXEEXT) fwevt_test_manifest$(EXEEXT) \
 	fwevt_test_map$(EXEEXT) fwevt_test_notify$(EXEEXT) \
 	fwevt_test_opcode$(EXEEXT) fwevt_test_provider$(EXEEXT) \
 	fwevt_test_support$(EXEEXT) fwevt_test_task$(EXEEXT) \
 	fwevt_test_template$(EXEEXT) fwevt_test_template_item$(EXEEXT) \
 	fwevt_test_xml_document$(EXEEXT) fwevt_test_xml_tag$(EXEEXT) \
 	fwevt_test_xml_template_value$(EXEEXT) \
-	fwevt_test_xml_token$(EXEEXT)
+	fwevt_test_xml_token$(EXEEXT) fwevt_test_xml_value$(EXEEXT)
 subdir = tests
 ACLOCAL_M4 = $(top_srcdir)/aclocal.m4
 am__aclocal_m4_deps = $(top_srcdir)/m4/common.m4 \
 	$(top_srcdir)/m4/gettext.m4 $(top_srcdir)/m4/host-cpu-c-abi.m4 \
 	$(top_srcdir)/m4/iconv.m4 $(top_srcdir)/m4/intlmacosx.m4 \
 	$(top_srcdir)/m4/lib-ld.m4 $(top_srcdir)/m4/lib-link.m4 \
 	$(top_srcdir)/m4/lib-prefix.m4 $(top_srcdir)/m4/libcdata.m4 \
@@ -195,14 +195,18 @@
 fwevt_test_xml_template_value_OBJECTS =  \
 	$(am_fwevt_test_xml_template_value_OBJECTS)
 fwevt_test_xml_template_value_DEPENDENCIES = ../libfwevt/libfwevt.la
 am_fwevt_test_xml_token_OBJECTS = fwevt_test_memory.$(OBJEXT) \
 	fwevt_test_xml_token.$(OBJEXT)
 fwevt_test_xml_token_OBJECTS = $(am_fwevt_test_xml_token_OBJECTS)
 fwevt_test_xml_token_DEPENDENCIES = ../libfwevt/libfwevt.la
+am_fwevt_test_xml_value_OBJECTS = fwevt_test_memory.$(OBJEXT) \
+	fwevt_test_xml_value.$(OBJEXT)
+fwevt_test_xml_value_OBJECTS = $(am_fwevt_test_xml_value_OBJECTS)
+fwevt_test_xml_value_DEPENDENCIES = ../libfwevt/libfwevt.la
 AM_V_P = $(am__v_P_@AM_V@)
 am__v_P_ = $(am__v_P_@AM_DEFAULT_V@)
 am__v_P_0 = false
 am__v_P_1 = :
 AM_V_GEN = $(am__v_GEN_@AM_V@)
 am__v_GEN_ = $(am__v_GEN_@AM_DEFAULT_V@)
 am__v_GEN_0 = @echo "  GEN     " $@;
@@ -227,15 +231,16 @@
 	./$(DEPDIR)/fwevt_test_support.Po \
 	./$(DEPDIR)/fwevt_test_task.Po \
 	./$(DEPDIR)/fwevt_test_template.Po \
 	./$(DEPDIR)/fwevt_test_template_item.Po \
 	./$(DEPDIR)/fwevt_test_xml_document.Po \
 	./$(DEPDIR)/fwevt_test_xml_tag.Po \
 	./$(DEPDIR)/fwevt_test_xml_template_value.Po \
-	./$(DEPDIR)/fwevt_test_xml_token.Po
+	./$(DEPDIR)/fwevt_test_xml_token.Po \
+	./$(DEPDIR)/fwevt_test_xml_value.Po
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
 	$(AM_CFLAGS) $(CFLAGS)
@@ -258,27 +263,29 @@
 	$(fwevt_test_opcode_SOURCES) $(fwevt_test_provider_SOURCES) \
 	$(fwevt_test_support_SOURCES) $(fwevt_test_task_SOURCES) \
 	$(fwevt_test_template_SOURCES) \
 	$(fwevt_test_template_item_SOURCES) \
 	$(fwevt_test_xml_document_SOURCES) \
 	$(fwevt_test_xml_tag_SOURCES) \
 	$(fwevt_test_xml_template_value_SOURCES) \
-	$(fwevt_test_xml_token_SOURCES)
+	$(fwevt_test_xml_token_SOURCES) \
+	$(fwevt_test_xml_value_SOURCES)
 DIST_SOURCES = $(fwevt_test_channel_SOURCES) \
 	$(fwevt_test_error_SOURCES) $(fwevt_test_event_SOURCES) \
 	$(fwevt_test_keyword_SOURCES) $(fwevt_test_level_SOURCES) \
 	$(fwevt_test_manifest_SOURCES) $(fwevt_test_map_SOURCES) \
 	$(fwevt_test_notify_SOURCES) $(fwevt_test_opcode_SOURCES) \
 	$(fwevt_test_provider_SOURCES) $(fwevt_test_support_SOURCES) \
 	$(fwevt_test_task_SOURCES) $(fwevt_test_template_SOURCES) \
 	$(fwevt_test_template_item_SOURCES) \
 	$(fwevt_test_xml_document_SOURCES) \
 	$(fwevt_test_xml_tag_SOURCES) \
 	$(fwevt_test_xml_template_value_SOURCES) \
-	$(fwevt_test_xml_token_SOURCES)
+	$(fwevt_test_xml_token_SOURCES) \
+	$(fwevt_test_xml_value_SOURCES)
 am__can_run_installinfo = \
   case $$AM_UPDATE_INFO_DIR in \
     n|no|NO) false;; \
     *) (install-info --version) >/dev/null 2>&1;; \
   esac
 am__extra_recursive_targets = sources-recursive splint-recursive
 am__tagged_files = $(HEADERS) $(SOURCES) $(TAGS_FILES) $(LISP)
@@ -1001,14 +1008,28 @@
 	fwevt_test_unused.h \
 	fwevt_test_xml_token.c
 
 fwevt_test_xml_token_LDADD = \
 	../libfwevt/libfwevt.la \
 	@LIBCERROR_LIBADD@
 
+fwevt_test_xml_value_SOURCES = \
+	fwevt_test_libcerror.h \
+	fwevt_test_libfvalue.h \
+	fwevt_test_libfwevt.h \
+	fwevt_test_libuna.h \
+	fwevt_test_macros.h \
+	fwevt_test_memory.c fwevt_test_memory.h \
+	fwevt_test_unused.h \
+	fwevt_test_xml_value.c
+
+fwevt_test_xml_value_LDADD = \
+	../libfwevt/libfwevt.la \
+	@LIBCERROR_LIBADD@
+
 DISTCLEANFILES = \
 	Makefile \
 	Makefile.in \
 	notify_stream.log
 
 all: all-am
 
@@ -1121,14 +1142,18 @@
 	@rm -f fwevt_test_xml_template_value$(EXEEXT)
 	$(AM_V_CCLD)$(LINK) $(fwevt_test_xml_template_value_OBJECTS) $(fwevt_test_xml_template_value_LDADD) $(LIBS)
 
 fwevt_test_xml_token$(EXEEXT): $(fwevt_test_xml_token_OBJECTS) $(fwevt_test_xml_token_DEPENDENCIES) $(EXTRA_fwevt_test_xml_token_DEPENDENCIES) 
 	@rm -f fwevt_test_xml_token$(EXEEXT)
 	$(AM_V_CCLD)$(LINK) $(fwevt_test_xml_token_OBJECTS) $(fwevt_test_xml_token_LDADD) $(LIBS)
 
+fwevt_test_xml_value$(EXEEXT): $(fwevt_test_xml_value_OBJECTS) $(fwevt_test_xml_value_DEPENDENCIES) $(EXTRA_fwevt_test_xml_value_DEPENDENCIES) 
+	@rm -f fwevt_test_xml_value$(EXEEXT)
+	$(AM_V_CCLD)$(LINK) $(fwevt_test_xml_value_OBJECTS) $(fwevt_test_xml_value_LDADD) $(LIBS)
+
 mostlyclean-compile:
 	-rm -f *.$(OBJEXT)
 
 distclean-compile:
 	-rm -f *.tab.c
 
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/fwevt_test_channel.Po@am__quote@ # am--include-marker
@@ -1146,14 +1171,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/fwevt_test_task.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/fwevt_test_template.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/fwevt_test_template_item.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/fwevt_test_xml_document.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/fwevt_test_xml_tag.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/fwevt_test_xml_template_value.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/fwevt_test_xml_token.Po@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/fwevt_test_xml_value.Po@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
 
@@ -1501,14 +1527,15 @@
 	-rm -f ./$(DEPDIR)/fwevt_test_task.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_template.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_template_item.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_xml_document.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_xml_tag.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_xml_template_value.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_xml_token.Po
+	-rm -f ./$(DEPDIR)/fwevt_test_xml_value.Po
 	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
@@ -1565,14 +1592,15 @@
 	-rm -f ./$(DEPDIR)/fwevt_test_task.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_template.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_template_item.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_xml_document.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_xml_tag.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_xml_template_value.Po
 	-rm -f ./$(DEPDIR)/fwevt_test_xml_token.Po
+	-rm -f ./$(DEPDIR)/fwevt_test_xml_value.Po
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
 	mostlyclean-libtool
```

### Comparing `libfwevt-20240419/tests/fwevt_test_template.c` & `libfwevt-20240426/tests/fwevt_test_template.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_error.c` & `libfwevt-20240426/tests/fwevt_test_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_unused.h` & `libfwevt-20240426/tests/fwevt_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/fwevt_test_libfvalue.h` & `libfwevt-20240426/tests/fwevt_test_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/tests/test_library.sh` & `libfwevt-20240426/tests/test_library.sh`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
-LIBRARY_TESTS="channel error event keyword level manifest map notify opcode provider support task template xml_document xml_tag xml_template_value xml_token";
+LIBRARY_TESTS="channel error event keyword level manifest map notify opcode provider support task template xml_document xml_tag xml_template_value xml_token xml_value";
 LIBRARY_TESTS_WITH_INPUT="";
 OPTION_SETS=();
 
 INPUT_GLOB="*";
 
 run_test()
 {
```

### Comparing `libfwevt-20240419/ossfuzz/xml_document_fuzzer.cc` & `libfwevt-20240426/ossfuzz/xml_document_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/ossfuzz/manifest_fuzzer.cc` & `libfwevt-20240426/ossfuzz/manifest_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/ossfuzz/Makefile.am` & `libfwevt-20240426/ossfuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/ossfuzz/ossfuzz_libfwevt.h` & `libfwevt-20240426/ossfuzz/ossfuzz_libfwevt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/ossfuzz/Makefile.in` & `libfwevt-20240426/ossfuzz/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/ltmain.sh` & `libfwevt-20240426/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/po/remove-potcdate.sin` & `libfwevt-20240426/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/po/Makefile.in.in` & `libfwevt-20240426/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/po/en@quot.header` & `libfwevt-20240426/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/po/en@boldquot.header` & `libfwevt-20240426/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/po/insert-header.sin` & `libfwevt-20240426/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/po/Makevars` & `libfwevt-20240426/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/po/Makevars.in` & `libfwevt-20240426/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/po/Rules-quot` & `libfwevt-20240426/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1251.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf16_string.c` & `libfwevt-20240426/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_base16_stream.c` & `libfwevt-20240426/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf8_stream.h` & `libfwevt-20240426/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_2.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_932.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_dingbats.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf8_string.c` & `libfwevt-20240426/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_base64_stream.c` & `libfwevt-20240426/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_error.h` & `libfwevt-20240426/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_turkish.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_unicode_character.c` & `libfwevt-20240426/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_gaelic.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_arabic.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_thai.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_874.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_15.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf8_string.h` & `libfwevt-20240426/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_16.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1255.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf7_stream.c` & `libfwevt-20240426/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_byte_stream.h` & `libfwevt-20240426/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_koi8_u.c` & `libfwevt-20240426/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_unused.h` & `libfwevt-20240426/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_6.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_14.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_base64_stream.h` & `libfwevt-20240426/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_error.c` & `libfwevt-20240426/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_centraleurroman.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_romanian.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_6.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_9.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_russian.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_dingbats.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_15.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_936.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_croatian.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_scsu.h` & `libfwevt-20240426/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/Makefile.am` & `libfwevt-20240426/libuna/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf32_stream.c` & `libfwevt-20240426/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_936.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_10.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_roman.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf7_stream.h` & `libfwevt-20240426/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_3.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_thai.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_farsi.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_ukrainian.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_inuit.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_932.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_874.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_5.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_10.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_definitions.h` & `libfwevt-20240426/libuna/libuna_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_url_stream.h` & `libfwevt-20240426/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_icelandic.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_koi8_u.h` & `libfwevt-20240426/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf16_stream.c` & `libfwevt-20240426/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1253.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_4.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_greek.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_libcerror.h` & `libfwevt-20240426/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_centraleurroman.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1254.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_13.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_7.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1255.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_unicode_character.h` & `libfwevt-20240426/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_8.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_13.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_949.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_cyrillic.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_celtic.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_support.h` & `libfwevt-20240426/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_4.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_949.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf16_stream.h` & `libfwevt-20240426/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_symbol.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_roman.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1257.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1254.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_950.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_extern.h` & `libfwevt-20240426/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1256.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_types.h` & `libfwevt-20240426/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_base32_stream.h` & `libfwevt-20240426/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1253.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_16.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf8_stream.c` & `libfwevt-20240426/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1250.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_2.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_support.c` & `libfwevt-20240426/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_koi8_r.c` & `libfwevt-20240426/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_5.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf16_string.h` & `libfwevt-20240426/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf32_string.c` & `libfwevt-20240426/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_icelandic.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1256.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf32_string.h` & `libfwevt-20240426/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_romanian.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_8.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_koi8_r.h` & `libfwevt-20240426/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_cyrillic.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_arabic.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_croatian.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_9.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_greek.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1258.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_7.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/Makefile.in` & `libfwevt-20240426/libuna/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_3.c` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1250.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_scsu.c` & `libfwevt-20240426/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1252.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_turkish.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_ukrainian.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_russian.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1258.c` & `libfwevt-20240426/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_celtic.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_byte_stream.c` & `libfwevt-20240426/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_gaelic.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_utf32_stream.h` & `libfwevt-20240426/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_symbol.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1257.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_inuit.h` & `libfwevt-20240426/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_mac_farsi.c` & `libfwevt-20240426/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_950.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_url_stream.c` & `libfwevt-20240426/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1251.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_windows_1252.h` & `libfwevt-20240426/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_codepage_iso_8859_14.h` & `libfwevt-20240426/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_base16_stream.h` & `libfwevt-20240426/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libuna/libuna_base32_stream.c` & `libfwevt-20240426/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/Makefile.in` & `libfwevt-20240426/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_filetime.c` & `libfwevt-20240426/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_utf16_string.c` & `libfwevt-20240426/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_libfwnt.h` & `libfwevt-20240426/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_value.c` & `libfwevt-20240426/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_value.h` & `libfwevt-20240426/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_definitions.h` & `libfwevt-20240426/libfvalue/libfvalue_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_codepage.h` & `libfwevt-20240426/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_split_utf16_string.c` & `libfwevt-20240426/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_error.c` & `libfwevt-20240426/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_utf8_string.c` & `libfwevt-20240426/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_unused.h` & `libfwevt-20240426/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_split_utf16_string.h` & `libfwevt-20240426/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_filetime.h` & `libfwevt-20240426/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_support.c` & `libfwevt-20240426/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_extern.h` & `libfwevt-20240426/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/Makefile.am` & `libfwevt-20240426/libfvalue/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_value_type.h` & `libfwevt-20240426/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_libcerror.h` & `libfwevt-20240426/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_split_utf8_string.c` & `libfwevt-20240426/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_data_handle.h` & `libfwevt-20240426/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_libcnotify.h` & `libfwevt-20240426/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_data_handle.c` & `libfwevt-20240426/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_integer.c` & `libfwevt-20240426/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_value_type.c` & `libfwevt-20240426/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_integer.h` & `libfwevt-20240426/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_binary_data.h` & `libfwevt-20240426/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_value_entry.h` & `libfwevt-20240426/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_utf16_string.h` & `libfwevt-20240426/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_error.h` & `libfwevt-20240426/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_table.h` & `libfwevt-20240426/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_libfguid.h` & `libfwevt-20240426/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_split_utf8_string.h` & `libfwevt-20240426/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_floating_point.h` & `libfwevt-20240426/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_libfdatetime.h` & `libfwevt-20240426/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_string.h` & `libfwevt-20240426/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_binary_data.c` & `libfwevt-20240426/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_value_entry.c` & `libfwevt-20240426/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_libcdata.h` & `libfwevt-20240426/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_support.h` & `libfwevt-20240426/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_table.c` & `libfwevt-20240426/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/Makefile.in` & `libfwevt-20240426/libfvalue/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_utf8_string.h` & `libfwevt-20240426/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_floating_point.c` & `libfwevt-20240426/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_types.h` & `libfwevt-20240426/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_string.c` & `libfwevt-20240426/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfvalue/libfvalue_libuna.h` & `libfwevt-20240426/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_definitions.h` & `libfwevt-20240426/libcnotify/libcnotify_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_extern.h` & `libfwevt-20240426/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_support.c` & `libfwevt-20240426/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_stream.h` & `libfwevt-20240426/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/Makefile.am` & `libfwevt-20240426/libcnotify/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_unused.h` & `libfwevt-20240426/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_verbose.h` & `libfwevt-20240426/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_print.h` & `libfwevt-20240426/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_stream.c` & `libfwevt-20240426/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_support.h` & `libfwevt-20240426/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_verbose.c` & `libfwevt-20240426/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/Makefile.in` & `libfwevt-20240426/libcnotify/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_libcerror.h` & `libfwevt-20240426/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcnotify/libcnotify_print.c` & `libfwevt-20240426/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/libcerror_system.c` & `libfwevt-20240426/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/libcerror_error.c` & `libfwevt-20240426/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/libcerror_extern.h` & `libfwevt-20240426/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/Makefile.am` & `libfwevt-20240426/libcerror/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/libcerror_types.h` & `libfwevt-20240426/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/libcerror_support.h` & `libfwevt-20240426/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/libcerror_error.h` & `libfwevt-20240426/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/libcerror_system.h` & `libfwevt-20240426/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/libcerror_definitions.h` & `libfwevt-20240426/libcerror/libcerror_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/libcerror_support.c` & `libfwevt-20240426/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/libcerror_unused.h` & `libfwevt-20240426/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libcerror/Makefile.in` & `libfwevt-20240426/libcerror/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_floatingtime.h` & `libfwevt-20240426/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_nsf_timedate.c` & `libfwevt-20240426/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_error.h` & `libfwevt-20240426/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_floatingtime.c` & `libfwevt-20240426/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_support.h` & `libfwevt-20240426/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_hfs_time.h` & `libfwevt-20240426/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_definitions.h` & `libfwevt-20240426/libfdatetime/libfdatetime_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_hfs_time.c` & `libfwevt-20240426/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/Makefile.am` & `libfwevt-20240426/libfdatetime/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_filetime.c` & `libfwevt-20240426/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_systemtime.h` & `libfwevt-20240426/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_extern.h` & `libfwevt-20240426/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_posix_time.c` & `libfwevt-20240426/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_unused.h` & `libfwevt-20240426/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_fat_date_time.h` & `libfwevt-20240426/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_systemtime.c` & `libfwevt-20240426/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_nsf_timedate.h` & `libfwevt-20240426/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_libcerror.h` & `libfwevt-20240426/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_support.c` & `libfwevt-20240426/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_error.c` & `libfwevt-20240426/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_posix_time.h` & `libfwevt-20240426/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_date_time_values.h` & `libfwevt-20240426/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_filetime.h` & `libfwevt-20240426/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_date_time_values.c` & `libfwevt-20240426/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_types.h` & `libfwevt-20240426/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/Makefile.in` & `libfwevt-20240426/libfdatetime/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/libfdatetime/libfdatetime_fat_date_time.c` & `libfwevt-20240426/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/aclocal.m4` & `libfwevt-20240426/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfwevt-20240419/configure.ac` & `libfwevt-20240426/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfwevt],
- [20240419],
+ [20240426],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfwevt.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

