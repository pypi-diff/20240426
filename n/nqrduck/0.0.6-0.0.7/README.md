# Comparing `tmp/nqrduck-0.0.6.tar.gz` & `tmp/nqrduck-0.0.7.tar.gz`

## Comparing `nqrduck-0.0.6.tar` & `nqrduck-0.0.7.tar`

### file list

```diff
@@ -1,61 +1,63 @@
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nqrduck-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 nqrduck-0.0.6/.github/workflows/main.yml
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 nqrduck-0.0.6/.github/workflows/ubuntu-python-package.yml
--rw-r--r--   0        0        0  1509874 2020-02-02 00:00:00.000000 nqrduck-0.0.6/docs/img/ui_structure_v2.png
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/__init__.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/__main__.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/animations.py
--rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/icons.py
--rw-r--r--   0        0        0    27758 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/animations/DuckKick_128x128.gif
--rw-r--r--   0        0        0   115443 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/animations/DuckSleep_128x128.gif
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/ArrowLeft_12x12.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/ArrowRight_12x12.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Attention_16x16.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Error_16x16.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Garbage_12x12.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Info_16x16.png
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/LabMallardnbg_32x32.png
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Load_16x16.png
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Logo_64x32.png
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Logo_full.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/New_16x16.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Pen_12x12.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Play_16x16.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/QuestionMark_16x16.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Save_16x16.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/logos/Settings_16x16.png
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/pulseparameters/GateOff.png
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/pulseparameters/GateOn.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/pulseparameters/RXOff.png
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/pulseparameters/RXOn.png
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/pulseparameters/TXCustom.png
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/pulseparameters/TXGauss.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/pulseparameters/TXOff.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/pulseparameters/TXRect.png
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/assets/pulseparameters/TXSinc.png
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/contrib/mplwidget.py
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/core/main_controller.py
--rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/core/main_model.py
--rw-r--r--   0        0        0    31378 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/core/main_view.py
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/core/main_window.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/core/resources/logo.png
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/core/resources/main_window.ui
--rw-r--r--   0        0        0    28916 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/core/resources/font/AsepriteFont.ttf
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/core/resources/font/LICENCE
--rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/helpers/duckwidgets.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/helpers/serializer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/helpers/signalprocessing.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/helpers/unitconverter.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/helpers/validators.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/module/__init__.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/module/module.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/module/module_controller.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/module/module_model.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 nqrduck-0.0.6/src/nqrduck/module/module_view.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nqrduck-0.0.6/tests/test_load_module.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nqrduck-0.0.6/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 nqrduck-0.0.6/LICENSE
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 nqrduck-0.0.6/README.md
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 nqrduck-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 nqrduck-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nqrduck-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nqrduck-0.0.7/.github/workflows/main.yml
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 nqrduck-0.0.7/.github/workflows/ubuntu-python-package.yml
+-rw-r--r--   0        0        0  1509874 2020-02-02 00:00:00.000000 nqrduck-0.0.7/docs/img/ui_structure_v2.png
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/__init__.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/__main__.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/animations.py
+-rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/icons.py
+-rw-r--r--   0        0        0    27758 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/animations/DuckKick_128x128.gif
+-rw-r--r--   0        0        0   115443 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/animations/DuckSleep_128x128.gif
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/ArrowLeft_12x12.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/ArrowRight_12x12.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Attention_16x16.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Error_16x16.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Garbage_12x12.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Info_16x16.png
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/LabMallardnbg_32x32.png
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Load_16x16.png
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Logo_64x32.png
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Logo_full.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/New_16x16.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Pen_12x12.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Play_16x16.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/QuestionMark_16x16.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Save_16x16.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/logos/Settings_16x16.png
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/GateOff.png
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/GateOn.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/RXOff.png
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/RXOn.png
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/TXCustom.png
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/TXGauss.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/TXOff.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/TXRect.png
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/assets/pulseparameters/TXSinc.png
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/contrib/mplwidget.py
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/main_controller.py
+-rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/main_model.py
+-rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/main_view.py
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/main_window.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/resources/logo.png
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/resources/main_window.ui
+-rw-r--r--   0        0        0    28916 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/resources/font/AsepriteFont.ttf
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/core/resources/font/LICENCE
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/duckwidgets.py
+-rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/formbuilder.py
+-rw-r--r--   0        0        0    12683 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/functions.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/serializer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/signalprocessing.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/unitconverter.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/helpers/validators.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/module/__init__.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/module/module.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/module/module_controller.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/module/module_model.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 nqrduck-0.0.7/src/nqrduck/module/module_view.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nqrduck-0.0.7/tests/test_load_module.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nqrduck-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 nqrduck-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nqrduck-0.0.7/README.md
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 nqrduck-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 nqrduck-0.0.7/PKG-INFO
```

### Comparing `nqrduck-0.0.6/.github/workflows/python-publish.yml` & `nqrduck-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/.github/workflows/ubuntu-python-package.yml` & `nqrduck-0.0.7/.github/workflows/ubuntu-python-package.yml`

 * *Files 15% similar despite different names*

```diff
@@ -27,11 +27,11 @@
         sudo apt-get update
         sudo apt-get -qq install python3-pyqt5 xvfb libgl1 xvfb libxkbcommon-dev libegl1 fontconfig libxcb-cursor0
         python -m pip install --upgrade pip
         pip install pytest
 
     - name: Install test module and dependencies
       run: |
-        pip install .[nqrduck-module]
+        pip install nqrduck-module
 
     - name: Run all the tests
       run: xvfb-run pytest tests/
```

### Comparing `nqrduck-0.0.6/docs/img/ui_structure_v2.png` & `nqrduck-0.0.7/docs/img/ui_structure_v2.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/__main__.py` & `nqrduck-0.0.7/src/nqrduck/__main__.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/assets/animations.py` & `nqrduck-0.0.7/src/nqrduck/assets/animations.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/assets/icons.py` & `nqrduck-0.0.7/src/nqrduck/assets/icons.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/assets/animations/DuckKick_128x128.gif` & `nqrduck-0.0.7/src/nqrduck/assets/animations/DuckKick_128x128.gif`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/assets/animations/DuckSleep_128x128.gif` & `nqrduck-0.0.7/src/nqrduck/assets/animations/DuckSleep_128x128.gif`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/assets/logos/LabMallardnbg_32x32.png` & `nqrduck-0.0.7/src/nqrduck/assets/logos/LabMallardnbg_32x32.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/assets/logos/Logo_64x32.png` & `nqrduck-0.0.7/src/nqrduck/assets/logos/Logo_64x32.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/assets/logos/Logo_full.png` & `nqrduck-0.0.7/src/nqrduck/assets/logos/Logo_full.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/contrib/mplwidget.py` & `nqrduck-0.0.7/src/nqrduck/contrib/mplwidget.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/core/main_controller.py` & `nqrduck-0.0.7/src/nqrduck/core/main_controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/core/main_model.py` & `nqrduck-0.0.7/src/nqrduck/core/main_model.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/core/main_view.py` & `nqrduck-0.0.7/src/nqrduck/core/main_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,15 @@
         mpl.rcParams["axes.unicode_minus"] = False
         mpl.rcParams["font.family"] = "sans-serif"
         mpl.rcParams["font.sans-serif"] = self._main_model.settings.settings.value(
             "font"
         )
         mpl.rcParams["font.size"] = font_size
 
-        logger.debug("Set stylesheet to %s" % self.styleSheet())
+        logger.debug(f"Set stylesheet to {self.styleSheet()}")
 
         mpl.rcParams.update(
             {
                 "figure.facecolor": (0.0, 0.0, 0.0, 0.00),  # transparent
                 "axes.facecolor": (0.0, 1.0, 0.0, 0.03),  # green
                 "savefig.facecolor": (0.0, 0.0, 0.0, 0.0),  # transparent
             }
@@ -335,15 +335,15 @@
             self.color = Qt.GlobalColor.yellow
             # self.icon = QIcon('path_to_warning_icon')
         elif type == "Error":
             self.color = Qt.GlobalColor.red
             # self.icon = QIcon('path_to_error_icon')
 
         self.messageLabel = QLabel(message)
-        self.messageLabel.setStyleSheet("QLabel { color : %s }" % self.color.name)
+        self.messageLabel.setStyleSheet(f"QLabel color :{self.color.name}")
         # self.iconLabel = QLabel()
         # self.iconLabel.setPixmap(self.icon.pixmap(32, 32))
 
         self.layout.addWidget(self.messageLabel)
         # self.layout.addWidget(self.iconLabel)
 
         self.setLayout(self.layout)
```

### Comparing `nqrduck-0.0.6/src/nqrduck/core/main_window.py` & `nqrduck-0.0.7/src/nqrduck/core/main_window.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/core/resources/logo.png` & `nqrduck-0.0.7/src/nqrduck/core/resources/logo.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/core/resources/main_window.ui` & `nqrduck-0.0.7/src/nqrduck/core/resources/main_window.ui`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/core/resources/font/AsepriteFont.ttf` & `nqrduck-0.0.7/src/nqrduck/core/resources/font/AsepriteFont.ttf`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/helpers/duckwidgets.py` & `nqrduck-0.0.7/src/nqrduck/helpers/duckwidgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -159,14 +159,16 @@
             self.spin_box = QSpinBox()
 
         # Maker the SpinBox 5 digits wide
         self.spin_box.setMinimumWidth(80)
 
         if min_value is not None and max_value is not None:
             self.spin_box.setRange(min_value, max_value)
+        else:
+            self.spin_box.setRange(-100000, 100000)
         self.spin_box.valueChanged.connect(self.on_value_changed)
 
         # This only can be an issue during development, better to catch it early
         assert not( slider is True and (min_value is None or max_value is None)), "If a slider is added, min_value and max_value must be set."
 
         if slider:
             self.slider = QSlider(Qt.Orientation.Horizontal)
@@ -195,7 +197,24 @@
 
         Args:
             value (int): The new value of the QSlider.
         """
         self.state_updated.emit(True, str(value))
         self.spin_box.setValue(value)
 
+    def set_value(self, value):
+        """Sets the value of the QSpinBox.
+
+        Args:
+            value (int): The value that should be set.
+        """
+        self.spin_box.setValue(value)
+        self.state_updated.emit(True, str(value))
+
+    def value(self):
+        """Returns the value of the QSpinBox.
+
+        Returns:
+            int: The value of the QSpinBox.
+        """
+        return self.spin_box.value()
+
```

### Comparing `nqrduck-0.0.6/src/nqrduck/helpers/serializer.py` & `nqrduck-0.0.7/src/nqrduck/helpers/serializer.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/helpers/signalprocessing.py` & `nqrduck-0.0.7/src/nqrduck/helpers/signalprocessing.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/helpers/unitconverter.py` & `nqrduck-0.0.7/src/nqrduck/helpers/unitconverter.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,16 +14,36 @@
         
         Args:
             value (str): The value to be converted
 
         Returns:
             decimal.Decimal: The converted value
         """
-        if value[-1] == "n":
-            return decimal.Decimal(value[:-1]) * decimal.Decimal("1e-9")
-        elif value[-1] == "u":
-            return decimal.Decimal(value[:-1]) * decimal.Decimal("1e-6")
-        elif value[-1] == "m":
-            return decimal.Decimal(value[:-1]) * decimal.Decimal("1e-3")
-        else:
+        try:
+            if value[-1] == "n":
+                return decimal.Decimal(value[:-1]) * decimal.Decimal("1e-9")
+            elif value[-1] == "u":
+                return decimal.Decimal(value[:-1]) * decimal.Decimal("1e-6")
+            elif value[-1] == "m":
+                return decimal.Decimal(value[:-1]) * decimal.Decimal("1e-3")
+            else:
+                return decimal.Decimal(value)
+        except TypeError:
             return decimal.Decimal(value)
 
+    @classmethod    
+    def to_float(cls, value : str) -> float:
+        """This method checks if the last character of the string is a suffix.
+
+        The available suffixes are:
+        - n for nano
+        - u for micro
+        - m for milli
+        
+        Args:
+            value (str): The value to be converted
+
+        Returns:
+            float: The converted value
+        """
+        return float(cls.to_decimal(value))
+
```

### Comparing `nqrduck-0.0.6/src/nqrduck/helpers/validators.py` & `nqrduck-0.0.7/src/nqrduck/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/module/module.py` & `nqrduck-0.0.7/src/nqrduck/module/module.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/module/module_controller.py` & `nqrduck-0.0.7/src/nqrduck/module/module_controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/module/module_model.py` & `nqrduck-0.0.7/src/nqrduck/module/module_model.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/src/nqrduck/module/module_view.py` & `nqrduck-0.0.7/src/nqrduck/module/module_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,12 +87,12 @@
                 "QFileManager - Save File",
                 "",
                 f"{extension_name} Files (*.{self.extension});;All Files (*)",
                 options=QFileDialog.Option.DontUseNativeDialog,
             )
             if fileName:
                 # Append the .quack extension if not present
-                if not fileName.endswith(".%s" % self.extension):
-                    fileName += ".%s" % self.extension
+                if not fileName.endswith(f".{self.extension}"):
+                    fileName += f".{self.extension}"
                 return fileName
             else:
                 return None
```

### Comparing `nqrduck-0.0.6/tests/test_load_module.py` & `nqrduck-0.0.7/tests/test_load_module.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/LICENSE` & `nqrduck-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.6/README.md` & `nqrduck-0.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 2. Create a virtual environment and activate it:
     ```bash
     python -m venv venv
     source venv/bin/activate
     ```
 
 You can install the  nqrduck core via PyPi or from the cloned repository.
-3. Install the package with `pip install .[all]` to install all available NQRduck modules inside the cloned repository or just `pip install nqrduck[all]` to install the core package from PyPi.
+3. Install the package with `pip install .[all]` to install all available NQRduck modules inside the cloned repository or just `pip install "nqrduck[all]"` to install the core package from PyPi.
 Careful here you might need additional dependencies specified in the respective module repositories.
-If  you only want to  install some base  modules use `pip install .[base]` inside the cloned repository or with `pip install nqrduck[base]` .
+If  you only want to  install some base  modules use `pip install .[base]` inside the cloned repository or with `pip install -U "nqrduck[base]"` .
 You can find the different modules [here](https://github.com/nqrduck).
 4. Run the program with `nqrduck`.
 
 ## Usage
 Individual features of the software can be installed as separate Python packages, like spectrometer control, pulse sequence programming or simulation of magnetic resonance experiments. The available functionality of the NQRduck program therefore depends on the installed packages.
 
 The UI is structured as follows:
 
-<img src="docs/img/ui_structure_v2.png" alt="drawing" width="800">
+<img src="https://raw.githubusercontent.com/nqrduck/nqrduck/7e35ecc52b6e9deb4c5739bbfcd712206edb731b/docs/img/ui_structure_v2.png" alt="drawing" width="800">
 
 The UI is separated into different areas. Section 'a', highlighted in red, represents the menu bar used for general settings of the program and spectrometer selection. Section 'b', outlined in green, allows switching among various modules within the main view of the core, with the active module displayed in bold. Section 'c', depicted in blue, is the active module's view. The currently active module in the figure is the [nqrduck-measurement](https://github.com/nqrduck/nqrduck-measurement) module used for single frequency mangetic resonance experiments. The overall application is part of the NQRduck core and opens when the NQRduck core is started. 
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

### Comparing `nqrduck-0.0.6/pyproject.toml` & `nqrduck-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "Simple Python script to interact with various python modules used for magnetic resonance spectroscopy."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck-0.0.6/PKG-INFO` & `nqrduck-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple Python script to interact with various python modules used for magnetic resonance spectroscopy.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
         
@@ -73,26 +73,26 @@
 2. Create a virtual environment and activate it:
     ```bash
     python -m venv venv
     source venv/bin/activate
     ```
 
 You can install the  nqrduck core via PyPi or from the cloned repository.
-3. Install the package with `pip install .[all]` to install all available NQRduck modules inside the cloned repository or just `pip install nqrduck[all]` to install the core package from PyPi.
+3. Install the package with `pip install .[all]` to install all available NQRduck modules inside the cloned repository or just `pip install "nqrduck[all]"` to install the core package from PyPi.
 Careful here you might need additional dependencies specified in the respective module repositories.
-If  you only want to  install some base  modules use `pip install .[base]` inside the cloned repository or with `pip install nqrduck[base]` .
+If  you only want to  install some base  modules use `pip install .[base]` inside the cloned repository or with `pip install -U "nqrduck[base]"` .
 You can find the different modules [here](https://github.com/nqrduck).
 4. Run the program with `nqrduck`.
 
 ## Usage
 Individual features of the software can be installed as separate Python packages, like spectrometer control, pulse sequence programming or simulation of magnetic resonance experiments. The available functionality of the NQRduck program therefore depends on the installed packages.
 
 The UI is structured as follows:
 
-<img src="docs/img/ui_structure_v2.png" alt="drawing" width="800">
+<img src="https://raw.githubusercontent.com/nqrduck/nqrduck/7e35ecc52b6e9deb4c5739bbfcd712206edb731b/docs/img/ui_structure_v2.png" alt="drawing" width="800">
 
 The UI is separated into different areas. Section 'a', highlighted in red, represents the menu bar used for general settings of the program and spectrometer selection. Section 'b', outlined in green, allows switching among various modules within the main view of the core, with the active module displayed in bold. Section 'c', depicted in blue, is the active module's view. The currently active module in the figure is the [nqrduck-measurement](https://github.com/nqrduck/nqrduck-measurement) module used for single frequency mangetic resonance experiments. The overall application is part of the NQRduck core and opens when the NQRduck core is started. 
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

