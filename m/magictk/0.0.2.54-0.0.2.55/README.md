# Comparing `tmp/magictk-0.0.2.54.tar.gz` & `tmp/magictk-0.0.2.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.54.tar", last modified: Fri Apr 26 01:09:12 2024, max compression
+gzip compressed data, was "magictk-0.0.2.55.tar", last modified: Fri Apr 26 01:36:38 2024, max compression
```

## Comparing `magictk-0.0.2.54.tar` & `magictk-0.0.2.55.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 01:09:12.358843 magictk-0.0.2.54/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-26 01:09:11.000000 magictk-0.0.2.54/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-26 01:09:12.358843 magictk-0.0.2.54/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-26 01:09:11.000000 magictk-0.0.2.54/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 01:09:12.358843 magictk-0.0.2.54/magictk/
--rw-r--r--   0 root         (0) root         (0)      442 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3285 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    17051 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11247 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12242 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)     3725 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)     1890 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/icon.py
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5995 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     8106 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/scrollbar.py
--rw-r--r--   0 root         (0) root         (0)     6178 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10245 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-26 01:09:11.000000 magictk-0.0.2.54/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 01:09:12.358843 magictk-0.0.2.54/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-26 01:09:12.000000 magictk-0.0.2.54/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      610 2024-04-26 01:09:12.000000 magictk-0.0.2.54/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 01:09:12.000000 magictk-0.0.2.54/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-26 01:09:12.000000 magictk-0.0.2.54/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 01:09:12.358843 magictk-0.0.2.54/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-26 01:09:11.000000 magictk-0.0.2.54/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 01:36:38.361008 magictk-0.0.2.55/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-26 01:36:37.000000 magictk-0.0.2.55/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-26 01:36:38.361008 magictk-0.0.2.55/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1683 2024-04-26 01:36:37.000000 magictk-0.0.2.55/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 01:36:38.361008 magictk-0.0.2.55/magictk/
+-rw-r--r--   0 root         (0) root         (0)      442 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    17051 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11247 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12242 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/icon.py
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5995 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     8106 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/scrollbar.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10245 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-26 01:36:37.000000 magictk-0.0.2.55/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 01:36:38.361008 magictk-0.0.2.55/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-26 01:36:38.000000 magictk-0.0.2.55/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      610 2024-04-26 01:36:38.000000 magictk-0.0.2.55/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 01:36:38.000000 magictk-0.0.2.55/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-26 01:36:38.000000 magictk-0.0.2.55/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 01:36:38.361008 magictk-0.0.2.55/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-26 01:36:37.000000 magictk-0.0.2.55/setup.py
```

### Comparing `magictk-0.0.2.54/PKG-INFO` & `magictk-0.0.2.55/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.54
+Version: 0.0.2.55
 Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.54/README.md` & `magictk-0.0.2.55/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,73 @@
-![icon](http://git.hmtsai.cn/cxykevin/magictk-img-readme/raw/branch/master/icon.ico)
-#                  magictk
-### 一个模仿 [element plus](https://element-plus.org/) 的 tkinter 组件库
+# magictk
+
+![icon](https://git.hmtsai.cn/cxykevin/magictk-img-readme/raw/branch/master/icon.ico)
+> 一个模仿 [element plus](https://element-plus.org/) 的 tkinter 组件库
 
 ## 演示
-<video width="420" height="240" controls="" src="/cxykevin/magictk-img-readme/raw/branch/master/2024-04-05_show.mp4">
-<strong>您的浏览器不支持使用 HTML5 'video' 标签。</strong>
-</video>
 
-## 依赖
+<video width="420" height="240" controls="" src="/cxykevin/magictk-img-readme/raw/branch/master/2024-04-05_show.mp4">您的浏览器不支持使用 HTML5 'video' 标签</video>
+
+## 依赖/需求
+
+- `python` >= 3.8
 - `pywin32` (Only in `Windows`)
 
+## 安装
+
+### pip
+
+任选其一
+
+``` bash
+pip install magictk -i https://pypi.org/simple
+
+pip install --index-url http://git.hmtsai.cn/api/packages/cxykevin/pypi/simple magictk
+```
+
+### 源码安装
+
+1. clone 本仓库
+2. 运行setup.py
+
+   ``` bash
+   python setup.py install
+   ```
+
 ## 性能
+
 测试机器：  
+
 - Arch Linux x86_64
 - Wayland + KDE Plasma
 - Intel Celeron G1840 (2) @ `2.800GHz`
 - Intel HD Graphics
 - Memory: `11665MiB`
 - htop
 
 CPU 占用：
+
 - 单窗口约 `20%`
+
 > 非最新数据
 
 Memory 占用：
+
 - 约 `50 MiB`
 
 > 性能测试会消耗 `200` MiB 内存, Tim Sort `sort()` 1e7 随机数据 测试
 
 ## 组件
+
 > 以下组件按完成时间从上(早)到下(晚)排序
+
 1. `Window`
-  > 在 Linux 下存在强制置顶问题，且最大化存在问题
-  > OSX 未经过测试
+  (在 Linux 下存在强制置顶问题，且最大化存在问题
+  OSX 未经过测试)
 2. `Button`
 3. `ProgressBar`
-4. `CheckBox` (`Radio`)
-  > `Radio` 可以使用 `Checkbox` 指定 `RadioGroup` 实现
+4. `CheckBox` (可以使用 `Checkbox` 指定 `RadioGroup` 实现 `Radio`)
 5. `Menu`
 6. `Select`
-7. `Frame`
-  > 所有组件必须配合自定义的 `Frame` 使用，因为 `Frame` 携带 `root` 信息(可手动指定)
-8. `Input`
-  > 在 `Linux` 下会弹出一个空窗口(如果没有这个窗口无法输入，原理尚不清楚)
----
-
-以下为计划开发顺序：
-9. `ScrollBar`
+7. `Frame` (所有组件必须配合自定义的 `Frame` 使用，因为 `Frame` 携带 `root` 信息，可手动指定)
+8. `Input`  (在 `Linux` 下会弹出一个空窗口(如果没有这个窗口无法输入，原理尚不清楚))
+9. `ScrollBar` (在多重嵌套时滚轮事件绑定稍有问题，在控件上绑定失效)
```

### Comparing `magictk-0.0.2.54/magictk/_window_ctl.py` & `magictk-0.0.2.55/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/_window_size.py` & `magictk-0.0.2.55/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/basicwindow.py` & `magictk-0.0.2.55/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/button.py` & `magictk-0.0.2.55/magictk/button.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/checkbox.py` & `magictk-0.0.2.55/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/color_tmpl.py` & `magictk-0.0.2.55/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/entry.py` & `magictk-0.0.2.55/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/fontconfig.py` & `magictk-0.0.2.55/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/frame.py` & `magictk-0.0.2.55/magictk/frame.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/icon.ico` & `magictk-0.0.2.55/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/icon.py` & `magictk-0.0.2.55/magictk/icon.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/photoload.py` & `magictk-0.0.2.55/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/progressbar.py` & `magictk-0.0.2.55/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/res.pickle` & `magictk-0.0.2.55/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/scrollbar.py` & `magictk-0.0.2.55/magictk/scrollbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/select.py` & `magictk-0.0.2.55/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/submenu.py` & `magictk-0.0.2.55/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/window.py` & `magictk-0.0.2.55/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk/workspace.py` & `magictk-0.0.2.55/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/magictk.egg-info/PKG-INFO` & `magictk-0.0.2.55/magictk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.54
+Version: 0.0.2.55
 Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.54/magictk.egg-info/SOURCES.txt` & `magictk-0.0.2.55/magictk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.54/setup.py` & `magictk-0.0.2.55/setup.py`

 * *Files identical despite different names*

