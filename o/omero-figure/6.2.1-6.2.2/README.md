# Comparing `tmp/omero-figure-6.2.1.tar.gz` & `tmp/omero-figure-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-figure-6.2.1.tar", last modified: Fri Apr 19 16:06:38 2024, max compression
+gzip compressed data, was "omero-figure-6.2.2.tar", last modified: Fri Apr 26 12:37:23 2024, max compression
```

## Comparing `omero-figure-6.2.1.tar` & `omero-figure-6.2.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.968554 omero-figure-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-19 16:06:28.000000 omero-figure-6.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 16:06:28.000000 omero-figure-6.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-19 16:06:38.968554 omero-figure-6.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-19 16:06:28.000000 omero-figure-6.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.956554 omero-figure-6.2.1/omero_figure/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.956554 omero-figure-6.2.1/omero_figure/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 16:06:31.000000 omero-figure-6.2.1/omero_figure/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-19 16:06:31.000000 omero-figure-6.2.1/omero_figure/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/omeroutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.952554 omero-figure-6.2.1/omero_figure/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.952554 omero-figure-6.2.1/omero_figure/scripts/omero/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.956554 omero-figure-6.2.1/omero_figure/scripts/omero/figure_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    94614 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.952554 omero-figure-6.2.1/omero_figure/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.956554 omero-figure-6.2.1/omero_figure/static/figure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.956554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (127)    59497 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/backbone-1.0.0.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.956554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/backbone.mousetrap/
--rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2032 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.952554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.960554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/
--rw-r--r--   0 runner    (1001) docker     (127)   119892 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    97339 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.960554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/
--rwxr-xr-x   0 runner    (1001) docker     (127)    14079 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot
--rwxr-xr-x   0 runner    (1001) docker     (127)    63157 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)    29512 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)    16448 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.960554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/
--rw-r--r--   0 runner    (1001) docker     (127)    58458 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    27427 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.952554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.960554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4143 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css
--rwxr-xr-x   0 runner    (1001) docker     (127)     3487 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.952554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.960554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3635 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     3271 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2837 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2972 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     8817 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.960554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/
--rw-r--r--   0 runner    (1001) docker     (127)    40582 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js
--rw-r--r--   0 runner    (1001) docker     (127)    17189 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.960554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-1.11.1/
--rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.960554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.960554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css
--rw-r--r--   0 runner    (1001) docker     (127)   228478 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    17348 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/json2.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.964554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/
--rw-r--r--   0 runner    (1001) docker     (127)    53802 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js
--rw-r--r--   0 runner    (1001) docker     (127)    16798 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.964554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4695 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/ome.csrf.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.964554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    91476 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js
--rw-r--r--   0 runner    (1001) docker     (127)   299677 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.964554 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    74385 2024-04-19 16:06:34.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.964554 omero-figure-6.2.1/omero_figure/static/figure/css/
--rw-r--r--   0 runner    (1001) docker     (127)    23374 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/css/figure.css
--rw-r--r--   0 runner    (1001) docker     (127)   381483 2024-04-19 16:06:37.000000 omero-figure-6.2.1/omero_figure/static/figure/figure.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.968554 omero-figure-6.2.1/omero_figure/static/figure/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/arrow-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/button-down-grey.png
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/button-down.png
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/button-flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/button-up.png
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/crop20.png
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/cursor-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/ellipse-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/gradient.png
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/line-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (127)    18556 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/luts_10.png
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/markdown_dark32x20.png
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/markdown_light32x20.png
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/polygon-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/polyline-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/projection20.png
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/static/figure/images/square-outline-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (127)    68246 2024-04-19 16:06:37.000000 omero-figure-6.2.1/omero_figure/static/figure/templates.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.952554 omero-figure-6.2.1/omero_figure/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.968554 omero-figure-6.2.1/omero_figure/templates/figure/
--rw-r--r--   0 runner    (1001) docker     (127)    63949 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/templates/figure/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24368 2024-04-19 16:06:28.000000 omero-figure-6.2.1/omero_figure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:06:38.956554 omero-figure-6.2.1/omero_figure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-19 16:06:38.000000 omero-figure-6.2.1/omero_figure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-19 16:06:38.000000 omero-figure-6.2.1/omero_figure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:06:38.000000 omero-figure-6.2.1/omero_figure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:06:38.000000 omero-figure-6.2.1/omero_figure.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 16:06:38.000000 omero-figure-6.2.1/omero_figure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 16:06:38.000000 omero-figure-6.2.1/omero_figure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 16:06:38.968554 omero-figure-6.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-19 16:06:28.000000 omero-figure-6.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.488867 omero-figure-6.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-26 12:37:12.000000 omero-figure-6.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-26 12:37:12.000000 omero-figure-6.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-26 12:37:23.488867 omero-figure-6.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-26 12:37:12.000000 omero-figure-6.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.476867 omero-figure-6.2.2/omero_figure/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.476867 omero-figure-6.2.2/omero_figure/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 12:37:15.000000 omero-figure-6.2.2/omero_figure/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 12:37:15.000000 omero-figure-6.2.2/omero_figure/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/omeroutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.472866 omero-figure-6.2.2/omero_figure/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.472866 omero-figure-6.2.2/omero_figure/scripts/omero/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.476867 omero-figure-6.2.2/omero_figure/scripts/omero/figure_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    94637 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.472866 omero-figure-6.2.2/omero_figure/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.480867 omero-figure-6.2.2/omero_figure/static/figure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.480867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)    59497 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/backbone-1.0.0.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.480867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/backbone.mousetrap/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2032 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.472866 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.480867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   119892 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    97339 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.480867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14079 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot
+-rwxr-xr-x   0 runner    (1001) docker     (127)    63157 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29512 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16448 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.480867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    58458 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27427 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.472866 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.484867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4143 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3487 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.472866 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.484867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3635 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3271 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2837 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2972 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8817 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.484867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    40582 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17189 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.484867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-1.11.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.484867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.484867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css
+-rw-r--r--   0 runner    (1001) docker     (127)   228478 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17348 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/json2.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.484867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/
+-rw-r--r--   0 runner    (1001) docker     (127)    53802 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16798 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.484867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4695 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/ome.csrf.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.488867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/raphael-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    91476 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   299677 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.488867 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    74385 2024-04-26 12:37:18.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.488867 omero-figure-6.2.2/omero_figure/static/figure/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    23374 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/css/figure.css
+-rw-r--r--   0 runner    (1001) docker     (127)   381483 2024-04-26 12:37:22.000000 omero-figure-6.2.2/omero_figure/static/figure/figure.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.488867 omero-figure-6.2.2/omero_figure/static/figure/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/arrow-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/button-down-grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/button-down.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/button-flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/button-up.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/crop20.png
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/cursor-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/ellipse-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/gradient.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/line-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18556 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/luts_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/markdown_dark32x20.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/markdown_light32x20.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/polygon-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/polyline-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/projection20.png
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/static/figure/images/square-outline-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68246 2024-04-26 12:37:22.000000 omero-figure-6.2.2/omero_figure/static/figure/templates.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.476867 omero-figure-6.2.2/omero_figure/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.488867 omero-figure-6.2.2/omero_figure/templates/figure/
+-rw-r--r--   0 runner    (1001) docker     (127)    63949 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/templates/figure/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24368 2024-04-26 12:37:12.000000 omero-figure-6.2.2/omero_figure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:37:23.476867 omero-figure-6.2.2/omero_figure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-26 12:37:23.000000 omero-figure-6.2.2/omero_figure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-26 12:37:23.000000 omero-figure-6.2.2/omero_figure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:37:23.000000 omero-figure-6.2.2/omero_figure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:37:23.000000 omero-figure-6.2.2/omero_figure.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 12:37:23.000000 omero-figure-6.2.2/omero_figure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 12:37:23.000000 omero-figure-6.2.2/omero_figure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 12:37:23.492867 omero-figure-6.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-26 12:37:12.000000 omero-figure-6.2.2/setup.py
```

### Comparing `omero-figure-6.2.1/LICENSE` & `omero-figure-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/PKG-INFO` & `omero-figure-6.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: omero-figure
-Version: 6.2.1
+Version: 6.2.2
 Summary: OMERO figure creation app
 Home-page: https://github.com/ome/omero-figure
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-figure/archive/v6.2.1.tar.gz
+Download-URL: https://github.com/ome/omero-figure/archive/v6.2.2.tar.gz
 Keywords: OMERO.web,figure
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omero-figure-6.2.1/README.rst` & `omero-figure-6.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/apps.py` & `omero-figure-6.2.2/omero_figure/apps.py`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/omeroutils.py` & `omero-figure-6.2.2/omero_figure/omeroutils.py`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py` & `omero-figure-6.2.2/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1533,20 +1533,20 @@
         width = region['width']
         height = region['height']
 
         zm_levels = image.getZoomLevelScaling()
         # e.g. {0: 1.0, 1: 0.25, 2: 0.0625, 3: 0.03123, 4: 0.01440}
         # Pick zoom such that returned image is below MAX size
         max_level = len(zm_levels.keys()) - 1
-
-        # Maximum size that the rendering engine will render without OOM
-        max_plane = self.conn.getDownloadAsMaxSizeSetting()
+        # Maximum size that the rendering engine will render
+        max_sizes = self.conn.getMaxPlaneSize()
 
         # start big, and go until we reach target size
         zm = 0
+        max_plane = max_sizes[0] * max_sizes[1]
         while (zm < max_level and
                zm_levels[zm] * width > max_width or
                zm_levels[zm] * width * zm_levels[zm] * height > max_plane):
             zm = zm + 1
 
         level = max_level - zm
```

### Comparing `omero-figure-6.2.1/omero_figure/settings.py` & `omero-figure-6.2.2/omero_figure/settings.py`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/backbone-1.0.0.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/backbone-1.0.0.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/json2.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/json2.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/ome.csrf.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/ome.csrf.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js` & `omero-figure-6.2.2/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/css/figure.css` & `omero-figure-6.2.2/omero_figure/static/figure/css/figure.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/figure.js` & `omero-figure-6.2.2/omero_figure/static/figure/figure.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/arrow-icon-16.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/arrow-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/button-down-grey.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/button-down-grey.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/button-down.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/button-down.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/button-flat.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/button-flat.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/button-up.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/button-up.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/crop20.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/crop20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/ellipse-icon-16.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/ellipse-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/gradient.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/gradient.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/line-icon-16.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/line-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/luts_10.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/luts_10.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/markdown_dark32x20.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/markdown_dark32x20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/markdown_light32x20.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/markdown_light32x20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/polygon-icon-16.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/polygon-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/polyline-icon-16.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/polyline-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/images/projection20.png` & `omero-figure-6.2.2/omero_figure/static/figure/images/projection20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/static/figure/templates.js` & `omero-figure-6.2.2/omero_figure/static/figure/templates.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/templates/figure/index.html` & `omero-figure-6.2.2/omero_figure/templates/figure/index.html`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/urls.py` & `omero-figure-6.2.2/omero_figure/urls.py`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure/utils.py` & `omero-figure-6.2.2/omero_figure/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 
 import json
 import os
 
-__version__ = "6.2.1"
+__version__ = "6.2.2"
 
 
 def read_file(fname, content_type=None):
     p = os.path.abspath(fname)
     with open(p) as f:
         if content_type in ('json',):
             data = json.load(f)
```

### Comparing `omero-figure-6.2.1/omero_figure/views.py` & `omero-figure-6.2.2/omero_figure/views.py`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/omero_figure.egg-info/PKG-INFO` & `omero-figure-6.2.2/omero_figure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: omero-figure
-Version: 6.2.1
+Version: 6.2.2
 Summary: OMERO figure creation app
 Home-page: https://github.com/ome/omero-figure
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-figure/archive/v6.2.1.tar.gz
+Download-URL: https://github.com/ome/omero-figure/archive/v6.2.2.tar.gz
 Keywords: OMERO.web,figure
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omero-figure-6.2.1/omero_figure.egg-info/SOURCES.txt` & `omero-figure-6.2.2/omero_figure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omero-figure-6.2.1/setup.py` & `omero-figure-6.2.2/setup.py`

 * *Files identical despite different names*

