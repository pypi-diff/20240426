# Comparing `tmp/pytest-8.1.0.tar.gz` & `tmp/pytest-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-8.1.0.tar", last modified: Sun Mar  3 21:21:07 2024, max compression
+gzip compressed data, was "pytest-8.1.1.tar", last modified: Sat Mar  9 11:49:46 2024, max compression
```

## Comparing `pytest-8.1.0.tar` & `pytest-8.1.1.tar`

### file list

```diff
@@ -1,677 +1,679 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.400143 pytest-8.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-03 21:20:48.000000 pytest-8.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-03 21:20:48.000000 pytest-8.1.0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-03 21:20:48.000000 pytest-8.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.296143 pytest-8.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.296143 pytest-8.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/ISSUE_TEMPLATE/1_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/ISSUE_TEMPLATE/2_feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/labels.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.296143 pytest-8.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/workflows/backport.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/workflows/prepare-release-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-03 21:20:48.000000 pytest-8.1.0/.github/workflows/update-plugin-list.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-03 21:20:48.000000 pytest-8.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-03 21:20:48.000000 pytest-8.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-03 21:20:48.000000 pytest-8.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-03-03 21:20:48.000000 pytest-8.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-03 21:20:48.000000 pytest-8.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-03 21:20:48.000000 pytest-8.1.0/CITATION
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-03 21:20:48.000000 pytest-8.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    20372 2024-03-03 21:20:48.000000 pytest-8.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-03 21:20:48.000000 pytest-8.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-03 21:20:48.000000 pytest-8.1.0/OPENCOLLECTIVE.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-03 21:21:07.400143 pytest-8.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-03-03 21:20:48.000000 pytest-8.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-03-03 21:20:48.000000 pytest-8.1.0/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-03 21:20:48.000000 pytest-8.1.0/TIDELIFT.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.300143 pytest-8.1.0/bench/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-03 21:20:48.000000 pytest-8.1.0/bench/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-03 21:20:48.000000 pytest-8.1.0/bench/bench_argcomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-03 21:20:48.000000 pytest-8.1.0/bench/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-03 21:20:48.000000 pytest-8.1.0/bench/manyparam.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-03 21:20:48.000000 pytest-8.1.0/bench/skip.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-03 21:20:48.000000 pytest-8.1.0/bench/unit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-03 21:20:48.000000 pytest-8.1.0/bench/xunit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.300143 pytest-8.1.0/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-03 21:20:48.000000 pytest-8.1.0/changelog/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-03 21:20:48.000000 pytest-8.1.0/changelog/_template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-03 21:20:48.000000 pytest-8.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.284143 pytest-8.1.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.304143 pytest-8.1.0/doc/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.304143 pytest-8.1.0/doc/en/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/_templates/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/_templates/links.html
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/_templates/relations.html
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/_templates/sidebarintro.html
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/_templates/slim_searchbox.html
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/adopt.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.336143 pytest-8.1.0/doc/en/announce/
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.0.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.1.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.2.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.3.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.3.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.3.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.3.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.5.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.5.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.5.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.6.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.6.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.6.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.6.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.7.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.7.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.7.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.8.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.8.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.8.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.8.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.8.6.rst
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.8.7.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.9.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.9.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-2.9.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.0.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.0.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.0.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.0.6.rst
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.0.7.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.1.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.10.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.10.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.2.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.2.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.2.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.3.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.5.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.5.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.6.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.6.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.6.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.6.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.6.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.7.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.7.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.7.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.7.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.7.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.8.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.8.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.8.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.9.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.9.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.9.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-3.9.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.5.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.6.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.6.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.6.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.6.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.6.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.6.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.6.6.rst
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.6.7.rst
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.6.8.rst
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-4.6.9.rst
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.1.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.2.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.2.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.3.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.3.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.3.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.3.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-5.4.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.0.0rc1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.2.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.2.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-6.2.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.0.0rc1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.1.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.3.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.4.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-7.4.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-8.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-8.0.0rc1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-8.0.0rc2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-8.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-8.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/release-8.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/announce/sprint2016.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/backwards-compatibility.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/builtin.rst
--rw-r--r--   0 runner    (1001) docker     (127)   404747 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/contents.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    38988 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/deprecations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/development_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.336143 pytest-8.1.0/doc/en/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.340143 pytest-8.1.0/doc/en/example/assertion/
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/assertion/failure_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.340143 pytest-8.1.0/doc/en/example/assertion/global_testmodule_config/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/assertion/global_testmodule_config/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/assertion/global_testmodule_config/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/assertion/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/assertion/test_setup_flow_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/attic.rst
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.340143 pytest-8.1.0/doc/en/example/customdirectory/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/customdirectory/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/customdirectory/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.340143 pytest-8.1.0/doc/en/example/customdirectory/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/customdirectory/tests/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/customdirectory/tests/test_first.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/customdirectory/tests/test_second.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/customdirectory/tests/test_third.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/customdirectory.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.344143 pytest-8.1.0/doc/en/example/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/fixture_availability.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/fixture_availability_plugins.svg
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse_flat.svg
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.svg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.svg
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_dependencies.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_dependencies_flat.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_dependencies_unclear.svg
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_scope.svg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_request_different_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/fixtures/test_fixtures_request_different_scope.svg
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26471 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/markers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/multipython.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.344143 pytest-8.1.0/doc/en/example/nonpython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/nonpython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/nonpython/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/nonpython/test_simple.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/nonpython.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22718 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/parametrize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/pythoncollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/pythoncollection.rst
--rw-r--r--   0 runner    (1001) docker     (127)    27266 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/reportingdemo.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35232 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/simple.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/special.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/example/xfail_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.344143 pytest-8.1.0/doc/en/explanation/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/explanation/anatomy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/explanation/fixtures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/explanation/flaky.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/explanation/goodpractices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/explanation/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/explanation/pythonpath.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/funcarg_compare.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/funcargs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/historical-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.348143 pytest-8.1.0/doc/en/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/assert.rst
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/bash-completion.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/capture-stdout-stderr.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/capture-warnings.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/doctest.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/existingtestsuite.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/failures.rst
--rw-r--r--   0 runner    (1001) docker     (127)    62010 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/fixtures.rst
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/mark.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/monkeypatch.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29330 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/output.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9828 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/parametrize.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/skipping.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/tmp_path.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/unittest.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/writing_hook_functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/writing_plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/how-to/xunit_setup.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.352143 pytest-8.1.0/doc/en/img/
--rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/img/cramer2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/img/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)   104057 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/img/freiburg2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/img/gaynor3.png
--rw-r--r--   0 runner    (1001) docker     (127)    23246 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/img/keleshev.png
--rw-r--r--   0 runner    (1001) docker     (127)    17035 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/img/pullrequest.png
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/img/pylib.png
--rw-r--r--   0 runner    (1001) docker     (127)    40974 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/img/pytest1.png
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/img/pytest_logo_curves.svg
--rw-r--r--   0 runner    (1001) docker     (127)    31476 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/img/theuni.png
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/naming20.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.352143 pytest-8.1.0/doc/en/proposals/
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/proposals/parametrize_with_fixtures.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/recwarn.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.352143 pytest-8.1.0/doc/en/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/reference/customize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/reference/exit-codes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16327 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/reference/fixtures.rst
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)   921217 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/reference/plugin_list.rst
--rw-r--r--   0 runner    (1001) docker     (127)    66318 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/reference/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/sponsor.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/talks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/tidelift.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-03 21:20:48.000000 pytest-8.1.0/doc/en/yieldfixture.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.352143 pytest-8.1.0/extra/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-03 21:20:48.000000 pytest-8.1.0/extra/get_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-03 21:20:48.000000 pytest-8.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.356143 pytest-8.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-03 21:20:48.000000 pytest-8.1.0/scripts/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-03 21:20:48.000000 pytest-8.1.0/scripts/generate-gh-release-notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-03-03 21:20:48.000000 pytest-8.1.0/scripts/prepare-release-pr.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-03 21:20:48.000000 pytest-8.1.0/scripts/release.major.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-03 21:20:48.000000 pytest-8.1.0/scripts/release.minor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-03 21:20:48.000000 pytest-8.1.0/scripts/release.patch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-03 21:20:48.000000 pytest-8.1.0/scripts/release.pre.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-03-03 21:20:48.000000 pytest-8.1.0/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-03 21:20:48.000000 pytest-8.1.0/scripts/towncrier-draft-to-file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-03-03 21:20:48.000000 pytest-8.1.0/scripts/update-plugin-list.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 21:21:07.400143 pytest-8.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.356143 pytest-8.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.364143 pytest-8.1.0/src/_pytest/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_argcomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.364143 pytest-8.1.0/src/_pytest/_code/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50043 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_code/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_code/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.364143 pytest-8.1.0/src/_pytest/_io/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19665 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_io/pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_io/saferepr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_io/terminalwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_io/wcwidth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.368143 pytest-8.1.0/src/_pytest/_py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_py/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    49888 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/_py/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-03 21:21:07.000000 pytest-8.1.0/src/_pytest/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.368143 pytest-8.1.0/src/_pytest/assertion/
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/assertion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47200 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/assertion/rewrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/assertion/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)    20307 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/assertion/util.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21140 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/cacheprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)    34963 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.368143 pytest-8.1.0/src/_pytest/config/
--rw-r--r--   0 runner    (1001) docker     (127)    69888 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/config/argparsing.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/config/findpaths.py
--rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    26051 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/faulthandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    67942 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/freeze_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/helpconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    41379 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/hookspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    25664 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/junitxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/legacypath.py
--rw-r--r--   0 runner    (1001) docker     (127)    35440 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    37466 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.368143 pytest-8.1.0/src/_pytest/mark/
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/mark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/mark/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/mark/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    25505 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/outcomes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (127)    30951 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    61879 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/pytester.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/pytester_assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)    69964 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    39138 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/python_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    13690 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/recwarn.py
--rw-r--r--   0 runner    (1001) docker     (127)    20911 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    19311 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/setuponly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/setupplan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/skipping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/stepwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    54950 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/threadexception.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/tmpdir.py
--rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/unraisableexception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/warning_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-03-03 21:20:48.000000 pytest-8.1.0/src/_pytest/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-03 21:20:48.000000 pytest-8.1.0/src/py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.368143 pytest-8.1.0/src/pytest/
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-03-03 21:20:48.000000 pytest-8.1.0/src/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-03 21:20:48.000000 pytest-8.1.0/src/pytest/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/src/pytest/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.400143 pytest-8.1.0/src/pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-03 21:21:07.000000 pytest-8.1.0/src/pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-03-03 21:21:07.000000 pytest-8.1.0/src/pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 21:21:07.000000 pytest-8.1.0/src/pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-03 21:21:07.000000 pytest-8.1.0/src/pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-03 21:21:07.000000 pytest-8.1.0/src/pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-03 21:21:07.000000 pytest-8.1.0/src/pytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.380143 pytest-8.1.0/testing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.380143 pytest-8.1.0/testing/_py/
--rw-r--r--   0 runner    (1001) docker     (127)    52687 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/_py/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/acceptance_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.380143 pytest-8.1.0/testing/code/
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/code/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    59954 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/code/test_excinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/code/test_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/deprecated_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.380143 pytest-8.1.0/testing/example_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.380143 pytest-8.1.0/testing/example_scripts/acceptance/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/acceptance/fixture_mock_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.288143 pytest-8.1.0/testing/example_scripts/collect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.380143 pytest-8.1.0/testing/example_scripts/collect/collect_init_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/collect/collect_init_tests/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.384143 pytest-8.1.0/testing/example_scripts/collect/collect_init_tests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/collect/collect_init_tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/collect/collect_init_tests/tests/test_foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.384143 pytest-8.1.0/testing/example_scripts/collect/package_infinite_recursion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/collect/package_infinite_recursion/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/collect/package_infinite_recursion/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.384143 pytest-8.1.0/testing/example_scripts/collect/package_infinite_recursion/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/collect/package_infinite_recursion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/collect/package_infinite_recursion/tests/test_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.288143 pytest-8.1.0/testing/example_scripts/collect/package_init_given_as_arg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.384143 pytest-8.1.0/testing/example_scripts/collect/package_init_given_as_arg/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/collect/package_init_given_as_arg/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/collect/package_init_given_as_arg/pkg/test_foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.288143 pytest-8.1.0/testing/example_scripts/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.384143 pytest-8.1.0/testing/example_scripts/config/collect_pytest_prefix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/config/collect_pytest_prefix/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/config/collect_pytest_prefix/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/config/collect_pytest_prefix/test_foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.384143 pytest-8.1.0/testing/example_scripts/conftest_usageerror/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/conftest_usageerror/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/conftest_usageerror/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.384143 pytest-8.1.0/testing/example_scripts/customdirectory/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/customdirectory/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/customdirectory/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.384143 pytest-8.1.0/testing/example_scripts/customdirectory/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/customdirectory/tests/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/customdirectory/tests/test_first.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/customdirectory/tests/test_second.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/customdirectory/tests/test_third.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.384143 pytest-8.1.0/testing/example_scripts/dataclasses/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/dataclasses/test_compare_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/dataclasses/test_compare_dataclasses_field_comparison_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/dataclasses/test_compare_dataclasses_verbose.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/dataclasses/test_compare_dataclasses_with_custom_eq.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/dataclasses/test_compare_initvar.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/dataclasses/test_compare_recursive_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/dataclasses/test_compare_two_different_dataclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.288143 pytest-8.1.0/testing/example_scripts/doctest/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.388143 pytest-8.1.0/testing/example_scripts/doctest/main_py/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/doctest/main_py/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/doctest/main_py/test_normal_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.388143 pytest-8.1.0/testing/example_scripts/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.388143 pytest-8.1.0/testing/example_scripts/fixtures/custom_item/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/custom_item/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/custom_item/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.388143 pytest-8.1.0/testing/example_scripts/fixtures/custom_item/foo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/custom_item/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/custom_item/foo/test_foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.388143 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.288143 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.388143 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/test_in_sub1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.388143 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/test_in_sub2.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_detect_recursive_dependency_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.388143 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.388143 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/test_spam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.392143 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/test_extend_fixture_conftest_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_module_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookup_classlevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookup_modulelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookupfails.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/test_fixture_named_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/fixtures/test_getfixturevalue_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.392143 pytest-8.1.0/testing/example_scripts/issue88_initial_file_multinodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/issue88_initial_file_multinodes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/issue88_initial_file_multinodes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/issue88_initial_file_multinodes/test_hello.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/issue_519.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/junit-10.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.292143 pytest-8.1.0/testing/example_scripts/marks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.392143 pytest-8.1.0/testing/example_scripts/marks/marks_considered_keywords/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/marks/marks_considered_keywords/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/marks/marks_considered_keywords/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/marks/marks_considered_keywords/test_marks_as_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.292143 pytest-8.1.0/testing/example_scripts/perf_examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.392143 pytest-8.1.0/testing/example_scripts/perf_examples/collect_stats/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/perf_examples/collect_stats/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/perf_examples/collect_stats/generate_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/perf_examples/collect_stats/template_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.392143 pytest-8.1.0/testing/example_scripts/tmpdir/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/tmpdir/tmp_path_fixture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.392143 pytest-8.1.0/testing/example_scripts/unittest/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/unittest/test_parametrized_fixture_error_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/unittest/test_setup_skip.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/unittest/test_setup_skip_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/unittest/test_setup_skip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/unittest/test_unittest_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/unittest/test_unittest_asynctest.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/unittest/test_unittest_plain_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.392143 pytest-8.1.0/testing/example_scripts/warnings/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/warnings/test_group_warnings_by_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.392143 pytest-8.1.0/testing/example_scripts/warnings/test_group_warnings_by_message_summary/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/warnings/test_group_warnings_by_message_summary/test_1.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/example_scripts/warnings/test_group_warnings_by_message_summary/test_2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.392143 pytest-8.1.0/testing/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/examples/test_issue519.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.392143 pytest-8.1.0/testing/freeze/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/freeze/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/freeze/create_executable.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/freeze/runtests_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.396143 pytest-8.1.0/testing/freeze/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/freeze/tests/test_doctest.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/freeze/tests/test_trivial.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/freeze/tox_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.396143 pytest-8.1.0/testing/io/
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/io/test_pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/io/test_saferepr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/io/test_terminalwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/io/test_wcwidth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.396143 pytest-8.1.0/testing/logging/
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/logging/test_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/logging/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    47293 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/logging/test_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.396143 pytest-8.1.0/testing/plugins_integration/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/bdd_wallet.feature
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/bdd_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/django_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/pytest_anyio_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/pytest_asyncio_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/pytest_mock_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/pytest_trio_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/pytest_twisted_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/plugins_integration/simple_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 21:21:07.400143 pytest-8.1.0/testing/python/
--rw-r--r--   0 runner    (1001) docker     (127)    34588 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/python/approx.py
--rw-r--r--   0 runner    (1001) docker     (127)    52366 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/python/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)   140883 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/python/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/python/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    70079 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/python/metafunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11768 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/python/raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/python/show_fixtures_per_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_argcomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    65668 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)    66663 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_assertrewrite.py
--rw-r--r--   0 runner    (1001) docker     (127)    45293 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_cacheprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)    52300 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    65092 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    79579 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25187 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    42797 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)    50721 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_error_diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_faulthandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_findpaths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_helpconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    57790 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_junitxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_legacypath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_link_resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)    11332 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    34663 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_mark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_mark_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    12801 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_parseopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_pastebin.py
--rw-r--r--   0 runner    (1001) docker     (127)    41768 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    17284 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_pluginmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    27327 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_pytester.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_recwarn.py
--rw-r--r--   0 runner    (1001) docker     (127)    19992 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    34598 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_runner_xunit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    15424 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_setuponly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_setupplan.py
--rw-r--r--   0 runner    (1001) docker     (127)    43971 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_skipping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    10633 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_stepwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    98552 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_threadexception.py
--rw-r--r--   0 runner    (1001) docker     (127)    19532 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_tmpdir.py
--rw-r--r--   0 runner    (1001) docker     (127)    45389 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_unraisableexception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_warning_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/test_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-03 21:20:48.000000 pytest-8.1.0/testing/typing_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-03-03 21:20:48.000000 pytest-8.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.633274 pytest-8.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-09 11:49:29.000000 pytest-8.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-09 11:49:29.000000 pytest-8.1.1/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-09 11:49:29.000000 pytest-8.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.521274 pytest-8.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.521274 pytest-8.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/ISSUE_TEMPLATE/1_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/ISSUE_TEMPLATE/2_feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/labels.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.525274 pytest-8.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/backport.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/prepare-release-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/update-plugin-list.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-09 11:49:29.000000 pytest-8.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-09 11:49:29.000000 pytest-8.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-09 11:49:29.000000 pytest-8.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-03-09 11:49:29.000000 pytest-8.1.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-09 11:49:29.000000 pytest-8.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-09 11:49:29.000000 pytest-8.1.1/CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-09 11:49:29.000000 pytest-8.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20372 2024-03-09 11:49:29.000000 pytest-8.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-09 11:49:29.000000 pytest-8.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-09 11:49:29.000000 pytest-8.1.1/OPENCOLLECTIVE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-09 11:49:46.633274 pytest-8.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-03-09 11:49:29.000000 pytest-8.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-03-09 11:49:29.000000 pytest-8.1.1/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-09 11:49:29.000000 pytest-8.1.1/TIDELIFT.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.525274 pytest-8.1.1/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/bench_argcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/manyparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/skip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/xunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.525274 pytest-8.1.1/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-09 11:49:29.000000 pytest-8.1.1/changelog/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-09 11:49:29.000000 pytest-8.1.1/changelog/_template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-09 11:49:29.000000 pytest-8.1.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.509275 pytest-8.1.1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.529274 pytest-8.1.1/doc/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.533274 pytest-8.1.1/doc/en/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/relations.html
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/sidebarintro.html
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/slim_searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/adopt.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.565274 pytest-8.1.1/doc/en/announce/
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.0.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.2.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.5.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.5.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.5.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.6.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.6.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.6.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.6.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.7.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.7.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.7.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.6.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.7.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.9.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.9.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.9.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.6.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.7.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.10.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.10.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.3.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.5.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.5.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.6.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.6.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.6.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.6.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.6.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.7.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.7.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.7.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.7.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.7.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.8.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.8.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.8.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.9.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.9.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.9.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.9.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.5.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.6.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.7.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.8.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.9.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.2.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.2.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.4.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.0.0rc1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.0.0rc1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.3.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.4.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.4.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.0.0rc1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.0.0rc2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/sprint2016.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/backwards-compatibility.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/builtin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   405803 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    38963 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/deprecations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/development_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.569274 pytest-8.1.1/doc/en/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.569274 pytest-8.1.1/doc/en/example/assertion/
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/assertion/failure_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.569274 pytest-8.1.1/doc/en/example/assertion/global_testmodule_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/assertion/global_testmodule_config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/assertion/global_testmodule_config/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/assertion/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/assertion/test_setup_flow_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/attic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.569274 pytest-8.1.1/doc/en/example/customdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.569274 pytest-8.1.1/doc/en/example/customdirectory/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/tests/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/tests/test_first.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/tests/test_second.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/tests/test_third.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.573274 pytest-8.1.1/doc/en/example/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/fixture_availability.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/fixture_availability_plugins.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_flat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies_flat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies_unclear.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_scope.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_request_different_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_request_different_scope.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26471 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/multipython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.573274 pytest-8.1.1/doc/en/example/nonpython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/nonpython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/nonpython/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/nonpython/test_simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/nonpython.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22718 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/parametrize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/pythoncollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/pythoncollection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    27266 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/reportingdemo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35232 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/simple.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/special.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/xfail_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.573274 pytest-8.1.1/doc/en/explanation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/anatomy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/fixtures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/flaky.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/goodpractices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/pythonpath.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/funcarg_compare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/funcargs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/historical-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.581274 pytest-8.1.1/doc/en/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/assert.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/bash-completion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/capture-stdout-stderr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/capture-warnings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/doctest.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/existingtestsuite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/failures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    62010 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/fixtures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/mark.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/monkeypatch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29330 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/output.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9828 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/parametrize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/skipping.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/tmp_path.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/unittest.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/writing_hook_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/writing_plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/xunit_setup.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.581274 pytest-8.1.1/doc/en/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/cramer2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   104057 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/freiburg2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/gaynor3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23246 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/keleshev.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17035 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/pullrequest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/pylib.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40974 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/pytest1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/pytest_logo_curves.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    31476 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/theuni.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/naming20.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.581274 pytest-8.1.1/doc/en/proposals/
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/proposals/parametrize_with_fixtures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/recwarn.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.585274 pytest-8.1.1/doc/en/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/customize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/exit-codes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16327 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/fixtures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   921217 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/plugin_list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    66318 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/sponsor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/talks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/tidelift.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/yieldfixture.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.585274 pytest-8.1.1/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-09 11:49:29.000000 pytest-8.1.1/extra/get_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-09 11:49:29.000000 pytest-8.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.585274 pytest-8.1.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/generate-gh-release-notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/prepare-release-pr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/release.major.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/release.minor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/release.patch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/release.pre.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/towncrier-draft-to-file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/update-plugin-list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 11:49:46.633274 pytest-8.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.585274 pytest-8.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.593274 pytest-8.1.1/src/_pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_argcomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.593274 pytest-8.1.1/src/_pytest/_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50043 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_code/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_code/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.597274 pytest-8.1.1/src/_pytest/_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19665 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_io/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_io/saferepr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_io/terminalwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_io/wcwidth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.597274 pytest-8.1.1/src/_pytest/_py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_py/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49888 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_py/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-09 11:49:46.000000 pytest-8.1.1/src/_pytest/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.597274 pytest-8.1.1/src/_pytest/assertion/
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/assertion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47200 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/assertion/rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/assertion/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20307 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/assertion/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21140 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/cacheprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34963 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.597274 pytest-8.1.1/src/_pytest/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    69979 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/config/argparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/config/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/config/findpaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/debugging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26051 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/faulthandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67942 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/freeze_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/helpconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41418 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/hookspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25664 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/junitxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/legacypath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35440 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37564 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.597274 pytest-8.1.1/src/_pytest/mark/
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/mark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/mark/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/mark/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26733 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    61879 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/pytester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/pytester_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70069 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39138 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/python_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13690 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/recwarn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20911 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19311 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/setuponly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/setupplan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/skipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54950 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/threadexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/tmpdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/unraisableexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/warning_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-09 11:49:29.000000 pytest-8.1.1/src/py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.601274 pytest-8.1.1/src/pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-03-09 11:49:29.000000 pytest-8.1.1/src/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-09 11:49:29.000000 pytest-8.1.1/src/pytest/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/src/pytest/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.633274 pytest-8.1.1/src/pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21867 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.609274 pytest-8.1.1/testing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.609274 pytest-8.1.1/testing/_py/
+-rw-r--r--   0 runner    (1001) docker     (127)    52687 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/_py/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/acceptance_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/code/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59954 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/code/test_excinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/code/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/deprecated_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/acceptance/fixture_mock_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.513275 pytest-8.1.1/testing/example_scripts/collect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/collect/collect_init_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/collect_init_tests/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/collect/collect_init_tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/collect_init_tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/collect_init_tests/tests/test_foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.513275 pytest-8.1.1/testing/example_scripts/collect/package_init_given_as_arg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/collect/package_init_given_as_arg/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_init_given_as_arg/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_init_given_as_arg/pkg/test_foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.513275 pytest-8.1.1/testing/example_scripts/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/config/collect_pytest_prefix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/config/collect_pytest_prefix/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/config/collect_pytest_prefix/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/config/collect_pytest_prefix/test_foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/conftest_usageerror/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/conftest_usageerror/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/conftest_usageerror/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/customdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/customdirectory/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/tests/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/tests/test_first.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/tests/test_second.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/tests/test_third.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_dataclasses_field_comparison_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_dataclasses_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_dataclasses_with_custom_eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_initvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_recursive_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_two_different_dataclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.513275 pytest-8.1.1/testing/example_scripts/doctest/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/doctest/main_py/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/doctest/main_py/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/doctest/main_py/test_normal_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/foo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/foo/test_foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.513275 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/test_in_sub1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/test_in_sub2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_detect_recursive_dependency_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/test_spam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/test_extend_fixture_conftest_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_module_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookup_classlevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookup_modulelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookupfails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/test_fixture_named_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/test_getfixturevalue_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/issue88_initial_file_multinodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/issue88_initial_file_multinodes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/issue88_initial_file_multinodes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/issue88_initial_file_multinodes/test_hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/issue_519.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/junit-10.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.517274 pytest-8.1.1/testing/example_scripts/marks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/marks/marks_considered_keywords/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/marks/marks_considered_keywords/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/marks/marks_considered_keywords/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/marks/marks_considered_keywords/test_marks_as_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.517274 pytest-8.1.1/testing/example_scripts/perf_examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/example_scripts/perf_examples/collect_stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/perf_examples/collect_stats/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/perf_examples/collect_stats/generate_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/perf_examples/collect_stats/template_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/example_scripts/tmpdir/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/tmpdir/tmp_path_fixture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/example_scripts/unittest/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_parametrized_fixture_error_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_setup_skip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_setup_skip_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_setup_skip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_unittest_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_unittest_asynctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_unittest_plain_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/example_scripts/warnings/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/warnings/test_group_warnings_by_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/example_scripts/warnings/test_group_warnings_by_message_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/warnings/test_group_warnings_by_message_summary/test_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/warnings/test_group_warnings_by_message_summary/test_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/examples/test_issue519.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/freeze/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/create_executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/runtests_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/freeze/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/tests/test_doctest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/tests/test_trivial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/tox_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.629274 pytest-8.1.1/testing/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/io/test_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/io/test_saferepr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/io/test_terminalwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/io/test_wcwidth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.629274 pytest-8.1.1/testing/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/logging/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/logging/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47293 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/logging/test_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.629274 pytest-8.1.1/testing/plugins_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/bdd_wallet.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/bdd_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/django_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest_anyio_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest_asyncio_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest_mock_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest_trio_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest_twisted_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/simple_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.633274 pytest-8.1.1/testing/python/
+-rw-r--r--   0 runner    (1001) docker     (127)    34588 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/approx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52366 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)   140883 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70079 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/metafunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11768 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/show_fixtures_per_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_argcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65668 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66663 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_assertrewrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45293 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_cacheprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52300 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65092 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79579 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25187 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42797 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50721 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_error_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_faulthandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_findpaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_helpconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57790 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_junitxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_legacypath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_link_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11332 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34663 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_mark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_mark_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12801 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_parseopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43988 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17284 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_pluginmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27327 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_pytester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_recwarn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19992 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34598 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_runner_xunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15424 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_setuponly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_setupplan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43971 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_skipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10633 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98552 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_threadexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19532 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_tmpdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45389 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_unraisableexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_warning_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/typing_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-03-09 11:49:29.000000 pytest-8.1.1/tox.ini
```

### Comparing `pytest-8.1.0/.coveragerc` & `pytest-8.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.git-blame-ignore-revs` & `pytest-8.1.1/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.github/ISSUE_TEMPLATE/2_feature_request.md` & `pytest-8.1.1/.github/ISSUE_TEMPLATE/2_feature_request.md`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `pytest-8.1.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.github/labels.toml` & `pytest-8.1.1/.github/labels.toml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.github/workflows/backport.yml` & `pytest-8.1.1/.github/workflows/backport.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.github/workflows/deploy.yml` & `pytest-8.1.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.github/workflows/prepare-release-pr.yml` & `pytest-8.1.1/.github/workflows/prepare-release-pr.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.github/workflows/stale.yml` & `pytest-8.1.1/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.github/workflows/test.yml` & `pytest-8.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.github/workflows/update-plugin-list.yml` & `pytest-8.1.1/.github/workflows/update-plugin-list.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.gitignore` & `pytest-8.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/.pre-commit-config.yaml` & `pytest-8.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/AUTHORS` & `pytest-8.1.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/CODE_OF_CONDUCT.md` & `pytest-8.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/CONTRIBUTING.rst` & `pytest-8.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/LICENSE` & `pytest-8.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/OPENCOLLECTIVE.rst` & `pytest-8.1.1/OPENCOLLECTIVE.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/PKG-INFO` & `pytest-8.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest
-Version: 8.1.0
+Version: 8.1.1
 Summary: pytest: simple powerful testing with Python
 Author: Holger Krekel, Bruno Oliveira, Ronny Pfannschmidt, Floris Bruynooghe, Brianna Laugher, Florian Bruhin, Others (See AUTHORS)
 License: MIT
 Project-URL: Changelog, https://docs.pytest.org/en/stable/changelog.html
 Project-URL: Homepage, https://docs.pytest.org/en/latest/
 Project-URL: Source, https://github.com/pytest-dev/pytest
 Project-URL: Tracker, https://github.com/pytest-dev/pytest/issues
```

### Comparing `pytest-8.1.0/README.rst` & `pytest-8.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/RELEASING.rst` & `pytest-8.1.1/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/TIDELIFT.rst` & `pytest-8.1.1/TIDELIFT.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/bench/bench_argcomplete.py` & `pytest-8.1.1/bench/bench_argcomplete.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/changelog/README.rst` & `pytest-8.1.1/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/changelog/_template.rst` & `pytest-8.1.1/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/Makefile` & `pytest-8.1.1/doc/en/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/_templates/globaltoc.html` & `pytest-8.1.1/doc/en/_templates/globaltoc.html`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/_templates/layout.html` & `pytest-8.1.1/doc/en/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/_templates/relations.html` & `pytest-8.1.1/doc/en/_templates/relations.html`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/_templates/slim_searchbox.html` & `pytest-8.1.1/doc/en/_templates/slim_searchbox.html`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/adopt.rst` & `pytest-8.1.1/doc/en/adopt.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/index.rst` & `pytest-8.1.1/doc/en/announce/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Release announcements
 ===========================================
 
 .. toctree::
    :maxdepth: 2
 
 
+   release-8.1.1
    release-8.1.0
    release-8.0.2
    release-8.0.1
    release-8.0.0
    release-8.0.0rc2
    release-8.0.0rc1
    release-7.4.4
```

### Comparing `pytest-8.1.0/doc/en/announce/release-2.0.0.rst` & `pytest-8.1.1/doc/en/announce/release-2.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.0.1.rst` & `pytest-8.1.1/doc/en/announce/release-2.0.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.0.2.rst` & `pytest-8.1.1/doc/en/announce/release-2.0.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.0.3.rst` & `pytest-8.1.1/doc/en/announce/release-2.0.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.1.0.rst` & `pytest-8.1.1/doc/en/announce/release-2.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.1.1.rst` & `pytest-8.1.1/doc/en/announce/release-2.1.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.1.2.rst` & `pytest-8.1.1/doc/en/announce/release-2.1.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.1.3.rst` & `pytest-8.1.1/doc/en/announce/release-2.1.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.2.0.rst` & `pytest-8.1.1/doc/en/announce/release-2.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.2.1.rst` & `pytest-8.1.1/doc/en/announce/release-2.2.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.2.2.rst` & `pytest-8.1.1/doc/en/announce/release-2.2.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.2.4.rst` & `pytest-8.1.1/doc/en/announce/release-2.2.4.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.3.0.rst` & `pytest-8.1.1/doc/en/announce/release-2.3.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.3.1.rst` & `pytest-8.1.1/doc/en/announce/release-2.3.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.3.2.rst` & `pytest-8.1.1/doc/en/announce/release-2.3.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.3.3.rst` & `pytest-8.1.1/doc/en/announce/release-2.3.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.3.4.rst` & `pytest-8.1.1/doc/en/announce/release-2.3.4.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.3.5.rst` & `pytest-8.1.1/doc/en/announce/release-2.3.5.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.4.0.rst` & `pytest-8.1.1/doc/en/announce/release-2.4.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.4.1.rst` & `pytest-8.1.1/doc/en/announce/release-2.4.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.4.2.rst` & `pytest-8.1.1/doc/en/announce/release-2.4.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.5.0.rst` & `pytest-8.1.1/doc/en/announce/release-2.5.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.5.1.rst` & `pytest-8.1.1/doc/en/announce/release-2.5.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.5.2.rst` & `pytest-8.1.1/doc/en/announce/release-2.5.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.6.0.rst` & `pytest-8.1.1/doc/en/announce/release-2.6.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.6.1.rst` & `pytest-8.1.1/doc/en/announce/release-2.6.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.6.2.rst` & `pytest-8.1.1/doc/en/announce/release-2.6.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.6.3.rst` & `pytest-8.1.1/doc/en/announce/release-2.6.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.7.0.rst` & `pytest-8.1.1/doc/en/announce/release-2.7.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.7.1.rst` & `pytest-8.1.1/doc/en/announce/release-2.7.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.7.2.rst` & `pytest-8.1.1/doc/en/announce/release-2.7.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.8.2.rst` & `pytest-8.1.1/doc/en/announce/release-2.8.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.8.3.rst` & `pytest-8.1.1/doc/en/announce/release-2.8.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.8.4.rst` & `pytest-8.1.1/doc/en/announce/release-2.8.4.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.8.5.rst` & `pytest-8.1.1/doc/en/announce/release-2.8.5.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.8.6.rst` & `pytest-8.1.1/doc/en/announce/release-2.8.6.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.8.7.rst` & `pytest-8.1.1/doc/en/announce/release-2.8.7.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.9.0.rst` & `pytest-8.1.1/doc/en/announce/release-2.9.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.9.1.rst` & `pytest-8.1.1/doc/en/announce/release-2.9.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-2.9.2.rst` & `pytest-8.1.1/doc/en/announce/release-2.9.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.0.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.0.1.rst` & `pytest-8.1.1/doc/en/announce/release-3.0.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.0.2.rst` & `pytest-8.1.1/doc/en/announce/release-3.0.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.0.3.rst` & `pytest-8.1.1/doc/en/announce/release-3.0.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.0.4.rst` & `pytest-8.1.1/doc/en/announce/release-3.0.4.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.0.5.rst` & `pytest-8.1.1/doc/en/announce/release-3.0.5.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.0.6.rst` & `pytest-8.1.1/doc/en/announce/release-3.0.6.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.0.7.rst` & `pytest-8.1.1/doc/en/announce/release-3.0.7.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.1.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.10.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.10.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.10.1.rst` & `pytest-8.1.1/doc/en/announce/release-3.10.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.2.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.2.2.rst` & `pytest-8.1.1/doc/en/announce/release-3.2.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.2.4.rst` & `pytest-8.1.1/doc/en/announce/release-3.2.4.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.3.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.3.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.3.1.rst` & `pytest-8.1.1/doc/en/announce/release-3.3.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.3.2.rst` & `pytest-8.1.1/doc/en/announce/release-3.3.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.4.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.4.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.4.1.rst` & `pytest-8.1.1/doc/en/announce/release-3.4.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.4.2.rst` & `pytest-8.1.1/doc/en/announce/release-3.4.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.5.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.5.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.5.1.rst` & `pytest-8.1.1/doc/en/announce/release-3.5.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.6.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.6.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.6.1.rst` & `pytest-8.1.1/doc/en/announce/release-3.6.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.6.2.rst` & `pytest-8.1.1/doc/en/announce/release-3.6.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.6.3.rst` & `pytest-8.1.1/doc/en/announce/release-3.6.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.7.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.7.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.7.2.rst` & `pytest-8.1.1/doc/en/announce/release-3.7.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.7.3.rst` & `pytest-8.1.1/doc/en/announce/release-3.7.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.8.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.8.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.8.1.rst` & `pytest-8.1.1/doc/en/announce/release-3.8.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.8.2.rst` & `pytest-8.1.1/doc/en/announce/release-3.8.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-3.9.0.rst` & `pytest-8.1.1/doc/en/announce/release-3.9.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.0.0.rst` & `pytest-8.1.1/doc/en/announce/release-4.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.1.0.rst` & `pytest-8.1.1/doc/en/announce/release-4.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.1.1.rst` & `pytest-8.1.1/doc/en/announce/release-4.1.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.2.0.rst` & `pytest-8.1.1/doc/en/announce/release-4.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.2.1.rst` & `pytest-8.1.1/doc/en/announce/release-4.2.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.3.0.rst` & `pytest-8.1.1/doc/en/announce/release-4.3.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.3.1.rst` & `pytest-8.1.1/doc/en/announce/release-4.3.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.4.0.rst` & `pytest-8.1.1/doc/en/announce/release-4.4.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.4.2.rst` & `pytest-8.1.1/doc/en/announce/release-4.4.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.5.0.rst` & `pytest-8.1.1/doc/en/announce/release-4.5.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-4.6.0.rst` & `pytest-8.1.1/doc/en/announce/release-4.6.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.0.0.rst` & `pytest-8.1.1/doc/en/announce/release-5.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.0.1.rst` & `pytest-8.1.1/doc/en/announce/release-5.0.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.1.0.rst` & `pytest-8.1.1/doc/en/announce/release-5.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.1.1.rst` & `pytest-8.1.1/doc/en/announce/release-5.1.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.2.0.rst` & `pytest-8.1.1/doc/en/announce/release-5.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.2.2.rst` & `pytest-8.1.1/doc/en/announce/release-5.2.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.2.3.rst` & `pytest-8.1.1/doc/en/announce/release-5.2.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.3.0.rst` & `pytest-8.1.1/doc/en/announce/release-5.3.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.3.1.rst` & `pytest-8.1.1/doc/en/announce/release-5.3.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.3.2.rst` & `pytest-8.1.1/doc/en/announce/release-5.3.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.3.3.rst` & `pytest-8.1.1/doc/en/announce/release-5.3.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-5.4.0.rst` & `pytest-8.1.1/doc/en/announce/release-5.4.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-6.0.0.rst` & `pytest-8.1.1/doc/en/announce/release-6.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-6.0.0rc1.rst` & `pytest-8.1.1/doc/en/announce/release-6.0.0rc1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-6.1.0.rst` & `pytest-8.1.1/doc/en/announce/release-6.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-6.2.0.rst` & `pytest-8.1.1/doc/en/announce/release-6.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-6.2.5.rst` & `pytest-8.1.1/doc/en/announce/release-6.2.5.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-7.0.0.rst` & `pytest-8.1.1/doc/en/announce/release-7.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-7.0.0rc1.rst` & `pytest-8.1.1/doc/en/announce/release-7.0.0rc1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-7.1.0.rst` & `pytest-8.1.1/doc/en/announce/release-7.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-7.1.3.rst` & `pytest-8.1.1/doc/en/announce/release-7.1.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-7.2.0.rst` & `pytest-8.1.1/doc/en/announce/release-7.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-7.2.1.rst` & `pytest-8.1.1/doc/en/announce/release-7.2.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-7.3.0.rst` & `pytest-8.1.1/doc/en/announce/release-7.3.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-7.4.0.rst` & `pytest-8.1.1/doc/en/announce/release-7.4.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-8.0.0.rst` & `pytest-8.1.1/doc/en/announce/release-8.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-8.0.0rc1.rst` & `pytest-8.1.1/doc/en/announce/release-8.0.0rc1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-8.0.0rc2.rst` & `pytest-8.1.1/doc/en/announce/release-8.0.0rc2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/release-8.1.0.rst` & `pytest-8.1.1/doc/en/announce/release-8.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/announce/sprint2016.rst` & `pytest-8.1.1/doc/en/announce/sprint2016.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/backwards-compatibility.rst` & `pytest-8.1.1/doc/en/backwards-compatibility.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/builtin.rst` & `pytest-8.1.1/doc/en/builtin.rst`

 * *Files 1% similar despite different names*

```diff
@@ -166,18 +166,18 @@
 
         .. warning::
 
             Currently this fixture **does not work** with the
             `pytest-xdist <https://github.com/pytest-dev/pytest-xdist>`__ plugin. See
             :issue:`7767` for details.
 
-    tmpdir_factory [session scope] -- .../_pytest/legacypath.py:317
+    tmpdir_factory [session scope] -- .../_pytest/legacypath.py:303
         Return a :class:`pytest.TempdirFactory` instance for the test session.
 
-    tmpdir -- .../_pytest/legacypath.py:324
+    tmpdir -- .../_pytest/legacypath.py:310
         Return a temporary directory path object which is unique to each test
         function invocation, created as a sub directory of the base temporary
         directory.
 
         By default, a new base temporary directory is created each test session,
         and old bases are removed after 3 sessions, to aid in debugging. If
         ``--basetemp`` is used then it is cleared each session. See
```

### Comparing `pytest-8.1.0/doc/en/changelog.rst` & `pytest-8.1.1/doc/en/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,22 @@
     .. The 'changelog_towncrier_draft' tag is included by our 'tox -e docs',
        but not on readthedocs.
 
     .. include:: _changelog_towncrier_draft.rst
 
 .. towncrier release notes start
 
-pytest 8.1.0 (2024-03-03)
+pytest 8.1.1 (2024-03-08)
 =========================
 
+.. note::
+
+       This release is not a usual bug fix release -- it contains features and improvements, being a follow up
+       to ``8.1.0``, which has been yanked from PyPI.
+
 Features
 --------
 
 - `#11475 <https://github.com/pytest-dev/pytest/issues/11475>`_: Added the new :confval:`consider_namespace_packages` configuration option, defaulting to ``False``.
 
   If set to ``True``, pytest will attempt to identify modules that are part of `namespace packages <https://packaging.python.org/en/latest/guides/packaging-namespace-packages>`__ when importing modules.
 
@@ -82,29 +87,31 @@
   Previously, only the first exception was reported.
 
 
 
 Bug Fixes
 ---------
 
+- `#11475 <https://github.com/pytest-dev/pytest/issues/11475>`_: Fixed regression where ``--importmode=importlib`` would import non-test modules more than once.
+
+
 - `#11904 <https://github.com/pytest-dev/pytest/issues/11904>`_: Fixed a regression in pytest 8.0.0 that would cause test collection to fail due to permission errors when using ``--pyargs``.
 
   This change improves the collection tree for tests specified using ``--pyargs``, see :pull:`12043` for a comparison with pytest 8.0 and <8.
 
 
 - `#12011 <https://github.com/pytest-dev/pytest/issues/12011>`_: Fixed a regression in 8.0.1 whereby ``setup_module`` xunit-style fixtures are not executed when ``--doctest-modules`` is passed.
 
 
 - `#12014 <https://github.com/pytest-dev/pytest/issues/12014>`_: Fix the ``stacklevel`` used when warning about marks used on fixtures.
 
 
 - `#12039 <https://github.com/pytest-dev/pytest/issues/12039>`_: Fixed a regression in ``8.0.2`` where tests created using :fixture:`tmp_path` have been collected multiple times in CI under Windows.
 
 
-
 Improved Documentation
 ----------------------
 
 - `#11790 <https://github.com/pytest-dev/pytest/issues/11790>`_: Documented the retention of temporary directories created using the ``tmp_path`` fixture in more detail.
 
 
 
@@ -116,14 +123,36 @@
   - ``FixtureManager._getautousenames()`` now takes a ``Node`` itself instead of the nodeid.
   - ``FixtureManager.getfixturedefs()`` now takes the ``Node`` itself instead of the nodeid.
   - The ``_pytest.nodes.iterparentnodeids()`` function is removed without replacement.
     Prefer to traverse the node hierarchy itself instead.
     If you really need to, copy the function from the previous pytest release.
 
 
+- `#12069 <https://github.com/pytest-dev/pytest/issues/12069>`_: Delayed the deprecation of the following features to ``9.0.0``:
+
+  * :ref:`node-ctor-fspath-deprecation`.
+  * :ref:`legacy-path-hooks-deprecated`.
+
+  It was discovered after ``8.1.0`` was released that the warnings about the impeding removal were not being displayed, so the team decided to revert the removal.
+
+  This is the reason for ``8.1.0`` being yanked.
+
+
+pytest 8.1.0 (YANKED)
+=====================
+
+
+.. note::
+
+       This release has been **yanked**: it broke some plugins without the proper warning period, due to
+       some warnings not showing up as expected.
+
+       See `#12069 <https://github.com/pytest-dev/pytest/issues/12069>`__.
+
+
 pytest 8.0.2 (2024-02-24)
 =========================
 
 Bug Fixes
 ---------
 
 - `#11895 <https://github.com/pytest-dev/pytest/issues/11895>`_: Fix collection on Windows where initial paths contain the short version of a path (for example ``c:\PROGRA~1\tests``).
```

### Comparing `pytest-8.1.0/doc/en/conf.py` & `pytest-8.1.1/doc/en/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,15 @@
     ("py:class", "_pytest.python_api.RaisesContext"),
     ("py:class", "_pytest.recwarn.WarningsChecker"),
     ("py:class", "_pytest.reports.BaseReport"),
     # Undocumented third parties
     ("py:class", "_tracing.TagTracerSub"),
     ("py:class", "warnings.WarningMessage"),
     # Undocumented type aliases
+    ("py:class", "LEGACY_PATH"),
     ("py:class", "_PluggyPlugin"),
     # TypeVars
     ("py:class", "_pytest._code.code.E"),
     ("py:class", "_pytest.fixtures.FixtureFunction"),
     ("py:class", "_pytest.nodes._NodeType"),
     ("py:class", "_pytest.python_api.E"),
     ("py:class", "_pytest.recwarn.T"),
```

### Comparing `pytest-8.1.0/doc/en/contact.rst` & `pytest-8.1.1/doc/en/contact.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/contents.rst` & `pytest-8.1.1/doc/en/contents.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/deprecations.rst` & `pytest-8.1.1/doc/en/deprecations.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,53 @@
 Deprecated Features
 -------------------
 
 Below is a complete list of all pytest features which are considered deprecated. Using those features will issue
 :class:`~pytest.PytestWarning` or subclasses, which can be filtered using :ref:`standard warning filters <warnings>`.
 
 
-.. _legacy-path-hooks-deprecated:
+.. _node-ctor-fspath-deprecation:
+
+``fspath`` argument for Node constructors replaced with ``pathlib.Path``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. deprecated:: 7.0
+
+In order to support the transition from ``py.path.local`` to :mod:`pathlib`,
+the ``fspath`` argument to :class:`~_pytest.nodes.Node` constructors like
+:func:`pytest.Function.from_parent()` and :func:`pytest.Class.from_parent()`
+is now deprecated.
+
+Plugins which construct nodes should pass the ``path`` argument, of type
+:class:`pathlib.Path`, instead of the ``fspath`` argument.
+
+Plugins which implement custom items and collectors are encouraged to replace
+``fspath`` parameters (``py.path.local``) with ``path`` parameters
+(``pathlib.Path``), and drop any other usage of the ``py`` library if possible.
+
+If possible, plugins with custom items should use :ref:`cooperative
+constructors <uncooperative-constructors-deprecated>` to avoid hardcoding
+arguments they only pass on to the superclass.
+
+.. note::
+    The name of the :class:`~_pytest.nodes.Node` arguments and attributes (the
+    new attribute being ``path``) is **the opposite** of the situation for
+    hooks, :ref:`outlined below <legacy-path-hooks-deprecated>` (the old
+    argument being ``path``).
+
+    This is an unfortunate artifact due to historical reasons, which should be
+    resolved in future versions as we slowly get rid of the :pypi:`py`
+    dependency (see :issue:`9283` for a longer discussion).
+
+Due to the ongoing migration of methods like :meth:`~pytest.Item.reportinfo`
+which still is expected to return a ``py.path.local`` object, nodes still have
+both ``fspath`` (``py.path.local``) and ``path`` (``pathlib.Path``) attributes,
+no matter what argument was used in the constructor. We expect to deprecate the
+``fspath`` attribute in a future release.
+
 
 Configuring hook specs/impls using markers
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Before pluggy, pytest's plugin library, was its own package and had a clear API,
 pytest just used ``pytest.mark`` to configure hooks.
 
@@ -58,14 +96,41 @@
 
 Changed ``hookwrapper`` attributes:
 
 * ``firstresult``
 * ``historic``
 
 
+.. _legacy-path-hooks-deprecated:
+
+``py.path.local`` arguments for hooks replaced with ``pathlib.Path``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. deprecated:: 7.0
+
+In order to support the transition from ``py.path.local`` to :mod:`pathlib`, the following hooks now receive additional arguments:
+
+*  :hook:`pytest_ignore_collect(collection_path: pathlib.Path) <pytest_ignore_collect>` as equivalent to ``path``
+*  :hook:`pytest_collect_file(file_path: pathlib.Path) <pytest_collect_file>` as equivalent to ``path``
+*  :hook:`pytest_pycollect_makemodule(module_path: pathlib.Path) <pytest_pycollect_makemodule>` as equivalent to ``path``
+*  :hook:`pytest_report_header(start_path: pathlib.Path) <pytest_report_header>` as equivalent to ``startdir``
+*  :hook:`pytest_report_collectionfinish(start_path: pathlib.Path) <pytest_report_collectionfinish>` as equivalent to ``startdir``
+
+The accompanying ``py.path.local`` based paths have been deprecated: plugins which manually invoke those hooks should only pass the new ``pathlib.Path`` arguments, and users should change their hook implementations to use the new ``pathlib.Path`` arguments.
+
+.. note::
+    The name of the :class:`~_pytest.nodes.Node` arguments and attributes,
+    :ref:`outlined above <node-ctor-fspath-deprecation>` (the new attribute
+    being ``path``) is **the opposite** of the situation for hooks (the old
+    argument being ``path``).
+
+    This is an unfortunate artifact due to historical reasons, which should be
+    resolved in future versions as we slowly get rid of the :pypi:`py`
+    dependency (see :issue:`9283` for a longer discussion).
+
 Directly constructing internal classes
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. deprecated:: 7.0
 
 Directly constructing the following classes is now deprecated:
 
@@ -204,81 +269,14 @@
 -------------------------------------
 
 As stated in our :ref:`backwards-compatibility` policy, deprecated features are removed only in major releases after
 an appropriate period of deprecation has passed.
 
 Some breaking changes which could not be deprecated are also listed.
 
-.. _node-ctor-fspath-deprecation:
-
-``fspath`` argument for Node constructors replaced with ``pathlib.Path``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-.. deprecated:: 7.0
-
-In order to support the transition from ``py.path.local`` to :mod:`pathlib`,
-the ``fspath`` argument to :class:`~_pytest.nodes.Node` constructors like
-:func:`pytest.Function.from_parent()` and :func:`pytest.Class.from_parent()`
-is now deprecated.
-
-Plugins which construct nodes should pass the ``path`` argument, of type
-:class:`pathlib.Path`, instead of the ``fspath`` argument.
-
-Plugins which implement custom items and collectors are encouraged to replace
-``fspath`` parameters (``py.path.local``) with ``path`` parameters
-(``pathlib.Path``), and drop any other usage of the ``py`` library if possible.
-
-If possible, plugins with custom items should use :ref:`cooperative
-constructors <uncooperative-constructors-deprecated>` to avoid hardcoding
-arguments they only pass on to the superclass.
-
-.. note::
-    The name of the :class:`~_pytest.nodes.Node` arguments and attributes (the
-    new attribute being ``path``) is **the opposite** of the situation for
-    hooks, :ref:`outlined below <legacy-path-hooks-deprecated>` (the old
-    argument being ``path``).
-
-    This is an unfortunate artifact due to historical reasons, which should be
-    resolved in future versions as we slowly get rid of the :pypi:`py`
-    dependency (see :issue:`9283` for a longer discussion).
-
-Due to the ongoing migration of methods like :meth:`~pytest.Item.reportinfo`
-which still is expected to return a ``py.path.local`` object, nodes still have
-both ``fspath`` (``py.path.local``) and ``path`` (``pathlib.Path``) attributes,
-no matter what argument was used in the constructor. We expect to deprecate the
-``fspath`` attribute in a future release.
-
-
-``py.path.local`` arguments for hooks replaced with ``pathlib.Path``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-.. deprecated:: 7.0
-.. versionremoved:: 8.0
-
-In order to support the transition from ``py.path.local`` to :mod:`pathlib`, the following hooks now receive additional arguments:
-
-*  :hook:`pytest_ignore_collect(collection_path: pathlib.Path) <pytest_ignore_collect>` as equivalent to ``path``
-*  :hook:`pytest_collect_file(file_path: pathlib.Path) <pytest_collect_file>` as equivalent to ``path``
-*  :hook:`pytest_pycollect_makemodule(module_path: pathlib.Path) <pytest_pycollect_makemodule>` as equivalent to ``path``
-*  :hook:`pytest_report_header(start_path: pathlib.Path) <pytest_report_header>` as equivalent to ``startdir``
-*  :hook:`pytest_report_collectionfinish(start_path: pathlib.Path) <pytest_report_collectionfinish>` as equivalent to ``startdir``
-
-The accompanying ``py.path.local`` based paths have been deprecated: plugins which manually invoke those hooks should only pass the new ``pathlib.Path`` arguments, and users should change their hook implementations to use the new ``pathlib.Path`` arguments.
-
-.. note::
-    The name of the :class:`~_pytest.nodes.Node` arguments and attributes,
-    :ref:`outlined above <node-ctor-fspath-deprecation>` (the new attribute
-    being ``path``) is **the opposite** of the situation for hooks (the old
-    argument being ``path``).
-
-    This is an unfortunate artifact due to historical reasons, which should be
-    resolved in future versions as we slowly get rid of the :pypi:`py`
-    dependency (see :issue:`9283` for a longer discussion).
-
-
 .. _nose-deprecation:
 
 Support for tests written for nose
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. deprecated:: 7.2
 .. versionremoved:: 8.0
```

### Comparing `pytest-8.1.0/doc/en/example/assertion/failure_demo.py` & `pytest-8.1.1/doc/en/example/assertion/failure_demo.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/assertion/test_setup_flow_example.py` & `pytest-8.1.1/doc/en/example/assertion/test_setup_flow_example.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/attic.rst` & `pytest-8.1.1/doc/en/example/attic.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/customdirectory/conftest.py` & `pytest-8.1.1/doc/en/example/customdirectory/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/customdirectory.rst` & `pytest-8.1.1/doc/en/example/customdirectory.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/fixture_availability.svg` & `pytest-8.1.1/doc/en/example/fixtures/fixture_availability.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/fixture_availability_plugins.svg` & `pytest-8.1.1/doc/en/example/fixtures/fixture_availability_plugins.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse.py` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse.svg` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse_flat.svg` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_flat.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.py` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.svg` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.py` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.svg` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_dependencies.py` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_dependencies.svg` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_dependencies_flat.svg` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies_flat.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_dependencies_unclear.svg` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies_unclear.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_scope.py` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_scope.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_order_scope.svg` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_scope.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/fixtures/test_fixtures_request_different_scope.svg` & `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_request_different_scope.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/index.rst` & `pytest-8.1.1/doc/en/example/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/markers.rst` & `pytest-8.1.1/doc/en/example/markers.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/multipython.py` & `pytest-8.1.1/doc/en/example/multipython.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/nonpython/conftest.py` & `pytest-8.1.1/doc/en/example/nonpython/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/nonpython.rst` & `pytest-8.1.1/doc/en/example/nonpython.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/parametrize.rst` & `pytest-8.1.1/doc/en/example/parametrize.rst`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
     $ pytest test_time.py --collect-only
     =========================== test session starts ============================
     platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
     rootdir: /home/sweet/project
     collected 8 items
 
-    <Dir parametrize.rst-195>
+    <Dir parametrize.rst-196>
       <Module test_time.py>
         <Function test_timedistance_v0[a0-b0-expected0]>
         <Function test_timedistance_v0[a1-b1-expected1]>
         <Function test_timedistance_v1[forward]>
         <Function test_timedistance_v1[backward]>
         <Function test_timedistance_v2[20011212-20011211-expected0]>
         <Function test_timedistance_v2[20011211-20011212-expected1]>
@@ -235,15 +235,15 @@
 
     $ pytest --collect-only test_scenarios.py
     =========================== test session starts ============================
     platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
     rootdir: /home/sweet/project
     collected 4 items
 
-    <Dir parametrize.rst-195>
+    <Dir parametrize.rst-196>
       <Module test_scenarios.py>
         <Class TestSampleWithScenarios>
           <Function test_demo1[basic]>
           <Function test_demo2[basic]>
           <Function test_demo1[advanced]>
           <Function test_demo2[advanced]>
 
@@ -314,15 +314,15 @@
 
     $ pytest test_backends.py --collect-only
     =========================== test session starts ============================
     platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
     rootdir: /home/sweet/project
     collected 2 items
 
-    <Dir parametrize.rst-195>
+    <Dir parametrize.rst-196>
       <Module test_backends.py>
         <Function test_db_initialized[d1]>
         <Function test_db_initialized[d2]>
 
     ======================== 2 tests collected in 0.12s ========================
 
 And then when we run the test:
```

### Comparing `pytest-8.1.0/doc/en/example/pythoncollection.rst` & `pytest-8.1.1/doc/en/example/pythoncollection.rst`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     $ pytest --collect-only
     =========================== test session starts ============================
     platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
     rootdir: /home/sweet/project
     configfile: pytest.ini
     collected 2 items
 
-    <Dir pythoncollection.rst-196>
+    <Dir pythoncollection.rst-197>
       <Module check_myapp.py>
         <Class CheckMyApp>
           <Function simple_check>
           <Function complex_check>
 
     ======================== 2 tests collected in 0.12s ========================
 
@@ -211,15 +211,15 @@
     . $ pytest --collect-only pythoncollection.py
     =========================== test session starts ============================
     platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
     rootdir: /home/sweet/project
     configfile: pytest.ini
     collected 3 items
 
-    <Dir pythoncollection.rst-196>
+    <Dir pythoncollection.rst-197>
       <Dir CWD>
         <Module pythoncollection.py>
           <Function test_function>
           <Class TestClass>
             <Function test_method>
             <Function test_anothermethod>
```

### Comparing `pytest-8.1.0/doc/en/example/reportingdemo.rst` & `pytest-8.1.1/doc/en/example/reportingdemo.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/simple.rst` & `pytest-8.1.1/doc/en/example/simple.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/example/special.rst` & `pytest-8.1.1/doc/en/example/special.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/explanation/anatomy.rst` & `pytest-8.1.1/doc/en/explanation/anatomy.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/explanation/fixtures.rst` & `pytest-8.1.1/doc/en/explanation/fixtures.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/explanation/flaky.rst` & `pytest-8.1.1/doc/en/explanation/flaky.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/explanation/goodpractices.rst` & `pytest-8.1.1/doc/en/explanation/goodpractices.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/explanation/pythonpath.rst` & `pytest-8.1.1/doc/en/explanation/pythonpath.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/funcarg_compare.rst` & `pytest-8.1.1/doc/en/funcarg_compare.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/getting-started.rst` & `pytest-8.1.1/doc/en/getting-started.rst`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     pip install -U pytest
 
 2. Check that you installed the correct version:
 
 .. code-block:: bash
 
     $ pytest --version
-    pytest 8.1.0
+    pytest 8.1.1
 
 .. _`simpletest`:
 
 Create your first test
 ----------------------------------------------------------
 
 Create a new file called ``test_sample.py``, containing a function, and a test:
```

### Comparing `pytest-8.1.0/doc/en/historical-notes.rst` & `pytest-8.1.1/doc/en/historical-notes.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/history.rst` & `pytest-8.1.1/doc/en/history.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/assert.rst` & `pytest-8.1.1/doc/en/how-to/assert.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/bash-completion.rst` & `pytest-8.1.1/doc/en/how-to/bash-completion.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/cache.rst` & `pytest-8.1.1/doc/en/how-to/cache.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/capture-stdout-stderr.rst` & `pytest-8.1.1/doc/en/how-to/capture-stdout-stderr.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/capture-warnings.rst` & `pytest-8.1.1/doc/en/how-to/capture-warnings.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/doctest.rst` & `pytest-8.1.1/doc/en/how-to/doctest.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/existingtestsuite.rst` & `pytest-8.1.1/doc/en/how-to/existingtestsuite.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/failures.rst` & `pytest-8.1.1/doc/en/how-to/failures.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/fixtures.rst` & `pytest-8.1.1/doc/en/how-to/fixtures.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1414,15 +1414,15 @@
 
    $ pytest --collect-only
    =========================== test session starts ============================
    platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
    rootdir: /home/sweet/project
    collected 12 items
 
-   <Dir fixtures.rst-214>
+   <Dir fixtures.rst-215>
      <Module test_anothersmtp.py>
        <Function test_showhelo[smtp.gmail.com]>
        <Function test_showhelo[mail.python.org]>
      <Module test_emaillib.py>
        <Function test_email_received>
      <Module test_finalizers.py>
        <Function test_bar>
```

### Comparing `pytest-8.1.0/doc/en/how-to/index.rst` & `pytest-8.1.1/doc/en/how-to/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/logging.rst` & `pytest-8.1.1/doc/en/how-to/logging.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/mark.rst` & `pytest-8.1.1/doc/en/how-to/mark.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/monkeypatch.rst` & `pytest-8.1.1/doc/en/how-to/monkeypatch.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/output.rst` & `pytest-8.1.1/doc/en/how-to/output.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/parametrize.rst` & `pytest-8.1.1/doc/en/how-to/parametrize.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/plugins.rst` & `pytest-8.1.1/doc/en/how-to/plugins.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/skipping.rst` & `pytest-8.1.1/doc/en/how-to/skipping.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/tmp_path.rst` & `pytest-8.1.1/doc/en/how-to/tmp_path.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/unittest.rst` & `pytest-8.1.1/doc/en/how-to/unittest.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/usage.rst` & `pytest-8.1.1/doc/en/how-to/usage.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/writing_hook_functions.rst` & `pytest-8.1.1/doc/en/how-to/writing_hook_functions.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/writing_plugins.rst` & `pytest-8.1.1/doc/en/how-to/writing_plugins.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/how-to/xunit_setup.rst` & `pytest-8.1.1/doc/en/how-to/xunit_setup.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/img/cramer2.png` & `pytest-8.1.1/doc/en/img/cramer2.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/img/favicon.png` & `pytest-8.1.1/doc/en/img/favicon.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/img/freiburg2.jpg` & `pytest-8.1.1/doc/en/img/freiburg2.jpg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/img/gaynor3.png` & `pytest-8.1.1/doc/en/img/gaynor3.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/img/keleshev.png` & `pytest-8.1.1/doc/en/img/keleshev.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/img/pullrequest.png` & `pytest-8.1.1/doc/en/img/pullrequest.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/img/pylib.png` & `pytest-8.1.1/doc/en/img/pylib.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/img/pytest1.png` & `pytest-8.1.1/doc/en/img/pytest1.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/img/pytest_logo_curves.svg` & `pytest-8.1.1/doc/en/img/pytest_logo_curves.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/img/theuni.png` & `pytest-8.1.1/doc/en/img/theuni.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/index.rst` & `pytest-8.1.1/doc/en/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/license.rst` & `pytest-8.1.1/doc/en/license.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/naming20.rst` & `pytest-8.1.1/doc/en/naming20.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/proposals/parametrize_with_fixtures.rst` & `pytest-8.1.1/doc/en/proposals/parametrize_with_fixtures.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/reference/customize.rst` & `pytest-8.1.1/doc/en/reference/customize.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/reference/exit-codes.rst` & `pytest-8.1.1/doc/en/reference/exit-codes.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/reference/fixtures.rst` & `pytest-8.1.1/doc/en/reference/fixtures.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/reference/plugin_list.rst` & `pytest-8.1.1/doc/en/reference/plugin_list.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/reference/reference.rst` & `pytest-8.1.1/doc/en/reference/reference.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/sponsor.rst` & `pytest-8.1.1/doc/en/sponsor.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/talks.rst` & `pytest-8.1.1/doc/en/talks.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/doc/en/tidelift.rst` & `pytest-8.1.1/doc/en/tidelift.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/extra/get_issues.py` & `pytest-8.1.1/extra/get_issues.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/pyproject.toml` & `pytest-8.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/scripts/generate-gh-release-notes.py` & `pytest-8.1.1/scripts/generate-gh-release-notes.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/scripts/prepare-release-pr.py` & `pytest-8.1.1/scripts/prepare-release-pr.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/scripts/release.major.rst` & `pytest-8.1.1/scripts/release.major.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/scripts/release.minor.rst` & `pytest-8.1.1/scripts/release.minor.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/scripts/release.pre.rst` & `pytest-8.1.1/scripts/release.pre.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/scripts/release.py` & `pytest-8.1.1/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/scripts/update-plugin-list.py` & `pytest-8.1.1/scripts/update-plugin-list.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/_argcomplete.py` & `pytest-8.1.1/src/_pytest/_argcomplete.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/_code/code.py` & `pytest-8.1.1/src/_pytest/_code/code.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/_code/source.py` & `pytest-8.1.1/src/_pytest/_code/source.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/_io/pprint.py` & `pytest-8.1.1/src/_pytest/_io/pprint.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/_io/saferepr.py` & `pytest-8.1.1/src/_pytest/_io/saferepr.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/_io/terminalwriter.py` & `pytest-8.1.1/src/_pytest/_io/terminalwriter.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/_io/wcwidth.py` & `pytest-8.1.1/src/_pytest/_io/wcwidth.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/_py/error.py` & `pytest-8.1.1/src/_pytest/_py/error.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/_py/path.py` & `pytest-8.1.1/src/_pytest/_py/path.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/assertion/__init__.py` & `pytest-8.1.1/src/_pytest/assertion/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/assertion/rewrite.py` & `pytest-8.1.1/src/_pytest/assertion/rewrite.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/assertion/truncate.py` & `pytest-8.1.1/src/_pytest/assertion/truncate.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/assertion/util.py` & `pytest-8.1.1/src/_pytest/assertion/util.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/cacheprovider.py` & `pytest-8.1.1/src/_pytest/cacheprovider.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/capture.py` & `pytest-8.1.1/src/_pytest/capture.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/compat.py` & `pytest-8.1.1/src/_pytest/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # mypy: allow-untyped-defs
 """Python version compatibility code."""
+
 from __future__ import annotations
 
 import dataclasses
 import enum
 import functools
 import inspect
 from inspect import Parameter
@@ -12,14 +13,30 @@
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
 from typing import Final
 from typing import NoReturn
 
+import py
+
+
+#: constant to prepare valuing pylib path replacements/lazy proxies later on
+#  intended for removal in pytest 8.0 or 9.0
+
+# fmt: off
+# intentional space to create a fake difference for the verification
+LEGACY_PATH = py.path. local
+# fmt: on
+
+
+def legacy_path(path: str | os.PathLike[str]) -> LEGACY_PATH:
+    """Internal wrapper to prepare lazy proxies for legacy_path instances"""
+    return LEGACY_PATH(path)
+
 
 # fmt: off
 # Singleton type for NOTSET, as described in:
 # https://www.python.org/dev/peps/pep-0484/#support-for-singleton-types-in-unions
 class NotSetType(enum.Enum):
     token = 0
 NOTSET: Final = NotSetType.token
```

### Comparing `pytest-8.1.0/src/_pytest/config/__init__.py` & `pytest-8.1.1/src/_pytest/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,20 +34,22 @@
 from typing import TextIO
 from typing import Tuple
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import Union
 import warnings
 
+import pluggy
 from pluggy import HookimplMarker
 from pluggy import HookimplOpts
 from pluggy import HookspecMarker
 from pluggy import HookspecOpts
 from pluggy import PluginManager
 
+from .compat import PathAwareHookProxy
 from .exceptions import PrintHelp as PrintHelp
 from .exceptions import UsageError as UsageError
 from .findpaths import determine_setup
 import _pytest._code
 from _pytest._code import ExceptionInfo
 from _pytest._code import filter_traceback
 from _pytest._io import TerminalWriter
@@ -1064,15 +1066,15 @@
 
         :type: Stash
         """
         # Deprecated alias. Was never public. Can be removed in a few releases.
         self._store = self.stash
 
         self.trace = self.pluginmanager.trace.root.get("config")
-        self.hook = self.pluginmanager.hook  # type: ignore[assignment]
+        self.hook: pluggy.HookRelay = PathAwareHookProxy(self.pluginmanager.hook)  # type: ignore[assignment]
         self._inicache: Dict[str, Any] = {}
         self._override_ini: Sequence[str] = ()
         self._opt2dest: Dict[str, str] = {}
         self._cleanup: List[Callable[[], None]] = []
         self.pluginmanager.register(self, "pytestconfig")
         self._configured = False
         self.hook.pytest_addoption.call_historic(
```

### Comparing `pytest-8.1.0/src/_pytest/config/argparsing.py` & `pytest-8.1.1/src/_pytest/config/argparsing.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/config/findpaths.py` & `pytest-8.1.1/src/_pytest/config/findpaths.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/debugging.py` & `pytest-8.1.1/src/_pytest/debugging.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/deprecated.py` & `pytest-8.1.1/src/_pytest/deprecated.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,14 +32,29 @@
     "Use @pytest.fixture instead; they are the same."
 )
 
 # This deprecation is never really meant to be removed.
 PRIVATE = PytestDeprecationWarning("A private pytest class or function was used.")
 
 
+HOOK_LEGACY_PATH_ARG = UnformattedWarning(
+    PytestRemovedIn9Warning,
+    "The ({pylib_path_arg}: py.path.local) argument is deprecated, please use ({pathlib_path_arg}: pathlib.Path)\n"
+    "see https://docs.pytest.org/en/latest/deprecations.html"
+    "#py-path-local-arguments-for-hooks-replaced-with-pathlib-path",
+)
+
+NODE_CTOR_FSPATH_ARG = UnformattedWarning(
+    PytestRemovedIn9Warning,
+    "The (fspath: py.path.local) argument to {node_type_name} is deprecated. "
+    "Please use the (path: pathlib.Path) argument instead.\n"
+    "See https://docs.pytest.org/en/latest/deprecations.html"
+    "#fspath-argument-for-node-constructors-replaced-with-pathlib-path",
+)
+
 HOOK_LEGACY_MARKING = UnformattedWarning(
     PytestDeprecationWarning,
     "The hook{type} {fullname} uses old-style configuration options (marks or attributes).\n"
     "Please use the pytest.hook{type}({hook_opts}) decorator instead\n"
     " to configure the hooks.\n"
     " See https://docs.pytest.org/en/latest/deprecations.html"
     "#configuring-hook-specs-impls-using-markers",
```

### Comparing `pytest-8.1.0/src/_pytest/doctest.py` & `pytest-8.1.1/src/_pytest/doctest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/faulthandler.py` & `pytest-8.1.1/src/_pytest/faulthandler.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/fixtures.py` & `pytest-8.1.1/src/_pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/freeze_support.py` & `pytest-8.1.1/src/_pytest/freeze_support.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/helpconfig.py` & `pytest-8.1.1/src/_pytest/helpconfig.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/hookspec.py` & `pytest-8.1.1/src/_pytest/hookspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 if TYPE_CHECKING:
     import pdb
     from typing import Literal
     import warnings
 
     from _pytest._code.code import ExceptionInfo
     from _pytest._code.code import ExceptionRepr
+    from _pytest.compat import LEGACY_PATH
     from _pytest.config import _PluggyPlugin
     from _pytest.config import Config
     from _pytest.config import ExitCode
     from _pytest.config import PytestPluginManager
     from _pytest.config.argparsing import Parser
     from _pytest.fixtures import FixtureDef
     from _pytest.fixtures import SubRequest
@@ -292,32 +293,32 @@
     =======================
 
     Any conftest plugin can implement this hook.
     """
 
 
 @hookspec(firstresult=True)
-def pytest_ignore_collect(collection_path: Path, config: "Config") -> Optional[bool]:
+def pytest_ignore_collect(
+    collection_path: Path, path: "LEGACY_PATH", config: "Config"
+) -> Optional[bool]:
     """Return True to prevent considering this path for collection.
 
     This hook is consulted for all files and directories prior to calling
     more specific hooks.
 
     Stops at first non-None result, see :ref:`firstresult`.
 
     :param collection_path: The path to analyze.
     :param path: The path to analyze (deprecated).
     :param config: The pytest config object.
 
     .. versionchanged:: 7.0.0
         The ``collection_path`` parameter was added as a :class:`pathlib.Path`
-        equivalent of the ``path`` parameter.
-
-    .. versionchanged:: 8.0.0
-        The ``path`` parameter has been removed.
+        equivalent of the ``path`` parameter. The ``path`` parameter
+        has been deprecated.
 
     Use in conftest plugins
     =======================
 
     Any conftest file can implement this hook. For a given collection path, only
     conftest files in parent directories of the collection path are consulted
     (if the path is a directory, its own conftest file is *not* consulted - a
@@ -350,31 +351,31 @@
     Any conftest file can implement this hook. For a given collection path, only
     conftest files in parent directories of the collection path are consulted
     (if the path is a directory, its own conftest file is *not* consulted - a
     directory cannot collect itself!).
     """
 
 
-def pytest_collect_file(file_path: Path, parent: "Collector") -> "Optional[Collector]":
+def pytest_collect_file(
+    file_path: Path, path: "LEGACY_PATH", parent: "Collector"
+) -> "Optional[Collector]":
     """Create a :class:`~pytest.Collector` for the given path, or None if not relevant.
 
     For best results, the returned collector should be a subclass of
     :class:`~pytest.File`, but this is not required.
 
     The new node needs to have the specified ``parent`` as a parent.
 
     :param file_path: The path to analyze.
     :param path: The path to collect (deprecated).
 
     .. versionchanged:: 7.0.0
         The ``file_path`` parameter was added as a :class:`pathlib.Path`
-        equivalent of the ``path`` parameter.
-
-    .. versionchanged:: 8.0.0
-        The ``path`` parameter was removed.
+        equivalent of the ``path`` parameter. The ``path`` parameter
+        has been deprecated.
 
     Use in conftest plugins
     =======================
 
     Any conftest file can implement this hook. For a given file path, only
     conftest files in parent directories of the file path are consulted.
     """
@@ -463,15 +464,17 @@
 
 # -------------------------------------------------------------------------
 # Python test function related hooks
 # -------------------------------------------------------------------------
 
 
 @hookspec(firstresult=True)
-def pytest_pycollect_makemodule(module_path: Path, parent) -> Optional["Module"]:
+def pytest_pycollect_makemodule(
+    module_path: Path, path: "LEGACY_PATH", parent
+) -> Optional["Module"]:
     """Return a :class:`pytest.Module` collector or None for the given path.
 
     This hook will be called for each matching test module path.
     The :hook:`pytest_collect_file` hook needs to be used if you want to
     create test modules for files that do not match as a test module.
 
     Stops at first non-None result, see :ref:`firstresult`.
@@ -479,16 +482,15 @@
     :param module_path: The path of the module to collect.
     :param path: The path of the module to collect (deprecated).
 
     .. versionchanged:: 7.0.0
         The ``module_path`` parameter was added as a :class:`pathlib.Path`
         equivalent of the ``path`` parameter.
 
-    .. versionchanged:: 8.0.0
-        The ``path`` parameter has been removed in favor of ``module_path``.
+        The ``path`` parameter has been deprecated in favor of ``fspath``.
 
     Use in conftest plugins
     =======================
 
     Any conftest file can implement this hook. For a given parent collector,
     only conftest files in the collector's directory and its parent directories
     are consulted.
@@ -988,15 +990,15 @@
 
 # -------------------------------------------------------------------------
 # Hooks for influencing reporting (invoked from _pytest_terminal).
 # -------------------------------------------------------------------------
 
 
 def pytest_report_header(  # type:ignore[empty-body]
-    config: "Config", start_path: Path
+    config: "Config", start_path: Path, startdir: "LEGACY_PATH"
 ) -> Union[str, List[str]]:
     """Return a string or list of strings to be displayed as header info for terminal reporting.
 
     :param config: The pytest config object.
     :param start_path: The starting dir.
     :param startdir: The starting dir (deprecated).
 
@@ -1005,29 +1007,28 @@
         Lines returned by a plugin are displayed before those of plugins which
         ran before it.
         If you want to have your line(s) displayed first, use
         :ref:`trylast=True <plugin-hookorder>`.
 
     .. versionchanged:: 7.0.0
         The ``start_path`` parameter was added as a :class:`pathlib.Path`
-        equivalent of the ``startdir`` parameter.
-
-    .. versionchanged:: 8.0.0
-        The ``startdir`` parameter has been removed.
+        equivalent of the ``startdir`` parameter. The ``startdir`` parameter
+        has been deprecated.
 
     Use in conftest plugins
     =======================
 
     This hook is only called for :ref:`initial conftests <pluginorder>`.
     """
 
 
 def pytest_report_collectionfinish(  # type:ignore[empty-body]
     config: "Config",
     start_path: Path,
+    startdir: "LEGACY_PATH",
     items: Sequence["Item"],
 ) -> Union[str, List[str]]:
     """Return a string or list of strings to be displayed after collection
     has finished successfully.
 
     These strings will be displayed after the standard "collected X items" message.
 
@@ -1043,18 +1044,16 @@
         Lines returned by a plugin are displayed before those of plugins which
         ran before it.
         If you want to have your line(s) displayed first, use
         :ref:`trylast=True <plugin-hookorder>`.
 
     .. versionchanged:: 7.0.0
         The ``start_path`` parameter was added as a :class:`pathlib.Path`
-        equivalent of the ``startdir`` parameter.
-
-    .. versionchanged:: 8.0.0
-        The ``startdir`` parameter has been removed.
+        equivalent of the ``startdir`` parameter. The ``startdir`` parameter
+        has been deprecated.
 
     Use in conftest plugins
     =======================
 
     Any conftest plugin can implement this hook.
     """
```

### Comparing `pytest-8.1.0/src/_pytest/junitxml.py` & `pytest-8.1.1/src/_pytest/junitxml.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/legacypath.py` & `pytest-8.1.1/src/_pytest/legacypath.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # mypy: allow-untyped-defs
 """Add backward compatibility support for the legacy py path type."""
+
 import dataclasses
-import os
 from pathlib import Path
 import shlex
 import subprocess
 from typing import Final
 from typing import final
 from typing import List
 from typing import Optional
 from typing import TYPE_CHECKING
 from typing import Union
 
 from iniconfig import SectionWrapper
 
-import py
-
 from _pytest.cacheprovider import Cache
+from _pytest.compat import LEGACY_PATH
+from _pytest.compat import legacy_path
 from _pytest.config import Config
 from _pytest.config import hookimpl
 from _pytest.config import PytestPluginManager
 from _pytest.deprecated import check_ispytest
 from _pytest.fixtures import fixture
 from _pytest.fixtures import FixtureRequest
 from _pytest.main import Session
@@ -35,28 +35,14 @@
 from _pytest.tmpdir import TempPathFactory
 
 
 if TYPE_CHECKING:
     import pexpect
 
 
-#: constant to prepare valuing pylib path replacements/lazy proxies later on
-#  intended for removal in pytest 8.0 or 9.0
-
-# fmt: off
-# intentional space to create a fake difference for the verification
-LEGACY_PATH = py.path. local
-# fmt: on
-
-
-def legacy_path(path: Union[str, "os.PathLike[str]"]) -> LEGACY_PATH:
-    """Internal wrapper to prepare lazy proxies for legacy_path instances"""
-    return LEGACY_PATH(path)
-
-
 @final
 class Testdir:
     """
     Similar to :class:`Pytester`, but this class works with legacy legacy_path objects instead.
 
     All methods just forward to an internal :class:`Pytester` instance, converting results
     to `legacy_path` objects as necessary.
```

### Comparing `pytest-8.1.0/src/_pytest/logging.py` & `pytest-8.1.1/src/_pytest/logging.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/main.py` & `pytest-8.1.1/src/_pytest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from _pytest.config import Config
 from _pytest.config import directory_arg
 from _pytest.config import ExitCode
 from _pytest.config import hookimpl
 from _pytest.config import PytestPluginManager
 from _pytest.config import UsageError
 from _pytest.config.argparsing import Parser
+from _pytest.config.compat import PathAwareHookProxy
 from _pytest.fixtures import FixtureManager
 from _pytest.outcomes import exit
 from _pytest.pathlib import absolutepath
 from _pytest.pathlib import bestrelpath
 from _pytest.pathlib import fnmatch_ex
 from _pytest.pathlib import safe_exists
 from _pytest.pathlib import scandir
@@ -553,14 +554,15 @@
     _fixturemanager: FixtureManager
     exitstatus: Union[int, ExitCode]
 
     def __init__(self, config: Config) -> None:
         super().__init__(
             name="",
             path=config.rootpath,
+            fspath=None,
             parent=None,
             config=config,
             session=self,
             nodeid="",
         )
         self.testsfailed = 0
         self.testscollected = 0
@@ -690,15 +692,15 @@
         # Check if we have the common case of running
         # hooks with all conftest.py files.
         my_conftestmodules = pm._getconftestmodules(path)
         remove_mods = pm._conftest_plugins.difference(my_conftestmodules)
         proxy: pluggy.HookRelay
         if remove_mods:
             # One or more conftests are not in use at this path.
-            proxy = FSHookProxy(pm, remove_mods)  # type: ignore[arg-type,assignment]
+            proxy = PathAwareHookProxy(FSHookProxy(pm, remove_mods))  # type: ignore[arg-type,assignment]
         else:
             # All plugins are active for this fspath.
             proxy = self.config.hook
         return proxy
 
     def _collect_path(
         self,
```

### Comparing `pytest-8.1.0/src/_pytest/mark/__init__.py` & `pytest-8.1.1/src/_pytest/mark/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/mark/expression.py` & `pytest-8.1.1/src/_pytest/mark/expression.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/mark/structures.py` & `pytest-8.1.1/src/_pytest/mark/structures.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/monkeypatch.py` & `pytest-8.1.1/src/_pytest/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/nodes.py` & `pytest-8.1.1/src/_pytest/nodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # mypy: allow-untyped-defs
 import abc
 from functools import cached_property
 from inspect import signature
 import os
+import pathlib
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import cast
 from typing import Iterable
 from typing import Iterator
 from typing import List
@@ -25,16 +26,19 @@
 import pluggy
 
 import _pytest._code
 from _pytest._code import getfslineno
 from _pytest._code.code import ExceptionInfo
 from _pytest._code.code import TerminalRepr
 from _pytest._code.code import Traceback
+from _pytest.compat import LEGACY_PATH
 from _pytest.config import Config
 from _pytest.config import ConftestImportFailure
+from _pytest.config.compat import _check_path
+from _pytest.deprecated import NODE_CTOR_FSPATH_ARG
 from _pytest.mark.structures import Mark
 from _pytest.mark.structures import MarkDecorator
 from _pytest.mark.structures import NodeKeywords
 from _pytest.outcomes import fail
 from _pytest.pathlib import absolutepath
 from _pytest.pathlib import commonpath
 from _pytest.stash import Stash
@@ -51,14 +55,37 @@
 
 SEP = "/"
 
 tracebackcutdir = Path(_pytest.__file__).parent
 
 
 _T = TypeVar("_T")
+
+
+def _imply_path(
+    node_type: Type["Node"],
+    path: Optional[Path],
+    fspath: Optional[LEGACY_PATH],
+) -> Path:
+    if fspath is not None:
+        warnings.warn(
+            NODE_CTOR_FSPATH_ARG.format(
+                node_type_name=node_type.__name__,
+            ),
+            stacklevel=6,
+        )
+    if path is not None:
+        if fspath is not None:
+            _check_path(path, fspath)
+        return path
+    else:
+        assert fspath is not None
+        return Path(fspath)
+
+
 _NodeType = TypeVar("_NodeType", bound="Node")
 
 
 class NodeMeta(abc.ABCMeta):
     """Metaclass used by :class:`Node` to enforce that direct construction raises
     :class:`Failed`.
 
@@ -106,14 +133,21 @@
     r"""Base class of :class:`Collector` and :class:`Item`, the components of
     the test collection tree.
 
     ``Collector``\'s are the internal nodes of the tree, and ``Item``\'s are the
     leaf nodes.
     """
 
+    # Implemented in the legacypath plugin.
+    #: A ``LEGACY_PATH`` copy of the :attr:`path` attribute. Intended for usage
+    #: for methods not migrated to ``pathlib.Path`` yet, such as
+    #: :meth:`Item.reportinfo <pytest.Item.reportinfo>`. Will be deprecated in
+    #: a future release, prefer using :attr:`path` instead.
+    fspath: LEGACY_PATH
+
     # Use __slots__ to make attribute access faster.
     # Note that __dict__ is still available.
     __slots__ = (
         "name",
         "parent",
         "config",
         "session",
@@ -125,14 +159,15 @@
 
     def __init__(
         self,
         name: str,
         parent: "Optional[Node]" = None,
         config: Optional[Config] = None,
         session: "Optional[Session]" = None,
+        fspath: Optional[LEGACY_PATH] = None,
         path: Optional[Path] = None,
         nodeid: Optional[str] = None,
     ) -> None:
         #: A unique name within the scope of the parent node.
         self.name: str = name
 
         #: The parent collector node.
@@ -150,19 +185,18 @@
             #: The pytest session this node is part of.
             self.session: Session = session
         else:
             if not parent:
                 raise TypeError("session or parent must be provided")
             self.session = parent.session
 
-        if path is None:
+        if path is None and fspath is None:
             path = getattr(parent, "path", None)
-        assert path is not None
         #: Filesystem path where this node was collected from (can be None).
-        self.path = path
+        self.path: pathlib.Path = _imply_path(type(self), path, fspath=fspath)
 
         # The explicit annotation is to avoid publicly exposing NodeKeywords.
         #: Keywords/markers collected from all scopes.
         self.keywords: MutableMapping[str, Any] = NodeKeywords(self)
 
         #: The marker objects belonging to this node.
         self.own_markers: List[Mark] = []
@@ -525,14 +559,15 @@
 
 
 class FSCollector(Collector, abc.ABC):
     """Base class for filesystem collectors."""
 
     def __init__(
         self,
+        fspath: Optional[LEGACY_PATH] = None,
         path_or_parent: Optional[Union[Path, Node]] = None,
         path: Optional[Path] = None,
         name: Optional[str] = None,
         parent: Optional[Node] = None,
         config: Optional[Config] = None,
         session: Optional["Session"] = None,
         nodeid: Optional[str] = None,
@@ -540,16 +575,16 @@
         if path_or_parent:
             if isinstance(path_or_parent, Node):
                 assert parent is None
                 parent = cast(FSCollector, path_or_parent)
             elif isinstance(path_or_parent, Path):
                 assert path is None
                 path = path_or_parent
-        assert path is not None
 
+        path = _imply_path(type(self), path, fspath=fspath)
         if name is None:
             name = path.name
             if parent is not None and parent.path != path:
                 try:
                     rel = path.relative_to(parent.path)
                 except ValueError:
                     pass
@@ -581,19 +616,20 @@
         )
 
     @classmethod
     def from_parent(
         cls,
         parent,
         *,
+        fspath: Optional[LEGACY_PATH] = None,
         path: Optional[Path] = None,
         **kw,
     ) -> "Self":
         """The public constructor."""
-        return super().from_parent(parent=parent, path=path, **kw)
+        return super().from_parent(parent=parent, fspath=fspath, path=path, **kw)
 
 
 class File(FSCollector, abc.ABC):
     """Base class for collecting tests from a file.
 
     :ref:`non-python tests`.
     """
```

### Comparing `pytest-8.1.0/src/_pytest/outcomes.py` & `pytest-8.1.1/src/_pytest/outcomes.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/pastebin.py` & `pytest-8.1.1/src/_pytest/pastebin.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/pathlib.py` & `pytest-8.1.1/src/_pytest/pathlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -535,14 +535,18 @@
         try:
             pkg_root, module_name = resolve_pkg_root_and_module_name(
                 path, consider_namespace_packages=consider_namespace_packages
             )
         except CouldNotResolvePathError:
             pass
         else:
+            # If the given module name is already in sys.modules, do not import it again.
+            with contextlib.suppress(KeyError):
+                return sys.modules[module_name]
+
             mod = _import_module_using_spec(
                 module_name, path, pkg_root, insert_modules=False
             )
             if mod is not None:
                 return mod
 
         # Could not import the module with the current sys.path, so we fall back
```

### Comparing `pytest-8.1.0/src/_pytest/pytester.py` & `pytest-8.1.1/src/_pytest/pytester.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/pytester_assertions.py` & `pytest-8.1.1/src/_pytest/pytester_assertions.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/python.py` & `pytest-8.1.1/src/_pytest/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from _pytest.compat import ascii_escaped
 from _pytest.compat import get_default_arg_names
 from _pytest.compat import get_real_func
 from _pytest.compat import getimfunc
 from _pytest.compat import getlocation
 from _pytest.compat import is_async_function
 from _pytest.compat import is_generator
+from _pytest.compat import LEGACY_PATH
 from _pytest.compat import NOTSET
 from _pytest.compat import safe_getattr
 from _pytest.compat import safe_isclass
 from _pytest.config import Config
 from _pytest.config import ExitCode
 from _pytest.config import hookimpl
 from _pytest.config.argparsing import Parser
@@ -661,25 +662,27 @@
     .. versionchanged:: 8.0
 
         Now inherits from :class:`~pytest.Directory`.
     """
 
     def __init__(
         self,
+        fspath: Optional[LEGACY_PATH],
         parent: nodes.Collector,
         # NOTE: following args are unused:
         config=None,
         session=None,
         nodeid=None,
         path: Optional[Path] = None,
     ) -> None:
         # NOTE: Could be just the following, but kept as-is for compat.
         # super().__init__(self, fspath, parent=parent)
         session = parent.session
         super().__init__(
+            fspath=fspath,
             path=path,
             parent=parent,
             config=config,
             session=session,
             nodeid=nodeid,
         )
```

### Comparing `pytest-8.1.0/src/_pytest/python_api.py` & `pytest-8.1.1/src/_pytest/python_api.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/python_path.py` & `pytest-8.1.1/src/_pytest/python_path.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/recwarn.py` & `pytest-8.1.1/src/_pytest/recwarn.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/reports.py` & `pytest-8.1.1/src/_pytest/reports.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/runner.py` & `pytest-8.1.1/src/_pytest/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/scope.py` & `pytest-8.1.1/src/_pytest/scope.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/setuponly.py` & `pytest-8.1.1/src/_pytest/setuponly.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/setupplan.py` & `pytest-8.1.1/src/_pytest/setupplan.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/skipping.py` & `pytest-8.1.1/src/_pytest/skipping.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/stash.py` & `pytest-8.1.1/src/_pytest/stash.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/stepwise.py` & `pytest-8.1.1/src/_pytest/stepwise.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/terminal.py` & `pytest-8.1.1/src/_pytest/terminal.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/threadexception.py` & `pytest-8.1.1/src/_pytest/threadexception.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/tmpdir.py` & `pytest-8.1.1/src/_pytest/tmpdir.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/unittest.py` & `pytest-8.1.1/src/_pytest/unittest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/unraisableexception.py` & `pytest-8.1.1/src/_pytest/unraisableexception.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/warning_types.py` & `pytest-8.1.1/src/_pytest/warning_types.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/_pytest/warnings.py` & `pytest-8.1.1/src/_pytest/warnings.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/pytest/__init__.py` & `pytest-8.1.1/src/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/src/pytest.egg-info/PKG-INFO` & `pytest-8.1.1/src/pytest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest
-Version: 8.1.0
+Version: 8.1.1
 Summary: pytest: simple powerful testing with Python
 Author: Holger Krekel, Bruno Oliveira, Ronny Pfannschmidt, Floris Bruynooghe, Brianna Laugher, Florian Bruhin, Others (See AUTHORS)
 License: MIT
 Project-URL: Changelog, https://docs.pytest.org/en/stable/changelog.html
 Project-URL: Homepage, https://docs.pytest.org/en/latest/
 Project-URL: Source, https://github.com/pytest-dev/pytest
 Project-URL: Tracker, https://github.com/pytest-dev/pytest/issues
```

### Comparing `pytest-8.1.0/src/pytest.egg-info/SOURCES.txt` & `pytest-8.1.1/src/pytest.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -236,14 +236,15 @@
 doc/en/announce/release-7.4.4.rst
 doc/en/announce/release-8.0.0.rst
 doc/en/announce/release-8.0.0rc1.rst
 doc/en/announce/release-8.0.0rc2.rst
 doc/en/announce/release-8.0.1.rst
 doc/en/announce/release-8.0.2.rst
 doc/en/announce/release-8.1.0.rst
+doc/en/announce/release-8.1.1.rst
 doc/en/announce/sprint2016.rst
 doc/en/example/attic.rst
 doc/en/example/conftest.py
 doc/en/example/customdirectory.rst
 doc/en/example/index.rst
 doc/en/example/markers.rst
 doc/en/example/multipython.py
@@ -403,14 +404,15 @@
 src/_pytest/_py/path.py
 src/_pytest/assertion/__init__.py
 src/_pytest/assertion/rewrite.py
 src/_pytest/assertion/truncate.py
 src/_pytest/assertion/util.py
 src/_pytest/config/__init__.py
 src/_pytest/config/argparsing.py
+src/_pytest/config/compat.py
 src/_pytest/config/exceptions.py
 src/_pytest/config/findpaths.py
 src/_pytest/mark/__init__.py
 src/_pytest/mark/expression.py
 src/_pytest/mark/structures.py
 src/pytest/__init__.py
 src/pytest/__main__.py
```

### Comparing `pytest-8.1.0/testing/_py/test_local.py` & `pytest-8.1.1/testing/_py/test_local.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/acceptance_test.py` & `pytest-8.1.1/testing/acceptance_test.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/code/test_code.py` & `pytest-8.1.1/testing/code/test_code.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/code/test_excinfo.py` & `pytest-8.1.1/testing/code/test_excinfo.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/code/test_source.py` & `pytest-8.1.1/testing/code/test_source.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/conftest.py` & `pytest-8.1.1/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/deprecated_test.py` & `pytest-8.1.1/testing/test_helpconfig.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,125 @@
 # mypy: allow-untyped-defs
-from _pytest import deprecated
+from _pytest.config import ExitCode
 from _pytest.pytester import Pytester
 import pytest
-from pytest import PytestDeprecationWarning
 
 
-@pytest.mark.parametrize("plugin", sorted(deprecated.DEPRECATED_EXTERNAL_PLUGINS))
-@pytest.mark.filterwarnings("default")
-def test_external_plugins_integrated(pytester: Pytester, plugin) -> None:
-    pytester.syspathinsert()
-    pytester.makepyfile(**{plugin: ""})
+def test_version_verbose(pytester: Pytester, pytestconfig, monkeypatch) -> None:
+    monkeypatch.delenv("PYTEST_DISABLE_PLUGIN_AUTOLOAD")
+    result = pytester.runpytest("--version", "--version")
+    assert result.ret == 0
+    result.stdout.fnmatch_lines([f"*pytest*{pytest.__version__}*imported from*"])
+    if pytestconfig.pluginmanager.list_plugin_distinfo():
+        result.stdout.fnmatch_lines(["*setuptools registered plugins:", "*at*"])
+
+
+def test_version_less_verbose(pytester: Pytester, pytestconfig, monkeypatch) -> None:
+    monkeypatch.delenv("PYTEST_DISABLE_PLUGIN_AUTOLOAD")
+    result = pytester.runpytest("--version")
+    assert result.ret == 0
+    result.stdout.fnmatch_lines([f"pytest {pytest.__version__}"])
+
+
+def test_versions():
+    """Regression check for the public version attributes in pytest."""
+    assert isinstance(pytest.__version__, str)
+    assert isinstance(pytest.version_tuple, tuple)
+
+
+def test_help(pytester: Pytester) -> None:
+    result = pytester.runpytest("--help")
+    assert result.ret == 0
+    result.stdout.fnmatch_lines(
+        """
+          -m MARKEXPR           Only run tests matching given mark expression. For
+                                example: -m 'mark1 and not mark2'.
+        Reporting:
+          --durations=N *
+          -V, --version         Display pytest version and information about plugins.
+                                When given twice, also display information about
+                                plugins.
+        *setup.cfg*
+        *minversion*
+        *to see*markers*pytest --markers*
+        *to see*fixtures*pytest --fixtures*
+    """
+    )
 
-    with pytest.warns(pytest.PytestConfigWarning):
-        pytester.parseconfig("-p", plugin)
 
+def test_none_help_param_raises_exception(pytester: Pytester) -> None:
+    """Test that a None help param raises a TypeError."""
+    pytester.makeconftest(
+        """
+        def pytest_addoption(parser):
+            parser.addini("test_ini", None, default=True, type="bool")
+    """
+    )
+    result = pytester.runpytest("--help")
+    result.stderr.fnmatch_lines(
+        ["*TypeError: help argument cannot be None for test_ini*"]
+    )
 
-def test_hookspec_via_function_attributes_are_deprecated():
-    from _pytest.config import PytestPluginManager
 
-    pm = PytestPluginManager()
+def test_empty_help_param(pytester: Pytester) -> None:
+    """Test that an empty help param is displayed correctly."""
+    pytester.makeconftest(
+        """
+        def pytest_addoption(parser):
+            parser.addini("test_ini", "", default=True, type="bool")
+    """
+    )
+    result = pytester.runpytest("--help")
+    assert result.ret == 0
+    lines = [
+        "  required_plugins (args):",
+        "                        Plugins that must be present for pytest to run*",
+        "  test_ini (bool):*",
+        "Environment variables:",
+    ]
+    result.stdout.fnmatch_lines(lines, consecutive=True)
+
 
-    class DeprecatedHookMarkerSpec:
-        def pytest_bad_hook(self):
+def test_hookvalidation_unknown(pytester: Pytester) -> None:
+    pytester.makeconftest(
+        """
+        def pytest_hello(xyz):
             pass
+    """
+    )
+    result = pytester.runpytest()
+    assert result.ret != 0
+    result.stdout.fnmatch_lines(["*unknown hook*pytest_hello*"])
 
-        pytest_bad_hook.historic = False  # type: ignore[attr-defined]
 
-    with pytest.warns(
-        PytestDeprecationWarning,
-        match=r"Please use the pytest\.hookspec\(historic=False\) decorator",
-    ) as recorder:
-        pm.add_hookspecs(DeprecatedHookMarkerSpec)
-    (record,) = recorder
-    assert (
-        record.lineno
-        == DeprecatedHookMarkerSpec.pytest_bad_hook.__code__.co_firstlineno
+def test_hookvalidation_optional(pytester: Pytester) -> None:
+    pytester.makeconftest(
+        """
+        import pytest
+        @pytest.hookimpl(optionalhook=True)
+        def pytest_hello(xyz):
+            pass
+    """
     )
-    assert record.filename == __file__
+    result = pytester.runpytest()
+    assert result.ret == ExitCode.NO_TESTS_COLLECTED
 
 
-def test_hookimpl_via_function_attributes_are_deprecated():
-    from _pytest.config import PytestPluginManager
+def test_traceconfig(pytester: Pytester) -> None:
+    result = pytester.runpytest("--traceconfig")
+    result.stdout.fnmatch_lines(["*using*pytest*", "*active plugins*"])
 
-    pm = PytestPluginManager()
 
-    class DeprecatedMarkImplPlugin:
-        def pytest_runtest_call(self):
-            pass
+def test_debug(pytester: Pytester) -> None:
+    result = pytester.runpytest_subprocess("--debug")
+    assert result.ret == ExitCode.NO_TESTS_COLLECTED
+    p = pytester.path.joinpath("pytestdebug.log")
+    assert "pytest_sessionstart" in p.read_text("utf-8")
 
-        pytest_runtest_call.tryfirst = True  # type: ignore[attr-defined]
 
-    with pytest.warns(
-        PytestDeprecationWarning,
-        match=r"Please use the pytest.hookimpl\(tryfirst=True\)",
-    ) as recorder:
-        pm.register(DeprecatedMarkImplPlugin())
-    (record,) = recorder
-    assert (
-        record.lineno
-        == DeprecatedMarkImplPlugin.pytest_runtest_call.__code__.co_firstlineno
-    )
-    assert record.filename == __file__
-
-
-def test_yield_fixture_is_deprecated() -> None:
-    with pytest.warns(DeprecationWarning, match=r"yield_fixture is deprecated"):
-
-        @pytest.yield_fixture
-        def fix():
-            assert False
-
-
-def test_private_is_deprecated() -> None:
-    class PrivateInit:
-        def __init__(self, foo: int, *, _ispytest: bool = False) -> None:
-            deprecated.check_ispytest(_ispytest)
-
-    with pytest.warns(
-        pytest.PytestDeprecationWarning, match="private pytest class or function"
-    ):
-        PrivateInit(10)
-
-    # Doesn't warn.
-    PrivateInit(10, _ispytest=True)
-
-
-def test_fixture_disallow_on_marked_functions():
-    """Test that applying @pytest.fixture to a marked function warns (#3364)."""
-    with pytest.warns(
-        pytest.PytestRemovedIn9Warning,
-        match=r"Marks applied to fixtures have no effect",
-    ) as record:
-
-        @pytest.fixture
-        @pytest.mark.parametrize("example", ["hello"])
-        @pytest.mark.usefixtures("tmp_path")
-        def foo():
-            raise NotImplementedError()
-
-    # it's only possible to get one warning here because you're already prevented
-    # from applying @fixture twice
-    # ValueError("fixture is being applied more than once to the same function")
-    assert len(record) == 1
-
-
-def test_fixture_disallow_marks_on_fixtures():
-    """Test that applying a mark to a fixture warns (#3364)."""
-    with pytest.warns(
-        pytest.PytestRemovedIn9Warning,
-        match=r"Marks applied to fixtures have no effect",
-    ) as record:
-
-        @pytest.mark.parametrize("example", ["hello"])
-        @pytest.mark.usefixtures("tmp_path")
-        @pytest.fixture
-        def foo():
-            raise NotImplementedError()
-
-    assert len(record) == 2  # one for each mark decorator
-    # should point to this file
-    assert all(rec.filename == __file__ for rec in record)
-
-
-def test_fixture_disallowed_between_marks():
-    """Test that applying a mark to a fixture warns (#3364)."""
-    with pytest.warns(
-        pytest.PytestRemovedIn9Warning,
-        match=r"Marks applied to fixtures have no effect",
-    ) as record:
-
-        @pytest.mark.parametrize("example", ["hello"])
-        @pytest.fixture
-        @pytest.mark.usefixtures("tmp_path")
-        def foo():
-            raise NotImplementedError()
-
-    assert len(record) == 2  # one for each mark decorator
+def test_PYTEST_DEBUG(pytester: Pytester, monkeypatch) -> None:
+    monkeypatch.setenv("PYTEST_DEBUG", "1")
+    result = pytester.runpytest_subprocess()
+    assert result.ret == ExitCode.NO_TESTS_COLLECTED
+    result.stderr.fnmatch_lines(
+        ["*pytest_plugin_registered*", "*manager*PluginManager*"]
+    )
```

### Comparing `pytest-8.1.0/testing/example_scripts/customdirectory/conftest.py` & `pytest-8.1.1/testing/example_scripts/customdirectory/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/example_scripts/dataclasses/test_compare_recursive_dataclasses.py` & `pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_recursive_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/example_scripts/issue_519.py` & `pytest-8.1.1/testing/example_scripts/issue_519.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/example_scripts/junit-10.xsd` & `pytest-8.1.1/testing/example_scripts/junit-10.xsd`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/example_scripts/perf_examples/collect_stats/generate_folders.py` & `pytest-8.1.1/testing/example_scripts/perf_examples/collect_stats/generate_folders.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/example_scripts/unittest/test_unittest_asyncio.py` & `pytest-8.1.1/testing/example_scripts/unittest/test_unittest_asyncio.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/io/test_pprint.py` & `pytest-8.1.1/testing/io/test_pprint.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/io/test_saferepr.py` & `pytest-8.1.1/testing/io/test_saferepr.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/io/test_terminalwriter.py` & `pytest-8.1.1/testing/io/test_terminalwriter.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/io/test_wcwidth.py` & `pytest-8.1.1/testing/io/test_wcwidth.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/logging/test_fixture.py` & `pytest-8.1.1/testing/logging/test_fixture.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/logging/test_formatter.py` & `pytest-8.1.1/testing/logging/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/logging/test_reporting.py` & `pytest-8.1.1/testing/logging/test_reporting.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/plugins_integration/README.rst` & `pytest-8.1.1/testing/plugins_integration/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/plugins_integration/bdd_wallet.py` & `pytest-8.1.1/testing/plugins_integration/bdd_wallet.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/python/approx.py` & `pytest-8.1.1/testing/python/approx.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/python/collect.py` & `pytest-8.1.1/testing/python/collect.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/python/fixtures.py` & `pytest-8.1.1/testing/python/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/python/integration.py` & `pytest-8.1.1/testing/python/integration.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/python/metafunc.py` & `pytest-8.1.1/testing/python/metafunc.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/python/raises.py` & `pytest-8.1.1/testing/python/raises.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/python/show_fixtures_per_test.py` & `pytest-8.1.1/testing/python/show_fixtures_per_test.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_argcomplete.py` & `pytest-8.1.1/testing/test_argcomplete.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_assertion.py` & `pytest-8.1.1/testing/test_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_assertrewrite.py` & `pytest-8.1.1/testing/test_assertrewrite.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_cacheprovider.py` & `pytest-8.1.1/testing/test_cacheprovider.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_capture.py` & `pytest-8.1.1/testing/test_capture.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_collection.py` & `pytest-8.1.1/testing/test_collection.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_compat.py` & `pytest-8.1.1/testing/test_compat.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_config.py` & `pytest-8.1.1/testing/test_config.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_conftest.py` & `pytest-8.1.1/testing/test_conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_debugging.py` & `pytest-8.1.1/testing/test_debugging.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_doctest.py` & `pytest-8.1.1/testing/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_error_diffs.py` & `pytest-8.1.1/testing/test_error_diffs.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_faulthandler.py` & `pytest-8.1.1/testing/test_faulthandler.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_findpaths.py` & `pytest-8.1.1/testing/test_findpaths.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_helpconfig.py` & `pytest-8.1.1/testing/test_python_path.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,125 +1,113 @@
 # mypy: allow-untyped-defs
-from _pytest.config import ExitCode
+import sys
+from textwrap import dedent
+from typing import Generator
+from typing import List
+from typing import Optional
+
 from _pytest.pytester import Pytester
 import pytest
 
 
-def test_version_verbose(pytester: Pytester, pytestconfig, monkeypatch) -> None:
-    monkeypatch.delenv("PYTEST_DISABLE_PLUGIN_AUTOLOAD")
-    result = pytester.runpytest("--version", "--version")
-    assert result.ret == 0
-    result.stdout.fnmatch_lines([f"*pytest*{pytest.__version__}*imported from*"])
-    if pytestconfig.pluginmanager.list_plugin_distinfo():
-        result.stdout.fnmatch_lines(["*setuptools registered plugins:", "*at*"])
-
-
-def test_version_less_verbose(pytester: Pytester, pytestconfig, monkeypatch) -> None:
-    monkeypatch.delenv("PYTEST_DISABLE_PLUGIN_AUTOLOAD")
-    result = pytester.runpytest("--version")
-    assert result.ret == 0
-    result.stdout.fnmatch_lines([f"pytest {pytest.__version__}"])
-
-
-def test_versions():
-    """Regression check for the public version attributes in pytest."""
-    assert isinstance(pytest.__version__, str)
-    assert isinstance(pytest.version_tuple, tuple)
-
+@pytest.fixture()
+def file_structure(pytester: Pytester) -> None:
+    pytester.makepyfile(
+        test_foo="""
+        from foo import foo
 
-def test_help(pytester: Pytester) -> None:
-    result = pytester.runpytest("--help")
-    assert result.ret == 0
-    result.stdout.fnmatch_lines(
+        def test_foo():
+            assert foo() == 1
         """
-          -m MARKEXPR           Only run tests matching given mark expression. For
-                                example: -m 'mark1 and not mark2'.
-        Reporting:
-          --durations=N *
-          -V, --version         Display pytest version and information about plugins.
-                                When given twice, also display information about
-                                plugins.
-        *setup.cfg*
-        *minversion*
-        *to see*markers*pytest --markers*
-        *to see*fixtures*pytest --fixtures*
-    """
     )
 
+    pytester.makepyfile(
+        test_bar="""
+        from bar import bar
 
-def test_none_help_param_raises_exception(pytester: Pytester) -> None:
-    """Test that a None help param raises a TypeError."""
-    pytester.makeconftest(
-        """
-        def pytest_addoption(parser):
-            parser.addini("test_ini", None, default=True, type="bool")
-    """
-    )
-    result = pytester.runpytest("--help")
-    result.stderr.fnmatch_lines(
-        ["*TypeError: help argument cannot be None for test_ini*"]
+        def test_bar():
+            assert bar() == 2
+        """
     )
 
-
-def test_empty_help_param(pytester: Pytester) -> None:
-    """Test that an empty help param is displayed correctly."""
-    pytester.makeconftest(
-        """
-        def pytest_addoption(parser):
-            parser.addini("test_ini", "", default=True, type="bool")
-    """
+    foo_py = pytester.mkdir("sub") / "foo.py"
+    content = dedent(
+        """
+        def foo():
+            return 1
+        """
     )
-    result = pytester.runpytest("--help")
-    assert result.ret == 0
-    lines = [
-        "  required_plugins (args):",
-        "                        Plugins that must be present for pytest to run*",
-        "  test_ini (bool):*",
-        "Environment variables:",
-    ]
-    result.stdout.fnmatch_lines(lines, consecutive=True)
+    foo_py.write_text(content, encoding="utf-8")
 
-
-def test_hookvalidation_unknown(pytester: Pytester) -> None:
-    pytester.makeconftest(
-        """
-        def pytest_hello(xyz):
-            pass
-    """
+    bar_py = pytester.mkdir("sub2") / "bar.py"
+    content = dedent(
+        """
+        def bar():
+            return 2
+        """
     )
-    result = pytester.runpytest()
-    assert result.ret != 0
-    result.stdout.fnmatch_lines(["*unknown hook*pytest_hello*"])
+    bar_py.write_text(content, encoding="utf-8")
 
 
-def test_hookvalidation_optional(pytester: Pytester) -> None:
-    pytester.makeconftest(
-        """
-        import pytest
-        @pytest.hookimpl(optionalhook=True)
-        def pytest_hello(xyz):
-            pass
-    """
-    )
-    result = pytester.runpytest()
-    assert result.ret == ExitCode.NO_TESTS_COLLECTED
+def test_one_dir(pytester: Pytester, file_structure) -> None:
+    pytester.makefile(".ini", pytest="[pytest]\npythonpath=sub\n")
+    result = pytester.runpytest("test_foo.py")
+    assert result.ret == 0
+    result.assert_outcomes(passed=1)
 
 
-def test_traceconfig(pytester: Pytester) -> None:
-    result = pytester.runpytest("--traceconfig")
-    result.stdout.fnmatch_lines(["*using*pytest*", "*active plugins*"])
+def test_two_dirs(pytester: Pytester, file_structure) -> None:
+    pytester.makefile(".ini", pytest="[pytest]\npythonpath=sub sub2\n")
+    result = pytester.runpytest("test_foo.py", "test_bar.py")
+    assert result.ret == 0
+    result.assert_outcomes(passed=2)
 
 
-def test_debug(pytester: Pytester) -> None:
-    result = pytester.runpytest_subprocess("--debug")
-    assert result.ret == ExitCode.NO_TESTS_COLLECTED
-    p = pytester.path.joinpath("pytestdebug.log")
-    assert "pytest_sessionstart" in p.read_text("utf-8")
+def test_module_not_found(pytester: Pytester, file_structure) -> None:
+    """Without the pythonpath setting, the module should not be found."""
+    pytester.makefile(".ini", pytest="[pytest]\n")
+    result = pytester.runpytest("test_foo.py")
+    assert result.ret == pytest.ExitCode.INTERRUPTED
+    result.assert_outcomes(errors=1)
+    expected_error = "E   ModuleNotFoundError: No module named 'foo'"
+    result.stdout.fnmatch_lines([expected_error])
+
+
+def test_no_ini(pytester: Pytester, file_structure) -> None:
+    """If no ini file, test should error."""
+    result = pytester.runpytest("test_foo.py")
+    assert result.ret == pytest.ExitCode.INTERRUPTED
+    result.assert_outcomes(errors=1)
+    expected_error = "E   ModuleNotFoundError: No module named 'foo'"
+    result.stdout.fnmatch_lines([expected_error])
+
+
+def test_clean_up(pytester: Pytester) -> None:
+    """Test that the plugin cleans up after itself."""
+    # This is tough to test behaviorally because the cleanup really runs last.
+    # So the test make several implementation assumptions:
+    # - Cleanup is done in pytest_unconfigure().
+    # - Not a hook wrapper.
+    # So we can add a hook wrapper ourselves to test what it does.
+    pytester.makefile(".ini", pytest="[pytest]\npythonpath=I_SHALL_BE_REMOVED\n")
+    pytester.makepyfile(test_foo="""def test_foo(): pass""")
+
+    before: Optional[List[str]] = None
+    after: Optional[List[str]] = None
+
+    class Plugin:
+        @pytest.hookimpl(wrapper=True, tryfirst=True)
+        def pytest_unconfigure(self) -> Generator[None, None, None]:
+            nonlocal before, after
+            before = sys.path.copy()
+            try:
+                return (yield)
+            finally:
+                after = sys.path.copy()
 
+    result = pytester.runpytest_inprocess(plugins=[Plugin()])
+    assert result.ret == 0
 
-def test_PYTEST_DEBUG(pytester: Pytester, monkeypatch) -> None:
-    monkeypatch.setenv("PYTEST_DEBUG", "1")
-    result = pytester.runpytest_subprocess()
-    assert result.ret == ExitCode.NO_TESTS_COLLECTED
-    result.stderr.fnmatch_lines(
-        ["*pytest_plugin_registered*", "*manager*PluginManager*"]
-    )
+    assert before is not None
+    assert after is not None
+    assert any("I_SHALL_BE_REMOVED" in entry for entry in before)
+    assert not any("I_SHALL_BE_REMOVED" in entry for entry in after)
```

### Comparing `pytest-8.1.0/testing/test_junitxml.py` & `pytest-8.1.1/testing/test_junitxml.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_legacypath.py` & `pytest-8.1.1/testing/test_legacypath.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # mypy: allow-untyped-defs
 from pathlib import Path
 
+from _pytest.compat import LEGACY_PATH
 from _pytest.fixtures import TopRequest
-from _pytest.legacypath import LEGACY_PATH
 from _pytest.legacypath import TempdirFactory
 from _pytest.legacypath import Testdir
 import pytest
 
 
 def test_item_fspath(pytester: pytest.Pytester) -> None:
     pytester.makepyfile("def test_func(): pass")
     items, hookrec = pytester.inline_genitems()
     assert len(items) == 1
     (item,) = items
     items2, hookrec = pytester.inline_genitems(item.nodeid)
     (item2,) = items2
     assert item2.name == item.name
-    assert item2.fspath == item.fspath  # type: ignore[attr-defined]
+    assert item2.fspath == item.fspath
     assert item2.path == item.path
 
 
 def test_testdir_testtmproot(testdir: Testdir) -> None:
     """Check test_tmproot is a py.path attribute for backward compatibility."""
     assert testdir.test_tmproot.check(dir=1)
```

### Comparing `pytest-8.1.0/testing/test_link_resolve.py` & `pytest-8.1.1/testing/test_link_resolve.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_main.py` & `pytest-8.1.1/testing/test_main.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_mark.py` & `pytest-8.1.1/testing/test_mark.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_mark_expression.py` & `pytest-8.1.1/testing/test_mark_expression.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_meta.py` & `pytest-8.1.1/testing/test_meta.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_monkeypatch.py` & `pytest-8.1.1/testing/test_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_nodes.py` & `pytest-8.1.1/testing/test_nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 import re
 from typing import cast
 from typing import Type
 import warnings
 
 from _pytest import nodes
+from _pytest.compat import legacy_path
 from _pytest.outcomes import OutcomeException
 from _pytest.pytester import Pytester
 from _pytest.warning_types import PytestWarning
 import pytest
 
 
 def test_node_from_parent_disallowed_arguments() -> None:
@@ -40,26 +41,28 @@
     inheritance constructors with missing args as found in plugins.
     """
     # We do not expect any warnings messages to issued during class definition.
     with warnings.catch_warnings():
         warnings.simplefilter("error")
 
         class SoWrong(nodes.Item, nodes.File):
-            def __init__(self, path, parent):
+            def __init__(self, fspath, parent):
                 """Legacy ctor with legacy call # don't wana see"""
-                super().__init__(parent, path)
+                super().__init__(fspath, parent)
 
             def collect(self):
                 raise NotImplementedError()
 
             def runtest(self):
                 raise NotImplementedError()
 
     with pytest.warns(PytestWarning) as rec:
-        SoWrong.from_parent(request.session, path=tmp_path / "broken.txt", wrong=10)
+        SoWrong.from_parent(
+            request.session, fspath=legacy_path(tmp_path / "broken.txt")
+        )
     messages = [str(x.message) for x in rec]
     assert any(
         re.search(".*SoWrong.* not using a cooperative constructor.*", x)
         for x in messages
     )
     assert any(
         re.search("(?m)SoWrong .* should not be a collector", x) for x in messages
```

### Comparing `pytest-8.1.0/testing/test_parseopt.py` & `pytest-8.1.1/testing/test_parseopt.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_pastebin.py` & `pytest-8.1.1/testing/test_pastebin.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_pathlib.py` & `pytest-8.1.1/testing/test_pathlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -583,14 +583,20 @@
             fn, mode="importlib", root=tmp_path, consider_namespace_packages=ns_param
         )
         Data: Any = getattr(module, "Data")
         data = Data(value="foo")
         assert data.value == "foo"
         assert data.__module__ == "_src.tests.test_dataclass"
 
+        # Ensure we do not import the same module again (#11475).
+        module2 = import_path(
+            fn, mode="importlib", root=tmp_path, consider_namespace_packages=ns_param
+        )
+        assert module is module2
+
     def test_importmode_importlib_with_pickle(
         self, tmp_path: Path, ns_param: bool
     ) -> None:
         """Ensure that importlib mode works with pickle (#7859)."""
         fn = tmp_path.joinpath("_src/tests/test_pickle.py")
         fn.parent.mkdir(parents=True)
         fn.write_text(
@@ -612,14 +618,20 @@
         module = import_path(
             fn, mode="importlib", root=tmp_path, consider_namespace_packages=ns_param
         )
         round_trip = getattr(module, "round_trip")
         action = round_trip()
         assert action() == 42
 
+        # Ensure we do not import the same module again (#11475).
+        module2 = import_path(
+            fn, mode="importlib", root=tmp_path, consider_namespace_packages=ns_param
+        )
+        assert module is module2
+
     def test_importmode_importlib_with_pickle_separate_modules(
         self, tmp_path: Path, ns_param: bool
     ) -> None:
         """
         Ensure that importlib mode works can load pickles that look similar but are
         defined in separate modules.
         """
@@ -812,14 +824,22 @@
         mod = import_path(
             init,
             root=tmp_path,
             mode=ImportMode.importlib,
             consider_namespace_packages=ns_param,
         )
         assert len(mod.instance.INSTANCES) == 1
+        # Ensure we do not import the same module again (#11475).
+        mod2 = import_path(
+            init,
+            root=tmp_path,
+            mode=ImportMode.importlib,
+            consider_namespace_packages=ns_param,
+        )
+        assert mod is mod2
 
     def test_importlib_root_is_package(self, pytester: Pytester) -> None:
         """
         Regression for importing a `__init__`.py file that is at the root
         (#11417).
         """
         pytester.makepyfile(__init__="")
@@ -938,32 +958,60 @@
             mode="importlib",
             root=pytester.path,
             consider_namespace_packages=ns_param,
         )
         assert mod.__name__ == "app.core"
         assert mod.__file__ and Path(mod.__file__) == core_py
 
+        # Ensure we do not import the same module again (#11475).
+        mod2 = import_path(
+            core_py,
+            mode="importlib",
+            root=pytester.path,
+            consider_namespace_packages=ns_param,
+        )
+        assert mod is mod2
+
         # tests are not reachable from sys.path, so they are imported as a standalone modules.
         # Instead of '.tests.a.test_core', we import as "_tests.a.test_core" because
         # importlib considers module names starting with '.' to be local imports.
         mod = import_path(
             test_path1,
             mode="importlib",
             root=pytester.path,
             consider_namespace_packages=ns_param,
         )
         assert mod.__name__ == "_tests.a.test_core"
+
+        # Ensure we do not import the same module again (#11475).
+        mod2 = import_path(
+            test_path1,
+            mode="importlib",
+            root=pytester.path,
+            consider_namespace_packages=ns_param,
+        )
+        assert mod is mod2
+
         mod = import_path(
             test_path2,
             mode="importlib",
             root=pytester.path,
             consider_namespace_packages=ns_param,
         )
         assert mod.__name__ == "_tests.b.test_core"
 
+        # Ensure we do not import the same module again (#11475).
+        mod2 = import_path(
+            test_path2,
+            mode="importlib",
+            root=pytester.path,
+            consider_namespace_packages=ns_param,
+        )
+        assert mod is mod2
+
     def test_import_using_normal_mechanism_first_integration(
         self, monkeypatch: MonkeyPatch, pytester: Pytester, ns_param: bool
     ) -> None:
         """
         Same test as above, but verify the behavior calling pytest.
 
         We should not make this call in the same test as above, as the modules have already
@@ -1017,14 +1065,22 @@
             mode=ImportMode.importlib,
             root=pytester.path,
             consider_namespace_packages=ns_param,
         )
         assert mod.__file__ and Path(mod.__file__) == x_in_sub_folder
         assert mod.X == "a/b/x"
 
+        mod2 = import_path(
+            x_in_sub_folder,
+            mode=ImportMode.importlib,
+            root=pytester.path,
+            consider_namespace_packages=ns_param,
+        )
+        assert mod is mod2
+
         # Attempt to import root 'x.py'.
         with pytest.raises(AssertionError, match="x at root"):
             _ = import_path(
                 x_at_root,
                 mode=ImportMode.importlib,
                 root=pytester.path,
                 consider_namespace_packages=ns_param,
@@ -1120,14 +1176,20 @@
 
         mod = import_path(
             models_py, mode=import_mode, root=tmp_path, consider_namespace_packages=True
         )
         assert mod.__name__ == "com.company.app.core.models"
         assert mod.__file__ == str(models_py)
 
+        # Ensure we do not import the same module again (#11475).
+        mod2 = import_path(
+            models_py, mode=import_mode, root=tmp_path, consider_namespace_packages=True
+        )
+        assert mod is mod2
+
         pkg_root, module_name = resolve_pkg_root_and_module_name(
             algorithms_py, consider_namespace_packages=True
         )
         assert (pkg_root, module_name) == (
             tmp_path / "src/dist2",
             "com.company.calc.algo.algorithms",
         )
@@ -1137,14 +1199,23 @@
             mode=import_mode,
             root=tmp_path,
             consider_namespace_packages=True,
         )
         assert mod.__name__ == "com.company.calc.algo.algorithms"
         assert mod.__file__ == str(algorithms_py)
 
+        # Ensure we do not import the same module again (#11475).
+        mod2 = import_path(
+            algorithms_py,
+            mode=import_mode,
+            root=tmp_path,
+            consider_namespace_packages=True,
+        )
+        assert mod is mod2
+
     @pytest.mark.parametrize("import_mode", ["prepend", "append", "importlib"])
     def test_incorrect_namespace_package(
         self,
         tmp_path: Path,
         monkeypatch: MonkeyPatch,
         pytester: Pytester,
         import_mode: str,
```

### Comparing `pytest-8.1.0/testing/test_pluginmanager.py` & `pytest-8.1.1/testing/test_pluginmanager.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_pytester.py` & `pytest-8.1.1/testing/test_pytester.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_python_path.py` & `pytest-8.1.1/testing/test_setupplan.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,120 @@
-# mypy: allow-untyped-defs
-import sys
-from textwrap import dedent
-from typing import Generator
-from typing import List
-from typing import Optional
-
 from _pytest.pytester import Pytester
-import pytest
 
 
-@pytest.fixture()
-def file_structure(pytester: Pytester) -> None:
+def test_show_fixtures_and_test(
+    pytester: Pytester, dummy_yaml_custom_test: None
+) -> None:
+    """Verify that fixtures are not executed."""
     pytester.makepyfile(
-        test_foo="""
-        from foo import foo
-
-        def test_foo():
-            assert foo() == 1
         """
+        import pytest
+        @pytest.fixture
+        def arg():
+            assert False
+        def test_arg(arg):
+            assert False
+    """
     )
 
-    pytester.makepyfile(
-        test_bar="""
-        from bar import bar
+    result = pytester.runpytest("--setup-plan")
+    assert result.ret == 0
 
-        def test_bar():
-            assert bar() == 2
-        """
+    result.stdout.fnmatch_lines(
+        ["*SETUP    F arg*", "*test_arg (fixtures used: arg)", "*TEARDOWN F arg*"]
     )
 
-    foo_py = pytester.mkdir("sub") / "foo.py"
-    content = dedent(
-        """
-        def foo():
-            return 1
-        """
-    )
-    foo_py.write_text(content, encoding="utf-8")
 
-    bar_py = pytester.mkdir("sub2") / "bar.py"
-    content = dedent(
-        """
-        def bar():
-            return 2
+def test_show_multi_test_fixture_setup_and_teardown_correctly_simple(
+    pytester: Pytester,
+) -> None:
+    """Verify that when a fixture lives for longer than a single test, --setup-plan
+    correctly displays the SETUP/TEARDOWN indicators the right number of times.
+
+    As reported in https://github.com/pytest-dev/pytest/issues/2049
+    --setup-plan was showing SETUP/TEARDOWN on every test, even when the fixture
+    should persist through multiple tests.
+
+    (Note that this bug never affected actual test execution, which used the
+    correct fixture lifetimes. It was purely a display bug for --setup-plan, and
+    did not affect the related --setup-show or --setup-only.)
+    """
+    pytester.makepyfile(
         """
+        import pytest
+        @pytest.fixture(scope = 'class')
+        def fix():
+            return object()
+        class TestClass:
+            def test_one(self, fix):
+                assert False
+            def test_two(self, fix):
+                assert False
+    """
     )
-    bar_py.write_text(content, encoding="utf-8")
 
-
-def test_one_dir(pytester: Pytester, file_structure) -> None:
-    pytester.makefile(".ini", pytest="[pytest]\npythonpath=sub\n")
-    result = pytester.runpytest("test_foo.py")
+    result = pytester.runpytest("--setup-plan")
     assert result.ret == 0
-    result.assert_outcomes(passed=1)
 
+    setup_fragment = "SETUP    C fix"
+    setup_count = 0
 
-def test_two_dirs(pytester: Pytester, file_structure) -> None:
-    pytester.makefile(".ini", pytest="[pytest]\npythonpath=sub sub2\n")
-    result = pytester.runpytest("test_foo.py", "test_bar.py")
-    assert result.ret == 0
-    result.assert_outcomes(passed=2)
+    teardown_fragment = "TEARDOWN C fix"
+    teardown_count = 0
 
+    for line in result.stdout.lines:
+        if setup_fragment in line:
+            setup_count += 1
+        if teardown_fragment in line:
+            teardown_count += 1
+
+    # before the fix this tests, there would have been a setup/teardown
+    # message for each test, so the counts would each have been 2
+    assert setup_count == 1
+    assert teardown_count == 1
+
+
+def test_show_multi_test_fixture_setup_and_teardown_same_as_setup_show(
+    pytester: Pytester,
+) -> None:
+    """Verify that SETUP/TEARDOWN messages match what comes out of --setup-show."""
+    pytester.makepyfile(
+        """
+        import pytest
+        @pytest.fixture(scope = 'session')
+        def sess():
+            return True
+        @pytest.fixture(scope = 'module')
+        def mod():
+            return True
+        @pytest.fixture(scope = 'class')
+        def cls():
+            return True
+        @pytest.fixture(scope = 'function')
+        def func():
+            return True
+        def test_outside(sess, mod, cls, func):
+            assert True
+        class TestCls:
+            def test_one(self, sess, mod, cls, func):
+                assert True
+            def test_two(self, sess, mod, cls, func):
+                assert True
+    """
+    )
 
-def test_module_not_found(pytester: Pytester, file_structure) -> None:
-    """Without the pythonpath setting, the module should not be found."""
-    pytester.makefile(".ini", pytest="[pytest]\n")
-    result = pytester.runpytest("test_foo.py")
-    assert result.ret == pytest.ExitCode.INTERRUPTED
-    result.assert_outcomes(errors=1)
-    expected_error = "E   ModuleNotFoundError: No module named 'foo'"
-    result.stdout.fnmatch_lines([expected_error])
-
-
-def test_no_ini(pytester: Pytester, file_structure) -> None:
-    """If no ini file, test should error."""
-    result = pytester.runpytest("test_foo.py")
-    assert result.ret == pytest.ExitCode.INTERRUPTED
-    result.assert_outcomes(errors=1)
-    expected_error = "E   ModuleNotFoundError: No module named 'foo'"
-    result.stdout.fnmatch_lines([expected_error])
-
-
-def test_clean_up(pytester: Pytester) -> None:
-    """Test that the plugin cleans up after itself."""
-    # This is tough to test behaviorally because the cleanup really runs last.
-    # So the test make several implementation assumptions:
-    # - Cleanup is done in pytest_unconfigure().
-    # - Not a hook wrapper.
-    # So we can add a hook wrapper ourselves to test what it does.
-    pytester.makefile(".ini", pytest="[pytest]\npythonpath=I_SHALL_BE_REMOVED\n")
-    pytester.makepyfile(test_foo="""def test_foo(): pass""")
-
-    before: Optional[List[str]] = None
-    after: Optional[List[str]] = None
-
-    class Plugin:
-        @pytest.hookimpl(wrapper=True, tryfirst=True)
-        def pytest_unconfigure(self) -> Generator[None, None, None]:
-            nonlocal before, after
-            before = sys.path.copy()
-            try:
-                return (yield)
-            finally:
-                after = sys.path.copy()
+    plan_result = pytester.runpytest("--setup-plan")
+    show_result = pytester.runpytest("--setup-show")
 
-    result = pytester.runpytest_inprocess(plugins=[Plugin()])
-    assert result.ret == 0
+    # the number and text of these lines should be identical
+    plan_lines = [
+        line
+        for line in plan_result.stdout.lines
+        if "SETUP" in line or "TEARDOWN" in line
+    ]
+    show_lines = [
+        line
+        for line in show_result.stdout.lines
+        if "SETUP" in line or "TEARDOWN" in line
+    ]
 
-    assert before is not None
-    assert after is not None
-    assert any("I_SHALL_BE_REMOVED" in entry for entry in before)
-    assert not any("I_SHALL_BE_REMOVED" in entry for entry in after)
+    assert plan_lines == show_lines
```

### Comparing `pytest-8.1.0/testing/test_recwarn.py` & `pytest-8.1.1/testing/test_recwarn.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_reports.py` & `pytest-8.1.1/testing/test_reports.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_runner.py` & `pytest-8.1.1/testing/test_runner.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_runner_xunit.py` & `pytest-8.1.1/testing/test_runner_xunit.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_scope.py` & `pytest-8.1.1/testing/test_scope.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_session.py` & `pytest-8.1.1/testing/test_session.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_setuponly.py` & `pytest-8.1.1/testing/test_setuponly.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_skipping.py` & `pytest-8.1.1/testing/test_skipping.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_stash.py` & `pytest-8.1.1/testing/test_stash.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_stepwise.py` & `pytest-8.1.1/testing/test_stepwise.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_terminal.py` & `pytest-8.1.1/testing/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_threadexception.py` & `pytest-8.1.1/testing/test_threadexception.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_tmpdir.py` & `pytest-8.1.1/testing/test_tmpdir.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_unittest.py` & `pytest-8.1.1/testing/test_unittest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_unraisableexception.py` & `pytest-8.1.1/testing/test_unraisableexception.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_warning_types.py` & `pytest-8.1.1/testing/test_warning_types.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/test_warnings.py` & `pytest-8.1.1/testing/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/testing/typing_checks.py` & `pytest-8.1.1/testing/typing_checks.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.0/tox.ini` & `pytest-8.1.1/tox.ini`

 * *Files identical despite different names*

