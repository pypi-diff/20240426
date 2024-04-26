# Comparing `tmp/megaradrp-0.9.2.tar.gz` & `tmp/megaradrp-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/megaradrp-0.9.2.tar", last modified: Tue Jul 30 16:50:50 2019, max compression
+gzip compressed data, was "dist/megaradrp-0.9.3.tar", last modified: Mon Jan 27 15:12:36 2020, max compression
```

## Comparing `megaradrp-0.9.2.tar` & `megaradrp-0.9.3.tar`

### file list

```diff
@@ -1,392 +1,223 @@
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/
--rw-rw-r--   0 spr       (1000) spr       (1000)      195 2019-06-28 12:44:28.000000 megaradrp-0.9.2/AUTHORS.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)    35147 2015-06-01 09:40:05.000000 megaradrp-0.9.2/LICENSE.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      133 2016-02-08 15:00:45.000000 megaradrp-0.9.2/MANIFEST.in
--rw-rw-r--   0 spr       (1000) spr       (1000)     2555 2019-07-30 16:50:50.000000 megaradrp-0.9.2/PKG-INFO
--rw-rw-r--   0 spr       (1000) spr       (1000)     1422 2019-07-30 16:46:10.000000 megaradrp-0.9.2/README.rst
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/
--rw-rw-r--   0 spr       (1000) spr       (1000)     5572 2015-06-01 09:40:05.000000 megaradrp-0.9.2/doc/Makefile
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/
--rw-rw-r--   0 spr       (1000) spr       (1000)      230 2017-01-13 17:09:21.000000 megaradrp-0.9.2/doc/_build/.buildinfo
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/.doctrees/
--rw-rw-r--   0 spr       (1000) spr       (1000)   201465 2017-01-13 17:09:18.000000 megaradrp-0.9.2/doc/_build/.doctrees/auxiliary.doctree
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/
--rw-rw-r--   0 spr       (1000) spr       (1000)    76734 2017-01-13 17:09:18.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/arc.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    40849 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/bias.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    66394 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/bpm.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    35021 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/dark.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    63455 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/fiberflat.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    11637 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/index.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    35987 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/linearity.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    51193 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/slitflat.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    66137 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/trace.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    79131 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/calibration/twilight.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)   174072 2017-01-13 17:09:20.000000 megaradrp-0.9.2/doc/_build/.doctrees/environment.pickle
--rw-rw-r--   0 spr       (1000) spr       (1000)     5918 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/glossary.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    95715 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/images.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     5650 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/index.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    41209 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/installation.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     4851 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/intro.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    26502 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/keywords.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     4658 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/modes.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     6035 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/products.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     4003 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/rawimages.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    10155 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/recipes.doctree
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/.doctrees/reference/
--rw-rw-r--   0 spr       (1000) spr       (1000)   130172 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/reference/core.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     8522 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/reference/index.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    13566 2017-01-13 17:09:19.000000 megaradrp-0.9.2/doc/_build/.doctrees/reference/instrument.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    31651 2017-01-13 17:09:20.000000 megaradrp-0.9.2/doc/_build/.doctrees/reference/products.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     3327 2017-01-13 17:09:20.000000 megaradrp-0.9.2/doc/_build/.doctrees/reference/recipes.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     3310 2017-01-13 17:09:20.000000 megaradrp-0.9.2/doc/_build/.doctrees/reference/simulation.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    41213 2017-01-13 17:09:20.000000 megaradrp-0.9.2/doc/_build/.doctrees/running.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)   311300 2017-01-13 17:09:20.000000 megaradrp-0.9.2/doc/_build/.doctrees/scientific.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     6230 2017-01-13 17:09:20.000000 megaradrp-0.9.2/doc/_build/.doctrees/testing.doctree
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/doctrees/
--rw-rw-r--   0 spr       (1000) spr       (1000)   209570 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/doctrees/auxiliary.doctree
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/
--rw-rw-r--   0 spr       (1000) spr       (1000)    68349 2017-01-15 11:12:48.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/arc.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    36199 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/bias.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    56283 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/bpm.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    29019 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/dark.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    55860 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/fiberflat.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    10653 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/index.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    31453 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/linearity.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    38208 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/slitflat.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    58553 2017-01-13 19:46:33.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/trace.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    67509 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/calibration/twilight.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)   159993 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/doctrees/environment.pickle
--rw-rw-r--   0 spr       (1000) spr       (1000)     5198 2017-01-13 17:20:31.000000 megaradrp-0.9.2/doc/_build/doctrees/glossary.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    81216 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/images.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     5147 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/index.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    35998 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/installation.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     4521 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/intro.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    22029 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/keywords.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     4295 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/modes.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     5442 2017-01-13 18:35:13.000000 megaradrp-0.9.2/doc/_build/doctrees/products.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     3640 2017-01-13 17:20:31.000000 megaradrp-0.9.2/doc/_build/doctrees/rawimages.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     9544 2017-01-13 17:20:31.000000 megaradrp-0.9.2/doc/_build/doctrees/recipes.doctree
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/doctrees/reference/
--rw-rw-r--   0 spr       (1000) spr       (1000)   111963 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/doctrees/reference/core.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     7475 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/doctrees/reference/index.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    11713 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/doctrees/reference/instrument.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    26510 2017-01-15 11:12:48.000000 megaradrp-0.9.2/doc/_build/doctrees/reference/products.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     3029 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/doctrees/reference/recipes.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     3012 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/doctrees/reference/simulation.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)    36960 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/doctrees/running.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)   269864 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/doctrees/scientific.doctree
--rw-rw-r--   0 spr       (1000) spr       (1000)     5739 2017-01-13 17:20:31.000000 megaradrp-0.9.2/doc/_build/doctrees/testing.doctree
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/html/
--rw-rw-r--   0 spr       (1000) spr       (1000)      230 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/.buildinfo
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/html/_images/
--rw-rw-r--   0 spr       (1000) spr       (1000)    27159 2017-01-13 17:20:32.000000 megaradrp-0.9.2/doc/_build/html/_images/graphviz-bde0b982ba89f521e3db7bfadbae78ef8e0da5a2.png
--rw-rw-r--   0 spr       (1000) spr       (1000)       29 2017-01-13 17:20:32.000000 megaradrp-0.9.2/doc/_build/html/_images/graphviz-bde0b982ba89f521e3db7bfadbae78ef8e0da5a2.png.map
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/html/_sources/
--rw-rw-r--   0 spr       (1000) spr       (1000)    15033 2017-01-13 19:50:21.000000 megaradrp-0.9.2/doc/_build/html/_sources/auxiliary.txt
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/
--rw-rw-r--   0 spr       (1000) spr       (1000)     3157 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/arc.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     1807 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/bias.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     3868 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/bpm.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     2160 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/dark.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     2895 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/fiberflat.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     2437 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/index.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     3420 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/linearity.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     3464 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/slitflat.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     2779 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/trace.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     3413 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/calibration/twilight.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      332 2015-06-01 09:40:05.000000 megaradrp-0.9.2/doc/_build/html/_sources/glossary.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)    13795 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/images.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      775 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/index.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     6812 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/installation.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      726 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/intro.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     2324 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/keywords.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      549 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/modes.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      593 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/products.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      160 2015-06-01 09:40:05.000000 megaradrp-0.9.2/doc/_build/html/_sources/rawimages.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     2519 2016-07-19 22:31:45.000000 megaradrp-0.9.2/doc/_build/html/_sources/recipes.txt
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/html/_sources/reference/
--rw-rw-r--   0 spr       (1000) spr       (1000)      282 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/reference/core.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      495 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/reference/index.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      585 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/reference/instrument.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      834 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/reference/products.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      192 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/reference/recipes.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      175 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/reference/simulation.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     9629 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/running.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)    20042 2017-01-13 18:15:26.000000 megaradrp-0.9.2/doc/_build/html/_sources/scientific.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      879 2015-06-01 09:40:05.000000 megaradrp-0.9.2/doc/_build/html/_sources/testing.txt
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/html/_static/
--rw-rw-r--   0 spr       (1000) spr       (1000)      673 2016-09-01 04:34:03.000000 megaradrp-0.9.2/doc/_build/html/_static/ajax-loader.gif
--rw-rw-r--   0 spr       (1000) spr       (1000)     9740 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/_static/basic.css
--rw-rw-r--   0 spr       (1000) spr       (1000)     4146 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/_static/classic.css
--rw-rw-r--   0 spr       (1000) spr       (1000)     3500 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/comment-bright.png
--rw-rw-r--   0 spr       (1000) spr       (1000)     3578 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/comment-close.png
--rw-rw-r--   0 spr       (1000) spr       (1000)     3445 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/comment.png
--rw-rw-r--   0 spr       (1000) spr       (1000)       28 2016-09-21 01:46:46.000000 megaradrp-0.9.2/doc/_build/html/_static/default.css
--rw-rw-r--   0 spr       (1000) spr       (1000)     8166 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/_static/doctools.js
--rw-rw-r--   0 spr       (1000) spr       (1000)      347 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/down-pressed.png
--rw-rw-r--   0 spr       (1000) spr       (1000)      347 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/down.png
--rw-rw-r--   0 spr       (1000) spr       (1000)      358 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/file.png
--rw-rw-r--   0 spr       (1000) spr       (1000)   282766 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/jquery-1.11.1.js
--rw-rw-r--   0 spr       (1000) spr       (1000)    95786 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/jquery.js
--rw-rw-r--   0 spr       (1000) spr       (1000)      173 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/minus.png
--rw-rw-r--   0 spr       (1000) spr       (1000)      173 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/plus.png
--rw-rw-r--   0 spr       (1000) spr       (1000)     4149 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/_static/pygments.css
--rw-rw-r--   0 spr       (1000) spr       (1000)    18862 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/_static/searchtools.js
--rw-rw-r--   0 spr       (1000) spr       (1000)     4803 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/_static/sidebar.js
--rw-rw-r--   0 spr       (1000) spr       (1000)    35168 2016-09-21 01:46:46.000000 megaradrp-0.9.2/doc/_build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 spr       (1000) spr       (1000)    12140 2016-09-01 04:34:03.000000 megaradrp-0.9.2/doc/_build/html/_static/underscore.js
--rw-rw-r--   0 spr       (1000) spr       (1000)      345 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/up-pressed.png
--rw-rw-r--   0 spr       (1000) spr       (1000)      345 2016-10-01 15:14:37.000000 megaradrp-0.9.2/doc/_build/html/_static/up.png
--rw-rw-r--   0 spr       (1000) spr       (1000)    25351 2016-09-21 01:46:46.000000 megaradrp-0.9.2/doc/_build/html/_static/websupport.js
--rw-rw-r--   0 spr       (1000) spr       (1000)    54651 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/auxiliary.html
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/html/calibration/
--rw-rw-r--   0 spr       (1000) spr       (1000)    19625 2017-01-15 11:12:48.000000 megaradrp-0.9.2/doc/_build/html/calibration/arc.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    14250 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/html/calibration/bias.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    18941 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/html/calibration/bpm.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    12597 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/html/calibration/dark.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    17509 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/html/calibration/fiberflat.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     8562 2017-01-15 11:12:48.000000 megaradrp-0.9.2/doc/_build/html/calibration/index.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    13920 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/html/calibration/linearity.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    14754 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/html/calibration/slitflat.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    18099 2017-01-13 19:46:33.000000 megaradrp-0.9.2/doc/_build/html/calibration/trace.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    20207 2017-01-13 18:35:14.000000 megaradrp-0.9.2/doc/_build/html/calibration/twilight.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    42204 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/genindex.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     4966 2017-01-13 17:20:32.000000 megaradrp-0.9.2/doc/_build/html/glossary.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    35334 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/images.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    10079 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/index.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    19089 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/installation.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     5676 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/intro.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     9125 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/keywords.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     8337 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/modes.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     2233 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/objects.inv
--rw-rw-r--   0 spr       (1000) spr       (1000)     8628 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/products.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     5855 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/py-modindex.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     6483 2017-01-13 17:20:32.000000 megaradrp-0.9.2/doc/_build/html/rawimages.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    10120 2017-01-13 17:20:32.000000 megaradrp-0.9.2/doc/_build/html/recipes.html
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_build/html/reference/
--rw-rw-r--   0 spr       (1000) spr       (1000)    25578 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/reference/core.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     8114 2017-01-15 11:12:48.000000 megaradrp-0.9.2/doc/_build/html/reference/index.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     8695 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/reference/instrument.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    11120 2017-01-15 11:12:48.000000 megaradrp-0.9.2/doc/_build/html/reference/products.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     5881 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/reference/recipes.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     5624 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/reference/simulation.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    35890 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/running.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    69989 2017-01-13 18:35:15.000000 megaradrp-0.9.2/doc/_build/html/scientific.html
--rw-rw-r--   0 spr       (1000) spr       (1000)     4047 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/search.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    31905 2017-01-16 00:58:04.000000 megaradrp-0.9.2/doc/_build/html/searchindex.js
--rw-rw-r--   0 spr       (1000) spr       (1000)     7213 2017-01-13 17:20:32.000000 megaradrp-0.9.2/doc/_build/html/testing.html
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_static/
--rw-rw-r--   0 spr       (1000) spr       (1000)     3799 2015-06-01 09:40:05.000000 megaradrp-0.9.2/doc/_static/megara.png
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/_templates/
--rw-rw-r--   0 spr       (1000) spr       (1000)      112 2015-06-01 09:40:05.000000 megaradrp-0.9.2/doc/_templates/index.html
--rw-rw-r--   0 spr       (1000) spr       (1000)    14979 2018-05-02 23:13:32.000000 megaradrp-0.9.2/doc/auxiliary.rst
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/calibration/
--rw-rw-r--   0 spr       (1000) spr       (1000)     3128 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/arc.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     1800 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/bias.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     3873 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/bpm.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     2160 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/dark.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     2919 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/fiberflat.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     2466 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/index.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     5233 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/lcbstd.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     3424 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/linearity.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     1828 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/model.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     3120 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/mosstd.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     3471 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/slitflat.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     2777 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/trace.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     3419 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/calibration/twilight.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     1321 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/combined.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     1992 2019-07-30 16:46:10.000000 megaradrp-0.9.2/doc/conf.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      332 2015-06-01 09:40:05.000000 megaradrp-0.9.2/doc/glossary.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)    12366 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/images.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      857 2019-06-28 12:44:48.000000 megaradrp-0.9.2/doc/index.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     6729 2018-12-11 16:36:50.000000 megaradrp-0.9.2/doc/installation.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      726 2019-07-21 10:45:59.000000 megaradrp-0.9.2/doc/intro.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     3860 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/keywords.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      561 2019-07-21 10:45:59.000000 megaradrp-0.9.2/doc/modes.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      613 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/products.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      160 2015-06-01 09:40:05.000000 megaradrp-0.9.2/doc/rawimages.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     2519 2019-07-21 10:45:59.000000 megaradrp-0.9.2/doc/recipes.rst
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/doc/reference/
--rw-rw-r--   0 spr       (1000) spr       (1000)      282 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/core.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      255 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/datamodel.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      571 2018-05-02 23:13:48.000000 megaradrp-0.9.2/doc/reference/index.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      283 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/instrument.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      473 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/processing.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     1421 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/products.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      250 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/recipes.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     1606 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/simulation.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      235 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/types.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      226 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/utils.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      236 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/validators.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      315 2018-05-02 23:12:40.000000 megaradrp-0.9.2/doc/reference/visualization.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     9406 2019-07-21 10:45:59.000000 megaradrp-0.9.2/doc/running.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)     6661 2018-05-02 23:15:16.000000 megaradrp-0.9.2/doc/scientific.rst
--rw-rw-r--   0 spr       (1000) spr       (1000)      879 2015-06-01 09:40:05.000000 megaradrp-0.9.2/doc/testing.rst
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/
--rw-rw-r--   0 spr       (1000) spr       (1000)      340 2019-07-30 16:46:10.000000 megaradrp-0.9.2/megaradrp/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      202 2018-08-07 16:05:02.000000 megaradrp-0.9.2/megaradrp/conftest.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/core/
--rw-rw-r--   0 spr       (1000) spr       (1000)       95 2016-02-08 15:00:45.000000 megaradrp-0.9.2/megaradrp/core/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3500 2019-07-30 16:46:10.000000 megaradrp-0.9.2/megaradrp/core/correctors.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     4370 2019-07-30 16:46:10.000000 megaradrp-0.9.2/megaradrp/core/recipe.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/core/tests/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2016-02-08 15:00:45.000000 megaradrp-0.9.2/megaradrp/core/tests/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      257 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/core/tests/test_recipe.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    11499 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/datamodel.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/db/
--rw-rw-r--   0 spr       (1000) spr       (1000)      134 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/db/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1007 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/db/control.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      940 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/db/model.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     6480 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/drp.yaml
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/instrument/
--rw-rw-r--   0 spr       (1000) spr       (1000)     8963 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/__init__.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/instrument/components/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      268 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/calibrationunit.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     4947 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/cover.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     6374 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/detector.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     6145 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/fibermos.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    12133 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/instrument.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1718 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/lamps.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      966 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/psslit.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1575 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/shutter.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1655 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/telescope.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      249 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/components/wheel.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/instrument/configs/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/instrument/configs/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    35445 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/configs/component-06fc5d6d-d20b-4eba-b3fa-57696f0a1103.json
--rw-rw-r--   0 spr       (1000) spr       (1000)      647 2019-07-30 16:46:10.000000 megaradrp-0.9.2/megaradrp/instrument/configs/component-2e02e135-2325-47c9-9975-466b445b0b8b.json
--rw-rw-r--   0 spr       (1000) spr       (1000)     3275 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/configs/component-715c7ced-f989-42a6-bb74-a5b5cda0495c.json
--rw-rw-r--   0 spr       (1000) spr       (1000)      383 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/configs/component-78f6d437-85d6-4d7a-bdb7-1e043368b442.json
--rw-rw-r--   0 spr       (1000) spr       (1000)    11537 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/configs/component-97d48545-3258-473e-9311-00e390999d52.json
--rw-rw-r--   0 spr       (1000) spr       (1000)      363 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/configs/instrument-4fd05b24-2ed9-457b-b563-a3c618bb1d4c.json
--rw-rw-r--   0 spr       (1000) spr       (1000)      445 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/configs/instrument-66f2283e-3049-4d4b-8ef1-14d62fcb611d.json
--rw-rw-r--   0 spr       (1000) spr       (1000)      389 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/configs/instrument-9a86b2b2-3f7d-48ec-8f4f-3780ec967c90.json
--rw-rw-r--   0 spr       (1000) spr       (1000)      369 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/configs/instrument-ca3558e3-e50d-4bbc-86bd-da50a0998a48.json
--rw-rw-r--   0 spr       (1000) spr       (1000)   357120 2018-05-02 23:19:54.000000 megaradrp-0.9.2/megaradrp/instrument/configs/lcb_default_header.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)   417600 2018-05-02 23:19:54.000000 megaradrp-0.9.2/megaradrp/instrument/configs/mos_default_header.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)     2882 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/instrument/configs/primary.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)    22153 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/instrument/configs/properties-86a6e968-8d3d-456f-89f8-09ff0c7f7c57.json
--rw-rw-r--   0 spr       (1000) spr       (1000)      328 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/loader.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/processing/
--rw-rw-r--   0 spr       (1000) spr       (1000)      161 2016-02-08 15:00:45.000000 megaradrp-0.9.2/megaradrp/processing/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     6371 2018-05-02 23:19:54.000000 megaradrp-0.9.2/megaradrp/processing/aperture.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1733 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/processing/combine.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    12960 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/processing/extractobj.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2857 2018-05-02 23:19:54.000000 megaradrp-0.9.2/megaradrp/processing/fiberflat.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     4973 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/processing/fibermatch.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3383 2019-07-24 18:59:06.000000 megaradrp-0.9.2/megaradrp/processing/fluxcalib.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      987 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/processing/multirss.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      865 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/processing/slitflat.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/processing/tests/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2016-02-08 15:00:45.000000 megaradrp-0.9.2/megaradrp/processing/tests/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      586 2018-08-06 23:50:43.000000 megaradrp-0.9.2/megaradrp/processing/tests/test_aperture.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1144 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/processing/tests/test_extractobj.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2099 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/processing/tests/test_fibermatch.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1433 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/processing/tests/test_fluxcalib.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1091 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/processing/tests/test_multirss.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3657 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/processing/tests/test_processing.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1970 2019-07-21 10:45:14.000000 megaradrp-0.9.2/megaradrp/processing/tests/test_trimover.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1111 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/processing/tests/test_wcs.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    12055 2019-07-21 10:45:14.000000 megaradrp-0.9.2/megaradrp/processing/trimover.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1797 2018-05-02 23:19:54.000000 megaradrp-0.9.2/megaradrp/processing/twilight.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    12131 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/processing/wavecalibration.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1085 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/processing/wcs.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2920 2018-05-02 23:19:54.000000 megaradrp-0.9.2/megaradrp/processing/weights.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/products/
--rw-rw-r--   0 spr       (1000) spr       (1000)      190 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/products/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     7090 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/products/modelmap.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1190 2018-08-06 23:50:43.000000 megaradrp-0.9.2/megaradrp/products/structured.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3163 2019-07-30 16:46:10.000000 megaradrp-0.9.2/megaradrp/products/tracemap.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2709 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/products/traces.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2087 2019-07-02 16:35:55.000000 megaradrp-0.9.2/megaradrp/products/wavecalibration.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/recipes/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2016-02-08 15:00:45.000000 megaradrp-0.9.2/megaradrp/recipes/__init__.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/recipes/auxiliary/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2016-02-08 15:00:45.000000 megaradrp-0.9.2/megaradrp/recipes/auxiliary/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     6941 2019-07-24 19:03:00.000000 megaradrp-0.9.2/megaradrp/recipes/auxiliary/acquisitionlcb.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     7162 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/auxiliary/acquisitionmos.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    16506 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/auxiliary/focusspec.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     7977 2019-07-24 15:13:38.000000 megaradrp-0.9.2/megaradrp/recipes/auxiliary/focustel.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2016-02-08 15:00:45.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    30956 2019-07-30 16:46:10.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/arc.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1812 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/base.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2083 2019-07-30 16:46:10.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/bias.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     4173 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/bpm.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1233 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/dark.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     8680 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/flat.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     5984 2019-07-30 16:46:10.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/lcbstdstar.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    15867 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/modelmap.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     5070 2019-07-24 15:13:38.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/mosstdstar.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3825 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/slitflat.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/tests/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2016-02-08 15:00:45.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/tests/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      607 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_arc.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1976 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_bias.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3384 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_bpm.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     4066 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_bpm_common.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3000 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_bpm_corrector.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3055 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_dark.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      608 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_tracemap.py
--r--r--r--   0 spr       (1000) spr       (1000)    18760 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/trace.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     8491 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/calibration/twilight.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/recipes/combined/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/recipes/combined/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1362 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/combined/extinctionstar.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1473 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/combined/sensstar.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/recipes/scientific/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/recipes/scientific/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3993 2018-07-15 09:41:16.000000 megaradrp-0.9.2/megaradrp/recipes/scientific/base.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     4651 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/scientific/lcb.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2101 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/recipes/scientific/lcbfastmapping.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     4831 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/scientific/mos.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/recipes/tests/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2016-02-08 15:00:45.000000 megaradrp-0.9.2/megaradrp/recipes/tests/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1462 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/recipes/tests/test_calibration.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3707 2018-12-11 16:36:50.000000 megaradrp-0.9.2/megaradrp/requirements.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/simulation/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/simulation/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    25329 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/simulation/actions.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3415 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/simulation/control.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2285 2018-05-02 23:19:54.000000 megaradrp-0.9.2/megaradrp/simulation/convolution.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1610 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/simulation/efficiency.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1216 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/simulation/extended.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     8579 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/simulation/factory.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1078 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/simulation/fiberbundle.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1316 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/simulation/focalplane.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1851 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/simulation/lightfiber.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2766 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/simulation/refraction.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2584 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/simulation/vph.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1004 2018-05-02 23:19:54.000000 megaradrp-0.9.2/megaradrp/taggers.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/tests/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2016-02-08 15:00:45.000000 megaradrp-0.9.2/megaradrp/tests/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2066 2018-08-06 23:50:43.000000 megaradrp-0.9.2/megaradrp/tests/create.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      540 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/tests/simpleobj.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      783 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/tests/test_binning.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3488 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/tests/test_datamodel.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    10427 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/tests/test_drp.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      190 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/tests/test_loader.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2347 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/tests/test_taggers.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     2418 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/tests/test_types.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1852 2018-05-02 23:19:54.000000 megaradrp-0.9.2/megaradrp/tests/test_utils.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/tools/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2018-08-06 23:50:43.000000 megaradrp-0.9.2/megaradrp/tools/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    22980 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/tools/overplot_traces.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp/tools/tests/
--rw-rw-r--   0 spr       (1000) spr       (1000)        0 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/tools/tests/__init__.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      254 2019-06-28 12:44:28.000000 megaradrp-0.9.2/megaradrp/tools/tests/test_overplot_traces.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     3328 2019-07-30 16:46:10.000000 megaradrp-0.9.2/megaradrp/types.py
--rw-rw-r--   0 spr       (1000) spr       (1000)      882 2018-05-02 23:19:54.000000 megaradrp-0.9.2/megaradrp/utils.py
--rw-rw-r--   0 spr       (1000) spr       (1000)     1179 2018-05-02 23:12:40.000000 megaradrp-0.9.2/megaradrp/validators.py
--rw-rw-r--   0 spr       (1000) spr       (1000)    15840 2019-07-21 10:45:14.000000 megaradrp-0.9.2/megaradrp/visualization.py
-drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp.egg-info/
--rw-rw-r--   0 spr       (1000) spr       (1000)     2555 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp.egg-info/PKG-INFO
--rw-rw-r--   0 spr       (1000) spr       (1000)    12915 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp.egg-info/SOURCES.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)        1 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp.egg-info/dependency_links.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)      187 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp.egg-info/entry_points.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)        1 2017-10-06 12:10:53.000000 megaradrp-0.9.2/megaradrp.egg-info/not-zip-safe
--rw-rw-r--   0 spr       (1000) spr       (1000)      167 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp.egg-info/requires.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)       10 2019-07-30 16:50:50.000000 megaradrp-0.9.2/megaradrp.egg-info/top_level.txt
--rw-rw-r--   0 spr       (1000) spr       (1000)       92 2019-07-30 16:50:50.000000 megaradrp-0.9.2/setup.cfg
--rw-rw-r--   0 spr       (1000) spr       (1000)     1954 2019-07-30 16:46:10.000000 megaradrp-0.9.2/setup.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/
+-rw-rw-r--   0 spr       (1000) spr       (1000)      195 2020-01-27 15:11:25.000000 megaradrp-0.9.3/AUTHORS.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)    35147 2020-01-27 15:11:25.000000 megaradrp-0.9.3/LICENSE.txt
+-rw-rw-r--   0 spr       (1000) spr       (1000)      133 2020-01-27 15:11:25.000000 megaradrp-0.9.3/MANIFEST.in
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2555 2020-01-27 15:12:36.000000 megaradrp-0.9.3/PKG-INFO
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1422 2020-01-27 15:12:06.000000 megaradrp-0.9.3/README.rst
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/doc/
+-rw-rw-r--   0 spr       (1000) spr       (1000)     5572 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/Makefile
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/doc/_static/
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3799 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/_static/megara.png
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/doc/_templates/
+-rw-rw-r--   0 spr       (1000) spr       (1000)      112 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/_templates/index.html
+-rw-rw-r--   0 spr       (1000) spr       (1000)    14979 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/auxiliary.rst
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/doc/calibration/
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3128 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/arc.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1800 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/bias.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3873 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/bpm.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2160 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/dark.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2919 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/fiberflat.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2466 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/index.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     5233 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/lcbstd.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3424 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/linearity.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1828 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/model.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3120 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/mosstd.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3471 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/slitflat.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2777 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/trace.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3419 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/calibration/twilight.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1321 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/combined.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1992 2020-01-27 15:12:06.000000 megaradrp-0.9.3/doc/conf.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      332 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/glossary.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)    12366 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/images.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      857 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/index.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     6729 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/installation.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      516 2020-01-27 15:12:06.000000 megaradrp-0.9.3/doc/intro.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3860 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/keywords.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      408 2020-01-27 15:12:06.000000 megaradrp-0.9.3/doc/modes.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      613 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/products.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      160 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/rawimages.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2520 2020-01-27 15:12:06.000000 megaradrp-0.9.3/doc/recipes.rst
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/doc/reference/
+-rw-rw-r--   0 spr       (1000) spr       (1000)      282 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/core.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      255 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/datamodel.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      571 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/index.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      283 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/instrument.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      473 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/processing.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1421 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/products.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      250 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/recipes.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1606 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/simulation.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      235 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/types.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      226 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/utils.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      236 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/validators.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      315 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/reference/visualization.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     9407 2020-01-27 15:12:06.000000 megaradrp-0.9.3/doc/running.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)     6661 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/scientific.rst
+-rw-rw-r--   0 spr       (1000) spr       (1000)      879 2020-01-27 15:11:25.000000 megaradrp-0.9.3/doc/testing.rst
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/
+-rw-rw-r--   0 spr       (1000) spr       (1000)      340 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      202 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/conftest.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/core/
+-rw-rw-r--   0 spr       (1000) spr       (1000)       95 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/core/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3500 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/core/correctors.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     4370 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/core/recipe.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/core/tests/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/core/tests/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      257 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/core/tests/test_recipe.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    11499 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/datamodel.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/db/
+-rw-rw-r--   0 spr       (1000) spr       (1000)      134 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/db/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1007 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/db/control.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      940 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/db/model.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     6480 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/drp.yaml
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/instrument/
+-rw-rw-r--   0 spr       (1000) spr       (1000)     8963 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/__init__.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/instrument/components/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      268 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/calibrationunit.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     4947 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/cover.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     6374 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/detector.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     6145 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/fibermos.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    12133 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/instrument.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1718 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/lamps.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      966 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/psslit.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1575 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/shutter.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1655 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/telescope.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      249 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/components/wheel.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/instrument/configs/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    35445 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/component-06fc5d6d-d20b-4eba-b3fa-57696f0a1103.json
+-rw-rw-r--   0 spr       (1000) spr       (1000)      647 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/instrument/configs/component-2e02e135-2325-47c9-9975-466b445b0b8b.json
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3275 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/component-715c7ced-f989-42a6-bb74-a5b5cda0495c.json
+-rw-rw-r--   0 spr       (1000) spr       (1000)      383 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/component-78f6d437-85d6-4d7a-bdb7-1e043368b442.json
+-rw-rw-r--   0 spr       (1000) spr       (1000)    11537 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/component-97d48545-3258-473e-9311-00e390999d52.json
+-rw-rw-r--   0 spr       (1000) spr       (1000)      363 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/instrument-4fd05b24-2ed9-457b-b563-a3c618bb1d4c.json
+-rw-rw-r--   0 spr       (1000) spr       (1000)      445 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/instrument-66f2283e-3049-4d4b-8ef1-14d62fcb611d.json
+-rw-rw-r--   0 spr       (1000) spr       (1000)      389 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/instrument-9a86b2b2-3f7d-48ec-8f4f-3780ec967c90.json
+-rw-rw-r--   0 spr       (1000) spr       (1000)      369 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/instrument-ca3558e3-e50d-4bbc-86bd-da50a0998a48.json
+-rw-rw-r--   0 spr       (1000) spr       (1000)   357120 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/lcb_default_header.txt
+-rw-rw-r--   0 spr       (1000) spr       (1000)   417600 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/mos_default_header.txt
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2882 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/primary.txt
+-rw-rw-r--   0 spr       (1000) spr       (1000)    22153 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/instrument/configs/properties-86a6e968-8d3d-456f-89f8-09ff0c7f7c57.json
+-rw-rw-r--   0 spr       (1000) spr       (1000)      328 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/loader.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/processing/
+-rw-rw-r--   0 spr       (1000) spr       (1000)      161 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     6371 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/aperture.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1733 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/combine.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    12960 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/processing/extractobj.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2857 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/fiberflat.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     4973 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/processing/fibermatch.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3383 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/fluxcalib.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      987 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/multirss.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      865 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/slitflat.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/processing/tests/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/tests/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      586 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/tests/test_aperture.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1144 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/tests/test_extractobj.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2099 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/tests/test_fibermatch.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1433 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/tests/test_fluxcalib.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1091 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/tests/test_multirss.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3657 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/tests/test_processing.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1970 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/tests/test_trimover.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1111 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/tests/test_wcs.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    12055 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/trimover.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1797 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/twilight.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    12131 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/wavecalibration.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1085 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/wcs.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2920 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/processing/weights.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/products/
+-rw-rw-r--   0 spr       (1000) spr       (1000)      190 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/products/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     7090 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/products/modelmap.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1190 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/products/structured.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3163 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/products/tracemap.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2709 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/products/traces.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2087 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/products/wavecalibration.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/recipes/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/__init__.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/recipes/auxiliary/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/auxiliary/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     6941 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/auxiliary/acquisitionlcb.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     7162 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/auxiliary/acquisitionmos.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    16506 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/auxiliary/focusspec.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     7977 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/auxiliary/focustel.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    30956 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/arc.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1812 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/base.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2083 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/bias.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     4173 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/bpm.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1233 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/dark.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     8680 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/flat.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     5984 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/lcbstdstar.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    15567 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/modelmap.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     5070 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/mosstdstar.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3825 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/slitflat.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/tests/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/tests/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      607 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_arc.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1976 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_bias.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3384 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_bpm.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     4066 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_bpm_common.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3000 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_bpm_corrector.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3055 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_dark.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      608 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_tracemap.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    18760 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/trace.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     8491 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/calibration/twilight.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/recipes/combined/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/combined/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1362 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/combined/extinctionstar.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1473 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/combined/sensstar.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/recipes/scientific/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/scientific/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3993 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/recipes/scientific/base.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     4651 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/scientific/lcb.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2101 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/scientific/lcbfastmapping.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     4831 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/scientific/mos.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/recipes/tests/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/tests/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1462 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/recipes/tests/test_calibration.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3707 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/requirements.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/simulation/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    25329 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/actions.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3415 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/control.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2285 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/convolution.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1610 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/efficiency.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1216 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/extended.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     8579 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/factory.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1078 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/fiberbundle.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1316 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/focalplane.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1851 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/lightfiber.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2766 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/refraction.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2584 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/simulation/vph.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1004 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/taggers.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/tests/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tests/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2066 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tests/create.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      540 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tests/simpleobj.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      783 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tests/test_binning.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3488 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tests/test_datamodel.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    10427 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tests/test_drp.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      190 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tests/test_loader.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2347 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tests/test_taggers.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2418 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tests/test_types.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1852 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tests/test_utils.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/tools/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tools/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    22980 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/tools/overplot_traces.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp/tools/tests/
+-rw-rw-r--   0 spr       (1000) spr       (1000)        0 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tools/tests/__init__.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      254 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/tools/tests/test_overplot_traces.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     3328 2020-01-27 15:12:06.000000 megaradrp-0.9.3/megaradrp/types.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)      882 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/utils.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1179 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/validators.py
+-rw-rw-r--   0 spr       (1000) spr       (1000)    15840 2020-01-27 15:11:25.000000 megaradrp-0.9.3/megaradrp/visualization.py
+drwxrwxr-x   0 spr       (1000) spr       (1000)        0 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp.egg-info/
+-rw-rw-r--   0 spr       (1000) spr       (1000)     2555 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp.egg-info/PKG-INFO
+-rw-rw-r--   0 spr       (1000) spr       (1000)     6742 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp.egg-info/SOURCES.txt
+-rw-rw-r--   0 spr       (1000) spr       (1000)        1 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp.egg-info/dependency_links.txt
+-rw-rw-r--   0 spr       (1000) spr       (1000)      187 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp.egg-info/entry_points.txt
+-rw-rw-r--   0 spr       (1000) spr       (1000)        1 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp.egg-info/not-zip-safe
+-rw-rw-r--   0 spr       (1000) spr       (1000)      167 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp.egg-info/requires.txt
+-rw-rw-r--   0 spr       (1000) spr       (1000)       10 2020-01-27 15:12:36.000000 megaradrp-0.9.3/megaradrp.egg-info/top_level.txt
+-rw-rw-r--   0 spr       (1000) spr       (1000)       92 2020-01-27 15:12:36.000000 megaradrp-0.9.3/setup.cfg
+-rw-rw-r--   0 spr       (1000) spr       (1000)     1954 2020-01-27 15:12:06.000000 megaradrp-0.9.3/setup.py
```

### Comparing `megaradrp-0.9.2/LICENSE.txt` & `megaradrp-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/PKG-INFO` & `megaradrp-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaradrp
-Version: 0.9.2
+Version: 0.9.3
 Summary: MEGARA Data Reduction Pipeline
 Home-page: https://github.com/guaix-ucm/megaradrp
 Author: Sergio Pascual
 Author-email: sergiopr@fis.ucm.es
 License: GPLv3
 Description: 
         ==========
```

### Comparing `megaradrp-0.9.2/README.rst` & `megaradrp-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/Makefile` & `megaradrp-0.9.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/auxiliary.txt` & `megaradrp-0.9.3/doc/auxiliary.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 Telescope focus
 ---------------
 
 :Mode: Telescope Focus
 :Usage: Online
-:Key: MEGARA_FOCUS_TELESCOPE
+:Key: MegaraFocusTelescope
 :Recipe: :class:`~megaradrp.recipes.auxiliary.focustel.FocusTelescopeRecipe`
 :Recipe input: :class:`~megaradrp.recipes.auxiliary.focustel.FocusTelescopeRecipe.FocusTelescopeRecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.auxiliary.focustel.FocusTelescopeRecipe.FocusTelescopeRecipeResult`
 
 This observing mode includes the required actions to focus GTC using MEGARA. A
 bright point source should be identified for this purpose. This mode is an
 alternative to obtain the best focus of the telescope using the A&G system.
@@ -97,15 +97,15 @@
       :members:
 
 Spectrograph focus
 ------------------
 
 :Mode: Spectrograph Focus
 :Usage: Online
-:Key: MEGARA_FOCUS_SPECTROGRAPH
+:Key: MegaraFocusSpectrograph
 :Recipe: :class:`~megaradrp.recipes.auxiliary.focusspec.FocusSpectrographRecipe`
 :Recipe input: :class:`~megaradrp.recipes.auxiliary.focusspec.FocusSpectrographRecipe.FocusSpectrographRecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.auxiliary.focusspec.FocusSpectrographRecipe.FocusSpectrographRecipeResult`
 
 
 This mode sequence includes the required actions to focus the MEGARA
 spectrograph. The arc lamps from the ICM will be used for this purpose. MEGARA
@@ -145,16 +145,14 @@
 analyzed. This analysis should include the computation of the FWHM of a few
 unresolved spectra lines at different wavelengths. This software should then
 decide based on the FWHM values computed at different wavelengths and positions
 along the pseudo-slit the best focus compromise. The best focus obtained for
 the VPH of choice should then be stored and used to determine the best foci for
 all spectral configurations (and instrument modes; TBC).
 
-
-
 Procedure
 +++++++++
 Spectrograph focus image sets through; at least, one of the MEGARA VPHs should
 be obtained at the beginning of every observing night by either the observer or
 the staff of the observatory (TBD). Once a VPH is checked, the rest of the
 values could be corrected relative to this one. It is expected that minor focus
 corrections should be done as the temperature changes. This could be modeled in
@@ -185,15 +183,15 @@
 
 
 Fine acquisition with the LCB IFU
 ---------------------------------
 
 :Mode: LCB Acquisition
 :Usage: Online
-:Key: MEGARA_LCB_ACQUISITION
+:Key: MegaraLcbAcquisition
 :Recipe: :class:`~megaradrp.recipes.auxiliary.acquisitionlcb.AcquireLCBRecipe`
 :Recipe input: :class:`~megaradrp.recipes.auxiliary.acquisitionlcb.AcquireLCBRecipe.RecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.auxiliary.acquisitionlcb.AcquireLCBRecipe.RecipeResult`
 
 
 This mode sequence includes the required actions to acquire a target with known
 celestial coordinates and place it at a reference position inside the LCB IFU
@@ -215,18 +213,14 @@
 As part of the MEGARA on-line quick-look software the image (or images)
 obtained as part of this observing mode should be processed and the spectra
 extracted so to determine the position of the centroid of the target in the
 corresponding field of view. A view of the field should be also produced in
 order to evaluate whether or not the angle of the Folded-Cass rotator matches
 that specified by the observer.
 
-
-Procedure
-+++++++++
-
 Products
 ++++++++
 Fine acquisition image sets should be obtained at the beginning of the
 observing night by either the observer or the staff of the observatory (TBD) or
 every time a problem with the telescope absolute pointing is suspected. Such
 image sets should be also obtained when an absolute positioning precision of
 the order of a fraction of the spaxel size is required, better than 0.62 arcsec
@@ -243,15 +237,15 @@
       :members:
 
 Fine acquisition with the Fiber MOS
 -----------------------------------
 
 :Mode: MOS Acquisition
 :Usage: Online
-:Key: MEGARA_LCB_ACQUISITION
+:Key: MegaraLcbAcquisition
 :Recipe: :class:`~megaradrp.recipes.auxiliary.acquisitionmos.AcquireMOSRecipe`
 :Recipe input: :class:`~megaradrp.recipes.auxiliary.acquisitionmos.AcquireMOSRecipe.RecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.auxiliary.acquisitionmos.AcquireMOSRecipe.RecipeResult`
 
 The sequence for this observing mode includes the required actions to acquire a
 list of targets with known celestial coordinates and place each target at the
 center of a different robotic positioner. The information on the assignment of
@@ -280,18 +274,14 @@
 should be included in each Fiber MOS configuration block in order for this
 observing mode to generate a solution. The quick-look software should compare
 the expected and the actual positions of these reference sources in order to
 determine the best-fitting set of offsets (both in X and Y) and rotation angle
 to apply to the telescope and Folded-Cass rotator, respectively, to then
 continue with one of the scientific observing modes described in next Section.
 
-
-Procedure
-+++++++++
-
 Products
 ++++++++
 Fine acquisition image sets should be obtained by the observer at the beginning
 of the observation of each field with the Fiber MOS. The observatory staff
 should decide whether or not the corrections derived (telescope offset and
 Folded-Cass rotator angle) must be applied to the acquisition of other fields
 with the Fiber MOS during the same observing night or exclusively to the target
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/calibration/arc.txt` & `megaradrp-0.9.3/doc/calibration/arc.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Arc Calibration
----------------
+Arc
+---
 
-:Mode: Arc Calibration
-:Usage: Offline
-:Key: MEGARA_ARC_CALIBRATION
+:Mode: Arc
+:Usage: Offline, Online
+:Key: MegaraArcCalibration
 :Product: :class:`~megaradrp.products.wavecalibration.WavelengthCalibration`
 :Recipe: :class:`~megaradrp.recipes.calibration.arc.ArcCalibrationRecipe`
 :Recipe input: :class:`~megaradrp.recipes.calibration.arc.ArcCalibrationRecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.calibration.arc.ArcCalibrationRecipeResult`
 
 This mode sequence includes the required actions to translate the geometrical
 position of each point in the detector into physical units of wavelength. The
@@ -55,8 +55,8 @@
 (the format is TBD), a QA flag, a text log file of the processing and a
 structured text file containing information about the processing.
 
 Recipe, inputs and results
 ++++++++++++++++++++++++++
 
 .. autoclass:: megaradrp.recipes.calibration.arc.ArcCalibrationRecipe
-      :members:
+      :members:
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/calibration/bias.txt` & `megaradrp-0.9.3/doc/calibration/bias.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 **********
 Bias Image
 **********
 
-:Mode: Bias Image
+:Mode: Bias
 :Usage: Offline, Online
-:Key: MEGARA_BIAS_IMAGE
+:Key: MegaraBIAS_IMAGE
 :Product: :class:`~megaradrp.types.MasterBias`
 :Recipe: :class:`~megaradrp.recipes.calibration.bias.BiasRecipe`
 :Recipe input: :class:`~megaradrp.recipes.calibration.bias.BiasRecipe.RecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.calibration.bias.BiasRecipe.RecipeResult`
 
 Before the Analog-to-Digital conversion is performed a pedestal (electronic)
 level is added to all images obtained with the MEGARA CCD. This is a standard
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/calibration/bpm.txt` & `megaradrp-0.9.3/doc/calibration/bpm.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Bad-pixels mask
 ---------------
 
 :Mode: Bad-pixels mask
-:Usage: Offline
-:Key: MEGARA_BAD_PIXEL_MASK
+:Usage: Offline, Online
+:Key: MegaraBadPixelMask
 :Product: :class:`~megaradrp.types.MasterBPM`
 :Recipe: :class:`~megaradrp.recipes.calibration.bpm.BadPixelsMaskRecipe`
 :Recipe input: :class:`~megaradrp.recipes.calibration.bpm.BadPixelsMaskRecipe.BadPixelsMaskRecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.calibration.bpm.BadPixelsMaskRecipe.BadPixelsMaskRecipeResult`
 
 Although science-grade CCD detectors show very few bad pixels / bad columns
 there will be a number of pixels (among the ~17 Million pixels in the MEGARA
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/calibration/dark.txt` & `megaradrp-0.9.3/doc/calibration/dark.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Dark Image
 ----------
 
-:Mode: Dark Image
-:Usage: Offline
-:Key: MEGARA_DARK_IMAGE
+:Mode: Dark
+:Usage: Offline, Online
+:Key: MegaraDarkImage
 :Product: :class:`~megaradrp.types.MasterDark`
 :Recipe: :class:`~megaradrp.recipes.calibration.dark.DarkRecipe`
 :Recipe input: :class:`~megaradrp.recipes.calibration.dark.DarkRecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.calibration.dark.DarkRecipeResult`
 
 The potential wells in CCD detectors spontaneously generate electron-ion pairs
 at a rate that is a function of temperature. For very long exposures this
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/calibration/fiberflat.txt` & `megaradrp-0.9.3/doc/calibration/fiberflat.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Fiber-flat
 ----------
 
 :Mode: Fiber-flat
-:Usage: Offline
-:Key: MEGARA_FIBER_FLAT_IMAGE
+:Usage: Offline, Online
+:Key: MegaraFiberFlatImage
 :Product: :class:`~megaradrp.types.MasterFiberFlat`
 :Recipe: :class:`~megaradrp.recipes.calibration.flat.FiberFlatRecipe`
 :Recipe input: :class:`~megaradrp.recipes.calibration.flat.FiberFlatRecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.calibration.flat.FiberFlatRecipeResult`
 
 In fiber-fed spectrographs such as MEGARA each optical fiber behaves like a
 different optical system, and therefore, its optical transmission is different
@@ -51,13 +51,14 @@
 
 Products
 ++++++++
 Fiber-flat image sets are to be obtained both as part of the activities related
 to the verification of the instrument status and for processing data for
 scientific exploitation.
 
+.. _ff-mode-label:
 
 Recipe, inputs and results
 ++++++++++++++++++++++++++
 
 .. autoclass:: megaradrp.recipes.calibration.flat.FiberFlatRecipe
    :members:
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/calibration/index.txt` & `megaradrp-0.9.3/doc/calibration/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -69,12 +69,15 @@
 .. toctree::
    :maxdepth: 1
 
    bias
    dark
    slitflat
    trace
+   model
    arc
    fiberflat
    twilight
    bpm
    linearity
+   lcbstd
+   mosstd
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/calibration/linearity.txt` & `megaradrp-0.9.3/doc/calibration/linearity.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Linearity tests
----------------
+Linearity test
+--------------
 
-:Mode: Linearity tests
-:Usage: Offline
-:Key: MEGARA_LINEARITY_TEST
+:Mode: Linearity test
+:Usage: Offline, Online
+:Key: MegaraLinearityTest
 :Product:
 :Recipe: :class:`~megaradrp.recipes.calibration.linearity.LinearityTestRecipe`
 :Recipe input: :class:`~megaradrp.recipes.calibration.linearity.LinearityTestRecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.calibration.linearity.LinearityTestRecipeResult`
 
 Although the linearity of the MEGARA CCD are well characterized at the LICA lab
 already, it might be advisable to generate linearity test frames both as part
@@ -65,8 +65,8 @@
 considered part of the "System Calibration Modes".
 
 
 Recipe, inputs and results
 ++++++++++++++++++++++++++
 
 .. autoclass:: megaradrp.recipes.calibration.linearity.LinearityTestRecipe
-      :members:
+      :members:
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/calibration/slitflat.txt` & `megaradrp-0.9.3/doc/calibration/slitflat.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Slit-flat
 ---------
 
 :Mode: Slit-flat
-:Usage: Offline
-:Key: MEGARA_SLIT_FLAT
+:Usage: Offline, Online
+:Key: MegaraSlitFlat
 :Product: :class:`~megaradrp.types.MasterSlitFlat`
 :Recipe: :class:`~megaradrp.recipes.calibration.slitflat.SlitFlatRecipe`
 :Recipe input: :class:`~megaradrp.recipes.calibration.slitflat.SlitFlatRecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.calibration.slitflat.SlitFlatRecipeResult`
 
 In the case of fiber-fed spectrographs the correction for the detector
 pixel-to-pixel variation of the sensibility is usually carried out using data
@@ -64,8 +64,8 @@
 processing and a structured text file containing information about the
 processing.
 
 Recipe, inputs and results
 ++++++++++++++++++++++++++
 
 .. autoclass:: megaradrp.recipes.calibration.slitflat.SlitFlatRecipe
-      :members:
+      :members:
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/calibration/trace.txt` & `megaradrp-0.9.3/doc/calibration/trace.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 =====
 Trace
 =====
 
 :Mode: Trace
 :Usage: Offline, Online
-:Key: MEGARA_TRACE_MAP
+:Key: MegaraTraceMap
 :Product: :class:`~megaradrp.products.tracemap.TraceMap`.
 :Recipe: :class:`~megaradrp.recipes.calibration.trace.TraceMapRecipe`
 :Recipe input: :class:`~megaradrp.recipes.calibration.trace.TraceMapRecipeInput`
 :Recipe result: :class:`~megaradrp.recipes.calibration.trace.TraceMapRecipeResult`
 
 
 Although for the majority of the observing modes described elsewhere in this
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/calibration/twilight.txt` & `megaradrp-0.9.3/doc/calibration/twilight.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Twilight fiber-flat
 -------------------
 
 :Mode: Twilight fiber-flat
-:Usage: Offline
-:Key: MEGARA_TWILIGHT_FLAT_IMAGE
+:Usage: Offline, Online
+:Key: MegaraTwilightFlatImage
 :Product: :class:`~megaradrp.types.MasterTwilightFlat`
 :Recipe: :class:`~megaradrp.recipes.calibration.twilight.TwilightFiberFlatRecipe`
 :Recipe input: :class:`megaradrp.recipes.calibration.twilight.RecipeInput`
 :Recipe result: :class:`megaradrp.recipes.calibration.twilight.RecipeResult`
 
 Depending on the final performance of the ICM (provided by the GTC) at F-C the
 twilight fiber-flat mode (proposed in this section) might be offered as
@@ -69,8 +69,8 @@
 .. autoclass:: megaradrp.recipes.calibration.twilight.RecipeInput
       :members:
 
 .. autoclass:: megaradrp.recipes.calibration.twilight.RecipeResult
       :members:
 
 .. autoclass:: megaradrp.recipes.calibration.twilight.TwilightFiberFlatRecipe
-      :members:
+      :members:
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/index.txt` & `megaradrp-0.9.3/doc/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -21,19 +21,20 @@
    :maxdepth: 2
 
    intro
    installation
    testing
    running
    modes
-
+   products
 
 Developer documentation
 -----------------------
 
 .. toctree::
    :maxdepth: 2
 
    recipes
-   products
    reference/index
-   glossary
+   glossary
+
+Maintainers: Sergio Pascual sergiopr@fis.ucm.es, Nicolás Cardiel cardiel@ucm.es
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/installation.txt` & `megaradrp-0.9.3/doc/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 ************
 Requirements
 ************
 
 The MEGARA Pipeline package requires the following packages installed in order to
 be able to be installed and work properly:
 
- - `python 2.7 <https://www.python.org>`_
+ - `python <https://www.python.org>`_ either 2.7 or >= 3.4
  - `setuptools <http://peak.telecommunity.com/DevCenter/setuptools>`_
  - `numpy <http://www.numpy.org/>`_ >= 1.7
  - `scipy <http://www.scipy.org/>`_
- - `astropy <http://www.astropy.org/>`_ >= 1.0
- - `numina <https://pypi.python.org/pypi/numina/>`_ >= 0.13
+ - `astropy <http://www.astropy.org/>`_ >= 2.0
+ - `numina <https://pypi.python.org/pypi/numina/>`_ >= 0.17
  - `scikit-image <http://scikit-image.org/>`_
 
 Additional packages are optionally required:
 
  - `py.test <http://pytest.org>`_ >= 2.5 to run the tests
  - `sphinx`_ to build the documentation
 
@@ -26,44 +26,35 @@
 *********************
 Installing MEGARA DRP
 *********************
 
 Using Conda
 ===========
 
-TBD
+`megaradrp` can be installed with conda using a custom channel.
+
+From the shell, execute:::
+
+ conda install -c conda-forge megaradrp
+
 
 Using pip
 =========
 To install with pip, simply run:::
 
    pip install --no-deps megaradrp
    
 .. note::
 
     The ``--no-deps`` flag is optional, but highly recommended if you already
     have Numpy installed, since otherwise pip will sometimes try to upgrade 
     your Numpy installation, which may not always be desired.
 
-MEGARA DRP is registered in the Python Package Index. That means (among 
-other things) that can be installed inside the environment with one command.
 
 
-  (myenv) $ pip install megaradrp
-  
-The requirements of megaradrp will be downloaded and installed inside
-the virtual environment. Once the installation is finished, you can check
-by listing the installed recipes with the command line interface tool ``numina``::
-
-  (myenv) $ ./bin/numina show-instruments
-  INFO: Numina simple recipe runner version 0.13.0
-  Instrument: MEGARA
-   has configuration 'default'
-   has pipeline 'default', version 1
-   has pipeline 'experimental', version 1
 
 Building from source
 ====================
 
 The latest stable version of MEGARA DRP can be downloaded from
 https://pypi.python.org/pypi/megaradrp
 
@@ -74,15 +65,29 @@
     $ python setup.py install
     
 The `install` command provides options to change the target directory. By 
 default installation requires administrative privileges. The different 
 installation options can be checked with::
 
    $ python setup.py install --help
-   
+
+
+Checking the installation
+=========================
+Once the installation is finished, you can check
+by listing the installed recipes with the command line interface tool ``numina``::
+
+  (myenv) $ ./bin/numina show-instruments
+  INFO: Numina simple recipe runner version 0.13.0
+  Instrument: MEGARA
+   has configuration 'default'
+   has pipeline 'default', version 1
+   has pipeline 'experimental', version 1
+
+
 Development version
 -------------------
 
 The development version can be checked out with::
 
     $ git clone https://github.com/guaix-ucm/megaradrp.git
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/products.txt` & `megaradrp-0.9.3/doc/products.rst`

 * *Files 27% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 Data Products
 *************
 
 Each recipe of the MEGARA Pipeline produces a set of predefined results, known
 as *data products*. In turn, the recipes may request different data products
 as computing requirements, effectively chaining the recipes.
 
-For example, the requirements of the :ref:`ff-mode-label` recipe include a
-:class:`~megara.products.MasterDark` object. This object is produced by
-the recipe :class:`~megaradrp.recipes.calibration.DarkRecipe`, which in turn requires a 
-:class:`~megara.products.MasterBias` object.
+For example, the requirements of :class:`~megaradrp.recipes.calibration.flat.FiberFlatRecipe`
+include a :class:`~megaradrp.types.MasterDark` object. This object is produced by
+the recipe :class:`~megaradrp.recipes.calibration.dark.DarkRecipe`, which in turn requires a
+:class:`~megaradrp.types.MasterBias` object.
 
 .. toctree::
 
    keywords
-   rawimages
    images
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/recipes.txt` & `megaradrp-0.9.3/doc/recipes.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
         
     @define_input(SomeRecipeInput)
     @define_result(SomeRecipeResult)
     class SomeRecipe(RecipeBase):        
         ...
 
         
-The data products of the MEGARA DRP are describe in :doc:`products`
+The data products of the MEGARA DRP are describe in :doc:`products`
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/running.txt` & `megaradrp-0.9.3/doc/running.rst`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 This is an example of the observation result file
 
 .. code-block:: yaml
 
     id: dark-test-21
     instrument: MEGARA
-    mode: MEGARA_DARK_IMAGE
+    mode: MegaraDarkImage
     images:
       - r0121.fits
       - r0122.fits
       - r0123.fits
       - r0124.fits
       - r0125.fits
       - r0126.fits
@@ -78,15 +78,15 @@
        - {id: 4, content: 'file4.fits', type: 'MasterBias', tags: {'readmode': 'cds'}, ob: 400} (3)
       MEGARA:
        - {id: 1, content: 'file1.fits', type: 'MasterFiberFlat', tags: {'vph': 'LR-U'}, ob: 1200} (3)
        - {id: 2, content: 'file2.yml', type: 'TraceMap', tags: {'vph': 'LR2', 'readmode': 'fast'}, ob: 1203} (3)
     requirements: (4)
       MEGARA:
          default:
-           MEGARA_ARC_IMAGE:  (5)
+           MegaraArcImage:  (5)
               polynomial_degree: 5 (6)
               nlines: [5, 5]       (6)
 
 
 1. Mandatory entry, ``version`` must be 1
 2. Products of other recipes are list, by instrument
 3. The products of the reduction recipes are listed. Each result must contain:
@@ -116,15 +116,15 @@
   $ numina run --workdir /tmp/test1 --datadir /scrat/obs/run12222 obs.yaml -r requires.yaml
 
 See :ref:`numina:cli` for a full description of the command line interface.
 
 Following the example, we create a directory ``data`` in our current directory and copy
 there the raw frames from ``r0121.fits`` to ``r0132.fits`` and the master bias ``master_bias-1.fits``.
 
-The we run::
+Then we run::
 
   $ numina run obsresult.yaml -r requirements.yaml
   INFO: Numina simple recipe runner version 0.15
   INFO: Loading observation result from 'obsrun.yaml'
   INFO: Identifier of the observation result: 1
   INFO: instrument name: MEGARA
   ...
@@ -174,20 +174,20 @@
         a0 -> a1 [rank=same];
         a1 -> a2 [rank=same];
         a1 -> a4 [rank=same];
         a2 -> a3 [rank=same];
         a4 -> a3 [rank=same];
         a5 -> a4 [rank=same];
 
-        a0 [label="MEGARA_BIAS_IMAGE"];
-        a1 [label="MEGARA_TRACE_MAP"];
-        a2 [label="MEGARA_ARC_CALIBRATION"];
-        a3 [label="MEGARA_FIBER_FLAT_IMAGE"];
-        a4 [label="MEGARA_WEIGHTS"];
-        a5 [label="MEGARA_SLIT_FLAT"];
+        a0 [label="MegaraBiasImage"];
+        a1 [label="MegaraTraceMap"];
+        a2 [label="MegaraArcCalibration"];
+        a3 [label="MegaraModelMap"];
+        a4 [label="MegaraFiberFlat"];
+        a5 [label="MegaraSlitFlat"];
 
     }
 
 It is important to emphasize the fact that each time a Recipe is run, the results must be
 renamed and copied to the ``data`` directory in order to be the input of the
 next Recipe if it is needed. Taking this in mind, the content of the
 ``requirements.yaml`` file might well be and is common to all Recipes:
@@ -195,114 +195,108 @@
 .. code-block:: yaml
 
     version: 1
     products:
       MEGARA:
       - {id: 1, type: 'LinesCatalog', tags: {}, content: 'ThAr_arc_LR-U.txt'}
       - {id: 2, type: 'MasterBias', tags: {}, content: 'master_bias.fits'}
-      - {id: 3, type: 'TraceMap', tags: {}, content: 'master_traces.yaml'}
+      - {id: 3, type: 'TraceMap', tags: {}, content: 'master_traces.json'}
       - {id: 4, type: 'MasterFiberFlat', tags: {}, content: 'master_fiberflat.fits'}
       - {id: 5, type: 'WavelengthCalibration', tags: {}, content: 'master_wlcalib.json'}
       - {id: 6, type: 'MasterFiberFlatFrame', tags: {}, content: 'fiberflat_frame.fits'}
-      - {id: 7, type: 'MasterWeights', tags: {}, content: 'master_weights.tar'}
+      - {id: 7, type: 'ModelMap', tags: {}, content: 'master_model.json'}
       - {id: 8, type: 'MasterSlitFlat', tags: {}, content: 'master_slitflat.fits'}
     requirements: {}
 
 In order to run the next example, the user should execute the next command
 at least 6 times taking into account that the file ``obsresult-%step.yaml`` should
 change with each execution::
 
     $ numina run obsresult-1.yaml -r requirements.yaml
     $ numina run obsresult-2.yaml -r requirements.yaml
     ...
     $ numina run obsresult-6.yaml -r requirements.yaml
 
-MEGARA_BIAS_IMAGE file, obsresult-1.yaml:
+MegaraBiasImage file, obsresult-1.yaml:
 
 .. code-block:: yaml
 
     id: 1
     instrument: MEGARA
-    mode: MEGARA_BIAS_IMAGE
-    configuration: science
+    mode: MegaraBiasImage
     images:
       - bias1.fits
       - bias2.fits
       - bias3.fits
       - bias4.fits
       - bias5.fits
 
-MEGARA_TRACE_MAP, obsresult-2.yaml:
+MegaraTraceMap, obsresult-2.yaml:
 
 .. code-block:: yaml
 
     id: 2
     instrument: MEGARA
-    mode: MEGARA_TRACE_MAP
-    configuration: science
+    mode: MegaraTraceMap
     images:
       - flat1.fits
       - flat2.fits
       - flat3.fits
       - flat4.fits
       - flat5.fits
 
-MEGARA_ARC_CALIBRATION, obsresult-3.yaml:
+MegaraArcCalibration, obsresult-3.yaml:
 
 .. code-block:: yaml
 
     id: 3
     instrument: MEGARA
-    mode: MEGARA_ARC_CALIBRATION
-    configuration: science
+    mode: MegaraArcCalibration
     images:
       - arc1.fits
       - arc2.fits
       - arc3.fits
       - arc4.fits
       - arc5.fits
 
-MEGARA_SLIT_FLAT, obsresult-4.yaml:
+MegaraSlitFlat, obsresult-4.yaml:
 
 .. code-block:: yaml
 
     id: 4
     instrument: MEGARA
-    mode: MEGARA_SLIT_FLAT
-    configuration: science
+    mode: MegaraSlitFlat
     images:
       - flat1.fits
       - flat2.fits
       - flat3.fits
       - flat4.fits
       - flat5.fits
 
-MEGARA_WEIGHTS, obsresult-5.yaml:
+MegaraModel, obsresult-5.yaml:
 
 .. code-block:: yaml
 
     id: 5
     instrument: MEGARA
-    mode: MEGARA_WEIGHTS
-    configuration: science
+    mode: MegaraModelMap
     images:
       - flat1.fits
       - flat2.fits
       - flat3.fits
       - flat4.fits
       - flat5.fits
 
-MEGARA_FIBER_FLAT_IMAGE, obsresult-6.yaml:
+MegaraFiberFlat, obsresult-6.yaml:
 
 .. code-block:: yaml
 
     id: 6
     instrument: MEGARA
-    mode: MEGARA_FIBER_FLAT_IMAGE
-    configuration: science
+    mode: MegaraFiberFlat
     images:
       - flat1.fits
       - flat2.fits
       - flat3.fits
       - flat4.fits
       - flat5.fits
```

### Comparing `megaradrp-0.9.2/doc/_build/html/_sources/testing.txt` & `megaradrp-0.9.3/doc/testing.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/_static/megara.png` & `megaradrp-0.9.3/doc/_static/megara.png`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/calibration/lcbstd.rst` & `megaradrp-0.9.3/doc/calibration/lcbstd.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/calibration/model.rst` & `megaradrp-0.9.3/doc/calibration/model.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/calibration/mosstd.rst` & `megaradrp-0.9.3/doc/calibration/mosstd.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/combined.rst` & `megaradrp-0.9.3/doc/combined.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/conf.py` & `megaradrp-0.9.3/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
               'sphinx.ext.mathjax', 'numpydoc']
 
 master_doc = 'index'
 templates_path = ['_templates']
 exclude_patterns = ['_build']
 
 project = u'MEGARA Data Reduction Pipeline'
-copyright = u'2013-2019, Universidad Complutense de Madrid'
+copyright = u'2013-2020, Universidad Complutense de Madrid'
 version = '0.9'
-release = '0.9.2'
+release = '0.9.3'
 show_authors = True
 
 numpydoc_show_class_members = False
 numpydoc_show_inherited_class_members = False
 
 
 # -- Options for HTML output ---------------------------------------------------
```

### Comparing `megaradrp-0.9.2/doc/images.rst` & `megaradrp-0.9.3/doc/images.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/keywords.rst` & `megaradrp-0.9.3/doc/keywords.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/reference/index.rst` & `megaradrp-0.9.3/doc/reference/index.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/reference/products.rst` & `megaradrp-0.9.3/doc/reference/products.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/reference/simulation.rst` & `megaradrp-0.9.3/doc/reference/simulation.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/doc/scientific.rst` & `megaradrp-0.9.3/doc/scientific.rst`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/core/correctors.py` & `megaradrp-0.9.3/megaradrp/core/correctors.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/core/recipe.py` & `megaradrp-0.9.3/megaradrp/core/recipe.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/datamodel.py` & `megaradrp-0.9.3/megaradrp/datamodel.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/db/control.py` & `megaradrp-0.9.3/megaradrp/db/control.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/db/model.py` & `megaradrp-0.9.3/megaradrp/db/model.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/drp.yaml` & `megaradrp-0.9.3/megaradrp/drp.yaml`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/__init__.py` & `megaradrp-0.9.3/megaradrp/instrument/__init__.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/components/cover.py` & `megaradrp-0.9.3/megaradrp/instrument/components/cover.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/components/detector.py` & `megaradrp-0.9.3/megaradrp/instrument/components/detector.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/components/fibermos.py` & `megaradrp-0.9.3/megaradrp/instrument/components/fibermos.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/components/instrument.py` & `megaradrp-0.9.3/megaradrp/instrument/components/instrument.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/components/lamps.py` & `megaradrp-0.9.3/megaradrp/instrument/components/lamps.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/components/psslit.py` & `megaradrp-0.9.3/megaradrp/instrument/components/psslit.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/components/shutter.py` & `megaradrp-0.9.3/megaradrp/instrument/components/shutter.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/components/telescope.py` & `megaradrp-0.9.3/megaradrp/instrument/components/telescope.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/configs/component-06fc5d6d-d20b-4eba-b3fa-57696f0a1103.json` & `megaradrp-0.9.3/megaradrp/instrument/configs/component-06fc5d6d-d20b-4eba-b3fa-57696f0a1103.json`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/configs/component-2e02e135-2325-47c9-9975-466b445b0b8b.json` & `megaradrp-0.9.3/megaradrp/instrument/configs/component-2e02e135-2325-47c9-9975-466b445b0b8b.json`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/configs/component-715c7ced-f989-42a6-bb74-a5b5cda0495c.json` & `megaradrp-0.9.3/megaradrp/instrument/configs/component-715c7ced-f989-42a6-bb74-a5b5cda0495c.json`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/configs/component-97d48545-3258-473e-9311-00e390999d52.json` & `megaradrp-0.9.3/megaradrp/instrument/configs/component-97d48545-3258-473e-9311-00e390999d52.json`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/configs/lcb_default_header.txt` & `megaradrp-0.9.3/megaradrp/instrument/configs/lcb_default_header.txt`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/configs/mos_default_header.txt` & `megaradrp-0.9.3/megaradrp/instrument/configs/mos_default_header.txt`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/configs/primary.txt` & `megaradrp-0.9.3/megaradrp/instrument/configs/primary.txt`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/instrument/configs/properties-86a6e968-8d3d-456f-89f8-09ff0c7f7c57.json` & `megaradrp-0.9.3/megaradrp/instrument/configs/properties-86a6e968-8d3d-456f-89f8-09ff0c7f7c57.json`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/aperture.py` & `megaradrp-0.9.3/megaradrp/processing/aperture.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/combine.py` & `megaradrp-0.9.3/megaradrp/processing/combine.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/extractobj.py` & `megaradrp-0.9.3/megaradrp/processing/extractobj.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/fiberflat.py` & `megaradrp-0.9.3/megaradrp/processing/fiberflat.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/fibermatch.py` & `megaradrp-0.9.3/megaradrp/processing/fibermatch.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/fluxcalib.py` & `megaradrp-0.9.3/megaradrp/processing/fluxcalib.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/multirss.py` & `megaradrp-0.9.3/megaradrp/processing/multirss.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/slitflat.py` & `megaradrp-0.9.3/megaradrp/processing/slitflat.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/tests/test_aperture.py` & `megaradrp-0.9.3/megaradrp/processing/tests/test_aperture.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/tests/test_extractobj.py` & `megaradrp-0.9.3/megaradrp/processing/tests/test_extractobj.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/tests/test_fibermatch.py` & `megaradrp-0.9.3/megaradrp/processing/tests/test_fibermatch.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/tests/test_fluxcalib.py` & `megaradrp-0.9.3/megaradrp/processing/tests/test_fluxcalib.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/tests/test_multirss.py` & `megaradrp-0.9.3/megaradrp/processing/tests/test_multirss.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/tests/test_processing.py` & `megaradrp-0.9.3/megaradrp/processing/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/tests/test_trimover.py` & `megaradrp-0.9.3/megaradrp/processing/tests/test_trimover.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/tests/test_wcs.py` & `megaradrp-0.9.3/megaradrp/processing/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/trimover.py` & `megaradrp-0.9.3/megaradrp/processing/trimover.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/twilight.py` & `megaradrp-0.9.3/megaradrp/processing/twilight.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/wavecalibration.py` & `megaradrp-0.9.3/megaradrp/processing/wavecalibration.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/wcs.py` & `megaradrp-0.9.3/megaradrp/processing/wcs.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/processing/weights.py` & `megaradrp-0.9.3/megaradrp/processing/weights.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/products/modelmap.py` & `megaradrp-0.9.3/megaradrp/products/modelmap.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/products/structured.py` & `megaradrp-0.9.3/megaradrp/products/structured.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/products/tracemap.py` & `megaradrp-0.9.3/megaradrp/products/tracemap.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/products/traces.py` & `megaradrp-0.9.3/megaradrp/products/traces.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/products/wavecalibration.py` & `megaradrp-0.9.3/megaradrp/products/wavecalibration.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/auxiliary/acquisitionlcb.py` & `megaradrp-0.9.3/megaradrp/recipes/auxiliary/acquisitionlcb.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/auxiliary/acquisitionmos.py` & `megaradrp-0.9.3/megaradrp/recipes/auxiliary/acquisitionmos.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/auxiliary/focusspec.py` & `megaradrp-0.9.3/megaradrp/recipes/auxiliary/focusspec.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/auxiliary/focustel.py` & `megaradrp-0.9.3/megaradrp/recipes/auxiliary/focustel.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/arc.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/arc.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/base.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/base.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/bias.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/bias.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/bpm.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/bpm.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/dark.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/dark.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/flat.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/flat.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/lcbstdstar.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/lcbstdstar.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/modelmap.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/modelmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,35 +331,27 @@
             for c, df in zip(candidates, dis_f):
                 if df > lateral:
                     # remove contribution
                     y -= gauss_box_model(xt, **init[c])
                 else:
                     fit_ids.append(c)
 
-            num_of_fibers = len(fit_ids)
+            # num_of_fibers = len(fit_ids)
             # print('lateral', lateral, val, fit_ids)
             # print('num', num_of_fibers)
 
-            Model = Const1D
-            for _ in range(num_of_fibers):
-                Model = Model + GaussBox
-
             # Extract values to create initials
-            sub_init = {}
-            sub_init["amplitude_0"] = 0.0
-            for idx, fib_id in enumerate(fit_ids, 1):
-                key = "amplitude_%d" % idx
-                sub_init[key] = init[fib_id]['amplitude']
-                key = "mean_%d" % idx
-                sub_init[key] = init[fib_id]['mean']
-                key = "stddev_%d" % idx
-                sub_init[key] = init[fib_id]['stddev']
-
-            # Model = sum_of_gaussian_factory(num_of_fibers)
-            model = Model(**sub_init)
+            model = Const1D(amplitude=0.0)
+            for fib_id in fit_ids:
+                newg = GaussBox(
+                    amplitude=init[fib_id]['amplitude'],
+                    mean=init[fib_id]['mean'],
+                    stddev=init[fib_id]['stddev']
+                )
+                model = model + newg
 
             # Set fit conditions
             model.amplitude_0.fixed = True
             for idx, fib_id in enumerate(fit_ids, 1):
                 key = "mean_%d" % idx
                 m_mean = getattr(model, key)
                 if fixed_centers:
```

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/mosstdstar.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/mosstdstar.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/slitflat.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/slitflat.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_arc.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_bias.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_bias.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_bpm.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_bpm.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_bpm_common.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_bpm_common.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_bpm_corrector.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_bpm_corrector.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_dark.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/tests/test_tracemap.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/tests/test_tracemap.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/trace.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/trace.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/calibration/twilight.py` & `megaradrp-0.9.3/megaradrp/recipes/calibration/twilight.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/combined/extinctionstar.py` & `megaradrp-0.9.3/megaradrp/recipes/combined/extinctionstar.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/combined/sensstar.py` & `megaradrp-0.9.3/megaradrp/recipes/combined/sensstar.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/scientific/base.py` & `megaradrp-0.9.3/megaradrp/recipes/scientific/base.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/scientific/lcb.py` & `megaradrp-0.9.3/megaradrp/recipes/scientific/lcb.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/scientific/lcbfastmapping.py` & `megaradrp-0.9.3/megaradrp/recipes/scientific/lcbfastmapping.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/scientific/mos.py` & `megaradrp-0.9.3/megaradrp/recipes/scientific/mos.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/recipes/tests/test_calibration.py` & `megaradrp-0.9.3/megaradrp/recipes/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/requirements.py` & `megaradrp-0.9.3/megaradrp/requirements.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/actions.py` & `megaradrp-0.9.3/megaradrp/simulation/actions.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/control.py` & `megaradrp-0.9.3/megaradrp/simulation/control.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/convolution.py` & `megaradrp-0.9.3/megaradrp/simulation/convolution.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/efficiency.py` & `megaradrp-0.9.3/megaradrp/simulation/efficiency.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/extended.py` & `megaradrp-0.9.3/megaradrp/simulation/extended.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/factory.py` & `megaradrp-0.9.3/megaradrp/simulation/factory.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/fiberbundle.py` & `megaradrp-0.9.3/megaradrp/simulation/fiberbundle.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/focalplane.py` & `megaradrp-0.9.3/megaradrp/simulation/focalplane.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/lightfiber.py` & `megaradrp-0.9.3/megaradrp/simulation/lightfiber.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/refraction.py` & `megaradrp-0.9.3/megaradrp/simulation/refraction.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/simulation/vph.py` & `megaradrp-0.9.3/megaradrp/simulation/vph.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/taggers.py` & `megaradrp-0.9.3/megaradrp/taggers.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/tests/create.py` & `megaradrp-0.9.3/megaradrp/tests/create.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/tests/simpleobj.py` & `megaradrp-0.9.3/megaradrp/tests/simpleobj.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/tests/test_binning.py` & `megaradrp-0.9.3/megaradrp/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/tests/test_datamodel.py` & `megaradrp-0.9.3/megaradrp/tests/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/tests/test_drp.py` & `megaradrp-0.9.3/megaradrp/tests/test_drp.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/tests/test_taggers.py` & `megaradrp-0.9.3/megaradrp/tests/test_taggers.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/tests/test_types.py` & `megaradrp-0.9.3/megaradrp/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/tests/test_utils.py` & `megaradrp-0.9.3/megaradrp/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/tools/overplot_traces.py` & `megaradrp-0.9.3/megaradrp/tools/overplot_traces.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/types.py` & `megaradrp-0.9.3/megaradrp/types.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/utils.py` & `megaradrp-0.9.3/megaradrp/utils.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/validators.py` & `megaradrp-0.9.3/megaradrp/validators.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp/visualization.py` & `megaradrp-0.9.3/megaradrp/visualization.py`

 * *Files identical despite different names*

### Comparing `megaradrp-0.9.2/megaradrp.egg-info/PKG-INFO` & `megaradrp-0.9.3/megaradrp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaradrp
-Version: 0.9.2
+Version: 0.9.3
 Summary: MEGARA Data Reduction Pipeline
 Home-page: https://github.com/guaix-ucm/megaradrp
 Author: Sergio Pascual
 Author-email: sergiopr@fis.ucm.es
 License: GPLv3
 Description: 
         ==========
```

### Comparing `megaradrp-0.9.2/setup.py` & `megaradrp-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name='megaradrp',
-    version='0.9.2',
+    version='0.9.3',
     author='Sergio Pascual',
     author_email='sergiopr@fis.ucm.es',
     url='https://github.com/guaix-ucm/megaradrp',
     license='GPLv3',
     description='MEGARA Data Reduction Pipeline',
     packages=find_packages(),
     package_data={
```

