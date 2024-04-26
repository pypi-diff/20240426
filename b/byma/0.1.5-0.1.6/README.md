# Comparing `tmp/byma-0.1.5.tar.gz` & `tmp/byma-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byma-0.1.5.tar", last modified: Fri Apr 12 08:12:59 2024, max compression
+gzip compressed data, was "byma-0.1.6.tar", last modified: Fri Apr 26 06:00:23 2024, max compression
```

## Comparing `byma-0.1.5.tar` & `byma-0.1.6.tar`

### file list

```diff
@@ -1,99 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.714717 byma-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-12 08:12:48.000000 byma-0.1.5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-12 08:12:48.000000 byma-0.1.5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      522 2024-04-12 08:12:48.000000 byma-0.1.5/CHANGELOG.txt
--rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-12 08:12:48.000000 byma-0.1.5/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-12 08:12:48.000000 byma-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3433 2024-04-12 08:12:59.713717 byma-0.1.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-12 08:12:48.000000 byma-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.702717 byma-0.1.5/byma/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-12 08:12:48.000000 byma-0.1.5/byma/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-12 08:12:59.000000 byma-0.1.5/byma/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.704717 byma-0.1.5/byma/interface/
--rw-rw-rw-   0 root         (0) root         (0)     2612 2024-04-12 08:12:48.000000 byma-0.1.5/byma/interface/BaseInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-12 08:12:48.000000 byma-0.1.5/byma/interface/NonlinearHeat.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2024-04-12 08:12:48.000000 byma-0.1.5/byma/interface/Time.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-12 08:12:48.000000 byma-0.1.5/byma/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.705717 byma-0.1.5/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)      187 2024-04-12 08:12:48.000000 byma-0.1.5/byma/iteral/Iteral.py
--rw-rw-rw-   0 root         (0) root         (0)     5149 2024-04-12 08:12:48.000000 byma-0.1.5/byma/iteral/Newton.py
--rw-rw-rw-   0 root         (0) root         (0)     4811 2024-04-12 08:12:48.000000 byma-0.1.5/byma/iteral/OrthogonalSubspace.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-12 08:12:48.000000 byma-0.1.5/byma/iteral/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.706717 byma-0.1.5/byma/nuby/
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-12 08:12:48.000000 byma-0.1.5/byma/nuby/Bifurcation.py
--rw-rw-rw-   0 root         (0) root         (0)     7951 2024-04-12 08:12:48.000000 byma-0.1.5/byma/nuby/Continuation.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-12 08:12:48.000000 byma-0.1.5/byma/nuby/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-12 08:12:48.000000 byma-0.1.5/byma/nuby/_nuby.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.706717 byma-0.1.5/byma/numy/
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-12 08:12:48.000000 byma-0.1.5/byma/numy/Numy.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-12 08:12:48.000000 byma-0.1.5/byma/numy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-12 08:12:48.000000 byma-0.1.5/byma/numy/_numy.py
--rw-rw-rw-   0 root         (0) root         (0)     3576 2024-04-12 08:12:48.000000 byma-0.1.5/byma/numy/integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.707717 byma-0.1.5/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-12 08:12:48.000000 byma-0.1.5/byma/pyplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6283 2024-04-12 08:12:48.000000 byma-0.1.5/byma/pyplot/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.713717 byma-0.1.5/byma.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3433 2024-04-12 08:12:59.000000 byma-0.1.5/byma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1918 2024-04-12 08:12:59.000000 byma-0.1.5/byma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 08:12:59.000000 byma-0.1.5/byma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-12 08:12:59.000000 byma-0.1.5/byma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.707717 byma-0.1.5/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-12 08:12:48.000000 byma-0.1.5/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-12 08:12:48.000000 byma-0.1.5/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-12 08:12:48.000000 byma-0.1.5/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.708717 byma-0.1.5/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.708717 byma-0.1.5/docs/source/autoapi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.708717 byma-0.1.5/docs/source/autoapi/byma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.708717 byma-0.1.5/docs/source/autoapi/byma/_version/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/_version/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.709717 byma-0.1.5/docs/source/autoapi/byma/interface/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.709717 byma-0.1.5/docs/source/autoapi/byma/interface/BaseInterface/
--rw-rw-rw-   0 root         (0) root         (0)     1551 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/interface/BaseInterface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.709717 byma-0.1.5/docs/source/autoapi/byma/interface/NonlinearHeat/
--rw-rw-rw-   0 root         (0) root         (0)     2105 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.709717 byma-0.1.5/docs/source/autoapi/byma/interface/Time/
--rw-rw-rw-   0 root         (0) root         (0)     6246 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/interface/Time/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3809 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/interface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.709717 byma-0.1.5/docs/source/autoapi/byma/iteral/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/iteral/Iteral/
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/iteral/Iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/iteral/Newton/
--rw-rw-rw-   0 root         (0) root         (0)     1912 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/iteral/Newton/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)     2112 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      405 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/nuby/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/nuby/Bifurcation/
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/nuby/Continuation/
--rw-rw-rw-   0 root         (0) root         (0)     4607 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/nuby/Continuation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.711717 byma-0.1.5/docs/source/autoapi/byma/nuby/_nuby/
--rw-rw-rw-   0 root         (0) root         (0)     4840 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/nuby/_nuby/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5112 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/nuby/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.711717 byma-0.1.5/docs/source/autoapi/byma/numy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.711717 byma-0.1.5/docs/source/autoapi/byma/numy/Numy/
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/numy/Numy/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.711717 byma-0.1.5/docs/source/autoapi/byma/numy/_numy/
--rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/numy/_numy/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2116 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/numy/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.711717 byma-0.1.5/docs/source/autoapi/byma/numy/integration/
--rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/numy/integration/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.712717 byma-0.1.5/docs/source/autoapi/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     3599 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/pyplot/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.712717 byma-0.1.5/docs/source/autoapi/byma/pyplot/plots/
--rw-rw-rw-   0 root         (0) root         (0)     3544 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/pyplot/plots/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3805 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.713717 byma-0.1.5/docs/source/user/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/user/Installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/user/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/user/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/user/whatisbyma.rst
--rwxrwxrwx   0 root         (0) root         (0)     1005 2024-04-12 08:12:48.000000 byma-0.1.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-12 08:12:48.000000 byma-0.1.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 08:12:59.714717 byma-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-12 08:12:48.000000 byma-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.713717 byma-0.1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 08:12:48.000000 byma-0.1.5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.794084 byma-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-26 06:00:11.000000 byma-0.1.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-26 06:00:11.000000 byma-0.1.6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-04-26 06:00:11.000000 byma-0.1.6/CHANGELOG.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-26 06:00:11.000000 byma-0.1.6/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-26 06:00:11.000000 byma-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-04-26 06:00:23.794084 byma-0.1.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-26 06:00:11.000000 byma-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.783084 byma-0.1.6/byma/
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2024-04-26 06:00:11.000000 byma-0.1.6/byma/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-26 06:00:23.000000 byma-0.1.6/byma/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.784085 byma-0.1.6/byma/interface/
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2024-04-26 06:00:11.000000 byma-0.1.6/byma/interface/BaseInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-26 06:00:11.000000 byma-0.1.6/byma/interface/NonlinearHeat.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2024-04-26 06:00:11.000000 byma-0.1.6/byma/interface/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-26 06:00:11.000000 byma-0.1.6/byma/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.785085 byma-0.1.6/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2024-04-26 06:00:11.000000 byma-0.1.6/byma/iteral/Iteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     5149 2024-04-26 06:00:11.000000 byma-0.1.6/byma/iteral/Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)     4872 2024-04-26 06:00:11.000000 byma-0.1.6/byma/iteral/OrthogonalSubspace.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-26 06:00:11.000000 byma-0.1.6/byma/iteral/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.785085 byma-0.1.6/byma/iteral/stationary/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 06:00:11.000000 byma-0.1.6/byma/iteral/stationary/OrthogonalSubspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.786085 byma-0.1.6/byma/nuby/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-26 06:00:11.000000 byma-0.1.6/byma/nuby/Bifurcation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7951 2024-04-26 06:00:11.000000 byma-0.1.6/byma/nuby/Continuation.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-26 06:00:11.000000 byma-0.1.6/byma/nuby/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-26 06:00:11.000000 byma-0.1.6/byma/nuby/_nuby.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.787084 byma-0.1.6/byma/numy/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-26 06:00:11.000000 byma-0.1.6/byma/numy/Numy.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-26 06:00:11.000000 byma-0.1.6/byma/numy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-26 06:00:11.000000 byma-0.1.6/byma/numy/_numy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2024-04-26 06:00:11.000000 byma-0.1.6/byma/numy/integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.787084 byma-0.1.6/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-26 06:00:11.000000 byma-0.1.6/byma/pyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6292 2024-04-26 06:00:11.000000 byma-0.1.6/byma/pyplot/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.794084 byma-0.1.6/byma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-04-26 06:00:23.000000 byma-0.1.6/byma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2012 2024-04-26 06:00:23.000000 byma-0.1.6/byma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 06:00:23.000000 byma-0.1.6/byma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-26 06:00:23.000000 byma-0.1.6/byma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.788085 byma-0.1.6/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-26 06:00:11.000000 byma-0.1.6/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-26 06:00:11.000000 byma-0.1.6/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-26 06:00:11.000000 byma-0.1.6/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.788085 byma-0.1.6/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.789085 byma-0.1.6/docs/source/autoapi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.789085 byma-0.1.6/docs/source/autoapi/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/OrthogonalSubspace/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.789085 byma-0.1.6/docs/source/autoapi/byma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.789085 byma-0.1.6/docs/source/autoapi/byma/_version/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/_version/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.789085 byma-0.1.6/docs/source/autoapi/byma/interface/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.790084 byma-0.1.6/docs/source/autoapi/byma/interface/BaseInterface/
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/interface/BaseInterface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.790084 byma-0.1.6/docs/source/autoapi/byma/interface/NonlinearHeat/
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.790084 byma-0.1.6/docs/source/autoapi/byma/interface/Time/
+-rw-rw-rw-   0 root         (0) root         (0)     6246 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/interface/Time/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9425 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/interface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.790084 byma-0.1.6/docs/source/autoapi/byma/iteral/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.790084 byma-0.1.6/docs/source/autoapi/byma/iteral/Iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/iteral/Iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.791084 byma-0.1.6/docs/source/autoapi/byma/iteral/Newton/
+-rw-rw-rw-   0 root         (0) root         (0)     1912 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/iteral/Newton/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.791084 byma-0.1.6/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)     2111 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      405 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.791084 byma-0.1.6/docs/source/autoapi/byma/nuby/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.791084 byma-0.1.6/docs/source/autoapi/byma/nuby/Bifurcation/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.791084 byma-0.1.6/docs/source/autoapi/byma/nuby/Continuation/
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/nuby/Continuation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.792084 byma-0.1.6/docs/source/autoapi/byma/nuby/_nuby/
+-rw-rw-rw-   0 root         (0) root         (0)     4840 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/nuby/_nuby/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/nuby/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.792084 byma-0.1.6/docs/source/autoapi/byma/numy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.792084 byma-0.1.6/docs/source/autoapi/byma/numy/Numy/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/numy/Numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.792084 byma-0.1.6/docs/source/autoapi/byma/numy/_numy/
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/numy/_numy/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.792084 byma-0.1.6/docs/source/autoapi/byma/numy/integration/
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/numy/integration/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.793084 byma-0.1.6/docs/source/autoapi/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     3599 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/pyplot/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.793084 byma-0.1.6/docs/source/autoapi/byma/pyplot/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     3544 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/pyplot/plots/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.793084 byma-0.1.6/docs/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/user/Installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/user/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/user/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/user/whatisbyma.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1005 2024-04-26 06:00:11.000000 byma-0.1.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-26 06:00:11.000000 byma-0.1.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 06:00:23.794084 byma-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-26 06:00:11.000000 byma-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.794084 byma-0.1.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 06:00:11.000000 byma-0.1.6/tests/__init__.py
```

### Comparing `byma-0.1.5/.gitlab-ci.yml` & `byma-0.1.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/CHANGELOG.txt` & `byma-0.1.6/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/LICENSE.md` & `byma-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/PKG-INFO` & `byma-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.5/README.md` & `byma-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/byma/__init__.py` & `byma-0.1.6/byma/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 ByMa: A scientific computing package for Python
 ================================================
 
-Documentation is available in the docstrings and
-online at 
+
 
 Subpackages
 -----------
 Using any of these subpackages requires an explicit import. For example,
 ``import byma.nuby``.
 
 ::
 
  nuby                         --- Numerical Bifurcation Analysis Tools
  iteral                       --- Tools for iterative algorithms
  pyplot                       --- Tools for plotting functions
  interface                    --- Interface functions
+ numy                         --- Basic Numerical Methods functions
 
 """
 
 import importlib as _importlib
 
 try:
     from importlib.metadata import version  # for Python 3.8+
```

### Comparing `byma-0.1.5/byma/interface/BaseInterface.py` & `byma-0.1.6/byma/interface/BaseInterface.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/byma/interface/NonlinearHeat.py` & `byma-0.1.6/byma/interface/NonlinearHeat.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/byma/interface/Time.py` & `byma-0.1.6/byma/interface/Time.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/byma/iteral/Newton.py` & `byma-0.1.6/byma/iteral/Newton.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/byma/iteral/OrthogonalSubspace.py` & `byma-0.1.6/byma/iteral/OrthogonalSubspace.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 import numpy as np
 from scipy.linalg import lu, inv, solve
+from scipy.sparse import csc_matrix
+from scipy.sparse.linalg import splu
 from numpy.linalg import qr
 from ..interface.BaseInterface import BaseInterface as bs
 from .Iteral import Iteral as Int
 import scipy.sparse as sp
 
 _DEFAULT_OPTS = {
         'stop': 'matrix',
         'maxit': 1e4,
         'tol': 1e-8,
-        'method': 'standard',
+        'which': 'SM',
         'verbose': True,
     }
 
 
     
-def _Z(V, A = None, P=None, L=None, U=None, method = 'standard'):
-    if method == 'LU':
-        y = solve(inv(U), P.dot(V))
-        z = solve(inv(L), y)
+def _Z(X, A = None, which = 'SM'):
+    if sp.issparse(A) == False:
+        A = csc_matrix(A)
+    if which == 'SM':
+        z = splu(A).solve(X)
     else:
-        z = A @ V
+        z = A @ X
     return z
 
 @bs.set_defaults(default_cls = Int, default_opts=_DEFAULT_OPTS)
-def osim(A, V, **kwargs):
+def osim(A, V = None, k = None, **kwargs):
     """
     Orthogonal Subspace Iteration Method (OSIM).
 
     Args:
     A : numpy.ndarray
         The matrix to compute the eigenvalues and eigenvectors for.
     V : numpy.ndarray
-        Initial guess of eigenvectors.
+        Initial guess of eigenvectors. Default None,
+    k : int
+        number of desired eigenvalues. Default None. 
+    
 
     Keyword Arguments:
         tol : float, optional
             Tolerance for convergence (default: 1e-8).
         maxit : int, optional
             Maximum number of iterations (default: 100).
         stop : str, optional
             Stopping criteria for convergence. Options are 'eig' (default), 'matrix', or 'residual'.
-        method : str, optional
-            Method for solving linear systems. Options are 'LU' (default) or any method supported by scipy.linalg.lu.
+        which : str, optional
+            If small or biggest eigenvalues. Default "SM" = smallest. 
         verbose : bool, optional
             If True, prints iteration information (default: True).
 
     Returns:
     numpy.ndarray
         Matrix of eigenvectors.
     numpy.ndarray
@@ -58,61 +64,61 @@
     This function implements the Orthogonal Subspace Iteration Method (OSIM) to compute eigenvectors and eigenvalues of a matrix A.
 
     Examples:
     >>> import numpy as np
     >>> from byma.interal import osim
     >>> A = np.array([[1, 0], [0, 1]])
     >>> V = np.array([[1], [0]])
-    >>> V, BV, iter = osim(A, V, tol=1e-8, maxit=1000, stop='eig', method='LU')
+    >>> V, BV, iter = osim(A, V, tol=1e-8, maxit=1000, stop='eig')
 
     You can also pass keyword arguments using a dictionary. For example:
-    >>> kwargs = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig', 'method': 'LU'}
+    >>> kwargs = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig'}
     >>> V, BV, iter = osim(A, V, **kwargs)
 
     You can also pass keyword arguments using two separate dictionaries for parameters and interface. For example:
-    >>> parameters = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig', 'method': 'LU'}
+    >>> parameters = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig'}
     >>> interface = {'verbose': True}
     >>> V, BV, iter = sosim(A, V, parameters=parameters, interface=interface)
     """
     
-    # Check if the number of rows of V matches the number of columns of A
-    if V.shape[0] != A.shape[1]:
-        raise ValueError("Number of rows of V must match the number of columns of A.")
-    
     _opts = bs.opts(**kwargs)
     verbose = _opts['verbose']
     tol = _opts['tol']
     maxit = int(_opts['maxit'])
     stop = _opts['stop']
-    method = _opts['method']
+    which = _opts['which']
+    
+    # Check if the number of rows of V matches the number of columns of A
+    if V != None:
+        if V.shape[0] != A.shape[1]:
+            raise ValueError("Number of rows of V must match the number of columns of A.")
+    else:
+        if k == None:
+            raise ValueError("Either V or k should be not-None")
+        else:
+            V = np.random.rand(A.shape[1], k)
     
     if verbose:
         print('------ OSIM initialization summary ------')
         print(f'tollerence: {tol}')
         print(f'maximum iter: {maxit}')
         print(f'stopping criteria: {stop}')
-        print(f'Linear system solving method: {method}')
+        print(f'Required eig: {which}')
     
         print('------ Start iteration ------')
-    
-    if method == 'LU':
-        if sp.issparse(A):
-            P, L, U = lu(A.toarray())
-        else:
-            P, L, U = lu(A)
-    else:
-        P = L = U = None
 
-    B = lambda V: V.T @ _Z(V = V, A = A, P = P, L = L, U = U, method = method)
+    B = lambda V: V.T @ _Z(X = V, A = A, which= which)
 
     iter = []
     for n in range(maxit):
-        Zn = _Z(V = V, A = A, P = P, L = L, U = U, method = method)
+        Zn = _Z(X = V, A = A, which= which)
         BV = B(V = V)
         eig = np.diag(BV)
+        if which == 'SM':
+            eig = 1/eig
         if verbose != False: 
             if (n % verbose == 0):
                 print(f"Eigenvalues at n = {n}: {eig}")
         else:
             if (n % 5000 == 0):
                 print(f"iteration n = {n}")
```

### Comparing `byma-0.1.5/byma/nuby/Continuation.py` & `byma-0.1.6/byma/nuby/Continuation.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/byma/numy/integration.py` & `byma-0.1.6/byma/numy/integration.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/byma/pyplot/plots.py` & `byma-0.1.6/byma/pyplot/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,26 +127,27 @@
                 plot_scale(x, y_i, label=label_i, scale=scale, style=style_i)
             else:
                 plot_scale(x_i, y_i, label=label_i, scale=scale, style=style_i)
             i += 1
 
 
     plt.legend()
-    plt.show()
 
     save_title = settings.get('save_title', settings.get('title', 'Plot'))
     save_path = settings.get('save_path', None)
 
     # Save the plot if requested
     if save_title:
         if save_path is None:
             save_path = '.'
         plt.savefig(f"{save_path}/{save_title}.png")
         print(f"Plot saved at: {save_path}/{save_title}.png")
         
+    plt.show()
+        
         
 def plot_numerical_error(n, func, solve_func, save_title=None, save_path=None, **kwargs):
     """
     Plot the numerical error between the exact and numerical solutions and print the maximum error.
 
     Parameters
     ----------
```

### Comparing `byma-0.1.5/byma.egg-info/PKG-INFO` & `byma-0.1.6/byma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.5/byma.egg-info/SOURCES.txt` & `byma-0.1.6/byma.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 byma/interface/NonlinearHeat.py
 byma/interface/Time.py
 byma/interface/__init__.py
 byma/iteral/Iteral.py
 byma/iteral/Newton.py
 byma/iteral/OrthogonalSubspace.py
 byma/iteral/__init__.py
+byma/iteral/stationary/OrthogonalSubspace.py
 byma/nuby/Bifurcation.py
 byma/nuby/Continuation.py
 byma/nuby/__init__.py
 byma/nuby/_nuby.py
 byma/numy/Numy.py
 byma/numy/__init__.py
 byma/numy/_numy.py
@@ -33,14 +34,15 @@
 byma/pyplot/plots.py
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/autoapi/index.rst
+docs/source/autoapi/OrthogonalSubspace/index.rst
 docs/source/autoapi/byma/index.rst
 docs/source/autoapi/byma/_version/index.rst
 docs/source/autoapi/byma/interface/index.rst
 docs/source/autoapi/byma/interface/BaseInterface/index.rst
 docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
 docs/source/autoapi/byma/interface/Time/index.rst
 docs/source/autoapi/byma/iteral/index.rst
```

### Comparing `byma-0.1.5/docs/Makefile` & `byma-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/make.bat` & `byma-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 .. py:module:: byma
 
 .. autoapi-nested-parse::
 
    ByMa: A scientific computing package for Python
    ================================================
 
-   Documentation is available in the docstrings and
-   online at 
+
 
    Subpackages
    -----------
    Using any of these subpackages requires an explicit import. For example,
    ``import byma.nuby``.
 
    ::
 
     nuby                         --- Numerical Bifurcation Analysis Tools
     iteral                       --- Tools for iterative algorithms
     pyplot                       --- Tools for plotting functions
     interface                    --- Interface functions
+    numy                         --- Basic Numerical Methods functions
 
 
 
 Subpackages
 -----------
 .. toctree::
    :titlesonly:
```

### Comparing `byma-0.1.5/docs/source/autoapi/byma/interface/BaseInterface/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/interface/BaseInterface/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/interface/Time/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/interface/Time/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/iteral/Newton/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/iteral/Newton/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -13,33 +13,36 @@
 
 .. autoapisummary::
 
    byma.iteral.OrthogonalSubspace.osim
 
 
 
-.. py:function:: osim(A, V, **kwargs)
+.. py:function:: osim(A, V=None, k=None, **kwargs)
 
    Orthogonal Subspace Iteration Method (OSIM).
 
    Args:
    A : numpy.ndarray
        The matrix to compute the eigenvalues and eigenvectors for.
    V : numpy.ndarray
-       Initial guess of eigenvectors.
+       Initial guess of eigenvectors. Default None,
+   k : int
+       number of desired eigenvalues. Default None. 
+
 
    Keyword Arguments:
        tol : float, optional
            Tolerance for convergence (default: 1e-8).
        maxit : int, optional
            Maximum number of iterations (default: 100).
        stop : str, optional
            Stopping criteria for convergence. Options are 'eig' (default), 'matrix', or 'residual'.
-       method : str, optional
-           Method for solving linear systems. Options are 'LU' (default) or any method supported by scipy.linalg.lu.
+       which : str, optional
+           If small or biggest eigenvalues. Default "SM" = smallest. 
        verbose : bool, optional
            If True, prints iteration information (default: True).
 
    Returns:
    numpy.ndarray
        Matrix of eigenvectors.
    numpy.ndarray
@@ -51,19 +54,19 @@
    This function implements the Orthogonal Subspace Iteration Method (OSIM) to compute eigenvectors and eigenvalues of a matrix A.
 
    Examples:
    >>> import numpy as np
    >>> from byma.interal import osim
    >>> A = np.array([[1, 0], [0, 1]])
    >>> V = np.array([[1], [0]])
-   >>> V, BV, iter = osim(A, V, tol=1e-8, maxit=1000, stop='eig', method='LU')
+   >>> V, BV, iter = osim(A, V, tol=1e-8, maxit=1000, stop='eig')
 
    You can also pass keyword arguments using a dictionary. For example:
-   >>> kwargs = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig', 'method': 'LU'}
+   >>> kwargs = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig'}
    >>> V, BV, iter = osim(A, V, **kwargs)
 
    You can also pass keyword arguments using two separate dictionaries for parameters and interface. For example:
-   >>> parameters = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig', 'method': 'LU'}
+   >>> parameters = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig'}
    >>> interface = {'verbose': True}
    >>> V, BV, iter = sosim(A, V, parameters=parameters, interface=interface)
```

### Comparing `byma-0.1.5/docs/source/autoapi/byma/nuby/Continuation/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/nuby/Continuation/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/nuby/_nuby/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/nuby/_nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/nuby/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/numy/_numy/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/numy/_numy/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/numy/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/numy/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/numy/integration/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/numy/integration/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/pyplot/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/pyplot/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/autoapi/byma/pyplot/plots/index.rst` & `byma-0.1.6/docs/source/autoapi/byma/pyplot/plots/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/conf.py` & `byma-0.1.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/docs/source/index.rst` & `byma-0.1.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/pyproject.toml` & `byma-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byma-0.1.5/setup.py` & `byma-0.1.6/setup.py`

 * *Files identical despite different names*

