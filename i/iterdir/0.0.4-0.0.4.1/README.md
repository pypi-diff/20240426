# Comparing `tmp/iterdir-0.0.4.tar.gz` & `tmp/iterdir-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterdir-0.0.4.tar", max compression
+gzip compressed data, was "iterdir-0.0.4.1.tar", max compression
```

## Comparing `iterdir-0.0.4.tar` & `iterdir-0.0.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.4/LICENSE
--rwxr-xr-x   0        0        0    10781 2024-04-26 15:16:26.832124 iterdir-0.0.4/iterdir/__init__.py
--rwxr-xr-x   0        0        0     8751 2024-04-26 15:17:56.986591 iterdir-0.0.4/iterdir/__main__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iterdir-0.0.4/iterdir/py.typed
--rw-r--r--   0        0        0     1113 2024-04-26 15:18:56.123801 iterdir-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3704 2024-04-19 12:19:41.653359 iterdir-0.0.4/readme.md
--rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 iterdir-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.4.1/LICENSE
+-rwxr-xr-x   0        0        0    10781 2024-04-26 15:16:26.832124 iterdir-0.0.4.1/iterdir/__init__.py
+-rwxr-xr-x   0        0        0     8994 2024-04-26 15:22:52.421236 iterdir-0.0.4.1/iterdir/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iterdir-0.0.4.1/iterdir/py.typed
+-rw-r--r--   0        0        0     1115 2024-04-26 15:23:17.792025 iterdir-0.0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3704 2024-04-19 12:19:41.653359 iterdir-0.0.4.1/readme.md
+-rw-r--r--   0        0        0     4801 1970-01-01 00:00:00.000000 iterdir-0.0.4.1/PKG-INFO
```

### Comparing `iterdir-0.0.4/LICENSE` & `iterdir-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.4/iterdir/__init__.py` & `iterdir-0.0.4.1/iterdir/__init__.py`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.4/iterdir/__main__.py` & `iterdir-0.0.4.1/iterdir/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         file.close()
 
 parser_iter.set_defaults(func=main_iter)
 
 parser_stats = subparsers.add_parser("stats", description="目录树遍历统计")
 
 parser_stats.add_argument("path", nargs="?", default="", help="文件夹路径，默认为当前工作目录")
+parser_stats.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 pathlib.Path），用于对路径进行筛选")
 parser_stats.add_argument("-m", "--min-depth", default=0, type=int, help="最小深度，默认值 0，小于 0 时不限")
 parser_stats.add_argument("-M", "--max-depth", default=-1, type=int, help="最大深度，默认值 -1，小于 0 时不限")
 parser_stats.add_argument("-v", "--version", action="store_true", help="输出版本号")
 
 def main_stats(args):
     from iterdir import __version__, DirEntry, statsdir
 
@@ -232,10 +233,15 @@
         min_depth=args.min_depth, 
         max_depth=args.max_depth, 
         predicate=predicate, 
     ))
 
 parser_stats.set_defaults(func=main_stats)
 
+parser.set_defaults(sub="")
+
 args = parser.parse_args()
-args.func(args)
+if args.sub:
+    args.func(args)
+else:
+    parser.parse_args(["-h"])
```

### Comparing `iterdir-0.0.4/pyproject.toml` & `iterdir-0.0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iterdir"
-version = "0.0.4"
+version = "0.0.4.1"
 description = "iterdir."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 keywords = ["iterdir", "traverse"]
```

### Comparing `iterdir-0.0.4/readme.md` & `iterdir-0.0.4.1/readme.md`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.4/PKG-INFO` & `iterdir-0.0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterdir
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: iterdir.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir
 License: MIT
 Keywords: iterdir,traverse
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

