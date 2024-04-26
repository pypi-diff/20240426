# Comparing `tmp/pytexmk-0.4.3.240405.tar.gz` & `tmp/pytexmk-0.5.0.240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytexmk-0.4.3.240405.tar", last modified: Fri Apr  5 01:10:10 2024, max compression
+gzip compressed data, was "pytexmk-0.5.0.240426.tar", last modified: Fri Apr 26 14:49:18 2024, max compression
```

## Comparing `pytexmk-0.4.3.240405.tar` & `pytexmk-0.5.0.240426.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)    35149 2024-02-28 15:10:35.000000 pytexmk-0.4.3.240405/LICENSE
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       30 2024-03-06 03:27:48.000000 pytexmk-0.4.3.240405/MANIFEST.in
--rw-rw-r--   0 yanming   (1000) yanming   (1000)      466 2024-03-06 03:27:48.000000 pytexmk-0.4.3.240405/Makefile
--rw-r--r--   0 yanming   (1000) yanming   (1000)     7406 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/PKG-INFO
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     6360 2024-03-22 06:40:11.000000 pytexmk-0.4.3.240405/README.md
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1195 2024-03-21 15:51:11.000000 pytexmk-0.4.3.240405/pyproject.toml
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       38 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/setup.cfg
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-05 01:10:10.307703 pytexmk-0.4.3.240405/src/
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/src/pytexmk/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1940 2024-02-29 11:40:30.000000 pytexmk-0.4.3.240405/src/pytexmk/__init__.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     9617 2024-04-05 01:04:06.000000 pytexmk-0.4.3.240405/src/pytexmk/__main__.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     8126 2024-04-05 00:55:30.000000 pytexmk-0.4.3.240405/src/pytexmk/additional_operation.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     9922 2024-03-22 06:51:11.000000 pytexmk-0.4.3.240405/src/pytexmk/compile_model.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     5896 2024-03-22 06:50:52.000000 pytexmk-0.4.3.240405/src/pytexmk/info_print.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1922 2024-04-05 01:06:45.000000 pytexmk-0.4.3.240405/src/pytexmk/version.py
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/src/pytexmk.egg-info/
--rw-r--r--   0 yanming   (1000) yanming   (1000)     7406 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/PKG-INFO
--rw-rw-r--   0 yanming   (1000) yanming   (1000)      441 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/SOURCES.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)        1 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/dependency_links.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       41 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/entry_points.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       13 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/requires.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)        8 2024-04-05 01:10:10.000000 pytexmk-0.4.3.240405/src/pytexmk.egg-info/top_level.txt
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-05 01:10:10.311704 pytexmk-0.4.3.240405/tests/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     9643 2024-03-22 06:30:29.000000 pytexmk-0.4.3.240405/tests/test.py
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)    35149 2024-02-28 15:10:35.000000 pytexmk-0.5.0.240426/LICENSE
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       30 2024-03-06 03:27:48.000000 pytexmk-0.5.0.240426/MANIFEST.in
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)      466 2024-03-06 03:27:48.000000 pytexmk-0.5.0.240426/Makefile
+-rw-r--r--   0 yanming   (1000) yanming   (1000)     9034 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/PKG-INFO
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     7988 2024-04-26 14:37:00.000000 pytexmk-0.5.0.240426/README.md
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     1195 2024-03-21 15:51:11.000000 pytexmk-0.5.0.240426/pyproject.toml
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       38 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/setup.cfg
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 14:49:18.817467 pytexmk-0.5.0.240426/src/
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/src/pytexmk/
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     1940 2024-02-29 11:40:30.000000 pytexmk-0.5.0.240426/src/pytexmk/__init__.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)    11483 2024-04-26 14:44:17.000000 pytexmk-0.5.0.240426/src/pytexmk/__main__.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)    10195 2024-04-26 14:32:56.000000 pytexmk-0.5.0.240426/src/pytexmk/additional_operation.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     9922 2024-03-22 06:51:11.000000 pytexmk-0.5.0.240426/src/pytexmk/compile_model.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     5896 2024-03-22 06:50:52.000000 pytexmk-0.5.0.240426/src/pytexmk/info_print.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     1922 2024-04-26 14:37:34.000000 pytexmk-0.5.0.240426/src/pytexmk/version.py
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/src/pytexmk.egg-info/
+-rw-r--r--   0 yanming   (1000) yanming   (1000)     9034 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/PKG-INFO
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)      441 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/SOURCES.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)        1 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/dependency_links.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       41 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/entry_points.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       13 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/requires.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)        8 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/top_level.txt
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/tests/
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     9643 2024-03-22 06:30:29.000000 pytexmk-0.5.0.240426/tests/test.py
```

### Comparing `pytexmk-0.4.3.240405/LICENSE` & `pytexmk-0.5.0.240426/LICENSE`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.3.240405/PKG-INFO` & `pytexmk-0.5.0.240426/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: pytexmk
-Version: 0.4.3.240405
-Summary: LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool
-Author-email: 焱铭 <lxb-yanming@foxmail.com>
-Project-URL: Homepage, https://github.com/YanMing-lxb/PyTeXMK
-Project-URL: Bug Tracker, https://github.com/YanMing-lxb/PyTeXMK/issues
-Keywords: LaTeX,build,latexmk
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers 
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: rich
-Requires-Dist: pymupdf
-
 <!--
  *  =======================================================================
  *  ····Y88b···d88P················888b·····d888·d8b·······················
  *  ·····Y88b·d88P·················8888b···d8888·Y8P·······················
  *  ······Y88o88P··················88888b·d88888···························
  *  ·······Y888P··8888b···88888b···888Y88888P888·888·88888b·····d88b·······
  *  ········888······"88b·888·"88b·888·Y888P·888·888·888·"88b·d88P"88b·····
@@ -37,15 +12,15 @@
  *  ··························································Y8b·d88P·····
  *  ···························································"Y88P"······
  *  =======================================================================
  * 
  *  -----------------------------------------------------------------------
  * Author       : 焱铭
  * Date         : 2024-02-29 10:23:19 +0800
- * LastEditTime : 2024-03-22 14:39:36 +0800
+ * LastEditTime : 2024-04-26 22:37:00 +0800
  * Github       : https://github.com/YanMing-lxb/
  * FilePath     : /PyTeXMK/README.md
  * Description  : 
  *  -----------------------------------------------------------------------
  -->
 
 # PyTeXMK
@@ -70,18 +45,19 @@
 
 ```
 pip3 install --upgrade pytexmk
 ```
 
 ## 使用入门
 
-PyTeXMK 默认使用 `xelatex` 编译，默认主文件名为 main（如果不是 main 就在 `pytexmk` 命令后添加文件名），默认 batch 模式编译，编译过程信息不显示（如需显示编译过程信息请使用 `-nq` 参数），默认将编译结果存放在 LaTeX 项目的 Build 文件夹下 ( VSCode 用户则需要在 `settings.json` 中注意设置 `"latex-workshop.latex.outDir": "./Build",` 使得latex workshop 能够找到pdf )。
+PyTeXMK 默认参数：`xelatex` 编译、主文件名 main、batch 模式（编译过程信息不显，如需显示编译过程信息请使用 `-nq` 参数）、编译结果存放在 LaTeX 项目的 Build 文件夹下 ( VSCode 用户则需要在 `settings.json` 中注意设置 `"latex-workshop.latex.outDir": "./Build",` 使得latex workshop 能够找到pdf )。
 
-在终端打开 LaTeX 项目所在文件夹，输入 `pytexmk` 即可使用默认参数进行编译，编译结果默认存放在 LaTeX 项目的 Build 文件夹下。
+请仔细阅读：[主文件及编译类型选定逻辑](#主文件及编译类型选定逻辑)
 
+### 编译命令
 PyTeXMK 支持：
 
 - 编译命令：`xelatex` `pdflatex` `lualatex`
 - 参考文献：`bibtex` `biblatex` `thebibliography`
 - 符号索引：`glossaries` `nomencl` `mkeidx`
 
 位置参数:
@@ -101,22 +77,51 @@
 | -C, --Clean      | 清除所有辅助文件和 pdf 文件                    |
 | -nq, --no-quiet  | 非安静模式运行，此模式下显示编译过程             |
 | -cp, --clean-pdf  | 清理所有 pdf 文件             |
 
 **说明：**
 `-cp` 参数的功能是 "当 LaTeX 编译过程中报类似 `invalid X X R object at offset XXXXX` 的警告时，可使用此参数清理所有 pdf 文件"
 
+### 魔法注释
+
+PyTeXMK 支持使用魔法注释来自定义编译命令、编译类型、编译结果存放位置等。    
+
+| Magic Comment | Description                                |
+|---------------|----------|
+| `% !TEX program = xelatex` | 指定编译类型，可选 `xelatex` `pdflatex` `lualatex` |
+| `% !TEX root = file.tex` | 指定主 LaTeX 文件名，仅支持主文件在项目根目录下的情况 |
+| `% !TEX outdir = PDFfile` | 指定编译结果存放位置，仅支持文件夹名称，如果使用 LaTeX-Workshop，则需要在 `settings.json` 中设置 `"latex-workshop.latex.outDir": "./PDFfile",` |
+
+### 主文件及编译类型选定逻辑
+- PyTeXMK 优先使用终端输入命令 `-p` `-x` `-l` 参数指定的编译类型，如果没有指定，则会使用 `% !TEX program = xelatex` 指定的编译类型，如果没有指定，则会使用默认的编译类型 `xelatex`
+- PyTeXMK 主文件选定逻辑顺序：
+    1. 使用终端输入的文件名
+    2. 使用 `% !TEX root = file.tex` 指定的主 LaTeX 文件名
+    3. 使用默认的主文件名 `main`
+    4. 检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
+    5. 根目录下 TeX 文件中只有一个文件，则选择该文件作为主文件
+        
+- PyTeXMK 会优先使用 `% !TEX outdir = PDFfile` 指定的编译结果存放位置，如果没有指定，则会使用默认的编译结果存放位置 `Build`
+
 # 更新日志
 
 - 2024-03-22 完善编译过程出错后的中断处理机制：在编译过程中出现错误时，程序会自动中断，并提示 `请用 -nq 模式运行以显示错误信息！`,使用 `-nq` 参数运行时，则会显示错误信息。
+- 2024-04-26 增加：
+    1. 魔法注释功能，使得用户可以自定义编译命令、编译类型、编译结果存放位置等
+    2. 完善主文件及编译类型选定逻辑
+
 
 # 未来工作方向
 
 - [X] 完善编译过程出错后的中断处理机制
 - [ ] 完善检索主 LaTeX 文件的功能：
-    - [ ] 根据魔法注释 `% !TEX root = relative/or/absolute/path/to/root/file.tex` 找到主 LaTeX 文件
+    - [X] 根据魔法注释 `% !TEX root = file.tex` 找到主 LaTeX 文件
     - [ ] 通过检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
 - [ ] 完善自动判断编译类型：
-    - [ ] 根据魔法注释 `% !TEX program = xelatex` 设置需要编译的类型
+    - [X] 根据魔法注释 `% !TEX program = xelatex` 设置需要编译的类型
+- [x] 通过魔法注释设置编译结果存放位置
+- [X] 通过魔法注释实现编译命令的自定义
 - [ ] 增加配置文件功能，用于改变默认设置
     - [ ] 指定生成的结果文件存放位置（目前默认存放在 `Build` 子文件夹下）
     - [ ] 默认的编译命令（目前默认编译命令是 `xelatex`）
+- [ ] texlive 宏包检缺失并自动安装
+- [ ] 多主文件编译功能
```

### Comparing `pytexmk-0.4.3.240405/pyproject.toml` & `pytexmk-0.5.0.240426/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.3.240405/src/pytexmk/__init__.py` & `pytexmk-0.5.0.240426/src/pytexmk/__init__.py`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.3.240405/src/pytexmk/__main__.py` & `pytexmk-0.5.0.240426/src/pytexmk/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,32 +12,32 @@
  ··························································Y8b·d88P·····
  ···························································"Y88P"······
  =======================================================================
 
  -----------------------------------------------------------------------
 Author       : 焱铭
 Date         : 2024-02-28 23:11:52 +0800
-LastEditTime : 2024-04-05 09:03:28 +0800
+LastEditTime : 2024-04-26 22:43:47 +0800
 Github       : https://github.com/YanMing-lxb/
 FilePath     : /PyTeXMK/src/pytexmk/__main__.py
 Description  : 
  -----------------------------------------------------------------------
 '''
 # -*- coding: utf-8 -*-
 import argparse
 import datetime
 from .version import script_name, __version__
 from .compile_model import compile_tex, compile_bib, compile_index, compile_xdv
-from .additional_operation import remove_aux, remove_result, remove_result_in_root, move_result, search_file, check_file_name, clean_all_pdf
+from .additional_operation import *
 from .info_print import time_count, time_print, print_message
 
 # ================================================================================
 # XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX 整体进行编译 XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
 # ================================================================================
-def compile(start_time,tex_name, file_name, quiet, build_path):
+def compile(start_time,tex_name, file_name, quiet, outdir):
     name_target_list = []
     time_run_list = []
 
     time_run_remove_aux, _ = time_count(remove_aux, file_name) # 清除已有辅助文件
     name_target_list.append("清除旧辅助文件")
     time_run_list.append(time_run_remove_aux)
 
@@ -86,30 +86,31 @@
           "▓" * 33 + " 完成所有编译 " + "▓" * 33 + "\n" +
           "=" * 80 + "\n")
     print(f"文档整体：{tex_name} 编译 {times_extra_complie+1} 次")
     print(f"参考文献：{print_bib}")
     print(f"目录索引：{print_index}")
     print_message("开始执行编译以外的附加命令！")
     
-    time_run_remove_res, _ = time_count(remove_result, build_path) # 清除已有结果文件
+    time_run_remove_res, _ = time_count(remove_result, outdir) # 清除已有结果文件
     name_target_list.append("清除旧结果文件")
     time_run_list.append(time_run_remove_res)
-    time_run_move_res, _ = time_count(move_result, file_name, build_path) # 移动生成结果文件
+    time_run_move_res, _ = time_count(move_result, file_name, outdir) # 移动生成结果文件
     name_target_list.append("移动结果文件")
     time_run_list.append(time_run_move_res)
     time_run_remove_aux, _ = time_count(remove_aux, file_name) # 清除生成辅助文件
     name_target_list.append("清除辅助文件")
     time_run_list.append(time_run_remove_aux)
 
     time_print(start_time, name_target_list, time_run_list) # 打印编译时长统计
 
 def main():
     # ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓ 设置默认 ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓
     tex_name = "xelatex"
-    build_path = "./Build/"
+    outdir = "./Build/"
+    magic_comments_keys = ["program", "root", "outdir"]
     # ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓
 
     start_time = datetime.datetime.now() # 计算开始时间
     
     # --------------------------------------------------------------------------------
     # 定义命令行参数
     # --------------------------------------------------------------------------------
@@ -122,36 +123,62 @@
     parser.add_argument('-C', '--Clean', action='store_true', help="清除所有辅助文件和 pdf 文件")
     parser.add_argument('-nq', '--no-quiet', action='store_true', help="非安静模式运行，此模式下显示编译过程")
     parser.add_argument('-cp', '--clean-pdf', action='store_true', help="清理 pdf 文件，当 LaTeX 编译过程中警告 invalid X X R object 时，可使用此参数清理所有 pdf 文件")
     
     parser.add_argument('document', nargs='?', help="要被编译的文件名")
     args = parser.parse_args()
 
+    tex_files = search_tex_file # 运行 search_tex_file 函数搜索当前目录下所有 tex 文件
+    magic_comments = search_magic_comments(tex_files, magic_comments_keys) # 运行 search_magic_comments 函数搜索 tex_files 列表中是否存在 magic comments
+
+    # --------------------------------------------------------------------------------
+    # 输出文件路径判断
+    # --------------------------------------------------------------------------------
+    if magic_comments['outdir']: # 如果存在 magic comments 且 outdir 存在
+        outdir = magic_comments['outdir'] # 使用 magic comments 中的 outdir 作为输出目录
+        print(f"通过魔法注释找到输出目录为 {outdir}！")
+
+    # --------------------------------------------------------------------------------
+    # 主文件逻辑判断
+    # --------------------------------------------------------------------------------
+    if args.document: # pytexmk 指定 latex 文件
+        file_name = check_file_name(args.document) # check_file_name 函数检查 args.document 参数输入的文件名是否正确
+    else: # pytexmk 未指定 latex 文件
+        if magic_comments['root']: # 如果存在 magic comments 且 root 存在
+            file_name = check_file_name(magic_comments['root']) # 使用 magic comments 中的 root 作为文件名
+            print(f"通过魔法注释找到 {file_name}.tex 文件！")
+        else: # pytexmk 和魔法注释都不存在，使用search_main_file方法搜索主文件
+            file_name = search_main_file(tex_files)
+    # --------------------------------------------------------------------------------
+    # 编译类型判断
+    # --------------------------------------------------------------------------------
     if args.xelatex:
         tex_name = "xelatex"
-    if args.pdflatex:
+    elif args.pdflatex:
         tex_name = "pdflatex"
-    if args.lualatex:
+    elif args.lualatex:
         tex_name = "lualatex"
-        
-    if args.document: # 指定 latex 文件
-        file_name = check_file_name(args.document) # check_file_name 函数检查 args.document 参数输入的文件名是否正确
-    else: # 未指定 latex 文件
-        file_name = search_file() # 运行 search_file 函数判断
+    elif magic_comments['program']: # 如果存在 magic comments 且 program 存在
+        tex_name = magic_comments['program'] # 使用 magic comments 中的 program 作为编译器
+        print(f"通过魔法注释设置编译器为 {tex_name}！")
+
+    # --------------------------------------------------------------------------------
+    # 编译程序运行
+    # --------------------------------------------------------------------------------
 
     if file_name: # 如果存在 file_name
         if args.clean:
             remove_aux(file_name)
         elif args.Clean:
             remove_aux(file_name)
-            remove_result(build_path)
+            remove_result(outdir)
             remove_result_in_root(file_name)
         elif args.clean_pdf:
-            clean_all_pdf('.', build_path, file_name)
+            clean_all_pdf('.', outdir, file_name)
         else:
-            compile(start_time, tex_name, file_name, not args.no_quiet, build_path)
+            compile(start_time, tex_name, file_name, not args.no_quiet, outdir)
             
     
 
 if __name__ == "__main__":
 
     main()
```

### Comparing `pytexmk-0.4.3.240405/src/pytexmk/additional_operation.py` & `pytexmk-0.5.0.240426/src/pytexmk/additional_operation.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  ··························································Y8b·d88P·····
  ···························································"Y88P"······
  =======================================================================
 
  -----------------------------------------------------------------------
 Author       : 焱铭
 Date         : 2024-02-29 16:02:37 +0800
-LastEditTime : 2024-04-05 08:55:30 +0800
+LastEditTime : 2024-04-26 22:32:56 +0800
 Github       : https://github.com/YanMing-lxb/
 FilePath     : /PyTeXMK/src/pytexmk/additional_operation.py
 Description  : 
  -----------------------------------------------------------------------
 '''
 # -*- coding: utf-8 -*-
 import os
@@ -50,18 +50,18 @@
         print("已清除辅助文件！")
     else:
         print("当前没有辅助文件！")
 
 # --------------------------------------------------------------------------------
 # 定义清除已有结果文件
 # --------------------------------------------------------------------------------
-def remove_result(build_path):
-    if os.path.exists(build_path):
-        shutil.rmtree(build_path)  # 删除整个文件夹
-        print(f"已删除 {build_path} 中的旧结果文件！")
+def remove_result(outdir):
+    if os.path.exists(outdir):
+        shutil.rmtree(outdir)  # 删除整个文件夹
+        print(f"已删除 {outdir} 中的旧结果文件！")
     
 def remove_result_in_root(file_name):
     extensions = [".pdf", ".synctex.gz", ".synctex"]
     for ext in extensions:
         file = file_name + ext
         if os.path.exists(file):
             try:
@@ -71,21 +71,21 @@
                 print(f"{file} 未能删除！")
         else:
             print(f"根目录下不存在 {file}")
 
 # --------------------------------------------------------------------------------
 # 定义移动生成文件
 # --------------------------------------------------------------------------------
-def move_result(file_name, build_path):
+def move_result(file_name, outdir):
     result_files = [f"{file_name}{ext}" for ext in [".pdf", ".synctex.gz"]]
-    os.mkdir(build_path)  # 创建空的 build_path 文件夹
+    os.mkdir(outdir)  # 创建空的 outdir 文件夹
     for file in result_files:
         if os.path.exists(file):
-            shutil.move(file, build_path)
-            print(f"{file} 移动到 {build_path}")
+            shutil.move(file, outdir)
+            print(f"{file} 移动到 {outdir}")
         else:
             print(f'{file} 不存在！')
 
 # --------------------------------------------------------------------------------
 # 定义清理所有 pdf 文件
 # --------------------------------------------------------------------------------
 def clean_all_pdf(root_dir, excluded_folder, file_name):
@@ -135,35 +135,65 @@
         print("提示：文件后缀不是.tex")
 
     return file_name_return
 
 # --------------------------------------------------------------------------------
 # 定义 tex 文件检索函数
 # --------------------------------------------------------------------------------
-def search_file():
+def search_tex_file():
     current_path = os.getcwd() # 获取当前路径
     # 遍历当前路径下的所有文件
     tex_files = [file for file in os.listdir(current_path) if file.endswith('.tex')]
+    return tex_files
 
+# --------------------------------------------------------------------------------
+# 定义 tex 主文件检索函数
+# --------------------------------------------------------------------------------
+def search_main_file(tex_files):
+    current_path = os.getcwd() # 获取当前路径
     if tex_files:
+        # 如果存在多个.tex文件
+        if 'main.tex' in tex_files:
+            # 存在名为main.tex的文件
+            file_name = 'main'
+            print(f"找到 {file_name}.tex 文件！")
         # 如果只有一个.tex文件，则直接提取文件名并打印
-        if len(tex_files) == 1:
+        elif len(tex_files) == 1:
             file_name = os.path.splitext(tex_files[0])[0]
             print(f"找到 {file_name}.tex 文件！")
+        elif len(tex_files) > 1:
+            # 存在多个.tex文件，但没有名为main.tex的文件
+            for file_path in tex_files:  # 遍历tex文件列表
+                with open(file_path, 'r') as file:  # 打开文件
+                    for _ in range(200):  # 遍历文件的前200行
+                        line = file.readline()  # 读取一行内容
+                        if "\documentclass" in line or "\begin{document}" in line:
+                            # 找到 \documentclass 或 \begin{document} 指令，提取文件名
+                            file_name = check_file_name(file_path)
+                            print(f"找到 {file_name}.tex 文件！")
         else:
-            # 如果存在多个.tex文件
-            if 'main.tex' in tex_files:
-                # 存在名为main.tex的文件
-                file_name = 'main'
-                print(f"找到 {file_name}.tex 文件！")
-            else:
-                # 不存在名为main.tex的文件，打印所有找到的.tex文件
-                file_name = None
-                print("存在多个 .tex 文件，请添加 main.tex 文件或终端输入：pytexmk <主文件名> 名进行编译")
-                print("例如终端输入: pytexmk test")
+            # 不存在名为main.tex的文件，打印所有找到的.tex文件
+            file_name = None
+            print("存在多个 .tex 文件，请：修改主文件名为 main.tex 或在文件中加入魔法注释 “% !TEX = <主文件名>” 或在终端输入：pytexmk <主文件名> 名进行编译")
+            print("[bold][red]注意：主文件名一定要放在项目根目录下[/red][/bold]")
     else:
         # 不存在.tex文件，打印当前路径并提示
         file_name = None
         print("终端路径下不存在 .tex 文件！请检查终端显示路径是否是项目路径")
         print(f"当前终端路径是：{current_path}")
 
     return file_name
+
+# --------------------------------------------------------------------------------
+# 定义魔法注释检索函数
+# --------------------------------------------------------------------------------
+def search_magic_comments(tex_files, magic_comments_keys):
+    magic_comments = {}  # 创建空字典用于存储结果
+    for file_path in tex_files:  # 遍历tex文件列表
+        with open(file_path, 'r') as file:  # 打开文件
+            for _ in range(50):  # 遍历文件的前50行
+                line = file.readline()  # 读取一行内容
+                for magic_comments_key in magic_comments_keys:  # 遍历关键字列表
+                    if f"% !TEX {magic_comments_key} =" in line:  # 如果关键字出现在这一行
+                        magic_comment = line.split(f"% !TEX {magic_comments_key} = ")[1].strip()  # 提取对应的值
+                        magic_comments[magic_comments_key] = magic_comment  # 将键值对存入字典
+    return magic_comments  # 返回提取的键值对字典
```

### Comparing `pytexmk-0.4.3.240405/src/pytexmk/compile_model.py` & `pytexmk-0.5.0.240426/src/pytexmk/compile_model.py`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.3.240405/src/pytexmk/info_print.py` & `pytexmk-0.5.0.240426/src/pytexmk/info_print.py`

 * *Files identical despite different names*

### Comparing `pytexmk-0.4.3.240405/src/pytexmk/version.py` & `pytexmk-0.5.0.240426/src/pytexmk/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,18 @@
  ··························································Y8b·d88P·····
  ···························································"Y88P"······
  =======================================================================
 
  -----------------------------------------------------------------------
 Author       : 焱铭
 Date         : 2024-03-01 15:52:28 +0800
-LastEditTime : 2024-04-05 08:57:01 +0800
+LastEditTime : 2024-04-26 22:37:34 +0800
 Github       : https://github.com/YanMing-lxb/
 FilePath     : /PyTeXMK/src/pytexmk/version.py
 Description  : 
  -----------------------------------------------------------------------
 '''
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python
 
 script_name = 'PyTeXMK'
-__version__ = '0.4.3.240405'
+__version__ = '0.5.0.240426'
```

### Comparing `pytexmk-0.4.3.240405/src/pytexmk.egg-info/PKG-INFO` & `pytexmk-0.5.0.240426/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytexmk
-Version: 0.4.3.240405
+Version: 0.5.0.240426
 Summary: LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool
 Author-email: 焱铭 <lxb-yanming@foxmail.com>
 Project-URL: Homepage, https://github.com/YanMing-lxb/PyTeXMK
 Project-URL: Bug Tracker, https://github.com/YanMing-lxb/PyTeXMK/issues
 Keywords: LaTeX,build,latexmk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers 
@@ -37,15 +37,15 @@
  *  ··························································Y8b·d88P·····
  *  ···························································"Y88P"······
  *  =======================================================================
  * 
  *  -----------------------------------------------------------------------
  * Author       : 焱铭
  * Date         : 2024-02-29 10:23:19 +0800
- * LastEditTime : 2024-03-22 14:39:36 +0800
+ * LastEditTime : 2024-04-26 22:37:00 +0800
  * Github       : https://github.com/YanMing-lxb/
  * FilePath     : /PyTeXMK/README.md
  * Description  : 
  *  -----------------------------------------------------------------------
  -->
 
 # PyTeXMK
@@ -70,18 +70,19 @@
 
 ```
 pip3 install --upgrade pytexmk
 ```
 
 ## 使用入门
 
-PyTeXMK 默认使用 `xelatex` 编译，默认主文件名为 main（如果不是 main 就在 `pytexmk` 命令后添加文件名），默认 batch 模式编译，编译过程信息不显示（如需显示编译过程信息请使用 `-nq` 参数），默认将编译结果存放在 LaTeX 项目的 Build 文件夹下 ( VSCode 用户则需要在 `settings.json` 中注意设置 `"latex-workshop.latex.outDir": "./Build",` 使得latex workshop 能够找到pdf )。
+PyTeXMK 默认参数：`xelatex` 编译、主文件名 main、batch 模式（编译过程信息不显，如需显示编译过程信息请使用 `-nq` 参数）、编译结果存放在 LaTeX 项目的 Build 文件夹下 ( VSCode 用户则需要在 `settings.json` 中注意设置 `"latex-workshop.latex.outDir": "./Build",` 使得latex workshop 能够找到pdf )。
 
-在终端打开 LaTeX 项目所在文件夹，输入 `pytexmk` 即可使用默认参数进行编译，编译结果默认存放在 LaTeX 项目的 Build 文件夹下。
+请仔细阅读：[主文件及编译类型选定逻辑](#主文件及编译类型选定逻辑)
 
+### 编译命令
 PyTeXMK 支持：
 
 - 编译命令：`xelatex` `pdflatex` `lualatex`
 - 参考文献：`bibtex` `biblatex` `thebibliography`
 - 符号索引：`glossaries` `nomencl` `mkeidx`
 
 位置参数:
@@ -101,22 +102,51 @@
 | -C, --Clean      | 清除所有辅助文件和 pdf 文件                    |
 | -nq, --no-quiet  | 非安静模式运行，此模式下显示编译过程             |
 | -cp, --clean-pdf  | 清理所有 pdf 文件             |
 
 **说明：**
 `-cp` 参数的功能是 "当 LaTeX 编译过程中报类似 `invalid X X R object at offset XXXXX` 的警告时，可使用此参数清理所有 pdf 文件"
 
+### 魔法注释
+
+PyTeXMK 支持使用魔法注释来自定义编译命令、编译类型、编译结果存放位置等。    
+
+| Magic Comment | Description                                |
+|---------------|----------|
+| `% !TEX program = xelatex` | 指定编译类型，可选 `xelatex` `pdflatex` `lualatex` |
+| `% !TEX root = file.tex` | 指定主 LaTeX 文件名，仅支持主文件在项目根目录下的情况 |
+| `% !TEX outdir = PDFfile` | 指定编译结果存放位置，仅支持文件夹名称，如果使用 LaTeX-Workshop，则需要在 `settings.json` 中设置 `"latex-workshop.latex.outDir": "./PDFfile",` |
+
+### 主文件及编译类型选定逻辑
+- PyTeXMK 优先使用终端输入命令 `-p` `-x` `-l` 参数指定的编译类型，如果没有指定，则会使用 `% !TEX program = xelatex` 指定的编译类型，如果没有指定，则会使用默认的编译类型 `xelatex`
+- PyTeXMK 主文件选定逻辑顺序：
+    1. 使用终端输入的文件名
+    2. 使用 `% !TEX root = file.tex` 指定的主 LaTeX 文件名
+    3. 使用默认的主文件名 `main`
+    4. 检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
+    5. 根目录下 TeX 文件中只有一个文件，则选择该文件作为主文件
+        
+- PyTeXMK 会优先使用 `% !TEX outdir = PDFfile` 指定的编译结果存放位置，如果没有指定，则会使用默认的编译结果存放位置 `Build`
+
 # 更新日志
 
 - 2024-03-22 完善编译过程出错后的中断处理机制：在编译过程中出现错误时，程序会自动中断，并提示 `请用 -nq 模式运行以显示错误信息！`,使用 `-nq` 参数运行时，则会显示错误信息。
+- 2024-04-26 增加：
+    1. 魔法注释功能，使得用户可以自定义编译命令、编译类型、编译结果存放位置等
+    2. 完善主文件及编译类型选定逻辑
+
 
 # 未来工作方向
 
 - [X] 完善编译过程出错后的中断处理机制
 - [ ] 完善检索主 LaTeX 文件的功能：
-    - [ ] 根据魔法注释 `% !TEX root = relative/or/absolute/path/to/root/file.tex` 找到主 LaTeX 文件
+    - [X] 根据魔法注释 `% !TEX root = file.tex` 找到主 LaTeX 文件
     - [ ] 通过检索 TeX 文件中的 `\documentclass[]{}` 或 `\begin{document}` 来判断
 - [ ] 完善自动判断编译类型：
-    - [ ] 根据魔法注释 `% !TEX program = xelatex` 设置需要编译的类型
+    - [X] 根据魔法注释 `% !TEX program = xelatex` 设置需要编译的类型
+- [x] 通过魔法注释设置编译结果存放位置
+- [X] 通过魔法注释实现编译命令的自定义
 - [ ] 增加配置文件功能，用于改变默认设置
     - [ ] 指定生成的结果文件存放位置（目前默认存放在 `Build` 子文件夹下）
     - [ ] 默认的编译命令（目前默认编译命令是 `xelatex`）
+- [ ] texlive 宏包检缺失并自动安装
+- [ ] 多主文件编译功能
```

### Comparing `pytexmk-0.4.3.240405/tests/test.py` & `pytexmk-0.5.0.240426/tests/test.py`

 * *Files identical despite different names*

