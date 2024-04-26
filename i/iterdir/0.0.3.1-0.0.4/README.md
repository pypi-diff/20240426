# Comparing `tmp/iterdir-0.0.3.1.tar.gz` & `tmp/iterdir-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterdir-0.0.3.1.tar", max compression
+gzip compressed data, was "iterdir-0.0.4.tar", max compression
```

## Comparing `iterdir-0.0.3.1.tar` & `iterdir-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.3.1/LICENSE
--rwxr-xr-x   0        0        0     9422 2024-04-19 12:20:28.873152 iterdir-0.0.3.1/iterdir/__init__.py
--rwxr-xr-x   0        0        0     6541 2024-04-19 12:03:02.095182 iterdir-0.0.3.1/iterdir/__main__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iterdir-0.0.3.1/iterdir/py.typed
--rw-r--r--   0        0        0     1070 2024-04-19 11:48:38.366578 iterdir-0.0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3704 2024-04-19 12:19:41.653359 iterdir-0.0.3.1/readme.md
--rw-r--r--   0        0        0     5170 1970-01-01 00:00:00.000000 iterdir-0.0.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.4/LICENSE
+-rwxr-xr-x   0        0        0    10781 2024-04-26 15:16:26.832124 iterdir-0.0.4/iterdir/__init__.py
+-rwxr-xr-x   0        0        0     8751 2024-04-26 15:17:56.986591 iterdir-0.0.4/iterdir/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iterdir-0.0.4/iterdir/py.typed
+-rw-r--r--   0        0        0     1113 2024-04-26 15:18:56.123801 iterdir-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3704 2024-04-19 12:19:41.653359 iterdir-0.0.4/readme.md
+-rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 iterdir-0.0.4/PKG-INFO
```

### Comparing `iterdir-0.0.3.1/LICENSE` & `iterdir-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.3.1/iterdir/__init__.py` & `iterdir-0.0.4/iterdir/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 3)
-__all__ = ["DirEntry", "iterdir"]
+__version__ = (0, 0, 4)
+__all__ = ["DirEntry", "iterdir", "statsdir"]
 
 from collections import deque
 from collections.abc import Callable, Iterable, Iterator
 from os import (
     fspath, listdir, lstat, scandir, stat, stat_result, 
     DirEntry as _DirEntry, PathLike, 
 )
@@ -83,15 +83,15 @@
     top: PathType, 
     /, 
     is_dir: Callable[[PathType], bool], 
     iter_dir: Callable[[PathType], Iterable[PathType]], 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[[PathType], Optional[bool]]] = None, 
-    onerror: bool | Callable = False, 
+    onerror: bool | Callable[[OSError], bool] = False, 
     follow_symlinks: bool = False, 
 ) -> Iterator[PathType]:
     dq: deque[tuple[int, PathType]] = deque()
     push, pop = dq.append, dq.popleft
     push((0, top))
     while dq:
         depth, path = pop()
@@ -126,15 +126,15 @@
     /, 
     is_dir: Callable[[PathType], bool], 
     iter_dir: Callable[[PathType], Iterable[PathType]], 
     topdown: bool = True, 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[[PathType], Optional[bool]]] = None, 
-    onerror: bool | Callable = False, 
+    onerror: bool | Callable[[OSError], bool] = False, 
     follow_symlinks: bool = False, 
 ) -> Iterator[PathType]:
     if not max_depth:
         return
     global_yield_me = True
     if min_depth > 1:
         global_yield_me = False
@@ -185,58 +185,58 @@
 def iterdir(
     top: None = None, 
     /, 
     topdown: Optional[bool] = True, 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[[DirEntry[str]], Optional[bool]]] = None, 
-    onerror: bool | Callable = False, 
+    onerror: bool | Callable[[OSError], bool] = False, 
     follow_symlinks: bool = False, 
 ) -> Iterator[DirEntry[str]]: ...
 @overload
 def iterdir(
     top: DirEntry[AnyStr], 
     /, 
     topdown: Optional[bool] = True, 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[[DirEntry[AnyStr]], Optional[bool]]] = None, 
-    onerror: bool | Callable = False, 
+    onerror: bool | Callable[[OSError], bool] = False, 
     follow_symlinks: bool = False, 
 ) -> Iterator[DirEntry[AnyStr]]: ...
 @overload
 def iterdir(
     top: Path, 
     /, 
     topdown: Optional[bool] = True, 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[[Path], Optional[bool]]] = None, 
-    onerror: bool | Callable = False, 
+    onerror: bool | Callable[[OSError], bool] = False, 
     follow_symlinks: bool = False, 
 ) -> Iterator[Path]: ...
 @overload
 def iterdir(
     top: AnyStr, 
     /, 
     topdown: Optional[bool] = True, 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[[AnyStr], Optional[bool]]] = None, 
-    onerror: bool | Callable = False, 
+    onerror: bool | Callable[[OSError], bool] = False, 
     follow_symlinks: bool = False, 
 ) -> Iterator[AnyStr]: ...
 def iterdir(
     top = None, 
     /, 
     topdown: Optional[bool] = True, 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[..., Optional[bool]]] = None, 
-    onerror: bool | Callable = False, 
+    onerror: bool | Callable[[OSError], bool] = False, 
     follow_symlinks: bool = False, 
 ) -> Iterator:
     """遍历目录树
 
     :param top: 根路径，默认为当前目录。
     :param topdown: 如果是 True，自顶向下深度优先搜索；如果是 False，自底向上深度优先搜索；如果是 None，广度优先搜索。
     :param min_depth: 最小深度，小于 0 时不限。参数 `top` 本身的深度为 0，它的直接跟随路径的深度是 1，以此类推。
@@ -289,7 +289,59 @@
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
             predicate=predicate, 
             onerror=onerror, 
         )
 
+
+def format_bytes(
+    n: int, 
+    /, 
+    unit: str = "", 
+    precision: int = 6, 
+) -> str:
+    "scale bytes to its proper byte format"
+    if unit == "B" or not unit and n < 1024:
+        return f"{n} B"
+    b = 1
+    b2 = 1024
+    for u in ["K", "M", "G", "T", "P", "E", "Z", "Y"]:
+        b, b2 = b2, b2 << 10
+        if u == unit if unit else n < b2:
+            break
+    return f"%.{precision}f {u}B" % (n / b)
+
+
+def statsdir(
+    top=None, 
+    /, 
+    min_depth: int = 0, 
+    max_depth: int = -1, 
+    predicate: Optional[Callable[..., Optional[bool]]] = None, 
+    onerror: bool | Callable[[OSError], bool] = False, 
+    follow_symlinks: bool = False, 
+) -> dict:
+    files = 0
+    dirs = 0
+    size = 0
+    for path in iterdir(
+        top, 
+        min_depth=min_depth, 
+        max_depth=max_depth, 
+        predicate=predicate, 
+        onerror=onerror, 
+        follow_symlinks=follow_symlinks, 
+    ):
+        if isdir(path) and not islink(path):
+            dirs += 1
+        else:
+            files += 1
+            size += lstat(path).st_size
+    return {
+        "total": files + dirs, 
+        "files": files, 
+        "dirs": dirs, 
+        "size": size, 
+        "fmt_size": format_bytes(size)
+    }
+
```

### Comparing `iterdir-0.0.3.1/iterdir/__main__.py` & `iterdir-0.0.4/iterdir/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,189 +1,241 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 
 from argparse import ArgumentParser, RawTextHelpFormatter
-from iterdir import __version__, iterdir, DirEntry
+
+parser = ArgumentParser(description="目录树工具集", formatter_class=RawTextHelpFormatter)
+subparsers = parser.add_subparsers()
 
 KEYS = ("inode", "name", "path", "relpath", "isdir", "islink", "stat")
 
-parser = ArgumentParser(description="目录树信息遍历导出", formatter_class=RawTextHelpFormatter)
-parser.add_argument("path", nargs="?", default="", help="文件夹路径，默认为当前工作目录")
-parser.add_argument("-k", "--keys", nargs="*", choices=KEYS, help=f"选择输出的 key，默认输出所有可选值")
-parser.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 pathlib.Path），用于对路径进行筛选")
-parser.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""输出类型，默认为 json
+parser_iter = subparsers.add_parser("iter", description="目录树信息遍历导出")
+
+parser_iter.add_argument("path", nargs="?", default="", help="文件夹路径，默认为当前工作目录")
+parser_iter.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 pathlib.Path），用于对路径进行筛选")
+parser_iter.add_argument("-m", "--min-depth", default=0, type=int, help="最小深度，默认值 0，小于 0 时不限")
+parser_iter.add_argument("-M", "--max-depth", default=-1, type=int, help="最大深度，默认值 -1，小于 0 时不限")
+parser_iter.add_argument("-v", "--version", action="store_true", help="输出版本号")
+
+parser_iter.add_argument("-k", "--keys", nargs="*", choices=KEYS, help=f"选择输出的 key，默认输出所有可选值")
+parser_iter.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""\
+输出类型，默认为 log
 - log   每行输出一条数据，每条数据输出为一个 json 的 object
 - json  输出一个 json 的 list，每条数据输出为一个 json 的 object
 - csv   输出一个 csv，第 1 行为表头，以后每行输出一条数据
 """)
-parser.add_argument("-o", "--output-file", help="保存到文件，此时命令行会输出进度条")
-parser.add_argument("-m", "--min-depth", default=0, type=int, help="最小深度，默认值 0，小于 0 时不限")
-parser.add_argument("-M", "--max-depth", default=-1, type=int, help="最大深度，默认值 -1，小于 0 时不限")
-parser.add_argument("-dfs", "--depth-first", action="store_true", help="使用深度优先搜索，否则使用广度优先")
-parser.add_argument("-fl", "--follow-symlinks", action="store_true", help="是否跟进符号连接（如果为否，则会把符号链接视为文件，即使它指向目录）")
-parser.add_argument("-v", "--version", action="store_true", help="输出版本号")
-args = parser.parse_args()
-if args.version:
-    print(".".join(map(str, __version__)))
-    raise SystemExit(0)
-
-from collections.abc import Callable, Iterator
-from os import fsdecode, lstat, stat, stat_result, PathLike
-from os.path import abspath, isdir, islink, relpath
-from operator import attrgetter
-from pathlib import Path
-from sys import stdout
-from typing import Optional
-
-STAT_FIELDS = tuple(
-    f for f in dir(stat_result) 
-    if f.startswith("st_")
-)
-
-def stat_to_dict(
-    path: None | bytes | str | PathLike = None, 
-    /, 
-    follow_symlinks: bool = False, 
-) -> Optional[dict]:
-    getstat: Callable[[bytes | str | PathLike], stat_result]
-    if follow_symlinks:
-        getstat = stat
-    else:
-        getstat = lstat
-    try:
-        return dict(zip(
-            STAT_FIELDS, 
-            attrgetter(*STAT_FIELDS)(getstat(path or ".")), 
-        ))
-    except OSError:
-        return None
-
-select = args.select
-predicate: Optional[Callable[[DirEntry], Optional[bool]]]
-if select:
-    if select.startswith("lambda "):
-        pred = eval(select)
+parser_iter.add_argument("-o", "--output-file", help="保存到文件，此时命令行会输出进度条")
+parser_iter.add_argument("-dfs", "--depth-first", action="store_true", help="使用深度优先搜索，否则使用广度优先")
+parser_iter.add_argument("-fl", "--follow-symlinks", action="store_true", help="是否跟进符号连接（如果为否，则会把符号链接视为文件，即使它指向目录）")
+
+def main_iter(args):
+    from iterdir import __version__, iterdir, DirEntry
+
+    if args.version:
+        print(".".join(map(str, __version__)))
+        raise SystemExit(0)
+
+    from collections.abc import Callable, Iterator
+    from os import fsdecode, lstat, stat, stat_result, PathLike
+    from os.path import abspath, isdir, islink, relpath
+    from operator import attrgetter
+    from pathlib import Path
+    from sys import stdout
+    from typing import Optional
+
+    STAT_FIELDS = tuple(
+        f for f in dir(stat_result) 
+        if f.startswith("st_")
+    )
+
+    def stat_to_dict(
+        path: None | bytes | str | PathLike = None, 
+        /, 
+        follow_symlinks: bool = False, 
+    ) -> Optional[dict]:
+        getstat: Callable[[bytes | str | PathLike], stat_result]
+        if follow_symlinks:
+            getstat = stat
+        else:
+            getstat = lstat
+        try:
+            return dict(zip(
+                STAT_FIELDS, 
+                attrgetter(*STAT_FIELDS)(getstat(path or ".")), 
+            ))
+        except OSError:
+            return None
+
+    select = args.select
+    predicate: Optional[Callable[[DirEntry], Optional[bool]]]
+    if select:
+        if select.startswith("lambda "):
+            pred = eval(select)
+        else:
+            pred = eval("lambda path:" + select)
+        predicate = lambda e: pred(Path(fsdecode(e)))
     else:
-        pred = eval("lambda path:" + select)
-    predicate = lambda e: pred(Path(fsdecode(e)))
-else:
-    predicate = None
-
-path = args.path
-top = abspath(path)
-fmap: dict[str, Callable] = {
-    "inode": DirEntry.inode, 
-    "name": lambda e: e.name, 
-    "path": lambda e: e.path, 
-    "relpath": lambda e: relpath(abspath(e), top), 
-    "isdir": isdir, 
-    "islink": islink, 
-    "stat": stat_to_dict, 
-}
-
-keys = args.keys or KEYS
-if keys:
-    fmap = {k: fmap[k] for k in keys if k in fmap}
-
-path_it: Iterator[DirEntry] = iterdir(
-    DirEntry(path), 
-    topdown=True if args.depth_first else None, 
-    min_depth=args.min_depth, 
-    max_depth=args.max_depth, 
-    predicate=predicate, 
-    follow_symlinks=args.follow_symlinks, 
-)
-
-output_file = args.output_file
-if output_file:
-    from collections import deque
-    from time import perf_counter
-
-    def format_time(t):
-        m, s = divmod(t, 60)
-        if m < 60:
-            return f"{m:02.0f}:{s:09.06f}"
-        h, m = divmod(m, 60)
-        if h < 24:
-            return f"{h:02.0f}:{m:02.0f}:{s:09.06f}"
-        d, h = divmod(h, 60)
-        return f"{d}d{h:02.0f}:{m:02.0f}:{s:09.06f}"
-
-    def progress(it):
-        write = stdout.buffer.raw.write # type: ignore
-        dq: deque[tuple[int, float]] = deque(maxlen=10*60)
-        push = dq.append
-        total = 0
-        ndirs = 0
-        nfiles = 0
-        start_t = last_t = perf_counter()
-        write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles}".encode())
-        push((total, start_t))
-        for p in it:
-            total += 1
-            if p.is_dir():
-                ndirs += 1
-            else:
-                nfiles += 1
+        predicate = None
+
+    path = args.path
+    top = abspath(path)
+    fmap: dict[str, Callable] = {
+        "inode": DirEntry.inode, 
+        "name": lambda e: e.name, 
+        "path": lambda e: e.path, 
+        "relpath": lambda e: relpath(abspath(e), top), 
+        "isdir": isdir, 
+        "islink": islink, 
+        "stat": stat_to_dict, 
+    }
+
+    keys = args.keys or KEYS
+    if keys:
+        fmap = {k: fmap[k] for k in keys if k in fmap}
+
+    path_it: Iterator[DirEntry] = iterdir(
+        DirEntry(path), 
+        topdown=True if args.depth_first else None, 
+        min_depth=args.min_depth, 
+        max_depth=args.max_depth, 
+        predicate=predicate, 
+        follow_symlinks=args.follow_symlinks, 
+    )
+
+    output_file = args.output_file
+    if output_file:
+        from collections import deque
+        from time import perf_counter
+
+        def format_time(t):
+            m, s = divmod(t, 60)
+            if m < 60:
+                return f"{m:02.0f}:{s:09.06f}"
+            h, m = divmod(m, 60)
+            if h < 24:
+                return f"{h:02.0f}:{m:02.0f}:{s:09.06f}"
+            d, h = divmod(h, 60)
+            return f"{d}d{h:02.0f}:{m:02.0f}:{s:09.06f}"
+
+        def progress(it):
+            write = stdout.buffer.raw.write # type: ignore
+            dq: deque[tuple[int, float]] = deque(maxlen=10*60)
+            push = dq.append
+            total = 0
+            ndirs = 0
+            nfiles = 0
+            start_t = last_t = perf_counter()
+            write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles}".encode())
+            push((total, start_t))
+            for p in it:
+                total += 1
+                if p.is_dir():
+                    ndirs += 1
+                else:
+                    nfiles += 1
+                cur_t = perf_counter()
+                if cur_t - last_t > 0.1:
+                    speed = (total - dq[0][0]) / (cur_t - dq[0][1])
+                    write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles} | 🕙 {format_time(cur_t-start_t)} | 🚀 {speed:.3f} it/s".encode())
+                    push((total, cur_t))
+                    last_t = cur_t
+                yield p
             cur_t = perf_counter()
-            if cur_t - last_t > 0.1:
-                speed = (total - dq[0][0]) / (cur_t - dq[0][1])
-                write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles} | 🕙 {format_time(cur_t-start_t)} | 🚀 {speed:.3f} it/s".encode())
-                push((total, cur_t))
-                last_t = cur_t
-            yield p
-        cur_t = perf_counter()
-        speed = total / (cur_t - start_t)
-        write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles} | 🕙 {format_time(cur_t-start_t)} | 🚀 {speed:.3f} it/s".encode())
-    file = open(output_file, "w")
-    path_it = iter(progress(path_it))
-else:
-    file = stdout # type: ignore
-
-records = ({k: f(e) for k, f in fmap.items()} for e in path_it)
-
-output_type = args.output_type
-dumps: Callable[..., bytes]
-if output_type in ("log", "json"):
-    try:
-        from orjson import dumps
-    except ImportError:
-        odumps: Callable
+            speed = total / (cur_t - start_t)
+            write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles} | 🕙 {format_time(cur_t-start_t)} | 🚀 {speed:.3f} it/s".encode())
+        file = open(output_file, "w")
+        path_it = iter(progress(path_it))
+    else:
+        file = stdout # type: ignore
+
+    records = ({k: f(e) for k, f in fmap.items()} for e in path_it)
+
+    output_type = args.output_type
+    dumps: Callable[..., bytes]
+    if output_type in ("log", "json"):
         try:
-            from ujson import dumps as odumps
+            from orjson import dumps
         except ImportError:
-            from json import dumps as odumps
-        dumps = lambda obj, /: bytes(odumps(obj, ensure_ascii=False), "utf-8")
-    if output_file:
-        write = file.buffer.write
-    else:
-        write = file.buffer.raw.write # type: ignore
+            odumps: Callable
+            try:
+                from ujson import dumps as odumps
+            except ImportError:
+                from json import dumps as odumps
+            dumps = lambda obj, /: bytes(odumps(obj, ensure_ascii=False), "utf-8")
+        if output_file:
+            write = file.buffer.write
+        else:
+            write = file.buffer.raw.write # type: ignore
 
-try:
-    if output_type == "json":
-        write(b"[")
-        for i, record in enumerate(records):
-            if i:
-                write(b", ")
-            write(dumps(record))
-        write(b"]")
-    elif output_type == "log":
-        for record in records:
-            write(dumps(record))
-            write(b"\n")
+    try:
+        if output_type == "json":
+            write(b"[")
+            for i, record in enumerate(records):
+                if i:
+                    write(b", ")
+                write(dumps(record))
+            write(b"]")
+        elif output_type == "log":
+            for record in records:
+                write(dumps(record))
+                write(b"\n")
+        else:
+            from csv import DictWriter
+
+            writer = DictWriter(file, fieldnames=keys)
+            writer.writeheader()
+            for record in records:
+                writer.writerow(record)
+    except KeyboardInterrupt:
+        pass
+    except BrokenPipeError:
+        from sys import stderr
+        stderr.close()
+    finally:
+        file.close()
+
+parser_iter.set_defaults(func=main_iter)
+
+parser_stats = subparsers.add_parser("stats", description="目录树遍历统计")
+
+parser_stats.add_argument("path", nargs="?", default="", help="文件夹路径，默认为当前工作目录")
+parser_stats.add_argument("-m", "--min-depth", default=0, type=int, help="最小深度，默认值 0，小于 0 时不限")
+parser_stats.add_argument("-M", "--max-depth", default=-1, type=int, help="最大深度，默认值 -1，小于 0 时不限")
+parser_stats.add_argument("-v", "--version", action="store_true", help="输出版本号")
+
+def main_stats(args):
+    from iterdir import __version__, DirEntry, statsdir
+
+    if args.version:
+        print(".".join(map(str, __version__)))
+        raise SystemExit(0)
+
+    from collections.abc import Callable
+    from os import fsdecode
+    from pathlib import Path
+    from typing import Optional
+
+    select = args.select
+    predicate: Optional[Callable[[DirEntry], Optional[bool]]]
+    if select:
+        if select.startswith("lambda "):
+            pred = eval(select)
+        else:
+            pred = eval("lambda path:" + select)
+        predicate = lambda e: pred(Path(fsdecode(e)))
     else:
-        from csv import DictWriter
+        predicate = None
+
+    print(statsdir(
+        args.path, 
+        min_depth=args.min_depth, 
+        max_depth=args.max_depth, 
+        predicate=predicate, 
+    ))
 
-        writer = DictWriter(file, fieldnames=keys)
-        writer.writeheader()
-        for record in records:
-            writer.writerow(record)
-except KeyboardInterrupt:
-    pass
-except BrokenPipeError:
-    from sys import stderr
-    stderr.close()
-finally:
-    file.close()
+parser_stats.set_defaults(func=main_stats)
+
+args = parser.parse_args()
+args.func(args)
```

### Comparing `iterdir-0.0.3.1/pyproject.toml` & `iterdir-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iterdir"
-version = "0.0.3.1"
+version = "0.0.4"
 description = "iterdir."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 keywords = ["iterdir", "traverse"]
@@ -21,13 +21,16 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE",
 ]
 
+[tool.poetry.dependencies]
+python = "^3.10"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
 include = "iterdir"
```

### Comparing `iterdir-0.0.3.1/readme.md` & `iterdir-0.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.3.1/PKG-INFO` & `iterdir-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: iterdir
-Version: 0.0.3.1
+Version: 0.0.4
 Summary: iterdir.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir
 License: MIT
 Keywords: iterdir,traverse
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

