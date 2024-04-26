# Comparing `tmp/PyQt6_DataVisualization-6.6.0.tar.gz` & `tmp/PyQt6_DataVisualization-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_DataVisualization-6.6.0.tar", last modified: Wed Oct 25 10:23:48 2023, max compression
+gzip compressed data, was "PyQt6_DataVisualization-6.7.0.tar", last modified: Sat Apr 20 16:02:30 2024, max compression
```

## Comparing `PyQt6_DataVisualization-6.6.0.tar` & `PyQt6_DataVisualization-6.7.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.172460 PyQt6_DataVisualization-6.6.0/
--rw-r--r--   0 phil       (501) staff       (20)     4623 2023-10-25 10:23:47.479840 PyQt6_DataVisualization-6.6.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2023-10-25 10:23:47.276791 PyQt6_DataVisualization-6.6.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      434 2023-10-25 10:22:51.793457 PyQt6_DataVisualization-6.6.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1711 2023-10-25 10:23:48.172622 PyQt6_DataVisualization-6.6.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1354 2023-10-25 10:23:47.481186 PyQt6_DataVisualization-6.6.0/README
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.153632 PyQt6_DataVisualization-6.6.0/examples/
--rwxr-xr-x   0 phil       (501) staff       (20)    17259 2023-10-25 10:22:51.799424 PyQt6_DataVisualization-6.6.0/examples/bars.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.149937 PyQt6_DataVisualization-6.6.0/examples/custominput/
--rwxr-xr-x   0 phil       (501) staff       (20)     7671 2023-10-25 10:22:51.800866 PyQt6_DataVisualization-6.6.0/examples/custominput/custominput.py
--rw-r--r--   0 phil       (501) staff       (20)    28985 2023-10-25 10:22:51.802598 PyQt6_DataVisualization-6.6.0/examples/custominput/data.txt
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.152300 PyQt6_DataVisualization-6.6.0/examples/customproxy/
--rwxr-xr-x   0 phil       (501) staff       (20)     9930 2023-10-25 10:22:51.803643 PyQt6_DataVisualization-6.6.0/examples/customproxy/customproxy.py
--rw-r--r--   0 phil       (501) staff       (20)     1995 2023-10-25 10:22:51.804502 PyQt6_DataVisualization-6.6.0/examples/customproxy/raindata.txt
--rwxr-xr-x   0 phil       (501) staff       (20)     5944 2023-10-25 10:22:51.805314 PyQt6_DataVisualization-6.6.0/examples/itemmodel.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.150808 PyQt6_DataVisualization-6.6.0/examples/rotations/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.151357 PyQt6_DataVisualization-6.6.0/examples/rotations/mesh/
--rw-r--r--   0 phil       (501) staff       (20)    59358 2023-10-25 10:22:51.807147 PyQt6_DataVisualization-6.6.0/examples/rotations/mesh/largesphere.obj
--rw-r--r--   0 phil       (501) staff       (20)    11371 2023-10-25 10:22:51.808099 PyQt6_DataVisualization-6.6.0/examples/rotations/mesh/narrowarrow.obj
--rwxr-xr-x   0 phil       (501) staff       (20)     8199 2023-10-25 10:22:51.808909 PyQt6_DataVisualization-6.6.0/examples/rotations/rotations.py
--rwxr-xr-x   0 phil       (501) staff       (20)     9599 2023-10-25 10:22:51.809722 PyQt6_DataVisualization-6.6.0/examples/scatter.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.153252 PyQt6_DataVisualization-6.6.0/examples/surface/
--rw-r--r--   0 phil       (501) staff       (20)    34540 2023-10-25 10:22:51.810702 PyQt6_DataVisualization-6.6.0/examples/surface/mountain.png
--rwxr-xr-x   0 phil       (501) staff       (20)    14938 2023-10-25 10:22:51.811573 PyQt6_DataVisualization-6.6.0/examples/surface/surface.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.154172 PyQt6_DataVisualization-6.6.0/examples/volumetric/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.155300 PyQt6_DataVisualization-6.6.0/examples/volumetric/heightmaps/
--rw-r--r--   0 phil       (501) staff       (20)    62477 2023-10-25 10:22:51.813540 PyQt6_DataVisualization-6.6.0/examples/volumetric/heightmaps/layer_ground.png
--rw-r--r--   0 phil       (501) staff       (20)    16550 2023-10-25 10:22:51.814978 PyQt6_DataVisualization-6.6.0/examples/volumetric/heightmaps/layer_magma.png
--rw-r--r--   0 phil       (501) staff       (20)    10181 2023-10-25 10:22:51.816430 PyQt6_DataVisualization-6.6.0/examples/volumetric/heightmaps/layer_water.png
--rwxr-xr-x   0 phil       (501) staff       (20)    36700 2023-10-25 10:22:51.817990 PyQt6_DataVisualization-6.6.0/examples/volumetric/volumetric.py
--rw-r--r--   0 phil       (501) staff       (20)      861 2023-10-25 10:23:47.481643 PyQt6_DataVisualization-6.6.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.155978 PyQt6_DataVisualization-6.6.0/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:23:48.172139 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/
--rw-r--r--   0 phil       (501) staff       (20)     3471 2023-10-25 10:23:47.920319 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/QtDataVisualizationmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3181 2023-10-25 10:23:47.929124 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dbars.sip
--rw-r--r--   0 phil       (501) staff       (20)     3278 2023-10-25 10:23:47.922781 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dcamera.sip
--rw-r--r--   0 phil       (501) staff       (20)     1988 2023-10-25 10:23:47.917433 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dinputhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     1272 2023-10-25 10:23:47.931946 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dlight.sip
--rw-r--r--   0 phil       (501) staff       (20)     1449 2023-10-25 10:23:47.934192 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     1997 2023-10-25 10:23:47.920925 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dscatter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2763 2023-10-25 10:23:47.926162 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dscene.sip
--rw-r--r--   0 phil       (501) staff       (20)     2143 2023-10-25 10:23:47.928318 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dsurface.sip
--rw-r--r--   0 phil       (501) staff       (20)     7480 2023-10-25 10:23:47.913426 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dtheme.sip
--rw-r--r--   0 phil       (501) staff       (20)     2550 2023-10-25 10:23:47.914379 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qabstract3daxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     6233 2023-10-25 10:23:47.930308 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qabstract3dgraph.sip
--rw-r--r--   0 phil       (501) staff       (20)     2344 2023-10-25 10:23:47.911472 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qabstract3dinputhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     3949 2023-10-25 10:23:47.927012 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qabstract3dseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1314 2023-10-25 10:23:47.918726 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qabstractdataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     1987 2023-10-25 10:23:47.918074 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qbar3dseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1343 2023-10-25 10:23:47.936215 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qbardataitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     3390 2023-10-25 10:23:47.919518 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qbardataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     1302 2023-10-25 10:23:47.933676 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qcategory3daxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     2692 2023-10-25 10:23:47.910786 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qcustom3ditem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2209 2023-10-25 10:23:47.934797 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qcustom3dlabel.sip
--rw-r--r--   0 phil       (501) staff       (20)     7271 2023-10-25 10:23:47.924359 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qcustom3dvolume.sip
--rw-r--r--   0 phil       (501) staff       (20)     2871 2023-10-25 10:23:47.936990 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qheightmapsurfacedataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     5828 2023-10-25 10:23:47.910006 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qitemmodelbardataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     3934 2023-10-25 10:23:47.935639 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qitemmodelscatterdataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     6348 2023-10-25 10:23:47.921913 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qitemmodelsurfacedataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     4388 2023-10-25 10:23:47.933191 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1849 2023-10-25 10:23:47.930883 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qlogvalue3daxisformatter.sip
--rw-r--r--   0 phil       (501) staff       (20)     1706 2023-10-25 10:23:47.916192 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qscatter3dseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1616 2023-10-25 10:23:47.925493 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qscatterdataitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2190 2023-10-25 10:23:47.931462 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qscatterdataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     2766 2023-10-25 10:23:47.927738 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qsurface3dseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1453 2023-10-25 10:23:47.915608 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qsurfacedataitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2615 2023-10-25 10:23:47.916841 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qsurfacedataproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     1261 2023-10-25 10:23:47.937511 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qtouch3dinputhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     1068 2023-10-25 10:23:47.912066 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qutils.sip
--rw-r--r--   0 phil       (501) staff       (20)     1835 2023-10-25 10:23:47.924953 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qvalue3daxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     2019 2023-10-25 10:23:47.915027 PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qvalue3daxisformatter.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.845211 PyQt6_DataVisualization-6.7.0/
+-rw-r--r--   0 phil       (501) staff       (20)     5430 2024-04-20 16:02:30.630119 PyQt6_DataVisualization-6.7.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2024-04-20 16:02:30.535800 PyQt6_DataVisualization-6.7.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      488 2024-04-20 16:01:59.781825 PyQt6_DataVisualization-6.7.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1637 2024-04-20 16:02:30.845276 PyQt6_DataVisualization-6.7.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1234 2024-04-20 16:02:30.630741 PyQt6_DataVisualization-6.7.0/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.837897 PyQt6_DataVisualization-6.7.0/examples/
+-rwxr-xr-x   0 phil       (501) staff       (20)    17259 2024-04-20 16:01:59.783967 PyQt6_DataVisualization-6.7.0/examples/bars.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.836220 PyQt6_DataVisualization-6.7.0/examples/custominput/
+-rwxr-xr-x   0 phil       (501) staff       (20)     7671 2024-04-20 16:01:59.784290 PyQt6_DataVisualization-6.7.0/examples/custominput/custominput.py
+-rw-r--r--   0 phil       (501) staff       (20)    28985 2024-04-20 16:01:59.784768 PyQt6_DataVisualization-6.7.0/examples/custominput/data.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.837300 PyQt6_DataVisualization-6.7.0/examples/customproxy/
+-rwxr-xr-x   0 phil       (501) staff       (20)     9930 2024-04-20 16:01:59.785043 PyQt6_DataVisualization-6.7.0/examples/customproxy/customproxy.py
+-rw-r--r--   0 phil       (501) staff       (20)     1995 2024-04-20 16:01:59.785257 PyQt6_DataVisualization-6.7.0/examples/customproxy/raindata.txt
+-rwxr-xr-x   0 phil       (501) staff       (20)     5944 2024-04-20 16:01:59.785450 PyQt6_DataVisualization-6.7.0/examples/itemmodel.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.836660 PyQt6_DataVisualization-6.7.0/examples/rotations/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.836895 PyQt6_DataVisualization-6.7.0/examples/rotations/mesh/
+-rw-r--r--   0 phil       (501) staff       (20)    59358 2024-04-20 16:01:59.786018 PyQt6_DataVisualization-6.7.0/examples/rotations/mesh/largesphere.obj
+-rw-r--r--   0 phil       (501) staff       (20)    11371 2024-04-20 16:01:59.786253 PyQt6_DataVisualization-6.7.0/examples/rotations/mesh/narrowarrow.obj
+-rwxr-xr-x   0 phil       (501) staff       (20)     8199 2024-04-20 16:01:59.786458 PyQt6_DataVisualization-6.7.0/examples/rotations/rotations.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     9599 2024-04-20 16:01:59.786686 PyQt6_DataVisualization-6.7.0/examples/scatter.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.837720 PyQt6_DataVisualization-6.7.0/examples/surface/
+-rw-r--r--   0 phil       (501) staff       (20)    34540 2024-04-20 16:01:59.787149 PyQt6_DataVisualization-6.7.0/examples/surface/mountain.png
+-rwxr-xr-x   0 phil       (501) staff       (20)    14938 2024-04-20 16:01:59.787402 PyQt6_DataVisualization-6.7.0/examples/surface/surface.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.838122 PyQt6_DataVisualization-6.7.0/examples/volumetric/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.838558 PyQt6_DataVisualization-6.7.0/examples/volumetric/heightmaps/
+-rw-r--r--   0 phil       (501) staff       (20)    62477 2024-04-20 16:01:59.788092 PyQt6_DataVisualization-6.7.0/examples/volumetric/heightmaps/layer_ground.png
+-rw-r--r--   0 phil       (501) staff       (20)    16550 2024-04-20 16:01:59.788384 PyQt6_DataVisualization-6.7.0/examples/volumetric/heightmaps/layer_magma.png
+-rw-r--r--   0 phil       (501) staff       (20)    10181 2024-04-20 16:01:59.788738 PyQt6_DataVisualization-6.7.0/examples/volumetric/heightmaps/layer_water.png
+-rwxr-xr-x   0 phil       (501) staff       (20)    36700 2024-04-20 16:01:59.789140 PyQt6_DataVisualization-6.7.0/examples/volumetric/volumetric.py
+-rw-r--r--   0 phil       (501) staff       (20)      829 2024-04-20 16:02:30.630959 PyQt6_DataVisualization-6.7.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.838801 PyQt6_DataVisualization-6.7.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:02:30.845073 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/
+-rw-r--r--   0 phil       (501) staff       (20)     3497 2024-04-20 16:02:30.726395 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/QtDataVisualizationmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3188 2024-04-20 16:02:30.730669 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dbars.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3285 2024-04-20 16:02:30.727537 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dcamera.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1995 2024-04-20 16:02:30.725188 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dinputhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1279 2024-04-20 16:02:30.732051 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dlight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1456 2024-04-20 16:02:30.733200 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2004 2024-04-20 16:02:30.726659 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dscatter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2770 2024-04-20 16:02:30.729224 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dscene.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2150 2024-04-20 16:02:30.730305 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dsurface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7487 2024-04-20 16:02:30.723483 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dtheme.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2557 2024-04-20 16:02:30.723845 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qabstract3daxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6233 2024-04-20 16:02:30.731286 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qabstract3dgraph.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2351 2024-04-20 16:02:30.722632 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qabstract3dinputhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3956 2024-04-20 16:02:30.729665 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qabstract3dseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1321 2024-04-20 16:02:30.725706 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qabstractdataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1994 2024-04-20 16:02:30.725467 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qbar3dseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1343 2024-04-20 16:02:30.734078 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qbardataitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3397 2024-04-20 16:02:30.726040 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qbardataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1309 2024-04-20 16:02:30.732964 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qcategory3daxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2699 2024-04-20 16:02:30.722319 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qcustom3ditem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2216 2024-04-20 16:02:30.733484 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qcustom3dlabel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7278 2024-04-20 16:02:30.728392 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qcustom3dvolume.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2878 2024-04-20 16:02:30.734438 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qheightmapsurfacedataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5835 2024-04-20 16:02:30.721936 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qitemmodelbardataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3941 2024-04-20 16:02:30.733841 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qitemmodelscatterdataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6355 2024-04-20 16:02:30.727134 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qitemmodelsurfacedataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4388 2024-04-20 16:02:30.732743 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1856 2024-04-20 16:02:30.731557 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qlogvalue3daxisformatter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1713 2024-04-20 16:02:30.724608 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qscatter3dseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1616 2024-04-20 16:02:30.728911 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qscatterdataitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2197 2024-04-20 16:02:30.731828 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qscatterdataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2773 2024-04-20 16:02:30.730019 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qsurface3dseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1453 2024-04-20 16:02:30.724359 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qsurfacedataitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2622 2024-04-20 16:02:30.724912 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qsurfacedataproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1268 2024-04-20 16:02:30.734655 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qtouch3dinputhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1068 2024-04-20 16:02:30.722835 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qutils.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1842 2024-04-20 16:02:30.728665 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qvalue3daxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2026 2024-04-20 16:02:30.724124 PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qvalue3daxisformatter.sip
```

### Comparing `PyQt6_DataVisualization-6.6.0/ChangeLog` & `PyQt6_DataVisualization-6.7.0/ChangeLog`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+2024-04-04  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS:
+	Updated for Qt v6.7.0.
+	[75a967fa7044] [6.7.0]
+
+2024-03-17  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-DataVisualization.msp:
+	Added support for Qt v6.7.
+	[3cd364407231]
+
+2024-02-18  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* README, README.md, pyproject.toml:
+	Migrated from [tool.sip.metadata] to [project] in pyproject.toml.
+	[9576a3abf060]
+
+	* NEWS:
+	Updated the NEWS file.
+	[46d1e93de1ea]
+
+	* Merged the 6.6-maint branch.
+	[8e249f56500e]
+
+2024-01-02  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, rb-product.toml:
+	Removed the project file.
+	[936095131d33] <6.6-maint>
+
+2023-10-25  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* .hgtags:
+	Added tag 6.6.0 for changeset c976fdb9e01e
+	[27258011464a]
+
 2023-10-22  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, PyQt6-DataVisualization.msp:
 	Updated to Qt v6.6.
 	[c976fdb9e01e] [6.6.0]
 
 2023-04-04  Phil Thompson  <phil@riverbankcomputing.com>
```

### Comparing `PyQt6_DataVisualization-6.6.0/LICENSE` & `PyQt6_DataVisualization-6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/PKG-INFO` & `PyQt6_DataVisualization-6.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 Metadata-Version: 2.1
 Name: PyQt6-DataVisualization
-Version: 6.6.0
-Requires-Python: >=3.7
+Version: 6.7.0
+Requires-Python: >=3.8
 Summary: Python bindings for the Qt Data Visualization library
-Home-Page: https://www.riverbankcomputing.com/software/pyqtdatavisualization/
-Author: Riverbank Computing Limited
-Author-Email: info@riverbankcomputing.com
-License: GPL v3
+Description-Content-Type: text/markdown
+Project-Url: homepage, https://www.riverbankcomputing.com/software/pyqtdatavisualization/
 Requires-Dist: PyQt6 (>=6.2.0)
+License: GPL v3
+Author-Email: Riverbank Computing Limited <info@riverbankcomputing.com>
 
-PyQt6-DataVisualization - Python Bindings for the Qt Data Visualization Library
-===============================================================================
+# PyQt6-DataVisualization - Python Bindings for the Qt Data Visualization Library
 
 PyQt6-DataVisualization is a set of Python bindings for The Qt Company's Qt
 Data Visualization library.  The bindings sit on top of PyQt6 and are
 implemented as a single module.
 
 
-Author
-------
+## Author
 
 PyQt6-DataVisualization is copyright (c) Riverbank Computing Limited.  Its
 homepage is https://www.riverbankcomputing.com/software/pyqtdatavisualization/.
 
 Support may be obtained from the PyQt mailing list at
 https://www.riverbankcomputing.com/mailman/listinfo/pyqt/.
 
 
-License
--------
+## License
 
 PyQt6-DataVisualization is released under the GPL v3 license and under a
 commercial license that allows for the development of proprietary applications.
 
 
-Documentation
--------------
+## Documentation
 
 The documentation for the latest release can be found
-`here <https://www.riverbankcomputing.com/static/Docs/PyQt6/>`__.
+[here](https://www.riverbankcomputing.com/static/Docs/PyQt6/).
 
 
-Installation
-------------
+## Installation
 
-The GPL version of PyQt6-DataVisualization can be installed from PyPI::
+The GPL version of PyQt6-DataVisualization can be installed from PyPI:
 
     pip install PyQt6-DataVisualization
 
-``pip`` will also build and install the bindings from the sdist package but
-Qt's ``qmake`` tool must be on ``PATH``.
+`pip` will also build and install the bindings from the sdist package but Qt's
+`qmake` tool must be on `PATH`.
 
-The ``sip-install`` tool will also install the bindings from the sdist package
+The `sip-install` tool will also install the bindings from the sdist package
 but will allow you to configure many aspects of the installation.
```

### Comparing `PyQt6_DataVisualization-6.6.0/README` & `PyQt6_DataVisualization-6.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-PyQt6-DataVisualization - Python Bindings for the Qt Data Visualization Library
-===============================================================================
+# PyQt6-DataVisualization - Python Bindings for the Qt Data Visualization Library
 
 PyQt6-DataVisualization is a set of Python bindings for The Qt Company's Qt
 Data Visualization library.  The bindings sit on top of PyQt6 and are
 implemented as a single module.
 
 
-Author
-------
+## Author
 
 PyQt6-DataVisualization is copyright (c) Riverbank Computing Limited.  Its
 homepage is https://www.riverbankcomputing.com/software/pyqtdatavisualization/.
 
 Support may be obtained from the PyQt mailing list at
 https://www.riverbankcomputing.com/mailman/listinfo/pyqt/.
 
 
-License
--------
+## License
 
 PyQt6-DataVisualization is released under the GPL v3 license and under a
 commercial license that allows for the development of proprietary applications.
 
 
-Documentation
--------------
+## Documentation
 
 The documentation for the latest release can be found
-`here <https://www.riverbankcomputing.com/static/Docs/PyQt6/>`__.
+[here](https://www.riverbankcomputing.com/static/Docs/PyQt6/).
 
 
-Installation
-------------
+## Installation
 
-The GPL version of PyQt6-DataVisualization can be installed from PyPI::
+The GPL version of PyQt6-DataVisualization can be installed from PyPI:
 
     pip install PyQt6-DataVisualization
 
-``pip`` will also build and install the bindings from the sdist package but
-Qt's ``qmake`` tool must be on ``PATH``.
+`pip` will also build and install the bindings from the sdist package but Qt's
+`qmake` tool must be on `PATH`.
 
-The ``sip-install`` tool will also install the bindings from the sdist package
+The `sip-install` tool will also install the bindings from the sdist package
 but will allow you to configure many aspects of the installation.
```

### Comparing `PyQt6_DataVisualization-6.6.0/examples/bars.py` & `PyQt6_DataVisualization-6.7.0/examples/bars.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/custominput/custominput.py` & `PyQt6_DataVisualization-6.7.0/examples/custominput/custominput.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/custominput/data.txt` & `PyQt6_DataVisualization-6.7.0/examples/custominput/data.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/customproxy/customproxy.py` & `PyQt6_DataVisualization-6.7.0/examples/customproxy/customproxy.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/customproxy/raindata.txt` & `PyQt6_DataVisualization-6.7.0/examples/customproxy/raindata.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/itemmodel.py` & `PyQt6_DataVisualization-6.7.0/examples/itemmodel.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/rotations/mesh/largesphere.obj` & `PyQt6_DataVisualization-6.7.0/examples/rotations/mesh/largesphere.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/rotations/mesh/narrowarrow.obj` & `PyQt6_DataVisualization-6.7.0/examples/rotations/mesh/narrowarrow.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/rotations/rotations.py` & `PyQt6_DataVisualization-6.7.0/examples/rotations/rotations.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/scatter.py` & `PyQt6_DataVisualization-6.7.0/examples/scatter.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/surface/mountain.png` & `PyQt6_DataVisualization-6.7.0/examples/surface/mountain.png`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/surface/surface.py` & `PyQt6_DataVisualization-6.7.0/examples/surface/surface.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/volumetric/heightmaps/layer_ground.png` & `PyQt6_DataVisualization-6.7.0/examples/volumetric/heightmaps/layer_ground.png`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/volumetric/heightmaps/layer_magma.png` & `PyQt6_DataVisualization-6.7.0/examples/volumetric/heightmaps/layer_magma.png`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/volumetric/heightmaps/layer_water.png` & `PyQt6_DataVisualization-6.7.0/examples/volumetric/heightmaps/layer_water.png`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/examples/volumetric/volumetric.py` & `PyQt6_DataVisualization-6.7.0/examples/volumetric/volumetric.py`

 * *Files identical despite different names*

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/QtDataVisualizationmod.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/QtDataVisualizationmod.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtDataVisualizationmod.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -20,18 +20,18 @@
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 %Module(name=PyQt6.QtDataVisualization, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtGui/QtGuimod.sip
 
-%Timeline {QtDataVisualization_6_0_0 QtDataVisualization_6_1_0 QtDataVisualization_6_2_0 QtDataVisualization_6_3_0 QtDataVisualization_6_4_0 QtDataVisualization_6_5_0 QtDataVisualization_6_6_0}
+%Timeline {QtDataVisualization_6_0_0 QtDataVisualization_6_1_0 QtDataVisualization_6_2_0 QtDataVisualization_6_3_0 QtDataVisualization_6_4_0 QtDataVisualization_6_5_0 QtDataVisualization_6_6_0 QtDataVisualization_6_7_0}
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-DataVisualization.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
@@ -47,16 +47,16 @@
 
 %DefaultSupertype PyQt6.sip.simplewrapper
 
 int PYQT_DATAVISUALIZATION_VERSION;
 const char *PYQT_DATAVISUALIZATION_VERSION_STR;
 
 %ModuleCode
-static int PYQT_DATAVISUALIZATION_VERSION = 0x060600;
-static const char *PYQT_DATAVISUALIZATION_VERSION_STR = "6.6.0";
+static int PYQT_DATAVISUALIZATION_VERSION = 0x060700;
+static const char *PYQT_DATAVISUALIZATION_VERSION_STR = "6.7.0";
 %End
 
 %Include q3dbars.sip
 %Include q3dcamera.sip
 %Include q3dinputhandler.sip
 %Include q3dlight.sip
 %Include q3dobject.sip
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dbars.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dbars.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dbars.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class Q3DBars : QAbstract3DGraph
+class Q3DBars : public QAbstract3DGraph
 {
 %TypeHeaderCode
 #include <q3dbars.h>
 %End
 
 public:
     Q3DBars(const QSurfaceFormat *format = 0, QWindow *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dcamera.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dcamera.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dcamera.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class Q3DCamera : Q3DObject
+class Q3DCamera : public Q3DObject
 {
 %TypeHeaderCode
 #include <q3dcamera.h>
 %End
 
 public:
     enum CameraPreset
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dinputhandler.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dinputhandler.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dinputhandler.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class Q3DInputHandler : QAbstract3DInputHandler
+class Q3DInputHandler : public QAbstract3DInputHandler
 {
 %TypeHeaderCode
 #include <q3dinputhandler.h>
 %End
 
 public:
     explicit Q3DInputHandler(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dlight.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dlight.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dlight.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class Q3DLight : Q3DObject
+class Q3DLight : public Q3DObject
 {
 %TypeHeaderCode
 #include <q3dlight.h>
 %End
 
 public:
     explicit Q3DLight(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dobject.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dobject.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dobject.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class Q3DObject : QObject
+class Q3DObject : public QObject
 {
 %TypeHeaderCode
 #include <q3dobject.h>
 %End
 
 public:
     explicit Q3DObject(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dscatter.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dscatter.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dscatter.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class Q3DScatter : QAbstract3DGraph
+class Q3DScatter : public QAbstract3DGraph
 {
 %TypeHeaderCode
 #include <q3dscatter.h>
 %End
 
 public:
     Q3DScatter(const QSurfaceFormat *format = 0, QWindow *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dscene.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dscene.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dscene.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class Q3DScene : QObject
+class Q3DScene : public QObject
 {
 %TypeHeaderCode
 #include <q3dscene.h>
 %End
 
 public:
     explicit Q3DScene(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dsurface.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dsurface.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dsurface.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class Q3DSurface : QAbstract3DGraph
+class Q3DSurface : public QAbstract3DGraph
 {
 %TypeHeaderCode
 #include <q3dsurface.h>
 %End
 
 public:
     Q3DSurface(const QSurfaceFormat *format = 0, QWindow *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/q3dtheme.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/q3dtheme.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // q3dtheme.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class Q3DTheme : QObject
+class Q3DTheme : public QObject
 {
 %TypeHeaderCode
 #include <q3dtheme.h>
 %End
 
 %ConvertToSubClassCode
     static struct class_graph {
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qabstract3daxis.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qabstract3daxis.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstract3daxis.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAbstract3DAxis : QObject /NoDefaultCtors/
+class QAbstract3DAxis : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qabstract3daxis.h>
 %End
 
 public:
     enum AxisOrientation
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qabstract3dgraph.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qabstract3dgraph.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstract3dgraph.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qabstract3dinputhandler.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qabstract3dinputhandler.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstract3dinputhandler.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAbstract3DInputHandler : QObject
+class QAbstract3DInputHandler : public QObject
 {
 %TypeHeaderCode
 #include <qabstract3dinputhandler.h>
 %End
 
 public:
     enum InputView
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qabstract3dseries.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qabstract3dseries.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstract3dseries.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAbstract3DSeries : QObject /NoDefaultCtors/
+class QAbstract3DSeries : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qabstract3dseries.h>
 %End
 
 public:
     enum SeriesType
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qabstractdataproxy.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qabstractdataproxy.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractdataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAbstractDataProxy : QObject /NoDefaultCtors/
+class QAbstractDataProxy : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qabstractdataproxy.h>
 %End
 
 public:
     enum DataType
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qbar3dseries.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qbar3dseries.sip`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbar3dseries.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QBar3DSeries : QAbstract3DSeries
+class QBar3DSeries : public QAbstract3DSeries
 {
 %TypeHeaderCode
 #include <qbar3dseries.h>
 %End
 
 public:
     QBar3DSeries(QBarDataProxy *dataProxy /Transfer/, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qbardataitem.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qbardataitem.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbardataitem.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qbardataproxy.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qbardataproxy.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbardataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -19,15 +19,15 @@
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 typedef QList<QBarDataItem> QBarDataRow;
 typedef QList<QList<QBarDataItem> *> QBarDataArray;
 
-class QBarDataProxy : QAbstractDataProxy
+class QBarDataProxy : public QAbstractDataProxy
 {
 %TypeHeaderCode
 #include <qbardataproxy.h>
 %End
 
 public:
     explicit QBarDataProxy(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qcategory3daxis.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qcategory3daxis.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcategory3daxis.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QCategory3DAxis : QAbstract3DAxis
+class QCategory3DAxis : public QAbstract3DAxis
 {
 %TypeHeaderCode
 #include <qcategory3daxis.h>
 %End
 
 public:
     explicit QCategory3DAxis(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qcustom3ditem.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qcustom3ditem.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcustom3ditem.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QCustom3DItem : QObject
+class QCustom3DItem : public QObject
 {
 %TypeHeaderCode
 #include <qcustom3ditem.h>
 %End
 
 public:
     explicit QCustom3DItem(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qcustom3dlabel.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qcustom3dlabel.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcustom3dlabel.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QCustom3DLabel : QCustom3DItem
+class QCustom3DLabel : public QCustom3DItem
 {
 %TypeHeaderCode
 #include <qcustom3dlabel.h>
 %End
 
 public:
     explicit QCustom3DLabel(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qcustom3dvolume.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qcustom3dvolume.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcustom3dvolume.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -169,15 +169,15 @@
  
     sipReleaseBufferInfo(&bi);
 
     return sipGetState(sipTransferObj);
 %End
 };
 
-class QCustom3DVolume : QCustom3DItem
+class QCustom3DVolume : public QCustom3DItem
 {
 %TypeHeaderCode
 #include <qcustom3dvolume.h>
 %End
 
 public:
     explicit QCustom3DVolume(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qheightmapsurfacedataproxy.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qheightmapsurfacedataproxy.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qheightmapsurfacedataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QHeightMapSurfaceDataProxy : QSurfaceDataProxy
+class QHeightMapSurfaceDataProxy : public QSurfaceDataProxy
 {
 %TypeHeaderCode
 #include <qheightmapsurfacedataproxy.h>
 %End
 
 public:
     explicit QHeightMapSurfaceDataProxy(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qitemmodelbardataproxy.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qitemmodelbardataproxy.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qitemmodelbardataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QItemModelBarDataProxy : QBarDataProxy
+class QItemModelBarDataProxy : public QBarDataProxy
 {
 %TypeHeaderCode
 #include <qitemmodelbardataproxy.h>
 %End
 
 public:
     QItemModelBarDataProxy(QAbstractItemModel *itemModel /KeepReference=120/, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qitemmodelscatterdataproxy.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qitemmodelscatterdataproxy.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qitemmodelscatterdataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QItemModelScatterDataProxy : QScatterDataProxy
+class QItemModelScatterDataProxy : public QScatterDataProxy
 {
 %TypeHeaderCode
 #include <qitemmodelscatterdataproxy.h>
 %End
 
 public:
     QItemModelScatterDataProxy(QAbstractItemModel *itemModel /KeepReference=120/, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qitemmodelsurfacedataproxy.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qitemmodelsurfacedataproxy.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qitemmodelsurfacedataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QItemModelSurfaceDataProxy : QSurfaceDataProxy
+class QItemModelSurfaceDataProxy : public QSurfaceDataProxy
 {
 %TypeHeaderCode
 #include <qitemmodelsurfacedataproxy.h>
 %End
 
 public:
     QItemModelSurfaceDataProxy(QAbstractItemModel *itemModel /KeepReference=120/, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qlist.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qlist.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 // This is the SIP interface definition for the QList based mapped types.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qlogvalue3daxisformatter.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qlogvalue3daxisformatter.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlogvalue3daxisformatter.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QLogValue3DAxisFormatter : QValue3DAxisFormatter
+class QLogValue3DAxisFormatter : public QValue3DAxisFormatter
 {
 %TypeHeaderCode
 #include <qlogvalue3daxisformatter.h>
 %End
 
 public:
     explicit QLogValue3DAxisFormatter(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qscatter3dseries.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qscatter3dseries.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscatter3dseries.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QScatter3DSeries : QAbstract3DSeries
+class QScatter3DSeries : public QAbstract3DSeries
 {
 %TypeHeaderCode
 #include <qscatter3dseries.h>
 %End
 
 public:
     QScatter3DSeries(QScatterDataProxy *dataProxy /Transfer/, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qscatterdataitem.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qscatterdataitem.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscatterdataitem.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qscatterdataproxy.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qscatterdataproxy.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscatterdataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -18,15 +18,15 @@
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 typedef QList<QScatterDataItem> QScatterDataArray;
 
-class QScatterDataProxy : QAbstractDataProxy
+class QScatterDataProxy : public QAbstractDataProxy
 {
 %TypeHeaderCode
 #include <qscatterdataproxy.h>
 %End
 
 public:
     explicit QScatterDataProxy(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qsurface3dseries.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qsurface3dseries.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsurface3dseries.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QSurface3DSeries : QAbstract3DSeries
+class QSurface3DSeries : public QAbstract3DSeries
 {
 %TypeHeaderCode
 #include <qsurface3dseries.h>
 %End
 
 public:
     enum DrawFlag /BaseType=Flag/
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qsurfacedataitem.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qsurfacedataitem.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsurfacedataitem.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qsurfacedataproxy.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qsurfacedataproxy.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsurfacedataproxy.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -19,15 +19,15 @@
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 typedef QList<QSurfaceDataItem> QSurfaceDataRow;
 typedef QList<QList<QSurfaceDataItem> *> QSurfaceDataArray;
 
-class QSurfaceDataProxy : QAbstractDataProxy
+class QSurfaceDataProxy : public QAbstractDataProxy
 {
 %TypeHeaderCode
 #include <qsurfacedataproxy.h>
 %End
 
 public:
     explicit QSurfaceDataProxy(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qtouch3dinputhandler.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qtouch3dinputhandler.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtouch3dinputhandler.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QTouch3DInputHandler : Q3DInputHandler
+class QTouch3DInputHandler : public Q3DInputHandler
 {
 %TypeHeaderCode
 #include <qtouch3dinputhandler.h>
 %End
 
 public:
     explicit QTouch3DInputHandler(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qutils.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qutils.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qutils.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qvalue3daxis.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qvalue3daxis.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvalue3daxis.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QValue3DAxis : QAbstract3DAxis
+class QValue3DAxis : public QAbstract3DAxis
 {
 %TypeHeaderCode
 #include <qvalue3daxis.h>
 %End
 
 public:
     explicit QValue3DAxis(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_DataVisualization-6.6.0/sip/QtDataVisualization/qvalue3daxisformatter.sip` & `PyQt6_DataVisualization-6.7.0/sip/QtDataVisualization/qvalue3daxisformatter.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvalue3daxisformatter.sip generated by MetaSIP
 //
 // This file is part of the QtDataVisualization Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-DataVisualization.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QValue3DAxisFormatter : QObject
+class QValue3DAxisFormatter : public QObject
 {
 %TypeHeaderCode
 #include <qvalue3daxisformatter.h>
 %End
 
 public:
     explicit QValue3DAxisFormatter(QObject *parent /TransferThis/ = 0);
```

