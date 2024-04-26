# Comparing `tmp/ophyd-async-0.3a1.tar.gz` & `tmp/ophyd_async-0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd-async-0.3a1.tar", last modified: Mon Mar 25 16:14:41 2024, max compression
+gzip compressed data, was "ophyd_async-0.3a2.tar", last modified: Tue Apr 23 14:45:33 2024, max compression
```

## Comparing `ophyd-async-0.3a1.tar` & `ophyd_async-0.3a2.tar`

### file list

```diff
@@ -1,186 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.070878 ophyd-async-0.3a1/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.046877 ophyd-async-0.3a1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.046877 ophyd-async-0.3a1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.038878 ophyd-async-0.3a1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.046877 ophyd-async-0.3a1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.046877 ophyd-async-0.3a1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     3041 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.046877 ophyd-async-0.3a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-03-25 16:14:41.070878 ophyd-async-0.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.046877 ophyd-async-0.3a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.050877 ophyd-async-0.3a1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/_templates/README
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.050877 ophyd-async-0.3a1/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.050877 ophyd-async-0.3a1/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.050877 ophyd-async-0.3a1/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/explanations/decisions/0003-ophyd-async-migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/explanations/decisions/0004-repository-structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/explanations/decisions/0005-respect-black-line-length.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/explanations/decisions/0006-procedural-device-definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.050877 ophyd-async-0.3a1/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.050877 ophyd-async-0.3a1/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.050877 ophyd-async-0.3a1/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.054878 ophyd-async-0.3a1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/images/bluesky_ophyd_epics_devices_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/images/bluesky_ophyd_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/images/ophyd_favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.054878 ophyd-async-0.3a1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.054878 ophyd-async-0.3a1/docs/user/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/user/examples/epics_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.054878 ophyd-async-0.3a1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/user/explanations/docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/user/explanations/event-loop-choice.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.054878 ophyd-async-0.3a1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/user/how-to/make-a-simple-device.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.054878 ophyd-async-0.3a1/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.054878 ophyd-async-0.3a1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/docs/user/tutorials/using-existing-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 16:14:41.070878 ophyd-async-0.3a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.042878 ophyd-async-0.3a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.054878 ophyd-async-0.3a1/src/ophyd_async/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-25 16:14:40.000000 ophyd-async-0.3a1/src/ophyd_async/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.058878 ophyd-async-0.3a1/src/ophyd_async/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/sim_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/standard_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.058878 ophyd-async-0.3a1/src/ophyd_async/epics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.058878 ophyd-async-0.3a1/src/ophyd_async/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/_backend/_aioca.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/_backend/_p4p.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/_backend/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.058878 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.058878 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.058878 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/drivers/ad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.058878 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/_hdffile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.062878 ophyd-async-0.3a1/src/ophyd_async/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/demo/mover.db
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/demo/sensor.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.062878 ophyd-async-0.3a1/src/ophyd_async/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/motion/motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/pvi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.062878 ophyd-async-0.3a1/src/ophyd_async/epics/signal/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/signal/_epics_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/epics/signal/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.062878 ophyd-async-0.3a1/src/ophyd_async/panda/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/panda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/panda/panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/panda/panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/panda/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/src/ophyd_async/panda/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.066878 ophyd-async-0.3a1/src/ophyd_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-03-25 16:14:41.000000 ophyd-async-0.3a1/src/ophyd_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-03-25 16:14:41.000000 ophyd-async-0.3a1/src/ophyd_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 16:14:41.000000 ophyd-async-0.3a1/src/ophyd_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-25 16:14:41.000000 ophyd-async-0.3a1/src/ophyd_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-25 16:14:41.000000 ophyd-async-0.3a1/src/ophyd_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-25 16:14:41.000000 ophyd-async-0.3a1/src/ophyd_async.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.062878 ophyd-async-0.3a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.062878 ophyd-async-0.3a1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/core/test_async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/core/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/core/test_device_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/core/test_device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/core/test_flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/core/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/core/test_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.062878 ophyd-async-0.3a1/tests/epics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.066878 ophyd-async-0.3a1/tests/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/areadetector/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/areadetector/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/areadetector/test_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/areadetector/test_single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/areadetector/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/areadetector/test_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.066878 ophyd-async-0.3a1/tests/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/demo/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/demo/test_demo_ad_sim_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.066878 ophyd-async-0.3a1/tests/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/motion/test_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/test_records.db
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/epics/test_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.066878 ophyd-async-0.3a1/tests/panda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:14:41.066878 ophyd-async-0.3a1/tests/panda/db/
--rw-r--r--   0 runner    (1001) docker     (127)    15494 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/panda/db/panda.db
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/panda/test_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/panda/test_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/panda/test_panda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/panda/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-25 16:14:36.000000 ophyd-async-0.3a1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.887047 ophyd_async-0.3a2/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.859047 ophyd_async-0.3a2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.859047 ophyd_async-0.3a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.855047 ophyd_async-0.3a2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.859047 ophyd_async-0.3a2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.859047 ophyd_async-0.3a2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-23 14:45:33.887047 ophyd_async-0.3a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/_templates/README
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/examples/epics_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0003-ophyd-async-migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0004-repository-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0005-respect-black-line-length.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/0006-procedural-device-definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations/event-loop-choice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.863047 ophyd_async-0.3a2/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/how-to/compound-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/how-to/make-a-simple-device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/how-to/write-tests-for-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.867047 ophyd_async-0.3a2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/images/bluesky_ophyd_epics_devices_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/images/bluesky_ophyd_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/images/ophyd_favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.867047 ophyd_async-0.3a2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.867047 ophyd_async-0.3a2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/tutorials/using-existing-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:45:33.887047 ophyd_async-0.3a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.855047 ophyd_async-0.3a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.867047 ophyd_async-0.3a2/src/ophyd_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/sim_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/_backend/_aioca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/_backend/_p4p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/_backend/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/aravis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/ad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/_hdffile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.871047 ophyd_async-0.3a2/src/ophyd_async/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/demo/mover.db
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/demo/sensor.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/motion/motor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/epics/pvi/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/pvi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/pvi/pvi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/epics/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/signal/_epics_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/epics/signal/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/panda/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_common_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/panda/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/writers/_hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/panda/writers/_panda_hdf_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/planstubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/planstubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/planstubs/prepare_trigger_and_dets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.875047 ophyd_async-0.3a2/src/ophyd_async/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/demo/sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/sim_pattern_detector_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/sim_pattern_detector_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/src/ophyd_async/sim/sim_pattern_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/src/ophyd_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 14:45:33.000000 ophyd_async-0.3a2/src/ophyd_async.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_device_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/epics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/_backend/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_aravis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/areadetector/test_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.879047 ophyd_async-0.3a2/tests/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/demo/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/demo/test_demo_ad_sim_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/motion/test_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/test_pvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/test_records.db
+-rw-r--r--   0 runner    (1001) docker     (127)    17239 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/epics/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/panda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/panda/db/
+-rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/db/panda.db
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_panda_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_panda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/panda/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/protocols/test_protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:33.883047 ophyd_async-0.3a2/tests/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/demo/test_sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/test_pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/test_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/test_sim_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/sim/test_streaming_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-23 14:45:27.000000 ophyd_async-0.3a2/tests/test_flyer_with_panda.py
```

### Comparing `ophyd-async-0.3a1/.devcontainer/devcontainer.json` & `ophyd_async-0.3a2/.devcontainer/devcontainer.json`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 // For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
-        "dockerfile": "Dockerfile",
-        "target": "build",
-        // Only upgrade pip, we will install the project below
-        "args": {
-            "PIP_OPTIONS": "--upgrade pip"
-        },
+        "dockerfile": "../Dockerfile",
+        "target": "developer"
     },
     "remoteEnv": {
+        // Allow X11 apps to run inside the container
         "DISPLAY": "${localEnv:DISPLAY}"
     },
-    // Set *default* container specific settings.json values on container create.
-    "settings": {
-        "python.defaultInterpreterPath": "/venv/bin/python"
-    },
     "customizations": {
         "vscode": {
+            // Set *default* container specific settings.json values on container create.
+            "settings": {
+                "python.defaultInterpreterPath": "/venv/bin/python",
+                "python.testing.unittestEnabled": false,
+                "python.testing.pytestEnabled": true,
+                "editor.formatOnSave": true,
+                "editor.codeActionsOnSave": {
+                    "source.organizeImports": "explicit"
+                },
+                "[python]": {
+                    "editor.defaultFormatter": "charliermarsh.ruff"
+                }
+            },
             // Add the IDs of extensions you want installed when the container is created.
             "extensions": [
                 "ms-python.python",
+                "github.vscode-github-actions",
                 "tamasfe.even-better-toml",
                 "redhat.vscode-yaml",
-                "ryanluker.vscode-coverage-gutters"
+                "ryanluker.vscode-coverage-gutters",
+                "charliermarsh.ruff",
+                "ms-azuretools.vscode-docker"
             ]
         }
     },
-    // Make sure the files we are mapping into the container exist on the host
-    "initializeCommand": "bash -c 'for i in $HOME/.inputrc; do [ -f $i ] || touch $i; done'",
+    "features": {
+        // Some default things like git config
+        "ghcr.io/devcontainers/features/common-utils:2": {
+            "upgradePackages": false
+        }
+    },
     "runArgs": [
+        // Allow the container to access the host X11 display and EPICS CA
         "--net=host",
-        "--security-opt=label=type:container_runtime_t"
-    ],
-    "mounts": [
-        "source=${localEnv:HOME}/.ssh,target=/root/.ssh,type=bind",
-        "source=${localEnv:HOME}/.inputrc,target=/root/.inputrc,type=bind",
-        // map in home directory - not strictly necessary but useful
-        "source=${localEnv:HOME},target=${localEnv:HOME},type=bind,consistency=cached"
+        // Make sure SELinux does not disable with access to host filesystems like tmp
+        "--security-opt=label=disable"
     ],
-    // make the workspace folder the same inside and outside of the container
-    "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
-    "workspaceFolder": "${localWorkspaceFolder}",
+    // Mount the parent as /workspaces so we can pip install peers as editable
+    "workspaceMount": "source=${localWorkspaceFolder}/..,target=/workspaces,type=bind",
     // After the container is created, install the python project in editable form
-    "postCreateCommand": "pip install -e .[dev] --config-settings editable_mode=compat"
-}
+    "postCreateCommand": "pip install $([ -f dev-requirements.txt ] && echo '-c dev-requirements.txt') -e '.[dev]' && pre-commit install"
+}
```

### Comparing `ophyd-async-0.3a1/.github/CONTRIBUTING.rst` & `ophyd_async-0.3a2/.github/CONTRIBUTING.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-Contributing to the project
-===========================
+# Contribute to the project
 
 Contributions and issues are most welcome! All issues and pull requests are
-handled through GitHub_. Also, please check for any existing issues before
+handled through [GitHub](https://github.com/bluesky/ophyd-async/issues). Also, please check for any existing issues before
 filing a new one. If you have a great idea but it involves big changes, please
 file a ticket before making a pull request! We want to make sure you don't spend
 your time coding something that might not fit the scope of the project.
 
-.. _GitHub: https://github.com/bluesky/ophyd-async/issues
+## Issue or Discussion?
 
-Issue or Discussion?
---------------------
-
-Github also offers discussions_ as a place to ask questions and share ideas. If
+Github also offers [discussions](https://github.com/bluesky/ophyd-async/discussions) as a place to ask questions and share ideas. If
 your issue is open ended and it is not obvious when it can be "closed", please
 raise it as a discussion instead.
 
-.. _discussions: https://github.com/bluesky/ophyd-async/discussions
-
-Code coverage
--------------
+## Code Coverage
 
 While 100% code coverage does not make a library bug-free, it significantly
 reduces the number of easily caught bugs! Please make sure coverage remains the
 same or is improved by a pull request!
-Developer guide
----------------
 
-The `Developer Guide`_ contains information on setting up a development
-environment, running the tests and what standards the code and documentation
-should follow.
+## Developer Information
+
+It is recommended that developers use a [vscode devcontainer](https://code.visualstudio.com/docs/devcontainers/containers). This repository contains configuration to set up a containerized development environment that suits its own needs.
+
+This project was created using the [Diamond Light Source Copier Template](https://github.com/DiamondLightSource/python-copier-template) for Python projects.
 
-.. _Developer Guide: https://blueskyproject.io/ophyd-async/main/developer/how-to/contribute.html
+For more information on common tasks like setting up a developer environment, running the tests, and setting a pre-commit hook, see the template's [How-to guides](https://diamondlightsource.github.io/python-copier-template/2.1.0/how-to.html).
```

### Comparing `ophyd-async-0.3a1/.github/pages/make_switcher.py` & `ophyd_async-0.3a2/.github/pages/make_switcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,29 +20,26 @@
 
 def get_sorted_tags_list() -> List[str]:
     """Get a list of sorted tags in descending order from the repository."""
     stdout = check_output(["git", "tag", "-l", "--sort=-v:refname"])
     return report_output(stdout, "Tags list")
 
 
-def get_versions(ref: str, add: Optional[str], remove: Optional[str]) -> List[str]:
+def get_versions(ref: str, add: Optional[str]) -> List[str]:
     """Generate the file containing the list of all GitHub Pages builds."""
     # Get the directories (i.e. builds) from the GitHub Pages branch
     try:
         builds = set(get_branch_contents(ref))
     except CalledProcessError:
         builds = set()
         logging.warning(f"Cannot get {ref} contents")
 
     # Add and remove from the list of builds
     if add:
         builds.add(add)
-    if remove:
-        assert remove in builds, f"Build '{remove}' not in {sorted(builds)}"
-        builds.remove(remove)
 
     # Get a sorted list of tags
     tags = get_sorted_tags_list()
 
     # Make the sorted versions list from main branches and tags
     versions: List[str] = []
     for version in ["master", "main"] + tags:
@@ -54,46 +51,45 @@
     versions += sorted(builds)
     print(f"Sorted versions: {versions}")
     return versions
 
 
 def write_json(path: Path, repository: str, versions: str):
     org, repo_name = repository.split("/")
+    pages_url = f"https://{org}.github.io"
+    if repo_name != f"{org}.github.io":
+        # Only add the repo name if it isn't the source for the org pages site
+        pages_url += f"/{repo_name}"
     struct = [
-        dict(version=version, url=f"https://{org}.github.io/{repo_name}/{version}/")
-        for version in versions
+        {"version": version, "url": f"{pages_url}/{version}/"} for version in versions
     ]
     text = json.dumps(struct, indent=2)
     print(f"JSON switcher:\n{text}")
     path.write_text(text, encoding="utf-8")
 
 
 def main(args=None):
     parser = ArgumentParser(
-        description="Make a versions.txt file from gh-pages directories"
+        description="Make a versions.json file from gh-pages directories"
     )
     parser.add_argument(
         "--add",
         help="Add this directory to the list of existing directories",
     )
     parser.add_argument(
-        "--remove",
-        help="Remove this directory from the list of existing directories",
-    )
-    parser.add_argument(
         "repository",
         help="The GitHub org and repository name: ORG/REPO",
     )
     parser.add_argument(
         "output",
         type=Path,
         help="Path of write switcher.json to",
     )
     args = parser.parse_args(args)
 
     # Write the versions file
-    versions = get_versions("origin/gh-pages", args.add, args.remove)
+    versions = get_versions("origin/gh-pages", args.add)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ophyd-async-0.3a1/.gitignore` & `ophyd_async-0.3a2/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -62,26 +62,30 @@
 # likely venv names
 .venv*
 venv*
 
 # further build artifacts
 lockfiles/
 
-# Origional File
+# Original File
 *.pyc
 *.swp
 *.bak
 
 # IDE Configs
 .idea/
 .ropeproject
 .vscode/
 
 # notebook checkpoints
 .ipynb_checkpoints
 
 # generated docs
-docs/*/generated
+docs/generated
 docs/savefig
 
 # generated version number
 ophyd_async/_version.py
+
+
+# ruff cache
+.ruff_cache/
```

### Comparing `ophyd-async-0.3a1/.mailmap` & `ophyd_async-0.3a2/.mailmap`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/LICENSE` & `ophyd_async-0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/docs/_templates/custom-class-template.rst` & `ophyd_async-0.3a2/docs/_templates/custom-class-template.rst`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 {{ fullname | escape | underline}}
 
 .. currentmodule:: {{ module }}
 
 .. autoclass:: {{ objname }}
    :members:
+   :undoc-members:
    :show-inheritance:
    :inherited-members:
    :special-members: __call__, __add__, __mul__
 
    {% block methods %}
    {% if methods %}
    .. rubric:: {{ _('Methods') }}
```

### Comparing `ophyd-async-0.3a1/docs/_templates/custom-module-template.rst` & `ophyd_async-0.3a2/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/docs/conf.py` & `ophyd_async-0.3a2/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 from subprocess import check_output
 
 import requests
 
 import ophyd_async
 
 # -- General configuration ------------------------------------------------
-# Source code dir relative to this file
 sys.path.insert(0, os.path.abspath("../../src"))
-
 # General information about the project.
 project = "ophyd-async"
 copyright = "2014, Brookhaven National Lab"
 
 # The full version, including alpha/beta/rc tags.
 release = ophyd_async.__version__
 
@@ -67,21 +65,23 @@
 # nitpicky = True
 
 # A list of (type, target) tuples (by default empty) that should be ignored when
 # generating warnings in "nitpicky mode". Note that type should include the
 # domain name if present. Example entries would be ('py:func', 'int') or
 # ('envvar', 'LD_LIBRARY_PATH').
 nitpick_ignore = [
+    # builtins
     ("py:class", "NoneType"),
     ("py:class", "'str'"),
     ("py:class", "'float'"),
     ("py:class", "'int'"),
     ("py:class", "'bool'"),
     ("py:class", "'object'"),
     ("py:class", "'id'"),
+    # typing
     ("py:class", "typing_extensions.Literal"),
 ]
 
 # Both the class’ and the __init__ method’s docstring are concatenated and
 # inserted into the main body of the autoclass directive
 autoclass_content = "both"
 
@@ -114,29 +114,28 @@
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 # This means you can link things like `str` and `asyncio` to the relevant
 # docs in the python documentation.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
-    "bluesky": ("https://blueskyproject.io/bluesky/", None),
+    "bluesky": ("https://blueskyproject.io/bluesky/main", None),
     "numpy": ("https://numpy.org/devdocs/", None),
     "databroker": ("https://blueskyproject.io/databroker/", None),
     "event-model": ("https://blueskyproject.io/event-model/main", None),
 }
 
 # A dictionary of graphviz graph attributes for inheritance diagrams.
-inheritance_graph_attrs = dict(rankdir="TB")
+inheritance_graph_attrs = {"rankdir": "TB"}
 
 # Common links that should be available on every page
 rst_epilog = """
 .. _NSLS: https://www.bnl.gov/nsls2
 .. _black: https://github.com/psf/black
-.. _flake8: https://flake8.pycqa.org/en/latest/
-.. _isort: https://github.com/PyCQA/isort
+.. _ruff: https://beta.ruff.rs/docs/
 .. _mypy: http://mypy-lang.org/
 .. _pre-commit: https://pre-commit.com/
 """
 
 # Ignore localhost links for periodic check that links in docs are valid
 linkcheck_ignore = [r"http://localhost:\d+/"]
 
@@ -147,71 +146,91 @@
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "pydata_sphinx_theme"
-github_repo = project
+github_repo = "ophyd-async"
 github_user = "bluesky"
-switcher_json = f"https://{github_user}.github.io/{github_repo}/switcher.json"
-# Don't check switcher if it doesn't exist, but warn in a non-failing way
-check_switcher = requests.get(switcher_json).ok
-if not check_switcher:
+switcher_json = "https://blueskyproject.io/ophyd-async/switcher.json"
+switcher_exists = requests.get(switcher_json).ok
+if not switcher_exists:
     print(
         "*** Can't read version switcher, is GitHub pages enabled? \n"
         "    Once Docs CI job has successfully run once, set the "
         "Github pages source branch to be 'gh-pages' at:\n"
         f"    https://github.com/{github_user}/{github_repo}/settings/pages",
         file=sys.stderr,
     )
 
 # Theme options for pydata_sphinx_theme
-html_theme_options = dict(
-    use_edit_page_button=True,
-    github_url=f"https://github.com/{github_user}/{github_repo}",
-    icon_links=[
-        dict(
-            name="PyPI",
-            url=f"https://pypi.org/project/{project}",
-            icon="fas fa-cube",
-        ),
-        dict(
-            name="Gitter",
-            url="https://gitter.im/NSLS-II/DAMA",
-            icon="fas fa-person-circle-question",
-        ),
+# We don't check switcher because there are 3 possible states for a repo:
+# 1. New project, docs are not published so there is no switcher
+# 2. Existing project with latest skeleton, switcher exists and works
+# 3. Existing project with old skeleton that makes broken switcher,
+#    switcher exists but is broken
+# Point 3 makes checking switcher difficult, because the updated skeleton
+# will fix the switcher at the end of the docs workflow, but never gets a chance
+# to complete as the docs build warns and fails.
+html_theme_options = {
+    "logo": {
+        "text": project,
+    },
+    "use_edit_page_button": True,
+    "github_url": f"https://github.com/{github_user}/{github_repo}",
+    "icon_links": [
+        {
+            "name": "PyPI",
+            "url": f"https://pypi.org/project/{project}",
+            "icon": "fas fa-cube",
+        },
+        {
+            "name": "Gitter",
+            "url": "https://gitter.im/NSLS-II/DAMA",
+            "icon": "fas fa-person-circle-question",
+        },
     ],
-    external_links=[
-        dict(
-            name="Bluesky Project",
-            url="https://blueskyproject.io",
-        )
+    "switcher": {
+        "json_url": switcher_json,
+        "version_match": version,
+    },
+    "check_switcher": False,
+    "navbar_end": ["theme-switcher", "icon-links", "version-switcher"],
+    "external_links": [
+        {
+            "name": "Bluesky Project",
+            "url": "https://blueskyproject.io",
+        },
+        {
+            "name": "Release Notes",
+            "url": f"https://github.com/{github_user}/{github_repo}/releases",
+        },
     ],
-    navigation_with_keys=False,
-)
-
+    "navigation_with_keys": False,
+}
 
 # A dictionary of values to pass into the template engine’s context for all pages
-html_context = dict(
-    github_user=github_user,
-    github_repo=project,
-    github_version="master",
-    doc_path="docs",
-)
-
-html_logo = "images/bluesky_ophyd_logo.svg"
-html_favicon = "images/ophyd_favicon.svg"
+html_context = {
+    "github_user": github_user,
+    "github_repo": project,
+    "github_version": version,
+    "doc_path": "docs",
+}
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
 html_show_sphinx = False
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
 html_show_copyright = False
 
+# Logo
+html_logo = "images/bluesky_ophyd_logo.svg"
+html_favicon = "images/ophyd_favicon.svg"
+
 # If False and a module has the __all__ attribute set, autosummary documents
 # every member listed in __all__ and no others. Default is True
 autosummary_ignore_module_all = False
 
 # Turn on sphinx.ext.autosummary
 autosummary_generate = True
```

### Comparing `ophyd-async-0.3a1/docs/developer/explanations/decisions/0003-ophyd-async-migration.rst` & `ophyd_async-0.3a2/docs/explanations/decisions/0003-ophyd-async-migration.rst`

 * *Files 2% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
 Relevant history between all three repositories should be preserved.
 
 Consequences
 ------------
 
 This will require changing the repository structure of Ophyd Async; see 
-the decision on repository structure `./0004-repository-structure` for details.
+the decision on repository structure :doc:`0004-repository-structure` for details.
```

### Comparing `ophyd-async-0.3a1/docs/developer/explanations/decisions/0004-repository-structure.rst` & `ophyd_async-0.3a2/docs/explanations/decisions/0004-repository-structure.rst`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/docs/developer/explanations/decisions/0005-respect-black-line-length.rst` & `ophyd_async-0.3a2/docs/explanations/decisions/0005-respect-black-line-length.rst`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/docs/developer/explanations/decisions/0006-procedural-device-definitions.rst` & `ophyd_async-0.3a2/docs/explanations/decisions/0006-procedural-device-definitions.rst`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/docs/images/bluesky_ophyd_epics_devices_logo.svg` & `ophyd_async-0.3a2/docs/images/bluesky_ophyd_epics_devices_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/docs/images/bluesky_ophyd_logo.svg` & `ophyd_async-0.3a2/docs/images/bluesky_ophyd_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/docs/images/ophyd_favicon.svg` & `ophyd_async-0.3a2/docs/images/ophyd_favicon.svg`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/docs/user/examples/epics_demo.py` & `ophyd_async-0.3a2/docs/examples/epics_demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 
 
 det_old = OldSensor(pv_prefix, name="det_old")
 
 # Create ophyd-async devices
 with DeviceCollector():
     det = demo.Sensor(pv_prefix)
+    det_group = demo.SensorGroup(pv_prefix)
     samp = demo.SampleStage(pv_prefix)
```

### Comparing `ophyd-async-0.3a1/docs/user/explanations/event-loop-choice.rst` & `ophyd_async-0.3a2/docs/explanations/event-loop-choice.rst`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/docs/user/how-to/make-a-simple-device.rst` & `ophyd_async-0.3a2/docs/how-to/make-a-simple-device.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 ====================
 
 .. currentmodule:: ophyd_async.core
 
 To make a simple device, you need to subclass from the
 `StandardReadable` class, create some `Signal` instances, and optionally implement
 other suitable Bluesky `Protocols <hardware_interface>` like
-:class:`~bluesky.protocols.Movable`.
+:external+bluesky:py:class:`bluesky.protocols.Movable`.
 
 The rest of this guide will show examples from ``src/ophyd_async/epics/demo/__init__.py``
 
 Readable
 --------
 
-For a simple :class:`~bluesky.protocols.Readable` object like a `Sensor`, you need to
+For a simple :external+bluesky:py:class:`bluesky.protocols.Readable` object like a `Sensor`, you need to
 define some signals, then tell the superclass which signals should contribute to
 ``read()`` and ``read_configuration()``:
 
-.. literalinclude:: ../../../src/ophyd_async/epics/demo/__init__.py
+.. literalinclude:: ../../src/ophyd_async/epics/demo/__init__.py
    :pyobject: Sensor
 
 First some Signals are constructed and stored on the Device. Each one is passed
 its Python type, which could be:
 
 - A primitive (`str`, `int`, `float`)
 - An array (`numpy.typing.NDArray` or ``Sequence[str]``)
@@ -49,32 +49,32 @@
 
 Movable
 -------
 
 For a more complicated device like a `Mover`, you can still use `StandardReadable`
 and implement some addition protocols:
 
-.. literalinclude:: ../../../src/ophyd_async/epics/demo/__init__.py
+.. literalinclude:: ../../src/ophyd_async/epics/demo/__init__.py
    :pyobject: Mover
 
-The ``set()`` method implements :class:`~bluesky.protocols.Movable`. This
+The ``set()`` method implements :external+bluesky:py:class:`bluesky.protocols.Movable`. This
 creates a `coroutine` ``do_set()`` which gets the old position, units and
 precision in parallel, sets the setpoint, then observes the readback value,
 informing watchers of the progress. When it gets to the requested value it
 completes. This co-routine is wrapped in a timeout handler, and passed to an
 `AsyncStatus` which will start executing it as soon as the Run Engine adds a
 callback to it. The ``stop()`` method then pokes a PV if the move needs to be
 interrupted. 
 
 Assembly
 --------
 
 Compound assemblies can be used to group Devices into larger logical Devices:
 
-.. literalinclude:: ../../../src/ophyd_async/epics/demo/__init__.py
+.. literalinclude:: ../../src/ophyd_async/epics/demo/__init__.py
    :pyobject: SampleStage
 
 This applies prefixes on construction:
 
 - SampleStage is passed a prefix like ``DEVICE:``
 - SampleStage.x will append its prefix ``X:`` to get ``DEVICE:X:``
 - SampleStage.x.velocity will append its suffix ``Velocity`` to get
```

### Comparing `ophyd-async-0.3a1/docs/user/reference/api.rst` & `ophyd_async-0.3a2/docs/reference/api.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 .. autosummary::
     :toctree: ../generated
     :template: custom-module-template.rst
     :recursive:
 
     core
     epics
-    panda
+    panda
```

### Comparing `ophyd-async-0.3a1/docs/user/tutorials/installation.rst` & `ophyd_async-0.3a2/docs/tutorials/installation.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-.. note::
+# Installation
 
-    Ophyd async is included on a provisional basis until the v1.0 release and 
-    may change API on minor release numbers before then
+## Check your version of python
 
-Installation
-============
+You will need python 3.10 or later. You can check your version of python by
+typing into a terminal:
 
-Check your version of python
-----------------------------
+```
+$ python3 --version
+```
 
-You will need python 3.9 or later. You can check your version of python by
-typing into a terminal::
-
-    $ python3 --version
-
-
-Create a virtual environment
-----------------------------
+## Create a virtual environment
 
 It is recommended that you install into a “virtual environment” so this
-installation will not interfere with any existing Python software::
-
-    $ python3 -m venv /path/to/venv
-    $ source /path/to/venv/bin/activate
+installation will not interfere with any existing Python software:
 
+```
+$ python3 -m venv /path/to/venv
+$ source /path/to/venv/bin/activate
+```
 
-Installing the library
-----------------------
+## Installing the library
 
-You can now use ``pip`` to install the library and its dependencies::
+You can now use `pip` to install the library and its dependencies:
 
-    $ python3 -m pip install ophyd-async
+```
+$ python3 -m pip install ophyd-async
+```
 
 If you require a feature that is not currently released you can also install
-from github::
+from github:
 
-    $ python3 -m pip install git+https://github.com/bluesky/ophyd-async.git
+```
+$ python3 -m pip install git+https://github.com/bluesky/ophyd-async.git
+```
 
 The library should now be installed and the commandline interface on your path.
-You can check the version that has been installed by typing::
+You can check the version that has been installed by typing:
 
-    $ ophyd-async --version
+```
+$ ophyd-async --version
+```
```

### Comparing `ophyd-async-0.3a1/docs/user/tutorials/using-existing-devices.rst` & `ophyd_async-0.3a2/docs/tutorials/using-existing-devices.rst`

 * *Files 13% similar despite different names*

```diff
@@ -78,18 +78,19 @@
     $ ipython -i epics_demo.py
     IPython 8.5.0 -- An enhanced Interactive Python. Type '?' for help.
 
     In [1]:
 
 .. ipython:: python
     :suppress:
+    :okexcept:
 
     import sys
     from pathlib import Path
-    sys.path.append(str(Path(".").absolute()/"docs/user/examples"))
+    sys.path.append(str(Path(".").absolute()/"docs/examples"))
     from epics_demo import *
     # Turn off progressbar and table
     RE.waiting_hook = None
     bec.disable_table()
 
 This is like a regular python console with the contents of that file executed.
 IPython adds some extra features like tab completion and magics (shortcut
@@ -99,76 +100,85 @@
 --------------
 
 Ophyd Devices give an interface to the `bluesky.run_engine.RunEngine` so they
 can be used in plans. We can move the ``samp.x`` mover to 100mm using
 `bluesky.plan_stubs.mv`:
 
 .. ipython::
+    :okexcept:
 
     In [1]: RE(mov(samp.x, 100))
 
 If this is too verbose to write, we registered a shorthand with
 ``bluesky.utils.register_transform``: ``<my_plan(args)`` is translated to
 ``RE(my_plan(args))``. The command above can also be run as:
 
 .. ipython::
+    :okexcept:
 
     In [1]: <mov(samp.x, 100)
 
 
 We can get the primary reading of ``samp.x``, in this case its readback value,
 using `bluesky.plan_stubs.rd`:
 
 .. ipython::
+    :okexcept:
 
     In [1]: <rd(samp.x)
 
 We can do a relative move of ``samp.x`` by 10mm, using `bluesky.plan_stubs.mvr`:
 
 .. ipython::
+    :okexcept:
 
     In [1]: <movr(samp.x, -10)
 
 Individual Devices will also expose some of the parameters of the underlying
 hardware on itself. In the case of a `Mover`, we can set and get its
 ``velocity``:
 
 .. ipython::
+    :okexcept:
 
     In [1]: <rd(samp.x.velocity)
 
 Do a scan
 ---------
 
 We can also use the `bluesky.run_engine.RunEngine` to run scans. For instance we
 can do a `bluesky.plans.grid_scan` of ``x`` and ``y`` and plot ``det``:
 
 .. ipython::
+    :okexcept:
 
     @savefig grid_scan1.png width=4in
     In [1]: <grid_scan([det], samp.x, 1, 2, 5, samp.y, 1, 2, 5)
 
 There is also an "energy mode" that can be changed to modify the ``det`` output.
 
 .. ipython::
+    :okexcept:
 
     In [1]: <rd(det.mode)
 
-Although this is an :class:`~enum.Enum` and programmatic code should import and
-use instances of :class:`~ophyd_async.epics.demo.EnergyMode`, we can set it using a
+Although this is an :external+python:py:class:`enum.Enum` and programmatic code should import and
+use instances of `EnergyMode`, we can set it using a
 string value on the commandline:
 
 .. ipython::
+    :okexcept:
 
     In [1]: <mov(det.mode, "High Energy")
 
 The same scan will now give a slightly different output. If we include the v1
 device we can see it gives the same result:
 
 .. ipython::
+    :okexcept:
 
     @savefig grid_scan2.png width=4in
     In [1]: <grid_scan([det, det_old], samp.x, 1, 2, 5, samp.y, 1, 2, 5)
 
 .. seealso::
 
-    How-to `../how-to/make-a-simple-device` to make your own Ophyd Async devices.
+    How-to :doc:`../how-to/make-a-simple-device` to make your own Ophyd Async devices.
```

### Comparing `ophyd-async-0.3a1/pyproject.toml` & `ophyd_async-0.3a2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,35 +3,32 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ophyd-async"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: BSD License",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango"
 dependencies = [
-    "typing-extensions;python_version<'3.8'",
     "networkx>=2.0",
     "numpy",
     "packaging",
     "pint",
     "bluesky>=1.13.0a3",
-    "event-model",
+    "event-model<1.21.0",
     "p4p",
     "pyyaml",
 ]
-
 dynamic = ["version"]
 license.file = "LICENSE"
-readme = "README.rst"
-requires-python = ">=3.9"
+readme = "README.md"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 ca = ["aioca>=1.6"]
 pva = ["p4p"]
 dev = [
     "ophyd_async[pva]",
     "ophyd_async[ca]",
@@ -40,30 +37,30 @@
     "flake8-isort",
     "Flake8-pyproject",
     "h5py",
     "inflection",
     "ipython",
     "ipywidgets",
     "matplotlib",
-    "mypy",
     "myst-parser",
     "numpydoc",
     "ophyd",
     "pickleshare",
     "pipdeptree",
     "pre-commit",
     "pydata-sphinx-theme>=0.12",
     "pyepics>=3.4.2",
-    "pyside6",
+    "pyside6==6.6.2",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-faulthandler",
     "pytest-rerunfailures",
     "pytest-timeout",
+    "ruff",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "sphinx-design",
     "tox-direct",
     "types-mock",
     "types-pyyaml",
 ]
@@ -78,42 +75,23 @@
 email = "tom.cobb@diamond.ac.uk"
 name = "Tom Cobb"
 
 
 [tool.setuptools_scm]
 write_to = "src/ophyd_async/_version.py"
 
-[tool.mypy]
-ignore_missing_imports = true          # Ignore missing stubs in imported modules
-plugins = ["numpy.typing.mypy_plugin"]
-
-[tool.isort]
-float_to_top = true
-profile = "black"
-
-[tool.flake8]
-extend-ignore = [
-    "E203", # See https://github.com/PyCQA/pycodestyle/issues/373
-    "F811", # support typing.overload decorator
-    "F722", # allow Annotated[typ, some_func("some string")]
-    "W504",
-    "W503",
-]
-max-line-length = 88 # Respect black's line length (default 88),
-exclude = [".tox", "venv"]
-
 [tool.pytest.ini_options]
 # Run pytest with all our checkers, and don't spam us with massive tracebacks on error
 addopts = """
-    --tb=native -vv --strict-markers --doctest-modules --doctest-glob="*.rst"
-    --ignore=docs/user/examples --ignore=docs/examples
+    --tb=native -vv --strict-markers --doctest-modules
+    --doctest-glob="*.rst" --doctest-glob="*.md" --ignore=docs/examples
     --cov=src/ophyd_async --cov-report term --cov-report xml:cov.xml
-"""
+    """
 # https://iscinumpy.gitlab.io/post/bound-version-constraints/#watch-for-warnings
-filterwarnings = ["error", "ignore::DeprecationWarning:pkg_resources"]
+filterwarnings = "error"
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "docs src tests"
 log_format = "%(asctime)s,%(msecs)03d %(levelname)s (%(threadName)s) %(message)s"
 log_date_format = "%H:%M:%S"
 
 markers = [
     "motorsim: require the motorsim IOC to be running",
@@ -131,23 +109,35 @@
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 skipsdist=True
 
-[testenv:{pre-commit,mypy,pytest,docs}]
+[testenv:{pre-commit,type-checking,tests,docs}]
 # Don't create a virtualenv for the command, requires tox-direct plugin
 direct = True
 passenv = *
-allowlist_externals = 
-    pytest 
+allowlist_externals =
+    pytest
     pre-commit
     mypy
     sphinx-build
     sphinx-autobuild
 commands =
-    pytest: pytest --cov=ophyd_async --cov-report term --cov-report xml:cov.xml {posargs}
-    mypy: mypy src tests {posargs}
+    tests: pytest --cov=ophyd_async --cov-report term --cov-report xml:cov.xml {posargs}
+    type-checking: ruff check src tests {posargs}
     pre-commit: pre-commit run --all-files {posargs}
     docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html
 """
+
+
+[tool.ruff]
+src = ["src", "tests"]
+line-length = 88
+lint.select = [
+    "C4",   # flake8-comprehensions - https://beta.ruff.rs/docs/rules/#flake8-comprehensions-c4
+    "E",    # pycodestyle errors - https://beta.ruff.rs/docs/rules/#error-e
+    "F",    # pyflakes rules - https://beta.ruff.rs/docs/rules/#pyflakes-f
+    "W",    # pycodestyle warnings - https://beta.ruff.rs/docs/rules/#warning-w
+    "I001", # isort
+]
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/__init__.py` & `ophyd_async-0.3a2/src/ophyd_async/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,37 +2,45 @@
     DirectoryInfo,
     DirectoryProvider,
     NameProvider,
     ShapeProvider,
     StaticDirectoryProvider,
 )
 from .async_status import AsyncStatus
-from .detector import DetectorControl, DetectorTrigger, DetectorWriter, StandardDetector
+from .detector import (
+    DetectorControl,
+    DetectorTrigger,
+    DetectorWriter,
+    StandardDetector,
+    TriggerInfo,
+)
 from .device import Device, DeviceCollector, DeviceVector
 from .device_save_loader import (
     get_signal_values,
     load_device,
     load_from_yaml,
     save_device,
     save_to_yaml,
     set_signal_values,
     walk_rw_signals,
 )
-from .flyer import HardwareTriggeredFlyable, TriggerInfo, TriggerLogic
+from .flyer import HardwareTriggeredFlyable, TriggerLogic
 from .signal import (
     Signal,
     SignalR,
     SignalRW,
     SignalW,
     SignalX,
     observe_value,
     set_and_wait_for_value,
     set_sim_callback,
     set_sim_put_proceeds,
     set_sim_value,
+    soft_signal_r_and_backend,
+    soft_signal_rw,
     wait_for_value,
 )
 from .signal_backend import SignalBackend
 from .sim_signal_backend import SimSignalBackend
 from .standard_readable import StandardReadable
 from .utils import (
     DEFAULT_TIMEOUT,
@@ -57,14 +65,16 @@
     "DeviceCollector",
     "DeviceVector",
     "Signal",
     "SignalR",
     "SignalW",
     "SignalRW",
     "SignalX",
+    "soft_signal_r_and_backend",
+    "soft_signal_rw",
     "observe_value",
     "set_and_wait_for_value",
     "set_sim_callback",
     "set_sim_put_proceeds",
     "set_sim_value",
     "wait_for_value",
     "AsyncStatus",
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/_providers.py` & `ophyd_async-0.3a2/src/ophyd_async/core/_providers.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,18 @@
 
 class StaticDirectoryProvider(DirectoryProvider):
     def __init__(
         self,
         directory_path: Union[str, Path],
         filename_prefix: str = "",
         filename_suffix: str = "",
-        resource_dir: Path = Path("."),
+        resource_dir: Optional[Path] = None,
     ) -> None:
+        if resource_dir is None:
+            resource_dir = Path(".")
         if isinstance(directory_path, str):
             directory_path = Path(directory_path)
         self._directory_info = DirectoryInfo(
             root=directory_path,
             resource_dir=resource_dir,
             prefix=filename_prefix,
             suffix=filename_suffix,
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/async_status.py` & `ophyd_async-0.3a2/src/ophyd_async/core/async_status.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/detector.py` & `ophyd_async-0.3a2/src/ophyd_async/core/detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,88 +6,113 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import (
     AsyncGenerator,
     AsyncIterator,
     Callable,
     Dict,
+    Generic,
     List,
     Optional,
     Sequence,
     TypeVar,
 )
 
 from bluesky.protocols import (
     Collectable,
-    Configurable,
     Descriptor,
     Flyable,
     Preparable,
-    Readable,
     Reading,
     Stageable,
     StreamAsset,
     Triggerable,
     WritesStreamAssets,
 )
 
+from ophyd_async.protocols import AsyncConfigurable, AsyncReadable
+
 from .async_status import AsyncStatus
 from .device import Device
 from .signal import SignalR
 from .utils import DEFAULT_TIMEOUT, merge_gathered_dicts
 
 T = TypeVar("T")
 
 
 class DetectorTrigger(str, Enum):
+    """Type of mechanism for triggering a detector to take frames"""
+
     #: Detector generates internal trigger for given rate
     internal = "internal"
     #: Expect a series of arbitrary length trigger signals
     edge_trigger = "edge_trigger"
     #: Expect a series of constant width external gate signals
     constant_gate = "constant_gate"
     #: Expect a series of variable width external gate signals
     variable_gate = "variable_gate"
 
 
 @dataclass(frozen=True)
 class TriggerInfo:
+    """Minimal set of information required to setup triggering on a detector"""
+
     #: Number of triggers that will be sent
     num: int
     #: Sort of triggers that will be sent
     trigger: DetectorTrigger
     #: What is the minimum deadtime between triggers
     deadtime: float
     #: What is the maximum high time of the triggers
     livetime: float
 
 
 class DetectorControl(ABC):
+    """
+    Classes implementing this interface should hold the logic for
+    arming and disarming a detector
+    """
+
     @abstractmethod
     def get_deadtime(self, exposure: float) -> float:
         """For a given exposure, how long should the time between exposures be"""
 
     @abstractmethod
     async def arm(
         self,
         num: int,
         trigger: DetectorTrigger = DetectorTrigger.internal,
         exposure: Optional[float] = None,
     ) -> AsyncStatus:
-        """Arm the detector and return AsyncStatus.
+        """
+        Arm detector, do all necessary steps to prepare detector for triggers.
+
+        Args:
+            num: Expected number of frames
+            trigger: Type of trigger for which to prepare the detector. Defaults to
+            DetectorTrigger.internal.
+            exposure: Exposure time with which to set up the detector. Defaults to None
+            if not applicable or the detector is expected to use its previously-set
+            exposure time.
 
-        Awaiting the return value will wait for num frames to be written.
+        Returns:
+            AsyncStatus: Status representing the arm operation. This function returning
+            represents the start of the arm. The returned status completing means
+            the detector is now armed.
         """
 
     @abstractmethod
     async def disarm(self):
-        """Disarm the detector"""
+        """Disarm the detector, return detector to an idle state"""
 
 
 class DetectorWriter(ABC):
+    """Logic for making a detector write data to somewhere persistent
+    (e.g. an HDF5 file)"""
+
     @abstractmethod
     async def open(self, multiplier: int = 1) -> Dict[str, Descriptor]:
         """Open writer and wait for it to be ready for data.
 
         Args:
             multiplier: Each StreamDatum index corresponds to this many
                 written exposures
@@ -96,66 +121,67 @@
             Output for ``describe()``
         """
 
     @abstractmethod
     def observe_indices_written(
         self, timeout=DEFAULT_TIMEOUT
     ) -> AsyncGenerator[int, None]:
-        """Yield each index as it is written"""
+        """Yield the index of each frame (or equivalent data point) as it is written"""
 
     @abstractmethod
     async def get_indices_written(self) -> int:
         """Get the number of indices written"""
 
     @abstractmethod
     def collect_stream_docs(self, indices_written: int) -> AsyncIterator[StreamAsset]:
         """Create Stream docs up to given number written"""
 
     @abstractmethod
     async def close(self) -> None:
-        """Close writer and wait for it to be finished"""
+        """Close writer, blocks until I/O is complete"""
 
 
 class StandardDetector(
     Device,
     Stageable,
-    Configurable,
-    Readable,
+    AsyncConfigurable,
+    AsyncReadable,
     Triggerable,
     Preparable,
     Flyable,
     Collectable,
     WritesStreamAssets,
+    Generic[T],
 ):
-    """Detector with useful step and flyscan behaviour.
-
-    Must be supplied instances of classes that inherit from DetectorControl and
-    DetectorData, to dictate how the detector will be controlled (i.e. arming and
-    disarming) as well as how the detector data will be written (i.e. opening and
-    closing the writer, and handling data writing indices).
-
+    """
+    Useful detector base class for step and fly scanning detectors.
+    Aggregates controller and writer logic together.
     """
 
     def __init__(
         self,
         controller: DetectorControl,
         writer: DetectorWriter,
         config_sigs: Sequence[SignalR] = (),
         name: str = "",
         writer_timeout: float = DEFAULT_TIMEOUT,
     ) -> None:
         """
-        Parameters
-        ----------
-        control:
-            instance of class which inherits from :class:`DetectorControl`
-        data:
-            instance of class which inherits from :class:`DetectorData`
-        name:
-            detector name
+        Constructor
+
+        Args:
+            controller: Logic for arming and disarming the detector
+            writer: Logic for making the detector write persistent data
+            config_sigs: Signals to read when describe and read
+            configuration are called. Defaults to ().
+            name: Device name. Defaults to "".
+            writer_timeout: Timeout for frame writing to start, if the
+            timeout is reached, ophyd-async assumes the detector
+            has a problem and raises an error.
+            Defaults to DEFAULT_TIMEOUT.
         """
         self._controller = controller
         self._writer = writer
         self._describe: Dict[str, Descriptor] = {}
         self._config_sigs = list(config_sigs)
         self._frame_writing_timeout = writer_timeout
         # For prepare
@@ -176,20 +202,20 @@
 
     @property
     def writer(self) -> DetectorWriter:
         return self._writer
 
     @AsyncStatus.wrap
     async def stage(self) -> None:
-        """Disarm the detector, stop filewriting, and open file for writing."""
-        await self.check_config_sigs()
+        # Disarm the detector, stop filewriting, and open file for writing.
+        await self._check_config_sigs()
         await asyncio.gather(self.writer.close(), self.controller.disarm())
         self._describe = await self.writer.open()
 
-    async def check_config_sigs(self):
+    async def _check_config_sigs(self):
         """Checks configuration signals are named and connected."""
         for signal in self._config_sigs:
             if signal._name == "":
                 raise Exception(
                     "config signal must be named before it is passed to the detector"
                 )
             try:
@@ -198,34 +224,33 @@
                 raise Exception(
                     f"config signal {signal._name} must be connected before it is "
                     + "passed to the detector"
                 )
 
     @AsyncStatus.wrap
     async def unstage(self) -> None:
-        """Stop data writing."""
+        # Stop data writing.
         await self.writer.close()
 
     async def read_configuration(self) -> Dict[str, Reading]:
         return await merge_gathered_dicts(sig.read() for sig in self._config_sigs)
 
     async def describe_configuration(self) -> Dict[str, Descriptor]:
         return await merge_gathered_dicts(sig.describe() for sig in self._config_sigs)
 
     async def read(self) -> Dict[str, Reading]:
-        """Read the detector"""
         # All data is in StreamResources, not Events, so nothing to output here
         return {}
 
-    def describe(self) -> Dict[str, Descriptor]:
+    async def describe(self) -> Dict[str, Descriptor]:
         return self._describe
 
     @AsyncStatus.wrap
     async def trigger(self) -> None:
-        """Arm the detector and wait for it to finish."""
+        # Arm the detector and wait for it to finish.
         indices_written = await self.writer.get_indices_written()
         written_status = await self.controller.arm(
             num=1,
             trigger=DetectorTrigger.internal,
         )
         await written_status
         end_observation = indices_written + 1
@@ -236,27 +261,31 @@
             if index >= end_observation:
                 break
 
     def prepare(
         self,
         value: T,
     ) -> AsyncStatus:
-        """Arm detector"""
+        # Just arm detector for the time being
         return AsyncStatus(self._prepare(value))
 
     async def _prepare(self, value: T) -> None:
-        """Arm detector.
+        """
+        Arm detector.
 
         Prepare the detector with trigger information. This is determined at and passed
         in from the plan level.
 
         This currently only prepares detectors for flyscans and stepscans just use the
         trigger information determined in trigger.
 
         To do: Unify prepare to be use for both fly and step scans.
+
+        Args:
+            value: TriggerInfo describing how to trigger the detector
         """
         assert type(value) is TriggerInfo
         self._trigger_info = value
         self._initial_frame = await self.writer.get_indices_written()
         self._last_frame = self._initial_frame + self._trigger_info.num
 
         required = self.controller.get_deadtime(self._trigger_info.livetime)
@@ -303,19 +332,17 @@
 
     async def describe_collect(self) -> Dict[str, Descriptor]:
         return self._describe
 
     async def collect_asset_docs(
         self, index: Optional[int] = None
     ) -> AsyncIterator[StreamAsset]:
-        """Collect stream datum documents for all indices written.
-
-        The index is optional, and provided for flyscans, however this needs to be
-        retrieved for stepscans.
-        """
+        # Collect stream datum documents for all indices written.
+        # The index is optional, and provided for fly scans, however this needs to be
+        # retrieved for step scans.
         if not index:
             index = await self.writer.get_indices_written()
         async for doc in self.writer.collect_stream_docs(index):
             yield doc
 
     async def get_index(self) -> int:
         return await self.writer.get_indices_written()
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/device.py` & `ophyd_async-0.3a2/src/ophyd_async/core/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,22 @@
             await wait_for_connection(**coros)
 
 
 VT = TypeVar("VT", bound=Device)
 
 
 class DeviceVector(Dict[int, VT], Device):
+    """
+    Defines device components with indices.
+
+    In the below example, foos becomes a dictionary on the parent device
+    at runtime, so parent.foos[2] returns a FooDevice. For example usage see
+    :class:`~ophyd_async.epics.demo.DynamicSensorGroup`
+    """
+
     def children(self) -> Generator[Tuple[str, Device], None, None]:
         for attr_name, attr in self.items():
             if isinstance(attr, Device):
                 yield str(attr_name), attr
 
 
 class DeviceCollector:
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/device_save_loader.py` & `ophyd_async-0.3a2/src/ophyd_async/core/device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/flyer.py` & `ophyd_async-0.3a2/src/ophyd_async/core/flyer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from abc import ABC, abstractmethod
-from typing import Dict, Generic, Optional, Sequence, TypeVar
+from typing import Dict, Generic, Sequence, TypeVar
 
 from bluesky.protocols import Descriptor, Flyable, Preparable, Reading, Stageable
 
 from .async_status import AsyncStatus
-from .detector import TriggerInfo
 from .device import Device
 from .signal import SignalR
 from .utils import merge_gathered_dicts
 
 T = TypeVar("T")
 
 
 class TriggerLogic(ABC, Generic[T]):
     @abstractmethod
-    def trigger_info(self, value: T) -> TriggerInfo:
-        """Return info about triggers that will be produced for a given value"""
-
-    @abstractmethod
     async def prepare(self, value: T):
         """Move to the start of the flyscan"""
 
     @abstractmethod
-    async def start(self):
+    async def kickoff(self):
         """Start the flyscan"""
 
     @abstractmethod
+    async def complete(self):
+        """Block until the flyscan is done"""
+
+    @abstractmethod
     async def stop(self):
         """Stop flying and wait everything to be stopped"""
 
 
 class HardwareTriggeredFlyable(
     Device,
     Stageable,
@@ -41,51 +40,43 @@
         self,
         trigger_logic: TriggerLogic[T],
         configuration_signals: Sequence[SignalR],
         name: str = "",
     ):
         self._trigger_logic = trigger_logic
         self._configuration_signals = tuple(configuration_signals)
-        self._describe: Dict[str, Descriptor] = {}
-        self._fly_status: Optional[AsyncStatus] = None
-        self._trigger_info: Optional[TriggerInfo] = None
         super().__init__(name=name)
 
     @property
     def trigger_logic(self) -> TriggerLogic[T]:
         return self._trigger_logic
 
-    @property
-    def trigger_info(self) -> Optional[TriggerInfo]:
-        return self._trigger_info
-
     @AsyncStatus.wrap
     async def stage(self) -> None:
         await self.unstage()
 
     @AsyncStatus.wrap
     async def unstage(self) -> None:
         await self._trigger_logic.stop()
 
     def prepare(self, value: T) -> AsyncStatus:
         """Setup trajectories"""
         return AsyncStatus(self._prepare(value))
 
     async def _prepare(self, value: T) -> None:
-        self._trigger_info = self._trigger_logic.trigger_info(value)
         # Move to start and setup the flyscan
         await self._trigger_logic.prepare(value)
 
     @AsyncStatus.wrap
     async def kickoff(self) -> None:
-        self._fly_status = AsyncStatus(self._trigger_logic.start())
+        await self._trigger_logic.kickoff()
 
-    def complete(self) -> AsyncStatus:
-        assert self._fly_status, "Kickoff not run"
-        return self._fly_status
+    @AsyncStatus.wrap
+    async def complete(self) -> None:
+        await self._trigger_logic.complete()
 
     async def describe_configuration(self) -> Dict[str, Descriptor]:
         return await merge_gathered_dicts(
             [sig.describe() for sig in self._configuration_signals]
         )
 
     async def read_configuration(self) -> Dict[str, Reading]:
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/signal.py` & `ophyd_async-0.3a2/src/ophyd_async/core/signal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 import asyncio
 import functools
-from typing import AsyncGenerator, Callable, Dict, Generic, Optional, Union
+from typing import AsyncGenerator, Callable, Dict, Generic, Optional, Tuple, Type, Union
 
 from bluesky.protocols import (
     Descriptor,
     Locatable,
     Location,
     Movable,
-    Readable,
     Reading,
     Stageable,
     Subscribable,
 )
 
+from ophyd_async.protocols import AsyncReadable
+
 from .async_status import AsyncStatus
 from .device import Device
 from .signal_backend import SignalBackend
 from .sim_signal_backend import SimSignalBackend
 from .utils import DEFAULT_TIMEOUT, Callback, ReadingValueCallback, T
 
 _sim_backends: Dict[Signal, SimSignalBackend] = {}
@@ -41,42 +42,36 @@
         return NotImplemented
 
 
 class Signal(Device, Generic[T]):
     """A Device with the concept of a value, with R, RW, W and X flavours"""
 
     def __init__(
-        self, backend: SignalBackend[T], timeout: Optional[float] = DEFAULT_TIMEOUT
+        self,
+        backend: SignalBackend[T],
+        timeout: Optional[float] = DEFAULT_TIMEOUT,
+        name: str = "",
     ) -> None:
-        self._name = ""
+        super().__init__(name)
         self._timeout = timeout
         self._init_backend = self._backend = backend
 
-    @property
-    def name(self) -> str:
-        return self._name
-
-    def set_name(self, name: str = ""):
-        self._name = name
-
     async def connect(self, sim=False, timeout=DEFAULT_TIMEOUT):
         if sim:
-            self._backend = SimSignalBackend(
-                datatype=self._init_backend.datatype, source=self._init_backend.source
-            )
+            self._backend = SimSignalBackend(datatype=self._init_backend.datatype)
             _sim_backends[self] = self._backend
         else:
             self._backend = self._init_backend
             _sim_backends.pop(self, None)
         await self._backend.connect(timeout=timeout)
 
     @property
     def source(self) -> str:
         """Like ca://PV_PREFIX:SIGNAL, or "" if not set"""
-        return self._backend.source
+        return self._backend.source(self.name)
 
     __lt__ = __le__ = __eq__ = __ge__ = __gt__ = __ne__ = _fail
 
     def __hash__(self):
         # Restore the default implementation so we can use in a set or dict
         return hash(id(self))
 
@@ -129,15 +124,15 @@
         return self._staged or bool(self._listeners)
 
     def set_staged(self, staged: bool):
         self._staged = staged
         return self._staged or bool(self._listeners)
 
 
-class SignalR(Signal[T], Readable, Stageable, Subscribable):
+class SignalR(Signal[T], AsyncReadable, Stageable, Subscribable):
     """Signal that can be read from and monitored"""
 
     _cache: Optional[_SignalCache] = None
 
     def _backend_or_cache(
         self, cached: Optional[bool]
     ) -> Union[_SignalCache, SignalBackend]:
@@ -164,15 +159,15 @@
     async def read(self, cached: Optional[bool] = None) -> Dict[str, Reading]:
         """Return a single item dict with the reading in it"""
         return {self.name: await self._backend_or_cache(cached).get_reading()}
 
     @_add_timeout
     async def describe(self) -> Dict[str, Descriptor]:
         """Return a single item dict with the descriptor in it"""
-        return {self.name: await self._backend.get_descriptor()}
+        return {self.name: await self._backend.get_descriptor(self.source)}
 
     @_add_timeout
     async def get_value(self, cached: Optional[bool] = None) -> T:
         """The current value"""
         return await self._backend_or_cache(cached).get_value()
 
     def subscribe_value(self, function: Callback[T]):
@@ -249,14 +244,38 @@
 
 
 def set_sim_callback(signal: Signal[T], callback: ReadingValueCallback[T]) -> None:
     """Monitor the value of a signal that is in sim mode"""
     return _sim_backends[signal].set_callback(callback)
 
 
+def soft_signal_rw(
+    datatype: Optional[Type[T]] = None,
+    initial_value: Optional[T] = None,
+    name: str = "",
+) -> SignalRW[T]:
+    """Creates a read-writable Signal with a SimSignalBackend"""
+    signal = SignalRW(SimSignalBackend(datatype, initial_value), name=name)
+    return signal
+
+
+def soft_signal_r_and_backend(
+    datatype: Optional[Type[T]] = None,
+    initial_value: Optional[T] = None,
+    name: str = "",
+) -> Tuple[SignalR[T], SimSignalBackend]:
+    """Returns a tuple of a read-only Signal and its SimSignalBackend through
+    which the signal can be internally modified within the device. Use
+    soft_signal_rw if you want a device that is externally modifiable
+    """
+    backend = SimSignalBackend(datatype, initial_value)
+    signal = SignalR(backend, name=name)
+    return (signal, backend)
+
+
 async def observe_value(signal: SignalR[T], timeout=None) -> AsyncGenerator[T, None]:
     """Subscribe to the value of a signal so it can be iterated from.
 
     Parameters
     ----------
     signal:
         Call subscribe_value on this at the start, and clear_sub on it at the
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/signal_backend.py` & `ophyd_async-0.3a2/src/ophyd_async/core/signal_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 class SignalBackend(Generic[T]):
     """A read/write/monitor backend for a Signals"""
 
     #: Datatype of the signal value
     datatype: Optional[Type[T]] = None
 
     #: Like ca://PV_PREFIX:SIGNAL
-    source: str = ""
+    @abstractmethod
+    def source(name: str) -> str:
+        """Return source of signal. Signals may pass a name to the backend, which can be
+        used or discarded."""
 
     @abstractmethod
     async def connect(self, timeout: float = DEFAULT_TIMEOUT):
         """Connect to underlying hardware"""
 
     @abstractmethod
     async def put(self, value: Optional[T], wait=True, timeout=None):
         """Put a value to the PV, if wait then wait for completion for up to timeout"""
 
     @abstractmethod
-    async def get_descriptor(self) -> Descriptor:
+    async def get_descriptor(self, source: str) -> Descriptor:
         """Metadata like source, dtype, shape, precision, units"""
 
     @abstractmethod
     async def get_reading(self) -> Reading:
         """The current value, timestamp and severity"""
 
     @abstractmethod
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/sim_signal_backend.py` & `ophyd_async-0.3a2/src/ophyd_async/core/sim_signal_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import asyncio
 import inspect
-import re
 import time
 from collections import abc
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, Generic, Optional, Type, Union, cast, get_origin
 
+import numpy as np
 from bluesky.protocols import Descriptor, Dtype, Reading
 
 from .signal_backend import SignalBackend
 from .utils import DEFAULT_TIMEOUT, ReadingValueCallback, T, get_dtype
 
 primitive_dtypes: Dict[type, Dtype] = {
     str: "string",
@@ -33,30 +33,35 @@
         return Reading(
             value=value,
             timestamp=timestamp,
             alarm_severity=-1 if severity > 2 else severity,
         )
 
     def descriptor(self, source: str, value) -> Descriptor:
+        dtype = type(value)
+        if np.issubdtype(dtype, np.integer):
+            dtype = int
+        elif np.issubdtype(dtype, np.floating):
+            dtype = float
         assert (
-            type(value) in primitive_dtypes
+            dtype in primitive_dtypes
         ), f"invalid converter for value of type {type(value)}"
-        dtype = primitive_dtypes[type(value)]
-        return dict(source=source, dtype=dtype, shape=[])
+        dtype_name = primitive_dtypes[dtype]
+        return {"source": source, "dtype": dtype_name, "shape": []}
 
     def make_initial_value(self, datatype: Optional[Type[T]]) -> T:
         if datatype is None:
             return cast(T, None)
 
         return datatype()
 
 
 class SimArrayConverter(SimConverter):
     def descriptor(self, source: str, value) -> Descriptor:
-        return dict(source=source, dtype="array", shape=[len(value)])
+        return {"source": source, "dtype": "array", "shape": [len(value)]}
 
     def make_initial_value(self, datatype: Optional[Type[T]]) -> T:
         if datatype is None:
             return cast(T, None)
 
         if get_origin(datatype) == abc.Sequence:
             return cast(T, [])
@@ -72,17 +77,15 @@
         if isinstance(value, Enum):
             return value
         else:
             return self.enum_class(value)
 
     def descriptor(self, source: str, value) -> Descriptor:
         choices = [e.value for e in self.enum_class]
-        return dict(
-            source=source, dtype="string", shape=[], choices=choices
-        )  # type: ignore
+        return {"source": source, "dtype": "string", "shape": [], "choices": choices}  # type: ignore
 
     def make_initial_value(self, datatype: Optional[Type[T]]) -> T:
         if datatype is None:
             return cast(T, None)
 
         return cast(T, list(datatype.__members__.values())[0])  # type: ignore
 
@@ -105,31 +108,40 @@
     return SimConverter()
 
 
 class SimSignalBackend(SignalBackend[T]):
     """An simulated backend to a Signal, created with ``Signal.connect(sim=True)``"""
 
     _value: T
-    _initial_value: T
+    _initial_value: Optional[T]
     _timestamp: float
     _severity: int
 
-    def __init__(self, datatype: Optional[Type[T]], source: str) -> None:
-        pv = re.split(r"://", source)[-1]
-        self.source = f"sim://{pv}"
+    def __init__(
+        self,
+        datatype: Optional[Type[T]],
+        initial_value: Optional[T] = None,
+    ) -> None:
         self.datatype = datatype
-        self.pv = source
         self.converter: SimConverter = DisconnectedSimConverter()
+        self._initial_value = initial_value
         self.put_proceeds = asyncio.Event()
         self.put_proceeds.set()
         self.callback: Optional[ReadingValueCallback[T]] = None
 
+    def source(self, name: str) -> str:
+        return f"soft://{name}"
+
     async def connect(self, timeout: float = DEFAULT_TIMEOUT) -> None:
         self.converter = make_converter(self.datatype)
-        self._initial_value = self.converter.make_initial_value(self.datatype)
+        if self._initial_value is None:
+            self._initial_value = self.converter.make_initial_value(self.datatype)
+        else:
+            # convert potentially unconverted initial value passed to init method
+            self._initial_value = self.converter.write_value(self._initial_value)
         self._severity = 0
 
         await self.put(None)
 
     async def put(self, value: Optional[T], wait=True, timeout=None):
         write_value = (
             self.converter.write_value(value)
@@ -148,16 +160,16 @@
         reading: Reading = self.converter.reading(
             self._value, self._timestamp, self._severity
         )
 
         if self.callback:
             self.callback(reading, self._value)
 
-    async def get_descriptor(self) -> Descriptor:
-        return self.converter.descriptor(self.source, self._value)
+    async def get_descriptor(self, source: str) -> Descriptor:
+        return self.converter.descriptor(source, self._value)
 
     async def get_reading(self) -> Reading:
         return self.converter.reading(self._value, self._timestamp, self._severity)
 
     async def get_value(self) -> T:
         return self.converter.value(self._value)
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/standard_readable.py` & `ophyd_async-0.3a2/src/ophyd_async/core/standard_readable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Dict, Sequence, Tuple
 
-from bluesky.protocols import Configurable, Descriptor, Readable, Reading, Stageable
+from bluesky.protocols import Descriptor, Reading, Stageable
+
+from ophyd_async.protocols import AsyncConfigurable, AsyncReadable
 
 from .async_status import AsyncStatus
 from .device import Device
 from .signal import SignalR
 from .utils import merge_gathered_dicts
 
 
-class StandardReadable(Device, Readable, Configurable, Stageable):
+class StandardReadable(Device, AsyncReadable, AsyncConfigurable, Stageable):
     """Device that owns its children and provides useful default behavior.
 
     - When its name is set it renames child Devices
     - Signals can be registered for read() and read_configuration()
     - These signals will be subscribed for read() between stage() and unstage()
     """
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/core/utils.py` & `ophyd_async-0.3a2/src/ophyd_async/core/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     if len(set_values) != 1:
         diffs = ", ".join(f"{k} has {v}" for k, v in values.items())
         raise TypeError(f"Differing {types}: {diffs}")
     return set_values.pop()
 
 
 async def merge_gathered_dicts(
-    coros: Iterable[Awaitable[Dict[str, T]]]
+    coros: Iterable[Awaitable[Dict[str, T]]],
 ) -> Dict[str, T]:
     """Merge dictionaries produced by a sequence of coroutines.
 
     Can be used for merging ``read()`` or ``describe``. For instance::
 
         combined_read = await merge_gathered_dicts(s.read() for s in signals)
     """
@@ -144,7 +144,24 @@
     for result in await asyncio.gather(*coros):
         ret.update(result)
     return ret
 
 
 async def gather_list(coros: Iterable[Awaitable[T]]) -> List[T]:
     return await asyncio.gather(*coros)
+
+
+def in_micros(t: float) -> int:
+    """
+    Converts between a positive number of seconds and an equivalent
+    number of microseconds.
+
+    Args:
+        t (float): A time in seconds
+    Raises:
+        ValueError: if t < 0
+    Returns:
+        t (int): A time in microseconds, rounded up to the nearest whole microsecond,
+    """
+    if t < 0:
+        raise ValueError(f"Expected a positive time in seconds, got {t!r}")
+    return int(np.ceil(t * 1e6))
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/_backend/_aioca.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/_backend/_aioca.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,37 +48,37 @@
     def write_value(self, value) -> Any:
         return value
 
     def value(self, value: AugmentedValue):
         return value
 
     def reading(self, value: AugmentedValue):
-        return dict(
-            value=self.value(value),
-            timestamp=value.timestamp,
-            alarm_severity=-1 if value.severity > 2 else value.severity,
-        )
+        return {
+            "value": self.value(value),
+            "timestamp": value.timestamp,
+            "alarm_severity": -1 if value.severity > 2 else value.severity,
+        }
 
     def descriptor(self, source: str, value: AugmentedValue) -> Descriptor:
-        return dict(source=source, dtype=dbr_to_dtype[value.datatype], shape=[])
+        return {"source": source, "dtype": dbr_to_dtype[value.datatype], "shape": []}
 
 
 class CaLongStrConverter(CaConverter):
     def __init__(self):
         return super().__init__(dbr.DBR_CHAR_STR, dbr.DBR_CHAR_STR)
 
     def write_value(self, value: str):
         # Add a null in here as this is what the commandline caput does
         # TODO: this should be in the server so check if it can be pushed to asyn
         return value + "\0"
 
 
 class CaArrayConverter(CaConverter):
     def descriptor(self, source: str, value: AugmentedValue) -> Descriptor:
-        return dict(source=source, dtype="array", shape=[len(value)])
+        return {"source": source, "dtype": "array", "shape": [len(value)]}
 
 
 @dataclass
 class CaEnumConverter(CaConverter):
     enum_class: Type[Enum]
 
     def write_value(self, value: Union[Enum, str]):
@@ -88,15 +88,15 @@
             return value
 
     def value(self, value: AugmentedValue):
         return self.enum_class(value)
 
     def descriptor(self, source: str, value: AugmentedValue) -> Descriptor:
         choices = [e.value for e in self.enum_class]
-        return dict(source=source, dtype="string", shape=[], choices=choices)
+        return {"source": source, "dtype": "string", "shape": [], "choices": choices}
 
 
 class DisconnectedCaConverter(CaConverter):
     def __getattribute__(self, __name: str) -> Any:
         raise NotImplementedError("No PV has been set as connect() has not been called")
 
 
@@ -166,17 +166,19 @@
 class CaSignalBackend(SignalBackend[T]):
     def __init__(self, datatype: Optional[Type[T]], read_pv: str, write_pv: str):
         self.datatype = datatype
         self.read_pv = read_pv
         self.write_pv = write_pv
         self.initial_values: Dict[str, AugmentedValue] = {}
         self.converter: CaConverter = DisconnectedCaConverter(None, None)
-        self.source = f"ca://{self.read_pv}"
         self.subscription: Optional[Subscription] = None
 
+    def source(self, name: str):
+        return f"ca://{self.read_pv}"
+
     async def _store_initial_value(self, pv, timeout: float = DEFAULT_TIMEOUT):
         try:
             self.initial_values[pv] = await caget(
                 pv, format=FORMAT_CTRL, timeout=timeout
             )
         except CANothing as exc:
             logging.debug(f"signal ca://{pv} timed out")
@@ -212,17 +214,17 @@
         return await caget(
             self.read_pv,
             datatype=self.converter.read_dbr,
             format=format,
             timeout=None,
         )
 
-    async def get_descriptor(self) -> Descriptor:
+    async def get_descriptor(self, source: str) -> Descriptor:
         value = await self._caget(FORMAT_CTRL)
-        return self.converter.descriptor(self.source, value)
+        return self.converter.descriptor(source, value)
 
     async def get_reading(self) -> Reading:
         value = await self._caget(FORMAT_TIME)
         return self.converter.reading(value)
 
     async def get_value(self) -> T:
         value = await self._caget(FORMAT_RAW)
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/_backend/_p4p.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/_backend/_p4p.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,23 +45,23 @@
 
     def value(self, value):
         return value["value"]
 
     def reading(self, value):
         ts = value["timeStamp"]
         sv = value["alarm"]["severity"]
-        return dict(
-            value=self.value(value),
-            timestamp=ts["secondsPastEpoch"] + ts["nanoseconds"] * 1e-9,
-            alarm_severity=-1 if sv > 2 else sv,
-        )
+        return {
+            "value": self.value(value),
+            "timestamp": ts["secondsPastEpoch"] + ts["nanoseconds"] * 1e-9,
+            "alarm_severity": -1 if sv > 2 else sv,
+        }
 
     def descriptor(self, source: str, value) -> Descriptor:
         dtype = specifier_to_dtype[value.type().aspy("value")]
-        return dict(source=source, dtype=dtype, shape=[])
+        return {"source": source, "dtype": dtype, "shape": []}
 
     def metadata_fields(self) -> List[str]:
         """
         Fields to request from PVA for metadata.
         """
         return ["alarm", "timeStamp"]
 
@@ -70,15 +70,15 @@
         Fields to request from PVA for the value.
         """
         return ["value"]
 
 
 class PvaArrayConverter(PvaConverter):
     def descriptor(self, source: str, value) -> Descriptor:
-        return dict(source=source, dtype="array", shape=[len(value["value"])])
+        return {"source": source, "dtype": "array", "shape": [len(value["value"])]}
 
 
 class PvaNDArrayConverter(PvaConverter):
     def metadata_fields(self) -> List[str]:
         return super().metadata_fields() + ["dimension"]
 
     def _get_dimensions(self, value) -> List[int]:
@@ -94,15 +94,15 @@
 
     def value(self, value):
         dims = self._get_dimensions(value)
         return value["value"].reshape(dims)
 
     def descriptor(self, source: str, value) -> Descriptor:
         dims = self._get_dimensions(value)
-        return dict(source=source, dtype="array", shape=dims)
+        return {"source": source, "dtype": "array", "shape": dims}
 
     def write_value(self, value):
         # No clear use-case for writing directly to an NDArray, and some
         # complexities around flattening to 1-D - e.g. dimension-order.
         # Don't support this for now.
         raise TypeError("Writing to NDArray not supported")
 
@@ -118,40 +118,40 @@
             return value
 
     def value(self, value):
         return list(self.enum_class)[value["value"]["index"]]
 
     def descriptor(self, source: str, value) -> Descriptor:
         choices = [e.value for e in self.enum_class]
-        return dict(source=source, dtype="string", shape=[], choices=choices)
+        return {"source": source, "dtype": "string", "shape": [], "choices": choices}
 
 
 class PvaEnumBoolConverter(PvaConverter):
     def value(self, value):
         return value["value"]["index"]
 
     def descriptor(self, source: str, value) -> Descriptor:
-        return dict(source=source, dtype="integer", shape=[])
+        return {"source": source, "dtype": "integer", "shape": []}
 
 
 class PvaTableConverter(PvaConverter):
     def value(self, value):
         return value["value"].todict()
 
     def descriptor(self, source: str, value) -> Descriptor:
         # This is wrong, but defer until we know how to actually describe a table
-        return dict(source=source, dtype="object", shape=[])  # type: ignore
+        return {"source": source, "dtype": "object", "shape": []}  # type: ignore
 
 
 class PvaDictConverter(PvaConverter):
     def reading(self, value):
         ts = time.time()
         value = value.todict()
         # Alarm severity is vacuously 0 for a table
-        return dict(value=value, timestamp=ts, alarm_severity=0)
+        return {"value": value, "timestamp": ts, "alarm_severity": 0}
 
     def value(self, value: Value):
         return value.todict()
 
     def descriptor(self, source: str, value) -> Descriptor:
         raise NotImplementedError("Describing Dict signals not currently supported")
 
@@ -232,18 +232,21 @@
 
     def __init__(self, datatype: Optional[Type[T]], read_pv: str, write_pv: str):
         self.datatype = datatype
         self.read_pv = read_pv
         self.write_pv = write_pv
         self.initial_values: Dict[str, Any] = {}
         self.converter: PvaConverter = DisconnectedPvaConverter()
-        self.source = f"pva://{self.read_pv}"
         self.subscription: Optional[Subscription] = None
 
     @property
+    def source(self, name: str):
+        return f"pva://{self.read_pv}"
+
+    @property
     def ctxt(self) -> Context:
         if PvaSignalBackend._ctxt is None:
             PvaSignalBackend._ctxt = Context("pva", nt=False)
 
             @atexit.register
             def _del_ctxt():
                 # If we don't do this we get messages like this on close:
@@ -275,28 +278,28 @@
         self.converter = make_converter(self.datatype, self.initial_values)
 
     async def put(self, value: Optional[T], wait=True, timeout=None):
         if value is None:
             write_value = self.initial_values[self.write_pv]
         else:
             write_value = self.converter.write_value(value)
-        coro = self.ctxt.put(self.write_pv, dict(value=write_value), wait=wait)
+        coro = self.ctxt.put(self.write_pv, {"value": write_value}, wait=wait)
         try:
             await asyncio.wait_for(coro, timeout)
         except asyncio.TimeoutError as exc:
             logging.debug(
                 f"signal pva://{self.write_pv} timed out \
                           put value: {write_value}",
                 exc_info=True,
             )
             raise NotConnected(f"pva://{self.write_pv}") from exc
 
-    async def get_descriptor(self) -> Descriptor:
+    async def get_descriptor(self, source: str) -> Descriptor:
         value = await self.ctxt.get(self.read_pv)
-        return self.converter.descriptor(self.source, value)
+        return self.converter.descriptor(source, value)
 
     def _pva_request_string(self, fields: List[str]) -> str:
         """
         Converts a list of requested fields into a PVA request string which can be
         passed to p4p.
         """
         return f"field({','.join(fields)})"
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/_backend/common.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/_backend/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 
 
 def get_supported_enum_class(
     pv: str,
     datatype: Optional[Type[Enum]],
     pv_choices: Tuple[Any, ...],
 ) -> Type[Enum]:
-    if datatype:
-        if not issubclass(datatype, Enum):
-            raise TypeError(f"{pv} has type Enum not {datatype.__name__}")
-        if not issubclass(datatype, str):
-            raise TypeError(f"{pv} has type Enum but doesn't inherit from String")
-        choices = tuple(v.value for v in datatype)
-        if set(choices).difference(pv_choices):
-            raise TypeError(f"{pv} has choices {pv_choices}: not all in {choices}")
-    return Enum(
-        "GeneratedChoices", {x or "_": x for x in pv_choices}, type=str
-    )  # type: ignore
+    if not datatype:
+        return Enum("GeneratedChoices", {x or "_": x for x in pv_choices}, type=str)  # type: ignore
+
+    if not issubclass(datatype, Enum):
+        raise TypeError(f"{pv} has type Enum not {datatype.__name__}")
+    if not issubclass(datatype, str):
+        raise TypeError(f"{pv} has type Enum but doesn't inherit from String")
+    choices = tuple(v.value for v in datatype)
+    if set(choices) != set(pv_choices):
+        raise TypeError(
+            (
+                f"{pv} has choices {pv_choices}, "
+                f"which do not match {datatype}, which has {choices}"
+            )
+        )
+    return datatype
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py` & `ophyd_async-0.3a2/tests/epics/areadetector/test_drivers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 import asyncio
-from typing import Optional, Set
 
-from ophyd_async.core import AsyncStatus, DetectorControl, DetectorTrigger
-from ophyd_async.epics.areadetector.drivers.ad_base import (
-    DEFAULT_GOOD_STATES,
+import pytest
+
+from ophyd_async.core import DeviceCollector, set_sim_value
+from ophyd_async.epics.areadetector.drivers import (
+    ADBase,
     DetectorState,
     start_acquiring_driver_and_ensure_status,
 )
 
-from ..drivers.pilatus_driver import PilatusDriver, TriggerMode
-from ..utils import ImageMode, stop_busy_record
 
-TRIGGER_MODE = {
-    DetectorTrigger.internal: TriggerMode.internal,
-    DetectorTrigger.constant_gate: TriggerMode.ext_enable,
-    DetectorTrigger.variable_gate: TriggerMode.ext_enable,
-}
-
-
-class PilatusController(DetectorControl):
-    def __init__(
-        self,
-        driver: PilatusDriver,
-        good_states: Set[DetectorState] = set(DEFAULT_GOOD_STATES),
-    ) -> None:
-        self.driver = driver
-        self.good_states = good_states
-
-    def get_deadtime(self, exposure: float) -> float:
-        return 0.001
-
-    async def arm(
-        self,
-        num: int,
-        trigger: DetectorTrigger = DetectorTrigger.internal,
-        exposure: Optional[float] = None,
-    ) -> AsyncStatus:
-        await asyncio.gather(
-            self.driver.trigger_mode.set(TRIGGER_MODE[trigger]),
-            self.driver.num_images.set(999_999 if num == 0 else num),
-            self.driver.image_mode.set(ImageMode.multiple),
-        )
-        return await start_acquiring_driver_and_ensure_status(
-            self.driver, good_states=self.good_states
-        )
+@pytest.fixture
+def driver(RE) -> ADBase:
+    with DeviceCollector(sim=True):
+        driver = ADBase("DRV:", name="drv")
+    return driver
+
+
+async def test_start_acquiring_driver_and_ensure_status_flags_immediate_failure(
+    driver: ADBase,
+):
+    set_sim_value(driver.detector_state, DetectorState.Error)
+    acquiring = await start_acquiring_driver_and_ensure_status(driver, timeout=0.01)
+    with pytest.raises(ValueError):
+        await acquiring
+
+
+async def test_start_acquiring_driver_and_ensure_status_fails_after_some_time(
+    driver: ADBase,
+):
+    """This test ensures a failing status is captured halfway through acquisition.
+
+    Real world application; it takes some time to start acquiring, and during that time
+    the detector gets itself into a bad state.
+    """
+    set_sim_value(driver.detector_state, DetectorState.Idle)
+
+    async def wait_then_fail():
+        await asyncio.sleep(0)
+        set_sim_value(driver.detector_state, DetectorState.Disconnected)
+
+    acquiring = await start_acquiring_driver_and_ensure_status(driver, timeout=0.1)
+    await wait_then_fail()
 
-    async def disarm(self):
-        await stop_busy_record(self.driver.acquire, False, timeout=1)
+    with pytest.raises(ValueError):
+        await acquiring
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/drivers/ad_base.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/drivers/ad_base.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/single_trigger_det.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/single_trigger_det.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/utils.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/_hdffile.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/_hdffile.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def stream_resources(self) -> Iterator[StreamResource]:
         for bundle in self._bundles:
             yield bundle.stream_resource_doc
 
     def stream_data(self, indices_written: int) -> Iterator[StreamDatum]:
         # Indices are relative to resource
         if indices_written > self._last_emitted:
-            indices = dict(
-                start=self._last_emitted,
-                stop=indices_written,
-            )
+            indices = {
+                "start": self._last_emitted,
+                "stop": indices_written,
+            }
             self._last_emitted = indices_written
             for bundle in self._bundles:
                 yield bundle.compose_stream_datum(indices)
         return None
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/hdf_writer.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/hdf_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -105,20 +105,25 @@
     async def collect_stream_docs(
         self, indices_written: int
     ) -> AsyncIterator[StreamAsset]:
         # TODO: fail if we get dropped frames
         await self.hdf.flush_now.set(True)
         if indices_written:
             if not self._file:
+                path = Path(await self.hdf.full_file_name.get_value())
                 self._file = _HDFFile(
                     self._directory_provider(),
                     # See https://github.com/bluesky/ophyd-async/issues/122
-                    Path(await self.hdf.full_file_name.get_value()),
+                    path,
                     self._datasets,
                 )
+                # stream resource says "here is a dataset",
+                # stream datum says "here are N frames in that stream resource",
+                # you get one stream resource and many stream datums per scan
+
                 for doc in self._file.stream_resources():
                     yield "stream_resource", doc
             for doc in self._file.stream_data(indices_written):
                 yield "stream_datum", doc
 
     async def close(self):
         # Already done a caput callback in _capture_status, so can't do one here
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/areadetector/writers/nd_plugin.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/areadetector/writers/nd_plugin.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/demo/__init__.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/demo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 from enum import Enum
 from pathlib import Path
 from typing import Callable, List, Optional
 
 import numpy as np
 from bluesky.protocols import Movable, Stoppable
 
-from ophyd_async.core import AsyncStatus, Device, StandardReadable, observe_value
+from ophyd_async.core import (
+    AsyncStatus,
+    Device,
+    DeviceVector,
+    StandardReadable,
+    observe_value,
+)
 
 from ..signal.signal import epics_signal_r, epics_signal_rw, epics_signal_x
 
 
 class EnergyMode(str, Enum):
     """Energy mode for `Sensor`"""
 
@@ -39,14 +45,27 @@
         self.set_readable_signals(
             read=[self.value],
             config=[self.mode],
         )
         super().__init__(name=name)
 
 
+class SensorGroup(StandardReadable):
+    def __init__(self, prefix: str, name: str = "", sensor_count: int = 3) -> None:
+        self.sensors = DeviceVector(
+            {i: Sensor(f"{prefix}{i}:") for i in range(1, sensor_count + 1)}
+        )
+
+        # Makes read() produce the values of all sensors
+        self.set_readable_signals(
+            read=[sensor.value for sensor in self.sensors.values()],
+        )
+        super().__init__(name)
+
+
 class Mover(StandardReadable, Movable, Stoppable):
     """A demo movable that moves based on velocity"""
 
     def __init__(self, prefix: str, name="") -> None:
         # Define some signals
         self.setpoint = epics_signal_rw(float, prefix + "Setpoint")
         self.readback = epics_signal_r(float, prefix + "Readback")
@@ -131,19 +150,30 @@
     """Start an IOC subprocess with EPICS database for sample stage and sensor
     with the same pv prefix
     """
 
     pv_prefix = "".join(random.choice(string.ascii_uppercase) for _ in range(12)) + ":"
     here = Path(__file__).absolute().parent
     args = [sys.executable, "-m", "epicscorelibs.ioc"]
+
+    # Create standalone sensor
     args += ["-m", f"P={pv_prefix}"]
     args += ["-d", str(here / "sensor.db")]
-    for suff in "XY":
-        args += ["-m", f"P={pv_prefix}{suff}:"]
+
+    # Create sensor group
+    for suffix in ["1", "2", "3"]:
+        args += ["-m", f"P={pv_prefix}{suffix}:"]
+        args += ["-d", str(here / "sensor.db")]
+
+    # Create X and Y motors
+    for suffix in ["X", "Y"]:
+        args += ["-m", f"P={pv_prefix}{suffix}:"]
         args += ["-d", str(here / "mover.db")]
+
+    # Start IOC
     process = subprocess.Popen(
         args,
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         universal_newlines=True,
     )
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/demo/demo_ad_sim_detector.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/demo/demo_ad_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/demo/mover.db` & `ophyd_async-0.3a2/src/ophyd_async/epics/demo/mover.db`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/demo/sensor.db` & `ophyd_async-0.3a2/src/ophyd_async/epics/demo/sensor.db`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/motion/motor.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/motion/motor.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,41 +10,47 @@
 
 
 class Motor(StandardReadable, Movable, Stoppable):
     """Device that moves a motor record"""
 
     def __init__(self, prefix: str, name="") -> None:
         # Define some signals
-        self.setpoint = epics_signal_rw(float, prefix + ".VAL")
-        self.readback = epics_signal_r(float, prefix + ".RBV")
+        self.user_setpoint = epics_signal_rw(float, prefix + ".VAL")
+        self.user_readback = epics_signal_r(float, prefix + ".RBV")
         self.velocity = epics_signal_rw(float, prefix + ".VELO")
-        self.units = epics_signal_r(str, prefix + ".EGU")
+        self.max_velocity = epics_signal_r(float, prefix + ".VMAX")
+        self.acceleration_time = epics_signal_rw(float, prefix + ".ACCL")
+        self.motor_egu = epics_signal_r(str, prefix + ".EGU")
         self.precision = epics_signal_r(int, prefix + ".PREC")
-        # Signals that collide with standard methods should have a trailing underscore
-        self.stop_ = epics_signal_x(prefix + ".STOP")
+        self.deadband = epics_signal_r(float, prefix + ".RDBD")
+        self.motor_done_move = epics_signal_r(float, prefix + ".DMOV")
+        self.low_limit_travel = epics_signal_rw(int, prefix + ".LLM")
+        self.high_limit_travel = epics_signal_rw(int, prefix + ".HLM")
+
+        self.motor_stop = epics_signal_x(prefix + ".STOP")
         # Whether set() should complete successfully or not
         self._set_success = True
         # Set name and signals for read() and read_configuration()
         self.set_readable_signals(
-            read=[self.readback],
-            config=[self.velocity, self.units],
+            read=[self.user_readback],
+            config=[self.velocity, self.motor_egu],
         )
         super().__init__(name=name)
 
     def set_name(self, name: str):
         super().set_name(name)
         # Readback should be named the same as its parent in read()
-        self.readback.set_name(name)
+        self.user_readback.set_name(name)
 
     async def _move(self, new_position: float, watchers: List[Callable] = []):
         self._set_success = True
         start = time.monotonic()
         old_position, units, precision = await asyncio.gather(
-            self.setpoint.get_value(),
-            self.units.get_value(),
+            self.user_setpoint.get_value(),
+            self.motor_egu.get_value(),
             self.precision.get_value(),
         )
 
         def update_watchers(current_position: float):
             for watcher in watchers:
                 watcher(
                     name=self.name,
@@ -52,19 +58,19 @@
                     initial=old_position,
                     target=new_position,
                     unit=units,
                     precision=precision,
                     time_elapsed=time.monotonic() - start,
                 )
 
-        self.readback.subscribe_value(update_watchers)
+        self.user_readback.subscribe_value(update_watchers)
         try:
-            await self.setpoint.set(new_position)
+            await self.user_setpoint.set(new_position)
         finally:
-            self.readback.clear_sub(update_watchers)
+            self.user_readback.clear_sub(update_watchers)
         if not self._set_success:
             raise RuntimeError("Motor was stopped")
 
     def move(self, new_position: float, timeout: Optional[float] = None):
         """Commandline only synchronous move of a Motor"""
         from bluesky.run_engine import call_in_bluesky_event_loop, in_bluesky_event_loop
 
@@ -77,9 +83,9 @@
         coro = asyncio.wait_for(self._move(new_position, watchers), timeout=timeout)
         return AsyncStatus(coro, watchers)
 
     async def stop(self, success=False):
         self._set_success = success
         # Put with completion will never complete as we are waiting for completion on
         # the move above, so need to pass wait=False
-        status = self.stop_.trigger(wait=False)
+        status = self.motor_stop.trigger(wait=False)
         await status
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/signal/_epics_transport.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/signal/_epics_transport.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async/epics/signal/signal.py` & `ophyd_async-0.3a2/src/ophyd_async/epics/signal/signal.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,62 +37,79 @@
     r_transport, r_pv = _transport_pv(read_pv)
     w_transport, w_pv = _transport_pv(write_pv)
     transport = get_unique({read_pv: r_transport, write_pv: w_transport}, "transports")
     return transport.value(datatype, r_pv, w_pv)
 
 
 def epics_signal_rw(
-    datatype: Type[T], read_pv: str, write_pv: Optional[str] = None
+    datatype: Type[T], read_pv: str, write_pv: Optional[str] = None, name: str = ""
 ) -> SignalRW[T]:
     """Create a `SignalRW` backed by 1 or 2 EPICS PVs
 
     Parameters
     ----------
     datatype:
         Check that the PV is of this type
     read_pv:
         The PV to read and monitor
     write_pv:
         If given, use this PV to write to, otherwise use read_pv
     """
     backend = _make_backend(datatype, read_pv, write_pv or read_pv)
-    return SignalRW(backend)
+    return SignalRW(backend, name=name)
 
 
-def epics_signal_r(datatype: Type[T], read_pv: str) -> SignalR[T]:
-    """Create a `SignalR` backed by 1 EPICS PV
+def epics_signal_rw_rbv(
+    datatype: Type[T], write_pv: str, read_suffix: str = "_RBV", name: str = ""
+) -> SignalRW[T]:
+    """Create a `SignalRW` backed by 1 or 2 EPICS PVs, with a suffix on the readback pv
 
     Parameters
     ----------
     datatype:
         Check that the PV is of this type
+    write_pv:
+        The PV to write to
+    read_suffix:
+        Append this suffix to the write pv to create the readback pv
+    """
+    return epics_signal_rw(datatype, f"{write_pv}{read_suffix}", write_pv, name)
+
+
+def epics_signal_r(datatype: Type[T], read_pv: str, name: str = "") -> SignalR[T]:
+    """Create a `SignalR` backed by 1 EPICS PV
+
+    Parameters
+    ---------
+    datatype
+        Check that the PV is of this type
     read_pv:
         The PV to read and monitor
     """
     backend = _make_backend(datatype, read_pv, read_pv)
-    return SignalR(backend)
+    return SignalR(backend, name=name)
 
 
-def epics_signal_w(datatype: Type[T], write_pv: str) -> SignalW[T]:
+def epics_signal_w(datatype: Type[T], write_pv: str, name: str = "") -> SignalW[T]:
     """Create a `SignalW` backed by 1 EPICS PVs
 
     Parameters
     ----------
     datatype:
         Check that the PV is of this type
     write_pv:
         The PV to write to
     """
     backend = _make_backend(datatype, write_pv, write_pv)
-    return SignalW(backend)
+    return SignalW(backend, name=name)
 
 
-def epics_signal_x(write_pv: str) -> SignalX:
+def epics_signal_x(write_pv: str, name: str = "") -> SignalX:
     """Create a `SignalX` backed by 1 EPICS PVs
 
     Parameters
     ----------
     write_pv:
         The PV to write its initial value to on trigger
     """
     backend: SignalBackend = _make_backend(None, write_pv, write_pv)
-    return SignalX(backend)
+    return SignalX(backend, name=name)
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/panda/panda_controller.py` & `ophyd_async-0.3a2/src/ophyd_async/panda/_panda_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,19 @@
 
 from ophyd_async.core import (
     AsyncStatus,
     DetectorControl,
     DetectorTrigger,
     wait_for_value,
 )
-
-from .panda import PcapBlock
+from ophyd_async.panda import PcapBlock
 
 
 class PandaPcapController(DetectorControl):
-    def __init__(
-        self,
-        pcap: PcapBlock,
-    ) -> None:
+    def __init__(self, pcap: PcapBlock) -> None:
         self.pcap = pcap
 
     def get_deadtime(self, exposure: float) -> float:
         return 0.000000008
 
     async def arm(
         self,
@@ -31,11 +27,11 @@
             DetectorTrigger.constant_gate,
             trigger == DetectorTrigger.variable_gate,
         ), "Only constant_gate and variable_gate triggering is supported on the PandA"
         await asyncio.gather(self.pcap.arm.set(True))
         await wait_for_value(self.pcap.active, True, timeout=1)
         return AsyncStatus(wait_for_value(self.pcap.active, False, timeout=None))
 
-    async def disarm(self):
+    async def disarm(self) -> AsyncStatus:
         await asyncio.gather(self.pcap.arm.set(False))
         await wait_for_value(self.pcap.active, False, timeout=1)
         return AsyncStatus(wait_for_value(self.pcap.active, False, timeout=None))
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async/panda/table.py` & `ophyd_async-0.3a2/src/ophyd_async/panda/_table.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/src/ophyd_async.egg-info/SOURCES.txt` & `ophyd_async-0.3a2/src/ophyd_async.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 .codecov.yml
+.copier-answers.yml
 .git-blame-ignore-revs
 .gitignore
 .mailmap
 .pre-commit-config.yaml
+Dockerfile
 LICENSE
-README.rst
+README.md
 pyproject.toml
-.devcontainer/Dockerfile
 .devcontainer/devcontainer.json
-.github/CONTRIBUTING.rst
+.github/CONTRIBUTING.md
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
 .github/pages/index.html
 .github/pages/make_switcher.py
-.github/workflows/code.yml
-.github/workflows/docs.yml
-.github/workflows/docs_clean.yml
-.github/workflows/linkcheck.yml
+.github/workflows/_check.yml
+.github/workflows/_dist.yml
+.github/workflows/_docs.yml
+.github/workflows/_pypi.yml
+.github/workflows/_release.yml
+.github/workflows/_test.yml
+.github/workflows/_tox.yml
+.github/workflows/ci.yml
+.github/workflows/periodic.yml
 docs/conf.py
+docs/explanations.md
 docs/genindex.rst
-docs/index.rst
+docs/how-to.md
+docs/index.md
+docs/reference.md
+docs/tutorials.md
 docs/_templates/README
 docs/_templates/custom-class-template.rst
 docs/_templates/custom-module-template.rst
-docs/developer/index.rst
-docs/developer/explanations/decisions.rst
-docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
-docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
-docs/developer/explanations/decisions/0003-ophyd-async-migration.rst
-docs/developer/explanations/decisions/0004-repository-structure.rst
-docs/developer/explanations/decisions/0005-respect-black-line-length.rst
-docs/developer/explanations/decisions/0006-procedural-device-definitions.rst
-docs/developer/how-to/build-docs.rst
-docs/developer/how-to/contribute.rst
-docs/developer/how-to/lint.rst
-docs/developer/how-to/make-release.rst
-docs/developer/how-to/pin-requirements.rst
-docs/developer/how-to/run-tests.rst
-docs/developer/how-to/static-analysis.rst
-docs/developer/how-to/test-container.rst
-docs/developer/how-to/update-tools.rst
-docs/developer/reference/standards.rst
-docs/developer/tutorials/dev-install.rst
+docs/examples/epics_demo.py
+docs/explanations/decisions.md
+docs/explanations/event-loop-choice.rst
+docs/explanations/decisions/0001-record-architecture-decisions.md
+docs/explanations/decisions/0002-switched-to-python-copier-template.md
+docs/explanations/decisions/0003-ophyd-async-migration.rst
+docs/explanations/decisions/0004-repository-structure.rst
+docs/explanations/decisions/0005-respect-black-line-length.rst
+docs/explanations/decisions/0006-procedural-device-definitions.rst
+docs/explanations/decisions/COPYME
+docs/how-to/compound-devices.rst
+docs/how-to/contribute.md
+docs/how-to/make-a-simple-device.rst
+docs/how-to/write-tests-for-devices.rst
 docs/images/bluesky_ophyd_epics_devices_logo.svg
 docs/images/bluesky_ophyd_logo.svg
 docs/images/ophyd_favicon.svg
-docs/user/index.rst
-docs/user/examples/epics_demo.py
-docs/user/explanations/docs-structure.rst
-docs/user/explanations/event-loop-choice.rst
-docs/user/how-to/make-a-simple-device.rst
-docs/user/how-to/run-container.rst
-docs/user/reference/api.rst
-docs/user/tutorials/installation.rst
-docs/user/tutorials/using-existing-devices.rst
+docs/reference/api.rst
+docs/tutorials/installation.md
+docs/tutorials/using-existing-devices.rst
 src/ophyd_async/__init__.py
 src/ophyd_async/__main__.py
 src/ophyd_async/_version.py
+src/ophyd_async/protocols.py
 src/ophyd_async.egg-info/PKG-INFO
 src/ophyd_async.egg-info/SOURCES.txt
 src/ophyd_async.egg-info/dependency_links.txt
 src/ophyd_async.egg-info/entry_points.txt
 src/ophyd_async.egg-info/requires.txt
 src/ophyd_async.egg-info/top_level.txt
 src/ophyd_async/core/__init__.py
@@ -72,69 +72,105 @@
 src/ophyd_async/core/flyer.py
 src/ophyd_async/core/signal.py
 src/ophyd_async/core/signal_backend.py
 src/ophyd_async/core/sim_signal_backend.py
 src/ophyd_async/core/standard_readable.py
 src/ophyd_async/core/utils.py
 src/ophyd_async/epics/__init__.py
-src/ophyd_async/epics/pvi.py
 src/ophyd_async/epics/_backend/__init__.py
 src/ophyd_async/epics/_backend/_aioca.py
 src/ophyd_async/epics/_backend/_p4p.py
 src/ophyd_async/epics/_backend/common.py
 src/ophyd_async/epics/areadetector/__init__.py
+src/ophyd_async/epics/areadetector/aravis.py
+src/ophyd_async/epics/areadetector/pilatus.py
 src/ophyd_async/epics/areadetector/single_trigger_det.py
 src/ophyd_async/epics/areadetector/utils.py
 src/ophyd_async/epics/areadetector/controllers/__init__.py
 src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
+src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
 src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
 src/ophyd_async/epics/areadetector/drivers/__init__.py
 src/ophyd_async/epics/areadetector/drivers/ad_base.py
+src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
 src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
 src/ophyd_async/epics/areadetector/writers/__init__.py
 src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
 src/ophyd_async/epics/areadetector/writers/_hdffile.py
 src/ophyd_async/epics/areadetector/writers/hdf_writer.py
 src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
 src/ophyd_async/epics/areadetector/writers/nd_plugin.py
 src/ophyd_async/epics/demo/__init__.py
 src/ophyd_async/epics/demo/demo_ad_sim_detector.py
 src/ophyd_async/epics/demo/mover.db
 src/ophyd_async/epics/demo/sensor.db
 src/ophyd_async/epics/motion/__init__.py
 src/ophyd_async/epics/motion/motor.py
+src/ophyd_async/epics/pvi/__init__.py
+src/ophyd_async/epics/pvi/pvi.py
 src/ophyd_async/epics/signal/__init__.py
 src/ophyd_async/epics/signal/_epics_transport.py
 src/ophyd_async/epics/signal/signal.py
 src/ophyd_async/panda/__init__.py
-src/ophyd_async/panda/panda.py
-src/ophyd_async/panda/panda_controller.py
-src/ophyd_async/panda/table.py
-src/ophyd_async/panda/utils.py
+src/ophyd_async/panda/_common_blocks.py
+src/ophyd_async/panda/_hdf_panda.py
+src/ophyd_async/panda/_panda_controller.py
+src/ophyd_async/panda/_table.py
+src/ophyd_async/panda/_trigger.py
+src/ophyd_async/panda/_utils.py
+src/ophyd_async/panda/writers/__init__.py
+src/ophyd_async/panda/writers/_hdf_writer.py
+src/ophyd_async/panda/writers/_panda_hdf_file.py
+src/ophyd_async/planstubs/__init__.py
+src/ophyd_async/planstubs/prepare_trigger_and_dets.py
+src/ophyd_async/sim/__init__.py
+src/ophyd_async/sim/pattern_generator.py
+src/ophyd_async/sim/sim_pattern_detector_control.py
+src/ophyd_async/sim/sim_pattern_detector_writer.py
+src/ophyd_async/sim/sim_pattern_generator.py
+src/ophyd_async/sim/demo/__init__.py
+src/ophyd_async/sim/demo/sim_motor.py
 tests/conftest.py
 tests/test_cli.py
+tests/test_flyer_with_panda.py
 tests/core/test_async_status.py
 tests/core/test_device.py
 tests/core/test_device_collector.py
 tests/core/test_device_save_loader.py
 tests/core/test_flyer.py
 tests/core/test_signal.py
 tests/core/test_sim.py
 tests/core/test_utils.py
+tests/epics/test_pvi.py
 tests/epics/test_records.db
 tests/epics/test_signals.py
+tests/epics/_backend/test_common.py
 tests/epics/areadetector/__init__.py
+tests/epics/areadetector/test_aravis.py
 tests/epics/areadetector/test_controllers.py
 tests/epics/areadetector/test_drivers.py
+tests/epics/areadetector/test_pilatus.py
 tests/epics/areadetector/test_scans.py
 tests/epics/areadetector/test_single_trigger_det.py
 tests/epics/areadetector/test_utils.py
 tests/epics/areadetector/test_writers.py
 tests/epics/demo/test_demo.py
 tests/epics/demo/test_demo_ad_sim_detector.py
 tests/epics/motion/__init__.py
 tests/epics/motion/test_motor.py
-tests/panda/test_panda.py
+tests/panda/test_hdf_panda.py
+tests/panda/test_panda_connect.py
 tests/panda/test_panda_controller.py
 tests/panda/test_panda_utils.py
 tests/panda/test_table.py
-tests/panda/db/panda.db
+tests/panda/test_trigger.py
+tests/panda/test_writer.py
+tests/panda/db/panda.db
+tests/protocols/test_protocols.py
+tests/sim/__init__.py
+tests/sim/conftest.py
+tests/sim/test_pattern_generator.py
+tests/sim/test_sim_detector.py
+tests/sim/test_sim_writer.py
+tests/sim/test_streaming_plan.py
+tests/sim/demo/__init__.py
+tests/sim/demo/test_sim_motor.py
```

### Comparing `ophyd-async-0.3a1/src/ophyd_async.egg-info/requires.txt` & `ophyd_async-0.3a2/src/ophyd_async.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 networkx>=2.0
 numpy
 packaging
 pint
 bluesky>=1.13.0a3
-event-model
+event-model<1.21.0
 p4p
 pyyaml
 
-[:python_version < "3.8"]
-typing-extensions
-
 [ca]
 aioca>=1.6
 
 [dev]
 ophyd_async[pva]
 ophyd_async[ca]
 black
@@ -21,30 +18,30 @@
 flake8-isort
 Flake8-pyproject
 h5py
 inflection
 ipython
 ipywidgets
 matplotlib
-mypy
 myst-parser
 numpydoc
 ophyd
 pickleshare
 pipdeptree
 pre-commit
 pydata-sphinx-theme>=0.12
 pyepics>=3.4.2
-pyside6
+pyside6==6.6.2
 pytest
 pytest-asyncio
 pytest-cov
 pytest-faulthandler
 pytest-rerunfailures
 pytest-timeout
+ruff
 sphinx-autobuild
 sphinx-copybutton
 sphinx-design
 tox-direct
 types-mock
 types-pyyaml
```

### Comparing `ophyd-async-0.3a1/tests/conftest.py` & `ophyd_async-0.3a2/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,41 @@
 import asyncio
+import os
 import subprocess
 import sys
 import time
 from pathlib import Path
 from typing import Any, Callable
 
 import pytest
 from bluesky.run_engine import RunEngine, TransitionError
 
-RECORD = str(Path(__file__).parent / "panda" / "db" / "panda.db")
+from ophyd_async.core import StaticDirectoryProvider
+
+PANDA_RECORD = str(Path(__file__).parent / "panda" / "db" / "panda.db")
 INCOMPLETE_BLOCK_RECORD = str(
     Path(__file__).parent / "panda" / "db" / "incomplete_block_panda.db"
 )
 INCOMPLETE_RECORD = str(Path(__file__).parent / "panda" / "db" / "incomplete_panda.db")
 EXTRA_BLOCKS_RECORD = str(
     Path(__file__).parent / "panda" / "db" / "extra_blocks_panda.db"
 )
 
+# Prevent pytest from catching exceptions when debugging in vscode so that break on
+# exception works correctly (see: https://github.com/pytest-dev/pytest/issues/7409)
+if os.getenv("PYTEST_RAISE", "0") == "1":
+
+    @pytest.hookimpl(tryfirst=True)
+    def pytest_exception_interact(call):
+        raise call.excinfo.value
+
+    @pytest.hookimpl(tryfirst=True)
+    def pytest_internalerror(excinfo):
+        raise excinfo.value
+
 
 @pytest.fixture(scope="function")
 def RE(request):
     loop = asyncio.new_event_loop()
     loop.set_debug(True)
     RE = RunEngine({}, call_returns_result=True, loop=loop)
 
@@ -35,25 +50,25 @@
         loop.close()
 
     request.addfinalizer(clean_event_loop)
     return RE
 
 
 @pytest.fixture(scope="module", params=["pva"])
-def pva():
+def panda_pva():
     processes = [
         subprocess.Popen(
             [
                 sys.executable,
                 "-m",
                 "epicscorelibs.ioc",
                 "-m",
                 macros,
                 "-d",
-                RECORD,
+                PANDA_RECORD,
             ],
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             universal_newlines=True,
         )
         for macros in [
@@ -85,7 +100,12 @@
 @pytest.fixture
 async def failing_coroutine() -> Callable[[], Any]:
     async def inner_coroutine():
         await asyncio.sleep(0.01)
         raise ValueError()
 
     return inner_coroutine
+
+
+@pytest.fixture
+def static_directory_provider(tmp_path: Path):
+    return StaticDirectoryProvider(directory_path=tmp_path)
```

### Comparing `ophyd-async-0.3a1/tests/core/test_async_status.py` & `ophyd_async-0.3a2/tests/core/test_async_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     assert isinstance(status.exception(), asyncio.CancelledError)
 
 
 async def coroutine_to_wrap(time: float):
     await asyncio.sleep(time)
 
 
-async def test_async_status_wrap():
+async def test_async_status_wrap() -> None:
     wrapped_coroutine = AsyncStatus.wrap(coroutine_to_wrap)
     status: AsyncStatus = wrapped_coroutine(0.01)
 
     await status
     assert status.success is True
```

### Comparing `ophyd-async-0.3a1/tests/core/test_device.py` & `ophyd_async-0.3a2/tests/core/test_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,17 +47,15 @@
         )
         assert child.parent == parent
 
 
 def test_device_vector_children():
     parent = DummyDeviceGroup("root")
 
-    device_vector_children = [
-        (name, child) for name, child in parent.dict_with_children.children()
-    ]
+    device_vector_children = list(parent.dict_with_children.children())
     assert device_vector_children == [("123", parent.dict_with_children[123])]
 
 
 async def test_children_of_device_have_set_names_and_get_connected(
     parent: DummyDeviceGroup,
 ):
     assert parent.name == "parent"
```

### Comparing `ophyd-async-0.3a1/tests/core/test_device_collector.py` & `ophyd_async-0.3a2/tests/core/test_device_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,16 @@
 
         def my_plan():
             yield from bps.mov(sim_motor, 3.14)
 
         RE(my_plan())
 
         assert (
-            checking_loop.run_until_complete(sim_motor.setpoint.read())[
-                "sim_motor-setpoint"
+            checking_loop.run_until_complete(sim_motor.user_setpoint.read())[
+                "sim_motor-user_setpoint"
             ]["value"]
             == 3.14
         )
 
     finally:
         if RE.state not in ("idle", "panicked"):
             try:
@@ -142,12 +142,12 @@
     def my_plan():
         yield from bps.mov(sim_motor, 3.14)
 
     RE(my_plan())
 
     # The set should fail since the run engine is on a different event loop
     assert (
-        device_connector_loop.run_until_complete(sim_motor.setpoint.read())[
-            "sim_motor-setpoint"
+        device_connector_loop.run_until_complete(sim_motor.user_setpoint.read())[
+            "sim_motor-user_setpoint"
         ]["value"]
         != 3.14
     )
```

### Comparing `ophyd-async-0.3a1/tests/core/test_device_save_loader.py` & `ophyd_async-0.3a2/tests/core/test_device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/tests/core/test_flyer.py` & `ophyd_async-0.3a2/tests/core/test_flyer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from enum import Enum
-from typing import AsyncGenerator, AsyncIterator, Dict, Optional, Sequence
+from typing import Any, AsyncGenerator, AsyncIterator, Dict, Optional, Sequence
 from unittest.mock import Mock
 
 import bluesky.plan_stubs as bps
 import pytest
 from bluesky.protocols import Descriptor, StreamAsset
 from bluesky.run_engine import RunEngine
 from event_model import ComposeStreamResourceBundle, compose_stream_resource
@@ -31,43 +31,41 @@
     stopping = "stopping"
 
 
 class DummyTriggerLogic(TriggerLogic[int]):
     def __init__(self):
         self.state = TriggerState.null
 
-    def trigger_info(self, value: int) -> TriggerInfo:
-        return TriggerInfo(
-            num=value, trigger=DetectorTrigger.constant_gate, deadtime=2, livetime=2
-        )
-
     async def prepare(self, value: int):
         self.state = TriggerState.preparing
         return value
 
-    async def start(self):
+    async def kickoff(self):
         self.state = TriggerState.starting
 
+    async def complete(self):
+        self.state = TriggerState.null
+
     async def stop(self):
         self.state = TriggerState.stopping
 
 
 class DummyWriter(DetectorWriter):
     def __init__(self, name: str, shape: Sequence[int]):
-        self.dummy_signal = SignalRW(backend=SimSignalBackend(int, source="test"))
+        self.dummy_signal = SignalRW(backend=SimSignalBackend(int))
         self._shape = shape
         self._name = name
         self._file: Optional[ComposeStreamResourceBundle] = None
         self._last_emitted = 0
         self.index = 0
 
     async def open(self, multiplier: int = 1) -> Dict[str, Descriptor]:
         return {
             self._name: Descriptor(
-                source="sim://some-source",
+                source="soft://some-source",
                 shape=self._shape,
                 dtype="number",
                 external="STREAM:",
             )
         }
 
     async def observe_indices_written(
@@ -95,18 +93,18 @@
                         "multiplier": 1,
                         "timestamps": "/entry/instrument/NDAttributes/NDArrayTimeStamp",
                     },
                 )
                 yield "stream_resource", self._file.stream_resource_doc
 
             if indices_written >= self._last_emitted:
-                indices = dict(
-                    start=self._last_emitted,
-                    stop=indices_written,
-                )
+                indices = {
+                    "start": self._last_emitted,
+                    "stop": indices_written,
+                }
                 self._last_emitted = indices_written
                 self._last_flush = time.monotonic()
                 yield "stream_datum", self._file.compose_stream_datum(indices)
 
     async def close(self) -> None:
         self._file = None
 
@@ -119,21 +117,21 @@
 
     async def dummy_arm_1(self=None, trigger=None, num=0, exposure=None):
         return writers[0].dummy_signal.set(1)
 
     async def dummy_arm_2(self=None, trigger=None, num=0, exposure=None):
         return writers[1].dummy_signal.set(1)
 
-    detector_1 = StandardDetector(
+    detector_1: StandardDetector[Any] = StandardDetector(
         Mock(spec=DetectorControl, get_deadtime=lambda num: num, arm=dummy_arm_1),
         writers[0],
         name="detector_1",
         writer_timeout=3,
     )
-    detector_2 = StandardDetector(
+    detector_2: StandardDetector[Any] = StandardDetector(
         Mock(spec=DetectorControl, get_deadtime=lambda num: num, arm=dummy_arm_2),
         writers[1],
         name="detector_2",
         writer_timeout=3,
     )
 
     return (detector_1, detector_2)
@@ -149,46 +147,49 @@
         names.append(name)
         docs.append(doc)
 
     RE.subscribe(append_and_print)
 
     trigger_logic = DummyTriggerLogic()
     flyer = HardwareTriggeredFlyable(trigger_logic, [], name="flyer")
+    trigger_info = TriggerInfo(
+        num=1, trigger=DetectorTrigger.constant_gate, deadtime=2, livetime=2
+    )
 
     def flying_plan():
         yield from bps.stage_all(*detector_list, flyer)
         assert flyer._trigger_logic.state == TriggerState.stopping
 
         # move the flyer to the correct place, before fly scanning.
         # Prepare the flyer first to get the trigger info for the detectors
         yield from bps.prepare(flyer, 1, wait=True)
 
         # prepare detectors second.
         for detector in detector_list:
             yield from bps.prepare(
                 detector,
-                flyer.trigger_info,
+                trigger_info,
                 wait=True,
             )
 
-        assert trigger_logic.state == TriggerState.preparing
+        assert flyer._trigger_logic.state == TriggerState.preparing
         for detector in detector_list:
             detector.controller.disarm.assert_called_once  # type: ignore
 
         yield from bps.open_run()
         yield from bps.declare_stream(*detector_list, name="main_stream", collect=True)
 
         yield from bps.kickoff(flyer)
         for detector in detector_list:
             yield from bps.kickoff(detector)
 
         yield from bps.complete(flyer, wait=False, group="complete")
         for detector in detector_list:
             yield from bps.complete(detector, wait=False, group="complete")
-        assert trigger_logic.state == TriggerState.starting
+        assert flyer._trigger_logic.state == TriggerState.null
 
         # Manually incremenet the index as if a frame was taken
         for detector in detector_list:
             detector.writer.index += 1
 
         done = False
         while not done:
@@ -197,17 +198,16 @@
             except TimeoutError:
                 pass
             else:
                 done = True
             yield from bps.collect(
                 *detector_list,
                 return_payload=False,
-                # name="main_stream",
+                name="main_stream",
             )
-            yield from bps.sleep(0.01)
         yield from bps.wait(group="complete")
         yield from bps.close_run()
 
         yield from bps.unstage_all(flyer, *detector_list)
         for detector in detector_list:
             assert detector.controller.disarm.called  # type: ignore
         assert trigger_logic.state == TriggerState.stopping
@@ -222,24 +222,14 @@
         "stream_datum",
         "stream_resource",
         "stream_datum",
         "stop",
     ]
 
 
-def test_flyer_has_trigger_logic_property():
-    flyer = HardwareTriggeredFlyable(DummyTriggerLogic(), [], name="flyer")
-    trigger_info = flyer.trigger_logic.trigger_info(1)
-    assert type(trigger_info) is TriggerInfo
-    assert trigger_info.num == 1
-    assert trigger_info.trigger == "constant_gate"
-    assert trigger_info.deadtime == 2
-    assert trigger_info.livetime == 2
-
-
 # To do: Populate configuration signals
 async def test_describe_configuration():
     flyer = HardwareTriggeredFlyable(DummyTriggerLogic(), [], name="flyer")
     assert await flyer.describe_configuration() == {}
 
 
 # To do: Populate configuration signals
```

### Comparing `ophyd-async-0.3a1/tests/core/test_sim.py` & `ophyd_async-0.3a2/tests/core/test_sim.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 class MyEnum(str, Enum):
     a = "Aaa"
     b = "Bbb"
     c = "Ccc"
 
 
 def integer_d(value):
-    return dict(dtype="integer", shape=[])
+    return {"dtype": "integer", "shape": []}
 
 
 def number_d(value):
-    return dict(dtype="number", shape=[])
+    return {"dtype": "number", "shape": []}
 
 
 def string_d(value):
-    return dict(dtype="string", shape=[])
+    return {"dtype": "string", "shape": []}
 
 
 def enum_d(value):
-    return dict(dtype="string", shape=[], choices=["Aaa", "Bbb", "Ccc"])
+    return {"dtype": "string", "shape": [], "choices": ["Aaa", "Bbb", "Ccc"]}
 
 
 def waveform_d(value):
-    return dict(dtype="array", shape=[len(value)])
+    return {"dtype": "array", "shape": [len(value)]}
 
 
 class MonitorQueue:
     def __init__(self, backend: SignalBackend):
         self.backend = backend
         self.updates: asyncio.Queue[Tuple[Reading, Any]] = asyncio.Queue()
         backend.set_callback(self.add_reading_value)
@@ -89,52 +89,52 @@
 )
 async def test_backend_get_put_monitor(
     datatype: Type[T],
     initial_value: T,
     put_value: T,
     descriptor: Callable[[Any], dict],
 ):
-    backend = SimSignalBackend(datatype, "")
+    backend = SimSignalBackend(datatype)
 
     await backend.connect()
     q = MonitorQueue(backend)
     try:
         # Check descriptor
-        assert (
-            dict(source="sim://", **descriptor(initial_value))
-            == await backend.get_descriptor()
-        )
+        source = "soft://test"
+        assert dict(
+            source=source, **descriptor(initial_value)
+        ) == await backend.get_descriptor(source)
         # Check initial value
         await q.assert_updates(
             pytest.approx(initial_value) if initial_value != "" else initial_value
         )
         # Put to new value and check that
         await backend.put(put_value)
         await q.assert_updates(pytest.approx(put_value))
     finally:
         q.close()
 
 
 async def test_sim_backend_if_disconnected():
-    sim_backend = SimSignalBackend(npt.NDArray[np.float64], "SOME-IOC:PV")
+    sim_backend = SimSignalBackend(npt.NDArray[np.float64])
     with pytest.raises(NotImplementedError):
         await sim_backend.get_value()
 
 
 async def test_sim_backend_with_numpy_typing():
-    sim_backend = SimSignalBackend(npt.NDArray[np.float64], "SOME-IOC:PV")
+    sim_backend = SimSignalBackend(npt.NDArray[np.float64])
     await sim_backend.connect()
 
     array = await sim_backend.get_value()
     assert array.shape == (0,)
 
 
 async def test_sim_backend_descriptor_fails_for_invalid_class():
     class myClass:
         def __init__(self) -> None:
             pass
 
-    sim_signal = Signal(SimSignalBackend(myClass, "test"))
+    sim_signal = Signal(SimSignalBackend(myClass))
     await sim_signal.connect(sim=True)
 
     with pytest.raises(AssertionError):
-        await sim_signal._backend.get_descriptor()
+        await sim_signal._backend.get_descriptor("")
```

### Comparing `ophyd-async-0.3a1/tests/core/test_utils.py` & `ophyd_async-0.3a2/tests/core/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     async def connect(self, timeout: float = DEFAULT_TIMEOUT):
         raise ValueError(self.exc_text)
 
 
 class WorkingDummyChildDevice(Device):
     def __init__(self, name: str = "working_dummy_child_device") -> None:
-        self.working_signal = SignalRW(backend=SimSignalBackend(int, "WORKING_SIGNAL"))
+        self.working_signal = SignalRW(backend=SimSignalBackend(int))
         super().__init__(name=name)
 
 
 class TimeoutDummyChildDeviceCA(Device):
     def __init__(self, name: str = "timeout_dummy_child_device_ca") -> None:
         self.timeout_signal = epics_signal_rw(int, "ca://A_NON_EXISTENT_SIGNAL")
         super().__init__(name=name)
@@ -135,17 +135,19 @@
 
     dummy_device_two_working_one_timeout_two_value_error = (
         DummyDeviceTwoWorkingTwoTimeOutTwoValueError()
     )
 
     # This should fail since the error is a ValueError
     with pytest.raises(NotConnected) as e:
-        await dummy_device_two_working_one_timeout_two_value_error.connect(
-            timeout=0.01
-        ),
+        (
+            await dummy_device_two_working_one_timeout_two_value_error.connect(
+                timeout=0.01
+            ),
+        )
     assert str(e.value) == str(TWO_WORKING_TWO_TIMEOUT_TWO_VALUE_ERROR_OUTPUT)
 
     logs = caplog.get_records("call")
     logs = [log for log in logs if "ophyd_async" in log.pathname]
     assert len(logs) == 4
 
     for i in range(0, 2):
@@ -209,15 +211,14 @@
         "    value_error_signal: ValueError: Some ValueError text\n"
         "value_error_child_device2: NotConnected:\n"
         "    value_error_signal: ValueError\n"
     )
 
 
 async def test_combining_top_level_signal_and_child_device():
-
     dummy_device1 = DummyDeviceCombiningTopLevelSignalAndSubDevice()
     with pytest.raises(NotConnected) as e:
         await dummy_device1.connect(timeout=0.01)
     assert str(e.value) == (
         "\ntimeout_signal: NotConnected: ca://A_NON_EXISTENT_SIGNAL\n"
         "sub_device: NotConnected:\n"
         "    value_error_signal: ValueError: Some ValueError text\n"
```

### Comparing `ophyd-async-0.3a1/tests/epics/areadetector/test_controllers.py` & `ophyd_async-0.3a2/tests/epics/areadetector/test_controllers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 from ophyd_async.core import DetectorTrigger, DeviceCollector
 from ophyd_async.epics.areadetector.controllers import (
     ADSimController,
     PilatusController,
 )
 from ophyd_async.epics.areadetector.drivers import ADBase, PilatusDriver
-from ophyd_async.epics.areadetector.drivers.pilatus_driver import (
-    TriggerMode as PilatusTrigger,
-)
+from ophyd_async.epics.areadetector.drivers.pilatus_driver import PilatusTriggerMode
 from ophyd_async.epics.areadetector.utils import ImageMode
 
 
 @pytest.fixture
 async def pilatus(RE) -> PilatusController:
     async with DeviceCollector(sim=True):
         drv = PilatusDriver("DRIVER:")
@@ -49,18 +47,18 @@
     assert await driver.acquire.get_value() is False
 
 
 async def test_pilatus_controller(RE, pilatus: PilatusController):
     with patch("ophyd_async.core.signal.wait_for_value", return_value=None):
         await pilatus.arm(num=1, trigger=DetectorTrigger.constant_gate)
 
-    driver = pilatus.driver
+    driver = pilatus._drv
     assert await driver.num_images.get_value() == 1
     assert await driver.image_mode.get_value() == ImageMode.multiple
-    assert await driver.trigger_mode.get_value() == PilatusTrigger.ext_enable
+    assert await driver.trigger_mode.get_value() == PilatusTriggerMode.ext_enable
     assert await driver.acquire.get_value() is True
 
     with patch(
         "ophyd_async.epics.areadetector.utils.wait_for_value", return_value=None
     ):
         await pilatus.disarm()
```

### Comparing `ophyd-async-0.3a1/tests/epics/areadetector/test_scans.py` & `ophyd_async-0.3a2/tests/epics/areadetector/test_scans.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 from pathlib import Path
-from typing import Optional
+from typing import Any, Optional
 from unittest.mock import AsyncMock
 
 import bluesky.plan_stubs as bps
 import bluesky.plans as bp
 import pytest
 from bluesky import RunEngine
 
@@ -24,23 +24,20 @@
 from ophyd_async.epics.areadetector.drivers import ADBase
 from ophyd_async.epics.areadetector.writers import HDFWriter, NDFileHDF
 
 
 class DummyTriggerLogic(TriggerLogic[int]):
     def __init__(self): ...
 
-    def trigger_info(self, value: int) -> TriggerInfo:
-        return TriggerInfo(
-            num=value, trigger=DetectorTrigger.constant_gate, deadtime=2, livetime=2
-        )
-
     async def prepare(self, value: int):
         return value
 
-    async def start(self): ...
+    async def kickoff(self): ...
+
+    async def complete(self): ...
 
     async def stop(self): ...
 
 
 class DummyController(DetectorControl):
     def __init__(self) -> None: ...
 
@@ -81,43 +78,48 @@
 
 async def test_hdf_writer_fails_on_timeout_with_stepscan(
     RE: RunEngine,
     writer: HDFWriter,
     controller: ADSimController,
 ):
     set_sim_value(writer.hdf.file_path_exists, True)
-    detector = StandardDetector(
+    detector: StandardDetector[Any] = StandardDetector(
         controller, writer, name="detector", writer_timeout=0.01
     )
 
     with pytest.raises(Exception) as exc:
         RE(bp.count([detector]))
 
     assert isinstance(exc.value.__cause__, asyncio.TimeoutError)
 
 
 def test_hdf_writer_fails_on_timeout_with_flyscan(RE: RunEngine, writer: HDFWriter):
     controller = DummyController()
     set_sim_value(writer.hdf.file_path_exists, True)
 
-    detector = StandardDetector(controller, writer, writer_timeout=0.01)
+    detector: StandardDetector[Optional[TriggerInfo]] = StandardDetector(
+        controller, writer, writer_timeout=0.01
+    )
     trigger_logic = DummyTriggerLogic()
 
     flyer = HardwareTriggeredFlyable(trigger_logic, [], name="flyer")
+    trigger_info = TriggerInfo(
+        num=1, trigger=DetectorTrigger.constant_gate, deadtime=2, livetime=2
+    )
 
     def flying_plan():
         """NOTE: the following is a workaround to ensure tests always pass.
         See https://github.com/bluesky/bluesky/issues/1630 for more details.
         """
         yield from bps.stage_all(detector, flyer)
         try:
             # Prepare the flyer first to get the trigger info for the detectors
             yield from bps.prepare(flyer, 1, wait=True)
             # prepare detector second.
-            yield from bps.prepare(detector, flyer.trigger_info, wait=True)
+            yield from bps.prepare(detector, trigger_info, wait=True)
             yield from bps.open_run()
             yield from bps.kickoff(flyer)
             yield from bps.kickoff(detector)
             yield from bps.complete(flyer, wait=True)
             yield from bps.complete(detector, wait=True)
             yield from bps.close_run()
         finally:
```

### Comparing `ophyd-async-0.3a1/tests/epics/areadetector/test_single_trigger_det.py` & `ophyd_async-0.3a2/tests/epics/areadetector/test_single_trigger_det.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,13 +40,9 @@
     assert 1 == await drv.acquire.get_value()
     assert ImageMode.single == await drv.image_mode.get_value()
     assert True is await drv.wait_for_plugins.get_value()
 
     assert names == ["start", "descriptor", "event", "stop"]
     _, descriptor, event, _ = docs
     assert descriptor["configuration"]["det"]["data"]["det-drv-acquire_time"] == 0.5
-    assert (
-        descriptor["data_keys"]["det-stats-unique_id"]["source"]
-        == "sim://PREFIX:STATSUniqueId_RBV"
-    )
     assert event["data"]["det-drv-array_counter"] == 1
     assert event["data"]["det-stats-unique_id"] == 3
```

### Comparing `ophyd-async-0.3a1/tests/epics/areadetector/test_utils.py` & `ophyd_async-0.3a2/tests/epics/areadetector/test_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/tests/epics/areadetector/test_writers.py` & `ophyd_async-0.3a2/tests/epics/areadetector/test_writers.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,27 +24,27 @@
 async def hdf_writer(RE) -> HDFWriter:
     async with DeviceCollector(sim=True):
         hdf = NDFileHDF("HDF:")
 
     return HDFWriter(
         hdf,
         StaticDirectoryProvider("some_path", "some_prefix"),
-        lambda: "test",
-        DummyShapeProvider(),
+        name_provider=lambda: "test",
+        shape_provider=DummyShapeProvider(),
     )
 
 
 async def test_correct_descriptor_doc_after_open(hdf_writer: HDFWriter):
     set_sim_value(hdf_writer.hdf.file_path_exists, True)
     with patch("ophyd_async.core.signal.wait_for_value", return_value=None):
         descriptor = await hdf_writer.open()
 
     assert descriptor == {
         "test": {
-            "source": "sim://HDF:FullFileName_RBV",
+            "source": "soft://hdf-full_file_name",
             "shape": (10, 10),
             "dtype": "array",
             "external": "STREAM:",
         }
     }
 
     await hdf_writer.close()
```

### Comparing `ophyd-async-0.3a1/tests/epics/demo/test_demo.py` & `ophyd_async-0.3a2/tests/epics/demo/test_demo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
+import subprocess
 from typing import Dict
-from unittest.mock import Mock, call
+from unittest.mock import ANY, Mock, call, patch
 
 import pytest
 from bluesky.protocols import Reading
 
 from ophyd_async.core import (
     DeviceCollector,
     NotConnected,
@@ -15,34 +16,44 @@
 
 # Long enough for multiple asyncio event loop cycles to run so
 # all the tasks have a chance to run
 A_WHILE = 0.001
 
 
 @pytest.fixture
-async def sim_mover():
+async def sim_mover() -> demo.Mover:
     async with DeviceCollector(sim=True):
         sim_mover = demo.Mover("BLxxI-MO-TABLE-01:X:")
         # Signals connected here
 
     assert sim_mover.name == "sim_mover"
     set_sim_value(sim_mover.units, "mm")
     set_sim_value(sim_mover.precision, 3)
     set_sim_value(sim_mover.velocity, 1)
-    yield sim_mover
+    return sim_mover
 
 
 @pytest.fixture
-async def sim_sensor():
+async def sim_sensor() -> demo.Sensor:
     async with DeviceCollector(sim=True):
         sim_sensor = demo.Sensor("SIM:SENSOR:")
         # Signals connected here
 
     assert sim_sensor.name == "sim_sensor"
-    yield sim_sensor
+    return sim_sensor
+
+
+@pytest.fixture
+async def sim_sensor_group() -> demo.SensorGroup:
+    async with DeviceCollector(sim=True):
+        sim_sensor_group = demo.SensorGroup("SIM:SENSOR:")
+        # Signals connected here
+
+    assert sim_sensor_group.name == "sim_sensor_group"
+    return sim_sensor_group
 
 
 class Watcher:
     def __init__(self) -> None:
         self._event = asyncio.Event()
         self._mock = Mock()
 
@@ -93,45 +104,61 @@
     assert s.success
     done.assert_called_once_with(s)
     done2 = Mock()
     s.add_callback(done2)
     done2.assert_called_once_with(s)
 
 
+async def test_sensor_reading_shows_value(sim_sensor: demo.Sensor):
+    # Check default value
+    assert (await sim_sensor.value.get_value()) == pytest.approx(0.0)
+    assert (await sim_sensor.read()) == {
+        "sim_sensor-value": {
+            "alarm_severity": 0,
+            "timestamp": ANY,
+            "value": 0.0,
+        }
+    }
+
+    # Check different value
+    set_sim_value(sim_sensor.value, 5.0)
+    assert (await sim_sensor.read()) == {
+        "sim_sensor-value": {
+            "alarm_severity": 0,
+            "timestamp": ANY,
+            "value": 5.0,
+        }
+    }
+
+
 async def test_mover_stopped(sim_mover: demo.Mover):
     callbacks = []
     set_sim_callback(sim_mover.stop_, lambda r, v: callbacks.append(v))
 
     assert callbacks == [None]
     await sim_mover.stop()
     assert callbacks == [None, None]
 
 
 async def test_read_mover(sim_mover: demo.Mover):
     await sim_mover.stage()
     assert (await sim_mover.read())["sim_mover"]["value"] == 0.0
-    assert (await sim_mover.describe())["sim_mover"][
-        "source"
-    ] == "sim://BLxxI-MO-TABLE-01:X:Readback"
     assert (await sim_mover.read_configuration())["sim_mover-velocity"]["value"] == 1
     assert (await sim_mover.describe_configuration())["sim_mover-units"]["shape"] == []
     set_sim_value(sim_mover.readback, 0.5)
     assert (await sim_mover.read())["sim_mover"]["value"] == 0.5
     await sim_mover.unstage()
     # Check we can still read and describe when not staged
     set_sim_value(sim_mover.readback, 0.1)
     assert (await sim_mover.read())["sim_mover"]["value"] == 0.1
     assert await sim_mover.describe()
 
 
 async def test_set_velocity(sim_mover: demo.Mover) -> None:
     v = sim_mover.velocity
-    assert (await v.describe())["sim_mover-velocity"][
-        "source"
-    ] == "sim://BLxxI-MO-TABLE-01:X:Velocity"
     q: asyncio.Queue[Dict[str, Reading]] = asyncio.Queue()
     v.subscribe(q.put_nowait)
     assert (await q.get())["sim_mover-velocity"]["value"] == 1.0
     await v.set(2.0)
     assert (await q.get())["sim_mover-velocity"]["value"] == 2.0
     v.clear_sub(q.put_nowait)
     await v.set(3.0)
@@ -158,17 +185,14 @@
     assert logs[1].message == ("signal ca://PRE:Mode timed out")
     assert s.name == "sensor"
 
 
 async def test_read_sensor(sim_sensor: demo.Sensor):
     sim_sensor.stage()
     assert (await sim_sensor.read())["sim_sensor-value"]["value"] == 0
-    assert (await sim_sensor.describe())["sim_sensor-value"][
-        "source"
-    ] == "sim://SIM:SENSOR:Value"
     assert (await sim_sensor.read_configuration())["sim_sensor-mode"][
         "value"
     ] == demo.EnergyMode.low
     desc = (await sim_sensor.describe_configuration())["sim_sensor-mode"]
     assert desc["dtype"] == "string"
     assert desc["choices"] == ["Low Energy", "High Energy"]  # type: ignore
     set_sim_value(sim_sensor.mode, demo.EnergyMode.high)
@@ -198,7 +222,75 @@
     def my_plan():
         sim_mover.move(0)
         return
         yield
 
     with pytest.raises(RuntimeError, match="Will deadlock run engine if run in a plan"):
         RE(my_plan())
+
+
+async def test_dynamic_sensor_group_disconnected():
+    with pytest.raises(NotConnected):
+        async with DeviceCollector(timeout=0.1):
+            sim_sensor_group_dynamic = demo.SensorGroup("SIM:SENSOR:")
+
+    assert sim_sensor_group_dynamic.name == "sim_sensor_group_dynamic"
+
+
+async def test_dynamic_sensor_group_read_and_describe(
+    sim_sensor_group: demo.SensorGroup,
+):
+    set_sim_value(sim_sensor_group.sensors[1].value, 0.0)
+    set_sim_value(sim_sensor_group.sensors[2].value, 0.5)
+    set_sim_value(sim_sensor_group.sensors[3].value, 1.0)
+
+    await sim_sensor_group.stage()
+    description = await sim_sensor_group.describe()
+    reading = await sim_sensor_group.read()
+    await sim_sensor_group.unstage()
+
+    assert description == {
+        "sim_sensor_group-sensors-1-value": {
+            "dtype": "number",
+            "shape": [],
+            "source": "soft://sim_sensor_group-sensors-1-value",
+        },
+        "sim_sensor_group-sensors-2-value": {
+            "dtype": "number",
+            "shape": [],
+            "source": "soft://sim_sensor_group-sensors-2-value",
+        },
+        "sim_sensor_group-sensors-3-value": {
+            "dtype": "number",
+            "shape": [],
+            "source": "soft://sim_sensor_group-sensors-3-value",
+        },
+    }
+    assert reading == {
+        "sim_sensor_group-sensors-1-value": {
+            "alarm_severity": 0,
+            "timestamp": ANY,
+            "value": 0.0,
+        },
+        "sim_sensor_group-sensors-2-value": {
+            "alarm_severity": 0,
+            "timestamp": ANY,
+            "value": 0.5,
+        },
+        "sim_sensor_group-sensors-3-value": {
+            "alarm_severity": 0,
+            "timestamp": ANY,
+            "value": 1.0,
+        },
+    }
+
+
+@patch("ophyd_async.epics.demo.subprocess.Popen")
+async def test_ioc_starts(mock_popen: Mock):
+    demo.start_ioc_subprocess()
+    mock_popen.assert_called_once_with(
+        ANY,
+        stdin=subprocess.PIPE,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        universal_newlines=True,
+    )
```

### Comparing `ophyd-async-0.3a1/tests/epics/demo/test_demo_ad_sim_detector.py` & `ophyd_async-0.3a2/tests/epics/demo/test_demo_ad_sim_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,23 +208,22 @@
         "stop",
     ]
 
 
 async def test_read_and_describe_detector(single_detector: StandardDetector):
     describe = await single_detector.describe_configuration()
     read = await single_detector.read_configuration()
-
     assert describe == {
         "test-drv-acquire_time": {
-            "source": "sim://TEST:DRV:AcquireTime_RBV",
+            "source": "soft://test-drv-acquire_time",
             "dtype": "number",
             "shape": [],
         },
         "test-drv-acquire": {
-            "source": "sim://TEST:DRV:Acquire_RBV",
+            "source": "soft://test-drv-acquire",
             "dtype": "boolean",
             "shape": [],
         },
     }
     assert read == {
         "test-drv-acquire_time": {
             "value": 0.0,
```

### Comparing `ophyd-async-0.3a1/tests/epics/motion/test_motor.py` & `ophyd_async-0.3a2/tests/epics/motion/test_motor.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 @pytest.fixture
 async def sim_motor():
     async with DeviceCollector(sim=True):
         sim_motor = motor.Motor("BLxxI-MO-TABLE-01:X")
         # Signals connected here
 
     assert sim_motor.name == "sim_motor"
-    set_sim_value(sim_motor.units, "mm")
+    set_sim_value(sim_motor.motor_egu, "mm")
     set_sim_value(sim_motor.precision, 3)
     set_sim_value(sim_motor.velocity, 1)
     yield sim_motor
 
 
 async def test_motor_moving_well(sim_motor: motor.Motor) -> None:
-    set_sim_put_proceeds(sim_motor.setpoint, False)
+    set_sim_put_proceeds(sim_motor.user_setpoint, False)
     s = sim_motor.set(0.55)
     watcher = Mock()
     s.watch(watcher)
     done = Mock()
     s.add_callback(done)
     await asyncio.sleep(A_BIT)
     assert watcher.call_count == 1
@@ -41,69 +41,65 @@
         initial=0.0,
         target=0.55,
         unit="mm",
         precision=3,
         time_elapsed=pytest.approx(0.0, abs=0.05),
     )
     watcher.reset_mock()
-    assert 0.55 == await sim_motor.setpoint.get_value()
+    assert 0.55 == await sim_motor.user_setpoint.get_value()
     assert not s.done
     await asyncio.sleep(0.1)
-    set_sim_value(sim_motor.readback, 0.1)
+    set_sim_value(sim_motor.user_readback, 0.1)
     assert watcher.call_count == 1
     assert watcher.call_args == call(
         name="sim_motor",
         current=0.1,
         initial=0.0,
         target=0.55,
         unit="mm",
         precision=3,
         time_elapsed=pytest.approx(0.1, abs=0.05),
     )
-    set_sim_put_proceeds(sim_motor.setpoint, True)
+    set_sim_put_proceeds(sim_motor.user_setpoint, True)
     await asyncio.sleep(A_BIT)
     assert s.done
     done.assert_called_once_with(s)
 
 
 async def test_motor_moving_stopped(sim_motor: motor.Motor):
-    set_sim_put_proceeds(sim_motor.setpoint, False)
+    set_sim_put_proceeds(sim_motor.user_setpoint, False)
     s = sim_motor.set(1.5)
     s.add_callback(Mock())
     await asyncio.sleep(0.2)
     assert not s.done
     await sim_motor.stop()
-    set_sim_put_proceeds(sim_motor.setpoint, True)
+    set_sim_put_proceeds(sim_motor.user_setpoint, True)
     await asyncio.sleep(A_BIT)
     assert s.done
     assert s.success is False
 
 
 async def test_read_motor(sim_motor: motor.Motor):
     sim_motor.stage()
     assert (await sim_motor.read())["sim_motor"]["value"] == 0.0
-    assert (await sim_motor.describe())["sim_motor"][
-        "source"
-    ] == "sim://BLxxI-MO-TABLE-01:X.RBV"
     assert (await sim_motor.read_configuration())["sim_motor-velocity"]["value"] == 1
-    assert (await sim_motor.describe_configuration())["sim_motor-units"]["shape"] == []
-    set_sim_value(sim_motor.readback, 0.5)
+    assert (await sim_motor.describe_configuration())["sim_motor-motor_egu"][
+        "shape"
+    ] == []
+    set_sim_value(sim_motor.user_readback, 0.5)
     assert (await sim_motor.read())["sim_motor"]["value"] == 0.5
     sim_motor.unstage()
     # Check we can still read and describe when not staged
-    set_sim_value(sim_motor.readback, 0.1)
+    set_sim_value(sim_motor.user_readback, 0.1)
     assert (await sim_motor.read())["sim_motor"]["value"] == 0.1
     assert await sim_motor.describe()
 
 
 async def test_set_velocity(sim_motor: motor.Motor) -> None:
     v = sim_motor.velocity
-    assert (await v.describe())["sim_motor-velocity"][
-        "source"
-    ] == "sim://BLxxI-MO-TABLE-01:X.VELO"
     q: asyncio.Queue[Dict[str, Reading]] = asyncio.Queue()
     v.subscribe(q.put_nowait)
     assert (await q.get())["sim_motor-velocity"]["value"] == 1.0
     await v.set(2.0)
     assert (await q.get())["sim_motor-velocity"]["value"] == 2.0
     v.clear_sub(q.put_nowait)
     await v.set(3.0)
```

### Comparing `ophyd-async-0.3a1/tests/epics/test_records.db` & `ophyd_async-0.3a2/tests/epics/test_records.db`

 * *Files identical despite different names*

### Comparing `ophyd-async-0.3a1/tests/epics/test_signals.py` & `ophyd_async-0.3a2/tests/epics/test_signals.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,22 @@
 import pytest
 from aioca import CANothing, purge_channel_caches
 from bluesky.protocols import Reading
 
 from ophyd_async.core import SignalBackend, T, get_dtype, load_from_yaml, save_to_yaml
 from ophyd_async.core.utils import NotConnected
 from ophyd_async.epics.signal._epics_transport import EpicsTransport
-from ophyd_async.epics.signal.signal import _make_backend
+from ophyd_async.epics.signal.signal import (
+    _make_backend,
+    epics_signal_r,
+    epics_signal_rw,
+    epics_signal_rw_rbv,
+    epics_signal_w,
+    epics_signal_x,
+)
 
 RECORDS = str(Path(__file__).parent / "test_records.db")
 PV_PREFIX = "".join(random.choice(string.ascii_lowercase) for _ in range(12))
 
 
 @dataclass
 class IOC:
@@ -121,16 +128,18 @@
     datatype: Optional[Type[T]] = None,
 ):
     backend = await ioc.make_backend(datatype, suffix)
     # Make a monitor queue that will monitor for updates
     q = MonitorQueue(backend)
     try:
         # Check descriptor
-        source = f"{ioc.protocol}://{PV_PREFIX}:{ioc.protocol}:{suffix}"
-        assert dict(source=source, **descriptor) == await backend.get_descriptor()
+        pv_name = f"{ioc.protocol}://{PV_PREFIX}:{ioc.protocol}:{suffix}"
+        assert dict(source=pv_name, **descriptor) == await backend.get_descriptor(
+            pv_name
+        )
         # Check initial value
         await q.assert_updates(pytest.approx(initial_value))
         # Put to new value and check that
         await backend.put(put_value)
         await q.assert_updates(pytest.approx(put_value))
     finally:
         q.close()
@@ -153,31 +162,31 @@
 class MyEnum(str, Enum):
     a = "Aaa"
     b = "Bbb"
     c = "Ccc"
 
 
 def integer_d(value):
-    return dict(dtype="integer", shape=[])
+    return {"dtype": "integer", "shape": []}
 
 
 def number_d(value):
-    return dict(dtype="number", shape=[])
+    return {"dtype": "number", "shape": []}
 
 
 def string_d(value):
-    return dict(dtype="string", shape=[])
+    return {"dtype": "string", "shape": []}
 
 
 def enum_d(value):
-    return dict(dtype="string", shape=[], choices=["Aaa", "Bbb", "Ccc"])
+    return {"dtype": "string", "shape": [], "choices": ["Aaa", "Bbb", "Ccc"]}
 
 
 def waveform_d(value):
-    return dict(dtype="array", shape=[len(value)])
+    return {"dtype": "array", "shape": [len(value)]}
 
 
 ls1 = "a string that is just longer than forty characters"
 ls2 = "another string that is just longer than forty characters"
 
 ca_dtype_mapping = {
     np.int8: np.uint8,
@@ -318,15 +327,18 @@
 
 @pytest.mark.parametrize(
     "typ, suff, error",
     [
         (
             BadEnum,
             "enum",
-            "has choices ('Aaa', 'Bbb', 'Ccc'): not all in ('Aaa', 'B', 'Ccc')",
+            (
+                "has choices ('Aaa', 'Bbb', 'Ccc'), which do not match "
+                "<enum 'BadEnum'>, which has ('Aaa', 'B', 'Ccc')"
+            ),
         ),
         (int, "str", "has type str not int"),
         (str, "float", "has type float not str"),
         (str, "stra", "has type [str] not str"),
         (int, "uint8a", "has type [uint8] not int"),
         (float, "enum", "has type Enum not float"),
         (npt.NDArray[np.int32], "float64a", "has type [float64] not [int32]"),
@@ -385,23 +397,25 @@
         bool=np.array([True, False], np.bool_),
         int=np.array([-5, 32], np.int32),
         float=np.array([8.5, -6.97], np.float64),
         str=["Hello", "Bat"],
         enum=[MyEnum.c, MyEnum.b],
     )
     # TODO: what should this be for a variable length table?
-    descriptor = dict(dtype="object", shape=[])
+    descriptor = {"dtype": "object", "shape": []}
     # Make and connect the backend
     for t, i, p in [(MyTable, initial, put), (None, put, initial)]:
         backend = await ioc.make_backend(t, "table")
         # Make a monitor queue that will monitor for updates
         q = MonitorQueue(backend)
         try:
             # Check descriptor
-            dict(source=backend.source, **descriptor) == await backend.get_descriptor()
+            dict(source="test-source", **descriptor) == await backend.get_descriptor(
+                "test-source"
+            )
             # Check initial value
             await q.assert_updates(approx_table(i))
             # Put to new value and check that
             await backend.put(p)
             await q.assert_updates(approx_table(p))
         finally:
             q.close()
@@ -428,15 +442,15 @@
         },
         "record": ANY,
     }
 
     try:
         # Check descriptor
         with pytest.raises(NotImplementedError):
-            await backend.get_descriptor()
+            await backend.get_descriptor("")
         # Check initial value
         await q.assert_updates(expected)
         await backend.get_value()
 
     finally:
         q.close()
 
@@ -455,18 +469,18 @@
     # not supporting direct writes to NDArray at the moment.
     raw_data_backend = await ioc.make_backend(npt.NDArray[np.int64], "ntndarray:data")
 
     # Make a monitor queue that will monitor for updates
     for i, p in [(initial, put), (put, initial)]:
         with closing(MonitorQueue(backend)) as q:
             assert {
-                "source": backend.source,
+                "source": "test-source",
                 "dtype": "array",
                 "shape": [2, 3],
-            } == await backend.get_descriptor()
+            } == await backend.get_descriptor("test-source")
             # Check initial value
             await q.assert_updates(pytest.approx(i))
             await raw_data_backend.put(p.flatten())
             await q.assert_updates(pytest.approx(p))
 
 
 async def test_writing_to_ndarray_raises_typeerror(ioc: IOC):
@@ -480,20 +494,46 @@
         await backend.put(np.zeros((6,), dtype=np.int64))
 
 
 async def test_non_existent_errors(ioc: IOC):
     backend = await ioc.make_backend(str, "non-existent", connect=False)
     # Can't use asyncio.wait_for on python3.8 because of
     # https://github.com/python/cpython/issues/84787
-
-    with pytest.raises(NotConnected, match=backend.source):
+    with pytest.raises(NotConnected):
         await backend.connect(timeout=0.1)
 
 
 def test_make_backend_fails_for_different_transports():
     read_pv = "test"
     write_pv = "pva://test"
 
     with pytest.raises(TypeError) as err:
         _make_backend(str, read_pv, write_pv)
         assert err.args[0] == f"Differing transports: {read_pv} has EpicsTransport.ca,"
         +" {write_pv} has EpicsTransport.pva"
+
+
+def test_signal_helpers():
+    read_write = epics_signal_rw(int, "ReadWrite")
+    assert read_write._backend.read_pv == "ReadWrite"
+    assert read_write._backend.write_pv == "ReadWrite"
+
+    read_write_rbv_manual = epics_signal_rw(int, "ReadWrite_RBV", "ReadWrite")
+    assert read_write_rbv_manual._backend.read_pv == "ReadWrite_RBV"
+    assert read_write_rbv_manual._backend.write_pv == "ReadWrite"
+
+    read_write_rbv = epics_signal_rw_rbv(int, "ReadWrite")
+    assert read_write_rbv._backend.read_pv == "ReadWrite_RBV"
+    assert read_write_rbv._backend.write_pv == "ReadWrite"
+
+    read_write_rbv_suffix = epics_signal_rw_rbv(int, "ReadWrite", read_suffix=":RBV")
+    assert read_write_rbv_suffix._backend.read_pv == "ReadWrite:RBV"
+    assert read_write_rbv_suffix._backend.write_pv == "ReadWrite"
+
+    read = epics_signal_r(int, "Read")
+    assert read._backend.read_pv == "Read"
+
+    write = epics_signal_w(int, "Write")
+    assert write._backend.write_pv == "Write"
+
+    execute = epics_signal_x("Execute")
+    assert execute._backend.write_pv == "Execute"
```

### Comparing `ophyd-async-0.3a1/tests/panda/db/panda.db` & `ophyd_async-0.3a2/tests/panda/db/panda.db`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,74 @@
                 "+channel": "NAME",
                 "+type": "plain"
             }
         }
     })
 }
 
+record(longin, "$(IOC_NAME=PANDAQSRV):SEQ1:REPEATS")
+{
+    field(PINI, "YES")
+    info(Q:group, {
+        "$(IOC_NAME=PANDAQSRV):SEQ1:PVI": {
+            "pvi.repeats.rw": {
+                "+channel": "NAME",
+                "+type": "plain"
+            }
+        }
+    })
+}
+
+record(ai, "$(IOC_NAME=PANDAQSRV):SEQ1:PRESCALE")
+{
+    field(PINI, "YES")
+    info(Q:group, {
+        "$(IOC_NAME=PANDAQSRV):SEQ1:PVI": {
+            "pvi.prescale.rw": {
+                "+channel": "NAME",
+                "+type": "plain"
+            }
+        }
+    })
+}
+
+record(mbbi, "$(IOC_NAME=PANDAQSRV):SEQ1:PRESCALE:UNITS")
+{
+    field(ZRST, "min")
+    field(ZRVL, "0")
+    field(ONST, "s")
+    field(ONVL, "1")
+    field(TWST, "ms")
+    field(TWVL, "2")
+    field(THST, "us")
+    field(THVL, "3")
+    field(PINI, "YES")
+    info(Q:group, {
+        "$(IOC_NAME=PANDAQSRV):SEQ1:PVI": {
+            "pvi.prescale_units.rw": {
+                "+channel": "NAME",
+                "+type": "plain"
+            }
+        }
+    })
+}
+
+record(stringout, "$(IOC_NAME=PANDAQSRV):SEQ1:ENABLE")
+{
+    field(PINI, "YES")
+    info(Q:group, {
+        "$(IOC_NAME=PANDAQSRV):SEQ1:PVI": {
+            "pvi.enable.rw": {
+                "+channel": "NAME",
+                "+type": "plain"
+            }
+        }
+    })
+}
+
 record(bi, "$(IOC_NAME=PANDAQSRV):PCAP:ACTIVE")
 {
     field(ZNAM,  "0")
     field(ONAM,  "1")
     field(PINI, "YES")
     info(Q:group, {
         "$(IOC_NAME=PANDAQSRV):PCAP:PVI": {
```

### Comparing `ophyd-async-0.3a1/tests/panda/test_table.py` & `ophyd_async-0.3a2/tests/panda/test_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pytest
 
-from ophyd_async.panda.table import seq_table_from_arrays
+from ophyd_async.panda._table import seq_table_from_arrays
 
 
 def test_from_arrays_inconsistent_lengths():
     length = 4
     time2 = np.zeros(length)
     time1 = np.zeros(length + 1)
     with pytest.raises(ValueError, match="time1: has length 5 not 4"):
```

