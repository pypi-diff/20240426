# Comparing `tmp/scarcc-0.1.8-py3-none-any.whl.zip` & `tmp/scarcc-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 73550 bytes, number of entries: 61
+Zip file size: 73560 bytes, number of entries: 61
 -rw-rw-rw-  2.0 fat      267 b- defN 24-Feb-15 07:22 scarcc/__init__.py
 -rw-rw-rw-  2.0 fat      559 b- defN 24-Mar-25 23:28 scarcc/data_analysis/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-20 23:08 scarcc/data_analysis/biomass/__init__.py
 -rw-rw-rw-  2.0 fat     8441 b- defN 24-Mar-01 18:11 scarcc/data_analysis/biomass/_pathway_summary.py
 -rw-rw-rw-  2.0 fat     9500 b- defN 24-Mar-01 18:11 scarcc/data_analysis/biomass/growth_summary.py
 -rw-rw-rw-  2.0 fat     1790 b- defN 24-Feb-15 07:22 scarcc/data_analysis/biomass/plot_growth_curve.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-23 14:56 scarcc/data_analysis/drug_combination_response/__init__.py
@@ -40,24 +40,24 @@
 -rw-rw-rw-  2.0 fat     1344 b- defN 24-Mar-23 02:15 scarcc/preparation/perturbation/function/iter_species.py
 -rw-rw-rw-  2.0 fat     4748 b- defN 24-Mar-20 13:20 scarcc/preparation/perturbation/function/stoichiometry_scaling.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-15 07:22 scarcc/preparation/target_gene/__init__.py
 -rw-rw-rw-  2.0 fat     4772 b- defN 24-Mar-28 23:26 scarcc/preparation/target_gene/gene_format_handler.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-15 07:22 scarcc/preparation/target_gene/process_double_gene.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-15 07:22 scarcc/sim_engine/__init__.py
 -rw-rw-rw-  2.0 fat     4225 b- defN 24-Apr-25 13:01 scarcc/sim_engine/checkerboard_workflow.py
--rw-rw-rw-  2.0 fat     6296 b- defN 24-Apr-26 05:50 scarcc/sim_engine/flux_extraction.py
+-rw-rw-rw-  2.0 fat     6316 b- defN 24-Apr-26 06:02 scarcc/sim_engine/flux_extraction.py
 -rw-rw-rw-  2.0 fat    10971 b- defN 24-Mar-27 00:05 scarcc/sim_engine/output.py
 -rw-rw-rw-  2.0 fat     3660 b- defN 24-Mar-01 18:11 scarcc/sim_engine/result_processing.py
 -rw-rw-rw-  2.0 fat     6628 b- defN 24-Apr-25 11:36 scarcc/sim_engine/simulation_configuration.py
 -rw-rw-rw-  2.0 fat    10695 b- defN 24-Mar-27 00:06 scarcc/sim_engine/simulation_workflow.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-15 07:22 scarcc/sim_engine/data_processing/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-15 07:22 scarcc/sim_engine/data_processing/preprocess_flux.py
 -rw-rw-rw-  2.0 fat       94 b- defN 24-Feb-15 17:51 scarcc/util/__init__.py
 -rw-rw-rw-  2.0 fat     1445 b- defN 24-Feb-15 17:17 scarcc/util/util.py
 -rw-rw-rw-  2.0 fat       94 b- defN 24-Feb-15 17:51 scarcc/utils/__init__.py
 -rw-rw-rw-  2.0 fat     1506 b- defN 24-Mar-25 22:51 scarcc/utils/util.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-26 05:52 scarcc-0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1726 b- defN 24-Apr-26 05:52 scarcc-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-26 05:52 scarcc-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-26 05:52 scarcc-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     5965 b- defN 24-Apr-26 05:52 scarcc-0.1.8.dist-info/RECORD
-61 files, 206502 bytes uncompressed, 63714 bytes compressed:  69.1%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-26 06:04 scarcc-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1726 b- defN 24-Apr-26 06:04 scarcc-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-26 06:04 scarcc-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-26 06:04 scarcc-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     5965 b- defN 24-Apr-26 06:04 scarcc-0.1.9.dist-info/RECORD
+61 files, 206522 bytes uncompressed, 63724 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -162,23 +162,23 @@
 
 Filename: scarcc/utils/__init__.py
 Comment: 
 
 Filename: scarcc/utils/util.py
 Comment: 
 
-Filename: scarcc-0.1.8.dist-info/LICENSE
+Filename: scarcc-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: scarcc-0.1.8.dist-info/METADATA
+Filename: scarcc-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: scarcc-0.1.8.dist-info/WHEEL
+Filename: scarcc-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: scarcc-0.1.8.dist-info/top_level.txt
+Filename: scarcc-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: scarcc-0.1.8.dist-info/RECORD
+Filename: scarcc-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scarcc/sim_engine/flux_extraction.py

```diff
@@ -47,15 +47,15 @@
         self.biomass_df = (self.sim_object.total_biomass.set_index('cycle'))
         self.model_dict = {'E0': self.E0, 'S0': self.S0}
         self.species_list = [self.model_dict[ele] for ele in self.biomass_df.columns]
         self.culture = 'coculture' if len(self.species_list)>1 else f'monoculture'
         self.biomass_df = self.biomass_df.add_suffix(f'_{self.current_gene}_{self.culture}')
         
         if 'lv_pairs' in self.alpha_table.columns:
-            self.lv_pairs = '_'+'.'.join(self.alpha_table.lv_pairs.iloc[0])
+            self.lv_pairs = '_'+'.'.join([str(lv) for lv in self.alpha_table.lv_pairs.iloc[0]])
         else:
             self.lv_pairs = ''
         if self.save_raw_flux:
             self.flux_data_directory = os.path.join(self.data_directory, 'flux')
             os.makedirs(self.flux_data_directory, exist_ok=True)
 
 def get_flux_snapshot(sob: SimObjectBase, model: 'cobra.Model' = None):
```

## Comparing `scarcc-0.1.8.dist-info/LICENSE` & `scarcc-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `scarcc-0.1.8.dist-info/METADATA` & `scarcc-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scarcc
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/TFwongw/scarccpy
 Author: Thomas Wong
 Author-email: wong0755@umn.edu
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas <2.3
```

## Comparing `scarcc-0.1.8.dist-info/RECORD` & `scarcc-0.1.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -39,23 +39,23 @@
 scarcc/preparation/perturbation/function/iter_species.py,sha256=XSW3JMHaSL6FXm5INC_XUH61ttWwU0AJ4nBXeTyLieI,1344
 scarcc/preparation/perturbation/function/stoichiometry_scaling.py,sha256=6DDdXPZ0jBZP-FCoj5NfX4BCwZASAl9rGKHrh2RzXGM,4748
 scarcc/preparation/target_gene/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scarcc/preparation/target_gene/gene_format_handler.py,sha256=m01UyJZCIW5ERTdrgVc-8owPoJRCNuSHvELdvG56uLo,4772
 scarcc/preparation/target_gene/process_double_gene.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scarcc/sim_engine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scarcc/sim_engine/checkerboard_workflow.py,sha256=UnpQQwQqrLx1m78p1xFMJZCP8KAaztfI7y89FBv7eH4,4225
-scarcc/sim_engine/flux_extraction.py,sha256=esMalcbgNdVmpxRDr2lk3r_XsWAoFFUMA_phei7WSLs,6296
+scarcc/sim_engine/flux_extraction.py,sha256=SV_j_kbvx6IhvYBuYWM-uLpJRT9YEOUK-e0xTEFluTE,6316
 scarcc/sim_engine/output.py,sha256=t97F6cACMO9JydcnuNQGErwi82gFs5O1mSsmIzmSW08,10971
 scarcc/sim_engine/result_processing.py,sha256=wqvNx_ICS63JpbKbuRMqBKTzNs7ofd03dQ9L2xtx1NE,3660
 scarcc/sim_engine/simulation_configuration.py,sha256=1lC2zBrGAdpFmV9rEzGyodK-PP6iNHhmYn7jkTg2wLc,6628
 scarcc/sim_engine/simulation_workflow.py,sha256=ToxhtA9jrCZNP1niTJp57ubxIuzd3uqwg21e3pi66to,10695
 scarcc/sim_engine/data_processing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scarcc/sim_engine/data_processing/preprocess_flux.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scarcc/util/__init__.py,sha256=bO6ihaVtxewg8P3NpiELHZXpoOJ-LvmboIpDSlPhcjc,94
 scarcc/util/util.py,sha256=f4SJWb_5S0zKpievnUaQmKy9XO836SN5JEg7YjeLxK8,1445
 scarcc/utils/__init__.py,sha256=bO6ihaVtxewg8P3NpiELHZXpoOJ-LvmboIpDSlPhcjc,94
 scarcc/utils/util.py,sha256=u4XSdeS_MEzY5DYUIKihlSoKT0A-iCLKV3GmNUZGvQI,1506
-scarcc-0.1.8.dist-info/LICENSE,sha256=uNkWzH-e9JFmx7x2OZrnq8fKt1VDpNiUvOs_sNvRvNY,1085
-scarcc-0.1.8.dist-info/METADATA,sha256=B8ffBaBtlLw8fV6VSI3Ml1kVlY6hAyYiYzbaE2gVgBM,1726
-scarcc-0.1.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-scarcc-0.1.8.dist-info/top_level.txt,sha256=UVrBEYeLMxoSMvJ9qBqt0b_LoWGP9Q1DhjbVf6GOa1k,7
-scarcc-0.1.8.dist-info/RECORD,,
+scarcc-0.1.9.dist-info/LICENSE,sha256=uNkWzH-e9JFmx7x2OZrnq8fKt1VDpNiUvOs_sNvRvNY,1085
+scarcc-0.1.9.dist-info/METADATA,sha256=QrBxSRBGthLkwm5SWRELz7OKKmP5MwDtG98fuhbKKJQ,1726
+scarcc-0.1.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+scarcc-0.1.9.dist-info/top_level.txt,sha256=UVrBEYeLMxoSMvJ9qBqt0b_LoWGP9Q1DhjbVf6GOa1k,7
+scarcc-0.1.9.dist-info/RECORD,,
```

