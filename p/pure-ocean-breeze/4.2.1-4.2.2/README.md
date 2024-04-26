# Comparing `tmp/pure_ocean_breeze-4.2.1.tar.gz` & `tmp/pure_ocean_breeze-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-4.2.1.tar", last modified: Wed Apr 10 00:57:14 2024, max compression
+gzip compressed data, was "pure_ocean_breeze-4.2.2.tar", last modified: Fri Apr 26 15:06:22 2024, max compression
```

## Comparing `pure_ocean_breeze-4.2.1.tar` & `pure_ocean_breeze-4.2.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.605353 pure_ocean_breeze-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-10 00:57:14.605353 pure_ocean_breeze-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.585353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.589352 pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31927 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    34899 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    66752 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.589352 pure_ocean_breeze-4.2.1/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23637 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.589352 pure_ocean_breeze-4.2.1/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.589352 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.589352 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/data/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14074 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    36390 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/data/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.589352 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/labor/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)    98694 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.589352 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/state/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.593353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/withs/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.593353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)   273197 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.593353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.593353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)   192825 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.593353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    85655 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.593353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)   314704 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.593353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.597353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29395 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    18816 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    43178 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.597353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.597353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.597353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)   138094 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.597353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.597353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.597353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.597353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.597353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29805 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    29153 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    45478 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.601353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.601353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.601353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)   193541 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.601353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.601353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.601353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.601353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.601353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.601353 pure_ocean_breeze-4.2.1/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:57:14.601353 pure_ocean_breeze-4.2.1/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-10 00:57:14.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-10 00:57:14.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:57:14.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-10 00:57:14.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 00:57:14.000000 pure_ocean_breeze-4.2.1/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:57:14.605353 pure_ocean_breeze-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-10 00:57:06.000000 pure_ocean_breeze-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.306055 pure_ocean_breeze-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-26 15:06:22.306055 pure_ocean_breeze-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.282055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.282055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31932 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34899 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66880 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.286055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23637 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.286055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.286055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.286055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14074 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38106 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/data/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.286055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/labor/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98492 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.286055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.286055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/withs/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.290055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   273197 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.290055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.290055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)   192825 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.290055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85655 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.290055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)   314704 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.290055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.294055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29395 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18816 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43178 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.294055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.294055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.294055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138094 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.294055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.298055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.298055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.298055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.298055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29805 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29153 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45478 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.298055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.298055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.298055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193541 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.302055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.302055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.302055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.302055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.302055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.302055 pure_ocean_breeze-4.2.2/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:06:22.302055 pure_ocean_breeze-4.2.2/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-26 15:06:22.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-26 15:06:22.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:06:22.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-26 15:06:22.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 15:06:22.000000 pure_ocean_breeze-4.2.2/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:06:22.306055 pure_ocean_breeze-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-26 15:06:18.000000 pure_ocean_breeze-4.2.2/setup.py
```

### Comparing `pure_ocean_breeze-4.2.1/LICENSE` & `pure_ocean_breeze-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/PKG-INFO` & `pure_ocean_breeze-4.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 4.2.1
+Version: 4.2.2
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.2.1/README.md` & `pure_ocean_breeze-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
 __updated__ = "2023-07-18 14:49:23"
-__version__ = "4.2.1"
+__version__ = "4.2.2"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
@@ -232,15 +232,16 @@
         from pure_ocean_breeze.data.write_data import *
 
         from pure_ocean_breeze.labor.process import *
         from pure_ocean_breeze.labor.comment import *
 
         from pure_ocean_breeze.mail.email import *
 except Exception:
-    print('您可能正在初始化；如果不是在初始化，则路径设置文件已经清除，请检查。')
+    # print('您可能正在初始化；如果不是在初始化，则路径设置文件已经清除，请检查。')
+    ...
```

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -825,15 +825,15 @@
 
     def __addapt_numpy_float64(self, numpy_float64):
         return AsIs(numpy_float64)
 
     def __addapt_numpy_int64(self, numpy_int64):
         return AsIs(numpy_int64)
 
-    @retry(stop=stop_after_attempt(10), wait=wait_fixed(3))
+    @retry(stop=stop_after_attempt(3000), wait=wait_fixed(0.01))
     def write_via_df(
         self,
         df: pd.DataFrame,
         table_name: str,
         symbols: Union[str, bool, List[int], List[str]] = None,
         tuple_col: Union[str, List[str]] = None,
     ) -> None:
```

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,27 +95,27 @@
         kind = "stock"
     else:
         kind = "index"
     return x, kind
 
 
 @do_on_dfs
-def add_suffix(code:str)->str:
+def add_suffix(code: str) -> str:
     """给股票代码加上后缀
 
     Parameters
     ----------
     code : str
         纯数字组成的字符串类型的股票代码，如000001
 
     Returns
     -------
     str
         添加完后缀后的股票代码，如000001.SZ
-    """    
+    """
     if not isinstance(code, str):
         code = str(code)
     if len(code) < 6:
         code = "0" * (6 - len(code)) + code
     if code.startswith("0") or code.startswith("3"):
         code = ".".join([code, "SZ"])
     elif code.startswith("6"):
@@ -286,16 +286,14 @@
     elif code.startswith("8"):
         code = code + ".BJ"
     else:
         code = code + ".UN"
     return code
 
 
-
-
 @do_on_dfs
 def 生成每日分类表(
     df: pd.DataFrame, code: str, entry: str, exit: str, kind: str
 ) -> pd.DataFrame:
     """
     ```
     df是要包含任意多列的表格，为dataframe格式，主要内容为，每一行是
@@ -533,15 +531,15 @@
         res = []
         if history_file is not None:
             if os.path.exists(homeplace.update_data_file + history_file):
                 old = pd.read_parquet(homeplace.update_data_file + history_file)
                 old_date = old.index.max()
                 if old_date == self.fac.date.max():
                     logger.info(f"本地文件已经是最新的了，无需计算")
-                    self.fac=old
+                    self.fac = old
                 else:
                     try:
                         new_date = self.find_begin(
                             self.tradedays, old_date, self.backsee
                         )
                         fac = self.fac[self.fac.date > new_date]
                         iter_item = [i for i in iter_item if i > new_date]
@@ -620,17 +618,21 @@
                         .unstack()
                     )
                     self.fac.columns = [i[1] for i in list(self.fac.columns)]
                     self.fac = self.fac.resample("M").last()
                 self.fac.to_parquet(homeplace.update_data_file + history_file)
                 logger.success(f"本地文件已经写入完成")
         else:
-            logger.warning("您本次计算没有指定任何本地文件路径，这很可能会导致大量的重复计算和不必要的时间浪费，请注意！")
+            logger.warning(
+                "您本次计算没有指定任何本地文件路径，这很可能会导致大量的重复计算和不必要的时间浪费，请注意！"
+            )
             if daily:
-                logger.warning("您指定的是日频计算，非月频计算，因此强烈建议您指定history_file参数！！")
+                logger.warning(
+                    "您指定的是日频计算，非月频计算，因此强烈建议您指定history_file参数！！"
+                )
             if whole_cross:
                 for end_date in tqdm.auto.tqdm(iter_item):
                     start_date = self.find_begin(self.tradedays, end_date, self.backsee)
                     if start_date < end_date:
                         df = self.fac[
                             (self.fac.date >= start_date) & (self.fac.date <= end_date)
                         ]
@@ -926,15 +928,17 @@
                     cors = pd.concat([old, cors])
                 cors = drop_duplicates_index(cors)
                 cors.to_parquet(homeplace.update_data_file + history)
                 new_end = datetime.datetime.strftime(cors.index.max(), "%Y%m%d")
                 logger.info(f"已经更新至{new_end}")
             return cors
     else:
-        logger.warning("您本次计算没有指定任何本地文件路径，这很可能会导致大量的重复计算和不必要的时间浪费，请注意！")
+        logger.warning(
+            "您本次计算没有指定任何本地文件路径，这很可能会导致大量的重复计算和不必要的时间浪费，请注意！"
+        )
         twins = merge_many([df1, df2])
         tqdm.auto.tqdm.pandas()
         corrs = twins.groupby(["code"]).progress_apply(func_rolling)
         cor = []
         for i in range(len(corrs)):
             df = pd.DataFrame(corrs.iloc[i]).dropna().assign(code=corrs.index[i])
             cor.append(df)
@@ -1094,15 +1098,15 @@
         return True
     else:
         print("不存在空值")
         return False
 
 
 @do_on_dfs
-def get_abs(df: pd.DataFrame, quantile: float=None, square: bool = 0) -> pd.DataFrame:
+def get_abs(df: pd.DataFrame, quantile: float = None, square: bool = 0) -> pd.DataFrame:
     """均值距离化：计算因子与截面均值的距离
 
     Parameters
     ----------
     df : pd.DataFrame
         未均值距离化的因子，index为时间，columns为股票代码
     quantile : bool, optional
@@ -1448,15 +1452,17 @@
     """将数据库中所有的feather文件都转化为parquet文件"""
     homeplace = HomePlace()
     feather_to_parquet(homeplace.daily_data_file)
     feather_to_parquet(homeplace.barra_data_file)
     feather_to_parquet(homeplace.final_factor_file)
     feather_to_parquet(homeplace.update_data_file)
     feather_to_parquet(homeplace.factor_data_file)
-    logger.success("数据库中的feather文件全部被转化为了parquet文件，您可以手动删除所有的feather文件了")
+    logger.success(
+        "数据库中的feather文件全部被转化为了parquet文件，您可以手动删除所有的feather文件了"
+    )
 
 
 def zip_many_dfs(dfs: List[pd.DataFrame]) -> pd.DataFrame:
     """将多个dataframe，拼在一起，相同index和columns指向的那个values，变为多个dataframe的值的列表
     通常用于存储整合分钟数据计算的因子值
 
     Parameters
@@ -1882,15 +1888,17 @@
             return x
 
         df = df.groupby(["date"]).apply(lambda x: clip_sing(x, n))
         try:
             df = df.reset_index()
         except Exception:
             ...
-        df = df.drop_duplicates(subset=['date','code']).pivot(index="date", columns="code", values="fac")
+        df = df.drop_duplicates(subset=["date", "code"]).pivot(
+            index="date", columns="code", values="fac"
+        )
         return df
     elif replace:
 
         def clip_sing(x: pd.Series, n: float = 3):
             median = x.quantile(0.5)
             diff_median = ((x - median).abs()).quantile(0.5)
             max_range = median + n * diff_median
```

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/__init__.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,16 @@
 
         most = "、".join(most)
         con2 = f"看来您最喜欢在{most}工作"
         con3 = "，".join(con3)
         con = con1 + "\n" + con2 + "\n" + con3
         print(con)
 except Exception:
-    print('您可能正在初始化；如果不是在初始化，则路径设置文件已经清除，请检查。')
+    # print('您可能正在初始化；如果不是在初始化，则路径设置文件已经清除，请检查。')
+    ...
 
 
 
 from pure_ocean_breeze.jason import state
 from pure_ocean_breeze.jason import data
 from pure_ocean_breeze.jason import labor
```

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/data/database.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/data/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
 
     def __addapt_numpy_float64(self, numpy_float64):
         return AsIs(numpy_float64)
 
     def __addapt_numpy_int64(self, numpy_int64):
         return AsIs(numpy_int64)
 
-    @retry(stop=stop_after_attempt(10), wait=wait_fixed(3))
+    @retry(stop=stop_after_attempt(3000), wait=wait_fixed(0.01))
     def write_via_df(
         self,
         df: pd.DataFrame,
         table_name: str,
         symbols: Union[str, bool, List[int], List[str]] = None,
         tuple_col: Union[str, List[str]] = None,
     ) -> None:
```

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/data/dicts.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/data/read_data.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/data/tools.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/data/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 import tqdm.auto
 import datetime
 import scipy.io as scio
 import numpy as np
 import scipy.stats as ss
 from functools import reduce, partial
 from typing import Callable, Union, Dict, List, Tuple
+import joblib
+import mpire
+import statsmodels.formula.api as smf
 
 from pure_ocean_breeze.jason.state.homeplace import HomePlace
 from pure_ocean_breeze.jason.state.decorators import do_on_dfs
 
 try:
     homeplace = HomePlace()
 except Exception:
@@ -700,15 +703,15 @@
     df = merge_many(dfs)
     cols = [df[f"fac{i}"] for i in range(1, len(dfs) + 1)]
     df = df.assign(fac=pd.Series(zip(*cols)))
     df = df.pivot(index="date", columns="code", values="fac")
     return df
 
 
-def get_values(df: pd.DataFrame) -> List[pd.DataFrame]:
+def get_values(df: pd.DataFrame,n_jobs:int=40) -> List[pd.DataFrame]:
     """从一个values为列表的dataframe中，一次性取出所有值，分别设置为一个dataframe，并依照顺序存储在列表中
 
     Parameters
     ----------
     df : pd.DataFrame
         一个values为list的dataframe
 
@@ -716,15 +719,19 @@
     -------
     List[pd.DataFrame]
         多个dataframe，每一个的values都是float形式
     """
     d = df.dropna(how="all", axis=1)
     d = d.iloc[:, 0].dropna()
     num = len(d.iloc[0])
-    facs = list(map(lambda x: get_value(df, x), range(num)))
+    if n_jobs>1:
+        facs=joblib.Parallel(n_jobs=40)(joblib.delayed(get_value)(df, x) for x in tqdm.auto.tqdm(list(range(num))))
+    else:
+        facs = list(map(lambda x: get_value(df, x), range(num)))
+
     return facs
 
 
 @do_on_dfs
 def lu计算连续期数(ret0: pd.Series, point: float = 0) -> pd.Series:
     """计算一列数，持续大于或持续小于某个临界点的期数
 
@@ -944,108 +951,127 @@
     fac = fac1 + fac2
     have = np.sign(fac1.abs() + 1)
     return fac * have
 
 
 @do_on_dfs
 def jason_to_wind(df: pd.DataFrame):
-    df.index = pd.to_datetime(df.index.astype(str))
-    df.columns = [add_suffix(i) for i in df.columns]
-    return df
+    df1 = df.copy()
+    df1.index = pd.to_datetime(df1.index.astype(str))
+    df1.columns = [add_suffix(i) for i in df1.columns]
+    return df1
+
 
 @do_on_dfs
 def wind_to_jason(df: pd.DataFrame):
-    df.columns = [i[:6] for i in df.columns]
-    df.index = df.index.strftime("%Y%m%d").astype(int)
-    return df
+    df1 = df.copy()
+    df1.columns = [i[:6] for i in df1.columns]
+    df1.index = df1.index.strftime("%Y%m%d").astype(int)
+    return df1
 
 
 @do_on_dfs
 def lu计算连续期数2(
     s: Union[pd.Series, pd.DataFrame],
     judge_number: float = 1,
     nan_value: float = np.nan,
 ) -> Union[pd.Series, pd.DataFrame]:
     """
     <<注意！使用此函数时，目标df的值必须全为1或nan！！！>>
     """
-      
+
     # 将Series中的值转换为布尔值，1为True，其余为False
     is_one = s == judge_number
 
     # 计算累计和以标识连续的1区块
     cumulative_sum = is_one.cumsum()
 
     # 重置每个连续1区块的累计和，为此，我们需要找到每个区块的开始并从cumulative_sum中减去该值
     reset_cumsum = cumulative_sum - cumulative_sum.where(~is_one).ffill().fillna(0)
 
     # 在每个连续的1区块内，使用cumsum计算连续1的个数
     continuous_ones = reset_cumsum * is_one
     return continuous_ones.replace(0, nan_value)
 
 
-def lu计算连续期数2片段递增(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
-    return lu计算连续期数2(s)+lu标记连续片段(s)
+def lu计算连续期数2片段递增(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
+    return lu计算连续期数2(s) + lu标记连续片段(s)
 
-def lu计算连续期数2片段递减(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
-    return lu计算连续期数2(s)-lu标记连续片段(s)
 
+def lu计算连续期数2片段递减(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
+    return lu计算连续期数2(s) - lu标记连续片段(s)
 
-def lu计算连续期数奇正偶反(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
-    if isinstance(s,pd.DataFrame):
+
+def lu计算连续期数奇正偶反(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
+    if isinstance(s, pd.DataFrame):
         return s.apply(lu计算连续期数奇正偶反)
     else:
-        s=s.reset_index(drop=True)
+        s = s.reset_index(drop=True)
         # 用于标记每个连续非NaN片段
         s_diff = (~s.isna()).astype(int).diff().fillna(1).cumsum()
 
         # 对每个连续片段进行编号（1开始）
         segment_nums = s_diff[s_diff.diff().fillna(1) != 0].cumsum()
 
         # 将连续片段编号映射回原始序列
         s_mapped = segment_nums.reindex_like(s).ffill().fillna(0)
 
         # 对每个连续非NaN片段生成顺序序列
         order = s.groupby(s_mapped).cumcount() + 1
 
         # 计算每个连续非NaN片段的长度
-        segment_lengths = s.groupby(s_mapped).transform('count')
+        segment_lengths = s.groupby(s_mapped).transform("count")
 
         # 对偶数编号的片段进行逆序排列
-        s[s.notna()] = np.where(s_mapped % 2 == 1, order, segment_lengths[s_mapped == s_mapped] - order + 1)
+        s[s.notna()] = np.where(
+            s_mapped % 2 == 1, order, segment_lengths[s_mapped == s_mapped] - order + 1
+        )
         return s.values
-    
-def lu计算连续期数偶正奇反(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
-    if isinstance(s,pd.DataFrame):
+
+
+def lu计算连续期数偶正奇反(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
+    if isinstance(s, pd.DataFrame):
         return s.apply(lu计算连续期数偶正奇反)
     else:
-        s=s.reset_index(drop=True)
+        s = s.reset_index(drop=True)
         # 用于标记每个连续非NaN片段
         s_diff = (~s.isna()).astype(int).diff().fillna(1).cumsum()
 
         # 对每个连续片段进行编号（1开始）
         segment_nums = s_diff[s_diff.diff().fillna(1) != 0].cumsum()
 
         # 将连续片段编号映射回原始序列
         s_mapped = segment_nums.reindex_like(s).ffill().fillna(0)
 
         # 对每个连续非NaN片段生成顺序序列
         order = s.groupby(s_mapped).cumcount() + 1
 
         # 计算每个连续非NaN片段的长度
-        segment_lengths = s.groupby(s_mapped).transform('count')
+        segment_lengths = s.groupby(s_mapped).transform("count")
 
         # 对偶数编号的片段进行逆序排列
-        s[s.notna()] = np.where(s_mapped % 2 == 1, segment_lengths[s_mapped == s_mapped] - order + 1, order)
+        s[s.notna()] = np.where(
+            s_mapped % 2 == 1, segment_lengths[s_mapped == s_mapped] - order + 1, order
+        )
         return s.values
 
 
-def lu计算连续期数长度(s:Union[pd.Series,pd.DataFrame],final_mean=1)->Union[float,pd.Series,pd.DataFrame]:
-    if isinstance(s,pd.DataFrame):
-        return s.apply(lambda x:lu计算连续期数长度(x,final_mean))
+def lu计算连续期数长度(
+    s: Union[pd.Series, pd.DataFrame], final_mean=1
+) -> Union[float, pd.Series, pd.DataFrame]:
+    if isinstance(s, pd.DataFrame):
+        return s.apply(lambda x: lu计算连续期数长度(x, final_mean))
     else:
         # 标识非 NaN 值
         not_nan = s.notnull()
 
         # 计算连续非 NaN 值的分组
         groups = not_nan.ne(not_nan.shift()).cumsum()[not_nan]
 
@@ -1056,111 +1082,192 @@
         average_length = segment_lengths.mean()
         if not final_mean:
             return segment_lengths.values
         else:
             return segment_lengths.mean()
 
 
-def lu标记连续片段(s:Union[pd.Series,pd.DataFrame],label_nan=0,number_continuous=1)->Union[pd.Series,pd.DataFrame]:
+def lu标记连续片段(
+    s: Union[pd.Series, pd.DataFrame], label_nan=0, number_continuous=1
+) -> Union[pd.Series, pd.DataFrame]:
     not_nan = ~s.isna()
-    segment_starts = not_nan.diff().fillna(True)  # 对序列首个元素填充True，因为diff会产生NaN
+    segment_starts = not_nan.diff().fillna(
+        True
+    )  # 对序列首个元素填充True，因为diff会产生NaN
 
     # 为每个连续片段分配一个唯一标识符
     segments = segment_starts.cumsum()
 
     # 仅对非NaN片段应用标识符，NaN值保持不变
     if not label_nan:
-        segments=segments*np.sign(s.abs()+1)
+        segments = segments * np.sign(s.abs() + 1)
     if number_continuous:
-        segments=(segments+1)//2
+        segments = (segments + 1) // 2
     return segments
-    
-def lu删去连续片段中的最大值(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
-    if isinstance(s,pd.DataFrame):
+
+
+def lu删去连续片段中的最大值(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
+    if isinstance(s, pd.DataFrame):
         return s.apply(lu删去连续片段中的最大值)
     else:
         # 生成连续片段的标识符
         s_diff = s.isna().astype(int).diff().fillna(0).ne(0).cumsum()
 
         # 对每个片段使用transform找到最大值
-        max_vals = s.groupby(s_diff).transform('max')
+        max_vals = s.groupby(s_diff).transform("max")
 
         # 将原始序列中等于最大值的元素替换为NaN
         s[s == max_vals] = np.nan
         return s
 
-def lu删去连续片段中的最小值(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
+
+def lu删去连续片段中的最小值(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
     return -lu删去连续片段中的最大值(-s)
 
 
-def lu仅保留连续片段中的最大值(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
-    if isinstance(s,pd.DataFrame):
+def lu仅保留连续片段中的最大值(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
+    if isinstance(s, pd.DataFrame):
         return s.apply(lu删去连续片段中的最大值)
     else:
         # 生成连续片段的标识符
         s_diff = s.isna().astype(int).diff().fillna(0).ne(0).cumsum()
 
         # 对每个片段使用transform找到最大值
-        max_vals = s.groupby(s_diff).transform('max')
+        max_vals = s.groupby(s_diff).transform("max")
 
         # 将原始序列中等于最大值的元素替换为NaN
         s[s != max_vals] = np.nan
         return s
 
-def lu仅保留连续片段中的最小值(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
+
+def lu仅保留连续片段中的最小值(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
     return -lu仅保留连续片段中的最大值(-s)
 
-def lu删去连续片段中的最大值及其后面的值(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
-    if isinstance(s,pd.DataFrame):
+
+def lu删去连续片段中的最大值及其后面的值(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
+    if isinstance(s, pd.DataFrame):
         return s.apply(lu删去连续片段中的最大值及其后面的值)
     else:
         # 生成连续片段的标识符
         s_diff = s.isna().astype(int).diff().fillna(0).ne(0).cumsum()
 
         # 对每个片段使用transform找到最大值
-        max_vals = s.groupby(s_diff).transform('max')
+        max_vals = s.groupby(s_diff).transform("max")
 
         # 使用cummax标记最大值及其之后的值
         max_flag = (s.groupby(s_diff).cummax() == max_vals).astype(int)
 
         # 使用cumsum在每个片段内生成标记，从最大值开始累加
         max_flag_cum = max_flag.groupby(s_diff).cumsum()
 
         # 将标记的值替换为NaN
         s[max_flag_cum > 0] = np.nan
         return s
-    
-def lu删去连续片段中的最小值及其后面的值(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
+
+
+def lu删去连续片段中的最小值及其后面的值(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
     return -lu删去连续片段中的最大值及其后面的值(-s)
 
-def lu删去连续片段中的最大值及其前面的值(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
+
+def lu删去连续片段中的最大值及其前面的值(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
     return lu删去连续片段中的最大值及其后面的值(s[::-1])[::-1]
 
-def lu删去连续片段中的最小值及其前面的值(s:Union[pd.Series,pd.DataFrame])->Union[pd.Series,pd.DataFrame]:
+
+def lu删去连续片段中的最小值及其前面的值(
+    s: Union[pd.Series, pd.DataFrame]
+) -> Union[pd.Series, pd.DataFrame]:
     return -lu删去连续片段中的最大值及其前面的值(-s)
 
 
 @do_on_dfs
-def is_pos(s: Union[pd.Series, pd.DataFrame],zero_as_pos:bool=1) -> Union[pd.Series, pd.DataFrame]:
+def is_pos(
+    s: Union[pd.Series, pd.DataFrame], zero_as_pos: bool = 1
+) -> Union[pd.Series, pd.DataFrame]:
     if zero_as_pos:
-        return np.sign(s).replace(0,1).replace(-1,np.nan)
+        return np.sign(s).replace(0, 1).replace(-1, np.nan)
     else:
-        return np.sign(s).replace(0,np.nan).replace(-1,np.nan)
-    
+        return np.sign(s).replace(0, np.nan).replace(-1, np.nan)
+
+
 @do_on_dfs
-def is_neg(s: Union[pd.Series, pd.DataFrame],zero_as_neg:bool=1) -> Union[pd.Series, pd.DataFrame]:
+def is_neg(
+    s: Union[pd.Series, pd.DataFrame], zero_as_neg: bool = 1
+) -> Union[pd.Series, pd.DataFrame]:
     if zero_as_neg:
-        return np.sign(s).replace(0,-1).replace(1,np.nan).replace(-1,1)
+        return np.sign(s).replace(0, -1).replace(1, np.nan).replace(-1, 1)
     else:
-        return np.sign(s).replace(0,np.nan).replace(1,np.nan).replace(-1,1)
-    
+        return np.sign(s).replace(0, np.nan).replace(1, np.nan).replace(-1, 1)
+
+
 @do_on_dfs
-def get_pos_value(s: Union[pd.Series, pd.DataFrame],judge_sign:Union[float,pd.Series, pd.DataFrame],zero_as_pos:bool=1) -> Union[pd.Series, pd.DataFrame]:
-    return s * is_pos(s-judge_sign,zero_as_pos)
+def get_pos_value(
+    s: Union[pd.Series, pd.DataFrame],
+    judge_sign: Union[float, pd.Series, pd.DataFrame],
+    zero_as_pos: bool = 1,
+) -> Union[pd.Series, pd.DataFrame]:
+    return s * is_pos(s - judge_sign, zero_as_pos)
+
 
 @do_on_dfs
-def get_neg_value(s: Union[pd.Series, pd.DataFrame],judge_sign:Union[float,pd.Series, pd.DataFrame],zero_as_neg:bool=1) -> Union[pd.Series, pd.DataFrame]:
-    return s * is_neg(s-judge_sign,zero_as_neg)
+def get_neg_value(
+    s: Union[pd.Series, pd.DataFrame],
+    judge_sign: Union[float, pd.Series, pd.DataFrame],
+    zero_as_neg: bool = 1,
+) -> Union[pd.Series, pd.DataFrame]:
+    return s * is_neg(s - judge_sign, zero_as_neg)
+
 
 @do_on_dfs
-def count_pos_neg(s:Union[pd.Series,pd.DataFrame]):
-    print("正数个数:",is_pos(s).sum().sum(),"负数个数:",is_neg(s).sum().sum())
+def count_pos_neg(s: Union[pd.Series, pd.DataFrame]):
+    print("正数个数:", is_pos(s).sum().sum(), "负数个数:", is_neg(s).sum().sum())
+
+
+
+def de_cross(
+    y: pd.DataFrame, xs: Union[List[pd.DataFrame], pd.DataFrame]
+) -> pd.DataFrame:
+    """使用若干因子对某个因子进行正交化处理
+
+    Parameters
+    ----------
+    y : pd.DataFrame
+        研究的目标，回归中的y
+    xs : Union[List[pd.DataFrame],pd.DataFrame]
+        用于正交化的若干因子，回归中的x
+
+    Returns
+    -------
+    pd.DataFrame
+        正交化之后的因子
+    """
+    if not isinstance(xs, list):
+        xs = [xs]
+    # y = pure_fallmount(y)
+    # xs = [pure_fallmount(i) for i in xs]
+    # return (y - xs)()
+    df=merge_many([y]+xs,how='inner')
+    xs_str='+'.join([f'fac{i+2}' for i in range(len(xs))])
+    def sing(date:pd.Timestamp):
+        df0=df[df.date==date].set_index(['date','code'])
+        if df0.shape[0]>0:
+            ols=smf.ols('fac1~'+xs_str,data=df0).fit()
+            df0.fac1=ols.resid
+            return df0[['fac1']]
+    dates=list(set(df.date))
+    with mpire.WorkerPool(20) as pool:
+        dfs=pool.map(sing,dates)
+    dfs=pd.concat(dfs).reset_index().pivot(index='date',columns='code',values='fac1')
+    return dfs
```

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/labor/comment.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/labor/process.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/labor/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,18 @@
 import plotly.graph_objects as go
 import mpire
 
 from texttable import Texttable
 
 import cufflinks as cf
 
-cf.set_config_file(offline=True)
+try:
+    cf.set_config_file(offline=True)
+except Exception:
+    pass
 from IPython.display import display
 from typing import Callable, Union, Dict, List, Tuple
 from pure_ocean_breeze.jason.data.read_data import (
     read_daily,
     read_market,
     get_industry_dummies,
 )
@@ -494,14 +497,15 @@
         corr = [show_corr(main_i, i, plt_plot=False, method=method) for i in follows]
         corr = [np.nan] * (i + 1) + corr
         corrs.append(corr)
     if factor_names is None:
         factor_names = [f"fac{i}" for i in list(range(1, len(factors) + 1))]
     corrs = pd.DataFrame(corrs, columns=factor_names, index=factor_names)
     np.fill_diagonal(corrs.to_numpy(), 1)
+    corrs=pd.DataFrame(corrs.fillna(0).to_numpy()+corrs.fillna(0).to_numpy().T-np.diag(np.diag(corrs)),index=corrs.index,columns=corrs.columns)
     if show_percent:
         pcorrs = corrs.applymap(to_percent)
     else:
         pcorrs = corrs.copy()
     if print_bool:
         return pcorrs
     else:
@@ -615,38 +619,14 @@
     else:
         pcorrs = corrs.copy()
     if print_bool:
         print(pcorrs)
     return corrs
 
 
-def de_cross(
-    y: pd.DataFrame, xs: Union[List[pd.DataFrame], pd.DataFrame]
-) -> pd.DataFrame:
-    """使用若干因子对某个因子进行正交化处理
-
-    Parameters
-    ----------
-    y : pd.DataFrame
-        研究的目标，回归中的y
-    xs : Union[List[pd.DataFrame],pd.DataFrame]
-        用于正交化的若干因子，回归中的x
-
-    Returns
-    -------
-    pd.DataFrame
-        正交化之后的因子
-    """
-    if not isinstance(xs, list):
-        xs = [xs]
-    y = pure_fallmount(y)
-    xs = [pure_fallmount(i) for i in xs]
-    return (y - xs)()
-
-
 @do_on_dfs
 def show_corrs_with_old(
     df: pd.DataFrame = None,
     method: str = "pearson",
 ) -> pd.DataFrame:
     """计算新因子和已有因子的相关系数
 
@@ -977,15 +957,15 @@
         )
         if not only_cap:
             self.factors = pd.merge(
                 self.factors, self.swindustry_dummy, on=["date", "code"]
             )
 
         dates=list(set(self.factors.date))
-        with mpire.WorkerPool(30) as pool:
+        with mpire.WorkerPool(20) as pool:
             res=pool.map(self.neutralize_factors,dates)
         self.factors = pd.concat(res)
         self.factors = self.factors.reset_index()
         self.factors = self.factors.pivot(index="date", columns="code", values="fac")
 
     def get_ic_rankic(cls, df):
         """计算IC和RankIC"""
@@ -1325,17 +1305,21 @@
                 )
             ]
         )
         # print(self.total_comments)
         self.group_mean_rets_monthly = self.group_rets.drop(
             columns=["long_short"]
         ).mean()
+        # self.group_mean_rets_monthly = (
+        #     self.group_mean_rets_monthly - self.group_mean_rets_monthly.mean()
+        # )
+        mar=self.market_ret.loc[self.factors_out.index]
         self.group_mean_rets_monthly = (
-            self.group_mean_rets_monthly - self.group_mean_rets_monthly.mean()
-        )
+            self.group_mean_rets_monthly - mar.mean()
+        )*self.freq_ctrl.counts_one_year
 
     def plot_net_values(self, y2, filename, iplot=1, ilegend=1, without_breakpoint=0):
         """使用matplotlib来画图，y2为是否对多空组合采用双y轴"""
         if not iplot:
             fig, ax = plt.subplots(nrows=1, ncols=3, figsize=(33, 8))
             self.group_net_values.plot(secondary_y=y2, rot=60, ax=ax[0])
             self.group_net_values.plot(secondary_y=y2, ax=ax[0])
@@ -2346,15 +2330,15 @@
         return df[['fac']]
 
     def get_snow_fac(self):
         """获得纯净因子"""
         dates=list(set(self.corr_pri.date))
         # dates=[self.corr_pri[self.corr_pri.date==i].set_index(['date','code']) for i in dates]
         # print(dates[0])
-        with mpire.WorkerPool(30) as pool:
+        with mpire.WorkerPool(20) as pool:
             res=pool.map(self.ols_in_group,dates)
         self.snow_fac = pd.concat(res)
         # self.snow_fac = (
         #     self.corr_pri.set_index(["date", "code"])
         #     .groupby(["date"],as_index=False)
         #     .apply(self.ols_in_group)
         # )
```

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/state/decorators.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/state/homeplace.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/state/states.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/jason/withs/requires.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/jason/withs/requires.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import time
 import datetime
 import os
 
 import numpy as np
 import pandas as pd
+import scipy
+import mpire
+import joblib
 import requests
 import scipy.io as scio
 import tqdm.auto
 from loguru import logger
 
 import matplotlib.pyplot as plt
```

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 4.2.1
+Version: 4.2.2
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.2.1/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-4.2.2/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.2.1/setup.py` & `pure_ocean_breeze-4.2.2/setup.py`

 * *Files identical despite different names*

