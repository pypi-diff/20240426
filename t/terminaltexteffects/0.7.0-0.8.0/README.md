# Comparing `tmp/terminaltexteffects-0.7.0.tar.gz` & `tmp/terminaltexteffects-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminaltexteffects-0.7.0.tar", max compression
+gzip compressed data, was "terminaltexteffects-0.8.0.tar", max compression
```

## Comparing `terminaltexteffects-0.7.0.tar` & `terminaltexteffects-0.8.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
--rwxr-xr-x   0        0        0     1072 2023-08-13 20:34:07.346818 terminaltexteffects-0.7.0/LICENSE
--rwxr-xr-x   0        0        0    94924 2024-03-28 10:59:20.342838 terminaltexteffects-0.7.0/README.md
--rwxr-xr-x   0        0        0      474 2024-03-28 11:03:13.019576 terminaltexteffects-0.7.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-08-12 13:15:55.921216 terminaltexteffects-0.7.0/terminaltexteffects/__init__.py
--rwxr-xr-x   0        0        0     1976 2024-03-20 12:45:46.590851 terminaltexteffects-0.7.0/terminaltexteffects/__main__.py
--rwxr-xr-x   0        0        0    10163 2024-03-19 15:49:53.265141 terminaltexteffects-0.7.0/terminaltexteffects/base_character.py
--rwxr-xr-x   0        0        0        0 2023-07-22 17:59:37.688921 terminaltexteffects-0.7.0/terminaltexteffects/effects/__init__.py
--rwxr-xr-x   0        0        0    13662 2024-03-27 11:38:51.531691 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_beams.py
--rwxr-xr-x   0        0        0    13147 2024-03-27 11:39:03.337550 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_binarypath.py
--rwxr-xr-x   0        0        0    16894 2024-03-27 11:39:17.646979 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_blackhole.py
--rwxr-xr-x   0        0        0     8514 2024-03-27 11:42:50.868052 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_bouncyballs.py
--rwxr-xr-x   0        0        0    14132 2024-03-27 11:39:27.220183 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_bubbles.py
--rwxr-xr-x   0        0        0     6548 2024-03-26 11:00:53.929709 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_burn.py
--rwxr-xr-x   0        0        0     9983 2024-03-27 11:39:38.109423 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_crumble.py
--rwxr-xr-x   0        0        0     9212 2024-03-26 11:12:14.441485 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_decrypt.py
--rwxr-xr-x   0        0        0    11367 2024-03-27 11:39:51.231233 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_errorcorrect.py
--rwxr-xr-x   0        0        0     6176 2024-03-26 11:18:57.890154 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_expand.py
--rwxr-xr-x   0        0        0    11322 2024-03-23 13:19:32.215144 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_fireworks.py
--rwxr-xr-x   0        0        0     8041 2024-03-27 11:40:04.336152 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_middleout.py
--rwxr-xr-x   0        0        0    13484 2024-03-27 11:40:13.541292 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_orbittingvolley.py
--rwxr-xr-x   0        0        0     8431 2024-03-27 11:40:21.142173 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_overflow.py
--rwxr-xr-x   0        0        0     9698 2024-03-26 11:36:27.552827 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_pour.py
--rwxr-xr-x   0        0        0     9861 2024-03-27 11:40:35.994424 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_print.py
--rwxr-xr-x   0        0        0     8009 2024-03-28 02:11:25.950328 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_rain.py
--rwxr-xr-x   0        0        0     5814 2024-03-26 12:08:32.039691 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_random_sequence.py
--rwxr-xr-x   0        0        0    16717 2024-03-27 11:40:52.073795 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_rings.py
--rwxr-xr-x   0        0        0     6287 2024-03-26 12:14:11.740155 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_scattered.py
--rwxr-xr-x   0        0        0    11332 2024-03-26 12:17:29.687271 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_slide.py
--rwxr-xr-x   0        0        0    11119 2024-03-27 11:41:07.453461 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_spotlights.py
--rwxr-xr-x   0        0        0     8915 2024-03-26 12:21:42.151249 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_spray.py
--rwxr-xr-x   0        0        0    12650 2024-03-27 11:41:20.285164 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_swarm.py
--rwxr-xr-x   0        0        0    17444 2024-03-27 11:41:34.378639 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_synthgrid.py
--rwxr-xr-x   0        0        0    10988 2024-03-24 17:54:49.908477 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_unstable.py
--rwxr-xr-x   0        0        0     6978 2024-03-27 02:39:28.464341 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_verticalslice.py
--rwxr-xr-x   0        0        0    21364 2024-03-27 02:41:59.311987 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_vhstape.py
--rwxr-xr-x   0        0        0     7862 2024-03-27 11:41:54.263979 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_waves.py
--rwxr-xr-x   0        0        0     6950 2024-03-27 11:42:00.293899 terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_wipe.py
--rwxr-xr-x   0        0        0     4763 2024-03-19 15:49:53.316273 terminaltexteffects-0.7.0/terminaltexteffects/template/effect_template.py
--rwxr-xr-x   0        0        0        0 2023-07-22 17:59:26.632934 terminaltexteffects-0.7.0/terminaltexteffects/utils/__init__.py
--rwxr-xr-x   0        0        0    20910 2024-03-19 15:49:53.316772 terminaltexteffects-0.7.0/terminaltexteffects/utils/animation.py
--rwxr-xr-x   0        0        0     2294 2024-03-01 12:06:27.830757 terminaltexteffects-0.7.0/terminaltexteffects/utils/ansitools.py
--rwxr-xr-x   0        0        0    13087 2024-03-19 15:49:53.398047 terminaltexteffects-0.7.0/terminaltexteffects/utils/arg_validators.py
--rwxr-xr-x   0        0        0    11704 2024-03-19 15:49:53.401639 terminaltexteffects-0.7.0/terminaltexteffects/utils/argsdataclass.py
--rwxr-xr-x   0        0        0     2225 2024-03-19 15:49:53.401996 terminaltexteffects-0.7.0/terminaltexteffects/utils/colorterm.py
--rwxr-xr-x   0        0        0    12421 2024-03-19 15:49:53.423980 terminaltexteffects-0.7.0/terminaltexteffects/utils/easing.py
--rwxr-xr-x   0        0        0     9515 2024-03-28 11:00:09.260352 terminaltexteffects-0.7.0/terminaltexteffects/utils/geometry.py
--rwxr-xr-x   0        0        0     9306 2024-03-19 15:49:53.428007 terminaltexteffects-0.7.0/terminaltexteffects/utils/graphics.py
--rwxr-xr-x   0        0        0     6861 2024-03-19 15:49:53.451057 terminaltexteffects-0.7.0/terminaltexteffects/utils/hexterm.py
--rwxr-xr-x   0        0        0    17326 2024-03-19 15:49:53.462026 terminaltexteffects-0.7.0/terminaltexteffects/utils/motion.py
--rwxr-xr-x   0        0        0    22023 2024-03-19 15:49:53.462818 terminaltexteffects-0.7.0/terminaltexteffects/utils/terminal.py
--rw-r--r--   0        0        0    95403 1970-01-01 00:00:00.000000 terminaltexteffects-0.7.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-08-13 20:34:07.346818 terminaltexteffects-0.8.0/LICENSE
+-rwxr-xr-x   0        0        0    90261 2024-04-26 11:02:43.515814 terminaltexteffects-0.8.0/README.md
+-rwxr-xr-x   0        0        0      474 2024-04-26 11:07:09.808701 terminaltexteffects-0.8.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-08-12 13:15:55.921216 terminaltexteffects-0.8.0/terminaltexteffects/__init__.py
+-rwxr-xr-x   0        0        0     1998 2024-04-26 11:00:38.365918 terminaltexteffects-0.8.0/terminaltexteffects/__main__.py
+-rwxr-xr-x   0        0        0    10163 2024-04-14 17:40:09.477328 terminaltexteffects-0.8.0/terminaltexteffects/base_character.py
+-rwxr-xr-x   0        0        0     2332 2024-04-26 11:00:38.366147 terminaltexteffects-0.8.0/terminaltexteffects/base_effect.py
+-rwxr-xr-x   0        0        0        0 2023-07-22 17:59:37.688921 terminaltexteffects-0.8.0/terminaltexteffects/effects/__init__.py
+-rwxr-xr-x   0        0        0    17319 2024-04-26 11:00:38.366596 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_beams.py
+-rwxr-xr-x   0        0        0    15730 2024-04-26 11:00:38.366968 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_binarypath.py
+-rwxr-xr-x   0        0        0    18729 2024-04-26 11:00:38.367369 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_blackhole.py
+-rwxr-xr-x   0        0        0    10997 2024-04-26 11:00:38.367709 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_bouncyballs.py
+-rwxr-xr-x   0        0        0    17694 2024-04-26 11:00:38.368114 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_bubbles.py
+-rwxr-xr-x   0        0        0     7957 2024-04-26 11:00:38.368431 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_burn.py
+-rwxr-xr-x   0        0        0    11118 2024-04-26 11:00:38.368776 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_crumble.py
+-rwxr-xr-x   0        0        0    11360 2024-04-26 11:00:38.369124 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_decrypt.py
+-rwxr-xr-x   0        0        0    13783 2024-04-26 11:00:38.369493 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_errorcorrect.py
+-rwxr-xr-x   0        0        0     8058 2024-04-26 11:00:38.369870 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_expand.py
+-rwxr-xr-x   0        0        0    13898 2024-04-26 11:00:38.370244 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_fireworks.py
+-rwxr-xr-x   0        0        0    10189 2024-04-26 11:00:38.370591 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_middleout.py
+-rwxr-xr-x   0        0        0    16681 2024-04-26 11:00:38.371134 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_orbittingvolley.py
+-rwxr-xr-x   0        0        0    10624 2024-04-26 11:00:38.371723 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_overflow.py
+-rwxr-xr-x   0        0        0    11864 2024-04-26 11:00:38.372078 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_pour.py
+-rwxr-xr-x   0        0        0    11543 2024-04-26 11:00:38.372424 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_print.py
+-rwxr-xr-x   0        0        0     9773 2024-04-26 11:00:38.372770 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_rain.py
+-rwxr-xr-x   0        0        0     7365 2024-04-26 11:00:38.373084 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_random_sequence.py
+-rwxr-xr-x   0        0        0    19662 2024-04-26 11:00:38.373495 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_rings.py
+-rwxr-xr-x   0        0        0     8232 2024-04-26 11:00:38.373825 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_scattered.py
+-rwxr-xr-x   0        0        0    13156 2024-04-26 11:00:38.374184 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_slide.py
+-rwxr-xr-x   0        0        0    13617 2024-04-26 11:00:38.374560 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_spotlights.py
+-rwxr-xr-x   0        0        0    10790 2024-04-26 11:00:38.374892 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_spray.py
+-rwxr-xr-x   0        0        0    14721 2024-04-26 11:00:38.375249 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_swarm.py
+-rwxr-xr-x   0        0        0    19976 2024-04-26 11:00:38.375649 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_synthgrid.py
+-rwxr-xr-x   0        0        0    13830 2024-04-26 11:00:38.376011 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_unstable.py
+-rwxr-xr-x   0        0        0     8500 2024-04-26 11:00:38.376337 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_verticalslice.py
+-rwxr-xr-x   0        0        0    23371 2024-04-26 11:00:38.376751 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_vhstape.py
+-rwxr-xr-x   0        0        0    10187 2024-04-26 11:00:38.377087 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_waves.py
+-rwxr-xr-x   0        0        0     8564 2024-04-26 11:00:38.377413 terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_wipe.py
+-rwxr-xr-x   0        0        0        0 2024-04-12 11:52:35.092907 terminaltexteffects-0.8.0/terminaltexteffects/py.typed
+-rwxr-xr-x   0        0        0     4762 2024-04-26 11:00:38.377749 terminaltexteffects-0.8.0/terminaltexteffects/template/effect_template.py
+-rwxr-xr-x   0        0        0        0 2023-07-22 17:59:26.632934 terminaltexteffects-0.8.0/terminaltexteffects/utils/__init__.py
+-rwxr-xr-x   0        0        0    20910 2024-03-19 15:49:53.316772 terminaltexteffects-0.8.0/terminaltexteffects/utils/animation.py
+-rwxr-xr-x   0        0        0     2294 2024-03-01 12:06:27.830757 terminaltexteffects-0.8.0/terminaltexteffects/utils/ansitools.py
+-rwxr-xr-x   0        0        0    14137 2024-04-26 11:00:38.378147 terminaltexteffects-0.8.0/terminaltexteffects/utils/arg_validators.py
+-rwxr-xr-x   0        0        0    11651 2024-04-26 11:00:38.378501 terminaltexteffects-0.8.0/terminaltexteffects/utils/argsdataclass.py
+-rwxr-xr-x   0        0        0     2225 2024-03-19 15:49:53.401996 terminaltexteffects-0.8.0/terminaltexteffects/utils/colorterm.py
+-rwxr-xr-x   0        0        0    12421 2024-03-19 15:49:53.423980 terminaltexteffects-0.8.0/terminaltexteffects/utils/easing.py
+-rwxr-xr-x   0        0        0        0 2024-04-26 11:00:38.378584 terminaltexteffects-0.8.0/terminaltexteffects/utils/exceptions.py
+-rwxr-xr-x   0        0        0     9515 2024-03-28 11:00:09.260352 terminaltexteffects-0.8.0/terminaltexteffects/utils/geometry.py
+-rwxr-xr-x   0        0        0     9115 2024-04-08 16:59:01.111903 terminaltexteffects-0.8.0/terminaltexteffects/utils/graphics.py
+-rwxr-xr-x   0        0        0     6861 2024-03-19 15:49:53.451057 terminaltexteffects-0.8.0/terminaltexteffects/utils/hexterm.py
+-rwxr-xr-x   0        0        0    17326 2024-03-19 15:49:53.462026 terminaltexteffects-0.8.0/terminaltexteffects/utils/motion.py
+-rwxr-xr-x   0        0        0    25355 2024-04-26 11:00:38.379138 terminaltexteffects-0.8.0/terminaltexteffects/utils/terminal.py
+-rw-r--r--   0        0        0    90791 1970-01-01 00:00:00.000000 terminaltexteffects-0.8.0/PKG-INFO
```

### Comparing `terminaltexteffects-0.7.0/LICENSE` & `terminaltexteffects-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.7.0/README.md` & `terminaltexteffects-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,81 +9,141 @@
   <p align="center">
     Inline Visual Effects in the Terminal
     <br/>
     <br/>
   </p>
 </p>
 
-[![PyPI - Version](https://img.shields.io/pypi/v/terminaltexteffects?style=flat&color=green)](http://pypi.org/project/terminaltexteffects/ "![PyPI - Version](https://img.shields.io/pypi/v/terminaltexteffects?style=flat&color=green)")  ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/terminaltexteffects) ![License](https://img.shields.io/github/license/ChrisBuilds/terminaltexteffects) 
+[![PyPI - Version](https://img.shields.io/pypi/v/terminaltexteffects?style=flat&color=green)](http://pypi.org/project/terminaltexteffects/ "![PyPI - Version](https://img.shields.io/pypi/v/terminaltexteffects?style=flat&color=green)")  ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/terminaltexteffects) ![License](https://img.shields.io/github/license/ChrisBuilds/terminaltexteffects)
 
 ## Table Of Contents
 
 * [About](#tte)
 * [Requirements](#requirements)
 * [Installation](#installation)
-* [Usage](#usage)
+* [Usage (Application)](#application)
+* [Usage (Library)](#library)
 * [Options](#options)
 * [Examples](#examples)
 * [In-Development Preview](#in-development-preview)
 * [Latest Release Notes](#latest-release-notes)
 * [License](#license)
 
-
 ## TTE
-![synthgrid_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/6d1bab16-0520-44fa-a508-8f92d7d3be9e)
 
+![synthgrid_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/6d1bab16-0520-44fa-a508-8f92d7d3be9e)
 
 TerminalTextEffects is a collection of visual effects that run inline in the terminal. The underlying visual effect engine supports the following:
+
 * Xterm 256 / RGB hex color support
 * Complex character movement via Paths, Waypoints, and
   motion easing.
 * Complex animations via Scenes with symbol/color changes,
   layers, easing, and Path synced progression.
-* Event handling for Path/Scene state changes with 
+* Event handling for Path/Scene state changes with
   custom callback support and many pre-defined actions.
-* Variable stop/step color gradient generation. 
+* Variable stop/step color gradient generation.
 * Extensive effect customization via per-effect arguments.
 * Runs inline, preserving terminal state and workflow.
 
 ## Requirements
 
 TerminalTextEffects is written in Python and does not require any 3rd party modules. Terminal interactions use standard ANSI terminal sequences and should work in most modern terminals.
 
 Note: Windows Terminal performance is slow for some effects.
 
 ## Installation
 
-
 ```pip install terminaltexteffects```
 OR
 ```pipx install terminaltexteffects```
 
 ## Usage
+
+### Application
+
 ```cat your_text | tte <effect> [options]```
 
 OR
 
-``` cat your_text | python -m terminaltexteffects <effect> [options]```
+```cat your_text | python -m terminaltexteffects <effect> [options]```
 
 * Use ```<effect> -h``` to view options for a specific effect, such as color or movement direction.
   * Ex: ```tte decrypt -h```
 
-## Options
+### Library
+
+All effects are iterators which return a string representing the current frame. Basic usage is as simple as importing the effect, instantiating it with the input text, and iterating over the effect.
+
+```python
+from terminaltexteffects.effects import effect_rain
+
+effect = effect_rain.Rain("your text here")
+
+for frame in effect:
+    # do something with the string
+    ...
+```
+
+In the event you want to allow TTE to handle the terminal setup/teardown, cursor positioning, and animation frame rate, a terminal_output() context manager is available.
+
+```python
+from terminaltexteffects.effects import effect_rain
+
+effect = effect_rain.Rain("your text here")
+with effect.terminal_output() as terminal:
+    for frame in effect:
+        terminal.print(frame)
+```
+
+All command line arguments are available within each effect via the `effect.effect_config` and `effect.terminal_config` attributes.
+
+```python
+from terminaltexteffects.effects import effect_rain
+
+effect = effect_rain.Rain("your text here")
+
+effect.effect_config.rain_colors = ("ff0000","00ff00","0000ff")
+effect.terminal_config.tab_width = 2
+effect.terminal_config.wrap_text = False
+
+for frame in effect:
+    # do something with the string
+    ...
+```
+
+For use cases where the terminal dimensions cannot be automatically discovered or you would like to manually define the dimensions, the ```effect.terminal_config``` can be configured as follows:
+
+```python
+effect.terminal_config.terminal_dimensions = (80, 24) # width, height
 ```
+
+If you would like to ignore terminal dimensions altogether and base the output dimensions solely on the input data:
+
+```python
+effect.terminal_config.ignore_terminal_dimensions = True
+```
+
+## Options
+
+```markdown
 options:
-  -h, --help            show this help message and exit
+-h, --help            show this help message and exit
   --tab-width (int > 0)
-                        Number of spaces to use for a tab character.
-  --xterm-colors        Convert any colors specified in RBG hex to the closest XTerm-256 color.
-  --no-color            Disable all colors in the effect.
-  --no-wrap             Disable wrapping of text.
-  -a ANIMATION_RATE, --animation-rate ANIMATION_RATE
-                        Minimum time, in seconds, between animation steps. This value does not normally need to be modified. Use this to increase the playback speed of all aspects of the effect. This will have
-                        no impact beyond a certain lower threshold due to the processing speed of your device.
-
+                        Number of spaces to use for a tab character. (default: 4)
+  --xterm-colors        Convert any colors specified in RBG hex to the closest XTerm-256 color. (default: False)
+  --no-color            Disable all colors in the effect. (default: False)
+  --wrap-text           Wrap text wider than the output area width. (default: False)
+  --frame-rate FRAME_RATE
+                        Target frame rate for the animation. (default: 100)
+  --terminal-dimensions TERMINAL_DIMENSIONS TERMINAL_DIMENSIONS
+                        Use the terminal dimensions to limit the size of the output area and support wrapping. If False, the output area is determined by the input data dimensions and may overflow the terminal
+                        width. (default: (0, 0))
+  --ignore-terminal-dimensions
+                        Ignore the terminal dimensions and use the input data dimensions for the output area. (default: False)
 Effect:
   Name of the effect to apply. Use <effect> -h for effect specific help.
 
   {beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,dev,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,test,unstable,verticalslice,vhstape,waves,wipe}
                         Available Effects
     beams               Create beams which travel over the output area illuminating the characters behind them.
     binarypath          Binary representations of each character move through the terminal towards the home coordinate of the character.
@@ -114,19 +174,22 @@
     verticalslice       Slices the input in half vertically and slides it into place from opposite directions.
     vhstape             Lines of characters glitch left and right and lose detail like an old VHS tape.
     waves               Waves travel across the terminal leaving behind the characters.
     wipe                Wipes the text across the terminal to reveal characters.
 
 Ex: ls -a | tte crumble --final-gradient-stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction diagonal
 ```
-## Examples
-Note: All effects support extensive customization via effect specific arguments. The examples shown below only represent one possible variant of 
+
+### Examples
+
+Note: All effects support extensive customization via effect specific arguments. The examples shown below only represent one possible variant of
 each effect. Check the effect help output to see arguments.
 
 #### Beams
+
 ![beams_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/6bb98dac-688e-43c9-96aa-1a45f451d4cb)
 <details>
 <summary>tte beams -h</summary>
 <br>
     beams | Create beams which travel over the output area illuminating the characters behind them.
 
     options:
@@ -160,14 +223,15 @@
       --final-wipe-speed (int > 0)
                             Speed of the final wipe as measured in diagonal groups activated per frame. (default: 1)
 
     Example: terminaltexteffects beams --beam-row-symbols ▂ ▁ _ --beam-column-symbols ▌ ▍ ▎ ▏ --beam-delay 10 --beam-row-speed-range 10-40 --beam-column-speed-range 6-10 --beam-gradient-stops ffffff 00D1FF 8A008A --beam-gradient-steps 2 8 --beam-gradient-frames 2 --final-gradient-stops 8A008A 00D1FF ffffff --final-gradient-steps 12 --final-gradient-frames 5 --final-gradient-direction vertical --final-wipe-speed 1
 </details>
 
 #### Binarypath
+
 ![binarypath_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/99ad3946-c475-4743-93e2-cdfb2a7f558f)
 <details>
 <summary>tte binarypath -h</summary>
 <br>
     binarypath | Binary representations of each character move through the terminal towards the home coordinate of the character.
 
     options:
@@ -186,14 +250,15 @@
       --active-binary-groups (0 <= float(n) <= 1)
                             Maximum number of binary groups that are active at any given time. Lower this to improve performance. (default: 0.05)
 
     Example: terminaltexteffects binarypath --final-gradient-stops 00d500 007500 --final-gradient-steps 12 --final-gradient-direction vertical --binary-colors 044E29 157e38 45bf55 95ed87 --movement-speed 1.0 --active-binary-groups 0.05
 </details>
 
 #### Blackhole
+
 ![blackhole_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/877579d3-d353-4bed-9a95-d3ea7a53200a)
 <details>
 <summary>tte blackhole -h</summary>
 <br>
     blackhole | Characters are consumed by a black hole and explode outwards.
 
     options:
@@ -211,14 +276,15 @@
       --final-gradient-direction (diagonal, horizontal, vertical, center)
                             Direction of the gradient for the final color. (default: Direction.DIAGONAL)
 
     Example: terminaltexteffects blackhole --star-colors ffcc0d ff7326 ff194d bf2669 702a8c 049dbf --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-direction vertical
 </details>
 
 #### Bouncyballs
+
 ![bouncyballs_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/84b12fd0-6e51-4661-bd09-407dad30023d)
 <details>
 <summary>tte bouncyballs -h</summary>
 <br>
     bouncyballs | Characters are bouncy balls falling from the top of the output area.
 
     options:
@@ -264,14 +330,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects bouncyballs --ball-colors d1f4a5 96e2a4 5acda9 --ball-symbols o "*" O 0 . --final-gradient-stops f8ffae 43c6ac --final-gradient-steps 12 --final-gradient-direction diagonal --ball-delay 7 --movement-speed 0.25 --easing OUT_BOUNCE
 </details>
 
 #### Bubbles
+
 ![bubbles_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/5a616538-7936-4f55-b2ff-28e6c4179fce)
 <details>
 <summary>tte bubbles -h</summary>
 <br>
     bubbles | Characters are formed into bubbles that float down and pop.
 
     options:
@@ -322,14 +389,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects bubbles --bubble-colors d33aff 7395c4 43c2a7 02ff7f --pop-color ffffff --final-gradient-stops d33aff 02ff7f --final-gradient-steps 12 --final-gradient-direction diagonal --bubble-speed 0.1 --bubble-delay 50 --pop-condition row --easing IN_OUT_SINE
 </details>
 
 #### Burn
+
 ![burn_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/9770711a-ea68-48cc-947f-fb13c6613a2e)
 <details>
 <summary>tte burn -h</summary>
 <br>
     burn | Burn the output area.
 
     options:
@@ -346,14 +414,15 @@
       --final-gradient-direction (diagonal, horizontal, vertical, center)
                             Direction of the gradient for the final color. (default: Direction.VERTICAL)
 
     Example: terminaltexteffects burn --starting-color 837373 --burn-colors ffffff fff75d fe650d 8a003c 510100 --final-gradient-stops 00c3ff ffff1c --final-gradient-steps 12
 </details>
 
 #### Crumble
+
 ![crumble_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/f9cdea9b-b695-41b7-b129-8288232cba13)
 <details>
 <summary>tte crumble -h</summary>
 <br>
     crumble | Characters lose color and crumble into dust, vacuumed up, and reformed.
 
     options:
@@ -366,14 +435,15 @@
       --final-gradient-direction (diagonal, horizontal, vertical, center)
                             Direction of the gradient for the final color. (default: Direction.DIAGONAL)
 
     Example: terminaltexteffects crumble --final-gradient-stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction diagonal
 </details>
 
 #### Decrypt
+
 ![decrypt_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/36c23e70-065d-4316-a09e-c2761882cbb3)
 <details>
 <summary>tte decrypt -h</summary>
 <br>
     decrypt | Movie style decryption effect.
 
     options:
@@ -390,14 +460,15 @@
       --final-gradient-direction (diagonal, horizontal, vertical, center)
                             Direction of the gradient for the final color. (default: Direction.VERTICAL)
 
     Example: terminaltexteffects decrypt --typing-speed 2 --ciphertext-colors 008000 00cb00 00ff00 --final-gradient-stops eda000 --final-gradient-steps 12 --final-gradient-direction vertical
 </details>
 
 #### Errorcorrect
+
 ![errorcorrect_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/a851d333-8fe2-4c12-9c45-536ed8ebbab8)
 <details>
 <summary>tte errorcorrect -h</summary>
 <br>
     errorcorrect | Some characters start in the wrong position and are corrected in sequence.
 
     options:
@@ -446,14 +517,15 @@
         Visit: https://easings.net/ for visualizations of the easing functions.
 
         
     Example: terminaltexteffects errorcorrect --error-pairs 0.1 --swap-delay 10 --error-color e74c3c --correct-color 45bf55 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --movement-speed 0.5
 </details>
 
 #### Expand
+
 ![expand_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/21d1c374-9028-4546-a5d7-ee538488ee7b)
 <details>
 <summary>tte expand -h</summary>
 <br>
     expand | Expands the text from a single point.
 
     options:
@@ -497,14 +569,15 @@
         Visit: https://easings.net/ for visualizations of the easing functions.
 
         
     Example: terminaltexteffects expand --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-frames 5 --movement-speed 0.35 --expand-easing IN_OUT_QUART
 </details>
 
 #### Fireworks
+
 ![fireworks_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/da6a97b1-c4fd-4370-9852-9ddb8a494b55)
 <details>
 <summary>tte fireworks -h</summary>
 <br>
     fireworks | Characters explode like fireworks and fall into place.
 
     options:
@@ -528,14 +601,15 @@
       --explode-distance (0 <= float(n) <= 1)
                             Maximum distance from the firework shell origin to the explode waypoint as a percentage of the total output area width. (default: 0.1)
 
     Example: terminaltexteffects fireworks --firework-colors 88F7E2 44D492 F5EB67 FFA15C FA233E --firework-symbol o --firework-volume 0.02 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --launch-delay 60 --explode-distance 0.1 --explode-anywhere
 </details>
 
 #### Middleout
+
 ![middleout_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/d78e37f6-ccb1-4d3b-a07c-f021b6893fce)
 <details>
 <summary>tte middleout -h</summary>
 <br>
     middleout | Text expands in a single row or column in the middle of the output area then out.
 
     options:
@@ -586,14 +660,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects middleout --starting-color 8A008A --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --expand-direction vertical --center-movement-speed 0.35 --full-movement-speed 0.35 --center-easing IN_OUT_SINE --full-easing IN_OUT_SINE
 </details>
 
 #### Orbittingvolley
+
 ![orbittingvolley_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/084038e5-9d49-4c7d-bf15-e989f541b15c)
 <details>
 <summary>tte orbittingvolley -h</summary>
 <br>
     orbittingvolley | Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.
 
     options:
@@ -649,14 +724,15 @@
         Visit: https://easings.net/ for visualizations of the easing functions.
 
         
     Example: terminaltexteffects orbittingvolley --top-launcher-symbol █ --right-launcher-symbol █ --bottom-launcher-symbol █ --left-launcher-symbol █ --final-gradient-stops FFA15C 44D492 --final-gradient-steps 12 --launcher-movement-speed 0.5 --character-movement-speed 1 --volley-size 0.03 --launch-delay 50 --character-easing OUT_SINE
 </details>
 
 #### Overflow
+
 ![overflow_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/37da1088-ba15-4be9-9489-c387a6a55930)
 <details>
 <summary>tte overflow -h</summary>
 <br>
     overflow | Input text overflows ands scrolls the terminal in a random order until eventually appearing ordered.
 
     options:
@@ -675,14 +751,15 @@
       --overflow-speed (int > 0)
                             Speed of the overflow effect. (default: 3)
 
     Example: terminaltexteffects overflow --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --overflow-gradient-stops f2ebc0 8dbfb3 f2ebc0 --overflow-cycles-range 2-4 --overflow-speed 3
 </details>
 
 #### Pour
+
 ![pour_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/145c2a4e-6b30-48c6-80a3-afb03edf7c22)
 <details>
 <summary>tte pour -h</summary>
 <br>
     pour | Pours the characters into position from the given direction.
 
     options:
@@ -731,14 +808,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects pour --pour-direction down --movement-speed 0.2 --gap 1 --starting-color FFFFFF --final-gradient-stops 8A008A 00D1FF FFFFFF --easing IN_QUAD
 </details>
 
 #### Print
+
 ![print_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/5d902350-e5d3-400c-9496-119c88d40643)
 <details>
 <summary>tte print -h</summary>
 <br>
     print | Lines are printed one at a time following a print head. Print head performs line feed, carriage return.
 
     options:
@@ -782,14 +860,15 @@
         Visit: https://easings.net/ for visualizations of the easing functions.
 
         
     Example: terminaltexteffects print --final-gradient-stops 02b8bd c1f0e3 00ffa0 --final-gradient-steps 12 --print-head-return-speed 1.25 --print-speed 1 --print-head-easing IN_OUT_QUAD
 </details>
 
 #### Rain
+
 ![rain_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/7b8cf447-67b6-41e9-b354-07b3e5161d10)
 <details>
 <summary>tte rain -h</summary>
 <br>
     rain | Rain characters from the top of the output area.
 
     options:
@@ -834,14 +913,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
     
     Example: terminaltexteffects rain --rain-symbols o . , "*" "|" --rain-colors 00315C 004C8F 0075DB 3F91D9 78B9F2 9AC8F5 B8D8F8 E3EFFC --final-gradient-stops 488bff b2e7de 57eaf7 --final-gradient-steps 12 --movement-speed 0.1-0.2 --easing IN_QUART
 </details>
 
 #### RandomSequence
+
 ![randomsequence_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/a2218f80-73b6-40ab-b2fb-49268cf9f890)
 <details>
 <summary>tte randomsequence -h</summary>
 <br>
     randomsequence | Prints the input data in a random sequence.
 
     options:
@@ -859,14 +939,15 @@
                             Direction of the gradient for the final color. (default: Direction.VERTICAL)
       --speed (float > 0)   Speed of the animation as a percentage of the total number of characters. (default: 0.004)
 
     Example: terminaltexteffects randomsequence --starting-color 000000 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-frames 12 --speed 0.004
 </details>
 
 #### Rings
+
 ![rings_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/cb7f6388-0f46-42f1-a2b3-6a267e9451f0)
 <details>
 <summary>tte rings -h</summary>
 <br>
     rings | Characters are dispersed and form into spinning rings.
 
     options:
@@ -890,14 +971,15 @@
       --spin-disperse-cycles SPIN_DISPERSE_CYCLES
                             Number of times the animation will cycles between spinning rings and dispersed characters. (default: 3)
 
     Example: terminaltexteffects rings --ring-colors ab48ff e7b2b2 fffebd --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --ring-gap 0.1 --spin-duration 200 --spin-speed 0.25-1.0 --disperse-duration 200 --spin-disperse-cycles 3
 </details>
 
 #### Scattered
+
 ![scattered_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/9948519d-0158-4ddf-ae3a-7d4eddb706d9)
 <details>
 <summary>tte scattered -h</summary>
 <br>
     scattered | Move the characters into place from random starting locations.
 
     options:
@@ -940,14 +1022,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects scattered --final-gradient-stops ff9048 ab9dff bdffea --final-gradient-steps 12 --final-gradient-frames 12 --movement-speed 0.5 --movement-easing IN_OUT_BACK
 </details>
 
 #### Slide
+
 ![slide_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/218e7218-e9ef-44de-b43b-5e824623a957)
 <details>
 <summary>tte slide -h</summary>
 <br>
     slide | Slide characters into view from outside the terminal, grouped by row, column, or diagonal.
 
     options:
@@ -995,14 +1078,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects slide --movement-speed 0.5 --grouping row --final-gradient-stops 833ab4 fd1d1d fcb045 --final-gradient-steps 12 --final-gradient-frames 10 --final-gradient-direction vertical --gap 3 --reverse-direction --merge --movement-easing OUT_QUAD
 </details>
 
 #### Spotlights
+
 ![spotlights_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/4ab93725-0c8a-4bdf-af91-057338f4e007)
 <details>
 <summary>tte spotlights -h</summary>
 <br>
     spotlights | Spotlights search the text area, illuminating characters, before converging in the center and expanding.
 
     options:
@@ -1049,14 +1133,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects spotlights --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --beam-width-ratio 2.0 --beam-falloff 0.3 --search-duration 750 --search-speed-range 0.25-0.5 --spotlight-count 3
 </details>
 
 #### Spray
+
 ![spray_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/0be02197-11c3-44d0-9e7f-cd90caefa876)
 <details>
 <summary>tte spray -h</summary>
 <br>
     spray | Draws the characters spawning at varying rates from a single point.
 
     options:
@@ -1101,14 +1186,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
         
     Example: terminaltexteffects spray --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --spray-position e --spray-volume 0.005 --movement-speed 0.4-1.0 --movement-easing OUT_EXPO
 </details>
 
 #### Swarm
+
 ![swarm_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/305e8390-a0fb-4edb-a541-7b52cef77c09)
 <details>
 <summary>tte swarm -h</summary>
 <br>
     swarm | Characters are grouped into swarms and move around the terminal before settling into position.
 
     options:
@@ -1131,14 +1217,15 @@
       --swarm-area-count (hyphen separated int range e.g. '1-10')
                             Range of the number of areas where characters will swarm. (default: (2, 4))
 
     Example: terminaltexteffects swarm --base-color 31a0d4 --flash-color f2ea79 --final-gradient-stops 31b900 f0ff65 --final-gradient-steps 12 --swarm-size 0.1 --swarm-coordination 0.80 --swarm-area-count 2-4
 </details>
 
 #### Synthgrid
+
 ![synthgrid_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/6d1bab16-0520-44fa-a508-8f92d7d3be9e)
 <details>
 <summary>tte synthgrid -h</summary>
 <br>
     synthgrid | Create a grid which fills with characters dissolving into the final text.
 
     options:
@@ -1164,14 +1251,15 @@
       --max-active-blocks (float > 0)
                             Maximum percentage of blocks to have active at any given time. For example, if set to 0.1, 10 percent of the blocks will be active at any given time. (default: 0.1)
 
     Example: terminaltexteffects synthgrid --grid-gradient-stops CC00CC ffffff --grid-gradient-steps 12 --text-gradient-stops 8A008A 00D1FF FFFFFF --text-gradient-steps 12 --grid-row-symbol ─ --grid-column-symbol "│" --text-generation-symbols ░ ▒ ▓ --max-active-blocks 0.1
 </details>
 
 #### Unstable
+
 ![unstable_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/29adb5bf-cd35-4d67-9ed4-fa73ebcb892d)
 <details>
 <summary>tte unstable -h</summary>
 <br>
     synthgrid | Create a grid which fills with characters dissolving into the final text.
 
     options:
@@ -1197,14 +1285,15 @@
       --max-active-blocks (float > 0)
                             Maximum percentage of blocks to have active at any given time. For example, if set to 0.1, 10 percent of the blocks will be active at any given time. (default: 0.1)
 
     Example: terminaltexteffects synthgrid --grid-gradient-stops CC00CC ffffff --grid-gradient-steps 12 --text-gradient-stops 8A008A 00D1FF FFFFFF --text-gradient-steps 12 --grid-row-symbol ─ --grid-column-symbol "│" --text-generation-symbols ░ ▒ ▓ --max-active-blocks 0.1
 </details>
 
 #### Verticalslice
+
 ![verticalslice_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/2341a822-7fef-4ebf-9420-8272fff64082)
 <details>
 <summary>tte verticalslice -h</summary>
 <br>
     verticalslice | Slices the input in half vertically and slides it into place from opposite directions.
 
     options:
@@ -1246,14 +1335,15 @@
         Visit: https://easings.net/ for visualizations of the easing functions.
 
         
     Example: terminaltexteffects verticalslice --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --movement-speed 0.15 --movement-easing IN_OUT_EXPO
 </details>
 
 #### VHSTape
+
 ![vhstape_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/720abbf4-f97d-4ce9-96ee-15ef973488d2)
 <details>
 <summary>tte vhstape -h</summary>
 <br>
     vhstape | Lines of characters glitch left and right and lose detail like an old VHS tape.
 
     options:
@@ -1280,14 +1370,15 @@
       --total-glitch-time (int > 0)
                             Total time, animation steps, that the glitching phase will last. (default: 1000)
 
     Example: terminaltexteffects vhstape --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --glitch-line-colors ffffff ff0000 00ff00 0000ff ffffff --glitch-wave-colors ffffff ff0000 00ff00 0000ff ffffff --noise-colors 1e1e1f 3c3b3d 6d6c70 a2a1a6 cbc9cf ffffff --glitch-line-chance 0.05 --noise-chance 0.004 --total-glitch-time 1000
 </details>
 
 #### Waves
+
 ![waves_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/ea9b04ca-e526-4c7e-b98d-a98a42f7137f)
 <details>
 <summary>tte waves -h</summary>
 <br>
     waves | Waves travel across the terminal leaving behind the characters.
 
     options:
@@ -1338,14 +1429,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects waves --wave-symbols ▁ ▂ ▃ ▄ ▅ ▆ ▇ █ ▇ ▆ ▅ ▄ ▃ ▂ ▁ --wave-gradient-stops f0ff65 ffb102 31a0d4 ffb102 f0ff65 --wave-gradient-steps 6 --final-gradient-stops ffb102 31a0d4 f0ff65 --final-gradient-steps 12 --wave-count 7 --wave-length 2 --wave-easing IN_OUT_SINE
 </details>
 
 #### Wipe
+
 ![wipe_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/40b8c81e-6143-4839-af56-12e361651a0a)
 <details>
 <summary>tte wipe -h</summary>
 <br>
     wipe | Wipes the text across the terminal to reveal characters.
 
     options:
@@ -1363,97 +1455,62 @@
       --wipe-delay (int >= 0)
                             Number of animation cycles to wait before adding the next character group. Increase, to slow down the effect. (default: 0)
 
     Example: terminaltexteffects wipe --wipe-direction diagonal_bottom_left_to_top_right --final-gradient-stops 833ab4 fd1d1d fcb045 --final-gradient-steps 12 --final-gradient-frames 5 --wipe-delay 0
 </details>
 
 ## In-Development Preview
-Any effects shown below are in development and will be available in the next release.
 
+Any effects shown below are in development and will be available in the next release.
 
 ## Latest Release Notes
 
-## 0.7.0
+## 0.8.0
+
+---
+
+### New Features (0.8.0)
+
+---
+
+#### New Engine Features (0.8.0)
+
+* Library support: TTE effects are now importable. All effects are iterators that return strings for each frame of the output. See README for more information.
+* Terminal: New terminal argument (--terminal-dimensions) allows specification of the terminal dimensions without relying on auto-detection. Especially useful in cases where TTE is being used as a library in non-terminal or TUI contexts.
+* Terminal: New terminal argument (--ignore-terminal-dimensions) causes the output area dimensions to match the input data dimensions without regard to the terminal.
+
+### Changes (0.8.0)
+
+---
+
+#### Effects Changes (0.8.0)
+
+* Scattered. Holds scrambled text at the start for a few frames.
+* Scattered. Lowered default movement-speed from 0.5 to 0.3.
+
+#### Engine Changes (0.8.0)
+
+* graphics.Gradient ```__iter___()``` refactored to return a generator. No longer improperly implements the iterator protocol by resetting index in ```___iter__()```.
+* Terminal: Argument --animation-rate is now --frame-rate and is specified as a target frames per second.
+* Terminal: Argument --no-wrap is now --wrap-text and defaults to False.
+* Terminal: If a terminal object is instantiated without a TerminalConfig passed, it will instantiate a new TerminalConfig.
+* Terminal: Terminal.get_formatted_output_string() will return a string representing the current frame.
+* Terminal: Terminal.print() will print the frame to the terminal and handle cursor position. The optional argument (enforce_frame_rate: bool = True) determines if the frame rate set at Terminal.config.frame_rate is enforced. If set to False, the print will occur without delay.
+* New argument validator for terminal dimensions (arg_validators.TerminalDeminsions).
+* New module base_effect.py:
+* base_effect.BaseEffect:
+  * This is an abstract class which forms the base iterable for all effects and provides the terminal_output() context manager.
+* base_effect.BaseEffectIterator:
+  * This is an abstract class which provides the functionality to enable iteration over effects.
+
+### Bug Fixes (0.8.0)
+
+---
+
+#### Engine Fixes (0.8.0)
 
-### New Features
-#### Effects
- * Beams. Light beams travel across the output area and illuminate the characters behind them.
- * Overflow. The input text is scrambled by row and repeated randomly, scrolling up the terminal, before eventually displaying in the correct order.
- * OrbitingVolley. Characters fire from launcher which orbit output area.
- * Spotlights. Spotlights search the text area, illuminating characters, before converging in the center and expanding.
-
-#### Engine
- * Gradients now support multiple step specification to control the distance between each stop pair. For example:
-   graphics.Gradient(RED, BLUE, YELLOW, steps=(2,5)) results in a spectrum of RED -> (1 step) -> BLUE -> (4 steps) -> YELLOW
- * graphics.Gradient.get_color_at_fraction(fraction: float) will return a color at the given fraction of the spectrum when provided a float between 0 and 1, inclusive. This can be used to match the color to a ratio/ For example, the character height in the terminal.
- * graphics.Gradient.build_coordinate_color_mapping() will map gradient colors to coordinates in the terminal and supports a Gradient.Direction argument to enable gradients in the following directions: horizontal, vertical, diagonal, center
- * graphics.Gradient, if printed, will show a colored spectrum and the description of its stops and steps.
- * The Scene class has a new method: apply_gradient_to_symbols(). This method will iterate over a list of symbols and apply the colors from a gradient to the symbols. A frame with the symbol will be added for each color starting from the last color used in the previous symbol, up to the the index determined by the ratio of the current symbol's index in the symbols list to the total length of the list. This method allows scenes to automatically create frames from a list of symbols and gradient of arbitrary length while ensuring every symbol and color is displayed.
- * On instatiation, Terminal creates EffectCharacters for every coordinate in the output area that does not have an input character. These EffectCharacters have the symbol " " and are stored in Terminal._fill_characters as well as added to Terminal.character_by_input_coord.
- * arg_validators.IntRange will validate a range specified as "int-int" and return a tuple[int,int].
- * arg_validators.FloatRange will validate a range of floats specified as "float-float" and return a tuple[float, float].
- * character.animation.set_appearance(symbol, color) will set the character symbol and color directly. If a Scene is active, the appearance will be overwritten with the Scene frame on the next call to step_animation(). This method is intended for the occasion where a full scene isn't needed, or the appearance needs to be set based on conditions not compatible with Scenes or the EventHandler. For example, setting the color based on the terminal row. 
- * Terminal.CharacterSort enums moved to Terminal.CharacterGroup, Terminal.CharacterSort is now used for sorting and return a flat list of characters.
- * Terminal.CharacterSort has new sort methods, TOP_TO_BOTTOM_LEFT_TO_RIGHT, TOP_TO_BOTTOM_RIGHT_TO_LEFT, BOTTOM_TO_TOP_LEFT_TO_RIGHT, BOTTOM_TO_TOP_RIGHT_TO_LEFT, OUTSIDE_ROW_TO_MIDDLE, MIDDLE_ROW_TO_OUTSIDE
- * New Terminal.CharacterGroup options, CENTER_TO_OUTSIDE_DIAMONDS and OUTSIDE_TO_CENTER_DIAMONS
- * graphics.Animation.adjust_color_brightness(color: graphics.Color, brightness: float) will convert the color to HSL, adjust the brightness to the given level, and return 
-   an RGB hex string.
- * CTRL-C keyboard interrupt during a running effect will exit gracefully.
- * geometry.find_coords_in_circle() has been rewritten to find all coords which fall in an ellipse. The result is a circle due to the height/width ratio of terminal cells. This function now finds all terminal coordinates within the 'circle' rather than an arbitrary subset.
- * All command line arguments are typed allowing for more easily defined and tested effect args. 
-
-### Changes
-#### Effects
- * All effects have been updated to use the latest API calls for improved performance.
- * All effects support gradients for the final appearance.
- * All effects support gradient direction.
- * All effects have had their default colors refreshed.
- * ErrorCorrect swap-delay lowered and error-pairs specification changed to percent float.
- * Rain effect supports character specification for rain drops and movement speed range for the rain drop falling speed.
- * Print effect uses the row final gradient color for the print head color.
- * RandomSequence effect accepts a starting color and a speed.
- * Rings effect prepares faster. Ring colors are set in order of appearance in the ring-colors argument. Ring spin speed is configurable. Rings with less than 25% visible characters based on radius are no longer generated. Ring gap is set as a percent of the smallest output area dimension.
- * Scattered effect gradient progresses from the first color to the row color.
- * Spray effect spray-volume is specified as a percent of the total number of characters and movement speed is a range.
- * Swarm effect swarm focus points algorithm changed to reduce long distances between points. 
- * Decrypt effect supports gradient specification for plaintext and multiple color specification for ciphertext.
- * Decrypt effect has a --typing-speed arg to increase the speed of the initial text typing effect.
- * Decrypt effect has had the decrypting speed increased.
- * Beams effect uses Animation.adjust_color_brightness() to lower the background character brightness and shows the lighter color when the beam passes by.
- * Crumble effect uses Animation.adjust_color_brightness() to set the weak and dust colors based on the final gradient.
- * Fireworks effect launch_delay argument has a +/- 0-50% randomness applied. 
- * Bubbles effect --no-rainbow changed to --rainbow and default set to False.
- * Bubbles effect --bubble-color changed to --bubble-colors. Bubble color is randomly chosen from the colors unless --rainbow is used.
- * Burn effect burns faster with some randomness in speed.
- * Burn effect final color fades in from the burned color.
- * Burn effect characters are shown prior to burning using a starting_color arg.
- * Pour effect has a --pour-speed argument.
-
-#### Engine
- * Geometry related methods have been removed from the motion class. They are now located at terminaltexteffects.utils.geometry as separate functions.
- * The Coord() object definition has been moved from the motion module to the geometry module.
- * Terminal.add_character() takes a geometry.Coord() argument to set the character's input_coordinate.
- * EffectCharacters have a unique ID set by the Terminal on instatiation. As a result, all EffectCharacters should be created using Terminal.add_character().
- * EffectCharacters added by the effect are stored in Terminal._added_characters.
- * Retrieving EffectCharacters from the terminal should no longer be done via accessing the lists of characters [_added_characters, _fill_characters, _input_characters], but should be retrieved via Terminal.get_characters() and Terminal.get_characters_sorted(). 
- * Setting EffectCharacter visibility is now done via Terminal.set_character_visibility(). This enables the terminal to keep track of all visible characters without needing to iterate over all characters on every call to _update_terminal_state().
- * EventHandler.Action.SET_CHARACTER_VISIBILITY_STATE has been removed as visibilty state is handled by the Terminal. To enable visibility state changes through the event system, use a CALLBACK action with target EventHandler.Callback(terminal.set_character_visibility, True/False).
- * geometry.find_coords_on_circle() num_points arg renamed to points_limit and new arg unique: bool, added to remove any duplicate Coords.
- * The animation rate argument (-a, --animation-rate) has been removed from all effects and is handled as a terminal argument specified prior to the effect name.
- * argtypes.py has been renamed arg_validators.py and all functions have been refactored into classes with a METAVAR class member and a type_parser method.
- * easing.EasingFunction type alias used anywhere an easing function is accepted.
- * Exceptions raised are no longer caught in a except clause. Only a finally clause is used to restore the cursor. Tracebacks are useful.
- 
- #### Other
- * More tests have been added.
-
-### Bug Fixes
-#### Effects
- * All effects with command line options that accept variable length arguments which require at least 1 argument will present an error message when the option is called with 0 arguments.
-
-#### Engine
- * Fixed division by zero error in geometry.find_coord_at_distance() when the origin coord and the target coord are the same.
- * Fixed gradient generating an extra color in the spectrum when the initial color pair was repeated. Ex: Gradient('ffffff','000000','ffffff','000000, steps=5) would result in the third color 'ffffff' being added to the spectrum when it was already present as the end of the generation from '000000'->'ffffff'. 
+* Fixed Argfield nargs type from str to str | int.
+* Implemented custom formatter into argsdataclass.py argument parsing.
 
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/main/LICENSE.md) for more information.
```

#### html2text {}

```diff
@@ -6,43 +6,70 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/
 terminaltexteffects?style=flat&color=green)](http://pypi.org/project/
 terminaltexteffects/ "![PyPI - Version](https://img.shields.io/pypi/v/
 terminaltexteffects?style=flat&color=green)") ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/terminaltexteffects) ![License](https://
 img.shields.io/github/license/ChrisBuilds/terminaltexteffects) ## Table Of
 Contents * [About](#tte) * [Requirements](#requirements) * [Installation]
-(#installation) * [Usage](#usage) * [Options](#options) * [Examples](#examples)
-* [In-Development Preview](#in-development-preview) * [Latest Release Notes]
-(#latest-release-notes) * [License](#license) ## TTE ![synthgrid_demo](https://
-github.com/ChrisBuilds/terminaltexteffects/assets/57874186/6d1bab16-0520-44fa-
-a508-8f92d7d3be9e) TerminalTextEffects is a collection of visual effects that
-run inline in the terminal. The underlying visual effect engine supports the
+(#installation) * [Usage (Application)](#application) * [Usage (Library)]
+(#library) * [Options](#options) * [Examples](#examples) * [In-Development
+Preview](#in-development-preview) * [Latest Release Notes](#latest-release-
+notes) * [License](#license) ## TTE ![synthgrid_demo](https://github.com/
+ChrisBuilds/terminaltexteffects/assets/57874186/6d1bab16-0520-44fa-a508-
+8f92d7d3be9e) TerminalTextEffects is a collection of visual effects that run
+inline in the terminal. The underlying visual effect engine supports the
 following: * Xterm 256 / RGB hex color support * Complex character movement via
 Paths, Waypoints, and motion easing. * Complex animations via Scenes with
 symbol/color changes, layers, easing, and Path synced progression. * Event
 handling for Path/Scene state changes with custom callback support and many
 pre-defined actions. * Variable stop/step color gradient generation. *
 Extensive effect customization via per-effect arguments. * Runs inline,
 preserving terminal state and workflow. ## Requirements TerminalTextEffects is
 written in Python and does not require any 3rd party modules. Terminal
 interactions use standard ANSI terminal sequences and should work in most
 modern terminals. Note: Windows Terminal performance is slow for some effects.
 ## Installation ```pip install terminaltexteffects``` OR ```pipx install
-terminaltexteffects``` ## Usage ```cat your_text | tte [options]``` OR ``` cat
-your_text | python -m terminaltexteffects [options]``` * Use ``` -h``` to view
-options for a specific effect, such as color or movement direction. * Ex:
-```tte decrypt -h``` ## Options ``` options: -h, --help show this help message
-and exit --tab-width (int > 0) Number of spaces to use for a tab character. --
-xterm-colors Convert any colors specified in RBG hex to the closest XTerm-256
-color. --no-color Disable all colors in the effect. --no-wrap Disable wrapping
-of text. -a ANIMATION_RATE, --animation-rate ANIMATION_RATE Minimum time, in
-seconds, between animation steps. This value does not normally need to be
-modified. Use this to increase the playback speed of all aspects of the effect.
-This will have no impact beyond a certain lower threshold due to the processing
-speed of your device. Effect: Name of the effect to apply. Use -h for effect
+terminaltexteffects``` ## Usage ### Application ```cat your_text | tte
+[options]``` OR ```cat your_text | python -m terminaltexteffects [options]``` *
+Use ``` -h``` to view options for a specific effect, such as color or movement
+direction. * Ex: ```tte decrypt -h``` ### Library All effects are iterators
+which return a string representing the current frame. Basic usage is as simple
+as importing the effect, instantiating it with the input text, and iterating
+over the effect. ```python from terminaltexteffects.effects import effect_rain
+effect = effect_rain.Rain("your text here") for frame in effect: # do something
+with the string ... ``` In the event you want to allow TTE to handle the
+terminal setup/teardown, cursor positioning, and animation frame rate, a
+terminal_output() context manager is available. ```python from
+terminaltexteffects.effects import effect_rain effect = effect_rain.Rain("your
+text here") with effect.terminal_output() as terminal: for frame in effect:
+terminal.print(frame) ``` All command line arguments are available within each
+effect via the `effect.effect_config` and `effect.terminal_config` attributes.
+```python from terminaltexteffects.effects import effect_rain effect =
+effect_rain.Rain("your text here") effect.effect_config.rain_colors =
+("ff0000","00ff00","0000ff") effect.terminal_config.tab_width = 2
+effect.terminal_config.wrap_text = False for frame in effect: # do something
+with the string ... ``` For use cases where the terminal dimensions cannot be
+automatically discovered or you would like to manually define the dimensions,
+the ```effect.terminal_config``` can be configured as follows: ```python
+effect.terminal_config.terminal_dimensions = (80, 24) # width, height ``` If
+you would like to ignore terminal dimensions altogether and base the output
+dimensions solely on the input data: ```python
+effect.terminal_config.ignore_terminal_dimensions = True ``` ## Options
+```markdown options: -h, --help show this help message and exit --tab-width
+(int > 0) Number of spaces to use for a tab character. (default: 4) --xterm-
+colors Convert any colors specified in RBG hex to the closest XTerm-256 color.
+(default: False) --no-color Disable all colors in the effect. (default: False)
+--wrap-text Wrap text wider than the output area width. (default: False) --
+frame-rate FRAME_RATE Target frame rate for the animation. (default: 100) --
+terminal-dimensions TERMINAL_DIMENSIONS TERMINAL_DIMENSIONS Use the terminal
+dimensions to limit the size of the output area and support wrapping. If False,
+the output area is determined by the input data dimensions and may overflow the
+terminal width. (default: (0, 0)) --ignore-terminal-dimensions Ignore the
+terminal dimensions and use the input data dimensions for the output area.
+(default: False) Effect: Name of the effect to apply. Use -h for effect
 specific help.
 {beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,dev,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,test,unstable,verticalslice,vhstape,waves,wipe}
 Available Effects beams Create beams which travel over the output area
 illuminating the characters behind them. binarypath Binary representations of
 each character move through the terminal towards the home coordinate of the
 character. blackhole Characters are consumed by a black hole and explode
 outwards. bouncyballs Characters are bouncy balls falling from the top of the
@@ -71,15 +98,15 @@
 jumbled, explode them to the edge of the output area, then reassemble them in
 the correct layout. verticalslice Slices the input in half vertically and
 slides it into place from opposite directions. vhstape Lines of characters
 glitch left and right and lose detail like an old VHS tape. waves Waves travel
 across the terminal leaving behind the characters. wipe Wipes the text across
 the terminal to reveal characters. Ex: ls -a | tte crumble --final-gradient-
 stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction
-diagonal ``` ## Examples Note: All effects support extensive customization via
+diagonal ``` ### Examples Note: All effects support extensive customization via
 effect specific arguments. The examples shown below only represent one possible
 variant of each effect. Check the effect help output to see arguments. ####
 Beams ![beams_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/
 57874186/6bb98dac-688e-43c9-96aa-1a45f451d4cb) tte beams -h
 beams | Create beams which travel over the output area illuminating the
 characters behind them. options: -h, --help show this help message and exit --
 beam-row-symbols (ASCII/UTF-8 character) [(ASCII/UTF-8 character) ...] Symbols
@@ -929,130 +956,40 @@
 center) Direction of the gradient for the final color. (default:
 Direction.VERTICAL) --wipe-delay (int >= 0) Number of animation cycles to wait
 before adding the next character group. Increase, to slow down the effect.
 (default: 0) Example: terminaltexteffects wipe --wipe-direction
 diagonal_bottom_left_to_top_right --final-gradient-stops 833ab4 fd1d1d fcb045 -
 -final-gradient-steps 12 --final-gradient-frames 5 --wipe-delay 0 ## In-
 Development Preview Any effects shown below are in development and will be
-available in the next release. ## Latest Release Notes ## 0.7.0 ### New
-Features #### Effects * Beams. Light beams travel across the output area and
-illuminate the characters behind them. * Overflow. The input text is scrambled
-by row and repeated randomly, scrolling up the terminal, before eventually
-displaying in the correct order. * OrbitingVolley. Characters fire from
-launcher which orbit output area. * Spotlights. Spotlights search the text
-area, illuminating characters, before converging in the center and expanding.
-#### Engine * Gradients now support multiple step specification to control the
-distance between each stop pair. For example: graphics.Gradient(RED, BLUE,
-YELLOW, steps=(2,5)) results in a spectrum of RED -> (1 step) -> BLUE -> (4
-steps) -> YELLOW * graphics.Gradient.get_color_at_fraction(fraction: float)
-will return a color at the given fraction of the spectrum when provided a float
-between 0 and 1, inclusive. This can be used to match the color to a ratio/ For
-example, the character height in the terminal. *
-graphics.Gradient.build_coordinate_color_mapping() will map gradient colors to
-coordinates in the terminal and supports a Gradient.Direction argument to
-enable gradients in the following directions: horizontal, vertical, diagonal,
-center * graphics.Gradient, if printed, will show a colored spectrum and the
-description of its stops and steps. * The Scene class has a new method:
-apply_gradient_to_symbols(). This method will iterate over a list of symbols
-and apply the colors from a gradient to the symbols. A frame with the symbol
-will be added for each color starting from the last color used in the previous
-symbol, up to the the index determined by the ratio of the current symbol's
-index in the symbols list to the total length of the list. This method allows
-scenes to automatically create frames from a list of symbols and gradient of
-arbitrary length while ensuring every symbol and color is displayed. * On
-instatiation, Terminal creates EffectCharacters for every coordinate in the
-output area that does not have an input character. These EffectCharacters have
-the symbol " " and are stored in Terminal._fill_characters as well as added to
-Terminal.character_by_input_coord. * arg_validators.IntRange will validate a
-range specified as "int-int" and return a tuple[int,int]. *
-arg_validators.FloatRange will validate a range of floats specified as "float-
-float" and return a tuple[float, float]. * character.animation.set_appearance
-(symbol, color) will set the character symbol and color directly. If a Scene is
-active, the appearance will be overwritten with the Scene frame on the next
-call to step_animation(). This method is intended for the occasion where a full
-scene isn't needed, or the appearance needs to be set based on conditions not
-compatible with Scenes or the EventHandler. For example, setting the color
-based on the terminal row. * Terminal.CharacterSort enums moved to
-Terminal.CharacterGroup, Terminal.CharacterSort is now used for sorting and
-return a flat list of characters. * Terminal.CharacterSort has new sort
-methods, TOP_TO_BOTTOM_LEFT_TO_RIGHT, TOP_TO_BOTTOM_RIGHT_TO_LEFT,
-BOTTOM_TO_TOP_LEFT_TO_RIGHT, BOTTOM_TO_TOP_RIGHT_TO_LEFT,
-OUTSIDE_ROW_TO_MIDDLE, MIDDLE_ROW_TO_OUTSIDE * New Terminal.CharacterGroup
-options, CENTER_TO_OUTSIDE_DIAMONDS and OUTSIDE_TO_CENTER_DIAMONS *
-graphics.Animation.adjust_color_brightness(color: graphics.Color, brightness:
-float) will convert the color to HSL, adjust the brightness to the given level,
-and return an RGB hex string. * CTRL-C keyboard interrupt during a running
-effect will exit gracefully. * geometry.find_coords_in_circle() has been
-rewritten to find all coords which fall in an ellipse. The result is a circle
-due to the height/width ratio of terminal cells. This function now finds all
-terminal coordinates within the 'circle' rather than an arbitrary subset. * All
-command line arguments are typed allowing for more easily defined and tested
-effect args. ### Changes #### Effects * All effects have been updated to use
-the latest API calls for improved performance. * All effects support gradients
-for the final appearance. * All effects support gradient direction. * All
-effects have had their default colors refreshed. * ErrorCorrect swap-delay
-lowered and error-pairs specification changed to percent float. * Rain effect
-supports character specification for rain drops and movement speed range for
-the rain drop falling speed. * Print effect uses the row final gradient color
-for the print head color. * RandomSequence effect accepts a starting color and
-a speed. * Rings effect prepares faster. Ring colors are set in order of
-appearance in the ring-colors argument. Ring spin speed is configurable. Rings
-with less than 25% visible characters based on radius are no longer generated.
-Ring gap is set as a percent of the smallest output area dimension. * Scattered
-effect gradient progresses from the first color to the row color. * Spray
-effect spray-volume is specified as a percent of the total number of characters
-and movement speed is a range. * Swarm effect swarm focus points algorithm
-changed to reduce long distances between points. * Decrypt effect supports
-gradient specification for plaintext and multiple color specification for
-ciphertext. * Decrypt effect has a --typing-speed arg to increase the speed of
-the initial text typing effect. * Decrypt effect has had the decrypting speed
-increased. * Beams effect uses Animation.adjust_color_brightness() to lower the
-background character brightness and shows the lighter color when the beam
-passes by. * Crumble effect uses Animation.adjust_color_brightness() to set the
-weak and dust colors based on the final gradient. * Fireworks effect
-launch_delay argument has a +/- 0-50% randomness applied. * Bubbles effect --
-no-rainbow changed to --rainbow and default set to False. * Bubbles effect --
-bubble-color changed to --bubble-colors. Bubble color is randomly chosen from
-the colors unless --rainbow is used. * Burn effect burns faster with some
-randomness in speed. * Burn effect final color fades in from the burned color.
-* Burn effect characters are shown prior to burning using a starting_color arg.
-* Pour effect has a --pour-speed argument. #### Engine * Geometry related
-methods have been removed from the motion class. They are now located at
-terminaltexteffects.utils.geometry as separate functions. * The Coord() object
-definition has been moved from the motion module to the geometry module. *
-Terminal.add_character() takes a geometry.Coord() argument to set the
-character's input_coordinate. * EffectCharacters have a unique ID set by the
-Terminal on instatiation. As a result, all EffectCharacters should be created
-using Terminal.add_character(). * EffectCharacters added by the effect are
-stored in Terminal._added_characters. * Retrieving EffectCharacters from the
-terminal should no longer be done via accessing the lists of characters
-[_added_characters, _fill_characters, _input_characters], but should be
-retrieved via Terminal.get_characters() and Terminal.get_characters_sorted(). *
-Setting EffectCharacter visibility is now done via
-Terminal.set_character_visibility(). This enables the terminal to keep track of
-all visible characters without needing to iterate over all characters on every
-call to _update_terminal_state(). *
-EventHandler.Action.SET_CHARACTER_VISIBILITY_STATE has been removed as
-visibilty state is handled by the Terminal. To enable visibility state changes
-through the event system, use a CALLBACK action with target
-EventHandler.Callback(terminal.set_character_visibility, True/False). *
-geometry.find_coords_on_circle() num_points arg renamed to points_limit and new
-arg unique: bool, added to remove any duplicate Coords. * The animation rate
-argument (-a, --animation-rate) has been removed from all effects and is
-handled as a terminal argument specified prior to the effect name. *
-argtypes.py has been renamed arg_validators.py and all functions have been
-refactored into classes with a METAVAR class member and a type_parser method. *
-easing.EasingFunction type alias used anywhere an easing function is accepted.
-* Exceptions raised are no longer caught in a except clause. Only a finally
-clause is used to restore the cursor. Tracebacks are useful. #### Other * More
-tests have been added. ### Bug Fixes #### Effects * All effects with command
-line options that accept variable length arguments which require at least 1
-argument will present an error message when the option is called with 0
-arguments. #### Engine * Fixed division by zero error in
-geometry.find_coord_at_distance() when the origin coord and the target coord
-are the same. * Fixed gradient generating an extra color in the spectrum when
-the initial color pair was repeated. Ex: Gradient
-('ffffff','000000','ffffff','000000, steps=5) would result in the third color
-'ffffff' being added to the spectrum when it was already present as the end of
-the generation from '000000'->'ffffff'. ## License Distributed under the MIT
-License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/
-main/LICENSE.md) for more information.
+available in the next release. ## Latest Release Notes ## 0.8.0 --- ### New
+Features (0.8.0) --- #### New Engine Features (0.8.0) * Library support: TTE
+effects are now importable. All effects are iterators that return strings for
+each frame of the output. See README for more information. * Terminal: New
+terminal argument (--terminal-dimensions) allows specification of the terminal
+dimensions without relying on auto-detection. Especially useful in cases where
+TTE is being used as a library in non-terminal or TUI contexts. * Terminal: New
+terminal argument (--ignore-terminal-dimensions) causes the output area
+dimensions to match the input data dimensions without regard to the terminal.
+### Changes (0.8.0) --- #### Effects Changes (0.8.0) * Scattered. Holds
+scrambled text at the start for a few frames. * Scattered. Lowered default
+movement-speed from 0.5 to 0.3. #### Engine Changes (0.8.0) * graphics.Gradient
+```__iter___()``` refactored to return a generator. No longer improperly
+implements the iterator protocol by resetting index in ```___iter__()```. *
+Terminal: Argument --animation-rate is now --frame-rate and is specified as a
+target frames per second. * Terminal: Argument --no-wrap is now --wrap-text and
+defaults to False. * Terminal: If a terminal object is instantiated without a
+TerminalConfig passed, it will instantiate a new TerminalConfig. * Terminal:
+Terminal.get_formatted_output_string() will return a string representing the
+current frame. * Terminal: Terminal.print() will print the frame to the
+terminal and handle cursor position. The optional argument (enforce_frame_rate:
+bool = True) determines if the frame rate set at Terminal.config.frame_rate is
+enforced. If set to False, the print will occur without delay. * New argument
+validator for terminal dimensions (arg_validators.TerminalDeminsions). * New
+module base_effect.py: * base_effect.BaseEffect: * This is an abstract class
+which forms the base iterable for all effects and provides the terminal_output
+() context manager. * base_effect.BaseEffectIterator: * This is an abstract
+class which provides the functionality to enable iteration over effects. ###
+Bug Fixes (0.8.0) --- #### Engine Fixes (0.8.0) * Fixed Argfield nargs type
+from str to str | int. * Implemented custom formatter into argsdataclass.py
+argument parsing. ## License Distributed under the MIT License. See [LICENSE]
+(https://github.com/ChrisBuilds/terminaltexteffects/blob/main/LICENSE.md) for
+more information.
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/__main__.py` & `terminaltexteffects-0.8.0/terminaltexteffects/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import argparse
 import importlib
 import pkgutil
-import sys
 
 import terminaltexteffects.effects
-import terminaltexteffects.utils.ansitools as ansitools
 import terminaltexteffects.utils.terminal as term
 from terminaltexteffects.utils.argsdataclass import ArgsDataClass
-from terminaltexteffects.utils.terminal import TerminalArgs
+from terminaltexteffects.utils.terminal import TerminalConfig
 
 
 def main():
     parser = (argparse.ArgumentParser)(
         prog="terminaltexteffects",
         description="Apply visual effects to terminal text piped in from stdin.",
         epilog="Ex: ls -a | python -m terminaltexteffects --xterm-colors decrypt -a 0.002 --ciphertext-color 00ff00 --plaintext-color ff0000 --final-color 0000ff",
     )
 
-    TerminalArgs.add_args_to_parser(parser)
+    TerminalConfig._add_args_to_parser(parser)
 
     subparsers = parser.add_subparsers(
         title="Effect",
         description="Name of the effect to apply. Use <effect> -h for effect specific help.",
         help="Available Effects",
         required=True,
     )
@@ -29,27 +27,28 @@
     for module_info in pkgutil.iter_modules(
         terminaltexteffects.effects.__path__, terminaltexteffects.effects.__name__ + "."
     ):
         module = importlib.import_module(module_info.name)
 
         if hasattr(module, "get_effect_and_args"):
             effect_class, args_class = tuple[any, ArgsDataClass](module.get_effect_and_args())
-            args_class.add_to_args_subparsers(subparsers)
+            args_class._add_to_args_subparsers(subparsers)
 
     args = parser.parse_args()
     input_data = term.Terminal.get_piped_input()
     if not input_data.strip():
         print("NO INPUT.")
     else:
-        try:
-            terminal_args = TerminalArgs.from_parsed_args_mapping(args, TerminalArgs)
-            terminal = term.Terminal(input_data, terminal_args)
-            effect_args = ArgsDataClass.from_parsed_args_mapping(args)
-            effect_class = effect_args.get_effect_class()
-            effect = effect_class(terminal, effect_args)
-            effect.run()
-        finally:
-            sys.stdout.write(ansitools.SHOW_CURSOR())
+        terminal_config = TerminalConfig._from_parsed_args_mapping(args, TerminalConfig)
+        effect_config = ArgsDataClass._from_parsed_args_mapping(args)
+        effect_class = effect_config.get_effect_class()
+        terminal_config.use_terminal_dimensions = True
+        effect = effect_class(input_data)
+        effect.effect_config = effect_config
+        effect.terminal_config = terminal_config
+        with effect.terminal_output() as terminal:
+            for frame in effect:
+                terminal.print(frame)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/base_character.py` & `terminaltexteffects-0.8.0/terminaltexteffects/base_character.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_beams.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_beams.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,266 +1,324 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return BeamsEffect, BeamsEffectArgs
+    return Beams, BeamsConfig
 
 
 @argclass(
     name="beams",
-    formatter_class=arg_validators.CustomFormatter,
     help="Create beams which travel over the output area illuminating the characters behind them.",
     description="beams | Create beams which travel over the output area illuminating the characters behind them.",
     epilog="""Example: terminaltexteffects beams --beam-row-symbols ▂ ▁ _ --beam-column-symbols ▌ ▍ ▎ ▏ --beam-delay 10 --beam-row-speed-range 10-40 --beam-column-speed-range 6-10 --beam-gradient-stops ffffff 00D1FF 8A008A --beam-gradient-steps 2 8 --beam-gradient-frames 2 --final-gradient-stops 8A008A 00D1FF ffffff --final-gradient-steps 12 --final-gradient-frames 5 --final-gradient-direction vertical --final-wipe-speed 1""",
 )
 @dataclass
-class BeamsEffectArgs(ArgsDataClass):
+class BeamsConfig(ArgsDataClass):
+    """Configuration for the Beams effect.
+
+    Attributes:
+        beam_row_symbols (tuple[str, ...]): Symbols to use for the beam effect when moving along a row. Strings will be used in sequence to create an animation.
+        beam_column_symbols (tuple[str, ...]): Symbols to use for the beam effect when moving along a column. Strings will be used in sequence to create an animation.
+        beam_delay (int): Number of frames to wait before adding the next group of beams. Beams are added in groups of size random(1, 5).
+        beam_row_speed_range (tuple[int, int]): Speed range of the beam when moving along a row.
+        beam_column_speed_range (tuple[int, int]): Speed range of the beam when moving along a column.
+        beam_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the beam, a gradient will be created between the colors.
+        beam_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops.
+        beam_gradient_frames (int): Number of frames to display each gradient step.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the wipe gradient.
+        final_gradient_steps (tuple[int,]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops.
+        final_gradient_frames (int): Number of frames to display each gradient step.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        final_wipe_speed (int): Speed of the final wipe as measured in diagonal groups activated per frame.
+    """
+
     beam_row_symbols: tuple[str, ...] = ArgField(
         cmd_name="--beam-row-symbols",
         type_parser=arg_validators.Symbol.type_parser,
         nargs="+",
         default=("▂", "▁", "_"),
         metavar=arg_validators.Symbol.METAVAR,
         help="Symbols to use for the beam effect when moving along a row. Strings will be used in sequence to create an animation.",
     )  # type: ignore[assignment]
+
+    "tuple[str, ...] : Symbols to use for the beam effect when moving along a row. Strings will be used in sequence to create an animation."
+
     beam_column_symbols: tuple[str, ...] = ArgField(
         cmd_name="--beam-column-symbols",
         type_parser=arg_validators.Symbol.type_parser,
         nargs="+",
         default=("▌", "▍", "▎", "▏"),
         metavar=arg_validators.Symbol.METAVAR,
         help="Symbols to use for the beam effect when moving along a column. Strings will be used in sequence to create an animation.",
     )  # type: ignore[assignment]
+
+    "tuple[str, ...] : Symbols to use for the beam effect when moving along a column. Strings will be used in sequence to create an animation."
+
     beam_delay: int = ArgField(
         cmd_name="--beam-delay",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=10,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Number of frames to wait before adding the next group of beams. Beams are added in groups of size random(1, 5).",
     )  # type: ignore[assignment]
+
+    "int : Number of frames to wait before adding the next group of beams. Beams are added in groups of size random(1, 5)."
+
     beam_row_speed_range: tuple[int, int] = ArgField(
         cmd_name="--beam-row-speed-range",
         type_parser=arg_validators.IntRange.type_parser,
         default=(10, 40),
         metavar=arg_validators.IntRange.METAVAR,
-        help="Minimum speed of the beam when moving along a row.",
+        help="Speed range of the beam when moving along a row.",
     )  # type: ignore[assignment]
+
+    "tuple[int, int] : Speed range of the beam when moving along a row."
+
     beam_column_speed_range: tuple[int, int] = ArgField(
         cmd_name="--beam-column-speed-range",
         type_parser=arg_validators.IntRange.type_parser,
         default=(6, 10),
         metavar=arg_validators.IntRange.METAVAR,
-        help="Minimum speed of the beam when moving along a column.",
+        help="Speed range of the beam when moving along a column.",
     )  # type: ignore[assignment]
+
+    "tuple[int, int] : Speed range of the beam when moving along a column."
+
     beam_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--beam-gradient-stops",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("ffffff", "00D1FF", "8A008A"),
         metavar="(XTerm [0-255] OR RGB Hex [000000-ffffff])",
         help="Space separated, unquoted, list of colors for the beam, a gradient will be created between the colors.",
     )  # type: ignore[assignment]
+
+    "tuple[graphics.Color, ...] : Tuple of colors for the beam, a gradient will be created between the colors."
+
     beam_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--beam-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(2, 8),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, numbers for the of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops.",
     )  # type: ignore[assignment]
+
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops."
+
     beam_gradient_frames: int = ArgField(
         cmd_name="--beam-gradient-frames",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=2,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Number of frames to display each gradient step.",
     )  # type: ignore[assignment]
+
+    "int : Number of frames to display each gradient step."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--final-gradient-stops",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "ffffff"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the wipe gradient.",
     )  # type: ignore[assignment]
+
+    "tuple[graphics.Color, ...] : Tuple of colors for the wipe gradient."
+
     final_gradient_steps: tuple[int,] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, numbers for the of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops.",
     )  # type: ignore[assignment]
+
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation. Steps are paired with the colors in final-gradient-stops."
+
     final_gradient_frames: int = ArgField(
         cmd_name="--final-gradient-frames",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=5,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Number of frames to display each gradient step.",
     )  # type: ignore[assignment]
+
+    "int : Number of frames to display each gradient step."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     final_wipe_speed: int = ArgField(
         cmd_name="--final-wipe-speed",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=1,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Speed of the final wipe as measured in diagonal groups activated per frame.",
     )  # type: ignore[assignment]
 
+    "int : Speed of the final wipe as measured in diagonal groups activated per frame."
+
     @classmethod
     def get_effect_class(cls):
-        return BeamsEffect
-
+        return Beams
 
-class Group:
-    def __init__(self, characters: list[EffectCharacter], direction: str, terminal: Terminal, args: BeamsEffectArgs):
-        self.characters = characters
-        self.direction: str = direction
-        self.terminal = terminal
-        direction_speed_range = {
-            "row": (args.beam_row_speed_range[0], args.beam_row_speed_range[1]),
-            "column": (args.beam_column_speed_range[0], args.beam_column_speed_range[1]),
-        }
-        self.speed = random.randint(direction_speed_range[direction][0], direction_speed_range[direction][1]) * 0.1
-        self.next_character_counter: float = 0
-        if self.direction == "row":
-            self.characters.sort(key=lambda character: character.input_coord.column)
-        elif self.direction == "column":
-            self.characters.sort(key=lambda character: character.input_coord.row)
-        if random.choice([True, False]):
-            self.characters.reverse()
-
-    def increment_next_character_counter(self) -> None:
-        self.next_character_counter += self.speed
-
-    def get_next_character(self) -> EffectCharacter | None:
-        self.next_character_counter -= 1
-        next_character = self.characters.pop(0)
-        if next_character.animation.active_scene:
-            next_character.animation.active_scene.reset_scene()
-            return_value = None
-        else:
-            self.terminal.set_character_visibility(next_character, True)
-            return_value = next_character
-        next_character.animation.activate_scene(next_character.animation.query_scene("beam_" + self.direction))
-        return return_value
-
-    def complete(self) -> bool:
-        return not self.characters
-
-
-class BeamsEffect:
-    """Effect that creates beams which travel over the output area illuminated the characters behind them."""
 
-    def __init__(self, terminal: Terminal, args: BeamsEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_groups: list[Group] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+class BeamsIterator(BaseEffectIterator[BeamsConfig]):
+    class _Group:
+        def __init__(self, characters: list[EffectCharacter], direction: str, terminal: Terminal, args: BeamsConfig):
+            self.characters = characters
+            self.direction: str = direction
+            self.terminal = terminal
+            direction_speed_range = {
+                "row": (args.beam_row_speed_range[0], args.beam_row_speed_range[1]),
+                "column": (args.beam_column_speed_range[0], args.beam_column_speed_range[1]),
+            }
+            self.speed = random.randint(direction_speed_range[direction][0], direction_speed_range[direction][1]) * 0.1
+            self.next_character_counter: float = 0
+            if self.direction == "row":
+                self.characters.sort(key=lambda character: character.input_coord.column)
+            elif self.direction == "column":
+                self.characters.sort(key=lambda character: character.input_coord.row)
+            if random.choice([True, False]):
+                self.characters.reverse()
+
+        def increment_next_character_counter(self) -> None:
+            self.next_character_counter += self.speed
+
+        def get_next_character(self) -> EffectCharacter | None:
+            self.next_character_counter -= 1
+            next_character = self.characters.pop(0)
+            if next_character.animation.active_scene:
+                next_character.animation.active_scene.reset_scene()
+                return_value = None
+            else:
+                self.terminal.set_character_visibility(next_character, True)
+                return_value = next_character
+            next_character.animation.activate_scene(next_character.animation.query_scene("beam_" + self.direction))
+            return return_value
+
+        def complete(self) -> bool:
+            return not self.characters
+
+    def __init__(self, effect: "Beams") -> None:
+        super().__init__(effect)
+        self._pending_groups: list[BeamsIterator._Group] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.active_groups: list[BeamsIterator._Group] = []
+        self.delay = 0
+        self.phase = "beams"
+        self.final_wipe_groups = self._terminal.get_characters_grouped(
+            Terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT
+        )
+        self._build()
 
-    def prepare_data(self) -> None:  # testing
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters(fill_chars=True):
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self._terminal.get_characters(fill_chars=True):
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
 
-        beam_gradient = graphics.Gradient(*self.args.beam_gradient_stops, steps=self.args.beam_gradient_steps)
-        groups: list[Group] = []
-        for row in self.terminal.get_characters_grouped(Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True):
-            groups.append(Group(row, "row", self.terminal, self.args))
-        for column in self.terminal.get_characters_grouped(
+        beam_gradient = graphics.Gradient(*self._config.beam_gradient_stops, steps=self._config.beam_gradient_steps)
+        groups: list[BeamsIterator._Group] = []
+        for row in self._terminal.get_characters_grouped(Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True):
+            groups.append(BeamsIterator._Group(row, "row", self._terminal, self._config))
+        for column in self._terminal.get_characters_grouped(
             Terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT, fill_chars=True
         ):
-            groups.append(Group(column, "column", self.terminal, self.args))
+            groups.append(BeamsIterator._Group(column, "column", self._terminal, self._config))
         for group in groups:
             for character in group.characters:
                 beam_row_scn = character.animation.new_scene(id="beam_row")
                 beam_column_scn = character.animation.new_scene(id="beam_column")
                 beam_row_scn.apply_gradient_to_symbols(
-                    beam_gradient, self.args.beam_row_symbols, self.args.beam_gradient_frames
+                    beam_gradient, self._config.beam_row_symbols, self._config.beam_gradient_frames
                 )
                 beam_column_scn.apply_gradient_to_symbols(
-                    beam_gradient, self.args.beam_column_symbols, self.args.beam_gradient_frames
+                    beam_gradient, self._config.beam_column_symbols, self._config.beam_gradient_frames
                 )
                 faded_color = character.animation.adjust_color_brightness(
-                    self.character_final_color_map[character], 0.3
+                    self._character_final_color_map[character], 0.3
                 )
-                fade_gradient = graphics.Gradient(self.character_final_color_map[character], faded_color, steps=10)
+                fade_gradient = graphics.Gradient(self._character_final_color_map[character], faded_color, steps=10)
                 beam_row_scn.apply_gradient_to_symbols(fade_gradient, character.input_symbol, 5)
                 beam_column_scn.apply_gradient_to_symbols(fade_gradient, character.input_symbol, 5)
-                brighten_gradient = graphics.Gradient(faded_color, self.character_final_color_map[character], steps=10)
+                brighten_gradient = graphics.Gradient(faded_color, self._character_final_color_map[character], steps=10)
                 brigthen_scn = character.animation.new_scene(id="brighten")
                 brigthen_scn.apply_gradient_to_symbols(
-                    brighten_gradient, character.input_symbol, self.args.final_gradient_frames
+                    brighten_gradient, character.input_symbol, self._config.final_gradient_frames
                 )
-        self.pending_groups = groups
-        random.shuffle(self.pending_groups)
+        self._pending_groups = groups
+        random.shuffle(self._pending_groups)
 
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        active_groups: list[Group] = []
-        delay = 0
-        phase = "beams"
-        final_wipe_groups = self.terminal.get_characters_grouped(
-            Terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT
-        )
-        while phase != "complete" or self.active_chars:
-            if phase == "beams":
-                if not delay:
-                    if self.pending_groups:
+    def __next__(self) -> str:
+        if self.phase != "complete" or self._active_chars:
+            if self.phase == "beams":
+                if not self.delay:
+                    if self._pending_groups:
                         for _ in range(random.randint(1, 5)):
-                            if self.pending_groups:
-                                active_groups.append(self.pending_groups.pop(0))
-                    delay = self.args.beam_delay
+                            if self._pending_groups:
+                                self.active_groups.append(self._pending_groups.pop(0))
+                    self.delay = self._config.beam_delay
                 else:
-                    delay -= 1
-                for group in active_groups:
+                    self.delay -= 1
+                for group in self.active_groups:
                     group.increment_next_character_counter()
                     if int(group.next_character_counter) > 1:
                         for _ in range(int(group.next_character_counter)):
                             if not group.complete():
                                 next_char = group.get_next_character()
                                 if next_char:
-                                    self.active_chars.append(next_char)
-                active_groups = [group for group in active_groups if not group.complete()]
-                if not self.pending_groups and not active_groups and not self.active_chars:
-                    phase = "final_wipe"
-            elif phase == "final_wipe":
-                if final_wipe_groups:
-                    for _ in range(self.args.final_wipe_speed):
-                        if not final_wipe_groups:
+                                    self._active_chars.append(next_char)
+                self.active_groups = [group for group in self.active_groups if not group.complete()]
+                if not self._pending_groups and not self.active_groups and not self._active_chars:
+                    self.phase = "final_wipe"
+            elif self.phase == "final_wipe":
+                if self.final_wipe_groups:
+                    for _ in range(self._config.final_wipe_speed):
+                        if not self.final_wipe_groups:
                             break
-                        next_group = final_wipe_groups.pop(0)
+                        next_group = self.final_wipe_groups.pop(0)
                         for character in next_group:
                             character.animation.activate_scene(character.animation.query_scene("brighten"))
-                            self.terminal.set_character_visibility(character, True)
-                            self.active_chars.append(character)
+                            self._terminal.set_character_visibility(character, True)
+                            self._active_chars.append(character)
                 else:
-                    phase = "complete"
-            self.terminal.print()
-            self.animate_chars()
-
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-        self.terminal.print()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+                    self.phase = "complete"
+            next_frame = self._terminal.get_formatted_output_string()
+            for character in self._active_chars:
+                character.tick()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return next_frame
+        else:
+            raise StopIteration
+
+
+class Beams(BaseEffect[BeamsConfig]):
+    """Effect that creates beams which travel over the output area illuminated the characters behind them."""
+
+    _config_cls = BeamsConfig
+    _iterator_cls = BeamsIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_binarypath.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_binarypath.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,143 +1,175 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return BinaryPathEffect, BinaryPathEffectArgs
+    return BinaryPath, BinaryPathConfig
 
 
 @argclass(
     name="binarypath",
-    formatter_class=arg_validators.CustomFormatter,
     help="Binary representations of each character move through the terminal towards the home coordinate of the character.",
     description="binarypath | Binary representations of each character move through the terminal towards the home coordinate of the character.",
     epilog="""Example: terminaltexteffects binarypath --final-gradient-stops 00d500 007500 --final-gradient-steps 12 --final-gradient-direction vertical --binary-colors 044E29 157e38 45bf55 95ed87 --movement-speed 1.0 --active-binary-groups 0.05""",
 )
 @dataclass
-class BinaryPathEffectArgs(ArgsDataClass):
+class BinaryPathConfig(ArgsDataClass):
+    """Configuration for the BinaryPath effect.
+
+    Attributes:
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        binary_colors (tuple[graphics.Color, ...]): Tuple of colors for the binary characters. Character color is randomly assigned from this list.
+        movement_speed (float): Speed of the binary groups as they travel around the terminal.
+        active_binary_groups (float): Maximum number of binary groups that are active at any given time as a percentage of the total number of binary groups. Lower this to improve performance."""
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("00d500", "007500"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.CENTER,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     binary_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--binary-colors"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("044E29", "157e38", "45bf55", "95ed87"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the binary characters. Character color is randomly assigned from this list.",
     )  # type: ignore[assignment]
+
+    "tuple[graphics.Color, ...] : Tuple of colors for the binary characters. Character color is randomly assigned from this list."
+
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
         type_parser=arg_validators.PositiveFloat.type_parser,
         default=1.0,
         metavar=arg_validators.PositiveFloat.METAVAR,
         help="Speed of the binary groups as they travel around the terminal.",
     )  # type: ignore[assignment]
+
+    "float : Speed of the binary groups as they travel around the terminal."
+
     active_binary_groups: float = ArgField(
         cmd_name="--active-binary-groups",
         type_parser=arg_validators.Ratio.type_parser,
         default=0.05,
         metavar=arg_validators.Ratio.METAVAR,
-        help="Maximum number of binary groups that are active at any given time. Lower this to improve performance.",
+        help="Maximum number of binary groups that are active at any given time as a percentage of the total number of binary groups. Lower this to improve performance.",
     )  # type: ignore[assignment]
 
+    "float : Maximum number of binary groups that are active at any given time as a percentage of the total number of binary groups. Lower this to improve performance."
+
     @classmethod
     def get_effect_class(cls):
-        return BinaryPathEffect
-
-
-class BinaryRepresentation:
-    def __init__(self, character: EffectCharacter, terminal: Terminal):
-        self.character = character
-        self.terminal = terminal
-        self.binary_string = format(ord(self.character.symbol), "08b")
-        self.binary_characters: list[EffectCharacter] = []
-        self.pending_binary_characters: list[EffectCharacter] = []
-        self.input_coord = self.character.input_coord
-        self.is_active = False
-
-    def travel_complete(self) -> bool:
-        """Determines if the binary representation has completed its travel, meaning all binary characters have reached their input coordinate.
-
-        Returns:
-            bool: True if the binary representation has completed its travel, False otherwise.
-        """
-        return all(bin_char.motion.current_coord == self.input_coord for bin_char in self.binary_characters)
-
-    def deactivate(self) -> None:
-        """Deactivates the binary representation by deactivating all binary characters."""
-        for bin_char in self.binary_characters:
-            self.terminal.set_character_visibility(bin_char, False)
-        self.is_active = False
-
-    def activate_source_character(self) -> None:
-        """Activates the source character of the binary representation."""
-        self.terminal.set_character_visibility(self.character, True)
-        self.character.animation.activate_scene(self.character.animation.query_scene("collapse_scn"))
+        return BinaryPath
 
 
-class BinaryPathEffect:
-    """Effect that decodes characters into their binary form. Characters travel from outside the output area towards their input coordinate,
-    moving at right angles."""
+class BinaryPathIterator(BaseEffectIterator[BinaryPathConfig]):
+    class _BinaryRepresentation:
+        def __init__(self, character: EffectCharacter, terminal: Terminal):
+            self.character = character
+            self.terminal = terminal
+            self.binary_string = format(ord(self.character.symbol), "08b")
+            self.binary_characters: list[EffectCharacter] = []
+            self.pending_binary_characters: list[EffectCharacter] = []
+            self.input_coord = self.character.input_coord
+            self.is_active = False
+
+        def travel_complete(self) -> bool:
+            """Determines if the binary representation has completed its travel, meaning all binary characters have reached their input coordinate.
+
+            Returns:
+                bool: True if the binary representation has completed its travel, False otherwise.
+            """
+            return all(bin_char.motion.current_coord == self.input_coord for bin_char in self.binary_characters)
+
+        def deactivate(self) -> None:
+            """Deactivates the binary representation by deactivating all binary characters."""
+            for bin_char in self.binary_characters:
+                self.terminal.set_character_visibility(bin_char, False)
+            self.is_active = False
+
+        def activate_source_character(self) -> None:
+            """Activates the source character of the binary representation."""
+            self.terminal.set_character_visibility(self.character, True)
+            self.character.animation.activate_scene(self.character.animation.query_scene("collapse_scn"))
+
+    def __init__(self, effect: "BinaryPath") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._pending_binary_representations: list[BinaryPathIterator._BinaryRepresentation] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._last_frame_provided = False
+        self._active_binary_reps: list[BinaryPathIterator._BinaryRepresentation] = []
+        self._complete = False
+        self._phase = "travel"
+        self._final_wipe_chars = self._terminal.get_characters_grouped(
+            grouping=self._terminal.CharacterGroup.DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT
+        )
+        self._max_active_binary_groups: int = 0
 
-    def __init__(self, terminal: Terminal, args: BinaryPathEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.pending_binary_representations: list[BinaryRepresentation] = []
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
 
-    def prepare_data(self) -> None:
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
 
-        for character in self.terminal.get_characters():
-            bin_rep = BinaryRepresentation(character, self.terminal)
+        for character in self._terminal.get_characters():
+            bin_rep = BinaryPathIterator._BinaryRepresentation(character, self._terminal)
             for binary_char in bin_rep.binary_string:
-                bin_rep.binary_characters.append(self.terminal.add_character(binary_char, Coord(0, 0)))
+                bin_rep.binary_characters.append(self._terminal.add_character(binary_char, Coord(0, 0)))
                 bin_rep.pending_binary_characters.append(bin_rep.binary_characters[-1])
-            self.pending_binary_representations.append(bin_rep)
+            self._pending_binary_representations.append(bin_rep)
 
-        for bin_rep in self.pending_binary_representations:
+        for bin_rep in self._pending_binary_representations:
             path_coords: list[Coord] = []
-            starting_coord = self.terminal.output_area.random_coord(outside_scope=True)
+            starting_coord = self._terminal.output_area.random_coord(outside_scope=True)
             path_coords.append(starting_coord)
             last_orientation = random.choice(("col", "row"))
             while path_coords[-1] != bin_rep.character.input_coord:
                 last_coord = path_coords[-1]
                 if last_coord.column > bin_rep.character.input_coord.column:
                     column_direction = -1
                 elif last_coord.column == bin_rep.character.input_coord.column:
@@ -153,15 +185,15 @@
                 max_column_distance = abs(last_coord.column - bin_rep.character.input_coord.column)
                 max_row_distance = abs(last_coord.row - bin_rep.character.input_coord.row)
                 if last_orientation == "col" and max_row_distance > 0:
                     next_coord = Coord(
                         last_coord.column,
                         last_coord.row
                         + (
-                            random.randint(1, min(max_row_distance, max(10, int(self.terminal.input_width * 0.2))))
+                            random.randint(1, min(max_row_distance, max(10, int(self._terminal.input_width * 0.2))))
                             * row_direction
                         ),
                     )
                     last_orientation = "row"
                 elif last_orientation == "row" and max_column_distance > 0:
                     next_coord = Coord(
                         last_coord.column + (random.randint(1, min(max_column_distance, 4)) * column_direction),
@@ -174,82 +206,91 @@
                 path_coords.append(next_coord)
 
             path_coords.append(next_coord)
             final_coord = bin_rep.character.input_coord
             path_coords.append(final_coord)
             for bin_effectchar in bin_rep.binary_characters:
                 bin_effectchar.motion.set_coordinate(path_coords[0])
-                digital_path = bin_effectchar.motion.new_path(speed=self.args.movement_speed)
+                digital_path = bin_effectchar.motion.new_path(speed=self._config.movement_speed)
                 for coord in path_coords:
                     digital_path.new_waypoint(coord)
                 bin_effectchar.motion.activate_path(digital_path)
                 bin_effectchar.layer = 1
                 color_scn = bin_effectchar.animation.new_scene()
-                color_scn.add_frame(bin_effectchar.symbol, 1, color=random.choice(self.args.binary_colors))
+                color_scn.add_frame(bin_effectchar.symbol, 1, color=random.choice(self._config.binary_colors))
                 bin_effectchar.animation.activate_scene(color_scn)
 
-        for character in self.terminal.get_characters():
+        for character in self._terminal.get_characters():
             collapse_scn = character.animation.new_scene(ease=easing.in_quad, id="collapse_scn")
-            dim_color = character.animation.adjust_color_brightness(self.character_final_color_map[character], 0.5)
+            dim_color = character.animation.adjust_color_brightness(self._character_final_color_map[character], 0.5)
             dim_gradient = graphics.Gradient("ffffff", dim_color, steps=10)
             collapse_scn.apply_gradient_to_symbols(dim_gradient, character.input_symbol, 7)
 
             brighten_scn = character.animation.new_scene(id="brighten_scn")
-            brighten_gradient = graphics.Gradient(dim_color, self.character_final_color_map[character], steps=10)
+            brighten_gradient = graphics.Gradient(dim_color, self._character_final_color_map[character], steps=10)
             brighten_scn.apply_gradient_to_symbols(brighten_gradient, character.input_symbol, 2)
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        active_binary_reps: list[BinaryRepresentation] = []
-        complete = False
-        phase = "travel"
-        final_wipe_chars = self.terminal.get_characters_grouped(
-            grouping=self.terminal.CharacterGroup.DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT
+        self._max_active_binary_groups = max(
+            1, int(self._config.active_binary_groups * len(self._pending_binary_representations))
         )
-        max_active_binary_groups = max(
-            1, int(self.args.active_binary_groups * len(self.pending_binary_representations))
-        )
-        while not complete or self.active_chars:
-            if phase == "travel":
-                while len(active_binary_reps) < max_active_binary_groups and self.pending_binary_representations:
-                    next_binary_rep = self.pending_binary_representations.pop(
-                        random.randrange(len(self.pending_binary_representations))
+
+    def __next__(self) -> str:
+        if not self._complete or self._active_chars:
+            if self._phase == "travel":
+                while (
+                    len(self._active_binary_reps) < self._max_active_binary_groups
+                    and self._pending_binary_representations
+                ):
+                    next_binary_rep = self._pending_binary_representations.pop(
+                        random.randrange(len(self._pending_binary_representations))
                     )
                     next_binary_rep.is_active = True
-                    active_binary_reps.append(next_binary_rep)
+                    self._active_binary_reps.append(next_binary_rep)
 
-                if active_binary_reps:
-                    for active_rep in active_binary_reps:
+                if self._active_binary_reps:
+                    for active_rep in self._active_binary_reps:
                         if active_rep.pending_binary_characters:
                             next_char = active_rep.pending_binary_characters.pop(0)
-                            self.active_chars.append(next_char)
-                            self.terminal.set_character_visibility(next_char, True)
+                            self._active_chars.append(next_char)
+                            self._terminal.set_character_visibility(next_char, True)
                         elif active_rep.travel_complete():
                             active_rep.deactivate()
                             active_rep.activate_source_character()
-                            self.active_chars.append(active_rep.character)
-
-                    active_binary_reps = [binary_rep for binary_rep in active_binary_reps if binary_rep.is_active]
+                            self._active_chars.append(active_rep.character)
 
-                if not self.active_chars:
-                    phase = "wipe"
-
-            if phase == "wipe":
-                if final_wipe_chars:
-                    next_group = final_wipe_chars.pop(0)
+                    self._active_binary_reps = [
+                        binary_rep for binary_rep in self._active_binary_reps if binary_rep.is_active
+                    ]
+
+                if not self._active_chars:
+                    self._phase = "wipe"
+
+            if self._phase == "wipe":
+                if self._final_wipe_chars:
+                    next_group = self._final_wipe_chars.pop(0)
                     for character in next_group:
                         character.animation.activate_scene(character.animation.query_scene("brighten_scn"))
-                        self.terminal.set_character_visibility(character, True)
-                        self.active_chars.append(character)
+                        self._terminal.set_character_visibility(character, True)
+                        self._active_chars.append(character)
                 else:
-                    complete = True
-            self.terminal.print()
-            self.animate_chars()
-
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-        self.terminal.print()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+                    self._complete = True
+            next_frame = self._terminal.get_formatted_output_string()
+            for character in self._active_chars:
+                character.tick()
+
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return next_frame
+        elif not self._last_frame_provided:
+            self._last_frame_provided = True
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class BinaryPath(BaseEffect):
+    """Effect that decodes characters into their binary form. Characters travel from outside the output area towards their input coordinate,
+    moving at right angles."""
+
+    _config_cls = BinaryPathConfig
+    _iterator_cls = BinaryPathIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_blackhole.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_blackhole.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,96 +1,116 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import animation, easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return BlackholeEffect, BlackholeEffectArgs
+    return Blackhole, BlackholeConfig
 
 
 @argclass(
     name="blackhole",
-    formatter_class=arg_validators.CustomFormatter,
     help="Characters are consumed by a black hole and explode outwards.",
     description="blackhole | Characters are consumed by a black hole and explode outwards.",
     epilog="""Example: terminaltexteffects blackhole --star-colors ffcc0d ff7326 ff194d bf2669 702a8c 049dbf --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-direction vertical""",
 )
 @dataclass
-class BlackholeEffectArgs(ArgsDataClass):
+class BlackholeConfig(ArgsDataClass):
+    """Configuration for the Blackhole effect.
+
+    Attributes:
+        blackhole_color (graphics.Color): Color for the stars that comprise the blackhole border.
+        star_colors (tuple[graphics.Color, ...]): Tuple of colors from which character colors will be chosen and applied after the explosion, but before the cooldown to final color.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color."""
+
     blackhole_color: graphics.Color = ArgField(
         cmd_name=["--blackhole-color"],
         type_parser=arg_validators.Color.type_parser,
         default="ffffff",
         metavar=arg_validators.Color.METAVAR,
         help="Color for the stars that comprise the blackhole border.",
     )  # type: ignore[assignment]
+
+    "graphics.Color : Color for the stars that comprise the blackhole border."
+
     star_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--star-colors"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("ffcc0d", "ff7326", "ff194d", "bf2669", "702a8c", "049dbf"),
         metavar=arg_validators.Color.METAVAR,
         help="List of colors from which character colors will be chosen and applied after the explosion, but before the cooldown to final color.",
     )  # type: ignore[assignment]
+
+    "tuple[graphics.Color, ...] : Tuple of colors from which character colors will be chosen and applied after the explosion, but before the cooldown to final color."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "ffffff"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
 
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     @classmethod
     def get_effect_class(cls):
-        return BlackholeEffect
+        return Blackhole
 
 
-class BlackholeEffect:
-    """Effect that creates a blackhole in a starfield, consumes the stars, and explodes the input characters out to position."""
-
-    def __init__(self, terminal: Terminal, args: BlackholeEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.blackhole_chars: list[EffectCharacter] = []
-        self.awaiting_consumption_chars: list[EffectCharacter] = []
-        self.blackhole_radius = max(
+class BlackholeIterator(BaseEffectIterator[BlackholeConfig]):
+    def __init__(self, effect: "Blackhole") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._blackhole_chars: list[EffectCharacter] = []
+        self._awaiting_consumption_chars: list[EffectCharacter] = []
+        self._blackhole_radius = max(
             min(
-                round(self.terminal.output_area.right * 0.3),
-                round(self.terminal.output_area.top * 0.3),
+                round(self._terminal.output_area.right * 0.3),
+                round(self._terminal.output_area.top * 0.3),
             ),
             3,
         )
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
 
-    def prepare_blackhole(self) -> None:
+    def _prepare_blackhole(self) -> None:
         star_symbols = [
             "*",
             "✸",
             "✺",
             "✹",
             "✷",
             "✵",
@@ -107,71 +127,71 @@
             "⬦",
             "⬥",
         ]
         starfield_colors = graphics.Gradient("4a4a4d", "ffffff", steps=6).spectrum
         gradient_map = {}
         for color in starfield_colors:
             gradient_map[color] = graphics.Gradient(color, "000000", steps=10)
-        available_chars = list(self.terminal._input_characters)
-        while len(self.blackhole_chars) < self.blackhole_radius * 3 and available_chars:
-            self.blackhole_chars.append(available_chars.pop(random.randrange(0, len(available_chars))))
+        available_chars = list(self._terminal._input_characters)
+        while len(self._blackhole_chars) < self._blackhole_radius * 3 and available_chars:
+            self._blackhole_chars.append(available_chars.pop(random.randrange(0, len(available_chars))))
         black_hole_ring_positions = geometry.find_coords_on_circle(
-            self.terminal.output_area.center,
-            self.blackhole_radius,
-            len(self.blackhole_chars),
+            self._terminal.output_area.center,
+            self._blackhole_radius,
+            len(self._blackhole_chars),
         )
-        for position_index, character in enumerate(self.blackhole_chars):
+        for position_index, character in enumerate(self._blackhole_chars):
             starting_pos = black_hole_ring_positions[position_index]
             blackhole_path = character.motion.new_path(id="blackhole", speed=0.5, ease=easing.in_out_sine)
             blackhole_path.new_waypoint(starting_pos)
             blackhole_scn = character.animation.new_scene(id="blackhole")
-            blackhole_scn.add_frame("✸", 1, color=self.args.blackhole_color)
+            blackhole_scn.add_frame("✸", 1, color=self._config.blackhole_color)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_ACTIVATED,
                 blackhole_path,
                 EventHandler.Action.SET_LAYER,
                 1,
             )
             # make rotation waypoints
             blackhole_rotation_path = character.motion.new_path(id="blackhole_rotation", speed=0.2, loop=True)
             for coord in black_hole_ring_positions[position_index:] + black_hole_ring_positions[:position_index]:
                 blackhole_rotation_path.new_waypoint(coord, id=str(len(blackhole_rotation_path.waypoints)))
-        for character in self.terminal.get_characters():
-            self.terminal.set_character_visibility(character, True)
+        for character in self._terminal.get_characters():
+            self._terminal.set_character_visibility(character, True)
             starting_scn = character.animation.new_scene()
             star_symbol = random.choice(star_symbols)
             star_color = random.choice(starfield_colors)
             starting_scn.add_frame(star_symbol, 1, color=star_color)
             character.animation.activate_scene(starting_scn)
-            if character not in self.blackhole_chars:
-                starfield_coord = self.terminal.output_area.random_coord()
+            if character not in self._blackhole_chars:
+                starfield_coord = self._terminal.output_area.random_coord()
                 character.motion.set_coordinate(starfield_coord)
-                if starfield_coord.row > self.terminal.output_area.center_row:
+                if starfield_coord.row > self._terminal.output_area.center_row:
                     if starfield_coord.column in range(
-                        round(self.terminal.output_area.right * 0.4),
-                        round(self.terminal.output_area.right * 0.7),
+                        round(self._terminal.output_area.right * 0.4),
+                        round(self._terminal.output_area.right * 0.7),
                     ):
                         # if within the top center 40% of the screen
-                        control_point = Coord(self.terminal.output_area.center.column, starfield_coord.row)
+                        control_point = Coord(self._terminal.output_area.center.column, starfield_coord.row)
                     else:
-                        control_point = Coord(starfield_coord.column, self.terminal.output_area.center_row)
+                        control_point = Coord(starfield_coord.column, self._terminal.output_area.center_row)
 
-                elif starfield_coord.row < self.terminal.output_area.center_row:
+                elif starfield_coord.row < self._terminal.output_area.center_row:
                     if starfield_coord.column in range(
-                        round(self.terminal.output_area.right * 0.4),
-                        round(self.terminal.output_area.right * 0.7),
+                        round(self._terminal.output_area.right * 0.4),
+                        round(self._terminal.output_area.right * 0.7),
                     ):
                         # if within the bottom center 40% of the screen
-                        control_point = Coord(self.terminal.output_area.center.column, starfield_coord.row)
+                        control_point = Coord(self._terminal.output_area.center.column, starfield_coord.row)
                     else:
-                        control_point = Coord(starfield_coord.column, self.terminal.output_area.center_row)
+                        control_point = Coord(starfield_coord.column, self._terminal.output_area.center_row)
                 else:
-                    control_point = self.terminal.output_area.center
+                    control_point = self._terminal.output_area.center
                 singularity_path = character.motion.new_path(id="singularity", speed=0.3, ease=easing.in_expo)
-                singularity_path.new_waypoint(self.terminal.output_area.center, bezier_control=control_point)
+                singularity_path.new_waypoint(self._terminal.output_area.center, bezier_control=control_point)
                 consumed_scn = character.animation.new_scene()
                 for color in gradient_map[star_color]:
                     consumed_scn.add_frame(star_symbol, 1, color=color)
                 consumed_scn.add_frame(" ", 1)
                 consumed_scn.sync = animation.SyncMetric.DISTANCE
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_ACTIVATED,
@@ -181,47 +201,47 @@
                 )
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_ACTIVATED,
                     singularity_path,
                     EventHandler.Action.ACTIVATE_SCENE,
                     consumed_scn,
                 )
-                self.awaiting_consumption_chars.append(character)
-        random.shuffle(self.awaiting_consumption_chars)
+                self._awaiting_consumption_chars.append(character)
+        random.shuffle(self._awaiting_consumption_chars)
 
-    def rotate_blackhole(self) -> None:
-        for character in self.blackhole_chars:
+    def _rotate_blackhole(self) -> None:
+        for character in self._blackhole_chars:
             character.motion.activate_path(character.motion.query_path("blackhole_rotation"))
-            self.active_chars.append(character)
+            self._active_chars.append(character)
 
-    def collapse_blackhole(self) -> None:
+    def _collapse_blackhole(self) -> None:
         black_hole_ring_positions = geometry.find_coords_on_circle(
-            self.terminal.output_area.center,
-            self.blackhole_radius + 3,
-            len(self.blackhole_chars),
+            self._terminal.output_area.center,
+            self._blackhole_radius + 3,
+            len(self._blackhole_chars),
         )
         unstable_symbols = ["◦", "◎", "◉", "●", "◉", "◎", "◦"]
         point_char_made = False
-        for character in self.blackhole_chars:
+        for character in self._blackhole_chars:
             next_pos = black_hole_ring_positions.pop(0)
             expand_path = character.motion.new_path(speed=0.1, ease=easing.in_expo)
             expand_path.new_waypoint(next_pos)
             collapse_path = character.motion.new_path(speed=0.3, ease=easing.in_expo)
-            collapse_path.new_waypoint(self.terminal.output_area.center)
+            collapse_path.new_waypoint(self._terminal.output_area.center)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_COMPLETE,
                 expand_path,
                 EventHandler.Action.ACTIVATE_PATH,
                 collapse_path,
             )
             if not point_char_made:
                 point_scn = character.animation.new_scene()
                 for _ in range(3):
                     for symbol in unstable_symbols:
-                        point_scn.add_frame(symbol, 6, color=random.choice(self.args.star_colors))
+                        point_scn.add_frame(symbol, 6, color=random.choice(self._config.star_colors))
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_COMPLETE,
                     collapse_path,
                     EventHandler.Action.ACTIVATE_SCENE,
                     point_scn,
                 )
                 character.event_handler.register_event(
@@ -229,30 +249,30 @@
                     collapse_path,
                     EventHandler.Action.SET_LAYER,
                     3,
                 )
                 point_char_made = True
 
             character.motion.activate_path(expand_path)
-            self.active_chars.append(character)
+            self._active_chars.append(character)
 
-    def explode_singularity(self) -> None:
+    def _explode_singularity(self) -> None:
         star_colors = ["ffcc0d", "ff7326", "ff194d", "bf2669", "702a8c" "049dbf"]
-        for character in self.terminal.get_characters():
+        for character in self._terminal.get_characters():
             nearby_coord = geometry.find_coords_on_circle(character.input_coord, 3, 5)[random.randrange(0, 5)]
             nearby_path = character.motion.new_path(speed=random.randint(2, 3) / 10, ease=easing.out_expo)
             nearby_path.new_waypoint(nearby_coord)
             input_path = character.motion.new_path(speed=random.randint(3, 5) / 100, ease=easing.in_cubic)
             input_path.new_waypoint(character.input_coord)
             explode_scn = character.animation.new_scene()
             explode_star_color = random.choice(star_colors)
             explode_scn.add_frame(character.input_symbol, 1, color=explode_star_color)
             cooling_scn = character.animation.new_scene()
             cooling_gradient = graphics.Gradient(
-                explode_star_color, self.character_final_color_map[character], steps=10
+                explode_star_color, self._character_final_color_map[character], steps=10
             )
             cooling_scn.apply_gradient_to_symbols(cooling_gradient, character.input_symbol, 20)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_COMPLETE,
                 nearby_path,
                 EventHandler.Action.ACTIVATE_PATH,
                 input_path,
@@ -261,84 +281,93 @@
                 EventHandler.Event.PATH_COMPLETE,
                 nearby_path,
                 EventHandler.Action.ACTIVATE_SCENE,
                 cooling_scn,
             )
             character.animation.activate_scene(explode_scn)
             character.motion.activate_path(nearby_path)
-            self.active_chars.append(character)
+            self._active_chars.append(character)
 
-    def prepare_data(self) -> None:
+    def _build(self) -> None:
         """Prepares the data for the effect by creating the starfield, blackhole, and consumption scenes/waypoints."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        self.prepare_blackhole()
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        self._prepare_blackhole()
+        self.formation_delay = max(100 // len(self._blackhole_chars), 10)
+        self.f_delay = self.formation_delay
+        self.next_char_consuming_delay = 0
+        self.max_consume = max(min(int(0.1 * len(self._terminal._input_characters)), 15), 2)
+        self.phase = "forming"
+        self.awaiting_blackhole_chars = list(self._blackhole_chars)
 
-    def run(self) -> None:
+    def __next__(self) -> str:
         """Runs the effect."""
-        self.prepare_data()
-        formation_delay = max(100 // len(self.blackhole_chars), 10)
-        f_delay = formation_delay
-        next_char_consuming_delay = 0
-        max_consume = max(min(int(0.1 * len(self.terminal._input_characters)), 15), 2)
-        phase = "forming"
-        awaiting_blackhole_chars = list(self.blackhole_chars)
-        while self.active_chars or phase != "complete":
-            if phase == "forming":
-                if awaiting_blackhole_chars:
-                    if not f_delay:
-                        next_char = awaiting_blackhole_chars.pop(0)
+        if self._active_chars or self.phase != "complete":
+            if self.phase == "forming":
+                if self.awaiting_blackhole_chars:
+                    if not self.f_delay:
+                        next_char = self.awaiting_blackhole_chars.pop(0)
                         next_char.motion.activate_path(next_char.motion.query_path("blackhole"))
                         next_char.animation.activate_scene(next_char.animation.query_scene("blackhole"))
-                        self.active_chars.append(next_char)
-                        f_delay = formation_delay
+                        self._active_chars.append(next_char)
+                        self.f_delay = self.formation_delay
                     else:
-                        f_delay -= 1
+                        self.f_delay -= 1
                 else:
-                    if not self.active_chars:
-                        self.rotate_blackhole()
-                        phase = "consuming"
-            elif phase == "consuming":
-                if self.awaiting_consumption_chars:
-                    if not next_char_consuming_delay:
-                        for _ in range(random.randrange(1, max_consume)):
-                            if self.awaiting_consumption_chars:
-                                next_char = self.awaiting_consumption_chars.pop(0)
+                    if not self._active_chars:
+                        self._rotate_blackhole()
+                        self.phase = "consuming"
+            elif self.phase == "consuming":
+                if self._awaiting_consumption_chars:
+                    if not self.next_char_consuming_delay:
+                        for _ in range(random.randrange(1, self.max_consume)):
+                            if self._awaiting_consumption_chars:
+                                next_char = self._awaiting_consumption_chars.pop(0)
                                 next_char.motion.activate_path(next_char.motion.query_path("singularity"))
-                                self.active_chars.append(next_char)
+                                self._active_chars.append(next_char)
                             else:
                                 break
-                        max_consume += 1
-                        next_char_consuming_delay = random.randrange(0, 10)
+                        self.max_consume += 1
+                        self.next_char_consuming_delay = random.randrange(0, 10)
                     else:
-                        next_char_consuming_delay -= 1
+                        self.next_char_consuming_delay -= 1
 
                 else:
-                    if all(character in self.blackhole_chars for character in self.active_chars):
-                        phase = "collapsing"
+                    if all(character in self._blackhole_chars for character in self._active_chars):
+                        self.phase = "collapsing"
 
-            elif phase == "collapsing":
-                self.collapse_blackhole()
-                phase = "exploding"
-            elif phase == "exploding":
+            elif self.phase == "collapsing":
+                self._collapse_blackhole()
+                self.phase = "exploding"
+            elif self.phase == "exploding":
                 if all(
                     [
                         character.motion.active_path is None and character.animation.active_scene is None
-                        for character in self.blackhole_chars
+                        for character in self._blackhole_chars
                     ]
                 ):
-                    self.explode_singularity()
-                    phase = "complete"
+                    self._explode_singularity()
+                    self.phase = "complete"
+
+            for character in self._active_chars:
+                character.tick()
+            next_frame = self._terminal.get_formatted_output_string()
 
-            self.animate_chars()
-            self.terminal.print()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return next_frame
+
+        else:
+            raise StopIteration
+
+
+class Blackhole(BaseEffect[BlackholeConfig]):
+    """Effect that creates a blackhole in a starfield, consumes the stars, and explodes the input characters out to position."""
 
-            self.active_chars = [character for character in self.active_chars if character.is_active]
+    _config_cls = BlackholeConfig
+    _iterator_cls = BlackholeIterator
 
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method."""
-        for character in self.active_chars:
-            character.tick()
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_bouncyballs.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_expand.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,166 +1,158 @@
-import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
-from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return BouncyBallsEffect, BouncyBallsEffectArgs
+    return Expand, ExpandConfig
 
 
 @argclass(
-    name="bouncyballs",
-    formatter_class=arg_validators.CustomFormatter,
-    help="Characters are bouncy balls falling from the top of the output area.",
-    description="bouncyballs | Characters are bouncy balls falling from the top of the output area.",
+    name="expand",
+    help="Expands the text from a single point.",
+    description="expand | Expands the text from a single point.",
     epilog=f"""{arg_validators.EASING_EPILOG}
-Example: terminaltexteffects bouncyballs --ball-colors d1f4a5 96e2a4 5acda9 --ball-symbols o "*" O 0 . --final-gradient-stops f8ffae 43c6ac --final-gradient-steps 12 --final-gradient-direction diagonal --ball-delay 7 --movement-speed 0.25 --easing OUT_BOUNCE""",
+    
+Example: terminaltexteffects expand --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-frames 5 --movement-speed 0.35 --expand-easing IN_OUT_QUART""",
 )
 @dataclass
-class BouncyBallsEffectArgs(ArgsDataClass):
-    ball_colors: tuple[graphics.Color, ...] = ArgField(
-        cmd_name=["--ball-colors"],
-        type_parser=arg_validators.Color.type_parser,
-        metavar=arg_validators.Color.METAVAR,
-        nargs="+",
-        default=("d1f4a5", "96e2a4", "5acda9"),
-        help="Space separated list of colors from which ball colors will be randomly selected. If no colors are provided, the colors are random.",
-    )  # type: ignore[assignment]
-    ball_symbols: tuple[str, ...] = ArgField(
-        cmd_name="--ball-symbols",
-        type_parser=arg_validators.Symbol.type_parser,
-        nargs="+",
-        default=("*", "o", "O", "0", "."),
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Space separated list of symbols to use for the balls.",
-    )  # type: ignore[assignment]
+class ExpandConfig(ArgsDataClass):
+    """Configuration for the Expand effect.
+
+    Attributes:
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_frames (int): Number of frames to display each gradient step.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        movement_speed (float): Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
+        expand_easing (typing.Callable): Easing function to use for character movement."""
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
-        default=("f8ffae", "43c6ac"),
+        default=("8A008A", "00D1FF", "FFFFFF"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name=["--final-gradient-steps"],
+        cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
+    final_gradient_frames: int = ArgField(
+        cmd_name="--final-gradient-frames",
+        type_parser=arg_validators.PositiveInt.type_parser,
+        default=5,
+        metavar=arg_validators.PositiveInt.METAVAR,
+        help="Number of frames to display each gradient step.",
+    )  # type: ignore[assignment]
+    "int : Number of frames to display each gradient step."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
-        default=graphics.Gradient.Direction.DIAGONAL,
+        default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
-    ball_delay: int = ArgField(
-        cmd_name="--ball-delay",
-        type_parser=arg_validators.NonNegativeInt.type_parser,
-        default=7,
-        metavar=arg_validators.NonNegativeInt.METAVAR,
-        help="Number of animation steps between ball drops, increase to reduce ball drop rate.",
-    )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
         type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.25,
+        default=0.35,
         metavar=arg_validators.PositiveFloat.METAVAR,
         help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
     )  # type: ignore[assignment]
-    easing: typing.Callable = ArgField(
-        cmd_name="--easing",
+    "float : Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+
+    expand_easing: easing.EasingFunction = ArgField(
+        cmd_name="--expand-easing",
+        default=easing.in_out_quart,
         type_parser=arg_validators.Ease.type_parser,
-        default=easing.out_bounce,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
-        return BouncyBallsEffect
+        return Expand
+
 
+class ExpandIterator(BaseEffectIterator[ExpandConfig]):
+    """Effect that draws the characters expanding from a single point."""
 
-class BouncyBallsEffect:
-    """Effect that displays the text as bouncy balls falling from the top of the output area."""
+    def __init__(
+        self,
+        effect: "Expand",
+    ):
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
 
-    def __init__(self, terminal: Terminal, args: BouncyBallsEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.group_by_row: dict[int, list[EffectCharacter | None]] = {}
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by assigning colors and waypoints and
-        organizing the characters by row."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        """Prepares the data for the effect by starting all of the characters from a point in the middle of the input data."""
+
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-            color = random.choice(self.args.ball_colors)
-            symbol = random.choice(self.args.ball_symbols)
-            ball_scene = character.animation.new_scene()
-            ball_scene.add_frame(symbol, 1, color=color)
-            final_scene = character.animation.new_scene()
-            char_final_gradient = graphics.Gradient(color, self.character_final_color_map[character], steps=10)
-            final_scene.apply_gradient_to_symbols(char_final_gradient, character.input_symbol, 10)
-            character.motion.set_coordinate(
-                Coord(character.input_coord.column, int(self.terminal.output_area.top * random.uniform(1.0, 1.5)))
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self._terminal.get_characters():
+            character.motion.set_coordinate(self._terminal.output_area.center)
+            input_coord_path = character.motion.new_path(
+                speed=self._config.movement_speed,
+                ease=self._config.expand_easing,
             )
-            input_coord_path = character.motion.new_path(speed=self.args.movement_speed, ease=self.args.easing)
             input_coord_path.new_waypoint(character.input_coord)
-            character.motion.activate_path(input_coord_path)
-            character.animation.activate_scene(ball_scene)
+            self._terminal.set_character_visibility(character, True)
+            self._active_chars.append(character)
+            character.event_handler.register_event(
+                EventHandler.Event.PATH_ACTIVATED, input_coord_path, EventHandler.Action.SET_LAYER, 1
+            )
             character.event_handler.register_event(
-                character.event_handler.Event.PATH_COMPLETE,
-                input_coord_path,
-                character.event_handler.Action.ACTIVATE_SCENE,
-                final_scene,
+                EventHandler.Event.PATH_COMPLETE, input_coord_path, EventHandler.Action.SET_LAYER, 0
+            )
+            character.motion.activate_path(input_coord_path)
+            gradient_scn = character.animation.new_scene()
+            gradient = graphics.Gradient(
+                final_gradient.spectrum[0], self._character_final_color_map[character], steps=10
             )
-            self.pending_chars.append(character)
-        for character in sorted(self.pending_chars, key=lambda c: c.input_coord.row):
-            if character.input_coord.row not in self.group_by_row:
-                self.group_by_row[character.input_coord.row] = []
-            self.group_by_row[character.input_coord.row].append(character)
+            gradient_scn.apply_gradient_to_symbols(gradient, character.input_symbol, self._config.final_gradient_frames)
+            character.animation.activate_scene(gradient_scn)
 
-    def run(self) -> None:
+    def __next__(self) -> str:
         """Runs the effect."""
-        self.prepare_data()
-        self.pending_chars.clear()
-        ball_delay = 0
-        while self.group_by_row or self.active_chars or self.pending_chars:
-            if not self.pending_chars and self.group_by_row:
-                self.pending_chars.extend(self.group_by_row.pop(min(self.group_by_row.keys())))  # type: ignore
-            if self.pending_chars:
-                if ball_delay == 0:
-                    for _ in range(random.randint(2, 6)):
-                        if self.pending_chars:
-                            next_character = self.pending_chars.pop(random.randint(0, len(self.pending_chars) - 1))
-                            self.terminal.set_character_visibility(next_character, True)
-                            self.active_chars.append(next_character)
-                        else:
-                            break
-                    ball_delay = self.args.ball_delay
-                else:
-                    ball_delay -= 1
-
-            self.animate_chars()
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-            self.terminal.print()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method."""
-        for character in self.active_chars:
-            character.tick()
+        if self._active_chars:
+            for character in self._active_chars:
+                character.tick()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class Expand(BaseEffect[ExpandConfig]):
+    """Effect that draws the characters expanding from a single point."""
+
+    _config_cls = ExpandConfig
+    _iterator_cls = ExpandIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_bubbles.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_bubbles.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,243 +1,278 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return BubblesEffect, BubblesEffectArgs
+    return Bubbles, BubblesConfig
 
 
 @argclass(
     name="bubbles",
-    formatter_class=arg_validators.CustomFormatter,
     help="Characters are formed into bubbles that float down and pop.",
     description="bubbles | Characters are formed into bubbles that float down and pop.",
     epilog=f"""{arg_validators.EASING_EPILOG}
 
 Example: terminaltexteffects bubbles --bubble-colors d33aff 7395c4 43c2a7 02ff7f --pop-color ffffff --final-gradient-stops d33aff 02ff7f --final-gradient-steps 12 --final-gradient-direction diagonal --bubble-speed 0.1 --bubble-delay 50 --pop-condition row --easing IN_OUT_SINE""",
 )
 @dataclass
-class BubblesEffectArgs(ArgsDataClass):
+class BubblesConfig(ArgsDataClass):
+    """Configuration for the Bubbles effect.
+
+    Attributes:
+        rainbow (bool): If set, the bubbles will be colored with a rotating rainbow gradient.
+        bubble_colors (tuple[graphics.Color, ...]): Tuple of colors for the bubbles. Ignored if --no-rainbow is left as default False.
+        pop_color (graphics.Color): Color for the spray emitted when a bubble pops.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        bubble_speed (float): Speed of the floating bubbles. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
+        bubble_delay (int): Number of animation steps between bubbles.
+        pop_condition (str): Condition for a bubble to pop. 'row' will pop the bubble when it reaches the the lowest row for which a character in the bubble originates. 'bottom' will pop the bubble at the bottom row of the terminal. 'anywhere' will pop the bubble randomly, or at the bottom of the terminal.
+        easing (typing.Callable): Easing function to use for character movement after a bubble pops.
+    """
+
     rainbow: bool = ArgField(
         cmd_name="--rainbow",
         action="store_true",
         default=False,
         help="If set, the bubbles will be colored with a rotating rainbow gradient.",
     )  # type: ignore[assignment]
+    "bool : If set, the bubbles will be colored with a rotating rainbow gradient."
+
     bubble_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--bubble-colors",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("d33aff", "7395c4", "43c2a7", "02ff7f"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the bubbles. Ignored if --no-rainbow is left as default False.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the bubbles. Ignored if --no-rainbow is left as default False."
+
     pop_color: graphics.Color = ArgField(
         cmd_name="--pop-color",
         type_parser=arg_validators.Color.type_parser,
         default="ffffff",
         metavar=arg_validators.Color.METAVAR,
         help="Color for the spray emitted when a bubble pops.",
     )  # type: ignore[assignment]
+    "graphics.Color : Color for the spray emitted when a bubble pops."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("d33aff", "02ff7f"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     bubble_speed: float = ArgField(
         cmd_name="--bubble-speed",
         type_parser=arg_validators.PositiveFloat.type_parser,
         default=0.1,
         metavar=arg_validators.PositiveFloat.METAVAR,
         help="Speed of the floating bubbles. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
     )  # type: ignore[assignment]
+    "float : Speed of the floating bubbles. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+
     bubble_delay: int = ArgField(
         cmd_name="--bubble-delay",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=50,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Number of animation steps between bubbles.",
     )  # type: ignore[assignment]
+    "int : Number of animation steps between bubbles."
+
     pop_condition: str = ArgField(
         cmd_name="--pop-condition",
         default="row",
         choices=["row", "bottom", "anywhere"],
         help="Condition for a bubble to pop. 'row' will pop the bubble when it reaches the the lowest row for which a character in the bubble originates. 'bottom' will pop the bubble at the bottom row of the terminal. 'anywhere' will pop the bubble randomly, or at the bottom of the terminal.",
     )  # type: ignore[assignment]
-    easing: typing.Callable = ArgField(
-        cmd_name=["--easing"],
+    "str : Condition for a bubble to pop. 'row' will pop the bubble when it reaches the the lowest row for which a character in the bubble originates. 'bottom' will pop the bubble at the bottom row of the terminal. 'anywhere' will pop the bubble randomly, or at the bottom of the terminal."
+
+    movement_easing: easing.EasingFunction = ArgField(
+        cmd_name=["--movement-easing"],
         default=easing.in_out_sine,
         type_parser=arg_validators.Ease.type_parser,
         metavar=arg_validators.Ease.METAVAR,
         help="Easing function to use for character movement after a bubble pops.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for character movement after a bubble pops."
 
     @classmethod
     def get_effect_class(cls):
-        return BubblesEffect
+        return Bubbles
 
 
-class Bubble:
-    def __init__(
-        self,
-        effect: "BubblesEffect",
-        origin: Coord,
-        characters: list[EffectCharacter],
-        terminal: Terminal,
-    ):
-        self.effect = effect
-        self.characters = characters
-        self.terminal = terminal
-        self.radius = max(len(self.characters) // 5, 1)
-        self.origin = origin
-        self.anchor_char = self.terminal.add_character(" ", self.origin)
-        if self.effect.args.pop_condition == "row":
-            self.lowest_row = min([char.input_coord.row for char in self.characters])
-        else:
-            self.lowest_row = self.effect.terminal.output_area.bottom
-        self.set_character_coordinates()
-        self.landed = False
-        self.make_waypoints()
-        self.make_gradients()
-
-    def set_character_coordinates(self) -> None:
-        for i, char in enumerate(self.characters):
-            point = geometry.find_coords_on_circle(
-                self.anchor_char.motion.current_coord, self.radius, len(self.characters), unique=False
-            )[i]
-            char.motion.set_coordinate(point)
-            if point.row == self.lowest_row:
-                self.landed = True
-
-        if self.effect.args.pop_condition == "anywhere":
-            if random.random() < 0.002:
-                self.landed = True
-
-    def make_waypoints(self):
-        waypoint_column = random.randint(self.effect.terminal.output_area.left, self.effect.terminal.output_area.right)
-        floor_path = self.anchor_char.motion.new_path(speed=self.effect.args.bubble_speed)
-        floor_path.new_waypoint(Coord(waypoint_column, self.lowest_row))
-        self.anchor_char.motion.activate_path(floor_path)
-
-    def make_gradients(self) -> None:
-        if self.effect.args.rainbow:
-            rainbow_gradient = list(self.effect.rainbow_gradient.spectrum)
-            gradient_offset = 0
-            for character in self.characters:
-                sheen_scene = character.animation.new_scene()
-                for step in rainbow_gradient:
-                    sheen_scene.add_frame(character.input_symbol, 5, color=step)
-                gradient_offset += 2
-                gradient_offset %= len(rainbow_gradient)
-                rainbow_gradient = rainbow_gradient[gradient_offset:] + rainbow_gradient[:gradient_offset]
-                character.animation.activate_scene(sheen_scene)
-                if character.animation.active_scene:
-                    character.animation.active_scene.is_looping = True
+class BubblesIterator(BaseEffectIterator[BubblesConfig]):
+    """Effect that forms circles with the characters. Circles float down and pop into the characters."""
 
-        else:
-            bubble_color = random.choice(self.effect.args.bubble_colors)
-            for character in self.characters:
-                sheen_scene = character.animation.new_scene()
-                sheen_scene.add_frame(character.input_symbol, 1, color=bubble_color)
-                character.animation.activate_scene(sheen_scene)
-
-    def pop(self) -> None:
-        char: EffectCharacter
-        point: Coord
-        for char, point in zip(
-            self.characters,
-            geometry.find_coords_on_circle(
-                self.anchor_char.motion.current_coord,
-                self.radius + 3,
-                len(self.characters),
-            ),
+    class _Bubble:
+        def __init__(
+            self,
+            effect: "BubblesIterator",
+            origin: Coord,
+            characters: list[EffectCharacter],
+            terminal: Terminal,
         ):
-            pop_out_path = char.motion.new_path(id="pop_out", speed=0.2, ease=easing.out_expo)
-            pop_out_path.new_waypoint(point)
-            char.event_handler.register_event(
-                EventHandler.Event.PATH_COMPLETE,
-                pop_out_path,
-                EventHandler.Action.ACTIVATE_PATH,
-                char.motion.paths["final"],
+            self.effect = effect
+            self.characters = characters
+            self.terminal = terminal
+            self.radius = max(len(self.characters) // 5, 1)
+            self.origin = origin
+            self.anchor_char = self.terminal.add_character(" ", self.origin)
+            if self.effect._config.pop_condition == "row":
+                self.lowest_row = min([char.input_coord.row for char in self.characters])
+            else:
+                self.lowest_row = self.effect._terminal.output_area.bottom
+            self.set_character_coordinates()
+            self.landed = False
+            self.make_waypoints()
+            self.make_gradients()
+
+        def set_character_coordinates(self) -> None:
+            for i, char in enumerate(self.characters):
+                point = geometry.find_coords_on_circle(
+                    self.anchor_char.motion.current_coord, self.radius, len(self.characters), unique=False
+                )[i]
+                char.motion.set_coordinate(point)
+                if point.row == self.lowest_row:
+                    self.landed = True
+
+            if self.effect._config.pop_condition == "anywhere":
+                if random.random() < 0.002:
+                    self.landed = True
+
+        def make_waypoints(self):
+            waypoint_column = random.randint(
+                self.effect._terminal.output_area.left, self.effect._terminal.output_area.right
             )
-        for character in self.characters:
-            character.animation.activate_scene(character.animation.query_scene("pop_1"))
-            character.motion.activate_path(character.motion.query_path("pop_out"))
-
-    def activate(self) -> None:
-        for char in self.characters:
-            self.terminal.set_character_visibility(char, True)
-
-    def move(self) -> None:
-        self.anchor_char.motion.move()
-        self.set_character_coordinates()
-        for character in self.characters:
-            character.animation.step_animation()
+            floor_path = self.anchor_char.motion.new_path(speed=self.effect._config.bubble_speed)
+            floor_path.new_waypoint(Coord(waypoint_column, self.lowest_row))
+            self.anchor_char.motion.activate_path(floor_path)
+
+        def make_gradients(self) -> None:
+            if self.effect._config.rainbow:
+                rainbow_gradient = list(self.effect.rainbow_gradient.spectrum)
+                gradient_offset = 0
+                for character in self.characters:
+                    sheen_scene = character.animation.new_scene()
+                    for step in rainbow_gradient:
+                        sheen_scene.add_frame(character.input_symbol, 5, color=step)
+                    gradient_offset += 2
+                    gradient_offset %= len(rainbow_gradient)
+                    rainbow_gradient = rainbow_gradient[gradient_offset:] + rainbow_gradient[:gradient_offset]
+                    character.animation.activate_scene(sheen_scene)
+                    if character.animation.active_scene:
+                        character.animation.active_scene.is_looping = True
 
+            else:
+                bubble_color = random.choice(self.effect._config.bubble_colors)
+                for character in self.characters:
+                    sheen_scene = character.animation.new_scene()
+                    sheen_scene.add_frame(character.input_symbol, 1, color=bubble_color)
+                    character.animation.activate_scene(sheen_scene)
+
+        def pop(self) -> None:
+            char: EffectCharacter
+            point: Coord
+            for char, point in zip(
+                self.characters,
+                geometry.find_coords_on_circle(
+                    self.anchor_char.motion.current_coord,
+                    self.radius + 3,
+                    len(self.characters),
+                ),
+            ):
+                pop_out_path = char.motion.new_path(id="pop_out", speed=0.2, ease=easing.out_expo)
+                pop_out_path.new_waypoint(point)
+                char.event_handler.register_event(
+                    EventHandler.Event.PATH_COMPLETE,
+                    pop_out_path,
+                    EventHandler.Action.ACTIVATE_PATH,
+                    char.motion.paths["final"],
+                )
+            for character in self.characters:
+                character.animation.activate_scene(character.animation.query_scene("pop_1"))
+                character.motion.activate_path(character.motion.query_path("pop_out"))
 
-class BubblesEffect:
-    """Effect that forms circles with the characters. Circles float down and pop into the characters."""
+        def activate(self) -> None:
+            for char in self.characters:
+                self.terminal.set_character_visibility(char, True)
+
+        def move(self) -> None:
+            self.anchor_char.motion.move()
+            self.set_character_coordinates()
+            for character in self.characters:
+                character.animation.step_animation()
 
-    def __init__(self, terminal: Terminal, args: BubblesEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.bubbles: list[Bubble] = []
+    def __init__(self, effect: "Bubbles"):
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._bubbles: list[BubblesIterator._Bubble] = []
         red = "e81416"
         orange = "ffa500"
         yellow = "faeb36"
         green = "79c314"
         blue = "487de7"
         indigo = "4b369d"
         violet = "70369d"
         self.rainbow_gradient = graphics.Gradient(red, orange, yellow, green, blue, indigo, violet, steps=5)
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
 
-    def prepare_data(self) -> None:
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
             character.layer = 1
             pop_1_scene = character.animation.new_scene(id="pop_1")
             pop_2_scene = character.animation.new_scene()
-            pop_1_scene.add_frame("*", 20, color=self.args.pop_color)
-            pop_2_scene.add_frame("'", 20, color=self.args.pop_color)
+            pop_1_scene.add_frame("*", 20, color=self._config.pop_color)
+            pop_2_scene.add_frame("'", 20, color=self._config.pop_color)
             final_scene = character.animation.new_scene()
             char_final_gradient = graphics.Gradient(
-                self.args.pop_color, self.character_final_color_map[character], steps=10
+                self._config.pop_color, self._character_final_color_map[character], steps=10
             )
             final_scene.apply_gradient_to_symbols(char_final_gradient, character.input_symbol, 10)
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE, pop_1_scene, EventHandler.Action.ACTIVATE_SCENE, pop_2_scene
             )
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE,
@@ -252,58 +287,64 @@
             )
             final_path.new_waypoint(character.input_coord)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_COMPLETE, final_path, EventHandler.Action.SET_LAYER, 0
             )
 
         unbubbled_chars = []
-        for char_list in self.terminal.get_characters_grouped(grouping=self.terminal.CharacterGroup.ROW_BOTTOM_TO_TOP):
+        for char_list in self._terminal.get_characters_grouped(
+            grouping=self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP
+        ):
             unbubbled_chars.extend(char_list)
-        self.bubbles = []
+        self._bubbles = []
         while unbubbled_chars:
             bubble_group = []
             if len(unbubbled_chars) < 5:
                 bubble_group.extend(unbubbled_chars)
                 unbubbled_chars.clear()
             else:
                 for _ in range(random.randint(5, min(len(unbubbled_chars), 20))):
                     bubble_group.append(unbubbled_chars.pop(0))
             bubble_origin = Coord(
-                random.randint(self.terminal.output_area.left, self.terminal.output_area.right),
-                self.terminal.output_area.top,
+                random.randint(self._terminal.output_area.left, self._terminal.output_area.right),
+                self._terminal.output_area.top,
             )
-            new_bubble = Bubble(self, bubble_origin, bubble_group, self.terminal)
-            self.bubbles.append(new_bubble)
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        animating_bubbles: list[Bubble] = []
-        steps_since_last_bubble = 0
-        while animating_bubbles or self.active_chars or self.bubbles:
-            if self.bubbles and steps_since_last_bubble >= self.args.bubble_delay:
-                next_bubble = self.bubbles.pop(0)
+            new_bubble = BubblesIterator._Bubble(self, bubble_origin, bubble_group, self._terminal)
+            self._bubbles.append(new_bubble)
+        self.animating_bubbles: list[BubblesIterator._Bubble] = []
+        self.steps_since_last_bubble = 0
+
+    def __next__(self) -> str:
+        if self.animating_bubbles or self._active_chars or self._bubbles:
+            if self._bubbles and self.steps_since_last_bubble >= self._config.bubble_delay:
+                next_bubble = self._bubbles.pop(0)
                 next_bubble.activate()
-                animating_bubbles.append(next_bubble)
-                steps_since_last_bubble = 0
-            steps_since_last_bubble += 1
+                self.animating_bubbles.append(next_bubble)
+                self.steps_since_last_bubble = 0
+            self.steps_since_last_bubble += 1
 
-            for bubble in animating_bubbles:
+            for bubble in self.animating_bubbles:
                 if bubble.landed:
                     bubble.pop()
-                    self.active_chars.extend(bubble.characters)
+                    self._active_chars.extend(bubble.characters)
+
+            self.animating_bubbles = [bubble for bubble in self.animating_bubbles if not bubble.landed]
+            for bubble in self.animating_bubbles:
+                bubble.move()
+            for character in self._active_chars:
+                character.tick()
+            next_frame = self._terminal.get_formatted_output_string()
+
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return next_frame
+        else:
+            raise StopIteration
+
+
+class Bubbles(BaseEffect[BubblesConfig]):
+    """Effect that forms circles with the characters. Circles float down and pop into the characters."""
+
+    _config_cls = BubblesConfig
+    _iterator_cls = BubblesIterator
 
-            animating_bubbles = [bubble for bubble in animating_bubbles if not bubble.landed]
-            self.animate_bubbles(animating_bubbles)
-            self.animate_chars()
-            self.terminal.print()
-
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-
-    def animate_bubbles(self, animating_bubbles: list[Bubble]) -> None:
-        for bubble in animating_bubbles:
-            bubble.move()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method."""
-        for character in self.active_chars:
-            character.tick()
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_burn.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_burn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,146 +1,169 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return BurnEffect, BurnEffectArgs
+    return Burn, BurnConfig
 
 
 @argclass(
     name="burn",
-    formatter_class=arg_validators.CustomFormatter,
     help="Burns vertically in the output area.",
     description="burn | Burn the output area.",
     epilog="Example: terminaltexteffects burn --starting-color 837373 --burn-colors ffffff fff75d fe650d 8a003c 510100 --final-gradient-stops 00c3ff ffff1c --final-gradient-steps 12",
 )
 @dataclass
-class BurnEffectArgs(ArgsDataClass):
+class BurnConfig(ArgsDataClass):
+    """Configuration for the Burn effect.
+
+    Attributes:
+        starting_color (graphics.Color): Color of the characters before they start to burn.
+        burn_colors (tuple[graphics.Color, ...]): Colors transitioned through as the characters burn.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color."""
+
     starting_color: graphics.Color = ArgField(
         cmd_name="--starting-color",
         type_parser=arg_validators.Color.type_parser,
         default="837373",
         metavar=arg_validators.Color.METAVAR,
         help="Color of the characters before they start to burn.",
     )  # type: ignore[assignment]
+    "graphics.Color : Color of the characters before they start to burn."
+
     burn_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--burn-colors"],
         type_parser=arg_validators.Color.type_parser,
         default=("ffffff", "fff75d", "fe650d", "8A003C", "510100"),
         nargs="+",
         metavar=arg_validators.Color.METAVAR,
         help="Colors transitioned through as the characters burn.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Colors transitioned through as the characters burn."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("00c3ff", "ffff1c"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
 
     @classmethod
     def get_effect_class(cls):
-        return BurnEffect
+        return Burn
 
 
-class BurnEffect:
+class BurnIterator(BaseEffectIterator[BurnConfig]):
     """Effect that burns up the screen."""
 
-    def __init__(self, terminal: Terminal, args: BurnEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+    def __init__(self, effect: "Burn"):
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
 
-    def prepare_data(self) -> None:
+    def _build(self) -> None:
         """Prepares the data for the effect by building the burn animation and organizing the data into columns."""
         vertical_build_order = [
             "'",
             ".",
             "▖",
             "▙",
             "█",
             "▜",
             "▀",
             "▝",
             ".",
         ]
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        fire_gradient = graphics.Gradient(*self.args.burn_colors, steps=10)
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        fire_gradient = graphics.Gradient(*self._config.burn_colors, steps=10)
         groups = {
             column_index: column
             for column_index, column in enumerate(
-                self.terminal.get_characters_grouped(grouping=self.terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT)
+                self._terminal.get_characters_grouped(grouping=self._terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT)
             )
         }
 
         def groups_remaining(rows) -> bool:
             return any(row for row in rows.values())
 
         while groups_remaining(groups):
             keys = [key for key in groups.keys() if groups[key]]
             next_char = groups[random.choice(keys)].pop(0)
-            self.terminal.set_character_visibility(next_char, True)
-            next_char.animation.set_appearance(next_char.input_symbol, color=self.args.starting_color)
+            self._terminal.set_character_visibility(next_char, True)
+            next_char.animation.set_appearance(next_char.input_symbol, color=self._config.starting_color)
             burn_scn = next_char.animation.new_scene(id="burn")
             burn_scn.apply_gradient_to_symbols(fire_gradient, vertical_build_order, 12)
             final_color_scn = next_char.animation.new_scene()
             for color in graphics.Gradient(
-                fire_gradient.spectrum[-1], self.character_final_color_map[next_char], steps=8
+                fire_gradient.spectrum[-1], self._character_final_color_map[next_char], steps=8
             ):
                 final_color_scn.add_frame(next_char.input_symbol, 4, color=color)
             next_char.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE, burn_scn, EventHandler.Action.ACTIVATE_SCENE, final_color_scn
             )
 
-            self.pending_chars.append(next_char)
+            self._pending_chars.append(next_char)
 
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        while self.pending_chars or self.active_chars:
+    def __next__(self) -> str:
+        if self._pending_chars or self._active_chars:
             for _ in range(random.randint(2, 4)):
-                if self.pending_chars:
-                    next_char = self.pending_chars.pop(0)
+                if self._pending_chars:
+                    next_char = self._pending_chars.pop(0)
                     next_char.animation.activate_scene(next_char.animation.query_scene("burn"))
                     # self.terminal.set_character_visibility(next_char, True)
-                    self.active_chars.append(next_char)
+                    self._active_chars.append(next_char)
+
+            for character in self._active_chars:
+                character.animation.step_animation()
+
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
 
-            self.animate_chars()
 
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-            self.terminal.print()
+class Burn(BaseEffect[BurnConfig]):
+    """Effect that burns up the screen."""
+
+    _config_cls = BurnConfig
+    _iterator_cls = BurnIterator
 
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method."""
-        for character in self.active_chars:
-            character.animation.step_animation()
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_crumble.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_crumble.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,101 +1,112 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import animation, easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return CrumbleEffect, CrumbleEffectArgs
+    return Crumble, CrumbleConfig
 
 
 @argclass(
     name="crumble",
-    formatter_class=arg_validators.CustomFormatter,
     help="Characters lose color and crumble into dust, vacuumed up, and reformed.",
     description="crumble | Characters lose color and crumble into dust, vacuumed up, and reformed.",
     epilog="""Example: terminaltexteffects crumble --final-gradient-stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction diagonal""",
 )
 @dataclass
-class CrumbleEffectArgs(ArgsDataClass):
+class CrumbleConfig(ArgsDataClass):
+    """Configuration for the Crumble effect.
+
+    Attributes:
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color."""
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("5CE1FF", "FF8C00"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
 
     @classmethod
     def get_effect_class(cls):
-        return CrumbleEffect
+        return Crumble
 
 
-class CrumbleEffect:
+class CrumbleIterator(BaseEffectIterator[CrumbleConfig]):
     """Characters crumble into dust before being vacuumed up and rebuilt."""
 
-    def __init__(self, terminal: Terminal, args: CrumbleEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by registering events and building scenes/waypoints."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def __init__(self, effect: "Crumble"):
+        super().__init__(effect)
+
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
+
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-            strengthen_flash_gradient = graphics.Gradient(self.character_final_color_map[character], "ffffff", steps=6)
-            strengthen_gradient = graphics.Gradient("ffffff", self.character_final_color_map[character], steps=9)
-            weak_color = character.animation.adjust_color_brightness(self.character_final_color_map[character], 0.65)
-            dust_color = character.animation.adjust_color_brightness(self.character_final_color_map[character], 0.55)
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+            strengthen_flash_gradient = graphics.Gradient(self._character_final_color_map[character], "ffffff", steps=6)
+            strengthen_gradient = graphics.Gradient("ffffff", self._character_final_color_map[character], steps=9)
+            weak_color = character.animation.adjust_color_brightness(self._character_final_color_map[character], 0.65)
+            dust_color = character.animation.adjust_color_brightness(self._character_final_color_map[character], 0.55)
             weaken_gradient = graphics.Gradient(weak_color, dust_color, steps=9)
-            self.terminal.set_character_visibility(character, True)
+            self._terminal.set_character_visibility(character, True)
             # set up initial and falling stage
             initial_scn = character.animation.new_scene()
             initial_scn.add_frame(character.input_symbol, 1, color=weak_color)
             character.animation.activate_scene(initial_scn)
             fall_path = character.motion.new_path(
                 speed=0.2,
                 ease=easing.out_bounce,
             )
-            fall_path.new_waypoint(Coord(character.input_coord.column, self.terminal.output_area.bottom))
+            fall_path.new_waypoint(Coord(character.input_coord.column, self._terminal.output_area.bottom))
             weaken_scn = character.animation.new_scene(id="weaken")
             weaken_scn.apply_gradient_to_symbols(weaken_gradient, character.input_symbol, 6)
 
             top_path = character.motion.new_path(id="top", speed=0.5, ease=easing.out_quint)
             top_path.new_waypoint(
-                Coord(character.input_coord.column, self.terminal.output_area.top),
-                bezier_control=Coord(self.terminal.output_area.center_column, self.terminal.output_area.center_row),
+                Coord(character.input_coord.column, self._terminal.output_area.top),
+                bezier_control=Coord(self._terminal.output_area.center_column, self._terminal.output_area.center_row),
             )
             # set up reset stage
             input_path = character.motion.new_path(id="input", speed=0.3)
             input_path.new_waypoint(character.input_coord)
             strengthen_flash_scn = character.animation.new_scene()
             strengthen_flash_scn.apply_gradient_to_symbols(strengthen_flash_gradient, character.input_symbol, 4)
             strengthen_scn = character.animation.new_scene()
@@ -122,72 +133,77 @@
             )
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE,
                 strengthen_flash_scn,
                 EventHandler.Action.ACTIVATE_SCENE,
                 strengthen_scn,
             )
-            self.pending_chars.append(character)
-
-    def run(self) -> None:
-        """Runs the effect."""
-        # Prepare data for the effect
-        self.prepare_data()
-        random.shuffle(self.pending_chars)
-        fall_delay = 20
-        max_fall_delay = 20
-        min_fall_delay = 15
-        reset = False
-        fall_group_maxsize = 1
-        stage = "falling"
-        unvacuumed_chars = list(self.terminal._input_characters)
-        random.shuffle(unvacuumed_chars)
-        self.terminal.print()
-        while stage != "complete":
-            if stage == "falling":
-                if self.pending_chars:
-                    if fall_delay == 0:
+            self._pending_chars.append(character)
+        random.shuffle(self._pending_chars)
+        self.fall_delay = 20
+        self.max_fall_delay = 20
+        self.min_fall_delay = 15
+        self.reset = False
+        self.fall_group_maxsize = 1
+        self.stage = "falling"
+        self.unvacuumed_chars = list(self._terminal._input_characters)
+        random.shuffle(self.unvacuumed_chars)
+
+    def __next__(self) -> str:
+        if self.stage != "complete":
+            if self.stage == "falling":
+                if self._pending_chars:
+                    if self.fall_delay == 0:
                         # Determine the size of the next group of falling characters
-                        fall_group_size = random.randint(1, fall_group_maxsize)
+                        fall_group_size = random.randint(1, self.fall_group_maxsize)
                         # Add the next group of falling characters to the animating characters list
                         for _ in range(fall_group_size):
-                            if self.pending_chars:
-                                next_char = self.pending_chars.pop(0)
+                            if self._pending_chars:
+                                next_char = self._pending_chars.pop(0)
                                 next_char.animation.activate_scene(next_char.animation.query_scene("weaken"))
-                                self.active_chars.append(next_char)
+                                self._active_chars.append(next_char)
                         # Reset the fall delay and adjust the fall group size and delay range
-                        fall_delay = random.randint(min_fall_delay, max_fall_delay)
+                        self.fall_delay = random.randint(self.min_fall_delay, self.max_fall_delay)
                         if random.randint(1, 10) > 4:  # 60% chance to modify the fall delay and group size
-                            fall_group_maxsize += 1
-                            min_fall_delay = max(0, min_fall_delay - 1)
-                            max_fall_delay = max(0, max_fall_delay - 1)
+                            self.fall_group_maxsize += 1
+                            self.min_fall_delay = max(0, self.min_fall_delay - 1)
+                            self.max_fall_delay = max(0, self.max_fall_delay - 1)
                     else:
-                        fall_delay -= 1
-                if not self.pending_chars and not self.active_chars:
-                    stage = "vacuuming"
-            elif stage == "vacuuming":
-                if unvacuumed_chars:
+                        self.fall_delay -= 1
+                if not self._pending_chars and not self._active_chars:
+                    self.stage = "vacuuming"
+            elif self.stage == "vacuuming":
+                if self.unvacuumed_chars:
                     for _ in range(random.randint(3, 10)):
-                        if unvacuumed_chars:
-                            next_char = unvacuumed_chars.pop(0)
+                        if self.unvacuumed_chars:
+                            next_char = self.unvacuumed_chars.pop(0)
                             next_char.motion.activate_path(next_char.motion.query_path("top"))
-                            self.active_chars.append(next_char)
-                if not self.active_chars:
-                    stage = "resetting"
-
-            elif stage == "resetting":
-                if not reset:
-                    for character in self.terminal.get_characters():
+                            self._active_chars.append(next_char)
+                if not self._active_chars:
+                    self.stage = "resetting"
+
+            elif self.stage == "resetting":
+                if not self.reset:
+                    for character in self._terminal.get_characters():
                         character.motion.activate_path(character.motion.query_path("input"))
-                        self.active_chars.append(character)
-                    reset = True
-                if not self.active_chars:
-                    stage = "complete"
-
-            self.terminal.print()
-            self.animate_chars()
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method."""
-        for character in self.active_chars:
-            character.tick()
+                        self._active_chars.append(character)
+                    self.reset = True
+                if not self._active_chars:
+                    self.stage = "complete"
+
+            next_frame = self._terminal.get_formatted_output_string()
+            for character in self._active_chars:
+                character.tick()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return next_frame
+        else:
+            raise StopIteration
+
+
+class Crumble(BaseEffect[CrumbleConfig]):
+    """Characters crumble into dust before being vacuumed up and rebuilt."""
+
+    _config_cls = CrumbleConfig
+    _iterator_cls = CrumbleIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_decrypt.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_decrypt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,190 +1,224 @@
 import random
 import typing
 from dataclasses import dataclass
 
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import animation, arg_validators, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return DecryptEffect, DecryptEffectArgs
+    return Decrypt, DecryptConfig
 
 
 @argclass(
     name="decrypt",
-    formatter_class=arg_validators.CustomFormatter,
     help="Display a movie style decryption effect.",
     description="decrypt | Movie style decryption effect.",
     epilog="Example: terminaltexteffects decrypt --typing-speed 2 --ciphertext-colors 008000 00cb00 00ff00 --final-gradient-stops eda000 --final-gradient-steps 12 --final-gradient-direction vertical",
 )
 @dataclass
-class DecryptEffectArgs(ArgsDataClass):
+class DecryptConfig(ArgsDataClass):
+    """Configuration for the Decrypt effect.
+
+    Attributes:
+        typing_speed (int): Number of characters typed per keystroke.
+        ciphertext_colors (tuple[graphics.Color, ...]): Colors for the ciphertext. Color will be randomly selected for each character.
+        final_gradient_stops (tuple[graphics.Color, ...]): Colors for the character gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color."""
+
     typing_speed: int = ArgField(
         cmd_name="--typing-speed",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=1,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Number of characters typed per keystroke.",
     )  # type: ignore[assignment]
+    "int : Number of characters typed per keystroke."
+
     ciphertext_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--ciphertext-colors"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("008000", "00cb00", "00ff00"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the ciphertext. Color will be randomly selected for each character.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Colors for the ciphertext. Color will be randomly selected for each character."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("eda000",),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Colors for the character gradient. If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
 
     @classmethod
     def get_effect_class(cls):
-        return DecryptEffect
-
-
-@dataclass
-class DecryptChars:
-    """Various decimal utf-8 character ranges."""
+        return Decrypt
 
-    keyboard = list(range(33, 127))
-    blocks = list(range(9608, 9632))
-    box_drawing = list(range(9472, 9599))
-    misc = list(range(174, 452))
 
-
-class DecryptEffect:
+class DecryptIterator(BaseEffectIterator[DecryptConfig]):
     """Effect that shows a movie style text decryption effect."""
 
-    def __init__(self, terminal: Terminal, args: DecryptEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.encrypted_symbols: list[str] = []
-        self.scenes: dict[str, animation.Scene] = {}
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-        self.make_encrypted_symbols()
-
-    def make_encrypted_symbols(self) -> None:
-        for n in DecryptChars.keyboard:
-            self.encrypted_symbols.append(chr(n))
-        for n in DecryptChars.blocks:
-            self.encrypted_symbols.append(chr(n))
-        for n in DecryptChars.box_drawing:
-            self.encrypted_symbols.append(chr(n))
-        for n in DecryptChars.misc:
-            self.encrypted_symbols.append(chr(n))
+    @dataclass
+    class _DecryptChars:
+        """Various decimal utf-8 character ranges."""
+
+        keyboard = list(range(33, 127))
+        blocks = list(range(9608, 9632))
+        box_drawing = list(range(9472, 9599))
+        misc = list(range(174, 452))
+
+    def __init__(self, effect: "Decrypt") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._typing_pending_chars: list[EffectCharacter] = []
+        self._decrypting_pending_chars: list[EffectCharacter] = []
+        self._phase = "typing"
+        self._active_chars: list[EffectCharacter] = []
+        self._encrypted_symbols: list[str] = []
+        self._scenes: dict[str, animation.Scene] = {}
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._make_encrypted_symbols()
+        self._build()
+
+    def _make_encrypted_symbols(self) -> None:
+        for n in DecryptIterator._DecryptChars.keyboard:
+            self._encrypted_symbols.append(chr(n))
+        for n in DecryptIterator._DecryptChars.blocks:
+            self._encrypted_symbols.append(chr(n))
+        for n in DecryptIterator._DecryptChars.box_drawing:
+            self._encrypted_symbols.append(chr(n))
+        for n in DecryptIterator._DecryptChars.misc:
+            self._encrypted_symbols.append(chr(n))
 
-    def make_decrypting_animation_scenes(self, character: EffectCharacter) -> None:
+    def _make_decrypting_animation_scenes(self, character: EffectCharacter) -> None:
         fast_decrypt_scene = character.animation.new_scene(id="fast_decrypt")
-        color = random.choice(self.args.ciphertext_colors)
+        color = random.choice(self._config.ciphertext_colors)
         for _ in range(80):
-            symbol = random.choice(self.encrypted_symbols)
+            symbol = random.choice(self._encrypted_symbols)
             fast_decrypt_scene.add_frame(symbol, 3, color=color)
             duration = 3
         slow_decrypt_scene = character.animation.new_scene(id="slow_decrypt")
         for _ in range(random.randint(1, 15)):  # 1-15 longer duration units
-            symbol = random.choice(self.encrypted_symbols)
+            symbol = random.choice(self._encrypted_symbols)
             if random.randint(0, 100) <= 30:  # 30% chance of extra long duration
                 duration = random.randrange(50, 125)  # wide long duration range reduces 'waves' in the animation
             else:
                 duration = random.randrange(5, 10)  # shorter duration creates flipping effect
             slow_decrypt_scene.add_frame(symbol, duration, color=color)
         discovered_scene = character.animation.new_scene(id="discovered")
-        discovered_gradient = graphics.Gradient("ffffff", self.character_final_color_map[character], steps=10)
+        discovered_gradient = graphics.Gradient("ffffff", self._character_final_color_map[character], steps=10)
         discovered_scene.apply_gradient_to_symbols(discovered_gradient, character.input_symbol, 8)
 
-    def prepare_data_for_type_effect(self) -> None:
+    def _prepare_data_for_type_effect(self) -> None:
         """Prepares the data for the effect by building the animation for each character."""
-        for character in self.terminal.get_characters():
+        for character in self._terminal.get_characters():
             typing_scene = character.animation.new_scene(id="typing")
             for block_char in ["▉", "▓", "▒", "░"]:
-                typing_scene.add_frame(block_char, 2, color=random.choice(self.args.ciphertext_colors))
+                typing_scene.add_frame(block_char, 2, color=random.choice(self._config.ciphertext_colors))
 
             typing_scene.add_frame(
-                random.choice(self.encrypted_symbols), 2, color=random.choice(self.args.ciphertext_colors)
+                random.choice(self._encrypted_symbols), 2, color=random.choice(self._config.ciphertext_colors)
             )
-            self.pending_chars.append(character)
+            self._typing_pending_chars.append(character)
 
-    def prepare_data_for_decrypt_effect(self) -> None:
+    def _prepare_data_for_decrypt_effect(self) -> None:
         """Prepares the data for the effect by building the animation for each character."""
-        for character in self.terminal.get_characters():
-            self.make_decrypting_animation_scenes(character)
+        for character in self._terminal.get_characters():
+            self._make_decrypting_animation_scenes(character)
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE,
                 character.animation.query_scene("fast_decrypt"),
                 EventHandler.Action.ACTIVATE_SCENE,
                 character.animation.query_scene("slow_decrypt"),
             )
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE,
                 character.animation.query_scene("slow_decrypt"),
                 EventHandler.Action.ACTIVATE_SCENE,
                 character.animation.query_scene("discovered"),
             )
             character.animation.activate_scene(character.animation.query_scene("fast_decrypt"))
-            self.active_chars.append(character)
+            self._decrypting_pending_chars.append(character)
 
-    def run(self) -> None:
-        """Runs the effect."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        """Builds the effect."""
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        self.prepare_data_for_type_effect()
-        self.run_type_effect()
-        self.prepare_data_for_decrypt_effect()
-        self.run_decryption_effect()
-
-    def run_type_effect(self) -> None:
-        """Runs the typing out the characters effect."""
-        self.terminal.print()
-        while self.pending_chars or self.active_chars:
-            if self.pending_chars:
-                if random.randint(0, 100) <= 75:
-                    for _ in range(self.args.typing_speed):
-                        if self.pending_chars:
-                            next_character = self.pending_chars.pop(0)
-                            self.terminal.set_character_visibility(next_character, True)
-                            next_character.animation.activate_scene(next_character.animation.query_scene("typing"))
-                            self.active_chars.append(next_character)
-            self.animate_chars()
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-            self.terminal.print()
-
-    def run_decryption_effect(self) -> None:
-        while self.active_chars:
-            self.animate_chars()
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-            self.terminal.print()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tween method and printing the characters to the terminal."""
-        for character in self.active_chars:
-            character.tick()
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        self._prepare_data_for_type_effect()
+        self._prepare_data_for_decrypt_effect()
+
+    def __next__(self) -> str:
+        if self._phase == "typing":
+            if self._typing_pending_chars or self._active_chars:
+                if self._typing_pending_chars:
+                    if random.randint(0, 100) <= 75:
+                        for _ in range(self._config.typing_speed):
+                            if self._typing_pending_chars:
+                                next_character = self._typing_pending_chars.pop(0)
+                                self._terminal.set_character_visibility(next_character, True)
+                                next_character.animation.activate_scene(next_character.animation.query_scene("typing"))
+                                self._active_chars.append(next_character)
+                for character in self._active_chars:
+                    character.tick()
+                self._active_chars = [character for character in self._active_chars if character.is_active]
+                return self._terminal.get_formatted_output_string()
+            else:
+                self._active_chars = self._decrypting_pending_chars
+                for char in self._active_chars:
+                    char.animation.activate_scene(char.animation.query_scene("fast_decrypt"))
+                self._phase = "decrypting"
+
+        if self._phase == "decrypting":
+            if self._active_chars:
+                for character in self._active_chars:
+                    character.tick()
+                self._active_chars = [character for character in self._active_chars if character.is_active]
+                return self._terminal.get_formatted_output_string()
+            else:
+                raise StopIteration
+        else:
+            raise StopIteration
+
+
+class Decrypt(BaseEffect[DecryptConfig]):
+    """Effect that shows a movie style text decryption effect."""
+
+    _config_cls = DecryptConfig
+    _iterator_cls = DecryptIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
+
+    def __iter__(self) -> DecryptIterator:
+        return DecryptIterator(self)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_errorcorrect.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_pour.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,222 +1,240 @@
-import random
+"""Effect that pours the characters into position from the top, bottom, left, or right."""
+
 import typing
 from dataclasses import dataclass
+from enum import Enum, auto
 
 import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.utils import animation, graphics
+from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
+from terminaltexteffects.utils.geometry import Coord
 from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return ErrorCorrectEffect, ErrorCorrectEffectArgs
+    return Pour, PourConfig
 
 
 @argclass(
-    name="errorcorrect",
-    formatter_class=arg_validators.CustomFormatter,
-    help="Some characters start in the wrong position and are corrected in sequence.",
-    description="errorcorrect | Some characters start in the wrong position and are corrected in sequence.",
+    name="pour",
+    help="Pours the characters into position from the given direction.",
+    description="pour | Pours the characters into position from the given direction.",
     epilog=f"""{arg_validators.EASING_EPILOG}
-    
-Example: terminaltexteffects errorcorrect --error-pairs 0.1 --swap-delay 10 --error-color e74c3c --correct-color 45bf55 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --movement-speed 0.5""",
+Example: terminaltexteffects pour --pour-direction down --movement-speed 0.2 --gap 1 --starting-color FFFFFF --final-gradient-stops 8A008A 00D1FF FFFFFF --easing IN_QUAD""",
 )
 @dataclass
-class ErrorCorrectEffectArgs(ArgsDataClass):
-    error_pairs: float = ArgField(
-        cmd_name="--error-pairs",
-        type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.1,
-        metavar="(int > 0)",
-        help="Percent of characters that are in the wrong position. This is a float between 0 and 1.0. 0.2 means 20 percent of the characters will be in the wrong position.",
+class PourConfig(ArgsDataClass):
+    """Configuration for the Pour effect.
+
+    Attributes:
+        pour_direction (str): Direction the text will pour.
+        pour_speed (int): Number of characters poured in per tick. Increase to speed up the effect.
+        movement_speed (float): Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
+        gap (int): Number of frames to wait between each character in the pour effect. Increase to slow down effect and create a more defined back and forth motion.
+        starting_color (graphics.Color): Color of the characters before the gradient starts.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_frames (int): Number of frames to display each gradient step.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        easing (typing.Callable): Easing function to use for character movement."""
+
+    pour_direction: str = ArgField(
+        cmd_name=["--pour-direction"],
+        default="down",
+        choices=["up", "down", "left", "right"],
+        help="Direction the text will pour.",
     )  # type: ignore[assignment]
-    swap_delay: int = ArgField(
-        cmd_name="--swap-delay",
+    "str : Direction the text will pour."
+
+    pour_speed: int = ArgField(
+        cmd_name="--pour-speed",
         type_parser=arg_validators.PositiveInt.type_parser,
-        default=10,
-        metavar="(int > 0)",
-        help="Number of animation steps between swaps.",
+        default=1,
+        metavar=arg_validators.PositiveInt.METAVAR,
+        help="Number of characters poured in per tick. Increase to speed up the effect.",
     )  # type: ignore[assignment]
-    error_color: graphics.Color = ArgField(
-        cmd_name=["--error-color"],
-        type_parser=arg_validators.Color.type_parser,
-        default="e74c3c",
-        metavar="(XTerm [0-255] OR RGB Hex [000000-ffffff])",
-        help="Color for the characters that are in the wrong position.",
+    "int : Number of characters poured in per tick. Increase to speed up the effect."
+
+    movement_speed: float = ArgField(
+        cmd_name="--movement-speed",
+        type_parser=arg_validators.PositiveFloat.type_parser,
+        default=0.2,
+        metavar=arg_validators.PositiveFloat.METAVAR,
+        help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+    )  # type: ignore[assignment]
+    "float : Movement speed of the characters."
+
+    gap: int = ArgField(
+        cmd_name="--gap",
+        type_parser=arg_validators.NonNegativeInt.type_parser,
+        default=1,
+        metavar=arg_validators.NonNegativeInt.METAVAR,
+        help="Number of frames to wait between each character in the pour effect. Increase to slow down effect and create a more defined back and forth motion.",
     )  # type: ignore[assignment]
-    correct_color: graphics.Color = ArgField(
-        cmd_name=["--correct-color"],
+    "int : Number of frames to wait between each character in the pour effect."
+
+    starting_color: graphics.Color = ArgField(
+        cmd_name=["--starting-color"],
         type_parser=arg_validators.Color.type_parser,
-        default="45bf55",
-        metavar="(XTerm [0-255] OR RGB Hex [000000-ffffff])",
-        help="Color for the characters once corrected, this is a gradient from error-color and fades to final-color.",
+        default="ffffff",
+        metavar=arg_validators.Color.METAVAR,
+        help="Color of the characters before the gradient starts.",
     )  # type: ignore[assignment]
+    "graphics.Color : Color of the characters before the gradient starts."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
-        metavar="(XTerm [0-255] OR RGB Hex [000000-ffffff])",
-        help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
+        metavar=arg_validators.Color.METAVAR,
+        help="Space separated, unquoted, list of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name="--final-gradient-steps",
+        cmd_name=["--final-gradient-steps"],
         type_parser=arg_validators.PositiveInt.type_parser,
-        nargs="+",
         default=(12,),
-        metavar="(int > 0)",
-        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
+        metavar=arg_validators.PositiveInt.METAVAR,
+        help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use."
+
+    final_gradient_frames: int = ArgField(
+        cmd_name=["--final-gradient-frames"],
+        type_parser=arg_validators.PositiveInt.type_parser,
+        default=10,
+        metavar=arg_validators.PositiveInt.METAVAR,
+        help="Number of frames to display each gradient step.",
+    )  # type: ignore[assignment]
+    "int : Number of frames to display each gradient step."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
 
-    movement_speed: float = ArgField(
-        cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.5,
-        metavar="(float > 0)",
-        help="Speed of the characters while moving to the correct position. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+    movement_easing: easing.EasingFunction = ArgField(
+        cmd_name="--movement-easing",
+        default=easing.in_quad,
+        type_parser=arg_validators.Ease.type_parser,
+        help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
-        return ErrorCorrectEffect
-
+        return Pour
 
-class ErrorCorrectEffect:
-    """Effect that swaps characters from an incorrect initial position to the correct position."""
 
-    def __init__(self, terminal: Terminal, args: ErrorCorrectEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.swapped: list[tuple[EffectCharacter, EffectCharacter]] = []
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by swapping positions and generating animations and waypoints."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+class PourDirection(Enum):
+    UP = auto()
+    DOWN = auto()
+    LEFT = auto()
+    RIGHT = auto()
+
+
+class PourIterator(BaseEffectIterator[PourConfig]):
+    def __init__(self, effect: "Pour") -> None:
+        super().__init__(effect)
+        self._pending_groups: list[list[EffectCharacter]] = []
+        self._active_characters: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
+
+    def _build(self) -> None:
+        self._pour_direction = {
+            "down": PourDirection.DOWN,
+            "up": PourDirection.UP,
+            "left": PourDirection.LEFT,
+            "right": PourDirection.RIGHT,
+        }.get(self._config.pour_direction, PourDirection.DOWN)
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        for character in self.terminal.get_characters():
-            spawn_scene = character.animation.new_scene()
-            spawn_scene.add_frame(character.input_symbol, 1, color=self.character_final_color_map[character])
-            character.animation.activate_scene(spawn_scene)
-            self.terminal.set_character_visibility(character, True)
-        all_characters: list[EffectCharacter] = list(self.terminal._input_characters)
-        correcting_gradient = graphics.Gradient(self.args.error_color, self.args.correct_color, steps=10)
-        block_symbol = "▓"
-        block_wipe_start = ("▁", "▂", "▃", "▄", "▅", "▆", "▇", "█")
-        block_wipe_end = ("▇", "▆", "▅", "▄", "▃", "▂", "▁")
-        for _ in range(int(self.args.error_pairs * len(self.terminal.get_characters()))):
-            if len(all_characters) < 2:
-                break
-            char1 = all_characters.pop(random.randrange(len(all_characters)))
-            char2 = all_characters.pop(random.randrange(len(all_characters)))
-            char1.motion.set_coordinate(char2.input_coord)
-            char1_input_coord_path = char1.motion.new_path(id="input_coord", speed=self.args.movement_speed)
-            char1_input_coord_path.new_waypoint(char1.input_coord)
-            char2.motion.set_coordinate(char1.input_coord)
-            char2_input_coord_path = char2.motion.new_path(id="input_coord", speed=self.args.movement_speed)
-            char2_input_coord_path.new_waypoint(char2.input_coord)
-            self.swapped.append((char1, char2))
-            for character in (char1, char2):
-                first_block_wipe = character.animation.new_scene()
-                last_block_wipe = character.animation.new_scene()
-                for block in block_wipe_start:
-                    first_block_wipe.add_frame(block, 3, color=self.args.error_color)
-                for block in block_wipe_end:
-                    last_block_wipe.add_frame(block, 3, color=self.args.correct_color)
-                initial_scene = character.animation.new_scene()
-                initial_scene.add_frame(character.input_symbol, 1, color=self.args.error_color)
-                character.animation.activate_scene(initial_scene)
-                error_scene = character.animation.new_scene(id="error")
-                for _ in range(10):
-                    error_scene.add_frame(block_symbol, 3, color=self.args.error_color)
-                    error_scene.add_frame(character.input_symbol, 3, color="ffffff")
-                correcting_scene = character.animation.new_scene(sync=animation.SyncMetric.DISTANCE)
-                correcting_scene.apply_gradient_to_symbols(correcting_gradient, "█", 3)
-                final_scene = character.animation.new_scene()
-                char_final_gradient = graphics.Gradient(
-                    self.args.correct_color, self.character_final_color_map[character], steps=10
-                )
-                final_scene.apply_gradient_to_symbols(char_final_gradient, character.input_symbol, 3)
-                input_coord_path = character.motion.query_path("input_coord")
-                character.event_handler.register_event(
-                    EventHandler.Event.SCENE_COMPLETE,
-                    error_scene,
-                    EventHandler.Action.ACTIVATE_SCENE,
-                    first_block_wipe,
-                )
-                character.event_handler.register_event(
-                    EventHandler.Event.SCENE_COMPLETE,
-                    first_block_wipe,
-                    EventHandler.Action.ACTIVATE_SCENE,
-                    correcting_scene,
-                )
-                character.event_handler.register_event(
-                    EventHandler.Event.SCENE_COMPLETE,
-                    first_block_wipe,
-                    EventHandler.Action.ACTIVATE_PATH,
-                    input_coord_path,
-                )
-                character.event_handler.register_event(
-                    EventHandler.Event.PATH_ACTIVATED,
-                    input_coord_path,
-                    EventHandler.Action.SET_LAYER,
-                    1,
-                )
-                character.event_handler.register_event(
-                    EventHandler.Event.PATH_COMPLETE,
-                    input_coord_path,
-                    EventHandler.Action.SET_LAYER,
-                    0,
-                )
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        sort_map = {
+            PourDirection.DOWN: Terminal.CharacterGroup.ROW_BOTTOM_TO_TOP,
+            PourDirection.UP: Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM,
+            PourDirection.LEFT: Terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT,
+            PourDirection.RIGHT: Terminal.CharacterGroup.COLUMN_RIGHT_TO_LEFT,
+        }
+        groups = self._terminal.get_characters_grouped(grouping=sort_map[self._pour_direction])
+        for i, group in enumerate(groups):
+            for character in group:
+                self._terminal.set_character_visibility(character, False)
+                if self._pour_direction == PourDirection.DOWN:
+                    character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.top))
+                elif self._pour_direction == PourDirection.UP:
+                    character.motion.set_coordinate(
+                        Coord(character.input_coord.column, self._terminal.output_area.bottom)
+                    )
+                elif self._pour_direction == PourDirection.LEFT:
+                    character.motion.set_coordinate(Coord(self._terminal.output_area.right, character.input_coord.row))
+                elif self._pour_direction == PourDirection.RIGHT:
+                    character.motion.set_coordinate(Coord(self._terminal.output_area.left, character.input_coord.row))
+                input_coord_path = character.motion.new_path(
+                    speed=self._config.movement_speed,
+                    ease=self._config.movement_easing,
+                )
+                input_coord_path.new_waypoint(character.input_coord)
+                character.motion.activate_path(input_coord_path)
+
+                pour_gradient = graphics.Gradient(
+                    self._config.starting_color,
+                    self._character_final_color_map[character],
+                    steps=self._config.final_gradient_steps,
+                )
+                pour_scn = character.animation.new_scene()
+                pour_scn.apply_gradient_to_symbols(
+                    pour_gradient, character.input_symbol, self._config.final_gradient_frames
+                )
+                character.animation.activate_scene(pour_scn)
+            if i % 2 == 0:
+                self._pending_groups.append(group)
+            else:
+                self._pending_groups.append(group[::-1])
+        self.gap = 0
+        self.current_group = self._pending_groups.pop(0)
+
+    def __next__(self) -> str:
+        if self._pending_groups or self._active_characters or self.current_group:
+            if not self.current_group:
+                if self._pending_groups:
+                    self.current_group = self._pending_groups.pop(0)
+            if self.current_group:
+                if not self.gap:
+                    for _ in range(self._config.pour_speed):
+                        if self.current_group:
+                            next_character = self.current_group.pop(0)
+                            self._terminal.set_character_visibility(next_character, True)
+                            self._active_characters.append(next_character)
+                    self.gap = self._config.gap
+                else:
+                    self.gap -= 1
+            for character in self._active_characters:
+                character.tick()
+            next_frame = self._terminal.get_formatted_output_string()
+            self._active_characters = [character for character in self._active_characters if character.is_active]
+            return next_frame
+        else:
+            raise StopIteration
 
-                character.event_handler.register_event(
-                    EventHandler.Event.PATH_COMPLETE,
-                    input_coord_path,
-                    EventHandler.Action.ACTIVATE_SCENE,
-                    last_block_wipe,
-                )
-                character.event_handler.register_event(
-                    EventHandler.Event.SCENE_COMPLETE,
-                    last_block_wipe,
-                    EventHandler.Action.ACTIVATE_SCENE,
-                    final_scene,
-                )
 
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        while self.swapped or self.active_chars:
-            swap_delay = self.args.swap_delay
-            if self.swapped:
-                next_pair = self.swapped.pop(0)
-                for char in next_pair:
-                    char.animation.activate_scene(char.animation.query_scene("error"))
-                    self.active_chars.append(char)
-            while swap_delay:
-                self.terminal.print()
-                self.animate_chars()
-
-                self.active_chars = [character for character in self.active_chars if character.is_active]
-                if not self.active_chars:
-                    pass
-                swap_delay -= 1
-        self.terminal.print()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+class Pour(BaseEffect[PourConfig]):
+    """Effect that pours the characters into position from the top, bottom, left, or right."""
+
+    _config_cls = PourConfig
+    _iterator_cls = PourIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_expand.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_random_sequence.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,127 +1,146 @@
+import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.utils import easing, graphics
+from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return ExpandEffect, ExpandEffectArgs
+    return RandomSequence, RandomSequenceConfig
 
 
 @argclass(
-    name="expand",
-    formatter_class=arg_validators.CustomFormatter,
-    help="Expands the text from a single point.",
-    description="expand | Expands the text from a single point.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
-    
-Example: terminaltexteffects expand --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-frames 5 --movement-speed 0.35 --expand-easing IN_OUT_QUART""",
+    name="randomsequence",
+    help="Prints the input data in a random sequence.",
+    description="randomsequence | Prints the input data in a random sequence.",
+    epilog="Example: terminaltexteffects randomsequence --starting-color 000000 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-frames 12 --speed 0.004",
 )
 @dataclass
-class ExpandEffectArgs(ArgsDataClass):
+class RandomSequenceConfig(ArgsDataClass):
+    """Configuration for the RandomSequence effect.
+
+    Attributes:
+        starting_color (graphics.Color): Color of the characters at spawn.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_frames (int): Number of frames to display each gradient step.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        speed (float): Speed of the animation as a percentage of the total number of characters to reveal in each tick.
+    """
+
+    starting_color: graphics.Color = ArgField(
+        cmd_name=["--starting-color"],
+        type_parser=arg_validators.Color.type_parser,
+        default="000000",
+        metavar=arg_validators.Color.METAVAR,
+        help="Color of the characters at spawn.",
+    )  # type: ignore[assignment]
+
+    "graphics.Color : Color of the characters at spawn."
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
     final_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name="--final-gradient-steps",
+        cmd_name=["--final-gradient-steps"],
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
     final_gradient_frames: int = ArgField(
-        cmd_name="--final-gradient-frames",
+        cmd_name=["--final-gradient-frames"],
         type_parser=arg_validators.PositiveInt.type_parser,
-        default=5,
+        default=12,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Number of frames to display each gradient step.",
     )  # type: ignore[assignment]
+
+    "int : Number of frames to display each gradient step."
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
-    movement_speed: float = ArgField(
-        cmd_name="--movement-speed",
+
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+    speed: float = ArgField(
+        cmd_name=["--speed"],
         type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.35,
+        default=0.004,
         metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
-    )  # type: ignore[assignment]
-    expand_easing: typing.Callable = ArgField(
-        cmd_name="--expand-easing",
-        default=easing.in_out_quart,
-        type_parser=arg_validators.Ease.type_parser,
-        help="Easing function to use for character movement.",
+        help="Speed of the animation as a percentage of the total number of characters to reveal in each tick.",
     )  # type: ignore[assignment]
 
+    "float : Speed of the animation as a percentage of the total number of characters to reveal in each tick."
+
     @classmethod
     def get_effect_class(cls):
-        return ExpandEffect
+        return RandomSequence
 
 
-class ExpandEffect:
-    """Effect that draws the characters expanding from a single point."""
+class RandomSequenceIterator(BaseEffectIterator[RandomSequenceConfig]):
+    def __init__(self, effect: "RandomSequence") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._characters_per_tick = max(int(self._config.speed * len(self._terminal._input_characters)), 1)
+        self._build()
 
-    def __init__(self, terminal: Terminal, args: ExpandEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by starting all of the characters from a point in the middle of the input data."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        for character in self.terminal.get_characters():
-            character.motion.set_coordinate(self.terminal.output_area.center)
-            input_coord_path = character.motion.new_path(
-                speed=self.args.movement_speed,
-                ease=self.args.expand_easing,
-            )
-            input_coord_path.new_waypoint(character.input_coord)
-            self.terminal.set_character_visibility(character, True)
-            self.active_chars.append(character)
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_ACTIVATED, input_coord_path, EventHandler.Action.SET_LAYER, 1
-            )
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_COMPLETE, input_coord_path, EventHandler.Action.SET_LAYER, 0
-            )
-            character.motion.activate_path(input_coord_path)
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+            self._terminal.set_character_visibility(character, False)
             gradient_scn = character.animation.new_scene()
             gradient = graphics.Gradient(
-                final_gradient.spectrum[0], self.character_final_color_map[character], steps=10
+                self._config.starting_color, self._character_final_color_map[character], steps=7
             )
-            gradient_scn.apply_gradient_to_symbols(gradient, character.input_symbol, self.args.final_gradient_frames)
+            gradient_scn.apply_gradient_to_symbols(gradient, character.input_symbol, self._config.final_gradient_frames)
             character.animation.activate_scene(gradient_scn)
+            self._pending_chars.append(character)
+        random.shuffle(self._pending_chars)
+
+    def __next__(self) -> str:
+        if self._pending_chars or self._active_chars:
+            for _ in range(self._characters_per_tick):
+                if self._pending_chars:
+                    next_char = self._pending_chars.pop()
+                    self._terminal.set_character_visibility(next_char, True)
+                    self._active_chars.append(next_char)
+            for character in self._active_chars:
+                character.tick()
+            next_frame = self._terminal.get_formatted_output_string()
+
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return next_frame
+        raise StopIteration
+
+
+class RandomSequence(BaseEffect[RandomSequenceConfig]):
+    """Prints the input data in a random sequence, one character at a time."""
+
+    _config_cls = RandomSequenceConfig
+    _iterator_cls = RandomSequenceIterator
 
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        self.terminal.print()
-        while self.active_chars:
-            self.animate_chars()
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-            self.terminal.print()
-
-    def animate_chars(self) -> None:
-        for character in self.active_chars:
-            character.tick()
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_fireworks.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_spray.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,223 +1,220 @@
+"""Effect that draws the characters spawning at varying rates from a single point."""
+
 import random
 import typing
 from dataclasses import dataclass
+from enum import Enum, auto
 
+import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.utils import arg_validators, easing, geometry, graphics
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return FireworksEffect, FireworksEffectArgs
+    return Spray, SprayConfig
 
 
 @argclass(
-    name="fireworks",
-    formatter_class=arg_validators.CustomFormatter,
-    help="Characters launch and explode like fireworks and fall into place.",
-    description="fireworks | Characters explode like fireworks and fall into place.",
-    epilog="""Example: terminaltexteffects fireworks --firework-colors 88F7E2 44D492 F5EB67 FFA15C FA233E --firework-symbol o --firework-volume 0.02 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --launch-delay 60 --explode-distance 0.1 --explode-anywhere""",
+    name="spray",
+    help="Draws the characters spawning at varying rates from a single point.",
+    description="spray | Draws the characters spawning at varying rates from a single point.",
+    epilog=f"""{arg_validators.EASING_EPILOG}    
+Example: terminaltexteffects spray --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --spray-position e --spray-volume 0.005 --movement-speed 0.4-1.0 --movement-easing OUT_EXPO""",
 )
 @dataclass
-class FireworksEffectArgs(ArgsDataClass):
-    explode_anywhere: bool = ArgField(
-        cmd_name="--explode-anywhere",
-        action="store_true",
-        default=False,
-        help="If set, fireworks explode anywhere in the output area. Otherwise, fireworks explode above highest settled row of text.",
-    )  # type: ignore[assignment]
-    firework_colors: tuple[graphics.Color, ...] = ArgField(
-        cmd_name="--firework-colors",
-        type_parser=arg_validators.Color.type_parser,
-        nargs="+",
-        default=("88F7E2", "44D492", "F5EB67", "FFA15C", "FA233E"),
-        metavar=arg_validators.Color.METAVAR,
-        help="Space separated list of colors from which firework colors will be randomly selected.",
-    )  # type: ignore[assignment]
-    firework_symbol: str = ArgField(
-        cmd_name="--firework-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
-        default="o",
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Symbol to use for the firework shell.",
-    )  # type: ignore[assignment]
-    firework_volume: float = ArgField(
-        cmd_name="--firework-volume",
-        type_parser=arg_validators.Ratio.type_parser,
-        default=0.02,
-        metavar=arg_validators.Ratio.METAVAR,
-        help="Percent of total characters in each firework shell.",
-    )  # type: ignore[assignment]
+class SprayConfig(ArgsDataClass):
+    """Configuration for the Spray effect.
+
+    Attributes:
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        spray_position (str): Position for the spray origin.
+        spray_volume (float): Number of characters to spray per tick as a percent of the total number of characters.
+        movement_speed (tuple[float, float]): Movement speed of the characters.
+        movement_easing (typing.Callable): Easing function to use for character movement."""
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name="--final-gradient-stops",
+        cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name="--final-gradient-steps",
+        cmd_name=["--final-gradient-steps"],
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
-        default=graphics.Gradient.Direction.HORIZONTAL,
+        default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
-    launch_delay: int = ArgField(
-        cmd_name="--launch-delay",
-        type_parser=arg_validators.NonNegativeInt.type_parser,
-        default=60,
-        metavar=arg_validators.NonNegativeInt.METAVAR,
-        help="Number of animation steps to wait between launching each firework shell. +/- 0-50 percent randomness is applied to this value.",
-    )  # type: ignore[assignment]
-    explode_distance: float = ArgField(
-        cmd_name="--explode-distance",
-        default=0.1,
-        type_parser=arg_validators.Ratio.type_parser,
-        metavar=arg_validators.Ratio.METAVAR,
-        help="Maximum distance from the firework shell origin to the explode waypoint as a percentage of the total output area width.",
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
+    spray_position: str = ArgField(
+        cmd_name="--spray-position",
+        choices=["n", "ne", "e", "se", "s", "sw", "w", "nw", "center"],
+        default="e",
+        help="Position for the spray origin.",
+    )  # type: ignore[assignment]
+    "str : Position for the spray origin."
+
+    spray_volume: float = ArgField(
+        cmd_name="--spray-volume",
+        type_parser=arg_validators.PositiveFloat.type_parser,
+        default=0.005,
+        metavar=arg_validators.PositiveFloat.METAVAR,
+        help="Number of characters to spray per tick as a percent of the total number of characters.",
+    )  # type: ignore[assignment]
+    "float : Number of characters to spray per tick as a percent of the total number of characters."
+
+    movement_speed: tuple[float, float] = ArgField(
+        cmd_name="--movement-speed",
+        type_parser=arg_validators.PositiveFloatRange.type_parser,
+        default=(0.4, 1.0),
+        metavar=arg_validators.PositiveFloatRange.METAVAR,
+        help="Movement speed of the characters.",
+    )  # type: ignore[assignment]
+    "tuple[float, float] : Movement speed of the characters."
+
+    movement_easing: easing.EasingFunction = ArgField(
+        cmd_name="--movement-easing",
+        type_parser=arg_validators.Ease.type_parser,
+        default=easing.out_expo,
+        help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
-        return FireworksEffect
+        return Spray
 
 
-class FireworksEffect:
-    """Effect that launches characters up the screen where they explode like fireworks and fall into place."""
-
-    def __init__(self, terminal: Terminal, args: FireworksEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.shells: list[list[EffectCharacter]] = []
-        self.firework_volume = max(1, round(self.args.firework_volume * len(self.terminal._input_characters)))
-        self.explode_distance = max(1, round(self.terminal.output_area.right * self.args.explode_distance))
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_waypoints(self) -> None:
-        firework_shell: list[EffectCharacter] = []
-        for character in self.terminal.get_characters():
-            if len(firework_shell) == self.firework_volume or not firework_shell:
-                self.shells.append(firework_shell)
-                firework_shell = []
-                origin_x = random.randrange(0, self.terminal.output_area.right)
-                if not self.args.explode_anywhere:
-                    min_row = character.input_coord.row
-                else:
-                    min_row = self.terminal.output_area.bottom
-                origin_y = random.randrange(min_row, self.terminal.output_area.top + 1)
-                origin_coord = Coord(origin_x, origin_y)
-                explode_waypoint_coords = geometry.find_coords_in_circle(origin_coord, self.explode_distance)
-            character.motion.set_coordinate(Coord(origin_x, self.terminal.output_area.bottom))
-            apex_path = character.motion.new_path(id="apex_pth", speed=0.2, ease=easing.out_expo)
-            apex_wpt = apex_path.new_waypoint(origin_coord)
-            explode_path = character.motion.new_path(speed=0.15, ease=easing.out_circ)
-            explode_wpt = explode_path.new_waypoint(random.choice(explode_waypoint_coords))
-
-            bloom_control_point = geometry.find_coord_at_distance(
-                apex_wpt.coord, explode_wpt.coord, self.explode_distance // 2
-            )
-            bloom_wpt = explode_path.new_waypoint(
-                Coord(bloom_control_point.column, max(1, bloom_control_point.row - 7)),
-                bezier_control=bloom_control_point,
-            )
-            input_path = character.motion.new_path(id="input_pth", speed=0.3, ease=easing.in_out_quart)
-            input_control_point = Coord(bloom_wpt.coord.column, 1)
-            input_path.new_waypoint(character.input_coord, bezier_control=input_control_point)
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_ACTIVATED, apex_path, EventHandler.Action.SET_LAYER, 2
-            )
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_COMPLETE, explode_path, EventHandler.Action.SET_LAYER, 0
+class SprayIterator(BaseEffectIterator[SprayConfig]):
+    class _SprayPosition(Enum):
+        """Position for the spray origin."""
+
+        N = auto()
+        NE = auto()
+        E = auto()
+        SE = auto()
+        S = auto()
+        SW = auto()
+        W = auto()
+        NW = auto()
+        CENTER = auto()
+
+    def __init__(
+        self,
+        effect: "Spray",
+    ) -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
+
+    def _build(self) -> None:
+        self._spray_position = {
+            "n": SprayIterator._SprayPosition.N,
+            "ne": SprayIterator._SprayPosition.NE,
+            "e": SprayIterator._SprayPosition.E,
+            "se": SprayIterator._SprayPosition.SE,
+            "s": SprayIterator._SprayPosition.S,
+            "sw": SprayIterator._SprayPosition.SW,
+            "w": SprayIterator._SprayPosition.W,
+            "nw": SprayIterator._SprayPosition.NW,
+            "center": SprayIterator._SprayPosition.CENTER,
+        }.get(self._config.spray_position, SprayIterator._SprayPosition.E)
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+        final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+        )
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        spray_origin_map = {
+            SprayIterator._SprayPosition.CENTER: (self._terminal.output_area.center),
+            SprayIterator._SprayPosition.N: Coord(
+                self._terminal.output_area.right // 2, self._terminal.output_area.top
+            ),
+            SprayIterator._SprayPosition.NW: Coord(self._terminal.output_area.left, self._terminal.output_area.top),
+            SprayIterator._SprayPosition.W: Coord(self._terminal.output_area.left, self._terminal.output_area.top // 2),
+            SprayIterator._SprayPosition.SW: Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
+            SprayIterator._SprayPosition.S: Coord(
+                self._terminal.output_area.right // 2, self._terminal.output_area.bottom
+            ),
+            SprayIterator._SprayPosition.SE: Coord(
+                self._terminal.output_area.right - 1, self._terminal.output_area.bottom
+            ),
+            SprayIterator._SprayPosition.E: Coord(
+                self._terminal.output_area.right - 1, self._terminal.output_area.top // 2
+            ),
+            SprayIterator._SprayPosition.NE: Coord(
+                self._terminal.output_area.right - 1, self._terminal.output_area.top
+            ),
+        }
+
+        for character in self._terminal.get_characters():
+            character.motion.set_coordinate(spray_origin_map[self._spray_position])
+            input_coord_path = character.motion.new_path(
+                speed=random.uniform(self._config.movement_speed[0], self._config.movement_speed[1]),
+                ease=self._config.movement_easing,
             )
+            input_coord_path.new_waypoint(character.input_coord)
             character.event_handler.register_event(
-                EventHandler.Event.PATH_COMPLETE,
-                apex_path,
-                EventHandler.Action.ACTIVATE_PATH,
-                explode_path,
+                EventHandler.Event.PATH_ACTIVATED, input_coord_path, EventHandler.Action.SET_LAYER, 1
             )
             character.event_handler.register_event(
-                EventHandler.Event.PATH_COMPLETE, explode_path, EventHandler.Action.ACTIVATE_PATH, input_path
+                EventHandler.Event.PATH_COMPLETE, input_coord_path, EventHandler.Action.SET_LAYER, 0
             )
+            droplet_scn = character.animation.new_scene()
+            spray_gradient = graphics.Gradient(
+                random.choice(final_gradient.spectrum), self._character_final_color_map[character], steps=7
+            )
+            droplet_scn.apply_gradient_to_symbols(spray_gradient, character.input_symbol, 20)
+            character.animation.activate_scene(droplet_scn)
+            character.motion.activate_path(input_coord_path)
+            self._pending_chars.append(character)
+        random.shuffle(self._pending_chars)
+        self._volume = max(int(len(self._pending_chars) * self._config.spray_volume), 1)
+
+    def __next__(self) -> str:
+        if self._pending_chars or self._active_chars:
+            if self._pending_chars:
+                for _ in range(random.randint(1, self._volume)):
+                    if self._pending_chars:
+                        next_character = self._pending_chars.pop()
+                        self._terminal.set_character_visibility(next_character, True)
+                        self._active_chars.append(next_character)
+
+            for character in self._active_chars:
+                character.tick()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
 
-            character.motion.activate_path(apex_path)
 
-            firework_shell.append(character)
-        if firework_shell:
-            self.shells.append(firework_shell)
+class Spray(BaseEffect[SprayConfig]):
+    """Effect that draws the characters spawning at varying rates from a single point."""
 
-    def prepare_scenes(self) -> None:
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
-        final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
-        )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        for firework_shell in self.shells:
-            shell_color = random.choice(self.args.firework_colors)
-            for character in firework_shell:
-                # launch scene
-                launch_scn = character.animation.new_scene()
-                launch_scn.add_frame(self.args.firework_symbol, 2, color=shell_color)
-                launch_scn.add_frame(self.args.firework_symbol, 1, color="FFFFFF")
-                launch_scn.is_looping = True
-                # bloom scene
-                bloom_scn = character.animation.new_scene()
-                bloom_scn.add_frame(character.input_symbol, 1, color=shell_color)
-                # fall scene
-                fall_scn = character.animation.new_scene()
-                fall_gradient = graphics.Gradient(shell_color, self.character_final_color_map[character], steps=15)
-                fall_scn.apply_gradient_to_symbols(fall_gradient, character.input_symbol, 15)
-                character.animation.activate_scene(launch_scn)
-                character.event_handler.register_event(
-                    EventHandler.Event.PATH_COMPLETE,
-                    character.motion.query_path("apex_pth"),
-                    EventHandler.Action.ACTIVATE_SCENE,
-                    bloom_scn,
-                )
-                character.event_handler.register_event(
-                    EventHandler.Event.PATH_ACTIVATED,
-                    character.motion.query_path("input_pth"),
-                    EventHandler.Action.ACTIVATE_SCENE,
-                    fall_scn,
-                )
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by building the firework shells and scenes."""
-        self.prepare_waypoints()
-        self.prepare_scenes()
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        launch_delay = 0
-        while self.shells or self.active_chars:
-            if self.shells and launch_delay == 0:
-                next_group = self.shells.pop()
-                for character in next_group:
-                    self.terminal.set_character_visibility(character, True)
-                    self.active_chars.append(character)
-                launch_delay = int(self.args.launch_delay * random.uniform(0.5, 1.5))
-            self.terminal.print()
-            self.animate_chars()
-            launch_delay -= 1
-
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-        self.terminal.print()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method."""
-        for character in self.active_chars:
-            character.tick()
+    _config_cls = SprayConfig
+    _iterator_cls = SprayIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_middleout.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_scattered.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,158 +1,157 @@
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.utils import easing, graphics
+from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import arg_validators, easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return MiddleoutEffect, MiddleoutEffectArgs
+    return Scattered, ScatteredConfig
 
 
 @argclass(
-    name="middleout",
-    formatter_class=arg_validators.CustomFormatter,
-    help="Text expands in a single row or column in the middle of the output area then out.",
-    description="middleout | Text expands in a single row or column in the middle of the output area then out.",
+    name="scattered",
+    help="Move the characters into place from random starting locations.",
+    description="scattered | Move the characters into place from random starting locations.",
     epilog=f"""{arg_validators.EASING_EPILOG}
-Example: terminaltexteffects middleout --starting-color 8A008A --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --expand-direction vertical --center-movement-speed 0.35 --full-movement-speed 0.35 --center-easing IN_OUT_SINE --full-easing IN_OUT_SINE""",
+Example: terminaltexteffects scattered --final-gradient-stops ff9048 ab9dff bdffea --final-gradient-steps 12 --final-gradient-frames 12 --movement-speed 0.5 --movement-easing IN_OUT_BACK""",
 )
 @dataclass
-class MiddleoutEffectArgs(ArgsDataClass):
-    starting_color: graphics.Color = ArgField(
-        cmd_name="--starting-color",
-        type_parser=arg_validators.Color.type_parser,
-        default="ffffff",
-        metavar=arg_validators.Color.METAVAR,
-        help="Color for the initial text in the center of the output area.",
-    )  # type: ignore[assignment]
+class ScatteredConfig(ArgsDataClass):
+    """Configuration for the effect.
+
+    Attributes:
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_frames (int): Number of frames to display each gradient step.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        movement_speed (float): Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
+        movement_easing (easing.EasingFunction): Easing function to use for character movement."""
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name="--final-gradient-stops",
+        cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
-        default=("8A008A", "00D1FF", "FFFFFF"),
+        default=("ff9048", "ab9dff", "bdffea"),
         metavar=arg_validators.Color.METAVAR,
-        help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
+        help="Space separated, unquoted, list of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
-        nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
-        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
+        help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
+    final_gradient_frames: int = ArgField(
+        cmd_name="--final-gradient-frames",
+        type_parser=arg_validators.PositiveInt.type_parser,
+        default=12,
+        metavar=arg_validators.PositiveInt.METAVAR,
+        help="Number of frames to display each gradient step.",
+    )  # type: ignore[assignment]
+    "int : Number of frames to display each gradient step."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
-    expand_direction: str = ArgField(
-        cmd_name="--expand-direction",
-        default="vertical",
-        choices=["vertical", "horizontal"],
-        help="Direction the text will expand.",
-    )  # type: ignore[assignment]
-    center_movement_speed: float = ArgField(
-        cmd_name="--center-movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.35,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Speed of the characters during the initial expansion of the center vertical/horiztonal line. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
-    )  # type: ignore[assignment]
-    full_movement_speed: float = ArgField(
-        cmd_name="--full-movement-speed",
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
+    movement_speed: float = ArgField(
+        cmd_name="--movement-speed",
         type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.35,
+        default=0.3,
         metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Speed of the characters during the final full expansion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+        help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
     )  # type: ignore[assignment]
-    center_easing: typing.Callable = ArgField(
-        cmd_name="--center-easing",
-        default=easing.in_out_sine,
-        type_parser=arg_validators.Ease.type_parser,
-        help="Easing function to use for initial expansion.",
-    )  # type: ignore[assignment]
-    full_easing: typing.Callable = ArgField(
-        cmd_name="--full-easing",
-        default=easing.in_out_sine,
+    "float : Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+
+    movement_easing: easing.EasingFunction = ArgField(
+        cmd_name="--movement-easing",
+        default=easing.in_out_back,
         type_parser=arg_validators.Ease.type_parser,
-        help="Easing function to use for full expansion.",
+        help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
-        return MiddleoutEffect
+        return Scattered
+
 
+class ScatteredIterator(BaseEffectIterator[ScatteredConfig]):
+    """Effect that moves the characters into position from random starting locations."""
 
-class MiddleoutEffect:
-    """Effect that expands a single row and column followed by the rest of the output area"""
+    def __init__(self, effect: "Scattered") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
 
-    def __init__(self, terminal: Terminal, args: MiddleoutEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-            character.motion.set_coordinate(self.terminal.output_area.center)
-            # setup waypoints
-            if self.args.expand_direction == "vertical":
-                column = character.input_coord.column
-                row = self.terminal.output_area.center_row
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+            if self._terminal.output_area.right < 2 or self._terminal.output_area.top < 2:
+                character.motion.set_coordinate(Coord(1, 1))
             else:
-                column = self.terminal.output_area.center_column
-                row = character.input_coord.row
-            center_path = character.motion.new_path(speed=self.args.center_movement_speed, ease=self.args.center_easing)
-            center_path.new_waypoint(Coord(column, row))
-            full_path = character.motion.new_path(
-                id="full", speed=self.args.full_movement_speed, ease=self.args.full_easing
+                character.motion.set_coordinate(self._terminal.output_area.random_coord())
+            input_coord_path = character.motion.new_path(
+                speed=self._config.movement_speed, ease=self._config.movement_easing
             )
-            full_path.new_waypoint(character.input_coord, id="full")
-
-            # setup scenes
-            full_scene = character.animation.new_scene(id="full")
-            full_gradient = graphics.Gradient(
-                self.args.starting_color, self.character_final_color_map[character], steps=10
+            input_coord_path.new_waypoint(character.input_coord)
+            character.event_handler.register_event(
+                EventHandler.Event.PATH_ACTIVATED, input_coord_path, EventHandler.Action.SET_LAYER, 1
+            )
+            character.event_handler.register_event(
+                EventHandler.Event.PATH_COMPLETE, input_coord_path, EventHandler.Action.SET_LAYER, 0
+            )
+            character.motion.activate_path(input_coord_path)
+            self._terminal.set_character_visibility(character, True)
+            gradient_scn = character.animation.new_scene()
+            char_gradient = graphics.Gradient(
+                final_gradient.spectrum[0], self._character_final_color_map[character], steps=10
+            )
+            gradient_scn.apply_gradient_to_symbols(
+                char_gradient, character.input_symbol, self._config.final_gradient_frames
             )
-            full_scene.apply_gradient_to_symbols(full_gradient, character.input_symbol, 10)
+            character.animation.activate_scene(gradient_scn)
+            self._active_chars.append(character)
+        self._initial_hold_frames = 25
+
+    def __next__(self) -> str:
+        if self._pending_chars or self._active_chars:
+            if self._initial_hold_frames:
+                self._initial_hold_frames -= 1
+                return self._terminal.get_formatted_output_string()
+            for character in self._active_chars:
+                character.tick()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class Scattered(BaseEffect[ScatteredConfig]):
+    """Effect that moves the characters into position from random starting locations."""
+
+    _config_cls = ScatteredConfig
+    _iterator_cls = ScatteredIterator
 
-            # initialize character state
-            character.motion.activate_path(center_path)
-            character.animation.set_appearance(character.input_symbol, self.args.starting_color)
-            self.terminal.set_character_visibility(character, True)
-            self.active_chars.append(character)
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        final = False
-        while self.pending_chars or self.active_chars:
-            if all([character.motion.active_path is None for character in self.active_chars]):
-                final = True
-                for character in self.active_chars:
-                    character.motion.activate_path(character.motion.query_path("full"))
-                    character.animation.activate_scene(character.animation.query_scene("full"))
-            self.terminal.print()
-            self.animate_chars()
-            if final:
-                self.active_chars = [character for character in self.active_chars if character.is_active]
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method."""
-        for character in self.active_chars:
-            character.tick()
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_orbittingvolley.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_slide.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,266 +1,252 @@
 import typing
 from dataclasses import dataclass
-from itertools import cycle
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.utils import easing, graphics
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
-from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return OrbittingVolleyEffect, OrbittingVolleyEffectArgs
+    return Slide, SlideConfig
 
 
 @argclass(
-    name="orbittingvolley",
-    formatter_class=arg_validators.CustomFormatter,
-    help="Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.",
-    description="orbittingvolley | Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.",
+    name="slide",
+    help="Slide characters into view from outside the terminal.",
+    description="slide | Slide characters into view from outside the terminal, grouped by row, column, or diagonal.",
     epilog=f"""{arg_validators.EASING_EPILOG}
-    
-Example: terminaltexteffects orbittingvolley --top-launcher-symbol █ --right-launcher-symbol █ --bottom-launcher-symbol █ --left-launcher-symbol █ --final-gradient-stops FFA15C 44D492 --final-gradient-steps 12 --launcher-movement-speed 0.5 --character-movement-speed 1 --volley-size 0.03 --launch-delay 50 --character-easing OUT_SINE""",
+Example: terminaltexteffects slide --movement-speed 0.5 --grouping row --final-gradient-stops 833ab4 fd1d1d fcb045 --final-gradient-steps 12 --final-gradient-frames 10 --final-gradient-direction vertical --gap 3 --reverse-direction --merge --movement-easing OUT_QUAD""",
 )
 @dataclass
-class OrbittingVolleyEffectArgs(ArgsDataClass):
-    top_launcher_symbol: str = ArgField(
-        cmd_name="--top-launcher-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
-        default="█",
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Symbol for the top launcher.",
-    )  # type: ignore[assignment]
-    right_launcher_symbol: str = ArgField(
-        cmd_name="--right-launcher-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
-        default="█",
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Symbol for the right launcher.",
-    )  # type: ignore[assignment]
-    bottom_launcher_symbol: str = ArgField(
-        cmd_name="--bottom-launcher-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
-        default="█",
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Symbol for the bottom launcher.",
+class SlideConfig(ArgsDataClass):
+    """Configuration for the Slide effect.
+
+    Attributes:
+        movement_speed (float): Speed of the characters.
+        grouping (str): Direction to group characters.
+        final_gradient_stops (tuple[int | str, ...]): Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_frames (int): Number of frames to display each gradient step.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient.
+        gap (int): Number of frames to wait before adding the next group of characters. Increasing this value creates a more staggered effect.
+        reverse_direction (bool): Reverse the direction of the characters.
+        merge (bool): Merge the character groups originating"""
+
+    movement_speed: float = ArgField(
+        cmd_name="--movement-speed",
+        type_parser=arg_validators.PositiveFloat.type_parser,
+        default=0.5,
+        metavar=arg_validators.PositiveFloat.METAVAR,
+        help="Speed of the characters.",
     )  # type: ignore[assignment]
-    left_launcher_symbol: str = ArgField(
-        cmd_name="--left-launcher-symbol",
-        type_parser=arg_validators.Symbol.type_parser,
-        default="█",
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Symbol for the left launcher.",
+    "float : Speed of the characters."
+
+    grouping: str = ArgField(
+        cmd_name="--grouping",
+        default="row",
+        choices=["row", "column", "diagonal"],
+        help="Direction to group characters.",
     )  # type: ignore[assignment]
-    final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name="--final-gradient-stops",
+    "str : Direction to group characters."
+
+    final_gradient_stops: tuple[int | str, ...] = ArgField(
+        cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
-        default=("FFA15C", "44D492"),
+        default=("833ab4", "fd1d1d", "fcb045"),
         metavar=arg_validators.Color.METAVAR,
-        help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
+        help="Space separated, unquoted, list of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[int | str, ...] : Tuple of colors for the character gradient. If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
-        nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
-        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
+        help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
+    final_gradient_frames: int = ArgField(
+        cmd_name="--final-gradient-frames",
+        type_parser=arg_validators.PositiveInt.type_parser,
+        default=10,
+        metavar=arg_validators.PositiveInt.METAVAR,
+        help="Number of frames to display each gradient step.",
+    )  # type: ignore[assignment]
+    "int : Number of frames to display each gradient step."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
+        default=graphics.Gradient.Direction.VERTICAL,
         type_parser=arg_validators.GradientDirection.type_parser,
-        default=graphics.Gradient.Direction.CENTER,
-        metavar=arg_validators.GradientDirection.METAVAR,
-        help="Direction of the gradient for the final color.",
-    )  # type: ignore[assignment]
-    launcher_movement_speed: float = ArgField(
-        cmd_name="--launcher-movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.5,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Orbitting speed of the launchers.",
-    )  # type: ignore[assignment]
-    character_movement_speed: float = ArgField(
-        cmd_name="--character-movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
-        default=1,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Speed of the launched characters.",
+        help="Direction of the gradient (vertical, horizontal, diagonal, center).",
     )  # type: ignore[assignment]
-    volley_size: float = ArgField(
-        cmd_name="--volley-size",
-        type_parser=arg_validators.Ratio.type_parser,
-        default=0.03,
-        metavar=arg_validators.Ratio.METAVAR,
-        help="Percent of total input characters each launcher will fire per volley. Lower limit of one character.",
-    )  # type: ignore[assignment]
-    launch_delay: int = ArgField(
-        cmd_name="--launch-delay",
+    "graphics.Gradient.Direction : Direction of the gradient."
+
+    gap: int = ArgField(
+        cmd_name="--gap",
         type_parser=arg_validators.NonNegativeInt.type_parser,
-        default=50,
+        default=3,
         metavar=arg_validators.NonNegativeInt.METAVAR,
-        help="Number of animation ticks to wait between volleys of characters.",
+        help="Number of frames to wait before adding the next group of characters. Increasing this value creates a more staggered effect.",
+    )  # type: ignore[assignment]
+    "int : Number of frames to wait before adding the next group of characters. Increasing this value creates a more staggered effect."
+
+    reverse_direction: bool = ArgField(
+        cmd_name="--reverse-direction",
+        action="store_true",
+        help="Reverse the direction of the characters.",
+    )  # type: ignore[assignment]
+    "bool : Reverse the direction of the characters."
+
+    merge: bool = ArgField(
+        cmd_name="--merge",
+        action="store_true",
+        help="Merge the character groups originating from either side of the terminal. (--reverse-direction is ignored when merging)",
     )  # type: ignore[assignment]
-    character_easing: typing.Callable = ArgField(
-        cmd_name=["--character-easing"],
-        default=easing.out_sine,
+    "bool : Merge the character groups originating from either side of the terminal."
+
+    movement_easing: easing.EasingFunction = ArgField(
+        cmd_name=["--movement-easing"],
+        default=easing.in_out_quad,
         type_parser=arg_validators.Ease.type_parser,
         metavar=arg_validators.Ease.METAVAR,
-        help="Easing function to use for launched character movement.",
+        help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
-        return OrbittingVolleyEffect
-
-
-class Launcher:
-    def __init__(self, terminal: Terminal, args: OrbittingVolleyEffectArgs, starting_edge_coord: Coord, symbol: str):
-        self.terminal = terminal
-        self.args = args
-        self.character = self.terminal.add_character(symbol, starting_edge_coord)
-        self.magazine: list[EffectCharacter] = []
-
-    def build_paths(self) -> None:
-        waypoints = [
-            Coord(self.terminal.output_area.left, self.terminal.output_area.top),
-            Coord(self.terminal.output_area.right, self.terminal.output_area.top),
-        ]
-
-        waypoint_start_index = waypoints.index(self.character.input_coord)
-        perimeter_path = self.character.motion.new_path(
-            speed=self.args.launcher_movement_speed, id="perimeter", layer=2
-        )
-        for waypoint in waypoints[waypoint_start_index:] + waypoints[:waypoint_start_index]:
-            perimeter_path.new_waypoint(waypoint)
+        return Slide
 
-    def launch(self) -> EffectCharacter | None:
-        if self.magazine:
-            next_char = self.magazine.pop(0)
-            next_char.motion.set_coordinate(self.character.motion.current_coord)
-            input_path = next_char.motion.query_path("input_path")
-            next_char.motion.activate_path(input_path)
-            self.terminal.set_character_visibility(next_char, True)
-        else:
-            next_char = None
-        return next_char
 
+class SlideIterator(BaseEffectIterator[SlideConfig]):
+    """Effect that slides characters into view from outside the terminal. Characters are grouped by column, row, or diagonal."""
 
-class OrbittingVolleyEffect:
-    def __init__(self, terminal: Terminal, args: OrbittingVolleyEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self.final_gradient_coordinate_map: dict[Coord, graphics.Color] = (
-            self.final_gradient.build_coordinate_color_mapping(
-                self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
-            )
+    def __init__(self, effect: "Slide") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._pending_groups: list[list[EffectCharacter]] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
+
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+        final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
 
-    def prepare_data(self) -> None:
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = self.final_gradient_coordinate_map[character.input_coord]
-            input_path = character.motion.new_path(
-                speed=self.args.character_movement_speed, ease=self.args.character_easing, id="input_path", layer=1
+        groups: list[list[EffectCharacter]] = []
+        if self._config.grouping == "row":
+            groups = self._terminal.get_characters_grouped(self._terminal.CharacterGroup.ROW_TOP_TO_BOTTOM)
+        elif self._config.grouping == "column":
+            groups = self._terminal.get_characters_grouped(self._terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT)
+        elif self._config.grouping == "diagonal":
+            groups = self._terminal.get_characters_grouped(
+                self._terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT
             )
-            input_path.new_waypoint(character.input_coord)
-            character.animation.set_appearance(character.input_symbol, self.character_final_color_map[character])
-
-    def set_launcher_coordinates(self, parent: Launcher, child: Launcher) -> None:
-        """Sets the coordinates for the child launcher."""
-        parent_progress = parent.character.motion.current_coord.column / self.terminal.output_area.right
-        if child.character.input_coord == Coord(self.terminal.output_area.right, self.terminal.output_area.top):
-            child_row = self.terminal.output_area.top - int((self.terminal.output_area.top * parent_progress))
-            child.character.motion.set_coordinate(Coord(self.terminal.output_area.right, max(1, child_row)))
-        elif child.character.input_coord == Coord(self.terminal.output_area.right, self.terminal.output_area.bottom):
-            child_column = self.terminal.output_area.right - int((self.terminal.output_area.right * parent_progress))
-            child.character.motion.set_coordinate(Coord(max(1, child_column), self.terminal.output_area.bottom))
-        elif child.character.input_coord == Coord(self.terminal.output_area.left, self.terminal.output_area.bottom):
-            child_row = self.terminal.output_area.bottom + int((self.terminal.output_area.top * parent_progress))
-            child.character.motion.set_coordinate(
-                Coord(self.terminal.output_area.left, min(self.terminal.output_area.top, child_row))
-            )
-        color = self.final_gradient_coordinate_map[child.character.motion.current_coord]
-        child.character.animation.set_appearance(child.character.input_symbol, color)
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        launchers: list[Launcher] = []
-        for coord, symbol in (
-            (
-                Coord(self.terminal.output_area.left, self.terminal.output_area.top),
-                self.args.top_launcher_symbol,
-            ),
-            (
-                Coord(self.terminal.output_area.right, self.terminal.output_area.top),
-                self.args.right_launcher_symbol,
-            ),
-            (
-                Coord(self.terminal.output_area.right, self.terminal.output_area.bottom),
-                self.args.bottom_launcher_symbol,
-            ),
-            (
-                Coord(self.terminal.output_area.left, self.terminal.output_area.bottom),
-                self.args.left_launcher_symbol,
-            ),
-        ):
-            launcher = Launcher(self.terminal, self.args, coord, symbol)
-            launcher.character.layer = 2
-            self.terminal.set_character_visibility(launcher.character, True)
-            self.active_chars.append(launcher.character)
-            launchers.append(launcher)
-        main_launcher = launchers[0]
-        main_launcher.character.animation.set_appearance(
-            main_launcher.character.input_symbol, self.final_gradient.spectrum[-1]
-        )
-        main_launcher.build_paths()
-        main_launcher.character.motion.activate_path(main_launcher.character.motion.query_path("perimeter"))
-        sorted_chars = []
-        for char_list in self.terminal.get_characters_grouped(Terminal.CharacterGroup.CENTER_TO_OUTSIDE_DIAMONDS):
-            sorted_chars.extend(char_list)
-        for launcher, character in zip(cycle(launchers), sorted_chars):
-            launcher.magazine.append(character)
-        delay = 0
-        while any([launcher.magazine for launcher in launchers]) or len(self.active_chars) > 1:
-            if main_launcher.character.motion.active_path is None:
-                perimeter_path = main_launcher.character.motion.query_path("perimeter")
-                main_launcher.character.motion.set_coordinate(perimeter_path.waypoints[0].coord)
-                main_launcher.character.motion.activate_path(perimeter_path)
-                self.active_chars.append(main_launcher.character)
-            main_launcher.character.animation.set_appearance(
-                self.args.top_launcher_symbol,
-                self.final_gradient_coordinate_map[main_launcher.character.motion.current_coord],
-            )
-            for launcher in launchers[1:]:
-                self.set_launcher_coordinates(main_launcher, launcher)
-            if not delay:
-                for launcher in launchers:
-                    characters_to_launch = max(
-                        int((self.args.volley_size * len(self.terminal._input_characters)) / 4), 1
+        for group in groups:
+            for character in group:
+                input_path = character.motion.new_path(
+                    id="input_path", speed=self._config.movement_speed, ease=self._config.movement_easing
+                )
+                input_path.new_waypoint(character.input_coord)
+
+        for group_index, group in enumerate(groups):
+            if self._config.grouping == "row":
+                if self._config.merge and group_index % 2 == 0:
+                    starting_column = self._terminal.output_area.right + 1
+                else:
+                    groups[group_index] = groups[group_index][::-1]
+                    starting_column = self._terminal.output_area.left - 1
+                if self._config.reverse_direction and not self._config.merge:
+                    groups[group_index] = groups[group_index][::-1]
+                    starting_column = self._terminal.output_area.right + 1
+                for character in groups[group_index]:
+                    character.motion.set_coordinate(geometry.Coord(starting_column, character.input_coord.row))
+            elif self._config.grouping == "column":
+                if self._config.merge and group_index % 2 == 0:
+                    starting_row = self._terminal.output_area.bottom - 1
+                else:
+                    groups[group_index] = groups[group_index][::-1]
+                    starting_row = self._terminal.output_area.top + 1
+                if self._config.reverse_direction and not self._config.merge:
+                    groups[group_index] = groups[group_index][::-1]
+                    starting_row = self._terminal.output_area.bottom - 1
+                for character in groups[group_index]:
+                    character.motion.set_coordinate(geometry.Coord(character.input_coord.column, starting_row))
+            if self._config.grouping == "diagonal":
+                distance_from_outside_bottom = group[-1].input_coord.row - (self._terminal.output_area.bottom - 1)
+                starting_coord = geometry.Coord(
+                    group[-1].input_coord.column - distance_from_outside_bottom,
+                    group[-1].input_coord.row - distance_from_outside_bottom,
+                )
+                if self._config.merge and group_index % 2 == 0:
+                    groups[group_index] = groups[group_index][::-1]
+                    distance_from_outside = (self._terminal.output_area.top + 1) - group[0].input_coord.row
+                    starting_coord = geometry.Coord(
+                        group[0].input_coord.column + distance_from_outside,
+                        group[0].input_coord.row + distance_from_outside,
+                    )
+                if self._config.reverse_direction and not self._config.merge:
+                    groups[group_index] = groups[group_index][::-1]
+                    distance_from_outside = (self._terminal.output_area.top + 1) - group[0].input_coord.row
+                    starting_coord = geometry.Coord(
+                        group[0].input_coord.column + distance_from_outside,
+                        group[0].input_coord.row + distance_from_outside,
                     )
-                    for _ in range(characters_to_launch):
-                        next_char = launcher.launch()
-                        if next_char:
-                            self.active_chars.append(next_char)
-                delay = self.args.launch_delay
+
+                for character in groups[group_index]:
+                    character.motion.set_coordinate(starting_coord)
+            for character in group:
+                gradient_scn = character.animation.new_scene()
+                char_gradient = graphics.Gradient(
+                    self._config.final_gradient_stops[0], self._character_final_color_map[character], steps=10
+                )
+                gradient_scn.apply_gradient_to_symbols(
+                    char_gradient, character.input_symbol, self._config.final_gradient_frames
+                )
+                character.animation.activate_scene(gradient_scn)
+
+        self._pending_groups = groups
+        self._active_groups: list[list[EffectCharacter]] = []
+        self._current_gap = 0
+
+    def __next__(self) -> str:
+        if self._pending_groups or self._active_chars or self._active_groups:
+            if self._current_gap == self._config.gap and self._pending_groups:
+                self._active_groups.append(self._pending_groups.pop(0))
+                self._current_gap = 0
             else:
-                delay -= 1
+                if self._pending_groups:
+                    self._current_gap += 1
+            for group in self._active_groups:
+                if group:
+                    next_char = group.pop(0)
+                    self._terminal.set_character_visibility(next_char, True)
+                    next_char.motion.activate_path(next_char.motion.paths["input_path"])
+                    self._active_chars.append(next_char)
+            self._active_groups = [group for group in self._active_groups if group]
+            for character in self._active_chars:
+                character.tick()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class Slide(BaseEffect[SlideConfig]):
+    """Effect that slides characters into view from outside the terminal. Characters are grouped by column, row, or diagonal."""
+
+    _config_cls = SlideConfig
+    _iterator_cls = SlideIterator
 
-            self.terminal.print()
-            self.animate_chars()
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-        for launcher in launchers:
-            self.terminal.set_character_visibility(launcher.character, False)
-            self.terminal.print()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_pour.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_rain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,204 +1,185 @@
-"""Effect that pours the characters into position from the top, bottom, left, or right."""
+"""Creates a rain effect where characters fall from the top of the terminal."""
 
+import random
 import typing
 from dataclasses import dataclass
-from enum import Enum, auto
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return PourEffect, PourEffectArgs
+    return Rain, RainConfig
 
 
 @argclass(
-    name="pour",
-    formatter_class=arg_validators.CustomFormatter,
-    help="Pours the characters into position from the given direction.",
-    description="pour | Pours the characters into position from the given direction.",
-    epilog=f"""{arg_validators.EASING_EPILOG}
-Example: terminaltexteffects pour --pour-direction down --movement-speed 0.2 --gap 1 --starting-color FFFFFF --final-gradient-stops 8A008A 00D1FF FFFFFF --easing IN_QUAD""",
+    name="rain",
+    help="Rain characters from the top of the output area.",
+    description="rain | Rain characters from the top of the output area.",
+    epilog=f"""{arg_validators.EASING_EPILOG} 
+Example: terminaltexteffects rain --rain-symbols o . , "*" "|" --rain-colors 00315C 004C8F 0075DB 3F91D9 78B9F2 9AC8F5 B8D8F8 E3EFFC --final-gradient-stops 488bff b2e7de 57eaf7 --final-gradient-steps 12 --movement-speed 0.1-0.2 --easing IN_QUART""",
 )
 @dataclass
-class PourEffectArgs(ArgsDataClass):
-    pour_direction: str = ArgField(
-        cmd_name=["--pour-direction"],
-        default="down",
-        choices=["up", "down", "left", "right"],
-        help="Direction the text will pour.",
-    )  # type: ignore[assignment]
-    pour_speed: int = ArgField(
-        cmd_name="--pour-speed",
-        type_parser=arg_validators.PositiveInt.type_parser,
-        default=1,
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Number of characters poured in per tick. Increase to speed up the effect.",
-    )  # type: ignore[assignment]
-    movement_speed: float = ArgField(
-        cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.2,
-        metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
-    )  # type: ignore[assignment]
-    gap: int = ArgField(
-        cmd_name="--gap",
-        type_parser=arg_validators.NonNegativeInt.type_parser,
-        default=1,
-        metavar=arg_validators.NonNegativeInt.METAVAR,
-        help="Number of frames to wait between each character in the pour effect. Increase to slow down effect and create a more defined back and forth motion.",
-    )  # type: ignore[assignment]
-    starting_color: graphics.Color = ArgField(
-        cmd_name=["--starting-color"],
+class RainConfig(ArgsDataClass):
+    """Configuration for the Rain effect.
+
+    Attributes:
+        rain_colors (tuple[graphics.Color, ...]): Tuple of colors for the rain drops. Colors are randomly chosen from the tuple.
+        movement_speed (tuple[float, float]): Falling speed range of the rain drops.
+        rain_symbols (tuple[str, ...]): Tuple of symbols to use for the rain drops. Symbols are randomly chosen from the tuple.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        easing (typing.Callable): Easing function to use for character movement."""
+
+    rain_colors: tuple[graphics.Color, ...] = ArgField(
+        cmd_name=["--rain-colors"],
         type_parser=arg_validators.Color.type_parser,
-        default="ffffff",
         metavar=arg_validators.Color.METAVAR,
-        help="Color of the characters before the gradient starts.",
+        nargs="+",
+        default=("00315C", "004C8F", "0075DB", "3F91D9", "78B9F2", "9AC8F5", "B8D8F8", "E3EFFC"),
+        help="List of colors for the rain drops. Colors are randomly chosen from the list.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the rain drops. Colors are randomly chosen from the tuple."
+
+    movement_speed: tuple[float, float] = ArgField(
+        cmd_name="--movement-speed",
+        type_parser=arg_validators.PositiveFloatRange.type_parser,
+        default=(0.1, 0.2),
+        metavar=arg_validators.PositiveFloatRange.METAVAR,
+        help="Falling speed range of the rain drops.",
+    )  # type: ignore[assignment]
+    "tuple[float, float] : Falling speed range of the rain drops."
+
+    rain_symbols: tuple[str, ...] = ArgField(
+        cmd_name="--rain-symbols",
+        type_parser=arg_validators.Symbol.type_parser,
+        nargs="+",
+        default=("o", ".", ",", "*", "|"),
+        metavar=arg_validators.Symbol.METAVAR,
+        help="Space separated list of symbols to use for the rain drops. Symbols are randomly chosen from the list.",
+    )  # type: ignore[assignment]
+    "tuple[str, ...] : Tuple of symbols to use for the rain drops. Symbols are randomly chosen from the tuple."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name=["--final-gradient-stops"],
+        cmd_name="--final-gradient-stops",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
-        default=("8A008A", "00D1FF", "FFFFFF"),
+        default=("488bff", "b2e7de", "57eaf7"),
         metavar=arg_validators.Color.METAVAR,
-        help="Space separated, unquoted, list of colors for the character gradient. If only one color is provided, the characters will be displayed in that color.",
+        help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name=["--final-gradient-steps"],
+        cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
+        nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
-        help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
-    )  # type: ignore[assignment]
-    final_gradient_frames: int = ArgField(
-        cmd_name=["--final-gradient-frames"],
-        type_parser=arg_validators.PositiveInt.type_parser,
-        default=10,
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Number of frames to display each gradient step.",
+        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
-        default=graphics.Gradient.Direction.VERTICAL,
+        default=graphics.Gradient.Direction.DIAGONAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
-    easing: typing.Callable = ArgField(
-        cmd_name="--easing",
-        default=easing.in_quad,
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
+    movement_easing: easing.EasingFunction = ArgField(
+        cmd_name=["--movement-easing"],
+        default=easing.in_quart,
         type_parser=arg_validators.Ease.type_parser,
+        metavar=arg_validators.Ease.METAVAR,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
-        return PourEffect
+        return Rain
 
 
-class PourDirection(Enum):
-    UP = auto()
-    DOWN = auto()
-    LEFT = auto()
-    RIGHT = auto()
-
-
-class PourEffect:
-    """Effect that pours the characters into position from the top, bottom, left, or right."""
-
-    def __init__(self, terminal: Terminal, args: PourEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_groups: list[list[EffectCharacter]] = []
-        self.active_characters: list[EffectCharacter] = []
-        self.pour_direction = {
-            "down": PourDirection.DOWN,
-            "up": PourDirection.UP,
-            "left": PourDirection.LEFT,
-            "right": PourDirection.RIGHT,
-        }.get(args.pour_direction, PourDirection.DOWN)
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by sorting the characters by the pour direction."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+class RainIterator(BaseEffectIterator[RainConfig]):
+    def __init__(self, effect: "Rain") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._group_by_row: dict[int, list[EffectCharacter | None]] = {}
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
+
+    def _build(self) -> None:
+        """Prepares the data for the effect by setting all characters y position to the input height and sorting by target y."""
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        sort_map = {
-            PourDirection.DOWN: Terminal.CharacterGroup.ROW_BOTTOM_TO_TOP,
-            PourDirection.UP: Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM,
-            PourDirection.LEFT: Terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT,
-            PourDirection.RIGHT: Terminal.CharacterGroup.COLUMN_RIGHT_TO_LEFT,
-        }
-        groups = self.terminal.get_characters_grouped(grouping=sort_map[self.pour_direction])
-        for i, group in enumerate(groups):
-            for character in group:
-                self.terminal.set_character_visibility(character, False)
-                if self.pour_direction == PourDirection.DOWN:
-                    character.motion.set_coordinate(Coord(character.input_coord.column, self.terminal.output_area.top))
-                elif self.pour_direction == PourDirection.UP:
-                    character.motion.set_coordinate(
-                        Coord(character.input_coord.column, self.terminal.output_area.bottom)
-                    )
-                elif self.pour_direction == PourDirection.LEFT:
-                    character.motion.set_coordinate(Coord(self.terminal.output_area.right, character.input_coord.row))
-                elif self.pour_direction == PourDirection.RIGHT:
-                    character.motion.set_coordinate(Coord(self.terminal.output_area.left, character.input_coord.row))
-                input_coord_path = character.motion.new_path(
-                    speed=self.args.movement_speed,
-                    ease=self.args.easing,
-                )
-                input_coord_path.new_waypoint(character.input_coord)
-                character.motion.activate_path(input_coord_path)
-
-                pour_gradient = graphics.Gradient(
-                    self.args.starting_color,
-                    self.character_final_color_map[character],
-                    steps=self.args.final_gradient_steps,
-                )
-                pour_scn = character.animation.new_scene()
-                pour_scn.apply_gradient_to_symbols(
-                    pour_gradient, character.input_symbol, self.args.final_gradient_frames
-                )
-                character.animation.activate_scene(pour_scn)
-            if i % 2 == 0:
-                self.pending_groups.append(group)
-            else:
-                self.pending_groups.append(group[::-1])
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        self.terminal.print()
-        current_group = self.pending_groups.pop(0)
-        gap = 0
-        while self.pending_groups or self.active_characters or current_group:
-            if not current_group:
-                if self.pending_groups:
-                    current_group = self.pending_groups.pop(0)
-            if current_group:
-                if not gap:
-                    for _ in range(self.args.pour_speed):
-                        if current_group:
-                            next_character = current_group.pop(0)
-                            self.terminal.set_character_visibility(next_character, True)
-                            self.active_characters.append(next_character)
-                    gap = self.args.gap
-                else:
-                    gap -= 1
-            self.animate_chars()
-            self.active_characters = [character for character in self.active_characters if character.is_active]
-            self.terminal.print()
-
-    def animate_chars(self) -> None:
-        """Animates the sliding characters."""
-        for character in self.active_characters:
-            character.tick()
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+
+        for character in self._terminal.get_characters():
+            raindrop_color = random.choice(self._config.rain_colors)
+            rain_scn = character.animation.new_scene()
+            rain_scn.add_frame(random.choice(self._config.rain_symbols), 1, color=raindrop_color)
+            raindrop_gradient = graphics.Gradient(raindrop_color, self._character_final_color_map[character], steps=7)
+            fade_scn = character.animation.new_scene()
+            fade_scn.apply_gradient_to_symbols(raindrop_gradient, character.input_symbol, 5)
+            character.animation.activate_scene(rain_scn)
+            character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.top))
+            input_path = character.motion.new_path(
+                speed=random.uniform(self._config.movement_speed[0], self._config.movement_speed[1]),
+                ease=self._config.movement_easing,
+            )
+            input_path.new_waypoint(character.input_coord)
+
+            character.event_handler.register_event(
+                character.event_handler.Event.PATH_COMPLETE,
+                input_path,
+                character.event_handler.Action.ACTIVATE_SCENE,
+                fade_scn,
+            )
+            character.motion.activate_path(input_path)
+            self._pending_chars.append(character)
+        for character in sorted(self._pending_chars, key=lambda c: c.input_coord.row):
+            if character.input_coord.row not in self._group_by_row:
+                self._group_by_row[character.input_coord.row] = []
+            self._group_by_row[character.input_coord.row].append(character)
+        self._pending_chars.clear()
+
+    def __next__(self) -> str:
+        if self._group_by_row or self._active_chars or self._pending_chars:
+            if not self._pending_chars and self._group_by_row:
+                self._pending_chars.extend(self._group_by_row.pop(min(self._group_by_row.keys())))  # type: ignore
+            if self._pending_chars:
+                for _ in range(random.randint(1, 3)):
+                    if self._pending_chars:
+                        next_character = self._pending_chars.pop(random.randint(0, len(self._pending_chars) - 1))
+                        self._terminal.set_character_visibility(next_character, True)
+                        self._active_chars.append(next_character)
+
+                    else:
+                        break
+            for character in self._active_chars:
+                character.tick()
+
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class Rain(BaseEffect[RainConfig]):
+    _config_cls = RainConfig
+    _iterator_cls = RainIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_print.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_verticalslice.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,206 +1,157 @@
-import random
 import typing
 from dataclasses import dataclass
 
-import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
-from terminaltexteffects.utils import easing, graphics
+from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import arg_validators, easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return PrintEffect, PrintEffectArgs
+    return VerticalSlice, VerticalSliceConfig
 
 
 @argclass(
-    name="print",
-    formatter_class=arg_validators.CustomFormatter,
-    help="Lines are printed one at a time following a print head. Print head performs line feed, carriage return.",
-    description="print | Lines are printed one at a time following a print head. Print head performs line feed, carriage return.",
+    name="verticalslice",
+    help="Slices the input in half vertically and slides it into place from opposite directions.",
+    description="verticalslice | Slices the input in half vertically and slides it into place from opposite directions.",
     epilog=f"""{arg_validators.EASING_EPILOG}
     
-Example: terminaltexteffects print --final-gradient-stops 02b8bd c1f0e3 00ffa0 --final-gradient-steps 12 --print-head-return-speed 1.25 --print-speed 1 --print-head-easing IN_OUT_QUAD""",
+Example: terminaltexteffects verticalslice --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --movement-speed 0.15 --movement-easing IN_OUT_EXPO""",
 )
 @dataclass
-class PrintEffectArgs(ArgsDataClass):
+class VerticalSliceConfig(ArgsDataClass):
+    """Configuration for the VerticalSlice effect.
+
+    Attributes:
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        movement_speed (float): Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
+        movement_easing (easing.EasingFunction): Easing function to use for character movement.
+    """
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
-        default=("02b8bd", "c1f0e3", "00ffa0"),
+        default=("8A008A", "00D1FF", "FFFFFF"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name=["--final-gradient-steps"],
+        cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
-        default=graphics.Gradient.Direction.DIAGONAL,
+        default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
-    print_head_return_speed: float = ArgField(
-        cmd_name=["--print-head-return-speed"],
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
+    movement_speed: float = ArgField(
+        cmd_name="--movement-speed",
         type_parser=arg_validators.PositiveFloat.type_parser,
-        default=1.25,
+        default=0.15,
         metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Speed of the print head when performing a carriage return.",
+        help="Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
     )  # type: ignore[assignment]
-    print_speed: int = ArgField(
-        cmd_name=["--print-speed"],
-        type_parser=arg_validators.PositiveInt.type_parser,
-        default=1,
-        metavar=arg_validators.PositiveInt.METAVAR,
-        help="Speed of the print head when printing characters.",
-    )  # type: ignore[assignment]
-    print_head_easing: typing.Callable = ArgField(
-        cmd_name=["--print-head-easing"],
-        default=easing.in_out_quad,
+    "float : Movement speed of the characters. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+
+    movement_easing: easing.EasingFunction = ArgField(
+        cmd_name="--movement-easing",
         type_parser=arg_validators.Ease.type_parser,
-        help="Easing function to use for print head movement.",
+        default=easing.in_out_expo,
+        help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for character movement."
 
     @classmethod
     def get_effect_class(cls):
-        return PrintEffect
+        return VerticalSlice
 
 
-class Row:
-    def __init__(
-        self,
-        characters: list[EffectCharacter],
-        character_final_color_map: dict[EffectCharacter, graphics.Color],
-        typing_head_color: str | int,
-    ):
-        self.untyped_chars: list[EffectCharacter] = []
-        self.typed_chars: list[EffectCharacter] = []
-        blank_row_accounted = False
-        for character in characters:
-            if character.input_symbol == " ":
-                if blank_row_accounted:
-                    continue
-                blank_row_accounted = True
-            character.motion.set_coordinate(Coord(character.input_coord.column, 1))
-            color_gradient = graphics.Gradient(typing_head_color, character_final_color_map[character], steps=5)
-            typed_animation = character.animation.new_scene()
-            typed_animation.apply_gradient_to_symbols(color_gradient, ("█", "▓", "▒", "░", character.input_symbol), 5)
-            character.animation.activate_scene(typed_animation)
-            self.untyped_chars.append(character)
-
-    def move_up(self):
-        for character in self.typed_chars:
-            current_row = character.motion.current_coord.row
-            character.motion.set_coordinate(Coord(character.motion.current_coord.column, current_row + 1))
-
-    def type_char(self) -> EffectCharacter | None:
-        if self.untyped_chars:
-            next_char = self.untyped_chars.pop(0)
-            self.typed_chars.append(next_char)
-            return next_char
-        return None
-
-
-class PrintEffect:
-    """Effect that moves a print head across the screen, printing characters, before performing a line feed and carriage return."""
-
-    def __init__(self, terminal: Terminal, args: PrintEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.pending_rows: list[Row] = []
-        self.processed_rows: list[Row] = []
-        self.typing_head = self.terminal.add_character("█", Coord(1, 1))
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+class VerticalSliceIterator(BaseEffectIterator[VerticalSliceConfig]):
+    """Effect that slices the input in half vertically and slides it into place from opposite directions."""
 
-    def prepare_data(self) -> None:
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def __init__(self, effect: "VerticalSlice") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._new_rows: list[list[EffectCharacter]] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
+
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
-        )
-        for character in self.terminal.get_characters(fill_chars=True):
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        input_rows = self.terminal.get_characters_grouped(
-            grouping=self.terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for input_row in input_rows:
-            self.pending_rows.append(
-                Row(
-                    input_row,
-                    self.character_final_color_map,
-                    self.character_final_color_map[input_row[-1]],
-                )
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+            character.animation.set_appearance(
+                character.input_symbol,
+                self._character_final_color_map[character],
             )
 
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        current_row: Row = self.pending_rows.pop(0)
-        typing = True
-        delay = 0
-        last_column = 0
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
-
-        while self.active_chars or typing:
-            if self.typing_head.motion.active_path:
-                pass
-            elif delay:
-                delay -= 1
-            else:
-                delay = random.randint(0, 0)
-                if current_row.untyped_chars:
-                    for _ in range(min(len(current_row.untyped_chars), self.args.print_speed)):
-                        next_char = current_row.type_char()
-                        if next_char:
-                            self.terminal.set_character_visibility(next_char, True)
-                            self.active_chars.append(next_char)
-                            last_column = next_char.input_coord.column
-                else:
-                    self.processed_rows.append(current_row)
-                    if self.pending_rows:
-                        for row in self.processed_rows:
-                            row.move_up()
-                        current_row = self.pending_rows.pop(0)
-                        current_row_height = current_row.untyped_chars[0].input_coord.row
-                        self.typing_head.motion.set_coordinate(Coord(last_column, 1))
-                        self.terminal.set_character_visibility(self.typing_head, True)
-                        self.typing_head.motion.paths.clear()
-                        carriage_return_path = self.typing_head.motion.new_path(
-                            speed=self.args.print_head_return_speed,
-                            ease=self.args.print_head_easing,
-                            id="carriage_return_path",
-                        )
-                        carriage_return_path.new_waypoint(Coord(1, 1))
-                        self.typing_head.motion.activate_path(carriage_return_path)
-                        self.typing_head.animation.set_appearance(
-                            self.typing_head.input_symbol,
-                            final_gradient.get_color_at_fraction(current_row_height / self.terminal.output_area.top),
-                        )
-                        self.typing_head.event_handler.register_event(
-                            EventHandler.Event.PATH_COMPLETE,
-                            carriage_return_path,
-                            EventHandler.Action.CALLBACK,
-                            EventHandler.Callback(self.terminal.set_character_visibility, False),
-                        )
-                        self.active_chars.append(self.typing_head)
-                    else:
-                        typing = False
-            self.terminal.print()
-            self.animate_chars()
-
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-        self.terminal.print()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+        self.rows = self._terminal.get_characters_grouped(grouping=self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP)
+        lengths = [max([c.input_coord.column for c in row]) for row in self.rows]
+        mid_point = sum(lengths) // len(lengths) // 2
+        for row_index, row in enumerate(self.rows):
+            new_row = []
+            left_half = [character for character in row if character.input_coord.column <= mid_point]
+            for character in left_half:
+                character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.top))
+                input_coord_path = character.motion.new_path(
+                    speed=self._config.movement_speed, ease=self._config.movement_easing
+                )
+                input_coord_path.new_waypoint(character.input_coord)
+                character.motion.activate_path(input_coord_path)
+            opposite_row = self.rows[-(row_index + 1)]
+            right_half = [c for c in opposite_row if c.input_coord.column > mid_point]
+            for character in right_half:
+                character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.bottom))
+                input_coord_path = character.motion.new_path(
+                    speed=self._config.movement_speed, ease=self._config.movement_easing
+                )
+                input_coord_path.new_waypoint(character.input_coord)
+                character.motion.activate_path(input_coord_path)
+            new_row.extend(left_half)
+            new_row.extend(right_half)
+            self._new_rows.append(new_row)
+
+    def __next__(self) -> str:
+        if self._new_rows or self._active_chars:
+            if self._new_rows:
+                next_row = self._new_rows.pop(0)
+                for character in next_row:
+                    self._terminal.set_character_visibility(character, True)
+                self._active_chars.extend(next_row)
+            for character in self._active_chars:
+                character.tick()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class VerticalSlice(BaseEffect[VerticalSliceConfig]):
+    """Effect that slices the input in half vertically and slides it into place from opposite directions."""
+
+    _config_cls = VerticalSliceConfig
+    _iterator_cls = VerticalSliceIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_rain.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_wipe.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,164 +1,171 @@
-"""Creates a rain effect where characters fall from the top of the terminal."""
-
-import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter
-from terminaltexteffects.utils import easing, graphics
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
+from terminaltexteffects.utils import graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
-from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return RainEffect, RainEffectArgs
+    return Wipe, WipeConfig
 
 
 @argclass(
-    name="rain",
-    formatter_class=arg_validators.CustomFormatter,
-    help="Rain characters from the top of the output area.",
-    description="rain | Rain characters from the top of the output area.",
-    epilog=f"""{arg_validators.EASING_EPILOG} 
-Example: terminaltexteffects rain --rain-symbols o . , "*" "|" --rain-colors 00315C 004C8F 0075DB 3F91D9 78B9F2 9AC8F5 B8D8F8 E3EFFC --final-gradient-stops 488bff b2e7de 57eaf7 --final-gradient-steps 12 --movement-speed 0.1-0.2 --easing IN_QUART""",
+    name="wipe",
+    help="Wipes the text across the terminal to reveal characters.",
+    description="wipe | Wipes the text across the terminal to reveal characters.",
+    epilog="""Example: terminaltexteffects wipe --wipe-direction diagonal_bottom_left_to_top_right --final-gradient-stops 833ab4 fd1d1d fcb045 --final-gradient-steps 12 --final-gradient-frames 5 --wipe-delay 0""",
 )
 @dataclass
-class RainEffectArgs(ArgsDataClass):
-    rain_colors: tuple[graphics.Color, ...] = ArgField(
-        cmd_name=["--rain-colors"],
-        type_parser=arg_validators.Color.type_parser,
-        metavar=arg_validators.Color.METAVAR,
-        nargs="+",
-        default=("00315C", "004C8F", "0075DB", "3F91D9", "78B9F2", "9AC8F5", "B8D8F8", "E3EFFC"),
-        help="List of colors for the rain drops. Colors are randomly chosen from the list.",
-    )  # type: ignore[assignment]
-    movement_speed: tuple[float, float] = ArgField(
-        cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloatRange.type_parser,
-        default=(0.1, 0.2),
-        metavar=arg_validators.PositiveFloatRange.METAVAR,
-        help="Falling speed range of the rain drops.",
-    )  # type: ignore[assignment]
+class WipeConfig(ArgsDataClass):
+    """Configuration for the Wipe effect.
 
-    rain_symbols: tuple[str, ...] = ArgField(
-        cmd_name="--rain-symbols",
-        type_parser=arg_validators.Symbol.type_parser,
-        nargs="+",
-        default=("o", ".", ",", "*", "|"),
-        metavar=arg_validators.Symbol.METAVAR,
-        help="Space separated list of symbols to use for the rain drops. Symbols are randomly chosen from the list.",
+    Attributes:
+        wipe_direction (str): Direction the text will wipe.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the wipe gradient.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_frames (int): Number of frames to display each gradient step.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        wipe_delay (int): Number of animation cycles to wait before adding the next character group. Increase, to slow down the effect."""
+
+    wipe_direction: str = ArgField(
+        cmd_name="--wipe-direction",
+        default="diagonal_bottom_left_to_top_right",
+        choices=[
+            "column_left_to_right",
+            "column_right_to_left",
+            "row_top_to_bottom",
+            "row_bottom_to_top",
+            "diagonal_top_left_to_bottom_right",
+            "diagonal_bottom_left_to_top_right",
+            "diagonal_top_right_to_bottom_left",
+            "diagonal_bottom_right_to_top_left",
+        ],
+        help="Direction the text will wipe.",
     )  # type: ignore[assignment]
+    "str : Direction the text will wipe. Options: column_left_to_right, column_right_to_left, row_top_to_bottom, row_bottom_to_top, diagonal_top_left_to_bottom_right, diagonal_bottom_left_to_top_right, diagonal_top_right_to_bottom_left, diagonal_bottom_right_to_top_left."
 
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--final-gradient-stops",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
-        default=("488bff", "b2e7de", "57eaf7"),
+        default=("833ab4", "fd1d1d", "fcb045"),
         metavar=arg_validators.Color.METAVAR,
-        help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
+        help="Space separated, unquoted, list of colors for the wipe gradient.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the wipe gradient."
 
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
-        help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
+        help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
+    final_gradient_frames: int = ArgField(
+        cmd_name="--final-gradient-frames",
+        type_parser=arg_validators.PositiveInt.type_parser,
+        default=5,
+        metavar=arg_validators.PositiveInt.METAVAR,
+        help="Number of frames to display each gradient step.",
+    )  # type: ignore[assignment]
+    "int : Number of frames to display each gradient step."
 
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
-        default=graphics.Gradient.Direction.DIAGONAL,
+        default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
 
-    easing: typing.Callable = ArgField(
-        cmd_name=["--easing"],
-        default=easing.in_quart,
-        type_parser=arg_validators.Ease.type_parser,
-        metavar=arg_validators.Ease.METAVAR,
-        help="Easing function to use for character movement.",
+    wipe_delay: int = ArgField(
+        cmd_name="--wipe-delay",
+        type_parser=arg_validators.NonNegativeInt.type_parser,
+        default=0,
+        metavar=arg_validators.NonNegativeInt.METAVAR,
+        help="Number of animation cycles to wait before adding the next character group. Increase, to slow down the effect.",
     )  # type: ignore[assignment]
+    "int : Number of animation cycles to wait before adding the next character group. Increase, to slow down the effect."
 
     @classmethod
     def get_effect_class(cls):
-        return RainEffect
+        return Wipe
 
 
-class RainEffect:
-    """Creates a rain effect where characters fall from the top of the output area."""
+class WipeIterator(BaseEffectIterator[WipeConfig]):
+    """Effect that performs a wipe across the terminal to reveal characters."""
 
-    def __init__(self, terminal: Terminal, args: RainEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.group_by_row: dict[int, list[EffectCharacter | None]] = {}
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by setting all characters y position to the input height and sorting by target y."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def __init__(self, effect: "Wipe") -> None:
+        super().__init__(effect)
+        self._pending_groups: list[list[EffectCharacter]] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
+
+    def _build(self) -> None:
+        direction = self._config.wipe_direction
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        sort_map = {
+            "column_left_to_right": self._terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT,
+            "column_right_to_left": self._terminal.CharacterGroup.COLUMN_RIGHT_TO_LEFT,
+            "row_top_to_bottom": self._terminal.CharacterGroup.ROW_TOP_TO_BOTTOM,
+            "row_bottom_to_top": self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP,
+            "diagonal_top_left_to_bottom_right": self._terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT,
+            "diagonal_bottom_left_to_top_right": self._terminal.CharacterGroup.DIAGONAL_BOTTOM_LEFT_TO_TOP_RIGHT,
+            "diagonal_top_right_to_bottom_left": self._terminal.CharacterGroup.DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT,
+            "diagonal_bottom_right_to_top_left": self._terminal.CharacterGroup.DIAGONAL_BOTTOM_RIGHT_TO_TOP_LEFT,
+        }
+        for group in self._terminal.get_characters_grouped(sort_map[direction]):
+            for character in group:
+                wipe_scn = character.animation.new_scene()
+                wipe_gradient = graphics.Gradient(
+                    final_gradient.spectrum[0],
+                    self._character_final_color_map[character],
+                    steps=self._config.final_gradient_steps,
+                )
+                wipe_scn.apply_gradient_to_symbols(
+                    wipe_gradient, character.input_symbol, self._config.final_gradient_frames
+                )
+                character.animation.activate_scene(wipe_scn)
+            self._pending_groups.append(group)
+        self._wipe_delay = self._config.wipe_delay
+
+    def __next__(self) -> str:
+        if self._pending_groups or self._active_chars:
+            if not self._wipe_delay:
+                if self._pending_groups:
+                    next_group = self._pending_groups.pop(0)
+                    for character in next_group:
+                        self._terminal.set_character_visibility(character, True)
+                        self._active_chars.append(character)
+                self._wipe_delay = self._config.wipe_delay
+            else:
+                self._wipe_delay -= 1
+            for character in self._active_chars:
+                character.tick()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class Wipe(BaseEffect[WipeConfig]):
+    """Effect that performs a wipe across the terminal to reveal characters."""
+
+    _config_cls = WipeConfig
+    _iterator_cls = WipeIterator
 
-        for character in self.terminal.get_characters():
-            raindrop_color = random.choice(self.args.rain_colors)
-            rain_scn = character.animation.new_scene()
-            rain_scn.add_frame(random.choice(self.args.rain_symbols), 1, color=raindrop_color)
-            raindrop_gradient = graphics.Gradient(raindrop_color, self.character_final_color_map[character], steps=7)
-            fade_scn = character.animation.new_scene()
-            fade_scn.apply_gradient_to_symbols(raindrop_gradient, character.input_symbol, 5)
-            character.animation.activate_scene(rain_scn)
-            character.motion.set_coordinate(Coord(character.input_coord.column, self.terminal.output_area.top))
-            input_path = character.motion.new_path(
-                speed=random.uniform(self.args.movement_speed[0], self.args.movement_speed[1]), ease=self.args.easing
-            )
-            input_path.new_waypoint(character.input_coord)
-
-            character.event_handler.register_event(
-                character.event_handler.Event.PATH_COMPLETE,
-                input_path,
-                character.event_handler.Action.ACTIVATE_SCENE,
-                fade_scn,
-            )
-            character.motion.activate_path(input_path)
-            self.pending_chars.append(character)
-        for character in sorted(self.pending_chars, key=lambda c: c.input_coord.row):
-            if character.input_coord.row not in self.group_by_row:
-                self.group_by_row[character.input_coord.row] = []
-            self.group_by_row[character.input_coord.row].append(character)
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        self.pending_chars.clear()
-        self.terminal.print()
-        while self.group_by_row or self.active_chars or self.pending_chars:
-            if not self.pending_chars and self.group_by_row:
-                self.pending_chars.extend(self.group_by_row.pop(min(self.group_by_row.keys())))  # type: ignore
-            if self.pending_chars:
-                for _ in range(random.randint(1, 3)):
-                    if self.pending_chars:
-                        next_character = self.pending_chars.pop(random.randint(0, len(self.pending_chars) - 1))
-                        self.terminal.set_character_visibility(next_character, True)
-                        self.active_chars.append(next_character)
-
-                    else:
-                        break
-            self.animate_chars()
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-            self.terminal.print()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method."""
-        for character in self.active_chars:
-            character.tick()
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_rings.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_rings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,355 +1,391 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, geometry, graphics, motion
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return RingsEffect, RingsEffectArgs
+    return Rings, RingsConfig
 
 
 @argclass(
     name="rings",
-    formatter_class=arg_validators.CustomFormatter,
     help="Characters are dispersed and form into spinning rings.",
     description="rings | Characters are dispersed and form into spinning rings.",
     epilog="""Example: terminaltexteffects rings --ring-colors ab48ff e7b2b2 fffebd --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --ring-gap 0.1 --spin-duration 200 --spin-speed 0.25-1.0 --disperse-duration 200 --spin-disperse-cycles 3""",
 )
 @dataclass
-class RingsEffectArgs(ArgsDataClass):
+class RingsConfig(ArgsDataClass):
+    """Configurations for the RingsEffect.
+
+    Attributes:
+        ring_colors (tuple[graphics.Color, ...]): Tuple of colors for the rings.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        ring_gap (float): Distance between rings as a percent of the smallest output area dimension.
+        spin_duration (int): Number of animation steps for each cycle of the spin phase.
+        spin_speed (tuple[float, float]): Range of speeds for the rotation of the rings. The speed is randomly selected from this range for each ring.
+        disperse_duration (int): Number of animation steps spent in the dispersed state between spinning cycles.
+        spin_disperse_cycles (int): Number of times the animation will cycles between spinning rings and dispersed characters.
+    """
+
     ring_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--ring-colors"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("ab48ff", "e7b2b2", "fffebd"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the rings.",
     )  # type: ignore[assignment]
 
+    "tuple[graphics.Color] : Tuple of colors for the rings."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("ab48ff", "e7b2b2", "fffebd"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
 
+    "tuple[graphics.Color] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
 
+    "tuple[int, ...] : Number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
 
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     ring_gap: float = ArgField(
         cmd_name=["--ring-gap"],
         type_parser=arg_validators.PositiveFloat.type_parser,
         default=0.1,
         help="Distance between rings as a percent of the smallest output area dimension.",
     )  # type: ignore[assignment]
 
+    "float : Distance between rings as a percent of the smallest output area dimension."
     spin_duration: int = ArgField(
         cmd_name=["--spin-duration"],
         type_parser=arg_validators.PositiveInt.type_parser,
         default=200,
         help="Number of animation steps for each cycle of the spin phase.",
     )  # type: ignore[assignment]
 
+    "int : Number of animation steps for each cycle of the spin phase."
+
     spin_speed: tuple[float, float] = ArgField(
         cmd_name=["--spin-speed"],
         type_parser=arg_validators.PositiveFloatRange.type_parser,
         default=(0.25, 1.0),
         metavar=arg_validators.PositiveFloatRange.METAVAR,
         help="Range of speeds for the rotation of the rings. The speed is randomly selected from this range for each ring.",
     )  # type: ignore[assignment]
 
+    "tuple[float, float] : Range of speeds for the rotation of the rings. The speed is randomly selected from this range for each ring."
+
     disperse_duration: int = ArgField(
         cmd_name=["--disperse-duration"],
         type_parser=arg_validators.PositiveInt.type_parser,
         default=200,
         help="Number of animation steps spent in the dispersed state between spinning cycles.",
     )  # type: ignore[assignment]
 
+    "int : Number of animation steps spent in the dispersed state between spinning cycles."
+
     spin_disperse_cycles: int = ArgField(
         cmd_name=["--spin-disperse-cycles"],
         type_parser=arg_validators.PositiveInt.type_parser,
         default=3,
         help="Number of times the animation will cycles between spinning rings and dispersed characters.",
     )  # type: ignore[assignment]
 
+    "int : Number of times the animation will cycles between spinning rings and dispersed characters."
+
     @classmethod
     def get_effect_class(cls):
-        return RingsEffect
+        return Rings
 
 
-class Ring:
-    def __init__(
-        self,
-        args: RingsEffectArgs,
-        radius: int,
-        origin: Coord,
-        ring_coords: list[Coord],
-        ring_gap: int,
-        ring_color: graphics.Color,
-        character_color_map: dict[EffectCharacter, graphics.Color],
-    ):
-        self.args = args
-        self.radius = radius
-        self.origin: Coord = origin
-        self.counter_clockwise_coords = ring_coords
-        self.clockwise_coords = ring_coords[::-1]
-        self.ring_gap = ring_gap
-        self.ring_color = ring_color
-        self.characters: list[EffectCharacter] = []
-        self.character_last_ring_path: dict[EffectCharacter, motion.Path] = {}
-        self.rotations = 0
-        self.rotation_speed = random.uniform(self.args.spin_speed[0], self.args.spin_speed[1])
-        self.character_color_map = character_color_map
-
-    def add_character(self, character: EffectCharacter, clockwise: int) -> None:
-        # make gradient scene
-        gradient_scn = character.animation.new_scene(id="gradient")
-        char_gradient = graphics.Gradient(self.character_color_map[character], self.ring_color, steps=8)
-        gradient_scn.apply_gradient_to_symbols(char_gradient, character.input_symbol, 5)
-
-        # make rotation waypoints
-        ring_paths: list[motion.Path] = []
-        character_starting_index = len(self.characters)
-        if clockwise:
-            coords = self.clockwise_coords
-        else:
-            coords = self.counter_clockwise_coords
-        for coord in coords[character_starting_index:] + coords[:character_starting_index]:
-            ring_path = character.motion.new_path(id=str(len(ring_paths)), speed=self.rotation_speed)
-            ring_path.new_waypoint(coord, id=str(len(ring_path.waypoints)))
-            ring_paths.append(ring_path)
-        self.character_last_ring_path[character] = ring_paths[0]
-        # make disperse scene
-        disperse_scn = character.animation.new_scene(is_looping=False, id="disperse")
-        disperse_gradient = graphics.Gradient(self.ring_color, self.character_color_map[character], steps=8)
-        disperse_scn.apply_gradient_to_symbols(disperse_gradient, character.input_symbol, 16)
-        character.motion.chain_paths(ring_paths, loop=True)
-        self.characters.append(character)
-
-    def make_disperse_waypoints(self, character: EffectCharacter, origin: Coord) -> motion.Path:
-        """Make the Path for the character to follow when the ring disperses.
-
-        Args:
-            character (EffectCharacter): Character to disperse.
-            origin (Coord): Origin coordinate for the character.
-
-        Returns:
-            motion.Path: the Path to follow.
-        """
-        disperse_coords = geometry.find_coords_in_rect(origin, self.ring_gap)
-        character.motion.paths.pop("disperse", None)
-        disperse_path = character.motion.new_path(speed=0.1, loop=True, id="disperse")
-        for _ in range(5):
-            disperse_path.new_waypoint(disperse_coords[random.randrange(0, len(disperse_coords))])
-        return disperse_path
-
-    def disperse(self) -> None:
-        """Disperse the characters from the ring."""
-        for character in self.characters:
-            if character.motion.active_path is not None:
-                self.character_last_ring_path[character] = character.motion.active_path
+class RingsIterator(BaseEffectIterator[RingsConfig]):
+    class _Ring:
+        def __init__(
+            self,
+            config: RingsConfig,
+            radius: int,
+            origin: Coord,
+            ring_coords: list[Coord],
+            ring_gap: int,
+            ring_color: graphics.Color,
+            character_color_map: dict[EffectCharacter, graphics.Color],
+        ):
+            self.config = config
+            self._built = False
+            self.radius = radius
+            self.origin: Coord = origin
+            self.counter_clockwise_coords = ring_coords
+            self.clockwise_coords = ring_coords[::-1]
+            self.ring_gap = ring_gap
+            self.ring_color = ring_color
+            self.characters: list[EffectCharacter] = []
+            self.character_last_ring_path: dict[EffectCharacter, motion.Path] = {}
+            self.rotations = 0
+            self.rotation_speed = random.uniform(self.config.spin_speed[0], self.config.spin_speed[1])
+            self.character_color_map = character_color_map
+
+        def add_character(self, character: EffectCharacter, clockwise: int) -> None:
+            # make gradient scene
+            gradient_scn = character.animation.new_scene(id="gradient")
+            char_gradient = graphics.Gradient(self.character_color_map[character], self.ring_color, steps=8)
+            gradient_scn.apply_gradient_to_symbols(char_gradient, character.input_symbol, 5)
+
+            # make rotation waypoints
+            ring_paths: list[motion.Path] = []
+            character_starting_index = len(self.characters)
+            if clockwise:
+                coords = self.clockwise_coords
             else:
-                self.character_last_ring_path[character] = character.motion.paths["0"]
-            character.motion.activate_path(self.make_disperse_waypoints(character, character.motion.current_coord))
-            character.animation.activate_scene(character.animation.query_scene("disperse"))
-
-    def spin(self) -> None:
-        for character in self.characters:
-            condense_path = character.motion.new_path(speed=0.1)
-            condense_path.new_waypoint(self.character_last_ring_path[character].waypoints[0].coord)
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_COMPLETE,
-                condense_path,
-                EventHandler.Action.ACTIVATE_PATH,
-                self.character_last_ring_path[character],
-            )
-            character.motion.activate_path(condense_path)
-            character.animation.activate_scene(character.animation.query_scene("gradient"))
-
-
-class RingsEffect:
-    """Effect that forms the characters into rings."""
+                coords = self.counter_clockwise_coords
+            for coord in coords[character_starting_index:] + coords[:character_starting_index]:
+                ring_path = character.motion.new_path(id=str(len(ring_paths)), speed=self.rotation_speed)
+                ring_path.new_waypoint(coord, id=str(len(ring_path.waypoints)))
+                ring_paths.append(ring_path)
+            self.character_last_ring_path[character] = ring_paths[0]
+            # make disperse scene
+            disperse_scn = character.animation.new_scene(is_looping=False, id="disperse")
+            disperse_gradient = graphics.Gradient(self.ring_color, self.character_color_map[character], steps=8)
+            disperse_scn.apply_gradient_to_symbols(disperse_gradient, character.input_symbol, 16)
+            character.motion.chain_paths(ring_paths, loop=True)
+            self.characters.append(character)
+
+        def make_disperse_waypoints(self, character: EffectCharacter, origin: Coord) -> motion.Path:
+            """Make the Path for the character to follow when the ring disperses.
+
+            Args:
+                character (EffectCharacter): Character to disperse.
+                origin (Coord): Origin coordinate for the character.
+
+            Returns:
+                motion.Path: the Path to follow.
+            """
+            disperse_coords = geometry.find_coords_in_rect(origin, self.ring_gap)
+            character.motion.paths.pop("disperse", None)
+            disperse_path = character.motion.new_path(speed=0.1, loop=True, id="disperse")
+            for _ in range(5):
+                disperse_path.new_waypoint(disperse_coords[random.randrange(0, len(disperse_coords))])
+            return disperse_path
+
+        def disperse(self) -> None:
+            """Disperse the characters from the ring."""
+            for character in self.characters:
+                if character.motion.active_path is not None:
+                    self.character_last_ring_path[character] = character.motion.active_path
+                else:
+                    self.character_last_ring_path[character] = character.motion.paths["0"]
+                character.motion.activate_path(self.make_disperse_waypoints(character, character.motion.current_coord))
+                character.animation.activate_scene(character.animation.query_scene("disperse"))
+
+        def spin(self) -> None:
+            for character in self.characters:
+                condense_path = character.motion.new_path(speed=0.1)
+                condense_path.new_waypoint(self.character_last_ring_path[character].waypoints[0].coord)
+                character.event_handler.register_event(
+                    EventHandler.Event.PATH_COMPLETE,
+                    condense_path,
+                    EventHandler.Action.ACTIVATE_PATH,
+                    self.character_last_ring_path[character],
+                )
+                character.motion.activate_path(condense_path)
+                character.animation.activate_scene(character.animation.query_scene("gradient"))
 
-    def __init__(self, terminal: Terminal, args: RingsEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.ring_chars: list[EffectCharacter] = []
-        self.non_ring_chars: list[EffectCharacter] = []
-        self.rings: dict[int, Ring] = {}
+    def __init__(self, effect: "Rings") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._ring_chars: list[EffectCharacter] = []
+        self._non_ring_chars: list[EffectCharacter] = []
+        self._rings: dict[int, RingsIterator._Ring] = {}
         self.ring_gap = int(
-            max(round(min(self.terminal.output_area.top, self.terminal.output_area.right) * self.args.ring_gap), 1)
+            max(round(min(self._terminal.output_area.top, self._terminal.output_area.right) * self._config.ring_gap), 1)
         )
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
 
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by building rings and associated animations/waypoints."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        self.ring_gap = int(
+            max(round(min(self._terminal.output_area.top, self._terminal.output_area.right) * self._config.ring_gap), 1)
+        )
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
             start_scn = character.animation.new_scene()
-            start_scn.add_frame(character.input_symbol, 1, color=self.character_final_color_map[character])
+            start_scn.add_frame(character.input_symbol, 1, color=self._character_final_color_map[character])
             home_path = character.motion.new_path(speed=0.8, ease=easing.out_quad, id="home")
             home_path.new_waypoint(character.input_coord)
             character.animation.activate_scene(start_scn)
-            self.terminal.set_character_visibility(character, True)
-            self.pending_chars.append(character)
+            self._terminal.set_character_visibility(character, True)
+            self._pending_chars.append(character)
 
-        random.shuffle(self.pending_chars)
+        random.shuffle(self._pending_chars)
         # make rings
-        for radius in range(1, max(self.terminal.output_area.right, self.terminal.output_area.top), self.ring_gap):
+        for radius in range(1, max(self._terminal.output_area.right, self._terminal.output_area.top), self.ring_gap):
             ring_coords = geometry.find_coords_on_circle(
-                self.terminal.output_area.center, radius, 7 * radius, unique=True
+                self._terminal.output_area.center, radius, 7 * radius, unique=True
             )
             # check if any part of the ring is in the output area, if not, stop creating rings
             if (
-                len([coord for coord in ring_coords if self.terminal.output_area.coord_is_in_output_area(coord)])
+                len([coord for coord in ring_coords if self._terminal.output_area.coord_is_in_output_area(coord)])
                 / len(ring_coords)
                 < 0.25
             ):
                 break
 
-            self.rings[radius] = Ring(
-                self.args,
+            self._rings[radius] = RingsIterator._Ring(
+                self._config,
                 radius,
-                self.terminal.output_area.center,
+                self._terminal.output_area.center,
                 ring_coords,
                 self.ring_gap,
-                self.args.ring_colors[len(self.rings) % len(self.args.ring_colors)],
-                self.character_final_color_map,
+                self._config.ring_colors[len(self._rings) % len(self._config.ring_colors)],
+                self._character_final_color_map,
             )
         # assign characters to rings
         ring_count = 0
-        for ring in self.rings.values():
+        for ring in self._rings.values():
             for _ in ring.counter_clockwise_coords:
-                if self.pending_chars:
-                    next_character = self.pending_chars.pop(0)
+                if self._pending_chars:
+                    next_character = self._pending_chars.pop(0)
                     # set rings to rotate in opposite directions
                     ring.add_character(next_character, clockwise=ring_count % 2)
-                    self.ring_chars.append(next_character)
+                    self._ring_chars.append(next_character)
             ring_count += 1
 
         # make external waypoints for characters not in rings
-        for character in self.terminal.get_characters():
-            if character not in self.ring_chars:
+        for character in self._terminal.get_characters():
+            if character not in self._ring_chars:
                 external_path = character.motion.new_path(id="external", speed=0.8, ease=easing.out_sine)
-                external_path.new_waypoint(self.terminal.output_area.random_coord(outside_scope=True))
+                external_path.new_waypoint(self._terminal.output_area.random_coord(outside_scope=True))
 
-                self.non_ring_chars.append(character)
+                self._non_ring_chars.append(character)
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_COMPLETE,
                     external_path,
                     EventHandler.Action.CALLBACK,
-                    EventHandler.Callback(self.terminal.set_character_visibility, False),
+                    EventHandler.Callback(self._terminal.set_character_visibility, False),
                 )
-
-    def run(self) -> None:
-        """Runs the effect."""
-
-        self.prepare_data()
-        rings = list(self.rings.values())
-        phase = "start"
-        initial_disperse_complete = False
-        spin_time_remaining = self.args.spin_duration
-        disperse_time_remaining = self.args.disperse_duration
-        cycles_remaining = self.args.spin_disperse_cycles
-        initial_phase_time_remaining = 100
-        while phase != "complete":
-            if phase == "start":
-                if not initial_phase_time_remaining:
-                    phase = "disperse"
+        self._rings_list = list(self._rings.values())
+        self._phase = "start"
+        self._initial_disperse_complete = False
+        self._spin_time_remaining = self._config.spin_duration
+        self._disperse_time_remaining = self._config.disperse_duration
+        self._cycles_remaining = self._config.spin_disperse_cycles
+        self._initial_phase_time_remaining = 100
+
+    def __next__(self) -> str:
+        if self._phase != "complete":
+            if self._phase == "start":
+                if not self._initial_phase_time_remaining:
+                    self._phase = "disperse"
                 else:
-                    initial_phase_time_remaining -= 1
+                    self._initial_phase_time_remaining -= 1
 
-            elif phase == "disperse":
-                if not initial_disperse_complete:
-                    initial_disperse_complete = True
-                    for ring in rings:
+            elif self._phase == "disperse":
+                if not self._initial_disperse_complete:
+                    self._initial_disperse_complete = True
+                    for ring in self._rings_list:
                         for character in ring.characters:
                             disperse_path = ring.make_disperse_waypoints(
                                 character, character.motion.paths["0"].waypoints[0].coord
                             )
                             initial_path = character.motion.new_path(speed=0.3, ease=easing.out_cubic)
                             initial_path.new_waypoint(disperse_path.waypoints[0].coord)
                             character.event_handler.register_event(
                                 EventHandler.Event.PATH_COMPLETE,
                                 initial_path,
                                 EventHandler.Action.ACTIVATE_PATH,
                                 disperse_path,
                             )
                             character.animation.activate_scene(character.animation.query_scene("disperse"))
                             character.motion.activate_path(initial_path)
-                            self.active_chars.append(character)
+                            self._active_chars.append(character)
 
-                    for character in self.non_ring_chars:
+                    for character in self._non_ring_chars:
                         character.motion.activate_path(character.motion.query_path("external"))
-                        self.active_chars.append(character)
+                        self._active_chars.append(character)
 
                 else:
-                    if not disperse_time_remaining:
-                        phase = "spin"
-                        cycles_remaining -= 1
-                        spin_time_remaining = self.args.spin_duration
-                        for ring in rings:
+                    if not self._disperse_time_remaining:
+                        self._phase = "spin"
+                        self._cycles_remaining -= 1
+                        self._spin_time_remaining = self._config.spin_duration
+                        for ring in self._rings_list:
                             ring.spin()
                     else:
-                        disperse_time_remaining -= 1
+                        self._disperse_time_remaining -= 1
 
-            elif phase == "spin":
-                if not spin_time_remaining:
-                    if not cycles_remaining:
-                        phase = "final"
-                        for character in self.terminal.get_characters():
-                            self.terminal.set_character_visibility(character, True)
+            elif self._phase == "spin":
+                if not self._spin_time_remaining:
+                    if not self._cycles_remaining:
+                        self._phase = "final"
+                        for character in self._terminal.get_characters():
+                            self._terminal.set_character_visibility(character, True)
                             character.motion.activate_path(character.motion.query_path("home"))
-                            self.active_chars.append(character)
+                            self._active_chars.append(character)
                             if "external" in character.motion.paths:
                                 continue
                             character.animation.activate_scene(character.animation.query_scene("disperse"))
                     else:
-                        disperse_time_remaining = self.args.disperse_duration
-                        for ring in rings:
+                        self._disperse_time_remaining = self._config.disperse_duration
+                        for ring in self._rings_list:
                             ring.disperse()
-                        phase = "disperse"
+                        self._phase = "disperse"
 
                 else:
-                    spin_time_remaining -= 1
+                    self._spin_time_remaining -= 1
+
+            elif self._phase == "final":
+                if not self._active_chars:
+                    self._phase = "complete"
+
+            for character in self._active_chars:
+                character.tick()
+            next_frame = self._terminal.get_formatted_output_string()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return next_frame
+        else:
+            raise StopIteration
+
+
+class Rings(BaseEffect[RingsConfig]):
+    """Characters are dispersed and form into spinning rings."""
+
+    _config_cls = RingsConfig
+    _iterator_cls = RingsIterator
 
-            elif phase == "final":
-                if not self.active_chars:
-                    phase = "complete"
-
-            self.terminal.print()
-            self.animate_chars()
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_spotlights.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_spotlights.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,226 +1,265 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import animation, easing, geometry, graphics, motion
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return SpotlightsEffect, SpotlightsEffectArgs
+    return Spotlights, SpotlightsConfig
 
 
 @argclass(
     name="spotlights",
-    formatter_class=arg_validators.CustomFormatter,
     help="Spotlights search the text area, illuminating characters, before converging in the center and expanding.",
     description="spotlights | Spotlights search the text area, illuminating characters, before converging in the center and expanding.",
     epilog=f"""{arg_validators.EASING_EPILOG}
 Example: terminaltexteffects spotlights --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --beam-width-ratio 2.0 --beam-falloff 0.3 --search-duration 750 --search-speed-range 0.25-0.5 --spotlight-count 3""",
 )
 @dataclass
-class SpotlightsEffectArgs(ArgsDataClass):
+class SpotlightsConfig(ArgsDataClass):
+    """Configuration for the Spotlights effect.
+
+    Attributes:
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        beam_width_ratio (float): Width of the beam of light as min(width, height) // n of the input text.
+        beam_falloff (float): Distance from the edge of the beam where the brightness begins to fall off, as a percentage of total beam width.
+        search_duration (int): Duration of the search phase, in animation steps, before the spotlights converge in the center.
+        search_speed_range (tuple[float, float]): Range of speeds for the spotlights during the search phase. The speed is a random value between the two provided values.
+        spotlight_count (int): Number of spotlights to use.
+    """
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("ab48ff", "e7b2b2", "fffebd"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     beam_width_ratio: float = ArgField(
         cmd_name="--beam-width-ratio",
         type_parser=arg_validators.PositiveFloat.type_parser,
         default=2.0,
         metavar=arg_validators.PositiveFloat.METAVAR,
         help="Width of the beam of light as min(width, height) // n of the input text.",
     )  # type: ignore[assignment]
+    "float : Width of the beam of light as min(width, height) // n of the input text."
+
     beam_falloff: float = ArgField(
         cmd_name="--beam-falloff",
         type_parser=arg_validators.NonNegativeFloat.type_parser,
         default=0.3,
         metavar=arg_validators.NonNegativeFloat.METAVAR,
         help="Distance from the edge of the beam where the brightness begins to fall off, as a percentage of total beam width.",
     )  # type: ignore[assignment]
+    "float : Distance from the edge of the beam where the brightness begins to fall off, as a percentage of total beam width."
+
     search_duration: int = ArgField(
         cmd_name="--search-duration",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=750,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Duration of the search phase, in animation steps, before the spotlights converge in the center.",
     )  # type: ignore[assignment]
+    "int : Duration of the search phase, in animation steps, before the spotlights converge in the center."
+
     search_speed_range: tuple[float, float] = ArgField(
         cmd_name="--search-speed-range",
         type_parser=arg_validators.PositiveFloatRange.type_parser,
         default=(0.25, 0.5),
         metavar=arg_validators.PositiveFloatRange.METAVAR,
         help="Range of speeds for the spotlights during the search phase. The speed is a random value between the two provided values.",
     )  # type: ignore[assignment]
+    "tuple[float, float] : Range of speeds for the spotlights during the search phase. The speed is a random value between the two provided values."
+
     spotlight_count: int = ArgField(
         cmd_name="--spotlight-count",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=3,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Number of spotlights to use.",
     )  # type: ignore[assignment]
+    "int : Number of spotlights to use."
 
     @classmethod
     def get_effect_class(cls):
-        return SpotlightsEffect
+        return Spotlights
 
 
-class SpotlightsEffect:
-    def __init__(self, terminal: Terminal, args: SpotlightsEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.spotlights: list[EffectCharacter] = self.make_spotlights(self.args.spotlight_count)
-        self.illuminated_chars: set[EffectCharacter] = set()
-        self.character_color_map: dict[EffectCharacter, tuple[graphics.Color, graphics.Color]] = {}  # (bright, dark)
+class SpotlightsIterator(BaseEffectIterator[SpotlightsConfig]):
+    def __init__(self, effect: "Spotlights") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._illuminated_chars: set[EffectCharacter] = set()
+        self._character_color_map: dict[EffectCharacter, tuple[graphics.Color, graphics.Color]] = {}  # (bright, dark)
+        self._build()
 
-    def make_spotlights(self, num_spotlights: int) -> list[EffectCharacter]:
+    def _make_spotlights(self, num_spotlights: int) -> list[EffectCharacter]:
         spotlights: list[EffectCharacter] = []
-        minimum_distance = self.terminal.output_area.right // 4
+        minimum_distance = self._terminal.output_area.right // 4
         for _ in range(num_spotlights):
-            spotlight = self.terminal.add_character("O", self.terminal.output_area.random_coord(outside_scope=True))
+            spotlight = self._terminal.add_character("O", self._terminal.output_area.random_coord(outside_scope=True))
             spotlights.append(spotlight)
 
             spotlight_target_coords: list[Coord] = []
-            last_coord = self.terminal.output_area.random_coord()
+            last_coord = self._terminal.output_area.random_coord()
             spotlight_target_coords.append(last_coord)
             for _ in range(10):
-                next_coord = self.find_coord_at_minimum_distance(last_coord, minimum_distance)
+                next_coord = self._find_coord_at_minimum_distance(last_coord, minimum_distance)
                 spotlight_target_coords.append(next_coord)
                 last_coord = next_coord
 
             paths: list[motion.Path] = []
             for coord in spotlight_target_coords:
                 path = spotlight.motion.new_path(
-                    speed=random.uniform(self.args.search_speed_range[0], self.args.search_speed_range[1]),
+                    speed=random.uniform(self._config.search_speed_range[0], self._config.search_speed_range[1]),
                     ease=easing.in_out_quad,
                     id=str(len(paths)),
                 )
-                path.new_waypoint(coord, bezier_control=self.terminal.output_area.random_coord(outside_scope=True))
+                path.new_waypoint(coord, bezier_control=self._terminal.output_area.random_coord(outside_scope=True))
                 paths.append(path)
             spotlight.motion.chain_paths(paths, loop=True)
 
             path = spotlight.motion.new_path(speed=0.5, ease=easing.in_out_sine, id="center")
-            path.new_waypoint(self.terminal.output_area.center)
+            path.new_waypoint(self._terminal.output_area.center)
 
         return spotlights
 
-    def find_coord_at_minimum_distance(self, origin_coord: Coord, minimum_distance: int) -> Coord:
+    def _find_coord_at_minimum_distance(self, origin_coord: Coord, minimum_distance: int) -> Coord:
         coord_found = False
         while not coord_found:
-            coord = self.terminal.output_area.random_coord()
+            coord = self._terminal.output_area.random_coord()
             distance = geometry.find_length_of_line(origin_coord, coord)
             if distance >= minimum_distance:
                 coord_found = True
         return coord
 
-    def illuminate_chars(self, range: int) -> None:
+    def _illuminate_chars(self, range: int) -> None:
         coords_in_range: list[Coord] = []
-        for spotlight in self.spotlights:
+        for spotlight in self._spotlights:
             coords_in_range.extend(geometry.find_coords_in_circle(spotlight.motion.current_coord, range))
         chars_in_range: set[EffectCharacter] = set()
         for coord in coords_in_range:
-            character = self.terminal.get_character_by_input_coord(coord)
+            character = self._terminal.get_character_by_input_coord(coord)
             if character and character.symbol != " ":
                 chars_in_range.add(character)
-        chars_no_longer_in_range = self.illuminated_chars - chars_in_range
+        chars_no_longer_in_range = self._illuminated_chars - chars_in_range
         for character in chars_no_longer_in_range:
             character.animation.set_appearance(
                 character.input_symbol,
-                self.character_color_map[character][1],
+                self._character_color_map[character][1],
             )
 
         for character in chars_in_range:
             distance = min(
                 [
                     geometry.find_length_of_line(
                         spotlight.motion.current_coord, character.input_coord, double_row_diff=True
                     )
-                    for spotlight in self.spotlights
+                    for spotlight in self._spotlights
                 ]
             )
 
-            if distance > range * (1 - self.args.beam_falloff):
+            if distance > range * (1 - self._config.beam_falloff):
                 brightness_factor = max(
-                    1 - (distance - range * (1 - self.args.beam_falloff)) / (range * self.args.beam_falloff), 0.2
+                    1 - (distance - range * (1 - self._config.beam_falloff)) / (range * self._config.beam_falloff), 0.2
                 )
                 adjusted_color = animation.Animation.adjust_color_brightness(
-                    self.character_color_map[character][0], brightness_factor
+                    self._character_color_map[character][0], brightness_factor
                 )
             else:
-                adjusted_color = self.character_color_map[character][0]
+                adjusted_color = self._character_color_map[character][0]
             character.animation.set_appearance(character.input_symbol, adjusted_color)
-        self.illuminated_chars = chars_in_range
+        self._illuminated_chars = chars_in_range
 
-    def prepare_data(self) -> None:
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        self._spotlights: list[EffectCharacter] = self._make_spotlights(self._config.spotlight_count)
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
+        for character in self._terminal.get_characters():
             color_bright = final_gradient_mapping[character.input_coord]
-            self.terminal.set_character_visibility(character, True)
+            self._terminal.set_character_visibility(character, True)
             color_dark = animation.Animation.adjust_color_brightness(color_bright, 0.2)
-            self.character_color_map[character] = (color_bright, color_dark)
+            self._character_color_map[character] = (color_bright, color_dark)
             character.animation.set_appearance(character.input_symbol, color_dark)
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        illuminate_range = int(
-            max(min(self.terminal.output_area.right, self.terminal.output_area.top) // self.args.beam_width_ratio, 1)
+        self._illuminate_range = int(
+            max(
+                min(self._terminal.output_area.right, self._terminal.output_area.top) // self._config.beam_width_ratio,
+                1,
+            )
         )
-        search_duration = self.args.search_duration
-        searching = True
-        complete = False
-        for spotlight in self.spotlights:
+        self._search_duration = self._config.search_duration
+        self._searching = True
+        self._complete = False
+        for spotlight in self._spotlights:
             spotlight_path_start = spotlight.motion.query_path("0")
             spotlight.motion.activate_path(spotlight_path_start)
-            self.active_chars.append(spotlight)
-        while not complete:
-            self.illuminate_chars(illuminate_range)
-            if searching:
-                search_duration -= 1
-                if not search_duration:
-                    for spotlight in self.spotlights:
+            self._active_chars.append(spotlight)
+
+    def __next__(self) -> str:
+        if not self._complete:
+            self._illuminate_chars(self._illuminate_range)
+            if self._searching:
+                self._search_duration -= 1
+                if not self._search_duration:
+                    for spotlight in self._spotlights:
                         spotlight_path_center = spotlight.motion.query_path("center")
                         spotlight.motion.activate_path(spotlight_path_center)
-                    searching = False
-            if not any([spotlight.motion.active_path for spotlight in self.spotlights]):
-                while len(self.spotlights) > 1:
-                    self.spotlights.pop()
-                illuminate_range += 1
-                if illuminate_range > max(self.terminal.output_area.right, self.terminal.output_area.top) // 1.5:
-                    complete = True
-
-            self.terminal.print()
-            self.animate_chars()
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+                    self._searching = False
+            if not any([spotlight.motion.active_path for spotlight in self._spotlights]):
+                while len(self._spotlights) > 1:
+                    self._spotlights.pop()
+                self._illuminate_range += 1
+                if (
+                    self._illuminate_range
+                    > max(self._terminal.output_area.right, self._terminal.output_area.top) // 1.5
+                ):
+                    self._complete = True
+
+            for character in self._active_chars:
+                character.tick()
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class Spotlights(BaseEffect[SpotlightsConfig]):
+    """Spotlights search the text area, illuminating characters, before converging in the center and expanding."""
+
+    _config_cls = SpotlightsConfig
+    _iterator_cls = SpotlightsIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_spray.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_middleout.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,191 +1,192 @@
-"""Effect that draws the characters spawning at varying rates from a single point."""
-
-import random
 import typing
 from dataclasses import dataclass
-from enum import Enum, auto
 
 import terminaltexteffects.utils.arg_validators as arg_validators
-from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return SprayEffect, SprayEffectArgs
+    return MiddleOut, MiddleOutConfig
 
 
 @argclass(
-    name="spray",
-    formatter_class=arg_validators.CustomFormatter,
-    help="Draws the characters spawning at varying rates from a single point.",
-    description="spray | Draws the characters spawning at varying rates from a single point.",
-    epilog=f"""{arg_validators.EASING_EPILOG}    
-Example: terminaltexteffects spray --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --spray-position e --spray-volume 0.005 --movement-speed 0.4-1.0 --movement-easing OUT_EXPO""",
+    name="middleout",
+    help="Text expands in a single row or column in the middle of the output area then out.",
+    description="middleout | Text expands in a single row or column in the middle of the output area then out.",
+    epilog=f"""{arg_validators.EASING_EPILOG}
+Example: terminaltexteffects middleout --starting-color 8A008A --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --expand-direction vertical --center-movement-speed 0.35 --full-movement-speed 0.35 --center-easing IN_OUT_SINE --full-easing IN_OUT_SINE""",
 )
 @dataclass
-class SprayEffectArgs(ArgsDataClass):
+class MiddleOutConfig(ArgsDataClass):
+    """Configuration for the Middleout effect.
+
+    Attributes:
+        starting_color (graphics.Color): Color for the initial text in the center of the output area.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        expand_direction (str): Direction the text will expand.
+        center_movement_speed (float): Speed of the characters during the initial expansion of the center vertical/horiztonal"""
+
+    starting_color: graphics.Color = ArgField(
+        cmd_name="--starting-color",
+        type_parser=arg_validators.Color.type_parser,
+        default="ffffff",
+        metavar=arg_validators.Color.METAVAR,
+        help="Color for the initial text in the center of the output area.",
+    )  # type: ignore[assignment]
+    "graphics.Color : Color for the initial text in the center of the output area."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
-        cmd_name=["--final-gradient-stops"],
+        cmd_name="--final-gradient-stops",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
-        cmd_name=["--final-gradient-steps"],
+        cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
-    spray_position: str = ArgField(
-        cmd_name="--spray-position",
-        choices=["n", "ne", "e", "se", "s", "sw", "w", "nw", "center"],
-        default="e",
-        help="Position for the spray origin.",
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
+    expand_direction: str = ArgField(
+        cmd_name="--expand-direction",
+        default="vertical",
+        choices=["vertical", "horizontal"],
+        help="Direction the text will expand.",
     )  # type: ignore[assignment]
-    spray_volume: float = ArgField(
-        cmd_name="--spray-volume",
+    "str : Direction the text will expand."
+
+    center_movement_speed: float = ArgField(
+        cmd_name="--center-movement-speed",
         type_parser=arg_validators.PositiveFloat.type_parser,
-        default=0.005,
+        default=0.35,
         metavar=arg_validators.PositiveFloat.METAVAR,
-        help="Number of characters to spray per tick as a percent of the total number of characters.",
+        help="Speed of the characters during the initial expansion of the center vertical/horiztonal line. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
     )  # type: ignore[assignment]
-    movement_speed: tuple[float, float] = ArgField(
-        cmd_name="--movement-speed",
-        type_parser=arg_validators.PositiveFloatRange.type_parser,
-        default=(0.4, 1.0),
-        metavar=arg_validators.PositiveFloatRange.METAVAR,
-        help="Movement speed of the characters.",
+    "float : Speed of the characters during the initial expansion of the center vertical/horiztonal line. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+
+    full_movement_speed: float = ArgField(
+        cmd_name="--full-movement-speed",
+        type_parser=arg_validators.PositiveFloat.type_parser,
+        default=0.35,
+        metavar=arg_validators.PositiveFloat.METAVAR,
+        help="Speed of the characters during the final full expansion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
+    )  # type: ignore[assignment]
+    "float : Speed of the characters during the final full expansion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+
+    center_easing: easing.EasingFunction = ArgField(
+        cmd_name="--center-easing",
+        default=easing.in_out_sine,
+        type_parser=arg_validators.Ease.type_parser,
+        help="Easing function to use for initial expansion.",
     )  # type: ignore[assignment]
-    movement_easing: easing.EasingFunction = ArgField(
-        cmd_name="--movement-easing",
+    "easing.EasingFunction : Easing function to use for initial expansion."
+
+    full_easing: easing.EasingFunction = ArgField(
+        cmd_name="--full-easing",
+        default=easing.in_out_sine,
         type_parser=arg_validators.Ease.type_parser,
-        default=easing.out_expo,
-        help="Easing function to use for character movement.",
+        help="Easing function to use for full expansion.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for full expansion."
 
     @classmethod
     def get_effect_class(cls):
-        return SprayEffect
+        return MiddleOut
 
 
-class SprayPosition(Enum):
-    """Position for the spray origin."""
+class MiddleOutIterator(BaseEffectIterator[MiddleOutConfig]):
+    def __init__(self, effect: "MiddleOut"):
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._phase = "center"
+        self._build()
 
-    N = auto()
-    NE = auto()
-    E = auto()
-    SE = auto()
-    S = auto()
-    SW = auto()
-    W = auto()
-    NW = auto()
-    CENTER = auto()
-
-
-class SprayEffect:
-    """Effect that draws the characters spawning at varying rates from a single point."""
-
-    def __init__(
-        self,
-        terminal: Terminal,
-        args: SprayEffectArgs,
-    ):
-        """Effect that draws the characters spawning at varying rates from a single point.
-
-        Args:
-            terminal (Terminal): terminal to use for the effect
-            args (argparse.Namespace): arguments from argparse
-        """
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.spray_position = {
-            "n": SprayPosition.N,
-            "ne": SprayPosition.NE,
-            "e": SprayPosition.E,
-            "se": SprayPosition.SE,
-            "s": SprayPosition.S,
-            "sw": SprayPosition.SW,
-            "w": SprayPosition.W,
-            "nw": SprayPosition.NW,
-            "center": SprayPosition.CENTER,
-        }.get(args.spray_position, SprayPosition.E)
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by starting all of the characters from a point based on SparklerPosition."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        spray_origin_map = {
-            SprayPosition.CENTER: (self.terminal.output_area.center),
-            SprayPosition.N: Coord(self.terminal.output_area.right // 2, self.terminal.output_area.top),
-            SprayPosition.NW: Coord(self.terminal.output_area.left, self.terminal.output_area.top),
-            SprayPosition.W: Coord(self.terminal.output_area.left, self.terminal.output_area.top // 2),
-            SprayPosition.SW: Coord(self.terminal.output_area.left, self.terminal.output_area.bottom),
-            SprayPosition.S: Coord(self.terminal.output_area.right // 2, self.terminal.output_area.bottom),
-            SprayPosition.SE: Coord(self.terminal.output_area.right - 1, self.terminal.output_area.bottom),
-            SprayPosition.E: Coord(self.terminal.output_area.right - 1, self.terminal.output_area.top // 2),
-            SprayPosition.NE: Coord(self.terminal.output_area.right - 1, self.terminal.output_area.top),
-        }
-
-        for character in self.terminal.get_characters():
-            character.motion.set_coordinate(spray_origin_map[self.spray_position])
-            input_coord_path = character.motion.new_path(
-                speed=random.uniform(self.args.movement_speed[0], self.args.movement_speed[1]),
-                ease=self.args.movement_easing,
-            )
-            input_coord_path.new_waypoint(character.input_coord)
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_ACTIVATED, input_coord_path, EventHandler.Action.SET_LAYER, 1
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+            character.motion.set_coordinate(self._terminal.output_area.center)
+            # setup waypoints
+            if self._config.expand_direction == "vertical":
+                column = character.input_coord.column
+                row = self._terminal.output_area.center_row
+            else:
+                column = self._terminal.output_area.center_column
+                row = character.input_coord.row
+            center_path = character.motion.new_path(
+                speed=self._config.center_movement_speed, ease=self._config.center_easing
             )
-            character.event_handler.register_event(
-                EventHandler.Event.PATH_COMPLETE, input_coord_path, EventHandler.Action.SET_LAYER, 0
+            center_path.new_waypoint(Coord(column, row))
+            full_path = character.motion.new_path(
+                id="full", speed=self._config.full_movement_speed, ease=self._config.full_easing
             )
-            droplet_scn = character.animation.new_scene()
-            spray_gradient = graphics.Gradient(
-                random.choice(final_gradient.spectrum), self.character_final_color_map[character], steps=7
+            full_path.new_waypoint(character.input_coord, id="full")
+
+            # setup scenes
+            full_scene = character.animation.new_scene(id="full")
+            full_gradient = graphics.Gradient(
+                self._config.starting_color, self._character_final_color_map[character], steps=10
             )
-            droplet_scn.apply_gradient_to_symbols(spray_gradient, character.input_symbol, 20)
-            character.animation.activate_scene(droplet_scn)
-            character.motion.activate_path(input_coord_path)
-            self.pending_chars.append(character)
-        random.shuffle(self.pending_chars)
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        volume = max(int(len(self.pending_chars) * self.args.spray_volume), 1)
-        while self.pending_chars or self.active_chars:
-            if self.pending_chars:
-                for _ in range(random.randint(1, volume)):
-                    if self.pending_chars:
-                        next_character = self.pending_chars.pop()
-                        self.terminal.set_character_visibility(next_character, True)
-                        self.active_chars.append(next_character)
-
-            self.animate_chars()
-            self.terminal.print()
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-
-    def animate_chars(self) -> None:
-        for character in self.active_chars:
-            character.tick()
+            full_scene.apply_gradient_to_symbols(full_gradient, character.input_symbol, 10)
+
+            # initialize character state
+            character.motion.activate_path(center_path)
+            character.animation.set_appearance(character.input_symbol, self._config.starting_color)
+            self._terminal.set_character_visibility(character, True)
+            self._active_chars.append(character)
+
+    def __next__(self) -> str:
+        if self._active_chars:
+            if (
+                all([character.motion.active_path is None for character in self._active_chars])
+                and self._phase == "center"
+            ):
+                for character in self._active_chars:
+                    character.motion.activate_path(character.motion.query_path("full"))
+                    character.animation.activate_scene(character.animation.query_scene("full"))
+                self._phase = "full"
+            for character in self._active_chars:
+                character.tick()
+            if self._phase == "full":
+                self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class MiddleOut(BaseEffect[MiddleOutConfig]):
+    """Text expands in a single row or column in the middle of the output area then out."""
+
+    _config_cls = MiddleOutConfig
+    _iterator_cls = MiddleOutIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_swarm.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_swarm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,153 +1,183 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import animation, easing, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return SwarmEffect, SwarmEffectArgs
+    return Swarm, SwarmConfig
 
 
 @argclass(
     name="swarm",
-    formatter_class=arg_validators.CustomFormatter,
     help="Characters are grouped into swarms and move around the terminal before settling into position.",
     description="swarm | Characters are grouped into swarms and move around the terminal before settling into position.",
     epilog="""Example: terminaltexteffects swarm --base-color 31a0d4 --flash-color f2ea79 --final-gradient-stops 31b900 f0ff65 --final-gradient-steps 12 --swarm-size 0.1 --swarm-coordination 0.80 --swarm-area-count 2-4""",
 )
 @dataclass
-class SwarmEffectArgs(ArgsDataClass):
+class SwarmConfig(ArgsDataClass):
+    """Configuration for the Swarm effect.
+
+    Attributes:
+        base_color (tuple[graphics.Color, ...]): Tuple of colors for the swarms.
+        flash_color (graphics.Color): Color for the character flash. Characters flash when moving.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        swarm_size (float): Percent of total characters in each swarm.
+        swarm_coordination (float): Percent of characters in a swarm that move as a group.
+        swarm_area_count (tuple[int, int]): Range of the number of areas where characters will swarm."""
+
     base_color: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--base-color"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("31a0d4",),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the swarms",
     )  # type: ignore[assignment]
+    """tuple[graphics.Color, ...] : Tuple of colors for the swarms"""
+
     flash_color: graphics.Color = ArgField(
         cmd_name=["--flash-color"],
         type_parser=arg_validators.Color.type_parser,
         default="f2ea79",
         metavar=arg_validators.Color.METAVAR,
         help="Color for the character flash. Characters flash when moving.",
     )  # type: ignore[assignment]
+    """graphics.Color : Color for the character flash. Characters flash when moving."""
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("31b900", "f0ff65"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.HORIZONTAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     swarm_size: float = ArgField(
         cmd_name="--swarm-size",
         type_parser=arg_validators.Ratio.type_parser,
         metavar=arg_validators.Ratio.METAVAR,
         default=0.1,
         help="Percent of total characters in each swarm.",
     )  # type: ignore[assignment]
+    "float : Percent of total characters in each swarm."
+
     swarm_coordination: float = ArgField(
         cmd_name="--swarm-coordination",
         type_parser=arg_validators.Ratio.type_parser,
         metavar=arg_validators.Ratio.METAVAR,
         default=0.80,
         help="Percent of characters in a swarm that move as a group.",
     )  # type: ignore[assignment]
+    "float : Percent of characters in a swarm that move as a group."
+
     swarm_area_count: tuple[int, int] = ArgField(
         cmd_name="--swarm-area-count",
         type_parser=arg_validators.IntRange.type_parser,
         metavar=arg_validators.IntRange.METAVAR,
         default=(2, 4),
         help="Range of the number of areas where characters will swarm.",
     )  # type: ignore[assignment]
+    "tuple[int, int] : Range of the number of areas where characters will swarm."
 
     @classmethod
     def get_effect_class(cls):
-        return SwarmEffect
+        return Swarm
 
 
-class SwarmEffect:
+class SwarmIterator(BaseEffectIterator[SwarmConfig]):
     """Characters behave with swarm characteristics before flying into position."""
 
-    def __init__(self, terminal: Terminal, args: SwarmEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.swarms: list[list[EffectCharacter]] = []
-        self.swarm_size: int = max(round(len(self.terminal._input_characters) * self.args.swarm_size), 1)
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+    def __init__(
+        self,
+        effect: "Swarm",
+    ) -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._swarms: list[list[EffectCharacter]] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
 
-    def make_swarms(self) -> None:
-        unswarmed_characters = list(self.terminal._input_characters[::-1])
+    def _make_swarms(self, swarm_size: int) -> None:
+        unswarmed_characters = list(self._terminal._input_characters[::-1])
         while unswarmed_characters:
             new_swarm: list[EffectCharacter] = []
-            for _ in range(self.swarm_size):
+            for _ in range(swarm_size):
                 if unswarmed_characters:
                     new_swarm.append(unswarmed_characters.pop())
                 else:
                     break
-            self.swarms.append(new_swarm)
+            self._swarms.append(new_swarm)
 
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by creating swarms of characters and setting waypoints and animations."""
-        self.make_swarms()
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def _build(self) -> None:
+        swarm_size: int = max(round(len(self._terminal._input_characters) * self._config.swarm_size), 1)
+        self._make_swarms(swarm_size)
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        flash_list = [self.args.flash_color for _ in range(10)]
-        for swarm in self.swarms:
-            swarm_gradient = graphics.Gradient(random.choice(self.args.base_color), self.args.flash_color, steps=7)
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        flash_list = [self._config.flash_color for _ in range(10)]
+        for swarm in self._swarms:
+            swarm_gradient = graphics.Gradient(
+                random.choice(self._config.base_color), self._config.flash_color, steps=7
+            )
             swarm_gradient_mirror = list(swarm_gradient) + flash_list + list(swarm_gradient)[::-1]
             swarm_area_coordinate_map: dict[Coord, list[Coord]] = {}
-            swarm_spawn = self.terminal.output_area.random_coord(outside_scope=True)
+            swarm_spawn = self._terminal.output_area.random_coord(outside_scope=True)
             swarm_areas: list[Coord] = []
-            swarm_area_count = random.randint(self.args.swarm_area_count[0], self.args.swarm_area_count[1])
+            swarm_area_count = random.randint(self._config.swarm_area_count[0], self._config.swarm_area_count[1])
             # create areas where characters will swarm
             last_focus_coord = swarm_spawn
-            radius = max(min(self.terminal.output_area.right, self.terminal.output_area.top) // 2, 1)
+            radius = max(min(self._terminal.output_area.right, self._terminal.output_area.top) // 2, 1)
             while len(swarm_areas) < swarm_area_count:
                 potential_focus_coords = geometry.find_coords_on_circle(last_focus_coord, radius)
                 random.shuffle(potential_focus_coords)
                 for coord in potential_focus_coords:
-                    if self.terminal.output_area.coord_is_in_output_area(coord):
+                    if self._terminal.output_area.coord_is_in_output_area(coord):
                         next_focus_coord = coord
                         break
                 else:
-                    next_focus_coord = self.terminal.output_area.random_coord()
+                    next_focus_coord = self._terminal.output_area.random_coord()
                 swarm_areas.append(next_focus_coord)
                 swarm_area_coordinate_map[last_focus_coord] = geometry.find_coords_in_circle(
                     last_focus_coord,
-                    max(min(self.terminal.output_area.right, self.terminal.output_area.top) // 6, 1) * 2,
+                    max(min(self._terminal.output_area.right, self._terminal.output_area.top) // 6, 1) * 2,
                 )
                 last_focus_coord = next_focus_coord
 
             # assign characters waypoints for swarm areas and inner waypoints within the swarm areas
             for character in swarm:
                 swarm_area_count = 0
                 character.motion.set_coordinate(swarm_spawn)
@@ -181,59 +211,66 @@
                         )
                         inner_path.new_waypoint(next_coord, id=str(len(character.motion.paths)))
                 # create landing waypoint and scene
                 input_path = character.motion.new_path(speed=0.3, ease=easing.in_out_quad)
                 input_path.new_waypoint(character.input_coord)
                 input_scn = character.animation.new_scene()
                 for step in graphics.Gradient(
-                    self.args.flash_color, self.character_final_color_map[character], steps=10
+                    self._config.flash_color, self._character_final_color_map[character], steps=10
                 ):
                     input_scn.add_frame(character.input_symbol, 3, color=step)
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_COMPLETE, input_path, EventHandler.Action.ACTIVATE_SCENE, input_scn
                 )
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_COMPLETE, input_path, EventHandler.Action.SET_LAYER, 0
                 )
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_ACTIVATED, input_path, EventHandler.Action.ACTIVATE_SCENE, flash_scn
                 )
                 character.motion.chain_paths(list(character.motion.paths.values()))
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        call_next = True
-        active_swarm_area = "0_swarm_area"
-        while self.swarms or self.active_chars:
-            if self.swarms and call_next:
-                call_next = False
-                current_swarm = self.swarms.pop()
-                active_swarm_area = "0_swarm_area"
-                for character in current_swarm:
+        self._call_next = False
+        self._active_swarm_area = "0_swarm_area"
+        self._current_swarm = self._swarms.pop()
+
+    def __next__(self) -> str:
+        if self._swarms or self._active_chars:
+            if self._swarms and self._call_next:
+                self._call_next = False
+                self._current_swarm = self._swarms.pop()
+                self._active_swarm_area = "0_swarm_area"
+                for character in self._current_swarm:
                     character.motion.activate_path(character.motion.query_path("0_swarm_area"))
-                    self.terminal.set_character_visibility(character, True)
-                    self.active_chars.append(character)
-            self.terminal.print()
-            self.animate_chars()
-            if len(self.active_chars) < len(current_swarm):
-                call_next = True
-            if current_swarm:
-                for character in current_swarm:
+                    self._terminal.set_character_visibility(character, True)
+                    self._active_chars.append(character)
+            for character in self._active_chars:
+                character.tick()
+            if len(self._active_chars) < len(self._current_swarm):
+                self._call_next = True
+            if self._current_swarm:
+                for character in self._current_swarm:
                     if (
                         character.motion.active_path
-                        and character.motion.active_path.path_id != active_swarm_area
+                        and character.motion.active_path.path_id != self._active_swarm_area
                         and "swarm_area" in character.motion.active_path.path_id
-                        and int(character.motion.active_path.path_id[0]) > int(active_swarm_area[0])
+                        and int(character.motion.active_path.path_id[0]) > int(self._active_swarm_area[0])
                     ):
-                        active_swarm_area = character.motion.active_path.path_id
-                        for other in current_swarm:
-                            if other is not character and random.random() < self.args.swarm_coordination:
-                                other.motion.activate_path(other.motion.paths[active_swarm_area])
+                        self._active_swarm_area = character.motion.active_path.path_id
+                        for other in self._current_swarm:
+                            if other is not character and random.random() < self._config.swarm_coordination:
+                                other.motion.activate_path(other.motion.paths[self._active_swarm_area])
                         break
 
-            self.active_chars = [character for character in self.active_chars if character.is_active]
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class Swarm(BaseEffect[SwarmConfig]):
+    """Characters are grouped into swarms and move around the terminal before settling into position."""
+
+    _config_cls = SwarmConfig
+    _iterator_cls = SwarmIterator
 
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method."""
-        for character in self.active_chars:
-            character.tick()
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_synthgrid.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_synthgrid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,117 +1,150 @@
 import random
 import typing
 from dataclasses import dataclass
 
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import arg_validators, geometry, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
 from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return SynthGridEffect, SynthGridEffectArgs
+    return SynthGrid, SynthGridConfig
 
 
 @argclass(
     name="synthgrid",
-    formatter_class=arg_validators.CustomFormatter,
     help="Create a grid which fills with characters dissolving into the final text.",
     description="synthgrid | Create a grid which fills with characters dissolving into the final text.",
     epilog="""Example: terminaltexteffects synthgrid --grid-gradient-stops CC00CC ffffff --grid-gradient-steps 12 --text-gradient-stops 8A008A 00D1FF FFFFFF --text-gradient-steps 12 --grid-row-symbol ─ --grid-column-symbol "│" --text-generation-symbols ░ ▒ ▓ --max-active-blocks 0.1""",
 )
 @dataclass
-class SynthGridEffectArgs(ArgsDataClass):
+class SynthGridConfig(ArgsDataClass):
+    """Configuration for the SynthGrid effect.
+
+    Attributes:
+        grid_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the grid gradient.
+        grid_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        grid_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the grid color.
+        text_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the text gradient.
+        text_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        text_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the text color.
+        grid_row_symbol (str): Symbol to use for grid row lines.
+        grid_column_symbol (str): Symbol to use for grid column lines.
+        text_generation_symbols (tuple[str, ...]): Tuple of characters for the text generation animation.
+        max_active_blocks (float): Maximum percentage of blocks to have active at any given time. For example, if set to 0.1, 10 percent of the blocks will be active at any given time."""
+
     grid_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--grid-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("CC00CC", "ffffff"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the grid gradient.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the grid gradient."
+
     grid_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--grid-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     grid_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--grid-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the grid color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the grid color."
+
     text_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--text-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the text gradient.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the text gradient."
+
     text_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--text-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     text_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--text-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the text color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the text color."
+
     grid_row_symbol: str = ArgField(
         cmd_name="--grid-row-symbol",
         type_parser=arg_validators.Symbol.type_parser,
         default="─",
         metavar=arg_validators.Symbol.METAVAR,
         help="Symbol to use for grid row lines.",
     )  # type: ignore[assignment]
+    "str : Symbol to use for grid row lines."
+
     grid_column_symbol: str = ArgField(
         cmd_name="--grid-column-symbol",
         type_parser=arg_validators.Symbol.type_parser,
         default="│",
         metavar=arg_validators.Symbol.METAVAR,
         help="Symbol to use for grid column lines.",
     )  # type: ignore[assignment]
+    "str : Symbol to use for grid column lines."
+
     text_generation_symbols: tuple[str, ...] = ArgField(
         cmd_name="--text-generation-symbols",
         type_parser=arg_validators.Symbol.type_parser,
         nargs="+",
         default=("░", "▒", "▓"),
         metavar=arg_validators.Symbol.METAVAR,
         help="Space separated, unquoted, list of characters for the text generation animation.",
     )  # type: ignore[assignment]
+    "tuple[str, ...] : Tuple of characters for the text generation animation."
+
     max_active_blocks: float = ArgField(
         cmd_name="--max-active-blocks",
         type_parser=arg_validators.PositiveFloat.type_parser,
         default=0.1,
         metavar=arg_validators.PositiveFloat.METAVAR,
         help="Maximum percentage of blocks to have active at any given time. For example, if set to 0.1, 10 percent of the blocks will be active at any given time.",
     )  # type: ignore[assignment]
+    "float : Maximum percentage of blocks to have active at any given time."
 
     @classmethod
     def get_effect_class(cls):
-        return SynthGridEffect
+        return SynthGrid
 
 
-class GridLine:
+class _GridLine:
     def __init__(
         self,
         terminal: Terminal,
-        args: SynthGridEffectArgs,
+        args: SynthGridConfig,
         origin: Coord,
         direction: str,
         grid_gradient_mapping: dict[geometry.Coord, graphics.Color],
     ):
         self.terminal = terminal
         self.args = args
         self.origin = origin
@@ -173,26 +206,26 @@
     def is_extended(self) -> bool:
         return not self.collapsed_characters
 
     def is_collapsed(self) -> bool:
         return not self.extended_characters
 
 
-class SynthGridEffect:
+class SynthGridIterator(BaseEffectIterator[SynthGridConfig]):
     """Effect that creates a grid where blocks of characters dissolved into the input characters."""
 
-    def __init__(self, terminal: Terminal, args: SynthGridEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_groups: list[tuple[int, list[EffectCharacter]]] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.grid_lines: list[GridLine] = []
-        self.group_tracker: dict[int, int] = {}
+    def __init__(self, effect: "SynthGrid") -> None:
+        super().__init__(effect)
+        self._pending_groups: list[tuple[int, list[EffectCharacter]]] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._grid_lines: list[_GridLine] = []
+        self._group_tracker: dict[int, int] = {}
+        self._build()
 
-    def find_even_gap(self, dimension: int) -> int:
+    def _find_even_gap(self, dimension: int) -> int:
         """Find the closest even gap to 20% of the longest dimension.
 
         Args:
             dimension (int): The longest dimension.
 
         Returns:
             int: The gap that is closest to 20% of the dimension length.
@@ -204,182 +237,191 @@
         for i in range(dimension, 4, -1):
             if dimension % i <= 1:
                 potential_gaps.append(i)
         if not potential_gaps:
             return 4
         return min(potential_gaps, key=lambda x: abs(x - dimension // 5))
 
-    def prepare_data(self) -> None:
-        grid_gradient = graphics.Gradient(*self.args.grid_gradient_stops, steps=self.args.grid_gradient_steps)
+    def _build(self) -> None:
+        grid_gradient = graphics.Gradient(*self._config.grid_gradient_stops, steps=self._config.grid_gradient_steps)
         grid_gradient_mapping = grid_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.grid_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.grid_gradient_direction
         )
-        text_gradient = graphics.Gradient(*self.args.text_gradient_stops, steps=self.args.text_gradient_steps)
+        text_gradient = graphics.Gradient(*self._config.text_gradient_stops, steps=self._config.text_gradient_steps)
         text_gradient_mapping = text_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.text_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.text_gradient_direction
         )
 
-        self.grid_lines.append(
-            GridLine(
-                self.terminal,
-                self.args,
-                Coord(self.terminal.output_area.left, self.terminal.output_area.bottom),
+        self._grid_lines.append(
+            _GridLine(
+                self._terminal,
+                self._config,
+                Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
                 "horizontal",
                 grid_gradient_mapping,
             )
         )
-        self.grid_lines.append(
-            GridLine(
-                self.terminal,
-                self.args,
-                Coord(self.terminal.output_area.left, self.terminal.output_area.top),
+        self._grid_lines.append(
+            _GridLine(
+                self._terminal,
+                self._config,
+                Coord(self._terminal.output_area.left, self._terminal.output_area.top),
                 "horizontal",
                 grid_gradient_mapping,
             )
         )
-        self.grid_lines.append(
-            GridLine(
-                self.terminal,
-                self.args,
-                Coord(self.terminal.output_area.left, self.terminal.output_area.bottom),
+        self._grid_lines.append(
+            _GridLine(
+                self._terminal,
+                self._config,
+                Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
                 "vertical",
                 grid_gradient_mapping,
             )
         )
-        self.grid_lines.append(
-            GridLine(
-                self.terminal,
-                self.args,
-                Coord(self.terminal.output_area.right, self.terminal.output_area.bottom),
+        self._grid_lines.append(
+            _GridLine(
+                self._terminal,
+                self._config,
+                Coord(self._terminal.output_area.right, self._terminal.output_area.bottom),
                 "vertical",
                 grid_gradient_mapping,
             )
         )
         column_indexes: list[int] = []
         row_indexes: list[int] = []
-        if self.terminal.output_area.top > 2 * self.terminal.output_area.right:
-            row_gap = self.find_even_gap(self.terminal.output_area.top) + 1
+        if self._terminal.output_area.top > 2 * self._terminal.output_area.right:
+            row_gap = self._find_even_gap(self._terminal.output_area.top) + 1
             column_gap = row_gap * 2
         else:
-            column_gap = self.find_even_gap(self.terminal.output_area.right) + 1
+            column_gap = self._find_even_gap(self._terminal.output_area.right) + 1
             row_gap = column_gap // 2
 
         for row_index in range(
-            self.terminal.output_area.bottom + row_gap, self.terminal.output_area.top, max(row_gap, 1)
+            self._terminal.output_area.bottom + row_gap, self._terminal.output_area.top, max(row_gap, 1)
         ):
-            if self.terminal.output_area.top - row_index < 2:
+            if self._terminal.output_area.top - row_index < 2:
                 continue
             row_indexes.append(row_index)
-            self.grid_lines.append(
-                GridLine(
-                    self.terminal,
-                    self.args,
-                    Coord(self.terminal.output_area.left, row_index),
+            self._grid_lines.append(
+                _GridLine(
+                    self._terminal,
+                    self._config,
+                    Coord(self._terminal.output_area.left, row_index),
                     "horizontal",
                     grid_gradient_mapping,
                 )
             )
         for column_index in range(
-            self.terminal.output_area.left + column_gap, self.terminal.output_area.right, max(column_gap, 1)
+            self._terminal.output_area.left + column_gap, self._terminal.output_area.right, max(column_gap, 1)
         ):
-            if self.terminal.output_area.right - column_index < 2:
+            if self._terminal.output_area.right - column_index < 2:
                 continue
             column_indexes.append(column_index)
-            self.grid_lines.append(
-                GridLine(
-                    self.terminal,
-                    self.args,
-                    Coord(column_index, self.terminal.output_area.bottom),
+            self._grid_lines.append(
+                _GridLine(
+                    self._terminal,
+                    self._config,
+                    Coord(column_index, self._terminal.output_area.bottom),
                     "vertical",
                     grid_gradient_mapping,
                 )
             )
-        row_indexes.append(self.terminal.output_area.top + 1)
-        column_indexes.append(self.terminal.output_area.right + 1)
+        row_indexes.append(self._terminal.output_area.top + 1)
+        column_indexes.append(self._terminal.output_area.right + 1)
         prev_row_index = 1
         for row_index in row_indexes:
             prev_column_index = 1
             for column_index in column_indexes:
                 coords_in_block: list[Coord] = []
-                if row_index == self.terminal.output_area.top:  # make sure the top row is included
+                if row_index == self._terminal.output_area.top:  # make sure the top row is included
                     row_index += 1
                 for row in range(prev_row_index, row_index):
                     for column in range(prev_column_index, column_index):
                         coords_in_block.append(Coord(column, row))
                 characters_in_block: list[EffectCharacter] = []
                 for coord in coords_in_block:
-                    if coord in self.terminal.character_by_input_coord:
-                        characters_in_block.append(self.terminal.character_by_input_coord[coord])
+                    if coord in self._terminal.character_by_input_coord:
+                        characters_in_block.append(self._terminal.character_by_input_coord[coord])
                 if characters_in_block:
-                    self.pending_groups.append((len(self.pending_groups), characters_in_block))
+                    self._pending_groups.append((len(self._pending_groups), characters_in_block))
                 prev_column_index = column_index
             prev_row_index = row_index
-        for group_number, group in self.pending_groups:
-            self.group_tracker[group_number] = 0
+        for group_number, group in self._pending_groups:
+            self._group_tracker[group_number] = 0
             for character in group:
                 dissolve_scn = character.animation.new_scene()
                 for _ in range(random.randint(15, 30)):
                     dissolve_scn.add_frame(
-                        random.choice(self.args.text_generation_symbols),
+                        random.choice(self._config.text_generation_symbols),
                         3,
                         color=random.choice(text_gradient.spectrum),
                     )
                 dissolve_scn.add_frame(character.input_symbol, 1, color=text_gradient_mapping[character.input_coord])
                 character.animation.activate_scene(dissolve_scn)
                 character.event_handler.register_event(
                     EventHandler.Event.SCENE_COMPLETE,
                     dissolve_scn,
                     EventHandler.Action.CALLBACK,
-                    EventHandler.Callback(self.update_group_tracker, group_number),
+                    EventHandler.Callback(self._update_group_tracker, group_number),
                 )
-        random.shuffle(self.pending_groups)
-
-    def update_group_tracker(self, character: EffectCharacter, *args) -> None:
-        self.group_tracker[args[0]] -= 1
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        phase = "grid_expand"
-        total_group_count = len(self.pending_groups)
-        if not total_group_count:
-            for character in self.terminal.get_characters():
-                self.terminal.set_character_visibility(character, True)
-                self.active_chars.append(character)
-        active_groups: int = 0
-        while self.pending_groups or self.active_chars or phase != "complete":
-            if phase == "grid_expand":
-                if not all([grid_line.is_extended() for grid_line in self.grid_lines]):
-                    for grid_line in self.grid_lines:
+        random.shuffle(self._pending_groups)
+        self._phase = "grid_expand"
+        self._total_group_count = len(self._pending_groups)
+        if not self._total_group_count:
+            for character in self._terminal.get_characters():
+                self._terminal.set_character_visibility(character, True)
+                self._active_chars.append(character)
+        self._active_groups: int = 0
+
+    def _update_group_tracker(self, character: EffectCharacter, *args) -> None:
+        self._group_tracker[args[0]] -= 1
+
+    def __next__(self) -> str:
+        if self._pending_groups or self._active_chars or self._phase != "complete":
+            if self._phase == "grid_expand":
+                if not all([grid_line.is_extended() for grid_line in self._grid_lines]):
+                    for grid_line in self._grid_lines:
                         if not grid_line.is_extended():
                             grid_line.extend()
                 else:
-                    phase = "add_chars"
-            elif phase == "add_chars":
-                if self.pending_groups and active_groups < total_group_count * self.args.max_active_blocks:
-                    group_number, next_group = self.pending_groups.pop(0)
+                    self._phase = "add_chars"
+            elif self._phase == "add_chars":
+                if (
+                    self._pending_groups
+                    and self._active_groups < self._total_group_count * self._config.max_active_blocks
+                ):
+                    group_number, next_group = self._pending_groups.pop(0)
                     for char in next_group:
-                        self.terminal.set_character_visibility(char, True)
-                        self.active_chars.append(char)
-                        self.group_tracker[group_number] += 1
-                if not self.pending_groups and not self.active_chars and not active_groups:
-                    phase = "collapse"
-            elif phase == "collapse":
-                if not all([grid_line.is_collapsed() for grid_line in self.grid_lines]):
-                    for grid_line in self.grid_lines:
+                        self._terminal.set_character_visibility(char, True)
+                        self._active_chars.append(char)
+                        self._group_tracker[group_number] += 1
+                if not self._pending_groups and not self._active_chars and not self._active_groups:
+                    self._phase = "collapse"
+            elif self._phase == "collapse":
+                if not all([grid_line.is_collapsed() for grid_line in self._grid_lines]):
+                    for grid_line in self._grid_lines:
                         if not grid_line.is_collapsed():
                             grid_line.collapse()
                 else:
-                    phase = "complete"
-            self.terminal.print()
-            self.animate_chars()
-
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-            active_groups = 0
-            for _, active_count in self.group_tracker.items():
+                    self._phase = "complete"
+            for character in self._active_chars:
+                character.tick()
+
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            self._active_groups = 0
+            for _, active_count in self._group_tracker.items():
                 if active_count:
-                    active_groups += 1
+                    self._active_groups += 1
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class SynthGrid(BaseEffect[SynthGridConfig]):
+    """Effect that creates a grid where blocks of characters dissolved into the input characters."""
+
+    _config_cls = SynthGridConfig
+    _iterator_cls = SynthGridIterator
 
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_unstable.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_unstable.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,218 +1,260 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return UnstableEffect, UnstableEffectArgs
+    return Unstable, UnstableConfig
 
 
 @argclass(
     name="unstable",
-    formatter_class=arg_validators.CustomFormatter,
     help="Spawn characters jumbled, explode them to the edge of the output area, then reassemble them in the correct layout.",
     description="unstable | Spawn characters jumbled, explode them to the edge of the output area, then reassemble them in the correct layout.",
     epilog=f"""{arg_validators.EASING_EPILOG}
     
     Example: terminaltexteffects unstable --unstable-color ff9200 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --explosion-ease OUT_EXPO --explosion-speed 0.75 --reassembly-ease OUT_EXPO --reassembly-speed 0.75""",
 )
 @dataclass
-class UnstableEffectArgs(ArgsDataClass):
+class UnstableConfig(ArgsDataClass):
+    """Configuration for the Unstable effect.
+
+    Attributes:
+        unstable_color (graphics.Color): Color transitioned to as the characters become unstable.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        explosion_ease (easing.EasingFunction): Easing function to use for character movement during the explosion.
+        explosion_speed (float): Speed of characters during explosion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.
+        reassembly_ease (easing.EasingFunction): Easing function to use for character reassembly.
+        reassembly_speed (float): Speed of characters during reassembly.
+    """
+
     unstable_color: graphics.Color = ArgField(
         cmd_name=["--unstable-color"],
         type_parser=arg_validators.Color.type_parser,
         default="ff9200",
         metavar=arg_validators.Color.METAVAR,
         help="Color transitioned to as the characters become unstable.",
     )  # type: ignore[assignment]
+    "graphics.Color : Color transitioned to as the characters become unstable."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name=["--final-gradient-steps"],
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     explosion_ease: easing.EasingFunction = ArgField(
         cmd_name=["--explosion-ease"],
         type_parser=arg_validators.Ease.type_parser,
         default=easing.out_expo,
         help="Easing function to use for character movement during the explosion.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for character movement during the explosion."
+
     explosion_speed: float = ArgField(
         cmd_name=["--explosion-speed"],
         type_parser=arg_validators.PositiveFloat.type_parser,
         default=0.75,
         metavar=arg_validators.PositiveFloat.METAVAR,
         help="Speed of characters during explosion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
     )  # type: ignore[assignment]
+    "float : Speed of characters during explosion. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect."
+
     reassembly_ease: easing.EasingFunction = ArgField(
         cmd_name=["--reassembly-ease"],
         type_parser=arg_validators.Ease.type_parser,
         default=easing.out_expo,
         help="Easing function to use for character reassembly.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for character reassembly."
+
     reassembly_speed: float = ArgField(
         cmd_name=["--reassembly-speed"],
         type_parser=arg_validators.PositiveFloat.type_parser,
         default=0.75,
         metavar=arg_validators.PositiveFloat.METAVAR,
         help="Speed of characters during reassembly. Note: Speed effects the number of steps in the easing function. Adjust speed and animation rate separately to fine tune the effect.",
     )  # type: ignore[assignment]
+    "float : Speed of characters during reassembly."
 
     @classmethod
     def get_effect_class(cls):
-        return UnstableEffect
+        return Unstable
 
 
-class UnstableEffect:
+class UnstableIterator(BaseEffectIterator[UnstableConfig]):
     """Effect that spawns characters jumbled, explodes them to the edge of the output area,
     then reassembles them in the correct layout."""
 
-    def __init__(self, terminal: Terminal, args: UnstableEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.jumbled_coords: dict[EffectCharacter, Coord] = dict()
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by jumbling the character positions and
-        choosing a location on the perimeter of the output area for the character to travel
-        after exploding. Creates all waypoints and scenes for the characters."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def __init__(self, effect: "Unstable") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._jumbled_coords: dict[EffectCharacter, Coord] = dict()
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
+
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        character_coords = [character.input_coord for character in self.terminal.get_characters()]
-        for character in self.terminal.get_characters():
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        character_coords = [character.input_coord for character in self._terminal.get_characters()]
+        for character in self._terminal.get_characters():
             pos = random.randint(0, 3)
             match pos:
                 case 0:
-                    col = self.terminal.output_area.left
-                    row = random.randint(1, self.terminal.output_area.top)
+                    col = self._terminal.output_area.left
+                    row = random.randint(1, self._terminal.output_area.top)
                 case 1:
-                    col = self.terminal.output_area.right
-                    row = random.randint(1, self.terminal.output_area.top)
+                    col = self._terminal.output_area.right
+                    row = random.randint(1, self._terminal.output_area.top)
                 case 2:
-                    col = random.randint(1, self.terminal.output_area.right)
-                    row = self.terminal.output_area.bottom
+                    col = random.randint(1, self._terminal.output_area.right)
+                    row = self._terminal.output_area.bottom
                 case 3:
-                    col = random.randint(1, self.terminal.output_area.right)
-                    row = self.terminal.output_area.top
+                    col = random.randint(1, self._terminal.output_area.right)
+                    row = self._terminal.output_area.top
             jumbled_coord = character_coords.pop(random.randint(0, len(character_coords) - 1))
-            self.jumbled_coords[character] = jumbled_coord
+            self._jumbled_coords[character] = jumbled_coord
             character.motion.set_coordinate(jumbled_coord)
-            explosion_path = character.motion.new_path(id="explosion", speed=1.25, ease=self.args.explosion_ease)
+            explosion_path = character.motion.new_path(id="explosion", speed=1.25, ease=self._config.explosion_ease)
             explosion_path.new_waypoint(Coord(col, row))
-            reassembly_path = character.motion.new_path(id="reassembly", speed=0.75, ease=self.args.reassembly_ease)
+            reassembly_path = character.motion.new_path(id="reassembly", speed=0.75, ease=self._config.reassembly_ease)
             reassembly_path.new_waypoint(character.input_coord)
             unstable_gradient = graphics.Gradient(
-                self.character_final_color_map[character], self.args.unstable_color, steps=25
+                self._character_final_color_map[character], self._config.unstable_color, steps=25
             )
             rumble_scn = character.animation.new_scene(id="rumble")
             rumble_scn.apply_gradient_to_symbols(
                 unstable_gradient,
                 character.input_symbol,
                 10,
             )
             final_color = graphics.Gradient(
-                self.args.unstable_color, self.character_final_color_map[character], steps=12
+                self._config.unstable_color, self._character_final_color_map[character], steps=12
             )
             final_scn = character.animation.new_scene(id="final")
             final_scn.apply_gradient_to_symbols(final_color, character.input_symbol, 5)
             character.animation.activate_scene(rumble_scn)
-            self.terminal.set_character_visibility(character, True)
+            self._terminal.set_character_visibility(character, True)
+        self._explosion_hold_time = 50
+        self.phase = "rumble"
+        self._max_rumble_steps = 250
+        self._current_rumble_steps = 0
+        self._rumble_mod_delay = 20
+
+    def __next__(self) -> str:
+        next_frame = None
+        if self.phase == "rumble":
+            if self._current_rumble_steps < self._max_rumble_steps:
+                if self._current_rumble_steps > 30 and self._current_rumble_steps % self._rumble_mod_delay == 0:
+                    row_offset = random.choice([-1, 0, 1])
+                    column_offset = random.choice([-1, 0, 1])
+                    for character in self._terminal.get_characters():
+                        character.motion.set_coordinate(
+                            Coord(
+                                character.motion.current_coord.column + column_offset,
+                                character.motion.current_coord.row + row_offset,
+                            )
+                        )
+                        character.animation.step_animation()
+                    next_frame = self._terminal.get_formatted_output_string()
+                    for character in self._terminal.get_characters():
+                        character.motion.set_coordinate(self._jumbled_coords[character])
+                    self._rumble_mod_delay -= 1
+                    self._rumble_mod_delay = max(self._rumble_mod_delay, 1)
+                else:
+                    for character in self._terminal.get_characters():
+                        character.animation.step_animation()
+                    next_frame = self._terminal.get_formatted_output_string()
 
-    def move_all_to_waypoint(self, path_id) -> None:
-        for character in self.terminal.get_characters():
-            if path_id == "reassembly":
-                character.animation.activate_scene(character.animation.query_scene("final"))
-            self.active_chars.append(character)
-            character.motion.activate_path(character.motion.query_path(path_id))
-        while self.active_chars:
-            self.terminal.print()
-            self.animate_chars()
-            if path_id == "reassembly":
-                self.active_chars = [
+                self._current_rumble_steps += 1
+            else:
+                self.phase = "explosion"
+                for character in self._terminal.get_characters():
+                    character.motion.activate_path(character.motion.query_path("explosion"))
+                self._active_chars = [character for character in self._terminal.get_characters()]
+
+        if self.phase == "explosion":
+            if self._active_chars:
+                for character in self._active_chars:
+                    character.tick()
+                self._active_chars = [
                     character
-                    for character in self.active_chars
-                    if not character.motion.current_coord == character.motion.query_path(path_id).waypoints[0].coord
-                    or not character.animation.active_scene_is_complete()
+                    for character in self._active_chars
+                    if not character.motion.current_coord == character.motion.query_path("explosion").waypoints[0].coord
                 ]
+                next_frame = self._terminal.get_formatted_output_string()
+
+            elif self._explosion_hold_time:
+                for character in self._active_chars:
+                    character.tick()
+                self._explosion_hold_time -= 1
+                next_frame = self._terminal.get_formatted_output_string()
             else:
-                self.active_chars = [
+                self.phase = "reassembly"
+                for character in self._terminal.get_characters():
+                    character.animation.activate_scene(character.animation.query_scene("final"))
+                    self._active_chars.append(character)
+                    character.motion.activate_path(character.motion.query_path("reassembly"))
+
+        if self.phase == "reassembly":
+            if self._active_chars:
+                for character in self._active_chars:
+                    character.tick()
+                self._active_chars = [
                     character
-                    for character in self.active_chars
-                    if not character.motion.current_coord == character.motion.query_path(path_id).waypoints[0].coord
+                    for character in self._active_chars
+                    if not character.motion.current_coord
+                    == character.motion.query_path("reassembly").waypoints[0].coord
+                    or not character.animation.active_scene_is_complete()
                 ]
+                next_frame = self._terminal.get_formatted_output_string()
 
-    def rumble(self) -> None:
-        max_rumble_steps = 250
-        current_rumble_steps = 0
-        rumble_mod_delay = 20
-        while current_rumble_steps < max_rumble_steps:
-            if current_rumble_steps > 30 and current_rumble_steps % rumble_mod_delay == 0:
-                row_offset = random.choice([-1, 0, 1])
-                column_offset = random.choice([-1, 0, 1])
-                for character in self.terminal.get_characters():
-                    character.motion.set_coordinate(
-                        Coord(
-                            character.motion.current_coord.column + column_offset,
-                            character.motion.current_coord.row + row_offset,
-                        )
-                    )
-                    character.animation.step_animation()
-                self.terminal.print()
-                for character in self.terminal.get_characters():
-                    character.motion.set_coordinate(self.jumbled_coords[character])
-                rumble_mod_delay -= 1
-                rumble_mod_delay = max(rumble_mod_delay, 1)
-            else:
-                for character in self.terminal.get_characters():
-                    character.animation.step_animation()
-                self.terminal.print()
-
-            current_rumble_steps += 1
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        explosion_hold_time = 50
-        self.rumble()
-        self.move_all_to_waypoint("explosion")
-        while explosion_hold_time:
-            self.terminal.print()
-            self.animate_chars()
-            explosion_hold_time -= 1
-        self.move_all_to_waypoint("reassembly")
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method."""
-        for character in self.active_chars:
-            character.tick()
+        if next_frame is not None:
+            return next_frame
+        else:
+            raise StopIteration
+
+
+class Unstable(BaseEffect[UnstableConfig]):
+    _config_cls = UnstableConfig
+    _iterator_cls = UnstableIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_vhstape.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_vhstape.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,136 @@
 import random
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import animation, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
 from terminaltexteffects.utils.geometry import Coord
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return VHSTapeEffect, VHSTapeEffectArgs
+    return VHSTape, VHSTapeConfig
 
 
 @argclass(
     name="vhstape",
-    formatter_class=arg_validators.CustomFormatter,
     help="Lines of characters glitch left and right and lose detail like an old VHS tape.",
     description="vhstape | Lines of characters glitch left and right and lose detail like an old VHS tape.",
     epilog="""Example: terminaltexteffects vhstape --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --glitch-line-colors ffffff ff0000 00ff00 0000ff ffffff --glitch-wave-colors ffffff ff0000 00ff00 0000ff ffffff --noise-colors 1e1e1f 3c3b3d 6d6c70 a2a1a6 cbc9cf ffffff --glitch-line-chance 0.05 --noise-chance 0.004 --total-glitch-time 1000""",
 )
 @dataclass
-class VHSTapeEffectArgs(ArgsDataClass):
+class VHSTapeConfig(ArgsDataClass):
+    """Configuration for the VHSTape effect.
+
+    Attributes:
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        glitch_line_colors (tuple[graphics.Color, ...]): Tuple of colors for the characters when a single line is glitching. Colors are applied in order as an animation.
+        glitch_wave_colors (tuple[graphics.Color, ...]): Tuple of colors for the characters in lines that are part of the glitch wave. Colors are applied in order as an animation.
+        noise_colors (tuple[graphics.Color, ...]): Tuple of colors for the characters during the noise phase.
+        glitch_line_chance (float): Chance that a line will glitch on any given frame.
+        noise_chance (float): Chance that all characters will experience noise on any given frame.
+        total_glitch_time (int): Total time, animation steps, that the glitching phase will last."""
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("ab48ff", "e7b2b2", "fffebd"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.VERTICAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     glitch_line_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--glitch-line-colors",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("ffffff", "ff0000", "00ff00", "0000ff", "ffffff"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the characters when a single line is glitching. Colors are applied in order as an animation.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the characters when a single line is glitching. Colors are applied in order as an animation."
+
     glitch_wave_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--glitch-wave-colors",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("ffffff", "ff0000", "00ff00", "0000ff", "ffffff"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the characters in lines that are part of the glitch wave. Colors are applied in order as an animation.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the characters in lines that are part of the glitch wave. Colors are applied in order as an animation."
+
     noise_colors: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--noise-colors",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("1e1e1f", "3c3b3d", "6d6c70", "a2a1a6", "cbc9cf", "ffffff"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the characters during the noise phase.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the characters during the noise phase."
+
     glitch_line_chance: float = ArgField(
         cmd_name="--glitch-line-chance",
         type_parser=arg_validators.Ratio.type_parser,
         default=0.05,
         metavar=arg_validators.Ratio.METAVAR,
         help="Chance that a line will glitch on any given frame.",
     )  # type: ignore[assignment]
+    "float : Chance that a line will glitch on any given frame."
+
     noise_chance: float = ArgField(
         cmd_name="--noise-chance",
         type_parser=arg_validators.Ratio.type_parser,
         default=0.004,
         metavar=arg_validators.Ratio.METAVAR,
         help="Chance that all characters will experience noise on any given frame.",
     )  # type: ignore[assignment]
+    "float : Chance that all characters will experience noise on any given frame."
+
     total_glitch_time: int = ArgField(
         cmd_name="--total-glitch-time",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=1000,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Total time, animation steps, that the glitching phase will last.",
     )  # type: ignore[assignment]
+    "int : Total time, animation steps, that the glitching phase will last."
 
     @classmethod
     def get_effect_class(cls):
-        return VHSTapeEffect
+        return VHSTape
 
 
-class Line:
+class _Line:
     """
     Represents a line of characters with various effects.
 
     Args:
         characters (list[EffectCharacter]): List of EffectCharacter objects representing the characters in the line.
         args (argparse.Namespace): Namespace object containing command-line arguments.
 
@@ -119,15 +148,15 @@
         line_movement_complete(): Checks if the movement of all characters in the line is complete.
 
     """
 
     def __init__(
         self,
         characters: list[EffectCharacter],
-        args: VHSTapeEffectArgs,
+        args: VHSTapeConfig,
         character_final_color_map: dict[EffectCharacter, graphics.Color],
     ) -> None:
         self.characters = characters
         self.args = args
         self.character_final_color_map = character_final_color_map
         self.build_line_effects()
 
@@ -261,175 +290,172 @@
         for character in self.characters:
             character.motion.activate_path(character.motion.query_path(path_id))
 
     def line_movement_complete(self):
         return all(character.motion.movement_is_complete() for character in self.characters)
 
 
-class VHSTapeEffect:
+class VHSTapeIterator(BaseEffectIterator[VHSTapeConfig]):
     """
     Represents a VHS tape effect for terminal text.
-
-    Attributes:
-        terminal (Terminal): The terminal object.
-        args (VHSTapeEffectArgs): The command-line arguments.
-        pending_chars (list[EffectCharacter]): The list of pending effect characters.
-        animating_chars (list[EffectCharacter]): The list of animating effect characters.
-        lines (dict[int, Line]): The dictionary of lines indexed by row index.
-        active_glitch_wave_top (int | None): The top row index of the active glitch wave, or None if no active wave.
-        active_glitch_wave_lines (list[Line]): The list of lines in the active glitch wave.
-        active_glitch_lines (list[Line]): The list of active glitch lines.
     """
 
-    def __init__(self, terminal: Terminal, args: VHSTapeEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.lines: dict[int, Line] = {}
-        self.active_glitch_wave_top: int | None = None
-        self.active_glitch_wave_lines: list[Line] = []
-        self.active_glitch_lines: list[Line] = []
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+    def __init__(self, effect: "VHSTape") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._lines: dict[int, _Line] = {}
+        self._active_glitch_wave_top: int | None = None
+        self._active_glitch_wave_lines: list[_Line] = []
+        self._active_glitch_lines: list[_Line] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def prepare_data(self) -> None:
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         for row_index, characters in enumerate(
-            self.terminal.get_characters_grouped(grouping=self.terminal.CharacterGroup.ROW_BOTTOM_TO_TOP)
+            self._terminal.get_characters_grouped(grouping=self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP)
         ):
-            self.lines[row_index] = Line(characters, self.args, self.character_final_color_map)
-        for character in self.terminal.get_characters():
-            self.terminal.set_character_visibility(character, True)
+            self._lines[row_index] = _Line(characters, self._config, self._character_final_color_map)
+        for character in self._terminal.get_characters():
+            self._terminal.set_character_visibility(character, True)
             character.animation.activate_scene(character.animation.query_scene("base"))
-
-    def glitch_wave(self) -> None:
-        if not self.active_glitch_wave_top:
-            if self.terminal.output_area.top >= 3:
+        self._glitching_steps_elapsed = 0
+        self._phase = "glitching"
+        self._to_redraw = list(self._lines.values())
+        self._redrawing = False
+
+    def _glitch_wave(self) -> None:
+        if not self._active_glitch_wave_top:
+            if self._terminal.output_area.top >= 3:
                 # choose a wave top index in the top half of the output area or at least 3 rows up
-                self.active_glitch_wave_top = random.randint(
-                    max((3, round(self.terminal.output_area.top * 0.5))), self.terminal.output_area.top
+                self._active_glitch_wave_top = random.randint(
+                    max((3, round(self._terminal.output_area.top * 0.5))), self._terminal.output_area.top
                 )
             else:
                 # not enough room for a wave
                 return
 
         # if all lines have completed movement, proceed to move/restore wave
-        if all(line.line_movement_complete() for line in self.active_glitch_wave_lines):
-            if self.active_glitch_wave_lines:
+        if all(line.line_movement_complete() for line in self._active_glitch_wave_lines):
+            if self._active_glitch_wave_lines:
                 # only move 30% of the time
                 if random.random() < 0.3:
                     # if moving, only move up 10% of the time
                     if random.random() < 0.3:
                         wave_top_delta = 1
                     else:
                         wave_top_delta = -1
                 else:
                     wave_top_delta = 0
-                self.active_glitch_wave_top += wave_top_delta
+                self._active_glitch_wave_top += wave_top_delta
                 # clamp wave top to output area
-                self.active_glitch_wave_top = max(2, min(self.active_glitch_wave_top, self.terminal.output_area.top))
+                self._active_glitch_wave_top = max(2, min(self._active_glitch_wave_top, self._terminal.output_area.top))
             # get the lines for the wave
-            new_wave_lines: list[Line] = []
-            for line_index in range(self.active_glitch_wave_top - 2, self.active_glitch_wave_top + 1):
-                if line_index in self.lines:
-                    new_wave_lines.append(self.lines[line_index])
+            new_wave_lines: list[_Line] = []
+            for line_index in range(self._active_glitch_wave_top - 2, self._active_glitch_wave_top + 1):
+                if line_index in self._lines:
+                    new_wave_lines.append(self._lines[line_index])
 
             # restore any lines that are no longer part of the wave
-            for line in self.active_glitch_wave_lines:
+            for line in self._active_glitch_wave_lines:
                 if line not in new_wave_lines:
                     line.restore()
-                    self.active_chars.extend(line.characters)
-            self.active_glitch_wave_lines = new_wave_lines
+                    self._active_chars.extend(line.characters)
+            self._active_glitch_wave_lines = new_wave_lines
 
-            if self.active_glitch_wave_top < 3:
+            if self._active_glitch_wave_top < 3:
                 # wave at bottom, restore lines
-                for line in self.active_glitch_wave_lines:
+                for line in self._active_glitch_wave_lines:
                     line.restore()
-                    self.active_chars.extend(line.characters)
-                self.active_glitch_wave_top = None
-                self.active_glitch_wave_lines = []
+                    self._active_chars.extend(line.characters)
+                self._active_glitch_wave_top = None
+                self._active_glitch_wave_lines = []
 
             else:
                 for line, path_id in zip(
-                    self.active_glitch_wave_lines, ("glitch_wave_mid", "glitch_wave_end", "glitch_wave_mid")
+                    self._active_glitch_wave_lines, ("glitch_wave_mid", "glitch_wave_end", "glitch_wave_mid")
                 ):
                     line.activate_path(path_id)
-                    self.active_chars.extend(line.characters)
+                    self._active_chars.extend(line.characters)
 
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-
-        self.terminal.print()
-        glitching_steps_elapsed = 0
-        phase = "glitching"
-        to_redraw = list(self.lines.values())
-        redrawing = False
-        while phase != "complete" or self.active_chars:
-            if phase == "glitching":
+    def __next__(self) -> str:
+        if self._phase != "complete" or self._active_chars:
+            if self._phase == "glitching":
                 # Check if all active glitch wave lines have completed their movement, if so move the wave
-                if not self.active_glitch_wave_lines or all(
-                    line.line_movement_complete() for line in self.active_glitch_wave_lines
+                if not self._active_glitch_wave_lines or all(
+                    line.line_movement_complete() for line in self._active_glitch_wave_lines
                 ):
-                    self.glitch_wave()
+                    self._glitch_wave()
                 # Remove completed glitch lines from active glitch lines
-                self.active_glitch_lines = [
-                    line for line in self.active_glitch_lines if not line.line_movement_complete()
+                self._active_glitch_lines = [
+                    line for line in self._active_glitch_lines if not line.line_movement_complete()
                 ]
                 # Randomly add new glitch lines
-                if random.random() < self.args.glitch_line_chance and len(self.active_glitch_lines) < 3:
-                    glitch_line: Line = random.choice(list(self.lines.values()))
-                    if glitch_line not in self.active_glitch_wave_lines and glitch_line not in self.active_glitch_lines:
+                if random.random() < self._config.glitch_line_chance and len(self._active_glitch_lines) < 3:
+                    glitch_line: _Line = random.choice(list(self._lines.values()))
+                    if (
+                        glitch_line not in self._active_glitch_wave_lines
+                        and glitch_line not in self._active_glitch_lines
+                    ):
                         glitch_line.set_hold_time(random.randint(30, 120))
-                        self.active_glitch_lines.append(glitch_line)
+                        self._active_glitch_lines.append(glitch_line)
                         glitch_line.glitch()
-                        self.active_chars.extend(glitch_line.characters)
+                        self._active_chars.extend(glitch_line.characters)
                 # Randomly add noise to all lines
-                if random.random() < self.args.noise_chance:
-                    for line in self.lines.values():
+                if random.random() < self._config.noise_chance:
+                    for line in self._lines.values():
                         line.snow()
-                        if line not in self.active_glitch_wave_lines and line not in self.active_glitch_lines:
-                            self.active_chars.extend(line.characters)
-                glitching_steps_elapsed += 1
+                        if line not in self._active_glitch_wave_lines and line not in self._active_glitch_lines:
+                            self._active_chars.extend(line.characters)
+                self._glitching_steps_elapsed += 1
                 # Check if glitching time has reached the total glitch time
-                if glitching_steps_elapsed >= self.args.total_glitch_time:
+                if self._glitching_steps_elapsed >= self._config.total_glitch_time:
                     # Restore glitch wave lines
-                    for line in self.active_glitch_wave_lines:
+                    for line in self._active_glitch_wave_lines:
                         line.restore()
                     # Restore glitch lines
-                    for line in self.active_glitch_lines:
+                    for line in self._active_glitch_lines:
                         line.restore()
-                    phase = "noise"
+                    self._phase = "noise"
 
-            elif phase == "noise":
+            elif self._phase == "noise":
                 # Activate final snow animation for all characters
-                if not self.active_chars:
-                    for character in self.terminal.get_characters():
+                if not self._active_chars:
+                    for character in self._terminal.get_characters():
                         character.animation.activate_scene(character.animation.query_scene("final_snow"))
-                        self.active_chars.append(character)
-                    phase = "redraw"
+                        self._active_chars.append(character)
+                    self._phase = "redraw"
 
-            elif phase == "redraw":
+            elif self._phase == "redraw":
                 # Redraw lines one by one
-                if redrawing or not self.active_chars:
-                    redrawing = True
-                    if to_redraw:
-                        next_line = to_redraw.pop()
+                if self._redrawing or not self._active_chars:
+                    self._redrawing = True
+                    if self._to_redraw:
+                        next_line = self._to_redraw.pop()
                         for character in next_line.characters:
                             character.animation.activate_scene(character.animation.query_scene("final_redraw"))
-                            self.active_chars.append(character)
+                            self._active_chars.append(character)
                     else:
-                        phase = "complete"
-            self.animate_chars()
-            self.terminal.print()
-
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+                        self._phase = "complete"
+            for character in self._active_chars:
+                character.tick()
+
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class VHSTape(BaseEffect[VHSTapeConfig]):
+    """Lines of characters glitch left and right and lose detail like an old VHS tape."""
+
+    _config_cls = VHSTapeConfig
+    _iterator_cls = VHSTapeIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/effects/effect_waves.py` & `terminaltexteffects-0.8.0/terminaltexteffects/effects/effect_waves.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,186 @@
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter, EventHandler
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
-from terminaltexteffects.utils.terminal import Terminal
 
 
 def get_effect_and_args() -> tuple[type[typing.Any], type[ArgsDataClass]]:
-    return WavesEffect, WavesEffectArgs
+    return Waves, WavesConfig
 
 
 @argclass(
     name="waves",
-    formatter_class=arg_validators.CustomFormatter,
     help="Waves travel across the terminal leaving behind the characters.",
     description="waves | Waves travel across the terminal leaving behind the characters.",
     epilog=f"""{arg_validators.EASING_EPILOG}
 Example: terminaltexteffects waves --wave-symbols ▁ ▂ ▃ ▄ ▅ ▆ ▇ █ ▇ ▆ ▅ ▄ ▃ ▂ ▁ --wave-gradient-stops f0ff65 ffb102 31a0d4 ffb102 f0ff65 --wave-gradient-steps 6 --final-gradient-stops ffb102 31a0d4 f0ff65 --final-gradient-steps 12 --wave-count 7 --wave-length 2 --wave-easing IN_OUT_SINE""",
 )
 @dataclass
-class WavesEffectArgs(ArgsDataClass):
+class WavesConfig(ArgsDataClass):
+    """Configuration for the Waves effect.
+
+    Attributes:
+        wave_symbols (tuple[str, ...]): Symbols to use for the wave animation. Multi-character strings will be used in sequence to create an animation.
+        wave_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        wave_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_stops (tuple[graphics.Color, ...]): Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.
+        final_gradient_steps (tuple[int, ...]): Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.
+        final_gradient_direction (graphics.Gradient.Direction): Direction of the gradient for the final color.
+        wave_count (int): Number of waves to generate. n > 0."""
+
     wave_symbols: tuple[str, ...] = ArgField(
         cmd_name="--wave-symbols",
         type_parser=arg_validators.Symbol.type_parser,
         default=("▁", "▂", "▃", "▄", "▅", "▆", "▇", "█", "▇", "▆", "▅", "▄", "▃", "▂", "▁"),
         nargs="+",
         metavar=arg_validators.Symbol.METAVAR,
         help="Symbols to use for the wave animation. Multi-character strings will be used in sequence to create an animation.",
     )  # type: ignore[assignment]
+    "tuple[str, ...] : Symbols to use for the wave animation. Multi-character strings will be used in sequence to create an animation."
+
     wave_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--wave-gradient-stops",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("f0ff65", "ffb102", "31a0d4", "ffb102", "f0ff65"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     wave_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--wave-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(6,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name="--final-gradient-stops",
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("ffb102", "31a0d4", "f0ff65"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+    "tuple[graphics.Color, ...] : Tuple of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color."
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+    "tuple[int, ...] : Tuple of the number of gradient steps to use. More steps will create a smoother and longer gradient animation."
+
     final_gradient_direction: graphics.Gradient.Direction = ArgField(
         cmd_name="--final-gradient-direction",
         type_parser=arg_validators.GradientDirection.type_parser,
         default=graphics.Gradient.Direction.DIAGONAL,
         metavar=arg_validators.GradientDirection.METAVAR,
         help="Direction of the gradient for the final color.",
     )  # type: ignore[assignment]
+    "graphics.Gradient.Direction : Direction of the gradient for the final color."
+
     wave_count: int = ArgField(
         cmd_name="--wave-count",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=7,
         help="Number of waves to generate. n > 0.",
     )  # type: ignore[assignment]
+    "int : Number of waves to generate. n > 0."
+
     wave_length: int = ArgField(
         cmd_name="--wave-length",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=2,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="The number of frames for each step of the wave. Higher wave-lengths will create a slower wave.",
     )  # type: ignore[assignment]
+    "int : The number of frames for each step of the wave. Higher wave-lengths will create a slower wave."
+
     wave_easing: easing.EasingFunction = ArgField(
         cmd_name="--wave-easing",
         type_parser=arg_validators.Ease.type_parser,
         default=easing.in_out_sine,
         help="Easing function to use for wave travel.",
     )  # type: ignore[assignment]
+    "easing.EasingFunction : Easing function to use for wave travel."
 
     @classmethod
     def get_effect_class(cls):
-        return WavesEffect
+        return Waves
 
 
-class WavesEffect:
+class WavesIterator(BaseEffectIterator[WavesConfig]):
     """Effect that creates waves that travel across the terminal, leaving behind the characters."""
 
-    def __init__(self, terminal: Terminal, args: WavesEffectArgs):
-        self.terminal = terminal
-        self.args = args
-        self.pending_columns: list[list[EffectCharacter]] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        """Prepares the data for the effect by creating the wave animations."""
-        final_gradient = graphics.Gradient(*self.args.final_gradient_stops, steps=self.args.final_gradient_steps)
+    def __init__(self, effect: "Waves") -> None:
+        super().__init__(effect)
+        self._pending_columns: list[list[EffectCharacter]] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
+
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self.terminal.output_area.top, self.terminal.output_area.right, self.args.final_gradient_direction
+            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
         )
-        wave_gradient = graphics.Gradient(*self.args.wave_gradient_stops, steps=self.args.wave_gradient_steps)
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        wave_gradient = graphics.Gradient(*self._config.wave_gradient_stops, steps=self._config.wave_gradient_steps)
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
             wave_scn = character.animation.new_scene()
-            wave_scn.ease = self.args.wave_easing
-            for _ in range(self.args.wave_count):
+            wave_scn.ease = self._config.wave_easing
+            for _ in range(self._config.wave_count):
                 wave_scn.apply_gradient_to_symbols(
-                    wave_gradient, self.args.wave_symbols, duration=self.args.wave_length
+                    wave_gradient, self._config.wave_symbols, duration=self._config.wave_length
                 )
             final_scn = character.animation.new_scene()
             for step in graphics.Gradient(
                 wave_gradient.spectrum[-1],
-                self.character_final_color_map[character],
-                steps=self.args.final_gradient_steps,
+                self._character_final_color_map[character],
+                steps=self._config.final_gradient_steps,
             ):
                 final_scn.add_frame(character.input_symbol, 10, color=step)
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE, wave_scn, EventHandler.Action.ACTIVATE_SCENE, final_scn
             )
             character.animation.activate_scene(wave_scn)
-        for column in self.terminal.get_characters_grouped(grouping=self.terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT):
-            self.pending_columns.append(column)
-
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        while self.pending_columns or self.active_chars:
-            if self.pending_columns:
-                next_column = self.pending_columns.pop(0)
+        for column in self._terminal.get_characters_grouped(
+            grouping=self._terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT
+        ):
+            self._pending_columns.append(column)
+
+    def __next__(self) -> str:
+        if self._pending_columns or self._active_chars:
+            if self._pending_columns:
+                next_column = self._pending_columns.pop(0)
                 for character in next_column:
-                    self.terminal.set_character_visibility(character, True)
-                    self.active_chars.append(character)
-            self.terminal.print()
-            self.animate_chars()
-
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+                    self._terminal.set_character_visibility(character, True)
+                    self._active_chars.append(character)
+            for character in self._active_chars:
+                character.tick()
+            self._active_chars = [character for character in self._active_chars if character.is_active]
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class Waves(BaseEffect[WavesConfig]):
+    """Effect that creates waves that travel across the terminal, leaving behind the characters."""
+
+    _config_cls = WavesConfig
+    _iterator_cls = WavesIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/template/effect_template.py` & `terminaltexteffects-0.8.0/terminaltexteffects/template/effect_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,125 @@
-import argparse
 import typing
 from dataclasses import dataclass
 
 import terminaltexteffects.utils.arg_validators as arg_validators
 from terminaltexteffects.base_character import EffectCharacter
+from terminaltexteffects.base_effect import BaseEffect, BaseEffectIterator
 from terminaltexteffects.utils import easing, graphics
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass, argclass
-from terminaltexteffects.utils.terminal import Terminal
 
 
 @argclass(
     name="namedeffect",
-    formatter_class=arg_validators.CustomFormatter,
     help="effect_description",
     description="effect_description",
     epilog=f"""{arg_validators.EASING_EPILOG}
     """,
 )
 @dataclass
-class NamedEffectArgs(ArgsDataClass):
+class EffectConfig(ArgsDataClass):
     color_single: graphics.Color = ArgField(
         cmd_name=["--color-single"],
         type_parser=arg_validators.Color.type_parser,
         default=0,
         metavar=arg_validators.Color.METAVAR,
         help="Color for the ___.",
     )  # type: ignore[assignment]
+
     color_list: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--color-list"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=0,
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the ___.",
     )  # type: ignore[assignment]
+
     final_color: graphics.Color = ArgField(
         cmd_name=["--final-color"],
         type_parser=arg_validators.Color.type_parser,
         default="ffffff",
         metavar=arg_validators.Color.METAVAR,
         help="Color for the final character.",
     )  # type: ignore[assignment]
+
     final_gradient_stops: tuple[graphics.Color, ...] = ArgField(
         cmd_name=["--final-gradient-stops"],
         type_parser=arg_validators.Color.type_parser,
         nargs="+",
         default=("8A008A", "00D1FF", "FFFFFF"),
         metavar=arg_validators.Color.METAVAR,
         help="Space separated, unquoted, list of colors for the character gradient (applied from bottom to top). If only one color is provided, the characters will be displayed in that color.",
     )  # type: ignore[assignment]
+
     final_gradient_steps: tuple[int, ...] = ArgField(
         cmd_name="--final-gradient-steps",
         type_parser=arg_validators.PositiveInt.type_parser,
         nargs="+",
         default=(12,),
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Space separated, unquoted, list of the number of gradient steps to use. More steps will create a smoother and longer gradient animation.",
     )  # type: ignore[assignment]
+
     final_gradient_frames: int = ArgField(
         cmd_name="--final-gradient-frames",
         type_parser=arg_validators.PositiveInt.type_parser,
         default=5,
         metavar=arg_validators.PositiveInt.METAVAR,
         help="Number of frames to display each gradient step.",
     )  # type: ignore[assignment]
+
     movement_speed: float = ArgField(
         cmd_name="--movement-speed",
         type_parser=arg_validators.PositiveFloat.type_parser,
         default=1,
         metavar=arg_validators.PositiveFloat.METAVAR,
         help="Speed of the ___.",
     )  # type: ignore[assignment]
+
     easing: typing.Callable = ArgField(
         cmd_name=["--easing"],
         default=easing.in_out_sine,
         type_parser=arg_validators.Ease.type_parser,
         help="Easing function to use for character movement.",
     )  # type: ignore[assignment]
 
     @classmethod
     def get_effect_class(cls):
         return NamedEffect
 
 
-class NamedEffect:
-    """Effect that ___."""
-
-    def __init__(self, terminal: Terminal, args: argparse.Namespace):
-        self.terminal = terminal
-        self.args = args
-        self.pending_chars: list[EffectCharacter] = []
-        self.active_chars: list[EffectCharacter] = []
-        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-
-    def prepare_data(self) -> None:
-        final_gradient = graphics.Gradient(self.args.final_gradient_stops, self.args.final_gradient_steps)
-        for character in self.terminal.get_characters():
-            self.character_final_color_map[character] = final_gradient.get_color_at_fraction(
-                character.input_coord.row / self.terminal.output_area.top
+class NamedEffectIterator(BaseEffectIterator[EffectConfig]):
+    def __init__(self, effect: "NamedEffect") -> None:
+        super().__init__(effect)
+        self._pending_chars: list[EffectCharacter] = []
+        self._active_chars: list[EffectCharacter] = []
+        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self._build()
+
+    def _build(self) -> None:
+        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+        for character in self._terminal.get_characters():
+            self._character_final_color_map[character] = final_gradient.get_color_at_fraction(
+                character.input_coord.row / self._terminal.output_area.top
             )
 
             # do something with the data if needed (sort, adjust positions, etc)
 
-    def run(self) -> None:
-        """Runs the effect."""
-        self.prepare_data()
-        while self.pending_chars or self.active_chars:
-            self.terminal.print()
-            self.animate_chars()
-
-            self.active_chars = [character for character in self.active_chars if character.is_active]
-
-    def animate_chars(self) -> None:
-        """Animates the characters by calling the tick method on all active characters."""
-        for character in self.active_chars:
-            character.tick()
+    def __next__(self) -> str:
+        if self._pending_chars or self._active_chars:
+            # perform effect logic
+            for character in self._active_chars:
+                character.tick()
+            return self._terminal.get_formatted_output_string()
+        else:
+            raise StopIteration
+
+
+class NamedEffect(BaseEffect[EffectConfig]):
+    """Effect description."""
+
+    _config_cls = EffectConfig
+    _iterator_cls = NamedEffectIterator
+
+    def __init__(self, input_data: str) -> None:
+        super().__init__(input_data)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/animation.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/animation.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/ansitools.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/ansitools.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/arg_validators.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/arg_validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -211,14 +211,48 @@
             return arg
         else:
             raise argparse.ArgumentTypeError(
                 f"invalid symbol: '{arg}' is not a valid symbol. Must be a single ASCII/UTF-8 character."
             )
 
 
+class TerminalDimensions:
+    """Argument type for terminal dimensions.
+
+    Terminal dimensions are a pair of non-negative integers separated by a space. Ex: 80 24
+
+    Raises:
+        argparse.ArgumentTypeError: Value is not a valid terminal dimension.
+    """
+
+    METAVAR = "(width height)"
+
+    @staticmethod
+    def type_parser(arg: str) -> int:
+        """Validates that the given argument is a valid terminal dimension.
+
+        Args:
+            arg (str): argument to validate
+
+        Returns:
+            tuple[int,int]: validated terminal dimension
+        """
+        try:
+            dimension = int(arg)
+            if dimension < 0:
+                raise argparse.ArgumentTypeError(
+                    f"invalid terminal dimensions: '{arg}' is not a valid terminal dimension. Must be >= 0."
+                )
+            return dimension
+        except ValueError:
+            raise argparse.ArgumentTypeError(
+                f"invalid terminal dimensions: '{arg}' is not a valid terminal dimension. Must be >= 0."
+            )
+
+
 class PositiveInt:
     """Argument type for positive integers.
 
     int(n) > 0
 
     Raises:
         argparse.ArgumentTypeError: Value is not a positive integer.
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/argsdataclass.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/argsdataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import argparse
 import inspect
 import typing
 from dataclasses import MISSING, Field, dataclass, fields
 
+from terminaltexteffects.utils.arg_validators import CustomFormatter
+
 
 class ArgField(Field):
     """
     A subclass of the dataclasses.Field class that represents a command-line argument.
 
     This class extends the built-in Field class to include additional metadata specific to command-line arguments.
     This metadata includes the command-line argument name, help text, type parser, metavar, nargs, action, required
@@ -42,15 +44,15 @@
     def __init__(
         self,
         # custom metadata
         cmd_name: str | list[str],
         help: str,
         type_parser: typing.Callable | None = None,
         metavar: str | None = None,
-        nargs: str | None = None,
+        nargs: str | int | None = None,
         action: str | None = None,
         required: bool = False,
         choices: list[str | int] | None = None,
         # python internal attrs
         default=MISSING,
         default_factory=MISSING,
         init=True,
@@ -77,29 +79,28 @@
         super().__init__(default, default_factory, init, repr, hash, compare, vars(additional_metadata), kw_only)
 
     @dataclass
     class FieldAdditionalMetaData:
         cmd_name: str | list[str]
         type_parser: typing.Any | None = None
         metavar: str | None = None
-        nargs: str | None = None
+        nargs: str | int | None = None
         help: str | None = None
         action: str | None = None
         required: bool = False
         choices: list[str | int] | None = None
 
 
 @dataclass
 class ArgParserDescriptor:
     """This dataclass contains required attributes to call "add_parser()" method of
     _argparse._SubParsersAction" class
     """
 
     name: str
-    formatter_class: typing.Any
     help: str
     description: str
     epilog: str
 
 
 @dataclass
 class ArgsDataClass:
@@ -111,15 +112,15 @@
 
     Note:
         This class does not define any fields itself. Instead, it is meant to be subclassed, with subclasses defining
         their own fields to represent the command-line arguments they expect.
     """
 
     @classmethod
-    def from_parsed_args_mapping(cls, parsed_args: argparse.Namespace, arg_class=None):
+    def _from_parsed_args_mapping(cls, parsed_args: argparse.Namespace, arg_class=None):
         """
         Creates an instance of the ArgsDataClass from parsed command-line arguments.
 
         This method takes a Namespace object, which is the result of parsing command-line arguments with argparse, and an
         optional class to instantiate. If no class is provided, it uses the 'arg_class' attribute from the parsed_args.
 
         It retrieves the signature of the __init__ method of the target class and iterates over its parameters. For each
@@ -153,15 +154,15 @@
                 param_value = tuple(param_value)
             params_dict[param] = param_value
 
         new_instance = arg_class(**params_dict)
         return new_instance
 
     @classmethod
-    def get_all_fields(cls) -> dict[str, Field]:
+    def _get_all_fields(cls) -> dict[str, Field]:
         """
         Retrieves all fields defined in the ArgsDataClass and returns them as a dictionary.
 
         This method uses the `fields` function from the `dataclasses` module to get a list of all fields defined in the
         ArgsDataClass. It then iterates over these fields, adding each one to a dictionary with the field's name as the key
         and the field itself as the value.
 
@@ -173,15 +174,15 @@
         fields_list = {}
         for f in fields(cls):
             fields_list[f.name] = f
 
         return fields_list
 
     @classmethod
-    def add_args_to_parser(cls, parser: argparse.ArgumentParser):
+    def _add_args_to_parser(cls, parser: argparse.ArgumentParser):
         """
         Adds arguments to the provided parser based on the fields defined in the ArgsDataClass.
 
         This method iterates over all fields in the ArgsDataClass. For each field, it checks if it has metadata.
         If metadata is present, it creates an instance of FieldAdditionalMetaData using the metadata.
         It then prepares a dictionary of argument descriptors, mapping field names to their corresponding values.
         These descriptors are used to add an argument to the parser with the `add_argument` method.
@@ -193,15 +194,15 @@
 
         Note:
             The 'type_parser' field name is specially handled and mapped to 'type' in the argument descriptors.
             The 'cmd_name' field is used as the name of the argument added to the parser. If 'cmd_name' is a string,
             it is wrapped in a list before being passed to `add_argument`.
             If a field has no metadata, it is skipped and no corresponding argument is added to the parser.
         """
-        arg_fields = cls.get_all_fields()
+        arg_fields = cls._get_all_fields()
         for arg in arg_fields.values():
             if not arg.metadata:
                 continue
             additional_metadata = ArgField.FieldAdditionalMetaData(**arg.metadata)
             if isinstance(additional_metadata.cmd_name, str):
                 additional_metadata.cmd_name = [additional_metadata.cmd_name]
             field_names_mapping = {"type_parser": "type"}
@@ -214,40 +215,38 @@
                     continue
                 if attr_name in field_names_mapping:
                     attr_name = field_names_mapping[attr_name]
 
                 arg_descriptor[attr_name] = value
 
             parser.add_argument(*additional_metadata.cmd_name, **arg_descriptor, default=arg.default)
+        parser.formatter_class = CustomFormatter
 
     @classmethod
-    def add_to_args_subparsers(cls, subparsers: argparse._SubParsersAction):
+    def _add_to_args_subparsers(cls, subparsers: argparse._SubParsersAction):
         """Adds arguments to the subparser.
 
         Args:
             arg_data_class (ArgsDataClass): ArgDataClass that required args defined in it
             subparser (argparse._SubParsersAction): subparser to add arguments to
         """
         sub_parser_descriptor = getattr(cls, "arg_class_metadata")
         new_parser = subparsers.add_parser(**vars(sub_parser_descriptor))
         new_parser.set_defaults(arg_class=cls)
-        cls.add_args_to_parser(new_parser)
+        cls._add_args_to_parser(new_parser)
 
 
-def argclass(name: str, formatter_class: typing.Any, help: str, description: str, epilog: str):
+def argclass(name: str, help: str, description: str, epilog: str):
     """Decorator for providing required metadata to an "ArgDataClass"
 
     Args:
         name (str): name for parser or subparser
-        formatter_class (any): formatter function for parser or subparser
         help (str): help string for parser or subparser
         description (str): description string for parser or subparser
         epilog (str): epilog string for parser or subparser
     """
 
     def decorator(cls):
-        cls.arg_class_metadata = ArgParserDescriptor(
-            name=name, formatter_class=formatter_class, help=help, description=description, epilog=epilog
-        )
+        cls.arg_class_metadata = ArgParserDescriptor(name=name, help=help, description=description, epilog=epilog)
         return cls
 
     return decorator
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/colorterm.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/colorterm.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/easing.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/easing.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/geometry.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/graphics.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Classes for storing and manipulating character graphics."""
 
 import itertools
 import typing
+from collections.abc import Iterator
 from enum import Enum, auto
 
 from terminaltexteffects.utils import colorterm, geometry, hexterm
 
 if typing.TYPE_CHECKING:
     pass
 
@@ -177,25 +178,16 @@
                 for column_value in range(1, max_column + 1):
                     fraction = ((row_value * 2) + column_value) / ((max_row * 2) + max_column)
                     color = self.get_color_at_fraction(fraction)
                     gradient_mapping[geometry.Coord(column_value, row_value)] = color
 
         return gradient_mapping
 
-    def __iter__(self) -> "Gradient":
-        self.index = 0
-        return self
-
-    def __next__(self) -> str:
-        if self.index < len(self.spectrum):
-            color = self.spectrum[self.index]
-            self.index += 1
-            return color
-        else:
-            raise StopIteration
+    def __iter__(self) -> Iterator[str]:
+        yield from self.spectrum
 
     def __len__(self) -> int:
         return len(self.spectrum)
 
     def __str__(self) -> str:
         color_blocks = [f"{colorterm.fg(color)}█{colorterm.RESET}" for color in self.spectrum]
         return f"Gradient: Stops({self.stops}), Steps({self.steps})\n" + "".join(color_blocks)
```

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/hexterm.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/hexterm.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/motion.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/motion.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.7.0/terminaltexteffects/utils/terminal.py` & `terminaltexteffects-0.8.0/terminaltexteffects/utils/terminal.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,46 +11,81 @@
 from terminaltexteffects.base_character import EffectCharacter
 from terminaltexteffects.utils import ansitools
 from terminaltexteffects.utils.argsdataclass import ArgField, ArgsDataClass
 from terminaltexteffects.utils.geometry import Coord
 
 
 @dataclass
-class TerminalArgs(ArgsDataClass):
+class TerminalConfig(ArgsDataClass):
+    """Configuration for the terminal.
+
+    Attributes:
+        tab_width (int): Number of spaces to use for a tab character.
+        xterm_colors (bool): Convert any colors specified in RBG hex to the closest XTerm-256 color.
+        no_color (bool): Disable all colors in the effect.
+        no_wrap (int): Disable wrapping of text.
+        animation_rate (float): Minimum time, in seconds, between animation steps.
+        use_terminal_dimensions (bool): Use the terminal dimensions to limit the size of the output area and support wrapping. If False, the output area is determined by the input data dimensions and may overflow the terminal width."""
+
     tab_width: int = ArgField(
         cmd_name=["--tab-width"],
         type_parser=arg_validators.PositiveInt.type_parser,
         metavar=arg_validators.PositiveInt.METAVAR,
         default=4,
         help="Number of spaces to use for a tab character.",
     )  # type: ignore[assignment]
 
+    "int : Number of spaces to use for a tab character."
+
     xterm_colors: bool = ArgField(
         cmd_name=["--xterm-colors"],
         default=False,
         action="store_true",
         help="Convert any colors specified in RBG hex to the closest XTerm-256 color.",
     )  # type: ignore[assignment]
 
+    "bool : Convert any colors specified in RBG hex to the closest XTerm-256 color."
+
     no_color: bool = ArgField(
         cmd_name=["--no-color"], default=False, action="store_true", help="Disable all colors in the effect."
     )  # type: ignore[assignment]
 
-    no_wrap: int = ArgField(cmd_name="--no-wrap", default=False, action="store_true", help="Disable wrapping of text.")  # type: ignore[assignment]
+    "bool : Disable all colors in the effect."
 
-    animation_rate: float = ArgField(
-        cmd_name=["-a", "--animation-rate"],
-        type_parser=arg_validators.NonNegativeFloat.type_parser,
-        default=0.01,
-        help="""Minimum time, in seconds, between animation steps. 
-        This value does not normally need to be modified. 
-        Use this to increase the playback speed of all aspects of the effect. 
-        This will have no impact beyond a certain lower threshold due to the 
-        processing speed of your device.""",
+    wrap_text: int = ArgField(
+        cmd_name="--wrap-text", default=False, action="store_true", help="Wrap text wider than the output area width."
+    )  # type: ignore[assignment]
+    "bool : Wrap text wider than the output area width."
+
+    frame_rate: float = ArgField(
+        cmd_name="--frame-rate",
+        type_parser=arg_validators.PositiveInt.type_parser,
+        default=100,
+        help="""Target frame rate for the animation.""",
+    )  # type: ignore[assignment]
+
+    "float : Minimum time, in seconds, between animation steps."
+
+    terminal_dimensions: tuple[int, int] = ArgField(
+        cmd_name=["--terminal-dimensions"],
+        type_parser=arg_validators.TerminalDimensions.type_parser,
+        nargs=2,
+        default=(0, 0),
+        help="Use the terminal dimensions to limit the size of the output area and support wrapping. If False, the output area is determined by the input data dimensions and may overflow the terminal width.",
+    )  # type: ignore[assignment]
+
+    "tuple(int,int) : Terminal dimensions as (width, height), if set to (0,0) the terminal dimensions are detected automatically."
+
+    ignore_terminal_dimensions: bool = ArgField(
+        cmd_name=["--ignore-terminal-dimensions"],
+        default=False,
+        action="store_true",
+        help="Ignore the terminal dimensions and use the input data dimensions for the output area.",
     )  # type: ignore[assignment]
+    "bool : Ignore the terminal dimensions and use the input data dimensions for the output area."
 
 
 @dataclass
 class OutputArea:
     """A class for storing the output area of an effect.
 
     Args:
@@ -138,20 +173,31 @@
         TOP_TO_BOTTOM_LEFT_TO_RIGHT = auto()
         TOP_TO_BOTTOM_RIGHT_TO_LEFT = auto()
         BOTTOM_TO_TOP_LEFT_TO_RIGHT = auto()
         BOTTOM_TO_TOP_RIGHT_TO_LEFT = auto()
         OUTSIDE_ROW_TO_MIDDLE = auto()
         MIDDLE_ROW_TO_OUTSIDE = auto()
 
-    def __init__(self, input_data: str, args: TerminalArgs):
-        self.input_data = input_data.replace("\t", " " * args.tab_width)
-        self.args = args
-        self.width, self.height = self._get_terminal_dimensions()
+    def __init__(self, input_data: str, config: TerminalConfig | None = None):
+        if config is None:
+            self.config = TerminalConfig()
+        else:
+            self.config = config
+        if not input_data:
+            input_data = "No Input."
+        self.input_data = input_data.replace("\t", " " * self.config.tab_width)
+        if self.config.ignore_terminal_dimensions:
+            self.width = max([len(line) for line in self.input_data.splitlines()])
+            self.height = len(self.input_data.splitlines()) + 1
+        elif self.config.terminal_dimensions == (0, 0):
+            self.width, self.height = self._get_terminal_dimensions()
+        else:
+            self.width, self.height = self.config.terminal_dimensions
         self.next_character_id = 0
-        self._input_characters = self._decompose_input(args.xterm_colors, args.no_color)
+        self._input_characters = self._decompose_input(self.config.xterm_colors, self.config.no_color)
         self._added_characters: list[EffectCharacter] = []
         self.input_width = max([character.input_coord.column for character in self._input_characters])
         self.input_height = max([character.input_coord.row for character in self._input_characters])
         self.output_area = OutputArea(min(self.height - 1, self.input_height), self.input_width)
         self._input_characters = [
             character
             for character in self._input_characters
@@ -159,20 +205,18 @@
             and character.input_coord.column <= self.output_area.right
         ]
         self.character_by_input_coord: dict[Coord, EffectCharacter] = {
             (character.input_coord): character for character in self._input_characters
         }
         self._fill_characters = self._make_fill_characters()
         self.visible_characters: set[EffectCharacter] = set()
-        self.animation_rate = args.animation_rate
+        self.frame_rate = self.config.frame_rate
         self.last_time_printed = time.time()
         self._update_terminal_state()
 
-        self._prep_outputarea()
-
     def _get_terminal_dimensions(self) -> tuple[int, int]:
         """Gets the terminal dimensions.
 
         Returns:
             tuple[int, int]: terminal width and height
         """
         try:
@@ -232,15 +276,15 @@
         Returns:
             list[Character]: list of EffectCharacter objects
         """
         formatted_lines = []
         if not self.input_data.strip():
             self.input_data = "No Input."
         lines = self.input_data.splitlines()
-        formatted_lines = self._wrap_lines(lines) if not self.args.no_wrap else [line[: self.width] for line in lines]
+        formatted_lines = self._wrap_lines(lines) if self.config.wrap_text else [line[: self.width] for line in lines]
         input_height = len(formatted_lines)
         input_characters = []
         for row, line in enumerate(formatted_lines):
             for column, symbol in enumerate(line):
                 if symbol != " ":
                     character = EffectCharacter(self.next_character_id, symbol, column + 1, input_height - row)
                     character.animation.use_xterm_colors = use_xterm_colors
@@ -274,16 +318,16 @@
             symbol (str): symbol to add
             coord: (Coord): set character's input coordinates
 
         Returns:
             EffectCharacter: the character that was added
         """
         character = EffectCharacter(self.next_character_id, symbol, coord.column, coord.row)
-        character.animation.use_xterm_colors = self.args.xterm_colors
-        character.animation.no_color = self.args.no_color
+        character.animation.use_xterm_colors = self.config.xterm_colors
+        character.animation.no_color = self.config.no_color
         self._added_characters.append(character)
         self.next_character_id += 1
         return character
 
     def _update_terminal_state(self):
         """Update the internal representation of the terminal state with the current position
         of all visible characters.
@@ -293,19 +337,23 @@
             row = character.motion.current_coord.row - 1
             column = character.motion.current_coord.column - 1
             if 0 <= row < self.output_area.top and 0 <= column < self.output_area.right:
                 rows[row][column] = character.symbol
         terminal_state = ["".join(row) for row in rows]
         self.terminal_state = terminal_state
 
-    def _prep_outputarea(self) -> None:
-        """Prepares the terminal for the effect by adding empty lines above."""
+    def prep_outputarea(self) -> None:
+        """Prepares the terminal for the effect by adding empty lines and hiding the cursor."""
         sys.stdout.write(ansitools.HIDE_CURSOR())
         print("\n" * self.output_area.top)
 
+    def restore_cursor(self) -> None:
+        """Restores the cursor visibility."""
+        sys.stdout.write(ansitools.SHOW_CURSOR())
+
     def get_characters(
         self,
         *,
         input_characters: bool = True,
         fill_chars: bool = False,
         added_chars: bool = False,
         sort: CharacterSort = CharacterSort.TOP_TO_BOTTOM_LEFT_TO_RIGHT,
@@ -483,21 +531,44 @@
         """
         character._is_visible = is_visible
         if is_visible:
             self.visible_characters.add(character)
         else:
             self.visible_characters.discard(character)
 
-    def print(self):
-        """Prints the current terminal state to stdout while preserving the cursor position."""
+    def get_formatted_output_string(self) -> str:
+        """Get the formatted output string based on the current terminal state.
+
+        This method updates the internal terminal representation state before returning the formatted output string.
+
+        Returns:
+            str: The formatted output string.
+        """
         self._update_terminal_state()
-        time_since_last_print = time.time() - self.last_time_printed
-        if time_since_last_print < self.animation_rate:
-            time.sleep(self.animation_rate - time_since_last_print)
-        output = "\n".join(self.terminal_state[::-1])
+        output_string = "\n".join(self.terminal_state[::-1])
+        return output_string
+
+    def print(self, output_string: str, *, enforce_frame_rate: bool = True):
+        """Prints the current terminal state to stdout while preserving the cursor position.
+
+        Args:
+            output_string (str): The string to be printed.
+            enforce_frame_rate (bool, optional): Whether to enforce the frame rate set in the terminal config. Defaults to True.
+
+        Notes:
+            This method includes animation timing to control the frame rate.
+            If the time since the last print is less than required to limit the frame rate, the method will sleep for the remaining time
+            to ensure a consistent animation speed.
+
+        """
+        if enforce_frame_rate:
+            frame_delay = 1 / self.frame_rate
+            time_since_last_print = time.time() - self.last_time_printed
+            if time_since_last_print < frame_delay:
+                time.sleep(frame_delay - time_since_last_print)
         sys.stdout.write(ansitools.DEC_SAVE_CURSOR_POSITION())
         sys.stdout.write(ansitools.MOVE_CURSOR_UP(self.output_area.top))
         sys.stdout.write(ansitools.MOVE_CURSOR_TO_COLUMN(1))
-        sys.stdout.write(output)
+        sys.stdout.write(output_string)
         sys.stdout.write(ansitools.DEC_RESTORE_CURSOR_POSITION())
         sys.stdout.flush()
         self.last_time_printed = time.time()
```

### Comparing `terminaltexteffects-0.7.0/PKG-INFO` & `terminaltexteffects-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: terminaltexteffects
-Version: 0.7.0
+Version: 0.8.0
 Summary: A collection of visual effects that can be applied to terminal piped stdin text.
 License: MIT
 Author: Chris
 Author-email: 741258@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 <br/>
 <p align="center">
   <a href="https://github.com/ChrisBuilds/terminaltexteffects">
     <img src="https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/66388e57-e95e-4619-b804-1d8d7ebd124f" alt="TTE" width="80" height="80">
   </a>
@@ -23,81 +24,141 @@
   <p align="center">
     Inline Visual Effects in the Terminal
     <br/>
     <br/>
   </p>
 </p>
 
-[![PyPI - Version](https://img.shields.io/pypi/v/terminaltexteffects?style=flat&color=green)](http://pypi.org/project/terminaltexteffects/ "![PyPI - Version](https://img.shields.io/pypi/v/terminaltexteffects?style=flat&color=green)")  ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/terminaltexteffects) ![License](https://img.shields.io/github/license/ChrisBuilds/terminaltexteffects) 
+[![PyPI - Version](https://img.shields.io/pypi/v/terminaltexteffects?style=flat&color=green)](http://pypi.org/project/terminaltexteffects/ "![PyPI - Version](https://img.shields.io/pypi/v/terminaltexteffects?style=flat&color=green)")  ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/terminaltexteffects) ![License](https://img.shields.io/github/license/ChrisBuilds/terminaltexteffects)
 
 ## Table Of Contents
 
 * [About](#tte)
 * [Requirements](#requirements)
 * [Installation](#installation)
-* [Usage](#usage)
+* [Usage (Application)](#application)
+* [Usage (Library)](#library)
 * [Options](#options)
 * [Examples](#examples)
 * [In-Development Preview](#in-development-preview)
 * [Latest Release Notes](#latest-release-notes)
 * [License](#license)
 
-
 ## TTE
-![synthgrid_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/6d1bab16-0520-44fa-a508-8f92d7d3be9e)
 
+![synthgrid_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/6d1bab16-0520-44fa-a508-8f92d7d3be9e)
 
 TerminalTextEffects is a collection of visual effects that run inline in the terminal. The underlying visual effect engine supports the following:
+
 * Xterm 256 / RGB hex color support
 * Complex character movement via Paths, Waypoints, and
   motion easing.
 * Complex animations via Scenes with symbol/color changes,
   layers, easing, and Path synced progression.
-* Event handling for Path/Scene state changes with 
+* Event handling for Path/Scene state changes with
   custom callback support and many pre-defined actions.
-* Variable stop/step color gradient generation. 
+* Variable stop/step color gradient generation.
 * Extensive effect customization via per-effect arguments.
 * Runs inline, preserving terminal state and workflow.
 
 ## Requirements
 
 TerminalTextEffects is written in Python and does not require any 3rd party modules. Terminal interactions use standard ANSI terminal sequences and should work in most modern terminals.
 
 Note: Windows Terminal performance is slow for some effects.
 
 ## Installation
 
-
 ```pip install terminaltexteffects```
 OR
 ```pipx install terminaltexteffects```
 
 ## Usage
+
+### Application
+
 ```cat your_text | tte <effect> [options]```
 
 OR
 
-``` cat your_text | python -m terminaltexteffects <effect> [options]```
+```cat your_text | python -m terminaltexteffects <effect> [options]```
 
 * Use ```<effect> -h``` to view options for a specific effect, such as color or movement direction.
   * Ex: ```tte decrypt -h```
 
-## Options
+### Library
+
+All effects are iterators which return a string representing the current frame. Basic usage is as simple as importing the effect, instantiating it with the input text, and iterating over the effect.
+
+```python
+from terminaltexteffects.effects import effect_rain
+
+effect = effect_rain.Rain("your text here")
+
+for frame in effect:
+    # do something with the string
+    ...
+```
+
+In the event you want to allow TTE to handle the terminal setup/teardown, cursor positioning, and animation frame rate, a terminal_output() context manager is available.
+
+```python
+from terminaltexteffects.effects import effect_rain
+
+effect = effect_rain.Rain("your text here")
+with effect.terminal_output() as terminal:
+    for frame in effect:
+        terminal.print(frame)
+```
+
+All command line arguments are available within each effect via the `effect.effect_config` and `effect.terminal_config` attributes.
+
+```python
+from terminaltexteffects.effects import effect_rain
+
+effect = effect_rain.Rain("your text here")
+
+effect.effect_config.rain_colors = ("ff0000","00ff00","0000ff")
+effect.terminal_config.tab_width = 2
+effect.terminal_config.wrap_text = False
+
+for frame in effect:
+    # do something with the string
+    ...
+```
+
+For use cases where the terminal dimensions cannot be automatically discovered or you would like to manually define the dimensions, the ```effect.terminal_config``` can be configured as follows:
+
+```python
+effect.terminal_config.terminal_dimensions = (80, 24) # width, height
 ```
+
+If you would like to ignore terminal dimensions altogether and base the output dimensions solely on the input data:
+
+```python
+effect.terminal_config.ignore_terminal_dimensions = True
+```
+
+## Options
+
+```markdown
 options:
-  -h, --help            show this help message and exit
+-h, --help            show this help message and exit
   --tab-width (int > 0)
-                        Number of spaces to use for a tab character.
-  --xterm-colors        Convert any colors specified in RBG hex to the closest XTerm-256 color.
-  --no-color            Disable all colors in the effect.
-  --no-wrap             Disable wrapping of text.
-  -a ANIMATION_RATE, --animation-rate ANIMATION_RATE
-                        Minimum time, in seconds, between animation steps. This value does not normally need to be modified. Use this to increase the playback speed of all aspects of the effect. This will have
-                        no impact beyond a certain lower threshold due to the processing speed of your device.
-
+                        Number of spaces to use for a tab character. (default: 4)
+  --xterm-colors        Convert any colors specified in RBG hex to the closest XTerm-256 color. (default: False)
+  --no-color            Disable all colors in the effect. (default: False)
+  --wrap-text           Wrap text wider than the output area width. (default: False)
+  --frame-rate FRAME_RATE
+                        Target frame rate for the animation. (default: 100)
+  --terminal-dimensions TERMINAL_DIMENSIONS TERMINAL_DIMENSIONS
+                        Use the terminal dimensions to limit the size of the output area and support wrapping. If False, the output area is determined by the input data dimensions and may overflow the terminal
+                        width. (default: (0, 0))
+  --ignore-terminal-dimensions
+                        Ignore the terminal dimensions and use the input data dimensions for the output area. (default: False)
 Effect:
   Name of the effect to apply. Use <effect> -h for effect specific help.
 
   {beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,dev,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,test,unstable,verticalslice,vhstape,waves,wipe}
                         Available Effects
     beams               Create beams which travel over the output area illuminating the characters behind them.
     binarypath          Binary representations of each character move through the terminal towards the home coordinate of the character.
@@ -128,19 +189,22 @@
     verticalslice       Slices the input in half vertically and slides it into place from opposite directions.
     vhstape             Lines of characters glitch left and right and lose detail like an old VHS tape.
     waves               Waves travel across the terminal leaving behind the characters.
     wipe                Wipes the text across the terminal to reveal characters.
 
 Ex: ls -a | tte crumble --final-gradient-stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction diagonal
 ```
-## Examples
-Note: All effects support extensive customization via effect specific arguments. The examples shown below only represent one possible variant of 
+
+### Examples
+
+Note: All effects support extensive customization via effect specific arguments. The examples shown below only represent one possible variant of
 each effect. Check the effect help output to see arguments.
 
 #### Beams
+
 ![beams_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/6bb98dac-688e-43c9-96aa-1a45f451d4cb)
 <details>
 <summary>tte beams -h</summary>
 <br>
     beams | Create beams which travel over the output area illuminating the characters behind them.
 
     options:
@@ -174,14 +238,15 @@
       --final-wipe-speed (int > 0)
                             Speed of the final wipe as measured in diagonal groups activated per frame. (default: 1)
 
     Example: terminaltexteffects beams --beam-row-symbols ▂ ▁ _ --beam-column-symbols ▌ ▍ ▎ ▏ --beam-delay 10 --beam-row-speed-range 10-40 --beam-column-speed-range 6-10 --beam-gradient-stops ffffff 00D1FF 8A008A --beam-gradient-steps 2 8 --beam-gradient-frames 2 --final-gradient-stops 8A008A 00D1FF ffffff --final-gradient-steps 12 --final-gradient-frames 5 --final-gradient-direction vertical --final-wipe-speed 1
 </details>
 
 #### Binarypath
+
 ![binarypath_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/99ad3946-c475-4743-93e2-cdfb2a7f558f)
 <details>
 <summary>tte binarypath -h</summary>
 <br>
     binarypath | Binary representations of each character move through the terminal towards the home coordinate of the character.
 
     options:
@@ -200,14 +265,15 @@
       --active-binary-groups (0 <= float(n) <= 1)
                             Maximum number of binary groups that are active at any given time. Lower this to improve performance. (default: 0.05)
 
     Example: terminaltexteffects binarypath --final-gradient-stops 00d500 007500 --final-gradient-steps 12 --final-gradient-direction vertical --binary-colors 044E29 157e38 45bf55 95ed87 --movement-speed 1.0 --active-binary-groups 0.05
 </details>
 
 #### Blackhole
+
 ![blackhole_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/877579d3-d353-4bed-9a95-d3ea7a53200a)
 <details>
 <summary>tte blackhole -h</summary>
 <br>
     blackhole | Characters are consumed by a black hole and explode outwards.
 
     options:
@@ -225,14 +291,15 @@
       --final-gradient-direction (diagonal, horizontal, vertical, center)
                             Direction of the gradient for the final color. (default: Direction.DIAGONAL)
 
     Example: terminaltexteffects blackhole --star-colors ffcc0d ff7326 ff194d bf2669 702a8c 049dbf --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-direction vertical
 </details>
 
 #### Bouncyballs
+
 ![bouncyballs_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/84b12fd0-6e51-4661-bd09-407dad30023d)
 <details>
 <summary>tte bouncyballs -h</summary>
 <br>
     bouncyballs | Characters are bouncy balls falling from the top of the output area.
 
     options:
@@ -278,14 +345,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects bouncyballs --ball-colors d1f4a5 96e2a4 5acda9 --ball-symbols o "*" O 0 . --final-gradient-stops f8ffae 43c6ac --final-gradient-steps 12 --final-gradient-direction diagonal --ball-delay 7 --movement-speed 0.25 --easing OUT_BOUNCE
 </details>
 
 #### Bubbles
+
 ![bubbles_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/5a616538-7936-4f55-b2ff-28e6c4179fce)
 <details>
 <summary>tte bubbles -h</summary>
 <br>
     bubbles | Characters are formed into bubbles that float down and pop.
 
     options:
@@ -336,14 +404,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects bubbles --bubble-colors d33aff 7395c4 43c2a7 02ff7f --pop-color ffffff --final-gradient-stops d33aff 02ff7f --final-gradient-steps 12 --final-gradient-direction diagonal --bubble-speed 0.1 --bubble-delay 50 --pop-condition row --easing IN_OUT_SINE
 </details>
 
 #### Burn
+
 ![burn_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/9770711a-ea68-48cc-947f-fb13c6613a2e)
 <details>
 <summary>tte burn -h</summary>
 <br>
     burn | Burn the output area.
 
     options:
@@ -360,14 +429,15 @@
       --final-gradient-direction (diagonal, horizontal, vertical, center)
                             Direction of the gradient for the final color. (default: Direction.VERTICAL)
 
     Example: terminaltexteffects burn --starting-color 837373 --burn-colors ffffff fff75d fe650d 8a003c 510100 --final-gradient-stops 00c3ff ffff1c --final-gradient-steps 12
 </details>
 
 #### Crumble
+
 ![crumble_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/f9cdea9b-b695-41b7-b129-8288232cba13)
 <details>
 <summary>tte crumble -h</summary>
 <br>
     crumble | Characters lose color and crumble into dust, vacuumed up, and reformed.
 
     options:
@@ -380,14 +450,15 @@
       --final-gradient-direction (diagonal, horizontal, vertical, center)
                             Direction of the gradient for the final color. (default: Direction.DIAGONAL)
 
     Example: terminaltexteffects crumble --final-gradient-stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction diagonal
 </details>
 
 #### Decrypt
+
 ![decrypt_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/36c23e70-065d-4316-a09e-c2761882cbb3)
 <details>
 <summary>tte decrypt -h</summary>
 <br>
     decrypt | Movie style decryption effect.
 
     options:
@@ -404,14 +475,15 @@
       --final-gradient-direction (diagonal, horizontal, vertical, center)
                             Direction of the gradient for the final color. (default: Direction.VERTICAL)
 
     Example: terminaltexteffects decrypt --typing-speed 2 --ciphertext-colors 008000 00cb00 00ff00 --final-gradient-stops eda000 --final-gradient-steps 12 --final-gradient-direction vertical
 </details>
 
 #### Errorcorrect
+
 ![errorcorrect_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/a851d333-8fe2-4c12-9c45-536ed8ebbab8)
 <details>
 <summary>tte errorcorrect -h</summary>
 <br>
     errorcorrect | Some characters start in the wrong position and are corrected in sequence.
 
     options:
@@ -460,14 +532,15 @@
         Visit: https://easings.net/ for visualizations of the easing functions.
 
         
     Example: terminaltexteffects errorcorrect --error-pairs 0.1 --swap-delay 10 --error-color e74c3c --correct-color 45bf55 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --movement-speed 0.5
 </details>
 
 #### Expand
+
 ![expand_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/21d1c374-9028-4546-a5d7-ee538488ee7b)
 <details>
 <summary>tte expand -h</summary>
 <br>
     expand | Expands the text from a single point.
 
     options:
@@ -511,14 +584,15 @@
         Visit: https://easings.net/ for visualizations of the easing functions.
 
         
     Example: terminaltexteffects expand --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-frames 5 --movement-speed 0.35 --expand-easing IN_OUT_QUART
 </details>
 
 #### Fireworks
+
 ![fireworks_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/da6a97b1-c4fd-4370-9852-9ddb8a494b55)
 <details>
 <summary>tte fireworks -h</summary>
 <br>
     fireworks | Characters explode like fireworks and fall into place.
 
     options:
@@ -542,14 +616,15 @@
       --explode-distance (0 <= float(n) <= 1)
                             Maximum distance from the firework shell origin to the explode waypoint as a percentage of the total output area width. (default: 0.1)
 
     Example: terminaltexteffects fireworks --firework-colors 88F7E2 44D492 F5EB67 FFA15C FA233E --firework-symbol o --firework-volume 0.02 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --launch-delay 60 --explode-distance 0.1 --explode-anywhere
 </details>
 
 #### Middleout
+
 ![middleout_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/d78e37f6-ccb1-4d3b-a07c-f021b6893fce)
 <details>
 <summary>tte middleout -h</summary>
 <br>
     middleout | Text expands in a single row or column in the middle of the output area then out.
 
     options:
@@ -600,14 +675,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects middleout --starting-color 8A008A --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --expand-direction vertical --center-movement-speed 0.35 --full-movement-speed 0.35 --center-easing IN_OUT_SINE --full-easing IN_OUT_SINE
 </details>
 
 #### Orbittingvolley
+
 ![orbittingvolley_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/084038e5-9d49-4c7d-bf15-e989f541b15c)
 <details>
 <summary>tte orbittingvolley -h</summary>
 <br>
     orbittingvolley | Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.
 
     options:
@@ -663,14 +739,15 @@
         Visit: https://easings.net/ for visualizations of the easing functions.
 
         
     Example: terminaltexteffects orbittingvolley --top-launcher-symbol █ --right-launcher-symbol █ --bottom-launcher-symbol █ --left-launcher-symbol █ --final-gradient-stops FFA15C 44D492 --final-gradient-steps 12 --launcher-movement-speed 0.5 --character-movement-speed 1 --volley-size 0.03 --launch-delay 50 --character-easing OUT_SINE
 </details>
 
 #### Overflow
+
 ![overflow_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/37da1088-ba15-4be9-9489-c387a6a55930)
 <details>
 <summary>tte overflow -h</summary>
 <br>
     overflow | Input text overflows ands scrolls the terminal in a random order until eventually appearing ordered.
 
     options:
@@ -689,14 +766,15 @@
       --overflow-speed (int > 0)
                             Speed of the overflow effect. (default: 3)
 
     Example: terminaltexteffects overflow --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --overflow-gradient-stops f2ebc0 8dbfb3 f2ebc0 --overflow-cycles-range 2-4 --overflow-speed 3
 </details>
 
 #### Pour
+
 ![pour_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/145c2a4e-6b30-48c6-80a3-afb03edf7c22)
 <details>
 <summary>tte pour -h</summary>
 <br>
     pour | Pours the characters into position from the given direction.
 
     options:
@@ -745,14 +823,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects pour --pour-direction down --movement-speed 0.2 --gap 1 --starting-color FFFFFF --final-gradient-stops 8A008A 00D1FF FFFFFF --easing IN_QUAD
 </details>
 
 #### Print
+
 ![print_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/5d902350-e5d3-400c-9496-119c88d40643)
 <details>
 <summary>tte print -h</summary>
 <br>
     print | Lines are printed one at a time following a print head. Print head performs line feed, carriage return.
 
     options:
@@ -796,14 +875,15 @@
         Visit: https://easings.net/ for visualizations of the easing functions.
 
         
     Example: terminaltexteffects print --final-gradient-stops 02b8bd c1f0e3 00ffa0 --final-gradient-steps 12 --print-head-return-speed 1.25 --print-speed 1 --print-head-easing IN_OUT_QUAD
 </details>
 
 #### Rain
+
 ![rain_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/7b8cf447-67b6-41e9-b354-07b3e5161d10)
 <details>
 <summary>tte rain -h</summary>
 <br>
     rain | Rain characters from the top of the output area.
 
     options:
@@ -848,14 +928,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
     
     Example: terminaltexteffects rain --rain-symbols o . , "*" "|" --rain-colors 00315C 004C8F 0075DB 3F91D9 78B9F2 9AC8F5 B8D8F8 E3EFFC --final-gradient-stops 488bff b2e7de 57eaf7 --final-gradient-steps 12 --movement-speed 0.1-0.2 --easing IN_QUART
 </details>
 
 #### RandomSequence
+
 ![randomsequence_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/a2218f80-73b6-40ab-b2fb-49268cf9f890)
 <details>
 <summary>tte randomsequence -h</summary>
 <br>
     randomsequence | Prints the input data in a random sequence.
 
     options:
@@ -873,14 +954,15 @@
                             Direction of the gradient for the final color. (default: Direction.VERTICAL)
       --speed (float > 0)   Speed of the animation as a percentage of the total number of characters. (default: 0.004)
 
     Example: terminaltexteffects randomsequence --starting-color 000000 --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --final-gradient-frames 12 --speed 0.004
 </details>
 
 #### Rings
+
 ![rings_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/cb7f6388-0f46-42f1-a2b3-6a267e9451f0)
 <details>
 <summary>tte rings -h</summary>
 <br>
     rings | Characters are dispersed and form into spinning rings.
 
     options:
@@ -904,14 +986,15 @@
       --spin-disperse-cycles SPIN_DISPERSE_CYCLES
                             Number of times the animation will cycles between spinning rings and dispersed characters. (default: 3)
 
     Example: terminaltexteffects rings --ring-colors ab48ff e7b2b2 fffebd --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --ring-gap 0.1 --spin-duration 200 --spin-speed 0.25-1.0 --disperse-duration 200 --spin-disperse-cycles 3
 </details>
 
 #### Scattered
+
 ![scattered_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/9948519d-0158-4ddf-ae3a-7d4eddb706d9)
 <details>
 <summary>tte scattered -h</summary>
 <br>
     scattered | Move the characters into place from random starting locations.
 
     options:
@@ -954,14 +1037,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects scattered --final-gradient-stops ff9048 ab9dff bdffea --final-gradient-steps 12 --final-gradient-frames 12 --movement-speed 0.5 --movement-easing IN_OUT_BACK
 </details>
 
 #### Slide
+
 ![slide_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/218e7218-e9ef-44de-b43b-5e824623a957)
 <details>
 <summary>tte slide -h</summary>
 <br>
     slide | Slide characters into view from outside the terminal, grouped by row, column, or diagonal.
 
     options:
@@ -1009,14 +1093,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects slide --movement-speed 0.5 --grouping row --final-gradient-stops 833ab4 fd1d1d fcb045 --final-gradient-steps 12 --final-gradient-frames 10 --final-gradient-direction vertical --gap 3 --reverse-direction --merge --movement-easing OUT_QUAD
 </details>
 
 #### Spotlights
+
 ![spotlights_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/4ab93725-0c8a-4bdf-af91-057338f4e007)
 <details>
 <summary>tte spotlights -h</summary>
 <br>
     spotlights | Spotlights search the text area, illuminating characters, before converging in the center and expanding.
 
     options:
@@ -1063,14 +1148,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects spotlights --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --beam-width-ratio 2.0 --beam-falloff 0.3 --search-duration 750 --search-speed-range 0.25-0.5 --spotlight-count 3
 </details>
 
 #### Spray
+
 ![spray_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/0be02197-11c3-44d0-9e7f-cd90caefa876)
 <details>
 <summary>tte spray -h</summary>
 <br>
     spray | Draws the characters spawning at varying rates from a single point.
 
     options:
@@ -1115,14 +1201,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
         
     Example: terminaltexteffects spray --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --spray-position e --spray-volume 0.005 --movement-speed 0.4-1.0 --movement-easing OUT_EXPO
 </details>
 
 #### Swarm
+
 ![swarm_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/305e8390-a0fb-4edb-a541-7b52cef77c09)
 <details>
 <summary>tte swarm -h</summary>
 <br>
     swarm | Characters are grouped into swarms and move around the terminal before settling into position.
 
     options:
@@ -1145,14 +1232,15 @@
       --swarm-area-count (hyphen separated int range e.g. '1-10')
                             Range of the number of areas where characters will swarm. (default: (2, 4))
 
     Example: terminaltexteffects swarm --base-color 31a0d4 --flash-color f2ea79 --final-gradient-stops 31b900 f0ff65 --final-gradient-steps 12 --swarm-size 0.1 --swarm-coordination 0.80 --swarm-area-count 2-4
 </details>
 
 #### Synthgrid
+
 ![synthgrid_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/6d1bab16-0520-44fa-a508-8f92d7d3be9e)
 <details>
 <summary>tte synthgrid -h</summary>
 <br>
     synthgrid | Create a grid which fills with characters dissolving into the final text.
 
     options:
@@ -1178,14 +1266,15 @@
       --max-active-blocks (float > 0)
                             Maximum percentage of blocks to have active at any given time. For example, if set to 0.1, 10 percent of the blocks will be active at any given time. (default: 0.1)
 
     Example: terminaltexteffects synthgrid --grid-gradient-stops CC00CC ffffff --grid-gradient-steps 12 --text-gradient-stops 8A008A 00D1FF FFFFFF --text-gradient-steps 12 --grid-row-symbol ─ --grid-column-symbol "│" --text-generation-symbols ░ ▒ ▓ --max-active-blocks 0.1
 </details>
 
 #### Unstable
+
 ![unstable_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/29adb5bf-cd35-4d67-9ed4-fa73ebcb892d)
 <details>
 <summary>tte unstable -h</summary>
 <br>
     synthgrid | Create a grid which fills with characters dissolving into the final text.
 
     options:
@@ -1211,14 +1300,15 @@
       --max-active-blocks (float > 0)
                             Maximum percentage of blocks to have active at any given time. For example, if set to 0.1, 10 percent of the blocks will be active at any given time. (default: 0.1)
 
     Example: terminaltexteffects synthgrid --grid-gradient-stops CC00CC ffffff --grid-gradient-steps 12 --text-gradient-stops 8A008A 00D1FF FFFFFF --text-gradient-steps 12 --grid-row-symbol ─ --grid-column-symbol "│" --text-generation-symbols ░ ▒ ▓ --max-active-blocks 0.1
 </details>
 
 #### Verticalslice
+
 ![verticalslice_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/2341a822-7fef-4ebf-9420-8272fff64082)
 <details>
 <summary>tte verticalslice -h</summary>
 <br>
     verticalslice | Slices the input in half vertically and slides it into place from opposite directions.
 
     options:
@@ -1260,14 +1350,15 @@
         Visit: https://easings.net/ for visualizations of the easing functions.
 
         
     Example: terminaltexteffects verticalslice --final-gradient-stops 8A008A 00D1FF FFFFFF --final-gradient-steps 12 --movement-speed 0.15 --movement-easing IN_OUT_EXPO
 </details>
 
 #### VHSTape
+
 ![vhstape_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/720abbf4-f97d-4ce9-96ee-15ef973488d2)
 <details>
 <summary>tte vhstape -h</summary>
 <br>
     vhstape | Lines of characters glitch left and right and lose detail like an old VHS tape.
 
     options:
@@ -1294,14 +1385,15 @@
       --total-glitch-time (int > 0)
                             Total time, animation steps, that the glitching phase will last. (default: 1000)
 
     Example: terminaltexteffects vhstape --final-gradient-stops ab48ff e7b2b2 fffebd --final-gradient-steps 12 --glitch-line-colors ffffff ff0000 00ff00 0000ff ffffff --glitch-wave-colors ffffff ff0000 00ff00 0000ff ffffff --noise-colors 1e1e1f 3c3b3d 6d6c70 a2a1a6 cbc9cf ffffff --glitch-line-chance 0.05 --noise-chance 0.004 --total-glitch-time 1000
 </details>
 
 #### Waves
+
 ![waves_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/ea9b04ca-e526-4c7e-b98d-a98a42f7137f)
 <details>
 <summary>tte waves -h</summary>
 <br>
     waves | Waves travel across the terminal leaving behind the characters.
 
     options:
@@ -1352,14 +1444,15 @@
         
         Visit: https://easings.net/ for visualizations of the easing functions.
 
     Example: terminaltexteffects waves --wave-symbols ▁ ▂ ▃ ▄ ▅ ▆ ▇ █ ▇ ▆ ▅ ▄ ▃ ▂ ▁ --wave-gradient-stops f0ff65 ffb102 31a0d4 ffb102 f0ff65 --wave-gradient-steps 6 --final-gradient-stops ffb102 31a0d4 f0ff65 --final-gradient-steps 12 --wave-count 7 --wave-length 2 --wave-easing IN_OUT_SINE
 </details>
 
 #### Wipe
+
 ![wipe_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/40b8c81e-6143-4839-af56-12e361651a0a)
 <details>
 <summary>tte wipe -h</summary>
 <br>
     wipe | Wipes the text across the terminal to reveal characters.
 
     options:
@@ -1377,98 +1470,63 @@
       --wipe-delay (int >= 0)
                             Number of animation cycles to wait before adding the next character group. Increase, to slow down the effect. (default: 0)
 
     Example: terminaltexteffects wipe --wipe-direction diagonal_bottom_left_to_top_right --final-gradient-stops 833ab4 fd1d1d fcb045 --final-gradient-steps 12 --final-gradient-frames 5 --wipe-delay 0
 </details>
 
 ## In-Development Preview
-Any effects shown below are in development and will be available in the next release.
 
+Any effects shown below are in development and will be available in the next release.
 
 ## Latest Release Notes
 
-## 0.7.0
+## 0.8.0
+
+---
+
+### New Features (0.8.0)
+
+---
+
+#### New Engine Features (0.8.0)
+
+* Library support: TTE effects are now importable. All effects are iterators that return strings for each frame of the output. See README for more information.
+* Terminal: New terminal argument (--terminal-dimensions) allows specification of the terminal dimensions without relying on auto-detection. Especially useful in cases where TTE is being used as a library in non-terminal or TUI contexts.
+* Terminal: New terminal argument (--ignore-terminal-dimensions) causes the output area dimensions to match the input data dimensions without regard to the terminal.
+
+### Changes (0.8.0)
+
+---
+
+#### Effects Changes (0.8.0)
+
+* Scattered. Holds scrambled text at the start for a few frames.
+* Scattered. Lowered default movement-speed from 0.5 to 0.3.
+
+#### Engine Changes (0.8.0)
+
+* graphics.Gradient ```__iter___()``` refactored to return a generator. No longer improperly implements the iterator protocol by resetting index in ```___iter__()```.
+* Terminal: Argument --animation-rate is now --frame-rate and is specified as a target frames per second.
+* Terminal: Argument --no-wrap is now --wrap-text and defaults to False.
+* Terminal: If a terminal object is instantiated without a TerminalConfig passed, it will instantiate a new TerminalConfig.
+* Terminal: Terminal.get_formatted_output_string() will return a string representing the current frame.
+* Terminal: Terminal.print() will print the frame to the terminal and handle cursor position. The optional argument (enforce_frame_rate: bool = True) determines if the frame rate set at Terminal.config.frame_rate is enforced. If set to False, the print will occur without delay.
+* New argument validator for terminal dimensions (arg_validators.TerminalDeminsions).
+* New module base_effect.py:
+* base_effect.BaseEffect:
+  * This is an abstract class which forms the base iterable for all effects and provides the terminal_output() context manager.
+* base_effect.BaseEffectIterator:
+  * This is an abstract class which provides the functionality to enable iteration over effects.
+
+### Bug Fixes (0.8.0)
+
+---
+
+#### Engine Fixes (0.8.0)
 
-### New Features
-#### Effects
- * Beams. Light beams travel across the output area and illuminate the characters behind them.
- * Overflow. The input text is scrambled by row and repeated randomly, scrolling up the terminal, before eventually displaying in the correct order.
- * OrbitingVolley. Characters fire from launcher which orbit output area.
- * Spotlights. Spotlights search the text area, illuminating characters, before converging in the center and expanding.
-
-#### Engine
- * Gradients now support multiple step specification to control the distance between each stop pair. For example:
-   graphics.Gradient(RED, BLUE, YELLOW, steps=(2,5)) results in a spectrum of RED -> (1 step) -> BLUE -> (4 steps) -> YELLOW
- * graphics.Gradient.get_color_at_fraction(fraction: float) will return a color at the given fraction of the spectrum when provided a float between 0 and 1, inclusive. This can be used to match the color to a ratio/ For example, the character height in the terminal.
- * graphics.Gradient.build_coordinate_color_mapping() will map gradient colors to coordinates in the terminal and supports a Gradient.Direction argument to enable gradients in the following directions: horizontal, vertical, diagonal, center
- * graphics.Gradient, if printed, will show a colored spectrum and the description of its stops and steps.
- * The Scene class has a new method: apply_gradient_to_symbols(). This method will iterate over a list of symbols and apply the colors from a gradient to the symbols. A frame with the symbol will be added for each color starting from the last color used in the previous symbol, up to the the index determined by the ratio of the current symbol's index in the symbols list to the total length of the list. This method allows scenes to automatically create frames from a list of symbols and gradient of arbitrary length while ensuring every symbol and color is displayed.
- * On instatiation, Terminal creates EffectCharacters for every coordinate in the output area that does not have an input character. These EffectCharacters have the symbol " " and are stored in Terminal._fill_characters as well as added to Terminal.character_by_input_coord.
- * arg_validators.IntRange will validate a range specified as "int-int" and return a tuple[int,int].
- * arg_validators.FloatRange will validate a range of floats specified as "float-float" and return a tuple[float, float].
- * character.animation.set_appearance(symbol, color) will set the character symbol and color directly. If a Scene is active, the appearance will be overwritten with the Scene frame on the next call to step_animation(). This method is intended for the occasion where a full scene isn't needed, or the appearance needs to be set based on conditions not compatible with Scenes or the EventHandler. For example, setting the color based on the terminal row. 
- * Terminal.CharacterSort enums moved to Terminal.CharacterGroup, Terminal.CharacterSort is now used for sorting and return a flat list of characters.
- * Terminal.CharacterSort has new sort methods, TOP_TO_BOTTOM_LEFT_TO_RIGHT, TOP_TO_BOTTOM_RIGHT_TO_LEFT, BOTTOM_TO_TOP_LEFT_TO_RIGHT, BOTTOM_TO_TOP_RIGHT_TO_LEFT, OUTSIDE_ROW_TO_MIDDLE, MIDDLE_ROW_TO_OUTSIDE
- * New Terminal.CharacterGroup options, CENTER_TO_OUTSIDE_DIAMONDS and OUTSIDE_TO_CENTER_DIAMONS
- * graphics.Animation.adjust_color_brightness(color: graphics.Color, brightness: float) will convert the color to HSL, adjust the brightness to the given level, and return 
-   an RGB hex string.
- * CTRL-C keyboard interrupt during a running effect will exit gracefully.
- * geometry.find_coords_in_circle() has been rewritten to find all coords which fall in an ellipse. The result is a circle due to the height/width ratio of terminal cells. This function now finds all terminal coordinates within the 'circle' rather than an arbitrary subset.
- * All command line arguments are typed allowing for more easily defined and tested effect args. 
-
-### Changes
-#### Effects
- * All effects have been updated to use the latest API calls for improved performance.
- * All effects support gradients for the final appearance.
- * All effects support gradient direction.
- * All effects have had their default colors refreshed.
- * ErrorCorrect swap-delay lowered and error-pairs specification changed to percent float.
- * Rain effect supports character specification for rain drops and movement speed range for the rain drop falling speed.
- * Print effect uses the row final gradient color for the print head color.
- * RandomSequence effect accepts a starting color and a speed.
- * Rings effect prepares faster. Ring colors are set in order of appearance in the ring-colors argument. Ring spin speed is configurable. Rings with less than 25% visible characters based on radius are no longer generated. Ring gap is set as a percent of the smallest output area dimension.
- * Scattered effect gradient progresses from the first color to the row color.
- * Spray effect spray-volume is specified as a percent of the total number of characters and movement speed is a range.
- * Swarm effect swarm focus points algorithm changed to reduce long distances between points. 
- * Decrypt effect supports gradient specification for plaintext and multiple color specification for ciphertext.
- * Decrypt effect has a --typing-speed arg to increase the speed of the initial text typing effect.
- * Decrypt effect has had the decrypting speed increased.
- * Beams effect uses Animation.adjust_color_brightness() to lower the background character brightness and shows the lighter color when the beam passes by.
- * Crumble effect uses Animation.adjust_color_brightness() to set the weak and dust colors based on the final gradient.
- * Fireworks effect launch_delay argument has a +/- 0-50% randomness applied. 
- * Bubbles effect --no-rainbow changed to --rainbow and default set to False.
- * Bubbles effect --bubble-color changed to --bubble-colors. Bubble color is randomly chosen from the colors unless --rainbow is used.
- * Burn effect burns faster with some randomness in speed.
- * Burn effect final color fades in from the burned color.
- * Burn effect characters are shown prior to burning using a starting_color arg.
- * Pour effect has a --pour-speed argument.
-
-#### Engine
- * Geometry related methods have been removed from the motion class. They are now located at terminaltexteffects.utils.geometry as separate functions.
- * The Coord() object definition has been moved from the motion module to the geometry module.
- * Terminal.add_character() takes a geometry.Coord() argument to set the character's input_coordinate.
- * EffectCharacters have a unique ID set by the Terminal on instatiation. As a result, all EffectCharacters should be created using Terminal.add_character().
- * EffectCharacters added by the effect are stored in Terminal._added_characters.
- * Retrieving EffectCharacters from the terminal should no longer be done via accessing the lists of characters [_added_characters, _fill_characters, _input_characters], but should be retrieved via Terminal.get_characters() and Terminal.get_characters_sorted(). 
- * Setting EffectCharacter visibility is now done via Terminal.set_character_visibility(). This enables the terminal to keep track of all visible characters without needing to iterate over all characters on every call to _update_terminal_state().
- * EventHandler.Action.SET_CHARACTER_VISIBILITY_STATE has been removed as visibilty state is handled by the Terminal. To enable visibility state changes through the event system, use a CALLBACK action with target EventHandler.Callback(terminal.set_character_visibility, True/False).
- * geometry.find_coords_on_circle() num_points arg renamed to points_limit and new arg unique: bool, added to remove any duplicate Coords.
- * The animation rate argument (-a, --animation-rate) has been removed from all effects and is handled as a terminal argument specified prior to the effect name.
- * argtypes.py has been renamed arg_validators.py and all functions have been refactored into classes with a METAVAR class member and a type_parser method.
- * easing.EasingFunction type alias used anywhere an easing function is accepted.
- * Exceptions raised are no longer caught in a except clause. Only a finally clause is used to restore the cursor. Tracebacks are useful.
- 
- #### Other
- * More tests have been added.
-
-### Bug Fixes
-#### Effects
- * All effects with command line options that accept variable length arguments which require at least 1 argument will present an error message when the option is called with 0 arguments.
-
-#### Engine
- * Fixed division by zero error in geometry.find_coord_at_distance() when the origin coord and the target coord are the same.
- * Fixed gradient generating an extra color in the spectrum when the initial color pair was repeated. Ex: Gradient('ffffff','000000','ffffff','000000, steps=5) would result in the third color 'ffffff' being added to the spectrum when it was already present as the end of the generation from '000000'->'ffffff'. 
+* Fixed Argfield nargs type from str to str | int.
+* Implemented custom formatter into argsdataclass.py argument parsing.
 
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/main/LICENSE.md) for more information.
```

#### html2text {}

```diff
@@ -1,54 +1,81 @@
-Metadata-Version: 2.1 Name: terminaltexteffects Version: 0.7.0 Summary: A
+Metadata-Version: 2.1 Name: terminaltexteffects Version: 0.8.0 Summary: A
 collection of visual effects that can be applied to terminal piped stdin text.
 License: MIT Author: Chris Author-email: 741258@pm.me Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-Content-
-Type: text/markdown
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Description-Content-Type: text/markdown
                                      _[_T_T_E_]
                         ******** TTeerrmmiinnaall TTeexxtt EEffffeeccttss ********
                      Inline Visual Effects in the Terminal
 
 [![PyPI - Version](https://img.shields.io/pypi/v/
 terminaltexteffects?style=flat&color=green)](http://pypi.org/project/
 terminaltexteffects/ "![PyPI - Version](https://img.shields.io/pypi/v/
 terminaltexteffects?style=flat&color=green)") ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/terminaltexteffects) ![License](https://
 img.shields.io/github/license/ChrisBuilds/terminaltexteffects) ## Table Of
 Contents * [About](#tte) * [Requirements](#requirements) * [Installation]
-(#installation) * [Usage](#usage) * [Options](#options) * [Examples](#examples)
-* [In-Development Preview](#in-development-preview) * [Latest Release Notes]
-(#latest-release-notes) * [License](#license) ## TTE ![synthgrid_demo](https://
-github.com/ChrisBuilds/terminaltexteffects/assets/57874186/6d1bab16-0520-44fa-
-a508-8f92d7d3be9e) TerminalTextEffects is a collection of visual effects that
-run inline in the terminal. The underlying visual effect engine supports the
+(#installation) * [Usage (Application)](#application) * [Usage (Library)]
+(#library) * [Options](#options) * [Examples](#examples) * [In-Development
+Preview](#in-development-preview) * [Latest Release Notes](#latest-release-
+notes) * [License](#license) ## TTE ![synthgrid_demo](https://github.com/
+ChrisBuilds/terminaltexteffects/assets/57874186/6d1bab16-0520-44fa-a508-
+8f92d7d3be9e) TerminalTextEffects is a collection of visual effects that run
+inline in the terminal. The underlying visual effect engine supports the
 following: * Xterm 256 / RGB hex color support * Complex character movement via
 Paths, Waypoints, and motion easing. * Complex animations via Scenes with
 symbol/color changes, layers, easing, and Path synced progression. * Event
 handling for Path/Scene state changes with custom callback support and many
 pre-defined actions. * Variable stop/step color gradient generation. *
 Extensive effect customization via per-effect arguments. * Runs inline,
 preserving terminal state and workflow. ## Requirements TerminalTextEffects is
 written in Python and does not require any 3rd party modules. Terminal
 interactions use standard ANSI terminal sequences and should work in most
 modern terminals. Note: Windows Terminal performance is slow for some effects.
 ## Installation ```pip install terminaltexteffects``` OR ```pipx install
-terminaltexteffects``` ## Usage ```cat your_text | tte [options]``` OR ``` cat
-your_text | python -m terminaltexteffects [options]``` * Use ``` -h``` to view
-options for a specific effect, such as color or movement direction. * Ex:
-```tte decrypt -h``` ## Options ``` options: -h, --help show this help message
-and exit --tab-width (int > 0) Number of spaces to use for a tab character. --
-xterm-colors Convert any colors specified in RBG hex to the closest XTerm-256
-color. --no-color Disable all colors in the effect. --no-wrap Disable wrapping
-of text. -a ANIMATION_RATE, --animation-rate ANIMATION_RATE Minimum time, in
-seconds, between animation steps. This value does not normally need to be
-modified. Use this to increase the playback speed of all aspects of the effect.
-This will have no impact beyond a certain lower threshold due to the processing
-speed of your device. Effect: Name of the effect to apply. Use -h for effect
+terminaltexteffects``` ## Usage ### Application ```cat your_text | tte
+[options]``` OR ```cat your_text | python -m terminaltexteffects [options]``` *
+Use ``` -h``` to view options for a specific effect, such as color or movement
+direction. * Ex: ```tte decrypt -h``` ### Library All effects are iterators
+which return a string representing the current frame. Basic usage is as simple
+as importing the effect, instantiating it with the input text, and iterating
+over the effect. ```python from terminaltexteffects.effects import effect_rain
+effect = effect_rain.Rain("your text here") for frame in effect: # do something
+with the string ... ``` In the event you want to allow TTE to handle the
+terminal setup/teardown, cursor positioning, and animation frame rate, a
+terminal_output() context manager is available. ```python from
+terminaltexteffects.effects import effect_rain effect = effect_rain.Rain("your
+text here") with effect.terminal_output() as terminal: for frame in effect:
+terminal.print(frame) ``` All command line arguments are available within each
+effect via the `effect.effect_config` and `effect.terminal_config` attributes.
+```python from terminaltexteffects.effects import effect_rain effect =
+effect_rain.Rain("your text here") effect.effect_config.rain_colors =
+("ff0000","00ff00","0000ff") effect.terminal_config.tab_width = 2
+effect.terminal_config.wrap_text = False for frame in effect: # do something
+with the string ... ``` For use cases where the terminal dimensions cannot be
+automatically discovered or you would like to manually define the dimensions,
+the ```effect.terminal_config``` can be configured as follows: ```python
+effect.terminal_config.terminal_dimensions = (80, 24) # width, height ``` If
+you would like to ignore terminal dimensions altogether and base the output
+dimensions solely on the input data: ```python
+effect.terminal_config.ignore_terminal_dimensions = True ``` ## Options
+```markdown options: -h, --help show this help message and exit --tab-width
+(int > 0) Number of spaces to use for a tab character. (default: 4) --xterm-
+colors Convert any colors specified in RBG hex to the closest XTerm-256 color.
+(default: False) --no-color Disable all colors in the effect. (default: False)
+--wrap-text Wrap text wider than the output area width. (default: False) --
+frame-rate FRAME_RATE Target frame rate for the animation. (default: 100) --
+terminal-dimensions TERMINAL_DIMENSIONS TERMINAL_DIMENSIONS Use the terminal
+dimensions to limit the size of the output area and support wrapping. If False,
+the output area is determined by the input data dimensions and may overflow the
+terminal width. (default: (0, 0)) --ignore-terminal-dimensions Ignore the
+terminal dimensions and use the input data dimensions for the output area.
+(default: False) Effect: Name of the effect to apply. Use -h for effect
 specific help.
 {beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,dev,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,test,unstable,verticalslice,vhstape,waves,wipe}
 Available Effects beams Create beams which travel over the output area
 illuminating the characters behind them. binarypath Binary representations of
 each character move through the terminal towards the home coordinate of the
 character. blackhole Characters are consumed by a black hole and explode
 outwards. bouncyballs Characters are bouncy balls falling from the top of the
@@ -77,15 +104,15 @@
 jumbled, explode them to the edge of the output area, then reassemble them in
 the correct layout. verticalslice Slices the input in half vertically and
 slides it into place from opposite directions. vhstape Lines of characters
 glitch left and right and lose detail like an old VHS tape. waves Waves travel
 across the terminal leaving behind the characters. wipe Wipes the text across
 the terminal to reveal characters. Ex: ls -a | tte crumble --final-gradient-
 stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction
-diagonal ``` ## Examples Note: All effects support extensive customization via
+diagonal ``` ### Examples Note: All effects support extensive customization via
 effect specific arguments. The examples shown below only represent one possible
 variant of each effect. Check the effect help output to see arguments. ####
 Beams ![beams_demo](https://github.com/ChrisBuilds/terminaltexteffects/assets/
 57874186/6bb98dac-688e-43c9-96aa-1a45f451d4cb) tte beams -h
 beams | Create beams which travel over the output area illuminating the
 characters behind them. options: -h, --help show this help message and exit --
 beam-row-symbols (ASCII/UTF-8 character) [(ASCII/UTF-8 character) ...] Symbols
@@ -935,130 +962,40 @@
 center) Direction of the gradient for the final color. (default:
 Direction.VERTICAL) --wipe-delay (int >= 0) Number of animation cycles to wait
 before adding the next character group. Increase, to slow down the effect.
 (default: 0) Example: terminaltexteffects wipe --wipe-direction
 diagonal_bottom_left_to_top_right --final-gradient-stops 833ab4 fd1d1d fcb045 -
 -final-gradient-steps 12 --final-gradient-frames 5 --wipe-delay 0 ## In-
 Development Preview Any effects shown below are in development and will be
-available in the next release. ## Latest Release Notes ## 0.7.0 ### New
-Features #### Effects * Beams. Light beams travel across the output area and
-illuminate the characters behind them. * Overflow. The input text is scrambled
-by row and repeated randomly, scrolling up the terminal, before eventually
-displaying in the correct order. * OrbitingVolley. Characters fire from
-launcher which orbit output area. * Spotlights. Spotlights search the text
-area, illuminating characters, before converging in the center and expanding.
-#### Engine * Gradients now support multiple step specification to control the
-distance between each stop pair. For example: graphics.Gradient(RED, BLUE,
-YELLOW, steps=(2,5)) results in a spectrum of RED -> (1 step) -> BLUE -> (4
-steps) -> YELLOW * graphics.Gradient.get_color_at_fraction(fraction: float)
-will return a color at the given fraction of the spectrum when provided a float
-between 0 and 1, inclusive. This can be used to match the color to a ratio/ For
-example, the character height in the terminal. *
-graphics.Gradient.build_coordinate_color_mapping() will map gradient colors to
-coordinates in the terminal and supports a Gradient.Direction argument to
-enable gradients in the following directions: horizontal, vertical, diagonal,
-center * graphics.Gradient, if printed, will show a colored spectrum and the
-description of its stops and steps. * The Scene class has a new method:
-apply_gradient_to_symbols(). This method will iterate over a list of symbols
-and apply the colors from a gradient to the symbols. A frame with the symbol
-will be added for each color starting from the last color used in the previous
-symbol, up to the the index determined by the ratio of the current symbol's
-index in the symbols list to the total length of the list. This method allows
-scenes to automatically create frames from a list of symbols and gradient of
-arbitrary length while ensuring every symbol and color is displayed. * On
-instatiation, Terminal creates EffectCharacters for every coordinate in the
-output area that does not have an input character. These EffectCharacters have
-the symbol " " and are stored in Terminal._fill_characters as well as added to
-Terminal.character_by_input_coord. * arg_validators.IntRange will validate a
-range specified as "int-int" and return a tuple[int,int]. *
-arg_validators.FloatRange will validate a range of floats specified as "float-
-float" and return a tuple[float, float]. * character.animation.set_appearance
-(symbol, color) will set the character symbol and color directly. If a Scene is
-active, the appearance will be overwritten with the Scene frame on the next
-call to step_animation(). This method is intended for the occasion where a full
-scene isn't needed, or the appearance needs to be set based on conditions not
-compatible with Scenes or the EventHandler. For example, setting the color
-based on the terminal row. * Terminal.CharacterSort enums moved to
-Terminal.CharacterGroup, Terminal.CharacterSort is now used for sorting and
-return a flat list of characters. * Terminal.CharacterSort has new sort
-methods, TOP_TO_BOTTOM_LEFT_TO_RIGHT, TOP_TO_BOTTOM_RIGHT_TO_LEFT,
-BOTTOM_TO_TOP_LEFT_TO_RIGHT, BOTTOM_TO_TOP_RIGHT_TO_LEFT,
-OUTSIDE_ROW_TO_MIDDLE, MIDDLE_ROW_TO_OUTSIDE * New Terminal.CharacterGroup
-options, CENTER_TO_OUTSIDE_DIAMONDS and OUTSIDE_TO_CENTER_DIAMONS *
-graphics.Animation.adjust_color_brightness(color: graphics.Color, brightness:
-float) will convert the color to HSL, adjust the brightness to the given level,
-and return an RGB hex string. * CTRL-C keyboard interrupt during a running
-effect will exit gracefully. * geometry.find_coords_in_circle() has been
-rewritten to find all coords which fall in an ellipse. The result is a circle
-due to the height/width ratio of terminal cells. This function now finds all
-terminal coordinates within the 'circle' rather than an arbitrary subset. * All
-command line arguments are typed allowing for more easily defined and tested
-effect args. ### Changes #### Effects * All effects have been updated to use
-the latest API calls for improved performance. * All effects support gradients
-for the final appearance. * All effects support gradient direction. * All
-effects have had their default colors refreshed. * ErrorCorrect swap-delay
-lowered and error-pairs specification changed to percent float. * Rain effect
-supports character specification for rain drops and movement speed range for
-the rain drop falling speed. * Print effect uses the row final gradient color
-for the print head color. * RandomSequence effect accepts a starting color and
-a speed. * Rings effect prepares faster. Ring colors are set in order of
-appearance in the ring-colors argument. Ring spin speed is configurable. Rings
-with less than 25% visible characters based on radius are no longer generated.
-Ring gap is set as a percent of the smallest output area dimension. * Scattered
-effect gradient progresses from the first color to the row color. * Spray
-effect spray-volume is specified as a percent of the total number of characters
-and movement speed is a range. * Swarm effect swarm focus points algorithm
-changed to reduce long distances between points. * Decrypt effect supports
-gradient specification for plaintext and multiple color specification for
-ciphertext. * Decrypt effect has a --typing-speed arg to increase the speed of
-the initial text typing effect. * Decrypt effect has had the decrypting speed
-increased. * Beams effect uses Animation.adjust_color_brightness() to lower the
-background character brightness and shows the lighter color when the beam
-passes by. * Crumble effect uses Animation.adjust_color_brightness() to set the
-weak and dust colors based on the final gradient. * Fireworks effect
-launch_delay argument has a +/- 0-50% randomness applied. * Bubbles effect --
-no-rainbow changed to --rainbow and default set to False. * Bubbles effect --
-bubble-color changed to --bubble-colors. Bubble color is randomly chosen from
-the colors unless --rainbow is used. * Burn effect burns faster with some
-randomness in speed. * Burn effect final color fades in from the burned color.
-* Burn effect characters are shown prior to burning using a starting_color arg.
-* Pour effect has a --pour-speed argument. #### Engine * Geometry related
-methods have been removed from the motion class. They are now located at
-terminaltexteffects.utils.geometry as separate functions. * The Coord() object
-definition has been moved from the motion module to the geometry module. *
-Terminal.add_character() takes a geometry.Coord() argument to set the
-character's input_coordinate. * EffectCharacters have a unique ID set by the
-Terminal on instatiation. As a result, all EffectCharacters should be created
-using Terminal.add_character(). * EffectCharacters added by the effect are
-stored in Terminal._added_characters. * Retrieving EffectCharacters from the
-terminal should no longer be done via accessing the lists of characters
-[_added_characters, _fill_characters, _input_characters], but should be
-retrieved via Terminal.get_characters() and Terminal.get_characters_sorted(). *
-Setting EffectCharacter visibility is now done via
-Terminal.set_character_visibility(). This enables the terminal to keep track of
-all visible characters without needing to iterate over all characters on every
-call to _update_terminal_state(). *
-EventHandler.Action.SET_CHARACTER_VISIBILITY_STATE has been removed as
-visibilty state is handled by the Terminal. To enable visibility state changes
-through the event system, use a CALLBACK action with target
-EventHandler.Callback(terminal.set_character_visibility, True/False). *
-geometry.find_coords_on_circle() num_points arg renamed to points_limit and new
-arg unique: bool, added to remove any duplicate Coords. * The animation rate
-argument (-a, --animation-rate) has been removed from all effects and is
-handled as a terminal argument specified prior to the effect name. *
-argtypes.py has been renamed arg_validators.py and all functions have been
-refactored into classes with a METAVAR class member and a type_parser method. *
-easing.EasingFunction type alias used anywhere an easing function is accepted.
-* Exceptions raised are no longer caught in a except clause. Only a finally
-clause is used to restore the cursor. Tracebacks are useful. #### Other * More
-tests have been added. ### Bug Fixes #### Effects * All effects with command
-line options that accept variable length arguments which require at least 1
-argument will present an error message when the option is called with 0
-arguments. #### Engine * Fixed division by zero error in
-geometry.find_coord_at_distance() when the origin coord and the target coord
-are the same. * Fixed gradient generating an extra color in the spectrum when
-the initial color pair was repeated. Ex: Gradient
-('ffffff','000000','ffffff','000000, steps=5) would result in the third color
-'ffffff' being added to the spectrum when it was already present as the end of
-the generation from '000000'->'ffffff'. ## License Distributed under the MIT
-License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/
-main/LICENSE.md) for more information.
+available in the next release. ## Latest Release Notes ## 0.8.0 --- ### New
+Features (0.8.0) --- #### New Engine Features (0.8.0) * Library support: TTE
+effects are now importable. All effects are iterators that return strings for
+each frame of the output. See README for more information. * Terminal: New
+terminal argument (--terminal-dimensions) allows specification of the terminal
+dimensions without relying on auto-detection. Especially useful in cases where
+TTE is being used as a library in non-terminal or TUI contexts. * Terminal: New
+terminal argument (--ignore-terminal-dimensions) causes the output area
+dimensions to match the input data dimensions without regard to the terminal.
+### Changes (0.8.0) --- #### Effects Changes (0.8.0) * Scattered. Holds
+scrambled text at the start for a few frames. * Scattered. Lowered default
+movement-speed from 0.5 to 0.3. #### Engine Changes (0.8.0) * graphics.Gradient
+```__iter___()``` refactored to return a generator. No longer improperly
+implements the iterator protocol by resetting index in ```___iter__()```. *
+Terminal: Argument --animation-rate is now --frame-rate and is specified as a
+target frames per second. * Terminal: Argument --no-wrap is now --wrap-text and
+defaults to False. * Terminal: If a terminal object is instantiated without a
+TerminalConfig passed, it will instantiate a new TerminalConfig. * Terminal:
+Terminal.get_formatted_output_string() will return a string representing the
+current frame. * Terminal: Terminal.print() will print the frame to the
+terminal and handle cursor position. The optional argument (enforce_frame_rate:
+bool = True) determines if the frame rate set at Terminal.config.frame_rate is
+enforced. If set to False, the print will occur without delay. * New argument
+validator for terminal dimensions (arg_validators.TerminalDeminsions). * New
+module base_effect.py: * base_effect.BaseEffect: * This is an abstract class
+which forms the base iterable for all effects and provides the terminal_output
+() context manager. * base_effect.BaseEffectIterator: * This is an abstract
+class which provides the functionality to enable iteration over effects. ###
+Bug Fixes (0.8.0) --- #### Engine Fixes (0.8.0) * Fixed Argfield nargs type
+from str to str | int. * Implemented custom formatter into argsdataclass.py
+argument parsing. ## License Distributed under the MIT License. See [LICENSE]
+(https://github.com/ChrisBuilds/terminaltexteffects/blob/main/LICENSE.md) for
+more information.
```

