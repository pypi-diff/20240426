# Comparing `tmp/super-ide-1.4.8.tar.gz` & `tmp/super-ide-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super-ide-1.4.8.tar", last modified: Fri Apr  5 05:04:10 2024, max compression
+gzip compressed data, was "super-ide-1.5.0.tar", last modified: Fri Apr 26 14:58:54 2024, max compression
```

## Comparing `super-ide-1.4.8.tar` & `super-ide-1.5.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:10.845612 super-ide-1.4.8/
--rwxrwxrwx   0 denk      (1000) denk      (1000)    34520 2024-04-03 15:40:53.000000 super-ide-1.4.8/LICENSE
--rwxrwxrwx   0 denk      (1000) denk      (1000)      111 2024-04-03 15:40:53.000000 super-ide-1.4.8/MANIFEST.in
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2187 2024-04-05 05:04:10.822430 super-ide-1.4.8/PKG-INFO
--rwxrwxrwx   0 denk      (1000) denk      (1000)      790 2024-04-03 15:40:53.000000 super-ide-1.4.8/README.rst
--rwxrwxrwx   0 denk      (1000) denk      (1000)       38 2024-04-05 05:04:10.848112 super-ide-1.4.8/setup.cfg
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3436 2024-04-03 15:40:53.000000 super-ide-1.4.8/setup.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:51.684482 super-ide-1.4.8/super_ide.egg-info/
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2187 2024-04-05 05:03:48.000000 super-ide-1.4.8/super_ide.egg-info/PKG-INFO
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2588 2024-04-05 05:03:50.000000 super-ide-1.4.8/super_ide.egg-info/SOURCES.txt
--rwxrwxrwx   0 denk      (1000) denk      (1000)        1 2024-04-05 05:03:48.000000 super-ide-1.4.8/super_ide.egg-info/dependency_links.txt
--rwxrwxrwx   0 denk      (1000) denk      (1000)      161 2024-04-05 05:03:48.000000 super-ide-1.4.8/super_ide.egg-info/entry_points.txt
--rwxrwxrwx   0 denk      (1000) denk      (1000)      284 2024-04-05 05:03:48.000000 super-ide-1.4.8/super_ide.egg-info/requires.txt
--rwxrwxrwx   0 denk      (1000) denk      (1000)        9 2024-04-05 05:03:48.000000 super-ide-1.4.8/super_ide.egg-info/top_level.txt
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:54.064067 super-ide-1.4.8/superide/
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2026 2024-04-05 04:45:54.000000 super-ide-1.4.8/superide/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     4449 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/__main__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     8340 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/app.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:54.657714 super-ide-1.4.8/superide/boards/
--rwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/boards/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      207 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/boards/boards.json
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2937 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/boards/cli.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     5203 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/cache.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3277 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/cli.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3553 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/compat.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:56.971315 super-ide-1.4.8/superide/debug/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6135 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/cli.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:58.331334 super-ide-1.4.8/superide/debug/config/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     8965 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/base.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2068 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/blackmagic.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1742 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/factory.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      969 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/generic.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1161 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/jlink.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      921 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/mspdebug.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      962 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/native.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      962 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/qemu.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1156 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/renode.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1195 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/exception.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     5218 2024-04-05 04:51:38.000000 super-ide-1.4.8/superide/debug/helpers.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:58.890354 super-ide-1.4.8/superide/debug/process/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/debug/process/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     4891 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/debug/process/base.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3449 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/debug/process/client.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     7141 2024-04-05 04:49:29.000000 super-ide-1.4.8/superide/debug/process/gdb.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     5727 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/debug/process/server.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3197 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/exception.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6701 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/fs.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:59.253784 super-ide-1.4.8/superide/home/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/home/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3986 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/home/app.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3208 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/home/cli.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:59.334033 super-ide-1.4.8/superide/home/rpc/
--rwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/__init__.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:00.747522 super-ide-1.4.8/superide/home/rpc/handlers/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2839 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/app.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      603 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/base.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2928 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/ide.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6430 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/os.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)    16695 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/project.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1202 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/registry.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      627 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/runServer.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:00.792499 super-ide-1.4.8/superide/home/static/
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:00.981417 super-ide-1.4.8/superide/home/static/assets/
--rwxrwxrwx   0 denk      (1000) denk      (1000)    15406 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/static/assets/favicon.ico
--rwxrwxrwx   0 denk      (1000) denk      (1000)   107097 2024-04-03 15:41:01.000000 super-ide-1.4.8/superide/home/static/assets/index-6fed80ed.css
--rwxrwxrwx   0 denk      (1000) denk      (1000)   439260 2024-04-03 15:41:02.000000 super-ide-1.4.8/superide/home/static/assets/index-d2bbbc6e.js
--rwxrwxrwx   0 denk      (1000) denk      (1000)      529 2024-04-03 15:41:04.000000 super-ide-1.4.8/superide/home/static/index.html
--rwxrwxrwx   0 denk      (1000) denk      (1000)     7468 2024-04-03 15:41:05.000000 super-ide-1.4.8/superide/http.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3522 2024-04-03 15:41:05.000000 super-ide-1.4.8/superide/lockfile.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)    10459 2024-04-03 15:41:05.000000 super-ide-1.4.8/superide/maintenance.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6432 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/proc.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:01.421762 super-ide-1.4.8/superide/project/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      960 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/cli.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:04.150597 super-ide-1.4.8/superide/project/commands/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/commands/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3253 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/commands/config.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     5446 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/commands/init.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2833 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/commands/metadata.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)    18874 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/config.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1846 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/exception.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6607 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/helpers.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)    31369 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/options.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3084 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/savedeps.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     8513 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/vcsclient.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1392 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/public.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:04.539155 super-ide-1.4.8/superide/registry/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/registry/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2900 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/registry/cli.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     8683 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/registry/client.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3690 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/registry/mirror.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:05.034778 super-ide-1.4.8/superide/run/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/run/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     9493 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/run/cli.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1600 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/run/helpers.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6718 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/run/processor.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:05.345009 super-ide-1.4.8/superide/system/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/system/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      971 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/system/cli.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:09.805641 super-ide-1.4.8/superide/system/commands/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/system/commands/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2448 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/system/commands/completion.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2933 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/system/commands/info.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3242 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/system/completion.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)    10925 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/telemetry.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:10.654629 super-ide-1.4.8/superide/toolchain/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/toolchain/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3569 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/toolchain/toolchain.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     5895 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/util.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:10.746552 super-ide-1.4.8/tests/
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3437 2024-04-03 15:41:07.000000 super-ide-1.4.8/tests/test_examples.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:54.654305 super-ide-1.5.0/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    34520 2024-04-03 15:40:53.000000 super-ide-1.5.0/LICENSE
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      111 2024-04-03 15:40:53.000000 super-ide-1.5.0/MANIFEST.in
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2206 2024-04-26 14:58:54.645712 super-ide-1.5.0/PKG-INFO
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      790 2024-04-03 15:40:53.000000 super-ide-1.5.0/README.rst
+-rwxrwxrwx   0 denk      (1000) denk      (1000)       38 2024-04-26 14:58:54.658429 super-ide-1.5.0/setup.cfg
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3436 2024-04-03 15:40:53.000000 super-ide-1.5.0/setup.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:57:45.482602 super-ide-1.5.0/super_ide.egg-info/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2206 2024-04-26 14:57:18.000000 super-ide-1.5.0/super_ide.egg-info/PKG-INFO
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2588 2024-04-26 14:57:29.000000 super-ide-1.5.0/super_ide.egg-info/SOURCES.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        1 2024-04-26 14:57:18.000000 super-ide-1.5.0/super_ide.egg-info/dependency_links.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      162 2024-04-26 14:57:18.000000 super-ide-1.5.0/super_ide.egg-info/entry_points.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      284 2024-04-26 14:57:18.000000 super-ide-1.5.0/super_ide.egg-info/requires.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        9 2024-04-26 14:57:18.000000 super-ide-1.5.0/super_ide.egg-info/top_level.txt
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:57:53.766468 super-ide-1.5.0/superide/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2087 2024-04-26 14:51:19.000000 super-ide-1.5.0/superide/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     4449 2024-04-03 15:40:53.000000 super-ide-1.5.0/superide/__main__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8340 2024-04-03 15:40:53.000000 super-ide-1.5.0/superide/app.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:57:55.972686 super-ide-1.5.0/superide/boards/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:40:53.000000 super-ide-1.5.0/superide/boards/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      207 2024-04-03 15:40:53.000000 super-ide-1.5.0/superide/boards/boards.json
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2937 2024-04-03 15:40:53.000000 super-ide-1.5.0/superide/boards/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5203 2024-04-03 15:40:53.000000 super-ide-1.5.0/superide/cache.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3277 2024-04-03 15:40:53.000000 super-ide-1.5.0/superide/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3553 2024-04-03 15:40:53.000000 super-ide-1.5.0/superide/compat.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:57:58.798969 super-ide-1.5.0/superide/debug/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:53.000000 super-ide-1.5.0/superide/debug/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6319 2024-04-26 08:57:38.000000 super-ide-1.5.0/superide/debug/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:09.643055 super-ide-1.5.0/superide/debug/config/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      559 2024-04-26 09:53:29.000000 super-ide-1.5.0/superide/debug/config/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8915 2024-04-26 09:53:24.000000 super-ide-1.5.0/superide/debug/config/base.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2015 2024-04-26 09:53:54.000000 super-ide-1.5.0/superide/debug/config/blackmagic.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1706 2024-04-26 09:53:18.000000 super-ide-1.5.0/superide/debug/config/factory.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      916 2024-04-26 09:54:07.000000 super-ide-1.5.0/superide/debug/config/generic.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1108 2024-04-26 09:54:13.000000 super-ide-1.5.0/superide/debug/config/jlink.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      868 2024-04-26 09:54:17.000000 super-ide-1.5.0/superide/debug/config/mspdebug.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      909 2024-04-26 09:54:24.000000 super-ide-1.5.0/superide/debug/config/native.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      909 2024-04-26 09:54:29.000000 super-ide-1.5.0/superide/debug/config/qemu.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1192 2024-04-26 09:54:34.000000 super-ide-1.5.0/superide/debug/config/renode.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1195 2024-04-03 15:40:53.000000 super-ide-1.5.0/superide/debug/exception.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5218 2024-04-05 04:51:38.000000 super-ide-1.5.0/superide/debug/helpers.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:13.386086 super-ide-1.5.0/superide/debug/process/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:54.000000 super-ide-1.5.0/superide/debug/process/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     4891 2024-04-03 15:40:54.000000 super-ide-1.5.0/superide/debug/process/base.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3448 2024-04-26 09:55:02.000000 super-ide-1.5.0/superide/debug/process/client.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     7722 2024-04-26 14:17:37.000000 super-ide-1.5.0/superide/debug/process/gdb.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5727 2024-04-03 15:40:54.000000 super-ide-1.5.0/superide/debug/process/server.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3197 2024-04-03 15:40:54.000000 super-ide-1.5.0/superide/exception.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6701 2024-04-03 15:40:54.000000 super-ide-1.5.0/superide/fs.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:15.303843 super-ide-1.5.0/superide/home/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:40:54.000000 super-ide-1.5.0/superide/home/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3986 2024-04-03 15:40:54.000000 super-ide-1.5.0/superide/home/app.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3208 2024-04-03 15:40:54.000000 super-ide-1.5.0/superide/home/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:15.737809 super-ide-1.5.0/superide/home/rpc/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:41:00.000000 super-ide-1.5.0/superide/home/rpc/__init__.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:21.477290 super-ide-1.5.0/superide/home/rpc/handlers/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:00.000000 super-ide-1.5.0/superide/home/rpc/handlers/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2839 2024-04-03 15:41:00.000000 super-ide-1.5.0/superide/home/rpc/handlers/app.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      603 2024-04-03 15:41:00.000000 super-ide-1.5.0/superide/home/rpc/handlers/base.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2928 2024-04-03 15:41:00.000000 super-ide-1.5.0/superide/home/rpc/handlers/ide.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6430 2024-04-03 15:41:00.000000 super-ide-1.5.0/superide/home/rpc/handlers/os.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    16695 2024-04-03 15:41:00.000000 super-ide-1.5.0/superide/home/rpc/handlers/project.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1202 2024-04-03 15:41:00.000000 super-ide-1.5.0/superide/home/rpc/handlers/registry.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      627 2024-04-03 15:41:00.000000 super-ide-1.5.0/superide/home/runServer.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:21.561415 super-ide-1.5.0/superide/home/static/
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:22.360168 super-ide-1.5.0/superide/home/static/assets/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    15406 2024-04-03 15:41:00.000000 super-ide-1.5.0/superide/home/static/assets/favicon.ico
+-rwxrwxrwx   0 denk      (1000) denk      (1000)   107097 2024-04-03 15:41:01.000000 super-ide-1.5.0/superide/home/static/assets/index-6fed80ed.css
+-rwxrwxrwx   0 denk      (1000) denk      (1000)   439260 2024-04-03 15:41:02.000000 super-ide-1.5.0/superide/home/static/assets/index-d2bbbc6e.js
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      529 2024-04-03 15:41:04.000000 super-ide-1.5.0/superide/home/static/index.html
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     7468 2024-04-03 15:41:05.000000 super-ide-1.5.0/superide/http.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3522 2024-04-03 15:41:05.000000 super-ide-1.5.0/superide/lockfile.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    10459 2024-04-03 15:41:05.000000 super-ide-1.5.0/superide/maintenance.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6432 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/proc.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:37.284613 super-ide-1.5.0/superide/project/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      960 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:37.923795 super-ide-1.5.0/superide/project/commands/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/commands/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3253 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/commands/config.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5446 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/commands/init.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2833 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/commands/metadata.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    18874 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/config.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1846 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/exception.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6674 2024-04-26 09:29:33.000000 super-ide-1.5.0/superide/project/helpers.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    31369 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/options.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3084 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/savedeps.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8513 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/project/vcsclient.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1392 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/public.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:39.877866 super-ide-1.5.0/superide/registry/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/registry/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2900 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/registry/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8683 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/registry/client.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3690 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/registry/mirror.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:47.675563 super-ide-1.5.0/superide/run/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/run/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     9493 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/run/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1600 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/run/helpers.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6718 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/run/processor.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:50.174423 super-ide-1.5.0/superide/system/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/system/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      971 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/system/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:52.508816 super-ide-1.5.0/superide/system/commands/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.5.0/superide/system/commands/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2448 2024-04-03 15:41:07.000000 super-ide-1.5.0/superide/system/commands/completion.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2933 2024-04-03 15:41:07.000000 super-ide-1.5.0/superide/system/commands/info.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3242 2024-04-03 15:41:07.000000 super-ide-1.5.0/superide/system/completion.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    10885 2024-04-26 14:23:47.000000 super-ide-1.5.0/superide/telemetry.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:52.866627 super-ide-1.5.0/superide/toolchain/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:07.000000 super-ide-1.5.0/superide/toolchain/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3675 2024-04-26 14:30:29.000000 super-ide-1.5.0/superide/toolchain/toolchain.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5895 2024-04-03 15:41:07.000000 super-ide-1.5.0/superide/util.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-26 14:58:53.231478 super-ide-1.5.0/tests/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3437 2024-04-03 15:41:07.000000 super-ide-1.5.0/tests/test_examples.py
```

### Comparing `super-ide-1.4.8/LICENSE` & `super-ide-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/PKG-INFO` & `super-ide-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: super-ide
-Version: 1.4.8
+Version: 1.5.0
 Summary: A professional Cross-platform IDE. Cross-platform IDE and Unified Debugger. Static Code Analyzer and Remote Unit Testing. Multi-platform and Multi-architecture Build System. Firmware File Explorer and Memory Inspection. IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, STMicroelectronics (STM8/STM32), Teensy
 Home-page: https://mengning.com.cn
 Author: Mengning Software
 Author-email: contact@mengning.com.cn
 License: AGPL-3.0 License
 Keywords: iot,embedded,arduino,mbed,esp8266,esp32,fpga,firmware,continuous-integration,cloud-ide,avr,arm,ide,unit-testing,hardware,verilog,microcontroller,debug
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
@@ -42,7 +43,8 @@
 
 License
 -------
 
 Copyright (c) 2022-present Mengning <contact@mengning.com.cn>
 
 The Super IDE is licensed under the AGPL 3.0 license or commercial license.
+
```

### Comparing `super-ide-1.4.8/README.rst` & `super-ide-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/setup.py` & `super-ide-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/super_ide.egg-info/PKG-INFO` & `super-ide-1.5.0/super_ide.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: super-ide
-Version: 1.4.8
+Version: 1.5.0
 Summary: A professional Cross-platform IDE. Cross-platform IDE and Unified Debugger. Static Code Analyzer and Remote Unit Testing. Multi-platform and Multi-architecture Build System. Firmware File Explorer and Memory Inspection. IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, STMicroelectronics (STM8/STM32), Teensy
 Home-page: https://mengning.com.cn
 Author: Mengning Software
 Author-email: contact@mengning.com.cn
 License: AGPL-3.0 License
 Keywords: iot,embedded,arduino,mbed,esp8266,esp32,fpga,firmware,continuous-integration,cloud-ide,avr,arm,ide,unit-testing,hardware,verilog,microcontroller,debug
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
@@ -42,7 +43,8 @@
 
 License
 -------
 
 Copyright (c) 2022-present Mengning <contact@mengning.com.cn>
 
 The Super IDE is licensed under the AGPL 3.0 license or commercial license.
+
```

### Comparing `super-ide-1.4.8/super_ide.egg-info/SOURCES.txt` & `super-ide-1.5.0/super_ide.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/__init__.py` & `super-ide-1.5.0/superide/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# Copyright (c) Mengning Software. 2023. All rights reserved.
-#
-# Super IDE licensed under GNU Affero General Public License v3 (AGPL-3.0) .
-# You can use this software according to the terms and conditions of the AGPL-3.0.
-# You may obtain a copy of AGPL-3.0 at:
-#
-#    https://www.gnu.org/licenses/agpl-3.0.txt
-#
-# THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
-# PURPOSE.
-# See the AGPL-3.0 for more details.
-
-VERSION = (1, 4, 8)
-__version__ = ".".join([str(s) for s in VERSION])
-
-__title__ = "super-ide"
-__description__ = (
-    "A professional Cross-platform IDE. "
-    "Cross-platform IDE and Unified Debugger. "
-    "Static Code Analyzer and Remote Unit Testing. "
-    "Multi-platform and Multi-architecture Build System. "
-    "Firmware File Explorer and Memory Inspection. "
-    "IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, "
-    "STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, "
-    "MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, "
-    "STMicroelectronics (STM8/STM32), Teensy"
-)
-__url__ = "https://mengning.com.cn"
-
-__author__ = "Mengning Software"
-__email__ = "contact@mengning.com.cn"
-
-__license__ = "AGPL-3.0 License"
-__copyright__ = "Copyright 2014-present Mengning Software"
-
-__accounts_api__ = "https://api.accounts.mengning.com.cn"
-__registry_mirror_hosts__ = [
-    "registry.mengning.com.cn",
-    "registry.nm1.mengning.com.cn",
-]
-__pioremote_endpoint__ = "ssl:host=remote.mengning.com.cn:port=4413"
-
-__core_packages__ = {
-    "tool-scons": "~4.40502.0",
-    "tool-cppcheck": "~1.270.0",
-    "tool-clangtidy": "~1.150005.0",
-    "tool-pvs-studio": "~7.18.0",
-}
-
-__check_internet_hosts__ = [
-    "185.199.110.153",  # Github.com
-    "88.198.170.159",  # mengning.com.cn
-    "github.com",
-] + __registry_mirror_hosts__
-
-__configfile__ = "SuperIDE.ini"
-
-__container_engine__ = "isula"
-
+# Copyright (c) Mengning Software. 2023. All rights reserved.
+#
+# Super IDE licensed under GNU Affero General Public License v3 (AGPL-3.0) .
+# You can use this software according to the terms and conditions of the AGPL-3.0.
+# You may obtain a copy of AGPL-3.0 at:
+#
+#    https://www.gnu.org/licenses/agpl-3.0.txt
+#
+# THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
+# PURPOSE.
+# See the AGPL-3.0 for more details.
+
+VERSION = (1, 5, 0)
+__version__ = ".".join([str(s) for s in VERSION])
+
+__title__ = "super-ide"
+__description__ = (
+    "A professional Cross-platform IDE. "
+    "Cross-platform IDE and Unified Debugger. "
+    "Static Code Analyzer and Remote Unit Testing. "
+    "Multi-platform and Multi-architecture Build System. "
+    "Firmware File Explorer and Memory Inspection. "
+    "IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, "
+    "STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, "
+    "MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, "
+    "STMicroelectronics (STM8/STM32), Teensy"
+)
+__url__ = "https://mengning.com.cn"
+
+__author__ = "Mengning Software"
+__email__ = "contact@mengning.com.cn"
+
+__license__ = "AGPL-3.0 License"
+__copyright__ = "Copyright 2014-present Mengning Software"
+
+__accounts_api__ = "https://api.accounts.mengning.com.cn"
+__registry_mirror_hosts__ = [
+    "registry.mengning.com.cn",
+    "registry.nm1.mengning.com.cn",
+]
+__pioremote_endpoint__ = "ssl:host=remote.mengning.com.cn:port=4413"
+
+__core_packages__ = {
+    "tool-scons": "~4.40502.0",
+    "tool-cppcheck": "~1.270.0",
+    "tool-clangtidy": "~1.150005.0",
+    "tool-pvs-studio": "~7.18.0",
+}
+
+__check_internet_hosts__ = [
+    "185.199.110.153",  # Github.com
+    "88.198.170.159",  # mengning.com.cn
+    "github.com",
+] + __registry_mirror_hosts__
+
+__configfile__ = "SuperIDE.ini"
+
+__container_engine__ = "docker"
+
```

### Comparing `super-ide-1.4.8/superide/__main__.py` & `super-ide-1.5.0/superide/__main__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/app.py` & `super-ide-1.5.0/superide/app.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/boards/cli.py` & `super-ide-1.5.0/superide/boards/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/cache.py` & `super-ide-1.5.0/superide/cache.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/cli.py` & `super-ide-1.5.0/superide/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/compat.py` & `super-ide-1.5.0/superide/compat.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/debug/__init__.py` & `super-ide-1.5.0/superide/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/debug/cli.py` & `super-ide-1.5.0/superide/project/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,184 +1,197 @@
-# Copyright (c) 2014-present PlatformIO <contact@platformio.org>
+# Copyright (c) Mengning Software. 2023. All rights reserved.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+# Super IDE licensed under GNU Affero General Public License v3 (AGPL-3.0) .
+# You can use this software according to the terms and conditions of the AGPL-3.0.
+# You may obtain a copy of AGPL-3.0 at:
 #
-#    http://www.apache.org/licenses/LICENSE-2.0
+#    https://www.gnu.org/licenses/agpl-3.0.txt
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
+# PURPOSE.
+# See the AGPL-3.0 for more details.
 
-# pylint: disable=too-many-arguments, too-many-locals
-# pylint: disable=too-many-branches, too-many-statements
-
-import asyncio
 import os
-import signal
+import re
 import subprocess
+from hashlib import sha1
 
-import click
+from click.testing import CliRunner
 
-from superide import app, exception, fs, proc
-from superide.compat import IS_WINDOWS
-from superide.debug import helpers
-from superide.debug.config.factory import DebugConfigFactory
-from superide.debug.exception import DebugInvalidOptionsError
-from superide.debug.process.gdb import GDBClientProcess
-from superide.exception import ReturnErrorCode
-# from superide.platform.factory import PlatformFactory
+from superide import __configfile__
+from superide import __version__, exception, fs
+from superide.compat import IS_MACOS, IS_WINDOWS, hashlib_encode_data
 from superide.project.config import ProjectConfig
-from superide.project.helpers import is_platformio_project
-from superide.project.options import ProjectOptions
-
 
-@click.command(
-    "debug",
-    context_settings=dict(ignore_unknown_options=True),
-    short_help="Unified Debugger",
-)
-@click.option(
-    "-d",
-    "--project-dir",
-    default=os.getcwd,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, writable=True),
-)
-@click.option(
-    "-c",
-    "--project-conf",
-    type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True),
-)
-@click.option("--environment", "-e", metavar="<environment>")
-@click.option("--load-mode", type=ProjectOptions["env.debug_load_mode"].type)
-@click.option("--verbose", "-v", is_flag=True)
-@click.option("--interface", type=click.Choice(["gdb"]))
-@click.argument("client_extra_args", nargs=-1, type=click.UNPROCESSED)
-@click.pass_context
-def cli(
-    ctx,
-    project_dir,
-    project_conf,
-    environment,
-    load_mode,
-    verbose,
-    interface,
-    client_extra_args,
-):
-    app.set_session_var("custom_project_conf", project_conf)
-
-    if not interface and client_extra_args:
-        raise click.UsageError("Please specify debugging interface")
-
-    # use env variables from Eclipse or CLion
-    for name in ("CWD", "PWD", "PLATFORMIO_PROJECT_DIR"):
-        if is_platformio_project(project_dir):
-            break
-        if os.getenv(name):
-            project_dir = os.getenv(name)
 
-    with fs.cd(project_dir):
-        project_config = ProjectConfig.get_instance(project_conf)
-        project_config.validate(envs=[environment] if environment else None)
-        env_name = environment or helpers.get_default_debug_env(project_config)
-
-        if not interface:
-            return helpers.predebug_project(
-                ctx, project_dir, project_config, env_name, False, verbose
-            )
-
-        configure_args = (
-            ctx,
-            project_config,
-            env_name,
-            load_mode,
-            verbose,
-            client_extra_args,
-        )
-        if helpers.is_gdbmi_mode():
-            os.environ["PLATFORMIO_DISABLE_PROGRESSBAR"] = "true"
-            stream = helpers.GDBMIConsoleStream()
-            with proc.capture_std_streams(stream):
-                debug_config = _configure(*configure_args)
-            stream.close()
-        else:
-            debug_config = _configure(*configure_args)
+def get_project_dir():
+    return os.getcwd()
 
-        _run(project_dir, debug_config, client_extra_args)
 
+def is_platformio_project(project_dir=None):
+    if not project_dir:
+        project_dir = get_project_dir()
+    return os.path.isfile(os.path.join(project_dir, __configfile__))
+
+
+def find_project_dir_above(path):
+    if os.path.isfile(path):
+        path = os.path.dirname(path)
+    if is_platformio_project(path):
+        return path
+    if os.path.isdir(os.path.dirname(path)):
+        return find_project_dir_above(os.path.dirname(path))
     return None
 
 
-def _configure(ctx, project_config, env_name, load_mode, verbose, client_extra_args):
-    # platform = PlatformFactory.from_env(env_name, autoinstall=True)
-    platform = None
-    debug_config = DebugConfigFactory.new(
-        platform,
-        project_config,
-        env_name,
-    )
-    if "--version" in client_extra_args:
-        raise ReturnErrorCode(
-            subprocess.run(
-                [debug_config.client_executable_path, "--version"], check=True
-            ).returncode
-        )
+def get_project_watch_lib_dirs():
+    """Used by superide-node-helpers.project.observer.fetchLibDirs"""
+    config = ProjectConfig.get_instance()
+    result = [
+        config.get("superide", "globallib_dir"),
+        config.get("superide", "lib_dir"),
+    ]
+    libdeps_dir = config.get("superide", "libdeps_dir")
+    if not os.path.isdir(libdeps_dir):
+        return result
+    for d in os.listdir(libdeps_dir):
+        if os.path.isdir(os.path.join(libdeps_dir, d)):
+            result.append(os.path.join(libdeps_dir, d))
+    return result
+
+
+get_project_all_lib_dirs = get_project_watch_lib_dirs
+
+
+def get_project_cache_dir():
+    """Deprecated, use ProjectConfig.get("superide", "cache_dir") instead"""
+    return ProjectConfig.get_instance().get("superide", "cache_dir")
 
-    try:
-        fs.ensure_udev_rules()
-    except exception.InvalidUdevRules as exc:
-        click.echo(str(exc))
-
-    rebuild_prog = False
-    preload = debug_config.load_cmds == ["preload"]
-    load_mode = load_mode or debug_config.load_mode
-    if load_mode == "always":
-        rebuild_prog = preload or not helpers.has_debug_symbols(
-            debug_config.program_path
-        )
-    elif load_mode == "modified":
-        rebuild_prog = helpers.is_prog_obsolete(
-            debug_config.program_path
-        ) or not helpers.has_debug_symbols(debug_config.program_path)
-
-    if not (debug_config.program_path and os.path.isfile(debug_config.program_path)):
-        rebuild_prog = True
-
-    if preload or (not rebuild_prog and load_mode != "always"):
-        # don't load firmware through debug server
-        debug_config.load_cmds = []
-
-    if rebuild_prog:
-        click.echo("Preparing firmware for debugging...")
-        helpers.predebug_project(
-            ctx, os.getcwd(), project_config, env_name, preload, verbose
-        )
-        # save SHA sum of newly created prog
-        if load_mode == "modified":
-            helpers.is_prog_obsolete(debug_config.program_path)
-
-    if not os.path.isfile(debug_config.program_path):
-        raise DebugInvalidOptionsError("Program/firmware is missed")
 
-    return debug_config
+def get_default_projects_dir():
+    docs_dir = os.path.join(fs.expanduser("~"), "Documents")
+    try:
+        assert IS_WINDOWS
+        import ctypes.wintypes  # pylint: disable=import-outside-toplevel
 
+        buf = ctypes.create_unicode_buffer(ctypes.wintypes.MAX_PATH)
+        ctypes.windll.shell32.SHGetFolderPathW(None, 5, None, 0, buf)
+        docs_dir = buf.value
+    except:  # pylint: disable=bare-except
+        if not IS_MACOS:
+            try:
+                docs_dir = (
+                    subprocess.check_output(["xdg-user-dir", "DOCUMENTS"])
+                    .decode("utf-8")
+                    .strip()
+                )
+            except FileNotFoundError:  # command not found
+                pass
+    return os.path.join(docs_dir, "superide", "Projects")
+
+
+def compute_project_checksum(config):
+    # rebuild when PIO Core version changes
+    checksum = sha1(hashlib_encode_data(__version__))
+
+    # configuration file state
+    config_data = config.to_json()
+    if IS_WINDOWS:
+        # issue #4600: fix drive letter
+        config_data = re.sub(
+            r"([A-Z]):\\",
+            lambda match: "%s:\\" % match.group(1).lower(),
+            config_data,
+            flags=re.I,
+        )
+    checksum.update(hashlib_encode_data(config_data))
 
-def _run(project_dir, debug_config, client_extra_args):
-    loop = asyncio.ProactorEventLoop() if IS_WINDOWS else asyncio.get_event_loop()
-    asyncio.set_event_loop(loop)
+    # project file structure
+    check_suffixes = (".c", ".cc", ".cpp", ".h", ".hpp", ".s", ".S")
+    for d in (
+        config.get("superide", "include_dir"),
+        config.get("superide", "src_dir"),
+        config.get("superide", "lib_dir"),
+    ):
+        if not os.path.isdir(d):
+            continue
+        chunks = []
+        for root, _, files in os.walk(d):
+            for f in files:
+                path = os.path.join(root, f)
+                if path.endswith(check_suffixes):
+                    chunks.append(path)
+        if not chunks:
+            continue
+        chunks_to_str = ",".join(sorted(chunks))
+        if IS_WINDOWS:  # case insensitive OS
+            chunks_to_str = chunks_to_str.lower()
+        checksum.update(hashlib_encode_data(chunks_to_str))
+
+    return checksum.hexdigest()
+
+
+def load_build_metadata(project_dir, env_or_envs, cache=False, debug=False):
+    assert env_or_envs
+    env_names = env_or_envs
+    if not isinstance(env_names, list):
+        env_names = [env_names]
 
-    client = GDBClientProcess(project_dir, debug_config)
-    coro = client.run(client_extra_args)
-    try:
-        signal.signal(signal.SIGINT, signal.SIG_IGN)
-        loop.run_until_complete(coro)
-        if IS_WINDOWS:
-            client.close()
-            # an issue with `asyncio` executor and STIDIN,
-            # it cannot be closed gracefully
-            proc.force_exit()
-    finally:
-        client.close()
-        loop.close()
+    with fs.cd(project_dir):
+        result = _get_cached_build_metadata(project_dir, env_names) if cache else {}
+        # incompatible build-type data
+        for name in list(result.keys()):
+            build_type = result[name].get("build_type", "")
+            outdated_conds = [
+                not build_type,
+                debug and "debug" not in build_type,
+                not debug and "debug" in build_type,
+            ]
+            if any(outdated_conds):
+                del result[name]
+        missed_env_names = set(env_names) - set(result.keys())
+        if missed_env_names:
+            result.update(_load_build_metadata(project_dir, missed_env_names, debug))
+
+    if not isinstance(env_or_envs, list) and env_or_envs in result:
+        return result[env_or_envs]
+    return result or None
+
+
+# Backward compatibiility with dev-platforms
+load_project_ide_data = load_build_metadata
+
+
+def _load_build_metadata(project_dir, env_names, debug=False):
+    # pylint: disable=import-outside-toplevel
+    from superide import app
+    from superide.run.cli import cli as cmd_run
+
+    args = ["--project-dir", project_dir, "--target", "__idedata"]
+    if debug:
+        args.extend(["--target", "__debug"])
+    for name in env_names:
+        args.extend(["-e", name])
+    # 此处需要运行superide run命令编译
+    # app.set_session_var("pause_telemetry", True)
+    # result = CliRunner().invoke(cmd_run, args)
+    # app.set_session_var("pause_telemetry", False)
+    # if result.exit_code != 0 and not isinstance(
+    #     result.exception, exception.ReturnErrorCode
+    # ):
+    #     raise result.exception
+    # if '"includes":' not in result.output:
+    #     raise exception.UserSideException(result.output)
+    return _get_cached_build_metadata(project_dir, env_names)
+
+
+def _get_cached_build_metadata(project_dir, env_names):
+    build_dir = ProjectConfig.get_instance(
+        os.path.join(project_dir, __configfile__)
+    ).get("superide", "build_dir")
+    result = {}
+    for name in env_names:
+        if not os.path.isfile(os.path.join(build_dir, name, "idedata.json")):
+            continue
+        result[name] = fs.load_json(os.path.join(build_dir, name, "idedata.json"))
+    return result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `super-ide-1.4.8/superide/debug/config/__init__.py` & `super-ide-1.5.0/superide/debug/process/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/debug/config/base.py` & `super-ide-1.5.0/superide/debug/config/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# Copyright (c) 2014-present PlatformIO <contact@platformio.org>
+# Copyright (c) Mengning Software. 2023. All rights reserved.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+# Super IDE licensed under GNU Affero General Public License v3 (AGPL-3.0) .
+# You can use this software according to the terms and conditions of the AGPL-3.0.
+# You may obtain a copy of AGPL-3.0 at:
 #
-#    http://www.apache.org/licenses/LICENSE-2.0
+#    https://www.gnu.org/licenses/agpl-3.0.txt
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
+# PURPOSE.
+# See the AGPL-3.0 for more details.
 
 import json
 import os
 
 from superide import fs, proc, util
 from superide.compat import string_types
 from superide.debug.exception import DebugInvalidOptionsError
```

### Comparing `super-ide-1.4.8/superide/debug/config/blackmagic.py` & `super-ide-1.5.0/superide/debug/config/blackmagic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-# Copyright (c) 2014-present PlatformIO <contact@platformio.org>
+# Copyright (c) Mengning Software. 2023. All rights reserved.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+# Super IDE licensed under GNU Affero General Public License v3 (AGPL-3.0) .
+# You can use this software according to the terms and conditions of the AGPL-3.0.
+# You may obtain a copy of AGPL-3.0 at:
 #
-#    http://www.apache.org/licenses/LICENSE-2.0
+#    https://www.gnu.org/licenses/agpl-3.0.txt
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
+# PURPOSE.
+# See the AGPL-3.0 for more details.
 
 from superide.debug.config.base import DebugConfigBase
 from superide.debug.exception import DebugInvalidOptionsError
 from superide.device.finder import SerialPortFinder, is_pattern_port
 
 
 class BlackmagicDebugConfig(DebugConfigBase):
     GDB_INIT_SCRIPT = """
-define pio_reset_halt_target
+define si_reset_halt_target
     set language c
     set *0xE000ED0C = 0x05FA0004
     set $busy = (*0xE000ED0C & 0x4)
     while ($busy)
         set $busy = (*0xE000ED0C & 0x4)
     end
     set language auto
 end
 
-define pio_reset_run_target
-    pio_reset_halt_target
+define si_reset_run_target
+    si_reset_halt_target
 end
 
 target extended-remote $DEBUG_PORT
 monitor swdp_scan
 attach 1
 set mem inaccessible-by-default off
 $LOAD_CMDS
```

### Comparing `super-ide-1.4.8/superide/debug/config/factory.py` & `super-ide-1.5.0/superide/debug/config/factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# Copyright (c) 2014-present PlatformIO <contact@platformio.org>
+# Copyright (c) Mengning Software. 2023. All rights reserved.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+# Super IDE licensed under GNU Affero General Public License v3 (AGPL-3.0) .
+# You can use this software according to the terms and conditions of the AGPL-3.0.
+# You may obtain a copy of AGPL-3.0 at:
 #
-#    http://www.apache.org/licenses/LICENSE-2.0
+#    https://www.gnu.org/licenses/agpl-3.0.txt
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
+# PURPOSE.
+# See the AGPL-3.0 for more details.
 
 import importlib
 import re
 
 from superide.debug.config.generic import GenericDebugConfig
 from superide.debug.config.native import NativeDebugConfig
 
@@ -23,21 +22,22 @@
     @staticmethod
     def get_clsname(name):
         name = re.sub(r"[^\da-z\_\-]+", "", name, flags=re.I)
         return "%sDebugConfig" % name.lower().capitalize()
 
     @classmethod
     def new(cls, platform, project_config, env_name):
-        board_id = project_config.get("env:" + env_name, "board")
+        #board_id = project_config.get("env:" + env_name, "board")
         config_cls = None
         tool_name = None
-        if board_id:
-            tool_name = platform.board_config(
-                project_config.get("env:" + env_name, "board")
-            ).get_debug_tool_name(project_config.get("env:" + env_name, "debug_tool"))
+
+        tool_name = project_config.get("env:" + env_name, "debug_tool")
+        #if board_id:
+            #tool_name = platform.board_config(
+            #).get_debug_tool_name(project_config.get("env:" + env_name, "debug_tool"))
         try:
             mod = importlib.import_module("superide.debug.config.%s" % tool_name)
             config_cls = getattr(mod, cls.get_clsname(tool_name))
         except ModuleNotFoundError:
             config_cls = (
                 GenericDebugConfig #platform.is_embedded() else NativeDebugConfig
             )
```

### Comparing `super-ide-1.4.8/superide/debug/config/generic.py` & `super-ide-1.5.0/superide/debug/config/generic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# Copyright (c) 2014-present PlatformIO <contact@platformio.org>
+# Copyright (c) Mengning Software. 2023. All rights reserved.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+# Super IDE licensed under GNU Affero General Public License v3 (AGPL-3.0) .
+# You can use this software according to the terms and conditions of the AGPL-3.0.
+# You may obtain a copy of AGPL-3.0 at:
 #
-#    http://www.apache.org/licenses/LICENSE-2.0
+#    https://www.gnu.org/licenses/agpl-3.0.txt
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
+# PURPOSE.
+# See the AGPL-3.0 for more details.
 
 from superide.debug.config.base import DebugConfigBase
 
 
 class GenericDebugConfig(DebugConfigBase):
     DEFAULT_PORT = ":3333"
     GDB_INIT_SCRIPT = """
-define pio_reset_halt_target
+define si_reset_halt_target
     monitor reset halt
 end
 
-define pio_reset_run_target
+define si_reset_run_target
     monitor reset
 end
 
 target extended-remote $DEBUG_PORT
 monitor init
 $LOAD_CMDS
-pio_reset_halt_target
+si_reset_halt_target
 $INIT_BREAK
 """
```

### Comparing `super-ide-1.4.8/superide/debug/exception.py` & `super-ide-1.5.0/superide/debug/exception.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/debug/helpers.py` & `super-ide-1.5.0/superide/debug/helpers.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/debug/process/base.py` & `super-ide-1.5.0/superide/debug/process/base.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/debug/process/client.py` & `super-ide-1.5.0/superide/debug/process/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         self._server_process = None
         self._session_id = None
 
         if not os.path.isdir(get_project_cache_dir()):
             os.makedirs(get_project_cache_dir())
         self.working_dir = tempfile.mkdtemp(
-            dir=get_project_cache_dir(), prefix=".piodebug-"
+            dir=get_project_cache_dir(), prefix=".sidebug-"
         )
 
         self._target_is_running = False
         self._errors_buffer = b""
 
     async def run(self):
         session_hash = (
```

### Comparing `super-ide-1.4.8/superide/debug/process/gdb.py` & `super-ide-1.5.0/superide/debug/process/gdb.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,185 +1,193 @@
-# Copyright (c) 2014-present PlatformIO <contact@platformio.org>
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import os
-import signal
-import time
-
-from superide import telemetry
-from superide.compat import aio_get_running_loop, is_bytes
-from superide.debug import helpers
-from superide.debug.exception import DebugInitError
-from superide.debug.process.client import DebugClientProcess
-
-
-class GDBClientProcess(DebugClientProcess):
-    PIO_SRC_NAME = ".pioinit"
-    INIT_COMPLETED_BANNER = "PlatformIO: Initialization completed"
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._target_is_running = False
-        self._errors_buffer = b""
-
-    async def run(self, extra_args):  # pylint: disable=arguments-differ
-        await super().run()
-
-        self.generate_init_script(os.path.join(self.working_dir, self.PIO_SRC_NAME))
-        gdb_path = self.debug_config.client_executable_path or "docker"
-        # start GDB client
-        args = [
-            gdb_path,
-            'exec',
-            '-i',
-            'boring_cray',
-            'gdb-multiarch',
-            '-q',
-            '--interpreter=mi2',
-            "--directory",
-            self.project_dir,
-            "-l",
-            "10",
-        ]
-        args.extend(list(extra_args or []))
-        gdb_data_dir = self._get_data_dir(gdb_path)
-        if gdb_data_dir:
-            args.extend(["--data-directory", gdb_data_dir])
-        args.append(self.debug_config.program_path)
-
-        await self.spawn(*args, cwd=self.project_dir, wait_until_exit=True)
-
-    @staticmethod
-    def _get_data_dir(gdb_path):
-        if "msp430" in gdb_path:
-            return None
-        gdb_data_dir = os.path.abspath(
-            os.path.join(os.path.dirname(gdb_path), "..", "share", "gdb")
-        )
-        return gdb_data_dir if os.path.isdir(gdb_data_dir) else None
-
-    def generate_init_script(self, dst):
-        # default GDB init commands depending on debug tool
-        commands = self.debug_config.get_init_script("gdb").split("\n")
-
-        if self.debug_config.init_cmds:
-            commands = self.debug_config.init_cmds
-        commands.extend(self.debug_config.extra_cmds)
-
-        if not any("define pio_reset_run_target" in cmd for cmd in commands):
-            commands = [
-                "define pio_reset_run_target",
-                "   echo Warning! Undefined pio_reset_run_target command\\n",
-                "   monitor reset",
-                "end",
-            ] + commands
-        if not any("define pio_reset_halt_target" in cmd for cmd in commands):
-            commands = [
-                "define pio_reset_halt_target",
-                "   echo Warning! Undefined pio_reset_halt_target command\\n",
-                "   monitor reset halt",
-                "end",
-            ] + commands
-        if not any("define pio_restart_target" in cmd for cmd in commands):
-            commands += [
-                "define pio_restart_target",
-                "   pio_reset_halt_target",
-                "   $INIT_BREAK",
-                "   %s" % ("continue" if self.debug_config.init_break else "next"),
-                "end",
-            ]
-
-        banner = [
-            "echo PlatformIO Unified Debugger -> https://bit.ly/pio-debug\\n",
-            "echo PlatformIO: debug_tool = %s\\n" % self.debug_config.tool_name,
-            "echo PlatformIO: Initializing remote target...\\n",
-        ]
-        footer = ["echo %s\\n" % self.INIT_COMPLETED_BANNER]
-        commands = banner + commands + footer
-
-        with open(dst, mode="w", encoding="utf8") as fp:
-            fp.write("\n".join(self.debug_config.reveal_patterns(commands)))
-
-    def stdin_data_received(self, data):
-        super().stdin_data_received(data)
-        if b"-exec-run" in data:
-            if self._target_is_running:
-                token, _ = data.split(b"-", 1)
-                self.stdout_data_received(token + b"^running\n")
-                return
-            # config和platform部分代码停用
-            # if self.debug_config.platform.is_embedded():
-            #     data = data.replace(b"-exec-run", b"-exec-continue")
-
-        if b"-exec-continue" in data:
-            self._target_is_running = True
-        if b"-gdb-exit" in data or data.strip() in (b"q", b"quit"):
-            # Allow terminating via SIGINT/CTRL+C
-            signal.signal(signal.SIGINT, signal.default_int_handler)
-            self.transport.get_pipe_transport(0).write(b"pio_reset_run_target\n")
-        self.transport.get_pipe_transport(0).write(data)
-
-    def stdout_data_received(self, data):
-        super().stdout_data_received(data)
-        self._handle_error(data)
-        # go to init break automatically
-        if self.INIT_COMPLETED_BANNER.encode() in data:
-            telemetry.log_debug_started(self.debug_config)
-            self._auto_exec_continue()
-
-    def console_log(self, msg):
-        if helpers.is_gdbmi_mode():
-            msg = helpers.escape_gdbmi_stream("~", msg)
-        self.stdout_data_received(msg if is_bytes(msg) else msg.encode())
-
-    def _auto_exec_continue(self):
-        auto_exec_delay = 0.5  # in seconds
-        if self._last_activity > (time.time() - auto_exec_delay):
-            aio_get_running_loop().call_later(0.1, self._auto_exec_continue)
-            return
-
-        if not self.debug_config.init_break or self._target_is_running:
-            return
-
-        self.console_log(
-            "PlatformIO: Resume the execution to `debug_init_break = %s`\n"
-            % self.debug_config.init_break
-        )
-        self.console_log(
-            "PlatformIO: More configuration options -> https://bit.ly/pio-debug\n"
-        )
-        if self.debug_config.platform.is_embedded():
-            self.transport.get_pipe_transport(0).write(
-                b"0-exec-continue\n" if helpers.is_gdbmi_mode() else b"continue\n"
-            )
-        else:
-            self.transport.get_pipe_transport(0).write(
-                b"0-exec-run\n" if helpers.is_gdbmi_mode() else b"run\n"
-            )
-        self._target_is_running = True
-
-    def stderr_data_received(self, data):
-        super().stderr_data_received(data)
-        self._handle_error(data)
-
-    def _handle_error(self, data):
-        self._errors_buffer = (self._errors_buffer + data)[-8192:]  # keep last 8 KBytes
-        if not (
-            self.PIO_SRC_NAME.encode() in self._errors_buffer
-            and b"Error in sourced" in self._errors_buffer
-        ):
-            return
-        telemetry.log_debug_exception(
-            DebugInitError(self._errors_buffer.decode()), self.debug_config
-        )
-        self.transport.close()
+# Copyright (c) Mengning Software. 2023. All rights reserved.
+#
+# Super IDE licensed under GNU Affero General Public License v3 (AGPL-3.0) .
+# You can use this software according to the terms and conditions of the AGPL-3.0.
+# You may obtain a copy of AGPL-3.0 at:
+#
+#    https://www.gnu.org/licenses/agpl-3.0.txt
+#
+# THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
+# PURPOSE.
+# See the AGPL-3.0 for more details.
+
+import os
+import signal
+import time
+
+from superide import telemetry
+from superide.compat import aio_get_running_loop, is_bytes
+from superide.debug import helpers
+from superide.debug.exception import DebugInitError
+from superide.debug.process.client import DebugClientProcess
+
+
+class GDBClientProcess(DebugClientProcess):
+    SI_SRC_NAME = ".gdbinit"
+    INIT_COMPLETED_BANNER = "Super IDE: Initialization completed"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._target_is_running = False
+        self._errors_buffer = b""
+
+    async def run(self, extra_args):  # pylint: disable=arguments-differ
+        await super().run()
+        # working_dir目前在.superide目录下，目前docker不挂载，这里把生成的.gdbinit文件放到项目目录下
+        self.generate_init_script(os.path.join(self.project_dir, self.SI_SRC_NAME))
+        gdb_path = "docker"
+        # start GDB client
+        args = [
+            gdb_path,
+            'run',
+            '-i',
+            '--rm',
+            '--network', 
+            'host',
+            '-v',
+            self.project_dir+':'+self.project_dir,
+            'denkchan/test:latest',
+            'gdb-multiarch',
+            '-q',
+            '--interpreter=mi2',
+            "--directory",
+            self.project_dir,
+            "-l",
+            "10",
+            "-x",
+            os.path.join(self.project_dir, self.SI_SRC_NAME),
+        ]
+        args.extend(list(extra_args or []))
+        gdb_data_dir = self._get_data_dir(gdb_path)
+        if gdb_data_dir:
+            args.extend(["--data-directory", gdb_data_dir])
+        args.append(self.debug_config.program_path)
+
+        await self.spawn(*args, cwd=self.project_dir, wait_until_exit=True)
+
+    @staticmethod
+    def _get_data_dir(gdb_path):
+        if "msp430" in gdb_path:
+            return None
+        gdb_data_dir = os.path.abspath(
+            os.path.join(os.path.dirname(gdb_path), "..", "share", "gdb")
+        )
+        return gdb_data_dir if os.path.isdir(gdb_data_dir) else None
+
+    def generate_init_script(self, dst):
+        # default GDB init commands depending on debug tool
+        commands = self.debug_config.get_init_script("gdb").split("\n")
+
+        if self.debug_config.init_cmds:
+            commands = self.debug_config.init_cmds
+        commands.extend(self.debug_config.extra_cmds)
+
+        if not any("define si_reset_run_target" in cmd for cmd in commands):
+            commands = [
+                "define si_reset_run_target",
+                "   echo Warning! Undefined si_reset_run_target command\\n",
+                "   monitor reset",
+                "end",
+            ] + commands
+        if not any("define si_reset_halt_target" in cmd for cmd in commands):
+            commands = [
+                "define si_reset_halt_target",
+                "   echo Warning! Undefined si_reset_halt_target command\\n",
+                "   monitor reset halt",
+                "end",
+            ] + commands
+        if not any("define si_restart_target" in cmd for cmd in commands):
+            commands += [
+                "define si_restart_target",
+                "   si_reset_halt_target",
+                "   $INIT_BREAK",
+                "   %s" % ("continue" if self.debug_config.init_break else "next"),
+                "end",
+            ]
+
+        banner = [
+            "echo Super IDE Unified Debugger -> https://\\n",
+            "echo Super IDE: debug_tool = %s\\n" % self.debug_config.tool_name,
+            "echo Super IDE: Initializing remote target...\\n",
+        ]
+        footer = ["echo %s\\n" % self.INIT_COMPLETED_BANNER]
+        commands = banner + commands + footer
+
+        with open(dst, mode="w", encoding="utf8") as fp:
+            fp.write("\n".join(self.debug_config.reveal_patterns(commands)))
+
+    def stdin_data_received(self, data):
+        super().stdin_data_received(data)
+        if b"-exec-run" in data:
+            if self._target_is_running:
+                token, _ = data.split(b"-", 1)
+                self.stdout_data_received(token + b"^running\n")
+                return
+            # config和platform部分代码停用
+            # if self.debug_config.platform.is_embedded():
+            #     data = data.replace(b"-exec-run", b"-exec-continue")
+
+        if b"-exec-continue" in data:
+            self._target_is_running = True
+        if b"-gdb-exit" in data or data.strip() in (b"q", b"quit"):
+            # Allow terminating via SIGINT/CTRL+C
+            signal.signal(signal.SIGINT, signal.default_int_handler)
+            self.transport.get_pipe_transport(0).write(b"si_reset_run_target\n")
+        self.transport.get_pipe_transport(0).write(data)
+
+    def stdout_data_received(self, data):
+        super().stdout_data_received(data)
+        self._handle_error(data)
+        # go to init break automatically
+        if self.INIT_COMPLETED_BANNER.encode() in data:
+            telemetry.log_debug_started(self.debug_config)
+            self._auto_exec_continue()
+
+    def console_log(self, msg):
+        if helpers.is_gdbmi_mode():
+            msg = helpers.escape_gdbmi_stream("~", msg)
+        self.stdout_data_received(msg if is_bytes(msg) else msg.encode())
+
+    def _auto_exec_continue(self):
+        auto_exec_delay = 0.5  # in seconds
+        if self._last_activity > (time.time() - auto_exec_delay):
+            aio_get_running_loop().call_later(0.1, self._auto_exec_continue)
+            return
+
+        if not self.debug_config.init_break or self._target_is_running:
+            return
+
+        self.console_log(
+            "Super IDE: Resume the execution to `debug_init_break = %s`\n"
+            % self.debug_config.init_break
+        )
+        self.console_log(
+            "Super IDE: More configuration options -> https://\n"
+        )
+        # 根据是否是嵌入式程序和mi模式确定不同的启动指令
+        # TODO：目前代码没有platform类，需要在ini增加字段或其他处理
+        # if self.debug_config.platform.is_embedded():
+        # self.transport.get_pipe_transport(0).write(
+        #          b"0-exec-continue\n" if helpers.is_gdbmi_mode() else b"continue\n"
+        #      )
+        # else:
+        #     self.transport.get_pipe_transport(0).write(
+        #         b"0-exec-run\n" if helpers.is_gdbmi_mode() else b"run\n"
+        #     )
+        self._target_is_running = True
+
+    def stderr_data_received(self, data):
+        super().stderr_data_received(data)
+        self._handle_error(data)
+
+    def _handle_error(self, data):
+        self._errors_buffer = (self._errors_buffer + data)[-8192:]  # keep last 8 KBytes
+        if not (
+            self.SI_SRC_NAME.encode() in self._errors_buffer
+            and b"Error in sourced" in self._errors_buffer
+        ):
+            return
+        telemetry.log_debug_exception(
+            DebugInitError(self._errors_buffer.decode()), self.debug_config
+        )
+        self.transport.close()
```

### Comparing `super-ide-1.4.8/superide/debug/process/server.py` & `super-ide-1.5.0/superide/debug/process/server.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/exception.py` & `super-ide-1.5.0/superide/exception.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/fs.py` & `super-ide-1.5.0/superide/fs.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/__init__.py` & `super-ide-1.5.0/superide/home/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/app.py` & `super-ide-1.5.0/superide/home/app.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/cli.py` & `super-ide-1.5.0/superide/home/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/rpc/handlers/__init__.py` & `super-ide-1.5.0/superide/home/rpc/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/rpc/handlers/app.py` & `super-ide-1.5.0/superide/home/rpc/handlers/app.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/rpc/handlers/base.py` & `super-ide-1.5.0/superide/home/rpc/handlers/base.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/rpc/handlers/ide.py` & `super-ide-1.5.0/superide/home/rpc/handlers/ide.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/rpc/handlers/os.py` & `super-ide-1.5.0/superide/home/rpc/handlers/os.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/rpc/handlers/project.py` & `super-ide-1.5.0/superide/home/rpc/handlers/project.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/rpc/handlers/registry.py` & `super-ide-1.5.0/superide/home/rpc/handlers/registry.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/runServer.py` & `super-ide-1.5.0/superide/home/runServer.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/static/assets/favicon.ico` & `super-ide-1.5.0/superide/home/static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/static/assets/index-6fed80ed.css` & `super-ide-1.5.0/superide/home/static/assets/index-6fed80ed.css`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/static/assets/index-d2bbbc6e.js` & `super-ide-1.5.0/superide/home/static/assets/index-d2bbbc6e.js`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/home/static/index.html` & `super-ide-1.5.0/superide/home/static/index.html`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/http.py` & `super-ide-1.5.0/superide/http.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/lockfile.py` & `super-ide-1.5.0/superide/lockfile.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/maintenance.py` & `super-ide-1.5.0/superide/maintenance.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/proc.py` & `super-ide-1.5.0/superide/proc.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/__init__.py` & `super-ide-1.5.0/superide/project/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/cli.py` & `super-ide-1.5.0/superide/project/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/commands/__init__.py` & `super-ide-1.5.0/superide/project/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/commands/config.py` & `super-ide-1.5.0/superide/project/commands/config.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/commands/init.py` & `super-ide-1.5.0/superide/project/commands/init.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/commands/metadata.py` & `super-ide-1.5.0/superide/project/commands/metadata.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/config.py` & `super-ide-1.5.0/superide/project/config.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/exception.py` & `super-ide-1.5.0/superide/project/exception.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/options.py` & `super-ide-1.5.0/superide/project/options.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/savedeps.py` & `super-ide-1.5.0/superide/project/savedeps.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/project/vcsclient.py` & `super-ide-1.5.0/superide/project/vcsclient.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/public.py` & `super-ide-1.5.0/superide/public.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/registry/__init__.py` & `super-ide-1.5.0/superide/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/registry/cli.py` & `super-ide-1.5.0/superide/registry/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/registry/client.py` & `super-ide-1.5.0/superide/registry/client.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/registry/mirror.py` & `super-ide-1.5.0/superide/registry/mirror.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/run/__init__.py` & `super-ide-1.5.0/superide/run/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/run/cli.py` & `super-ide-1.5.0/superide/run/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/run/helpers.py` & `super-ide-1.5.0/superide/run/helpers.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/run/processor.py` & `super-ide-1.5.0/superide/run/processor.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/system/__init__.py` & `super-ide-1.5.0/superide/system/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/system/cli.py` & `super-ide-1.5.0/superide/system/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/system/commands/__init__.py` & `super-ide-1.5.0/superide/system/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/system/commands/completion.py` & `super-ide-1.5.0/superide/system/commands/completion.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/system/commands/info.py` & `super-ide-1.5.0/superide/system/commands/info.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/system/completion.py` & `super-ide-1.5.0/superide/system/completion.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/telemetry.py` & `super-ide-1.5.0/superide/telemetry.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import traceback
 from collections import deque
 
 import requests
 
 from superide import __title__, __version__, app, exception, fs, util
 from superide.cli import SuperIDECLI
-# from superide.debug.config.base import DebugConfigBase
+from superide.debug.config.base import DebugConfigBase
 from superide.http import HTTPSession, ensure_internet_on
 from superide.proc import is_ci
 
 KEEP_MAX_REPORTS = 100
 SEND_MAX_EVENTS = 25
 
 
@@ -214,16 +214,16 @@
     section = f"env:{env}"
     params = {
         option: config.get(section, option)
         for option in non_sensitive_data
         if config.has_option(section, option)
     }
     params["pid"] = app.get_project_id(os.path.dirname(config.path))
-    params["platform_name"] = platform.name
-    params["platform_version"] = platform.version
+    params["platform_name"] = None # platform.name
+    params["platform_version"] = None # platform.version
     return params
 
 
 def log_platform_run(platform, project_config, project_env, targets=None):
     params = dump_project_env_params(project_config, project_env, platform)
     if targets:
         params["targets"] = targets
@@ -271,42 +271,42 @@
         "traceback": trace,
         "cmd_args": sys.argv[1:],
         "is_fatal": is_fatal,
     }
     log_event("exception", params)
 
 
-# def log_debug_started(debug_config: DebugConfigBase):
-#     log_event(
-#         "debug_started",
-#         dump_project_env_params(
-#             debug_config.project_config, debug_config.env_name, debug_config.platform
-#         ),
-#     )
-
-
-# def log_debug_exception(exc, debug_config: DebugConfigBase):
-#     # cleanup sensitive information, such as paths
-#     description = fs.to_unix_path(str(exc))
-#     description = re.sub(
-#         r'(^|\s+|")(?:[a-z]\:)?((/[^"/]+)+)(\s+|"|$)',
-#         lambda m: " %s " % os.path.join(*m.group(2).split("/")[-2:]),
-#         description,
-#         re.I | re.M,
-#     )
-#     params = {
-#         "name": exc.__class__.__name__,
-#         "description": description.strip(),
-#     }
-#     params.update(
-#         dump_project_env_params(
-#             debug_config.project_config, debug_config.env_name, debug_config.platform
-#         )
-#     )
-#     log_event("debug_exception", params)
+def log_debug_started(debug_config: DebugConfigBase):
+    log_event(
+        "debug_started",
+        dump_project_env_params(
+            debug_config.project_config, debug_config.env_name, debug_config.platform
+        ),
+    )
+
+
+def log_debug_exception(exc, debug_config: DebugConfigBase):
+    # cleanup sensitive information, such as paths
+    description = fs.to_unix_path(str(exc))
+    description = re.sub(
+        r'(^|\s+|")(?:[a-z]\:)?((/[^"/]+)+)(\s+|"|$)',
+        lambda m: " %s " % os.path.join(*m.group(2).split("/")[-2:]),
+        description,
+        re.I | re.M,
+    )
+    params = {
+        "name": exc.__class__.__name__,
+        "description": description.strip(),
+    }
+    params.update(
+        dump_project_env_params(
+            debug_config.project_config, debug_config.env_name, debug_config.platform
+        )
+    )
+    log_event("debug_exception", params)
 
 
 @atexit.register
 def _finalize():
     timeout = 1000  # msec
     elapsed = 0
     telemetry = TelemetryLogger()
```

### Comparing `super-ide-1.4.8/superide/toolchain/__init__.py` & `super-ide-1.5.0/superide/toolchain/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/superide/toolchain/toolchain.py` & `super-ide-1.5.0/superide/toolchain/toolchain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import json
-import subprocess
-import os
-from superide import __container_engine__, exception
-
-class Toolchain:
-    check_image_flag = False
-
-    def __init__(self, image_name, project_directory):
-        check_container_engine_availability()
-        self.image_name = image_name
-        self.project_directory = project_directory
-        self.contain_project_directory = "/app/project"
-        self.check_image()
-        
-        
-    def check_image(self):
-        if(Toolchain.check_image_flag):
-            return
-        try:
-            print('check image...')
-            if(__container_engine__ == 'docker'):
-                output = subprocess.check_output(["docker", "images", "-q", self.image_name])
-                if output:
-                    Toolchain.check_image_flag = True
-                    return
-            subprocess.run([__container_engine__, 'pull', self.image_name], stderr=subprocess.DEVNULL)
-            Toolchain.check_image_flag = True
-        except subprocess.CalledProcessError:
-            raise exception.ImageNotGet()
-
-    def init_project(self):
-        # 文件夹非空则不能创建项目
-        if(len(os.listdir(self.project_directory)) != 0):
-            print("can't init project in Non empty folder")
-            raise exception.InitProjectError()
-        
-        source_path = '/app/ExampleProject/.'
-        destination_path = self.contain_project_directory
-        try:
-            command = [__container_engine__, "run","-it","--rm", "-v", self.project_directory+":"+self.contain_project_directory, self.image_name, 
-                       'cp', '-r', source_path, destination_path];
-            subprocess.run(command)
-        except Exception:
-            print("init project failed")
-            raise exception.InitProjectError()
-
-    def _get_tools(self):
-        with open(f'{self.project_directory}/.vscode/tasks.json') as file:
-            config = json.load(file)
-        for task in config['tasks']:
-            if task['label'] == 'Build':
-                self.build_task = task
-            if task['label'] == 'Check':
-                self.check_task = task
-            if task['label'] == 'Run':
-                self.run_task = task
-
-    def build(self):
-        self._get_tools()
-        build_command = self.build_task["command"]+ " " + " ".join(self.build_task["args"])
-        return self.container_command(build_command)
-
-    def check(self):
-        self._get_tools()
-        check_command = self.check_task["command"]+ " " + " ".join(self.check_task["args"])
-        return self.container_command(check_command)
-    
-    def run(self):
-        self._get_tools()
-        run_command = self.run_task["command"]+ " " + " ".join(self.run_task["args"])
-        return self.container_command(run_command)
-
-    def container_command(self, command):
-        return " ".join([__container_engine__, "run","-it","--rm", "-v", self.project_directory+":"+self.contain_project_directory, self.image_name, command])
-    
-
-def get_container_engine_path():
-    try:
-        path = subprocess.check_output(['which', __container_engine__]).decode().strip()
-        return path
-    except subprocess.CalledProcessError:
-        return None
-
-def check_container_engine_availability():
-    path = get_container_engine_path()
-    if path:
-        try:
-            subprocess.run([path, '--version'], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        except subprocess.CalledProcessError:
-            raise exception.ContainerEngineNotFound()
-    else:
+import json
+import subprocess
+import os
+from superide import __container_engine__, exception
+
+class Toolchain:
+    check_image_flag = False
+
+    def __init__(self, image_name, project_directory):
+        check_container_engine_availability()
+        self.image_name = image_name
+        self.project_directory = project_directory
+        self.contain_project_directory = "/workspaces/project"
+        self.check_image()
+        
+        
+    def check_image(self):
+        if(Toolchain.check_image_flag):
+            return
+        try:
+            print('check image...')
+            if(__container_engine__ == 'docker'):
+                output = subprocess.check_output(["docker", "images", "-q", self.image_name])
+                if output:
+                    Toolchain.check_image_flag = True
+                    return
+            subprocess.run([__container_engine__, 'pull', self.image_name], stderr=subprocess.DEVNULL)
+            Toolchain.check_image_flag = True
+        except subprocess.CalledProcessError:
+            raise exception.ImageNotGet()
+
+    def init_project(self):
+        # 文件夹非空则不能创建项目
+        if(len(os.listdir(self.project_directory)) != 0):
+            print("can't init project in Non empty folder")
+            raise exception.InitProjectError()
+        
+        source_path = '/workspaces/ExampleProject/.'
+        destination_path = self.contain_project_directory
+        try:
+            command = [__container_engine__, "run","-it","--rm", "-v", self.project_directory+":"+self.contain_project_directory, self.image_name, 
+                       'cp', '-r', source_path, destination_path];
+            subprocess.run(command)
+        except Exception:
+            print("init project failed")
+            raise exception.InitProjectError()
+
+    def _get_tools(self):
+        with open(f'{self.project_directory}/.vscode/tasks.json') as file:
+            config = json.load(file)
+        for task in config['tasks']:
+            if task['label'] == 'Build':
+                self.build_task = task
+            if task['label'] == 'Check':
+                self.check_task = task
+            if task['label'] == 'Run':
+                self.run_task = task
+
+    def build(self):
+        self._get_tools()
+        build_command = self.build_task["command"]+ " " + " ".join(self.build_task["args"])
+        return self.container_command(build_command)
+
+    def check(self):
+        self._get_tools()
+        check_command = self.check_task["command"]+ " " + " ".join(self.check_task["args"])
+        return self.container_command(check_command)
+    
+    def run(self):
+        self._get_tools()
+        run_command = self.run_task["command"]+ " " + " ".join(self.run_task["args"])
+        return self.container_command(run_command)
+
+    def container_command(self, command):
+        return " ".join([__container_engine__, "run","-it","--rm", "-v", self.project_directory+":"+self.contain_project_directory, self.image_name, command])
+    
+
+def get_container_engine_path():
+    try:
+        path = subprocess.check_output(['which', __container_engine__]).decode().strip()
+        return path
+    except subprocess.CalledProcessError:
+        return None
+
+def check_container_engine_availability():
+    path = get_container_engine_path()
+    if path:
+        try:
+            subprocess.run([path, '--version'], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        except subprocess.CalledProcessError:
+            raise exception.ContainerEngineNotFound()
+    else:
         raise exception.ContainerEngineNotFound()
```

### Comparing `super-ide-1.4.8/superide/util.py` & `super-ide-1.5.0/superide/util.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.8/tests/test_examples.py` & `super-ide-1.5.0/tests/test_examples.py`

 * *Files identical despite different names*

