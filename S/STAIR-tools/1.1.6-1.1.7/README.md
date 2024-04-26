# Comparing `tmp/STAIR-tools-1.1.6.tar.gz` & `tmp/STAIR-tools-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.1.6.tar", last modified: Thu Apr 25 03:13:49 2024, max compression
+gzip compressed data, was "STAIR-tools-1.1.7.tar", last modified: Fri Apr 26 05:50:41 2024, max compression
```

## Comparing `STAIR-tools-1.1.6.tar` & `STAIR-tools-1.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 03:13:49.307667 STAIR-tools-1.1.6/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-25 03:13:49.307490 STAIR-tools-1.1.6/PKG-INFO
--rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.1.6/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 03:13:49.303140 STAIR-tools-1.1.6/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1.6/STAIR/ABA_annotation.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 03:13:49.303425 STAIR-tools-1.1.6/STAIR/ABAanno/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.6/STAIR/ABAanno/__init__.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.6/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18516 2024-04-25 03:13:12.000000 STAIR-tools-1.1.6/STAIR/emb_alignment.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 03:13:49.305183 STAIR-tools-1.1.6/STAIR/embedding/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.1.6/STAIR/embedding/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3013 2023-12-23 11:23:11.000000 STAIR-tools-1.1.6/STAIR/embedding/dataset_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3889 2023-12-23 11:23:12.000000 STAIR-tools-1.1.6/STAIR/embedding/dataset_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.1.6/STAIR/embedding/loss.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.1.6/STAIR/embedding/module_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.1.6/STAIR/embedding/module_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.1.6/STAIR/embedding/module_hgat1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12324 2024-04-25 02:44:23.000000 STAIR-tools-1.1.6/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14202 2024-04-25 02:44:36.000000 STAIR-tools-1.1.6/STAIR/loc_prediction.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 03:13:49.306715 STAIR-tools-1.1.6/STAIR/location/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.6/STAIR/location/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.1.6/STAIR/location/align_fine.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.1.6/STAIR/location/align_init.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.1.6/STAIR/location/edge_detection.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.1.6/STAIR/location/edge_detection1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.1.6/STAIR/location/transformation.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1.6/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 03:13:49.307302 STAIR-tools-1.1.6/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-25 03:13:49.000000 STAIR-tools-1.1.6/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-04-25 03:13:49.000000 STAIR-tools-1.1.6/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-04-25 03:13:49.000000 STAIR-tools-1.1.6/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-04-25 03:13:49.000000 STAIR-tools-1.1.6/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-04-25 03:13:49.307715 STAIR-tools-1.1.6/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      317 2024-04-25 03:13:40.000000 STAIR-tools-1.1.6/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-26 05:50:41.900809 STAIR-tools-1.1.7/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-26 05:50:41.900599 STAIR-tools-1.1.7/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.1.7/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-26 05:50:41.895612 STAIR-tools-1.1.7/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1.7/STAIR/ABA_annotation.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-26 05:50:41.895854 STAIR-tools-1.1.7/STAIR/ABAanno/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.7/STAIR/ABAanno/__init__.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.7/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18516 2024-04-26 05:49:50.000000 STAIR-tools-1.1.7/STAIR/emb_alignment.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-26 05:50:41.897696 STAIR-tools-1.1.7/STAIR/embedding/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.1.7/STAIR/embedding/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3013 2023-12-23 11:23:11.000000 STAIR-tools-1.1.7/STAIR/embedding/dataset_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3891 2024-04-25 06:09:45.000000 STAIR-tools-1.1.7/STAIR/embedding/dataset_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.1.7/STAIR/embedding/loss.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.1.7/STAIR/embedding/module_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.1.7/STAIR/embedding/module_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.1.7/STAIR/embedding/module_hgat1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12324 2024-04-25 02:44:23.000000 STAIR-tools-1.1.7/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14202 2024-04-25 02:44:36.000000 STAIR-tools-1.1.7/STAIR/loc_prediction.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-26 05:50:41.899657 STAIR-tools-1.1.7/STAIR/location/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.7/STAIR/location/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.1.7/STAIR/location/align_fine.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.1.7/STAIR/location/align_init.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.1.7/STAIR/location/edge_detection.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.1.7/STAIR/location/edge_detection1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.1.7/STAIR/location/transformation.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1.7/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-26 05:50:41.900385 STAIR-tools-1.1.7/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-26 05:50:41.000000 STAIR-tools-1.1.7/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-04-26 05:50:41.000000 STAIR-tools-1.1.7/STAIR_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-04-26 05:50:41.000000 STAIR-tools-1.1.7/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-04-26 05:50:41.000000 STAIR-tools-1.1.7/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-04-26 05:50:41.900859 STAIR-tools-1.1.7/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      317 2024-04-26 05:50:31.000000 STAIR-tools-1.1.7/setup.py
```

### Comparing `STAIR-tools-1.1.6/README.md` & `STAIR-tools-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/ABA_annotation.py` & `STAIR-tools-1.1.7/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/emb_alignment.py` & `STAIR-tools-1.1.7/STAIR/emb_alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             self.makeLog(f"  Input scale: {scale}")
             self.makeLog(f"  Hvg: {self.hvg}")
 
     def preprocess( self,
                     lr = 0.001, 
                     weight_decay = 0, 
                     epoch_ae = 40, 
-                    batch_size = 128,
+                    batch_size = 64,
                     plot = False):
         '''
         Preprocessed training part using AE module
         
         Parameters
         ----------
         weight_decay
@@ -267,27 +267,27 @@
                     lib_tmp = lib_tmp.to(self.device)
                     rate_scaled_tmp, logits_tmp, _, z_tmp = self.ae(feat_tmp)
                     z = torch.cat([z, z_tmp.cpu()[:,:self.n_latent]])
                     rate_tmp = rate_scaled_tmp*lib_tmp
                     mean_tmp = rate_tmp*logits_tmp
                     mean = torch.cat([mean, mean_tmp.cpu()])
 
-        self.adata.obsm['X_CE'] = z.detach().cpu().numpy()
+        self.adata.obsm['latent'] = z.detach().cpu().numpy()
         self.adata.layers['Denoise'] = mean.detach().cpu().numpy()
 
         if return_data:
             return self.adata
     
     def prepare_hgat(self,
                      slice_key = None,
                      slice_order = None,
                      spatial_key = 'spatial',
                      n_neigh_hom = 10, 
                      c_neigh_het = 0.9,
-                     kernal_thresh = 0.5):
+                     kernal_thresh = 0.):
         '''
         Construct heterogeneous graph for HAT module.
 
         Parameters
         ----------
         slice_key
             Key of slice information in .obs.
@@ -314,16 +314,16 @@
         if self.make_log:
             self.makeLog(f"Module parameter set of HGAT")
             self.makeLog(f"  Spatial key: {spatial_key}")
             self.makeLog(f"  Neighbor number of intra-slice: {n_neigh_hom}")
             self.makeLog(f"  Similarity cutoff of inter-slice: {c_neigh_het}")
             
     def train_hgat( self,
-                    gamma: float = 0.9,
-                    epoch_hgat: int = 100,
+                    gamma: float = 0.8,
+                    epoch_hgat: int = 150,
                     re_weight: float = 1.,
                     si_weight: float = 0.,
                     lr: float = 0.001, 
                     weight_decay: float = 0.,
                     negative_slope: float = 0.2,
                     dropout_hom: float = 0.5,
                     dropout_het: float = 0.5,
```

### Comparing `STAIR-tools-1.1.6/STAIR/embedding/dataset_ae.py` & `STAIR-tools-1.1.7/STAIR/embedding/dataset_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/embedding/dataset_hgat.py` & `STAIR-tools-1.1.7/STAIR/embedding/dataset_hgat.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     feat_dict = {}
     adj_dict = {}
     coord_dict = {}
     index_dict = {}
 
     for batch_tmp in batch_order:
         adata_tmp = adata[adata.obs[batch_key]==batch_tmp].copy()
-        feat_tmp = adata_tmp.obsm['X_CE']
+        feat_tmp = adata_tmp.obsm['latent']
         coord_tmp = adata_tmp.obsm[spatial_key]
         adj_tmp = calcu_adj(coord_tmp, 
                             neigh_cal = 'knn', 
                             n_neigh = n_neigh_hom, 
                             metric ='minkowski')._indices()
         feat_dict[batch_tmp] = feat_tmp
         coord_dict[batch_tmp] = coord_tmp
```

### Comparing `STAIR-tools-1.1.6/STAIR/embedding/loss.py` & `STAIR-tools-1.1.7/STAIR/embedding/loss.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/embedding/module_ae.py` & `STAIR-tools-1.1.7/STAIR/embedding/module_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/embedding/module_hgat.py` & `STAIR-tools-1.1.7/STAIR/embedding/module_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/embedding/module_hgat1.py` & `STAIR-tools-1.1.7/STAIR/embedding/module_hgat1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/loc_alignment.py` & `STAIR-tools-1.1.7/STAIR/loc_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/loc_prediction.py` & `STAIR-tools-1.1.7/STAIR/loc_prediction.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/location/align_fine.py` & `STAIR-tools-1.1.7/STAIR/location/align_fine.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/location/align_init.py` & `STAIR-tools-1.1.7/STAIR/location/align_init.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/location/edge_detection.py` & `STAIR-tools-1.1.7/STAIR/location/edge_detection.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/location/edge_detection1.py` & `STAIR-tools-1.1.7/STAIR/location/edge_detection1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/location/transformation.py` & `STAIR-tools-1.1.7/STAIR/location/transformation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR/utils.py` & `STAIR-tools-1.1.7/STAIR/utils.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.6/STAIR_tools.egg-info/SOURCES.txt` & `STAIR-tools-1.1.7/STAIR_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

