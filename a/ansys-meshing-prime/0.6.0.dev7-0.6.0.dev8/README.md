# Comparing `tmp/ansys_meshing_prime-0.6.0.dev7.tar.gz` & `tmp/ansys_meshing_prime-0.6.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_meshing_prime-0.6.0.dev7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_meshing_prime-0.6.0.dev8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_meshing_prime-0.6.0.dev7.tar` & `ansys_meshing_prime-0.6.0.dev8.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     1090 2024-04-05 11:31:19.583258 ansys_meshing_prime-0.6.0.dev7/LICENSE
--rw-r--r--   0        0        0     4090 2024-04-05 11:31:19.583258 ansys_meshing_prime-0.6.0.dev7/README.md
--rw-r--r--   0        0        0     3239 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/pyproject.toml
--rw-r--r--   0        0        0     6218 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/__init__.py
--rw-r--r--   0        0        0      428 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/_version.py
--rw-r--r--   0        0        0     2654 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/automesh.py
--rw-r--r--   0        0        0    61369 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/automeshstructs.py
--rw-r--r--   0        0        0    11093 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/autoquadmesher.py
--rw-r--r--   0        0        0   165219 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/autoquadmesherstructs.py
--rw-r--r--   0        0        0     6123 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
--rw-r--r--   0        0        0     3977 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/collapsetool.py
--rw-r--r--   0        0        0    14791 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
--rw-r--r--   0        0        0    28002 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/commonstructs.py
--rw-r--r--   0        0        0     3875 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/commontypes.py
--rw-r--r--   0        0        0    14928 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/connect.py
--rw-r--r--   0        0        0    95082 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/connectstructs.py
--rw-r--r--   0        0        0    12218 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/controldata.py
--rw-r--r--   0        0        0    91621 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/controlstructs.py
--rw-r--r--   0        0        0      714 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/coreobject.py
--rw-r--r--   0        0        0     3433 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/deletetool.py
--rw-r--r--   0        0        0    14080 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/deletetoolstructs.py
--rw-r--r--   0        0        0     5585 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/featureextraction.py
--rw-r--r--   0        0        0    35361 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/featureextractionstructs.py
--rw-r--r--   0        0        0    31271 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/fileio.py
--rw-r--r--   0        0        0   169973 2024-04-05 11:31:19.667259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/fileiostructs.py
--rw-r--r--   0        0        0    71909 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/igastructs.py
--rw-r--r--   0        0        0     4136 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/materialpointmanager.py
--rw-r--r--   0        0        0    16431 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
--rw-r--r--   0        0        0     4866 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/meshinfo.py
--rw-r--r--   0        0        0    60305 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/meshinfostructs.py
--rw-r--r--   0        0        0    16840 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/model.py
--rw-r--r--   0        0        0    27452 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/modelstructs.py
--rw-r--r--   0        0        0     3803 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/morpher.py
--rw-r--r--   0        0        0     7876 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
--rw-r--r--   0        0        0    24470 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/morpherstructs.py
--rw-r--r--   0        0        0     7869 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/multizonecontrol.py
--rw-r--r--   0        0        0    59442 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/part.py
--rw-r--r--   0        0        0   168878 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/partstructs.py
--rw-r--r--   0        0        0     7671 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/periodiccontrol.py
--rw-r--r--   0        0        0    13543 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
--rw-r--r--   0        0        0    33989 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/primeconfig.py
--rw-r--r--   0        0        0     5733 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/prismcontrol.py
--rw-r--r--   0        0        0    14608 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
--rw-r--r--   0        0        0     2937 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/quadtospline.py
--rw-r--r--   0        0        0     7253 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/scaffolder.py
--rw-r--r--   0        0        0    38220 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/scaffolderstructs.py
--rw-r--r--   0        0        0    18400 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/sizecontrol.py
--rw-r--r--   0        0        0    53218 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
--rw-r--r--   0        0        0     2794 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/sizefield.py
--rw-r--r--   0        0        0    19028 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/sizefieldstructs.py
--rw-r--r--   0        0        0     4286 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/splittoolstructs.py
--rw-r--r--   0        0        0    21687 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surfacesearch.py
--rw-r--r--   0        0        0   124157 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
--rw-r--r--   0        0        0    27325 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surfaceutilities.py
--rw-r--r--   0        0        0   166806 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
--rw-r--r--   0        0        0     7198 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surfer.py
--rw-r--r--   0        0        0    45142 2024-04-05 11:31:19.671259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surferstructs.py
--rw-r--r--   0        0        0     5773 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
--rw-r--r--   0        0        0     7117 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
--rw-r--r--   0        0        0    10182 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/topodata.py
--rw-r--r--   0        0        0     9409 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/topodatastructs.py
--rw-r--r--   0        0        0     1761 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/toposearchstructs.py
--rw-r--r--   0        0        0     2650 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/topoutilities.py
--rw-r--r--   0        0        0    13257 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/topoutilitystructs.py
--rw-r--r--   0        0        0     2966 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/transform.py
--rw-r--r--   0        0        0     8817 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/transformstructs.py
--rw-r--r--   0        0        0     5986 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumecontrol.py
--rw-r--r--   0        0        0     6304 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
--rw-r--r--   0        0        0     6962 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumemeshtool.py
--rw-r--r--   0        0        0    29781 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
--rw-r--r--   0        0        0     2763 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumesearch.py
--rw-r--r--   0        0        0    25627 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumesearchstructs.py
--rw-r--r--   0        0        0     4896 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumesweeper.py
--rw-r--r--   0        0        0    25625 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
--rw-r--r--   0        0        0     2927 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/vtcomposer.py
--rw-r--r--   0        0        0     8476 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/vtcomposerstructs.py
--rw-r--r--   0        0        0     7270 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/wrapper.py
--rw-r--r--   0        0        0    10832 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/wrappercontrol.py
--rw-r--r--   0        0        0    89981 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/wrapperstructs.py
--rw-r--r--   0        0        0    15856 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/controldata.py
--rw-r--r--   0        0        0   121829 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/dynaexportutils.py
--rw-r--r--   0        0        0    20701 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/fileio.py
--rw-r--r--   0        0        0   161431 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/mapdlcdbexportutils.py
--rw-r--r--   0        0        0    11168 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/model.py
--rw-r--r--   0        0        0      767 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/multizonecontrol.py
--rw-r--r--   0        0        0     4181 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/part.py
--rw-r--r--   0        0        0     2287 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/periodiccontrol.py
--rw-r--r--   0        0        0     2208 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/sizecontrol.py
--rw-r--r--   0        0        0     4069 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/surfaceutilities.py
--rw-r--r--   0        0        0     4664 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/surfer.py
--rw-r--r--   0        0        0     2309 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/volumecontrol.py
--rw-r--r--   0        0        0     3064 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/volumesweeper.py
--rw-r--r--   0        0        0     7289 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/wrapper.py
--rw-r--r--   0        0        0     2115 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/wrappercontrol.py
--rw-r--r--   0        0        0     1269 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/examples/__init__.py
--rw-r--r--   0        0        0     4566 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/examples/download_utilities.py
--rw-r--r--   0        0        0    47227 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/examples/examples.py
--rw-r--r--   0        0        0     1514 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/examples/unit_test_examples.py
--rw-r--r--   0        0        0       59 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/__init__.py
--rw-r--r--   0        0        0    41774 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/graphics.py
--rw-r--r--   0        0        0     2234 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/bin.png
--rw-r--r--   0        0        0     1708 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/invert_visibility.png
--rw-r--r--   0        0        0     2510 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/parts.png
--rw-r--r--   0        0        0     1297 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/selectioninfo.png
--rw-r--r--   0        0        0     2440 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/show_edges.png
--rw-r--r--   0        0        0      203 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/show_ruler.png
--rw-r--r--   0        0        0     1547 2024-04-05 11:31:19.675259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/surface_body.png
--rw-r--r--   0        0        0     1612 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/trame_gui.py
--rw-r--r--   0        0        0     5692 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/client.py
--rw-r--r--   0        0        0      626 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/comm_manager.py
--rw-r--r--   0        0        0     1881 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/communicator.py
--rw-r--r--   0        0        0     5045 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/config.py
--rw-r--r--   0        0        0     3121 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/defaults.py
--rw-r--r--   0        0        0    40442 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/error_handling.py
--rw-r--r--   0        0        0     8935 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/grpc_communicator.py
--rw-r--r--   0        0        0      951 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/grpc_utils.py
--rw-r--r--   0        0        0     2319 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/json_utils.py
--rw-r--r--   0        0        0     8307 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/launcher.py
--rw-r--r--   0        0        0     2586 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/logger.py
--rw-r--r--   0        0        0     3182 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/prime_communicator.py
--rw-r--r--   0        0        0    12339 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/utils.py
--rw-r--r--   0        0        0      143 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/lucid/__init__.py
--rw-r--r--   0        0        0    70047 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/lucid/mesh_util.py
--rw-r--r--   0        0        0     7532 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/lucid/scope.py
--rw-r--r--   0        0        0     1493 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/lucid/utils.py
--rw-r--r--   0        0        0     2346 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/params/primestructs.py
--rw-r--r--   0        0        0     4369 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/relaxed_json/__init__.py
--rw-r--r--   0        0        0    13490 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/relaxed_json/decoder.py
--rw-r--r--   0        0        0    13168 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/relaxed_json/encoder.py
--rw-r--r--   0        0        0     3024 2024-04-05 11:31:19.679259 ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/relaxed_json/scanner.py
--rw-r--r--   0        0        0     6089 1970-01-01 00:00:00.000000 ansys_meshing_prime-0.6.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-26 12:39:26.833204 ansys_meshing_prime-0.6.0.dev8/LICENSE
+-rw-r--r--   0        0        0     4090 2024-04-26 12:39:26.833204 ansys_meshing_prime-0.6.0.dev8/README.md
+-rw-r--r--   0        0        0     3239 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0     6218 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/__init__.py
+-rw-r--r--   0        0        0      428 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/_version.py
+-rw-r--r--   0        0        0     2654 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/automesh.py
+-rw-r--r--   0        0        0    61369 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/automeshstructs.py
+-rw-r--r--   0        0        0    11093 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/autoquadmesher.py
+-rw-r--r--   0        0        0   165219 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/autoquadmesherstructs.py
+-rw-r--r--   0        0        0     6123 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
+-rw-r--r--   0        0        0     3977 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/collapsetool.py
+-rw-r--r--   0        0        0    14791 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
+-rw-r--r--   0        0        0    28002 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/commonstructs.py
+-rw-r--r--   0        0        0     3875 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/commontypes.py
+-rw-r--r--   0        0        0    15145 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/connect.py
+-rw-r--r--   0        0        0    95433 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/connectstructs.py
+-rw-r--r--   0        0        0    12218 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/controldata.py
+-rw-r--r--   0        0        0    91621 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/controlstructs.py
+-rw-r--r--   0        0        0      714 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/coreobject.py
+-rw-r--r--   0        0        0     3433 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/deletetool.py
+-rw-r--r--   0        0        0    14080 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/deletetoolstructs.py
+-rw-r--r--   0        0        0     5585 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/featureextraction.py
+-rw-r--r--   0        0        0    35361 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/featureextractionstructs.py
+-rw-r--r--   0        0        0    31271 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/fileio.py
+-rw-r--r--   0        0        0   169973 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/fileiostructs.py
+-rw-r--r--   0        0        0    71909 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/igastructs.py
+-rw-r--r--   0        0        0     4136 2024-04-26 12:39:26.913204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanager.py
+-rw-r--r--   0        0        0    16431 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
+-rw-r--r--   0        0        0     4866 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/meshinfo.py
+-rw-r--r--   0        0        0    60305 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/meshinfostructs.py
+-rw-r--r--   0        0        0    16840 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/model.py
+-rw-r--r--   0        0        0    27452 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/modelstructs.py
+-rw-r--r--   0        0        0     3803 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/morpher.py
+-rw-r--r--   0        0        0     7876 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
+-rw-r--r--   0        0        0    24470 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/morpherstructs.py
+-rw-r--r--   0        0        0     7869 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/multizonecontrol.py
+-rw-r--r--   0        0        0    59442 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/part.py
+-rw-r--r--   0        0        0   168878 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/partstructs.py
+-rw-r--r--   0        0        0     7671 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrol.py
+-rw-r--r--   0        0        0    13543 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
+-rw-r--r--   0        0        0    34490 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/primeconfig.py
+-rw-r--r--   0        0        0     5733 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/prismcontrol.py
+-rw-r--r--   0        0        0    14608 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
+-rw-r--r--   0        0        0     2937 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/quadtospline.py
+-rw-r--r--   0        0        0     7253 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/scaffolder.py
+-rw-r--r--   0        0        0    38220 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/scaffolderstructs.py
+-rw-r--r--   0        0        0    18400 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/sizecontrol.py
+-rw-r--r--   0        0        0    53218 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
+-rw-r--r--   0        0        0     2794 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/sizefield.py
+-rw-r--r--   0        0        0    19028 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/sizefieldstructs.py
+-rw-r--r--   0        0        0     4286 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/splittoolstructs.py
+-rw-r--r--   0        0        0    21687 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surfacesearch.py
+-rw-r--r--   0        0        0   124157 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
+-rw-r--r--   0        0        0    27325 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilities.py
+-rw-r--r--   0        0        0   166806 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
+-rw-r--r--   0        0        0     7198 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surfer.py
+-rw-r--r--   0        0        0    45142 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surferstructs.py
+-rw-r--r--   0        0        0     5773 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
+-rw-r--r--   0        0        0     7117 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
+-rw-r--r--   0        0        0    10182 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/topodata.py
+-rw-r--r--   0        0        0     9409 2024-04-26 12:39:26.917204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/topodatastructs.py
+-rw-r--r--   0        0        0     1761 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/toposearchstructs.py
+-rw-r--r--   0        0        0     2650 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/topoutilities.py
+-rw-r--r--   0        0        0    13257 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/topoutilitystructs.py
+-rw-r--r--   0        0        0     2966 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/transform.py
+-rw-r--r--   0        0        0     8817 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/transformstructs.py
+-rw-r--r--   0        0        0     5986 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumecontrol.py
+-rw-r--r--   0        0        0     6304 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
+-rw-r--r--   0        0        0     6962 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtool.py
+-rw-r--r--   0        0        0    29781 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
+-rw-r--r--   0        0        0     2763 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumesearch.py
+-rw-r--r--   0        0        0    25627 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumesearchstructs.py
+-rw-r--r--   0        0        0     4896 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumesweeper.py
+-rw-r--r--   0        0        0    25625 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
+-rw-r--r--   0        0        0     2927 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/vtcomposer.py
+-rw-r--r--   0        0        0     8476 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/vtcomposerstructs.py
+-rw-r--r--   0        0        0     7270 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/wrapper.py
+-rw-r--r--   0        0        0    10832 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/wrappercontrol.py
+-rw-r--r--   0        0        0    89981 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/wrapperstructs.py
+-rw-r--r--   0        0        0    15856 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/controldata.py
+-rw-r--r--   0        0        0   121829 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/dynaexportutils.py
+-rw-r--r--   0        0        0    20701 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/fileio.py
+-rw-r--r--   0        0        0   163121 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/mapdlcdbexportutils.py
+-rw-r--r--   0        0        0    11168 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/model.py
+-rw-r--r--   0        0        0      767 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/multizonecontrol.py
+-rw-r--r--   0        0        0     4181 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/part.py
+-rw-r--r--   0        0        0     2287 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/periodiccontrol.py
+-rw-r--r--   0        0        0     2208 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/sizecontrol.py
+-rw-r--r--   0        0        0     4069 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/surfaceutilities.py
+-rw-r--r--   0        0        0     4664 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/surfer.py
+-rw-r--r--   0        0        0     2309 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/volumecontrol.py
+-rw-r--r--   0        0        0     3064 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/volumesweeper.py
+-rw-r--r--   0        0        0     7289 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/wrapper.py
+-rw-r--r--   0        0        0     2115 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/wrappercontrol.py
+-rw-r--r--   0        0        0     1269 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/examples/__init__.py
+-rw-r--r--   0        0        0     4566 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/examples/download_utilities.py
+-rw-r--r--   0        0        0    47227 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/examples/examples.py
+-rw-r--r--   0        0        0     1514 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/examples/unit_test_examples.py
+-rw-r--r--   0        0        0       59 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/__init__.py
+-rw-r--r--   0        0        0    41774 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/graphics.py
+-rw-r--r--   0        0        0     2234 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/bin.png
+-rw-r--r--   0        0        0     1708 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/invert_visibility.png
+-rw-r--r--   0        0        0     2510 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/parts.png
+-rw-r--r--   0        0        0     1297 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/selectioninfo.png
+-rw-r--r--   0        0        0     2440 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/show_edges.png
+-rw-r--r--   0        0        0      203 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/show_ruler.png
+-rw-r--r--   0        0        0     1547 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/surface_body.png
+-rw-r--r--   0        0        0     1612 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/trame_gui.py
+-rw-r--r--   0        0        0     5692 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/client.py
+-rw-r--r--   0        0        0      626 2024-04-26 12:39:26.921203 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/comm_manager.py
+-rw-r--r--   0        0        0     1881 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/communicator.py
+-rw-r--r--   0        0        0     5045 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/config.py
+-rw-r--r--   0        0        0     3168 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/defaults.py
+-rw-r--r--   0        0        0    40888 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/error_handling.py
+-rw-r--r--   0        0        0     8935 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/grpc_communicator.py
+-rw-r--r--   0        0        0      951 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/grpc_utils.py
+-rw-r--r--   0        0        0     2319 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/json_utils.py
+-rw-r--r--   0        0        0     8307 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/launcher.py
+-rw-r--r--   0        0        0     2586 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/logger.py
+-rw-r--r--   0        0        0     3182 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/prime_communicator.py
+-rw-r--r--   0        0        0    12339 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/utils.py
+-rw-r--r--   0        0        0      143 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/lucid/__init__.py
+-rw-r--r--   0        0        0    70047 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/lucid/mesh_util.py
+-rw-r--r--   0        0        0     7532 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/lucid/scope.py
+-rw-r--r--   0        0        0     1493 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/lucid/utils.py
+-rw-r--r--   0        0        0     2346 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/params/primestructs.py
+-rw-r--r--   0        0        0     4369 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/relaxed_json/__init__.py
+-rw-r--r--   0        0        0    13490 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/relaxed_json/decoder.py
+-rw-r--r--   0        0        0    13168 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/relaxed_json/encoder.py
+-rw-r--r--   0        0        0     3024 2024-04-26 12:39:26.925204 ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/relaxed_json/scanner.py
+-rw-r--r--   0        0        0     6089 1970-01-01 00:00:00.000000 ansys_meshing_prime-0.6.0.dev8/PKG-INFO
```

### Comparing `ansys_meshing_prime-0.6.0.dev7/LICENSE` & `ansys_meshing_prime-0.6.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/README.md` & `ansys_meshing_prime-0.6.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/pyproject.toml` & `ansys_meshing_prime-0.6.0.dev8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-meshing-prime"
-version = "0.6.0.dev7"
+version = "0.6.0.dev8"
 description = "PyPrimeMesh is a Python client to Ansys Prime Server, which delivers core Ansys meshing technology."
 readme = "README.md"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 maintainers =  [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 classifiers = [
@@ -36,20 +36,20 @@
   "pytest==8.1.1",
   "pytest-cov==4.1.0",
   "pytest-pyvista==0.1.9",
   "pytest-xvfb==3.0.0",
   "pyvista[trame]==0.43.4"
 ]
 doc = [
-  "ansys-sphinx-theme==0.14.1",
+  "ansys-sphinx-theme==0.15.2",
   "jupyter-sphinx==0.5.3",
-  "numpydoc==1.6.0",
+  "numpydoc==1.7.0",
   "Sphinx==7.2.6",
   "pyvista==0.43.4",
-  "sphinx-autodoc-typehints==2.0.0",
+  "sphinx-autodoc-typehints==2.0.1",
   "sphinx-copybutton==0.5.2",
   "sphinx-gallery==0.15.0",
   "sphinx-notfound-page==1.0.0",
   "sphinxemoji==0.3.1",
 ]
 all = [
   "pyvista[jupyter]>=0.38.1",
```

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/__init__.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/automesh.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/automesh.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/automeshstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/automeshstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/autoquadmesher.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/autoquadmesher.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/autoquadmesherstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/autoquadmesherstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/collapsetool.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/collapsetool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/collapsetoolstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/collapsetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/commonstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/commonstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/commontypes.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/commontypes.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/connect.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,21 +122,21 @@
         command_name = "PrimeMesh::Connect/JoinFaceZonelets"
         self._model._print_logs_before_command("join_face_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("join_face_zonelets", ConnectResults(model = self._model, json_data = result))
         return ConnectResults(model = self._model, json_data = result)
 
     def subtract_volumes(self, part_id : int, target_volumes : Iterable[int], cutter_volumes : Iterable[int], params : SubtractVolumesParams) -> SubtractVolumesResults:
-        """ Subtract cutter volumes from target volumes. Volumes should be computed prior to calling this function.
+        """ Subtract cutter volumes from target volumes. Volumes should be computed prior to calling this function. If multiple parts are being merged to form a single part, then volumes should be computed for each part prior to merging. Use compute_closed_volumes to do so.
 
 
         Parameters
         ----------
         part_id : int
-            Id of a part.
+            Id of part containing target and cutter volumes for subtract operation.
         target_volumes : Iterable[int]
             Ids of target volumes.
         cutter_volumes : Iterable[int]
             Ids of cutter volumes.
         params : SubtractVolumesParams
             Parameters to control subtraction of volumes.
```

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/connectstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/connectstructs.py`

 * *Files 2% similar despite different names*

```diff
@@ -852,15 +852,15 @@
         Parameters
         ----------
         model: Model
             Model to create a ``SubtractVolumesParams`` object with default parameters.
         ignore_face_zonelets: Iterable[int], optional
             Face zonelet ids that subtract volumes should not remove (for example, periodic or fluid cap zonelets). If ignore face zonelets are provided, then the target volumes after subtract operation need to be recomputed.
         check_cutters: bool, optional
-            Option to analyze overlapping or intersecting cutter volumes.
+            Option to manage intersecting cutter volumes. When keep_cutters is False an error message is provided if multiple cutters intersect. Overlapping cutter volumes are not supported.
         keep_cutters: bool, optional
             Option to retain cutter volumes.
             This is a beta parameter. The behavior and name may change in the future.
         json_data: dict, optional
             JSON dictionary to create a ``SubtractVolumesParams`` object with provided parameters.
 
         Examples
@@ -904,15 +904,15 @@
         """Set the default values of the ``SubtractVolumesParams`` object.
 
         Parameters
         ----------
         ignore_face_zonelets: Iterable[int], optional
             Face zonelet ids that subtract volumes should not remove (for example, periodic or fluid cap zonelets). If ignore face zonelets are provided, then the target volumes after subtract operation need to be recomputed.
         check_cutters: bool, optional
-            Option to analyze overlapping or intersecting cutter volumes.
+            Option to manage intersecting cutter volumes. When keep_cutters is False an error message is provided if multiple cutters intersect. Overlapping cutter volumes are not supported.
         keep_cutters: bool, optional
             Option to retain cutter volumes.
         """
         args = locals()
         [SubtractVolumesParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
@@ -951,15 +951,15 @@
 
     @ignore_face_zonelets.setter
     def ignore_face_zonelets(self, value: Iterable[int]):
         self._ignore_face_zonelets = value
 
     @property
     def check_cutters(self) -> bool:
-        """Option to analyze overlapping or intersecting cutter volumes.
+        """Option to manage intersecting cutter volumes. When keep_cutters is False an error message is provided if multiple cutters intersect. Overlapping cutter volumes are not supported.
         """
         return self._check_cutters
 
     @check_cutters.setter
     def check_cutters(self, value: bool):
         self._check_cutters = value
```

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/controldata.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/controldata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/controlstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/controlstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/coreobject.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/coreobject.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/deletetool.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/deletetool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/deletetoolstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/deletetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/featureextraction.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/featureextraction.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/featureextractionstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/featureextractionstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/fileio.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/fileio.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/fileiostructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/fileiostructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/igastructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/igastructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/materialpointmanager.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanager.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/meshinfo.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/meshinfo.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/meshinfostructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/meshinfostructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/model.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/model.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/modelstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/modelstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/morpher.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/morpher.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/morpherbcsstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/morpherbcsstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/morpherstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/morpherstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/multizonecontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/multizonecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/part.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/part.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/partstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/partstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/periodiccontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/primeconfig.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/primeconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,15 +333,15 @@
     INVALIDINPUTZONELETS = 1309
     """Invalid input zonelets."""
     MERGEZONELETSFAILED = 1310
     """Merge zonelets failed."""
     MERGESMALLZONELETSSUPPORTEDFORFACEZONELETS = 1311
     """Merge small zonelets option is supported for only face zonelets."""
     INVALIDINPUTVOLUMES = 1312
-    """Invalid input volumes."""
+    """List of volume ids provided is empty or incorrect."""
     MORPHER_COMPUTEBCS = 1410
     """Failed to compute boundary conditions."""
     MORPHER_MATCHMORPHINVALIDSOURCEINPUT = 1450
     """Invalid source input for match morphing."""
     MORPHER_BCPAIRINPUTTYPEMISMATCH = 1451
     """Entity type does not match with input for defined boundary condition pair."""
     INVALIDGLOBALMINMAX = 1500
@@ -647,14 +647,23 @@
     """Bad shape properties."""
     AUTOQUADMESHER_NEGATIVEINPUTPARAMETER = 15000
     """Autoquadmesher error codes.
     This is a beta parameter. The behavior and name may change in the future."""
     AUTOQUADMESHER_INVALIDMINMAXSIZES = 15001
     """Difference in maximum value and minimum value is negative.
     This is a beta parameter. The behavior and name may change in the future."""
+    ZEROELEMENTSREADFROMCDBFILE = 16500
+    """No elements read from CDB file.
+    This is a beta parameter. The behavior and name may change in the future."""
+    ZERONODESREADFROMCDBFILE = 16501
+    """No nodes read from CDB file.
+    This is a beta parameter. The behavior and name may change in the future."""
+    ZEROELEMENTSFORCDBEXPORT = 16600
+    """No elements found for cdb export.
+    This is a beta parameter. The behavior and name may change in the future."""
 
 class WarningCode(enum.IntEnum):
     """Warning codes associated with the PyPrimeMesh operation.
     """
     NOWARNING = 0
     """No warnings."""
     UNKNOWN = 1
```

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/prismcontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/prismcontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/prismcontrolstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/prismcontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/quadtospline.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/quadtospline.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/scaffolder.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/scaffolder.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/scaffolderstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/scaffolderstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/sizecontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/sizecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/sizecontrolstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/sizecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/sizefield.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/sizefield.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/sizefieldstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/sizefieldstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/splittoolstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/splittoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surfacesearch.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surfacesearch.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surfacesearchstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surfacesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surfaceutilities.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surfer.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surfer.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/surferstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/surferstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/thinvolumecontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/topodata.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/topodata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/topodatastructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/topodatastructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/toposearchstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/toposearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/topoutilities.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/topoutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/topoutilitystructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/topoutilitystructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/transform.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/transform.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/transformstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/transformstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumecontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumecontrolstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumemeshtool.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumesearch.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumesearch.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumesearchstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumesweeper.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumesweeper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/volumesweeperstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/volumesweeperstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/vtcomposer.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/vtcomposer.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/vtcomposerstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/vtcomposerstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/wrapper.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/wrappercontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/wrappercontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/autogen/wrapperstructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/autogen/wrapperstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/controldata.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/controldata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/dynaexportutils.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/dynaexportutils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/fileio.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/fileio.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/mapdlcdbexportutils.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/mapdlcdbexportutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -677,88 +677,95 @@
                 mapdl_text_data = self._get_mat_comands(material)
                 break
         return mapdl_text_data
 
     def _process_expansion_data(self, property_dict, material, mat_id):
         expansion_data = ''
         zero = 0.0
+        data = []
+        parameters = []
+        if 'Parameters' in property_dict and property_dict['Parameters'] is not None:
+            parameters = property_dict['Parameters']
+        if 'Data' in property_dict and property_dict['Data'] is not None:
+            data = property_dict['Data']
         exp_type = 'ISO'
-        if 'ZERO' in property_dict['Parameters']:
-            zero = float(property_dict['Parameters']['ZERO'])
-        if 'TYPE' in property_dict['Parameters']:
-            exp_type = property_dict['Parameters']['TYPE']
-        if (
-            'DEPENDENCIES' in property_dict['Parameters']
-            or 'PORE FLUID' in property_dict['Parameters']
-            or 'USER' in property_dict['Parameters']
-        ):
+        if 'ZERO' in parameters:
+            zero = float(parameters['ZERO'])
+        if 'TYPE' in parameters:
+            exp_type = parameters['TYPE']
+        if 'DEPENDENCIES' in parameters or 'PORE FLUID' in parameters or 'USER' in parameters:
             self._logger.warning(
                 f"Arguments PORE FLUID, DEPENDENCIES and USER on "
                 f"*EXPANSION are not processed for material {material}"
             )
             return ''
         if exp_type == 'SHORT FIBER' or exp_type == 'ANISO':
             self._logger.warning(
                 f"*EXPANSION of type SHORT FIBER and ANISO are "
                 f"not processed for material {material}."
             )
             return ''
-        if 'ZERO' in property_dict['Parameters']:
-            expansion_data += f"MP,REFT,{mat_id},{zero}"
+        if 'ZERO' in parameters:
+            expansion_data += f"MP,REFT,{mat_id},{zero}\n"
         if exp_type == 'ISO':
             temperature = [None]
-            if 'Temperature' in property_dict['Data']:
-                temperature = property_dict['Data']['Temperature']
-            if 'a' in property_dict['Data']:
-                ctes = property_dict['Data']['a']
+            ctes = [None]
+            if 'Temperature' in data:
+                temperature = data['Temperature']
+            if 'a' in data:
+                ctes = data['a']
             expansion_data += f"TB, CTE, {mat_id},,,\n"
             for temp, cte in zip(temperature, ctes):
                 if temp is not None:
                     expansion_data += f"TBTEMP,{temp}\n"
                 expansion_data += f"TBDATA, 1, {cte}\n"
         if exp_type == 'ORTHO':
-            if 'A11' in property_dict['Data']:
-                ctexs = property_dict['Data']['A11']
+            if 'A11' in data:
+                ctexs = data['A11']
             cteys = ['0.0'] * len(ctexs)
-            if 'A22' in property_dict['Data']:
-                cteys = property_dict['Data']['A22']
+            if 'A22' in data:
+                cteys = data['A22']
             ctezs = ['0.0'] * len(ctexs)
-            if 'A33' in property_dict['Data']:
-                ctezs = property_dict['Data']['A33']
+            if 'A33' in data:
+                ctezs = data['A33']
             temperature = [None] * len(ctexs)
-            if 'Temperature' in property_dict['Data']:
-                temperature = property_dict['Data']['Temperature']
+            if 'Temperature' in data:
+                temperature = data['Temperature']
             expansion_data += f"TB, CTE, {mat_id},,,\n"
             for temp, ctex, ctey, ctez in zip(temperature, ctexs, cteys, ctezs):
                 if temp is not None:
                     expansion_data += f"TBTEMP,{temp}\n"
                 expansion_data += f"TBDATA, 1, {ctex}, {ctey}, {ctez}\n"
             expansion_data += "\n"
         return expansion_data
 
     def _process_damping_data(self, property_dict, material, mat_id):
         damping_data = ''
         if property_dict['Parameters'] is None:
             self._logger.warning(f"*DAMPING does not have parameters to process.")
-        if 'ALPHA' in property_dict['Parameters']:
-            damping_data += f"MP, ALPD, {mat_id}, {property_dict['Parameters']['ALPHA']} \n"
-        if float(property_dict['Parameters']['BETA']) != 0.0:
-            self._logger.warning(f"Parameter {'BETA'} on *DAMPING is not processed.")
-        if float(property_dict['Parameters']['COMPOSITE']) != 0.0:
-            self._logger.warning(f"Parameter {'COMPOSITE'} on *DAMPING is not processed.")
+        else:
+            if 'ALPHA' in property_dict['Parameters']:
+                damping_data += f"MP, ALPD, {mat_id}, {property_dict['Parameters']['ALPHA']} \n"
+            if float(property_dict['Parameters']['BETA']) != 0.0:
+                self._logger.warning(f"Parameter {'BETA'} on *DAMPING is not processed.")
+            if float(property_dict['Parameters']['COMPOSITE']) != 0.0:
+                self._logger.warning(f"Parameter {'COMPOSITE'} on *DAMPING is not processed.")
         damping_data += f"\n"
         return damping_data
 
     def _process_density(self, property_dict, material, mat_id):
         density_data = ''
+        data = []
+        if 'Data' in property_dict and property_dict['Data'] is not None:
+            data = property_dict['Data']
         if "Parameters" in property_dict and property_dict['Parameters'] is not None:
             self._logger.warning(f"Parameter on *DENSITY are not processed.")
-        density = property_dict['Data']['Mass density']
-        if 'Temperature' in property_dict['Data']:
-            temperature = property_dict['Data']['Temperature']
+        density = data['Mass density']
+        if 'Temperature' in data:
+            temperature = data['Temperature']
             if len(density) != len(temperature):
                 self._logger.warning(
                     f"data values on *DENSITY are not consistent for material {material}."
                 )
         if len(density) > 1:
             self._logger.warning(
                 f"there are multiple data values on *DENSITY, "
@@ -769,24 +776,27 @@
         else:
             density_data += f"MP,DENS,{mat_id},{density[0]}\n"
         density_data += f"\n"
         return density_data
 
     def _process_elastic_modulus(self, property_dict, material, mat_id):
         elastic_modulus = ''
+        data = []
+        if 'Data' in property_dict and property_dict['Data'] is not None:
+            data = property_dict['Data']
         if property_dict["Parameters"]["TYPE"] == "ISOTROPIC":
             # self._logger.warning(f"Only isotropic elastic modulus is processed, "
             # f"Elastic Modulus for the material {material} "
             #       f"is not processed.")
             # return ''
-            youngs_mod = property_dict['Data']['E']
-            nu = property_dict['Data']['V']
-            # temperature = property_dict['Data']['Temperature']
-            if 'Temperature' in property_dict['Data']:
-                temperature = property_dict['Data']['Temperature']
+            youngs_mod = data['E']
+            nu = data['V']
+            # temperature = data['Temperature']
+            if 'Temperature' in data:
+                temperature = data['Temperature']
                 if len(youngs_mod) != len(temperature):
                     self._logger.warning(
                         f"data values on *ELASTIC are not consistent for material {material}."
                     )
             if len(youngs_mod) != len(nu):
                 self._logger.warning(
                     f"data values on *ELASTIC are not consistent for material {material}."
@@ -816,21 +826,21 @@
             if self._material_linked_to_zone_type[material] != 'Cohesive':
                 self._logger.warning(
                     f"Elastic Modulus with type = TRACTION is defined "
                     f"for non cohesive material {material}, "
                     f" this is not processed."
                 )
                 return ''
-            knn = property_dict['Data']['E/Knn']
-            kss = property_dict['Data']['G1/Kss']
-            ktt = property_dict['Data']['G2/Ktt']
+            knn = data['E/Knn']
+            kss = data['G1/Kss']
+            ktt = data['G2/Ktt']
             t = self._cohezive_zone_thickness_data[material]['Thickness']
-            # temperature = property_dict['Data']['Temperature']
-            if 'Temperature' in property_dict['Data']:
-                temperature = property_dict['Data']['Temperature']
+            # temperature = data['Temperature']
+            if 'Temperature' in data:
+                temperature = data['Temperature']
                 if len(knn) != len(temperature):
                     self._logger.warning(
                         f"data values on *ELASTIC are not consistent for material {material}."
                     )
             if len(knn) != len(kss):
                 self._logger.warning(
                     f"data values on *ELASTIC are not consistent for material {material}."
@@ -857,53 +867,59 @@
                 f"{property_dict['Parameters']['TYPE']} is not processed."
             )
             return ''
         return elastic_modulus
 
     def _process_plastic_data(self, property_dict, material, mat_id):
         plastic_data = ''
+        data = []
+        if 'Data' in property_dict and property_dict['Data'] is not None:
+            data = property_dict['Data']
         if property_dict["Parameters"]["HARDENING"] != "ISOTROPIC":
             self._logger.warning(
                 f"Only HARDENING=ISOTROPIC is processed, "
                 f"*PLASTIC for the material {material} "
                 f"is not processed."
             )
             return ''
         if self._material_linked_to_zone_type[material] == 'Cohesive':
             return ''
-        strains = property_dict['Data']['Plastic strain']
-        stresses = property_dict['Data']['Yield stress']
-        # temperature = property_dict['Data']['Temperature']
+        strains = data['Plastic strain']
+        stresses = data['Yield stress']
+        # temperature = data['Temperature']
         data_points = len(strains)
-        if 'Temperature' in property_dict['Data']:
-            temperature = property_dict['Data']['Temperature']
+        if 'Temperature' in data:
+            temperature = data['Temperature']
             unique_temperatures = len(list(set(temperature)))
             data_points = len(strains) / unique_temperatures
             if len(stresses) != len(temperature):
                 self._logger.warning(
                     f"data values on *PLASTIC are not consistent for material {material}."
                 )
         if len(stresses) != len(strains):
             self._logger.warning(
                 f"data values on *PLASTIC are not consistent for material {material}."
             )
         plastic_data += f"TB,PLAS,{mat_id},,{int(data_points)},MISO\n"
         curr_temp = None
         for i, strain in enumerate(strains):
-            if 'Temperature' in property_dict['Data']:
+            if 'Temperature' in data:
                 if curr_temp != temperature[i]:
                     curr_temp = temperature[i]
                     plastic_data += f"TBTEMP,{curr_temp}\n"
             plastic_data += f"TBPT,,{strain},{stresses[i]}\n"
         plastic_data += f"\n"
         return plastic_data
 
     def _process_hyperelastic_data(self, property_dict, material, mat_id):
         hyperelastic_data = ''
         param_keys = property_dict["Parameters"].keys()
+        data = []
+        if 'Data' in property_dict and property_dict['Data'] is not None:
+            data = property_dict['Data']
         if (
             'REDUCED POLYNOMIAL' not in param_keys
             and 'YEOH' not in param_keys
             and 'NEO HOOKE' not in param_keys
         ):
             self._logger.warning(
                 f"Only parameter REDUCED POLYNOMIAL, "
@@ -911,64 +927,64 @@
                 f"there are more parameters on *HYPERELASTIC,*HYPERELASTIC "
                 f"for material {material} is not processed."
             )
             return ''
         if self._material_linked_to_zone_type[material] == 'Cohesive':
             return ''
         if 'NEO HOOKE' in param_keys:
-            if 'Temperature' in property_dict['Data']:
-                temperature = property_dict['Data']['Temperature']
+            if 'Temperature' in data:
+                temperature = data['Temperature']
                 temp_data_points = len(temperature)
             else:
                 self._logger.warning(
                     f"temperature is not provided for HYPERELASTIC material: {material}."
                 )
                 temp_data_points = 1
                 temperature = [None]
-            if 'C10' in property_dict['Data'].keys():
-                c10 = property_dict['Data']['C10']
-                if 'D1' in property_dict['Data'].keys():
-                    d1 = property_dict['Data']['D1']
+            if 'C10' in data.keys():
+                c10 = data['C10']
+                if 'D1' in data.keys():
+                    d1 = data['D1']
                 else:
                     d1 = [0.0] * len(c10)
             hyperelastic_data += f"TB,HYPE,{mat_id},,,NEO\n"
             for i in range(len(temperature)):
                 if temperature[i] is not None:
                     hyperelastic_data += f"TBTEMP, {temperature[i]}\n"
                 hyperelastic_data += f"TBDATA, 1, {float(c10[i])*2}, {d1[i]}\n"
         if 'REDUCED POLYNOMIAL' in param_keys or 'YEOH' in param_keys:
-            if 'Temperature' in property_dict['Data']:
-                temperature = property_dict['Data']['Temperature']
+            if 'Temperature' in data:
+                temperature = data['Temperature']
                 temp_data_points = len(temperature)
             else:
                 self._logger.warning(
                     f"temperature is not provided for HYPERELASTIC material: {material}."
                 )
                 temp_data_points = 1
                 temperature = [None]
             number_of_constants = 3
-            if 'C10' in property_dict['Data'].keys():
+            if 'C10' in data.keys():
                 number_of_constants = 1
-                c10 = property_dict['Data']['C10']
-                if 'D1' in property_dict['Data'].keys():
-                    d1 = property_dict['Data']['D1']
+                c10 = data['C10']
+                if 'D1' in data.keys():
+                    d1 = data['D1']
                 else:
                     d1 = [0.0] * len(c10)
-            if 'C20' in property_dict['Data'].keys():
+            if 'C20' in data.keys():
                 number_of_constants = 2
-                c20 = property_dict['Data']['C20']
-                if 'D2' in property_dict['Data'].keys():
-                    d2 = property_dict['Data']['D2']
+                c20 = data['C20']
+                if 'D2' in data.keys():
+                    d2 = data['D2']
                 else:
                     d2 = [0.0] * len(c20)
-            if 'C30' in property_dict['Data'].keys():
+            if 'C30' in data.keys():
                 number_of_constants = 3
-                c30 = property_dict['Data']['C30']
-                if 'D3' in property_dict['Data'].keys():
-                    d3 = property_dict['Data']['D3']
+                c30 = data['C30']
+                if 'D3' in data.keys():
+                    d3 = data['D3']
                 else:
                     d3 = [0.0] * len(c30)
             hyperelastic_data += f"TB,HYPE,{mat_id},,{number_of_constants},YEOH\n"
             for i in range(len(temperature)):
                 if temperature[i] is not None:
                     hyperelastic_data += f"TBTEMP, {temperature[i]}\n"
                 if number_of_constants == 1:
@@ -978,16 +994,16 @@
                 elif number_of_constants == 3:
                     hyperelastic_data += (
                         f"TBDATA, 1, {c10[i]}, {c20[i]}, {c30[i]}, {d1[i]}, {d2[i]}, {d3[i]}\n"
                     )
                 else:
                     pass
         # if 'REDUCED POLYNOMIAL' in param_keys:
-        #     if 'Temperature' in property_dict['Data']:
-        #         temperature = property_dict['Data']['Temperature']
+        #     if 'Temperature' in data:
+        #         temperature = data['Temperature']
         #         temp_data_points = len(temperature)
         #     else:
         #         self._logger.warning(
         # f"temperature is not provided for HYPERELASTIC material: {material}."
         # )
         #         temp_data_points = 1
         #         temperature = [None]
@@ -1404,29 +1420,32 @@
         property_dict = property_dict[0]
         comp1_str = "Length1"
         comp2_str = "Length2"
         comp3_str = "Length3"
         comp4_str = "Angle1"
         comp5_str = "Angle2"
         comp6_str = "Angle3"
+        data = []
+        if 'Data' in property_dict and property_dict['Data'] is not None:
+            data = property_dict['Data']
         # self._logger.info("property_dict")
         # self._logger.info(property_dict)
-        # self._logger.info(property_dict['Data'])
-        if comp1_str in property_dict['Data']:
-            ref_length[0] = property_dict['Data'][comp1_str]
-        if comp2_str in property_dict['Data']:
-            ref_length[1] = property_dict['Data'][comp2_str]
-        if comp3_str in property_dict['Data']:
-            ref_length[2] = property_dict['Data'][comp3_str]
-        if comp4_str in property_dict['Data']:
-            ref_length[3] = property_dict['Data'][comp4_str]
-        if comp5_str in property_dict['Data']:
-            ref_length[4] = property_dict['Data'][comp5_str]
-        if comp6_str in property_dict['Data']:
-            ref_length[5] = property_dict['Data'][comp6_str]
+        # self._logger.info(data)
+        if comp1_str in data:
+            ref_length[0] = data[comp1_str]
+        if comp2_str in data:
+            ref_length[1] = data[comp2_str]
+        if comp3_str in data:
+            ref_length[2] = data[comp3_str]
+        if comp4_str in data:
+            ref_length[3] = data[comp4_str]
+        if comp5_str in data:
+            ref_length[4] = data[comp5_str]
+        if comp6_str in data:
+            ref_length[5] = data[comp6_str]
         return ref_length
 
 
 class _BoundaryProcessor:
     __slots__ = (
         '_simulation_data',
         '_boundaries_data',
@@ -1461,14 +1480,35 @@
             boundary_commands += self._get_commands(boundary_data)
             # self._logger.info(boundary_commands)
         return boundary_commands
 
     def get_boundary_commands_by_id(self, boundary_id):
         pass
 
+    def get_boundary_comp_name_with_base_motion(self, base_motion_name):
+        boundaries_data = self._boundaries_data
+        comp_names = []
+        for boundary_data in boundaries_data:
+            if 'Parameters' in boundary_data:
+                params = boundary_data['Parameters']
+                if params is not None and 'BASE NAME' in params:
+                    if params['BASE NAME'] == base_motion_name:
+                        data_lines = boundary_data['Data']
+                        if data_lines is not None:
+                            for data_line in data_lines:
+                                comp_names.append(str(data_line['node_set']))
+                else:
+                    if base_motion_name == "":
+                        data_lines = boundary_data['Data']
+                        if data_lines is not None:
+                            for data_line in data_lines:
+                                comp_names.append(str(data_line['node_set']))
+
+        return comp_names
+
     def _get_commands(self, boundary_data):
         # self._logger.info("boundary data is ")
         # self._logger.info(boundary_data)
         boundary_commands = ''
         dof_map = {
             1: 'UX',
             2: 'UY',
@@ -2568,25 +2608,26 @@
                     nrm_key = 'ON'
             if 'RESIDUAL MODES' in data:
                 res_modes = 'ON'
                 self._previous_modal_resvec = 'ON'
         if self._simulation_data is not None:
             if "ConnectorBehavior" in self._simulation_data:
                 all_conn_behavior = self._simulation_data['ConnectorBehavior']
-                for mat in all_conn_behavior:
-                    conn_mat = all_conn_behavior[mat]
-                    if 'CONNECTOR DAMPING' in conn_mat:
-                        for conn_damp in conn_mat['CONNECTOR DAMPING']:
-                            if 'Parameters' in conn_damp:
-                                if (
-                                    "TYPE" in conn_damp['Parameters']
-                                    and conn_damp['Parameters']['TYPE'] == 'VISCOUS'
-                                ):
-                                    modopt_method = 'QRDAMP'
-                                    break
+                if all_conn_behavior:
+                    for mat in all_conn_behavior:
+                        conn_mat = all_conn_behavior[mat]
+                        if conn_mat and 'CONNECTOR DAMPING' in conn_mat:
+                            for conn_damp in conn_mat['CONNECTOR DAMPING']:
+                                if conn_damp and 'Parameters' in conn_damp:
+                                    if (
+                                        "TYPE" in conn_damp['Parameters']
+                                        and conn_damp['Parameters']['TYPE'] == 'VISCOUS'
+                                    ):
+                                        modopt_method = 'QRDAMP'
+                                        break
         frequency_analysis_commands += (
             f'! -------------------------- STEP: {self._step_counter} -----------------------\n'
         )
         if self._previous_analysis == "STATIC":
             frequency_analysis_commands += f'FINISH\n'
             frequency_analysis_commands += f'\n'
             frequency_analysis_commands += (
@@ -2717,15 +2758,15 @@
             for output in output_data:
                 if 'Data' in output and output['Data'] is not None:
                     if 'ModalOutput' in output['Data']:
                         has_modal_output = True
                         for modal_ouput in output['Data']['ModalOutput']:
                             # modal_ouput = output['ModalOutput']
                             for key in modal_ouput['Data']['keys']:
-                                if key in ["GV", "GA", "GPV", "GPA"]:
+                                if key in ["GV", "GA", "GPV", "GPA", "A1", "A2", "A3"]:
                                     has_velocities = True
         return has_modal_output, has_velocities
 
     def get_maximum_output_interval(self):
         ninterval = 0
         if "Output" in self._curr_step:
             output_data = self._curr_step["Output"]
@@ -2833,15 +2874,15 @@
                             output_analysis_commands += "0\n"
                         else:
                             output_analysis_commands += "1\n"
                 if 'NodeOutput' in output['Data']:
                     for nodeout in output['Data']['NodeOutput']:
                         # nodeout = output['NodeOutput']
                         for key in nodeout['Data']['keys']:
-                            if key in ["RF", "U", "UT"]:
+                            if key in ["RF", "U", "UT", "U1", "U2", "U3", "A1", "A2", "A3"]:
                                 output_analysis_commands += "OUTRES, "
                                 if key == "RF":
                                     output_analysis_commands += "RSOL, "
                                     if time_points is not None:
                                         output_analysis_commands += f'%{time_points}%, '
                                     else:
                                         if ninterval:
@@ -2849,15 +2890,15 @@
                                                 output_analysis_commands += f'%{ninterval}%, '
                                             else:
                                                 output_analysis_commands += f'-{ninterval}, '
                                         elif nfreq:
                                             output_analysis_commands += f'{nfreq}, '
                                         else:
                                             output_analysis_commands += 'ALL, '
-                                elif key == "U" or key == "UT":
+                                elif key in ["U", "UT", "U1", "U2", "U3", "A1", "A2", "A3"]:
                                     output_analysis_commands += "NSOL, "
                                     if time_points is not None:
                                         output_analysis_commands += f'%{time_points}%, '
                                     else:
                                         if ninterval:
                                             if number_interval_to_table:
                                                 output_analysis_commands += f'%{ninterval}%, '
@@ -3035,33 +3076,37 @@
                     for base_motion_data in base_motions_data:
                         params = base_motion_data['Parameters']
                         if len(params) == 0:
                             continue
                         base_name = ""
                         if 'BASE NAME' in params:
                             base_name = params['BASE NAME']
+                        boundaries_for_motion = self.get_step_boundary_component_data(
+                            self._curr_step["Boundary"], base_name
+                        )
                         dof = int(params['DOF'])
                         scale = 0
                         if 'SCALE' in params:
                             scale = float(params['SCALE'])
                         if self._previous_modal_resvec:
                             if count_load_vectors != 0:
                                 vector_commands += 'SOLVE\n'
                                 vector_commands += '\n'
                             vector_commands += f'FDELE, ALL, ALL \n'
                             vector_commands += f'SFDELE, ALL, ALL \n'
                             vector_commands += f'SFEDELE, ALL, ALL, ALL \n'
                             vector_commands += f'ACEL, 0, 0, 0 \n'
                             vector_commands += f'\n'
-                        vector_commands += f"F, {base_name}, {dof_map[dof]}, 1\n"
-                        count_load_vectors += 1
-                        self._modal_load_vectors[count_load_vectors] = {
-                            'SET': base_name,
-                            "COMP": dof_map[dof],
-                        }
+                        for item in boundaries_for_motion:
+                            vector_commands += f"F, {item}, {dof_map[dof]}, 1\n"
+                            count_load_vectors += 1
+                            self._modal_load_vectors[count_load_vectors] = {
+                                'SET': base_name,
+                                "COMP": dof_map[dof],
+                            }
         # else:
         # vector_commands += 'SOLVE\n'
         return vector_commands
 
     def get_step_base_motion_data(self, base_motions_data):
         # self._logger.info(f"scale_factor = {self._scale_factor}")
         # self._logger.info(f"step_start_time = {self._step_start_time}")
@@ -3136,14 +3181,27 @@
         )
         # TODO this needs to be in List of boundaries instead of single Boundary
         boundary_commands = ''
         boundary_commands += boundary_processor.get_all_boundary_commands()
         self._boundary_ampl_commands += boundary_processor.get_ampl_commands()
         return boundary_commands
 
+    def get_step_boundary_component_data(self, boundaries_data, base_name):
+        boundary_processor = _BoundaryProcessor(
+            self._model,
+            boundaries_data,
+            self._step_start_time,
+            self._step_end_time,
+            sim_data=self._simulation_data,
+        )
+        # TODO this needs to be in List of boundaries instead of single Boundary
+        comp_names = []
+        comp_names.extend(boundary_processor.get_boundary_comp_name_with_base_motion(base_name))
+        return comp_names
+
     def get_global_damping_commnads(self, global_damping_data):
         global_damping_processor = _GlobalDampingProcessing(self._model, global_damping_data)
         global_damping_commands = global_damping_processor.get_global_damping_commands(
             self._previous_analysis, self._step_MSUP
         )
         return global_damping_commands
```

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/model.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/model.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/multizonecontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/multizonecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/part.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/part.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/periodiccontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/periodiccontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/sizecontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/sizecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/surfaceutilities.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/surfaceutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/surfer.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/surfer.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/volumecontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/volumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/volumesweeper.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/volumesweeper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/wrapper.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/core/wrappercontrol.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/core/wrappercontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/examples/__init__.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/examples/download_utilities.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/examples/download_utilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/examples/examples.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/examples/examples.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/examples/unit_test_examples.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/examples/unit_test_examples.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/graphics.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/graphics.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/bin.png` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/bin.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/invert_visibility.png` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/invert_visibility.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/parts.png` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/parts.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/selectioninfo.png` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/selectioninfo.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/show_edges.png` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/show_edges.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/images/surface_body.png` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/images/surface_body.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/graphics/trame_gui.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/graphics/trame_gui.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/client.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/client.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/comm_manager.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/comm_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/communicator.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/communicator.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/config.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/config.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/defaults.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/defaults.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 if not os.path.exists(EXAMPLES_PATH):  # pragma: no cover
     os.makedirs(EXAMPLES_PATH)
 
 LOCAL_OUTDIR = os.path.join(USER_DATA_PATH, 'output')
 if not os.path.exists(LOCAL_OUTDIR):  # pragma: no cover
     os.makedirs(LOCAL_OUTDIR)
 
-CONTAINER_USER_DATA = '/data'
+CONTAINER_USER_DATA = os.getenv('PYPRIMEMESH_CONTAINER_USER_DATA ', '/data')
 CONTAINER_EXAMPLES = os.path.join(CONTAINER_USER_DATA, 'examples')
 CONTAINER_OUTDIR = os.path.join(CONTAINER_USER_DATA, 'output')
 
 __DEFAULT_IP = '127.0.0.1'
 __DEFAULT_PORT = 50055
 __DEFAULT_CONNECTION_TIMEOUT = 20.0
 __DEFAULT_COMM_LOG = False
```

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/error_handling.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/error_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ErrorCode.POLYMESHFAILED: "Poly meshing failed.",
     ErrorCode.PYRAMIDMESHFAILED: "Pyramid meshing failed.",
     ErrorCode.DELETEMESHFAILED: "Deleting mesh failed.",
     ErrorCode.INVALIDPRISMCONTROLS: "Conflict of prism settings on zonelets or invalid prism controls selected.",
     ErrorCode.PERIODICSURFACESNOTSUPPORTEDFORPRISMS: "Periodic surfaces selected for prism generation, not supported.",
     ErrorCode.ALREADYVOLUMEMESHED: "Already volume meshed.",
     ErrorCode.INCREMENTALVOLUMEMESHINGNOTSUPPORTED: "Incremental volume meshing is not supported.",
-    ErrorCode.VOLUMESNOTUPTODATE: "Volumes are not up to date. Update volumes and try again.",
+    ErrorCode.VOLUMESNOTUPTODATE: "Volumes are not up to date. Compute topovolumes for topology part or compute closed volumes for non topology parts and try again.",
     ErrorCode.QUADRATICMESHSUPPORTEDONLYFORTETS: "Quadratic meshing is supported only for tetrahedrons.",
     ErrorCode.NOACTIVESFFOUND: "Active size fields are not available.",
     ErrorCode.AITOVERLAPALONGMULTIFOUND: "Overlapping faces along multi-connection found.",
     ErrorCode.TRIANGULATIONFAILED: "Planar triangulation failed.",
     ErrorCode.TOPOFACESREMESHFAILED: "Failed to remesh some topofaces.",
     ErrorCode.PARTNOTFOUND: "Part not found.",
     ErrorCode.TOPODATANOTFOUND: "Topodata not found.",
@@ -304,14 +304,17 @@
     ErrorCode.SOURCEFACINGCELLZONELETS: "Source face zonelets facing existing volume mesh.",
     ErrorCode.TARGETWITHCELLZONELETS: "Target face zonelets with volume mesh on both sides.",
     ErrorCode.SIDEZONELETSNOTFIT: "Side face zonelets are not sweepable for thin volume mesh.",
     ErrorCode.SOURCETARGETZONELETSNOTFIT: "Source and target zonelets do not fit to thin volume mesh.",
     ErrorCode.AUTOQUADMESHER_INVALIDMINMAXSIZES: "Minimum size is more than maximum size.",
     ErrorCode.AUTOQUADMESHER_NEGATIVEINPUTPARAMETER: "Input parameters contain one or more negative values.",
     ErrorCode.FACEZONELETSHAVECELLSCONNECTED: "Face zonelets have cells connected.",
+    ErrorCode.ZEROELEMENTSREADFROMCDBFILE: "No mesh elements found. Check the input CDB file.",
+    ErrorCode.ZERONODESREADFROMCDBFILE: "No nodes found. Check the input CDB file.",
+    ErrorCode.ZEROELEMENTSFORCDBEXPORT: "No mesh elements found for CDB export. Check if the model is meshed, or set write_by_zones in ExportMapdlCdbParams to false if zones are not defined.",
 }
 
 prime_warning_messages = {
     WarningCode.NOWARNING: "Success.",
     WarningCode.UNKNOWN: "Unknown Warning.",
     WarningCode.SURFER_QUADCLEANUP_MULTITHREADINGNOTSUPPORTED: "Warning: Multithreading is skipped for quad cleanup.",
     WarningCode.SURFERLAYEREDQUADFAILED: "Surface Meshing Warning: Layered quad region has triangles.",
```

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/grpc_communicator.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/grpc_communicator.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/grpc_utils.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/grpc_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/json_utils.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/json_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/launcher.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/logger.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/prime_communicator.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/prime_communicator.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/internals/utils.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/internals/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/lucid/mesh_util.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/lucid/mesh_util.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/lucid/scope.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/lucid/scope.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/lucid/utils.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/lucid/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/params/primestructs.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/params/primestructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/relaxed_json/__init__.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/relaxed_json/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/relaxed_json/decoder.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/relaxed_json/decoder.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/relaxed_json/encoder.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/relaxed_json/encoder.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/src/ansys/meshing/prime/relaxed_json/scanner.py` & `ansys_meshing_prime-0.6.0.dev8/src/ansys/meshing/prime/relaxed_json/scanner.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.6.0.dev7/PKG-INFO` & `ansys_meshing_prime-0.6.0.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-meshing-prime
-Version: 0.6.0.dev7
+Version: 0.6.0.dev8
 Summary: PyPrimeMesh is a Python client to Ansys Prime Server, which delivers core Ansys meshing technology.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -14,20 +14,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansys-api-meshing-prime==0.1.2
 Requires-Dist: numpy>=1.14.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
 Requires-Dist: pyvista[jupyter]>=0.38.1 ; extra == "all"
-Requires-Dist: ansys-sphinx-theme==0.14.1 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
 Requires-Dist: jupyter-sphinx==0.5.3 ; extra == "doc"
-Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
+Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
 Requires-Dist: Sphinx==7.2.6 ; extra == "doc"
 Requires-Dist: pyvista==0.43.4 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==2.0.0 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==2.0.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.15.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==1.0.0 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.3.1 ; extra == "doc"
 Requires-Dist: pyvista[jupyter]>=0.38.1 ; extra == "graphics"
 Requires-Dist: pytest==8.1.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
```

