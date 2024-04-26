# Comparing `tmp/PyQtUIkit-2.7.4.tar.gz` & `tmp/PyQtUIkit-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.7.4.tar", last modified: Wed Apr 24 09:33:41 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.8.1.tar", last modified: Fri Apr 26 06:50:03 2024, max compression
```

## Comparing `PyQtUIkit-2.7.4.tar` & `PyQtUIkit-2.8.1.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.634496 PyQtUIkit-2.7.4/
--rw-rw-rw-   0        0        0     1090 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-24 09:33:41.618862 PyQtUIkit-2.7.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.587642 PyQtUIkit-2.7.4/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3896 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/_icons.py
--rw-rw-rw-   0        0        0     3342 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/_translate.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.587642 PyQtUIkit-2.7.4/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.587642 PyQtUIkit-2.7.4/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     5248 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.603240 PyQtUIkit-2.7.4/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.618862 PyQtUIkit-2.7.4/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     3908 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  2340473 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1830 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/locale.py
--rw-rw-rw-   0        0        0     1470 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.618862 PyQtUIkit-2.7.4/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1670 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3304 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     7885 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2794 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    11413 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     8328 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5876 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2542 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/form.py
--rw-rw-rw-   0        0        0     2280 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     1578 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1171 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     5272 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/layout.py
--rw-rw-rw-   0        0        0     1697 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3671 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1758 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     4253 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     4948 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/menu_bar.py
--rw-rw-rw-   0        0        0     7084 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2647 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6683 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     4021 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7515 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    14062 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1295 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     4538 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    17878 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/tree_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.587642 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2576 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 09:33:41.634496 PyQtUIkit-2.7.4/setup.cfg
--rw-rw-rw-   0        0        0     1474 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:50:03.332809 PyQtUIkit-2.8.1/
+-rw-rw-rw-   0        0        0     1090 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-26 06:50:03.332809 PyQtUIkit-2.8.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-26 06:50:03.285938 PyQtUIkit-2.8.1/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3896 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/_icons.py
+-rw-rw-rw-   0        0        0     3271 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/_translate.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:50:03.301561 PyQtUIkit-2.8.1/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:50:03.301561 PyQtUIkit-2.8.1/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     5248 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:50:03.317183 PyQtUIkit-2.8.1/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-26 06:50:03.317183 PyQtUIkit-2.8.1/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     4176 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  2340473 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1830 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/themes/locale.py
+-rw-rw-rw-   0        0        0     1470 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:50:03.332809 PyQtUIkit-2.8.1/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1734 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3304 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     7885 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2794 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    11413 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     8328 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5876 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2542 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/form.py
+-rw-rw-rw-   0        0        0     4350 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/grid_layout.py
+-rw-rw-rw-   0        0        0     2280 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     1578 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1171 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     5344 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/layout.py
+-rw-rw-rw-   0        0        0     1697 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3671 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1758 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     4253 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     4948 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/menu_bar.py
+-rw-rw-rw-   0        0        0     7145 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6805 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     4021 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7515 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    14123 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1297 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/tabs_layout.py
+-rw-rw-rw-   0        0        0     4538 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    17878 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/PyQtUIkit/widgets/tree_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:50:03.301561 PyQtUIkit-2.8.1/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-26 06:50:03.000000 PyQtUIkit-2.8.1/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2024-04-26 06:50:03.000000 PyQtUIkit-2.8.1/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 06:50:03.000000 PyQtUIkit-2.8.1/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-04-26 06:50:03.000000 PyQtUIkit-2.8.1/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-04-26 06:50:03.000000 PyQtUIkit-2.8.1/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-26 06:50:03.000000 PyQtUIkit-2.8.1/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 06:50:03.332809 PyQtUIkit-2.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-04-26 06:49:22.000000 PyQtUIkit-2.8.1/setup.py
```

### Comparing `PyQtUIkit-2.7.4/LICENSE` & `PyQtUIkit-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PKG-INFO` & `PyQtUIkit-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.7.4
+Version: 2.8.1
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/_icons.py` & `PyQtUIkit-2.8.1/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/_translate.py` & `PyQtUIkit-2.8.1/PyQtUIkit/_translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import argparse
 import importlib
 import os
 
 import PyQtUIkit.core._version as version
 from PyQtUIkit.themes.locale import KitLocale
 
-LANGUAGES = dict()
 _translator = None
 
 
 def init_googletrans():
     try:
-        from googletrans import Translator, LANGUAGES as LANGS
+        from translatepy import Translator, Language
 
         global _translator
         _translator = Translator()
-        global LANGUAGES
-        LANGUAGES = LANGS
     except ImportError:
-        print("googletrans is not installed.\nPlease install it with `pip install googletrans==3.1.0a0`")
+        print("translatepy is not installed.\nPlease install it with `pip install translatepy`")
         exit(0)
 
 
 def translate(text, dest):
-    return _translator.translate(text, dest=dest).text
+    return _translator.translate(text, dest).result
 
 
 def get_exists_langs(filename):
     if not filename.endswith('.py'):
         filename += '.py'
     for el in os.listdir(os.path.dirname(filename)):
         if el.endswith('.py') and el != os.path.basename(filename):
@@ -50,15 +47,16 @@
         try:
             dst_locale = import_module(f"{os.path.dirname(filename)}/{lang}.py").locale
         except ImportError:
             pass
         except AttributeError:
             pass
     if dst_locale is None:
-        dst_locale = KitLocale(lang, translate(LANGUAGES[lang].capitalize(), lang), dict())
+        from translatepy import Language
+        dst_locale = KitLocale(lang, translate(Language(lang).name, lang).capitalize(), dict())
 
     print(f"Translating to {lang.capitalize()}...")
     res = ["from PyQtUIkit.themes.locale import KitLocale\n",
            f"locale = KitLocale('{lang}', '{dst_locale.name}', {{"]
     for key, item in src_locale.items():
         try:
             res.append(f"    '{key}': \"{dst_locale.get(key)}\",")
@@ -85,13 +83,13 @@
     init_googletrans()
 
     for lang in args.langs:
         translate_to_lang(args.filename, lang, rewrite=args.rewrite)
 
     if args.update:
         for lang in get_exists_langs(args.filename):
-            if lang not in args.langs and lang in LANGUAGES:
+            if lang not in args.langs:
                 translate_to_lang(args.filename, lang, rewrite=args.rewrite)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.8.1/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.8.1/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.8.1/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/core/font.py` & `PyQtUIkit-2.8.1/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.8.1/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.8.1/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.8.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.8.1/PyQtUIkit/themes/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import importlib
+import os.path
 from importlib.resources import files
 
 from PyQt6.QtCore import QLocale
 from PyQt6.QtGui import QPixmap, QImage, QIcon, QFontDatabase
 
 from PyQtUIkit.themes.builtin_themes import basic_theme, builtin_themes
 from PyQtUIkit.themes.icons import icons
@@ -61,14 +62,21 @@
             icon.resize(*size)
         return QPixmap.fromImage(QImage.fromData(icon.bytes()))
 
     def icon(self, name, color=None, size=None):
         return QIcon(self.pixmap(name, color, size))
 
     @staticmethod
+    def add_icons(path: str, prefix=None):
+        if prefix is None:
+            prefix = os.path.basename(path)
+        for el in os.listdir(path):
+            ThemeManager.add_icon(os.path.join(path, el), f'{prefix}-{el}')
+
+    @staticmethod
     def add_icon(icon: str, name: str):
         """
         Add icon (from .svg file or from data)
         :param icon: path to file or data
         :param name: icon name, str
         :return:
         """
```

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.8.1/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.8.1/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/themes/locale.py` & `PyQtUIkit-2.8.1/PyQtUIkit/themes/locale.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.8.1/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.8.1/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from PyQtUIkit.widgets.spinner import KitSpinner
 from PyQtUIkit.widgets.progress_bar import KitProgressBar
 from PyQtUIkit.widgets.tree_widget import KitTreeWidget, KitTreeWidgetItem
 from PyQtUIkit.widgets.menu import KitMenu
 from PyQtUIkit.widgets.group import KitHGroup, KitVGroup
 from PyQtUIkit.widgets.navigation import KitNavigation
 from PyQtUIkit.widgets.radio import KitVRadio, KitHRadio
-from PyQtUIkit.widgets.tabs import KitTabLayout
+from PyQtUIkit.widgets.tabs_layout import KitTabLayout
 from PyQtUIkit.widgets.text_edit import KitTextEdit, KitTextBrowser
 from PyQtUIkit.widgets.form import KitForm
 from PyQtUIkit.widgets.dialog import KitDialog, KitFormDialog
 from PyQtUIkit.widgets.application import KitApplication, KitAsyncApplication
 from PyQtUIkit.widgets.separator import KitHSeparator, KitVSeparator
 from PyQtUIkit.widgets.menu_bar import KitMenuBar
+from PyQtUIkit.widgets.grid_layout import KitGridLayout
```

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/form.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/form.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/layout.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,17 +46,20 @@
             self.__layout.insertWidget(index, widget, stretch)
         else:
             self.__layout.insertWidget(index, widget)
         self._widgets.insert(index, widget)
         if hasattr(widget, '_set_tm'):
             widget._set_tm(self._tm)
 
-    def deleteWidget(self, w: int | QWidget):
-        if isinstance(w, int):
-            w = self.__layout.takeAt(w).widget()
+    def removeWidget(self, w: int | QWidget):
+        if isinstance(w, QWidget):
+            w = self._widgets.index(w)
+
+        self._widgets.pop(w)
+        w = self.__layout.takeAt(w).widget()
         w.setParent(None)
         return w
 
     def clear(self):
         for _ in range(self.__layout.count()):
             self.__layout.takeAt(0).widget().setParent(None)
         self._widgets.clear()
```

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/menu_bar.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/navigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,16 @@
     def clear(self):
         super().clear()
         self.addWidget(self.__button)
         self.__tabs.clear()
         self.__current = None
 
     def currentIndex(self):
+        if self.__current is None:
+            return None
         return self.__tabs.index(self.__current)
 
     def _apply_theme(self):
         self.setMaximumWidth(self.button_size + self.contentsMargins().left() + self.contentsMargins().right())
         self.__button.main_palette = self._main_palette
         self.__button.size = self.button_size
         for el in self.__tabs:
```

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/radio.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,14 +118,16 @@
 
     def clear(self):
         super().clear()
         self.__items.clear()
         self.__current = None
 
     def currentIndex(self):
+        if self.__current is None:
+            return None
         return self.__items.index(self.__current)
 
     def _apply_theme(self):
         for el in self.__items:
             el.main_palette = self.main_palette
             el.font = self.font
             el.font_size = self.font_size
@@ -179,14 +181,16 @@
 
     def clear(self):
         super().clear()
         self.__items.clear()
         self.__current = None
 
     def currentIndex(self):
+        if self.__current is None:
+            return None
         return self.__items.index(self.__current)
 
     def _apply_theme(self):
         for el in self.__items:
             el.main_palette = self.main_palette
             el.font = self.font
             el.font_size = self.font_size
```

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/tab_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,16 @@
         self.__button_right = KitButton(icon='line-chevron-forward')
         self.__button_right.border = 0
         self.__button_right.setFixedWidth(20)
         self.__button_right.clicked.connect(self._scroll_right)
         self.addWidget(self.__button_right)
 
     def currentIndex(self):
+        if self.__current is None:
+            return None
         return self.__tabs.index(self.__current)
 
     def currentTab(self):
         return self.__current
 
     def tab(self, index):
         return self.__tabs[index]
```

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/tabs_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,9 +27,9 @@
         self._widgets[self.__current].show()
 
     def connect(self, widget: KitTabBar | KitNavigation | KitVRadio | KitHRadio):
         if self.__connected_widget is not None:
             raise Exception("can connect only one widget")
         self.__connected_widget = widget
         widget.currentChanged.connect(self.setCurrent)
-        if widget.currentTab():
+        if widget.currentIndex():
             self.setCurrent(widget.currentIndex())
```

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.8.1/PyQtUIkit/widgets/tree_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.8.1/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.7.4
+Version: 2.8.1
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.7.4/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.8.1/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 PyQtUIkit/widgets/application.py
 PyQtUIkit/widgets/button.py
 PyQtUIkit/widgets/checkbox.py
 PyQtUIkit/widgets/combo_box.py
 PyQtUIkit/widgets/dialog.py
 PyQtUIkit/widgets/flow_layout.py
 PyQtUIkit/widgets/form.py
+PyQtUIkit/widgets/grid_layout.py
 PyQtUIkit/widgets/group.py
 PyQtUIkit/widgets/icon_widget.py
 PyQtUIkit/widgets/label.py
 PyQtUIkit/widgets/layout.py
 PyQtUIkit/widgets/line_edit.py
 PyQtUIkit/widgets/list_widget.py
 PyQtUIkit/widgets/main_window.py
@@ -71,11 +72,11 @@
 PyQtUIkit/widgets/progress_bar.py
 PyQtUIkit/widgets/radio.py
 PyQtUIkit/widgets/scroll_area.py
 PyQtUIkit/widgets/separator.py
 PyQtUIkit/widgets/spin_box.py
 PyQtUIkit/widgets/spinner.py
 PyQtUIkit/widgets/tab_bar.py
-PyQtUIkit/widgets/tabs.py
+PyQtUIkit/widgets/tabs_layout.py
 PyQtUIkit/widgets/text_edit.py
 PyQtUIkit/widgets/toggle.py
 PyQtUIkit/widgets/tree_widget.py
```

### Comparing `PyQtUIkit-2.7.4/setup.py` & `PyQtUIkit-2.8.1/setup.py`

 * *Files identical despite different names*

