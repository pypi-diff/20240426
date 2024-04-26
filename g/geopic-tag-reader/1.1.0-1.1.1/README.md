# Comparing `tmp/geopic_tag_reader-1.1.0.tar.gz` & `tmp/geopic_tag_reader-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopic_tag_reader-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geopic_tag_reader-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geopic_tag_reader-1.1.0.tar` & `geopic_tag_reader-1.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0       56 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/.gitignore
--rw-r--r--   0        0        0     1009 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0       91 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6697 2024-04-17 06:35:08.457091 geopic_tag_reader-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/LICENSE
--rw-r--r--   0        0        0      676 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/Makefile
--rw-r--r--   0        0        0     5243 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/README.md
--rw-r--r--   0        0        0       65 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/.pages
--rw-r--r--   0        0        0     3393 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.0/docs/API_USAGE.md
--rw-r--r--   0        0        0     1835 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/CLI_USAGE.md
--rw-r--r--   0        0        0      999 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/Develop.md
--rw-r--r--   0        0        0     2015 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/Install.md
--rw-r--r--   0        0        0     1066 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/camera.md
--rw-r--r--   0        0        0      529 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.0/docs/model.md
--rw-r--r--   0        0        0     8930 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.0/docs/reader.md
--rw-r--r--   0        0        0     4301 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/docs/writer.md
--rw-r--r--   0        0        0       47 2024-04-17 06:35:08.457091 geopic_tag_reader-1.1.0/geopic_tag_reader/__init__.py
--rw-r--r--   0        0        0     1643 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/geopic_tag_reader/camera.py
--rw-r--r--   0        0        0     3141 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.0/geopic_tag_reader/main.py
--rw-r--r--   0        0        0      129 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/geopic_tag_reader/model.py
--rw-r--r--   0        0        0        0 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/geopic_tag_reader/py.typed
--rw-r--r--   0        0        0    22867 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.0/geopic_tag_reader/reader.py
--rw-r--r--   0        0        0     8672 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.0/geopic_tag_reader/writer.py
--rw-r--r--   0        0        0     1142 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       37 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/pytest.ini
--rw-r--r--   0        0        0        0 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0      195 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0    79729 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/fixtures/1.jpg
--rw-r--r--   0        0        0    24664 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/fixtures/IMG_20210720_144918.jpg
--rw-r--r--   0        0        0    38766 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/fixtures/IMG_20210720_161352.jpg
--rw-r--r--   0        0        0    75709 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.0/tests/fixtures/a1.jpg
--rw-r--r--   0        0        0    29130 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/b1.jpg
--rw-r--r--   0        0        0    39810 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/broken_makernotes.jpg
--rw-r--r--   0        0        0    69903 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/c1.jpg
--rw-r--r--   0        0        0     4867 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/charset.jpg
--rw-r--r--   0        0        0    30503 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/cropped.jpg
--rw-r--r--   0        0        0    33446 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/d1.jpg
--rw-r--r--   0        0        0     5415 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/datetime_ms_float.jpg
--rw-r--r--   0        0        0    35109 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/datetime_offset.jpg
--rw-r--r--   0        0        0    51474 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0    29141 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/flat.jpg
--rw-r--r--   0        0        0    70264 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/gopromax_flat.jpg
--rw-r--r--   0        0        0     4174 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/gps_date_slash.jpg
--rw-r--r--   0        0        0     5237 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/gps_date_time_stamp.jpg
--rw-r--r--   0        0        0    66264 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_Ricoh_Theta.jpg
--rw-r--r--   0        0        0     5360 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_V4MPack.jpg
--rw-r--r--   0        0        0    66961 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_categorisee.jpg
--rw-r--r--   0        0        0   135574 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_datetimeoriginal.jpg
--rw-r--r--   0        0        0    29503 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_gps_date_string.jpg
--rw-r--r--   0        0        0    35282 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.0/tests/fixtures/img_gps_datestamp.jpg
--rw-r--r--   0        0        0    43696 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/img_gps_sotm.jpg
--rw-r--r--   0        0        0    33170 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/img_invalid_gps_date.jpg
--rw-r--r--   0        0        0    34454 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/img_without_coord.jpg
--rw-r--r--   0        0        0    34518 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/img_without_dt.jpg
--rw-r--r--   0        0        0    12643 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/img_without_exif_tags.jpg
--rw-r--r--   0        0        0    11646 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/insta360_date.jpg
--rw-r--r--   0        0        0    55140 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/int_long_tag.jpg
--rw-r--r--   0        0        0    39169 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/out_of_bounds_lat.jpg
--rw-r--r--   0        0        0    39169 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/out_of_bounds_lon.jpg
--rw-r--r--   0        0        0     9665 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/pic_with_float_lat.jpg
--rw-r--r--   0        0        0     3130 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/fixtures/ricoh_theta_no_projection.jpg
--rw-r--r--   0        0        0      612 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.0/tests/test_main.py
--rw-r--r--   0        0        0    22277 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.0/tests/test_reader.py
--rw-r--r--   0        0        0    11365 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.0/tests/test_writer.py
--rw-r--r--   0        0        0     6303 1970-01-01 00:00:00.000000 geopic_tag_reader-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1009 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0       91 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6887 2024-04-26 12:19:17.765989 geopic_tag_reader-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/LICENSE
+-rw-r--r--   0        0        0      676 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/Makefile
+-rw-r--r--   0        0        0     5243 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/README.md
+-rw-r--r--   0        0        0       65 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/docs/.pages
+-rw-r--r--   0        0        0     3393 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.1/docs/API_USAGE.md
+-rw-r--r--   0        0        0     1835 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/docs/CLI_USAGE.md
+-rw-r--r--   0        0        0      999 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/docs/Develop.md
+-rw-r--r--   0        0        0     2015 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/docs/Install.md
+-rw-r--r--   0        0        0     1066 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/docs/camera.md
+-rw-r--r--   0        0        0      529 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.1/docs/model.md
+-rw-r--r--   0        0        0     9338 2024-04-26 12:19:17.769989 geopic_tag_reader-1.1.1/docs/reader.md
+-rw-r--r--   0        0        0     4301 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/docs/writer.md
+-rw-r--r--   0        0        0       47 2024-04-26 12:19:17.769989 geopic_tag_reader-1.1.1/geopic_tag_reader/__init__.py
+-rw-r--r--   0        0        0     1643 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/geopic_tag_reader/camera.py
+-rw-r--r--   0        0        0     3219 2024-04-24 07:53:47.595124 geopic_tag_reader-1.1.1/geopic_tag_reader/main.py
+-rw-r--r--   0        0        0      129 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/geopic_tag_reader/model.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/geopic_tag_reader/py.typed
+-rw-r--r--   0        0        0    24543 2024-04-24 08:57:35.438995 geopic_tag_reader-1.1.1/geopic_tag_reader/reader.py
+-rw-r--r--   0        0        0     8672 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.1/geopic_tag_reader/writer.py
+-rw-r--r--   0        0        0     1142 2024-04-15 10:48:00.708002 geopic_tag_reader-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/pytest.ini
+-rw-r--r--   0        0        0        0 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0    79729 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/tests/fixtures/1.jpg
+-rw-r--r--   0        0        0    24664 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/tests/fixtures/IMG_20210720_144918.jpg
+-rw-r--r--   0        0        0    38766 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/tests/fixtures/IMG_20210720_161352.jpg
+-rw-r--r--   0        0        0    75709 2024-04-12 10:18:21.653502 geopic_tag_reader-1.1.1/tests/fixtures/a1.jpg
+-rw-r--r--   0        0        0    29130 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/b1.jpg
+-rw-r--r--   0        0        0    39810 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/broken_makernotes.jpg
+-rw-r--r--   0        0        0    69903 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/c1.jpg
+-rw-r--r--   0        0        0     4867 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/charset.jpg
+-rw-r--r--   0        0        0    30503 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/cropped.jpg
+-rw-r--r--   0        0        0    33446 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/d1.jpg
+-rw-r--r--   0        0        0     5415 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/datetime_ms_float.jpg
+-rw-r--r--   0        0        0    35109 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/datetime_offset.jpg
+-rw-r--r--   0        0        0    51474 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0    29141 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/flat.jpg
+-rw-r--r--   0        0        0    70264 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/gopromax_flat.jpg
+-rw-r--r--   0        0        0     4174 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/gps_date_slash.jpg
+-rw-r--r--   0        0        0     5237 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/gps_date_time_stamp.jpg
+-rw-r--r--   0        0        0    66264 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/img_Ricoh_Theta.jpg
+-rw-r--r--   0        0        0     5360 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/img_V4MPack.jpg
+-rw-r--r--   0        0        0    66961 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/img_categorisee.jpg
+-rw-r--r--   0        0        0   135574 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/img_datetimeoriginal.jpg
+-rw-r--r--   0        0        0    29503 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/img_gps_date_string.jpg
+-rw-r--r--   0        0        0    35282 2024-04-12 10:18:21.657502 geopic_tag_reader-1.1.1/tests/fixtures/img_gps_datestamp.jpg
+-rw-r--r--   0        0        0    43696 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/img_gps_sotm.jpg
+-rw-r--r--   0        0        0    33170 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/img_invalid_gps_date.jpg
+-rw-r--r--   0        0        0    34454 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/img_without_coord.jpg
+-rw-r--r--   0        0        0    34518 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/img_without_dt.jpg
+-rw-r--r--   0        0        0    12643 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/img_without_exif_tags.jpg
+-rw-r--r--   0        0        0    11646 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/insta360_date.jpg
+-rw-r--r--   0        0        0    55140 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/int_long_tag.jpg
+-rw-r--r--   0        0        0    39169 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/out_of_bounds_lat.jpg
+-rw-r--r--   0        0        0    39169 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/out_of_bounds_lon.jpg
+-rw-r--r--   0        0        0     9665 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/pic_with_float_lat.jpg
+-rw-r--r--   0        0        0     3130 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/fixtures/ricoh_theta_no_projection.jpg
+-rw-r--r--   0        0        0      612 2024-04-12 10:18:21.661502 geopic_tag_reader-1.1.1/tests/test_main.py
+-rw-r--r--   0        0        0    22571 2024-04-24 07:53:47.595124 geopic_tag_reader-1.1.1/tests/test_reader.py
+-rw-r--r--   0        0        0    11365 2024-04-16 10:04:34.508732 geopic_tag_reader-1.1.1/tests/test_writer.py
+-rw-r--r--   0        0        0     6303 1970-01-01 00:00:00.000000 geopic_tag_reader-1.1.1/PKG-INFO
```

### Comparing `geopic_tag_reader-1.1.0/.gitlab-ci.yml` & `geopic_tag_reader-1.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/CHANGELOG.md` & `geopic_tag_reader-1.1.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.1.1] - 2024-04-26
+
+### Added
+
+- Reader now handles pitch & roll values from various EXIF/XMP tags.
+
 ## [1.1.0] - 2024-04-17
 
 ### Changed
 
 - Encoding information (`charset=...`) is now stripped out of text EXIF tags.
 - `GeoPicTags` objects returns `ts` as a Python `datetime` object (instead of decimal epoch).
 - Improved timezone handling in reader, GPS coordinates are used to find appropriate timezone when no timezone is defined in EXIF tags. If a UTC fallback is done, a warning is thrown.
@@ -156,15 +162,16 @@
 
 ## [0.0.1] - 2023-03-31
 
 ### Added
 
 - EXIF tag reading methods extracted from [GeoVisio API](https://gitlab.com/geovisio/api)
 
-[Unreleased]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.1.0...main
+[Unreleased]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.1.1...main
+[1.1.1]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.1.0...1.1.1
 [1.1.0]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.6...1.1.0
 [1.0.6]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.5...1.0.6
 [1.0.5]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.4...1.0.5
 [1.0.4]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.3...1.0.4
 [1.0.3]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.2...1.0.3
 [1.0.2]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.1...1.0.2
 [1.0.1]: https://gitlab.com/geovisio/geo-picture-tag-reader/-/compare/1.0.0...1.0.1
```

### Comparing `geopic_tag_reader-1.1.0/CODE_OF_CONDUCT.md` & `geopic_tag_reader-1.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/LICENSE` & `geopic_tag_reader-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/Makefile` & `geopic_tag_reader-1.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/README.md` & `geopic_tag_reader-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/docs/API_USAGE.md` & `geopic_tag_reader-1.1.1/docs/API_USAGE.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/docs/CLI_USAGE.md` & `geopic_tag_reader-1.1.1/docs/CLI_USAGE.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/docs/Develop.md` & `geopic_tag_reader-1.1.1/docs/Develop.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/docs/Install.md` & `geopic_tag_reader-1.1.1/docs/Install.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/docs/camera.md` & `geopic_tag_reader-1.1.1/docs/camera.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/docs/model.md` & `geopic_tag_reader-1.1.1/docs/model.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/docs/reader.md` & `geopic_tag_reader-1.1.1/docs/reader.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L118"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L124"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `readPictureMetadata`
 
 ```python
 readPictureMetadata(picture: bytes) → GeoPicTags
 ```
 
@@ -31,56 +31,56 @@
 **Returns:**
  
  - <b>`GeoPicTags`</b>:  Extracted metadata from picture 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L355"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L394"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeMakeModel`
 
 ```python
 decodeMakeModel(value) → str
 ```
 
 Python 2/3 compatible decoding of make/model field. 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L366"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L405"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `isValidManyFractions`
 
 ```python
 isValidManyFractions(value: str) → bool
 ```
 
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L373"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L412"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeManyFractions`
 
 ```python
 decodeManyFractions(value: str) → List[Fraction]
 ```
 
 Try to decode a list of fractions, separated by spaces 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L386"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L425"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeLatLon`
 
 ```python
 decodeLatLon(
     data: dict,
     group: str
@@ -88,15 +88,15 @@
 ```
 
 Reads GPS info from given group to get latitude/longitude as float coordinates 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L441"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L480"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeDateTimeOriginal`
 
 ```python
 decodeDateTimeOriginal(
     data: dict,
     datetimeField: str,
@@ -108,30 +108,30 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L495"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L534"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeTimeOffset`
 
 ```python
 decodeTimeOffset(data: dict, offsetTimeField: str) → Optional[tzinfo]
 ```
 
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L501"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L540"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeGPSDateTime`
 
 ```python
 decodeGPSDateTime(
     data: dict,
     group: str,
@@ -143,15 +143,15 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L552"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L591"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `decodeSecondsAndMicroSeconds`
 
 ```python
 decodeSecondsAndMicroSeconds(
     secondsRaw: str,
     microsecondsRaw: str
@@ -161,15 +161,15 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L578"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L617"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `isExifTagUsable`
 
 ```python
 isExifTagUsable(exif, tag, expectedType: Any = <class 'str'>) → bool
 ```
 
@@ -241,23 +241,25 @@
 
 
 **Attributes:**
  
  - <b>`lat`</b> (float):  GPS Latitude (in WGS84) 
  - <b>`lon`</b> (float):  GPS Longitude (in WGS84) 
  - <b>`ts`</b> (datetime):  The capture date (date & time with timezone) 
- - <b>`heading`</b> (int):  Picture heading (in degrees, North = 0°, East = 90°, South = 180°, West = 270°) 
+ - <b>`heading`</b> (int):  Picture heading/yaw (in degrees, North = 0°, East = 90°, South = 180°, West = 270°) 
  - <b>`type`</b> (str):  The kind of picture (flat, equirectangular) 
  - <b>`make`</b> (str):  The camera manufacturer name 
  - <b>`model`</b> (str):  The camera model name 
  - <b>`focal_length`</b> (float):  The camera focal length (in mm) 
  - <b>`crop`</b> (CropValues):  The picture cropped area metadata (optional) 
  - <b>`exif`</b> (dict[str, str]):  Raw EXIF tags from picture (following Exiv2 naming scheme, see https://exiv2.org/metadata.html) 
  - <b>`tagreader_warnings`</b> (list[str]):  List of thrown warnings during metadata reading 
  - <b>`altitude`</b> (float):  altitude (in m) (optional) 
+ - <b>`pitch`</b> (float):  Picture pitch angle, compared to horizon (in degrees, bottom = -90°, horizon = 0°, top = 90°) 
+ - <b>`roll`</b> (float):  Picture roll angle, on a right/left axis (in degrees, left-arm down = -90°, flat = 0°, right-arm down = 90°) 
 
 
 
 Implementation note: this needs to be sync with the PartialGeoPicTags structure 
 
 <a href="../<string>"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
@@ -272,34 +274,36 @@
     type: str,
     make: Optional[str],
     model: Optional[str],
     focal_length: Optional[float],
     crop: Optional[CropValues],
     exif: Dict[str, str] = <factory>,
     tagreader_warnings: List[str] = <factory>,
-    altitude: Optional[float] = None
+    altitude: Optional[float] = None,
+    pitch: Optional[float] = None,
+    roll: Optional[float] = None
 ) → None
 ```
 
 
 
 
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L77"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L81"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `InvalidExifException`
 Exception for invalid EXIF information from image 
 
-<a href="../geopic_tag_reader/reader.py#L80"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L84"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `__init__`
 
 ```python
 __init__(msg)
 ```
 
@@ -309,15 +313,15 @@
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L84"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L88"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PartialGeoPicTags`
 Tags associated to a geolocated picture when not all tags have been found 
 
 Implementation note: this needs to be sync with the GeoPicTags structure 
 
 <a href="../<string>"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
@@ -333,36 +337,38 @@
     type: Optional[str] = None,
     make: Optional[str] = None,
     model: Optional[str] = None,
     focal_length: Optional[float] = None,
     crop: Optional[CropValues] = None,
     exif: Dict[str, str] = <factory>,
     tagreader_warnings: List[str] = <factory>,
-    altitude: Optional[float] = None
+    altitude: Optional[float] = None,
+    pitch: Optional[float] = None,
+    roll: Optional[float] = None
 ) → None
 ```
 
 
 
 
 
 
 
 
 
 ---
 
-<a href="../geopic_tag_reader/reader.py#L105"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L111"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PartialExifException`
 Exception for partial / missing EXIF information from image 
 
 Contains a PartialGeoPicTags with all tags that have been read and the list of missing tags 
 
-<a href="../geopic_tag_reader/reader.py#L112"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../geopic_tag_reader/reader.py#L118"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `__init__`
 
 ```python
 __init__(msg, missing_mandatory_tags: Set[str], partial_tags: PartialGeoPicTags)
 ```
```

#### html2text {}

```diff
@@ -40,42 +40,47 @@
 Cropped area top offset _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
 _c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `__init__` ```python __init__( fullWidth:
 int, fullHeight: int, width: int, height: int, left: int, top: int ) â None
 ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
 `GeoPicTags` Tags associated to a geolocated picture **Attributes:** - ``llaatt``
 (float): GPS Latitude (in WGS84) - ``lloonn`` (float): GPS Longitude (in WGS84) -
 ``ttss`` (datetime): The capture date (date & time with timezone) - ``hheeaaddiinngg``
-(int): Picture heading (in degrees, North = 0Â°, East = 90Â°, South = 180Â°,
-West = 270Â°) - ``ttyyppee`` (str): The kind of picture (flat, equirectangular) -
-``mmaakkee`` (str): The camera manufacturer name - ``mmooddeell`` (str): The camera model
-name - ``ffooccaall__lleennggtthh`` (float): The camera focal length (in mm) - ``ccrroopp``
-(CropValues): The picture cropped area metadata (optional) - ``eexxiiff`` (dict[str,
-str]): Raw EXIF tags from picture (following Exiv2 naming scheme, see https://
-exiv2.org/metadata.html) - ``ttaaggrreeaaddeerr__wwaarrnniinnggss`` (list[str]): List of thrown
-warnings during metadata reading - ``aallttiittuuddee`` (float): altitude (in m)
-(optional) Implementation note: this needs to be sync with the
+(int): Picture heading/yaw (in degrees, North = 0Â°, East = 90Â°, South =
+180Â°, West = 270Â°) - ``ttyyppee`` (str): The kind of picture (flat,
+equirectangular) - ``mmaakkee`` (str): The camera manufacturer name - ``mmooddeell`` (str):
+The camera model name - ``ffooccaall__lleennggtthh`` (float): The camera focal length (in mm)
+- ``ccrroopp`` (CropValues): The picture cropped area metadata (optional) - ``eexxiiff``
+(dict[str, str]): Raw EXIF tags from picture (following Exiv2 naming scheme,
+see https://exiv2.org/metadata.html) - ``ttaaggrreeaaddeerr__wwaarrnniinnggss`` (list[str]): List
+of thrown warnings during metadata reading - ``aallttiittuuddee`` (float): altitude (in
+m) (optional) - ``ppiittcchh`` (float): Picture pitch angle, compared to horizon (in
+degrees, bottom = -90Â°, horizon = 0Â°, top = 90Â°) - ``rroollll`` (float): Picture
+roll angle, on a right/left axis (in degrees, left-arm down = -90Â°, flat =
+0Â°, right-arm down = 90Â°) Implementation note: this needs to be sync with the
 PartialGeoPicTags structure _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
 _c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `__init__` ```python __init__( lat: float,
 lon: float, ts: datetime, heading: Optional[int], type: str, make: Optional
 [str], model: Optional[str], focal_length: Optional[float], crop: Optional
 [CropValues], exif: Dict[str, str] = , tagreader_warnings: List[str] = ,
-altitude: Optional[float] = None ) â None ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `InvalidExifException`
-Exception for invalid EXIF information from image _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+altitude: Optional[float] = None, pitch: Optional[float] = None, roll: Optional
+[float] = None ) â None ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `InvalidExifException` Exception for invalid
+EXIF information from image _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `__init__` ```python __init__(msg) ``` ---
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
+`PartialGeoPicTags` Tags associated to a geolocated picture when not all tags
+have been found Implementation note: this needs to be sync with the GeoPicTags
+structure _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
+method `__init__` ```python __init__( lat: Optional[float] = None, lon:
+Optional[float] = None, ts: Optional[datetime] = None, heading: Optional[int] =
+None, type: Optional[str] = None, make: Optional[str] = None, model: Optional
+[str] = None, focal_length: Optional[float] = None, crop: Optional[CropValues]
+= None, exif: Dict[str, str] = , tagreader_warnings: List[str] = , altitude:
+Optional[float] = None, pitch: Optional[float] = None, roll: Optional[float] =
+None ) â None ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `PartialExifException` Exception for partial
+/ missing EXIF information from image Contains a PartialGeoPicTags with all
+tags that have been read and the list of missing tags _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `__init__` ```python __init__
-(msg) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]##
-class `PartialGeoPicTags` Tags associated to a geolocated picture when not all
-tags have been found Implementation note: this needs to be sync with the
-GeoPicTags structure _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]### method `__init__` ```python __init__( lat: Optional[float] = None,
-lon: Optional[float] = None, ts: Optional[datetime] = None, heading: Optional
-[int] = None, type: Optional[str] = None, make: Optional[str] = None, model:
-Optional[str] = None, focal_length: Optional[float] = None, crop: Optional
-[CropValues] = None, exif: Dict[str, str] = , tagreader_warnings: List[str] = ,
-altitude: Optional[float] = None ) â None ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `PartialExifException`
-Exception for partial / missing EXIF information from image Contains a
-PartialGeoPicTags with all tags that have been read and the list of missing
-tags _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`__init__` ```python __init__(msg, missing_mandatory_tags: Set[str],
-partial_tags: PartialGeoPicTags) ``` --- _This file was automatically generated
-via [lazydocs](https://github.com/ml-tooling/lazydocs)._
+(msg, missing_mandatory_tags: Set[str], partial_tags: PartialGeoPicTags) ``` --
+- _This file was automatically generated via [lazydocs](https://github.com/ml-
+tooling/lazydocs)._
```

### Comparing `geopic_tag_reader-1.1.0/docs/writer.md` & `geopic_tag_reader-1.1.1/docs/writer.md`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/geopic_tag_reader/camera.py` & `geopic_tag_reader-1.1.1/geopic_tag_reader/camera.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/geopic_tag_reader/main.py` & `geopic_tag_reader-1.1.1/geopic_tag_reader/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         print("Timestamp:", metadata.ts.isoformat())
         print("Heading:", metadata.heading)
         print("Type:", metadata.type)
         print("Make:", metadata.make)
         print("Model:", metadata.model)
         print("Focal length:", metadata.focal_length)
         print("Crop parameters:", metadata.crop)
+        print("Pitch:", metadata.pitch)
+        print("Roll:", metadata.roll)
 
         if len(metadata.tagreader_warnings) > 0:
             print("Warnings raised by reader:")
             for w in metadata.tagreader_warnings:
                 print(" - " + w)
```

### Comparing `geopic_tag_reader-1.1.0/geopic_tag_reader/reader.py` & `geopic_tag_reader-1.1.1/geopic_tag_reader/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,23 +42,25 @@
 class GeoPicTags:
     """Tags associated to a geolocated picture
 
     Attributes:
         lat (float): GPS Latitude (in WGS84)
         lon (float): GPS Longitude (in WGS84)
         ts (datetime): The capture date (date & time with timezone)
-        heading (int): Picture heading (in degrees, North = 0°, East = 90°, South = 180°, West = 270°)
+        heading (int): Picture heading/yaw (in degrees, North = 0°, East = 90°, South = 180°, West = 270°)
         type (str): The kind of picture (flat, equirectangular)
         make (str): The camera manufacturer name
         model (str): The camera model name
         focal_length (float): The camera focal length (in mm)
         crop (CropValues): The picture cropped area metadata (optional)
         exif (dict[str, str]): Raw EXIF tags from picture (following Exiv2 naming scheme, see https://exiv2.org/metadata.html)
         tagreader_warnings (list[str]): List of thrown warnings during metadata reading
         altitude (float): altitude (in m) (optional)
+        pitch (float): Picture pitch angle, compared to horizon (in degrees, bottom = -90°, horizon = 0°, top = 90°)
+        roll (float): Picture roll angle, on a right/left axis (in degrees, left-arm down = -90°, flat = 0°, right-arm down = 90°)
 
 
     Implementation note: this needs to be sync with the PartialGeoPicTags structure
     """
 
     lat: float
     lon: float
@@ -68,14 +70,16 @@
     make: Optional[str]
     model: Optional[str]
     focal_length: Optional[float]
     crop: Optional[CropValues]
     exif: Dict[str, str] = field(default_factory=lambda: {})
     tagreader_warnings: List[str] = field(default_factory=lambda: [])
     altitude: Optional[float] = None
+    pitch: Optional[float] = None
+    roll: Optional[float] = None
 
 
 class InvalidExifException(Exception):
     """Exception for invalid EXIF information from image"""
 
     def __init__(self, msg):
         super().__init__(msg)
@@ -96,14 +100,16 @@
     make: Optional[str] = None
     model: Optional[str] = None
     focal_length: Optional[float] = None
     crop: Optional[CropValues] = None
     exif: Dict[str, str] = field(default_factory=lambda: {})
     tagreader_warnings: List[str] = field(default_factory=lambda: [])
     altitude: Optional[float] = None
+    pitch: Optional[float] = None
+    roll: Optional[float] = None
 
 
 class PartialExifException(Exception):
     """
     Exception for partial / missing EXIF information from image
 
     Contains a PartialGeoPicTags with all tags that have been read and the list of missing tags
@@ -209,15 +215,15 @@
                 milliseconds * 1000,
                 tzinfo=datetime.timezone.utc,
             )
 
         except Exception as e:
             warnings.append("Skipping Mapillary date/time as it was not recognized:\n\t" + str(e))
 
-    # Heading
+    # Heading/Yaw
     heading = None
     if isExifTagUsable(data, "Xmp.GPano.PoseHeadingDegrees", float) and isExifTagUsable(data, "Exif.GPSInfo.GPSImgDirection", Fraction):
         gpsDir = int(round(float(Fraction(data["Exif.GPSInfo.GPSImgDirection"]))))
         gpanoHeading = int(round(float(data["Xmp.GPano.PoseHeadingDegrees"])))
         if gpsDir > 0 and gpanoHeading == 0:
             heading = gpsDir
         elif gpsDir == 0 and gpanoHeading > 0:
@@ -232,14 +238,43 @@
 
     elif isExifTagUsable(data, "Exif.GPSInfo.GPSImgDirection", Fraction):
         heading = int(round(float(Fraction(data["Exif.GPSInfo.GPSImgDirection"]))))
 
     elif "MAPCompassHeading" in data and isExifTagUsable(data["MAPCompassHeading"], "TrueHeading", float):
         heading = int(round(float(data["MAPCompassHeading"]["TrueHeading"])))
 
+    # Pitch & roll
+    pitch = None
+    roll = None
+    exifPRFields = ["Xmp.Camera.$$", "Exif.GPSInfo.GPS$$", "Xmp.GPano.Pose$$Degrees", "Xmp.GPano.InitialView$$Degrees"]
+    # For each potential EXIF field
+    for exifField in exifPRFields:
+        # Try out both Pitch & Roll variants
+        for checkField in ["Pitch", "Roll"]:
+            exifCheckField = exifField.replace("$$", checkField)
+            foundValue = None
+            # Look for float or fraction
+            if isExifTagUsable(data, exifCheckField, float):
+                foundValue = float(data[exifCheckField])
+            elif isExifTagUsable(data, exifCheckField, Fraction):
+                foundValue = float(Fraction(data[exifCheckField]))
+
+            # Save to correct variable (if not already set)
+            if foundValue is not None:
+                if checkField == "Pitch":
+                    if pitch is None:
+                        pitch = foundValue
+                    else:
+                        continue
+                elif checkField == "Roll":
+                    if roll is None:
+                        roll = foundValue
+                    else:
+                        continue
+
     # Make and model
     make = data.get("Exif.Image.Make") or data.get("MAPDeviceMake")
     model = data.get("Exif.Image.Model") or data.get("MAPDeviceModel")
 
     if make is not None:
         make = decodeMakeModel(make).strip()
 
@@ -328,14 +363,16 @@
                 make,
                 model,
                 focalLength,
                 crop,
                 exif=data,
                 tagreader_warnings=warnings,
                 altitude=altitude,
+                pitch=pitch,
+                roll=roll,
             ),
         )
 
     assert lon and lat and d  # at this point all those fields cannot be null
     return GeoPicTags(
         lat,
         lon,
@@ -345,14 +382,16 @@
         make,
         model,
         focalLength,
         crop,
         exif=data,
         tagreader_warnings=warnings,
         altitude=altitude,
+        pitch=pitch,
+        roll=roll,
     )
 
 
 def decodeMakeModel(value) -> str:
     """Python 2/3 compatible decoding of make/model field."""
     if hasattr(value, "decode"):
         try:
```

### Comparing `geopic_tag_reader-1.1.0/geopic_tag_reader/writer.py` & `geopic_tag_reader-1.1.1/geopic_tag_reader/writer.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/pyproject.toml` & `geopic_tag_reader-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/1.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/IMG_20210720_144918.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/IMG_20210720_144918.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/IMG_20210720_161352.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/IMG_20210720_161352.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/a1.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/a1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/b1.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/b1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/broken_makernotes.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/broken_makernotes.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/c1.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/c1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/charset.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/charset.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/cropped.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/cropped.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/d1.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/d1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/datetime_ms_float.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/datetime_ms_float.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/datetime_offset.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/datetime_offset.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/e1.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/flat.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/flat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/gopromax_flat.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/gopromax_flat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/gps_date_slash.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/gps_date_slash.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/gps_date_time_stamp.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/gps_date_time_stamp.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_Ricoh_Theta.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_Ricoh_Theta.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_V4MPack.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_V4MPack.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_categorisee.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_categorisee.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_datetimeoriginal.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_datetimeoriginal.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_gps_date_string.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_gps_date_string.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_gps_datestamp.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_gps_datestamp.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_gps_sotm.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_gps_sotm.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_invalid_gps_date.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_invalid_gps_date.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_without_coord.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_without_coord.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_without_dt.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_without_dt.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/img_without_exif_tags.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/img_without_exif_tags.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/insta360_date.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/insta360_date.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/int_long_tag.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/int_long_tag.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/out_of_bounds_lat.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/out_of_bounds_lat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/out_of_bounds_lon.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/out_of_bounds_lon.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/pic_with_float_lat.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/pic_with_float_lat.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/fixtures/ricoh_theta_no_projection.jpg` & `geopic_tag_reader-1.1.1/tests/fixtures/ricoh_theta_no_projection.jpg`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/test_main.py` & `geopic_tag_reader-1.1.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/tests/test_reader.py` & `geopic_tag_reader-1.1.1/tests/test_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     assert gpt.lon == expectedDict.get("lon")
     assert gpt.heading == expectedDict.get("heading")
     assert gpt.type == expectedDict.get("type")
     assert gpt.make == expectedDict.get("make")
     assert gpt.model == expectedDict.get("model")
     assert gpt.focal_length == expectedDict.get("focal_length")
     assert gpt.altitude == expectedDict.get("altitude")
+    assert gpt.pitch == expectedDict.get("pitch")
+    assert gpt.roll == expectedDict.get("roll")
     assert gpt.tagreader_warnings == expectedDict.get("tagreader_warnings", [])
     assert len(gpt.exif) > 0
 
     if expectedDict.get("ts") is not None:
         assert gpt.ts is not None
         assert gpt.ts.isoformat() == expectedDict["ts"]
     else:
@@ -45,14 +47,16 @@
             "ts": "2021-07-29T11:16:54+02:00",
             "heading": 349,
             "type": "equirectangular",
             "make": "GoPro",
             "model": "Max",
             "focal_length": 3,
             "altitude": 93,
+            "roll": 0,
+            "pitch": 0,
         },
     )
 
 
 @pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "a1.jpg"))
 def test_readPictureMetadata_negCoords(datafiles):
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/a1.jpg"))
@@ -64,14 +68,16 @@
             "ts": "2022-05-13T16:53:00+02:00",
             "heading": 32,
             "type": "equirectangular",
             "make": "GoPro",
             "model": "Max",
             "focal_length": 3,
             "altitude": 79,
+            "roll": 0,
+            "pitch": 0,
         },
     )
 
 
 @pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "b1.jpg"))
 def test_readPictureMetadata_flat(datafiles):
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/b1.jpg"))
@@ -157,14 +163,16 @@
                 "heading": 270,
                 "lat": 48.83930905577957,
                 "lon": 2.3205357914890987,
                 "make": "RICOH",
                 "model": "THETA m15",
                 "ts": "2016-03-25T14:12:13+01:00",
                 "type": "equirectangular",
+                "roll": 3,
+                "pitch": 1,
             },
         )
 
 
 @pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "img_V4MPack.jpg"))
 def test_readPictureMetadata_v4mpack(datafiles):
     for f in datafiles.iterdir():
@@ -598,14 +606,16 @@
             "ts": "2022-05-13T16:54:11+02:00",
             "heading": 32,
             "type": "equirectangular",
             "make": "GoPro",
             "model": "Max",
             "focal_length": 3,
             "altitude": 79,
+            "roll": 0,
+            "pitch": 0,
         },
     )
 
 
 @pytest.mark.datafiles(os.path.join(FIXTURE_DIR, "gps_date_slash.jpg"))
 def test_readPictureMetadata_gps_date_slash(datafiles):
     result = reader.readPictureMetadata(openImg(str(datafiles) + "/gps_date_slash.jpg"))
```

### Comparing `geopic_tag_reader-1.1.0/tests/test_writer.py` & `geopic_tag_reader-1.1.1/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `geopic_tag_reader-1.1.0/PKG-INFO` & `geopic_tag_reader-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopic-tag-reader
-Version: 1.1.0
+Version: 1.1.1
 Summary: GeoPicTagReader
 Author-email: Adrien PAVIE <panieravide@riseup.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: typer ~= 0.12
 Requires-Dist: xmltodict ~= 0.13
```

