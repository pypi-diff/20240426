# Comparing `tmp/stardist-0.9.0.tar.gz` & `tmp/stardist-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stardist-0.9.0.tar", last modified: Tue Apr 23 22:13:57 2024, max compression
+gzip compressed data, was "stardist-0.9.1.tar", last modified: Thu Apr 25 21:28:38 2024, max compression
```

## Comparing `stardist-0.9.0.tar` & `stardist-0.9.1.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.337786 stardist-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-23 22:13:49.000000 stardist-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 22:13:49.000000 stardist-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21476 2024-04-23 22:13:57.337786 stardist-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20038 2024-04-23 22:13:49.000000 stardist-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 22:13:49.000000 stardist-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 22:13:57.337786 stardist-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-23 22:13:49.000000 stardist-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.313786 stardist-0.9.0/stardist/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25283 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/big.py
--rw-r--r--   0 runner    (1001) docker     (127)    20014 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/bioimageio_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.313786 stardist-0.9.0/stardist/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.317786 stardist-0.9.0/stardist/data/images/
--rw-r--r--   0 runner    (1001) docker     (127)    35505 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/images/histo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   524544 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/images/img2d.tif
--rw-r--r--   0 runner    (1001) docker     (127)   138925 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/images/img3d.tif
--rw-r--r--   0 runner    (1001) docker     (127)   524544 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/images/mask2d.tif
--rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/data/images/mask3d.tif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.317786 stardist-0.9.0/stardist/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/geometry/geom2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12542 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/geometry/geom3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.317786 stardist-0.9.0/stardist/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/kernels/stardist2d.cl
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/kernels/stardist3d.cl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.321786 stardist-0.9.0/stardist/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.309785 stardist-0.9.0/stardist/lib/external/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.321786 stardist-0.9.0/stardist/lib/external/clipper/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/clipper/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   142184 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/clipper/clipper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/clipper/clipper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.321786 stardist-0.9.0/stardist/lib/external/nanoflann/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/nanoflann/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    73558 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/nanoflann/nanoflann.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.321786 stardist-0.9.0/stardist/lib/external/qhull_src/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/Announce.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21849 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.313786 stardist-0.9.0/stardist/lib/external/qhull_src/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.325785 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/
--rw-r--r--   0 runner    (1001) docker     (127)    73854 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c
--rw-r--r--   0 runner    (1001) docker     (127)    45785 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h
--rw-r--r--   0 runner    (1001) docker     (127)    75784 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c
--rw-r--r--   0 runner    (1001) docker     (127)   140430 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h
--rw-r--r--   0 runner    (1001) docker     (127)    66346 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c
--rw-r--r--   0 runner    (1001) docker     (127)    56702 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h
--rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h
--rw-r--r--   0 runner    (1001) docker     (127)   208318 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c
--rw-r--r--   0 runner    (1001) docker     (127)    12247 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h
--rw-r--r--   0 runner    (1001) docker     (127)   145471 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c
--rw-r--r--   0 runner    (1001) docker     (127)    47472 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h
--rw-r--r--   0 runner    (1001) docker     (127)    34690 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c
--rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h
--rw-r--r--   0 runner    (1001) docker     (127)    25609 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c
--rw-r--r--   0 runner    (1001) docker     (127)    30324 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c
--rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h
--rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c
--rw-r--r--   0 runner    (1001) docker     (127)    33496 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.333785 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h
--rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h
--rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     7186 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18839 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19140 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist2d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    47204 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist3d_impl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist3d_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist3d_lib.c
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/stardist3d_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/test_lib3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/lib/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    19434 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.333785 stardist-0.9.0/stardist/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56860 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    28670 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/models/model2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    33562 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/models/model3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/nms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.333785 stardist-0.9.0/stardist/plot/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/plot/render.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/rays3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/sample_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.333785 stardist-0.9.0/stardist/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/scripts/predict2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/scripts/predict3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    15710 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 22:13:49.000000 stardist-0.9.0/stardist/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:13:57.333785 stardist-0.9.0/stardist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21476 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 22:13:57.000000 stardist-0.9.0/stardist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:38.005641 stardist-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-25 21:28:31.000000 stardist-0.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-25 21:28:31.000000 stardist-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-25 21:28:38.005641 stardist-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20008 2024-04-25 21:28:31.000000 stardist-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-25 21:28:32.000000 stardist-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 21:28:38.005641 stardist-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-25 21:28:32.000000 stardist-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.985641 stardist-0.9.1/stardist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25283 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/big.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20012 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/bioimageio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.985641 stardist-0.9.1/stardist/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.989641 stardist-0.9.1/stardist/data/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    35505 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/data/images/histo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   524544 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/data/images/img2d.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   138925 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/data/images/img3d.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   524544 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/data/images/mask2d.tif
+-rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/data/images/mask3d.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.989641 stardist-0.9.1/stardist/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/geometry/geom2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12542 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/geometry/geom3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.989641 stardist-0.9.1/stardist/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/kernels/stardist2d.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/kernels/stardist3d.cl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.989641 stardist-0.9.1/stardist/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.981641 stardist-0.9.1/stardist/lib/external/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.989641 stardist-0.9.1/stardist/lib/external/clipper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/clipper/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   142184 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/clipper/clipper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/clipper/clipper.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.989641 stardist-0.9.1/stardist/lib/external/nanoflann/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/nanoflann/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    73558 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/nanoflann/nanoflann.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.993641 stardist-0.9.1/stardist/lib/external/qhull_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/Announce.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21849 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.981641 stardist-0.9.1/stardist/lib/external/qhull_src/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:37.997641 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/
+-rw-r--r--   0 runner    (1001) docker     (127)    73854 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45785 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)    75784 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)   140430 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)    66346 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    56702 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)   208318 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12247 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)   145471 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    47472 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34690 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25609 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    30324 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33496 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:38.001641 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7186 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18839 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19140 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/stardist2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/stardist3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47204 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/stardist3d_impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/stardist3d_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/stardist3d_lib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/stardist3d_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/test_lib3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/lib/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19434 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:38.005641 stardist-0.9.1/stardist/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56860 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28670 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/models/model2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33562 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/models/model3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/nms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:38.005641 stardist-0.9.1/stardist/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/rays3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/sample_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:38.005641 stardist-0.9.1/stardist/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/scripts/predict2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/scripts/predict3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15710 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 21:28:32.000000 stardist-0.9.1/stardist/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:28:38.005641 stardist-0.9.1/stardist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-25 21:28:37.000000 stardist-0.9.1/stardist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-25 21:28:37.000000 stardist-0.9.1/stardist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:28:37.000000 stardist-0.9.1/stardist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 21:28:37.000000 stardist-0.9.1/stardist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 21:28:37.000000 stardist-0.9.1/stardist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 21:28:37.000000 stardist-0.9.1/stardist.egg-info/top_level.txt
```

### Comparing `stardist-0.9.0/LICENSE.txt` & `stardist-0.9.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2018-2023, Uwe Schmidt, Martin Weigert
+Copyright (c) 2018-2024, Uwe Schmidt, Martin Weigert
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `stardist-0.9.0/PKG-INFO` & `stardist-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stardist
-Version: 0.9.0
+Version: 0.9.1
 Summary: StarDist - Object Detection with Star-convex Shapes
 Home-page: https://github.com/stardist/stardist
 Author: Uwe Schmidt, Martin Weigert
 Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -39,19 +39,19 @@
 [![Test](https://github.com/stardist/stardist/workflows/Test/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3ATest)
 [![Test (PyPI)](https://github.com/stardist/stardist/workflows/Test%20(PyPI)/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3A%22Test+%28PyPI%29%22)
 [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fstardist.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&suffix=%20topics&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/stardist)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/stardist)](https://pypistats.org/packages/stardist)
 
 # *StarDist* - Object Detection with Star-convex Shapes
 
-![](https://github.com/stardist/stardist/raw/master/images/stardist_overview.png)
+![](https://github.com/stardist/stardist/raw/main/images/stardist_overview.png)
 
 This repository contains the Python implementation of star-convex object detection for 2D and 3D images, as described in the papers:
 
-<img src="https://github.com/stardist/stardist/raw/master/images/stardist_logo.jpg" title="siân is the king of the universe" width="25%" align="right">
+<img src="https://github.com/stardist/stardist/raw/main/images/stardist_logo.jpg" title="siân is the king of the universe" width="25%" align="right">
 
 - Uwe Schmidt, Martin Weigert, Coleman Broaddus, and Gene Myers.  
 [*Cell Detection with Star-convex Polygons*](https://arxiv.org/abs/1806.03535).  
 International Conference on Medical Image Computing and Computer-Assisted Intervention (MICCAI), Granada, Spain, September 2018.
 
 - Martin Weigert, Uwe Schmidt, Robert Haase, Ko Sugawara, and Gene Myers.  
 [*Star-convex Polyhedra for 3D Object Detection and Segmentation in Microscopy*](http://openaccess.thecvf.com/content_WACV_2020/papers/Weigert_Star-convex_Polyhedra_for_3D_Object_Detection_and_Segmentation_in_Microscopy_WACV_2020_paper.pdf).  
@@ -61,19 +61,19 @@
 
 
 ## Overview
 
 The following figure illustrates the general approach for 2D images. The training data consists of corresponding pairs of input (i.e. raw) images and fully annotated label images (i.e. every pixel is labeled with a unique object id or 0 for background).
 A model is trained to densely predict the distances (r) to the object boundary along a fixed set of rays and object probabilities (d), which together produce an overcomplete set of candidate polygons for a given input image. The final result is obtained via non-maximum suppression (NMS) of these candidates.
 
-![](https://github.com/stardist/stardist/raw/master/images/overview_2d.png)
+![](https://github.com/stardist/stardist/raw/main/images/overview_2d.png)
 
 The approach for 3D volumes is similar to the one described for 2D, using pairs of input and fully annotated label volumes as training data.
 
-![](https://github.com/stardist/stardist/raw/master/images/overview_3d.png)
+![](https://github.com/stardist/stardist/raw/main/images/overview_3d.png)
 
 ## Webinar/Tutorial
 
 If you want to know more about the concepts and practical applications of StarDist, please have a look at the following webinar that was given at NEUBIAS Academy @Home 2020:
 
 [![webinar video](http://img.youtube.com/vi/Amn_eHRGX5M/0.jpg)](http://www.youtube.com/watch?v=Amn_eHRGX5M "Webinar")
 
@@ -84,15 +84,15 @@
 
 If you only want to use a StarDist plugin for a GUI-based software, please read [this](#plugins-for-other-software).
 
 1. Please first [install TensorFlow](https://www.tensorflow.org/install)
 (either TensorFlow 1 or 2) by following the official instructions.
 For [GPU support](https://www.tensorflow.org/install/gpu), it is very
 important to install the specific versions of CUDA and cuDNN that are
-compatible with the respective version of TensorFlow. (If you need help and can use `conda`, take a look at [this](https://github.com/CSBDeep/CSBDeep/tree/master/extras#conda-environment).)
+compatible with the respective version of TensorFlow. (If you need help and can use `conda`, take a look at [this](https://github.com/CSBDeep/CSBDeep/tree/main/extras#conda-environment).)
 
 2. *StarDist* can then be installed with `pip`:
 
     - If you installed TensorFlow 2 (version *2.x.x*):
 
           pip install stardist
 
@@ -108,27 +108,27 @@
 - We provide pre-compiled binaries ("wheels") that should work for most Linux, Windows, and macOS platforms. If you're having problems, please see the [troubleshooting](#installation-1) section below.
 - *(Optional)* You need to install [gputools](https://github.com/maweigert/gputools) if you want to use OpenCL-based computations on the GPU to speed up training.
 - *(Optional)* You might experience improved performance during training if you additionally install the [Multi-Label Anisotropic 3D Euclidean Distance Transform (MLAEDT-3D)](https://github.com/seung-lab/euclidean-distance-transform-3d).
 
 
 ## Usage
 
-We provide example workflows for 2D and 3D via Jupyter [notebooks](https://github.com/stardist/stardist/tree/master/examples) that illustrate how this package can be used.
+We provide example workflows for 2D and 3D via Jupyter [notebooks](https://github.com/stardist/stardist/tree/main/examples) that illustrate how this package can be used.
 
-![](https://github.com/stardist/stardist/raw/master/images/example_steps.png)
+![](https://github.com/stardist/stardist/raw/main/images/example_steps.png)
 
 ### Pretrained Models for 2D
 
 Currently we provide some pretrained models in 2D that might already be suitable for your images:
 
 
 | key | Modality (Staining) | Image format | Example Image    | Description  |
 | :-- | :-: | :-:| :-:| :-- |
-| `2D_versatile_fluo` `2D_paper_dsb2018`| Fluorescence (nuclear marker) | 2D single channel| <img src="https://github.com/stardist/stardist/raw/master/images/example_fluo.jpg" title="example image fluo" width="120px" align="center">       | *Versatile (fluorescent nuclei)* and *DSB 2018 (from StarDist 2D paper)* that were both trained on a [subset of the DSB 2018 nuclei segmentation challenge dataset](https://github.com/stardist/stardist/releases/download/0.1.0/dsb2018.zip). |
-|`2D_versatile_he` | Brightfield (H&E) | 2D RGB  | <img src="https://github.com/stardist/stardist/raw/master/images/example_histo.jpg" title="example image histo" width="120px" align="center">       | *Versatile (H&E nuclei)* that was trained on images from the [MoNuSeg 2018 training data](https://monuseg.grand-challenge.org/Data/) and the [TNBC dataset from Naylor et al. (2018)](https://zenodo.org/record/1175282#.X6mwG9so-CN). |
+| `2D_versatile_fluo` `2D_paper_dsb2018`| Fluorescence (nuclear marker) | 2D single channel| <img src="https://github.com/stardist/stardist/raw/main/images/example_fluo.jpg" title="example image fluo" width="120px" align="center">       | *Versatile (fluorescent nuclei)* and *DSB 2018 (from StarDist 2D paper)* that were both trained on a [subset of the DSB 2018 nuclei segmentation challenge dataset](https://github.com/stardist/stardist/releases/download/0.1.0/dsb2018.zip). |
+|`2D_versatile_he` | Brightfield (H&E) | 2D RGB  | <img src="https://github.com/stardist/stardist/raw/main/images/example_histo.jpg" title="example image histo" width="120px" align="center">       | *Versatile (H&E nuclei)* that was trained on images from the [MoNuSeg 2018 training data](https://monuseg.grand-challenge.org/Data/) and the [TNBC dataset from Naylor et al. (2018)](https://zenodo.org/record/1175282#.X6mwG9so-CN). |
 
 
 You can access these pretrained models from `stardist.models.StarDist2D`
 
 ```python
 from stardist.models import StarDist2D
 
@@ -176,41 +176,41 @@
 
 1. Install [Fiji](https://fiji.sc) and the [Labkit](https://imagej.net/Labkit) plugin
 2. Open the (2D or 3D) image and start Labkit via `Plugins > Labkit > Open Current Image With Labkit`
 3. Successively add a new label and annotate a single cell instance with the brush tool until *all* cells are labeled.  
    (Always disable `allow overlapping labels` or – in older versions of LabKit – enable the `override` option.) 
 4. Export the label image via `Labeling > Save Labeling ...` with `Files of Type > TIF Image` making sure that the file name ends with `.tif` or `.tiff`.
 
-![](https://github.com/stardist/stardist/raw/master/images/labkit_2d_labkit.png)
+![](https://github.com/stardist/stardist/raw/main/images/labkit_2d_labkit.png)
 
 
 Additional tips:
 
 * The Labkit viewer uses [BigDataViewer](https://imagej.net/BigDataViewer) and its keybindings (e.g. <kbd>s</kbd> for contrast options, <kbd>CTRL</kbd>+<kbd>Shift</kbd>+<kbd>mouse-wheel</kbd> for zoom-in/out etc.)
 * For 3D images (XYZ) it is best to first convert it to a (XYT) timeseries (via `Re-Order Hyperstack` and swapping `z` and `t`) and then use <kbd>[</kbd> and <kbd>]</kbd> in Labkit to walk through the slices.
 
 #### Annotating with QuPath (2D)
 
 1. Install [QuPath](https://qupath.github.io/)
 2. Create a new project (`File -> Project...-> Create project`) and add your raw images
 3. Annotate nuclei/objects
-4. Run [this script](https://raw.githubusercontent.com/stardist/stardist/master/extras/qupath_export_annotations.groovy) to export the annotations (save the script and drag it on QuPath. Then execute it with `Run for project`). The script will create a `ground_truth` folder within your QuPath project that includes both the `images` and `masks` subfolder that then can directly be used with *StarDist*.
+4. Run [this script](https://raw.githubusercontent.com/stardist/stardist/main/extras/qupath_export_annotations.groovy) to export the annotations (save the script and drag it on QuPath. Then execute it with `Run for project`). The script will create a `ground_truth` folder within your QuPath project that includes both the `images` and `masks` subfolder that then can directly be used with *StarDist*.
 
-To see how this could be done, have a look at the following [example QuPath project](https://raw.githubusercontent.com/stardist/stardist/master/extras/qupath_example_project.zip) (data courtesy of Romain Guiet, EPFL).
+To see how this could be done, have a look at the following [example QuPath project](https://raw.githubusercontent.com/stardist/stardist/main/extras/qupath_example_project.zip) (data courtesy of Romain Guiet, EPFL).
 
-![](https://github.com/stardist/stardist/raw/master/images/qupath.png)
+![](https://github.com/stardist/stardist/raw/main/images/qupath.png)
 
 
 ### Multi-class Prediction
 
 StarDist also supports multi-class prediction, i.e. each found object instance can additionally be classified into a fixed number of discrete object classes (e.g. cell types):
 
-![](https://github.com/stardist/stardist/raw/master/images/stardist_multiclass.png)
+![](https://github.com/stardist/stardist/raw/main/images/stardist_multiclass.png)
 
-Please see the [multi-class example notebook](https://nbviewer.jupyter.org/github/stardist/stardist/blob/master/examples/other2D/multiclass.ipynb) if you're interested in this.
+Please see the [multi-class example notebook](https://nbviewer.jupyter.org/github/stardist/stardist/blob/main/examples/other2D/multiclass.ipynb) if you're interested in this.
 
 ## Instance segmentation metrics
 
 StarDist contains the `stardist.matching` submodule that provides functions to compute common instance segmentation metrics between ground-truth label masks and predictions (not necessarily from StarDist). Currently available metrics are
 
 * `tp`, `fp`, `fn`
 * `precision`, `recall`, `accuracy`, `f1`
```

### Comparing `stardist-0.9.0/README.md` & `stardist-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 [![Test](https://github.com/stardist/stardist/workflows/Test/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3ATest)
 [![Test (PyPI)](https://github.com/stardist/stardist/workflows/Test%20(PyPI)/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3A%22Test+%28PyPI%29%22)
 [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fstardist.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&suffix=%20topics&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/stardist)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/stardist)](https://pypistats.org/packages/stardist)
 
 # *StarDist* - Object Detection with Star-convex Shapes
 
-![](https://github.com/stardist/stardist/raw/master/images/stardist_overview.png)
+![](https://github.com/stardist/stardist/raw/main/images/stardist_overview.png)
 
 This repository contains the Python implementation of star-convex object detection for 2D and 3D images, as described in the papers:
 
-<img src="https://github.com/stardist/stardist/raw/master/images/stardist_logo.jpg" title="siân is the king of the universe" width="25%" align="right">
+<img src="https://github.com/stardist/stardist/raw/main/images/stardist_logo.jpg" title="siân is the king of the universe" width="25%" align="right">
 
 - Uwe Schmidt, Martin Weigert, Coleman Broaddus, and Gene Myers.  
 [*Cell Detection with Star-convex Polygons*](https://arxiv.org/abs/1806.03535).  
 International Conference on Medical Image Computing and Computer-Assisted Intervention (MICCAI), Granada, Spain, September 2018.
 
 - Martin Weigert, Uwe Schmidt, Robert Haase, Ko Sugawara, and Gene Myers.  
 [*Star-convex Polyhedra for 3D Object Detection and Segmentation in Microscopy*](http://openaccess.thecvf.com/content_WACV_2020/papers/Weigert_Star-convex_Polyhedra_for_3D_Object_Detection_and_Segmentation_in_Microscopy_WACV_2020_paper.pdf).  
@@ -25,19 +25,19 @@
 
 
 ## Overview
 
 The following figure illustrates the general approach for 2D images. The training data consists of corresponding pairs of input (i.e. raw) images and fully annotated label images (i.e. every pixel is labeled with a unique object id or 0 for background).
 A model is trained to densely predict the distances (r) to the object boundary along a fixed set of rays and object probabilities (d), which together produce an overcomplete set of candidate polygons for a given input image. The final result is obtained via non-maximum suppression (NMS) of these candidates.
 
-![](https://github.com/stardist/stardist/raw/master/images/overview_2d.png)
+![](https://github.com/stardist/stardist/raw/main/images/overview_2d.png)
 
 The approach for 3D volumes is similar to the one described for 2D, using pairs of input and fully annotated label volumes as training data.
 
-![](https://github.com/stardist/stardist/raw/master/images/overview_3d.png)
+![](https://github.com/stardist/stardist/raw/main/images/overview_3d.png)
 
 ## Webinar/Tutorial
 
 If you want to know more about the concepts and practical applications of StarDist, please have a look at the following webinar that was given at NEUBIAS Academy @Home 2020:
 
 [![webinar video](http://img.youtube.com/vi/Amn_eHRGX5M/0.jpg)](http://www.youtube.com/watch?v=Amn_eHRGX5M "Webinar")
 
@@ -48,15 +48,15 @@
 
 If you only want to use a StarDist plugin for a GUI-based software, please read [this](#plugins-for-other-software).
 
 1. Please first [install TensorFlow](https://www.tensorflow.org/install)
 (either TensorFlow 1 or 2) by following the official instructions.
 For [GPU support](https://www.tensorflow.org/install/gpu), it is very
 important to install the specific versions of CUDA and cuDNN that are
-compatible with the respective version of TensorFlow. (If you need help and can use `conda`, take a look at [this](https://github.com/CSBDeep/CSBDeep/tree/master/extras#conda-environment).)
+compatible with the respective version of TensorFlow. (If you need help and can use `conda`, take a look at [this](https://github.com/CSBDeep/CSBDeep/tree/main/extras#conda-environment).)
 
 2. *StarDist* can then be installed with `pip`:
 
     - If you installed TensorFlow 2 (version *2.x.x*):
 
           pip install stardist
 
@@ -72,27 +72,27 @@
 - We provide pre-compiled binaries ("wheels") that should work for most Linux, Windows, and macOS platforms. If you're having problems, please see the [troubleshooting](#installation-1) section below.
 - *(Optional)* You need to install [gputools](https://github.com/maweigert/gputools) if you want to use OpenCL-based computations on the GPU to speed up training.
 - *(Optional)* You might experience improved performance during training if you additionally install the [Multi-Label Anisotropic 3D Euclidean Distance Transform (MLAEDT-3D)](https://github.com/seung-lab/euclidean-distance-transform-3d).
 
 
 ## Usage
 
-We provide example workflows for 2D and 3D via Jupyter [notebooks](https://github.com/stardist/stardist/tree/master/examples) that illustrate how this package can be used.
+We provide example workflows for 2D and 3D via Jupyter [notebooks](https://github.com/stardist/stardist/tree/main/examples) that illustrate how this package can be used.
 
-![](https://github.com/stardist/stardist/raw/master/images/example_steps.png)
+![](https://github.com/stardist/stardist/raw/main/images/example_steps.png)
 
 ### Pretrained Models for 2D
 
 Currently we provide some pretrained models in 2D that might already be suitable for your images:
 
 
 | key | Modality (Staining) | Image format | Example Image    | Description  |
 | :-- | :-: | :-:| :-:| :-- |
-| `2D_versatile_fluo` `2D_paper_dsb2018`| Fluorescence (nuclear marker) | 2D single channel| <img src="https://github.com/stardist/stardist/raw/master/images/example_fluo.jpg" title="example image fluo" width="120px" align="center">       | *Versatile (fluorescent nuclei)* and *DSB 2018 (from StarDist 2D paper)* that were both trained on a [subset of the DSB 2018 nuclei segmentation challenge dataset](https://github.com/stardist/stardist/releases/download/0.1.0/dsb2018.zip). |
-|`2D_versatile_he` | Brightfield (H&E) | 2D RGB  | <img src="https://github.com/stardist/stardist/raw/master/images/example_histo.jpg" title="example image histo" width="120px" align="center">       | *Versatile (H&E nuclei)* that was trained on images from the [MoNuSeg 2018 training data](https://monuseg.grand-challenge.org/Data/) and the [TNBC dataset from Naylor et al. (2018)](https://zenodo.org/record/1175282#.X6mwG9so-CN). |
+| `2D_versatile_fluo` `2D_paper_dsb2018`| Fluorescence (nuclear marker) | 2D single channel| <img src="https://github.com/stardist/stardist/raw/main/images/example_fluo.jpg" title="example image fluo" width="120px" align="center">       | *Versatile (fluorescent nuclei)* and *DSB 2018 (from StarDist 2D paper)* that were both trained on a [subset of the DSB 2018 nuclei segmentation challenge dataset](https://github.com/stardist/stardist/releases/download/0.1.0/dsb2018.zip). |
+|`2D_versatile_he` | Brightfield (H&E) | 2D RGB  | <img src="https://github.com/stardist/stardist/raw/main/images/example_histo.jpg" title="example image histo" width="120px" align="center">       | *Versatile (H&E nuclei)* that was trained on images from the [MoNuSeg 2018 training data](https://monuseg.grand-challenge.org/Data/) and the [TNBC dataset from Naylor et al. (2018)](https://zenodo.org/record/1175282#.X6mwG9so-CN). |
 
 
 You can access these pretrained models from `stardist.models.StarDist2D`
 
 ```python
 from stardist.models import StarDist2D
 
@@ -140,41 +140,41 @@
 
 1. Install [Fiji](https://fiji.sc) and the [Labkit](https://imagej.net/Labkit) plugin
 2. Open the (2D or 3D) image and start Labkit via `Plugins > Labkit > Open Current Image With Labkit`
 3. Successively add a new label and annotate a single cell instance with the brush tool until *all* cells are labeled.  
    (Always disable `allow overlapping labels` or – in older versions of LabKit – enable the `override` option.) 
 4. Export the label image via `Labeling > Save Labeling ...` with `Files of Type > TIF Image` making sure that the file name ends with `.tif` or `.tiff`.
 
-![](https://github.com/stardist/stardist/raw/master/images/labkit_2d_labkit.png)
+![](https://github.com/stardist/stardist/raw/main/images/labkit_2d_labkit.png)
 
 
 Additional tips:
 
 * The Labkit viewer uses [BigDataViewer](https://imagej.net/BigDataViewer) and its keybindings (e.g. <kbd>s</kbd> for contrast options, <kbd>CTRL</kbd>+<kbd>Shift</kbd>+<kbd>mouse-wheel</kbd> for zoom-in/out etc.)
 * For 3D images (XYZ) it is best to first convert it to a (XYT) timeseries (via `Re-Order Hyperstack` and swapping `z` and `t`) and then use <kbd>[</kbd> and <kbd>]</kbd> in Labkit to walk through the slices.
 
 #### Annotating with QuPath (2D)
 
 1. Install [QuPath](https://qupath.github.io/)
 2. Create a new project (`File -> Project...-> Create project`) and add your raw images
 3. Annotate nuclei/objects
-4. Run [this script](https://raw.githubusercontent.com/stardist/stardist/master/extras/qupath_export_annotations.groovy) to export the annotations (save the script and drag it on QuPath. Then execute it with `Run for project`). The script will create a `ground_truth` folder within your QuPath project that includes both the `images` and `masks` subfolder that then can directly be used with *StarDist*.
+4. Run [this script](https://raw.githubusercontent.com/stardist/stardist/main/extras/qupath_export_annotations.groovy) to export the annotations (save the script and drag it on QuPath. Then execute it with `Run for project`). The script will create a `ground_truth` folder within your QuPath project that includes both the `images` and `masks` subfolder that then can directly be used with *StarDist*.
 
-To see how this could be done, have a look at the following [example QuPath project](https://raw.githubusercontent.com/stardist/stardist/master/extras/qupath_example_project.zip) (data courtesy of Romain Guiet, EPFL).
+To see how this could be done, have a look at the following [example QuPath project](https://raw.githubusercontent.com/stardist/stardist/main/extras/qupath_example_project.zip) (data courtesy of Romain Guiet, EPFL).
 
-![](https://github.com/stardist/stardist/raw/master/images/qupath.png)
+![](https://github.com/stardist/stardist/raw/main/images/qupath.png)
 
 
 ### Multi-class Prediction
 
 StarDist also supports multi-class prediction, i.e. each found object instance can additionally be classified into a fixed number of discrete object classes (e.g. cell types):
 
-![](https://github.com/stardist/stardist/raw/master/images/stardist_multiclass.png)
+![](https://github.com/stardist/stardist/raw/main/images/stardist_multiclass.png)
 
-Please see the [multi-class example notebook](https://nbviewer.jupyter.org/github/stardist/stardist/blob/master/examples/other2D/multiclass.ipynb) if you're interested in this.
+Please see the [multi-class example notebook](https://nbviewer.jupyter.org/github/stardist/stardist/blob/main/examples/other2D/multiclass.ipynb) if you're interested in this.
 
 ## Instance segmentation metrics
 
 StarDist contains the `stardist.matching` submodule that provides functions to compute common instance segmentation metrics between ground-truth label masks and predictions (not necessarily from StarDist). Currently available metrics are
 
 * `tp`, `fp`, `fn`
 * `precision`, `recall`, `accuracy`, `f1`
```

### Comparing `stardist-0.9.0/setup.py` & `stardist-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/__init__.py` & `stardist-0.9.1/stardist/__init__.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/big.py` & `stardist-0.9.1/stardist/big.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/bioimageio_utils.py` & `stardist-0.9.1/stardist/bioimageio_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             'cells', 'nuclei', # content
             'tensorflow', # framework
             'fiji', # software
             'unet', # network
             'instance-segmentation', 'object-detection', # task
             'stardist',
         ],
-        covers=["https://raw.githubusercontent.com/stardist/stardist/master/images/stardist_logo.jpg"],
+        covers=["https://raw.githubusercontent.com/stardist/stardist/main/images/stardist_logo.jpg"],
         documentation=_create_stardist_doc(outdir),
     )
     if generate_default_deps:  # only if requested, as not required for bioimage.io
         data['dependencies'] = _create_stardist_dependencies(outdir)
 
     return data
```

### Comparing `stardist-0.9.0/stardist/data/__init__.py` & `stardist-0.9.1/stardist/data/__init__.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/data/images/histo.jpg` & `stardist-0.9.1/stardist/data/images/histo.jpg`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/data/images/img2d.tif` & `stardist-0.9.1/stardist/data/images/img2d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/data/images/img3d.tif` & `stardist-0.9.1/stardist/data/images/img3d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/data/images/mask2d.tif` & `stardist-0.9.1/stardist/data/images/mask2d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/data/images/mask3d.tif` & `stardist-0.9.1/stardist/data/images/mask3d.tif`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/geometry/geom2d.py` & `stardist-0.9.1/stardist/geometry/geom2d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/geometry/geom3d.py` & `stardist-0.9.1/stardist/geometry/geom3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/kernels/stardist2d.cl` & `stardist-0.9.1/stardist/kernels/stardist2d.cl`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/kernels/stardist3d.cl` & `stardist-0.9.1/stardist/kernels/stardist3d.cl`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/clipper/LICENSE.txt` & `stardist-0.9.1/stardist/lib/external/clipper/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/clipper/clipper.cpp` & `stardist-0.9.1/stardist/lib/external/clipper/clipper.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/clipper/clipper.hpp` & `stardist-0.9.1/stardist/lib/external/clipper/clipper.hpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/nanoflann/LICENSE.txt` & `stardist-0.9.1/stardist/lib/external/nanoflann/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/nanoflann/nanoflann.hpp` & `stardist-0.9.1/stardist/lib/external/nanoflann/nanoflann.hpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/Announce.txt` & `stardist-0.9.1/stardist/lib/external/qhull_src/Announce.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/COPYING.txt` & `stardist-0.9.1/stardist/lib/external/qhull_src/COPYING.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/README.txt` & `stardist-0.9.1/stardist/lib/external/qhull_src/README.txt`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/geom2_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/geom_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/global_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/io_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/io_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/libqhull_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/mem_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/merge_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/poly2_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/poly_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/qhull_ra.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/qset_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/random_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/random_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/rboxlib_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/stat_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/user_r.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhull_r/user_r.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/Coordinates.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/PointCoordinates.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/Qhull.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullError.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetList.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullFacetSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullHyperplane.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullIterator.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullLinkedList.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoint.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPointSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullPoints.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullQh.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullRidge.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullSets.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullStat.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertex.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/QhullVertexSet.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RboxPoints.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RoadError.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/RoadLogEvent.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/functionObjects.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp` & `stardist-0.9.1/stardist/lib/external/qhull_src/src/libqhullcpp/usermem_r-cpp.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/stardist2d.cpp` & `stardist-0.9.1/stardist/lib/stardist2d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/stardist3d.cpp` & `stardist-0.9.1/stardist/lib/stardist3d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/stardist3d_impl.cpp` & `stardist-0.9.1/stardist/lib/stardist3d_impl.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/stardist3d_impl.h` & `stardist-0.9.1/stardist/lib/stardist3d_impl.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/stardist3d_lib.c` & `stardist-0.9.1/stardist/lib/stardist3d_lib.c`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/stardist3d_lib.h` & `stardist-0.9.1/stardist/lib/stardist3d_lib.h`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/test_lib3d.cpp` & `stardist-0.9.1/stardist/lib/test_lib3d.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/lib/utils.cpp` & `stardist-0.9.1/stardist/lib/utils.cpp`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/matching.py` & `stardist-0.9.1/stardist/matching.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/models/__init__.py` & `stardist-0.9.1/stardist/models/__init__.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/models/base.py` & `stardist-0.9.1/stardist/models/base.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/models/model2d.py` & `stardist-0.9.1/stardist/models/model2d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/models/model3d.py` & `stardist-0.9.1/stardist/models/model3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/nms.py` & `stardist-0.9.1/stardist/nms.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/plot/plot.py` & `stardist-0.9.1/stardist/plot/plot.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/plot/render.py` & `stardist-0.9.1/stardist/plot/render.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/rays3d.py` & `stardist-0.9.1/stardist/rays3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/sample_patches.py` & `stardist-0.9.1/stardist/sample_patches.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/scripts/predict2d.py` & `stardist-0.9.1/stardist/scripts/predict2d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/scripts/predict3d.py` & `stardist-0.9.1/stardist/scripts/predict3d.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist/utils.py` & `stardist-0.9.1/stardist/utils.py`

 * *Files identical despite different names*

### Comparing `stardist-0.9.0/stardist.egg-info/PKG-INFO` & `stardist-0.9.1/stardist.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stardist
-Version: 0.9.0
+Version: 0.9.1
 Summary: StarDist - Object Detection with Star-convex Shapes
 Home-page: https://github.com/stardist/stardist
 Author: Uwe Schmidt, Martin Weigert
 Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -39,19 +39,19 @@
 [![Test](https://github.com/stardist/stardist/workflows/Test/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3ATest)
 [![Test (PyPI)](https://github.com/stardist/stardist/workflows/Test%20(PyPI)/badge.svg)](https://github.com/stardist/stardist/actions?query=workflow%3A%22Test+%28PyPI%29%22)
 [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fstardist.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&suffix=%20topics&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/stardist)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/stardist)](https://pypistats.org/packages/stardist)
 
 # *StarDist* - Object Detection with Star-convex Shapes
 
-![](https://github.com/stardist/stardist/raw/master/images/stardist_overview.png)
+![](https://github.com/stardist/stardist/raw/main/images/stardist_overview.png)
 
 This repository contains the Python implementation of star-convex object detection for 2D and 3D images, as described in the papers:
 
-<img src="https://github.com/stardist/stardist/raw/master/images/stardist_logo.jpg" title="siân is the king of the universe" width="25%" align="right">
+<img src="https://github.com/stardist/stardist/raw/main/images/stardist_logo.jpg" title="siân is the king of the universe" width="25%" align="right">
 
 - Uwe Schmidt, Martin Weigert, Coleman Broaddus, and Gene Myers.  
 [*Cell Detection with Star-convex Polygons*](https://arxiv.org/abs/1806.03535).  
 International Conference on Medical Image Computing and Computer-Assisted Intervention (MICCAI), Granada, Spain, September 2018.
 
 - Martin Weigert, Uwe Schmidt, Robert Haase, Ko Sugawara, and Gene Myers.  
 [*Star-convex Polyhedra for 3D Object Detection and Segmentation in Microscopy*](http://openaccess.thecvf.com/content_WACV_2020/papers/Weigert_Star-convex_Polyhedra_for_3D_Object_Detection_and_Segmentation_in_Microscopy_WACV_2020_paper.pdf).  
@@ -61,19 +61,19 @@
 
 
 ## Overview
 
 The following figure illustrates the general approach for 2D images. The training data consists of corresponding pairs of input (i.e. raw) images and fully annotated label images (i.e. every pixel is labeled with a unique object id or 0 for background).
 A model is trained to densely predict the distances (r) to the object boundary along a fixed set of rays and object probabilities (d), which together produce an overcomplete set of candidate polygons for a given input image. The final result is obtained via non-maximum suppression (NMS) of these candidates.
 
-![](https://github.com/stardist/stardist/raw/master/images/overview_2d.png)
+![](https://github.com/stardist/stardist/raw/main/images/overview_2d.png)
 
 The approach for 3D volumes is similar to the one described for 2D, using pairs of input and fully annotated label volumes as training data.
 
-![](https://github.com/stardist/stardist/raw/master/images/overview_3d.png)
+![](https://github.com/stardist/stardist/raw/main/images/overview_3d.png)
 
 ## Webinar/Tutorial
 
 If you want to know more about the concepts and practical applications of StarDist, please have a look at the following webinar that was given at NEUBIAS Academy @Home 2020:
 
 [![webinar video](http://img.youtube.com/vi/Amn_eHRGX5M/0.jpg)](http://www.youtube.com/watch?v=Amn_eHRGX5M "Webinar")
 
@@ -84,15 +84,15 @@
 
 If you only want to use a StarDist plugin for a GUI-based software, please read [this](#plugins-for-other-software).
 
 1. Please first [install TensorFlow](https://www.tensorflow.org/install)
 (either TensorFlow 1 or 2) by following the official instructions.
 For [GPU support](https://www.tensorflow.org/install/gpu), it is very
 important to install the specific versions of CUDA and cuDNN that are
-compatible with the respective version of TensorFlow. (If you need help and can use `conda`, take a look at [this](https://github.com/CSBDeep/CSBDeep/tree/master/extras#conda-environment).)
+compatible with the respective version of TensorFlow. (If you need help and can use `conda`, take a look at [this](https://github.com/CSBDeep/CSBDeep/tree/main/extras#conda-environment).)
 
 2. *StarDist* can then be installed with `pip`:
 
     - If you installed TensorFlow 2 (version *2.x.x*):
 
           pip install stardist
 
@@ -108,27 +108,27 @@
 - We provide pre-compiled binaries ("wheels") that should work for most Linux, Windows, and macOS platforms. If you're having problems, please see the [troubleshooting](#installation-1) section below.
 - *(Optional)* You need to install [gputools](https://github.com/maweigert/gputools) if you want to use OpenCL-based computations on the GPU to speed up training.
 - *(Optional)* You might experience improved performance during training if you additionally install the [Multi-Label Anisotropic 3D Euclidean Distance Transform (MLAEDT-3D)](https://github.com/seung-lab/euclidean-distance-transform-3d).
 
 
 ## Usage
 
-We provide example workflows for 2D and 3D via Jupyter [notebooks](https://github.com/stardist/stardist/tree/master/examples) that illustrate how this package can be used.
+We provide example workflows for 2D and 3D via Jupyter [notebooks](https://github.com/stardist/stardist/tree/main/examples) that illustrate how this package can be used.
 
-![](https://github.com/stardist/stardist/raw/master/images/example_steps.png)
+![](https://github.com/stardist/stardist/raw/main/images/example_steps.png)
 
 ### Pretrained Models for 2D
 
 Currently we provide some pretrained models in 2D that might already be suitable for your images:
 
 
 | key | Modality (Staining) | Image format | Example Image    | Description  |
 | :-- | :-: | :-:| :-:| :-- |
-| `2D_versatile_fluo` `2D_paper_dsb2018`| Fluorescence (nuclear marker) | 2D single channel| <img src="https://github.com/stardist/stardist/raw/master/images/example_fluo.jpg" title="example image fluo" width="120px" align="center">       | *Versatile (fluorescent nuclei)* and *DSB 2018 (from StarDist 2D paper)* that were both trained on a [subset of the DSB 2018 nuclei segmentation challenge dataset](https://github.com/stardist/stardist/releases/download/0.1.0/dsb2018.zip). |
-|`2D_versatile_he` | Brightfield (H&E) | 2D RGB  | <img src="https://github.com/stardist/stardist/raw/master/images/example_histo.jpg" title="example image histo" width="120px" align="center">       | *Versatile (H&E nuclei)* that was trained on images from the [MoNuSeg 2018 training data](https://monuseg.grand-challenge.org/Data/) and the [TNBC dataset from Naylor et al. (2018)](https://zenodo.org/record/1175282#.X6mwG9so-CN). |
+| `2D_versatile_fluo` `2D_paper_dsb2018`| Fluorescence (nuclear marker) | 2D single channel| <img src="https://github.com/stardist/stardist/raw/main/images/example_fluo.jpg" title="example image fluo" width="120px" align="center">       | *Versatile (fluorescent nuclei)* and *DSB 2018 (from StarDist 2D paper)* that were both trained on a [subset of the DSB 2018 nuclei segmentation challenge dataset](https://github.com/stardist/stardist/releases/download/0.1.0/dsb2018.zip). |
+|`2D_versatile_he` | Brightfield (H&E) | 2D RGB  | <img src="https://github.com/stardist/stardist/raw/main/images/example_histo.jpg" title="example image histo" width="120px" align="center">       | *Versatile (H&E nuclei)* that was trained on images from the [MoNuSeg 2018 training data](https://monuseg.grand-challenge.org/Data/) and the [TNBC dataset from Naylor et al. (2018)](https://zenodo.org/record/1175282#.X6mwG9so-CN). |
 
 
 You can access these pretrained models from `stardist.models.StarDist2D`
 
 ```python
 from stardist.models import StarDist2D
 
@@ -176,41 +176,41 @@
 
 1. Install [Fiji](https://fiji.sc) and the [Labkit](https://imagej.net/Labkit) plugin
 2. Open the (2D or 3D) image and start Labkit via `Plugins > Labkit > Open Current Image With Labkit`
 3. Successively add a new label and annotate a single cell instance with the brush tool until *all* cells are labeled.  
    (Always disable `allow overlapping labels` or – in older versions of LabKit – enable the `override` option.) 
 4. Export the label image via `Labeling > Save Labeling ...` with `Files of Type > TIF Image` making sure that the file name ends with `.tif` or `.tiff`.
 
-![](https://github.com/stardist/stardist/raw/master/images/labkit_2d_labkit.png)
+![](https://github.com/stardist/stardist/raw/main/images/labkit_2d_labkit.png)
 
 
 Additional tips:
 
 * The Labkit viewer uses [BigDataViewer](https://imagej.net/BigDataViewer) and its keybindings (e.g. <kbd>s</kbd> for contrast options, <kbd>CTRL</kbd>+<kbd>Shift</kbd>+<kbd>mouse-wheel</kbd> for zoom-in/out etc.)
 * For 3D images (XYZ) it is best to first convert it to a (XYT) timeseries (via `Re-Order Hyperstack` and swapping `z` and `t`) and then use <kbd>[</kbd> and <kbd>]</kbd> in Labkit to walk through the slices.
 
 #### Annotating with QuPath (2D)
 
 1. Install [QuPath](https://qupath.github.io/)
 2. Create a new project (`File -> Project...-> Create project`) and add your raw images
 3. Annotate nuclei/objects
-4. Run [this script](https://raw.githubusercontent.com/stardist/stardist/master/extras/qupath_export_annotations.groovy) to export the annotations (save the script and drag it on QuPath. Then execute it with `Run for project`). The script will create a `ground_truth` folder within your QuPath project that includes both the `images` and `masks` subfolder that then can directly be used with *StarDist*.
+4. Run [this script](https://raw.githubusercontent.com/stardist/stardist/main/extras/qupath_export_annotations.groovy) to export the annotations (save the script and drag it on QuPath. Then execute it with `Run for project`). The script will create a `ground_truth` folder within your QuPath project that includes both the `images` and `masks` subfolder that then can directly be used with *StarDist*.
 
-To see how this could be done, have a look at the following [example QuPath project](https://raw.githubusercontent.com/stardist/stardist/master/extras/qupath_example_project.zip) (data courtesy of Romain Guiet, EPFL).
+To see how this could be done, have a look at the following [example QuPath project](https://raw.githubusercontent.com/stardist/stardist/main/extras/qupath_example_project.zip) (data courtesy of Romain Guiet, EPFL).
 
-![](https://github.com/stardist/stardist/raw/master/images/qupath.png)
+![](https://github.com/stardist/stardist/raw/main/images/qupath.png)
 
 
 ### Multi-class Prediction
 
 StarDist also supports multi-class prediction, i.e. each found object instance can additionally be classified into a fixed number of discrete object classes (e.g. cell types):
 
-![](https://github.com/stardist/stardist/raw/master/images/stardist_multiclass.png)
+![](https://github.com/stardist/stardist/raw/main/images/stardist_multiclass.png)
 
-Please see the [multi-class example notebook](https://nbviewer.jupyter.org/github/stardist/stardist/blob/master/examples/other2D/multiclass.ipynb) if you're interested in this.
+Please see the [multi-class example notebook](https://nbviewer.jupyter.org/github/stardist/stardist/blob/main/examples/other2D/multiclass.ipynb) if you're interested in this.
 
 ## Instance segmentation metrics
 
 StarDist contains the `stardist.matching` submodule that provides functions to compute common instance segmentation metrics between ground-truth label masks and predictions (not necessarily from StarDist). Currently available metrics are
 
 * `tp`, `fp`, `fn`
 * `precision`, `recall`, `accuracy`, `f1`
```

### Comparing `stardist-0.9.0/stardist.egg-info/SOURCES.txt` & `stardist-0.9.1/stardist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

