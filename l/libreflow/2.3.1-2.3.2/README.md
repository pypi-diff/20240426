# Comparing `tmp/libreflow-2.3.1.tar.gz` & `tmp/libreflow-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow-2.3.1.tar", last modified: Thu Mar 14 17:22:01 2024, max compression
+gzip compressed data, was "libreflow-2.3.2.tar", last modified: Fri Apr 26 08:19:43 2024, max compression
```

## Comparing `libreflow-2.3.1.tar` & `libreflow-2.3.2.tar`

### file list

```diff
@@ -1,346 +1,353 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.844721 libreflow-2.3.1/
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-03-14 17:21:53.000000 libreflow-2.3.1/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    69916 2024-03-14 17:21:53.000000 libreflow-2.3.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1047 2024-03-14 17:21:53.000000 libreflow-2.3.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-14 17:21:53.000000 libreflow-2.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    70953 2024-03-14 17:22:01.844721 libreflow-2.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1640 2024-03-14 17:21:53.000000 libreflow-2.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-03-14 17:22:01.845721 libreflow-2.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2279 2024-03-14 17:21:53.000000 libreflow-2.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.771723 libreflow-2.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.845721 libreflow-2.3.1/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)      911 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-03-14 17:22:01.845721 libreflow-2.3.1/src/libreflow/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.786723 libreflow-2.3.1/src/libreflow/baseflow/
--rw-rw-rw-   0 root         (0) root         (0)    31485 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6008 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     7427 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/departments.py
--rw-rw-rw-   0 root         (0) root         (0)    34140 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/entity_manager.py
--rw-rw-rw-   0 root         (0) root         (0)   201294 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/file.py
--rw-rw-rw-   0 root         (0) root         (0)    28331 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/film.py
--rw-rw-rw-   0 root         (0) root         (0)    34322 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/kitsu.py
--rw-rw-rw-   0 root         (0) root         (0)     4875 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4712 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/maputils.py
--rw-rw-rw-   0 root         (0) root         (0)    18934 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/mytasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/runactions.py
--rw-rw-rw-   0 root         (0) root         (0)    14585 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/runners.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/shot.py
--rw-rw-rw-   0 root         (0) root         (0)    49335 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/site.py
--rw-rw-rw-   0 root         (0) root         (0)    19053 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/task.py
--rw-rw-rw-   0 root         (0) root         (0)    67470 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/task_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.788723 libreflow-2.3.1/src/libreflow/baseflow/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25652 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/controller.py
--rw-rw-rw-   0 root         (0) root         (0)    13555 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/delegate.py
--rw-rw-rw-   0 root         (0) root         (0)    11242 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/file.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/file_cell.py
--rw-rw-rw-   0 root         (0) root         (0)      642 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/file_history.py
--rw-rw-rw-   0 root         (0) root         (0)    12971 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/file_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.789723 libreflow-2.3.1/src/libreflow/baseflow/ui/importfiles/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/importfiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7233 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/importfiles/custom_widget.py
--rw-rw-rw-   0 root         (0) root         (0)    12827 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/importfiles/files_list.py
--rw-rw-rw-   0 root         (0) root         (0)    17843 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/importfiles/target_wizard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.790723 libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17306 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/components.py
--rw-rw-rw-   0 root         (0) root         (0)    14000 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/edit_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     7047 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/file_list.py
--rw-rw-rw-   0 root         (0) root         (0)    49039 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/mytasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/qmodel.py
--rw-rw-rw-   0 root         (0) root         (0)     4086 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/qmodel.py
--rw-rw-rw-   0 root         (0) root         (0)    18102 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/ui/task.py
--rw-rw-rw-   0 root         (0) root         (0)    16888 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/baseflow/users.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.790723 libreflow-2.3.1/src/libreflow/custom_home/
--rw-rw-rw-   0 root         (0) root         (0)     7239 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/custom_home/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4642 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/custom_home/ui.py
--rw-rw-rw-   0 root         (0) root         (0)   211828 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/custom_home/wizard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.791723 libreflow-2.3.1/src/libreflow/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.792723 libreflow-2.3.1/src/libreflow/examples/demoflow/
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/demoflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/demoflow/film.py
--rw-rw-rw-   0 root         (0) root         (0)     2889 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/demoflow/lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.793722 libreflow-2.3.1/src/libreflow/examples/majorque/
--rw-rw-rw-   0 root         (0) root         (0)     2435 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/majorque/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3214 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/majorque/departments.py
--rw-rw-rw-   0 root         (0) root         (0)    10006 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/majorque/file.py
--rw-rw-rw-   0 root         (0) root         (0)     5209 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/majorque/film.py
--rw-rw-rw-   0 root         (0) root         (0)     4005 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/majorque/kitsu.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/majorque/lib.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/majorque/runners.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/examples/majorque/users.py
--rw-rw-rw-   0 root         (0) root         (0)     2557 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/gui.py
--rw-rw-rw-   0 root         (0) root         (0)     5674 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/jobs_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/jobs_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.793722 libreflow-2.3.1/src/libreflow/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.798722 libreflow-2.3.1/src/libreflow/resources/file_templates/
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1897 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.abc
--rw-rw-rw-   0 root         (0) root         (0)     8621 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.aep
--rw-rw-rw-   0 root         (0) root         (0)   323555 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.ai
--rw-rw-rw-   0 root         (0) root         (0)   120981 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.blend
--rw-rw-rw-   0 root         (0) root         (0)    32284 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.fbx
--rw-rw-rw-   0 root         (0) root         (0)    20632 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.jpg
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.json
--rw-rw-rw-   0 root         (0) root         (0)    65344 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.kra
--rw-rw-rw-   0 root         (0) root         (0)    11248 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.mov
--rw-rw-rw-   0 root         (0) root         (0)    63071 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.obj
--rw-rw-rw-   0 root         (0) root         (0)    36592 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.png
--rw-rw-rw-   0 root         (0) root         (0)   417005 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.psb
--rw-rw-rw-   0 root         (0) root         (0)   397099 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.psd
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.txt
--rw-rw-rw-   0 root         (0) root         (0)     1232 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.usd
--rw-rw-rw-   0 root         (0) root         (0)    88244 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/file_templates/template.wav
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.799723 libreflow-2.3.1/src/libreflow/resources/fonts/
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.799723 libreflow-2.3.1/src/libreflow/resources/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.800722 libreflow-2.3.1/src/libreflow/resources/icons/applications/
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/applications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/applications/rv.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.801722 libreflow-2.3.1/src/libreflow/resources/icons/flow/
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6763 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/flow/alembic.png
--rw-rw-rw-   0 root         (0) root         (0)     5862 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/flow/explorer.png
--rw-rw-rw-   0 root         (0) root         (0)     1236 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/flow/photoshop.png
--rw-rw-rw-   0 root         (0) root         (0)    10783 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/flow/quicktime.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.808722 libreflow-2.3.1/src/libreflow/resources/icons/gui/
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/add-file.png
--rw-rw-rw-   0 root         (0) root         (0)     1289 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/add-folder.png
--rw-rw-rw-   0 root         (0) root         (0)     1236 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/arrow-down.png
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)      821 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/check-box-empty-dark.png
--rw-rw-rw-   0 root         (0) root         (0)    10906 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/clean.png
--rw-rw-rw-   0 root         (0) root         (0)     1411 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/close.png
--rw-rw-rw-   0 root         (0) root         (0)     4867 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/compositing.png
--rw-rw-rw-   0 root         (0) root         (0)      868 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/duplicate.png
--rw-rw-rw-   0 root         (0) root         (0)    17838 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/location-worldwide-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)    17853 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/location-worldwide.png
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/maximize.png
--rw-rw-rw-   0 root         (0) root         (0)    18568 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/menu.png
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/menu_dots.png
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/minimize.png
--rw-rw-rw-   0 root         (0) root         (0)     5694 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/misc.png
--rw-rw-rw-   0 root         (0) root         (0)     2029 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/mytasks-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)     1678 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/mytasks.png
--rw-rw-rw-   0 root         (0) root         (0)     1524 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-left-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)      930 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-left.png
--rw-rw-rw-   0 root         (0) root         (0)     2254 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-refresh-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-refresh.png
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-right-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)     1596 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)     1706 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/ref-broken.png
--rw-rw-rw-   0 root         (0) root         (0)     1513 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/ref.png
--rw-rw-rw-   0 root         (0) root         (0)     2360 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/refresh.png
--rw-rw-rw-   0 root         (0) root         (0)     6914 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/send.png
--rw-rw-rw-   0 root         (0) root         (0)    13652 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/gui/send2.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.809722 libreflow-2.3.1/src/libreflow/resources/icons/history/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/history/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/history/check.png
--rw-rw-rw-   0 root         (0) root         (0)      836 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/history/done.png
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/history/init.png
--rw-rw-rw-   0 root         (0) root         (0)      838 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/history/retake.png
--rw-rw-rw-   0 root         (0) root         (0)      831 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/history/wfa.png
--rw-rw-rw-   0 root         (0) root         (0)     1427 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/history/wip.png
--rw-rw-rw-   0 root         (0) root         (0)      944 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/history/working_copy.png
--rw-rw-rw-   0 root         (0) root         (0)     1499 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/history/working_copy_mine.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.825722 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)     1755 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/3d-object.png
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/active_site.png
--rw-rw-rw-   0 root         (0) root         (0)     1617 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/afterfx.png
--rw-rw-rw-   0 root         (0) root         (0)     6101 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/archive.png
--rw-rw-rw-   0 root         (0) root         (0)     1386 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/available.png
--rw-rw-rw-   0 root         (0) root         (0)     6331 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/blank.png
--rw-rw-rw-   0 root         (0) root         (0)     1438 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/blender.png
--rw-rw-rw-   0 root         (0) root         (0)     1556 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/checked-symbol-colored.png
--rw-rw-rw-   0 root         (0) root         (0)     1566 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/checked-symbol.png
--rw-rw-rw-   0 root         (0) root         (0)     1711 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/circle-shape-outline.png
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/circle-shape-right-eye-outline.png
--rw-rw-rw-   0 root         (0) root         (0)     1730 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/circular-shape-right-eye-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/circular-shape-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/clean.png
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/clipboard.png
--rw-rw-rw-   0 root         (0) root         (0)     2108 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/compare-previews.png
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/cross-mark-on-a-black-circle-background-colored.png
--rw-rw-rw-   0 root         (0) root         (0)     3131 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/custom_home_star.png
--rw-rw-rw-   0 root         (0) root         (0)     1229 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/delete.png
--rw-rw-rw-   0 root         (0) root         (0)     1726 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/dependencies.png
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/download.png
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/downloadable.png
--rw-rw-rw-   0 root         (0) root         (0)     1424 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/duplicate.png
--rw-rw-rw-   0 root         (0) root         (0)    15134 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/edit-blank.png
--rw-rw-rw-   0 root         (0) root         (0)     2428 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/edit-lock-green.png
--rw-rw-rw-   0 root         (0) root         (0)     2610 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/edit-lock-red.png
--rw-rw-rw-   0 root         (0) root         (0)      939 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/error.png
--rw-rw-rw-   0 root         (0) root         (0)     2052 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/exchange.png
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/exclamation-sign-colored.png
--rw-rw-rw-   0 root         (0) root         (0)     2027 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/fbx.png
--rw-rw-rw-   0 root         (0) root         (0)     6192 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/firefox.png
--rw-rw-rw-   0 root         (0) root         (0)     1475 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/hide.png
--rw-rw-rw-   0 root         (0) root         (0)     6372 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/history.png
--rw-rw-rw-   0 root         (0) root         (0)     1419 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/illustrator.png
--rw-rw-rw-   0 root         (0) root         (0)     2104 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/json.png
--rw-rw-rw-   0 root         (0) root         (0)     1498 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/jsx.png
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu.svg
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_done.png
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_oklodv.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_omit.png
--rw-rw-rw-   0 root         (0) root         (0)     1124 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_retake.png
--rw-rw-rw-   0 root         (0) root         (0)     1040 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_todo.png
--rw-rw-rw-   0 root         (0) root         (0)     1126 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_wfa.png
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_wip.png
--rw-rw-rw-   0 root         (0) root         (0)     2866 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/krita.png
--rw-rw-rw-   0 root         (0) root         (0)     1167 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/lock-green.png
--rw-rw-rw-   0 root         (0) root         (0)     1171 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/lock-red.png
--rw-rw-rw-   0 root         (0) root         (0)     1483 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/log_out.png
--rw-rw-rw-   0 root         (0) root         (0)    37128 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/multi-share-option.png
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/nuke.png
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/origin-site.png
--rw-rw-rw-   0 root         (0) root         (0)     1475 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/padlock.png
--rw-rw-rw-   0 root         (0) root         (0)     1575 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/padlock_green.png
--rw-rw-rw-   0 root         (0) root         (0)     1482 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/padlock_red.png
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/publish-ae.png
--rw-rw-rw-   0 root         (0) root         (0)     1082 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/publish-blender.png
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/publish.png
--rw-rw-rw-   0 root         (0) root         (0)     1918 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/quicktime.png
--rw-rw-rw-   0 root         (0) root         (0)     1699 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/refresh.png
--rw-rw-rw-   0 root         (0) root         (0)     1785 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/request.png
--rw-rw-rw-   0 root         (0) root         (0)     1338 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/requestable.png
--rw-rw-rw-   0 root         (0) root         (0)     1160 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/run.png
--rw-rw-rw-   0 root         (0) root         (0)     1510 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/show.png
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/stop.png
--rw-rw-rw-   0 root         (0) root         (0)     1861 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/sync.png
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/sync_arrow.png
--rw-rw-rw-   0 root         (0) root         (0)     2143 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/time_format.png
--rw-rw-rw-   0 root         (0) root         (0)     1606 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/unavailable.png
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/upload.png
--rw-rw-rw-   0 root         (0) root         (0)     2197 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/vscodium.png
--rw-rw-rw-   0 root         (0) root         (0)    73670 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/waiting.png
--rw-rw-rw-   0 root         (0) root         (0)     1279 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/warning.png
--rw-rw-rw-   0 root         (0) root         (0)     1586 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/libreflow/watch.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.828722 libreflow-2.3.1/src/libreflow/resources/icons/status/
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/done.png
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/err.png
--rw-rw-rw-   0 root         (0) root         (0)     3014 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/inv.png
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/none.png
--rw-rw-rw-   0 root         (0) root         (0)     2999 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/nys.png
--rw-rw-rw-   0 root         (0) root         (0)     3130 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/oop.png
--rw-rw-rw-   0 root         (0) root         (0)     3112 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/rtk.png
--rw-rw-rw-   0 root         (0) root         (0)     3113 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/rvw.png
--rw-rw-rw-   0 root         (0) root         (0)     3212 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/wait.png
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/warn.png
--rw-rw-rw-   0 root         (0) root         (0)     3218 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/status/wip.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.830722 libreflow-2.3.1/src/libreflow/resources/icons/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/animation.svg
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/clean.svg
--rw-rw-rw-   0 root         (0) root         (0)     1350 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/colo.svg
--rw-rw-rw-   0 root         (0) root         (0)     1762 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/compositing.svg
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/design.svg
--rw-rw-rw-   0 root         (0) root         (0)     1440 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/layout.svg
--rw-rw-rw-   0 root         (0) root         (0)      903 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/lighting.svg
--rw-rw-rw-   0 root         (0) root         (0)     1421 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/modeling.svg
--rw-rw-rw-   0 root         (0) root         (0)     1267 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/rigging.svg
--rw-rw-rw-   0 root         (0) root         (0)      786 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/icons/tasks/shading.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.831722 libreflow-2.3.1/src/libreflow/resources/mark_sequence/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/mark_sequence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.831722 libreflow-2.3.1/src/libreflow/resources/mark_sequence/fields/
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/mark_sequence/fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1920 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/mark_sequence/fields/default.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.831722 libreflow-2.3.1/src/libreflow/resources/mark_sequence/fonts/
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/mark_sequence/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.831722 libreflow-2.3.1/src/libreflow/resources/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.832722 libreflow-2.3.1/src/libreflow/resources/scripts/blender/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/scripts/blender/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6076 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/scripts/blender/disable_save_keymap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.832722 libreflow-2.3.1/src/libreflow/resources/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.832722 libreflow-2.3.1/src/libreflow/resources/styles/lfs_tech/
--rw-rw-rw-   0 root         (0) root         (0)     3280 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/styles/lfs_tech/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10492 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/resources/styles/lfs_tech/lfs_tech_style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.833722 libreflow-2.3.1/src/libreflow/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16095 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/scripts/mark_sequence.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/scripts/minio_file_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/scripts/minio_file_uploader.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/scripts/session_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1251 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/session.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/sync.py
--rw-rw-rw-   0 root         (0) root         (0)     2750 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/sync_jobs_cleaner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.834722 libreflow-2.3.1/src/libreflow/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/b3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.836722 libreflow-2.3.1/src/libreflow/utils/flow/
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14474 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/flow/action_values.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/flow/context_values.py
--rw-rw-rw-   0 root         (0) root         (0)     5358 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/flow/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/flow/file_processing.py
--rw-rw-rw-   0 root         (0) root         (0)    16613 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/flow/import_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5412 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/flow/process_files.py
--rw-rw-rw-   0 root         (0) root         (0)     2356 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/flow/values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.836722 libreflow-2.3.1/src/libreflow/utils/kabaret/
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.836722 libreflow-2.3.1/src/libreflow/utils/kabaret/flow_entities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/flow_entities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9034 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/flow_entities/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.838722 libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/
--rw-rw-rw-   0 root         (0) root         (0)        2 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2747 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/demo_flow.py
--rw-rw-rw-   0 root         (0) root         (0)    27913 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/jobs_actor.py
--rw-rw-rw-   0 root         (0) root         (0)     6738 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/jobs_flow.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/jobs_flow_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4660 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/jobs_node.py
--rw-rw-rw-   0 root         (0) root         (0)    11242 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/jobs_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.838722 libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.838722 libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/actor/
--rw-rw-rw-   0 root         (0) root         (0)     4584 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/actor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.839722 libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/flow/
--rw-rw-rw-   0 root         (0) root         (0)     1016 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5670 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/runner_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.839722 libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/views/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18305 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/views/subprocess_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.840721 libreflow-2.3.1/src/libreflow/utils/kabaret/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8365 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/ui/flow_view.py
--rw-rw-rw-   0 root         (0) root         (0)     6285 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/ui/main_window.py
--rw-rw-rw-   0 root         (0) root         (0)    20792 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/ui/navigation_control.py
--rw-rw-rw-   0 root         (0) root         (0)     1861 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/kabaret/ui/widget_view.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/os.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.841722 libreflow-2.3.1/src/libreflow/utils/search/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/actor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.841722 libreflow-2.3.1/src/libreflow/utils/search/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.843721 libreflow-2.3.1/src/libreflow/utils/search/data/icons/
--rw-rw-rw-   0 root         (0) root         (0)      133 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      885 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/icons/export.png
--rw-rw-rw-   0 root         (0) root         (0)     1000 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/icons/filter-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/icons/filter-enabled.png
--rw-rw-rw-   0 root         (0) root         (0)      901 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/icons/import.png
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/icons/magn-glass.png
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/icons/minus-button.png
--rw-rw-rw-   0 root         (0) root         (0)      735 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/icons/plus-button.png
--rw-rw-rw-   0 root         (0) root         (0)     1229 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/icons/remove.png
--rw-rw-rw-   0 root         (0) root         (0)      938 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/data/icons/run-button.png
--rw-rw-rw-   0 root         (0) root         (0)    16126 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/search/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.843721 libreflow-2.3.1/src/libreflow/utils/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20399 2024-03-14 17:21:53.000000 libreflow-2.3.1/src/libreflow/utils/ui/file_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:22:01.844721 libreflow-2.3.1/src/libreflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)    70953 2024-03-14 17:22:01.000000 libreflow-2.3.1/src/libreflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14091 2024-03-14 17:22:01.000000 libreflow-2.3.1/src/libreflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 17:22:01.000000 libreflow-2.3.1/src/libreflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      212 2024-03-14 17:22:01.000000 libreflow-2.3.1/src/libreflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-14 17:22:01.000000 libreflow-2.3.1/src/libreflow.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    70144 2024-03-14 17:21:53.000000 libreflow-2.3.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.873053 libreflow-2.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-04-26 08:19:34.000000 libreflow-2.3.2/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    71705 2024-04-26 08:19:34.000000 libreflow-2.3.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2024-04-26 08:19:34.000000 libreflow-2.3.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-26 08:19:34.000000 libreflow-2.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    72742 2024-04-26 08:19:43.873053 libreflow-2.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2024-04-26 08:19:34.000000 libreflow-2.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-26 08:19:43.873053 libreflow-2.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2405 2024-04-26 08:19:34.000000 libreflow-2.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.786050 libreflow-2.3.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.874053 libreflow-2.3.2/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)      911 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-26 08:19:43.874053 libreflow-2.3.2/src/libreflow/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.805050 libreflow-2.3.2/src/libreflow/baseflow/
+-rw-rw-rw-   0 root         (0) root         (0)    31578 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6008 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     7427 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/departments.py
+-rw-rw-rw-   0 root         (0) root         (0)    34140 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/entity_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)   201280 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/file.py
+-rw-rw-rw-   0 root         (0) root         (0)    28331 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)    35159 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/kitsu.py
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4712 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/maputils.py
+-rw-rw-rw-   0 root         (0) root         (0)    18934 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/mytasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/runactions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14917 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/runners.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/shot.py
+-rw-rw-rw-   0 root         (0) root         (0)    49390 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/site.py
+-rw-rw-rw-   0 root         (0) root         (0)    19053 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/task.py
+-rw-rw-rw-   0 root         (0) root         (0)    72943 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/task_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.807051 libreflow-2.3.2/src/libreflow/baseflow/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25652 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    13555 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/delegate.py
+-rw-rw-rw-   0 root         (0) root         (0)    11242 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/file.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/file_cell.py
+-rw-rw-rw-   0 root         (0) root         (0)      642 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/file_history.py
+-rw-rw-rw-   0 root         (0) root         (0)    12971 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/file_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.808051 libreflow-2.3.2/src/libreflow/baseflow/ui/importfiles/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/importfiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7233 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/importfiles/custom_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)    12827 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/importfiles/files_list.py
+-rw-rw-rw-   0 root         (0) root         (0)    17843 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/importfiles/target_wizard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.809051 libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17306 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/components.py
+-rw-rw-rw-   0 root         (0) root         (0)    14000 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/edit_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     7051 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/file_list.py
+-rw-rw-rw-   0 root         (0) root         (0)    49203 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/mytasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/qmodel.py
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/qmodel.py
+-rw-rw-rw-   0 root         (0) root         (0)    18098 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/ui/task.py
+-rw-rw-rw-   0 root         (0) root         (0)    16888 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/baseflow/users.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.810051 libreflow-2.3.2/src/libreflow/custom_home/
+-rw-rw-rw-   0 root         (0) root         (0)     7239 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/custom_home/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4642 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/custom_home/ui.py
+-rw-rw-rw-   0 root         (0) root         (0)   211828 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/custom_home/wizard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.810051 libreflow-2.3.2/src/libreflow/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.811051 libreflow-2.3.2/src/libreflow/examples/demoflow/
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/demoflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/demoflow/film.py
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/demoflow/lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.813051 libreflow-2.3.2/src/libreflow/examples/majorque/
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/majorque/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/majorque/departments.py
+-rw-rw-rw-   0 root         (0) root         (0)    10006 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/majorque/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5209 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/majorque/film.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/majorque/kitsu.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/majorque/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/majorque/runners.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/examples/majorque/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2557 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     5674 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/jobs_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/jobs_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.813051 libreflow-2.3.2/src/libreflow/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.820051 libreflow-2.3.2/src/libreflow/resources/file_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.abc
+-rw-rw-rw-   0 root         (0) root         (0)     8621 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.aep
+-rw-rw-rw-   0 root         (0) root         (0)   323555 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.ai
+-rw-rw-rw-   0 root         (0) root         (0)   120981 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.blend
+-rw-rw-rw-   0 root         (0) root         (0)    32284 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.fbx
+-rw-rw-rw-   0 root         (0) root         (0)    20632 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.jpg
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.jsx
+-rw-rw-rw-   0 root         (0) root         (0)    65344 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.kra
+-rw-rw-rw-   0 root         (0) root         (0)    11248 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.mov
+-rw-rw-rw-   0 root         (0) root         (0)  1263464 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.mp4
+-rw-rw-rw-   0 root         (0) root         (0)     1651 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.nk
+-rw-rw-rw-   0 root         (0) root         (0)    63071 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.obj
+-rw-rw-rw-   0 root         (0) root         (0)    36592 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.png
+-rw-rw-rw-   0 root         (0) root         (0)   417005 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.psb
+-rw-rw-rw-   0 root         (0) root         (0)   397099 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.psd
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1232 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.usd
+-rw-rw-rw-   0 root         (0) root         (0)    88244 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/file_templates/template.wav
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.821051 libreflow-2.3.2/src/libreflow/resources/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    86400 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/fonts/SpaceGrotesk-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    86504 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/fonts/SpaceGrotesk-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.821051 libreflow-2.3.2/src/libreflow/resources/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.821051 libreflow-2.3.2/src/libreflow/resources/icons/applications/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/applications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/applications/rv.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.823051 libreflow-2.3.2/src/libreflow/resources/icons/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6763 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/flow/alembic.png
+-rw-rw-rw-   0 root         (0) root         (0)     5862 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/flow/explorer.png
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/flow/photoshop.png
+-rw-rw-rw-   0 root         (0) root         (0)    10783 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/flow/quicktime.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.830052 libreflow-2.3.2/src/libreflow/resources/icons/gui/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/add-file.png
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/add-folder.png
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/arrow-down.png
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/arrow-right.png
+-rw-rw-rw-   0 root         (0) root         (0)      821 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/check-box-empty-dark.png
+-rw-rw-rw-   0 root         (0) root         (0)    10906 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/clean.png
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/close.png
+-rw-rw-rw-   0 root         (0) root         (0)     4867 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/compositing.png
+-rw-rw-rw-   0 root         (0) root         (0)      868 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/duplicate.png
+-rw-rw-rw-   0 root         (0) root         (0)    17838 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/location-worldwide-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)    17853 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/location-worldwide.png
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/maximize.png
+-rw-rw-rw-   0 root         (0) root         (0)    18568 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/menu.png
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/menu_dots.png
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/minimize.png
+-rw-rw-rw-   0 root         (0) root         (0)     5694 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/misc.png
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/mytasks-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/mytasks.png
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-left-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)      930 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-left.png
+-rw-rw-rw-   0 root         (0) root         (0)     2254 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-refresh-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-refresh.png
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-right-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-right.png
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/ref-broken.png
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/ref.png
+-rw-rw-rw-   0 root         (0) root         (0)     2360 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/refresh.png
+-rw-rw-rw-   0 root         (0) root         (0)     6914 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/send.png
+-rw-rw-rw-   0 root         (0) root         (0)    13652 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/gui/send2.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.832052 libreflow-2.3.2/src/libreflow/resources/icons/history/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/history/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/history/check.png
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/history/done.png
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/history/init.png
+-rw-rw-rw-   0 root         (0) root         (0)      838 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/history/retake.png
+-rw-rw-rw-   0 root         (0) root         (0)      831 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/history/wfa.png
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/history/wip.png
+-rw-rw-rw-   0 root         (0) root         (0)      944 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/history/working_copy.png
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/history/working_copy_mine.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.849052 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/3d-object.png
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/active_site.png
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/afterfx.png
+-rw-rw-rw-   0 root         (0) root         (0)     6101 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/archive.png
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/available.png
+-rw-rw-rw-   0 root         (0) root         (0)     6331 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/blank.png
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/blender.png
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/checked-symbol-colored.png
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/checked-symbol.png
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/circle-shape-outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/circle-shape-right-eye-outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     1730 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/circular-shape-right-eye-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/circular-shape-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/clean.png
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/clipboard.png
+-rw-rw-rw-   0 root         (0) root         (0)     2108 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/compare-previews.png
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/cross-mark-on-a-black-circle-background-colored.png
+-rw-rw-rw-   0 root         (0) root         (0)     3131 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/custom_home_star.png
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/delete.png
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/dependencies.png
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/download.png
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/downloadable.png
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/duplicate.png
+-rw-rw-rw-   0 root         (0) root         (0)    15134 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/edit-blank.png
+-rw-rw-rw-   0 root         (0) root         (0)     2428 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/edit-lock-green.png
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/edit-lock-red.png
+-rw-rw-rw-   0 root         (0) root         (0)      939 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/error.png
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/exchange.png
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/exclamation-sign-colored.png
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/fbx.png
+-rw-rw-rw-   0 root         (0) root         (0)     6192 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/firefox.png
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/hide.png
+-rw-rw-rw-   0 root         (0) root         (0)     6372 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/history.png
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/illustrator.png
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/json.png
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/jsx.png
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_done.png
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_oklodv.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_omit.png
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_retake.png
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_todo.png
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_wfa.png
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_wip.png
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/krita.png
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/lock-green.png
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/lock-red.png
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/log_out.png
+-rw-rw-rw-   0 root         (0) root         (0)    37128 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/multi-share-option.png
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/nuke.png
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/origin-site.png
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/padlock.png
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/padlock_green.png
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/padlock_red.png
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/premiere-pro.png
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/publish-ae.png
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/publish-blender.png
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/publish.png
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/quicktime.png
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/refresh.png
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/request.png
+-rw-rw-rw-   0 root         (0) root         (0)     1338 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/requestable.png
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/run.png
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/show.png
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/stop.png
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/sync.png
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/sync_arrow.png
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/time_format.png
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/unavailable.png
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/upload.png
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/vscodium.png
+-rw-rw-rw-   0 root         (0) root         (0)    73670 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/waiting.png
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/warning.png
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/libreflow/watch.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.852052 libreflow-2.3.2/src/libreflow/resources/icons/status/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/done.png
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/err.png
+-rw-rw-rw-   0 root         (0) root         (0)     3014 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/inv.png
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/none.png
+-rw-rw-rw-   0 root         (0) root         (0)     2999 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/nys.png
+-rw-rw-rw-   0 root         (0) root         (0)     3130 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/oop.png
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/rtk.png
+-rw-rw-rw-   0 root         (0) root         (0)     3113 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/rvw.png
+-rw-rw-rw-   0 root         (0) root         (0)     3212 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/wait.png
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/warn.png
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/status/wip.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.854052 libreflow-2.3.2/src/libreflow/resources/icons/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/animation.svg
+-rw-rw-rw-   0 root         (0) root         (0)      738 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/clean.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/colo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/compositing.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/design.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/layout.svg
+-rw-rw-rw-   0 root         (0) root         (0)      903 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/lighting.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/modeling.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/rigging.svg
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/icons/tasks/shading.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.854052 libreflow-2.3.2/src/libreflow/resources/mark_sequence/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/mark_sequence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.855052 libreflow-2.3.2/src/libreflow/resources/mark_sequence/fields/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/mark_sequence/fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1920 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/mark_sequence/fields/default.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.856052 libreflow-2.3.2/src/libreflow/resources/mark_sequence/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   313408 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/mark_sequence/fonts/LiberationMono-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/mark_sequence/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.856052 libreflow-2.3.2/src/libreflow/resources/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.857052 libreflow-2.3.2/src/libreflow/resources/scripts/blender/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/scripts/blender/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6076 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/scripts/blender/disable_save_keymap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.857052 libreflow-2.3.2/src/libreflow/resources/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.857052 libreflow-2.3.2/src/libreflow/resources/styles/lfs_tech/
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/styles/lfs_tech/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10492 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/resources/styles/lfs_tech/lfs_tech_style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.859053 libreflow-2.3.2/src/libreflow/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16095 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/scripts/mark_sequence.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/scripts/minio_file_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/scripts/minio_file_uploader.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/scripts/session_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/sync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/sync_jobs_cleaner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.860053 libreflow-2.3.2/src/libreflow/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/b3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.862053 libreflow-2.3.2/src/libreflow/utils/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14474 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/flow/action_values.py
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/flow/context_values.py
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/flow/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/flow/file_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)    16613 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/flow/import_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5412 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/flow/process_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/flow/values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.862053 libreflow-2.3.2/src/libreflow/utils/kabaret/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.863053 libreflow-2.3.2/src/libreflow/utils/kabaret/flow_entities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/flow_entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9034 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/flow_entities/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.864053 libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2747 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/demo_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)    27913 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/jobs_actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6738 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/jobs_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/jobs_flow_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4660 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/jobs_node.py
+-rw-rw-rw-   0 root         (0) root         (0)    11242 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/jobs_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.865053 libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.865053 libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/actor/
+-rw-rw-rw-   0 root         (0) root         (0)     4584 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/actor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.866053 libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5670 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/runner_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.866053 libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/views/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18305 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/views/subprocess_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.868053 libreflow-2.3.2/src/libreflow/utils/kabaret/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8365 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/ui/flow_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/ui/main_window.py
+-rw-rw-rw-   0 root         (0) root         (0)    20792 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/ui/navigation_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/kabaret/ui/widget_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/os.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.868053 libreflow-2.3.2/src/libreflow/utils/search/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16196 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/actor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.869053 libreflow-2.3.2/src/libreflow/utils/search/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.871053 libreflow-2.3.2/src/libreflow/utils/search/data/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      885 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/icons/export.png
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/icons/filter-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/icons/filter-enabled.png
+-rw-rw-rw-   0 root         (0) root         (0)      901 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/icons/import.png
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/icons/magn-glass.png
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/icons/minus-button.png
+-rw-rw-rw-   0 root         (0) root         (0)      735 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/icons/plus-button.png
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/icons/remove.png
+-rw-rw-rw-   0 root         (0) root         (0)      938 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/data/icons/run-button.png
+-rw-rw-rw-   0 root         (0) root         (0)    16126 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/search/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.872053 libreflow-2.3.2/src/libreflow/utils/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20399 2024-04-26 08:19:34.000000 libreflow-2.3.2/src/libreflow/utils/ui/file_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 08:19:43.872053 libreflow-2.3.2/src/libreflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    72742 2024-04-26 08:19:43.000000 libreflow-2.3.2/src/libreflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14481 2024-04-26 08:19:43.000000 libreflow-2.3.2/src/libreflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 08:19:43.000000 libreflow-2.3.2/src/libreflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      212 2024-04-26 08:19:43.000000 libreflow-2.3.2/src/libreflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 08:19:43.000000 libreflow-2.3.2/src/libreflow.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70144 2024-04-26 08:19:34.000000 libreflow-2.3.2/versioneer.py
```

### Comparing `libreflow-2.3.1/CHANGELOG.md` & `libreflow-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: libreflow
+Version: 2.3.2
+Summary: An example flow for kabaret
+Home-page: https://gitlab.com/lfs.coop/libreflow
+Author: Flavio Perez
+Author-email: flavio@lfs.coop
+License: LGPLv3+
+Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: kabaret>=2.2.0rc6
+Requires-Dist: pyside2~=5.0
+Requires-Dist: six~=1.0
+Requires-Dist: kabaret.script-view
+Requires-Dist: kabaret.subprocess-manager
+Requires-Dist: kabaret.flow-contextaul-dict
+Requires-Dist: kabaret.flow-entities
+Requires-Dist: gazu>=0.8.33
+Requires-Dist: minio
+Requires-Dist: timeago
+Requires-Dist: blender-asset-tracer
+Requires-Dist: psutil
+Requires-Dist: fileseq
+Requires-Dist: sentry-sdk
+
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)[^1].
 
@@ -15,14 +47,45 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.3.2] - 2024-04-26
+
+### Added
+
+* Kitsu (Gazu) wrapper has a new method `get_project_type()` for retrieve project type (Short, TV Show etc.)
+* MXF and PRPROJ file formats support.
+* Premiere Pro added in runners list.
+* A parameter in default files to specify the target Kitsu task type. Only used for Kitsu uploadable files.
+
+### Changed
+
+* Users list now sorted alphabetically (by user ID) by default.
+* Default Tasks in Task Manager are now sorted by task position number.
+* Improved log messages for Create Task Default Files and Kitsu Tasks actions.
+
+### Fixed
+
+* Kitsu episodes is now handled in `get_entity_data()` of Kitsu (Gazu) wrapper.
+  * Caused problems when trying to retrieve kitsu entity of a shot when project is a TV Show.
+* File and revision paths are now normalised to avoid opening issues with differents slashes.
+* Task Template now has a function to get path format and fixes the action for creating files in a task template.
+* Import Files action: typo on `Resolving files` popup.
+* User tasks: the display of a file entry's action menu when the file is right-clicked and its secondary action button is clicked.
+* User tasks: dragging a file out of the UI.
+* User tasks: focus detection for keyboard shortcuts when using multiple views in the window
+* View title is updated again when current oid is changed. Fixed confusion when multiple views were docked.
+* View width is no longer expanded if the current oid is on a custom UI page and there are multiple views.
+* Fixed *Create default files* task action when a file is incremented from its base file.
+* Lock a synchronization job starting to be processed by setting its status to `PROCESSING` (avoids multiples processing of the same job from different sessions).
+* Synchronization session: rectified deprecated OIDs and automatic relaunch when an error occurs.
+
 ## [2.3.1] - 2024-03-14
 
 ### Added
 
 * New parameters `width` and `height` in the project settings. These are available in the project default contextual dict.
 * New task icons to display in a shot or asset task list.
   * If a color is defined in a task, the new icon will match it, maintaining its brightness and saturation.
@@ -46,15 +109,14 @@
 * Color of file actions error messages has been adapted to LFS style class color scheme.
 * Value of the *Upload after publish* is not stored anymore in the action value store. It only depends on the *auto upload* project setting.
 * Logging level of the session worker (INFO).
 
 ### Fixed
 
 * Create Kitsu Tasks action: switch to case insensitive for check task templates names.
-* Import Files action: typo on `Resolving files` popup.
 * The `TaskManager.get_task_files()` method now returns enabled only files when corresponding attribute is used.
 * Create default files:
   * `NoneType` error when a default file was created from a base file which has no revision or whose latest revision wasn't available.
   * A default file is now not create by default, when it already exists and use base file mode is enabled.
     * The user can still manually choose to create the revision from base file. This is to avoid issues when action is used in a batch way.
 * User Tasks: 
   * Libreflow bookmarks no longer break the interface
@@ -1450,8 +1512,8 @@
 Initial public commit and pypi setup. This version is an early version of libreflow. It includes a baseflow and examples flows overriding the baseflow. We have been working on departments, files, file version history, and stuff like that.
 
 ### Fixed
 
 issue #6 : Pip Package is now ready for use
 
 
-[^1]: Except we started libreflow MAJOR version number at 1, as we consider our in-house previous flow being version 0.
+[^1]: Except we started libreflow MAJOR version number at 1, as we consider our in-house previous flow being version 0.
```

### Comparing `libreflow-2.3.1/LICENSE` & `libreflow-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/PKG-INFO` & `libreflow-2.3.2/src/libreflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow
-Version: 2.3.1
+Version: 2.3.2
 Summary: An example flow for kabaret
 Home-page: https://gitlab.com/lfs.coop/libreflow
 Author: Flavio Perez
 Author-email: flavio@lfs.coop
 License: LGPLv3+
 Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
 Classifier: Programming Language :: Python :: 3
@@ -47,14 +47,45 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.3.2] - 2024-04-26
+
+### Added
+
+* Kitsu (Gazu) wrapper has a new method `get_project_type()` for retrieve project type (Short, TV Show etc.)
+* MXF and PRPROJ file formats support.
+* Premiere Pro added in runners list.
+* A parameter in default files to specify the target Kitsu task type. Only used for Kitsu uploadable files.
+
+### Changed
+
+* Users list now sorted alphabetically (by user ID) by default.
+* Default Tasks in Task Manager are now sorted by task position number.
+* Improved log messages for Create Task Default Files and Kitsu Tasks actions.
+
+### Fixed
+
+* Kitsu episodes is now handled in `get_entity_data()` of Kitsu (Gazu) wrapper.
+  * Caused problems when trying to retrieve kitsu entity of a shot when project is a TV Show.
+* File and revision paths are now normalised to avoid opening issues with differents slashes.
+* Task Template now has a function to get path format and fixes the action for creating files in a task template.
+* Import Files action: typo on `Resolving files` popup.
+* User tasks: the display of a file entry's action menu when the file is right-clicked and its secondary action button is clicked.
+* User tasks: dragging a file out of the UI.
+* User tasks: focus detection for keyboard shortcuts when using multiple views in the window
+* View title is updated again when current oid is changed. Fixed confusion when multiple views were docked.
+* View width is no longer expanded if the current oid is on a custom UI page and there are multiple views.
+* Fixed *Create default files* task action when a file is incremented from its base file.
+* Lock a synchronization job starting to be processed by setting its status to `PROCESSING` (avoids multiples processing of the same job from different sessions).
+* Synchronization session: rectified deprecated OIDs and automatic relaunch when an error occurs.
+
 ## [2.3.1] - 2024-03-14
 
 ### Added
 
 * New parameters `width` and `height` in the project settings. These are available in the project default contextual dict.
 * New task icons to display in a shot or asset task list.
   * If a color is defined in a task, the new icon will match it, maintaining its brightness and saturation.
@@ -78,15 +109,14 @@
 * Color of file actions error messages has been adapted to LFS style class color scheme.
 * Value of the *Upload after publish* is not stored anymore in the action value store. It only depends on the *auto upload* project setting.
 * Logging level of the session worker (INFO).
 
 ### Fixed
 
 * Create Kitsu Tasks action: switch to case insensitive for check task templates names.
-* Import Files action: typo on `Resolving files` popup.
 * The `TaskManager.get_task_files()` method now returns enabled only files when corresponding attribute is used.
 * Create default files:
   * `NoneType` error when a default file was created from a base file which has no revision or whose latest revision wasn't available.
   * A default file is now not create by default, when it already exists and use base file mode is enabled.
     * The user can still manually choose to create the revision from base file. This is to avoid issues when action is used in a batch way.
 * User Tasks: 
   * Libreflow bookmarks no longer break the interface
```

### Comparing `libreflow-2.3.1/README.md` & `libreflow-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/setup.py` & `libreflow-2.3.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,12 +65,17 @@
             '*.psd',
             '*.psb',
             '*.txt',
             '*.usd',
             '*.fbx',
             '*.json',
             '*.obj',
-            '*.wav'
+            '*.wav',
+            '*.pproj',
+            '*.ttf',
+            '*.otf',
+            '*.nk',
+            '*.jsx',
+            '*.mp4'
         ],
     },
-
 )
```

### Comparing `libreflow-2.3.1/src/libreflow/__init__.py` & `libreflow-2.3.2/src/libreflow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/__init__.py` & `libreflow-2.3.2/src/libreflow/baseflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     MarkSequenceRunner,
     Firefox,
     SessionWorker,
     DefaultEditor,
     ImageMagick,
     RV,
     Nuke,
+    PremierePro,
     DefaultApps,
 )
 from .site import (
     Synchronize, GotoCurrentSiteQueue,
     WorkingSites, ExchangeSites,
     MinioFileUploader, MinioFileDownloader,
     ExchangeSiteChoiceValue,
@@ -603,15 +604,15 @@
 class Admin(flow.Object):
 
     ICON = ("icons.gui", "team-admin")
 
     _project = flow.Parent()
 
     project_settings = flow.Child(ProjectSettings).injectable()
-    users = flow.Child(Users).ui(show_filter=True).injectable()
+    users = flow.Child(Users).ui(show_filter=True, sort_by='ID').injectable()
     multisites = flow.Child(MultisiteConfig).ui(label='Sites')
     kitsu = flow.Child(KitsuConfig)
 
     dependency_templates = flow.Child(DependencyTemplates)
     
     user_environment = flow.Child(UserEnvironment).ui(
         expanded=False,
@@ -903,14 +904,15 @@
         self._RUNNERS_FACTORY.ensure_runner_type(MinioFileUploader)
         self._RUNNERS_FACTORY.ensure_runner_type(MinioFileDownloader)
         self._RUNNERS_FACTORY.ensure_runner_type(SessionWorker)
         self._RUNNERS_FACTORY.ensure_runner_type(Firefox)
         self._RUNNERS_FACTORY.ensure_runner_type(ImageMagick)
         self._RUNNERS_FACTORY.ensure_runner_type(RV)
         self._RUNNERS_FACTORY.ensure_runner_type(Nuke)
+        self._RUNNERS_FACTORY.ensure_runner_type(PremierePro)
 
     def ensure_runners_loaded(self):
         session = self.root().session()
         subprocess_manager = session.get_actor("SubprocessManager")
 
         if self._RUNNERS_FACTORY is None:
             self._RUNNERS_FACTORY = subprocess_manager.create_new_factory(
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/asset.py` & `libreflow-2.3.2/src/libreflow/baseflow/asset.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/departments.py` & `libreflow-2.3.2/src/libreflow/baseflow/departments.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/dependency.py` & `libreflow-2.3.2/src/libreflow/baseflow/dependency.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/entity_manager.py` & `libreflow-2.3.2/src/libreflow/baseflow/entity_manager.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/file.py` & `libreflow-2.3.2/src/libreflow/baseflow/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -748,15 +748,14 @@
         self.comment.apply_preset()
         self.keep_editing.apply_preset()
         self.upload_after_publish.check_default_value()
     
     def update_presets(self):
         self.comment.update_preset()
         self.keep_editing.update_preset()
-        self.upload_after_publish.update_preset()
 
     def run(self, button):
         if button == 'Cancel':
             return
         
         self.update_presets()
 
@@ -977,17 +976,17 @@
         if path == '' or path is None:
             raise Exception((
                 f'Cannot call get_path() on revision {self.oid()} '
                  'since its path is undefined.'
             ))
 
         if not relative:
-            path = os.path.join(
+            path = os.path.normpath(os.path.join(
                 self.root().project().get_root(), path
-            )
+            ))
         
         return path
     
     def update_path(self, path_format=None):
         '''
         Updates the relative path of this revision.
 
@@ -2005,18 +2004,18 @@
     settings = flow.Child(ContextualView).ui(hidden=True)
     path = flow.Computed(cached=True)
 
     def get_name(self):
         return self.name()
 
     def get_path(self):
-        return os.path.join(
+        return os.path.normpath(os.path.join(
             self.root().project().get_root(),
             self.path.get()
-        )
+        ))
 
     def get_last_edit_time(self):
         path = self.get_path()
         if os.path.exists(path):
             return os.path.getmtime(path)
         
         return 0
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/film.py` & `libreflow-2.3.2/src/libreflow/baseflow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/kitsu.py` & `libreflow-2.3.2/src/libreflow/baseflow/kitsu.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,25 @@
                 self._config.project_name.get()
             )
         except requests.exceptions.ConnectionError:
             return None
         else:
             return data['fps']
 
+    def get_project_type(self):
+        import requests
+        try:
+            data = gazu.project.get_project_by_name(
+                self._config.project_name.get()
+            )
+        except requests.exceptions.ConnectionError:
+            return None
+        else:
+            return data['production_type']
+
     def get_entity_type_data(self, entity_type_id):
         return gazu.entity.get_entity_type(entity_type_id)
    
     def get_shot_data(self, name, sequence, episode_name=None):
         if isinstance(sequence, str):
             sequence = self.get_sequence_data(sequence, episode_name)
 
@@ -621,18 +632,23 @@
                 task_types += type_names
         
         return task_types
     
     def get_entity_data(self, contextual_settings):
         kitsu_api = self.root().project().kitsu_api()
         entities_data = {
-            'shot': ['shot', 'sequence'],
+            'shot': ['shot', 'sequence', 'episode'],
             'asset': ['asset'],
         }
         
+        # Remove episode key if kitsu project is not a TV Show
+        project_type = kitsu_api.get_project_type()
+        if project_type != 'tvshow':
+            entities_data['shot'].remove('episode')
+        
         entity_data = {}
         
         for entity_type, entity_keys in entities_data.items():
             for key in entity_keys:
                 entity_data[key] = contextual_settings.get(key, None)
             
             if all(v is not None for v in entity_data.values()):
@@ -640,23 +656,33 @@
                 return entity_data
             else:
                 entity_data = {}
         
         return None
     
     def get_kitsu_entity(self, entity_data):
+        if entity_data is None:
+            return None
+
         entity_type = entity_data['entity_type']
         
         if entity_type == 'shot':
             return self._kitsu_api().get_shot_data(entity_data['shot'], entity_data['sequence'], entity_data.get('episode'))
         elif entity_type == 'asset':
             return self._kitsu_api().get_asset_data(entity_data['asset'])
         else:
             return None
 
+    def set_task_type(self, file_name, task_type):
+        task_types = self.task_type_files.get()
+        task_types[file_name] = task_type
+        self.task_type_files.set(task_types)
+        
+        return self.task_type_files.get()
+
 
 class ChangeKitsuUserLogin(flow.Action):
 
     login = flow.SessionParam('')
 
     _user = flow.Parent()
     _map  = flow.Parent(2)
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/lib.py` & `libreflow-2.3.2/src/libreflow/baseflow/lib.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/maputils.py` & `libreflow-2.3.2/src/libreflow/baseflow/maputils.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/mytasks.py` & `libreflow-2.3.2/src/libreflow/baseflow/mytasks.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/runactions.py` & `libreflow-2.3.2/src/libreflow/baseflow/runactions.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/runners.py` & `libreflow-2.3.2/src/libreflow/baseflow/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,32 @@
 # from kabaret.subprocess_manager.flow import RunAction
 
 from ..utils.kabaret.subprocess_manager.runner_factory import Runner
 from ..utils.kabaret.subprocess_manager.flow import RunAction
 from ..resources.icons import flow as flow_icons
 
 
-FILE_EXTENSIONS = ["blend", "kra", "png", "jpg", "txt", "nk", "abc", "mov", "psd", "psb", "aep", "zip", "mp4", "fbx", "ai", "json", "jsx", "obj", "wav"]
+FILE_EXTENSIONS = ["blend", "kra", "png", "jpg", "txt", "nk", "abc", "mov", "psd", "psb", "aep", "prproj", "zip", "mp4", "mxf", "fbx", "ai", "json", "jsx", "obj", "wav"]
 FILE_EXTENSION_ICONS = {
             "blend": ("icons.libreflow", "blender"),
             "kra": ("icons.libreflow", "krita"),
             "png": ("icons.gui", "picture"),
             "jpg": ("icons.gui", "picture"),
             "txt": ('icons.gui', 'text-file-1'),
             "nk": ("icons.libreflow", "nuke"),
             "abc": ("icons.flow", "alembic"),
             "aep": ("icons.libreflow", "afterfx"),
             "psd": ("icons.flow", "photoshop"),
             "psb": ("icons.flow", "photoshop"),
+            "prproj": ("icons.libreflow", "premiere-pro"),
             "mov": ("icons.flow", "quicktime"),
             "ai":  ("icons.libreflow", "illustrator"),
             "zip": ("icons.libreflow", "archive"),
             "mp4": ("icons.gui", "youtube-logo"),
+            "mxf": ("icons.gui", "youtube-logo"),
             "fbx": ("icons.libreflow", "fbx"),
             "json": ("icons.libreflow", "json"),
             "jsx": ("icons.libreflow", "jsx"),
             "obj": ("icons.libreflow", "3d-object"),
             "wav": ("icons.gui", "youtube-logo"),
         }
 
@@ -220,14 +222,24 @@
     ]
 
     @classmethod
     def supported_extensions(cls):
         return [".nk"]
 
 
+class PremierePro(EditFileRunner):
+
+    ICON = ("icons.libreflow", "premiere-pro")
+    TAGS = ["Video Editing"]
+
+    @classmethod
+    def supported_extensions(cls):
+        return [".prproj"]
+
+
 class PythonRunner(Runner):
 
     def executable(self):
         return sys.executable
     
     def show_terminal(self):
         return False
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/shot.py` & `libreflow-2.3.2/src/libreflow/baseflow/shot.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/site.py` & `libreflow-2.3.2/src/libreflow/baseflow/site.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def choices(self):
         return self.CHOICES
 
 
 class JobStatus(PropertyValue):
 
     DEFAULT_EDITOR = 'choice'
-    CHOICES = ['WFA', 'WAITING', 'PROCESSED', 'ERROR', 'PAUSE', 'DONE']
+    CHOICES = ['WFA', 'WAITING', 'PROCESSING', 'PROCESSED', 'ERROR', 'PAUSE', 'DONE']
 
     def choices(self):
         return self.CHOICES
 
 
 class ResetJob(flow.Action):
 
@@ -614,14 +614,15 @@
         )
 
     def process(self, job):
         if not job.check_valid_state():
             return
         
         try:
+            job.status.set('PROCESSING')
             sync_manager = self.root().project().get_exchange_site().sync_manager
         
             if job.type.get() == 'Upload':
                 sync_manager.upload(
                     job.get_server_path(),
                     job.get_local_path()
                 )
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/task.py` & `libreflow-2.3.2/src/libreflow/baseflow/task.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/task_manager.py` & `libreflow-2.3.2/src/libreflow/baseflow/task_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,29 +198,30 @@
             mgr = self.root().project().get_task_manager()
             default_files = mgr.get_task_files(
                 self._task.name(), enabled_only=True
             )
 
             self._cache = {}
 
-            for n, (file_name, path_format, file_type, optional, is_primary_file, use_base_file, template_file, template_revision, from_task, base_file_name, auto_open) in default_files.items():
+            for n, (file_name, path_format, file_type, optional, is_primary_file, use_base_file, template_file, template_revision, from_task, base_file_name, target_kitsu_task_type, auto_open) in default_files.items():
                 n = file_name.replace('.', '_')
                 exists = self._file_exists(file_name)
                 self._cache[n] = dict(
                     file_name=file_name,
                     file_type=file_type,
                     path_format=path_format,
                     create=not optional and not exists,
                     exists=exists,
                     is_primary_file=is_primary_file,
                     use_base_file=use_base_file,
                     template_file=template_file,
                     template_file_revision=template_revision,
                     from_task=from_task,
                     base_file_name=base_file_name,
+                    target_kitsu_task_type=target_kitsu_task_type,
                     auto_open=auto_open,
                 )
         
         return self._cache.keys()
     
     def columns(self):
         return ['Do create', 'File', 'From']
@@ -320,33 +321,34 @@
         file_name = default_file.file_name.get()
         name, ext = os.path.splitext(file_name)
         target_file = None
 
         # Create default file
         if not default_file.exists.get():
             if ext:
+                print(f'Create Task Default Files : Creating File {file_name}')
                 target_file = self._task.files.add_file(
                     name, ext[1:],
                     display_name=file_name,
                     tracked=True,
                     default_path_format=default_file.path_format.get()
                 )
-                print('create default file')
             else:
+                print(f'Create Task Default Files : Creating Folder {file_name}')
                 target_file = self._task.files.add_folder(
                     name,
                     display_name=file_name,
                     tracked=True,
                     default_path_format=default_file.path_format.get()
                 )
-                print('create default folder')
             
             target_file.file_type.set(default_file.file_type.get())
             target_file.is_primary_file.set(default_file.is_primary_file.get())
         else:
+            print(f'Create Task Default Files : File {file_name} exists')
             target_file = self._task.files[default_file.name()]
         
         source_revision = None
         comment = None
         
         # Increment file from base/template file
         if default_file.use_base_file.get():
@@ -362,33 +364,36 @@
 
                 if exists:
                     source_file = source_task.files[base_file_name.replace('.', '_')]
                     source_revision = source_file.get_head_revision(sync_status="Available")
                     
                     if source_revision is not None:
                         comment = f'from base file {base_file_name} {source_revision.name()}'
-                        print(f'Use base file {source_file.oid()} - {source_revision.name()}')
+                        print(f'Create Task Default Files : Use Base File {source_file.display_name.get()} - {source_revision.name()}')
         else:
             template_file = default_file.template_file.get()
             if template_file is not None:
                 template_file_revision = default_file.template_file_revision.get()
                 if template_file_revision == 'Latest':
                     source_revision = template_file.get_head_revision(sync_status='Available')
                 else:
                     source_revision = template_file.get_revision(template_file_revision)
                 
                 if source_revision is not None:
                     comment = f'from template {source_revision.name()}'
-                    print(f'Use template file {template_file.oid()} - {source_revision.name()}')
+                    print(f'Create Task Default Files : Use template file {template_file.oid()} - {source_revision.name()}')
 
         if source_revision is not None and os.path.exists(source_revision.get_path()):
-            print('revision exists: copy')
             r = target_file.add_revision(comment=comment)
+            print(f'Create Task Default Files : Creating Revision {file_name} {r.name()}')
+
             target_path = r.get_path()
             os.makedirs(os.path.dirname(target_path), exist_ok=True)
+            
+            print(f'Create Task Default Files : Copying Source Revision')
 
             if ext:
                 shutil.copy2(source_revision.get_path(), target_path)
             else:
                 shutil.copytree(source_revision.get_path(), target_path)
 
 
@@ -576,23 +581,38 @@
     with flow.group('Template file settings'):
         template_file          = flow.Connection(related_type=TrackedFile)
         # template_file_revision = Property(TemplateFileRevision)
         template_file_revision = Property()
     with flow.group('Base file settings'):
         from_task = Property()
         base_file_name = Property()
+    with flow.group('Kitsu settings'):
+        target_kitsu_task_type = Property().ui(label='Target Task Type').watched()
 
     action_display_order = Property()
     visible_action_count = Property()
 
     remove = flow.Child(RemoveDefaultFileAction)
 
-    # def child_value_changed(self, child_value):
-    #     if child_value is self.template_file:
-    #         self.template_file_revision.revert_to_default()
+    def child_value_changed(self, child_value):
+        super(DefaultFile, self).child_value_changed(child_value)
+        if child_value is self.target_kitsu_task_type:
+            # Update task type files dict on kitsu bindings
+            if child_value.get() is not None and child_value.get() not in ['', []]:
+                self.root().project().kitsu_bindings().set_task_type(
+                    self.file_name.get(), child_value.get()
+                )
+            
+            # Remove in task type files dict on kitsu bindings
+            else:
+                task_type_files = self.root().project().kitsu_bindings().task_type_files.get()
+
+                if self.file_name.get() in task_type_files:
+                    task_type_files.pop(self.file_name.get())
+                    self.root().project().kitsu_bindings().task_type_files.set(task_type_files)
 
 
 class DefaultFiles(CustomEntityCollection):
 
     add_dft_file = flow.Child(CreateDefaultFileAction).ui(
         label='Add default file'
     )
@@ -740,14 +760,39 @@
 
 class EditableKitsuTaskNames(PropertyValue):
 
     add_action = flow.Child(AddKitsuTaskNameAction).ui(label='Add')
     remove_action = flow.Child(RemoveKitsuTaskNameAction).ui(label='Remove')
 
 
+class KitsuTargetTaskType(flow.values.SessionValue):
+  
+    _action = flow.Parent()
+    _dft_task = flow.Parent(3)
+
+    add_action = flow.Child(AddKitsuTaskNameAction).ui(label='Add')
+    remove_action = flow.Child(RemoveKitsuTaskNameAction).ui(label='Remove')
+
+    def update_default_value(self):
+        # Reset value with Kitsu task names defined on default task.
+        return self.set(self._dft_task.kitsu_tasks.get())
+    
+    def _fill_ui(self, ui):
+        super(KitsuTargetTaskType, self)._fill_ui(ui)
+
+        # Use condition only if hidden param is not defined or set to False
+        if ui['hidden'] is False:
+            _, ext = os.path.splitext(self._action._dft_file.file_name.get())
+            # Hide param if file has no extension or cannot be uploaded to Kitsu
+            ui['hidden'] = bool(
+                not ext or self.root().project().kitsu_config().is_uploadable(
+                    self._action._dft_file.file_name.get()) is False
+            )
+
+
 class EditDefaultTaskFile(flow.Action):
     """
     Allows to edit a default task's file.
     """
 
     ICON = ('icons.libreflow', 'edit-blank')
 
@@ -763,14 +808,17 @@
     with flow.group('Template file settings'):
         template_file          = flow.Connection(related_type=TrackedFile).watched()
         # template_file_revision = flow.SessionParam(TemplateFileRevision)
         template_file_revision = flow.SessionParam('Latest', value_type=TemplateFileRevision)
     with flow.group('Base file settings'):
         from_task = flow.SessionParam()
         base_file_name = flow.SessionParam()
+    with flow.group('Kitsu settings'):
+        target_kitsu_task_type = flow.SessionParam(None, KitsuTargetTaskType).ui(label='Target Task Type')
+    
     action_display_order = flow.SessionParam(dict)
     visible_action_count = flow.SessionParam(0)
 
     _dft_file   = flow.Parent()
     _map        = flow.Parent(2)
     _dft_task   = flow.Parent(3)
 
@@ -795,14 +843,15 @@
                 self.template_file.set_watched(True)
         else:
             self.template_file.set(None)
 
         self.template_file_revision.set(self._dft_file.template_file_revision.get())
         self.from_task.set(self._dft_file.from_task.get())
         self.base_file_name.set(self._dft_file.base_file_name.get())
+        self.target_kitsu_task_type.set(self._dft_file.target_kitsu_task_type.get())
         self.action_display_order.set(self._dft_file.action_display_order.get())
         self.visible_action_count.set(self._dft_file.visible_action_count.get())
 
         buttons = ['Save']
         mgr = self.root().project().get_task_manager()
         task_template = mgr.task_templates[self._dft_task.template.get()]
 
@@ -838,14 +887,15 @@
             dft_file.is_primary_file.set(self.is_primary_file.get())
             dft_file.use_base_file.set(self.use_base_file.get())
             dft_file.auto_open.set(self.auto_open.get())
             dft_file.template_file.set(self.template_file.get())
             dft_file.template_file_revision.set(self.template_file_revision.get())
             dft_file.from_task.set(self.from_task.get())
             dft_file.base_file_name.set(self.base_file_name.get())
+            dft_file.target_kitsu_task_type.set(self.target_kitsu_task_type.get())
             dft_file.action_display_order.set(self.action_display_order.get())
             dft_file.visible_action_count.set(self.visible_action_count.get())
 
         self._map.touch()
 
 
 class RemoveDefaultTaskFile(flow.Action):
@@ -869,40 +919,52 @@
             f'from task <b>{self._task.name()}</b> files ?'
         )
         return ['Confirm', 'Cancel']
     
     def run(self, button):
         if button == 'Cancel':
             return
+        
+        # Remove in task type files dict on kitsu bindings
+        task_type_files = self.root().project().kitsu_bindings().task_type_files.get()
 
+        if self._dft_file.file_name.get() in task_type_files:
+            task_type_files.pop(self._dft_file.file_name.get())
+            self.root().project().kitsu_bindings().task_type_files.set(task_type_files)
+        
         self._map.edits.remove(self._dft_file.name())
         self._map.touch()
         self._mgr.default_files.touch()
 
 
 class AddDefaultTaskFileEdit(flow.Action):
     """
     Allows to add a file in the files of a default task.
     """
 
-    file_name   = flow.SessionParam('').ui(label='Name')
+    file_name   = flow.SessionParam('').ui(label='Name').watched()
     file_type   = flow.SessionParam('Works', FileTypeValue)
     path_format = flow.SessionParam(DEFAULT_PATH_FORMAT, PathFormatValue)
     enabled     = flow.SessionParam(True).ui(editor='bool')
     optional    = flow.SessionParam(False).ui(editor='bool')
     is_primary_file = flow.SessionParam(False).ui(editor='bool')
     use_base_file = flow.SessionParam(False).ui(editor='bool')
     auto_open = flow.SessionParam(False).ui(editor='bool',
         tooltip="Automatically open last revision at double-click")
     with flow.group('Template file settings'):
         template_file          = flow.Connection(related_type=TrackedFile).watched()
         template_file_revision = flow.SessionParam('Latest', value_type=TemplateFileRevision)
     with flow.group('Base file settings'):
         from_task = flow.SessionParam('')
         base_file_name = flow.SessionParam('')
+    with flow.group('Kitsu settings'):
+        target_kitsu_task_type = flow.SessionParam(None, KitsuTargetTaskType).ui(
+            label='Target Task Type',
+            hidden=True
+        )
 
     _map = flow.Parent()
     _task = flow.Parent(2)
     _mgr = flow.Parent(4)
 
     def get_buttons(self):
         self.message.set('<h2>Add default task file</h2>')
@@ -932,21 +994,30 @@
         df.is_primary_file.set(self.is_primary_file.get())
         df.use_base_file.set(self.use_base_file.get())
         df.auto_open.set(self.auto_open.get())
         df.template_file.set(self.template_file.get())
         df.template_file_revision.set(self.template_file_revision.get())
         df.from_task.set(self.from_task.get())
         df.base_file_name.set(self.base_file_name.get())
+        df.target_kitsu_task_type.set(self.target_kitsu_task_type.get())
 
         self._map.touch()
         self._mgr.default_files.touch()
     
     def child_value_changed(self, child_value):
         if child_value is self.template_file:
             self.template_file_revision.revert_to_default()
+        # If file is uploadable to Kitsu, target Kitsu task type is set.
+        elif child_value is self.file_name:
+            _, ext = os.path.splitext(self.file_name.get())
+
+            if ext and self.root().project().kitsu_config().is_uploadable(self.file_name.get()):
+                self.target_kitsu_task_type.update_default_value()
+            else:
+                self.target_kitsu_task_type.set(None)
     
     def _filename_is_valid(self):
         title = '<h2>Add default task file</h2>'
 
         if self.file_name.get() == '':
             self.message.set((
                 f'{title}<font color=#D66700>'
@@ -978,25 +1049,36 @@
     auto_open = flow.Computed().ui(editable=False, editor='bool')
     with flow.group('Template file settings'):
         template_file          = flow.Computed().ui(editable=False)
         template_file_revision = flow.Computed().ui(editable=False)
     with flow.group('Base file settings'):
         from_task = flow.Computed().ui(editable=False)
         base_file_name = flow.Computed().ui(editable=False)
+    with flow.group('Kitsu settings'):
+        target_kitsu_task_type = flow.Computed().ui(editable=False, label='Target Task Type')
 
     action_display_order = flow.Computed().ui(editable=False)
     visible_action_count = flow.Computed().ui(editable=False)
     is_edit     = flow.Computed().ui(editable=False, editor='bool')
 
     edit        = flow.Child(EditDefaultTaskFile)
     remove      = flow.Child(RemoveDefaultTaskFile)
 
     _map = flow.Parent()
     
     def compute_child_value(self, child_value):
+        # If value is empty, we check if there is one in the task type files dict on kitsu bindings.
+        if child_value is self.target_kitsu_task_type:
+            cache_child_value = self._map.get_child_value(self.name(), child_value.name())
+            task_type_files = self.root().project().kitsu_bindings().get_task_types(self.file_name.get())
+
+            if (cache_child_value is None or cache_child_value in ['', []]) and task_type_files:
+                self._map.edits[self.name()].target_kitsu_task_type.set(task_type_files)
+                return child_value.set(task_type_files)
+
         child_value.set(self._map.get_child_value(self.name(), child_value.name()))
 
 
 class DefaultTaskFiles(flow.DynamicMap):
 
     edits = flow.Child(DefaultFiles).ui(hidden=True)
 
@@ -1056,14 +1138,15 @@
                     is_primary_file=default_file.is_primary_file.get(),
                     auto_open=bool(default_file.auto_open.get()),
                     use_base_file=default_file.use_base_file.get(),
                     template_file=template_file.oid() if template_file else None,
                     template_file_revision=default_file.template_file_revision.get(),
                     from_task=default_file.from_task.get(),
                     base_file_name=default_file.base_file_name.get(),
+                    target_kitsu_task_type=default_file.target_kitsu_task_type.get(),
                     action_display_order=action_display_order,
                     visible_action_count=visible_action_count
                 ))
                 self._cache[name] = data
             
             # Collect remaining edits
             for name in edit_names:
@@ -1084,14 +1167,15 @@
                     is_primary_file=default_file.is_primary_file.get(),
                     auto_open=bool(default_file.auto_open.get()),
                     use_base_file=default_file.use_base_file.get(),
                     template_file=template_file.oid() if template_file else None,
                     template_file_revision=default_file.template_file_revision.get(),
                     from_task=default_file.from_task.get(),
                     base_file_name=default_file.base_file_name.get(),
+                    target_kitsu_task_type=default_file.target_kitsu_task_type.get(),
                     action_display_order=default_file.action_display_order.get(),
                     visible_action_count=default_file.visible_action_count.get(),
                     is_edit=True
                 )
                 self._cache[name] = data
         
         return self._cache.keys()
@@ -1340,28 +1424,28 @@
 
     def run(self, button):
         if button == 'Back':
             return self.get_result(next_action=self._map.add_kitsu_tasks.oid())
         
         for item in self.tasks.mapped_items():
             if not self._mgr.default_tasks.has_mapped_name(item.task_name.get()):
+                print(f'Create Kitsu Tasks : Creating Default Task {item.task_name.get()}')
+                
                 t = self._mgr.default_tasks.add_default_task(
                     item.task_name.get(),
                     item.task_name.get(),
                     item.task_type.get(),
                     0
                 )
 
                 kitsu_task_names = t.kitsu_tasks.get() or []
                 kitsu_task_names.append(item.task_name.get())
                 t.kitsu_tasks.set(kitsu_task_names)
             else:
                 continue
-            
-            print(f'Create default task: {item.task_name.get()}')
         
         self._mgr.default_tasks.touch()
 
 
 class DefaultTask(Entity):
     """
     Defines a set of presets used to create a task in the project.
@@ -1468,14 +1552,33 @@
     add_kitsu_tasks = flow.Child(CreateKitsuTasksPage1)
     add_kitsu_tasks_page2 = flow.Child(CreateKitsuTasksPage2).ui(hidden=True)
 
     @classmethod
     def mapped_type(cls):
         return DefaultTask
 
+    def mapped_names(self, page_num=0, page_size=None):
+        '''
+        Returns task names sorted by task positions.
+        '''
+        names = super(DefaultTasks, self).mapped_names(page_num, page_size)
+        return sorted(names, key=self.get_task_position)
+
+    def get_task_position(self, task_name):
+        '''
+        Returns the position of the task `task_name` in this
+        collection. If not defined (i.e. not `None` neither `""`),
+        returns `0`.
+        '''
+        super(DefaultTasks, self).mapped_names() # ensure cache exists
+        pos = self._document_cache[task_name].get('position')
+        if pos is None or pos == "":
+            pos = 0
+        return pos
+
     def add_default_task(self, name, display_name, template_name, position=-1, code=None, prefix=None, path_format=None, entity_filter=None, enabled=True, optional=False, icon=None):
         if position < 0:
             position = len(self)
         
         dt = self.add(name)
         dt.display_name.set(display_name)
         dt.code.set(code)
@@ -1544,14 +1647,20 @@
     prefix = Property()
     color = Property(EditableTaskColor)
     icon  = Property()
     files = flow.Child(DefaultFiles).ui(expanded=True)
     path_format = Property()
     primary_files = flow.Computed(None).ui(editable=False)
 
+    def get_path_format(self):
+        '''
+        Returns the path format of this task template.
+        '''
+        return self.path_format.get()
+
     def compute_child_value(self, child_value):
         if child_value is self.primary_files:
             files = []
             for dft_file in self.files.mapped_items():
                 if dft_file.enabled.get() and dft_file.is_primary_file.get():
                     files.append(dft_file.file_name.get())
             
@@ -1959,14 +2068,15 @@
                             df.optional.get(),
                             df.is_primary_file.get(),
                             df.use_base_file.get(),
                             template_file,
                             df.template_file_revision.get(),
                             df.from_task.get(),
                             df.base_file_name.get(),
+                            df.target_kitsu_task_type.get(),
                             df.auto_open.get(),
                         )
         
         return files
     
     def has_default_task(self, task_name):
         return self.default_tasks.has_mapped_name(task_name)
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/controller.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/controller.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/delegate.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/delegate.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/file.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/file.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/file_history.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/file_history.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/file_list.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/file_list.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/importfiles/custom_widget.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/importfiles/custom_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             self.add_files(self.session.cmds.Flow.get_value(self.oid+'/paths'))
             self.session.cmds.Flow.set_value(self.oid+'/paths', [])
             self.session.cmds.Flow.set_value(self.oid+'/source_task', '')
 
     def add_files(self, paths):
         self.button_import.setEnabled(False)
         self.list.show()
-        self.popup.pop('Resovling files', 'Please wait...')
+        self.popup.pop('Resolving files', 'Please wait...')
         QtWidgets.QApplication.processEvents()
         QtWidgets.QApplication.processEvents()
 
         self.session.cmds.Flow.call(self.oid, 'resolve_paths', [paths], {})
         self.list.refresh(True)
        
         self.popup.hide()
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/importfiles/files_list.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/importfiles/files_list.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/importfiles/target_wizard.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/importfiles/target_wizard.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/components.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/components.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/edit_dialog.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/edit_dialog.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/file_list.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/file_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.build()
       
     def mousePressEvent(self, event):
         data = self.widget.task_item.file_data[self.widget.row]
         data.update_actions()
 
         has_actions = self.widget.action_manager.update_oid_menu(
-            data.oid, self.menu, with_submenus=True
+            data.oid(), self.menu, with_submenus=True
         )
 
         super(BaseFileActionsButton, self).mousePressEvent(event)
 
     def _on_action_menu_triggered(self, action):
         self.widget.flow_page.show_action_dialog(action.oid)
 
@@ -174,15 +174,15 @@
     def _on_context_menu_requested(self, pos):
         index = self.indexAt(pos)
         if not index.isValid():
             return
         
         data = self.task_item.file_data[index.row()]
         has_actions = self.action_manager.update_oid_menu(
-            data.oid, self.action_menu, with_submenus=True
+            data.oid(), self.action_menu, with_submenus=True
         )
 
         if has_actions:
             self.action_menu.exec_(self.viewport().mapToGlobal(pos))
     
     def _on_item_double_clicked(self, index):
         data = self.task_item.file_data[index.row()]
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/mytasks.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/mytasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -717,15 +717,15 @@
     def entered_row_boundary(self, entered):
         pass
 
 
 class MyTasksList(HeaderlessTableView):
 
     def __init__(self, page_widget):
-        super().__init__()
+        super(MyTasksList, self).__init__(page_widget)
         self.page_widget = page_widget
         self.tasks_expanded = self.page_widget.get_user_expanded()
         self.cellsContent = []
 
         self.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
 
         # Set attributes for drag handler
@@ -741,14 +741,15 @@
 
         # Display a row line when a task can be resized
         # self.setItemDelegate(TaskBorderDelegate(self))
     
     def eventFilter(self, obj, event):
         # Enable drag if mouse click is press
         if event.type() == QtCore.QEvent.MouseButtonPress:
+            self.page_widget.setFocus()
             if self.row_index() != -1:
                 task_widget = self.cellWidget(self.row_index(), 0)
 
                 # Only accept if task is expanded
                 if task_widget and task_widget.expanded:
                     # Store mouse position and scroll value
                     self.m_mouse_pos = self.mapFromGlobal(QtGui.QCursor.pos())
@@ -1083,15 +1084,15 @@
     def _on_fdt_button_clicked(self):
         webbrowser.open('https://fdt.lesfees.net/')
 
 
 class MyTasksContent(QtWidgets.QWidget):
 
     def __init__(self, page_widget):
-        super(MyTasksContent, self).__init__()
+        super(MyTasksContent, self).__init__(page_widget)
         self.setObjectName('MyTasksContent')
         self.page_widget = page_widget
 
         self.setAttribute(QtCore.Qt.WA_StyledBackground, True)
         self.setStyleSheet('#MyTasksContent { background-color: #232d33; border-radius: 5px; }')
 
         self.build()
@@ -1153,17 +1154,22 @@
         self.list_compare.finished.connect(self.needs_update)
 
         self.auto_compare.setInterval(30000)
         self.auto_compare.timeout.connect(self.compare_thread.start)
 
         self.content.search.widget.textChanged.connect(self.content.list.refresh_search)
         self.content.list.refresh()
+
+        self.setFocus()
     
     def sizeHint(self):
-        return QtCore.QSize(2000, 2000)
+        return QtCore.QSize(0, 2880)
+
+    def mousePressEvent(self, event):
+        self.setFocus()
     
     def keyPressEvent(self, event):
         super(MyTasksPageWidget, self).keyPressEvent(event)
 
         if event.key() == QtCore.Qt.Key_Shift:
             self.content.list.toggle_description()
             self.key_press_start_time = time.time()
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/mytasks/qmodel.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/mytasks/qmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         if role == QtCore.Qt.UserRole:
             data = self.task_item.file_data[index.row()]
             return data
 
     def mimeData(self, indexes):
         mime_data = super(BaseQFileListModel, self).mimeData(indexes)
         oids = [
-            self.task_item.file_data[index.row()].oid
+            self.task_item.file_data[index.row()].oid()
             for index in indexes
         ]
         md = self.session.cmds.Flow.to_mime_data(oids)
         for data_type, data in md.items():
             mime_data.setData(data_type, data)
 
         return mime_data
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/qmodel.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/qmodel.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/ui/task.py` & `libreflow-2.3.2/src/libreflow/baseflow/ui/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         self.key_press_start_time = -1
     
     def on_touch_event(self, oid):
         if self.controller is not None:
             self.controller.on_touch_event(oid)
     
     def sizeHint(self):
-        return QtCore.QSize(2000, 2000)
+        return QtCore.QSize(0, 2880)
     
     def keyPressEvent(self, event):
         super(TaskPageWidget, self).keyPressEvent(event)
 
         if event.key() == QtCore.Qt.Key_Escape:
             # This will automatically reset the selected item in the controller
             # (see selectionChanged())
@@ -475,15 +475,15 @@
         # Add widgets to Main Layout
         grid.addWidget(scroll, 0, 0, 1, 4)
         grid.setColumnStretch(1, 1)
         grid.addWidget(self.button_visibility_toggle, 1, 2)
         grid.addWidget(button_add_task, 1, 3)
     
     def sizeHint(self):
-        return QtCore.QSize(300, 800)
+        return QtCore.QSize(0, 2880)
     
     def refresh_list(self):
         # Clear all existing tasks
         for i in reversed(range(self.task_list_lo.count())):
             self.task_list_lo.itemAt(i).widget().deleteLater()
         
         # Create tasks buttons
```

### Comparing `libreflow-2.3.1/src/libreflow/baseflow/users.py` & `libreflow-2.3.2/src/libreflow/baseflow/users.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/custom_home/__init__.py` & `libreflow-2.3.2/src/libreflow/custom_home/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/custom_home/ui.py` & `libreflow-2.3.2/src/libreflow/custom_home/ui.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/custom_home/wizard.py` & `libreflow-2.3.2/src/libreflow/custom_home/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -4490,15 +4490,15 @@
 
         self.setup_steps.refresh()
 
         if self.get_default_page() is not None:
             self.reset_store_values()
 
     def sizeHint(self):
-        return QtCore.QSize(0, 3840)
+        return QtCore.QSize(0, 2880)
 
     def reset_store_values(self):
         return self.session.cmds.Flow.call(
             self.oid, 'reset_store_values', [], {}
         )
 
     def get_project_store_name(self):
```

### Comparing `libreflow-2.3.1/src/libreflow/examples/demoflow/film.py` & `libreflow-2.3.2/src/libreflow/examples/demoflow/film.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/examples/demoflow/lib.py` & `libreflow-2.3.2/src/libreflow/examples/demoflow/lib.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/examples/majorque/__init__.py` & `libreflow-2.3.2/src/libreflow/examples/majorque/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/examples/majorque/departments.py` & `libreflow-2.3.2/src/libreflow/examples/majorque/departments.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/examples/majorque/file.py` & `libreflow-2.3.2/src/libreflow/examples/majorque/file.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/examples/majorque/film.py` & `libreflow-2.3.2/src/libreflow/examples/majorque/film.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/examples/majorque/kitsu.py` & `libreflow-2.3.2/src/libreflow/examples/majorque/kitsu.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/examples/majorque/lib.py` & `libreflow-2.3.2/src/libreflow/examples/majorque/lib.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/examples/majorque/runners.py` & `libreflow-2.3.2/src/libreflow/examples/majorque/runners.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/gui.py` & `libreflow-2.3.2/src/libreflow/gui.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/jobs_cleaner.py` & `libreflow-2.3.2/src/libreflow/jobs_cleaner.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/jobs_node.py` & `libreflow-2.3.2/src/libreflow/jobs_node.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.abc` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.abc`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.aep` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.aep`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.ai` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.ai`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.blend` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.blend`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.fbx` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.fbx`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.jpg` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.jpg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.kra` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.kra`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.mov` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.mov`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.obj` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.obj`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.png` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.psb` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.psb`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.psd` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.psd`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.usd` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.usd`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/file_templates/template.wav` & `libreflow-2.3.2/src/libreflow/resources/file_templates/template.wav`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/applications/rv.png` & `libreflow-2.3.2/src/libreflow/resources/icons/applications/rv.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/flow/alembic.png` & `libreflow-2.3.2/src/libreflow/resources/icons/flow/alembic.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/flow/explorer.png` & `libreflow-2.3.2/src/libreflow/resources/icons/flow/explorer.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/flow/photoshop.png` & `libreflow-2.3.2/src/libreflow/resources/icons/flow/photoshop.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/flow/quicktime.png` & `libreflow-2.3.2/src/libreflow/resources/icons/flow/quicktime.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/add-file.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/add-file.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/add-folder.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/add-folder.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/arrow-down.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/arrow-down.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/arrow-right.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/arrow-right.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/check-box-empty-dark.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/check-box-empty-dark.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/clean.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/clean.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/close.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/close.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/compositing.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/compositing.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/duplicate.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/duplicate.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/location-worldwide-disabled.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/location-worldwide-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/location-worldwide.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/location-worldwide.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/maximize.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/maximize.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/menu.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/menu.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/menu_dots.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/menu_dots.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/minimize.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/minimize.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/misc.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/misc.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/mytasks-disabled.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/mytasks-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/mytasks.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/mytasks.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-left-disabled.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-left-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-left.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-left.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-refresh-disabled.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-refresh-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-refresh.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-refresh.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-right-disabled.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-right-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/nav-arrow-right.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/nav-arrow-right.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/ref-broken.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/ref-broken.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/ref.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/ref.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/refresh.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/refresh.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/send.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/send.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/gui/send2.png` & `libreflow-2.3.2/src/libreflow/resources/icons/gui/send2.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/history/check.png` & `libreflow-2.3.2/src/libreflow/resources/icons/history/check.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/history/done.png` & `libreflow-2.3.2/src/libreflow/resources/icons/history/done.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/history/retake.png` & `libreflow-2.3.2/src/libreflow/resources/icons/history/retake.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/history/wfa.png` & `libreflow-2.3.2/src/libreflow/resources/icons/history/wfa.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/history/wip.png` & `libreflow-2.3.2/src/libreflow/resources/icons/history/wip.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/history/working_copy.png` & `libreflow-2.3.2/src/libreflow/resources/icons/history/working_copy.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/history/working_copy_mine.png` & `libreflow-2.3.2/src/libreflow/resources/icons/history/working_copy_mine.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/3d-object.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/3d-object.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/active_site.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/active_site.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/afterfx.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/afterfx.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/archive.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/archive.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/available.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/available.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/blank.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/blank.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/blender.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/blender.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/checked-symbol-colored.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/checked-symbol-colored.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/checked-symbol.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/checked-symbol.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/circle-shape-outline.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/circle-shape-outline.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/circle-shape-right-eye-outline.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/circle-shape-right-eye-outline.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/circular-shape-right-eye-silhouette.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/circular-shape-right-eye-silhouette.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/circular-shape-silhouette.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/circular-shape-silhouette.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/clean.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/clean.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/clipboard.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/clipboard.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/compare-previews.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/compare-previews.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/cross-mark-on-a-black-circle-background-colored.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/cross-mark-on-a-black-circle-background-colored.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/custom_home_star.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/custom_home_star.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/delete.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/delete.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/dependencies.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/dependencies.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/download.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/download.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/downloadable.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/downloadable.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/duplicate.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/duplicate.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/edit-blank.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/edit-blank.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/edit-lock-green.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/edit-lock-green.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/edit-lock-red.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/edit-lock-red.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/error.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/error.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/exchange.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/exchange.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/exclamation-sign-colored.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/exclamation-sign-colored.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/fbx.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/fbx.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/firefox.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/firefox.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/hide.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/hide.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/history.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/history.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/illustrator.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/illustrator.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/json.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/json.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/jsx.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/jsx.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_done.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_done.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_oklodv.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_oklodv.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_omit.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_omit.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_retake.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_retake.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_todo.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_todo.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_wfa.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_wfa.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/kitsu_status_wip.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/kitsu_status_wip.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/krita.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/krita.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/lock-green.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/lock-green.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/lock-red.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/lock-red.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/log_out.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/log_out.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/multi-share-option.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/multi-share-option.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/nuke.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/nuke.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/origin-site.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/origin-site.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/padlock.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/padlock.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/padlock_green.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/padlock_green.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/padlock_red.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/padlock_red.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/publish-ae.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/publish-ae.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/publish-blender.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/publish-blender.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/publish.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/publish.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/quicktime.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/quicktime.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/refresh.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/refresh.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/request.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/request.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/requestable.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/requestable.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/run.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/run.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/show.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/show.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/stop.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/stop.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/sync.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/sync.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/sync_arrow.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/sync_arrow.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/time_format.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/time_format.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/unavailable.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/unavailable.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/upload.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/upload.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/vscodium.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/vscodium.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/waiting.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/waiting.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/warning.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/warning.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/libreflow/watch.png` & `libreflow-2.3.2/src/libreflow/resources/icons/libreflow/watch.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/done.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/done.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/err.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/err.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/inv.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/inv.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/none.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/none.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/nys.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/nys.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/oop.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/oop.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/rtk.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/rtk.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/rvw.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/rvw.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/wait.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/wait.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/warn.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/warn.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/status/wip.png` & `libreflow-2.3.2/src/libreflow/resources/icons/status/wip.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/tasks/animation.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/tasks/animation.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/tasks/clean.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/tasks/clean.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/tasks/colo.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/tasks/colo.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/tasks/compositing.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/tasks/compositing.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/tasks/design.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/tasks/design.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/tasks/layout.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/tasks/layout.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/tasks/lighting.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/tasks/lighting.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/tasks/modeling.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/tasks/modeling.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/tasks/rigging.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/tasks/rigging.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/icons/tasks/shading.svg` & `libreflow-2.3.2/src/libreflow/resources/icons/tasks/shading.svg`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/mark_sequence/fields/default.json` & `libreflow-2.3.2/src/libreflow/resources/mark_sequence/fields/default.json`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/scripts/blender/disable_save_keymap.py` & `libreflow-2.3.2/src/libreflow/resources/scripts/blender/disable_save_keymap.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/styles/lfs_tech/__init__.py` & `libreflow-2.3.2/src/libreflow/resources/styles/lfs_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/resources/styles/lfs_tech/lfs_tech_style.css` & `libreflow-2.3.2/src/libreflow/resources/styles/lfs_tech/lfs_tech_style.css`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/scripts/mark_sequence.py` & `libreflow-2.3.2/src/libreflow/scripts/mark_sequence.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/scripts/session_worker.py` & `libreflow-2.3.2/src/libreflow/scripts/session_worker.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/session.py` & `libreflow-2.3.2/src/libreflow/session.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/sync.py` & `libreflow-2.3.2/src/libreflow/sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 import argparse
 import time
+import traceback
 
 from .session import BaseCLISession
 
 
 def parse_remaining_args(args):
     parser = argparse.ArgumentParser(
         description='Libreflow Synchronization Session Arguments'
@@ -49,48 +50,56 @@
         "ensure_runners_loaded",
         args={}, kwargs={}
     )
 
     if site:
         os.environ["KABARET_SITE_NAME"] = site
     
-    site_oid = "/%s/admin/sites/%s" % (project, site)
-    sync_action = "/%s/admin/process_jobs" % project
-    job_queue_oid = site_oid + "/queue"
+    site_oid = f"/{project}/admin/multisites/working_sites/{site}"
+    job_queue_oid = f"{site_oid}/queue/job_list"
+    sync_action_oid = f"/{project}/synchronization/synchronize_files"
 
     exchange_site = session.cmds.Flow.call(
         "/" + project, "get_exchange_site",
         args={}, kwargs={}
     )
     
     get_next_waiting_job = lambda qid: session.cmds.Flow.call(
         qid, "get_next_waiting_job", args={}, kwargs={}
     )
     synchronize_job = lambda job: session.cmds.Flow.call(
-        sync_action, "_process", args={job}, kwargs={}
+        sync_action_oid, "process", args={job}, kwargs={}
     )
     set_revision_sync_status = lambda oid, status, site_name=None: session.cmds.Flow.call(
         oid, "set_sync_status", args={status}, kwargs=dict(site_name=site_name)
     )
     touch = lambda oid: session.cmds.Flow.call(
         oid, "touch", args={}, kwargs={}
     )
 
     while (True):
-        job = get_next_waiting_job(job_queue_oid)
+        try:
+            job = get_next_waiting_job(job_queue_oid)
+            if job is not None:
+                synchronize_job(job)
+            if job is None or job.status.get() != "PROCESSED":
+                time.sleep(1)
+                continue
 
-        if job:
-            synchronize_job(job)
-        
-        time.sleep(1)
-
-        if job and job.status.get() == "PROCESSED":
             if job.type.get() == "Download":
                 set_revision_sync_status(job.emitter_oid.get(), "Available")
             elif job.type.get() == "Upload":
                 set_revision_sync_status(job.emitter_oid.get(), "Available", exchange_site.name())
-            
-            touch(session.cmds.Flow.resolve_path(job.emitter_oid.get() + "/.."))
+            touch(session.cmds.Flow.resolve_path(job.emitter_oid.get() + "/..")) # update revision map
+            touch(session.cmds.Flow.resolve_path(sync_action_oid + "/..")) # update synchronization
+        except (Exception, KeyboardInterrupt) as e:
+            if isinstance(e, KeyboardInterrupt):
+                print("Synchronization stopped")
+                break
+            else:
+                print("The following error occurred:")
+                print(traceback.format_exc())
+                print("Restart synchronization...")
 
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `libreflow-2.3.1/src/libreflow/sync_jobs_cleaner.py` & `libreflow-2.3.2/src/libreflow/sync_jobs_cleaner.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/flow/action_values.py` & `libreflow-2.3.2/src/libreflow/utils/flow/action_values.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/flow/context_values.py` & `libreflow-2.3.2/src/libreflow/utils/flow/context_values.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/flow/entities.py` & `libreflow-2.3.2/src/libreflow/utils/flow/entities.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/flow/file_processing.py` & `libreflow-2.3.2/src/libreflow/utils/flow/file_processing.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/flow/import_files.py` & `libreflow-2.3.2/src/libreflow/utils/flow/import_files.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/flow/process_files.py` & `libreflow-2.3.2/src/libreflow/utils/flow/process_files.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/flow/values.py` & `libreflow-2.3.2/src/libreflow/utils/flow/values.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/flow_entities/entities.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/flow_entities/entities.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/demo_flow.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/demo_flow.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/jobs_actor.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/jobs_actor.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/jobs_flow.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/jobs_flow.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/jobs_flow_worker.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/jobs_flow_worker.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/jobs_node.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/jobs_node.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/jobs/jobs_view.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/jobs/jobs_view.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/actor/__init__.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/flow/__init__.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/runner_factory.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/runner_factory.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/subprocess_manager/views/subprocess_view.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/subprocess_manager/views/subprocess_view.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/ui/flow_view.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/ui/flow_view.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/ui/main_window.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/ui/main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     
     def uninstall_tools(self):
         # FIXME: shouldn't a Hide be enough?
         self.btn_view_menu.setMenu(None)
     
     def on_view_title_change(self):
         self.title.setText(self.view.view_title())
+        self.dock.setWindowTitle(self.view.view_title())
     
     def on_floating(self, b):
         if b:
             self.dock.setTitleBarWidget(None)
             self.uninstall_tools()
         else:
             self.dock.setTitleBarWidget(self)
```

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/ui/navigation_control.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/ui/navigation_control.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/kabaret/ui/widget_view.py` & `libreflow-2.3.2/src/libreflow/utils/kabaret/ui/widget_view.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/os.py` & `libreflow-2.3.2/src/libreflow/utils/os.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/actor.py` & `libreflow-2.3.2/src/libreflow/utils/search/actor.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/data/icons/export.png` & `libreflow-2.3.2/src/libreflow/utils/search/data/icons/export.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/data/icons/filter-disabled.png` & `libreflow-2.3.2/src/libreflow/utils/search/data/icons/filter-disabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/data/icons/filter-enabled.png` & `libreflow-2.3.2/src/libreflow/utils/search/data/icons/filter-enabled.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/data/icons/import.png` & `libreflow-2.3.2/src/libreflow/utils/search/data/icons/import.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/data/icons/magn-glass.png` & `libreflow-2.3.2/src/libreflow/utils/search/data/icons/magn-glass.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/data/icons/minus-button.png` & `libreflow-2.3.2/src/libreflow/utils/search/data/icons/minus-button.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/data/icons/plus-button.png` & `libreflow-2.3.2/src/libreflow/utils/search/data/icons/plus-button.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/data/icons/remove.png` & `libreflow-2.3.2/src/libreflow/utils/search/data/icons/remove.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/data/icons/run-button.png` & `libreflow-2.3.2/src/libreflow/utils/search/data/icons/run-button.png`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/search/view.py` & `libreflow-2.3.2/src/libreflow/utils/search/view.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow/utils/ui/file_processing.py` & `libreflow-2.3.2/src/libreflow/utils/ui/file_processing.py`

 * *Files identical despite different names*

### Comparing `libreflow-2.3.1/src/libreflow.egg-info/PKG-INFO` & `libreflow-2.3.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: libreflow
-Version: 2.3.1
-Summary: An example flow for kabaret
-Home-page: https://gitlab.com/lfs.coop/libreflow
-Author: Flavio Perez
-Author-email: flavio@lfs.coop
-License: LGPLv3+
-Keywords: kabaret cgwire kitsu gazu animation pipeline libreflow
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-Requires-Dist: kabaret>=2.2.0rc6
-Requires-Dist: pyside2~=5.0
-Requires-Dist: six~=1.0
-Requires-Dist: kabaret.script-view
-Requires-Dist: kabaret.subprocess-manager
-Requires-Dist: kabaret.flow-contextaul-dict
-Requires-Dist: kabaret.flow-entities
-Requires-Dist: gazu>=0.8.33
-Requires-Dist: minio
-Requires-Dist: timeago
-Requires-Dist: blender-asset-tracer
-Requires-Dist: psutil
-Requires-Dist: fileseq
-Requires-Dist: sentry-sdk
-
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)[^1].
 
@@ -47,14 +15,45 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [2.3.2] - 2024-04-26
+
+### Added
+
+* Kitsu (Gazu) wrapper has a new method `get_project_type()` for retrieve project type (Short, TV Show etc.)
+* MXF and PRPROJ file formats support.
+* Premiere Pro added in runners list.
+* A parameter in default files to specify the target Kitsu task type. Only used for Kitsu uploadable files.
+
+### Changed
+
+* Users list now sorted alphabetically (by user ID) by default.
+* Default Tasks in Task Manager are now sorted by task position number.
+* Improved log messages for Create Task Default Files and Kitsu Tasks actions.
+
+### Fixed
+
+* Kitsu episodes is now handled in `get_entity_data()` of Kitsu (Gazu) wrapper.
+  * Caused problems when trying to retrieve kitsu entity of a shot when project is a TV Show.
+* File and revision paths are now normalised to avoid opening issues with differents slashes.
+* Task Template now has a function to get path format and fixes the action for creating files in a task template.
+* Import Files action: typo on `Resolving files` popup.
+* User tasks: the display of a file entry's action menu when the file is right-clicked and its secondary action button is clicked.
+* User tasks: dragging a file out of the UI.
+* User tasks: focus detection for keyboard shortcuts when using multiple views in the window
+* View title is updated again when current oid is changed. Fixed confusion when multiple views were docked.
+* View width is no longer expanded if the current oid is on a custom UI page and there are multiple views.
+* Fixed *Create default files* task action when a file is incremented from its base file.
+* Lock a synchronization job starting to be processed by setting its status to `PROCESSING` (avoids multiples processing of the same job from different sessions).
+* Synchronization session: rectified deprecated OIDs and automatic relaunch when an error occurs.
+
 ## [2.3.1] - 2024-03-14
 
 ### Added
 
 * New parameters `width` and `height` in the project settings. These are available in the project default contextual dict.
 * New task icons to display in a shot or asset task list.
   * If a color is defined in a task, the new icon will match it, maintaining its brightness and saturation.
@@ -78,15 +77,14 @@
 * Color of file actions error messages has been adapted to LFS style class color scheme.
 * Value of the *Upload after publish* is not stored anymore in the action value store. It only depends on the *auto upload* project setting.
 * Logging level of the session worker (INFO).
 
 ### Fixed
 
 * Create Kitsu Tasks action: switch to case insensitive for check task templates names.
-* Import Files action: typo on `Resolving files` popup.
 * The `TaskManager.get_task_files()` method now returns enabled only files when corresponding attribute is used.
 * Create default files:
   * `NoneType` error when a default file was created from a base file which has no revision or whose latest revision wasn't available.
   * A default file is now not create by default, when it already exists and use base file mode is enabled.
     * The user can still manually choose to create the revision from base file. This is to avoid issues when action is used in a batch way.
 * User Tasks: 
   * Libreflow bookmarks no longer break the interface
@@ -1482,8 +1480,8 @@
 Initial public commit and pypi setup. This version is an early version of libreflow. It includes a baseflow and examples flows overriding the baseflow. We have been working on departments, files, file version history, and stuff like that.
 
 ### Fixed
 
 issue #6 : Pip Package is now ready for use
 
 
-[^1]: Except we started libreflow MAJOR version number at 1, as we consider our in-house previous flow being version 0.
+[^1]: Except we started libreflow MAJOR version number at 1, as we consider our in-house previous flow being version 0.
```

### Comparing `libreflow-2.3.1/src/libreflow.egg-info/SOURCES.txt` & `libreflow-2.3.2/src/libreflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -77,23 +77,28 @@
 src/libreflow/resources/file_templates/template.abc
 src/libreflow/resources/file_templates/template.aep
 src/libreflow/resources/file_templates/template.ai
 src/libreflow/resources/file_templates/template.blend
 src/libreflow/resources/file_templates/template.fbx
 src/libreflow/resources/file_templates/template.jpg
 src/libreflow/resources/file_templates/template.json
+src/libreflow/resources/file_templates/template.jsx
 src/libreflow/resources/file_templates/template.kra
 src/libreflow/resources/file_templates/template.mov
+src/libreflow/resources/file_templates/template.mp4
+src/libreflow/resources/file_templates/template.nk
 src/libreflow/resources/file_templates/template.obj
 src/libreflow/resources/file_templates/template.png
 src/libreflow/resources/file_templates/template.psb
 src/libreflow/resources/file_templates/template.psd
 src/libreflow/resources/file_templates/template.txt
 src/libreflow/resources/file_templates/template.usd
 src/libreflow/resources/file_templates/template.wav
+src/libreflow/resources/fonts/SpaceGrotesk-Bold.ttf
+src/libreflow/resources/fonts/SpaceGrotesk-Regular.ttf
 src/libreflow/resources/fonts/__init__.py
 src/libreflow/resources/icons/__init__.py
 src/libreflow/resources/icons/applications/__init__.py
 src/libreflow/resources/icons/applications/rv.png
 src/libreflow/resources/icons/flow/__init__.py
 src/libreflow/resources/icons/flow/alembic.png
 src/libreflow/resources/icons/flow/explorer.png
@@ -189,14 +194,15 @@
 src/libreflow/resources/icons/libreflow/log_out.png
 src/libreflow/resources/icons/libreflow/multi-share-option.png
 src/libreflow/resources/icons/libreflow/nuke.png
 src/libreflow/resources/icons/libreflow/origin-site.png
 src/libreflow/resources/icons/libreflow/padlock.png
 src/libreflow/resources/icons/libreflow/padlock_green.png
 src/libreflow/resources/icons/libreflow/padlock_red.png
+src/libreflow/resources/icons/libreflow/premiere-pro.png
 src/libreflow/resources/icons/libreflow/publish-ae.png
 src/libreflow/resources/icons/libreflow/publish-blender.png
 src/libreflow/resources/icons/libreflow/publish.png
 src/libreflow/resources/icons/libreflow/quicktime.png
 src/libreflow/resources/icons/libreflow/refresh.png
 src/libreflow/resources/icons/libreflow/request.png
 src/libreflow/resources/icons/libreflow/requestable.png
@@ -234,14 +240,15 @@
 src/libreflow/resources/icons/tasks/lighting.svg
 src/libreflow/resources/icons/tasks/modeling.svg
 src/libreflow/resources/icons/tasks/rigging.svg
 src/libreflow/resources/icons/tasks/shading.svg
 src/libreflow/resources/mark_sequence/__init__.py
 src/libreflow/resources/mark_sequence/fields/__init__.py
 src/libreflow/resources/mark_sequence/fields/default.json
+src/libreflow/resources/mark_sequence/fonts/LiberationMono-Regular.ttf
 src/libreflow/resources/mark_sequence/fonts/__init__.py
 src/libreflow/resources/scripts/__init__.py
 src/libreflow/resources/scripts/blender/__init__.py
 src/libreflow/resources/scripts/blender/disable_save_keymap.py
 src/libreflow/resources/styles/__init__.py
 src/libreflow/resources/styles/lfs_tech/__init__.py
 src/libreflow/resources/styles/lfs_tech/lfs_tech_style.css
```

### Comparing `libreflow-2.3.1/versioneer.py` & `libreflow-2.3.2/versioneer.py`

 * *Files identical despite different names*

