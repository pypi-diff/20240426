# Comparing `tmp/rad-0.19.2.tar.gz` & `tmp/rad-0.19.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-0.19.2.tar", last modified: Wed Apr 17 15:33:51 2024, max compression
+gzip compressed data, was "rad-0.19.3.tar", last modified: Fri Apr 26 14:01:09 2024, max compression
```

## Comparing `rad-0.19.2.tar` & `rad-0.19.3.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.016332 rad-0.19.2/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-17 15:33:33.000000 rad-0.19.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:50.996333 rad-0.19.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-17 15:33:33.000000 rad-0.19.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-17 15:33:33.000000 rad-0.19.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:50.996333 rad-0.19.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 15:33:33.000000 rad-0.19.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-17 15:33:33.000000 rad-0.19.2/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-17 15:33:33.000000 rad-0.19.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-17 15:33:33.000000 rad-0.19.2/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-17 15:33:33.000000 rad-0.19.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-17 15:33:33.000000 rad-0.19.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-17 15:33:33.000000 rad-0.19.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 15:33:33.000000 rad-0.19.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-04-17 15:33:33.000000 rad-0.19.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-17 15:33:33.000000 rad-0.19.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-17 15:33:33.000000 rad-0.19.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-17 15:33:33.000000 rad-0.19.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:33.000000 rad-0.19.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-17 15:33:51.016332 rad-0.19.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-17 15:33:33.000000 rad-0.19.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-17 15:33:33.000000 rad-0.19.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-17 15:33:33.000000 rad-0.19.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    59966 2024-04-17 15:33:33.000000 rad-0.19.2/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:50.992333 rad-0.19.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-17 15:33:33.000000 rad-0.19.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-17 15:33:33.000000 rad-0.19.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-17 15:33:33.000000 rad-0.19.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 15:33:33.000000 rad-0.19.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-17 15:33:33.000000 rad-0.19.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-17 15:33:33.000000 rad-0.19.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-04-17 15:33:33.000000 rad-0.19.2/docs/creating.rst
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 15:33:33.000000 rad-0.19.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-17 15:33:33.000000 rad-0.19.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 15:33:33.000000 rad-0.19.2/docs/manifests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-17 15:33:33.000000 rad-0.19.2/docs/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-17 15:33:33.000000 rad-0.19.2/docs/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-17 15:33:33.000000 rad-0.19.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-04-17 15:33:33.000000 rad-0.19.2/scripts/insert_next_release.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      954 2024-04-17 15:33:33.000000 rad-0.19.2/scripts/set_release_date.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:33:51.016332 rad-0.19.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:50.992333 rad-0.19.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/src/rad/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/src/rad/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/src/rad/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/manifests/datamodels-1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.012333 rad-0.19.2/src/rad/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/aperture-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/base_exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/base_guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/cal_logs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/coordinates-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/ephemeris-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/fps-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/ground_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/groundtest-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/guidewindow-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/msos_stack-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/observation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/outlier_detection-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/photometry-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/pointing-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/program-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/rad_schema-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/ramp-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/ref_file-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.012333 rad-0.19.2/src/rad/resources/schemas/reference_files/
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/resample-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/segmentation_map-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/source_catalog-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/source_detection-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.016332 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/target-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tvac-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/visit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_image-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.016332 rad-0.19.2/src/rad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.016332 rad-0.19.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:33.000000 rad-0.19.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-17 15:33:33.000000 rad-0.19.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-17 15:33:33.000000 rad-0.19.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-17 15:33:33.000000 rad-0.19.2/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-17 15:33:33.000000 rad-0.19.2/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-17 15:33:33.000000 rad-0.19.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.142450 rad-0.19.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-26 14:00:57.000000 rad-0.19.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.118450 rad-0.19.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-26 14:00:57.000000 rad-0.19.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-26 14:00:57.000000 rad-0.19.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.122450 rad-0.19.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-26 14:00:57.000000 rad-0.19.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-26 14:00:57.000000 rad-0.19.3/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-26 14:00:57.000000 rad-0.19.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-26 14:00:57.000000 rad-0.19.3/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-26 14:00:57.000000 rad-0.19.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-26 14:00:57.000000 rad-0.19.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-26 14:00:57.000000 rad-0.19.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 14:00:57.000000 rad-0.19.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-04-26 14:00:57.000000 rad-0.19.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-26 14:00:57.000000 rad-0.19.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-26 14:00:57.000000 rad-0.19.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-26 14:00:57.000000 rad-0.19.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:00:57.000000 rad-0.19.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-26 14:01:09.142450 rad-0.19.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-26 14:00:57.000000 rad-0.19.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.122450 rad-0.19.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-26 14:00:57.000000 rad-0.19.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.122450 rad-0.19.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-26 14:00:57.000000 rad-0.19.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    59966 2024-04-26 14:00:57.000000 rad-0.19.3/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.118450 rad-0.19.3/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.122450 rad-0.19.3/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-26 14:00:57.000000 rad-0.19.3/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-26 14:00:57.000000 rad-0.19.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 14:00:57.000000 rad-0.19.3/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-26 14:00:57.000000 rad-0.19.3/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-26 14:00:57.000000 rad-0.19.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-26 14:00:57.000000 rad-0.19.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-04-26 14:00:57.000000 rad-0.19.3/docs/creating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-26 14:00:57.000000 rad-0.19.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-26 14:00:57.000000 rad-0.19.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 14:00:57.000000 rad-0.19.3/docs/manifests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-26 14:00:57.000000 rad-0.19.3/docs/reference_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-26 14:00:57.000000 rad-0.19.3/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-26 14:00:57.000000 rad-0.19.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.122450 rad-0.19.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-04-26 14:00:57.000000 rad-0.19.3/scripts/insert_next_release.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      954 2024-04-26 14:00:57.000000 rad-0.19.3/scripts/set_release_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:01:09.142450 rad-0.19.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.118450 rad-0.19.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.126450 rad-0.19.3/src/rad/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.126450 rad-0.19.3/src/rad/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.126450 rad-0.19.3/src/rad/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/manifests/datamodels-1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.134450 rad-0.19.3/src/rad/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/aperture-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/base_exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/base_guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/cal_logs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/coordinates-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/ephemeris-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/fps-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/ground_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/groundtest-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/guidewindow-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/msos_stack-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/observation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/outlier_detection-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/photometry-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/pointing-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/program-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/rad_schema-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/ramp-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/ref_file-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.138450 rad-0.19.3/src/rad/resources/schemas/reference_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/resample-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/segmentation_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/source_catalog-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/source_detection-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.138450 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/target-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tvac-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/visit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_image-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.138450 rad-0.19.3/src/rad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.138450 rad-0.19.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:00:57.000000 rad-0.19.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 14:00:57.000000 rad-0.19.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-26 14:00:57.000000 rad-0.19.3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-26 14:00:57.000000 rad-0.19.3/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-26 14:00:57.000000 rad-0.19.3/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-26 14:00:57.000000 rad-0.19.3/tox.ini
```

### Comparing `rad-0.19.2/.github/pull_request_template.md` & `rad-0.19.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/.github/workflows/changelog.yml` & `rad-0.19.3/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/.github/workflows/ci_cron.yml` & `rad-0.19.3/.github/workflows/ci_cron.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/.github/workflows/release.yml` & `rad-0.19.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/.gitignore` & `rad-0.19.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/.pre-commit-config.yaml` & `rad-0.19.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/CHANGES.rst` & `rad-0.19.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-0.19.3 (unreleased)
+0.19.4 (unreleased)
 -------------------
 
-- 
+
+
+0.19.3 (2024-04-25)
+-------------------
+
+- Duplicated the keywords from groundtest to tvac_groundtest. [#409]
+
 
 0.19.2 (2024-04-17)
 -------------------
 
 - Duplicated the keywords from base_exposure to exposure and similarly for base_guidestar and guidestar. [#406]
 
 0.19.1 (2024-04-04)
```

### Comparing `rad-0.19.2/CODE_OF_CONDUCT.md` & `rad-0.19.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/LICENSE` & `rad-0.19.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/PKG-INFO` & `rad-0.19.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.19.2
+Version: 0.19.3
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.19.2/README.md` & `rad-0.19.3/README.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/docs/Makefile` & `rad-0.19.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/docs/_static/custom.css` & `rad-0.19.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/docs/_static/stsci_logo.png` & `rad-0.19.3/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/docs/conf.py` & `rad-0.19.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/docs/creating.rst` & `rad-0.19.3/docs/creating.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/docs/index.rst` & `rad-0.19.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/docs/make.bat` & `rad-0.19.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/docs/reference_files.rst` & `rad-0.19.3/docs/reference_files.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/docs/schemas.rst` & `rad-0.19.3/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/pyproject.toml` & `rad-0.19.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/scripts/insert_next_release.py` & `rad-0.19.3/scripts/insert_next_release.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/scripts/set_release_date.py` & `rad-0.19.3/scripts/set_release_date.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/integration.py` & `rad-0.19.3/src/rad/integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/manifests/datamodels-1.0.yaml` & `rad-0.19.3/src/rad/resources/manifests/datamodels-1.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/aperture-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/aperture-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/associations-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/associations-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/base_exposure-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/base_exposure-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/base_guidestar-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/base_guidestar-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/basic-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/common-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/coordinates-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/coordinates-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/ephemeris-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/ephemeris-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/exposure-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/exposure-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/exposure_type-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/fps-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/fps-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/ground_common-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/ground_common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/groundtest-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/groundtest-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/guidestar-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/guidestar-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/guidewindow-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/guidewindow-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/msos_stack-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/msos_stack-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/observation-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/observation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/photometry-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/photometry-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/pointing-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/pointing-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/program-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/program-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/rad_schema-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/rad_schema-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/ramp-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/ramp-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/ref_file-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/ref_file-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/resample-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/resample-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/segmentation_map-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/segmentation_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/source_catalog-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/source_catalog-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/target-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/target-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/tvac-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/tvac-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,345 +1,483 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/tvac_groundtest-1.0.0
 
 title: TVAC Ground Test Information
-allOf:
-  - $ref: asdf://stsci.edu/datamodels/roman/schemas/groundtest-1.0.0
-  - type: object
-    properties:
-      activity_number:
-        title: TVAC Activity Number
-        type: integer
-        archive_catalog:
-          datatype: int
-          destination: [WFITvac.activity_number]
-      led_bank1_band_number_on:
-        title: Band number of LED illuminating in the sRCS in bank 1
-        type: array
-        items:
-          type: integer
-      led_bank2_bank1_number_on:
-        title: Band number of LED illuminating in the sRCS in bank 2
-        type: array
-        items:
-          type: integer
-      led_bank1_approx_wlen:
-        title: Approximate wavelength of LED illuminating in the sRCS in bank 1
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          value:
-            tag: tag:stsci.edu:asdf/core/ndarray-1.*
-            datatype: float64
-            exact_datatype: true
-            # needs ndim
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: ["nm"]
-      led_bank2_approx_wlen:
-        title: Approximate wavelength of LED illuminating in the sRCS in bank 2
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          value:
-            tag: tag:stsci.edu:asdf/core/ndarray-1.*
-            datatype: float64
-            exact_datatype: true
-            # needs ndim
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: ["nm"]
-      srcs_pd_voltage:
-        title: sRCS Photodiode Voltage
-        type: number
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.srcs_pd_voltage]
-      srcs_led_flux:
-        title: Target flux for the sRCS LEDs
-        type: number
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.srcs_led_flux]
-      wfi_mce_srcs_bank1_led_i:
-        title: |
-          Commanded current for the SRCS -> GSFC will send us the flux
-          in target e-/s/px in the center of the sca
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: ["A"]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.wfi_mce_srcs_bank1_led_i]
-      wfi_mce_srcs_bank1_led_range:
-        title: |
-          Commanded range for the SRCS -> GSFC will send us the flux in
-          target e-/s/px in the center of the sca
-        type: string
-        # enum: [] add enum values
-        archive_catalog:
-          datatype: nvarchar(80)
-          destination: [WFITvac.wfi_mce_srcs_bank1_led_range]
-      wfi_mce_srcs_bank2_led_i:
-        title: |
-          Commanded current for the SRCS -> GSFC will send us the flux
-          in target e-/s/px in the center of the sca
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: ["A"]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.wfi_mce_srcs_bank2_led_i]
-      wfi_mce_srcs_bank2_led_range:
-        title: |
-          Commanded range for the SRCS -> GSFC will send us the flux in
-          target e-/s/px in the center of the sca
-        type: string
-        # enum: [] add enum values
-        archive_catalog:
-          datatype: nvarchar(80)
-          destination: [WFITvac.wfi_mce_srcs_bank2_led_range]
-      srcs_led_current:
-        title: Input LED current set point
-        type: number
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.srcs_led_current]
-      wfi_opt_targettype:
-        title: WFI-team defined target types
-        type: string
-        enum: [NONE, FLAT-sRCS, FLAT-SORC, POINT SOURCE, SPECTRUM, DARK,
-                DARK-DARKEL, DARK-W146, PHARET-GW, PHARET-FF, PHARET-FF-F158,
-                PHARET-FF-M3MM, PHARET-FF-M6MM, PHARET-FF-P3MM, PHARET-FF-P6MM,
-                PHARET-FF-PRISM, PHARET-FF-W146, POINT-SOURCE-GW, STRAY LIGHT]
-        archive_catalog:
-          datatype: nvarchar(20)
-          destination: [WFITvac.wfi_opt_targettype]
-      analysis_tag:
-        title: WFI-team defined tags for data aggregation/analysis
-        type: string
-        archive_catalog:
-          datatype: nvarchar(32)
-          destination: [WFITvac.analysis_tag]
-      gsorc_pose_mode:
-        title: SORC pose mode
-        type: string
-        # enum: [] add enum values
-        archive_catalog:
-          datatype: nvarchar(20)
-          destination: [WFITvac.gsorc_pose_mode]
-      gsorc_pose_target:
-        title: SORC pose target
-        type: string
-        # enum: [] add enum values
-        archive_catalog:
-          datatype: nvarchar(20)
-          destination: [WFITvac.gsorc_pose_target]
-      gsorc_sds_active_atten:
-        title: Attenuation from SDS
-        type: number
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.gsorc_sds_active_atten]
-      gsorc_sds_lltfir_wave:
-        title: Commanded wavelength for the LLTF
-        type: number
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.gsorc_sds_lltfir_wave]
-      gsorc_sds_sorc_on:
-        title: SORC on/off
-        type: boolean
-        archive_catalog:
-          datatype: nchar(1)
-          destination: [WFITvac.gsorc_sds_sorc_on]
-      gsorc_sds_sorc_wlen:
-        title: SORC wavelength
-        type: number
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.gsorc_sds_sorc_wlen]
-      gsorc_sds_active_source:
-        title: Laser name
-        type: string
-        archive_catalog:
-          datatype: nvarchar(20)
-          destination: [WFITvac.gsorc_sds_active_source]
-      gsorc_sds_dq_pulse:
-        title: whether the source is pulsing or not
-        type: string
-        enum: [pulse, cw]
-        archive_catalog:
-          datatype: nvarchar(10)
-          destination: [WFITvac.gsorc_sds_dq_pulse]
-      gsorc_sds_daq_pw:
-        title: pulse width – originally in HDF5 file is in units of 0.1 ms
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [ms]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.gsorc_sds_daq_pw]
-      gsorc_heater1_setpt:
-        title: SORC temperature set point
-        type: number
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.gsorc_heater1_setpt]
-      wfi_otp_wfi_ewa:
-        title: Element Wheel position
-        type: string
-        # enum: [] add enum values
-        archive_catalog:
-          datatype: nvarchar(15)
-          destination: [WFITvac.wfi_otp_wfi_ewa]
-      sca_temp:
-        title: SCE temperature
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [K]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.sca_temp]
-      mpa_temp:
-        title: MPA temperature
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [K]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.mpa_temp]
-      ewa_temp:
-        title: ewa temp ish (there's no actual temperature sensor inside)
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [K]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.ewa_temp]
-      ewta_outer_heater_temp:
-        title: ewa_outer temperature sensor
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [K]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.ewta_outer_heater_temp]
-      ewta_inner_heater_temp:
-        title: ewa_inner temperature sensor
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [K]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.ewta_inner_heater_temp]
-      coba_temp_near_ewta:
-        title: COBA temperature near element wheel
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [K]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.coba_temp_near_ewta]
-      scea_temp:
-        title: SCEA temperature
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [K]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.scea_temp]
-      wfi_sce_1_vbiasgate_v:
-        title: SCE gate voltage bias.
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [V]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.wfi_sce_1_vbiasgate_v]
-      wfi_sce_1_vbiaspwr_i:
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [A]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.wfi_sce_1_vbiaspwr_i]
-      wfi_sce_1_vbiaspwr_v:
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [V]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.wfi_sce_1_vbiaspwr_v]
-      wfi_sce_1_vreset_v:
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [V]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.wfi_sce_1_vreset_v]
-      wfi_sce_1_vreset_i:
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [A]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.wfi_sce_1_vreset_i]
-      wfi_mcu_a_offs_csense_fpssen:
-        title: temperature in eng units -> will change for TVAC2.
-        tag: tag:stsci.edu:asdf/unit/quantity-1.*
-        properties:
-          # needs a datatype
-          unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.*
-            enum: [K]
-        archive_catalog:
-          datatype: float
-          destination: [WFITvac.wfi_mcu_a_offs_csense_fpssen]
-
+type: object
+properties:
+  test_name:
+    title: I&T Test Name
+    type: string
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFICommon.test_name]
+  test_phase:
+    title: I&T Testing Phase
+    type: string
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFICommon.test_phase]
+  test_environment:
+    title: I&T Testing Environment
+    type: string
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFICommon.test_environment]
+  test_script:
+    title: Name of Testing Script Run
+    type: string
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFICommon.test_script]
+  product_date:
+    title: Source File Creation Time
+    tag: tag:stsci.edu:asdf/time/time-1.*
+    archive_catalog:
+      datatype: datetime2
+      destination: [WFICommon.product_date]
+  product_version:
+    title: I&T Software Used to Generate Source File
+    type: string
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFICommon.product_version]
+  conversion_date:
+    title: HDF5 to ASDF Conversion Date
+    tag: tag:stsci.edu:asdf/time/time-1.*
+    archive_catalog:
+      datatype: datetime2
+      destination: [WFICommon.conversion_date]
+  conversion_version:
+    title: HDF5 to ASDF Converter Version
+    type: string
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFICommon.conversion_version]
+  filename_pnt5:
+    title: L0.5 File Name
+    type: string
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFICommon.filename_pnt5]
+  filepath_level_pnt5:
+    title: L0.5 File Path
+    type: string
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFICommon.filepath_level_pnt5]
+  filename_l1a:
+    title: L1A File Name
+    type: string
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFICommon.filename_l1a]
+  detector_id:
+    title: SCA Identifier
+    type: string
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFICommon.detector_id]
+  detector_temp:
+    title: Mean Detector Temperature (Kelvin)
+    type: number
+    archive_catalog:
+      datatype: float
+      destination: [WFICommon.detector_temp]
+  frames_temp:
+    title: Interpolated Temperature of Frames (Kelvin)
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
+    datatype: float64
+    exact_datatype: true
+    # needs a ndim
+  ota_temp:
+    title: Mean OTA Temperature (Kelvin)
+    type: number
+    archive_catalog:
+      datatype: float
+      destination: [WFICommon.ota_temp]
+  rcs_on:
+    title: RCS On/Off
+    type: boolean
+    archive_catalog:
+      datatype: nchar(1)
+      destination: [WFICommon.rcs_on]
+  readout_col_num:
+    title: Number of Readout Columns
+    type: integer
+    archive_catalog:
+      datatype: int
+      destination: [WFICommon.readout_col_num]
+  detector_pixel_size:
+    title: Pixel Size (cm)
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: float64
+        exact_datatype: true
+        # needs ndim
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: ["cm"]
+  sensor_error:
+    title: Sensor Error
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
+    datatype: float64
+    exact_datatype: true
+    # needs ndim
+  activity_number:
+    title: TVAC Activity Number
+    type: integer
+    archive_catalog:
+      datatype: int
+      destination: [WFITvac.activity_number]
+  led_bank1_band_number_on:
+    title: Band number of LED illuminating in the sRCS in bank 1
+    type: array
+    items:
+      type: integer
+  led_bank2_bank1_number_on:
+    title: Band number of LED illuminating in the sRCS in bank 2
+    type: array
+    items:
+      type: integer
+  led_bank1_approx_wlen:
+    title: Approximate wavelength of LED illuminating in the sRCS in bank 1
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: float64
+        exact_datatype: true
+        # needs ndim
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: ["nm"]
+  led_bank2_approx_wlen:
+    title: Approximate wavelength of LED illuminating in the sRCS in bank 2
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: float64
+        exact_datatype: true
+        # needs ndim
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: ["nm"]
+  srcs_pd_voltage:
+    title: sRCS Photodiode Voltage
+    type: number
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.srcs_pd_voltage]
+  srcs_led_flux:
+    title: Target flux for the sRCS LEDs
+    type: number
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.srcs_led_flux]
+  wfi_mce_srcs_bank1_led_i:
+    title: |
+      Commanded current for the SRCS -> GSFC will send us the flux
+      in target e-/s/px in the center of the sca
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: ["A"]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.wfi_mce_srcs_bank1_led_i]
+  wfi_mce_srcs_bank1_led_range:
+    title: |
+      Commanded range for the SRCS -> GSFC will send us the flux in
+      target e-/s/px in the center of the sca
+    type: string
+    # enum: [] add enum values
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFITvac.wfi_mce_srcs_bank1_led_range]
+  wfi_mce_srcs_bank2_led_i:
+    title: |
+      Commanded current for the SRCS -> GSFC will send us the flux
+      in target e-/s/px in the center of the sca
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: ["A"]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.wfi_mce_srcs_bank2_led_i]
+  wfi_mce_srcs_bank2_led_range:
+    title: |
+      Commanded range for the SRCS -> GSFC will send us the flux in
+      target e-/s/px in the center of the sca
+    type: string
+    # enum: [] add enum values
+    archive_catalog:
+      datatype: nvarchar(80)
+      destination: [WFITvac.wfi_mce_srcs_bank2_led_range]
+  srcs_led_current:
+    title: Input LED current set point
+    type: number
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.srcs_led_current]
+  wfi_opt_targettype:
+    title: WFI-team defined target types
+    type: string
+    enum: [NONE, FLAT-sRCS, FLAT-SORC, POINT SOURCE, SPECTRUM, DARK,
+            DARK-DARKEL, DARK-W146, PHARET-GW, PHARET-FF, PHARET-FF-F158,
+            PHARET-FF-M3MM, PHARET-FF-M6MM, PHARET-FF-P3MM, PHARET-FF-P6MM,
+            PHARET-FF-PRISM, PHARET-FF-W146, POINT-SOURCE-GW, STRAY LIGHT]
+    archive_catalog:
+      datatype: nvarchar(20)
+      destination: [WFITvac.wfi_opt_targettype]
+  analysis_tag:
+    title: WFI-team defined tags for data aggregation/analysis
+    type: string
+    archive_catalog:
+      datatype: nvarchar(32)
+      destination: [WFITvac.analysis_tag]
+  gsorc_pose_mode:
+    title: SORC pose mode
+    type: string
+    # enum: [] add enum values
+    archive_catalog:
+      datatype: nvarchar(20)
+      destination: [WFITvac.gsorc_pose_mode]
+  gsorc_pose_target:
+    title: SORC pose target
+    type: string
+    # enum: [] add enum values
+    archive_catalog:
+      datatype: nvarchar(20)
+      destination: [WFITvac.gsorc_pose_target]
+  gsorc_sds_active_atten:
+    title: Attenuation from SDS
+    type: number
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.gsorc_sds_active_atten]
+  gsorc_sds_lltfir_wave:
+    title: Commanded wavelength for the LLTF
+    type: number
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.gsorc_sds_lltfir_wave]
+  gsorc_sds_sorc_on:
+    title: SORC on/off
+    type: boolean
+    archive_catalog:
+      datatype: nchar(1)
+      destination: [WFITvac.gsorc_sds_sorc_on]
+  gsorc_sds_sorc_wlen:
+    title: SORC wavelength
+    type: number
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.gsorc_sds_sorc_wlen]
+  gsorc_sds_active_source:
+    title: Laser name
+    type: string
+    archive_catalog:
+      datatype: nvarchar(20)
+      destination: [WFITvac.gsorc_sds_active_source]
+  gsorc_sds_dq_pulse:
+    title: whether the source is pulsing or not
+    type: string
+    enum: [pulse, cw]
+    archive_catalog:
+      datatype: nvarchar(10)
+      destination: [WFITvac.gsorc_sds_dq_pulse]
+  gsorc_sds_daq_pw:
+    title: pulse width – originally in HDF5 file is in units of 0.1 ms
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [ms]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.gsorc_sds_daq_pw]
+  gsorc_heater1_setpt:
+    title: SORC temperature set point
+    type: number
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.gsorc_heater1_setpt]
+  wfi_otp_wfi_ewa:
+    title: Element Wheel position
+    type: string
+    # enum: [] add enum values
+    archive_catalog:
+      datatype: nvarchar(15)
+      destination: [WFITvac.wfi_otp_wfi_ewa]
+  sca_temp:
+    title: SCE temperature
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [K]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.sca_temp]
+  mpa_temp:
+    title: MPA temperature
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [K]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.mpa_temp]
+  ewa_temp:
+    title: ewa temp ish (there's no actual temperature sensor inside)
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [K]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.ewa_temp]
+  ewta_outer_heater_temp:
+    title: ewa_outer temperature sensor
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [K]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.ewta_outer_heater_temp]
+  ewta_inner_heater_temp:
+    title: ewa_inner temperature sensor
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [K]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.ewta_inner_heater_temp]
+  coba_temp_near_ewta:
+    title: COBA temperature near element wheel
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [K]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.coba_temp_near_ewta]
+  scea_temp:
+    title: SCEA temperature
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [K]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.scea_temp]
+  wfi_sce_1_vbiasgate_v:
+    title: SCE gate voltage bias.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [V]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.wfi_sce_1_vbiasgate_v]
+  wfi_sce_1_vbiaspwr_i:
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [A]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.wfi_sce_1_vbiaspwr_i]
+  wfi_sce_1_vbiaspwr_v:
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [V]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.wfi_sce_1_vbiaspwr_v]
+  wfi_sce_1_vreset_v:
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [V]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.wfi_sce_1_vreset_v]
+  wfi_sce_1_vreset_i:
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [A]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.wfi_sce_1_vreset_i]
+  wfi_mcu_a_offs_csense_fpssen:
+    title: temperature in eng units -> will change for TVAC2.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      # needs a datatype
+      unit:
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
+        enum: [K]
+    archive_catalog:
+      datatype: float
+      destination: [WFITvac.wfi_mcu_a_offs_csense_fpssen]
+propertyOrder: [test_name, test_phase, test_environment, test_script,
+                product_date, product_version, conversion_date, conversion_version,
+                filename_pnt5, filepath_level_pnt5, filename_l1a, detector_id,
+                detector_temp, frames_temp, ota_temp, rcs_on, readout_col_num,
+                detector_pixel_size, sensor_error,
+                analysis_tag, sca_temp, gsorc_heater1_setpt, srcs_led_current,
+                gsorc_sds_active_source, wfi_sce_1_vreset_v, ewa_temp, wfi_sce_1_vreset_i,
+                wfi_sce_1_vbiasgate_v, srcs_pd_voltage, gsorc_sds_daq_pw, activity_number,
+                mpa_temp, gsorc_sds_active_atten, gsorc_sds_dq_pulse, ewta_inner_heater_temp,
+                wfi_otp_wfi_ewa, wfi_mce_srcs_bank2_led_i, gsorc_sds_sorc_wlen,
+                gsorc_sds_sorc_on, wfi_mcu_a_offs_csense_fpssen, gsorc_sds_lltfir_wave,
+                wfi_mce_srcs_bank1_led_range, led_bank2_bank1_number_on, wfi_sce_1_vbiaspwr_v,
+                srcs_led_flux, gsorc_pose_mode, wfi_mce_srcs_bank1_led_i, wfi_sce_1_vbiaspwr_i,
+                led_bank2_approx_wlen, wfi_mce_srcs_bank2_led_range, ewta_outer_heater_temp,
+                gsorc_pose_target, led_bank1_band_number_on, led_bank1_approx_wlen,
+                wfi_opt_targettype, scea_temp, coba_temp_near_ewta]
 flowStyle: block
+required: [test_name, test_phase, test_environment, test_script,
+           product_date, product_version, conversion_date, conversion_version,
+           filename_pnt5, filepath_level_pnt5, filename_l1a, detector_id,
+           detector_temp, frames_temp, ota_temp, rcs_on, readout_col_num,
+           detector_pixel_size, sensor_error]
 ...
```

### Comparing `rad-0.19.2/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/visit-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/visit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/wcsinfo-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/wfi_image-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/wfi_image-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/wfi_mode-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/wfi_mode-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml` & `rad-0.19.3/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/src/rad.egg-info/PKG-INFO` & `rad-0.19.3/src/rad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.19.2
+Version: 0.19.3
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.19.2/src/rad.egg-info/SOURCES.txt` & `rad-0.19.3/src/rad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/tests/test_integration.py` & `rad-0.19.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/tests/test_manifest.py` & `rad-0.19.3/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/tests/test_schemas.py` & `rad-0.19.3/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.2/tox.ini` & `rad-0.19.3/tox.ini`

 * *Files identical despite different names*

