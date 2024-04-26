# Comparing `tmp/vos-3.6.1.tar.gz` & `tmp/vos-3.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vos-3.6.1.tar", last modified: Fri Apr 26 16:33:04 2024, max compression
+gzip compressed data, was "vos-3.6rc0.tar", last modified: Thu Apr 11 07:00:08 2024, max compression
```

## Comparing `vos-3.6.1.tar` & `vos-3.6rc0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.214303 vos-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-26 16:33:00.000000 vos-3.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-26 16:33:00.000000 vos-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-26 16:33:04.214303 vos-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-26 16:33:00.000000 vos-3.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.198303 vos-3.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-26 16:33:00.000000 vos-3.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.198303 vos-3.6.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.202303 vos-3.6.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-26 16:33:00.000000 vos-3.6.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-26 16:33:00.000000 vos-3.6.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-26 16:33:00.000000 vos-3.6.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-26 16:33:00.000000 vos-3.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 16:33:00.000000 vos-3.6.1/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:00.000000 vos-3.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-26 16:33:00.000000 vos-3.6.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-26 16:33:04.214303 vos-3.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4512 2024-04-26 16:33:00.000000 vos-3.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.202303 vos-3.6.1/vos/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-26 16:33:00.000000 vos-3.6.1/vos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.206303 vos-3.6.1/vos/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/interrupt_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.206303 vos-3.6.1/vos/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.210303 vos-3.6.1/vos/commands/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vcat.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vchmod.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vcp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vln.txt
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vlock.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vls.txt
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vmkdir.txt
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vmv.txt
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vrm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vrmdir.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vsync.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/help_vtag.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vcat.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vchmod.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vcp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vln.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vlock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vls.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vmkdir.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vmv.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vrm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vrmdir.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vsync.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/data/vtag.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/test_vls.py
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/tests/test_vsync.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6595 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9041 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vchmod.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21405 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vcp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5671 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vln.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5470 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vlock.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10673 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vls.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5503 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vmkdir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5536 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vmv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6292 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vrm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5358 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vrmdir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19840 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vsync.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7872 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commands/vtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-04-26 16:33:00.000000 vos-3.6.1/vos/commonparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.210303 vos-3.6.1/vos/data/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-26 16:33:00.000000 vos-3.6.1/vos/data/default-vos-config
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-26 16:33:00.000000 vos-3.6.1/vos/logExceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-26 16:33:00.000000 vos-3.6.1/vos/md5_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-26 16:33:00.000000 vos-3.6.1/vos/node_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.210303 vos-3.6.1/vos/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 16:33:00.000000 vos-3.6.1/vos/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.210303 vos-3.6.1/vos/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 16:33:00.000000 vos-3.6.1/vos/tests/data/default-vos-config
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-26 16:33:00.000000 vos-3.6.1/vos/tests/test_commonparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-04-26 16:33:00.000000 vos-3.6.1/vos/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-26 16:33:00.000000 vos-3.6.1/vos/tests/test_md5_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-04-26 16:33:00.000000 vos-3.6.1/vos/tests/test_node_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    14121 2024-04-26 16:33:00.000000 vos-3.6.1/vos/tests/test_vofile.py
--rw-r--r--   0 runner    (1001) docker     (127)    38193 2024-04-26 16:33:00.000000 vos-3.6.1/vos/tests/test_vos.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 16:33:03.000000 vos-3.6.1/vos/version.py
--rw-r--r--   0 runner    (1001) docker     (127)   117051 2024-04-26 16:33:00.000000 vos-3.6.1/vos/vos.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-26 16:33:00.000000 vos-3.6.1/vos/vosconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:33:04.214303 vos-3.6.1/vos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-26 16:33:04.000000 vos-3.6.1/vos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-26 16:33:04.000000 vos-3.6.1/vos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:33:04.000000 vos-3.6.1/vos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-26 16:33:04.000000 vos-3.6.1/vos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:33:04.000000 vos-3.6.1/vos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 16:33:04.000000 vos-3.6.1/vos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-26 16:33:04.000000 vos-3.6.1/vos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-11 07:00:04.000000 vos-3.6rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-11 07:00:04.000000 vos-3.6rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-11 07:00:08.222293 vos-3.6rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-11 07:00:04.000000 vos-3.6rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.210293 vos-3.6rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.206293 vos-3.6rc0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.210293 vos-3.6rc0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-11 07:00:04.000000 vos-3.6rc0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-11 07:00:08.222293 vos-3.6rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4512 2024-04-11 07:00:04.000000 vos-3.6rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.210293 vos-3.6rc0/vos/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.214293 vos-3.6rc0/vos/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/interrupt_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.218294 vos-3.6rc0/vos/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/vos/commands/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vcat.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vchmod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vcp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vln.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vlock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vls.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vmkdir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vmv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vrm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vrmdir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vsync.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/help_vtag.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vcat.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vchmod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vcp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vln.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vlock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vls.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vmkdir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vmv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vrm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vrmdir.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vsync.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/data/vtag.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/test_vls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/tests/test_vsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6595 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9041 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vchmod.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21456 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vcp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5671 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vln.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5470 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vlock.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10673 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vls.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5503 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vmkdir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5536 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vmv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6292 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vrm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5358 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vrmdir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19963 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7872 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commands/vtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/commonparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/vos/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/data/default-vos-config
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/logExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/md5_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/node_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/vos/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/vos/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/data/default-vos-config
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_commonparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_md5_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_node_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14121 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_vofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44009 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/tests/test_vos.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 07:00:07.000000 vos-3.6rc0/vos/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127771 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/vos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-11 07:00:04.000000 vos-3.6rc0/vos/vosconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:00:08.222293 vos-3.6rc0/vos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-11 07:00:08.000000 vos-3.6rc0/vos.egg-info/top_level.txt
```

### Comparing `vos-3.6.1/LICENSE` & `vos-3.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/PKG-INFO` & `vos-3.6rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vos
-Version: 3.6.1
+Version: 3.6rc0
 Summary: CADC VOS Class Libraries
 Home-page: https://www.canfar.net/en/docs/storage
 Author: JJ Kavelaars, Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
 Project-URL: Source, https://github.com/opencadc/vostools
 Project-URL: Issues, https://github.com/opencadc/vostools/issues
@@ -12,15 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7, <4
 License-File: LICENSE
 Requires-Dist: html2text>=2016.5.29
-Requires-Dist: cadcutils>=1.5.2.2
+Requires-Dist: cadcutils>=1.5.1
 Requires-Dist: aenum
 Provides-Extra: test
 Requires-Dist: pytest>=4.6; extra == "test"
 Requires-Dist: pytest-cov>=2.5.1; extra == "test"
 Requires-Dist: flake8>=3.4.1; extra == "test"
 
 DOCUMENTATION
```

### Comparing `vos-3.6.1/README.rst` & `vos-3.6rc0/README.rst`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/docs/Makefile` & `vos-3.6rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/docs/conf.py` & `vos-3.6rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/docs/make.bat` & `vos-3.6rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/setup.cfg` & `vos-3.6rc0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 author_email = cadc@nrc-cnrc.gc.ca
 license = AGPLv3
 url = https://www.canfar.net/en/docs/storage
 edit_on_github = False
 github_project = opencadc/vostools
 install_requires = 
 	html2text>=2016.5.29
-	cadcutils>=1.5.2.2
+	cadcutils>=1.5.1
 	aenum
-version = 3.6.1
+version = 3.6rc
 
 [options.extras_require]
 test = 
 	pytest>=4.6
 	pytest-cov>=2.5.1
 	flake8>=3.4.1
```

### Comparing `vos-3.6.1/setup.py` & `vos-3.6rc0/setup.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/__init__.py` & `vos-3.6rc0/vos/__init__.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/__init__.py` & `vos-3.6rc0/vos/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/interrupt_exception.py` & `vos-3.6rc0/vos/commands/interrupt_exception.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vcat.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vcat.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vchmod.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vchmod.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vcp.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vcp.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vln.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vln.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vlock.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vlock.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vls.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vls.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vmkdir.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vmkdir.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vmv.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vmv.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vrm.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vrm.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vrmdir.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vrmdir.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vsync.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vsync.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/data/help_vtag.txt` & `vos-3.6rc0/vos/commands/tests/data/help_vtag.txt`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/test_cli.py` & `vos-3.6rc0/vos/commands/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/test_vls.py` & `vos-3.6rc0/vos/commands/tests/test_vls.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/tests/test_vsync.py` & `vos-3.6rc0/vos/commands/tests/test_vsync.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/vcat.py` & `vos-3.6rc0/vos/commands/vcat.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/vchmod.py` & `vos-3.6rc0/vos/commands/vchmod.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/vcp.py` & `vos-3.6rc0/vos/commands/vcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,15 +340,16 @@
 
                 if not skip:
                     logging.info("%s -> %s " % (source_name, destination_name))
                 niters = 0
                 while not skip:
                     try:
                         logging.debug("Starting call to copy")
-                        client.copy(source_name, destination_name, head=head)
+                        client.copy(source_name, destination_name,
+                                    send_md5=True, head=head)
                         logging.debug("Call to copy returned")
                         break
                     except Exception as client_exception:
                         logging.debug("{}".format(client_exception))
                         if getattr(client_exception, 'errno', -1) == 104:
                             # 104 is connection reset by peer.
                             # Try again on this error
```

### Comparing `vos-3.6.1/vos/commands/vln.py` & `vos-3.6rc0/vos/commands/vln.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/vlock.py` & `vos-3.6rc0/vos/commands/vlock.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/vls.py` & `vos-3.6rc0/vos/commands/vls.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/vmkdir.py` & `vos-3.6rc0/vos/commands/vmkdir.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/vmv.py` & `vos-3.6rc0/vos/commands/vmv.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/vrm.py` & `vos-3.6rc0/vos/commands/vrm.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/vrmdir.py` & `vos-3.6rc0/vos/commands/vrmdir.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commands/vsync.py` & `vos-3.6rc0/vos/commands/vsync.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,22 +217,25 @@
                 result.bytes_skipped = dest_length
                 return result
         except (transfer_exceptions.AlreadyExistsException,
                 transfer_exceptions.NotFoundException):
             pass
     logging.info('{} -> {}'.format(src, dest))
     try:
-        client.copy(src, dest)
+        client.copy(src, dest, send_md5=True)
         node = client.get_node(dest, limit=None)
         dest_md5 = node.props.get(
             'MD5', 'd41d8cd98f00b204e9800998ecf8427e')
         dest_length = node.attr['st_size']
         dest_time = node.attr['st_ctime']
         if opt.cache_nodes:
-            global_md5_cache.update(dest, dest_md5, dest_length, dest_time)
+            global_md5_cache.update(dest,
+                                    dest_md5,
+                                    dest_length,
+                                    dest_time)
         result.files_sent += 1
         result.bytes_sent += stat.st_size
         return result
     except (IOError, OSError) as exc:
         logging.error(
             'Error writing {} to server, skipping'.format(src))
         logging.debug(str(exc))
```

### Comparing `vos-3.6.1/vos/commands/vtag.py` & `vos-3.6rc0/vos/commands/vtag.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/commonparser.py` & `vos-3.6rc0/vos/commonparser.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/logExceptions.py` & `vos-3.6rc0/vos/logExceptions.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/md5_cache.py` & `vos-3.6rc0/vos/md5_cache.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/node_cache.py` & `vos-3.6rc0/vos/node_cache.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/tests/test_commonparser.py` & `vos-3.6rc0/vos/tests/test_commonparser.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/tests/test_config.py` & `vos-3.6rc0/vos/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/tests/test_md5_cache.py` & `vos-3.6rc0/vos/tests/test_md5_cache.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/tests/test_node_cache.py` & `vos-3.6rc0/vos/tests/test_node_cache.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/tests/test_vofile.py` & `vos-3.6rc0/vos/tests/test_vofile.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos/tests/test_vos.py` & `vos-3.6rc0/vos/tests/test_vos.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,24 +66,27 @@
 # ***********************************************************************
 #
 
 # Test the vos Client class
 
 import os
 import unittest
+import urllib.parse
+
 import pytest
 import requests
 from xml.etree import ElementTree
 from unittest.mock import Mock, patch, MagicMock, call
 from vos import Client, Connection, Node, VOFile, vosconfig
 from vos import vos as vos
 from urllib.parse import urlparse, unquote
 from io import BytesIO
 import hashlib
 import tempfile
+from cadcutils.net import add_md5_header
 
 
 # The following is a temporary workaround for Python issue 25532
 # (https://bugs.python.org/issue25532)
 call.__wrapped__ = None
 
 NODE_XML = """
@@ -148,23 +151,25 @@
     client.get_session = Mock(return_value=mock_session)
     client._fs_type = False
     assert transfer_url == \
         client.get_node_url('vos://cadc.nrc.ca!vospace/auser',
                             view='header')
 
     # test fits header
-    assert {'META': 'true'} == client._get_soda_params(view='header')
+    assert transfer_url + "?META=true" == client._add_soda_ops(transfer_url, view='header')
 
     # test pixel cutouts
     pcutout = '[1][100:125,100:175]'
-    assert {'SUB': pcutout} == client._get_soda_params(cutout=pcutout)
+    assert transfer_url + "?SUB=" + pcutout == client._add_soda_ops(transfer_url,
+                                                                    cutout=pcutout)
 
     # test sky coordinates
     scutout = '1.1,2.2,3.3'
-    assert {'CIRCLE':  scutout} == client._get_soda_params(cutout='CIRCLE='+scutout)
+    assert (transfer_url + "?CIRCLE=" + urllib.parse.quote(scutout) ==
+            client._add_soda_ops(transfer_url, cutout='CIRCLE='+scutout))
 
 
 class TestClient(unittest.TestCase):
     """Test the vos Client class.
     """
     @classmethod
     def setUpClass(cls):
@@ -394,30 +399,30 @@
         computed_md5_mock.return_value = md5sum
 
         # mock the props of the corresponding node
         props = MagicMock()
         props.get.return_value = md5sum
         # add props to the mocked node
         node = MagicMock(spec=Node)
-        node.props = {'MD5': md5sum, 'length': len(file_content)}
+        node.props = {'MD5': md5sum, 'length': 12}
 
         # mock one by one the chain of connection.session.response.headers
         session = MagicMock()
         response = MagicMock()
         headers = MagicMock()
         headers.get.return_value = md5sum
         response.headers = headers
         session.get.return_value = response
         response.iter_content.return_value = BytesIO(file_content)
 
         test_client = Client()
         test_client.get_session = Mock(return_value=session)
         # use the mocked connection instead of the real one
-        node_location_url = 'http://cadc.ca/test'
-        get_node_url_mock = Mock(return_value=node_location_url)
+        get_node_url_mock = Mock(
+            return_value=['http://cadc.ca/test', 'http://cadc.ca/test'])
         test_client.get_node_url = get_node_url_mock
         mock_update = Mock()
         test_client.update = mock_update
 
         # patch Client.get_node to return our mocked node
         get_node_mock = Mock(return_value=node)
         test_client.get_node = get_node_mock
@@ -425,75 +430,74 @@
         # time to test...
         vospaceLocation = 'vos://authority~test/foo'
         osLocation = '/tmp/foo'
         if os.path.isfile(osLocation):
             os.remove(osLocation)
         # copy from vospace
         test_client.is_remote_file = is_remote_file
-        test_client._get_si_client = Mock()
-        test_client._get_si_client.return_value.download_file = (
-            Mock(return_value=('foo', md5sum, len(file_content))))
-        cp_size = test_client.copy(vospaceLocation, osLocation)
+        test_client.get_endpoints = Mock()
+        test_client.copy(vospaceLocation, osLocation)
         get_node_url_mock.assert_called_once_with(vospaceLocation,
                                                   method='GET',
                                                   cutout=None, view='data')
-        si_calls = [call('vos://authority~test/foo'),
-                    call().download_file(url=node_location_url, dest=osLocation, params={})]
-        assert si_calls == test_client._get_si_client.mock_calls
         assert not computed_md5_mock.called, 'MD5 should be computed on the fly'
-        assert cp_size == len(file_content)
+
+        # repeat - local file and vospace file are now the same -> only
+        # get_node is called to get the md5 of remote file
+        computed_md5_mock.reset_mock()
+        session.get.reset_mock()
+        files_response = Mock(headers={'Content-Length': '12'})
+        add_md5_header(files_response.headers, md5sum)
+        session.head.return_value = files_response
+        test_client.copy(vospaceLocation, osLocation)
+        assert not session.get.called
+        computed_md5_mock.assert_called_once_with(osLocation)
 
         # change the content of local files to trigger a new copy
         get_node_url_mock.reset_mock()
         get_node_mock.reset_mock()
 
         computed_md5_mock.reset_mock()
-        test_client._get_si_client.reset_mock()
         computed_md5_mock.return_value = 'd002233'
         response.iter_content.return_value = BytesIO(file_content)
         test_client.copy(vospaceLocation, osLocation)
         get_node_url_mock.assert_called_once_with(vospaceLocation,
                                                   method='GET',
                                                   cutout=None, view='data')
-        si_calls = [call('vos://authority~test/foo'),
-                    call().download_file(url=node_location_url,
-                                         dest=osLocation, params={})]
-        assert si_calls == test_client._get_si_client.mock_calls
+        computed_md5_mock.assert_called_with(osLocation)
 
         # change the content of local files to trigger a new copy
         get_node_url_mock.reset_mock()
-        get_node_url_mock.return_value = 'https://mysite.com/files/node123/cutout'
+        get_node_url_mock.return_value = \
+            ['https://mysite.com/files/node123/cutout']
         computed_md5_mock.reset_mock()
-        test_client._get_si_client.reset_mock()
         computed_md5_mock.return_value = 'd002233'
         # computed_md5_mock.side_effect = ['d002233', md5sum]
         get_node_mock.reset_mock()
         response.iter_content.return_value = BytesIO(file_content)
         session.get.return_value = response
         test_client.get_session = Mock(return_value=session)
         # client must be a vault client
         test_client._fs_type = False
+        test_client._add_soda_ops = Mock()
         test_client.copy('{}{}'.format(vospaceLocation,
                                        '[1][10:60]'), osLocation)
 
-        si_calls = [call('vos://authority~test/foo'),
-                    call().download_file(url='https://mysite.com/files/node123/cutout',
-                                         dest=osLocation, params={'SUB': '[1][10:60]'})]
-        assert si_calls == test_client._get_si_client.mock_calls
+        test_client._add_soda_ops.assert_called_once_with(
+            'https://mysite.com/files/node123/cutout', view='cutout', cutout='[1][10:60]')
 
         # test cavern does not support SODA operations
         test_client._fs_type = True
         with pytest.raises(ValueError):
             test_client.copy('{}{}'.format(vospaceLocation, '[1][10:60]'), osLocation)
             with pytest.raises(ValueError):
                 test_client.copy(vospaceLocation, osLocation, head=True)
 
         test_client._fs_type = False
         # copy to vospace when md5 sums are the same -> only update occurs
-        open(osLocation, 'wb').write(file_content)
         get_node_url_mock.reset_mock()
         computed_md5_mock.reset_mock()
         computed_md5_mock.side_effect = None
         computed_md5_mock.return_value = md5sum
         test_client.copy(osLocation, vospaceLocation)
         mock_update.assert_called_once()
         assert not get_node_url_mock.called
@@ -502,84 +506,199 @@
         get_node_url_mock.reset_mock()
         get_node_url_mock.return_value =\
             ['http://cadc.ca/test', 'http://cadc.ca/test']
         computed_md5_mock.reset_mock()
         mock_update.reset_mock()
         computed_md5_mock.return_value = md5sum
         to_update_node = MagicMock()
-        to_update_node.props = {'MD5': 'abcde', 'length': len(file_content)}
+        to_update_node.props = {'MD5': 'abcde', 'length': 12}
         test_client.get_node = Mock(side_effect=[to_update_node, node])
-        test_client._get_si_client.return_value.upload_file = (
-            Mock(return_value=('foo', md5sum, len(file_content))))
-        cp_size = test_client.copy(osLocation, vospaceLocation)
+        test_client.copy(osLocation, vospaceLocation)
         assert not mock_update.called
-        get_node_url_mock.assert_called_once_with(vospaceLocation, method='PUT',
-                                                  full_negotiation=True)
+        get_node_url_mock.assert_called_once_with(vospaceLocation, 'PUT',
+                                                  content_length=12,
+                                                  md5_checksum='abcde')
         computed_md5_mock.assert_called_once_with(osLocation)
-        assert cp_size == len(file_content)
 
         # copy 0 size file -> delete and create node but no bytes
         # transferred
         get_node_url_mock.reset_mock()
         computed_md5_mock.reset_mock()
         test_client.get_node = Mock(return_value=node)
         node.props['length'] = 0
         mock_delete = Mock()
         mock_create = Mock()
         test_client.delete = mock_delete
         test_client.create = mock_create
         with patch('vos.vos.os.stat', Mock()) as stat_mock:
             stat_mock.return_value = Mock(st_size=0)
-            cp_size = test_client.copy(osLocation, vospaceLocation)
+            test_client.copy(osLocation, vospaceLocation)
         mock_create.assert_called_once_with(vospaceLocation)
         mock_delete.assert_called_once_with(vospaceLocation)
         assert not get_node_url_mock.called
-        assert 0 == cp_size
 
         # copy new 0 size file -> create node but no bytes transferred
         get_node_url_mock.reset_mock()
         computed_md5_mock.reset_mock()
         mock_delete.reset_mock()
         mock_create.reset_mock()
         test_client.get_node = Mock(side_effect=[Exception(), node])
         mock_delete = Mock()
         mock_create = Mock()
         test_client.delete = mock_delete
         test_client.create = mock_create
         with patch('vos.vos.os.stat', Mock()) as stat_mock:
             stat_mock.return_value = Mock(st_size=0)
-            cp_size = test_client.copy(osLocation, vospaceLocation)
+            test_client.copy(osLocation, vospaceLocation)
         mock_create.assert_called_once_with(vospaceLocation)
         assert not mock_delete.called
         assert not get_node_url_mock.called
-        assert cp_size == 0
 
-        # requests just the headers when md5 not provided in the header
-        props.get.side_effect = [None]
-        get_node_url_mock = Mock(
-            return_value=['http://cadc.ca/test', 'http://cadc.ca/test'])
-        test_client.get_node_url = get_node_url_mock
-        get_node_mock.reset_mock()
-        headers.get.return_value = None
-        test_client.copy(vospaceLocation, osLocation, head=True)
-        get_node_url_mock.assert_called_once_with(vospaceLocation,
-                                                  method='GET',
-                                                  cutout=None, view='header')
+        # error tests - md5sum mismatch
+        computed_md5_mock.return_value = '000bad000'
+        test_client.get_node = Mock(return_value=node)
+        with self.assertRaises(OSError):
+            test_client.copy(vospaceLocation, osLocation)
 
-        # repeat headers request when md5 provided in the header
-        props.get.side_effect = md5sum
-        get_node_url_mock = Mock(
-            return_value=['http://cadc.ca/test', 'http://cadc.ca/test'])
-        test_client.get_node_url = get_node_url_mock
-        get_node_mock.reset_mock()
-        response.iter_content.return_value = BytesIO(file_content)
-        test_client.copy(vospaceLocation, osLocation, head=True)
-        get_node_url_mock.assert_called_once_with(vospaceLocation,
-                                                  method='GET',
-                                                  cutout=None, view='header')
+        # # existing file
+        # mock_delete.reset_mock()
+        # get_node_mock.reset_mock()
+        #
+        # with self.assertRaises(OSError):
+        #     with patch('vos.vos.os.stat', Mock()) as stat_mock:
+        #         stat_mock.return_value = Mock(st_size=12)
+        #         test_client.copy(osLocation, vospaceLocation)
+        # assert not mock_delete.called  # server takes care of cleanup
+
+        # new file
+        # mock_delete.reset_mock()
+        # with self.assertRaises(OSError):
+        #     with patch('vos.vos.os.stat', Mock()) as stat_mock:
+        #         stat_mock.return_value = Mock(st_size=12)
+        #         node.props['MD5'] = None
+        #         test_client.copy(osLocation, vospaceLocation)
+        # assert mock_delete.called  # cleanup required
+
+        # requests just the headers when md5 not provided in the header
+        # props.get.side_effect = [None]
+        # get_node_url_mock = Mock(
+        #     return_value=['http://cadc.ca/test', 'http://cadc.ca/test'])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # headers.get.return_value = None
+        # test_client.copy(vospaceLocation, osLocation, head=True)
+        # get_node_url_mock.assert_called_once_with(vospaceLocation,
+        #                                           method='GET',
+        #                                           cutout=None, view='header', full_negotiation=True)
+        #
+        # # repeat headers request when md5 provided in the header
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     return_value=['http://cadc.ca/test', 'http://cadc.ca/test'])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # test_client.copy(vospaceLocation, osLocation, head=True)
+        # get_node_url_mock.assert_called_once_with(vospaceLocation,
+        #                                           method='GET',
+        #                                           cutout=None, view='header', full_negotiation=True)
+        #
+        # # test GET intermittent exceptions on both URLs
+        # props.get.side_effect = md5sum
+        # # first side effect corresponds to the files end point call, the second to full negotiation
+        # get_node_url_mock = Mock(side_effect=['http://cadc1.ca/test', ['http://cadc2.ca/test']])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.get.reset_mock()
+        # session.get.side_effect = \
+        #     [exceptions.TransferException()] * 2 * vos.MAX_INTERMTTENT_RETRIES
+        # with pytest.raises(OSError):
+        #     test_client.copy(vospaceLocation, osLocation, head=False)
+        # assert session.get.call_count == 2 * vos.MAX_INTERMTTENT_RETRIES
+        #
+        # # test GET Transfer error on one URL and a "permanent" one on the other
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     side_effect=[None, ['http://cadc1.ca/test', 'http://cadc2.ca/test']])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.get.reset_mock()
+        # session.get.side_effect = [exceptions.TransferException(),
+        #                            exceptions.HttpException(),
+        #                            exceptions.TransferException(),
+        #                            exceptions.TransferException()]
+        # with pytest.raises(OSError):
+        #     test_client.copy(vospaceLocation, osLocation, head=True)
+        # assert session.get.call_count == vos.MAX_INTERMTTENT_RETRIES + 1
+        #
+        # # test GET both "permanent" errors
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     side_effect=['http://cadc1.ca/test', ['http://cadc2.ca/test']])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.get.reset_mock()
+        # session.get.side_effect = [exceptions.HttpException(),
+        #                            exceptions.HttpException()]
+        # with pytest.raises(OSError):
+        #     test_client.copy(vospaceLocation, osLocation, head=True)
+        # assert session.get.call_count == 2
+        #
+        # # test PUT intermittent exceptions on both URLs
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     return_value=['http://cadc1.ca/test', 'http://cadc2.ca/test'])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.put.reset_mock()
+        # session.put.side_effect = \
+        #     [exceptions.TransferException()] * 2 * vos.MAX_INTERMTTENT_RETRIES
+        # with pytest.raises(OSError):
+        #     test_client.copy(osLocation, vospaceLocation, head=True)
+        # assert session.put.call_count == 2 * vos.MAX_INTERMTTENT_RETRIES
+        #
+        # # test GET Transfer error on one URL and a "permanent" one on the other
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     return_value=['http://cadc1.ca/test', 'http://cadc2.ca/test'])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.put.reset_mock()
+        # session.put.side_effect = [exceptions.TransferException(),
+        #                            exceptions.HttpException(),
+        #                            exceptions.TransferException(),
+        #                            exceptions.TransferException()]
+        # with pytest.raises(OSError):
+        #     test_client.copy(osLocation, vospaceLocation, head=True)
+        # assert session.put.call_count == vos.MAX_INTERMTTENT_RETRIES + 1
+        #
+        # # test GET both "permanent" errors
+        # props.get.side_effect = md5sum
+        # get_node_url_mock = Mock(
+        #     return_value=['http://cadc1.ca/test', 'http://cadc2.ca/test'])
+        # test_client.get_node_url = get_node_url_mock
+        # get_node_mock.reset_mock()
+        # response.iter_content.return_value = BytesIO(file_content)
+        # headers.get.return_value = None
+        # session.put.reset_mock()
+        # session.put.side_effect = [exceptions.HttpException(),
+        #                            exceptions.HttpException()]
+        # with pytest.raises(OSError):
+        #     test_client.copy(osLocation, vospaceLocation, head=True)
+        # assert session.put.call_count == 2
 
     def test_add_props(self):
         old_node = Node(ElementTree.fromstring(NODE_XML))
         old_node.uri = 'vos:sometest'
         new_node = Node(ElementTree.fromstring(NODE_XML))
         new_node.props['quota'] = '1000'
         new_node.create = Mock(return_value=new_node.node)
```

### Comparing `vos-3.6.1/vos/vos.py` & `vos-3.6rc0/vos/vos.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 import warnings
 import copy
 import errno
 from datetime import datetime
 import fnmatch
 from enum import Enum
 import hashlib
+from urllib.parse import quote
 
 try:
     from cStringIO import StringIO
 except ImportError:
     from io import StringIO
 import requests
 from requests.exceptions import HTTPError
@@ -105,14 +106,15 @@
 except ImportError:
     version = "unknown"
 from cadcutils import net, exceptions, util
 from . import md5_cache
 
 from urllib.parse import urlparse, parse_qs
 logger = logging.getLogger('vos')
+logger.setLevel(logging.ERROR)
 
 if sys.version_info[1] > 6:
     logger.addHandler(logging.NullHandler())
 
 # ch = logging.StreamHandler()
 # ch.setLevel(logging.DEBUG)
 # logger.addHandler(ch)
@@ -142,16 +144,15 @@
 SSO_SECURITY_METHODS = {
     'tls-with-certificate': 'ivo://ivoa.net/sso#tls-with-certificate',
     'cookie': 'ivo://ivoa.net/sso#cookie',
     'token': 'vos://cadc.nrc.ca~vospace/CADC/std/Auth#token-1.0'
 }
 
 SUPPORTED_SERVER_VERSIONS = {'vault': '1.1',
-                             'cavern': '1.0',
-                             'storage-inventory/minoc': '1.0'}
+                             'cavern': '0.4'}
 
 # this should one day go into its own uws library
 UWS_NSMAP = {'uws': 'http://www.ivoa.net/xml/UWS/v1.0',
              'xlink': 'http://www.w3.org/1999/xlink'}
 
 
 # sorting-related uris
@@ -1317,15 +1318,19 @@
             "Direct write to a VOSpaceFile is not supported, use "
             "copy instead.")
 
 
 class EndPoints(object):
     VOSPACE_WEBSERVICE = os.getenv('VOSPACE_WEBSERVICE', os.getenv('LOCAL_VOSPACE_WEBSERVICE', None))
 
+    VO_FILES_OLD = 'ivo://ivoa.net/std/VOSpace/v2.x#files'
+    VO_PROPERTIES_OLD = 'vos://cadc.nrc.ca~vospace/CADC/std/VOSpace#nodeprops'
+
     # standard ids
+    # TODO - VO_PROPERTIES has been replaced by VO_RECURSIVE_PROPS
     VO_NODES = 'ivo://ivoa.net/std/VOSpace/v2.0#nodes'
     VO_FILES = 'ivo://ivoa.net/std/VOSpace#files-proto'
     VO_TRANSFER = 'ivo://ivoa.net/std/VOSpace#sync-2.1'
     VO_ASYNC_TRANSFER = 'ivo://ivoa.net/std/VOSpace/v2.0#transfers'
     VO_RECURSIVE_DEL = 'ivo://ivoa.net/std/VOSpace#recursive-delete-proto'
     VO_RECURSIVE_PROPS = 'ivo://ivoa.net/std/VOSpace#recursive-nodeprops-proto'
 
@@ -1391,29 +1396,37 @@
         return self.conn.ws_client._get_url((self.VO_NODES, None))
 
     @property
     def files(self):
         """
         :return: The files service endpoint.
         """
-        return self.conn.ws_client._get_url((self.VO_FILES, None))
+        try:
+            return self.conn.ws_client._get_url((self.VO_FILES, None))
+        except KeyError:
+            # TODO Temporary
+            return self.conn.ws_client._get_url((self.VO_FILES_OLD, None))
 
     @property
     def recursive_del(self):
         """
         :return: recursive delete endpoint
         """
         return self.conn.ws_client._get_url((self.VO_RECURSIVE_DEL, None))
 
     @property
     def recursive_props(self):
         """
         :return: recusive property set endpoint
         """
-        return self.conn.ws_client._get_url((self.VO_RECURSIVE_PROPS, None))
+        try:
+            return self.conn.ws_client._get_url((self.VO_RECURSIVE_PROPS, None))
+        except KeyError:
+            # TODO temporary for regression
+            return self.conn.ws_client._get_url((self.VO_PROPERTIES_OLD, None))
 
     @property
     def session(self):
         # TODO can we use just the ws_client instead?
         return self.conn.ws_client._get_session()
 
     def set_auth(self, vospace_certfile=None, vospace_token=None):
@@ -1514,15 +1527,14 @@
         self.secure_get = secure_get
         self._endpoints = {}
         self.vospace_certfile = vospace_certfile is None and \
             Client.VOSPACE_CERTFILE or vospace_certfile
         self.vospace_token = vospace_token
         self.insecure = insecure
         self._fs_type = True  # True - file system type (cavern), False - db type (vault)
-        self._si_client = None
 
     def glob(self, pathname):
         """Return a list of paths matching a pathname pattern.
 
         The pattern may contain simple shell-style wildcards a la
         fnmatch. However, unlike fnmatch, file names starting with a
         dot are special cases that are not matched by '*' and '?'
@@ -1710,24 +1722,14 @@
     def get_session(self, uri):
         return self.get_endpoints(uri).session
 
     @staticmethod
     def has_magic(s):
         return MAGIC_GLOB_CHECK.search(s) is not None
 
-    def _get_si_client(self, uri):
-        ep = self.get_endpoints(uri)
-        if not self._si_client:
-            self._si_client = net.BaseDataClient(ep.resource_id, ep.subject,
-                                                 ep.conn.ws_client.agent, retry=True,
-                                                 host=ep.conn.ws_client.host,
-                                                 insecure=self.insecure,
-                                                 server_versions=SUPPORTED_SERVER_VERSIONS)
-        return self._si_client
-
     # @logExceptions()
     def copy(self, source, destination, send_md5=False, disposition=False,
              head=None):
         """copy from source to destination.
 
         One of source or destination must be a vospace location and the other
         must be a local location.
@@ -1752,34 +1754,56 @@
 
         """
         # TODO: handle vospace to vospace copies.
 
         success = False
         copy_failed_message = ""
         dest_size = None
+        dest_md5 = None
+        src_size = None
         src_md5 = None
+        check_md5 = True  # by default try to check all md5
         must_delete = False  # delete node after failed transfer
-        transf_file = None
+        # NOTE: file size and md5 are used to check the opportunity (files
+        # migth be the same) and correctness of the file transfer (interrupted
+        # or incomplete transfer). Although the most reliable of the 2,
+        # md5 checksum introduces higher local computational overheads,
+        # (especially for large files) and might not be available on the server
+        # side. Therefore, sometimes size is used instead.
+        # The algorithm tries to strike a balance between efficiency and
+        # reliability. Worst case scenario is updates to large files that
+        # have only the content updated (FITS headers for example). In that
+        # case both md5 checksum and file transfer are performed
+
         get_node_url_retried = False
+        content_disposition = None
         # url retry counter - how many times an url has been retried
 
         if self.is_remote_file(source):
             # GET
             retried_urls = {}
             files_url = None
+            # TODO - remove. This is temporary for regression
+            try:
+                self.get_endpoints(source).recursive_del
+                new_vos = True
+            except KeyError:
+                # TODO - to delete temporary regression code
+                new_vos = False
             if destination is None:
                 # Set the destination, initially, to the same directory as
                 # the source (strip the scheme)
                 destination = os.path.dirname(urlparse(source).path)
             if os.path.isdir(destination):
                 # We can't write to a directory so take file name from
                 # content-disposition or from filename part of source.
                 disposition = True
-            get_urls = []
+            check_md5 = False
             cutout_match = FILENAME_PATTERN_MAGIC.search(source)
+            get_urls = []
             if cutout_match is not None and cutout_match.group('cutout'):
                 view = 'cutout'
                 if cutout_match.group('pix'):
                     cutout = cutout_match.group('pix')
                 elif cutout_match.group('wcs') is not None:
                     cutout = 'CIRCLE=' + '{} {} {}'.format(
                         cutout_match.group('ra'),
@@ -1790,64 +1814,138 @@
                 source = cutout_match.group('filename')
             elif head:
                 view = 'header'
                 cutout = None
             else:
                 view = 'data'
                 cutout = None
+                check_md5 = True
+                src_md5 = None
+                src_size = None
+                if new_vos:
+                    files_url = self.get_node_url(source, method='GET',
+                                                  cutout=cutout,
+                                                  view=view)
+                    if files_url:
+                        try:
+                            response = self.get_session(source).head(files_url)
+                            response.raise_for_status()
+                            src_md5 = net.extract_md5(response.headers)
+                            src_size = response.headers.get('Content-Length', None)
+                            get_urls.append(
+                                self._add_soda_ops(files_url, view=view, cutout=cutout))
+                        except Exception:
+                            # not much to do. With transfer negotiation it could
+                            # try a different URL.
+                            pass
+                else:
+                    source_props = self.get_node(source, force=True).props
+                    src_md5 = source_props.get('MD5', None)
+                    src_size = source_props.get('length', None)
+                if src_size:
+                    src_size = int(src_size)
+                if src_size == 0:
+                    if os.path.isdir(destination):
+                        dest_name = os.path.split(source)[-1]
+                        destination = os.path.join(destination, dest_name)
+                    if os.path.isfile(destination) and os.stat(destination).st_size == 0:
+                        logger.info('copy: src and dest are already the same')
+                    else:
+                        open(destination, 'w').write('')
+                    if send_md5:
+                        return ZERO_MD5
+                    return 0
+
+                if os.path.isfile(destination):
+                    # check if the local file is up to date before doing the
+                    # transfer. Use size for first comparison as it's faster
+                    dest_size = os.stat(destination).st_size
+                    if dest_size == src_size:
+                        # calculate the destination md5
+                        dest_md5 = \
+                            md5_cache.MD5Cache.compute_md5(destination)
+                        if src_md5 == dest_md5:
+                            logger.info(
+                                'copy: src and dest are already the same')
+                            if disposition:
+                                return None
+                            if send_md5:
+                                return dest_md5
+                            return dest_size
 
             if self._fs_type and (cutout or view == 'header'):
                 raise ValueError('cavern/arc service does not support cutouts or header operations')
 
-            files_url = self.get_node_url(source, method='GET',
-                                          cutout=cutout,
-                                          view=view)
-            try:
-                transf_file = self._get_si_client(source).download_file(
-                    url=files_url, dest=destination,
-                    params=self._get_soda_params(view=view, cutout=cutout))
-                success = True
-            except Exception as e:
-                # not much to do but to fall through with full negotiation
-                logger.debug('GET fail on files endpoint for {}'.format(source), e)
-
-            if not success:
-                # at this point it's probably time to check whether the node is actually empty
-                src_node = self.get_node(source, force=True)
-                src_size = src_node.props.get('length', None)
-                src_size = int(src_size)
-                if src_size == 0:
-                    dest_file = destination
-                    if os.path.isdir(dest_file):
-                        dest_file = os.path.join(dest_file, os.path.basename(source))
-                    open(dest_file, 'wb').write(b'')  # empty file
-                    transf_file = dest_file, ZERO_MD5, 0
-                    dest_size = 0
-                    success = True
-
             while not success:
                 if len(get_urls) == 0:
                     if not get_node_url_retried:
                         get_urls = self.get_node_url(source, method='GET',
                                                      cutout=cutout, view=view,
                                                      full_negotiation=True)
-                        if len(get_urls) > 1:
-                            # remove files_url that we've tried already
+                        # remove files_url that we've tried already
+                        if new_vos:
+                            get_urls = [self._add_soda_ops(url, view=view, cutout=cutout)
+                                        for url in get_urls if url != files_url]
+                        else:
                             get_urls = [url for url in get_urls if url != files_url]
                         get_node_url_retried = True
                 if len(get_urls) == 0:
                     break
                 get_url = get_urls.pop(0)
 
                 try:
-                    transf_file = self._get_si_client(source).download_file(
-                        url=get_url, dest=destination,
-                        params=self._get_soda_params(view=view, cutout=cutout))
+                    response = self.get_session(source).get(
+                        get_url, stream=True)
+                    response.raise_for_status()
+                    if disposition:
+                        # Build the destination location from the
+                        # content-disposition value, or source name.
+                        content_disposition = response.headers.get(
+                            'content-disposition', destination)
+                        content_disposition = re.search(r'.*filename=(\S*).*',
+                                                        content_disposition)
+                        if content_disposition is not None:
+                            content_disposition = content_disposition.group(
+                                1).strip()
+                        else:
+                            content_disposition = os.path.split(source)[-1]
+                        if os.path.isdir(destination):
+                            destination = os.path.join(destination,
+                                                       content_disposition)
+                    src_md5 = response.headers.get('Content-MD5', None)
+                    if src_md5:
+                        # server knows to do md5s even for cutouts or headers
+                        check_md5 = True
+                    transfer_md5 = hashlib.md5()
+                    with open(destination, 'wb') as fout:
+                        for chunk in response.iter_content(
+                                chunk_size=512 * 1024):
+                            if chunk:
+                                transfer_md5.update(chunk)
+                                fout.write(chunk)
+                                fout.flush()
+                    dest_md5 = transfer_md5.hexdigest()
+                    dest_size = os.stat(destination).st_size
+                    if check_md5:
+                        if src_md5:
+                            if dest_md5 != src_md5:
+                                raise IOError(
+                                    'Source and destination md5 do not  '
+                                    'match: {} vs. {}'.format(src_md5,
+                                                              dest_md5))
+                        elif src_size:
+                            if dest_size != src_size:
+                                raise exceptions.TransferException(
+                                    'Source and destination sizes do not '
+                                    'match: {} vs. {}'.format(src_size,
+                                                              dest_size))
+                        else:
+                            logger.debug(
+                                "Source md5 or size not available to check")
                     success = True
-                    break
                 except exceptions.HttpException as ex:
                     msg = ''
                     if isinstance(ex, exceptions.TransferException):
                         msg = ' (intermittent error)'
                         retried_urls[get_url] = \
                             retried_urls.get(get_url, 0) + 1
                         if retried_urls[get_url] < MAX_INTERMTTENT_RETRIES:
@@ -1856,20 +1954,20 @@
                     copy_failed_message = str(ex)
                     logging.debug("Failed to GET {0}: {1}{2}".format(
                         get_url, str(ex), msg))
                     continue
         else:
             # PUT
             success = False
+            dest_md5 = None
             dest_size = None
             destination_node = None
-            dest_node_md5 = None
             try:
                 destination_node = self.get_node(destination, force=True)
-                dest_node_md5 = destination_node.props.get('MD5', None)
+                dest_md5 = destination_node.props.get('MD5', None)
                 dest_size = destination_node.props.get('length', None)
                 if dest_size:
                     dest_size = int(dest_size)
             except Exception:
                 pass
             src_size = os.stat(source).st_size
             # check 2 cases where file sending not required:
@@ -1878,80 +1976,164 @@
             if src_size == 0:
                 logger.info("src: size is 0")
                 if destination_node:
                     # TODO delete and recreate the node. Is there a better way
                     # to delete just the content of the node?
                     self.delete(destination)
                 self.create(destination)
-                transf_file = os.path.basename(destination), ZERO_MD5, 0
+                destination_node = self.get_node(destination, force=True)
+                dest_md5 = destination_node.props.get('MD5')
+                dest_size = destination_node.props.get('length')
+                # In vault the presence of size is optional
+                if dest_size is not None:
+                    dest_size = int(dest_size)
+                    if dest_size != src_size:
+                        raise IOError(
+                            "Source size ({}) != destination size ({})".
+                            format(src_size, dest_size))
                 success = True
             elif src_size == dest_size:
-                if dest_node_md5 is not None:
+                if dest_md5 is not None:
                     # compute the md5 of the source file. This serves 2
                     # purposes:
                     #   1. Check if source is identical to destination and
                     #   avoid sending the bytes again.
                     #   2. send info to the service so it can recover in case
                     #   the bytes got corrupted on the way
                     src_md5 = md5_cache.MD5Cache.compute_md5(source)
-                    if src_md5 == dest_node_md5:
-                        logger.info('Source and destination identical for {}. Skip transfer!'.format(source))
+                    if src_md5 == dest_md5:
+                        logger.info(
+                            'copy: src and dest are already the same -> '
+                            'update node metadata')
                         # post the node so that the modify time is updated
                         self.update(destination_node)
-                        transf_file = os.path.basename(destination), dest_node_md5, dest_size
                         success = True
             if not success:
-                # transfer the bytes with source md5 available
-                while not success:
-                    if not get_node_url_retried:
-                        put_urls = self.get_node_url(
-                            destination, method='PUT',
-                            full_negotiation=True)
-                        get_node_url_retried = True
-                    if len(put_urls) == 0:
+                if dest_md5 is not None:
+                    if not src_md5:
+                        src_md5 = md5_cache.MD5Cache.compute_md5(source)
+                    # transfer the bytes with source md5 available
+                    put_urls = self.get_node_url(destination, 'PUT',
+                                                 content_length=src_size,
+                                                 md5_checksum=dest_md5)
+                    while not success:
+                        if len(put_urls) == 0:
+                            if not get_node_url_retried:
+                                put_urls = self.get_node_url(
+                                    destination, method='PUT',
+                                    full_negotiation=True)
+                                # remove the first one as we already tried
+                                # that one.
+                                if put_urls:
+                                    put_urls.pop(0)
+                                get_node_url_retried = True
+                        if len(put_urls) == 0:
+                            break
+                        put_url = put_urls.pop(0)
+                        try:
+                            with open(source, str('rb')) as fin:
+                                response = self.get_session(destination).put(
+                                    put_url, data=fin)
+                            response.raise_for_status()
+                            dest_md5 = net.extract_md5(response.headers)
+                            if dest_md5 and dest_md5 != src_md5:
+                                # raise TransferException so that the URL
+                                # can be retried later
+                                raise exceptions.TransferException(
+                                   "Source md5 ({}) != destination md5 ({})".
+                                   format(src_md5, dest_md5))
+                        except exceptions.HttpException as ex:
+                            msg = ''
+                            if isinstance(ex, exceptions.TransferException):
+                                msg = ' (intermittent error)'
+                                retried_urls[put_url] = retried_urls.get(
+                                    put_url, 0) + 1
+                                if retried_urls[put_url] < \
+                                        MAX_INTERMTTENT_RETRIES:
+                                    # intermittent error - worth retrying later
+                                    put_urls.append(put_url)
+                            copy_failed_message = str(ex)
+                            logger.debug(
+                                "FAILED to PUT to {0}: {1}{2}".format(
+                                    put_url, str(ex), msg))
+                            continue
+                        success = True
                         break
-                    put_url = put_urls.pop(0)
-                    try:
-                        transf_file = self._get_si_client(destination).upload_file(
-                            url=put_url,
-                            src=source,
-                            md5_checksum=src_md5)
-                    except Exception as ex:
-                        msg = ''
-                        if isinstance(ex, exceptions.TransferException):
-                            msg = ' (intermittent error)'
-                            retried_urls[put_url] = retried_urls.get(
-                                put_url, 0) + 1
-                            if retried_urls[put_url] < \
-                                    MAX_INTERMTTENT_RETRIES:
-                                # intermittent error - worth retrying later
-                                put_urls.append(put_url)
-                        copy_failed_message = str(ex)
-                        logger.debug(
-                            "FAILED to PUT to {0}: {1}{2}".format(
-                                put_url, str(ex), msg))
-                        continue
-                    success = True
-                    break
+                else:
+                    must_delete = True
+                    # transfer the bytes and compute md5 on-the-fly
+                    put_urls = self.get_node_url(destination, 'PUT')
+                    while not success:
+                        if len(put_urls) == 0:
+                            if not get_node_url_retried:
+                                put_urls = self.get_node_url(
+                                    destination, method='PUT',
+                                    full_negotiation=True)
+                                # remove the first one as we already tried
+                                # that one.
+                                if put_urls:
+                                    put_urls.pop(0)
+                                get_node_url_retried = True
+                        if len(put_urls) == 0:
+                            break
+                        put_url = put_urls.pop(0)
+                        try:
+                            with Md5File(source, 'rb') as reader:
+                                response = self.get_session(destination).put(
+                                    put_url, data=reader)
+                            response.raise_for_status()
+                            src_md5 = reader.md5_checksum
+                            dest_md5 = net.extract_md5(response.headers)
+                            if dest_md5 and dest_md5 != src_md5:
+                                # raise TransferException so that the URL
+                                # can be retried later
+                                raise exceptions.TransferException(
+                                    "Source md5 ({}) != destination md5 ({})".
+                                    format(src_md5, dest_md5))
+                            success = True
+                        except exceptions.HttpException as ex:
+                            msg = ''
+                            if isinstance(ex, exceptions.TransferException):
+                                msg = ' (intermittent error)'
+                                retried_urls[put_url] = retried_urls.get(
+                                    put_url, 0) + 1
+                                if retried_urls[put_url] < \
+                                        MAX_INTERMTTENT_RETRIES:
+                                    # intermittent error - worth retrying later
+                                    put_urls.append(put_url)
+                            copy_failed_message = str(ex)
+                            logger.debug(
+                                "FAILED to PUT to site {0}: {1}{2}".format(
+                                    put_url, str(ex), msg))
+                            continue
+                        break
+
         if not success:
             if must_delete:
                 # cleanup
                 self.delete(destination)
             raise OSError(errno.EFAULT,
-                          "Failed copying {0} -> {1}.\nReason for failure: {2}".
+                          "Failed copying {0} -> {1} and also failed "
+                          "cleaning up after.\nReason for failure: {2}".
+                          format(source, destination, copy_failed_message))
+        elif check_md5 and src_md5 and dest_md5 and src_md5 != dest_md5:
+            copy_failed_message = 'BUG: Mismatched md5 src ({}) != dest ({})'.\
+                format(src_md5, dest_md5)
+            raise OSError(errno.EFAULT,
+                          "Failed copying {0} -> {1}\n{2}".
                           format(source, destination, copy_failed_message))
         else:
-            logger.info('Transfer successful')
-        if transf_file is None:
-            raise RuntimeError('BUG: Not found details of successful transfer')
-        if disposition and transf_file:
-            return transf_file[0]  # file name
-        if send_md5 and transf_file:
-            return transf_file[1]  # file md5
-        return transf_file[2]  # file size
+            logger.info(
+                'Transfer successful: source md5 ({}) == destination md5 ({})'.
+                format(src_md5, dest_md5))
+        if disposition:
+            return content_disposition
+        if send_md5:
+            return dest_md5
+        return dest_size
 
     def fix_uri(self, uri):
         """given a uri check if the authority part is there and if it isn't
         then add the VOSpace authority
 
         :param uri: The string that should be parsed into a proper URI, if
         possible.
@@ -2175,17 +2357,29 @@
             logger.debug('URL: {} ({})'.format(url, method))
             return url
 
         # This is the shortcut. We do a GET request on the service with the
         # parameters sent as arguments.
 
         direction = {'GET': 'pullFromVoSpace', 'PUT': 'pushToVoSpace'}
-        urls = self.transfer(self.get_endpoints(uri).transfer, uri, direction[method], None, None)
-        logger.debug('Transfer URLs: ' + ', '.join(urls))
-        return urls
+        try:
+            self.get_endpoints(uri).recursive_del
+            urls = self.transfer(self.get_endpoints(uri).transfer, uri, direction[method], None, None)
+            logger.debug('Transfer URLs: ' + ', '.join(urls))
+            return urls
+        except KeyError:
+            # TODO - delete temporary code for regression
+            old_cutout = cutout
+            if old_cutout:
+                old_cutout = old_cutout.replace('CIRCLE=', 'CIRCLE ICRS ')
+                old_cutout = old_cutout.replace('SUB=', 'CUTOUT ')
+            urls = self.transfer(self.get_endpoints(uri).transfer, uri,
+                                 direction[method], view=view, cutout=old_cutout)
+            logger.debug('Transfer URLs: ' + ', '.join(urls))
+            return urls
 
     def link(self, src_uri, link_uri):
         """Make link_uri point to src_uri.
 
         :param src_uri: the existing resource, either a vospace uri or a http
         url
         :type src_uri: unicode
@@ -2259,26 +2453,26 @@
                 response.raise_for_status()
             except Exception:
                 return None
             if response.status_code == 303:
                 return response.headers.get('Location', None)
             return None
 
-    def _get_soda_params(self, view=None, cutout=None):
-        # returns HTTP header corresponding to the soda params
-        result = {}
+    def _add_soda_ops(self, url, view=None, cutout=None):
+        # assume that the url points to a SODA service
+        result = url
         if view == 'header':
-            result['META'] = 'true'
+            result = '{}?META=true'.format(result)
         elif cutout:
             if cutout.strip().startswith('['):
                 # pixel cutout
-                result['SUB'] = cutout
+                result = '{}?SUB={}'.format(result, cutout)
             elif cutout.strip().startswith('CIRCLE'):
                 # circle cutout
-                result['CIRCLE'] = cutout.replace('CIRCLE=', '')
+                result = '{}?CIRCLE={}'.format(result, quote(cutout.replace('CIRCLE=', '')))
             else:
                 # TODO add support for other SODA cutouts SUB, POL etc
                 raise ValueError('Unknown cutout type: ' + cutout)
         return result
 
     def _put(self, uri, content_length=None, md5_checksum=None):
         with nodeCache.volatile(uri):
```

### Comparing `vos-3.6.1/vos/vosconfig.py` & `vos-3.6rc0/vos/vosconfig.py`

 * *Files identical despite different names*

### Comparing `vos-3.6.1/vos.egg-info/PKG-INFO` & `vos-3.6rc0/vos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vos
-Version: 3.6.1
+Version: 3.6rc0
 Summary: CADC VOS Class Libraries
 Home-page: https://www.canfar.net/en/docs/storage
 Author: JJ Kavelaars, Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
 Project-URL: Source, https://github.com/opencadc/vostools
 Project-URL: Issues, https://github.com/opencadc/vostools/issues
@@ -12,15 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7, <4
 License-File: LICENSE
 Requires-Dist: html2text>=2016.5.29
-Requires-Dist: cadcutils>=1.5.2.2
+Requires-Dist: cadcutils>=1.5.1
 Requires-Dist: aenum
 Provides-Extra: test
 Requires-Dist: pytest>=4.6; extra == "test"
 Requires-Dist: pytest-cov>=2.5.1; extra == "test"
 Requires-Dist: flake8>=3.4.1; extra == "test"
 
 DOCUMENTATION
```

### Comparing `vos-3.6.1/vos.egg-info/SOURCES.txt` & `vos-3.6rc0/vos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

