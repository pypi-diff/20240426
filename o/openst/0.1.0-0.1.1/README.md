# Comparing `tmp/openst-0.1.0.tar.gz` & `tmp/openst-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openst-0.1.0.tar", max compression
+gzip compressed data, was "openst-0.1.1.tar", max compression
```

## Comparing `openst-0.1.0.tar` & `openst-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0      896 2024-04-18 14:20:31.331344 openst-0.1.0/LICENSE
--rw-r--r--   0        0        0     4265 2024-04-25 15:58:08.164649 openst-0.1.0/README.md
--rw-r--r--   0        0        0       22 2024-04-25 15:58:08.252649 openst-0.1.0/openst/__init__.py
--rw-r--r--   0        0        0      358 2024-04-25 16:16:49.572600 openst-0.1.0/openst/__main__.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.611322 openst-0.1.0/openst/alignment/__init__.py
--rw-r--r--   0        0        0     5878 2024-04-18 13:23:51.785039 openst-0.1.0/openst/alignment/apply_transform.py
--rw-r--r--   0        0        0    12248 2024-04-25 16:16:49.576600 openst-0.1.0/openst/alignment/feature_matching.py
--rw-r--r--   0        0        0     3628 2024-02-14 16:40:22.623322 openst-0.1.0/openst/alignment/fiducial_detection.py
--rw-r--r--   0        0        0    50862 2024-04-25 16:16:49.580600 openst-0.1.0/openst/alignment/manual_pairwise_aligner.py
--rw-r--r--   0        0        0    23898 2024-04-25 16:16:49.580600 openst-0.1.0/openst/alignment/pairwise_aligner.py
--rw-r--r--   0        0        0     5505 2024-04-25 15:58:08.256649 openst-0.1.0/openst/alignment/transcript_assign.py
--rw-r--r--   0        0        0      798 2024-04-18 13:23:51.825039 openst-0.1.0/openst/alignment/transformation.py
--rw-r--r--   0        0        0    47711 2024-04-25 16:16:49.584600 openst-0.1.0/openst/cli.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.655321 openst-0.1.0/openst/metadata/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.659321 openst-0.1.0/openst/metadata/classes/__init__.py
--rw-r--r--   0        0        0     2899 2024-04-25 16:16:49.588600 openst-0.1.0/openst/metadata/classes/base.py
--rw-r--r--   0        0        0     3539 2024-04-25 16:16:49.592600 openst-0.1.0/openst/metadata/classes/pairwise_alignment.py
--rw-r--r--   0        0        0     1798 2024-02-14 16:40:22.679321 openst-0.1.0/openst/metadata/classes/segmentation.py
--rw-r--r--   0        0        0     3787 2024-02-14 16:40:22.683321 openst-0.1.0/openst/metadata/example_json.json
--rw-r--r--   0        0        0     1450 2024-04-18 13:23:51.849039 openst-0.1.0/openst/metadata/report.py
--rw-r--r--   0        0        0  1187390 2024-02-14 16:40:22.715321 openst-0.1.0/openst/metadata/templates/pairwise_alignment.html
--rw-r--r--   0        0        0     1745 2024-02-14 16:40:22.723321 openst-0.1.0/openst/preprocessing/CUT/README.md
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.723321 openst-0.1.0/openst/preprocessing/CUT/__init__.py
--rw-r--r--   0        0        0     3157 2024-04-25 15:58:08.256649 openst-0.1.0/openst/preprocessing/CUT/models/__init__.py
--rw-r--r--   0        0        0    11347 2024-04-25 15:58:08.256649 openst-0.1.0/openst/preprocessing/CUT/models/base_model.py
--rw-r--r--   0        0        0    10006 2024-04-25 15:58:08.256649 openst-0.1.0/openst/preprocessing/CUT/models/cut_model.py
--rw-r--r--   0        0        0    59845 2024-04-25 15:58:08.260649 openst-0.1.0/openst/preprocessing/CUT/models/networks.py
--rw-r--r--   0        0        0     2317 2024-04-25 15:58:08.260649 openst-0.1.0/openst/preprocessing/CUT/models/patchnce.py
--rw-r--r--   0        0        0     6013 2024-04-25 15:58:08.260649 openst-0.1.0/openst/preprocessing/CUT/models/template_model.py
--rw-r--r--   0        0        0      136 2024-02-14 16:40:22.755321 openst-0.1.0/openst/preprocessing/CUT/options/__init__.py
--rw-r--r--   0        0        0     8760 2024-04-25 15:58:08.260649 openst-0.1.0/openst/preprocessing/CUT/options/base_options.py
--rw-r--r--   0        0        0     1006 2024-04-25 15:58:08.260649 openst-0.1.0/openst/preprocessing/CUT/options/test_options.py
--rw-r--r--   0        0        0      132 2024-04-25 15:58:08.264649 openst-0.1.0/openst/preprocessing/CUT/util/__init__.py
--rw-r--r--   0        0        0     5135 2024-02-14 16:40:22.783321 openst-0.1.0/openst/preprocessing/CUT/util/util.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.787321 openst-0.1.0/openst/preprocessing/__init__.py
--rw-r--r--   0        0        0     4102 2024-04-25 16:16:49.596600 openst-0.1.0/openst/preprocessing/barcode_preprocessing.py
--rw-r--r--   0        0        0     7323 2024-04-25 15:58:08.264649 openst-0.1.0/openst/preprocessing/image_preprocess.py
--rw-r--r--   0        0        0     4607 2024-04-18 13:23:51.877039 openst-0.1.0/openst/preprocessing/image_stitch.py
--rw-r--r--   0        0        0      690 2024-02-14 16:40:22.811321 openst-0.1.0/openst/preprocessing/imagej_macros/keyence_stitch.ijm
--rw-r--r--   0        0        0      833 2024-04-18 13:23:51.885039 openst-0.1.0/openst/preprocessing/merge_modalities.py
--rw-r--r--   0        0        0     8996 2024-04-18 13:23:51.893039 openst-0.1.0/openst/preprocessing/spatial_stitch.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.819321 openst-0.1.0/openst/segmentation/__init__.py
--rw-r--r--   0        0        0    14694 2024-04-25 15:58:08.264649 openst-0.1.0/openst/segmentation/segment.py
--rw-r--r--   0        0        0     3842 2024-04-18 13:23:51.913039 openst-0.1.0/openst/segmentation/segment_merge.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.827321 openst-0.1.0/openst/threed/__init__.py
--rw-r--r--   0        0        0     9811 2024-04-18 13:23:51.925039 openst-0.1.0/openst/threed/from_3d_registration.py
--rw-r--r--   0        0        0     2500 2024-04-18 13:23:51.933039 openst-0.1.0/openst/threed/to_3d_registration.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.843321 openst-0.1.0/openst/utils/__init__.py
--rw-r--r--   0        0        0     9843 2024-04-25 16:16:49.596600 openst-0.1.0/openst/utils/file.py
--rw-r--r--   0        0        0    13953 2024-04-18 13:23:51.953039 openst-0.1.0/openst/utils/from_spacemake.py
--rw-r--r--   0        0        0     9680 2024-04-25 16:16:49.600600 openst-0.1.0/openst/utils/pimage.py
--rw-r--r--   0        0        0     3018 2024-02-14 16:40:22.859321 openst-0.1.0/openst/utils/points.py
--rw-r--r--   0        0        0     2419 2024-04-18 13:23:51.969039 openst-0.1.0/openst/utils/preview.py
--rw-r--r--   0        0        0    10060 2024-04-25 16:16:49.604600 openst-0.1.0/openst/utils/pseudoimage.py
--rw-r--r--   0        0        0        0 2024-02-14 16:40:22.867321 openst-0.1.0/openst/utils/scanpy/__init__.py
--rw-r--r--   0        0        0       37 2024-02-14 16:40:22.875321 openst-0.1.0/openst/utils/scanpy/pp/__init__.py
--rw-r--r--   0        0        0    10779 2024-02-14 16:40:22.879321 openst-0.1.0/openst/utils/scanpy/pp/_qc.py
--rw-r--r--   0        0        0     3737 2024-04-18 13:23:51.997039 openst-0.1.0/openst/utils/spacemake.py
--rw-r--r--   0        0        0     1991 2024-04-25 16:16:49.608600 openst-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 openst-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      896 2024-04-18 14:20:31.331344 openst-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4265 2024-04-25 15:58:08.164649 openst-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-25 15:58:08.252649 openst-0.1.1/openst/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-25 16:16:49.572600 openst-0.1.1/openst/__main__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.611322 openst-0.1.1/openst/alignment/__init__.py
+-rw-r--r--   0        0        0     5878 2024-04-26 07:55:53.608030 openst-0.1.1/openst/alignment/apply_transform.py
+-rw-r--r--   0        0        0    12248 2024-04-25 16:16:49.576600 openst-0.1.1/openst/alignment/feature_matching.py
+-rw-r--r--   0        0        0     3628 2024-02-14 16:40:22.623322 openst-0.1.1/openst/alignment/fiducial_detection.py
+-rw-r--r--   0        0        0    51422 2024-04-26 18:04:33.636901 openst-0.1.1/openst/alignment/manual_pairwise_aligner.py
+-rw-r--r--   0        0        0    23898 2024-04-25 16:16:49.580600 openst-0.1.1/openst/alignment/pairwise_aligner.py
+-rw-r--r--   0        0        0     6620 2024-04-26 07:18:57.894428 openst-0.1.1/openst/alignment/transcript_assign.py
+-rw-r--r--   0        0        0      798 2024-04-18 13:23:51.825039 openst-0.1.1/openst/alignment/transformation.py
+-rw-r--r--   0        0        0    47711 2024-04-25 16:16:49.584600 openst-0.1.1/openst/cli.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.655321 openst-0.1.1/openst/metadata/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.659321 openst-0.1.1/openst/metadata/classes/__init__.py
+-rw-r--r--   0        0        0     2899 2024-04-25 16:16:49.588600 openst-0.1.1/openst/metadata/classes/base.py
+-rw-r--r--   0        0        0     3539 2024-04-25 16:16:49.592600 openst-0.1.1/openst/metadata/classes/pairwise_alignment.py
+-rw-r--r--   0        0        0     1798 2024-02-14 16:40:22.679321 openst-0.1.1/openst/metadata/classes/segmentation.py
+-rw-r--r--   0        0        0     3787 2024-02-14 16:40:22.683321 openst-0.1.1/openst/metadata/example_json.json
+-rw-r--r--   0        0        0     1450 2024-04-18 13:23:51.849039 openst-0.1.1/openst/metadata/report.py
+-rw-r--r--   0        0        0  1187390 2024-02-14 16:40:22.715321 openst-0.1.1/openst/metadata/templates/pairwise_alignment.html
+-rw-r--r--   0        0        0     1745 2024-02-14 16:40:22.723321 openst-0.1.1/openst/preprocessing/CUT/README.md
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.723321 openst-0.1.1/openst/preprocessing/CUT/__init__.py
+-rw-r--r--   0        0        0     3157 2024-04-25 15:58:08.256649 openst-0.1.1/openst/preprocessing/CUT/models/__init__.py
+-rw-r--r--   0        0        0    11347 2024-04-25 15:58:08.256649 openst-0.1.1/openst/preprocessing/CUT/models/base_model.py
+-rw-r--r--   0        0        0    10006 2024-04-25 15:58:08.256649 openst-0.1.1/openst/preprocessing/CUT/models/cut_model.py
+-rw-r--r--   0        0        0    59845 2024-04-25 15:58:08.260649 openst-0.1.1/openst/preprocessing/CUT/models/networks.py
+-rw-r--r--   0        0        0     2317 2024-04-25 15:58:08.260649 openst-0.1.1/openst/preprocessing/CUT/models/patchnce.py
+-rw-r--r--   0        0        0     6013 2024-04-25 15:58:08.260649 openst-0.1.1/openst/preprocessing/CUT/models/template_model.py
+-rw-r--r--   0        0        0      136 2024-02-14 16:40:22.755321 openst-0.1.1/openst/preprocessing/CUT/options/__init__.py
+-rw-r--r--   0        0        0     8760 2024-04-25 15:58:08.260649 openst-0.1.1/openst/preprocessing/CUT/options/base_options.py
+-rw-r--r--   0        0        0     1006 2024-04-25 15:58:08.260649 openst-0.1.1/openst/preprocessing/CUT/options/test_options.py
+-rw-r--r--   0        0        0      132 2024-04-25 15:58:08.264649 openst-0.1.1/openst/preprocessing/CUT/util/__init__.py
+-rw-r--r--   0        0        0     5135 2024-02-14 16:40:22.783321 openst-0.1.1/openst/preprocessing/CUT/util/util.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.787321 openst-0.1.1/openst/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4102 2024-04-25 16:16:49.596600 openst-0.1.1/openst/preprocessing/barcode_preprocessing.py
+-rw-r--r--   0        0        0     7323 2024-04-25 15:58:08.264649 openst-0.1.1/openst/preprocessing/image_preprocess.py
+-rw-r--r--   0        0        0     4607 2024-04-18 13:23:51.877039 openst-0.1.1/openst/preprocessing/image_stitch.py
+-rw-r--r--   0        0        0      690 2024-02-14 16:40:22.811321 openst-0.1.1/openst/preprocessing/imagej_macros/keyence_stitch.ijm
+-rw-r--r--   0        0        0      833 2024-04-18 13:23:51.885039 openst-0.1.1/openst/preprocessing/merge_modalities.py
+-rw-r--r--   0        0        0     8996 2024-04-18 13:23:51.893039 openst-0.1.1/openst/preprocessing/spatial_stitch.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.819321 openst-0.1.1/openst/segmentation/__init__.py
+-rw-r--r--   0        0        0    14694 2024-04-25 15:58:08.264649 openst-0.1.1/openst/segmentation/segment.py
+-rw-r--r--   0        0        0     3842 2024-04-18 13:23:51.913039 openst-0.1.1/openst/segmentation/segment_merge.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.827321 openst-0.1.1/openst/threed/__init__.py
+-rw-r--r--   0        0        0     9811 2024-04-18 13:23:51.925039 openst-0.1.1/openst/threed/from_3d_registration.py
+-rw-r--r--   0        0        0     2500 2024-04-18 13:23:51.933039 openst-0.1.1/openst/threed/to_3d_registration.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.843321 openst-0.1.1/openst/utils/__init__.py
+-rw-r--r--   0        0        0     9843 2024-04-25 16:16:49.596600 openst-0.1.1/openst/utils/file.py
+-rw-r--r--   0        0        0    13953 2024-04-18 13:23:51.953039 openst-0.1.1/openst/utils/from_spacemake.py
+-rw-r--r--   0        0        0     3401 2024-04-26 07:21:44.301924 openst-0.1.1/openst/utils/molecular_dynamics.py
+-rw-r--r--   0        0        0     9680 2024-04-25 16:16:49.600600 openst-0.1.1/openst/utils/pimage.py
+-rw-r--r--   0        0        0     3018 2024-02-14 16:40:22.859321 openst-0.1.1/openst/utils/points.py
+-rw-r--r--   0        0        0     2419 2024-04-18 13:23:51.969039 openst-0.1.1/openst/utils/preview.py
+-rw-r--r--   0        0        0    10060 2024-04-25 16:16:49.604600 openst-0.1.1/openst/utils/pseudoimage.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:40:22.867321 openst-0.1.1/openst/utils/scanpy/__init__.py
+-rw-r--r--   0        0        0       37 2024-02-14 16:40:22.875321 openst-0.1.1/openst/utils/scanpy/pp/__init__.py
+-rw-r--r--   0        0        0    10779 2024-02-14 16:40:22.879321 openst-0.1.1/openst/utils/scanpy/pp/_qc.py
+-rw-r--r--   0        0        0     3737 2024-04-18 13:23:51.997039 openst-0.1.1/openst/utils/spacemake.py
+-rw-r--r--   0        0        0     1991 2024-04-26 18:04:33.640901 openst-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 openst-0.1.1/PKG-INFO
```

### Comparing `openst-0.1.0/LICENSE` & `openst-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/README.md` & `openst-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/alignment/apply_transform.py` & `openst-0.1.1/openst/alignment/apply_transform.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/alignment/feature_matching.py` & `openst-0.1.1/openst/alignment/feature_matching.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/alignment/fiducial_detection.py` & `openst-0.1.1/openst/alignment/fiducial_detection.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/alignment/manual_pairwise_aligner.py` & `openst-0.1.1/openst/alignment/manual_pairwise_aligner.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,15 +313,23 @@
         _i_counts_above_threshold = total_counts > self.threshold_counts
         sts_coords = sts_coords[_i_counts_above_threshold]
         tile_id = tile_id[_i_counts_above_threshold]
 
         # We keep the limits also when filtering by UMI (avoid issues with offsets)
         sts_coords = np.concatenate([sts_coords, np.array([[x_all_max, y_all_max],
                                                         [x_all_min, y_all_min]])])
-        tile_id = np.concatenate([tile_id, [-1, -1]])
+        
+        if not self.recenter_coarse:
+            min_lim, max_lim = [0, 0], staining_image.shape[:2][::-1]
+            x_all_min, y_all_min = min_lim
+            x_all_max, y_all_max = max_lim
+            sts_coords = np.concatenate([sts_coords, np.array([[x_all_max, y_all_max],
+                                                        [x_all_min, y_all_min]])])
+    
+        tile_id = np.concatenate([tile_id, [-1, -1, -2, -2]])
 
         # TODO: instead of this, we plot specific sections...
         if self.layer == "all_tiles_coarse":
             staining_image_rescaled = staining_image[:: self.rescale_factor_coarse, :: self.rescale_factor_coarse]
             sts_pseudoimage = create_paired_pseudoimage(
                 sts_coords[:, ::-1],
                 self.pseudoimg_size,
@@ -1106,14 +1114,17 @@
                     {
                         "layer": k,
                         "point_src": [f"{(xA+xA_0+radius_A):.2f}", f"{(yA+yA_0+radius_A):.2f}"],
                         "point_dst": [f"{(xB+xB_0+radius_B):.2f}", f"{(yB+yB_0+radius_B):.2f}"],
                         "lims": _lims,
                         "factor_rescale": _rescale,
                         "offset_factor": _ofs_factor,
+                        "rescaling_factor": v['rescaling_factor'],
+                        "scale": v['scale'],
+                        "rescale_factor": v['rescale_factor'],
                         "point_src_offset_rescaled": [
                             f"{((((xA+xA_0+radius_A)+_lims[0])*_rescale)):.2f}",
                             f"{((((yA+yA_0+radius_A)+_lims[2])*_rescale)):.2f}",
                         ],
                         "point_dst_offset_rescaled": [
                             # f"{((((xB+xB_0)+_lims[0])*_rescale*_scale)+_ofs_factor[1]):.2f}",
                             # f"{((((yB+yB_0)+_lims[2])*_rescale*_scale)+_ofs_factor[0]):.2f}",
```

### Comparing `openst-0.1.0/openst/alignment/pairwise_aligner.py` & `openst-0.1.1/openst/alignment/pairwise_aligner.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/alignment/transcript_assign.py` & `openst-0.1.1/openst/alignment/transcript_assign.py`

 * *Files 14% similar despite different names*

```diff
@@ -83,14 +83,38 @@
         adata_shuffled.obs[col] = 1
 
     adata_shuffled.var_names = adata.var_names
 
     return adata_shuffled
 
 
+def diffuse_umi(adata, spatial_key='spatial'):
+    from scipy.sparse import csr_array, csc_matrix
+    import anndata as ad
+
+    X_0_repeat = np.repeat(adata.X.nonzero()[0], adata.X.data.astype(int))
+    X_1_repeat = np.repeat(adata.X.nonzero()[1], adata.X.data.astype(int))
+    tile_id = np.repeat(adata.obs['tile_id'].astype(str).values, np.array(adata.X.sum(axis=1)).flatten().astype(int))
+    idx_range = np.arange(len(X_0_repeat))
+    loc_random = np.random.randint(0, len(adata.obsm[spatial_key]), len(X_1_repeat))
+    # obsm_spatial_expanded = tiles_transformed_coords_refined_concatenated[loc_random]
+    obsm_spatial_expanded = adata.obsm[spatial_key][loc_random]
+    X_repeat = csc_matrix(csr_array((np.ones_like(X_0_repeat), (idx_range, X_1_repeat))))
+    adata_shuffled = ad.AnnData(X=X_repeat)
+    adata_shuffled.obs_names = (pd.Series(idx_range.astype(str)) + ":" + pd.Series(tile_id)).values
+    adata_shuffled.obsm[spatial_key] = obsm_spatial_expanded
+
+    for col in adata.obs.columns:
+        adata_shuffled.obs[col] = 1
+
+    adata_shuffled.var_names = adata.var_names
+
+    return adata_shuffled
+
+
 def _run_transcript_assign(args):
     """_run_transcript_assign
     
     This one uses AnnData instead of h5py, so the obsm/ and uns/ keys must be parsed 
     """
     # TODO: load with dask if it is too large
```

### Comparing `openst-0.1.0/openst/alignment/transformation.py` & `openst-0.1.1/openst/alignment/transformation.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/cli.py` & `openst-0.1.1/openst/cli.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/metadata/classes/base.py` & `openst-0.1.1/openst/metadata/classes/base.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/metadata/classes/pairwise_alignment.py` & `openst-0.1.1/openst/metadata/classes/pairwise_alignment.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/metadata/classes/segmentation.py` & `openst-0.1.1/openst/metadata/classes/segmentation.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/metadata/example_json.json` & `openst-0.1.1/openst/metadata/example_json.json`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/metadata/report.py` & `openst-0.1.1/openst/metadata/report.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/metadata/templates/pairwise_alignment.html` & `openst-0.1.1/openst/metadata/templates/pairwise_alignment.html`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/CUT/README.md` & `openst-0.1.1/openst/preprocessing/CUT/README.md`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/CUT/models/__init__.py` & `openst-0.1.1/openst/preprocessing/CUT/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/CUT/models/base_model.py` & `openst-0.1.1/openst/preprocessing/CUT/models/base_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/CUT/models/cut_model.py` & `openst-0.1.1/openst/preprocessing/CUT/models/cut_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/CUT/models/networks.py` & `openst-0.1.1/openst/preprocessing/CUT/models/networks.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/CUT/models/patchnce.py` & `openst-0.1.1/openst/preprocessing/CUT/models/patchnce.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/CUT/models/template_model.py` & `openst-0.1.1/openst/preprocessing/CUT/models/template_model.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/CUT/options/base_options.py` & `openst-0.1.1/openst/preprocessing/CUT/options/base_options.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/CUT/options/test_options.py` & `openst-0.1.1/openst/preprocessing/CUT/options/test_options.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/CUT/util/util.py` & `openst-0.1.1/openst/preprocessing/CUT/util/util.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/barcode_preprocessing.py` & `openst-0.1.1/openst/preprocessing/barcode_preprocessing.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/image_preprocess.py` & `openst-0.1.1/openst/preprocessing/image_preprocess.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/image_stitch.py` & `openst-0.1.1/openst/preprocessing/image_stitch.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/imagej_macros/keyence_stitch.ijm` & `openst-0.1.1/openst/preprocessing/imagej_macros/keyence_stitch.ijm`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/merge_modalities.py` & `openst-0.1.1/openst/preprocessing/merge_modalities.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/preprocessing/spatial_stitch.py` & `openst-0.1.1/openst/preprocessing/spatial_stitch.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/segmentation/segment.py` & `openst-0.1.1/openst/segmentation/segment.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/segmentation/segment_merge.py` & `openst-0.1.1/openst/segmentation/segment_merge.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/threed/from_3d_registration.py` & `openst-0.1.1/openst/threed/from_3d_registration.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/threed/to_3d_registration.py` & `openst-0.1.1/openst/threed/to_3d_registration.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/utils/file.py` & `openst-0.1.1/openst/utils/file.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/utils/from_spacemake.py` & `openst-0.1.1/openst/utils/from_spacemake.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/utils/pimage.py` & `openst-0.1.1/openst/utils/pimage.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/utils/points.py` & `openst-0.1.1/openst/utils/points.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/utils/preview.py` & `openst-0.1.1/openst/utils/preview.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/utils/pseudoimage.py` & `openst-0.1.1/openst/utils/pseudoimage.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/utils/scanpy/pp/_qc.py` & `openst-0.1.1/openst/utils/scanpy/pp/_qc.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/openst/utils/spacemake.py` & `openst-0.1.1/openst/utils/spacemake.py`

 * *Files identical despite different names*

### Comparing `openst-0.1.0/pyproject.toml` & `openst-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openst"
-version = "0.1.0"
+version = "0.1.1"
 description = "The computational pipeline for the Open-ST method."
 license = "GPL-2.0"
 authors = [
     "Daniel León-Periñán <daniel.leonperinan@mdc-berlin.de>",
     "Nikolaos Karaiskos <nikolaos.karaiskos@mdc-berlin.de>",
 ]
 maintainers = [
```

### Comparing `openst-0.1.0/PKG-INFO` & `openst-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openst
-Version: 0.1.0
+Version: 0.1.1
 Summary: The computational pipeline for the Open-ST method.
 License: GPL-2.0
 Author: Daniel León-Periñán
 Author-email: daniel.leonperinan@mdc-berlin.de
 Maintainer: Daniel León-Periñán
 Maintainer-email: daniel.leonperinan@mdc-berlin.de
 Requires-Python: >3.8,<3.12
```

