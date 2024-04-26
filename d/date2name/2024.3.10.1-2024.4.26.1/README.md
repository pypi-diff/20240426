# Comparing `tmp/date2name-2024.3.10.1.tar.gz` & `tmp/date2name-2024.4.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "date2name-2024.3.10.1.tar", max compression
+gzip compressed data, was "date2name-2024.4.26.1.tar", max compression
```

## Comparing `date2name-2024.3.10.1.tar` & `date2name-2024.4.26.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35147 2018-02-16 16:47:32.496641 date2name-2024.3.10.1/LICENSE.txt
--rw-r--r--   0        0        0     9395 2021-11-25 14:24:36.264783 date2name-2024.3.10.1/README.org
--rwxr-xr-x   0        0        0    18482 2024-03-10 16:26:53.803291 date2name-2024.3.10.1/date2name/__init__.py
--rw-r--r--   0        0        0     1079 2024-03-10 16:42:20.749879 date2name-2024.3.10.1/pyproject.toml
--rw-r--r--   0        0        0    10214 1970-01-01 00:00:00.000000 date2name-2024.3.10.1/setup.py
--rw-r--r--   0        0        0     9797 1970-01-01 00:00:00.000000 date2name-2024.3.10.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2018-02-16 16:47:32.496641 date2name-2024.4.26.1/LICENSE.txt
+-rw-r--r--   0        0        0     9395 2021-11-25 14:24:36.264783 date2name-2024.4.26.1/README.org
+-rwxr-xr-x   0        0        0    18470 2024-04-26 13:52:55.631823 date2name-2024.4.26.1/date2name/__init__.py
+-rw-r--r--   0        0        0     1128 2024-04-26 13:52:20.330373 date2name-2024.4.26.1/pyproject.toml
+-rw-r--r--   0        0        0    10317 1970-01-01 00:00:00.000000 date2name-2024.4.26.1/setup.py
+-rw-r--r--   0        0        0     9897 1970-01-01 00:00:00.000000 date2name-2024.4.26.1/PKG-INFO
```

### Comparing `date2name-2024.3.10.1/LICENSE.txt` & `date2name-2024.4.26.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `date2name-2024.3.10.1/README.org` & `date2name-2024.4.26.1/README.org`

 * *Files identical despite different names*

### Comparing `date2name-2024.3.10.1/date2name/__init__.py` & `date2name-2024.4.26.1/date2name/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-PROG_VERSION = u"Time-stamp: <2022-01-10 12:56:17 vk>"
+PROG_VERSION = u"Time-stamp: <2024-04-26>"
 
 """
 date2name
 ~~~~~~~~~
 
 This script adds (or removes) datestamps to (or from) file(s)
```

### Comparing `date2name-2024.3.10.1/setup.py` & `date2name-2024.4.26.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 
 packages = \
 ['date2name']
 
 package_data = \
 {'': ['*']}
 
+entry_points = \
+{'console_scripts': ['date2name = date2name:main']}
+
 setup_kwargs = {
     'name': 'date2name',
-    'version': '2024.3.10.1',
+    'version': '2024.4.26.1',
     'description': 'Handling time-stamps and date-stamps in file names',
     'long_description': '* Handling time-stamps and date-stamps in file names\n\n#+BEGIN_HTML\n<a href="https://karl-voit.at/demo-date2name">\n<img src="https://raw.githubusercontent.com/novoid/screencasts/master/file_management/date2name.gif" />\n</a>\n#+END_HTML\n\n[[file:bin/screencast.gif]]\n\nPer default, date2name gets the modification time of matching files\nand directories and adds a datestamp in standard ISO 8601+ format\nYYYY-MM-DD (http://datestamps.org/index.shtml) at the beginning of\nthe file- or directoryname.\n\nIf an existing timestamp is found, its style will be converted to the\nselected ISO datestamp format but the numbers stays the same.\nExecuted with an examplefilename "file" this results e.g. in\n"2008-12-31_file".\n\nNote: Other that defined in ISO 8601+ the delimiter between hours,\nminutes, and seconds is not a colon but a dot. Colons are causing\nseveral problems on different file systems and are there fore replaced\nwith the (older) DIN 5008 version with dots.\n\n: Usage:\n:          date2name [options] file ...\n\nRun "date2name --help" for usage hints such as:\n\n: Options:\n:   -h, --help         show the extended help message and exit\n:   -d, --directories  modify only directory names\n:   -f, --files        modify only file names\n:   -S, --short        use short datestamp               (YYMMDD)\n:   -C, --compact      use compact datestamp             (YYYYMMDD)\n:   -M, --month        use datestamp with year and month (YYYY-MM)\n:   -w, --withtime     use datestamp including seconds   (YYYY-MM-DDThh.mm.ss)\n:   -r, --remove       remove all known datestamps\n:   -m, --mtime        take modification time for datestamp [default]\n:   -c, --ctime        take creation time for datestamp\n:   --delimiter        overwrite default delimiter\n:   --nocorrections    do not convert existing datestamps to new format\n:   -q, --quiet        do not output anything but just errors on console\n:   -v, --verbose      enable verbose mode\n:   -s, --dryrun       enable dryrun mode: just simulate what would happen, do\n:                      not modify files or directories\n:   --version          display version and exit\n\n* Installation\n\nFirst, you need the programming platform [[https://www.python.org/downloads/][Python]] installed.\n\nThen, you can\n\n1. get =date2name= manually from [[https://github.com/novoid/date2name][GitHub]] OR\n2. install it via =pip install date2name= which is simplest method.\n\n* Integration Into Common Tools\n\n** Integration into Windows File Explorer\n\nThe easiest way to integrate =date2name= into File Explorer ("Send to"\ncontext menu) is by using [[https://github.com/novoid/integratethis][integratethis]].\n\nExecute this in your command line environment:\n\n: pip install date2name integratethis\n: integratethis date2name\n: integratethis time2name\n\n*** Manual Integration into Windows Explorer for single files\n\nUse this only if the [[https://github.com/novoid/integratethis][integratethis]] method can not be applied:\n\nCreate a registry file =add_date2name_to_context_menu.reg= and edit it\nto meet the following template. Please make sure to replace the paths\n(python, =USERNAME= and =date2name.py=) accordingly:\n\n#+BEGIN_EXAMPLE\nWindows Registry Editor Version 5.00\n\n;; for files:\n\n[HKEY_CLASSES_ROOT\\*\\shell\\date2name]\n@="date2name (single file)"\n\n[HKEY_CLASSES_ROOT\\*\\shell\\date2name\\command]\n@="C:\\\\Python36\\\\python.exe C:\\\\Users\\\\USERNAME\\\\src\\\\date2name\\\\date2name.py -i \\"%1\\""\n#+END_EXAMPLE\n\nExecute the reg-file, confirm the warnings (you are modifying your\nWindows registry after all) and cheer up when you notice "date2name\n(single file)" in the context menu of your Windows Explorer.\n\nAs the heading and the link name suggests: [[https://stackoverflow.com/questions/6440715/how-to-pass-multiple-filenames-to-a-context-menu-shell-command][this method works on single\nfiles]]. So if you select three files and invoke this context menu item,\nyou will get three different filetag-windows to tag one file each.\n\n** Integration into Thunar\n\n[[https://en.wikipedia.org/wiki/Thunar][Thunar]] is a popular GNU/Linux file browser for the xfce environment.\n\nUnfortunately, it is rather complicated to add custom commands to\nThunar. I found [[https://askubuntu.com/questions/403922/keyboard-shortcut-for-thunar-custom-actions][a good description]] which you might want to follow.\n\nTo my disappoinment, even this manual confguration is not stable\nsomehow. From time to time, the IDs of ~$HOME/.config/Thunar/uca.xml~\nand ~$HOME/.config/Thunar/accels.scm~ differ.\n\nFor people using Org-mode, I automated the updating process (not the\ninitial adding process) to match IDs again:\n\nScript for checking "tag": do it ~tag-ID~ and path in ~accels.scm~ match?\n: #+BEGIN_SRC sh :var myname="tag"\n: ID=`egrep -A 2 "<name>$myname" $HOME/.config/Thunar/uca.xml | grep unique-id | sed \'s#.*<unique-id>##\' | sed \'s#<.*$##\'`\n: echo "$myname-ID of uca.xml: $ID"\n: echo "In accels.scm: "`grep -i "$ID" $HOME/.config/Thunar/accels.scm`\n: #+END_SRC\n\nIf they don\'t match, following script re-writes ~accels.scm~ with the current ID:\n: #+BEGIN_SRC sh :var myname="tag" :var myshortcut="<Alt>t"\n: ID=`egrep -A 2 "<name>$myname" $HOME/.config/Thunar/uca.xml | grep unique-id | sed \'s#.*<unique-id>##\' | sed \'s#<.*$##\'`\n: echo "appending $myname-ID of uca.xml to accels.scm: $ID"\n: mv $HOME/.config/Thunar/accels.scm $HOME/.config/Thunar/accels.scm.OLD\n: grep -v "\\"$myshortcut\\"" $HOME/.config/Thunar/accels.scm.OLD > $HOME/.config/Thunar/accels.scm\n: rm $HOME/.config/Thunar/accels.scm.OLD\n: echo "(gtk_accel_path \\"<Actions>/ThunarActions/uca-action-$ID\\" \\"$myshortcut\\")" >> $HOME/.config/Thunar/accels.scm\n: #+END_SRC\n\n** Integration into FreeCommander\n\n[[http://freecommander.com/en/summary/][FreeCommander]] is a [[https://en.wikipedia.org/wiki/File_manager#Orthodox_file_managers][orthodox file manager]] for Windows. You can add\ndate2name as an favorite command:\n\n- Tools → Favorite tools → Favorite tools edit... (S-C-y)\n  - Create new toolbar (if none is present)\n  - Icon for "Add new item"\n    - Name: date2name\n    - Program or folder: <Path to date2name.bar>\n\t- =date2name.bat= looks like: (please do modify the paths to meet your requirement)\n        : C:\\Python36\\python.exe C:\\Users\\YOURUSERNAME\\src\\date2name\\date2name %*\n\t  : REM optionally: set /p DUMMY=Hit ENTER to continue...\n    - Start folder: =%ActivDir%=\n    - Parameter: =%ActivSel%=\n    - [X] Enclose each selected item with ="=\n    - Hotkey: select next available one such as =Ctrl-1= (it gets overwritten below)\n\t- remember its name such as "Favorite tool 01"\n  - OK\n\nSo far, we\'ve got =date2name= added as a favorite command which can be\naccessed via menu or icon toolbar and the selected keyboard shortcut.\nIf you want to assign a different keyboard shortcut than =Ctrl-1= like\n=Alt-d= you might as well follow following procedure:\n\n- Tools → Define keyboard shortcuts...\n  - Scroll down to the last section "Favorite tools"\n  - locate the name such as "Favorite tool 01"\n  - Define your shortcut of choice like =Alt-d= in the right hand side of the window\n    - If your shortcut is taken, you\'ll get a notification. Don\'t\n      overwrite essential shortcuts you\'re using.\n  - OK\n\n* Related tools and workflows\n\nAlternative implementations of date2name:\n- https://github.com/DerBeutlin/date2name.el for Emacs/dired\n- https://github.com/muehlburger/d2n in Go\n\n---------------\n\nThis tool is part of a tool-set which I use to manage my digital files\nsuch as photographs. My work-flows are described in [[http://karl-voit.at/managing-digital-photographs/][this blog posting]]\nyou might like to read.\n\nIn short:\n\nFor *tagging*, please refer to [[https://github.com/novoid/filetags][filetags]] and its documentation.\n\nSee [[https://github.com/novoid/date2name][date2name]] for easily adding ISO *time-stamps or date-stamps* to\nfiles.\n\nFor *easily naming and tagging* files within file browsers that allow\nintegration of external tools, see [[https://github.com/novoid/appendfilename][appendfilename]] (once more) and\n[[https://github.com/novoid/filetags][filetags]].\n\nMoving to the archive folders is done using [[https://github.com/novoid/move2archive][move2archive]].\n\nHaving tagged photographs gives you many advantages. For example, I\nautomatically [[https://github.com/novoid/set_desktop_background_according_to_season][choose my *desktop background image* according to the\ncurrent season]].\n\nFiles containing an ISO time/date-stamp gets indexed by the\nfilename-module of [[https://github.com/novoid/Memacs][Memacs]].\n\nHere is [[https://glt18-programm.linuxtage.at/events/321.html][a 45 minute talk I gave]] at [[https://glt18.linuxtage.at/][Linuxtage Graz 2018]] presenting the\nidea of and workflows related to appendfilename and other handy tools\nfor file management:\n\n[[https://media.ccc.de/v/GLT18_-_321_-_en_-_g_ap147_004_-_201804281550_-_the_advantages_of_file_name_conventions_and_tagging_-_karl_voit/][bin/2018-05-06 filetags demo slide for video preview with video button -- screenshots.png]]\n\n* How to Thank Me\n\nI\'m glad you like my tools. If you want to support me:\n\n- Send old-fashioned *postcard* per snailmail - I love personal feedback!\n  - see [[http://tinyurl.com/j6w8hyo][my address]]\n- Send feature wishes or improvements as an issue on GitHub\n- Create issues on GitHub for bugs\n- Contribute merge requests for bug fixes\n- Check out my other cool [[https://github.com/novoid][projects on GitHub]]\n',
     'author': 'Karl Voit',
     'author_email': 'tools@Karl-Voit.at',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.11,<4.0',
+    'entry_points': entry_points,
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['date2name']
-package_data = \ {'': ['*']} setup_kwargs = { 'name': 'date2name', 'version':
-'2024.3.10.1', 'description': 'Handling time-stamps and date-stamps in file
+package_data = \ {'': ['*']} entry_points = \ {'console_scripts': ['date2name =
+date2name:main']} setup_kwargs = { 'name': 'date2name', 'version':
+'2024.4.26.1', 'description': 'Handling time-stamps and date-stamps in file
 names', 'long_description': '* Handling time-stamps and date-stamps in file
 names\n\n#+BEGIN_HTML\n_\_n_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_n_o_v_o_i_d_/_s_c_r_e_e_n_c_a_s_t_s_/
 _m_a_s_t_e_r_/_f_i_l_e___m_a_n_a_g_e_m_e_n_t_/_d_a_t_e_2_n_a_m_e_._g_i_f_]_\_n\n#+END_HTML\n\n[[file:bin/
 screencast.gif]]\n\nPer default, date2name gets the modification time of
 matching files\nand directories and adds a datestamp in standard ISO 8601+
 format\nYYYY-MM-DD (http://datestamps.org/index.shtml) at the beginning of\nthe
 file- or directoryname.\n\nIf an existing timestamp is found, its style will be
@@ -124,8 +125,9 @@
 want to support me:\n\n- Send old-fashioned *postcard* per snailmail - I love
 personal feedback!\n - see [[http://tinyurl.com/j6w8hyo][my address]]\n- Send
 feature wishes or improvements as an issue on GitHub\n- Create issues on GitHub
 for bugs\n- Contribute merge requests for bug fixes\n- Check out my other cool
 [[https://github.com/novoid][projects on GitHub]]\n', 'author': 'Karl Voit',
 'author_email': 'tools@Karl-Voit.at', 'maintainer': 'None', 'maintainer_email':
 'None', 'url': 'None', 'packages': packages, 'package_data': package_data,
-'python_requires': '>=3.11,<4.0', } setup(**setup_kwargs)
+'entry_points': entry_points, 'python_requires': '>=3.9,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `date2name-2024.3.10.1/PKG-INFO` & `date2name-2024.4.26.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: date2name
-Version: 2024.3.10.1
+Version: 2024.4.26.1
 Summary: Handling time-stamps and date-stamps in file names
 License: GPL v3
 Author: Karl Voit
 Author-email: tools@Karl-Voit.at
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/plain
 
 * Handling time-stamps and date-stamps in file names
 
 #+BEGIN_HTML
 <a href="https://karl-voit.at/demo-date2name">
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: date2name Version: 2024.3.10.1 Summary: Handling
+Metadata-Version: 2.1 Name: date2name Version: 2024.4.26.1 Summary: Handling
 time-stamps and date-stamps in file names License: GPL v3 Author: Karl Voit
-Author-email: tools@Karl-Voit.at Requires-Python: >=3.11,<4.0 Classifier:
+Author-email: tools@Karl-Voit.at Requires-Python: >=3.9,<4.0 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.11 Description-Content-
-Type: text/plain * Handling time-stamps and date-stamps in file names
-#+BEGIN_HTML _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_n_o_v_o_i_d_/_s_c_r_e_e_n_c_a_s_t_s_/_m_a_s_t_e_r_/
-_f_i_l_e___m_a_n_a_g_e_m_e_n_t_/_d_a_t_e_2_n_a_m_e_._g_i_f_]#+END_HTML [[file:bin/screencast.gif]] Per
+:: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/plain * Handling time-stamps and date-stamps in
+file names #+BEGIN_HTML _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_n_o_v_o_i_d_/_s_c_r_e_e_n_c_a_s_t_s_/
+_m_a_s_t_e_r_/_f_i_l_e___m_a_n_a_g_e_m_e_n_t_/_d_a_t_e_2_n_a_m_e_._g_i_f_]#+END_HTML [[file:bin/screencast.gif]] Per
 default, date2name gets the modification time of matching files and directories
 and adds a datestamp in standard ISO 8601+ format YYYY-MM-DD (http://
 datestamps.org/index.shtml) at the beginning of the file- or directoryname. If
 an existing timestamp is found, its style will be converted to the selected ISO
 datestamp format but the numbers stays the same. Executed with an
 examplefilename "file" this results e.g. in "2008-12-31_file". Note: Other that
 defined in ISO 8601+ the delimiter between hours, minutes, and seconds is not a
```

