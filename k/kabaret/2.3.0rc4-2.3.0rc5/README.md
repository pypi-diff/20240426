# Comparing `tmp/kabaret-2.3.0rc4.tar.gz` & `tmp/kabaret-2.3.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kabaret-2.3.0rc4.tar", last modified: Wed Jan 31 16:58:53 2024, max compression
+gzip compressed data, was "kabaret-2.3.0rc5.tar", last modified: Fri Apr 26 12:18:36 2024, max compression
```

## Comparing `kabaret-2.3.0rc4.tar` & `kabaret-2.3.0rc5.tar`

### file list

```diff
@@ -1,306 +1,306 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.424527 kabaret-2.3.0rc4/
--rw-rw-rw-   0 root         (0) root         (0)      358 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    12425 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13938 2024-01-31 16:58:53.423527 kabaret-2.3.0rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      333 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     7650 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/lgpl-3.0.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.362527 kabaret-2.3.0rc4/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.367527 kabaret-2.3.0rc4/python/dev_studio/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 16:58:44.000000 kabaret-2.3.0rc4/python/dev_studio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.367527 kabaret-2.3.0rc4/python/dev_studio/flow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 16:58:44.000000 kabaret-2.3.0rc4/python/dev_studio/flow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.367527 kabaret-2.3.0rc4/python/dev_studio/flow/custom_home/
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/custom_home/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.367527 kabaret-2.3.0rc4/python/dev_studio/flow/demo_project/
--rw-rw-rw-   0 root         (0) root         (0)    16229 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/demo_project/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.368527 kabaret-2.3.0rc4/python/dev_studio/flow/demo_project/maya_startup/
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/demo_project/maya_startup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1911 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/demo_project/maya_startup/userSetup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.368527 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.368527 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/icon_browser/
--rw-rw-rw-   0 root         (0) root         (0)     3055 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/icon_browser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.371527 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/
--rw-rw-rw-   0 root         (0) root         (0)      280 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4357 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/action_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4858 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/action_dialog_size.py
--rw-rw-rw-   0 root         (0) root         (0)     2671 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/action_submenus_demo.py
--rw-rw-rw-   0 root         (0) root         (0)    11520 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     5468 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/custom_page.py
--rw-rw-rw-   0 root         (0) root         (0)    11276 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/editors.py
--rw-rw-rw-   0 root         (0) root         (0)    11533 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/injection.py
--rw-rw-rw-   0 root         (0) root         (0)     2427 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/map_as_view.py
--rw-rw-rw-   0 root         (0) root         (0)    10468 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/maps.py
--rw-rw-rw-   0 root         (0) root         (0)     1959 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/other.py
--rw-rw-rw-   0 root         (0) root         (0)     5749 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/relations.py
--rw-rw-rw-   0 root         (0) root         (0)     6317 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/ui_config.py
--rw-rw-rw-   0 root         (0) root         (0)     5299 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/values.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.371527 kabaret-2.3.0rc4/python/dev_studio/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 16:58:44.000000 kabaret-2.3.0rc4/python/dev_studio/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.372527 kabaret-2.3.0rc4/python/dev_studio/icons/flow/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/icons/flow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.372527 kabaret-2.3.0rc4/python/dev_studio/icons/gui/
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/icons/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6462 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/dev_studio/icons/gui/kabaret_icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.424527 kabaret-2.3.0rc4/python/kabaret/
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/__init__.py
--rw-r--r--   0 root         (0) root         (0)      500 2024-01-31 16:58:53.424527 kabaret-2.3.0rc4/python/kabaret/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.375527 kabaret-2.3.0rc4/python/kabaret/app/
--rw-rw-rw-   0 root         (0) root         (0)     1368 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2044 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/_actor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.375527 kabaret-2.3.0rc4/python/kabaret/app/actors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 16:58:44.000000 kabaret-2.3.0rc4/python/kabaret/app/actors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9343 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/actors/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/actors/default_actors_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.376527 kabaret-2.3.0rc4/python/kabaret/app/actors/flow/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/actors/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39838 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/actors/flow/actor.py
--rw-rw-rw-   0 root         (0) root         (0)     5938 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/actors/flow/generic_home_flow.py
--rw-rw-rw-   0 root         (0) root         (0)     1778 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/actors/flow/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4572 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/actors/flow/value_store.py
--rw-rw-rw-   0 root         (0) root         (0)     2969 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/plugin_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/resources.py
--rw-rw-rw-   0 root         (0) root         (0)    24780 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.377527 kabaret-2.3.0rc4/python/kabaret/app/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 16:58:44.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.377527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2179 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/embedded.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.377527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 16:58:44.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.389527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/3dsmax.png
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/action.png
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/afterfx.png
--rw-rw-rw-   0 root         (0) root         (0)     3435 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/alembic.png
--rw-rw-rw-   0 root         (0) root         (0)     3237 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/asset.png
--rw-rw-rw-   0 root         (0) root         (0)     3409 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/asset_family.png
--rw-rw-rw-   0 root         (0) root         (0)     3284 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/bank.png
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/branch-end.png
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/branch-more.png
--rw-rw-rw-   0 root         (0) root         (0)      783 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/branch.png
--rw-rw-rw-   0 root         (0) root         (0)     3245 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/casting.png
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/collapsed.png
--rw-rw-rw-   0 root         (0) root         (0)     3109 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/editor_proc.png
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/expanded.png
--rw-rw-rw-   0 root         (0) root         (0)     3407 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/explorer.png
--rw-rw-rw-   0 root         (0) root         (0)     3058 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/file.png
--rw-rw-rw-   0 root         (0) root         (0)     3056 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/film.png
--rw-rw-rw-   0 root         (0) root         (0)     3353 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/folder.png
--rw-rw-rw-   0 root         (0) root         (0)     3205 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/goto.png
--rw-rw-rw-   0 root         (0) root         (0)     4080 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/guerilla.png
--rw-rw-rw-   0 root         (0) root         (0)      710 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/hannah.png
--rw-rw-rw-   0 root         (0) root         (0)     3461 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/houdini.png
--rw-rw-rw-   0 root         (0) root         (0)     3141 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/input.png
--rw-rw-rw-   0 root         (0) root         (0)     3242 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/job.png
--rw-rw-rw-   0 root         (0) root         (0)     1411 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/jobs.png
--rw-rw-rw-   0 root         (0) root         (0)     3348 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/jump_to.png
--rw-rw-rw-   0 root         (0) root         (0)     7894 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/lightroom_xmp.png
--rw-rw-rw-   0 root         (0) root         (0)     3741 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/maya.png
--rw-rw-rw-   0 root         (0) root         (0)     1673 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/maya_tools.png
--rw-rw-rw-   0 root         (0) root         (0)     3602 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/mayapy.png
--rw-rw-rw-   0 root         (0) root         (0)     4978 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/mrviewer.png
--rw-rw-rw-   0 root         (0) root         (0)      763 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/muster8.png
--rw-rw-rw-   0 root         (0) root         (0)     4706 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/natron.png
--rw-rw-rw-   0 root         (0) root         (0)     3233 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/node.png
--rw-rw-rw-   0 root         (0) root         (0)     3170 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/note.png
--rw-rw-rw-   0 root         (0) root         (0)     3379 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/notepad.png
--rw-rw-rw-   0 root         (0) root         (0)     3323 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/notethread.png
--rw-rw-rw-   0 root         (0) root         (0)     3389 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/nuke.png
--rw-rw-rw-   0 root         (0) root         (0)     3577 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/nuke10.png
--rw-rw-rw-   0 root         (0) root         (0)     3111 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/object.png
--rw-rw-rw-   0 root         (0) root         (0)     3111 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/output.png
--rw-rw-rw-   0 root         (0) root         (0)     3132 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/parent.png
--rw-rw-rw-   0 root         (0) root         (0)      765 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/pdplayer.png
--rw-rw-rw-   0 root         (0) root         (0)     5032 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/photoshop.png
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/python.png
--rw-rw-rw-   0 root         (0) root         (0)     3679 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/quicktime.png
--rw-rw-rw-   0 root         (0) root         (0)     3205 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/ref.png
--rw-rw-rw-   0 root         (0) root         (0)     3522 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/resolve.png
--rw-rw-rw-   0 root         (0) root         (0)     3322 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/scheduled.png
--rw-rw-rw-   0 root         (0) root         (0)     3226 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/sequence.png
--rw-rw-rw-   0 root         (0) root         (0)     3121 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/shot.png
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/slop.png
--rw-rw-rw-   0 root         (0) root         (0)     5674 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/smedge.png
--rw-rw-rw-   0 root         (0) root         (0)     3105 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/speedgrade.png
--rw-rw-rw-   0 root         (0) root         (0)     3180 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/task.png
--rw-rw-rw-   0 root         (0) root         (0)     3141 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/value.png
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/vrak.png
--rw-rw-rw-   0 root         (0) root         (0)     3283 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/workstation.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.409527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2974 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/bookmark-black-shape.png
--rw-rw-rw-   0 root         (0) root         (0)     2983 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/check-box-empty.png
--rw-rw-rw-   0 root         (0) root         (0)     3217 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/check-mark.png
--rw-rw-rw-   0 root         (0) root         (0)     3285 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/check.png
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/checked-white.png
--rw-rw-rw-   0 root         (0) root         (0)     3938 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-down-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)     3139 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-down.png
--rw-rw-rw-   0 root         (0) root         (0)     3750 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-left-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)     3057 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-left.png
--rw-rw-rw-   0 root         (0) root         (0)     3773 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-to-right-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)     3062 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-to-right.png
--rw-rw-rw-   0 root         (0) root         (0)     3932 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-up-disabled.png
--rw-rw-rw-   0 root         (0) root         (0)     3112 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-up.png
--rw-rw-rw-   0 root         (0) root         (0)     3107 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/circle-shape-outline.png
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/cog-wheel-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     3239 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/copy-document.png
--rw-rw-rw-   0 root         (0) root         (0)     3084 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/correct-symbol.png
--rw-rw-rw-   0 root         (0) root         (0)     3082 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/cross-mark-on-a-black-circle-background.png
--rw-rw-rw-   0 root         (0) root         (0)    10274 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/dice.png
--rw-rw-rw-   0 root         (0) root         (0)    11336 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/dice_3d.png
--rw-rw-rw-   0 root         (0) root         (0)     3165 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/exclamation-sign.png
--rw-rw-rw-   0 root         (0) root         (0)     3002 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/file.png
--rw-rw-rw-   0 root         (0) root         (0)     3165 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/film-strip-with-two-photograms.png
--rw-rw-rw-   0 root         (0) root         (0)     2977 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/filter-tool-black-shape.png
--rw-rw-rw-   0 root         (0) root         (0)     2981 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/folder-closed-black-shape.png
--rw-rw-rw-   0 root         (0) root         (0)     3084 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/folder-white-shape.png
--rw-rw-rw-   0 root         (0) root         (0)     3323 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/group-profile-users.png
--rw-rw-rw-   0 root         (0) root         (0)     3322 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/heart-shape-outline.png
--rw-rw-rw-   0 root         (0) root         (0)     3138 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/heart-shape-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     1272 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/home-outline.png
--rw-rw-rw-   0 root         (0) root         (0)     3215 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/home.png
--rw-rw-rw-   0 root         (0) root         (0)     3152 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/italicize-text.png
--rw-rw-rw-   0 root         (0) root         (0)     6234 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/kabaret_icon.png
--rw-rw-rw-   0 root         (0) root         (0)   341293 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/kabaret_logo.gif
--rw-rw-rw-   0 root         (0) root         (0)     4960 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/kabaret_logo_vector.svg
--rw-rw-rw-   0 root         (0) root         (0)     3141 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/man.png
--rw-rw-rw-   0 root         (0) root         (0)      703 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/maximize.png
--rw-rw-rw-   0 root         (0) root         (0)      720 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/minimize.png
--rw-rw-rw-   0 root         (0) root         (0)     3021 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/minus-button.png
--rw-rw-rw-   0 root         (0) root         (0)     3201 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/open-folder-outline.png
--rw-rw-rw-   0 root         (0) root         (0)     3104 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/open-folder.png
--rw-rw-rw-   0 root         (0) root         (0)     3058 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/open-laptop-computer.png
--rw-rw-rw-   0 root         (0) root         (0)     3109 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/open-padlock-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     3117 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/padlock.png
--rw-rw-rw-   0 root         (0) root         (0)     3120 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/paste-from-clipboard.png
--rw-rw-rw-   0 root         (0) root         (0)     3130 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/picture.png
--rw-rw-rw-   0 root         (0) root         (0)     2935 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/plus-black-symbol.png
--rw-rw-rw-   0 root         (0) root         (0)     3107 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/plus-sign-in-a-black-circle.png
--rw-rw-rw-   0 root         (0) root         (0)     2998 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/plus-symbol-in-a-rounded-black-square.png
--rw-rw-rw-   0 root         (0) root         (0)    10876 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/power_button.png
--rw-rw-rw-   0 root         (0) root         (0)    10903 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/power_button_2.png
--rw-rw-rw-   0 root         (0) root         (0)     3170 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/remove-button.png
--rw-rw-rw-   0 root         (0) root         (0)     3000 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/remove-symbol.png
--rw-rw-rw-   0 root         (0) root         (0)     3320 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/search.png
--rw-rw-rw-   0 root         (0) root         (0)     3459 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/settings.png
--rw-rw-rw-   0 root         (0) root         (0)     3169 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/share-option.png
--rw-rw-rw-   0 root         (0) root         (0)     3140 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/share-post-symbol.png
--rw-rw-rw-   0 root         (0) root         (0)     3339 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/share-symbol.png
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/sitemap.png
--rw-rw-rw-   0 root         (0) root         (0)     3010 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/sort-arrows-couple-pointing-up-and-down.png
--rw-rw-rw-   0 root         (0) root         (0)     2944 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/sort-down.png
--rw-rw-rw-   0 root         (0) root         (0)     2920 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/sort-up.png
--rw-rw-rw-   0 root         (0) root         (0)     3266 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/speech-bubbles-comment-option.png
--rw-rw-rw-   0 root         (0) root         (0)     3339 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/star-1.png
--rw-rw-rw-   0 root         (0) root         (0)     3279 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/star-half-empty.png
--rw-rw-rw-   0 root         (0) root         (0)     3138 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/star.png
--rw-rw-rw-   0 root         (0) root         (0)     3109 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/submenu.png
--rw-rw-rw-   0 root         (0) root         (0)     3342 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/sun.png
--rw-rw-rw-   0 root         (0) root         (0)    10543 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/switch.png
--rw-rw-rw-   0 root         (0) root         (0)    10895 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/switch_arrow.png
--rw-rw-rw-   0 root         (0) root         (0)    10905 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/switch_binary.png
--rw-rw-rw-   0 root         (0) root         (0)     3088 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/tag-black-shape.png
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/tags.png
--rw-rw-rw-   0 root         (0) root         (0)     3416 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/team-admin.png
--rw-rw-rw-   0 root         (0) root         (0)     3513 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/team-lead.png
--rw-rw-rw-   0 root         (0) root         (0)     3323 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/team.png
--rw-rw-rw-   0 root         (0) root         (0)     3082 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/text-file-1.png
--rw-rw-rw-   0 root         (0) root         (0)     3139 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/text-file.png
--rw-rw-rw-   0 root         (0) root         (0)      340 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/ui-layout.png
--rw-rw-rw-   0 root         (0) root         (0)    13060 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/undefined.png
--rw-rw-rw-   0 root         (0) root         (0)     3215 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/user-admin.png
--rw-rw-rw-   0 root         (0) root         (0)     3324 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/user-lead.png
--rw-rw-rw-   0 root         (0) root         (0)     3378 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/user-md-symbol.png
--rw-rw-rw-   0 root         (0) root         (0)     3127 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/user-shape.png
--rw-rw-rw-   0 root         (0) root         (0)     3127 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/user.png
--rw-rw-rw-   0 root         (0) root         (0)     3124 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/users.png
--rw-rw-rw-   0 root         (0) root         (0)     6941 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/wheel_throbber.gif
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/youtube-logo.png
--rw-rw-rw-   0 root         (0) root         (0)     3391 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/zoom-in.png
--rw-rw-rw-   0 root         (0) root         (0)     3338 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/zoom-out.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.412527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/DONE.png
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/ERR.png
--rw-rw-rw-   0 root         (0) root         (0)     3014 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/INV.png
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/NONE.png
--rw-rw-rw-   0 root         (0) root         (0)     2999 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/NYS.png
--rw-rw-rw-   0 root         (0) root         (0)     3130 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/OOP.png
--rw-rw-rw-   0 root         (0) root         (0)     3112 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/RTK.png
--rw-rw-rw-   0 root         (0) root         (0)     3113 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/RVW.png
--rw-rw-rw-   0 root         (0) root         (0)     3212 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/WAIT.png
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/WARN.png
--rw-rw-rw-   0 root         (0) root         (0)     3218 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/WIP.png
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3806 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/standalone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.412527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/
--rw-rw-rw-   0 root         (0) root         (0)     2640 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.412527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/dark/
--rw-rw-rw-   0 root         (0) root         (0)     4601 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/dark/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14339 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/dark/dark_style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.413527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/gray/
--rw-rw-rw-   0 root         (0) root         (0)     2551 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/gray/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7679 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/gray/gray_style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.413527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/neonative/
--rw-rw-rw-   0 root         (0) root         (0)      564 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/neonative/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12549 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/neonative/neonative_style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.415527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-31 16:58:44.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.418527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/
--rw-rw-rw-   0 root         (0) root         (0)     2171 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3632 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/bool_value.py
--rw-rw-rw-   0 root         (0) root         (0)     4292 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/choice_value.py
--rw-rw-rw-   0 root         (0) root         (0)    69953 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/default_thumbnail.py
--rw-rw-rw-   0 root         (0) root         (0)    10405 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/image_value.py
--rw-rw-rw-   0 root         (0) root         (0)     5839 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/interface.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/label.py
--rw-rw-rw-   0 root         (0) root         (0)     7293 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/multichoice_value.py
--rw-rw-rw-   0 root         (0) root         (0)      781 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/password_value.py
--rw-rw-rw-   0 root         (0) root         (0)    12187 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/path_value.py
--rw-rw-rw-   0 root         (0) root         (0)     3060 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/percent_value.py
--rw-rw-rw-   0 root         (0) root         (0)     3951 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/python_value.py
--rw-rw-rw-   0 root         (0) root         (0)     6651 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/textarea.py
--rw-rw-rw-   0 root         (0) root         (0)     9715 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/thumbnail.py
--rw-rw-rw-   0 root         (0) root         (0)     5717 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/time_value.py
--rw-rw-rw-   0 root         (0) root         (0)     4060 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/event_filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.421527 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/flow_editors.py
--rw-rw-rw-   0 root         (0) root         (0)    12229 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/flow_field.py
--rw-rw-rw-   0 root         (0) root         (0)    32692 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/flow_form.py
--rw-rw-rw-   0 root         (0) root         (0)    21502 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/flow_view.py
--rw-rw-rw-   0 root         (0) root         (0)    18977 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/map_field.py
--rw-rw-rw-   0 root         (0) root         (0)     9352 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/navigation_control.py
--rw-rw-rw-   0 root         (0) root         (0)     3987 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/navigator.py
--rw-rw-rw-   0 root         (0) root         (0)     5973 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/ref_by.py
--rw-rw-rw-   0 root         (0) root         (0)     2927 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/script_line.py
--rw-rw-rw-   0 root         (0) root         (0)     2784 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow_layout.py
--rw-rw-rw-   0 root         (0) root         (0)     9397 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/form_tree.py
--rw-rw-rw-   0 root         (0) root         (0)    10797 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/main_window.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/popup_menu.py
--rw-rw-rw-   0 root         (0) root         (0)     4573 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/session_toolbar.py
--rw-rw-rw-   0 root         (0) root         (0)    14129 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/widget_view.py
--rw-rw-rw-   0 root         (0) root         (0)     2759 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/app/ui/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.423527 kabaret-2.3.0rc4/python/kabaret/flow/
--rw-rw-rw-   0 root         (0) root         (0)     4021 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/flow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6698 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/flow/action.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/flow/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7540 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/flow/injection.py
--rw-rw-rw-   0 root         (0) root         (0)    33049 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/flow/map.py
--rw-rw-rw-   0 root         (0) root         (0)    31344 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/flow/object.py
--rw-rw-rw-   0 root         (0) root         (0)    14403 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/flow/relations.py
--rw-rw-rw-   0 root         (0) root         (0)     6598 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/flow/value_store.py
--rw-rw-rw-   0 root         (0) root         (0)    15531 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/python/kabaret/flow/values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:58:53.423527 kabaret-2.3.0rc4/python/kabaret.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13938 2024-01-31 16:58:53.000000 kabaret-2.3.0rc4/python/kabaret.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13413 2024-01-31 16:58:53.000000 kabaret-2.3.0rc4/python/kabaret.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 16:58:53.000000 kabaret-2.3.0rc4/python/kabaret.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-01-31 16:58:53.000000 kabaret-2.3.0rc4/python/kabaret.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-01-31 16:58:53.000000 kabaret-2.3.0rc4/python/kabaret.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-01-31 16:58:53.424527 kabaret-2.3.0rc4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2158 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2024-01-31 16:58:43.000000 kabaret-2.3.0rc4/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.207012 kabaret-2.3.0rc5/
+-rw-rw-rw-   0 root         (0) root         (0)      358 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    13304 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14817 2024-04-26 12:18:36.207012 kabaret-2.3.0rc5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      333 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7650 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/lgpl-3.0.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.147013 kabaret-2.3.0rc5/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.151013 kabaret-2.3.0rc5/python/dev_studio/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.151013 kabaret-2.3.0rc5/python/dev_studio/flow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.152013 kabaret-2.3.0rc5/python/dev_studio/flow/custom_home/
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/custom_home/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.152013 kabaret-2.3.0rc5/python/dev_studio/flow/demo_project/
+-rw-rw-rw-   0 root         (0) root         (0)    16229 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/demo_project/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.152013 kabaret-2.3.0rc5/python/dev_studio/flow/demo_project/maya_startup/
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/demo_project/maya_startup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/demo_project/maya_startup/userSetup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.152013 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.153013 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/icon_browser/
+-rw-rw-rw-   0 root         (0) root         (0)     3055 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/icon_browser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.156013 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4357 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/action_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4858 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/action_dialog_size.py
+-rw-rw-rw-   0 root         (0) root         (0)     2671 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/action_submenus_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)    11520 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/custom_page.py
+-rw-rw-rw-   0 root         (0) root         (0)    11276 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/editors.py
+-rw-rw-rw-   0 root         (0) root         (0)    11533 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/injection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2427 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/map_as_view.py
+-rw-rw-rw-   0 root         (0) root         (0)    10468 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1959 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/other.py
+-rw-rw-rw-   0 root         (0) root         (0)     5749 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/relations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6317 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/ui_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5299 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/values.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.156013 kabaret-2.3.0rc5/python/dev_studio/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.156013 kabaret-2.3.0rc5/python/dev_studio/icons/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/icons/flow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.157013 kabaret-2.3.0rc5/python/dev_studio/icons/gui/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/icons/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/dev_studio/icons/gui/kabaret_icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.208011 kabaret-2.3.0rc5/python/kabaret/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      500 2024-04-26 12:18:36.208011 kabaret-2.3.0rc5/python/kabaret/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.159013 kabaret-2.3.0rc5/python/kabaret/app/
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/_actor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.160013 kabaret-2.3.0rc5/python/kabaret/app/actors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/actors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9343 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/actors/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/actors/default_actors_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.161013 kabaret-2.3.0rc5/python/kabaret/app/actors/flow/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/actors/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39838 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/actors/flow/actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5938 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/actors/flow/generic_home_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/actors/flow/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4572 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/actors/flow/value_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/plugin_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)    31765 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.161013 kabaret-2.3.0rc5/python/kabaret/app/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.162013 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2179 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/embedded.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.162013 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.174012 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/3dsmax.png
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/action.png
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/afterfx.png
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/alembic.png
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/asset.png
+-rw-rw-rw-   0 root         (0) root         (0)     3409 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/asset_family.png
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/bank.png
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/branch-end.png
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/branch-more.png
+-rw-rw-rw-   0 root         (0) root         (0)      783 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/branch.png
+-rw-rw-rw-   0 root         (0) root         (0)     3245 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/casting.png
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/collapsed.png
+-rw-rw-rw-   0 root         (0) root         (0)     3109 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/editor_proc.png
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/expanded.png
+-rw-rw-rw-   0 root         (0) root         (0)     3407 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/explorer.png
+-rw-rw-rw-   0 root         (0) root         (0)     3058 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/file.png
+-rw-rw-rw-   0 root         (0) root         (0)     3056 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/film.png
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/folder.png
+-rw-rw-rw-   0 root         (0) root         (0)     3205 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/goto.png
+-rw-rw-rw-   0 root         (0) root         (0)     4080 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/guerilla.png
+-rw-rw-rw-   0 root         (0) root         (0)      710 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/hannah.png
+-rw-rw-rw-   0 root         (0) root         (0)     3461 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/houdini.png
+-rw-rw-rw-   0 root         (0) root         (0)     3141 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/input.png
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/job.png
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/jobs.png
+-rw-rw-rw-   0 root         (0) root         (0)     3348 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/jump_to.png
+-rw-rw-rw-   0 root         (0) root         (0)     7894 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/lightroom_xmp.png
+-rw-rw-rw-   0 root         (0) root         (0)     3741 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/maya.png
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/maya_tools.png
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/mayapy.png
+-rw-rw-rw-   0 root         (0) root         (0)     4978 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/mrviewer.png
+-rw-rw-rw-   0 root         (0) root         (0)      763 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/muster8.png
+-rw-rw-rw-   0 root         (0) root         (0)     4706 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/natron.png
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/node.png
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/note.png
+-rw-rw-rw-   0 root         (0) root         (0)     3379 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/notepad.png
+-rw-rw-rw-   0 root         (0) root         (0)     3323 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/notethread.png
+-rw-rw-rw-   0 root         (0) root         (0)     3389 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/nuke.png
+-rw-rw-rw-   0 root         (0) root         (0)     3577 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/nuke10.png
+-rw-rw-rw-   0 root         (0) root         (0)     3111 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/object.png
+-rw-rw-rw-   0 root         (0) root         (0)     3111 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/output.png
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/parent.png
+-rw-rw-rw-   0 root         (0) root         (0)      765 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/pdplayer.png
+-rw-rw-rw-   0 root         (0) root         (0)     5032 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/photoshop.png
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/python.png
+-rw-rw-rw-   0 root         (0) root         (0)     3679 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/quicktime.png
+-rw-rw-rw-   0 root         (0) root         (0)     3205 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/ref.png
+-rw-rw-rw-   0 root         (0) root         (0)     3522 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/resolve.png
+-rw-rw-rw-   0 root         (0) root         (0)     3322 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/scheduled.png
+-rw-rw-rw-   0 root         (0) root         (0)     3226 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/sequence.png
+-rw-rw-rw-   0 root         (0) root         (0)     3121 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/shot.png
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/slop.png
+-rw-rw-rw-   0 root         (0) root         (0)     5674 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/smedge.png
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/speedgrade.png
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/task.png
+-rw-rw-rw-   0 root         (0) root         (0)     3141 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/value.png
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/vrak.png
+-rw-rw-rw-   0 root         (0) root         (0)     3283 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/workstation.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.193012 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2974 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/bookmark-black-shape.png
+-rw-rw-rw-   0 root         (0) root         (0)     2983 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/check-box-empty.png
+-rw-rw-rw-   0 root         (0) root         (0)     3217 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/check-mark.png
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/check.png
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/checked-white.png
+-rw-rw-rw-   0 root         (0) root         (0)     3938 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-down-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)     3139 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-down.png
+-rw-rw-rw-   0 root         (0) root         (0)     3750 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-left-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-left.png
+-rw-rw-rw-   0 root         (0) root         (0)     3773 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-to-right-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)     3062 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-to-right.png
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-up-disabled.png
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-up.png
+-rw-rw-rw-   0 root         (0) root         (0)     3107 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/circle-shape-outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/cog-wheel-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/copy-document.png
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/correct-symbol.png
+-rw-rw-rw-   0 root         (0) root         (0)     3082 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/cross-mark-on-a-black-circle-background.png
+-rw-rw-rw-   0 root         (0) root         (0)    10274 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/dice.png
+-rw-rw-rw-   0 root         (0) root         (0)    11336 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/dice_3d.png
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/exclamation-sign.png
+-rw-rw-rw-   0 root         (0) root         (0)     3002 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/file.png
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/film-strip-with-two-photograms.png
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/filter-tool-black-shape.png
+-rw-rw-rw-   0 root         (0) root         (0)     2981 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/folder-closed-black-shape.png
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/folder-white-shape.png
+-rw-rw-rw-   0 root         (0) root         (0)     3323 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/group-profile-users.png
+-rw-rw-rw-   0 root         (0) root         (0)     3322 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/heart-shape-outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     3138 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/heart-shape-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/home-outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     3215 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/home.png
+-rw-rw-rw-   0 root         (0) root         (0)     3152 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/italicize-text.png
+-rw-rw-rw-   0 root         (0) root         (0)     6234 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/kabaret_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)   341293 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/kabaret_logo.gif
+-rw-rw-rw-   0 root         (0) root         (0)     4960 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/kabaret_logo_vector.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3141 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/man.png
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/maximize.png
+-rw-rw-rw-   0 root         (0) root         (0)      720 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/minimize.png
+-rw-rw-rw-   0 root         (0) root         (0)     3021 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/minus-button.png
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/open-folder-outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/open-folder.png
+-rw-rw-rw-   0 root         (0) root         (0)     3058 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/open-laptop-computer.png
+-rw-rw-rw-   0 root         (0) root         (0)     3109 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/open-padlock-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/padlock.png
+-rw-rw-rw-   0 root         (0) root         (0)     3120 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/paste-from-clipboard.png
+-rw-rw-rw-   0 root         (0) root         (0)     3130 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/picture.png
+-rw-rw-rw-   0 root         (0) root         (0)     2935 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/plus-black-symbol.png
+-rw-rw-rw-   0 root         (0) root         (0)     3107 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/plus-sign-in-a-black-circle.png
+-rw-rw-rw-   0 root         (0) root         (0)     2998 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/plus-symbol-in-a-rounded-black-square.png
+-rw-rw-rw-   0 root         (0) root         (0)    10876 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/power_button.png
+-rw-rw-rw-   0 root         (0) root         (0)    10903 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/power_button_2.png
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/remove-button.png
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/remove-symbol.png
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/search.png
+-rw-rw-rw-   0 root         (0) root         (0)     3459 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/settings.png
+-rw-rw-rw-   0 root         (0) root         (0)     3169 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/share-option.png
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/share-post-symbol.png
+-rw-rw-rw-   0 root         (0) root         (0)     3339 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/share-symbol.png
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/sitemap.png
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/sort-arrows-couple-pointing-up-and-down.png
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/sort-down.png
+-rw-rw-rw-   0 root         (0) root         (0)     2920 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/sort-up.png
+-rw-rw-rw-   0 root         (0) root         (0)     3266 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/speech-bubbles-comment-option.png
+-rw-rw-rw-   0 root         (0) root         (0)     3339 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/star-1.png
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/star-half-empty.png
+-rw-rw-rw-   0 root         (0) root         (0)     3138 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/star.png
+-rw-rw-rw-   0 root         (0) root         (0)     3109 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/submenu.png
+-rw-rw-rw-   0 root         (0) root         (0)     3342 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/sun.png
+-rw-rw-rw-   0 root         (0) root         (0)    10543 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/switch.png
+-rw-rw-rw-   0 root         (0) root         (0)    10895 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/switch_arrow.png
+-rw-rw-rw-   0 root         (0) root         (0)    10905 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/switch_binary.png
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/tag-black-shape.png
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/tags.png
+-rw-rw-rw-   0 root         (0) root         (0)     3416 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/team-admin.png
+-rw-rw-rw-   0 root         (0) root         (0)     3513 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/team-lead.png
+-rw-rw-rw-   0 root         (0) root         (0)     3323 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/team.png
+-rw-rw-rw-   0 root         (0) root         (0)     3082 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/text-file-1.png
+-rw-rw-rw-   0 root         (0) root         (0)     3139 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/text-file.png
+-rw-rw-rw-   0 root         (0) root         (0)      340 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/ui-layout.png
+-rw-rw-rw-   0 root         (0) root         (0)    13060 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/undefined.png
+-rw-rw-rw-   0 root         (0) root         (0)     3215 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/user-admin.png
+-rw-rw-rw-   0 root         (0) root         (0)     3324 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/user-lead.png
+-rw-rw-rw-   0 root         (0) root         (0)     3378 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/user-md-symbol.png
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/user-shape.png
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/user.png
+-rw-rw-rw-   0 root         (0) root         (0)     3124 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/users.png
+-rw-rw-rw-   0 root         (0) root         (0)     6941 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/wheel_throbber.gif
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/youtube-logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/zoom-in.png
+-rw-rw-rw-   0 root         (0) root         (0)     3338 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/zoom-out.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.196012 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/DONE.png
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/ERR.png
+-rw-rw-rw-   0 root         (0) root         (0)     3014 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/INV.png
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/NONE.png
+-rw-rw-rw-   0 root         (0) root         (0)     2999 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/NYS.png
+-rw-rw-rw-   0 root         (0) root         (0)     3130 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/OOP.png
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/RTK.png
+-rw-rw-rw-   0 root         (0) root         (0)     3113 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/RVW.png
+-rw-rw-rw-   0 root         (0) root         (0)     3212 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/WAIT.png
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/WARN.png
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/WIP.png
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4143 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/standalone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.196012 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.196012 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/dark/
+-rw-rw-rw-   0 root         (0) root         (0)     4601 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/dark/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14402 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/dark/dark_style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.197012 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/gray/
+-rw-rw-rw-   0 root         (0) root         (0)     2551 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/gray/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7679 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/gray/gray_style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.197012 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/neonative/
+-rw-rw-rw-   0 root         (0) root         (0)      564 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/neonative/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12549 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/neonative/neonative_style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.199012 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.202012 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3632 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/bool_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     4292 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/choice_value.py
+-rw-rw-rw-   0 root         (0) root         (0)    69953 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/default_thumbnail.py
+-rw-rw-rw-   0 root         (0) root         (0)    10405 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/image_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     5839 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/label.py
+-rw-rw-rw-   0 root         (0) root         (0)     7293 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/multichoice_value.py
+-rw-rw-rw-   0 root         (0) root         (0)      781 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/password_value.py
+-rw-rw-rw-   0 root         (0) root         (0)    12187 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/path_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/percent_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     3951 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/python_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     6651 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/textarea.py
+-rw-rw-rw-   0 root         (0) root         (0)     9715 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/thumbnail.py
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/time_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     4060 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/event_filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.204012 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/flow_editors.py
+-rw-rw-rw-   0 root         (0) root         (0)    12229 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/flow_field.py
+-rw-rw-rw-   0 root         (0) root         (0)    32692 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/flow_form.py
+-rw-rw-rw-   0 root         (0) root         (0)    22229 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/flow_view.py
+-rw-rw-rw-   0 root         (0) root         (0)    18977 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/map_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     9352 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/navigation_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/navigator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5973 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/ref_by.py
+-rw-rw-rw-   0 root         (0) root         (0)     2927 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/script_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     2784 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow_layout.py
+-rw-rw-rw-   0 root         (0) root         (0)     9397 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/form_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)    11734 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/main_window.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/popup_menu.py
+-rw-rw-rw-   0 root         (0) root         (0)     8699 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/session_toolbar.py
+-rw-rw-rw-   0 root         (0) root         (0)    15858 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/widget_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     2759 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/app/ui/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.206012 kabaret-2.3.0rc5/python/kabaret/flow/
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/flow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6698 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/flow/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/flow/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7540 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/flow/injection.py
+-rw-rw-rw-   0 root         (0) root         (0)    33049 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/flow/map.py
+-rw-rw-rw-   0 root         (0) root         (0)    31344 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/flow/object.py
+-rw-rw-rw-   0 root         (0) root         (0)    14403 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/flow/relations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/flow/value_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    15531 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/python/kabaret/flow/values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:18:36.207012 kabaret-2.3.0rc5/python/kabaret.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14817 2024-04-26 12:18:36.000000 kabaret-2.3.0rc5/python/kabaret.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13413 2024-04-26 12:18:36.000000 kabaret-2.3.0rc5/python/kabaret.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 12:18:36.000000 kabaret-2.3.0rc5/python/kabaret.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 12:18:36.000000 kabaret-2.3.0rc5/python/kabaret.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-26 12:18:36.000000 kabaret-2.3.0rc5/python/kabaret.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-04-26 12:18:36.208011 kabaret-2.3.0rc5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2158 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2024-04-26 12:18:27.000000 kabaret-2.3.0rc5/versioneer.py
```

### Comparing `kabaret-2.3.0rc4/CHANGELOG.md` & `kabaret-2.3.0rc5/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,28 @@
 
 issue #120 - New `path` editor which allows to select one or more file paths through the file explorer.
 
 issue #121 - New `image` editor which allows to load an image to the base64 format and display it. The image can be selected through the file explorer or dragged and dropped.
 
 issue #117 - The `KabaretStandaloneGUISession` session now keeps track of the `FlowView` currently focused, which can be retrieved using the session's `current_view()` method. Whenever the current view changes, a `focus_changed` event is dispatched with the ID of the new current view.
 
+issue #122 - Layout preset tools on the `SessionToolBar` view have been improved to handle additional view state data such as size, position, navigation history and also window geometry.
+For now, presets are stored locally in `.json` files on the user session and structured by cluster. You can specify a different folder path with `--layout-savepath` command line argument.
+The upcoming 'Users' actor will extend storage possibilities, such as store presets in the redis database.
+Activation of layout tools is done on the `KabaretStandaloneGUISession` session and new command line arguments are here for easy disabling if needed.
+A session layout autosave feature can be enabled, making backups of the last five sessions in their most recent state.
+
 ### Changed
 
 issue #112 - Versioneer is now used for versioning control system. You can access kabaret version using : `import kabaret; print(kabaret.__version__)`. Versioneer will be more usefull for releases.
 
+### Fixed
+
+Remove a stretch in layout when using Custom Page. Caused problems for resizing and fully expanding the page size.
+
 ## [2.2.0] - 2023-02-01
 
 ### ! Python version support !
 
 2.2 is the last version of Kabaret supporting Python 2. Incoming versions starting from 2.3 will exclusively support Python 3.
 
 ### ! Breaking changes !
```

### Comparing `kabaret-2.3.0rc4/LICENSE` & `kabaret-2.3.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/PKG-INFO` & `kabaret-2.3.0rc5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kabaret
-Version: 2.3.0rc4
+Version: 2.3.0rc5
 Summary: VFX/Animation Studio Framework
 Home-page: http://www.kabaretstudio.com
 Author: Damien dee Coureau
 Author-email: kabaret-dev@googlegroups.com
 License: LGPLv3+
 Keywords: vfx animation framewok dataflow workflow asset manager production tracker
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,18 +57,28 @@
 
 issue #120 - New `path` editor which allows to select one or more file paths through the file explorer.
 
 issue #121 - New `image` editor which allows to load an image to the base64 format and display it. The image can be selected through the file explorer or dragged and dropped.
 
 issue #117 - The `KabaretStandaloneGUISession` session now keeps track of the `FlowView` currently focused, which can be retrieved using the session's `current_view()` method. Whenever the current view changes, a `focus_changed` event is dispatched with the ID of the new current view.
 
+issue #122 - Layout preset tools on the `SessionToolBar` view have been improved to handle additional view state data such as size, position, navigation history and also window geometry.
+For now, presets are stored locally in `.json` files on the user session and structured by cluster. You can specify a different folder path with `--layout-savepath` command line argument.
+The upcoming 'Users' actor will extend storage possibilities, such as store presets in the redis database.
+Activation of layout tools is done on the `KabaretStandaloneGUISession` session and new command line arguments are here for easy disabling if needed.
+A session layout autosave feature can be enabled, making backups of the last five sessions in their most recent state.
+
 ### Changed
 
 issue #112 - Versioneer is now used for versioning control system. You can access kabaret version using : `import kabaret; print(kabaret.__version__)`. Versioneer will be more usefull for releases.
 
+### Fixed
+
+Remove a stretch in layout when using Custom Page. Caused problems for resizing and fully expanding the page size.
+
 ## [2.2.0] - 2023-02-01
 
 ### ! Python version support !
 
 2.2 is the last version of Kabaret supporting Python 2. Incoming versions starting from 2.3 will exclusively support Python 3.
 
 ### ! Breaking changes !
```

### Comparing `kabaret-2.3.0rc4/lgpl-3.0.txt` & `kabaret-2.3.0rc5/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/demo_project/__init__.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/demo_project/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/demo_project/maya_startup/__init__.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/demo_project/maya_startup/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/demo_project/maya_startup/userSetup.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/demo_project/maya_startup/userSetup.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/__init__.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/icon_browser/__init__.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/icon_browser/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/action_context.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/action_context.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/action_dialog_size.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/action_dialog_size.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/action_submenus_demo.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/action_submenus_demo.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/actions.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/actions.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/custom_page.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/custom_page.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/editors.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/editors.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/injection.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/injection.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/map_as_view.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/map_as_view.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/maps.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/maps.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/other.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/other.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/relations.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/relations.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/ui_config.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/ui_config.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/flow/unittest_project/showcase/values.py` & `kabaret-2.3.0rc5/python/dev_studio/flow/unittest_project/showcase/values.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/gui.py` & `kabaret-2.3.0rc5/python/dev_studio/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,14 +80,19 @@
 
 if __name__ == '__main__':
     argv = sys.argv[1:]  # get ride of first args wich is script filename
     (
         session_name,
         host, port, cluster_name,
         db_index, password, debug,
+        layout_mgr, layout_autosave, layout_savepath,
         remaining_args
     ) = MyStudioGUISession.parse_command_line_args(argv)
-    session = MyStudioGUISession(session_name=session_name)
+
+    session = MyStudioGUISession(
+        session_name=session_name, debug=debug,
+        layout_mgr=layout_mgr, layout_autosave=layout_autosave, layout_savepath=layout_savepath
+    )
     session.cmds.Cluster.connect(host, port, cluster_name, db_index, password)
 
     session.start()
     session.close()
```

### Comparing `kabaret-2.3.0rc4/python/dev_studio/icons/flow/__init__.py` & `kabaret-2.3.0rc5/python/dev_studio/icons/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/dev_studio/icons/gui/kabaret_icon.png` & `kabaret-2.3.0rc5/python/dev_studio/icons/gui/kabaret_icon.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/__init__.py` & `kabaret-2.3.0rc5/python/kabaret/app/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/_actor.py` & `kabaret-2.3.0rc5/python/kabaret/app/_actor.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/actors/cluster.py` & `kabaret-2.3.0rc5/python/kabaret/app/actors/cluster.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/actors/default_actors_plugin.py` & `kabaret-2.3.0rc5/python/kabaret/app/actors/default_actors_plugin.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/actors/flow/actor.py` & `kabaret-2.3.0rc5/python/kabaret/app/actors/flow/actor.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/actors/flow/generic_home_flow.py` & `kabaret-2.3.0rc5/python/kabaret/app/actors/flow/generic_home_flow.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/actors/flow/utils.py` & `kabaret-2.3.0rc5/python/kabaret/app/actors/flow/utils.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/actors/flow/value_store.py` & `kabaret-2.3.0rc5/python/kabaret/app/actors/flow/value_store.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/plugin_manager.py` & `kabaret-2.3.0rc5/python/kabaret/app/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/resources.py` & `kabaret-2.3.0rc5/python/kabaret/app/resources.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/session.py` & `kabaret-2.3.0rc5/python/kabaret/app/session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import sys, os
 import logging
 import platform
 import getpass
 import re
 import traceback
 import argparse
+import pathlib
+import json
 
 import six
 
+from datetime import datetime
 from .plugin_manager import PluginManager
 from .actors import default_actors_plugin
 
 class SessionCmds(object):
 
     def __init__(self):
         super(SessionCmds, self).__init__()
@@ -117,20 +120,37 @@
         )
         parser.add_argument(
             '-p', '--password', default=None, dest='password', help='Database Password'
         )
         parser.add_argument(
             '-d', '--debug', default=False, action='store_const', const=True, dest='debug', help='Debug Mode'
         )
+        parser.add_argument(
+            '--layout-mgr', default=False, action='store_true', dest='layout_mgr', help='Enable Layout Manager'
+        )
+        parser.add_argument(
+            '--no-layout-mgr', action='store_false', dest='layout_mgr', help='Disable Layout Manager'
+        )
+        parser.add_argument(
+            '--layout-autosave', default=False, action='store_true', dest='layout_autosave', help='Use Layout Autosave'
+        )
+        parser.add_argument(
+            '--no-layout-autosave', action='store_false', dest='layout_autosave', help='Disable Layout Autosave'
+        )
+        parser.add_argument(
+            '--layout-savepath', default=None, dest='layout_savepath', help='Specify Layout Saves Path'
+        )
 
         values, remaining_args = parser.parse_known_args(args)
         return (
             values.session_name,
             values.host, values.port, values.cluster_name,
-            values.db, values.password, values.debug, remaining_args
+            values.db, values.password, values.debug,
+            values.layout_mgr, values.layout_autosave, values.layout_savepath,
+            remaining_args
         )
 
     @classmethod
     def get_session(cls, session_uid=None):
         '''
         Returns one of the sessions. If `session_uid` is None,
         the last created one is returned.
@@ -154,41 +174,57 @@
                 return session
         raise ValueError(
             "No session with uid '{}' found.".format(
                 session_uid
             )
         )
 
-    def __init__(self, session_name=None, debug=False):
+    def __init__(self,
+        session_name=None, debug=False,
+        layout_mgr=False, layout_autosave=False, layout_savepath=None
+    ):
         super(KabaretSession, self).__init__()
         self._session_name = session_name or self.__class__.__name__
         
         self.__class__._SESSIONS.append(self)
 
         self._ticked = []
         self._actors = {}
         self.cmds = SessionCmds()
         self.debug_mode = debug
 
         # View Management
         self._view_types = {}
         self._views = {}
 
+        self.layout_manager = layout_mgr
+        self.layout_autosave = layout_autosave
+        self.layout_savepath = layout_savepath
+        
+        self.layout_load = False
+        self.layout_sessionpath = None
+
         self.log_formatter = logging.Formatter("%(name)s -- %(asctime)s -- %(levelname)s: %(message)s")
         self.stream_formatter = logging.Formatter("%(name)s - %(levelname)s: %(message)s")
         self.logger = logging.getLogger('kabaret')
         if debug:
             self.logger.setLevel(logging.DEBUG)
         else:
             self.logger.setLevel(logging.INFO)
 
         self.default_log_handler = logging.StreamHandler(sys.stdout)
         self.default_log_handler.setFormatter(self.stream_formatter)
         self.logger.addHandler(self.default_log_handler)
 
+        if self.layout_manager:
+            self.log_info("Enabling Layout Manager")
+        
+        if self.layout_autosave:
+            self.log_info("Enabling Layout Autosave")
+
         self._plugin_manager = PluginManager(self)
         self.register_plugins(self._plugin_manager)
 
         self.log_info("Plugins installed:")
         for name, plugin in self._plugin_manager._manager.list_name_plugin():
             self.log_info('    {}'.format(name))
         self._plugin_manager.apply_block_list()
@@ -400,14 +436,36 @@
 
         :param actor_name: name of the Actor to return
         :return: :class:`kabaret.app._actor.Actor` subclass instance.
         '''
         return self._actors[actor_name]
 
     #
+    #       USER SETTINGS
+    #
+    def user_settings_folder(self):
+        # Switch to specific path if argument is used
+        if self.layout_savepath:
+            if os.path.exists(self.layout_savepath):
+                return os.path.join(
+                    self.layout_savepath,
+                    ".kabaret",
+                    self._cluster_actor.get_cluster_name()
+                )
+            else:
+                self.log_warning('Layout save path does not exist. Fallback to default.')
+        
+        # Use default path
+        return os.path.join(
+            pathlib.Path.home(),
+            ".kabaret",
+            self._cluster_actor.get_cluster_name()
+        )
+
+    #
     #       VIEW MANAGEMENT
     #
     def register_view_types(self):
         '''
         Register all the view types available in the session.
 
         Subclasses can override this to install customs Views.
@@ -590,60 +648,181 @@
         (:class:`KabaretStandaloneGUISession` does.)
 
         The ``state`` argument is the return value of a call to
         :meth:`_get_layout_state`
         '''
         raise NotImplementedError()
 
-    def get_views_state(self):
+    def _get_geometry_state(self):
+        '''
+        Subclasses with GUI must override this to return a state valid
+        for :meth:`_get_geometry_state`.
+        (:class:`KabaretStandaloneGUISession` does.)
+
+        :return: a json serializable object describing the current UI geometry state.
+        '''
+        raise NotImplementedError()
+    
+    def _set_geometry_state(self, state):
+        '''
+        Subclasses with GUI must implement this to restore the GUI
+        geometry state described by ``state``.
+        (:class:`KabaretStandaloneGUISession` does.)
+
+        The ``state`` argument is the return value of a call to
+        :meth:`_get_geometry_state`
+        '''
+        raise NotImplementedError()
+
+    def get_views_state(self, main_geometry=False):
         '''
         Returns the state of all views.
 
         The return value can be used as argument for
         :meth:`set_views_state` to restore all the views
         to this state.
         '''
+
+        # Get all current views and their statuses
         views = []
         for view_id, view in six.iteritems(self._views):
             view_state = view.get_view_state()
             if view_state is not None:
                 views.append((
                     view.view_type_name(), 
                     view.view_id(),
+                    view.isHidden(),
+                    view.areaPosition().name.decode("utf-8"),
+                    json.dumps(bytes(view.saveGeometry().toHex()).decode("ascii")), # ByteArray to unicode
                     view_state
                 ))
-            
-        layout = self._get_layout_state()
+        
+        # Get window layout state
+        layout = json.dumps(bytes(self._get_layout_state().toHex()).decode("ascii")) # ByteArray to unicode
+        
         state = dict(views=views, layout=layout)
+        
+        # Get window position (geometry) if attribute is true
+        if main_geometry:
+            geometry = json.dumps(bytes(self._get_geometry_state().toHex()).decode("ascii")) # ByteArray to unicode
+            state["geometry"] = geometry
+        
         return state
 
     def set_views_state(self, state):
         '''
         Restores the views to the state described by ``state``
 
         The ``state`` value must be one returned by
         :meth:`get_views_state`
         '''
-        for view in self._views.values():
+        from qtpy import QtCore
+
+        # For block specific signals (such as autosave)
+        self.layout_load = True
+
+        # Clear all current views
+        for view in list(self._views.values()):
             view.delete_view()
         self._views.clear()
 
-        from qtpy import QtWidgets
-        QtWidgets.QApplication.processEvents()
-
+        # Instantiate views to the state
         views = state.get('views', [])
         view_ids = []
-        for view_type_name, view_id, view_state in views:
+        for view_type_name, view_id, view_hidden, view_area, view_geometry, view_state in views:
             view_ids.append(view_id)
-            view = self.add_view(view_type_name, view_id)
+            
+            kwargs = {"area": view_area, "hidden": view_hidden}
+            if "oid" in view_state:
+                kwargs['oid'] = view_state['oid']
+
+            view = self.add_view(view_type_name, view_id, **kwargs)
             view.set_view_state(view_state)
 
+            view_geometry = QtCore.QByteArray.fromHex(bytes(view_geometry, 'ascii')) # Restore to ByteArray format
+            view.restoreGeometry(view_geometry)
+        
+        # Restore main window geometry
+        geometry = state.get('geometry')
+        if geometry is not None:
+            geometry = QtCore.QByteArray.fromHex(bytes(geometry, 'ascii')) # Restore to ByteArray format
+            self._set_geometry_state(geometry)
+        
+        # Restore layout state
         layout = state.get('layout')
         if layout is not None:
+            layout = QtCore.QByteArray.fromHex(bytes(layout, 'ascii')) # Restore to ByteArray format
             self._set_layout_state(layout)
+        
+        self.layout_load = False
+
+    def get_layout_presets(self, autosaves=False):
+        # Tmp until we have a User actor to store those things
+        layout_folder = os.path.join(self.user_settings_folder(), 'layouts')
+        if autosaves:
+            layout_folder += '/autosaves'
+
+        # Open and store all json files
+        layouts = {}
+        if os.path.exists(layout_folder):
+            for file_name in os.listdir(layout_folder):
+                if os.path.isfile(os.path.join(layout_folder, file_name)) and file_name.endswith('.json'):
+                    layout_name = file_name.strip('.json')
+                    
+                    f = open(os.path.join(layout_folder, file_name), 'r')
+                    layouts[layout_name] = json.load(f)
+                    
+                    f.close()
+
+        return layouts
+
+    def store_layout_preset(self, layout_preset, name=None, autosave=False):
+        # Tmp until we have a User actor to store those things
+        
+        # Set folder path
+        layout_folder = os.path.join(self.user_settings_folder(), 'layouts')
+        if autosave:
+            layout_folder += '/autosaves'
+            name = datetime.now().strftime('%Y-%m-%d %H-%M-%S') # Autosave will be named with current date and time
+        
+        # Create folder if not exists
+        if not os.path.exists(layout_folder):
+            os.makedirs(layout_folder)
+        
+        if autosave:
+            # Use current session save if one already exists
+            if self.layout_sessionpath:
+                name, _ = os.path.basename(self.layout_sessionpath).split('.json')
+            else:
+                self.layout_sessionpath = f'{layout_folder}/{name}.json'
+
+        # Write json file
+        with open(f'{layout_folder}/{name}.json', 'w') as f:
+            json.dump(layout_preset, f)
+
+        if autosave:
+            # Get all saves to keep only the last five sessions
+            list_of_saves = [
+                os.path.join(layout_folder, save_name)
+                for save_name in os.listdir(layout_folder)
+            ]
+
+            if len(list_of_saves) >= 6:
+                oldest_save = min(list_of_saves, key=os.path.getctime)
+                os.remove(os.path.abspath(oldest_save))
+
+    def delete_layout_preset(self, names):
+        # Tmp until we have a User actor to store those things
+
+        # Set folder path
+        layout_folder = os.path.join(self.user_settings_folder(), 'layouts')
+        
+        if os.path.exists(layout_folder):
+            for file_name in names:
+                os.remove(os.path.join(layout_folder, f'{file_name}.json'))
 
     #
     #       LOGGING
     #
     def log(self, context, *words):
         self._log(logging.INFO, ' '.join([str(i) for i in words]), extra={'context': context})
```

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/embedded.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/embedded.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/3dsmax.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/3dsmax.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/action.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/action.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/afterfx.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/afterfx.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/alembic.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/alembic.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/asset.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/asset.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/asset_family.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/asset_family.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/bank.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/bank.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/branch.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/branch.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/casting.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/casting.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/editor_proc.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/editor_proc.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/explorer.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/explorer.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/file.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/file.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/film.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/film.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/folder.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/folder.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/goto.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/goto.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/guerilla.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/guerilla.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/hannah.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/hannah.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/houdini.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/houdini.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/input.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/input.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/job.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/job.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/jobs.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/jobs.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/jump_to.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/jump_to.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/lightroom_xmp.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/lightroom_xmp.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/maya.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/maya.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/maya_tools.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/maya_tools.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/mayapy.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/mayapy.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/mrviewer.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/mrviewer.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/muster8.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/muster8.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/natron.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/natron.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/node.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/node.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/note.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/note.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/notepad.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/notepad.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/notethread.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/notethread.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/nuke.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/nuke.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/nuke10.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/nuke10.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/object.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/object.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/output.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/output.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/parent.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/parent.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/pdplayer.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/pdplayer.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/photoshop.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/photoshop.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/quicktime.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/quicktime.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/ref.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/ref.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/resolve.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/resolve.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/scheduled.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/scheduled.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/sequence.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/sequence.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/shot.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/shot.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/slop.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/slop.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/smedge.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/smedge.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/speedgrade.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/speedgrade.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/task.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/task.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/value.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/value.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/vrak.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/vrak.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/flow/workstation.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/flow/workstation.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/bookmark-black-shape.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/bookmark-black-shape.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/check-box-empty.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/check-box-empty.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/check-mark.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/check-mark.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/check.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/check.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-down-disabled.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-down-disabled.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-down.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-down.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-left-disabled.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-left-disabled.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-left.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-left.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-to-right-disabled.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-to-right-disabled.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-to-right.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-to-right.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-up-disabled.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-up-disabled.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/chevron-sign-up.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/chevron-sign-up.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/circle-shape-outline.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/circle-shape-outline.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/cog-wheel-silhouette.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/cog-wheel-silhouette.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/copy-document.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/copy-document.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/correct-symbol.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/correct-symbol.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/cross-mark-on-a-black-circle-background.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/cross-mark-on-a-black-circle-background.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/dice.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/dice.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/dice_3d.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/dice_3d.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/exclamation-sign.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/exclamation-sign.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/file.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/file.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/film-strip-with-two-photograms.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/film-strip-with-two-photograms.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/filter-tool-black-shape.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/filter-tool-black-shape.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/folder-closed-black-shape.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/folder-closed-black-shape.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/folder-white-shape.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/folder-white-shape.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/group-profile-users.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/group-profile-users.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/heart-shape-outline.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/heart-shape-outline.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/heart-shape-silhouette.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/heart-shape-silhouette.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/home-outline.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/home-outline.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/home.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/home.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/italicize-text.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/italicize-text.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/kabaret_icon.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/kabaret_icon.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/kabaret_logo.gif` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/kabaret_logo.gif`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/kabaret_logo_vector.svg` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/kabaret_logo_vector.svg`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/man.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/man.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/maximize.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/maximize.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/minimize.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/minimize.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/minus-button.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/minus-button.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/open-folder-outline.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/open-folder-outline.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/open-folder.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/open-folder.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/open-laptop-computer.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/open-laptop-computer.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/open-padlock-silhouette.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/open-padlock-silhouette.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/padlock.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/padlock.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/paste-from-clipboard.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/paste-from-clipboard.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/picture.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/picture.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/plus-black-symbol.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/plus-black-symbol.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/plus-sign-in-a-black-circle.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/plus-sign-in-a-black-circle.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/plus-symbol-in-a-rounded-black-square.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/plus-symbol-in-a-rounded-black-square.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/power_button.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/power_button.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/power_button_2.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/power_button_2.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/remove-button.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/remove-button.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/remove-symbol.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/remove-symbol.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/search.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/search.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/settings.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/settings.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/share-option.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/share-option.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/share-post-symbol.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/share-post-symbol.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/share-symbol.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/share-symbol.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/sitemap.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/sitemap.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/sort-arrows-couple-pointing-up-and-down.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/sort-arrows-couple-pointing-up-and-down.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/sort-down.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/sort-down.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/sort-up.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/sort-up.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/speech-bubbles-comment-option.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/speech-bubbles-comment-option.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/star-1.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/star-1.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/star-half-empty.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/star-half-empty.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/star.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/star.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/submenu.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/submenu.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/sun.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/sun.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/switch.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/switch.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/switch_arrow.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/switch_arrow.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/switch_binary.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/switch_binary.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/tag-black-shape.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/tag-black-shape.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/tags.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/tags.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/team-admin.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/team-admin.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/team-lead.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/team-lead.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/team.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/team.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/text-file-1.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/text-file-1.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/text-file.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/text-file.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/undefined.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/undefined.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/user-admin.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/user-admin.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/user-lead.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/user-lead.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/user-md-symbol.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/user-md-symbol.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/user-shape.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/user-shape.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/user.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/user.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/users.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/users.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/wheel_throbber.gif` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/wheel_throbber.gif`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/youtube-logo.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/youtube-logo.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/zoom-in.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/zoom-in.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/gui/zoom-out.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/gui/zoom-out.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/DONE.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/DONE.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/ERR.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/ERR.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/INV.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/INV.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/NONE.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/NONE.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/NYS.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/NYS.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/OOP.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/OOP.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/RTK.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/RTK.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/RVW.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/RVW.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/WAIT.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/WAIT.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/WARN.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/WARN.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/icons/status/WIP.png` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/icons/status/WIP.png`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/standalone.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/standalone.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 from qtpy import QtCore, QtWidgets
 from .widgets.main_window import MainWindowManager
 from .widgets.flow.flow_view import FlowView
 from .widgets.flow import FlowViewPlugin
 
 class KabaretStandaloneGUISession(KabaretSession):
 
-    def __init__(self, session_name='Standalone', tick_every_ms=10, debug=False):
-        super(KabaretStandaloneGUISession, self).__init__(session_name, debug)
+    def __init__(self,
+        session_name='Standalone', tick_every_ms=10, debug=False,
+        layout_mgr=False, layout_autosave=False, layout_savepath=None
+    ):
+        super(KabaretStandaloneGUISession, self).__init__(session_name, debug, layout_mgr, layout_autosave, layout_savepath)
         self.main_window_manager = None
         self.tick_every_ms = tick_every_ms
         self._current_view = None
 
     def is_gui(self):
         return True
 
@@ -92,14 +95,20 @@
         super(KabaretStandaloneGUISession, self).register_view_types()
 
     def _get_layout_state(self):
         return self.main_window_manager.get_layout_state()
 
     def _set_layout_state(self, state):
         self.main_window_manager.set_layout_state(state)
+    
+    def _get_geometry_state(self):
+        return self.main_window_manager.get_geometry_state()
+    
+    def _set_geometry_state(self, state):
+        self.main_window_manager.set_geometry_state(state)
 
     def _on_cluster_connected(self):
         '''
         Overridden to also dispatch a 'cluster_connection' event to GUI.
         '''
         super(KabaretStandaloneGUISession, self)._on_cluster_connected()
         self.dispatch_event(
```

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/__init__.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/dark/__init__.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/dark/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/dark/dark_style.css` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/dark/dark_style.css`

 * *Files 2% similar despite different names*

```diff
@@ -137,28 +137,33 @@
 /*
 ###############################
 		ComboBox
 ###############################
 */
 QComboBox
 {
-	border: 2px solid palette(dark);
-	padding-left: 0.5em;
-	padding-right: 0.5em;
+	border: 1px solid palette(dark);
+	border-radius: 5px;
+	padding: 5px;
+	text-align: center;
 }
 QComboBox QAbstractItemView 
 {
 	border: 1px solid palette(shadow);
 	border-top: none;
 }
 QComboBox QAbstractItemView::focus
 {
 	border: 1px solid palette(shadow);
 	border-top: none;
 }
+QComboBox:editable
+{
+	background: palette(base);
+}
 QComboBox:!editable
 {
 	background: palette(window);
 	border: 1px solid palette(dark);
 	border-radius: 5px;
 	padding: 5px;
 	text-align: center;
```

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/gray/__init__.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/gray/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/gray/gray_style.css` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/gray/gray_style.css`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/neonative/__init__.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/neonative/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/styles/neonative/neonative_style.css` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/styles/neonative/neonative_style.css`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/__init__.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/bool_value.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/bool_value.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/choice_value.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/choice_value.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/default_thumbnail.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/default_thumbnail.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/image_value.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/image_value.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/interface.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/interface.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/label.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/label.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/multichoice_value.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/multichoice_value.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/password_value.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/password_value.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/path_value.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/path_value.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/percent_value.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/percent_value.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/python_value.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/python_value.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/textarea.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/textarea.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/thumbnail.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/thumbnail.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/editors/time_value.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/editors/time_value.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/event_filters.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/event_filters.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/__init__.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/flow_editors.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/flow_editors.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/flow_field.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/flow_field.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/flow_form.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/flow_form.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/flow_view.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/flow_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,14 +80,17 @@
 
     def __init__(self, page):
         super(CustomPageHost, self).__init__(page)
         self.page = page
         self._hosted = None
         self.setLayout(QtWidgets.QVBoxLayout())
 
+    def has_host(self):
+        return bool(self._hosted)
+
     def unhost(self):
         self.hide()
         if self._hosted is not None:
             self._hosted.die()
 
         # Clear all layout items (including spacing stuff)
         li = self.layout().takeAt(0)
@@ -143,15 +146,14 @@
     def host(self, oid, custom_page_str):
         if self._hosted is not None:
             self.unhost()
         self._hosted = self._create_hosted(custom_page_str)
         self.show()
         self._hosted.set_oid(oid)
         self.layout().addWidget(self._hosted)
-        self.layout().addStretch(100)
 
     def dispatch_touch_event(self, oid):
         if self._hosted is not None:
             self._hosted.on_touch_event(oid)
 
 class FlowPage(QtWidgets.QWidget):
 
@@ -179,33 +181,46 @@
         lo.setContentsMargins(0, 0, 0, 0)
         lo.setSpacing(0)
         self.setLayout(lo)
         lo.addWidget(self.form, 100)
         lo.addWidget(self.custom_page_host, 100)
 
         self._navigator.add_on_current_changed(self.refresh)
+        self._navigator.add_on_list_changed(self.nav_bar.nav_ctrl.update)
 
         self._source_view_id = None
         # self._dialogs = {}  # oid to dialg widget
 
         # FIXME: wtf is this ?!? why isn't this in NavigationBar class ?!?
         self.nav_bar.setAttribute(QtCore.Qt.WA_StyledBackground, True)
 
     def root_oid(self):
         return self._navigator.root_oid()
+    
+    def set_root_oid(self, oid):
+        return self._navigator.apply_new_root_oid(oid)
 
     def current_oid(self):
         return self._navigator.current_oid()
 
     def set_source_view_id(self, source_view_id):
         '''
         Used by run_action to find affected vie by stuffs like 'goto' request
         '''
         self._source_view_id = source_view_id
 
+    def history_oids(self):
+        return self._navigator.history_oids()
+
+    def set_history_oids(self, oids):
+        return self._navigator.apply_history_oids(oids)
+
+    def has_custom_page(self):
+        return self.custom_page_host.has_host()
+
     def open(self, oid):
         self._navigator.goto(oid, new_view=True)
 
     def goto(self, oid):
         in_new_view = (
                 QtWidgets.QApplication.keyboardModifiers() == QtCore.Qt.ControlModifier
         )
@@ -327,14 +342,25 @@
         if custom_page:
             self.custom_page_host.host(oid, custom_page)
             self.form.hide()
         else:
             self.custom_page_host.unhost()
             self.form.show()
             self.form.build_roots(oid)
+        
+        # Update session layout autosave
+        if (
+            self.session.layout_autosave 
+            and self.session.layout_load is False
+            and (isinstance(self.view, FlowView) and self.view.dock_widget())
+        ):
+            self.session.store_layout_preset(
+                self.session.get_views_state(main_geometry=True),
+                autosave=True
+            )
 
     def receive_event(self, event, data):
         # print('   --- FlowPage got event', event, data)
         if event == 'flow_touched':
             oid = data['oid']
             self.custom_page_host.dispatch_touch_event(oid)
             root = self.form.invisibleRootItem()
@@ -423,18 +449,14 @@
         self.resize(w, h)
 
     def show(self):
         super(FlowDialogView, self).show()
         self.flow_page.refresh()
         self.fitSize()
 
-    def delete_view(self):
-        self.flow_page.form.stop_building()
-        super(FlowDialogView, self).delete_view()
-
     def receive_event(self, event, data):
         # print('   --- FlowDialogView got event', event, data)
         if event == 'flow_touched':
             self.flow_page.receive_event(event, data)
 
     def on_action_result_close(self):
         self.accept()
@@ -536,40 +558,38 @@
         main_parent.setLayout(lo)
         self.flow_page.refresh()
 
     def _build(self, top_parent, top_layout, main_parent, header_parent, header_layout):
         self.build_top(top_parent, top_layout, header_parent, header_layout)
         self.build_page(main_parent)
 
-    def delete_view(self):
-        self.flow_page.form.stop_building()
-        super(FlowView, self).delete_view()
-
     def get_view_state(self):
         self.setObjectName(self.view_id())
         self.dock_widget().setObjectName(self.view_id())
 
         return dict(
             oid=self.flow_page.current_oid(),
             root_oid=self._root_oid,
+            history_oids=self.flow_page.history_oids(),
             form_config=self.flow_page.form.config()
         )
 
     def set_view_state(self, state):
         oid = state.get('oid', self.flow_page.current_oid())
         root_oid = state.get('root_oid', self._root_oid)
+        history_oids = state.get('history_oids', [])
         form_config = state.get('form_config')
 
-        if form_config is not None:
+        if form_config is not None and self.flow_page.has_custom_page() is False:
             self.flow_page.form.configure(**form_config)
 
         self._start_oid = oid
         self._root_oid = root_oid
-        self.flow_page._navigator._root_oid = root_oid  # ugly !!! add a public api for that !
-        self.flow_page.goto(oid)
+        self.flow_page.set_root_oid(root_oid)
+        self.flow_page.set_history_oids(history_oids)
 
     def set_show_references_relations(self, b):
         self.flow_page.form.configure(show_references_relation=b)
 
     def set_show_navigation_bar(self, b):
         self.flow_page.nav_bar.setVisible(b)
         self._show_nav_bar_action.setChecked(b)
```

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/map_field.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/map_field.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/navigation_control.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/navigation_control.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/navigator.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/navigator.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
         self._current_oid = current_oid or root_oid
         self._prev_list = []
         self._next_list = []
 
         self._on_current_changed = []  # list of callables
         #---OLD self._on_current_corrected = [] # list of callbles
 
+        self._on_list_changed = []  # list of callables
+
         self._create_view_function = None
 
         self.refresh()
 
     def add_on_current_changed(self, callable):
         '''callable must accept no args'''
         self._on_current_changed.append(callable)
@@ -38,14 +40,21 @@
     #     self._on_current_corrected.remove(callable)
 
     # def correct_current_oid(self, oid):
     #     self._current_oid = oid
     #     for callable in self._on_current_corrected:
     #         callable(self._current_oid)
 
+    def add_on_list_changed(self, callable):
+        '''callable must accept no args'''
+        self._on_list_changed.append(callable)
+
+    def remove_on_list_changed(self, callable):
+        self._on_list_changed.remove(callable)
+
     def set_create_view_function(self, f):
         '''
         The callable f must accept one argument:
                 the oid to load on the new view.
         '''
         self._create_view_function = f
 
@@ -60,14 +69,17 @@
     def refresh(self):
         ''' -> goto current oid'''
         self.goto(self.current_oid())
 
     def root_oid(self):
         return self._root_oid
 
+    def apply_new_root_oid(self, oid):
+        self._root_oid = oid
+
     def current_oid(self):
         return self._current_oid
 
     def _apply_new_current_oid(self, oid):
         self._current_oid = self.session.cmds.Flow.resolve_path(oid)
         for callable in self._on_current_changed:
             callable()
@@ -78,14 +90,22 @@
             return
 
         self._next_list = []
         if self._current_oid and oid != self._current_oid:
             self._prev_list.append(self._current_oid)
         self._apply_new_current_oid(oid)
 
+    def history_oids(self):
+        return self._prev_list
+
+    def apply_history_oids(self, prev_list):
+        self._prev_list = prev_list
+        for callable in self._on_list_changed:
+            callable()
+
     def has_prev(self):
         return self._prev_list and True or False
 
     def goto_prev(self):
         if not self._prev_list:
             return
         self._next_list.append(self._current_oid)
```

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/ref_by.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/ref_by.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow/script_line.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow/script_line.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/flow_layout.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/form_tree.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/form_tree.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/main_window.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/main_window.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import print_function
 
 import traceback
 
 from qtpy import QtWidgets, QtCore
+from datetime import datetime
 
 from ..styles import StylesManager
 
 from ..icons import gui     # noqa # just declaring resources...
 from ..icons import status  # noqa # just declaring resources...
 from kabaret.app import resources
 
@@ -95,23 +96,32 @@
     def dock_area(self):
         mw = self.parentWidget()
         return mw.dockWidgetArea(self)
 
 
 class MainWindow(QtWidgets.QMainWindow):
 
-    def __init__(self, parent=None):
+    def __init__(self, session, parent=None):
         super(MainWindow, self).__init__(parent)
+        self.session = session
+    
+    def closeEvent(self, event):
+        # Save views state on exit to be restored
+        if self.session.layout_manager and self.session.layout_autosave:
+            self.session.store_layout_preset(
+                self.session.get_views_state(main_geometry=True),
+                autosave=True
+            )
 
 
 class MainWindowManager(object):
 
     @classmethod
     def create_window(cls, session, parent=None):
-        mw = MainWindow(parent)
+        mw = MainWindow(session, parent)
         manager = cls(session, mw, embed_mode=False)
         return manager
 
     def __init__(self, session, main_window, embed_mode=False):
         super(MainWindowManager, self).__init__()
         self.main_window = main_window
         self.session = session
@@ -154,18 +164,23 @@
             view.about_to_delete()
             self._docks.remove(dock)
             dock.deleteLater()
             return
 
     def dock_visibility_changed(self, visible, dock, view):
         if not visible:
+            view.hidden = True
             view.on_hide()
         else:
+            view.hidden = False
             view.on_show()
 
+    def dock_location_changed(self, location, dock, view):
+        view.area = location
+
     def register_view_type(self, Type):
         print('!!! WARNING !!!')
         print('!!! WARNING !!! session.main_window_manager.register_view_type() is deprecated !')
         print('!!! WARNING !!! (You must use session.register_view_type() instead)')
         print('!!! WARNING !!!')
         return self.session.register_view_type(Type)
 
@@ -201,38 +216,43 @@
             tb.deleteLater()
 
         dock.setWidget(view)
 
         dock.visibilityChanged.connect(
             lambda visible, dock=dock, view=view: self.dock_visibility_changed(visible, dock, view)
         )
+        dock.dockLocationChanged.connect(
+            lambda area, dock=dock, view=view: self.dock_location_changed(area, dock, view)
+        )
         dock.setObjectName('Dock_%s_%i' % (view.view_title(), len(self._docks),))
 
         area = area or QtCore.Qt.LeftDockWidgetArea
         self.main_window.addDockWidget(area, dock)
 
+        if hidden:
+            dock.hide()
+
         # Auto tabify views of matching type name:
         target_view = self.find_docked_view(view.view_type_name(), area=area)
         if target_view is not None:
+            target_view.dock_widget().show()
+            dock.show()
             self.main_window.tabifyDockWidget(target_view.dock_widget(), dock)
 
         self._docks.append(dock)
 
         if len(self._docks) > 1:
             for d in self._docks:
                 if d.titleBarWidget() and d.titleBarWidget().maximize_butt:
                     d.titleBarWidget().maximize_butt.setEnabled(True)
         else:
             for d in self._docks:
                 if d.titleBarWidget() and d.titleBarWidget().maximize_butt:
                     d.titleBarWidget().maximize_butt.setEnabled(False)
 
-        if hidden:
-            dock.hide()
-
         return dock
 
     def tabify_view(self, first_view, second_view):
         d1 = first_view.dock_widget()
         d2 = second_view.dock_widget()
         self.main_window.tabifyDockWidget(d1, d2)
 
@@ -308,13 +328,19 @@
     #     if event_type == 'cluster_connection':
     #         cluster_name = data['cluster_name']
     #         self._set_title(cluster_name)
 
     #     for T in self._view_types.values():
     #         for view in T._VIEWS:
     #             view.receive_event(event_type, data)
+
+    def get_geometry_state(self):
+        return self.main_window.saveGeometry()
+    
+    def set_geometry_state(self, state):
+        self.main_window.restoreGeometry(state)
     
     def get_layout_state(self):
         return self.main_window.saveState()
 
     def set_layout_state(self, state):
         self.main_window.restoreState(state)
```

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/popup_menu.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/popup_menu.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/gui/widgets/widget_view.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/gui/widgets/widget_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,32 +66,62 @@
                 'The "%s" view cannont be used in a session without a main_window' % (
                     self.__class__.__name__
                 )
             )
         ViewMixin.__init__(self, session, view_id)
         QtWidgets.QToolBar.__init__(self, main_window)
 
+        self.hidden = hidden
+        self.area = area
+        self._main_window_manager = session.main_window_manager
+        
+        # Restore correct ToolBarArea enum value from string
+        self.areaEnum = dict(
+            LeftToolBarArea=QtCore.Qt.LeftToolBarArea,
+            RightToolBarArea=QtCore.Qt.RightToolBarArea,
+            TopToolBarArea=QtCore.Qt.TopToolBarArea,
+            BottomToolBarArea=QtCore.Qt.BottomToolBarArea,
+        )
+
+        if isinstance(self.area, str):
+            self.area = self.getAreaFromEnum()
+
         # This is needed for layout state
         # Multi instance view types must use another policy
         self.setObjectName(self.view_type_name())
 
-        session.main_window_manager.add_toolbar_view(self, hidden=hidden, area=area)
+        self._main_window_manager.add_toolbar_view(self, hidden=hidden, area=self.area)
+
+        self.visibilityChanged.connect(self.toolbar_visibility_changed)
 
         self.set_on_view_title_change(self._on_view_title_change)
         self.set_view_title(self.view_type_name())
 
     def _fix_raise_fail_on_windows(self):
         self.raise_()
 
     def ensure_visible(self):
         # There is a known bug on window where calling raise() works only
         # if the view is already parented+visible.
         # Known workaround is to delay the raise().
         QtCore.QTimer.singleShot(0, self._fix_raise_fail_on_windows)
 
+    def isHidden(self):
+        return self.hidden
+
+    def areaPosition(self):
+        return self.area
+
+    def getAreaFromEnum(self):
+        return self.areaEnum[self.area] if self.area in self.areaEnum else None
+
+    def toolbar_visibility_changed(self, visible):
+        self.hidden = not visible
+        self.area = self._main_window_manager.main_window.toolBarArea(self)
+
     def _on_view_title_change(self):
         self.setWindowTitle(self.view_title())
 
     def delete_view(self):
         self.session.forget_view(self)
         self.session.main_window_manager.main_window.removeToolBar(self)
         self.deleteLater()
@@ -107,15 +137,28 @@
                 'The "%s" view cannont be used in a session without a main_window'%(
                     self.__class__.__name__
                 )
             )
         ViewMixin.__init__(self, session, view_id)
         QtWidgets.QWidget.__init__(self, None)
 
+        self.hidden = hidden
+        self.area = area
         self._main_window_manager = session.main_window_manager
+        
+        # Restore correct DockWidgetArea enum value from string
+        self.areaEnum = dict(
+            LeftDockWidgetArea=QtCore.Qt.LeftDockWidgetArea,
+            RightDockWidgetArea=QtCore.Qt.RightDockWidgetArea,
+            TopDockWidgetArea=QtCore.Qt.TopDockWidgetArea,
+            BottomDockWidgetArea=QtCore.Qt.BottomDockWidgetArea,
+        )
+
+        if isinstance(self.area, str):
+            self.area = self.getAreaFromEnum()
 
         # Menu
         self.menubar = QtWidgets.QMenuBar(self)
         self.view_menu = QtWidgets.QMenu(self.view_title())
         self.menubar.addMenu(self.view_menu)
 
         # Tools
@@ -143,15 +186,15 @@
         self._build(
             self, top_layout, content_widget,
             self, header_widgets_layout
         )
 
         self._update_menus()
 
-        dock = self._main_window_manager.create_docked_view_dock(self, hidden=hidden, area=area)
+        dock = self._main_window_manager.create_docked_view_dock(self, hidden=hidden, area=self.area)
 
         # This is needed for layout state
         # Multi instance view types must use another policy
         dock.setObjectName(self.view_id())
 
     def _create_scrolled_area(self, parent):
         scroll_area = QtWidgets.QScrollArea(parent)
@@ -194,14 +237,23 @@
         self.dock_widget().raise_()
 
     def ensure_visible(self):
         # There is a known bug on window where calling raise() works only
         # if the view is already parented+visible.
         # Known workaround is to delay the raise().
         QtCore.QTimer.singleShot(0, self._fix_raise_fail_on_windows)
+    
+    def isHidden(self):
+        return self.hidden
+    
+    def areaPosition(self):
+        return self.area
+
+    def getAreaFromEnum(self):
+        return self.areaEnum[self.area] if self.area in self.areaEnum else None
 
     # def set_on_view_title_change(self, f):
     #     self._on_view_title_change = f
 
     # def set_view_title(self, title):
     #     self._view_title = title
     #     if self._on_view_title_change is not None:
```

### Comparing `kabaret-2.3.0rc4/python/kabaret/app/ui/view.py` & `kabaret-2.3.0rc5/python/kabaret/app/ui/view.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/flow/__init__.py` & `kabaret-2.3.0rc5/python/kabaret/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/flow/action.py` & `kabaret-2.3.0rc5/python/kabaret/flow/action.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/flow/exceptions.py` & `kabaret-2.3.0rc5/python/kabaret/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/flow/injection.py` & `kabaret-2.3.0rc5/python/kabaret/flow/injection.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/flow/map.py` & `kabaret-2.3.0rc5/python/kabaret/flow/map.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/flow/object.py` & `kabaret-2.3.0rc5/python/kabaret/flow/object.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/flow/relations.py` & `kabaret-2.3.0rc5/python/kabaret/flow/relations.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/flow/value_store.py` & `kabaret-2.3.0rc5/python/kabaret/flow/value_store.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret/flow/values.py` & `kabaret-2.3.0rc5/python/kabaret/flow/values.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/python/kabaret.egg-info/PKG-INFO` & `kabaret-2.3.0rc5/python/kabaret.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kabaret
-Version: 2.3.0rc4
+Version: 2.3.0rc5
 Summary: VFX/Animation Studio Framework
 Home-page: http://www.kabaretstudio.com
 Author: Damien dee Coureau
 Author-email: kabaret-dev@googlegroups.com
 License: LGPLv3+
 Keywords: vfx animation framewok dataflow workflow asset manager production tracker
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,18 +57,28 @@
 
 issue #120 - New `path` editor which allows to select one or more file paths through the file explorer.
 
 issue #121 - New `image` editor which allows to load an image to the base64 format and display it. The image can be selected through the file explorer or dragged and dropped.
 
 issue #117 - The `KabaretStandaloneGUISession` session now keeps track of the `FlowView` currently focused, which can be retrieved using the session's `current_view()` method. Whenever the current view changes, a `focus_changed` event is dispatched with the ID of the new current view.
 
+issue #122 - Layout preset tools on the `SessionToolBar` view have been improved to handle additional view state data such as size, position, navigation history and also window geometry.
+For now, presets are stored locally in `.json` files on the user session and structured by cluster. You can specify a different folder path with `--layout-savepath` command line argument.
+The upcoming 'Users' actor will extend storage possibilities, such as store presets in the redis database.
+Activation of layout tools is done on the `KabaretStandaloneGUISession` session and new command line arguments are here for easy disabling if needed.
+A session layout autosave feature can be enabled, making backups of the last five sessions in their most recent state.
+
 ### Changed
 
 issue #112 - Versioneer is now used for versioning control system. You can access kabaret version using : `import kabaret; print(kabaret.__version__)`. Versioneer will be more usefull for releases.
 
+### Fixed
+
+Remove a stretch in layout when using Custom Page. Caused problems for resizing and fully expanding the page size.
+
 ## [2.2.0] - 2023-02-01
 
 ### ! Python version support !
 
 2.2 is the last version of Kabaret supporting Python 2. Incoming versions starting from 2.3 will exclusively support Python 3.
 
 ### ! Breaking changes !
```

### Comparing `kabaret-2.3.0rc4/python/kabaret.egg-info/SOURCES.txt` & `kabaret-2.3.0rc5/python/kabaret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/setup.py` & `kabaret-2.3.0rc5/setup.py`

 * *Files identical despite different names*

### Comparing `kabaret-2.3.0rc4/versioneer.py` & `kabaret-2.3.0rc5/versioneer.py`

 * *Files identical despite different names*

