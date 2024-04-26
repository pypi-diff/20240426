# Comparing `tmp/mintalib-0.0.7.tar.gz` & `tmp/mintalib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mintalib-0.0.7.tar", last modified: Mon Jan  8 18:43:54 2024, max compression
+gzip compressed data, was "mintalib-0.0.8.tar", last modified: Fri Apr 26 01:16:11 2024, max compression
```

## Comparing `mintalib-0.0.7.tar` & `mintalib-0.0.8.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-01-08 18:43:54.705362 mintalib-0.0.7/
--rw-r--r--   0 frederic   (501) staff       (20)     1080 2023-11-27 20:51:02.000000 mintalib-0.0.7/LICENSE.txt
--rw-r--r--   0 frederic   (501) staff       (20)      111 2023-12-31 16:09:00.000000 mintalib-0.0.7/MANIFEST.in
--rw-r--r--   0 frederic   (501) staff       (20)     8978 2024-01-08 18:43:54.705147 mintalib-0.0.7/PKG-INFO
--rw-r--r--   0 frederic   (501) staff       (20)     8227 2023-11-27 20:51:02.000000 mintalib-0.0.7/README.md
--rwxr-xr-x   0 frederic   (501) staff       (20)      859 2024-01-08 18:40:54.000000 mintalib-0.0.7/pyproject.toml
--rw-r--r--   0 frederic   (501) staff       (20)       38 2024-01-08 18:43:54.705400 mintalib-0.0.7/setup.cfg
--rwxr-xr-x   0 frederic   (501) staff       (20)      812 2023-12-31 16:31:32.000000 mintalib-0.0.7/setup.py
-drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-01-08 18:43:54.695836 mintalib-0.0.7/src/
-drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-01-08 18:43:54.699194 mintalib-0.0.7/src/mintalib/
--rw-r--r--   0 frederic   (501) staff       (20)       19 2023-12-31 16:24:09.000000 mintalib-0.0.7/src/mintalib/__init__.py
--rw-r--r--   0 frederic   (501) staff       (20)  3569205 2023-12-31 20:06:42.000000 mintalib-0.0.7/src/mintalib/core.c
--rw-r--r--   0 frederic   (501) staff       (20)      248 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/core.pyx
-drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-01-08 18:43:54.704195 mintalib-0.0.7/src/mintalib/cython/
--rwxr-xr-x   0 frederic   (501) staff       (20)        0 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/__init__.py
--rw-r--r--   0 frederic   (501) staff       (20)      770 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/_all_core.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     2678 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/_common.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     2172 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/adx.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     2638 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/atr.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      709 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/bbands.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      692 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/bop.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      537 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/cci.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      791 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/cmf.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1606 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/cross.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     3577 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/curve.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      534 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/dema.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      814 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/diff.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1955 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/ema.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      371 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/eval.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      473 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/exp.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     4841 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/flags.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     2676 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/kama.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      718 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/keltner.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      468 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/log.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      759 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/macd.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1245 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/mad.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1188 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/matype.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      988 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/max.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      673 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/mfi.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      989 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/min.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      788 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/ppo.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     3732 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/price.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1384 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/rma.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      902 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/roc.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1421 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/rsi.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     2049 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/sar.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     3527 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/slope.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1179 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/sma.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1155 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/stdev.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1017 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/stoch.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1781 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/streak.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1086 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/sum.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      656 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/tema.pxi
--rw-r--r--   0 frederic   (501) staff       (20)     1061 2023-11-27 20:51:02.000000 mintalib-0.0.7/src/mintalib/cython/wma.pxi
--rw-r--r--   0 frederic   (501) staff       (20)      758 2023-12-31 16:24:09.000000 mintalib-0.0.7/src/mintalib/functions.py
--rw-r--r--   0 frederic   (501) staff       (20)     1111 2023-12-31 16:24:09.000000 mintalib-0.0.7/src/mintalib/helper.py
--rw-r--r--   0 frederic   (501) staff       (20)    15330 2023-12-31 16:24:09.000000 mintalib-0.0.7/src/mintalib/indicators.py
--rw-r--r--   0 frederic   (501) staff       (20)     1723 2023-12-31 16:24:09.000000 mintalib-0.0.7/src/mintalib/model.py
--rw-r--r--   0 frederic   (501) staff       (20)     3295 2023-12-31 16:36:51.000000 mintalib-0.0.7/src/mintalib/reflib.py
-drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-01-08 18:43:54.704405 mintalib-0.0.7/src/mintalib/samples/
--rw-r--r--   0 frederic   (501) staff       (20)     1673 2024-01-08 14:27:54.000000 mintalib-0.0.7/src/mintalib/samples/__init__.py
--rw-r--r--   0 frederic   (501) staff       (20)   145504 2024-01-08 14:00:59.000000 mintalib-0.0.7/src/mintalib/samples/sample-prices.csv
--rw-r--r--   0 frederic   (501) staff       (20)     2879 2023-12-31 16:24:09.000000 mintalib-0.0.7/src/mintalib/utils.py
-drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-01-08 18:43:54.704772 mintalib-0.0.7/src/mintalib.egg-info/
--rw-r--r--   0 frederic   (501) staff       (20)     8978 2024-01-08 18:43:54.000000 mintalib-0.0.7/src/mintalib.egg-info/PKG-INFO
--rw-r--r--   0 frederic   (501) staff       (20)     1708 2024-01-08 18:43:54.000000 mintalib-0.0.7/src/mintalib.egg-info/SOURCES.txt
--rw-r--r--   0 frederic   (501) staff       (20)        1 2024-01-08 18:43:54.000000 mintalib-0.0.7/src/mintalib.egg-info/dependency_links.txt
--rw-r--r--   0 frederic   (501) staff       (20)       60 2024-01-08 18:43:54.000000 mintalib-0.0.7/src/mintalib.egg-info/requires.txt
--rw-r--r--   0 frederic   (501) staff       (20)        9 2024-01-08 18:43:54.000000 mintalib-0.0.7/src/mintalib.egg-info/top_level.txt
-drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-01-08 18:43:54.704618 mintalib-0.0.7/tests/
--rw-r--r--   0 frederic   (501) staff       (20)     1800 2023-12-31 16:26:47.000000 mintalib-0.0.7/tests/test_mintalib.py
+drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-04-26 01:16:11.218821 mintalib-0.0.8/
+-rw-r--r--   0 frederic   (501) staff       (20)     1080 2023-11-27 20:51:02.000000 mintalib-0.0.8/LICENSE.txt
+-rw-r--r--   0 frederic   (501) staff       (20)      111 2023-12-31 16:09:00.000000 mintalib-0.0.8/MANIFEST.in
+-rw-r--r--   0 frederic   (501) staff       (20)     8954 2024-04-26 01:16:11.218589 mintalib-0.0.8/PKG-INFO
+-rw-r--r--   0 frederic   (501) staff       (20)     8195 2024-04-26 00:50:51.000000 mintalib-0.0.8/README.md
+-rwxr-xr-x   0 frederic   (501) staff       (20)      867 2024-04-26 00:42:10.000000 mintalib-0.0.8/pyproject.toml
+-rw-r--r--   0 frederic   (501) staff       (20)       38 2024-04-26 01:16:11.218860 mintalib-0.0.8/setup.cfg
+-rwxr-xr-x   0 frederic   (501) staff       (20)      812 2024-01-20 10:18:46.000000 mintalib-0.0.8/setup.py
+drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-04-26 01:16:11.209140 mintalib-0.0.8/src/
+drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-04-26 01:16:11.212576 mintalib-0.0.8/src/mintalib/
+-rw-r--r--   0 frederic   (501) staff       (20)       19 2023-12-31 16:24:09.000000 mintalib-0.0.8/src/mintalib/__init__.py
+-rw-r--r--   0 frederic   (501) staff       (20)  3484579 2024-04-26 00:57:09.000000 mintalib-0.0.8/src/mintalib/core.c
+-rw-r--r--   0 frederic   (501) staff       (20)      248 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/core.pyx
+drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-04-26 01:16:11.217571 mintalib-0.0.8/src/mintalib/cython/
+-rwxr-xr-x   0 frederic   (501) staff       (20)        0 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/__init__.py
+-rw-r--r--   0 frederic   (501) staff       (20)      750 2024-04-26 00:44:13.000000 mintalib-0.0.8/src/mintalib/cython/_all_core.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     2678 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/_common.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     2172 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/adx.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     2638 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/atr.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      709 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/bbands.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      692 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/bop.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      537 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/cci.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      791 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/cmf.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1606 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/cross.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      534 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/dema.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      814 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/diff.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1955 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/ema.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      371 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/eval.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      473 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/exp.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     4841 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/flags.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     2676 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/kama.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      718 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/keltner.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      468 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/log.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      759 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/macd.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1245 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/mad.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1188 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/matype.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      988 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/max.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      673 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/mfi.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      989 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/min.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      788 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/ppo.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     3732 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/price.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1384 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/rma.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      902 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/roc.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1421 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/rsi.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     2049 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/sar.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     3527 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/slope.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1179 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/sma.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1155 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/stdev.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1017 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/stoch.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1781 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/streak.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1086 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/sum.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      656 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/tema.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)     1061 2023-11-27 20:51:02.000000 mintalib-0.0.8/src/mintalib/cython/wma.pxi
+-rw-r--r--   0 frederic   (501) staff       (20)      745 2024-04-26 00:51:57.000000 mintalib-0.0.8/src/mintalib/functions.py
+-rw-r--r--   0 frederic   (501) staff       (20)     1111 2023-12-31 16:24:09.000000 mintalib-0.0.8/src/mintalib/helper.py
+-rw-r--r--   0 frederic   (501) staff       (20)    14706 2024-04-26 00:51:36.000000 mintalib-0.0.8/src/mintalib/indicators.py
+-rw-r--r--   0 frederic   (501) staff       (20)     1723 2023-12-31 16:24:09.000000 mintalib-0.0.8/src/mintalib/model.py
+-rw-r--r--   0 frederic   (501) staff       (20)     2981 2024-04-26 00:46:23.000000 mintalib-0.0.8/src/mintalib/reflib.py
+drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-04-26 01:16:11.217815 mintalib-0.0.8/src/mintalib/samples/
+-rw-r--r--   0 frederic   (501) staff       (20)     1673 2024-01-08 14:27:54.000000 mintalib-0.0.8/src/mintalib/samples/__init__.py
+-rw-r--r--   0 frederic   (501) staff       (20)   145504 2024-01-08 14:00:59.000000 mintalib-0.0.8/src/mintalib/samples/sample-prices.csv
+-rw-r--r--   0 frederic   (501) staff       (20)     2879 2023-12-31 16:24:09.000000 mintalib-0.0.8/src/mintalib/utils.py
+drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-04-26 01:16:11.218182 mintalib-0.0.8/src/mintalib.egg-info/
+-rw-r--r--   0 frederic   (501) staff       (20)     8954 2024-04-26 01:16:11.000000 mintalib-0.0.8/src/mintalib.egg-info/PKG-INFO
+-rw-r--r--   0 frederic   (501) staff       (20)     1678 2024-04-26 01:16:11.000000 mintalib-0.0.8/src/mintalib.egg-info/SOURCES.txt
+-rw-r--r--   0 frederic   (501) staff       (20)        1 2024-04-26 01:16:11.000000 mintalib-0.0.8/src/mintalib.egg-info/dependency_links.txt
+-rw-r--r--   0 frederic   (501) staff       (20)       60 2024-04-26 01:16:11.000000 mintalib-0.0.8/src/mintalib.egg-info/requires.txt
+-rw-r--r--   0 frederic   (501) staff       (20)        9 2024-04-26 01:16:11.000000 mintalib-0.0.8/src/mintalib.egg-info/top_level.txt
+drwxr-xr-x   0 frederic   (501) staff       (20)        0 2024-04-26 01:16:11.218021 mintalib-0.0.8/tests/
+-rw-r--r--   0 frederic   (501) staff       (20)     1800 2023-12-31 16:26:47.000000 mintalib-0.0.8/tests/test_mintalib.py
```

### Comparing `mintalib-0.0.7/LICENSE.txt` & `mintalib-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/PKG-INFO` & `mintalib-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mintalib
-Version: 0.0.7
+Version: 0.0.8
 Summary: Minimal Technical Analysis Library for Python
 Author-email: Furechan <furechan@xsmail.com>
-License: MIT
+License: MIT License
 Project-URL: homepage, https://github.com/furechan/mintalib
 Keywords: python,cython,finance,technical-analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -26,17 +26,17 @@
 This library offers a curated list of technical analysis indicators
 implemented in cython.
 It is built around `numpy` arrays and aims to be compatible
 with both `pandas` and `polars` dataframes where possible.
 
 
 > **Warning**
-> This is work in progress.
-> For a similar project with a mature api
-> you may want to look at [ta-lib](https://pypi.org/project/TA-Lib/).
+> This project is experimental and the interface can change.
+> For a similar project with a mature api you may want to look at
+> [ta-lib](https://pypi.org/project/TA-Lib/).
 
 
 ## Structure
 The `mintalib` package contains three main modules:
 - `mintalib.core` low level calculation rountines implemented in cython
 - `mintalib.functions` single use functions to compute indicators
 - `mintalib.indicators` composable interface to indicators
@@ -149,15 +149,14 @@
 | AVGPRICE         | Average Price                             |
 | BBANDS           | Bollinger Bands                           |
 | BOP              | Balance of Power                          |
 | CCI              | Commodity Channel Index                   |
 | CMF              | Chaikin Money Flow                        |
 | CROSSOVER        | Cross Over                                |
 | CROSSUNDER       | Cross Under                               |
-| CURVE            | Curve (time curvilinear regression)       |
 | DEMA             | Double Exponential Moving Average         |
 | DIFF             | Difference                                |
 | EFFICIENCY_RATIO | Efficiency Ratio (Kaufman)                |
 | EMA              | Exponential Moving Average                |
 | EVAL             | Expression Eval (pandas only)             |
 | EXP              | Exponential                               |
 | FLAG_ABOVE       | Flag for value above level                |
```

### Comparing `mintalib-0.0.7/README.md` & `mintalib-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 This library offers a curated list of technical analysis indicators
 implemented in cython.
 It is built around `numpy` arrays and aims to be compatible
 with both `pandas` and `polars` dataframes where possible.
 
 
 > **Warning**
-> This is work in progress.
-> For a similar project with a mature api
-> you may want to look at [ta-lib](https://pypi.org/project/TA-Lib/).
+> This project is experimental and the interface can change.
+> For a similar project with a mature api you may want to look at
+> [ta-lib](https://pypi.org/project/TA-Lib/).
 
 
 ## Structure
 The `mintalib` package contains three main modules:
 - `mintalib.core` low level calculation rountines implemented in cython
 - `mintalib.functions` single use functions to compute indicators
 - `mintalib.indicators` composable interface to indicators
@@ -127,15 +127,14 @@
 | AVGPRICE         | Average Price                             |
 | BBANDS           | Bollinger Bands                           |
 | BOP              | Balance of Power                          |
 | CCI              | Commodity Channel Index                   |
 | CMF              | Chaikin Money Flow                        |
 | CROSSOVER        | Cross Over                                |
 | CROSSUNDER       | Cross Under                               |
-| CURVE            | Curve (time curvilinear regression)       |
 | DEMA             | Double Exponential Moving Average         |
 | DIFF             | Difference                                |
 | EFFICIENCY_RATIO | Efficiency Ratio (Kaufman)                |
 | EMA              | Exponential Moving Average                |
 | EVAL             | Expression Eval (pandas only)             |
 | EXP              | Exponential                               |
 | FLAG_ABOVE       | Flag for value above level                |
```

### Comparing `mintalib-0.0.7/pyproject.toml` & `mintalib-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools", "cython"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mintalib"
-version = "0.0.7"
+version = "0.0.8"
 readme = "README.md"
 requires-python = ">=3.9"
-license = { text = "MIT" }
+license = { text = "MIT License" }
 description = "Minimal Technical Analysis Library for Python"
 urls = { homepage = "https://github.com/furechan/mintalib" }
 authors = [{ name = "Furechan", email = "furechan@xsmail.com" }]
 dependencies = ["numpy", "pandas"]
 keywords = ["python", "cython", "finance", "technical-analysis"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `mintalib-0.0.7/setup.py` & `mintalib-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/core.c` & `mintalib-0.0.8/src/mintalib/core.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.7 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-Wno-unreachable-code",
@@ -37,18 +37,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_7" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030007F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -132,14 +132,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -193,14 +195,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -254,60 +258,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -390,14 +417,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -582,22 +612,22 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
         #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
         Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
@@ -647,15 +677,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -733,16 +763,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1086,15 +1121,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1173,15 +1208,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1280,32 +1315,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1347,15 +1365,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1502,15 +1520,14 @@
   "src/mintalib/cython/bop.pxi",
   "src/mintalib/cython/bbands.pxi",
   "src/mintalib/cython/keltner.pxi",
   "src/mintalib/cython/kama.pxi",
   "src/mintalib/cython/macd.pxi",
   "src/mintalib/cython/ppo.pxi",
   "src/mintalib/cython/slope.pxi",
-  "src/mintalib/cython/curve.pxi",
   "src/mintalib/cython/stoch.pxi",
   "src/mintalib/cython/streak.pxi",
   "src/mintalib/cython/eval.pxi",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
@@ -1735,16 +1752,14 @@
 typedef struct __pyx_defaults32 __pyx_defaults32;
 struct __pyx_defaults33;
 typedef struct __pyx_defaults33 __pyx_defaults33;
 struct __pyx_defaults34;
 typedef struct __pyx_defaults34 __pyx_defaults34;
 struct __pyx_defaults35;
 typedef struct __pyx_defaults35 __pyx_defaults35;
-struct __pyx_defaults36;
-typedef struct __pyx_defaults36 __pyx_defaults36;
 
 /* "src/mintalib/cython/slope.pxi":3
  * """ Slope (time linear regression) """
  * 
  * cdef enum:             # <<<<<<<<<<<<<<
  *     SLOPE_OPTION_SLOPE = 0
  *     SLOPE_OPTION_INTERCEPT = 1
@@ -1754,30 +1769,14 @@
   __pyx_e_8mintalib_4core_SLOPE_OPTION_INTERCEPT = 1,
   __pyx_e_8mintalib_4core_SLOPE_OPTION_RVALUE = 2,
   __pyx_e_8mintalib_4core_SLOPE_OPTION_RSQUARE = 3,
   __pyx_e_8mintalib_4core_SLOPE_OPTION_RMSERROR = 4,
   __pyx_e_8mintalib_4core_SLOPE_OPTION_FORECAST = 5,
   __pyx_e_8mintalib_4core_SLOPE_OPTION_BADOPTION = 6
 };
-
-/* "src/mintalib/cython/curve.pxi":4
- * 
- * 
- * cdef enum:             # <<<<<<<<<<<<<<
- *     CURVE_OPTION_CURVE = 0
- *     CURVE_OPTION_SLOPE = 1
- */
-enum  {
-  __pyx_e_8mintalib_4core_CURVE_OPTION_CURVE = 0,
-  __pyx_e_8mintalib_4core_CURVE_OPTION_SLOPE = 1,
-  __pyx_e_8mintalib_4core_CURVE_OPTION_RVALUE = 2,
-  __pyx_e_8mintalib_4core_CURVE_OPTION_RSQUARE = 3,
-  __pyx_e_8mintalib_4core_CURVE_OPTION_RMSERROR = 4,
-  __pyx_e_8mintalib_4core_CURVE_OPTION_BADOPTION = 5
-};
 struct __pyx_defaults {
   double __pyx_arg_na_value;
 };
 struct __pyx_defaults1 {
   double __pyx_arg_na_value;
 };
 struct __pyx_defaults2 {
@@ -1896,17 +1895,14 @@
 };
 struct __pyx_defaults34 {
   PyObject *__pyx_arg_period;
   PyObject *__pyx_arg_offset;
 };
 struct __pyx_defaults35 {
   PyObject *__pyx_arg_period;
-};
-struct __pyx_defaults36 {
-  PyObject *__pyx_arg_period;
   PyObject *__pyx_arg_fastn;
   PyObject *__pyx_arg_slown;
 };
 
 /* "src/mintalib/cython/_common.pxi":57
  * 
  * 
@@ -2365,16 +2361,16 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
@@ -2382,16 +2378,17 @@
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
     CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2856,15 +2853,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -3549,15 +3546,14 @@
 static const char __pyx_k_ph[] = "ph";
 static const char __pyx_k_pl[] = "pl";
 static const char __pyx_k_pv[] = "pv";
 static const char __pyx_k_px[] = "px";
 static const char __pyx_k_py[] = "py";
 static const char __pyx_k_sx[] = "sx";
 static const char __pyx_k_sy[] = "sy";
-static const char __pyx_k_sz[] = "sz";
 static const char __pyx_k_tr[] = "tr";
 static const char __pyx_k_up[] = "up";
 static const char __pyx_k_xs[] = "xs";
 static const char __pyx_k_ys[] = "ys";
 static const char __pyx_k_zs[] = "zs";
 static const char __pyx_k_ADX[] = "ADX";
 static const char __pyx_k_ATR[] = "ATR";
@@ -3619,39 +3615,33 @@
 static const char __pyx_k_rsi[] = "rsi";
 static const char __pyx_k_sar[] = "sar";
 static const char __pyx_k_sma[] = "sma";
 static const char __pyx_k_std[] = "std";
 static const char __pyx_k_str[] = "str";
 static const char __pyx_k_sxx[] = "sxx";
 static const char __pyx_k_sxy[] = "sxy";
-static const char __pyx_k_sxz[] = "sxz";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_syy[] = "syy";
-static const char __pyx_k_syz[] = "syz";
-static const char __pyx_k_szz[] = "szz";
 static const char __pyx_k_typ[] = "typ";
 static const char __pyx_k_ups[] = "ups";
 static const char __pyx_k_vxx[] = "vxx";
 static const char __pyx_k_vxy[] = "vxy";
-static const char __pyx_k_vxz[] = "vxz";
 static const char __pyx_k_vyy[] = "vyy";
-static const char __pyx_k_vyz[] = "vyz";
-static const char __pyx_k_vzz[] = "vzz";
 static const char __pyx_k_wcl[] = "wcl";
 static const char __pyx_k_yes[] = "yes";
 static const char __pyx_k_DEMA[] = "DEMA";
 static const char __pyx_k_DIFF[] = "DIFF";
 static const char __pyx_k_EVAL[] = "EVAL";
 static const char __pyx_k_KAMA[] = "KAMA";
 static const char __pyx_k_LATR[] = "LATR";
 static const char __pyx_k_MACD[] = "MACD";
 static const char __pyx_k_NATR[] = "NATR";
 static const char __pyx_k_None[] = "None";
 static const char __pyx_k_TEMA[] = "TEMA";
-static const char __pyx_k__221[] = "?";
+static const char __pyx_k__217[] = "?";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_bool[] = "bool";
 static const char __pyx_k_clip[] = "clip";
 static const char __pyx_k_core[] = ".core";
 static const char __pyx_k_corr[] = "corr";
 static const char __pyx_k_data[] = "data";
@@ -3684,34 +3674,31 @@
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_prev[] = "prev";
 static const char __pyx_k_repr[] = "__repr__";
 static const char __pyx_k_rmse[] = "rmse";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_send[] = "send";
 static const char __pyx_k_size[] = "size";
-static const char __pyx_k_skip[] = "skip";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_vsum[] = "vsum";
 static const char __pyx_k_wrap[] = "wrap";
 static const char __pyx_k_wsum[] = "wsum";
 static const char __pyx_k_ASCII[] = "ASCII";
-static const char __pyx_k_CURVE[] = "CURVE";
 static const char __pyx_k_PRICE[] = "PRICE";
 static const char __pyx_k_SLOPE[] = "SLOPE";
 static const char __pyx_k_STDEV[] = "STDEV";
 static const char __pyx_k_STOCH[] = "STOCH";
 static const char __pyx_k_all_2[] = "__all__";
 static const char __pyx_k_alpha[] = "alpha";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_count[] = "count";
-static const char __pyx_k_curve[] = "curve";
 static const char __pyx_k_doc_2[] = "doc";
 static const char __pyx_k_downs[] = "downs";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_enter[] = "__enter__";
 static const char __pyx_k_ercnt[] = "ercnt";
 static const char __pyx_k_erdiv[] = "erdiv";
 static const char __pyx_k_ernum[] = "ernum";
@@ -3777,15 +3764,14 @@
 static const char __pyx_k_pandas[] = "pandas";
 static const char __pyx_k_period[] = "period";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_polars[] = "polars";
 static const char __pyx_k_prices[] = "prices";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_result[] = "result";
-static const char __pyx_k_rvalue[] = "rvalue";
 static const char __pyx_k_series[] = "series";
 static const char __pyx_k_signal[] = "signal";
 static const char __pyx_k_source[] = "source";
 static const char __pyx_k_streak[] = "streak";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_trange[] = "trange";
 static const char __pyx_k_unpack[] = "unpack";
@@ -3807,15 +3793,14 @@
 static const char __pyx_k_islower[] = "islower";
 static const char __pyx_k_ma_type[] = "ma_type";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_modules[] = "modules";
 static const char __pyx_k_ndarray[] = "ndarray";
 static const char __pyx_k_percent[] = "percent";
 static const char __pyx_k_prepare[] = "__prepare__";
-static const char __pyx_k_rsquare[] = "rsquare";
 static const char __pyx_k_up_flag[] = "up_flag";
 static const char __pyx_k_use_log[] = "use_log";
 static const char __pyx_k_AVGPRICE[] = "AVGPRICE";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_FORECAST[] = "FORECAST";
 static const char __pyx_k_MIDPRICE[] = "MIDPRICE";
 static const char __pyx_k_RMSERROR[] = "RMSERROR";
@@ -3879,15 +3864,14 @@
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_streak_up[] = "streak_up";
 static const char __pyx_k_CROSSUNDER[] = "CROSSUNDER";
 static const char __pyx_k_FLAG_ABOVE[] = "FLAG_ABOVE";
 static const char __pyx_k_FLAG_BELOW[] = "FLAG_BELOW";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
-static const char __pyx_k_calc_curve[] = "calc_curve";
 static const char __pyx_k_calc_price[] = "calc_price";
 static const char __pyx_k_calc_slope[] = "calc_slope";
 static const char __pyx_k_calc_stdev[] = "calc_stdev";
 static const char __pyx_k_calc_stoch[] = "calc_stoch";
 static const char __pyx_k_check_size[] = "check_size";
 static const char __pyx_k_crossunder[] = "crossunder";
 static const char __pyx_k_down_level[] = "down_level";
@@ -3899,15 +3883,14 @@
 static const char __pyx_k_ppo_result[] = "ppo_result";
 static const char __pyx_k_price_func[] = "price_func";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_same_scale[] = "same_scale";
 static const char __pyx_k_start_flag[] = "start_flag";
 static const char __pyx_k_where_flag[] = "where_flag";
-static const char __pyx_k_CurveOption[] = "CurveOption";
 static const char __pyx_k_INVERT_FLAG[] = "INVERT_FLAG";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_STREAK_DOWN[] = "STREAK_DOWN";
 static const char __pyx_k_SlopeOption[] = "SlopeOption";
 static const char __pyx_k_UPDOWN_FLAG[] = "UPDOWN_FLAG";
 static const char __pyx_k_calc_bbands[] = "calc_bbands";
@@ -3955,15 +3938,14 @@
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_EFFICIENCY_RATIO[] = "EFFICIENCY_RATIO";
 static const char __pyx_k_Invalid_option_d[] = "Invalid option %d";
 static const char __pyx_k_efficiency_ratio[] = "efficiency_ratio";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
-static const char __pyx_k_CurveOption___repr[] = "CurveOption.__repr__";
 static const char __pyx_k_SlopeOption___repr[] = "SlopeOption.__repr__";
 static const char __pyx_k_Unknown_price_type[] = "Unknown price type ";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
 static const char __pyx_k_Invalid_period_value[] = "Invalid period value ";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
@@ -3971,15 +3953,14 @@
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_ppo_pposignal_ppohist[] = "ppo, pposignal, ppohist";
 static const char __pyx_k_Cannot_get_series_from[] = "Cannot get series from ";
 static const char __pyx_k_Cannot_index_with_type[] = "Cannot index with type '";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
-static const char __pyx_k_Curve_Option_Enumeration[] = " Curve Option Enumeration ";
 static const char __pyx_k_Slope_Option_Enumeration[] = " Slope Option Enumeration ";
 static const char __pyx_k_macd_macdsignal_macdhist[] = "macd, macdsignal, macdhist";
 static const char __pyx_k_Dimension_d_is_not_direct[] = "Dimension %d is not direct";
 static const char __pyx_k_Index_out_of_bounds_axis_d[] = "Index out of bounds (axis %d)";
 static const char __pyx_k_Step_may_not_be_zero_axis_d[] = "Step may not be zero (axis %d)";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_src_mintalib_cython_adx_pxi[] = "src/mintalib/cython/adx.pxi";
@@ -4005,15 +3986,14 @@
 static const char __pyx_k_src_mintalib_cython_dema_pxi[] = "src/mintalib/cython/dema.pxi";
 static const char __pyx_k_src_mintalib_cython_diff_pxi[] = "src/mintalib/cython/diff.pxi";
 static const char __pyx_k_src_mintalib_cython_eval_pxi[] = "src/mintalib/cython/eval.pxi";
 static const char __pyx_k_src_mintalib_cython_kama_pxi[] = "src/mintalib/cython/kama.pxi";
 static const char __pyx_k_src_mintalib_cython_macd_pxi[] = "src/mintalib/cython/macd.pxi";
 static const char __pyx_k_src_mintalib_cython_tema_pxi[] = "src/mintalib/cython/tema.pxi";
 static const char __pyx_k_src_mintalib_cython_cross_pxi[] = "src/mintalib/cython/cross.pxi";
-static const char __pyx_k_src_mintalib_cython_curve_pxi[] = "src/mintalib/cython/curve.pxi";
 static const char __pyx_k_src_mintalib_cython_flags_pxi[] = "src/mintalib/cython/flags.pxi";
 static const char __pyx_k_src_mintalib_cython_price_pxi[] = "src/mintalib/cython/price.pxi";
 static const char __pyx_k_src_mintalib_cython_slope_pxi[] = "src/mintalib/cython/slope.pxi";
 static const char __pyx_k_src_mintalib_cython_stdev_pxi[] = "src/mintalib/cython/stdev.pxi";
 static const char __pyx_k_src_mintalib_cython_stoch_pxi[] = "src/mintalib/cython/stoch.pxi";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_src_mintalib_cython_bbands_pxi[] = "src/mintalib/cython/bbands.pxi";
@@ -4037,15 +4017,15 @@
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got ";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis ";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension ";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_8mintalib_4core_226genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_222genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -4101,146 +4081,142 @@
 static PyObject *__pyx_pf_8mintalib_4core_26WCLPRICE(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_28MIDPRICE(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_30PRICE(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_32crossover(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_level, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_34crossunder(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_level, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_36CROSSOVER(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_level, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_38CROSSUNDER(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_level, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_229__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_225__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_40flag_above(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_level, double __pyx_v_na_value, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_231__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_227__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_42flag_below(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_level, double __pyx_v_na_value, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_233__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_229__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_44invert_flag(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_na_value, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_235__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_231__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_46updown_flag(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_up_level, double __pyx_v_down_level, double __pyx_v_up_flag, double __pyx_v_down_flag, double __pyx_v_start_flag, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_237__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_233__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_48where_flag(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_flag, PyObject *__pyx_v_x, PyObject *__pyx_v_y, PyObject *__pyx_v_z, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_239__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_235__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_50FLAG_ABOVE(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_level, double __pyx_v_na_value, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_241__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_237__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_52FLAG_BELOW(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_level, double __pyx_v_na_value, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_243__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_239__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_54INVERT_FLAG(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_na_value, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_245__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_241__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_56UPDOWN_FLAG(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, double __pyx_v_up_level, double __pyx_v_down_level, double __pyx_v_up_flag, double __pyx_v_down_flag, double __pyx_v_start_flag, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_58calc_log(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_60LOG(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_62calc_exp(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_64EXP(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_66calc_roc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_247__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_243__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_68ROC(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_70calc_diff(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_249__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_245__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_72DIFF(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_74calc_min(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_76MIN(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_78calc_max(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_80MAX(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_82calc_sum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_84SUM(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_86calc_mad(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_251__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_247__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_88MAD(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_90calc_stdev(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_253__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_249__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_92STDEV(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_94calc_sma(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_96SMA(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_98calc_ema(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, int __pyx_v_adjust, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_100EMA(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_adjust, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_102calc_rma(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_104RMA(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_106calc_wma(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_108WMA(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_110calc_dema(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_112DEMA(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_114calc_tema(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_255__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_251__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_116TEMA(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_118calc_ma(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_ma_type, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_257__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_253__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_120MA(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_ma_type, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_122calc_rsi(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_259__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_255__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_124RSI(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_126calc_plusdi(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_128calc_minusdi(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_130calc_adx(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_261__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_257__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_132PLUSDI(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_263__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_259__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_134MINUSDI(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_265__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_261__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_136ADX(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_138calc_trange(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_log_prices, PyObject *__pyx_v_percent, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_140calc_atr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_142calc_natr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_144calc_latr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_146TRANGE(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_log_prices, PyObject *__pyx_v_percent); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_267__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_263__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_148ATR(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_269__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_265__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_150NATR(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_271__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_267__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_152LATR(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_154calc_sar(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, double __pyx_v_afs, double __pyx_v_maxaf, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_156SAR(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, double __pyx_v_afs, double __pyx_v_maxaf); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_158calc_cci(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_273__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_269__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_160CCI(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_162calc_cmf(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_275__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_271__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_164CMF(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_166calc_mfi(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_277__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_273__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_168MFI(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_170calc_bop(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_279__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_275__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_172BOP(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_174calc_bbands(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, double __pyx_v_nbdev, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_281__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_277__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_176BBANDS(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period, double __pyx_v_nbdev); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_178calc_keltner(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, double __pyx_v_nbatr, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_283__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_279__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_180KELTNER(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period, double __pyx_v_nbatr); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_182efficiency_ratio(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, int __pyx_v_period, PyObject *__pyx_v_wrap); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_184calc_kama(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, int __pyx_v_period, int __pyx_v_fastn, int __pyx_v_slown, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_285__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_281__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_186EFFICIENCY_RATIO(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_287__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_283__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_188KAMA(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_fastn, PyObject *__pyx_v_slown, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_190calc_macd(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_n1, long __pyx_v_n2, long __pyx_v_n3, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_289__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_285__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_192MACD(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_n1, PyObject *__pyx_v_n2, PyObject *__pyx_v_n3, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_194calc_ppo(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_n1, long __pyx_v_n2, long __pyx_v_n3, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_291__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_287__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_196PPO(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_n1, PyObject *__pyx_v_n2, PyObject *__pyx_v_n3, PyObject *__pyx_v_item); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_11SlopeOption___repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_198calc_slope(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, int __pyx_v_option, int __pyx_v_offset, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_293__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_289__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_200SLOPE(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_295__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_291__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_202RVALUE(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_297__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_293__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8mintalib_4core_204FORECAST(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_offset, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_11CurveOption___repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_206calc_curve(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, int __pyx_v_option, CYTHON_UNUSED int __pyx_v_offset, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_299__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_208CURVE(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_210calc_stoch(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, long __pyx_v_fastn, long __pyx_v_slown, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_301__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_212STOCH(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period, PyObject *__pyx_v_fastn, PyObject *__pyx_v_slown); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_214streak_up(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_216streak_down(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_wrap); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_218STREAK_UP(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_220STREAK_DOWN(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_item); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_222calc_eval(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_expr); /* proto */
-static PyObject *__pyx_pf_8mintalib_4core_224EVAL(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_expr); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_206calc_stoch(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, long __pyx_v_fastn, long __pyx_v_slown, PyObject *__pyx_v_wrap); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_295__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_208STOCH(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period, PyObject *__pyx_v_fastn, PyObject *__pyx_v_slown); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_210streak_up(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_wrap); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_212streak_down(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_wrap); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_214STREAK_UP(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_item); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_216STREAK_DOWN(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_item); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_218calc_eval(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_expr); /* proto */
+static PyObject *__pyx_pf_8mintalib_4core_220EVAL(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_expr); /* proto */
 static PyObject *__pyx_tp_new_8mintalib_4core___pyx_scope_struct__wrap_function(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_8mintalib_4core___pyx_scope_struct_1_wrap_indicator(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_8mintalib_4core___pyx_scope_struct_2_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -4302,24 +4278,20 @@
   PyObject *__pyx_n_s_BBANDS;
   PyObject *__pyx_n_s_BOP;
   PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
   PyObject *__pyx_n_s_CCI;
   PyObject *__pyx_n_s_CMF;
   PyObject *__pyx_n_s_CROSSOVER;
   PyObject *__pyx_n_s_CROSSUNDER;
-  PyObject *__pyx_n_s_CURVE;
   PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
   PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
   PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
   PyObject *__pyx_kp_u_Cannot_get_series_from;
   PyObject *__pyx_kp_u_Cannot_index_with_type;
   PyObject *__pyx_kp_s_Cannot_transpose_memoryview_with;
-  PyObject *__pyx_n_s_CurveOption;
-  PyObject *__pyx_n_s_CurveOption___repr;
-  PyObject *__pyx_kp_s_Curve_Option_Enumeration;
   PyObject *__pyx_n_s_DEMA;
   PyObject *__pyx_n_u_DEMA;
   PyObject *__pyx_n_s_DIFF;
   PyObject *__pyx_n_s_DataFrame;
   PyObject *__pyx_kp_u_Different_sizes;
   PyObject *__pyx_kp_s_Dimension_d_is_not_direct;
   PyObject *__pyx_n_s_EFFICIENCY_RATIO;
@@ -4401,15 +4373,15 @@
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_View_MemoryView;
   PyObject *__pyx_n_s_WCLPRICE;
   PyObject *__pyx_n_s_WMA;
   PyObject *__pyx_n_u_WMA;
   PyObject *__pyx_kp_u__15;
   PyObject *__pyx_kp_u__2;
-  PyObject *__pyx_n_s__221;
+  PyObject *__pyx_n_s__217;
   PyObject *__pyx_n_s__3;
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_kp_u__7;
   PyObject *__pyx_n_s_abc;
   PyObject *__pyx_n_s_abs;
   PyObject *__pyx_n_s_adjust;
   PyObject *__pyx_n_s_af;
@@ -4438,15 +4410,14 @@
   PyObject *__pyx_n_s_calc_adx;
   PyObject *__pyx_n_s_calc_atr;
   PyObject *__pyx_n_s_calc_avgprice;
   PyObject *__pyx_n_s_calc_bbands;
   PyObject *__pyx_n_s_calc_bop;
   PyObject *__pyx_n_s_calc_cci;
   PyObject *__pyx_n_s_calc_cmf;
-  PyObject *__pyx_n_s_calc_curve;
   PyObject *__pyx_n_s_calc_dema;
   PyObject *__pyx_n_s_calc_diff;
   PyObject *__pyx_n_s_calc_ema;
   PyObject *__pyx_n_s_calc_eval;
   PyObject *__pyx_n_s_calc_exp;
   PyObject *__pyx_n_s_calc_kama;
   PyObject *__pyx_n_s_calc_keltner;
@@ -4492,15 +4463,14 @@
   PyObject *__pyx_kp_s_contiguous_and_direct;
   PyObject *__pyx_kp_s_contiguous_and_indirect;
   PyObject *__pyx_kp_u_core;
   PyObject *__pyx_n_s_corr;
   PyObject *__pyx_n_s_count;
   PyObject *__pyx_n_s_crossover;
   PyObject *__pyx_n_s_crossunder;
-  PyObject *__pyx_n_s_curve;
   PyObject *__pyx_n_s_data;
   PyObject *__pyx_kp_u_data_2;
   PyObject *__pyx_n_s_dataframe_like;
   PyObject *__pyx_n_s_decorator;
   PyObject *__pyx_n_s_default_item;
   PyObject *__pyx_n_s_di1;
   PyObject *__pyx_n_s_di2;
@@ -4703,30 +4673,27 @@
   PyObject *__pyx_n_s_res;
   PyObject *__pyx_n_s_result;
   PyObject *__pyx_n_s_rho;
   PyObject *__pyx_n_s_rma;
   PyObject *__pyx_n_s_rmse;
   PyObject *__pyx_n_s_roc;
   PyObject *__pyx_n_s_rsi;
-  PyObject *__pyx_n_s_rsquare;
-  PyObject *__pyx_n_s_rvalue;
   PyObject *__pyx_n_s_s;
   PyObject *__pyx_n_s_same_scale;
   PyObject *__pyx_n_u_same_scale;
   PyObject *__pyx_n_s_sar;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_n_s_send;
   PyObject *__pyx_n_s_series;
   PyObject *__pyx_n_s_set_name;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_shape;
   PyObject *__pyx_n_s_signal;
   PyObject *__pyx_n_s_size;
-  PyObject *__pyx_n_s_skip;
   PyObject *__pyx_n_s_slope;
   PyObject *__pyx_n_s_slowd;
   PyObject *__pyx_n_s_slowf;
   PyObject *__pyx_n_s_slowk;
   PyObject *__pyx_kp_u_slowk_slowd;
   PyObject *__pyx_n_s_slown;
   PyObject *__pyx_n_s_sma;
@@ -4736,15 +4703,14 @@
   PyObject *__pyx_kp_s_src_mintalib_cython_adx_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_atr_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_bbands_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_bop_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_cci_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_cmf_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_cross_pxi;
-  PyObject *__pyx_kp_s_src_mintalib_cython_curve_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_dema_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_diff_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_ema_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_eval_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_exp_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_flags_pxi;
   PyObject *__pyx_kp_s_src_mintalib_cython_kama_pxi;
@@ -4786,21 +4752,17 @@
   PyObject *__pyx_kp_s_strided_and_indirect;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_struct;
   PyObject *__pyx_n_s_super;
   PyObject *__pyx_n_s_sx;
   PyObject *__pyx_n_s_sxx;
   PyObject *__pyx_n_s_sxy;
-  PyObject *__pyx_n_s_sxz;
   PyObject *__pyx_n_s_sy;
   PyObject *__pyx_n_s_sys;
   PyObject *__pyx_n_s_syy;
-  PyObject *__pyx_n_s_syz;
-  PyObject *__pyx_n_s_sz;
-  PyObject *__pyx_n_s_szz;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_throw;
   PyObject *__pyx_n_s_tname;
   PyObject *__pyx_n_s_total;
   PyObject *__pyx_n_s_tr;
   PyObject *__pyx_n_s_trange;
   PyObject *__pyx_n_s_trend;
@@ -4822,18 +4784,15 @@
   PyObject *__pyx_n_s_value;
   PyObject *__pyx_n_s_version_info;
   PyObject *__pyx_n_s_volume;
   PyObject *__pyx_n_u_volume;
   PyObject *__pyx_n_s_vsum;
   PyObject *__pyx_n_s_vxx;
   PyObject *__pyx_n_s_vxy;
-  PyObject *__pyx_n_s_vxz;
   PyObject *__pyx_n_s_vyy;
-  PyObject *__pyx_n_s_vyz;
-  PyObject *__pyx_n_s_vzz;
   PyObject *__pyx_n_s_wcl;
   PyObject *__pyx_n_s_where;
   PyObject *__pyx_n_s_where_flag;
   PyObject *__pyx_n_s_wrap;
   PyObject *__pyx_n_s_wrap_function;
   PyObject *__pyx_n_s_wrap_function_locals_decorator;
   PyObject *__pyx_n_s_wrap_indicator;
@@ -4952,21 +4911,20 @@
   PyObject *__pyx_tuple__187;
   PyObject *__pyx_tuple__189;
   PyObject *__pyx_tuple__191;
   PyObject *__pyx_tuple__192;
   PyObject *__pyx_tuple__195;
   PyObject *__pyx_tuple__197;
   PyObject *__pyx_tuple__201;
+  PyObject *__pyx_tuple__203;
   PyObject *__pyx_tuple__204;
-  PyObject *__pyx_tuple__207;
+  PyObject *__pyx_tuple__206;
   PyObject *__pyx_tuple__208;
-  PyObject *__pyx_tuple__210;
-  PyObject *__pyx_tuple__212;
-  PyObject *__pyx_tuple__217;
-  PyObject *__pyx_tuple__219;
+  PyObject *__pyx_tuple__213;
+  PyObject *__pyx_tuple__215;
   PyObject *__pyx_codeobj__12;
   PyObject *__pyx_codeobj__14;
   PyObject *__pyx_codeobj__27;
   PyObject *__pyx_codeobj__29;
   PyObject *__pyx_codeobj__31;
   PyObject *__pyx_codeobj__33;
   PyObject *__pyx_codeobj__36;
@@ -5066,25 +5024,22 @@
   PyObject *__pyx_codeobj__193;
   PyObject *__pyx_codeobj__194;
   PyObject *__pyx_codeobj__196;
   PyObject *__pyx_codeobj__198;
   PyObject *__pyx_codeobj__199;
   PyObject *__pyx_codeobj__200;
   PyObject *__pyx_codeobj__202;
-  PyObject *__pyx_codeobj__203;
   PyObject *__pyx_codeobj__205;
-  PyObject *__pyx_codeobj__206;
+  PyObject *__pyx_codeobj__207;
   PyObject *__pyx_codeobj__209;
+  PyObject *__pyx_codeobj__210;
   PyObject *__pyx_codeobj__211;
-  PyObject *__pyx_codeobj__213;
+  PyObject *__pyx_codeobj__212;
   PyObject *__pyx_codeobj__214;
-  PyObject *__pyx_codeobj__215;
   PyObject *__pyx_codeobj__216;
-  PyObject *__pyx_codeobj__218;
-  PyObject *__pyx_codeobj__220;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -5147,24 +5102,20 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_BBANDS);
   Py_CLEAR(clear_module_state->__pyx_n_s_BOP);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Buffer_view_does_not_expose_stri);
   Py_CLEAR(clear_module_state->__pyx_n_s_CCI);
   Py_CLEAR(clear_module_state->__pyx_n_s_CMF);
   Py_CLEAR(clear_module_state->__pyx_n_s_CROSSOVER);
   Py_CLEAR(clear_module_state->__pyx_n_s_CROSSUNDER);
-  Py_CLEAR(clear_module_state->__pyx_n_s_CURVE);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Can_only_create_a_buffer_that_is);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Cannot_assign_to_read_only_memor);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Cannot_create_writable_memory_vi);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Cannot_get_series_from);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Cannot_index_with_type);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Cannot_transpose_memoryview_with);
-  Py_CLEAR(clear_module_state->__pyx_n_s_CurveOption);
-  Py_CLEAR(clear_module_state->__pyx_n_s_CurveOption___repr);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_Curve_Option_Enumeration);
   Py_CLEAR(clear_module_state->__pyx_n_s_DEMA);
   Py_CLEAR(clear_module_state->__pyx_n_u_DEMA);
   Py_CLEAR(clear_module_state->__pyx_n_s_DIFF);
   Py_CLEAR(clear_module_state->__pyx_n_s_DataFrame);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Different_sizes);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Dimension_d_is_not_direct);
   Py_CLEAR(clear_module_state->__pyx_n_s_EFFICIENCY_RATIO);
@@ -5246,15 +5197,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_View_MemoryView);
   Py_CLEAR(clear_module_state->__pyx_n_s_WCLPRICE);
   Py_CLEAR(clear_module_state->__pyx_n_s_WMA);
   Py_CLEAR(clear_module_state->__pyx_n_u_WMA);
   Py_CLEAR(clear_module_state->__pyx_kp_u__15);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
-  Py_CLEAR(clear_module_state->__pyx_n_s__221);
+  Py_CLEAR(clear_module_state->__pyx_n_s__217);
   Py_CLEAR(clear_module_state->__pyx_n_s__3);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__7);
   Py_CLEAR(clear_module_state->__pyx_n_s_abc);
   Py_CLEAR(clear_module_state->__pyx_n_s_abs);
   Py_CLEAR(clear_module_state->__pyx_n_s_adjust);
   Py_CLEAR(clear_module_state->__pyx_n_s_af);
@@ -5283,15 +5234,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_adx);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_atr);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_avgprice);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_bbands);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_bop);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_cci);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_cmf);
-  Py_CLEAR(clear_module_state->__pyx_n_s_calc_curve);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_dema);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_diff);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_ema);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_eval);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_exp);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_kama);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_keltner);
@@ -5337,15 +5287,14 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_contiguous_and_direct);
   Py_CLEAR(clear_module_state->__pyx_kp_s_contiguous_and_indirect);
   Py_CLEAR(clear_module_state->__pyx_kp_u_core);
   Py_CLEAR(clear_module_state->__pyx_n_s_corr);
   Py_CLEAR(clear_module_state->__pyx_n_s_count);
   Py_CLEAR(clear_module_state->__pyx_n_s_crossover);
   Py_CLEAR(clear_module_state->__pyx_n_s_crossunder);
-  Py_CLEAR(clear_module_state->__pyx_n_s_curve);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_kp_u_data_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_dataframe_like);
   Py_CLEAR(clear_module_state->__pyx_n_s_decorator);
   Py_CLEAR(clear_module_state->__pyx_n_s_default_item);
   Py_CLEAR(clear_module_state->__pyx_n_s_di1);
   Py_CLEAR(clear_module_state->__pyx_n_s_di2);
@@ -5548,30 +5497,27 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_res);
   Py_CLEAR(clear_module_state->__pyx_n_s_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_rho);
   Py_CLEAR(clear_module_state->__pyx_n_s_rma);
   Py_CLEAR(clear_module_state->__pyx_n_s_rmse);
   Py_CLEAR(clear_module_state->__pyx_n_s_roc);
   Py_CLEAR(clear_module_state->__pyx_n_s_rsi);
-  Py_CLEAR(clear_module_state->__pyx_n_s_rsquare);
-  Py_CLEAR(clear_module_state->__pyx_n_s_rvalue);
   Py_CLEAR(clear_module_state->__pyx_n_s_s);
   Py_CLEAR(clear_module_state->__pyx_n_s_same_scale);
   Py_CLEAR(clear_module_state->__pyx_n_u_same_scale);
   Py_CLEAR(clear_module_state->__pyx_n_s_sar);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_n_s_send);
   Py_CLEAR(clear_module_state->__pyx_n_s_series);
   Py_CLEAR(clear_module_state->__pyx_n_s_set_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_shape);
   Py_CLEAR(clear_module_state->__pyx_n_s_signal);
   Py_CLEAR(clear_module_state->__pyx_n_s_size);
-  Py_CLEAR(clear_module_state->__pyx_n_s_skip);
   Py_CLEAR(clear_module_state->__pyx_n_s_slope);
   Py_CLEAR(clear_module_state->__pyx_n_s_slowd);
   Py_CLEAR(clear_module_state->__pyx_n_s_slowf);
   Py_CLEAR(clear_module_state->__pyx_n_s_slowk);
   Py_CLEAR(clear_module_state->__pyx_kp_u_slowk_slowd);
   Py_CLEAR(clear_module_state->__pyx_n_s_slown);
   Py_CLEAR(clear_module_state->__pyx_n_s_sma);
@@ -5581,15 +5527,14 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_adx_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_atr_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_bbands_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_bop_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_cci_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_cmf_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_cross_pxi);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_curve_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_dema_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_diff_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_ema_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_eval_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_exp_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_flags_pxi);
   Py_CLEAR(clear_module_state->__pyx_kp_s_src_mintalib_cython_kama_pxi);
@@ -5631,21 +5576,17 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_strided_and_indirect);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_struct);
   Py_CLEAR(clear_module_state->__pyx_n_s_super);
   Py_CLEAR(clear_module_state->__pyx_n_s_sx);
   Py_CLEAR(clear_module_state->__pyx_n_s_sxx);
   Py_CLEAR(clear_module_state->__pyx_n_s_sxy);
-  Py_CLEAR(clear_module_state->__pyx_n_s_sxz);
   Py_CLEAR(clear_module_state->__pyx_n_s_sy);
   Py_CLEAR(clear_module_state->__pyx_n_s_sys);
   Py_CLEAR(clear_module_state->__pyx_n_s_syy);
-  Py_CLEAR(clear_module_state->__pyx_n_s_syz);
-  Py_CLEAR(clear_module_state->__pyx_n_s_sz);
-  Py_CLEAR(clear_module_state->__pyx_n_s_szz);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_throw);
   Py_CLEAR(clear_module_state->__pyx_n_s_tname);
   Py_CLEAR(clear_module_state->__pyx_n_s_total);
   Py_CLEAR(clear_module_state->__pyx_n_s_tr);
   Py_CLEAR(clear_module_state->__pyx_n_s_trange);
   Py_CLEAR(clear_module_state->__pyx_n_s_trend);
@@ -5667,18 +5608,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_value);
   Py_CLEAR(clear_module_state->__pyx_n_s_version_info);
   Py_CLEAR(clear_module_state->__pyx_n_s_volume);
   Py_CLEAR(clear_module_state->__pyx_n_u_volume);
   Py_CLEAR(clear_module_state->__pyx_n_s_vsum);
   Py_CLEAR(clear_module_state->__pyx_n_s_vxx);
   Py_CLEAR(clear_module_state->__pyx_n_s_vxy);
-  Py_CLEAR(clear_module_state->__pyx_n_s_vxz);
   Py_CLEAR(clear_module_state->__pyx_n_s_vyy);
-  Py_CLEAR(clear_module_state->__pyx_n_s_vyz);
-  Py_CLEAR(clear_module_state->__pyx_n_s_vzz);
   Py_CLEAR(clear_module_state->__pyx_n_s_wcl);
   Py_CLEAR(clear_module_state->__pyx_n_s_where);
   Py_CLEAR(clear_module_state->__pyx_n_s_where_flag);
   Py_CLEAR(clear_module_state->__pyx_n_s_wrap);
   Py_CLEAR(clear_module_state->__pyx_n_s_wrap_function);
   Py_CLEAR(clear_module_state->__pyx_n_s_wrap_function_locals_decorator);
   Py_CLEAR(clear_module_state->__pyx_n_s_wrap_indicator);
@@ -5797,21 +5735,20 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__187);
   Py_CLEAR(clear_module_state->__pyx_tuple__189);
   Py_CLEAR(clear_module_state->__pyx_tuple__191);
   Py_CLEAR(clear_module_state->__pyx_tuple__192);
   Py_CLEAR(clear_module_state->__pyx_tuple__195);
   Py_CLEAR(clear_module_state->__pyx_tuple__197);
   Py_CLEAR(clear_module_state->__pyx_tuple__201);
+  Py_CLEAR(clear_module_state->__pyx_tuple__203);
   Py_CLEAR(clear_module_state->__pyx_tuple__204);
-  Py_CLEAR(clear_module_state->__pyx_tuple__207);
+  Py_CLEAR(clear_module_state->__pyx_tuple__206);
   Py_CLEAR(clear_module_state->__pyx_tuple__208);
-  Py_CLEAR(clear_module_state->__pyx_tuple__210);
-  Py_CLEAR(clear_module_state->__pyx_tuple__212);
-  Py_CLEAR(clear_module_state->__pyx_tuple__217);
-  Py_CLEAR(clear_module_state->__pyx_tuple__219);
+  Py_CLEAR(clear_module_state->__pyx_tuple__213);
+  Py_CLEAR(clear_module_state->__pyx_tuple__215);
   Py_CLEAR(clear_module_state->__pyx_codeobj__12);
   Py_CLEAR(clear_module_state->__pyx_codeobj__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__27);
   Py_CLEAR(clear_module_state->__pyx_codeobj__29);
   Py_CLEAR(clear_module_state->__pyx_codeobj__31);
   Py_CLEAR(clear_module_state->__pyx_codeobj__33);
   Py_CLEAR(clear_module_state->__pyx_codeobj__36);
@@ -5911,25 +5848,22 @@
   Py_CLEAR(clear_module_state->__pyx_codeobj__193);
   Py_CLEAR(clear_module_state->__pyx_codeobj__194);
   Py_CLEAR(clear_module_state->__pyx_codeobj__196);
   Py_CLEAR(clear_module_state->__pyx_codeobj__198);
   Py_CLEAR(clear_module_state->__pyx_codeobj__199);
   Py_CLEAR(clear_module_state->__pyx_codeobj__200);
   Py_CLEAR(clear_module_state->__pyx_codeobj__202);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__203);
   Py_CLEAR(clear_module_state->__pyx_codeobj__205);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__206);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__207);
   Py_CLEAR(clear_module_state->__pyx_codeobj__209);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__210);
   Py_CLEAR(clear_module_state->__pyx_codeobj__211);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__213);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__212);
   Py_CLEAR(clear_module_state->__pyx_codeobj__214);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__215);
   Py_CLEAR(clear_module_state->__pyx_codeobj__216);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__218);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__220);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -5970,24 +5904,20 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_BBANDS);
   Py_VISIT(traverse_module_state->__pyx_n_s_BOP);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Buffer_view_does_not_expose_stri);
   Py_VISIT(traverse_module_state->__pyx_n_s_CCI);
   Py_VISIT(traverse_module_state->__pyx_n_s_CMF);
   Py_VISIT(traverse_module_state->__pyx_n_s_CROSSOVER);
   Py_VISIT(traverse_module_state->__pyx_n_s_CROSSUNDER);
-  Py_VISIT(traverse_module_state->__pyx_n_s_CURVE);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Can_only_create_a_buffer_that_is);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Cannot_assign_to_read_only_memor);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Cannot_create_writable_memory_vi);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Cannot_get_series_from);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Cannot_index_with_type);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Cannot_transpose_memoryview_with);
-  Py_VISIT(traverse_module_state->__pyx_n_s_CurveOption);
-  Py_VISIT(traverse_module_state->__pyx_n_s_CurveOption___repr);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_Curve_Option_Enumeration);
   Py_VISIT(traverse_module_state->__pyx_n_s_DEMA);
   Py_VISIT(traverse_module_state->__pyx_n_u_DEMA);
   Py_VISIT(traverse_module_state->__pyx_n_s_DIFF);
   Py_VISIT(traverse_module_state->__pyx_n_s_DataFrame);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Different_sizes);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Dimension_d_is_not_direct);
   Py_VISIT(traverse_module_state->__pyx_n_s_EFFICIENCY_RATIO);
@@ -6069,15 +5999,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_View_MemoryView);
   Py_VISIT(traverse_module_state->__pyx_n_s_WCLPRICE);
   Py_VISIT(traverse_module_state->__pyx_n_s_WMA);
   Py_VISIT(traverse_module_state->__pyx_n_u_WMA);
   Py_VISIT(traverse_module_state->__pyx_kp_u__15);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
-  Py_VISIT(traverse_module_state->__pyx_n_s__221);
+  Py_VISIT(traverse_module_state->__pyx_n_s__217);
   Py_VISIT(traverse_module_state->__pyx_n_s__3);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__7);
   Py_VISIT(traverse_module_state->__pyx_n_s_abc);
   Py_VISIT(traverse_module_state->__pyx_n_s_abs);
   Py_VISIT(traverse_module_state->__pyx_n_s_adjust);
   Py_VISIT(traverse_module_state->__pyx_n_s_af);
@@ -6106,15 +6036,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_adx);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_atr);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_avgprice);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_bbands);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_bop);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_cci);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_cmf);
-  Py_VISIT(traverse_module_state->__pyx_n_s_calc_curve);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_dema);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_diff);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_ema);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_eval);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_exp);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_kama);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_keltner);
@@ -6160,15 +6089,14 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_contiguous_and_direct);
   Py_VISIT(traverse_module_state->__pyx_kp_s_contiguous_and_indirect);
   Py_VISIT(traverse_module_state->__pyx_kp_u_core);
   Py_VISIT(traverse_module_state->__pyx_n_s_corr);
   Py_VISIT(traverse_module_state->__pyx_n_s_count);
   Py_VISIT(traverse_module_state->__pyx_n_s_crossover);
   Py_VISIT(traverse_module_state->__pyx_n_s_crossunder);
-  Py_VISIT(traverse_module_state->__pyx_n_s_curve);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_kp_u_data_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_dataframe_like);
   Py_VISIT(traverse_module_state->__pyx_n_s_decorator);
   Py_VISIT(traverse_module_state->__pyx_n_s_default_item);
   Py_VISIT(traverse_module_state->__pyx_n_s_di1);
   Py_VISIT(traverse_module_state->__pyx_n_s_di2);
@@ -6371,30 +6299,27 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_res);
   Py_VISIT(traverse_module_state->__pyx_n_s_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_rho);
   Py_VISIT(traverse_module_state->__pyx_n_s_rma);
   Py_VISIT(traverse_module_state->__pyx_n_s_rmse);
   Py_VISIT(traverse_module_state->__pyx_n_s_roc);
   Py_VISIT(traverse_module_state->__pyx_n_s_rsi);
-  Py_VISIT(traverse_module_state->__pyx_n_s_rsquare);
-  Py_VISIT(traverse_module_state->__pyx_n_s_rvalue);
   Py_VISIT(traverse_module_state->__pyx_n_s_s);
   Py_VISIT(traverse_module_state->__pyx_n_s_same_scale);
   Py_VISIT(traverse_module_state->__pyx_n_u_same_scale);
   Py_VISIT(traverse_module_state->__pyx_n_s_sar);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_n_s_send);
   Py_VISIT(traverse_module_state->__pyx_n_s_series);
   Py_VISIT(traverse_module_state->__pyx_n_s_set_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_shape);
   Py_VISIT(traverse_module_state->__pyx_n_s_signal);
   Py_VISIT(traverse_module_state->__pyx_n_s_size);
-  Py_VISIT(traverse_module_state->__pyx_n_s_skip);
   Py_VISIT(traverse_module_state->__pyx_n_s_slope);
   Py_VISIT(traverse_module_state->__pyx_n_s_slowd);
   Py_VISIT(traverse_module_state->__pyx_n_s_slowf);
   Py_VISIT(traverse_module_state->__pyx_n_s_slowk);
   Py_VISIT(traverse_module_state->__pyx_kp_u_slowk_slowd);
   Py_VISIT(traverse_module_state->__pyx_n_s_slown);
   Py_VISIT(traverse_module_state->__pyx_n_s_sma);
@@ -6404,15 +6329,14 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_adx_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_atr_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_bbands_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_bop_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_cci_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_cmf_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_cross_pxi);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_curve_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_dema_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_diff_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_ema_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_eval_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_exp_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_flags_pxi);
   Py_VISIT(traverse_module_state->__pyx_kp_s_src_mintalib_cython_kama_pxi);
@@ -6454,21 +6378,17 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_strided_and_indirect);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_struct);
   Py_VISIT(traverse_module_state->__pyx_n_s_super);
   Py_VISIT(traverse_module_state->__pyx_n_s_sx);
   Py_VISIT(traverse_module_state->__pyx_n_s_sxx);
   Py_VISIT(traverse_module_state->__pyx_n_s_sxy);
-  Py_VISIT(traverse_module_state->__pyx_n_s_sxz);
   Py_VISIT(traverse_module_state->__pyx_n_s_sy);
   Py_VISIT(traverse_module_state->__pyx_n_s_sys);
   Py_VISIT(traverse_module_state->__pyx_n_s_syy);
-  Py_VISIT(traverse_module_state->__pyx_n_s_syz);
-  Py_VISIT(traverse_module_state->__pyx_n_s_sz);
-  Py_VISIT(traverse_module_state->__pyx_n_s_szz);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_throw);
   Py_VISIT(traverse_module_state->__pyx_n_s_tname);
   Py_VISIT(traverse_module_state->__pyx_n_s_total);
   Py_VISIT(traverse_module_state->__pyx_n_s_tr);
   Py_VISIT(traverse_module_state->__pyx_n_s_trange);
   Py_VISIT(traverse_module_state->__pyx_n_s_trend);
@@ -6490,18 +6410,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_value);
   Py_VISIT(traverse_module_state->__pyx_n_s_version_info);
   Py_VISIT(traverse_module_state->__pyx_n_s_volume);
   Py_VISIT(traverse_module_state->__pyx_n_u_volume);
   Py_VISIT(traverse_module_state->__pyx_n_s_vsum);
   Py_VISIT(traverse_module_state->__pyx_n_s_vxx);
   Py_VISIT(traverse_module_state->__pyx_n_s_vxy);
-  Py_VISIT(traverse_module_state->__pyx_n_s_vxz);
   Py_VISIT(traverse_module_state->__pyx_n_s_vyy);
-  Py_VISIT(traverse_module_state->__pyx_n_s_vyz);
-  Py_VISIT(traverse_module_state->__pyx_n_s_vzz);
   Py_VISIT(traverse_module_state->__pyx_n_s_wcl);
   Py_VISIT(traverse_module_state->__pyx_n_s_where);
   Py_VISIT(traverse_module_state->__pyx_n_s_where_flag);
   Py_VISIT(traverse_module_state->__pyx_n_s_wrap);
   Py_VISIT(traverse_module_state->__pyx_n_s_wrap_function);
   Py_VISIT(traverse_module_state->__pyx_n_s_wrap_function_locals_decorator);
   Py_VISIT(traverse_module_state->__pyx_n_s_wrap_indicator);
@@ -6620,21 +6537,20 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__187);
   Py_VISIT(traverse_module_state->__pyx_tuple__189);
   Py_VISIT(traverse_module_state->__pyx_tuple__191);
   Py_VISIT(traverse_module_state->__pyx_tuple__192);
   Py_VISIT(traverse_module_state->__pyx_tuple__195);
   Py_VISIT(traverse_module_state->__pyx_tuple__197);
   Py_VISIT(traverse_module_state->__pyx_tuple__201);
+  Py_VISIT(traverse_module_state->__pyx_tuple__203);
   Py_VISIT(traverse_module_state->__pyx_tuple__204);
-  Py_VISIT(traverse_module_state->__pyx_tuple__207);
+  Py_VISIT(traverse_module_state->__pyx_tuple__206);
   Py_VISIT(traverse_module_state->__pyx_tuple__208);
-  Py_VISIT(traverse_module_state->__pyx_tuple__210);
-  Py_VISIT(traverse_module_state->__pyx_tuple__212);
-  Py_VISIT(traverse_module_state->__pyx_tuple__217);
-  Py_VISIT(traverse_module_state->__pyx_tuple__219);
+  Py_VISIT(traverse_module_state->__pyx_tuple__213);
+  Py_VISIT(traverse_module_state->__pyx_tuple__215);
   Py_VISIT(traverse_module_state->__pyx_codeobj__12);
   Py_VISIT(traverse_module_state->__pyx_codeobj__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__27);
   Py_VISIT(traverse_module_state->__pyx_codeobj__29);
   Py_VISIT(traverse_module_state->__pyx_codeobj__31);
   Py_VISIT(traverse_module_state->__pyx_codeobj__33);
   Py_VISIT(traverse_module_state->__pyx_codeobj__36);
@@ -6734,25 +6650,22 @@
   Py_VISIT(traverse_module_state->__pyx_codeobj__193);
   Py_VISIT(traverse_module_state->__pyx_codeobj__194);
   Py_VISIT(traverse_module_state->__pyx_codeobj__196);
   Py_VISIT(traverse_module_state->__pyx_codeobj__198);
   Py_VISIT(traverse_module_state->__pyx_codeobj__199);
   Py_VISIT(traverse_module_state->__pyx_codeobj__200);
   Py_VISIT(traverse_module_state->__pyx_codeobj__202);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__203);
   Py_VISIT(traverse_module_state->__pyx_codeobj__205);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__206);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__207);
   Py_VISIT(traverse_module_state->__pyx_codeobj__209);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__210);
   Py_VISIT(traverse_module_state->__pyx_codeobj__211);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__213);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__212);
   Py_VISIT(traverse_module_state->__pyx_codeobj__214);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__215);
   Py_VISIT(traverse_module_state->__pyx_codeobj__216);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__218);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__220);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -6807,24 +6720,20 @@
 #define __pyx_n_s_BBANDS __pyx_mstate_global->__pyx_n_s_BBANDS
 #define __pyx_n_s_BOP __pyx_mstate_global->__pyx_n_s_BOP
 #define __pyx_kp_s_Buffer_view_does_not_expose_stri __pyx_mstate_global->__pyx_kp_s_Buffer_view_does_not_expose_stri
 #define __pyx_n_s_CCI __pyx_mstate_global->__pyx_n_s_CCI
 #define __pyx_n_s_CMF __pyx_mstate_global->__pyx_n_s_CMF
 #define __pyx_n_s_CROSSOVER __pyx_mstate_global->__pyx_n_s_CROSSOVER
 #define __pyx_n_s_CROSSUNDER __pyx_mstate_global->__pyx_n_s_CROSSUNDER
-#define __pyx_n_s_CURVE __pyx_mstate_global->__pyx_n_s_CURVE
 #define __pyx_kp_s_Can_only_create_a_buffer_that_is __pyx_mstate_global->__pyx_kp_s_Can_only_create_a_buffer_that_is
 #define __pyx_kp_s_Cannot_assign_to_read_only_memor __pyx_mstate_global->__pyx_kp_s_Cannot_assign_to_read_only_memor
 #define __pyx_kp_s_Cannot_create_writable_memory_vi __pyx_mstate_global->__pyx_kp_s_Cannot_create_writable_memory_vi
 #define __pyx_kp_u_Cannot_get_series_from __pyx_mstate_global->__pyx_kp_u_Cannot_get_series_from
 #define __pyx_kp_u_Cannot_index_with_type __pyx_mstate_global->__pyx_kp_u_Cannot_index_with_type
 #define __pyx_kp_s_Cannot_transpose_memoryview_with __pyx_mstate_global->__pyx_kp_s_Cannot_transpose_memoryview_with
-#define __pyx_n_s_CurveOption __pyx_mstate_global->__pyx_n_s_CurveOption
-#define __pyx_n_s_CurveOption___repr __pyx_mstate_global->__pyx_n_s_CurveOption___repr
-#define __pyx_kp_s_Curve_Option_Enumeration __pyx_mstate_global->__pyx_kp_s_Curve_Option_Enumeration
 #define __pyx_n_s_DEMA __pyx_mstate_global->__pyx_n_s_DEMA
 #define __pyx_n_u_DEMA __pyx_mstate_global->__pyx_n_u_DEMA
 #define __pyx_n_s_DIFF __pyx_mstate_global->__pyx_n_s_DIFF
 #define __pyx_n_s_DataFrame __pyx_mstate_global->__pyx_n_s_DataFrame
 #define __pyx_kp_u_Different_sizes __pyx_mstate_global->__pyx_kp_u_Different_sizes
 #define __pyx_kp_s_Dimension_d_is_not_direct __pyx_mstate_global->__pyx_kp_s_Dimension_d_is_not_direct
 #define __pyx_n_s_EFFICIENCY_RATIO __pyx_mstate_global->__pyx_n_s_EFFICIENCY_RATIO
@@ -6906,15 +6815,15 @@
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_View_MemoryView __pyx_mstate_global->__pyx_n_s_View_MemoryView
 #define __pyx_n_s_WCLPRICE __pyx_mstate_global->__pyx_n_s_WCLPRICE
 #define __pyx_n_s_WMA __pyx_mstate_global->__pyx_n_s_WMA
 #define __pyx_n_u_WMA __pyx_mstate_global->__pyx_n_u_WMA
 #define __pyx_kp_u__15 __pyx_mstate_global->__pyx_kp_u__15
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
-#define __pyx_n_s__221 __pyx_mstate_global->__pyx_n_s__221
+#define __pyx_n_s__217 __pyx_mstate_global->__pyx_n_s__217
 #define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
 #define __pyx_n_s_abc __pyx_mstate_global->__pyx_n_s_abc
 #define __pyx_n_s_abs __pyx_mstate_global->__pyx_n_s_abs
 #define __pyx_n_s_adjust __pyx_mstate_global->__pyx_n_s_adjust
 #define __pyx_n_s_af __pyx_mstate_global->__pyx_n_s_af
@@ -6943,15 +6852,14 @@
 #define __pyx_n_s_calc_adx __pyx_mstate_global->__pyx_n_s_calc_adx
 #define __pyx_n_s_calc_atr __pyx_mstate_global->__pyx_n_s_calc_atr
 #define __pyx_n_s_calc_avgprice __pyx_mstate_global->__pyx_n_s_calc_avgprice
 #define __pyx_n_s_calc_bbands __pyx_mstate_global->__pyx_n_s_calc_bbands
 #define __pyx_n_s_calc_bop __pyx_mstate_global->__pyx_n_s_calc_bop
 #define __pyx_n_s_calc_cci __pyx_mstate_global->__pyx_n_s_calc_cci
 #define __pyx_n_s_calc_cmf __pyx_mstate_global->__pyx_n_s_calc_cmf
-#define __pyx_n_s_calc_curve __pyx_mstate_global->__pyx_n_s_calc_curve
 #define __pyx_n_s_calc_dema __pyx_mstate_global->__pyx_n_s_calc_dema
 #define __pyx_n_s_calc_diff __pyx_mstate_global->__pyx_n_s_calc_diff
 #define __pyx_n_s_calc_ema __pyx_mstate_global->__pyx_n_s_calc_ema
 #define __pyx_n_s_calc_eval __pyx_mstate_global->__pyx_n_s_calc_eval
 #define __pyx_n_s_calc_exp __pyx_mstate_global->__pyx_n_s_calc_exp
 #define __pyx_n_s_calc_kama __pyx_mstate_global->__pyx_n_s_calc_kama
 #define __pyx_n_s_calc_keltner __pyx_mstate_global->__pyx_n_s_calc_keltner
@@ -6997,15 +6905,14 @@
 #define __pyx_kp_s_contiguous_and_direct __pyx_mstate_global->__pyx_kp_s_contiguous_and_direct
 #define __pyx_kp_s_contiguous_and_indirect __pyx_mstate_global->__pyx_kp_s_contiguous_and_indirect
 #define __pyx_kp_u_core __pyx_mstate_global->__pyx_kp_u_core
 #define __pyx_n_s_corr __pyx_mstate_global->__pyx_n_s_corr
 #define __pyx_n_s_count __pyx_mstate_global->__pyx_n_s_count
 #define __pyx_n_s_crossover __pyx_mstate_global->__pyx_n_s_crossover
 #define __pyx_n_s_crossunder __pyx_mstate_global->__pyx_n_s_crossunder
-#define __pyx_n_s_curve __pyx_mstate_global->__pyx_n_s_curve
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_kp_u_data_2 __pyx_mstate_global->__pyx_kp_u_data_2
 #define __pyx_n_s_dataframe_like __pyx_mstate_global->__pyx_n_s_dataframe_like
 #define __pyx_n_s_decorator __pyx_mstate_global->__pyx_n_s_decorator
 #define __pyx_n_s_default_item __pyx_mstate_global->__pyx_n_s_default_item
 #define __pyx_n_s_di1 __pyx_mstate_global->__pyx_n_s_di1
 #define __pyx_n_s_di2 __pyx_mstate_global->__pyx_n_s_di2
@@ -7208,30 +7115,27 @@
 #define __pyx_n_s_res __pyx_mstate_global->__pyx_n_s_res
 #define __pyx_n_s_result __pyx_mstate_global->__pyx_n_s_result
 #define __pyx_n_s_rho __pyx_mstate_global->__pyx_n_s_rho
 #define __pyx_n_s_rma __pyx_mstate_global->__pyx_n_s_rma
 #define __pyx_n_s_rmse __pyx_mstate_global->__pyx_n_s_rmse
 #define __pyx_n_s_roc __pyx_mstate_global->__pyx_n_s_roc
 #define __pyx_n_s_rsi __pyx_mstate_global->__pyx_n_s_rsi
-#define __pyx_n_s_rsquare __pyx_mstate_global->__pyx_n_s_rsquare
-#define __pyx_n_s_rvalue __pyx_mstate_global->__pyx_n_s_rvalue
 #define __pyx_n_s_s __pyx_mstate_global->__pyx_n_s_s
 #define __pyx_n_s_same_scale __pyx_mstate_global->__pyx_n_s_same_scale
 #define __pyx_n_u_same_scale __pyx_mstate_global->__pyx_n_u_same_scale
 #define __pyx_n_s_sar __pyx_mstate_global->__pyx_n_s_sar
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_n_s_send __pyx_mstate_global->__pyx_n_s_send
 #define __pyx_n_s_series __pyx_mstate_global->__pyx_n_s_series
 #define __pyx_n_s_set_name __pyx_mstate_global->__pyx_n_s_set_name
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_shape __pyx_mstate_global->__pyx_n_s_shape
 #define __pyx_n_s_signal __pyx_mstate_global->__pyx_n_s_signal
 #define __pyx_n_s_size __pyx_mstate_global->__pyx_n_s_size
-#define __pyx_n_s_skip __pyx_mstate_global->__pyx_n_s_skip
 #define __pyx_n_s_slope __pyx_mstate_global->__pyx_n_s_slope
 #define __pyx_n_s_slowd __pyx_mstate_global->__pyx_n_s_slowd
 #define __pyx_n_s_slowf __pyx_mstate_global->__pyx_n_s_slowf
 #define __pyx_n_s_slowk __pyx_mstate_global->__pyx_n_s_slowk
 #define __pyx_kp_u_slowk_slowd __pyx_mstate_global->__pyx_kp_u_slowk_slowd
 #define __pyx_n_s_slown __pyx_mstate_global->__pyx_n_s_slown
 #define __pyx_n_s_sma __pyx_mstate_global->__pyx_n_s_sma
@@ -7241,15 +7145,14 @@
 #define __pyx_kp_s_src_mintalib_cython_adx_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_adx_pxi
 #define __pyx_kp_s_src_mintalib_cython_atr_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_atr_pxi
 #define __pyx_kp_s_src_mintalib_cython_bbands_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_bbands_pxi
 #define __pyx_kp_s_src_mintalib_cython_bop_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_bop_pxi
 #define __pyx_kp_s_src_mintalib_cython_cci_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_cci_pxi
 #define __pyx_kp_s_src_mintalib_cython_cmf_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_cmf_pxi
 #define __pyx_kp_s_src_mintalib_cython_cross_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_cross_pxi
-#define __pyx_kp_s_src_mintalib_cython_curve_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_curve_pxi
 #define __pyx_kp_s_src_mintalib_cython_dema_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_dema_pxi
 #define __pyx_kp_s_src_mintalib_cython_diff_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_diff_pxi
 #define __pyx_kp_s_src_mintalib_cython_ema_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_ema_pxi
 #define __pyx_kp_s_src_mintalib_cython_eval_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_eval_pxi
 #define __pyx_kp_s_src_mintalib_cython_exp_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_exp_pxi
 #define __pyx_kp_s_src_mintalib_cython_flags_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_flags_pxi
 #define __pyx_kp_s_src_mintalib_cython_kama_pxi __pyx_mstate_global->__pyx_kp_s_src_mintalib_cython_kama_pxi
@@ -7291,21 +7194,17 @@
 #define __pyx_kp_s_strided_and_indirect __pyx_mstate_global->__pyx_kp_s_strided_and_indirect
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_struct __pyx_mstate_global->__pyx_n_s_struct
 #define __pyx_n_s_super __pyx_mstate_global->__pyx_n_s_super
 #define __pyx_n_s_sx __pyx_mstate_global->__pyx_n_s_sx
 #define __pyx_n_s_sxx __pyx_mstate_global->__pyx_n_s_sxx
 #define __pyx_n_s_sxy __pyx_mstate_global->__pyx_n_s_sxy
-#define __pyx_n_s_sxz __pyx_mstate_global->__pyx_n_s_sxz
 #define __pyx_n_s_sy __pyx_mstate_global->__pyx_n_s_sy
 #define __pyx_n_s_sys __pyx_mstate_global->__pyx_n_s_sys
 #define __pyx_n_s_syy __pyx_mstate_global->__pyx_n_s_syy
-#define __pyx_n_s_syz __pyx_mstate_global->__pyx_n_s_syz
-#define __pyx_n_s_sz __pyx_mstate_global->__pyx_n_s_sz
-#define __pyx_n_s_szz __pyx_mstate_global->__pyx_n_s_szz
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_throw __pyx_mstate_global->__pyx_n_s_throw
 #define __pyx_n_s_tname __pyx_mstate_global->__pyx_n_s_tname
 #define __pyx_n_s_total __pyx_mstate_global->__pyx_n_s_total
 #define __pyx_n_s_tr __pyx_mstate_global->__pyx_n_s_tr
 #define __pyx_n_s_trange __pyx_mstate_global->__pyx_n_s_trange
 #define __pyx_n_s_trend __pyx_mstate_global->__pyx_n_s_trend
@@ -7327,18 +7226,15 @@
 #define __pyx_n_s_value __pyx_mstate_global->__pyx_n_s_value
 #define __pyx_n_s_version_info __pyx_mstate_global->__pyx_n_s_version_info
 #define __pyx_n_s_volume __pyx_mstate_global->__pyx_n_s_volume
 #define __pyx_n_u_volume __pyx_mstate_global->__pyx_n_u_volume
 #define __pyx_n_s_vsum __pyx_mstate_global->__pyx_n_s_vsum
 #define __pyx_n_s_vxx __pyx_mstate_global->__pyx_n_s_vxx
 #define __pyx_n_s_vxy __pyx_mstate_global->__pyx_n_s_vxy
-#define __pyx_n_s_vxz __pyx_mstate_global->__pyx_n_s_vxz
 #define __pyx_n_s_vyy __pyx_mstate_global->__pyx_n_s_vyy
-#define __pyx_n_s_vyz __pyx_mstate_global->__pyx_n_s_vyz
-#define __pyx_n_s_vzz __pyx_mstate_global->__pyx_n_s_vzz
 #define __pyx_n_s_wcl __pyx_mstate_global->__pyx_n_s_wcl
 #define __pyx_n_s_where __pyx_mstate_global->__pyx_n_s_where
 #define __pyx_n_s_where_flag __pyx_mstate_global->__pyx_n_s_where_flag
 #define __pyx_n_s_wrap __pyx_mstate_global->__pyx_n_s_wrap
 #define __pyx_n_s_wrap_function __pyx_mstate_global->__pyx_n_s_wrap_function
 #define __pyx_n_s_wrap_function_locals_decorator __pyx_mstate_global->__pyx_n_s_wrap_function_locals_decorator
 #define __pyx_n_s_wrap_indicator __pyx_mstate_global->__pyx_n_s_wrap_indicator
@@ -7457,21 +7353,20 @@
 #define __pyx_tuple__187 __pyx_mstate_global->__pyx_tuple__187
 #define __pyx_tuple__189 __pyx_mstate_global->__pyx_tuple__189
 #define __pyx_tuple__191 __pyx_mstate_global->__pyx_tuple__191
 #define __pyx_tuple__192 __pyx_mstate_global->__pyx_tuple__192
 #define __pyx_tuple__195 __pyx_mstate_global->__pyx_tuple__195
 #define __pyx_tuple__197 __pyx_mstate_global->__pyx_tuple__197
 #define __pyx_tuple__201 __pyx_mstate_global->__pyx_tuple__201
+#define __pyx_tuple__203 __pyx_mstate_global->__pyx_tuple__203
 #define __pyx_tuple__204 __pyx_mstate_global->__pyx_tuple__204
-#define __pyx_tuple__207 __pyx_mstate_global->__pyx_tuple__207
+#define __pyx_tuple__206 __pyx_mstate_global->__pyx_tuple__206
 #define __pyx_tuple__208 __pyx_mstate_global->__pyx_tuple__208
-#define __pyx_tuple__210 __pyx_mstate_global->__pyx_tuple__210
-#define __pyx_tuple__212 __pyx_mstate_global->__pyx_tuple__212
-#define __pyx_tuple__217 __pyx_mstate_global->__pyx_tuple__217
-#define __pyx_tuple__219 __pyx_mstate_global->__pyx_tuple__219
+#define __pyx_tuple__213 __pyx_mstate_global->__pyx_tuple__213
+#define __pyx_tuple__215 __pyx_mstate_global->__pyx_tuple__215
 #define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
 #define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 #define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
 #define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
 #define __pyx_codeobj__36 __pyx_mstate_global->__pyx_codeobj__36
@@ -7571,37 +7466,34 @@
 #define __pyx_codeobj__193 __pyx_mstate_global->__pyx_codeobj__193
 #define __pyx_codeobj__194 __pyx_mstate_global->__pyx_codeobj__194
 #define __pyx_codeobj__196 __pyx_mstate_global->__pyx_codeobj__196
 #define __pyx_codeobj__198 __pyx_mstate_global->__pyx_codeobj__198
 #define __pyx_codeobj__199 __pyx_mstate_global->__pyx_codeobj__199
 #define __pyx_codeobj__200 __pyx_mstate_global->__pyx_codeobj__200
 #define __pyx_codeobj__202 __pyx_mstate_global->__pyx_codeobj__202
-#define __pyx_codeobj__203 __pyx_mstate_global->__pyx_codeobj__203
 #define __pyx_codeobj__205 __pyx_mstate_global->__pyx_codeobj__205
-#define __pyx_codeobj__206 __pyx_mstate_global->__pyx_codeobj__206
+#define __pyx_codeobj__207 __pyx_mstate_global->__pyx_codeobj__207
 #define __pyx_codeobj__209 __pyx_mstate_global->__pyx_codeobj__209
+#define __pyx_codeobj__210 __pyx_mstate_global->__pyx_codeobj__210
 #define __pyx_codeobj__211 __pyx_mstate_global->__pyx_codeobj__211
-#define __pyx_codeobj__213 __pyx_mstate_global->__pyx_codeobj__213
+#define __pyx_codeobj__212 __pyx_mstate_global->__pyx_codeobj__212
 #define __pyx_codeobj__214 __pyx_mstate_global->__pyx_codeobj__214
-#define __pyx_codeobj__215 __pyx_mstate_global->__pyx_codeobj__215
 #define __pyx_codeobj__216 __pyx_mstate_global->__pyx_codeobj__216
-#define __pyx_codeobj__218 __pyx_mstate_global->__pyx_codeobj__218
-#define __pyx_codeobj__220 __pyx_mstate_global->__pyx_codeobj__220
 /* #### Code section: module_code ### */
-static PyObject *__pyx_gb_8mintalib_4core_228generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_8mintalib_4core_224generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "mintalib/core.pyx":6
  * 
  * __all__ = tuple(
  *     k for k, v in globals().items()             # <<<<<<<<<<<<<<
  *         if k.islower() and callable(v)
  *         and v.__module__.endswith(".core")
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_226genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
+static PyObject *__pyx_pf_8mintalib_4core_222genexpr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
   struct __pyx_obj_8mintalib_4core___pyx_scope_struct_2_genexpr *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
@@ -7613,15 +7505,15 @@
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8mintalib_4core_228generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_genexpr, __pyx_n_s_mintalib_core); if (unlikely(!gen)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8mintalib_4core_224generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_genexpr, __pyx_n_s_mintalib_core); if (unlikely(!gen)) __PYX_ERR(2, 6, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7629,15 +7521,15 @@
   __pyx_r = NULL;
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_8mintalib_4core_228generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_8mintalib_4core_224generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_8mintalib_4core___pyx_scope_struct_2_genexpr *__pyx_cur_scope = ((struct __pyx_obj_8mintalib_4core___pyx_scope_struct_2_genexpr *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
@@ -29050,15 +28942,15 @@
  * """ Flag functions """
  * 
  * def flag_above(series, double level=0.0, *, double na_value=NAN, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Flag for value above level """
  * 
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_229__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_225__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -29622,15 +29514,15 @@
  * 
  * 
  * def flag_below(series, double level=0.0, *, double na_value=NAN, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Flag for value below level """
  * 
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_231__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_227__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -30194,15 +30086,15 @@
  * 
  * 
  * def invert_flag(series, *, double na_value=NAN, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Invert flag  """
  * 
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_233__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_229__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -30738,15 +30630,15 @@
  * 
  * 
  * def updown_flag(series, double up_level=0.0, double down_level=0.0, *,             # <<<<<<<<<<<<<<
  *                 double up_flag=1.0, double down_flag=0.0, double start_flag=NAN,
  *                 wrap: bool = False):
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_235__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_231__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -31408,15 +31300,15 @@
  * 
  * 
  * def where_flag(flag, x, y, z=NAN, *, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Value according to flag """
  * 
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_237__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_233__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -32248,15 +32140,15 @@
  * 
  * 
  * @wrap_function(flag_above)             # <<<<<<<<<<<<<<
  * def FLAG_ABOVE(series, level: float = 0.0, *, na_value: float = NAN, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_239__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_235__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -32624,15 +32516,15 @@
  * 
  * 
  * @wrap_function(flag_below)             # <<<<<<<<<<<<<<
  * def FLAG_BELOW(series, level: float = 0.0, *, na_value: float = NAN, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_241__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_237__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -33000,15 +32892,15 @@
  * 
  * 
  * @wrap_function(invert_flag)             # <<<<<<<<<<<<<<
  * def INVERT_FLAG(series, *, na_value: float = NAN, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_243__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_239__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -33328,15 +33220,15 @@
  * 
  * 
  * @wrap_function(updown_flag)             # <<<<<<<<<<<<<<
  * def UPDOWN_FLAG(series, up_level: float = 0.0, down_level: float = 0.0, *,
  *                 up_flag: float = 1.0, down_flag: float = 0.0, start_flag: float = NAN, item: str = None):
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_245__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_241__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -35751,15 +35643,15 @@
  * 
  * 
  * @wrap_function(calc_roc)             # <<<<<<<<<<<<<<
  * def ROC(series, period: int = 1, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_247__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_243__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -36591,15 +36483,15 @@
  * 
  * 
  * @wrap_function(calc_diff)             # <<<<<<<<<<<<<<
  * def DIFF(series, period: int = 1, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_249__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_245__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -40152,15 +40044,15 @@
  * 
  * 
  * @wrap_function(calc_mad)             # <<<<<<<<<<<<<<
  * def MAD(series, period: int = 20, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_251__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_247__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -41096,15 +40988,15 @@
  * 
  * 
  * @wrap_function(calc_stdev)             # <<<<<<<<<<<<<<
  * def STDEV(series, period: int = 20, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_253__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_249__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -45961,15 +45853,15 @@
  * 
  * 
  * @wrap_function(calc_tema)             # <<<<<<<<<<<<<<
  * def TEMA(series, period: int = 20, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_255__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_251__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -46832,15 +46724,15 @@
  * 
  * 
  * @wrap_function(calc_ma)             # <<<<<<<<<<<<<<
  * def MA(series, period: int = 20, *, ma_type: str = None, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_257__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_253__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -47873,15 +47765,15 @@
  * 
  * 
  * @wrap_function(calc_rsi)             # <<<<<<<<<<<<<<
  * def RSI(series, period: int = 14, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_259__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_255__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -50408,15 +50300,15 @@
  * 
  * 
  * @wrap_function(calc_plusdi)             # <<<<<<<<<<<<<<
  * def PLUSDI(prices, period: int = 14):
  *     result = calc_plusdi(prices, period=period)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_261__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_257__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -50671,15 +50563,15 @@
  * 
  * 
  * @wrap_function(calc_minusdi)             # <<<<<<<<<<<<<<
  * def MINUSDI(prices, period: int = 14):
  *     result = calc_minusdi(prices, period=period)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_263__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_259__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -50934,15 +50826,15 @@
  * 
  * 
  * @wrap_function(calc_adx)             # <<<<<<<<<<<<<<
  * def ADX(prices, period: int = 14):
  *     result = calc_adx(prices, period=period)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_265__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_261__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -53138,15 +53030,15 @@
  * 
  * 
  * @wrap_function(calc_atr)             # <<<<<<<<<<<<<<
  * def ATR(prices, period: int = 14):
  *     result = calc_atr(prices, period=period)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_267__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_263__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -53401,15 +53293,15 @@
  * 
  * 
  * @wrap_function(calc_natr)             # <<<<<<<<<<<<<<
  * def NATR(prices, period: int = 14):
  *     result = calc_natr(prices, period=period)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_269__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_265__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -53664,15 +53556,15 @@
  * 
  * 
  * @wrap_function(calc_latr)             # <<<<<<<<<<<<<<
  * def LATR(prices, period: int = 14):
  *     result = calc_latr(prices, period=period)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_271__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_267__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -55736,15 +55628,15 @@
  * 
  * 
  * @wrap_function(calc_cci)             # <<<<<<<<<<<<<<
  * def CCI(prices, period: int = 20):
  *     result = calc_cci(prices, period=period)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_273__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_269__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -56702,15 +56594,15 @@
  * 
  * 
  * @wrap_function(calc_cmf)             # <<<<<<<<<<<<<<
  * def CMF(prices, period: int = 20):
  *     result = calc_cmf(prices, period=period)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_275__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_271__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -57609,15 +57501,15 @@
  * 
  * 
  * @wrap_function(calc_mfi)             # <<<<<<<<<<<<<<
  * def MFI(prices, period: int = 14):
  *     result = calc_mfi(prices, period=period)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_277__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_273__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -58515,15 +58407,15 @@
  * 
  * 
  * @wrap_function(calc_bop)             # <<<<<<<<<<<<<<
  * def BOP(prices, period: int = 20):
  *     result = calc_bop(prices, period=period)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_279__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_275__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -59218,15 +59110,15 @@
  * 
  * 
  * @wrap_function(calc_bbands)             # <<<<<<<<<<<<<<
  * def BBANDS(prices, period: int = 20, nbdev: float = 2.0):
  *     result = calc_bbands(prices, period=period, nbdev=nbdev)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_281__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_277__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -59963,15 +59855,15 @@
  * 
  * 
  * @wrap_function(calc_keltner)             # <<<<<<<<<<<<<<
  * def KELTNER(prices, period: int = 20, nbatr: float = 2.0):
  *     result = calc_keltner(prices, period=period, nbatr=nbatr)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_283__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_279__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -61679,15 +61571,15 @@
  * 
  * 
  * @wrap_function(efficiency_ratio)             # <<<<<<<<<<<<<<
  * def EFFICIENCY_RATIO(series, period: int = 10, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_285__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_281__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -62016,15 +61908,15 @@
  * 
  * 
  * @wrap_function(calc_kama)             # <<<<<<<<<<<<<<
  * def KAMA(series, period: int = 10, fastn: int = 2, slown: int = 30, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_287__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_283__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -62845,15 +62737,15 @@
  * 
  * 
  * @wrap_function(calc_macd)             # <<<<<<<<<<<<<<
  * def MACD(series, n1: int = 12, n2: int = 26, n3: int = 9, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_289__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_285__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -63822,15 +63714,15 @@
  * 
  * 
  * @wrap_function(calc_ppo)             # <<<<<<<<<<<<<<
  * def PPO(series, n1: int = 12, n2: int = 26, n3: int = 9, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_291__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_287__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -65405,15 +65297,15 @@
  * 
  * 
  * @wrap_function(calc_slope)             # <<<<<<<<<<<<<<
  * def SLOPE(series, period: int = 20, *, item: str = None):
  *     """ Slope (time linear regression) """
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_293__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_289__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -65747,15 +65639,15 @@
  * 
  * 
  * @wrap_function(calc_slope)             # <<<<<<<<<<<<<<
  * def RVALUE(series, period: int = 20, *, item: str = None):
  *     """ RValue (time linear regression) """
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_295__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_291__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -66089,15 +65981,15 @@
  * 
  * 
  * @wrap_function(calc_slope)             # <<<<<<<<<<<<<<
  * def FORECAST(series, period: int = 20, offset: int = 0, *, item: str = None):
  *     """ Forecast (time linear regression) """
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_297__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_293__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -66441,1988 +66333,33 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_series);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/mintalib/cython/curve.pxi":15
- * class CurveOption(IntEnum):
- *     """ Curve Option Enumeration """
- *     def __repr__(self):             # <<<<<<<<<<<<<<
- *         return str(self)
- * 
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_11CurveOption_1__repr__(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_8mintalib_4core_11CurveOption_1__repr__ = {"__repr__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_11CurveOption_1__repr__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8mintalib_4core_11CurveOption_1__repr__(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_self = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[1] = {0};
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__repr__ (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 15, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__repr__") < 0)) __PYX_ERR(36, 15, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 1)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-    }
-    __pyx_v_self = values[0];
-  }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__repr__", 1, 1, 1, __pyx_nargs); __PYX_ERR(36, 15, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_AddTraceback("mintalib.core.CurveOption.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8mintalib_4core_11CurveOption___repr__(__pyx_self, __pyx_v_self);
-
-  /* function exit code */
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_8mintalib_4core_11CurveOption___repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__repr__", 1);
-
-  /* "src/mintalib/cython/curve.pxi":16
- *     """ Curve Option Enumeration """
- *     def __repr__(self):
- *         return str(self)             # <<<<<<<<<<<<<<
- * 
- *     CURVE = 0
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_Str(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "src/mintalib/cython/curve.pxi":15
- * class CurveOption(IntEnum):
- *     """ Curve Option Enumeration """
- *     def __repr__(self):             # <<<<<<<<<<<<<<
- *         return str(self)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("mintalib.core.CurveOption.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "src/mintalib/cython/curve.pxi":25
- * 
- * 
- * def calc_curve(series, long period=20, *, int option=0, int offset=0, wrap: bool = False):             # <<<<<<<<<<<<<<
- *     """ Curve (time curvilinear regression) """
- * 
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_207calc_curve(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8mintalib_4core_206calc_curve, " Curve (time curvilinear regression) ");
-static PyMethodDef __pyx_mdef_8mintalib_4core_207calc_curve = {"calc_curve", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_207calc_curve, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8mintalib_4core_206calc_curve};
-static PyObject *__pyx_pw_8mintalib_4core_207calc_curve(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_series = 0;
-  long __pyx_v_period;
-  int __pyx_v_option;
-  CYTHON_UNUSED int __pyx_v_offset;
-  PyObject *__pyx_v_wrap = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[5] = {0,0,0,0,0};
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("calc_curve (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_series,&__pyx_n_s_period,&__pyx_n_s_option,&__pyx_n_s_offset,&__pyx_n_s_wrap,0};
-    values[4] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_False)));
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_series)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 25, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_period);
-          if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 25, __pyx_L3_error)
-        }
-      }
-      if (kw_args > 0 && likely(kw_args <= 3)) {
-        Py_ssize_t index;
-        for (index = 2; index < 5 && kw_args > 0; index++) {
-          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
-          if (value) { values[index] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 25, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_curve") < 0)) __PYX_ERR(36, 25, __pyx_L3_error)
-      }
-    } else {
-      switch (__pyx_nargs) {
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_series = values[0];
-    if (values[1]) {
-      __pyx_v_period = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v_period == (long)-1) && PyErr_Occurred())) __PYX_ERR(36, 25, __pyx_L3_error)
-    } else {
-      __pyx_v_period = ((long)((long)20));
-    }
-    if (values[2]) {
-      __pyx_v_option = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_option == (int)-1) && PyErr_Occurred())) __PYX_ERR(36, 25, __pyx_L3_error)
-    } else {
-      __pyx_v_option = ((int)((int)0));
-    }
-    if (values[3]) {
-      __pyx_v_offset = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(36, 25, __pyx_L3_error)
-    } else {
-      __pyx_v_offset = ((int)((int)0));
-    }
-    __pyx_v_wrap = values[4];
-  }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calc_curve", 0, 1, 2, __pyx_nargs); __PYX_ERR(36, 25, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_AddTraceback("mintalib.core.calc_curve", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8mintalib_4core_206calc_curve(__pyx_self, __pyx_v_series, __pyx_v_period, __pyx_v_option, __pyx_v_offset, __pyx_v_wrap);
-
-  /* function exit code */
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_8mintalib_4core_206calc_curve(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, long __pyx_v_period, int __pyx_v_option, CYTHON_UNUSED int __pyx_v_offset, PyObject *__pyx_v_wrap) {
-  __Pyx_memviewslice __pyx_v_zs = { 0, 0, { 0 }, { 0 }, { 0 } };
-  long __pyx_v_size;
-  PyObject *__pyx_v_result = 0;
-  __Pyx_memviewslice __pyx_v_output = { 0, 0, { 0 }, { 0 }, { 0 } };
-  double __pyx_v_x;
-  double __pyx_v_sx;
-  double __pyx_v_sxx;
-  double __pyx_v_vxx;
-  double __pyx_v_y;
-  double __pyx_v_sy;
-  double __pyx_v_syy;
-  double __pyx_v_vyy;
-  double __pyx_v_z;
-  double __pyx_v_sz;
-  double __pyx_v_szz;
-  double __pyx_v_vzz;
-  double __pyx_v_s;
-  double __pyx_v_sxz;
-  double __pyx_v_vxz;
-  double __pyx_v_syz;
-  double __pyx_v_vyz;
-  double __pyx_v_slope;
-  double __pyx_v_curve;
-  CYTHON_UNUSED double __pyx_v_intercept;
-  double __pyx_v_mse;
-  double __pyx_v_rmse;
-  double __pyx_v_rvalue;
-  int __pyx_v_skip;
-  long __pyx_v_i;
-  long __pyx_v_j;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  __Pyx_memviewslice __pyx_t_7 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  long __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
-  PyObject *__pyx_t_10 = NULL;
-  __Pyx_memviewslice __pyx_t_11 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  long __pyx_t_12;
-  long __pyx_t_13;
-  double __pyx_t_14;
-  double __pyx_t_15;
-  Py_ssize_t __pyx_t_16;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("calc_curve", 1);
-
-  /* "src/mintalib/cython/curve.pxi":28
- *     """ Curve (time curvilinear regression) """
- * 
- *     if option < 0 or option >= CURVE_OPTION_BADOPTION:             # <<<<<<<<<<<<<<
- *         raise ValueError("Invalid option %d" % option)
- * 
- */
-  __pyx_t_2 = (__pyx_v_option < 0);
-  if (!__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L4_bool_binop_done;
-  }
-  __pyx_t_2 = (__pyx_v_option >= __pyx_e_8mintalib_4core_CURVE_OPTION_BADOPTION);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L4_bool_binop_done:;
-  if (unlikely(__pyx_t_1)) {
-
-    /* "src/mintalib/cython/curve.pxi":29
- * 
- *     if option < 0 or option >= CURVE_OPTION_BADOPTION:
- *         raise ValueError("Invalid option %d" % option)             # <<<<<<<<<<<<<<
- * 
- *     cdef const double[:] zs = np.asarray(series, float)
- */
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_option); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 29, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyUnicode_Format(__pyx_kp_u_Invalid_option_d, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 29, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 29, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(36, 29, __pyx_L1_error)
-
-    /* "src/mintalib/cython/curve.pxi":28
- *     """ Curve (time curvilinear regression) """
- * 
- *     if option < 0 or option >= CURVE_OPTION_BADOPTION:             # <<<<<<<<<<<<<<
- *         raise ValueError("Invalid option %d" % option)
- * 
- */
-  }
-
-  /* "src/mintalib/cython/curve.pxi":31
- *         raise ValueError("Invalid option %d" % option)
- * 
- *     cdef const double[:] zs = np.asarray(series, float)             # <<<<<<<<<<<<<<
- *     cdef long size = zs.size
- * 
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = NULL;
-  __pyx_t_6 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_4);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-      __pyx_t_6 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_v_series, ((PyObject *)(&PyFloat_Type))};
-    __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 31, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_double__const__(__pyx_t_3, 0); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(36, 31, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_zs = __pyx_t_7;
-  __pyx_t_7.memview = NULL;
-  __pyx_t_7.data = NULL;
-
-  /* "src/mintalib/cython/curve.pxi":32
- * 
- *     cdef const double[:] zs = np.asarray(series, float)
- *     cdef long size = zs.size             # <<<<<<<<<<<<<<
- * 
- *     cdef object result = np.full(size, np.nan)
- */
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_zs, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_8 = __Pyx_PyInt_As_long(__pyx_t_5); if (unlikely((__pyx_t_8 == (long)-1) && PyErr_Occurred())) __PYX_ERR(36, 32, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_size = __pyx_t_8;
-
-  /* "src/mintalib/cython/curve.pxi":34
- *     cdef long size = zs.size
- * 
- *     cdef object result = np.full(size, np.nan)             # <<<<<<<<<<<<<<
- *     cdef double[:] output = result
- * 
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_full); if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_nan); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = NULL;
-  __pyx_t_6 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_9)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_9);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
-      __pyx_t_6 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[3] = {__pyx_t_9, __pyx_t_3, __pyx_t_10};
-    __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 34, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  }
-  __pyx_v_result = __pyx_t_5;
-  __pyx_t_5 = 0;
-
-  /* "src/mintalib/cython/curve.pxi":35
- * 
- *     cdef object result = np.full(size, np.nan)
- *     cdef double[:] output = result             # <<<<<<<<<<<<<<
- * 
- *     cdef double x, sx, sxx, vxx
- */
-  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_result, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(36, 35, __pyx_L1_error)
-  __pyx_v_output = __pyx_t_11;
-  __pyx_t_11.memview = NULL;
-  __pyx_t_11.data = NULL;
-
-  /* "src/mintalib/cython/curve.pxi":44
- *     cdef double slope, curve, intercept, mse, rmse, rvalue, rsquare
- * 
- *     cdef bint skip = 0             # <<<<<<<<<<<<<<
- * 
- *     cdef long i = 0, j = 0
- */
-  __pyx_v_skip = 0;
-
-  /* "src/mintalib/cython/curve.pxi":46
- *     cdef bint skip = 0
- * 
- *     cdef long i = 0, j = 0             # <<<<<<<<<<<<<<
- * 
- *     if period >= size:
- */
-  __pyx_v_i = 0;
-  __pyx_v_j = 0;
-
-  /* "src/mintalib/cython/curve.pxi":48
- *     cdef long i = 0, j = 0
- * 
- *     if period >= size:             # <<<<<<<<<<<<<<
- *         return result
- * 
- */
-  __pyx_t_1 = (__pyx_v_period >= __pyx_v_size);
-  if (__pyx_t_1) {
-
-    /* "src/mintalib/cython/curve.pxi":49
- * 
- *     if period >= size:
- *         return result             # <<<<<<<<<<<<<<
- * 
- *     s = sx = sxx = sy = syy = 0.0
- */
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_v_result);
-    __pyx_r = __pyx_v_result;
-    goto __pyx_L0;
-
-    /* "src/mintalib/cython/curve.pxi":48
- *     cdef long i = 0, j = 0
- * 
- *     if period >= size:             # <<<<<<<<<<<<<<
- *         return result
- * 
- */
-  }
-
-  /* "src/mintalib/cython/curve.pxi":51
- *         return result
- * 
- *     s = sx = sxx = sy = syy = 0.0             # <<<<<<<<<<<<<<
- * 
- *     x = (1 - period) / 2.0
- */
-  __pyx_v_s = 0.0;
-  __pyx_v_sx = 0.0;
-  __pyx_v_sxx = 0.0;
-  __pyx_v_sy = 0.0;
-  __pyx_v_syy = 0.0;
-
-  /* "src/mintalib/cython/curve.pxi":53
- *     s = sx = sxx = sy = syy = 0.0
- * 
- *     x = (1 - period) / 2.0             # <<<<<<<<<<<<<<
- *     for i in range(period):
- *         y = x * x
- */
-  __pyx_v_x = (((double)(1 - __pyx_v_period)) / 2.0);
-
-  /* "src/mintalib/cython/curve.pxi":54
- * 
- *     x = (1 - period) / 2.0
- *     for i in range(period):             # <<<<<<<<<<<<<<
- *         y = x * x
- *         s += 1
- */
-  __pyx_t_8 = __pyx_v_period;
-  __pyx_t_12 = __pyx_t_8;
-  for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
-    __pyx_v_i = __pyx_t_13;
-
-    /* "src/mintalib/cython/curve.pxi":55
- *     x = (1 - period) / 2.0
- *     for i in range(period):
- *         y = x * x             # <<<<<<<<<<<<<<
- *         s += 1
- *         sx += x
- */
-    __pyx_v_y = (__pyx_v_x * __pyx_v_x);
-
-    /* "src/mintalib/cython/curve.pxi":56
- *     for i in range(period):
- *         y = x * x
- *         s += 1             # <<<<<<<<<<<<<<
- *         sx += x
- *         sy += y
- */
-    __pyx_v_s = (__pyx_v_s + 1.0);
-
-    /* "src/mintalib/cython/curve.pxi":57
- *         y = x * x
- *         s += 1
- *         sx += x             # <<<<<<<<<<<<<<
- *         sy += y
- *         sxx += x*x
- */
-    __pyx_v_sx = (__pyx_v_sx + __pyx_v_x);
-
-    /* "src/mintalib/cython/curve.pxi":58
- *         s += 1
- *         sx += x
- *         sy += y             # <<<<<<<<<<<<<<
- *         sxx += x*x
- *         syy += y*y
- */
-    __pyx_v_sy = (__pyx_v_sy + __pyx_v_y);
-
-    /* "src/mintalib/cython/curve.pxi":59
- *         sx += x
- *         sy += y
- *         sxx += x*x             # <<<<<<<<<<<<<<
- *         syy += y*y
- *         x += 1.0
- */
-    __pyx_v_sxx = (__pyx_v_sxx + (__pyx_v_x * __pyx_v_x));
-
-    /* "src/mintalib/cython/curve.pxi":60
- *         sy += y
- *         sxx += x*x
- *         syy += y*y             # <<<<<<<<<<<<<<
- *         x += 1.0
- * 
- */
-    __pyx_v_syy = (__pyx_v_syy + (__pyx_v_y * __pyx_v_y));
-
-    /* "src/mintalib/cython/curve.pxi":61
- *         sxx += x*x
- *         syy += y*y
- *         x += 1.0             # <<<<<<<<<<<<<<
- * 
- *     vxx = (sxx / s - sx * sx / s / s )
- */
-    __pyx_v_x = (__pyx_v_x + 1.0);
-  }
-
-  /* "src/mintalib/cython/curve.pxi":63
- *         x += 1.0
- * 
- *     vxx = (sxx / s - sx * sx / s / s )             # <<<<<<<<<<<<<<
- *     vyy = (syy / s - sy * sy / s / s )
- * 
- */
-  if (unlikely(__pyx_v_s == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(36, 63, __pyx_L1_error)
-  }
-  __pyx_t_14 = (__pyx_v_sx * __pyx_v_sx);
-  if (unlikely(__pyx_v_s == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(36, 63, __pyx_L1_error)
-  }
-  __pyx_t_15 = (__pyx_t_14 / __pyx_v_s);
-  if (unlikely(__pyx_v_s == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(36, 63, __pyx_L1_error)
-  }
-  __pyx_v_vxx = ((__pyx_v_sxx / __pyx_v_s) - (__pyx_t_15 / __pyx_v_s));
-
-  /* "src/mintalib/cython/curve.pxi":64
- * 
- *     vxx = (sxx / s - sx * sx / s / s )
- *     vyy = (syy / s - sy * sy / s / s )             # <<<<<<<<<<<<<<
- * 
- *     if vxx <= 0 or vyy <= 0:
- */
-  if (unlikely(__pyx_v_s == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(36, 64, __pyx_L1_error)
-  }
-  __pyx_t_15 = (__pyx_v_sy * __pyx_v_sy);
-  if (unlikely(__pyx_v_s == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(36, 64, __pyx_L1_error)
-  }
-  __pyx_t_14 = (__pyx_t_15 / __pyx_v_s);
-  if (unlikely(__pyx_v_s == 0)) {
-    PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(36, 64, __pyx_L1_error)
-  }
-  __pyx_v_vyy = ((__pyx_v_syy / __pyx_v_s) - (__pyx_t_14 / __pyx_v_s));
-
-  /* "src/mintalib/cython/curve.pxi":66
- *     vyy = (syy / s - sy * sy / s / s )
- * 
- *     if vxx <= 0 or vyy <= 0:             # <<<<<<<<<<<<<<
- *         return result
- * 
- */
-  __pyx_t_2 = (__pyx_v_vxx <= 0.0);
-  if (!__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L10_bool_binop_done;
-  }
-  __pyx_t_2 = (__pyx_v_vyy <= 0.0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L10_bool_binop_done:;
-  if (__pyx_t_1) {
-
-    /* "src/mintalib/cython/curve.pxi":67
- * 
- *     if vxx <= 0 or vyy <= 0:
- *         return result             # <<<<<<<<<<<<<<
- * 
- *     for j in range(period - 1, size):
- */
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_v_result);
-    __pyx_r = __pyx_v_result;
-    goto __pyx_L0;
-
-    /* "src/mintalib/cython/curve.pxi":66
- *     vyy = (syy / s - sy * sy / s / s )
- * 
- *     if vxx <= 0 or vyy <= 0:             # <<<<<<<<<<<<<<
- *         return result
- * 
- */
-  }
-
-  /* "src/mintalib/cython/curve.pxi":69
- *         return result
- * 
- *     for j in range(period - 1, size):             # <<<<<<<<<<<<<<
- *         skip = False
- * 
- */
-  __pyx_t_8 = __pyx_v_size;
-  __pyx_t_12 = __pyx_t_8;
-  for (__pyx_t_13 = (__pyx_v_period - 1); __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
-    __pyx_v_j = __pyx_t_13;
-
-    /* "src/mintalib/cython/curve.pxi":70
- * 
- *     for j in range(period - 1, size):
- *         skip = False             # <<<<<<<<<<<<<<
- * 
- *         sz = sxz = szz = 0.0
- */
-    __pyx_v_skip = 0;
-
-    /* "src/mintalib/cython/curve.pxi":72
- *         skip = False
- * 
- *         sz = sxz = szz = 0.0             # <<<<<<<<<<<<<<
- *         x = (1 - period) / 2.0
- *         i = j - period + 1
- */
-    __pyx_v_sz = 0.0;
-    __pyx_v_sxz = 0.0;
-    __pyx_v_szz = 0.0;
-
-    /* "src/mintalib/cython/curve.pxi":73
- * 
- *         sz = sxz = szz = 0.0
- *         x = (1 - period) / 2.0             # <<<<<<<<<<<<<<
- *         i = j - period + 1
- *         while i <= j:
- */
-    __pyx_v_x = (((double)(1 - __pyx_v_period)) / 2.0);
-
-    /* "src/mintalib/cython/curve.pxi":74
- *         sz = sxz = szz = 0.0
- *         x = (1 - period) / 2.0
- *         i = j - period + 1             # <<<<<<<<<<<<<<
- *         while i <= j:
- *             z = zs[i]
- */
-    __pyx_v_i = ((__pyx_v_j - __pyx_v_period) + 1);
-
-    /* "src/mintalib/cython/curve.pxi":75
- *         x = (1 - period) / 2.0
- *         i = j - period + 1
- *         while i <= j:             # <<<<<<<<<<<<<<
- *             z = zs[i]
- *             if isnan(z):
- */
-    while (1) {
-      __pyx_t_1 = (__pyx_v_i <= __pyx_v_j);
-      if (!__pyx_t_1) break;
-
-      /* "src/mintalib/cython/curve.pxi":76
- *         i = j - period + 1
- *         while i <= j:
- *             z = zs[i]             # <<<<<<<<<<<<<<
- *             if isnan(z):
- *                 skip = True
- */
-      __pyx_t_16 = __pyx_v_i;
-      __pyx_t_6 = -1;
-      if (__pyx_t_16 < 0) {
-        __pyx_t_16 += __pyx_v_zs.shape[0];
-        if (unlikely(__pyx_t_16 < 0)) __pyx_t_6 = 0;
-      } else if (unlikely(__pyx_t_16 >= __pyx_v_zs.shape[0])) __pyx_t_6 = 0;
-      if (unlikely(__pyx_t_6 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_6);
-        __PYX_ERR(36, 76, __pyx_L1_error)
-      }
-      __pyx_v_z = (*((double const  *) ( /* dim=0 */ (__pyx_v_zs.data + __pyx_t_16 * __pyx_v_zs.strides[0]) )));
-
-      /* "src/mintalib/cython/curve.pxi":77
- *         while i <= j:
- *             z = zs[i]
- *             if isnan(z):             # <<<<<<<<<<<<<<
- *                 skip = True
- *                 break
- */
-      __pyx_t_1 = isnan(__pyx_v_z);
-      if (__pyx_t_1) {
-
-        /* "src/mintalib/cython/curve.pxi":78
- *             z = zs[i]
- *             if isnan(z):
- *                 skip = True             # <<<<<<<<<<<<<<
- *                 break
- *             sz += z
- */
-        __pyx_v_skip = 1;
-
-        /* "src/mintalib/cython/curve.pxi":79
- *             if isnan(z):
- *                 skip = True
- *                 break             # <<<<<<<<<<<<<<
- *             sz += z
- *             sxz += x * z
- */
-        goto __pyx_L15_break;
-
-        /* "src/mintalib/cython/curve.pxi":77
- *         while i <= j:
- *             z = zs[i]
- *             if isnan(z):             # <<<<<<<<<<<<<<
- *                 skip = True
- *                 break
- */
-      }
-
-      /* "src/mintalib/cython/curve.pxi":80
- *                 skip = True
- *                 break
- *             sz += z             # <<<<<<<<<<<<<<
- *             sxz += x * z
- *             szz += z * z
- */
-      __pyx_v_sz = (__pyx_v_sz + __pyx_v_z);
-
-      /* "src/mintalib/cython/curve.pxi":81
- *                 break
- *             sz += z
- *             sxz += x * z             # <<<<<<<<<<<<<<
- *             szz += z * z
- *             i += 1
- */
-      __pyx_v_sxz = (__pyx_v_sxz + (__pyx_v_x * __pyx_v_z));
-
-      /* "src/mintalib/cython/curve.pxi":82
- *             sz += z
- *             sxz += x * z
- *             szz += z * z             # <<<<<<<<<<<<<<
- *             i += 1
- *             x += 1.0
- */
-      __pyx_v_szz = (__pyx_v_szz + (__pyx_v_z * __pyx_v_z));
-
-      /* "src/mintalib/cython/curve.pxi":83
- *             sxz += x * z
- *             szz += z * z
- *             i += 1             # <<<<<<<<<<<<<<
- *             x += 1.0
- * 
- */
-      __pyx_v_i = (__pyx_v_i + 1);
-
-      /* "src/mintalib/cython/curve.pxi":84
- *             szz += z * z
- *             i += 1
- *             x += 1.0             # <<<<<<<<<<<<<<
- * 
- *         if skip:
- */
-      __pyx_v_x = (__pyx_v_x + 1.0);
-    }
-    __pyx_L15_break:;
-
-    /* "src/mintalib/cython/curve.pxi":86
- *             x += 1.0
- * 
- *         if skip:             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-    if (__pyx_v_skip) {
-
-      /* "src/mintalib/cython/curve.pxi":87
- * 
- *         if skip:
- *             continue             # <<<<<<<<<<<<<<
- * 
- *         vxz = (sxz / s - sx * sz / s / s)
- */
-      goto __pyx_L12_continue;
-
-      /* "src/mintalib/cython/curve.pxi":86
- *             x += 1.0
- * 
- *         if skip:             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-    }
-
-    /* "src/mintalib/cython/curve.pxi":89
- *             continue
- * 
- *         vxz = (sxz / s - sx * sz / s / s)             # <<<<<<<<<<<<<<
- *         vzz = (szz / s - sz * sz / s / s)
- * 
- */
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 89, __pyx_L1_error)
-    }
-    __pyx_t_14 = (__pyx_v_sx * __pyx_v_sz);
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 89, __pyx_L1_error)
-    }
-    __pyx_t_15 = (__pyx_t_14 / __pyx_v_s);
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 89, __pyx_L1_error)
-    }
-    __pyx_v_vxz = ((__pyx_v_sxz / __pyx_v_s) - (__pyx_t_15 / __pyx_v_s));
-
-    /* "src/mintalib/cython/curve.pxi":90
- * 
- *         vxz = (sxz / s - sx * sz / s / s)
- *         vzz = (szz / s - sz * sz / s / s)             # <<<<<<<<<<<<<<
- * 
- *         slope = vxz / vxx
- */
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 90, __pyx_L1_error)
-    }
-    __pyx_t_15 = (__pyx_v_sz * __pyx_v_sz);
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 90, __pyx_L1_error)
-    }
-    __pyx_t_14 = (__pyx_t_15 / __pyx_v_s);
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 90, __pyx_L1_error)
-    }
-    __pyx_v_vzz = ((__pyx_v_szz / __pyx_v_s) - (__pyx_t_14 / __pyx_v_s));
-
-    /* "src/mintalib/cython/curve.pxi":92
- *         vzz = (szz / s - sz * sz / s / s)
- * 
- *         slope = vxz / vxx             # <<<<<<<<<<<<<<
- * 
- *         if option == CURVE_OPTION_SLOPE:
- */
-    if (unlikely(__pyx_v_vxx == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 92, __pyx_L1_error)
-    }
-    __pyx_v_slope = (__pyx_v_vxz / __pyx_v_vxx);
-
-    /* "src/mintalib/cython/curve.pxi":94
- *         slope = vxz / vxx
- * 
- *         if option == CURVE_OPTION_SLOPE:             # <<<<<<<<<<<<<<
- *             output[j] = slope
- *             continue
- */
-    __pyx_t_1 = (__pyx_v_option == __pyx_e_8mintalib_4core_CURVE_OPTION_SLOPE);
-    if (__pyx_t_1) {
-
-      /* "src/mintalib/cython/curve.pxi":95
- * 
- *         if option == CURVE_OPTION_SLOPE:
- *             output[j] = slope             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-      __pyx_t_16 = __pyx_v_j;
-      __pyx_t_6 = -1;
-      if (__pyx_t_16 < 0) {
-        __pyx_t_16 += __pyx_v_output.shape[0];
-        if (unlikely(__pyx_t_16 < 0)) __pyx_t_6 = 0;
-      } else if (unlikely(__pyx_t_16 >= __pyx_v_output.shape[0])) __pyx_t_6 = 0;
-      if (unlikely(__pyx_t_6 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_6);
-        __PYX_ERR(36, 95, __pyx_L1_error)
-      }
-      *((double *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_16 * __pyx_v_output.strides[0]) )) = __pyx_v_slope;
-
-      /* "src/mintalib/cython/curve.pxi":96
- *         if option == CURVE_OPTION_SLOPE:
- *             output[j] = slope
- *             continue             # <<<<<<<<<<<<<<
- * 
- *         sz = syz = szz = 0.0
- */
-      goto __pyx_L12_continue;
-
-      /* "src/mintalib/cython/curve.pxi":94
- *         slope = vxz / vxx
- * 
- *         if option == CURVE_OPTION_SLOPE:             # <<<<<<<<<<<<<<
- *             output[j] = slope
- *             continue
- */
-    }
-
-    /* "src/mintalib/cython/curve.pxi":98
- *             continue
- * 
- *         sz = syz = szz = 0.0             # <<<<<<<<<<<<<<
- *         x = (1 - period) / 2.0
- *         i = j - period + 1
- */
-    __pyx_v_sz = 0.0;
-    __pyx_v_syz = 0.0;
-    __pyx_v_szz = 0.0;
-
-    /* "src/mintalib/cython/curve.pxi":99
- * 
- *         sz = syz = szz = 0.0
- *         x = (1 - period) / 2.0             # <<<<<<<<<<<<<<
- *         i = j - period + 1
- *         while i <= j:
- */
-    __pyx_v_x = (((double)(1 - __pyx_v_period)) / 2.0);
-
-    /* "src/mintalib/cython/curve.pxi":100
- *         sz = syz = szz = 0.0
- *         x = (1 - period) / 2.0
- *         i = j - period + 1             # <<<<<<<<<<<<<<
- *         while i <= j:
- *             y = x * x
- */
-    __pyx_v_i = ((__pyx_v_j - __pyx_v_period) + 1);
-
-    /* "src/mintalib/cython/curve.pxi":101
- *         x = (1 - period) / 2.0
- *         i = j - period + 1
- *         while i <= j:             # <<<<<<<<<<<<<<
- *             y = x * x
- *             z = zs[i] - slope * x
- */
-    while (1) {
-      __pyx_t_1 = (__pyx_v_i <= __pyx_v_j);
-      if (!__pyx_t_1) break;
-
-      /* "src/mintalib/cython/curve.pxi":102
- *         i = j - period + 1
- *         while i <= j:
- *             y = x * x             # <<<<<<<<<<<<<<
- *             z = zs[i] - slope * x
- *             if isnan(z):
- */
-      __pyx_v_y = (__pyx_v_x * __pyx_v_x);
-
-      /* "src/mintalib/cython/curve.pxi":103
- *         while i <= j:
- *             y = x * x
- *             z = zs[i] - slope * x             # <<<<<<<<<<<<<<
- *             if isnan(z):
- *                 skip = True
- */
-      __pyx_t_16 = __pyx_v_i;
-      __pyx_t_6 = -1;
-      if (__pyx_t_16 < 0) {
-        __pyx_t_16 += __pyx_v_zs.shape[0];
-        if (unlikely(__pyx_t_16 < 0)) __pyx_t_6 = 0;
-      } else if (unlikely(__pyx_t_16 >= __pyx_v_zs.shape[0])) __pyx_t_6 = 0;
-      if (unlikely(__pyx_t_6 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_6);
-        __PYX_ERR(36, 103, __pyx_L1_error)
-      }
-      __pyx_v_z = ((*((double const  *) ( /* dim=0 */ (__pyx_v_zs.data + __pyx_t_16 * __pyx_v_zs.strides[0]) ))) - (__pyx_v_slope * __pyx_v_x));
-
-      /* "src/mintalib/cython/curve.pxi":104
- *             y = x * x
- *             z = zs[i] - slope * x
- *             if isnan(z):             # <<<<<<<<<<<<<<
- *                 skip = True
- *                 break
- */
-      __pyx_t_1 = isnan(__pyx_v_z);
-      if (__pyx_t_1) {
-
-        /* "src/mintalib/cython/curve.pxi":105
- *             z = zs[i] - slope * x
- *             if isnan(z):
- *                 skip = True             # <<<<<<<<<<<<<<
- *                 break
- *             sz += z
- */
-        __pyx_v_skip = 1;
-
-        /* "src/mintalib/cython/curve.pxi":106
- *             if isnan(z):
- *                 skip = True
- *                 break             # <<<<<<<<<<<<<<
- *             sz += z
- *             syz += y * z
- */
-        goto __pyx_L20_break;
-
-        /* "src/mintalib/cython/curve.pxi":104
- *             y = x * x
- *             z = zs[i] - slope * x
- *             if isnan(z):             # <<<<<<<<<<<<<<
- *                 skip = True
- *                 break
- */
-      }
-
-      /* "src/mintalib/cython/curve.pxi":107
- *                 skip = True
- *                 break
- *             sz += z             # <<<<<<<<<<<<<<
- *             syz += y * z
- *             szz += z * z
- */
-      __pyx_v_sz = (__pyx_v_sz + __pyx_v_z);
-
-      /* "src/mintalib/cython/curve.pxi":108
- *                 break
- *             sz += z
- *             syz += y * z             # <<<<<<<<<<<<<<
- *             szz += z * z
- *             i += 1
- */
-      __pyx_v_syz = (__pyx_v_syz + (__pyx_v_y * __pyx_v_z));
-
-      /* "src/mintalib/cython/curve.pxi":109
- *             sz += z
- *             syz += y * z
- *             szz += z * z             # <<<<<<<<<<<<<<
- *             i += 1
- *             x += 1.0
- */
-      __pyx_v_szz = (__pyx_v_szz + (__pyx_v_z * __pyx_v_z));
-
-      /* "src/mintalib/cython/curve.pxi":110
- *             syz += y * z
- *             szz += z * z
- *             i += 1             # <<<<<<<<<<<<<<
- *             x += 1.0
- * 
- */
-      __pyx_v_i = (__pyx_v_i + 1);
-
-      /* "src/mintalib/cython/curve.pxi":111
- *             szz += z * z
- *             i += 1
- *             x += 1.0             # <<<<<<<<<<<<<<
- * 
- *         if skip:
- */
-      __pyx_v_x = (__pyx_v_x + 1.0);
-    }
-    __pyx_L20_break:;
-
-    /* "src/mintalib/cython/curve.pxi":113
- *             x += 1.0
- * 
- *         if skip:             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-    if (__pyx_v_skip) {
-
-      /* "src/mintalib/cython/curve.pxi":114
- * 
- *         if skip:
- *             continue             # <<<<<<<<<<<<<<
- * 
- *         vyz = (syz / s - sy * sz / s / s)
- */
-      goto __pyx_L12_continue;
-
-      /* "src/mintalib/cython/curve.pxi":113
- *             x += 1.0
- * 
- *         if skip:             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-    }
-
-    /* "src/mintalib/cython/curve.pxi":116
- *             continue
- * 
- *         vyz = (syz / s - sy * sz / s / s)             # <<<<<<<<<<<<<<
- *         vzz = (szz / s - sz * sz / s / s)
- * 
- */
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 116, __pyx_L1_error)
-    }
-    __pyx_t_14 = (__pyx_v_sy * __pyx_v_sz);
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 116, __pyx_L1_error)
-    }
-    __pyx_t_15 = (__pyx_t_14 / __pyx_v_s);
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 116, __pyx_L1_error)
-    }
-    __pyx_v_vyz = ((__pyx_v_syz / __pyx_v_s) - (__pyx_t_15 / __pyx_v_s));
-
-    /* "src/mintalib/cython/curve.pxi":117
- * 
- *         vyz = (syz / s - sy * sz / s / s)
- *         vzz = (szz / s - sz * sz / s / s)             # <<<<<<<<<<<<<<
- * 
- *         curve = vyz / vyy
- */
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 117, __pyx_L1_error)
-    }
-    __pyx_t_15 = (__pyx_v_sz * __pyx_v_sz);
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 117, __pyx_L1_error)
-    }
-    __pyx_t_14 = (__pyx_t_15 / __pyx_v_s);
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 117, __pyx_L1_error)
-    }
-    __pyx_v_vzz = ((__pyx_v_szz / __pyx_v_s) - (__pyx_t_14 / __pyx_v_s));
-
-    /* "src/mintalib/cython/curve.pxi":119
- *         vzz = (szz / s - sz * sz / s / s)
- * 
- *         curve = vyz / vyy             # <<<<<<<<<<<<<<
- *         intercept = (sz - curve * sy) / s
- *         rvalue = vyz / math.sqrt(vyy * vzz) if vyy * vzz > 0 else NAN
- */
-    if (unlikely(__pyx_v_vyy == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 119, __pyx_L1_error)
-    }
-    __pyx_v_curve = (__pyx_v_vyz / __pyx_v_vyy);
-
-    /* "src/mintalib/cython/curve.pxi":120
- * 
- *         curve = vyz / vyy
- *         intercept = (sz - curve * sy) / s             # <<<<<<<<<<<<<<
- *         rvalue = vyz / math.sqrt(vyy * vzz) if vyy * vzz > 0 else NAN
- *         mse = (1.0 - rvalue * rvalue) * vzz
- */
-    __pyx_t_14 = (__pyx_v_sz - (__pyx_v_curve * __pyx_v_sy));
-    if (unlikely(__pyx_v_s == 0)) {
-      PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(36, 120, __pyx_L1_error)
-    }
-    __pyx_v_intercept = (__pyx_t_14 / __pyx_v_s);
-
-    /* "src/mintalib/cython/curve.pxi":121
- *         curve = vyz / vyy
- *         intercept = (sz - curve * sy) / s
- *         rvalue = vyz / math.sqrt(vyy * vzz) if vyy * vzz > 0 else NAN             # <<<<<<<<<<<<<<
- *         mse = (1.0 - rvalue * rvalue) * vzz
- *         rmse = math.sqrt(mse) if mse >= 0 else NAN
- */
-    __pyx_t_1 = ((__pyx_v_vyy * __pyx_v_vzz) > 0.0);
-    if (__pyx_t_1) {
-      __pyx_t_15 = sqrt((__pyx_v_vyy * __pyx_v_vzz));
-      if (unlikely(__pyx_t_15 == 0)) {
-        PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-        __PYX_ERR(36, 121, __pyx_L1_error)
-      }
-      __pyx_t_14 = (__pyx_v_vyz / __pyx_t_15);
-    } else {
-      __pyx_t_14 = __pyx_v_8mintalib_4core_NAN;
-    }
-    __pyx_v_rvalue = __pyx_t_14;
-
-    /* "src/mintalib/cython/curve.pxi":122
- *         intercept = (sz - curve * sy) / s
- *         rvalue = vyz / math.sqrt(vyy * vzz) if vyy * vzz > 0 else NAN
- *         mse = (1.0 - rvalue * rvalue) * vzz             # <<<<<<<<<<<<<<
- *         rmse = math.sqrt(mse) if mse >= 0 else NAN
- * 
- */
-    __pyx_v_mse = ((1.0 - (__pyx_v_rvalue * __pyx_v_rvalue)) * __pyx_v_vzz);
-
-    /* "src/mintalib/cython/curve.pxi":123
- *         rvalue = vyz / math.sqrt(vyy * vzz) if vyy * vzz > 0 else NAN
- *         mse = (1.0 - rvalue * rvalue) * vzz
- *         rmse = math.sqrt(mse) if mse >= 0 else NAN             # <<<<<<<<<<<<<<
- * 
- * 
- */
-    __pyx_t_1 = (__pyx_v_mse >= 0.0);
-    if (__pyx_t_1) {
-      __pyx_t_14 = sqrt(__pyx_v_mse);
-    } else {
-      __pyx_t_14 = __pyx_v_8mintalib_4core_NAN;
-    }
-    __pyx_v_rmse = __pyx_t_14;
-
-    /* "src/mintalib/cython/curve.pxi":126
- * 
- * 
- *         if option == CURVE_OPTION_CURVE:             # <<<<<<<<<<<<<<
- *             output[j] = curve
- *             continue
- */
-    __pyx_t_1 = (__pyx_v_option == __pyx_e_8mintalib_4core_CURVE_OPTION_CURVE);
-    if (__pyx_t_1) {
-
-      /* "src/mintalib/cython/curve.pxi":127
- * 
- *         if option == CURVE_OPTION_CURVE:
- *             output[j] = curve             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-      __pyx_t_16 = __pyx_v_j;
-      __pyx_t_6 = -1;
-      if (__pyx_t_16 < 0) {
-        __pyx_t_16 += __pyx_v_output.shape[0];
-        if (unlikely(__pyx_t_16 < 0)) __pyx_t_6 = 0;
-      } else if (unlikely(__pyx_t_16 >= __pyx_v_output.shape[0])) __pyx_t_6 = 0;
-      if (unlikely(__pyx_t_6 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_6);
-        __PYX_ERR(36, 127, __pyx_L1_error)
-      }
-      *((double *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_16 * __pyx_v_output.strides[0]) )) = __pyx_v_curve;
-
-      /* "src/mintalib/cython/curve.pxi":128
- *         if option == CURVE_OPTION_CURVE:
- *             output[j] = curve
- *             continue             # <<<<<<<<<<<<<<
- * 
- *         if option == CURVE_OPTION_RVALUE:
- */
-      goto __pyx_L12_continue;
-
-      /* "src/mintalib/cython/curve.pxi":126
- * 
- * 
- *         if option == CURVE_OPTION_CURVE:             # <<<<<<<<<<<<<<
- *             output[j] = curve
- *             continue
- */
-    }
-
-    /* "src/mintalib/cython/curve.pxi":130
- *             continue
- * 
- *         if option == CURVE_OPTION_RVALUE:             # <<<<<<<<<<<<<<
- *             output[j] = rvalue
- *             continue
- */
-    __pyx_t_1 = (__pyx_v_option == __pyx_e_8mintalib_4core_CURVE_OPTION_RVALUE);
-    if (__pyx_t_1) {
-
-      /* "src/mintalib/cython/curve.pxi":131
- * 
- *         if option == CURVE_OPTION_RVALUE:
- *             output[j] = rvalue             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-      __pyx_t_16 = __pyx_v_j;
-      __pyx_t_6 = -1;
-      if (__pyx_t_16 < 0) {
-        __pyx_t_16 += __pyx_v_output.shape[0];
-        if (unlikely(__pyx_t_16 < 0)) __pyx_t_6 = 0;
-      } else if (unlikely(__pyx_t_16 >= __pyx_v_output.shape[0])) __pyx_t_6 = 0;
-      if (unlikely(__pyx_t_6 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_6);
-        __PYX_ERR(36, 131, __pyx_L1_error)
-      }
-      *((double *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_16 * __pyx_v_output.strides[0]) )) = __pyx_v_rvalue;
-
-      /* "src/mintalib/cython/curve.pxi":132
- *         if option == CURVE_OPTION_RVALUE:
- *             output[j] = rvalue
- *             continue             # <<<<<<<<<<<<<<
- * 
- *         if option == CURVE_OPTION_RSQUARE:
- */
-      goto __pyx_L12_continue;
-
-      /* "src/mintalib/cython/curve.pxi":130
- *             continue
- * 
- *         if option == CURVE_OPTION_RVALUE:             # <<<<<<<<<<<<<<
- *             output[j] = rvalue
- *             continue
- */
-    }
-
-    /* "src/mintalib/cython/curve.pxi":134
- *             continue
- * 
- *         if option == CURVE_OPTION_RSQUARE:             # <<<<<<<<<<<<<<
- *             output[j] = rvalue * rvalue
- *             continue
- */
-    __pyx_t_1 = (__pyx_v_option == __pyx_e_8mintalib_4core_CURVE_OPTION_RSQUARE);
-    if (__pyx_t_1) {
-
-      /* "src/mintalib/cython/curve.pxi":135
- * 
- *         if option == CURVE_OPTION_RSQUARE:
- *             output[j] = rvalue * rvalue             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-      __pyx_t_16 = __pyx_v_j;
-      __pyx_t_6 = -1;
-      if (__pyx_t_16 < 0) {
-        __pyx_t_16 += __pyx_v_output.shape[0];
-        if (unlikely(__pyx_t_16 < 0)) __pyx_t_6 = 0;
-      } else if (unlikely(__pyx_t_16 >= __pyx_v_output.shape[0])) __pyx_t_6 = 0;
-      if (unlikely(__pyx_t_6 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_6);
-        __PYX_ERR(36, 135, __pyx_L1_error)
-      }
-      *((double *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_16 * __pyx_v_output.strides[0]) )) = (__pyx_v_rvalue * __pyx_v_rvalue);
-
-      /* "src/mintalib/cython/curve.pxi":136
- *         if option == CURVE_OPTION_RSQUARE:
- *             output[j] = rvalue * rvalue
- *             continue             # <<<<<<<<<<<<<<
- * 
- *         if option == CURVE_OPTION_RMSERROR:
- */
-      goto __pyx_L12_continue;
-
-      /* "src/mintalib/cython/curve.pxi":134
- *             continue
- * 
- *         if option == CURVE_OPTION_RSQUARE:             # <<<<<<<<<<<<<<
- *             output[j] = rvalue * rvalue
- *             continue
- */
-    }
-
-    /* "src/mintalib/cython/curve.pxi":138
- *             continue
- * 
- *         if option == CURVE_OPTION_RMSERROR:             # <<<<<<<<<<<<<<
- *             output[j] = rmse
- *             continue
- */
-    __pyx_t_1 = (__pyx_v_option == __pyx_e_8mintalib_4core_CURVE_OPTION_RMSERROR);
-    if (__pyx_t_1) {
-
-      /* "src/mintalib/cython/curve.pxi":139
- * 
- *         if option == CURVE_OPTION_RMSERROR:
- *             output[j] = rmse             # <<<<<<<<<<<<<<
- *             continue
- * 
- */
-      __pyx_t_16 = __pyx_v_j;
-      __pyx_t_6 = -1;
-      if (__pyx_t_16 < 0) {
-        __pyx_t_16 += __pyx_v_output.shape[0];
-        if (unlikely(__pyx_t_16 < 0)) __pyx_t_6 = 0;
-      } else if (unlikely(__pyx_t_16 >= __pyx_v_output.shape[0])) __pyx_t_6 = 0;
-      if (unlikely(__pyx_t_6 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_6);
-        __PYX_ERR(36, 139, __pyx_L1_error)
-      }
-      *((double *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_16 * __pyx_v_output.strides[0]) )) = __pyx_v_rmse;
-
-      /* "src/mintalib/cython/curve.pxi":140
- *         if option == CURVE_OPTION_RMSERROR:
- *             output[j] = rmse
- *             continue             # <<<<<<<<<<<<<<
- * 
- *     if wrap:
- */
-      goto __pyx_L12_continue;
-
-      /* "src/mintalib/cython/curve.pxi":138
- *             continue
- * 
- *         if option == CURVE_OPTION_RMSERROR:             # <<<<<<<<<<<<<<
- *             output[j] = rmse
- *             continue
- */
-    }
-    __pyx_L12_continue:;
-  }
-
-  /* "src/mintalib/cython/curve.pxi":142
- *             continue
- * 
- *     if wrap:             # <<<<<<<<<<<<<<
- *         result = wrap_result(result, series)
- * 
- */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_wrap); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(36, 142, __pyx_L1_error)
-  if (__pyx_t_1) {
-
-    /* "src/mintalib/cython/curve.pxi":143
- * 
- *     if wrap:
- *         result = wrap_result(result, series)             # <<<<<<<<<<<<<<
- * 
- *     return result
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 143, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = NULL;
-    __pyx_t_6 = 0;
-    #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_10)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_10);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
-        __pyx_t_6 = 1;
-      }
-    }
-    #endif
-    {
-      PyObject *__pyx_callargs[3] = {__pyx_t_10, __pyx_v_result, __pyx_v_series};
-      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
-      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 143, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    }
-    __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_5);
-    __pyx_t_5 = 0;
-
-    /* "src/mintalib/cython/curve.pxi":142
- *             continue
- * 
- *     if wrap:             # <<<<<<<<<<<<<<
- *         result = wrap_result(result, series)
- * 
- */
-  }
-
-  /* "src/mintalib/cython/curve.pxi":145
- *         result = wrap_result(result, series)
- * 
- *     return result             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_result);
-  __pyx_r = __pyx_v_result;
-  goto __pyx_L0;
-
-  /* "src/mintalib/cython/curve.pxi":25
- * 
- * 
- * def calc_curve(series, long period=20, *, int option=0, int offset=0, wrap: bool = False):             # <<<<<<<<<<<<<<
- *     """ Curve (time curvilinear regression) """
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __PYX_XCLEAR_MEMVIEW(&__pyx_t_7, 1);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_10);
-  __PYX_XCLEAR_MEMVIEW(&__pyx_t_11, 1);
-  __Pyx_AddTraceback("mintalib.core.calc_curve", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __PYX_XCLEAR_MEMVIEW(&__pyx_v_zs, 1);
-  __Pyx_XDECREF(__pyx_v_result);
-  __PYX_XCLEAR_MEMVIEW(&__pyx_v_output, 1);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "src/mintalib/cython/curve.pxi":149
- * 
- * 
- * @wrap_function(calc_curve)             # <<<<<<<<<<<<<<
- * def CURVE(series, period: int = 20, *, item: str = None):
- *     """ Curve (time curvilinear regression) """
- */
-
-static PyObject *__pyx_pf_8mintalib_4core_299__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__defaults__", 1);
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_period);
-  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_period);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_period)) __PYX_ERR(36, 149, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-
-  /* "src/mintalib/cython/curve.pxi":150
- * 
- * @wrap_function(calc_curve)
- * def CURVE(series, period: int = 20, *, item: str = None):             # <<<<<<<<<<<<<<
- *     """ Curve (time curvilinear regression) """
- * 
- */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_item, Py_None) < 0) __PYX_ERR(36, 149, __pyx_L1_error)
-
-  /* "src/mintalib/cython/curve.pxi":149
- * 
- * 
- * @wrap_function(calc_curve)             # <<<<<<<<<<<<<<
- * def CURVE(series, period: int = 20, *, item: str = None):
- *     """ Curve (time curvilinear regression) """
- */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(36, 149, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(36, 149, __pyx_L1_error);
-  __pyx_t_1 = 0;
-  __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_3;
-  __pyx_t_3 = 0;
-  goto __pyx_L0;
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("mintalib.core.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_209CURVE(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8mintalib_4core_208CURVE, " Curve (time curvilinear regression) ");
-static PyMethodDef __pyx_mdef_8mintalib_4core_209CURVE = {"CURVE", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_209CURVE, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8mintalib_4core_208CURVE};
-static PyObject *__pyx_pw_8mintalib_4core_209CURVE(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_series = 0;
-  PyObject *__pyx_v_period = 0;
-  PyObject *__pyx_v_item = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[3] = {0,0,0};
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("CURVE (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_series,&__pyx_n_s_period,&__pyx_n_s_item,0};
-    __pyx_defaults35 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self);
-    values[1] = __Pyx_Arg_NewRef_FASTCALL(__pyx_dynamic_args->__pyx_arg_period);
-
-    /* "src/mintalib/cython/curve.pxi":150
- * 
- * @wrap_function(calc_curve)
- * def CURVE(series, period: int = 20, *, item: str = None):             # <<<<<<<<<<<<<<
- *     """ Curve (time curvilinear regression) """
- * 
- */
-    values[2] = __Pyx_Arg_NewRef_FASTCALL(((PyObject*)Py_None));
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_series)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 149, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_period);
-          if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 149, __pyx_L3_error)
-        }
-      }
-      if (kw_args == 1) {
-        const Py_ssize_t index = 2;
-        PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
-        if (value) { values[index] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 149, __pyx_L3_error)
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "CURVE") < 0)) __PYX_ERR(36, 149, __pyx_L3_error)
-      }
-    } else {
-      switch (__pyx_nargs) {
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_series = values[0];
-    __pyx_v_period = ((PyObject*)values[1]);
-    __pyx_v_item = ((PyObject*)values[2]);
-  }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("CURVE", 0, 1, 2, __pyx_nargs); __PYX_ERR(36, 149, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_AddTraceback("mintalib.core.CURVE", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_period), (&PyInt_Type), 0, "period", 1))) __PYX_ERR(36, 150, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_item), (&PyUnicode_Type), 1, "item", 1))) __PYX_ERR(36, 150, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8mintalib_4core_208CURVE(__pyx_self, __pyx_v_series, __pyx_v_period, __pyx_v_item);
-
-  /* "src/mintalib/cython/curve.pxi":149
- * 
- * 
- * @wrap_function(calc_curve)             # <<<<<<<<<<<<<<
- * def CURVE(series, period: int = 20, *, item: str = None):
- *     """ Curve (time curvilinear regression) """
- */
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_8mintalib_4core_208CURVE(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_period, PyObject *__pyx_v_item) {
-  PyObject *__pyx_v_result = NULL;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("CURVE", 0);
-  __Pyx_INCREF(__pyx_v_series);
-
-  /* "src/mintalib/cython/curve.pxi":153
- *     """ Curve (time curvilinear regression) """
- * 
- *     series = get_series(series, item=item)             # <<<<<<<<<<<<<<
- *     result = calc_curve(series, period=period, option=CURVE_OPTION_CURVE)
- *     return wrap_result(result, series)
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_series); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 153, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 153, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_v_series);
-  __Pyx_GIVEREF(__pyx_v_series);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_series)) __PYX_ERR(36, 153, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 153, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_item, __pyx_v_item) < 0) __PYX_ERR(36, 153, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 153, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF_SET(__pyx_v_series, __pyx_t_4);
-  __pyx_t_4 = 0;
-
-  /* "src/mintalib/cython/curve.pxi":154
- * 
- *     series = get_series(series, item=item)
- *     result = calc_curve(series, period=period, option=CURVE_OPTION_CURVE)             # <<<<<<<<<<<<<<
- *     return wrap_result(result, series)
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_calc_curve); if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_INCREF(__pyx_v_series);
-  __Pyx_GIVEREF(__pyx_v_series);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_series)) __PYX_ERR(36, 154, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_period, __pyx_v_period) < 0) __PYX_ERR(36, 154, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyInt_From___pyx_anon_enum(__pyx_e_8mintalib_4core_CURVE_OPTION_CURVE); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_option, __pyx_t_1) < 0) __PYX_ERR(36, 154, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_result = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "src/mintalib/cython/curve.pxi":155
- *     series = get_series(series, item=item)
- *     result = calc_curve(series, period=period, option=CURVE_OPTION_CURVE)
- *     return wrap_result(result, series)             # <<<<<<<<<<<<<<
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 155, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  __pyx_t_5 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-      __pyx_t_5 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_result, __pyx_v_series};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 155, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "src/mintalib/cython/curve.pxi":149
- * 
- * 
- * @wrap_function(calc_curve)             # <<<<<<<<<<<<<<
- * def CURVE(series, period: int = 20, *, item: str = None):
- *     """ Curve (time curvilinear regression) """
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("mintalib.core.CURVE", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_result);
-  __Pyx_XDECREF(__pyx_v_series);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* "src/mintalib/cython/stoch.pxi":6
  * stoch_result = namedtuple("stoch_result", "slowk, slowd")
  * 
  * def calc_stoch(prices, long period=14, long fastn=3, long slown=3, *, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Stochastic Oscillator """
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_211calc_stoch(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8mintalib_4core_207calc_stoch(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8mintalib_4core_210calc_stoch, " Stochastic Oscillator ");
-static PyMethodDef __pyx_mdef_8mintalib_4core_211calc_stoch = {"calc_stoch", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_211calc_stoch, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8mintalib_4core_210calc_stoch};
-static PyObject *__pyx_pw_8mintalib_4core_211calc_stoch(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_8mintalib_4core_206calc_stoch, " Stochastic Oscillator ");
+static PyMethodDef __pyx_mdef_8mintalib_4core_207calc_stoch = {"calc_stoch", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_207calc_stoch, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8mintalib_4core_206calc_stoch};
+static PyObject *__pyx_pw_8mintalib_4core_207calc_stoch(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_prices = 0;
@@ -68469,47 +66406,47 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_prices)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 6, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 6, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_period);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 6, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 6, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fastn);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 6, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 6, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_slown);
           if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 6, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 6, __pyx_L3_error)
         }
       }
       if (kw_args == 1) {
         const Py_ssize_t index = 4;
         PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
         if (value) { values[index] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 6, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 6, __pyx_L3_error)
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_stoch") < 0)) __PYX_ERR(37, 6, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_stoch") < 0)) __PYX_ERR(36, 6, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -68518,60 +66455,60 @@
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_prices = values[0];
     if (values[1]) {
-      __pyx_v_period = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v_period == (long)-1) && PyErr_Occurred())) __PYX_ERR(37, 6, __pyx_L3_error)
+      __pyx_v_period = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v_period == (long)-1) && PyErr_Occurred())) __PYX_ERR(36, 6, __pyx_L3_error)
     } else {
       __pyx_v_period = ((long)((long)14));
     }
     if (values[2]) {
-      __pyx_v_fastn = __Pyx_PyInt_As_long(values[2]); if (unlikely((__pyx_v_fastn == (long)-1) && PyErr_Occurred())) __PYX_ERR(37, 6, __pyx_L3_error)
+      __pyx_v_fastn = __Pyx_PyInt_As_long(values[2]); if (unlikely((__pyx_v_fastn == (long)-1) && PyErr_Occurred())) __PYX_ERR(36, 6, __pyx_L3_error)
     } else {
       __pyx_v_fastn = ((long)((long)3));
     }
     if (values[3]) {
-      __pyx_v_slown = __Pyx_PyInt_As_long(values[3]); if (unlikely((__pyx_v_slown == (long)-1) && PyErr_Occurred())) __PYX_ERR(37, 6, __pyx_L3_error)
+      __pyx_v_slown = __Pyx_PyInt_As_long(values[3]); if (unlikely((__pyx_v_slown == (long)-1) && PyErr_Occurred())) __PYX_ERR(36, 6, __pyx_L3_error)
     } else {
       __pyx_v_slown = ((long)((long)3));
     }
     __pyx_v_wrap = values[4];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calc_stoch", 0, 1, 4, __pyx_nargs); __PYX_ERR(37, 6, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calc_stoch", 0, 1, 4, __pyx_nargs); __PYX_ERR(36, 6, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("mintalib.core.calc_stoch", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8mintalib_4core_210calc_stoch(__pyx_self, __pyx_v_prices, __pyx_v_period, __pyx_v_fastn, __pyx_v_slown, __pyx_v_wrap);
+  __pyx_r = __pyx_pf_8mintalib_4core_206calc_stoch(__pyx_self, __pyx_v_prices, __pyx_v_period, __pyx_v_fastn, __pyx_v_slown, __pyx_v_wrap);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8mintalib_4core_210calc_stoch(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, long __pyx_v_fastn, long __pyx_v_slown, PyObject *__pyx_v_wrap) {
+static PyObject *__pyx_pf_8mintalib_4core_206calc_stoch(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, long __pyx_v_period, long __pyx_v_fastn, long __pyx_v_slown, PyObject *__pyx_v_wrap) {
   __Pyx_memviewslice __pyx_v_high = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_low = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_close = { 0, 0, { 0 }, { 0 }, { 0 } };
   CYTHON_UNUSED long __pyx_v_size;
   PyObject *__pyx_v_hi = NULL;
   PyObject *__pyx_v_lo = NULL;
   PyObject *__pyx_v_fastk = NULL;
@@ -68606,20 +66543,20 @@
   /* "src/mintalib/cython/stoch.pxi":9
  *     """ Stochastic Oscillator """
  * 
  *     cdef const double[:] high = np.asarray(prices['high'], float)             # <<<<<<<<<<<<<<
  *     cdef const double[:] low = np.asarray(prices['low'], float)
  *     cdef const double[:] close = np.asarray(prices['close'], float)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 9, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 9, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_prices, __pyx_n_u_high); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_prices, __pyx_n_u_high); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -68632,37 +66569,37 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_2, ((PyObject *)(&PyFloat_Type))};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 9, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_ds_double__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(37, 9, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_ds_double__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(36, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_high = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
   /* "src/mintalib/cython/stoch.pxi":10
  * 
  *     cdef const double[:] high = np.asarray(prices['high'], float)
  *     cdef const double[:] low = np.asarray(prices['low'], float)             # <<<<<<<<<<<<<<
  *     cdef const double[:] close = np.asarray(prices['close'], float)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 10, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 10, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_prices, __pyx_n_u_low); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 10, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_prices, __pyx_n_u_low); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -68675,37 +66612,37 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_3, ((PyObject *)(&PyFloat_Type))};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 10, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 10, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_double__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(37, 10, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_double__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(36, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_low = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
   /* "src/mintalib/cython/stoch.pxi":11
  *     cdef const double[:] high = np.asarray(prices['high'], float)
  *     cdef const double[:] low = np.asarray(prices['low'], float)
  *     cdef const double[:] close = np.asarray(prices['close'], float)             # <<<<<<<<<<<<<<
  * 
  *     cdef long size = check_size(high, low, close)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 11, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 11, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_prices, __pyx_n_u_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 11, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_prices, __pyx_n_u_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -68718,38 +66655,38 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_2, ((PyObject *)(&PyFloat_Type))};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 11, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 11, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_double__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(37, 11, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_double__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(36, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_close = __pyx_t_8;
   __pyx_t_8.memview = NULL;
   __pyx_t_8.data = NULL;
 
   /* "src/mintalib/cython/stoch.pxi":13
  *     cdef const double[:] close = np.asarray(prices['close'], float)
  * 
  *     cdef long size = check_size(high, low, close)             # <<<<<<<<<<<<<<
  * 
  *     hi = calc_max(high, period)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_check_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 13, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_check_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_high, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 13, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_high, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_low, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 13, __pyx_L1_error)
+  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_low, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_close, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(37, 13, __pyx_L1_error)
+  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_close, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_10 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_10)) {
@@ -68764,34 +66701,34 @@
   {
     PyObject *__pyx_callargs[4] = {__pyx_t_10, __pyx_t_2, __pyx_t_4, __pyx_t_9};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 3+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 13, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_1); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(37, 13, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_1); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(36, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_size = __pyx_t_11;
 
   /* "src/mintalib/cython/stoch.pxi":15
  *     cdef long size = check_size(high, low, close)
  * 
  *     hi = calc_max(high, period)             # <<<<<<<<<<<<<<
  *     lo = calc_min(low, period)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_calc_max); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 15, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_calc_max); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_high, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(37, 15, __pyx_L1_error)
+  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_high, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_period); if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 15, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_period); if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -68805,33 +66742,33 @@
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_t_9, __pyx_t_4};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 15, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_hi = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "src/mintalib/cython/stoch.pxi":16
  * 
  *     hi = calc_max(high, period)
  *     lo = calc_min(low, period)             # <<<<<<<<<<<<<<
  * 
  *     with np.errstate(divide='ignore'):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_calc_min); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 16, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_calc_min); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_low, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 16, __pyx_L1_error)
+  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_low, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __Pyx_PyInt_From_long(__pyx_v_period); if (unlikely(!__pyx_t_9)) __PYX_ERR(37, 16, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_From_long(__pyx_v_period); if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -68845,44 +66782,44 @@
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_t_4, __pyx_t_9};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 16, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 16, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_lo = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "src/mintalib/cython/stoch.pxi":18
  *     lo = calc_min(low, period)
  * 
  *     with np.errstate(divide='ignore'):             # <<<<<<<<<<<<<<
  *         fastk = 100 * (close - lo) /(hi - lo)
  * 
  */
   /*with:*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 18, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 18, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_errstate); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 18, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_errstate); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 18, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 18, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 18, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_divide, __pyx_n_u_ignore) < 0) __PYX_ERR(37, 18, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_9)) __PYX_ERR(37, 18, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_divide, __pyx_n_u_ignore) < 0) __PYX_ERR(36, 18, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 18, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_12 = __Pyx_PyObject_LookupSpecial(__pyx_t_9, __pyx_n_s_exit); if (unlikely(!__pyx_t_12)) __PYX_ERR(37, 18, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_LookupSpecial(__pyx_t_9, __pyx_n_s_exit); if (unlikely(!__pyx_t_12)) __PYX_ERR(36, 18, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_9, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 18, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_9, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 18, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -68894,15 +66831,15 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 18, __pyx_L3_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 18, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     /*try:*/ {
       {
@@ -68917,25 +66854,25 @@
           /* "src/mintalib/cython/stoch.pxi":19
  * 
  *     with np.errstate(divide='ignore'):
  *         fastk = 100 * (close - lo) /(hi - lo)             # <<<<<<<<<<<<<<
  * 
  *     slowk = calc_sma(fastk, fastn)
  */
-          __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_close, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(37, 19, __pyx_L7_error)
+          __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_close, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 19, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_9);
-          __pyx_t_1 = PyNumber_Subtract(__pyx_t_9, __pyx_v_lo); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 19, __pyx_L7_error)
+          __pyx_t_1 = PyNumber_Subtract(__pyx_t_9, __pyx_v_lo); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 19, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          __pyx_t_9 = __Pyx_PyInt_MultiplyCObj(__pyx_int_100, __pyx_t_1, 0x64, 0, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(37, 19, __pyx_L7_error)
+          __pyx_t_9 = __Pyx_PyInt_MultiplyCObj(__pyx_int_100, __pyx_t_1, 0x64, 0, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 19, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = PyNumber_Subtract(__pyx_v_hi, __pyx_v_lo); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 19, __pyx_L7_error)
+          __pyx_t_1 = PyNumber_Subtract(__pyx_v_hi, __pyx_v_lo); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 19, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_9, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 19, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_9, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 19, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_v_fastk = __pyx_t_3;
           __pyx_t_3 = 0;
 
           /* "src/mintalib/cython/stoch.pxi":18
@@ -68961,36 +66898,36 @@
         __PYX_XCLEAR_MEMVIEW(&__pyx_t_7, 1);
         __pyx_t_7.memview = NULL; __pyx_t_7.data = NULL;
         __PYX_XCLEAR_MEMVIEW(&__pyx_t_8, 1);
         __pyx_t_8.memview = NULL; __pyx_t_8.data = NULL;
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("mintalib.core.calc_stoch", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_9) < 0) __PYX_ERR(37, 18, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_9) < 0) __PYX_ERR(36, 18, __pyx_L9_except_error)
           __Pyx_XGOTREF(__pyx_t_3);
           __Pyx_XGOTREF(__pyx_t_1);
           __Pyx_XGOTREF(__pyx_t_9);
-          __pyx_t_4 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_1, __pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 18, __pyx_L9_except_error)
+          __pyx_t_4 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_1, __pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 18, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_4);
           __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_4, NULL);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_16)) __PYX_ERR(37, 18, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_16)) __PYX_ERR(36, 18, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_16);
           __pyx_t_17 = __Pyx_PyObject_IsTrue(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          if (__pyx_t_17 < 0) __PYX_ERR(37, 18, __pyx_L9_except_error)
+          if (__pyx_t_17 < 0) __PYX_ERR(36, 18, __pyx_L9_except_error)
           __pyx_t_18 = (!__pyx_t_17);
           if (unlikely(__pyx_t_18)) {
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_XGIVEREF(__pyx_t_9);
             __Pyx_ErrRestoreWithState(__pyx_t_3, __pyx_t_1, __pyx_t_9);
             __pyx_t_3 = 0; __pyx_t_1 = 0; __pyx_t_9 = 0; 
-            __PYX_ERR(37, 18, __pyx_L9_except_error)
+            __PYX_ERR(36, 18, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -69008,15 +66945,15 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_12) {
           __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_tuple__16, NULL);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          if (unlikely(!__pyx_t_15)) __PYX_ERR(37, 18, __pyx_L1_error)
+          if (unlikely(!__pyx_t_15)) __PYX_ERR(36, 18, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
@@ -69030,18 +66967,18 @@
   /* "src/mintalib/cython/stoch.pxi":21
  *         fastk = 100 * (close - lo) /(hi - lo)
  * 
  *     slowk = calc_sma(fastk, fastn)             # <<<<<<<<<<<<<<
  *     slowd = calc_sma(slowk, slown)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_calc_sma); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 21, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_calc_sma); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(!__pyx_v_fastk)) { __Pyx_RaiseUnboundLocalError("fastk"); __PYX_ERR(37, 21, __pyx_L1_error) }
-  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_fastn); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 21, __pyx_L1_error)
+  if (unlikely(!__pyx_v_fastk)) { __Pyx_RaiseUnboundLocalError("fastk"); __PYX_ERR(36, 21, __pyx_L1_error) }
+  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_fastn); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
@@ -69054,31 +66991,31 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_v_fastk, __pyx_t_3};
     __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_9)) __PYX_ERR(37, 21, __pyx_L1_error)
+    if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 21, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_v_slowk = __pyx_t_9;
   __pyx_t_9 = 0;
 
   /* "src/mintalib/cython/stoch.pxi":22
  * 
  *     slowk = calc_sma(fastk, fastn)
  *     slowd = calc_sma(slowk, slown)             # <<<<<<<<<<<<<<
  * 
  *     result = stoch_result(slowk, slowd)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_calc_sma); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 22, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_calc_sma); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_slown); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 22, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_slown); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
@@ -69091,29 +67028,29 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_v_slowk, __pyx_t_3};
     __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_9)) __PYX_ERR(37, 22, __pyx_L1_error)
+    if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_v_slowd = __pyx_t_9;
   __pyx_t_9 = 0;
 
   /* "src/mintalib/cython/stoch.pxi":24
  *     slowd = calc_sma(slowk, slown)
  * 
  *     result = stoch_result(slowk, slowd)             # <<<<<<<<<<<<<<
  * 
  *     if wrap:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_stoch_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 24, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_stoch_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
@@ -69125,39 +67062,39 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_slowk, __pyx_v_slowd};
     __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_9)) __PYX_ERR(37, 24, __pyx_L1_error)
+    if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 24, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_v_result = __pyx_t_9;
   __pyx_t_9 = 0;
 
   /* "src/mintalib/cython/stoch.pxi":26
  *     result = stoch_result(slowk, slowd)
  * 
  *     if wrap:             # <<<<<<<<<<<<<<
  *         result = wrap_result(result, prices)
  * 
  */
-  __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_v_wrap); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(37, 26, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_v_wrap); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(36, 26, __pyx_L1_error)
   if (__pyx_t_18) {
 
     /* "src/mintalib/cython/stoch.pxi":27
  * 
  *     if wrap:
  *         result = wrap_result(result, prices)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 27, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 27, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_3)) {
@@ -69169,15 +67106,15 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_result, __pyx_v_prices};
       __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_9)) __PYX_ERR(37, 27, __pyx_L1_error)
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(36, 27, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_9);
     __pyx_t_9 = 0;
 
     /* "src/mintalib/cython/stoch.pxi":26
@@ -69241,42 +67178,42 @@
  * 
  * 
  * @wrap_function(calc_stoch)             # <<<<<<<<<<<<<<
  * def STOCH(prices, period: int = 14, fastn: int = 3, slown: int = 3):
  *     result = calc_stoch(prices, period=period, fastn=fastn, slown=slown)
  */
 
-static PyObject *__pyx_pf_8mintalib_4core_301__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8mintalib_4core_295__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 32, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_self)->__pyx_arg_period);
-  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_self)->__pyx_arg_period);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_self)->__pyx_arg_period)) __PYX_ERR(37, 32, __pyx_L1_error);
-  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_self)->__pyx_arg_fastn);
-  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_self)->__pyx_arg_fastn);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_self)->__pyx_arg_fastn)) __PYX_ERR(37, 32, __pyx_L1_error);
-  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_self)->__pyx_arg_slown);
-  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_self)->__pyx_arg_slown);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_self)->__pyx_arg_slown)) __PYX_ERR(37, 32, __pyx_L1_error);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 32, __pyx_L1_error)
+  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_period);
+  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_period);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_period)) __PYX_ERR(36, 32, __pyx_L1_error);
+  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_fastn);
+  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_fastn);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_fastn)) __PYX_ERR(36, 32, __pyx_L1_error);
+  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_slown);
+  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_slown);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self)->__pyx_arg_slown)) __PYX_ERR(36, 32, __pyx_L1_error);
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(37, 32, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(36, 32, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None)) __PYX_ERR(37, 32, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None)) __PYX_ERR(36, 32, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -69287,23 +67224,23 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_213STOCH(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8mintalib_4core_209STOCH(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8mintalib_4core_213STOCH = {"STOCH", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_213STOCH, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8mintalib_4core_213STOCH(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8mintalib_4core_209STOCH = {"STOCH", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_209STOCH, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8mintalib_4core_209STOCH(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_prices = 0;
@@ -69327,15 +67264,15 @@
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_prices,&__pyx_n_s_period,&__pyx_n_s_fastn,&__pyx_n_s_slown,0};
-    __pyx_defaults36 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_self);
+    __pyx_defaults35 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_self);
     values[1] = __Pyx_Arg_NewRef_FASTCALL(__pyx_dynamic_args->__pyx_arg_period);
     values[2] = __Pyx_Arg_NewRef_FASTCALL(__pyx_dynamic_args->__pyx_arg_fastn);
     values[3] = __Pyx_Arg_NewRef_FASTCALL(__pyx_dynamic_args->__pyx_arg_slown);
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
@@ -69352,41 +67289,41 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_prices)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 32, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 32, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_period);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 32, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 32, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fastn);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 32, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 32, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_slown);
           if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 32, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(36, 32, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "STOCH") < 0)) __PYX_ERR(37, 32, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "STOCH") < 0)) __PYX_ERR(36, 32, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -69400,32 +67337,32 @@
     __pyx_v_prices = values[0];
     __pyx_v_period = ((PyObject*)values[1]);
     __pyx_v_fastn = ((PyObject*)values[2]);
     __pyx_v_slown = ((PyObject*)values[3]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("STOCH", 0, 1, 4, __pyx_nargs); __PYX_ERR(37, 32, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("STOCH", 0, 1, 4, __pyx_nargs); __PYX_ERR(36, 32, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("mintalib.core.STOCH", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_period), (&PyInt_Type), 0, "period", 1))) __PYX_ERR(37, 33, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fastn), (&PyInt_Type), 0, "fastn", 1))) __PYX_ERR(37, 33, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_slown), (&PyInt_Type), 0, "slown", 1))) __PYX_ERR(37, 33, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8mintalib_4core_212STOCH(__pyx_self, __pyx_v_prices, __pyx_v_period, __pyx_v_fastn, __pyx_v_slown);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_period), (&PyInt_Type), 0, "period", 1))) __PYX_ERR(36, 33, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fastn), (&PyInt_Type), 0, "fastn", 1))) __PYX_ERR(36, 33, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_slown), (&PyInt_Type), 0, "slown", 1))) __PYX_ERR(36, 33, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8mintalib_4core_208STOCH(__pyx_self, __pyx_v_prices, __pyx_v_period, __pyx_v_fastn, __pyx_v_slown);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -69434,15 +67371,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8mintalib_4core_212STOCH(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period, PyObject *__pyx_v_fastn, PyObject *__pyx_v_slown) {
+static PyObject *__pyx_pf_8mintalib_4core_208STOCH(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_period, PyObject *__pyx_v_fastn, PyObject *__pyx_v_slown) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -69455,42 +67392,42 @@
   /* "src/mintalib/cython/stoch.pxi":34
  * @wrap_function(calc_stoch)
  * def STOCH(prices, period: int = 14, fastn: int = 3, slown: int = 3):
  *     result = calc_stoch(prices, period=period, fastn=fastn, slown=slown)             # <<<<<<<<<<<<<<
  *     return wrap_result(result, prices)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_calc_stoch); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 34, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_calc_stoch); if (unlikely(!__pyx_t_1)) __PYX_ERR(36, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 34, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(36, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_prices);
   __Pyx_GIVEREF(__pyx_v_prices);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_prices)) __PYX_ERR(37, 34, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 34, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_prices)) __PYX_ERR(36, 34, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_period, __pyx_v_period) < 0) __PYX_ERR(37, 34, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_fastn, __pyx_v_fastn) < 0) __PYX_ERR(37, 34, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_slown, __pyx_v_slown) < 0) __PYX_ERR(37, 34, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_period, __pyx_v_period) < 0) __PYX_ERR(36, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_fastn, __pyx_v_fastn) < 0) __PYX_ERR(36, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_slown, __pyx_v_slown) < 0) __PYX_ERR(36, 34, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "src/mintalib/cython/stoch.pxi":35
  * def STOCH(prices, period: int = 14, fastn: int = 3, slown: int = 3):
  *     result = calc_stoch(prices, period=period, fastn=fastn, slown=slown)
  *     return wrap_result(result, prices)             # <<<<<<<<<<<<<<
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 35, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(36, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -69502,15 +67439,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_v_result, __pyx_v_prices};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 35, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(36, 35, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
@@ -69542,24 +67479,24 @@
  * 
  * def streak_up(series, *, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Consecutive streak of ups """
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_215streak_up(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8mintalib_4core_211streak_up(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8mintalib_4core_214streak_up, " Consecutive streak of ups ");
-static PyMethodDef __pyx_mdef_8mintalib_4core_215streak_up = {"streak_up", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_215streak_up, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8mintalib_4core_214streak_up};
-static PyObject *__pyx_pw_8mintalib_4core_215streak_up(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_8mintalib_4core_210streak_up, " Consecutive streak of ups ");
+static PyMethodDef __pyx_mdef_8mintalib_4core_211streak_up = {"streak_up", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_211streak_up, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8mintalib_4core_210streak_up};
+static PyObject *__pyx_pw_8mintalib_4core_211streak_up(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_series = 0;
@@ -69597,65 +67534,65 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_series)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 3, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 3, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (kw_args == 1) {
         const Py_ssize_t index = 1;
         PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
         if (value) { values[index] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 3, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 3, __pyx_L3_error)
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "streak_up") < 0)) __PYX_ERR(38, 3, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "streak_up") < 0)) __PYX_ERR(37, 3, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_series = values[0];
     __pyx_v_wrap = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("streak_up", 1, 1, 1, __pyx_nargs); __PYX_ERR(38, 3, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("streak_up", 1, 1, 1, __pyx_nargs); __PYX_ERR(37, 3, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("mintalib.core.streak_up", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8mintalib_4core_214streak_up(__pyx_self, __pyx_v_series, __pyx_v_wrap);
+  __pyx_r = __pyx_pf_8mintalib_4core_210streak_up(__pyx_self, __pyx_v_series, __pyx_v_wrap);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8mintalib_4core_214streak_up(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_wrap) {
+static PyObject *__pyx_pf_8mintalib_4core_210streak_up(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_wrap) {
   __Pyx_memviewslice __pyx_v_xs = { 0, 0, { 0 }, { 0 }, { 0 } };
   long __pyx_v_size;
   PyObject *__pyx_v_result = 0;
   __Pyx_memviewslice __pyx_v_output = { 0, 0, { 0 }, { 0 }, { 0 } };
   double __pyx_v_value;
   double __pyx_v_prev;
   double __pyx_v_diff;
@@ -69686,17 +67623,17 @@
   /* "src/mintalib/cython/streak.pxi":6
  *     """ Consecutive streak of ups """
  * 
  *     cdef const double[:] xs = np.asarray(series, float)             # <<<<<<<<<<<<<<
  *     cdef long size = xs.size
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(38, 6, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 6, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -69709,57 +67646,57 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_v_series, ((PyObject *)(&PyFloat_Type))};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 6, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 6, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_ds_double__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(38, 6, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_ds_double__const__(__pyx_t_1, 0); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(37, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_xs = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
   /* "src/mintalib/cython/streak.pxi":7
  * 
  *     cdef const double[:] xs = np.asarray(series, float)
  *     cdef long size = xs.size             # <<<<<<<<<<<<<<
  * 
  *     cdef object result = np.full(size, np.nan)
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_xs, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 7, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_xs, 1, (PyObject *(*)(char *)) __pyx_memview_get_double__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 7, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_6 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_6 == (long)-1) && PyErr_Occurred())) __PYX_ERR(38, 7, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_6 == (long)-1) && PyErr_Occurred())) __PYX_ERR(37, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_size = __pyx_t_6;
 
   /* "src/mintalib/cython/streak.pxi":9
  *     cdef long size = xs.size
  * 
  *     cdef object result = np.full(size, np.nan)             # <<<<<<<<<<<<<<
  *     cdef double[:] output = result
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 9, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_full); if (unlikely(!__pyx_t_2)) __PYX_ERR(38, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_full); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 9, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(38, 9, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_nan); if (unlikely(!__pyx_t_8)) __PYX_ERR(38, 9, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_nan); if (unlikely(!__pyx_t_8)) __PYX_ERR(37, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
@@ -69774,29 +67711,29 @@
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_7, __pyx_t_1, __pyx_t_8};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 9, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_result = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "src/mintalib/cython/streak.pxi":10
  * 
  *     cdef object result = np.full(size, np.nan)
  *     cdef double[:] output = result             # <<<<<<<<<<<<<<
  * 
  *     cdef double value = NAN, prev = NAN, diff=NAN
  */
-  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_result, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(38, 10, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_result, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(37, 10, __pyx_L1_error)
   __pyx_v_output = __pyx_t_9;
   __pyx_t_9.memview = NULL;
   __pyx_t_9.data = NULL;
 
   /* "src/mintalib/cython/streak.pxi":12
  *     cdef double[:] output = result
  * 
@@ -69849,15 +67786,15 @@
     __pyx_t_4 = -1;
     if (__pyx_t_12 < 0) {
       __pyx_t_12 += __pyx_v_xs.shape[0];
       if (unlikely(__pyx_t_12 < 0)) __pyx_t_4 = 0;
     } else if (unlikely(__pyx_t_12 >= __pyx_v_xs.shape[0])) __pyx_t_4 = 0;
     if (unlikely(__pyx_t_4 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_4);
-      __PYX_ERR(38, 18, __pyx_L1_error)
+      __PYX_ERR(37, 18, __pyx_L1_error)
     }
     __pyx_v_value = (*((double const  *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_12 * __pyx_v_xs.strides[0]) )));
 
     /* "src/mintalib/cython/streak.pxi":20
  *         value = xs[i]
  * 
  *         if not isnan(value):             # <<<<<<<<<<<<<<
@@ -69957,37 +67894,37 @@
     __pyx_t_4 = -1;
     if (__pyx_t_12 < 0) {
       __pyx_t_12 += __pyx_v_output.shape[0];
       if (unlikely(__pyx_t_12 < 0)) __pyx_t_4 = 0;
     } else if (unlikely(__pyx_t_12 >= __pyx_v_output.shape[0])) __pyx_t_4 = 0;
     if (unlikely(__pyx_t_4 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_4);
-      __PYX_ERR(38, 28, __pyx_L1_error)
+      __PYX_ERR(37, 28, __pyx_L1_error)
     }
     *((double *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_12 * __pyx_v_output.strides[0]) )) = __pyx_v_streak;
   }
 
   /* "src/mintalib/cython/streak.pxi":30
  *         output[i] = streak
  * 
  *     if wrap:             # <<<<<<<<<<<<<<
  *         result = wrap_result(result, series)
  * 
  */
-  __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_v_wrap); if (unlikely((__pyx_t_13 < 0))) __PYX_ERR(38, 30, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_v_wrap); if (unlikely((__pyx_t_13 < 0))) __PYX_ERR(37, 30, __pyx_L1_error)
   if (__pyx_t_13) {
 
     /* "src/mintalib/cython/streak.pxi":31
  * 
  *     if wrap:
  *         result = wrap_result(result, series)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_2)) __PYX_ERR(38, 31, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 31, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_8 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
@@ -69999,15 +67936,15 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_8, __pyx_v_result, __pyx_v_series};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 31, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 31, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "src/mintalib/cython/streak.pxi":30
@@ -70064,24 +68001,24 @@
  * 
  * def streak_down(series, *, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Consecutive streak of downs """
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_217streak_down(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8mintalib_4core_213streak_down(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8mintalib_4core_216streak_down, " Consecutive streak of downs ");
-static PyMethodDef __pyx_mdef_8mintalib_4core_217streak_down = {"streak_down", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_217streak_down, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8mintalib_4core_216streak_down};
-static PyObject *__pyx_pw_8mintalib_4core_217streak_down(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_8mintalib_4core_212streak_down, " Consecutive streak of downs ");
+static PyMethodDef __pyx_mdef_8mintalib_4core_213streak_down = {"streak_down", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_213streak_down, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8mintalib_4core_212streak_down};
+static PyObject *__pyx_pw_8mintalib_4core_213streak_down(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_series = 0;
@@ -70119,65 +68056,65 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_series)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 38, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 38, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (kw_args == 1) {
         const Py_ssize_t index = 1;
         PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
         if (value) { values[index] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 38, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 38, __pyx_L3_error)
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "streak_down") < 0)) __PYX_ERR(38, 38, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "streak_down") < 0)) __PYX_ERR(37, 38, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_series = values[0];
     __pyx_v_wrap = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("streak_down", 1, 1, 1, __pyx_nargs); __PYX_ERR(38, 38, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("streak_down", 1, 1, 1, __pyx_nargs); __PYX_ERR(37, 38, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("mintalib.core.streak_down", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8mintalib_4core_216streak_down(__pyx_self, __pyx_v_series, __pyx_v_wrap);
+  __pyx_r = __pyx_pf_8mintalib_4core_212streak_down(__pyx_self, __pyx_v_series, __pyx_v_wrap);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8mintalib_4core_216streak_down(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_wrap) {
+static PyObject *__pyx_pf_8mintalib_4core_212streak_down(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_wrap) {
   __Pyx_memviewslice __pyx_v_xs = { 0, 0, { 0 }, { 0 }, { 0 } };
   long __pyx_v_size;
   PyObject *__pyx_v_result = 0;
   __Pyx_memviewslice __pyx_v_output = { 0, 0, { 0 }, { 0 }, { 0 } };
   double __pyx_v_value;
   double __pyx_v_prev;
   double __pyx_v_diff;
@@ -70207,17 +68144,17 @@
   /* "src/mintalib/cython/streak.pxi":41
  *     """ Consecutive streak of downs """
  * 
  *     cdef double[:] xs = np.asarray(series, float)             # <<<<<<<<<<<<<<
  *     cdef long size = xs.size
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(38, 41, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 41, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -70230,57 +68167,57 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_v_series, ((PyObject *)(&PyFloat_Type))};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 41, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 41, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(38, 41, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(37, 41, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_xs = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
   /* "src/mintalib/cython/streak.pxi":42
  * 
  *     cdef double[:] xs = np.asarray(series, float)
  *     cdef long size = xs.size             # <<<<<<<<<<<<<<
  * 
  *     cdef object result = np.full(size, np.nan)
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_xs, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 42, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_xs, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 42, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_6 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_6 == (long)-1) && PyErr_Occurred())) __PYX_ERR(38, 42, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_6 == (long)-1) && PyErr_Occurred())) __PYX_ERR(37, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_size = __pyx_t_6;
 
   /* "src/mintalib/cython/streak.pxi":44
  *     cdef long size = xs.size
  * 
  *     cdef object result = np.full(size, np.nan)             # <<<<<<<<<<<<<<
  *     cdef double[:] output = result
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 44, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_full); if (unlikely(!__pyx_t_2)) __PYX_ERR(38, 44, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_full); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 44, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(38, 44, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_nan); if (unlikely(!__pyx_t_8)) __PYX_ERR(38, 44, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_nan); if (unlikely(!__pyx_t_8)) __PYX_ERR(37, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
@@ -70295,29 +68232,29 @@
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_7, __pyx_t_1, __pyx_t_8};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 44, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_result = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "src/mintalib/cython/streak.pxi":45
  * 
  *     cdef object result = np.full(size, np.nan)
  *     cdef double[:] output = result             # <<<<<<<<<<<<<<
  * 
  *     cdef double value = NAN, prev = NAN, diff=NAN
  */
-  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_result, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(38, 45, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_result, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(37, 45, __pyx_L1_error)
   __pyx_v_output = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
   /* "src/mintalib/cython/streak.pxi":47
  *     cdef double[:] output = result
  * 
@@ -70370,15 +68307,15 @@
     __pyx_t_4 = -1;
     if (__pyx_t_11 < 0) {
       __pyx_t_11 += __pyx_v_xs.shape[0];
       if (unlikely(__pyx_t_11 < 0)) __pyx_t_4 = 0;
     } else if (unlikely(__pyx_t_11 >= __pyx_v_xs.shape[0])) __pyx_t_4 = 0;
     if (unlikely(__pyx_t_4 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_4);
-      __PYX_ERR(38, 53, __pyx_L1_error)
+      __PYX_ERR(37, 53, __pyx_L1_error)
     }
     __pyx_v_value = (*((double *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_11 * __pyx_v_xs.strides[0]) )));
 
     /* "src/mintalib/cython/streak.pxi":55
  *         value = xs[i]
  * 
  *         if not isnan(value):             # <<<<<<<<<<<<<<
@@ -70478,37 +68415,37 @@
     __pyx_t_4 = -1;
     if (__pyx_t_11 < 0) {
       __pyx_t_11 += __pyx_v_output.shape[0];
       if (unlikely(__pyx_t_11 < 0)) __pyx_t_4 = 0;
     } else if (unlikely(__pyx_t_11 >= __pyx_v_output.shape[0])) __pyx_t_4 = 0;
     if (unlikely(__pyx_t_4 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_4);
-      __PYX_ERR(38, 63, __pyx_L1_error)
+      __PYX_ERR(37, 63, __pyx_L1_error)
     }
     *((double *) ( /* dim=0 */ (__pyx_v_output.data + __pyx_t_11 * __pyx_v_output.strides[0]) )) = __pyx_v_streak;
   }
 
   /* "src/mintalib/cython/streak.pxi":65
  *         output[i] = streak
  * 
  *     if wrap:             # <<<<<<<<<<<<<<
  *         result = wrap_result(result, series)
  * 
  */
-  __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_v_wrap); if (unlikely((__pyx_t_12 < 0))) __PYX_ERR(38, 65, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_v_wrap); if (unlikely((__pyx_t_12 < 0))) __PYX_ERR(37, 65, __pyx_L1_error)
   if (__pyx_t_12) {
 
     /* "src/mintalib/cython/streak.pxi":66
  * 
  *     if wrap:
  *         result = wrap_result(result, series)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_2)) __PYX_ERR(38, 66, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_8 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
@@ -70520,15 +68457,15 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_8, __pyx_v_result, __pyx_v_series};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 66, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 66, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "src/mintalib/cython/streak.pxi":65
@@ -70584,23 +68521,23 @@
  * 
  * @wrap_function(streak_up)             # <<<<<<<<<<<<<<
  * def STREAK_UP(series, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_219STREAK_UP(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8mintalib_4core_215STREAK_UP(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8mintalib_4core_219STREAK_UP = {"STREAK_UP", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_219STREAK_UP, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8mintalib_4core_219STREAK_UP(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8mintalib_4core_215STREAK_UP = {"STREAK_UP", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_215STREAK_UP, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8mintalib_4core_215STREAK_UP(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_series = 0;
@@ -70646,53 +68583,53 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_series)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 72, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 72, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (kw_args == 1) {
         const Py_ssize_t index = 1;
         PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
         if (value) { values[index] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 72, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 72, __pyx_L3_error)
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "STREAK_UP") < 0)) __PYX_ERR(38, 72, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "STREAK_UP") < 0)) __PYX_ERR(37, 72, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_series = values[0];
     __pyx_v_item = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("STREAK_UP", 1, 1, 1, __pyx_nargs); __PYX_ERR(38, 72, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("STREAK_UP", 1, 1, 1, __pyx_nargs); __PYX_ERR(37, 72, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("mintalib.core.STREAK_UP", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_item), (&PyUnicode_Type), 1, "item", 1))) __PYX_ERR(38, 73, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8mintalib_4core_218STREAK_UP(__pyx_self, __pyx_v_series, __pyx_v_item);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_item), (&PyUnicode_Type), 1, "item", 1))) __PYX_ERR(37, 73, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8mintalib_4core_214STREAK_UP(__pyx_self, __pyx_v_series, __pyx_v_item);
 
   /* "src/mintalib/cython/streak.pxi":72
  * 
  * 
  * @wrap_function(streak_up)             # <<<<<<<<<<<<<<
  * def STREAK_UP(series, *, item: str = None):
  *     series = get_series(series, item=item)
@@ -70709,15 +68646,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8mintalib_4core_218STREAK_UP(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_item) {
+static PyObject *__pyx_pf_8mintalib_4core_214STREAK_UP(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_item) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -70731,40 +68668,40 @@
   /* "src/mintalib/cython/streak.pxi":74
  * @wrap_function(streak_up)
  * def STREAK_UP(series, *, item: str = None):
  *     series = get_series(series, item=item)             # <<<<<<<<<<<<<<
  *     result = streak_up(series)
  *     return wrap_result(result, series)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_series); if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 74, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_series); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(38, 74, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_series);
   __Pyx_GIVEREF(__pyx_v_series);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_series)) __PYX_ERR(38, 74, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 74, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_series)) __PYX_ERR(37, 74, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_item, __pyx_v_item) < 0) __PYX_ERR(38, 74, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(38, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_item, __pyx_v_item) < 0) __PYX_ERR(37, 74, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_series, __pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "src/mintalib/cython/streak.pxi":75
  * def STREAK_UP(series, *, item: str = None):
  *     series = get_series(series, item=item)
  *     result = streak_up(series)             # <<<<<<<<<<<<<<
  *     return wrap_result(result, series)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_streak_up); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 75, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_streak_up); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -70776,30 +68713,30 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_series};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(38, 75, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_result = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "src/mintalib/cython/streak.pxi":76
  *     series = get_series(series, item=item)
  *     result = streak_up(series)
  *     return wrap_result(result, series)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 76, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -70811,15 +68748,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_v_result, __pyx_v_series};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(38, 76, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
@@ -70852,23 +68789,23 @@
  * 
  * @wrap_function(streak_down)             # <<<<<<<<<<<<<<
  * def STREAK_DOWN(series, *, item: str = None):
  *     series = get_series(series, item=item)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_221STREAK_DOWN(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8mintalib_4core_217STREAK_DOWN(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8mintalib_4core_221STREAK_DOWN = {"STREAK_DOWN", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_221STREAK_DOWN, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8mintalib_4core_221STREAK_DOWN(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8mintalib_4core_217STREAK_DOWN = {"STREAK_DOWN", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_217STREAK_DOWN, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8mintalib_4core_217STREAK_DOWN(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_series = 0;
@@ -70914,53 +68851,53 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_series)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 79, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 79, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (kw_args == 1) {
         const Py_ssize_t index = 1;
         PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
         if (value) { values[index] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 79, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(37, 79, __pyx_L3_error)
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "STREAK_DOWN") < 0)) __PYX_ERR(38, 79, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "STREAK_DOWN") < 0)) __PYX_ERR(37, 79, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_series = values[0];
     __pyx_v_item = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("STREAK_DOWN", 1, 1, 1, __pyx_nargs); __PYX_ERR(38, 79, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("STREAK_DOWN", 1, 1, 1, __pyx_nargs); __PYX_ERR(37, 79, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("mintalib.core.STREAK_DOWN", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_item), (&PyUnicode_Type), 1, "item", 1))) __PYX_ERR(38, 80, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8mintalib_4core_220STREAK_DOWN(__pyx_self, __pyx_v_series, __pyx_v_item);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_item), (&PyUnicode_Type), 1, "item", 1))) __PYX_ERR(37, 80, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8mintalib_4core_216STREAK_DOWN(__pyx_self, __pyx_v_series, __pyx_v_item);
 
   /* "src/mintalib/cython/streak.pxi":79
  * 
  * 
  * @wrap_function(streak_down)             # <<<<<<<<<<<<<<
  * def STREAK_DOWN(series, *, item: str = None):
  *     series = get_series(series, item=item)
@@ -70977,15 +68914,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8mintalib_4core_220STREAK_DOWN(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_item) {
+static PyObject *__pyx_pf_8mintalib_4core_216STREAK_DOWN(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_series, PyObject *__pyx_v_item) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -70999,40 +68936,40 @@
   /* "src/mintalib/cython/streak.pxi":81
  * @wrap_function(streak_down)
  * def STREAK_DOWN(series, *, item: str = None):
  *     series = get_series(series, item=item)             # <<<<<<<<<<<<<<
  *     result = streak_down(series)
  *     return wrap_result(result, series)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_series); if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 81, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_series); if (unlikely(!__pyx_t_1)) __PYX_ERR(37, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(38, 81, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(37, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_series);
   __Pyx_GIVEREF(__pyx_v_series);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_series)) __PYX_ERR(38, 81, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 81, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_series)) __PYX_ERR(37, 81, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_item, __pyx_v_item) < 0) __PYX_ERR(38, 81, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(38, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_item, __pyx_v_item) < 0) __PYX_ERR(37, 81, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_series, __pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "src/mintalib/cython/streak.pxi":82
  * def STREAK_DOWN(series, *, item: str = None):
  *     series = get_series(series, item=item)
  *     result = streak_down(series)             # <<<<<<<<<<<<<<
  *     return wrap_result(result, series)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_streak_down); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 82, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_streak_down); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -71044,30 +68981,30 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_series};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(38, 82, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_result = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "src/mintalib/cython/streak.pxi":83
  *     series = get_series(series, item=item)
  *     result = streak_down(series)
  *     return wrap_result(result, series)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 83, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(37, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -71079,15 +69016,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_v_result, __pyx_v_series};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(38, 83, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(37, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
@@ -71120,24 +69057,24 @@
  * 
  * def calc_eval(prices, expr: str):             # <<<<<<<<<<<<<<
  *     """
  *     Expression Eval (pandas only)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_223calc_eval(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8mintalib_4core_219calc_eval(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8mintalib_4core_222calc_eval, "\n    Expression Eval (pandas only)\n\n    Args:\n        expr (str) : expression to evaluate on the prices dataframe\n    ");
-static PyMethodDef __pyx_mdef_8mintalib_4core_223calc_eval = {"calc_eval", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_223calc_eval, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8mintalib_4core_222calc_eval};
-static PyObject *__pyx_pw_8mintalib_4core_223calc_eval(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_8mintalib_4core_218calc_eval, "\n    Expression Eval (pandas only)\n\n    Args:\n        expr (str) : expression to evaluate on the prices dataframe\n    ");
+static PyMethodDef __pyx_mdef_8mintalib_4core_219calc_eval = {"calc_eval", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_219calc_eval, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8mintalib_4core_218calc_eval};
+static PyObject *__pyx_pw_8mintalib_4core_219calc_eval(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_prices = 0;
@@ -71176,58 +69113,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_prices)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(39, 3, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 3, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_expr)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(39, 3, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 3, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("calc_eval", 1, 2, 2, 1); __PYX_ERR(39, 3, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calc_eval", 1, 2, 2, 1); __PYX_ERR(38, 3, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_eval") < 0)) __PYX_ERR(39, 3, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_eval") < 0)) __PYX_ERR(38, 3, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_prices = values[0];
     __pyx_v_expr = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calc_eval", 1, 2, 2, __pyx_nargs); __PYX_ERR(39, 3, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calc_eval", 1, 2, 2, __pyx_nargs); __PYX_ERR(38, 3, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("mintalib.core.calc_eval", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_expr), (&PyUnicode_Type), 0, "expr", 1))) __PYX_ERR(39, 3, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8mintalib_4core_222calc_eval(__pyx_self, __pyx_v_prices, __pyx_v_expr);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_expr), (&PyUnicode_Type), 0, "expr", 1))) __PYX_ERR(38, 3, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8mintalib_4core_218calc_eval(__pyx_self, __pyx_v_prices, __pyx_v_expr);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -71236,15 +69173,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8mintalib_4core_222calc_eval(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_expr) {
+static PyObject *__pyx_pf_8mintalib_4core_218calc_eval(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_expr) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -71257,15 +69194,15 @@
  *     """
  * 
  *     return prices.eval(expr).astype(float)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_prices, __pyx_n_s_eval); if (unlikely(!__pyx_t_3)) __PYX_ERR(39, 11, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_prices, __pyx_n_s_eval); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -71277,19 +69214,19 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_expr};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(39, 11, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(38, 11, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(39, 11, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -71302,15 +69239,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, ((PyObject *)(&PyFloat_Type))};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(39, 11, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 11, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
@@ -71341,23 +69278,23 @@
  * 
  * @wrap_function(calc_eval)             # <<<<<<<<<<<<<<
  * def EVAL(prices, expr: str):
  *     result = calc_eval(prices, expr=expr)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8mintalib_4core_225EVAL(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8mintalib_4core_221EVAL(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8mintalib_4core_225EVAL = {"EVAL", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_225EVAL, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8mintalib_4core_225EVAL(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8mintalib_4core_221EVAL = {"EVAL", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8mintalib_4core_221EVAL, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8mintalib_4core_221EVAL(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_prices = 0;
@@ -71396,58 +69333,58 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_prices)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(39, 14, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 14, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_expr)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(39, 14, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(38, 14, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("EVAL", 1, 2, 2, 1); __PYX_ERR(39, 14, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("EVAL", 1, 2, 2, 1); __PYX_ERR(38, 14, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "EVAL") < 0)) __PYX_ERR(39, 14, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "EVAL") < 0)) __PYX_ERR(38, 14, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_prices = values[0];
     __pyx_v_expr = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("EVAL", 1, 2, 2, __pyx_nargs); __PYX_ERR(39, 14, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("EVAL", 1, 2, 2, __pyx_nargs); __PYX_ERR(38, 14, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("mintalib.core.EVAL", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_expr), (&PyUnicode_Type), 0, "expr", 1))) __PYX_ERR(39, 15, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8mintalib_4core_224EVAL(__pyx_self, __pyx_v_prices, __pyx_v_expr);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_expr), (&PyUnicode_Type), 0, "expr", 1))) __PYX_ERR(38, 15, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8mintalib_4core_220EVAL(__pyx_self, __pyx_v_prices, __pyx_v_expr);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -71456,15 +69393,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8mintalib_4core_224EVAL(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_expr) {
+static PyObject *__pyx_pf_8mintalib_4core_220EVAL(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_prices, PyObject *__pyx_v_expr) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -71477,40 +69414,40 @@
   /* "src/mintalib/cython/eval.pxi":16
  * @wrap_function(calc_eval)
  * def EVAL(prices, expr: str):
  *     result = calc_eval(prices, expr=expr)             # <<<<<<<<<<<<<<
  *     return wrap_result(result, prices)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_calc_eval); if (unlikely(!__pyx_t_1)) __PYX_ERR(39, 16, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_calc_eval); if (unlikely(!__pyx_t_1)) __PYX_ERR(38, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(39, 16, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(38, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_prices);
   __Pyx_GIVEREF(__pyx_v_prices);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_prices)) __PYX_ERR(39, 16, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(39, 16, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_prices)) __PYX_ERR(38, 16, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_expr, __pyx_v_expr) < 0) __PYX_ERR(39, 16, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(39, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_expr, __pyx_v_expr) < 0) __PYX_ERR(38, 16, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(38, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "src/mintalib/cython/eval.pxi":17
  * def EVAL(prices, expr: str):
  *     result = calc_eval(prices, expr=expr)
  *     return wrap_result(result, prices)             # <<<<<<<<<<<<<<
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(39, 17, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_wrap_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(38, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -71522,15 +69459,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_v_result, __pyx_v_prices};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(39, 17, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(38, 17, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
@@ -71553,24 +69490,26 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_8mintalib_4core___pyx_scope_struct__wrap_function *__pyx_freelist_8mintalib_4core___pyx_scope_struct__wrap_function[8];
 static int __pyx_freecount_8mintalib_4core___pyx_scope_struct__wrap_function = 0;
+#endif
 
 static PyObject *__pyx_tp_new_8mintalib_4core___pyx_scope_struct__wrap_function(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_8mintalib_4core___pyx_scope_struct__wrap_function > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8mintalib_4core___pyx_scope_struct__wrap_function)))) {
     o = (PyObject*)__pyx_freelist_8mintalib_4core___pyx_scope_struct__wrap_function[--__pyx_freecount_8mintalib_4core___pyx_scope_struct__wrap_function];
     memset(o, 0, sizeof(struct __pyx_obj_8mintalib_4core___pyx_scope_struct__wrap_function));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -71589,15 +69528,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_8mintalib_4core___pyx_scope_struct__wrap_function) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_doc);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_8mintalib_4core___pyx_scope_struct__wrap_function < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8mintalib_4core___pyx_scope_struct__wrap_function)))) {
     __pyx_freelist_8mintalib_4core___pyx_scope_struct__wrap_function[__pyx_freecount_8mintalib_4core___pyx_scope_struct__wrap_function++] = ((struct __pyx_obj_8mintalib_4core___pyx_scope_struct__wrap_function *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -71722,24 +69661,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_8mintalib_4core___pyx_scope_struct_1_wrap_indicator *__pyx_freelist_8mintalib_4core___pyx_scope_struct_1_wrap_indicator[8];
 static int __pyx_freecount_8mintalib_4core___pyx_scope_struct_1_wrap_indicator = 0;
+#endif
 
 static PyObject *__pyx_tp_new_8mintalib_4core___pyx_scope_struct_1_wrap_indicator(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_8mintalib_4core___pyx_scope_struct_1_wrap_indicator > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8mintalib_4core___pyx_scope_struct_1_wrap_indicator)))) {
     o = (PyObject*)__pyx_freelist_8mintalib_4core___pyx_scope_struct_1_wrap_indicator[--__pyx_freecount_8mintalib_4core___pyx_scope_struct_1_wrap_indicator];
     memset(o, 0, sizeof(struct __pyx_obj_8mintalib_4core___pyx_scope_struct_1_wrap_indicator));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -71758,15 +69699,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_8mintalib_4core___pyx_scope_struct_1_wrap_indicator) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_doc);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_8mintalib_4core___pyx_scope_struct_1_wrap_indicator < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8mintalib_4core___pyx_scope_struct_1_wrap_indicator)))) {
     __pyx_freelist_8mintalib_4core___pyx_scope_struct_1_wrap_indicator[__pyx_freecount_8mintalib_4core___pyx_scope_struct_1_wrap_indicator++] = ((struct __pyx_obj_8mintalib_4core___pyx_scope_struct_1_wrap_indicator *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -71891,24 +69832,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_8mintalib_4core___pyx_scope_struct_2_genexpr *__pyx_freelist_8mintalib_4core___pyx_scope_struct_2_genexpr[8];
 static int __pyx_freecount_8mintalib_4core___pyx_scope_struct_2_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_8mintalib_4core___pyx_scope_struct_2_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_8mintalib_4core___pyx_scope_struct_2_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8mintalib_4core___pyx_scope_struct_2_genexpr)))) {
     o = (PyObject*)__pyx_freelist_8mintalib_4core___pyx_scope_struct_2_genexpr[--__pyx_freecount_8mintalib_4core___pyx_scope_struct_2_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_8mintalib_4core___pyx_scope_struct_2_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -71930,15 +69873,15 @@
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_k);
   Py_CLEAR(p->__pyx_v_v);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_8mintalib_4core___pyx_scope_struct_2_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8mintalib_4core___pyx_scope_struct_2_genexpr)))) {
     __pyx_freelist_8mintalib_4core___pyx_scope_struct_2_genexpr[__pyx_freecount_8mintalib_4core___pyx_scope_struct_2_genexpr++] = ((struct __pyx_obj_8mintalib_4core___pyx_scope_struct_2_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -73038,24 +70981,20 @@
     {&__pyx_n_s_BBANDS, __pyx_k_BBANDS, sizeof(__pyx_k_BBANDS), 0, 0, 1, 1},
     {&__pyx_n_s_BOP, __pyx_k_BOP, sizeof(__pyx_k_BOP), 0, 0, 1, 1},
     {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
     {&__pyx_n_s_CCI, __pyx_k_CCI, sizeof(__pyx_k_CCI), 0, 0, 1, 1},
     {&__pyx_n_s_CMF, __pyx_k_CMF, sizeof(__pyx_k_CMF), 0, 0, 1, 1},
     {&__pyx_n_s_CROSSOVER, __pyx_k_CROSSOVER, sizeof(__pyx_k_CROSSOVER), 0, 0, 1, 1},
     {&__pyx_n_s_CROSSUNDER, __pyx_k_CROSSUNDER, sizeof(__pyx_k_CROSSUNDER), 0, 0, 1, 1},
-    {&__pyx_n_s_CURVE, __pyx_k_CURVE, sizeof(__pyx_k_CURVE), 0, 0, 1, 1},
     {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
     {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
     {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
     {&__pyx_kp_u_Cannot_get_series_from, __pyx_k_Cannot_get_series_from, sizeof(__pyx_k_Cannot_get_series_from), 0, 1, 0, 0},
     {&__pyx_kp_u_Cannot_index_with_type, __pyx_k_Cannot_index_with_type, sizeof(__pyx_k_Cannot_index_with_type), 0, 1, 0, 0},
     {&__pyx_kp_s_Cannot_transpose_memoryview_with, __pyx_k_Cannot_transpose_memoryview_with, sizeof(__pyx_k_Cannot_transpose_memoryview_with), 0, 0, 1, 0},
-    {&__pyx_n_s_CurveOption, __pyx_k_CurveOption, sizeof(__pyx_k_CurveOption), 0, 0, 1, 1},
-    {&__pyx_n_s_CurveOption___repr, __pyx_k_CurveOption___repr, sizeof(__pyx_k_CurveOption___repr), 0, 0, 1, 1},
-    {&__pyx_kp_s_Curve_Option_Enumeration, __pyx_k_Curve_Option_Enumeration, sizeof(__pyx_k_Curve_Option_Enumeration), 0, 0, 1, 0},
     {&__pyx_n_s_DEMA, __pyx_k_DEMA, sizeof(__pyx_k_DEMA), 0, 0, 1, 1},
     {&__pyx_n_u_DEMA, __pyx_k_DEMA, sizeof(__pyx_k_DEMA), 0, 1, 0, 1},
     {&__pyx_n_s_DIFF, __pyx_k_DIFF, sizeof(__pyx_k_DIFF), 0, 0, 1, 1},
     {&__pyx_n_s_DataFrame, __pyx_k_DataFrame, sizeof(__pyx_k_DataFrame), 0, 0, 1, 1},
     {&__pyx_kp_u_Different_sizes, __pyx_k_Different_sizes, sizeof(__pyx_k_Different_sizes), 0, 1, 0, 0},
     {&__pyx_kp_s_Dimension_d_is_not_direct, __pyx_k_Dimension_d_is_not_direct, sizeof(__pyx_k_Dimension_d_is_not_direct), 0, 0, 1, 0},
     {&__pyx_n_s_EFFICIENCY_RATIO, __pyx_k_EFFICIENCY_RATIO, sizeof(__pyx_k_EFFICIENCY_RATIO), 0, 0, 1, 1},
@@ -73137,15 +71076,15 @@
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
     {&__pyx_n_s_WCLPRICE, __pyx_k_WCLPRICE, sizeof(__pyx_k_WCLPRICE), 0, 0, 1, 1},
     {&__pyx_n_s_WMA, __pyx_k_WMA, sizeof(__pyx_k_WMA), 0, 0, 1, 1},
     {&__pyx_n_u_WMA, __pyx_k_WMA, sizeof(__pyx_k_WMA), 0, 1, 0, 1},
     {&__pyx_kp_u__15, __pyx_k__15, sizeof(__pyx_k__15), 0, 1, 0, 0},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-    {&__pyx_n_s__221, __pyx_k__221, sizeof(__pyx_k__221), 0, 0, 1, 1},
+    {&__pyx_n_s__217, __pyx_k__217, sizeof(__pyx_k__217), 0, 0, 1, 1},
     {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
     {&__pyx_n_s_abc, __pyx_k_abc, sizeof(__pyx_k_abc), 0, 0, 1, 1},
     {&__pyx_n_s_abs, __pyx_k_abs, sizeof(__pyx_k_abs), 0, 0, 1, 1},
     {&__pyx_n_s_adjust, __pyx_k_adjust, sizeof(__pyx_k_adjust), 0, 0, 1, 1},
     {&__pyx_n_s_af, __pyx_k_af, sizeof(__pyx_k_af), 0, 0, 1, 1},
@@ -73174,15 +71113,14 @@
     {&__pyx_n_s_calc_adx, __pyx_k_calc_adx, sizeof(__pyx_k_calc_adx), 0, 0, 1, 1},
     {&__pyx_n_s_calc_atr, __pyx_k_calc_atr, sizeof(__pyx_k_calc_atr), 0, 0, 1, 1},
     {&__pyx_n_s_calc_avgprice, __pyx_k_calc_avgprice, sizeof(__pyx_k_calc_avgprice), 0, 0, 1, 1},
     {&__pyx_n_s_calc_bbands, __pyx_k_calc_bbands, sizeof(__pyx_k_calc_bbands), 0, 0, 1, 1},
     {&__pyx_n_s_calc_bop, __pyx_k_calc_bop, sizeof(__pyx_k_calc_bop), 0, 0, 1, 1},
     {&__pyx_n_s_calc_cci, __pyx_k_calc_cci, sizeof(__pyx_k_calc_cci), 0, 0, 1, 1},
     {&__pyx_n_s_calc_cmf, __pyx_k_calc_cmf, sizeof(__pyx_k_calc_cmf), 0, 0, 1, 1},
-    {&__pyx_n_s_calc_curve, __pyx_k_calc_curve, sizeof(__pyx_k_calc_curve), 0, 0, 1, 1},
     {&__pyx_n_s_calc_dema, __pyx_k_calc_dema, sizeof(__pyx_k_calc_dema), 0, 0, 1, 1},
     {&__pyx_n_s_calc_diff, __pyx_k_calc_diff, sizeof(__pyx_k_calc_diff), 0, 0, 1, 1},
     {&__pyx_n_s_calc_ema, __pyx_k_calc_ema, sizeof(__pyx_k_calc_ema), 0, 0, 1, 1},
     {&__pyx_n_s_calc_eval, __pyx_k_calc_eval, sizeof(__pyx_k_calc_eval), 0, 0, 1, 1},
     {&__pyx_n_s_calc_exp, __pyx_k_calc_exp, sizeof(__pyx_k_calc_exp), 0, 0, 1, 1},
     {&__pyx_n_s_calc_kama, __pyx_k_calc_kama, sizeof(__pyx_k_calc_kama), 0, 0, 1, 1},
     {&__pyx_n_s_calc_keltner, __pyx_k_calc_keltner, sizeof(__pyx_k_calc_keltner), 0, 0, 1, 1},
@@ -73228,15 +71166,14 @@
     {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
     {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
     {&__pyx_kp_u_core, __pyx_k_core, sizeof(__pyx_k_core), 0, 1, 0, 0},
     {&__pyx_n_s_corr, __pyx_k_corr, sizeof(__pyx_k_corr), 0, 0, 1, 1},
     {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
     {&__pyx_n_s_crossover, __pyx_k_crossover, sizeof(__pyx_k_crossover), 0, 0, 1, 1},
     {&__pyx_n_s_crossunder, __pyx_k_crossunder, sizeof(__pyx_k_crossunder), 0, 0, 1, 1},
-    {&__pyx_n_s_curve, __pyx_k_curve, sizeof(__pyx_k_curve), 0, 0, 1, 1},
     {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
     {&__pyx_kp_u_data_2, __pyx_k_data_2, sizeof(__pyx_k_data_2), 0, 1, 0, 0},
     {&__pyx_n_s_dataframe_like, __pyx_k_dataframe_like, sizeof(__pyx_k_dataframe_like), 0, 0, 1, 1},
     {&__pyx_n_s_decorator, __pyx_k_decorator, sizeof(__pyx_k_decorator), 0, 0, 1, 1},
     {&__pyx_n_s_default_item, __pyx_k_default_item, sizeof(__pyx_k_default_item), 0, 0, 1, 1},
     {&__pyx_n_s_di1, __pyx_k_di1, sizeof(__pyx_k_di1), 0, 0, 1, 1},
     {&__pyx_n_s_di2, __pyx_k_di2, sizeof(__pyx_k_di2), 0, 0, 1, 1},
@@ -73439,30 +71376,27 @@
     {&__pyx_n_s_res, __pyx_k_res, sizeof(__pyx_k_res), 0, 0, 1, 1},
     {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
     {&__pyx_n_s_rho, __pyx_k_rho, sizeof(__pyx_k_rho), 0, 0, 1, 1},
     {&__pyx_n_s_rma, __pyx_k_rma, sizeof(__pyx_k_rma), 0, 0, 1, 1},
     {&__pyx_n_s_rmse, __pyx_k_rmse, sizeof(__pyx_k_rmse), 0, 0, 1, 1},
     {&__pyx_n_s_roc, __pyx_k_roc, sizeof(__pyx_k_roc), 0, 0, 1, 1},
     {&__pyx_n_s_rsi, __pyx_k_rsi, sizeof(__pyx_k_rsi), 0, 0, 1, 1},
-    {&__pyx_n_s_rsquare, __pyx_k_rsquare, sizeof(__pyx_k_rsquare), 0, 0, 1, 1},
-    {&__pyx_n_s_rvalue, __pyx_k_rvalue, sizeof(__pyx_k_rvalue), 0, 0, 1, 1},
     {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
     {&__pyx_n_s_same_scale, __pyx_k_same_scale, sizeof(__pyx_k_same_scale), 0, 0, 1, 1},
     {&__pyx_n_u_same_scale, __pyx_k_same_scale, sizeof(__pyx_k_same_scale), 0, 1, 0, 1},
     {&__pyx_n_s_sar, __pyx_k_sar, sizeof(__pyx_k_sar), 0, 0, 1, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
     {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
     {&__pyx_n_s_series, __pyx_k_series, sizeof(__pyx_k_series), 0, 0, 1, 1},
     {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
     {&__pyx_n_s_signal, __pyx_k_signal, sizeof(__pyx_k_signal), 0, 0, 1, 1},
     {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
-    {&__pyx_n_s_skip, __pyx_k_skip, sizeof(__pyx_k_skip), 0, 0, 1, 1},
     {&__pyx_n_s_slope, __pyx_k_slope, sizeof(__pyx_k_slope), 0, 0, 1, 1},
     {&__pyx_n_s_slowd, __pyx_k_slowd, sizeof(__pyx_k_slowd), 0, 0, 1, 1},
     {&__pyx_n_s_slowf, __pyx_k_slowf, sizeof(__pyx_k_slowf), 0, 0, 1, 1},
     {&__pyx_n_s_slowk, __pyx_k_slowk, sizeof(__pyx_k_slowk), 0, 0, 1, 1},
     {&__pyx_kp_u_slowk_slowd, __pyx_k_slowk_slowd, sizeof(__pyx_k_slowk_slowd), 0, 1, 0, 0},
     {&__pyx_n_s_slown, __pyx_k_slown, sizeof(__pyx_k_slown), 0, 0, 1, 1},
     {&__pyx_n_s_sma, __pyx_k_sma, sizeof(__pyx_k_sma), 0, 0, 1, 1},
@@ -73472,15 +71406,14 @@
     {&__pyx_kp_s_src_mintalib_cython_adx_pxi, __pyx_k_src_mintalib_cython_adx_pxi, sizeof(__pyx_k_src_mintalib_cython_adx_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_atr_pxi, __pyx_k_src_mintalib_cython_atr_pxi, sizeof(__pyx_k_src_mintalib_cython_atr_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_bbands_pxi, __pyx_k_src_mintalib_cython_bbands_pxi, sizeof(__pyx_k_src_mintalib_cython_bbands_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_bop_pxi, __pyx_k_src_mintalib_cython_bop_pxi, sizeof(__pyx_k_src_mintalib_cython_bop_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_cci_pxi, __pyx_k_src_mintalib_cython_cci_pxi, sizeof(__pyx_k_src_mintalib_cython_cci_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_cmf_pxi, __pyx_k_src_mintalib_cython_cmf_pxi, sizeof(__pyx_k_src_mintalib_cython_cmf_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_cross_pxi, __pyx_k_src_mintalib_cython_cross_pxi, sizeof(__pyx_k_src_mintalib_cython_cross_pxi), 0, 0, 1, 0},
-    {&__pyx_kp_s_src_mintalib_cython_curve_pxi, __pyx_k_src_mintalib_cython_curve_pxi, sizeof(__pyx_k_src_mintalib_cython_curve_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_dema_pxi, __pyx_k_src_mintalib_cython_dema_pxi, sizeof(__pyx_k_src_mintalib_cython_dema_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_diff_pxi, __pyx_k_src_mintalib_cython_diff_pxi, sizeof(__pyx_k_src_mintalib_cython_diff_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_ema_pxi, __pyx_k_src_mintalib_cython_ema_pxi, sizeof(__pyx_k_src_mintalib_cython_ema_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_eval_pxi, __pyx_k_src_mintalib_cython_eval_pxi, sizeof(__pyx_k_src_mintalib_cython_eval_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_exp_pxi, __pyx_k_src_mintalib_cython_exp_pxi, sizeof(__pyx_k_src_mintalib_cython_exp_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_flags_pxi, __pyx_k_src_mintalib_cython_flags_pxi, sizeof(__pyx_k_src_mintalib_cython_flags_pxi), 0, 0, 1, 0},
     {&__pyx_kp_s_src_mintalib_cython_kama_pxi, __pyx_k_src_mintalib_cython_kama_pxi, sizeof(__pyx_k_src_mintalib_cython_kama_pxi), 0, 0, 1, 0},
@@ -73522,21 +71455,17 @@
     {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
     {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
     {&__pyx_n_s_sx, __pyx_k_sx, sizeof(__pyx_k_sx), 0, 0, 1, 1},
     {&__pyx_n_s_sxx, __pyx_k_sxx, sizeof(__pyx_k_sxx), 0, 0, 1, 1},
     {&__pyx_n_s_sxy, __pyx_k_sxy, sizeof(__pyx_k_sxy), 0, 0, 1, 1},
-    {&__pyx_n_s_sxz, __pyx_k_sxz, sizeof(__pyx_k_sxz), 0, 0, 1, 1},
     {&__pyx_n_s_sy, __pyx_k_sy, sizeof(__pyx_k_sy), 0, 0, 1, 1},
     {&__pyx_n_s_sys, __pyx_k_sys, sizeof(__pyx_k_sys), 0, 0, 1, 1},
     {&__pyx_n_s_syy, __pyx_k_syy, sizeof(__pyx_k_syy), 0, 0, 1, 1},
-    {&__pyx_n_s_syz, __pyx_k_syz, sizeof(__pyx_k_syz), 0, 0, 1, 1},
-    {&__pyx_n_s_sz, __pyx_k_sz, sizeof(__pyx_k_sz), 0, 0, 1, 1},
-    {&__pyx_n_s_szz, __pyx_k_szz, sizeof(__pyx_k_szz), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
     {&__pyx_n_s_tname, __pyx_k_tname, sizeof(__pyx_k_tname), 0, 0, 1, 1},
     {&__pyx_n_s_total, __pyx_k_total, sizeof(__pyx_k_total), 0, 0, 1, 1},
     {&__pyx_n_s_tr, __pyx_k_tr, sizeof(__pyx_k_tr), 0, 0, 1, 1},
     {&__pyx_n_s_trange, __pyx_k_trange, sizeof(__pyx_k_trange), 0, 0, 1, 1},
     {&__pyx_n_s_trend, __pyx_k_trend, sizeof(__pyx_k_trend), 0, 0, 1, 1},
@@ -73558,18 +71487,15 @@
     {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
     {&__pyx_n_s_version_info, __pyx_k_version_info, sizeof(__pyx_k_version_info), 0, 0, 1, 1},
     {&__pyx_n_s_volume, __pyx_k_volume, sizeof(__pyx_k_volume), 0, 0, 1, 1},
     {&__pyx_n_u_volume, __pyx_k_volume, sizeof(__pyx_k_volume), 0, 1, 0, 1},
     {&__pyx_n_s_vsum, __pyx_k_vsum, sizeof(__pyx_k_vsum), 0, 0, 1, 1},
     {&__pyx_n_s_vxx, __pyx_k_vxx, sizeof(__pyx_k_vxx), 0, 0, 1, 1},
     {&__pyx_n_s_vxy, __pyx_k_vxy, sizeof(__pyx_k_vxy), 0, 0, 1, 1},
-    {&__pyx_n_s_vxz, __pyx_k_vxz, sizeof(__pyx_k_vxz), 0, 0, 1, 1},
     {&__pyx_n_s_vyy, __pyx_k_vyy, sizeof(__pyx_k_vyy), 0, 0, 1, 1},
-    {&__pyx_n_s_vyz, __pyx_k_vyz, sizeof(__pyx_k_vyz), 0, 0, 1, 1},
-    {&__pyx_n_s_vzz, __pyx_k_vzz, sizeof(__pyx_k_vzz), 0, 0, 1, 1},
     {&__pyx_n_s_wcl, __pyx_k_wcl, sizeof(__pyx_k_wcl), 0, 0, 1, 1},
     {&__pyx_n_s_where, __pyx_k_where, sizeof(__pyx_k_where), 0, 0, 1, 1},
     {&__pyx_n_s_where_flag, __pyx_k_where_flag, sizeof(__pyx_k_where_flag), 0, 0, 1, 1},
     {&__pyx_n_s_wrap, __pyx_k_wrap, sizeof(__pyx_k_wrap), 0, 0, 1, 1},
     {&__pyx_n_s_wrap_function, __pyx_k_wrap_function, sizeof(__pyx_k_wrap_function), 0, 0, 1, 1},
     {&__pyx_n_s_wrap_function_locals_decorator, __pyx_k_wrap_function_locals_decorator, sizeof(__pyx_k_wrap_function_locals_decorator), 0, 0, 1, 1},
     {&__pyx_n_s_wrap_indicator, __pyx_k_wrap_indicator, sizeof(__pyx_k_wrap_indicator), 0, 0, 1, 1},
@@ -74980,141 +72906,111 @@
  *     """ Forecast (time linear regression) """
  */
   __pyx_tuple__201 = PyTuple_Pack(5, __pyx_n_s_series, __pyx_n_s_period, __pyx_n_s_offset, __pyx_n_s_item, __pyx_n_s_result); if (unlikely(!__pyx_tuple__201)) __PYX_ERR(35, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__201);
   __Pyx_GIVEREF(__pyx_tuple__201);
   __pyx_codeobj__202 = (PyObject*)__Pyx_PyCode_New(3, 0, 1, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__201, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_slope_pxi, __pyx_n_s_FORECAST, 121, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__202)) __PYX_ERR(35, 121, __pyx_L1_error)
 
-  /* "src/mintalib/cython/curve.pxi":15
- * class CurveOption(IntEnum):
- *     """ Curve Option Enumeration """
- *     def __repr__(self):             # <<<<<<<<<<<<<<
- *         return str(self)
- * 
- */
-  __pyx_codeobj__203 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__195, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_curve_pxi, __pyx_n_s_repr, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__203)) __PYX_ERR(36, 15, __pyx_L1_error)
-
-  /* "src/mintalib/cython/curve.pxi":25
- * 
- * 
- * def calc_curve(series, long period=20, *, int option=0, int offset=0, wrap: bool = False):             # <<<<<<<<<<<<<<
- *     """ Curve (time curvilinear regression) """
- * 
- */
-  __pyx_tuple__204 = PyTuple_Pack(36, __pyx_n_s_series, __pyx_n_s_period, __pyx_n_s_option, __pyx_n_s_offset, __pyx_n_s_wrap, __pyx_n_s_zs, __pyx_n_s_size, __pyx_n_s_result, __pyx_n_s_output, __pyx_n_s_x, __pyx_n_s_sx, __pyx_n_s_sxx, __pyx_n_s_vxx, __pyx_n_s_y, __pyx_n_s_sy, __pyx_n_s_syy, __pyx_n_s_vyy, __pyx_n_s_z, __pyx_n_s_sz, __pyx_n_s_szz, __pyx_n_s_vzz, __pyx_n_s_s, __pyx_n_s_sxz, __pyx_n_s_vxz, __pyx_n_s_syz, __pyx_n_s_vyz, __pyx_n_s_slope, __pyx_n_s_curve, __pyx_n_s_intercept, __pyx_n_s_mse, __pyx_n_s_rmse, __pyx_n_s_rvalue, __pyx_n_s_rsquare, __pyx_n_s_skip, __pyx_n_s_i, __pyx_n_s_j); if (unlikely(!__pyx_tuple__204)) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__204);
-  __Pyx_GIVEREF(__pyx_tuple__204);
-  __pyx_codeobj__205 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 36, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__204, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_curve_pxi, __pyx_n_s_calc_curve, 25, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__205)) __PYX_ERR(36, 25, __pyx_L1_error)
-
-  /* "src/mintalib/cython/curve.pxi":149
- * 
- * 
- * @wrap_function(calc_curve)             # <<<<<<<<<<<<<<
- * def CURVE(series, period: int = 20, *, item: str = None):
- *     """ Curve (time curvilinear regression) """
- */
-  __pyx_codeobj__206 = (PyObject*)__Pyx_PyCode_New(2, 0, 1, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__87, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_curve_pxi, __pyx_n_s_CURVE, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__206)) __PYX_ERR(36, 149, __pyx_L1_error)
-
   /* "src/mintalib/cython/stoch.pxi":4
  * 
  * 
  * stoch_result = namedtuple("stoch_result", "slowk, slowd")             # <<<<<<<<<<<<<<
  * 
  * def calc_stoch(prices, long period=14, long fastn=3, long slown=3, *, wrap: bool = False):
  */
-  __pyx_tuple__207 = PyTuple_Pack(2, __pyx_n_u_stoch_result, __pyx_kp_u_slowk_slowd); if (unlikely(!__pyx_tuple__207)) __PYX_ERR(37, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__207);
-  __Pyx_GIVEREF(__pyx_tuple__207);
+  __pyx_tuple__203 = PyTuple_Pack(2, __pyx_n_u_stoch_result, __pyx_kp_u_slowk_slowd); if (unlikely(!__pyx_tuple__203)) __PYX_ERR(36, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__203);
+  __Pyx_GIVEREF(__pyx_tuple__203);
 
   /* "src/mintalib/cython/stoch.pxi":6
  * stoch_result = namedtuple("stoch_result", "slowk, slowd")
  * 
  * def calc_stoch(prices, long period=14, long fastn=3, long slown=3, *, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Stochastic Oscillator """
  * 
  */
-  __pyx_tuple__208 = PyTuple_Pack(15, __pyx_n_s_prices, __pyx_n_s_period, __pyx_n_s_fastn, __pyx_n_s_slown, __pyx_n_s_wrap, __pyx_n_s_high, __pyx_n_s_low, __pyx_n_s_close, __pyx_n_s_size, __pyx_n_s_hi, __pyx_n_s_lo, __pyx_n_s_fastk, __pyx_n_s_slowk, __pyx_n_s_slowd, __pyx_n_s_result); if (unlikely(!__pyx_tuple__208)) __PYX_ERR(37, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__208);
-  __Pyx_GIVEREF(__pyx_tuple__208);
-  __pyx_codeobj__209 = (PyObject*)__Pyx_PyCode_New(4, 0, 1, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__208, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_stoch_pxi, __pyx_n_s_calc_stoch, 6, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__209)) __PYX_ERR(37, 6, __pyx_L1_error)
+  __pyx_tuple__204 = PyTuple_Pack(15, __pyx_n_s_prices, __pyx_n_s_period, __pyx_n_s_fastn, __pyx_n_s_slown, __pyx_n_s_wrap, __pyx_n_s_high, __pyx_n_s_low, __pyx_n_s_close, __pyx_n_s_size, __pyx_n_s_hi, __pyx_n_s_lo, __pyx_n_s_fastk, __pyx_n_s_slowk, __pyx_n_s_slowd, __pyx_n_s_result); if (unlikely(!__pyx_tuple__204)) __PYX_ERR(36, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__204);
+  __Pyx_GIVEREF(__pyx_tuple__204);
+  __pyx_codeobj__205 = (PyObject*)__Pyx_PyCode_New(4, 0, 1, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__204, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_stoch_pxi, __pyx_n_s_calc_stoch, 6, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__205)) __PYX_ERR(36, 6, __pyx_L1_error)
 
   /* "src/mintalib/cython/stoch.pxi":32
  * 
  * 
  * @wrap_function(calc_stoch)             # <<<<<<<<<<<<<<
  * def STOCH(prices, period: int = 14, fastn: int = 3, slown: int = 3):
  *     result = calc_stoch(prices, period=period, fastn=fastn, slown=slown)
  */
-  __pyx_tuple__210 = PyTuple_Pack(5, __pyx_n_s_prices, __pyx_n_s_period, __pyx_n_s_fastn, __pyx_n_s_slown, __pyx_n_s_result); if (unlikely(!__pyx_tuple__210)) __PYX_ERR(37, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__210);
-  __Pyx_GIVEREF(__pyx_tuple__210);
-  __pyx_codeobj__211 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__210, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_stoch_pxi, __pyx_n_s_STOCH, 32, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__211)) __PYX_ERR(37, 32, __pyx_L1_error)
+  __pyx_tuple__206 = PyTuple_Pack(5, __pyx_n_s_prices, __pyx_n_s_period, __pyx_n_s_fastn, __pyx_n_s_slown, __pyx_n_s_result); if (unlikely(!__pyx_tuple__206)) __PYX_ERR(36, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__206);
+  __Pyx_GIVEREF(__pyx_tuple__206);
+  __pyx_codeobj__207 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__206, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_stoch_pxi, __pyx_n_s_STOCH, 32, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__207)) __PYX_ERR(36, 32, __pyx_L1_error)
 
   /* "src/mintalib/cython/streak.pxi":3
  * """ Streak """
  * 
  * def streak_up(series, *, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Consecutive streak of ups """
  * 
  */
-  __pyx_tuple__212 = PyTuple_Pack(11, __pyx_n_s_series, __pyx_n_s_wrap, __pyx_n_s_xs, __pyx_n_s_size, __pyx_n_s_result, __pyx_n_s_output, __pyx_n_s_value, __pyx_n_s_prev, __pyx_n_s_diff, __pyx_n_s_streak, __pyx_n_s_i); if (unlikely(!__pyx_tuple__212)) __PYX_ERR(38, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__212);
-  __Pyx_GIVEREF(__pyx_tuple__212);
-  __pyx_codeobj__213 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__212, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_streak_pxi, __pyx_n_s_streak_up, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__213)) __PYX_ERR(38, 3, __pyx_L1_error)
+  __pyx_tuple__208 = PyTuple_Pack(11, __pyx_n_s_series, __pyx_n_s_wrap, __pyx_n_s_xs, __pyx_n_s_size, __pyx_n_s_result, __pyx_n_s_output, __pyx_n_s_value, __pyx_n_s_prev, __pyx_n_s_diff, __pyx_n_s_streak, __pyx_n_s_i); if (unlikely(!__pyx_tuple__208)) __PYX_ERR(37, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__208);
+  __Pyx_GIVEREF(__pyx_tuple__208);
+  __pyx_codeobj__209 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__208, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_streak_pxi, __pyx_n_s_streak_up, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__209)) __PYX_ERR(37, 3, __pyx_L1_error)
 
   /* "src/mintalib/cython/streak.pxi":38
  * 
  * 
  * def streak_down(series, *, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Consecutive streak of downs """
  * 
  */
-  __pyx_codeobj__214 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__212, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_streak_pxi, __pyx_n_s_streak_down, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__214)) __PYX_ERR(38, 38, __pyx_L1_error)
+  __pyx_codeobj__210 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__208, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_streak_pxi, __pyx_n_s_streak_down, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__210)) __PYX_ERR(37, 38, __pyx_L1_error)
 
   /* "src/mintalib/cython/streak.pxi":72
  * 
  * 
  * @wrap_function(streak_up)             # <<<<<<<<<<<<<<
  * def STREAK_UP(series, *, item: str = None):
  *     series = get_series(series, item=item)
  */
-  __pyx_codeobj__215 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_streak_pxi, __pyx_n_s_STREAK_UP, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__215)) __PYX_ERR(38, 72, __pyx_L1_error)
+  __pyx_codeobj__211 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_streak_pxi, __pyx_n_s_STREAK_UP, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__211)) __PYX_ERR(37, 72, __pyx_L1_error)
 
   /* "src/mintalib/cython/streak.pxi":79
  * 
  * 
  * @wrap_function(streak_down)             # <<<<<<<<<<<<<<
  * def STREAK_DOWN(series, *, item: str = None):
  *     series = get_series(series, item=item)
  */
-  __pyx_codeobj__216 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_streak_pxi, __pyx_n_s_STREAK_DOWN, 79, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__216)) __PYX_ERR(38, 79, __pyx_L1_error)
+  __pyx_codeobj__212 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_streak_pxi, __pyx_n_s_STREAK_DOWN, 79, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__212)) __PYX_ERR(37, 79, __pyx_L1_error)
 
   /* "src/mintalib/cython/eval.pxi":3
  * """ Expression eval """
  * 
  * def calc_eval(prices, expr: str):             # <<<<<<<<<<<<<<
  *     """
  *     Expression Eval (pandas only)
  */
-  __pyx_tuple__217 = PyTuple_Pack(2, __pyx_n_s_prices, __pyx_n_s_expr); if (unlikely(!__pyx_tuple__217)) __PYX_ERR(39, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__217);
-  __Pyx_GIVEREF(__pyx_tuple__217);
-  __pyx_codeobj__218 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__217, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_eval_pxi, __pyx_n_s_calc_eval, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__218)) __PYX_ERR(39, 3, __pyx_L1_error)
+  __pyx_tuple__213 = PyTuple_Pack(2, __pyx_n_s_prices, __pyx_n_s_expr); if (unlikely(!__pyx_tuple__213)) __PYX_ERR(38, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__213);
+  __Pyx_GIVEREF(__pyx_tuple__213);
+  __pyx_codeobj__214 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__213, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_eval_pxi, __pyx_n_s_calc_eval, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__214)) __PYX_ERR(38, 3, __pyx_L1_error)
 
   /* "src/mintalib/cython/eval.pxi":14
  * 
  * 
  * @wrap_function(calc_eval)             # <<<<<<<<<<<<<<
  * def EVAL(prices, expr: str):
  *     result = calc_eval(prices, expr=expr)
  */
-  __pyx_tuple__219 = PyTuple_Pack(3, __pyx_n_s_prices, __pyx_n_s_expr, __pyx_n_s_result); if (unlikely(!__pyx_tuple__219)) __PYX_ERR(39, 14, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__219);
-  __Pyx_GIVEREF(__pyx_tuple__219);
-  __pyx_codeobj__220 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__219, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_eval_pxi, __pyx_n_s_EVAL, 14, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__220)) __PYX_ERR(39, 14, __pyx_L1_error)
+  __pyx_tuple__215 = PyTuple_Pack(3, __pyx_n_s_prices, __pyx_n_s_expr, __pyx_n_s_result); if (unlikely(!__pyx_tuple__215)) __PYX_ERR(38, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__215);
+  __Pyx_GIVEREF(__pyx_tuple__215);
+  __pyx_codeobj__216 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__215, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mintalib_cython_eval_pxi, __pyx_n_s_EVAL, 14, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__216)) __PYX_ERR(38, 14, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -76932,15 +74828,15 @@
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_wrap, __pyx_n_s_bool) < 0) __PYX_ERR(5, 3, __pyx_L1_error)
   __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_41flag_above, 0, __pyx_n_s_flag_above, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__64)); if (unlikely(!__pyx_t_7)) __PYX_ERR(5, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_7, sizeof(__pyx_defaults), 0)) __PYX_ERR(5, 3, __pyx_L1_error)
   __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_7)->__pyx_arg_na_value = __pyx_v_8mintalib_4core_NAN;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_229__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_225__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_flag_above, __pyx_t_7) < 0) __PYX_ERR(5, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/flags.pxi":35
  * 
@@ -76952,15 +74848,15 @@
   __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(5, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_wrap, __pyx_n_s_bool) < 0) __PYX_ERR(5, 35, __pyx_L1_error)
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_43flag_below, 0, __pyx_n_s_flag_below, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__65)); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_5, sizeof(__pyx_defaults1), 0)) __PYX_ERR(5, 35, __pyx_L1_error)
   __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_5)->__pyx_arg_na_value = __pyx_v_8mintalib_4core_NAN;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_231__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_227__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_flag_below, __pyx_t_5) < 0) __PYX_ERR(5, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/mintalib/cython/flags.pxi":67
  * 
@@ -76972,15 +74868,15 @@
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_wrap, __pyx_n_s_bool) < 0) __PYX_ERR(5, 67, __pyx_L1_error)
   __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_45invert_flag, 0, __pyx_n_s_invert_flag, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__67)); if (unlikely(!__pyx_t_7)) __PYX_ERR(5, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_7, sizeof(__pyx_defaults2), 0)) __PYX_ERR(5, 67, __pyx_L1_error)
   __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_7)->__pyx_arg_na_value = __pyx_v_8mintalib_4core_NAN;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_233__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_229__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_invert_flag, __pyx_t_7) < 0) __PYX_ERR(5, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/flags.pxi":99
  * 
@@ -77000,15 +74896,15 @@
  * 
  * def updown_flag(series, double up_level=0.0, double down_level=0.0, *,
  *                 double up_flag=1.0, double down_flag=0.0, double start_flag=NAN,             # <<<<<<<<<<<<<<
  *                 wrap: bool = False):
  *     """ Flag for value crossing levels up & down """
  */
   __Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_t_5)->__pyx_arg_start_flag = __pyx_v_8mintalib_4core_NAN;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_235__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_231__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_updown_flag, __pyx_t_5) < 0) __PYX_ERR(5, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/mintalib/cython/flags.pxi":134
  * 
@@ -77024,15 +74920,15 @@
   __Pyx_GOTREF(__pyx_t_7);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_7, sizeof(__pyx_defaults4), 1)) __PYX_ERR(5, 134, __pyx_L1_error)
   __pyx_t_10 = PyFloat_FromDouble(__pyx_v_8mintalib_4core_NAN); if (unlikely(!__pyx_t_10)) __PYX_ERR(5, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_CyFunction_Defaults(__pyx_defaults4, __pyx_t_7)->__pyx_arg_z = __pyx_t_10;
   __Pyx_GIVEREF(__pyx_t_10);
   __pyx_t_10 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_237__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_233__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_where_flag, __pyx_t_7) < 0) __PYX_ERR(5, 134, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/flags.pxi":172
  * 
@@ -77062,15 +74958,15 @@
  * 
  * @wrap_function(flag_above)
  * def FLAG_ABOVE(series, level: float = 0.0, *, na_value: float = NAN, item: str = None):             # <<<<<<<<<<<<<<
  *     series = get_series(series, item=item)
  *     result = flag_above(series, level=level, na_value=na_value)
  */
   __Pyx_CyFunction_Defaults(__pyx_defaults5, __pyx_t_7)->__pyx_arg_na_value = __pyx_v_8mintalib_4core_NAN;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_239__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_235__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/mintalib/cython/flags.pxi":172
  * 
  * 
  * @wrap_function(flag_above)             # <<<<<<<<<<<<<<
@@ -77112,15 +75008,15 @@
  * 
  * @wrap_function(flag_below)
  * def FLAG_BELOW(series, level: float = 0.0, *, na_value: float = NAN, item: str = None):             # <<<<<<<<<<<<<<
  *     series = get_series(series, item=item)
  *     result = flag_below(series, level=level, na_value=na_value)
  */
   __Pyx_CyFunction_Defaults(__pyx_defaults6, __pyx_t_5)->__pyx_arg_na_value = __pyx_v_8mintalib_4core_NAN;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_241__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_237__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/flags.pxi":179
  * 
  * 
  * @wrap_function(flag_below)             # <<<<<<<<<<<<<<
@@ -77161,15 +75057,15 @@
  * 
  * @wrap_function(invert_flag)
  * def INVERT_FLAG(series, *, na_value: float = NAN, item: str = None):             # <<<<<<<<<<<<<<
  *     series = get_series(series, item=item)
  *     result = invert_flag(series, na_value=na_value)
  */
   __Pyx_CyFunction_Defaults(__pyx_defaults7, __pyx_t_7)->__pyx_arg_na_value = __pyx_v_8mintalib_4core_NAN;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_243__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_239__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/mintalib/cython/flags.pxi":186
  * 
  * 
  * @wrap_function(invert_flag)             # <<<<<<<<<<<<<<
@@ -77214,15 +75110,15 @@
  * @wrap_function(updown_flag)
  * def UPDOWN_FLAG(series, up_level: float = 0.0, down_level: float = 0.0, *,
  *                 up_flag: float = 1.0, down_flag: float = 0.0, start_flag: float = NAN, item: str = None):             # <<<<<<<<<<<<<<
  *     series = get_series(series, item=item)
  *     result = updown_flag(series, up_level=up_level, down_level=down_level, up_flag=up_flag, down_flag=down_flag, start_flag=start_flag)
  */
   __Pyx_CyFunction_Defaults(__pyx_defaults8, __pyx_t_5)->__pyx_arg_start_flag = __pyx_v_8mintalib_4core_NAN;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_245__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_241__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/flags.pxi":193
  * 
  * 
  * @wrap_function(updown_flag)             # <<<<<<<<<<<<<<
@@ -77441,15 +75337,15 @@
  *     series = get_series(series, item=item)
  *     result = calc_roc(series, period=period)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_1))) __PYX_ERR(8, 33, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_CyFunction_Defaults(__pyx_defaults9, __pyx_t_11)->__pyx_arg_period = ((PyObject*)__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_247__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_243__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_11, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/roc.pxi":32
  * 
  * 
  * @wrap_function(calc_roc)             # <<<<<<<<<<<<<<
@@ -77524,15 +75420,15 @@
  *     series = get_series(series, item=item)
  *     result = calc_diff(series, period=period)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_1))) __PYX_ERR(9, 32, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_CyFunction_Defaults(__pyx_defaults10, __pyx_t_5)->__pyx_arg_period = ((PyObject*)__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_249__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_245__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/diff.pxi":31
  * 
  * 
  * @wrap_function(calc_diff)             # <<<<<<<<<<<<<<
@@ -77826,15 +75722,15 @@
  *     series = get_series(series, item=item)
  *     result = calc_mad(series, period=period)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(13, 51, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults11, __pyx_t_5)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_251__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_247__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/mad.pxi":50
  * 
  * 
  * @wrap_function(calc_mad)             # <<<<<<<<<<<<<<
@@ -77909,15 +75805,15 @@
  *     series = get_series(series, item=item)
  *     result = calc_stdev(series, period=period)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(14, 48, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults12, __pyx_t_11)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_253__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_249__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_11, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/stdev.pxi":47
  * 
  * 
  * @wrap_function(calc_stdev)             # <<<<<<<<<<<<<<
@@ -78359,15 +76255,15 @@
  *     series = get_series(series, item=item)
  *     result = calc_tema(series, period=period)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(20, 24, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults13, __pyx_t_10)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_255__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_251__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_10, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/tema.pxi":23
  * 
  * 
  * @wrap_function(calc_tema)             # <<<<<<<<<<<<<<
@@ -78445,15 +76341,15 @@
  *     series = get_series(series, item=item)
  *     result = calc_ma(series, period=period, ma_type=ma_type)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(21, 40, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults14, __pyx_t_5)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_257__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_253__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_11);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
   /* "src/mintalib/cython/matype.pxi":39
  * 
  * 
  * @wrap_function(calc_ma)             # <<<<<<<<<<<<<<
@@ -78528,15 +76424,15 @@
  *     series = get_series(series, item=item)
  *     result = calc_rsi(series, period=period)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_14)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_14))) __PYX_ERR(22, 54, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_14);
   __Pyx_CyFunction_Defaults(__pyx_defaults15, __pyx_t_10)->__pyx_arg_period = ((PyObject*)__pyx_int_14);
   __Pyx_GIVEREF(__pyx_int_14);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_259__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_255__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_10, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/rsi.pxi":53
  * 
  * 
  * @wrap_function(calc_rsi)             # <<<<<<<<<<<<<<
@@ -78672,15 +76568,15 @@
  *     result = calc_plusdi(prices, period=period)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_14)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_14))) __PYX_ERR(23, 74, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_14);
   __Pyx_CyFunction_Defaults(__pyx_defaults16, __pyx_t_11)->__pyx_arg_period = ((PyObject*)__pyx_int_14);
   __Pyx_GIVEREF(__pyx_int_14);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_261__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_257__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_11, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/mintalib/cython/adx.pxi":73
  * 
  * 
  * @wrap_function(calc_plusdi)             # <<<<<<<<<<<<<<
@@ -78723,15 +76619,15 @@
  *     result = calc_minusdi(prices, period=period)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_14)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_14))) __PYX_ERR(23, 80, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_14);
   __Pyx_CyFunction_Defaults(__pyx_defaults17, __pyx_t_5)->__pyx_arg_period = ((PyObject*)__pyx_int_14);
   __Pyx_GIVEREF(__pyx_int_14);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_263__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_259__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_11);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
   /* "src/mintalib/cython/adx.pxi":79
  * 
  * 
  * @wrap_function(calc_minusdi)             # <<<<<<<<<<<<<<
@@ -78774,15 +76670,15 @@
  *     result = calc_adx(prices, period=period)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_14)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_14))) __PYX_ERR(23, 86, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_14);
   __Pyx_CyFunction_Defaults(__pyx_defaults18, __pyx_t_11)->__pyx_arg_period = ((PyObject*)__pyx_int_14);
   __Pyx_GIVEREF(__pyx_int_14);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_265__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_261__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_11, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/mintalib/cython/adx.pxi":85
  * 
  * 
  * @wrap_function(calc_adx)             # <<<<<<<<<<<<<<
@@ -78980,15 +76876,15 @@
  *     result = calc_atr(prices, period=period)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_14)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_14))) __PYX_ERR(24, 98, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_14);
   __Pyx_CyFunction_Defaults(__pyx_defaults19, __pyx_t_5)->__pyx_arg_period = ((PyObject*)__pyx_int_14);
   __Pyx_GIVEREF(__pyx_int_14);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_267__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_263__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/atr.pxi":97
  * 
  * 
  * @wrap_function(calc_atr)             # <<<<<<<<<<<<<<
@@ -79031,15 +76927,15 @@
  *     result = calc_natr(prices, period=period)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_14)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_14))) __PYX_ERR(24, 104, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_14);
   __Pyx_CyFunction_Defaults(__pyx_defaults20, __pyx_t_10)->__pyx_arg_period = ((PyObject*)__pyx_int_14);
   __Pyx_GIVEREF(__pyx_int_14);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_269__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_265__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_10, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/mintalib/cython/atr.pxi":103
  * 
  * 
  * @wrap_function(calc_natr)             # <<<<<<<<<<<<<<
@@ -79082,15 +76978,15 @@
  *     result = calc_latr(prices, period=period)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_14)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_14))) __PYX_ERR(24, 110, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_14);
   __Pyx_CyFunction_Defaults(__pyx_defaults21, __pyx_t_5)->__pyx_arg_period = ((PyObject*)__pyx_int_14);
   __Pyx_GIVEREF(__pyx_int_14);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_271__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_267__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/atr.pxi":109
  * 
  * 
  * @wrap_function(calc_latr)             # <<<<<<<<<<<<<<
@@ -79260,15 +77156,15 @@
  *     result = calc_cci(prices, period=period)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(26, 21, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults22, __pyx_t_11)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_273__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_269__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_11, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/mintalib/cython/cci.pxi":20
  * 
  * 
  * @wrap_function(calc_cci)             # <<<<<<<<<<<<<<
@@ -79342,15 +77238,15 @@
  *     result = calc_cmf(prices, period=period)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(27, 29, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults23, __pyx_t_10)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_275__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_271__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_10, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/cmf.pxi":28
  * 
  * 
  * @wrap_function(calc_cmf)             # <<<<<<<<<<<<<<
@@ -79424,15 +77320,15 @@
  *     result = calc_mfi(prices, period=period)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_14)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_14))) __PYX_ERR(28, 25, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_14);
   __Pyx_CyFunction_Defaults(__pyx_defaults24, __pyx_t_11)->__pyx_arg_period = ((PyObject*)__pyx_int_14);
   __Pyx_GIVEREF(__pyx_int_14);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_277__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_273__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_11, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "src/mintalib/cython/mfi.pxi":24
  * 
  * 
  * @wrap_function(calc_mfi)             # <<<<<<<<<<<<<<
@@ -79506,15 +77402,15 @@
  *     result = calc_bop(prices, period=period)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(29, 25, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults25, __pyx_t_10)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_279__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_275__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_10, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/bop.pxi":24
  * 
  * 
  * @wrap_function(calc_bop)             # <<<<<<<<<<<<<<
@@ -79609,15 +77505,15 @@
  *     result = calc_bbands(prices, period=period, nbdev=nbdev)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(30, 27, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults26, __pyx_t_11)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_281__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_11, __pyx_pf_8mintalib_4core_277__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_11, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/bbands.pxi":26
  * 
  * 
  * @wrap_function(calc_bbands)             # <<<<<<<<<<<<<<
@@ -79712,15 +77608,15 @@
  *     result = calc_keltner(prices, period=period, nbatr=nbatr)
  *     return wrap_result(result, prices)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(31, 24, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults27, __pyx_t_5)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_283__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_8mintalib_4core_279__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_11);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
   /* "src/mintalib/cython/keltner.pxi":23
  * 
  * 
  * @wrap_function(calc_keltner)             # <<<<<<<<<<<<<<
@@ -79836,15 +77732,15 @@
  *     series = get_series(series, item=item)
  *     result = efficiency_ratio(series, period=period)
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_10)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_10))) __PYX_ERR(32, 102, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_10);
   __Pyx_CyFunction_Defaults(__pyx_defaults28, __pyx_t_7)->__pyx_arg_period = ((PyObject*)__pyx_int_10);
   __Pyx_GIVEREF(__pyx_int_10);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_285__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_281__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/kama.pxi":101
  * 
  * 
  * @wrap_function(efficiency_ratio)             # <<<<<<<<<<<<<<
@@ -79898,15 +77794,15 @@
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_CyFunction_Defaults(__pyx_defaults29, __pyx_t_10)->__pyx_arg_fastn = ((PyObject*)__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_30)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_30))) __PYX_ERR(32, 109, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_30);
   __Pyx_CyFunction_Defaults(__pyx_defaults29, __pyx_t_10)->__pyx_arg_slown = ((PyObject*)__pyx_int_30);
   __Pyx_GIVEREF(__pyx_int_30);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_287__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_283__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_10, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/kama.pxi":108
  * 
  * 
  * @wrap_function(calc_kama)             # <<<<<<<<<<<<<<
@@ -80014,15 +77910,15 @@
   __Pyx_INCREF(__pyx_int_26);
   __Pyx_CyFunction_Defaults(__pyx_defaults30, __pyx_t_7)->__pyx_arg_n2 = ((PyObject*)__pyx_int_26);
   __Pyx_GIVEREF(__pyx_int_26);
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_9)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_9))) __PYX_ERR(33, 24, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_9);
   __Pyx_CyFunction_Defaults(__pyx_defaults30, __pyx_t_7)->__pyx_arg_n3 = ((PyObject*)__pyx_int_9);
   __Pyx_GIVEREF(__pyx_int_9);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_289__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_285__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_11);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
   /* "src/mintalib/cython/macd.pxi":23
  * 
  * 
  * @wrap_function(calc_macd)             # <<<<<<<<<<<<<<
@@ -80132,15 +78028,15 @@
   __Pyx_INCREF(__pyx_int_26);
   __Pyx_CyFunction_Defaults(__pyx_defaults31, __pyx_t_7)->__pyx_arg_n2 = ((PyObject*)__pyx_int_26);
   __Pyx_GIVEREF(__pyx_int_26);
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_9)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_9))) __PYX_ERR(34, 27, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_9);
   __Pyx_CyFunction_Defaults(__pyx_defaults31, __pyx_t_7)->__pyx_arg_n3 = ((PyObject*)__pyx_int_9);
   __Pyx_GIVEREF(__pyx_int_9);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_291__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_287__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_11);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
   /* "src/mintalib/cython/ppo.pxi":26
  * 
  * 
  * @wrap_function(calc_ppo)             # <<<<<<<<<<<<<<
@@ -80329,15 +78225,15 @@
  *     """ Slope (time linear regression) """
  * 
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(35, 104, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults32, __pyx_t_7)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_293__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_289__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/slope.pxi":103
  * 
  * 
  * @wrap_function(calc_slope)             # <<<<<<<<<<<<<<
@@ -80381,15 +78277,15 @@
  *     """ RValue (time linear regression) """
  * 
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(35, 113, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults33, __pyx_t_10)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_295__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_10, __pyx_pf_8mintalib_4core_291__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_10, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/slope.pxi":112
  * 
  * 
  * @wrap_function(calc_slope)             # <<<<<<<<<<<<<<
@@ -80438,15 +78334,15 @@
   __Pyx_INCREF(__pyx_int_20);
   __Pyx_CyFunction_Defaults(__pyx_defaults34, __pyx_t_7)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
   __Pyx_GIVEREF(__pyx_int_20);
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(35, 122, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_CyFunction_Defaults(__pyx_defaults34, __pyx_t_7)->__pyx_arg_offset = ((PyObject*)__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_297__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_293__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/slope.pxi":121
  * 
  * 
  * @wrap_function(calc_slope)             # <<<<<<<<<<<<<<
@@ -80456,544 +78352,356 @@
   __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(35, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_FORECAST, __pyx_t_10) < 0) __PYX_ERR(35, 121, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "src/mintalib/cython/curve.pxi":13
- * 
- * 
- * class CurveOption(IntEnum):             # <<<<<<<<<<<<<<
- *     """ Curve Option Enumeration """
- *     def __repr__(self):
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_IntEnum); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GIVEREF(__pyx_t_10);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_10)) __PYX_ERR(36, 13, __pyx_L1_error);
-  __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PEP560_update_bases(__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_11 = __Pyx_CalculateMetaclass(NULL, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(36, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_11, __pyx_t_10, __pyx_n_s_CurveOption, __pyx_n_s_CurveOption, (PyObject *) NULL, __pyx_n_s_mintalib_core, __pyx_kp_s_Curve_Option_Enumeration); if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (__pyx_t_10 != __pyx_t_7) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_7) < 0))) __PYX_ERR(36, 13, __pyx_L1_error)
-  }
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-
-  /* "src/mintalib/cython/curve.pxi":15
- * class CurveOption(IntEnum):
- *     """ Curve Option Enumeration """
- *     def __repr__(self):             # <<<<<<<<<<<<<<
- *         return str(self)
- * 
- */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_11CurveOption_1__repr__, 0, __pyx_n_s_CurveOption___repr, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__203)); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_repr, __pyx_t_7) < 0) __PYX_ERR(36, 15, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-
-  /* "src/mintalib/cython/curve.pxi":18
- *         return str(self)
- * 
- *     CURVE = 0             # <<<<<<<<<<<<<<
- *     SLOPE = 1
- *     RVALUE = 2
- */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_CURVE, __pyx_int_0) < 0) __PYX_ERR(36, 18, __pyx_L1_error)
-
-  /* "src/mintalib/cython/curve.pxi":19
- * 
- *     CURVE = 0
- *     SLOPE = 1             # <<<<<<<<<<<<<<
- *     RVALUE = 2
- *     RSQUARE = 3
- */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_SLOPE, __pyx_int_1) < 0) __PYX_ERR(36, 19, __pyx_L1_error)
-
-  /* "src/mintalib/cython/curve.pxi":20
- *     CURVE = 0
- *     SLOPE = 1
- *     RVALUE = 2             # <<<<<<<<<<<<<<
- *     RSQUARE = 3
- *     RMSERROR = 4
- */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_RVALUE, __pyx_int_2) < 0) __PYX_ERR(36, 20, __pyx_L1_error)
-
-  /* "src/mintalib/cython/curve.pxi":21
- *     SLOPE = 1
- *     RVALUE = 2
- *     RSQUARE = 3             # <<<<<<<<<<<<<<
- *     RMSERROR = 4
- * 
- */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_RSQUARE, __pyx_int_3) < 0) __PYX_ERR(36, 21, __pyx_L1_error)
-
-  /* "src/mintalib/cython/curve.pxi":22
- *     RVALUE = 2
- *     RSQUARE = 3
- *     RMSERROR = 4             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_RMSERROR, __pyx_int_4) < 0) __PYX_ERR(36, 22, __pyx_L1_error)
-
-  /* "src/mintalib/cython/curve.pxi":13
- * 
- * 
- * class CurveOption(IntEnum):             # <<<<<<<<<<<<<<
- *     """ Curve Option Enumeration """
- *     def __repr__(self):
- */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_11, __pyx_n_s_CurveOption, __pyx_t_10, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CurveOption, __pyx_t_7) < 0) __PYX_ERR(36, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-
-  /* "src/mintalib/cython/curve.pxi":25
- * 
- * 
- * def calc_curve(series, long period=20, *, int option=0, int offset=0, wrap: bool = False):             # <<<<<<<<<<<<<<
- *     """ Curve (time curvilinear regression) """
- * 
- */
-  __pyx_t_10 = __Pyx_PyInt_From_long(((long)20)); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
-  __Pyx_GIVEREF(__pyx_t_10);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_10)) __PYX_ERR(36, 25, __pyx_L1_error);
-  __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_5 = __Pyx_PyInt_From_int(((int)0)); if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_option, __pyx_t_5) < 0) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(((int)0)); if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_offset, __pyx_t_5) < 0) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_wrap, ((PyObject *)Py_False)) < 0) __PYX_ERR(36, 25, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_wrap, __pyx_n_s_bool) < 0) __PYX_ERR(36, 25, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_207calc_curve, 0, __pyx_n_s_calc_curve, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__205)); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_t_11);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_7, __pyx_t_10);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
-  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_curve, __pyx_t_7) < 0) __PYX_ERR(36, 25, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-
-  /* "src/mintalib/cython/curve.pxi":149
- * 
- * 
- * @wrap_function(calc_curve)             # <<<<<<<<<<<<<<
- * def CURVE(series, period: int = 20, *, item: str = None):
- *     """ Curve (time curvilinear regression) """
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_wrap_function); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_calc_curve); if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_period, __pyx_n_s_int) < 0) __PYX_ERR(36, 149, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_item, __pyx_n_s_str) < 0) __PYX_ERR(36, 149, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_209CURVE, 0, __pyx_n_s_CURVE, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__206)); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_7, sizeof(__pyx_defaults35), 1)) __PYX_ERR(36, 149, __pyx_L1_error)
-
-  /* "src/mintalib/cython/curve.pxi":150
- * 
- * @wrap_function(calc_curve)
- * def CURVE(series, period: int = 20, *, item: str = None):             # <<<<<<<<<<<<<<
- *     """ Curve (time curvilinear regression) """
- * 
- */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_20)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_20))) __PYX_ERR(36, 150, __pyx_L1_error)
-  __Pyx_INCREF(__pyx_int_20);
-  __Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_t_7)->__pyx_arg_period = ((PyObject*)__pyx_int_20);
-  __Pyx_GIVEREF(__pyx_int_20);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_299__defaults__);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-
-  /* "src/mintalib/cython/curve.pxi":149
- * 
- * 
- * @wrap_function(calc_curve)             # <<<<<<<<<<<<<<
- * def CURVE(series, period: int = 20, *, item: str = None):
- *     """ Curve (time curvilinear regression) """
- */
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CURVE, __pyx_t_5) < 0) __PYX_ERR(36, 149, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-
   /* "src/mintalib/cython/stoch.pxi":4
  * 
  * 
  * stoch_result = namedtuple("stoch_result", "slowk, slowd")             # <<<<<<<<<<<<<<
  * 
  * def calc_stoch(prices, long period=14, long fastn=3, long slown=3, *, wrap: bool = False):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_namedtuple); if (unlikely(!__pyx_t_5)) __PYX_ERR(37, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__207, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 4, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_namedtuple); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_tuple__203, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_stoch_result, __pyx_t_7) < 0) __PYX_ERR(37, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_stoch_result, __pyx_t_7) < 0) __PYX_ERR(36, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/stoch.pxi":6
  * stoch_result = namedtuple("stoch_result", "slowk, slowd")
  * 
  * def calc_stoch(prices, long period=14, long fastn=3, long slown=3, *, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Stochastic Oscillator """
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_long(((long)14)); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 6, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_long(((long)14)); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyInt_From_long(((long)3)); if (unlikely(!__pyx_t_5)) __PYX_ERR(37, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_10 = __Pyx_PyInt_From_long(((long)3)); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 6, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_From_long(((long)3)); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(37, 6, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_From_long(((long)3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(36, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(36, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7)) __PYX_ERR(37, 6, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_5)) __PYX_ERR(37, 6, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7)) __PYX_ERR(36, 6, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_10);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_t_10)) __PYX_ERR(37, 6, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_10)) __PYX_ERR(36, 6, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_11);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_11)) __PYX_ERR(36, 6, __pyx_L1_error);
   __pyx_t_7 = 0;
-  __pyx_t_5 = 0;
   __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 6, __pyx_L1_error)
+  __pyx_t_11 = 0;
+  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(36, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_wrap, ((PyObject *)Py_False)) < 0) __PYX_ERR(36, 6, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_wrap, ((PyObject *)Py_False)) < 0) __PYX_ERR(37, 6, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(37, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_wrap, __pyx_n_s_bool) < 0) __PYX_ERR(37, 6, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_211calc_stoch, 0, __pyx_n_s_calc_stoch, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__209)); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 6, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_wrap, __pyx_n_s_bool) < 0) __PYX_ERR(36, 6, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_207calc_stoch, 0, __pyx_n_s_calc_stoch, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__205)); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_t_11);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_7, __pyx_t_10);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_t_5);
+  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_7, __pyx_t_11);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_10);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_stoch, __pyx_t_7) < 0) __PYX_ERR(37, 6, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_stoch, __pyx_t_7) < 0) __PYX_ERR(36, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/stoch.pxi":32
  * 
  * 
  * @wrap_function(calc_stoch)             # <<<<<<<<<<<<<<
  * def STOCH(prices, period: int = 14, fastn: int = 3, slown: int = 3):
  *     result = calc_stoch(prices, period=period, fastn=fastn, slown=slown)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_wrap_function); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 32, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_wrap_function); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_calc_stoch); if (unlikely(!__pyx_t_5)) __PYX_ERR(37, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 32, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_calc_stoch); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(36, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(37, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_period, __pyx_n_s_int) < 0) __PYX_ERR(37, 32, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_fastn, __pyx_n_s_int) < 0) __PYX_ERR(37, 32, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_slown, __pyx_n_s_int) < 0) __PYX_ERR(37, 32, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_213STOCH, 0, __pyx_n_s_STOCH, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__211)); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 32, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_period, __pyx_n_s_int) < 0) __PYX_ERR(36, 32, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_fastn, __pyx_n_s_int) < 0) __PYX_ERR(36, 32, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_slown, __pyx_n_s_int) < 0) __PYX_ERR(36, 32, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_209STOCH, 0, __pyx_n_s_STOCH, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__207)); if (unlikely(!__pyx_t_7)) __PYX_ERR(36, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_7, sizeof(__pyx_defaults36), 3)) __PYX_ERR(37, 32, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_7, sizeof(__pyx_defaults35), 3)) __PYX_ERR(36, 32, __pyx_L1_error)
 
   /* "src/mintalib/cython/stoch.pxi":33
  * 
  * @wrap_function(calc_stoch)
  * def STOCH(prices, period: int = 14, fastn: int = 3, slown: int = 3):             # <<<<<<<<<<<<<<
  *     result = calc_stoch(prices, period=period, fastn=fastn, slown=slown)
  *     return wrap_result(result, prices)
  */
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_14)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_14))) __PYX_ERR(37, 33, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_14)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_14))) __PYX_ERR(36, 33, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_14);
-  __Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_t_7)->__pyx_arg_period = ((PyObject*)__pyx_int_14);
+  __Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_t_7)->__pyx_arg_period = ((PyObject*)__pyx_int_14);
   __Pyx_GIVEREF(__pyx_int_14);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_3))) __PYX_ERR(37, 33, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_3))) __PYX_ERR(36, 33, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_3);
-  __Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_t_7)->__pyx_arg_fastn = ((PyObject*)__pyx_int_3);
+  __Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_t_7)->__pyx_arg_fastn = ((PyObject*)__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_3))) __PYX_ERR(37, 33, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_3))) __PYX_ERR(36, 33, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_3);
-  __Pyx_CyFunction_Defaults(__pyx_defaults36, __pyx_t_7)->__pyx_arg_slown = ((PyObject*)__pyx_int_3);
+  __Pyx_CyFunction_Defaults(__pyx_defaults35, __pyx_t_7)->__pyx_arg_slown = ((PyObject*)__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_301__defaults__);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_8mintalib_4core_295__defaults__);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_10);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/stoch.pxi":32
  * 
  * 
  * @wrap_function(calc_stoch)             # <<<<<<<<<<<<<<
  * def STOCH(prices, period: int = 14, fastn: int = 3, slown: int = 3):
  *     result = calc_stoch(prices, period=period, fastn=fastn, slown=slown)
  */
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(37, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(36, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_STOCH, __pyx_t_5) < 0) __PYX_ERR(37, 32, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_STOCH, __pyx_t_10) < 0) __PYX_ERR(36, 32, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/streak.pxi":3
  * """ Streak """
  * 
  * def streak_up(series, *, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Consecutive streak of ups """
  * 
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(38, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_wrap, ((PyObject *)Py_False)) < 0) __PYX_ERR(38, 3, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(38, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_wrap, __pyx_n_s_bool) < 0) __PYX_ERR(38, 3, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_215streak_up, 0, __pyx_n_s_streak_up, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__213)); if (unlikely(!__pyx_t_10)) __PYX_ERR(38, 3, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_10, __pyx_t_5);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_10, __pyx_t_7);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_streak_up, __pyx_t_10) < 0) __PYX_ERR(38, 3, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_wrap, ((PyObject *)Py_False)) < 0) __PYX_ERR(37, 3, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_wrap, __pyx_n_s_bool) < 0) __PYX_ERR(37, 3, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_211streak_up, 0, __pyx_n_s_streak_up, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__209)); if (unlikely(!__pyx_t_11)) __PYX_ERR(37, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_11, __pyx_t_10);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_11, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_streak_up, __pyx_t_11) < 0) __PYX_ERR(37, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
   /* "src/mintalib/cython/streak.pxi":38
  * 
  * 
  * def streak_down(series, *, wrap: bool = False):             # <<<<<<<<<<<<<<
  *     """ Consecutive streak of downs """
  * 
  */
-  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(38, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_wrap, ((PyObject *)Py_False)) < 0) __PYX_ERR(38, 38, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(38, 38, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(37, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_wrap, ((PyObject *)Py_False)) < 0) __PYX_ERR(37, 38, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_wrap, __pyx_n_s_bool) < 0) __PYX_ERR(38, 38, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_217streak_down, 0, __pyx_n_s_streak_down, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__214)); if (unlikely(!__pyx_t_5)) __PYX_ERR(38, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_5, __pyx_t_10);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_7);
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_wrap, __pyx_n_s_bool) < 0) __PYX_ERR(37, 38, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_213streak_down, 0, __pyx_n_s_streak_down, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__210)); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_10, __pyx_t_11);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_10, __pyx_t_7);
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_streak_down, __pyx_t_5) < 0) __PYX_ERR(38, 38, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_streak_down, __pyx_t_10) < 0) __PYX_ERR(37, 38, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/streak.pxi":72
  * 
  * 
  * @wrap_function(streak_up)             # <<<<<<<<<<<<<<
  * def STREAK_UP(series, *, item: str = None):
  *     series = get_series(series, item=item)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_wrap_function); if (unlikely(!__pyx_t_5)) __PYX_ERR(38, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_streak_up); if (unlikely(!__pyx_t_7)) __PYX_ERR(38, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(38, 72, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_wrap_function); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_streak_up); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(37, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(38, 72, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
 
   /* "src/mintalib/cython/streak.pxi":73
  * 
  * @wrap_function(streak_up)
  * def STREAK_UP(series, *, item: str = None):             # <<<<<<<<<<<<<<
  *     series = get_series(series, item=item)
  *     result = streak_up(series)
  */
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_item, Py_None) < 0) __PYX_ERR(38, 72, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_item, Py_None) < 0) __PYX_ERR(37, 72, __pyx_L1_error)
 
   /* "src/mintalib/cython/streak.pxi":72
  * 
  * 
  * @wrap_function(streak_up)             # <<<<<<<<<<<<<<
  * def STREAK_UP(series, *, item: str = None):
  *     series = get_series(series, item=item)
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(38, 72, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_item, __pyx_n_s_str) < 0) __PYX_ERR(37, 72, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_215STREAK_UP, 0, __pyx_n_s_STREAK_UP, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__211)); if (unlikely(!__pyx_t_5)) __PYX_ERR(37, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_item, __pyx_n_s_str) < 0) __PYX_ERR(38, 72, __pyx_L1_error)
-  __pyx_t_11 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_219STREAK_UP, 0, __pyx_n_s_STREAK_UP, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__215)); if (unlikely(!__pyx_t_11)) __PYX_ERR(38, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_11, __pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_11, __pyx_t_5);
+  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_5, __pyx_t_7);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(38, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_STREAK_UP, __pyx_t_5) < 0) __PYX_ERR(38, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_STREAK_UP, __pyx_t_10) < 0) __PYX_ERR(37, 72, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/streak.pxi":79
  * 
  * 
  * @wrap_function(streak_down)             # <<<<<<<<<<<<<<
  * def STREAK_DOWN(series, *, item: str = None):
  *     series = get_series(series, item=item)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_wrap_function); if (unlikely(!__pyx_t_5)) __PYX_ERR(38, 79, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_wrap_function); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_streak_down); if (unlikely(!__pyx_t_5)) __PYX_ERR(37, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_streak_down); if (unlikely(!__pyx_t_11)) __PYX_ERR(38, 79, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(37, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(38, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(38, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(37, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
 
   /* "src/mintalib/cython/streak.pxi":80
  * 
  * @wrap_function(streak_down)
  * def STREAK_DOWN(series, *, item: str = None):             # <<<<<<<<<<<<<<
  *     series = get_series(series, item=item)
  *     result = streak_down(series)
  */
-  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_item, Py_None) < 0) __PYX_ERR(38, 79, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_item, Py_None) < 0) __PYX_ERR(37, 79, __pyx_L1_error)
 
   /* "src/mintalib/cython/streak.pxi":79
  * 
  * 
  * @wrap_function(streak_down)             # <<<<<<<<<<<<<<
  * def STREAK_DOWN(series, *, item: str = None):
  *     series = get_series(series, item=item)
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(38, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_item, __pyx_n_s_str) < 0) __PYX_ERR(38, 79, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_221STREAK_DOWN, 0, __pyx_n_s_STREAK_DOWN, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__216)); if (unlikely(!__pyx_t_7)) __PYX_ERR(38, 79, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_item, __pyx_n_s_str) < 0) __PYX_ERR(37, 79, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_217STREAK_DOWN, 0, __pyx_n_s_STREAK_DOWN, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__212)); if (unlikely(!__pyx_t_7)) __PYX_ERR(37, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_7, __pyx_t_11);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
-  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_7, __pyx_t_5);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(38, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(37, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_STREAK_DOWN, __pyx_t_5) < 0) __PYX_ERR(38, 79, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_STREAK_DOWN, __pyx_t_10) < 0) __PYX_ERR(37, 79, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "src/mintalib/cython/eval.pxi":3
  * """ Expression eval """
  * 
  * def calc_eval(prices, expr: str):             # <<<<<<<<<<<<<<
  *     """
  *     Expression Eval (pandas only)
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(39, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_expr, __pyx_n_s_str) < 0) __PYX_ERR(39, 3, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_223calc_eval, 0, __pyx_n_s_calc_eval, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__218)); if (unlikely(!__pyx_t_7)) __PYX_ERR(39, 3, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(38, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_expr, __pyx_n_s_str) < 0) __PYX_ERR(38, 3, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_219calc_eval, 0, __pyx_n_s_calc_eval, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__214)); if (unlikely(!__pyx_t_7)) __PYX_ERR(38, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_eval, __pyx_t_7) < 0) __PYX_ERR(39, 3, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_10);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_eval, __pyx_t_7) < 0) __PYX_ERR(38, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "src/mintalib/cython/eval.pxi":14
  * 
  * 
  * @wrap_function(calc_eval)             # <<<<<<<<<<<<<<
  * def EVAL(prices, expr: str):
  *     result = calc_eval(prices, expr=expr)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_wrap_function); if (unlikely(!__pyx_t_7)) __PYX_ERR(39, 14, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_wrap_function); if (unlikely(!__pyx_t_7)) __PYX_ERR(38, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_calc_eval); if (unlikely(!__pyx_t_5)) __PYX_ERR(39, 14, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(39, 14, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_calc_eval); if (unlikely(!__pyx_t_10)) __PYX_ERR(38, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(38, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(39, 14, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_expr, __pyx_n_s_str) < 0) __PYX_ERR(39, 14, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_225EVAL, 0, __pyx_n_s_EVAL, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__220)); if (unlikely(!__pyx_t_7)) __PYX_ERR(39, 14, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(38, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_expr, __pyx_n_s_str) < 0) __PYX_ERR(38, 14, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_8mintalib_4core_221EVAL, 0, __pyx_n_s_EVAL, NULL, __pyx_n_s_mintalib_core, __pyx_d, ((PyObject *)__pyx_codeobj__216)); if (unlikely(!__pyx_t_7)) __PYX_ERR(38, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_5);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(39, 14, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_10);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(38, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_EVAL, __pyx_t_5) < 0) __PYX_ERR(39, 14, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_EVAL, __pyx_t_10) < 0) __PYX_ERR(38, 14, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "mintalib/core.pyx":6
  * 
  * __all__ = tuple(
  *     k for k, v in globals().items()             # <<<<<<<<<<<<<<
  *         if k.islower() and callable(v)
  *         and v.__module__.endswith(".core")
  */
-  __pyx_t_5 = __Pyx_Globals(); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __pyx_pf_8mintalib_4core_226genexpr(NULL, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 6, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_Globals(); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_7 = __pyx_pf_8mintalib_4core_222genexpr(NULL, __pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "mintalib/core.pyx":5
  * include "cython/_all_core.pxi"
  * 
  * __all__ = tuple(             # <<<<<<<<<<<<<<
  *     k for k, v in globals().items()
  *         if k.islower() and callable(v)
  */
-  __pyx_t_5 = __Pyx_PySequence_Tuple(__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_10 = __Pyx_PySequence_Tuple(__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all_2, __pyx_t_5) < 0) __PYX_ERR(2, 5, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all_2, __pyx_t_10) < 0) __PYX_ERR(2, 5, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "mintalib/core.pyx":1
  * # cython: language_level=3, binding=True             # <<<<<<<<<<<<<<
  * 
  * include "cython/_all_core.pxi"
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_5) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_10) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
@@ -81220,17 +78928,18 @@
 #endif
     }
     return result;
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
+    PyObject* exc_type;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
+    exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
         if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
         __Pyx_PyErr_Clear();
         return 0;
     }
     return 0;
@@ -82148,19 +79857,19 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
 CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
@@ -82265,15 +79974,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -82284,15 +79993,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -82316,15 +80025,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -83876,17 +81585,18 @@
 #endif
     return PyObject_SetAttr(obj, attr_name, value);
 }
 #endif
 
 /* UnpackUnboundCMethod */
 static PyObject *__Pyx_SelflessCall(PyObject *method, PyObject *args, PyObject *kwargs) {
+    PyObject *result;
     PyObject *selfless_args = PyTuple_GetSlice(args, 1, PyTuple_Size(args));
     if (unlikely(!selfless_args)) return NULL;
-    PyObject *result = PyObject_Call(method, selfless_args, kwargs);
+    result = PyObject_Call(method, selfless_args, kwargs);
     Py_DECREF(selfless_args);
     return result;
 }
 static PyMethodDef __Pyx_UnboundCMethod_Def = {
      "CythonUnboundCMethod",
      __PYX_REINTERPRET_FUNCION(PyCFunction, __Pyx_SelflessCall),
      METH_VARARGS | METH_KEYWORDS,
@@ -85132,15 +82842,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -86991,15 +84701,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -89177,15 +86887,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__221);
+        name = __Pyx_NewRef(__pyx_n_s__217);
     }
     return name;
 }
 #endif
 
 /* PyObjectCallMethod1 */
   #if !(CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2)
```

### Comparing `mintalib-0.0.7/src/mintalib/cython/_all_core.pxi` & `mintalib-0.0.8/src/mintalib/cython/_all_core.pxi`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
 include "kama.pxi"
 
 include "macd.pxi"
 include "ppo.pxi"
 
 include "slope.pxi"
-include "curve.pxi"
 
 include "stoch.pxi"
 
 include "streak.pxi"
 
 include "eval.pxi"
```

### Comparing `mintalib-0.0.7/src/mintalib/cython/_common.pxi` & `mintalib-0.0.8/src/mintalib/cython/_common.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/adx.pxi` & `mintalib-0.0.8/src/mintalib/cython/adx.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/atr.pxi` & `mintalib-0.0.8/src/mintalib/cython/atr.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/bbands.pxi` & `mintalib-0.0.8/src/mintalib/cython/bbands.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/bop.pxi` & `mintalib-0.0.8/src/mintalib/cython/bop.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/cci.pxi` & `mintalib-0.0.8/src/mintalib/cython/cci.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/cmf.pxi` & `mintalib-0.0.8/src/mintalib/cython/cmf.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/cross.pxi` & `mintalib-0.0.8/src/mintalib/cython/cross.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/dema.pxi` & `mintalib-0.0.8/src/mintalib/cython/dema.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/diff.pxi` & `mintalib-0.0.8/src/mintalib/cython/diff.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/ema.pxi` & `mintalib-0.0.8/src/mintalib/cython/ema.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/flags.pxi` & `mintalib-0.0.8/src/mintalib/cython/flags.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/kama.pxi` & `mintalib-0.0.8/src/mintalib/cython/kama.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/keltner.pxi` & `mintalib-0.0.8/src/mintalib/cython/keltner.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/macd.pxi` & `mintalib-0.0.8/src/mintalib/cython/macd.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/mad.pxi` & `mintalib-0.0.8/src/mintalib/cython/mad.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/matype.pxi` & `mintalib-0.0.8/src/mintalib/cython/matype.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/max.pxi` & `mintalib-0.0.8/src/mintalib/cython/max.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/mfi.pxi` & `mintalib-0.0.8/src/mintalib/cython/mfi.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/min.pxi` & `mintalib-0.0.8/src/mintalib/cython/min.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/ppo.pxi` & `mintalib-0.0.8/src/mintalib/cython/ppo.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/price.pxi` & `mintalib-0.0.8/src/mintalib/cython/price.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/rma.pxi` & `mintalib-0.0.8/src/mintalib/cython/rma.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/roc.pxi` & `mintalib-0.0.8/src/mintalib/cython/roc.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/rsi.pxi` & `mintalib-0.0.8/src/mintalib/cython/rsi.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/sar.pxi` & `mintalib-0.0.8/src/mintalib/cython/sar.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/slope.pxi` & `mintalib-0.0.8/src/mintalib/cython/slope.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/sma.pxi` & `mintalib-0.0.8/src/mintalib/cython/sma.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/stdev.pxi` & `mintalib-0.0.8/src/mintalib/cython/stdev.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/stoch.pxi` & `mintalib-0.0.8/src/mintalib/cython/stoch.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/streak.pxi` & `mintalib-0.0.8/src/mintalib/cython/streak.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/sum.pxi` & `mintalib-0.0.8/src/mintalib/cython/sum.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/tema.pxi` & `mintalib-0.0.8/src/mintalib/cython/tema.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/cython/wma.pxi` & `mintalib-0.0.8/src/mintalib/cython/wma.pxi`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/functions.py` & `mintalib-0.0.8/src/mintalib/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     EFFICIENCY_RATIO,
     KAMA,
     MACD,
     PPO,
     SLOPE,
     RVALUE,
     FORECAST,
-    CURVE,
     STOCH,
     STREAK_UP,
     STREAK_DOWN,
-    EVAL,
+    EVAL
 )
 
-__all__ = tuple(name for name in dir() if name.isupper())
+__all__ = tuple(name for name in dir() if name.isupper())
```

### Comparing `mintalib-0.0.7/src/mintalib/helper.py` & `mintalib-0.0.8/src/mintalib/helper.py`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/indicators.py` & `mintalib-0.0.8/src/mintalib/indicators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Do not edit! This file was generated by make-indicators.ipynb
 
 from . import core
 from . import model
 
-nan = float("nan")
-
+nan = float('nan')
 
 @core.wrap_function(core.AVGPRICE)
 class AVGPRICE(model.Indicator):
     def __call__(self, prices):
         return core.AVGPRICE(prices)
 
 
@@ -63,71 +62,50 @@
 class FLAG_ABOVE(model.Indicator):
     def __init__(self, level: float = 0.0, *, na_value: float = nan, item: str = None):
         self.level = level
         self.na_value = na_value
         self.item = item
 
     def __call__(self, series):
-        return core.FLAG_ABOVE(
-            series, level=self.level, na_value=self.na_value, item=self.item
-        )
+        return core.FLAG_ABOVE(series, level=self.level, na_value=self.na_value, item=self.item)
 
 
 @core.wrap_function(core.FLAG_BELOW)
 class FLAG_BELOW(model.Indicator):
     def __init__(self, level: float = 0.0, *, na_value: float = nan, item: str = None):
         self.level = level
         self.na_value = na_value
         self.item = item
 
     def __call__(self, series):
-        return core.FLAG_BELOW(
-            series, level=self.level, na_value=self.na_value, item=self.item
-        )
+        return core.FLAG_BELOW(series, level=self.level, na_value=self.na_value, item=self.item)
 
 
 @core.wrap_function(core.INVERT_FLAG)
 class INVERT_FLAG(model.Indicator):
     def __init__(self, *, na_value: float = nan, item: str = None):
         self.na_value = na_value
         self.item = item
 
     def __call__(self, series):
         return core.INVERT_FLAG(series, na_value=self.na_value, item=self.item)
 
 
 @core.wrap_function(core.UPDOWN_FLAG)
 class UPDOWN_FLAG(model.Indicator):
-    def __init__(
-        self,
-        up_level: float = 0.0,
-        down_level: float = 0.0,
-        *,
-        up_flag: float = 1.0,
-        down_flag: float = 0.0,
-        start_flag: float = nan,
-        item: str = None,
-    ):
+    def __init__(self, up_level: float = 0.0, down_level: float = 0.0, *, up_flag: float = 1.0, down_flag: float = 0.0, start_flag: float = nan, item: str = None):
         self.up_level = up_level
         self.down_level = down_level
         self.up_flag = up_flag
         self.down_flag = down_flag
         self.start_flag = start_flag
         self.item = item
 
     def __call__(self, series):
-        return core.UPDOWN_FLAG(
-            series,
-            up_level=self.up_level,
-            down_level=self.down_level,
-            up_flag=self.up_flag,
-            down_flag=self.down_flag,
-            start_flag=self.start_flag,
-            item=self.item,
-        )
+        return core.UPDOWN_FLAG(series, up_level=self.up_level, down_level=self.down_level, up_flag=self.up_flag, down_flag=self.down_flag, start_flag=self.start_flag, item=self.item)
 
 
 @core.wrap_function(core.LOG)
 class LOG(model.Indicator):
     def __init__(self, *, item: str = None):
         self.item = item
 
@@ -434,30 +412,22 @@
 
     def __call__(self, series):
         return core.EFFICIENCY_RATIO(series, period=self.period, item=self.item)
 
 
 @core.wrap_function(core.KAMA)
 class KAMA(model.Indicator):
-    def __init__(
-        self, period: int = 10, fastn: int = 2, slown: int = 30, *, item: str = None
-    ):
+    def __init__(self, period: int = 10, fastn: int = 2, slown: int = 30, *, item: str = None):
         self.period = period
         self.fastn = fastn
         self.slown = slown
         self.item = item
 
     def __call__(self, series):
-        return core.KAMA(
-            series,
-            period=self.period,
-            fastn=self.fastn,
-            slown=self.slown,
-            item=self.item,
-        )
+        return core.KAMA(series, period=self.period, fastn=self.fastn, slown=self.slown, item=self.item)
 
 
 @core.wrap_function(core.MACD)
 class MACD(model.Indicator):
     def __init__(self, n1: int = 12, n2: int = 26, n3: int = 9, *, item: str = None):
         self.n1 = n1
         self.n2 = n2
@@ -504,40 +474,26 @@
 class FORECAST(model.Indicator):
     def __init__(self, period: int = 20, offset: int = 0, *, item: str = None):
         self.period = period
         self.offset = offset
         self.item = item
 
     def __call__(self, series):
-        return core.FORECAST(
-            series, period=self.period, offset=self.offset, item=self.item
-        )
-
-
-@core.wrap_function(core.CURVE)
-class CURVE(model.Indicator):
-    def __init__(self, period: int = 20, *, item: str = None):
-        self.period = period
-        self.item = item
-
-    def __call__(self, series):
-        return core.CURVE(series, period=self.period, item=self.item)
+        return core.FORECAST(series, period=self.period, offset=self.offset, item=self.item)
 
 
 @core.wrap_function(core.STOCH)
 class STOCH(model.Indicator):
     def __init__(self, period: int = 14, fastn: int = 3, slown: int = 3):
         self.period = period
         self.fastn = fastn
         self.slown = slown
 
     def __call__(self, prices):
-        return core.STOCH(
-            prices, period=self.period, fastn=self.fastn, slown=self.slown
-        )
+        return core.STOCH(prices, period=self.period, fastn=self.fastn, slown=self.slown)
 
 
 @core.wrap_function(core.STREAK_UP)
 class STREAK_UP(model.Indicator):
     def __init__(self, *, item: str = None):
         self.item = item
```

### Comparing `mintalib-0.0.7/src/mintalib/model.py` & `mintalib-0.0.8/src/mintalib/model.py`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/reflib.py` & `mintalib-0.0.8/src/mintalib/reflib.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,18 +117,7 @@
             return np.nan
 
         return np.polyfit(xx, xs, 1)[0]
 
     return series.rolling(period).apply(func, raw=True)
 
 
-def calc_curve(series, period: int = 20):
-    """Curve (time curvilinear regression)"""
-    xx = np.arange(period) - (period - 1.0) / 2.0
-
-    def func(xs):
-        if np.any(np.isnan(xs)):
-            return np.nan
-
-        return np.polyfit(xx, xs, 2)[0]
-
-    return series.rolling(period).apply(func, raw=True)
```

### Comparing `mintalib-0.0.7/src/mintalib/samples/__init__.py` & `mintalib-0.0.8/src/mintalib/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/samples/sample-prices.csv` & `mintalib-0.0.8/src/mintalib/samples/sample-prices.csv`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib/utils.py` & `mintalib-0.0.8/src/mintalib/utils.py`

 * *Files identical despite different names*

### Comparing `mintalib-0.0.7/src/mintalib.egg-info/PKG-INFO` & `mintalib-0.0.8/src/mintalib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mintalib
-Version: 0.0.7
+Version: 0.0.8
 Summary: Minimal Technical Analysis Library for Python
 Author-email: Furechan <furechan@xsmail.com>
-License: MIT
+License: MIT License
 Project-URL: homepage, https://github.com/furechan/mintalib
 Keywords: python,cython,finance,technical-analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -26,17 +26,17 @@
 This library offers a curated list of technical analysis indicators
 implemented in cython.
 It is built around `numpy` arrays and aims to be compatible
 with both `pandas` and `polars` dataframes where possible.
 
 
 > **Warning**
-> This is work in progress.
-> For a similar project with a mature api
-> you may want to look at [ta-lib](https://pypi.org/project/TA-Lib/).
+> This project is experimental and the interface can change.
+> For a similar project with a mature api you may want to look at
+> [ta-lib](https://pypi.org/project/TA-Lib/).
 
 
 ## Structure
 The `mintalib` package contains three main modules:
 - `mintalib.core` low level calculation rountines implemented in cython
 - `mintalib.functions` single use functions to compute indicators
 - `mintalib.indicators` composable interface to indicators
@@ -149,15 +149,14 @@
 | AVGPRICE         | Average Price                             |
 | BBANDS           | Bollinger Bands                           |
 | BOP              | Balance of Power                          |
 | CCI              | Commodity Channel Index                   |
 | CMF              | Chaikin Money Flow                        |
 | CROSSOVER        | Cross Over                                |
 | CROSSUNDER       | Cross Under                               |
-| CURVE            | Curve (time curvilinear regression)       |
 | DEMA             | Double Exponential Moving Average         |
 | DIFF             | Difference                                |
 | EFFICIENCY_RATIO | Efficiency Ratio (Kaufman)                |
 | EMA              | Exponential Moving Average                |
 | EVAL             | Expression Eval (pandas only)             |
 | EXP              | Exponential                               |
 | FLAG_ABOVE       | Flag for value above level                |
```

### Comparing `mintalib-0.0.7/src/mintalib.egg-info/SOURCES.txt` & `mintalib-0.0.8/src/mintalib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 src/mintalib/cython/adx.pxi
 src/mintalib/cython/atr.pxi
 src/mintalib/cython/bbands.pxi
 src/mintalib/cython/bop.pxi
 src/mintalib/cython/cci.pxi
 src/mintalib/cython/cmf.pxi
 src/mintalib/cython/cross.pxi
-src/mintalib/cython/curve.pxi
 src/mintalib/cython/dema.pxi
 src/mintalib/cython/diff.pxi
 src/mintalib/cython/ema.pxi
 src/mintalib/cython/eval.pxi
 src/mintalib/cython/exp.pxi
 src/mintalib/cython/flags.pxi
 src/mintalib/cython/kama.pxi
```

### Comparing `mintalib-0.0.7/tests/test_mintalib.py` & `mintalib-0.0.8/tests/test_mintalib.py`

 * *Files identical despite different names*

