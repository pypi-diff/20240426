# Comparing `tmp/bcmd-0.0.71.tar.gz` & `tmp/bcmd-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcmd-0.0.71.tar", last modified: Wed Apr 24 06:27:12 2024, max compression
+gzip compressed data, was "bcmd-0.0.72.tar", last modified: Fri Apr 26 07:25:05 2024, max compression
```

## Comparing `bcmd-0.0.71.tar` & `bcmd-0.0.72.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 06:27:12.070712 bcmd-0.0.71/
--rw-rw-rw-   0        0        0       29 2023-09-28 02:51:40.000000 bcmd-0.0.71/MANIFEST.in
--rw-rw-rw-   0        0        0      285 2024-04-24 06:27:12.069476 bcmd-0.0.71/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-08-28 06:50:10.000000 bcmd-0.0.71/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 06:27:12.045830 bcmd-0.0.71/bcmd/
--rw-rw-rw-   0        0        0        0 2023-08-28 06:50:11.000000 bcmd-0.0.71/bcmd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 06:27:12.053342 bcmd-0.0.71/bcmd/common/
--rw-rw-rw-   0        0        0        0 2023-10-10 06:24:00.000000 bcmd-0.0.71/bcmd/common/__init__.py
--rw-rw-rw-   0        0        0     1347 2024-02-28 09:10:56.000000 bcmd-0.0.71/bcmd/common/password.py
--rw-rw-rw-   0        0        0      131 2024-04-23 08:32:30.000000 bcmd-0.0.71/bcmd/main.py
-drwxrwxrwx   0        0        0        0 2024-04-24 06:27:12.068475 bcmd-0.0.71/bcmd/tasks/
--rw-rw-rw-   0        0        0      311 2024-04-24 06:25:36.000000 bcmd-0.0.71/bcmd/tasks/__init__.py
--rw-rw-rw-   0        0        0     3082 2023-10-11 06:16:53.000000 bcmd-0.0.71/bcmd/tasks/bin.py
--rw-rw-rw-   0        0        0     3127 2024-02-28 09:11:35.000000 bcmd-0.0.71/bcmd/tasks/crypto.py
--rw-rw-rw-   0        0        0     3004 2024-03-04 08:51:50.000000 bcmd-0.0.71/bcmd/tasks/debian.py
--rw-rw-rw-   0        0        0     1052 2024-01-24 02:30:52.000000 bcmd-0.0.71/bcmd/tasks/download.py
--rw-rw-rw-   0        0        0      635 2023-09-18 08:06:47.000000 bcmd-0.0.71/bcmd/tasks/json.py
--rw-rw-rw-   0        0        0     2407 2024-02-19 03:06:05.000000 bcmd-0.0.71/bcmd/tasks/jwt.py
--rw-rw-rw-   0        0        0     4528 2024-03-27 02:16:57.000000 bcmd-0.0.71/bcmd/tasks/lib.py
--rw-rw-rw-   0        0        0     4302 2023-09-18 08:06:47.000000 bcmd-0.0.71/bcmd/tasks/math.py
--rw-rw-rw-   0        0        0     1448 2023-09-18 08:06:47.000000 bcmd-0.0.71/bcmd/tasks/mirror.py
--rw-rw-rw-   0        0        0      939 2024-03-27 02:03:22.000000 bcmd-0.0.71/bcmd/tasks/project.py
--rw-rw-rw-   0        0        0      660 2023-09-18 08:06:47.000000 bcmd-0.0.71/bcmd/tasks/proxy.py
--rw-rw-rw-   0        0        0     4738 2024-03-27 02:07:27.000000 bcmd-0.0.71/bcmd/tasks/task.py
--rw-rw-rw-   0        0        0      766 2024-01-24 01:21:39.000000 bcmd-0.0.71/bcmd/tasks/temp.py
--rw-rw-rw-   0        0        0     2586 2023-09-18 08:06:47.000000 bcmd-0.0.71/bcmd/tasks/time.py
--rw-rw-rw-   0        0        0     4127 2024-04-07 07:18:21.000000 bcmd-0.0.71/bcmd/tasks/venv.py
-drwxrwxrwx   0        0        0        0 2024-04-24 06:27:12.069476 bcmd-0.0.71/bcmd.egg-info/
--rw-rw-rw-   0        0        0      285 2024-04-24 06:27:12.000000 bcmd-0.0.71/bcmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2024-04-24 06:27:12.000000 bcmd-0.0.71/bcmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 06:27:12.000000 bcmd-0.0.71/bcmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-24 06:27:12.000000 bcmd-0.0.71/bcmd.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-24 06:27:12.000000 bcmd-0.0.71/bcmd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-24 06:27:12.000000 bcmd-0.0.71/bcmd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      529 2024-04-24 06:26:48.000000 bcmd-0.0.71/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-24 06:27:12.070712 bcmd-0.0.71/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 07:25:05.360708 bcmd-0.0.72/
+-rw-rw-rw-   0        0        0       29 2023-09-28 02:51:40.000000 bcmd-0.0.72/MANIFEST.in
+-rw-rw-rw-   0        0        0      308 2024-04-26 07:25:05.359708 bcmd-0.0.72/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-08-28 06:50:10.000000 bcmd-0.0.72/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 07:25:05.336885 bcmd-0.0.72/bcmd/
+-rw-rw-rw-   0        0        0        0 2023-08-28 06:50:11.000000 bcmd-0.0.72/bcmd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:25:05.343197 bcmd-0.0.72/bcmd/common/
+-rw-rw-rw-   0        0        0        0 2023-10-10 06:24:00.000000 bcmd-0.0.72/bcmd/common/__init__.py
+-rw-rw-rw-   0        0        0     1347 2024-04-26 07:19:59.000000 bcmd-0.0.72/bcmd/common/password.py
+-rw-rw-rw-   0        0        0      131 2024-04-23 08:32:30.000000 bcmd-0.0.72/bcmd/main.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:25:05.357707 bcmd-0.0.72/bcmd/tasks/
+-rw-rw-rw-   0        0        0      311 2024-04-24 06:25:36.000000 bcmd-0.0.72/bcmd/tasks/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-10-11 06:16:53.000000 bcmd-0.0.72/bcmd/tasks/bin.py
+-rw-rw-rw-   0        0        0     3127 2024-02-28 09:11:35.000000 bcmd-0.0.72/bcmd/tasks/crypto.py
+-rw-rw-rw-   0        0        0     3004 2024-03-04 08:51:50.000000 bcmd-0.0.72/bcmd/tasks/debian.py
+-rw-rw-rw-   0        0        0     1052 2024-01-24 02:30:52.000000 bcmd-0.0.72/bcmd/tasks/download.py
+-rw-rw-rw-   0        0        0      635 2023-09-18 08:06:47.000000 bcmd-0.0.72/bcmd/tasks/json.py
+-rw-rw-rw-   0        0        0     2407 2024-02-19 03:06:05.000000 bcmd-0.0.72/bcmd/tasks/jwt.py
+-rw-rw-rw-   0        0        0     4528 2024-03-27 02:16:57.000000 bcmd-0.0.72/bcmd/tasks/lib.py
+-rw-rw-rw-   0        0        0     2857 2024-04-26 07:11:32.000000 bcmd-0.0.72/bcmd/tasks/math.py
+-rw-rw-rw-   0        0        0     1448 2023-09-18 08:06:47.000000 bcmd-0.0.72/bcmd/tasks/mirror.py
+-rw-rw-rw-   0        0        0      939 2024-03-27 02:03:22.000000 bcmd-0.0.72/bcmd/tasks/project.py
+-rw-rw-rw-   0        0        0     1314 2024-04-26 06:53:35.000000 bcmd-0.0.72/bcmd/tasks/proxy.py
+-rw-rw-rw-   0        0        0     4939 2024-04-26 07:03:50.000000 bcmd-0.0.72/bcmd/tasks/task.py
+-rw-rw-rw-   0        0        0      766 2024-01-24 01:21:39.000000 bcmd-0.0.72/bcmd/tasks/temp.py
+-rw-rw-rw-   0        0        0     2586 2023-09-18 08:06:47.000000 bcmd-0.0.72/bcmd/tasks/time.py
+-rw-rw-rw-   0        0        0     4127 2024-04-07 07:18:21.000000 bcmd-0.0.72/bcmd/tasks/venv.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:25:05.358709 bcmd-0.0.72/bcmd.egg-info/
+-rw-rw-rw-   0        0        0      308 2024-04-26 07:25:05.000000 bcmd-0.0.72/bcmd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2024-04-26 07:25:05.000000 bcmd-0.0.72/bcmd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 07:25:05.000000 bcmd-0.0.72/bcmd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-26 07:25:05.000000 bcmd-0.0.72/bcmd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-04-26 07:25:05.000000 bcmd-0.0.72/bcmd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 07:25:05.000000 bcmd-0.0.72/bcmd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      541 2024-04-26 07:24:28.000000 bcmd-0.0.72/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 07:25:05.360708 bcmd-0.0.72/setup.cfg
```

### Comparing `bcmd-0.0.71/bcmd/common/password.py` & `bcmd-0.0.72/bcmd/common/password.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/bin.py` & `bcmd-0.0.72/bcmd/tasks/bin.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/crypto.py` & `bcmd-0.0.72/bcmd/tasks/crypto.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/debian.py` & `bcmd-0.0.72/bcmd/tasks/debian.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/download.py` & `bcmd-0.0.72/bcmd/tasks/download.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/json.py` & `bcmd-0.0.72/bcmd/tasks/json.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/jwt.py` & `bcmd-0.0.72/bcmd/tasks/jwt.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/lib.py` & `bcmd-0.0.72/bcmd/tasks/lib.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/math.py` & `bcmd-0.0.72/bcmd/tasks/math.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from math import nan
 from typing import Final
 
 import typer
 from beni import bcolor, btask
 from beni.bfunc import Counter, syncCall, toFloat
 from prettytable import PrettyTable
 
@@ -39,60 +38,14 @@
             ['B', b, bcolor.magenta(str(dd)), bcolor.magenta('D')],
         ])
     print(table.get_string(header=False))
 
 
 @app.command()
 @syncCall
-async def increase(
-    old: float = typer.Argument(nan, help='原始数值'),
-    new: float = typer.Argument(nan, help='新数值'),
-):
-    '''
-    计算增长率
-
-    例子：beni math increase 123 456
-
-    例子（连续对话）：beni math increase
-    '''
-    if old is not nan and new is not nan:
-        value = (new - old) / old
-        if value > 0:
-            valueStr = bcolor.red(f'{value*100:+,.3f}%')
-        else:
-            valueStr = bcolor.green(f'{value*100:+,.3f}%')
-        table = PrettyTable(
-            title=bcolor.yellow('计算增长率'),
-        )
-        table.add_rows([
-            ['旧数值', f'{old:,}'],
-            ['新数值', f'{new:,}'],
-            ['增长率', valueStr],
-        ])
-        print()
-        print(table.get_string(header=False))
-    elif old is nan and new is nan:
-        while True:
-            print()
-            value = input('输入2个数值，空格分隔，退出输入 [exit] ：').strip()
-            if value == 'exit':
-                break
-            try:
-                ary = value.split(' ')
-                ary = [float(x) for x in ary if x]
-                assert len(ary) == 2, '参数必须要2个数值'
-                increase(ary[0], ary[1])
-            except Exception as e:
-                bcolor.printRed(e)
-    else:
-        btask.abort('参数错误，不传参数，或者传入2个数值参数')
-
-
-@app.command()
-@syncCall
 async def discount(
     values: list[str] = typer.Argument(..., help='每组数据使用#作为分隔符，注意后面的数据不能为0，例：123#500'),
 ):
     '计算折扣，例子：beni math discount 123#500 130#550'
     btask.check(len(values) >= 2, '至少需要提供2组数据用作比较')
 
     class Data:
@@ -131,14 +84,14 @@
             colorFunc = bcolor.green
         elif data.v == maxV:
             colorFunc = bcolor.red
         columns = [
             f'{data.a:,}',
             f'{data.b:,}',
             f'{data.v:,.3f}',
-            f'{data.discount*100:+,.3f}%' if data.discount else '',
+            f'{data.discount * 100:+,.3f}%' if data.discount else '',
         ]
         table.add_column(
             chr(65 + counter()),
             [colorFunc(x) for x in columns],
         )
     print(table.get_string())
```

### Comparing `bcmd-0.0.71/bcmd/tasks/mirror.py` & `bcmd-0.0.72/bcmd/tasks/mirror.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/project.py` & `bcmd-0.0.72/bcmd/tasks/project.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/task.py` & `bcmd-0.0.72/bcmd/tasks/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,19 +123,24 @@
     btask.check(initFile.is_file(), '文件不存在', initFile)
     files = bpath.listFile(tasks_path)
     files = [x for x in files if not x.name.startswith('_')]
     contents = [f'from . import {x.stem}' for x in files]
     contents.insert(0, '# type: ignore')
     contents.append('')
     content = '\n'.join(contents)
-    await bfile.writeText(
-        initFile,
-        content,
-    )
-    print(content)
+    oldContent = await bfile.readText(initFile)
+    if oldContent != content:
+        await bfile.writeText(
+            initFile,
+            content,
+        )
+        bcolor.printYellow(initFile)
+        bcolor.printMagenta(content)
+    else:
+        bcolor.printGreen('无需修改')
 
 
 async def _getBucket():
     ak, sk = await password.getQiniu()
     return QiniuBucket(
         'pytask',
         'http://qiniu-cdn.pytask.com',
```

### Comparing `bcmd-0.0.71/bcmd/tasks/temp.py` & `bcmd-0.0.72/bcmd/tasks/temp.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/time.py` & `bcmd-0.0.72/bcmd/tasks/time.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd/tasks/venv.py` & `bcmd-0.0.72/bcmd/tasks/venv.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/bcmd.egg-info/SOURCES.txt` & `bcmd-0.0.72/bcmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.71/pyproject.toml` & `bcmd-0.0.72/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # https://peps.python.org/pep-0621/#example
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata
 
 [project]
 name = 'bcmd'
-version = '0.0.71'
+version = '0.0.72'
 description = 'Commands for Beni'
 requires-python = '>=3.10'
 keywords = ['benimang', 'beni', 'bcmd']
 authors = [{ name = 'Beni Mang', email = 'benimang@126.com' }]
 maintainers = [{ name = 'Beni Mang', email = 'benimang@126.com' }]
 
 
 dependencies = [
   'benimang==0.5.26',
   'pathspec',
+  'psutil',
 ]
 
 [project.scripts]
 beni = 'bcmd.main:run'
```

