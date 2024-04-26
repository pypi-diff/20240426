# Comparing `tmp/autolab-1.1.9.tar.gz` & `tmp/autolab-2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autolab-1.1.9.tar", last modified: Fri Feb 21 14:47:52 2020, max compression
+gzip compressed data, was "autolab-2.0b2.tar", last modified: Fri Apr 26 20:39:48 2024, max compression
```

## Comparing `autolab-1.1.9.tar` & `autolab-2.0b2.tar`

### file list

```diff
@@ -1,218 +1,120 @@
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1270 2020-02-21 14:47:52.000000 autolab-1.1.9/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      563 2020-02-12 16:43:30.000000 autolab-1.1.9/README.md
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/
--rw-r--r--   0 bruno     (1000) bruno     (1000)      740 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/__init__.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/core/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       97 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3178 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/config.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2246 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/devices.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    19040 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/drivers.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    15231 2020-02-12 16:43:34.000000 autolab-1.1.9/autolab/core/elements.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/core/gui/
--rw-r--r--   0 bruno     (1000) bruno     (1000)      893 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/__init__.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/core/gui/controlcenter/
--rw-r--r--   0 bruno     (1000) bruno     (1000)        0 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/controlcenter/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     6042 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/controlcenter/main.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3179 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/controlcenter/thread.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    14206 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/controlcenter/treewidgets.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/core/gui/monitoring/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/monitoring/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1614 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/monitoring/data.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2759 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/monitoring/figure.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     6652 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/monitoring/main.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3679 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/monitoring/monitor.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/core/gui/scanning/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/scanning/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    16890 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/scanning/config.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     8101 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/scanning/data.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    19699 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/scanning/figure.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2372 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/scanning/main.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2665 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/scanning/parameter.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    12945 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/scanning/recipe.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    10723 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/scanning/scan.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     8046 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/gui/scanning/scanrange.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)      586 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/paths.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    10311 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/recorder.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2438 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/stats.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)      983 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/utilities.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)      252 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/core/web.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/__init__.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/agilent_33220A/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_33220A/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2983 2020-02-18 15:04:44.000000 autolab-1.1.9/autolab/drivers/agilent_33220A/agilent_33220A.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1876 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_33220A/agilent_33220A_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/agilent_81150A/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_81150A/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3768 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_81150A/agilent_81150A.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3799 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_81150A/agilent_81150A_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/agilent_DSA91304A/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_DSA91304A/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5573 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_DSA91304A/agilent_DSA91304A.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3398 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_DSA91304A/agilent_DSA91304A_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/agilent_DSO54853A/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_DSO54853A/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5437 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_DSO54853A/agilent_DSO54853A.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3420 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_DSO54853A/agilent_DSO54853A_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/agilent_DSO81204B/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_DSO81204B/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5555 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_DSO81204B/agilent_DSO81204B.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3428 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_DSO81204B/agilent_DSO81204B_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/agilent_E8244A/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_E8244A/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1554 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_E8244A/agilent_E8244A.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1482 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_E8244A/agilent_E8244A_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/agilent_MXAN9020A/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_MXAN9020A/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4348 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_MXAN9020A/agilent_MXAN9020A.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2014 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/agilent_MXAN9020A/agilent_MXAN9020A_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/aimtti_TGA12104/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/aimtti_TGA12104/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3515 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/aimtti_TGA12104/aimtti_TGA12104.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1998 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/aimtti_TGA12104/aimtti_TGA12104_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/aimtti_TGF3162/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/aimtti_TGF3162/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4579 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/aimtti_TGF3162/aimtti_TGF3162.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2481 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/aimtti_TGF3162/aimtti_TGF3162_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/ando_AQ6315A/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/ando_AQ6315A/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     6713 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/ando_AQ6315A/ando_AQ6315A.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1942 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/ando_AQ6315A/ando_AQ6315A_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/anritsu_MS9740A/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/anritsu_MS9740A/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1942 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/anritsu_MS9740A/anritsu_MS9740A.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1864 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/anritsu_MS9740A/anritsu_MS9740A_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/arduino_CUSTOMSHUTTERS/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/arduino_CUSTOMSHUTTERS/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5932 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/arduino_CUSTOMSHUTTERS/arduino_CUSTOMSHUTTERS.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1847 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/arduino_CUSTOMSHUTTERS/arduino_CUSTOMSHUTTERS_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/dummy/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/dummy/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5361 2020-02-12 16:43:34.000000 autolab-1.1.9/autolab/drivers/dummy/dummy.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1852 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/dummy/dummy_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/exfo_IQS605P/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/exfo_IQS605P/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4199 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/exfo_IQS605P/exfo_IQS605P.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2459 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/exfo_IQS605P/exfo_IQS605P_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/exfo_LTB1/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/exfo_LTB1/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4647 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/exfo_LTB1/exfo_LTB1.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2461 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/exfo_LTB1/exfo_LTB1_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/exfo_PM1613/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/exfo_PM1613/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4204 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/exfo_PM1613/exfo_PM1613.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1876 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/exfo_PM1613/exfo_PM1613_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/hp_8656B/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/hp_8656B/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1880 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/hp_8656B/hp_8656B.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1897 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/hp_8656B/hp_8656B_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/ilxlightwave_LDC3724/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/ilxlightwave_LDC3724/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    11291 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/ilxlightwave_LDC3724/ilxlightwave_LDC3724.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1811 2020-02-12 16:43:30.000000 autolab-1.1.9/autolab/drivers/ilxlightwave_LDC3724/ilxlightwave_LDC3724_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/keithley_2200/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:34.000000 autolab-1.1.9/autolab/drivers/keithley_2200/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4018 2020-02-12 16:43:34.000000 autolab-1.1.9/autolab/drivers/keithley_2200/keithley_2200.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1990 2020-02-12 16:43:34.000000 autolab-1.1.9/autolab/drivers/keithley_2200/keithley_2200_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/keithley_K2600B/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/keithley_K2600B/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     8020 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/keithley_K2600B/keithley_K2600B.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1762 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/keithley_K2600B/keithley_K2600B_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/keopsys_CEFA_C_PB_HP/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/keopsys_CEFA_C_PB_HP/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1701 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/keopsys_CEFA_C_PB_HP/keopsys_CEFA_C_PB_HP.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1327 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/keopsys_CEFA_C_PB_HP/keopsys_CEFA_C_PB_HP_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/lecroy_WAVEMASTER/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/lecroy_WAVEMASTER/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    11939 2020-02-12 16:43:34.000000 autolab-1.1.9/autolab/drivers/lecroy_WAVEMASTER/lecroy_WAVEMASTER.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4416 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/lecroy_WAVEMASTER/lecroy_WAVEMASTER_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/newport_1918C/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_1918C/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     7072 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_1918C/newport_1918C.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2021 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_1918C/newport_1918C_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/newport_CONEXPP/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_CONEXPP/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    13696 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_CONEXPP/newport_CONEXPP.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2467 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_CONEXPP/newport_CONEXPP_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/newport_SMC100/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_SMC100/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4344 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_SMC100/newport_SMC100.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2485 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_SMC100/newport_SMC100_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/newport_TLB6700/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_TLB6700/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5173 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_TLB6700/newport_TLB6700.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3278 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_TLB6700/newport_TLB6700_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/newport_XPS/
--rw-r--r--   0 bruno     (1000) bruno     (1000)    98150 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_XPS/XPS.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_XPS/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    14903 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_XPS/newport_XPS.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2480 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/newport_XPS/newport_XPS_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/princeton_SPECTRO32/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/princeton_SPECTRO32/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4870 2020-02-12 16:43:34.000000 autolab-1.1.9/autolab/drivers/princeton_SPECTRO32/princeton_SPECTRO32.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2803 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/princeton_SPECTRO32/princeton_SPECTRO32_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/princeton_WINSPEC/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/princeton_WINSPEC/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     9378 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/princeton_WINSPEC/princeton_WINSPEC.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2515 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/princeton_WINSPEC/princeton_WINSPEC_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/sacher_PC500/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-21 14:43:30.000000 autolab-1.1.9/autolab/drivers/sacher_PC500/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2631 2020-02-21 11:05:17.000000 autolab-1.1.9/autolab/drivers/sacher_PC500/sacher_PC500.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1211 2020-02-20 16:08:54.000000 autolab-1.1.9/autolab/drivers/sacher_PC500/sacher_PC500_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/signalrecovery_7XXX/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/signalrecovery_7XXX/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3650 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/signalrecovery_7XXX/signalrecovery_7XXX.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1891 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/signalrecovery_7XXX/signalrecovery_7XXX_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/srs_DG645/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/srs_DG645/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4017 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/srs_DG645/srs_DG645.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3453 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/srs_DG645/srs_DG645_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/srs_DS345/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/srs_DS345/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2553 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/srs_DS345/srs_DS345.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2104 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/srs_DS345/srs_DS345_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/srs_SIM900/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/srs_SIM900/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5507 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/srs_SIM900/srs_SIM900.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3697 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/srs_SIM900/srs_SIM900_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/system/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/system/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1716 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/system/system.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/tektronix_DPO4104/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/tektronix_DPO4104/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4950 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/tektronix_DPO4104/tektronix_DPO4104.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1886 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/tektronix_DPO4104/tektronix_DPO4104_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/tektronix_TDS5104B/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/tektronix_TDS5104B/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5179 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/tektronix_TDS5104B/tektronix_TDS5104B.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2403 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/tektronix_TDS5104B/tektronix_TDS5104B_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/thorlabs_ITC4001/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/thorlabs_ITC4001/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1307 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/thorlabs_ITC4001/thorlabs_ITC4001.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1261 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/thorlabs_ITC4001/thorlabs_ITC4001_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/yenista_OSICS/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/yenista_OSICS/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    11204 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/yenista_OSICS/yenista_OSICS.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2384 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/yenista_OSICS/yenista_OSICS_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/yenista_TUNICS/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/yenista_TUNICS/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4731 2020-02-12 16:43:34.000000 autolab-1.1.9/autolab/drivers/yenista_TUNICS/yenista_TUNICS.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2245 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/yenista_TUNICS/yenista_TUNICS_utilities.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab/drivers/yokogawa_AQ6370/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/yokogawa_AQ6370/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4593 2020-02-20 17:44:18.000000 autolab-1.1.9/autolab/drivers/yokogawa_AQ6370/yokogawa_AQ6370.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2054 2020-02-12 16:43:31.000000 autolab-1.1.9/autolab/drivers/yokogawa_AQ6370/yokogawa_AQ6370_utilities.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    15120 2020-02-12 16:43:34.000000 autolab-1.1.9/autolab/scan.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab.egg-info/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1270 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab.egg-info/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)     7471 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab.egg-info/SOURCES.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab.egg-info/dependency_links.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       50 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab.egg-info/entry_points.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       70 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab.egg-info/requires.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       16 2020-02-21 14:47:52.000000 autolab-1.1.9/autolab.egg-info/top_level.txt
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-02-21 14:47:52.000000 autolab-1.1.9/scripts/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       98 2020-02-12 16:43:31.000000 autolab-1.1.9/scripts/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    14058 2020-02-12 16:43:34.000000 autolab-1.1.9/scripts/autolab.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2020-02-21 14:47:52.000000 autolab-1.1.9/setup.cfg
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1463 2020-02-12 16:43:31.000000 autolab-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.455566 autolab-2.0b2/
+-rw-rw-rw-   0        0        0    35823 2024-02-14 08:41:38.000000 autolab-2.0b2/LICENSE
+-rw-rw-rw-   0        0        0       73 2024-02-14 08:41:38.000000 autolab-2.0b2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2610 2024-04-26 20:39:48.447505 autolab-2.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0      999 2024-02-14 08:41:38.000000 autolab-2.0b2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.295273 autolab-2.0b2/autolab/
+-rw-rw-rw-   0        0        0     2598 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/__init__.py
+-rw-rw-rw-   0        0        0    13667 2024-04-17 07:54:24.000000 autolab-2.0b2/autolab/_entry_script.py
+-rw-rw-rw-   0        0        0   831700 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/autolab.pdf
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.335482 autolab-2.0b2/autolab/core/
+-rw-rw-rw-   0        0        0      103 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/__init__.py
+-rw-rw-rw-   0        0        0     1985 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/_create_shortcut.py
+-rw-rw-rw-   0        0        0    12697 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/config.py
+-rw-rw-rw-   0        0        0     1287 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/default_driver_utilities.py
+-rw-rw-rw-   0        0        0     5409 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/devices.py
+-rw-rw-rw-   0        0        0     9968 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/drivers.py
+-rw-rw-rw-   0        0        0    17730 2024-04-18 12:02:50.000000 autolab-2.0b2/autolab/core/elements.py
+-rw-rw-rw-   0        0        0    10158 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gitdir.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.335482 autolab-2.0b2/autolab/core/gui/
+-rw-rw-rw-   0        0        0      993 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/GUI_utilities.py
+-rw-rw-rw-   0        0        0     2082 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.347950 autolab-2.0b2/autolab/core/gui/controlcenter/
+-rw-rw-rw-   0        0        0      141 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/controlcenter/__init__.py
+-rw-rw-rw-   0        0        0    21155 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/controlcenter/main.py
+-rw-rw-rw-   0        0        0    10643 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/controlcenter/slider.py
+-rw-rw-rw-   0        0        0     6589 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/controlcenter/thread.py
+-rw-rw-rw-   0        0        0    26842 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/controlcenter/treewidgets.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.406485 autolab-2.0b2/autolab/core/gui/icons/
+-rw-rw-rw-   0        0        0     4441 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.416696 autolab-2.0b2/autolab/core/gui/icons/__pycache__/
+-rw-rw-rw-   0        0        0     7151 2024-03-16 11:24:49.000000 autolab-2.0b2/autolab/core/gui/icons/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6746 2024-03-16 10:56:12.000000 autolab-2.0b2/autolab/core/gui/icons/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2881 2024-03-16 10:59:07.000000 autolab-2.0b2/autolab/core/gui/icons/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0     2885 2024-02-16 15:34:56.000000 autolab-2.0b2/autolab/core/gui/icons/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2893 2024-02-14 15:51:33.000000 autolab-2.0b2/autolab/core/gui/icons/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1550 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/action-icon.svg
+-rw-rw-rw-   0        0        0     1647 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/add-icon.svg
+-rw-rw-rw-   0        0        0    93062 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/icons/autolab-icon.ico
+-rw-rw-rw-   0        0        0     9874 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/icons/autolab-icon.png
+-rw-rw-rw-   0        0        0     4715 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/icons/autolab-icon.svg
+-rw-rw-rw-   0        0        0     1877 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/bool-icon.svg
+-rw-rw-rw-   0        0        0     1877 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/bytes-icon.svg
+-rw-rw-rw-   0        0        0     4515 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/config-icon.svg
+-rw-rw-rw-   0        0        0     3250 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/dataframe-icon.svg
+-rw-rw-rw-   0        0        0     2862 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/disconnect-icon.svg
+-rw-rw-rw-   0        0        0     1484 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/down-icon.svg
+-rw-rw-rw-   0        0        0     1682 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/export-icon.svg
+-rw-rw-rw-   0        0        0     1787 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/float-icon.svg
+-rw-rw-rw-   0        0        0      963 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/github-icon.svg
+-rw-rw-rw-   0        0        0     1836 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/import-icon.svg
+-rw-rw-rw-   0        0        0     1875 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/int-icon.svg
+-rw-rw-rw-   0        0        0     1779 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/is-disable-icon.svg
+-rw-rw-rw-   0        0        0     1713 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/is-enable-icon.svg
+-rw-rw-rw-   0        0        0     2481 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/measure-icon.svg
+-rw-rw-rw-   0        0        0     3536 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/monitor-icon.svg
+-rw-rw-rw-   0        0        0     3136 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/ndarray-icon.svg
+-rw-rw-rw-   0        0        0     4063 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/parameter-icon.svg
+-rw-rw-rw-   0        0        0     8465 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/pdf-icon.svg
+-rw-rw-rw-   0        0        0     2472 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/plotter-icon.svg
+-rw-rw-rw-   0        0        0     1711 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/read-save-icon.svg
+-rw-rw-rw-   0        0        0     2601 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/readthedocs-icon.svg
+-rw-rw-rw-   0        0        0     3533 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/recipe-icon.svg
+-rw-rw-rw-   0        0        0     1897 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/redo-icon.svg
+-rw-rw-rw-   0        0        0     3468 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/remove-icon.svg
+-rw-rw-rw-   0        0        0     2689 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/rename-icon.svg
+-rw-rw-rw-   0        0        0     3693 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/scanner-icon.svg
+-rw-rw-rw-   0        0        0     2070 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/slider-icon.svg
+-rw-rw-rw-   0        0        0     1875 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/str-icon.svg
+-rw-rw-rw-   0        0        0     1777 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/tuple-icon.svg
+-rw-rw-rw-   0        0        0     1903 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/undo-icon.svg
+-rw-rw-rw-   0        0        0     1485 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/up-icon.svg
+-rw-rw-rw-   0        0        0     2118 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/icons/write-icon.svg
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.425212 autolab-2.0b2/autolab/core/gui/monitoring/
+-rw-rw-rw-   0        0        0      105 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/monitoring/__init__.py
+-rw-rw-rw-   0        0        0     3378 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/monitoring/data.py
+-rw-rw-rw-   0        0        0     4594 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/monitoring/figure.py
+-rw-rw-rw-   0        0        0     7523 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/monitoring/interface.ui
+-rw-rw-rw-   0        0        0     8984 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/monitoring/main.py
+-rw-rw-rw-   0        0        0     3692 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/monitoring/monitor.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.435352 autolab-2.0b2/autolab/core/gui/plotting/
+-rw-rw-rw-   0        0        0       90 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/plotting/__init__.py
+-rw-rw-rw-   0        0        0    16060 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/plotting/data.py
+-rw-rw-rw-   0        0        0     7069 2024-03-16 10:55:44.000000 autolab-2.0b2/autolab/core/gui/plotting/figure.py
+-rw-rw-rw-   0        0        0    16966 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/plotting/interface.ui
+-rw-rw-rw-   0        0        0    20037 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/plotting/main.py
+-rw-rw-rw-   0        0        0     5533 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/plotting/thread.py
+-rw-rw-rw-   0        0        0    15909 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/plotting/treewidgets.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.447505 autolab-2.0b2/autolab/core/gui/scanning/
+-rw-rw-rw-   0        0        0      105 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/gui/scanning/__init__.py
+-rw-rw-rw-   0        0        0    48998 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/scanning/config.py
+-rw-rw-rw-   0        0        0    16017 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/scanning/customWidgets.py
+-rw-rw-rw-   0        0        0    18452 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/scanning/data.py
+-rw-rw-rw-   0        0        0     3082 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/scanning/display.py
+-rw-rw-rw-   0        0        0    16595 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/scanning/figure.py
+-rw-rw-rw-   0        0        0    20181 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/scanning/interface.ui
+-rw-rw-rw-   0        0        0    19158 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/scanning/main.py
+-rw-rw-rw-   0        0        0    29256 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/scanning/parameter.py
+-rw-rw-rw-   0        0        0    20777 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/scanning/recipe.py
+-rw-rw-rw-   0        0        0    15043 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/scanning/scan.py
+-rw-rw-rw-   0        0        0    22128 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/gui/variables.py
+-rw-rw-rw-   0        0        0     6650 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/infos.py
+-rw-rw-rw-   0        0        0     1247 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/paths.py
+-rw-rw-rw-   0        0        0     9875 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/recorder.py
+-rw-rw-rw-   0        0        0    14522 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/repository.py
+-rw-rw-rw-   0        0        0    10997 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/server.py
+-rw-rw-rw-   0        0        0    12360 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/core/utilities.py
+-rw-rw-rw-   0        0        0     1865 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/version_adapter.py
+-rw-rw-rw-   0        0        0     1801 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/core/web.py
+-rw-rw-rw-   0        0        0    15637 2024-02-14 08:41:38.000000 autolab-2.0b2/autolab/scan.py
+-rw-rw-rw-   0        0        0        5 2024-04-26 20:32:01.000000 autolab-2.0b2/autolab/version.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 20:39:48.305388 autolab-2.0b2/autolab.egg-info/
+-rw-rw-rw-   0        0        0     2610 2024-04-26 20:39:48.000000 autolab-2.0b2/autolab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3734 2024-04-26 20:39:48.000000 autolab-2.0b2/autolab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 20:39:48.000000 autolab-2.0b2/autolab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 20:39:48.000000 autolab-2.0b2/autolab.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2024-04-26 20:39:48.000000 autolab-2.0b2/autolab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 20:39:48.000000 autolab-2.0b2/autolab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1543 2024-04-26 20:32:01.000000 autolab-2.0b2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 20:39:48.455566 autolab-2.0b2/setup.cfg
+-rw-rw-rw-   0        0        0     2077 2024-04-26 20:32:01.000000 autolab-2.0b2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `autolab-1.1.9/README.md` & `autolab-2.0b2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,23 @@
-# Autolab
-__Python package for scientific experiments automation__
-
-The purpose of this package it to provide easy and efficient tools to deal with your scientific instruments, and to run automated experiments with them, by command line instructions or through a graphical user interface (GUI). 
-
-Created by Quentin Chateiller, Python drivers from Quentin Chateiller and Bruno Garbin, for the C2N-CNRS (Center for Nanosciences and Nanotechnologies, Palaiseau, France) ToniQ team.
-
-Visit https://autolab.readthedocs.io/ for the full documentation of this package.
+# Autolab
+__Python package for scientific experiments automation__
+
+The purpose of this package it to provide easy and efficient tools to deal with your scientific instruments, and to run automated experiments with them, by command line instructions or through a graphical user interface (GUI).
+
+Created by Quentin Chateiller, Python drivers originally from Quentin Chateiller and Bruno Garbin, for the C2N-CNRS (Center for Nanosciences and Nanotechnologies, Palaiseau, France) ToniQ team.
+Project continued by Jonathan Peltier, for the C2N-CNRS, Minaphot team.
+
+Project hosted at https://github.com/autolab-project/autolab
+
+Drivers made for this package can be found at https://github.com/autolab-project/autolab-drivers
+
+Visit https://autolab.readthedocs.io/ for the full documentation of this package.
+
+## Overview
+
+![Autolab scheme](docs/scheme.png)
+
+## GUI example
+
+![Autolab Scanning GUI](docs/gui/scanning.png)
+
+![Autolab Control Panel GUI](docs/gui/control_panel.png)
```

### Comparing `autolab-1.1.9/autolab/core/paths.py` & `autolab-2.0b2/autolab/core/paths.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,33 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Sep 20 17:11:57 2019
-
-@author: qchat
-"""
-
-import os 
-
-USER_FOLDER = os.path.join(os.path.expanduser('~'),'autolab')
-USER_LAST_CUSTOM_FOLDER = os.path.expanduser('~')
-LOCAL_CONFIG = os.path.join(USER_FOLDER,'local_config.ini')
-AUTOLAB_CONFIG = os.path.join(USER_FOLDER,'autolab_config.ini')
-LOCAL_CONFIG_TEMPLATE = os.path.join(os.path.dirname(__file__),'local_config.ini')
-        
-DRIVER_SOURCES = {'main':os.path.join(os.path.dirname(os.path.dirname(__file__)),'drivers'),
-                  'local':os.path.join(USER_FOLDER,'local_drivers')}
+# -*- coding: utf-8 -*-
+"""
+Created on Fri Sep 20 17:11:57 2019
+
+@author: qchat
+"""
+
+import os
+
+
+AUTOLAB_FOLDER = os.path.dirname(os.path.dirname(__file__))
+
+VERSION = os.path.join(AUTOLAB_FOLDER, 'version.txt')
+
+USER_FOLDER = os.path.join(os.path.expanduser('~'), 'autolab')
+USER_LAST_CUSTOM_FOLDER = os.path.expanduser('~')
+DEVICES_CONFIG = os.path.join(USER_FOLDER, 'devices_config.ini')
+AUTOLAB_CONFIG = os.path.join(USER_FOLDER, 'autolab_config.ini')
+PLOTTER_CONFIG = os.path.join(USER_FOLDER, 'plotter_config.ini')
+HISTORY_CONFIG = os.path.join(USER_FOLDER, '.history_config.txt')
+
+# Drivers locations
+DRIVERS = os.path.join(USER_FOLDER,'drivers')
+DRIVER_LEGACY = {'official': os.path.join(AUTOLAB_FOLDER, 'drivers'),
+                  'local': os.path.join(USER_FOLDER, 'local_drivers')}
+# can add paths in autolab_config.ini [extra_driver_path]
+DRIVER_SOURCES = {'official': os.path.join(DRIVERS, 'official'),
+                  'local': os.path.join(DRIVERS, 'local')}
+
+# Driver repository
+# can add paths in autolab_config.ini [extra_driver_url_repo]
+# format is {'path to install': 'url to download'}
+DRIVER_REPOSITORY = {DRIVER_SOURCES['official']: 'https://github.com/autolab-project/autolab-drivers'}
```

### Comparing `autolab-1.1.9/autolab/core/recorder.py` & `autolab-2.0b2/autolab/core/recorder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,325 +1,322 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Sun Jul 21 22:13:21 2019
-
-@author: qchat
-"""
-
-
-import os
-import shutil
-
-
-
-
-
-
-def checkForbiddenCharacters(value):
-    try : 
-        assert '/' not in value
-        assert '<' not in value
-        assert '>' not in value
-        assert ':' not in value
-        assert '?' not in value
-        assert '!' not in value
-        assert '\\' not in value
-        assert '*' not in value
-        assert '|' not in value
-        return True
-    except :
-        return False  
-    
-    
-    
-    
-class Recorder :
-    
-    def __init__(self,name,customPath=None,verbose=True):
-        
-        if isinstance(name,str) is False or checkForbiddenCharacters(name) is False:
-            raise ValueError(f'The name "{name}" is not valid')           
-            		
-        print(f'Starting Recorder with name "{name}"')
-                
-        self.verbose = verbose 
-        
-        self.name = name
-        self.path = None
-        
-        self.var = {}
-        self.varList= []
-        self.started = False
-        self.count = 0
-        self.mainFile = None
-        
-        
-        if customPath is None :
-            self.setPath(os.getcwd())
-        else :
-            self.createFolder(customPath)
-            self.setPath(customPath)
-        
-    #--------------------------------------------------------------------------
-    # Path
-    #--------------------------------------------------------------------------
-        
-    def createFolder(self,path):
-        if os.path.exists(path) is False :
-            parentFolder = os.path.realpath(os.path.dirname(path))
-            if os.path.exists(parentFolder) is False :
-                self.createFolder(parentFolder)
-            os.mkdir(path)
-                
-    
-    def getPath(self):
-        return self.path
-    
-    def setPath(self,folderPath):
-        if self.started is False :
-            
-            if os.path.exists(folderPath) is False :
-                raise ValueError(f'The path "{os.path.dirname(folderPath)}" does not exists')
-    
-            path = os.path.join(folderPath,self.name)
-            compt = 0
-            while True :
-                if os.path.exists(path):
-                    compt += 1
-                    path = os.path.join(folderPath,self.name+'_'+str(compt))
-                else :
-                    break
-            self.path = path
-            print(f'Recorder "{self.name}" will save its data at "{self.path}"')
-            
-        else : 
-            raise ValueError('You cannot change the path after having started to save your data')
-        
-        
-        
-    #--------------------------------------------------------------------------
-    # Variables
-    #--------------------------------------------------------------------------    
-    
-    def setValue(self,varName,value):
-        if isinstance(varName,str) is False :
-            raise ValueError(f'"{varName}" is not a valid name for a variable')
-        if self.started and varName not in self.getVariableList() :
-            raise ValueError('You cannot add a new variable after having started to save your data')
-        if varName not in self.getVariableList():
-            self.varList.append(varName)
-        self.var[varName] = value
-        
-        
-    def getValue(self,varName):
-        if varName not in self.getVariableList():
-            raise ValueError(f'Variable unknown "{varName}"')
-        return self.var[varName]
-        
-        
-    def getVariableList(self):
-        return tuple(self.varList)
-
-    
-    def getValueType(self,varName):
-        if varName not in self.getVariableList():
-            raise ValueError(f'Variable unknown "{varName}"')
-        return type(self.var[varName])
-        
-    
-    #--------------------------------------------------------------------------
-    # Data file
-    #--------------------------------------------------------------------------     
-
-    def initialize(self):
-        
-        import pandas as pd
-        self.started = True
-        
-        os.mkdir(self.path)
-        
-        # Sauvegarde script
-        try :
-            scriptPath = os.path.realpath(__file__)
-            shutil.copyfile(scriptPath,os.path.join(self.path,'script_backup.py'))
-        except :
-            pass
-        
-        # Création datafile        
-        headerLine = '# MeasID - Variable'
-        for varName in self.getVariableList() :
-            if self.getValueType(varName) != pd.DataFrame :
-                headerLine += f',{varName}'
-            else :
-                os.mkdir(os.path.join(self.path,varName.replace(' ','_')))
-                        
-        self.mainFile = open(os.path.join(self.path,'data.txt'), 'w')
-        self.mainFile.write(headerLine+'\n')
-        
-        
-    def save(self):
-        
-        import pandas as pd
-        
-        if self.started is False :
-            self.initialize()
-            
-        self.count += 1
-        
-        valueLine = f'{self.count}'
-
-        for varName in self.getVariableList() :
-            if self.getValueType(varName) != pd.DataFrame :
-                valueLine += f',{self.getValue(varName)}'
-            else :
-                varValue = self.getValue(varName)
-                varValue.to_csv(os.path.join(self.path,varName.replace(' ','_'),f'{self.count}.txt'),index=False)
-
-                        
-        self.mainFile.write(valueLine+'\n')
-        
-        if self.verbose is True :
-            print()
-            print(f'Recorder "{self.name}" saving data point #{self.count} :')
-            for varName in self.getVariableList() :
-                print(f' - {varName} = {self.getValue(varName)}')
-            print()
-        
-
-    def close(self):
-        if self.started is True :
-            self.mainFile.close()
-        print(f'Recorder "{self.name}" closed')
-    
-            
-            
-            
-class Recorder_V2 :
-    
-    def __init__(self,name,customPath=None,verbose=True):
-        
-        import pandas as pd
-        
-        if isinstance(name,str) is False or checkForbiddenCharacters(name) is False:
-            raise ValueError(f'The name "{name}" is not valid')           
-            
-        print(f'Starting Recorder with name "{name}"')
-            		
-        self.verbose = verbose 
-        
-        self.name = name
-        self.path = None
-        
-        self.var = {}
-        self.varNameHistory = []
-        self.dataframe = pd.DataFrame()
-        self.started = False
-        self.count = 0
-        
-        
-        if customPath is None :
-            self.setPath(os.getcwd())
-        else :
-            self.createFolder(customPath)
-            self.setPath(customPath)
-        
-    #--------------------------------------------------------------------------
-    # Path
-    #--------------------------------------------------------------------------
-        
-    def createFolder(self,path):
-        if os.path.exists(path) is False :
-            parentFolder = os.path.realpath(os.path.dirname(path))
-            if os.path.exists(parentFolder) is False :
-                self.createFolder(parentFolder)
-            os.mkdir(path)
-                
-    
-    def getPath(self):
-        return self.path
-    
-    def setPath(self,folderPath):
-        if self.started is False :
-            
-            if os.path.exists(folderPath) is False :
-                raise ValueError(f'The path "{os.path.dirname(folderPath)}" does not exists')
-    
-            path = os.path.join(folderPath,self.name)
-            compt = 0
-            while True :
-                if os.path.exists(path):
-                    compt += 1
-                    path = os.path.join(folderPath,self.name+'_'+str(compt))
-                else :
-                    break
-            self.path = path
-            print(f'Recorder "{self.name}" will save its data at "{self.path}"')
-            
-        else : 
-            raise ValueError('You cannot change the path after having started to save your data')
-        
-        
-        
-    #--------------------------------------------------------------------------
-    # Variables
-    #--------------------------------------------------------------------------    
-    
-    def getVariableList(self):
-        return tuple(self.var.keys())
-    
-    def setValue(self,varName,value):
-        if isinstance(varName,str) is False :
-            raise ValueError(f'"{varName}" is not a valid name for a variable')
-        if self.started and varName not in self.getVariableList() :
-            raise ValueError('You cannot add a new variable after having started to save your data')
-        assert type(value) in [str, int, float, bool]
-        if varName not in self.getVariableList() :
-            self.varNameHistory.append(varName)
-        self.var[varName] = value
-        
-    def getValue(self,varName):
-        if varName not in self.getVariableList():
-            raise ValueError(f'Variable unknown "{varName}"')
-        return self.var[varName]
-        
-
-    def getValueType(self,varName):
-        if varName not in self.getVariableList():
-            raise ValueError(f'Variable unknown "{varName}"')
-        return type(self.var[varName])
-        
-    
-    #--------------------------------------------------------------------------
-    # Data file
-    #--------------------------------------------------------------------------     
-
-    def initialize(self):
-        self.started = True
-        
-        os.mkdir(self.path)        
-
-        
-        
-    def save(self):
-        
-        if self.started is False :
-            self.initialize()
-        
-        # Ajout du set de variable à la fin du dataframe
-        self.dataframe = self.dataframe.append(self.var, ignore_index=True)
-
-        # Copie de la dernière ligne dans le fichier
-        filePath = os.path.join(self.getPath(),'data.csv')
-        if len(self.dataframe) == 1 :
-            self.dataframe=self.dataframe[self.varNameHistory]
-            self.dataframe.iloc[[-1]].to_csv(filePath,sep=';')
-        else :
-            self.dataframe.iloc[[-1]].to_csv(filePath,sep=';', mode='a', header=False)
-            
-        # Log
-        if self.verbose is True :
-            print()
-            print(f'Recorder "{self.name}" saving data point #{self.count} :')
-            print(self.dataframe.iloc[-1])
-        
-
-    
+# -*- coding: utf-8 -*-
+"""
+Created on Sun Jul 21 22:13:21 2019
+
+@author: qchat
+"""
+
+
+import os
+import shutil
+
+
+
+
+
+
+def checkForbiddenCharacters(value):
+    try :
+        assert '/' not in value
+        assert '<' not in value
+        assert '>' not in value
+        assert ':' not in value
+        assert '?' not in value
+        assert '!' not in value
+        assert '\\' not in value
+        assert '*' not in value
+        assert '|' not in value
+        return True
+    except :
+        return False
+
+
+
+
+class Recorder :
+
+    def __init__(self,name,customPath=None,verbose=True):
+
+        if isinstance(name,str) is False or checkForbiddenCharacters(name) is False:
+            raise ValueError(f'The name "{name}" is not valid')
+
+        print(f'Starting Recorder with name "{name}"')
+
+        self.verbose = verbose
+
+        self.name = name
+        self.path = None
+
+        self.var = {}
+        self.varList= []
+        self.started = False
+        self.count = 0
+        self.mainFile = None
+
+
+        if customPath is None :
+            self.setPath(os.getcwd())
+        else :
+            self.createFolder(customPath)
+            self.setPath(customPath)
+
+    #--------------------------------------------------------------------------
+    # Path
+    #--------------------------------------------------------------------------
+
+    def createFolder(self,path):
+        if os.path.exists(path) is False :
+            parentFolder = os.path.realpath(os.path.dirname(path))
+            if os.path.exists(parentFolder) is False :
+                self.createFolder(parentFolder)
+            os.mkdir(path)
+
+
+    def getPath(self):
+        return self.path
+
+    def setPath(self,folderPath):
+        if self.started is False :
+
+            if os.path.exists(folderPath) is False :
+                raise ValueError(f'The path "{os.path.dirname(folderPath)}" does not exists')
+
+            path = os.path.join(folderPath,self.name)
+            compt = 0
+            while True :
+                if os.path.exists(path):
+                    compt += 1
+                    path = os.path.join(folderPath,self.name+'_'+str(compt))
+                else :
+                    break
+            self.path = path
+            print(f'Recorder "{self.name}" will save its data at "{self.path}"')
+
+        else :
+            raise ValueError('You cannot change the path after having started to save your data')
+
+
+
+    #--------------------------------------------------------------------------
+    # Variables
+    #--------------------------------------------------------------------------
+
+    def setValue(self,varName,value):
+        if isinstance(varName,str) is False :
+            raise ValueError(f'"{varName}" is not a valid name for a variable')
+        if self.started and varName not in self.getVariableList() :
+            raise ValueError('You cannot add a new variable after having started to save your data')
+        if varName not in self.getVariableList():
+            self.varList.append(varName)
+        self.var[varName] = value
+
+
+    def getValue(self,varName):
+        if varName not in self.getVariableList():
+            raise ValueError(f'Variable unknown "{varName}"')
+        return self.var[varName]
+
+
+    def getVariableList(self):
+        return tuple(self.varList)
+
+
+    def getValueType(self,varName):
+        if varName not in self.getVariableList():
+            raise ValueError(f'Variable unknown "{varName}"')
+        return type(self.var[varName])
+
+
+    #--------------------------------------------------------------------------
+    # Data file
+    #--------------------------------------------------------------------------
+
+    def initialize(self):
+
+        import pandas as pd
+        self.started = True
+
+        os.mkdir(self.path)
+
+        # Sauvegarde script
+        try :
+            scriptPath = os.path.realpath(__file__)
+            shutil.copyfile(scriptPath,os.path.join(self.path,'script_backup.py'))
+        except :
+            pass
+
+        # Création datafile
+        headerLine = '# MeasID - Variable'
+        for varName in self.getVariableList() :
+            if self.getValueType(varName) != pd.DataFrame :
+                headerLine += f',{varName}'
+            else :
+                os.mkdir(os.path.join(self.path,varName.replace(' ','_')))
+
+        self.mainFile = open(os.path.join(self.path,'data.txt'), 'w')
+        self.mainFile.write(headerLine+'\n')
+
+
+    def save(self):
+
+        import pandas as pd
+
+        if self.started is False :
+            self.initialize()
+
+        self.count += 1
+
+        valueLine = f'{self.count}'
+
+        for varName in self.getVariableList() :
+            if self.getValueType(varName) != pd.DataFrame :
+                valueLine += f',{self.getValue(varName)}'
+            else :
+                varValue = self.getValue(varName)
+                varValue.to_csv(os.path.join(self.path,varName.replace(' ','_'),f'{self.count}.txt'),index=False)
+
+
+        self.mainFile.write(valueLine+'\n')
+
+        if self.verbose is True :
+            print()
+            print(f'Recorder "{self.name}" saving data point #{self.count} :')
+            for varName in self.getVariableList() :
+                print(f' - {varName} = {self.getValue(varName)}')
+            print()
+
+
+    def close(self):
+        if self.started is True :
+            self.mainFile.close()
+        print(f'Recorder "{self.name}" closed')
+
+
+
+
+class Recorder_V2 :
+
+    def __init__(self,name,customPath=None,verbose=True):
+
+        import pandas as pd
+
+        if isinstance(name,str) is False or checkForbiddenCharacters(name) is False:
+            raise ValueError(f'The name "{name}" is not valid')
+
+        print(f'Starting Recorder with name "{name}"')
+
+        self.verbose = verbose
+
+        self.name = name
+        self.path = None
+
+        self.var = {}
+        self.varNameHistory = []
+        self.dataframe = pd.DataFrame()
+        self.started = False
+        self.count = 0
+
+
+        if customPath is None :
+            self.setPath(os.getcwd())
+        else :
+            self.createFolder(customPath)
+            self.setPath(customPath)
+
+    #--------------------------------------------------------------------------
+    # Path
+    #--------------------------------------------------------------------------
+
+    def createFolder(self,path):
+        if os.path.exists(path) is False :
+            parentFolder = os.path.realpath(os.path.dirname(path))
+            if os.path.exists(parentFolder) is False :
+                self.createFolder(parentFolder)
+            os.mkdir(path)
+
+
+    def getPath(self):
+        return self.path
+
+    def setPath(self,folderPath):
+        if self.started is False :
+
+            if os.path.exists(folderPath) is False :
+                raise ValueError(f'The path "{os.path.dirname(folderPath)}" does not exists')
+
+            path = os.path.join(folderPath,self.name)
+            compt = 0
+            while True :
+                if os.path.exists(path):
+                    compt += 1
+                    path = os.path.join(folderPath,self.name+'_'+str(compt))
+                else :
+                    break
+            self.path = path
+            print(f'Recorder "{self.name}" will save its data at "{self.path}"')
+
+        else :
+            raise ValueError('You cannot change the path after having started to save your data')
+
+
+
+    #--------------------------------------------------------------------------
+    # Variables
+    #--------------------------------------------------------------------------
+
+    def getVariableList(self):
+        return tuple(self.var.keys())
+
+    def setValue(self,varName,value):
+        if isinstance(varName,str) is False :
+            raise ValueError(f'"{varName}" is not a valid name for a variable')
+        if self.started and varName not in self.getVariableList() :
+            raise ValueError('You cannot add a new variable after having started to save your data')
+        assert type(value) in [str, int, float, bool]
+        if varName not in self.getVariableList() :
+            self.varNameHistory.append(varName)
+        self.var[varName] = value
+
+    def getValue(self,varName):
+        if varName not in self.getVariableList():
+            raise ValueError(f'Variable unknown "{varName}"')
+        return self.var[varName]
+
+
+    def getValueType(self,varName):
+        if varName not in self.getVariableList():
+            raise ValueError(f'Variable unknown "{varName}"')
+        return type(self.var[varName])
+
+
+    #--------------------------------------------------------------------------
+    # Data file
+    #--------------------------------------------------------------------------
+
+    def initialize(self):
+        self.started = True
+
+        os.mkdir(self.path)
+
+
+
+    def save(self):
+
+        if self.started is False :
+            self.initialize()
+
+        # Ajout du set de variable à la fin du dataframe
+        self.dataframe = self.dataframe.append(self.var, ignore_index=True)
+
+        # Copie de la dernière ligne dans le fichier
+        filePath = os.path.join(self.getPath(),'data.csv')
+        if len(self.dataframe) == 1 :
+            self.dataframe=self.dataframe[self.varNameHistory]
+            self.dataframe.iloc[[-1]].to_csv(filePath,sep=';')
+        else :
+            self.dataframe.iloc[[-1]].to_csv(filePath,sep=';', mode='a', header=False)
+
+        # Log
+        if self.verbose is True :
+            print()
+            print(f'Recorder "{self.name}" saving data point #{self.count} :')
+            print(self.dataframe.iloc[-1])
```

### Comparing `autolab-1.1.9/autolab/drivers/sacher_PC500/sacher_PC500_utilities.py` & `autolab-2.0b2/autolab/core/default_driver_utilities.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-category = 'Optical source'
-
-class Driver_parser():
-    def __init__(self, Instance, name, **kwargs):
-        self.name     = name
-        self.Instance = Instance
-        
-        
-    def add_parser_usage(self,message):
-        """Usage to be used by the parser"""
-        usage = f"""
-{message}
-
-----------------  Examples:  ----------------
-
-usage:    autolab driver [options] args
-
-    autolab driver -D {self.name} -A TCPIP::192.168.0.4::INSTR -C VISA -a 0.5
-    load {self.name} driver using VISA communication protocol with address TCPIP... and set the amplitude to 0.5V
-    
-    autolab driver -D nickname -a 0.5
-    same as before but using the device nickname as defined in local_config.ini
-            """
-        return usage
-    
-    def add_parser_arguments(self,parser):
-        """Add arguments to the parser passed as input"""
-        parser.add_argument("-c", "--current", type=float, dest="current", default=None, help="Set the laser current in mA." )
-        return parser
-
-    def do_something(self,args):
-        if args.current:
-            getattr(self.Instance,'current')(args.current)
-
-    def exit(self):
-        self.Instance.close()
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Apr 17 09:27:19 2024
+
+@author: Jonathan
+"""
+
+
+class Driver_parser():
+    def __init__(self, Instance, name, **kwargs):
+        self.name     = name
+        self.Instance = Instance
+
+
+    def add_parser_usage(self,message):
+        """Usage to be used by the parser"""
+        usage = f"""
+{message}
+
+----------------  Examples:  ----------------
+
+usage:    autolab driver [options] args
+
+    autolab driver -D {self.name} -A GPIB::2::INSTR -C VISA
+    load {self.name} driver using VISA communication protocol with address GPIB...
+
+    autolab driver -D nickname
+    same as before but using the device nickname as defined in local_config.ini
+            """
+        return usage
+
+    def add_parser_arguments(self,parser):
+        """Add arguments to the parser passed as input"""
+        # parser.add_argument("-p", "--power", type=str, dest="power", default=None, help="Set the pump power setpoint in 1/10dBm (e.g. 100 <=> 10dBm; this conversion may depend on the model, please verify)." )
+
+        return parser
+
+    def do_something(self,args):
+        pass
+        # if args.power:
+        #     getattr(self.Instance,'set_power')(args.power)
+
+    def exit(self):
+        self.Instance.close()
```

### Comparing `autolab-1.1.9/autolab/scan.py` & `autolab-2.0b2/autolab/scan.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,517 +1,517 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Nov 22 21:03:46 2019
-
-@author: qchat
-"""
-from threading import Thread, Event
-from autolab.core import elements
-import collections
-import itertools
-import os
-import time
-import h5py
-
-class Scanner :
-    
-    def __init__(self):
-        
-        self._parameters = collections.OrderedDict()
-        self._recipe = collections.OrderedDict()
-        self._initrecipe = collections.OrderedDict()
-        self._endrecipe = collections.OrderedDict()
-    
-        self._name = 'scan'
-        self._datapath = os.path.realpath('./')
-        
-        self._thread = None
-        self.verbose = False
-        
-        
-    # Utilities
-    # =========================================================================
-    
-    def _check_item_name(self,name):
-        try : 
-            assert name not in self._parameters.keys()
-            assert name not in self._initrecipe.keys()
-            assert name not in self._recipe.keys()
-            assert name not in self._endrecipe.keys()
-        except :
-            raise ValueError(f"Item '{name}' already exists.")
-            
-    
-    def _check_modif_allowed(self):
-        assert self._thread is None, f"Scan is running, stop it first to modify it."
-
-            
-    def clear(self):
-        for obj_name in ['parameters','initrecipe','recipe','endrecipe']:
-            self._clear_object(obj_name)
-
-    def _add_item(self,obj_name,item_name,item):
-        self._check_modif_allowed()
-        self._check_item_name(item_name)
-        getattr(self, f'_{obj_name}')[item_name] = item
-        
-    def _clear_object(self,obj_name):
-        self._check_modif_allowed()
-        setattr(self, f'_{obj_name}', collections.OrderedDict())
-            
-        
-        
-    # Paths
-    # =========================================================================
-    
-    def set_datapath(self,path):
-        self._check_modif_allowed()
-        path = os.path.realpath(path)
-        assert os.path.exists(path), "This path doesn't exists."
-        self._datapath = path
-        
-    def get_datapath(self):
-        return self._datapath
-    
-    
-    
-    
-    # Scan name
-    # =========================================================================
-    
-    def set_name(self,name):
-        self._check_modif_allowed()
-        self._name = name
-        
-    def get_name(self,name):
-        return self._name
-
-
-        
-    # Parameters and recipe
-    # =========================================================================
-        
-    def add_parameter(self, param_name, parameter):
-        assert isinstance(parameter,Parameter), "Wrong object type"
-        self._add_item('parameters', param_name, parameter)
-        
-    def add_recipe_step(self, step_name, step):
-        assert isinstance(step,(Measure,Set,Execute,Wait)), "Wrong object type"
-        self._add_item('recipe', step_name, step)
-    
-    def add_init_recipe_step(self, step_name, step):
-        assert isinstance(step,(Measure,Set,Execute,Wait)), "Wrong object type"
-        self._add_item('initrecipe', step_name, step)
-     
-    def add_end_recipe_step(self, step_name, step):
-        assert isinstance(step,(Measure,Set,Execute,Wait)), "Wrong object type"
-        self._add_item('endrecipe', step_name, step)
-        
-    
-    def clear_parameters(self):
-        self._clear_object('parameters')
-
-    def clear_recipe(self):
-        self._clear_object('recipe')
-
-    def clear_init_recipe(self):
-        self._clear_object('intirecipe')
-
-    def clear_end_recipe(self):
-        self._clear_object('endrecipe')
-    
-    
-    
-    
-    
-    # Structure
-    # =========================================================================
-    
-    def show_configuration(self):
-        
-        ''' Prints the current configuration of the scan '''
-        
-        # Init recipe
-        print()
-        if len(self._initrecipe) == 0 : print("No init recipe\n"+'='*len('No init recipe'))
-        else : 
-            print('Init recipe:\n'+'='*len('Init recipe:'))
-            i = 1
-            for name in self._initrecipe.keys() :
-                print(f' {i}) {name}: {self._initrecipe[name].info()}')
-                i += 1
-                
-        # Parameters
-        indent = 0
-        print()
-        if len(self._parameters) == 0 : print("No parameters\n"+'='*len('No parameters'))
-        else : 
-            print('Parameters:\n'+'='*len('Parameters:'))
-            for name in self._parameters.keys() :
-                print("   "*indent+f' - {name}: {self._parameters[name].info()}')
-                indent += 1
-        
-        # Recipe
-        indent += 1
-        print()
-        if len(self._recipe) == 0 : print("   "*indent+"No recipe\n"+"   "*indent+'='*len('No recipe'))
-        else : 
-            print("   "*indent+'Recipe:\n'+"   "*indent+'='*len('Recipe:'))
-            i = 1
-            for name in self._recipe.keys() :
-                print("   "*indent+f' {i}) {name}: {self._recipe[name].info()}')
-                i += 1
-                
-        # End recipe
-        print()
-        if len(self._endrecipe) == 0 : print("No end recipe\n"+'='*len('No end recipe'))
-        else : 
-            print('End recipe:\n'+'='*len('End recipe:'))
-            i = 1
-            for name in self._endrecipe.keys() :
-                print(f' {i}) {name}: {self._endrecipe[name].info()}')
-                i += 1
-        
-        
-       
-        
-        
-        
-    # Scan state
-    # =========================================================================
-        
-    def start(self):
-        
-        ''' Start a new scan '''
-        
-        assert self._thread is None, f'The scan is already running'
-        self._thread = ScanThread(self)
-        self._thread.start()
-        if self.verbose : print('Scan started')
-        
-        
-        
-    def stop(self):
-        
-        ''' Stop the ongoing scan '''
-        
-        assert self._thread is not None, f'The scan is not running.'
-        self._thread.stop_event.set()
-        self._thread.join()
-        self._thread = None
-        if self.verbose : print('Scan stopped')
-        
-        
-        
-    def pause(self):
-        
-        ''' Pause the ongoing scan '''
-        
-        assert self._thread is not None, f'The scan is not running.'
-        self._thread.pause_event.set()
-        print('Scan paused')
-        
-        
-        
-    def resume(self):
-        
-        ''' Resume the ongoing scan '''
-        
-        assert self._thread is not None, f'The scan is not running.'
-        self._thread.pause_event.clear()
-        print('Scan resumed')
-        
-        
-        
-        
-        
-        
-        
-class ScanThread(Thread):
-    
-    def __init__(self,scanner):
-        
-        self.scanner = scanner
-        Thread.__init__(self)
-        
-        # Itertools product on parameters
-        self.param_sets = list(dict(zip(self.scanner._parameters.keys(),x)) for x in itertools.product(*[a.values for a in self.scanner._parameters.values()]) )
-            
-        # Pause and stop events
-        self.stop_event = Event()
-        self.pause_event = Event()
-        
-        # Current data
-        self.data = collections.OrderedDict()
-        
-        # Prepare datafile
-        self.prepare_datafile()
-        
-        
-        
-    def prepare_datafile(self):
-        
-        ''' Find a unique name for the datafile and initialize it size and name 
-        of parameters and step names '''
-        
-         # Create a unique name for the datafile
-        suffix = ''
-        count = 0
-        while os.path.exists(os.path.join(self.scanner._datapath,self.scanner._name+suffix+'.hdf5')) :
-            count += 1
-            suffix = f'_{count}'
-        self.datapath = os.path.join(self.scanner._datapath,self.scanner._name+suffix+'.hdf5')
-
-        # Prepare structure
-        def configure(file,obj,data_length):
-            for key in obj.keys(): 
-                if isinstance(obj[key],(Parameter,Measure)) :
-                    file.create_dataset(key, (data_length,))     
-        with h5py.File(self.datapath, "a") as file :
-            configure(file,self.scanner._initrecipe,1)
-            configure(file,self.scanner._parameters,len(self.param_sets))
-            configure(file,self.scanner._recipe,len(self.param_sets))
-            configure(file,self.scanner._endrecipe,1)
-
-
-
-    def run(self):
-        
-        ''' Start the execution of the scan '''
-        
-        # Init recipe
-        self.reset_data()
-        self.execute_recipe(self.scanner._initrecipe)
-        
-        # Main recipe of each set of parameter
-        self.reset_data()
-        for i in range(len(self.param_sets)) :
-            self.set_parameters(i)
-            self.execute_recipe(self.scanner._recipe,i)
-            
-        # End recipe
-        self.reset_data()
-        self.execute_recipe(self.scanner._endrecipe)
-        
-        
-        
-    def reset_data(self):
-        
-        ''' Reset the self.data dictionnary '''
-        
-        self.data = collections.OrderedDict()
-        
-        
-        
-    def execute_recipe(self,recipe,i=0):
-        
-        """ Execute the given recipe for the i-th time """
-        
-        for key in recipe.keys() :
-            
-            # If the scan has not been stopped
-            if self.stop_event.is_set() is False :
-                
-                # Execute step
-                step = recipe[key]
-                ans = step.execute()
-                if ans is not None :
-                    self.data[key] = ans
-                if self.scanner.verbose : print(key, step.info(), ans)
-                
-                # If scan is paused, wait for resume
-                while self.pause_event.is_set() :
-                    time.sleep(0.1)
-              
-            # If the scan has been stopped
-            else :
-                break
-        
-        # Save data
-        if self.stop_event.is_set() is False :
-            self.save_data(i)
-        
-        
-        
-    def set_parameters(self,i):
-        
-        """ Apply the i-th set of parameters """
-        
-        param_set = self.param_sets[i]
-        
-        for key in param_set.keys() :
-            
-            # If the scan has not been stopped
-            if self.stop_event.is_set() is False :
-                
-                value = param_set[key]
-                if key not in self.data.keys() or value != self.data[key] : 
-                    parameter = self.scanner._parameters[key]
-                    parameter.element(param_set[key])
-                    self.data[key] = value
-                    if self.scanner.verbose : print(key, parameter.info(), value)
-                    
-                # If scan is paused, wait for resume
-                while self.pause_event.is_set() :
-                    time.sleep(0.1)
-        
-            # If the scan has been stopped
-            else :
-                break
-            
-        # Save data
-        if self.stop_event.is_set() is False :
-            self.save_data(i)
-        
-        
-    
-    def save_data(self,i=0):
-        
-        """ Save in the whole content of the current self.data dictionnary 
-        in the hdf5 datafile """
-        
-        with h5py.File(self.datapath, "a") as file :
-            for key in self.data.keys():
-                file[key][i] = self.data[key]
-        if self.scanner.verbose : print('Saving data')
-            
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-# PARAMETERS AND STEPS
-# +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-        
-        
-class Parameter:
-    
-    ''' Class dedicated to parameter declaration '''
-    
-    def __init__(self,element,values):
-        assert isinstance(element,elements.Variable), "A parameter must be a Variable"
-        assert element.writable is True, f"SET step: Variable {element.address()} is not writable."
-        self.element = element
-        assert hasattr(values, '__iter__'), "Parameter values must be iterable"
-        self.values = values  
-        
-    def info(self):
-        return f"Sweep parameter {self.element.address()} with {len(self.values)} values."
-        
-        
-        
-        
-class Execute:
-    
-    ''' Scan step dedicated to execute an Action '''
-    
-    def __init__(self,element,value=None):
-        assert isinstance(element,elements.Action), "EXECUTE step element must be an Action."
-        self.element = element
-        self.value = None
-        if value is not None :
-            assert element.has_parameter is True, f"EXECUTE step: element {element.address()} has no parameter."
-            try : value = element.type(value)
-            except : raise ValueError(f'EXECUTE step: value must be of type {element.type}.')
-            self.value = value
-    
-    def info(self):
-        if self.value is None : return f'Execute action {self.element.address()}.'
-        else : return f'Execute action {self.element.address()} with value {self.value}.'
-        
-    def execute(self):
-        if self.value is None : self.element()
-        else : self.element(self.value)
-
-
-
-
-
-
-class Set:
-    
-    ''' Scan step dedicated to set the value of a Variable '''
-    
-    def __init__(self,element,value):
-        assert isinstance(element,elements.Variable), "SET step element must be a Variable."
-        assert element.writable is True, f"SET step: Variable {element.address()} is not writable."
-        self.element = element
-        try : value = element.type(value)
-        except : raise ValueError(f'SET step: value must be of type {element.type}.')
-        self.value = value
-        
-    def info(self):
-        return f'Set variable {self.element.address()} with value {self.value}.'
-        
-    def execute(self):
-        self.element(self.value)
-        
-        
-        
-        
-        
-class Measure:
-    
-    ''' Scan step dedicated to measure a Variable '''
-
-    def __init__(self,element):
-        assert isinstance(element,elements.Variable), "MEASURE step element must be a Variable."
-        assert element.readable is True, f"MEASURE step: Variable {element.address()} is not readable."
-        self.element = element
-        
-    def info(self):
-        return f'Measure variable {self.element.address()}.'
-        
-    def execute(self):
-        return self.element()
-
-
-
-
-
-class Wait:
-    
-    ''' Scan step dedicated to pause the scan from a certain amount of time '''
-    
-    def __init__(self,delay):
-        try : delay = float(delay)
-        except : raise ValueError('WAIT step delay must be numerical.')
-        self.delay = delay
-        
-    def info(self):
-        return f'Wait {self.value} seconds.'
-        
-    def execute(self):
-        time.sleep(self.delay)
- 
-    
-    
-# Futures classes, to be defined
- 
-#class WaitUser:
-#    
-#    def __init__(self):
-#        
-#        
-#    
-#class SendEmail:
-#    
-#    def __init__(self, address, message):
-#        
-#        
-#       
-#class While:
-#    
-#    def __init__(self, element, '<', value):
-#        
-#    def execute():
-#        while()
-#        
-        
-
+# -*- coding: utf-8 -*-
+"""
+Created on Fri Nov 22 21:03:46 2019
+
+@author: qchat
+"""
+from threading import Thread, Event
+from autolab.core import elements
+import collections
+import itertools
+import os
+import time
+import h5py
+
+class Scanner :
+    
+    def __init__(self):
+        
+        self._parameters = collections.OrderedDict()
+        self._recipe = collections.OrderedDict()
+        self._initrecipe = collections.OrderedDict()
+        self._endrecipe = collections.OrderedDict()
+    
+        self._name = 'scan'
+        self._datapath = os.path.realpath('./')
+        
+        self._thread = None
+        self.verbose = False
+        
+        
+    # Utilities
+    # =========================================================================
+    
+    def _check_item_name(self,name):
+        try : 
+            assert name not in self._parameters.keys()
+            assert name not in self._initrecipe.keys()
+            assert name not in self._recipe.keys()
+            assert name not in self._endrecipe.keys()
+        except :
+            raise ValueError(f"Item '{name}' already exists.")
+            
+    
+    def _check_modif_allowed(self):
+        assert self._thread is None, f"Scan is running, stop it first to modify it."
+
+            
+    def clear(self):
+        for obj_name in ['parameters','initrecipe','recipe','endrecipe']:
+            self._clear_object(obj_name)
+
+    def _add_item(self,obj_name,item_name,item):
+        self._check_modif_allowed()
+        self._check_item_name(item_name)
+        getattr(self, f'_{obj_name}')[item_name] = item
+        
+    def _clear_object(self,obj_name):
+        self._check_modif_allowed()
+        setattr(self, f'_{obj_name}', collections.OrderedDict())
+            
+        
+        
+    # Paths
+    # =========================================================================
+    
+    def set_datapath(self,path):
+        self._check_modif_allowed()
+        path = os.path.realpath(path)
+        assert os.path.exists(path), "This path doesn't exists."
+        self._datapath = path
+        
+    def get_datapath(self):
+        return self._datapath
+    
+    
+    
+    
+    # Scan name
+    # =========================================================================
+    
+    def set_name(self,name):
+        self._check_modif_allowed()
+        self._name = name
+        
+    def get_name(self,name):
+        return self._name
+
+
+        
+    # Parameters and recipe
+    # =========================================================================
+        
+    def add_parameter(self, param_name, parameter):
+        assert isinstance(parameter,Parameter), "Wrong object type"
+        self._add_item('parameters', param_name, parameter)
+        
+    def add_recipe_step(self, step_name, step):
+        assert isinstance(step,(Measure,Set,Execute,Wait)), "Wrong object type"
+        self._add_item('recipe', step_name, step)
+    
+    def add_init_recipe_step(self, step_name, step):
+        assert isinstance(step,(Measure,Set,Execute,Wait)), "Wrong object type"
+        self._add_item('initrecipe', step_name, step)
+     
+    def add_end_recipe_step(self, step_name, step):
+        assert isinstance(step,(Measure,Set,Execute,Wait)), "Wrong object type"
+        self._add_item('endrecipe', step_name, step)
+        
+    
+    def clear_parameters(self):
+        self._clear_object('parameters')
+
+    def clear_recipe(self):
+        self._clear_object('recipe')
+
+    def clear_init_recipe(self):
+        self._clear_object('intirecipe')
+
+    def clear_end_recipe(self):
+        self._clear_object('endrecipe')
+    
+    
+    
+    
+    
+    # Structure
+    # =========================================================================
+    
+    def show_configuration(self):
+        
+        ''' Prints the current configuration of the scan '''
+        
+        # Init recipe
+        print()
+        if len(self._initrecipe) == 0 : print("No init recipe\n"+'='*len('No init recipe'))
+        else : 
+            print('Init recipe:\n'+'='*len('Init recipe:'))
+            i = 1
+            for name in self._initrecipe.keys() :
+                print(f' {i}) {name}: {self._initrecipe[name].info()}')
+                i += 1
+                
+        # Parameters
+        indent = 0
+        print()
+        if len(self._parameters) == 0 : print("No parameters\n"+'='*len('No parameters'))
+        else : 
+            print('Parameters:\n'+'='*len('Parameters:'))
+            for name in self._parameters.keys() :
+                print("   "*indent+f' - {name}: {self._parameters[name].info()}')
+                indent += 1
+        
+        # Recipe
+        indent += 1
+        print()
+        if len(self._recipe) == 0 : print("   "*indent+"No recipe\n"+"   "*indent+'='*len('No recipe'))
+        else : 
+            print("   "*indent+'Recipe:\n'+"   "*indent+'='*len('Recipe:'))
+            i = 1
+            for name in self._recipe.keys() :
+                print("   "*indent+f' {i}) {name}: {self._recipe[name].info()}')
+                i += 1
+                
+        # End recipe
+        print()
+        if len(self._endrecipe) == 0 : print("No end recipe\n"+'='*len('No end recipe'))
+        else : 
+            print('End recipe:\n'+'='*len('End recipe:'))
+            i = 1
+            for name in self._endrecipe.keys() :
+                print(f' {i}) {name}: {self._endrecipe[name].info()}')
+                i += 1
+        
+        
+       
+        
+        
+        
+    # Scan state
+    # =========================================================================
+        
+    def start(self):
+        
+        ''' Start a new scan '''
+        
+        assert self._thread is None, f'The scan is already running'
+        self._thread = ScanThread(self)
+        self._thread.start()
+        if self.verbose : print('Scan started')
+        
+        
+        
+    def stop(self):
+        
+        ''' Stop the ongoing scan '''
+        
+        assert self._thread is not None, f'The scan is not running.'
+        self._thread.stop_event.set()
+        self._thread.join()
+        self._thread = None
+        if self.verbose : print('Scan stopped')
+        
+        
+        
+    def pause(self):
+        
+        ''' Pause the ongoing scan '''
+        
+        assert self._thread is not None, f'The scan is not running.'
+        self._thread.pause_event.set()
+        print('Scan paused')
+        
+        
+        
+    def resume(self):
+        
+        ''' Resume the ongoing scan '''
+        
+        assert self._thread is not None, f'The scan is not running.'
+        self._thread.pause_event.clear()
+        print('Scan resumed')
+        
+        
+        
+        
+        
+        
+        
+class ScanThread(Thread):
+    
+    def __init__(self,scanner):
+        
+        self.scanner = scanner
+        Thread.__init__(self)
+        
+        # Itertools product on parameters
+        self.param_sets = list(dict(zip(self.scanner._parameters.keys(),x)) for x in itertools.product(*[a.values for a in self.scanner._parameters.values()]) )
+            
+        # Pause and stop events
+        self.stop_event = Event()
+        self.pause_event = Event()
+        
+        # Current data
+        self.data = collections.OrderedDict()
+        
+        # Prepare datafile
+        self.prepare_datafile()
+        
+        
+        
+    def prepare_datafile(self):
+        
+        ''' Find a unique name for the datafile and initialize it size and name 
+        of parameters and step names '''
+        
+         # Create a unique name for the datafile
+        suffix = ''
+        count = 0
+        while os.path.exists(os.path.join(self.scanner._datapath,self.scanner._name+suffix+'.hdf5')) :
+            count += 1
+            suffix = f'_{count}'
+        self.datapath = os.path.join(self.scanner._datapath,self.scanner._name+suffix+'.hdf5')
+
+        # Prepare structure
+        def configure(file,obj,data_length):
+            for key in obj.keys(): 
+                if isinstance(obj[key],(Parameter,Measure)) :
+                    file.create_dataset(key, (data_length,))     
+        with h5py.File(self.datapath, "a") as file :
+            configure(file,self.scanner._initrecipe,1)
+            configure(file,self.scanner._parameters,len(self.param_sets))
+            configure(file,self.scanner._recipe,len(self.param_sets))
+            configure(file,self.scanner._endrecipe,1)
+
+
+
+    def run(self):
+        
+        ''' Start the execution of the scan '''
+        
+        # Init recipe
+        self.reset_data()
+        self.execute_recipe(self.scanner._initrecipe)
+        
+        # Main recipe of each set of parameter
+        self.reset_data()
+        for i in range(len(self.param_sets)) :
+            self.set_parameters(i)
+            self.execute_recipe(self.scanner._recipe,i)
+            
+        # End recipe
+        self.reset_data()
+        self.execute_recipe(self.scanner._endrecipe)
+        
+        
+        
+    def reset_data(self):
+        
+        ''' Reset the self.data dictionnary '''
+        
+        self.data = collections.OrderedDict()
+        
+        
+        
+    def execute_recipe(self,recipe,i=0):
+        
+        """ Execute the given recipe for the i-th time """
+        
+        for key in recipe.keys() :
+            
+            # If the scan has not been stopped
+            if self.stop_event.is_set() is False :
+                
+                # Execute step
+                step = recipe[key]
+                ans = step.execute()
+                if ans is not None :
+                    self.data[key] = ans
+                if self.scanner.verbose : print(key, step.info(), ans)
+                
+                # If scan is paused, wait for resume
+                while self.pause_event.is_set() :
+                    time.sleep(0.1)
+              
+            # If the scan has been stopped
+            else :
+                break
+        
+        # Save data
+        if self.stop_event.is_set() is False :
+            self.save_data(i)
+        
+        
+        
+    def set_parameters(self,i):
+        
+        """ Apply the i-th set of parameters """
+        
+        param_set = self.param_sets[i]
+        
+        for key in param_set.keys() :
+            
+            # If the scan has not been stopped
+            if self.stop_event.is_set() is False :
+                
+                value = param_set[key]
+                if key not in self.data.keys() or value != self.data[key] : 
+                    parameter = self.scanner._parameters[key]
+                    parameter.element(param_set[key])
+                    self.data[key] = value
+                    if self.scanner.verbose : print(key, parameter.info(), value)
+                    
+                # If scan is paused, wait for resume
+                while self.pause_event.is_set() :
+                    time.sleep(0.1)
+        
+            # If the scan has been stopped
+            else :
+                break
+            
+        # Save data
+        if self.stop_event.is_set() is False :
+            self.save_data(i)
+        
+        
+    
+    def save_data(self,i=0):
+        
+        """ Save in the whole content of the current self.data dictionnary 
+        in the hdf5 datafile """
+        
+        with h5py.File(self.datapath, "a") as file :
+            for key in self.data.keys():
+                file[key][i] = self.data[key]
+        if self.scanner.verbose : print('Saving data')
+            
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+# PARAMETERS AND STEPS
+# +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+        
+        
+class Parameter:
+    
+    ''' Class dedicated to parameter declaration '''
+    
+    def __init__(self,element,values):
+        assert isinstance(element,elements.Variable), "A parameter must be a Variable"
+        assert element.writable is True, f"SET step: Variable {element.address()} is not writable."
+        self.element = element
+        assert hasattr(values, '__iter__'), "Parameter values must be iterable"
+        self.values = values  
+        
+    def info(self):
+        return f"Sweep parameter {self.element.address()} with {len(self.values)} values."
+        
+        
+        
+        
+class Execute:
+    
+    ''' Scan step dedicated to execute an Action '''
+    
+    def __init__(self,element,value=None):
+        assert isinstance(element,elements.Action), "EXECUTE step element must be an Action."
+        self.element = element
+        self.value = None
+        if value is not None :
+            assert element.has_parameter is True, f"EXECUTE step: element {element.address()} has no parameter."
+            try : value = element.type(value)
+            except : raise ValueError(f'EXECUTE step: value must be of type {element.type}.')
+            self.value = value
+    
+    def info(self):
+        if self.value is None : return f'Execute action {self.element.address()}.'
+        else : return f'Execute action {self.element.address()} with value {self.value}.'
+        
+    def execute(self):
+        if self.value is None : self.element()
+        else : self.element(self.value)
+
+
+
+
+
+
+class Set:
+    
+    ''' Scan step dedicated to set the value of a Variable '''
+    
+    def __init__(self,element,value):
+        assert isinstance(element,elements.Variable), "SET step element must be a Variable."
+        assert element.writable is True, f"SET step: Variable {element.address()} is not writable."
+        self.element = element
+        try : value = element.type(value)
+        except : raise ValueError(f'SET step: value must be of type {element.type}.')
+        self.value = value
+        
+    def info(self):
+        return f'Set variable {self.element.address()} with value {self.value}.'
+        
+    def execute(self):
+        self.element(self.value)
+        
+        
+        
+        
+        
+class Measure:
+    
+    ''' Scan step dedicated to measure a Variable '''
+
+    def __init__(self,element):
+        assert isinstance(element,elements.Variable), "MEASURE step element must be a Variable."
+        assert element.readable is True, f"MEASURE step: Variable {element.address()} is not readable."
+        self.element = element
+        
+    def info(self):
+        return f'Measure variable {self.element.address()}.'
+        
+    def execute(self):
+        return self.element()
+
+
+
+
+
+class Wait:
+    
+    ''' Scan step dedicated to pause the scan from a certain amount of time '''
+    
+    def __init__(self,delay):
+        try : delay = float(delay)
+        except : raise ValueError('WAIT step delay must be numerical.')
+        self.delay = delay
+        
+    def info(self):
+        return f'Wait {self.value} seconds.'
+        
+    def execute(self):
+        time.sleep(self.delay)
+ 
+    
+    
+# Futures classes, to be defined
+ 
+#class WaitUser:
+#    
+#    def __init__(self):
+#        
+#        
+#    
+#class SendEmail:
+#    
+#    def __init__(self, address, message):
+#        
+#        
+#       
+#class While:
+#    
+#    def __init__(self, element, '<', value):
+#        
+#    def execute():
+#        while()
+#        
+        
+
```

### Comparing `autolab-1.1.9/scripts/autolab.py` & `autolab-2.0b2/autolab/_entry_script.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,302 +1,299 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-Created on Fri May 17 15:04:04 2019
-
-@author: quentin.chateiller
-"""
-
-
-import sys
-import autolab
-import argparse
-
-
-def print_help():
-    print()
-    print('Usage:')
-    print('  autolab [-h] <command> ...')
-    print()
-    print('Commands:')
-    print('  gui                   Start the Graphical User Interface')
-    print('  driver                Driver interface')
-    print('  device                Device interface')
-    print('  doc                   Open the online documentation (readthedocs)')
-    print('  report                Open the online report/suggestions webpage (github)')
-    print('  infos                 Displays the avalaible drivers and local configurations we ')
-    print('  stats                 Manage the data collection state')
-    print()
-    print('General Options:')
-    print('  -h, --help            Show this help message')
-    print()
-
-
-def main() :
-    
-    args = sys.argv
-    
-    # No command provided or -h/--help option : print help
-    if len(args)==1 or args[1]=='-h' or args[1]=='--help':
-        print_help()
-        
-    else :
-        command = args[1]   # first is 'autolab'
-        
-        # Update the sys.argv for parsers
-        args = [f'autolab {command}'] + args[2:]  # first is 'autolab' and second is command 
-        sys.argv = args
-        
-        if command=='doc':   # Open help on read the docs
-            autolab.doc()
-        elif command=='report':        # Open github report issue webpage
-            autolab.report()
-        elif command=='gui':           # GUI
-            autolab.gui()
-        elif command=='infos':           # GUI
-            autolab.infos()
-        elif command=='stats':
-            statistics(args)
-        elif command=='driver':
-            driver_parser(args)
-        elif command=='device':
-            device_parser(args)
-        else :
-            print(f"Command {command} not known. Autolab doesn't have Super Cow Power... yet ^^")
-              
-            
-    sys.exit()
-    
-####################################################################################
-################################## autolab stats ###################################      
-def statistics(args_list):
-    usage = f"""autolab stats [-h] [options]
-    
-Management of the anonymous data collection in Autolab.  \n\n
-{autolab._stats.get_explanation()}
-"""
-    parser = argparse.ArgumentParser(add_help=False,usage=usage)
-    parser.add_argument("-e", "--enable", action="store_true", dest="enable", help="Enable anonymous data collection." )
-    parser.add_argument("-d", "--disable", action="store_true", dest="disable", help="Disable anonymous data collection." )
-    parser.add_argument("-q", "--query", action="store_true", dest="query", help="Query anonymous data collection state." )
-    parser.add_argument("-h", "--help", action="store_true", dest="help", help="Display this help message." )
-    args, unknown = parser.parse_known_args(args_list)
-    
-    if len(args_list)==1 or args_list[1]=='-h' or args_list[1]=='--help': parser.print_help(); sys.exit()
-    assert not(args.enable and args.disable), "You may either enable or disable not both"
-    if args.query: print('Stats is ENABLED' if autolab.is_stats_enabled() else 'Stats is DISABLED')
-    elif args.enable: autolab.set_stats_enabled(True); print('Turning stats ON permanently')
-    elif args.disable: autolab.set_stats_enabled(False); print('Turning stats OFF permanently')
-################################## autolab stats ###################################
-####################################################################################
-
-####################################################################################
-######################### autolab driver/device utilities ##########################
-def process_config(args_list):
-    
-    parser = argparse.ArgumentParser(add_help=False)
-    parser.add_argument("-D", "--driver", type=str, dest="driver", help="Set the nickname or driver to use: 1) uses nickname if it is defined in local_config.ini OR(if it is not) 2) Set the driver name to use." )
-    parser.add_argument("-C", "--connection", type=str, dest="connection", help="Set the connection type to use for the connection." )
-    parser.add_argument("-A", "--address", type=str, dest="address", help="Set the address to use for the communication." )
-    parser.add_argument("-O","--other", nargs='+', dest="other", help="Set other parameters [ports (e.g SOCKET), board_index, slots,...)." )
-
-    args, unknown = parser.parse_known_args(args_list)
-    
-    config = {}
-    if args.connection is not None : config['connection'] = args.connection
-    if args.address is not None : config['address'] = args.address
-    if args.other is not None : 
-        for part in args.other : 
-            part = part.replace(' ','')
-            config[part.split('=')[0]] = part.split('=')[1]
-    
-    # Help for autolab driver/device -h/--help and autolab driver/device -h/--help -D driver_name
-    if not args.driver or (not args.driver and args_list[1]=='-h' or args_list[1]=='--help'): print_help_parser(parser,args_list); sys.exit()
-    if args.driver and (args_list[1]=='-h' or args_list[1]=='--help'): 
-        assert args.driver in autolab.list_drivers(), f"Driver {args.driver} not known"
-        autolab.config_help(args.driver,_parser=True)
-        sys.exit()
-    
-    return args.driver, config, parser
-
-def print_help_parser(parser,args_list):
-    parser.usage = f"""
-
-----------------  General informations:  ----------------
-
-This is a very basic help message for usage of {args_list[0]}. More info can be found on read the doc website (command: autolab doc). To display a more extensive help, please have a look at the section help below.
-    
-    Usage:   {args_list[0]} -D driver_name -C connection -A address -h
-
-Recquired connection arguments (capital letters):
-    -D driver_name: name of the driver to use (e.g.: agilent_33220A). driver_name can be either the driver_name or the defined nickname, as defined by the user in the local_config.ini. See below for accessing the list of available drivers.
-    -C connection type to use to communicate with the device (e.g.: VISA, VXI11, SOCKET, TELNET, USB, GPIB, ...). You may access the available connections types with an help (see below helps section).
-    -A address: full address to reach the device that depends on the connection type (e.g.: 192.168.0.2  [for VXI11]) and on the way you configured the instrument.
-    
-    
-----------------  Helps (-h option)  ----------------       
-
-Three helps are configured:
-    {args_list[0]} -h
-    Print this help message.
-    
-    {args_list[0]} -h -D driver_name
-    Print useful informations on the {args_list[0].split(' ')[1]}, including available connection types, etc.
-    
-    {args_list[0]} -D driver_name -C connection -A address -h
-    Full help message about the {args_list[0].split(' ')[1]}. This requires the address to be valid and the {args_list[0].split(' ')[1]} to be instantiated.
-    
-    
-----------------  List of available drivers and local configurations (-D option) ----------------
-   
-To display the full list of available drivers and local configurations, use:
-    autolab infos
-    
-
----------------- Accepted options ----------------"""
-    
-    parser.print_help()
-########################## autolab driver/device utilities ##########################
-#####################################################################################
-
-
-#####################################################################################
-################################## autolab driver ###################################
-def driver_parser(args_list):
-    # Reading of connection information
-    driver_name, config, parser = process_config(args_list)
-    
-    # Reading of methods
-    parser.add_argument("-m", "--methods", nargs='+', dest="methods", help="Set the methods to use." )
-    parser.add_argument("-h", "--help", dest="help", help="Print this help message." )
-    
-    # Instantiation of driver.py and driver_utilities.py
-    global driver_instance
-    driver_instance           = autolab.get_driver(driver_name,**config)
-    
-    if driver_name in autolab.list_local_configs():        
-        # Load config object
-        config = dict(autolab.get_local_config(driver_name))
-        # Check if driver provided
-        assert 'driver' in config.keys(), f"Driver name not found in driver config '{driver_name}'"
-        driver_name = config['driver']
-        
-    driver_utilities          = autolab.load_driver_utilities_lib(driver_name+'_utilities')
-    driver_utilities_instance = driver_utilities.Driver_parser(driver_instance,driver_name)
-    
-    # Add arguments to the existing parser (driver dependant)
-    parser = driver_utilities_instance.add_parser_arguments(parser)
-    
-    # Add help and usage to the parser only if "-h" options requested
-    if '-h' in args_list:
-        dirver_infos_for_usage = build_driver_infos_for_usage(driver_name,driver_instance)
-        parser.usage = driver_utilities_instance.add_parser_usage(dirver_infos_for_usage)
-        parser.usage = parser.usage + f"""
-    autolab driver -D nickname -m 'some_methods1(arg1,arg2=23)' 'some_methods2(arg1="test")'
-    Execute some_methods of the driver. A list of available methods is present at the top of this help along with arguments definition. Note if strings are passed as arguments, mind the usage of ' and " (follow some_methods2 example)."""
-        parser.print_help()
-        sys.exit()
-        
-    args = parser.parse_args()
-
-    # Finally, execute functions according to the arguments provided
-    driver_utilities_instance.do_something(args)
-    
-    # Process given methods
-    if args.methods:
-        global message
-        method_list = [method_args[0] for method_args in autolab.get_instance_methods(driver_instance)]
-        for method in args.methods:
-            message = None
-            print(method)
-            assert method.split('(')[0] in method_list, f"Method {method} not known or bound. Methods known are: {method_list}"
-            print(f'\nExecuting command:  {method}')
-            exec(f"message = driver_instance.{method}",globals())
-            if message is not None: print(f'Return:  {message}\n')
-    
-    # Driver closing
-    driver_utilities_instance.exit()
-
-def build_driver_infos_for_usage(driver_name,driver_instance):
-    driver_lib = autolab.load_driver_lib(driver_name)
-    
-    # build necessary list
-    list_connection_classes = autolab.get_connection_names(driver_lib)
-    list_additional_classes = autolab.get_module_names(driver_lib)
-    list_instance_methods_and_args = autolab.get_instance_methods(driver_instance)
-    
-    mess = '\n----------------  Driver informations:  ----------------\n'
-    mess += '\n    Available connections types (-C option):\n'
-    for connection in list_connection_classes: 
-        mess += f'     - {connection}\n'
-    mess += '\n'
-    mess += '\n    Available additional modules:\n'
-    if list_additional_classes==[]:
-        mess += f'     {list_additional_classes}'
-    else:
-        for additional_class in list_additional_classes: 
-            mess += f'     - {additional_class}\n'
-    mess += '\n'
-    mess += '\n    Available methods (with arguments):'
-    for method in list_instance_methods_and_args:
-        mess += f'\n     - {method[0]}({",".join(method[1])})'
-    mess += '\n'
-            
-    return mess
-################################## autolab driver ###################################   
-#####################################################################################
-
-
-#####################################################################################
-################################## autolab device ###################################
-def device_parser(args_list):
-    
-    # autolab device -D mydummy -e amplitude -p C:\Users\               GET AND SAVE VARIABLE VALUE
-    # autolab device -D mydummy -e something                            EXECUTE ACTION
-    # autolab device -D mydummy -e amplitude -v 4                       SET VARIABLE VALUE
-    # autolab device -D mydummy -e channel1.amplitude -h                DISPLAY ELEMENT HELP
-
-    # Reading of connection information
-    driver_name, config, parser = process_config(args_list)
-    
-    # Parser configuration
-    parser.add_argument('-e', '--element', type=str, dest="element", help='Address of the element to open' )
-    parser.add_argument("-v", "--value", type=str, dest="value", help='Value to set')
-    parser.add_argument("-p", "--path", type=str, dest="path", help='Path where to save data')
-    parser.add_argument("-h", "--help", action='store_true', dest="help", help='Display element help')
-    
-    # In autolab driver, this is done after the last help request
-    args, unknown = parser.parse_known_args(args_list)
-
-    # Instantiation
-    instance = autolab.get_device(driver_name,**config)
-    element = instance
-    
-    # Open element
-    if args.element is not None :
-        for name in args.element.split('.') :
-            element = getattr(element,name)
-        
-    # Execute order
-    if args.help is True : element.help()
-        
-    elif args.path is not None: 
-        assert element._element_type == 'variable', f"This element is not a Variable"
-        value = element()
-        element.save(args.path,value=value)
-        
-    elif args.value is not None :
-        if element._element_type == 'variable' : element(args.value)
-        elif element._element_type == 'action' : element(args.value)
-        
-    else :
-        assert element._element_type in ['variable','action'], f"Please provide a Variable or Action element"
-        if element._element_type == 'variable' : print(element())
-        elif element._element_type == 'action' : element()
-    
-    instance.close()
-################################## autolab device ###################################
-#####################################################################################
-
-
-if __name__ == '__main__' : 
-    main()
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+"""
+Created on Fri May 17 15:04:04 2019
+
+@author: quentin.chateiller
+"""
+
+import sys
+import argparse
+from typing import List, Type
+
+import autolab
+
+
+def print_help():
+    print(f'Autolab {autolab.__version__}')
+    print()
+    print('Usage:')
+    print('  autolab [-h] <command> ...')
+    print()
+    print('Commands:')
+    print('  gui                   Start the Graphical User Interface')
+    print('  install_drivers       Install drivers from GitHub')
+    print('  driver                Driver interface')
+    print('  device                Device interface')
+    print('  doc                   Open the online documentation (readthedocs)')
+    print('  report                Open the online report/suggestions webpage (github)')
+    print('  infos                 Displays the available drivers and devices configuration')
+    print()
+    print('General Options:')
+    print('  -h, --help            Show this help message')
+    print()
+
+
+def main():
+
+    args = sys.argv
+
+    # No command provided or -h/--help option : print help
+    if (len(args) == 1) or (args[1] == '-h') or (args[1] == '--help'):
+        print_help()
+
+    else:
+        command = args[1]   # first is 'autolab'
+
+        # Update the sys.argv for parsers
+        args = [f'autolab {command}'] + args[2: ]  # first is 'autolab' and second is command
+        sys.argv = args
+
+        if command == 'doc':   # Open help on read the docs
+            autolab.doc()
+        elif command == 'report':        # Open github report issue webpage
+            autolab.report()
+        elif command == 'gui':           # GUI
+            autolab.gui()
+        elif command == 'infos':
+            autolab.infos()
+        elif command == 'install_drivers':
+            autolab.install_drivers()
+        elif command == 'driver':
+            driver_parser(args)
+        elif command == 'device':
+            device_parser(args)
+        else:
+            print(f"Command {command} not known. Autolab doesn't have Super Cow Power... yet ^^")
+
+    sys.exit()
+
+
+####################################################################################
+######################### autolab driver/device utilities ##########################
+def process_config(args_list: List[str]):
+
+    parser = argparse.ArgumentParser(add_help=False)
+    parser.add_argument("-D", "--driver", type=str, dest="driver", help="Set the nickname or driver to use: 1) uses nickname if it is defined in devices_config.ini OR(if it is not) 2) Set the driver name to use." )
+    parser.add_argument("-C", "--connection", type=str, dest="connection", help="Set the connection type to use for the connection." )
+    parser.add_argument("-A", "--address", type=str, dest="address", help="Set the address to use for the communication." )
+    parser.add_argument("-O", "--other", nargs='+', dest="other", help="Set other parameters [ports (e.g SOCKET), board_index, slots,...)." )
+
+    args, unknown = parser.parse_known_args(args_list)
+
+    config = {}
+    if args.connection is not None: config['connection'] = args.connection
+    if args.address is not None: config['address'] = args.address
+    if args.other is not None:
+        for part in args.other:
+            part = part.replace(' ', '')
+            config[part.split('=')[0]] = part.split('=')[1]
+
+    # Help for autolab driver/device -h/--help and autolab driver/device -h/--help -D driver_name
+    if not args.driver or (
+            (not args.driver
+             and args_list[1] == '-h') or args_list[1] == '--help'):
+        print_help_parser(parser,args_list); sys.exit()
+    if args.driver and (args_list[1] == '-h' or args_list[1] == '--help'):
+        if args.driver in autolab._devices.list_devices():
+            try:
+                args.driver = autolab._devices.get_final_device_config(args.driver)["driver"]
+            except:
+                pass
+        assert args.driver in autolab._drivers.list_drivers(), f"Driver {args.driver} not known"
+        autolab.config_help(args.driver,_parser=True)
+        sys.exit()
+
+    return args.driver, config, parser
+
+
+def print_help_parser(parser: argparse.ArgumentParser, args_list: List[str]):
+    parser.usage = f"""
+
+----------------  General informations:  ----------------
+
+This is a very basic help message for usage of {args_list[0]}. More info can be found on read the doc website (command: autolab doc). To display a more extensive help, please have a look at the section help below.
+
+    Usage:   {args_list[0]} -D driver_name -C connection -A address -h
+
+Recquired connection arguments (capital letters):
+    -D driver_name: name of the driver to use (e.g.: agilent_33220A). driver_name can be either the driver_name or the defined nickname, as defined by the user in the devices_config.ini. See below for accessing the list of available drivers.
+    -C connection type to use to communicate with the device (e.g.: VISA, VXI11, SOCKET, TELNET, USB, GPIB, ...). You may access the available connections types with an help (see below helps section).
+    -A address: full address to reach the device that depends on the connection type (e.g.: 192.168.0.2  [for VXI11]) and on the way you configured the instrument.
+
+
+----------------  Helps (-h option)  ----------------
+
+Three helps are configured:
+    {args_list[0]} -h
+    Print this help message.
+
+    {args_list[0]} -h -D driver_name
+    Print useful informations on the {args_list[0].split(' ')[1]}, including available connection types, etc.
+
+    {args_list[0]} -D driver_name -C connection -A address -h
+    Full help message about the {args_list[0].split(' ')[1]}. This requires the address to be valid and the {args_list[0].split(' ')[1]} to be instantiated.
+
+
+----------------  List of available drivers and local configurations (-D option) ----------------
+
+To display the full list of available drivers and local configurations, use:
+    autolab infos
+
+
+---------------- Accepted options ----------------"""
+
+    parser.print_help()
+########################## autolab driver/device utilities ##########################
+#####################################################################################
+
+
+#####################################################################################
+################################## autolab driver ###################################
+def driver_parser(args_list: List[str]):
+
+    # autolab driver -D mydummy -C CONN -A GPIB0::5::INSTR -m set_verbose(1)
+    # autolab driver -D mydummy -C CONN -A GPIB0::5::INSTR -verb 1
+
+    # Reading of connection information
+    driver_name, config, parser = process_config(args_list)
+
+    # Reading of methods
+    parser.add_argument("-m", "--methods", nargs='+', dest="methods", help="Set the methods to use." )
+    parser.add_argument("-h", "--help", dest="help", help="Print this help message." )
+
+    # Instantiation of driver.py and driver_utilities.py
+    global driver_instance
+    assert 'connection' in config.keys(), f"Must provide a connection for the driver using -C connection with connection being for this driver among {autolab._drivers.get_connection_names(autolab._drivers.load_driver_lib(driver_name))}"
+    driver_instance = autolab.get_driver(driver_name, **config)
+
+    if driver_name in autolab._config.list_all_devices_configs():
+        # Load config object
+        config = dict(autolab._config.get_device_config(driver_name))
+        # Check if driver provided
+        assert 'driver' in config.keys(), f"Driver name not found in driver config '{driver_name}'"
+        driver_name = config['driver']
+
+    driver_utilities = autolab._drivers.load_driver_utilities_lib(driver_name + '_utilities')
+    driver_utilities_instance = driver_utilities.Driver_parser(driver_instance, driver_name)
+
+    # Add arguments to the existing parser (driver dependant)
+    parser = driver_utilities_instance.add_parser_arguments(parser)
+
+    # Add help and usage to the parser only if "-h" options requested
+    if '-h' in args_list:
+        dirver_infos_for_usage = build_driver_infos_for_usage(driver_name, driver_instance)
+        parser.usage = driver_utilities_instance.add_parser_usage(dirver_infos_for_usage)
+        parser.usage = parser.usage + """
+    autolab driver -D nickname -m 'some_methods1(arg1,arg2=23)' 'some_methods2(arg1="test")'
+    Execute some_methods of the driver. A list of available methods is present at the top of this help along with arguments definition. Note if strings are passed as arguments, mind the usage of ' and " (follow some_methods2 example)."""
+        parser.print_help()
+        sys.exit()
+
+    args = parser.parse_args()
+
+    # Finally, execute functions according to the arguments provided
+    driver_utilities_instance.do_something(args)
+
+    # Process given methods
+    if args.methods:
+        global message
+        method_list = [method_args[0] for method_args in autolab._drivers.get_instance_methods(driver_instance)]
+        for method in args.methods:
+            message = None
+            print(method)
+            assert method.split('(')[0] in method_list, f"Method {method} not known or bound. Methods known are: {method_list}"
+            print(f'\nExecuting command:  {method}')
+            exec(f"message = driver_instance.{method}", globals())
+            if message is not None: print(f'Return:  {message}\n')
+
+    # Driver closing
+    driver_utilities_instance.exit()
+
+def build_driver_infos_for_usage(driver_name: str, driver_instance: Type):
+    driver_lib = autolab._drivers.load_driver_lib(driver_name)
+
+    # build necessary list
+    list_connection_classes = autolab._drivers.get_connection_names(driver_lib)
+    list_additional_classes = autolab._drivers.get_module_names(driver_lib)
+    list_instance_methods_and_args = autolab._drivers.get_instance_methods(driver_instance)
+
+    mess = '\n----------------  Driver informations:  ----------------\n'
+    mess += '\n    Available connections types (-C option):\n'
+    for connection in list_connection_classes:
+        mess += f'     - {connection}\n'
+    mess += '\n'
+    mess += '\n    Available additional modules:\n'
+    if list_additional_classes==[]:
+        mess += f'     {list_additional_classes}'
+    else:
+        for additional_class in list_additional_classes:
+            mess += f'     - {additional_class}\n'
+    mess += '\n'
+    mess += '\n    Available methods (with arguments):'
+    for method in list_instance_methods_and_args:
+        mess += f'\n     - {method[0]}({",".join(method[1])})'
+    mess += '\n'
+
+    return mess
+################################## autolab driver ###################################
+#####################################################################################
+
+
+#####################################################################################
+################################## autolab device ###################################
+def device_parser(args_list: List[str]):
+
+    # autolab device -D mydummy -e amplitude -p C:\Users\               GET AND SAVE VARIABLE VALUE
+    # autolab device -D mydummy -e something                            EXECUTE ACTION
+    # autolab device -D mydummy -e amplitude -v 4                       SET VARIABLE VALUE
+    # autolab device -D mydummy -e channel1.amplitude -h                DISPLAY ELEMENT HELP
+
+    # Reading of connection information
+    driver_name, config, parser = process_config(args_list)
+
+    # Parser configuration
+    parser.add_argument('-e', '--element', type=str, dest="element", help='Address of the element to open' )
+    parser.add_argument("-v", "--value", type=str, dest="value", help='Value to set')
+    parser.add_argument("-p", "--path", type=str, dest="path", help='Path where to save data')
+    parser.add_argument("-h", "--help", action='store_true', dest="help", help='Display element help')
+
+    # In autolab driver, this is done after the last help request
+    if "-e" in list(set([x for x in args_list if args_list.count(x) >= 2])):
+        print("Warning, device will only consider the last element provided with -e. Use driver instead to do multiple operations in the same command")
+
+    args, unknown = parser.parse_known_args(args_list)
+
+    # Instantiation
+    instance = autolab.get_device(driver_name, **config)
+    element = instance
+
+    # Open element
+    if args.element is not None:
+        for name in args.element.split('.'):
+            element = getattr(element, name)
+
+    # Execute order
+    if args.help: element.help()
+
+    elif args.path is not None:
+        assert element._element_type == 'variable', "This element is not a Variable"
+        value = element()
+        element.save(args.path,value=value)
+
+    elif args.value is not None:
+        assert element._element_type in ('variable', 'action'), "Please provide a Variable or Action element using -e <element>"
+        if element._element_type == 'variable': element(args.value)
+        elif element._element_type == 'action': element(args.value)
+    else:
+        if element._element_type == 'variable': print(element())
+        elif element._element_type == 'action': element()
+
+    args = parser.parse_args()  # return error if give bad arg
+
+    instance.close()
+################################## autolab device ###################################
+#####################################################################################
+
+
+if __name__ == '__main__':
+    main()
```

