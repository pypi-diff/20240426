# Comparing `tmp/pawnlib-1.1.3.tar.gz` & `tmp/pawnlib-1.1.5.tar.gz`

## Comparing `pawnlib-1.1.3.tar` & `pawnlib-1.1.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    10481 2020-02-02 00:00:00.000000 pawnlib-1.1.3/README.md
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/.DS_Store
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/__main__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/__version__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/asyncio/__init__.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/asyncio/run.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/builder/__init__.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/builder/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/builder/templates/__init__.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/builder/templates/app_with_logging.tmpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/__init__.py
--rwxr-xr-x   0        0        0     3290 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/aws.py
--rwxr-xr-x   0        0        0     1170 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/banner.py
--rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/docker.py
--rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/gs.py
--rwxr-xr-x   0        0        0    21479 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/http.py
--rwxr-xr-x   0        0        0     2805 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/icon.py
--rwxr-xr-x   0        0        0     6105 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/info.py
--rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/init.py
--rwxr-xr-x   0        0        0     6923 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/main_cli.py
--rwxr-xr-x   0        0        0     2965 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/main_cli_with_required.py__
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/net.py
--rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/pawns_cli.py__
--rwxr-xr-x   0        0        0    16005 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/proxy.py
--rw-r--r--   0        0        0    16006 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/rpc.py
--rwxr-xr-x   0        0        0    11497 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/top.py
--rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/wallet.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/templates/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/templates/docker_echo.tmpl
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/cli/templates/docker_planet.tmpl
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/config/__fix_import.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/config/__init__.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/config/configure.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/config/console.py
--rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/config/first_run_checker.py
--rw-r--r--   0        0        0    30148 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/config/globalconfig.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/docker/__init__.py
--rw-r--r--   0        0        0    15894 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/docker/async_docker.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/input/__init__.py
--rw-r--r--   0        0        0    43248 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/input/prompt.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/output/__init__.py
--rw-r--r--   0        0        0    55490 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/output/color_print.py
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/output/file.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/resource/__init__.py
--rw-r--r--   0        0        0    16910 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/resource/net.py
--rw-r--r--   0        0        0    34175 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/resource/server.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/typing/__init__.py
--rw-r--r--   0        0        0    18737 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/typing/check.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/typing/constants.py
--rw-r--r--   0        0        0    82280 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/typing/converter.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/typing/date_utils.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/typing/defines.py
--rw-r--r--   0        0        0    14793 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/typing/generator.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/utils/__init__.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/utils/genesis.py
--rw-r--r--   0        0        0    80276 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/utils/http.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/utils/icx_raw_singer.py
--rw-r--r--   0        0        0    27296 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/utils/icx_signer.py
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/utils/in_memory_zip.py
--rw-r--r--   0        0        0    12702 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/utils/log.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/utils/notify.py
--rw-r--r--   0        0        0    25574 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pawnlib/utils/operate_handler.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pawnlib-1.1.3/.gitignore
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 pawnlib-1.1.3/pyproject.toml
--rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 pawnlib-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    10481 2020-02-02 00:00:00.000000 pawnlib-1.1.5/README.md
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/.DS_Store
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/__main__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/__version__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/asyncio/__init__.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/asyncio/run.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/builder/__init__.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/builder/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/builder/templates/__init__.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/builder/templates/app_with_logging.tmpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/__init__.py
+-rwxr-xr-x   0        0        0     3290 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/aws.py
+-rwxr-xr-x   0        0        0     1170 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/banner.py
+-rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/docker.py
+-rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/gs.py
+-rwxr-xr-x   0        0        0    21479 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/http.py
+-rwxr-xr-x   0        0        0     2805 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/icon.py
+-rwxr-xr-x   0        0        0     6105 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/info.py
+-rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/init.py
+-rwxr-xr-x   0        0        0     6923 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/main_cli.py
+-rwxr-xr-x   0        0        0     2965 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/main_cli_with_required.py__
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/net.py
+-rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/pawns_cli.py__
+-rwxr-xr-x   0        0        0    16005 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/proxy.py
+-rw-r--r--   0        0        0    16006 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/rpc.py
+-rwxr-xr-x   0        0        0    11497 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/top.py
+-rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/wallet.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/templates/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/templates/docker_echo.tmpl
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/cli/templates/docker_planet.tmpl
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/config/__fix_import.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/config/__init__.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/config/configure.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/config/console.py
+-rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/config/first_run_checker.py
+-rw-r--r--   0        0        0    30148 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/config/globalconfig.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/docker/__init__.py
+-rw-r--r--   0        0        0    15894 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/docker/async_docker.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/input/__init__.py
+-rw-r--r--   0        0        0    43248 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/input/prompt.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/output/__init__.py
+-rw-r--r--   0        0        0    55490 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/output/color_print.py
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/output/file.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/resource/__init__.py
+-rw-r--r--   0        0        0    19961 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/resource/net.py
+-rw-r--r--   0        0        0    34175 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/resource/server.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/typing/__init__.py
+-rw-r--r--   0        0        0    18737 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/typing/check.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/typing/constants.py
+-rw-r--r--   0        0        0    83951 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/typing/converter.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/typing/date_utils.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/typing/defines.py
+-rw-r--r--   0        0        0    14793 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/typing/generator.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/utils/__init__.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/utils/genesis.py
+-rw-r--r--   0        0        0    80276 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/utils/http.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/utils/icx_raw_singer.py
+-rw-r--r--   0        0        0    27296 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/utils/icx_signer.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/utils/in_memory_zip.py
+-rw-r--r--   0        0        0    12702 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/utils/log.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/utils/notify.py
+-rw-r--r--   0        0        0    25574 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pawnlib/utils/operate_handler.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pawnlib-1.1.5/.gitignore
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 pawnlib-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 pawnlib-1.1.5/PKG-INFO
```

### Comparing `pawnlib-1.1.3/README.md` & `pawnlib-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/.DS_Store` & `pawnlib-1.1.5/pawnlib/.DS_Store`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/__init__.py` & `pawnlib-1.1.5/pawnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/__main__.py` & `pawnlib-1.1.5/pawnlib/__main__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/asyncio/run.py` & `pawnlib-1.1.5/pawnlib/asyncio/run.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/builder/generator.py` & `pawnlib-1.1.5/pawnlib/builder/generator.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/builder/templates/app_with_logging.tmpl` & `pawnlib-1.1.5/pawnlib/builder/templates/app_with_logging.tmpl`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/aws.py` & `pawnlib-1.1.5/pawnlib/cli/aws.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/banner.py` & `pawnlib-1.1.5/pawnlib/cli/banner.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/docker.py` & `pawnlib-1.1.5/pawnlib/cli/docker.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/gs.py` & `pawnlib-1.1.5/pawnlib/cli/gs.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/http.py` & `pawnlib-1.1.5/pawnlib/cli/http.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/icon.py` & `pawnlib-1.1.5/pawnlib/cli/icon.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/info.py` & `pawnlib-1.1.5/pawnlib/cli/info.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/init.py` & `pawnlib-1.1.5/pawnlib/cli/init.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/main_cli.py` & `pawnlib-1.1.5/pawnlib/cli/main_cli.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/main_cli_with_required.py__` & `pawnlib-1.1.5/pawnlib/cli/main_cli_with_required.py__`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/net.py` & `pawnlib-1.1.5/pawnlib/cli/net.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,22 +95,25 @@
     )
     parser.add_argument('-d', '--debug', action='store_true', help='Debug mode (True/False)')
     parser.add_argument('-v', '--verbose', action='count', help='Verbose mode (view level)', default=0)
 
     parser.add_argument('-p', '--port', type=int, help='Port number (e.g., 80)', default=80)
     parser.add_argument('--host', type=str, help='Single host IP (e.g., 192.168.1.1)', default="localhost")
     parser.add_argument('--host-range', type=str, help='Host IP range (e.g., 192.168.1.1-192.168.1.255)', default="")
-    parser.add_argument('--port-range', type=str, help='Port range (e.g., 20-80)', default="")
-    parser.add_argument('-w', '--worker', type=int, help='Max concurrency worker count', default=100)
+    parser.add_argument('--port-range', type=str, help='Port range (e.g., 20-80)', default="0-65535")
+    parser.add_argument('-w', '--worker', type=int, help='Max concurrency worker count', default=10000)
     parser.add_argument('-t', '--timeout', type=float, help='timeout', default=1)
-    parser.add_argument('-b', '--batch-size', type=int, help='timeout', default=10000)
+    parser.add_argument('-b', '--batch-size', type=int, help='timeout', default=1000)
+    parser.add_argument('-f', '--fast-scan', action='store_true', help='fast scan mode', default=False)
+
     parser.add_argument('--view-type', type=str, choices=['open', 'closed', 'all'], help='Type of results to view (open, closed, all)', default="open")
 
     return parser
 
+
 def print_banner():
     banner = generate_banner(
         app_name="NET",
         author=f"jinwoo",
         description="Network checker",
         font="graffiti",
         version=_version
@@ -158,25 +161,28 @@
     elif args.command == "check":
         find_fastest_region(args)
 
     elif args.command == "wait":
         wait_for_port_open(args.host, args.port, timeout=args.timeout)
 
     elif args.command == "scan":
+        if not args.host_range and args.host:
+            args.host_range = f"{args.host}-{args.host}"
+
         host_range = validate_host_range(args.host_range)
         port_range = validate_port_range(args.port_range)
         pawn.console.log(f"🔎 Start scanning worker={args.worker}, view_type={args.view_type} 🔎\n Host range:{format_range(host_range)} , Port range:{format_range(port_range)} ")
 
         scanner = net.AsyncPortScanner(
             ip_range=host_range,
             port_range=port_range,
             max_concurrency=args.worker,
             batch_size=args.batch_size,
-
+            timeout=args.timeout,
         )
-        scanner.run_scan()
+        scanner.run_scan(fast_scan=args.fast_scan)
         print("\n\n")
         scanner.print_scan_results(view=args.view_type)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pawnlib-1.1.3/pawnlib/cli/pawns_cli.py__` & `pawnlib-1.1.5/pawnlib/cli/pawns_cli.py__`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/proxy.py` & `pawnlib-1.1.5/pawnlib/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/rpc.py` & `pawnlib-1.1.5/pawnlib/cli/rpc.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/top.py` & `pawnlib-1.1.5/pawnlib/cli/top.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/wallet.py` & `pawnlib-1.1.5/pawnlib/cli/wallet.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/websocket.py` & `pawnlib-1.1.5/pawnlib/cli/websocket.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/templates/docker_echo.tmpl` & `pawnlib-1.1.5/pawnlib/cli/templates/docker_echo.tmpl`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/cli/templates/docker_planet.tmpl` & `pawnlib-1.1.5/pawnlib/cli/templates/docker_planet.tmpl`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/config/__fix_import.py` & `pawnlib-1.1.5/pawnlib/config/__fix_import.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/config/configure.py` & `pawnlib-1.1.5/pawnlib/config/configure.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/config/console.py` & `pawnlib-1.1.5/pawnlib/config/console.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/config/first_run_checker.py` & `pawnlib-1.1.5/pawnlib/config/first_run_checker.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/config/globalconfig.py` & `pawnlib-1.1.5/pawnlib/config/globalconfig.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/docker/async_docker.py` & `pawnlib-1.1.5/pawnlib/docker/async_docker.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/input/__init__.py` & `pawnlib-1.1.5/pawnlib/input/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/input/prompt.py` & `pawnlib-1.1.5/pawnlib/input/prompt.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/output/__init__.py` & `pawnlib-1.1.5/pawnlib/output/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/output/color_print.py` & `pawnlib-1.1.5/pawnlib/output/color_print.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/output/file.py` & `pawnlib-1.1.5/pawnlib/output/file.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/resource/__init__.py` & `pawnlib-1.1.5/pawnlib/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/resource/net.py` & `pawnlib-1.1.5/pawnlib/resource/net.py`

 * *Files 14% similar despite different names*

```diff
@@ -176,81 +176,144 @@
 
         .. code-block:: python
 
             scanner = AsyncPortScanner(("192.168.0.1", "192.168.0.255"), (1, 1024), 50)
             asyncio.run(scanner.scan_all())
     """
 
-    def __init__(self, ip_range: Tuple[str, str], port_range: Tuple[int, int] = (0, 65535), max_concurrency: int = 30, timeout=1, batch_size=50000):
+    def __init__(self, ip_range: Tuple[str, str], port_range: Tuple[int, int] = (0, 65535),
+                 max_concurrency: int = 30, timeout=1, ping_timeout=0.05, fast_scan_ports: List[int] = [22, 80, 443], batch_size=50000):
         self.start_ip, self.end_ip = ip_range
         self.start_port, self.end_port = port_range
         self.scan_results = {}
         self.semaphore = asyncio.Semaphore(max_concurrency)
         self.timeout = timeout
+        self.ping_timeout = ping_timeout
+        self.fast_scan_ports = fast_scan_ports
         self.batch_size = batch_size
 
-    async def scan_port(self, ip: str, port: int) -> bool:
-        async with self.semaphore:
-            pawn.console.debug(f"Scanning {ip}:{port} - Acquired semaphore")
+    async def ping_host(self, ip: str) -> bool:
+        common_ports = [22, 80, 443]
+        for port in common_ports:
+            try:
+                await asyncio.wait_for(asyncio.open_connection(ip, port), timeout=self.ping_timeout)
+                return ip  # 연결 성공, 호스트가 살아 있음
+            except Exception:
+                continue  # 해당 포트에 대한 연결 실패, 다음 포트 시도
+        return False  # 모든 시도 실패, 호스트가 닫혀 있음
+
+    async def try_ping_host(self, ip: str, progress: Progress, task_id: int):
+        progress.advance(task_id)
+        for port in self.fast_scan_ports:
             try:
                 await asyncio.wait_for(asyncio.open_connection(ip, port), timeout=self.timeout)
-                # pawn.console.debug(f"Connection successful: {ip}:{port}")
+                if progress is not None and task_id is not None:
+                    progress.advance(task_id)  # 성공적으로 핑을 완료하면 진행 상황을 업데이트합니다.
+                return ip
+            except (asyncio.TimeoutError, Exception):
+                continue  # 해당 포트에서 연결 실패, 다음 포트로 계속 시도합니다.
+        return False
+
+    async def scan_all(self, fast_scan: bool = False):
+        if fast_scan:
+            tasks = [self.check_and_scan_host(ip) for ip in self._generate_ips()]
+        else:
+            tasks = [
+                self.wrap_scan(ip, port)
+                for ip in self._generate_ips()
+                for port in range(self.start_port, self.end_port + 1)
+            ]
+        await asyncio.gather(*tasks)
+
+    async def check_and_scan_host(self, ip):
+        if await self.ping_host(ip):
+            print(f"{ip} is up, scanning ports...")
+            tasks = [self.wrap_scan(ip, port) for port in range(self.start_port, self.end_port + 1)]
+            await asyncio.gather(*tasks)
+        else:
+            print(f"{ip} is down, skipping...")
+
+    async def scan_port(self, ip: str, port: int) ->(str, int, bool):
+        async with (self.semaphore):
+            pawn.console.debug(f"Scanning {ip}:{port} - Acquired semaphore, timeout={self.timeout}")
+            try:
+                await asyncio.wait_for(asyncio.open_connection(ip, port), timeout=self.timeout)
+                pawn.console.debug(f"Connection successful: {ip}:{port}")
                 return ip, port, True
             except asyncio.TimeoutError:
-                # pawn.console.debug(f"Timeout: {ip}:{port}")
+                pawn.console.debug(f"Timeout: {ip}:{port}")
                 return ip, port, False
             except Exception as e:
-                # pawn.console.debug(f"Error scanning {ip}:{port} - {e}")
+                if "Too many" in str(e):
+                    pawn.console.log(f"Error scanning -> [red]{e}[/red]")
+                else:
+                    pawn.console.debug(f"Error scanning {ip}:{port} - {e}")
                 return ip, port, False
             # finally:
-            #     pawn.console.debug(f"Releasing semaphore: {ip}:{port}")
+            #     pawn.console.log(f"Releasing semaphore: {ip}:{port}")
 
     def calculate_scan_range(self):
         start_ip_int = self.ip_to_int(self.start_ip)
         end_ip_int = self.ip_to_int(self.end_ip)
         total_ips = end_ip_int - start_ip_int + 1
         total_ports = self.end_port - self.start_port + 1
         total_tasks = total_ips * total_ports
         return start_ip_int, end_ip_int, total_tasks
 
-    async def scan(self, progress: Progress):
-        start_ip_int, end_ip_int, total_tasks = self.calculate_scan_range()
-        task_id = progress.add_task("[cyan]Scanning...", total=total_tasks)
-
+    async def scan(self, fast_scan: bool = False, progress: Progress = None):
         tasks = []
-        for ip_int in range(start_ip_int, end_ip_int + 1):
-            ip = self.int_to_ip(ip_int)
+        ips_to_scan = await self.get_ips_to_scan(fast_scan, progress)
+        if fast_scan:
+            if ips_to_scan:
+                pawn.console.log(f"<FAST SCAN> Alive IPs: {ips_to_scan}")
+            else:
+                pawn.console.log(f"<FAST SCAN> [red]No open servers found on ports {self.fast_scan_ports}.[/red]")
+
+        total_ports = self.end_port - self.start_port + 1
+        total_tasks = len(ips_to_scan) * total_ports
+        fast_scan_string = "FastScan" if fast_scan else ""
+        task_id = progress.add_task(f"[cyan]Scanning {fast_scan_string}...", total=total_tasks)
+        if fast_scan:
+            pawn.console.log(f"Alive IP: {ips_to_scan}")
+
+        for ip in ips_to_scan:
             for port in range(self.start_port, self.end_port + 1):
-                tasks.append(self.wrap_scan(ip, port, progress, task_id))
+                task = self.wrap_scan(ip, port, progress, task_id)
+                tasks.append(task)
                 if len(tasks) >= self.batch_size:
-                    pawn.console.debug(f"Processing batch of {self.batch_size} tasks")
                     await asyncio.gather(*tasks)
-                    tasks = []
+                    tasks.clear()
 
-        # 남은 태스크 처리
         if tasks:
-            pawn.console.debug(f"Processing final batch of {len(tasks)} tasks")
             await asyncio.gather(*tasks)
 
-        pawn.console.log("task_completed")
-        # self._process_results(results)
+    async def get_ips_to_scan(self, fast_scan: bool, progress: Progress) -> List[str]:
+        ips = self._generate_ips()
+        if not fast_scan:
+            return ips
+
+        task_id = progress.add_task("Checking IPs...", total=len(ips))
+        ping_tasks = [self.try_ping_host(ip, progress, task_id) for ip in ips]
+
+        results = await asyncio.gather(*ping_tasks)
+        alive_ips = [result for result in results if result]
+        return alive_ips
 
     async def wrap_scan(self, ip, port, progress, task_id):
         async with self.semaphore:
             result = await self.scan_port(ip, port)
             progress.update(task_id, advance=1)
             self._process_results(result)
             return result
 
     def _generate_ips(self) -> List[str]:
         start_int = self.ip_to_int(self.start_ip)
         end_int = self.ip_to_int(self.end_ip)
         return [self.int_to_ip(ip_int) for ip_int in range(start_int, end_int + 1)]
 
-
     @staticmethod
     def ip_to_int(ip: str) -> int:
         return sum([int(octet) << (8 * i) for i, octet in enumerate(reversed(ip.split('.')))])
 
     @staticmethod
     def int_to_ip(ip_int: int) -> str:
         return '.'.join(str((ip_int >> (8 * i)) & 0xFF) for i in reversed(range(4)))
@@ -279,25 +342,26 @@
                     parsed_data = f"\t \[{is_open}] {port}"
                     # is_data = True
 
             if parsed_data:
                 pawn.console.print(ipaddr)
                 pawn.console.print(parsed_data)
 
-
-    def run_scan(self):
+    def run_scan(self, fast_scan: bool = False):
         with Progress(
                 TextColumn("[bold blue]{task.description}", justify="right"),
                 BarColumn(bar_width=None),
                 TextColumn("{task.completed}/{task.total} • [progress.percentage]{task.percentage:>3.0f}%"),
                 "•",
                 TimeRemainingColumn(),
                 transient=True  # Hide the progress bar when done
         ) as progress:
-            asyncio.get_event_loop().run_until_complete(self.scan(progress))
+            # asyncio.get_event_loop().run_until_complete(self.scan(progress))
+            asyncio.get_event_loop().run_until_complete(self.scan(fast_scan, progress))
+
 
 def get_local_ip():
     """
 
     Get the local IP address
 
     :return:
```

### Comparing `pawnlib-1.1.3/pawnlib/resource/server.py` & `pawnlib-1.1.5/pawnlib/resource/server.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/typing/__init__.py` & `pawnlib-1.1.5/pawnlib/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/typing/check.py` & `pawnlib-1.1.5/pawnlib/typing/check.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/typing/constants.py` & `pawnlib-1.1.5/pawnlib/typing/constants.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/typing/converter.py` & `pawnlib-1.1.5/pawnlib/typing/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1354,38 +1354,63 @@
                 else:
                     ret[f"{key}{separator}{i}"] = value
         else:
             ret[key] = val
     return ret
 
 
-def dict_to_line(dict_param: dict, quotes: bool = False, separator: str = "=", end_separator: str = ",") -> str:
+def dict_to_line(dict_param: dict, quotes: bool = False, separator: str = "=", end_separator: str = ",",
+                 pad_width: int = 0, key_pad_width: int = 0, alignment: str = 'left', key_alignment: str = 'right',
+                 callback: callable = None) -> str:
     """
-    This function converts a dict to a line.
+       Converts a dictionary into a string with various formatting options.
 
-    :param dict_param:
-    :param quotes:
-    :param separator:
-    :param end_separator:
-    :return:
+       :param dict_param: The dictionary to convert.
+       :param quotes: If True, wraps values in quotes.
+       :param separator: The separator between keys and values.
+       :param end_separator: The separator between key-value pairs.
+       :param pad_width: The minimum width for value alignment.
+       :param key_pad_width: The minimum width for key alignment.
+       :param alignment: The alignment of the values ('left', 'right', 'center').
+       :param key_alignment: The alignment of the keys ('left', 'right', 'center').
+       :param callback: An optional callback function to apply to each value.
+       :return: The formatted string.
+
+       Example:
+
+           .. code-block:: python
+
+               dict_param = {'a': 1, 'bb': 22, 'ccc': 333}
+               print(dict_to_line(dict_param, quotes=True, separator=": ", end_separator="; ", pad_width=5, key_pad_width=4, alignment='right', key_alignment='left'))
+               # "a   : "    1"; bb  : "   22"; ccc : "  333"
+       """
+    def _format_with_alignment(text, width, alignment):
+        """
+        Formats text according to the given alignment and width.
+        """
+        formats = {'left': f"<{width}", 'right': f">{width}", 'center': f"^{width}"}
+        format_spec = formats.get(alignment, "<")
+        return f"{text:{format_spec}}"
 
-    Example:
-
-        .. code-block:: python
+    formatted_pairs = []
+    for k, v in sorted(dict_param.items()):
+        if callback and callable(callback):
+            v = callback(v)  # Apply the callback function to the value, if provided
 
-            # >> {"a": "1234", "b": "1235"} => "a=1234,b=1235"
+        # Apply alignment and padding to keys and values
+        formatted_key = _format_with_alignment(k, key_pad_width, key_alignment)
+        formatted_value = _format_with_alignment(v, pad_width, alignment)
 
-    """
-    return_value = ""
-    for k, v in sorted(dict_param.items()):
+        # Handle quotes option for values
         if quotes:
-            return_value += f"{k}{separator}\"{v}\"{end_separator}"
-        else:
-            return_value += f"{k}{separator}{v}{end_separator}"
-    return return_value.rstrip(end_separator)
+            formatted_value = f"\"{formatted_value}\""
+
+        formatted_pairs.append(f"{formatted_key}{separator}{formatted_value}")
+
+    return end_separator.join(formatted_pairs)
 
 
 def dict_none_to_zero(data: dict) -> dict:
     """
     Convert the None type of the dictionary to zero.
```

### Comparing `pawnlib-1.1.3/pawnlib/typing/date_utils.py` & `pawnlib-1.1.5/pawnlib/typing/date_utils.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/typing/defines.py` & `pawnlib-1.1.5/pawnlib/typing/defines.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/typing/generator.py` & `pawnlib-1.1.5/pawnlib/typing/generator.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/utils/__init__.py` & `pawnlib-1.1.5/pawnlib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/utils/genesis.py` & `pawnlib-1.1.5/pawnlib/utils/genesis.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/utils/http.py` & `pawnlib-1.1.5/pawnlib/utils/http.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/utils/icx_raw_singer.py` & `pawnlib-1.1.5/pawnlib/utils/icx_raw_singer.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/utils/icx_signer.py` & `pawnlib-1.1.5/pawnlib/utils/icx_signer.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/utils/in_memory_zip.py` & `pawnlib-1.1.5/pawnlib/utils/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/utils/log.py` & `pawnlib-1.1.5/pawnlib/utils/log.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/utils/notify.py` & `pawnlib-1.1.5/pawnlib/utils/notify.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pawnlib/utils/operate_handler.py` & `pawnlib-1.1.5/pawnlib/utils/operate_handler.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/.gitignore` & `pawnlib-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/pyproject.toml` & `pawnlib-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.3/PKG-INFO` & `pawnlib-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawnlib
-Version: 1.1.3
+Version: 1.1.5
 Summary: pawnlib is a collection of libraries for IaC.
 Project-URL: Changelog, https://github.com/jinwoo-j/pawnlib
 Project-URL: Documentation, https://pawnlib.readthedocs.io
 Project-URL: Homepage, https://pawnlib.readthedocs.io
 Project-URL: Source, https://github.com/jinwoo-j/pawnlib
 Author-email: Jinwoo <jinwoo@parametacorp.com>
 License-Expression: MIT
```

