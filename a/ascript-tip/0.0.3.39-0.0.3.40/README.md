# Comparing `tmp/ascript-tip-0.0.3.39.tar.gz` & `tmp/ascript-tip-0.0.3.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascript-tip-0.0.3.39.tar", last modified: Thu Mar  7 08:44:11 2024, max compression
+gzip compressed data, was "ascript-tip-0.0.3.40.tar", last modified: Fri Apr 26 06:24:20 2024, max compression
```

## Comparing `ascript-tip-0.0.3.39.tar` & `ascript-tip-0.0.3.40.tar`

### file list

```diff
@@ -1,167 +1,174 @@
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.896507 ascript-tip-0.0.3.39/
--rw-r--r--   0 freedom    (501) staff       (20)       49 2024-03-07 08:39:44.000000 ascript-tip-0.0.3.39/MANIFEST.in
--rw-r--r--   0 freedom    (501) staff       (20)      456 2024-03-07 08:44:11.896326 ascript-tip-0.0.3.39/PKG-INFO
--rw-r--r--   0 freedom    (501) staff       (20)       62 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/README.md
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.855940 ascript-tip-0.0.3.39/ascript/
--rw-r--r--   0 freedom    (501) staff       (20)        1 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/__init__.py
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.858041 ascript-tip-0.0.3.39/ascript/android/
--rw-r--r--   0 freedom    (501) staff       (20)      145 2024-01-29 09:55:38.000000 ascript-tip-0.0.3.39/ascript/android/__init__.py
--rw-r--r--   0 freedom    (501) staff       (20)     4198 2024-02-26 14:15:08.000000 ascript-tip-0.0.3.39/ascript/android/action.py
--rw-r--r--   0 freedom    (501) staff       (20)      215 2024-01-23 03:55:43.000000 ascript-tip-0.0.3.39/ascript/android/data.py
--rw-r--r--   0 freedom    (501) staff       (20)     1692 2024-02-26 13:26:52.000000 ascript-tip-0.0.3.39/ascript/android/media.py
--rw-r--r--   0 freedom    (501) staff       (20)     6181 2024-01-27 09:40:51.000000 ascript-tip-0.0.3.39/ascript/android/node.py
--rw-r--r--   0 freedom    (501) staff       (20)     9270 2024-02-26 03:33:04.000000 ascript-tip-0.0.3.39/ascript/android/screen.py
--rw-r--r--   0 freedom    (501) staff       (20)     2897 2024-02-20 06:55:29.000000 ascript-tip-0.0.3.39/ascript/android/system.py
--rw-r--r--   0 freedom    (501) staff       (20)     3596 2024-02-26 08:36:09.000000 ascript-tip-0.0.3.39/ascript/android/ui.py
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.859259 ascript-tip-0.0.3.39/ascript/windows/
--rw-r--r--   0 freedom    (501) staff       (20)        3 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/__init__.py
--rw-r--r--   0 freedom    (501) staff       (20)     1745 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/action.py
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.860550 ascript-tip-0.0.3.39/ascript/windows/client/
--rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/__init__.py
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.860736 ascript-tip-0.0.3.39/ascript/windows/client/assets/
--rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/__init__.py
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.854191 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.865371 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/
--rw-r--r--   0 freedom    (501) staff       (20)    67472 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.css
--rw-r--r--   0 freedom    (501) staff       (20)   163856 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.css.map
--rw-r--r--   0 freedom    (501) staff       (20)    50636 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.min.css
--rw-r--r--   0 freedom    (501) staff       (20)   115091 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0 freedom    (501) staff       (20)     4784 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.css
--rw-r--r--   0 freedom    (501) staff       (20)    78154 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.css.map
--rw-r--r--   0 freedom    (501) staff       (20)     3922 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.min.css
--rw-r--r--   0 freedom    (501) staff       (20)    33156 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 freedom    (501) staff       (20)   200387 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.css
--rw-r--r--   0 freedom    (501) staff       (20)   515619 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.css.map
--rw-r--r--   0 freedom    (501) staff       (20)   162264 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.min.css
--rw-r--r--   0 freedom    (501) staff       (20)   654593 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.871764 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/
--rw-r--r--   0 freedom    (501) staff       (20)   230599 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.js
--rw-r--r--   0 freedom    (501) staff       (20)   426918 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.js.map
--rw-r--r--   0 freedom    (501) staff       (20)    83376 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.min.js
--rw-r--r--   0 freedom    (501) staff       (20)   308871 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 freedom    (501) staff       (20)   137714 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.js
--rw-r--r--   0 freedom    (501) staff       (20)   271784 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.js.map
--rw-r--r--   0 freedom    (501) staff       (20)    62563 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.min.js
--rw-r--r--   0 freedom    (501) staff       (20)   185257 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.min.js.map
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.873818 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/
--rw-r--r--   0 freedom    (501) staff       (20)      577 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/arrow-repeat.svg
--rw-r--r--   0 freedom    (501) staff       (20)      435 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/camera-video-off-fill.svg
--rw-r--r--   0 freedom    (501) staff       (20)      290 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/chevron-down.svg
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.875553 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/
--rw-r--r--   0 freedom    (501) staff       (20)    98255 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.css
--rw-r--r--   0 freedom    (501) staff       (20)    52358 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.json
--rw-r--r--   0 freedom    (501) staff       (20)    85875 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.min.css
--rw-r--r--   0 freedom    (501) staff       (20)    57755 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.scss
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.876335 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/fonts/
--rw-r--r--   0 freedom    (501) staff       (20)   176088 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/fonts/bootstrap-icons.woff
--rw-r--r--   0 freedom    (501) staff       (20)   130648 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/fonts/bootstrap-icons.woff2
--rw-r--r--   0 freedom    (501) staff       (20)      371 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/info.svg
--rw-r--r--   0 freedom    (501) staff       (20)      539 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/trash.svg
--rw-r--r--   0 freedom    (501) staff       (20)      397 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/x-square-fill.svg
--rw-r--r--   0 freedom    (501) staff       (20)      550 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/zoom-in.svg
--rw-r--r--   0 freedom    (501) staff       (20)      503 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/zoom-out.svg
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.876896 ascript-tip-0.0.3.39/ascript/windows/client/assets/css/
--rw-r--r--   0 freedom    (501) staff       (20)     6026 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/css/colors.css
--rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/css/hwnd.css
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.885090 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/
--rw-r--r--   0 freedom    (501) staff       (20)     1525 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_app.png
--rw-r--r--   0 freedom    (501) staff       (20)     2446 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_apps.png
--rw-r--r--   0 freedom    (501) staff       (20)     1428 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_capture.png
--rw-r--r--   0 freedom    (501) staff       (20)     1246 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_close.png
--rw-r--r--   0 freedom    (501) staff       (20)     2230 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_config.png
--rw-r--r--   0 freedom    (501) staff       (20)      785 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_dev.png
--rw-r--r--   0 freedom    (501) staff       (20)      675 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_floder.png
--rw-r--r--   0 freedom    (501) staff       (20)     2642 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_home.png
--rw-r--r--   0 freedom    (501) staff       (20)     1104 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_log.png
--rw-r--r--   0 freedom    (501) staff       (20)      843 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_min.png
--rw-r--r--   0 freedom    (501) staff       (20)      545 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_package.png
--rw-r--r--   0 freedom    (501) staff       (20)     1578 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_pic.png
--rw-r--r--   0 freedom    (501) staff       (20)      431 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_play.png
--rw-r--r--   0 freedom    (501) staff       (20)     2070 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_pycharm.png
--rw-r--r--   0 freedom    (501) staff       (20)     1654 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_python.png
--rw-r--r--   0 freedom    (501) staff       (20)      645 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_python_20.png
--rw-r--r--   0 freedom    (501) staff       (20)     1024 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_python_32.png
--rw-r--r--   0 freedom    (501) staff       (20)     1946 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_run.png
--rw-r--r--   0 freedom    (501) staff       (20)     1382 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_setting.png
--rw-r--r--   0 freedom    (501) staff       (20)     1259 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_stop.png
--rw-r--r--   0 freedom    (501) staff       (20)      343 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_swap_right.png
--rw-r--r--   0 freedom    (501) staff       (20)     1408 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_tool.png
--rw-r--r--   0 freedom    (501) staff       (20)      869 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_win.png
--rw-r--r--   0 freedom    (501) staff       (20)    17888 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/img/logo.png
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.854796 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.885335 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/css/
--rw-r--r--   0 freedom    (501) staff       (20)     6233 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/css/zTreeStyle.css
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.886088 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.888170 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/
--rw-r--r--   0 freedom    (501) staff       (20)      601 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/1_close.png
--rw-r--r--   0 freedom    (501) staff       (20)      580 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/1_open.png
--rw-r--r--   0 freedom    (501) staff       (20)      570 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/2.png
--rw-r--r--   0 freedom    (501) staff       (20)      762 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/3.png
--rw-r--r--   0 freedom    (501) staff       (20)      399 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/4.png
--rw-r--r--   0 freedom    (501) staff       (20)      710 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/5.png
--rw-r--r--   0 freedom    (501) staff       (20)      432 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/6.png
--rw-r--r--   0 freedom    (501) staff       (20)      534 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/7.png
--rw-r--r--   0 freedom    (501) staff       (20)      529 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/8.png
--rw-r--r--   0 freedom    (501) staff       (20)      467 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/9.png
--rw-r--r--   0 freedom    (501) staff       (20)       45 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/line_conn.gif
--rw-r--r--   0 freedom    (501) staff       (20)      381 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/loading.gif
--rw-r--r--   0 freedom    (501) staff       (20)     2744 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/tree-node-btn.png
--rw-r--r--   0 freedom    (501) staff       (20)     5564 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/zTreeStandard.gif
--rw-r--r--   0 freedom    (501) staff       (20)    11173 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/zTreeStandard.png
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.888338 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/js/
--rw-r--r--   0 freedom    (501) staff       (20)    67966 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/js/jquery.ztree.all.min.js
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.889164 ascript-tip-0.0.3.39/ascript/windows/client/assets/js/
--rw-r--r--   0 freedom    (501) staff       (20)      736 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/js/base.js
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.890162 ascript-tip-0.0.3.39/ascript/windows/client/assets/js/colors/
--rw-r--r--   0 freedom    (501) staff       (20)    19016 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/js/colors/colors.js
--rw-r--r--   0 freedom    (501) staff       (20)    13166 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/js/colors/colors_choosecolor.js
--rw-r--r--   0 freedom    (501) staff       (20)    16132 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/js/colors/colors_findimage.js
--rw-r--r--   0 freedom    (501) staff       (20)     6981 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/js/colors/ocr.js
--rw-r--r--   0 freedom    (501) staff       (20)    10248 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/js/hwnd.js
--rw-r--r--   0 freedom    (501) staff       (20)    87532 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/js/jquery-3.7.js
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.892820 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/
--rw-r--r--   0 freedom    (501) staff       (20)    12320 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/bar.ui
--rw-r--r--   0 freedom    (501) staff       (20)     6143 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/config.ui
--rw-r--r--   0 freedom    (501) staff       (20)    12030 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/home.ui
--rw-r--r--   0 freedom    (501) staff       (20)     2189 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/hwnd.ui
--rw-r--r--   0 freedom    (501) staff       (20)     3044 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/item_app.ui
--rw-r--r--   0 freedom    (501) staff       (20)     1042 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/log.ui
--rw-r--r--   0 freedom    (501) staff       (20)     1347 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/main.ui
--rw-r--r--   0 freedom    (501) staff       (20)     4633 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/pycharminstall.ui
--rw-r--r--   0 freedom    (501) staff       (20)     6876 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/pyinstall.ui
--rw-r--r--   0 freedom    (501) staff       (20)     6997 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/step.ui
--rw-r--r--   0 freedom    (501) staff       (20)     2929 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/workspace.ui
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.893751 ascript-tip-0.0.3.39/ascript/windows/client/assets/templates/
--rw-r--r--   0 freedom    (501) staff       (20)     2140 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/templates/base.html
--rw-r--r--   0 freedom    (501) staff       (20)    37134 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/templates/colors.html
--rw-r--r--   0 freedom    (501) staff       (20)     8206 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/templates/hwnd.html
--rw-r--r--   0 freedom    (501) staff       (20)      452 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/templates/index.html
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.855157 ascript-tip-0.0.3.39/ascript/windows/client/assets/tools/
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.893919 ascript-tip-0.0.3.39/ascript/windows/client/assets/tools/capture/
--rw-r--r--   0 freedom    (501) staff       (20)   127355 2024-02-29 07:51:26.000000 ascript-tip-0.0.3.39/ascript/windows/client/assets/tools/capture/1708245806.png
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.894615 ascript-tip-0.0.3.39/ascript/windows/client/dao/
--rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/dao/__init__.py
--rw-r--r--   0 freedom    (501) staff       (20)      909 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/dao/server_dao.py
--rw-r--r--   0 freedom    (501) staff       (20)     7424 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/server.py
--rw-r--r--   0 freedom    (501) staff       (20)      332 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/start.py
--rw-r--r--   0 freedom    (501) staff       (20)     2945 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/tools.py
--rw-r--r--   0 freedom    (501) staff       (20)    27686 2024-02-29 08:11:55.000000 ascript-tip-0.0.3.39/ascript/windows/client/ui.py
--rw-r--r--   0 freedom    (501) staff       (20)     3131 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/client/worker.py
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.894962 ascript-tip-0.0.3.39/ascript/windows/daos/
--rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/daos/__init__.py
--rw-r--r--   0 freedom    (501) staff       (20)     1442 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/daos/screen.py
--rw-r--r--   0 freedom    (501) staff       (20)    13806 2024-02-29 07:51:26.000000 ascript-tip-0.0.3.39/ascript/windows/screen.py
--rw-r--r--   0 freedom    (501) staff       (20)      650 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/system.py
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.895558 ascript-tip-0.0.3.39/ascript/windows/utils/
--rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/utils/__init__.py
--rw-r--r--   0 freedom    (501) staff       (20)    10743 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/utils/airclickcv.py
--rw-r--r--   0 freedom    (501) staff       (20)       77 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/utils/node_utils.py
--rw-r--r--   0 freedom    (501) staff       (20)     5499 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/utils/screen_utils.py
--rw-r--r--   0 freedom    (501) staff       (20)     4276 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.39/ascript/windows/window.py
-drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-03-07 08:44:11.896085 ascript-tip-0.0.3.39/ascript_tip.egg-info/
--rw-r--r--   0 freedom    (501) staff       (20)      456 2024-03-07 08:44:11.000000 ascript-tip-0.0.3.39/ascript_tip.egg-info/PKG-INFO
--rw-r--r--   0 freedom    (501) staff       (20)     6977 2024-03-07 08:44:11.000000 ascript-tip-0.0.3.39/ascript_tip.egg-info/SOURCES.txt
--rw-r--r--   0 freedom    (501) staff       (20)        1 2024-03-07 08:44:11.000000 ascript-tip-0.0.3.39/ascript_tip.egg-info/dependency_links.txt
--rw-r--r--   0 freedom    (501) staff       (20)        8 2024-03-07 08:44:11.000000 ascript-tip-0.0.3.39/ascript_tip.egg-info/top_level.txt
--rw-r--r--   0 freedom    (501) staff       (20)       38 2024-03-07 08:44:11.896551 ascript-tip-0.0.3.39/setup.cfg
--rw-r--r--   0 freedom    (501) staff       (20)     1049 2024-03-07 08:41:55.000000 ascript-tip-0.0.3.39/setup.py
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.515957 ascript-tip-0.0.3.40/
+-rw-r--r--   0 freedom    (501) staff       (20)       49 2024-03-07 08:39:44.000000 ascript-tip-0.0.3.40/MANIFEST.in
+-rw-r--r--   0 freedom    (501) staff       (20)      450 2024-04-26 06:24:20.515809 ascript-tip-0.0.3.40/PKG-INFO
+-rw-r--r--   0 freedom    (501) staff       (20)       62 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/README.md
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.483881 ascript-tip-0.0.3.40/ascript/
+-rw-r--r--   0 freedom    (501) staff       (20)        1 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/__init__.py
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.485754 ascript-tip-0.0.3.40/ascript/android/
+-rw-r--r--   0 freedom    (501) staff       (20)      164 2024-03-13 14:49:25.000000 ascript-tip-0.0.3.40/ascript/android/__init__.py
+-rw-r--r--   0 freedom    (501) staff       (20)     4215 2024-04-22 07:01:16.000000 ascript-tip-0.0.3.40/ascript/android/action.py
+-rw-r--r--   0 freedom    (501) staff       (20)      215 2024-01-23 03:55:43.000000 ascript-tip-0.0.3.40/ascript/android/data.py
+-rw-r--r--   0 freedom    (501) staff       (20)     1692 2024-02-26 13:26:52.000000 ascript-tip-0.0.3.40/ascript/android/media.py
+-rw-r--r--   0 freedom    (501) staff       (20)     6265 2024-04-03 09:26:48.000000 ascript-tip-0.0.3.40/ascript/android/node.py
+-rw-r--r--   0 freedom    (501) staff       (20)      117 2024-03-13 02:33:38.000000 ascript-tip-0.0.3.40/ascript/android/plug.py
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.486681 ascript-tip-0.0.3.40/ascript/android/screen/
+-rw-r--r--   0 freedom    (501) staff       (20)    19200 2024-04-25 15:53:43.000000 ascript-tip-0.0.3.40/ascript/android/screen/__init__.py
+-rw-r--r--   0 freedom    (501) staff       (20)     7372 2024-04-26 00:16:12.000000 ascript-tip-0.0.3.40/ascript/android/screen/ascv.py
+-rw-r--r--   0 freedom    (501) staff       (20)     5676 2024-04-23 03:44:27.000000 ascript-tip-0.0.3.40/ascript/android/screen/gp.py
+-rw-r--r--   0 freedom    (501) staff       (20)    10454 2024-04-22 07:28:52.000000 ascript-tip-0.0.3.40/ascript/android/screen/gp_tasks.py
+-rw-r--r--   0 freedom    (501) staff       (20)     3575 2024-04-23 03:40:42.000000 ascript-tip-0.0.3.40/ascript/android/screen/gp_tool.py
+-rw-r--r--   0 freedom    (501) staff       (20)     9270 2024-02-26 03:33:04.000000 ascript-tip-0.0.3.40/ascript/android/screen.py
+-rw-r--r--   0 freedom    (501) staff       (20)     3223 2024-04-25 16:09:45.000000 ascript-tip-0.0.3.40/ascript/android/system.py
+-rw-r--r--   0 freedom    (501) staff       (20)     4668 2024-03-29 10:45:03.000000 ascript-tip-0.0.3.40/ascript/android/ui.py
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.487636 ascript-tip-0.0.3.40/ascript/windows/
+-rw-r--r--   0 freedom    (501) staff       (20)        3 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/__init__.py
+-rw-r--r--   0 freedom    (501) staff       (20)     1745 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/action.py
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.488710 ascript-tip-0.0.3.40/ascript/windows/client/
+-rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/__init__.py
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.488840 ascript-tip-0.0.3.40/ascript/windows/client/assets/
+-rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/__init__.py
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.481959 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.493354 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/
+-rw-r--r--   0 freedom    (501) staff       (20)    67472 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.css
+-rw-r--r--   0 freedom    (501) staff       (20)   163856 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.css.map
+-rw-r--r--   0 freedom    (501) staff       (20)    50636 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 freedom    (501) staff       (20)   115091 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 freedom    (501) staff       (20)     4784 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.css
+-rw-r--r--   0 freedom    (501) staff       (20)    78154 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0 freedom    (501) staff       (20)     3922 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 freedom    (501) staff       (20)    33156 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 freedom    (501) staff       (20)   200387 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.css
+-rw-r--r--   0 freedom    (501) staff       (20)   515619 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.css.map
+-rw-r--r--   0 freedom    (501) staff       (20)   162264 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.min.css
+-rw-r--r--   0 freedom    (501) staff       (20)   654593 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.499716 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/
+-rw-r--r--   0 freedom    (501) staff       (20)   230599 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.js
+-rw-r--r--   0 freedom    (501) staff       (20)   426918 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0 freedom    (501) staff       (20)    83376 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 freedom    (501) staff       (20)   308871 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 freedom    (501) staff       (20)   137714 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.js
+-rw-r--r--   0 freedom    (501) staff       (20)   271784 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.js.map
+-rw-r--r--   0 freedom    (501) staff       (20)    62563 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.min.js
+-rw-r--r--   0 freedom    (501) staff       (20)   185257 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.min.js.map
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.501683 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/
+-rw-r--r--   0 freedom    (501) staff       (20)      577 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/arrow-repeat.svg
+-rw-r--r--   0 freedom    (501) staff       (20)      435 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/camera-video-off-fill.svg
+-rw-r--r--   0 freedom    (501) staff       (20)      290 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/chevron-down.svg
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.502573 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/
+-rw-r--r--   0 freedom    (501) staff       (20)    98255 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.css
+-rw-r--r--   0 freedom    (501) staff       (20)    52358 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.json
+-rw-r--r--   0 freedom    (501) staff       (20)    85875 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.min.css
+-rw-r--r--   0 freedom    (501) staff       (20)    57755 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.scss
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.503194 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/fonts/
+-rw-r--r--   0 freedom    (501) staff       (20)   176088 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/fonts/bootstrap-icons.woff
+-rw-r--r--   0 freedom    (501) staff       (20)   130648 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 freedom    (501) staff       (20)      371 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/info.svg
+-rw-r--r--   0 freedom    (501) staff       (20)      539 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/trash.svg
+-rw-r--r--   0 freedom    (501) staff       (20)      397 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/x-square-fill.svg
+-rw-r--r--   0 freedom    (501) staff       (20)      550 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/zoom-in.svg
+-rw-r--r--   0 freedom    (501) staff       (20)      503 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/zoom-out.svg
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.503634 ascript-tip-0.0.3.40/ascript/windows/client/assets/css/
+-rw-r--r--   0 freedom    (501) staff       (20)     6026 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/css/colors.css
+-rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/css/hwnd.css
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.507009 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/
+-rw-r--r--   0 freedom    (501) staff       (20)     1525 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_app.png
+-rw-r--r--   0 freedom    (501) staff       (20)     2446 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_apps.png
+-rw-r--r--   0 freedom    (501) staff       (20)     1428 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_capture.png
+-rw-r--r--   0 freedom    (501) staff       (20)     1246 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_close.png
+-rw-r--r--   0 freedom    (501) staff       (20)     2230 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_config.png
+-rw-r--r--   0 freedom    (501) staff       (20)      785 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_dev.png
+-rw-r--r--   0 freedom    (501) staff       (20)      675 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_floder.png
+-rw-r--r--   0 freedom    (501) staff       (20)     2642 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_home.png
+-rw-r--r--   0 freedom    (501) staff       (20)     1104 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_log.png
+-rw-r--r--   0 freedom    (501) staff       (20)      843 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_min.png
+-rw-r--r--   0 freedom    (501) staff       (20)      545 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_package.png
+-rw-r--r--   0 freedom    (501) staff       (20)     1578 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_pic.png
+-rw-r--r--   0 freedom    (501) staff       (20)      431 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_play.png
+-rw-r--r--   0 freedom    (501) staff       (20)     2070 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_pycharm.png
+-rw-r--r--   0 freedom    (501) staff       (20)     1654 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_python.png
+-rw-r--r--   0 freedom    (501) staff       (20)      645 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_python_20.png
+-rw-r--r--   0 freedom    (501) staff       (20)     1024 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_python_32.png
+-rw-r--r--   0 freedom    (501) staff       (20)     1946 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_run.png
+-rw-r--r--   0 freedom    (501) staff       (20)     1382 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_setting.png
+-rw-r--r--   0 freedom    (501) staff       (20)     1259 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_stop.png
+-rw-r--r--   0 freedom    (501) staff       (20)      343 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_swap_right.png
+-rw-r--r--   0 freedom    (501) staff       (20)     1408 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_tool.png
+-rw-r--r--   0 freedom    (501) staff       (20)      869 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_win.png
+-rw-r--r--   0 freedom    (501) staff       (20)    17888 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/img/logo.png
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.482557 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.507192 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/css/
+-rw-r--r--   0 freedom    (501) staff       (20)     6233 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/css/zTreeStyle.css
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.507861 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.509298 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/
+-rw-r--r--   0 freedom    (501) staff       (20)      601 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/1_close.png
+-rw-r--r--   0 freedom    (501) staff       (20)      580 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/1_open.png
+-rw-r--r--   0 freedom    (501) staff       (20)      570 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/2.png
+-rw-r--r--   0 freedom    (501) staff       (20)      762 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/3.png
+-rw-r--r--   0 freedom    (501) staff       (20)      399 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/4.png
+-rw-r--r--   0 freedom    (501) staff       (20)      710 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/5.png
+-rw-r--r--   0 freedom    (501) staff       (20)      432 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/6.png
+-rw-r--r--   0 freedom    (501) staff       (20)      534 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/7.png
+-rw-r--r--   0 freedom    (501) staff       (20)      529 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/8.png
+-rw-r--r--   0 freedom    (501) staff       (20)      467 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/9.png
+-rw-r--r--   0 freedom    (501) staff       (20)       45 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/line_conn.gif
+-rw-r--r--   0 freedom    (501) staff       (20)      381 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/loading.gif
+-rw-r--r--   0 freedom    (501) staff       (20)     2744 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/tree-node-btn.png
+-rw-r--r--   0 freedom    (501) staff       (20)     5564 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/zTreeStandard.gif
+-rw-r--r--   0 freedom    (501) staff       (20)    11173 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/zTreeStandard.png
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.509432 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/js/
+-rw-r--r--   0 freedom    (501) staff       (20)    67966 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/js/jquery.ztree.all.min.js
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.510159 ascript-tip-0.0.3.40/ascript/windows/client/assets/js/
+-rw-r--r--   0 freedom    (501) staff       (20)      736 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/js/base.js
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.510938 ascript-tip-0.0.3.40/ascript/windows/client/assets/js/colors/
+-rw-r--r--   0 freedom    (501) staff       (20)    19016 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/js/colors/colors.js
+-rw-r--r--   0 freedom    (501) staff       (20)    13166 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/js/colors/colors_choosecolor.js
+-rw-r--r--   0 freedom    (501) staff       (20)    16132 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/js/colors/colors_findimage.js
+-rw-r--r--   0 freedom    (501) staff       (20)     6981 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/js/colors/ocr.js
+-rw-r--r--   0 freedom    (501) staff       (20)    10248 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/js/hwnd.js
+-rw-r--r--   0 freedom    (501) staff       (20)    87532 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/js/jquery-3.7.js
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.512537 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/
+-rw-r--r--   0 freedom    (501) staff       (20)    12320 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/bar.ui
+-rw-r--r--   0 freedom    (501) staff       (20)     6143 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/config.ui
+-rw-r--r--   0 freedom    (501) staff       (20)    12030 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/home.ui
+-rw-r--r--   0 freedom    (501) staff       (20)     2189 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/hwnd.ui
+-rw-r--r--   0 freedom    (501) staff       (20)     3044 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/item_app.ui
+-rw-r--r--   0 freedom    (501) staff       (20)     1042 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/log.ui
+-rw-r--r--   0 freedom    (501) staff       (20)     1347 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/main.ui
+-rw-r--r--   0 freedom    (501) staff       (20)     4633 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/pycharminstall.ui
+-rw-r--r--   0 freedom    (501) staff       (20)     6876 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/pyinstall.ui
+-rw-r--r--   0 freedom    (501) staff       (20)     6997 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/step.ui
+-rw-r--r--   0 freedom    (501) staff       (20)     2929 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/workspace.ui
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.513188 ascript-tip-0.0.3.40/ascript/windows/client/assets/templates/
+-rw-r--r--   0 freedom    (501) staff       (20)     2140 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/templates/base.html
+-rw-r--r--   0 freedom    (501) staff       (20)    37134 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/templates/colors.html
+-rw-r--r--   0 freedom    (501) staff       (20)     8206 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/templates/hwnd.html
+-rw-r--r--   0 freedom    (501) staff       (20)      452 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/templates/index.html
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.482905 ascript-tip-0.0.3.40/ascript/windows/client/assets/tools/
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.513349 ascript-tip-0.0.3.40/ascript/windows/client/assets/tools/capture/
+-rw-r--r--   0 freedom    (501) staff       (20)   127355 2024-02-29 07:51:26.000000 ascript-tip-0.0.3.40/ascript/windows/client/assets/tools/capture/1708245806.png
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.514104 ascript-tip-0.0.3.40/ascript/windows/client/dao/
+-rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/dao/__init__.py
+-rw-r--r--   0 freedom    (501) staff       (20)      909 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/dao/server_dao.py
+-rw-r--r--   0 freedom    (501) staff       (20)     7424 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/server.py
+-rw-r--r--   0 freedom    (501) staff       (20)      332 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/start.py
+-rw-r--r--   0 freedom    (501) staff       (20)     2945 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/tools.py
+-rw-r--r--   0 freedom    (501) staff       (20)    27686 2024-02-29 08:11:55.000000 ascript-tip-0.0.3.40/ascript/windows/client/ui.py
+-rw-r--r--   0 freedom    (501) staff       (20)     3131 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/client/worker.py
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.514468 ascript-tip-0.0.3.40/ascript/windows/daos/
+-rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/daos/__init__.py
+-rw-r--r--   0 freedom    (501) staff       (20)     1442 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/daos/screen.py
+-rw-r--r--   0 freedom    (501) staff       (20)    13806 2024-02-29 07:51:26.000000 ascript-tip-0.0.3.40/ascript/windows/screen.py
+-rw-r--r--   0 freedom    (501) staff       (20)      650 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/system.py
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.515098 ascript-tip-0.0.3.40/ascript/windows/utils/
+-rw-r--r--   0 freedom    (501) staff       (20)        0 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/utils/__init__.py
+-rw-r--r--   0 freedom    (501) staff       (20)    10743 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/utils/airclickcv.py
+-rw-r--r--   0 freedom    (501) staff       (20)       77 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/utils/node_utils.py
+-rw-r--r--   0 freedom    (501) staff       (20)     5499 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/utils/screen_utils.py
+-rw-r--r--   0 freedom    (501) staff       (20)     4276 2024-02-02 08:46:24.000000 ascript-tip-0.0.3.40/ascript/windows/window.py
+drwxr-xr-x   0 freedom    (501) staff       (20)        0 2024-04-26 06:24:20.515561 ascript-tip-0.0.3.40/ascript_tip.egg-info/
+-rw-r--r--   0 freedom    (501) staff       (20)      450 2024-04-26 06:24:20.000000 ascript-tip-0.0.3.40/ascript_tip.egg-info/PKG-INFO
+-rw-r--r--   0 freedom    (501) staff       (20)     7165 2024-04-26 06:24:20.000000 ascript-tip-0.0.3.40/ascript_tip.egg-info/SOURCES.txt
+-rw-r--r--   0 freedom    (501) staff       (20)        1 2024-04-26 06:24:20.000000 ascript-tip-0.0.3.40/ascript_tip.egg-info/dependency_links.txt
+-rw-r--r--   0 freedom    (501) staff       (20)        8 2024-04-26 06:24:20.000000 ascript-tip-0.0.3.40/ascript_tip.egg-info/top_level.txt
+-rw-r--r--   0 freedom    (501) staff       (20)       38 2024-04-26 06:24:20.516000 ascript-tip-0.0.3.40/setup.cfg
+-rw-r--r--   0 freedom    (501) staff       (20)     1043 2024-04-26 06:23:42.000000 ascript-tip-0.0.3.40/setup.py
```

### Comparing `ascript-tip-0.0.3.39/ascript/android/action.py` & `ascript-tip-0.0.3.40/ascript/android/action.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,58 +7,63 @@
 from airscript.action import input as asinput
 from airscript.action import key as askey
 from .node import Selector
 from airscript.action import gesture as asgesture
 from airscript.action import path as aspath
 from airscript.action import hid as ashid
 
-def click(x:Union[int,Point],y:int=None,dur:int = 20):
+
+def click(x: Union[int, Point], y: int = None, dur: int = 20):
     if type(x) == float:
         x = int(x)
 
     if type(y) == float:
         y = int(y)
 
-
-    if type(x)==int:
-        asclick(x,y,dur)
+    if type(x) == int:
+        asclick(x, y, dur)
     else:
-        asclick(x,dur)
-def swipe(x:int,y:int,x1:int,y1:int,dur:int=20):
+        asclick(x, dur)
+
+
+def swipe(x: int, y: int, x1: int, y1: int, dur: int = 20):
     x = int(x)
     y = int(y)
     x1 = int(x1)
     y1 = int(y1)
 
-    return asslide(x,y,x1,y1,dur)
+    return asslide(x, y, x1, y1, dur)
+
 
-def input(msg:str="",selector:Selector=None):
+def input(msg: str = "", selector: Selector = None):
     if selector:
-        asinput(msg,selector.sel)
+        asinput(msg, selector.sel)
     else:
         asinput(msg)
 
+
 class Touch:
     @staticmethod
-    def down(x,y,dur:int=20):
+    def down(x, y, dur: int = 20):
         x = int(x)
         y = int(y)
-        astouch.down(x,y,dur)
+        astouch.down(x, y, dur)
 
     @staticmethod
     def move(x, y, dur: int = 20):
         x = int(x)
         y = int(y)
-        astouch.move(x,y,dur)
+        astouch.move(x, y, dur)
 
     @staticmethod
     def up(x, y, dur: int = 20):
         x = int(x)
         y = int(y)
-        astouch.up(x,y,dur)
+        astouch.up(x, y, dur)
+
 
 class Key:
     @staticmethod
     def home():
         askey.home()
 
     @staticmethod
@@ -77,89 +82,93 @@
     def screenshot():
         askey.screenshot()
 
     @staticmethod
     def recents():
         askey.recents()
 
+
 class Hid:
     @staticmethod
-    def click(x:int,y:int,dur:int=20):
+    def click(x: int, y: int, dur: int = 20):
         x = int(x)
         y = int(y)
-        ashid.click(x,y,dur)
+        ashid.click(x, y, dur)
 
     @staticmethod
-    def swipe(x:int,y:int,x1:int,y1:int,dur:int=20):
+    def swipe(x: int, y: int, x1: int, y1: int, dur: int = 20):
         x = int(x)
         y = int(y)
         x1 = int(x1)
         y1 = int(y1)
-        ashid.slide(x,y,x1,y1,dur)
+        ashid.slide(x, y, x1, y1, dur)
 
     @staticmethod
     def key(**keycode):
         ashid.key(keycode)
 
+
 class Path:
-    def __init__(self,start_time:int=0, duration:int=20, will_continue:bool=False):
-        self.mpath = aspath(start_time,duration,will_continue)
+    def __init__(self, start_time: int = 0, duration: int = 20, will_continue: bool = False):
+        self.mpath = aspath(start_time, duration, will_continue)
 
-    def quadTo(self,x1, y1, x2, y2):
+    def quadTo(self, x1, y1, x2, y2):
         self.mpath.quadTo(x1, y1, x2, y2)
 
-    def lineTo(self,x1, y1):
+    def lineTo(self, x1, y1):
         self.mpath.lineTo(x1, y1)
-    def rCubicTo(self,x1, y1, x2, y2,x3,y3):
-        self.mpath.rCubicTo(x1, y1, x2, y2,x3,y3)
 
-    def rMoveTo(self,x1, y1):
+    def rCubicTo(self, x1, y1, x2, y2, x3, y3):
+        self.mpath.rCubicTo(x1, y1, x2, y2, x3, y3)
+
+    def rMoveTo(self, x1, y1):
         self.mpath.rMoveTo(x1, y1)
 
     def reset(self):
         self.mpath.reset()
 
     def rewind(self):
         self.mpath.rewind()
 
-    def moveTo(self,x1, y1):
+    def moveTo(self, x1, y1):
         self.mpath.moveTo(x1, y1)
 
-    def rQuadTo(self, dx1,  dy1,  dx2,  dy2):
-        self.mpath.rQuadTo(dx1,  dy1,  dx2,  dy2)
+    def rQuadTo(self, dx1, dy1, dx2, dy2):
+        self.mpath.rQuadTo(dx1, dy1, dx2, dy2)
 
-    def addArc(self,  left,  top,  right,  bottom,  startAngle,  sweepAngle):
-        self.mpath.addArc( left,  top,  right,  bottom,  startAngle,  sweepAngle)
+    def addArc(self, left, top, right, bottom, startAngle, sweepAngle):
+        self.mpath.addArc(left, top, right, bottom, startAngle, sweepAngle)
 
-    def addCircle(self, x,  y,  radius,  dir):
-        self.mpath.addCircle(x,  y,  radius,  dir)
+    def addCircle(self, x, y, radius, dir):
+        self.mpath.addCircle(x, y, radius, dir)
 
-    def addOval(self,  left,  top,  right,  bottom,  dir):
-        self.mpath.addOval(left,  top,  right,  bottom,  dir)
+    def addOval(self, left, top, right, bottom, dir):
+        self.mpath.addOval(left, top, right, bottom, dir)
 
-    def addRect(self,  left,  top,  right,  bottom,  dir):
-        self.mpath.addRect(left,  top,  right,  bottom,  dir)
+    def addRect(self, left, top, right, bottom, dir):
+        self.mpath.addRect(left, top, right, bottom, dir)
 
-    def addRoundRect(self,  left,  top,  right,  bottom,  rx,  ry,  dir):
-        self.mpath.addRoundRect( left,  top,  right,  bottom,  rx,  ry,  dir)
+    def addRoundRect(self, left, top, right, bottom, rx, ry, dir):
+        self.mpath.addRoundRect(left, top, right, bottom, rx, ry, dir)
 
-    def arcTo(self,  left,  top,  right,  bottom,  startAngle,  sweepAngle,  forceMoveTo):
-        self.mpath.arcTo(  left,  top,  right,  bottom,  startAngle,  sweepAngle,  forceMoveTo)
+    def arcTo(self, left, top, right, bottom, startAngle, sweepAngle, forceMoveTo):
+        self.mpath.arcTo(left, top, right, bottom, startAngle, sweepAngle, forceMoveTo)
 
-    def cubicTo(self,   x1,  y1,  x2,  y2,  x3,  y3):
-        self.mpath.cubicTo(x1,  y1,  x2,  y2,  x3,  y3)
+    def cubicTo(self, x1, y1, x2, y2, x3, y3):
+        self.mpath.cubicTo(x1, y1, x2, y2, x3, y3)
 
-    def setLastPoint(self,  dx,  dy):
-        self.mpath.setLastPoint(dx,dy)
+    def setLastPoint(self, dx, dy):
+        self.mpath.setLastPoint(dx, dy)
 
     def close(self):
         self.mpath.close()
 
-    def rLineTo(self,  dx,  dy):
-        self.mpath.rLineTo( dx,  dy)
+    def rLineTo(self, dx, dy):
+        self.mpath.rLineTo(dx, dy)
+
 
-def gesture(paths:List[Path],listener=None):
+def gesture(paths: List[Path], listener=None):
     py_paths = []
     for p in paths:
         py_paths.append(p.mpath)
 
-    asgesture.perform(py_paths,listener)
+    asgesture.perform(py_paths, listener)
```

### Comparing `ascript-tip-0.0.3.39/ascript/android/media.py` & `ascript-tip-0.0.3.40/ascript/android/media.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/android/node.py` & `ascript-tip-0.0.3.40/ascript/android/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,18 @@
 
     def find(self) -> Node:
         res = self.find_all(1)
         if res and len(res)>0:
             return res[0]
         return None
 
+    @staticmethod
+    def cache(is_cache:bool):
+        asSelector.cache(is_cache)
+
     def find_all(self,num:int=999999)-> List[Node]:
         nodes = self.sel.find_all()
         res = []
         if nodes:
             for n in nodes:
                 res.append(Node(n))
```

### Comparing `ascript-tip-0.0.3.39/ascript/android/screen.py` & `ascript-tip-0.0.3.40/ascript/android/screen.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/android/system.py` & `ascript-tip-0.0.3.40/ascript/android/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from airscript.system import Channel as asChannel
 from airscript.data import Kv as asKv
 from airscript.intent import Intent  as asIntent
 
 
 class R:
     name = asR.moudle_name
-    context = asR.context
+    context = asR.context()
+    package_name = asR.context().getPackageName()
 
     @staticmethod
     def res(child_path=None):
         if child_path:
             file_path = child_path.lstrip("/")
             file_path =  os.path.join(asR.module_path,"res",file_path)
             return file_path
@@ -44,14 +45,25 @@
 
     @staticmethod
     def sd(child_path=None):
         if child_path:
             return asR.sd(child_path)
         return asR.sd()
 
+    @staticmethod
+    def rel(path:str=__file__,rel_path:str=None):
+        if not os.path.isdir(path):
+            path = os.path.dirname(path)
+
+        real_path = os.path.join(path, rel_path)
+        real_path = os.path.normpath(real_path)
+
+        return real_path
+
+
 
 def exit():
     asR.exit()
 
 def reboot(delay_time:int=0):
     asR.reboot(delay_time)
 
@@ -122,8 +134,10 @@
 class KeyValue:
     @staticmethod
     def save(key:str,value):
         asKv.save(key,value)
 
     @staticmethod
     def get(key:str,default_value):
-        return asKv.get(key,default_value)
+        return asKv.get(key,default_value)
+
+
```

### Comparing `ascript-tip-0.0.3.39/ascript/windows/action.py` & `ascript-tip-0.0.3.40/ascript/windows/action.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.css` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.css.map` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.min.css` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.min.css.map` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.css` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.css.map` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.min.css` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.min.css.map` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.css` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.css.map` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.min.css` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.min.css.map` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.js.map` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.min.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.min.js.map` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.js.map` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.min.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.min.js.map` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-4.6.2-dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/arrow-repeat.svg` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/arrow-repeat.svg`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.css` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.json` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.min.css` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.scss` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/fonts/bootstrap-icons.woff` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/fonts/bootstrap-icons.woff2` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/font/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/trash.svg` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/trash.svg`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/bootstrap-icons-1.11.2/zoom-in.svg` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/bootstrap-icons-1.11.2/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/css/colors.css` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/css/colors.css`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_app.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_app.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_apps.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_apps.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_capture.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_capture.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_close.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_close.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_config.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_config.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_dev.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_dev.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_floder.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_floder.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_home.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_home.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_log.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_log.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_min.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_min.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_package.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_package.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_pic.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_pic.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_pycharm.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_pycharm.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_python.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_python.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_python_20.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_python_20.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_python_32.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_python_32.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_run.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_run.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_setting.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_setting.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_stop.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_stop.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_tool.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_tool.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/ico_win.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/ico_win.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/img/logo.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/css/zTreeStyle.css` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/css/zTreeStyle.css`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/1_close.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/1_close.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/1_open.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/1_open.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/2.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/2.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/3.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/3.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/5.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/5.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/7.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/7.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/diy/8.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/diy/8.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/tree-node-btn.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/tree-node-btn.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/zTreeStandard.gif` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/zTreeStandard.gif`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/img/zTreeStandard.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/img/zTreeStandard.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/jquery-zTree/js/jquery.ztree.all.min.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/jquery-zTree/js/jquery.ztree.all.min.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/js/base.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/js/base.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/js/colors/colors.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/js/colors/colors.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/js/colors/colors_choosecolor.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/js/colors/colors_choosecolor.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/js/colors/colors_findimage.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/js/colors/colors_findimage.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/js/colors/ocr.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/js/colors/ocr.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/js/hwnd.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/js/hwnd.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/js/jquery-3.7.js` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/js/jquery-3.7.js`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/bar.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/bar.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/config.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/config.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/home.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/home.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/hwnd.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/hwnd.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/item_app.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/item_app.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/log.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/log.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/main.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/main.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/pycharminstall.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/pycharminstall.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/pyinstall.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/pyinstall.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/step.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/step.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/pyui/workspace.ui` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/pyui/workspace.ui`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/templates/base.html` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/templates/base.html`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/templates/colors.html` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/templates/colors.html`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/templates/hwnd.html` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/templates/hwnd.html`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/assets/tools/capture/1708245806.png` & `ascript-tip-0.0.3.40/ascript/windows/client/assets/tools/capture/1708245806.png`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/dao/server_dao.py` & `ascript-tip-0.0.3.40/ascript/windows/client/dao/server_dao.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/server.py` & `ascript-tip-0.0.3.40/ascript/windows/client/server.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/tools.py` & `ascript-tip-0.0.3.40/ascript/windows/client/tools.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/ui.py` & `ascript-tip-0.0.3.40/ascript/windows/client/ui.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/client/worker.py` & `ascript-tip-0.0.3.40/ascript/windows/client/worker.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/daos/screen.py` & `ascript-tip-0.0.3.40/ascript/windows/daos/screen.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/screen.py` & `ascript-tip-0.0.3.40/ascript/windows/screen.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/system.py` & `ascript-tip-0.0.3.40/ascript/windows/system.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/utils/airclickcv.py` & `ascript-tip-0.0.3.40/ascript/windows/utils/airclickcv.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/utils/screen_utils.py` & `ascript-tip-0.0.3.40/ascript/windows/utils/screen_utils.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript/windows/window.py` & `ascript-tip-0.0.3.40/ascript/windows/window.py`

 * *Files identical despite different names*

### Comparing `ascript-tip-0.0.3.39/ascript_tip.egg-info/SOURCES.txt` & `ascript-tip-0.0.3.40/ascript_tip.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 setup.py
 ascript/__init__.py
 ascript/android/__init__.py
 ascript/android/action.py
 ascript/android/data.py
 ascript/android/media.py
 ascript/android/node.py
+ascript/android/plug.py
 ascript/android/screen.py
 ascript/android/system.py
 ascript/android/ui.py
+ascript/android/screen/__init__.py
+ascript/android/screen/ascv.py
+ascript/android/screen/gp.py
+ascript/android/screen/gp_tasks.py
+ascript/android/screen/gp_tool.py
 ascript/windows/__init__.py
 ascript/windows/action.py
 ascript/windows/screen.py
 ascript/windows/system.py
 ascript/windows/window.py
 ascript/windows/client/__init__.py
 ascript/windows/client/server.py
```

### Comparing `ascript-tip-0.0.3.39/setup.py` & `ascript-tip-0.0.3.40/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pip._internal.req import req_file
 from setuptools.glob import glob
 
-VERSION = '0.0.3.39'
-DESCRIPTION = 'ascript 相关python包'
+VERSION = '0.0.3.40'
+DESCRIPTION = 'ascript Python库'
 is_tip = True
 include_data = True
 libname = "ascript"
 requirments = req_file.parse_requirements('requirements.txt', session='hack')
 instll_requires = [req.requirement for req in requirments]
 
 if is_tip:
```

