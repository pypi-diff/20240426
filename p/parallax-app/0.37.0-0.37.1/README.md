# Comparing `tmp/parallax_app-0.37.0.tar.gz` & `tmp/parallax_app-0.37.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallax_app-0.37.0.tar", last modified: Tue Apr 23 17:19:21 2024, max compression
+gzip compressed data, was "parallax_app-0.37.1.tar", last modified: Fri Apr 26 19:23:07 2024, max compression
```

## Comparing `parallax_app-0.37.0.tar` & `parallax_app-0.37.1.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:19:21.692225 parallax_app-0.37.0/
--rw-rw-rw-   0        0        0      304 2024-04-23 17:15:24.000000 parallax_app-0.37.0/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-11-14 21:33:47.000000 parallax_app-0.37.0/LICENSE
--rw-rw-rw-   0        0        0     2581 2024-04-23 17:19:21.691225 parallax_app-0.37.0/PKG-INFO
--rw-rw-rw-   0        0        0     1515 2024-04-01 18:06:06.000000 parallax_app-0.37.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 17:19:21.621224 parallax_app-0.37.0/docs/
--rw-rw-rw-   0        0        0      654 2024-04-01 18:06:06.000000 parallax_app-0.37.0/docs/Makefile
--rw-rw-rw-   0        0        0     1114 2024-04-01 18:06:06.000000 parallax_app-0.37.0/docs/ReadMe.rst
--rw-rw-rw-   0        0        0     1110 2024-04-22 16:27:11.000000 parallax_app-0.37.0/docs/conf.py
--rw-rw-rw-   0        0        0      481 2024-04-01 18:06:06.000000 parallax_app-0.37.0/docs/index.rst
--rwxrwxrwx   0        0        0      800 2024-04-01 18:06:06.000000 parallax_app-0.37.0/docs/make.bat
--rw-rw-rw-   0        0        0       92 2024-04-01 18:06:06.000000 parallax_app-0.37.0/docs/modules.rst
--rw-rw-rw-   0        0        0     3826 2024-04-01 18:06:06.000000 parallax_app-0.37.0/docs/parallax.rst
-drwxrwxrwx   0        0        0        0 2024-04-23 17:19:21.630224 parallax_app-0.37.0/img/
--rw-rw-rw-   0        0        0     4622 2023-11-14 21:33:47.000000 parallax_app-0.37.0/img/arrow-right.png
--rw-rw-rw-   0        0        0     1257 2023-11-14 21:33:47.000000 parallax_app-0.37.0/img/gear.png
--rw-rw-rw-   0        0        0     1145 2023-11-14 21:33:47.000000 parallax_app-0.37.0/img/recordingButton.png
--rw-rw-rw-   0        0        0    28195 2023-11-14 21:33:47.000000 parallax_app-0.37.0/img/sextant.png
--rw-rw-rw-   0        0        0     7808 2023-11-14 21:33:47.000000 parallax_app-0.37.0/img/snapshotButton_white.png
--rw-rw-rw-   0        0        0    11773 2023-11-14 21:33:47.000000 parallax_app-0.37.0/img/stop-sign.png
--rw-rw-rw-   0        0        0    22337 2023-11-14 21:33:47.000000 parallax_app-0.37.0/img/target.png
-drwxrwxrwx   0        0        0        0 2024-04-23 17:19:21.650224 parallax_app-0.37.0/parallax/
--rw-rw-rw-   0        0        0      131 2024-04-23 17:13:07.000000 parallax_app-0.37.0/parallax/__init__.py
--rw-rw-rw-   0        0        0     2386 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/__main__.py
--rw-rw-rw-   0        0        0    19816 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/calibration_camera.py
--rw-rw-rw-   0        0        0    27387 2024-04-01 18:06:06.000000 parallax_app-0.37.0/parallax/camera.py
--rw-rw-rw-   0        0        0    11095 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/curr_bg_cmp_processor.py
--rw-rw-rw-   0        0        0     8926 2024-04-01 18:06:06.000000 parallax_app-0.37.0/parallax/curr_prev_cmp_processor.py
--rw-rw-rw-   0        0        0    32086 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/main_window_wip.py
--rw-rw-rw-   0        0        0     4766 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/mask_generator.py
--rw-rw-rw-   0        0        0     5321 2024-04-23 17:15:24.000000 parallax_app-0.37.0/parallax/model.py
--rw-rw-rw-   0        0        0     3769 2024-04-01 18:06:06.000000 parallax_app-0.37.0/parallax/no_filter.py
--rw-rw-rw-   0        0        0    12355 2024-04-23 17:12:57.000000 parallax_app-0.37.0/parallax/probe_calibration.py
--rw-rw-rw-   0        0        0    10322 2024-04-23 17:15:24.000000 parallax_app-0.37.0/parallax/probe_detect_manager.py
--rw-rw-rw-   0        0        0    17672 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/probe_detector.py
--rw-rw-rw-   0        0        0     6202 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/probe_fine_tip_detector.py
--rw-rw-rw-   0        0        0     4641 2024-04-01 18:06:06.000000 parallax_app-0.37.0/parallax/recording_manager.py
--rw-rw-rw-   0        0        0    10738 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/reticle_detect_manager.py
--rw-rw-rw-   0        0        0    22122 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/reticle_detection.py
--rw-rw-rw-   0        0        0     6809 2024-04-01 18:06:06.000000 parallax_app-0.37.0/parallax/reticle_detection_coords_interests.py
--rw-rw-rw-   0        0        0    12642 2024-04-23 17:15:24.000000 parallax_app-0.37.0/parallax/screen_widget.py
--rw-rw-rw-   0        0        0    17862 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/stage_listener.py
--rw-rw-rw-   0        0        0     4188 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/stage_ui.py
--rw-rw-rw-   0        0        0    25380 2024-04-23 17:15:24.000000 parallax_app-0.37.0/parallax/stage_widget.py
--rw-rw-rw-   0        0        0     6763 2024-04-22 16:27:11.000000 parallax_app-0.37.0/parallax/user_setting_manager.py
--rw-rw-rw-   0        0        0     3345 2024-04-01 18:06:06.000000 parallax_app-0.37.0/parallax/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:19:21.690225 parallax_app-0.37.0/parallax_app.egg-info/
--rw-rw-rw-   0        0        0     2581 2024-04-23 17:19:21.000000 parallax_app-0.37.0/parallax_app.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1719 2024-04-23 17:19:21.000000 parallax_app-0.37.0/parallax_app.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:19:21.000000 parallax_app-0.37.0/parallax_app.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      193 2024-04-23 17:19:21.000000 parallax_app-0.37.0/parallax_app.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-23 17:19:21.000000 parallax_app-0.37.0/parallax_app.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1397 2024-04-23 16:37:03.000000 parallax_app-0.37.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 17:19:21.692225 parallax_app-0.37.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2024-04-23 16:37:03.000000 parallax_app-0.37.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:19:21.666224 parallax_app-0.37.0/tests/
--rw-rw-rw-   0        0        0      536 2024-04-01 18:06:06.000000 parallax_app-0.37.0/tests/camera.py
--rw-rw-rw-   0        0        0      184 2024-04-01 18:06:06.000000 parallax_app-0.37.0/tests/model.py
--rw-rw-rw-   0        0        0      457 2024-04-01 18:06:06.000000 parallax_app-0.37.0/tests/screen_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:19:21.674225 parallax_app-0.37.0/ui/
--rw-rw-rw-   0        0        0   192973 2024-01-02 17:20:46.000000 parallax_app-0.37.0/ui/ParallaxReadME.JPG
-drwxrwxrwx   0        0        0        0 2024-04-23 17:19:21.675225 parallax_app-0.37.0/ui/font/
--rw-rw-rw-   0        0        0   259308 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/font/FiraCode-VariableFont_wght.ttf
--rw-rw-rw-   0        0        0     9977 2024-04-01 18:06:06.000000 parallax_app-0.37.0/ui/mainWindow.ui
--rw-rw-rw-   0        0        0     4500 2024-04-22 16:27:11.000000 parallax_app-0.37.0/ui/probe_calib.ui
-drwxrwxrwx   0        0        0        0 2024-04-23 17:19:21.689225 parallax_app-0.37.0/ui/resources/
--rw-rw-rw-   0        0        0     4622 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/resources/arrow-right.png
--rw-rw-rw-   0        0        0      934 2024-04-22 16:27:11.000000 parallax_app-0.37.0/ui/resources/check.png
--rw-rw-rw-   0        0        0     1257 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/resources/gear.png
--rw-rw-rw-   0        0        0     4794 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/resources/recordingButton.png
--rw-rw-rw-   0        0        0     4781 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/resources/recordingButton_disabled.png
--rw-rw-rw-   0        0        0    28195 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/resources/sextant.png
--rw-rw-rw-   0        0        0    13098 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/resources/snapshotButton_disabled.png
--rw-rw-rw-   0        0        0     8144 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/resources/snapshotButton_green.png
--rw-rw-rw-   0        0        0    15545 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/resources/snapshotButton_white.png
--rw-rw-rw-   0        0        0    11773 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/resources/stop-sign.png
--rw-rw-rw-   0        0        0    22337 2023-11-14 21:33:47.000000 parallax_app-0.37.0/ui/resources/target.png
--rw-rw-rw-   0        0        0      436 2024-04-22 16:27:11.000000 parallax_app-0.37.0/ui/resources/x.png
--rw-rw-rw-   0        0        0     4019 2024-04-22 16:27:11.000000 parallax_app-0.37.0/ui/reticle_calib.ui
--rw-rw-rw-   0        0        0    10881 2024-01-17 23:10:00.000000 parallax_app-0.37.0/ui/settingPopUpMenu.ui
--rw-rw-rw-   0        0        0    10735 2024-04-22 16:27:11.000000 parallax_app-0.37.0/ui/stage_info.ui
+drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.389256 parallax_app-0.37.1/
+-rw-rw-rw-   0        0        0      345 2024-04-26 18:57:43.000000 parallax_app-0.37.1/.gitignore
+-rw-rw-rw-   0        0        0      284 2024-04-26 18:57:43.000000 parallax_app-0.37.1/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1113 2024-04-26 18:57:43.000000 parallax_app-0.37.1/LICENSE
+-rw-rw-rw-   0        0        0     3081 2024-04-26 19:23:07.388255 parallax_app-0.37.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1892 2024-04-26 18:57:43.000000 parallax_app-0.37.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.264814 parallax_app-0.37.1/docs/
+-rw-rw-rw-   0        0        0      654 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/Makefile
+-rw-rw-rw-   0        0        0     1606 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/ReadMe.rst
+-rw-rw-rw-   0        0        0     1110 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/conf.py
+-rw-rw-rw-   0        0        0      481 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/index.rst
+-rwxrwxrwx   0        0        0      800 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/make.bat
+-rw-rw-rw-   0        0        0       92 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/modules.rst
+-rw-rw-rw-   0        0        0     3826 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/parallax.rst
+-rw-rw-rw-   0        0        0       26 2024-04-26 18:57:43.000000 parallax_app-0.37.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.296815 parallax_app-0.37.1/img/
+-rw-rw-rw-   0        0        0     4622 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/arrow-right.png
+-rw-rw-rw-   0        0        0     1257 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/gear.png
+-rw-rw-rw-   0        0        0     1145 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/recordingButton.png
+-rw-rw-rw-   0        0        0    28195 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/sextant.png
+-rw-rw-rw-   0        0        0     7808 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/snapshotButton_white.png
+-rw-rw-rw-   0        0        0    11773 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/stop-sign.png
+-rw-rw-rw-   0        0        0    22337 2024-04-26 18:57:43.000000 parallax_app-0.37.1/img/target.png
+drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.317207 parallax_app-0.37.1/parallax/
+-rw-rw-rw-   0        0        0      137 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/__init__.py
+-rw-rw-rw-   0        0        0     2323 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/__main__.py
+-rw-rw-rw-   0        0        0    20640 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/calibration_camera.py
+-rw-rw-rw-   0        0        0    28521 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/camera.py
+-rw-rw-rw-   0        0        0    11558 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/curr_bg_cmp_processor.py
+-rw-rw-rw-   0        0        0     9100 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/curr_prev_cmp_processor.py
+-rw-rw-rw-   0        0        0    33169 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/main_window_wip.py
+-rw-rw-rw-   0        0        0     4852 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/mask_generator.py
+-rw-rw-rw-   0        0        0     5288 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/model.py
+-rw-rw-rw-   0        0        0     3747 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/no_filter.py
+-rw-rw-rw-   0        0        0    13008 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/probe_calibration.py
+-rw-rw-rw-   0        0        0    12242 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/probe_detect_manager.py
+-rw-rw-rw-   0        0        0    18723 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/probe_detector.py
+-rw-rw-rw-   0        0        0     6451 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/probe_fine_tip_detector.py
+-rw-rw-rw-   0        0        0     4681 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/recording_manager.py
+-rw-rw-rw-   0        0        0    11329 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/reticle_detect_manager.py
+-rw-rw-rw-   0        0        0    22539 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/reticle_detection.py
+-rw-rw-rw-   0        0        0     6712 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/reticle_detection_coords_interests.py
+-rw-rw-rw-   0        0        0    12601 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/screen_widget.py
+-rw-rw-rw-   0        0        0    18015 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/stage_listener.py
+-rw-rw-rw-   0        0        0     4334 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/stage_ui.py
+-rw-rw-rw-   0        0        0    25986 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/stage_widget.py
+-rw-rw-rw-   0        0        0     6843 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/user_setting_manager.py
+-rw-rw-rw-   0        0        0     3364 2024-04-26 18:57:43.000000 parallax_app-0.37.1/parallax/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.386256 parallax_app-0.37.1/parallax_app.egg-info/
+-rw-rw-rw-   0        0        0     3081 2024-04-26 19:23:07.000000 parallax_app-0.37.1/parallax_app.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1774 2024-04-26 19:23:07.000000 parallax_app-0.37.1/parallax_app.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 19:23:07.000000 parallax_app-0.37.1/parallax_app.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      234 2024-04-26 19:23:07.000000 parallax_app-0.37.1/parallax_app.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-26 19:23:07.000000 parallax_app-0.37.1/parallax_app.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1753 2024-04-26 18:57:43.000000 parallax_app-0.37.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 19:23:07.389256 parallax_app-0.37.1/setup.cfg
+-rw-rw-rw-   0        0        0      216 2024-04-26 18:57:43.000000 parallax_app-0.37.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.344233 parallax_app-0.37.1/tests/
+-rw-rw-rw-   0        0        0      479 2024-04-26 18:57:43.000000 parallax_app-0.37.1/tests/test_camera.py
+-rw-rw-rw-   0        0        0      405 2024-04-26 18:57:43.000000 parallax_app-0.37.1/tests/test_model.py
+-rw-rw-rw-   0        0        0     1579 2024-04-26 18:57:43.000000 parallax_app-0.37.1/tests/test_screen_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.355255 parallax_app-0.37.1/ui/
+-rw-rw-rw-   0        0        0   192973 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/ParallaxReadME.JPG
+drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.355255 parallax_app-0.37.1/ui/font/
+-rw-rw-rw-   0        0        0   259308 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/font/FiraCode-VariableFont_wght.ttf
+-rw-rw-rw-   0        0        0     9977 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/mainWindow.ui
+-rw-rw-rw-   0        0        0     4500 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/probe_calib.ui
+drwxrwxrwx   0        0        0        0 2024-04-26 19:23:07.385255 parallax_app-0.37.1/ui/resources/
+-rw-rw-rw-   0        0        0     4622 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/arrow-right.png
+-rw-rw-rw-   0        0        0      934 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/check.png
+-rw-rw-rw-   0        0        0     1257 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/gear.png
+-rw-rw-rw-   0        0        0     4794 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/recordingButton.png
+-rw-rw-rw-   0        0        0     4781 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/recordingButton_disabled.png
+-rw-rw-rw-   0        0        0    28195 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/sextant.png
+-rw-rw-rw-   0        0        0    13098 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/snapshotButton_disabled.png
+-rw-rw-rw-   0        0        0     8144 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/snapshotButton_green.png
+-rw-rw-rw-   0        0        0    15545 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/snapshotButton_white.png
+-rw-rw-rw-   0        0        0    11773 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/stop-sign.png
+-rw-rw-rw-   0        0        0    22337 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/target.png
+-rw-rw-rw-   0        0        0      436 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/resources/x.png
+-rw-rw-rw-   0        0        0     4019 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/reticle_calib.ui
+-rw-rw-rw-   0        0        0    10881 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/settingPopUpMenu.ui
+-rw-rw-rw-   0        0        0    10735 2024-04-26 18:57:43.000000 parallax_app-0.37.1/ui/stage_info.ui
```

### Comparing `parallax_app-0.37.0/LICENSE` & `parallax_app-0.37.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/PKG-INFO` & `parallax_app-0.37.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallax-app
-Version: 0.37.0
+Version: 0.37.1
 Summary: GUI software for photogrammetry-assisted probe targeting in electrophysiology
 Author-email: Hanna Lee <hanna.lee@alleninstitute.org>
 License: Allen Institute Software License
 Keywords: parallax
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
@@ -15,20 +15,23 @@
 Requires-Dist: opencv-python
 Requires-Dist: spinnaker-python
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: scikit-image
 Requires-Dist: requests
 Requires-Dist: scikit-learn
+Provides-Extra: dev
+Requires-Dist: parallax-app[linters]; extra == "dev"
 Provides-Extra: linters
 Requires-Dist: codespell; extra == "linters"
 Requires-Dist: coverage; extra == "linters"
 Requires-Dist: flake8; extra == "linters"
 Requires-Dist: interrogate; extra == "linters"
 Requires-Dist: isort; extra == "linters"
+Requires-Dist: pytest-mock; extra == "linters"
 Provides-Extra: docs
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-jinja; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 
 # Parallax
 
@@ -39,41 +42,60 @@
 
 ### Prerequisites
 - Python~=3.8 (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
 - PySpin (for Linux or Mac OS users)
 
 
 ### Installation
-1. Clone the repository:
-```bash
-git clone https://github.com/AllenNeuralDynamics/parallax.git
-```
-
-2. Create virtual environment and activate it:
+1. Create virtual environment and activate it:
 - On Windows:
 ```bash
 python -m venv venv
 ./venv/Scripts/activate
 ```
 - On Linux/Mac:
 ```bash
 python -m venv venv
 source venv/bin/activate
 ```
 
-3. Install Dependencies:
+2. To install the latest version:
 ```bash
-python -m pip install -e .
+pip install parallax-app
+```
+To upgrate to the latest version:
+```bash
+pip install parallax-app --upgrade
 ```
 
 ### Running Parallax
 ```bash
 python -m parallax
 ```
 
+### Development mode
+1. Clone the repository:
+```bash
+git clone https://github.com/AllenNeuralDynamics/parallax.git
+```
+2. Install Dependencies:
+```bash
+pip install -e .[dev]
+```
+
+### Documentation
+1. To install the dependencies:
+```bash
+pip install -e .[docs]
+```
+2. Then to create the documentation html files, run:
+```bash
+sphinx-build -b html docs/ docs/_build
+```
+
 ### Additional Setup for Linux and Mac OS
 For Linux or Mac OS, you'll need to install PySpin manually (not required for
 Windows):
 * download the Spinnaker SDK package for your system from [here](https://flir.app.boxcn.net/v/SpinnakerSDK)
 * follow the installation instructions in the README
 * Install the Python bindings found alongside the SDK package
```

### Comparing `parallax_app-0.37.0/README.md` & `parallax_app-0.37.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,41 +7,60 @@
 
 ### Prerequisites
 - Python~=3.8 (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
 - PySpin (for Linux or Mac OS users)
 
 
 ### Installation
-1. Clone the repository:
-```bash
-git clone https://github.com/AllenNeuralDynamics/parallax.git
-```
-
-2. Create virtual environment and activate it:
+1. Create virtual environment and activate it:
 - On Windows:
 ```bash
 python -m venv venv
 ./venv/Scripts/activate
 ```
 - On Linux/Mac:
 ```bash
 python -m venv venv
 source venv/bin/activate
 ```
 
-3. Install Dependencies:
+2. To install the latest version:
 ```bash
-python -m pip install -e .
+pip install parallax-app
+```
+To upgrate to the latest version:
+```bash
+pip install parallax-app --upgrade
 ```
 
 ### Running Parallax
 ```bash
 python -m parallax
 ```
 
+### Development mode
+1. Clone the repository:
+```bash
+git clone https://github.com/AllenNeuralDynamics/parallax.git
+```
+2. Install Dependencies:
+```bash
+pip install -e .[dev]
+```
+
+### Documentation
+1. To install the dependencies:
+```bash
+pip install -e .[docs]
+```
+2. Then to create the documentation html files, run:
+```bash
+sphinx-build -b html docs/ docs/_build
+```
+
 ### Additional Setup for Linux and Mac OS
 For Linux or Mac OS, you'll need to install PySpin manually (not required for
 Windows):
 * download the Spinnaker SDK package for your system from [here](https://flir.app.boxcn.net/v/SpinnakerSDK)
 * follow the installation instructions in the README
 * Install the Python bindings found alongside the SDK package
```

### Comparing `parallax_app-0.37.0/docs/Makefile` & `parallax_app-0.37.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/docs/ReadMe.rst` & `parallax_app-0.37.1/docs/ReadMe.rst`

 * *Files 12% similar despite different names*

```diff
@@ -12,42 +12,73 @@
 - Python~=3.8 (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
 - PySpin (for Linux or Mac OS users)
 
 
 Installing and Upgrading
 =========================
 
-1. To install the latest version:
-
-.. code-block:: bash
-
-   git clone https://github.com/AllenNeuralDynamics/parallax.git
-
-2. Create virtual environment and activate it:
-
+1. Create virtual environment and activate it:
 - On Windows:
 
 .. code-block:: bash
 
    python -m venv venv
    ./venv/Scripts/activate
 
 - On Linux/Mac:
 
 .. code-block:: bash
 
    python -m venv venv
    source venv/bin/activate
 
-3. Install Dependencies:
+2. To install the latest version:
 
 .. code-block:: bash
 
-   python -m pip install -e.
+   pip install parallax-app
+
+To upgrate to the latest version:
+
+.. code-block:: bash
 
+   pip install parallax-app --upgrade
 
 Running Parallax
 =========================
 
 .. code-block:: bash
 
-   python -m parallax
+   python -m parallax
+
+   
+Development mode
+=========================
+
+1. Clone the repository:
+
+.. code-block:: bash
+
+   git clone https://github.com/AllenNeuralDynamics/parallax.git
+
+2. Install Dependencies:
+
+.. code-block:: bash
+
+   pip install -e .[dev]
+
+
+Documentation
+=========================
+
+1. To install the dependencies:
+
+.. code-block:: bash
+
+   pip install -e .[docs]
+
+2. Then to create the documentation html files, run:
+
+.. code-block:: bash
+
+   sphinx-build -b html docs/ docs/_build
+
```

### Comparing `parallax_app-0.37.0/docs/conf.py` & `parallax_app-0.37.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/docs/make.bat` & `parallax_app-0.37.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/docs/parallax.rst` & `parallax_app-0.37.1/docs/parallax.rst`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/img/arrow-right.png` & `parallax_app-0.37.1/img/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/img/gear.png` & `parallax_app-0.37.1/img/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/img/recordingButton.png` & `parallax_app-0.37.1/img/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/img/sextant.png` & `parallax_app-0.37.1/img/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/img/snapshotButton_white.png` & `parallax_app-0.37.1/img/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/img/stop-sign.png` & `parallax_app-0.37.1/img/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/img/target.png` & `parallax_app-0.37.1/img/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/parallax/__main__.py` & `parallax_app-0.37.1/parallax/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,74 @@
 """
 Parallax: A GUI application for controlling hardware devices.
 """
-# Import necessary libraries and modules for the GUI application
-from PyQt5.QtWidgets import QApplication
-from parallax.model import Model
-from parallax.main_window_wip import MainWindow as MainWindowV2
-import atexit
+
 import argparse
+import atexit
 import logging
 import os
 
+from PyQt5.QtWidgets import QApplication
+
+from parallax.main_window_wip import MainWindow as MainWindowV2
+from parallax.model import Model
+
+
 def setup_logging():
     """Set up logging to file."""
     logger = logging.getLogger()
     logger.handlers.clear()
     logger.setLevel(logging.WARNING)
-    
+
     # Create the directory if it doesn't exist
     package_dir = os.path.dirname(os.path.abspath(__file__))
-    debug_dir = os.path.join(os.path.dirname(package_dir), 'debug')
+    debug_dir = os.path.join(os.path.dirname(package_dir), "debug")
     os.makedirs(debug_dir, exist_ok=True)
-    log_file_path = os.path.join(debug_dir, 'parallax_debug.log')
+    log_file_path = os.path.join(debug_dir, "parallax_debug.log")
 
-    with open(log_file_path, 'w') as log_file:
+    with open(log_file_path, "w") as log_file:
         # Clear the log file
         pass
-    
+
     log_handler = logging.FileHandler(log_file_path)
     log_handler.setLevel(logging.DEBUG)
     log_handler.setFormatter(
-        logging.Formatter(fmt='%(asctime)s:%(name)s:%(levelname)s: %(message)s')
+        logging.Formatter(
+            fmt="%(asctime)s:%(name)s:%(levelname)s: %(message)s"
+        )
     )
-    logger.addHandler(log_handler)    
+    logger.addHandler(log_handler)
+
 
 # Main function to run the Parallax application
-if __name__ == '__main__':
+if __name__ == "__main__":
     # Parse command line arguments to configure application behavior
     parser = argparse.ArgumentParser()
-    parser.add_argument('-d', '--dummy', action='store_true', help='Dummy mode for testing without hardware')
+    parser.add_argument(
+        "-d",
+        "--dummy",
+        action="store_true",
+        help="Dummy mode for testing without hardware",
+    )
     args = parser.parse_args()
 
     # Print a message if running in dummy mode (no hardware interaction)
     if args.dummy:
-        print('\nRunning in dummy mode; hardware devices will be inaccessible.')
+        print("\nRunning in dummy mode; hardware devices not accessible.")
 
     # Set up logging as configured in the setup_logging function
     setup_logging()
 
     # Initialize the Qt application
     app = QApplication([])
     model = Model(version="V2")  # Initialize the data model with version "V2"
-    main_window = MainWindowV2(model, dummy=args.dummy)  # Version 2 of the main window
+    main_window = MainWindowV2(model, dummy=args.dummy)  # main window
 
     # Show the main window on screen
     main_window.show()
     # Start the Qt application's main loop
     app.exec()
 
     # Register cleanup functions to be called on program termination
     atexit.register(model.clean)  # Clean up resources used by the model
-    # Save user configurations on exit, specific to version 2 of the main window
-    atexit.register(main_window.save_user_configs)
+    # Save user configurations on exit
+    atexit.register(main_window.save_user_configs)
```

### Comparing `parallax_app-0.37.0/parallax/calibration_camera.py` & `parallax_app-0.37.1/parallax/calibration_camera.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """
 Module for camera calibration and stereo calibration.
-This module provides classes for intrinsic camera calibration (`CalibrationCamera`)
-and stereo camera calibration (`CalibrationStereo`).
+This module provides classes for intrinsic camera calibration
+(`CalibrationCamera`) and stereo camera calibration (`CalibrationStereo`).
 Classes:
 -CalibrationCamera: Class for intrinsic camera calibration.
 -CalibrationStereo: Class for stereo camera calibration.
 """
-import numpy as np
-import cv2
+
 import logging
 
+import cv2
+import numpy as np
+
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+# Set the logging level for PyQt5.uic.uiparser/properties
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.DEBUG)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.DEBUG)
 
 # Objectpoints
-WORLD_SCALE = 0.2   # 200 um per tick mark --> Translation matrix will be in mm
+WORLD_SCALE = 0.2  # 200 um per tick mark --> Translation matrix will be in mm
 X_COORDS_HALF = 15
 Y_COORDS_HALF = 15
 X_COORDS = X_COORDS_HALF * 2 + 1
 Y_COORDS = Y_COORDS_HALF * 2 + 1
 OBJPOINTS = np.zeros((X_COORDS + Y_COORDS, 3), np.float32)
-OBJPOINTS[:X_COORDS, 0] = np.arange(-X_COORDS_HALF, X_COORDS_HALF+1)  # For x-coordinates
-OBJPOINTS[X_COORDS:, 1] = np.arange(-Y_COORDS_HALF, Y_COORDS_HALF+1)
+OBJPOINTS[:X_COORDS, 0] = np.arange(-X_COORDS_HALF, X_COORDS_HALF + 1)
+OBJPOINTS[X_COORDS:, 1] = np.arange(-Y_COORDS_HALF, Y_COORDS_HALF + 1)
 OBJPOINTS = OBJPOINTS * WORLD_SCALE
 OBJPOINTS = np.around(OBJPOINTS, decimals=2)
 CENTER_INDEX_X = X_COORDS_HALF
-CENTER_INDEX_Y = X_COORDS + Y_COORDS_HALF 
+CENTER_INDEX_Y = X_COORDS + Y_COORDS_HALF
 
 # Calibration
 CRIT = (cv2.TERM_CRITERIA_EPS, 0, 1e-11)
 """
 imtx = np.array([[1.52e+04, 0.0e+00, 2e+03],
                 [0.0e+00, 1.52e+04, 1.5e+03],
                 [0.0e+00, 0.0e+00, 1.0e+00]],
@@ -49,61 +51,68 @@
                     dtype=np.float32)
 """
 imtx = np.array([[1.519e+04, 0.0e+00, 2e+03],
                 [0.0e+00, 1.519e+04, 1.5e+03],
                 [0.0e+00, 0.0e+00, 1.0e+00]],
                 dtype=np.float32)
 
-idist = np.array([[ 0e+00, 0e+00, 0e+00, 0e+00, 0e+00 ]],
-                    dtype=np.float32)
+idist = np.array([[0e00, 0e00, 0e00, 0e00, 0e00]], dtype=np.float32)
 
 # Intrinsic flag
-myflags1 = cv2.CALIB_USE_INTRINSIC_GUESS | \
-            cv2.CALIB_FIX_FOCAL_LENGTH | \
-            cv2.CALIB_FIX_PRINCIPAL_POINT | \
-            cv2.CALIB_FIX_ASPECT_RATIO | \
-            cv2.CALIB_FIX_K1 | \
-            cv2.CALIB_FIX_K2 | \
-            cv2.CALIB_FIX_K3 | \
-            cv2.CALIB_FIX_TANGENT_DIST
-
-myflags2 =   cv2.CALIB_FIX_PRINCIPAL_POINT | \
-            cv2.CALIB_USE_INTRINSIC_GUESS | \
-            cv2.CALIB_FIX_ASPECT_RATIO | \
-            cv2.CALIB_FIX_FOCAL_LENGTH
+myflags1 = (
+    cv2.CALIB_USE_INTRINSIC_GUESS
+    | cv2.CALIB_FIX_FOCAL_LENGTH
+    | cv2.CALIB_FIX_PRINCIPAL_POINT
+    | cv2.CALIB_FIX_ASPECT_RATIO
+    | cv2.CALIB_FIX_K1
+    | cv2.CALIB_FIX_K2
+    | cv2.CALIB_FIX_K3
+    | cv2.CALIB_FIX_TANGENT_DIST
+)
+
+myflags2 = (
+    cv2.CALIB_FIX_PRINCIPAL_POINT
+    | cv2.CALIB_USE_INTRINSIC_GUESS
+    | cv2.CALIB_FIX_ASPECT_RATIO
+    | cv2.CALIB_FIX_FOCAL_LENGTH
+)
+
+SIZE = (4000, 3000)
 
-SIZE = (4000,3000)
 
 class CalibrationCamera:
     """Class for intrinsic calibration."""
+
     def __init__(self, camera_name):
         """Initialize the CalibrationCamera object"""
         self.name = camera_name
         self.n_interest_pixels = 15
         self.imgpoints = None
         self.objpoints = None
-        
+
     def _get_changed_data_format(self, x_axis, y_axis):
         """
         Change data format for calibration.
 
         Args:
             x_axis (list): X-axis coordinates.
             y_axis (list): Y-axis coordinates.
 
         Returns:
             numpy.ndarray: Reshaped coordinates.
         """
         x_axis = np.array(x_axis)
         y_axis = np.array(y_axis)
-        coords_lines =  np.vstack([x_axis, y_axis])
+        coords_lines = np.vstack([x_axis, y_axis])
         nCoords_per_axis = self.n_interest_pixels * 2 + 1
-        coords_lines_reshaped = coords_lines.reshape((nCoords_per_axis*2, 2)).astype(np.float32)
+        coords_lines_reshaped = coords_lines.reshape(
+            (nCoords_per_axis * 2, 2)
+        ).astype(np.float32)
         return coords_lines_reshaped
-    
+
     def _process_reticle_points(self, x_axis, y_axis):
         """
         Process reticle points for calibration.
         Args:
             x_axis (list): X-axis coordinates.
             y_axis (list): Y-axis coordinates.
         Returns:
@@ -111,15 +120,15 @@
         """
         self.objpoints = []
         self.imgpoints = []
 
         coords_lines_foramtted = self._get_changed_data_format(x_axis, y_axis)
         self.imgpoints.append(coords_lines_foramtted)
         self.objpoints.append(OBJPOINTS)
-        
+
         self.objpoints = np.array(self.objpoints)
         self.imgpoints = np.array(self.imgpoints)
         return self.imgpoints, self.objpoints
 
     def calibrate_camera(self, x_axis, y_axis):
         """
         Calibrate camera Intrinsic.
@@ -128,37 +137,52 @@
             x_axis (list): X-axis coordinates.
             y_axis (list): Y-axis coordinates.
 
         Returns:
             tuple: Calibration results (ret, mtx, dist).
         """
         self._process_reticle_points(x_axis, y_axis)
-        ret, self.mtx, self.dist, self.rvecs, self.tvecs = cv2.calibrateCamera(self.objpoints, self.imgpoints, \
-                                            SIZE, imtx, idist, flags=myflags1, criteria=CRIT)
-         
-        formatted_mtxt = "\n".join([" ".join([f"{val:.2f}" for val in row]) for row in self.mtx]) + "\n"
-        formatted_dist = " ".join([f"{val:.2f}" for val in self.dist[0]]) + "\n"
+        ret, self.mtx, self.dist, self.rvecs, self.tvecs = cv2.calibrateCamera(
+            self.objpoints,
+            self.imgpoints,
+            SIZE,
+            imtx,
+            idist,
+            flags=myflags1,
+            criteria=CRIT,
+        )
+
+        format_mtxt = (
+            "\n".join(
+                [" ".join([f"{val:.2f}" for val in row]) for row in self.mtx]
+            )
+            + "\n"
+        )
+        format_dist = " ".join([f"{val:.2f}" for val in self.dist[0]]) + "\n"
         logger.debug(f"A reproj error: {ret}")
-        logger.debug(f"Intrinsic: {formatted_mtxt}\n")
-        logger.debug(f"Distortion: {formatted_dist}\n")
+        logger.debug(f"Intrinsic: {format_mtxt}\n")
+        logger.debug(f"Distortion: {format_dist}\n")
         logger.debug(f"Focal length: {self.mtx[0][0]*1.85/1000}")
         distancesA = [np.linalg.norm(vec) for vec in self.tvecs]
-        logger.debug(f"Distance from camera to world center: {np.mean(distancesA)}")
+        logger.debug(
+            f"Distance from camera to world center: {np.mean(distancesA)}"
+        )
         return ret, self.mtx, self.dist
 
     def get_predefined_intrinsic(self, x_axis, y_axis):
         """
         Fetches predefined intrinsic camera parameters for specific models.
         Parameters:
         - x_axis (int or float): The x-axis value for reticle processing.
         - y_axis (int or float): The y-axis value for reticle processing.
 
         Returns:
-        - A tuple of (bool, numpy.ndarray or None, numpy.ndarray or None) representing success status,
-        intrinsic matrix, and distortion coefficients respectively.
+        - A tuple of (bool, numpy.ndarray or None, numpy.ndarray or None) 
+        representing success status, intrinsic matrix, 
+        and distortion coefficients respectively.
         """
         self._process_reticle_points(x_axis, y_axis)
         if self.name == "22517664":
             self.mtx = np.array([[1.520480e+04, 0.0e+00, 2e+03],
                 [0.0e+00, 1.520480e+04, 1.5e+03],
                 [0.0e+00, 0.0e+00, 1.0e+00]],
                 dtype=np.float32)
@@ -176,168 +200,213 @@
             return True, self.mtx, self.dist
         
         else:
             return False, None, None
 
     def get_origin_xyz(self):
         """
-        Get origin (0,0) and axis points (in x, y, z coords) in image coordinates.
+        Get origin (0,0) and axis points (x, y, z coords) in image coordinates.
 
         Returns:
             tuple: Origin, x-axis, y-axis, z-axis points.
         """
-        axis = np.float32([[3,0,0], [0,3,0], [0,0,3]]).reshape(-1,3)
+        axis = np.float32([[3, 0, 0], [0, 3, 0], [0, 0, 3]]).reshape(-1, 3)
         # Find the rotation and translation vectors.
-        # Output rotation vector (see Rodrigues ) that, together with tvec, 
-        # brings points from the model coordinate system to the camera coordinate system.
+        # Output rotation vector (see Rodrigues ) that, together with tvec,
+        # brings points from the model coordinate system 
+        # to the camera coordinate system.
         if self.objpoints is not None:
-            #_, rvecs, tvecs, _ = cv2.solvePnPRansac(self.objpoints, self.imgpoints, self.mtx, self.dist)
             solvePnP_method = cv2.SOLVEPNP_ITERATIVE
-            _, rvecs, tvecs = cv2.solvePnP(self.objpoints, self.imgpoints, self.mtx, self.dist, flags=solvePnP_method)
-            imgpts, _ = cv2.projectPoints(axis, rvecs, tvecs, self.mtx, self.dist)
-            origin = tuple(self.imgpoints[0][CENTER_INDEX_X].ravel().astype(int))
+            _, rvecs, tvecs = cv2.solvePnP(
+                self.objpoints,
+                self.imgpoints,
+                self.mtx,
+                self.dist,
+                flags=solvePnP_method,
+            )
+            imgpts, _ = cv2.projectPoints(
+                axis, rvecs, tvecs, self.mtx, self.dist
+            )
+            origin = tuple(
+                self.imgpoints[0][CENTER_INDEX_X].ravel().astype(int)
+            )
             x = tuple(imgpts[0].ravel().astype(int))
             y = tuple(imgpts[1].ravel().astype(int))
             z = tuple(imgpts[2].ravel().astype(int))
             return origin, x, y, z
         else:
             return None
-        
+
+
 class CalibrationStereo(CalibrationCamera):
     """
     Class for stereo camera calibration.
     """
-    def __init__(self, camA, imgpointsA, intrinsicA, camB, imgpointsB, intrinsicB):
+
+    def __init__(
+        self, camA, imgpointsA, intrinsicA, camB, imgpointsB, intrinsicB):
         """Initialize the CalibrationStereo object"""
         self.n_interest_pixels = 15
         self.camA = camA
         self.camB = camB
-        self.imgpointsA, self.objpoints = self._process_reticle_points(imgpointsA[0], imgpointsA[1])
-        self.imgpointsB, self.objpoints = self._process_reticle_points(imgpointsB[0], imgpointsB[1])
-        self.mtxA, self.distA = intrinsicA[0], intrinsicA[1] 
-        self.mtxB, self.distB = intrinsicB[0], intrinsicB[1] 
+        self.imgpointsA, self.objpoints = self._process_reticle_points(
+            imgpointsA[0], imgpointsA[1])
+        self.imgpointsB, self.objpoints = self._process_reticle_points(
+            imgpointsB[0], imgpointsB[1])
+        self.mtxA, self.distA = intrinsicA[0], intrinsicA[1]
+        self.mtxB, self.distB = intrinsicB[0], intrinsicB[1]
         self.criteria = (cv2.TERM_CRITERIA_EPS + cv2.TERM_CRITERIA_MAX_ITER, 100, 0.001)
         self.flags = cv2.CALIB_FIX_INTRINSIC
         self.retval, self.R_AB, self.T_AB, self.E_AB, self.F_AB = None, None, None, None, None 
         self.P_A, self.P_B = None, None
 
     def calibrate_stereo(self):
         """Calibrate stereo cameras.
 
         Returns:
             tuple: Stereo calibration results (retval, R_AB, T_AB, E_AB, F_AB).
         """
-        self.retval, _, _, _, _, self.R_AB, self.T_AB, self.E_AB, self.F_AB = \
-            cv2.stereoCalibrate(self.objpoints, 
-            self.imgpointsA, 
-            self.imgpointsB,
-            self.mtxA, self.distA, self.mtxB, self.distB, SIZE, 
-            criteria=self.criteria,
-            flags=self.flags)
-        
+        self.retval, _, _, _, _, self.R_AB, self.T_AB, self.E_AB, self.F_AB = (
+            cv2.stereoCalibrate(
+                self.objpoints,
+                self.imgpointsA,
+                self.imgpointsB,
+                self.mtxA,
+                self.distA,
+                self.mtxB,
+                self.distB,
+                SIZE,
+                criteria=self.criteria,
+                flags=self.flags,
+            )
+        )
+
         print("\n== Stereo Calibration ==")
         print("AB")
         print(self.retval)
         print(f"R: \n{self.R_AB}")
         print(f"T: \n{self.T_AB}")
         print(np.linalg.norm(self.T_AB))
 
-        formatted_F = "F_AB:\n" + "\n".join([" ".join([f"{val:.5f}" for val in row]) for row in self.F_AB]) + "\n"
-        formatted_E = "E_AB:\n" + "\n".join([" ".join([f"{val:.5f}" for val in row]) for row in self.E_AB]) + "\n"
+        formatted_F = (
+            "F_AB:\n"
+            + "\n".join(
+                [" ".join([f"{val:.5f}" for val in row]) for row in self.F_AB]
+            ) + "\n")
+        formatted_E = (
+            "E_AB:\n"
+            + "\n".join(
+                [" ".join([f"{val:.5f}" for val in row]) for row in self.E_AB]
+            ) + "\n")
         print(formatted_F)
         print(formatted_E)
 
-        self.P_A = self.mtxA @ np.hstack((np.eye(3), np.zeros((3, 1)))) 
+        self.P_A = self.mtxA @ np.hstack((np.eye(3), np.zeros((3, 1))))
         self.P_B = self.mtxB @ np.hstack((self.R_AB, self.T_AB.reshape(-1, 1)))
 
         return self.retval, self.R_AB, self.T_AB, self.E_AB, self.F_AB
-    
+
     def _matching_camera_order(self, camA, coordA, camB, coordB):
         """Match camera order based on initialization order.
 
         Args:
             camA (str): Camera A name.
             coordA (tuple): Coordinates from camera A.
             camB (str): Camera B name.
             coordB (tuple): Coordinates from camera B.
 
         Returns:
             tuple: Matched camera order and coordinates.
         """
         if self.camA == camA:
             return camA, coordA, camB, coordB
-        
+
         if self.camA == camB:
             return camB, coordB, camA, coordA
-        
+
     def triangulation(self, P_1, P_2, imgpoints_1, imgpoints_2):
         """Triangulate 3D points from stereo image points.
 
         Args:
             P_1 (numpy.ndarray): Projection matrix of camera 1.
             P_2 (numpy.ndarray): Projection matrix of camera 2.
             imgpoints_1 (numpy.ndarray): Image points from camera 1.
             imgpoints_2 (numpy.ndarray): Image points from camera 2.
 
         Returns:
             numpy.ndarray: Triangulated 3D points.
         """
-        points_4d_hom= cv2.triangulatePoints(P_1, P_2, imgpoints_1.T, imgpoints_2.T)
+        points_4d_hom = cv2.triangulatePoints(
+            P_1, P_2, imgpoints_1.T, imgpoints_2.T
+        )
         points_3d_hom = points_4d_hom / points_4d_hom[3]
         points_3d_hom = points_3d_hom.T
-        return points_3d_hom[:,:3]
-    
+        return points_3d_hom[:, :3]
+
     def change_coords_system_from_camA_to_global(self, points_3d_AB):
         """
-        Change coordinate system from camera A to global using solvePnPRansac().
+        Change coordinate system from camera A to global using solvePnPRansac.
 
         Args:
-            points_3d_AB (numpy.ndarray): 3D points in camera A coordinate system.
+            points_3d_AB (numpy.ndarray):
+            3D points in camera A coordinate system.
 
         Returns:
             numpy.ndarray: 3D points in global coordinate system.
         """
-        _, rvecs, tvecs, _ = cv2.solvePnPRansac(self.objpoints, self.imgpointsA, self.mtxA, self.distA)
+        _, rvecs, tvecs, _ = cv2.solvePnPRansac(
+            self.objpoints, self.imgpointsA, self.mtxA, self.distA
+        )
         # Convert rotation vectors to rotation matrices
         rmat, _ = cv2.Rodrigues(rvecs)
         # Invert the rotation and translation
         rmat_inv = rmat.T  # Transpose of rotation matrix is its inverse
         tvecs_inv = -rmat_inv @ tvecs
         # Transform the points
         points_3d_G = np.dot(rmat_inv, points_3d_AB.T).T + tvecs_inv.T
         return points_3d_G
-    
+
     def change_coords_system_from_camA_to_global_iterative(self, points_3d_AB):
-        """Change coordinate system from camera A to global using iterative method.
+        """Change coordinate system from camera A to global 
+        using iterative method.
 
         Args:
-            points_3d_AB (numpy.ndarray): 3D points in camera A coordinate system.
+            points_3d_AB (numpy.ndarray):
+            3D points in camera A coordinate system.
 
         Returns:
             numpy.ndarray: 3D points in global coordinate system.
         """
         solvePnP_method = cv2.SOLVEPNP_ITERATIVE
-        _, rvecs, tvecs = cv2.solvePnP(self.objpoints, self.imgpointsA, self.mtxA, self.distA, flags=solvePnP_method)
+        _, rvecs, tvecs = cv2.solvePnP(
+            self.objpoints,
+            self.imgpointsA,
+            self.mtxA,
+            self.distA,
+            flags=solvePnP_method,
+        )
         logger.debug("solvePnP")
         logger.debug(rvecs)
         logger.debug(tvecs)
         # Convert rotation vectors to rotation matrices
         rmat, _ = cv2.Rodrigues(rvecs)
         # Invert the rotation and translation
         self.rmat_inv = rmat.T  # Transpose of rotation matrix is its inverse
         self.tvecs_inv = -self.rmat_inv @ tvecs
         # Transform the points
         points_3d_G = np.dot(self.rmat_inv, points_3d_AB.T).T + self.tvecs_inv.T
         return points_3d_G
 
     def change_coords_system_from_camA_to_global_savedRT(self, points_3d_AB):
-        """Change coordinate system from camera A to global using saved rotation and translation.
+        """Change coordinate system from camera A to global
+        using saved rotation and translation.
 
         Args:
-            points_3d_AB (numpy.ndarray): 3D points in camera A coordinate system.
+            points_3d_AB (numpy.ndarray):
+            3D points in camera A coordinate system.
 
         Returns:
             numpy.ndarray: 3D points in global coordinate system.
         """
         points_3d_G = np.dot(self.rmat_inv, points_3d_AB.T).T + self.tvecs_inv.T
         return points_3d_G
 
@@ -349,102 +418,139 @@
             coordA (tuple): Coordinates from camera A.
             camB (str): Camera B name.
             coordB (tuple): Coordinates from camera B.
 
         Returns:
             numpy.ndarray: 3D points in global coordinate system.
         """
-        camA, coordA, camB, coordB = self._matching_camera_order(camA, coordA, camB, coordB)
+        camA, coordA, camB, coordB = self._matching_camera_order(
+            camA, coordA, camB, coordB
+        )
         coordA = np.array(coordA).astype(np.float32)
         coordB = np.array(coordB).astype(np.float32)
         points_3d_AB = self.triangulation(self.P_B, self.P_A, coordB, coordA)
-        #points_3d_G = self.change_coords_system_from_camA_to_global(points_3d_AB)
-        #points_3d_G = self.change_coords_system_from_camA_to_global_iterative(points_3d_AB)
-        points_3d_G = self.change_coords_system_from_camA_to_global_savedRT(points_3d_AB)
-
-        logger.debug(f"points_3d_G: {points_3d_G}, coordA: {coordA}, coordB: {coordB}")
+        points_3d_G = self.change_coords_system_from_camA_to_global_savedRT(
+            points_3d_AB
+        )
+
+        logger.debug(
+            f"points_3d_G: {points_3d_G}, coordA: {coordA}, coordB: {coordB}"
+        )
         return points_3d_G
-    
+
     def test_x_y_z_performance(self, points_3d_G):
         # Calculate the differences for each dimension
         differences_x = points_3d_G[:, 0] - self.objpoints[0, :, 0]
         differences_y = points_3d_G[:, 1] - self.objpoints[0, :, 1]
         differences_z = points_3d_G[:, 2] - self.objpoints[0, :, 2]
 
         # Calculate the mean squared differences for each dimension
         mean_squared_diff_x = np.mean(np.square(differences_x))
         mean_squared_diff_y = np.mean(np.square(differences_y))
         mean_squared_diff_z = np.mean(np.square(differences_z))
 
-        # If required, calculate the L2 norm (Euclidean distance) for each dimension
-        average_l2_x = np.sqrt(mean_squared_diff_x)
-        average_l2_y = np.sqrt(mean_squared_diff_y)
-        average_l2_z = np.sqrt(mean_squared_diff_z)
-
-        print(f"x: {average_l2_x*1000}µm³, y: {average_l2_y*1000}µm³, z:{average_l2_z*1000}µm³")
-
+        # Calculate the L2 norm (Euclidean distance) for each dimension
+        l2_x = np.sqrt(mean_squared_diff_x)
+        l2_y = np.sqrt(mean_squared_diff_y)
+        l2_z = np.sqrt(mean_squared_diff_z)
+
+        print(
+            f"x: {l2_x*1000}µm³, y: {l2_y*1000}µm³, z:{l2_z*1000}µm³"
+        )
 
     def test_performance(self, camA, coordA, camB, coordB):
         """Test stereo calibration.
 
         Args:
             camA (str): Camera A name.
             coordA (tuple): Coordinates from camera A.
             camB (str): Camera B name.
             coordB (tuple): Coordinates from camera B.
 
         Returns:
             numpy.ndarray: Predicted 3D points in global coordinate system.
         """
-        camA, coordA, camB, coordB = self._matching_camera_order(camA, coordA, camB, coordB)
+        camA, coordA, camB, coordB = self._matching_camera_order(
+            camA, coordA, camB, coordB
+        )
         logger.debug(f"coordA: {coordA}")
         logger.debug(f"coordB: {coordB}")
-        points_3d_AB = self.triangulation(self.P_B, self.P_A, self.imgpointsB, self.imgpointsA)
-        np.set_printoptions(suppress=True, precision=8) 
-
-        points_3d_G = self.change_coords_system_from_camA_to_global_iterative(points_3d_AB)
+        points_3d_AB = self.triangulation(
+            self.P_B, self.P_A, self.imgpointsB, self.imgpointsA
+        )
+        np.set_printoptions(suppress=True, precision=8)
+
+        points_3d_G = self.change_coords_system_from_camA_to_global_iterative(
+            points_3d_AB
+        )
         print("\n=solvePnP SOLVEPNP_ITERATIVE=")
         differences = points_3d_G - self.objpoints[0]
         squared_distances = np.sum(np.square(differences), axis=1)
         euclidean_distances = np.sqrt(squared_distances)
         average_L2_distance = np.mean(euclidean_distances)
-        print(f"(Reprojection error) Object points L2 diff: {average_L2_distance*1000} µm³")
+        print(
+            f"(Reprojection error) Object points L2 diff: \
+            {average_L2_distance*1000} µm³"
+        )
         self.test_x_y_z_performance(points_3d_G)
         print(f"Object points predict:\n{np.around(points_3d_G, decimals=5)}")
 
         self.test_pixel_error()
         return average_L2_distance
-    
+
     def test_pixel_error(self):
         """Test pixel reprojection error."""
         mean_error = 0
         for i in range(len(self.objpoints)):
-            imgpointsA_converted = np.array(self.imgpointsA[i], dtype=np.float32).reshape(-1,2)
+            imgpointsA_converted = np.array(
+                self.imgpointsA[i], dtype=np.float32
+            ).reshape(-1, 2)
             solvePnP_method = cv2.SOLVEPNP_ITERATIVE
-            retval, rvecs, tvecs = cv2.solvePnP(self.objpoints[i], imgpointsA_converted, self.mtxA, self.distA, flags=solvePnP_method)
-            imgpoints2, _ = cv2.projectPoints(self.objpoints[i], rvecs, tvecs, self.mtxA, self.distA)
-            
-            imgpoints2_reshaped = imgpoints2.reshape(-1,2) 
+            retval, rvecs, tvecs = cv2.solvePnP(
+                self.objpoints[i],
+                imgpointsA_converted,
+                self.mtxA,
+                self.distA,
+                flags=solvePnP_method,
+            )
+            imgpoints2, _ = cv2.projectPoints(
+                self.objpoints[i], rvecs, tvecs, self.mtxA, self.distA
+            )
+
+            imgpoints2_reshaped = imgpoints2.reshape(-1, 2)
             differences = imgpointsA_converted - imgpoints2_reshaped
             squared_distances = np.sum(np.square(differences), axis=1)
             distances = np.sqrt(squared_distances)
             average_L2_distance = np.mean(distances)
             mean_error += average_L2_distance
             logger.debug("A pixel diff")
             logger.debug(imgpointsA_converted-imgpoints2_reshaped)
-        print(f"(Reprojection error) Pixel L2 diff A: {mean_error / len(self.objpoints)} pixels")
+        total_err = mean_error / len(self.objpoints)
+        print(f"(Reprojection error) Pixel L2 diff A: {total_err} pixels")
 
         mean_error = 0
         for i in range(len(self.objpoints)):
-            imgpointsB_converted = np.array(self.imgpointsB[i], dtype=np.float32).reshape(-1,2)
+            imgpointsB_converted = np.array(
+                self.imgpointsB[i], dtype=np.float32
+            ).reshape(-1, 2)
             solvePnP_method = cv2.SOLVEPNP_ITERATIVE
-            retval, rvecs, tvecs = cv2.solvePnP(self.objpoints[i], imgpointsB_converted, self.mtxB, self.distB, flags=solvePnP_method)
-            imgpoints2, _ = cv2.projectPoints(self.objpoints[i], rvecs, tvecs, self.mtxB, self.distB)
-            
-            imgpoints2_reshaped = imgpoints2.reshape(-1,2) 
+            retval, rvecs, tvecs = cv2.solvePnP(
+                self.objpoints[i],
+                imgpointsB_converted,
+                self.mtxB,
+                self.distB,
+                flags=solvePnP_method,
+            )
+            imgpoints2, _ = cv2.projectPoints(
+                self.objpoints[i], rvecs, tvecs, self.mtxB, self.distB
+            )
+
+            imgpoints2_reshaped = imgpoints2.reshape(-1, 2)
             differences = imgpointsB_converted - imgpoints2_reshaped
             distances = np.sqrt(np.sum(np.square(differences), axis=1))
             average_L2_distance = np.mean(distances)
             mean_error += average_L2_distance
             logger.debug("B pixel diff")
-            logger.debug(imgpointsB_converted-imgpoints2_reshaped)
-        print(f"(Reprojection error) Pixel L2 diff B: {mean_error / len(self.objpoints)} pixels")
+            logger.debug(imgpointsB_converted - imgpoints2_reshaped)
+
+        total_err = mean_error / len(self.objpoints)
+        print(f"(Reprojection error) Pixel L2 diff B: {total_err} pixels")
```

### Comparing `parallax_app-0.37.0/parallax/camera.py` & `parallax_app-0.37.1/parallax/camera.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 """
 PySpinCamera: A class to interface with cameras using the PySpin library.
 """
-import time
+
 import datetime
-import threading
-import numpy as np
 import logging
 import os
+import threading
+import time
+
 import cv2
+import numpy as np
 
 # Initialize the logger
 logger = logging.getLogger(__name__)
 supported_camera_models = ["BFS-U3-120S4C", "BFS-U3-04S2M"]
 
 # Check for the availability of the PySpin library
 try:
     import PySpin
 except ImportError:
     PySpin = None
     logger.warn("Could not import PySpin.")
 
+
 def list_cameras(dummy=False, version="V1"):
     """
     List available cameras.
-    
+
     Parameters:
     - dummy (bool): If True, lists only mock cameras. Default is False.
-    
+
     Returns:
     - list: List of available PySpin cameras.
     """
     # Init version, V1: original, V2: WIP with new GUI
     global VERSION
     VERSION = version
 
     global pyspin_cameras, pyspin_instance
     cameras = []
     if not dummy:
         if PySpin is not None:
             cameras.extend(PySpinCamera.list_cameras())
     return cameras
 
+
 def close_cameras():
     """Close all available cameras."""
     if PySpin is not None:
         PySpinCamera.close_cameras()
 
+
 class PySpinCamera:
     """
     Represents a camera managed by the PySpin library.
     """
+
     pyspin_cameras = None
     pyspin_instance = None
     cameras = []
- 
+
     @classmethod
     def list_cameras(cls):
         """
         List available PySpin cameras.
-        
+
         Returns:
         - list: List of available PySpin cameras.
         """
         if cls.pyspin_instance is None:
             cls.pyspin_instance = PySpin.System.GetInstance()
         cls.pyspin_cameras = cls.pyspin_instance.GetCameras()
         ncameras = cls.pyspin_cameras.GetSize()
@@ -71,16 +77,15 @@
         for i in range(ncameras):
             camera_pyspin = cls.pyspin_cameras.GetByIndex(i)
             camera = PySpinCamera(camera_pyspin)
             if camera is not None:
                 cls.cameras.append(camera)
             else:
                 camera.stop(clean=True)
-        
-        # cls.cameras = [PySpinCamera(cls.pyspin_cameras.GetByIndex(i)) for i in range(ncameras)]
+
         return cls.cameras
 
     # Class method to close all PySpin cameras
     @classmethod
     def close_cameras(cls):
         """
         Release resources and close all PySpin cameras.
@@ -88,153 +93,209 @@
         logger.info("cleaning up SpinSDK")
         for camera in cls.cameras:
             camera.stop(clean=True)
         if cls.pyspin_cameras is not None:
             cls.pyspin_cameras.Clear()
         if cls.pyspin_instance is not None:
             cls.pyspin_instance.ReleaseInstance()
-        
+
     # Constructor for PySpinCamera
     def __init__(self, camera_pyspin):
         """
         Initialize a PySpinCamera instance.
-        
+
         Parameters:
         - camera_pyspin: The underlying PySpin camera object.
         """
         self.running = False
         self.camera = camera_pyspin
         self.tldnm = self.camera.GetTLDeviceNodeMap()
         self.camera.Init()
         self.node_map = self.camera.GetNodeMap()
-        
+
         self.last_image = None
         self.last_image_filled = threading.Event()
         self.last_image_cleared = threading.Event()
 
         self.video_output = None
         self.video_recording_on = threading.Event()
         self.video_recording_idle = threading.Event()
         self.height = None
         self.width = None
         self.channels = None
         self.frame_rate = None
-        
+
         self.device_model = self.camera.DeviceModelName()
         self.device_color_type = None
-        camera_color_type = self.device_model.split('-')[2][-1]
-        if camera_color_type == 'M':
+        camera_color_type = self.device_model.split("-")[2][-1]
+        if camera_color_type == "M":
             self.device_color_type = "Mono"
-        elif camera_color_type == 'C':
+        elif camera_color_type == "C":
             self.device_color_type = "Color"
-        elif camera_color_type == 'P':
+        elif camera_color_type == "P":
             self.device_color_type = "Polarized"
             print("Polarized Camera model not supported.")
             return None
         else:
             print("Not supported camera type.")
             return None
-        print(self.device_model, self.device_color_type, self.name(sn_only=True))
+        print(
+            self.device_model, self.device_color_type, self.name(sn_only=True)
+        )
 
         # set BufferHandlingMode to NewestOnly (necessary to update the image)
         s_nodemap = self.camera.GetTLStreamNodeMap()
-        node_bufferhandling_mode = PySpin.CEnumerationPtr(s_nodemap.GetNode('StreamBufferHandlingMode'))
-        node_newestonly = node_bufferhandling_mode.GetEntryByName('NewestOnly')
+        node_bufferhandling_mode = PySpin.CEnumerationPtr(
+            s_nodemap.GetNode("StreamBufferHandlingMode")
+        )
+        node_newestonly = node_bufferhandling_mode.GetEntryByName("NewestOnly")
         node_newestonly_mode = node_newestonly.GetValue()
         node_bufferhandling_mode.SetIntValue(node_newestonly_mode)
-        
+
         # Set White Balance
         if self.device_color_type == "Color":
-            self.node_wbauto_mode = PySpin.CEnumerationPtr(self.node_map.GetNode("BalanceWhiteAuto"))
-            self.node_wbauto_mode_off = self.node_wbauto_mode.GetEntryByName("Off")
-            self.node_wbauto_mode_on = self.node_wbauto_mode.GetEntryByName("Continuous")
-            self.node_wbauto_mode.SetIntValue(self.node_wbauto_mode_on.GetValue())      # Default: Auto mode on 
-            self.node_balanceratio_mode = PySpin.CEnumerationPtr(self.node_map.GetNode("BalanceRatioSelector"))
-            self.node_wb = PySpin.CFloatPtr(self.node_map.GetNode("BalanceRatio"))
-            self.node_balanceratio_mode_red = self.node_balanceratio_mode.GetEntryByName("Red")     # Red Channel    
-            self.node_balanceratio_mode_blue = self.node_balanceratio_mode.GetEntryByName("Blue")   # Blue Channel 
+            self.node_wbauto_mode = PySpin.CEnumerationPtr(
+                self.node_map.GetNode("BalanceWhiteAuto")
+            )
+            self.node_wbauto_mode_off = self.node_wbauto_mode.GetEntryByName(
+                "Off"
+            )
+            self.node_wbauto_mode_on = self.node_wbauto_mode.GetEntryByName(
+                "Continuous"
+            )
+            self.node_wbauto_mode.SetIntValue(
+                self.node_wbauto_mode_on.GetValue()
+            )  # Default: Auto mode on
+            self.node_balanceratio_mode = PySpin.CEnumerationPtr(
+                self.node_map.GetNode("BalanceRatioSelector")
+            )
+            self.node_wb = PySpin.CFloatPtr(
+                self.node_map.GetNode("BalanceRatio")
+            )
+            self.node_balanceratio_mode_red = (
+                self.node_balanceratio_mode.GetEntryByName("Red")
+            )  # Red Channel
+            self.node_balanceratio_mode_blue = (
+                self.node_balanceratio_mode.GetEntryByName("Blue")
+            )  # Blue Channel
 
         # set exposure time
-        self.node_expauto_mode = PySpin.CEnumerationPtr(self.node_map.GetNode("ExposureAuto"))
-        self.node_expauto_mode_off = self.node_expauto_mode.GetEntryByName("Off")
-        self.node_expauto_mode_on = self.node_expauto_mode.GetEntryByName("Continuous")
-        self.node_expauto_mode.SetIntValue(self.node_expauto_mode_on.GetValue())        # Default: Auto mode on 
-        self.node_exptime = PySpin.CFloatPtr(self.node_map.GetNode("ExposureTime"))
+        self.node_expauto_mode = PySpin.CEnumerationPtr(
+            self.node_map.GetNode("ExposureAuto")
+        )
+        self.node_expauto_mode_off = self.node_expauto_mode.GetEntryByName(
+            "Off"
+        )
+        self.node_expauto_mode_on = self.node_expauto_mode.GetEntryByName(
+            "Continuous"
+        )
+        self.node_expauto_mode.SetIntValue(
+            self.node_expauto_mode_on.GetValue()
+        )  # Default: Auto mode on
+        self.node_exptime = PySpin.CFloatPtr(
+            self.node_map.GetNode("ExposureTime")
+        )
 
         # set gain
-        self.node_gainauto_mode = PySpin.CEnumerationPtr(self.node_map.GetNode("GainAuto"))
-        self.node_gainauto_mode_off = self.node_gainauto_mode.GetEntryByName("Off")
-        self.node_gainauto_mode_on = self.node_gainauto_mode.GetEntryByName("Continuous")
+        self.node_gainauto_mode = PySpin.CEnumerationPtr(
+            self.node_map.GetNode("GainAuto")
+        )
+        self.node_gainauto_mode_off = self.node_gainauto_mode.GetEntryByName(
+            "Off"
+        )
+        self.node_gainauto_mode_on = self.node_gainauto_mode.GetEntryByName(
+            "Continuous"
+        )
         self.node_gain = PySpin.CFloatPtr(self.node_map.GetNode("Gain"))
-        self.node_gainauto_mode.SetIntValue(self.node_gainauto_mode_on.GetValue())      # Default: Auto mode on    
-
-        # set gamma  
-        self.node_gammaenable_mode = PySpin.CBooleanPtr(self.node_map.GetNode("GammaEnable"))
-        self.node_gammaenable_mode.SetValue(True)                # Default: Gammal Enable on 
+        self.node_gainauto_mode.SetIntValue(
+            self.node_gainauto_mode_on.GetValue()
+        )  # Default: Auto mode on
+
+        # set gamma
+        self.node_gammaenable_mode = PySpin.CBooleanPtr(
+            self.node_map.GetNode("GammaEnable")
+        )
+        self.node_gammaenable_mode.SetValue(True)  # Default: Gammal Enable on
         self.node_gamma = PySpin.CFloatPtr(self.node_map.GetNode("Gamma"))
-        self.node_gamma.SetValue(0.8)  
+        self.node_gamma.SetValue(0.8)
 
         # set pixel format
-        node_pixelformat = PySpin.CEnumerationPtr(self.node_map.GetNode("PixelFormat"))
+        node_pixelformat = PySpin.CEnumerationPtr(
+            self.node_map.GetNode("PixelFormat")
+        )
         self.pixelformat = None
         if self.device_color_type == "Mono":
             self.pixelformat = "Mono"
             entry_pixelformat_mono8 = node_pixelformat.GetEntryByName("Mono8")
             node_pixelformat.SetIntValue(entry_pixelformat_mono8.GetValue())
         elif self.device_color_type == "Color":
             self.pixelformat = "BayerRG8"
-            entry_pixelformat_bayerRG8 = node_pixelformat.GetEntryByName("BayerRG8")
+            entry_pixelformat_bayerRG8 = node_pixelformat.GetEntryByName(
+                "BayerRG8"
+            )
             node_pixelformat.SetIntValue(entry_pixelformat_bayerRG8.GetValue())
 
-        # acquisition on initialization             
+        # acquisition on initialization
         if VERSION == "V1":
             # begin acquisition
-            # V1: Start continuous acquisition on initialization. 
+            # V1: Start continuous acquisition on initialization.
             self.begin_continuous_acquisition()
         elif VERSION == "V2":
-            # V2: Start continous acquisition when 'Start' button is toggled and end acquisition when untoggled.
-            # On initialization, start onetime acquisition to get one frame. 
+            # V2: Start continuous acquisition when 'Start' button is toggled and end acquisition when untoggled.
+            # On initialization, start onetime acquisition to get one frame.
             pass
-        
+
     def set_wb(self, channel, wb=1.2):
         """
         Sets the white balance of the camera.
 
         Args:
         - wb (float): The desired white balance value. min:1.8, max:2.5
         """
         if self.device_color_type == "Color":
-            self.node_wbauto_mode.SetIntValue(self.node_wbauto_mode_off.GetValue())
+            self.node_wbauto_mode.SetIntValue(
+                self.node_wbauto_mode_off.GetValue()
+            )
             if channel == "Red":
-                self.node_balanceratio_mode.SetIntValue(self.node_balanceratio_mode_red.GetValue())
+                self.node_balanceratio_mode.SetIntValue(
+                    self.node_balanceratio_mode_red.GetValue()
+                )
                 self.node_wb.SetValue(wb)
             elif channel == "Blue":
-                self.node_balanceratio_mode.SetIntValue(self.node_balanceratio_mode_blue.GetValue())
+                self.node_balanceratio_mode.SetIntValue(
+                    self.node_balanceratio_mode_blue.GetValue()
+                )
                 self.node_wb.SetValue(wb)
         else:
             pass
-    
+
     def get_wb(self, channel):
         """
         Get the gamma of the camera for the auto mode.
         """
         if self.device_color_type == "Color":
-            self.node_wbauto_mode.SetIntValue(self.node_wbauto_mode_on.GetValue()) # Set continous for mono camera
+            self.node_wbauto_mode.SetIntValue(
+                self.node_wbauto_mode_on.GetValue()
+            )  # Set continuous for mono camera
             time.sleep(0.5)
             if channel == "Red":
-                self.node_balanceratio_mode.SetIntValue(self.node_balanceratio_mode_red.GetValue())
+                self.node_balanceratio_mode.SetIntValue(
+                    self.node_balanceratio_mode_red.GetValue()
+                )
                 time.sleep(0.5)
-                return self.node_wb.GetValue()                
+                return self.node_wb.GetValue()
             elif channel == "Blue":
-                self.node_balanceratio_mode.SetIntValue(self.node_balanceratio_mode_blue.GetValue())
+                self.node_balanceratio_mode.SetIntValue(
+                    self.node_balanceratio_mode_blue.GetValue()
+                )
                 time.sleep(0.5)
                 return self.node_wb.GetValue()
         else:
             return -1
-        
+
     def set_gamma(self, gamma=1.0):
         """
         Sets the gamma correction of the camera.
 
         Args:
         - gamma (float): The desired gamma value. min:0.25 max:1.25
         """
@@ -250,207 +311,252 @@
     def set_gain(self, gain=20.0):
         """
         Sets the gain of the camera.
 
         Args:
         - gain (float): The desired gain value. min:0, max:27.0
         """
-        self.node_gainauto_mode.SetIntValue(self.node_gainauto_mode_off.GetValue())
+        self.node_gainauto_mode.SetIntValue(
+            self.node_gainauto_mode_off.GetValue()
+        )
         self.node_gain.SetValue(gain)
 
     def get_gain(self):
         """
         Get the gain of the camera for the auto mode.
         """
         initial_val = self.node_gain.GetValue()
-        self.node_gainauto_mode.SetIntValue(self.node_gainauto_mode_on.GetValue()) # Set continous for mono camera
+        self.node_gainauto_mode.SetIntValue(
+            self.node_gainauto_mode_on.GetValue()
+        )  # Set continuous for mono camera
 
         time.sleep(0.5)  # Wait for a short period
         updated_val = self.node_gain.GetValue()
         if updated_val != initial_val:
             return updated_val  # Return the updated value if there's a change
 
         return initial_val  # Return the initial value if no change is detected
 
     def set_exposure(self, expTime=16000):
         """
         Sets the exposure time of the camera.
 
         Args:
-        - expTime (int): The desired exposure time in microseconds. 
+        - expTime (int): The desired exposure time in microseconds.
         """
-        self.node_expauto_mode.SetIntValue(self.node_expauto_mode_off.GetValue())   # Return back to manual mode
+        self.node_expauto_mode.SetIntValue(
+            self.node_expauto_mode_off.GetValue()
+        )  # Return back to manual mode
         self.node_exptime.SetValue(expTime)
-    
+
     def get_exposure(self):
         """
         Get the exposure time of the camera for the auto mode.
         """
         initial_val = self.node_exptime.GetValue()
-        self.node_expauto_mode.SetIntValue(self.node_expauto_mode_on.GetValue())    # Enable the Auto mode
-        
+        self.node_expauto_mode.SetIntValue(
+            self.node_expauto_mode_on.GetValue()
+        )  # Enable the Auto mode
+
         time.sleep(0.5)  # Wait for a short period
         updated_val = self.node_exptime.GetValue()
         if updated_val != initial_val:
             return updated_val  # Return the updated value if there's a change
-        
+
         return initial_val  # Return the initial value if no change is detected
 
     def name(self, sn_only=False):
         """
         Retrieves the name and serial number of the camera.
 
         Args:
         - sn_only (bool): Whether to return only the serial number.
 
         Returns:
         - str: The device model and serial number or just the serial number.
-        """        
+        """
         sn = self.camera.DeviceSerialNumber()
         device_model = self.camera.DeviceModelName()
         if sn_only:
             return sn
         else:
-            return '%s (Serial # %s)' % (device_model, sn)
+            return "%s (Serial # %s)" % (device_model, sn)
 
     def begin_singleframe_acquisition(self):
         """
-        Begings a single Frame image acquisition. 
-        """  
+        Begings a single Frame image acquisition.
+        """
         # set acquisition mode to singleFrame
-        node_acquisition_mode = PySpin.CEnumerationPtr(self.node_map.GetNode('AcquisitionMode'))
-        node_acquisition_mode_singleframe = node_acquisition_mode.GetEntryByName('SingleFrame')
-        acquisition_mode_singleframe = node_acquisition_mode_singleframe.GetValue()
+        node_acquisition_mode = PySpin.CEnumerationPtr(
+            self.node_map.GetNode("AcquisitionMode")
+        )
+        node_acquisition_mode_singleframe = (
+            node_acquisition_mode.GetEntryByName("SingleFrame")
+        )
+        acquisition_mode_singleframe = (
+            node_acquisition_mode_singleframe.GetValue()
+        )
         node_acquisition_mode.SetIntValue(acquisition_mode_singleframe)
 
         # Begin Acquisition: Image acquisition must be ended when no more images are needed.
-        self.camera.BeginAcquisition() 
+        self.camera.BeginAcquisition()
         print(f"Begin Single Frame Acquisition {self.name(sn_only=True)} ")
-        self.capture_thread = threading.Thread(target=self.capture, daemon=False)
+        self.capture_thread = threading.Thread(
+            target=self.capture, daemon=False
+        )
         self.capture_thread.start()
-        
+
     def end_singleframe_acquisition(self):
-        """ End Acquisition """
+        """End Acquisition"""
         self.last_image_cleared.wait()
         self.capture_thread.join()
         self.camera.EndAcquisition()
         self.last_image = None
         self.last_image_cleared.clear()
         self.last_image_filled.clear()
 
     def begin_continuous_acquisition(self):
         """
         Begins the image acquisition process in continuous mode and starts the capture loop in a separate thread.
-        """    
+        """
         if self.running:
             print("Error: camera is already running")
             return -1
 
         # set acquisition mode continuous (continuous stream of images)
-        node_acquisition_mode = PySpin.CEnumerationPtr(self.node_map.GetNode('AcquisitionMode'))
-        node_acquisition_mode_continuous = node_acquisition_mode.GetEntryByName('Continuous')
-        acquisition_mode_continuous = node_acquisition_mode_continuous.GetValue()
+        node_acquisition_mode = PySpin.CEnumerationPtr(
+            self.node_map.GetNode("AcquisitionMode")
+        )
+        node_acquisition_mode_continuous = node_acquisition_mode.GetEntryByName(
+            "Continuous"
+        )
+        acquisition_mode_continuous = (
+            node_acquisition_mode_continuous.GetValue()
+        )
         node_acquisition_mode.SetIntValue(acquisition_mode_continuous)
 
         # Begin Acquisition: Image acquisition must be ended when no more images are needed.
-        self.camera.BeginAcquisition() 
+        self.camera.BeginAcquisition()
         logger.debug(f"BeginAcquisition {self.name(sn_only=True)} ")
         self.running = True
-        self.capture_thread = threading.Thread(target=self.capture_loop, daemon=True)
+        self.capture_thread = threading.Thread(
+            target=self.capture_loop, daemon=True
+        )
         self.capture_thread.start()
 
     def capture_loop(self):
         """
         Continuous loop to capture images while the camera is running.
         """
         while self.running:
             self.capture()
             # print(".", end="",flush=True)
 
     def capture(self):
         """
-        Captures an image and checks for its completeness. 
+        Captures an image and checks for its completeness.
         If video recording is enabled, writes the image to the video file.
 
         *** NOTES ***
         Capturing an image houses images on the camera buffer.
         Trying to capture an image that does not exist will hang the camera.
         Using-statements help ensure that images are released.
-        If too many images remain unreleased, the buffer will fill, 
-        causing the camera to hang. 
+        If too many images remain unreleased, the buffer will fill,
+        causing the camera to hang.
         Images can also be released manually by calling Release().
         """
         # Timestamp for the current capture
         ts = time.time()
         self.last_capture_time = ts
 
         # Retrieve the next image from the camera
         image = self.camera.GetNextImage(1000)
-    
+
         while image.IsIncomplete():
             time.sleep(0.001)
-        
+
         # Release the previous image from the buffer if it exists
         if self.last_image is not None:
             try:
                 self.last_image.Release()
             except PySpin.SpinnakerException:
                 print("Spinnaker Exception: Couldn't release last image")
 
         # Update the last captured image reference
         self.last_image = image
         self.last_image_filled.set()
 
-        # Record the image if video recording is active     
-        if self.video_recording_on.is_set(): 
+        # Record the image if video recording is active
+        if self.video_recording_on.is_set():
             self.video_recording_idle.clear()
-            
+
             frame = self.get_last_image_data()
             frame = cv2.cvtColor(frame, cv2.COLOR_RGB2BGR)
 
             self.video_output.write(frame)
             self.video_recording_idle.set()
-        
+
     def get_last_capture_time(self, millisecond=False):
         """
         Returns the timestamp of the last captured image in a formatted string.
 
         Returns:
         - str: Timestamp in the format 'YYYYMMDD-HHMMSS'.
         """
         ts = self.last_capture_time
         dt = datetime.datetime.fromtimestamp(ts)
         if millisecond:
-            return '%04d%02d%02d-%02d%02d%02d.%03d' % (dt.year, dt.month, dt.day,
-                        dt.hour, dt.minute, dt.second, dt.microsecond // 1000)
+            return "%04d%02d%02d-%02d%02d%02d.%03d" % (
+                dt.year,
+                dt.month,
+                dt.day,
+                dt.hour,
+                dt.minute,
+                dt.second,
+                dt.microsecond // 1000,
+            )
         else:
-            return '%04d%02d%02d-%02d%02d%02d' % (dt.year, dt.month, dt.day,
-                                              dt.hour, dt.minute, dt.second)
-
-    def save_last_image(self, filepath, isTimestamp=False, custom_name="Microscope_"):
+            return "%04d%02d%02d-%02d%02d%02d" % (
+                dt.year,
+                dt.month,
+                dt.day,
+                dt.hour,
+                dt.minute,
+                dt.second,
+            )
+
+    def save_last_image(
+        self, filepath, isTimestamp=False, custom_name="Microscope_"
+    ):
         """
         Saves the last captured image to the specified file path.
 
         Args:
         - filepath (str): Directory to save the image.
         - isTimestamp (bool): Whether to append a timestamp to the filename.
-        - custom_name (str): Custom prefix for the filename. S/N is set as custom name.
+        - custom_name (str): Custom prefix for the filename. 
+        S/N is set as custom name.
         """
-        image_name = "{}_{}.png".format(custom_name, self.get_last_capture_time()) \
-            if isTimestamp else "{}.png".format(custom_name)
+        image_name = (
+            "{}_{}.png".format(custom_name, self.get_last_capture_time())
+            if isTimestamp
+            else "{}.png".format(custom_name)
+        )
         full_path = os.path.join(filepath, image_name)
         logger.debug(f"Saving image to {full_path}")
         print(f"Saving image to {full_path}")
 
         # Save the image
         try:
             image_converted = self.get_last_image_data()
             if image_converted is not None:
                 # Convert the image from RGB to BGR
-                image_converted = cv2.cvtColor(image_converted, cv2.COLOR_RGB2BGR)
+                image_converted = cv2.cvtColor(
+                    image_converted, cv2.COLOR_RGB2BGR
+                )
                 cv2.imwrite(full_path, image_converted)
             else:
                 logger.error("Image not found or couldn't be retrieved.")
         except Exception as e:
             logger.error(f"An error occurred while saving the image: {e}")
 
     def get_last_image(self):
@@ -493,57 +599,70 @@
         if self.pixelformat == "BayerRG8":
             frame_image = cv2.cvtColor(frame_image, cv2.COLOR_BayerRG2BGR)
         self.last_image_cleared.set()
         return frame_image
 
     def camera_info(self):
         """
-        Retrieves and logs the camera's essential information such as frame dimensions and channels.
+        Retrieves and logs the camera's essential information 
+        such as frame dimensions and channels.
         """
         # Gather camera details
         self.height = self.camera.Height()
         self.width = self.camera.Width()
         try:
             if self.last_image is not None:
                 self.channels = self.last_image.GetNumChannels()
         except Exception as e:
             logger.error(f"An error occurred while getting channel info: {e}")
-        logger.info(f"camera frame width: {self.width}, height: {self.width}, channels: {self.channels}")
+        logger.info(
+            f"camera frame width: {self.width}, height: {self.width}, channels: {self.channels}"
+        )
 
         # Set frame rate equal to the current acquisition frame rate (Hz)
-        nodeFramerate = PySpin.CFloatPtr(self.node_map.GetNode('AcquisitionFrameRate'))
-        if (not PySpin.IsAvailable(nodeFramerate)) or (not PySpin.IsReadable(nodeFramerate)):
-            logger.error('Unable to retrieve frame rate. Aborting...')
+        nodeFramerate = PySpin.CFloatPtr(
+            self.node_map.GetNode("AcquisitionFrameRate")
+        )
+        if (not PySpin.IsAvailable(nodeFramerate)) or (
+            not PySpin.IsReadable(nodeFramerate)
+        ):
+            logger.error("Unable to retrieve frame rate. Aborting...")
             return -1
         self.frame_rate = nodeFramerate.GetValue()
         logger.info(f"Frame rate to be set to {self.frame_rate}")
 
-    def save_recording(self, filepath, isTimestamp=False, custom_name="Microscope_"):
+    def save_recording(
+        self, filepath, isTimestamp=False, custom_name="Microscope_"
+    ):
         """
         Begins video recording and saves the video to the specified file path.
 
         Args:
         - filepath (str): Directory to save the video.
         - isTimestamp (bool): Whether to append a timestamp to the filename.
         - custom_name (str): Custom prefix for the filename.
         """
         # Formulate the video name based on the input parameters
-        video_name = "{}_{}.avi".format(custom_name, self.get_last_capture_time()) \
-            if isTimestamp else "{}.avi".format(custom_name)
+        video_name = (
+            "{}_{}.avi".format(custom_name, self.get_last_capture_time())
+            if isTimestamp
+            else "{}.avi".format(custom_name)
+        )
         full_path = os.path.join(filepath, video_name)
         print(f"Saving video to {full_path}")
         logger.debug(f"Try saving video to {full_path}")
 
         # Update camera details
         self.camera_info()
 
         # Begin the video recording with appropriate configurations
-        fourcc = cv2.VideoWriter_fourcc(*'XVID')
-        self.video_output = cv2.VideoWriter(full_path, fourcc, self.frame_rate, \
-                                            (self.width, self.height), True) 
+        fourcc = cv2.VideoWriter_fourcc(*"XVID")
+        self.video_output = cv2.VideoWriter(
+            full_path, fourcc, self.frame_rate, (self.width, self.height), True
+        )
         self.video_recording_on.set()
 
     def stop_recording(self):
         """
         Stops the ongoing video capture process and releases video resources.
         """
         self.video_recording_on.clear()
@@ -553,144 +672,156 @@
 
     # Clean up the camera
     def stop(self, clean=False):
         """
         Cleans up resources associated with the camera and video recording.
 
         Note:
-            Do not change the order of codes without refering PySpin manual.
-            They are ordered by PySpin Camera Init / Turn off sequence. 
+            Do not change the order of codes without referring PySpin manual.
+            They are ordered by PySpin Camera Init / Turn off sequence.
         """
         if self.running:
             self.running = False
             self.capture_thread.join()
             self.camera.EndAcquisition()
             self.last_image = None
             self.last_image_filled.clear()
 
         if self.video_recording_on.is_set():
             self.stop_recording()
-        
+
         if clean:
             del self.camera
 
+
 # Class for simulating a mock camera
 class MockCamera:
-    """ Mock Camera showing salts and pepper noise images """
+    """Mock Camera showing salts and pepper noise images"""
+
     n_cameras = 0
+
     def __init__(self):
-        """ Initialize a mock camera with a unique name """
+        """Initialize a mock camera with a unique name"""
         self._name = f"MockCamera{MockCamera.n_cameras}"
         MockCamera.n_cameras += 1
         # Create mock image data with random values
-        self.data = np.random.randint(0, 255, size=(5, 3000, 4000), dtype='ubyte')
+        self.data = np.random.randint(
+            0, 255, size=(5, 3000, 4000), dtype="ubyte"
+        )
         self._next_frame = 0
         self.device_color_type = None
-        
+
     def name(self, sn_only=False):
-        """ Get the name of the mock camera """
+        """Get the name of the mock camera"""
         return self._name
 
     def get_last_image_data(self):
         """
-        Return last image as numpy array with shape (height, width, 3) for RGB or (height, width) for mono. 
+        Return last image as numpy array with shape (height, width, 3) for RGB
+		or (height, width) for mono.
         """
         frame = self.data[self._next_frame]
         self._next_frame = (self._next_frame + 1) % self.data.shape[0]
         return frame
-    
-    def save_last_image(self, filepath, isTimestamp=False, custom_name="MockCamera_"):
-        """ Dummy function """
+
+    def save_last_image(
+        self, filepath, isTimestamp=False, custom_name="MockCamera_"
+    ):
+        """Dummy function"""
         print("This is MockCamera. Cannot capture the image")
         return
-    
+
     def set_wb(self, wb=2.0):
-        """ Dummy function """
-        logger.info("This is MockCamera. Setting is not appliable")
+        """Dummy function"""
+        logger.info("This is MockCamera. Setting is not applicable")
         return
-    
+
     def set_gamma(self, gamma=1.0):
-        """ Dummy function """
-        logger.info("This is MockCamera. Setting is not appliable")
+        """Dummy function"""
+        logger.info("This is MockCamera. Setting is not applicable")
         return
 
     def set_gain(self, gain=25.0):
-        """ Dummy function """
-        logger.info("This is MockCamera. Setting is not appliable")
+        """Dummy function"""
+        logger.info("This is MockCamera. Setting is not applicable")
         return
-    
+
     def set_exposure(self, expTime=16000):
-        """ Dummy function """
-        logger.info("This is MockCamera. Setting is not appliable")
+        """Dummy function"""
+        logger.info("This is MockCamera. Setting is not applicable")
         return
 
     def stop(self, clean=False):
-        """ Dummy function """
+        """Dummy function"""
         logger.info("This is MockCamera. Stop")
         return
-    
+
     def begin_continuous_acquisition(self):
-        """ Dummy function """
+        """Dummy function"""
         return
-    
+
     def get_last_capture_time(self, millisecond=False):
-        """ Dummy function """
-        return 
-    
+        """Dummy function"""
+        return
+
     def stop(self, clean=False):
-        """ Dummy function """
+        """Dummy function"""
         return
-    
+
+
 class VideoSource:
-    """ Video Source """
+    """Video Source"""
+
     def __init__(self, filename):
-        """ Initialize a video source with a given filename """
+        """Initialize a video source with a given filename"""
         self.filename = filename
         self._name = os.path.basename(self.filename)
         self.cap = cv2.VideoCapture(self.filename)
 
     def name(self, sn_only=False):
-        """ Get the name of the video source """
+        """Get the name of the video source"""
         return self._name
 
     def get_last_image_data(self):
-        """ Read the last captured frame from the video source """
+        """Read the last captured frame from the video source"""
         ret, frame = self.cap.read()
         if ret:
             return frame
         else:
             # If the video has ended, reset the video source to the beginning
             self.cap.set(cv2.CAP_PROP_POS_FRAMES, 0)
-            return np.random.randint(0, 255, size=(3000, 4000), dtype='ubyte')
-        
-    def save_last_image(self, filepath, isTimestamp=False, custom_name="VideoSource_"):
-        """ Dummy function """
+            return np.random.randint(0, 255, size=(3000, 4000), dtype="ubyte")
+
+    def save_last_image(
+        self, filepath, isTimestamp=False, custom_name="VideoSource_"
+    ):
+        """Dummy function"""
         print("This is from Video Source. Cannot capture the image")
         return
-    
+
     def set_wb(self, wb=2.0):
-        """ Dummy function """
-        logger.info("This is VideoSource. Setting is not appliable")
+        """Dummy function"""
+        logger.info("This is VideoSource. Setting is not applicable")
         return
-    
+
     def set_gamma(self, gamma=1.0):
-        """ Dummy function """
-        logger.info("This is VideoSource. Setting is not appliable")
+        """Dummy function"""
+        logger.info("This is VideoSource. Setting is not applicable")
         return
 
     def set_gain(self, gain=25.0):
-        """ Dummy function """
-        logger.info("This is VideoSource. Setting is not appliable")
+        """Dummy function"""
+        logger.info("This is VideoSource. Setting is not applicable")
         return
-    
+
     def set_exposure(self, expTime=125000):
-        """ Dummy function """
-        logger.info("This is VideoSource. Setting is not appliable")
+        """Dummy function"""
+        logger.info("This is VideoSource. Setting is not applicable")
         return
-    
+
     def begin_continuous_acquisition(self):
-        """ Dummy function """
+        """Dummy function"""
         return
-    
+
     def stop(self, clean=False):
-        """ Dummy function """
-        return
+        """Dummy function"""
+        return
```

### Comparing `parallax_app-0.37.0/parallax/curr_bg_cmp_processor.py` & `parallax_app-0.37.1/parallax/curr_bg_cmp_processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 """
-CurrBgCmpProcessor: Module for finding the difference image using Current and Background Comparison.
+CurrBgCmpProcessor: Module for finding the difference image 
+using Current and Background Comparison.
 
-This module provides classes and methods for processing images to detect differences 
-between a current image and a background image, with the aim of detecting a probe and its tip.
+This module provides classes and methods for processing images 
+to detect differences between a current image and a background image, 
+with the aim of detecting a probe and its tip.
 
 Classes:
-    - CurrBgCmpProcessor: Main class for performing the comparison and detecting the probe.
+    - CurrBgCmpProcessor: Main class for performing the comparison
+      and detecting the probe.
 
 Usage:
     - Initialize an instance of CurrBgCmpProcessor with necessary parameters.
     - Use the first_cmp() method to perform the initial comparison.
-    - Use the update_cmp() method to update the comparison and detect changes over time.
+    - Use the update_cmp() method to update the comparison and detect changes 
+    over time.
 """
-from .utils import UtilsCoords, UtilsCrops
-from .probe_fine_tip_detector import ProbeFineTipDetector 
+
+import logging
+
 import cv2
 import numpy as np
-import logging
+
+from .probe_fine_tip_detector import ProbeFineTipDetector
+from .utils import UtilsCoords, UtilsCrops
 
 # Set logger name
 logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, 
+# to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class CurrBgCmpProcessor(UtilsCoords, UtilsCrops, ProbeFineTipDetector):
     """Finding diff image using Current and Background Comparison"""
-    def __init__(self, ProbeDetector, original_size, resized_size, reticle_zone=None):
+
+    def __init__(
+        self, ProbeDetector, original_size, resized_size, reticle_zone=None
+    ):
         """
         Initialize the CurrBgCmpProcessor.
 
         Args:
             ProbeDetector (object): An instance of the ProbeDetector class.
             original_size (tuple): The original size of the image (height, width).
             resized_size (tuple): The resized size of the image (height, width).
@@ -47,23 +59,23 @@
         self.bg = None
         self.org_img = None
         self.IMG_SIZE = resized_size
         self.IMG_SIZE_ORIGINAL = original_size
         self.ProbeDetector = ProbeDetector
         self.reticle_zone = reticle_zone
         self.crop_init = 50
-        
+
     def update_reticle_zone(self, reticle_zone):
         """Update the reticle zone.
-        
+
         Args:
             reticle_zone (numpy.ndarray): Reticle zone image.
         """
         self.reticle_zone = reticle_zone
-        
+
     def first_cmp(self, curr_img, mask, org_img, img_fname=None):
         """Perform first comparison
 
         Args:
             curr_img (numpy.ndarray): Current image.
             mask (numpy.ndarray): Mask image.
             org_img (numpy.ndarray): Original image.
@@ -81,16 +93,18 @@
         if self.bg is None:
             self._create_bg(self.curr_img)
         self._preprocess_diff_image(self.curr_img)
         ret = self._detect_probe()
         if ret:
             logger.debug("FirstCurrBgCmpProcessor:: detect")
             _ = self._get_precise_tip(org_img)
-            self.bg = cv2.bitwise_not(cv2.bitwise_xor(self.diff_img, self.curr_img), mask=self.mask)
-            
+            self.bg = cv2.bitwise_not(
+                cv2.bitwise_xor(self.diff_img, self.curr_img), mask=self.mask
+            )
+
         return ret
 
     def update_cmp(self, curr_img, mask, org_img, img_fname=None):
         """Update the comparison.
 
         Args:
             curr_img (numpy.ndarray): Current image.
@@ -104,102 +118,137 @@
         ret = False
         self.img_fname = img_fname
         self.mask = mask
         self.curr_img = curr_img
         self.curr_img = self._get_binary(self.curr_img)
         if self.bg is None:
             self._create_bg(self.curr_img)
-        
+
         self._preprocess_diff_image(self.curr_img)
         ret = self._update_crop()
         if ret:
-            ret_precise_tip = self._get_precise_tip(org_img)    
+            ret_precise_tip = self._get_precise_tip(org_img)
             self._update_bg()
             pass
-        
+
         return ret and ret_precise_tip
-    
+
     def _update_bg(self):
         """Update the background image."""
         kernel = np.ones((3, 3), np.uint8)
-        self.diff_img_crop = cv2.dilate(self.diff_img_crop, kernel, iterations=1)
-        
+        self.diff_img_crop = cv2.dilate(
+            self.diff_img_crop, kernel, iterations=1
+        )
+
         # Find and process contours
-        contours, _ = cv2.findContours(self.diff_img_crop, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+        contours, _ = cv2.findContours(
+            self.diff_img_crop, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
         if len(contours) >= 2:
             largest_contour = max(contours, key=cv2.contourArea)
             for contour in contours:
                 if contour is not largest_contour:
-                    self.diff_img_crop = cv2.drawContours(self.diff_img_crop, [contour], -1, (0, 0, 0), -1)
+                    self.diff_img_crop = cv2.drawContours(
+                        self.diff_img_crop, [contour], -1, (0, 0, 0), -1
+                    )
 
         # Initialize an empty image for drawing
         diff_img = np.zeros_like(self.diff_img)
-        
+
         # Calculate the direction and extend the line between probe tip and base
         offset = 10
-        tip_direction = np.array(self.ProbeDetector.probe_tip) - np.array(self.ProbeDetector.probe_base)
+        tip_direction = np.array(self.ProbeDetector.probe_tip) - np.array(
+            self.ProbeDetector.probe_base
+        )
         tip_direction_normalized = tip_direction / np.linalg.norm(tip_direction)
-        extended_probe_tip = tuple(np.array(self.ProbeDetector.probe_tip) + (offset * tip_direction_normalized).astype(int))
-        extended_probe_base = tuple(np.array(self.ProbeDetector.probe_base) - (offset * tip_direction_normalized).astype(int))
-        
+        extended_probe_tip = tuple(
+            np.array(self.ProbeDetector.probe_tip)
+            + (offset * tip_direction_normalized).astype(int)
+        )
+        extended_probe_base = tuple(
+            np.array(self.ProbeDetector.probe_base)
+            - (offset * tip_direction_normalized).astype(int)
+        )
+
         # Draw the extended line
-        cv2.line(diff_img, extended_probe_tip, extended_probe_base, 255, thickness=5)
-        
+        cv2.line(
+            diff_img, extended_probe_tip, extended_probe_base, 255, thickness=5
+        )
+
         # Combine the processed image with the current image to extract the background
         self.bg = cv2.bitwise_and(self.curr_img, cv2.bitwise_not(diff_img))
         self.bg = cv2.bitwise_not(self.bg, mask=self.mask)
 
-
     def _update_crop(self):
         """Update the crop region.
 
         Returns:
             bool: True if probe is detected, False otherwise.
         """
-        #Draw
-        #diff_img_ = self.diff_img.copy()
-        #diff_img_ = cv2.cvtColor(diff_img_, cv2.COLOR_GRAY2BGR)
+        # Draw
+        # diff_img_ = self.diff_img.copy()
+        # diff_img_ = cv2.cvtColor(diff_img_, cv2.COLOR_GRAY2BGR)
 
         ret = False
         crop_size = self.crop_init
         crop_utils = UtilsCrops()
-        while (ret is False) and (crop_size <= max(self.IMG_SIZE[0], self.IMG_SIZE[1])):
-            top, bottom, left, right = crop_utils.calculate_crop_region(self.ProbeDetector.probe_tip, \
-                                                        self.ProbeDetector.probe_base, crop_size, self.IMG_SIZE)
+        while (ret is False) and (
+            crop_size <= max(self.IMG_SIZE[0], self.IMG_SIZE[1])
+        ):
+            top, bottom, left, right = crop_utils.calculate_crop_region(
+                self.ProbeDetector.probe_tip,
+                self.ProbeDetector.probe_base,
+                crop_size,
+                self.IMG_SIZE,
+            )
             self.diff_img_crop = self.diff_img[top:bottom, left:right]
-            hough_minLineLength_adpative = 60 + int(crop_size/self.crop_init)*5
-            ret = self.ProbeDetector.update_probe(self.diff_img_crop, self.mask, \
-                                                    hough_minLineLength=hough_minLineLength_adpative, maxLineGap=0,\
-                                                    offset_x = left, offset_y = top, img_fname=self.img_fname)
-            
-            #cv2.rectangle(diff_img_, (left, top), (right, bottom), (155, 155, 0), 5)  # Green rectangle
-            
-            if ret and crop_utils.is_point_on_crop_region(self.ProbeDetector.probe_tip, top, bottom, left, right, buffer=5):            
+            hough_minLineLength_adpative = (
+                60 + int(crop_size / self.crop_init) * 5
+            )
+            ret = self.ProbeDetector.update_probe(
+                self.diff_img_crop,
+                self.mask,
+                hough_minLineLength=hough_minLineLength_adpative,
+                maxLineGap=0,
+                offset_x=left,
+                offset_y=top,
+                img_fname=self.img_fname,
+            )
+
+            # cv2.rectangle(diff_img_, (left, top), (right, bottom), (155, 155, 0), 5)  # Green rectangle
+
+            if ret and crop_utils.is_point_on_crop_region(
+                self.ProbeDetector.probe_tip, top, bottom, left, right, buffer=5
+            ):
                 ret = False
             """
             if ret:
                 cv2.circle(diff_img_, self.ProbeDetector.probe_tip, 3, (0, 0, 255), -1)  # RED circle
                 cv2.circle(diff_img_, self.ProbeDetector.probe_base, 3, (0, 255, 0), -1)  # Green circle
                 cv2.imwrite('debug/crop.jpg', diff_img_)
                 cv2.imwrite('debug/reticle_zone.jpg', self.reticle_zone)
             """
             if ret and self.reticle_zone is not None:
-                tip_in_reticle = self._is_point_in_reticle_region(self.reticle_zone, self.ProbeDetector.probe_tip)
-                base_in_reticle = self._is_point_in_reticle_region(self.reticle_zone, self.ProbeDetector.probe_base)
+                tip_in_reticle = self._is_point_in_reticle_region(
+                    self.reticle_zone, self.ProbeDetector.probe_tip
+                )
+                base_in_reticle = self._is_point_in_reticle_region(
+                    self.reticle_zone, self.ProbeDetector.probe_base
+                )
                 if tip_in_reticle and base_in_reticle:
                     return False
-            
+
             if ret:
                 break
-            
+
             crop_size += 100
-        
-        del crop_utils # Garbage Collect 
+
+        del crop_utils  # Garbage Collect
         return ret
-        
+
     def _is_point_in_reticle_region(self, image, point):
         """Check if a point is in the reticle region."""
         return image[point[1], point[0]] == 255
 
     def _get_precise_tip(self, org_img):
         """Get precise probe tip on original size image
         Args:
@@ -209,45 +258,63 @@
             bool: True if precise tip is found, False otherwise.
         """
         coords_utils = UtilsCoords(self.IMG_SIZE_ORIGINAL, self.IMG_SIZE)
         probe_fine_tip = ProbeFineTipDetector()
         crop_utils = UtilsCrops()
         ret = False
 
-        probe_tip_original_coords = coords_utils.scale_coords_to_original(self.ProbeDetector.probe_tip)
-        top, bottom, left, right = crop_utils.calculate_crop_region(probe_tip_original_coords, \
-                                            probe_tip_original_coords, crop_size=20, IMG_SIZE=self.IMG_SIZE_ORIGINAL)
+        probe_tip_original_coords = coords_utils.scale_coords_to_original(
+            self.ProbeDetector.probe_tip
+        )
+        top, bottom, left, right = crop_utils.calculate_crop_region(
+            probe_tip_original_coords,
+            probe_tip_original_coords,
+            crop_size=20,
+            IMG_SIZE=self.IMG_SIZE_ORIGINAL,
+        )
         self.tip_image = org_img[top:bottom, left:right]
-        ret = probe_fine_tip.get_precise_tip(self.tip_image, probe_tip_original_coords, \
-                                            offset_x=left, offset_y=top, \
-                                            direction=self.ProbeDetector.probe_tip_direction, img_fname=self.img_fname)
+        ret = probe_fine_tip.get_precise_tip(
+            self.tip_image,
+            probe_tip_original_coords,
+            offset_x=left,
+            offset_y=top,
+            direction=self.ProbeDetector.probe_tip_direction,
+            img_fname=self.img_fname,
+        )
         if ret:
             self.ProbeDetector.probe_tip_org = probe_fine_tip.tip
 
-        del probe_fine_tip # Garbage Collect
+        del probe_fine_tip  # Garbage Collect
         del coords_utils
         del crop_utils
-        
+
         return ret
 
     def _get_binary(self, curr_img):
         """Get binary image.
         Args:
             curr_img (numpy.ndarray): Current image.
         Returns:
             numpy.ndarray: Binary image.
         """
-        curr_img = cv2.adaptiveThreshold(curr_img, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY, 17, 2)
+        curr_img = cv2.adaptiveThreshold(
+            curr_img,
+            255,
+            cv2.ADAPTIVE_THRESH_GAUSSIAN_C,
+            cv2.THRESH_BINARY,
+            17,
+            2,
+        )
         curr_img = cv2.bitwise_not(curr_img)
         return curr_img
-    
+
     def _create_bg(self, curr_img):
         """Create background image."""
         self.bg = cv2.bitwise_not(curr_img)
 
     def _preprocess_diff_image(self, curr_img):
         """Preprocess difference image."""
         self.diff_img = cv2.bitwise_and(curr_img, self.bg, mask=self.mask)
-    
+
     def _detect_probe(self):
         """Detect probe in difference image."""
         return self.ProbeDetector.first_detect_probe(self.diff_img, self.mask)
```

### Comparing `parallax_app-0.37.0/parallax/curr_prev_cmp_processor.py` & `parallax_app-0.37.1/parallax/curr_prev_cmp_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 """
-CurrPrevCmpProcessor: Module for finding the difference image using Current Previous Comparison.
+CurrPrevCmpProcessor: Module for finding the difference image 
+using Current Previous Comparison.
 
-This module provides classes and methods for processing images to detect differences between a current image and a previous image, with the aim of detecting a probe and its tip.
+This module provides classes and methods for processing images
+to detect differences between a current image and a previous image, with the aim of detecting a probe and its tip.
 
 Classes:
-    - CurrPrevCmpProcessor: Main class for performing the comparison and detecting the probe.
+    - CurrPrevCmpProcessor: Main class for performing
+      the comparison and detecting the probe.
 
 Usage:
     - Initialize an instance of CurrPrevCmpProcessor with necessary parameters.
     - Use the first_cmp() method to perform the initial comparison.
-    - Use the update_cmp() method to update the comparison and detect changes over time.
+    - Use the update_cmp() method to update the comparison
+      and detect changes over time.
 """
-from .utils import UtilsCoords, UtilsCrops
-from .probe_fine_tip_detector import ProbeFineTipDetector 
+
+import logging
 import os
+
 import cv2
 import numpy as np
 
-import logging
+from .probe_fine_tip_detector import ProbeFineTipDetector
+from .utils import UtilsCoords, UtilsCrops
+
 # Set logger name
 logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+# Set the logging level for PyQt5.uic.uiparser/properties
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class CurrPrevCmpProcessor(UtilsCoords, UtilsCrops, ProbeFineTipDetector):
     """Finding diff image using Current Previous Comparison"""
+
     def __init__(self, ProbeDetector, original_size, resized_size):
         """
         Initialize the CurrPrevCmpProcessor.
 
         Args:
             ProbeDetector (object): An instance of the ProbeDetector class.
             original_size (tuple): The original size of the image (height, width).
@@ -61,24 +70,24 @@
 
         Returns:
             bool: True if probe is detected, False otherwise.
         """
         ret = False
         self.img_fname = img_fname
         self.mask = mask
-        self._preprocess_diff_images(curr_img, prev_img) # Subtraction
+        self._preprocess_diff_images(curr_img, prev_img)  # Subtraction
         if not self._apply_threshold():
             return ret
         ret = self.ProbeDetector.first_detect_probe(self.diff_img, self.mask)
         if ret:
             logger.debug("CurrPrevCmpProcessor First::detect")
             ret_precise_tip = self._get_precise_tip(org_img)
 
-        return ret 
-    
+        return ret
+
     def update_cmp(self, curr_img, prev_img, mask, org_img, img_fname=None):
         """Update the comparison.
 
         Args:
             curr_img (numpy.ndarray): Current image.
             prev_img (numpy.ndarray): Previous image.
             mask (numpy.ndarray): Mask image.
@@ -87,95 +96,120 @@
 
         Returns:
             bool: True if probe is detected and precise tip is found, False otherwise.
         """
         ret = False
         self.img_fname = img_fname
         self.mask = mask
-        self._preprocess_diff_images(curr_img, prev_img) # Subtraction
+        self._preprocess_diff_images(curr_img, prev_img)  # Subtraction
         if not self._apply_threshold():
             return False
         ret = self._update_crop()
         if ret:
             logger.debug("CurrPrevCmpProcessor Update::detect")
             ret_precise_tip = self._get_precise_tip(org_img)
 
         return ret and ret_precise_tip
-    
+
     def _update_crop(self):
         """Update the crop region.
 
         Returns:
             bool: True if probe is detected, False otherwise.
-        """    
-        #Draw
-        #diff_img_ = self.diff_img.copy()
-        #diff_img_ = cv2.cvtColor(diff_img_, cv2.COLOR_GRAY2BGR)
+        """
+        # Draw
+        # diff_img_ = self.diff_img.copy()
+        # diff_img_ = cv2.cvtColor(diff_img_, cv2.COLOR_GRAY2BGR)
 
         ret = False
         crop_size = self.crop_init
         crop_utils = UtilsCrops()
-        while (ret is False) and (crop_size <= max(self.IMG_SIZE[0], self.IMG_SIZE[1])):
-            top, bottom, left, right = crop_utils.calculate_crop_region(self.ProbeDetector.probe_tip, \
-                                                        self.ProbeDetector.probe_base, crop_size, self.IMG_SIZE)
+        while (ret is False) and (
+            crop_size <= max(self.IMG_SIZE[0], self.IMG_SIZE[1])
+        ):
+            top, bottom, left, right = crop_utils.calculate_crop_region(
+                self.ProbeDetector.probe_tip,
+                self.ProbeDetector.probe_base,
+                crop_size,
+                self.IMG_SIZE,
+            )
             diff_img_crop = self.diff_img[top:bottom, left:right]
-            hough_minLineLength_adpative = 40 + int(crop_size/self.crop_init)*5
-            ret = self.ProbeDetector.update_probe(diff_img_crop, self.mask, \
-                                                    hough_minLineLength=hough_minLineLength_adpative, \
-                                                    offset_x = left, offset_y = top, img_fname=self.img_fname)
-            #cv2.rectangle(diff_img_, (left, top), (right, bottom), (0, 155, 155), 5)  # Green rectangle
-
-            if ret and crop_utils.is_point_on_crop_region(self.ProbeDetector.probe_tip, top, bottom, left, right):
+            hough_minLineLength_adpative = (
+                40 + int(crop_size / self.crop_init) * 5
+            )
+            ret = self.ProbeDetector.update_probe(
+                diff_img_crop,
+                self.mask,
+                hough_minLineLength=hough_minLineLength_adpative,
+                offset_x=left,
+                offset_y=top,
+                img_fname=self.img_fname,
+            )
+            # cv2.rectangle(diff_img_, (left, top), (right, bottom), (0, 155, 155), 5)  # Green rectangle
+
+            if ret and crop_utils.is_point_on_crop_region(
+                self.ProbeDetector.probe_tip, top, bottom, left, right
+            ):
                 ret = False
-            
+
             """
             if ret:
                 cv2.circle(diff_img_, self.ProbeDetector.probe_tip, 3, (0, 0, 255), -1)  # RED circle
                 cv2.circle(diff_img_, self.ProbeDetector.probe_base, 3, (0, 255, 0), -1)  # RED circle
                 #output_fname = os.path.basename(self.img_fname).replace('.', '_2_diff_thres.')
                 #cv2.imwrite('output/' + output_fname, diff_img_)
                 break
             """
-            
+
             crop_size += 100
 
-        del crop_utils # Garbage Collect
+        del crop_utils  # Garbage Collect
         return ret
 
-
     def _get_precise_tip(self, org_img):
         """Get precise probe tip using original image
 
         Args:
             org_img (numpy.ndarray): Original image.
 
         Returns:
             bool: True if precise tip is found, False otherwise.
         """
         coords_utils = UtilsCoords(self.IMG_SIZE_ORIGINAL, self.IMG_SIZE)
         probe_fine_tip = ProbeFineTipDetector()
         crop_utils = UtilsCrops()
         ret = False
 
-        probe_tip_original_coords = coords_utils.scale_coords_to_original(self.ProbeDetector.probe_tip)
-        top, bottom, left, right = crop_utils.calculate_crop_region(probe_tip_original_coords, \
-                                            probe_tip_original_coords, crop_size=25, IMG_SIZE=self.IMG_SIZE_ORIGINAL)
+        probe_tip_original_coords = coords_utils.scale_coords_to_original(
+            self.ProbeDetector.probe_tip
+        )
+        top, bottom, left, right = crop_utils.calculate_crop_region(
+            probe_tip_original_coords,
+            probe_tip_original_coords,
+            crop_size=25,
+            IMG_SIZE=self.IMG_SIZE_ORIGINAL,
+        )
         self.tip_image = org_img[top:bottom, left:right]
-        ret = probe_fine_tip.get_precise_tip(self.tip_image, probe_tip_original_coords, \
-                                            offset_x=left, offset_y=top, \
-                                            direction=self.ProbeDetector.probe_tip_direction, img_fname=self.img_fname)
+        ret = probe_fine_tip.get_precise_tip(
+            self.tip_image,
+            probe_tip_original_coords,
+            offset_x=left,
+            offset_y=top,
+            direction=self.ProbeDetector.probe_tip_direction,
+            img_fname=self.img_fname,
+        )
         if ret:
             self.ProbeDetector.probe_tip_org = probe_fine_tip.tip
 
-        del probe_fine_tip # Garbage Collect
+        del probe_fine_tip  # Garbage Collect
         del coords_utils
         del crop_utils
-        
+
         return ret
-          
+
     def _detect_probe(self):
         """Detect probe in difference image.
 
         Returns:
             bool: True if probe is detected, False otherwise.
         """
         return self.ProbeDetector.first_detect_probe(self.diff_img, self.mask)
@@ -184,27 +218,33 @@
         """Subtract current image from previous image to find differences.
 
         Args:
             curr_img (numpy.ndarray): Current image.
             prev_img (numpy.ndarray): Previous image.
         """
         self.diff_img = cv2.subtract(prev_img, curr_img, mask=self.mask)
-        #output_fname = os.path.basename(self.img_fname).replace('.', '_2_diff.')
-        #cv2.imwrite('output/' + output_fname, self.diff_img)
+        # output_fname = os.path.basename(self.img_fname).replace('.', '_2_diff.')
+        # cv2.imwrite('output/' + output_fname, self.diff_img)
 
     def _apply_threshold(self):
         """Apply threshold to suppress shadows and check significant differences.
 
         Returns:
             bool: True if significant differences are found, False otherwise.
         """
         max_value = np.max(self.diff_img)
         if max_value < 20:
-            logger.debug(f"Not strong pattern detected on diff image. max_value: {max_value}")
+            logger.debug(
+                f"Not strong pattern detected on diff image. max_value: {max_value}"
+            )
             return False
-        
+
         threshold_value = self.shadow_threshold * max_value
         self.diff_img[self.diff_img < threshold_value] = 0
-        _, self.diff_img = cv2.threshold(self.diff_img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
-        self.diff_img = cv2.bitwise_and(self.diff_img, self.diff_img, mask=self.mask)
+        _, self.diff_img = cv2.threshold(
+            self.diff_img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU
+        )
+        self.diff_img = cv2.bitwise_and(
+            self.diff_img, self.diff_img, mask=self.mask
+        )
 
         return True
```

### Comparing `parallax_app-0.37.0/parallax/main_window_wip.py` & `parallax_app-0.37.1/parallax/main_window_wip.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,272 +1,301 @@
 """
-This script defines the main components of the application including the main window, UI elements,
+This script defines the main components of the application
+including the main window, UI elements,
 camera and stage management, and recording functionality.
 
 Modules imported:
 - PyQt5 modules for building the graphical user interface.
 - Other libraries and modules necessary for the application's functionality.
 
 Classes:
 - MainWindow: Represents the main window of the application.
 """
-# Import required PyQt5 modules and other libraries
-from PyQt5.QtWidgets import QApplication, QMainWindow, QWidget, QFileDialog, QScrollArea, QSplitter, QGridLayout
-from PyQt5.QtWidgets import QGroupBox, QVBoxLayout, QToolButton
-from PyQt5.QtCore import QCoreApplication, QStandardPaths, QTimer, QPoint
+
+import logging
+import os
+from functools import partial
+
+from PyQt5.QtCore import QCoreApplication, QPoint, QStandardPaths, QTimer
 from PyQt5.QtGui import QFont, QFontDatabase
+# Import required PyQt5 modules and other libraries
+from PyQt5.QtWidgets import (QApplication, QFileDialog, QGridLayout, QGroupBox,
+                             QMainWindow, QScrollArea, QSplitter, QToolButton,
+                             QVBoxLayout, QWidget)
 from PyQt5.uic import loadUi
-from .screen_widget import ScreenWidget
+
 from .recording_manager import RecordingManager
+from .screen_widget import ScreenWidget
 from .stage_widget import StageWidget
 from .user_setting_manager import UserSettingsManager
-from functools import partial
-import os
-import logging
 
 # Set logger name
 logger = logging.getLogger(__name__)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+# Set the logging level for PyQt5.uic.uiparser/properties
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
 # User Preferences (Data directory, UI config..) setting file
 package_dir = os.path.dirname(os.path.abspath(__file__))
-ui_dir = os.path.join(os.path.dirname(package_dir), 'ui')
-SETTINGS_FILE = 'settings.json'
+ui_dir = os.path.join(os.path.dirname(package_dir), "ui")
+SETTINGS_FILE = "settings.json"
+
 
 # Main application window
 class MainWindow(QMainWindow):
     """
     The main window of the application.
-    
-    This class represents the main window of the application and handles the user interface
+
+    This class represents the main window of the application
+    and handles the user interface
     components, camera and stage management, and recording functionality.
     """
+
     def __init__(self, model, dummy=False):
         """
         Initialize the MainWindow.
-        
+
         Args:
             model (object): The data model for the application.
-            dummy (bool, optional): Flag indicating whether to run in dummy mode. Defaults to False.
+            dummy (bool, optional): Flag indicating whether
+            to run in dummy mode. Defaults to False.
         """
-        QMainWindow.__init__(self) # Initialize the QMainWindow
+        QMainWindow.__init__(self)  # Initialize the QMainWindow
         self.model = model
         self.dummy = dummy
-        # self.model.clean() TBD call to close the camera when there was abnormal program exit in previous run.
-
+        
         # Initialize an empty list to keep track of microscopeGrp widgets instances
         self.screen_widgets = []
         self.recording_camera_list = []
-        
+
         # Update camera information
         self.refresh_cameras()
-        logger.debug(f"nPySpinCameras: {self.model.nPySpinCameras}, nMockCameras: {self.model.nMockCameras}")
-    
+        logger.debug(
+            f"nPySpinCameras: {self.model.nPySpinCameras}, nMockCameras: {self.model.nMockCameras}"
+        )
+
         # Update stage information
         self.refresh_stages()
         logger.debug(f"stages: {self.model.stages}")
-        
+
         self.user_setting = UserSettingsManager()
         # Load column configuration from user preferences
         self.nColumn = self.user_setting.load_settings_item("main", "nColumn")
         if self.nColumn is None or 0:
             self.nColumn = 1
         if self.model.nPySpinCameras:
             self.nColumn = min(self.model.nPySpinCameras, self.nColumn)
 
         # Load the main widget with UI components
         ui = os.path.join(ui_dir, "mainWindow.ui")
         loadUi(ui, self)
 
         # Load Fira Code font
-        fira_code_font_path = os.path.join(ui_dir, "font/FiraCode-VariableFont_wght.ttf")
+        fira_code_font_path = os.path.join(
+            ui_dir, "font/FiraCode-VariableFont_wght.ttf"
+        )
         QFontDatabase.addApplicationFont(fira_code_font_path)
-        fira_code_font = QFont("Fira Code Light", 10) # Setting font size to 10
+        fira_code_font = QFont("Fira Code Light", 10)  # Setting font size to 10
         QApplication.setFont(fira_code_font)
 
         # Load existing user preferences
-        nColumn, directory, width, height = self.user_setting.load_mainWindow_settings()
+        nColumn, directory, width, height = (
+            self.user_setting.load_mainWindow_settings()
+        )
         self.nColumnsSpinBox.setValue(nColumn)
-        self.dirLabel.setText(directory) 
+        self.dirLabel.setText(directory)
         if width is not None and height is not None:
             self.resize(width, height)
-                        
+
         # Attach directory selection event handler for saving files
         self.browseDirButton.clicked.connect(self.dir_setting_handler)
 
         # Configure the column spin box
         self.nColumnsSpinBox.setMaximum(max(self.model.nPySpinCameras, 1))
         self.nColumnsSpinBox.setValue(self.nColumn)
         if self.model.nPySpinCameras:
-            self.nColumnsSpinBox.valueChanged.connect(self.column_changed_handler)
+            self.nColumnsSpinBox.valueChanged.connect(
+                self.column_changed_handler
+            )
 
         # Refreshing the settingMenu while it is toggled
         self.settings_refresh_timer = QTimer()
 
         # Create the widget for screen
         self.scrollArea = QScrollArea(self.centralwidget)
         self.scrollArea.setWidgetResizable(True)
         self.scrollArea.setObjectName("scrollArea")
         self.scrollAreaWidgetContents = QWidget()
         self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
         self.gridLayout = QGridLayout(self.scrollAreaWidgetContents)
 
         # Dynamically generate Microscope display
         if self.model.nPySpinCameras:
-            self.display_microscope() # Attach screen widget
-        else: # Display only mock camera
+            self.display_microscope()  # Attach screen widget
+        else:  # Display only mock camera
             self.display_mock_camera()
 
         # Stage_widget
         self.stage_widget = StageWidget(self.model, ui_dir, self.screen_widgets)
         splitter = QSplitter()
         splitter.addWidget(self.scrollAreaWidgetContents)
         splitter.addWidget(self.stage_widget)
         self.verticalLayout_4.addWidget(splitter)
 
-        # Start button. If toggled, start camera acquisition  
+        # Start button. If toggled, start camera acquisition
         self.startButton.clicked.connect(self.start_button_handler)
-        
+
         # Recording functions
         self.recordingManager = RecordingManager(self.model)
-        self.snapshotButton.clicked.connect(lambda: \
-                self.recordingManager.save_last_image(self.dirLabel.text(), self.screen_widgets))
-        self.recordButton.clicked.connect(self.record_button_handler)       # Recording video button
+        self.snapshotButton.clicked.connect(
+            lambda: self.recordingManager.save_last_image(
+                self.dirLabel.text(), self.screen_widgets
+            )
+        )
+        self.recordButton.clicked.connect(
+            self.record_button_handler
+        )  # Recording video button
 
         # Refreshing the screen timer
         self.refresh_timer = QTimer()
         self.refresh_timer.timeout.connect(self.refresh)
 
         # Toggle start button on init
         self.start_button_handler()
-    
+
     def refresh_cameras(self):
         """
         This method is responsible for scanning for available cameras and updating the camera list.
         It adds mock cameras for testing purposes and scans for actual cameras if the application
         is not in dummy mode. This ensures that the list of available cameras is always up-to-date.
         """
         # Add mock cameras for testing purposes
         self.model.add_mock_cameras()
         # If not in dummy mode, scan for actual available cameras
         if not self.dummy:
             try:
                 self.model.scan_for_cameras()
             except Exception as e:
-                    print(f" Something still holds a reference to the camera.\n {e}")
+                print(
+                    f" Something still holds a reference to the camera.\n {e}"
+                )
 
     def refresh_stages(self):
-        """ Search for connected stages """
+        """Search for connected stages"""
         if not self.dummy:
             self.model.scan_for_usb_stages()
 
     def record_button_handler(self):
         """
         Handles the record button press event.
         If the record button is checked, start recording. Otherwise, stop recording.
         """
         if self.recordButton.isChecked():
-            save_path = self.dirLabel.text() 
+            save_path = self.dirLabel.text()
             self.recordingManager.save_recording(save_path, self.screen_widgets)
         else:
             self.recordingManager.stop_recording(self.screen_widgets)
-            
+
     def start_button_handler(self):
         """
         Handles the start button press event.
-        
+
         If the start button is checked, initiate acquisition from all cameras and start refreshing images.
         If unchecked, stop acquisition from all cameras and stop refreshing images.
         """
         # Initialize the list to keep track of cameras that have been started or stopped
         refresh_camera_list = []
-        
+
         # Check if the start button is toggled on
         if self.startButton.isChecked():
             print("\nRefreshing Screen")
             # Camera begin acquisition
             for screen in self.screen_widgets:
                 camera_name = screen.get_camera_name()
                 if camera_name not in refresh_camera_list:
                     screen.start_acquisition_camera()
                     refresh_camera_list.append(camera_name)
-            
+
             # Refreshing images to display screen
             self.refresh_timer.start(125)
 
-            # Start button is checked, enable record and snapshot button. 
+            # Start button is checked, enable record and snapshot button.
             self.recordButton.setEnabled(True)
             self.snapshotButton.setEnabled(True)
 
-        else:  
+        else:
             print("Stop Refreshing Screen")
-            # Start button is unchecked, disable record and snapshot button. 
+            # Start button is unchecked, disable record and snapshot button.
             self.recordButton.setEnabled(False)
             self.recordButton.setChecked(False)
             self.snapshotButton.setEnabled(False)
-            
+
             # Stop Refresh: stop refreshing images to display screen
             if self.refresh_timer.isActive():
                 self.refresh_timer.stop()
 
             # End acquisition from camera: stop acquiring images from camera to framebuffer
             for screen in self.screen_widgets:
                 camera_name = screen.get_camera_name()
                 if camera_name not in refresh_camera_list:
                     screen.stop_acquisition_camera()
                     refresh_camera_list.append(camera_name)
 
     def refresh(self):
-        """ Refreshing from framebuffer to screen"""
+        """Refreshing from framebuffer to screen"""
         for screen in self.screen_widgets:
-            screen.refresh()        # Refresh the screens
-        
+            screen.refresh()  # Refresh the screens
+
     def display_mock_camera(self):
         """Display mock camera when there is no detected camera."""
         self.createNewGroupBox(0, 0, mock=True)
 
     def display_microscope(self):
         """Dynamically arrange Microscopes based on camera count and column configuration."""
         # Calculate rows and columns
-        rows, cols, cnt = self.model.nPySpinCameras//self.nColumn, self.nColumn, 0
+        rows, cols, cnt = (
+            self.model.nPySpinCameras // self.nColumn,
+            self.nColumn,
+            0,
+        )
         rows += 1 if self.model.nPySpinCameras % cols else 0
         # Create grid of Microscope displays
-        for row_idx  in range(0, rows):
-            for col_idx  in range(0, cols):
+        for row_idx in range(0, rows):
+            for col_idx in range(0, cols):
                 if cnt < self.model.nPySpinCameras:
                     self.createNewGroupBox(row_idx, col_idx, screen_index=cnt)
                     cnt += 1
                 else:
-                    break # Stop when all Microscopes are displayed
+                    break  # Stop when all Microscopes are displayed
 
     def column_changed_handler(self, val):
         """Rearrange the layout of Microscopes when the column number changes."""
         # Identify current Microscope widgets
         camera_screen_list = []
         # Detach the identified widgets
         for i in range(self.gridLayout.count()):
             widget = self.gridLayout.itemAt(i).widget()
-            if isinstance(widget, QGroupBox):  # Ensure we're handling the correct type of widget
+            if isinstance(
+                widget, QGroupBox
+            ):  # Ensure we're handling the correct type of widget
                 camera_screen_list.append(widget)
 
         # Detach the identified widgets
         for widget in camera_screen_list:
             self.gridLayout.removeWidget(widget)
-            widget.hide() # Temporarily hide the widget
+            widget.hide()  # Temporarily hide the widget
 
         # Calculate new rows and columns layout
-        rows, cols, cnt = self.model.nPySpinCameras//val, val, 0
+        rows, cols, cnt = self.model.nPySpinCameras // val, val, 0
         rows += 1 if self.model.nPySpinCameras % cols else 0
 
         # Reattach widgets in the new layout
-        for row_idx  in range(0, rows):
-            for col_idx  in range(0, cols):
-                if cnt < len(camera_screen_list): 
+        for row_idx in range(0, rows):
+            for col_idx in range(0, cols):
+                if cnt < len(camera_screen_list):
                     widget = camera_screen_list[cnt]
                     self.gridLayout.addWidget(widget, row_idx, col_idx, 1, 1)
                     widget.show()  # Make the widget visible again
                     cnt += 1
                 else:
                     break
 
@@ -289,182 +318,284 @@
         newNameMicroscope = ""
         # Generate unique names based on camera number
         if mock:
             newNameMicroscope = "Mock Camera"
         else:
             newNameMicroscope = f"Microscope_{screen_index+1}"
         microscopeGrp = QGroupBox(self.scrollAreaWidgetContents)
-       
+
         # Construct and configure the Microscope widget
         microscopeGrp.setObjectName(newNameMicroscope)
-        microscopeGrp.setStyleSheet(u"background-color: rgb(58, 58, 58);")
+        microscopeGrp.setStyleSheet("background-color: rgb(58, 58, 58);")
         font_grpbox = QFont()
         font_grpbox.setPointSize(9)  # Setting font size to 9
         microscopeGrp.setFont(font_grpbox)
         verticalLayout = QVBoxLayout(microscopeGrp)
-        verticalLayout.setObjectName(u"verticalLayout")
-        
+        verticalLayout.setObjectName("verticalLayout")
+
         # Add screens
         if mock:
-            screen = ScreenWidget(self.model.cameras[0], model=self.model, parent=microscopeGrp)
+            screen = ScreenWidget(
+                self.model.cameras[0], model=self.model, parent=microscopeGrp
+            )
         else:
-            screen = ScreenWidget(self.model.cameras[screen_index], model=self.model, parent=microscopeGrp)
+            screen = ScreenWidget(
+                self.model.cameras[screen_index],
+                model=self.model,
+                parent=microscopeGrp,
+            )
         screen.setObjectName(f"Screen")
         verticalLayout.addWidget(screen)
-        
+
         if mock is False:
             # Add setting button
             settingButton = QToolButton(microscopeGrp)
             settingButton.setObjectName(f"Setting")
             settingButton.setFont(font_grpbox)
             settingButton.setCheckable(True)
-            self.create_settings_menu(microscopeGrp, newNameMicroscope, screen, screen_index)
-            settingButton.toggled.connect(lambda checked: self.show_settings_menu(settingButton, checked))
+            self.create_settings_menu(
+                microscopeGrp, newNameMicroscope, screen, screen_index
+            )
+            settingButton.toggled.connect(
+                lambda checked: self.show_settings_menu(settingButton, checked)
+            )
             verticalLayout.addWidget(settingButton)
-            settingButton.setText(QCoreApplication.translate("MainWindow", u"SETTINGS \u25ba", None))
-       
+            settingButton.setText(
+                QCoreApplication.translate(
+                    "MainWindow", "SETTINGS \u25ba", None
+                )
+            )
+
             # Load setting file from JSON
             self.update_setting_menu(microscopeGrp)
 
         # Add widget to the gridlayout
         self.gridLayout.addWidget(microscopeGrp, rows, cols, 1, 1)
-        
+
         # Add the new microscopeGrpBox instance to the list
-        self.screen_widgets.append(screen) 
+        self.screen_widgets.append(screen)
 
-    def create_settings_menu(self, microscopeGrp, newNameMicroscope, screen, screen_index):
+    def create_settings_menu(
+        self, microscopeGrp, newNameMicroscope, screen, screen_index
+    ):
         """
         Create the settings menu for each Microscope widget.
 
-        This function initializes the settings menu UI, loads it with necessary data, 
-        and associates the relevant signals with their slots. 
-        The settings menu is hidden by default and will be shown 
+        This function initializes the settings menu UI, loads it with necessary data,
+        and associates the relevant signals with their slots.
+        The settings menu is hidden by default and will be shown
         when the user toggles the settings button.
 
         Parameters:
         - microscopeGrp (QGroupBox): The group box representing a Microscope widget.
         - newNameMicroscope (str): The unique name assigned to the Microscope widget.
         - screen (ScreenWidget): The screen widget associated with the Microscope.
         - screen_index (int): The index of the camera in the model's camera list to be associated with this screen.
         """
         # Initialize the settings menu UI from the .ui file
         settingMenu = QWidget(microscopeGrp)
         setting_ui = os.path.join(ui_dir, "settingPopUpMenu.ui")
         loadUi(setting_ui, settingMenu)
-        settingMenu.setObjectName("SettingsMenu")        
+        settingMenu.setObjectName("SettingsMenu")
         settingMenu.hide()  # Hide the menu by default
-        
+
         # S/N
-        for sn in self.model.cameras_sn:        # Add the list of cameras (serial number) in ComboBox
+        # Add the list of cameras (serial number) in ComboBox
+        for sn in self.model.cameras_sn:        
             settingMenu.snComboBox.addItem(sn) 
-        sn = screen.get_camera_name()           # Select the sn for the current screen
+        # Select the sn for the current screen
+        sn = screen.get_camera_name()           
         index = settingMenu.snComboBox.findText(sn)
         if index >= 0:
             settingMenu.snComboBox.setCurrentIndex(index)
         else:
             logger.error("SN not found in the list")
 
         # If serial number is changed, connect to update_screen function and update setting menu
-        settingMenu.snComboBox.currentIndexChanged.connect(lambda: self.update_screen(screen, \
-                                             screen_index, settingMenu.snComboBox.currentText()))
-        
+        settingMenu.snComboBox.currentIndexChanged.connect(
+            lambda: self.update_screen(
+                screen, screen_index, settingMenu.snComboBox.currentText()
+            )
+        )
+
         # Custom name
-        customName = self.user_setting.load_settings_item(sn, "customName")  # Default name on init
+        customName = self.user_setting.load_settings_item(
+            sn, "customName"
+        )  # Default name on init
         customName = customName if customName else newNameMicroscope
         settingMenu.customName.setText(customName)
-        self.update_groupbox_name(microscopeGrp, customName)    # Update GroupBox name
-        # Name) If custom name is changed, change the groupBox name. 
-        settingMenu.customName.textChanged.connect(lambda: self.update_groupbox_name(microscopeGrp, \
-                                                                            settingMenu.customName.text()))
-        settingMenu.customName.textChanged.connect(lambda: self.user_setting.update_user_configs_settingMenu(microscopeGrp, \
-                                                            "customName", settingMenu.customName.text()))
-        
+        self.update_groupbox_name(
+            microscopeGrp, customName
+        )  # Update GroupBox name
+        # Name) If custom name is changed, change the groupBox name.
+        settingMenu.customName.textChanged.connect(
+            lambda: self.update_groupbox_name(
+                microscopeGrp, settingMenu.customName.text()
+            )
+        )
+        settingMenu.customName.textChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "customName", settingMenu.customName.text()
+            )
+        )
+
         # Exposure
-        settingMenu.expSlider.valueChanged.connect(lambda: screen.set_camera_setting(setting = "exposure",\
-                                                                val = settingMenu.expSlider.value()*1000))
-        settingMenu.expSlider.valueChanged.connect(lambda: settingMenu.expNum.setNum(settingMenu.expSlider.value()))
-        settingMenu.expSlider.valueChanged.connect(lambda: self.user_setting.update_user_configs_settingMenu(microscopeGrp, \
-                            "exp", settingMenu.expSlider.value()))       
-        settingMenu.expAuto.clicked.connect(lambda: settingMenu.expSlider.setValue(\
-                            int(screen.get_camera_setting(setting = "exposure")/1000)))
+        settingMenu.expSlider.valueChanged.connect(
+            lambda: screen.set_camera_setting(
+                setting="exposure", val=settingMenu.expSlider.value() * 1000
+            )
+        )
+        settingMenu.expSlider.valueChanged.connect(
+            lambda: settingMenu.expNum.setNum(settingMenu.expSlider.value())
+        )
+        settingMenu.expSlider.valueChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "exp", settingMenu.expSlider.value()
+            )
+        )
+        settingMenu.expAuto.clicked.connect(
+            lambda: settingMenu.expSlider.setValue(
+                int(screen.get_camera_setting(setting="exposure") / 1000)
+            )
+        )
 
         # Gain
-        settingMenu.gainSlider.valueChanged.connect(lambda: screen.set_camera_setting(setting = "gain",\
-                                                                val = settingMenu.gainSlider.value()))
-        settingMenu.gainSlider.valueChanged.connect(lambda: settingMenu.gainNum.setNum(settingMenu.gainSlider.value()))
-        settingMenu.gainSlider.valueChanged.connect(lambda: self.user_setting.update_user_configs_settingMenu(microscopeGrp, \
-                            "gain", settingMenu.gainSlider.value()))
-        settingMenu.gainAuto.clicked.connect(lambda: settingMenu.gainSlider.setValue(\
-                            screen.get_camera_setting(setting = "gain")))
+        settingMenu.gainSlider.valueChanged.connect(
+            lambda: screen.set_camera_setting(
+                setting="gain", val=settingMenu.gainSlider.value()
+            )
+        )
+        settingMenu.gainSlider.valueChanged.connect(
+            lambda: settingMenu.gainNum.setNum(settingMenu.gainSlider.value())
+        )
+        settingMenu.gainSlider.valueChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "gain", settingMenu.gainSlider.value()
+            )
+        )
+        settingMenu.gainAuto.clicked.connect(
+            lambda: settingMenu.gainSlider.setValue(
+                screen.get_camera_setting(setting="gain")
+            )
+        )
 
         # Gamma
-        settingMenu.gammaSlider.valueChanged.connect(lambda: screen.set_camera_setting(setting = "gamma",\
-                                                                val = settingMenu.gammaSlider.value()/100))
-        settingMenu.gammaSlider.valueChanged.connect(lambda: settingMenu.gammaNum.setText(
-                            "{:.2f}".format(settingMenu.gammaSlider.value()/100)))
-        settingMenu.gammaSlider.valueChanged.connect(lambda: self.user_setting.update_user_configs_settingMenu(microscopeGrp, \
-                            "gamma", settingMenu.gammaSlider.value()))
-        settingMenu.gammaAuto.clicked.connect(lambda: settingMenu.gammaSlider.setEnabled(
-                            not settingMenu.gammaSlider.isEnabled()))
-        settingMenu.gammaAuto.clicked.connect(lambda: self.user_setting.update_user_configs_settingMenu(microscopeGrp, "gammaAuto", \
-                            settingMenu.gammaSlider.isEnabled()))
-                            
+        settingMenu.gammaSlider.valueChanged.connect(
+            lambda: screen.set_camera_setting(
+                setting="gamma", val=settingMenu.gammaSlider.value() / 100
+            )
+        )
+        settingMenu.gammaSlider.valueChanged.connect(
+            lambda: settingMenu.gammaNum.setText(
+                "{:.2f}".format(settingMenu.gammaSlider.value() / 100)
+            )
+        )
+        settingMenu.gammaSlider.valueChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "gamma", settingMenu.gammaSlider.value()
+            )
+        )
+        settingMenu.gammaAuto.clicked.connect(
+            lambda: settingMenu.gammaSlider.setEnabled(
+                not settingMenu.gammaSlider.isEnabled()
+            )
+        )
+        settingMenu.gammaAuto.clicked.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "gammaAuto", settingMenu.gammaSlider.isEnabled()
+            )
+        )
+
         # W/B
         settingLayout = settingMenu.layout()
         settingLayout.addWidget(settingMenu.wbAuto, 5, 1, 2, 1)
         # Blue Channel
-        settingMenu.wbSliderBlue.valueChanged.connect(lambda: screen.set_camera_setting(setting = "wbBlue",\
-                                                                val = settingMenu.wbSliderBlue.value()/100))
-        settingMenu.wbSliderBlue.valueChanged.connect(lambda: settingMenu.wbNumBlue.setText(\
-                        "{:.2f}".format(settingMenu.wbSliderBlue.value()/100)))
-        settingMenu.wbSliderBlue.valueChanged.connect(lambda: self.user_setting.update_user_configs_settingMenu(microscopeGrp, \
-                        "wbBlue", settingMenu.wbSliderBlue.value()))
-        settingMenu.wbAuto.clicked.connect(lambda: settingMenu.wbSliderBlue.setValue(\
-                        screen.get_camera_setting(setting = "wbBlue")*100))
-        
+        settingMenu.wbSliderBlue.valueChanged.connect(
+            lambda: screen.set_camera_setting(
+                setting="wbBlue", val=settingMenu.wbSliderBlue.value() / 100
+            )
+        )
+        settingMenu.wbSliderBlue.valueChanged.connect(
+            lambda: settingMenu.wbNumBlue.setText(
+                "{:.2f}".format(settingMenu.wbSliderBlue.value() / 100)
+            )
+        )
+        settingMenu.wbSliderBlue.valueChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "wbBlue", settingMenu.wbSliderBlue.value()
+            )
+        )
+        settingMenu.wbAuto.clicked.connect(
+            lambda: settingMenu.wbSliderBlue.setValue(
+                screen.get_camera_setting(setting="wbBlue") * 100
+            )
+        )
+
         # Red Channel
-        settingMenu.wbSliderRed.valueChanged.connect(lambda: screen.set_camera_setting(setting = "wbRed",\
-                                                                val = settingMenu.wbSliderRed.value()/100))
-        settingMenu.wbSliderRed.valueChanged.connect(lambda: settingMenu.wbNumRed.setText(\
-                        "{:.2f}".format(settingMenu.wbSliderRed.value()/100)))
-        settingMenu.wbSliderRed.valueChanged.connect(lambda: self.user_setting.update_user_configs_settingMenu(microscopeGrp, \
-                        "wbRed", settingMenu.wbSliderRed.value()))
-        settingMenu.wbAuto.clicked.connect(lambda: settingMenu.wbSliderRed.setValue(\
-                        screen.get_camera_setting(setting = "wbRed")*100))
-        
+        settingMenu.wbSliderRed.valueChanged.connect(
+            lambda: screen.set_camera_setting(
+                setting="wbRed", val=settingMenu.wbSliderRed.value() / 100
+            )
+        )
+        settingMenu.wbSliderRed.valueChanged.connect(
+            lambda: settingMenu.wbNumRed.setText(
+                "{:.2f}".format(settingMenu.wbSliderRed.value() / 100)
+            )
+        )
+        settingMenu.wbSliderRed.valueChanged.connect(
+            lambda: self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "wbRed", settingMenu.wbSliderRed.value()
+            )
+        )
+        settingMenu.wbAuto.clicked.connect(
+            lambda: settingMenu.wbSliderRed.setValue(
+                screen.get_camera_setting(setting="wbRed") * 100
+            )
+        )
+
     def update_screen(self, screen, screen_index, selected_sn):
         """
         Update the screen with a new camera based on the selected serial number.
 
         This method manages the update of the camera associated with a specific microscope screen. It takes into
         account the current state of the application, i.e., whether acquisition is ongoing or not, and performs
         the necessary actions to update the camera and manage acquisition accordingly.
 
         Parameters:
         - screen (ScreenWidget): The screen widget associated with the microscope.
         - screen_index (int): The index of the screen in the list of all microscope screens.
         - selected_sn (str): The serial number of the camera selected to be associated with the microscope.
         """
         # Camera lists that currently attached on the model.
-        camera_list = {camera.name(sn_only=True): camera for camera in self.model.cameras}
+        camera_list = {
+            camera.name(sn_only=True): camera for camera in self.model.cameras
+        }
 
         # Get the prev camera lists displaying on the screen
         prev_camera, curr_camera = screen.get_camera_name(), selected_sn
-        prev_lists = [screen.get_camera_name() for screen in self.screen_widgets if screen.get_camera_name()]
-        if 0 <= screen_index < len(prev_lists):  # Ensure screen_index is within valid range
+        prev_lists = [
+            screen.get_camera_name()
+            for screen in self.screen_widgets
+            if screen.get_camera_name()
+        ]
+        if (
+            0 <= screen_index < len(prev_lists)
+        ):  # Ensure screen_index is within valid range
             curr_list = prev_lists[:]
             curr_list.pop(screen_index)
             curr_list.insert(screen_index, curr_camera)
         else:
             logger.error(f"Invalid screen index: {screen_index}")
-        logger.debug(f"prev_list: {prev_lists}")    
+        logger.debug(f"prev_list: {prev_lists}")
         logger.debug(f"curr_list: {curr_list}")
 
         # Handle updates based on the current state of the application
-        if self.startButton.isChecked():        # If the 'Start' button is enabled (continuous acquisition mode)
+        if (
+            self.startButton.isChecked()
+        ):  # If the 'Start' button is enabled (continuous acquisition mode)
             if set(prev_lists) == set(curr_list):
                 # If the list of cameras hasn't changed, just update the current screen's camera
                 screen.set_camera(camera_list.get(curr_camera))
             else:
                 if prev_camera not in curr_list:
                     # If the previous camera has been removed from the list, stop its acquisition
                     screen.stop_acquisition_camera()
@@ -487,15 +618,15 @@
         This method is used to update the visual representation of a microscope based on a custom name provided
         by the user.
 
         Parameters:
         - microscopeGrp (QGroupBox): The group box representing the microscope.
         - customName (str): The custom name to set as the title and object name of the group box.
         """
-        if customName: 
+        if customName:
             microscopeGrp.setTitle(customName)
             microscopeGrp.setObjectName(customName)
 
     def show_settings_menu(self, settingButton, is_checked):
         """
         Show or hide the settings menu associated with a microscope group box.
 
@@ -507,113 +638,138 @@
         Parameters:
         - settingButton (QToolButton): The settings button associated with the microscope group box.
         - is_checked (bool): Indicates whether the settings button is checked (True) or unchecked (False).
         """
         microscopeGrp = settingButton.parent()
         # Find the settingMenu within this microscopeGrp
         settingMenu = microscopeGrp.findChild(QWidget, "SettingsMenu")
-        self.settings_refresh_timer.timeout.connect(partial(self.update_setting_menu, microscopeGrp))
+        self.settings_refresh_timer.timeout.connect(
+            partial(self.update_setting_menu, microscopeGrp)
+        )
 
         if is_checked:
-            # If the settings button is checked, start the settings refresh timer and show the settings menu
-            self.settings_refresh_timer.start(100)      # update setting menu every 0.1 sec
+            # If the settings button is checked, start the settings refresh 
+            # timer and show the settings menu
+            # update setting menu every 0.1 sec
+            self.settings_refresh_timer.start(100)      
             
+
             # Show the setting menu next to setting button
             button_position = settingButton.mapToGlobal(settingButton.pos())
             menu_x = button_position.x() + settingButton.width()
             menu_x = menu_x - microscopeGrp.mapToGlobal(QPoint(0, 0)).x()
-            menu_y = settingButton.y() + settingButton.height() - settingMenu.height()
-            logger.debug(f"(SettingMenu) coordinates of setting menu: x: {menu_x}, y: {menu_y}")
+            menu_y = (
+                settingButton.y()
+                + settingButton.height()
+                - settingMenu.height()
+            )
+            logger.debug(
+                f"(SettingMenu) coordinates of setting menu: x: {menu_x}, y: {menu_y}"
+            )
             settingMenu.move(menu_x, menu_y)
             settingMenu.show()
         else:
-            # If the settings button is unchecked, stop the settings refresh timer and hide the settings menu
+            # If the settings button is unchecked, stop the settings 
+            # refresh timer and hide the settings menu
             self.settings_refresh_timer.stop()
             settingMenu.hide()
 
     def update_setting_menu(self, microscopeGrp):
         """
         Update the values displayed in the settings menu based on the current camera settings.
 
         This method is called periodically by a QTimer to refresh the values displayed in the
         settings menu, ensuring they are up-to-date with the current settings of the camera.
 
         Parameters:
         - microscopeGrp (QGroupBox): The microscope group box associated with the settings menu to be updated.
         """
-        
+
         # Find the settingMenu within this microscopeGrp
         settingMenu = microscopeGrp.findChild(QWidget, "SettingsMenu")
         screen = microscopeGrp.findChild(ScreenWidget, "Screen")
 
-        # Display the S/N of camera 
+        # Display the S/N of camera
         sn = screen.get_camera_name()
         # Load the saved settings
         saved_settings = self.user_setting.load_settings_item(sn)
         if saved_settings:
             # If saved settings are found, update the sliders in the settings menu with the saved values
-            settingMenu.expSlider.setValue(saved_settings.get('exp', 15))
-            settingMenu.gainSlider.setValue(saved_settings.get('gain', 20))
+            settingMenu.expSlider.setValue(saved_settings.get("exp", 15))
+            settingMenu.gainSlider.setValue(saved_settings.get("gain", 20))
 
             # Gamma
-            gammaAuto = saved_settings.get('gammaAuto', None)
+            gammaAuto = saved_settings.get("gammaAuto", None)
             if gammaAuto == True:
                 settingMenu.gammaSlider.setEnabled(True)
-                settingMenu.gammaSlider.setValue(saved_settings.get('gamma', 100))
+                settingMenu.gammaSlider.setValue(
+                    saved_settings.get("gamma", 100)
+                )
             elif gammaAuto == False:
                 settingMenu.gammaSlider.setEnabled(False)
             else:
                 pass
 
             # W/B
             if screen.get_camera_color_type() == "Color":
                 settingMenu.wbAuto.setDisabled(False)
                 settingMenu.wbSliderRed.setDisabled(False)
                 settingMenu.wbSliderBlue.setDisabled(False)
-                settingMenu.wbSliderRed.setValue(saved_settings.get('wbRed', 1.2))
-                settingMenu.wbSliderBlue.setValue(saved_settings.get('wbBlue', 2.8))
+                settingMenu.wbSliderRed.setValue(
+                    saved_settings.get("wbRed", 1.2)
+                )
+                settingMenu.wbSliderBlue.setValue(
+                    saved_settings.get("wbBlue", 2.8)
+                )
             elif screen.get_camera_color_type() == "Mono":
                 settingMenu.wbAuto.setDisabled(True)
                 settingMenu.wbSliderRed.setDisabled(True)
                 settingMenu.wbSliderBlue.setDisabled(True)
                 settingMenu.wbNumRed.setText("--")
                 settingMenu.wbNumBlue.setText("--")
 
-        else: 
+        else:
             settingMenu.gainAuto.click()
             settingMenu.wbAuto.click()
             settingMenu.expAuto.click()
-            self.user_setting.update_user_configs_settingMenu(microscopeGrp, "gammaAuto", True)
-            self.user_setting.update_user_configs_settingMenu(microscopeGrp, "gamma", settingMenu.gammaSlider.value())
-            
+            self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "gammaAuto", True
+            )
+            self.user_setting.update_user_configs_settingMenu(
+                microscopeGrp, "gamma", settingMenu.gammaSlider.value()
+            )
+
     def dir_setting_handler(self):
         """
         This method handles the selection of a directory for saving files. It opens a dialog that allows
         the user to browse their filesystem and select a directory. The selected directory's path is then
         displayed on the user interface.
 
         This is a crucial function for users who need to save data or configurations, as it provides a
         simple and intuitive way to specify the location where files should be saved.
         """
         # Fetch the default documents directory path
-        documents_dir = QStandardPaths.writableLocation(QStandardPaths.DocumentsLocation)
+        documents_dir = QStandardPaths.writableLocation(
+            QStandardPaths.DocumentsLocation
+        )
         # Open a dialog to allow the user to select a directory
-        directory = QFileDialog.getExistingDirectory(self, "Select Directory", documents_dir)
+        directory = QFileDialog.getExistingDirectory(
+            self, "Select Directory", documents_dir
+        )
         # If a directory is chosen, update the label to display the chosen path
         if directory:
             self.dirLabel.setText(directory)
-        
+
     def save_user_configs(self):
         """
         Saves user configuration settings to a persistent storage.
 
         This method retrieves current configuration values from the UI, including
         the number of columns (nColumn), directory path (directory), and the window's
         width and height. It then passes these values to the `save_user_configs` method
         of the `user_setting` object to be saved.
         """
         nColumn = self.nColumnsSpinBox.value()
         directory = self.dirLabel.text()
         width = self.width()
         height = self.height()
         self.user_setting.save_user_configs(nColumn, directory, width, height)
-
```

### Comparing `parallax_app-0.37.0/parallax/mask_generator.py` & `parallax_app-0.37.1/parallax/mask_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,115 +1,131 @@
 """
-MaskGenerator: Generates a mask from an input image using various image processing techniques.
+MaskGenerator: Generates a mask from an input image 
+using various image processing techniques.
 """
+
+import logging
+
 import cv2
 import numpy as np
-import logging
 
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+# Set the logging level for PyQt5.uic.uiparser/properties.
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class MaskGenerator:
     """Class for generating a mask from an image."""
+
     def __init__(self):
-        """ Initialize mask generator object """
+        """Initialize mask generator object"""
         self.img = None
         self.original_size = (None, None)
-        self.is_reticle_exist = True #TODO
+        self.is_reticle_exist = True  # TODO
 
     def _resize_and_blur(self):
         """Resize and blur the image."""
         if len(self.img.shape) > 2:
             self.img = cv2.cvtColor(self.img, cv2.COLOR_BGR2GRAY)
         self.img = cv2.resize(self.img, (400, 300))
         self.img = cv2.GaussianBlur(self.img, (9, 9), 0)
 
     def _apply_threshold(self):
         """Apply binary threshold to the image."""
-        _, self.img = cv2.threshold(self.img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
+        _, self.img = cv2.threshold(
+            self.img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU
+        )
 
     def _keep_largest_contour(self):
         """Keep the largest contour in the image."""
-        contours, _ = cv2.findContours(self.img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+        contours, _ = cv2.findContours(
+            self.img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
         if len(contours) >= 2:
             largest_contour = max(contours, key=cv2.contourArea)
             for contour in contours:
                 if contour is not largest_contour:
-                    self.img = cv2.drawContours(self.img, [contour], -1, (0, 0, 0), -1)
+                    self.img = cv2.drawContours(
+                        self.img, [contour], -1, (0, 0, 0), -1
+                    )
 
     def _apply_morphological_operations(self):
         """Apply morphological operations to the image."""
         kernels = [cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (8, 8)),
                    cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (10, 10))]
         
         self.img = cv2.morphologyEx(self.img, cv2.MORPH_CLOSE, kernels[0])
         self.img = cv2.erode(self.img, kernels[1], iterations=1)
-        
-        self.img = cv2.bitwise_not(self.img)  # Invert image to prepare for dilate and final operations
+
+        # Invert image to prepare for dilate and final operations
+        self.img = cv2.bitwise_not(self.img)
         self._remove_small_contours()
         self.img = cv2.dilate(self.img, kernels[1], iterations=1)
         self.img = cv2.bitwise_not(self.img)  # Re-invert image back
 
     def _remove_small_contours(self):
         """Remove small contours from the image."""
-        contours, _ = cv2.findContours(self.img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+        contours, _ = cv2.findContours(
+            self.img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
         for contour in contours:
             if cv2.contourArea(contour) < 50 * 50:
-                self.img = cv2.drawContours(self.img, [contour], -1, (0, 0, 0), -1)
+                self.img = cv2.drawContours(
+                    self.img, [contour], -1, (0, 0, 0), -1
+                )
 
     def _finalize_image(self):
         """Resize the image back to its original size."""
         self.img = cv2.resize(self.img, self.original_size)
         self.img = cv2.convertScaleAbs(self.img)
 
     def _is_reticle_frame(self):
         """Check if the image contains a reticle frame.
-        
+
         Returns:
             bool: True if the image contains a reticle frame, False otherwise.
         """
         img = cv2.normalize(self.img, None, 0, 255, cv2.NORM_MINMAX)
         img = img.astype(np.uint8)
-        
+
         hist = cv2.calcHist([img], [0], None, [255], [0, 255])
-        hist = cv2.GaussianBlur(hist, (91,91), 0)
-        hist_smoothed = hist.squeeze() 
+        hist = cv2.GaussianBlur(hist, (91, 91), 0)
+        hist_smoothed = hist.squeeze()
         peaks = np.where((hist_smoothed[:-2] < hist_smoothed[1:-1]) & 
                     (hist_smoothed[1:-1] > hist_smoothed[2:]) & 
                     (hist_smoothed[1:-1] > 300))[0] + 1
 
         self.is_reticle_exist = True if len(peaks) >= 2 else False
         logger.debug(f"is_reticle_exist: {self.is_reticle_exist}")
         return self.is_reticle_exist
-    
+
     def process(self, img):
         """Process the input image and generate a mask.
-        
+
         Args:
             img (numpy.ndarray): Input image.
-            
+
         Returns:
             numpy.ndarray: Generated mask image.
         """
         if img is None:
             logger.debug("Input image of ReticleFrameDetection is None.")
             return None
-        
+
         # Convert image to grayscale if it is not already
         if len(img.shape) == 3 and img.shape[2] == 3:
             img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
 
         self.img = img
         self.original_size = img.shape[1], img.shape[0]
         self._resize_and_blur()
         if self.is_reticle_exist is None:
             self._is_reticle_frame()
         self._apply_threshold()
         self._keep_largest_contour()
         self._apply_morphological_operations()
-        self._finalize_image()   # Resize to oiginal size
+        self._finalize_image()  # Resize to original size
 
         return self.img
```

### Comparing `parallax_app-0.37.0/parallax/model.py` & `parallax_app-0.37.1/parallax/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,62 @@
 """
 The Model class is the core component for managing cameras, stages, and calibration data.
 """
-from PyQt5.QtCore import pyqtSignal
+
 from PyQt5.QtCore import QObject, pyqtSignal
-from .camera import list_cameras, close_cameras, MockCamera, PySpinCamera
-from .stage_listener import StageInfo, Stage
+
+from .camera import MockCamera, PySpinCamera, close_cameras, list_cameras
+from .stage_listener import Stage, StageInfo
+
 
 class Model(QObject):
     """Model class to handle cameras, stages, and calibration data."""
+
     msg_posted = pyqtSignal(str)
     accutest_point_reached = pyqtSignal()
 
     def __init__(self, version="V1"):
-        """ Initialize model object """
+        """Initialize model object"""
         QObject.__init__(self)
         self.version = version
         # camera
         self.cameras = []
         self.cameras_sn = []
         self.nPySpinCameras = 0
         self.nMockCameras = 0
         self.focos = []
 
         # stage
         self.nStages = 0
         self.init_stages()
         self.elevators = {}
-        self.stage_listener_url = 'http://localhost:8080/'
+        self.stage_listener_url = "http://localhost:8080/"
 
         # probe detector
         self.probeDetectors = []
 
         # coords axis
         self.coords_axis = {}
-        
         self.camera_intrinsic = {}
         self.camera_extrinsic = {}
         self.calibration = None
         self.calibrations = {}
-    
+
         self.cal_in_progress = False
         self.accutest_in_progress = False
         self.lcorr, self.rcorr = False, False
-        
+
         self.img_point_last = None
         self.obj_point_last = None
         self.transforms = {}
 
-    @property
-    def ncameras(self):
-        """Get the number of cameras."""
-        return len(self.cameras)
-
     def set_last_object_point(self, obj_point):
         """Set the last object point."""
         self.obj_point_last = obj_point
 
-    def set_last_image_point(self, lcorr, rcorr):
-        """Set the last image point."""
-        self.img_point_last = (lcorr + rcorr)
-
     def add_calibration(self, cal):
         """Add a calibration."""
         self.calibrations[cal.name] = cal
 
     def set_calibration(self, calibration):
         """Set the calibration."""
         self.calibration = calibration
@@ -95,33 +88,49 @@
     def add_mock_cameras(self, n=1):
         """Add mock cameras."""
         for i in range(n):
             self.cameras.append(MockCamera())
 
     def scan_for_cameras(self):
         """Scan for cameras."""
-        self.cameras = list_cameras(version = self.version) + self.cameras
+        self.cameras = list_cameras(version=self.version) + self.cameras
         self.cameras_sn = [camera.name(sn_only=True) for camera in self.cameras]
-        self.nMockCameras = len([camera for camera in self.cameras if isinstance(camera, MockCamera)])
-        self.nPySpinCameras = len([camera for camera in self.cameras if isinstance(camera, PySpinCamera)])
+        self.nMockCameras = len(
+            [
+                camera
+                for camera in self.cameras
+                if isinstance(camera, MockCamera)
+            ]
+        )
+        self.nPySpinCameras = len(
+            [
+                camera
+                for camera in self.cameras
+                if isinstance(camera, PySpinCamera)
+            ]
+        )
 
     def scan_for_usb_stages(self):
         """Scan for USB stages."""
         stage_info = StageInfo(self.stage_listener_url)
         instances = stage_info.get_instances()
         self.init_stages()
         for instance in instances:
-            stage = Stage(stage_info = instance)
+            stage = Stage(stage_info=instance)
             self.add_stage(stage)
         self.nStages = len(self.stages)
 
     def add_stage(self, stage):
         """Add a stage."""
         self.stages[stage.sn] = stage
 
+    def get_stage(self, stage_sn):
+        """Get a stage."""
+        return self.stages.get(stage_sn)
+
     def add_probe_detector(self, probeDetector):
         """Add a probe detector."""
         self.probeDetectors.append(probeDetector)
 
     def add_coords_axis(self, camera_name, coords):
         """Add coordinates axis."""
         self.coords_axis[camera_name] = coords
@@ -133,30 +142,27 @@
     def add_camera_intrinsic(self, camera_name, mtx, dist):
         """Add camera intrinsic parameters."""
         self.camera_intrinsic[camera_name] = [mtx, dist]
 
     def get_camera_intrinsic(self, camera_name):
         """Get camera intrinsic parameters."""
         return self.camera_intrinsic.get(camera_name)
-    
+
     def add_camera_extrinsic(self, name1, name2, retVal, R, T, E, F):
         """Add camera extrinsic parameters."""
-        self.camera_extrinsic[name1+"-"+name2] = [retVal, R, T, E, F]
+        self.camera_extrinsic[name1 + "-" + name2] = [retVal, R, T, E, F]
 
     def get_camera_extrinsic(self, name1, name2):
         """Get camera extrinsic parameters."""
-        return self.camera_extrinsic.get(name1+"-"+name2)
-    
+        return self.camera_extrinsic.get(name1 + "-" + name2)
+
     def clean(self):
         """Clean up."""
         close_cameras()
 
     def save_all_camera_frames(self):
         """Save all camera frames."""
-        for i,camera in enumerate(self.cameras):
+        for i, camera in enumerate(self.cameras):
             if camera.last_image:
                 filename = 'camera%d_%s.png' % (i, camera.get_last_capture_time())
                 camera.save_last_image(filename)
-                self.msg_log.post('Saved camera frame: %s' % filename)
-
-
-
+                self.msg_log.post("Saved camera frame: %s" % filename)
```

### Comparing `parallax_app-0.37.0/parallax/no_filter.py` & `parallax_app-0.37.1/parallax/no_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 """
 NoFilter serves as a pass-through component in a frame processing pipeline, 
 employing a worker-thread model to asynchronously handle frames without modification, 
 facilitating integration and optional processing steps.
 """
-from PyQt5.QtCore import pyqtSignal, QObject, QThread
+
 import time
 
+from PyQt5.QtCore import QObject, QThread, pyqtSignal
+
+
 class NoFilter(QObject):
     """Class representing no filter."""
+
     name = "None"
     frame_processed = pyqtSignal(object)
 
     class Worker(QObject):
         """Worker class for processing frames in a separate thread."""
+
         finished = pyqtSignal()
         frame_processed = pyqtSignal(object)
 
         def __init__(self, name):
             """Initialize the worker object."""
             QObject.__init__(self)
             self.name = name
             self.running = True
             self.new = False
 
         def update_frame(self, frame):
             """Update the frame to be processed.
-        
+
             Args:
                 frame: The frame to be processed.
             """
             self.frame = frame
             self.new = True
 
         def process(self, frame):
@@ -65,42 +70,42 @@
         self.init_thread()
 
     def init_thread(self):
         """Initialize or reinitialize the worker and thread"""
         self.thread = QThread()
         self.worker = self.Worker(self.name)
         self.worker.moveToThread(self.thread)
-        
+
         self.thread.started.connect(self.worker.run)
         self.worker.frame_processed.connect(self.frame_processed.emit)
         self.worker.finished.connect(self.thread.quit)
         self.worker.finished.connect(lambda: self.thread_deleted)
         self.worker.finished.connect(self.worker.deleteLater)
         self.thread.finished.connect(self.thread.deleteLater)
-        
+
         self.thread.start()
 
     def process(self, frame):
         """Process the frame using the worker.
-    
+
         Args:
             frame: The frame to be processed.
         """
         if self.worker is not None:
             self.worker.update_frame(frame)
 
     def start(self):
         """Start the filter by reinitializing and starting the worker and thread."""
         self.init_thread()  # Reinitialize and start the worker and thread
 
     def stop(self):
         """Stop the filter by stopping the worker."""
         if self.worker is not None:
             self.worker.stop_running()
-    
+
     def clean(self):
         """Clean up the filter by stopping the worker and waiting for the thread to finish."""
         if self.worker is not None:
             self.worker.stop_running()
         if self.thread is not None:
             self.thread.quit()
             self.thread.wait()
```

### Comparing `parallax_app-0.37.0/parallax/probe_calibration.py` & `parallax_app-0.37.1/parallax/probe_calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,174 +1,209 @@
 """
 ProbeCalibration transforms probe coordinates from local to global space"
 - local space: Stage coordinates
 - global space: Reticle coordinates
 """
-from PyQt5.QtCore import QObject, pyqtSignal
-from sklearn.linear_model import LinearRegression
+
+import csv
 import logging
+import os
+
 import numpy as np
 import pandas as pd
-import csv
-import os
+from PyQt5.QtCore import QObject, pyqtSignal
+from sklearn.linear_model import LinearRegression
 
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class ProbeCalibration(QObject):
     """
     Handles the transformation of probe coordinates from local (stage) to global (reticle) space.
 
     Attributes:
         calib_complete_x (pyqtSignal): Signal emitted when calibration in the X direction is complete.
         calib_complete_y (pyqtSignal): Signal emitted when calibration in the Y direction is complete.
         calib_complete_z (pyqtSignal): Signal emitted when calibration in the Z direction is complete.
         calib_complete (pyqtSignal): General signal emitted when calibration is fully complete.
 
     Args:
         stage_listener (QObject): The stage listener object that emits signals related to stage movements.
     """
+
     calib_complete_x = pyqtSignal()
     calib_complete_y = pyqtSignal()
     calib_complete_z = pyqtSignal()
     calib_complete = pyqtSignal(str, object)
     transM_info = pyqtSignal(object, float, object)
 
     """Class for probe calibration."""
+
     def __init__(self, stage_listener):
         """
         Initializes the ProbeCalibration object with a given stage listener.
         """
         super().__init__()
         self.stage_listener = stage_listener
         self.stage_listener.probeCalibRequest.connect(self.update)
         self.stages = {}
         self.df = None
         self.inliers = []
         self.stage = None
-        self.threshold_min_max = 2000 #TODO 
+        self.threshold_min_max = 2000  # TODO
         self.model_LR, self.transM_LR, self.transM_LR_prev = None, None, None
-        self.threshold_matrix = np.array([[0.00002, 0.00002, 0.00002, 50.0], #TODO
-                                            [0.00002, 0.00002, 0.00002, 50.0],
-                                            [0.00002, 0.00002, 0.00002, 50.0],
-                                            [0.0, 0.0, 0.0, 0.0]])
-        self.LR_err_L2_threshold = 20 #TODO
+        self.threshold_matrix = np.array(
+            [
+                [0.00002, 0.00002, 0.00002, 50.0],  # TODO
+                [0.00002, 0.00002, 0.00002, 50.0],
+                [0.00002, 0.00002, 0.00002, 50.0],
+                [0.0, 0.0, 0.0, 0.0],
+            ]
+        )
+        self.LR_err_L2_threshold = 20  # TODO
         self._create_file()
-    
+
         # Test signal
         self.reset_calib()
 
     def reset_calib(self):
         """
         Resets calibration to its initial state, clearing any stored min and max values.
         """
-        self.min_x, self.max_x = float('inf'), float('-inf')
-        self.min_y, self.max_y = float('inf'), float('-inf')
-        self.min_z, self.max_z = float('inf'), float('-inf')
-        self.transM_LR_prev = np.zeros((4,4), dtype=np.float64)
-        self.signal_emitted_x, self.signal_emitted_y, self.signal_emitted_z = False, False, False
+        self.min_x, self.max_x = float("inf"), float("-inf")
+        self.min_y, self.max_y = float("inf"), float("-inf")
+        self.min_z, self.max_z = float("inf"), float("-inf")
+        self.transM_LR_prev = np.zeros((4, 4), dtype=np.float64)
+        self.signal_emitted_x = False
+        self.signal_emitted_y = False
+        self.signal_emitted_z = False
 
     def _create_file(self):
         """
         Creates or clears the CSV file used to store local and global points during calibration.
         """
         package_dir = os.path.dirname(os.path.abspath(__file__))
-        debug_dir = os.path.join(os.path.dirname(package_dir), 'debug')
+        debug_dir = os.path.join(os.path.dirname(package_dir), "debug")
         os.makedirs(debug_dir, exist_ok=True)
-        self.csv_file = os.path.join(debug_dir, 'points.csv')
+        self.csv_file = os.path.join(debug_dir, "points.csv")
 
         # Check if the file exists and remove it if it does
         if os.path.exists(self.csv_file):
             os.remove(self.csv_file)
 
         # Create a new file and write column names
-        with open(self.csv_file, 'w', newline='') as file:
+        with open(self.csv_file, "w", newline="") as file:
             writer = csv.writer(file)
             # Define column names
-            column_names = ['local_x', 'local_y', 'local_z', 'global_x', 'global_y', 'global_z']
+            column_names = [
+                "local_x",
+                "local_y",
+                "local_z",
+                "global_x",
+                "global_y",
+                "global_z",
+            ]
             writer.writerow(column_names)
 
     def clear(self):
         """
         Clears all stored data and resets the transformation matrix to its default state.
         """
         self._create_file()
         self.model_LR, self.transM_LR, self.transM_LR_prev = None, None, None
-    
+
     def _get_local_global_points(self):
         """
         Retrieves local and global points from the CSV file as numpy arrays.
 
         Returns:
             tuple: A tuple containing arrays of local points and global points.
         """
         self.df = pd.read_csv(self.csv_file)
         # Extract local and global points
-        local_points = self.df[['local_x', 'local_y', 'local_z']].values
-        global_points = self.df[['global_x', 'global_y', 'global_z']].values
+        local_points = self.df[["local_x", "local_y", "local_z"]].values
+        global_points = self.df[["global_x", "global_y", "global_z"]].values
         return local_points, global_points
 
     def _get_transM_LR(self, local_points, global_points):
         """
         Computes the transformation matrix from local to global coordinates.
 
         Args:
             local_points (np.array): Array of local points.
             global_points (np.array): Array of global points.
 
         Returns:
             tuple: Linear regression model and transformation matrix.
         """
-        local_points_with_bias = np.hstack([local_points, np.ones((local_points.shape[0], 1))])
+        local_points_with_bias = np.hstack(
+            [local_points, np.ones((local_points.shape[0], 1))]
+        )
 
         # Train the linear regression model
-        model = LinearRegression(fit_intercept=False) 
+        model = LinearRegression(fit_intercept=False)
         model.fit(local_points_with_bias, global_points)
 
         # Weights and Bias
-        weights = model.coef_[:, :-1] # All but last column, which are the weights
+        # All but last column, which are the weights
+        weights = model.coef_[:, :-1]
         bias = model.coef_[:, -1] # Last column, which is the bias
 
         # Combine weights and bias to form the transformation matrix
         transformation_matrix = np.hstack([weights, bias.reshape(-1, 1)])
         # Adding the extra row to complete the affine transformation matrix
         transformation_matrix = np.vstack([transformation_matrix, [0, 0, 0, 1]])
-        
+
         return model, transformation_matrix
 
     def _update_local_global_point(self):
         """
         Updates the CSV file with a new set of local and global points from the current stage position.
         """
-        with open(self.csv_file, 'a', newline='') as file:
+        with open(self.csv_file, "a", newline="") as file:
             writer = csv.writer(file)
-            writer.writerow([self.stage.stage_x, self.stage.stage_y, self.stage.stage_z, 
-                             self.stage.stage_x_global, self.stage.stage_y_global, self.stage.stage_z_global])
+            writer.writerow(
+                [
+                    self.stage.stage_x,
+                    self.stage.stage_y,
+                    self.stage.stage_z,
+                    self.stage.stage_x_global,
+                    self.stage.stage_y_global,
+                    self.stage.stage_z_global,
+                ]
+            )
 
     def _is_criteria_met_transM(self):
         """
         Checks if the transformation matrix has stabilized within certain thresholds.
 
         Returns:
             bool: True if the criteria are met, otherwise False.
         """
         diff_matrix = np.abs(self.transM_LR - self.transM_LR_prev)
-        if np.all(diff_matrix <= self.threshold_matrix): 
+        if np.all(diff_matrix <= self.threshold_matrix):
             return True
         else:
             return False
 
     def _update_min_max_x_y_z(self):
-        self.min_x, self.max_x = min(self.min_x, self.stage.stage_x), max(self.max_x, self.stage.stage_x)
-        self.min_y, self.max_y = min(self.min_y, self.stage.stage_y), max(self.max_y, self.stage.stage_y)
-        self.min_z, self.max_z = min(self.min_z, self.stage.stage_z), max(self.max_z, self.stage.stage_z)
+        self.min_x, self.max_x = min(self.min_x, self.stage.stage_x), max(
+            self.max_x, self.stage.stage_x
+        )
+        self.min_y, self.max_y = min(self.min_y, self.stage.stage_y), max(
+            self.max_y, self.stage.stage_y
+        )
+        self.min_z, self.max_z = min(self.min_z, self.stage.stage_z), max(
+            self.max_z, self.stage.stage_z
+        )
 
     def _is_criteria_met_points_min_max(self):
         """
         Checks if the range of collected points in each direction exceeds minimum thresholds.
 
         Returns:
             bool: True if sufficient range is achieved, otherwise False.
@@ -189,21 +224,29 @@
     def _apply_transformation(self):
         """
         Applies the calculated transformation matrix to convert a local point to global coordinates.
 
         Returns:
             np.array: The transformed global point.
         """
-        local_point = np.array([self.stage.stage_x, self.stage.stage_y, self.stage.stage_z, 1])
+        local_point = np.array(
+            [self.stage.stage_x, self.stage.stage_y, self.stage.stage_z, 1]
+        )
         global_point = np.dot(self.transM_LR, local_point)
         return global_point[:3]
 
     def _l2_error_current_point(self):
         transformed_point = self._apply_transformation()
-        global_point = np.array([self.stage.stage_x_global, self.stage.stage_y_global, self.stage.stage_z_global])
+        global_point = np.array(
+            [
+                self.stage.stage_x_global,
+                self.stage.stage_y_global,
+                self.stage.stage_z_global,
+            ]
+        )
         LR_err_L2 = np.linalg.norm(transformed_point - global_point)
 
         return LR_err_L2
 
     def _is_criteria_met_l2_error(self):
         """
         Evaluates if the L2 error between the transformed point and the actual global point is within threshold.
@@ -216,83 +259,94 @@
         else:
             return False
 
     def _enough_points_emit_signal(self):
         """
         Emits calibration complete signals based on the sufficiency of point ranges in each direction.
         """
-        if not self.signal_emitted_x and self.max_x - self.min_x > self.threshold_min_max:
+        if (
+            not self.signal_emitted_x
+            and self.max_x - self.min_x > self.threshold_min_max
+        ):
             self.calib_complete_x.emit()
             self.signal_emitted_x = True
-        if not self.signal_emitted_y and self.max_y - self.min_y > self.threshold_min_max:
+        if (
+            not self.signal_emitted_y
+            and self.max_y - self.min_y > self.threshold_min_max
+        ):
             self.calib_complete_y.emit()
             self.signal_emitted_y = True
-        if not self.signal_emitted_z and self.max_z - self.min_z > self.threshold_min_max:
+        if (
+            not self.signal_emitted_z
+            and self.max_z - self.min_z > self.threshold_min_max
+        ):
             self.calib_complete_z.emit()
             self.signal_emitted_z = True
 
     def _is_enough_points(self):
         """Check if there are enough points for calibration.
-        
+
         Returns:
             bool: True if there are enough points, False otherwise.
-        """ 
-        # End Criteria: 
+        """
+        # End Criteria:
         # 1. distance maxX-minX, maxY-minY, maxZ-minZ
         # 2. transM_LR difference in some epsilon value
         # 3. L2 error (Global and Exp) is less than some values (e.g. 20 mincrons)
         if self._is_criteria_met_points_min_max():
             if self._is_criteria_met_transM():
                 if self._is_criteria_met_l2_error():
                     logger.debug("Enough points gathered.")
                     return True
 
         self.transM_LR_prev = self.transM_LR
         return False
-    
+
     def _update_info_ui(self):
         x_diff = self.max_x - self.min_x
         y_diff = self.max_y - self.min_y
         z_diff = self.max_z - self.min_z
-        self.transM_info.emit(self.transM_LR, self.LR_err_L2_current, np.array([x_diff, y_diff, z_diff]))
+        self.transM_info.emit(
+            self.transM_LR,
+            self.LR_err_L2_current,
+            np.array([x_diff, y_diff, z_diff]),
+        )
 
     def update(self, stage):
         """
         Main method to update calibration with a new stage position and check if calibration is complete.
 
         Args:
             stage (Stage): The current stage object with new position data.
         """
         # update points in the file
         self.stage = stage
         self._update_local_global_point()
         # get whole list of local and global points in pd format
         local_points, global_points = self._get_local_global_points()
-        self.model_LR, self.transM_LR = self._get_transM_LR(local_points, global_points)
-        self.LR_err_L2_current = self._l2_error_current_point() 
-        self._update_min_max_x_y_z()  # update min max x,y,z 
+        self.model_LR, self.transM_LR = self._get_transM_LR(
+            local_points, global_points
+        )
+        self.LR_err_L2_current = self._l2_error_current_point()
+        self._update_min_max_x_y_z()  # update min max x,y,z
 
         # update transformation matrix and overall LR in UI
         self._update_info_ui()
 
         # if ret, send the signal
         ret = self._is_enough_points()
         if ret:
-            self.calib_complete.emit(self.stage.sn , self.transM_LR)
-            logger.debug(f"complete probe calibration {self.stage.sn}, {self.transM_LR}")
-    
+            self.calib_complete.emit(self.stage.sn, self.transM_LR)
+            logger.debug(
+                f"complete probe calibration {self.stage.sn}, {self.transM_LR}"
+            )
+
     def reshape_array(self):
         """
         Reshapes arrays of local and global points for processing.
 
         Returns:
             tuple: Reshaped local and global points arrays.
         """
         local_points = np.array(self.local_points)
         global_points = np.array(self.global_points)
         return local_points.reshape(-1, 1, 3), global_points.reshape(-1, 1, 3)
-    
-
-
-
-
-
```

### Comparing `parallax_app-0.37.0/parallax/probe_detect_manager.py` & `parallax_app-0.37.1/parallax/probe_detect_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,138 +1,182 @@
 """
 ProbeDetectManager coordinates probe detection in images, leveraging PyQt threading 
 and signals for real-time processing. It handles frame updates, detection, 
 and result communication, utilizing components like MaskGenerator and ProbeDetector.
 """
-from PyQt5.QtCore import pyqtSignal, QObject, QThread
+
+import logging
+import time
+
+import cv2
+import numpy as np
+from PyQt5.QtCore import QObject, QThread, pyqtSignal
+
+from .curr_bg_cmp_processor import CurrBgCmpProcessor
+from .curr_prev_cmp_processor import CurrPrevCmpProcessor
 from .mask_generator import MaskGenerator
-from .reticle_detection import ReticleDetection
 from .probe_detector import ProbeDetector
-from .curr_prev_cmp_processor import CurrPrevCmpProcessor
-from .curr_bg_cmp_processor import CurrBgCmpProcessor
-import cv2
-import time
-import logging
+from .reticle_detection import ReticleDetection
 
 # Set logger name
 logger = logging.getLogger(__name__)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class ProbeDetectManager(QObject):
     """Manager class for probe detection."""
+
     name = "None"
     frame_processed = pyqtSignal(object)
     found_coords = pyqtSignal(str, str, tuple, tuple)
 
     class Worker(QObject):
         """Worker class for probe detection."""
+
         finished = pyqtSignal()
         frame_processed = pyqtSignal(object)
         found_coords = pyqtSignal(str, str, tuple)
 
-        def __init__(self, name):
-            """ Initialize Worker object """
+        def __init__(self, name, model):
+            """Initialize Worker object"""
             QObject.__init__(self)
+            self.model = model
             self.name = name
             self.running = False
             self.is_detection_on = False
             self.new = False
             self.frame = None
+            self.reticle_coords = self.model.get_coords_axis(self.name)
 
             # TODO move to model structure
             self.prev_img = None
             self.reticle_zone = None
             self.is_probe_updated = True
             self.probes = {}
             self.sn = None
 
             self.IMG_SIZE = (1000, 750)
-            self.IMG_SIZE_ORIGINAL = (4000, 3000) # TODO
+            self.IMG_SIZE_ORIGINAL = (4000, 3000)  # TODO
             self.CROP_INIT = 50
             self.mask_detect = MaskGenerator()
 
         def update_sn(self, sn):
             """Update the serial number and initialize probe detectors.
 
             Args:
                 sn (str): Serial number.
             """
             if sn not in self.probes.keys():
                 self.sn = sn
                 self.probeDetect = ProbeDetector(self.sn, self.IMG_SIZE)
-                self.currPrevCmpProcess = CurrPrevCmpProcessor(self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE)
-                self.currBgCmpProcess = CurrBgCmpProcessor(self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE)
-                self.probes[self.sn] = {'probeDetector': self.probeDetect,
-                              'currPrevCmpProcess': self.currPrevCmpProcess,
-                              'currBgCmpProcess': self.currBgCmpProcess}
+                self.currPrevCmpProcess = CurrPrevCmpProcessor(
+                    self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE
+                )
+                self.currBgCmpProcess = CurrBgCmpProcessor(
+                    self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE
+                )
+                self.probes[self.sn] = {
+                    "probeDetector": self.probeDetect,
+                    "currPrevCmpProcess": self.currPrevCmpProcess,
+                    "currBgCmpProcess": self.currBgCmpProcess,
+                }
             else:
                 if sn != self.sn:
                     self.sn = sn
-                    self.probeDetect = self.probes[self.sn]['probeDetector']
-                    self.currPrevCmpProcess = self.probes[self.sn]['currPrevCmpProcess']
-                    self.currBgCmpProcess = self.probes[self.sn]['currBgCmpProcess']
-                else: 
+                    self.probeDetect = self.probes[self.sn]["probeDetector"]
+                    self.currPrevCmpProcess = self.probes[self.sn][
+                        "currPrevCmpProcess"
+                    ]
+                    self.currBgCmpProcess = self.probes[self.sn][
+                        "currBgCmpProcess"
+                    ]
+                else:
                     pass
-                
+
         def update_frame(self, frame, timestamp):
             """Update the frame and timestamp.
 
             Args:
                 frame (numpy.ndarray): Input frame.
                 timestamp (str): Timestamp of the frame.
             """
             self.frame = frame
             self.new = True
             self.timestamp = timestamp
 
         def process(self, frame, timestamp):
-            """ Process the frame for probe detection.
-            1. First run currPrevCmpProcess 
+            """Process the frame for probe detection.
+            1. First run currPrevCmpProcess
             2. If it fails on 1, run currBgCmpProcess
 
             Args:
                 frame (numpy.ndarray): Input frame.
                 timestamp (str): Timestamp of the frame.
 
             Returns:
                 tuple: Processed frame and timestamp.
             """
             if frame.ndim > 2:
                 gray_img = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
             else:
                 gray_img = frame
-        
+
             resized_img = cv2.resize(gray_img, self.IMG_SIZE)
             self.curr_img = cv2.GaussianBlur(resized_img, (9, 9), 0)
-            mask = self.mask_detect.process(resized_img)                # Generate Mask
+            mask = self.mask_detect.process(resized_img)  # Generate Mask
 
             if self.mask_detect.is_reticle_exist and self.reticle_zone is None:
-                reticle = ReticleDetection(self.IMG_SIZE, self.mask_detect, self.name)
-                self.reticle_zone = reticle.get_reticle_zone(frame)     # Generate X and Y Coordinates zone
+                reticle = ReticleDetection(
+                    self.IMG_SIZE, self.mask_detect, self.name
+                )
+                self.reticle_zone = reticle.get_reticle_zone(
+                    frame
+                )  # Generate X and Y Coordinates zone
                 self.currBgCmpProcess.update_reticle_zone(self.reticle_zone)
-            
+
             if self.prev_img is not None:
-                if self.probeDetect.angle is None:  # Detecting probe for the first time
-                    ret = self.currPrevCmpProcess.first_cmp(self.curr_img, self.prev_img, mask, gray_img)
+                if (
+                    self.probeDetect.angle is None
+                ):  # Detecting probe for the first time
+                    ret = self.currPrevCmpProcess.first_cmp(
+                        self.curr_img, self.prev_img, mask, gray_img
+                    )
                     if ret is False:
-                        ret = self.currBgCmpProcess.first_cmp(self.curr_img, mask, gray_img)
+                        ret = self.currBgCmpProcess.first_cmp(
+                            self.curr_img, mask, gray_img
+                        )
                     if ret:
                         logger.debug("First detect")
-                        logger.debug(f"angle: {self.probeDetect.angle}, tip: {self.probeDetect.probe_tip}, \
-                                                                base: {self.probeDetect.probe_base}")
-                else:                               # Tracking for the known probe
-                    ret = self.currPrevCmpProcess.update_cmp(self.curr_img, self.prev_img, mask, gray_img)
+                        logger.debug(
+                            f"angle: {self.probeDetect.angle}, \
+                            tip: {self.probeDetect.probe_tip}, \
+                            base: {self.probeDetect.probe_base}"
+                        )
+                else:  # Tracking for the known probe
+                    ret = self.currPrevCmpProcess.update_cmp(
+                        self.curr_img, self.prev_img, mask, gray_img
+                    )
                     if ret is False:
-                        ret = self.currBgCmpProcess.update_cmp(self.curr_img, mask, gray_img)
-            
-                    if ret:     # Found
-                        self.found_coords.emit(timestamp, self.sn, self.probeDetect.probe_tip_org)
-                        cv2.circle(frame, self.probeDetect.probe_tip_org, 5, (255, 255, 0), -1)
+                        ret = self.currBgCmpProcess.update_cmp(
+                            self.curr_img, mask, gray_img
+                        )
+
+                    if ret:  # Found
+                        self.found_coords.emit(
+                            timestamp, self.sn, self.probeDetect.probe_tip_org
+                        )
+                        cv2.circle(
+                            frame,
+                            self.probeDetect.probe_tip_org,
+                            5,
+                            (255, 255, 0),
+                            -1,
+                        )
 
                 if ret:
                     self.prev_img = self.curr_img
             else:
                 self.prev_img = self.curr_img
 
             return frame, timestamp
@@ -149,40 +193,61 @@
             """Start the probe detection."""
             self.is_detection_on = True
 
         def stop_detection(self):
             """Stop the probe detection."""
             self.is_detection_on = False
 
+        def process_draw_reticle(self, frame):
+            if self.reticle_coords is not None:
+                for idx, coords in enumerate(self.reticle_coords):
+                    # Normalize indices to 0-255 for colormap application.
+                    indices = np.linspace(
+                        0, 255, len(coords), endpoint=True, dtype=np.uint8
+                    )
+                    # Apply 'jet' colormap to x-coords, 'winter' to the y-coords.
+                    colormap = cv2.applyColorMap(
+                        indices,
+                        cv2.COLORMAP_JET if idx == 0 else cv2.COLORMAP_WINTER,
+                    )
+
+                    for point_idx, (x, y) in enumerate(coords):
+                        color = colormap[point_idx][0].tolist()
+                        cv2.circle(frame, (x, y), 2, color, -1)
+            return frame
+
         def run(self):
             """Run the worker thread."""
             print("probe_detect_manager running ")
             while self.running:
                 if self.new:
                     if self.is_detection_on:
-                        self.frame, self.timestamp = self.process(self.frame, self.timestamp)
+                        self.frame, self.timestamp = self.process(
+                            self.frame, self.timestamp
+                        )
+                    self.frame = self.process_draw_reticle(self.frame)
                     self.frame_processed.emit(self.frame)
                     self.new = False
                 time.sleep(0.001)
             print("probe_detect_manager running done")
             self.finished.emit()
 
-    def __init__(self, stages, camera_name):
-        """ Initialize ProbeDetectManager object """
+    def __init__(self, model, camera_name):
+        """Initialize ProbeDetectManager object"""
         super().__init__()
-        self.stages = stages
+        self.model = model
         self.worker = None
         self.name = camera_name
         self.thread = None
         self.init_thread()
 
     def init_thread(self):
         """Initialize the worker thread."""
         self.thread = QThread()
-        self.worker = self.Worker(self.name)
+        self.worker = self.Worker(self.name, self.model)
         self.worker.moveToThread(self.thread)
         self.thread.started.connect(self.worker.run)
         self.worker.frame_processed.connect(self.frame_processed)
         self.worker.found_coords.connect(self.found_coords_print)
         self.worker.finished.connect(self.thread.quit)
         self.worker.finished.connect(self.worker.deleteLater)
         self.thread.finished.connect(self.thread.deleteLater)
@@ -192,51 +257,55 @@
 
         Args:
             frame (numpy.ndarray): Input frame.
             timestamp (str): Timestamp of the frame.
         """
         if self.worker is not None:
             self.worker.update_frame(frame, timestamp)
-    
+
     def found_coords_print(self, timestamp, sn, pixel_coords):
         """Emit the found coordinates signal.
 
         Args:
             timestamp (str): Timestamp of the frame.
             sn (str): Serial number.
             pixel_coords (tuple): Pixel coordinates of the probe tip.
         """
-        moving_stage = self.stages.get(sn)
+        moving_stage = self.model.get_stage(sn)
         if moving_stage is not None:
-            stage_info = (moving_stage.stage_x, moving_stage.stage_y, moving_stage.stage_z)
-        #print(timestamp, sn, stage_info, pixel_coords)
+            stage_info = (
+                moving_stage.stage_x,
+                moving_stage.stage_y,
+                moving_stage.stage_z,
+            )
+        # print(timestamp, sn, stage_info, pixel_coords)
         self.found_coords.emit(timestamp, sn, stage_info, pixel_coords)
 
     def start(self):
         """Start the probe detection manager."""
         self.init_thread()  # Reinitialize and start the worker and thread
         self.worker.start_running()
         self.thread.start()
 
     def stop(self):
         """Stop the probe detection manager."""
         if self.worker is not None:
             self.worker.stop_running()
 
-    def start_detection(self, sn):       # Call from stage listener.
+    def start_detection(self, sn):  # Call from stage listener.
         """Start the probe detection for a specific serial number.
 
         Args:
             sn (str): Serial number.
         """
         if self.worker is not None:
             self.worker.update_sn(sn)
             self.worker.start_detection()
-    
-    def stop_detection(self, sn):       # Call from stage listener.
+
+    def stop_detection(self, sn):  # Call from stage listener.
         """Stop the probe detection for a specific serial number.
 
         Args:
             sn (str): Serial number.
         """
         if self.worker is not None:
             self.worker.stop_detection()
```

### Comparing `parallax_app-0.37.0/parallax/probe_detector.py` & `parallax_app-0.37.1/parallax/probe_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,84 +1,101 @@
 """
 ProbeDetector identifies probe tip and base in images using contour processing 
 and Hough Line Transform, with gradient analysis for refinement and directional 
 checks to ensure accuracy.
 """
-import numpy as np
-import cv2
+
 import logging
 from collections import Counter
 
+import cv2
+import numpy as np
+
 # Set logger name
 logger = logging.getLogger(__name__)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class ProbeDetector:
     """Class for detecting the probe in an image."""
+
     def __init__(self, sn, IMG_SIZE, angle_step=9):
-        """ Initialize Probe Detector object """
+        """Initialize Probe Detector object"""
         self.sn = sn
         self.IMG_SIZE = IMG_SIZE
         self.angle_step = angle_step
         self.angle = None
-        self.probe_tip, self.probe_base = (0,0), (0,0)
-        self.probe_tip_org = (0,0)
+        self.probe_tip, self.probe_base = (0, 0), (0, 0)
+        self.probe_tip_org = (0, 0)
         self.probe_tip_direction = "S"
         self.gradients = []
         self.angle_step_bins, self.angle_step_bins_with_neighbor = [], []
         self._init_gradient_bins()
-    
+
     def _init_gradient_bins(self):
         """Initialize gradient bins."""
-        self.angle_step_bins = np.arange(0, 180 + self.angle_step, self.angle_step)
-        self.angle_step_bins_with_neighbor = np.append(np.insert(self.angle_step_bins, 0, 180), 0)
+        self.angle_step_bins = np.arange(
+            0, 180 + self.angle_step, self.angle_step
+        )
+        self.angle_step_bins_with_neighbor = np.append(
+            np.insert(self.angle_step_bins, 0, 180), 0
+        )
 
     def _find_represent_gradient(self, gradient=0):
         """Find the representative gradient.
         Returns:
             float: Representative gradient value.
         """
         index = np.argmin(np.abs(self.angle_step_bins - gradient))
         return self.angle_step_bins[index]
-    
+
     def _find_neighboring_gradients(self, target_angle):
         """Find the neighboring gradients.
         Args:
             target_angle (float): Target angle.
         Returns:
             numpy.ndarray: Neighboring gradients.
         """
         gradient_index = np.where(self.angle_step_bins == target_angle)[0][0]
-        neighboring_gradients = self.angle_step_bins_with_neighbor[gradient_index:gradient_index + 3]
+        neighboring_gradients = self.angle_step_bins_with_neighbor[
+            gradient_index : gradient_index + 3
+        ]
         return neighboring_gradients
 
-    def _contour_preprocessing(self, img, thresh=20, remove_noise=True, noise_threshold=1):
+    def _contour_preprocessing(
+        self, img, thresh=20, remove_noise=True, noise_threshold=1
+    ):
         """Preprocess the image using contour detection.
         Args:
             img (numpy.ndarray): Input image.
             thresh (int): Threshold for contour area. Defaults to 20.
             remove_noise (bool): Flag to remove noise contours. Defaults to True.
             noise_threshold (int): Threshold for noise contour area. Defaults to 1.
         Returns:
             numpy.ndarray: Preprocessed image.
         """
         # Contour
-        contours, _ = cv2.findContours(img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+        contours, _ = cv2.findContours(
+            img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
         if not contours:
-            logger.debug(f"get_probe:: Not found contours. threshold: {thresh}", )
+            logger.debug(f"get_probe:: Not found contours. threshold: {thresh}")
             return None
         largest_contour = max(contours, key=cv2.contourArea)
         if cv2.contourArea(largest_contour) < thresh:
-            logger.debug(f"get_probe:: largest_contour is less than threshold {cv2.contourArea(largest_contour)}" )
+            logger.debug(
+                f"get_probe:: largest_contour is less than threshold {cv2.contourArea(largest_contour)}"
+            )
             return None
-        if remove_noise: 
+        if remove_noise:
             for contour in contours:
-                if cv2.contourArea(contour) < noise_threshold*noise_threshold:  # Remove Noise
+                # Remove Noise
+                if cv2.contourArea(contour) < noise_threshold*noise_threshold:
                     img = cv2.drawContours(img, [contour], -1, (0, 0, 0), -1)
         return img
 
     def _get_probe_direction(self, probe_tip, probe_base):
         """Get the direction of the probe.
         Args:
             probe_tip (tuple): Coordinates of the probe tip.
@@ -105,43 +122,54 @@
         else:
             if dx > 0:
                 return "E"
             elif dx < 0:
                 return "W"
             else:
                 return "Unknown"
-            
-    def _hough_line_first_detection(self, img, minLineLength=150, maxLineGap=40):
+
+    def _hough_line_first_detection(
+        self, img, minLineLength=150, maxLineGap=40
+    ):
         """Perform Hough line detection for the first time.
-        
+
         Args:
             img (numpy.ndarray): Input image.
             minLineLength (int): Minimum length of the line. Defaults to 150.
             maxLineGap (int): Maximum gap between line segments. Defaults to 40.
-            
+
         Returns:
             tuple: (found_ret, highest_point, lowest_point)
                 - found_ret (bool): Flag indicating if the probe is found.
                 - highest_point (tuple): Coordinates of the highest point of the probe.
                 - lowest_point (tuple): Coordinates of the lowest point of the probe.
         """
         found_ret = False
         self.gradients = []
         max_y, min_y = 0, img.shape[0]
-        lowest_point = (0,0)
-        highest_point = (0,0)
-        line_segments = cv2.HoughLinesP(img, 1, np.pi/180, 100, minLineLength=minLineLength, maxLineGap=maxLineGap)
-        
+        lowest_point = (0, 0)
+        highest_point = (0, 0)
+        line_segments = cv2.HoughLinesP(
+            img,
+            1,
+            np.pi / 180,
+            100,
+            minLineLength=minLineLength,
+            maxLineGap=maxLineGap,
+        )
+
         # Draw the line segments
         if line_segments is not None:
-            #logger.debug(len(line_segments)) 
+            # logger.debug(len(line_segments))
             if (len(line_segments)) >= 30:
-                logger.debug("hough_line_detection:: Too many line detected. Possibly Plane image ")
+                logger.debug(
+                    "hough_line_detection:: Too many line detected. Possibly Plane image "
+                )
                 return None, highest_point, lowest_point
-            
+
             for line in line_segments:
                 x2, y2, x1, y1 = line[0]
                 # Calculate the gradient
                 gradient = np.arctan2(y2 - y1, x2 - x1)
                 gradient = np.degrees(gradient)
                 gradient += 180
                 gradient %= 180
@@ -155,73 +183,86 @@
                     lowest_point = (x2, y2)
                 if y1 < min_y:
                     min_y = y1
                     highest_point = (x1, y1)
                 if y2 <= min_y:
                     min_y = y2
                     highest_point = (x2, y2)
-        
+
         if len(self.gradients) > 0:
             if self._is_distance_in_thres(highest_point, lowest_point):
-                logger.debug(f"Distance between tip and base is too close {highest_point} {lowest_point}")
+                logger.debug(
+                    f"Distance between tip and base is too close {highest_point} {lowest_point}"
+                )
                 return False, highest_point, lowest_point
             found_ret = True
             logger.debug(f"First line detection {self.gradients}")
             self.angle = np.median(self.gradients)
             return found_ret, highest_point, lowest_point
         else:
             return found_ret, highest_point, lowest_point
 
     def _hough_line_update(self, img, minLineLength=50, maxLineGap=9):
         """Update the Hough line detection.
         Args:
             img (numpy.ndarray): Input image.
             minLineLength (int): Minimum length of the line. Defaults to 50.
             maxLineGap (int): Maximum gap between line segments. Defaults to 9.
-            
+
         Returns:
             tuple: (found_ret, highest_point, lowest_point)
                 - found_ret (bool): Flag indicating if the probe is found.
                 - highest_point (tuple): Coordinates of the highest point of the probe.
                 - lowest_point (tuple): Coordinates of the lowest point of the probe.
         """
         self.gradients = []
         updated_gradient = self.angle
         max_y, min_y = 0, img.shape[0]
-        line_segments = cv2.HoughLinesP(img, 1, np.pi/180, 50, minLineLength=minLineLength, maxLineGap=maxLineGap)
-        found_ret, lowest_point, highest_point = False, (0,0), (0,0)
-        
+        line_segments = cv2.HoughLinesP(
+            img,
+            1,
+            np.pi / 180,
+            50,
+            minLineLength=minLineLength,
+            maxLineGap=maxLineGap,
+        )
+        found_ret, lowest_point, highest_point = False, (0, 0), (0, 0)
+
         # Find the neighboring gradients
         gradient_index = np.where(self.angle_step_bins == self.angle)
-        
+
         if gradient_index is None:
             return found_ret, highest_point, lowest_point
-        
+
         # Check if gradient_index is not empty
         if gradient_index[0].size == 0:
             return found_ret, highest_point, lowest_point
-    
+
         gradient_index = gradient_index[0][0]
-        neighboring_gradients = self.angle_step_bins_with_neighbor[gradient_index:gradient_index+3]
-        
+        neighboring_gradients = self.angle_step_bins_with_neighbor[
+            gradient_index : gradient_index + 3
+        ]
+
         # Draw the line segments
-        if line_segments is not None: 
+        if line_segments is not None:
             if (len(line_segments)) >= 30:
-                logger.debug("get_tip_hough_line_detection:: Too many line detected. Possibly Plane image")
+                logger.debug(
+                    "get_tip_hough_line_detection:: Too many line detected. Possibly Plane image"
+                )
                 return found_ret, highest_point, lowest_point
-        
+
             for line in line_segments:
                 x2, y2, x1, y1 = line[0]
                 # Calculate the gradient
                 gradient = np.arctan2(y2 - y1, x2 - x1)
                 gradient = np.degrees(gradient)
                 gradient += 180
                 gradient %= 180
                 representing_gradient = self._find_represent_gradient(gradient)
-                
+
                 if representing_gradient in neighboring_gradients:
                     self.gradients.append(representing_gradient)
                     found_ret = True
                     if y1 > max_y:
                         max_y = y1
                         lowest_point = (x1, y1)
                     if y2 > max_y:
@@ -229,159 +270,218 @@
                         lowest_point = (x2, y2)
                     if y1 < min_y:
                         min_y = y1
                         highest_point = (x1, y1)
                     if y2 <= min_y:
                         min_y = y2
                         highest_point = (x2, y2)
-            
+
             if found_ret is False:
-                return found_ret, highest_point, lowest_point      
+                return found_ret, highest_point, lowest_point
         else:
             logger.debug("get_tip_hough_line_detection:: Not found the line")
             return found_ret, highest_point, lowest_point
-        
+
         if found_ret:
             if self._is_distance_in_thres(highest_point, lowest_point):
-                logger.debug(f"Distance between tip and base is too close, {highest_point} {lowest_point}")
+                logger.debug(
+                    f"Distance between tip and base is too close, {highest_point} {lowest_point}"
+                )
                 return False, highest_point, lowest_point
-    
+
             gradient_counts = Counter(self.gradients)
             updated_gradient, _ = gradient_counts.most_common(1)[0]
-            logger.debug(f"target angle: {self.angle}, updated_detected: {updated_gradient}, neighbor: {neighboring_gradients}" )
-            #logger.debug(gradient_counts)
+            logger.debug(
+                f"target angle: {self.angle}, updated_detected: {updated_gradient}, neighbor: {neighboring_gradients}"
+            )
+            # logger.debug(gradient_counts)
             self.angle = updated_gradient
             return found_ret, highest_point, lowest_point
         else:
             return found_ret, highest_point, lowest_point
-        
+
     def _get_probe_point(self, mask, p1, p2, img_fname=None):
         """Get the probe tip and base points.
-        
+
         Args:
             mask (numpy.ndarray): Mask image.
             p1 (tuple): First point coordinates.
             p2 (tuple): Second point coordinates.
             img_fname (str, optional): Image filename. Defaults to None.
-            
+
         Returns:
             tuple: (probe_tip, probe_base)
                 - probe_tip (tuple): Coordinates of the probe tip.
                 - probe_base (tuple): Coordinates of the probe base.
         """
 
-        mask = cv2.copyMakeBorder(mask, 1, 1, 1, 1, cv2.BORDER_CONSTANT, value=[0, 0, 0])
+        mask = cv2.copyMakeBorder(
+            mask, 1, 1, 1, 1, cv2.BORDER_CONSTANT, value=[0, 0, 0]
+        )
         dist_transform = cv2.distanceTransform(mask, cv2.DIST_L2, 3)
         """
         if img_fname:
             mask_ = cv2.cvtColor(mask, cv2.COLOR_GRAY2BGR)
             cv2.circle(mask_, p1, 5, (0, 255, 0), -1)  # Green circle
             cv2.circle(mask_, p2, 5, (0, 0, 255), -1)  # Green circle
             
             output_fname = os.path.basename(img_fname).replace('.', '_mask.')
             cv2.imwrite('output/' + output_fname, mask_)
         """
         dist_p1 = dist_transform[p1[1], p1[0]]  # [y, x]
         dist_p2 = dist_transform[p2[1], p2[0]]
         logger.debug(f"dist_p1: {dist_p1}, dist_p2: {dist_p2}")
         if dist_p1 > dist_p2:
-            return p1, p2       # Return order: probe_tip, probe_base
+            return p1, p2  # Return order: probe_tip, probe_base
         else:
             return p2, p1
-    
-    def _get_probe_point_known_direction(self, highest_point, lowest_point, direction="S"):
+
+    def _get_probe_point_known_direction(
+        self, highest_point, lowest_point, direction="S"
+    ):
         """Get the probe tip and base points based on known direction.
-        
+
         Args:
             highest_point (tuple): Coordinates of the highest point.
             lowest_point (tuple): Coordinates of the lowest point.
             direction (str): Direction of the probe. Defaults to "S".
-            
+
         Returns:
             tuple: (probe_tip, probe_base)
                 - probe_tip (tuple): Coordinates of the probe tip.
                 - probe_base (tuple): Coordinates of the probe base.
         """
         if direction in ["S", "W", "SW", "SE"]:
-            return lowest_point, highest_point 
+            return lowest_point, highest_point
         else:
             return highest_point, lowest_point
-    
+
     def _is_distance_in_thres(self, point1, point2, thres=50):
         """Check if the distance between two points is within a threshold.
-        
+
         Args:
             point1 (tuple): Coordinates of the first point.
             point2 (tuple): Coordinates of the second point.
             thres (int): Distance threshold. Defaults to 50.
-            
+
         Returns:
             bool: True if the distance is within the threshold, False otherwise.
         """
         dist = ((point1[0] - point2[0]) ** 2 +
                 (point1[1] - point2[1]) ** 2 )** 0.5
         return dist < thres
 
     # Get the gradient / pixel points of probe at first time
-    def first_detect_probe(self, img, mask, contour_thresh=50, hough_minLineLength=130, offset_x = 0, offset_y = 0):
+    def first_detect_probe(
+        self,
+        img,
+        mask,
+        contour_thresh=50,
+        hough_minLineLength=130,
+        offset_x=0,
+        offset_y=0,
+    ):
         """Detect the probe in the image for the first time.
-        
+
         Args:
             img (numpy.ndarray): Input image.
             mask (numpy.ndarray): Mask image.
             contour_thresh (int): Threshold for contour area. Defaults to 50.
             hough_minLineLength (int): Minimum length of the line for Hough transform. Defaults to 130.
             offset_x (int): X-offset for probe coordinates.
             offset_y (int): Y-offset for probe coordinates.
-            
+
         Returns:
             bool: True if the probe is detected, False otherwise.
         """
         ret = False
         img = self._contour_preprocessing(img, thresh=contour_thresh)
         if img is None:
             return ret
-        
-        ret, highest_point, lowest_point = self._hough_line_first_detection(img, minLineLength=hough_minLineLength, maxLineGap=50) # update self.angle
+
+        ret, highest_point, lowest_point = self._hough_line_first_detection(
+            img, minLineLength=hough_minLineLength, maxLineGap=50
+        )  # update self.angle
         if ret:
-            self.probe_tip, self.probe_base = self._get_probe_point(mask, highest_point, lowest_point)
-            self.probe_tip_direction = self._get_probe_direction(self.probe_tip, self.probe_base)
-            self.probe_tip = (self.probe_tip[0] + offset_x, self.probe_tip[1] + offset_y)
-            self.probe_base = (self.probe_base[0] + offset_x, self.probe_base[1] + offset_y)
-            logger.debug(f"tip : {self.probe_tip}, base: {self.probe_base}" )
+            self.probe_tip, self.probe_base = self._get_probe_point(
+                mask, highest_point, lowest_point
+            )
+            self.probe_tip_direction = self._get_probe_direction(
+                self.probe_tip, self.probe_base
+            )
+            self.probe_tip = (
+                self.probe_tip[0] + offset_x,
+                self.probe_tip[1] + offset_y,
+            )
+            self.probe_base = (
+                self.probe_base[0] + offset_x,
+                self.probe_base[1] + offset_y,
+            )
+            logger.debug(f"tip : {self.probe_tip}, base: {self.probe_base}")
         return ret
 
-    
-    def update_probe(self, img, mask, contour_thresh=20, hough_minLineLength=200, maxLineGap=10, offset_x = 0, offset_y = 0, img_fname=None):
+    def update_probe(
+        self,
+        img,
+        mask,
+        contour_thresh=20,
+        hough_minLineLength=200,
+        maxLineGap=10,
+        offset_x=0,
+        offset_y=0,
+        img_fname=None,
+    ):
         """Update the probe detection in the image."""
         ret = False
-        img = self._contour_preprocessing(img, thresh=contour_thresh, remove_noise=False)
+        img = self._contour_preprocessing(
+            img, thresh=contour_thresh, remove_noise=False
+        )
         if img is None:
             logger.debug("update_probe:: contour_preprocessing fail")
             return False
 
         backup_angle = self.angle
-        ret, highest_point, lowest_point = self._hough_line_update(img, minLineLength=hough_minLineLength, maxLineGap=maxLineGap) #self.angle updated
+        ret, highest_point, lowest_point = self._hough_line_update(
+            img, minLineLength=hough_minLineLength, maxLineGap=maxLineGap
+        )  # self.angle updated
         if ret:
-            highest_point = (highest_point[0] + offset_x, highest_point[1] + offset_y)
-            lowest_point = (lowest_point[0] + offset_x, lowest_point[1] + offset_y)
-            
-            logger.debug(f"backup_angle: {backup_angle}, self.angle: {self.angle}")
+            highest_point = (
+                highest_point[0] + offset_x,
+                highest_point[1] + offset_y,
+            )
+            lowest_point = (
+                lowest_point[0] + offset_x,
+                lowest_point[1] + offset_y,
+            )
+
+            logger.debug(
+                f"backup_angle: {backup_angle}, self.angle: {self.angle}"
+            )
             if self.angle == backup_angle:
-                self.probe_tip, self.probe_base = self._get_probe_point_known_direction(highest_point, lowest_point, direction=self.probe_tip_direction)
+                self.probe_tip, self.probe_base = (
+                    self._get_probe_point_known_direction(
+                        highest_point,
+                        lowest_point,
+                        direction=self.probe_tip_direction,
+                    )
+                )
             else:
-                self.probe_tip, self.probe_base = self._get_probe_point(mask, highest_point, lowest_point)
-                self.probe_tip_direction = self._get_probe_direction(self.probe_tip, self.probe_base)
-                
+                self.probe_tip, self.probe_base = self._get_probe_point(
+                    mask, highest_point, lowest_point
+                )
+                self.probe_tip_direction = self._get_probe_direction(
+                    self.probe_tip, self.probe_base
+                )
+
                 """
                 print(self.probe_tip, self.probe_base, self.probe_tip_direction)
                 mask = cv2.cvtColor(mask, cv2.COLOR_GRAY2BGR)
                 cv2.circle(mask, self.probe_tip, 3, (0, 0, 255), 5)  # RED circle
                 cv2.circle(mask, self.probe_base, 3, (0, 255, 0), 5)  # RED circle
                 output_fname = os.path.basename(img_fname).replace('.', '_4_mask.')
                 cv2.imwrite('output/' + output_fname, mask)
                 """
         else:
             logger.debug("update_probe:: get_tip_hough_line_detection fail")
             return False
-        
+
         return ret
```

### Comparing `parallax_app-0.37.0/parallax/probe_fine_tip_detector.py` & `parallax_app-0.37.1/parallax/probe_fine_tip_detector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,105 +1,122 @@
 """
 ProbeFineTipDetector identifies a probe's fine tip in original images through preprocessing, 
 Harris corner detection, and geometric analysis, accommodating various probe orientations 
 for precise positioning tasks.
 """
+
+import logging
+
 import cv2
 import numpy as np
-import logging
+
 # Set logger name
 logger = logging.getLogger(__name__)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class ProbeFineTipDetector:
     """Class for detecting the fine tip of the probe in an image."""
+
     def __init__(self):
-        """ Initialize ProbeFineTipDetector object """
+        """Initialize ProbeFineTipDetector object"""
         self.img = None
-        self.tip = (0,0)
+        self.tip = (0, 0)
         self.offset_x = 0
         self.offset_y = 0
         self.direction = "S"
         self.img_fname = None
 
     def _preprocess_image(self):
         """Preprocess the image for tip detection."""
         self.img = cv2.GaussianBlur(self.img, (7, 7), 0)
         sharpened_image = cv2.Laplacian(self.img, cv2.CV_64F)
         sharpened_image = np.uint8(np.absolute(sharpened_image))
-        _, self.img = cv2.threshold(self.img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
-        #kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3)) #TODO
-        #self.img = cv2.erode(self.img, kernel_ellipse_3, iterations=1)
+        _, self.img = cv2.threshold(
+            self.img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU
+        )
+        # kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3)) #TODO
+        # self.img = cv2.erode(self.img, kernel_ellipse_3, iterations=1)
 
     def _is_valid(self):
         """Check if the image is valid for tip detection.
         Returns:
             bool: True if the image is valid, False otherwise.
         """
         height, width = self.img.shape[:2]
         boundary_img = np.zeros_like(self.img)
-        cv2.rectangle(boundary_img, (0, 0), (width-1, height-1), 255, 1)
+        cv2.rectangle(boundary_img, (0, 0), (width - 1, height - 1), 255, 1)
         and_result = cv2.bitwise_and(cv2.bitwise_not(self.img), boundary_img)
-        contours_boundary, _ = cv2.findContours(and_result, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+        contours_boundary, _ = cv2.findContours(
+            and_result, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
         if len(contours_boundary) >= 2:
-            logger.debug(f"get_probe_precise_tip fail. N of contours_boundary :{len(contours_boundary)}" )
+            logger.debug(
+                f"get_probe_precise_tip fail. N of contours_boundary :{len(contours_boundary)}"
+            )
             return False
-        
+
         boundary_img = np.zeros_like(self.img)
-        boundary_img[0,0] = 255
-        boundary_img[width-1, 0] = 255
-        boundary_img[0, height-1] = 255
-        boundary_img[width-1, height-1] = 255
+        boundary_img[0, 0] = 255
+        boundary_img[width - 1, 0] = 255
+        boundary_img[0, height - 1] = 255
+        boundary_img[width - 1, height - 1] = 255
         and_result = cv2.bitwise_and(and_result, boundary_img)
-        contours_boundary, _ = cv2.findContours(and_result, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+        contours_boundary, _ = cv2.findContours(
+            and_result, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
         if len(contours_boundary) >= 2:
-            logger.debug(f"get_probe_precise_tip fail. No detection of tip :{len(contours_boundary)}")
+            logger.debug(
+                f"get_probe_precise_tip fail. No detection of tip :{len(contours_boundary)}"
+            )
             return False
-        
+
         return True
 
     def _detect_closest_centroid(self):
         """Detect the closest centroid to the tip.
-        
+
         Returns:
             tuple: Coordinates of the closest centroid.
         """
         cx, cy = self.tip[0], self.tip[1]
         closest_centroid = (cx, cy)
-        min_distance = float('inf')
+        min_distance = float("inf")
 
         harris_corners = cv2.cornerHarris(self.img, blockSize=7, ksize=5, k=0.1)
         threshold = 0.3 * harris_corners.max()
 
         corner_marks = np.zeros_like(self.img)
         corner_marks[harris_corners > threshold] = 255
-        contours, _ = cv2.findContours(corner_marks, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
+        contours, _ = cv2.findContours(
+            corner_marks, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE
+        )
 
         for contour in contours:
             tip = self._get_direction_tip(contour)
             tip_x, tip_y = tip[0] + self.offset_x, tip[1] + self.offset_y
-            distance = np.sqrt((tip_x - cx)**2 + (tip_y - cy)**2)
+            distance = np.sqrt((tip_x - cx) ** 2 + (tip_y - cy) ** 2)
             if distance < min_distance:
                 min_distance = distance
                 closest_centroid = (tip_x, tip_y)
 
         return closest_centroid
 
     def _get_direction_tip(self, contour):
         """Get the tip coordinates based on the direction.
-        
+
         Args:
             contour (numpy.ndarray): Contour of the tip.
-            
+
         Returns:
             tuple: Coordinates of the tip based on the direction.
         """
-        tip = (0,0)
+        tip = (0, 0)
         if self.direction == "S":
             tip = max(contour, key=lambda point: point[0][1])[0]
         elif self.direction == "N":
             tip = min(contour, key=lambda point: point[0][1])[0]
         elif self.direction == "E":
             tip = max(contour, key=lambda point: point[0][0])[0]
         elif self.direction == "W":
@@ -108,36 +125,47 @@
             tip = min(contour, key=lambda point: point[0][1] - point[0][0])[0]
         elif self.direction == "NW":
             tip = min(contour, key=lambda point: point[0][1] + point[0][0])[0]
         elif self.direction == "SE":
             tip = max(contour, key=lambda point: point[0][1] + point[0][0])[0]
         elif self.direction == "SW":
             tip = max(contour, key=lambda point: point[0][1] - point[0][0])[0]
-            
+
         return tip
-    
-    def _register(self, img, tip, offset_x=0, offset_y=0, direction=None, img_fname=None):
+
+    def _register(
+        self, img, tip, offset_x=0, offset_y=0, direction=None, img_fname=None
+    ):
         """Register the image, tip coordinates, offsets, direction, and filename."""
         self.img = img
         self.tip = tip
         self.offset_x = offset_x
         self.offset_y = offset_y
         self.direction = direction
         self.img_fname = img_fname
-    
-    def get_precise_tip(self, img, tip, offset_x=0, offset_y=0, direction=None, img_fname=None):
+
+    def get_precise_tip(
+        self, img, tip, offset_x=0, offset_y=0, direction=None, img_fname=None
+    ):
         """Get the precise tip coordinates from the image."""
-        self._register(img, tip, offset_x=offset_x, offset_y=offset_y, direction=direction, img_fname=img_fname)
+        self._register(
+            img,
+            tip,
+            offset_x=offset_x,
+            offset_y=offset_y,
+            direction=direction,
+            img_fname=img_fname,
+        )
 
         self._preprocess_image()
         if not self._is_valid():
             logger.debug("Boundary check failed.")
             return False
 
         self.tip = self._detect_closest_centroid()
-        #cv2.circle(self.img, (self.tip[0]-offset_x, self.tip[1]-offset_y), 1, (255, 255, 0), -1)
+        # cv2.circle(self.img, (self.tip[0]-offset_x, self.tip[1]-offset_y), 1, (255, 255, 0), -1)
 
         # Save the final image with the detected tip
-        #output_fname = os.path.basename(self.img_fname).replace('.', '_3_tip.')
-        #cv2.imwrite('output/' + output_fname, self.img_original)
+        # output_fname = os.path.basename(self.img_fname).replace('.', '_3_tip.')
+        # cv2.imwrite('output/' + output_fname, self.img_original)
 
         return True
```

### Comparing `parallax_app-0.37.0/parallax/recording_manager.py` & `parallax_app-0.37.1/parallax/recording_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 """
 RecordingManager manages snapshot saving and video recording from multiple camera feeds, 
 supporting custom file naming and ensuring recordings are properly initiated and 
 stopped across active cameras.
 """
-import os
+
 import logging
+import os
 
 # Set logger name
 logger = logging.getLogger(__name__)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class RecordingManager:
     """RecordingManager manages snapshot saving and video recording"""
+
     def __init__(self, model):
         """Initialize recording manager"""
         self.model = model
         self.recording_camera_list = []
 
     def save_last_image(self, save_path, screen_widgets):
         """Saves the last captured image from all active camera feeds."""
-         # Initialize the list to keep track of cameras from which an image has been saved
+        # Initialize the list to keep track of cameras from which an image has been saved
         snapshot_camera_list = []
         # Get the directory path where the images will be saved
         if os.path.exists(save_path):
             print("\nSnapshot...")
             for screen in screen_widgets:
-                # Save image only for 'Blackfly' camera 
-                if screen.is_camera():      
+                # Save image only for 'Blackfly' camera
+                if screen.is_camera():
                     # Use custom name of the camera if it has one, otherwise use the camera's serial number
                     camera_name = screen.get_camera_name()
                     if camera_name not in snapshot_camera_list:
                         customName = screen.parent().title()
-                        customName =  customName if customName else camera_name
-                        
+                        customName = customName if customName else camera_name
+
                         # Save the image with a timestamp and custom name
-                        screen.save_image(save_path, isTimestamp=True, name=customName)
-                        
+                        screen.save_image(
+                            save_path, isTimestamp=True, name=customName
+                        )
+
                         # Add the camera to the list of cameras from which an image has been saved
                         snapshot_camera_list.append(camera_name)
                 else:
                     logger.debug("save_last_image) camera not found")
         else:
             print(f"Directory {save_path} does not exist!")
 
@@ -49,39 +54,43 @@
         """
         Initiates recording for all active camera feeds.
         Records video from all active camera feeds and saves them to a specified directory.
         The directory path is taken from the label showing the current save directory.
         """
         # Initialize the list to keep track of cameras that are currently recording
         self.recording_camera_list = []
-               
+
         if os.path.exists(save_path):
             # Iterate through each screen widget
             print("\nRecording... ")
             for screen in screen_widgets:
                 # Check if the current screen is a camera
-                if screen.is_camera():                      # If name is 'Blackfly"
-                    camera_name = screen.get_camera_name()  # Get the name of the camer
+                if screen.is_camera():  # If name is 'Blackfly"
+                    camera_name = (
+                        screen.get_camera_name()
+                    )  # Get the name of the camer
                     # If this camera is not already in the list of recording cameras, then record
                     if camera_name not in self.recording_camera_list:
                         # Use custom name of the camera if it has one, otherwise use the camera's serial number
                         customName = screen.parent().title()
-                        customName =  customName if customName else camera_name
+                        customName = customName if customName else camera_name
                         # Start recording and save the video with a timestamp and custom name
-                        screen.save_recording(save_path, isTimestamp=True, name=customName)
+                        screen.save_recording(
+                            save_path, isTimestamp=True, name=customName
+                        )
                         self.recording_camera_list.append(camera_name)
         else:
-            # If the save directory does not exist   
+            # If the save directory does not exist
             print(f"Directory {save_path} does not exist!")
 
     def stop_recording(self, screen_widgets):
         """
         Stops recording for all cameras that are currently recording.
         """
         # Iterate through each screen widget
         for screen in screen_widgets:
-                camera_name =  screen.get_camera_name()
-                # Check if it is 'Balckfly' camera and in the list of recording cameras
-                if screen.is_camera() and camera_name in self.recording_camera_list:
-                    screen.stop_recording()         # Stop recording
-                    # Remove the camera from the list of cameras that are currently recording 
-                    self.recording_camera_list.remove(camera_name) 
+            camera_name = screen.get_camera_name()
+            # Check if it is 'Balckfly' camera and in the list of recording cameras
+            if screen.is_camera() and camera_name in self.recording_camera_list:
+                screen.stop_recording()  # Stop recording
+                # Remove the camera from the list of cameras that are currently recording
+                self.recording_camera_list.remove(camera_name)
```

### Comparing `parallax_app-0.37.0/parallax/reticle_detect_manager.py` & `parallax_app-0.37.1/parallax/reticle_detect_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,72 @@
 """
 Manages reticle detection in images through a worker thread, integrating line detection, 
 masking, coordinate analysis, and camera calibration. Uses PyQt's signals 
 for thread-safe operations and real-time processing feedback.
 """
-from PyQt5.QtCore import pyqtSignal, QObject, QThread
-from .reticle_detection import ReticleDetection
-from .mask_generator import MaskGenerator
-from .reticle_detection_coords_interests import ReticleDetectCoordsInterest
-from .calibration_camera import CalibrationCamera
+
+import logging
+import time
+
 import cv2
 import numpy as np
-import time
-import logging
+from PyQt5.QtCore import QObject, QThread, pyqtSignal
+
+from .calibration_camera import CalibrationCamera
+from .mask_generator import MaskGenerator
+from .reticle_detection import ReticleDetection
+from .reticle_detection_coords_interests import ReticleDetectCoordsInterest
 
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.DEBUG)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.DEBUG)
 
+
 class ReticleDetectManager(QObject):
-    """ Reticle detection class """
+    """Reticle detection class"""
+
     name = "None"
     frame_processed = pyqtSignal(object)
     found_coords = pyqtSignal(np.ndarray, np.ndarray, np.ndarray, np.ndarray)
 
     class Worker(QObject):
-        """ Reticle detection Worker Thread """
+        """Reticle detection Worker Thread"""
+
         finished = pyqtSignal()
         frame_processed = pyqtSignal(object)
-        found_coords = pyqtSignal(np.ndarray, np.ndarray, np.ndarray, np.ndarray) 
+        found_coords = pyqtSignal(
+            np.ndarray, np.ndarray, np.ndarray, np.ndarray
+        )
 
         def __init__(self, name):
             """Initialize the worker"""
             QObject.__init__(self)
             self.name = name
             self.running = False
             self.is_detection_on = False
             self.new = False
             self.frame = None
-            self.IMG_SIZE_ORIGINAL = (4000, 3000) # TODO
+            self.IMG_SIZE_ORIGINAL = (4000, 3000)  # TODO
             self.frame_success = None
 
             self.mask_detect = MaskGenerator()
-            self.reticleDetector = ReticleDetection(self.IMG_SIZE_ORIGINAL, self.mask_detect, self.name)
+            self.reticleDetector = ReticleDetection(
+                self.IMG_SIZE_ORIGINAL, self.mask_detect, self.name
+            )
             self.coordsInterests = ReticleDetectCoordsInterest()
             self.calibrationCamera = CalibrationCamera(self.name)
-                
+
         def update_frame(self, frame):
             """Update the frame to be processed."""
             self.frame = frame
-            if self.new is False: # Deal with one frame at a time. This may cause the frame drop
+            # Deal with one frame at a time. This may cause the frame drop
+            if self.new is False:
                 self.new = True
 
         def draw(self, frame, x_axis_coords, y_axis_coords):
             """Draw the coordinates on the frame.
 
             Args:
                 frame (numpy.ndarray): Input frame.
@@ -70,88 +81,122 @@
             for pixel in x_axis_coords:
                 pt = tuple(pixel)
                 cv2.circle(frame, pt, 7, (255, 255, 0), -1)
             for pixel in y_axis_coords:
                 pt = tuple(pixel)
                 cv2.circle(frame, pt, 7, (0, 255, 255), -1)
             return frame
-        
+
         def draw_xyz(self, frame, origin, x, y, z):
             """Draw the XYZ axes on the frame."""
             frame = cv2.line(frame, origin, x, (0, 0, 255), 3)  # Blue line
             frame = cv2.line(frame, origin, y, (0, 255, 0), 3)  # Green line
             frame = cv2.line(frame, origin, z, (255, 0, 0), 3)  # Red line
             return frame
 
         def draw_calibration_info(self, frame, ret, mtx, dist):
             """
             Draw calibration information on the frame.
-            
+
             Parameters:
             - frame: The image frame on which to draw.
             - ret: Boolean indicating if calibration was successful.
             - mtx: The camera matrix obtained from calibration.
             - dist: The distortion coefficients obtained from calibration.
             """
-            
+
             # Starting position for the text
             offset_start = 50
             line_height = 60
-            
+
             # Basic settings for the text
             font = cv2.FONT_HERSHEY_SIMPLEX
             font_scale = 1.5
             font_color = (255, 255, 255)  # White color
             line_type = 2
-            
+
             # Status text
             status_text = f"Overall RMS re-projection error: {ret}"
-            cv2.putText(frame, status_text, (10, offset_start), font, font_scale, font_color, line_type)
-            
+            cv2.putText(
+                frame,
+                status_text,
+                (10, offset_start),
+                font,
+                font_scale,
+                font_color,
+                line_type,
+            )
+
             # Camera matrix text
             mtx_lines = [
                 f"Camera Matrix:",
                 f"[{mtx[0][0]:.2f}, {mtx[0][1]:.2f}, {mtx[0][2]:.2f}]",
                 f"[{mtx[1][0]:.2f}, {mtx[1][1]:.2f}, {mtx[1][2]:.2f}]",
                 f"[{mtx[2][0]:.2f}, {mtx[2][1]:.2f}, {mtx[2][2]:.2f}]"
             ]
             # Draw each line of the camera matrix
             for i, line in enumerate(mtx_lines):
-                cv2.putText(frame, line, (10, offset_start+line_height + i * line_height), 
-                            font, font_scale, font_color, line_type)
-                
+                cv2.putText(
+                    frame,
+                    line,
+                    (10, offset_start + line_height + i * line_height),
+                    font,
+                    font_scale,
+                    font_color,
+                    line_type,
+                )
+
             # Distortion coefficients text
-            dist_text = f"Dist Coeffs: [{dist[0][0]:.4f}, {dist[0][1]:.4f}, {dist[0][2]:.4f}, {dist[0][3]:.4f} {dist[0][4]:.4f}]"
-            cv2.putText(frame, dist_text, (10, offset_start + line_height*5), font, font_scale, font_color, line_type)
-            
+            dist_text = f"Dist Coeffs: [{dist[0][0]:.4f}, {dist[0][1]:.4f}, \
+                {dist[0][2]:.4f}, {dist[0][3]:.4f} {dist[0][4]:.4f}]"
+            cv2.putText(
+                frame,
+                dist_text,
+                (10, offset_start + line_height * 5),
+                font,
+                font_scale,
+                font_color,
+                line_type,
+            )
+
             return frame
 
         def process(self, frame):
             """Process the frame for reticle detection."""
-            #cv2.circle(frame, (2000,1500), 10, (255, 0, 0), -1)
-            ret, frame_, _, inliner_lines_pixels = self.reticleDetector.get_coords(frame)
+            # cv2.circle(frame, (2000,1500), 10, (255, 0, 0), -1)
+            ret, frame_, _, inliner_lines_pixels = (
+                self.reticleDetector.get_coords(frame)
+            )
             if ret:
-                ret, x_axis_coords, y_axis_coords = self.coordsInterests.get_coords_interest(inliner_lines_pixels)
+                ret, x_axis_coords, y_axis_coords = (
+                    self.coordsInterests.get_coords_interest(
+                        inliner_lines_pixels
+                    )
+                )
             if ret:
                 # TODO
-                #ret, mtx, dist = self.calibrationCamera.get_predefined_intrinsic(x_axis_coords, y_axis_coords)
-                #if not ret:
-                ret, mtx, dist = self.calibrationCamera.calibrate_camera(x_axis_coords, y_axis_coords) 
+                # ret, mtx, dist = self.calibrationCamera.get_predefined_intrinsic(x_axis_coords, y_axis_coords)
+                # if not ret:
+                ret, mtx, dist = self.calibrationCamera.calibrate_camera(
+                    x_axis_coords, y_axis_coords
+                )
                 if ret:
                     # Draw
-                    self.found_coords.emit(x_axis_coords, y_axis_coords, mtx, dist)
+                    self.found_coords.emit(
+                        x_axis_coords, y_axis_coords, mtx, dist
+                    )
                     origin, x, y, z = self.calibrationCamera.get_origin_xyz()
                     frame = self.draw_xyz(frame, origin, x, y, z)
                     frame = self.draw(frame, x_axis_coords, y_axis_coords)
                     frame = self.draw_calibration_info(frame, ret, mtx, dist)
                 self.frame_success = frame
             if self.frame_success is None:
                 logger.debug(f"{ self.name} reticle detection fail ")
                 return frame
-            else: 
+            else:
                 logger.debug(f"{ self.name} reticle detection success ")
                 return self.frame_success
 
         def stop_running(self):
             """Stop the worker from running."""
             self.running = False
 
@@ -175,60 +220,60 @@
                     self.frame_processed.emit(self.frame)
                 self.new = False
                 time.sleep(0.001)
             self.finished.emit()
             logger.debug(f"thread finished {self.name}")
 
         def set_name(self, name):
-            """ Set name as camera serial number. """
+            """Set name as camera serial number."""
             self.name = name
 
     def __init__(self, camera_name):
         """Initialize the reticle detection manager."""
         logger.debug("Init reticle detect manager")
         super().__init__()
         self.worker = None
         self.name = camera_name
         self.thread = None
-    
+
     def init_thread(self):
         """Initialize the worker thread."""
         if self.thread is not None:
             self.clean()  # Clean up existing thread and worker before reinitializing
         self.thread = QThread()
         self.worker = self.Worker(self.name)
         self.worker.moveToThread(self.thread)
 
         self.thread.started.connect(self.worker.run)
         self.thread.finished.connect(self.thread.deleteLater)
         self.thread.destroyed.connect(self.onThreadDestroyed)
         self.threadDeleted = False
 
         self.worker.frame_processed.connect(self.frame_processed)
-        self.worker.found_coords.connect(self.found_coords) 
+        self.worker.found_coords.connect(self.found_coords)
         self.worker.finished.connect(self.thread.quit)
         self.worker.finished.connect(self.worker.deleteLater)
         logger.debug(f"init camera name: {self.name}")
 
     def process(self, frame):
         """Process the frame using the worker.
 
         Args:
             frame (numpy.ndarray): Input frame.
         """
         if self.worker is not None:
             self.worker.update_frame(frame)
-    
+
     def start(self):
         """Start the reticle detection manager."""
         self.init_thread()  # Reinitialize and start the worker and thread
         self.worker.start_running()
         self.thread.start()
         logger.debug(f"thread started {self.name}")
-    
+
     def stop(self):
         """Stop the reticle detection manager."""
         if self.worker is not None:
             self.worker.stop_running()
 
     def set_name(self, camera_name):
         """Set camera name."""
@@ -245,13 +290,13 @@
         if not self.threadDeleted and self.thread.isRunning():
             self.thread.quit()  # Ask the thread to quit
             self.thread.wait()  # Wait for the thread to finish
         self.thread = None  # Clear the reference to the thread
         self.worker = None  # Clear the reference to the worker
 
     def onThreadDestroyed(self):
-        """ Flag if thread is deleted """
+        """Flag if thread is deleted"""
         self.threadDeleted = True
 
     def __del__(self):
         """Destructor for the reticle detection manager."""
         self.clean()
```

### Comparing `parallax_app-0.37.0/parallax/reticle_detection.py` & `parallax_app-0.37.1/parallax/reticle_detection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """ ReticleDetection for identifying reticle coordinates in microscopy images
 
 Process: 
 - preprocessing, masking, and morphological operations
 - Utilizes adaptive thresholding, Gaussian blurring, and RANSAC for line detection, line drawing, and pixel refinement
 - Supports line intersection and missing point estimation
 """
-from scipy.stats import linregress
-from skimage.measure import LineModelND, ransac
-import numpy as np
-import cv2
+
 import logging
 import warnings
 
+import cv2
+import numpy as np
+from scipy.stats import linregress
+from skimage.measure import LineModelND, ransac
+
 # Set logger name
 logger = logging.getLogger(__name__)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logger.setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class ReticleDetection:
     """Class for detecting reticle lines and coordinates."""
+
     def __init__(self, IMG_SIZE, reticle_frame_detector, camera_name):
-        """ Initialize Reticle Detection object """
+        """Initialize Reticle Detection object"""
         self.image_size = IMG_SIZE
         self.reticle_frame_detector = reticle_frame_detector
         self.mask = None
         self.name = camera_name
 
     def _preprocess_image(self, img):
         """Convert image to grayscale, blur, and resize."""
@@ -48,42 +52,54 @@
         """Draw lines on the reticle points based on detected pixels."""
         reticle_points = np.zeros_like(img)
         width, height = self.image_size
 
         for pixels_in_line in pixels_in_lines:
             self._draw_line(reticle_points, pixels_in_line, width, height)
 
-        #cv2.imwrite("debug/reticle_zone.jpg", reticle_points)
+        # cv2.imwrite("debug/reticle_zone.jpg", reticle_points)
         return reticle_points
 
     def _draw_line(self, reticle_points, pixels_in_line, width, height):
         """Draw a single line across the reticle points."""
         x1, y1 = pixels_in_line[0]
         x2, y2 = pixels_in_line[-1]
-                
+
         if x2 - x1 == 0:  # Prevent division by zero
             m = np.inf
             x_vert = x1  # Vertical line x-coordinate
         else:
             m = (y2 - y1) / (x2 - x1)
             b = y1 - m * x1
 
         if m == np.inf:
-            cv2.line(reticle_points, (x_vert, 0), (x_vert, height), (255, 255, 255), 35)
+            cv2.line(
+                reticle_points,
+                (x_vert, 0),
+                (x_vert, height),
+                (255, 255, 255),
+                35,
+            )
         else:
             y_start = int(m * 0 + b)
             y_end = int(m * width + b)
-            cv2.line(reticle_points, (0, y_start), (width, y_end), (255, 255, 255), 35)
-    
+            cv2.line(
+                reticle_points,
+                (0, y_start),
+                (width, y_end),
+                (255, 255, 255),
+                35,
+            )
+
     def _ransac_detect_lines(self, img):
         """Detect lines using RANSAC algorithm.
-        
+
         Args:
             img (numpy.ndarray): Input image.
-            
+
         Returns:
             tuple: (ret, inlier_lines, inlier_pixels)
                 - ret (bool): True if two lines are detected, False otherwise.
                 - inlier_lines (list): List of detected line models.
                 - inlier_pixels (list): List of inlier pixel coordinates for each line.
         """
         inlier_lines = []
@@ -94,124 +110,128 @@
 
         # Draw
         if len(img.shape) == 2:  # Grayscale image
             img_color = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
         else:  # Color image
             img_color = img.copy()
 
-        contours, _ = cv2.findContours(img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+        contours, _ = cv2.findContours(
+            img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        )
         centroids = np.array(self._get_centroid(contours))
         if len(centroids) < 10:
             logger.debug("points for rasac line detection are less than 10")
             return False, inlier_lines, inlier_pixels
-        
+
         max_trials = 7000
         residual_threshold = 2
         counter = 50
         while len(inlier_lines) < 2 and counter > 0:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", RuntimeWarning)
-                model_robust, inliers = ransac(centroids, 
-                                               LineModelND, 
-                                               min_samples=9, 
-                                               residual_threshold=residual_threshold, 
-                                               max_trials=max_trials)
+                model_robust, inliers = ransac(
+                    centroids,
+                    LineModelND,
+                    min_samples=9,
+                    residual_threshold=residual_threshold,
+                    max_trials=max_trials,
+                )
             inlier_points = centroids[inliers]
             if len(inlier_points) >= 20:
                 logger.debug(f"residual_threshold: {residual_threshold}")
                 inlier_pixels.append(inlier_points)
                 inlier_lines.append(model_robust)
                 centroids = centroids[~inliers]
                 max_trials = 7000
                 residual_threshold = 2
-                counter = 50   # Reset counter
+                counter = 50  # Reset counter
             else:
-                max_trials += 2000                  # if not found, run RASAC again
+                max_trials += 2000  # if not found, run RASAC again
                 counter -= 1
                 if residual_threshold <= 15:
                     residual_threshold += 1
                 continue
 
         # Draw the centroids
         """
         for points in inlier_pixels:
             for point in points:
                 cv2.circle(img_color, (int(point[0]), int(point[1])), 1, (0, 0, 255), -1)  # Draw green circles
         cv2.imwrite("debug/centroid.jpg", img_color)
         """
-        
-        return len(inlier_lines)==2, inlier_lines, inlier_pixels
-    
+
+        return len(inlier_lines) == 2, inlier_lines, inlier_pixels
+
     def _fit_line(self, pixels):
         """Fit a line to the given pixels.
-        
+
         Args:
             pixels (numpy.ndarray): Pixel coordinates.
-            
+
         Returns:
             tuple: (slope, intercept) of the fitted line.
         """
         x_coords, y_coords = zip(*pixels)
         slope, intercept, _, _, _ = linregress(x_coords, y_coords)
         return slope, intercept
 
     def _find_intersection(self, line1, line2):
         """Find the intersection point of two lines.
-        
+
         Args:
             line1 (tuple): (slope, intercept) of the first line.
             line2 (tuple): (slope, intercept) of the second line.
-            
+
         Returns:
             tuple or None: (x, y) coordinates of the intersection point if it exists, None otherwise.
         """
         slope1, intercept1 = line1
         slope2, intercept2 = line2
 
         if slope1 == slope2:
             return None  # No intersection (parallel lines)
 
         x_intersect = (intercept2 - intercept1) / (slope1 - slope2)
         y_intersect = slope1 * x_intersect + intercept1
         return int(round(x_intersect)), int(round(y_intersect))
-        
+
     def _get_center_coords_index(self, center, coords):
         """Get the index of the center coordinates in the given coordinates.
-        
+
         Args:
             center (tuple): Center coordinates (x, y).
             coords (numpy.ndarray): Array of coordinates.
-            
+
         Returns:
             int or None: Index of the center coordinates in the coords array, None if not found.
         """
         x_center, y_center = center
         for i in range(-4, 5):
             for j in range(-4, 5):
                 test_center = np.array([x_center + i, y_center + j])
                 result = np.where((coords == test_center).all(axis=1))
                 if len(result[0]) > 0:
                     return result[0][0]
         return None
 
     def _get_pixels_interest(self, center, coords, dist=10):
         """Get the pixels of interest around the center coordinates.
-        
+
         Args:
             center (tuple): Center coordinates (x, y).
             coords (numpy.ndarray): Array of coordinates.
             dist (int): Distance from the center to select pixels of interest. Defaults to 10.
-            
+
         Returns:
             numpy.ndarray or None: Selected pixels of interest, None if center is not found.
         """
         center_index = self._get_center_coords_index(center, coords)
         if center_index is None:
             return
-        
+
         start_index = max(center_index - dist, 0)
         end_index = min(center_index + dist + 1, len(coords))
         return coords[start_index:end_index]
 
     def _find_reticle_coords(self, pixels_in_lines):
         """Find the reticle coordinates from the pixels in lines.
         Args:
@@ -231,66 +251,68 @@
             coords = self._get_pixels_interest(center_point, pixels_in_line)
             coords_interest.append(coords)
 
         return coords_interest
 
     def _eroding(self, img):
         """Erode the image until the desired contour conditions are met.
-        
+
         Args:
             img (numpy.ndarray): Input image.
-            
+
         Returns:
             numpy.ndarray: Eroded image.
         """
         kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3))
         counter = 100
         while counter > 0:
-            contours, _ = cv2.findContours(img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+            contours, _ = cv2.findContours(
+                img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+            )
             if not contours:
                 break
-            
+
             largest_contour = max(contours, key=cv2.contourArea)
             largest_contour_area = cv2.contourArea(largest_contour)
-            if 50 < len(contours) < 300 and largest_contour_area < 30*30:
+            if 50 < len(contours) < 300 and largest_contour_area < 30 * 30:
                 break
             img = cv2.erode(img, kernel_ellipse_3, iterations=1)
             img = cv2.morphologyEx(img, cv2.MORPH_OPEN, kernel_ellipse_3)
             counter -= 1
         return img
 
     def _get_centroid(self, contours):
         """Get the centroid of each contour.
-        
+
         Args:
             contours (list): List of contours.
-            
+
         Returns:
             list: List of centroid coordinates for each contour.
         """
         centroids = []
         for contour in contours:
             M = cv2.moments(contour)
             if M["m00"] != 0:
                 cX = int(M["m10"] / M["m00"])
                 cY = int(M["m01"] / M["m00"])
                 centroids.append([cX, cY])
         return centroids
-    
+
     def __del__(self):
-        """ Delete the instance """
-        #print("ReticleDetection Object destroyed")
+        """Delete the instance"""
+        # print("ReticleDetection Object destroyed")
         pass
-    
+
     def _sort_points(self, points):
         """Sort the points based on the dimension with greater median distance.
-        
+
         Args:
             points (numpy.ndarray): Array of points.
-            
+
         Returns:
             numpy.ndarray: Sorted points.
         """
         # Calculate differences between consecutive points
         diffs = np.diff(points, axis=0)
         x_diffs = diffs[:, 0]
         y_diffs = diffs[:, 1]
@@ -307,54 +329,58 @@
             # Sort points based on y component if y has greater median distance
             sorted_points = points[np.argsort(-points[:, 1])]
 
         return sorted_points
 
     def _estimate_missing_points(self, points, threshold_factor=1.5):
         """Estimate missing points in the given points based on the average distance.
-        
+
         Args:
             points (numpy.ndarray): Array of points.
             threshold_factor (float): Factor to determine the threshold for large gaps. Defaults to 1.5.
-            
+
         Returns:
             numpy.ndarray: Array of estimated missing points.
         """
         points = self._sort_points(points)
 
         # Calculate the Euclidean distances between consecutive points
         distances = np.linalg.norm(np.diff(points, axis=0), axis=1)
-        
+
         # Estimate the average distance
         average_distance = np.median(distances)
 
         # Identify large gaps
         threshold = threshold_factor * average_distance
         large_gaps = np.where(distances > threshold)[0]
 
         # Estimate missing points in the large gaps
         missing_points = []
         for gap_index in large_gaps:
             start_point = points[gap_index]
             end_point = points[gap_index + 1]
-            num_missing = int(round(distances[gap_index] / average_distance)) - 1
+            num_missing = (
+                int(round(distances[gap_index] / average_distance)) - 1
+            )
             for i in range(1, num_missing + 1):
-                missing_point = start_point + (end_point - start_point) * (i / (num_missing + 1))
+                missing_point = start_point + (end_point - start_point) * (
+                    i / (num_missing + 1)
+                )
                 missing_points.append(np.round(missing_point))
 
         return np.array(missing_points)
 
     def _add_missing_pixels(self, bg, lines, line_pixels):
         """Add missing pixels to the line pixels based on the estimated missing points.
-        
+
         Args:
             bg (numpy.ndarray): Background image.
             lines (list): List of line models.
             line_pixels (list): List of pixel coordinates for each line.
-            
+
         Returns:
             tuple: (bg, refined_pixels)
                 - bg (numpy.ndarray): Background image with missing points drawn.
                 - refined_pixels (list): List of refined pixel coordinates for each line.
         """
         refined_pixels = []
 
@@ -363,160 +389,193 @@
             missing_points = self._estimate_missing_points(pixels_array)
 
             if missing_points.ndim == 1 and missing_points.size > 0:
                 missing_points = missing_points.reshape(-1, 2)  # Reshape to 2D if it's flat but not empty
             elif missing_points.size == 0:
                 missing_points_adjusted = np.array([])  # Handle empty case
             else:
-                missing_points_adjusted = np.array([(x, line_model.predict_y(np.array([x]))[0]) for x in missing_points[:, 0]])
+                missing_points_adjusted = np.array(
+                    [
+                        (x, line_model.predict_y(np.array([x]))[0])
+                        for x in missing_points[:, 0]
+                    ]
+                )
 
             # Combine original and adjusted missing points
             if missing_points_adjusted.size > 0:
-                full_line_pixels = np.vstack((pixels_array, missing_points_adjusted))
+                full_line_pixels = np.vstack(
+                    (pixels_array, missing_points_adjusted)
+                )
             else:
                 full_line_pixels = pixels_array
-            
+
             # Sort pixels
             # Calculate the ranges for x and y coordinates
-            minX, maxX = full_line_pixels[:, 0].min(), full_line_pixels[:, 0].max()
-            minY, maxY = full_line_pixels[:, 1].min(), full_line_pixels[:, 1].max()
+            minX, maxX = (
+                full_line_pixels[:, 0].min(),
+                full_line_pixels[:, 0].max(),
+            )
+            minY, maxY = (
+                full_line_pixels[:, 1].min(),
+                full_line_pixels[:, 1].max(),
+            )
             # Determine the sorting order based on the comparison of ranges
             if maxX - minX > maxY - minY:
                 # If range of x is greater, sort by x-coordinate
-                full_line_pixels = full_line_pixels[full_line_pixels[:, 0].argsort()]
+                full_line_pixels = full_line_pixels[
+                    full_line_pixels[:, 0].argsort()
+                ]
             else:
                 # Otherwise, sort by y-coordinate
-                full_line_pixels = full_line_pixels[full_line_pixels[:, 1].argsort()]
+                full_line_pixels = full_line_pixels[
+                    full_line_pixels[:, 1].argsort()
+                ]
 
             full_line_pixels = np.around(full_line_pixels).astype(int)
             refined_pixels.append(full_line_pixels)
 
             if len(missing_points_adjusted) > 0:
                 for pixel in missing_points_adjusted:
                     pt = tuple(int(coordinate) for coordinate in pixel)
-                    cv2.circle(bg, pt, 2, (0, 255, 255), -1)  
-                    
+                    cv2.circle(bg, pt, 2, (0, 255, 255), -1)
+
         return bg, refined_pixels
-    
+
     def _refine_pixels(self, bg, lines, line_pixels):
         """Refine the pixel coordinates fitting into lines based on the line models.
-    
+
         Args:
             bg (numpy.ndarray): Background image.
             lines (list): List of line models.
             line_pixels (list): List of pixel coordinates for each line.
-            
+
         Returns:
             tuple: (bg, lines, refined_pixels)
                 - bg (numpy.ndarray): Background image with refined pixels drawn.
                 - lines (list): List of line models.
                 - refined_pixels (list): List of refined pixel coordinates for each line.
         """
         refined_pixels = []
-        
+
         for line_model, pixels in zip(lines, line_pixels):
             origin, direction = line_model.params[0], line_model.params[1]
-            # Draw
-            point1 = tuple((origin + -2000 * direction).astype(int))  # Extend the line
-            point2 = tuple((origin + 2000 * direction).astype(int))  # Extend the line
-            cv2.line(bg, point1, point2, (0, 0, 255), 1) 
+            # Extend the line
+            point1 = tuple((origin + -2000 * direction).astype(int))  
+            point2 = tuple((origin + 2000 * direction).astype(int))
+            cv2.line(bg, point1, point2, (0, 0, 255), 1)
             pixels = np.array(pixels)
             to_pixels = pixels - origin
-            proj_lengths = np.dot(to_pixels, direction) / np.linalg.norm(direction)**2
+            proj_lengths = (
+                np.dot(to_pixels, direction) / np.linalg.norm(direction) ** 2
+            )
             proj_points = np.outer(proj_lengths, direction) + origin
 
             proj_points = np.round(proj_points).astype(int)
             refined_pixels.append(proj_points)
 
         # Draw
         for refined_pixels_per_line in refined_pixels:
             for pixel in refined_pixels_per_line:
-                    pt = tuple(pixel)
-                    cv2.circle(bg, pt, 3, (255, 0, 0), -1)
-        #cv2.imwrite("debug/refined_pixels.jpg", bg)
+                pt = tuple(pixel)
+                cv2.circle(bg, pt, 3, (255, 0, 0), -1)
+        # cv2.imwrite("debug/refined_pixels.jpg", bg)
         return bg, lines, refined_pixels
 
     def get_reticle_zone(self, img):
         """Get the reticle zone from the image.
-    
+
         Args:
             img (numpy.ndarray): Input image.
-            
+
         Returns:
             numpy.ndarray or None: Reticle zone image if reticle exists, None otherwise.
         """
         bg = self._preprocess_image(img)
         bg = cv2.resize(bg, self.image_size)
         masked = self._apply_mask(bg)
         if self.reticle_frame_detector.is_reticle_exist:
             ret, bg, _, pixels_in_lines = self.coords_detect_morph(bg)
             return self._draw_reticle_lines(bg, pixels_in_lines)
         else:
             return None
-    
+
     def coords_detect_morph(self, img):
         """
-        Applies morphological operations and adaptive thresholding 
-        to detect coordinates in an image. 
+        Applies morphological operations and adaptive thresholding
+        to detect coordinates in an image.
         """
         img_color = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
-        if img.shape == (3000,4000):
-            img = cv2.adaptiveThreshold(img, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY, 13, 2)
+        if img.shape == (3000, 4000):
+            img = cv2.adaptiveThreshold(
+                img,
+                255,
+                cv2.ADAPTIVE_THRESH_GAUSSIAN_C,
+                cv2.THRESH_BINARY,
+                13,
+                2,
+            )
         else:
-            img = cv2.adaptiveThreshold(img, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY, 11, 3)
+            img = cv2.adaptiveThreshold(
+                img,
+                255,
+                cv2.ADAPTIVE_THRESH_GAUSSIAN_C,
+                cv2.THRESH_BINARY,
+                11,
+                3,
+            )
         img = cv2.medianBlur(img, 5)
         img = cv2.bitwise_not(img, mask=self.mask)
-        kernel_ellipse_5 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE,(5,5))
-        kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE,(3,3))
+        kernel_ellipse_5 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (5, 5))
+        kernel_ellipse_3 = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (3, 3))
         img = cv2.morphologyEx(img, cv2.MORPH_CLOSE, kernel_ellipse_5)
 
         img = self._eroding(img)
-        #cv2.imwrite("debug/after_eroding.jpg", img)
+        # cv2.imwrite("debug/after_eroding.jpg", img)
         ret, inliner_lines, inliner_lines_pixels = self._ransac_detect_lines(img)
         logger.debug(f"n of inliner lines: {len(inliner_lines_pixels)}")
-        
+
         # Draw
         for inliner_lines_pixel in inliner_lines_pixels:
             for pixel in inliner_lines_pixel:
-                    pt = tuple(pixel)
-                    cv2.circle(img_color, pt, 1, (0, 255, 0), -1)  
-        #cv2.imwrite("debug/inliner_pixels.jpg", img_color)
-        
+                pt = tuple(pixel)
+                cv2.circle(img_color, pt, 1, (0, 255, 0), -1)
+        # cv2.imwrite("debug/inliner_pixels.jpg", img_color)
+
         return ret, img, inliner_lines, inliner_lines_pixels
-    
+
     def get_coords(self, img):
         """Detect coordinates using morphological operations.
-    
+
         Args:
             img (numpy.ndarray): Input image.
-            
+
         Returns:
             tuple: (ret, img, inliner_lines, inliner_lines_pixels)
                 - ret (bool): True if coordinates are detected, False otherwise.
                 - img (numpy.ndarray): Processed image.
                 - inliner_lines (list): List of inlier line models.
                 - inliner_lines_pixels (list): List of inlier pixel coordinates for each line.
         """
         bg = self._preprocess_image(img)
         masked = self._apply_mask(bg)
 
-        #if self.mask is not None:
+        # if self.mask is not None:
         #    cv2.imwrite("debug/mask.jpg", self.mask)
 
         if self.reticle_frame_detector.is_reticle_exist:
             ret, bg, inliner_lines, pixels_in_lines = self.coords_detect_morph(bg)
             logger.debug(f"{self.name} nLines: {len(pixels_in_lines)}")
             if ret:
                 bg, inliner_lines, pixels_in_lines = self._refine_pixels(bg, inliner_lines, pixels_in_lines)
                 logger.debug(f"{self.name} detect: {len(pixels_in_lines[0])}, {len(pixels_in_lines[1])}" )
                 bg, pixels_in_lines = self._add_missing_pixels(bg, inliner_lines, pixels_in_lines)
                 logger.debug(f"{self.name} interpolate: {len(pixels_in_lines[0])} {len(pixels_in_lines[1])}")
-                #cv2.imwrite("debug/added_missing_points.jpg", bg)
+                # cv2.imwrite("debug/added_missing_points.jpg", bg)
             return ret, bg, inliner_lines, pixels_in_lines
-        
+
         return False, bg, None, None
 
     """
     def is_distance_tip_reticle_threshold(self, probe, reticle, thresh=10):
         tip_x, tip_y = probe["tip_coords"]
         dist_transform = cv2.distanceTransform(reticle, cv2.DIST_L2, cv2.DIST_MASK_PRECISE)
         # Get the distance at the tip location
```

### Comparing `parallax_app-0.37.0/parallax/reticle_detection_coords_interests.py` & `parallax_app-0.37.1/parallax/reticle_detection_coords_interests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 
 """
 Provides functionality to detect and analyze points of interest on reticle lines in images, 
 employing line fitting and orientation determination techniques suitable 
 for microscopy image analysis tasks.
 """
-from scipy.stats import linregress
-from PyQt5.QtCore import QObject
-import numpy as np
+
 import logging
 
+import numpy as np
+from PyQt5.QtCore import QObject
+from scipy.stats import linregress
+
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class ReticleDetectCoordsInterest(QObject):
     """Class for detecting coordinates of interest in reticle lines."""
+
     def __init__(self):
-        """ Initialize object """
+        """Initialize object"""
         self.n_interest_pixels = 15
         pass
-    
+
     def _fit_line(self, pixels):
         """Fit a line to the given pixels.
 
         Args:
             pixels (list): List of pixel coordinates.
 
         Returns:
@@ -56,86 +60,86 @@
         # Calculate intersection point
         x_intersect = (intercept2 - intercept1) / (slope1 - slope2)
         y_intersect = slope1 * x_intersect + intercept1
         return int(round(x_intersect)), int(round(y_intersect))
 
     def _get_center_coords_index(self, center, coords):
         """Get the index of the center coordinates in the given coordinates.
-        
+
         Args:
             center (tuple): Center coordinates.
             coords (numpy.ndarray): Array of coordinates.
-            
+
         Returns:
             int or None: Index of the center coordinates if found, None otherwise.
         """
         x_center, y_center = center
         for i in range(-5, 6):  # Range from -5 to 5
             for j in range(-5, 6):  # Range from -5 to 5
                 test_center = np.array([x_center + i, y_center + j])
                 result = np.where((coords == test_center).all(axis=1))
                 if len(result[0]) > 0:  # Check if the element was found
                     return result[0][0]  # Return the first occurrence index
         return None
 
     def _get_pixels_interest(self, center, coords):
         """Get the pixels of interest around the center coordinates.
-        
+
         Args:
             center (tuple): Center coordinates.
             coords (numpy.ndarray): Array of coordinates.
-            
+
         Returns:
             numpy.ndarray or None: Pixels of interest if found, None otherwise.
         """
         center_index = self._get_center_coords_index(center, coords)
         if center_index is None:
             return
-        
-        coords[center_index] = center # Replace center to center point we gets
+
+        coords[center_index] = center  # Replace center to center point we gets
         start_index = max(center_index - self.n_interest_pixels, 0)
         end_index = min(center_index + self.n_interest_pixels + 1, len(coords))
         return coords[start_index:end_index]
 
     def _get_orientation(self, pixels_in_lines):
         """Get the orientation of the reticle lines.
-        
+
         Args:
             pixels_in_lines (list): List of pixel lines.
-            
+
         Returns:
             tuple: (ret, x_axis, y_axis)
                 - ret (bool): True if orientation is determined, False otherwise.
                 - x_axis (numpy.ndarray): X-axis coordinates.
                 - y_axis (numpy.ndarray): Y-axis coordinates.
         """
-        if pixels_in_lines[0] is None or pixels_in_lines[1] is None: 
+        if pixels_in_lines[0] is None or pixels_in_lines[1] is None:
             logger.error("One of the pixel lines is None. Cannot proceed with orientation calculation.")
             return False, None, None
 
-        # Temp solution: first coords of X axis is left side to first coords of Y axis. 
+        # Temp solution: first coords of X axis is left side to first coords of Y axis.
         min_x_value_line0 = min(pixels_in_lines[0], key=lambda x: x[0])
         min_x_value_line1 = min(pixels_in_lines[1], key=lambda x: x[0])
-        #print(min_x_value_line0, min_x_value_line1)
+        # print(min_x_value_line0, min_x_value_line1)
         if min_x_value_line0[0] < min_x_value_line1[0]:
             x_axis, y_axis = pixels_in_lines[0], pixels_in_lines[1]
-        else: 
+        else:
             x_axis, y_axis = pixels_in_lines[1], pixels_in_lines[0]
-        
+
         # Sort by ascending order
         x_axis = x_axis[np.argsort(x_axis[:, 0])]
         y_axis = y_axis[np.argsort(-y_axis[:, 1])]
         return True, x_axis, y_axis
-    
+
     def get_coords_interest(self, pixels_in_lines):
         """Get the coordinates of interest from the pixel lines.
-        
+
         Args:
             pixels_in_lines (list): List of pixel lines.
-            
+
         Returns:
             tuple: (ret, x_axis, y_axis)
                 - ret (bool): True if coordinates of interest are found, False otherwise.
                 - x_axis (numpy.ndarray): X-axis coordinates.
                 - y_axis (numpy.ndarray): Y-axis coordinates.
         """
         if len(pixels_in_lines) != 2:
@@ -153,15 +157,15 @@
         line1 = self._fit_line(pixels_in_lines[0])
         line2 = self._fit_line(pixels_in_lines[1])
         center_point = self._find_intersection(line1, line2)
         logger.debug(f"center_point: {center_point}")
 
         for pixels_in_line in pixels_in_lines:
             coords = self._get_pixels_interest(center_point, pixels_in_line)
-            if coords is None or len(coords) < self.n_interest_pixels*2 + 1:
+            if coords is None or len(coords) < self.n_interest_pixels * 2 + 1:
                 return False, None, None
             coords_interest.append(coords)
 
         ret, x_axis, y_axis = self._get_orientation(coords_interest)
         if ret is False:
             return False, None, None
         return True, x_axis, y_axis
```

### Comparing `parallax_app-0.37.0/parallax/screen_widget.py` & `parallax_app-0.37.1/parallax/screen_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 
 """
 Provides ScreenWidget for image interaction in microscopy apps, supporting image display, 
 point selection, and zooming. It integrates with probe and reticle detection managers 
 for real-time processing and offers camera control functions.
 """
-from PyQt5.QtCore import pyqtSignal, Qt
+
+import logging
+
+import cv2
+import pyqtgraph as pg
 from PyQt5 import QtCore
+from PyQt5.QtCore import Qt, pyqtSignal
+
+from .no_filter import NoFilter
 from .probe_detect_manager import ProbeDetectManager
 from .reticle_detect_manager import ReticleDetectManager
-from .no_filter import NoFilter
-import pyqtgraph as pg
-import cv2
-import logging
 
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class ScreenWidget(pg.GraphicsView):
-    """ Screens Class """
+    """Screens Class"""
+
     selected = pyqtSignal(int, int)
     cleared = pyqtSignal()
     reticle_coords_detected = pyqtSignal()
     probe_coords_detected = pyqtSignal()
 
     def __init__(self, camera, filename=None, model=None, parent=None):
-        """ Init screen widget object """
+        """Init screen widget object"""
         super().__init__(parent=parent)
         self.filename = filename
         self.model = model
 
         self.view_box = pg.ViewBox(defaultPadding=0)
         self.setCentralItem(self.view_box)
         self.view_box.setAspectLocked()
         self.view_box.invertY()
 
         self.image_item = ClickableImage()
-        self.image_item.axisOrder = 'row-major'
+        self.image_item.axisOrder = "row-major"
         self.view_box.addItem(self.image_item)
         self.image_item.mouse_clicked.connect(self.image_clicked)
 
         self.click_target = pg.TargetItem()
         self.view_box.addItem(self.click_target)
         self.click_target.setVisible(False)
 
@@ -70,22 +75,26 @@
 
         # No filter
         self.filter = NoFilter()
         self.filter.frame_processed.connect(self.set_image_item_from_data)
 
         # Reticle Detection
         self.reticleDetector = ReticleDetectManager(camera_name)
-        self.reticleDetector.frame_processed.connect(self.set_image_item_from_data)
+        self.reticleDetector.frame_processed.connect(
+            self.set_image_item_from_data
+        )
         self.reticleDetector.found_coords.connect(self.found_reticle_coords)
         self.reticleDetector.found_coords.connect(self.reticle_coords_detected)
 
         # Probe Detection
-        self.probeDetector = ProbeDetectManager(self.model.stages, camera_name)
+        self.probeDetector = ProbeDetectManager(self.model, camera_name)
         self.model.add_probe_detector(self.probeDetector)
-        self.probeDetector.frame_processed.connect(self.set_image_item_from_data)
+        self.probeDetector.frame_processed.connect(
+            self.set_image_item_from_data
+        )
         self.probeDetector.found_coords.connect(self.found_probe_coords)
         self.probeDetector.found_coords.connect(self.probe_coords_detected)
 
         if self.filename:
             self.set_data(cv2.imread(filename, cv2.IMREAD_GRAYSCALE))
 
     def refresh(self):
@@ -98,15 +107,15 @@
 
     def start_acquisition_camera(self):
         """
         Start the camera acquisition. (Continuously)
         """
         if self.camera:
             self.camera.begin_continuous_acquisition()
-    
+
     def stop_acquisition_camera(self):
         """
         Stop the camera acquisition. (Continuously)
         """
         if self.camera:
             self.camera.stop(clean=False)
 
@@ -120,80 +129,80 @@
 
     def single_acquisition_camera(self):
         """
         Start the camera acquisition. (Single Frame)
         """
         if self.camera:
             self.camera.begin_singleframe_acquisition()
-    
+
     def stop_single_acquisition_camera(self):
         """
         Stop the camera acquisition. (Single Frame)
         """
         if self.camera:
             self.camera.end_singleframe_acquisition()
 
     def set_data(self, data):
         """
         Set the data displayed in the screen widget.
         """
         self.filter.process(data)
         self.reticleDetector.process(data)
-        captured_time = self.camera.get_last_capture_time(millisecond=True) #TODO
+        captured_time = self.camera.get_last_capture_time(millisecond=True)
         self.probeDetector.process(data, captured_time)
-    
+
     def is_camera(self):
         """
         Return True if the camera is 'Blackfly' camera.
         """
         camera_name = self.camera.name(sn_only=False)
         return True if "Blackfly" in camera_name else False
 
     def get_camera_name(self):
         """
         Return the name of the camera.
         """
-        return self.camera.name(sn_only=True) if self.camera else None 
+        return self.camera.name(sn_only=True) if self.camera else None
 
     def clear_selected(self):
         """
         Clear the selected target.
         """
         self.click_target.setVisible(False)
         self.cleared.emit()
 
     def save_image(self, filepath, isTimestamp=False, name="Microscope_"):
         """
         Save the image displayed in the screen widget.
         """
         if self.camera:
             self.camera.save_last_image(filepath, isTimestamp, name)
-            
+
     def save_recording(self, filepath, isTimestamp=False, name="Microscope_"):
         """
-        Save the recording frames that are displayed from camera. 
+        Save the recording frames that are displayed from camera.
         """
         if self.camera:
             self.camera.save_recording(filepath, isTimestamp, name)
-    
+
     def stop_recording(self):
         """
         Stop the recording.
         """
         if self.camera:
             self.camera.stop_recording()
 
     def set_image_item_from_data(self, data):
-        """ display image from data """
+        """display image from data"""
         self.image_item.setImage(data, autoLevels=False)
 
     def set_camera_setting(self, setting, val):
         """
         Set the camera settings. (exposure, gain, gamma, wb)
-        
+
         exposure (int): min: 90,000(10fps) max: 250,000(4fps)
         gain (float): The desired gain value. min:0, max:27.0
         wb (float): The desired white balance value. min:1.8, max:2.5
         gamma (float): The desired gamma value. min:0.25 max:1.25
         """
         if self.camera:
             if setting == "exposure":
@@ -202,22 +211,22 @@
                 self.camera.set_gain(val)
             elif setting == "gamma":
                 self.camera.set_gamma(val)
             elif setting == "wbRed":
                 self.camera.set_wb("Red", val)
             elif setting == "wbBlue":
                 self.camera.set_wb("Blue", val)
-        
+
     def get_camera_setting(self, setting):
         """Get the specified camera setting value.
-    
+
         Args:
-            setting (str): The camera setting to retrieve. 
+            setting (str): The camera setting to retrieve.
                 Possible values: "exposure", "gain", "gamma", "wbRed", "wbBlue".
-        
+
         Returns:
             float: The value of the specified camera setting.
         """
         val = 0
         if self.camera:
             if setting == "exposure":
                 val = self.camera.get_exposure()
@@ -229,28 +238,28 @@
                 val = self.camera.get_wb("Red")
             elif setting == "wbBlue":
                 val = self.camera.get_wb("Blue")
         return val
 
     def get_camera_color_type(self):
         """Get the color type of the camera.
-    
+
         Returns:
             str: The color type of the camera.
         """
         if self.camera:
             return self.camera.device_color_type
 
     def image_clicked(self, event):
         """
         Handle the image click event.
         """
-        if event.button() == QtCore.Qt.MouseButton.LeftButton:            
+        if event.button() == QtCore.Qt.MouseButton.LeftButton:
             self.select(event.pos())
-        elif event.button() == QtCore.Qt.MouseButton.MiddleButton:            
+        elif event.button() == QtCore.Qt.MouseButton.MiddleButton:
             self.zoom_out()
 
     def select(self, pos):
         """Select a position and emit the selected coordinates."""
         self.click_target.setPos(pos)
         self.click_target.setVisible(True)
         self.selected.emit(*self.get_selected())
@@ -274,21 +283,21 @@
         self.reticleDetector.set_name(self.get_camera_name())
 
     def run_reticle_detection(self):
         """Run reticle detection by stopping the filter and starting the reticle detector."""
         logger.debug("run_reticle_detection")
         self.filter.stop()
         self.reticleDetector.start()
-    
+
     def run_probe_detection(self):
         """Run probe detection by stopping the filter and starting the probe detector."""
         logger.debug("run_probe_detection")
         self.filter.stop()
         self.probeDetector.start()
-    
+
     def run_no_filter(self):
         """Run without any filter by stopping the reticle detector and probe detector."""
         logger.debug("run_no_filter")
         self.reticleDetector.stop()
         self.probeDetector.stop()
         self.filter.start()
 
@@ -307,22 +316,24 @@
         self.probe_detect_last_timestamp = timestamp
         self.probe_detect_last_sn = probe_sn
         self.stage_info = stage_info
         self.probe_detect_last_coords = tip_coords
 
     def get_last_detect_probe_info(self):
         """Get the last detected probe information."""
-        return self.probe_detect_last_timestamp, \
-                self.probe_detect_last_sn, \
-                self.probe_detect_last_coords
+        return (
+            self.probe_detect_last_timestamp,
+            self.probe_detect_last_sn,
+            self.probe_detect_last_coords,
+        )
 
     def get_camera_intrinsic(self):
         """Get the camera intrinsic parameters."""
         return self.mtx, self.dist
-    
+
     def get_reticle_coords(self):
         """Get the reticle coordinates."""
         return self.reticle_coords
 
     def get_selected(self):
         """
         Return the selected target position.
@@ -344,16 +355,19 @@
             if self.focochan:
                 foco, chan = self.focochan
                 dist = 20 if shift else 100
                 foco.time_move(chan, forward, dist, wait=True)
         else:
             super().wheelEvent(e)
 
+
 class ClickableImage(pg.ImageItem):
-    """ This class captures mouse click events on images. """
+    """This class captures mouse click events on images."""
+
     mouse_clicked = pyqtSignal(object)
+
     def mouseClickEvent(self, ev):
         """
         Handle the mouse click event.
         """
         super().mouseClickEvent(ev)
         self.mouse_clicked.emit(ev)
```

### Comparing `parallax_app-0.37.0/parallax/stage_listener.py` & `parallax_app-0.37.1/parallax/stage_listener.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """
 Provides classes to manage stage data fetching, representation, and updates in microscopy 
 applications, using PyQt5 for threading and signals, and requests for HTTP requests.
 """
-from PyQt5.QtCore import QObject, pyqtSignal, QThread, QTimer
-from datetime import datetime
+
+import logging
+import time
 from collections import deque
+from datetime import datetime
+
 import numpy as np
 import requests
-import time
-import logging
+from PyQt5.QtCore import QObject, QThread, QTimer, pyqtSignal
 
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class StageInfo(QObject):
     """Class for retrieving stage information."""
+
     def __init__(self, url):
-        """ Initialize StageInfo thread """
+        """Initialize StageInfo thread"""
         super().__init__()
         self.url = url
         self.nStages = 0
         self.stages_sn = []
 
     def get_instances(self):
         """Get the instances of the stages.
-        
+
         Returns:
             list: List of stage instances.
         """
         stages = []
         try:
             response = requests.get(self.url, timeout=5)
             if response.status_code == 200:
@@ -44,56 +48,60 @@
                     stages.append(stage)
         except Exception as e:
             print(f"\nHttpServer for stages not enabled: {e}")
             print("* Trouble Shooting: ")
             print("1. Check New Scale Stage connection.")
             print("2. Enable Http Server: 'http://localhost:8080/'")
             print("3. Click 'Connect' on New Scale SW")
-        
+
         return stages
 
+
 class Stage(QObject):
     """Class representing a stage."""
-    def __init__(self, stage_info = None):
-        """ Initialize Stage thread """
+
+    def __init__(self, stage_info=None):
+        """Initialize Stage thread"""
         QObject.__init__(self)
         if stage_info is not None:
             self.sn = stage_info["SerialNumber"]
             self.name = stage_info["Id"]
-            self.stage_x = stage_info["Stage_X"]*1000
-            self.stage_y = stage_info["Stage_Y"]*1000
-            self.stage_z = stage_info["Stage_Z"]*1000
+            self.stage_x = stage_info["Stage_X"] * 1000
+            self.stage_y = stage_info["Stage_Y"] * 1000
+            self.stage_z = stage_info["Stage_Z"] * 1000
             self.stage_x_global = None
             self.stage_y_global = None
             self.stage_z_global = None
 
+
 class Worker(QObject):
     """Worker class for fetching stage data."""
+
     dataChanged = pyqtSignal(dict)
     stage_moving = pyqtSignal(dict)
     stage_not_moving = pyqtSignal(dict)
 
     def __init__(self, url):
-        """ Initialize worker thread """
+        """Initialize worker thread"""
         super().__init__()
         self.url = url
         self.timer = QTimer()
         self.timer.timeout.connect(self.fetchData)
         self.last_stage_info = None
         self.last_bigmove_stage_info = None
         self.last_bigmove_detected_time = None
         self._low_freq_interval = 1000
-        self._high_freq_interval = 10    # TODO
+        self._high_freq_interval = 10  # TODO
         self.curr_interval = self._low_freq_interval
         self._idle_time = 2
         self.is_error_log_printed = False
-        
+
     def start(self, interval=1000):
         """Start the worker thread.
-        
+
         Args:
             interval (int): Interval in milliseconds. Defaults to 1000.
         """
         self.timer.start(interval)
 
     def stop(self):
         """Stop the timer."""
@@ -105,35 +113,35 @@
         print("1. Check New Scale Stage connection.")
         print("2. Enable Http Server: 'http://localhost:8080/'")
         print("3. Click 'Connect' on New Scale SW")
 
     def fetchData(self):
         """Fetches content from the URL and checks for significant changes."""
         try:
-            response = requests.get(self.url, timeout=1)        
-            if response.status_code == 200:   
+            response = requests.get(self.url, timeout=1)
+            if response.status_code == 200:
                 data = response.json()
                 if data["Probes"] == 0:
                     if self.is_error_log_printed == False:
                         self.is_error_log_printed = True
                         print("\nStage is not connected to New Scale SW")
                         self.print_trouble_shooting_msg()
                 else:
                     selected_probe = data["SelectedProbe"]
-                    probe = data["ProbeArray"][selected_probe]  
+                    probe = data["ProbeArray"][selected_probe]
 
-                    if self.last_stage_info is None: # Initial 
+                    if self.last_stage_info is None:  # Initial
                         self.last_stage_info = probe
                         self.last_bigmove_stage_info = probe
                         self.dataChanged.emit(probe)
 
                     if self.curr_interval == self._high_freq_interval:
                         # Update
                         self.isSmallChange(probe)
-                        # If last updated move (in 30um) is more than 1 sec ago, swith to w/ low freq
+                        # If last updated move (in 30um) is more than 1 sec ago, switch to w/ low freq
                         current_time = time.time()
                         if current_time - self.last_bigmove_detected_time >= self._idle_time:
                             logger.debug("low freq mode")
                             self.curr_interval = self._low_freq_interval
                             self.stop()
                             self.start(interval=self.curr_interval)
                             self.stage_not_moving.emit(probe)
@@ -161,113 +169,131 @@
         """Check if the change in any axis exceeds the threshold."""
         for axis in ['Stage_X', 'Stage_Y', 'Stage_Z']:
             if abs(current_stage_info[axis] - self.last_bigmove_stage_info[axis]) >= stage_threshold:
                 self.last_bigmove_detected_time = time.time()
                 self.last_bigmove_stage_info = current_stage_info
                 return True
         return False
-    
+
     def isSmallChange(self, current_stage_info, stage_threshold=0.0005):
         """Check if the change in any axis exceeds the threshold."""
         for axis in ['Stage_X', 'Stage_Y', 'Stage_Z']:
             if abs(current_stage_info[axis] - self.last_stage_info[axis]) >= stage_threshold:
                 self.dataChanged.emit(current_stage_info)
                 self.last_stage_info = current_stage_info
                 return True
         return False
 
+
 class StageListener(QObject):
     """Class for listening to stage updates."""
+
     probeCalibRequest = pyqtSignal(QObject)
+
     def __init__(self, model, stage_ui):
-        """ Initialize Stage Listener object """
+        """Initialize Stage Listener object"""
         super().__init__()
         self.model = model
         self.timestamp_local, self.timestamp_img_captured = None, None
         self.worker = Worker(self.model.stage_listener_url)
         self.thread = QThread()
         self.stage_ui = stage_ui
         self.thread.started.connect(self.worker.start)
         self.worker.dataChanged.connect(self.handleDataChange)
         self.worker.stage_moving.connect(self.stageMovingStatus)
         self.worker.stage_not_moving.connect(self.stageNotMovingStatus)
         self.buffer_size = 20
         self.buffer_ts_local_coords = deque(maxlen=self.buffer_size)
         self.stage_global_data = None
         self.transM_dict = {}
-    
+
     def start(self):
         """Start the stage listener."""
         if self.model.nStages != 0:
             self.worker.moveToThread(self.thread)
             self.thread.start()
 
     def get_last_moved_time(self, millisecond=False):
         """Get the last moved time of the stage.
-        
+
         Args:
             millisecond (bool): Include milliseconds in the timestamp. Defaults to False.
-            
+
         Returns:
             str: Last moved time as a string.
         """
         ts = time.time()
         dt = datetime.fromtimestamp(ts)
         if millisecond:
-            return '%04d%02d%02d-%02d%02d%02d.%03d' % (dt.year, dt.month, dt.day,
-                        dt.hour, dt.minute, dt.second, dt.microsecond // 1000)
+            return "%04d%02d%02d-%02d%02d%02d.%03d" % (
+                dt.year,
+                dt.month,
+                dt.day,
+                dt.hour,
+                dt.minute,
+                dt.second,
+                dt.microsecond // 1000,
+            )
         else:
-            return '%04d%02d%02d-%02d%02d%02d' % (dt.year, dt.month, dt.day,
-                                              dt.hour, dt.minute, dt.second)
-        
+            return "%04d%02d%02d-%02d%02d%02d" % (
+                dt.year,
+                dt.month,
+                dt.day,
+                dt.hour,
+                dt.minute,
+                dt.second,
+            )
+
     def append_to_buffer(self, ts, stage):
         """Append stage data to the buffer.
-        
+
         Args:
             ts (str): Timestamp.
             stage (Stage): Stage object.
         """
-        self.buffer_ts_local_coords.append((ts, [stage.stage_x, stage.stage_y, stage.stage_z]))
+        self.buffer_ts_local_coords.append(
+            (ts, [stage.stage_x, stage.stage_y, stage.stage_z])
+        )
 
     def handleDataChange(self, probe):
         """Handle changes in stage data.
-        
+
         Args:
             probe (dict): Probe data.
         """
         # Format the current timestamp
         self.timestamp_local = self.get_last_moved_time(millisecond=True)
-        
-        id = probe['Id']
-        sn = probe['SerialNumber']
-        local_coords_x = round(probe['Stage_X']*1000, 1)
-        local_coords_y = round(probe['Stage_Y']*1000, 1)
-        local_coords_z = round(probe['Stage_Z']*1000, 1)
+
+        id = probe["Id"]
+        sn = probe["SerialNumber"]
+        local_coords_x = round(probe["Stage_X"] * 1000, 1)
+        local_coords_y = round(probe["Stage_Y"] * 1000, 1)
+        local_coords_z = round(probe["Stage_Z"] * 1000, 1)
 
         # update into model
         moving_stage = self.model.stages.get(sn)
-        
+
         if moving_stage is not None:
             moving_stage.stage_x = local_coords_x
             moving_stage.stage_y = local_coords_y
             moving_stage.stage_z = local_coords_z
 
         # Update to buffer
         self.append_to_buffer(self.timestamp_local, moving_stage)
 
         # Update into UI
         if self.stage_ui.get_selected_stage_sn() == sn:
             self.stage_ui.updateStageLocalCoords()
-        #logger.debug(sn, moving_stage.stage_x, self.stage_ui.get_selected_stage_sn())
+        # logger.debug(sn, moving_stage.stage_x, self.stage_ui.get_selected_stage_sn())
 
         if sn in self.transM_dict:
             transM = self.transM_dict[sn]
             if transM is not None:
                 self._updateGlobalDataTransformM(sn, moving_stage, transM)
-            
+
     def _updateGlobalDataTransformM(self, sn, moving_stage, transM):
         """
         Applies a transformation matrix to the local coordinates of a moving stage and updates its global coordinates.
 
         Args:
             sn (str): The serial number of the moving stage.
             moving_stage (Stage): An object representing the moving stage, with attributes for its local and global coordinates.
@@ -275,40 +301,47 @@
                                 to global coordinates.
 
         Effects:
             - Updates the moving_stage object's `stage_x_global`, `stage_y_global`, and `stage_z_global` attributes with the
             transformed global coordinates.
             - If the moving stage is the currently selected stage in the UI, triggers an update of the global coordinates display.
         """
-         # Transform
-        local_point = np.array([moving_stage.stage_x, moving_stage.stage_y, moving_stage.stage_z, 1])
+        # Transform
+        local_point = np.array(
+            [
+                moving_stage.stage_x,
+                moving_stage.stage_y,
+                moving_stage.stage_z,
+                1,
+            ]
+        )
         global_point = np.dot(transM, local_point)
-        global_point =  np.around(global_point[:3], decimals=1)
+        global_point = np.around(global_point[:3], decimals=1)
         logger.debug(f"_updateGlobalDataTransformM: {sn}, {global_point}")
 
         # Update into UI
         moving_stage.stage_x_global = global_point[0]
         moving_stage.stage_y_global = global_point[1]
         moving_stage.stage_z_global = global_point[2]
         if self.stage_ui.get_selected_stage_sn() == sn:
             self.stage_ui.updateStageGlobalCoords()
-    
+
     def requestUpdateGlobalDataTransformM(self, sn, transM):
         """
         Stores or updates a transformation matrix for a specific stage identified by its serial number.
         This method updates an internal dictionary, `transM_dict`, mapping stage serial numbers to their
         corresponding transformation matrices.
 
         Args:
             sn (str): The serial number of the stage.
             transM (np.ndarray): A 4x4 numpy array representing the transformation matrix for the specified stage.
         """
         self.transM_dict[sn] = transM
         logger.debug(f"requestUpdateGlobalDataTransformM {sn} {transM}")
-        
+
     def requestClearGlobalDataTransformM(self):
         """
         Clears all stored transformation matrices and resets the UI to default global coordinates.
 
         Effects:
             - Clears `transM_dict`, removing all stored transformation matrices.
             - Triggers a UI update to reset the display of global coordinates to default values.
@@ -321,25 +354,25 @@
         """Change the time format from string to datetime."""
         fmt = "%Y%m%d-%H%M%S.%f"
         date_time = datetime.strptime(str_time, fmt)
         return date_time
 
     def _find_closest_local_coords(self):
         """Find the closest local coordinates based on the image capture timestamp.
-        
+
         Returns:
             tuple: (closest_ts, closest_coords)
                 - closest_ts (str): Closest timestamp.
                 - closest_coords (list): Closest local coordinates.
         """
         closest_ts = None
         closest_coords = None
         # Initialize a variable to track the smallest time difference
         # Use a large initial value
-        smallest_time_diff = float('inf')
+        smallest_time_diff = float("inf")
 
         for ts, local_coords in self.buffer_ts_local_coords:
             ts_datetime = self._change_time_format(ts)
             time_diff = (self.ts_img_captured - ts_datetime).total_seconds()
 
             if time_diff < 0:
                 break
@@ -350,70 +383,72 @@
                 closest_ts = ts
                 closest_coords = local_coords
 
         return closest_ts, closest_coords
 
     def handleGlobalDataChange(self, sn, global_coords, ts_img_captured):
         """Handle changes in global stage data.
-        
+
         Args:
             sn (str): Serial number of the stage.
             coords (list): Global coordinates.
             ts_img_captured (str): Timestamp of the captured image.
         """
         self.ts_img_captured = self._change_time_format(ts_img_captured)
         ts_local_coords, local_coords = self._find_closest_local_coords()
 
-        logger.debug(f"\ntimestamp local:{ts_local_coords} img_captured:{ts_img_captured}" )
-        global_coords_x = round(global_coords[0][0]*1000, 1)
-        global_coords_y = round(global_coords[0][1]*1000, 1)
-        global_coords_z = round(global_coords[0][2]*1000, 1)
-        
+        logger.debug(
+            f"\ntimestamp local:{ts_local_coords} img_captured:{ts_img_captured}"
+        )
+        global_coords_x = round(global_coords[0][0] * 1000, 1)
+        global_coords_y = round(global_coords[0][1] * 1000, 1)
+        global_coords_z = round(global_coords[0][2] * 1000, 1)
+
         if self.stage_global_data is None:
             stage_info = {}
             stage_info["SerialNumber"] = sn
             stage_info["Id"] = None
-            stage_info['Stage_X'] =  local_coords[0]
-            stage_info['Stage_Y'] =  local_coords[1]
-            stage_info['Stage_Z'] =  local_coords[2]
+            stage_info["Stage_X"] = local_coords[0]
+            stage_info["Stage_Y"] = local_coords[1]
+            stage_info["Stage_Z"] = local_coords[2]
             self.stage_global_data = Stage(stage_info)
-        
+
         if local_coords is not None:
             self.sn = sn
             self.stage_global_data.sn = sn
-            self.stage_global_data.stage_x =  local_coords[0]
-            self.stage_global_data.stage_y =  local_coords[1]
-            self.stage_global_data.stage_z =  local_coords[2]
+            self.stage_global_data.stage_x = local_coords[0]
+            self.stage_global_data.stage_y = local_coords[1]
+            self.stage_global_data.stage_z = local_coords[2]
             self.stage_global_data.stage_x_global = global_coords_x
             self.stage_global_data.stage_y_global = global_coords_y
             self.stage_global_data.stage_z_global = global_coords_z
-            
+
             self.probeCalibRequest.emit(self.stage_global_data)
-        
+
             # Update into UI
             moving_stage = self.model.stages.get(sn)
             if moving_stage is not None:
                 moving_stage.stage_x_global = global_coords_x
                 moving_stage.stage_y_global = global_coords_y
                 moving_stage.stage_z_global = global_coords_z
             if self.stage_ui.get_selected_stage_sn() == sn:
                 self.stage_ui.updateStageGlobalCoords()
 
     def stageMovingStatus(self, probe):
         """Handle stage moving status.
-        
+
         Args:
             probe (dict): Probe data.
         """
-        sn = probe['SerialNumber']
+        sn = probe["SerialNumber"]
         for probeDetector in self.model.probeDetectors:
             probeDetector.start_detection(sn)
 
     def stageNotMovingStatus(self, probe):
         """Handle not moving probe status.
-        
+
         Args:
             probe (dict): Probe data.
         """
-        sn = probe['SerialNumber']
+        sn = probe["SerialNumber"]
         for probeDetector in self.model.probeDetectors:
             probeDetector.stop_detection(sn)
```

### Comparing `parallax_app-0.37.0/parallax/stage_ui.py` & `parallax_app-0.37.1/parallax/stage_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,71 @@
 """
 Defines StageUI, a PyQt5 QWidget for showing and updating stage information in the UI, 
 including serial numbers and coordinates. It interacts with the model to reflect 
 real-time data changes.
 """
+
 from PyQt5.QtWidgets import QWidget
 
+
 class StageUI(QWidget):
     """User interface for stage control and display."""
+
     def __init__(self, model, parent=None):
-        """ Initialize StageUI object """
+        """Initialize StageUI object"""
         QWidget.__init__(self, parent)
         self.selected_stage = None
         self.model = model
         self.ui = parent
         self.update_stage_selector()
         self.updateStageSN()
         self.updateStageLocalCoords()
         self.updateStageGlobalCoords()
 
         self.ui.stage_selector.currentIndexChanged.connect(self.updateStageSN)
-        self.ui.stage_selector.currentIndexChanged.connect(self.updateStageLocalCoords)
-        self.ui.stage_selector.currentIndexChanged.connect(self.updateStageGlobalCoords)
+        self.ui.stage_selector.currentIndexChanged.connect(
+            self.updateStageLocalCoords
+        )
+        self.ui.stage_selector.currentIndexChanged.connect(
+            self.updateStageGlobalCoords
+        )
 
     def get_selected_stage_sn(self):
         """Get the serial number of the selected stage.
-        
+
         Returns:
             str or None: The serial number of the selected stage, or None if no stage is selected.
         """
         if self.selected_stage is not None:
             return self.selected_stage.sn
         return None
 
     def update_stage_selector(self):
         """Update the stage selector with available stages."""
         self.ui.stage_selector.clear()
         for stage in self.model.stages.keys():
             self.ui.stage_selector.addItem("Probe " + stage, stage)
-            
+
     def _get_current_stage_id(self):
         """Get the ID of the currently selected stage.
-        
+
         Returns:
             str or None: The ID of the currently selected stage, or None if no stage is selected.
         """
         currentIndex = self.ui.stage_selector.currentIndex()
         stage_id = self.ui.stage_selector.itemData(currentIndex)
         return stage_id
-        
+
     def updateStageSN(self):
         """Update the displayed stage serial number."""
         stage_id = self._get_current_stage_id()
         if stage_id:
             self.selected_stage = self.model.stages.get(stage_id)
             if self.selected_stage:
-                self.ui.stage_sn.setText(" "+self.selected_stage.sn)
+                self.ui.stage_sn.setText(" " + self.selected_stage.sn)
 
     def updateStageLocalCoords(self):
         """Update the displayed local coordinates of the selected stage."""
         stage_id = self._get_current_stage_id()
         if stage_id:
             self.selected_stage = self.model.stages.get(stage_id)
             if self.selected_stage:
@@ -71,23 +78,29 @@
         stage_id = self._get_current_stage_id()
         if stage_id:
             self.selected_stage = self.model.stages.get(stage_id)
             if self.selected_stage:
                 if self.selected_stage.stage_x_global is not None \
                 and self.selected_stage.stage_y_global is not None \
                 and self.selected_stage.stage_z_global is not None:
-                    self.ui.global_coords_x.setText(str(self.selected_stage.stage_x_global))
-                    self.ui.global_coords_y.setText(str(self.selected_stage.stage_y_global))
-                    self.ui.global_coords_z.setText(str(self.selected_stage.stage_z_global))
+                    self.ui.global_coords_x.setText(
+                        str(self.selected_stage.stage_x_global)
+                    )
+                    self.ui.global_coords_y.setText(
+                        str(self.selected_stage.stage_y_global)
+                    )
+                    self.ui.global_coords_z.setText(
+                        str(self.selected_stage.stage_z_global)
+                    )
                 else:
-                    self.updateStageGlobalCoords_default()              
+                    self.updateStageGlobalCoords_default()
 
     def updateStageGlobalCoords_default(self):
         """
         Resets the global coordinates displayed in the UI to default placeholders.
 
         This method is used to clear the display of global coordinates in the user interface,
         setting them back to a default placeholder value ('-').
         """
-        self.ui.global_coords_x.setText('-')
-        self.ui.global_coords_y.setText('-')
-        self.ui.global_coords_z.setText('-')    
+        self.ui.global_coords_x.setText("-")
+        self.ui.global_coords_y.setText("-")
+        self.ui.global_coords_z.setText("-")
```

### Comparing `parallax_app-0.37.0/parallax/stage_widget.py` & `parallax_app-0.37.1/parallax/stage_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 """
 This module contains the StageWidget class, which is a PyQt5 QWidget subclass for controlling 
 and calibrating stages in microscopy instruments. It interacts with the application's model 
 to manage calibration data and provides UI functionalities for reticle and probe detection, 
 and camera calibration. The class integrates with PyQt5 for the UI, handling UI loading, 
 initializing components, and linking user actions to calibration processes.
 """
-from PyQt5.QtWidgets import QWidget, QMessageBox, QPushButton, QLabel, QSpacerItem, QSizePolicy
-from PyQt5.uic import loadUi
+
+import logging
+import os
+
+import numpy as np
 from PyQt5.QtCore import QTimer
-from .stage_listener import StageListener
-from .probe_calibration import ProbeCalibration
+from PyQt5.QtWidgets import (QLabel, QMessageBox, QPushButton, QSizePolicy,
+                             QSpacerItem, QWidget)
+from PyQt5.uic import loadUi
+
 from .calibration_camera import CalibrationStereo
+from .probe_calibration import ProbeCalibration
+from .stage_listener import StageListener
 from .stage_ui import StageUI
-import os
-import logging
-import  numpy as np
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 
+
 class StageWidget(QWidget):
     """Widget for stage control and calibration."""
+
     def __init__(self, model, ui_dir, screen_widgets):
-        """ Initializes the StageWidget instance. 
+        """Initializes the StageWidget instance.
 
         Parameters:
             model: The data model used for storing calibration and stage information.
             ui_dir (str): The directory path where UI files are located.
             screen_widgets (list): A list of ScreenWidget instances for reticle and probe detection.
         """
         super().__init__()
         self.model = model
         self.screen_widgets = screen_widgets
         loadUi(os.path.join(ui_dir, "stage_info.ui"), self)
         self.setMaximumWidth(380)
-                
+
         # Load reticle_calib.ui into its placeholder
         self.reticle_calib_widget = QWidget()  # Create a new widget
         loadUi(os.path.join(ui_dir, "reticle_calib.ui"), self.reticle_calib_widget)
         # Assuming reticleCalibPlaceholder is the name of an empty widget designated as a placeholder in your stage_info.ui
         self.stage_status_ui.layout().addWidget(self.reticle_calib_widget)  # Add it to the placeholder's layout
         self.reticle_calib_widget.setMinimumSize(0, 160)
 
@@ -51,55 +57,80 @@
         
         # Create a vertical spacer with expanding policy
         spacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
         # Add the spacer to the layout
         self.stage_status_ui.addItem(spacer)
 
         # Access probe_calibration_btn
-        self.probe_calibration_btn = self.probe_calib_widget.findChild(QPushButton, "probe_calibration_btn")
-        self.reticle_calibration_btn = self.reticle_calib_widget.findChild(QPushButton, "reticle_calibration_btn")
-        self.acceptButton = self.reticle_calib_widget.findChild(QPushButton, "acceptButton")
-        self.rejectButton = self.reticle_calib_widget.findChild(QPushButton, "rejectButton")
-        self.reticleCalibrationLabel = self.reticle_calib_widget.findChild(QLabel, "reticleCalibResultLabel")
+        self.probe_calibration_btn = self.probe_calib_widget.findChild(
+            QPushButton, "probe_calibration_btn"
+        )
+        self.reticle_calibration_btn = self.reticle_calib_widget.findChild(
+            QPushButton, "reticle_calibration_btn"
+        )
+        self.acceptButton = self.reticle_calib_widget.findChild(
+            QPushButton, "acceptButton"
+        )
+        self.rejectButton = self.reticle_calib_widget.findChild(
+            QPushButton, "rejectButton"
+        )
+        self.reticleCalibrationLabel = self.reticle_calib_widget.findChild(
+            QLabel, "reticleCalibResultLabel"
+        )
         self.calib_x = self.probe_calib_widget.findChild(QPushButton, "calib_x")
         self.calib_y = self.probe_calib_widget.findChild(QPushButton, "calib_y")
         self.calib_z = self.probe_calib_widget.findChild(QPushButton, "calib_z")
-        self.probeCalibrationLabel = self.probe_calib_widget.findChild(QLabel, "probeCalibrationLabel")
+        self.probeCalibrationLabel = self.probe_calib_widget.findChild(
+            QLabel, "probeCalibrationLabel"
+        )
 
         # Reticle Widget
-        self.reticle_detection_status = None    # options: default, process, detected, accepted
-        self.reticle_calibration_btn.clicked.connect(self.reticle_detection_button_handler)
+        self.reticle_detection_status = (
+            None  # options: default, process, detected, accepted
+        )
+        self.reticle_calibration_btn.clicked.connect(
+            self.reticle_detection_button_handler
+        )
         self.calibrationStereo = None
         # Hide Accept and Reject Button in Reticle Detection
-        self.acceptButton.hide() 
-        self.rejectButton.hide() 
-        self.acceptButton.clicked.connect(self.reticle_detect_accept_detected_status)
+        self.acceptButton.hide()
+        self.rejectButton.hide()
+        self.acceptButton.clicked.connect(
+            self.reticle_detect_accept_detected_status
+        )
         self.rejectButton.clicked.connect(self.reticle_detect_default_status)
         # Add a QTimer for delayed check
         self.reticle_calibration_timer = QTimer(self)
-        self.reticle_calibration_timer.timeout.connect(self.reticle_detect_default_status)
-        
+        self.reticle_calibration_timer.timeout.connect(
+            self.reticle_detect_default_status
+        )
+
         # Stage widget
         self.stageUI = StageUI(self.model, self)
         self.probe_calibration_btn.setEnabled(False)
-        self.probe_calibration_btn.clicked.connect(self.probe_detection_button_handler)
-        #self.probe_calibration_btn.clicked.connect(self.probe_detection_button_handler) 
+        self.probe_calibration_btn.clicked.connect(
+            self.probe_detection_button_handler
+        )
         # Start refreshing stage info
         self.stageListener = StageListener(self.model, self.stageUI)
         self.stageListener.start()
         self.probeCalibration = ProbeCalibration(self.stageListener)
         # Hide X, Y, and Z Buttons in Probe Detection
-        self.calib_x.hide() 
+        self.calib_x.hide()
         self.calib_y.hide()
         self.calib_z.hide()
         self.probeCalibration.calib_complete_x.connect(self.calib_x_complete)
         self.probeCalibration.calib_complete_y.connect(self.calib_y_complete)
         self.probeCalibration.calib_complete_z.connect(self.calib_z_complete)
-        self.probeCalibration.calib_complete.connect(self.probe_detect_accepted_status)
-        self.probeCalibration.transM_info.connect(self.update_probe_calib_status)
+        self.probeCalibration.calib_complete.connect(
+            self.probe_detect_accepted_status
+        )
+        self.probeCalibration.transM_info.connect(
+            self.update_probe_calib_status
+        )
         self.calib_status_x, self.calib_status_y, self.calib_status_z = False, False, False
         self.probe_detection_status = None    # options: default, process, x_y_z_detected, accepted
 
         self.filter = "no_filter"
 
     def reticle_detection_button_handler(self):
         """
@@ -110,113 +141,127 @@
             # Run reticle detectoin
             self.reticle_detect_process_status()
         else:
             if self.reticle_detection_status == "accepted":
                 response = self.overwrite_popup_window()
                 if response:
                     # Overwrite the result
-                    self.reticle_detect_default_status()    
+                    self.reticle_detect_default_status()
                 else:
                     # Keep the last calibration result
                     self.reticle_calibration_btn.setChecked(True)
-    
+
     def reticle_detect_default_status(self):
         """
         Resets the reticle detection process to its default state and updates the UI accordingly.
         """
         # Enable reticle_calibration_btn button
         if not self.reticle_calibration_btn.isEnabled():
             self.reticle_calibration_btn.setEnabled(True)
 
         if self.reticle_detection_status == "process":
             self.reticle_detect_fail_popup_window()
-            
+
         # Stop reticle detectoin, and run no filter
         self.reticle_calibration_timer.stop()
 
         if self.reticle_detection_status != "accepted":
             for screen in self.screen_widgets:
-                screen.reticle_coords_detected.disconnect(self.reticle_detect_all_screen)
+                screen.reticle_coords_detected.disconnect(
+                    self.reticle_detect_all_screen
+                )
                 screen.run_no_filter()
             self.filter = "no_filter"
 
         # Hide Accept and Reject Button
-        self.acceptButton.hide() 
-        self.rejectButton.hide() 
-        
-        self.reticle_calibration_btn.setStyleSheet("""
+        self.acceptButton.hide()
+        self.rejectButton.hide()
+
+        self.reticle_calibration_btn.setStyleSheet(
+            """
             QPushButton {
                 color: white;
                 background-color: black;
             }
             QPushButton:hover {
                 background-color: #641e1e;
             }
         """)
         self.reticle_detection_status = "default"
         self.reticleCalibrationLabel.setText("")
-        if self.probe_calibration_btn.isEnabled():        
+        if self.probe_calibration_btn.isEnabled():
             # Disable probe calibration
             self.probe_detect_default_status()
 
     def overwrite_popup_window(self):
         """
         Displays a confirmation dialog to decide whether to overwrite the current reticle position.
-        
+
         Returns:
             bool: True if the user chooses to overwrite, False otherwise.
         """
-        message = f"Are you sure you want to overwrite the current reticle position?"
-        response = QMessageBox.warning(self, "Reticle Detection Failed", message, 
-                            QMessageBox.Yes | QMessageBox.No, QMessageBox.No)
-        
+        message = (
+            f"Are you sure you want to overwrite the current reticle position?"
+        )
+        response = QMessageBox.warning(
+            self,
+            "Reticle Detection Failed",
+            message,
+            QMessageBox.Yes | QMessageBox.No,
+            QMessageBox.No,
+        )
+
         # Check which button was clicked
         if response == QMessageBox.Yes:
             logger.debug("User clicked Yes.")
             return True
         else:
             logger.debug("User clicked No.")
             return False
-    
+
     def reticle_detect_fail_popup_window(self):
         """
         Displays a warning dialog indicating the failure of reticle detection on one or more cameras.
         """
         coords_detect_fail_cameras = []
         for screen in self.screen_widgets:
             coords = screen.get_reticle_coords()
             if coords is None:
                 camera_name = screen.get_camera_name()
                 coords_detect_fail_cameras.append(camera_name)
 
-        message = f"No reticle detected on cameras: {coords_detect_fail_cameras}"
+        message = (
+            f"No reticle detected on cameras: {coords_detect_fail_cameras}"
+        )
         QMessageBox.warning(self, "Reticle Detection Failed", message)
 
     def reticle_detect_process_status(self):
         """
         Updates the UI and internal state to reflect that the reticle detection process is underway.
         """
         # Disable reticle_calibration_btn button
         if self.reticle_calibration_btn.isEnabled():
             self.reticle_calibration_btn.setEnabled(False)
-        
+
         # Run reticle detectoin
         self.reticle_calibration_btn.setStyleSheet(
             "color: gray;"
             "background-color: #ffaaaa;"
         )
         for screen in self.screen_widgets:
-            screen.reset_reticle_coords()  
-            screen.reticle_coords_detected.connect(self.reticle_detect_all_screen)
+            screen.reset_reticle_coords()
+            screen.reticle_coords_detected.connect(
+                self.reticle_detect_all_screen
+            )
             screen.run_reticle_detection()
         self.filter = "reticle_detection"
 
         # Hide Accept and Reject Button
-        self.acceptButton.hide() 
-        self.rejectButton.hide() 
+        self.acceptButton.hide()
+        self.rejectButton.hide()
 
         # Start the timer for 10 seconds to check the status later
         self.reticle_detection_status = "process"
         self.reticle_calibration_timer.start(10000)
         logger.debug(self.reticle_detection_status)
 
     def reticle_detect_detected_status(self):
@@ -224,108 +269,121 @@
         Updates the UI and internal state to reflect that the reticle has been detected.
         """
         # Found the coords
         self.reticle_detection_status = "detected"
         self.reticle_calibration_timer.stop()
 
         # Show Accept and Reject Button
-        self.acceptButton.show() 
-        self.rejectButton.show() 
+        self.acceptButton.show()
+        self.rejectButton.show()
 
         # Change the button to brown.
         self.reticle_calibration_btn.setStyleSheet(
             "color: white;"
             "background-color: #bc9e44;"
         )
 
     def reticle_detect_accept_detected_status(self):
         """
         Finalizes the reticle detection process, accepting the detected reticle position and updating the UI accordingly.
         """
         self.reticle_detection_status = "accepted"
-        
+
         # Change the button to green.
         self.reticle_calibration_btn.setStyleSheet(
             "color: white;"
             "background-color: #84c083;"
         )
         # Show Accept and Reject Button
-        self.acceptButton.hide() 
-        self.rejectButton.hide() 
+        self.acceptButton.hide()
+        self.rejectButton.hide()
 
         result = self.calibrate_stereo()
         if result:
             self.reticleCalibrationLabel.setText(
                 f"<span style='color:green;'><small>Coords Reproj RMSE:<br></small>"
                 f"<span style='color:green;'>{result*1000:.1f} µm³</span>"
             )
 
         for screen in self.screen_widgets:
-            screen.reticle_coords_detected.disconnect(self.reticle_detect_all_screen)
+            screen.reticle_coords_detected.disconnect(
+                self.reticle_detect_all_screen
+            )
             screen.run_no_filter()
         self.filter = "no_filter"
 
         # Enable reticle_calibration_btn button
         if not self.reticle_calibration_btn.isEnabled():
             self.reticle_calibration_btn.setEnabled(True)
         logger.debug(self.reticle_detection_status)
 
         # Enable probe calibration
-        if not self.probe_calibration_btn.isEnabled():   
+        if not self.probe_calibration_btn.isEnabled():
             self.probe_calibration_btn.setEnabled(True)
 
     def calibrate_stereo(self):
         """
         Performs stereo calibration using the detected reticle positions and updates the model with the calibration data.
         """
         # Streo Camera Calibration
         if len(self.model.coords_axis) >=2 and len(self.model.camera_intrinsic) >=2:
             img_coords = []
             intrinsics = []
             cam_names = []
-            
-            for screen in self.screen_widgets: 
+
+            for screen in self.screen_widgets:
                 camera_name = screen.get_camera_name()
                 cam_names.append(camera_name)
                 img_coords.append(self.model.get_coords_axis(camera_name))
                 intrinsics.append(self.model.get_camera_intrinsic(camera_name))
 
             if len(intrinsics) >= 2:
                 print("\n== intrinsics ==")
                 print(f" cam {cam_names[0]}:\n  {intrinsics[0]}")
                 print(f" cam {cam_names[1]}:\n  {intrinsics[1]}")
 
-            # TODO 
-            self.calibrationStereo = CalibrationStereo(cam_names[0], img_coords[0], intrinsics[0], \
-                                                    cam_names[1], img_coords[1], intrinsics[1])
-            retval, R_AB, T_AB, E_AB, F_AB = self.calibrationStereo.calibrate_stereo()
-            self.model.add_camera_extrinsic(cam_names[0], cam_names[1], retval, R_AB, T_AB, E_AB, F_AB)
+            # TODO
+            self.calibrationStereo = CalibrationStereo(
+                cam_names[0],
+                img_coords[0],
+                intrinsics[0],
+                cam_names[1],
+                img_coords[1],
+                intrinsics[1],
+            )
+            retval, R_AB, T_AB, E_AB, F_AB = (
+                self.calibrationStereo.calibrate_stereo()
+            )
+            self.model.add_camera_extrinsic(
+                cam_names[0], cam_names[1], retval, R_AB, T_AB, E_AB, F_AB
+            )
 
             # Test
-            err = self.calibrationStereo.test_performance(cam_names[0], img_coords[0], cam_names[1], img_coords[1])
+            err = self.calibrationStereo.test_performance(
+                cam_names[0], img_coords[0], cam_names[1], img_coords[1]
+            )
             return err
         else:
             return None
 
-         
     def reticle_detect_all_screen(self):
         """
         Checks all screens for reticle detection results and updates the status based on whether the reticle
         has been detected on all screens.
         """
         """Detect reticle coordinates on all screens."""
         for screen in self.screen_widgets:
             coords = screen.get_reticle_coords()
             if coords is None:
                 return
-        
+
         # Found the coords
         self.reticle_detect_detected_status()
 
-        #self.reticle_calibration_btn.setText("Confirm ?")
+        # self.reticle_calibration_btn.setText("Confirm ?")
         for screen in self.screen_widgets:
             coords = screen.get_reticle_coords()
             mtx, dist = screen.get_camera_intrinsic()
             camera_name = screen.get_camera_name()
             # Retister the reticle coords in the model
             self.model.add_coords_axis(camera_name, coords)
             self.model.add_camera_intrinsic(camera_name, mtx, dist)
@@ -334,53 +392,62 @@
         """Detect probe coordinates on all screens."""
         timestamp_cmp, sn_cmp = None, None
         cam_names = []
         tip_coords = []
 
         if self.calibrationStereo is None:
             print("Camera calibration has not done")
-            return 
+            return
 
         for screen in self.screen_widgets:
             timestamp, sn, tip_coord = screen.get_last_detect_probe_info()
-            
+
             if (sn is None) or (tip_coords is None) or (timestamp is None):
                 return
 
             if timestamp_cmp is None:
-                timestamp_cmp = timestamp    
-            else: # if timestamp is different between screens, return
+                timestamp_cmp = timestamp
+            else:  # if timestamp is different between screens, return
                 if timestamp_cmp[:-2] != timestamp[:-2]:
                     return
 
             if sn_cmp is None:
                 sn_cmp = sn
-            else: # if sn is different between screens, return
+            else:  # if sn is different between screens, return
                 if sn_cmp != sn:
                     return
-            
+
             camera_name = screen.get_camera_name()
             cam_names.append(camera_name)
             tip_coords.append(tip_coord)
 
         # All screen has the same timestamp. Proceed the triangulation
-        global_coords = self.calibrationStereo.get_global_coords(cam_names[0], tip_coords[0], cam_names[1], tip_coords[1])
+        global_coords = self.calibrationStereo.get_global_coords(
+            cam_names[0], tip_coords[0], cam_names[1], tip_coords[1]
+        )
         self.stageListener.handleGlobalDataChange(sn, global_coords, timestamp)
 
     def probe_overwrite_popup_window(self):
         """
         Displays a confirmation dialog asking the user if they want to overwrite the current probe position.
 
         Returns:
             bool: True if the user confirms the overwrite, False otherwise.
         """
-        message = f"Are you sure you want to overwrite the current probe position?"
-        response = QMessageBox.warning(self, "Reticle Detection Failed", message, 
-                            QMessageBox.Yes | QMessageBox.No, QMessageBox.No)
-        
+        message = (
+            f"Are you sure you want to overwrite the current probe position?"
+        )
+        response = QMessageBox.warning(
+            self,
+            "Reticle Detection Failed",
+            message,
+            QMessageBox.Yes | QMessageBox.No,
+            QMessageBox.No,
+        )
+
         # Check which button was clicked
         if response == QMessageBox.Yes:
             logger.debug("User clicked Yes.")
             return True
         else:
             logger.debug("User clicked No.")
             return False
@@ -411,35 +478,37 @@
             QPushButton:hover {
                 background-color: #641e1e;
             }
         """)
         self.hide_x_y_z()
         self.probeCalibrationLabel.setText("")
         self.probeCalibration.reset_calib()
-        #self.reset_calib_status()
+        # self.reset_calib_status()
 
         self.probe_calibration_btn.setChecked(False)
         if self.reticle_detection_status == "default":
             self.probe_calibration_btn.setEnabled(False)
-        
+
         if self.filter == "probe_detection":
             for screen in self.screen_widgets:
-                screen.probe_coords_detected.disconnect(self.probe_detect_all_screen)
+                screen.probe_coords_detected.disconnect(
+                    self.probe_detect_all_screen
+                )
                 screen.run_no_filter()
 
             self.filter = "no_filter"
             self.probeCalibration.clear()
 
         # update global coords
         self.stageListener.requestClearGlobalDataTransformM()
-        
-    def probe_detect_process_status(self): 
+
+    def probe_detect_process_status(self):
         """
         Updates the UI and internal state to reflect that the probe detection process is underway.
-        """   
+        """
         self.probe_detection_status = "process"
         self.probe_calibration_btn.setStyleSheet(
             "color: white;"
             "background-color: #bc9e44;"
         )
         self.calib_x.show()
         self.calib_y.show()
@@ -447,15 +516,15 @@
 
         for screen in self.screen_widgets:
             screen.probe_coords_detected.connect(self.probe_detect_all_screen)
             screen.run_probe_detection()
         self.filter = "probe_detection"
 
         # message
-        message = f"Move probe at leas 20 mm along X, Y, and Z axes"
+        message = f"Move probe at least 2mm along X, Y, and Z axes"
         QMessageBox.information(self, "Probe calibration info", message)
 
     def probe_detect_accepted_status(self, stage_sn, transformation_matrix):
         """
         Finalizes the probe detection process, accepting the detected probe position and updating the UI accordingly.
         Additionally, it updates the model with the transformation matrix obtained from the calibration.
 
@@ -467,22 +536,26 @@
         self.probe_calibration_btn.setStyleSheet(
             "color: white;"
             "background-color: #84c083;"
         )
         self.hide_x_y_z()
         if self.filter == "probe_detection":
             for screen in self.screen_widgets:
-                screen.probe_coords_detected.disconnect(self.probe_detect_all_screen)
+                screen.probe_coords_detected.disconnect(
+                    self.probe_detect_all_screen
+                )
                 screen.run_no_filter()
 
             self.filter = "no_filter"
 
         # update global coords
-        self.stageListener.requestUpdateGlobalDataTransformM(stage_sn, transformation_matrix)
-        
+        self.stageListener.requestUpdateGlobalDataTransformM(
+            stage_sn, transformation_matrix
+        )
+
     def hide_x_y_z(self):
         """
         Hides the X, Y, and Z calibration buttons and updates their styles to indicate that the calibration for
         each axis has been completed.
         """
         if self.calib_x.isVisible():
             self.calib_x.hide()
@@ -523,31 +596,33 @@
         """
         if self.calib_y.isVisible():
             # Change the button to green.
             self.calib_y.setStyleSheet(
             "color: white;"
             "background-color: #84c083;"
         )
-            
+
+
     def calib_z_complete(self):
         """
         Updates the UI to indicate that the calibration for the Z-axis is complete.
         """
         if self.calib_z.isVisible():
             # Change the button to green.
             self.calib_z.setStyleSheet(
             "color: white;"
             "background-color: #84c083;"
         )
+
     def update_probe_calib_status_transM(self, transformation_matrix):
         # Extract the rotation matrix (top-left 3x3)
         R = transformation_matrix[:3, :3]
         # Extract the translation vector (top 3 elements of the last column)
         T = transformation_matrix[:3, 3]
-                
+
         # Set the formatted string as the label's text
         content = (
             f"<span style='color:yellow;'><small>"
             f"[Transformation Matrix]<br></small></span>"
             f"<span style='color:green;'><small><b>R:</b><br>"
             f" {R[0][0]:.5f}, {R[0][1]:.5f}, {R[0][2]:.5f},<br>"
             f" {R[1][0]:.5f}, {R[1][1]:.5f}, {R[1][2]:.5f},<br>"
@@ -580,8 +655,7 @@
         content_transM = self.update_probe_calib_status_transM(transformation_matrix)
         content_L2 = self.update_probe_calib_status_L2(L2_err)
         content_L2_travel = self.update_probe_calib_status_distance_traveled(dist_traveled)
         # Ensure HTML content is properly combined
         full_content = content_transM + content_L2 + content_L2_travel
 
         self.probeCalibrationLabel.setText(full_content)
-
```

### Comparing `parallax_app-0.37.0/parallax/user_setting_manager.py` & `parallax_app-0.37.1/parallax/user_setting_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,50 +7,54 @@
 - Logging of operational messages for error handling and debugging.
 
 Example:
     settings_manager = UserSettingsManager()
     nColumn, directory, width, height = settings_manager.load_mainWindow_settings()
     settings_manager.save_user_configs(nColumn, directory, width, height)
 """
-from .screen_widget import ScreenWidget
+
 import json
-import os
 import logging
+import os
+
+from .screen_widget import ScreenWidget
 
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
-# Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
+# Set the logging level for PyQt5.uic.uiparser/properties
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
+
 class UserSettingsManager:
-    " UserSettingsManager class"
+    "UserSettingsManager class"
+
     def __init__(self):
         """
         Initialize the UserSettingsManager by setting the path to the settings file.
         The settings file is located in the 'ui' directory. The settings are
         loaded upon initialization.
         """
         package_dir = os.path.dirname(os.path.abspath(__file__))
-        ui_dir = os.path.join(os.path.dirname(package_dir), 'ui')
-        settings_file = os.path.join(ui_dir, 'settings.json')
+        ui_dir = os.path.join(os.path.dirname(package_dir), "ui")
+        settings_file = os.path.join(ui_dir, "settings.json")
         self.settings_file = settings_file
         self.settings = self.load_settings()
 
     def load_settings(self):
         """
         Load user settings from a JSON file specified by self.settings_file.
 
         Returns:
             dict: A dictionary containing the loaded settings. Returns an empty
             dictionary if the settings file does not exist or cannot be read.
         """
         if os.path.exists(self.settings_file):
-            with open(self.settings_file, 'r') as file:
+            with open(self.settings_file, "r") as file:
                 return json.load(file)
         return {}
 
     def save_user_configs(self, nColumn, directory, width, height):
         """
         Save user configurations to the settings JSON file.
 
@@ -61,26 +65,26 @@
             height (int): The height of the main window.
 
         This method updates the settings with the provided configurations and saves them
         back to the JSON file.
         """
         # Read current settings from file
         if os.path.exists(self.settings_file):
-            with open(self.settings_file, 'r') as file:
+            with open(self.settings_file, "r") as file:
                 settings = json.load(file)
         else:
             settings = {}
 
         settings["main"] = {
             "nColumn": nColumn,
             "directory": directory,
             "width": width,
-            "height":height,  
+            "height": height,
         }
-        with open(self.settings_file, 'w') as file:
+        with open(self.settings_file, "w") as file:
             json.dump(settings, file)
 
     def load_mainWindow_settings(self):
         """
         Load settings for the main window from the settings JSON file.
 
         Returns:
@@ -107,26 +111,30 @@
             category (str): The category of settings to retrieve.
             item (Optional[str]): The specific item to retrieve from the category. If None, all items in the category are returned.
 
         Returns:
             The requested settings item(s). Returns None if the category or item does not exist.
         """
         if os.path.exists(self.settings_file):
-            with open(self.settings_file, 'r') as file:
+            with open(self.settings_file, "r") as file:
                 settings = json.load(file)
                 if category in settings:
                     if item is not None:
                         if item in settings[category]:
                             return settings[category][item]
                         else:
-                            logger.debug(f"load_settings_item: Item '{item}' not found in settings.")
+                            logger.debug(
+                                f"load_settings_item: Item '{item}' not found in settings."
+                            )
                             return None
                     return settings[category]
                 else:
-                    logger.debug(f"load_settings_item: Section '{category}' not found in settings.")
+                    logger.debug(
+                        f"load_settings_item: Section '{category}' not found in settings."
+                    )
                     return None
         else:
             logger.debug("load_settings_item: Settings file not found.")
             return None
 
     def update_user_configs_settingMenu(self, microscopeGrp, item, val):
         """
@@ -141,25 +149,25 @@
         the camera's serial number, and updates the setting specified by 'item' with the new value
         'val' in the settings JSON file.
         """
 
         # Find the screen within this microscopeGrp
         screen = microscopeGrp.findChild(ScreenWidget, "Screen")
 
-        # Display the S/N of camera 
+        # Display the S/N of camera
         sn = screen.get_camera_name()
 
         # Read current settings from file
         if os.path.exists(self.settings_file):
-            with open(self.settings_file, 'r') as file:
+            with open(self.settings_file, "r") as file:
                 settings = json.load(file)
         else:
             settings = {}
 
         # Update settings with values from the settingMenu of current screen
         if sn not in settings:
             settings[sn] = {}
         settings[sn][item] = val
 
         # Write updated settings back to file
-        with open(self.settings_file, 'w') as file:
+        with open(self.settings_file, "w") as file:
             json.dump(settings, file)
```

### Comparing `parallax_app-0.37.0/parallax/utils.py` & `parallax_app-0.37.1/parallax/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 This module provides utility classes for manipulating coordinates and calculating
 crop regions within images. 
 - UtilsCoords: scaling coordinates between original and resized images
 - UtilsCrops: calculating crop regions based on specified criteria.
 """
 
+
 class UtilsCoords:
     """Utility class for coordinate scaling."""
+
     def __init__(self, original_size, resized_size):
         """Initialize the UtilsCoords object.
 
         Args:
             original_size (tuple): Original size of the image (width, height).
             resized_size (tuple): Resized size of the image (width, height).
         """
@@ -34,16 +36,18 @@
         scale_y = original_height / resized_height
 
         original_x = int(x * scale_x)
         original_y = int(y * scale_y)
 
         return original_x, original_y
 
+
 class UtilsCrops:
     """Utility class for calculating crop regions."""
+
     def __init__(self):
         """Initialize the UtilsCrops object."""
         pass
 
     def calculate_crop_region(self, tip, base, crop_size, IMG_SIZE):
         """Calculate the crop region based on tip and base coordinates.
 
@@ -75,11 +79,13 @@
             right (int): Right coordinate of the crop region.
             buffer (int): Buffer size around the crop region boundary. Defaults to 5.
 
         Returns:
             bool: True if the point is on the crop region boundary, False otherwise.
         """
         x, y = point
-        return (top - buffer <= y <= top + buffer) or \
-               (bottom - buffer <= y <= bottom + buffer) or \
-               (left - buffer <= x <= left + buffer) or \
-               (right - buffer <= x <= right + buffer)
+        return (
+            (top - buffer <= y <= top + buffer)
+            or (bottom - buffer <= y <= bottom + buffer)
+            or (left - buffer <= x <= left + buffer)
+            or (right - buffer <= x <= right + buffer)
+        )
```

### Comparing `parallax_app-0.37.0/parallax_app.egg-info/PKG-INFO` & `parallax_app-0.37.1/parallax_app.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallax-app
-Version: 0.37.0
+Version: 0.37.1
 Summary: GUI software for photogrammetry-assisted probe targeting in electrophysiology
 Author-email: Hanna Lee <hanna.lee@alleninstitute.org>
 License: Allen Institute Software License
 Keywords: parallax
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
@@ -15,20 +15,23 @@
 Requires-Dist: opencv-python
 Requires-Dist: spinnaker-python
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: scikit-image
 Requires-Dist: requests
 Requires-Dist: scikit-learn
+Provides-Extra: dev
+Requires-Dist: parallax-app[linters]; extra == "dev"
 Provides-Extra: linters
 Requires-Dist: codespell; extra == "linters"
 Requires-Dist: coverage; extra == "linters"
 Requires-Dist: flake8; extra == "linters"
 Requires-Dist: interrogate; extra == "linters"
 Requires-Dist: isort; extra == "linters"
+Requires-Dist: pytest-mock; extra == "linters"
 Provides-Extra: docs
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-jinja; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 
 # Parallax
 
@@ -39,41 +42,60 @@
 
 ### Prerequisites
 - Python~=3.8 (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
 - PySpin (for Linux or Mac OS users)
 
 
 ### Installation
-1. Clone the repository:
-```bash
-git clone https://github.com/AllenNeuralDynamics/parallax.git
-```
-
-2. Create virtual environment and activate it:
+1. Create virtual environment and activate it:
 - On Windows:
 ```bash
 python -m venv venv
 ./venv/Scripts/activate
 ```
 - On Linux/Mac:
 ```bash
 python -m venv venv
 source venv/bin/activate
 ```
 
-3. Install Dependencies:
+2. To install the latest version:
 ```bash
-python -m pip install -e .
+pip install parallax-app
+```
+To upgrate to the latest version:
+```bash
+pip install parallax-app --upgrade
 ```
 
 ### Running Parallax
 ```bash
 python -m parallax
 ```
 
+### Development mode
+1. Clone the repository:
+```bash
+git clone https://github.com/AllenNeuralDynamics/parallax.git
+```
+2. Install Dependencies:
+```bash
+pip install -e .[dev]
+```
+
+### Documentation
+1. To install the dependencies:
+```bash
+pip install -e .[docs]
+```
+2. Then to create the documentation html files, run:
+```bash
+sphinx-build -b html docs/ docs/_build
+```
+
 ### Additional Setup for Linux and Mac OS
 For Linux or Mac OS, you'll need to install PySpin manually (not required for
 Windows):
 * download the Spinnaker SDK package for your system from [here](https://flir.app.boxcn.net/v/SpinnakerSDK)
 * follow the installation instructions in the README
 * Install the Python bindings found alongside the SDK package
```

### Comparing `parallax_app-0.37.0/parallax_app.egg-info/SOURCES.txt` & `parallax_app-0.37.1/parallax_app.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 .gitignore
+.readthedocs.yaml
 LICENSE
 README.md
 pyproject.toml
 setup.py
 docs/Makefile
 docs/ReadMe.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/modules.rst
 docs/parallax.rst
+docs/requirements.txt
 img/arrow-right.png
 img/gear.png
 img/recordingButton.png
 img/sextant.png
 img/snapshotButton_white.png
 img/stop-sign.png
 img/target.png
@@ -42,17 +44,17 @@
 parallax/user_setting_manager.py
 parallax/utils.py
 parallax_app.egg-info/PKG-INFO
 parallax_app.egg-info/SOURCES.txt
 parallax_app.egg-info/dependency_links.txt
 parallax_app.egg-info/requires.txt
 parallax_app.egg-info/top_level.txt
-tests/camera.py
-tests/model.py
-tests/screen_widget.py
+tests/test_camera.py
+tests/test_model.py
+tests/test_screen_widget.py
 ui/ParallaxReadME.JPG
 ui/mainWindow.ui
 ui/probe_calib.ui
 ui/reticle_calib.ui
 ui/settingPopUpMenu.ui
 ui/stage_info.ui
 ui/font/FiraCode-VariableFont_wght.ttf
```

### Comparing `parallax_app-0.37.0/pyproject.toml` & `parallax_app-0.37.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -52,37 +52,59 @@
 00000330: 6c73 2e64 796e 616d 6963 5d0d 0a76 6572  ls.dynamic]..ver
 00000340: 7369 6f6e 203d 207b 6174 7472 203d 2022  sion = {attr = "
 00000350: 7061 7261 6c6c 6178 2e5f 5f76 6572 7369  parallax.__versi
 00000360: 6f6e 5f5f 227d 0d0a 7265 6164 6d65 203d  on__"}..readme =
 00000370: 207b 6669 6c65 203d 2022 5245 4144 4d45   {file = "README
 00000380: 2e6d 6422 7d0d 0a20 0d0a 5b70 726f 6a65  .md"}.. ..[proje
 00000390: 6374 2e6f 7074 696f 6e61 6c2d 6465 7065  ct.optional-depe
-000003a0: 6e64 656e 6369 6573 5d0d 0a6c 696e 7465  ndencies]..linte
-000003b0: 7273 203d 205b 0d0a 2020 2020 2763 6f64  rs = [..    'cod
-000003c0: 6573 7065 6c6c 272c 0d0a 2020 2020 2763  espell',..    'c
-000003d0: 6f76 6572 6167 6527 2c0d 0a20 2020 2027  overage',..    '
-000003e0: 666c 616b 6538 272c 0d0a 2020 2020 2769  flake8',..    'i
-000003f0: 6e74 6572 726f 6761 7465 272c 0d0a 2020  nterrogate',..  
-00000400: 2020 2769 736f 7274 270d 0a5d 0d0a 0d0a    'isort'..]....
-00000410: 646f 6373 203d 205b 0d0a 2020 2020 2753  docs = [..    'S
-00000420: 7068 696e 7827 2c0d 0a20 2020 2027 7370  phinx',..    'sp
-00000430: 6869 6e78 2d6a 696e 6a61 272c 0d0a 2020  hinx-jinja',..  
-00000440: 2020 2766 7572 6f27 0d0a 5d0d 0a0d 0a5b    'furo'..]....[
-00000450: 746f 6f6c 2e69 6e74 6572 726f 6761 7465  tool.interrogate
-00000460: 5d0d 0a66 6169 6c2d 756e 6465 7220 3d20  ]..fail-under = 
-00000470: 3130 300d 0a20 0d0a 5b74 6f6f 6c2e 636f  100.. ..[tool.co
-00000480: 6465 7370 656c 6c5d 0d0a 736b 6970 203d  despell]..skip =
-00000490: 2022 2e67 6974 2c2a 2e6a 736f 6e2c 2a2e   ".git,*.json,*.
-000004a0: 6c6f 6722 0d0a 200d 0a5b 746f 6f6c 5d0d  log".. ..[tool].
-000004b0: 0a68 6f6d 6570 6167 6520 3d20 2268 7474  .homepage = "htt
-000004c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000004d0: 416c 6c65 6e4e 6575 7261 6c44 796e 616d  AllenNeuralDynam
-000004e0: 6963 732f 7061 7261 6c6c 6178 220d 0a72  ics/parallax"..r
-000004f0: 6570 6f73 6974 6f72 7920 3d20 2268 7474  epository = "htt
-00000500: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000510: 416c 6c65 6e4e 6575 7261 6c44 796e 616d  AllenNeuralDynam
-00000520: 6963 732f 7061 7261 6c6c 6178 220d 0a64  ics/parallax"..d
-00000530: 6f63 756d 656e 7461 7469 6f6e 203d 2022  ocumentation = "
-00000540: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000550: 6f6d 2f41 6c6c 656e 4e65 7572 616c 4479  om/AllenNeuralDy
-00000560: 6e61 6d69 6373 2f70 6172 616c 6c61 782f  namics/parallax/
-00000570: 7769 6b69 22                             wiki"
+000003a0: 6e64 656e 6369 6573 5d0d 0a64 6576 203d  ndencies]..dev =
+000003b0: 205b 0d0a 2020 2020 2770 6172 616c 6c61   [..    'paralla
+000003c0: 782d 6170 705b 6c69 6e74 6572 735d 270d  x-app[linters]'.
+000003d0: 0a5d 0d0a 0d0a 6c69 6e74 6572 7320 3d20  .]....linters = 
+000003e0: 5b0d 0a20 2020 2027 636f 6465 7370 656c  [..    'codespel
+000003f0: 6c27 2c0d 0a20 2020 2027 636f 7665 7261  l',..    'covera
+00000400: 6765 272c 0d0a 2020 2020 2766 6c61 6b65  ge',..    'flake
+00000410: 3827 2c0d 0a20 2020 2027 696e 7465 7272  8',..    'interr
+00000420: 6f67 6174 6527 2c0d 0a20 2020 2027 6973  ogate',..    'is
+00000430: 6f72 7427 2c0d 0a20 2020 2027 7079 7465  ort',..    'pyte
+00000440: 7374 2d6d 6f63 6b27 0d0a 5d0d 0a0d 0a64  st-mock'..]....d
+00000450: 6f63 7320 3d20 5b0d 0a20 2020 2027 5370  ocs = [..    'Sp
+00000460: 6869 6e78 272c 0d0a 2020 2020 2773 7068  hinx',..    'sph
+00000470: 696e 782d 6a69 6e6a 6127 2c0d 0a20 2020  inx-jinja',..   
+00000480: 2027 6675 726f 270d 0a5d 0d0a 0d0a 5b74   'furo'..]....[t
+00000490: 6f6f 6c2e 636f 7665 7261 6765 2e72 756e  ool.coverage.run
+000004a0: 5d0d 0a6f 6d69 7420 3d20 5b0d 0a20 2020  ]..omit = [..   
+000004b0: 2022 2a5f 5f69 6e69 745f 5f2a 220d 0a5d   "*__init__*"..]
+000004c0: 0d0a 736f 7572 6365 203d 205b 2270 6172  ..source = ["par
+000004d0: 616c 6c61 7822 2c20 2274 6573 7473 225d  allax", "tests"]
+000004e0: 0d0a 0d0a 5b74 6f6f 6c2e 636f 7665 7261  ....[tool.covera
+000004f0: 6765 2e72 6570 6f72 745d 0d0a 6578 636c  ge.report]..excl
+00000500: 7564 655f 6c69 6e65 7320 3d20 5b22 6966  ude_lines = ["if
+00000510: 205f 5f6e 616d 655f 5f20 3d3d 202e 5f5f   __name__ == .__
+00000520: 6d61 696e 5f5f 2e3a 222c 2022 7072 6167  main__.:", "prag
+00000530: 6d61 3a20 6e6f 2063 6f76 6572 225d 0d0a  ma: no cover"]..
+00000540: 6661 696c 5f75 6e64 6572 203d 2031 3030  fail_under = 100
+00000550: 0d0a 0d0a 5b74 6f6f 6c2e 6973 6f72 745d  ....[tool.isort]
+00000560: 0d0a 6c69 6e65 5f6c 656e 6774 6820 3d20  ..line_length = 
+00000570: 3132 300d 0a70 726f 6669 6c65 203d 2022  120..profile = "
+00000580: 626c 6163 6b22 0d0a 0d0a 5b74 6f6f 6c2e  black"....[tool.
+00000590: 696e 7465 7272 6f67 6174 655d 0d0a 6578  interrogate]..ex
+000005a0: 636c 7564 6520 3d20 5b22 7365 7475 702e  clude = ["setup.
+000005b0: 7079 222c 2022 646f 6373 222c 2022 6275  py", "docs", "bu
+000005c0: 696c 6422 5d0d 0a66 6169 6c2d 756e 6465  ild"]..fail-unde
+000005d0: 7220 3d20 3130 300d 0a20 0d0a 5b74 6f6f  r = 100.. ..[too
+000005e0: 6c2e 636f 6465 7370 656c 6c5d 0d0a 736b  l.codespell]..sk
+000005f0: 6970 203d 2022 2e67 6974 2c2a 2e6a 736f  ip = ".git,*.jso
+00000600: 6e2c 2a2e 6c6f 6722 0d0a 200d 0a5b 746f  n,*.log".. ..[to
+00000610: 6f6c 5d0d 0a68 6f6d 6570 6167 6520 3d20  ol]..homepage = 
+00000620: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000630: 636f 6d2f 416c 6c65 6e4e 6575 7261 6c44  com/AllenNeuralD
+00000640: 796e 616d 6963 732f 7061 7261 6c6c 6178  ynamics/parallax
+00000650: 220d 0a72 6570 6f73 6974 6f72 7920 3d20  "..repository = 
+00000660: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000670: 636f 6d2f 416c 6c65 6e4e 6575 7261 6c44  com/AllenNeuralD
+00000680: 796e 616d 6963 732f 7061 7261 6c6c 6178  ynamics/parallax
+00000690: 220d 0a64 6f63 756d 656e 7461 7469 6f6e  "..documentation
+000006a0: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
+000006b0: 7562 2e63 6f6d 2f41 6c6c 656e 4e65 7572  ub.com/AllenNeur
+000006c0: 616c 4479 6e61 6d69 6373 2f70 6172 616c  alDynamics/paral
+000006d0: 6c61 782f 7769 6b69 22                   lax/wiki"
```

### Comparing `parallax_app-0.37.0/ui/ParallaxReadME.JPG` & `parallax_app-0.37.1/ui/ParallaxReadME.JPG`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/font/FiraCode-VariableFont_wght.ttf` & `parallax_app-0.37.1/ui/font/FiraCode-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/mainWindow.ui` & `parallax_app-0.37.1/ui/mainWindow.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/probe_calib.ui` & `parallax_app-0.37.1/ui/probe_calib.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/arrow-right.png` & `parallax_app-0.37.1/ui/resources/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/check.png` & `parallax_app-0.37.1/ui/resources/check.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/gear.png` & `parallax_app-0.37.1/ui/resources/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/recordingButton.png` & `parallax_app-0.37.1/ui/resources/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/recordingButton_disabled.png` & `parallax_app-0.37.1/ui/resources/recordingButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/sextant.png` & `parallax_app-0.37.1/ui/resources/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/snapshotButton_disabled.png` & `parallax_app-0.37.1/ui/resources/snapshotButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/snapshotButton_green.png` & `parallax_app-0.37.1/ui/resources/snapshotButton_green.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/snapshotButton_white.png` & `parallax_app-0.37.1/ui/resources/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/stop-sign.png` & `parallax_app-0.37.1/ui/resources/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/resources/target.png` & `parallax_app-0.37.1/ui/resources/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/reticle_calib.ui` & `parallax_app-0.37.1/ui/reticle_calib.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/settingPopUpMenu.ui` & `parallax_app-0.37.1/ui/settingPopUpMenu.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.0/ui/stage_info.ui` & `parallax_app-0.37.1/ui/stage_info.ui`

 * *Files identical despite different names*

