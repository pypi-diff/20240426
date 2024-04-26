# Comparing `tmp/opticallyshallowdeep-1.2.0.tar.gz` & `tmp/opticallyshallowdeep-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opticallyshallowdeep-1.2.0.tar", last modified: Sun Mar 24 18:48:58 2024, max compression
+gzip compressed data, was "opticallyshallowdeep-1.2.1.tar", last modified: Fri Apr 26 01:47:15 2024, max compression
```

## Comparing `opticallyshallowdeep-1.2.0.tar` & `opticallyshallowdeep-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-24 18:48:58.778664 opticallyshallowdeep-1.2.0/
--rw-r--r--   0 yw         (501) staff       (20)    35129 2024-03-08 23:19:25.000000 opticallyshallowdeep-1.2.0/LICENSE
--rw-r--r--   0 yw         (501) staff       (20)       43 2024-03-09 22:47:55.000000 opticallyshallowdeep-1.2.0/MANIFEST.in
--rw-r--r--   0 yw         (501) staff       (20)     3222 2024-03-24 18:48:58.778448 opticallyshallowdeep-1.2.0/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     2661 2024-03-24 04:04:59.000000 opticallyshallowdeep-1.2.0/README.md
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-24 18:48:58.775867 opticallyshallowdeep-1.2.0/opticallyshallowdeep/
--rw-r--r--   0 yw         (501) staff       (20)       20 2024-03-16 21:56:23.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)      221 2024-03-24 18:44:59.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/check_transpose.py
--rw-r--r--   0 yw         (501) staff       (20)     3566 2024-03-24 18:44:54.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/cloud_mask.py
--rw-r--r--   0 yw         (501) staff       (20)     1025 2024-03-16 21:56:49.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/find_epsg.py
--rw-r--r--   0 yw         (501) staff       (20)     2122 2024-03-18 00:36:33.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/make_multiband_image.py
--rw-r--r--   0 yw         (501) staff       (20)     1623 2024-03-24 03:11:28.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/make_vertical_strips.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-24 18:48:58.777706 opticallyshallowdeep-1.2.0/opticallyshallowdeep/models/
--rw-r--r--   0 yw         (501) staff       (20)   212192 2024-01-27 04:43:28.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/models/SR.h5
--rw-r--r--   0 yw         (501) staff       (20)   137376 2024-01-26 22:31:46.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/models/TOA.h5
--rw-r--r--   0 yw         (501) staff       (20)     3337 2024-03-24 14:56:21.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/netcdf_to_multiband_geotiff.py
--rw-r--r--   0 yw         (501) staff       (20)      942 2024-03-16 21:58:52.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/parse_string.py
--rw-r--r--   0 yw         (501) staff       (20)    21501 2024-03-24 04:13:22.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/process_as_strips.py
--rw-r--r--   0 yw         (501) staff       (20)     4379 2024-03-24 18:44:29.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/run.py
--rw-r--r--   0 yw         (501) staff       (20)      961 2024-03-24 04:09:42.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep/write_georef_image.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-24 18:48:58.776494 opticallyshallowdeep-1.2.0/opticallyshallowdeep.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)     3222 2024-03-24 18:48:58.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)      760 2024-03-24 18:48:58.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2024-03-24 18:48:58.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       90 2024-03-24 18:48:58.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)       21 2024-03-24 18:48:58.000000 opticallyshallowdeep-1.2.0/opticallyshallowdeep.egg-info/top_level.txt
--rw-r--r--   0 yw         (501) staff       (20)       38 2024-03-24 18:48:58.778706 opticallyshallowdeep-1.2.0/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)      865 2024-03-24 18:46:31.000000 opticallyshallowdeep-1.2.0/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 01:47:15.248676 opticallyshallowdeep-1.2.1/
+-rw-r--r--   0 yw         (501) staff       (20)    35129 2024-03-08 23:19:25.000000 opticallyshallowdeep-1.2.1/LICENSE
+-rw-r--r--   0 yw         (501) staff       (20)       43 2024-03-09 22:47:55.000000 opticallyshallowdeep-1.2.1/MANIFEST.in
+-rw-r--r--   0 yw         (501) staff       (20)     3273 2024-04-26 01:47:15.248468 opticallyshallowdeep-1.2.1/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     2712 2024-04-26 01:33:33.000000 opticallyshallowdeep-1.2.1/README.md
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 01:47:15.245884 opticallyshallowdeep-1.2.1/opticallyshallowdeep/
+-rw-r--r--   0 yw         (501) staff       (20)       20 2024-03-16 21:56:23.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)      221 2024-03-24 18:44:59.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/check_transpose.py
+-rw-r--r--   0 yw         (501) staff       (20)     3566 2024-03-24 18:44:54.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/cloud_mask.py
+-rw-r--r--   0 yw         (501) staff       (20)     1025 2024-03-16 21:56:49.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/find_epsg.py
+-rw-r--r--   0 yw         (501) staff       (20)     2122 2024-03-18 00:36:33.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/make_multiband_image.py
+-rw-r--r--   0 yw         (501) staff       (20)     1623 2024-03-24 03:11:28.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/make_vertical_strips.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 01:47:15.247725 opticallyshallowdeep-1.2.1/opticallyshallowdeep/models/
+-rw-r--r--   0 yw         (501) staff       (20)   212192 2024-01-27 04:43:28.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/models/SR.h5
+-rw-r--r--   0 yw         (501) staff       (20)   137376 2024-01-26 22:31:46.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/models/TOA.h5
+-rw-r--r--   0 yw         (501) staff       (20)     3337 2024-03-24 14:56:21.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/netcdf_to_multiband_geotiff.py
+-rw-r--r--   0 yw         (501) staff       (20)      942 2024-03-16 21:58:52.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/parse_string.py
+-rw-r--r--   0 yw         (501) staff       (20)    21531 2024-04-26 01:19:20.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/process_as_strips.py
+-rw-r--r--   0 yw         (501) staff       (20)     4508 2024-04-25 20:25:47.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/run.py
+-rw-r--r--   0 yw         (501) staff       (20)      961 2024-03-24 04:09:42.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep/write_georef_image.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-26 01:47:15.246545 opticallyshallowdeep-1.2.1/opticallyshallowdeep.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)     3273 2024-04-26 01:47:15.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)      760 2024-04-26 01:47:15.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2024-04-26 01:47:15.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       90 2024-04-26 01:47:15.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)       21 2024-04-26 01:47:15.000000 opticallyshallowdeep-1.2.1/opticallyshallowdeep.egg-info/top_level.txt
+-rw-r--r--   0 yw         (501) staff       (20)       38 2024-04-26 01:47:15.248720 opticallyshallowdeep-1.2.1/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)      865 2024-04-26 01:46:33.000000 opticallyshallowdeep-1.2.1/setup.py
```

### Comparing `opticallyshallowdeep-1.2.0/LICENSE` & `opticallyshallowdeep-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/PKG-INFO` & `opticallyshallowdeep-1.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,12 @@
-Metadata-Version: 2.1
-Name: opticallyshallowdeep
-Version: 1.2.0
-Summary: Identify optically shallow and deep waters in satellite imagery
-Author: Yulun Wu
-Author-email: yulunwu8@gmail.com
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: geopandas
-Requires-Dist: rasterio
-Requires-Dist: tifffile
-Requires-Dist: netCDF4
-Requires-Dist: pyproj
-Requires-Dist: joblib
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: imagecodecs
-Requires-Dist: tensorflow
-
 # Optically-Shallow-Deep 
 
 This python tool delineates optically shallow and deep waters in Sentinel-2 imagery. The tool uses a deep neural network (DNN) that was trained on a diverse set of global images.
 
-Supported input includes L1C SAFE files and ACOLITE-processed L2R netCDF files. The output geotiff contains probabilities of water pixels being optically shallow and deep. 
+Supported input includes Level-1C (L1C) SAFE files and ACOLITE-processed L2R netCDF files. The output geotiff contains probabilities of water pixels being optically shallow and deep. 
 
 Originally coded by by Galen Richardson and Anders Knudby, modified and packaged by Yulun Wu
 
 Home page: <a href="https://github.com/yulunwu8/Optically-Shallow-Deep" target="_blank">https://github.com/yulunwu8/Optically-Shallow-Deep</a>
 
 
  
@@ -43,30 +22,21 @@
 **2 - Install tensorflow**
 
 For mac OS: 
 
 ```bash
 conda install -c apple tensorflow-deps
 python -m pip install tensorflow-macos
-
 ```
 
 
 For windows:
 
 ```bash
 pip3 install tensorflow==2.13.0
-
-```
-
-In case of compatibility issues, please try the newest version of tensorflow: 
-
-```bash
-pip3 install --upgrade --force-reinstall tensorflow
-
 ```
 
 
 For Linux and more on installing tensorflow: [https://www.tensorflow.org/install](https://www.tensorflow.org/install)
 
 
 **3 - Install opticallyshallowdeep:**
@@ -102,24 +72,31 @@
 file_L1C = 'test_folder_in/S2.SAFE' 
 file_L2R = 'test_folder_in/L2R.nc' 
 
 # Output folder 
 folder_out = 'folder/test_folder_out'
 
 # Run the OSW/ODW classifier 
-osd.run(file_in, folder_out, file_L2R=file_L2R)
+osd.run(file_L1C, folder_out, file_L2R=file_L2R)
 ```
 
-The L1C file is always required as it contains a cloud mask. Pixels within 8 pixels of the cloud mask are masked to reduce the impact of clouds. 
+The L1C file is always required as it contains a built-in cloud mask. Pixels within 8 pixels of the cloud mask are masked to reduce the impact of clouds. 
 
 
-Output is a 1-band geotiff, with values of prediction probability of OSW (100 means most likely OSW, 0 means most likely ODW). Non-water pixels are masked. It is recommended to use pixels between 0 and 40 as ODW, and pixels between 60 and 100 as OSW (publication in review).
+Output is a 1-band geotiff, with values of prediction probability of optically shallow water (OSW): 100 means most likely OSW, 0 means most likely optically deep water (ODW). Non-water pixels are masked. It is recommended to treat pixels between 0 and 40 as ODW, and pixels between 60 and 100 as OSW (publication in review).
 
 A log file, an intermediate multi-band geotiff, and a preview PNG are also generated in the output folder. They can be deleted after the processing. 
 
+
+**Sample Sentinel-2 scene and output:**
+
+<img src="images/TOA.jpeg"  height="500">
+
+<img src="images/OSW.jpeg"  height="500">
+
 ## Training, test, and validation data 
 
 All annotated shapefiles used in training, testing, and validating the DNN model are in the annotated_shapefiles folder, grouped by Sentinel-2 Scene ID.
```

#### html2text {}

```diff
@@ -1,40 +1,33 @@
-Metadata-Version: 2.1 Name: opticallyshallowdeep Version: 1.2.0 Summary:
-Identify optically shallow and deep waters in satellite imagery Author: Yulun
-Wu Author-email: yulunwu8@gmail.com Classifier: Programming Language :: Python
-:: 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: geopandas Requires-Dist: rasterio Requires-Dist:
-tifffile Requires-Dist: netCDF4 Requires-Dist: pyproj Requires-Dist: joblib
-Requires-Dist: scipy Requires-Dist: matplotlib Requires-Dist: imagecodecs
-Requires-Dist: tensorflow # Optically-Shallow-Deep This python tool delineates
-optically shallow and deep waters in Sentinel-2 imagery. The tool uses a deep
-neural network (DNN) that was trained on a diverse set of global images.
-Supported input includes L1C SAFE files and ACOLITE-processed L2R netCDF files.
-The output geotiff contains probabilities of water pixels being optically
-shallow and deep. Originally coded by by Galen Richardson and Anders Knudby,
-modified and packaged by Yulun Wu Home page: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_y_u_l_u_n_w_u_8_/
-_O_p_t_i_c_a_l_l_y_-_S_h_a_l_l_o_w_-_D_e_e_p ## Installation **1 - Create a conda environment and
-activate it:** ```bash conda create --name opticallyshallowdeep python=3.10
-conda activate opticallyshallowdeep ``` **2 - Install tensorflow** For mac OS:
-```bash conda install -c apple tensorflow-deps python -m pip install
-tensorflow-macos ``` For windows: ```bash pip3 install tensorflow==2.13.0 ```
-In case of compatibility issues, please try the newest version of tensorflow:
-```bash pip3 install --upgrade --force-reinstall tensorflow ``` For Linux and
-more on installing tensorflow: [https://www.tensorflow.org/install](https://
+# Optically-Shallow-Deep This python tool delineates optically shallow and deep
+waters in Sentinel-2 imagery. The tool uses a deep neural network (DNN) that
+was trained on a diverse set of global images. Supported input includes Level-
+1C (L1C) SAFE files and ACOLITE-processed L2R netCDF files. The output geotiff
+contains probabilities of water pixels being optically shallow and deep.
+Originally coded by by Galen Richardson and Anders Knudby, modified and
+packaged by Yulun Wu Home page: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_y_u_l_u_n_w_u_8_/_O_p_t_i_c_a_l_l_y_-_S_h_a_l_l_o_w_-
+_D_e_e_p ## Installation **1 - Create a conda environment and activate it:**
+```bash conda create --name opticallyshallowdeep python=3.10 conda activate
+opticallyshallowdeep ``` **2 - Install tensorflow** For mac OS: ```bash conda
+install -c apple tensorflow-deps python -m pip install tensorflow-macos ``` For
+windows: ```bash pip3 install tensorflow==2.13.0 ``` For Linux and more on
+installing tensorflow: [https://www.tensorflow.org/install](https://
 www.tensorflow.org/install) **3 - Install opticallyshallowdeep:** ```bash pip3
 install opticallyshallowdeep ``` ## Quick Start For L1C files: ```python import
 opticallyshallowdeep as osd # Input file file_L1C = 'folder/S2.SAFE' # Output
 folder folder_out = 'folder/test_folder_out' # Run the OSW/ODW classifier
 osd.run(file_L1C, folder_out) ``` For ACOLITE L2R files: ```python import
 opticallyshallowdeep as osd # Input files file_L1C = 'test_folder_in/S2.SAFE'
 file_L2R = 'test_folder_in/L2R.nc' # Output folder folder_out = 'folder/
-test_folder_out' # Run the OSW/ODW classifier osd.run(file_in, folder_out,
-file_L2R=file_L2R) ``` The L1C file is always required as it contains a cloud
-mask. Pixels within 8 pixels of the cloud mask are masked to reduce the impact
-of clouds. Output is a 1-band geotiff, with values of prediction probability of
-OSW (100 means most likely OSW, 0 means most likely ODW). Non-water pixels are
-masked. It is recommended to use pixels between 0 and 40 as ODW, and pixels
-between 60 and 100 as OSW (publication in review). A log file, an intermediate
-multi-band geotiff, and a preview PNG are also generated in the output folder.
-They can be deleted after the processing. ## Training, test, and validation
-data All annotated shapefiles used in training, testing, and validating the DNN
-model are in the annotated_shapefiles folder, grouped by Sentinel-2 Scene ID.
+test_folder_out' # Run the OSW/ODW classifier osd.run(file_L1C, folder_out,
+file_L2R=file_L2R) ``` The L1C file is always required as it contains a built-
+in cloud mask. Pixels within 8 pixels of the cloud mask are masked to reduce
+the impact of clouds. Output is a 1-band geotiff, with values of prediction
+probability of optically shallow water (OSW): 100 means most likely OSW, 0
+means most likely optically deep water (ODW). Non-water pixels are masked. It
+is recommended to treat pixels between 0 and 40 as ODW, and pixels between 60
+and 100 as OSW (publication in review). A log file, an intermediate multi-band
+geotiff, and a preview PNG are also generated in the output folder. They can be
+deleted after the processing. **Sample Sentinel-2 scene and output:** [images/
+TOA.jpeg][images/OSW.jpeg]## Training, test, and validation data All annotated
+shapefiles used in training, testing, and validating the DNN model are in the
+annotated_shapefiles folder, grouped by Sentinel-2 Scene ID.
```

### Comparing `opticallyshallowdeep-1.2.0/README.md` & `opticallyshallowdeep-1.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,33 @@
+Metadata-Version: 2.1
+Name: opticallyshallowdeep
+Version: 1.2.1
+Summary: Identify optically shallow and deep waters in satellite imagery
+Author: Yulun Wu
+Author-email: yulunwu8@gmail.com
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: geopandas
+Requires-Dist: rasterio
+Requires-Dist: tifffile
+Requires-Dist: netCDF4
+Requires-Dist: pyproj
+Requires-Dist: joblib
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: imagecodecs
+Requires-Dist: tensorflow
+
 # Optically-Shallow-Deep 
 
 This python tool delineates optically shallow and deep waters in Sentinel-2 imagery. The tool uses a deep neural network (DNN) that was trained on a diverse set of global images.
 
-Supported input includes L1C SAFE files and ACOLITE-processed L2R netCDF files. The output geotiff contains probabilities of water pixels being optically shallow and deep. 
+Supported input includes Level-1C (L1C) SAFE files and ACOLITE-processed L2R netCDF files. The output geotiff contains probabilities of water pixels being optically shallow and deep. 
 
 Originally coded by by Galen Richardson and Anders Knudby, modified and packaged by Yulun Wu
 
 Home page: <a href="https://github.com/yulunwu8/Optically-Shallow-Deep" target="_blank">https://github.com/yulunwu8/Optically-Shallow-Deep</a>
 
 
  
@@ -22,30 +43,21 @@
 **2 - Install tensorflow**
 
 For mac OS: 
 
 ```bash
 conda install -c apple tensorflow-deps
 python -m pip install tensorflow-macos
-
 ```
 
 
 For windows:
 
 ```bash
 pip3 install tensorflow==2.13.0
-
-```
-
-In case of compatibility issues, please try the newest version of tensorflow: 
-
-```bash
-pip3 install --upgrade --force-reinstall tensorflow
-
 ```
 
 
 For Linux and more on installing tensorflow: [https://www.tensorflow.org/install](https://www.tensorflow.org/install)
 
 
 **3 - Install opticallyshallowdeep:**
@@ -81,24 +93,31 @@
 file_L1C = 'test_folder_in/S2.SAFE' 
 file_L2R = 'test_folder_in/L2R.nc' 
 
 # Output folder 
 folder_out = 'folder/test_folder_out'
 
 # Run the OSW/ODW classifier 
-osd.run(file_in, folder_out, file_L2R=file_L2R)
+osd.run(file_L1C, folder_out, file_L2R=file_L2R)
 ```
 
-The L1C file is always required as it contains a cloud mask. Pixels within 8 pixels of the cloud mask are masked to reduce the impact of clouds. 
+The L1C file is always required as it contains a built-in cloud mask. Pixels within 8 pixels of the cloud mask are masked to reduce the impact of clouds. 
 
 
-Output is a 1-band geotiff, with values of prediction probability of OSW (100 means most likely OSW, 0 means most likely ODW). Non-water pixels are masked. It is recommended to use pixels between 0 and 40 as ODW, and pixels between 60 and 100 as OSW (publication in review).
+Output is a 1-band geotiff, with values of prediction probability of optically shallow water (OSW): 100 means most likely OSW, 0 means most likely optically deep water (ODW). Non-water pixels are masked. It is recommended to treat pixels between 0 and 40 as ODW, and pixels between 60 and 100 as OSW (publication in review).
 
 A log file, an intermediate multi-band geotiff, and a preview PNG are also generated in the output folder. They can be deleted after the processing. 
 
+
+**Sample Sentinel-2 scene and output:**
+
+<img src="images/TOA.jpeg"  height="500">
+
+<img src="images/OSW.jpeg"  height="500">
+
 ## Training, test, and validation data 
 
 All annotated shapefiles used in training, testing, and validating the DNN model are in the annotated_shapefiles folder, grouped by Sentinel-2 Scene ID.
```

#### html2text {}

```diff
@@ -1,33 +1,41 @@
-# Optically-Shallow-Deep This python tool delineates optically shallow and deep
-waters in Sentinel-2 imagery. The tool uses a deep neural network (DNN) that
-was trained on a diverse set of global images. Supported input includes L1C
-SAFE files and ACOLITE-processed L2R netCDF files. The output geotiff contains
-probabilities of water pixels being optically shallow and deep. Originally
-coded by by Galen Richardson and Anders Knudby, modified and packaged by Yulun
-Wu Home page: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_y_u_l_u_n_w_u_8_/_O_p_t_i_c_a_l_l_y_-_S_h_a_l_l_o_w_-_D_e_e_p ##
-Installation **1 - Create a conda environment and activate it:** ```bash conda
-create --name opticallyshallowdeep python=3.10 conda activate
-opticallyshallowdeep ``` **2 - Install tensorflow** For mac OS: ```bash conda
-install -c apple tensorflow-deps python -m pip install tensorflow-macos ``` For
-windows: ```bash pip3 install tensorflow==2.13.0 ``` In case of compatibility
-issues, please try the newest version of tensorflow: ```bash pip3 install --
-upgrade --force-reinstall tensorflow ``` For Linux and more on installing
-tensorflow: [https://www.tensorflow.org/install](https://www.tensorflow.org/
-install) **3 - Install opticallyshallowdeep:** ```bash pip3 install
-opticallyshallowdeep ``` ## Quick Start For L1C files: ```python import
-opticallyshallowdeep as osd # Input file file_L1C = 'folder/S2.SAFE' # Output
-folder folder_out = 'folder/test_folder_out' # Run the OSW/ODW classifier
-osd.run(file_L1C, folder_out) ``` For ACOLITE L2R files: ```python import
-opticallyshallowdeep as osd # Input files file_L1C = 'test_folder_in/S2.SAFE'
-file_L2R = 'test_folder_in/L2R.nc' # Output folder folder_out = 'folder/
-test_folder_out' # Run the OSW/ODW classifier osd.run(file_in, folder_out,
-file_L2R=file_L2R) ``` The L1C file is always required as it contains a cloud
-mask. Pixels within 8 pixels of the cloud mask are masked to reduce the impact
-of clouds. Output is a 1-band geotiff, with values of prediction probability of
-OSW (100 means most likely OSW, 0 means most likely ODW). Non-water pixels are
-masked. It is recommended to use pixels between 0 and 40 as ODW, and pixels
-between 60 and 100 as OSW (publication in review). A log file, an intermediate
-multi-band geotiff, and a preview PNG are also generated in the output folder.
-They can be deleted after the processing. ## Training, test, and validation
-data All annotated shapefiles used in training, testing, and validating the DNN
-model are in the annotated_shapefiles folder, grouped by Sentinel-2 Scene ID.
+Metadata-Version: 2.1 Name: opticallyshallowdeep Version: 1.2.1 Summary:
+Identify optically shallow and deep waters in satellite imagery Author: Yulun
+Wu Author-email: yulunwu8@gmail.com Classifier: Programming Language :: Python
+:: 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: geopandas Requires-Dist: rasterio Requires-Dist:
+tifffile Requires-Dist: netCDF4 Requires-Dist: pyproj Requires-Dist: joblib
+Requires-Dist: scipy Requires-Dist: matplotlib Requires-Dist: imagecodecs
+Requires-Dist: tensorflow # Optically-Shallow-Deep This python tool delineates
+optically shallow and deep waters in Sentinel-2 imagery. The tool uses a deep
+neural network (DNN) that was trained on a diverse set of global images.
+Supported input includes Level-1C (L1C) SAFE files and ACOLITE-processed L2R
+netCDF files. The output geotiff contains probabilities of water pixels being
+optically shallow and deep. Originally coded by by Galen Richardson and Anders
+Knudby, modified and packaged by Yulun Wu Home page: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
+_y_u_l_u_n_w_u_8_/_O_p_t_i_c_a_l_l_y_-_S_h_a_l_l_o_w_-_D_e_e_p ## Installation **1 - Create a conda
+environment and activate it:** ```bash conda create --name opticallyshallowdeep
+python=3.10 conda activate opticallyshallowdeep ``` **2 - Install tensorflow**
+For mac OS: ```bash conda install -c apple tensorflow-deps python -m pip
+install tensorflow-macos ``` For windows: ```bash pip3 install
+tensorflow==2.13.0 ``` For Linux and more on installing tensorflow: [https://
+www.tensorflow.org/install](https://www.tensorflow.org/install) **3 - Install
+opticallyshallowdeep:** ```bash pip3 install opticallyshallowdeep ``` ## Quick
+Start For L1C files: ```python import opticallyshallowdeep as osd # Input file
+file_L1C = 'folder/S2.SAFE' # Output folder folder_out = 'folder/
+test_folder_out' # Run the OSW/ODW classifier osd.run(file_L1C, folder_out) ```
+For ACOLITE L2R files: ```python import opticallyshallowdeep as osd # Input
+files file_L1C = 'test_folder_in/S2.SAFE' file_L2R = 'test_folder_in/L2R.nc' #
+Output folder folder_out = 'folder/test_folder_out' # Run the OSW/ODW
+classifier osd.run(file_L1C, folder_out, file_L2R=file_L2R) ``` The L1C file is
+always required as it contains a built-in cloud mask. Pixels within 8 pixels of
+the cloud mask are masked to reduce the impact of clouds. Output is a 1-band
+geotiff, with values of prediction probability of optically shallow water
+(OSW): 100 means most likely OSW, 0 means most likely optically deep water
+(ODW). Non-water pixels are masked. It is recommended to treat pixels between 0
+and 40 as ODW, and pixels between 60 and 100 as OSW (publication in review). A
+log file, an intermediate multi-band geotiff, and a preview PNG are also
+generated in the output folder. They can be deleted after the processing.
+**Sample Sentinel-2 scene and output:** [images/TOA.jpeg][images/OSW.jpeg]##
+Training, test, and validation data All annotated shapefiles used in training,
+testing, and validating the DNN model are in the annotated_shapefiles folder,
+grouped by Sentinel-2 Scene ID.
```

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/cloud_mask.py` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/cloud_mask.py`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/find_epsg.py` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/find_epsg.py`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/make_multiband_image.py` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/make_multiband_image.py`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/make_vertical_strips.py` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/make_vertical_strips.py`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/models/SR.h5` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/models/SR.h5`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/models/TOA.h5` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/models/TOA.h5`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/netcdf_to_multiband_geotiff.py` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/netcdf_to_multiband_geotiff.py`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/parse_string.py` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/parse_string.py`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/process_as_strips.py` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/process_as_strips.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,21 +175,23 @@
 def process_image_with_filters(img, selected_columns):
     height, width, bands = img.shape#the output of this is an image of the filters required for this model
     filter_list = [value for value in selected_columns if value not in [["lat"], ["long"], ["lat_abs"]]]
     output_bands = []
     for band, kernel_size, filter_type in filter_list:
         
         if filter_type is None:
-            filtered_band = img[:, :, band].astype(np.uint16)#this means it is a single pixel
+            filtered_band = img[:, :, band]
         else:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", category=RuntimeWarning)
                 filtered_band = apply_filter(img[:, :, band].astype(np.float32), kernel_size, filter_type)
                 filtered_band[filtered_band==-32768] = 32768
-                filtered_band = filtered_band.astype(np.uint16)
+            
+        filtered_band[filtered_band<0] = 0
+        filtered_band = filtered_band.astype(np.uint16)#this means it is a single pixel
             
         output_bands.append(filtered_band)#append to list of filters
         del filtered_band
         gc.collect()
     del img
     output_image = np.stack(output_bands, axis=-1)# Stack along the last dimension to make filter image
     del output_bands
```

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/run.py` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,19 @@
         os.makedirs(folder_out)
     
     ### Print all metadata/settings and save them in a txt file
     if to_log: 
         # Start logging in txt file
         orig_stdout = sys.stdout
         
-        log_base = os.path.basename(file_L1C).replace('.safe','.txt').replace('.SAFE','.txt')
+        if file_L2R is None: 
+            log_base = os.path.basename(file_L1C).replace('.safe','.txt').replace('.SAFE','.txt')
+        else:
+            log_base = os.path.basename(file_L2R).replace('.nc','.txt')
+        
         log_base = 'OSD_log_'+ log_base
         log_file = os.path.join(folder_out,log_base)
 
         class Logger:
             def __init__(self, filename):
                 self.console = sys.stdout
                 self.file = open(filename, 'w')
```

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep/write_georef_image.py` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep/write_georef_image.py`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep.egg-info/PKG-INFO` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticallyshallowdeep
-Version: 1.2.0
+Version: 1.2.1
 Summary: Identify optically shallow and deep waters in satellite imagery
 Author: Yulun Wu
 Author-email: yulunwu8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,15 +19,15 @@
 Requires-Dist: imagecodecs
 Requires-Dist: tensorflow
 
 # Optically-Shallow-Deep 
 
 This python tool delineates optically shallow and deep waters in Sentinel-2 imagery. The tool uses a deep neural network (DNN) that was trained on a diverse set of global images.
 
-Supported input includes L1C SAFE files and ACOLITE-processed L2R netCDF files. The output geotiff contains probabilities of water pixels being optically shallow and deep. 
+Supported input includes Level-1C (L1C) SAFE files and ACOLITE-processed L2R netCDF files. The output geotiff contains probabilities of water pixels being optically shallow and deep. 
 
 Originally coded by by Galen Richardson and Anders Knudby, modified and packaged by Yulun Wu
 
 Home page: <a href="https://github.com/yulunwu8/Optically-Shallow-Deep" target="_blank">https://github.com/yulunwu8/Optically-Shallow-Deep</a>
 
 
  
@@ -43,30 +43,21 @@
 **2 - Install tensorflow**
 
 For mac OS: 
 
 ```bash
 conda install -c apple tensorflow-deps
 python -m pip install tensorflow-macos
-
 ```
 
 
 For windows:
 
 ```bash
 pip3 install tensorflow==2.13.0
-
-```
-
-In case of compatibility issues, please try the newest version of tensorflow: 
-
-```bash
-pip3 install --upgrade --force-reinstall tensorflow
-
 ```
 
 
 For Linux and more on installing tensorflow: [https://www.tensorflow.org/install](https://www.tensorflow.org/install)
 
 
 **3 - Install opticallyshallowdeep:**
@@ -102,24 +93,31 @@
 file_L1C = 'test_folder_in/S2.SAFE' 
 file_L2R = 'test_folder_in/L2R.nc' 
 
 # Output folder 
 folder_out = 'folder/test_folder_out'
 
 # Run the OSW/ODW classifier 
-osd.run(file_in, folder_out, file_L2R=file_L2R)
+osd.run(file_L1C, folder_out, file_L2R=file_L2R)
 ```
 
-The L1C file is always required as it contains a cloud mask. Pixels within 8 pixels of the cloud mask are masked to reduce the impact of clouds. 
+The L1C file is always required as it contains a built-in cloud mask. Pixels within 8 pixels of the cloud mask are masked to reduce the impact of clouds. 
 
 
-Output is a 1-band geotiff, with values of prediction probability of OSW (100 means most likely OSW, 0 means most likely ODW). Non-water pixels are masked. It is recommended to use pixels between 0 and 40 as ODW, and pixels between 60 and 100 as OSW (publication in review).
+Output is a 1-band geotiff, with values of prediction probability of optically shallow water (OSW): 100 means most likely OSW, 0 means most likely optically deep water (ODW). Non-water pixels are masked. It is recommended to treat pixels between 0 and 40 as ODW, and pixels between 60 and 100 as OSW (publication in review).
 
 A log file, an intermediate multi-band geotiff, and a preview PNG are also generated in the output folder. They can be deleted after the processing. 
 
+
+**Sample Sentinel-2 scene and output:**
+
+<img src="images/TOA.jpeg"  height="500">
+
+<img src="images/OSW.jpeg"  height="500">
+
 ## Training, test, and validation data 
 
 All annotated shapefiles used in training, testing, and validating the DNN model are in the annotated_shapefiles folder, grouped by Sentinel-2 Scene ID.
```

#### html2text {}

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.1 Name: opticallyshallowdeep Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: opticallyshallowdeep Version: 1.2.1 Summary:
 Identify optically shallow and deep waters in satellite imagery Author: Yulun
 Wu Author-email: yulunwu8@gmail.com Classifier: Programming Language :: Python
 :: 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: geopandas Requires-Dist: rasterio Requires-Dist:
 tifffile Requires-Dist: netCDF4 Requires-Dist: pyproj Requires-Dist: joblib
 Requires-Dist: scipy Requires-Dist: matplotlib Requires-Dist: imagecodecs
 Requires-Dist: tensorflow # Optically-Shallow-Deep This python tool delineates
 optically shallow and deep waters in Sentinel-2 imagery. The tool uses a deep
 neural network (DNN) that was trained on a diverse set of global images.
-Supported input includes L1C SAFE files and ACOLITE-processed L2R netCDF files.
-The output geotiff contains probabilities of water pixels being optically
-shallow and deep. Originally coded by by Galen Richardson and Anders Knudby,
-modified and packaged by Yulun Wu Home page: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_y_u_l_u_n_w_u_8_/
-_O_p_t_i_c_a_l_l_y_-_S_h_a_l_l_o_w_-_D_e_e_p ## Installation **1 - Create a conda environment and
-activate it:** ```bash conda create --name opticallyshallowdeep python=3.10
-conda activate opticallyshallowdeep ``` **2 - Install tensorflow** For mac OS:
-```bash conda install -c apple tensorflow-deps python -m pip install
-tensorflow-macos ``` For windows: ```bash pip3 install tensorflow==2.13.0 ```
-In case of compatibility issues, please try the newest version of tensorflow:
-```bash pip3 install --upgrade --force-reinstall tensorflow ``` For Linux and
-more on installing tensorflow: [https://www.tensorflow.org/install](https://
-www.tensorflow.org/install) **3 - Install opticallyshallowdeep:** ```bash pip3
-install opticallyshallowdeep ``` ## Quick Start For L1C files: ```python import
-opticallyshallowdeep as osd # Input file file_L1C = 'folder/S2.SAFE' # Output
-folder folder_out = 'folder/test_folder_out' # Run the OSW/ODW classifier
-osd.run(file_L1C, folder_out) ``` For ACOLITE L2R files: ```python import
-opticallyshallowdeep as osd # Input files file_L1C = 'test_folder_in/S2.SAFE'
-file_L2R = 'test_folder_in/L2R.nc' # Output folder folder_out = 'folder/
-test_folder_out' # Run the OSW/ODW classifier osd.run(file_in, folder_out,
-file_L2R=file_L2R) ``` The L1C file is always required as it contains a cloud
-mask. Pixels within 8 pixels of the cloud mask are masked to reduce the impact
-of clouds. Output is a 1-band geotiff, with values of prediction probability of
-OSW (100 means most likely OSW, 0 means most likely ODW). Non-water pixels are
-masked. It is recommended to use pixels between 0 and 40 as ODW, and pixels
-between 60 and 100 as OSW (publication in review). A log file, an intermediate
-multi-band geotiff, and a preview PNG are also generated in the output folder.
-They can be deleted after the processing. ## Training, test, and validation
-data All annotated shapefiles used in training, testing, and validating the DNN
-model are in the annotated_shapefiles folder, grouped by Sentinel-2 Scene ID.
+Supported input includes Level-1C (L1C) SAFE files and ACOLITE-processed L2R
+netCDF files. The output geotiff contains probabilities of water pixels being
+optically shallow and deep. Originally coded by by Galen Richardson and Anders
+Knudby, modified and packaged by Yulun Wu Home page: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
+_y_u_l_u_n_w_u_8_/_O_p_t_i_c_a_l_l_y_-_S_h_a_l_l_o_w_-_D_e_e_p ## Installation **1 - Create a conda
+environment and activate it:** ```bash conda create --name opticallyshallowdeep
+python=3.10 conda activate opticallyshallowdeep ``` **2 - Install tensorflow**
+For mac OS: ```bash conda install -c apple tensorflow-deps python -m pip
+install tensorflow-macos ``` For windows: ```bash pip3 install
+tensorflow==2.13.0 ``` For Linux and more on installing tensorflow: [https://
+www.tensorflow.org/install](https://www.tensorflow.org/install) **3 - Install
+opticallyshallowdeep:** ```bash pip3 install opticallyshallowdeep ``` ## Quick
+Start For L1C files: ```python import opticallyshallowdeep as osd # Input file
+file_L1C = 'folder/S2.SAFE' # Output folder folder_out = 'folder/
+test_folder_out' # Run the OSW/ODW classifier osd.run(file_L1C, folder_out) ```
+For ACOLITE L2R files: ```python import opticallyshallowdeep as osd # Input
+files file_L1C = 'test_folder_in/S2.SAFE' file_L2R = 'test_folder_in/L2R.nc' #
+Output folder folder_out = 'folder/test_folder_out' # Run the OSW/ODW
+classifier osd.run(file_L1C, folder_out, file_L2R=file_L2R) ``` The L1C file is
+always required as it contains a built-in cloud mask. Pixels within 8 pixels of
+the cloud mask are masked to reduce the impact of clouds. Output is a 1-band
+geotiff, with values of prediction probability of optically shallow water
+(OSW): 100 means most likely OSW, 0 means most likely optically deep water
+(ODW). Non-water pixels are masked. It is recommended to treat pixels between 0
+and 40 as ODW, and pixels between 60 and 100 as OSW (publication in review). A
+log file, an intermediate multi-band geotiff, and a preview PNG are also
+generated in the output folder. They can be deleted after the processing.
+**Sample Sentinel-2 scene and output:** [images/TOA.jpeg][images/OSW.jpeg]##
+Training, test, and validation data All annotated shapefiles used in training,
+testing, and validating the DNN model are in the annotated_shapefiles folder,
+grouped by Sentinel-2 Scene ID.
```

### Comparing `opticallyshallowdeep-1.2.0/opticallyshallowdeep.egg-info/SOURCES.txt` & `opticallyshallowdeep-1.2.1/opticallyshallowdeep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opticallyshallowdeep-1.2.0/setup.py` & `opticallyshallowdeep-1.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='opticallyshallowdeep',
-    version='1.2.0',
+    version='1.2.1',
     author='Yulun Wu',
     author_email='yulunwu8@gmail.com',
     description='Identify optically shallow and deep waters in satellite imagery',
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     # packages=find_packages(),
     packages=['opticallyshallowdeep','opticallyshallowdeep.models'],
```

