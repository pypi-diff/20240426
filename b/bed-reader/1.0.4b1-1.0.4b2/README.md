# Comparing `tmp/bed_reader-1.0.4b1.tar.gz` & `tmp/bed_reader-1.0.4b2.tar.gz`

## Comparing `bed_reader-1.0.4b1.tar` & `bed_reader-1.0.4b2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 bed_reader-1.0.4b1/Cargo.toml
--rw-r--r--   0     1001      127       58 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/.flake8
--rw-r--r--   0     1001      127     4952 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/.github/workflows/ci.yml
--rw-r--r--   0     1001      127     2222 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/.gitignore
--rw-r--r--   0     1001      127      186 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/.isort.cfg
--rw-r--r--   0     1001      127       27 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/AUTHORS.txt
--rw-r--r--   0     1001      127     1251 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/CHANGELOG.md
--rw-r--r--   0     1001      127    62584 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/Cargo.lock
--rw-r--r--   0     1001      127    11352 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/LICENSE.md
--rw-r--r--   0     1001      127     6031 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/README-rust.md
--rw-r--r--   0     1001      127     3475 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/README.md
--rw-r--r--   0     1001      127     4412 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0     1001      127    15715 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/_static/basic.css
--rw-r--r--   0     1001      127     4472 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/_static/doctools.js
--rw-r--r--   0     1001      127      440 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/_static/documentation_options.js
--rw-r--r--   0     1001      127      286 2024-04-24 16:28:53.000000 bed_reader-1.0.4b1/_static/file.png
--rw-r--r--   0     1001      127   290962 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/jquery-3.4.1.js
--rw-r--r--   0     1001      127   287630 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/jquery-3.5.1.js
--rw-r--r--   0     1001      127   288580 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/jquery-3.6.0.js
--rw-r--r--   0     1001      127    89501 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/jquery.js
--rw-r--r--   0     1001      127      934 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/js/badge_only.js
--rw-r--r--   0     1001      127     4370 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0     1001      127     2734 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/js/html5shiv.min.js
--rw-r--r--   0     1001      127    15418 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/js/modernizr.min.js
--rw-r--r--   0     1001      127     5023 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/js/theme.js
--rw-r--r--   0     1001      127     4957 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/language_data.js
--rw-r--r--   0     1001      127       90 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/minus.png
--rw-r--r--   0     1001      127       90 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/plus.png
--rw-r--r--   0     1001      127     4892 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/pygments.css
--rw-r--r--   0     1001      127    18215 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/searchtools.js
--rw-r--r--   0     1001      127     4712 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/sphinx_highlight.js
--rw-r--r--   0     1001      127    69719 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/underscore-1.12.0.js
--rw-r--r--   0     1001      127    68420 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/underscore-1.13.1.js
--rw-r--r--   0     1001      127    35168 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/underscore-1.3.1.js
--rw-r--r--   0     1001      127    19530 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/_static/underscore.js
--rw-r--r--   0     1001      127      901 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/__init__.py
--rw-r--r--   0     1001      127    63647 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/_open_bed.py
--rw-r--r--   0     1001      127     3976 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/_sample_data.py
--rw-r--r--   0     1001      127    22133 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/_to_bed.py
--rw-r--r--   0     1001      127       50 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/__init__.py
--rw-r--r--   0     1001      127     8332 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/benchmark/bench2.ipynb
--rw-r--r--   0     1001      127     3719 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/benchmark/benchmark.py
--rw-r--r--   0     1001      127     3388 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/registry.txt
--rw-r--r--   0     1001      127    11008 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/test_file_dot.py
--rw-r--r--   0     1001      127    57134 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/test_open_bed.py
--rw-r--r--   0     1001      127    46079 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/test_open_bed_cloud.py
--rw-r--r--   0     1001      127      707 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/test_opt_dep.py
--rw-r--r--   0     1001      127      135 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/build.rs
--rw-r--r--   0     1001      127     1316 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/examples/cloud.rs
--rw-r--r--   0     1001      127      853 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/examples/no_cloud.rs
--rw-r--r--   0     1001      127      124 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/pytest.ini
--rw-r--r--   0     1001      127      235 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/requirements-dev.txt
--rw-r--r--   0     1001      127       35 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/requirements-min-dev.txt
--rw-r--r--   0     1001      127       38 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/requirements.txt
--rw-r--r--   0     1001      127       46 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/setpath.bat
--rw-r--r--   0     1001      127   101801 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/src/bed_cloud.rs
--rw-r--r--   0     1001      127   264109 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/src/lib.rs
--rw-r--r--   0     1001      127    22631 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/src/python_module.rs
--rw-r--r--   0     1001      127     8507 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/src/supplemental_documents/cloud_urls_etc.md
--rw-r--r--   0     1001      127     4958 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/src/supplemental_documents/options_etc.md
--rw-r--r--   0     1001      127    36712 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/src/tests.rs
--rw-r--r--   0     1001      127    73879 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/tests/tests_api.rs
--rw-r--r--   0     1001      127    81719 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/tests/tests_api_cloud.rs
--rw-r--r--   0     1001      127     1715 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/useful.md
--rw-r--r--   0     1001      127      930 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/pyproject.toml
--rw-r--r--   0     1001      127        7 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/smallmodebad.bed
--rw-r--r--   0     1001      127     2503 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/some_missing.bed
--rw-r--r--   0     1001      127       63 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/sparse.bed
--rw-r--r--   0     1001      127     1690 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/some_missing.fam
--rw-r--r--   0     1001      127    14361 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/toydata.5chrom.fam
--rw-r--r--   0     1001      127       87 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small.bim
--rw-r--r--   0     1001      127       96 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small2_array.memmap
--rw-r--r--   0     1001      127      130 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.fam
--rw-r--r--   0     1001      127       48 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small_array.memmap
--rw-r--r--   0     1001      127       85 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small.fam
--rw-r--r--   0     1001      127        7 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small_no_bim.bed
--rw-r--r--   0     1001      127       80 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small.bad_bim
--rw-r--r--   0     1001      127        6 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small_too_short.bed
--rw-r--r--   0     1001      127        7 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/smallmode0.bed
--rw-r--r--   0     1001      127        7 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small.bed
--rw-r--r--   0     1001      127  1250003 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/toydata.5chrom.bed
--rw-r--r--   0     1001      127      303 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bed
--rw-r--r--   0     1001      127       68 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small.mib
--rw-r--r--   0     1001      127     2184 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bim
--rw-r--r--   0     1001      127      557 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/sparse.bim
--rw-r--r--   0     1001      127    80128 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/some_missing.val.npy
--rw-r--r--   0     1001      127       30 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/badfile.bed
--rw-r--r--   0     1001      127       87 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small_too_short.bim
--rw-r--r--   0     1001      127      114 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/smallmode0.fam
--rw-r--r--   0     1001      127   227784 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/toydata.5chrom.bim
--rw-r--r--   0     1001      127        0 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/empty.bed
--rw-r--r--   0     1001      127  1600640 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/500x400_o640_array.memmap
--rw-r--r--   0     1001      127       85 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small_too_short.fam
--rw-r--r--   0     1001      127     2588 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/some_missing.bim
--rw-r--r--   0     1001      127        7 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small_no_fam.bed
--rw-r--r--   0     1001      127       84 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small.bim_bad_positions.bim
--rw-r--r--   0     1001      127       64 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/smallmode0.bim
--rw-r--r--   0     1001      127    12160 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/some_missing.properties.npz
--rw-r--r--   0     1001      127       85 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small_no_bim.fam
--rw-r--r--   0     1001      127       87 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small_no_fam.bim
--rw-r--r--   0     1001      127       90 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small.fam_bad
--rw-r--r--   0     1001      127        7 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small.deb
--rw-r--r--   0     1001      127      160 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/sparse.fam
--rw-r--r--   0     1001      127       45 2024-04-24 16:28:54.000000 bed_reader-1.0.4b1/bed_reader/tests/data/small.maf
--rw-r--r--   0        0        0     4700 1970-01-01 00:00:00.000000 bed_reader-1.0.4b1/PKG-INFO
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 bed_reader-1.0.4b2/Cargo.toml
+-rw-r--r--   0     1001      127       58 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/.flake8
+-rw-r--r--   0     1001      127     4952 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     2222 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/.gitignore
+-rw-r--r--   0     1001      127      186 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/.isort.cfg
+-rw-r--r--   0     1001      127       27 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/AUTHORS.txt
+-rw-r--r--   0     1001      127     1251 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/CHANGELOG.md
+-rw-r--r--   0     1001      127    62584 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/Cargo.lock
+-rw-r--r--   0     1001      127    11352 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/LICENSE.md
+-rw-r--r--   0     1001      127     6031 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/README-rust.md
+-rw-r--r--   0     1001      127     3475 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/README.md
+-rw-r--r--   0     1001      127     4412 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0     1001      127    15715 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/basic.css
+-rw-r--r--   0     1001      127     4472 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/doctools.js
+-rw-r--r--   0     1001      127      440 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/documentation_options.js
+-rw-r--r--   0     1001      127      286 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/file.png
+-rw-r--r--   0     1001      127   290962 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/jquery-3.4.1.js
+-rw-r--r--   0     1001      127   287630 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/jquery-3.5.1.js
+-rw-r--r--   0     1001      127   288580 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/jquery-3.6.0.js
+-rw-r--r--   0     1001      127    89501 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/jquery.js
+-rw-r--r--   0     1001      127      934 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/js/badge_only.js
+-rw-r--r--   0     1001      127     4370 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0     1001      127     2734 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/js/html5shiv.min.js
+-rw-r--r--   0     1001      127    15418 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/js/modernizr.min.js
+-rw-r--r--   0     1001      127     5023 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/js/theme.js
+-rw-r--r--   0     1001      127     4957 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/language_data.js
+-rw-r--r--   0     1001      127       90 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/minus.png
+-rw-r--r--   0     1001      127       90 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/plus.png
+-rw-r--r--   0     1001      127     4892 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/pygments.css
+-rw-r--r--   0     1001      127    18215 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/searchtools.js
+-rw-r--r--   0     1001      127     4712 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/sphinx_highlight.js
+-rw-r--r--   0     1001      127    69719 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/underscore-1.12.0.js
+-rw-r--r--   0     1001      127    68420 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/underscore-1.13.1.js
+-rw-r--r--   0     1001      127    35168 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/underscore-1.3.1.js
+-rw-r--r--   0     1001      127    19530 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/_static/underscore.js
+-rw-r--r--   0     1001      127      901 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/__init__.py
+-rw-r--r--   0     1001      127    64033 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/_open_bed.py
+-rw-r--r--   0     1001      127     3976 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/_sample_data.py
+-rw-r--r--   0     1001      127    22133 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/_to_bed.py
+-rw-r--r--   0     1001      127       50 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/__init__.py
+-rw-r--r--   0     1001      127     8332 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/benchmark/bench2.ipynb
+-rw-r--r--   0     1001      127     3719 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/benchmark/benchmark.py
+-rw-r--r--   0     1001      127     3388 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/registry.txt
+-rw-r--r--   0     1001      127    11008 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/test_file_dot.py
+-rw-r--r--   0     1001      127    57036 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/test_open_bed.py
+-rw-r--r--   0     1001      127    45977 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/test_open_bed_cloud.py
+-rw-r--r--   0     1001      127      707 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/test_opt_dep.py
+-rw-r--r--   0     1001      127      135 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/build.rs
+-rw-r--r--   0     1001      127     1316 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/examples/cloud.rs
+-rw-r--r--   0     1001      127      853 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/examples/no_cloud.rs
+-rw-r--r--   0     1001      127      124 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/pytest.ini
+-rw-r--r--   0     1001      127      235 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/requirements-dev.txt
+-rw-r--r--   0     1001      127       35 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/requirements-min-dev.txt
+-rw-r--r--   0     1001      127       38 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/requirements.txt
+-rw-r--r--   0     1001      127       46 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/setpath.bat
+-rw-r--r--   0     1001      127   101801 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/src/bed_cloud.rs
+-rw-r--r--   0     1001      127   264109 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/src/lib.rs
+-rw-r--r--   0     1001      127    22631 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/src/python_module.rs
+-rw-r--r--   0     1001      127     8507 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/src/supplemental_documents/cloud_urls_etc.md
+-rw-r--r--   0     1001      127     4958 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/src/supplemental_documents/options_etc.md
+-rw-r--r--   0     1001      127    36712 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/src/tests.rs
+-rw-r--r--   0     1001      127    73879 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/tests/tests_api.rs
+-rw-r--r--   0     1001      127    81719 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/tests/tests_api_cloud.rs
+-rw-r--r--   0     1001      127     1715 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/useful.md
+-rw-r--r--   0     1001      127      930 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/pyproject.toml
+-rw-r--r--   0     1001      127        7 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/smallmodebad.bed
+-rw-r--r--   0     1001      127     2503 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/some_missing.bed
+-rw-r--r--   0     1001      127       63 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/sparse.bed
+-rw-r--r--   0     1001      127     1690 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/some_missing.fam
+-rw-r--r--   0     1001      127    14361 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/toydata.5chrom.fam
+-rw-r--r--   0     1001      127       87 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small.bim
+-rw-r--r--   0     1001      127       96 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small2_array.memmap
+-rw-r--r--   0     1001      127      130 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.fam
+-rw-r--r--   0     1001      127       48 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small_array.memmap
+-rw-r--r--   0     1001      127       85 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small.fam
+-rw-r--r--   0     1001      127        7 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small_no_bim.bed
+-rw-r--r--   0     1001      127       80 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small.bad_bim
+-rw-r--r--   0     1001      127        6 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small_too_short.bed
+-rw-r--r--   0     1001      127        7 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/smallmode0.bed
+-rw-r--r--   0     1001      127        7 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small.bed
+-rw-r--r--   0     1001      127  1250003 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/toydata.5chrom.bed
+-rw-r--r--   0     1001      127      303 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bed
+-rw-r--r--   0     1001      127       68 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small.mib
+-rw-r--r--   0     1001      127     2184 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bim
+-rw-r--r--   0     1001      127      557 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/sparse.bim
+-rw-r--r--   0     1001      127    80128 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/some_missing.val.npy
+-rw-r--r--   0     1001      127       30 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/badfile.bed
+-rw-r--r--   0     1001      127       87 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small_too_short.bim
+-rw-r--r--   0     1001      127      114 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/smallmode0.fam
+-rw-r--r--   0     1001      127   227784 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/toydata.5chrom.bim
+-rw-r--r--   0     1001      127        0 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/empty.bed
+-rw-r--r--   0     1001      127  1600640 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/500x400_o640_array.memmap
+-rw-r--r--   0     1001      127       85 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small_too_short.fam
+-rw-r--r--   0     1001      127     2588 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/some_missing.bim
+-rw-r--r--   0     1001      127        7 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small_no_fam.bed
+-rw-r--r--   0     1001      127       84 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small.bim_bad_positions.bim
+-rw-r--r--   0     1001      127       64 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/smallmode0.bim
+-rw-r--r--   0     1001      127    12160 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/some_missing.properties.npz
+-rw-r--r--   0     1001      127       85 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small_no_bim.fam
+-rw-r--r--   0     1001      127       87 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small_no_fam.bim
+-rw-r--r--   0     1001      127       90 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small.fam_bad
+-rw-r--r--   0     1001      127        7 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small.deb
+-rw-r--r--   0     1001      127      160 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/sparse.fam
+-rw-r--r--   0     1001      127       45 2024-04-25 23:06:39.000000 bed_reader-1.0.4b2/bed_reader/tests/data/small.maf
+-rw-r--r--   0        0        0     4700 1970-01-01 00:00:00.000000 bed_reader-1.0.4b2/PKG-INFO
```

### Comparing `bed_reader-1.0.4b1/Cargo.toml` & `bed_reader-1.0.4b2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [package]
-version = "1.0.4-beta.1"
+version = "1.0.4-beta.2"
 name = "bed-reader"
 description = "Read and write the PLINK BED format, simply and efficiently."
 repository = "https://github.com/fastlmm/bed-reader"
 readme = "README-rust.md"
 documentation = "https://docs.rs/bed-reader/latest/bed_reader/"
 authors = ["FaST-LMM Team <fastlmm-dev@python.org>"]
 license = "Apache-2.0"  # toml-ignore
```

### Comparing `bed_reader-1.0.4b1/.github/workflows/ci.yml` & `bed_reader-1.0.4b2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/.gitignore` & `bed_reader-1.0.4b2/.gitignore`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/CHANGELOG.md` & `bed_reader-1.0.4b2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/Cargo.lock` & `bed_reader-1.0.4b2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "bed-reader"
-version = "1.0.4-beta.1"
+version = "1.0.4-beta.2"
 dependencies = [
  "anyhow",
  "anyinput",
  "bytecount",
  "byteorder",
  "bytes",
  "cloud-file",
```

### Comparing `bed_reader-1.0.4b1/LICENSE.md` & `bed_reader-1.0.4b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/README-rust.md` & `bed_reader-1.0.4b2/README-rust.md`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/README.md` & `bed_reader-1.0.4b2/README.md`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/_sphinx_javascript_frameworks_compat.js` & `bed_reader-1.0.4b2/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/basic.css` & `bed_reader-1.0.4b2/_static/basic.css`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/doctools.js` & `bed_reader-1.0.4b2/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/jquery-3.4.1.js` & `bed_reader-1.0.4b2/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/jquery-3.5.1.js` & `bed_reader-1.0.4b2/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/jquery-3.6.0.js` & `bed_reader-1.0.4b2/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/jquery.js` & `bed_reader-1.0.4b2/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/js/badge_only.js` & `bed_reader-1.0.4b2/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/js/html5shiv-printshiv.min.js` & `bed_reader-1.0.4b2/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/js/html5shiv.min.js` & `bed_reader-1.0.4b2/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/js/modernizr.min.js` & `bed_reader-1.0.4b2/_static/js/modernizr.min.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/js/theme.js` & `bed_reader-1.0.4b2/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/language_data.js` & `bed_reader-1.0.4b2/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/pygments.css` & `bed_reader-1.0.4b2/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/searchtools.js` & `bed_reader-1.0.4b2/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/sphinx_highlight.js` & `bed_reader-1.0.4b2/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/underscore-1.12.0.js` & `bed_reader-1.0.4b2/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/underscore-1.13.1.js` & `bed_reader-1.0.4b2/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/underscore-1.3.1.js` & `bed_reader-1.0.4b2/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/_static/underscore.js` & `bed_reader-1.0.4b2/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/__init__.py` & `bed_reader-1.0.4b2/bed_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/_open_bed.py` & `bed_reader-1.0.4b2/bed_reader/_open_bed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1341,28 +1341,36 @@
             return open_bed._fix_up_properties_array(
                 np.array(input), dtype, missing_value, key
             )
 
         if len(input.shape) != 1:
             raise ValueError(f"{key} should be one dimensional")
 
-        if not np.issubdtype(input.dtype, dtype):
+        do_missing_values = True
+        if np.issubdtype(input.dtype, np.floating) and np.issubdtype(dtype, int):
+            input[input != input] = missing_value
+            old_settings = np.seterr(invalid="warn")
+            try:
+                output = np.array(input, dtype=dtype)
+            finally:
+                np.seterr(**old_settings)
+        elif not np.issubdtype(input.dtype, dtype):
             # This will convert, for example, numerical sids to string sids or
             # floats that happen to be integers into ints,
             # but there will be a warning generated.
+            old_settings = np.seterr(invalid="warn")
             try:
-                np.seterr(invalid="warn")
                 output = np.array(input, dtype=dtype)
             finally:
-                np.seterr(invalid="raise")
+                np.seterr(**old_settings)
         else:
             output = input
 
         # Change NaN in input to correct missing value
-        if np.issubdtype(input.dtype, np.floating):
+        if do_missing_values and np.issubdtype(input.dtype, np.floating):
             output[input != input] = missing_value
 
         return output
 
     @staticmethod
     def _fix_up_properties(properties, iid_count, sid_count, use_fill_sequence):
         for key in properties:
```

### Comparing `bed_reader-1.0.4b1/bed_reader/_sample_data.py` & `bed_reader-1.0.4b2/bed_reader/_sample_data.py`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/_to_bed.py` & `bed_reader-1.0.4b2/bed_reader/_to_bed.py`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/benchmark/bench2.ipynb` & `bed_reader-1.0.4b2/bed_reader/tests/benchmark/bench2.ipynb`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/benchmark/benchmark.py` & `bed_reader-1.0.4b2/bed_reader/tests/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/registry.txt` & `bed_reader-1.0.4b2/bed_reader/tests/registry.txt`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/test_file_dot.py` & `bed_reader-1.0.4b2/bed_reader/tests/test_file_dot.py`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/test_open_bed.py` & `bed_reader-1.0.4b2/bed_reader/tests/test_open_bed.py`

 * *Files 1% similar despite different names*

```diff
@@ -876,19 +876,18 @@
         to_bed(tmp_path / "ignore", val)
     val = np.zeros((3, 5), dtype=np.str_)
     with pytest.raises(ValueError):
         to_bed(tmp_path / "ignore", val)
 
 
 def test_coverage3(shared_datadir, tmp_path):
-    with pytest.warns(RuntimeWarning, match="invalid value encountered in cast"):
-        with open_bed(
-            shared_datadir / "small.bed", properties={"sex": [1.0, np.nan, 1.0, 2.0]}
-        ) as bed:
-            assert np.array_equal(bed.sex, np.array([1, 0, 1, 2]))
+    with open_bed(
+        shared_datadir / "small.bed", properties={"sex": [1.0, np.nan, 1.0, 2.0]}
+    ) as bed:
+        assert np.array_equal(bed.sex, np.array([1, 0, 1, 2]))
 
     with open_bed(
         shared_datadir / "small.bed",
         properties={"cm_position": [1000.0, np.nan, 2000.0, 3000.0]},
     ) as bed:
         assert np.array_equal(bed.cm_position, np.array([1000, 0, 2000, 3000]))
```

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/test_open_bed_cloud.py` & `bed_reader-1.0.4b2/bed_reader/tests/test_open_bed_cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,20 +708,19 @@
         to_bed(tmp_path / "ignore", val)
     val = np.zeros((3, 5), dtype=np.str_)
     with pytest.raises(ValueError):
         to_bed(tmp_path / "ignore", val)
 
 
 def test_cloud_coverage3(shared_datadir, tmp_path):
-    with pytest.warns(RuntimeWarning, match="invalid value encountered in cast"):
-        with open_bed(
-            file_to_url(shared_datadir / "small.bed"),
-            properties={"sex": [1.0, np.nan, 1.0, 2.0]},
-        ) as bed:
-            assert np.array_equal(bed.sex, np.array([1, 0, 1, 2]))
+    with open_bed(
+        file_to_url(shared_datadir / "small.bed"),
+        properties={"sex": [1.0, np.nan, 1.0, 2.0]},
+    ) as bed:
+        assert np.array_equal(bed.sex, np.array([1, 0, 1, 2]))
 
     with open_bed(
         file_to_url(shared_datadir / "small.bed"),
         properties={"cm_position": [1000.0, np.nan, 2000.0, 3000.0]},
     ) as bed:
         assert np.array_equal(bed.cm_position, np.array([1000, 0, 2000, 3000]))
```

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/test_opt_dep.py` & `bed_reader-1.0.4b2/bed_reader/tests/test_opt_dep.py`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/examples/cloud.rs` & `bed_reader-1.0.4b2/examples/cloud.rs`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/examples/no_cloud.rs` & `bed_reader-1.0.4b2/examples/no_cloud.rs`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/src/bed_cloud.rs` & `bed_reader-1.0.4b2/src/bed_cloud.rs`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/src/lib.rs` & `bed_reader-1.0.4b2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/src/python_module.rs` & `bed_reader-1.0.4b2/src/python_module.rs`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/src/supplemental_documents/cloud_urls_etc.md` & `bed_reader-1.0.4b2/src/supplemental_documents/cloud_urls_etc.md`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/src/supplemental_documents/options_etc.md` & `bed_reader-1.0.4b2/src/supplemental_documents/options_etc.md`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/src/tests.rs` & `bed_reader-1.0.4b2/src/tests.rs`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/tests/tests_api.rs` & `bed_reader-1.0.4b2/tests/tests_api.rs`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/tests/tests_api_cloud.rs` & `bed_reader-1.0.4b2/tests/tests_api_cloud.rs`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/useful.md` & `bed_reader-1.0.4b2/useful.md`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/pyproject.toml` & `bed_reader-1.0.4b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/some_missing.bed` & `bed_reader-1.0.4b2/bed_reader/tests/data/some_missing.bed`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/some_missing.fam` & `bed_reader-1.0.4b2/bed_reader/tests/data/some_missing.fam`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/toydata.5chrom.fam` & `bed_reader-1.0.4b2/bed_reader/tests/data/toydata.5chrom.fam`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/toydata.5chrom.bed` & `bed_reader-1.0.4b2/bed_reader/tests/data/toydata.5chrom.bed`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bim` & `bed_reader-1.0.4b2/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bim`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/sparse.bim` & `bed_reader-1.0.4b2/bed_reader/tests/data/sparse.bim`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/some_missing.val.npy` & `bed_reader-1.0.4b2/bed_reader/tests/data/some_missing.val.npy`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/toydata.5chrom.bim` & `bed_reader-1.0.4b2/bed_reader/tests/data/toydata.5chrom.bim`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/500x400_o640_array.memmap` & `bed_reader-1.0.4b2/bed_reader/tests/data/500x400_o640_array.memmap`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/some_missing.bim` & `bed_reader-1.0.4b2/bed_reader/tests/data/some_missing.bim`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/bed_reader/tests/data/some_missing.properties.npz` & `bed_reader-1.0.4b2/bed_reader/tests/data/some_missing.properties.npz`

 * *Files identical despite different names*

### Comparing `bed_reader-1.0.4b1/PKG-INFO` & `bed_reader-1.0.4b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bed-reader
-Version: 1.0.4b1
+Version: 1.0.4b2
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
```

