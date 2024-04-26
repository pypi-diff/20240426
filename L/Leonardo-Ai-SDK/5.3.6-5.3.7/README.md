# Comparing `tmp/Leonardo-Ai-SDK-5.3.6.tar.gz` & `tmp/Leonardo-Ai-SDK-5.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-5.3.6.tar", last modified: Wed Apr 24 00:02:32 2024, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-5.3.7.tar", last modified: Fri Apr 26 03:23:08 2024, max compression
```

## Comparing `Leonardo-Ai-SDK-5.3.6.tar` & `Leonardo-Ai-SDK-5.3.7.tar`

### file list

```diff
@@ -1,91 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     9808 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.608148 Leonardo-Ai-SDK-5.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.612148 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-24 00:02:32.000000 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-24 00:02:32.000000 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:02:32.000000 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-24 00:02:32.000000 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 00:02:32.000000 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.612148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.612148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    44786 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/initimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    27064 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.612148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.612148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/creategeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createlcmgeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createtexturegeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationnobg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationunzoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/get3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getuserself.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getvariationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/listelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/listplatformmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performinpaintinglcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performinstantrefine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/promptimprove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/promptrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploadinitimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploadmodelasset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/controlnet_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/custom_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/lcm_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/model_asset_texture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/sd_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/sd_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/strength.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/variation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13748 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:23:08.136206 Leonardo-Ai-SDK-5.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-04-26 03:23:08.136206 Leonardo-Ai-SDK-5.3.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9937 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 03:23:08.136206 Leonardo-Ai-SDK-5.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:23:08.124206 Leonardo-Ai-SDK-5.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:23:08.124206 Leonardo-Ai-SDK-5.3.7/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-04-26 03:23:07.000000 Leonardo-Ai-SDK-5.3.7/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-26 03:23:08.000000 Leonardo-Ai-SDK-5.3.7/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 03:23:07.000000 Leonardo-Ai-SDK-5.3.7/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-26 03:23:07.000000 Leonardo-Ai-SDK-5.3.7/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 03:23:07.000000 Leonardo-Ai-SDK-5.3.7/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:23:08.124206 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:23:08.128206 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44786 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/initimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27064 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:23:08.128206 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:23:08.128206 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:23:08.132206 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/creategeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createlcmgeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createtexturegeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createvariationnobg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createvariationunzoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/get3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getuserself.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/listelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/listplatformmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/performinpaintinglcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/performinstantrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/promptimprove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/promptrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/uploadinitimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/uploadmodelasset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:23:08.136206 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/controlnet_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/custom_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/lcm_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/model_asset_texture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/sd_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/strength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/universal_upscaler_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/variation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:23:08.136206 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-04-26 03:22:53.000000 Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-5.3.6/LICENSE.md` & `Leonardo-Ai-SDK-5.3.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/PKG-INFO` & `Leonardo-Ai-SDK-5.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.3.6
+Version: 5.3.7
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
@@ -98,14 +98,15 @@
         ### [prompt](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md)
         
         * [prompt_improve](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_improve) - Improve a Prompt
         * [prompt_random](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_random) - Generate a Random prompt
         
         ### [variation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md)
         
+        * [create_universal_upscaler_job](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md#create_universal_upscaler_job) - Create using Universal Upscaler
         * [create_variation_no_bg](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_no_bg) - Create no background
         * [create_variation_unzoom](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_unzoom) - Create unzoom
         * [create_variation_upscale](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_upscale) - Create upscale
         * [get_variation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md#get_variation_by_id) - Get variation by ID
         <!-- End Available Resources and Operations [operations] -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.6 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.7 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
@@ -97,14 +97,17 @@
 github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
 prompt/README.md) * [prompt_improve](https://github.com/Leonardo-Interactive/
 leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_improve) -
 Improve a Prompt * [prompt_random](https://github.com/Leonardo-Interactive/
 leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_random) -
 Generate a Random prompt ### [variation](https://github.com/Leonardo-
 Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md) *
+[create_universal_upscaler_job](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/variation/
+README.md#create_universal_upscaler_job) - Create using Universal Upscaler *
 [create_variation_no_bg](https://github.com/Leonardo-Interactive/leonardo-
 python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_no_bg) -
 Create no background * [create_variation_unzoom](https://github.com/Leonardo-
 Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
 sdks/variation/README.md#create_variation_upscale) - Create upscale *
```

### Comparing `Leonardo-Ai-SDK-5.3.6/README.md` & `Leonardo-Ai-SDK-5.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 ### [prompt](docs/sdks/prompt/README.md)
 
 * [prompt_improve](docs/sdks/prompt/README.md#prompt_improve) - Improve a Prompt
 * [prompt_random](docs/sdks/prompt/README.md#prompt_random) - Generate a Random prompt
 
 ### [variation](docs/sdks/variation/README.md)
 
+* [create_universal_upscaler_job](docs/sdks/variation/README.md#create_universal_upscaler_job) - Create using Universal Upscaler
 * [create_variation_no_bg](docs/sdks/variation/README.md#create_variation_no_bg) - Create no background
 * [create_variation_unzoom](docs/sdks/variation/README.md#create_variation_unzoom) - Create unzoom
 * [create_variation_upscale](docs/sdks/variation/README.md#create_variation_upscale) - Create upscale
 * [get_variation_by_id](docs/sdks/variation/README.md#get_variation_by_id) - Get variation by ID
 <!-- End Available Resources and Operations [operations] -->
```

#### html2text {}

```diff
@@ -54,15 +54,17 @@
 [get_model_by_id](docs/sdks/model/README.md#get_model_by_id) - Get a Single
 Custom Model by ID * [list_platform_models](docs/sdks/model/
 README.md#list_platform_models) - List Platform Models * [upload_model_asset]
 (docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model ### [prompt]
 (docs/sdks/prompt/README.md) * [prompt_improve](docs/sdks/prompt/
 README.md#prompt_improve) - Improve a Prompt * [prompt_random](docs/sdks/
 prompt/README.md#prompt_random) - Generate a Random prompt ### [variation]
-(docs/sdks/variation/README.md) * [create_variation_no_bg](docs/sdks/variation/
+(docs/sdks/variation/README.md) * [create_universal_upscaler_job](docs/sdks/
+variation/README.md#create_universal_upscaler_job) - Create using Universal
+Upscaler * [create_variation_no_bg](docs/sdks/variation/
 README.md#create_variation_no_bg) - Create no background *
 [create_variation_unzoom](docs/sdks/variation/
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (docs/sdks/variation/README.md#create_variation_upscale) - Create upscale *
 [get_variation_by_id](docs/sdks/variation/README.md#get_variation_by_id) - Get
 variation by ID ## Error Handling Handling errors in this SDK should largely
 match your expectations. All operations return a response object or raise an
```

### Comparing `Leonardo-Ai-SDK-5.3.6/setup.py` & `Leonardo-Ai-SDK-5.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='Leonardo-Ai-SDK',
-    version='5.3.6',
+    version='5.3.7',
     author='Leonardo-Ai',
     description='Leonardo AI Python Client SDK',
     url='https://github.com/Leonardo-Interactive/leonardo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-5.3.7/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.3.6
+Version: 5.3.7
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
@@ -98,14 +98,15 @@
         ### [prompt](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md)
         
         * [prompt_improve](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_improve) - Improve a Prompt
         * [prompt_random](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_random) - Generate a Random prompt
         
         ### [variation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md)
         
+        * [create_universal_upscaler_job](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md#create_universal_upscaler_job) - Create using Universal Upscaler
         * [create_variation_no_bg](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_no_bg) - Create no background
         * [create_variation_unzoom](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_unzoom) - Create unzoom
         * [create_variation_upscale](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_upscale) - Create upscale
         * [get_variation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md#get_variation_by_id) - Get variation by ID
         <!-- End Available Resources and Operations [operations] -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.6 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.7 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
@@ -97,14 +97,17 @@
 github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
 prompt/README.md) * [prompt_improve](https://github.com/Leonardo-Interactive/
 leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_improve) -
 Improve a Prompt * [prompt_random](https://github.com/Leonardo-Interactive/
 leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_random) -
 Generate a Random prompt ### [variation](https://github.com/Leonardo-
 Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md) *
+[create_universal_upscaler_job](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/variation/
+README.md#create_universal_upscaler_job) - Create using Universal Upscaler *
 [create_variation_no_bg](https://github.com/Leonardo-Interactive/leonardo-
 python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_no_bg) -
 Create no background * [create_variation_unzoom](https://github.com/Leonardo-
 Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
 sdks/variation/README.md#create_variation_upscale) - Create upscale *
```

### Comparing `Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-5.3.7/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/leonardoaisdk/models/operations/__init__.py
 src/leonardoaisdk/models/operations/createdataset.py
 src/leonardoaisdk/models/operations/creategeneration.py
 src/leonardoaisdk/models/operations/createlcmgeneration.py
 src/leonardoaisdk/models/operations/createmodel.py
 src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
 src/leonardoaisdk/models/operations/createtexturegeneration.py
+src/leonardoaisdk/models/operations/createuniversalupscalerjob.py
 src/leonardoaisdk/models/operations/createvariationnobg.py
 src/leonardoaisdk/models/operations/createvariationunzoom.py
 src/leonardoaisdk/models/operations/createvariationupscale.py
 src/leonardoaisdk/models/operations/delete3dmodelbyid.py
 src/leonardoaisdk/models/operations/deletedatasetbyid.py
 src/leonardoaisdk/models/operations/deletegenerationbyid.py
 src/leonardoaisdk/models/operations/deleteinitimagebyid.py
@@ -69,11 +70,12 @@
 src/leonardoaisdk/models/shared/lcm_generation_style.py
 src/leonardoaisdk/models/shared/model_asset_texture_types.py
 src/leonardoaisdk/models/shared/sd_generation_schedulers.py
 src/leonardoaisdk/models/shared/sd_generation_style.py
 src/leonardoaisdk/models/shared/sd_versions.py
 src/leonardoaisdk/models/shared/security.py
 src/leonardoaisdk/models/shared/strength.py
+src/leonardoaisdk/models/shared/universal_upscaler_style.py
 src/leonardoaisdk/models/shared/variation_type.py
 src/leonardoaisdk/utils/__init__.py
 src/leonardoaisdk/utils/retries.py
 src/leonardoaisdk/utils/utils.py
```

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/sdkhooks.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/types.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/dataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/element.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/element.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/generation.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/generation.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/initimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/model.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/errors/sdkerror.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from .createdataset import *
 from .creategeneration import *
 from .createlcmgeneration import *
 from .createmodel import *
 from .createsvdmotiongeneration import *
 from .createtexturegeneration import *
+from .createuniversalupscalerjob import *
 from .createvariationnobg import *
 from .createvariationunzoom import *
 from .createvariationupscale import *
 from .delete3dmodelbyid import *
 from .deletedatasetbyid import *
 from .deletegenerationbyid import *
 from .deleteinitimagebyid import *
@@ -34,8 +35,8 @@
 from .promptimprove import *
 from .promptrandom import *
 from .uploaddatasetimage import *
 from .uploaddatasetimagefromgen import *
 from .uploadinitimage import *
 from .uploadmodelasset import *
 
-__all__ = ["CreateDatasetRequestBody","CreateDatasetResponse","CreateDatasetResponseBody","CreateGenerationRequestBody","CreateGenerationResponse","CreateGenerationResponseBody","CreateLCMGenerationRequestBody","CreateLCMGenerationResponse","CreateLCMGenerationResponseBody","CreateModelRequestBody","CreateModelResponse","CreateModelResponseBody","CreateSVDMotionGenerationRequestBody","CreateSVDMotionGenerationResponse","CreateSVDMotionGenerationResponseBody","CreateTextureGenerationRequestBody","CreateTextureGenerationResponse","CreateTextureGenerationResponseBody","CreateVariationNoBGRequestBody","CreateVariationNoBGResponse","CreateVariationNoBGResponseBody","CreateVariationUnzoomRequestBody","CreateVariationUnzoomResponse","CreateVariationUnzoomResponseBody","CreateVariationUpscaleRequestBody","CreateVariationUpscaleResponse","CreateVariationUpscaleResponseBody","CreateVariationUpscaleSDUpscaleJobOutput","CustomModels","DatasetGenUploadOutput","DatasetImages","DatasetUploadOutput","Datasets","Delete3DModelByIDRequest","Delete3DModelByIDRequestBody","Delete3DModelByIDResponse","Delete3DModelByIDResponseBody","DeleteDatasetByIDDatasets","DeleteDatasetByIDRequest","DeleteDatasetByIDResponse","DeleteDatasetByIDResponseBody","DeleteGenerationByIDRequest","DeleteGenerationByIDResponse","DeleteGenerationByIDResponseBody","DeleteInitImageByIDRequest","DeleteInitImageByIDResponse","DeleteInitImageByIDResponseBody","DeleteModelByIDRequest","DeleteModelByIDResponse","DeleteModelByIDResponseBody","DeleteTextureGenerationByIDRequest","DeleteTextureGenerationByIDRequestBody","DeleteTextureGenerationByIDResponse","DeleteTextureGenerationByIDResponseBody","Elements","GeneratedImageVariationGeneric","GeneratedImages","GenerationElements","Generations","Get3DModelByIDModelAssets","Get3DModelByIDRequest","Get3DModelByIDRequestBody","Get3DModelByIDResponse","Get3DModelByIDResponseBody","Get3DModelsByUserIDModelAssets","Get3DModelsByUserIDRequest","Get3DModelsByUserIDRequestBody","Get3DModelsByUserIDResponse","Get3DModelsByUserIDResponseBody","GetDatasetByIDDatasets","GetDatasetByIDRequest","GetDatasetByIDResponse","GetDatasetByIDResponseBody","GetGenerationByIDGeneratedImageVariationGeneric","GetGenerationByIDGenerations","GetGenerationByIDLoras","GetGenerationByIDRequest","GetGenerationByIDResponse","GetGenerationByIDResponseBody","GetGenerationsByUserIDGeneratedImageVariationGeneric","GetGenerationsByUserIDGeneratedImages","GetGenerationsByUserIDGenerationElements","GetGenerationsByUserIDGenerations","GetGenerationsByUserIDRequest","GetGenerationsByUserIDResponse","GetGenerationsByUserIDResponseBody","GetInitImageByIDInitImages","GetInitImageByIDRequest","GetInitImageByIDResponse","GetInitImageByIDResponseBody","GetModelByIDCustomModels","GetModelByIDRequest","GetModelByIDResponse","GetModelByIDResponseBody","GetTextureGenerationByIDModelAssetTextureGenerations","GetTextureGenerationByIDRequest","GetTextureGenerationByIDRequestBody","GetTextureGenerationByIDResponse","GetTextureGenerationByIDResponseBody","GetTextureGenerationsByModelIDModelAssetTextureGenerations","GetTextureGenerationsByModelIDModelAssetTextureImages","GetTextureGenerationsByModelIDRequest","GetTextureGenerationsByModelIDRequestBody","GetTextureGenerationsByModelIDResponse","GetTextureGenerationsByModelIDResponseBody","GetUserSelfResponse","GetUserSelfResponseBody","GetVariationByIDRequest","GetVariationByIDResponse","GetVariationByIDResponseBody","InitImageUploadOutput","InitImages","LcmGenerationOutput","ListElementsResponse","ListElementsResponseBody","ListPlatformModelsCustomModels","ListPlatformModelsGeneratedImages","ListPlatformModelsResponse","ListPlatformModelsResponseBody","Loras","ModelAssetTextureGenerations","ModelAssetTextureImages","ModelAssetUploadOutput","ModelAssets","MotionSvdGenerationOutput","PerformAlchemyUpscaleLCMLCMGenerationOutput","PerformAlchemyUpscaleLCMRequestBody","PerformAlchemyUpscaleLCMResponse","PerformAlchemyUpscaleLCMResponseBody","PerformInpaintingLCMLCMGenerationOutput","PerformInpaintingLCMRequestBody","PerformInpaintingLCMResponse","PerformInpaintingLCMResponseBody","PerformInstantRefineLcmGenerationOutput","PerformInstantRefineRequestBody","PerformInstantRefineResponse","PerformInstantRefineResponseBody","PromptGenerationOutput","PromptImproveRequestBody","PromptImproveResponse","PromptImproveResponseBody","PromptRandomPromptGenerationOutput","PromptRandomResponse","PromptRandomResponseBody","SDGenerationOutput","SDTrainingOutput","SDUnzoomOutput","SDUpscaleJobOutput","TextureGenerationJobOutput","TransparencyType","UploadDatasetImageFromGenRequest","UploadDatasetImageFromGenRequestBody","UploadDatasetImageFromGenResponse","UploadDatasetImageFromGenResponseBody","UploadDatasetImageRequest","UploadDatasetImageRequestBody","UploadDatasetImageResponse","UploadDatasetImageResponseBody","UploadInitImageRequestBody","UploadInitImageResponse","UploadInitImageResponseBody","UploadModelAssetRequestBody","UploadModelAssetResponse","UploadModelAssetResponseBody","UserDetails","Users"]
+__all__ = ["CreateDatasetRequestBody","CreateDatasetResponse","CreateDatasetResponseBody","CreateGenerationRequestBody","CreateGenerationResponse","CreateGenerationResponseBody","CreateLCMGenerationRequestBody","CreateLCMGenerationResponse","CreateLCMGenerationResponseBody","CreateModelRequestBody","CreateModelResponse","CreateModelResponseBody","CreateSVDMotionGenerationRequestBody","CreateSVDMotionGenerationResponse","CreateSVDMotionGenerationResponseBody","CreateTextureGenerationRequestBody","CreateTextureGenerationResponse","CreateTextureGenerationResponseBody","CreateUniversalUpscalerJobRequestBody","CreateUniversalUpscalerJobResponse","CreateUniversalUpscalerJobResponseBody","CreateVariationNoBGRequestBody","CreateVariationNoBGResponse","CreateVariationNoBGResponseBody","CreateVariationUnzoomRequestBody","CreateVariationUnzoomResponse","CreateVariationUnzoomResponseBody","CreateVariationUpscaleRequestBody","CreateVariationUpscaleResponse","CreateVariationUpscaleResponseBody","CreateVariationUpscaleSDUpscaleJobOutput","CustomModels","DatasetGenUploadOutput","DatasetImages","DatasetUploadOutput","Datasets","Delete3DModelByIDRequest","Delete3DModelByIDRequestBody","Delete3DModelByIDResponse","Delete3DModelByIDResponseBody","DeleteDatasetByIDDatasets","DeleteDatasetByIDRequest","DeleteDatasetByIDResponse","DeleteDatasetByIDResponseBody","DeleteGenerationByIDRequest","DeleteGenerationByIDResponse","DeleteGenerationByIDResponseBody","DeleteInitImageByIDRequest","DeleteInitImageByIDResponse","DeleteInitImageByIDResponseBody","DeleteModelByIDRequest","DeleteModelByIDResponse","DeleteModelByIDResponseBody","DeleteTextureGenerationByIDRequest","DeleteTextureGenerationByIDRequestBody","DeleteTextureGenerationByIDResponse","DeleteTextureGenerationByIDResponseBody","Elements","GeneratedImageVariationGeneric","GeneratedImages","GenerationElements","Generations","Get3DModelByIDModelAssets","Get3DModelByIDRequest","Get3DModelByIDRequestBody","Get3DModelByIDResponse","Get3DModelByIDResponseBody","Get3DModelsByUserIDModelAssets","Get3DModelsByUserIDRequest","Get3DModelsByUserIDRequestBody","Get3DModelsByUserIDResponse","Get3DModelsByUserIDResponseBody","GetDatasetByIDDatasets","GetDatasetByIDRequest","GetDatasetByIDResponse","GetDatasetByIDResponseBody","GetGenerationByIDGeneratedImageVariationGeneric","GetGenerationByIDGenerations","GetGenerationByIDLoras","GetGenerationByIDRequest","GetGenerationByIDResponse","GetGenerationByIDResponseBody","GetGenerationsByUserIDGeneratedImageVariationGeneric","GetGenerationsByUserIDGeneratedImages","GetGenerationsByUserIDGenerationElements","GetGenerationsByUserIDGenerations","GetGenerationsByUserIDRequest","GetGenerationsByUserIDResponse","GetGenerationsByUserIDResponseBody","GetInitImageByIDInitImages","GetInitImageByIDRequest","GetInitImageByIDResponse","GetInitImageByIDResponseBody","GetModelByIDCustomModels","GetModelByIDRequest","GetModelByIDResponse","GetModelByIDResponseBody","GetTextureGenerationByIDModelAssetTextureGenerations","GetTextureGenerationByIDRequest","GetTextureGenerationByIDRequestBody","GetTextureGenerationByIDResponse","GetTextureGenerationByIDResponseBody","GetTextureGenerationsByModelIDModelAssetTextureGenerations","GetTextureGenerationsByModelIDModelAssetTextureImages","GetTextureGenerationsByModelIDRequest","GetTextureGenerationsByModelIDRequestBody","GetTextureGenerationsByModelIDResponse","GetTextureGenerationsByModelIDResponseBody","GetUserSelfResponse","GetUserSelfResponseBody","GetVariationByIDRequest","GetVariationByIDResponse","GetVariationByIDResponseBody","InitImageUploadOutput","InitImages","LcmGenerationOutput","ListElementsResponse","ListElementsResponseBody","ListPlatformModelsCustomModels","ListPlatformModelsGeneratedImages","ListPlatformModelsResponse","ListPlatformModelsResponseBody","Loras","ModelAssetTextureGenerations","ModelAssetTextureImages","ModelAssetUploadOutput","ModelAssets","MotionSvdGenerationOutput","PerformAlchemyUpscaleLCMLCMGenerationOutput","PerformAlchemyUpscaleLCMRequestBody","PerformAlchemyUpscaleLCMResponse","PerformAlchemyUpscaleLCMResponseBody","PerformInpaintingLCMLCMGenerationOutput","PerformInpaintingLCMRequestBody","PerformInpaintingLCMResponse","PerformInpaintingLCMResponseBody","PerformInstantRefineLcmGenerationOutput","PerformInstantRefineRequestBody","PerformInstantRefineResponse","PerformInstantRefineResponseBody","PromptGenerationOutput","PromptImproveRequestBody","PromptImproveResponse","PromptImproveResponseBody","PromptRandomPromptGenerationOutput","PromptRandomResponse","PromptRandomResponseBody","SDGenerationOutput","SDTrainingOutput","SDUnzoomOutput","SDUpscaleJobOutput","TextureGenerationJobOutput","TransparencyType","UniversalUpscalerOutput","UploadDatasetImageFromGenRequest","UploadDatasetImageFromGenRequestBody","UploadDatasetImageFromGenResponse","UploadDatasetImageFromGenResponseBody","UploadDatasetImageRequest","UploadDatasetImageRequestBody","UploadDatasetImageResponse","UploadDatasetImageResponseBody","UploadInitImageRequestBody","UploadInitImageResponse","UploadInitImageResponseBody","UploadModelAssetRequestBody","UploadModelAssetResponse","UploadModelAssetResponseBody","UserDetails","Users"]
```

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createlcmgeneration.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createlcmgeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createtexturegeneration.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createtexturegeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationnobg.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createvariationnobg.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationunzoom.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createvariationunzoom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/delete3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/delete3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/get3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/get3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/listelements.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/listelements.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/listplatformmodels.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/listplatformmodels.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performinpaintinglcm.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/performinpaintinglcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performinstantrefine.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/performinstantrefine.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/promptimprove.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/promptimprove.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/promptrandom.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/promptrandom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploadmodelasset.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/operations/uploadmodelasset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/element_input.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/element_input.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/lcm_generation_style.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/lcm_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/sd_generation_style.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/sd_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/sd_versions.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/models/shared/sd_versions.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/prompt.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/prompt.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/sdk.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '5.3.6'
-    gen_version: str = '2.312.0'
-    user_agent: str = 'speakeasy-sdk/python 5.3.6 2.312.0 v1.0.0 Leonardo-Ai-SDK'
+    sdk_version: str = '5.3.7'
+    gen_version: str = '2.312.1'
+    user_agent: str = 'speakeasy-sdk/python 5.3.7 2.312.1 v1.0.0 Leonardo-Ai-SDK'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/user.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-5.3.7/src/leonardoaisdk/variation.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,75 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
+    def create_universal_upscaler_job(self, request: operations.CreateUniversalUpscalerJobRequestBody) -> operations.CreateUniversalUpscalerJobResponse:
+        r"""Create using Universal Upscaler
+        This endpoint will create a high resolution image using Universal Upscaler
+        """
+        hook_ctx = HookContext(operation_id='CreateUniversalUpscalerJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = base_url + '/variations/universal-upscaler'
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateUniversalUpscalerJobRequestBody, "request", False, False, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        try:
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
+        else:
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
+        
+        
+        res = operations.CreateUniversalUpscalerJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateUniversalUpscalerJobResponseBody])
+                res.object = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+        return res
+
+    
+    
     def create_variation_no_bg(self, request: operations.CreateVariationNoBGRequestBody) -> operations.CreateVariationNoBGResponse:
         r"""Create no background
         This endpoint will create a no background variation of the provided image ID
         """
         hook_ctx = HookContext(operation_id='createVariationNoBG', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
```

