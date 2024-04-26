# Comparing `tmp/libnk2-python-20240210.tar.gz` & `tmp/libnk2-python-20240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libnk2-python-20240210.tar", last modified: Sat Feb 10 03:54:58 2024, max compression
+gzip compressed data, was "libnk2-python-20240426.tar", last modified: Fri Apr 26 04:11:43 2024, max compression
```

## Comparing `libnk2-python-20240210.tar` & `libnk2-python-20240426.tar`

### file list

```diff
@@ -1,863 +1,863 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/libnk2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-10 03:39:33.000000 libnk2-20240210/libnk2/libnk2_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43071 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_record_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3809 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5295 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_record_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31872 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1805 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1732 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9264 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2343 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1959 2023-12-03 09:12:04.000000 libnk2-20240210/libnk2/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1066 2024-02-10 03:39:33.000000 libnk2-20240210/libnk2/libnk2.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13965 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/nk2_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/nk2_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1807 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_file_footer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13347 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_mapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6909 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_file_footer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1660 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7443 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1789 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2308 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_mapi_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_libfmapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/nk2_file_footer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2467 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3843 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34168 2024-02-10 03:39:23.000000 libnk2-20240210/libnk2/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15997 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2_mapi_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1068 2024-02-10 03:30:40.000000 libnk2-20240210/libnk2/libnk2.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-10 03:30:39.000000 libnk2-20240210/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-10 03:39:23.000000 libnk2-20240210/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:30:39.000000 libnk2-20240210/NEWS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3231 2024-02-10 03:30:39.000000 libnk2-20240210/libnk2.spec.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-10 03:39:24.000000 libnk2-20240210/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29024 2024-02-10 03:39:23.000000 libnk2-20240210/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-10 03:39:05.000000 libnk2-20240210/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8809 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libfwnt.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:12:03.000000 libnk2-20240210/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:12:03.000000 libnk2-20240210/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:12:04.000000 libnk2-20240210/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:12:03.000000 libnk2-20240210/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:12:04.000000 libnk2-20240210/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:12:04.000000 libnk2-20240210/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-10 03:39:17.000000 libnk2-20240210/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-10 03:39:17.000000 libnk2-20240210/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:12:04.000000 libnk2-20240210/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-10 03:39:17.000000 libnk2-20240210/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:12:04.000000 libnk2-20240210/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8941 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libfmapi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:12:04.000000 libnk2-20240210/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-10 03:39:17.000000 libnk2-20240210/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:12:04.000000 libnk2-20240210/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:12:04.000000 libnk2-20240210/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-10 03:39:17.000000 libnk2-20240210/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:12:04.000000 libnk2-20240210/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:12:04.000000 libnk2-20240210/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 09:12:03.000000 libnk2-20240210/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:12:04.000000 libnk2-20240210/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:12:04.000000 libnk2-20240210/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/include/libnk2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1917 2024-02-10 03:30:39.000000 libnk2-20240210/include/libnk2/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1915 2024-02-10 03:39:33.000000 libnk2-20240210/include/libnk2/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4996 2024-02-10 03:30:39.000000 libnk2-20240210/include/libnk2/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4865 2024-02-10 03:39:33.000000 libnk2-20240210/include/libnk2/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12373 2024-02-10 03:30:39.000000 libnk2-20240210/include/libnk2/mapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-10 03:30:39.000000 libnk2-20240210/include/libnk2/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-02-10 03:30:39.000000 libnk2-20240210/include/libnk2/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-10 03:30:39.000000 libnk2-20240210/include/libnk2/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-02-10 03:39:33.000000 libnk2-20240210/include/libnk2/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2024-02-10 03:30:39.000000 libnk2-20240210/include/libnk2/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      461 2024-02-10 03:30:39.000000 libnk2-20240210/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15283 2024-02-10 03:30:39.000000 libnk2-20240210/include/libnk2.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27549 2024-02-10 03:39:23.000000 libnk2-20240210/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15283 2024-02-10 03:39:33.000000 libnk2-20240210/include/libnk2.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-10 03:30:39.000000 libnk2-20240210/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-10 03:30:39.000000 libnk2-20240210/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-10 03:30:39.000000 libnk2-20240210/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-10 03:30:39.000000 libnk2-20240210/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-10 03:30:39.000000 libnk2-20240210/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-10 03:30:39.000000 libnk2-20240210/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-10 03:30:39.000000 libnk2-20240210/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-10 03:30:39.000000 libnk2-20240210/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-10 03:30:39.000000 libnk2-20240210/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2024-02-10 03:39:33.000000 libnk2-20240210/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15894 2024-02-10 03:39:22.000000 libnk2-20240210/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16835 2024-02-10 03:39:33.000000 libnk2-20240210/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-10 03:30:39.000000 libnk2-20240210/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-10 03:30:39.000000 libnk2-20240210/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-10 03:30:39.000000 libnk2-20240210/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24577 2024-02-10 03:39:23.000000 libnk2-20240210/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29580 2024-02-10 03:39:23.000000 libnk2-20240210/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-10 03:38:58.000000 libnk2-20240210/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2023-12-05 04:10:44.000000 libnk2-20240210/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33039 2024-02-10 03:39:23.000000 libnk2-20240210/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-10 03:38:51.000000 libnk2-20240210/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:11:53.000000 libnk2-20240210/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-10 03:39:23.000000 libnk2-20240210/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2024-02-10 03:30:40.000000 libnk2-20240210/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-10 03:30:39.000000 libnk2-20240210/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1988 2024-02-10 03:30:39.000000 libnk2-20240210/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-10 03:30:39.000000 libnk2-20240210/dpkg/libnk2.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      753 2024-02-10 03:30:39.000000 libnk2-20240210/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-10 03:30:39.000000 libnk2-20240210/dpkg/libnk2-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-10 03:30:39.000000 libnk2-20240210/dpkg/libnk2-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      119 2024-02-10 03:30:39.000000 libnk2-20240210/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2024-02-10 03:39:33.000000 libnk2-20240210/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-10 03:30:39.000000 libnk2-20240210/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-10 03:30:39.000000 libnk2-20240210/dpkg/libnk2-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      476 2024-02-10 03:39:33.000000 libnk2-20240210/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-10 03:30:39.000000 libnk2-20240210/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1918879 2024-02-10 03:39:21.000000 libnk2-20240210/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-10 03:39:23.000000 libnk2-20240210/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-10 03:39:23.000000 libnk2-20240210/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libnk2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8279 2024-02-10 03:31:02.000000 libnk2-20240210/msvscpp/libnk2/libnk2.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-02-10 03:31:02.000000 libnk2-20240210/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6048 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_tools_info_handle/nk2_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_item/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5862 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_item/nk2_test_item.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5545 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_error/nk2_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-10 03:31:02.000000 libnk2-20240210/msvscpp/libclocale/libclocale.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1289 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_record_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6050 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_record_entry/nk2_test_record_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-10 03:31:02.000000 libnk2-20240210/msvscpp/libbfio/libbfio.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30455 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/libnk2.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_file_footer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_file_footer/nk2_test_file_footer.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5733 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_tools_output/nk2_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-10 03:31:02.000000 libnk2-20240210/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5788 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_notify/nk2_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-10 03:31:02.000000 libnk2-20240210/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libfmapi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7276 2024-02-10 03:31:02.000000 libnk2-20240210/msvscpp/libfmapi/libfmapi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2info/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7093 2024-02-10 03:31:03.000000 libnk2-20240210/msvscpp/nk2info/nk2info.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6429 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_file/nk2_test_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-10 03:31:02.000000 libnk2-20240210/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-10 03:31:02.000000 libnk2-20240210/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-02-10 03:31:03.000000 libnk2-20240210/msvscpp/libfwnt/libfwnt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6438 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_support/nk2_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5733 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_tools_signal/nk2_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-10 03:31:03.000000 libnk2-20240210/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_mapi_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5642 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_mapi_value/nk2_test_mapi_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_file_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_file_header/nk2_test_file_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-10 03:31:03.000000 libnk2-20240210/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22834 2024-02-10 03:39:23.000000 libnk2-20240210/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8076 2024-02-10 03:31:03.000000 libnk2-20240210/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-10 03:31:03.000000 libnk2-20240210/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2export/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7662 2024-02-10 03:31:03.000000 libnk2-20240210/msvscpp/nk2export/nk2export.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-10 03:31:03.000000 libnk2-20240210/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/nk2_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5797 2024-02-10 03:31:30.000000 libnk2-20240210/msvscpp/nk2_test_io_handle/nk2_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-10 03:31:03.000000 libnk2-20240210/msvscpp/libfdatetime/libfdatetime.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-02-10 03:30:39.000000 libnk2-20240210/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30344 2024-02-10 03:39:23.000000 libnk2-20240210/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-10 03:38:56.000000 libnk2-20240210/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      359 2024-02-10 03:31:30.000000 libnk2-20240210/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-10 03:39:23.000000 libnk2-20240210/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/pynk2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-02-10 03:31:50.000000 libnk2-20240210/pynk2/pynk2_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8937 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_items.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1352 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3244 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3218 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2483 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_record_entries.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1347 2023-12-03 09:12:03.000000 libnk2-20240210/pynk2/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_libnk2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26675 2024-02-10 03:31:50.000000 libnk2-20240210/pynk2/pynk2_record_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15381 2024-02-10 03:31:50.000000 libnk2-20240210/pynk2/pynk2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2842 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3187 2024-02-10 03:31:50.000000 libnk2-20240210/pynk2/pynk2_record_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30383 2024-02-10 03:31:50.000000 libnk2-20240210/pynk2/pynk2_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9479 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_record_entries.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2024-02-10 03:31:50.000000 libnk2-20240210/pynk2/pynk2_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48659 2024-02-10 03:39:24.000000 libnk2-20240210/pynk2/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1165 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2294 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_items.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1804 2024-02-10 03:30:40.000000 libnk2-20240210/pynk2/pynk2_datetime.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32028 2024-02-10 03:39:23.000000 libnk2-20240210/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-10 03:38:53.000000 libnk2-20240210/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-10 03:30:39.000000 libnk2-20240210/pyproject.toml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/libfmapi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   124848 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1913 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_x400_object_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2174 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_entry_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40853 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_one_off_entry_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5468 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_one_off_entry_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1543 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3422 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1510 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2927 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10342 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_entry_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2951 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_class_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3877 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2189 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_class_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1670 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_checksum.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   158504 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_property_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16455 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_lzfu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3352 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_property_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2015 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_lzfu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2780 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_service_provider_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33364 2024-02-10 03:39:23.000000 libnk2-20240210/libfmapi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1523 2024-02-10 03:39:07.000000 libnk2-20240210/libfmapi/libfmapi_service_provider_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      631 2024-02-10 03:30:39.000000 libnk2-20240210/libnk2.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      477 2024-02-10 03:30:39.000000 libnk2-20240210/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-10 03:39:23.000000 libnk2-20240210/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-10 03:30:39.000000 libnk2-20240210/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-10 03:30:39.000000 libnk2-20240210/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:11:53.000000 libnk2-20240210/config.rpath
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2257 2024-02-10 03:39:33.000000 libnk2-20240210/libnk2.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32434 2024-02-10 03:39:23.000000 libnk2-20240210/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-10 03:39:03.000000 libnk2-20240210/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-10 03:39:24.000000 libnk2-20240210/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29622 2024-02-10 03:39:23.000000 libnk2-20240210/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-10 03:39:00.000000 libnk2-20240210/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-12-03 09:11:53.000000 libnk2-20240210/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7287 2024-02-10 03:30:40.000000 libnk2-20240210/manuals/libnk2.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-02-10 03:30:40.000000 libnk2-20240210/manuals/nk2info.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      180 2023-12-03 09:12:03.000000 libnk2-20240210/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1975 2024-02-10 03:30:40.000000 libnk2-20240210/manuals/nk2export.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26569 2024-02-10 03:39:23.000000 libnk2-20240210/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77832 2024-02-10 03:31:30.000000 libnk2-20240210/tests/nk2_test_record_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_libnk2.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3306 2024-02-10 03:30:40.000000 libnk2-20240210/tests/test_nk2info.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7856 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12118 2024-02-10 03:31:30.000000 libnk2-20240210/tests/nk2_test_file_footer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_libcerror.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4062 2024-02-10 03:31:50.000000 libnk2-20240210/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6989 2024-02-10 03:31:50.000000 libnk2-20240210/tests/pynk2_test_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6194 2024-02-10 03:31:30.000000 libnk2-20240210/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13463 2024-02-10 03:31:30.000000 libnk2-20240210/tests/nk2_test_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11176 2024-02-10 03:31:30.000000 libnk2-20240210/tests/nk2_test_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14091 2024-02-10 03:31:30.000000 libnk2-20240210/tests/nk2_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13235 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_functions.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-10 03:30:40.000000 libnk2-20240210/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4070 2024-02-10 03:30:40.000000 libnk2-20240210/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5546 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_tools_info_handle.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4679 2024-02-10 03:30:40.000000 libnk2-20240210/tests/test_nk2export.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-10 03:30:40.000000 libnk2-20240210/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_mapi_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33596 2024-02-10 03:31:30.000000 libnk2-20240210/tests/nk2_test_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2024-02-10 03:30:40.000000 libnk2-20240210/tests/nk2_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3408 2024-02-10 03:31:50.000000 libnk2-20240210/tests/pynk2_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59904 2024-02-10 03:39:24.000000 libnk2-20240210/tests/Makefile.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4122 2024-02-10 03:31:50.000000 libnk2-20240210/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2024-02-10 03:30:40.000000 libnk2-20240210/ossfuzz/ossfuzz_libnk2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      886 2023-12-03 09:12:03.000000 libnk2-20240210/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-10 03:30:40.000000 libnk2-20240210/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-02-10 03:30:40.000000 libnk2-20240210/ossfuzz/file_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31770 2024-02-10 03:39:24.000000 libnk2-20240210/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-10 03:39:17.000000 libnk2-20240210/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_locale_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_lzxpress.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_security_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_lznt1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_security_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_access_control_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_security_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_access_control_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_lznt1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_locale_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_lzx.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_access_control_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_lzxpress.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_security_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_lzx.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33249 2024-02-10 03:39:23.000000 libnk2-20240210/libfwnt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-02-10 03:39:10.000000 libnk2-20240210/libfwnt/libfwnt_access_control_entry.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/nk2tools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2143 2024-02-10 03:31:50.000000 libnk2-20240210/nk2tools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1403 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5687 2024-02-10 03:31:50.000000 libnk2-20240210/nk2tools/nk2info.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libnk2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/item_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44179 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/item_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2451 2023-12-03 09:12:05.000000 libnk2-20240210/nk2tools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10303 2024-02-10 03:31:50.000000 libnk2-20240210/nk2tools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10016 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2export.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39131 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/export_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2input.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4314 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5936 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/log_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8347 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2input.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5076 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/export_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libfmapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33555 2024-02-10 03:39:24.000000 libnk2-20240210/nk2tools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1672 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/log_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1756 2024-02-10 03:30:40.000000 libnk2-20240210/nk2tools/nk2tools_libfvalue.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30402 2024-02-10 03:39:23.000000 libnk2-20240210/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-10 03:39:01.000000 libnk2-20240210/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:12:05.000000 libnk2-20240210/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:12:05.000000 libnk2-20240210/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:12:05.000000 libnk2-20240210/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:12:05.000000 libnk2-20240210/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:12:05.000000 libnk2-20240210/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:12:05.000000 libnk2-20240210/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:12:05.000000 libnk2-20240210/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:12:05.000000 libnk2-20240210/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:12:05.000000 libnk2-20240210/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-02-10 03:39:33.000000 libnk2-20240210/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:12:05.000000 libnk2-20240210/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:12:05.000000 libnk2-20240210/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53146 2024-02-10 03:39:23.000000 libnk2-20240210/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-10 03:39:13.000000 libnk2-20240210/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40581 2024-02-10 03:39:23.000000 libnk2-20240210/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34908 2024-02-10 03:39:23.000000 libnk2-20240210/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-10 03:39:08.000000 libnk2-20240210/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29456 2024-02-10 03:39:23.000000 libnk2-20240210/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-10 03:38:59.000000 libnk2-20240210/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:56.000000 libnk2-20240210/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-10 03:38:54.000000 libnk2-20240210/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28969 2024-02-10 03:39:23.000000 libnk2-20240210/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-10 03:54:57.000000 libnk2-20240210/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32195 2024-02-10 03:39:23.000000 libnk2-20240210/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-10 03:39:04.000000 libnk2-20240210/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56826 2024-02-10 03:39:20.000000 libnk2-20240210/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7681 2024-02-10 03:30:39.000000 libnk2-20240210/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      408 2024-02-10 03:54:58.474411 libnk2-20240210/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:41.000000 libnk2-20240426/libnk2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-26 03:53:23.000000 libnk2-20240426/libnk2/libnk2_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42880 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_record_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3809 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5295 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_record_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31872 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1805 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1732 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9264 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2343 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1945 2024-04-26 03:36:01.000000 libnk2-20240426/libnk2/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1066 2024-04-26 03:53:23.000000 libnk2-20240426/libnk2/libnk2.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13965 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/nk2_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/nk2_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1807 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_file_footer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13347 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_mapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6909 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_file_footer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1660 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7443 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1789 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2308 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_mapi_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_libfmapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/nk2_file_footer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2467 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3843 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34651 2024-04-26 03:53:05.000000 libnk2-20240426/libnk2/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15997 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2_mapi_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1068 2024-04-26 03:27:33.000000 libnk2-20240426/libnk2/libnk2.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-26 03:27:30.000000 libnk2-20240426/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-26 03:53:04.000000 libnk2-20240426/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 03:27:30.000000 libnk2-20240426/NEWS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3231 2024-04-26 03:27:30.000000 libnk2-20240426/libnk2.spec.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-26 03:53:05.000000 libnk2-20240426/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:40.000000 libnk2-20240426/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29174 2024-04-26 03:53:05.000000 libnk2-20240426/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-26 03:52:46.000000 libnk2-20240426/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:38.000000 libnk2-20240426/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9040 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libfwnt.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:12:03.000000 libnk2-20240426/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:12:03.000000 libnk2-20240426/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:12:04.000000 libnk2-20240426/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:12:03.000000 libnk2-20240426/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:12:04.000000 libnk2-20240426/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-26 03:27:35.000000 libnk2-20240426/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-26 03:52:59.000000 libnk2-20240426/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-26 03:52:59.000000 libnk2-20240426/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:12:04.000000 libnk2-20240426/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-26 03:52:59.000000 libnk2-20240426/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:12:04.000000 libnk2-20240426/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9177 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libfmapi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:12:04.000000 libnk2-20240426/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-26 03:52:59.000000 libnk2-20240426/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:12:04.000000 libnk2-20240426/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:12:04.000000 libnk2-20240426/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-26 03:52:59.000000 libnk2-20240426/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:12:04.000000 libnk2-20240426/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-26 03:27:35.000000 libnk2-20240426/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-26 03:27:36.000000 libnk2-20240426/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:12:04.000000 libnk2-20240426/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-26 03:27:35.000000 libnk2-20240426/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:38.000000 libnk2-20240426/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:38.000000 libnk2-20240426/include/libnk2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1917 2024-04-26 03:27:33.000000 libnk2-20240426/include/libnk2/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1915 2024-04-26 03:53:23.000000 libnk2-20240426/include/libnk2/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4996 2024-04-26 03:27:33.000000 libnk2-20240426/include/libnk2/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4865 2024-04-26 03:53:23.000000 libnk2-20240426/include/libnk2/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12373 2024-04-26 03:27:33.000000 libnk2-20240426/include/libnk2/mapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-26 03:27:33.000000 libnk2-20240426/include/libnk2/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-04-26 03:27:33.000000 libnk2-20240426/include/libnk2/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-26 03:27:33.000000 libnk2-20240426/include/libnk2/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-26 03:53:23.000000 libnk2-20240426/include/libnk2/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2024-04-26 03:27:33.000000 libnk2-20240426/include/libnk2/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      412 2024-04-26 03:36:01.000000 libnk2-20240426/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15283 2024-04-26 03:27:33.000000 libnk2-20240426/include/libnk2.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27529 2024-04-26 03:53:05.000000 libnk2-20240426/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15283 2024-04-26 03:53:23.000000 libnk2-20240426/include/libnk2.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:38.000000 libnk2-20240426/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-26 03:27:32.000000 libnk2-20240426/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-26 03:27:32.000000 libnk2-20240426/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-26 03:27:32.000000 libnk2-20240426/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-26 03:27:32.000000 libnk2-20240426/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-26 03:27:32.000000 libnk2-20240426/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-26 03:27:32.000000 libnk2-20240426/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-26 03:27:32.000000 libnk2-20240426/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-26 03:36:01.000000 libnk2-20240426/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-26 03:27:32.000000 libnk2-20240426/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2024-04-26 03:53:23.000000 libnk2-20240426/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15894 2024-04-26 03:53:04.000000 libnk2-20240426/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16835 2024-04-26 03:53:23.000000 libnk2-20240426/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-26 03:27:32.000000 libnk2-20240426/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-26 03:27:32.000000 libnk2-20240426/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-26 03:27:32.000000 libnk2-20240426/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24584 2024-04-26 03:53:04.000000 libnk2-20240426/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:38.000000 libnk2-20240426/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29782 2024-04-26 03:53:05.000000 libnk2-20240426/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-26 03:52:38.000000 libnk2-20240426/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2080 2024-04-26 03:36:01.000000 libnk2-20240426/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:40.000000 libnk2-20240426/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33634 2024-04-26 03:53:05.000000 libnk2-20240426/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-04-26 03:52:33.000000 libnk2-20240426/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:11:53.000000 libnk2-20240426/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-26 03:53:04.000000 libnk2-20240426/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:38.000000 libnk2-20240426/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2024-04-26 03:27:35.000000 libnk2-20240426/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:38.000000 libnk2-20240426/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-26 03:27:30.000000 libnk2-20240426/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1988 2024-04-26 03:27:30.000000 libnk2-20240426/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-26 03:27:30.000000 libnk2-20240426/dpkg/libnk2.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      753 2024-04-26 03:27:30.000000 libnk2-20240426/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-26 03:27:30.000000 libnk2-20240426/dpkg/libnk2-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-04-26 03:27:30.000000 libnk2-20240426/dpkg/libnk2-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      119 2024-04-26 03:27:30.000000 libnk2-20240426/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2024-04-26 03:53:23.000000 libnk2-20240426/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-26 03:27:30.000000 libnk2-20240426/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-26 03:27:30.000000 libnk2-20240426/dpkg/libnk2-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      476 2024-04-26 03:53:23.000000 libnk2-20240426/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-26 03:27:30.000000 libnk2-20240426/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1921456 2024-04-26 03:53:03.000000 libnk2-20240426/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-26 03:53:04.000000 libnk2-20240426/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-26 03:53:04.000000 libnk2-20240426/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libnk2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8279 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libnk2/libnk2.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6048 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_tools_info_handle/nk2_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_item/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5862 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_item/nk2_test_item.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5545 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_error/nk2_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libclocale/libclocale.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1260 2024-04-26 03:36:01.000000 libnk2-20240426/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_record_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6050 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_record_entry/nk2_test_record_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libbfio/libbfio.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30455 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/libnk2.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_file_footer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_file_footer/nk2_test_file_footer.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5733 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_tools_output/nk2_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5788 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_notify/nk2_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libfmapi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7276 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libfmapi/libfmapi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2info/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7093 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/nk2info/nk2info.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6429 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_file/nk2_test_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libfwnt/libfwnt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6438 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_support/nk2_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5733 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_tools_signal/nk2_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_mapi_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5642 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_mapi_value/nk2_test_mapi_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_file_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_file_header/nk2_test_file_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22834 2024-04-26 03:53:05.000000 libnk2-20240426/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8076 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2export/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7662 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/nk2export/nk2export.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/nk2_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5797 2024-04-26 03:28:32.000000 libnk2-20240426/msvscpp/nk2_test_io_handle/nk2_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-26 03:28:04.000000 libnk2-20240426/msvscpp/libfdatetime/libfdatetime.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-04-26 03:27:32.000000 libnk2-20240426/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:39.000000 libnk2-20240426/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30615 2024-04-26 03:53:05.000000 libnk2-20240426/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-04-26 03:52:37.000000 libnk2-20240426/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      359 2024-04-26 03:28:58.000000 libnk2-20240426/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-26 03:53:04.000000 libnk2-20240426/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:41.000000 libnk2-20240426/pynk2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-26 03:28:58.000000 libnk2-20240426/pynk2/pynk2_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8937 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_items.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1352 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3244 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3218 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2483 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_record_entries.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1343 2024-04-26 03:36:01.000000 libnk2-20240426/pynk2/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_libnk2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26667 2024-04-26 03:28:58.000000 libnk2-20240426/pynk2/pynk2_record_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15381 2024-04-26 03:28:58.000000 libnk2-20240426/pynk2/pynk2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2842 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3187 2024-04-26 03:28:58.000000 libnk2-20240426/pynk2/pynk2_record_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30383 2024-04-26 03:28:58.000000 libnk2-20240426/pynk2/pynk2_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9479 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_record_entries.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2024-04-26 03:28:58.000000 libnk2-20240426/pynk2/pynk2_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49256 2024-04-26 03:53:05.000000 libnk2-20240426/pynk2/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1165 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2294 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_items.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1804 2024-04-26 03:27:34.000000 libnk2-20240426/pynk2/pynk2_datetime.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:38.000000 libnk2-20240426/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32528 2024-04-26 03:53:05.000000 libnk2-20240426/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-26 03:52:34.000000 libnk2-20240426/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-26 03:27:30.000000 libnk2-20240426/pyproject.toml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:40.000000 libnk2-20240426/libfmapi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   124848 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1913 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_x400_object_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2174 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_entry_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40853 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_one_off_entry_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5468 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_one_off_entry_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1543 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3422 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1506 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2927 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10342 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_entry_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2951 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_class_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3877 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2189 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_class_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1670 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_checksum.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   158504 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_property_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16455 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_lzfu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3352 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_property_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2015 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_lzfu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2780 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_service_provider_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33941 2024-04-26 03:53:05.000000 libnk2-20240426/libfmapi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1523 2024-04-26 03:52:48.000000 libnk2-20240426/libfmapi/libfmapi_service_provider_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      631 2024-04-26 03:27:30.000000 libnk2-20240426/libnk2.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      477 2024-04-26 03:27:30.000000 libnk2-20240426/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-26 03:53:04.000000 libnk2-20240426/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-26 03:27:30.000000 libnk2-20240426/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-26 03:27:30.000000 libnk2-20240426/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:11:53.000000 libnk2-20240426/config.rpath
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2257 2024-04-26 03:53:23.000000 libnk2-20240426/libnk2.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:38.000000 libnk2-20240426/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-26 03:52:44.000000 libnk2-20240426/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-26 03:52:44.000000 libnk2-20240426/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32967 2024-04-26 03:53:05.000000 libnk2-20240426/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-26 03:52:43.000000 libnk2-20240426/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-26 03:53:05.000000 libnk2-20240426/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:39.000000 libnk2-20240426/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29813 2024-04-26 03:53:05.000000 libnk2-20240426/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-04-26 03:52:41.000000 libnk2-20240426/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-12-03 09:11:53.000000 libnk2-20240426/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7287 2024-04-26 03:27:35.000000 libnk2-20240426/manuals/libnk2.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-04-26 03:27:35.000000 libnk2-20240426/manuals/nk2info.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      151 2024-04-26 03:36:01.000000 libnk2-20240426/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1975 2024-04-26 03:27:35.000000 libnk2-20240426/manuals/nk2export.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26569 2024-04-26 03:53:05.000000 libnk2-20240426/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77832 2024-04-26 03:28:32.000000 libnk2-20240426/tests/nk2_test_record_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_libnk2.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3275 2024-04-26 03:27:35.000000 libnk2-20240426/tests/test_nk2info.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7856 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12118 2024-04-26 03:28:32.000000 libnk2-20240426/tests/nk2_test_file_footer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_libcerror.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4031 2024-04-26 03:30:33.000000 libnk2-20240426/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6989 2024-04-26 03:28:58.000000 libnk2-20240426/tests/pynk2_test_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6211 2024-04-26 03:36:01.000000 libnk2-20240426/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13463 2024-04-26 03:28:32.000000 libnk2-20240426/tests/nk2_test_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11176 2024-04-26 03:28:32.000000 libnk2-20240426/tests/nk2_test_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14091 2024-04-26 03:28:32.000000 libnk2-20240426/tests/nk2_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13235 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_functions.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-26 03:27:35.000000 libnk2-20240426/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4401 2024-04-26 03:27:35.000000 libnk2-20240426/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5546 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_tools_info_handle.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4648 2024-04-26 03:42:39.000000 libnk2-20240426/tests/test_nk2export.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-26 03:27:35.000000 libnk2-20240426/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_mapi_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33596 2024-04-26 03:28:32.000000 libnk2-20240426/tests/nk2_test_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2024-04-26 03:27:35.000000 libnk2-20240426/tests/nk2_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3408 2024-04-26 03:28:58.000000 libnk2-20240426/tests/pynk2_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60805 2024-04-26 03:53:05.000000 libnk2-20240426/tests/Makefile.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4091 2024-04-26 03:30:20.000000 libnk2-20240426/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2024-04-26 03:27:34.000000 libnk2-20240426/ossfuzz/ossfuzz_libnk2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      882 2024-04-26 03:36:01.000000 libnk2-20240426/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-26 03:27:33.000000 libnk2-20240426/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-04-26 03:27:33.000000 libnk2-20240426/ossfuzz/file_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31831 2024-04-26 03:53:05.000000 libnk2-20240426/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-26 03:52:58.000000 libnk2-20240426/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:40.000000 libnk2-20240426/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_locale_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_lzxpress.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_security_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_lznt1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_security_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_access_control_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_security_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_access_control_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_lznt1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_locale_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_lzx.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_access_control_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_lzxpress.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_security_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_lzx.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33892 2024-04-26 03:53:05.000000 libnk2-20240426/libfwnt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-04-26 03:52:51.000000 libnk2-20240426/libfwnt/libfwnt_access_control_entry.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:41.000000 libnk2-20240426/nk2tools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2143 2024-04-26 03:28:58.000000 libnk2-20240426/nk2tools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1403 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5687 2024-04-26 03:28:58.000000 libnk2-20240426/nk2tools/nk2info.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libnk2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/item_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44179 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/item_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-04-26 03:36:01.000000 libnk2-20240426/nk2tools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10303 2024-04-26 03:28:58.000000 libnk2-20240426/nk2tools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10016 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2export.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39131 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/export_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2input.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4314 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5936 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/log_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8347 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2input.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5076 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/export_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libfmapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33933 2024-04-26 03:53:05.000000 libnk2-20240426/nk2tools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1672 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/log_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1756 2024-04-26 03:27:35.000000 libnk2-20240426/nk2tools/nk2tools_libfvalue.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:39.000000 libnk2-20240426/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30710 2024-04-26 03:53:05.000000 libnk2-20240426/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-04-26 03:52:42.000000 libnk2-20240426/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:42.000000 libnk2-20240426/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:12:05.000000 libnk2-20240426/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:12:05.000000 libnk2-20240426/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:12:05.000000 libnk2-20240426/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:12:05.000000 libnk2-20240426/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:12:05.000000 libnk2-20240426/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:12:05.000000 libnk2-20240426/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:12:05.000000 libnk2-20240426/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:12:05.000000 libnk2-20240426/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:12:05.000000 libnk2-20240426/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-04-26 03:53:23.000000 libnk2-20240426/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:12:05.000000 libnk2-20240426/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:12:05.000000 libnk2-20240426/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:39.000000 libnk2-20240426/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56294 2024-04-26 03:53:05.000000 libnk2-20240426/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-26 03:52:54.000000 libnk2-20240426/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40463 2024-04-26 03:53:04.000000 libnk2-20240426/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:41.000000 libnk2-20240426/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35652 2024-04-26 03:53:05.000000 libnk2-20240426/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-26 03:52:49.000000 libnk2-20240426/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:39.000000 libnk2-20240426/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29651 2024-04-26 03:53:05.000000 libnk2-20240426/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-26 03:52:40.000000 libnk2-20240426/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:38.000000 libnk2-20240426/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-26 03:52:36.000000 libnk2-20240426/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29118 2024-04-26 03:53:05.000000 libnk2-20240426/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-26 04:11:40.000000 libnk2-20240426/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32702 2024-04-26 03:53:05.000000 libnk2-20240426/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-26 03:52:45.000000 libnk2-20240426/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56826 2024-04-26 03:53:01.000000 libnk2-20240426/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7681 2024-04-26 03:27:30.000000 libnk2-20240426/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      408 2024-04-26 04:11:43.687178 libnk2-20240426/PKG-INFO
```

### Comparing `libnk2-20240210/libnk2/libnk2_libuna.h` & `libnk2-20240426/libnk2/libnk2_libuna.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_libcerror.h` & `libnk2-20240426/libnk2/libnk2_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_definitions.h` & `libnk2-20240426/libnk2/libnk2_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBNK2 )
 #include <libnk2/definitions.h>
 
 /* The definitions in <libnk2/definitions.h> are copied here
  * for local use of libnk2
  */
 #else
-#define LIBNK2_VERSION					20240210
+#define LIBNK2_VERSION					20240426
 
 /* The version string
  */
-#define LIBNK2_VERSION_STRING				"20240210"
+#define LIBNK2_VERSION_STRING				"20240426"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBNK2_ACCESS_FLAGS
```

### Comparing `libnk2-20240210/libnk2/libnk2_types.h` & `libnk2-20240426/libnk2/libnk2_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_record_entry.c` & `libnk2-20240426/libnk2/libnk2_record_entry.c`

 * *Files 0% similar despite different names*

```diff
@@ -687,32 +687,22 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid data.",
 		 function );
 
 		return( -1 );
 	}
-	if( data_size > (size_t) SSIZE_MAX )
+	if( ( data_size < internal_record_entry->value_data_size )
+	 || ( data_size > (size_t) SSIZE_MAX ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
-		 "%s: invalid data size value exceeds maximum.",
-		 function );
-
-		return( -1 );
-	}
-	if( data_size < internal_record_entry->value_data_size )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
-		 "%s: invalid data value too small.",
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid data size value out of bounds.",
 		 function );
 
 		return( -1 );
 	}
 	if( memory_copy(
 	     data,
 	     internal_record_entry->value_data,
```

### Comparing `libnk2-20240210/libnk2/libnk2_unused.h` & `libnk2-20240426/libnk2/libnk2_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_file.h` & `libnk2-20240426/libnk2/libnk2_file.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_libbfio.h` & `libnk2-20240426/libnk2/libnk2_libbfio.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_record_entry.h` & `libnk2-20240426/libnk2/libnk2_record_entry.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_file.c` & `libnk2-20240426/libnk2/libnk2_file.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_error.h` & `libnk2-20240426/libnk2/libnk2_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2.c` & `libnk2-20240426/libnk2/libnk2.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_debug.h` & `libnk2-20240426/libnk2/libnk2_debug.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_support.h` & `libnk2-20240426/libnk2/libnk2_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_error.c` & `libnk2-20240426/libnk2/libnk2_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_support.c` & `libnk2-20240426/libnk2/libnk2_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_definitions.h.in` & `libnk2-20240426/libnk2/libnk2_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_codepage.h` & `libnk2-20240426/libnk2/libnk2_codepage.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/Makefile.am` & `libnk2-20240426/libnk2/Makefile.am`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -67,21 +67,19 @@
 libnk2_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libnk2_definitions.h.in \
 	libnk2.rc \
 	libnk2.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libnk2_definitions.h \
+	libnk2.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libnk2_definitions.h
-	-rm -f libnk2.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libnk2 ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libnk2_la_SOURCES)
```

### Comparing `libnk2-20240210/libnk2/libnk2.rc` & `libnk2-20240426/libnk2/libnk2.rc`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Nickfile (NK2) format\0"
-      VALUE "FileVersion",		"20240210" "\0"
+      VALUE "FileVersion",		"20240426" "\0"
       VALUE "InternalName",		"libnk2.dll\0"
       VALUE "LegalCopyright",		"(C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libnk2.dll\0"
       VALUE "ProductName",		"libnk2\0"
-      VALUE "ProductVersion",		"20240210" "\0"
+      VALUE "ProductVersion",		"20240426" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libnk2/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libnk2-20240210/libnk2/libnk2_item.c` & `libnk2-20240426/libnk2/libnk2_item.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/nk2_file_header.h` & `libnk2-20240426/libnk2/nk2_file_header.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/nk2_item.h` & `libnk2-20240426/libnk2/nk2_item.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_file_footer.h` & `libnk2-20240426/libnk2/libnk2_file_footer.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_libcdata.h` & `libnk2-20240426/libnk2/libnk2_libcdata.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_libfdatetime.h` & `libnk2-20240426/libnk2/libnk2_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_libcnotify.h` & `libnk2-20240426/libnk2/libnk2_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_mapi.h` & `libnk2-20240426/libnk2/libnk2_mapi.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_file_footer.c` & `libnk2-20240426/libnk2/libnk2_file_footer.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_io_handle.h` & `libnk2-20240426/libnk2/libnk2_io_handle.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_libclocale.h` & `libnk2-20240426/libnk2/libnk2_libclocale.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_file_header.c` & `libnk2-20240426/libnk2/libnk2_file_header.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_debug.c` & `libnk2-20240426/libnk2/libnk2_debug.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_file_header.h` & `libnk2-20240426/libnk2/libnk2_file_header.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_mapi_value.h` & `libnk2-20240426/libnk2/libnk2_mapi_value.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_notify.c` & `libnk2-20240426/libnk2/libnk2_notify.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_libfmapi.h` & `libnk2-20240426/libnk2/libnk2_libfmapi.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_notify.h` & `libnk2-20240426/libnk2/libnk2_notify.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_extern.h` & `libnk2-20240426/libnk2/libnk2_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/nk2_file_footer.h` & `libnk2-20240426/libnk2/nk2_file_footer.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_item.h` & `libnk2-20240426/libnk2/libnk2_item.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2_io_handle.c` & `libnk2-20240426/libnk2/libnk2_io_handle.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/Makefile.in` & `libnk2-20240426/libnk2/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -544,16 +544,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -614,15 +614,18 @@
 
 libnk2_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libnk2_definitions.h.in \
 	libnk2.rc \
 	libnk2.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libnk2_definitions.h \
+	libnk2.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -864,24 +867,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libnk2.Plo
+	-rm -f ./$(DEPDIR)/libnk2_debug.Plo
+	-rm -f ./$(DEPDIR)/libnk2_error.Plo
+	-rm -f ./$(DEPDIR)/libnk2_file.Plo
+	-rm -f ./$(DEPDIR)/libnk2_file_footer.Plo
+	-rm -f ./$(DEPDIR)/libnk2_file_header.Plo
+	-rm -f ./$(DEPDIR)/libnk2_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libnk2_item.Plo
+	-rm -f ./$(DEPDIR)/libnk2_mapi_value.Plo
+	-rm -f ./$(DEPDIR)/libnk2_notify.Plo
+	-rm -f ./$(DEPDIR)/libnk2_record_entry.Plo
+	-rm -f ./$(DEPDIR)/libnk2_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -976,19 +993,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libnk2_definitions.h
-	-rm -f libnk2.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libnk2 ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libnk2_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libnk2/libnk2_mapi_value.c` & `libnk2-20240426/libnk2/libnk2_mapi_value.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2/libnk2.rc.in` & `libnk2-20240426/libnk2/libnk2.rc.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/COPYING` & `libnk2-20240426/COPYING`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/install-sh` & `libnk2-20240426/install-sh`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2.spec.in` & `libnk2-20240426/libnk2.spec.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/depcomp` & `libnk2-20240426/depcomp`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfguid/libfguid_error.c` & `libnk2-20240426/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfguid/libfguid_support.h` & `libnk2-20240426/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfguid/libfguid_identifier.h` & `libnk2-20240426/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfguid/libfguid_libcerror.h` & `libnk2-20240426/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfguid/Makefile.am` & `libnk2-20240426/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libnk2-20240210/libfguid/libfguid_unused.h` & `libnk2-20240426/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfguid/libfguid_extern.h` & `libnk2-20240426/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfguid/libfguid_types.h` & `libnk2-20240426/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfguid/libfguid_identifier.c` & `libnk2-20240426/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfguid/libfguid_support.c` & `libnk2-20240426/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfguid/libfguid_definitions.h` & `libnk2-20240426/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libnk2-20240210/libfguid/Makefile.in` & `libnk2-20240426/libfguid/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -511,30 +511,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -736,24 +737,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -839,17 +845,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libfguid/libfguid_error.h` & `libnk2-20240426/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/libfwnt.m4` & `libnk2-20240426/m4/libfwnt.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfwnt required headers and functions
 dnl
-dnl Version: 20191217
+dnl Version: 20240413
 
 dnl Function to detect if libfwnt is available
 dnl ac_libfwnt_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFWNT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwnt" = xno],
     [ac_cv_libfwnt=no],
     [ac_cv_libfwnt=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfwnt which returns "yes" and --with-libfwnt= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect],
+      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfwnt"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfwnt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwnt}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfwnt],
           [1])
@@ -214,16 +216,17 @@
           fwnt,
           libfwnt_lzxpress_huffman_decompress,
           [ac_cv_libfwnt_dummy=yes],
           [ac_cv_libfwnt=no])
 
         ac_cv_libfwnt_LIBADD="-lfwnt"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_libfwnt" != xyes],
+      [test "x$ac_cv_libfwnt" != xyes && test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfwnt in directory: $ac_cv_with_libfwnt],
         [1])
       ])
     ])
 
   AS_IF(
@@ -245,15 +248,15 @@
     ])
   ])
 
 dnl Function to detect if libfwnt dependencies are available
 AC_DEFUN([AX_LIBFWNT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
   ])
 
 dnl Function to detect how to enable libfwnt
 AC_DEFUN([AX_LIBFWNT_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/libcfile.m4` & `libnk2-20240426/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/libfdatetime.m4` & `libnk2-20240426/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/tests.m4` & `libnk2-20240426/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/libcpath.m4` & `libnk2-20240426/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/lib-prefix.m4` & `libnk2-20240426/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/progtest.m4` & `libnk2-20240426/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/libuna.m4` & `libnk2-20240426/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/gettext.m4` & `libnk2-20240426/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/lib-ld.m4` & `libnk2-20240426/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/libclocale.m4` & `libnk2-20240426/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/libcdata.m4` & `libnk2-20240426/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/libcsplit.m4` & `libnk2-20240426/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/common.m4` & `libnk2-20240426/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libnk2-20240210/m4/libcthreads.m4` & `libnk2-20240426/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libnk2-20240210/m4/ltversion.m4` & `libnk2-20240426/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/ltsugar.m4` & `libnk2-20240426/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/host-cpu-c-abi.m4` & `libnk2-20240426/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/libtool.m4` & `libnk2-20240426/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/po.m4` & `libnk2-20240426/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/libcerror.m4` & `libnk2-20240426/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/libcnotify.m4` & `libnk2-20240426/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/libfguid.m4` & `libnk2-20240426/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libnk2-20240210/m4/libbfio.m4` & `libnk2-20240426/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/libfmapi.m4` & `libnk2-20240426/m4/libfmapi.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfmapi required headers and functions
 dnl
-dnl Version: 20230404
+dnl Version: 20240413
 
 dnl Function to detect if libfmapi is available
 dnl ac_libfmapi_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFMAPI_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfmapi" = xno],
     [ac_cv_libfmapi=no],
     [ac_cv_libfmapi=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfmapi which returns "yes" and --with-libfmapi= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect],
+      [test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_with_libfmapi" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfmapi"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfmapi}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfmapi}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfmapi],
           [1])
@@ -179,16 +181,17 @@
           fmapi,
           libfmapi_lzfu_decompress,
           [ac_cv_libfmapi_dummy=yes],
           [ac_cv_libfmapi=no])
 
         ac_cv_libfmapi_LIBADD="-lfmapi"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_libfmapi" != xyes],
+      [test "x$ac_cv_libfmapi" != xyes && test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_with_libfmapi" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfmapi in directory: $ac_cv_with_libfmapi],
         [1])
       ])
     ])
 
   dnl Check for debug functions
@@ -236,15 +239,15 @@
     ])
   ])
 
 dnl Function to detect if libfmapi dependencies are available
 AC_DEFUN([AX_LIBFMAPI_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfmapi_CPPFLAGS="-I../libfmapi";
+  ac_cv_libfmapi_CPPFLAGS="-I../libfmapi -I\$(top_srcdir)/libfmapi";
   ac_cv_libfmapi_LIBADD="../libfmapi/libfmapi.la";
 
   ac_cv_libfmapi=local
   ])
 
 dnl Function to detect how to enable libfmapi
 AC_DEFUN([AX_LIBFMAPI_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/intlmacosx.m4` & `libnk2-20240426/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/lt~obsolete.m4` & `libnk2-20240426/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/lib-link.m4` & `libnk2-20240426/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/iconv.m4` & `libnk2-20240426/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/ltoptions.m4` & `libnk2-20240426/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/nls.m4` & `libnk2-20240426/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/python.m4` & `libnk2-20240426/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libnk2-20240210/m4/libfvalue.m4` & `libnk2-20240426/m4/libfvalue.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfvalue required headers and functions
 dnl
-dnl Version: 20200711
+dnl Version: 20240413
 
 dnl Function to detect if libfvalue is available
 dnl ac_libfvalue_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFVALUE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno],
     [ac_cv_libfvalue=no],
     [ac_cv_libfvalue=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfvalue which returns "yes" and --with-libfvalue= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect],
+      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfvalue"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfvalue],
           [1])
@@ -585,16 +587,17 @@
           fvalue,
           libfvalue_value_type_set_data_strings_array,
           [ac_cv_libfvalue_dummy=yes],
           [ac_cv_libfvalue=no])
 
         ac_cv_libfvalue_LIBADD="-lfvalue"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes],
+      [test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfvalue in directory: $ac_cv_with_libfvalue],
         [1])
       ])
     ])
 
   AS_IF(
@@ -616,15 +619,15 @@
     ])
   ])
 
 dnl Function to detect if libfvalue dependencies are available
 AC_DEFUN([AX_LIBFVALUE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
   ])
 
 dnl Function to detect how to enable libfvalue
 AC_DEFUN([AX_LIBFVALUE_CHECK_ENABLE],
```

### Comparing `libnk2-20240210/m4/types.m4` & `libnk2-20240426/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/m4/pthread.m4` & `libnk2-20240426/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libnk2-20240210/include/libnk2/definitions.h.in` & `libnk2-20240426/include/libnk2/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/include/libnk2/definitions.h` & `libnk2-20240426/include/libnk2/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBNK2_DEFINITIONS_H )
 #define _LIBNK2_DEFINITIONS_H
 
 #include <libnk2/types.h>
 
-#define LIBNK2_VERSION					20240210
+#define LIBNK2_VERSION					20240426
 
 /* The version string
  */
-#define LIBNK2_VERSION_STRING				"20240210"
+#define LIBNK2_VERSION_STRING				"20240426"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBNK2_ACCESS_FLAGS
```

### Comparing `libnk2-20240210/include/libnk2/types.h.in` & `libnk2-20240426/include/libnk2/types.h.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/include/libnk2/types.h` & `libnk2-20240426/include/libnk2/types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/include/libnk2/mapi.h` & `libnk2-20240426/include/libnk2/mapi.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/include/libnk2/features.h.in` & `libnk2-20240426/include/libnk2/features.h.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/include/libnk2/error.h` & `libnk2-20240426/include/libnk2/error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/include/libnk2/extern.h` & `libnk2-20240426/include/libnk2/extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/include/libnk2/features.h` & `libnk2-20240426/include/libnk2/features.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/include/libnk2/codepage.h` & `libnk2-20240426/include/libnk2/codepage.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/include/libnk2.h.in` & `libnk2-20240426/include/libnk2.h.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/include/Makefile.in` & `libnk2-20240426/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -518,15 +518,20 @@
 
 EXTRA_DIST = \
 	libnk2.h.in \
 	libnk2/definitions.h.in \
 	libnk2/features.h.in \
 	libnk2/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libnk2.h \
+	libnk2/definitions.h \
+	libnk2/features.h \
+	libnk2/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -723,23 +728,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -821,17 +828,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libnk2.h
-	-rm -f libnk2/definitions.h
-	-rm -f libnk2/features.h
-	-rm -f libnk2/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libnk2-20240210/include/libnk2.h` & `libnk2-20240426/include/libnk2.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/config_borlandc.h` & `libnk2-20240426/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/file_stream.h` & `libnk2-20240426/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/memory.h` & `libnk2-20240426/common/memory.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/byte_stream.h` & `libnk2-20240426/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/common.h` & `libnk2-20240426/common/common.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/config_winapi.h` & `libnk2-20240426/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/system_string.h` & `libnk2-20240426/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/types.h.in` & `libnk2-20240426/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/types.h` & `libnk2-20240426/common/types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/config.h.in` & `libnk2-20240426/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/config.h` & `libnk2-20240426/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -523,24 +523,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libnk2"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libnk2 20240210"
+#define PACKAGE_STRING "libnk2 20240426"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libnk2"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240210"
+#define PACKAGE_VERSION "20240426"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -558,15 +558,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240210"
+#define VERSION "20240426"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libnk2-20240210/common/wide_string.h` & `libnk2-20240426/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/narrow_string.h` & `libnk2-20240426/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/config_msc.h` & `libnk2-20240426/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/common/Makefile.in` & `libnk2-20240426/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -470,15 +470,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -486,15 +488,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -662,23 +667,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -758,15 +765,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libnk2-20240210/libclocale/libclocale_wide_string.c` & `libnk2-20240426/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libclocale/libclocale_support.h` & `libnk2-20240426/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libclocale/Makefile.am` & `libnk2-20240426/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libnk2-20240210/libclocale/libclocale_definitions.h` & `libnk2-20240426/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libnk2-20240210/libclocale/libclocale_unused.h` & `libnk2-20240426/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libclocale/libclocale_libcerror.h` & `libnk2-20240426/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libclocale/libclocale_locale.h` & `libnk2-20240426/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libclocale/libclocale_support.c` & `libnk2-20240426/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libclocale/libclocale_codepage.c` & `libnk2-20240426/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libclocale/libclocale_locale.c` & `libnk2-20240426/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libclocale/Makefile.in` & `libnk2-20240426/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -516,30 +516,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -742,24 +743,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -846,17 +853,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libclocale/libclocale_extern.h` & `libnk2-20240426/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libclocale/libclocale_wide_string.h` & `libnk2-20240426/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libclocale/libclocale_codepage.h` & `libnk2-20240426/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/Makefile.am` & `libnk2-20240426/Makefile.am`

 * *Files 10% similar despite different names*

```diff
@@ -60,16 +60,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libnk2.pc \
+	libnk2.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libnk2.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -92,19 +99,7 @@
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfmapi && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libnk2 && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libnk2.pc
-	-rm -f libnk2.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libnk2-20240210/libbfio/libbfio_file_range.h` & `libnk2-20240426/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_file_range_io_handle.c` & `libnk2-20240426/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_support.c` & `libnk2-20240426/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_libcpath.h` & `libnk2-20240426/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_error.h` & `libnk2-20240426/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_libclocale.h` & `libnk2-20240426/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_error.c` & `libnk2-20240426/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_libuna.h` & `libnk2-20240426/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_file_io_handle.h` & `libnk2-20240426/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_file_pool.h` & `libnk2-20240426/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_file_range.c` & `libnk2-20240426/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_types.h` & `libnk2-20240426/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_unused.h` & `libnk2-20240426/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_libcdata.h` & `libnk2-20240426/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_file.h` & `libnk2-20240426/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/Makefile.am` & `libnk2-20240426/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libnk2-20240210/libbfio/libbfio_libcfile.h` & `libnk2-20240426/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_definitions.h` & `libnk2-20240426/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libnk2-20240210/libbfio/libbfio_codepage.h` & `libnk2-20240426/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_file_io_handle.c` & `libnk2-20240426/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_support.h` & `libnk2-20240426/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_memory_range.h` & `libnk2-20240426/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_file_pool.c` & `libnk2-20240426/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_file_range_io_handle.h` & `libnk2-20240426/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_libcthreads.h` & `libnk2-20240426/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_system_string.h` & `libnk2-20240426/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_memory_range_io_handle.c` & `libnk2-20240426/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_handle.c` & `libnk2-20240426/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_file.c` & `libnk2-20240426/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_handle.h` & `libnk2-20240426/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_memory_range.c` & `libnk2-20240426/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_pool.c` & `libnk2-20240426/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_libcerror.h` & `libnk2-20240426/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/Makefile.in` & `libnk2-20240426/libbfio/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -536,16 +536,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -576,15 +576,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -795,24 +796,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -881,14 +896,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -899,23 +916,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libnk2-20240210/libbfio/libbfio_system_string.c` & `libnk2-20240426/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_memory_range_io_handle.h` & `libnk2-20240426/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_extern.h` & `libnk2-20240426/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/libbfio/libbfio_pool.h` & `libnk2-20240426/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libnk2-20240210/config.guess` & `libnk2-20240426/config.guess`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/dpkg/copyright` & `libnk2-20240426/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/dpkg/control` & `libnk2-20240426/dpkg/control`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/dpkg/rules` & `libnk2-20240426/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/COPYING.LESSER` & `libnk2-20240426/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/configure` & `libnk2-20240426/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libnk2 20240210.
+# Generated by GNU Autoconf 2.71 for libnk2 20240426.
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
 PACKAGE_NAME='libnk2'
 PACKAGE_TARNAME='libnk2'
-PACKAGE_VERSION='20240210'
-PACKAGE_STRING='libnk2 20240210'
+PACKAGE_VERSION='20240426'
+PACKAGE_STRING='libnk2 20240426'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libnk2.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1654,15 +1654,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libnk2 20240210 to adapt to many kinds of systems.
+\`configure' configures libnk2 20240426 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1725,15 +1725,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libnk2 20240210:";;
+     short | recursive ) echo "Configuration of libnk2 20240426:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1977,15 +1977,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libnk2 configure 20240210
+libnk2 configure 20240426
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2698,15 +2698,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libnk2 $as_me 20240210, which was
+It was created by libnk2 $as_me 20240426, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4187,15 +4187,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libnk2'
- VERSION='20240210'
+ VERSION='20240426'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23782,15 +23782,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24281,15 +24281,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24431,15 +24432,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24533,15 +24534,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26173,15 +26174,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26235,47 +26236,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26309,15 +26315,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26351,15 +26357,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26394,15 +26400,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26436,15 +26442,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26478,15 +26484,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26520,15 +26526,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26562,15 +26568,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26605,15 +26611,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26647,15 +26653,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26689,15 +26695,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26731,15 +26737,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26773,15 +26779,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26816,15 +26822,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26858,15 +26864,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26900,15 +26906,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26942,15 +26948,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26984,15 +26990,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27027,67 +27033,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27175,15 +27190,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30954,15 +30969,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30987,15 +31003,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31065,15 +31081,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31620,15 +31636,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31784,15 +31801,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31862,15 +31879,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32320,15 +32337,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32383,15 +32401,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32461,15 +32479,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33184,15 +33202,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33217,15 +33236,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33295,15 +33314,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40505,15 +40524,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40538,15 +40558,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40616,15 +40636,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41805,15 +41825,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42127,15 +42148,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42205,15 +42226,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43010,15 +43031,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43208,15 +43230,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43286,15 +43308,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45404,15 +45426,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45437,15 +45460,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45515,15 +45538,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -48959,15 +48982,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -48992,15 +49016,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -49070,15 +49094,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49652,15 +49676,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49685,15 +49710,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -49763,15 +49788,15 @@
 printf "%s\n" "$ac_cv_with_libfwnt" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwnt" = xno
 then :
   ac_cv_libfwnt=no
 else $as_nop
   ac_cv_libfwnt=check
-        if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect
+                if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes
 then :
   if test -d "$ac_cv_with_libfwnt"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfwnt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwnt}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -51153,15 +51178,16 @@
 fi
 
 
         ac_cv_libfwnt_LIBADD="-lfwnt"
 fi
 
 fi
-    if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_libfwnt" != xyes
+
+    if test "x$ac_cv_libfwnt" != xyes && test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfwnt in directory: $ac_cv_with_libfwnt
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -51186,15 +51212,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfwnt" != xyes
 then :
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFWNT 1" >>confdefs.h
@@ -51264,15 +51290,15 @@
 printf "%s\n" "$ac_cv_with_libfmapi" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfmapi" = xno
 then :
   ac_cv_libfmapi=no
 else $as_nop
   ac_cv_libfmapi=check
-        if test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect
+                if test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_with_libfmapi" != xyes
 then :
   if test -d "$ac_cv_with_libfmapi"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfmapi}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfmapi}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -52437,15 +52463,16 @@
 fi
 
 
         ac_cv_libfmapi_LIBADD="-lfmapi"
 fi
 
 fi
-    if test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_libfmapi" != xyes
+
+    if test "x$ac_cv_libfmapi" != xyes && test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_with_libfmapi" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfmapi in directory: $ac_cv_with_libfmapi
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -52644,15 +52671,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfmapi" != xyes
 then :
 
-  ac_cv_libfmapi_CPPFLAGS="-I../libfmapi";
+  ac_cv_libfmapi_CPPFLAGS="-I../libfmapi -I\$(top_srcdir)/libfmapi";
   ac_cv_libfmapi_LIBADD="../libfmapi/libfmapi.la";
 
   ac_cv_libfmapi=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFMAPI 1" >>confdefs.h
@@ -52963,16 +52990,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -53135,15 +53166,15 @@
 printf "%s\n" "$ac_cv_with_libfvalue" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno
 then :
   ac_cv_libfvalue=no
 else $as_nop
   ac_cv_libfvalue=check
-        if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect
+                if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   if test -d "$ac_cv_with_libfvalue"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -57449,15 +57480,16 @@
 fi
 
 
         ac_cv_libfvalue_LIBADD="-lfvalue"
 fi
 
 fi
-    if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes
+
+    if test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfvalue in directory: $ac_cv_with_libfvalue
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -57482,15 +57514,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -58444,15 +58476,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libnk2 $as_me 20240210, which was
+This file was extended by libnk2 $as_me 20240426, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -58512,15 +58544,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libnk2 config.status 20240210
+libnk2 config.status 20240426
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libnk2-20240210/compile` & `libnk2-20240426/compile`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/missing` & `libnk2-20240426/missing`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libnk2/libnk2.vcproj` & `libnk2-20240426/msvscpp/libnk2/libnk2.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libfguid/libfguid.vcproj` & `libnk2-20240426/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_tools_info_handle/nk2_test_tools_info_handle.vcproj` & `libnk2-20240426/msvscpp/nk2_test_tools_info_handle/nk2_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_item/nk2_test_item.vcproj` & `libnk2-20240426/msvscpp/nk2_test_item/nk2_test_item.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_error/nk2_test_error.vcproj` & `libnk2-20240426/msvscpp/nk2_test_error/nk2_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libclocale/libclocale.vcproj` & `libnk2-20240426/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/Makefile.am` & `libnk2-20240426/msvscpp/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -31,13 +31,11 @@
 	nk2export/nk2export.vcproj \
 	nk2info/nk2info.vcproj \
 	libnk2.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libnk2-20240210/msvscpp/nk2_test_record_entry/nk2_test_record_entry.vcproj` & `libnk2-20240426/msvscpp/nk2_test_record_entry/nk2_test_record_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libbfio/libbfio.vcproj` & `libnk2-20240426/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libnk2.sln` & `libnk2-20240426/msvscpp/libnk2.sln`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_file_footer/nk2_test_file_footer.vcproj` & `libnk2-20240426/msvscpp/nk2_test_file_footer/nk2_test_file_footer.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_tools_output/nk2_test_tools_output.vcproj` & `libnk2-20240426/msvscpp/nk2_test_tools_output/nk2_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libcfile/libcfile.vcproj` & `libnk2-20240426/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_notify/nk2_test_notify.vcproj` & `libnk2-20240426/msvscpp/nk2_test_notify/nk2_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libcdata/libcdata.vcproj` & `libnk2-20240426/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libfmapi/libfmapi.vcproj` & `libnk2-20240426/msvscpp/libfmapi/libfmapi.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2info/nk2info.vcproj` & `libnk2-20240426/msvscpp/nk2info/nk2info.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_file/nk2_test_file.vcproj` & `libnk2-20240426/msvscpp/nk2_test_file/nk2_test_file.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libcthreads/libcthreads.vcproj` & `libnk2-20240426/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libcpath/libcpath.vcproj` & `libnk2-20240426/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libfwnt/libfwnt.vcproj` & `libnk2-20240426/msvscpp/libfwnt/libfwnt.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_support/nk2_test_support.vcproj` & `libnk2-20240426/msvscpp/nk2_test_support/nk2_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_tools_signal/nk2_test_tools_signal.vcproj` & `libnk2-20240426/msvscpp/nk2_test_tools_signal/nk2_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libcsplit/libcsplit.vcproj` & `libnk2-20240426/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_mapi_value/nk2_test_mapi_value.vcproj` & `libnk2-20240426/msvscpp/nk2_test_mapi_value/nk2_test_mapi_value.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_file_header/nk2_test_file_header.vcproj` & `libnk2-20240426/msvscpp/nk2_test_file_header/nk2_test_file_header.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libuna/libuna.vcproj` & `libnk2-20240426/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/Makefile.in` & `libnk2-20240426/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -489,15 +489,16 @@
 	nk2export/nk2export.vcproj \
 	nk2info/nk2info.vcproj \
 	libnk2.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -601,23 +602,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -696,13 +699,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libnk2-20240210/msvscpp/libfvalue/libfvalue.vcproj` & `libnk2-20240426/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libcnotify/libcnotify.vcproj` & `libnk2-20240426/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2export/nk2export.vcproj` & `libnk2-20240426/msvscpp/nk2export/nk2export.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libcerror/libcerror.vcproj` & `libnk2-20240426/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/nk2_test_io_handle/nk2_test_io_handle.vcproj` & `libnk2-20240426/msvscpp/nk2_test_io_handle/nk2_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/msvscpp/libfdatetime/libfdatetime.vcproj` & `libnk2-20240426/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_extern.h` & `libnk2-20240426/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_support.h` & `libnk2-20240426/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_unused.h` & `libnk2-20240426/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_notify.h` & `libnk2-20240426/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_support.c` & `libnk2-20240426/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_types.h` & `libnk2-20240426/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/Makefile.am` & `libnk2-20240426/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libnk2-20240210/libcfile/libcfile_notify.c` & `libnk2-20240426/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_system_string.h` & `libnk2-20240426/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_file.h` & `libnk2-20240426/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_libcnotify.h` & `libnk2-20240426/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_system_string.c` & `libnk2-20240426/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_error.h` & `libnk2-20240426/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_libcerror.h` & `libnk2-20240426/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_file.c` & `libnk2-20240426/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_libclocale.h` & `libnk2-20240426/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_winapi.h` & `libnk2-20240426/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/Makefile.in` & `libnk2-20240426/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -518,16 +518,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -542,15 +542,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -755,24 +756,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -861,17 +870,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libcfile/libcfile_error.c` & `libnk2-20240426/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_libuna.h` & `libnk2-20240426/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_winapi.c` & `libnk2-20240426/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcfile/libcfile_definitions.h` & `libnk2-20240426/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libnk2-20240210/INSTALL` & `libnk2-20240426/INSTALL`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_file_object_io_handle.c` & `libnk2-20240426/pynk2/pynk2_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_item.c` & `libnk2-20240426/pynk2/pynk2_item.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_items.c` & `libnk2-20240426/pynk2/pynk2_items.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_libfguid.h` & `libnk2-20240426/pynk2/pynk2_libfguid.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_file.h` & `libnk2-20240426/pynk2/pynk2_file.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_codepage.c` & `libnk2-20240426/pynk2/pynk2_codepage.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_error.h` & `libnk2-20240426/pynk2/pynk2_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_record_entries.h` & `libnk2-20240426/pynk2/pynk2_record_entries.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/Makefile.am` & `libnk2-20240426/pynk2/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -49,13 +49,11 @@
 	@LIBFGUID_LIBADD@
 
 pynk2_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pynk2_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libnk2-20240210/pynk2/pynk2_unused.h` & `libnk2-20240426/pynk2/pynk2_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_datetime.c` & `libnk2-20240426/pynk2/pynk2_datetime.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_integer.h` & `libnk2-20240426/pynk2/pynk2_integer.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_libnk2.h` & `libnk2-20240426/pynk2/pynk2_libnk2.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_file_object_io_handle.h` & `libnk2-20240426/pynk2/pynk2_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_record_entry.c` & `libnk2-20240426/pynk2/pynk2_record_entry.c`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 	  "get_value_type() -> Integer or None\n"
 	  "\n"
 	  "Retrieves the value type." },
 
 	{ "get_data",
 	  (PyCFunction) pynk2_record_entry_get_data,
 	  METH_NOARGS,
-	  "get_data() -> Binary string or None\n"
+	  "get_data() -> Bytes or None\n"
 	  "\n"
 	  "Retrieves the data." },
 
 	{ "get_data_as_boolean",
 	  (PyCFunction) pynk2_record_entry_get_data_as_boolean,
 	  METH_NOARGS,
 	  "get_data_as_boolean() -> Integer or None\n"
```

### Comparing `libnk2-20240210/pynk2/pynk2.c` & `libnk2-20240426/pynk2/pynk2.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_error.c` & `libnk2-20240426/pynk2/pynk2_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2.h` & `libnk2-20240426/pynk2/pynk2.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_libbfio.h` & `libnk2-20240426/pynk2/pynk2_libbfio.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_guid.c` & `libnk2-20240426/pynk2/pynk2_guid.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_record_entry.h` & `libnk2-20240426/pynk2/pynk2_record_entry.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_file.c` & `libnk2-20240426/pynk2/pynk2_file.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_python.h` & `libnk2-20240426/pynk2/pynk2_python.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_integer.c` & `libnk2-20240426/pynk2/pynk2_integer.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_codepage.h` & `libnk2-20240426/pynk2/pynk2_codepage.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_libclocale.h` & `libnk2-20240426/pynk2/pynk2_libclocale.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_record_entries.c` & `libnk2-20240426/pynk2/pynk2_record_entries.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_item.h` & `libnk2-20240426/pynk2/pynk2_item.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/Makefile.in` & `libnk2-20240426/pynk2/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -565,16 +565,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -614,15 +614,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_LIBADD@
 
 @HAVE_PYTHON_TRUE@pynk2_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pynk2_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -944,24 +945,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pynk2_la-pynk2.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_codepage.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_datetime.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_error.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_file.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_guid.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_integer.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_item.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_items.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_record_entries.Plo
+	-rm -f ./$(DEPDIR)/pynk2_la-pynk2_record_entry.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1057,13 +1072,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libnk2-20240210/pynk2/pynk2_libcerror.h` & `libnk2-20240426/pynk2/pynk2_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_guid.h` & `libnk2-20240426/pynk2/pynk2_guid.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_items.h` & `libnk2-20240426/pynk2/pynk2_items.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/pynk2/pynk2_datetime.h` & `libnk2-20240426/pynk2/pynk2_datetime.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_list_element.h` & `libnk2-20240426/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_array.h` & `libnk2-20240426/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_definitions.h` & `libnk2-20240426/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libnk2-20240210/libcdata/libcdata_libcerror.h` & `libnk2-20240426/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_unused.h` & `libnk2-20240426/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_btree.h` & `libnk2-20240426/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_btree.c` & `libnk2-20240426/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_support.c` & `libnk2-20240426/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_list.c` & `libnk2-20240426/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_extern.h` & `libnk2-20240426/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_list.h` & `libnk2-20240426/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_btree_values_list.h` & `libnk2-20240426/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/Makefile.am` & `libnk2-20240426/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libnk2-20240210/libcdata/libcdata_btree_node.h` & `libnk2-20240426/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_range_list_value.h` & `libnk2-20240426/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_range_list.h` & `libnk2-20240426/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_range_list.c` & `libnk2-20240426/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_array.c` & `libnk2-20240426/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_list_element.c` & `libnk2-20240426/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_libcthreads.h` & `libnk2-20240426/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_tree_node.h` & `libnk2-20240426/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_error.h` & `libnk2-20240426/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_types.h` & `libnk2-20240426/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_btree_node.c` & `libnk2-20240426/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_tree_node.c` & `libnk2-20240426/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_support.h` & `libnk2-20240426/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/Makefile.in` & `libnk2-20240426/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -532,16 +532,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -558,15 +558,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -776,24 +777,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -887,17 +901,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libcdata/libcdata_range_list_value.c` & `libnk2-20240426/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_btree_values_list.c` & `libnk2-20240426/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcdata/libcdata_error.c` & `libnk2-20240426/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_value_type.h` & `libnk2-20240426/libfmapi/libfmapi_value_type.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_debug.c` & `libnk2-20240426/libfmapi/libfmapi_debug.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_x400_object_identifier.h` & `libnk2-20240426/libfmapi/libfmapi_x400_object_identifier.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_libfguid.h` & `libnk2-20240426/libfmapi/libfmapi_libfguid.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_libcnotify.h` & `libnk2-20240426/libfmapi/libfmapi_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_entry_identifier.h` & `libnk2-20240426/libfmapi/libfmapi_entry_identifier.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_libfwnt.h` & `libnk2-20240426/libfmapi/libfmapi_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_one_off_entry_identifier.c` & `libnk2-20240426/libfmapi/libfmapi_one_off_entry_identifier.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_one_off_entry_identifier.h` & `libnk2-20240426/libfmapi/libfmapi_one_off_entry_identifier.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_codepage.h` & `libnk2-20240426/libfmapi/libfmapi_codepage.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_codepage.c` & `libnk2-20240426/libfmapi/libfmapi_codepage.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/Makefile.am` & `libnk2-20240426/libfmapi/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFMAPI
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -36,19 +36,17 @@
 	libfmapi_support.c libfmapi_support.h \
 	libfmapi_types.h \
 	libfmapi_unused.h \
 	libfmapi_value_type.c libfmapi_value_type.h \
 	libfmapi_x400_object_identifier.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfmapi ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfmapi_la_SOURCES)
```

### Comparing `libnk2-20240210/libfmapi/libfmapi_error.h` & `libnk2-20240426/libfmapi/libfmapi_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_debug.h` & `libnk2-20240426/libfmapi/libfmapi_debug.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_entry_identifier.c` & `libnk2-20240426/libfmapi/libfmapi_entry_identifier.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_class_identifier.h` & `libnk2-20240426/libfmapi/libfmapi_class_identifier.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_value_type.c` & `libnk2-20240426/libfmapi/libfmapi_value_type.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_libuna.h` & `libnk2-20240426/libfmapi/libfmapi_libuna.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_definitions.h` & `libnk2-20240426/libfmapi/libfmapi_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfmapi/definitions.h> are copied here
  * for local use of libfmapi
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFMAPI_VERSION					20240117
+#define LIBFMAPI_VERSION					20240415
 
 /* The libfmapi version string
  */
-#define LIBFMAPI_VERSION_STRING					"20240117"
+#define LIBFMAPI_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFMAPI_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFMAPI_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 enum LIBFMAPI_ENTRY_IDENTIFIER_FLAGS
```

### Comparing `libnk2-20240210/libfmapi/libfmapi_support.c` & `libnk2-20240426/libfmapi/libfmapi_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_unused.h` & `libnk2-20240426/libfmapi/libfmapi_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_class_identifier.c` & `libnk2-20240426/libfmapi/libfmapi_class_identifier.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_checksum.h` & `libnk2-20240426/libfmapi/libfmapi_checksum.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_checksum.c` & `libnk2-20240426/libfmapi/libfmapi_checksum.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_property_type.c` & `libnk2-20240426/libfmapi/libfmapi_property_type.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_libfdatetime.h` & `libnk2-20240426/libfmapi/libfmapi_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_lzfu.c` & `libnk2-20240426/libfmapi/libfmapi_lzfu.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_types.h` & `libnk2-20240426/libfmapi/libfmapi_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_property_type.h` & `libnk2-20240426/libfmapi/libfmapi_property_type.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_lzfu.h` & `libnk2-20240426/libfmapi/libfmapi_lzfu.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_libcerror.h` & `libnk2-20240426/libfmapi/libfmapi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_service_provider_identifier.c` & `libnk2-20240426/libfmapi/libfmapi_service_provider_identifier.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_error.c` & `libnk2-20240426/libfmapi/libfmapi_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/Makefile.in` & `libnk2-20240426/libfmapi/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -540,16 +540,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFMAPI_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFMAPI_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFMAPI_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFMAPI_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFMAPI_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBFGUID_CPPFLAGS@ \
@@ -578,15 +578,16 @@
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_service_provider_identifier.c libfmapi_service_provider_identifier.h \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_support.c libfmapi_support.h \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_types.h \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_unused.h \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_value_type.c libfmapi_value_type.h \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_x400_object_identifier.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -797,24 +798,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfmapi_checksum.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_class_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_codepage.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_debug.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_entry_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_error.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_lzfu.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_one_off_entry_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_property_type.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_service_provider_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_support.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -909,17 +924,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfmapi ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfmapi_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libfmapi/libfmapi_support.h` & `libnk2-20240426/libfmapi/libfmapi_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_extern.h` & `libnk2-20240426/libfmapi/libfmapi_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfmapi/libfmapi_service_provider_identifier.h` & `libnk2-20240426/libfmapi/libfmapi_service_provider_identifier.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2.pc.in` & `libnk2-20240426/libnk2.pc.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/config.sub` & `libnk2-20240426/config.sub`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/setup.py` & `libnk2-20240426/setup.py`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/acinclude.m4` & `libnk2-20240426/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/config.rpath` & `libnk2-20240426/config.rpath`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libnk2.spec` & `libnk2-20240426/libnk2.spec`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libnk2
-Version: 20240210
+Version: 20240426
 Release: 1
 Summary: Library to access the Nickfile (NK2) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libnk2
               
@@ -91,10 +91,10 @@
 %files -n libnk2-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sat Feb 10 2024 Joachim Metz <joachim.metz@gmail.com> 20240210-1
+* Fri Apr 26 2024 Joachim Metz <joachim.metz@gmail.com> 20240426-1
 - Auto-generated
```

### Comparing `libnk2-20240210/libcthreads/libcthreads_thread.h` & `libnk2-20240426/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_read_write_lock.h` & `libnk2-20240426/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_thread.c` & `libnk2-20240426/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_thread_pool.h` & `libnk2-20240426/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_support.h` & `libnk2-20240426/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_lock.h` & `libnk2-20240426/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_unused.h` & `libnk2-20240426/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_lock.c` & `libnk2-20240426/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_condition.h` & `libnk2-20240426/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_repeating_thread.h` & `libnk2-20240426/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/Makefile.am` & `libnk2-20240426/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libnk2-20240210/libcthreads/libcthreads_support.c` & `libnk2-20240426/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_mutex.c` & `libnk2-20240426/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_queue.c` & `libnk2-20240426/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_mutex.h` & `libnk2-20240426/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_types.h` & `libnk2-20240426/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_thread_attributes.h` & `libnk2-20240426/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_condition.c` & `libnk2-20240426/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_error.c` & `libnk2-20240426/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_read_write_lock.c` & `libnk2-20240426/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_libcerror.h` & `libnk2-20240426/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_definitions.h` & `libnk2-20240426/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libnk2-20240210/libcthreads/libcthreads_thread_pool.c` & `libnk2-20240426/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_error.h` & `libnk2-20240426/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_thread_attributes.c` & `libnk2-20240426/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_extern.h` & `libnk2-20240426/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/libcthreads_repeating_thread.c` & `libnk2-20240426/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcthreads/Makefile.in` & `libnk2-20240426/libcthreads/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -536,16 +536,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -560,15 +560,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -778,24 +779,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -889,17 +903,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libcthreads/libcthreads_queue.h` & `libnk2-20240426/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/test-driver` & `libnk2-20240426/test-driver`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_support.c` & `libnk2-20240426/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_libcerror.h` & `libnk2-20240426/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_definitions.h` & `libnk2-20240426/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libnk2-20240210/libcpath/Makefile.am` & `libnk2-20240426/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libnk2-20240210/libcpath/libcpath_error.c` & `libnk2-20240426/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_extern.h` & `libnk2-20240426/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_system_string.h` & `libnk2-20240426/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_support.h` & `libnk2-20240426/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_libcsplit.h` & `libnk2-20240426/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_system_string.c` & `libnk2-20240426/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_libclocale.h` & `libnk2-20240426/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_error.h` & `libnk2-20240426/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/Makefile.in` & `libnk2-20240426/libcpath/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -512,16 +512,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -533,15 +533,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -744,24 +745,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -848,17 +855,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libcpath/libcpath_libuna.h` & `libnk2-20240426/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_unused.h` & `libnk2-20240426/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_path.c` & `libnk2-20240426/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcpath/libcpath_path.h` & `libnk2-20240426/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/ChangeLog` & `libnk2-20240426/ChangeLog`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/manuals/libnk2.3` & `libnk2-20240426/manuals/libnk2.3`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/manuals/nk2info.1` & `libnk2-20240426/manuals/nk2info.1`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/manuals/nk2export.1` & `libnk2-20240426/manuals/nk2export.1`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/manuals/Makefile.in` & `libnk2-20240426/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -494,15 +494,16 @@
 	libnk2.3
 
 EXTRA_DIST = \
 	nk2export.1 \
 	nk2info.1 \
 	libnk2.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -695,23 +696,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -793,13 +796,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libnk2-20240210/tests/nk2_test_record_entry.c` & `libnk2-20240426/tests/nk2_test_record_entry.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_memory.c` & `libnk2-20240426/tests/nk2_test_memory.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_libnk2.h` & `libnk2-20240426/tests/nk2_test_libnk2.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/test_nk2info.sh` & `libnk2-20240426/tests/test_nk2info.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("nk2info");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libnk2-20240210/tests/nk2_test_io_handle.c` & `libnk2-20240426/tests/nk2_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_file_footer.c` & `libnk2-20240426/tests/nk2_test_file_footer.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_unused.h` & `libnk2-20240426/tests/nk2_test_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_libcerror.h` & `libnk2-20240426/tests/nk2_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/test_tools.sh` & `libnk2-20240426/tests/test_tools.sh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle output signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libnk2-20240210/tests/pynk2_test_file.py` & `libnk2-20240426/tests/pynk2_test_file.py`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_functions.h` & `libnk2-20240426/tests/nk2_test_functions.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/Makefile.am` & `libnk2-20240426/tests/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -278,13 +278,12 @@
 	nk2_test_tools_signal.c \
 	nk2_test_unused.h
 
 nk2_test_tools_signal_LDADD = \
 	../libnk2/libnk2.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libnk2-20240210/tests/nk2_test_file_header.c` & `libnk2-20240426/tests/nk2_test_file_header.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_item.c` & `libnk2-20240426/tests/nk2_test_item.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_libbfio.h` & `libnk2-20240426/tests/nk2_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_support.c` & `libnk2-20240426/tests/nk2_test_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_tools_signal.c` & `libnk2-20240426/tests/nk2_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_functions.c` & `libnk2-20240426/tests/nk2_test_functions.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/test_python_module.sh` & `libnk2-20240426/tests/test_python_module.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="file";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libnk2";
+PYTHON_MODULE="pynk2";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pynk2_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pynk2_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pynk2");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libnk2-20240210/tests/nk2_test_tools_output.c` & `libnk2-20240426/tests/nk2_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_error.c` & `libnk2-20240426/tests/nk2_test_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_notify.c` & `libnk2-20240426/tests/nk2_test_notify.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_getopt.c` & `libnk2-20240426/tests/nk2_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_tools_info_handle.c` & `libnk2-20240426/tests/nk2_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/test_nk2export.sh` & `libnk2-20240426/tests/test_nk2export.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Export tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("nk2export");
 OPTIONS_PER_PROFILE=("");
@@ -70,20 +70,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libnk2-20240210/tests/nk2_test_memory.h` & `libnk2-20240426/tests/nk2_test_memory.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_libclocale.h` & `libnk2-20240426/tests/nk2_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/test_runner.sh` & `libnk2-20240426/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_libuna.h` & `libnk2-20240426/tests/nk2_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_getopt.h` & `libnk2-20240426/tests/nk2_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_mapi_value.c` & `libnk2-20240426/tests/nk2_test_mapi_value.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_libcnotify.h` & `libnk2-20240426/tests/nk2_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_file.c` & `libnk2-20240426/tests/nk2_test_file.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/nk2_test_macros.h` & `libnk2-20240426/tests/nk2_test_macros.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/pynk2_test_support.py` & `libnk2-20240426/tests/pynk2_test_support.py`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/tests/Makefile.in` & `libnk2-20240426/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -800,16 +800,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -1064,16 +1064,18 @@
 	nk2_test_tools_signal.c \
 	nk2_test_unused.h
 
 nk2_test_tools_signal_LDADD = \
 	../libnk2/libnk2.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1554,24 +1556,46 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../nk2tools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../nk2tools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../nk2tools/$(DEPDIR)/info_handle.Po
+	-rm -f ../nk2tools/$(DEPDIR)/nk2input.Po
+	-rm -f ../nk2tools/$(DEPDIR)/nk2tools_output.Po
+	-rm -f ../nk2tools/$(DEPDIR)/nk2tools_signal.Po
+	-rm -f ./$(DEPDIR)/nk2_test_error.Po
+	-rm -f ./$(DEPDIR)/nk2_test_file.Po
+	-rm -f ./$(DEPDIR)/nk2_test_file_footer.Po
+	-rm -f ./$(DEPDIR)/nk2_test_file_header.Po
+	-rm -f ./$(DEPDIR)/nk2_test_functions.Po
+	-rm -f ./$(DEPDIR)/nk2_test_getopt.Po
+	-rm -f ./$(DEPDIR)/nk2_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/nk2_test_item.Po
+	-rm -f ./$(DEPDIR)/nk2_test_mapi_value.Po
+	-rm -f ./$(DEPDIR)/nk2_test_memory.Po
+	-rm -f ./$(DEPDIR)/nk2_test_notify.Po
+	-rm -f ./$(DEPDIR)/nk2_test_record_entry.Po
+	-rm -f ./$(DEPDIR)/nk2_test_support.Po
+	-rm -f ./$(DEPDIR)/nk2_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/nk2_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/nk2_test_tools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1674,13 +1698,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libnk2-20240210/tests/test_library.sh` & `libnk2-20240426/tests/test_library.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="error file_footer file_header io_handle item mapi_value notify record_entry";
 LIBRARY_TESTS_WITH_INPUT="file support";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libnk2-20240210/ossfuzz/ossfuzz_libnk2.h` & `libnk2-20240426/ossfuzz/ossfuzz_libnk2.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/ossfuzz/Makefile.am` & `libnk2-20240426/ossfuzz/Makefile.am`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -29,17 +29,15 @@
 	../libnk2/libnk2.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
```

### Comparing `libnk2-20240210/ossfuzz/ossfuzz_libbfio.h` & `libnk2-20240426/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/ossfuzz/file_fuzzer.cc` & `libnk2-20240426/ossfuzz/file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/ossfuzz/Makefile.in` & `libnk2-20240426/ossfuzz/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -525,16 +525,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -554,15 +554,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libnk2/libnk2.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -804,23 +805,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/file_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -904,17 +908,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libnk2-20240210/ltmain.sh` & `libnk2-20240426/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_locale_identifier.h` & `libnk2-20240426/libfwnt/libfwnt_locale_identifier.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_lzxpress.c` & `libnk2-20240426/libfwnt/libfwnt_lzxpress.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_extern.h` & `libnk2-20240426/libfwnt/libfwnt_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_security_identifier.c` & `libnk2-20240426/libfwnt/libfwnt_security_identifier.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_libcerror.h` & `libnk2-20240426/libfwnt/libfwnt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_bit_stream.c` & `libnk2-20240426/libfwnt/libfwnt_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_error.h` & `libnk2-20240426/libfwnt/libfwnt_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_lznt1.h` & `libnk2-20240426/libfwnt/libfwnt_lznt1.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_notify.c` & `libnk2-20240426/libfwnt/libfwnt_notify.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/Makefile.am` & `libnk2-20240426/libfwnt/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFWNT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfwnt.la
@@ -30,19 +30,17 @@
 	libfwnt_security_descriptor.c libfwnt_security_descriptor.h \
 	libfwnt_security_identifier.c libfwnt_security_identifier.h \
 	libfwnt_support.c libfwnt_support.h \
 	libfwnt_types.h \
 	libfwnt_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
```

### Comparing `libnk2-20240210/libfwnt/libfwnt_security_identifier.h` & `libnk2-20240426/libfwnt/libfwnt_security_identifier.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_support.h` & `libnk2-20240426/libfwnt/libfwnt_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_huffman_tree.h` & `libnk2-20240426/libfwnt/libfwnt_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_error.c` & `libnk2-20240426/libfwnt/libfwnt_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_access_control_list.h` & `libnk2-20240426/libfwnt/libfwnt_access_control_list.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_security_descriptor.c` & `libnk2-20240426/libfwnt/libfwnt_security_descriptor.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_access_control_list.c` & `libnk2-20240426/libfwnt/libfwnt_access_control_list.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_definitions.h` & `libnk2-20240426/libfwnt/libfwnt_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwnt/definitions.h> are copied here
  * for local use of libfwnt
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWNT_VERSION					20240126
+#define LIBFWNT_VERSION					20240415
 
 /* The version string
  */
-#define LIBFWNT_VERSION_STRING				"20240126"
+#define LIBFWNT_VERSION_STRING				"20240415"
 
 
 /* The endian definitions
  */
 #define LIBFWNT_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWNT_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
```

### Comparing `libnk2-20240210/libfwnt/libfwnt_huffman_tree.c` & `libnk2-20240426/libfwnt/libfwnt_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_debug.c` & `libnk2-20240426/libfwnt/libfwnt_debug.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_lznt1.c` & `libnk2-20240426/libfwnt/libfwnt_lznt1.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_notify.h` & `libnk2-20240426/libfwnt/libfwnt_notify.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_locale_identifier.c` & `libnk2-20240426/libfwnt/libfwnt_locale_identifier.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_debug.h` & `libnk2-20240426/libfwnt/libfwnt_debug.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_libcdata.h` & `libnk2-20240426/libfwnt/libfwnt_libcdata.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_lzx.h` & `libnk2-20240426/libfwnt/libfwnt_lzx.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_unused.h` & `libnk2-20240426/libfwnt/libfwnt_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_libcnotify.h` & `libnk2-20240426/libfwnt/libfwnt_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_access_control_entry.c` & `libnk2-20240426/libfwnt/libfwnt_access_control_entry.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_lzxpress.h` & `libnk2-20240426/libfwnt/libfwnt_lzxpress.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_security_descriptor.h` & `libnk2-20240426/libfwnt/libfwnt_security_descriptor.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_lzx.c` & `libnk2-20240426/libfwnt/libfwnt_lzx.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/Makefile.in` & `libnk2-20240426/libfwnt/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -538,16 +538,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFWNT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFWNT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFWNT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFWNT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFWNT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFWNT_TRUE@noinst_LTLIBRARIES = libfwnt.la
@@ -570,15 +570,16 @@
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_notify.c libfwnt_notify.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_security_descriptor.c libfwnt_security_descriptor.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_security_identifier.c libfwnt_security_identifier.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_support.c libfwnt_support.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_types.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -791,24 +792,40 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfwnt_access_control_entry.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_access_control_list.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_error.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_locale_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lznt1.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzx.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzxpress.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_notify.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -905,17 +922,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libfwnt/libfwnt_bit_stream.h` & `libnk2-20240426/libfwnt/libfwnt_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_types.h` & `libnk2-20240426/libfwnt/libfwnt_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_support.c` & `libnk2-20240426/libfwnt/libfwnt_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfwnt/libfwnt_access_control_entry.h` & `libnk2-20240426/libfwnt/libfwnt_access_control_entry.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_i18n.h` & `libnk2-20240426/nk2tools/nk2tools_i18n.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libbfio.h` & `libnk2-20240426/nk2tools/nk2tools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/info_handle.h` & `libnk2-20240426/nk2tools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libcpath.h` & `libnk2-20240426/nk2tools/nk2tools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2info.c` & `libnk2-20240426/nk2tools/nk2info.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libnk2.h` & `libnk2-20240426/nk2tools/nk2tools_libnk2.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libfwnt.h` & `libnk2-20240426/nk2tools/nk2tools_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/item_file.h` & `libnk2-20240426/nk2tools/item_file.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/item_file.c` & `libnk2-20240426/nk2tools/item_file.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/Makefile.am` & `libnk2-20240426/nk2tools/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -90,19 +90,17 @@
 	@LIBUNA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libnk2/libnk2.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on nk2export ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(nk2export_SOURCES)
 	@echo "Running splint on nk2info ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(nk2info_SOURCES)
```

### Comparing `libnk2-20240210/nk2tools/nk2tools_libfguid.h` & `libnk2-20240426/nk2tools/nk2tools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libuna.h` & `libnk2-20240426/nk2tools/nk2tools_libuna.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/info_handle.c` & `libnk2-20240426/nk2tools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2export.c` & `libnk2-20240426/nk2tools/nk2export.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/export_handle.c` & `libnk2-20240426/nk2tools/export_handle.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libcerror.h` & `libnk2-20240426/nk2tools/nk2tools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_signal.h` & `libnk2-20240426/nk2tools/nk2tools_signal.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_signal.c` & `libnk2-20240426/nk2tools/nk2tools_signal.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2input.h` & `libnk2-20240426/nk2tools/nk2input.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_output.h` & `libnk2-20240426/nk2tools/nk2tools_output.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_getopt.h` & `libnk2-20240426/nk2tools/nk2tools_getopt.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_output.c` & `libnk2-20240426/nk2tools/nk2tools_output.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/log_handle.c` & `libnk2-20240426/nk2tools/log_handle.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_unused.h` & `libnk2-20240426/nk2tools/nk2tools_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_getopt.c` & `libnk2-20240426/nk2tools/nk2tools_getopt.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2input.c` & `libnk2-20240426/nk2tools/nk2input.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libcfile.h` & `libnk2-20240426/nk2tools/nk2tools_libcfile.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libcnotify.h` & `libnk2-20240426/nk2tools/nk2tools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/export_handle.h` & `libnk2-20240426/nk2tools/export_handle.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libfmapi.h` & `libnk2-20240426/nk2tools/nk2tools_libfmapi.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libclocale.h` & `libnk2-20240426/nk2tools/nk2tools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/Makefile.in` & `libnk2-20240426/nk2tools/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -516,16 +516,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -606,15 +606,16 @@
 	@LIBUNA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libnk2/libnk2.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -869,23 +870,35 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/export_handle.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/item_file.Po
+	-rm -f ./$(DEPDIR)/log_handle.Po
+	-rm -f ./$(DEPDIR)/nk2export.Po
+	-rm -f ./$(DEPDIR)/nk2info.Po
+	-rm -f ./$(DEPDIR)/nk2input.Po
+	-rm -f ./$(DEPDIR)/nk2tools_getopt.Po
+	-rm -f ./$(DEPDIR)/nk2tools_output.Po
+	-rm -f ./$(DEPDIR)/nk2tools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -978,17 +991,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on nk2export ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(nk2export_SOURCES)
 	@echo "Running splint on nk2info ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(nk2info_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/nk2tools/log_handle.h` & `libnk2-20240426/nk2tools/log_handle.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libfdatetime.h` & `libnk2-20240426/nk2tools/nk2tools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/nk2tools/nk2tools_libfvalue.h` & `libnk2-20240426/nk2tools/nk2tools_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_narrow_string.c` & `libnk2-20240426/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_definitions.h` & `libnk2-20240426/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libnk2-20240210/libcsplit/libcsplit_types.h` & `libnk2-20240426/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_wide_split_string.c` & `libnk2-20240426/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_support.h` & `libnk2-20240426/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/Makefile.am` & `libnk2-20240426/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libnk2-20240210/libcsplit/libcsplit_libcerror.h` & `libnk2-20240426/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_wide_string.c` & `libnk2-20240426/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_unused.h` & `libnk2-20240426/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_wide_split_string.h` & `libnk2-20240426/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_error.c` & `libnk2-20240426/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_narrow_split_string.c` & `libnk2-20240426/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_extern.h` & `libnk2-20240426/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_error.h` & `libnk2-20240426/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_support.c` & `libnk2-20240426/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_wide_string.h` & `libnk2-20240426/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/Makefile.in` & `libnk2-20240426/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -522,16 +522,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -540,15 +540,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -753,24 +754,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -859,17 +868,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libcsplit/libcsplit_narrow_split_string.h` & `libnk2-20240426/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcsplit/libcsplit_narrow_string.h` & `libnk2-20240426/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/po/remove-potcdate.sin` & `libnk2-20240426/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/po/Makefile.in.in` & `libnk2-20240426/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/po/en@quot.header` & `libnk2-20240426/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/po/en@boldquot.header` & `libnk2-20240426/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/po/insert-header.sin` & `libnk2-20240426/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/po/Makevars` & `libnk2-20240426/po/Makevars`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/po/Makevars.in` & `libnk2-20240426/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/po/Rules-quot` & `libnk2-20240426/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1251.c` & `libnk2-20240426/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf16_string.c` & `libnk2-20240426/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_base16_stream.c` & `libnk2-20240426/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf8_stream.h` & `libnk2-20240426/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_2.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_932.c` & `libnk2-20240426/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_dingbats.h` & `libnk2-20240426/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf8_string.c` & `libnk2-20240426/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_base64_stream.c` & `libnk2-20240426/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_error.h` & `libnk2-20240426/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_turkish.h` & `libnk2-20240426/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_unicode_character.c` & `libnk2-20240426/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_gaelic.c` & `libnk2-20240426/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_arabic.h` & `libnk2-20240426/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_thai.c` & `libnk2-20240426/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_874.h` & `libnk2-20240426/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_15.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf8_string.h` & `libnk2-20240426/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_16.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1255.c` & `libnk2-20240426/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf7_stream.c` & `libnk2-20240426/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_byte_stream.h` & `libnk2-20240426/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_koi8_u.c` & `libnk2-20240426/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_unused.h` & `libnk2-20240426/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_6.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_14.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_base64_stream.h` & `libnk2-20240426/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_error.c` & `libnk2-20240426/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_centraleurroman.h` & `libnk2-20240426/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_romanian.c` & `libnk2-20240426/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_6.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_9.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_russian.h` & `libnk2-20240426/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_dingbats.c` & `libnk2-20240426/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_15.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_936.c` & `libnk2-20240426/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_croatian.h` & `libnk2-20240426/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_scsu.h` & `libnk2-20240426/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/Makefile.am` & `libnk2-20240426/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libnk2-20240210/libuna/libuna_utf32_stream.c` & `libnk2-20240426/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_936.h` & `libnk2-20240426/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_10.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_roman.c` & `libnk2-20240426/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf7_stream.h` & `libnk2-20240426/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_3.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_thai.h` & `libnk2-20240426/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_farsi.h` & `libnk2-20240426/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_ukrainian.c` & `libnk2-20240426/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_inuit.c` & `libnk2-20240426/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_932.h` & `libnk2-20240426/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_874.c` & `libnk2-20240426/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_5.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_10.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_definitions.h` & `libnk2-20240426/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libnk2-20240210/libuna/libuna_url_stream.h` & `libnk2-20240426/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_icelandic.h` & `libnk2-20240426/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_koi8_u.h` & `libnk2-20240426/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf16_stream.c` & `libnk2-20240426/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1253.c` & `libnk2-20240426/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_4.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_greek.c` & `libnk2-20240426/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_libcerror.h` & `libnk2-20240426/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_centraleurroman.c` & `libnk2-20240426/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1254.c` & `libnk2-20240426/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_13.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_7.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1255.h` & `libnk2-20240426/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_unicode_character.h` & `libnk2-20240426/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_8.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_13.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_949.h` & `libnk2-20240426/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_cyrillic.c` & `libnk2-20240426/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_celtic.c` & `libnk2-20240426/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_support.h` & `libnk2-20240426/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_4.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_949.c` & `libnk2-20240426/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf16_stream.h` & `libnk2-20240426/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_symbol.c` & `libnk2-20240426/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_roman.h` & `libnk2-20240426/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1257.c` & `libnk2-20240426/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1254.h` & `libnk2-20240426/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_950.c` & `libnk2-20240426/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_extern.h` & `libnk2-20240426/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1256.c` & `libnk2-20240426/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_types.h` & `libnk2-20240426/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_base32_stream.h` & `libnk2-20240426/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1253.h` & `libnk2-20240426/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_16.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf8_stream.c` & `libnk2-20240426/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1250.h` & `libnk2-20240426/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_2.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_support.c` & `libnk2-20240426/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_koi8_r.c` & `libnk2-20240426/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_5.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf16_string.h` & `libnk2-20240426/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf32_string.c` & `libnk2-20240426/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_icelandic.c` & `libnk2-20240426/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1256.h` & `libnk2-20240426/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf32_string.h` & `libnk2-20240426/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_romanian.h` & `libnk2-20240426/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_8.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_koi8_r.h` & `libnk2-20240426/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_cyrillic.h` & `libnk2-20240426/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_arabic.c` & `libnk2-20240426/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_croatian.c` & `libnk2-20240426/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_9.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_greek.h` & `libnk2-20240426/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1258.h` & `libnk2-20240426/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_7.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/Makefile.in` & `libnk2-20240426/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -690,16 +690,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -765,15 +765,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1035,24 +1036,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1198,17 +1264,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_3.c` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1250.c` & `libnk2-20240426/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_scsu.c` & `libnk2-20240426/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1252.c` & `libnk2-20240426/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_turkish.c` & `libnk2-20240426/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_ukrainian.h` & `libnk2-20240426/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_russian.c` & `libnk2-20240426/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1258.c` & `libnk2-20240426/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_celtic.h` & `libnk2-20240426/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_byte_stream.c` & `libnk2-20240426/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_gaelic.h` & `libnk2-20240426/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_utf32_stream.h` & `libnk2-20240426/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_symbol.h` & `libnk2-20240426/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1257.h` & `libnk2-20240426/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_inuit.h` & `libnk2-20240426/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_mac_farsi.c` & `libnk2-20240426/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_950.h` & `libnk2-20240426/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_url_stream.c` & `libnk2-20240426/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1251.h` & `libnk2-20240426/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_windows_1252.h` & `libnk2-20240426/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_codepage_iso_8859_14.h` & `libnk2-20240426/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_base16_stream.h` & `libnk2-20240426/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libuna/libuna_base32_stream.c` & `libnk2-20240426/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/Makefile.in` & `libnk2-20240426/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -636,16 +636,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libnk2.pc \
+	libnk2.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libnk2.pc
 
 all: all-recursive
 
@@ -1062,23 +1069,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1189,22 +1199,10 @@
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfmapi && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libnk2 && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libnk2.pc
-	-rm -f libnk2.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libnk2-20240210/libfvalue/libfvalue_filetime.c` & `libnk2-20240426/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_utf16_string.c` & `libnk2-20240426/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_libfwnt.h` & `libnk2-20240426/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_value.c` & `libnk2-20240426/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_value.h` & `libnk2-20240426/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_definitions.h` & `libnk2-20240426/libfvalue/libfvalue_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20240124
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20240124"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libnk2-20240210/libfvalue/libfvalue_codepage.h` & `libnk2-20240426/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_split_utf16_string.c` & `libnk2-20240426/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_error.c` & `libnk2-20240426/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_utf8_string.c` & `libnk2-20240426/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_unused.h` & `libnk2-20240426/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_split_utf16_string.h` & `libnk2-20240426/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_filetime.h` & `libnk2-20240426/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_support.c` & `libnk2-20240426/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_extern.h` & `libnk2-20240426/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/Makefile.am` & `libnk2-20240426/libfvalue/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFVALUE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -41,19 +41,17 @@
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
 	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 	libfvalue_utf16_string.c libfvalue_utf16_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libnk2-20240210/libfvalue/libfvalue_value_type.h` & `libnk2-20240426/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_libcerror.h` & `libnk2-20240426/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_split_utf8_string.c` & `libnk2-20240426/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_data_handle.h` & `libnk2-20240426/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_libcnotify.h` & `libnk2-20240426/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_data_handle.c` & `libnk2-20240426/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_integer.c` & `libnk2-20240426/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_value_type.c` & `libnk2-20240426/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_integer.h` & `libnk2-20240426/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_binary_data.h` & `libnk2-20240426/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_value_entry.h` & `libnk2-20240426/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_utf16_string.h` & `libnk2-20240426/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_error.h` & `libnk2-20240426/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_table.h` & `libnk2-20240426/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_libfguid.h` & `libnk2-20240426/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_split_utf8_string.h` & `libnk2-20240426/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_floating_point.h` & `libnk2-20240426/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_libfdatetime.h` & `libnk2-20240426/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_string.h` & `libnk2-20240426/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_binary_data.c` & `libnk2-20240426/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_value_entry.c` & `libnk2-20240426/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_libcdata.h` & `libnk2-20240426/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_support.h` & `libnk2-20240426/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_table.c` & `libnk2-20240426/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/Makefile.in` & `libnk2-20240426/libfvalue/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -553,16 +553,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFVALUE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFGUID_CPPFLAGS@ \
@@ -596,15 +596,16 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -819,24 +820,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfvalue_binary_data.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_error.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_floating_point.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_integer.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_support.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_table.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_entry.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -935,17 +954,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libfvalue/libfvalue_utf8_string.h` & `libnk2-20240426/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_floating_point.c` & `libnk2-20240426/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_types.h` & `libnk2-20240426/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_string.c` & `libnk2-20240426/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfvalue/libfvalue_libuna.h` & `libnk2-20240426/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/libcnotify_definitions.h` & `libnk2-20240426/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libnk2-20240210/libcnotify/libcnotify_extern.h` & `libnk2-20240426/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/libcnotify_support.c` & `libnk2-20240426/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/libcnotify_stream.h` & `libnk2-20240426/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/Makefile.am` & `libnk2-20240426/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libnk2-20240210/libcnotify/libcnotify_unused.h` & `libnk2-20240426/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/libcnotify_verbose.h` & `libnk2-20240426/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/libcnotify_print.h` & `libnk2-20240426/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/libcnotify_stream.c` & `libnk2-20240426/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/libcnotify_support.h` & `libnk2-20240426/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/libcnotify_verbose.c` & `libnk2-20240426/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/Makefile.in` & `libnk2-20240426/libcnotify/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -514,30 +514,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -740,24 +741,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -844,17 +851,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libcnotify/libcnotify_libcerror.h` & `libnk2-20240426/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcnotify/libcnotify_print.c` & `libnk2-20240426/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcerror/libcerror_system.c` & `libnk2-20240426/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcerror/libcerror_error.c` & `libnk2-20240426/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcerror/libcerror_extern.h` & `libnk2-20240426/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcerror/Makefile.am` & `libnk2-20240426/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libnk2-20240210/libcerror/libcerror_types.h` & `libnk2-20240426/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcerror/libcerror_support.h` & `libnk2-20240426/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcerror/libcerror_error.h` & `libnk2-20240426/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcerror/libcerror_system.h` & `libnk2-20240426/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcerror/libcerror_definitions.h` & `libnk2-20240426/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libnk2-20240210/libcerror/libcerror_support.c` & `libnk2-20240426/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcerror/libcerror_unused.h` & `libnk2-20240426/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libcerror/Makefile.in` & `libnk2-20240426/libcerror/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -511,28 +511,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -734,24 +735,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -837,17 +843,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_floatingtime.h` & `libnk2-20240426/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_nsf_timedate.c` & `libnk2-20240426/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_error.h` & `libnk2-20240426/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_floatingtime.c` & `libnk2-20240426/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_support.h` & `libnk2-20240426/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_hfs_time.h` & `libnk2-20240426/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_definitions.h` & `libnk2-20240426/libfdatetime/libfdatetime_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20240115
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20240115"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_hfs_time.c` & `libnk2-20240426/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/Makefile.am` & `libnk2-20240426/libfdatetime/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,19 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_filetime.c` & `libnk2-20240426/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_systemtime.h` & `libnk2-20240426/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_extern.h` & `libnk2-20240426/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_posix_time.c` & `libnk2-20240426/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_unused.h` & `libnk2-20240426/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_fat_date_time.h` & `libnk2-20240426/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_systemtime.c` & `libnk2-20240426/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_nsf_timedate.h` & `libnk2-20240426/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_libcerror.h` & `libnk2-20240426/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_support.c` & `libnk2-20240426/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_error.c` & `libnk2-20240426/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_posix_time.h` & `libnk2-20240426/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_date_time_values.h` & `libnk2-20240426/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_filetime.h` & `libnk2-20240426/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_date_time_values.c` & `libnk2-20240426/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_types.h` & `libnk2-20240426/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/libfdatetime/Makefile.in` & `libnk2-20240426/libfdatetime/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -533,16 +533,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -555,15 +555,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -772,24 +773,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -882,17 +895,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libnk2-20240210/libfdatetime/libfdatetime_fat_date_time.c` & `libnk2-20240426/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/aclocal.m4` & `libnk2-20240426/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libnk2-20240210/configure.ac` & `libnk2-20240426/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libnk2],
- [20240210],
+ [20240426],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libnk2.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

