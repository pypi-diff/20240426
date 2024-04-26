# Comparing `tmp/tgeraser-1.2.7.tar.gz` & `tmp/tgeraser-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgeraser-1.2.7.tar", last modified: Mon Nov 20 05:13:10 2023, max compression
+gzip compressed data, was "tgeraser-1.2.8.tar", last modified: Fri Apr 26 16:51:13 2024, max compression
```

## Comparing `tgeraser-1.2.7.tar` & `tgeraser-1.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 05:13:10.160047 tgeraser-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-20 05:12:58.000000 tgeraser-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-11-20 05:13:10.160047 tgeraser-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2023-11-20 05:12:58.000000 tgeraser-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-11-20 05:12:58.000000 tgeraser-1.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-11-20 05:13:10.160047 tgeraser-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-20 05:12:58.000000 tgeraser-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 05:13:10.156047 tgeraser-1.2.7/tgeraser/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-20 05:12:58.000000 tgeraser-1.2.7/tgeraser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-20 05:12:58.000000 tgeraser-1.2.7/tgeraser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-20 05:13:01.000000 tgeraser-1.2.7/tgeraser/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2023-11-20 05:12:58.000000 tgeraser-1.2.7/tgeraser/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2023-11-20 05:12:58.000000 tgeraser-1.2.7/tgeraser/eraser.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-20 05:12:58.000000 tgeraser-1.2.7/tgeraser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-11-20 05:12:58.000000 tgeraser-1.2.7/tgeraser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 05:13:10.160047 tgeraser-1.2.7/tgeraser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-11-20 05:13:10.000000 tgeraser-1.2.7/tgeraser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-11-20 05:13:10.000000 tgeraser-1.2.7/tgeraser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 05:13:10.000000 tgeraser-1.2.7/tgeraser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-20 05:13:10.000000 tgeraser-1.2.7/tgeraser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 05:13:09.000000 tgeraser-1.2.7/tgeraser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-20 05:13:10.000000 tgeraser-1.2.7/tgeraser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-20 05:13:10.000000 tgeraser-1.2.7/tgeraser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:51:13.834400 tgeraser-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:51:08.000000 tgeraser-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-26 16:51:13.834400 tgeraser-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-26 16:51:08.000000 tgeraser-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-26 16:51:08.000000 tgeraser-1.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-26 16:51:13.834400 tgeraser-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 16:51:08.000000 tgeraser-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:51:13.834400 tgeraser-1.2.8/tgeraser/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-26 16:51:08.000000 tgeraser-1.2.8/tgeraser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-26 16:51:08.000000 tgeraser-1.2.8/tgeraser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-26 16:51:10.000000 tgeraser-1.2.8/tgeraser/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-26 16:51:08.000000 tgeraser-1.2.8/tgeraser/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-26 16:51:08.000000 tgeraser-1.2.8/tgeraser/eraser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-26 16:51:08.000000 tgeraser-1.2.8/tgeraser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-26 16:51:08.000000 tgeraser-1.2.8/tgeraser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:51:13.834400 tgeraser-1.2.8/tgeraser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-26 16:51:13.000000 tgeraser-1.2.8/tgeraser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-26 16:51:13.000000 tgeraser-1.2.8/tgeraser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:51:13.000000 tgeraser-1.2.8/tgeraser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 16:51:13.000000 tgeraser-1.2.8/tgeraser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:51:13.000000 tgeraser-1.2.8/tgeraser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 16:51:13.000000 tgeraser-1.2.8/tgeraser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 16:51:13.000000 tgeraser-1.2.8/tgeraser.egg-info/top_level.txt
```

### Comparing `tgeraser-1.2.7/LICENSE` & `tgeraser-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tgeraser-1.2.7/PKG-INFO` & `tgeraser-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgeraser
-Version: 1.2.7
+Version: 1.2.8
 Summary: Tool deletes all your messages from chat/channel/conversation on Telegram.
 Home-page: https://github.com/en9inerd/tgeraser
 Author: Vladimir Loskutov
 Author-email: vladimir@enginerd.io
 License: MIT License
 Keywords: telegram,api,delete messages
 Classifier: Programming Language :: Python
```

### Comparing `tgeraser-1.2.7/README.md` & `tgeraser-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `tgeraser-1.2.7/setup.cfg` & `tgeraser-1.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `tgeraser-1.2.7/tgeraser/core.py` & `tgeraser-1.2.8/tgeraser/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,27 @@
 
 from .__version__ import VERSION
 from .eraser import Eraser
 from .exceptions import TgEraserException
 from .utils import cast_to_int, get_credentials
 
 
+def signal_handler():
+    print("\nCtrl+C captured, exiting...")
+    sys.stdout.flush()
+    os._exit(0)
+
+
 async def main() -> None:
     """
     Entry function
     """
+    loop = asyncio.get_running_loop()
+    loop.add_signal_handler(signal.SIGINT, signal_handler)
+
     arguments = docopt(__doc__, version=VERSION)
     if arguments["--limit"]:
         arguments["--limit"] = cast_to_int(arguments["--limit"], "limit")
     if arguments["--time-period"]:
         periods = {
             "seconds": 1,
             "minutes": 60,
@@ -93,16 +102,14 @@
                         period[1],
                     )
                 )
                 await asyncio.sleep(int(period[0]) * periods[period[1]])
             else:
                 break
         await client.disconnect()
-    except asyncio.CancelledError as err:
-        print("\n\nCancelled by user.\n", file=sys.stderr)
     except Exception as err:
         raise TgEraserException(err) from err
 
 
 def entry() -> None:
     """
     Entry point function
```

### Comparing `tgeraser-1.2.7/tgeraser/eraser.py` & `tgeraser-1.2.8/tgeraser/eraser.py`

 * *Files identical despite different names*

### Comparing `tgeraser-1.2.7/tgeraser/utils.py` & `tgeraser-1.2.8/tgeraser/utils.py`

 * *Files identical despite different names*

### Comparing `tgeraser-1.2.7/tgeraser.egg-info/PKG-INFO` & `tgeraser-1.2.8/tgeraser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgeraser
-Version: 1.2.7
+Version: 1.2.8
 Summary: Tool deletes all your messages from chat/channel/conversation on Telegram.
 Home-page: https://github.com/en9inerd/tgeraser
 Author: Vladimir Loskutov
 Author-email: vladimir@enginerd.io
 License: MIT License
 Keywords: telegram,api,delete messages
 Classifier: Programming Language :: Python
```

