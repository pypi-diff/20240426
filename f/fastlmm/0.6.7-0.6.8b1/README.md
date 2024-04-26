# Comparing `tmp/fastlmm-0.6.7.tar.gz` & `tmp/fastlmm-0.6.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlmm-0.6.7.tar", last modified: Fri Aug 11 14:17:31 2023, max compression
+gzip compressed data, was "fastlmm-0.6.8b1.tar", last modified: Fri Apr 26 02:01:31 2024, max compression
```

## Comparing `fastlmm-0.6.7.tar` & `fastlmm-0.6.8b1.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:31.974887 fastlmm-0.6.7/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      131 2022-02-24 16:06:33.000000 fastlmm-0.6.7/AUTHORS.txt
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    11554 2022-02-24 16:06:33.000000 fastlmm-0.6.7/LICENSE.md
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      214 2022-02-24 16:06:33.000000 fastlmm-0.6.7/MANIFEST.in
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     4826 2023-08-11 14:17:31.971887 fastlmm-0.6.7/PKG-INFO
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     4028 2022-06-22 20:24:55.000000 fastlmm-0.6.7/README.md
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:27.350250 fastlmm-0.6.7/fastlmm/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1157 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/__init__.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:28.235701 fastlmm-0.6.7/fastlmm/association/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    74141 2023-08-08 23:36:07.000000 fastlmm-0.6.7/fastlmm/association/FastLmmSet.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     3289 2023-08-08 23:36:06.000000 fastlmm-0.6.7/fastlmm/association/FastLmmSetLOOC.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:28.573790 fastlmm-0.6.7/fastlmm/association/Fastlmm_autoselect/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)   562014 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)  8451072 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe
--rwxrwxrwx   0 carlk     (1000) carlk     (1000) 12772999 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/Fastlmm_autoselect/fastlmmc
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)  1170360 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2633 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/LeaveOneChromosomeOut.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    15200 2023-08-08 23:36:08.000000 fastlmm-0.6.7/fastlmm/association/LocoGwas.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1648 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/PairResult.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     5843 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/PrecomputeLocoPcs.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2547 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/Result.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      720 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1362 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/_matchscript.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     9975 2023-08-08 23:36:09.000000 fastlmm-0.6.7/fastlmm/association/_pipelines.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:28.769533 fastlmm-0.6.7/fastlmm/association/altset_list/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      825 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/altset_list/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2195 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/altset_list/consecutive.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1790 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/altset_list/minmaxsetsize.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2044 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/altset_list/snpandsetnamecollection.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1662 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/altset_list/subset.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    28684 2023-08-08 23:36:06.000000 fastlmm-0.6.7/fastlmm/association/epistasis.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2727 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/fixed.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    13867 2023-08-08 23:36:06.000000 fastlmm-0.6.7/fastlmm/association/gwas.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    13069 2023-05-02 23:19:31.000000 fastlmm-0.6.7/fastlmm/association/gwas_eval.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    48104 2023-08-08 23:36:08.000000 fastlmm-0.6.7/fastlmm/association/heritability_spatial_correction.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    14572 2023-08-08 23:36:08.000000 fastlmm-0.6.7/fastlmm/association/lrt.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     4734 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/meta_analysis.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    20396 2023-08-08 23:36:08.000000 fastlmm-0.6.7/fastlmm/association/score.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    74854 2023-08-08 23:36:18.000000 fastlmm-0.6.7/fastlmm/association/single_snp.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    26459 2023-08-08 23:36:11.000000 fastlmm-0.6.7/fastlmm/association/single_snp_all_plus_select.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     9965 2023-08-08 23:36:10.000000 fastlmm-0.6.7/fastlmm/association/single_snp_linreg.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    78291 2023-08-08 23:36:10.000000 fastlmm-0.6.7/fastlmm/association/single_snp_scale.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    12977 2023-08-08 23:36:10.000000 fastlmm-0.6.7/fastlmm/association/single_snp_select.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     5873 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/snp_set.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    10038 2023-08-08 23:36:09.000000 fastlmm-0.6.7/fastlmm/association/testCV.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:29.344446 fastlmm-0.6.7/fastlmm/association/tests/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    10844 2023-08-08 23:36:12.000000 fastlmm-0.6.7/fastlmm/association/tests/Cv.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    11240 2023-08-08 23:36:12.000000 fastlmm-0.6.7/fastlmm/association/tests/LRT_up.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     7452 2023-08-08 23:36:12.000000 fastlmm-0.6.7/fastlmm/association/tests/Lrt.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     6806 2023-08-08 23:36:12.000000 fastlmm-0.6.7/fastlmm/association/tests/Sc.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      740 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/tests/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    20390 2023-08-08 23:36:11.000000 fastlmm-0.6.7/fastlmm/association/tests/test_gpu_perf.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    17823 2023-08-08 23:36:11.000000 fastlmm-0.6.7/fastlmm/association/tests/test_gwas.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     5468 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/tests/test_heritability_spatial_correction.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    52161 2023-08-08 23:36:12.000000 fastlmm-0.6.7/fastlmm/association/tests/test_single_snp.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    11187 2023-05-01 17:04:16.000000 fastlmm-0.6.7/fastlmm/association/tests/test_single_snp_all_plus_select.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     4864 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/tests/test_single_snp_linreg.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    15868 2022-10-23 19:11:46.000000 fastlmm-0.6.7/fastlmm/association/tests/test_single_snp_scale.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     9656 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/tests/test_single_snp_select.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     7398 2022-06-22 20:24:56.000000 fastlmm-0.6.7/fastlmm/association/tests/test_snp_set.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    20693 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/tests/testepistasis.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     3336 2023-08-08 23:36:11.000000 fastlmm-0.6.7/fastlmm/association/tests/tests_util.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      998 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/association/varcomp_test.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     7506 2023-08-08 23:36:09.000000 fastlmm-0.6.7/fastlmm/association/windowing_gwas.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:29.398488 fastlmm-0.6.7/fastlmm/external/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/external/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    30386 2023-08-08 23:36:12.000000 fastlmm-0.6.7/fastlmm/external/pca.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:29.464192 fastlmm-0.6.7/fastlmm/external/util/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/external/util/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1904 2023-05-02 23:19:31.000000 fastlmm-0.6.7/fastlmm/external/util/math.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:29.691029 fastlmm-0.6.7/fastlmm/feature_selection/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    20089 2023-08-08 23:36:16.000000 fastlmm-0.6.7/fastlmm/feature_selection/PerformSelectionDistributable.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      102 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/feature_selection/__init__.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:30.212698 fastlmm-0.6.7/fastlmm/feature_selection/examples/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      933 2023-08-08 23:36:16.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      616 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      702 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/ScanOSP.Toydata.config.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      217 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/bronze.txt
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)  1250003 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.5chrom.bed
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)   237784 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.5chrom.bim
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    14861 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.5chrom.fam
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    10798 2022-02-24 16:06:33.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.cov
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)   197784 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.map
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    11016 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.phe
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    11164 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.shufflePlus.phe
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)       24 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.sim
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     5357 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/toydataTest.phe
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     5473 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/feature_selection/examples/toydataTrain.phe
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    43490 2023-08-08 23:36:16.000000 fastlmm-0.6.7/fastlmm/feature_selection/feature_selection_cv.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2351 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/feature_selection/feature_selection_example.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    13525 2023-05-02 23:19:31.000000 fastlmm-0.6.7/fastlmm/feature_selection/feature_selection_two_kernel.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     6573 2023-05-02 23:19:31.000000 fastlmm-0.6.7/fastlmm/feature_selection/kernel_ridge_cv.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    23331 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/feature_selection/test.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:30.490776 fastlmm-0.6.7/fastlmm/inference/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1712 2023-08-08 23:36:14.000000 fastlmm-0.6.7/fastlmm/inference/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    13253 2023-08-08 23:36:13.000000 fastlmm-0.6.7/fastlmm/inference/ep.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    38590 2023-08-08 23:36:13.000000 fastlmm-0.6.7/fastlmm/inference/fastlmm_predictor.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    27004 2023-08-08 23:36:15.000000 fastlmm-0.6.7/fastlmm/inference/glmm.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    18157 2023-08-11 01:23:10.000000 fastlmm-0.6.7/fastlmm/inference/laplace.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     3100 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/inference/likelihood.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    20846 2023-08-08 23:36:13.000000 fastlmm-0.6.7/fastlmm/inference/linear_regression.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    40938 2023-08-08 23:36:14.000000 fastlmm-0.6.7/fastlmm/inference/lmm.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    24336 2023-08-08 23:36:13.000000 fastlmm-0.6.7/fastlmm/inference/lmm2k.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    56272 2023-08-08 23:36:14.000000 fastlmm-0.6.7/fastlmm/inference/lmm_cov.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:30.623216 fastlmm-0.6.7/fastlmm/inference/tests/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/inference/tests/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    27208 2023-08-10 22:41:19.000000 fastlmm-0.6.7/fastlmm/inference/tests/test.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    58459 2023-08-08 23:36:16.000000 fastlmm-0.6.7/fastlmm/inference/tests/test_fastlmm_predictor.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     9815 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/inference/tests/test_linear_regression.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:30.767172 fastlmm-0.6.7/fastlmm/pyplink/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)       49 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/__init__.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:30.933453 fastlmm-0.6.7/fastlmm/pyplink/altset_list/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2263 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/altset_list/Consecutive.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1759 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/altset_list/MinMaxSetSize.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     3647 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1634 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/altset_list/Subset.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      685 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/altset_list/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     7392 2023-08-08 23:36:03.000000 fastlmm-0.6.7/fastlmm/pyplink/plink.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1712 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/setup.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:31.073200 fastlmm-0.6.7/fastlmm/pyplink/snpreader/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    13017 2023-08-08 23:36:03.000000 fastlmm-0.6.7/fastlmm/pyplink/snpreader/Bed.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     8253 2023-08-08 23:36:03.000000 fastlmm-0.6.7/fastlmm/pyplink/snpreader/Dat.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     9674 2023-08-08 23:36:03.000000 fastlmm-0.6.7/fastlmm/pyplink/snpreader/Hdf5.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      160 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/snpreader/__init__.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:31.274896 fastlmm-0.6.7/fastlmm/pyplink/snpset/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1147 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/snpset/AllSnps.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1840 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/snpset/PositionRange.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1734 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/snpset/RandomSnpSet.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1377 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/snpset/SnpIndexList.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1489 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/snpset/SnpSetAndName.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1717 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/snpset/SnpsFromFile.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      762 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/snpset/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1238 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/test.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2866 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/pyplink/vcfpy.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:31.658258 fastlmm-0.6.7/fastlmm/util/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    12054 2023-08-08 23:36:02.000000 fastlmm-0.6.7/fastlmm/util/NearBronze.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     4103 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/VertexCut.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      197 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     3014 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/_example_file.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2116 2023-08-08 23:36:01.000000 fastlmm-0.6.7/fastlmm/util/computePC.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     7008 2023-08-08 23:36:01.000000 fastlmm-0.6.7/fastlmm/util/compute_auto_pcs.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2122 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/est_h2.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     6515 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/fastlmm.hashdown.json
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     3677 2023-08-08 23:36:02.000000 fastlmm-0.6.7/fastlmm/util/genphen.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2138 2022-09-08 16:36:29.000000 fastlmm-0.6.7/fastlmm/util/gensnp.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:31.718093 fastlmm-0.6.7/fastlmm/util/matrix/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/matrix/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    10139 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/matrix/mmultfile.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     6044 2023-08-08 23:36:02.000000 fastlmm-0.6.7/fastlmm/util/mingrid.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1095 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/pickle_io.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1873 2023-08-08 23:36:02.000000 fastlmm-0.6.7/fastlmm/util/preprocess.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     9019 2023-05-02 23:19:31.000000 fastlmm-0.6.7/fastlmm/util/run_fastlmmc.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:31.840393 fastlmm-0.6.7/fastlmm/util/standardizer/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1387 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/standardizer/Beta.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1370 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/standardizer/Unit.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     2410 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/standardizer/__init__.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:31.926246 fastlmm-0.6.7/fastlmm/util/stats/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     5895 2023-08-08 23:36:02.000000 fastlmm-0.6.7/fastlmm/util/stats/__init__.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    13559 2023-08-08 23:36:03.000000 fastlmm-0.6.7/fastlmm/util/stats/chi2mixture.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    32968 2023-08-08 23:36:03.000000 fastlmm-0.6.7/fastlmm/util/stats/plotp.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     1932 2022-02-24 16:06:34.000000 fastlmm-0.6.7/fastlmm/util/test.py
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)    22975 2023-08-08 23:36:02.000000 fastlmm-0.6.7/fastlmm/util/util.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:27.460501 fastlmm-0.6.7/fastlmm.egg-info/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     4826 2023-08-11 14:17:26.000000 fastlmm-0.6.7/fastlmm.egg-info/PKG-INFO
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     5484 2023-08-11 14:17:27.000000 fastlmm-0.6.7/fastlmm.egg-info/SOURCES.txt
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)        1 2023-08-11 14:17:26.000000 fastlmm-0.6.7/fastlmm.egg-info/dependency_links.txt
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      143 2023-08-11 14:17:26.000000 fastlmm-0.6.7/fastlmm.egg-info/requires.txt
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      364 2023-08-11 14:17:26.000000 fastlmm-0.6.7/fastlmm.egg-info/top_level.txt
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)      137 2022-02-24 16:06:34.000000 fastlmm-0.6.7/pyproject.toml
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)       38 2023-08-11 14:17:31.975888 fastlmm-0.6.7/setup.cfg
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     3282 2023-08-11 14:17:23.000000 fastlmm-0.6.7/setup.py
-drwxrwxrwx   0 carlk     (1000) carlk     (1000)        0 2023-08-11 14:17:31.950758 fastlmm-0.6.7/tests/
--rwxrwxrwx   0 carlk     (1000) carlk     (1000)     7962 2023-05-02 23:19:31.000000 fastlmm-0.6.7/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.328031 fastlmm-0.6.8b1/fastlmm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.332031 fastlmm-0.6.8b1/fastlmm/association/
+-rw-r--r--   0 runner    (1001) docker     (127)    74123 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/FastLmmSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/FastLmmSetLOOC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.360031 fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/
+-rw-r--r--   0 runner    (1001) docker     (127)   562014 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)  8451072 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe
+-rw-r--r--   0 runner    (1001) docker     (127) 12772999 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/fastlmmc
+-rw-r--r--   0 runner    (1001) docker     (127)  1170360 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/LeaveOneChromosomeOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15180 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/LocoGwas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/PairResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/PrecomputeLocoPcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/_matchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.360031 fastlmm-0.6.8b1/fastlmm/association/altset_list/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/altset_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/altset_list/consecutive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/altset_list/minmaxsetsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/altset_list/snpandsetnamecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/altset_list/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28684 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/epistasis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/gwas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/gwas_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48108 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/heritability_spatial_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/meta_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20307 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74820 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/single_snp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26459 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/single_snp_all_plus_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/single_snp_linreg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78291 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/single_snp_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/single_snp_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/snp_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/testCV.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.364030 fastlmm-0.6.8b1/fastlmm/association/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/Cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/LRT_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/Lrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/Sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20390 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_gpu_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_gwas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_heritability_spatial_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52161 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_all_plus_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_linreg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15875 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_snp_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21938 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/testepistasis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/tests_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/varcomp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/windowing_gwas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.364030 fastlmm-0.6.8b1/fastlmm/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30319 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/external/pca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.364030 fastlmm-0.6.8b1/fastlmm/external/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/external/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/external/util/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.364030 fastlmm-0.6.8b1/fastlmm/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/PerformSelectionDistributable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.368030 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanOSP.Toydata.config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/bronze.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1250003 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   237784 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.bim
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.fam
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.cov
+-rw-r--r--   0 runner    (1001) docker     (127)   197784 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.map
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.phe
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.shufflePlus.phe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.sim
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydataTest.phe
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydataTrain.phe
+-rw-r--r--   0 runner    (1001) docker     (127)    43450 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_two_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/kernel_ridge_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27797 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.372030 fastlmm-0.6.8b1/fastlmm/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/ep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38590 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/fastlmm_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26907 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/glmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20767 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40898 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/lmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24225 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/lmm2k.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56134 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/lmm_cov.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.372030 fastlmm-0.6.8b1/fastlmm/inference/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58459 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/tests/test_fastlmm_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/tests/test_linear_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.372030 fastlmm-0.6.8b1/fastlmm/pyplink/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.376030 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/Consecutive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/MinMaxSetSize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/Subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/plink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.376030 fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Dat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.376030 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/AllSnps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/PositionRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/RandomSnpSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpIndexList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpSetAndName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpsFromFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/vcfpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/fastlmm/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/NearBronze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/VertexCut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/_example_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/computePC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/compute_auto_pcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/est_h2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/fastlmm.hashdown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/genphen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/gensnp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/fastlmm/util/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/matrix/mmultfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/mingrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/pickle_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/run_fastlmmc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/fastlmm/util/standardizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/standardizer/Beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/standardizer/Unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/standardizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/fastlmm/util/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/stats/chi2mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32930 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/stats/plotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.328031 fastlmm-0.6.8b1/fastlmm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-26 02:01:31.000000 fastlmm-0.6.8b1/fastlmm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-26 02:01:31.000000 fastlmm-0.6.8b1/fastlmm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 02:01:31.000000 fastlmm-0.6.8b1/fastlmm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 02:01:31.000000 fastlmm-0.6.8b1/fastlmm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-26 02:01:31.000000 fastlmm-0.6.8b1/fastlmm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/tests/test.py
```

### Comparing `fastlmm-0.6.7/LICENSE.md` & `fastlmm-0.6.8b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/PKG-INFO` & `fastlmm-0.6.8b1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlmm
-Version: 0.6.7
+Version: 0.6.8b1
 Summary: Fast GWAS
 Home-page: https://fastlmm.github.io/
 Author: FaST-LMM Team
 Author-email: fastlmm-dev@python.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/fastlmm/FaST-LMM/issues
 Project-URL: Documentation, http://fastlmm.github.io/FaST-LMM
@@ -15,52 +15,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS.txt
+Requires-Dist: pandas>=1.1.1
+Requires-Dist: matplotlib>=1.5.1
+Requires-Dist: scikit-learn>=0.19.1
+Requires-Dist: bed-reader>=1.0.4
+Requires-Dist: pysnptools>=0.5.11
+Requires-Dist: cloudpickle>=2.2.0
+Requires-Dist: statsmodels>=0.10.1
+Requires-Dist: psutil>=5.6.7
+Requires-Dist: fastlmmclib>=0.0.3
 
 FaST-LMM
 =================================
 
 FaST-LMM, which stands for Factored Spectrally Transformed Linear Mixed Models, is a program for performing 
 genome-wide association studies (GWAS) on datasets of all sizes, up to one millions samples.
 
 This release contains the following features, each illustrated with an IPython notebook.
 
-* Core FaST-LMM ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
+* Core FaST-LMM ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
 
 Improvements:
 
-* New features for single_snp (including effect size and multiple phenotype support) and epistasis (including reporting beta and using pre-computed eigenvalue decompositions) ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb))  -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
-* Ludicrous-Speed GWAS ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)) -- [Kadie and Heckerman, *bioRxiv* 2018](https://www.biorxiv.org/content/10.1101/154682v2)
-* Heritability with Spatial Correction ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)), [Heckerman *et al.*, *PNAS* 2016](http://www.pnas.org/content/113/27/7377.abstract)
-* Two Kernels ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Widmer *et al.*, *Scientific Reports* 2014](http://www.nature.com/srep/2014/141112/srep06874/full/srep06874.html)
-* Set Analysis ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Bioinformatics* 2014](http://bioinformatics.oxfordjournals.org/content/early/2014/09/07/bioinformatics.btu504)
-* Epistasis ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Scientific Reports,* 2013](http://www.nature.com/srep/2013/130122/srep01099/full/srep01099.html)
-* Prediction ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
+* New features for single_snp (including effect size and multiple phenotype support) and epistasis (including reporting beta and using pre-computed eigenvalue decompositions) ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb))  -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
+* Ludicrous-Speed GWAS ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)) -- [Kadie and Heckerman, *bioRxiv* 2018](https://www.biorxiv.org/content/10.1101/154682v2)
+* Heritability with Spatial Correction ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)), [Heckerman *et al.*, *PNAS* 2016](http://www.pnas.org/content/113/27/7377.abstract)
+* Two Kernels ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Widmer *et al.*, *Scientific Reports* 2014](http://www.nature.com/srep/2014/141112/srep06874/full/srep06874.html)
+* Set Analysis ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Bioinformatics* 2014](http://bioinformatics.oxfordjournals.org/content/early/2014/09/07/bioinformatics.btu504)
+* Epistasis ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Scientific Reports,* 2013](http://www.nature.com/srep/2013/130122/srep01099/full/srep01099.html)
+* Prediction ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
 
 *A C++ version, which is generally less functional, is available. See http://fastlmm.github.io/.*
 
 Quick install:
 =================================
 
 `pip install fastlmm`
 
 For best performance, be sure your Python distribution includes a fast version of NumPy. We use Anaconda's [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
 
 Documentation
 =================================
 
 * IPython Notebooks:
-	* [Core, Epistasis, Set Analysis, Two Kernels](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)
-    * [Multiple-Phenotype GWAS and related features](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb)
-	* [Heritability with Spatial Correction](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)
-	* [Ludicrous-Speed GWAS](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)
+	* [Core, Epistasis, Set Analysis, Two Kernels](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)
+    * [Multiple-Phenotype GWAS and related features](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb)
+	* [Heritability with Spatial Correction](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)
+	* [Ludicrous-Speed GWAS](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)
 * [Main Documentation](http://fastlmm.github.io/FaST-LMM/)
 * [Project Home and Full Annotated Bibliography](https://fastlmm.github.io/)
 
 
 Code
 =================================
 * [PyPi](https://pypi.org/project/fastlmm/)
```

### Comparing `fastlmm-0.6.7/README.md` & `fastlmm-0.6.8b1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 =================================
 
 FaST-LMM, which stands for Factored Spectrally Transformed Linear Mixed Models, is a program for performing 
 genome-wide association studies (GWAS) on datasets of all sizes, up to one millions samples.
 
 This release contains the following features, each illustrated with an IPython notebook.
 
-* Core FaST-LMM ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
+* Core FaST-LMM ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
 
 Improvements:
 
-* New features for single_snp (including effect size and multiple phenotype support) and epistasis (including reporting beta and using pre-computed eigenvalue decompositions) ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb))  -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
-* Ludicrous-Speed GWAS ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)) -- [Kadie and Heckerman, *bioRxiv* 2018](https://www.biorxiv.org/content/10.1101/154682v2)
-* Heritability with Spatial Correction ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)), [Heckerman *et al.*, *PNAS* 2016](http://www.pnas.org/content/113/27/7377.abstract)
-* Two Kernels ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Widmer *et al.*, *Scientific Reports* 2014](http://www.nature.com/srep/2014/141112/srep06874/full/srep06874.html)
-* Set Analysis ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Bioinformatics* 2014](http://bioinformatics.oxfordjournals.org/content/early/2014/09/07/bioinformatics.btu504)
-* Epistasis ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Scientific Reports,* 2013](http://www.nature.com/srep/2013/130122/srep01099/full/srep01099.html)
-* Prediction ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
+* New features for single_snp (including effect size and multiple phenotype support) and epistasis (including reporting beta and using pre-computed eigenvalue decompositions) ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb))  -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
+* Ludicrous-Speed GWAS ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)) -- [Kadie and Heckerman, *bioRxiv* 2018](https://www.biorxiv.org/content/10.1101/154682v2)
+* Heritability with Spatial Correction ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)), [Heckerman *et al.*, *PNAS* 2016](http://www.pnas.org/content/113/27/7377.abstract)
+* Two Kernels ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Widmer *et al.*, *Scientific Reports* 2014](http://www.nature.com/srep/2014/141112/srep06874/full/srep06874.html)
+* Set Analysis ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Bioinformatics* 2014](http://bioinformatics.oxfordjournals.org/content/early/2014/09/07/bioinformatics.btu504)
+* Epistasis ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Scientific Reports,* 2013](http://www.nature.com/srep/2013/130122/srep01099/full/srep01099.html)
+* Prediction ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
 
 *A C++ version, which is generally less functional, is available. See http://fastlmm.github.io/.*
 
 Quick install:
 =================================
 
 `pip install fastlmm`
 
 For best performance, be sure your Python distribution includes a fast version of NumPy. We use Anaconda's [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
 
 Documentation
 =================================
 
 * IPython Notebooks:
-	* [Core, Epistasis, Set Analysis, Two Kernels](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)
-    * [Multiple-Phenotype GWAS and related features](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb)
-	* [Heritability with Spatial Correction](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)
-	* [Ludicrous-Speed GWAS](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)
+	* [Core, Epistasis, Set Analysis, Two Kernels](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)
+    * [Multiple-Phenotype GWAS and related features](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb)
+	* [Heritability with Spatial Correction](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)
+	* [Ludicrous-Speed GWAS](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)
 * [Main Documentation](http://fastlmm.github.io/FaST-LMM/)
 * [Project Home and Full Annotated Bibliography](https://fastlmm.github.io/)
 
 
 Code
 =================================
 * [PyPi](https://pypi.org/project/fastlmm/)
```

### Comparing `fastlmm-0.6.7/fastlmm/__init__.py` & `fastlmm-0.6.8b1/fastlmm/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-from __future__ import absolute_import
 import warnings
 
+
 class OutputWriter(object):
-    ''' Centralize output without messing with sys.stdout. '''
+    """Centralize output without messing with sys.stdout."""
+
     _streams = []
 
     def addOutputStream(self, out):
         for o in self._streams:
             if o is out:
                 return
         self._streams.append(out)
-    
+
     def write(self, msg):
-        warnings.warn("Pr and OutputWriter are deprecated. Use the standard logging.info() instead", DeprecationWarning)
+        warnings.warn(
+            "Pr and OutputWriter are deprecated. Use the standard logging.info() instead",
+            DeprecationWarning,
+        )
         for s in self._streams:
             s.write(msg)
-    
+
     def prin(self, msg):
-        warnings.warn("Pr and OutputWriter are deprecated. Use the standard logging.info() instead", DeprecationWarning)
-        self.write(msg+'\n')
+        warnings.warn(
+            "Pr and OutputWriter are deprecated. Use the standard logging.info() instead",
+            DeprecationWarning,
+        )
+        self.write(msg + "\n")
 
     def close(self):
         for s in self._streams:
             s.close()
 
     def fileno(self):
         for s in self._streams:
-            if 'fileno' in dir(s):
+            if "fileno" in dir(s):
                 return s.fileno()
         return 0
 
     def flush(self):
         for s in self._streams:
-            if 'flush' in dir(s):
+            if "flush" in dir(s):
                 s.flush()
 
+
 # This is the only OutputWriter instance that you should use.
 Pr = OutputWriter()
```

### Comparing `fastlmm-0.6.7/fastlmm/association/FastLmmSet.py` & `fastlmm-0.6.8b1/fastlmm/association/FastLmmSet.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import fastlmm.util.util as utilx
 import fastlmm.util.stats as ss
 import time
 from .Result import *
 from .PairResult import *
 from fastlmm.association.tests import *
 import fastlmm.util.genphen as gp
-import scipy as sp
 import numpy as np
 from itertools import *
 from fastlmm.pyplink.snpreader.Bed import *
 import logging
 import warnings
 from tempfile import TemporaryFile
 import fastlmm.util.preprocess as util
@@ -184,15 +183,15 @@
                 * (1 + self.nperm)
             )
 
     def printPhenToFile(self, nInd, SNPsalt, y):
         self._synthphenfile = utilx.appendtofilename(self.outfile, "synthPhenVarBack")
         np.savetxt(self._synthphenfile, y)
         with open(self._synthphenfile, "w") as fp:
-            for n in sp.arange(0, nInd):
+            for n in np.arange(0, nInd):
                 fp.write(
                     SNPsalt["iid"][n][0]
                     + "\t"
                     + SNPsalt["iid"][n][1]
                     + "\t"
                     + "%f" % y[n]
                     + "\n"
@@ -216,20 +215,20 @@
             if self.altset_list2 is None:  # singleton sets
                 for iset, altset in enumerate(self.altsetlist_filtbysnps):
                     for iperm in range(
                         -1, self.nperm
                     ):  # note that self.nperm is the 'stop', not the 'count'
                         SNPsalt = altset.read()
                         SNPsalt["snps"] = util.standardize(SNPsalt["snps"])
-                        G1 = SNPsalt["snps"] / sp.sqrt(SNPsalt["snps"].shape[1])
+                        G1 = SNPsalt["snps"] / np.sqrt(SNPsalt["snps"].shape[1])
                         ichrm = ",".join(
-                            sp.array(sp.unique(SNPsalt["pos"][:, 0]), dtype=str)
+                            np.array(np.unique(SNPsalt["pos"][:, 0]), dtype=str)
                         )
-                        minpos = str(sp.min(SNPsalt["pos"][:, 2]))
-                        maxpos = str(sp.max(SNPsalt["pos"][:, 2]))
+                        minpos = str(np.min(SNPsalt["pos"][:, 2]))
+                        maxpos = str(np.max(SNPsalt["pos"][:, 2]))
                         iposrange = minpos + "-" + maxpos
 
                         if self.genphen is None:
                             y = self.__y
                         else:
                             assert (
                                 self.permute is None
@@ -243,38 +242,38 @@
                                 newseed = self.mainseed ^ self.genphen["seed"]
                                 from numpy.random import RandomState
 
                                 randomstate = RandomState(newseed)
                                 nSnp = self.__SNPs0["data"]["snps"].shape[1]
                                 # good for low rank, other wise, use the dual, as in gp.genphen
                                 raise Exception("Bug below. should be randn, is rand")
-                                y_G0 = sp.sqrt(
+                                y_G0 = np.sqrt(
                                     self.genphen["varBack"] / nSnp
                                 ) * self.__SNPs0["data"]["snps"].dot(
                                     randomstate.rand(nSnp, 1)
                                 )  # TODO: CL This seems to be a bug. Should be randn
-                                # y_G0=sp.sqrt(self.genphen["varBack"])*self.__SNPs0['data']['snps'].dot(randomstate.rand(nSnp,1))    #TODO: CL This seems to be a bug. Should be randn
+                                # y_G0=np.sqrt(self.genphen["varBack"])*self.__SNPs0['data']['snps'].dot(randomstate.rand(nSnp,1))    #TODO: CL This seems to be a bug. Should be randn
                             elif self.__SNPs0 is None:
                                 y_G0 = 0
 
                             # always have the same background signal
                             if (
                                 self.genphen["varBackNullFileGen"] is not None
                                 and y_back is None
                             ):
                                 nSnp = self.__SNPs0["data"]["snps"].shape[1]
                                 y_back = (
-                                    sp.sqrt(self.genphen["varBack"] / nSnp)
+                                    np.sqrt(self.genphen["varBack"] / nSnp)
                                     * self.__varBackNullSnpsGen["snps"].dot(
                                         np.random.randn(
                                             self.__varBackNullSnpsGen["snps"].shape[1],
                                             1,
                                         )
                                     )
-                                    / sp.sqrt(
+                                    / np.sqrt(
                                         self.__varBackNullSnpsGen["snps"].shape[1]
                                     )
                                 )
                                 # self.printPhenToFile(nInd, SNPsalt, y_back);
                             elif (
                                 "varBackNullPhenGen" in self.genphen
                                 and self.genphen["varBackNullPhenGen"] is not None
@@ -411,38 +410,38 @@
             logging.info("distributable = " + self.__repr__())
 
             self.run_once()  # load files, etc. -- doesn't actually do the work if it's already been done
             # note, however, that before reduce is called, work_count calls run_once() anyhow
 
             result_dict = {}
 
-            lrt = SP.nan * SP.ones(len(self.altsetlist_filtbysnps))
+            lrt = np.nan * np.ones(len(self.altsetlist_filtbysnps))
             # whether alt and null models give the same margll
             alteqnull = [None] * len(self.altsetlist_filtbysnps)
 
-            lrtperm = SP.nan * SP.ones(len(self.altsetlist_filtbysnps) * self.nperm)
+            lrtperm = np.nan * np.ones(len(self.altsetlist_filtbysnps) * self.nperm)
             alteqnullperm = [None] * len(self.altsetlist_filtbysnps) * self.nperm
-            setsizeperm = SP.nan * SP.ones(len(self.altsetlist_filtbysnps) * self.nperm)
+            setsizeperm = np.nan * np.ones(len(self.altsetlist_filtbysnps) * self.nperm)
 
             npvals = self.test.npvals
-            pv_adj = sp.nan * sp.ones((len(self.altsetlist_filtbysnps)))
+            pv_adj = np.nan * np.ones((len(self.altsetlist_filtbysnps)))
 
             # results can come in any order, so we have to use iperm and iset to put them in the right place
             # there is one result instance for each combination of test and permutation, and here we are just gathering them
             # into the arrays from above
 
             for result_list in result_list_sequence:
                 for result in result_list:
                     if result.iperm < 0:
                         result_dict[result.iset] = result
                         # iset is the index of the test (irrespective of permutation)
                         lrt[result.iset] = self.test.lrt_method(result)
-                        alteqnull[
-                            result.iset
-                        ] = result.alteqnull  # equiv to result["alteqnull"]
+                        alteqnull[result.iset] = (
+                            result.alteqnull
+                        )  # equiv to result["alteqnull"]
                         # pv_adj[result.iset,:] = self.test.pv_adj_from_result(result)
                         pv_adj[result.iset] = self.test.pv_adj_from_result(result)
                     else:
                         isetiperm = result.iset + result.iperm * len(
                             self.altsetlist_filtbysnps
                         )
                         lrtperm[isetiperm] = self.test.lrt_method(result)
@@ -512,23 +511,23 @@
     #    from numpy.random import RandomState
     #    import pysnptools.util.gensnp as gp #!!! does this work?
     #    randomstate = RandomState(newseed)
     #    nSnp=genphen["numBackSnps"]
     #    #randsnps=self.alt_snpreader.read(RandomSnpSet(nSnp,newseed))     #this appears to be VERY slow
     #    #snps=randsnps['snps']
     #    snps=gp.gensnps(nInd,nSnp)
-    #    randG = snps/sp.sqrt(nSnp) #pre-process for kernel
-    #    y_randG=sp.sqrt(genphen["varBack"])*randG.dot(randomstate.rand(nSnp,1))
+    #    randG = snps/np.sqrt(nSnp) #pre-process for kernel
+    #    y_randG=np.sqrt(genphen["varBack"])*randG.dot(randomstate.rand(nSnp,1))
     #    return y_randG
 
     def TESTBEFOREUSINGKfromAltSnps(self, N, SNPsalt=None):
         print("constructing K from all SNPs")
         t0 = time.time()
 
-        Kall = sp.zeros([N, N])
+        Kall = np.zeros([N, N])
         nSnpTotal = self.alt_snpreader.snp_count
         print("reading in " + str(nSnpTotal) + " SNPs and adding up kernels")
         # altsnps = readBED(self.bedfilealt,standardizeSNPs=True)['snps'] #loads all in to memory
         blocksize = 100
         ct = 0
         ts = time.time()
         if self.alt_snpreader.snp_count < N:
@@ -545,18 +544,18 @@
             Kall = Kall + snps.dot(snps.T)
             t1 = time.time()
             if ct % 50000 == 0:
                 print("read %s SNPs in %.2f seconds" % (ct, t1 - ts))
                 ts = time.time()
             # if ct==2:
             #    break
-            #    Kall=sp.rand((N,N))
+            #    Kall=np.rand((N,N))
             #    Kall=Kall.dot(Kall.T)
-        Kall = Kall / sp.sqrt(self.alt_snpreader.snp_count)
-        Kall = Kall + 1e-5 * sp.eye(N, N)
+        Kall = Kall / np.sqrt(self.alt_snpreader.snp_count)
+        Kall = Kall + 1e-5 * np.eye(N, N)
         t1 = time.time()
         logging.info("%.2f seconds elapsed" % (t1 - t0))
 
         return Kall
 
     def _saveArray(self, appendNameFile, header, values):
         outfile = utilx.appendtofilename(self.outfile, appendNameFile)
@@ -568,18 +567,18 @@
                     outfile
                 )
             )
 
         logging.info("writing to file " + outfile + ".")
 
         assert (
-            type(values) == sp.ndarray or type(values) == tuple
-        ), "values can only be sp.ndarray or a tuple of sp.ndarray."
+            type(values) == np.ndarray or type(values) == tuple
+        ), "values can only be np.ndarray or a tuple of np.ndarray."
 
-        if type(values) == sp.ndarray:
+        if type(values) == np.ndarray:
             values = (values,)
 
         values = list(map(list, list(zip(*values))))
 
         with open(outfile, "w") as fp:
             fp.write("\t".join(header) + "\n")
             for v in values:
@@ -726,15 +725,15 @@
 
         randomstate = RandomState(self.rseed)
         checkpoint = 1000
         powerneeded = 2
         for pm in range(self.nlocalperm):
             if pm == checkpoint:
                 logging.info("checkpointing " + str(pm))
-                numbetter = sp.sum(permstatbetter)
+                numbetter = np.sum(permstatbetter)
                 pv = numbetter / float(pm)
                 t1 = time.time()
                 logging.info("Checkpoint time elapsed=%.2f seconds" % (t1 - t0))
                 if pv * checkpoint >= 10**powerneeded:
                     logging.info("stopping due to checkpoint")
                     break
                 checkpoint = checkpoint * 2
@@ -744,37 +743,37 @@
             Xperm = self.__X[permutationIndex]
 
             permresult = varcomp_test.testGupdate(yperm, Xperm, self.test)
             allstat.append(permresult["stat"])
             alteqnullperm.append(permresult["alteqnull"])
             permstatbetter.append(permresult["stat"] - result.test["stat"] > tol)
 
-        numbetter = sp.maximum(0.99, sp.sum(permstatbetter))
+        numbetter = np.maximum(0.99, np.sum(permstatbetter))
         pv = numbetter / float(pm)
         result.test["pv-local"] = pv
         result.test["pv"] = result.test["pv"]
 
         if self.fitlocal and pv * pm < 10**powerneeded:
             import fastlmm.association.tests.Cv as cv
 
             logging.info("fitting aUD to local with " + str(pm + 1) + " permutations")
             pv_adj, mixture, scale, dof = cv.lrtpvals_qqfit(
                 nperm=self.nlocalperm,
-                lrt=sp.array([result.test["stat"]]),
-                lrtperm=sp.array(allstat),
-                alteqnull=sp.array([result.test["alteqnull"]]),
-                alteqnullperm=sp.array(alteqnullperm),
+                lrt=np.array([result.test["stat"]]),
+                lrtperm=np.array(allstat),
+                alteqnull=np.array([result.test["alteqnull"]]),
+                alteqnullperm=np.array(alteqnullperm),
                 qmax=self.qmax,
             )
             result.test["pv-local-aUD"] = pv_adj[0]
             logging.info("mixture (non-zero dof)=" + str(mixture))
             logging.info("dof=" + str(dof))
             logging.info("scale=" + str(scale))
         else:
-            result.test["pv-local-aUD"] = sp.NaN
+            result.test["pv-local-aUD"] = np.NaN
 
         logging.info(
             "    used "
             + str(pm + 1)
             + " permutations to compute p="
             + str(pv)
             + ", p50="
@@ -787,15 +786,15 @@
         else:
             snp_names = self.__SNPs0["reader"].rs[i_exclude]
             snp_set = SnpAndSetName("G_exclude", snp_names)
             G_exclude = self.__SNPs0["reader"].read(snp_set)["snps"]
             G_exclude = util.standardize(G_exclude)
             # normalize
             pass
-        G_exclude /= sp.sqrt(self.__SNPs0["num_snps"])
+        G_exclude /= np.sqrt(self.__SNPs0["num_snps"])
         return G_exclude
 
     def run_test(
         self, SNPs1, G1, y, altset, iset, ichrm, iposrange, iperm=-1, varcomp_test=None
     ):
         """
         This function does the main work of the class, and also reads in the SNPs for the alternative model.
@@ -834,15 +833,15 @@
         )
 
         if varcomp_test is None or not self.cache_from_perm:
             if G1.shape[1] == 0:
                 logging.info("no SNPS in set " + setname)
                 result = None
                 return [result]
-            if sp.isnan(G1.sum()):
+            if np.isnan(G1.sum()):
                 raise Exception(
                     "found missing values in test SNPs that remain after intersection for "
                     + str(altset)
                 )
 
             result.setsize = SNPs1["snps"].shape[1]
 
@@ -882,15 +881,15 @@
         if varcomp_test is None or not self.cache_from_perm:
             # need to make this caching smarter for when background kernel changes in every test (e.g. interactions)
             if (self.permute is not None) or (iperm >= 0):
                 G1 = G1[permutationIndex]
 
             # if result.nexclude:
             #    logging.info(" (computing needed null info anew) ")
-            #    G0_to_use = self.__SNPs0#['data']['snps'][:,~i_exclude]/SP.sqrt(self.__SNPs0['data']['snps'][:,~i_exclude].shape[1])
+            #    G0_to_use = self.__SNPs0#['data']['snps'][:,~i_exclude]/np.sqrt(self.__SNPs0['data']['snps'][:,~i_exclude].shape[1])
             # else:
             #    G0_to_use=self.__G0
 
             if (
                 (str(self.test) != "lrt_up")
                 and (self.genphen is not None)
                 and (not self.genphen["once"])
@@ -992,15 +991,15 @@
 
         SNPs1b = altset2.read()  # second set
         SNPs1b["snps"] = util.standardize(SNPs1b["snps"])
 
         SNPs1 = dict(SNPs1a)
         SNPs1.update(SNPs1b)  # concatenate the SNP dictionaries
 
-        G1 = SNPs1["snps"] / sp.sqrt(SNPs1["snps"].shape[1])
+        G1 = SNPs1["snps"] / np.sqrt(SNPs1["snps"].shape[1])
         if G1.shape[1] == 0:
             raise Exception("no SNPs to test")
         result.setsize = SNPs1["snps"].shape[1]
 
         logging.info(" (" + str(result.setsize) + " SNPs)")
 
         if self.permute >= 0:
@@ -1033,15 +1032,15 @@
             result.nexclude = 0
 
         null_model_changed = result.nexclude > 0
 
         # need to make this caching smarter for when background kernel changes in every test (e.g. interactions)
         if null_model_changed:
             logging.info(" (computing needed null info anew) ")
-            G0_to_use = self.__SNPs0["data"]["snps"][:, ~i_exclude] / SP.sqrt(
+            G0_to_use = self.__SNPs0["data"]["snps"][:, ~i_exclude] / np.sqrt(
                 self.__SNPs0["data"]["snps"][:, ~i_exclude].shape[1]
             )  # excluded SNPs
             null_model = None
         else:  # use cached values
             G0_to_use = self.__G0
             null_model = self.__varcomp_test
             logging.info(" (using cached null info)")
@@ -1253,15 +1252,15 @@
         phenhead, phentail = os.path.split(self.phenofile)
         logging.info("Reading Pheno: " + phentail + "")
         pheno = loadPhen(filename=self.phenofile, missing="NaN")
         pheno["vals"] = pheno["vals"][
             :, self.mpheno - 1
         ]  # use -1 so compatible with C++ version
         # pheno['header']=pheno['header'][self.mpheno-1] #header is empty
-        goodind = sp.logical_not(sp.isnan(pheno["vals"]))
+        goodind = np.logical_not(np.isnan(pheno["vals"]))
         pheno["vals"] = pheno["vals"][goodind]
         pheno["iid"] = pheno["iid"][goodind, :]
 
         if self.genphen is not None:
             # for synthetic data generation--this is the background signal added to the phenotype
             if self.genphen["varBackNullFileGen"] is not None:
                 self.__varBackNullSnpsGen = readBED(self.genphen["varBackNullFileGen"])
@@ -1296,35 +1295,35 @@
                 pass
             else:
                 raise Exception("covarimp=" + self.covarimp + " not implemented")
 
         covar, pheno, indarr = self.intersect_data(covar, pheno)
         N = pheno["vals"].shape[0]
         if self.covarfile == None:
-            self.__X = sp.ones((N, 1))
+            self.__X = np.ones((N, 1))
         else:
             # check for covariates which are constant, as the lmm code crashes on these
             badind = utilx.indof_constfeatures(covar["vals"], axis=0)
             if len(badind) > 0:
                 raise Exception(
                     "found constant covariates with indexes: %s: please remove, or modify code here to do so"
                     % badind
                 )
-            self.__X = sp.hstack((sp.ones((N, 1)), covar["vals"]))
+            self.__X = np.hstack((np.ones((N, 1)), covar["vals"]))
         self.__y = pheno["vals"]
 
-        if not covar is None and sp.isnan(covar["vals"].sum()):
+        if not covar is None and np.isnan(covar["vals"].sum()):
             raise Exception(
                 "found missing values in covariates file that remain after intersection"
             )
-        if sp.isnan(self.__y.sum()):
+        if np.isnan(self.__y.sum()):
             raise Exception(
                 "found missing values in phenotype file that remain after intersection"
             )
-        # if hasattr(self,'__G0') and not self.__G0 is None and sp.isnan(self.__G0.sum())): raise Exception("found missing values in background SNPs that remain after intersection")
+        # if hasattr(self,'__G0') and not self.__G0 is None and np.isnan(self.__G0.sum())): raise Exception("found missing values in background SNPs that remain after intersection")
 
         # creating sets from set defn files. Looks at bed file to filter down the SNPs to only those present in the bed file
         (
             self.altset_list,
             self.altsetlist_filtbysnps,
         ) = self.create_altsetlist_filtbysnps(self.altset_list, self.alt_snpreader)
         if self.altset_list2 is not None:
@@ -1333,15 +1332,15 @@
                 self.__altsetlist2_filtbysnps,
             ) = self.create_altsetlist_filtbysnps(self.altset_list2, self.alt_snpreader)
 
         if self.npermabs is not None and self.nperm is not None:
             assert self.nperm is None, "cannot use both nperm and npermabs"
         if self.npermabs is not None:
             num_tests = len(self.altsetlist_filtbysnps)
-            self.nperm = int(sp.ceil(self.npermabs / num_tests))
+            self.nperm = int(np.ceil(self.npermabs / num_tests))
             logging.info(
                 "using npermabs=%i, found %i tests, so using %i permutations per test"
                 % (self.npermabs, num_tests, self.nperm)
             )
             self.npermabs = None
 
         logging.info("------------------------------------------------")
@@ -1397,15 +1396,15 @@
         logging.info("------------------------------------------------")
 
         logging.info("Creating null model... ")
         # cache whatever is needed for each case (sometimes likelihood, sometimes rotated items, sometimes nothing)
         t0 = time.time()
 
         # if self.filenull  is not None: #aka two-kernel
-        #    self.__G0 = self.__SNPs0['data']['snps']/sp.sqrt(self.__SNPs0['data']['snps'].shape[1])
+        #    self.__G0 = self.__SNPs0['data']['snps']/np.sqrt(self.__SNPs0['data']['snps'].shape[1])
         # else:
         #    self.__G0=None
 
         # for some models, this caches important and expensive information
         # as appropriate, gets re-computed in run_test()
         if (
             self.genphen is None
@@ -1424,36 +1423,36 @@
 
         t1 = time.time()
         logging.info("done. %.2f seconds elapsed" % (t1 - t0))
 
     def check_id_order(self, covar, pheno):
         ids_pheno = pheno["iid"]
         ids_SNPs = self.alt_snpreader.original_iids
-        if (len(ids_pheno) != len(ids_SNPs)) or (not sp.all(ids_pheno == ids_SNPs)):
+        if (len(ids_pheno) != len(ids_SNPs)) or (not np.all(ids_pheno == ids_SNPs)):
             return False
         if self.covarfile is not None:
             ids_X = covar["iid"]
-            if (len(ids_pheno) != len(ids_X)) or (not sp.all(ids_pheno == ids_X)):
+            if (len(ids_pheno) != len(ids_X)) or (not np.all(ids_pheno == ids_X)):
                 return False
         if self.filenull is not None:
             ids_nullSNPs = self.__SNPs0["original_iids"]
-            if not sp.all(ids_pheno == ids_nullSNPs):
+            if not np.all(ids_pheno == ids_nullSNPs):
                 return False
         if (
             hasattr(self, "__varBackNullSnpsGen")
             and self.__varBackNullSnpsGen is not None
         ):  # for synthetic data generation
             ids_SNPgen = self.__varBackNullSnpsGen["iid"]
-            if not sp.all(ids_pheno == ids_SNPgen):
+            if not np.all(ids_pheno == ids_SNPgen):
                 return False
         return True
 
     def intersect_data(self, covar, pheno):
         if self.check_id_order(covar, pheno):
-            indarr = SP.arange(pheno["iid"].shape[0])
+            indarr = np.arange(pheno["iid"].shape[0])
             logging.info(str(indarr.shape[0]) + " IDs match up across data sets")
         else:
             logging.info(
                 "IDs do not match up, so intersecting the data over individuals"
             )
             if self.filenull is not None:
                 nullsnpids = self.__SNPs0["original_iids"]
@@ -1486,30 +1485,30 @@
             )
             assert (
                 indarr.shape[0] > 0
             ), "no individuals remain after intersection, check that ids match in files"
             # sort the indexes so that SNPs ids in their original order (and
             # therefore we have to move things around in memory the least amount)
             # [indarr[:,3] holds the SNP order
-            sortind = sp.argsort(indarr[:, 3])
+            sortind = np.argsort(indarr[:, 3])
             indarr = indarr[sortind]
 
             pheno["iid"] = pheno["iid"][indarr[:, 0]]
             pheno["vals"] = pheno["vals"][indarr[:, 0]]
 
             self.alt_snpreader.ind_used = indarr[:, 1]
 
             if self.covarfile is not None:
                 covar["iid"] = covar["iid"][indarr[:, 2]]
                 covar["vals"] = covar["vals"][indarr[:, 2]]
 
             if self.filenull is not None:
                 # copy in memory to make later access faster (presumably?):
-                # self.__SNPs0['iid']=sp.copy(self.__SNPs0['iid'][indarr[:,3]])
-                # self.__SNPs0['snps']=sp.copy(self.__SNPs0['snps'][indarr[:,3]])
+                # self.__SNPs0['iid']=np.copy(self.__SNPs0['iid'][indarr[:,3]])
+                # self.__SNPs0['snps']=np.copy(self.__SNPs0['snps'][indarr[:,3]])
                 # self.__SNPs0['data']['iid']=self.__SNPs0['data']['iid'][indarr[:,3]]
                 if "data" in self.__SNPs0:
                     self.__SNPs0["data"]["iid"] = self.__SNPs0["data"]["iid"][
                         indarr[:, 3]
                     ]
                     self.__SNPs0["data"]["snps"] = self.__SNPs0["data"]["snps"][
                         indarr[:, 3]
```

### Comparing `fastlmm-0.6.7/fastlmm/association/FastLmmSetLOOC.py` & `fastlmm-0.6.8b1/fastlmm/association/FastLmmSetLOOC.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-from __future__ import print_function
 from fastlmm.association.FastLmmSet import *
 
 # from pysnptools.util.mapreduce1.distributable import *
 from pysnptools.util.mapreduce1.runner import *
 import os
 import sys
 import time
```

### Comparing `fastlmm-0.6.7/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf` & `fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe` & `fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/Fastlmm_autoselect/fastlmmc` & `fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/fastlmmc`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll` & `fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/LeaveOneChromosomeOut.py` & `fastlmm-0.6.8b1/fastlmm/association/LeaveOneChromosomeOut.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 
 """
 Created on 2014-03-11
 @author: Christian Widmer
 @summary: Module for performing GWAS
 """
 
-from __future__ import absolute_import
 import logging
 
 import numpy as np
-import scipy as sp
 import pandas as pd
 from scipy import stats
 import pylab
 
 import time
 
 import fastlmm.inference as fastlmm
 
-import fastlmm.util.util as util 
+import fastlmm.util.util as util
 from fastlmm.util.pickle_io import load, save
 from fastlmm.util.util import argintersect_left
 
 
 class LeaveOneChromosomeOut(object):
     """LeaveOneChromosomeOut cross validation iterator (based on sklearn).
 
@@ -49,44 +47,43 @@
     random_state : int or RandomState
             Pseudo number generator state used for random sampling.
 
     """
 
     def __init__(self, chr_names, indices=True, random_state=None):
 
-        #random_state = check_random_state(random_state)
+        # random_state = check_random_state(random_state)
 
         self.chr_names = np.array(chr_names)
         self.unique_chr_names = list(set(chr_names))
         self.unique_chr_names.sort()
 
         assert len(self.unique_chr_names) > 1
         self.n = len(self.chr_names)
         self.n_folds = len(self.unique_chr_names)
         self.indices = indices
         self.idxs = np.arange(self.n)
 
-
     def __iter__(self):
         if self.indices:
             ind = np.arange(self.n)
-        
+
         for chr_name in self.unique_chr_names:
-            
+
             test_index = self.chr_names == chr_name
             train_index = np.logical_not(test_index)
-            
+
             if self.indices:
                 train_index = ind[train_index]
                 test_index = ind[test_index]
-            
+
             yield train_index, test_index
 
     def __repr__(self):
-        return '%s.%s(n=%i, n_folds=%i)' % (
+        return "%s.%s(n=%i, n_folds=%i)" % (
             self.__class__.__module__,
             self.__class__.__name__,
             self.n,
             self.n_folds,
         )
 
     def __len__(self):
```

### Comparing `fastlmm-0.6.7/fastlmm/association/LocoGwas.py` & `fastlmm-0.6.8b1/fastlmm/association/LocoGwas.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import time
 import logging
 import os.path
 from unittest.mock import patch
 
 import numpy as np
-import scipy as sp
 import pandas as pd
 from scipy import stats
 
 import fastlmm.inference as fastlmm
 
 import fastlmm.util.util as util
 from fastlmm.util.pickle_io import load, save
```

### Comparing `fastlmm-0.6.7/fastlmm/association/PairResult.py` & `fastlmm-0.6.8b1/fastlmm/association/PairResult.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/PrecomputeLocoPcs.py` & `fastlmm-0.6.8b1/fastlmm/association/PrecomputeLocoPcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,33 @@
 # Copyright (C) 2014 Microsoft Research
 
 """
 Created on 2014-04-02
 @summary: Helper Module for precomputing principal components for Leave one Chromosme out GWAS
 """
 
-from __future__ import absolute_import
-from __future__ import print_function
 import logging
 import numpy as np
-import scipy as sp
 import pandas as pd
 from scipy import stats
 import pylab
 import fastlmm.pyplink.plink as plink
 import pysnptools.util.pheno as pstpheno
 import pysnptools.util as pstutil
-import fastlmm.util.util as util 
+import fastlmm.util.util as util
 import fastlmm.util.standardizer as stdizer
 from fastlmm.util.pickle_io import load, save
 import os.path
 from sklearn.decomposition import PCA
 
 import fastlmm.association.LeaveOneChromosomeOut as LeaveOneChromosomeOut
 import fastlmm.pyplink.snpset.AllSnps as AllSnps
-from six.moves import range
 
-def load_intersect(snp_reader, pheno_fn_or_none,snp_set=AllSnps()):
+
+def load_intersect(snp_reader, pheno_fn_or_none, snp_set=AllSnps()):
     """
     load SNPs and phenotype, intersect ids
     ----------------------------------------------------------------------
     Input:
     bed_reader : SnpReader object (e.g. BedReader)
     pheno_fn   : str, file name of phenotype file, defa
     ----------------------------------------------------------------------
@@ -40,128 +37,138 @@
     G : numpy array containing SNP data
     y : numpy (1d) containing phenotype
     ----------------------------------------------------------------------
     """
 
     standardizer = stdizer.Unit()
 
-    geno = snp_reader.read(order='C',snp_set=snp_set)
-    G = geno['snps']
+    geno = snp_reader.read(order="C", snp_set=snp_set)
+    G = geno["snps"]
     G = standardizer.standardize(G)
 
-    snp_names = geno['rs']
-    chr_ids = geno['pos'][:,0]
+    snp_names = geno["rs"]
+    chr_ids = geno["pos"][:, 0]
 
     if not pheno_fn_or_none is None:
 
         # load phenotype
         pheno = pstpheno.loadOnePhen(pheno_fn_or_none, 0)
-        y = pheno['vals'][:,0]
+        y = pheno["vals"][:, 0]
 
         # load covariates and intersect ids
         import warnings
-        warnings.warn("This intersect_ids is deprecated. Pysnptools includes newer versions of intersect_ids", DeprecationWarning)
-        indarr = util.intersect_ids([pheno['iid'], snp_reader.original_iids])
-    
-        #print "warning: random phen"
-        #y = np.random.random_sample(len(y)) 
-
 
-        if not (indarr[:,0] == indarr[:,1]).all():
-            assert False, "ERROR: this code assumes the same order for snp and phen file"
+        warnings.warn(
+            "This intersect_ids is deprecated. Pysnptools includes newer versions of intersect_ids",
+            DeprecationWarning,
+        )
+        indarr = util.intersect_ids([pheno["iid"], snp_reader.original_iids])
+
+        # print "warning: random phen"
+        # y = np.random.random_sample(len(y))
+
+        if not (indarr[:, 0] == indarr[:, 1]).all():
+            assert (
+                False
+            ), "ERROR: this code assumes the same order for snp and phen file"
 
             print("reindexing")
-            y = y[indarr[:,0]]
-            G = G[indarr[:,1]]
+            y = y[indarr[:, 0]]
+            G = G[indarr[:, 1]]
     else:
         y = None
 
-
     return G, y, snp_names, chr_ids
 
 
-
-class PrecomputeLocoPcs(object) : #implements IDistributable
-    '''
+class PrecomputeLocoPcs(object):  # implements IDistributable
+    """
     Find the PCs of a snp data set and phenotype
-    '''
+    """
+
     def __init__(self, chrom_count, snp_reader, pheno_fn, cache_prefix):
         self.snp_reader = snp_reader
         self.pheno_fn = pheno_fn
         self.cache_prefix = cache_prefix
         self.chrom_count = chrom_count
 
- #start of IDistributable interface--------------------------------------
+    # start of IDistributable interface--------------------------------------
     @property
     def work_count(self):
         return self.chrom_count
 
     def work_sequence(self):
 
-        G, y, snp_name,chr_ids = load_intersect(self.snp_reader, self.pheno_fn)
+        G, y, snp_name, chr_ids = load_intersect(self.snp_reader, self.pheno_fn)
         loco = LeaveOneChromosomeOut.LeaveOneChromosomeOut(chr_ids, indices=True)
-        if len(loco) is not self.chrom_count :  raise Exception("The snp reader has {0} chromosome, not {1} as specified".format(len(loco),self.chrom_count))
+        if len(loco) is not self.chrom_count:
+            raise Exception(
+                "The snp reader has {0} chromosome, not {1} as specified".format(
+                    len(loco), self.chrom_count
+                )
+            )
 
-    
         for i, (train_snp_idx, _) in enumerate(loco):
-            yield lambda i=i, train_snp_idx=train_snp_idx,G=G: self.dowork(i,train_snp_idx,G)  # the 'i=i',etc is need to get around a strangeness in Python
+            yield lambda i=i, train_snp_idx=train_snp_idx, G=G: self.dowork(
+                i, train_snp_idx, G
+            )  # the 'i=i',etc is need to get around a strangeness in Python
 
     def reduce(self, result_sequence):
-        '''
-        '''
+        """ """
         for i, pcs in result_sequence:
             out_fn = self.create_out_fn(self.cache_prefix, i)
             pstutil.create_directory_if_necessary(out_fn)
             save(out_fn, pcs)
         return None
 
-    #optional override -- the str name of the instance is used by the cluster as the job name
+    # optional override -- the str name of the instance is used by the cluster as the job name
     def __str__(self):
-        return "{0}({1},'{2}','{3}')".format(self.__class__.__name__, self.snp_reader, self.pheno_fn, self.cache_prefix)
- #end of IDistributable interface---------------------------------------
+        return "{0}({1},'{2}','{3}')".format(
+            self.__class__.__name__, self.snp_reader, self.pheno_fn, self.cache_prefix
+        )
+
+    # end of IDistributable interface---------------------------------------
 
     def is_run_needed(self):
         # don't recompute if all files exist
         for i in range(self.chrom_count):
             pc_fn = self.create_out_fn(self.cache_prefix, i)
             if not os.path.isfile(pc_fn):
                 return True
         return False
 
     @staticmethod
     def create_out_fn(cache_prefix, i):
-        #TODO: throw exception if it's top level
+        # TODO: throw exception if it's top level
         out_fn = "%s_%04d.pickle.bzip" % (cache_prefix, i)
         return out_fn
 
     def dowork(self, i, train_snp_idx, G):
-        '''
+        """
         This can return anything, but note that it will be binary serialized (pickleable), and you don't want to have more than is required there for reduce
-        '''
+        """
         # fast indexing (needs to be C-order)
         assert np.isfortran(G) == False
         G_train = G.take(train_snp_idx, axis=1)
-        
+
         pca = PCA()
         pcs = pca.fit_transform(G_train)
         # n_ind, n_pcs
 
         return i, pcs
 
-
     #!! would be nice of this was optional and if not given the OS was asked
     # required by IDistributable
     @property
     def tempdirectory(self):
         return ".work_directory." + self.cache_prefix
 
-
     def copyinputs(self, copier):
         copier.input(self.pheno_fn)
         copier.input(self.snp_reader)
 
-    #Note that the files created are not automatically copied. Instead,
+    # Note that the files created are not automatically copied. Instead,
     # whenever we want another file to be created, a second change must be made here so that it will be copied.
-    def copyoutputs(self,copier):
+    def copyoutputs(self, copier):
         for i in range(self.chrom_count):
             out_fn = self.create_out_fn(self.cache_prefix, i)
             copier.output(out_fn)
```

### Comparing `fastlmm-0.6.7/fastlmm/association/Result.py` & `fastlmm-0.6.8b1/fastlmm/association/Result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from __future__ import absolute_import
 import logging
 
+
 class Result:
-    '''
+    """
     'lik0'          : null likelihood
                         'nLL'       : negative log-likelihood
                         'sigma2'    : the model variance sigma^2
                         'beta'      : [D*1] array of fixed effects weights beta
                         'h2'        : mixture weight between Covariance and noise
                         'REML'      : True: REML was computed, False: ML was computed
                         'a2'        : mixture weight between K0 and K1
@@ -15,65 +15,63 @@
                         'sigma2'    : the model variance sigma^2
                         'beta'      : [D*1] array of fixed effects weights beta
                         'h2'        : mixture weight between Covariance and noise
                         'REML'      : True: REML was computed, False: ML was computed
                         'a2'        : mixture weight between K0 and K1
     'nexclude'      : array of the number of excluded snps from null
     'test'          : "lrt", "sc_davies", sc_..."
-    '''
-
+    """
 
-    def __init__(self,setname,iset,iperm,ichrm,iposrange):
+    def __init__(self, setname, iset, iperm, ichrm, iposrange):
         self.setname = setname
         self.iset = iset
         self.iperm = iperm
         self.ichrm = ichrm
         self.iposrange = iposrange
 
     # computing observed lrt statistics and a2 parameters
     @property
     def stat(self):
-        return self.test['stat']
-        #return 2 * (self.lik0['nLL'] - self.lik1['nLL'])
+        return self.test["stat"]
+        # return 2 * (self.lik0['nLL'] - self.lik1['nLL'])
 
     @property
     def a2(self):
-        return self.test['lik1']['a2']
+        return self.test["lik1"]["a2"]
 
     @property
     def h2(self):
         try:
-            return self.test['lik1']['h2'][0]
+            return self.test["lik1"]["h2"][0]
         except:
             logging.info("found a scalar h2")
-            return self.test['lik1']['h2']
+            return self.test["lik1"]["h2"]
 
     @property
     def h2_1(self):
         try:
-            return self.test['lik1']['h2_1'][0]
+            return self.test["lik1"]["h2_1"][0]
         except:
             logging.info("found a scalar h2_1")
-            return self.test['lik1']['h2_1']
-
+            return self.test["lik1"]["h2_1"]
 
     @property
     def type(self):
-        return self.test['type']
+        return self.test["type"]
 
     @property
     def pv(self):
-        return self.test['pv']
-    
+        return self.test["pv"]
+
     @property
     def alteqnull(self):
-        if 'alteqnull' in self.test:
-            return self.test['alteqnull']
+        if "alteqnull" in self.test:
+            return self.test["alteqnull"]
         return None
 
     @property
     def lik0Details(self):
-        return self.test['lik0']
+        return self.test["lik0"]
 
     @property
     def lik1Details(self):
-        return self.test['lik1']
+        return self.test["lik1"]
```

### Comparing `fastlmm-0.6.7/fastlmm/association/__init__.py` & `fastlmm-0.6.8b1/fastlmm/association/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/_matchscript.py` & `fastlmm-0.6.8b1/fastlmm/association/_matchscript.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-#import os
-#import subprocess, sys, os.path
-#import numpy as SP
+# import os
+# import subprocess, sys, os.path
+# import numpy as np
 
-#def should_output(bigrow, littlefields):
+# def should_output(bigrow, littlefields):
 #    bigrs = bigrow[1]
 #    bigchr = bigrow[0]
 #    bigdist = float(bigrow[2])
 #    for littlerow in littlefields:
 #        littlers = littlerow[1]
 #        if bigrs == littlers:
 #            return False
@@ -14,31 +14,26 @@
 #        if bigchr == littlechr:
 #            littledist = float(littlerow[2])
 #            if abs(bigdist - littledist) < 2.0:
 #                return False
 #    return True
 
 
-
-
-#if __name__ == "__main__":
+# if __name__ == "__main__":
 #    assert len(sys.argv) == 4, "expect 3 arguments"
 #    bigfile = sys.argv[1]
 #    littlefile = sys.argv[2]
 #    outfile = sys.argv[3]
 
 #    logging.info("Loading bim file {0}\n".format(bigfile))
-#    bigfields = SP.loadtxt(bigfile,delimiter = '\t',dtype = 'str',usecols = (0,1,2,3),comments=None)
+#    bigfields = np.loadtxt(bigfile,delimiter = '\t',dtype = 'str',usecols = (0,1,2,3),comments=None)
 
 #    logging.info("Loading bim file {0}\n".format(littlefile))
-#    littlefields = SP.loadtxt(littlefile,delimiter = '\t',dtype = 'str',usecols = (0,1,2,3),comments=None)
+#    littlefields = np.loadtxt(littlefile,delimiter = '\t',dtype = 'str',usecols = (0,1,2,3),comments=None)
 
 #    logging.info("comparing\n")
 #    import fastlmm.util.util as ut
 #    ut.create_directory_if_necessary(outfile)
 #    with open(outfile,"w") as out_fp:
 #        for bigrow in bigfields:
 #            if should_output(bigrow,littlefields):
 #                out_fp.write(bigrow[1] + "\n")
-
-
-
```

### Comparing `fastlmm-0.6.7/fastlmm/association/_pipelines.py` & `fastlmm-0.6.8b1/fastlmm/association/_pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import fastlmm.util.preprocess as util
 
 
 def TESTBEFOREUSING_score_testfilesFromDir(
     phenofile,
     base0,
     pedfilesalt,
@@ -45,58 +43,58 @@
                   log-likelihoods of the alternative models,
     'nexclude'  : [Nalt] array of numbers of SNPs excluded,
     'filenames' : [Nalt] array of basefilenames
     --------------------------------------------------------------------------
     """
     pheno = pstpheno.loadPhen(filename=phenofile, missing="-9", pheno=None)
     if covarfile is None:
-        X = SP.ones((pheno["vals"].shape[0], 1))
+        X = np.ones((pheno["vals"].shape[0], 1))
     else:
         covar = pstpheno.loadPhen(filename=covarfile, missing="-9", pheno=None)
-        X = SP.hstack((SP.ones((pheno["vals"].shape[0], 1)), covar["vals"]))
+        X = np.hstack((np.ones((pheno["vals"].shape[0], 1)), covar["vals"]))
     if filetype == "PED":
         SNPs0 = plink.readPED(
             basefilename=base0, delimiter=" ", missing="0", standardize=True, pheno=None
         )
     elif filetype == "BED":
         SNPs0 = plink.readBED(basefilename=base0)
         SNPs0["snps"] = util.standardize(SNPs0["snps"])
 
     y = pheno["vals"][:, ipheno]
-    G0 = SNPs0["snps"] / SP.sqrt(SNPs0["snps"].shape[1])
+    G0 = SNPs0["snps"] / np.sqrt(SNPs0["snps"].shape[1])
 
     # build the null model
-    test2K = scoretest(Y=y[:, SP.newaxis], X=X, K=None, G=G0)
+    test2K = scoretest(Y=y[:, np.newaxis], X=X, K=None, G=G0)
 
-    squaredform = SP.zeros(len(pedfilesalt))
-    expectationsqform = SP.zeros(len(pedfilesalt))
-    varsqform = SP.zeros(len(pedfilesalt))
-    squaredform2K = SP.zeros(len(pedfilesalt))
-    expectationsqform2K = SP.zeros(len(pedfilesalt))
-    varsqform2K = SP.zeros(len(pedfilesalt))
-    nexclude = SP.zeros(len(pedfilesalt))
-    include = SP.zeros(len(pedfilesalt))
-    Pv = SP.zeros(len(pedfilesalt))
-    Pv2K = SP.zeros(len(pedfilesalt))
+    squaredform = np.zeros(len(pedfilesalt))
+    expectationsqform = np.zeros(len(pedfilesalt))
+    varsqform = np.zeros(len(pedfilesalt))
+    squaredform2K = np.zeros(len(pedfilesalt))
+    expectationsqform2K = np.zeros(len(pedfilesalt))
+    varsqform2K = np.zeros(len(pedfilesalt))
+    nexclude = np.zeros(len(pedfilesalt))
+    include = np.zeros(len(pedfilesalt))
+    Pv = np.zeros(len(pedfilesalt))
+    Pv2K = np.zeros(len(pedfilesalt))
 
     for i, base1 in enumerate(pedfilesalt):  # iterate over all ped files
         SNPs1 = plink.readPED(
             basefilename=base1, delimiter=" ", missing="0", standardize=True, pheno=None
         )
         if mindist >= 0:
             i_exclude = excludeinds(
                 SNPs0["pos"], SNPs1["pos"], mindist=mindist, idist=idist
             )
             nexclude[i] = i_exclude.sum()
         else:
             nexclude[i] = 0
-        G1 = SNPs1["snps"] / SP.sqrt(SNPs1["snps"].shape[1])
+        G1 = SNPs1["snps"] / np.sqrt(SNPs1["snps"].shape[1])
 
         if nexclude[i] > 0:
-            test2Ke = scoretest(Y=y[:, SP.newaxis], X=X, K=None, G=G0[:, ~i_exclude])
+            test2Ke = scoretest(Y=y[:, np.newaxis], X=X, K=None, G=G0[:, ~i_exclude])
             squaredform2K[i], expectationsqform2K[i], varsqform2K[i] = test2Ke.score(
                 G=G1
             )
         else:
             squaredform2K[i], expectationsqform2K[i], varsqform2K[i] = test2K.score(
                 G=G1
             )
@@ -109,30 +107,30 @@
             squaredform2K[i], expectationsqform2K[i], varsqform2K[i]
         )
         Pv[i], dofchi2, scalechi2 = pv_mom(
             squaredform[i], expectationsqform[i], varsqform[i]
         )
 
     ret = {
-        "filenames": SP.array(pedfilesalt, dtype=str),
+        "filenames": np.array(pedfilesalt, dtype=str),
         "squaredform": squaredform,
         "expectationsqform": expectationsqform,
         "varsqform": varsqform,
         "P": Pv,
         "squaredform2K": squaredform2K,
         "expectationsqform2K": expectationsqform2K,
         "varsqform2K": varsqform2K,
         "nexclude": nexclude,
         "P2K": Pv2K,
     }
     if outfile is not None:
         # TODO
         print("implement me!")
-        # header = SP.array(['PV_5050','neg_log_lik_0','neg_loglik_alt','n_snps_excluded','filename_alt'])
-        # data = SP.concatenate(())
+        # header = np.array(['PV_5050','neg_log_lik_0','neg_loglik_alt','n_snps_excluded','filename_alt'])
+        # data = np.concatenate(())
     return ret
 
 
 def lrt_testfilesFromDir(
     phenofile,
     base0,
     pedfilesalt,
@@ -174,66 +172,66 @@
                   log-likelihoods of the alternative models,
     'nexclude'  : [Nalt] array of numbers of SNPs excluded,
     'filenames' : [Nalt] array of basefilenames
     --------------------------------------------------------------------------
     """
     pheno = pstpheno.loadPhen(filename=phenofile, missing="-9", pheno=None)
     if covarfile is None:
-        X = SP.ones((pheno["vals"].shape[0], 1))
+        X = np.ones((pheno["vals"].shape[0], 1))
     else:
         covar = pstpheno.loadPhen(filename=covarfile, missing="-9", pheno=None)
-        X = SP.hstack((SP.ones((pheno["vals"].shape[0], 1)), covar["vals"]))
+        X = np.hstack((np.ones((pheno["vals"].shape[0], 1)), covar["vals"]))
     if filetype == "PED":
         SNPs0 = plink.readPED(
             basefilename=base0, delimiter=" ", missing="0", standardize=True, pheno=None
         )
     elif filetype == "BED":
         SNPs0 = plink.readBED()
     y = pheno["vals"][:, ipheno]
-    G0 = SNPs0["snps"] / SP.sqrt(SNPs0["snps"].shape[1])
+    G0 = SNPs0["snps"] / np.sqrt(SNPs0["snps"].shape[1])
 
     # build the null model
     a0 = fastlmm.getLMM()
     a0.setG(G0)
     a0.setX(X)
     a0.sety(y)
     lik0_default = (
         a0.findH2()
     )  # The null model only has a single kernel and only needs to find h2
-    lik0 = SP.zeros(len(pedfilesalt), dtype="object")
-    lik1 = SP.zeros(len(pedfilesalt), dtype="object")
-    lrt = SP.zeros(len(pedfilesalt))
-    pv = SP.zeros(len(pedfilesalt))
-    nexclude = SP.zeros(len(pedfilesalt))
+    lik0 = np.zeros(len(pedfilesalt), dtype="object")
+    lik1 = np.zeros(len(pedfilesalt), dtype="object")
+    lrt = np.zeros(len(pedfilesalt))
+    pv = np.zeros(len(pedfilesalt))
+    nexclude = np.zeros(len(pedfilesalt))
     for i, base1 in enuemrate(pedfilesalt):  # iterate over all ped files
         SNPs1 = plink.readPED(
             basefilename=base1, delimiter=" ", missing="0", standardize=True, pheno=None
         )
         i_exclude = excludeinds(
             SNPs0["pos"], SNPs1["pos"], mindist=mindist, idist=idist
         )
         nexclude[i] = i_exclude.sum()
-        G1 = SNPs1["snps"] / SP.sqrt(SNPs1["snps"].shape[1])
+        G1 = SNPs1["snps"] / np.sqrt(SNPs1["snps"].shape[1])
         if nexclude[i]:  # recompute the null likelihood
-            G0_excluded = SNPs0["snps"][:, ~i_exclude] / SP.sqrt(
+            G0_excluded = SNPs0["snps"][:, ~i_exclude] / np.sqrt(
                 SNPs0["snps"][:, ~i_exclude].shape[1]
             )
             [pv[i], lik0[i], lik1[i]] = twokerneltest(
                 G0=G0_excluded, G1=G1, y=y, covar=X, appendbias=False, lik0=None
             )
         else:  # use precomputed null likelihood
             [pv[i], lik0[i], lik1[i]] = twokerneltest(
                 G0=G0, G1=G1, y=y, covar=X, appendbias=False, lik0=lik0_default
             )
     ret = {
         "pv": pv,
         "lik0": lik0,
         "lik1": lik1,
         "nexclude": nexclude,
-        "filenames": SP.array(pedfilesalt, dtype=str),
+        "filenames": np.array(pedfilesalt, dtype=str),
     }
     if outfile is not None:
         # TODO
         print("implement me!")
-        # header = SP.array(['PV_5050','neg_log_lik_0','neg_loglik_alt','n_snps_excluded','filename_alt'])
-        # data = SP.concatenate(())
+        # header = np.array(['PV_5050','neg_log_lik_0','neg_loglik_alt','n_snps_excluded','filename_alt'])
+        # data = np.concatenate(())
     return ret
```

### Comparing `fastlmm-0.6.7/fastlmm/association/altset_list/__init__.py` & `fastlmm-0.6.8b1/fastlmm/association/altset_list/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/altset_list/consecutive.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/Consecutive.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,72 @@
-from __future__ import absolute_import
 import numpy as np
 import subprocess, sys, os.path
 from itertools import *
+from fastlmm.pyplink.snpset import *
 import math
-from six.moves import range
+
 
 class Consecutive(object):  # implements ISnpSetList
     """
-    The sets should be every consecutive set of SNPs within a 2cM window of each user 
+    The sets should be every consecutive set of SNPs within a 2cM window of each user
     (distance in cM is in the 3rd column of the bim file).  As for the name of the set,
     please make it <position-of-first-snp>@<position-of-middle-snp>@<position-of-last-snp>.
     For 'middle' please break a tie to the first SNP.
     """
 
-    def __init__(self, bimFileName,cMWindow):
+    def __init__(self, bimFileName, cMWindow):
         self.BimFileName = bimFileName
         self.CMWindow = cMWindow
 
     def addbed(self, bed):
-        return _ConsecutivePlusBed(self,bed)
+        return ConsecutivePlusBed(self, bed)
 
     def copyinputs(self, copier):
         copier.input(self.BimFileName)
 
-    #would be nicer if these used generic pretty printer
+    # would be nicer if these used generic pretty printer
     def __repr__(self):
-        return "Consecutive(bimFileName={0},bimFileName={1})".format(self.BimFileName,self.CMWindow)
+        return "Consecutive(bimFileName={0},bimFileName={1})".format(
+            self.BimFileName, self.CMWindow
+        )
 
 
-        
-class _ConsecutivePlusBed(object): # implements ISnpSetListPlusBed
+class ConsecutivePlusBed(object):  # implements ISnpSetListPlusBed
     def __init__(self, spec, bed):
         self.spec = spec
         self.bed = bed
         import pandas as pd
-        bimfields = pd.read_csv(self.spec.BimFileName,delimiter = '\t',usecols = (0,1,2,3),header=None,index_col=False)
+
+        bimfields = pd.read_csv(
+            self.spec.BimFileName,
+            delimiter="\s",
+            usecols=(0, 1, 2, 3),
+            header=None,
+            index_col=False,
+            engine="python",
+        )
         self.chrom = bimfields[0]
-        self.sid = bimfields[1]
+        self.rs = bimfields[1]
         self.cm = bimfields[2]
 
-
     def __iter__(self):
-        startIndex=-1
-        endIndex=0 #one too far
-        while(True):
-            startIndex+=1
-            if startIndex >= len(self.sid):
+        startIndex = -1
+        endIndex = 0  # one too far
+        while True:
+            startIndex += 1
+            if startIndex >= len(self.rs):
                 return
-            while endIndex < len(self.sid) and self.chrom[startIndex] == self.chrom[endIndex] and  self.cm[endIndex] - self.cm[startIndex] <= self.spec.CMWindow:
-                endIndex+=1
-            lastIndex = endIndex - 1;
-            midIndex = math.floor((startIndex+lastIndex)/2.0)
-            name = "{0}@{1}@{2}".format(startIndex,midIndex,lastIndex)
+            while (
+                endIndex < len(self.rs)
+                and self.chrom[startIndex] == self.chrom[endIndex]
+                and self.cm[endIndex] - self.cm[startIndex] <= self.spec.CMWindow
+            ):
+                endIndex += 1
+            lastIndex = endIndex - 1
+            midIndex = math.floor((startIndex + lastIndex) / 2.0)
+            name = "{0}@{1}@{2}".format(startIndex, midIndex, lastIndex)
 
-            snpList=self.sid[list(range(startIndex,endIndex))]
-            yield _SnpAndSetNamePlusBed(name,snpList,self.bed)
+            snpList = self.rs[list(range(startIndex, endIndex))]
+            yield SnpAndSetNamePlusBed(name, snpList, self.bed)
 
     def __len__(self):
-        return len(self.sid)
+        return len(self.rs)
```

### Comparing `fastlmm-0.6.7/fastlmm/association/altset_list/minmaxsetsize.py` & `fastlmm-0.6.8b1/fastlmm/association/altset_list/minmaxsetsize.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/altset_list/snpandsetnamecollection.py` & `fastlmm-0.6.8b1/fastlmm/association/altset_list/snpandsetnamecollection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,66 @@
-from __future__ import absolute_import
 import numpy as np
 import subprocess, sys, os.path
 from itertools import *
 import logging
-import six
+
 
 class SnpAndSetNameCollection(object):  # implements ISnpSetList
-    '''
+    """
     Specifies a list of snp sets via a file that has columns 'snp' and 'group'.
     See the Bed class's 'read' method of examples of its use.
     See __init__.py for specification of interface it implements.
-    '''
+    """
+
     def __init__(self, filename):
         self.filename = filename
         logging.info("Reading {0}".format(filename))
         import pandas as pd
-        snp_and_setname_sequence = pd.read_csv(filename,delimiter = '\t',index_col=False)
+
+        snp_and_setname_sequence = pd.read_csv(
+            filename, delimiter="\t", index_col=False
+        )
 
         from collections import defaultdict
+
         setname_to_sid = defaultdict(list)
-        for snp,gene in snp_and_setname_sequence.itertuples(index=False):
+        for snp, gene in snp_and_setname_sequence.itertuples(index=False):
             setname_to_sid[gene].append(snp)
-        self.bigToSmall = sorted(setname_to_sid.items(), key = lambda gene_sid:-len(gene_sid[1]))
+        self.bigToSmall = sorted(
+            setname_to_sid.items(), key=lambda gene_sid: -len(gene_sid[1])
+        )
 
     def addbed(self, bed):
-        return _SnpAndSetNameCollectionPlusBed(self,bed)
+        return _SnpAndSetNameCollectionPlusBed(self, bed)
 
     def copyinputs(self, copier):
         copier.input(self.filename)
 
-    #would be nicer if these used generic pretty printer
+    # would be nicer if these used generic pretty printer
     def __repr__(self):
         return "SnpAndSetNameCollection(filename={0})".format(self.filename)
 
     def __iter__(self):
-        for gene,sid in self.bigToSmall:
-            yield gene,sid
+        for gene, sid in self.bigToSmall:
+            yield gene, sid
 
 
-class _SnpAndSetNameCollectionPlusBed(object): # implements ISnpSetListPlusBed
-    '''
+class _SnpAndSetNameCollectionPlusBed(object):  # implements ISnpSetListPlusBed
+    """
     The SnpAndSetNameCollection with the addition of BED information.
-    '''
+    """
+
     def __init__(self, spec, bed):
         self.spec = spec
         self.bed = bed
 
     def __len__(self):
         return len(self.spec.bigToSmall)
 
     def __iter__(self):
         for gene, sid in self.spec.bigToSmall:
-            if len(set(sid)) != len(sid) : raise Exception("Some snps in gene {0} are listed more than once".format(gene))
+            if len(set(sid)) != len(sid):
+                raise Exception(
+                    "Some snps in gene {0} are listed more than once".format(gene)
+                )
             sid_index = self.bed.sid_to_index(sid)
-            yield gene, self.bed[:,sid_index]
+            yield gene, self.bed[:, sid_index]
```

### Comparing `fastlmm-0.6.7/fastlmm/association/altset_list/subset.py` & `fastlmm-0.6.8b1/fastlmm/association/altset_list/subset.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/epistasis.py` & `fastlmm-0.6.8b1/fastlmm/association/epistasis.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/gwas.py` & `fastlmm-0.6.8b1/fastlmm/association/gwas.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # original file at https://github.com/fastlmm/FaST-LMM
 
 # modified 2015 by Christoph Lippert
 
-from __future__ import absolute_import
-from __future__ import print_function
 import numpy as np
 import numpy.linalg as la
 import scipy.optimize as opt
 import scipy.stats as st
 import scipy.special as ss
 import pandas as pd
 from fastlmm.util.mingrid import *
@@ -35,15 +33,14 @@
 import pysnptools.standardizer
 import pysnptools
 import pysnptools.util
 import pysnptools.util.pheno
 import time
 import fastlmm.inference.lmm_cov as lmm_cov
 import glob
-from six.moves import range
 
 
 def create_dir(filename, is_dir=True):
     if is_dir:
         dirname = filename
     else:
         dirname = os.path.dirname(filename)
```

### Comparing `fastlmm-0.6.7/fastlmm/association/gwas_eval.py` & `fastlmm-0.6.8b1/fastlmm/association/gwas_eval.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,110 +5,108 @@
 
 """
 Created on 2014-04-07
 @author: Christian Widmer
 @summary: Module containing helper function to evaluate quality of GWAS
 """
 
-from __future__ import absolute_import
-from __future__ import print_function
 import time
 import os.path
 
 import numpy as np
-import scipy as sp
 from scipy import stats
 
 from fastlmm.util.pickle_io import load
 from fastlmm.util.util import excludeinds
 
 
-
 def estimate_lambda(pv):
     """estimate lambda form a set of PV"""
-    LOD2 = sp.median(stats.chi2.isf(pv,1))
-    L = (LOD2/0.456)
-    return (L)
+    LOD2 = np.median(stats.chi2.isf(pv, 1))
+    L = LOD2 / 0.456
+    return L
 
 
 def cut_snps_close_to_causals(p_values, pos, causal_idx, mindist, plot=False):
 
     i_causal_all = np.zeros(len(p_values), dtype=bool)
     i_causal_all[causal_idx] = True
-        
+
     # cut out snps in LD to causal snps
     pos_all = np.array(pos)
     pos_causal = np.array(pos)[causal_idx]
 
     close_to_causals_mask = excludeinds(pos_all, pos_causal, mindist=mindist, idist=2)
-    
+
     # keep causals and far away snps
     i_keepers = np.bitwise_or(i_causal_all, ~close_to_causals_mask)
-        
-    print(("keeping %i/%i SNPs (mindist=%f)" % (sum(i_keepers), len(i_keepers), mindist)))
+
+    print(
+        ("keeping %i/%i SNPs (mindist=%f)" % (sum(i_keepers), len(i_keepers), mindist))
+    )
 
     pv = p_values[i_keepers]
-    #pv_lin = p_values_lin[i_keepers]
+    # pv_lin = p_values_lin[i_keepers]
     i_causal = i_causal_all[i_keepers]
 
     if plot:
         import pylab
-        pylab.plot(pos[i_keepers,2], pos[i_keepers,0], "+")
-        pylab.plot(pos[:,2], pos[:,0]+0.5, "+")
+
+        pylab.plot(pos[i_keepers, 2], pos[i_keepers, 0], "+")
+        pylab.plot(pos[:, 2], pos[:, 0] + 0.5, "+")
         pylab.show()
 
     return pv, i_causal
 
 
-
 def eval_gwas(pv, i_causal, out_fn=None, plot=False):
-    """
-    
-    """
+    """ """
 
     pv_thresholds = [1e-3, 5e-4, 1e-4, 5e-5, 1e-5, 5e-6, 1e-6, 5e-7, 1e-7, 5e-8, 1e-8]
 
     # compute lambda on all p-values?
-    #lambda_gc = estimate_lambda(p_values)
+    # lambda_gc = estimate_lambda(p_values)
     lambda_gc = estimate_lambda(pv)
-        
+
     n_causal = i_causal.sum()
 
-    #compute power and Type-1 error
+    # compute power and Type-1 error
     power = np.zeros_like(pv_thresholds)
     t1err = np.zeros_like(pv_thresholds)
     power_corr = np.zeros_like(pv_thresholds)
     t1err_corr = np.zeros_like(pv_thresholds)
-        
-    pvcorr = stats.chi2.sf(stats.chi2.isf(pv,1)/lambda_gc,1)
 
-    for i_t, t in enumerate(pv_thresholds):
-        #compute uncorrected power and T1
-        i_lower = pv<t
-        power[i_t] =  i_causal[i_lower].sum()/(1.0*(n_causal))
-        t1err[i_t] = (~i_causal[i_lower]).sum()/(1.0*(len(i_causal)-n_causal))
-
-        #compute GC corrected Power and T1
-        i_lower_corr = pvcorr<t
-        power_corr[i_t] =  i_causal[i_lower_corr].sum()/(1.0*(n_causal))
-        t1err_corr[i_t] = (~i_causal[i_lower_corr]).sum()/(1.0*(len(i_causal)-n_causal))
+    pvcorr = stats.chi2.sf(stats.chi2.isf(pv, 1) / lambda_gc, 1)
 
+    for i_t, t in enumerate(pv_thresholds):
+        # compute uncorrected power and T1
+        i_lower = pv < t
+        power[i_t] = i_causal[i_lower].sum() / (1.0 * (n_causal))
+        t1err[i_t] = (~i_causal[i_lower]).sum() / (1.0 * (len(i_causal) - n_causal))
+
+        # compute GC corrected Power and T1
+        i_lower_corr = pvcorr < t
+        power_corr[i_t] = i_causal[i_lower_corr].sum() / (1.0 * (n_causal))
+        t1err_corr[i_t] = (~i_causal[i_lower_corr]).sum() / (
+            1.0 * (len(i_causal) - n_causal)
+        )
 
     if plot == True:
         import pylab
+
         pylab.figure()
         pylab.title("lambda_gc=%f" % lambda_gc)
         pylab.plot(pv_thresholds, power, "-o")
         pylab.yscale("log")
         pylab.xscale("log")
         pylab.xlabel("pv threshold")
         pylab.ylabel("power")
         pylab.grid(True)
         pylab.plot(pv_thresholds, power_corr, "-o")
-            
+
         if not out_fn is None:
             pow_fn = out_fn.replace(".pickle", "_pow.pdf")
             pylab.savefig(pow_fn)
         else:
             pylab.show()
 
         pylab.figure()
@@ -116,167 +114,185 @@
         pylab.plot(pv_thresholds, t1err, "-o", label="t1err")
         pylab.plot(pv_thresholds, t1err_corr, "-o", label="t1err_gc")
         pylab.yscale("log")
         pylab.xscale("log")
         pylab.xlabel("pv threshold")
         pylab.ylabel("t1err")
         pylab.grid(True)
-          
+
         pylab.plot(pv_thresholds, pv_thresholds, "-", label="thres")
         pylab.legend(loc="upper left")
         if not out_fn is None:
             t1err_fn = out_fn.replace(".pickle", "_t1err.pdf")
             pylab.savefig(t1err_fn)
         else:
             pylab.show()
 
         # plot auROC
         if out_fn is None:
             roc_fn = None
         else:
             roc_fn = out_fn.replace(".pickle", "_roc.pdf")
-        plot_roc(i_causal, -pv, label='lambda_gc=%0.4f' % (lambda_gc), out_fn=roc_fn)
+        plot_roc(i_causal, -pv, label="lambda_gc=%0.4f" % (lambda_gc), out_fn=roc_fn)
 
         # plot auPRC
         if out_fn is None:
             prc_fn = None
         else:
             prc_fn = out_fn.replace(".pickle", "_prc.pdf")
-        plot_prc(i_causal, -pv, label='lambda_gc=%0.4f' % (lambda_gc), out_fn=prc_fn)
-
+        plot_prc(i_causal, -pv, label="lambda_gc=%0.4f" % (lambda_gc), out_fn=prc_fn)
 
     # wrap up metrics
     res = {}
     res["lambda"] = lambda_gc
     res["pv_thresholds"] = pv_thresholds
     res["power"] = power
     res["power_corr"] = power_corr
     res["t1err"] = t1err
     res["t1err_corr"] = t1err_corr
 
     return res
 
 
-
 ###############################################################
 # t1err
 ###############################################################
 
+
 def plot_t1err_noshow(pv, i_causal, label="", gc_correct=False):
     """
     False Positive Rate = FP / N = 1 - specificity
     """
     pv_thresholds, t1err = compute_t1err_data(pv, i_causal)
     draw_t1err_curve(pv_thresholds, t1err, label, len(pv), gc_correct=gc_correct)
 
 
 def compute_t1err_data(pv, i_causal):
     gc_correct = False
-    pv_thresholds = [1e-3, 5e-4, 1e-4, 5e-5, 1e-5, 5e-6, 1e-6] #, 5e-7, 1e-7, 5e-8, 1e-8]
-
-
+    pv_thresholds = [
+        1e-3,
+        5e-4,
+        1e-4,
+        5e-5,
+        1e-5,
+        5e-6,
+        1e-6,
+    ]  # , 5e-7, 1e-7, 5e-8, 1e-8]
 
     n_causal = i_causal.sum()
 
-    #compute power and Type-1 error
+    # compute power and Type-1 error
     t1err = np.zeros_like(pv_thresholds)
-    
+
     if gc_correct:
         t1err_corr = np.zeros_like(pv_thresholds)
         # compute lambda on all p-values?
-        lambda_gc = estimate_lambda(pv)        
-        pvcorr = stats.chi2.sf(stats.chi2.isf(pv,1)/lambda_gc,1)
+        lambda_gc = estimate_lambda(pv)
+        pvcorr = stats.chi2.sf(stats.chi2.isf(pv, 1) / lambda_gc, 1)
 
     for i_t, t in enumerate(pv_thresholds):
-        #compute uncorrected power and T1
-        i_lower = pv<t
-        t1err[i_t] = (~i_causal[i_lower]).sum()/(1.0*(len(i_causal)-n_causal))
+        # compute uncorrected power and T1
+        i_lower = pv < t
+        t1err[i_t] = (~i_causal[i_lower]).sum() / (1.0 * (len(i_causal) - n_causal))
 
-        #compute GC corrected Power and T1
+        # compute GC corrected Power and T1
         if gc_correct:
-            i_lower_corr = pvcorr<t
-            t1err_corr[i_t] = (~i_causal[i_lower_corr]).sum()/(1.0*(len(i_causal)-n_causal))
+            i_lower_corr = pvcorr < t
+            t1err_corr[i_t] = (~i_causal[i_lower_corr]).sum() / (
+                1.0 * (len(i_causal) - n_causal)
+            )
 
     return pv_thresholds, t1err
 
 
 def draw_t1err_curve(pv_thresholds, t1err, label, num_trials):
     import pylab
+
     pylab.plot(pv_thresholds, t1err, "-o", label=label)
     pylab.yscale("log")
     pylab.xscale("log")
-    pylab.xlabel(r"$\alpha$",fontsize="large")
-    pylab.ylabel("type I error",fontsize="large")
+    pylab.xlabel(r"$\alpha$", fontsize="large")
+    pylab.ylabel("type I error", fontsize="large")
     pylab.grid(True)
-    pylab.xlim([1e-6,1e-3])
-    pylab.ylim([1e-6,1e0])
+    pylab.xlim([1e-6, 1e-3])
+    pylab.ylim([1e-6, 1e0])
 
     rt = pv_thresholds[::-1]
 
     import scipy.stats as stats
-    lower = [max(1e-7,(stats.distributions.binom.ppf(0.025, num_trials, t)-1)/float(num_trials)) for t in rt]
-    upper = [stats.distributions.binom.ppf(0.975, num_trials, t)/float(num_trials) for t in rt]
-    pylab.fill_between(rt, lower, upper, alpha=0.7, facecolor='#DDDDDD')
-    pylab.plot(pv_thresholds, pv_thresholds, 'k--')
+
+    lower = [
+        max(
+            1e-7,
+            (stats.distributions.binom.ppf(0.025, num_trials, t) - 1)
+            / float(num_trials),
+        )
+        for t in rt
+    ]
+    upper = [
+        stats.distributions.binom.ppf(0.975, num_trials, t) / float(num_trials)
+        for t in rt
+    ]
+    pylab.fill_between(rt, lower, upper, alpha=0.7, facecolor="#DDDDDD")
+    pylab.plot(pv_thresholds, pv_thresholds, "k--")
     pylab.legend(loc="lower right")
 
 
 ###############################################################
 # Power
 ###############################################################
 
+
 def plot_power_noshow(pv, i_causal, label="", gc_correct=False):
     pv_thresholds, power = compute_power_data(pv, i_causal)
     draw_power_curve(pv_thresholds, power, label, gc_correct=gc_correct)
 
 
-
 def compute_power_data(pv, i_causal):
 
-
     pv_thresholds = [1e-3, 5e-4, 1e-4, 5e-5, 1e-5, 5e-6, 1e-6, 5e-7, 1e-7, 5e-8, 1e-8]
 
     n_causal = i_causal.sum()
     power = np.zeros(len(pv_thresholds), dtype=np.float)
 
-
     for i_t, t in enumerate(pv_thresholds):
-        #compute uncorrected power and T1
-
-        i_lower = pv<t
-        power[i_t] = i_causal[i_lower].sum()/(1.0*(n_causal))
+        # compute uncorrected power and T1
 
+        i_lower = pv < t
+        power[i_t] = i_causal[i_lower].sum() / (1.0 * (n_causal))
 
     return pv_thresholds, power
 
 
 def draw_power_curve(pv_thresholds, power, label):
     import pylab
-    pylab.plot(pv_thresholds, power, "-o", label=label)
 
+    pylab.plot(pv_thresholds, power, "-o", label=label)
 
     pylab.yscale("log")
     pylab.xscale("log")
-    pylab.xlabel(r'$\alpha$', fontsize="large")
+    pylab.xlabel(r"$\alpha$", fontsize="large")
     pylab.ylabel("power", fontsize="large")
     pylab.grid(True)
-    
+
     pylab.legend(loc="lower right")
-        
+
 
 ###############################################################
 # auROC
 ###############################################################
 
+
 def plot_roc(y, out, label="", out_fn=None):
     """
     show or save ROC curve
     """
 
     import pylab
+
     pylab.figure()
     plot_roc_noshow(y, out, label=label)
 
     if not out_fn is None:
         pylab.savefig(out_fn)
     else:
         pylab.show()
@@ -294,47 +310,54 @@
 def compute_roc_data(y, out):
     """
     compte relevant metrics for auROC
     """
 
     # plot auc
     from sklearn.metrics import roc_curve, auc
+
     fpr, tpr, thresholds = roc_curve(y, out)
     roc_auc = auc(fpr, tpr)
 
     return fpr, tpr, roc_auc
 
+
 def draw_roc_curve(fpr, tpr, roc_auc, label):
-    
+
     if len(fpr) > 1000:
-        sub_idx = [int(a) for a in np.linspace(0, len(fpr)-1, num=1000, endpoint=True)]
+        sub_idx = [
+            int(a) for a in np.linspace(0, len(fpr) - 1, num=1000, endpoint=True)
+        ]
         fpr, tpr = fpr[sub_idx], tpr[sub_idx]
 
     import pylab
-    pylab.plot(fpr, tpr, label='%s (area = %0.4f)' % (label, roc_auc))
-    pylab.plot([0, 1], [0, 1], 'k--')
+
+    pylab.plot(fpr, tpr, label="%s (area = %0.4f)" % (label, roc_auc))
+    pylab.plot([0, 1], [0, 1], "k--")
     pylab.xlim([0.0, 1.0])
     pylab.ylim([0.0, 1.0])
-    pylab.xlabel('False Positive Rate')
-    pylab.ylabel('True Positive Rate')
-    pylab.title('Receiver operating characteristic example')
+    pylab.xlabel("False Positive Rate")
+    pylab.ylabel("True Positive Rate")
+    pylab.title("Receiver operating characteristic example")
     pylab.grid(True)
     pylab.legend(loc="lower right")
 
 
 ###############################################################
 # auPRC
 ###############################################################
 
+
 def plot_prc(y, out, label="", out_fn=None):
     """
     plot precision recall plot
     """
 
     import pylab
+
     pylab.figure()
     plot_prc_noshow(y, out, label=label)
 
     if not out_fn is None:
         pylab.savefig(out_fn)
     else:
         pylab.show()
@@ -352,33 +375,35 @@
     precision, recall, thresholds = precision_recall_curve(y, out)
     area = auc(recall, precision)
 
     return precision, recall, area
 
 
 def draw_prc_curve(precision, recall, area, label):
- 
+
     import pylab
-    pylab.plot(recall, precision, label='%s (area = %0.4f)' % (label, area))
-    pylab.xlabel('Recall')
-    pylab.ylabel('Precision')
+
+    pylab.plot(recall, precision, label="%s (area = %0.4f)" % (label, area))
+    pylab.xlabel("Recall")
+    pylab.ylabel("Precision")
     pylab.ylim([0.0, 1.05])
     pylab.xlim([0.0, 1.0])
     pylab.grid(True)
     pylab.legend(loc="upper right")
 
 
 def merge_results(results_dir, fn_filter_list, mindist):
     """
     visualize gwas results based on results file names
     """
 
     files = [fn for fn in os.listdir(results_dir) if fn.endswith("pickle")]
 
     import pylab
+
     pylab.figure()
 
     for fn_idx, fn_filter in enumerate(fn_filter_list):
 
         method_files = [fn for fn in files if fn.find(fn_filter) != -1]
 
         p_values = []
@@ -386,57 +411,62 @@
         i_causal = []
 
         for method_fn in method_files:
             tmp_fn = results_dir + "/" + method_fn
             print(tmp_fn)
             dat = load(tmp_fn)
 
-            pv_m, i_causal_m = cut_snps_close_to_causals(dat["p_values_uncut"], dat["pos"], dat["causal_idx"], mindist=mindist)
-            pv_lin_m, i_causal_m2 = cut_snps_close_to_causals(dat["p_values_lin_uncut"], dat["pos"], dat["causal_idx"], mindist=mindist)
+            pv_m, i_causal_m = cut_snps_close_to_causals(
+                dat["p_values_uncut"], dat["pos"], dat["causal_idx"], mindist=mindist
+            )
+            pv_lin_m, i_causal_m2 = cut_snps_close_to_causals(
+                dat["p_values_lin_uncut"],
+                dat["pos"],
+                dat["causal_idx"],
+                mindist=mindist,
+            )
 
             np.testing.assert_array_equal(i_causal_m, i_causal_m2)
 
             p_values.extend(pv_m)
             p_values_lin.extend(pv_lin_m)
             i_causal.extend(i_causal_m)
 
         p_values = np.array(p_values)
         p_values_lin = np.array(p_values_lin)
         i_causal = np.array(i_causal)
 
-
-        method_label = fn_filter.replace("_", "")# underscore prefix hides label
+        method_label = fn_filter.replace("_", "")  # underscore prefix hides label
         pylab.subplot(221)
         plot_prc_noshow(i_causal, -p_values, label=method_label)
         if fn_idx == 0:
             plot_prc_noshow(i_causal, -p_values_lin, label="lin")
 
         pylab.subplot(222)
         plot_roc_noshow(i_causal, -p_values, label=method_label)
         if fn_idx == 0:
             plot_roc_noshow(i_causal, -p_values_lin, label="lin")
-                
+
         pylab.subplot(223)
         plot_t1err_noshow(p_values, i_causal, label=method_label)
         if fn_idx == 0:
             plot_t1err_noshow(p_values_lin, i_causal, label="lin")
 
         pylab.subplot(224)
         plot_power_noshow(p_values, i_causal, label=method_label)
         if fn_idx == 0:
             plot_power_noshow(p_values_lin, i_causal, label="lin")
 
         print(p_values)
         print(i_causal)
 
-
     pylab.show()
 
 
 if __name__ == "__main__":
     num = 700000 * 500
     pv = X = np.random.random((num))
     i_causal = X = np.ones((num), dtype=bool)
-    
+
     t0 = time.time()
     compute_power_data(pv, i_causal)
     print(("time taken:", time.time() - t0))
```

### Comparing `fastlmm-0.6.7/fastlmm/association/heritability_spatial_correction.py` & `fastlmm-0.6.8b1/fastlmm/association/heritability_spatial_correction.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,15 +551,15 @@
                 == [alpha_dict[phen][0] for phen in jackknife_table.phen],
             )
             jk_table_corr = pd.pivot_table(
                 jackknife_table[corr_rows],
                 values=["h2uncorr", "h2corr", "diff", "e2"],
                 index=["phen"],
                 columns=[],
-                aggfunc=np.std,
+                aggfunc="std",
             )
             jk_table_corr["h2uncorr SE"] = jk_table_corr["h2uncorr"] * np.sqrt(
                 jackknife_count_actual - 1
             )
             jk_table_corr["h2corr SE"] = jk_table_corr["h2corr"] * np.sqrt(
                 jackknife_count_actual - 1
             )
@@ -579,15 +579,15 @@
                 == [alpha_dict[phen][1] for phen in jackknife_table.phen],
             )
             jk_table_gxe2 = pd.pivot_table(
                 jackknife_table[gxe2_rows],
                 values=["gxe2"],
                 index=["phen"],
                 columns=[],
-                aggfunc=np.std,
+                aggfunc="std",
             )
             jk_table_gxe2["gxe2 SE"] = jk_table_gxe2["gxe2"] * np.sqrt(
                 jackknife_count_actual - 1
             )
             del jk_table_gxe2["gxe2"]
 
             # Join the SE's to the main results table
@@ -692,15 +692,15 @@
         perm_table = permplus_table[permplus_table.permute_plus_index != -1]
         result = perm_table.join(real_result_permplus, on="phen")
         result["P(e2)"] = [
             1.0 if b else 0.0 for b in result.nLLcorr <= result.nLLcorr_real
         ]  # create a column showing where the perm is better (or as good) as the real
         # Use pivottable to find the fraction of of times when permutation is better
         pivot_table_plus = pd.pivot_table(
-            result, values=["P(e2)"], index=["phen"], columns=[], aggfunc=np.mean
+            result, values=["P(e2)"], index=["phen"], columns=[], aggfunc="mean"
         )
         if cache_folder is not None:
             summary_permplus_table_fn = (
                 "{0}/summary.permutation.GPlusE.{1}.count{2}.txt".format(
                     cache_folder, pheno.sid_count, permute_plus_count
                 )
             )
@@ -728,15 +728,15 @@
                 pheno_one = pheno[
                     :, pheno.col_to_index([phen_target])
                 ]  # Look at only this pheno_target
                 alpha_corr, alpha_gxe2 = alpha_dict[phen_target]
                 a2 = float(
                     permplus_table[permplus_table.phen == phen_target][
                         permplus_table.permute_plus_index == -1
-                    ]["a2"]
+                    ]["a2"].iloc[0]
                 )
                 for permute_index in range(-1, permute_times_count):
                     # pheno, G_kernel, spatial_coor, spatial_iid, alpha,          alpha_powerm (permute_index, permute_count, permute_seed),
                     arg_tuple = (
                         pheno_one,
                         G_kernel,
                         spatial_coor,
@@ -792,15 +792,15 @@
             perm_table = permtimes_table[permtimes_table.permute_times_index != -1]
             resultx = perm_table.join(real_result_permtimes, on="phen")
             resultx["P(gxe2)"] = [
                 1.0 if b else 0.0 for b in resultx.nLL_gxe2 <= resultx.nLL_gxe2_real
             ]  # create a column showing where the perm is better (or as good) as the real
             # Use pivottable to find the fraction of times when permutation is better
             pivot_table_times = pd.pivot_table(
-                resultx, values=["P(gxe2)"], index=["phen"], columns=[], aggfunc=np.mean
+                resultx, values=["P(gxe2)"], index=["phen"], columns=[], aggfunc="mean"
             )
             if cache_folder is not None:
                 _write_csv(pivot_table_times, True, summary_permtimes_table_fn)
 
         #######################
         # Create final table of results by combining the summary tables
         #######################
```

### Comparing `fastlmm-0.6.7/fastlmm/association/lrt.py` & `fastlmm-0.6.8b1/fastlmm/association/lrt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from __future__ import absolute_import
 import copy
-import pdb
 import scipy.linalg as LA
-import scipy as SP
-import numpy as NP
+import numpy as np
 import logging as LG
 import scipy.optimize as opt
 import scipy.stats as ST
 import scipy.special as SS
 import os
 import sys
 from fastlmm.pyplink.plink import *
@@ -17,15 +14,14 @@
 import fastlmm.util.stats as ss
 import fastlmm.inference as inference
 import fastlmm.association.score as score
 import fastlmm.association as association
 import statsmodels.api as sm
 
 from sklearn import linear_model
-from six.moves import range
 
 
 class lrt(association.varcomp_test):
     __slots__ = [
         "model0",
         "model1",
         "lrt",
@@ -87,26 +83,26 @@
         import statsmodels.api as sm
 
         logreg_mod = sm.Logit(self.Y, self.X)
         # logreg_sk = linear_model.LogisticRegression(penalty=penalty)
 
         logreg_result = logreg_mod.fit(disp=0)
         self.model0["nLL"] = logreg_result.llf
-        self.model0[
-            "h2"
-        ] = SP.nan  # so that code for both one-kernel and two-kernel prints out
-        self.model0["a2"] = SP.nan
+        self.model0["h2"] = (
+            np.nan
+        )  # so that code for both one-kernel and two-kernel prints out
+        self.model0["a2"] = np.nan
 
     def _nullModelLinReg(self, G0):
         assert G0 is None, "Linear regression cannot handle two kernels."
         self.model0 = {}
         model = ss.linreg(self.X, self.Y)
-        self.model0[
-            "h2"
-        ] = SP.nan  # so that code for both one-kernel and two-kernel prints out
+        self.model0["h2"] = (
+            np.nan
+        )  # so that code for both one-kernel and two-kernel prints out
         self.model0["nLL"] = model["nLL"]
 
     def _nullModelMixedEffectLinear(self, G0=None, K0=None):
         lmm0 = inference.getLMM(forcefullrank=self.forcefullrank)
         if G0 is not None:
             lmm0.setG(G0=G0, K0=K0)
         lmm0.setX(self.X)
@@ -126,15 +122,15 @@
         else:
             glmm0 = inference.getGLMM(approx, link, self.Y, None, None, penalty=penalty)
         glmm0.setX(self.X)
         glmm0.sety(self.Y)
         glmm0.optimize()
         self.model0 = {}
         self.model0["h2"] = 0.0
-        self.model0["a2"] = NP.nan
+        self.model0["a2"] = np.nan
         self.model0["nLL"] = -glmm0.marginal_loglikelihood()
         self.model0["sig02"] = glmm0.sig02
         self.model0["sig12"] = glmm0.sig12
         self.model0["sign2"] = glmm0.sign2
         for i in range(len(glmm0.beta)):
             self.model0["beta" + str(i)] = glmm0.beta[i]
 
@@ -145,16 +141,16 @@
             glmm0 = inference.getGLMM(approx, link, self.Y, G0, None, penalty=penalty)
         glmm0.setX(self.X)
         glmm0.setG(G0)
         glmm0.sety(self.Y)
         glmm0.optimize()
         self.model0 = {}
 
-        if glmm0.sig02 + glmm0.sign2 <= NP.sqrt(NP.finfo(NP.float).eps):
-            h2 = NP.nan
+        if glmm0.sig02 + glmm0.sign2 <= np.sqrt(np.finfo(np.float).eps):
+            h2 = np.nan
         else:
             h2 = glmm0.sig02 / (glmm0.sig02 + glmm0.sign2)
 
         self.model0["h2"] = h2
         self.model0["a2"] = 0.0
         self.model0["nLL"] = -glmm0.marginal_loglikelihood()
         self.model0["sig02"] = glmm0.sig02
@@ -191,15 +187,15 @@
         else:
             raise Exception("not implemented")
 
         # due to optimization the alternative log-likelihood might be a about 1E-6 worse than the null log-likelihood
         pvreg = ST.chi2.sf(
             stat, 1.0
         )  # standard way to compute p-value when no boundary conditions
-        if SP.isnan(pvreg) or pvreg > 1.0:
+        if np.isnan(pvreg) or pvreg > 1.0:
             pvreg = 1.0
         pv = 0.5 * pvreg  # conservative 50/50 estimate
         if alteqnull:
             pv = 1.0  # chi_0 component
 
         test = {
             "pv": pv,
@@ -248,15 +244,15 @@
         else:
             assert False, "Unkown effect type."
 
         # due to optimization the alternative log-likelihood might be a about 1E-6 worse than the null log-likelihood
         pvreg = ST.chi2.sf(
             stat, 1.0
         )  # standard way to compute p-value when no boundary conditions
-        if SP.isnan(pvreg) or pvreg > 1.0:
+        if np.isnan(pvreg) or pvreg > 1.0:
             pvreg = 1.0
         pv = 0.5 * pvreg  # conservative 50/50 estimate
         if alteqnull:
             pv = 1.0  # chi_0 component
 
         test = {
             "pv": pv,
@@ -342,20 +338,20 @@
         glmm1.sety(self.Y)
 
         glmm1.setG(G1)
         glmm1.optimize()
 
         assert glmm1.sig02 >= 0.0 and glmm1.sign2 >= 0
 
-        if glmm1.sig02 + glmm1.sign2 <= NP.sqrt(NP.finfo(NP.float).eps):
-            h2 = NP.nan
+        if glmm1.sig02 + glmm1.sign2 <= np.sqrt(np.finfo(np.float).eps):
+            h2 = np.nan
         else:
             h2 = glmm1.sig02 / (glmm1.sig02 + glmm1.sign2)
 
-        a2 = NP.nan
+        a2 = np.nan
 
         lik1 = {"nLL": -glmm1.marginal_loglikelihood(), "h2": h2, "a2": a2}
 
         lik1["sig02"] = glmm1.sig02
         lik1["sig12"] = glmm1.sig12
         lik1["sign2"] = glmm1.sign2
         for i in range(len(glmm1.beta)):
@@ -377,24 +373,24 @@
         glmm1.sety(self.Y)
 
         glmm1.setG(self.G0, G1)
         glmm1.optimize()
 
         assert glmm1.sig02 >= 0.0 and glmm1.sig12 >= 0.0 and glmm1.sign2 >= 0
 
-        if glmm1.sig02 + glmm1.sig12 + glmm1.sign2 <= NP.sqrt(NP.finfo(NP.float).eps):
+        if glmm1.sig02 + glmm1.sig12 + glmm1.sign2 <= np.sqrt(np.finfo(np.float).eps):
             # in this case we don't have enough precision to calculate the
             # proportion between sig02+sig12 and the total or it does not make sense
             # because the covariance of the posterior tends to zero
-            h2 = NP.nan
+            h2 = np.nan
         else:
             h2 = (glmm1.sig02 + glmm1.sig12) / (glmm1.sig02 + glmm1.sig12 + glmm1.sign2)
 
-        if glmm1.sig02 + glmm1.sig12 <= NP.sqrt(NP.finfo(NP.float).eps):
-            a2 = NP.nan
+        if glmm1.sig02 + glmm1.sig12 <= np.sqrt(np.finfo(np.float).eps):
+            a2 = np.nan
         else:
             a2 = glmm1.sig12 / (glmm1.sig02 + glmm1.sig12)
 
         lik1 = {"nLL": -glmm1.marginal_loglikelihood(), "h2": h2, "a2": a2}
 
         lik1["sig02"] = glmm1.sig02
         lik1["sig12"] = glmm1.sig12
```

### Comparing `fastlmm-0.6.7/fastlmm/association/meta_analysis.py` & `fastlmm-0.6.8b1/fastlmm/association/meta_analysis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,179 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import numpy as np
 import scipy.stats as st
 import fastlmm.util.mingrid as mingrid
-from six.moves import range
 
 
 class MetaAnalysis(object):
-    
+
     def __init__(self, beta, ste, tau=0):
         self.beta = beta
         self.ste = ste
         self.tau = tau
-    
+
     def var_beta(self):
         var = self.ste * self.ste + self.tau
         return var
 
     def inverse_variance_weights(self):
         return 1.0 / self.var_beta()
 
     def z_score(self):
         z_score = self.mean_beta() / self.ste_mean()
         return z_score
 
     def meta_pvalue(self):
-        z_score = self.z_score()        
+        z_score = self.z_score()
         chi2 = z_score * z_score
         return st.chi2.sf(chi2, 1)
 
     def mean_beta(self):
         weights = self.inverse_variance_weights()
         mean_beta = self.beta.dot(weights) / (weights).sum()
         return mean_beta
-        
+
     def ste_mean(self):
         return 1.0 / np.sqrt(self.inverse_variance_weights().sum())
 
     def log_likelihood(self, tau=None, mean_beta=None, reml=False):
-        
+
         if tau is None:
             var = self.var_beta()
         else:
             var = self.ste * self.ste + tau
 
         determinant = np.log(var).sum()
         if mean_beta is None:
             # ML (equiv. REML) estimate of beta:
             mean_beta = (self.beta / var).sum() / (1.0 / var).sum()
             if reml:
                 # perform REML
                 determinant += np.log((1.0 / var).sum()) - np.log(self.beta.shape)
-        residuals = (self.beta - mean_beta)
+        residuals = self.beta - mean_beta
         rss = (residuals * residuals / var).sum()
-        
-        log_likelihood = - 0.5 * (determinant + rss)
+
+        log_likelihood = -0.5 * (determinant + rss)
         return log_likelihood
 
 
 class FixefEffects(MetaAnalysis):
 
     def __init__(self, beta, ste):
         MetaAnalysis.__init__(self, beta=beta, ste=ste, tau=0)
 
 
 class RandomEffects(MetaAnalysis):
     """
-    We use REML to 
+    We use REML to
 
 
     Quantifying heterogeneity in a meta-analysis
     Julian P. T. Higgins and Simon G. Thompson
     MRC Biostatistics Unit; Institute of Public Health; Robinson Way; Cambridge CB2 2SR; U.K.
     """
+
     def __init__(self, beta, ste, reml=True):
-        self.reml=reml
+        self.reml = reml
         tau = self.estimate_tau(beta=beta, ste=ste)
         MetaAnalysis.__init__(self, beta=beta, ste=ste, tau=tau)
 
     def tau_ml(self, beta, ste):
         meta = MetaAnalysis(beta=beta, ste=ste, tau=0)
+
         def f(x):
             return -meta.log_likelihood(tau=x, mean_beta=0)
 
-        tau = mingrid.minimize1D(f, evalgrid=None, nGrid=10, minval=0.0, maxval=(beta*beta).mean(), verbose=False, brent=True,check_boundaries=True, resultgrid=None, return_grid=False)
+        tau = mingrid.minimize1D(
+            f,
+            evalgrid=None,
+            nGrid=10,
+            minval=0.0,
+            maxval=(beta * beta).mean(),
+            verbose=False,
+            brent=True,
+            check_boundaries=True,
+            resultgrid=None,
+            return_grid=False,
+        )
         return tau[0]
 
     def estimate_tau(self, beta, ste):
         meta = MetaAnalysis(beta=beta, ste=ste, tau=0)
+
         def f(x):
             return -meta.log_likelihood(tau=x, mean_beta=None, reml=self.reml)
 
-        tau = mingrid.minimize1D(f, evalgrid=None, nGrid=10, minval=0.0, maxval=(beta*beta).mean(), verbose=False, brent=True,check_boundaries=True, resultgrid=None, return_grid=False)
+        tau = mingrid.minimize1D(
+            f,
+            evalgrid=None,
+            nGrid=10,
+            minval=0.0,
+            maxval=(beta * beta).mean(),
+            verbose=False,
+            brent=True,
+            check_boundaries=True,
+            resultgrid=None,
+            return_grid=False,
+        )
         return tau[0]
 
 
 class HierarchicalRandomEffects(object):
     def __init__(self):
         pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import pylab as plt
+
     plt.ion()
 
     N_repeats = 1000
     tau = 0.0
     beta_true = 0.0
     N_tests = 1000
 
     z_scores = np.zeros(N_repeats)
     p_values = np.zeros(N_repeats)
     z_scores_re = np.zeros(N_repeats)
     p_values_re = np.zeros(N_repeats)
     for i in range(N_repeats):
-       
+
         var = np.random.uniform(size=N_tests)
         ste = np.sqrt(var)
-        beta = np.random.normal(size=N_tests) * np.sqrt(var+tau) + beta_true
-        
+        beta = np.random.normal(size=N_tests) * np.sqrt(var + tau) + beta_true
+
         fe = FixefEffects(beta=beta, ste=ste)
         p_values[i] = fe.meta_pvalue()
         mean_fe = fe.mean_beta()
         ste_fe = fe.ste_mean()
         var_beta = fe.var_beta()
         z_scores[i] = fe.z_score()
 
-        print("Fixed effects:  mean=%.6f, ste=%.6f, pv=%.6f, z_score=%.6f" % (mean_fe, ste_fe, p_values[i], z_scores[i]))
+        print(
+            "Fixed effects:  mean=%.6f, ste=%.6f, pv=%.6f, z_score=%.6f"
+            % (mean_fe, ste_fe, p_values[i], z_scores[i])
+        )
 
         re = RandomEffects(beta=beta, ste=ste)
         p_values_re[i] = re.meta_pvalue()
         mean_fe = re.mean_beta()
         ste_fe = re.ste_mean()
         var_beta = re.var_beta()
         z_scores_re[i] = re.z_score()
-        print("random effects:  mean=%.6f, ste=%.6f, pv=%.6f, z_score=%.6f" % (mean_fe, ste_fe, p_values_re[i], z_scores_re[i]))
-
-    plt.figure(); plt.hist(z_scores, bins=50)
-    plt.figure(); plt.hist(p_values)
-
-    plt.figure(); plt.hist(z_scores_re, bins=50)
-    plt.figure(); plt.hist(p_values_re)
-
-    plt.figure(); plt.plot(z_scores_re*z_scores_re, z_scores*z_scores, '.')
-
-
+        print(
+            "random effects:  mean=%.6f, ste=%.6f, pv=%.6f, z_score=%.6f"
+            % (mean_fe, ste_fe, p_values_re[i], z_scores_re[i])
+        )
+
+    plt.figure()
+    plt.hist(z_scores, bins=50)
+    plt.figure()
+    plt.hist(p_values)
+
+    plt.figure()
+    plt.hist(z_scores_re, bins=50)
+    plt.figure()
+    plt.hist(p_values_re)
 
+    plt.figure()
+    plt.plot(z_scores_re * z_scores_re, z_scores * z_scores, ".")
```

### Comparing `fastlmm-0.6.7/fastlmm/association/score.py` & `fastlmm-0.6.8b1/fastlmm/association/score.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from __future__ import absolute_import
-import numpy as NP
-import scipy as sp
+import numpy as np
 import scipy.linalg as LA
 import numpy.linalg as nla
 import os
 import sys
 import glob
-from six.moves import range
 
 sys.path.append("./../../pyplink")
 from fastlmm.pyplink.plink import *
 from pysnptools.util.pheno import *
 from fastlmm.util.mingrid import *
 
 # import pdb
@@ -81,31 +78,31 @@
         "stdY",
         "VX",
         "pinvVX",
     ]
 
     def __init__(self, Y, X=None, appendbias=False):
         ## check if is binary
-        uniquey = sp.unique(Y)
-        if not sp.sort(uniquey).tolist() == [0, 1]:
+        uniquey = np.unique(Y)
+        if not np.sort(uniquey).tolist() == [0, 1]:
             raise Exception(
                 "must use binary data in {0,1} for logit tests, found:" + str(Y)
             )
 
         scoretest.__init__(self, Y=Y, X=X, appendbias=appendbias)
         # from sklearn.linear_model import LogisticRegression as LR
         # logreg_sk = LR(C=200000.0)
         # logreg_sk.fit( X, Y )
         import statsmodels.api as sm
 
         self.logreg_mod = sm.Logit(Y[:, 0], X)
         self.logreg_result = self.logreg_mod.fit(disp=0)
         self.pY = self.logreg_result.predict(X)
-        self.stdY = sp.sqrt(self.pY * (1.0 - self.pY))
-        self.VX = self.X * NP.lib.stride_tricks.as_strided(
+        self.stdY = np.sqrt(self.pY * (1.0 - self.pY))
+        self.VX = self.X * np.lib.stride_tricks.as_strided(
             (self.stdY), (self.stdY.size, self.X.shape[1]), (self.stdY.itemsize, 0)
         )
         self.pinvVX = nla.pinv(self.VX)
 
     def _score(self, G1):
         """
         compute the score
@@ -128,15 +125,15 @@
         if X is None:
             D = 1  # num of covariates (and assumes they are independent)
         else:
             D = X.shape[1]
         RxY = (
             self.Y.flatten() - self.pY
         )  # residual of y regressed on X, which here, is equivalent to sigma2*Py (P is the projection matrix, which is idempotent)
-        VG = G1 * NP.lib.stride_tricks.as_strided(
+        VG = G1 * np.lib.stride_tricks.as_strided(
             self.stdY, (self.stdY.size, G1.shape[1]), (self.stdY.itemsize, 0)
         )
         GY = G1.T.dot(RxY)
         squaredform = (GY * GY).sum() / (2.0 * P)
 
         RxVG, Xd = linreg(VG, X=self.VX, Xdagger=self.pinvVX, rcond=-1)
         if G1.shape[0] < G1.shape[1]:
@@ -182,30 +179,30 @@
         else:
             P = Y.shape[1]
         D = 1
         if X is not None:
             D = X.shape[1]
         self.Neff = N - D
         if self.K is not None:
-            ar = sp.arange(self.K.shape[0])
+            ar = np.arange(self.K.shape[0])
             self.K[ar, ar] += 1.0
             self.PxKPx, self.Xdagger = linreg(
                 Y=(self.K), X=self.X, Xdagger=self.Xdagger
             )
             self.PxKPx, self.Xdagger = linreg(
                 Y=self.PxKPx.T, X=self.X, Xdagger=self.Xdagger
             )
             [self.S, self.U] = LA.eigh(self.PxKPx)
             self.K[ar, ar] -= 1.0
             self.U = self.U[:, D:N]
             self.S = self.S[D:N] - 1.0
         elif 0.7 * (self.Neff) <= self.G0.shape[1] or forcefullrank:
             self.K = self.G0.dot(self.G0.T)
             # BR: changed K to self.K (K is not defined)
-            ar = sp.arange(self.K.shape[0])
+            ar = np.arange(self.K.shape[0])
             self.K[ar, ar] += 1.0
             self.PxKPx, self.Xdagger = linreg(
                 Y=(self.K), X=self.X, Xdagger=self.Xdagger
             )
             self.PxKPx, self.Xdagger = linreg(
                 Y=self.PxKPx.T, X=self.X, Xdagger=self.Xdagger
             )
@@ -242,15 +239,15 @@
             return res["nLL"]
 
         min = minimize1D(f, evalgrid=None, nGrid=20, minval=0.0, maxval=0.99999)
 
         self.optparams = resmin[0]
 
         # pre-compute model parameters
-        self.expectedinfo = sp.zeros((2, 2))
+        self.expectedinfo = np.zeros((2, 2))
         # tr(PIPI)
         Sd = 1.0 / ((1.0 - self.optparams["h2"]) + self.optparams["h2"] * self.S)
         Sd *= Sd
         self.expectedinfo[0, 0] = (
             Sd
         ).sum()  # /(self.optparams['sigma2']*self.optparams['sigma2'])
         if self.lowrank:
@@ -294,41 +291,41 @@
         N = self.Y.shape[0]
         if self.Y.ndim == 1:
             P = 1
         else:
             P = self.Y.shape[1]
 
         Sd = h2 * self.S + (1.0 - h2)
-        UYS = self.UY / NP.lib.stride_tricks.as_strided(
+        UYS = self.UY / np.lib.stride_tricks.as_strided(
             Sd, (Sd.size, self.UY.shape[1]), (Sd.itemsize, 0)
         )
 
         YKY = (UYS * self.UY).sum()
 
-        logdetK = sp.log(Sd).sum()
+        logdetK = np.log(Sd).sum()
 
         if self.lowrank:  # low rank part
             YKY += self.YUUY / (1.0 - h2)
-            logdetK += sp.log(1.0 - h2) * (self.Neff * P - k)
+            logdetK += np.log(1.0 - h2) * (self.Neff * P - k)
 
         sigma2 = YKY / (self.Neff * P)
-        nLL = 0.5 * (logdetK + self.Neff * P * (sp.log(2.0 * sp.pi * sigma2) + 1))
+        nLL = 0.5 * (logdetK + self.Neff * P * (np.log(2.0 * np.pi * sigma2) + 1))
         result = {"nLL": nLL, "sigma2": sigma2, "h2": h2}
         return result
 
     def _score(self, G1):
         """
         compute the score with a background kernel
         """
         # if 1:
         #    #background kernel
         #    self.K=self.G.dot(self.G.T)
         #    h2 = self.optparams['h2']
         #    sig = self.optparams['sigma2']
-        #    V = h2*self.K + (1-h2)*sp.eye(self.K.shape[0])
+        #    V = h2*self.K + (1-h2)*np.eye(self.K.shape[0])
         #    V*=sig
         #    Vi=LA.inv(V)
         #    P =LA.inv(self.X.T.dot(Vi).dot(self.X))
         #    P=self.X.dot(P.dot(self.X.T))
         #    P=Vi.dot(P.dot(Vi))
         #    Px = Vi-P
 
@@ -336,15 +333,15 @@
         resG, Xdagger = linreg(Y=G1, X=self.X, Xdagger=self.Xdagger)
         sigma2e = (1.0 - self.optparams["h2"]) * self.optparams["sigma2"]
         sigma2g = self.optparams["h2"] * self.optparams["sigma2"]
         UG = self.U.T.dot(resG)
         if self.lowrank:
             UUG = resG - self.U.dot(UG)
         Sd = 1.0 / (self.S * sigma2g + sigma2e)
-        SUG = UG * NP.lib.stride_tricks.as_strided(
+        SUG = UG * np.lib.stride_tricks.as_strided(
             Sd, (Sd.size, UG.shape[1]), (Sd.itemsize, 0)
         )
         # tr(YPGGPY)
         GPY = SUG.T.dot(self.UY)
         if self.lowrank:
             GPY += UUG.T.dot(self.UUY) / sigma2e
         squaredform = 0.5 * (GPY * GPY).sum()
@@ -354,18 +351,18 @@
         else:
             GPG = SUG.dot(UG.T)
         expectationsqform = 0.5 * P * GPG.trace()
         # tr(PGGPGG)
         trPGGPGG = 0.5 * P * (GPG * GPG).sum()
         # tr(PGGPI)
         SUG *= SUG
-        expectedInfoCross = sp.empty(2)
+        expectedInfoCross = np.empty(2)
         expectedInfoCross[0] = 0.5 * P * SUG.sum()
         # tr(PGGPK)
-        SUG *= NP.lib.stride_tricks.as_strided(
+        SUG *= np.lib.stride_tricks.as_strided(
             self.S, (self.S.size, SUG.shape[1]), (self.S.itemsize, 0)
         )
         expectedInfoCross[1] = 0.5 * P * SUG.sum()
         if self.lowrank:
             if G1.shape[0] > G1.shape[1]:
                 GPG_lowr = UUG.T.dot(UUG) / sigma2e
             else:
@@ -469,40 +466,40 @@
     #     also note that "RxY"=Py=1/sigma2*(I-Xdagger*X)y is nothing more (except for 1/sigma2) than the residual of y regressed on X (i.e. y-X*beta),
     #     and similarly for PG="RxG"
     GtRxY = G.T.dot(RxY)
     squaredform = ((GtRxY * GtRxY).sum()) * (
         0.5 / (sigma2 * sigma2)
     )  # yPKPy=yPG^T*GPy=(yPG^T)*(yPG^T)^T
     if G.shape[0] > G.shape[1]:
-        GPG = sp.dot(
+        GPG = np.dot(
             RxG.T, RxG
         )  # GPG is always a square matrix in the smaller dimension
     else:
-        GPG = sp.dot(RxG, RxG.T)
+        GPG = np.dot(RxG, RxG.T)
     expectationsqform = (
         P * (GPG.trace()) * (0.5 / sigma2)
     )  # note this is Trace(PKP)=Trace(PPK)=Trace(PK), for P=projection matrix in comment, and in the code P=1=#phen
     expectedinfo00 = P * (GPG * GPG).sum() * (0.5 / (sigma2 * sigma2))
     expectedinfo10 = expectationsqform / sigma2  # P*0.5/(sigma2*sigma2)*GPG.trace()
     expectedinfo11 = P * (N - D) * (0.5 / (sigma2 * sigma2))
     varsqform = 1.0 / (
         expectedinfo00 - expectedinfo10 * expectedinfo10 / expectedinfo11
     )
     # if 1:
     #    XXi=LA.inv(X.T.dot(X))
-    #    Px=(sp.eye(N)-X.dot(XXi).dot(X.T))/sigma2
+    #    Px=(np.eye(N)-X.dot(XXi).dot(X.T))/sigma2
     # pdb.set_trace()
     GPG /= (
         sigma2 * 2.0
     )  # what we will take eigenvalues of for Davies (which is P^1/2*K*P^1/2)
 
     # for debugging, explicitly compute GPG=P^1/2 * K * P^1/2
-    # SigInv=(1/sigma2)*sp.eye(N,N)
+    # SigInv=(1/sigma2)*np.eye(N,N)
     # Phat=X.dot(LA.inv(X.T.dot(SigInv).dot(X))).dot(X.T).dot(SigInv)
-    # PP=SigInv.dot(sp.eye(N,N)-Phat)
+    # PP=SigInv.dot(np.eye(N,N)-Phat)
     # K=G.dot(G.T)
     # PKP=PP.dot(K).dot(PP)
     # ss.stats(PKP-PKP.T)
     ##eigvalsFull=LA.eigh(PKP,eigvals_only=True)
     # eigvalsFull2=LA.eigvals(PKP)
     # eigvalsLow =LA.eigh(GPG,eigvals_only=True)
     # GPG=PKP*0.5
```

### Comparing `fastlmm-0.6.7/fastlmm/association/single_snp.py` & `fastlmm-0.6.8b1/fastlmm/association/single_snp.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,16 +207,16 @@
     >>> test_snps = example_file("fastlmm/feature_selection/examples/toydata.5chrom.*","*.bed")
     >>> results_dataframe = single_snp(test_snps=test_snps, pheno=pheno_fn, count_A1=False)
     >>> print(results_dataframe.iloc[0].SNP,round(results_dataframe.iloc[0].PValue,7),len(results_dataframe))
     null_576 1e-07 10000
 
     For more examples, see:
 
-    * `Main FaST-LMM notebook <https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb>`_
-    * `Effect size, multiple phenotypes, and related new features <https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb>`_
+    * `Main FaST-LMM notebook <https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb>`_
+    * `Effect size, multiple phenotypes, and related new features <https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb>`_
     """
     #!!!LATER raise error if covar has NaN
     t0 = time.time()
     if force_full_rank and force_low_rank:
         raise Exception("Can't force both full rank and low rank")
 
     if K1 or G1:  # If 2nd kernel given, use numpy
```

### Comparing `fastlmm-0.6.7/fastlmm/association/single_snp_all_plus_select.py` & `fastlmm-0.6.8b1/fastlmm/association/single_snp_all_plus_select.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/single_snp_linreg.py` & `fastlmm-0.6.8b1/fastlmm/association/single_snp_linreg.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/single_snp_scale.py` & `fastlmm-0.6.8b1/fastlmm/association/single_snp_scale.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/single_snp_select.py` & `fastlmm-0.6.8b1/fastlmm/association/single_snp_select.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from __future__ import absolute_import
-from __future__ import print_function
+import warnings
 import numpy as np
 import logging
 from sklearn.model_selection import KFold
 import pandas as pd
 import os
 import time
 from unittest.mock import patch
+import sys
 
 import pysnptools.util as pstutil
 from pysnptools.util.mapreduce1 import map_reduce
 from pysnptools.util.mapreduce1.runner import Local
 from pysnptools.standardizer import Unit
 from pysnptools.kernelreader import KernelReader
 from pysnptools.kernelreader import KernelData
@@ -49,14 +49,16 @@
     force_full_rank=False,
     force_low_rank=False,
     h2=None,
     runner=None,
     count_A1=None,
 ):
     """
+    DEPRECATED: Runs only on Intel, not AMD. We can't test this function because `compute_auto_pcs` uses the 'fastlmmC' executable which is not available in the test environment.
+
     Function performing single SNP GWAS based on covariates (often PCs) and a similarity matrix constructed of the top *k* SNPs where
     SNPs are ordered via the PValue from :meth:`.single_snp_linreg` and *k* is determined via out-of-sample prediction. Will reorder and intersect IIDs as needed.
 
     :param test_snps: SNPs to test. Can be any `SnpReader <http://fastlmm.github.io/PySnpTools/#snpreader-snpreader>`__. If you give a string, it should be the base name of a set of PLINK Bed-formatted files.
            (For backwards compatibility can also be dictionary with keys 'vals', 'iid', 'header')
     :type test_snps: a `SnpReader <http://fastlmm.github.io/PySnpTools/#snpreader-snpreader>`__ or a string
 
@@ -128,14 +130,17 @@
     >>> phen_fn = example_file("tests/datasets/synth/pheno_10_causals.txt")
     >>> covar = compute_auto_pcs(bed_fn,count_A1=False)
     >>> results_dataframe = single_snp_select(test_snps=bed_fn, G=bed_fn, pheno=phen_fn, covar=covar, GB_goal=2, count_A1=False)
     >>> print(results_dataframe.iloc[0].SNP,round(results_dataframe.iloc[0].PValue,7),len(results_dataframe))
     snp495_m0_.01m1_.04 0.0 5000
 
     """
+    warning_text = "This function is deprecated. Runs only on Intel, not AMD. We can't test this function because `compute_auto_pcs` uses the 'fastlmmC' executable which is not available in the test environment."
+    warnings.warn(warning_text, category=DeprecationWarning, stacklevel=2)
+    print(warning_text, file=sys.stderr)
     with patch.dict("os.environ", {"ARRAY_MODULE": "numpy"}) as _:
         #!!!code similar to single_snp and feature_selection
         if force_full_rank and force_low_rank:
             raise Exception("Can't force both full rank and low rank")
 
         assert test_snps is not None, "test_snps must be given as input"
```

### Comparing `fastlmm-0.6.7/fastlmm/association/snp_set.py` & `fastlmm-0.6.8b1/fastlmm/association/snp_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-from __future__ import absolute_import
-from __future__ import print_function
 from pysnptools.util.mapreduce1.runner import *
 import logging
 import fastlmm.pyplink.plink as plink
 import numpy as np
 from fastlmm.inference.lmm_cov import LMM as fastLMM
 import scipy.stats as stats
 from fastlmm.util.pickle_io import load, save
 import time
 import pandas as pd
 
+
 def snp_set(
-        test_snps,
-        set_list,
-        pheno,
-        covar = None,
-        output_file_name = None,
-        G0 = None,
-        test="lrt",
-        write_lrtperm = False,
-        nperm = 10,
-        npermabs = None,
-        mpheno=1,
-        G0_fit="qq",
-        qmax=0.1,
-        seed =   None,
-        minsetsize = None,
-        maxsetsize = None,
-        mindist=0,
-        idist=1,
-        show_pvalue_5050 = False
-    ):
+    test_snps,
+    set_list,
+    pheno,
+    covar=None,
+    output_file_name=None,
+    G0=None,
+    test="lrt",
+    write_lrtperm=False,
+    nperm=10,
+    npermabs=None,
+    mpheno=1,
+    G0_fit="qq",
+    qmax=0.1,
+    seed=None,
+    minsetsize=None,
+    maxsetsize=None,
+    mindist=0,
+    idist=1,
+    show_pvalue_5050=False,
+):
     """
     Function performing GWAS on sets of snps
 
 
     :param test_snps: The base name of the file containing the SNPs for alternative kernel. The file must be in PLINK Bed format.
     :type test_snps: a string
 
@@ -109,70 +108,74 @@
     ...     set_list = '../../tests/datasets/set_input.23.txt',
     ...     pheno = '../../tests/datasets/phenSynthFrom22.23.N300.txt')
     >>> print(result_dataframe.iloc[0].SetId, round(result_dataframe.iloc[0]['P-value'],15))
     set23 0.0
 
     """
 
-    assert test=="lrt" or test=="sc_davies", "Expect test to be 'lrt' or 'sc_davies'"
+    assert (
+        test == "lrt" or test == "sc_davies"
+    ), "Expect test to be 'lrt' or 'sc_davies'"
 
     if G0 is None:
-        nullModel={'effect':'fixed', 'link':'linear'}
-        altModel={'effect':'mixed', 'link':'linear'}
+        nullModel = {"effect": "fixed", "link": "linear"}
+        altModel = {"effect": "mixed", "link": "linear"}
     else:
-        nullModel={'effect':'mixed', 'link':'linear'}
-        altModel={'effect':'mixed', 'link':'linear'}
-        if test=="lrt":
-            test="lrt_up"
-
+        nullModel = {"effect": "mixed", "link": "linear"}
+        altModel = {"effect": "mixed", "link": "linear"}
+        if test == "lrt":
+            test = "lrt_up"
 
     if output_file_name is None:
         import tempfile
+
         fileno, output_file_name = tempfile.mkstemp()
-        fptr= os.fdopen(fileno)
+        fptr = os.fdopen(fileno)
         is_temp = True
     else:
         is_temp = False
 
-
     from fastlmm.association.FastLmmSet import FastLmmSet
+
     fast_lmm_set = FastLmmSet(
         outfile=output_file_name,
         phenofile=pheno,
         alt_snpreader=test_snps,
         altset_list=set_list,
         covarfile=covar,
         filenull=G0,
         nperm=nperm,
         mindist=mindist,
         idist=idist,
         mpheno=mpheno,
-        nullfit = G0_fit,
+        nullfit=G0_fit,
         qmax=qmax,
         test=test,
         autoselect=False,
         nullModel=nullModel,
         altModel=altModel,
-        npermabs = npermabs,
-        calseed = seed,
-        minsetsize = minsetsize,
-        maxsetsize = maxsetsize,
-        write_lrtperm = write_lrtperm,
-        show_pvalue_5050 = show_pvalue_5050,
-        )
+        npermabs=npermabs,
+        calseed=seed,
+        minsetsize=minsetsize,
+        maxsetsize=maxsetsize,
+        write_lrtperm=write_lrtperm,
+        show_pvalue_5050=show_pvalue_5050,
+    )
     result = Local().run(fast_lmm_set)
 
-    dataframe=pd.read_csv(output_file_name,delimiter='\t',comment=None) #Need \t instead of \s because the output has tabs by design and spaces in column names(?)
+    dataframe = pd.read_csv(
+        output_file_name, delimiter="\t", comment=None
+    )  # Need \t instead of \s because the output has tabs by design and spaces in column names(?)
     if is_temp:
         fptr.close()
         os.remove(output_file_name)
 
     return dataframe
-    
+
 
 if __name__ == "__main__":
 
     import doctest
+
     doctest.testmod()
 
     print("done")
-
```

### Comparing `fastlmm-0.6.7/fastlmm/association/testCV.py` & `fastlmm-0.6.8b1/fastlmm/association/testCV.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-from __future__ import absolute_import
 import fastlmm.association as association
-import scipy as sp
+import numpy as np
 from sklearn import linear_model
 from sklearn import model_selection
 from sklearn.model_selection import GridSearchCV
 
 #!! from fastlmm.external.sklearn.metrics.scorer import SCORERS, Scorer
 from fastlmm import inference
 import fastlmm.util.util as util
-import pdb
-from six.moves import range
 
 
 class testCV(association.varcomp_test):
     __slots__ = [
         "G0",
         "greater_is_better",
         "model",
@@ -157,26 +154,26 @@
         elif modelDesc["effect"] == "mixed":
             return self._getParamGridMixedEffectModel(G0, G1)
 
         assert False
 
     def _getParamGridFixedEffectModel(self, G0, G1, link):
         if link == "linear":
-            param_grid = dict(alpha=0.5 * sp.logspace(-5, 5, 20))
+            param_grid = dict(alpha=0.5 * np.logspace(-5, 5, 20))
         elif link == "logistic":
-            param_grid = dict(C=sp.logspace(-5, 5, 20))
+            param_grid = dict(C=np.logspace(-5, 5, 20))
         else:
             assert False
 
         return param_grid
 
     def _getParamGridMixedEffectModel(self, G0, G1):
         param_grid = dict(
-            sig02=sp.arange(0.0, 2.1, 0.4),
-            sig12=sp.arange(0.0, 2.1, 0.4),
+            sig02=np.arange(0.0, 2.1, 0.4),
+            sig12=np.arange(0.0, 2.1, 0.4),
             sign2=[None],
             beta=[None],
         )
 
         if G0 is None:
             param_grid["sig02"] = [0.0]
         if G1 is None:
@@ -218,15 +215,15 @@
 
     # the effect parameter should not be used here, but I dont have a better an idea for now
     def score_nestedCV(self, G1, model, param_grid, effect, nested):
         k_fold = model_selection.KFold(n_splits=self.n_folds).split(
             list(range(self.Y.shape[0]))
         )
         i_fold = 0
-        scores = sp.zeros(self.n_folds)
+        scores = np.zeros(self.n_folds)
         params = list()
 
         for train, test in k_fold:
             (trainData, trainY) = self._packData(G1, train, effect)
             (testData, testY) = self._packData(G1, test, effect)
 
             if nested:
@@ -254,29 +251,29 @@
         return scores, params
 
     def _packData(self, G1, indices2select, effect):
         if effect == "fixed":
             if G1 is None and self.G0 is None:
                 data = self.X[self.data_permutation][indices2select]
             elif G1 is None:
-                data = sp.column_stack(
+                data = np.column_stack(
                     (
                         self.G0[self.data_permutation][indices2select],
                         self.X[self.data_permutation][indices2select],
                     )
                 )
             elif self.G0 is None:
-                data = sp.column_stack(
+                data = np.column_stack(
                     (
                         G1[self.data_permutation][indices2select],
                         self.X[self.data_permutation][indices2select],
                     )
                 )
             else:
-                data = sp.column_stack(
+                data = np.column_stack(
                     (
                         self.G0[self.data_permutation][indices2select],
                         G1[self.data_permutation][indices2select],
                         self.X[self.data_permutation][indices2select],
                     )
                 )
         elif effect == "mixed":
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/Cv.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/Cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from __future__ import absolute_import
 import fastlmm.association.lrt as lr
-import scipy as SP
+import numpy as np
 import fastlmm.util.stats.chi2mixture as c2
 import fastlmm.association.testCV as testCV
 import logging
-from six.moves import range
 
 
 class Cv(object):
     """description of class"""
 
     __slots__ = []
 
@@ -30,15 +28,15 @@
         SNPs0=None,
         nullModel=None,
         altModel=None,
         scoring=None,
         greater_is_better=None,
     ):
         return testCV.testCV(
-            Y=Y[:, SP.newaxis],
+            Y=Y[:, np.newaxis],
             X=X,
             G0=G0,
             nullModel=nullModel,
             altModel=altModel,
             scoring=scoring,
             greater_is_better=greater_is_better,
         )
@@ -54,23 +52,23 @@
         raise Exception("'pv' doesn't apply to cv only to davies")
 
     @property
     def npvals(self):
         return 1  # returns 1 type of p-value
 
     def w2(self, G0, result):
-        return SP.nan
+        return np.nan
 
     def lrt_method(self, result):
         return result.test[
             "stat"
         ]  # iset is the index of the test (irrespective of permutation)
 
     def pv_adj_from_result(self, result):
-        return SP.nan
+        return np.nan
 
     def write(self, fp, ind, result_dict, pv_adj, detailed_table):
         fp.write(
             "\t".join(
                 (
                     "SetId",
                     "stat",
@@ -106,15 +104,15 @@
                     + "\n"
                 )
             )
 
     def pv_etc(
         self, filenull, G0_to_use, G1, y, x, null_model, varcomp_test, forcefullrank
     ):
-        return [SP.nan, SP.nan, SP.nan]
+        return [np.nan, np.nan, np.nan]
 
     #!! could these three methods be move to __init__.py?
     @staticmethod
     def pv_adj_and_ind(
         nperm,
         pv_adj,
         nullfit,
@@ -197,15 +195,15 @@
                 qmax=qmax,
                 alteqnull=alteqnullperm,
                 abserr=abserr,
                 fitdof=fitdof,
                 dof=dof,
             )
 
-            res = mix.fit_params_Qreg()  # paramter fitting
+            res = mix.fit_params_Qreg()  # parameter fitting
 
             imax = res["imax"]
             mse = res["mse"]
             logging.info("# of pvals used for nullfit=" + str(imax))
             pv_adj = mix.sf(
                 lrt=lrt, alteqnull=alteqnull
             )  # getting p-values for real data
@@ -239,15 +237,15 @@
                 qmax=qmax,
                 alteqnull=alteqnullfile,
                 abserr=abserr,
                 fitdof=fitdof,
                 dof=dof,
             )
 
-            res = mix.fit_params_Qreg()  # paramter fitting
+            res = mix.fit_params_Qreg()  # parameter fitting
 
             imax = res["imax"]
             mse = res["mse"]
             logging.info("# of pvals used for nullfit=" + str(imax))
             pv_adj = mix.sf(
                 lrt=lrt, alteqnull=alteqnull
             )  # getting p-values for real data
@@ -266,15 +264,15 @@
                 lrt=lrt,
                 qmax=qmax,
                 alteqnull=alteqnull,
                 abserr=abserr,
                 fitdof=fitdof,
                 dof=dof,
             )
-            res = mix.fit_params_Qreg()  # paramter fitting
+            res = mix.fit_params_Qreg()  # parameter fitting
             imax = res["imax"]
             logging.info("# of pvals used for nullfit=" + str(imax))
             pv_adj = mix.sf()  # getting p-values
             logging.info(" Done")
         if mix.mixture == 0:
             # raise Exception("only zero dof component items found")
             logging.info("*****WARNING*****: only zero dof component items found")
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/LRT_up.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/LRT_up.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import fastlmm.inference.lmm_cov as lmm
 import numpy as np
 import fastlmm.util.stats.chi2mixture as c2
 import fastlmm.association as association
 import scipy.stats as st
 from . import tests_util as tu
-from six.moves import range
 
 
 class lrt(association.varcomp_test):
     __slots__ = [
         "lmm",
         "lrt",
         "forcefullrank",
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/Lrt.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/Lrt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from __future__ import absolute_import
 import fastlmm.association.lrt as lr
-import scipy as sp
+import numpy as np
 import fastlmm.util.stats.chi2mixture as c2
 
 from . import tests_util as tu
-from six.moves import range
 
 
 class Lrt(object):
     """description of class"""
 
     def check_nperm(self, nperm):
         return nperm  # permutations are fine, so just return
@@ -70,20 +68,20 @@
     def lrt_method(self, result):
         return result.stat
 
     def pv_adj_from_result(self, result):
         """
         If local aUD exists, take that, if not, take the raw local.
         """
-        if "pv-local-aUD" in result.test and not sp.isnan(result.test["pv-local-aUD"]):
+        if "pv-local-aUD" in result.test and not np.isnan(result.test["pv-local-aUD"]):
             return result.test["pv-local-aUD"]
         elif "pv-local" in result.test:
             return result.test["pv-local"]
         else:
-            return sp.nan
+            return np.nan
 
     def pv_adj_and_ind(
         self,
         nperm,
         pv_adj,
         nullfit,
         lrt,
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/Sc.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/Sc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from __future__ import absolute_import
 import fastlmm.association.lrt as lr
-import scipy as SP
+import numpy as np
 import fastlmm.util.stats.chi2mixture as c2
 import fastlmm.association.score as score
 import scipy.linalg as LA
 import scipy.stats as ST
 from . import tests_util as tu
-from six.moves import range
 
 
 class Sc(object):
     """description of class"""
 
     __slots__ = ["score"]
 
@@ -51,15 +49,15 @@
             )
         G0, K0 = tu.set_snps0(
             SNPs0=SNPs0,
             sample_size=Y.shape[0],
             i_exclude=i_exclude,
             forcefullrank=forcefullrank,
         )
-        return score.scoretest2K(Y=Y[:, SP.newaxis], X=X, K=K0, G0=G0)
+        return score.scoretest2K(Y=Y[:, np.newaxis], X=X, K=K0, G0=G0)
 
     def construct_no_backgound_kernel(
         self, Y, X, forcefullrank, nullModel, altModel, scoring, greater_is_better
     ):
         if nullModel["link"] == "logistic":
             assert (
                 nullModel["effect"] == "fixed"
@@ -68,29 +66,29 @@
             ), (
                 "By choosing the logistic link for the "
                 "null model, you should also select "
                 "fixed effect for null model, "
                 "mixed effect and logistic link for alt "
                 "model."
             )
-            return score.scoretest_logit(Y=Y[:, SP.newaxis], X=X)
+            return score.scoretest_logit(Y=Y[:, np.newaxis], X=X)
 
         elif nullModel["link"] == "linear":
             assert (
                 nullModel["effect"] == "fixed"
                 and altModel["link"] == "linear"
                 and altModel["effect"] == "mixed"
             ), (
                 "By choosing the linear link for the "
                 "null model, you should also select "
                 "fixed effect for null model, "
                 "mixed effect and linear link for alt "
                 "model."
             )
-            return score.scoretest(Y=Y[:, SP.newaxis], X=X)
+            return score.scoretest(Y=Y[:, np.newaxis], X=X)
         else:
             raise Exception("Invalid link for score null model: " + link)
 
     def pv(self, squaredform, expectationsqform, varsqform, GPG):
         if self.score == "davies":
             return Sc.pv_davies(squaredform, expectationsqform, varsqform, GPG)
         elif self.score == "mom":
@@ -196,13 +194,13 @@
                 G1=G1,
                 y=y,
                 nulldistrib=self,
                 covar=x,
                 appendbias=False,
                 test2K=null_model,
             )
-            return pv, SP.nan, SP.nan
+            return pv, np.nan, np.nan
         else:
             pv = score.onekerneltest(
                 G0=G1, y=y, nulldistrib=self, covar=x, appendbias=False
             )
-            return pv, SP.nan, SP.nan
+            return pv, np.nan, np.nan
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/__init__.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 '''
-#!! fix comments
 snpset is a named set of snps.  See the Bed class's 'read' method of examples of their use.
 
 A snpset is defined with two classes that implement these two interfaces: ISnpSet and ISnpSetPlusBed.
 Note: Python doesn't enforce interfaces.
 
 interface ISnpSet
     def addbed(self, bed):
@@ -16,13 +15,13 @@
     def __iter__(self):
         return # index number to position in BIM file
 
     def __str__(self):
         return # string of name of this set of snps
 '''
 
-from __future__ import absolute_import
-from .Lrt import *
-from .Cv import *
-from .Sc import *
-from . import LRT_up as lrt
-
+from .AllSnps import *
+from .PositionRange import *
+from .SnpSetAndName import *
+from .SnpsFromFile import *
+from .SnpIndexList import *
+from .RandomSnpSet import *
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/test_gpu_perf.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_gpu_perf.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/test_gwas.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_gwas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from __future__ import absolute_import
 import numpy as np
-import scipy as sp
 import logging
 from scipy import stats
 from fastlmm.pyplink.snpreader.Bed import Bed
 
 # from fastlmm.association.gwas import LeaveOneChromosomeOut, LocoGwas, FastGwas, load_intersect
 from fastlmm.association.LeaveOneChromosomeOut import LeaveOneChromosomeOut
 from fastlmm.association.PrecomputeLocoPcs import load_intersect
 from fastlmm.association.LocoGwas import FastGwas, LocoGwas
 from fastlmm.util import run_fastlmmc
 from fastlmm.inference import LMM
 import unittest
 import os.path
 import time
-from six.moves import range
+
 import platform
 
 currentFolder = os.path.dirname(os.path.realpath(__file__))
 
 
 class TestGwas(unittest.TestCase):
     @classmethod
@@ -92,14 +90,32 @@
     ## make sure we get p-values right
     # np.testing.assert_array_almost_equal(gwas.p_values, gwas_c.p_values, decimal=3)
     # np.testing.assert_array_almost_equal(gwas.p_values, gwas_f.p_values, decimal=3)
 
     # np.testing.assert_array_almost_equal(gwas.sorted_p_values, gwas_c.sorted_p_values, decimal=3)
     # np.testing.assert_array_almost_equal(gwas.sorted_p_values, gwas_f.sorted_p_values, decimal=3)
 
+    @staticmethod
+    def read_results(filename):
+        import pandas as pd
+
+        out_file = os.path.normpath(
+            os.path.join(
+                os.path.dirname(__file__),
+                "../Fastlmm_autoselect/bypass",
+                filename,
+            )
+        )
+        table = pd.read_csv(out_file, sep="\t")
+
+        p_values = table.sort_values(["Chromosome", "Position"])["Pvalue"].tolist()
+        sorted_p_values = table["Pvalue"].tolist()
+        sorted_snps = table["SNP"].tolist()
+        return p_values, sorted_p_values, sorted_snps
+
     def test_results_identical_with_fastlmmc(self):
         """
         make sure gwas yields same results as fastlmmC
         """
         if platform.system() == "Darwin":  # Don't run old C code on Mac
             return
 
@@ -139,15 +155,18 @@
         # REML IN lmm.py is BROKEN!!
 
         # we compare REML=False in lmm.py to fastlmmc
         REML = False
         gwas_c_reml = GwasTest(
             bed_fn, pheno_fn, snp_pos_sim, snp_pos_test, delta, REML=REML
         )
-        gwas_c_reml.run_gwas()
+        # cmk gwas_c_reml.run_gwas()
+        gwas_c_reml.p_values, gwas_c_reml.sorted_p_values, _ = TestGwas.read_results(
+            "out1.txt"
+        )
 
         gwas = GwasPrototype(G_chr1, G_chr2, y, delta, REML=False)
         gwas.run_gwas()
 
         # check p-values in log-space!
         np.testing.assert_array_almost_equal(
             np.log(gwas.p_values), np.log(gwas_c_reml.p_values), decimal=3
@@ -157,15 +176,16 @@
 
             pylab.plot(np.log(gwas_c_reml.p_values), np.log(gwas_f.p_values_F), "x")
             pylab.plot(list(range(-66, 0, 1)), list(range(-66, 0, 1)))
             pylab.show()
 
         # we compare lmm_cov.py to fastlmmc with REML=False
         gwas_c = GwasTest(bed_fn, pheno_fn, snp_pos_sim, snp_pos_test, delta, REML=True)
-        gwas_c.run_gwas()
+        # cmk gwas_c.run_gwas()
+        gwas_c.p_values, _, _ = TestGwas.read_results("out2.txt")
         gwas_f = FastGwas(G_chr1, G_chr2, y, delta, findh2=False)
         gwas_f.run_gwas()
         np.testing.assert_array_almost_equal(
             np.log(gwas_c.p_values), np.log(gwas_f.p_values_F), decimal=2
         )
 
         # additional testing code for the new wrapper functions
@@ -195,15 +215,18 @@
             gwas_f.sorted_p_values_F, gwas_c_reml.sorted_p_values, rtol=0.1
         )
 
         # Search over delta
         gwas_c_reml_search = GwasTest(
             bed_fn, pheno_fn, snp_pos_sim, snp_pos_test, delta=None, REML=True
         )
-        gwas_c_reml_search.run_gwas()
+        # cmk gwas_c_reml_search.run_gwas()
+        gwas_c_reml_search.p_values, gwas_c_reml_search.sorted_p_values, _ = (
+            TestGwas.read_results("out3.txt")
+        )
 
         frame_search = single_snp(
             test_snps=snpreader[:, idx_test],
             pheno=pheno_fn,
             G0=snpreader[:, idx_sim],
             h2=None,
             leave_out_one_chrom=False,
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/test_heritability_spatial_correction.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_heritability_spatial_correction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,123 +1,188 @@
-from __future__ import absolute_import
 import numpy as np
-import scipy as sp
 import logging
 import unittest
 import os.path
 import time
 import sys
 import doctest
 import pandas as pd
 import fastlmm.util.util as ut
-from fastlmm.association.heritability_spatial_correction import heritability_spatial_correction
+from fastlmm.association.heritability_spatial_correction import (
+    heritability_spatial_correction,
+)
 from pysnptools.util.mapreduce1.runner import Local, LocalMultiProc
 from pysnptools.snpreader import Dat, Bed, Pheno, SnpData
 from fastlmm.feature_selection.test import TestFeatureSelection
-from six.moves import range
+
 
 tolerance = 1e-4
 
 
 class TestHeritabilitySpatialCorrection(unittest.TestCase):
 
     @classmethod
     def setUpClass(self):
         from pysnptools.util import create_directory_if_necessary
+
         create_directory_if_necessary(self.tempout_dir, isfile=False)
-        self.pythonpath = os.path.abspath(os.path.join(os.path.dirname(os.path.realpath(__file__)),"..","..",".."))
-        self.snpreader_whole = Bed(self.pythonpath + "/tests/datasets/synth/all.bed",count_A1=False)
-        self.pheno_whole = Pheno(self.pythonpath + "/tests/datasets/synth/pheno_10_causals.txt")
+        self.pythonpath = os.path.abspath(
+            os.path.join(os.path.dirname(os.path.realpath(__file__)), "..", "..", "..")
+        )
+        self.snpreader_whole = Bed(
+            self.pythonpath + "/tests/datasets/synth/all.bed", count_A1=False
+        )
+        self.pheno_whole = Pheno(
+            self.pythonpath + "/tests/datasets/synth/pheno_10_causals.txt"
+        )
 
     tempout_dir = "tempout/heritability_spatial_correction"
 
-    def file_name(self,testcase_name):
-        temp_fn = os.path.join(self.tempout_dir,testcase_name)
+    def file_name(self, testcase_name):
+        temp_fn = os.path.join(self.tempout_dir, testcase_name)
         if os.path.exists(temp_fn):
             os.remove(temp_fn)
         return temp_fn
 
     def test_one(self):
-        '''
+        """
         Lock in results on arbitrary data -- because meaningful runs take too long to run.
-        '''
+        """
         fn = "one.txt"
         logging.info(fn)
         tmpOutfile = self.file_name(fn)
 
         half = self.pheno_whole.read().val
-        pheno = SnpData(iid=self.pheno_whole.iid,sid=["pheno0","pheno1"],val=np.c_[half,half])
-
-        spatial_coor = [[i,-i] for i in range(self.snpreader_whole.iid_count)]
-        alpha_list = alpha_list_big=[int(v) for v in np.logspace(2,np.log10(4000), 2)]
-        dataframe = heritability_spatial_correction(self.snpreader_whole,spatial_coor,self.snpreader_whole.iid,alpha_list,2,pheno,jackknife_count=2,permute_plus_count=1,permute_times_count=1,just_testing=True)
-
-        dataframe.to_csv(tmpOutfile,sep="\t",index=False)
-        referenceOutfile = TestFeatureSelection.reference_file("heritability_spatial_correction/"+fn)
-        out,msg=ut.compare_files(tmpOutfile, referenceOutfile, tolerance)                
-        self.assertTrue(out, "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile))
+        pheno = SnpData(
+            iid=self.pheno_whole.iid, sid=["pheno0", "pheno1"], val=np.c_[half, half]
+        )
+
+        spatial_coor = [[i, -i] for i in range(self.snpreader_whole.iid_count)]
+        alpha_list = alpha_list_big = [
+            int(v) for v in np.logspace(2, np.log10(4000), 2)
+        ]
+        dataframe = heritability_spatial_correction(
+            self.snpreader_whole,
+            spatial_coor,
+            self.snpreader_whole.iid,
+            alpha_list,
+            2,
+            pheno,
+            jackknife_count=2,
+            permute_plus_count=1,
+            permute_times_count=1,
+            just_testing=True,
+        )
+
+        dataframe.to_csv(tmpOutfile, sep="\t", index=False)
+        referenceOutfile = TestFeatureSelection.reference_file(
+            "heritability_spatial_correction/" + fn
+        )
+        out, msg = ut.compare_files(tmpOutfile, referenceOutfile, tolerance)
+        self.assertTrue(
+            out,
+            "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile),
+        )
 
     def test_two(self):
-        '''
+        """
         Lock in results on arbitrary data -- because meaningful runs take too long to run.
-        '''
+        """
         fn = "two.txt"
         logging.info(fn)
         tmpOutfile = self.file_name(fn)
 
-        snpreader = self.snpreader_whole[:10,:]
+        snpreader = self.snpreader_whole[:10, :]
 
-        spatial_coor = [[i,-i] for i in range(snpreader.iid_count)]
-        alpha_list = alpha_list_big=[int(v) for v in np.logspace(2,np.log10(4000), 2)]
-        dataframe = heritability_spatial_correction(snpreader,spatial_coor,snpreader.iid,alpha_list,2,self.pheno_whole,jackknife_count=2,permute_plus_count=1,permute_times_count=1,just_testing=False)
-
-        dataframe.to_csv(tmpOutfile,sep="\t",index=False)
-        referenceOutfile = TestFeatureSelection.reference_file("heritability_spatial_correction/"+fn)
-        out,msg=ut.compare_files(tmpOutfile, referenceOutfile, tolerance)                
-        self.assertTrue(out, "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile))
+        spatial_coor = [[i, -i] for i in range(snpreader.iid_count)]
+        alpha_list = alpha_list_big = [
+            int(v) for v in np.logspace(2, np.log10(4000), 2)
+        ]
+        dataframe = heritability_spatial_correction(
+            snpreader,
+            spatial_coor,
+            snpreader.iid,
+            alpha_list,
+            2,
+            self.pheno_whole,
+            jackknife_count=2,
+            permute_plus_count=1,
+            permute_times_count=1,
+            just_testing=False,
+        )
+
+        dataframe.to_csv(tmpOutfile, sep="\t", index=False)
+        referenceOutfile = TestFeatureSelection.reference_file(
+            "heritability_spatial_correction/" + fn
+        )
+        out, msg = ut.compare_files(tmpOutfile, referenceOutfile, tolerance)
+        self.assertTrue(
+            out,
+            "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile),
+        )
 
     def test_three(self):
-        '''
+        """
         Lock in results on arbitrary data -- because meaningful runs take too long to run.
-        '''
+        """
         fn = "three.txt"
         logging.info(fn)
         tmpOutfile = self.file_name(fn)
 
-        snpreader = self.snpreader_whole[:10,:]
+        snpreader = self.snpreader_whole[:10, :]
 
-        spatial_coor = [[i,-i] for i in range(snpreader.iid_count)]
-        alpha_list = alpha_list_big=[int(v) for v in np.logspace(2,np.log10(4000), 2)]
-        dataframe = heritability_spatial_correction(snpreader,spatial_coor,snpreader.iid,alpha_list,2,self.pheno_whole,jackknife_count=0,permute_plus_count=0,permute_times_count=0,just_testing=False)
-
-        dataframe.to_csv(tmpOutfile,sep="\t",index=False)
-        referenceOutfile = TestFeatureSelection.reference_file("heritability_spatial_correction/"+fn)
-        out,msg=ut.compare_files(tmpOutfile, referenceOutfile, tolerance)                
-        self.assertTrue(out, "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile))
+        spatial_coor = [[i, -i] for i in range(snpreader.iid_count)]
+        alpha_list = alpha_list_big = [
+            int(v) for v in np.logspace(2, np.log10(4000), 2)
+        ]
+        dataframe = heritability_spatial_correction(
+            snpreader,
+            spatial_coor,
+            snpreader.iid,
+            alpha_list,
+            2,
+            self.pheno_whole,
+            jackknife_count=0,
+            permute_plus_count=0,
+            permute_times_count=0,
+            just_testing=False,
+        )
+
+        dataframe.to_csv(tmpOutfile, sep="\t", index=False)
+        referenceOutfile = TestFeatureSelection.reference_file(
+            "heritability_spatial_correction/" + fn
+        )
+        out, msg = ut.compare_files(tmpOutfile, referenceOutfile, tolerance)
+        self.assertTrue(
+            out,
+            "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile),
+        )
 
     def test_doctest(self):
         old_dir = os.getcwd()
-        os.chdir(os.path.dirname(os.path.realpath(__file__))+"/..")
-        result = doctest.testmod(sys.modules['fastlmm.association.heritability_spatial_correction'])
+        os.chdir(os.path.dirname(os.path.realpath(__file__)) + "/..")
+        result = doctest.testmod(
+            sys.modules["fastlmm.association.heritability_spatial_correction"]
+        )
         os.chdir(old_dir)
         assert result.failed == 0, "failed doc test: " + __file__
 
 
-
 def getTestSuite():
-    
-    suite1 = unittest.TestLoader().loadTestsFromTestCase(TestHeritabilitySpatialCorrection)
-    return unittest.TestSuite([suite1])
 
+    suite1 = unittest.TestLoader().loadTestsFromTestCase(
+        TestHeritabilitySpatialCorrection
+    )
+    return unittest.TestSuite([suite1])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     logging.basicConfig(level=logging.DEBUG)
 
     # this import is needed for the runner
-    #from fastlmm.association.tests.test_heritability_spatical_correction import TestHeritabilitySpatialCorrection
+    # from fastlmm.association.tests.test_heritability_spatical_correction import TestHeritabilitySpatialCorrection
     suites = unittest.TestSuite([getTestSuite()])
 
     r = unittest.TextTestRunner(failfast=False)
     ret = r.run(suites)
     assert ret.wasSuccessful()
     logging.info("done with testing")
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/test_single_snp.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/test_single_snp_all_plus_select.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_all_plus_select.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/test_single_snp_linreg.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_linreg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,122 +1,136 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import sys
 import numpy as np
 import logging
 import unittest
 import os.path
 import doctest
 import pandas as pd
 import sys
 
 from fastlmm.association import single_snp
 from fastlmm.association import single_snp_linreg
 import pysnptools.util.pheno as pstpheno
 from fastlmm.feature_selection.test import TestFeatureSelection
 from pysnptools.util.mapreduce1.runner import Local, LocalMultiProc
-from pysnptools.kernelreader import  Identity as KernelIdentity
+from pysnptools.kernelreader import Identity as KernelIdentity
 from pysnptools.standardizer import Unit
 from pysnptools.snpreader import Bed, Pheno, SnpData
 from pysnptools.kernelreader import SnpKernel
 
 
 class TestSingleSnpLinReg(unittest.TestCase):
 
     @classmethod
     def setUpClass(self):
         from pysnptools.util import create_directory_if_necessary
+
         create_directory_if_necessary(self.tempout_dir, isfile=False)
-        self.pythonpath = os.path.abspath(os.path.join(os.path.dirname(os.path.realpath(__file__)),"..","..",".."))
-        self.bedbase = os.path.join(self.pythonpath, 'tests/datasets/all_chr.maf0.001.N300')
-        self.phen_fn = os.path.join(self.pythonpath, 'tests/datasets/phenSynthFrom22.23.N300.randcidorder.txt')
-        self.cov_fn = os.path.join(self.pythonpath,  'tests/datasets/all_chr.maf0.001.covariates.N300.txt')
+        self.pythonpath = os.path.abspath(
+            os.path.join(os.path.dirname(os.path.realpath(__file__)), "..", "..", "..")
+        )
+        self.bedbase = os.path.join(
+            self.pythonpath, "tests/datasets/all_chr.maf0.001.N300"
+        )
+        self.phen_fn = os.path.join(
+            self.pythonpath, "tests/datasets/phenSynthFrom22.23.N300.randcidorder.txt"
+        )
+        self.cov_fn = os.path.join(
+            self.pythonpath, "tests/datasets/all_chr.maf0.001.covariates.N300.txt"
+        )
 
     tempout_dir = "tempout/single_snp_linreg"
 
-    def file_name(self,testcase_name):
-        temp_fn = os.path.join(self.tempout_dir,testcase_name+".txt")
+    def file_name(self, testcase_name):
+        temp_fn = os.path.join(self.tempout_dir, testcase_name + ".txt")
         if os.path.exists(temp_fn):
             os.remove(temp_fn)
         return temp_fn
 
     def test_linreg(self):
         logging.info("TestSingleSnpLinReg test_linreg")
-        test_snps = Bed(self.bedbase,count_A1=False)
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
         covar = self.cov_fn
 
         output_file = self.file_name("linreg")
 
-        frame1 = single_snp_linreg(test_snps=test_snps[:,:10], pheno=pheno,
-                                    covar=covar, 
-                                    output_file_name=output_file,
-                                    count_A1=False
-                                    )
-
-        frame1 = frame1[['sid_index', 'SNP', 'Chr', 'GenDist', 'ChrPos', 'PValue']]
-        self.compare_files(frame1,"linreg")
-
-        frame2 = single_snp_linreg(test_snps=test_snps[:,:10], pheno=pheno, 
-                                    covar=covar, 
-                                    output_file_name=output_file,count_A1=False
-                                    )
-        self.compare_files(frame2,"linreg")
+        frame1 = single_snp_linreg(
+            test_snps=test_snps[:, :10],
+            pheno=pheno,
+            covar=covar,
+            output_file_name=output_file,
+            count_A1=False,
+        )
+
+        frame1 = frame1[["sid_index", "SNP", "Chr", "GenDist", "ChrPos", "PValue"]]
+        self.compare_files(frame1, "linreg")
+
+        frame2 = single_snp_linreg(
+            test_snps=test_snps[:, :10],
+            pheno=pheno,
+            covar=covar,
+            output_file_name=output_file,
+            count_A1=False,
+        )
+        self.compare_files(frame2, "linreg")
+
+    def compare_files(self, frame, ref_base):
+        reffile = TestFeatureSelection.reference_file(
+            "single_snp/" + ref_base + ".txt"
+        )  # Results are in single_snp, not single_snp_lin_reg
 
+        # sid_list,pvalue_list = frame['SNP'].values,frame['Pvalue'].values
 
-    def compare_files(self,frame,ref_base):
-        reffile = TestFeatureSelection.reference_file("single_snp/"+ref_base+".txt") #Results are in single_snp, not single_snp_lin_reg
-
-        #sid_list,pvalue_list = frame['SNP'].values,frame['Pvalue'].values
-
-        #sid_to_pvalue = {}
-        #for index, sid in enumerate(sid_list):
+        # sid_to_pvalue = {}
+        # for index, sid in enumerate(sid_list):
         #    sid_to_pvalue[sid] = pvalue_list[index]
 
-        reference=pd.read_csv(reffile,delimiter='\s',comment=None,engine='python')
-        assert len(frame) == len(reference), "# of pairs differs from file '{0}'".format(reffile)
+        reference = pd.read_csv(reffile, delimiter="\s", comment=None, engine="python")
+        assert len(frame) == len(
+            reference
+        ), "# of pairs differs from file '{0}'".format(reffile)
         for _, row in reference.iterrows():
             sid = row.SNP
-            pvalue = frame[frame['SNP'] == sid].iloc[0].PValue
-            assert abs(row.PValue - pvalue) < 1e-5, "pair {0} differs too much from file '{1}'".format(sid,reffile)
+            pvalue = frame[frame["SNP"] == sid].iloc[0].PValue
+            assert (
+                abs(row.PValue - pvalue) < 1e-5
+            ), "pair {0} differs too much from file '{1}'".format(sid, reffile)
 
     def test_doctest(self):
         old_dir = os.getcwd()
-        os.chdir(os.path.dirname(os.path.realpath(__file__))+"/..")
-        result = doctest.testmod(sys.modules['fastlmm.association.single_snp_linreg'])
+        os.chdir(os.path.dirname(os.path.realpath(__file__)) + "/..")
+        result = doctest.testmod(sys.modules["fastlmm.association.single_snp_linreg"])
         os.chdir(old_dir)
         assert result.failed == 0, "failed doc test: " + __file__
 
 
 def getTestSuite():
-    
 
     suite1 = unittest.TestLoader().loadTestsFromTestCase(TestSingleSnpLinReg)
     return unittest.TestSuite([suite1])
 
 
-
-if __name__ == '__main__':
-
-
+if __name__ == "__main__":
 
     # this import is needed for the runner
     from fastlmm.association.tests.test_single_snp_linreg import TestSingleSnpLinReg
+
     suites = unittest.TestSuite([getTestSuite()])
 
-    if True: #Standard test run
+    if True:  # Standard test run
         r = unittest.TextTestRunner(failfast=False)
         ret = r.run(suites)
         assert ret.wasSuccessful()
-    else: #Cluster test run
+    else:  # Cluster test run
         logging.basicConfig(level=logging.INFO)
 
         from pysnptools.util.mapreduce1.distributabletest import DistributableTest
+
         runner = Local()
-        #runner = LocalMultiProc(taskcount=20,mkl_num_threads=5)
-        #runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
-        #runner = Hadoop(100, mapmemory=8*1024, reducememory=8*1024, mkl_num_threads=1, queue="default")
-        distributable_test = DistributableTest(suites,"temp_test")
+        # runner = LocalMultiProc(taskcount=20,mkl_num_threads=5)
+        # runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
+        # runner = Hadoop(100, mapmemory=8*1024, reducememory=8*1024, mkl_num_threads=1, queue="default")
+        distributable_test = DistributableTest(suites, "temp_test")
         print(runner.run(distributable_test))
 
-
     logging.info("done with testing")
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/test_single_snp_scale.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_scale.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
                 pvalue_reference = np.array(
                     sorted(reference[reference["SNP"] == sid].PValue)
                 )
                 assert (
                     abs(pvalue_frame - pvalue_reference) < 1e-5
                 ).all, "pair {0} differs too much from reference".format(sid)
 
-    def test_local_distribute(self):
+    def test_local_distribute(self):  # cmk
         logging.info("test_local_distribute")
         force_python_only = False
 
         output_file = self.file_name("local_distribute")
 
         storage = LocalCache("local_cache/local_distribute")
         test_storage = storage.join("test_snps")
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/test_single_snp_select.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_select.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,209 +1,282 @@
-from __future__ import absolute_import
-from __future__ import print_function
-#import matplotlib
-#matplotlib.use("TKAgg",warn=False)
-#import pylab
+# import matplotlib
+# matplotlib.use("TKAgg",warn=False)
+# import pylab
 import pandas as pd
 import sys
 
 import numpy as np
 import logging
 import unittest
 import doctest
 import os.path
-from pysnptools.snpreader import Bed, Pheno,SnpData
+from pysnptools.snpreader import Bed, Pheno, SnpData
 from fastlmm.association import single_snp_select
 from fastlmm.feature_selection.test import TestFeatureSelection
 import platform
 import multiprocessing
 from pysnptools.util.mapreduce1.runner import LocalMultiProc
 
 
-class TestSingleSnpSelect(unittest.TestCase): 
+class TestSingleSnpSelect(unittest.TestCase):
 
     @classmethod
     def setUpClass(self):
         from pysnptools.util import create_directory_if_necessary
+
         create_directory_if_necessary(self.tempout_dir, isfile=False)
-        self.pythonpath = os.path.abspath(os.path.join(os.path.dirname(os.path.realpath(__file__)),"..","..",".."))
-        self.bedbase = os.path.join(self.pythonpath, 'tests/datasets/all_chr.maf0.001.N300')
-        self.phen_fn = os.path.join(self.pythonpath, 'tests/datasets/phenSynthFrom22.23.N300.randcidorder.txt')
-        self.cov_fn = os.path.join(self.pythonpath,  'tests/datasets/all_chr.maf0.001.covariates.N300.txt')
+        self.pythonpath = os.path.abspath(
+            os.path.join(os.path.dirname(os.path.realpath(__file__)), "..", "..", "..")
+        )
+        self.bedbase = os.path.join(
+            self.pythonpath, "tests/datasets/all_chr.maf0.001.N300"
+        )
+        self.phen_fn = os.path.join(
+            self.pythonpath, "tests/datasets/phenSynthFrom22.23.N300.randcidorder.txt"
+        )
+        self.cov_fn = os.path.join(
+            self.pythonpath, "tests/datasets/all_chr.maf0.001.covariates.N300.txt"
+        )
 
     tempout_dir = "tempout/single_snp_select"
 
-    def file_name(self,testcase_name):
-        temp_fn = os.path.join(self.tempout_dir,testcase_name+".txt")
+    def file_name(self, testcase_name):
+        temp_fn = os.path.join(self.tempout_dir, testcase_name + ".txt")
         if os.path.exists(temp_fn):
             os.remove(temp_fn)
         return temp_fn
 
-    #Break these tests up into six parts so they can run faster when on cluster.
-    def test_sel_plus_pc_h2Search(self): #!!! rather a big test case
+    # Break these tests up into six parts so they can run faster when on cluster.
+    def test_sel_plus_pc_h2Search(self):  #!!! rather a big test case
         logging.info("TestSingleSnpSelect sel_plus_pc_h2Search")
-        self._sel_plus_pc(None,None,None,count_A1=False)
+        self._sel_plus_pc(None, None, None, count_A1=False)
 
-    def test_sel_plus_pc_h2Search_low(self): #!!! rather a big test case
+    def test_sel_plus_pc_h2Search_low(self):  #!!! rather a big test case
         logging.info("TestSingleSnpSelect sel_plus_pc_h2Search_low")
-        self._sel_plus_pc(None,True,False,count_A1=False)
+        self._sel_plus_pc(None, True, False, count_A1=False)
 
-    def test_sel_plus_pc_h2Search_full(self): #!!! rather a big test case
+    def test_sel_plus_pc_h2Search_full(self):  #!!! rather a big test case
         logging.info("TestSingleSnpSelect sel_plus_pc_h2Search_full")
-        self._sel_plus_pc(None,False,True,count_A1=False)
+        self._sel_plus_pc(None, False, True, count_A1=False)
 
-    def test_sel_plus_pc_h2IsHalf(self): #!!! rather a big test case
+    def test_sel_plus_pc_h2IsHalf(self):  #!!! rather a big test case
         logging.info("TestSingleSnpSelect sel_plus_pc_h2IsHalf")
-        self._sel_plus_pc(.5,None,None,count_A1=False)
+        self._sel_plus_pc(0.5, None, None, count_A1=False)
 
-    def test_sel_plus_pc_h2IsHalf_low(self): #!!! rather a big test case
+    def test_sel_plus_pc_h2IsHalf_low(self):  #!!! rather a big test case
         logging.info("TestSingleSnpSelect sel_plus_pc_h2IsHalf_low")
-        self._sel_plus_pc(.5,True,False,count_A1=False)
+        self._sel_plus_pc(0.5, True, False, count_A1=False)
 
-    def test_sel_plus_pc_h2IsHalf_full(self): #!!! rather a big test case
+    def test_sel_plus_pc_h2IsHalf_full(self):  #!!! rather a big test case
         logging.info("TestSingleSnpSelect sel_plus_pc_h2IsHalf_full")
-        self._sel_plus_pc(.5,False,True,count_A1=False)
+        self._sel_plus_pc(0.5, False, True, count_A1=False)
 
-    def _sel_plus_pc(self,h2,force_low_rank,force_full_rank,count_A1=None):
+    def _sel_plus_pc(self, h2, force_low_rank, force_full_rank, count_A1=None):
         do_plot = False
         use_cache = False
 
         # define file names
         bed_fn = self.pythonpath + "/tests/datasets/synth/all.bed"
         phen_fn = self.pythonpath + "/tests/datasets/synth/pheno_10_causals.txt"
 
-        pcs_fn = os.path.join(self.tempout_dir,"sel_plus_pc.pcs.txt")
+        pcs_fn = os.path.join(self.tempout_dir, "sel_plus_pc.pcs.txt")
         if not (use_cache and os.path.exists(pcs_fn)):
             from fastlmm.util import compute_auto_pcs
-            covar = compute_auto_pcs(bed_fn,count_A1=count_A1)
+
+            covar = compute_auto_pcs(bed_fn, count_A1=count_A1)
             logging.info("selected number of PCs: {0}".format(covar["vals"].shape[1]))
-            Pheno.write(pcs_fn,SnpData(iid=covar['iid'],sid=covar['header'],val=covar['vals']))
+            Pheno.write(
+                pcs_fn,
+                SnpData(iid=covar["iid"], sid=covar["header"], val=covar["vals"]),
+            )
         else:
             logging.info("Using top pcs's cache")
-            covar=Pheno(pcs_fn)
+            covar = Pheno(pcs_fn)
 
-        runner = LocalMultiProc(multiprocessing.cpu_count(),mkl_num_threads=2)
+        runner = LocalMultiProc(multiprocessing.cpu_count(), mkl_num_threads=2)
 
-        logging.info("Working on h2={0},force_low_rank={1},force_full_rank={2}".format(h2,force_low_rank,force_full_rank))
-        result_file_name = "sel_plus_pc_{0}".format("h2IsHalf" if h2 == .5 else "h2Search")
-        output_file_name = os.path.join(self.tempout_dir,result_file_name)+".txt"
-        results = single_snp_select(test_snps=bed_fn, G=bed_fn, pheno=phen_fn,
-                                        k_list = [0,1,2,3,4,5,6,7,8,9,10,20,30,40,50,60,70,80,90,100,125,160,200,250,320,400,500,630,800,1000],
-                                        h2=h2,
-                                        n_folds = self.pythonpath + "/tests/datasets/synth/DebugEmitFolds.txt",
-                                        covar=covar,
-                                        output_file_name=output_file_name,
-                                        force_low_rank=force_low_rank,force_full_rank=force_full_rank,
-                                        GB_goal=2,
-                                        count_A1=False
-                                        #runner = runner
-                                    )
+        logging.info(
+            "Working on h2={0},force_low_rank={1},force_full_rank={2}".format(
+                h2, force_low_rank, force_full_rank
+            )
+        )
+        result_file_name = "sel_plus_pc_{0}".format(
+            "h2IsHalf" if h2 == 0.5 else "h2Search"
+        )
+        output_file_name = os.path.join(self.tempout_dir, result_file_name) + ".txt"
+        results = single_snp_select(
+            test_snps=bed_fn,
+            G=bed_fn,
+            pheno=phen_fn,
+            k_list=[
+                0,
+                1,
+                2,
+                3,
+                4,
+                5,
+                6,
+                7,
+                8,
+                9,
+                10,
+                20,
+                30,
+                40,
+                50,
+                60,
+                70,
+                80,
+                90,
+                100,
+                125,
+                160,
+                200,
+                250,
+                320,
+                400,
+                500,
+                630,
+                800,
+                1000,
+            ],
+            h2=h2,
+            n_folds=self.pythonpath + "/tests/datasets/synth/DebugEmitFolds.txt",
+            covar=covar,
+            output_file_name=output_file_name,
+            force_low_rank=force_low_rank,
+            force_full_rank=force_full_rank,
+            GB_goal=2,
+            count_A1=False,
+            # runner = runner
+        )
         logging.info(results.head())
-        self.compare_files(results,result_file_name)
-
+        self.compare_files(results, result_file_name)
 
-    def test_old_sel_plus_pc(self): #!!! rather a big test case
-        if platform.system() == "Darwin": #Don't run old C code on Mac
+    def test_old_sel_plus_pc(self):  #!!! rather a big test case
+        if platform.system() == "Darwin":  # Don't run old C code on Mac
             return
 
         logging.info("TestSingleSnpSelect old_sel_plus_pc")
 
         from pysnptools.snpreader import Bed
         from fastlmm.util import compute_auto_pcs
 
         # define file names
         bed_fn = self.pythonpath + "/tests/datasets/synth/all"
         cov_fn = "pcs_cov.txt"
 
         # run PCgeno
-        #TODO: rename to auto_pcs
-        result = compute_auto_pcs(bed_fn, output_file_name=cov_fn,count_A1=False)
+        # TODO: rename to auto_pcs
+        result = compute_auto_pcs(bed_fn, output_file_name=cov_fn, count_A1=False)
         logging.info("selected number of PCs: {0}".format(result["vals"].shape[1]))
 
         # import algorithms
         from fastlmm.util.run_fastlmmc import runFASTLMM, runLMMSELECT
 
         # set some file paths for fastlmmc
         phen_fn = self.pythonpath + "/tests/datasets/synth/pheno_10_causals.txt"
         out_dir = self.tempout_dir
         fastlmm_path = self.pythonpath + "/external/fastlmmc"
 
         # consists of two fastlmmc calls, one that does feature selection and one that runs GWAS
-        for suffix,logdelta in [("h2IsHalf",0),("h2Search",None)]:
-            result_file_name = "sel_plus_pc_old_{0}".format("h2IsHalf" if logdelta == 0 else "h2Search")
-            runLMMSELECT(bed_fn, phen_fn, out_dir, result_file_name, bfileSim=bed_fn, covar=cov_fn, fastlmm_path=fastlmm_path,autoSelectCriterionMSE=False,excludeByGeneticDistance=1000,optLogdelta=logdelta)
+        for suffix, logdelta in [("h2IsHalf", 0), ("h2Search", None)]:
+            result_file_name = "sel_plus_pc_old_{0}".format(
+                "h2IsHalf" if logdelta == 0 else "h2Search"
+            )
+            runLMMSELECT(
+                bed_fn,
+                phen_fn,
+                out_dir,
+                result_file_name,
+                bfileSim=bed_fn,
+                covar=cov_fn,
+                fastlmm_path=fastlmm_path,
+                autoSelectCriterionMSE=False,
+                excludeByGeneticDistance=1000,
+                optLogdelta=logdelta,
+            )
             # compare sel_plus_pc_old_h2*.LMMSELECT.out.txt
-            short = result_file_name+".LMMSELECT.out"
-            results=pd.read_csv(self.tempout_dir+"/"+short+".txt",delimiter='\s',comment=None,engine='python')
-            results['PValue']=results.Pvalue #add a new column with different capitalization
-            self.compare_files(results,short)
-
-
+            short = result_file_name + ".LMMSELECT.out"
+            results = pd.read_csv(
+                self.tempout_dir + "/" + short + ".txt",
+                delimiter="\s",
+                comment=None,
+                engine="python",
+            )
+            results["PValue"] = (
+                results.Pvalue
+            )  # add a new column with different capitalization
+            self.compare_files(results, short)
+
+    def compare_files(self, frame, ref_base):
+        reffile = TestFeatureSelection.reference_file(
+            "single_snp_select/" + ref_base + ".txt"
+        )
 
-    def compare_files(self,frame,ref_base):
-        reffile = TestFeatureSelection.reference_file("single_snp_select/"+ref_base+".txt")
+        # sid_list,pvalue_list = frame['SNP'].values,frame['Pvalue'].values
 
-        #sid_list,pvalue_list = frame['SNP'].values,frame['Pvalue'].values
-
-        #sid_to_pvalue = {}
-        #for index, sid in enumerate(sid_list):
+        # sid_to_pvalue = {}
+        # for index, sid in enumerate(sid_list):
         #    sid_to_pvalue[sid] = pvalue_list[index]
 
-        reference=pd.read_csv(reffile,delimiter='\s',comment=None,engine='python')
-        if 'Pvalue' in reference.columns: reference['PValue']=reference.Pvalue #add a new column with different capitalization if it is there
-
-
-        assert len(frame) == len(reference), "# of pairs differs from file '{0}'".format(reffile)
+        reference = pd.read_csv(reffile, delimiter="\s", comment=None, engine="python")
+        if "Pvalue" in reference.columns:
+            reference["PValue"] = (
+                reference.Pvalue
+            )  # add a new column with different capitalization if it is there
+
+        assert len(frame) == len(
+            reference
+        ), "# of pairs differs from file '{0}'".format(reffile)
         for _, row in reference.iterrows():
             sid = row.SNP
-            pvalue = frame[frame['SNP'] == sid].iloc[0].PValue
-            assert abs(row.PValue - pvalue) < 1e-5, "pair {0} differs too much from file '{1}'".format(sid,reffile)
+            pvalue = frame[frame["SNP"] == sid].iloc[0].PValue
+            assert (
+                abs(row.PValue - pvalue) < 1e-5
+            ), "pair {0} differs too much from file '{1}'".format(sid, reffile)
 
     def test_doctest(self):
         old_dir = os.getcwd()
-        os.chdir(os.path.dirname(os.path.realpath(__file__))+"/..")
-        result = doctest.testmod(sys.modules['fastlmm.association.single_snp_select'])
+        os.chdir(os.path.dirname(os.path.realpath(__file__)) + "/..")
+        result = doctest.testmod(sys.modules["fastlmm.association.single_snp_select"])
         os.chdir(old_dir)
         assert result.failed == 0, "failed doc test: " + __file__
 
 
-
 def getTestSuite():
-    
+
     suite1 = unittest.TestLoader().loadTestsFromTestCase(TestSingleSnpSelect)
     return unittest.TestSuite([suite1])
 
 
-
-if __name__ == '__main__':
+if __name__ == "__main__":
 
     # this import is needed for the runner
     from fastlmm.association.tests.test_single_snp_select import TestSingleSnpSelect
+
     suites = unittest.TestSuite([getTestSuite()])
 
-    if True: #Standard test run
+    if True:  # Standard test run
         r = unittest.TextTestRunner(failfast=False)
         ret = r.run(suites)
         assert ret.wasSuccessful()
-    else: #Cluster test run
-
-
+    else:  # Cluster test run
 
         from pysnptools.util.mapreduce1.runner import Local, LocalMultiProc
+
         logging.basicConfig(level=logging.INFO)
 
         from pysnptools.util.mapreduce1.distributabletest import DistributableTest
 
-
-        #runner = HPC(10, 'RR1-N13-09-H44',r'\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\Redmond',
+        # runner = HPC(10, 'RR1-N13-09-H44',r'\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\Redmond',
         #                remote_python_parent=r"\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\REDMOND\carlk\Source\carlk\july_7_14\tests\runs\2014-07-24_15_02_02_554725991686\pythonpath",
         #                update_remote_python_parent=True,
         #                priority="AboveNormal",mkl_num_threads=1)
         runner = Local()
-        #runner = LocalMultiProc(taskcount=20,mkl_num_threads=5)
-        #runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
-        #runner = Hadoop(100, mapmemory=8*1024, reducememory=8*1024, mkl_num_threads=1, queue="default")
-        distributable_test = DistributableTest(suites,"temp_test")
+        # runner = LocalMultiProc(taskcount=20,mkl_num_threads=5)
+        # runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
+        # runner = Hadoop(100, mapmemory=8*1024, reducememory=8*1024, mkl_num_threads=1, queue="default")
+        distributable_test = DistributableTest(suites, "temp_test")
         print(runner.run(distributable_test))
 
-
     logging.info("done with testing")
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/test_snp_set.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_snp_set.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import numpy as np
-import scipy as sp
 import logging
 import unittest
 import os.path
 import time
 import sys
 import doctest
 import pandas as pd
@@ -23,159 +20,215 @@
 
     #!!created a Expect Durbin, too
 
     @classmethod
     def setUpClass(self):
 
         from pysnptools.util import create_directory_if_necessary
+
         create_directory_if_necessary(self.tempout_dir, isfile=False)
         self.currentFolder = os.path.dirname(os.path.realpath(__file__))
 
     tempout_dir = "tempout/snp_set"
- 
-    def file_name(self,testcase_name):
-        temp_fn = os.path.join(self.tempout_dir,testcase_name)
+
+    def file_name(self, testcase_name):
+        temp_fn = os.path.join(self.tempout_dir, testcase_name)
         if os.path.exists(temp_fn):
             os.remove(temp_fn)
         return temp_fn
 
     def test_one(self):
         logging.info("TestSnpSet test_one")
 
         fn = "lrt_one_kernel_fixed_mixed_effect_linear_qqfit.N300.txt"
         tmpOutfile = self.file_name(fn)
         referenceOutfile = self._referenceOutfile(fn)
 
         result_dataframe = snp_set(
-            test_snps = self.currentFolder+'/../../../tests/datasets/all_chr.maf0.001.N300',
-            set_list = self.currentFolder+'/../../../tests/datasets/set_input.23.txt',
-            pheno = self.currentFolder+'/../../../tests/datasets/phenSynthFrom22.23.N300.txt',
-            output_file_name = tmpOutfile
-            )
-
-
-        out,msg=ut.compare_files(tmpOutfile, referenceOutfile, tolerance)                
-        self.assertTrue(out, "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile))
+            test_snps=self.currentFolder
+            + "/../../../tests/datasets/all_chr.maf0.001.N300",
+            set_list=self.currentFolder + "/../../../tests/datasets/set_input.23.txt",
+            pheno=self.currentFolder
+            + "/../../../tests/datasets/phenSynthFrom22.23.N300.txt",
+            output_file_name=tmpOutfile,
+        )
+
+        out, msg = ut.compare_files(tmpOutfile, referenceOutfile, tolerance)
+        self.assertTrue(
+            out,
+            "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile),
+        )
 
     def test_two(self):
         logging.info("TestSnpSet test_two")
 
         fn = "lrt_up_two_kernel_mixed_effect_linear_qqfit.N300.fullrank.txt"
         tmpOutfile = self.file_name(fn)
         referenceOutfile = self._referenceOutfile(fn)
 
         result_dataframe = snp_set(
-            test_snps = self.currentFolder+'/../../../tests/datasets/all_chr.maf0.001.N300',
-            set_list = self.currentFolder+'/../../../tests/datasets/set_input.23.txt',
-            pheno = self.currentFolder+'/../../../tests/datasets/phenSynthFrom22.23.N300.txt',
-            G0 = self.currentFolder+'/../../../tests/datasets/all_chr.maf0.001.chr22.23.N300.bed',
-            output_file_name = tmpOutfile,
-            test="lrt"
-            )
-
-
-        out,msg=ut.compare_files(tmpOutfile, referenceOutfile, tolerance)                
-        self.assertTrue(out,msg)#msg='Files %s and %s are different.' % (tmpOutfile, referenceOutfile))
-
+            test_snps=self.currentFolder
+            + "/../../../tests/datasets/all_chr.maf0.001.N300",
+            set_list=self.currentFolder + "/../../../tests/datasets/set_input.23.txt",
+            pheno=self.currentFolder
+            + "/../../../tests/datasets/phenSynthFrom22.23.N300.txt",
+            G0=self.currentFolder
+            + "/../../../tests/datasets/all_chr.maf0.001.chr22.23.N300.bed",
+            output_file_name=tmpOutfile,
+            test="lrt",
+        )
+
+        out, msg = ut.compare_files(tmpOutfile, referenceOutfile, tolerance)
+        self.assertTrue(
+            out, msg
+        )  # msg='Files %s and %s are different.' % (tmpOutfile, referenceOutfile))
 
     def test_three(self):
         logging.info("TestSnpSet test_three")
 
         fn = "sc_davies_one_kernel_linear_qqfit.N300.txt"
         tmpOutfile = self.file_name(fn)
         referenceOutfile = self._referenceOutfile(fn)
 
         result_dataframe = snp_set(
-            test_snps = self.currentFolder+'/../../../tests/datasets/all_chr.maf0.001.N300',
-            set_list = self.currentFolder+'/../../../tests/datasets/set_input.small.txt',
-            pheno = self.currentFolder+'/../../../tests/datasets/phenSynthFrom22.23.N300.txt',
-            test = "sc_davies",
-            output_file_name = tmpOutfile
-            )
-
-
-        out,msg=ut.compare_files(tmpOutfile, referenceOutfile, tolerance)                
-        self.assertTrue(out, "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile))
-
+            test_snps=self.currentFolder
+            + "/../../../tests/datasets/all_chr.maf0.001.N300",
+            set_list=self.currentFolder
+            + "/../../../tests/datasets/set_input.small.txt",
+            pheno=self.currentFolder
+            + "/../../../tests/datasets/phenSynthFrom22.23.N300.txt",
+            test="sc_davies",
+            output_file_name=tmpOutfile,
+        )
+
+        out, msg = ut.compare_files(tmpOutfile, referenceOutfile, tolerance)
+        self.assertTrue(
+            out,
+            "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile),
+        )
 
     def test_four(self):
         logging.info("TestSnpSet test_four")
 
         fn = "sc_davies_two_kernel_linear_qqfit.N300.noautoselect.txt"
         tmpOutfile = self.file_name(fn)
         referenceOutfile = self._referenceOutfile(fn)
 
         result_dataframe = snp_set(
-            test_snps = self.currentFolder+'/../../../tests/datasets/all_chr.maf0.001.N300',
-            set_list = self.currentFolder+'/../../../tests/datasets/set_input.small.txt',
-            pheno = self.currentFolder+'/../../../tests/datasets/phenSynthFrom22.23.N300.randcidorder.txt',
-            G0 = self.currentFolder+'/../../../tests/datasets/all_chr.maf0.001.chr22.23.N300.bed',
-            test = 'sc_davies',
-            output_file_name = tmpOutfile
-            )
-
-
-        out,msg=ut.compare_files(tmpOutfile, referenceOutfile, tolerance)                
-        self.assertTrue(out, "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile))
+            test_snps=self.currentFolder
+            + "/../../../tests/datasets/all_chr.maf0.001.N300",
+            set_list=self.currentFolder
+            + "/../../../tests/datasets/set_input.small.txt",
+            pheno=self.currentFolder
+            + "/../../../tests/datasets/phenSynthFrom22.23.N300.randcidorder.txt",
+            G0=self.currentFolder
+            + "/../../../tests/datasets/all_chr.maf0.001.chr22.23.N300.bed",
+            test="sc_davies",
+            output_file_name=tmpOutfile,
+        )
+
+        out, msg = ut.compare_files(tmpOutfile, referenceOutfile, tolerance)
+        self.assertTrue(
+            out,
+            "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile),
+        )
+
+    def test_notebook(self):
+        # define file names
+        test_snps_fn = self.currentFolder + "/../../../tests/datasets/synth/chr1"
+        pheno_fn = (
+            self.currentFolder + "/../../../tests/datasets/synth/pheno_10_causals.txt"
+        )
+        cov_fn = self.currentFolder + "/../../../tests/datasets/synth/cov.txt"
+        set_list_fn = (
+            self.currentFolder + "/../../../tests/datasets/synth/chr1.sets.txt"
+        )
+        G0_fn = None
+
+        # run SNP-set analysis
+        results_df = snp_set(
+            test_snps=test_snps_fn,
+            G0=G0_fn,
+            set_list=set_list_fn,
+            pheno=pheno_fn,
+            covar=cov_fn,
+            test="lrt",
+        )
+        top = results_df.iloc[0]
+        logging.debug(top)
+        assert top["SetId"] == "set_65"
+        assert np.abs(top["P-value"] - 0.002564) < 0.0001
 
     def test_doctest(self):
         old_dir = os.getcwd()
-        os.chdir(os.path.dirname(os.path.realpath(__file__))+"/..")
-        result = doctest.testmod(sys.modules['fastlmm.association.snp_set'])
+        os.chdir(os.path.dirname(os.path.realpath(__file__)) + "/..")
+        result = doctest.testmod(sys.modules["fastlmm.association.snp_set"])
         os.chdir(old_dir)
         assert result.failed == 0, "failed doc test: " + __file__
 
+    def _referenceOutfile(self, _infile):
+        import platform
 
-    def _referenceOutfile(self,_infile):
-        import platform;
-        os_string=platform.platform()
+        os_string = platform.platform()
         outfile = os.path.splitext(_infile)[0]
 
-        windows_fn = self.currentFolder+'/../../../tests/expected-Windows/'+outfile+'.txt'
+        windows_fn = (
+            self.currentFolder + "/../../../tests/expected-Windows/" + outfile + ".txt"
+        )
         assert os.path.exists(windows_fn), "Can't find file '{0}'".format(windows_fn)
-        debian_fn = self.currentFolder+'/../../../tests/expected-debian/'+outfile  +'.txt'
-        if not os.path.exists(debian_fn): #If reference file is not in debian folder, look in windows folder
+        debian_fn = (
+            self.currentFolder + "/../../../tests/expected-debian/" + outfile + ".txt"
+        )
+        if not os.path.exists(
+            debian_fn
+        ):  # If reference file is not in debian folder, look in windows folder
             debian_fn = windows_fn
 
         if "debian" in os_string or "Linux" in os_string:
             if "Linux" in os_string:
-                logging.warning("comparing to Debian output even though found: %s" % os_string)
+                logging.warning(
+                    "comparing to Debian output even though found: %s" % os_string
+                )
             return debian_fn
         else:
             if "Windows" not in os_string:
-                logging.warning("comparing to Windows output even though found: %s" % os_string)
-            return windows_fn 
+                logging.warning(
+                    "comparing to Windows output even though found: %s" % os_string
+                )
+            return windows_fn
 
 
 def getTestSuite():
-    
 
     suite1 = unittest.TestLoader().loadTestsFromTestCase(TestSnpSet)
     return unittest.TestSuite([suite1])
 
 
-
-if __name__ == '__main__':    
+if __name__ == "__main__":
     from fastlmm.association.tests.test_snp_set import TestSnpSet
+
     suites = unittest.TestSuite([getTestSuite()])
 
-    if True: #Standard test run
+    if True:  # Standard test run
         r = unittest.TextTestRunner(failfast=False)
         ret = r.run(suites)
         assert ret.wasSuccessful()
-    else: #Cluster test run
+    else:  # Cluster test run
         from pysnptools.util.mapreduce1.distributabletest import DistributableTest
 
-
-        runner = HPC(10, 'RR1-N13-09-H44',r'\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\Redmond',
-                     remote_python_parent=r"\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\REDMOND\carlk\Source\carlk\july_7_14\tests\runs\2014-07-24_15_02_02_554725991686\pythonpath",
-                     update_remote_python_parent=True,
-                     priority="AboveNormal",mkl_num_threads=1)
+        runner = HPC(
+            10,
+            "RR1-N13-09-H44",
+            r"\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\Redmond",
+            remote_python_parent=r"\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\REDMOND\carlk\Source\carlk\july_7_14\tests\runs\2014-07-24_15_02_02_554725991686\pythonpath",
+            update_remote_python_parent=True,
+            priority="AboveNormal",
+            mkl_num_threads=1,
+        )
         runner = Local()
-        #runner = LocalMultiProc(taskcount=20,mkl_num_threads=5)
-        #runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
-        #runner = Hadoop(100, mapmemory=8*1024, reducememory=8*1024, mkl_num_threads=1, queue="default")
-        distributable_test = DistributableTest(suites,"temp_test")
+        # runner = LocalMultiProc(taskcount=20,mkl_num_threads=5)
+        # runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
+        # runner = Hadoop(100, mapmemory=8*1024, reducememory=8*1024, mkl_num_threads=1, queue="default")
+        distributable_test = DistributableTest(suites, "temp_test")
         print(runner.run(distributable_test))
 
-
     logging.info("done with testing")
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/testepistasis.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/testepistasis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,302 +1,461 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import numpy as np
-import scipy as sp
 import logging
 import unittest
 import os.path
 import time
 import sys
 import doctest
 
 from fastlmm.association import epistasis
 from fastlmm.association.epistasis import write
 import fastlmm.pyplink.plink as plink
 import pysnptools.util.pheno as pstpheno
 from fastlmm.feature_selection.test import TestFeatureSelection
-from pysnptools.util.mapreduce1.runner import Local,LocalMultiProc, LocalInParts
+from pysnptools.util.mapreduce1.runner import Local, LocalMultiProc, LocalInParts
 
-class TestEpistasis(unittest.TestCase):
 
+class TestEpistasis(unittest.TestCase):
 
     @classmethod
     def setUpClass(self):
         from pysnptools.util import create_directory_if_necessary
-        create_directory_if_necessary(self.tempout_dir, isfile=False)
-        self.pythonpath = os.path.abspath(os.path.join(os.path.dirname(os.path.realpath(__file__)),"..","..",".."))
-        self.bedbase = os.path.join(self.pythonpath, 'tests/datasets/all_chr.maf0.001.N300')
-        self.phen_fn = os.path.join(self.pythonpath, 'tests/datasets/phenSynthFrom22.23.N300.randcidorder.txt')
-        self.cov_fn = os.path.join(self.pythonpath,  'tests/datasets/all_chr.maf0.001.covariates.N300.txt')
-
 
+        create_directory_if_necessary(self.tempout_dir, isfile=False)
+        self.pythonpath = os.path.abspath(
+            os.path.join(os.path.dirname(os.path.realpath(__file__)), "..", "..", "..")
+        )
+        self.bedbase = os.path.join(
+            self.pythonpath, "tests/datasets/all_chr.maf0.001.N300"
+        )
+        self.phen_fn = os.path.join(
+            self.pythonpath, "tests/datasets/phenSynthFrom22.23.N300.randcidorder.txt"
+        )
+        self.cov_fn = os.path.join(
+            self.pythonpath, "tests/datasets/all_chr.maf0.001.covariates.N300.txt"
+        )
 
     tempout_dir = "tempout/epistasis"
 
     def test_match_cpp(self):
-        '''
+        """
         match
             FaSTLMM.207\Data\DemoData>fastlmmc -snpPairs -bfile snps -extract topsnps.txt -bfileSim snps -extractSim ASout.snps.txt -pheno pheno.txt -covar covariate.txt -out topsnps.pairs.txt -logDelta 0 -verbose 100
 
-        '''
+        """
         logging.info("TestEpistasis test_match_cpp")
         from pysnptools.snpreader import Bed
-        snps = Bed(os.path.join(self.pythonpath, "tests/datasets/selecttest/snps.bed"),count_A1=False)
+
+        snps = Bed(
+            os.path.join(self.pythonpath, "tests/datasets/selecttest/snps.bed"),
+            count_A1=False,
+        )
         pheno = os.path.join(self.pythonpath, "tests/datasets/selecttest/pheno.txt")
         covar = os.path.join(self.pythonpath, "tests/datasets/selecttest/covariate.txt")
-        sim_sid = ["snp26250_m0_.19m1_.19","snp82500_m0_.28m1_.28","snp63751_m0_.23m1_.23","snp48753_m0_.4m1_.4","snp45001_m0_.26m1_.26","snp52500_m0_.05m1_.05","snp75002_m0_.39m1_.39","snp41253_m0_.07m1_.07","snp11253_m0_.2m1_.2","snp86250_m0_.33m1_.33","snp3753_m0_.23m1_.23","snp75003_m0_.32m1_.32","snp30002_m0_.25m1_.25","snp26252_m0_.19m1_.19","snp67501_m0_.15m1_.15","snp63750_m0_.28m1_.28","snp30001_m0_.28m1_.28","snp52502_m0_.35m1_.35","snp33752_m0_.31m1_.31","snp37503_m0_.37m1_.37","snp15002_m0_.11m1_.11","snp3751_m0_.34m1_.34","snp7502_m0_.18m1_.18","snp52503_m0_.3m1_.3","snp30000_m0_.39m1_.39","isnp4457_m0_.11m1_.11","isnp23145_m0_.2m1_.2","snp60001_m0_.39m1_.39","snp33753_m0_.16m1_.16","isnp60813_m0_.2m1_.2","snp82502_m0_.34m1_.34","snp11252_m0_.13m1_.13"]
+        sim_sid = [
+            "snp26250_m0_.19m1_.19",
+            "snp82500_m0_.28m1_.28",
+            "snp63751_m0_.23m1_.23",
+            "snp48753_m0_.4m1_.4",
+            "snp45001_m0_.26m1_.26",
+            "snp52500_m0_.05m1_.05",
+            "snp75002_m0_.39m1_.39",
+            "snp41253_m0_.07m1_.07",
+            "snp11253_m0_.2m1_.2",
+            "snp86250_m0_.33m1_.33",
+            "snp3753_m0_.23m1_.23",
+            "snp75003_m0_.32m1_.32",
+            "snp30002_m0_.25m1_.25",
+            "snp26252_m0_.19m1_.19",
+            "snp67501_m0_.15m1_.15",
+            "snp63750_m0_.28m1_.28",
+            "snp30001_m0_.28m1_.28",
+            "snp52502_m0_.35m1_.35",
+            "snp33752_m0_.31m1_.31",
+            "snp37503_m0_.37m1_.37",
+            "snp15002_m0_.11m1_.11",
+            "snp3751_m0_.34m1_.34",
+            "snp7502_m0_.18m1_.18",
+            "snp52503_m0_.3m1_.3",
+            "snp30000_m0_.39m1_.39",
+            "isnp4457_m0_.11m1_.11",
+            "isnp23145_m0_.2m1_.2",
+            "snp60001_m0_.39m1_.39",
+            "snp33753_m0_.16m1_.16",
+            "isnp60813_m0_.2m1_.2",
+            "snp82502_m0_.34m1_.34",
+            "snp11252_m0_.13m1_.13",
+        ]
         sim_idx = snps.sid_to_index(sim_sid)
-        test_sid = ["snp26250_m0_.19m1_.19","snp63751_m0_.23m1_.23","snp82500_m0_.28m1_.28","snp48753_m0_.4m1_.4","snp45001_m0_.26m1_.26","snp52500_m0_.05m1_.05","snp75002_m0_.39m1_.39","snp41253_m0_.07m1_.07","snp86250_m0_.33m1_.33","snp15002_m0_.11m1_.11","snp33752_m0_.31m1_.31","snp26252_m0_.19m1_.19","snp30001_m0_.28m1_.28","snp11253_m0_.2m1_.2","snp67501_m0_.15m1_.15","snp3753_m0_.23m1_.23","snp52502_m0_.35m1_.35","snp30000_m0_.39m1_.39","snp30002_m0_.25m1_.25"]
+        test_sid = [
+            "snp26250_m0_.19m1_.19",
+            "snp63751_m0_.23m1_.23",
+            "snp82500_m0_.28m1_.28",
+            "snp48753_m0_.4m1_.4",
+            "snp45001_m0_.26m1_.26",
+            "snp52500_m0_.05m1_.05",
+            "snp75002_m0_.39m1_.39",
+            "snp41253_m0_.07m1_.07",
+            "snp86250_m0_.33m1_.33",
+            "snp15002_m0_.11m1_.11",
+            "snp33752_m0_.31m1_.31",
+            "snp26252_m0_.19m1_.19",
+            "snp30001_m0_.28m1_.28",
+            "snp11253_m0_.2m1_.2",
+            "snp67501_m0_.15m1_.15",
+            "snp3753_m0_.23m1_.23",
+            "snp52502_m0_.35m1_.35",
+            "snp30000_m0_.39m1_.39",
+            "snp30002_m0_.25m1_.25",
+        ]
         test_idx = snps.sid_to_index(test_sid)
 
-        frame = epistasis(snps[:,test_idx], pheno,covar=covar, G0 = snps[:,sim_idx],log_delta=0,count_A1=False)
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-
-        referenceOutfile = TestFeatureSelection.reference_file("epistasis/topsnps.pairs.txt")
+        frame = epistasis(
+            snps[:, test_idx],
+            pheno,
+            covar=covar,
+            G0=snps[:, sim_idx],
+            log_delta=0,
+            count_A1=False,
+        )
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+
+        referenceOutfile = TestFeatureSelection.reference_file(
+            "epistasis/topsnps.pairs.txt"
+        )
 
         import pandas as pd
-        table = pd.read_csv(referenceOutfile,sep="\t") # We've manually remove all comments and blank lines from this file
+
+        table = pd.read_csv(
+            referenceOutfile, sep="\t"
+        )  # We've manually remove all comments and blank lines from this file
         assert len(pvalue_list) == len(table)
         for row in table.iterrows():
-            snp0cpp,snp1cpp,pvaluecpp,i1,i2 = row[1]
+            snp0cpp, snp1cpp, pvaluecpp, i1, i2 = row[1]
             for i in range(len(pvalue_list)):
                 found = False
                 pvaluepy = pvalue_list[i]
                 snp0py = sid0[i]
                 snp1py = sid1[i]
-                if (snp0py == snp0cpp and snp1py == snp1cpp) or (snp0py == snp1cpp and snp1py == snp0cpp):
+                if (snp0py == snp0cpp and snp1py == snp1cpp) or (
+                    snp0py == snp1cpp and snp1py == snp0cpp
+                ):
                     found = True
-                    diff = abs(pvaluecpp - pvaluepy)/pvaluecpp
-                    assert diff < .035, "'{0}' '{1}' pvalue_list differ too much {4} -- {2} vs {3}".format(snp0cpp,snp1cpp,pvaluecpp,pvaluepy,diff)
+                    diff = abs(pvaluecpp - pvaluepy) / pvaluecpp
+                    assert (
+                        diff < 0.035
+                    ), "'{0}' '{1}' pvalue_list differ too much {4} -- {2} vs {3}".format(
+                        snp0cpp, snp1cpp, pvaluecpp, pvaluepy, diff
+                    )
                     break
             assert found
-                
-        
-        #self.sorted_pvalue_list = table["Pvalue"].tolist()
-        #self.sorted_snps = table["SNP"].tolist()
-        
-        #self.pvalue_list = table.sort_values("Position")["Pvalue"].tolist()
 
+        # self.sorted_pvalue_list = table["Pvalue"].tolist()
+        # self.sorted_snps = table["SNP"].tolist()
 
-        #print "done"
-        #for i,pvalue_list in enumerate(pvalue_list):
+        # self.pvalue_list = table.sort_values("Position")["Pvalue"].tolist()
+
+        # print "done"
+        # for i,pvalue_list in enumerate(pvalue_list):
         #    print "{0}\t{1}\t{2}".format(sid0[i],sid1[i],pvalue_list)
-        #print "more done"
- 
-    def file_name(self,testcase_name):
-        temp_fn = os.path.join(self.tempout_dir,testcase_name+".txt")
+        # print "more done"
+
+    def file_name(self, testcase_name):
+        temp_fn = os.path.join(self.tempout_dir, testcase_name + ".txt")
         if os.path.exists(temp_fn):
             os.remove(temp_fn)
         return temp_fn
 
     def test_one(self):
         logging.info("TestEpistasis test_one")
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
+
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
         covar = self.cov_fn
 
         output_file = self.file_name("one")
-        frame = epistasis(test_snps, pheno, G0=test_snps, 
-                                  covar=covar, 
-                                  sid_list_0=test_snps.sid[:10], #first 10 snps
-                                  sid_list_1=test_snps.sid[5:15], #Skip 5 snps, use next 10
-                                  output_file_name=output_file,count_A1=False
-                                  )
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            covar=covar,
+            sid_list_0=test_snps.sid[:10],  # first 10 snps
+            sid_list_1=test_snps.sid[5:15],  # Skip 5 snps, use next 10
+            output_file_name=output_file,
+            count_A1=False,
+        )
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
 
-        #Check the output file
-        self.compare_files(sid0,sid1,pvalue_list,"one")
+        # Check the output file
+        self.compare_files(sid0, sid1, pvalue_list, "one")
 
-        #Check the values returned
+        # Check the values returned
         output_file2 = self.file_name("one_again")
-        write(sid0,sid1,pvalue_list,output_file2)
-        self.compare_files(sid0,sid1,pvalue_list,"one")
-        
+        write(sid0, sid1, pvalue_list, output_file2)
+        self.compare_files(sid0, sid1, pvalue_list, "one")
 
     def test_preload_files(self):
         logging.info("TestEpistasis test_preload_files")
         from pysnptools.snpreader import Bed
+
         test_snps = self.bedbase
-        pheno = pstpheno.loadOnePhen(self.phen_fn,vectorize=True)
+        pheno = pstpheno.loadOnePhen(self.phen_fn, vectorize=True)
         covar = pstpheno.loadPhen(self.cov_fn)
-        bed = Bed(test_snps,count_A1=False)
+        bed = Bed(test_snps, count_A1=False)
 
         output_file = self.file_name("preload_files")
 
-        frame = epistasis(test_snps, pheno, G0=test_snps, 
-                                  covar=covar, 
-                                  sid_list_0=bed.sid[:10], #first 10 snps
-                                  sid_list_1=bed.sid[5:15], #Skip 5 snps, use next 10
-                                  output_file_name=output_file,count_A1=False
-                                  )
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-        self.compare_files(sid0,sid1,pvalue_list,"one")
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            covar=covar,
+            sid_list_0=bed.sid[:10],  # first 10 snps
+            sid_list_1=bed.sid[5:15],  # Skip 5 snps, use next 10
+            output_file_name=output_file,
+            count_A1=False,
+        )
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+        self.compare_files(sid0, sid1, pvalue_list, "one")
 
-        
     def test_G0_has_reader(self):
         logging.info("TestEpistasis test_G0_has_reader")
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
+
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
         covar = self.cov_fn
 
         output_file = self.file_name("G0_has_reader")
 
-        frame = epistasis(test_snps, pheno, G0=test_snps, 
-                                  covar=covar, 
-                                  sid_list_0=test_snps.sid[:10], #first 10 snps
-                                  sid_list_1=test_snps.sid[5:15], #Skip 5 snps, use next 10
-                                  output_file_name=output_file,count_A1=False
-                                  )
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-        self.compare_files(sid0,sid1,pvalue_list,"one")
-        
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            covar=covar,
+            sid_list_0=test_snps.sid[:10],  # first 10 snps
+            sid_list_1=test_snps.sid[5:15],  # Skip 5 snps, use next 10
+            output_file_name=output_file,
+            count_A1=False,
+        )
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+        self.compare_files(sid0, sid1, pvalue_list, "one")
 
     def test_no_sid_list_0(self):
         logging.info("TestEpistasis test_no_sid_list_0")
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
+
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
         covar = self.cov_fn
 
         output_file = self.file_name("no_sid_list_0")
-        frame = epistasis(test_snps, pheno, G0=test_snps, 
-                                  covar=covar, 
-                                  sid_list_0=['1_4'],
-                                  output_file_name=output_file,count_A1=False
-                                  )
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-        self.compare_files(sid0,sid1,pvalue_list,"no_sid_list_0")
-        
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            covar=covar,
+            sid_list_0=["1_4"],
+            output_file_name=output_file,
+            count_A1=False,
+        )
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+        self.compare_files(sid0, sid1, pvalue_list, "no_sid_list_0")
 
     def test_no_sid_list_1(self):
         logging.info("TestEpistasis test_no_sid_list_1")
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
+
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
         covar = self.cov_fn
 
         output_file = self.file_name("no_sid_list_1")
-        frame = epistasis(test_snps, pheno, G0=test_snps, 
-                                  covar=covar, 
-                                  sid_list_1=['1_4'],count_A1=False
-                                  )
-
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-        write(sid0,sid1,pvalue_list,output_file)        
-        self.compare_files(sid1,sid0,pvalue_list,"no_sid_list_0") #Swap order of sid0 and sid1
-        
-        
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            covar=covar,
+            sid_list_1=["1_4"],
+            count_A1=False,
+        )
+
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+        write(sid0, sid1, pvalue_list, output_file)
+        self.compare_files(
+            sid1, sid0, pvalue_list, "no_sid_list_0"
+        )  # Swap order of sid0 and sid1
 
     def test_no_cov(self):
         logging.info("TestEpistasis test_no_cov")
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
+
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
 
         output_file = self.file_name("no_cov")
-        frame = epistasis(test_snps, pheno, G0=test_snps, 
-                                          sid_list_0=test_snps.sid[:10], #first 10 snps
-                                          sid_list_1=test_snps.sid[5:15], #Skip 5 snps, use next 10
-                                          output_file_name=output_file,count_A1=False
-                                          )
-
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-        self.compare_files(sid0,sid1,pvalue_list,"no_cov")
-        
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            sid_list_0=test_snps.sid[:10],  # first 10 snps
+            sid_list_1=test_snps.sid[5:15],  # Skip 5 snps, use next 10
+            output_file_name=output_file,
+            count_A1=False,
+        )
+
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+        self.compare_files(sid0, sid1, pvalue_list, "no_cov")
 
     def test_no_cov_b(self):
         logging.info("TestEpistasis test_no_cov_b")
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
+
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
 
         output_file = self.file_name("no_cov_b")
         covar = pstpheno.loadPhen(self.cov_fn)
-        covar['vals'] = np.delete(covar['vals'], np.s_[:],1) #Remove all the columns
+        covar["vals"] = np.delete(covar["vals"], np.s_[:], 1)  # Remove all the columns
 
-        frame = epistasis(test_snps, pheno, G0=test_snps, 
-                                  covar=covar,
-                                  sid_list_0=test_snps.sid[:10], #first 10 snps
-                                  sid_list_1=test_snps.sid[5:15], #Skip 5 snps, use next 10
-                                  output_file_name=output_file,count_A1=False
-                                  )
-
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-        self.compare_files(sid0,sid1,pvalue_list,"no_cov")
-        
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            covar=covar,
+            sid_list_0=test_snps.sid[:10],  # first 10 snps
+            sid_list_1=test_snps.sid[5:15],  # Skip 5 snps, use next 10
+            output_file_name=output_file,
+            count_A1=False,
+        )
+
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+        self.compare_files(sid0, sid1, pvalue_list, "no_cov")
 
     def test_G1(self):
         logging.info("TestEpistasis test_G1")
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
+
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
         covar = self.cov_fn
 
         output_file = self.file_name("G1")
-        frame = epistasis(test_snps, pheno, G0=test_snps, 
-                                      covar=covar, 
-                                      sid_list_0=test_snps.sid[:10], #first 10 snps
-                                      sid_list_1=test_snps.sid[5:15], #Skip 5 snps, use next 10
-                                      G1=test_snps,
-                                      mixing=.5,
-                                      output_file_name=output_file,count_A1=False
-                                      )
-
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-        self.compare_files(sid0,sid1,pvalue_list,"G1")
-        
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            covar=covar,
+            sid_list_0=test_snps.sid[:10],  # first 10 snps
+            sid_list_1=test_snps.sid[5:15],  # Skip 5 snps, use next 10
+            G1=test_snps,
+            mixing=0.5,
+            output_file_name=output_file,
+            count_A1=False,
+        )
+
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+        self.compare_files(sid0, sid1, pvalue_list, "G1")
 
     def test_G1b(self):
         logging.info("TestEpistasis test_G1b")
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
+
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
         covar = self.cov_fn
 
         output_file = self.file_name("G1b")
-        frame = epistasis(test_snps, pheno, G0=test_snps, 
-                                  covar=covar, 
-                                  sid_list_0=test_snps.sid[:10], #first 10 snps
-                                  sid_list_1=test_snps.sid[5:15], #Skip 5 snps, use next 10
-                                  G1=test_snps,
-                                  mixing=.5,
-                                  output_file_name=output_file,count_A1=False
-                                  )
-
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-        self.compare_files(sid0,sid1,pvalue_list,"G1")
-        
-
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            covar=covar,
+            sid_list_0=test_snps.sid[:10],  # first 10 snps
+            sid_list_1=test_snps.sid[5:15],  # Skip 5 snps, use next 10
+            G1=test_snps,
+            mixing=0.5,
+            output_file_name=output_file,
+            count_A1=False,
+        )
+
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+        self.compare_files(sid0, sid1, pvalue_list, "G1")
 
     def test_G1_mixing(self):
         logging.info("TestEpistasis test_G1_mixing")
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
+
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
         covar = self.cov_fn
 
         output_file = self.file_name("G1_mixing")
-        frame = epistasis(test_snps, pheno, G0=test_snps,
-                                  covar=covar, 
-                                  sid_list_0=test_snps.sid[:10], #first 10 snps
-                                  sid_list_1=test_snps.sid[5:15], #Skip 5 snps, use next 10
-                                  G1=test_snps,
-                                  mixing=0,
-                                  output_file_name=output_file,count_A1=False
-                                  )
-
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-        self.compare_files(sid0,sid1,pvalue_list,"one")
-        
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            covar=covar,
+            sid_list_0=test_snps.sid[:10],  # first 10 snps
+            sid_list_1=test_snps.sid[5:15],  # Skip 5 snps, use next 10
+            G1=test_snps,
+            mixing=0,
+            output_file_name=output_file,
+            count_A1=False,
+        )
+
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+        self.compare_files(sid0, sid1, pvalue_list, "one")
 
-
-    #def test_REML_delta(self):
+    # def test_REML_delta(self):
     #    logging.info("TestEpistasis test_REML_delta")
 
     #    from pysnptools.snpreader import Bed
     #    snps = Bed(os.path.join(self.pythonpath, "tests/datasets/selecttest/snps.bed"),count_A1=False)
     #    pheno = os.path.join(self.pythonpath, "tests/datasets/selecttest/pheno.txt")
     #    covar = os.path.join(self.pythonpath, "tests/datasets/selecttest/covariate.txt")
     #    sim_sid = ["snp26250_m0_.19m1_.19","snp82500_m0_.28m1_.28","snp63751_m0_.23m1_.23","snp48753_m0_.4m1_.4","snp45001_m0_.26m1_.26","snp52500_m0_.05m1_.05","snp75002_m0_.39m1_.39","snp41253_m0_.07m1_.07","snp11253_m0_.2m1_.2","snp86250_m0_.33m1_.33","snp3753_m0_.23m1_.23","snp75003_m0_.32m1_.32","snp30002_m0_.25m1_.25","snp26252_m0_.19m1_.19","snp67501_m0_.15m1_.15","snp63750_m0_.28m1_.28","snp30001_m0_.28m1_.28","snp52502_m0_.35m1_.35","snp33752_m0_.31m1_.31","snp37503_m0_.37m1_.37","snp15002_m0_.11m1_.11","snp3751_m0_.34m1_.34","snp7502_m0_.18m1_.18","snp52503_m0_.3m1_.3","snp30000_m0_.39m1_.39","isnp4457_m0_.11m1_.11","isnp23145_m0_.2m1_.2","snp60001_m0_.39m1_.39","snp33753_m0_.16m1_.16","isnp60813_m0_.2m1_.2","snp82502_m0_.34m1_.34","snp11252_m0_.13m1_.13"]
@@ -309,104 +468,129 @@
     #    sid0,sid1,pvalue_list = epistasis(snps[:,test_idx], pheno,covar=covar, G0 = snps[:,sim_idx],log_delta=np.log(1),REML=True, G1=covar, mixing=.5,output_file=output_file,count_A1=False)
     #    self.compare_files(sid0,sid1,pvalue_list,"REML_delta")
 
     def test_unknown_sid(self):
         logging.info("TestEpistasis test_unknown_sid")
 
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
+
+        test_snps = Bed(self.bedbase, count_A1=False)
         pheno = self.phen_fn
         covar = self.cov_fn
 
         try:
-            frame = epistasis(test_snps, pheno,covar=covar,sid_list_0=['1_4','bogus sid','1_9'],sid_list_1=test_snps.sid[5:15],count_A1=False) #Skip 5 snps, use next 10
+            frame = epistasis(
+                test_snps,
+                pheno,
+                covar=covar,
+                sid_list_0=["1_4", "bogus sid", "1_9"],
+                sid_list_1=test_snps.sid[5:15],
+                count_A1=False,
+            )  # Skip 5 snps, use next 10
             failed = False
         except:
             failed = True
 
-        assert(failed)
+        assert failed
 
     def test_cid_intersect(self):
         logging.info("TestEpistasis test_cid_intersect")
         from pysnptools.snpreader import Bed
-        test_snps = Bed(self.bedbase,count_A1=False)
-        pheno = pstpheno.loadOnePhen(self.phen_fn,vectorize=True)
-        pheno['iid'] = np.vstack([pheno['iid'][::-1],[['Bogus','Bogus']]])
-        pheno['vals'] = np.hstack([pheno['vals'][::-1],[-34343]])
 
-        
+        test_snps = Bed(self.bedbase, count_A1=False)
+        pheno = pstpheno.loadOnePhen(self.phen_fn, vectorize=True)
+        pheno["iid"] = np.vstack([pheno["iid"][::-1], [["Bogus", "Bogus"]]])
+        pheno["vals"] = np.hstack([pheno["vals"][::-1], [-34343]])
+
         covar = self.cov_fn
         output_file = self.file_name("cid_intersect")
-        frame = epistasis(test_snps, pheno, G0=test_snps,
-                                  covar=covar, 
-                                  sid_list_0=test_snps.sid[:10], #first 10 snps
-                                  sid_list_1=test_snps.sid[5:15], #Skip 5 snps, use next 10
-                                  output_file_name=output_file,count_A1=False
-                                  )
-
-        sid0,sid1,pvalue_list =np.array(frame['SNP0']),np.array(frame['SNP1']),np.array(frame['PValue'])
-        self.compare_files(sid0,sid1,pvalue_list,"one")
-        
+        frame = epistasis(
+            test_snps,
+            pheno,
+            G0=test_snps,
+            covar=covar,
+            sid_list_0=test_snps.sid[:10],  # first 10 snps
+            sid_list_1=test_snps.sid[5:15],  # Skip 5 snps, use next 10
+            output_file_name=output_file,
+            count_A1=False,
+        )
+
+        sid0, sid1, pvalue_list = (
+            np.array(frame["SNP0"]),
+            np.array(frame["SNP1"]),
+            np.array(frame["PValue"]),
+        )
+        self.compare_files(sid0, sid1, pvalue_list, "one")
 
-    def compare_files(self,sid0_list,sid1_list,pvalue_list,ref_base):
-        reffile = TestFeatureSelection.reference_file("epistasis/"+ref_base+".txt")
+    def compare_files(self, sid0_list, sid1_list, pvalue_list, ref_base):
+        reffile = TestFeatureSelection.reference_file("epistasis/" + ref_base + ".txt")
 
         pair_to_pvalue = {}
         for index, sid0 in enumerate(sid0_list):
             sid1 = sid1_list[index]
             if sid0 < sid1:
                 key = (sid0, sid1)
             else:
                 key = (sid1, sid0)
             pair_to_pvalue[key] = pvalue_list[index]
 
-        reference=sp.loadtxt(reffile,dtype='str',delimiter='\t',comments=None,skiprows=1)
-        assert len(pvalue_list) == len(reference), "# of pairs differs from file '{0}'".format(reffile)
+        reference = np.loadtxt(
+            reffile, dtype="str", delimiter="\t", comments=None, skiprows=1
+        )
+        assert len(pvalue_list) == len(
+            reference
+        ), "# of pairs differs from file '{0}'".format(reffile)
         for row in reference:
             sid0 = row[0]
             sid1 = row[4]
             if sid0 < sid1:
                 key = (sid0, sid1)
             else:
                 key = (sid1, sid0)
 
-            assert abs(float(row[8])-pair_to_pvalue[key]) < 1e-5, "pair {0} differs too much from file '{1}'".format(key,reffile)
+            assert (
+                abs(float(row[8]) - pair_to_pvalue[key]) < 1e-5
+            ), "pair {0} differs too much from file '{1}'".format(key, reffile)
 
     def test_doctest(self):
         old_dir = os.getcwd()
-        os.chdir(os.path.dirname(os.path.realpath(__file__))+"/..")
-        result = doctest.testmod(sys.modules['fastlmm.association.epistasis'])
+        os.chdir(os.path.dirname(os.path.realpath(__file__)) + "/..")
+        result = doctest.testmod(sys.modules["fastlmm.association.epistasis"])
         os.chdir(old_dir)
         assert result.failed == 0, "failed doc test: " + __file__
 
+
 def getTestSuite():
     suite1 = unittest.TestLoader().loadTestsFromTestCase(TestEpistasis)
     return unittest.TestSuite([suite1])
 
 
+if __name__ == "__main__":
 
-if __name__ == '__main__':
-  
     from fastlmm.association.tests.testepistasis import TestEpistasis
+
     suites = unittest.TestSuite([getTestSuite()])
 
-    if True: #Standard test run
+    if True:  # Standard test run
         r = unittest.TextTestRunner(failfast=False)
         ret = r.run(suites)
         assert ret.wasSuccessful()
-    else: #Cluster test run
+    else:  # Cluster test run
         from pysnptools.util.mapreduce1.distributabletest import DistributableTest
 
-
-        runner = HPC(10, 'RR1-N13-09-H44',r'\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\Redmond',
-                     remote_python_parent=r"\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\REDMOND\carlk\Source\carlk\july_7_14\tests\runs\2014-07-24_15_02_02_554725991686\pythonpath",
-                     update_remote_python_parent=True,
-                     priority="AboveNormal",mkl_num_threads=1)
+        runner = HPC(
+            10,
+            "RR1-N13-09-H44",
+            r"\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\Redmond",
+            remote_python_parent=r"\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\REDMOND\carlk\Source\carlk\july_7_14\tests\runs\2014-07-24_15_02_02_554725991686\pythonpath",
+            update_remote_python_parent=True,
+            priority="AboveNormal",
+            mkl_num_threads=1,
+        )
         runner = Local()
-        #runner = LocalMultiProc(taskcount=20,mkl_num_threads=5)
-        #runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
-        #runner = Hadoop(100, mapmemory=8*1024, reducememory=8*1024, mkl_num_threads=1, queue="default")
-        distributable_test = DistributableTest(suites,"temp_test")
+        # runner = LocalMultiProc(taskcount=20,mkl_num_threads=5)
+        # runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
+        # runner = Hadoop(100, mapmemory=8*1024, reducememory=8*1024, mkl_num_threads=1, queue="default")
+        distributable_test = DistributableTest(suites, "temp_test")
         print(runner.run(distributable_test))
 
-
     logging.info("done with testing")
```

### Comparing `fastlmm-0.6.7/fastlmm/association/tests/tests_util.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/tests_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import absolute_import
 from fastlmm.feature_selection import PerformSelectionDistributable as psd
 import fastlmm.util.preprocess as up
 import numpy as np
 
 
 def set_Gexclude(G_exclude, G1, i_exclude):
     if G_exclude is None and i_exclude is not None and i_exclude.sum() > 0:
```

### Comparing `fastlmm-0.6.7/fastlmm/association/varcomp_test.py` & `fastlmm-0.6.8b1/fastlmm/association/varcomp_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-from __future__ import absolute_import
 import numpy as np
-from six.moves import range
+
 
 class varcomp_test(object):
-    __slots__ = ["Y","X"]
-  
-    def __init__(self, Y, X=None, appendbias = False):
-        self.Y=Y
+    __slots__ = ["Y", "X"]
+
+    def __init__(self, Y, X=None, appendbias=False):
+        self.Y = Y
 
-        N=self.Y.shape[0]
+        N = self.Y.shape[0]
         if X is None:
-            self.X = np.ones((N,1))
+            self.X = np.ones((N, 1))
         elif appendbias:
-            assert self.hasBias() is False, ('You are trying to append a bias column in a dataset '
-                                             'that already has one.')
-            self.X=SP.hstack((np.ones((N,1)),X))
+            assert self.hasBias() is False, (
+                "You are trying to append a bias column in a dataset "
+                "that already has one."
+            )
+            self.X = np.hstack((np.ones((N, 1)), X))
         else:
             self.X = X
 
     def _updateYX(self, Y, X):
-        self.Y=Y        
-        self.X=X
+        self.Y = Y
+        self.X = X
 
     def hasBias(self):
 
         for i in range(self.X.shape[1]):
-            if np.all(self.X[:,i] == 1.0):
+            if np.all(self.X[:, i] == 1.0):
                 return True
 
         return False
 
-    def testG(self, G1, type = None,i_exclude=None):
+    def testG(self, G1, type=None, i_exclude=None):
         raise NotImplementedError
         pv = None
         stat = None
-        return pv, stat
+        return pv, stat
```

### Comparing `fastlmm-0.6.7/fastlmm/association/windowing_gwas.py` & `fastlmm-0.6.8b1/fastlmm/association/windowing_gwas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """
 implementation of windowing to cut out only single snp from G0 (which is used to condition on AND to test)
 
 Authors: Chris Widmer
 Created: 9/25/2014
 """
 
-from __future__ import absolute_import
 import os
 import numpy as np
 import logging
 from scipy import stats
 from pysnptools.snpreader import Bed
 from pysnptools.util import intersect_apply
 import pysnptools.util.pheno as pstpheno
 import fastlmm.util.standardizer as stdizer
 from fastlmm.inference import LMM
-from six.moves import range
 
 
 class WindowingGwas(object):
     """
     class to perform genome-wide scan with single-snp windowing
     """
```

### Comparing `fastlmm-0.6.7/fastlmm/external/pca.py` & `fastlmm-0.6.8b1/fastlmm/external/pca.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 # Author: Alexandre Gramfort <alexandre.gramfort@inria.fr>
 #         Olivier Grisel <olivier.grisel@ensta.org>
 #         Mathieu Blondel <mathieu@mblondel.org>
 #         Denis A. Engemann <d.engemann@fz-juelich.de>
 #
 # License: BSD 3 clause
 
-from __future__ import absolute_import
 from math import log, sqrt
 import warnings
 
 import numpy as np
 from scipy import linalg
 from scipy.special import gammaln
 
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils import check_random_state, as_float_array, check_array
 
 # from sklearn.utils import atleast2d_or_csr
 from sklearn.utils import deprecated
 from sklearn.utils.extmath import fast_logdet, safe_sparse_dot, randomized_svd  # ,
-from six.moves import range
+
 
 # fast_dot)
 
 
 def _assess_dimension_(spectrum, rank, n_samples, n_features):
     """Compute the likelihood of a rank ``rank`` dataset
```

### Comparing `fastlmm-0.6.7/fastlmm/external/util/math.py` & `fastlmm-0.6.8b1/fastlmm/external/util/math.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,71 @@
-from __future__ import absolute_import
 import numpy as np
-import scipy as sp
+import scipy.linalg as la
+
 
 def mvnormpdf(b, mean, cov, precision=False):
     k = b.shape[0]
-    part1 = np.exp(-0.5*k*np.log(2.0*np.pi))
-    dev = b-mean
+    part1 = np.exp(-0.5 * k * np.log(2.0 * np.pi))
+    dev = b - mean
     if precision is False:
-        part2 = np.power(np.linalg.det(cov),-0.5)
-        part3 = np.exp(-0.5*np.dot(np.dot(dev,np.linalg.inv(cov)),dev))
+        part2 = np.power(np.linalg.det(cov), -0.5)
+        part3 = np.exp(-0.5 * np.dot(np.dot(dev, np.linalg.inv(cov)), dev))
     else:
-        part2 = np.power(np.linalg.det(cov),0.5)
-        part3 = np.exp(-0.5*np.dot(np.dot(dev,cov),dev))
-    return part1*part2*part3
+        part2 = np.power(np.linalg.det(cov), 0.5)
+        part3 = np.exp(-0.5 * np.dot(np.dot(dev, cov), dev))
+    return part1 * part2 * part3
+
 
 # Performs np.tr(dot(A, B))
 def trace2(A, B):
-    assert len(A.shape)==2 and len(B.shape)==2
-    assert A.shape[1]==B.shape[0] and A.shape[0]==B.shape[1]
-    return np.sum(A.T*B)
+    assert len(A.shape) == 2 and len(B.shape) == 2
+    assert A.shape[1] == B.shape[0] and A.shape[0] == B.shape[1]
+    return np.sum(A.T * B)
+
 
 def dotd(A, B):
     """Multiply two matrices and return the
     resulting diagonal.
     If A is nxp and B is pxn, it is done in O(pn).
     """
-    return np.sum(A * B.T,1)
+    return np.sum(A * B.T, 1)
+
 
 def ddot(d, mtx, left=True):
     """Multiply a full matrix by a diagonal matrix.
     This function should always be faster than dot.
 
     Input:
       d -- 1D (N,) array (contains the diagonal elements)
       mtx -- 2D (N,N) array
 
     Output:
       ddot(d, mts, left=True) == dot(diag(d), mtx)
       ddot(d, mts, left=False) == dot(mtx, diag(d))
     """
     if left:
-        return (d*mtx.T).T
+        return (d * mtx.T).T
     else:
-        return d*mtx
+        return d * mtx
+
 
 def check_definite_positiveness(A):
     B = np.empty_like(A)
     B[:] = A
     B[np.diag_indices_from(B)] += np.sqrt(np.finfo(float).eps)
     try:
         np.linalg.cholesky(B)
     except np.linalg.LinAlgError:
         return False
     return True
 
+
 def check_symmetry(A):
-    return abs(A-A.T).max() < np.sqrt(np.finfo(float).eps)
+    return abs(A - A.T).max() < np.sqrt(np.finfo(float).eps)
+
+
+def kl_divergence(p, q):
+    return np.sum(np.log(p / q) * p)
 
-def kl_divergence(p,q):
-    return np.sum(np.log(p/q)*p)
 
-stl = lambda a, b : sp.linalg.solve_triangular(a, b, lower=True, check_finite=False)
-stu = lambda a, b : sp.linalg.solve_triangular(a, b, lower=False, check_finite=False)
+stl = lambda a, b: la.solve_triangular(a, b, lower=True, check_finite=False)
+stu = lambda a, b: la.solve_triangular(a, b, lower=False, check_finite=False)
```

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/PerformSelectionDistributable.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/PerformSelectionDistributable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # std modules
-from __future__ import absolute_import
 from collections import defaultdict
 import gzip
 import bz2
 import pickle
 import time
 import os
 import gc
 import logging
 import io
 
 # common modules
-from six.moves import range
-import scipy as sp
 import numpy as np
 import pandas as pd
 import sys
 
 # sklearn
 from sklearn.linear_model import RidgeCV, Ridge
 from sklearn.model_selection import KFold, LeaveOneOut, ShuffleSplit
@@ -214,31 +211,31 @@
         best_snps, sorted_pval = self.feature_selection_strategy.final_scan(
             best_k, lingreg_results
         )
 
         # write report file
         if self.output_prefix is not None:
             report = "k_grid: " + str([k for k in self.k_values]) + "\n"
-            ln_delta_grid = np.array([sp.log(x) for x in self.delta_values])
+            ln_delta_grid = np.array([np.log(x) for x in self.delta_values])
             report += (
                 "ln_delta_grid: ["
                 + ", ".join([f"{v:.1f}" for v in ln_delta_grid])
                 + "]\n"
             )
             report += "best k=%i\nbest ln_delta=%.1e\nbest objective=%.2f" % (
                 best_k,
-                sp.log(best_delta),
+                np.log(best_delta),
                 best_obj,
             )
             if (
                 self.feature_selection_strategy.interpolate_delta
                 and best_delta_interp is not None
             ):
                 report += "\nbest ln_delta_interp=%.1e\nbest objective_interp=%.2f" % (
-                    sp.log(best_delta_interp),
+                    np.log(best_delta_interp),
                     best_obj_interp,
                 )
 
             report_fn = self.output_prefix + "_report.txt"
             pstutil.create_directory_if_necessary(report_fn)
             report_file = open(report_fn, "w")
             report_file.write(report)
@@ -472,15 +469,15 @@
     if hasattr(alt_snpreader, "ind_used") and alt_snpreader.ind_used is not None:
         N = len(alt_snpreader.ind_used)
     else:
         N = len(alt_snpreader.original_iids)
 
     t0 = time.time()
 
-    K = sp.zeros([N, N])
+    K = np.zeros([N, N])
     num_snps = alt_snpreader.snp_count
 
     if snp_idx is not None:
         snp_names = alt_snpreader.rs[snp_idx]
         current_size = len(snp_names)
         logging.info(
             "reading %i SNPs in blocks of %i and adding up kernels"
@@ -512,14 +509,14 @@
         # logging.info("start = {0}".format(start))
         K += snps.dot(snps.T)
 
         if ct % blocksize == 0:
             logging.info("read %s SNPs in %.2f seconds" % (ct, time.time() - ts))
 
     # normalize kernel
-    # K = K/sp.sqrt(alt_snpreader.snp_count)
+    # K = K/np.sqrt(alt_snpreader.snp_count)
 
-    # K = K + 1e-5*sp.eye(N,N)
+    # K = K + 1e-5*np.eye(N,N)
     t1 = time.time()
     logging.info("%.2f seconds elapsed" % (t1 - t0))
 
     return K
```

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 exactUpdate = False
 topKbyLinReg = 16
-logdelta = SP.log(16)
+logdelta = np.log(16)
 
 if topKbyLinReg is not None:
     outFile = "examples/ScanISP.exact%d.nSnps%d.logdelta%.2f.out.txt" % (
         exactUpdate,
         topKbyLinReg,
         logdelta,
     )
```

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.5chrom.bed` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.bed`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.5chrom.bim` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.bim`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.5chrom.fam` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.fam`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.cov` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.cov`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.map` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.map`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.phe` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/toydata.shufflePlus.phe` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.shufflePlus.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/toydataTest.phe` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydataTest.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/examples/toydataTrain.phe` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydataTrain.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/feature_selection_cv.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_cv.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import gc
 import subprocess
 import sys
 import logging
 from unittest.mock import patch
 
 # common modules
-import scipy as sp
 import numpy as np
 import pandas as pd
 
 # sklearn
 from sklearn.linear_model import RidgeCV, Ridge
 from sklearn.model_selection import KFold, LeaveOneOut, ShuffleSplit
 from sklearn.metrics import mean_squared_error
@@ -173,17 +172,17 @@
             cov_iid = pheno["iid"]
             X = np.ones((len(cov_iid), 1))
         else:
             cov = pstpheno.loadPhen(self.cov_fn)
             X = cov["vals"]
             cov_iid = cov["iid"]
             # add bias column if not present - #!! LATER -- Bug? should this test be done after intersection in case removing an iid makes it constant?
-            if self.offset and sp.all(X.std(0) != 0):
-                offset = sp.ones((len(X), 1))
-                self.X = sp.hstack((X, offset))
+            if self.offset and np.all(X.std(0) != 0):
+                offset = np.ones((len(X), 1))
+                self.X = np.hstack((X, offset))
         return X, cov_iid
 
     def load_data(self):
         """load data"""
         with patch.dict("os.environ", {"ARRAY_MODULE": "numpy"}) as _:
             tt0 = time.time()
             logging.info("loading data...")
@@ -281,15 +280,15 @@
 
             [s, u] = la.eigh(self.K)
             s = s[::-1]
             u = u[:, ::-1]
             self.pcs = u[:, 0 : self.num_pcs]
         assert self.pcs.shape[1] == self.num_pcs
 
-        self.X = sp.hstack((self.X, self.pcs))
+        self.X = np.hstack((self.X, self.pcs))
 
         logging.info("...done. PCA time %.2f s" % (float(time.time() - tt0)))
 
     def setup_linear_regression(self, max_k, start=0, stop=None):
         """precompute univariate ranking for each split
 
         max_k : int
@@ -520,15 +519,15 @@
                     error_3pt = average_loss[
                         best_k_idx, best_delta_idx - 1 : best_delta_idx + 2
                     ]
 
                     best_ln_delta_interp, best_obj_interp = self.fit_parabola(
                         log_deltas, error_3pt, output_prefix=None
                     )
-                    best_delta_interp = sp.exp(best_ln_delta_interp)
+                    best_delta_interp = np.exp(best_ln_delta_interp)
                     best_str += ", ln_d_interp=%.2f" % (best_ln_delta_interp)
                     logging.info(
                         "best interpolated ln_delta {0}".format(best_ln_delta_interp)
                     )
                 else:
                     logging.warning(
                         "(select by %s): best ln_delta for all k is at the boundary (idx=%i) of search grid, please consider a larger grid"
@@ -545,15 +544,15 @@
                 # visualize results
                 import pylab
 
                 pylab.figure()
                 ax = pylab.subplot(111)
                 try:
                     for delta_idx, delta in enumerate(delta_values):
-                        ln_delta = sp.log(delta)
+                        ln_delta = np.log(delta)
                         ax.semilogx(
                             k_values,
                             average_loss[:, delta_idx],
                             "-x",
                             label="ln_d=%.1f" % (ln_delta),
                         )
 
@@ -847,17 +846,17 @@
     (y, yiid), G, (X, xiid) = pstutil.intersect_apply(
         [(pheno["vals"], pheno["iid"]), geno, (cov["vals"], cov["iid"])],
         sort_by_dataset=False,
     )
     G = G.read(order="C", view_ok=True)
 
     # add bias column if not present
-    if offset and sp.all(X.std(0) != 0):
-        offset = sp.ones((len(indarr), 1))
-        X = sp.hstack((X, offset))
+    if offset and np.all(X.std(0) != 0):
+        offset = np.ones((len(indarr), 1))
+        X = np.hstack((X, offset))
 
     return G, X, y
 
 
 from pysnptools.standardizer import Unit
 from pysnptools.standardizer import Identity
 from pysnptools.standardizer import Beta
@@ -1130,17 +1129,16 @@
     def __repr__(self):
         s = "InMemory({0},{1})".format(self._snpreader, self._standardizer)
         return s
 
     @property
     def val(self):
         if self._val is None:
-            self._snpreader = self._snpreader.read(
-                order="C"
-            )  #!!LATER when should this be order='F' and when order='C'?
+            #!!LATER when should this be order='F' and when order='C'?
+            self._snpreader = self._snpreader.read(order="C")
             self._val = self._snpreader.val
             self._val.flags.writeable = False
         return self._val
 
     @property
     def iid(self):
         return self._snpreader.iid
```

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/feature_selection_example.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_example.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,105 @@
 """
 example of how to use feature selection from python (see also command line interface)
 """
 
-from __future__ import absolute_import
 import numpy as np
 from fastlmm.feature_selection import FeatureSelectionStrategy
 from pysnptools.snpreader import Bed
 
 import logging
 
-def runselect(bed_fn=None, pheno_fn=None, strategy=None, select_by_ll=True, output_prefix=None,num_pcs=0, random_state=3, num_snps_in_memory=1000, cov_fn=None, k_values=None, delta_values=None,num_folds=10,penalty=0.0):
+
+def runselect(
+    bed_fn=None,
+    pheno_fn=None,
+    strategy=None,
+    select_by_ll=True,
+    output_prefix=None,
+    num_pcs=0,
+    random_state=3,
+    num_snps_in_memory=1000,
+    cov_fn=None,
+    k_values=None,
+    delta_values=None,
+    num_folds=10,
+    penalty=0.0,
+):
     logging.basicConfig(level=logging.INFO)
 
     # set up data
     ##############################
     if bed_fn is None:
         bed_fn = Bed("examples/toydata")
         pheno_fn = "examples/toydata.phe"
-    
 
     # set up grid
     ##############################
     num_steps_delta = 10
     num_steps_k = 5
 
     # log_2 space and all SNPs
-    #k_values = np.logspace(0, 9, base=2, num=num_steps_k, endpoint=True).tolist() + [10000]
+    # k_values = np.logspace(0, 9, base=2, num=num_steps_k, endpoint=True).tolist() + [10000]
     if k_values is None:
-        k_values = [0, 1, 5, 10, 20, 50, 100, 500, 1000, 2000, 5000, 10000, 456345643256] #100, 110, 120, 130, 140, 150, 160, 170, 180, 190, 200, 210, 220, 230, 240, 250, 260, 270, 280, 290, 300, 400, 500, 1000]
+        k_values = [
+            0,
+            1,
+            5,
+            10,
+            20,
+            50,
+            100,
+            500,
+            1000,
+            2000,
+            5000,
+            10000,
+            456345643256,
+        ]  # 100, 110, 120, 130, 140, 150, 160, 170, 180, 190, 200, 210, 220, 230, 240, 250, 260, 270, 280, 290, 300, 400, 500, 1000]
     if delta_values is None:
-        delta_values = np.logspace(-10, 10, endpoint=True, num=num_steps_delta, base=np.exp(1))
-    #delta_values = [np.exp(1), np.exp(2), np.exp(3), np.exp(4), np.exp(5), np.exp(6)]
+        delta_values = np.logspace(
+            -10, 10, endpoint=True, num=num_steps_delta, base=np.exp(1)
+        )
+    # delta_values = [np.exp(1), np.exp(2), np.exp(3), np.exp(4), np.exp(5), np.exp(6)]
 
     if strategy is None:
-        strategy = 'lmm_full_cv'
+        strategy = "lmm_full_cv"
         select_by_ll = True
     if 0:
-        strategy = 'insample_cv'
+        strategy = "insample_cv"
         select_by_ll = True
     # where to save output
     ##############################
     if output_prefix is None:
         output_prefix = "example_pc%i" % (num_pcs)
-    
-    # go!
-    fss = FeatureSelectionStrategy(bed_fn, pheno_fn, num_folds, random_state=random_state, num_pcs=num_pcs, num_snps_in_memory=num_snps_in_memory, interpolate_delta=False, cov_fn=cov_fn)
 
-    best_k, best_delta, best_obj, best_snps = fss.perform_selection(k_values, delta_values, output_prefix=output_prefix, select_by_ll=select_by_ll, strategy = strategy, penalty=penalty)
+    # go!
+    fss = FeatureSelectionStrategy(
+        bed_fn,
+        pheno_fn,
+        num_folds,
+        random_state=random_state,
+        num_pcs=num_pcs,
+        num_snps_in_memory=num_snps_in_memory,
+        interpolate_delta=False,
+        cov_fn=cov_fn,
+    )
+
+    best_k, best_delta, best_obj, best_snps = fss.perform_selection(
+        k_values,
+        delta_values,
+        output_prefix=output_prefix,
+        select_by_ll=select_by_ll,
+        strategy=strategy,
+        penalty=penalty,
+    )
     res = {
-           'best_k':best_k,
-           'best_delta':best_delta,
-           'best_obj':best_obj, 
-           'best_snps':best_snps
-           }
+        "best_k": best_k,
+        "best_delta": best_delta,
+        "best_obj": best_obj,
+        "best_snps": best_snps,
+    }
     return res
-    
+
 
 if __name__ == "__main__":
     result = runselect()
-
```

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/feature_selection_two_kernel.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_two_kernel.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,23 +19,32 @@
 
 from fastlmm.association.LocoGwas import FastGwas
 import fastlmm.inference.linear_regression as lin_reg
 
 
 class FeatureSelectionInSample(object):
 
-    def __init__(self, n_folds=5, measure="mse", n_k_grid=7, max_log_k=10, order_by_lmm=False, random_state=None, debug=False):
+    def __init__(
+        self,
+        n_folds=5,
+        measure="mse",
+        n_k_grid=7,
+        max_log_k=10,
+        order_by_lmm=False,
+        random_state=None,
+        debug=False,
+    ):
         """set up two kernel feature selection
-    
+
         Parameters
         ----------
         n_folds : int
             Number of repeats for shuffle split
 
-        measure : string ("mse" or "ll")  
+        measure : string ("mse" or "ll")
             Criterion to be used to measure predition accuracy
 
         n_k_grid : int
             Number of k-values to search
 
         max_log_k : int
             Maximum search value for number of snps in log2-space (i.e. 2^max_log_k)
@@ -60,26 +69,29 @@
 
         self.n_folds = n_folds
         self.n_k_grid = n_k_grid
 
         self.mse = np.zeros((self.n_folds, self.n_k_grid))
         self.ll = np.zeros((self.n_folds, self.n_k_grid))
 
-        self.grid_k = [int(k) for k in np.logspace(0, max_log_k, base=2, num=self.n_k_grid, endpoint=True)]
+        self.grid_k = [
+            int(k)
+            for k in np.logspace(0, max_log_k, base=2, num=self.n_k_grid, endpoint=True)
+        ]
         print(self.grid_k)
         self.random_state = random_state
         self.mixes = np.zeros((self.n_folds, self.n_k_grid))
         self.h2 = np.zeros((self.n_folds, self.n_k_grid))
         self.deltas = np.zeros((self.n_folds, self.n_k_grid))
 
         self.debug = False
 
     def run_select(self, G0, G_bg, y, cov=None):
         """set up two kernel feature selection
-    
+
         Parameters
         ----------
         G0 : numpy array of shape (num_ind, num_snps)
             Data matrix from which foreground snps will be selected
 
         G0_bg : numpy array of shape (num_ind, num_snps)
             Data matrix containing background snps on which will be conditioned
@@ -94,43 +106,48 @@
         -------
         best_k, feat_idx, best_mix, best_delta: tuple(int, np.array(int), float, float)
             best_k is the best number of SNPs selected,
             feat_idx is a np.array of integers denoting the indices of these snps,
             best_mix is the best mixing coefficient between foreground and background kernel,
             best_delta is the best regularization coefficient
         """
-        with patch.dict('os.environ', {'ARRAY_MODULE': 'numpy'}) as _:
+        with patch.dict("os.environ", {"ARRAY_MODULE": "numpy"}) as _:
 
             num_ind = len(y)
 
             if cov is None:
-                cov = np.ones((num_ind,1))
+                cov = np.ones((num_ind, 1))
             else:
                 logging.info("normalizing covariates")
                 cov = cov.copy()
-                cov = 1./np.sqrt((cov**2).sum() / float(cov.shape[0])) * cov
+                cov = 1.0 / np.sqrt((cov**2).sum() / float(cov.shape[0])) * cov
             cov.flags.writeable = False
-        
+
             # normalize to diag(K) = N
-            norm_factor = 1./np.sqrt((G_bg**2).sum() / float(G_bg.shape[0]))
+            norm_factor = 1.0 / np.sqrt((G_bg**2).sum() / float(G_bg.shape[0]))
 
             # we copy in case G and G_bg are pointing to the same object
             G_bg = norm_factor * G_bg
-       
+
             K_bg_full = G_bg.dot(G_bg.T)
             K_bg_full.flags.writeable = False
-        
+
             # some asserts
             np.testing.assert_almost_equal(sum(np.diag(K_bg_full)), G_bg.shape[0])
             if self.debug:
-                norm_factor_check = 1./np.sqrt(G_bg.shape[1])
-                np.testing.assert_array_almost_equal(norm_factor, norm_factor_check, decimal=1)
-            
-
-            for kfold_idx, (train_idx, test_idx) in enumerate(KFold(n_splits=self.n_folds, random_state=self.random_state, shuffle=True).split(list(range(num_ind)))):
+                norm_factor_check = 1.0 / np.sqrt(G_bg.shape[1])
+                np.testing.assert_array_almost_equal(
+                    norm_factor, norm_factor_check, decimal=1
+                )
+
+            for kfold_idx, (train_idx, test_idx) in enumerate(
+                KFold(
+                    n_splits=self.n_folds, random_state=self.random_state, shuffle=True
+                ).split(list(range(num_ind)))
+            ):
 
                 t0 = time.time()
                 logging.info("running fold: %i" % kfold_idx)
 
                 y_train = y.take(train_idx, axis=0)
                 y_test = y.take(test_idx, axis=0)
                 G0_train = G0.take(train_idx, axis=0)
@@ -149,182 +166,238 @@
                 G0_test.flags.writeable = False
                 G_bg_train.flags.writeable = False
                 G_bg_test.flags.writeable = False
                 cov_train.flags.writeable = False
                 cov_test.flags.writeable = False
 
                 # precompute background kernel
-                K_bg_train = K_bg_full.take(train_idx, axis=0).take(train_idx, axis=1) 
+                K_bg_train = K_bg_full.take(train_idx, axis=0).take(train_idx, axis=1)
                 K_bg_train.flags.writeable = False
 
                 if self.measure != "mse":
                     K_bg_test = K_bg_full.take(test_idx, axis=0).take(test_idx, axis=1)
                     K_bg_test.flags.writeable = False
 
                 # rank features
                 if self.order_by_lmm:
                     logging.info("using linear mixed model to rank features")
                     t0 = time.time()
-                    gwas = FastGwas(G_bg_train, G0_train, y_train, delta=None, train_pcs=None, mixing=0.0, cov=cov_train)
+                    gwas = FastGwas(
+                        G_bg_train,
+                        G0_train,
+                        y_train,
+                        delta=None,
+                        train_pcs=None,
+                        mixing=0.0,
+                        cov=cov_train,
+                    )
                     gwas.run_gwas()
                     _pval = gwas.p_values
-                    logging.info("time taken: %s" % (str(time.time()-t0)))
+                    logging.info("time taken: %s" % (str(time.time() - t0)))
                 else:
                     logging.info("using linear regression to rank features")
-                    _F,_pval = lin_reg.f_regression_block(lin_reg.f_regression_cov_alt, G0_train, y_train, blocksize=10000, C=cov_train)
+                    _F, _pval = lin_reg.f_regression_block(
+                        lin_reg.f_regression_cov_alt,
+                        G0_train,
+                        y_train,
+                        blocksize=10000,
+                        C=cov_train,
+                    )
 
                 feat_idx = np.argsort(_pval)
-            
+
                 for k_idx, max_k in enumerate(self.grid_k):
 
                     feat_idx_subset = feat_idx[0:max_k]
                     G_fs_train = G0_train.take(feat_idx_subset, axis=1)
                     G_fs_test = G0_test.take(feat_idx_subset, axis=1)
 
                     # normalize to sum(diag)=N
-                    norm_factor = 1./np.sqrt((G_fs_train**2).sum() / float(G_fs_train.shape[0]))
+                    norm_factor = (
+                        1.0
+                        / np.sqrt(
+                            (G_fs_train**2).sum() / float(G_fs_train.shape[0])
+                        ).item()
+                    )
 
                     G_fs_train *= norm_factor
                     G_fs_test *= norm_factor
-                                
+
                     G_fs_train.flags.writeable = False
                     G_fs_test.flags.writeable = False
 
                     # asserts
                     if self.debug:
                         norm_factor_check = 1.0 / np.sqrt(max_k)
-                        np.testing.assert_array_almost_equal(norm_factor, norm_factor_check, decimal=1)
-                        np.testing.assert_almost_equal(sum(np.diag(G_fs_train.dot(G_fs_train.T))), G_fs_train.shape[0])
+                        np.testing.assert_array_almost_equal(
+                            norm_factor, norm_factor_check, decimal=1
+                        )
+                        np.testing.assert_almost_equal(
+                            sum(np.diag(G_fs_train.dot(G_fs_train.T))),
+                            G_fs_train.shape[0],
+                        )
 
                     logging.info("k: %i" % (max_k))
 
                     # use LMM
                     from fastlmm.inference.lmm_cov import LMM as fastLMM
 
                     if G_bg_train.shape[1] <= G_bg_train.shape[0]:
-                        lmm = fastLMM(X=cov_train, Y=y_train[:,np.newaxis], G=G_bg_train)
+                        lmm = fastLMM(
+                            X=cov_train, Y=y_train[:, np.newaxis], G=G_bg_train
+                        )
                     else:
-                        lmm = fastLMM(X=cov_train, Y=y_train[:,np.newaxis], K=K_bg_train)
+                        lmm = fastLMM(
+                            X=cov_train, Y=y_train[:, np.newaxis], K=K_bg_train
+                        )
 
                     W = G_fs_train.copy()
-                    UGup,UUGup = lmm.rotate(W)
-                
+                    UGup, UUGup = lmm.rotate(W)
+
                     i_up = np.zeros((G_fs_train.shape[1]), dtype=bool)
                     i_G1 = np.ones((G_fs_train.shape[1]), dtype=bool)
                     t0 = time.time()
-                    res = lmm.findH2_2K(nGridH2=10, minH2=0.0, maxH2=0.99999, i_up=i_up, i_G1=i_G1, UW=UGup, UUW=UUGup)
-                    logging.info("time taken for k=%i: %s" % (max_k, str(time.time()-t0)))
-                
+                    res = lmm.findH2_2K(
+                        nGridH2=10,
+                        minH2=0.0,
+                        maxH2=0.99999,
+                        i_up=i_up,
+                        i_G1=i_G1,
+                        UW=UGup,
+                        UUW=UUGup,
+                    )
+                    logging.info(
+                        "time taken for k=%i: %s" % (max_k, str(time.time() - t0))
+                    )
+
                     # recover a2 from alternate parameterization
                     a2 = res["h2_1"] / float(res["h2"] + res["h2_1"])
                     h2 = res["h2"] + res["h2_1"]
-                    delta = (1-h2) / h2
-                    #res_cov = res
-
+                    delta = (1 - h2) / h2
+                    # res_cov = res
 
                     # do final prediction using lmm.py
                     from fastlmm.inference import LMM
+
                     lmm = LMM(forcefullrank=False)
                     lmm.setG(G0=G_bg_train, G1=G_fs_train, a2=a2)
                     lmm.setX(cov_train)
                     lmm.sety(y_train)
 
                     # we take an additional step to estimate betas on covariates (not given from new model)
                     res = lmm.nLLeval(delta=delta, REML=True)
-                
+
                     # predict on test set
                     lmm.setTestData(Xstar=cov_test, G0star=G_bg_test, G1star=G_fs_test)
                     out = lmm.predictMean(beta=res["beta"], delta=delta)
 
                     mse = mean_squared_error(y_test, out)
                     logging.info("mse: %f" % (mse))
 
                     self.mse[kfold_idx, k_idx] = mse
 
                     self.mixes[kfold_idx, k_idx] = a2
                     self.deltas[kfold_idx, k_idx] = delta
 
                     if self.measure != "mse":
-                        K_test_test = a2 * G_fs_test.dot(G_fs_test.T) + (1.0-a2) * K_bg_test 
-                        ll = lmm.nLLeval_test(y_test, res["beta"], sigma2=res["sigma2"], delta=delta, Kstar_star=K_test_test, robust=True)
+                        K_test_test = (
+                            a2 * G_fs_test.dot(G_fs_test.T) + (1.0 - a2) * K_bg_test
+                        )
+                        ll = lmm.nLLeval_test(
+                            y_test,
+                            res["beta"],
+                            sigma2=res["sigma2"],
+                            delta=delta,
+                            Kstar_star=K_test_test,
+                            robust=True,
+                        )
 
                         if self.debug:
-                            ll2 = lmm.nLLeval_test(y_test, res["beta"], sigma2=res["sigma2"], delta=delta, Kstar_star=None, robust=True)
+                            ll2 = lmm.nLLeval_test(
+                                y_test,
+                                res["beta"],
+                                sigma2=res["sigma2"],
+                                delta=delta,
+                                Kstar_star=None,
+                                robust=True,
+                            )
                             np.testing.assert_almost_equal(ll, ll2, decimal=4)
 
                         logging.info("ll: %f" % (ll))
-                        self.ll[kfold_idx, k_idx]  = ll
-                    
+                        self.ll[kfold_idx, k_idx] = ll
 
-                logging.info("time taken for fold: %s" % str(time.time()-t0))
-        
+                logging.info("time taken for fold: %s" % str(time.time() - t0))
 
             best_k, best_mix, best_delta = self.select_best_k()
 
-            logging.info("best_k: %i, best_mix: %f, best_delta: %f" % (best_k, best_mix, best_delta))
+            logging.info(
+                "best_k: %i, best_mix: %f, best_delta: %f"
+                % (best_k, best_mix, best_delta)
+            )
 
-            # final scan 
+            # final scan
             if self.order_by_lmm:
                 logging.info("final scan using LMM")
-                gwas = FastGwas(G_bg, G0, y, delta=None, train_pcs=None, mixing=0.0, cov=cov)
+                gwas = FastGwas(
+                    G_bg, G0, y, delta=None, train_pcs=None, mixing=0.0, cov=cov
+                )
                 gwas.run_gwas()
                 _pval = gwas.p_values
                 feat_idx = np.argsort(_pval)[0:best_k]
             else:
                 logging.info("final scan using LR")
-                _F,_pval = lin_reg.f_regression_block(lin_reg.f_regression_cov_alt, G0, y, C=cov, blocksize=10000)
-        
+                _F, _pval = lin_reg.f_regression_block(
+                    lin_reg.f_regression_cov_alt, G0, y, C=cov, blocksize=10000
+                )
+
             logging.info("number of snps selected: %i" % (best_k))
 
             return best_k, feat_idx, best_mix, best_delta
 
-
     def select_best_k(self):
         """after running cross-vlidation, choose best number of snps
 
         Returns
         -------
         best_k, best_mix, best_delta: tuple(int, float, float)
             best_k is the best number of SNPs selected,
             best_mix is the best mixing coefficient between foreground and background kernel,
             best_delta is the best regularization coefficient
         """
-        with patch.dict('os.environ', {'ARRAY_MODULE': 'numpy'}) as _:
+        with patch.dict("os.environ", {"ARRAY_MODULE": "numpy"}) as _:
 
             perf = self.mse
 
             if self.measure == "ll":
                 logging.info("using nLL to select best_k")
                 perf = self.ll
             else:
                 logging.info("using MSE to select best_k")
 
             min_ = perf.mean(axis=0)
             arg_min_k = np.argmin(min_)
 
-
             best_k = self.grid_k[arg_min_k]
-            best_mix = np.median(self.mixes[:,arg_min_k])
-            best_delta = np.median(self.deltas[:,arg_min_k])
+            best_mix = np.median(self.mixes[:, arg_min_k])
+            best_delta = np.median(self.deltas[:, arg_min_k])
             return best_k, best_mix, best_delta
 
-
     def plot_results(self, measure="mse"):
         """
         visualize trained model, either measure="ll" or measure="mse"
         """
         import pylab
+
         if measure == "ll":
             pylab.plot(self.grid_k, self.ll.mean(axis=0).T, "-x", label=self.grid_k)
             pylab.ylabel("-ll")
         else:
             pylab.plot(self.grid_k, self.mse.mean(axis=0).T, "-x", label=self.grid_k)
             pylab.ylabel("mse")
-        #pylab.yscale("log")
-        #pylab.xscale("log")
+        # pylab.yscale("log")
+        # pylab.xscale("log")
         pylab.xlabel("num features in foreground")
-        
+
         pylab.grid(True)
         pylab.title(measure)
-        #pylab.legend()
+        # pylab.legend()
         pylab.show()
-
```

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/kernel_ridge_cv.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/kernel_ridge_cv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import time
 import os
 import sys
 
-import scipy as SP
 import numpy as np
 import sklearn.metrics as SKM
 
 import sklearn.feature_selection as SKFS
-import sklearn.model_selection as SKCV 
+import sklearn.model_selection as SKCV
 import sklearn.metrics as SKM
 
 from pysnptools.util.mapreduce1.distributable import *
 from pysnptools.util.mapreduce1.runner import *
 import fastlmm.pyplink.plink as plink
 import fastlmm.pyplink.Bed as Bed
 import fastlmm.pyplink.snpset.PositionRange as PositionRange
 import fastlmm.pyplink.snpset.SnpSetAndName as SnpSetAndName
 import fastlmm.util.util as util
 import fastlmm.inference as fastlmm
 
 from .feature_selection_cv import load_snp_data
-from six.moves import range
 
-class KernelRidgeCV(): # implements IDistributable
-    '''
+
+class KernelRidgeCV:  # implements IDistributable
+    """
     A class for running cross-validation on kernel ridge regression: The method determines the best regularization parameter alpha by
     cross-validating it.
 
     The Rdige regression optimization problem is given by:
     min  1./2n*||y - Xw||_2^2 + alpha * ||w||_2
-    '''
+    """
 
-    def __init__(self, bed_fn, pheno_fn, num_folds,random_state=None,cov_fn=None,offset=True):
+    def __init__(
+        self, bed_fn, pheno_fn, num_folds, random_state=None, cov_fn=None, offset=True
+    ):
         """set up kernel ridge regression
         ----------
 
         bed_fn : str
             File name of binary SNP file
 
         pheno_fn : str
@@ -48,28 +47,28 @@
 
         cov_fn : str, optional, default=None
             File name of covariates file
 
         offset : bool, default=True
             adds offset to the covariates specified in cov_fn, if necessary
         """
- 
+
         # data file names
         self.bed_fn = bed_fn
         self.pheno_fn = pheno_fn
         self.cov_fn = cov_fn
 
         # optional parameters
         self.num_folds = num_folds
         self.fold_to_train_data = None
         self.random_state = random_state
         self.offset = offset
         self.K = None
 
-    def perform_selection(self,delta_values,strategy,plots_fn=None,results_fn=None):
+    def perform_selection(self, delta_values, strategy, plots_fn=None, results_fn=None):
         """Perform delta selection for kernel ridge regression
 
         delta_values : array-like, shape = [n_steps_delta]
             Array of delta values to test
 
         strategy : {'full_cv','insample_cv'}
             Strategy to perform feature selection:
@@ -83,103 +82,110 @@
             file name for saving cross-validation results. if not specified, nothing is saved
         Returns
         -------
         best_delta : float
             best regularization parameter delta for ridge regression
 
         """
-        import matplotlib.pylab as PLT 
-
+        import matplotlib.pylab as PLT
 
         # use precomputed data if available
         if self.K == None:
             self.setup_kernel()
 
-        print('run selection strategy %s'%strategy)
+        print("run selection strategy %s" % strategy)
 
         model = fastlmm.lmm()
         nInds = self.K.shape[0]
-   
-        if strategy=='insample':
+
+        if strategy == "insample":
             # take delta with largest likelihood
             model.setK(self.K)
             model.sety(self.y)
             model.setX(self.X)
             best_delta = None
-            best_nLL = SP.inf
+            best_nLL = np.inf
 
             # evaluate negative log-likelihood for different values of alpha
-            nLLs = SP.zeros(len(delta_values))
+            nLLs = np.zeros(len(delta_values))
             for delta_idx, delta in enumerate(delta_values):
-                res = model.nLLeval(delta=delta,REML=True)
+                res = model.nLLeval(delta=delta, REML=True)
                 if res["nLL"] < best_nLL:
                     best_delta = delta
                     best_nLL = res["nLL"]
 
-                nLLs[delta_idx] = res['nLL']
+                nLLs[delta_idx] = res["nLL"]
 
             fig = PLT.figure()
             fig.add_subplot(111)
-            PLT.semilogx(delta_values,nLLs,color='g',linestyle='-')
-            PLT.axvline(best_delta,color='r',linestyle='--')
-            PLT.xlabel('logdelta')
-            PLT.ylabel('nLL')
-            PLT.title('Best delta: %f'%best_delta)
+            PLT.semilogx(delta_values, nLLs, color="g", linestyle="-")
+            PLT.axvline(best_delta, color="r", linestyle="--")
+            PLT.xlabel("logdelta")
+            PLT.ylabel("nLL")
+            PLT.title("Best delta: %f" % best_delta)
             PLT.grid(True)
-            if plots_fn!=None:
+            if plots_fn != None:
                 PLT.savefig(plots_fn)
-            if results_fn!=None:
-                SP.savetxt(results_fn, SP.vstack((delta_values,nLLs)).T,delimiter='\t',header='delta\tnLLs')
-            
-        if strategy=='cv':
+            if results_fn != None:
+                np.savetxt(
+                    results_fn,
+                    np.vstack((delta_values, nLLs)).T,
+                    delimiter="\t",
+                    header="delta\tnLLs",
+                )
+
+        if strategy == "cv":
             # run cross-validation for determining best delta
-            kfoldIter = SKCV.KFold(n_splits=self.num_folds,shuffle=True,random_state=self.random_state).split(list(range(nInds)))
-            Ypred = SP.zeros((len(delta_values),nInds))
-            for Itrain,Itest in kfoldIter:
-                model.setK(self.K[Itrain][:,Itrain])
+            kfoldIter = SKCV.KFold(
+                n_splits=self.num_folds, shuffle=True, random_state=self.random_state
+            ).split(list(range(nInds)))
+            Ypred = np.zeros((len(delta_values), nInds))
+            for Itrain, Itest in kfoldIter:
+                model.setK(self.K[Itrain][:, Itrain])
                 model.sety(self.y[Itrain])
                 model.setX(self.X[Itrain])
 
-                model.setTestData(Xstar=self.X[Itest],K0star=self.K[Itest][:,Itrain])
-                
-                for delta_idx,delta in enumerate(delta_values):
-                    res = model.nLLeval(delta=delta,REML=True)
-                    beta = res['beta']
-                    Ypred[delta_idx,Itest] = model.predictMean(beta=beta,delta=delta)
+                model.setTestData(Xstar=self.X[Itest], K0star=self.K[Itest][:, Itrain])
+
+                for delta_idx, delta in enumerate(delta_values):
+                    res = model.nLLeval(delta=delta, REML=True)
+                    beta = res["beta"]
+                    Ypred[delta_idx, Itest] = model.predictMean(beta=beta, delta=delta)
 
-            MSE = SP.zeros(len(delta_values))
+            MSE = np.zeros(len(delta_values))
             for i in range(len(delta_values)):
-                MSE[i] = SKM.mean_squared_error(self.y,Ypred[i])
-            idx_bestdelta = SP.argmin(MSE)
+                MSE[i] = SKM.mean_squared_error(self.y, Ypred[i])
+            idx_bestdelta = np.argmin(MSE)
             best_delta = delta_values[idx_bestdelta]
 
             fig = PLT.figure()
             fig.add_subplot(111)
-            PLT.semilogx(delta_values,MSE,color='g',linestyle='-')
-            PLT.axvline(best_delta,color='r',linestyle='--')
-            PLT.xlabel('logdelta')
-            PLT.ylabel('MSE')
+            PLT.semilogx(delta_values, MSE, color="g", linestyle="-")
+            PLT.axvline(best_delta, color="r", linestyle="--")
+            PLT.xlabel("logdelta")
+            PLT.ylabel("MSE")
             PLT.grid(True)
-            PLT.title('Best delta: %f'%best_delta)
-            if plots_fn!=None:
+            PLT.title("Best delta: %f" % best_delta)
+            if plots_fn != None:
                 PLT.savefig(plots_fn)
-            if results_fn!=None:
-                SP.savetxt(results_fn, SP.vstack((delta_values,MSE)).T,delimiter='\t',header='delta\tnLLs')
+            if results_fn != None:
+                np.savetxt(
+                    results_fn,
+                    np.vstack((delta_values, MSE)).T,
+                    delimiter="\t",
+                    header="delta\tnLLs",
+                )
 
         return best_delta
-    
 
-    
     def setup_kernel(self):
-        """precomputes the kernel
-        """
+        """precomputes the kernel"""
         print("loading data...")
-        G, self.X, self.y = load_snp_data(self.bed_fn, self.pheno_fn, cov_fn=self.cov_fn,offset=self.offset)
+        G, self.X, self.y = load_snp_data(
+            self.bed_fn, self.pheno_fn, cov_fn=self.cov_fn, offset=self.offset
+        )
         print("done.")
         print("precomputing kernel... ")
         nSnps = G.shape[1]
-        self.K = 1./nSnps * np.dot(G,G.T)
+        self.K = 1.0 / nSnps * np.dot(G, G.T)
         print("done.")
         del G
-   
-
-
```

### Comparing `fastlmm-0.6.7/fastlmm/feature_selection/test.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,124 +1,131 @@
 import numpy as np
 import logging
 
 from fastlmm.feature_selection import FeatureSelectionStrategy, load_snp_data
 from pysnptools.snpreader import Bed
 import pysnptools.util.pheno as pstpheno
-import fastlmm.inference.linear_regression as lin_reg 
+import fastlmm.inference.linear_regression as lin_reg
 from pysnptools.snpreader import Hdf5
 from pysnptools.snpreader import Dat
 from pysnptools.snpreader import Ped
 
 #  sklearn
 from sklearn.model_selection import KFold
 from pysnptools.standardizer import Unit
 
 from fastlmm.inference import getLMM
 import unittest
 import os.path
 from unittest.mock import patch
 
 import pysnptools.util
-from fastlmm.feature_selection.feature_selection_two_kernel import FeatureSelectionInSample
+from fastlmm.feature_selection.feature_selection_two_kernel import (
+    FeatureSelectionInSample,
+)
 import fastlmm.util.standardizer as stdizer
 
 
-
 class TestTwoKernelFeatureSelection(unittest.TestCase):
     @classmethod
     def setUpClass(self):
         currentFolder = os.path.dirname(os.path.realpath(__file__))
         self.snp_fn = currentFolder + "/../../tests/datasets/mouse/alldata"
-        self.pheno_fn = currentFolder + "/../../tests/datasets/mouse/pheno_10_causals.txt"
-        #self.cov_fn = currentFolder + "/examples/toydata.cov"
+        self.pheno_fn = (
+            currentFolder + "/../../tests/datasets/mouse/pheno_10_causals.txt"
+        )
+        # self.cov_fn = currentFolder + "/examples/toydata.cov"
 
         # load data
         ###################################################################
-        snp_reader = Bed(self.snp_fn,count_A1=False)
+        snp_reader = Bed(self.snp_fn, count_A1=False)
         pheno = pstpheno.loadOnePhen(self.pheno_fn)
-        #cov = pstpheno.loadPhen(self.cov_fn)
-        
+        # cov = pstpheno.loadPhen(self.cov_fn)
+
         # intersect sample ids
         snp_reader, pheno = pysnptools.util.intersect_apply([snp_reader, pheno])
-        
-        self.G = snp_reader.read(order='C').val
+
+        self.G = snp_reader.read(order="C").val
         self.G = stdizer.Unit().standardize(self.G)
         self.G.flags.writeable = False
-        self.y = pheno['vals'][:,0]
+        self.y = pheno["vals"][:, 0]
         self.y.flags.writeable = False
 
         # load pcs
-        #self.G_cov = cov['vals']
+        # self.G_cov = cov['vals']
         self.G_cov = np.ones((len(self.y), 1))
         self.G_cov.flags.writeable = False
-        
 
     def test_regression_lmm(self):
 
-
         # invoke fs
-        select = FeatureSelectionInSample(n_folds=2, max_log_k=6, order_by_lmm=True, measure="mse", random_state=42)
-        best_k, feat_idx, best_mix, best_delta = select.run_select(self.G, self.G, self.y, cov=self.G_cov)    
-    
+        select = FeatureSelectionInSample(
+            n_folds=2, max_log_k=6, order_by_lmm=True, measure="mse", random_state=42
+        )
+        best_k, feat_idx, best_mix, best_delta = select.run_select(
+            self.G, self.G, self.y, cov=self.G_cov
+        )
+
         # print results
         print("best_k:", best_k)
         print("best_mix:", best_mix)
         print("best_delta:", best_delta)
 
         self.assertEqual(best_k, 64)
         self.assertAlmostEqual(best_mix, 0.8621642030968627, places=6)
         self.assertAlmostEqual(best_delta, 0.7255878551207211, places=6)
 
-
     def test_regression_lr(self):
 
         # invoke fs
-        select = FeatureSelectionInSample(n_folds=2, max_log_k=6, order_by_lmm=False, measure="mse", random_state=42)
-        best_k, feat_idx, best_mix, best_delta = select.run_select(self.G, self.G, self.y, cov=self.G_cov)    
-    
+        select = FeatureSelectionInSample(
+            n_folds=2, max_log_k=6, order_by_lmm=False, measure="mse", random_state=42
+        )
+        best_k, feat_idx, best_mix, best_delta = select.run_select(
+            self.G, self.G, self.y, cov=self.G_cov
+        )
+
         # print results
         print("best_k:", best_k)
         print("best_mix:", best_mix)
         print("best_delta:", best_delta)
 
         self.assertEqual(best_k, 32)
         self.assertAlmostEqual(best_mix, 0.6786566031577429, places=6)
         self.assertAlmostEqual(best_delta, 0.70148446599200931, places=6)
 
 
 class TestFeatureSelection(unittest.TestCase):
     @classmethod
     def setUpClass(self):
         currentFolder = os.path.dirname(os.path.realpath(__file__))
-        self.snpreader_bed = Bed(currentFolder + "/examples/toydata.5chrom.bed",count_A1=False)
-        #Creating Hdf5 data ...
-        #snpData = self.snpreader_bed.read()
-        #Hdf5.write(snpData, currentFolder + "/examples/toydata.snpmajor.hdf5")
-        #Hdf5.write(snpData, currentFolder + "/examples/toydata.iidmajor.hdf5",snp_major=False)
-
-        #Creating Dat data ...
-        #snpData = self.snpreader_bed.read()
-        #Dat.write(snpData, currentFolder + "/examples/toydata.dat")
+        self.snpreader_bed = Bed(
+            currentFolder + "/examples/toydata.5chrom.bed", count_A1=False
+        )
+        # Creating Hdf5 data ...
+        # snpData = self.snpreader_bed.read()
+        # Hdf5.write(snpData, currentFolder + "/examples/toydata.snpmajor.hdf5")
+        # Hdf5.write(snpData, currentFolder + "/examples/toydata.iidmajor.hdf5",snp_major=False)
+
+        # Creating Dat data ...
+        # snpData = self.snpreader_bed.read()
+        # Dat.write(snpData, currentFolder + "/examples/toydata.dat")
 
         ###Creating Ped data ...
-        #snpData = self.snpreader_bed.read()
-        #Ped.write(snpData, currentFolder + "/examples/toydata.ped")
-        #fromPed = Ped(currentFolder + "/examples/toydata").read()
-        #self.assertTrue(np.allclose(snpData.val, fromPed.val, rtol=1e-05, atol=1e-05))
-        
-        
+        # snpData = self.snpreader_bed.read()
+        # Ped.write(snpData, currentFolder + "/examples/toydata.ped")
+        # fromPed = Ped(currentFolder + "/examples/toydata").read()
+        # self.assertTrue(np.allclose(snpData.val, fromPed.val, rtol=1e-05, atol=1e-05))
+
         self.snpreader_hdf5 = Hdf5(currentFolder + "/examples/toydata.snpmajor.hdf5")
         self.snpreader_dat = Dat(currentFolder + "/examples/toydata.dat")
         self.snpreader_ped = Ped(currentFolder + "/examples/toydata")
         self.pheno_fn = currentFolder + "/examples/toydata.phe"
         self.pheno_shuffleplus_fn = currentFolder + "/examples/toydata.shufflePlus.phe"
 
- 
-
     """
     make sure the used pca yields the same result as standard pca
     def test_pca(self):
 
         from sklearn.decomposition import PCA, KernelPCA
 
         print "testing PCA"
@@ -139,15 +146,14 @@
             pc_1 = fss.pcs[:,i]
             pc_2 = pcs[:,i]
             # sign -1 if signs different, 1 else
             sign = np.sign(pc_1[0]) * np.sign(pc_2[0])
 
             np.testing.assert_array_almost_equal(pc_1, sign*pc_2)
     """
- 
 
     def test_regression_bed(self):
         self.regression(self.snpreader_bed, self.regular_regression_answers)
 
     def test_regression_hdf5(self):
         self.regression(self.snpreader_hdf5, self.regular_regression_answers)
 
@@ -155,241 +161,449 @@
         self.regression(self.snpreader_dat, self.regular_regression_answers)
 
     def test_regression_ped(self):
         self.regression(self.snpreader_ped, self.regular_regression_answers)
 
     regular_regression_answers = (22, 20.085536923, 61.2448170241, 0.67586545761317196)
     cov_pca_regression_answers = (22, 20.085536923, 61.8146293815, 0.692761716513)
-    cov_pca_insample_cv_regression_answers = (22, 1.6513737331988527, 63.6062289765, 0.71724685708485092)
+    cov_pca_insample_cv_regression_answers = (
+        22,
+        1.6513737331988527,
+        63.6062289765,
+        0.71724685708485092,
+    )
 
     def test_regression_cov_pcs(self):
         currentFolder = os.path.dirname(os.path.realpath(__file__))
         cov_fn = currentFolder + "/examples/toydata.cov"
-        self.regression(self.snpreader_bed, self.cov_pca_regression_answers, cov_fn=cov_fn, num_pcs=3)
+        self.regression(
+            self.snpreader_bed,
+            self.cov_pca_regression_answers,
+            cov_fn=cov_fn,
+            num_pcs=3,
+        )
 
     def test_regression_cov_pcs_insample_cv(self):
         currentFolder = os.path.dirname(os.path.realpath(__file__))
         cov_fn = currentFolder + "/examples/toydata.cov"
-        self.regression(self.snpreader_bed, self.cov_pca_insample_cv_regression_answers, cov_fn=cov_fn, num_pcs=3, strategy = "insample_cv", delta=5)
-
-    def regression(self, snpreader, answers, cov_fn=None, num_pcs=0, strategy = "lmm_full_cv", delta=7):
+        self.regression(
+            self.snpreader_bed,
+            self.cov_pca_insample_cv_regression_answers,
+            cov_fn=cov_fn,
+            num_pcs=3,
+            strategy="insample_cv",
+            delta=5,
+        )
+
+    def regression(
+        self,
+        snpreader,
+        answers,
+        cov_fn=None,
+        num_pcs=0,
+        strategy="lmm_full_cv",
+        delta=7,
+    ):
         """
         compare against previous results of this code base
         """
-    
+
         # set up grid
         ##############################
         num_steps_delta = 5
         num_steps_k = 5
         num_folds = 2
 
-
         # log_2 space and all SNPs
-        k_values = np.array(np.logspace(0, 9, base=2, num=num_steps_k, endpoint=True),dtype=np.int64).tolist() + [10000]
-        #k_values = np.logspace(0, 9, base=2, num=num_steps_k, endpoint=True).tolist() + [10000]
-        delta_values = np.logspace(-3, 3, endpoint=True, num=num_steps_delta, base=np.exp(1))
+        k_values = np.array(
+            np.logspace(0, 9, base=2, num=num_steps_k, endpoint=True), dtype=np.int64
+        ).tolist() + [10000]
+        # k_values = np.logspace(0, 9, base=2, num=num_steps_k, endpoint=True).tolist() + [10000]
+        delta_values = np.logspace(
+            -3, 3, endpoint=True, num=num_steps_delta, base=np.exp(1)
+        )
         random_state = 42
 
         output_prefix = None
 
         # select by LL
-        fss = FeatureSelectionStrategy(snpreader, self.pheno_fn, num_folds, random_state=random_state, cov_fn=cov_fn, num_pcs=num_pcs, interpolate_delta=True,count_A1=False)
-        best_k, best_delta, best_obj, best_snps = fss.perform_selection(k_values, delta_values, strategy, output_prefix=output_prefix, select_by_ll=True,create_pdf=False)
-        
+        fss = FeatureSelectionStrategy(
+            snpreader,
+            self.pheno_fn,
+            num_folds,
+            random_state=random_state,
+            cov_fn=cov_fn,
+            num_pcs=num_pcs,
+            interpolate_delta=True,
+            count_A1=False,
+        )
+        best_k, best_delta, best_obj, best_snps = fss.perform_selection(
+            k_values,
+            delta_values,
+            strategy,
+            output_prefix=output_prefix,
+            select_by_ll=True,
+            create_pdf=False,
+        )
+
         self.assertEqual(best_k, answers[0])
         self.assertAlmostEqual(best_delta, answers[1], delta)
-        self.assertTrue(abs(best_obj-answers[2])<.005) #accept a range answers for when standardization is done with doubles, floats, etc
+        self.assertTrue(
+            abs(best_obj - answers[2]) < 0.005
+        )  # accept a range answers for when standardization is done with doubles, floats, etc
 
         # select by MSE
-        fss = FeatureSelectionStrategy(snpreader, self.pheno_fn, num_folds, random_state=random_state, cov_fn=cov_fn, num_pcs=num_pcs, interpolate_delta=True,count_A1=False)
-        best_k, best_delta, best_obj, best_snps = fss.perform_selection(k_values, delta_values, strategy, output_prefix=output_prefix, select_by_ll=False,create_pdf=False)
-        
+        fss = FeatureSelectionStrategy(
+            snpreader,
+            self.pheno_fn,
+            num_folds,
+            random_state=random_state,
+            cov_fn=cov_fn,
+            num_pcs=num_pcs,
+            interpolate_delta=True,
+            count_A1=False,
+        )
+        best_k, best_delta, best_obj, best_snps = fss.perform_selection(
+            k_values,
+            delta_values,
+            strategy,
+            output_prefix=output_prefix,
+            select_by_ll=False,
+            create_pdf=False,
+        )
+
         self.assertEqual(best_k, answers[0])
         self.assertAlmostEqual(best_delta, answers[1], delta)
         self.assertAlmostEqual(best_obj, answers[3])
 
     def test_blocking_bed(self):
         currentFolder = os.path.dirname(os.path.realpath(__file__))
-        self.blocking(currentFolder + "/examples/toydata.5chrom.bed") # use string instead of reader, to test that strings work
+        self.blocking(
+            currentFolder + "/examples/toydata.5chrom.bed"
+        )  # use string instead of reader, to test that strings work
 
     def test_blocking_hdf5(self):
         self.blocking(self.snpreader_hdf5)
 
     def test_blocking_dat(self):
         self.blocking(self.snpreader_dat)
 
     def test_blocking_ped(self):
         self.blocking(self.snpreader_ped)
 
-
     tolerance = 1e-4
 
     def test_blocking_cov_pcs(self):
         self.blocking_cov_pcs(strategy="lmm_full_cv")
 
-    def getworkingtest_blocking_cov_pcs_insample_cv(self): #!!!
+    def getworkingtest_blocking_cov_pcs_insample_cv(self):  #!!!
         self.blocking_cov_pcs(strategy="insample_cv")
 
     @staticmethod
     def reference_file(outfile):
         #!!similar code elsewhere
-        import platform;
-        os_string=platform.platform()
+        import platform
 
-        file_path = os.path.join(os.path.dirname(os.path.realpath(__file__)),"..","..","tests")
-        windows_fn = file_path + '/expected-Windows/'+outfile
+        os_string = platform.platform()
+
+        file_path = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "..", "..", "tests"
+        )
+        windows_fn = file_path + "/expected-Windows/" + outfile
         assert os.path.exists(windows_fn), "Can't find file '{0}'".format(windows_fn)
-        debian_fn = file_path + '/expected-debian/'+outfile
-        if not os.path.exists(debian_fn): #If reference file is not in debian folder, look in windows folder
+        debian_fn = file_path + "/expected-debian/" + outfile
+        if not os.path.exists(
+            debian_fn
+        ):  # If reference file is not in debian folder, look in windows folder
             debian_fn = windows_fn
 
         if "debian" in os_string or "Linux" in os_string:
             if "Linux" in os_string:
-                logging.warning("comparing to Debian output even though found: %s" % os_string)
+                logging.warning(
+                    "comparing to Debian output even though found: %s" % os_string
+                )
             return debian_fn
         else:
             if "Windows" not in os_string:
-                logging.warning("comparing to Windows output even though found: %s" % os_string)
-            return windows_fn 
-
+                logging.warning(
+                    "comparing to Windows output even though found: %s" % os_string
+                )
+            return windows_fn
 
-    def blocking_cov_pcs(self,strategy):
+    def blocking_cov_pcs(self, strategy):
         currentFolder = os.path.dirname(os.path.realpath(__file__))
         cov_fn = currentFolder + "/examples/toydata.cov"
-        output_dir="tmp"
+        output_dir = "tmp"
         try:
             os.mkdir(output_dir)
         except:
             pass
         output_dir = output_dir + "/feature_selection"
         try:
             os.mkdir(output_dir)
         except:
             pass
-        self.blocking(self.snpreader_bed, cov_fn, num_pcs=3, strategy=strategy, output_prefix=os.path.join(output_dir,strategy))
+        self.blocking(
+            self.snpreader_bed,
+            cov_fn,
+            num_pcs=3,
+            strategy=strategy,
+            output_prefix=os.path.join(output_dir, strategy),
+        )
 
         for outfile in os.listdir(output_dir):
             referenceOutfile = TestFeatureSelection.reference_file(outfile)
 
             import fastlmm.util.util as ut
-            if outfile.lower().endswith(".pdf") or outfile == "output_prefix_report.txt" or outfile.lower().endswith("_k_pcs.txt"):
+
+            if (
+                outfile.lower().endswith(".pdf")
+                or outfile == "output_prefix_report.txt"
+                or outfile.lower().endswith("_k_pcs.txt")
+            ):
                 self.assertTrue(os.path.exists(referenceOutfile))
             else:
                 delimiter = "," if outfile.lower().endswith(".csv") else "\t"
-                tmpOutfile=os.path.join(output_dir,outfile)
-                out,msg=ut.compare_mixed_files(tmpOutfile, referenceOutfile, self.tolerance,delimiter=delimiter)
+                tmpOutfile = os.path.join(output_dir, outfile)
+                out, msg = ut.compare_mixed_files(
+                    tmpOutfile, referenceOutfile, self.tolerance, delimiter=delimiter
+                )
                 if not out:
                     from pathlib import Path
+
                     msg = f"{msg}: tempOutfile={Path(tmpOutfile).read_text()} referenceOutfile={Path(referenceOutfile).read_text()}"
-                self.assertTrue(out, "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile))
-      
-     
-    def blocking(self, snpreader, cov_fn=None, num_pcs=0, output_prefix = None, strategy="lmm_full_cv"):
+                self.assertTrue(
+                    out,
+                    "msg='{0}', ref='{1}', tmp='{2}'".format(
+                        msg, referenceOutfile, tmpOutfile
+                    ),
+                )
+
+    def blocking(
+        self,
+        snpreader,
+        cov_fn=None,
+        num_pcs=0,
+        output_prefix=None,
+        strategy="lmm_full_cv",
+    ):
         """
         compare three different cases:
 
-        To control memory use, we've introduced a parameter called "num_snps_in_memory", which defaults to 100000. 
+        To control memory use, we've introduced a parameter called "num_snps_in_memory", which defaults to 100000.
         Here are the interesting cases to consider (and choose num_snps_in_memory accordingly):
 
         1) num_snps_in_memory > total_num_snps
 
-           In this case, the same code as before should be 
-           executed (except the kernel matrix on all SNPs is now cached). 
+           In this case, the same code as before should be
+           executed (except the kernel matrix on all SNPs is now cached).
 
 
         2) num_snps_in_memory < total_num_snps
             num_snps_in_memory > k (excluding all_snps)
 
-            Here, the linear regression will be blocked, 
-            while the data for cross-validation is cached, 
+            Here, the linear regression will be blocked,
+            while the data for cross-validation is cached,
             saving time for loading and re-indexing.
 
 
         3) num_snps_in_memory < total_num_snps
             num_snps_in_memory < k (excluding all_snps)
 
-            Finally, both operations - linear regression 
+            Finally, both operations - linear regression
             and building the kernel will be blocked.
 
         4,5,6) Same as #1,2,3, but with a phenos that has extra iids and for which the iids are shuffled.
 
 
         """
 
         # set up grid
         ##############################
         num_steps_delta = 5
         num_folds = 2
 
         # log_2 space and all SNPs
-        k_values = [0, 1, 5, 10, 100, 500, 700, 10000] 
-        delta_values = np.logspace(-3, 3, endpoint=True, num=num_steps_delta, base=np.exp(1))
-        
-        random_state = 42
+        k_values = [0, 1, 5, 10, 100, 500, 700, 10000]
+        delta_values = np.logspace(
+            -3, 3, endpoint=True, num=num_steps_delta, base=np.exp(1)
+        )
 
+        random_state = 42
 
         # case 1
-        fss_1 = FeatureSelectionStrategy(snpreader, self.pheno_fn, num_folds, cov_fn=cov_fn, random_state=random_state, num_pcs=num_pcs, interpolate_delta=True, num_snps_in_memory=20000,count_A1=False)
-        best_k_1, best_delta_1, best_obj_1, best_snps_1 = fss_1.perform_selection(k_values, delta_values, output_prefix=output_prefix, select_by_ll=True, strategy=strategy,create_pdf=False)
+        fss_1 = FeatureSelectionStrategy(
+            snpreader,
+            self.pheno_fn,
+            num_folds,
+            cov_fn=cov_fn,
+            random_state=random_state,
+            num_pcs=num_pcs,
+            interpolate_delta=True,
+            num_snps_in_memory=20000,
+            count_A1=False,
+        )
+        best_k_1, best_delta_1, best_obj_1, best_snps_1 = fss_1.perform_selection(
+            k_values,
+            delta_values,
+            output_prefix=output_prefix,
+            select_by_ll=True,
+            strategy=strategy,
+            create_pdf=False,
+        )
 
-        #some misc testing
+        # some misc testing
         from fastlmm.feature_selection import PerformSelectionDistributable as psd
-        perform_selection_distributable = psd.PerformSelectionDistributable(fss_1, k_values, delta_values, strategy, output_prefix, select_by_ll=True, penalty=0.0,create_pdf=False)
+
+        perform_selection_distributable = psd.PerformSelectionDistributable(
+            fss_1,
+            k_values,
+            delta_values,
+            strategy,
+            output_prefix,
+            select_by_ll=True,
+            penalty=0.0,
+            create_pdf=False,
+        )
         self.assertEqual(perform_selection_distributable.work_count, 3)
         s = perform_selection_distributable.tempdirectory
         s = str(perform_selection_distributable)
         s = "%r" % perform_selection_distributable
         from fastlmm.feature_selection.feature_selection_cv import GClass
-        s = "%r" % GClass.factory(snpreader,1000000, Unit(), 50,count_A1=False)
+
+        s = "%r" % GClass.factory(snpreader, 1000000, Unit(), 50, count_A1=False)
         s = s
         #!!making  test for each break point.
 
-
         # case 2
-        fss_2 = FeatureSelectionStrategy(snpreader, self.pheno_fn, num_folds, cov_fn=cov_fn, random_state=random_state, num_pcs=num_pcs, interpolate_delta=True, num_snps_in_memory=5000,count_A1=False)
-        best_k_2, best_delta_2, best_obj_2, best_snps_2 = fss_2.perform_selection(k_values, delta_values, output_prefix=output_prefix, select_by_ll=True, strategy=strategy,create_pdf=False)
+        fss_2 = FeatureSelectionStrategy(
+            snpreader,
+            self.pheno_fn,
+            num_folds,
+            cov_fn=cov_fn,
+            random_state=random_state,
+            num_pcs=num_pcs,
+            interpolate_delta=True,
+            num_snps_in_memory=5000,
+            count_A1=False,
+        )
+        best_k_2, best_delta_2, best_obj_2, best_snps_2 = fss_2.perform_selection(
+            k_values,
+            delta_values,
+            output_prefix=output_prefix,
+            select_by_ll=True,
+            strategy=strategy,
+            create_pdf=False,
+        )
 
         # case 3
-        fss_3 = FeatureSelectionStrategy(snpreader, self.pheno_fn, num_folds, cov_fn=cov_fn, random_state=random_state, num_pcs=num_pcs, interpolate_delta=True, num_snps_in_memory=600,count_A1=False)
-        best_k_3, best_delta_3, best_obj_3, best_snps_3 = fss_3.perform_selection(k_values, delta_values, output_prefix=output_prefix, select_by_ll=True, strategy=strategy,create_pdf=False)
+        fss_3 = FeatureSelectionStrategy(
+            snpreader,
+            self.pheno_fn,
+            num_folds,
+            cov_fn=cov_fn,
+            random_state=random_state,
+            num_pcs=num_pcs,
+            interpolate_delta=True,
+            num_snps_in_memory=600,
+            count_A1=False,
+        )
+        best_k_3, best_delta_3, best_obj_3, best_snps_3 = fss_3.perform_selection(
+            k_values,
+            delta_values,
+            output_prefix=output_prefix,
+            select_by_ll=True,
+            strategy=strategy,
+            create_pdf=False,
+        )
 
         # case 4
-        fss_4 = FeatureSelectionStrategy(snpreader, self.pheno_shuffleplus_fn, num_folds, cov_fn=cov_fn, random_state=random_state, num_pcs=num_pcs, interpolate_delta=True, num_snps_in_memory=20000,count_A1=False)
-        best_k_4, best_delta_4, best_obj_4, best_snps_4 = fss_4.perform_selection(k_values, delta_values, output_prefix=output_prefix, select_by_ll=True, strategy=strategy,create_pdf=False)
+        fss_4 = FeatureSelectionStrategy(
+            snpreader,
+            self.pheno_shuffleplus_fn,
+            num_folds,
+            cov_fn=cov_fn,
+            random_state=random_state,
+            num_pcs=num_pcs,
+            interpolate_delta=True,
+            num_snps_in_memory=20000,
+            count_A1=False,
+        )
+        best_k_4, best_delta_4, best_obj_4, best_snps_4 = fss_4.perform_selection(
+            k_values,
+            delta_values,
+            output_prefix=output_prefix,
+            select_by_ll=True,
+            strategy=strategy,
+            create_pdf=False,
+        )
 
         # case 5
-        fss_5 = FeatureSelectionStrategy(snpreader, self.pheno_shuffleplus_fn, num_folds, cov_fn=cov_fn, random_state=random_state, num_pcs=num_pcs, interpolate_delta=True, num_snps_in_memory=5000,count_A1=False)
-        best_k_5, best_delta_5, best_obj_5, best_snps_5 = fss_5.perform_selection(k_values, delta_values, output_prefix=output_prefix, select_by_ll=True, strategy=strategy,create_pdf=False)
+        fss_5 = FeatureSelectionStrategy(
+            snpreader,
+            self.pheno_shuffleplus_fn,
+            num_folds,
+            cov_fn=cov_fn,
+            random_state=random_state,
+            num_pcs=num_pcs,
+            interpolate_delta=True,
+            num_snps_in_memory=5000,
+            count_A1=False,
+        )
+        best_k_5, best_delta_5, best_obj_5, best_snps_5 = fss_5.perform_selection(
+            k_values,
+            delta_values,
+            output_prefix=output_prefix,
+            select_by_ll=True,
+            strategy=strategy,
+            create_pdf=False,
+        )
 
         # case 6
-        fss_6 = FeatureSelectionStrategy(snpreader, self.pheno_shuffleplus_fn, num_folds, cov_fn=cov_fn, random_state=random_state, num_pcs=num_pcs, interpolate_delta=True, num_snps_in_memory=600,count_A1=False)
-        best_k_6, best_delta_6, best_obj_6, best_snps_6 = fss_6.perform_selection(k_values, delta_values, output_prefix=output_prefix, select_by_ll=True, strategy=strategy,create_pdf=False)
+        fss_6 = FeatureSelectionStrategy(
+            snpreader,
+            self.pheno_shuffleplus_fn,
+            num_folds,
+            cov_fn=cov_fn,
+            random_state=random_state,
+            num_pcs=num_pcs,
+            interpolate_delta=True,
+            num_snps_in_memory=600,
+            count_A1=False,
+        )
+        best_k_6, best_delta_6, best_obj_6, best_snps_6 = fss_6.perform_selection(
+            k_values,
+            delta_values,
+            output_prefix=output_prefix,
+            select_by_ll=True,
+            strategy=strategy,
+            create_pdf=False,
+        )
 
         self.assertEqual(int(best_k_1), int(best_k_2))
         self.assertEqual(int(best_k_1), int(best_k_3))
-        #self.assertEqual(int(best_k_1), int(best_k_4))
-        #self.assertEqual(int(best_k_1), int(best_k_5))
-        #self.assertEqual(int(best_k_1), int(best_k_6))
+        # self.assertEqual(int(best_k_1), int(best_k_4))
+        # self.assertEqual(int(best_k_1), int(best_k_5))
+        # self.assertEqual(int(best_k_1), int(best_k_6))
         self.assertAlmostEqual(best_obj_1, best_obj_2)
         self.assertAlmostEqual(best_obj_1, best_obj_3)
-        #self.assertAlmostEqual(best_obj_1, best_obj_4)
+        # self.assertAlmostEqual(best_obj_1, best_obj_4)
         self.assertAlmostEqual(best_obj_4, best_obj_5)
         self.assertAlmostEqual(best_obj_4, best_obj_6)
 
         if strategy != "insample_cv":
             self.assertAlmostEqual(best_delta_1, best_delta_2)
             self.assertAlmostEqual(best_delta_1, best_delta_3)
-            #self.assertAlmostEqual(best_delta_1, best_delta_4)
+            # self.assertAlmostEqual(best_delta_1, best_delta_4)
             self.assertAlmostEqual(best_delta_4, best_delta_5)
             self.assertAlmostEqual(best_delta_4, best_delta_6)
-       
 
     def test_log_likelihood_bed(self):
         self.log_likelihood(self.snpreader_bed)
-        
+
     def test_log_likelihood_hdf5(self):
         self.log_likelihood(self.snpreader_hdf5)
 
     def test_log_likelihood_dat(self):
         self.log_likelihood(self.snpreader_dat)
 
     def test_log_likelihood_ped(self):
@@ -399,59 +613,151 @@
         """
         test mean, variance against C++ results (autoselect):
 
         FastLmmC.exe -autoselect test -bfilesim toydata -pheno toydata.phe -logDelta X -autoSelectSearchValues k -verboseOutput > debug.txt
         """
 
         # low-rank, small delta
-        ll_1_expected = np.array([79.7217, 80.5289, 79.9218, 53.7485, 71.4134, 71.5751, 58.4209, 69.82, 85.5727, 72.7218])
+        ll_1_expected = np.array(
+            [
+                79.7217,
+                80.5289,
+                79.9218,
+                53.7485,
+                71.4134,
+                71.5751,
+                58.4209,
+                69.82,
+                85.5727,
+                72.7218,
+            ]
+        )
         ll_1 = core_run(snpreader, self.pheno_fn, 50, np.exp(-5))
 
         for i in range(len(ll_1)):
-            np.testing.assert_approx_equal(ll_1[i], ll_1_expected[i], significant=3, err_msg='Log-likelihoods differ', verbose=True)
-
+            np.testing.assert_approx_equal(
+                ll_1[i],
+                ll_1_expected[i],
+                significant=3,
+                err_msg="Log-likelihoods differ",
+                verbose=True,
+            )
 
         # low-rank, large delta
-        ll_2_expected = np.array([68.7098, 70.0446, 75.1816, 62.3675, 69.34, 74.6755, 59.9937, 66.6408, 74.1564, 68.3146])
+        ll_2_expected = np.array(
+            [
+                68.7098,
+                70.0446,
+                75.1816,
+                62.3675,
+                69.34,
+                74.6755,
+                59.9937,
+                66.6408,
+                74.1564,
+                68.3146,
+            ]
+        )
         ll_2 = core_run(snpreader, self.pheno_fn, 50, np.exp(10))
 
         for i in range(len(ll_2)):
-            np.testing.assert_approx_equal(ll_2[i], ll_2_expected[i], significant=3, err_msg='Log-likelihoods differ', verbose=True)
-
+            np.testing.assert_approx_equal(
+                ll_2[i],
+                ll_2_expected[i],
+                significant=3,
+                err_msg="Log-likelihoods differ",
+                verbose=True,
+            )
 
         # full-rank, small delta
         # these values appear to indicate numerical instability. the python version will continue to match these
         # results for the time being, but provide a flag "robust" to lead to a numerically more stable solution
-        ll_3_expected = np.array([1636.33, 28711.8, 32008.8, 1363.74, 128444, 22277.6, 16389.2, 95458.7, 4710.33, 68308.9])
+        ll_3_expected = np.array(
+            [
+                1636.33,
+                28711.8,
+                32008.8,
+                1363.74,
+                128444,
+                22277.6,
+                16389.2,
+                95458.7,
+                4710.33,
+                68308.9,
+            ]
+        )
         ll_3 = core_run(snpreader, self.pheno_fn, 5000, np.exp(-5))
 
         for i in range(len(ll_3)):
-            np.testing.assert_approx_equal(ll_3[i], ll_3_expected[i], significant=2, err_msg='Log-likelihoods differ', verbose=True)
+            np.testing.assert_approx_equal(
+                ll_3[i],
+                ll_3_expected[i],
+                significant=2,
+                err_msg="Log-likelihoods differ",
+                verbose=True,
+            )
 
-        
         # full-rank, small delta
-        ll_4_expected = np.array([68.4794, 70.7483, 76.6886, 62.2721, 69.0659, 76.8207, 59.5216, 66.1517, 75.9149, 68.6061])
+        ll_4_expected = np.array(
+            [
+                68.4794,
+                70.7483,
+                76.6886,
+                62.2721,
+                69.0659,
+                76.8207,
+                59.5216,
+                66.1517,
+                75.9149,
+                68.6061,
+            ]
+        )
         ll_4 = core_run(snpreader, self.pheno_fn, 5000, np.exp(10))
 
         for i in range(len(ll_4)):
-            np.testing.assert_approx_equal(ll_4[i], ll_4_expected[i], significant=3, err_msg='Log-likelihoods differ', verbose=True)
-
+            np.testing.assert_approx_equal(
+                ll_4[i],
+                ll_4_expected[i],
+                significant=3,
+                err_msg="Log-likelihoods differ",
+                verbose=True,
+            )
 
         # square matrix, delta 2
-        ll_5_expected = np.array([259.91, 351.914, 389.971, 313.807, 334.883, 345.312, 221.556, 206.15, 270.53, 304.231])
+        ll_5_expected = np.array(
+            [
+                259.91,
+                351.914,
+                389.971,
+                313.807,
+                334.883,
+                345.312,
+                221.556,
+                206.15,
+                270.53,
+                304.231,
+            ]
+        )
         ll_5 = core_run(snpreader, self.pheno_fn, 500, np.exp(2))
 
         for i in range(len(ll_5)):
-            np.testing.assert_approx_equal(ll_5[i], ll_5_expected[i], significant=3, err_msg='Log-likelihoods differ', verbose=True)
+            np.testing.assert_approx_equal(
+                ll_5[i],
+                ll_5_expected[i],
+                significant=3,
+                err_msg="Log-likelihoods differ",
+                verbose=True,
+            )
+
 
 def core_run(snpreader, pheno_fn, k, delta):
     """
     extracted core functionality, to avoid shuffle of data and not correct delta
     """
-    with patch.dict('os.environ', {'ARRAY_MODULE': 'numpy'}) as _:
+    with patch.dict("os.environ", {"ARRAY_MODULE": "numpy"}) as _:
 
         G, X, y = load_snp_data(snpreader, pheno_fn, standardizer=Unit())
         kf = KFold(n_splits=10, shuffle=False).split(list(range(len(y))))
 
         ll = np.zeros(10)
 
         fold_idx = 0
@@ -460,58 +766,64 @@
             fold_idx += 1
 
             fold_data["train_idx"] = train_idx
             fold_data["test_idx"] = test_idx
 
             # set up data
             ##############################
-            fold_data["G_train"] = G[train_idx,:].read()
-            fold_data["G_test"] = G[test_idx,:]
+            fold_data["G_train"] = G[train_idx, :].read()
+            fold_data["G_test"] = G[test_idx, :]
 
             fold_data["X_train"] = X[train_idx]
             fold_data["X_test"] = X[test_idx]
 
             fold_data["y_train"] = y[train_idx]
             fold_data["y_test"] = y[test_idx]
 
-
             # feature selection
             ##############################
-            _F,_pval = lin_reg.f_regression_block(lin_reg.f_regression_cov_alt,fold_data["G_train"].val,fold_data["y_train"],blocksize=1E4,C=fold_data["X_train"])
+            _F, _pval = lin_reg.f_regression_block(
+                lin_reg.f_regression_cov_alt,
+                fold_data["G_train"].val,
+                fold_data["y_train"],
+                blocksize=1e4,
+                C=fold_data["X_train"],
+            )
             feat_idx = np.argsort(_pval)
             fold_data["feat_idx"] = feat_idx
-        
+
             # re-order SNPs (and cut to max num)
             ##############################
-            fold_data["G_train"] = fold_data["G_train"][:,feat_idx[0:k]].read()
-            fold_data["G_test"] = fold_data["G_test"][:,feat_idx[0:k]].read()
+            fold_data["G_train"] = fold_data["G_train"][:, feat_idx[0:k]].read()
+            fold_data["G_test"] = fold_data["G_test"][:, feat_idx[0:k]].read()
 
             model = getLMM()
             model.setG(fold_data["G_train"].val)
             model.sety(fold_data["y_train"])
             model.setX(fold_data["X_train"])
 
             REML = False
-        
+
             # predict on test set
             res = model.nLLeval(delta=delta, REML=REML)
             model.setTestData(Xstar=fold_data["X_test"], G0star=fold_data["G_test"].val)
             model.predictMean(beta=res["beta"], delta=delta)
-            #mse_cv1[k_idx, delta_idx] = mean_squared_error(fold_data["y_test"],
-            #out)
-            ll[split_idx] = model.nLLeval_test(fold_data["y_test"], res["beta"], sigma2=res["sigma2"], delta=delta)
-
+            # mse_cv1[k_idx, delta_idx] = mean_squared_error(fold_data["y_test"],
+            # out)
+            ll[split_idx] = model.nLLeval_test(
+                fold_data["y_test"], res["beta"], sigma2=res["sigma2"], delta=delta
+            )
 
         return ll
 
 
 def getTestSuite():
     """
     set up composite test suite
     """
     suite1 = unittest.TestLoader().loadTestsFromTestCase(TestTwoKernelFeatureSelection)
     suite2 = unittest.TestLoader().loadTestsFromTestCase(TestFeatureSelection)
-    return unittest.TestSuite([suite1,suite2])
+    return unittest.TestSuite([suite1, suite2])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/__init__.py` & `fastlmm-0.6.8b1/fastlmm/inference/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import absolute_import
 from fastlmm.inference.fastlmm_predictor import FastLMM
 from fastlmm.inference.linear_regression import LinearRegression
 
 
 # from bin2kernel import Bin2Kernel
 # from bin2kernel import makeBin2KernelAsEstimator
 # from bin2kernel import Bin2KernelLaplaceLinearN
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/ep.py` & `fastlmm-0.6.8b1/fastlmm/inference/ep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from __future__ import absolute_import
 import numpy as NP
-import scipy as SP
 from numpy import dot
 import scipy.stats as ST
 from scipy.linalg import cholesky, solve_triangular
 from fastlmm.external.util.math import (
     check_definite_positiveness,
     check_symmetry,
     mvnormpdf,
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/fastlmm_predictor.py` & `fastlmm-0.6.8b1/fastlmm/inference/fastlmm_predictor.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/inference/glmm.py` & `fastlmm-0.6.8b1/fastlmm/inference/glmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from __future__ import absolute_import
-import scipy as SP
+import scipy.optimize as opt
 import scipy.stats as ST
 import numpy as NP
 from numpy import dot
 from scipy.linalg import cholesky, solve_triangular
 from fastlmm.external.util.math import (
     check_definite_positiveness,
     check_symmetry,
@@ -11,15 +10,15 @@
     dotd,
     trace2,
 )
 from fastlmm.external.util.math import stl, stu
 from sklearn.base import BaseEstimator
 from fastlmm import Pr
 import sys
-from six.moves import range
+
 
 """
     Important! Always run test.py in the current folder for unit testing after
     changes have been made.
 """
 
 
@@ -420,18 +419,16 @@
         if optSig12:
             bounds.append((lowerBound, maxsig2))
         if optSign2:
             bounds.append((lowerBound, maxsig2))
         if optBeta:
             bounds += [(-maxbeta, maxbeta)] * self._D
 
-        (xfinal, aa, bb) = SP.optimize.fmin_tnc(
-            func, x, fprime=grad, bounds=bounds, disp=0
-        )
-        #        (xfinal,cost,msgs) = SP.optimize.fmin_l_bfgs_b(func, x, fprime=grad, bounds=bounds,
+        (xfinal, aa, bb) = opt.fmin_tnc(func, x, fprime=grad, bounds=bounds, disp=0)
+        #        (xfinal,cost,msgs) = opt.fmin_l_bfgs_b(func, x, fprime=grad, bounds=bounds,
         #                                                        disp=self._verbose)
         #                                                        disp=False)
         self._unwrap_hyp(xfinal, optSig02, optSig12, optSign2, optBeta)
         marg = self.marginal_loglikelihood()
         #        marg = -cost
 
         # if self._verbose:
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/laplace.py` & `fastlmm-0.6.8b1/fastlmm/inference/laplace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from __future__ import absolute_import
 from fastlmm import Pr
-import scipy as sp
-import numpy as NP
+import scipy.optimize as opt
+import numpy as np
 from numpy import dot
 import scipy.integrate
 from scipy.linalg import cholesky, solve_triangular
 from fastlmm.external.util.math import (
     check_definite_positiveness,
     check_symmetry,
     mvnormpdf,
@@ -56,15 +55,15 @@
         da = a - aprev
 
         def fobj(alpha):
             a = aprev + alpha * da
             f = self._rdotK(a) + m
             return -(self._likelihood.log(f, self._y) - (f - m).dot(a) / 2.0)
 
-        (alpha, obj, iter, funcalls) = sp.optimize.fminbound(
+        (alpha, obj, iter, funcalls) = opt.fminbound(
             fobj, 0.0, 1.0, full_output=True, xtol=1e-4, maxfun=25
         )
         obj = -obj
         a = aprev + alpha * da
         f = self._rdotK(a) + m
         return (f, a, obj)
 
@@ -79,28 +78,28 @@
         iters = [
             self._debugUACalls[i].innerIters for i in range(len(self._debugUACalls))
         ]
         sig02 = [self._debugUACalls[i].sig02 for i in range(len(self._debugUACalls))]
         sig12 = [self._debugUACalls[i].sig12 for i in range(len(self._debugUACalls))]
         sign2 = [self._debugUACalls[i].sign2 for i in range(len(self._debugUACalls))]
         gradMeans = [
-            NP.mean(abs(self._debugUACalls[i].lastGrad))
+            np.mean(abs(self._debugUACalls[i].lastGrad))
             for i in range(len(self._debugUACalls))
         ]
 
         Pr.prin("*** Update approximation ***")
         Pr.prin("calls: %d" % (len(self._debugUACalls),))
 
         table = [
             ["", "min", "max", "mean"],
-            ["iters", min(iters), max(iters), NP.mean(iters)],
-            ["|grad|_{mean}", min(gradMeans), max(gradMeans), NP.mean(gradMeans)],
-            ["sig01", min(sig02), max(sig02), NP.mean(sig02)],
-            ["sig11", min(sig12), max(sig12), NP.mean(sig12)],
-            ["sign1", min(sign2), max(sign2), NP.mean(sign2)],
+            ["iters", min(iters), max(iters), np.mean(iters)],
+            ["|grad|_{mean}", min(gradMeans), max(gradMeans), np.mean(gradMeans)],
+            ["sig01", min(sig02), max(sig02), np.mean(sig02)],
+            ["sig11", min(sig12), max(sig12), np.mean(sig12)],
+            ["sign1", min(sign2), max(sign2), np.mean(sign2)],
         ]
         Pr.prin(tabulate(table))
 
     def _updateApproximation(self):
         """
         Calculates the Laplace approximation for the posterior.
         It can be defined by two variables: f mode and W at f mode.
@@ -118,28 +117,28 @@
         objEpsStop = 1e-8
         gradEpsErr = 1e-3
 
         self._mean = self._calculateMean()
         m = self._mean
 
         if self._lasta is None or self._lasta.shape[0] != self._N:
-            aprev = NP.zeros(self._N)
+            aprev = np.zeros(self._N)
         else:
             aprev = self._lasta
 
         fprev = self._rdotK(aprev) + m
         objprev = self._likelihood.log(fprev, self._y) - (fprev - m).dot(aprev) / 2.0
         ii = 0
         line_search = False
         maxIter = 1000
         failed = False
         failedMsg = ""
         while ii < maxIter:
             grad = self._calculateUAGrad(fprev, aprev)
-            if NP.mean(abs(grad)) < gradEpsStop:
+            if np.mean(abs(grad)) < gradEpsStop:
                 a = aprev
                 f = fprev
                 break
 
             # The following is just a Newton step (eq. (3.18) [1]) to maximize
             # log(p(F|X,y)) over F
             g = self._likelihood.gradient_log(fprev, self._y)
@@ -168,15 +167,15 @@
                     f = fprev
                     break
                 line_search = True
             ii += 1
 
         self._lasta = a
 
-        err = NP.mean(abs(grad))
+        err = np.mean(abs(grad))
         if err > gradEpsErr:
             failed = True
             failedMsg = "Gradient not too small in the Laplace update approximation.\n"
             failedMsg = (
                 failedMsg
                 + "Problem in the f mode estimation. |grad|_{mean} = %.6f." % (err,)
             )
@@ -211,19 +210,19 @@
 
         self._updateApproximationCount = 0
 
     def _predict(self, meanstar, kstar, kstarstar, prob):
         self._updateConstants()
         self._updateApproximation()
 
-        if NP.isscalar(kstarstar):
+        if np.isscalar(kstarstar):
             return self._predict_each(meanstar, kstar, kstarstar, prob)
 
         n = len(kstarstar)
-        ps = NP.zeros(n)
+        ps = np.zeros(n)
 
         for i in range(n):
             ps[i] = self._predict_each(meanstar[i], kstar[i, :], kstarstar[i], prob)
 
         return ps
 
 
@@ -258,15 +257,15 @@
         return a
 
     def _updateApproximationEnd(self, f, a):
         self._f = f
         self._a = a
 
         self._W = self._calculateW(f)
-        self._Wsq = NP.sqrt(self._W)
+        self._Wsq = np.sqrt(self._W)
 
         self._A = 1.0 + self._W * self._sign2
         self._V = self._W / self._A
         self._Lk = self._calculateLk(self._G01, self._V)
 
     def _updateApproximation(self):
         LaplaceGLMM._updateApproximation(self)
@@ -281,18 +280,18 @@
         (f, a) = (self._f, self._a)
 
         loglike = self._likelihood.log(f, self._y)
 
         r = (
             loglike
             - dot(f - self._mean, a) / 2.0
-            - sum(NP.log(NP.diag(self._Lk)))
-            - sum(NP.log(self._A)) / 2.0
+            - sum(np.log(np.diag(self._Lk)))
+            - sum(np.log(self._A)) / 2.0
         )
-        assert NP.isfinite(r), "Not finite regular marginal loglikelihood."
+        assert np.isfinite(r), "Not finite regular marginal loglikelihood."
 
         return r
 
     def _rmll_gradient(self, optSig02=True, optSig12=True, optSign2=True, optBeta=True):
         self._updateConstants()
         self._updateApproximation()
 
@@ -336,15 +335,15 @@
             LkG01VG0 = dot(H, G0)
             VG0 = ddot(V, G0, left=True)
 
             ret0 = (
                 dot(a, dF0)
                 - 0.5 * dot(a, dK0a)
                 + dot(f - m, t)
-                + 0.5 * NP.sum(diags * dF0)
+                + 0.5 * np.sum(diags * dF0)
                 + -0.5 * trace2(VG0, G0.T)
                 + 0.5 * trace2(LkG01VG0.T, LkG01VG0)
             )
 
             ret.append(ret0)
 
         if optSig12:
@@ -355,49 +354,49 @@
             LkG01VG1 = dot(H, G1)
             VG1 = ddot(V, G1, left=True)
 
             ret1 = (
                 dot(a, dF1)
                 - 0.5 * dot(a, dK1a)
                 + dot(f - m, t)
-                + 0.5 * NP.sum(diags * dF1)
+                + 0.5 * np.sum(diags * dF1)
                 + -0.5 * trace2(VG1, G1.T)
                 + 0.5 * trace2(LkG01VG1.T, LkG01VG1)
             )
 
             ret.append(ret1)
 
         if optSign2:
             t = V * a - dot(H.T, dot(H, a))
             dFn = a - self._rdotK(t)
 
             retn = (
                 dot(a, dFn)
                 - 0.5 * dot(a, a)
                 + dot(f - m, t)
-                + 0.5 * NP.sum(diags * dFn)
-                + -0.5 * NP.sum(V)
+                + 0.5 * np.sum(diags * dFn)
+                + -0.5 * np.sum(V)
                 + 0.5 * trace2(H.T, H)
             )
 
             ret.append(retn)
 
         if optBeta:
             t = ddot(V, X, left=True) - dot(H.T, dot(H, X))
             dFbeta = X - self._rdotK(t)
 
             retbeta = dot(a, dFbeta) + dot(f - m, t)
             for i in range(dFbeta.shape[1]):
-                retbeta[i] += 0.5 * NP.sum(diags * dFbeta[:, i])
+                retbeta[i] += 0.5 * np.sum(diags * dFbeta[:, i])
 
             ret.extend(retbeta)
 
-        ret = NP.array(ret)
-        assert NP.all(
-            NP.isfinite(ret)
+        ret = np.array(ret)
+        assert np.all(
+            np.isfinite(ret)
         ), "Not finite regular marginal loglikelihood gradient."
 
         return ret
 
     def _predict(self, meanstar, kstar, kstarstar, prob):
         return LaplaceGLMM._predict(self, meanstar, kstar, kstarstar, prob)
 
@@ -436,36 +435,36 @@
         GLMM_N3K1.__init__(
             self, penalty=penalty, penalizeBias=penalizeBias, debug=debug
         )
         LaplaceGLMM.__init__(self, link)
         self._link = link
 
     def _updateApproximationBegin(self):
-        self._K = NP.eye(self._N) * self._sign2
+        self._K = np.eye(self._N) * self._sign2
         if self._isK0Set:
             self._K += self._sig02 * (
                 self._K0 if self._K0 is not None else dot(self._G0, self._G0.T)
             )
         if self._isK1Set:
             self._K += self._sig12 * (
                 self._K1 if self._K1 is not None else dot(self._G1, self._G1.T)
             )
 
     def _calculateUAa(self, b, W):
-        Wsq = NP.sqrt(W)
+        Wsq = np.sqrt(W)
         Ln = self._calculateLn(self._K, Wsq)
         a = b - Wsq * stu(Ln.T, stl(Ln, Wsq * dot(self._K, b)))
         return a
 
     def _updateApproximationEnd(self, f, a):
         self._f = f
         self._a = a
 
         self._W = self._calculateW(f)
-        self._Wsq = NP.sqrt(self._W)
+        self._Wsq = np.sqrt(self._W)
 
         self._A = 1.0 + self._W * self._sign2
         V = self._W / self._A
         self._Ln = self._calculateLn(self._K, self._Wsq)
 
     def _regular_marginal_loglikelihood(self):
         self._updateConstants()
@@ -474,16 +473,16 @@
         if self._is_kernel_zero():
             return self._likelihood.log(self._mean, self._y)
 
         (f, a) = (self._f, self._a)
 
         loglike = self._likelihood.log(f, self._y)
 
-        r = loglike - dot(f - self._mean, a) / 2.0 - sum(NP.log(NP.diag(self._Ln)))
-        assert NP.isfinite(r), "Not finite regular marginal loglikelihood."
+        r = loglike - dot(f - self._mean, a) / 2.0 - sum(np.log(np.diag(self._Ln)))
+        assert np.isfinite(r), "Not finite regular marginal loglikelihood."
 
         return r
 
     def _rmll_gradient(self, optSig02=True, optSig12=True, optSign2=True, optBeta=True):
         self._updateConstants()
         self._updateApproximation()
 
@@ -494,15 +493,15 @@
         K0 = self._K0
         K1 = self._K1
         m = self._mean
         a = self._a
         Ln = self._Ln
         X = self._X
 
-        LnWsq = stl(Ln, NP.diag(Wsq))
+        LnWsq = stl(Ln, np.diag(Wsq))
         LnWsqK = dot(LnWsq, K)
 
         d = self._dKn()
         h = self._likelihood.third_derivative_log(f)
         diags = (d - dotd(LnWsqK.T, LnWsqK)) * h
 
         ret = []
@@ -511,58 +510,58 @@
             dK0a = dot(K0, a)
             dF0 = dK0a - dot(LnWsqK.T, dot(LnWsq, dK0a))
 
             r = (
                 dot(a, dF0)
                 - dot(a, dF0)
                 + 0.5 * dot(a, dK0a)
-                + 0.5 * NP.sum(diags * dF0)
+                + 0.5 * np.sum(diags * dF0)
                 - 0.5 * trace2(LnWsq.T, dot(LnWsq, K0))
             )
 
             ret.append(r)
 
         if optSig12:
             dK1a = dot(K1, a)
             dF1 = dK1a - dot(LnWsqK.T, dot(LnWsq, dK1a))
 
             r = (
                 dot(a, dF1)
                 - dot(a, dF1)
                 + 0.5 * dot(a, dK1a)
-                + 0.5 * NP.sum(diags * dF1)
+                + 0.5 * np.sum(diags * dF1)
                 - 0.5 * trace2(LnWsq.T, dot(LnWsq, K1))
             )
 
             ret.append(r)
 
         if optSign2:
             dFn = a - dot(LnWsqK.T, dot(LnWsq, a))
 
             r = (
                 dot(a, dFn)
                 - dot(a, dFn)
                 + 0.5 * dot(a, a)
-                + 0.5 * NP.sum(diags * dFn)
+                + 0.5 * np.sum(diags * dFn)
                 - 0.5 * trace2(LnWsq.T, LnWsq)
             )
 
             ret.append(r)
 
         if optBeta:
             dFmb = -dot(LnWsqK.T, dot(LnWsq, X))
             dFb = dFmb + X
 
-            r = dot(a, dFb) - dot(a, dFmb) + 0.5 * NP.sum(diags * dFb.T, 1)
+            r = dot(a, dFb) - dot(a, dFmb) + 0.5 * np.sum(diags * dFb.T, 1)
 
             ret += list(r)
 
-        ret = NP.array(ret)
-        assert NP.all(
-            NP.isfinite(ret)
+        ret = np.array(ret)
+        assert np.all(
+            np.isfinite(ret)
         ), "Not finite regular marginal loglikelihood gradient."
 
         return ret
 
     def _updateApproximation(self):
         LaplaceGLMM._updateApproximation(self)
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/likelihood.py` & `fastlmm-0.6.8b1/fastlmm/inference/likelihood.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,110 @@
-from __future__ import absolute_import
 import scipy.stats as ST
 import numpy as NP
 
 logit_sigmoid = lambda x: 1.0 / (1.0 + NP.exp(-x))
 probit_sigmoid = lambda x: ST.norm.cdf(x)
 
+
 class Likelihood:
     def __init__(self):
         pass
 
     # likelihood
     def plain(self, f, y):
         raise NotImplementedError
-    
+
     # log likelihood
     def log(self, f, y):
         raise NotImplementedError
-    
+
     # gradient of the log likelihood
     def gradient_log(self, f, y):
         raise NotImplementedError
-    
+
     # hessian of the log likelihood
     def hessian_log(self, f):
         raise NotImplementedError
 
     def third_derivative_log(self, f):
         raise NotImplementedError
 
+
 class ProbitLikelihood(Likelihood):
     def __init__(self):
         Likelihood.__init__(self)
 
     # likelihood
     def plain(self, f, y):
-        return ST.norm._cdf(y*f).prod()
+        return ST.norm._cdf(y * f).prod()
 
     # log likelihood
     def log(self, f, y):
-        return ST.norm._logcdf(y*f).sum()
+        return ST.norm._logcdf(y * f).sum()
+
 
 # Implements p(y|F) = prod_{i=1}^n p(y_i|f_i)
 #                   = prod_{i=1}^n logistic(y_i*f_i).
 class LogitLikelihood(Likelihood):
     def __init__(self):
         Likelihood.__init__(self)
-        #self.sigmoid = lambda x: 1.0 / (1.0 + NP.exp(-x))
-        self.sigmoid = logit_sigmoid 
+        # self.sigmoid = lambda x: 1.0 / (1.0 + NP.exp(-x))
+        self.sigmoid = logit_sigmoid
 
     # likelihood
     def plain(self, f, y):
-        return self.sigmoid(y*f).prod()
-    
+        return self.sigmoid(y * f).prod()
+
     # log likelihood
-    def log(self, f, y): 
-        yf = y*f 
-        r = self.sigmoid(yf) 
-        ok = r>0.0 
-        r[ok] = NP.log( r[ok] ) 
+    def log(self, f, y):
+        yf = y * f
+        r = self.sigmoid(yf)
+        ok = r > 0.0
+        r[ok] = NP.log(r[ok])
         r[~ok] = yf[~ok]
         return r.sum()
-    
+
     # gradient of the log likelihood
     def gradient_log(self, f, y):
-        return y*self.sigmoid(-y*f)
-    
+        return y * self.sigmoid(-y * f)
+
     # hessian of the log likelihood
     def hessian_log(self, f):
-        r = self.sigmoid(f)*self.sigmoid(-f)
+        r = self.sigmoid(f) * self.sigmoid(-f)
         ok = r >= 1e-16
         r[~ok] = 1e-16
         return -r
         # maybe faster, but maybe less precise version
         # pi = self.sigmoid(f)
         # return -pi*(1.0-pi)
 
     def third_derivative_log(self, f):
         pi = self.sigmoid(f)
-        return -pi*self.sigmoid(-f)*(1.0-2.0*pi)
+        return -pi * self.sigmoid(-f) * (1.0 - 2.0 * pi)
         # maybe faster, but maybe less precise version
         # return -pi*(1.0-pi)*(1.0-2.0*pi)
 
     def intOverGauss(self, mu, sig2):
         # horta201306 we approximate \int logistic(x) N(x, mu, sig2) dx
         # by observing that logistic(x) is cdf of the standard logistic distribution
         # and that this distribution is similar in shape with the normal one
         # so we approximate the logistic pdf by a mixture of five normal
         # distributions, and then calculate the integral
         # we adopted the coefficients c and lambd from Rasmussen and Williams' GP toolbox
         # for Matlab.
 
-        c = NP.array([1.146480988574439e+02,-1.508871030070582e+03,2.676085036831241e+03,-1.356294962039222e+03,7.543285642111850e+01])
-        lambd = NP.array([0.44,0.41,0.40,0.39,0.36])
+        c = NP.array(
+            [
+                1.146480988574439e02,
+                -1.508871030070582e03,
+                2.676085036831241e03,
+                -1.356294962039222e03,
+                7.543285642111850e01,
+            ]
+        )
+        lambd = NP.array([0.44, 0.41, 0.40, 0.39, 0.36])
 
-        sigs = 1.0/(lambd*NP.sqrt(2))
+        sigs = 1.0 / (lambd * NP.sqrt(2))
 
-        z = mu / (  sigs * NP.sqrt(1.0 + sig2/sigs**2)  )
+        z = mu / (sigs * NP.sqrt(1.0 + sig2 / sigs**2))
 
-        return NP.sum(c*ST.norm.cdf(z))
+        return NP.sum(c * ST.norm.cdf(z))
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/linear_regression.py` & `fastlmm-0.6.8b1/fastlmm/inference/linear_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import numpy as np
 import logging
 import unittest
 import os
 import scipy.linalg as LA
 import time
 from sklearn.utils import safe_sqr, check_array
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/lmm.py` & `fastlmm-0.6.8b1/fastlmm/inference/lmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import scipy as SP
-import numpy as NP
 import numpy as np
 import scipy.linalg as LA
 import scipy.optimize as opt
 import scipy.stats as ST
 import scipy.special as SS
 from fastlmm.util.mingrid import *
 from fastlmm.util.util import *
@@ -214,16 +212,16 @@
                     K1 = self.G1.dot(self.G1.T)
                 self.setK(K0=K0, K1=K1, a2=a2)
                 # K=self.G.dot(self.G.T)
                 # self.setK(K)
             self.a2 = a2
             pass
         else:  # rank of kernel = 0 (linear regression case)
-            self.S = SP.zeros((0))
-            self.U = SP.zeros_like(self.G)
+            self.S = np.zeros((0))
+            self.U = np.zeros_like(self.G)
 
     def setK(self, K0, K1=None, a2=0.0):
         """
         set the Kernel (1-a2)*K0 and a2*K1.
         This has to be done before setting the data setX() and setY().
         --------------------------------------------------------------------------
         Input:
@@ -462,15 +460,15 @@
             delta = np.exp(logdelta)
 
         if delta is not None:
             Sd = (self.S + delta) * scale
         else:
             Sd = (h2 * self.S + (1.0 - h2)) * scale
 
-        UXS = self.UX / NP.lib.stride_tricks.as_strided(
+        UXS = self.UX / np.lib.stride_tricks.as_strided(
             Sd, (Sd.size, self.UX.shape[1]), (Sd.itemsize, 0)
         )
         UyS = self.Uy / Sd
 
         XKX = UXS.T.dot(self.UX)
         XKy = UXS.T.dot(self.Uy)
         yKy = UyS.T.dot(self.Uy)
@@ -496,20 +494,20 @@
         if len(self.exclude_idx) > 0:
             num_exclude = len(self.exclude_idx)
 
             # consider only excluded SNPs
             G_exclude = self.G[:, self.exclude_idx]
 
             self.UW = self.U.T.dot(G_exclude)  # needed for proximal contamination
-            UWS = self.UW / NP.lib.stride_tricks.as_strided(
+            UWS = self.UW / np.lib.stride_tricks.as_strided(
                 Sd, (Sd.size, num_exclude), (Sd.itemsize, 0)
             )
             assert UWS.shape == (k, num_exclude)
 
-            WW = NP.eye(num_exclude) - UWS.T.dot(self.UW)
+            WW = np.eye(num_exclude) - UWS.T.dot(self.UW)
             WX = UWS.T.dot(self.UX)
             Wy = UWS.T.dot(self.Uy)
             assert WW.shape == (num_exclude, num_exclude)
             assert WX.shape == (num_exclude, D)
             assert Wy.shape == (num_exclude,)
 
             if k < N:  # low rank part
@@ -525,15 +523,15 @@
 
             UWX = U_WW.T.dot(WX)
             UWy = U_WW.T.dot(Wy)
             assert UWX.shape == (num_exclude, D)
             assert UWy.shape == (num_exclude,)
 
             # compute S_WW^{-1} * UWX
-            WX = UWX / NP.lib.stride_tricks.as_strided(
+            WX = UWX / np.lib.stride_tricks.as_strided(
                 S_WW, (S_WW.size, UWX.shape[1]), (S_WW.itemsize, 0)
             )
             # compute S_WW^{-1} * UWy
             Wy = UWy / S_WW
             # determinant update
             logdetK += np.log(S_WW).sum()
             assert WX.shape == (num_exclude, D)
@@ -562,20 +560,20 @@
                 logdetXX = np.log(Sxx).sum()
                 logdetXKX = np.log(SxKx).sum()
                 sigma2 = r2 / (N - D)
                 nLL = 0.5 * (
                     logdetK
                     + logdetXKX
                     - logdetXX
-                    + (N - D) * (np.log(2.0 * SP.pi * sigma2) + 1)
+                    + (N - D) * (np.log(2.0 * np.pi * sigma2) + 1)
                 )
                 variance_beta = None
             else:
                 sigma2 = r2 / (N)
-                nLL = 0.5 * (logdetK + N * (np.log(2.0 * SP.pi * sigma2) + 1))
+                nLL = 0.5 * (logdetK + N * (np.log(2.0 * np.pi * sigma2) + 1))
                 if delta is not None:
                     h2 = 1.0 / (delta + 1)
                 # This is a faster version of h2 * sigma2 * np.diag(LA.inv(XKX))
                 # where h2*sigma2 is sigma2_g
                 variance_beta = (
                     h2
                     * sigma2
@@ -601,22 +599,22 @@
                 nLL = 0.5 * (
                     logdetK
                     + logdetXKX
                     - logdetXX
                     + (dof + (N - D)) * np.log(1.0 + r2 / dof)
                 )
                 nLL += (
-                    0.5 * (N - D) * np.log(dof * SP.pi)
+                    0.5 * (N - D) * np.log(dof * np.pi)
                     + SS.gammaln(0.5 * dof)
                     - SS.gammaln(0.5 * (dof + (N - D)))
                 )
             else:
                 nLL = 0.5 * (logdetK + (dof + N) * np.log(1.0 + r2 / dof))
                 nLL += (
-                    0.5 * N * np.log(dof * SP.pi)
+                    0.5 * N * np.log(dof * np.pi)
                     + SS.gammaln(0.5 * dof)
                     - SS.gammaln(0.5 * (dof + N))
                 )
             result = {
                 "nLL": nLL,
                 "dof": dof,
                 "beta": beta,
@@ -760,15 +758,15 @@
         ystar           : [M] 1-dimensional array of predicted phenotype values
         --------------------------------------------------------------------------
         """
 
         M = self.Xstar.shape[0]
 
         if (h2 < 0.0) or (h2 >= 1.0):
-            return SP.nan * SP.ones(M)
+            return np.nan * np.ones(M)
 
         k = self.S.shape[0]
         N = self.y.shape[0]
         # D=self.UX.shape[1]
 
         if logdelta is not None:
             delta = np.exp(logdelta)
@@ -808,19 +806,19 @@
             UUyres = yres - np.dot(self.U, Uyres)
             yrandom += np.dot(UUKstar.T, UUyres) / denom
 
         # proximal contamination (see Supplement Note 2: An Efficient Algorithm for Avoiding Proximal Contamination)
         # available at: http://www.nature.com/nmeth/journal/v9/n6/extref/nmeth.2037-S1.pdf
         # exclude SNPs from the RRM in the likelihood evaluation
         if len(self.exclude_idx) > 0:
-            UWS = self.UW / NP.lib.stride_tricks.as_strided(
+            UWS = self.UW / np.lib.stride_tricks.as_strided(
                 Sd, (Sd.size, num_exclude), (Sd.itemsize, 0)
             )
             assert UWS.shape == (k, num_exclude)
-            WW = NP.eye(num_exclude) - UWS.T.dot(self.UW)
+            WW = np.eye(num_exclude) - UWS.T.dot(self.UW)
             WKstar = UWS.T.dot(UKstar)
             Wyres = UWS.T.dot(Uyres)
             assert WW.shape == (num_exclude, num_exclude)
             assert WKstar.shape == (num_exclude, M)
             assert Wyres.shape == (num_exclude,)
 
             if k < N:  # low rank part
@@ -834,15 +832,15 @@
 
             UWKstar = U_WW.T.dot(WKstar)
             UWyres = U_WW.T.dot(Wyres)
             assert UWKstar.shape == (num_exclude, M)
             assert UWyres.shape == (num_exclude,)
 
             # compute S_WW^{-1} * UWX
-            WKstar = UWKstar / NP.lib.stride_tricks.as_strided(
+            WKstar = UWKstar / np.lib.stride_tricks.as_strided(
                 S_WW, (S_WW.size, UWKstar.shape[1]), (S_WW.itemsize, 0)
             )
             # compute S_WW^{-1} * UWy
             Wyres = UWyres / S_WW
             assert WKstar.shape == (num_exclude, M)
             assert Wyres.shape == (num_exclude,)
 
@@ -912,15 +910,15 @@
         --------------------------------------------------------------------------
         """
 
         # TODO: proximal contamination
         # TODO: REML?
 
         if (h2 < 0.0) or (h2 >= 1.0):
-            return SP.nan * SP.ones(M)
+            return np.nan * np.ones(M)
 
         k = self.S.shape[0]
         N = self.y.shape[0]
         # D = self.UX.shape[1]
 
         # print "k, N, D", k, N, D
 
@@ -948,26 +946,26 @@
         else:
             Kstar_star = Kstar_star.copy()
 
         N_test = Kstar_star.shape[0]
         assert N_test == Kstar_star.shape[1]
 
         part1 = Kstar_star
-        part1 += SP.eye(N_test) * delta
+        part1 += np.eye(N_test) * delta
         part1 *= sigma2
 
         # print "part1", part1[0,0]
         # print "delta", delta, "sigma2", sigma2
 
         # part 2 from c-code
         # (U1^T a)^T (S_1 + delta*I)^{-1} (U1^T a)
         SUKstarTUkStar = np.dot(Sdi * self.UKstar.T, self.UKstar)
 
-        # UXS = self.UKstar / NP.lib.stride_tricks.as_strided(Sd, (Sd.size,self.UKstar.shape[1]), (Sd.itemsize,0))
-        # NP.testing.assert_array_almost_equal(SUKstarTUkStar, np.dot(UXS.T, self.UKstar), decimal=4)
+        # UXS = self.UKstar / np.lib.stride_tricks.as_strided(Sd, (Sd.size,self.UKstar.shape[1]), (Sd.itemsize,0))
+        # np.testing.assert_array_almost_equal(SUKstarTUkStar, np.dot(UXS.T, self.UKstar), decimal=4)
 
         SUKstarTUkStar *= sigma2
 
         # print "UKstar[0,0]", self.UKstar[0,0]
         # print "UKstarS[0,0]", UXS[0,0]
         # print "SUK", SUKstarTUkStar[0,0]
 
@@ -1017,17 +1015,17 @@
 
         # TODO: benchmark, record speed difference
         """
         # efficient computation of: (y - mu)^T sigma2^{-1} (y - mu)
         # Solve the linear system x = (L L^T)^-1 res
 
         try:
-            L = SP.linalg.cho_factor(sigma)
-            res_sig = SP.linalg.cho_solve(L, res)
-            logdetK = NP.linalg.slogdet(sigma)[1]
+            L = np.linalg.cho_factor(sigma)
+            res_sig = np.linalg.cho_solve(L, res)
+            logdetK = np.linalg.slogdet(sigma)[1]
 
         except Exception, detail:
             print "Cholesky failed, using eigen-value decomposition!"
         """
 
         [S_, U_] = LA.eigh(sigma)
 
@@ -1041,23 +1039,23 @@
         Sdi = 1 / S
 
         res_sig = res.T.dot(Sdi * U).dot(U.T)
         logdetK = np.log(S).sum()
 
         # some sanity checks
         if False:
-            res_sig3 = SP.linalg.pinv(sigma).dot(res)
-            NP.testing.assert_array_almost_equal(res_sig, res_sig3, decimal=2)
+            res_sig3 = np.linalg.pinv(sigma).dot(res)
+            np.testing.assert_array_almost_equal(res_sig, res_sig3, decimal=2)
 
         # see Carl Rasmussen's book on GPs, equation 5.10, or
         term1 = -0.5 * logdetK
         term2 = -0.5 * np.dot(
             res_sig.reshape(-1).T, res.reshape(-1)
         )  # Change the inputs to the functions so that these are vectors, not 1xn,nx1
-        term3 = -0.5 * len(res) * np.log(2 * SP.pi)
+        term3 = -0.5 * len(res) * np.log(2 * np.pi)
 
         if term2 < -10000:
             logging.warning(
                 "looks like nLLeval_test is running into numerical difficulties"
             )
 
             SC = S.copy()
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/lmm2k.py` & `fastlmm-0.6.8b1/fastlmm/inference/lmm2k.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-from __future__ import absolute_import
-from __future__ import print_function
-import scipy as SP
 import numpy as NP
 import numpy as np
 import scipy.linalg as LA
 import scipy.optimize as opt
 import scipy.stats as ST
 import scipy.special as SS
 from fastlmm.util.mingrid import *
 from fastlmm.util.util import *
 import time
-import pdb
 
 from bin2kernel import Bin2Kernel
 from bin2kernel import makeBin2KernelAsEstimator
 from bin2kernel import Bin2KernelLaplaceLinearN
 from bin2kernel import getFastestBin2Kernel
 from bin2kernel import Bin2KernelEPLinearN
 
@@ -372,15 +368,15 @@
                 except LA.LinAlgError:  # revert to Eigenvalue decomposition
                     print(
                         "Got SVD exception, trying eigenvalue decomposition of square of G. Note that this is a little bit less accurate"
                     )
                     [S_, V_] = LA.eigh(self.G1rot.T.dot(self.G1rot))
                     S_nonz = S_ > 0.0
                     S1 = S_[S_nonz]
-                    U1 = self.G1rot.dot(V_[:, S_nonz] / SP.sqrt(S1))
+                    U1 = self.G1rot.dot(V_[:, S_nonz] / np.sqrt(S1))
                     self.eig1 = [S1, U1]
         return self.eig1
 
     def getEig0(self):
         """ """
         if self.eig0 is None:
             # compute eig0
@@ -394,15 +390,15 @@
                 except LA.LinAlgError:  # revert to Eigenvalue decomposition
                     print(
                         "Got SVD exception, trying eigenvalue decomposition of square of G. Note that this is a little bit less accurate"
                     )
                     [S_, V_] = LA.eigh(self.G0.T.dot(self.G0))
                     S_nonz = S_ > 0.0
                     S0 = S_[S_nonz]
-                    U0 = self.G0.dot(V_[:, S_nonz] / SP.sqrt(S0))
+                    U0 = self.G0.dot(V_[:, S_nonz] / np.sqrt(S0))
                     self.eig0 = [S0, U0]
         return self.eig1
 
     def set_exclude_idx(self, idx):
         """
         Set the indices of SNPs to be removed
         --------------------------------------------------------------------------
@@ -637,19 +633,19 @@
                 logdetXX = np.log(Sxx).sum()
                 logdetXKX = np.log(SxKx).sum()
                 sigma2 = r2 / (N - D)
                 nLL = 0.5 * (
                     logdetK
                     + logdetXKX
                     - logdetXX
-                    + (N - D) * (np.log(2.0 * SP.pi * sigma2) + 1)
+                    + (N - D) * (np.log(2.0 * np.pi * sigma2) + 1)
                 )
             else:
                 sigma2 = r2 / (N)
-                nLL = 0.5 * (logdetK + N * (np.log(2.0 * SP.pi * sigma2) + 1))
+                nLL = 0.5 * (logdetK + N * (np.log(2.0 * np.pi * sigma2) + 1))
             result = {
                 "nLL": nLL,
                 "sigma2": sigma2,
                 "beta": beta,
                 "gamma1": gamma1,
                 "REML": REML,
                 "gamma0": self.gamma0,
@@ -666,22 +662,22 @@
                 nLL = 0.5 * (
                     logdetK
                     + logdetXKX
                     - logdetXX
                     + (dof + (N - D)) * np.log(1.0 + r2 / dof)
                 )
                 nLL += (
-                    0.5 * (N - D) * np.log(dof * SP.pi)
+                    0.5 * (N - D) * np.log(dof * np.pi)
                     + SS.gammaln(0.5 * dof)
                     - SS.gammaln(0.5 * (dof + (N - D)))
                 )
             else:
                 nLL = 0.5 * (logdetK + (dof + N) * np.log(1.0 + r2 / dof))
                 nLL += (
-                    0.5 * N * np.log(dof * SP.pi)
+                    0.5 * N * np.log(dof * np.pi)
                     + SS.gammaln(0.5 * dof)
                     - SS.gammaln(0.5 * (dof + N))
                 )
             result = {
                 "nLL": nLL,
                 "dof": dof,
                 "sigma2": sigma2,
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/lmm_cov.py` & `fastlmm-0.6.8b1/fastlmm/inference/lmm_cov.py`

 * *Files 2% similar despite different names*

```diff
@@ -929,15 +929,15 @@
         YKY = np.full(P, np.nan)
         for pheno_index in range(P):
             YKY[pheno_index] = self.computeAKA(
                 Sd=Sd[:, pheno_index : pheno_index + 1],
                 denom=denom[pheno_index],
                 UA=UY[:, pheno_index : pheno_index + 1],
                 UUA=None if UUY is None else UUY[:, pheno_index : pheno_index + 1],
-            )
+            ).item()
 
         logdetK = np.log(Sd).sum(0)
 
         if UUY is not None:  # low rank part
             logdetK += (N - k) * np.log(denom)
 
         if Usnps is not None:
@@ -1032,21 +1032,21 @@
             logdetK += np.log(np.absolute(S_WW)).sum()
 
             ########
 
         if Usnps is not None:
             penalty_ = penalty or 0.0
             assert penalty_ >= 0.0, "penalty has to be non-negative"
-            with warnings.catch_warnings():
-                warnings.filterwarnings(
-                    "ignore",
-                    category=RuntimeWarning,
-                    message="invalid value encountered in divide",
-                )
+            old_settings = np.seterr(
+                divide="ignore", invalid="ignore"
+            )  # turn /0 into NaN
+            try:
                 beta = snpsKY / (snpsKsnps + penalty_)
+            finally:
+                np.seterr(**old_settings)
             if np.isnan(beta.min()):
                 logging.debug(
                     "NaN beta value seen, may be due to an SNC (a constant SNP)"
                 )
                 beta[snpsKY == 0] = 0.0
             variance_explained_beta = snpsKY * beta
             r2 = YKY[np.newaxis, :] - variance_explained_beta
@@ -1057,21 +1057,19 @@
                     * (snpsKsnps / ((snpsKsnps + penalty_) * (snpsKsnps + penalty_)))
                 )  # note that we assume the loss in DOF is 1 here, even though it is less, so the
                 # variance estimate is conservative, due to N-1 for penalty case
                 variance_explained_beta *= (snpsKsnps / (snpsKsnps + penalty_)) * (
                     snpsKsnps / (snpsKsnps + penalty_)
                 )
             else:
-                with warnings.catch_warnings():
-                    warnings.filterwarnings(
-                        "ignore",
-                        category=RuntimeWarning,
-                        message="divide by zero encountered in divide",
-                    )
+                old_settings = np.seterr(divide="ignore")  # turn /0 into NaN
+                try:
                     variance_beta = r2 / (N - 1.0) / snpsKsnps
+                finally:
+                    np.seterr(**old_settings)
                 fraction_variance_explained_beta = (
                     variance_explained_beta / YKY[np.newaxis, :]
                 )  # variance explained by beta over total variance
         else:
             r2 = YKY
             beta = None
             variance_beta = None
@@ -1213,15 +1211,15 @@
 
     linreg = linreg(X=X)
     Kinv_ = linreg.regress(Kinv)
     Kinv_ = linreg.regress(Kinv_.T)
     P_ = Kinv_  # this one does not match with P
 
     X_K_ = linreg.regress(X_K)
-    S_x = linreg.regress(sp.eye(N))
+    S_x = linreg.regress(np.eye(N))
     S_x = linreg.regress(S_x.T)
     K_ = X_K_.dot(X_K_.T) + S_x
     [u, s, v] = la.svd(X_K_)  # Use big_svd
     inonz = s > 1e-10
     s = s[inonz] * s[inonz] + 1
 
     u = u[:, inonz]
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/tests/test.py` & `fastlmm-0.6.8b1/fastlmm/inference/tests/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from __future__ import absolute_import
-import numpy as NP
 import numpy as np
-import scipy as SP
+import scipy.optimize as opt
 from fastlmm.inference.laplace import LaplaceGLMM_N3K1, LaplaceGLMM_N1K3
 from fastlmm.inference.ep import EPGLMM_N3K1, EPGLMM_N1K3
 from fastlmm.inference import getLMM
 import unittest
 import os.path
 import logging
 
@@ -74,26 +72,26 @@
         model.setG(G0=self._G0, G1=self._G1, a2=self._a2)
         model.setX(self._X)
         model.sety(self._y)
         result = model.nLLeval(REML=False, delta=1.0)
 
         target_result = {
             "scale": 1.0,
-            "beta": NP.array([0.05863443]),
+            "beta": np.array([0.05863443]),
             "a2": 0.4,
             "REML": False,
             "nLL": 91.92983775736522,
             "sigma2": 0.94826207355429604,
             "variance_beta": 0.0118125903,
             "h2": 0.5,
         }
 
         # make sure results are the same
         for key in result.keys():
-            NP.testing.assert_array_almost_equal(result[key], target_result[key])
+            np.testing.assert_array_almost_equal(result[key], target_result[key])
             # self.assertAlmostEqual(result[key], target_result[key])
 
     def test_nLLeval_2(self):
         """
         small regression test to check negative log likelihood function
 
         delta = 1, REML = True
@@ -104,23 +102,23 @@
         model.setX(self._X)
         model.sety(self._y)
         result = model.nLLeval(REML=True, delta=1.0)
 
         target_result = {
             "scale": 1.0,
             "h2": 0.0,
-            "beta": NP.array([0.05863443]),
+            "beta": np.array([0.05863443]),
             "a2": 0.4,
             "REML": True,
             "nLL": 90.940636012858121,
             "sigma2": 0.96761436076968987,
         }
         # make sure results are the same
         for key in result.keys():
-            NP.testing.assert_array_almost_equal(result[key], target_result[key])
+            np.testing.assert_array_almost_equal(result[key], target_result[key])
             # self.assertAlmostEqual(result[key], target_result[key])
 
     def test_nLLeval_3(self):
         """
         small regression test to check negative log likelihood function
 
         delta = None, h2 = 0.5, REML = True
@@ -131,23 +129,23 @@
         model.setX(self._X)
         model.sety(self._y)
         result = model.nLLeval(REML=True, delta=None, h2=0.5)
 
         target_result = {
             "scale": 1.0,
             "h2": 0.5,
-            "beta": NP.array([0.05863443]),
+            "beta": np.array([0.05863443]),
             "a2": 0.4,
             "REML": True,
             "nLL": 90.940636012858121,
             "sigma2": 1.9352287215393797,
         }
         # make sure results are the same
         for key in result.keys():
-            NP.testing.assert_array_almost_equal(result[key], target_result[key])
+            np.testing.assert_array_almost_equal(result[key], target_result[key])
             # self.assertAlmostEqual(result[key], target_result[key])
 
 
 class TestProximalContamination(unittest.TestCase):
     def test_one_kernel_fullrank(self):
         """
         test for one kernel only, using delta=1.0, REML=False
@@ -181,18 +179,18 @@
         ret_cut = lmm_cut.nLLeval(REML=False, delta=delta)
 
         lmm_cut.setTestData(Xstar=X[:3], G0star=G0[:3])
         ypred_cut = lmm_cut.predictMean(beta=ret_cut["beta"], delta=delta)
 
         # make sure results are the same
         for key in ret_nocut.keys():
-            NP.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
+            np.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
             # self.assertAlmostEqual(ret_cut[key], ret_nocut[key])
 
-        wproj = NP.random.randn(ypred_nocut.shape[0])
+        wproj = np.random.randn(ypred_nocut.shape[0])
         self.assertAlmostEqual((wproj * ypred_nocut).sum(), (wproj * ypred_cut).sum())
 
     def test_one_kernel_lowrank(self):
         """
         test for one kernel only, using delta=1.0, REML=False
         """
         delta = 1.0
@@ -221,18 +219,18 @@
 
         ret_cut = lmm_cut.nLLeval(REML=False, delta=delta)
         lmm_cut.setTestData(Xstar=X[:3], G0star=G0[:3])
         ypred_cut = lmm_cut.predictMean(beta=ret_cut["beta"], delta=delta)
 
         # make sure results are the same
         for key in ret_nocut.keys():
-            NP.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
+            np.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
             # self.assertAlmostEqual(ret_cut[key], ret_nocut[key])
 
-        wproj = NP.random.randn(ypred_nocut.shape[0])
+        wproj = np.random.randn(ypred_nocut.shape[0])
         self.assertAlmostEqual((wproj * ypred_nocut).sum(), (wproj * ypred_cut).sum())
 
     def test_two_kernels_fullrank(self):
         """
         two kernels, using delta=1.0, REML=False
         """
         delta = 1.0
@@ -261,17 +259,17 @@
 
         ret_cut = lmm_cut.nLLeval(REML=False, delta=delta)
         lmm_cut.setTestData(Xstar=X[:3], G0star=G0[:3], G1star=G1[:3])
         ypred_cut = lmm_cut.predictMean(beta=ret_cut["beta"], delta=delta)
 
         # make sure results are the same
         for key in ret_nocut.keys():
-            NP.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
+            np.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
             # self.assertAlmostEqual(ret_cut[key], ret_nocut[key])
-        wproj = NP.random.randn(ypred_nocut.shape[0])
+        wproj = np.random.randn(ypred_nocut.shape[0])
         self.assertAlmostEqual((wproj * ypred_nocut).sum(), (wproj * ypred_cut).sum())
 
     def test_two_kernels_lowrank(self):
         """
         two kernels, using delta=1.0, REML=False
         """
         delta = 1.0
@@ -300,17 +298,17 @@
 
         ret_cut = lmm_cut.nLLeval(REML=False, delta=delta)
         lmm_cut.setTestData(Xstar=X[:3], G0star=G0[:3], G1star=G1[:3])
         ypred_cut = lmm_cut.predictMean(beta=ret_cut["beta"], delta=delta)
 
         # make sure results are the same
         for key in ret_nocut.keys():
-            NP.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
+            np.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
             # self.assertAlmostEqual(ret_cut[key], ret_nocut[key])
-        wproj = NP.random.randn(ypred_nocut.shape[0])
+        wproj = np.random.randn(ypred_nocut.shape[0])
         self.assertAlmostEqual((wproj * ypred_nocut).sum(), (wproj * ypred_cut).sum())
 
     def test_two_kernels_fullrank_REML(self):
         """
         two kernels, using delta=1.0, REML=True
         """
         delta = 2.0
@@ -335,15 +333,15 @@
         lmm_cut.sety(y)
         lmm_cut.set_exclude_idx(exclude_idx)
 
         ret_cut = lmm_cut.nLLeval(REML=True, delta=delta)
 
         # make sure results are the same
         for key in ret_nocut.keys():
-            NP.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
+            np.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
             # self.assertAlmostEqual(ret_cut[key], ret_nocut[key])
 
     def test_two_kernels_lowrank_REML(self):
         """
         two kernels, using delta=1.0, REML=True
         """
         delta = 0.5
@@ -368,34 +366,34 @@
         lmm_cut.sety(y)
         lmm_cut.set_exclude_idx(exclude_idx)
 
         ret_cut = lmm_cut.nLLeval(REML=True, delta=delta)
 
         # make sure results are the same
         for key in ret_nocut.keys():
-            NP.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
+            np.testing.assert_array_almost_equal(ret_cut[key], ret_nocut[key])
             # self.assertAlmostEqual(ret_cut[key], ret_nocut[key])
 
 
 def generate_random_data(N, d, s_c):
     """
     small helper to generate a random data set
     """
 
     num_excludes = s_c // 2
     s = s_c  # total number of SNPs to be tested
 
-    X = NP.ones((N, d))
-    y = NP.random.rand(N)
+    X = np.ones((N, d))
+    y = np.random.rand(N)
 
-    G0 = NP.random.rand(N, s_c)
-    G1 = NP.random.rand(N, s)
+    G0 = np.random.rand(N, s_c)
+    G1 = np.random.rand(N, s)
 
     # exclude randomly
-    perm = NP.random.permutation(s_c)
+    perm = np.random.permutation(s_c)
     exclude_idx = perm[:num_excludes]
     include_idx = perm[num_excludes:]
     G0_small = G0[:, include_idx]
 
     return X, y, G0, G1, G0_small, exclude_idx
 
 
@@ -421,128 +419,128 @@
         model = LaplaceGLMM_N3K1("logistic")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
 
         self.assertAlmostEqual(
             -13.821329282675068, model._regular_marginal_loglikelihood()
         )
 
         model = EPGLMM_N3K1("erf")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
 
         self.assertAlmostEqual(
             -16.599719862714529, model._regular_marginal_loglikelihood()
         )
 
     def test_margll(self):
         model = LaplaceGLMM_N3K1("logistic", "l2")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
         self.assertAlmostEqual(-14.635329282675063, model.marginal_loglikelihood())
 
         model = EPGLMM_N3K1("erf", "l2")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
         self.assertAlmostEqual(-17.413719862714526, model.marginal_loglikelihood())
 
     def test_rmargll_after_optimization(self):
         model = LaplaceGLMM_N3K1("logistic")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
         model.optimize()
 
         self.assertAlmostEqual(-6.75677866924, model._regular_marginal_loglikelihood())
 
         model = EPGLMM_N3K1("erf")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
         model.optimize()
 
         self.assertAlmostEqual(-6.75424440734, model._regular_marginal_loglikelihood())
 
         model = LaplaceGLMM_N3K1("logistic", "l2")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
         model.optimize()
 
         self.assertAlmostEqual(
             -6.7584132443836662, model._regular_marginal_loglikelihood()
         )
 
         model = EPGLMM_N3K1("erf", "l2")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
         model.optimize()
 
         self.assertAlmostEqual(
             -6.7545709287754718, model._regular_marginal_loglikelihood()
         )
 
     def test_setK_rmargll_after_optimization(self):
         model = LaplaceGLMM_N3K1("logistic")
-        model.setK(NP.dot(self._G0, self._G0.T), NP.dot(self._G1, self._G1.T))
+        model.setK(np.dot(self._G0, self._G0.T), np.dot(self._G1, self._G1.T))
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
         model.optimize()
 
         self.assertAlmostEqual(-6.75677866924, model._regular_marginal_loglikelihood())
 
         model = EPGLMM_N3K1("erf")
-        model.setK(NP.dot(self._G0, self._G0.T), NP.dot(self._G1, self._G1.T))
+        model.setK(np.dot(self._G0, self._G0.T), np.dot(self._G1, self._G1.T))
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
         model.optimize()
 
         self.assertAlmostEqual(-6.75424440734, model._regular_marginal_loglikelihood())
 
     def test_rmargll_gradient(self):
         def func(x, model):
             model.sig02 = x[0]
@@ -561,30 +559,26 @@
         model = LaplaceGLMM_N3K1("logistic")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
 
         self.assertAlmostEqual(
             0.0,
-            SP.optimize.check_grad(
-                func, grad, NP.array([1.0, 1.2, 1.5, -3.0, 0.4]), model
-            ),
+            opt.check_grad(func, grad, np.array([1.0, 1.2, 1.5, -3.0, 0.4]), model),
             places=5,
         )
 
         model = EPGLMM_N3K1("erf")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
 
         self.assertAlmostEqual(
             0.0,
-            SP.optimize.check_grad(
-                func, grad, NP.array([1.0, 1.2, 1.5, -3.0, 0.4]), model
-            ),
+            opt.check_grad(func, grad, np.array([1.0, 1.2, 1.5, -3.0, 0.4]), model),
             places=5,
         )
 
     def test_margll_gradient(self):
         def func(x, model):
             model.sig02 = x[0]
             model.sig12 = x[1]
@@ -601,43 +595,39 @@
 
         model = LaplaceGLMM_N3K1("logistic", "l2")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         self.assertAlmostEqual(
             0.0,
-            SP.optimize.check_grad(
-                func, grad, NP.array([1.0, 1.2, 1.5, -3.0, 0.4]), model
-            ),
+            opt.check_grad(func, grad, np.array([1.0, 1.2, 1.5, -3.0, 0.4]), model),
             places=5,
         )
 
         model = EPGLMM_N3K1("erf", "l2")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         self.assertAlmostEqual(
             0.0,
-            SP.optimize.check_grad(
-                func, grad, NP.array([1.0, 1.2, 1.5, -3.0, 0.4]), model
-            ),
+            opt.check_grad(func, grad, np.array([1.0, 1.2, 1.5, -3.0, 0.4]), model),
             places=5,
         )
 
     def test_prediction(self):
         model = LaplaceGLMM_N3K1("logistic")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
 
-        ps = NP.array(
+        ps = np.array(
             [
                 0.30481858,
                 0.22520247,
                 0.78060709,
                 0.44734337,
                 0.58824651,
                 0.052388,
@@ -655,17 +645,17 @@
         model = EPGLMM_N3K1("erf")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
 
-        ps = NP.array(
+        ps = np.array(
             [
                 0.35487175,
                 0.20959901,
                 0.77285232,
                 0.48305102,
                 0.59542164,
                 0.02770879,
@@ -684,53 +674,53 @@
         model = LaplaceGLMM_N1K3("logistic")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
 
         self.assertAlmostEqual(
             -13.821329282675068, model._regular_marginal_loglikelihood()
         )
 
         model = EPGLMM_N1K3("erf")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
 
         self.assertAlmostEqual(-16.5997198627, model._regular_marginal_loglikelihood())
 
     def testr_rmargll_after_optimization_linearn(self):
         model = LaplaceGLMM_N1K3("logistic")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
         model.optimize()
 
         self.assertAlmostEqual(-6.75677866924, model._regular_marginal_loglikelihood())
 
-        # cmk
+        # switch out brent
         # model = EPGLMM_N1K3("erf")
         # model.setG(self._G0, self._G1)
         # model.setX(self._X)
         # model.sety(self._y)
         # model.sig02 = 1.5
         # model.sig12 = 0.5
         # model.sign2 = 0.8
-        # model.beta = NP.array([2.0, -1.0])
+        # model.beta = np.array([2.0, -1.0])
         # model.optimize()
 
         # self.assertAlmostEqual(-6.75424440734, model._regular_marginal_loglikelihood())
 
     def test_rmargll_gradient_linearn(self):
         def func(x, model):
             model.sig02 = x[0]
@@ -749,44 +739,40 @@
         model = LaplaceGLMM_N1K3("logistic")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
 
         self.assertAlmostEqual(
             0.0,
-            SP.optimize.check_grad(
-                func, grad, NP.array([1.0, 1.2, 1.5, -3.0, 0.4]), model
-            ),
+            opt.check_grad(func, grad, np.array([1.0, 1.2, 1.5, -3.0, 0.4]), model),
             places=5,
         )
 
         model = EPGLMM_N1K3("erf")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
 
         self.assertAlmostEqual(
             0.0,
-            SP.optimize.check_grad(
-                func, grad, NP.array([1.0, 1.2, 1.5, -3.0, 0.4]), model
-            ),
+            opt.check_grad(func, grad, np.array([1.0, 1.2, 1.5, -3.0, 0.4]), model),
             places=5,
         )
 
     def test_prediction_linearn(self):
         model = LaplaceGLMM_N1K3("logistic")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
 
-        ps = NP.array(
+        ps = np.array(
             [
                 0.30483881,
                 0.2252297,
                 0.78056257,
                 0.44734442,
                 0.58824122,
                 0.05238813,
@@ -804,17 +790,17 @@
         model = EPGLMM_N1K3("erf")
         model.setG(self._G0, self._G1)
         model.setX(self._X)
         model.sety(self._y)
         model.sig02 = 1.5
         model.sig12 = 0.5
         model.sign2 = 0.8
-        model.beta = NP.array([2.0, -1.0])
+        model.beta = np.array([2.0, -1.0])
 
-        ps = NP.array(
+        ps = np.array(
             [
                 0.35487175,
                 0.20959901,
                 0.77285232,
                 0.48305102,
                 0.59542164,
                 0.02770879,
```

### Comparing `fastlmm-0.6.7/fastlmm/inference/tests/test_fastlmm_predictor.py` & `fastlmm-0.6.8b1/fastlmm/inference/tests/test_fastlmm_predictor.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/inference/tests/test_linear_regression.py` & `fastlmm-0.6.8b1/fastlmm/inference/tests/test_linear_regression.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import logging
 import numpy as np
 import unittest
 import os.path
 import doctest
 import pandas as pd
 import pysnptools.util as pstutil
@@ -14,196 +12,262 @@
 from pysnptools.snpreader import Dat, Bed, Pheno, SnpData
 from fastlmm.feature_selection.test import TestFeatureSelection
 from pysnptools.standardizer import Unit, Standardizer
 from pysnptools.standardizer import Identity as SS_Identity
 from pysnptools.kernelstandardizer import Identity as KS_Identity
 from pysnptools.kernelreader import Identity as KernelIdentity
 from pysnptools.kernelreader import KernelData, SnpKernel
-from six.moves import range
+
 
 class TestLinRegTrain(unittest.TestCase):
     @classmethod
     def setUpClass(self):
         from pysnptools.util import create_directory_if_necessary
-        create_directory_if_necessary(self.tempout_dir, isfile=False)
-        self.pythonpath = os.path.abspath(os.path.join(os.path.dirname(os.path.realpath(__file__)),"..","..",".."))
 
-        self.snpreader_whole = Bed(self.pythonpath + "/tests/datasets/synth/all.bed",count_A1=False)
+        create_directory_if_necessary(self.tempout_dir, isfile=False)
+        self.pythonpath = os.path.abspath(
+            os.path.join(os.path.dirname(os.path.realpath(__file__)), "..", "..", "..")
+        )
+
+        self.snpreader_whole = Bed(
+            self.pythonpath + "/tests/datasets/synth/all.bed", count_A1=False
+        )
         self.covariate_whole = Pheno(self.pythonpath + "/tests/datasets/synth/cov.txt")
-        self.pheno_whole = Pheno(self.pythonpath + "/tests/datasets/synth/pheno_10_causals.txt")
+        self.pheno_whole = Pheno(
+            self.pythonpath + "/tests/datasets/synth/pheno_10_causals.txt"
+        )
 
     tempout_dir = "tempout/linear_regression"
 
-    def file_name(self,testcase_name):
-        temp_fn = os.path.join(self.tempout_dir,testcase_name+".dat")
+    def file_name(self, testcase_name):
+        temp_fn = os.path.join(self.tempout_dir, testcase_name + ".dat")
         if os.path.exists(temp_fn):
             os.remove(temp_fn)
         return temp_fn
 
     def test_lr_real(self):
         do_plot = False
 
         import pylab
+
         logging.info("TestLinRegTrain test_lr_real")
 
-        train_idx = np.r_[10:self.snpreader_whole.iid_count] # iids 10 and on
-        test_idx  = np.r_[0:10] # the first 10 iids
+        train_idx = np.r_[10 : self.snpreader_whole.iid_count]  # iids 10 and on
+        test_idx = np.r_[0:10]  # the first 10 iids
 
-        #make covar just numbers 0,1,...
+        # make covar just numbers 0,1,...
         covar = self.covariate_whole.read()
         covar.val = np.array([[float(num)] for num in range(covar.iid_count)])
-        covariate_train = covar[train_idx,:].read()
-        covariate_test = covar[test_idx,:].read()
+        covariate_train = covar[train_idx, :].read()
+        covariate_test = covar[test_idx, :].read()
         K0_test_test = KernelIdentity(covariate_test.iid)
 
-        #make pheno  # pheno = 2*covar+100+normal(0,1)*10
+        # make pheno  # pheno = 2*covar+100+normal(0,1)*10
         pheno = self.pheno_whole.read()
         np.random.seed(0)
-        pheno.val = covar.val * 2.0 + 100 + np.random.normal(size=covar.val.shape)*10
+        pheno.val = covar.val * 2.0 + 100 + np.random.normal(size=covar.val.shape) * 10
 
-        pheno_train = pheno[train_idx,:].read()
-        pheno_test = pheno[test_idx,:].read()
+        pheno_train = pheno[train_idx, :].read()
+        pheno_test = pheno[test_idx, :].read()
 
         if do_plot:
-            #Plot training x and y, testing x and y
-            pylab.plot(covariate_train.val, pheno_train.val,".",covariate_test.val, pheno_test.val,".")
+            # Plot training x and y, testing x and y
+            pylab.plot(
+                covariate_train.val,
+                pheno_train.val,
+                ".",
+                covariate_test.val,
+                pheno_test.val,
+                ".",
+            )
             pylab.suptitle("Plot training x and y, testing x and y")
             pylab.show()
 
-        Xtrain = np.c_[covariate_train.val,np.ones((covariate_train.iid_count,1))]
-        Xtest = np.c_[covariate_test.val,np.ones((covariate_test.iid_count,1))]
-        lsqSol = np.linalg.lstsq(Xtrain, pheno_train.val[:,0],rcond=-1)
-        bs=lsqSol[0] #weights
-        r2=lsqSol[1] #squared residuals
-        D=lsqSol[2]  #rank of design matrix
-        N=pheno_train.iid_count
+        Xtrain = np.c_[covariate_train.val, np.ones((covariate_train.iid_count, 1))]
+        Xtest = np.c_[covariate_test.val, np.ones((covariate_test.iid_count, 1))]
+        lsqSol = np.linalg.lstsq(Xtrain, pheno_train.val[:, 0], rcond=-1)
+        bs = lsqSol[0]  # weights
+        r2 = lsqSol[1]  # squared residuals
+        D = lsqSol[2]  # rank of design matrix
+        N = pheno_train.iid_count
         REML = False
         if not REML:
-            sigma2 = float(r2/N)
-            nLL =  N*0.5*np.log(2*np.pi*sigma2) + N*0.5
+            sigma2 = float(r2 / N)
+            nLL = N * 0.5 * np.log(2 * np.pi * sigma2) + N * 0.5
         else:
-            sigma2 = float(r2 / (N-D))
-            nLL = N*0.5*np.log(2*np.pi*sigma2) + 0.5/sigma2*r2;
-            nLL -= 0.5*D*np.log(2*np.pi*sigma2);#REML term
+            sigma2 = float(r2 / (N - D))
+            nLL = N * 0.5 * np.log(2 * np.pi * sigma2) + 0.5 / sigma2 * r2
+            nLL -= 0.5 * D * np.log(2 * np.pi * sigma2)
+            # REML term
 
         predicted = Xtest.dot(bs)
         yerr = [np.sqrt(sigma2)] * len(predicted)
         if do_plot:
-            pylab.plot(covariate_test.val, pheno_test.val,"g.",covariate_test.val, predicted,"r.")
+            pylab.plot(
+                covariate_test.val,
+                pheno_test.val,
+                "g.",
+                covariate_test.val,
+                predicted,
+                "r.",
+            )
             pylab.xlim([-1, 10])
-            pylab.errorbar(covariate_test.val, predicted,yerr,linestyle='None')
+            pylab.errorbar(covariate_test.val, predicted, yerr, linestyle="None")
             pylab.suptitle("real linear regression: actual to prediction")
             pylab.show()
 
-        #These should all give the same result
+        # These should all give the same result
         first_name = None
-        for name,K0_train,K0_whole_test in [("Identity Kernel",None,None)]:
+        for name, K0_train, K0_whole_test in [("Identity Kernel", None, None)]:
 
             first_name = first_name or name
-            #Learn model, save, load
-            modelx = LinearRegression().fit(K0_train=K0_train, X=covariate_train, y=pheno_train)
-                
-                
+            # Learn model, save, load
+            modelx = LinearRegression().fit(
+                K0_train=K0_train, X=covariate_train, y=pheno_train
+            )
+
             filename = self.tempout_dir + "/model_lr_real.flm.p"
             pstutil.create_directory_if_necessary(filename)
             model = modelx
 
             do_test_on_train = True
             if do_test_on_train:
-                #Predict with model (test on train)
-                predicted_pheno, covar = model.predict(K0_whole_test=K0_train, X=covariate_train) #test on train
-                output_file = self.file_name("lr_reala_"+name)
-                Dat.write(output_file,predicted_pheno)
-                covar2 = SnpData(iid=covar.row,sid=covar.col[:,1],val=covar.val) #kludge to write kernel to text format
-                output_file = self.file_name("lr_reala.cov_"+name)
-                Dat.write(output_file,covar2)
+                # Predict with model (test on train)
+                predicted_pheno, covar = model.predict(
+                    K0_whole_test=K0_train, X=covariate_train
+                )  # test on train
+                output_file = self.file_name("lr_reala_" + name)
+                Dat.write(output_file, predicted_pheno)
+                covar2 = SnpData(
+                    iid=covar.row, sid=covar.col[:, 1], val=covar.val
+                )  # kludge to write kernel to text format
+                output_file = self.file_name("lr_reala.cov_" + name)
+                Dat.write(output_file, covar2)
 
                 yerr = np.sqrt(np.diag(covar.val))
                 predicted = predicted_pheno.val
                 if do_plot:
-                    pylab.plot(covariate_train.val, pheno_train.val,"g.",covariate_train.val, predicted,"r.")
+                    pylab.plot(
+                        covariate_train.val,
+                        pheno_train.val,
+                        "g.",
+                        covariate_train.val,
+                        predicted,
+                        "r.",
+                    )
                     pylab.xlim([0, 50])
                     pylab.ylim([100, 200])
-                    pylab.errorbar(covariate_train.val, predicted,yerr,linestyle='None')
-                    pylab.suptitle(name+": test on train: train X to true target (green) and prediction (red)")
+                    pylab.errorbar(
+                        covariate_train.val, predicted, yerr, linestyle="None"
+                    )
+                    pylab.suptitle(
+                        name
+                        + ": test on train: train X to true target (green) and prediction (red)"
+                    )
                     pylab.show()
 
-                self.compare_files(predicted_pheno,"lr2a_"+first_name)
-                self.compare_files(covar2,"lr2a.cov_"+first_name)
+                self.compare_files(predicted_pheno, "lr2a_" + first_name)
+                self.compare_files(covar2, "lr2a.cov_" + first_name)
 
-            #Predict with model (test on test)
-            predicted_pheno, covar  = model.predict(K0_whole_test=K0_whole_test, X=covariate_test) #test on train
-            output_file = self.file_name("lr_realb_"+name)
-            Dat.write(output_file,predicted_pheno)
-            covar2 = SnpData(iid=covar.row,sid=covar.col[:,1],val=covar.val) #kludge to write kernel to text format
-            output_file = self.file_name("lr_realb.cov_"+name)
-            Dat.write(output_file,covar2)
+            # Predict with model (test on test)
+            predicted_pheno, covar = model.predict(
+                K0_whole_test=K0_whole_test, X=covariate_test
+            )  # test on train
+            output_file = self.file_name("lr_realb_" + name)
+            Dat.write(output_file, predicted_pheno)
+            covar2 = SnpData(
+                iid=covar.row, sid=covar.col[:, 1], val=covar.val
+            )  # kludge to write kernel to text format
+            output_file = self.file_name("lr_realb.cov_" + name)
+            Dat.write(output_file, covar2)
 
             yerr = np.sqrt(np.diag(covar.val))
             predicted = predicted_pheno.val
             if do_plot:
-                pylab.plot(covariate_test.val, pheno_test.val,"g.",covariate_test.val, predicted,"r.")
+                pylab.plot(
+                    covariate_test.val,
+                    pheno_test.val,
+                    "g.",
+                    covariate_test.val,
+                    predicted,
+                    "r.",
+                )
                 pylab.xlim([-1, 10])
-                pylab.errorbar(covariate_test.val, predicted,yerr,linestyle='None')
-                pylab.suptitle(name+": test on test: test X to true target (green) and prediction (red)")
+                pylab.errorbar(covariate_test.val, predicted, yerr, linestyle="None")
+                pylab.suptitle(
+                    name
+                    + ": test on test: test X to true target (green) and prediction (red)"
+                )
                 pylab.show()
                 ## Plot y and predicted y (test on train)
-                #pylab.plot(pheno_test.val,predicted_pheno.val,".")
-                #pylab.suptitle(name+": test on test: true target to prediction")
-                #pylab.show()
-
-            self.compare_files(predicted_pheno,"lr2b_"+first_name)
-            self.compare_files(covar2,"lr2b.cov_"+first_name)
-
-
-
-    def compare_files(self,answer,ref_base):
-        reffile = TestFeatureSelection.reference_file("fastlmm/"+ref_base+".dat") #Uses same results folder as lmm_train
-        reference=Dat(reffile).read()
-        assert np.array_equal(answer.col,reference.col), "sid differs. File '{0}'".format(reffile)
-        assert np.array_equal(answer.row,reference.row), "iid differs. File '{0}'".format(reffile)
+                # pylab.plot(pheno_test.val,predicted_pheno.val,".")
+                # pylab.suptitle(name+": test on test: true target to prediction")
+                # pylab.show()
+
+            self.compare_files(predicted_pheno, "lr2b_" + first_name)
+            self.compare_files(covar2, "lr2b.cov_" + first_name)
+
+    def compare_files(self, answer, ref_base):
+        reffile = TestFeatureSelection.reference_file(
+            "fastlmm/" + ref_base + ".dat"
+        )  # Uses same results folder as lmm_train
+        reference = Dat(reffile).read()
+        assert np.array_equal(
+            answer.col, reference.col
+        ), "sid differs. File '{0}'".format(reffile)
+        assert np.array_equal(
+            answer.row, reference.row
+        ), "iid differs. File '{0}'".format(reffile)
         for iid_index in range(reference.row_count):
             for sid_index in range(reference.col_count):
-                a_v = answer.val[iid_index,sid_index]
-                r_v = reference.val[iid_index,sid_index]
-                assert abs(a_v - r_v) < 1e-4, "Value at {0},{1} differs too much from file '{2}'".format(iid_index,sid_index,reffile)
+                a_v = answer.val[iid_index, sid_index]
+                r_v = reference.val[iid_index, sid_index]
+                assert (
+                    abs(a_v - r_v) < 1e-4
+                ), "Value at {0},{1} differs too much from file '{2}'".format(
+                    iid_index, sid_index, reffile
+                )
 
     def test_doctest(self):
         old_dir = os.getcwd()
-        os.chdir(os.path.dirname(os.path.realpath(__file__))+"/..")
-        result = doctest.testmod(sys.modules['fastlmm.inference.linear_regression'])
+        os.chdir(os.path.dirname(os.path.realpath(__file__)) + "/..")
+        result = doctest.testmod(sys.modules["fastlmm.inference.linear_regression"])
         os.chdir(old_dir)
         assert result.failed == 0, "failed doc test: " + __file__
 
 
 def getTestSuite():
     suite1 = unittest.TestLoader().loadTestsFromTestCase(TestLinRegTrain)
     return unittest.TestSuite([suite1])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     logging.basicConfig(level=logging.DEBUG)
 
     # this import is needed for the runner
-    #from fastlmm.inference.tests.test_linear_regression import TestLinRegTrain
+    # from fastlmm.inference.tests.test_linear_regression import TestLinRegTrain
     suites = unittest.TestSuite([getTestSuite()])
 
-    if True: #Standard test run
+    if True:  # Standard test run
         r = unittest.TextTestRunner(failfast=False)
         ret = r.run(suites)
         assert ret.wasSuccessful()
-    else: #Cluster test run
+    else:  # Cluster test run
         from pysnptools.util.mapreduce1.distributabletest import DistributableTest
 
-        runner = HPC(10, 'RR1-N13-09-H44',r'\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\Redmond',
-                     remote_python_parent=r"\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\REDMOND\carlk\Source\carlk\july_7_14\tests\runs\2014-07-24_15_02_02_554725991686\pythonpath",
-                     update_remote_python_parent=True,
-                     priority="AboveNormal",mkl_num_threads=1)
+        runner = HPC(
+            10,
+            "RR1-N13-09-H44",
+            r"\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\Redmond",
+            remote_python_parent=r"\\msr-arrays\Scratch\msr-pool\Scratch_Storage4\REDMOND\carlk\Source\carlk\july_7_14\tests\runs\2014-07-24_15_02_02_554725991686\pythonpath",
+            update_remote_python_parent=True,
+            priority="AboveNormal",
+            mkl_num_threads=1,
+        )
         runner = Local()
-        #runner = LocalMultiProc(taskcount=20,mkl_num_threads=5)
-        #runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
-        #runner = Hadoop(100, mapmemory=8*1024, reducememory=8*1024, mkl_num_threads=1, queue="default")
-        distributable_test = DistributableTest(suites,"temp_test")
+        # runner = LocalMultiProc(taskcount=20,mkl_num_threads=5)
+        # runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
+        # runner = Hadoop(100, mapmemory=8*1024, reducememory=8*1024, mkl_num_threads=1, queue="default")
+        distributable_test = DistributableTest(suites, "temp_test")
         print(runner.run(distributable_test))
 
-
     logging.info("done with testing")
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/altset_list/Consecutive.py` & `fastlmm-0.6.8b1/fastlmm/association/altset_list/consecutive.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,70 @@
-from __future__ import absolute_import
-import numpy as SP
+import numpy as np
 import subprocess, sys, os.path
 from itertools import *
-from fastlmm.pyplink.snpset import *
 import math
-from six.moves import range
+
 
 class Consecutive(object):  # implements ISnpSetList
     """
-    The sets should be every consecutive set of SNPs within a 2cM window of each user 
+    The sets should be every consecutive set of SNPs within a 2cM window of each user
     (distance in cM is in the 3rd column of the bim file).  As for the name of the set,
     please make it <position-of-first-snp>@<position-of-middle-snp>@<position-of-last-snp>.
     For 'middle' please break a tie to the first SNP.
     """
 
-    def __init__(self, bimFileName,cMWindow):
+    def __init__(self, bimFileName, cMWindow):
         self.BimFileName = bimFileName
         self.CMWindow = cMWindow
 
     def addbed(self, bed):
-        return ConsecutivePlusBed(self,bed)
+        return _ConsecutivePlusBed(self, bed)
 
     def copyinputs(self, copier):
         copier.input(self.BimFileName)
 
-    #would be nicer if these used generic pretty printer
+    # would be nicer if these used generic pretty printer
     def __repr__(self):
-        return "Consecutive(bimFileName={0},bimFileName={1})".format(self.BimFileName,self.CMWindow)
+        return "Consecutive(bimFileName={0},bimFileName={1})".format(
+            self.BimFileName, self.CMWindow
+        )
 
 
-        
-class ConsecutivePlusBed(object): # implements ISnpSetListPlusBed
+class _ConsecutivePlusBed(object):  # implements ISnpSetListPlusBed
     def __init__(self, spec, bed):
         self.spec = spec
         self.bed = bed
         import pandas as pd
-        bimfields = pd.read_csv(self.spec.BimFileName,delimiter = '\s',usecols = (0,1,2,3),header=None,index_col=False,engine='python')
+
+        bimfields = pd.read_csv(
+            self.spec.BimFileName,
+            delimiter="\t",
+            usecols=(0, 1, 2, 3),
+            header=None,
+            index_col=False,
+        )
         self.chrom = bimfields[0]
-        self.rs = bimfields[1]
+        self.sid = bimfields[1]
         self.cm = bimfields[2]
 
-
     def __iter__(self):
-        startIndex=-1
-        endIndex=0 #one too far
-        while(True):
-            startIndex+=1
-            if startIndex >= len(self.rs):
+        startIndex = -1
+        endIndex = 0  # one too far
+        while True:
+            startIndex += 1
+            if startIndex >= len(self.sid):
                 return
-            while endIndex < len(self.rs) and self.chrom[startIndex] == self.chrom[endIndex] and  self.cm[endIndex] - self.cm[startIndex] <= self.spec.CMWindow:
-                endIndex+=1
-            lastIndex = endIndex - 1;
-            midIndex = math.floor((startIndex+lastIndex)/2.0)
-            name = "{0}@{1}@{2}".format(startIndex,midIndex,lastIndex)
+            while (
+                endIndex < len(self.sid)
+                and self.chrom[startIndex] == self.chrom[endIndex]
+                and self.cm[endIndex] - self.cm[startIndex] <= self.spec.CMWindow
+            ):
+                endIndex += 1
+            lastIndex = endIndex - 1
+            midIndex = math.floor((startIndex + lastIndex) / 2.0)
+            name = "{0}@{1}@{2}".format(startIndex, midIndex, lastIndex)
 
-            snpList=self.rs[list(range(startIndex,endIndex))]
-            yield SnpAndSetNamePlusBed(name,snpList,self.bed)                
+            snpList = self.sid[list(range(startIndex, endIndex))]
+            yield _SnpAndSetNamePlusBed(name, snpList, self.bed)
 
     def __len__(self):
-        return len(self.rs)
-
-
-
+        return len(self.sid)
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/altset_list/MinMaxSetSize.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/MinMaxSetSize.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,101 +1,112 @@
-from __future__ import absolute_import
-import numpy as SP
+import numpy as np
 import subprocess, sys, os.path
 from itertools import *
 from fastlmm.pyplink.snpset import *
 import logging
-import six
+
 
 class SnpAndSetNameCollection(object):  # implements ISnpSetList
-    '''
+    """
     Specifies a list of snp sets via a file that has columns 'snp' and 'group'.
     See the Bed class's 'read' method of examples of its use.
     See __init__.py for specification of interface it implements.
-    '''
+    """
+
     def __init__(self, filename):
         self.filename = filename
         logging.info("Reading {0}".format(filename))
         import pandas as pd
-        snp_and_setname_sequence = pd.read_csv(filename,delimiter = '\s',index_col=False,engine='python')
+
+        snp_and_setname_sequence = pd.read_csv(
+            filename, delimiter="\s", index_col=False, engine="python"
+        )
 
         from collections import defaultdict
+
         setname_to_snp_list = defaultdict(list)
-        for snp,gene in snp_and_setname_sequence.itertuples(index=False):
+        for snp, gene in snp_and_setname_sequence.itertuples(index=False):
             setname_to_snp_list[gene].append(snp)
-        self.bigToSmall = sorted(setname_to_snp_list.items(), key = lambda gene_snp_list:-len(gene_snp_list[1]))
+        self.bigToSmall = sorted(
+            setname_to_snp_list.items(),
+            key=lambda gene_snp_list: -len(gene_snp_list[1]),
+        )
 
     def addbed(self, bed):
-        return SnpAndSetNameCollectionPlusBed(self,bed)
+        return SnpAndSetNameCollectionPlusBed(self, bed)
 
     def copyinputs(self, copier):
         copier.input(self.filename)
 
-    #would be nicer if these used generic pretty printer
+    # would be nicer if these used generic pretty printer
     def __repr__(self):
         return "SnpAndSetNameCollection(filename={0})".format(self.filename)
 
     def __iter__(self):
-        for gene,snp_list in self.bigToSmall:
-            yield gene,snp_list
+        for gene, snp_list in self.bigToSmall:
+            yield gene, snp_list
 
 
 class GenomeSplitCollection(object):  # implements ISnpSetList
-    '''
+    """
     Specifies a list of snp sets by splitting the genome into windows of fixed size.
-    '''
-    def __init__(self, bed, windowsize,idist): # implements ISnpSetListPlusBed
-        '''
+    """
+
+    def __init__(self, bed, windowsize, idist):  # implements ISnpSetListPlusBed
+        """
         Input:
         bed         : bed object
         windowsize  : size of the window
         idist       : index in pos array that the exclusion is based on.
                   (1=genetic distance, 2=basepair distance)
-        '''
+        """
         self.bed = bed
         self.snp_list = []
-        chrom = bed.pos[:,0]
-        dist = bed.pos[:,idist]
+        chrom = bed.pos[:, 0]
+        dist = bed.pos[:, idist]
 
         # divide into blocks
-        chromUnique = SP.unique(chrom)
-        blockId=0
+        chromUnique = np.unique(chrom)
+        blockId = 0
         for chromId in chromUnique:
-            chromIdx = chromId==chrom
+            chromIdx = chromId == chrom
             distStart = dist[chromIdx].min()
             distMax = dist[chromIdx].max()
 
-            while distStart<distMax:
+            while distStart < distMax:
                 distStop = distStart + windowsize
-                idxBlock = SP.logical_and(chromIdx,SP.logical_and(distStart<=dist,dist<distStop))
-                self.snp_list.append(('block%d'%blockId,bed.rs[idxBlock]))
+                idxBlock = np.logical_and(
+                    chromIdx, np.logical_and(distStart <= dist, dist < distStop)
+                )
+                self.snp_list.append(("block%d" % blockId, bed.rs[idxBlock]))
                 blockId += 1
                 distStart = distStop
 
-       
-
     def __len__(self):
         return len(self.snp_list)
 
-
     def __iter__(self):
         for block, snp_list in self.snp_list:
-            if len(set(snp_list)) != len(snp_list) : raise Exception("Some snps are listed more than once.")
-            yield SnpAndSetNamePlusBed(block,snp_list,self.bed)
+            if len(set(snp_list)) != len(snp_list):
+                raise Exception("Some snps are listed more than once.")
+            yield SnpAndSetNamePlusBed(block, snp_list, self.bed)
 
 
-
-class SnpAndSetNameCollectionPlusBed(object): # implements ISnpSetListPlusBed
-    '''
+class SnpAndSetNameCollectionPlusBed(object):  # implements ISnpSetListPlusBed
+    """
     The SnpAndSetNameCollection with the addition of BED information.
-    '''
+    """
+
     def __init__(self, spec, bed):
         self.spec = spec
         self.bed = bed
 
     def __len__(self):
         return len(self.spec.bigToSmall)
 
     def __iter__(self):
         for gene, snp_list in self.spec.bigToSmall:
-            if len(set(snp_list)) != len(snp_list) : raise Exception("Some snps in gene {0} are listed more than once".format(gene))
-            yield SnpAndSetNamePlusBed(gene,snp_list,self.bed)
+            if len(set(snp_list)) != len(snp_list):
+                raise Exception(
+                    "Some snps in gene {0} are listed more than once".format(gene)
+                )
+            yield SnpAndSetNamePlusBed(gene, snp_list, self.bed)
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/altset_list/Subset.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/Subset.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/altset_list/__init__.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''
+"""
 a altset_list is a list of snpsets
 
 
 A altset_list is defined with two classes that implement these two interfaces: ISnpSetList and ISnpSetListPlusBed.
 Note: Python doesn't know enforce interfaces.
 
 interface ISnpSetList
@@ -12,14 +12,14 @@
 interface ISnpSetListPlusBed:
     def __len__(self):
         return # number of snpsets in this list
 
     def __iter__(self):
         return # a sequence of ISnpSetPlusBed's
 
-'''
-from __future__ import absolute_import
+"""
+
 from fastlmm.pyplink.snpset import *
 from .SnpAndSetNameCollection import *
 from .Subset import *
 from .MinMaxSetSize import *
 from .Consecutive import *
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/plink.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/plink.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-from __future__ import absolute_import
-import pdb
 import os
-import numpy as SP
+import numpy as np
 from .snpset import *
 import logging
-from six.moves import range
 
 
 def readPED(basefilename, delimiter=" ", missing="0", standardize=True, pheno=None):
     """
     read [basefilename].ped and [basefilename].map
     optionally standardize the SNPs and mean impute missing SNPs
     --------------------------------------------------------------------------
@@ -25,35 +22,35 @@
     'pos'    : [S*3] array of positions [chromosome, genetic dist, basepair dist],
     'snps'   : [N*S] array of snps-data,
     'iid'    : [N*2] array of family IDs and individual IDs
     --------------------------------------------------------------------------
     """
     pedfile = basefilename + ".ped"
     mapfile = basefilename + ".map"
-    map = SP.loadtxt(mapfile, dtype="str", comments=None)
+    map = np.loadtxt(mapfile, dtype="str", comments=None)
 
     rs = map[:, 1]
-    pos = SP.array(map[:, (0, 2, 3)], dtype="float")
+    pos = np.array(map[:, (0, 2, 3)], dtype="float")
     map = None
 
-    ped = SP.loadtxt(pedfile, dtype="str", comments=None)
+    ped = np.loadtxt(pedfile, dtype="str", comments=None)
     iid = ped[:, 0:2]
     snpsstr = ped[:, 6::]
     inan = snpsstr == missing
-    snps = SP.zeros((snpsstr.shape[0], snpsstr.shape[1] // 2))
+    snps = np.zeros((snpsstr.shape[0], snpsstr.shape[1] // 2))
     if standardize:
         for i in range(snpsstr.shape[1] // 2):
             snps[inan[:, 2 * i], i] = 0
             vals = snpsstr[~inan[:, 2 * i], 2 * i : 2 * (i + 1)]
             snps[~inan[:, 2 * i], i] += (vals == vals[0, 0]).sum(1)
             snps[~inan[:, 2 * i], i] -= snps[~inan[:, 2 * i], i].mean()
             snps[~inan[:, 2 * i], i] /= snps[~inan[:, 2 * i], i].std()
     else:
         for i in range(snpsstr.shape[1] / 2):
-            snps[inan[:, 2 * i], i] = SP.nan
+            snps[inan[:, 2 * i], i] = np.nan
             vals = snpsstr[~inan[:, 2 * i], 2 * i : 2 * (i + 1)]
             snps[~inan[:, 2 * i], i] += (vals == vals[0, 0]).sum(1)
     if pheno is not None:
         # TODO: sort and filter SNPs according to pheno
         pass
     ret = {"rs": rs, "pos": pos, "snps": snps, "iid": iid}
     return ret
@@ -77,34 +74,34 @@
     'pos'    : [S*3] array of positions [chromosome, genetic dist, basepair dist],
     'snps'   : [N*S] array of snps-data,
     'iid'    : [N*2] array of family IDs and individual IDs
     --------------------------------------------------------------------------
     """
     rawfile = basefilename + ".raw"
     # mapfile = basefilename+".map"
-    # map = SP.loadtxt(mapfile,dtype = 'str',comments=None)
+    # map = np.loadtxt(mapfile,dtype = 'str',comments=None)
 
     # rs = map[:,1]
-    # pos = SP.array(map[:,(0,2,3)],dtype = 'float')
+    # pos = np.array(map[:,(0,2,3)],dtype = 'float')
     # map = None
-    raw = SP.loadtxt(rawfile, dtype="str", comments=None)
+    raw = np.loadtxt(rawfile, dtype="str", comments=None)
     iid = raw[:, 0:2]
     snpsstr = raw[:, 6::]
     inan = snpsstr == missing
-    snps = SP.zeros((snpsstr.shape[0], snpsstr.shape[1] / 2))
+    snps = np.zeros((snpsstr.shape[0], snpsstr.shape[1] / 2))
     if standardize:
         for i in range(snpsstr.shape[1] / 2):
             raw[inan[:, 2 * i], i] = 0
             vals = snpsstr[~inan[:, 2 * i], 2 * i : 2 * (i + 1)]
             snps[~inan[:, 2 * i], i] += (vals == vals[0, 0]).sum(1)
             snps[~inan[:, 2 * i], i] -= snps[~inan[:, 2 * i], i].mean()
             snps[~inan[:, 2 * i], i] /= snps[~inan[:, 2 * i], i].std()
     else:
         for i in range(snpsstr.shape[1] / 2):
-            snps[inan[:, 2 * i], i] = SP.nan
+            snps[inan[:, 2 * i], i] = np.nan
             vals = snpsstr[~inan[:, 2 * i], 2 * i : 2 * (i + 1)]
             snps[~inan[:, 2 * i], i] += (vals == vals[0, 0]).sum(1)
     if pheno is not None:
         # TODO: sort and filter SNPs according to pheno
         pass
     ret = {"rs": rs, "pos": pos, "snps": snps, "iid": iid}
     return ret
@@ -137,15 +134,15 @@
 
     bed = sr.Bed(basefilename)
     return bed.read(snp_set, order=order)
 
 
 def nSnpFromBim(basefilename):
     bim = basefilename + ".bim"
-    bimx = SP.loadtxt(bim, dtype="str", usecols=(0, 1, 2, 3), comments=None)
+    bimx = np.loadtxt(bim, dtype="str", usecols=(0, 1, 2, 3), comments=None)
     S = bimx.shape[0]
     return S
 
 
 def findIndex(idsSep, bedidsSep):
     sids = set()
     for i in range(idsSep.shape[0]):
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/setup.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/setup.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/snpreader/Bed.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Bed.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/snpreader/Dat.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Dat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from __future__ import absolute_import
-import numpy as SP
+import numpy as np
 import subprocess, sys, os.path
 from itertools import *
 from fastlmm.pyplink.snpset import *
 from fastlmm.pyplink.altset_list import *
 import pandas as pd
 import logging
-from six.moves import range
 
 
 class Dat(object):
     """
     This is a class that reads into memory from DAT/FAM/MAP files.
     """
 
@@ -46,29 +44,29 @@
             return
         self._ran_once = True
 
         famfile, mapfile = self.names_of_other_files()
 
         #!!similar code in BED reader
         logging.info("Loading fam file {0}".format(famfile))
-        self._original_iids = SP.loadtxt(
+        self._original_iids = np.loadtxt(
             famfile, dtype="str", usecols=(0, 1), comments=None
         )
 
         #!!similar code in BED reader
         logging.info("Loading map file {0}".format(mapfile))
         self.bimfields = pd.read_csv(
             mapfile,
             delimiter="\s",
             usecols=(0, 1, 2, 3),
             header=None,
             index_col=False,
             engine="python",
         )
-        self.rs = SP.array(self.bimfields[1].tolist(), dtype="str")
+        self.rs = np.array(self.bimfields[1].tolist(), dtype="str")
         self.pos = self.bimfields[[0, 2, 3]].values
         self._snp_to_index = {}
         logging.info("indexing snps")
         for i in range(self.snp_count):
             snp = self.rs[i]
             if snp in self._snp_to_index:
                 raise Exception(
@@ -76,15 +74,15 @@
                 )
             self._snp_to_index[snp] = i
 
         #!!could change to just create/find an index to the file position of each row. Instead, reading all into memory
         datfields = pd.read_csv(
             self.dat_filename, delimiter="\s", header=None, index_col=False
         )
-        if not sp.array_equal(sp.array(datfields[0], dtype="string"), self.rs):
+        if not np.array_equal(np.array(datfields[0], dtype="string"), self.rs):
             raise Exception(
                 "Expect snp list in map file to exactly match snp list in dat file"
             )
         self.start_column = 3
         if len(self._original_iids) != datfields.shape[1] - self.start_column:
             raise Exception("Expect # iids in fam file to match dat file")
         self.datfields = datfields.T
@@ -104,15 +102,15 @@
 
     @property
     def snp_count(self):
         self.run_once()
         return len(self.bimfields)
 
     def read(
-        self, snp_set=AllSnps(), order="F", dtype=SP.float64, force_python_only=False
+        self, snp_set=AllSnps(), order="F", dtype=np.float64, force_python_only=False
     ):
         """
         Input: a snp_set. Choices include
             AllSnps() [the default],
             PositionRange(snpIndex,nSNPs)
             SnpAndSetName(groupname,snplist),
 
@@ -172,29 +170,29 @@
             snp_count_in,
             snp_count_out,
             snp_index_out,
         )
 
     @staticmethod
     def read_with_specification(
-        snpset_withdat, order="F", dtype=SP.float64, force_python_only=False
+        snpset_withdat, order="F", dtype=np.float64, force_python_only=False
     ):
         dat = snpset_withdat.bed  #!!bed is a misnomer
         (
             iid_count_in,
             iid_count_out,
             iid_index_out,
             snp_count_in,
             snp_count_out,
             snp_index_out,
         ) = dat.counts_and_indexes(snpset_withdat)
 
-        SNPs = SP.zeros((iid_count_out, snp_count_out), order=order, dtype=dtype)
+        SNPs = np.zeros((iid_count_out, snp_count_out), order=order, dtype=dtype)
         for SNPsIndex, bimIndex in enumerate(snp_index_out):
-            row = sp.array(dat.datfields[bimIndex])[dat.start_column :,]
+            row = np.array(dat.datfields[bimIndex])[dat.start_column :,]
             SNPs[:, SNPsIndex] = row[iid_index_out]
 
         ret = {
             "rs": dat.rs[snp_index_out],
             "pos": dat.pos[snp_index_out, :],
             "snps": SNPs,
             "iid": dat.original_iids[iid_index_out, :],
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/snpreader/Hdf5.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-from __future__ import absolute_import
-from six.moves import range
-
 try:
     import h5py
 except:
     pass
 
 import logging
-import scipy as sp
+import numpy as np
 from fastlmm.pyplink.snpset import *
 from fastlmm.pyplink.altset_list import *
 
 #!!document the format
 
 
 class Hdf5(object):
@@ -41,17 +38,17 @@
         except IOError as e:
             raise IOError(
                 "Missing or unopenable file '{0}' -- Native error message: {1}".format(
                     self.filename, e
                 )
             )
 
-        self._original_iids = sp.array(sp.array(self.h5["iid"]), dtype=str)
-        self.rs = sp.array(sp.array(self.h5["rs"]), dtype="str")
-        self.pos = sp.array(self.h5["pos"])
+        self._original_iids = np.array(np.array(self.h5["iid"]), dtype=str)
+        self.rs = np.array(np.array(self.h5["rs"]), dtype="str")
+        self.pos = np.array(self.h5["pos"])
 
         ## similar code in bed
         self._snp_to_index = {}
         logging.info("indexing snps")
         for i, snp in enumerate(self.rs):
             if snp in self._snp_to_index:
                 raise Exception(
@@ -88,15 +85,15 @@
     @property
     def original_iids(self):
         self.run_once()
         return self._original_iids
 
     # same code is in Bed. Could this be moved to an abstract class?
     def read(
-        self, snp_set=AllSnps(), order="F", dtype=SP.float64, force_python_only=False
+        self, snp_set=AllSnps(), order="F", dtype=np.float64, force_python_only=False
     ):
         self.run_once()
         snpset_withbed = snp_set.addbed(self)
         return self.read_with_specification(
             snpset_withbed,
             order=order,
             dtype=dtype,
@@ -115,15 +112,15 @@
 
     def __del__(self):
         if (
             self.h5 is not None
         ):  # we need to test this because Python doesn't guarantee that __init__ was fully run
             self.h5.close()
 
-    def read_direct(self, snps, selection=sp.s_[:, :]):
+    def read_direct(self, snps, selection=np.s_[:, :]):
         if self.is_snp_major:
             selection = tuple(reversed(selection))
 
         if snps.flags["F_CONTIGUOUS"]:
             self.snpsInFile.read_direct(snps.T, selection)
         else:
             self.snpsInFile.read_direct(snps, selection)
@@ -134,49 +131,49 @@
         matches_order = self.is_snp_major == (
             order == "F"
         )  # similar code else where -- make a method
         opposite_order = (
             "C" if order == "F" else "F"
         )  # similar code else where -- make a method
         if matches_order:
-            return sp.empty([N_original, blocksize], dtype=dtype, order=order)
+            return np.empty([N_original, blocksize], dtype=dtype, order=order)
         else:
-            return sp.empty([N_original, blocksize], dtype=dtype, order=opposite_order)
+            return np.empty([N_original, blocksize], dtype=dtype, order=opposite_order)
 
     def read_with_specification(
         self,
         snpset_with_snpreader,
         order="F",
-        dtype=SP.float64,
+        dtype=np.float64,
         force_python_only=False,
     ):
         self.run_once()
 
         order = order.upper()
         opposite_order = "C" if order == "F" else "F"
 
-        snp_index_list = sp.array(
+        snp_index_list = np.array(
             list(snpset_with_snpreader)
         )  # Is there a way to create an array from an iterator without putting it through a list first?
         S = len(snp_index_list)
         S_original = self.snp_count
         N_original = len(self.original_iids)
 
         # Check if snps and iids indexes are in order and in range
         snps_are_sorted = Hdf5.is_sorted_without_repeats(snp_index_list)
         if hasattr(self, "_ind_used"):
             iid_index_list = self._ind_used
             iid_is_sorted = Hdf5.is_sorted_without_repeats(iid_index_list)
         else:
-            iid_index_list = sp.arange(N_original)
+            iid_index_list = np.arange(N_original)
             iid_is_sorted = True
 
         N = len(iid_index_list)
 
-        SNPs = sp.empty([N, S], dtype=dtype, order=order)
+        SNPs = np.empty([N, S], dtype=dtype, order=order)
 
         matches_order = self.is_snp_major == (order == "F")
         is_simple = (
             not force_python_only
             and iid_is_sorted
             and snps_are_sorted
             and matches_order
@@ -184,47 +181,47 @@
 
         # case 1 - all snps & all ids requested
         if is_simple and S == S_original and N == N_original:
             self.read_direct(SNPs)
 
         # case 2 - some snps and all ids
         elif is_simple and N == N_original:
-            self.read_direct(SNPs, sp.s_[:, snp_index_list])
+            self.read_direct(SNPs, np.s_[:, snp_index_list])
 
         # case 3 all snps and some ids
         elif is_simple and S == S_original:
-            self.read_direct(SNPs, sp.s_[iid_index_list, :])
+            self.read_direct(SNPs, np.s_[iid_index_list, :])
 
         # case 4 some snps and some ids -- use blocks
         else:
             blocksize = min(self.blocksize, S)
             block = self.create_block(blocksize, dtype, order)
 
             if not snps_are_sorted:
-                snp_index_index_list = sp.argsort(snp_index_list)
+                snp_index_index_list = np.argsort(snp_index_list)
                 snp_index_list_sorted = snp_index_list[snp_index_index_list]
             else:
-                snp_index_index_list = sp.arange(S)
+                snp_index_index_list = np.arange(S)
                 snp_index_list_sorted = snp_index_list
 
             for start in range(0, S, blocksize):
                 # print start
                 end = min(start + blocksize, S)
                 if (
                     end - start < blocksize
                 ):  # On the last loop, the buffer might be too big, so make it smaller
                     block = self.create_block(end - start, dtype, order)
                 snp_index_list_forblock = snp_index_list_sorted[start:end]
                 snp_index_index_list_forblock = snp_index_index_list[start:end]
-                self.read_direct(block, sp.s_[:, snp_index_list_forblock])
+                self.read_direct(block, np.s_[:, snp_index_list_forblock])
                 SNPs[:, snp_index_index_list_forblock] = block[iid_index_list, :]
 
         rs = self.rs[snp_index_list]
         pos = self.pos[snp_index_list, :]
-        iids = sp.array(
+        iids = np.array(
             self.original_iids[iid_index_list], dtype="str"
         )  # Need to make another copy of to stop it from being converted to a list of 1-d string arrays
 
         has_right_order = (order == "C" and SNPs.flags["C_CONTIGUOUS"]) or (
             order == "F" and SNPs.flags["F_CONTIGUOUS"]
         )
         # if SNPs.shape == (1, 1):
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/snpset/AllSnps.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpIndexList.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,51 @@
-from __future__ import absolute_import
-import numpy as SP
+import numpy as np
 import subprocess, sys, os.path
-from six.moves import range
 
 
-class AllSnps(object): # implements ISnpSet
-    '''
-    When given to a bed reader, tells it to read all snps. See the Bed class's 'read' method of examples of its use.
-    See __init__.py for specification of interface it implements.
-    '''
+class SnpIndexList(object):  # implements ISnpSet
+    """
+    When given to a bed reader, tells it to read the snps at the indexes given
+     See the Bed class's 'read' method of examples of its use.
+     See __init__.py for specification of interface it implements.
+    """
+
+    def __init__(self, list):
+        """
+        list of snp indexes to include
+        """
+        self.list = list
+
     def addbed(self, bed):
-        return AllSnpsPlusBed(bed)
+        return SnpIndexListPlusBed(self, bed)
 
-class AllSnpsPlusBed(object): # implements ISnpSetPlusBed
 
-    def __init__(self,bed):
+class SnpIndexListPlusBed(object):  # implements ISnpSetPlusBed
+    def __init__(self, spec, bed):
+        self.spec = spec
         self.bed = bed
 
-    def __len__(self):
-        return self.bed.snp_count
+    def __str__(self):
+        return "SnpIndex(...)"
 
     def __iter__(self):
-        for bimindex in range(self.bed.snp_count):
+        for bimindex in self.spec.list:
             yield bimindex
 
-    def __str__(self):
-        return "AllSnps"
+    def __len__(self):
+        return len(self.spec.list)
 
-    def read(self): 
+    def read(self):  #!!why don't all the interface implementers have this method?
         return self.bed.read_with_specification(self)
 
     @property
     def pos(self):
         """
         Returns:
             pos:    position of the SNPs in the specification
         """
         return self.bed.pos[self.to_index]
 
     @property
     def to_index(self):
         iter = self.__iter__()
-        return [i for i in iter]
+        return [i for i in iter]
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/snpset/PositionRange.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/PositionRange.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,58 @@
-from __future__ import absolute_import
-import numpy as SP
+import numpy as np
 import subprocess, sys, os.path
-from six.moves import range
 
-class PositionRange(object): # implements ISnpSet
-    '''
+
+class PositionRange(object):  # implements ISnpSet
+    """
     When given to a bed reader, tells it to read 'nSNPs' starting at index position 'start'.
      See the Bed class's 'read' method of examples of its use.
      See __init__.py for specification of interface it implements.
-    '''
+    """
 
-    def __init__(self, start=0,nSnps=SP.inf):
-        '''
+    def __init__(self, start=0, nSnps=np.inf):
+        """
         start           : index of the first SNP to be loaded from the .bed-file
                           (default 0)
-        nSNPs           : load nSNPs from the .bed file (default SP.inf, meaning all)
-        '''
+        nSNPs           : load nSNPs from the .bed file (default np.inf, meaning all)
+        """
         self.start = start
         self.nSNPs = nSnps
 
     def addbed(self, bed):
-        return PositionRangePlusBed(self,bed)
+        return PositionRangePlusBed(self, bed)
+
 
-class PositionRangePlusBed(object): # implements ISnpSetPlusBed
+class PositionRangePlusBed(object):  # implements ISnpSetPlusBed
     def __init__(self, spec, bed):
         self.spec = spec
         self.bed = bed
 
     def __str__(self):
-        return "PositionRange(start={0},nSNPs={1})".format(self.spec.start,self.spec.nSNPs)
+        return "PositionRange(start={0},nSNPs={1})".format(
+            self.spec.start, self.spec.nSNPs
+        )
 
     def __iter__(self):
-        for bimindex in range(self.spec.start,self.spec.start+len(self)):  #note that 'self.spec.start+len(self)' is the 'stop', not the 'count'
+        for bimindex in range(
+            self.spec.start, self.spec.start + len(self)
+        ):  # note that 'self.spec.start+len(self)' is the 'stop', not the 'count'
             yield bimindex
 
     def __len__(self):
-        return min(self.bed.snp_count-self.spec.start,self.spec.nSNPs)
+        return min(self.bed.snp_count - self.spec.start, self.spec.nSNPs)
 
-    def read(self): #!!why don't all the interface implementers have this method?
+    def read(self):  #!!why don't all the interface implementers have this method?
         return self.bed.read_with_specification(self)
 
     @property
     def pos(self):
         """
         Returns:
             pos:    position of the SNPs in the specification
         """
         return self.bed.pos[self.to_index]
 
     @property
     def to_index(self):
         iter = self.__iter__()
-        return [i for i in iter]
+        return [i for i in iter]
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/snpset/RandomSnpSet.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/RandomSnpSet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,61 @@
-from __future__ import absolute_import
-import numpy as sp
+import numpy as np
 import subprocess, sys, os.path
 import fastlmm.util.util as utilx
 
 
-class RandomSnpSet(object): # implements ISnpSet
-    '''
-     See the Bed class's 'read' method of examples of its use.
-     See __init__.py for specification of interface it implements.
-     '''
-    def __init__(self, numsnps, randomseed):        
-        self.numsnps=numsnps
-        self.randomseed=randomseed
+class RandomSnpSet(object):  # implements ISnpSet
+    """
+    See the Bed class's 'read' method of examples of its use.
+    See __init__.py for specification of interface it implements.
+    """
+
+    def __init__(self, numsnps, randomseed):
+        self.numsnps = numsnps
+        self.randomseed = randomseed
 
     def addbed(self, bed):
-        return RandomSnpSetPlusBed(self.numsnps,self.randomseed,bed)
+        return RandomSnpSetPlusBed(self.numsnps, self.randomseed, bed)
 
-class RandomSnpSetPlusBed(object): # implements ISnpSetPlusBed
-    '''
+
+class RandomSnpSetPlusBed(object):  # implements ISnpSetPlusBed
+    """
     One random set of snps.
-    '''
+    """
+
     def __init__(self, numsnps, randomseed, bed):
-        self.numsnps=numsnps
-        self.randomseed=randomseed
+        self.numsnps = numsnps
+        self.randomseed = randomseed
         self.bed = bed
-        #very inefficient extraction of a few random SNP indexes:        
-        self.snpindlist = utilx.generate_permutation(sp.arange(0,bed.snp_count),randomseed)[0:numsnps]
-        self.snpindlist.sort()        
+        # very inefficient extraction of a few random SNP indexes:
+        self.snpindlist = utilx.generate_permutation(
+            np.arange(0, bed.snp_count), randomseed
+        )[0:numsnps]
+        self.snpindlist.sort()
 
     def __str__(self):
-        return "RandomSnpSet(numsnps={0},randomseed={1})".format(self.numsnps,self.randomseed)
+        return "RandomSnpSet(numsnps={0},randomseed={1})".format(
+            self.numsnps, self.randomseed
+        )
 
     def __len__(self):
         return self.numsnps
 
-    def __iter__(self):       
-        for i in self.snpindlist:        
+    def __iter__(self):
+        for i in self.snpindlist:
             yield i
 
-    def read(self): #!!why don't all the interface implementers have this method?
+    def read(self):  #!!why don't all the interface implementers have this method?
         return self.bed.read_with_specification(self)
 
     @property
     def pos(self):
         """
         Returns:
             pos:    position of the SNPs in the specification
         """
         return self.bed.pos[self.to_index]
 
     @property
     def to_index(self):
         iter = self.__iter__()
-        return [i for i in iter]
+        return [i for i in iter]
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/snpset/SnpSetAndName.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpSetAndName.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-from __future__ import absolute_import
-import numpy as SP
+import numpy as np
 import subprocess, sys, os.path
 
 
-class SnpAndSetName(object): # implements ISnpSet
-    '''
-     See the Bed class's 'read' method of examples of its use.
-     See __init__.py for specification of interface it implements.
-     '''
+class SnpAndSetName(object):  # implements ISnpSet
+    """
+    See the Bed class's 'read' method of examples of its use.
+    See __init__.py for specification of interface it implements.
+    """
+
     def __init__(self, setname, snplist):
         self.name = setname
         self.snplist = snplist
 
     def addbed(self, bed):
-        return SnpAndSetNamePlusBed(self.name,self.snplist,bed)
+        return SnpAndSetNamePlusBed(self.name, self.snplist, bed)
+
 
-class SnpAndSetNamePlusBed(object): # implements ISnpSetPlusBed
-    '''
+class SnpAndSetNamePlusBed(object):  # implements ISnpSetPlusBed
+    """
     A single set of snps.
-    '''
+    """
+
     def __init__(self, setname, snplist, bed):
         self.name = setname
-        self.snplist = [val for val in snplist if val in bed.snp_to_index] #use the intersection
+        self.snplist = [
+            val for val in snplist if val in bed.snp_to_index
+        ]  # use the intersection
         self.bed = bed
 
     def __str__(self):
         return self.name
 
     def __len__(self):
         return len(self.snplist)
 
     def __iter__(self):
         for snp in self.snplist:
             index = self.bed.snp_to_index[snp]
             yield index
 
-    def read(self): #!!why don't all the interface implementers have this method?
+    def read(self):  #!!why don't all the interface implementers have this method?
         return self.bed.read_with_specification(self)
 
     @property
     def pos(self):
         """
         Returns:
             pos:    position of the SNPs in the specification
         """
         return self.bed.pos[self.to_index]
 
     @property
     def to_index(self):
         iter = self.__iter__()
-        return [i for i in iter]
+        return [i for i in iter]
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/snpset/SnpsFromFile.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpsFromFile.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,38 @@
-from __future__ import absolute_import
-import numpy as SP
+import numpy as np
 import subprocess, sys, os.path
 
-class SnpsFromFile(object): # implements ISnpSet
-    '''
-     See the Bed class's 'read' method of examples of its use.
-     See __init__.py for specification of interface it implements.
-     '''
+
+class SnpsFromFile(object):  # implements ISnpSet
+    """
+    See the Bed class's 'read' method of examples of its use.
+    See __init__.py for specification of interface it implements.
+    """
+
     def __init__(self, filename):
         self.filename = filename
 
     def addbed(self, bed):
         return SnpsFromFilePlusBed(self.filename, bed)
 
-class SnpsFromFilePlusBed(object): # implements ISnpSetPlusBed
+
+class SnpsFromFilePlusBed(object):  # implements ISnpSetPlusBed
     def __init__(self, filename, bed):
         self.filename = filename
         snplist0 = ReadTokens(filename)
         bed.run_once()
-        self.snplist = [val for val in snplist0 if val in bed.snp_to_index] #use the intersection        
-        if len(snplist0) != len(self.snplist): raise Exception("The file '{0}' contains SNPs not in bed '{1}'".format(filename,bed.basefilename))
+        self.snplist = [
+            val for val in snplist0 if val in bed.snp_to_index
+        ]  # use the intersection
+        if len(snplist0) != len(self.snplist):
+            raise Exception(
+                "The file '{0}' contains SNPs not in bed '{1}'".format(
+                    filename, bed.basefilename
+                )
+            )
         self.bed = bed
 
     def __str__(self):
         return self.filename
 
     def __len__(self):
         return len(self.snplist)
@@ -31,24 +40,27 @@
     def __iter__(self):
         for snp in self.snplist:
             index = self.bed.snp_to_index[snp]
             yield index
 
     def read(self):
         return self.bed.read_with_specification(self)
-    
+
     @property
     def pos(self):
         """
         Returns:
             pos:    position of the SNPs in the specification
         """
         return self.bed.pos[self.to_index]
 
     @property
     def to_index(self):
         iter = self.__iter__()
         return [i for i in iter]
 
+
 def ReadTokens(filename):
-    token_list = open(filename).read().split() # could be written to 'yield' the tokens one at a time
-    return token_list;
+    token_list = (
+        open(filename).read().split()
+    )  # could be written to 'yield' the tokens one at a time
+    return token_list
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/snpset/__init__.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-'''
+"""
+#!! fix comments
 snpset is a named set of snps.  See the Bed class's 'read' method of examples of their use.
 
 A snpset is defined with two classes that implement these two interfaces: ISnpSet and ISnpSetPlusBed.
 Note: Python doesn't enforce interfaces.
 
 interface ISnpSet
     def addbed(self, bed):
@@ -13,15 +14,13 @@
         return # number of snps in this set
 
     def __iter__(self):
         return # index number to position in BIM file
 
     def __str__(self):
         return # string of name of this set of snps
-'''
+"""
 
-from .AllSnps import *
-from .PositionRange import *
-from .SnpSetAndName import *
-from .SnpsFromFile import *
-from .SnpIndexList import *
-from .RandomSnpSet import *
+from .Lrt import *
+from .Cv import *
+from .Sc import *
+from . import LRT_up as lrt
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/test.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import numpy as np
-import scipy as sp
 import logging
 import doctest
 import sys
 
 import unittest
 import os.path
 import time
 
+
 # We do it this way instead of using doctest.DocTestSuite because doctest.DocTestSuite requires modules to be pickled, which python doesn't allow.
 # We need tests to be pickleable so that they can be run on a cluster.
 class TestDocStrings(unittest.TestCase):
 
     def test_bed(self):
         import fastlmm.pyplink.snpreader.Bed
+
         old_dir = os.getcwd()
         os.chdir(os.path.dirname(os.path.realpath(__file__)))
-        result = doctest.testmod(sys.modules['fastlmm.pyplink.snpreader.Bed'])
+        result = doctest.testmod(sys.modules["fastlmm.pyplink.snpreader.Bed"])
         os.chdir(old_dir)
         assert result.failed == 0, "failed doc test: " + __file__
 
 
-
 def getTestSuite():
     """
     set up composite test suite
     """
-    
+
     test_suite = unittest.TestSuite([])
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestDocStrings))
 
     return test_suite
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
 
     suites = getTestSuite()
     r = unittest.TextTestRunner(failfast=False)
     ret = r.run(suites)
     assert ret.wasSuccessful()
     print("done")
```

### Comparing `fastlmm-0.6.7/fastlmm/pyplink/vcfpy.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/vcfpy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,114 +1,122 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import sys
-import pdb
 import os
 import gzip
 import re
-import scipy as SP
-from six.moves import range
+import numpy as np
+
 writesmall = 0
 
 datadir = ""
 base = ""
-tbi = base+".tbi"
-basef=os.path.join(datadir,base)
+tbi = base + ".tbi"
+basef = os.path.join(datadir, base)
 basefsmall = "chr22.small.txt.gz"
-basefsmall = 'chr22.small.txt'
+basefsmall = "chr22.small.txt"
 baseftbi = basef + ".tbi"
 
 if writesmall:
-    file = gzip.GzipFile(basef, 'r')
-    #outfsmall = gzip.GzipFile(basefsmall,'w')
-    outfsmall = open(basefsmall,'w')
+    file = gzip.GzipFile(basef, "r")
+    # outfsmall = gzip.GzipFile(basefsmall,'w')
+    outfsmall = open(basefsmall, "w")
 else:
-    file = open(basefsmall,'r')
+    file = open(basefsmall, "r")
 line = file.readline()
 if writesmall:
     outfsmall.write(line)
-if line != '##fileformat=VCFv4.1\n':
-    print('wrong format')
+if line != "##fileformat=VCFv4.1\n":
+    print("wrong format")
 iline = 0
-header = ''
-while (line[0:2]=='##'):
-    header = header+line
+header = ""
+while line[0:2] == "##":
+    header = header + line
     line = file.readline()
     if writesmall:
         outfsmall.write(line)
-    iline+=1;
-if line[0:6] == '#CHROM':
-    fields = line[1::].strip().split('\t')
-    indID=fields[9::]
-    fields=fields[0:9]
+    iline += 1
+if line[0:6] == "#CHROM":
+    fields = line[1::].strip().split("\t")
+    indID = fields[9::]
+    fields = fields[0:9]
 
 
-famfile = open('test.fam','w')
+famfile = open("test.fam", "w")
 for id in indID:
-   outline = '0 ' + id + ' 0 0 0 -9\n'
-   famfile.write(outline)
+    outline = "0 " + id + " 0 0 0 -9\n"
+    famfile.write(outline)
 famfile.close()
 ninds = len(indID)
 
 line = file.readline()
 if writesmall:
     outfsmall.write(line)
 
-bedfile = open('test.bed','wb')
-bimfile = open('test.bim','w')
+bedfile = open("test.bed", "wb")
+bimfile = open("test.bim", "w")
 
-#init bedfile
-bedfile.write(b'l\x1b')#bed header
-bedfile.write(b'\x01')
-#genomap=[]
-#geno = []
+# init bedfile
+bedfile.write(b"l\x1b")  # bed header
+bedfile.write(b"\x01")
+# genomap=[]
+# geno = []
 iline = 0
 if writesmall:
-    maxline =100
+    maxline = 100
 else:
     maxline = 10000000
-while (iline < maxline ) and (line !=''):
-    vals = line.strip().split('\t')
-    if (vals[6]=='PASS'):
-        linebim = vals[0] + ' ' + vals[2] + ' 0 ' + vals[1] + ' ' + vals[3] + ' ' + vals[4] + '\n'
+while (iline < maxline) and (line != ""):
+    vals = line.strip().split("\t")
+    if vals[6] == "PASS":
+        linebim = (
+            vals[0]
+            + " "
+            + vals[2]
+            + " 0 "
+            + vals[1]
+            + " "
+            + vals[3]
+            + " "
+            + vals[4]
+            + "\n"
+        )
         bimfile.write(linebim)
-        #genomap.append(vals[0:9])
-        #geno.append(vals[9::])
+        # genomap.append(vals[0:9])
+        # geno.append(vals[9::])
 
-        #write bedfile entries
-        nbytes = SP.ceil(ninds/4.0)
+        # write bedfile entries
+        nbytes = np.ceil(ninds / 4.0)
         ndone = 0
-        for i in range(int(SP.ceil(ninds/4.0))):
-            num = min(4,ninds-ndone)
-            geno = vals[9+i*4:9+(i)*4+num]
+        for i in range(int(np.ceil(ninds / 4.0))):
+            num = min(4, ninds - ndone)
+            geno = vals[9 + i * 4 : 9 + (i) * 4 + num]
             byte = 0
-            #pdb.set_trace()
+            # pdb.set_trace()
             for j in range(num):
 
-                if geno[j][0:3]=='0|0':
-                    #byte += 0*(2**(2*j))
+                if geno[j][0:3] == "0|0":
+                    # byte += 0*(2**(2*j))
                     pass
-                elif geno[j][0:3]=='0|1' or geno[j][0:3]=='1|0':
-                    byte += 2*(2**(2*j))
-                elif geno[j][0:3]=='1|1':
-                    byte += 3*(2**(2*j))
+                elif geno[j][0:3] == "0|1" or geno[j][0:3] == "1|0":
+                    byte += 2 * (2 ** (2 * j))
+                elif geno[j][0:3] == "1|1":
+                    byte += 3 * (2 ** (2 * j))
                 else:
-                    #pdb.set_trace()
-                    byte += 1*(2**(2*j))
+                    # pdb.set_trace()
+                    byte += 1 * (2 ** (2 * j))
                 pass
 
-            bytestr = '%c'%byte
+            bytestr = "%c" % byte
             bedfile.write(bytestr)
-            ndone +=num
+            ndone += num
             pass
     line = file.readline()
     if writesmall:
         outfsmall.write(line)
-    iline+=1
+    iline += 1
 file.close()
 if writesmall:
     outfsmall.close()
 bimfile.close()
 bedfile.close()
 
-#filetbi = open(baseftbi,'r')
-#filetbigz = gzip.GzipFile(baseftbi,'r')
+# filetbi = open(baseftbi,'r')
+# filetbigz = gzip.GzipFile(baseftbi,'r')
```

### Comparing `fastlmm-0.6.7/fastlmm/util/NearBronze.py` & `fastlmm-0.6.8b1/fastlmm/util/NearBronze.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from __future__ import absolute_import
 import pandas as pd
 import logging
-import six
 
 
 class NearBronze:
     @staticmethod
     def Parse():
         import argparse
```

### Comparing `fastlmm-0.6.7/fastlmm/util/VertexCut.py` & `fastlmm-0.6.8b1/fastlmm/util/VertexCut.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''
+"""
 
 A class for finding a vertex cut. A vertex cut is a a set of nodes, ideally the smallest number, that when removed yields a disconnected graph.
 Apparently this is np-hard, so we settle for the following heuristic: iteratively remove the node that has the most edges until the graph is disconnected.
 
 
 Examples:
 
@@ -10,78 +10,82 @@
     #>>> VertexCut().work(sparse_input_sequence)
     #['a']
 
     >>> matrix = np.array([[3, 3, 1],[3, 3, 1],[1, 1, 3]])
     >>> VertexCut().work(matrix,2)
     [0]
 
-'''
-from __future__ import absolute_import
-from __future__ import print_function
+"""
+
 import numpy as np
-import scipy as sp
 from collections import defaultdict
 import logging
 import itertools
-import six
-from six.moves import zip
 
-class VertexCut(object):
 
+class VertexCut(object):
 
     def work(self, matrix, minvalue):
-        assert(len(matrix.shape) == 2 and matrix.shape[0] == matrix.shape[1])
+        assert len(matrix.shape) == 2 and matrix.shape[0] == matrix.shape[1]
 
         graph = self._load_graph_from_matrix(matrix, minvalue)
 
         node_list = []
         while self._piece_count(graph) < len(graph):
             logging.debug("len(graph)={0}".format(len(graph)))
             aMostConnectedNode = self._find_a_most_connected_node(graph)
-            #logging.debug("aMostConnectedNode={0}".format(aMostConnectedNode))
+            # logging.debug("aMostConnectedNode={0}".format(aMostConnectedNode))
             self._remove_node(graph, aMostConnectedNode)
-            #logging.debug("removed")
+            # logging.debug("removed")
             node_list.append(aMostConnectedNode)
             if len(node_list) % 10 == 0:
                 logging.info("# nodes removed is {0}".format(len(node_list)))
         return node_list
 
     def _load_graph_from_matrix(self, matrix, minvalue):
         where = np.where(matrix >= minvalue)
-        sparse_input_sequence = zip(where[0],where[1])
-        graph = self._load_graph(sparse_input_sequence,len(where[0]))
+        sparse_input_sequence = zip(where[0], where[1])
+        graph = self._load_graph(sparse_input_sequence, len(where[0]))
         return graph
 
-    def _load_graph(self, sparse_input_sequence,len_input_sequence):
+    def _load_graph(self, sparse_input_sequence, len_input_sequence):
         graph = defaultdict(list)
         i = -1
         for node1, node2 in sparse_input_sequence:
             i += 1
-            #don't need graph[node1] because singleton's don't need to be included in the graph
-            if node1 != node2 :
+            # don't need graph[node1] because singleton's don't need to be included in the graph
+            if node1 != node2:
                 if i % 100000 == 0:
-                    logging.info("added {0} of {1} ({2}%)".format(i, len_input_sequence, float(i)/len_input_sequence*100.0))
+                    logging.info(
+                        "added {0} of {1} ({2}%)".format(
+                            i, len_input_sequence, float(i) / len_input_sequence * 100.0
+                        )
+                    )
                 graph[node1].append(node2)
         #!! self._check_that_symmetric(graph)
         return graph
 
     def _check_that_symmetric(self, graph):
         for node1, list in graph.items():
             for node2 in list:
                 if not node1 in graph[node2]:
-                    raise Exception("expect symmetric graph {0}, {1}".format(node1, node2))
+                    raise Exception(
+                        "expect symmetric graph {0}, {1}".format(node1, node2)
+                    )
 
     def _remove_node(self, graph, node1):
         node2List = graph[node1]
         del graph[node1]
         for node2 in node2List:
             graph[node2].remove(node1)
 
     def _find_a_most_connected_node(self, graph):
-        best_node, best_list = max(sorted(graph.items()), key=lambda pair : len(pair[1])) # find the node connected to the most other nodes
+        best_node, best_list = max(
+            sorted(graph.items()), key=lambda pair: len(pair[1])
+        )  # find the node connected to the most other nodes
         logging.debug("Removing a node with {0} connections".format(len(best_list)))
         return best_node
 
     def _piece_count(self, graph):
         unassigned = sorted(set(graph.keys()))
         pieceCount = 0
         while len(unassigned) > 0:
@@ -99,12 +103,14 @@
                             nextWorkList.append(node2)
                 workList = nextWorkList
                 nextWorkList = []
 
         logging.debug("piece_count={0}".format(pieceCount))
         return pieceCount
 
+
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
     import doctest
+
     doctest.testmod()
     print("done")
```

### Comparing `fastlmm-0.6.7/fastlmm/util/_example_file.py` & `fastlmm-0.6.8b1/fastlmm/util/_example_file.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/util/computePC.py` & `fastlmm-0.6.8b1/fastlmm/util/computePC.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 example of how to use feature selection from python (see also command line interface)
 """
 
-from __future__ import absolute_import
-from __future__ import print_function
 import numpy as np
 import scipy.linalg as LA
 import sys, os
 from fastlmm.pyplink.snpreader.Bed import Bed
 from fastlmm.feature_selection import PerformSelectionDistributable as dist
 
 if __name__ == "__main__":
```

### Comparing `fastlmm-0.6.7/fastlmm/util/compute_auto_pcs.py` & `fastlmm-0.6.8b1/fastlmm/util/compute_auto_pcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import warnings
 import numpy as np
-import scipy as sp
 import sys
 import logging
 import time
 from fastlmm.external.pca import PCA
 from pysnptools.snpreader import Bed
 from unittest.mock import patch
 
 
 def compute_auto_pcs(
     snpreader, cutoff=0.1, k_values=np.arange(11), output_file_name=None, count_A1=None
 ):
     """
+    DEPRECATED: Runs only on Intel, not AMD. We can't test this function because `compute_auto_pcs` uses the 'fastlmmC' executable which is not available in the test environment.
+
     Function automatically finds the best principle components (PCs)
 
     :param snpreader: SNPs for which to find the best PCs
           If you give a string, it should be the base name of a set of PLINK Bed-formatted files.
     :type snpreader: a `SnpReader <http://fastlmm.github.io/PySnpTools/#snpreader-snpreader>`__ or a string
 
     :param cutoff: (default: .1) The degree of relatedness to remove before finding the best number of PCs.
@@ -39,14 +41,17 @@
     >>> logging.basicConfig(level=logging.INFO)
     >>> file_name = example_file("fastlmm/feature_selection/examples/toydata.5chrom.*","*.bed")
     >>> best_pcs = compute_auto_pcs(file_name,count_A1=False)
     >>> print(int(best_pcs['vals'].shape[0]),int(best_pcs['vals'].shape[1]))
     500 0
 
     """
+    warning_text = "This function is deprecated. Runs only on Intel, not AMD. We can't test this function because `compute_auto_pcs` uses the 'fastlmmC' executable which is not available in the test environment."
+    warnings.warn(warning_text, category=DeprecationWarning, stacklevel=2)
+    print(warning_text, file=sys.stderr)
     with patch.dict("os.environ", {"ARRAY_MODULE": "numpy"}) as _:
         #!!could use regression tests beyond the docttest
 
         snpreader = _snp_fixup(snpreader, count_A1=count_A1)
 
         logging.info("reading all_std_snpdata")
         all_std_snpdata = (
@@ -144,15 +149,15 @@
             with open(output_file_name, "w") as f:
                 for iid_index, (famid, indid) in enumerate(all_std_snpdata.iid):
                     f.write("{0} {1} ".format(famid, indid))
                     f.write(" ".join([str(pc) for pc in X_fit[iid_index, :]]))
                     f.write("\n")
 
         result = {
-            "iid": sp.array(snpreader.iid),
+            "iid": np.array(snpreader.iid),
             "vals": X_fit,
             "header": ["pc_{0}".format(index) for index in range(bestNumPCs)],
         }
         return result
 
 
 def _snp_fixup(snp_input, count_A1=None):
```

### Comparing `fastlmm-0.6.7/fastlmm/util/est_h2.py` & `fastlmm-0.6.8b1/fastlmm/util/est_h2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import fastlmm.inference.lmm_cov as lmm_cov
 import numpy as np
 
+
 def est_h2(Y, K, covariates=None, nGridH2=10000, plot=True, verbose=True):
     """
     This function implements the Bayesian heritability estimate from Furlotte et al., 2014
 
     Furlotte, Nicholas A., David Heckerman, and Christoph Lippert.
     "Quantifying the uncertainty in heritability." Journal of human genetics 59.5 (2014): 269-275.
 
@@ -20,27 +19,48 @@
     returns:
         REML estimate of h^2 (as in Yang et al. 2010)
         posterior mean of h^2
         posterior variance of h^2
         h2 values on a grid
         posterior for h2 values on a grid
     """
-    lmm = lmm_cov.LMM(forcefullrank=False, X=covariates, linreg=None, Y=Y, G=None, K=K, regressX=True, inplace=False)
+    lmm = lmm_cov.LMM(
+        forcefullrank=False,
+        X=covariates,
+        linreg=None,
+        Y=Y,
+        G=None,
+        K=K,
+        regressX=True,
+        inplace=False,
+    )
     h2 = lmm.findH2()
     h2_posterior = lmm.posterior_h2(nGridH2=nGridH2)
     logp = -h2_posterior[2]
     grid = h2_posterior[1]
-    post_h2 = np.exp(logp-logp.max())/np.exp(logp-logp.max()).sum()*logp.shape[0]
-    h2_mean = (np.exp(logp-logp.max())*grid[:,np.newaxis]).sum()/np.exp(logp-logp.max()).sum()
-    h2_var = (np.exp(logp-logp.max())*(grid[:,np.newaxis] - h2_mean)**2.0).sum()/np.exp(logp-logp.max()).sum()
+    post_h2 = (
+        np.exp(logp - logp.max()) / np.exp(logp - logp.max()).sum() * logp.shape[0]
+    )
+    h2_mean = (np.exp(logp - logp.max()) * grid[:, np.newaxis]).sum() / np.exp(
+        logp - logp.max()
+    ).sum()
+    h2_var = (
+        np.exp(logp - logp.max()) * (grid[:, np.newaxis] - h2_mean) ** 2.0
+    ).sum() / np.exp(logp - logp.max()).sum()
     if plot:
         import pylab as plt
+
         plt.figure()
-        plt.plot([h2['h2'],h2['h2']],[0,1],"r")
-        plt.plot([h2_mean,h2_mean],[0,1],"g")
-        plt.legend(["REML-estimate = %.3f"%h2['h2'],"posterior mean = %.3f"%h2_mean])
-        plt.plot(grid.flatten(),post_h2.flatten())
+        plt.plot([h2["h2"], h2["h2"]], [0, 1], "r")
+        plt.plot([h2_mean, h2_mean], [0, 1], "g")
+        plt.legend(
+            ["REML-estimate = %.3f" % h2["h2"], "posterior mean = %.3f" % h2_mean]
+        )
+        plt.plot(grid.flatten(), post_h2.flatten())
         plt.xlabel("$h^2$")
         plt.ylabel("$p( h^2 | Data)$")
     if verbose:
-        print("max[h^2] = %.5f  E[h^2] = %.5f +- %.5f" % (h2['h2'], h2_mean,np.sqrt(h2_var)))
-    return h2, h2_mean, h2_var, grid, post_h2 
+        print(
+            "max[h^2] = %.5f  E[h^2] = %.5f +- %.5f"
+            % (h2["h2"], h2_mean, np.sqrt(h2_var))
+        )
+    return h2, h2_mean, h2_var, grid, post_h2
```

### Comparing `fastlmm-0.6.7/fastlmm/util/fastlmm.hashdown.json` & `fastlmm-0.6.8b1/fastlmm/util/fastlmm.hashdown.json`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/util/genphen.py` & `fastlmm-0.6.8b1/fastlmm/util/genphen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from __future__ import absolute_import
-import scipy as sp
 import numpy as np
-import pdb
 import scipy.linalg as la
 import fastlmm.util.util as utilx
 import sys
 
 
 def genphen(y_G0, G1, covDat, options, nInd, K1=None, fracCausal=None, randseed=None):
     """
@@ -37,68 +34,68 @@
     fracCausal = options["fracCausal"]
 
     if G1 is not None and options["varG"] > 0:
         if fracCausal > 1.0 or fracCausal < 0.01:
             raise Exception("fraCausal should be between 0.01 and 1")
         nSnp = G1.shape[1]
         if fracCausal != 1.0:
-            nSnpNew = sp.ceil(fracCausal * nSnp)
-            permutationIndex = utilx.generate_permutation(sp.arange(0, nSnp), randseed)[
+            nSnpNew = np.ceil(fracCausal * nSnp)
+            permutationIndex = utilx.generate_permutation(np.arange(0, nSnp), randseed)[
                 0:nSnpNew
             ]
             G1new = G1[:, permutationIndex]
         else:
             nSnpNew = nSnp
             G1new = G1
     elif K1 is not None:
         assert fracCausal == 1.0 or fracCausal is None
         pass
     else:
         assert (
             options["varG"] == 0
         ), "varG is not zero, but neither G1 nor K1 were provided"
 
-    stdG = sp.sqrt(options["varG"])
+    stdG = np.sqrt(options["varG"])
 
     if stdG > 0:
         if G1 is not None:
             y_G1 = stdG * G1new.dot(np.random.randn(nSnpNew, 1))  # good for low rank
         else:
             K1chol = la.cholesky(K1)
             y_G1 = stdG * K1chol.dot(np.random.randn(nInd, 1))  # good for full rank
     else:
         y_G1 = 0.0
     ##----------------------------------------------------------------
 
     if covDat is not None:
         nCov = covDat.shape[1]
-        covWeights = np.random.randn(nCov, 1) * sp.sqrt(options["varCov"])
+        covWeights = np.random.randn(nCov, 1) * np.sqrt(options["varCov"])
         y_beta = covDat.dot(covWeights)
     else:
         y_beta = 0.0
 
     y_noise_t = 0
     # heavy-tailed noise
     if options["varET"] > 0:
         y_noise_t = np.random.standard_t(
             df=options["varETd"], size=(nInd, 1)
-        ) * sp.sqrt(options["varET"])
+        ) * np.sqrt(options["varET"])
     else:
         y_noise_t = 0
 
     # gaussian noise
-    y_noise = np.random.randn(nInd, 1) * sp.sqrt(options["varE"])
+    y_noise = np.random.randn(nInd, 1) * np.sqrt(options["varE"])
 
     y = y_noise + y_noise_t + y_G0 + y_beta + y_G1
     y = y[:, 0]  # y.flatten()
 
     if options["link"] == "linear":
         return y
     elif options["link"] == "logistic":
         if options["casefrac"] is None:
             options["casefrac"] = 0.5
-        ysort = sp.sort(y, axis=None)
-        thresh = ysort[sp.floor(nInd * options["casefrac"])]
-        ybin = sp.array(y > thresh, dtype="float")
+        ysort = np.sort(y, axis=None)
+        thresh = ysort[np.floor(nInd * options["casefrac"])]
+        ybin = np.array(y > thresh, dtype="float")
         return ybin
     else:
         raise Exception("Invald link function for data generation")
```

### Comparing `fastlmm-0.6.7/fastlmm/util/gensnp.py` & `fastlmm-0.6.8b1/fastlmm/util/gensnp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from __future__ import absolute_import
-import scipy as sp
 import numpy as np
-import pdb
 import scipy.linalg as la
 
 
 def gendat(
     TWO_KERNEL,
     nInd,
     nSnp,
@@ -27,31 +24,31 @@
         y
         psSnps
     """
 
     if TWO_KERNEL:
         psSnps = gensnps(nInd, nSnp, minMaf, maxMaf)
         psK = psSnps.dot(psSnps.T)
-        psK += 1e-5 * sp.eye(nInd)
+        psK += 1e-5 * np.eye(nInd)
         psKchol = la.cholesky(psK)
     else:
         psSnps = None
 
     covDat = np.random.uniform(0, 1, (nInd, nCovar))
     covWeights = np.random.uniform(-0.5, 0.5, (nCovar, 1))
 
     sigE2 = np.random.uniform(low=minSigE2, high=maxSigE2)
     sigG2 = np.random.uniform(low=minSigG2, high=maxSigG2)
 
     ##generate the phenotype using the background kernel and covariates
     if TWO_KERNEL:
-        y_pop = sp.sqrt(sigG2) * psKchol.dot(sp.randn(nInd, 1))
+        y_pop = np.sqrt(sigG2) * psKchol.dot(np.randn(nInd, 1))
     else:
         y_pop = 0
-    y_noise = sp.randn(nInd, 1) * sp.sqrt(sigE2)
+    y_noise = np.randn(nInd, 1) * np.sqrt(sigE2)
     y = (covDat.dot(covWeights) + y_pop + y_noise).squeeze()
     return covDat, y, psSnps
 
 
 def gensnps(numSnp, nInd, minMaf=0.05, maxMaf=0.4, standardize=False):
     """
     Generate independent SNPs, from independent people (no population structure)
@@ -63,16 +60,16 @@
         raise Exception("invalid minMaf provided")
     if maxMaf < minMaf:
         raise Exception("invalid minMaf/maxMaf combo provided")
 
     maf = np.random.uniform(low=minMaf, high=maxMaf, size=(numSnp, 1))
 
     numChrm = 2
-    snpDat = sp.zeros((numSnp, nInd))
-    for ch in sp.arange(0, numChrm):
-        mafRep = sp.tile(maf, (1, nInd))
+    snpDat = np.zeros((numSnp, nInd))
+    for ch in np.arange(0, numChrm):
+        mafRep = np.tile(maf, (1, nInd))
         snpDat += np.random.uniform(size=(numSnp, nInd)) < mafRep
 
     if standardize:
         raise NotImplementedError()
 
     return snpDat
```

### Comparing `fastlmm-0.6.7/fastlmm/util/matrix/mmultfile.py` & `fastlmm-0.6.8b1/fastlmm/util/matrix/mmultfile.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/fastlmm/util/mingrid.py` & `fastlmm-0.6.8b1/fastlmm/util/mingrid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from __future__ import absolute_import
-from __future__ import print_function
-import scipy as SP
 import numpy as np
 import scipy.optimize as opt
-from six.moves import range
 
 
 def minimize1D(
     f,
     evalgrid=None,
     nGrid=10,
     minval=0.0,
@@ -113,36 +109,36 @@
 
 def evalgrid1D(f, evalgrid=None, nGrid=10, minval=0.0, maxval=0.99999, dimF=0):
     """
     evaluate a function f(x) on all values of a grid.
     --------------------------------------------------------------------------
     Input:
     f(x)    : callable target function
-    evalgrid: 1-D array prespecified grid of x-values
+    evalgrid: 1-D array pre-specified grid of x-values
     nGrid   : number of x-grid points to evaluate f(x)
     minval  : minimum x-value for optimization of f(x)
     maxval  : maximum x-value for optimization of f(x)
     --------------------------------------------------------------------------
     Output:
     evalgrid    : x-values
     resultgrid  : f(x)-values
     --------------------------------------------------------------------------
     """
     if evalgrid is None:
         step = (maxval - minval) / (nGrid)
-        evalgrid = SP.arange(minval, maxval + step, step)
+        evalgrid = np.arange(minval, maxval + step, step)
     if dimF:
-        resultgrid = SP.ones((evalgrid.shape[0], dimF)) * 9999999999999.0
+        resultgrid = np.ones((evalgrid.shape[0], dimF)) * 9999999999999.0
     else:
-        resultgrid = SP.ones(evalgrid.shape[0]) * 9999999999999.0
+        resultgrid = np.ones(evalgrid.shape[0]) * 9999999999999.0
     for i in range(evalgrid.shape[0]):
         fevalgrid = f(evalgrid[i])
 
         is_real = False
         try:
             is_real = np.isreal(fevalgrid).all()
-        except:
+        except Exception:
             is_real = np.isreal(fevalgrid)
         assert is_real, "function returned imaginary value"
 
         resultgrid[i] = fevalgrid
     return (evalgrid, resultgrid)
```

### Comparing `fastlmm-0.6.7/fastlmm/util/pickle_io.py` & `fastlmm-0.6.8b1/fastlmm/util/pickle_io.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 """
 simple module to save and load compressed pickle files
 """
 
-from __future__ import absolute_import
 import pickle
 import bz2
 import sys
 
- 
+
 def save(filename, myobj):
     """
     save object to file using pickle
-    
+
     @param filename: name of destination file
     @type filename: str
     @param myobj: object to save (has to be pickleable)
     @type myobj: obj
     """
- 
+
     try:
-        f = bz2.BZ2File(filename, 'wb')
+        f = bz2.BZ2File(filename, "wb")
     except IOError as details:
-        sys.stderr.write('File ' + filename + ' cannot be written\n')
+        sys.stderr.write("File " + filename + " cannot be written\n")
         sys.stderr.write(details)
         return
- 
+
     pickle.dump(myobj, f, protocol=2)
     f.close()
- 
- 
- 
+
+
 def load(filename):
     """
     Load from filename using pickle
-    
+
     @param filename: name of file to load from
     @type filename: str
     """
- 
+
     try:
-        f = bz2.BZ2File(filename, 'rb')
+        f = bz2.BZ2File(filename, "rb")
     except IOError as details:
-        sys.stderr.write('File ' + filename + ' cannot be read\n')
+        sys.stderr.write("File " + filename + " cannot be read\n")
         sys.stderr.write(details)
         return
- 
+
     myobj = pickle.load(f)
     f.close()
     return myobj
-
-
```

### Comparing `fastlmm-0.6.7/fastlmm/util/preprocess.py` & `fastlmm-0.6.8b1/fastlmm/util/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import absolute_import
 import numpy as np
 import time
 import fastlmm.util.standardizer as stdizer
 import warnings
 
 
 # TODO: wrap C-stuff here?
```

### Comparing `fastlmm-0.6.7/fastlmm/util/run_fastlmmc.py` & `fastlmm-0.6.8b1/fastlmm/util/run_fastlmmc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from __future__ import absolute_import
-from __future__ import print_function
-import subprocess 
-import os 
+import subprocess
+import os
 import scipy
 import scipy.io as IO
 import sys
 import logging
 
- # methods to call FaSTLMM-C++ Code
+# methods to call FaSTLMM-C++ Code
 
 
-def runLIN(bfile,pheno,outFilename,fastlmm_path=None,**kwargs):
-    '''    
+def runLIN(bfile, pheno, outFilename, fastlmm_path=None, **kwargs):
+    """
     use linear model for filtering SNPs
 
     --------------------------------------------------------------------------
     Input:
     bfile       basename for PLINK's binary .bed,.fam and .bin files
     pheno       name of phenotype file
     outDir      folder in which results flie is save
@@ -23,62 +21,92 @@
     topKbyLinReg save topK snps in file
     recode      boolean. if true, recode topK snps as binary plink files
     --------------------------------------------------------------------------
     Output
     linRegFile  file containing list of topK snps
     bfileTopK   PLINK binary file containing the topK snps
     --------------------------------------------------------------------------
-    '''
-    run(bfile,pheno,out=outFilename,linreg=True,fastlmm_path=fastlmm_path,**kwargs)
+    """
+    run(bfile, pheno, out=outFilename, linreg=True, fastlmm_path=fastlmm_path, **kwargs)
 
 
-
-def runFASTLMM(bfile,pheno,outDir,outFilename,methodsName=None,**kwargs):
-    '''
+def runFASTLMM(bfile, pheno, outDir, outFilename, methodsName=None, **kwargs):
+    """
     runs FASTLMM code
     --------------------------------------------------------------------------
     Input:
     bfile       basename for PLINK's binary .bed,.fam and .bin files
     pheno       name of phenotype file
     outDir      folder in which results flie is save
     outFilename the name of the output file
-   
+
     for more information, we refer to the user-manual of fast-lmm
-    '''
-    out = '%s/%s.%s.out.txt'%(outDir,outFilename,methodsName)
-    run(bfile,pheno,out=out,**kwargs)
+    """
+    out = "%s/%s.%s.out.txt" % (outDir, outFilename, methodsName)
+    run(bfile, pheno, out=out, **kwargs)
 
 
-def runLMMSELECT(bfile,pheno,outDir,outFilename,autoSelectCriterionMSE=True,**kwargs):
-    '''
+def runLMMSELECT(
+    bfile, pheno, outDir, outFilename, autoSelectCriterionMSE=True, **kwargs
+):
+    """
     runs LMM-Select code
 
     --------------------------------------------------------------------------
     Input:
     bfile       basename for PLINK's binary .bed,.fam and .bin files
     pheno       name of phenotype file
     outDir      folder in which results flie is save
     outFilename the name of the output file
-    autoSelectCriterionMSE  directs AutoSelect ot use out-of-sample mean-squared error for the selection criterion. 
+    autoSelectCriterionMSE  directs AutoSelect ot use out-of-sample mean-squared error for the selection criterion.
                             Otherwise out-of-sample log likelihood is used
-   
+
     for more information, we refer to the user-manual of fast-lmm
-    '''
-   # 1. determine number of SNPs in the kernel
-    autoSelect = '%s/%s.LMMSELECT.aoselect'%(outDir,outFilename)
-    run(bfile,pheno, autoSelect=autoSelect,autoSelectCriterionMSE=autoSelectCriterionMSE,**kwargs)
+    """
+    # 1. determine number of SNPs in the kernel
+    autoSelect = "%s/%s.LMMSELECT.aoselect" % (outDir, outFilename)
+    run(
+        bfile,
+        pheno,
+        autoSelect=autoSelect,
+        autoSelectCriterionMSE=autoSelectCriterionMSE,
+        **kwargs
+    )
     # 2. run GWAS
-    out = '%s/%s.%s.out.txt'%(outDir,outFilename,'LMMSELECT')
-    extractSim = '%s/%s.LMMSELECT.aoselect.snps.txt'%(outDir,outFilename)
-    run(bfile,pheno,out=out,extractSim=extractSim,**kwargs)
- 
-
-def run(bfile=None,pheno=None,bfileSim=None,sim=None,linreg=None,covar=None,out=None,optLogdelta=None,extract=None,extractSim=None,autoSelect=None,autoSelectCriterionMSE=False,
-        excludeByPosition=None,excludeByGeneticDistance=None,eigen=None,eigenOut=None,maxThreads=None,simOut=None,fastlmm_path=None,topKbyLinReg=None,numJobs=None,thisJob=None,REML=False):
-    '''
+    out = "%s/%s.%s.out.txt" % (outDir, outFilename, "LMMSELECT")
+    extractSim = "%s/%s.LMMSELECT.aoselect.snps.txt" % (outDir, outFilename)
+    run(bfile, pheno, out=out, extractSim=extractSim, **kwargs)
+
+
+def run(
+    bfile=None,
+    pheno=None,
+    bfileSim=None,
+    sim=None,
+    linreg=None,
+    covar=None,
+    out=None,
+    optLogdelta=None,
+    extract=None,
+    extractSim=None,
+    autoSelect=None,
+    autoSelectCriterionMSE=False,
+    excludeByPosition=None,
+    excludeByGeneticDistance=None,
+    eigen=None,
+    eigenOut=None,
+    maxThreads=None,
+    simOut=None,
+    fastlmm_path=None,
+    topKbyLinReg=None,
+    numJobs=None,
+    thisJob=None,
+    REML=False,
+):
+    """
     interface for FastLMM software
 
     --------------------------------------------------------------------------
     Input:
     bfile       basename for PLINK's binary .bed,.fam and .bin files
     pheno       name of phenotype file
     bfileSim    basename for PLINK's binary files for building genetic similarity
@@ -96,96 +124,112 @@
     excludeByGeneticDistance excludes the SNP tested and those within this distance from the genetic similarity matrix
     eigen       load the spectral decomposition object from the directory name
     eigenOut    save the spectral decomposition object to the directory name
     maxThreads  suggests the level of parallelism to use
     simOut      specifies that genetic similarities are to be written to this file
     topKbyLinRegdirects AutoSelect to use only the top <int> SNPs, as determined by linear regression, while selecting SNPs
     for more information, we refer to the user-manual of fast-lmm
-    '''
+    """
     os.environ["FastLmmUseAnyMklLib"] = "1"
-    logging.info('Run FAST-LMM')
+    logging.info("Run FAST-LMM")
 
     osname = sys.platform
-    if (osname.find("win") >= 0):    #         was loaded, if it was loaded from a file
+    if osname.find("win") >= 0:  #         was loaded, if it was loaded from a file
         fastlmmpath = os.path.join(fastlmm_path, "fastlmmc.exe")
-    elif (osname.find("linux") >= 0):
+    elif osname.find("linux") >= 0:
         fastlmmpath = os.path.join(fastlmm_path, "fastlmmc")
         import stat
+
         st = os.stat(fastlmmpath)
         os.chmod(fastlmmpath, st.st_mode | stat.S_IEXEC)
     else:
-        logging.info('\n\n unsupported operating system!')
-    if not os.path.isfile(fastlmmpath) : raise Exception("Expect file {0}".format(fastlmmpath))
+        logging.info("\n\n unsupported operating system!")
+    if not os.path.isfile(fastlmmpath):
+        raise Exception("Expect file {0}".format(fastlmmpath))
     logging.info("fastlmmC path=" + fastlmmpath)
 
-
-    cmd = '\"%s\" -simLearnType Once'%(fastlmmpath) # change that! logdelta is always only optimized on the null model
-    
-    if bfile!=None:
-        assert os.path.exists(bfile + '.bed'), 'ouch, bfile is missing: %s'%bfile
-        assert os.path.exists(bfile + '.bim'), 'ouch, bfile is missing: %s'%bfile
-        assert os.path.exists(bfile + '.fam'), 'ouch, bfile is missing: %s'%bfile
-        cmd += ' -bfile %s'%bfile
-    if pheno!=None:
-        assert os.path.exists(pheno), 'ouch, pheno is missing: %s'%pheno
-        cmd += ' -pheno %s'%pheno
-    if sim!=None:
-        assert os.path.exists(sim), 'ouch, sim is missing: %s'%sim
-        cmd += ' -sim %s'%sim
-    if linreg==True:
-        cmd += ' -linreg'
-    if covar!=None:
-        assert os.path.exists(covar), 'ouch, covar is missing: %s'%covar
-        cmd += ' -covar %s'%covar
+    cmd = '"%s" -simLearnType Once' % (
+        fastlmmpath
+    )  # change that! logdelta is always only optimized on the null model
+
+    if bfile != None:
+        assert os.path.exists(bfile + ".bed"), "ouch, bfile is missing: %s" % bfile
+        assert os.path.exists(bfile + ".bim"), "ouch, bfile is missing: %s" % bfile
+        assert os.path.exists(bfile + ".fam"), "ouch, bfile is missing: %s" % bfile
+        cmd += " -bfile %s" % bfile
+    if pheno != None:
+        assert os.path.exists(pheno), "ouch, pheno is missing: %s" % pheno
+        cmd += " -pheno %s" % pheno
+    if sim != None:
+        assert os.path.exists(sim), "ouch, sim is missing: %s" % sim
+        cmd += " -sim %s" % sim
+    if linreg == True:
+        cmd += " -linreg"
+    if covar != None:
+        assert os.path.exists(covar), "ouch, covar is missing: %s" % covar
+        cmd += " -covar %s" % covar
     if REML:
-        cmd += ' -REML'
+        cmd += " -REML"
     else:
-        cmd += ' -ML'
-    if out!=None:
-        cmd += ' -out %s'%out
-    if optLogdelta!=None:
-        cmd += ' -brentMinLogVal %.4f -brentMaxLogVal %.4f -brentStarts 1 -brentMaxIter 1'%(optLogdelta-1E-3,optLogdelta+1E-3) #Why substract .001?
+        cmd += " -ML"
+    if out != None:
+        cmd += " -out %s" % out
+    if optLogdelta != None:
+        cmd += (
+            " -brentMinLogVal %.4f -brentMaxLogVal %.4f -brentStarts 1 -brentMaxIter 1"
+            % (optLogdelta - 1e-3, optLogdelta + 1e-3)
+        )  # Why substract .001?
     else:
-        cmd += ' -brentMinLogVal %.4f -brentMaxLogVal %.4f '%(-5,10)
-    if extract!=None:
-        assert os.path.exists(extract), 'ouch, extract is missing: %s'%extract
-        cmd += ' -extract %s'%extract
-    if extractSim!=None:
-        assert os.path.exists(extractSim), 'ouch, extractSim is missing: %s'%extractSim
-        cmd += ' -extractSim %s'%extractSim
-    if autoSelect!=None:
-        cmd += ' -autoSelect %s'%autoSelect
+        cmd += " -brentMinLogVal %.4f -brentMaxLogVal %.4f " % (-5, 10)
+    if extract != None:
+        assert os.path.exists(extract), "ouch, extract is missing: %s" % extract
+        cmd += " -extract %s" % extract
+    if extractSim != None:
+        assert os.path.exists(extractSim), (
+            "ouch, extractSim is missing: %s" % extractSim
+        )
+        cmd += " -extractSim %s" % extractSim
+    if autoSelect != None:
+        cmd += " -autoSelect %s" % autoSelect
     if autoSelectCriterionMSE == True:
-        cmd += ' -autoSelectCriterionMSE'
-    if excludeByGeneticDistance!=None:
-        cmd += ' -excludeByGeneticDistance %d'%excludeByGeneticDistance
-    if excludeByPosition!=None:
-        cmd += ' -excludeByPosition %d -verboseOut'%excludeByPosition
-    if eigen!=None:
-        cmd += ' -eigen %s'%eigen
-    if eigenOut!=None:
-        cmd += ' -eigenOut %s -runGwasType NORUN'%eigenOut # stop after computing the EVD
-    if maxThreads!=None:
-        cmd += ' -maxThreads %d'%maxThreads
-    if simOut!=None:
-        cmd += ' -simOut %s -runGwasType NORUN'%simOut # stop after computer the EVD
-    if numJobs!=None:
-        cmd += ' -numjobs %d'%numJobs
-    if thisJob!=None:
-        cmd += ' -thisjob %d'%thisJob
-
-    if bfileSim!=None:
-        assert os.path.exists(bfileSim + '.bed'), 'ouch, bfileSim is missing: %s'%bfileSim
-        assert os.path.exists(bfileSim + '.bim'), 'ouch, bfileSim is missing: %s'%bfileSim
-        assert os.path.exists(bfileSim + '.fam'), 'ouch, bfileSim is missing: %s'%bfileSim
-        cmd += ' -bfileSim %s'%bfileSim
-    if topKbyLinReg!=None:
-        cmd += ' -topKbyLinReg %d'%topKbyLinReg
+        cmd += " -autoSelectCriterionMSE"
+    if excludeByGeneticDistance != None:
+        cmd += " -excludeByGeneticDistance %d" % excludeByGeneticDistance
+    if excludeByPosition != None:
+        cmd += " -excludeByPosition %d -verboseOut" % excludeByPosition
+    if eigen != None:
+        cmd += " -eigen %s" % eigen
+    if eigenOut != None:
+        cmd += (
+            " -eigenOut %s -runGwasType NORUN" % eigenOut
+        )  # stop after computing the EVD
+    if maxThreads != None:
+        cmd += " -maxThreads %d" % maxThreads
+    if simOut != None:
+        cmd += " -simOut %s -runGwasType NORUN" % simOut  # stop after computer the EVD
+    if numJobs != None:
+        cmd += " -numjobs %d" % numJobs
+    if thisJob != None:
+        cmd += " -thisjob %d" % thisJob
+
+    if bfileSim != None:
+        assert os.path.exists(bfileSim + ".bed"), (
+            "ouch, bfileSim is missing: %s" % bfileSim
+        )
+        assert os.path.exists(bfileSim + ".bim"), (
+            "ouch, bfileSim is missing: %s" % bfileSim
+        )
+        assert os.path.exists(bfileSim + ".fam"), (
+            "ouch, bfileSim is missing: %s" % bfileSim
+        )
+        cmd += " -bfileSim %s" % bfileSim
+    if topKbyLinReg != None:
+        cmd += " -topKbyLinReg %d" % topKbyLinReg
     logging.info(cmd)
-    
+
     output = ""
     try:
         output = subprocess.check_output(cmd, shell=True, stderr=subprocess.STDOUT)
     except Exception as e:
         print(e)
     print(output)
     # LG.info(output)
```

### Comparing `fastlmm-0.6.7/fastlmm/util/standardizer/Beta.py` & `fastlmm-0.6.8b1/fastlmm/util/standardizer/Beta.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,52 @@
-from __future__ import absolute_import
 import numpy as np
-import scipy as sp
 import logging
 
-class Beta(object): #IStandardizer
+
+class Beta(object):  # IStandardizer
     """The specification for beta standardization"""
-    def __init__(self,a=1,b=25):
+
+    def __init__(self, a=1, b=25):
         import warnings
+
         #!!warnings.warn("This Beta is deprecated. Pysnptools includes newer versions of Beta", DeprecationWarning)
         self.a = a
         self.b = b
 
-    def standardize(self, snps, blocksize=None, force_python_only=False,num_threads=None):
-        l = self.lambdaFactory(snps, blocksize=blocksize, force_python_only=force_python_only,num_threads=num_threads)
+    def standardize(
+        self, snps, blocksize=None, force_python_only=False, num_threads=None
+    ):
+        l = self.lambdaFactory(
+            snps,
+            blocksize=blocksize,
+            force_python_only=force_python_only,
+            num_threads=num_threads,
+        )
         import fastlmm.util.standardizer as stdizer
+
         return stdizer.standardize_with_lambda(snps, l, blocksize)
 
     @staticmethod
-    def _standardizer(snps,a,b,force_python_only,num_threads):
+    def _standardizer(snps, a, b, force_python_only, num_threads):
         from pysnptools.standardizer import Standardizer
-        Standardizer._standardize_unit_and_beta(snps, is_beta=True, a=a, b=b, apply_in_place=True, use_stats=False,stats=None,force_python_only=force_python_only,num_threads=num_threads)
-        return snps
 
+        Standardizer._standardize_unit_and_beta(
+            snps,
+            is_beta=True,
+            a=a,
+            b=b,
+            apply_in_place=True,
+            use_stats=False,
+            stats=None,
+            force_python_only=force_python_only,
+            num_threads=num_threads,
+        )
+        return snps
 
-    def lambdaFactory(self, snps, blocksize=None, force_python_only=False,num_theads=None):
+    def lambdaFactory(
+        self, snps, blocksize=None, force_python_only=False, num_theads=None
+    ):
         from pysnptools.standardizer import Standardizer
-        return lambda s,a=self.a,b=self.b,force_python_only=force_python_only:self._standardizer(snps,a,b,force_python_only,num_threads)
-
 
+        return lambda s, a=self.a, b=self.b, force_python_only=force_python_only: self._standardizer(
+            snps, a, b, force_python_only, num_threads
+        )
```

### Comparing `fastlmm-0.6.7/fastlmm/util/standardizer/Unit.py` & `fastlmm-0.6.8b1/fastlmm/util/standardizer/Unit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,52 @@
-from __future__ import absolute_import
 import numpy as np
-import scipy as sp
 import logging
 
-class Unit(object):  #IStandardizer
+
+class Unit(object):  # IStandardizer
     """The specification for unit standardization"""
+
     def __init__(self):
         import warnings
+
         #!!warnings.warn("This Unit is deprecated. Pysnptools includes newer versions of Unit", DeprecationWarning)
         pass
 
-    def standardize(self, snps, blocksize=None, force_python_only=False,num_threads=None):
-        l = self.lambdaFactory(snps, blocksize=blocksize, force_python_only=force_python_only,num_threads=num_threads)
+    def standardize(
+        self, snps, blocksize=None, force_python_only=False, num_threads=None
+    ):
+        l = self.lambdaFactory(
+            snps,
+            blocksize=blocksize,
+            force_python_only=force_python_only,
+            num_threads=num_threads,
+        )
         import fastlmm.util.standardizer as stdizer
+
         return stdizer.standardize_with_lambda(snps, l, blocksize)
 
     @staticmethod
-    def _standardizer(snps,force_python_only,num_threads):
+    def _standardizer(snps, force_python_only, num_threads):
         from pysnptools.standardizer import Standardizer
-        Standardizer._standardize_unit_and_beta(snps, is_beta=False, a=float("NaN"), b=float("NaN"), apply_in_place=True, use_stats=False,stats=None,force_python_only=force_python_only,num_threads=num_threads)
+
+        Standardizer._standardize_unit_and_beta(
+            snps,
+            is_beta=False,
+            a=float("NaN"),
+            b=float("NaN"),
+            apply_in_place=True,
+            use_stats=False,
+            stats=None,
+            force_python_only=force_python_only,
+            num_threads=num_threads,
+        )
         return snps
 
-    def lambdaFactory(self, snps, blocksize=None, force_python_only=False,num_threads=None):
-        return lambda s,force_python_only=force_python_only:self._standardizer(snps,force_python_only,num_threads)
+    def lambdaFactory(
+        self, snps, blocksize=None, force_python_only=False, num_threads=None
+    ):
+        return lambda s, force_python_only=force_python_only: self._standardizer(
+            snps, force_python_only, num_threads
+        )
 
     def __str__(self):
         return "{0}()".format(self.__class__.__name__)
```

### Comparing `fastlmm-0.6.7/fastlmm/util/standardizer/__init__.py` & `fastlmm-0.6.8b1/fastlmm/util/standardizer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,93 +1,101 @@
-from __future__ import absolute_import
 from .Beta import *
 from .Unit import *
 
-#import warnings
-#warnings.warn("This __init__.py is deprecated. Pysnptools includes newer version", DeprecationWarning)
+# import warnings
+# warnings.warn("This __init__.py is deprecated. Pysnptools includes newer version", DeprecationWarning)
+
 
 def factory(s):
     s = s.capitalize()
-    if s == "Unit" or s=="Unit()":
+    if s == "Unit" or s == "Unit()":
         return Unit()
 
-    if s=="Beta":
+    if s == "Beta":
         return Beta()
 
     if s.startswith("Beta("):
         standardizer = eval(s)
         return standardizer
 
-def standardize_with_lambda(snps, lambdax, blocksize = None):
-    if blocksize==None:
-       return lambdax(snps)
+
+def standardize_with_lambda(snps, lambdax, blocksize=None):
+    if blocksize == None:
+        return lambdax(snps)
 
     idx_start = 0
     idx_stop = blocksize
 
-    while idx_start<snps.shape[1]:
-        #print idx_start
-        lambdax(snps[:,idx_start:idx_stop])
+    while idx_start < snps.shape[1]:
+        # print idx_start
+        lambdax(snps[:, idx_start:idx_stop])
 
         idx_start = idx_stop
         idx_stop += blocksize
-        if idx_stop>snps.shape[1]:
+        if idx_stop > snps.shape[1]:
             idx_stop = snps.shape[1]
 
     return snps
 
+
 def standardize_unit_python(snps, returnStats=False):
-    '''
+    """
     standardize snps to zero-mean and unit variance
-    '''
+    """
 
     N = snps.shape[0]
     S = snps.shape[1]
 
     imissX = np.isnan(snps)
-    snp_sum =  np.nansum(snps,axis=0)
+    snp_sum = np.nansum(snps, axis=0)
     n_obs_sum = (~imissX).sum(0)
-    
-    snp_mean = (snp_sum*1.0)/n_obs_sum
+
+    snp_mean = (snp_sum * 1.0) / n_obs_sum
     snps -= snp_mean
-    snp_std = np.sqrt(np.nansum(snps**2, axis=0)/n_obs_sum)
+    snp_std = np.sqrt(np.nansum(snps**2, axis=0) / n_obs_sum)
 
     # avoid div by 0 when standardizing
     if snp_std.__contains__(0.0):
-        logging.warning("A least one snps has only one value, that is, its standard deviation is zero")
+        logging.warning(
+            "A least one snps has only one value, that is, its standard deviation is zero"
+        )
     snp_std[snp_std == 0.0] = 1.0
     snps /= snp_std
     snps[imissX] = 0
-    
+
     if returnStats:
-        return snps,snp_mean,snp_std
+        return snps, snp_mean, snp_std
 
     return snps
 
+
 def standardize_beta_python(snps, betaA, betaB):
-    '''
+    """
     standardize snps with Beta prior
-    '''
+    """
 
     N = snps.shape[0]
     S = snps.shape[1]
 
     imissX = np.isnan(snps)
-    snp_sum =  np.nansum(snps,axis=0)
+    snp_sum = np.nansum(snps, axis=0)
     n_obs_sum = (~imissX).sum(0)
-    
-    snp_mean = (snp_sum*1.0)/n_obs_sum
+
+    snp_mean = (snp_sum * 1.0) / n_obs_sum
     snps -= snp_mean
-    snp_std = np.sqrt(np.nansum(snps**2, axis=0)/n_obs_sum)
+    snp_std = np.sqrt(np.nansum(snps**2, axis=0) / n_obs_sum)
     if snp_std.__contains__(0.0):
-        logging.warning("A least one snps has only one value, that is, its standard deviation is zero")
+        logging.warning(
+            "A least one snps has only one value, that is, its standard deviation is zero"
+        )
 
-    maf = snp_mean/2.0
-    maf[maf>0.5]=1.0- maf[maf>0.5]
+    maf = snp_mean / 2.0
+    maf[maf > 0.5] = 1.0 - maf[maf > 0.5]
 
     # avoid div by 0 when standardizing
     import scipy.stats as st
+
     maf_beta = st.beta.pdf(maf, betaA, betaB)
-    snps*=maf_beta
+    snps *= maf_beta
     snps[imissX] = 0.0
-     
+
     return snps
```

### Comparing `fastlmm-0.6.7/fastlmm/util/stats/__init__.py` & `fastlmm-0.6.8b1/fastlmm/util/stats/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import numpy as np
-import scipy as sp
 import scipy.stats as st
 import scipy.interpolate
 import scipy.linalg as la
 import fastlmm.util.preprocess as util
 import scipy.stats as st
 import time
-from six.moves import range
 
 # import ipdb
 
 
 def print_missing_info(y):
     print(
         str(np.isnan(y).sum().sum())
@@ -50,33 +46,33 @@
     [N, M] = snps.shape
     print("found nind=" + str(N) + ", nsnp=" + str(M))
     if M < N:
         print("only doing full rank, should use low rank here")
 
     # not needed, and in practice, makes no difference
     # mean center the individuals
-    # meanval=sp.mean(snps,axis=0)
+    # meanval=np.mean(snps,axis=0)
     # snps=snps-meanval
 
     print("computing kernel...")
     t0 = time.time()
-    K = sp.dot(snps, snps.T)
+    K = np.dot(snps, snps.T)
     t1 = time.time()
     print(("Elapsed time %.2f seconds" % (t1 - t0)))
     snps = None
 
     t0 = time.time()
     print("computing svd...")
     [U, S, V] = la.svd(K, full_matrices=False)  #!!!use big_svd?
     t1 = time.time()
     print(("Elapsed time %.2f seconds" % (t1 - t0)))
 
-    S = sp.sqrt(S)
-    # UShalf=sp.dot(U,sp.diag(S)) #expensive
-    UShalf = sp.multiply(
+    S = np.sqrt(S)
+    # UShalf=np.dot(U,np.diag(S)) #expensive
+    UShalf = np.multiply(
         U, np.tile(S, (N, 1))
     )  # faster, but not as fast as as_strided which I can't get to work
     pccov = UShalf[:, 0:npc]
     print("done.")
     if outfile is not None:
         import fastlmm.util.util as ut
 
@@ -92,15 +88,15 @@
     colname = "2*(LL(alt)-LL(null))"
     lrtperm = pd.read_csv(
         filein, delimiter="\t", dtype={colname: np.float64}, usecols=[colname]
     )[colname].values
     print("found " + str(len(lrtperm)) + "null test stats")
 
     mix = c2.chi2mixture(lrt=lrtperm, qmax=qmax, alteqnull=None)
-    res = mix.fit_params_Qreg()  # paramter fitting
+    res = mix.fit_params_Qreg()  # parameter fitting
     print("mixture (non-zero dof)=" + str(mix.mixture) + "\n")
     print("dof=" + str(res["dof"]) + "\n")
     print("scale=" + str(res["scale"]) + "\n")
 
 
 def lrt_method(stat, dof):
     """
@@ -161,19 +157,19 @@
     r2 = lsqSol[1]  # squared residuals
     D = lsqSol[2]  # rank of design matrix
 
     N = y.shape[0]
 
     if not (REML):
         sigma2 = r2 / (N)
-        nLL = N * 0.5 * sp.log(2 * sp.pi * sigma2) + N * 0.5
+        nLL = N * 0.5 * np.log(2 * np.pi * sigma2) + N * 0.5
     else:
         sigma2 = r2 / (N - D)
-        nLL = N * 0.5 * sp.log(2 * sp.pi * sigma2) + 0.5 / sigma2 * r2
-        nLL -= 0.5 * D * sp.log(2 * sp.pi * sigma2)
+        nLL = N * 0.5 * np.log(2 * np.pi * sigma2) + 0.5 / sigma2 * r2
+        nLL -= 0.5 * D * np.log(2 * np.pi * sigma2)
         # REML term
 
     result = {"nLL": nLL, "sigma2": sigma2, "beta": beta, "REML": REML}
     if result["nLL"] is None:
         raise Exception("no nLL result")
     return result
```

### Comparing `fastlmm-0.6.7/fastlmm/util/stats/chi2mixture.py` & `fastlmm-0.6.8b1/fastlmm/util/stats/chi2mixture.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-from __future__ import absolute_import
-import scipy as sp
 import numpy as np
 import scipy.stats as st
-import scipy.special
+import scipy.special as ss
 import fastlmm.util.mingrid as mingrid
-import pdb
 import logging
-from six.moves import range
 
 
 class chi2mixture(object):
     """
     mixture here denotes the weight on the non-zero dof compnent
     """
 
@@ -82,32 +78,32 @@
         """
         if self.tol < 0.0:
             logging.info("tol has to be larger or equal than zero.")
         if self.alteqnull is None:
             self.alteqnull = self.lrt == 0
             logging.info("WARNING: alteqnull not provided, so using alteqnull=(lrt==0)")
         if self.mixture is None:
-            self.mixture = 1.0 - (sp.array(self.alteqnull).sum() * 1.0) / (
-                sp.array(self.alteqnull).shape[0] * 1.0
+            self.mixture = 1.0 - (np.array(self.alteqnull).sum() * 1.0) / (
+                np.array(self.alteqnull).shape[0] * 1.0
             )
         return self.alteqnull, self.mixture
 
     def fit_params_Qreg(self):
         """
         Fit the scale and dof parameters of the model by minimizing the squared error between
         the model log quantiles and the log P-values obtained on the lrt values.
 
-        Only the top qmax quantile is being used for the fit (self.qmax is used in fit_scale_logP).
+        Only the top qmax quartile is being used for the fit (self.qmax is used in fit_scale_logP).
         """
-        # imin= sp.argsort(self.lrt[~self.i0])
+        # imin= np.argsort(self.lrt[~self.i0])
         # ntests = self.lrt.shape[0]
         if self.isortlrt is None:
             self.isortlrt = self.lrt.argsort()[::-1]
             self.qnulllrtsort = (
-                0.5 + sp.arange(self.mixture * self.isortlrt.shape[0])
+                0.5 + np.arange(self.mixture * self.isortlrt.shape[0])
             ) / (self.mixture * self.isortlrt.shape[0])
             self.lrtsort = self.lrt[self.isortlrt]
         resmin = [
             None
         ]  # CL says it had to be a list or wouldn't work, even though doesn't make sense
         if self.fitdof:  # fit both scale and dof
 
@@ -160,37 +156,33 @@
 
         min = mingrid.minimize1D(
             f=f, nGrid=10, minval=self.scalemin, maxval=self.scalemax
         )
         return resmin[0]
 
     def scale_dof_obj(self, scale, dof):
-        base = sp.exp(
-            1
-        )  # fitted params are invariant to this logarithm base (i.e.10, or e)
+        nfalse = len(self.alteqnull) - np.sum(self.alteqnull)
 
-        nfalse = len(self.alteqnull) - sp.sum(self.alteqnull)
-
-        imax = int(sp.ceil(self.qmax * nfalse))  # of only non zer dof component
+        imax = int(np.ceil(self.qmax * nfalse))  # of only non zer dof component
         p = st.chi2.sf(self.lrtsort[0:imax] / scale, dof)
-        logp = sp.logn(base, p)
-        r = sp.logn(base, self.qnulllrtsort[0:imax]) - logp
+        logp = np.log(p)
+        r = np.log(self.qnulllrtsort[0:imax]) - logp
         if self.abserr:
-            err = sp.absolute(r).sum()
+            err = np.absolute(r).sum()
         else:  # mean square error
             err = (r * r).mean()
         return err, imax
 
-    def mse_qreg(self, scale, dof, lrt, base):
+    def mse_qreg(self, scale, dof, lrt):
         """
         For debugging: returns mse for particular scale and dof, given pre-filtered lrt
         """
         p = st.chi2.sf(lrt / scale, dof)
-        logp = sp.logn(base, p)
-        r = sp.logn(base, self.qnulllrtsort[0 : len(lrt)]) - logp
+        logp = ss.log(p)
+        r = ss.log(self.qnulllrtsort[0 : len(lrt)]) - logp
         mse = (r * r).mean()
         return mse
 
     def sf(self, lrt=None, alteqnull=None):
         """
         compute the survival function of the mixture of scaled chi-square_0 and scaled chi-square_dof
         ---------------------------------------------------------------------------
@@ -207,15 +199,15 @@
             alteqnull = self.alteqnull
         else:
             assert (
                 alteqnull is not None
             ), "alteqnull is none, but lrt is not (seems unexpected, JL)"
 
         pv = st.chi2.sf(lrt / self.scale, self.dof) * self.mixture
-        pv[sp.array(alteqnull)] = 1.0
+        pv[np.array(alteqnull)] = 1.0
         return pv
 
     # OBSOLETE: but was known to work. Can delete once we get past problems with python code solved.
     def computePVmixtureChi2(lrt, a2=None, tol=0.0, mixture=0.5, scale=1.0, dof=1.0):
         """
         OBSOLETE: but was known to work. Can delete once we get past problems with python code solved.
 
@@ -259,30 +251,30 @@
             if a2 is None:
                 i0 = lrt <= (0.0 + tol)
             else:
                 i0 = a2 <= (0.0 + tol)
 
         N = (~i0).sum()
         sumX = (lrt[~i0]).sum()
-        logsumX = (sp.log(lrt[~i0])).sum()
+        logsumX = (np.log(lrt[~i0])).sum()
         if (dof is None) and (scale is None):
             # f is the Gamma likelihood with the scale parameter maximized analytically as a function of 0.5 * the degrees of freedom
             f = lambda k: -1.0 * (
-                -N * sp.special.gammaln(k)
-                - k * N * (sp.log(sumX) - sp.log(k) - sp.log(N))
+                -N * np.special.gammaln(k)
+                - k * N * (np.log(sumX) - np.log(k) - np.log(N))
                 + (k - 1.0) * logsumX
                 - k * N
             )
             # f_ = lambda(x): 1-N*N/(2.0*x*sumX)
             res = minimize1D(f, evalgrid=None, nGrid=10, minval=0.1, maxval=3.0)
             dof = 2.0 * res[0]
         elif dof is None:
             f = lambda k: -1.0 * (
-                -N * sp.special.gammaln(k)
-                - k * N * sp.log(2.0 * scale)
+                -N * np.special.gammaln(k)
+                - k * N * np.log(2.0 * scale)
                 + (k - 1.0) * logsumX
                 - sumX / (2.0 * scale)
             )
             res = minimize1D(f, evalgrid=None, nGrid=10, minval=0.1, maxval=3.0)
             dof = 2.0 * res[0]
         if scale is None:
             # compute condition for ML
@@ -305,24 +297,24 @@
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
     logging.info("generate chi-2 distributed values")
     scale = 3
     dof = 2
     mixture = 0.5
     ntests = 10000
-    lrt = sp.zeros((ntests))
-    lrttest = sp.zeros((ntests))
+    lrt = np.zeros((ntests))
+    lrttest = np.zeros((ntests))
     for i in range(dof):
         x = np.randn(ntests)
-        xtest = sp.randn(ntests)
+        xtest = np.randn(ntests)
         lrt += scale * (x * x)
         lrttest += scale * (xtest * xtest)
 
-    lrt[np.random.permutation(ntests)[0 : sp.ceil(ntests * mixture)]] = 0.0
-    lrttest[np.random.permutation(ntests)[0 : sp.ceil(ntests * mixture)]] = 0.0
+    lrt[np.random.permutation(ntests)[0 : np.ceil(ntests * mixture)]] = 0.0
+    lrttest[np.random.permutation(ntests)[0 : np.ceil(ntests * mixture)]] = 0.0
 
     qmax = 0.2
     logging.info(("create the distribution object, with qmax = %.4f" % qmax))
     mix = chi2mixture(lrt=lrt, a2=None, qmax=0.2)  # object constructor
 
     logging.info("fit the parameter of the object by log-Pvalue quantile regression")
     import time
```

### Comparing `fastlmm-0.6.7/fastlmm/util/stats/plotp.py` & `fastlmm-0.6.8b1/fastlmm/util/stats/plotp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import scipy as sp
 import scipy.stats as st
 import scipy.interpolate
 import scipy.linalg as la
 import pylab as pl
 from fastlmm.association.tests import Cv
 import fastlmm.util.util as ut
 
@@ -21,15 +20,15 @@
 
 
 def excludefiles():
     return ["work_directory", "info", "lrtperm", "synthPhen.txt"]
 
 
 def threshlist():
-    return sp.array([1e-10, 1e-9, 1e-8, 1e-7, 1e-6, 1e-5, 1e-4, 1e-3, 1e-2, 1e-1])
+    return np.array([1e-10, 1e-9, 1e-8, 1e-7, 1e-6, 1e-5, 1e-4, 1e-3, 1e-2, 1e-1])
 
 
 def getfiles(dirin, filepattern):
     import glob
 
     filepatternorig = filepattern
     filepattern = dirin + r"/" + filepattern
@@ -111,22 +110,22 @@
     betaDown        lower error bars
     theoreticalPvals    theoretical P-values under uniform
     --------------------------------------------------------------------
     """
 
     # assumes 'log10'
 
-    mRange = 10 ** (sp.arange(sp.log10(0.5), sp.log10(M - 0.5) + 0.1, 0.1))
+    mRange = 10 ** (np.arange(np.log10(0.5), np.log10(M - 0.5) + 0.1, 0.1))
     # should be exp or 10**?
     numPts = len(mRange)
-    betaalphaLevel = sp.zeros(numPts)
+    betaalphaLevel = np.zeros(numPts)
     # down in the plot
-    betaOneMinusalphaLevel = sp.zeros(numPts)
+    betaOneMinusalphaLevel = np.zeros(numPts)
     # up in the plot
-    betaInvHalf = sp.zeros(numPts)
+    betaInvHalf = np.zeros(numPts)
     for n in range(numPts):
         m = mRange[n]
         # numplessThanThresh=m;
         betaInvHalf[n] = st.beta.ppf(0.5, m, M - m)
         betaalphaLevel[n] = st.beta.ppf(alphalevel, m, M - m)
         betaOneMinusalphaLevel[n] = st.beta.ppf(1 - alphalevel, m, M - m)
         pass
@@ -159,32 +158,32 @@
     for f in myfilestmp:
         keep = True
         for str in excludefiles():
             if str in f:
                 keep = False
         if keep:
             myfiles.append(f)
-    indrange = sp.arange(0, len(myfiles))
+    indrange = np.arange(0, len(myfiles))
     pv0 = {}
     pv1 = {}
     rowids = {}
     label = {}
     for j in indrange:
         pv0[j], rowids[j], garb1, garb2 = extractpvals(
             myfiles[j], [pnames[0]], rownames, sort=True
         )
         if logspace:
-            pv0[j] = -sp.log10(pv0[j])
+            pv0[j] = -np.log10(pv0[j])
         label[j] = os.path.basename(myfiles[j])
 
         pv1[j], rowids[j], garb1, garb2 = extractpvals(
             myfiles[j], [pnames[1]], rownames, sort=True
         )
         if logspace:
-            pv1[j] = -sp.log10(pv1[j])
+            pv1[j] = -np.log10(pv1[j])
 
     import pylab as pl
 
     pl.ion()
     for j1 in indrange:
         assert len(pv0[j1]) == len(pv1[j1]), "different # of pvals"
         pl.figure()
@@ -227,53 +226,53 @@
             if strn in f:
                 keep = False
         if keep:
             myfiles.append(f)
             print("keeping: " + f)
         else:
             print("not including: " + f)
-    indrange = sp.arange(0, len(myfiles))
+    indrange = np.arange(0, len(myfiles))
     if len(myfiles) == 0:
         raise Exception("no files found")
     pv = {}
     pvorig = {}
     lambdas = {}
     rowids = {}
     label = {}
     for j in indrange:
         pv[j], rowids[j], dummy1, dummy2 = extractpvals(
             myfiles[j], pnames, rownames, sort=True
         )
         pvorig[j] = pv[j]
         lambdas[j] = lambda_gc = estimate_lambda(pv[j])
-        # pv[j]=-sp.log10(pv[j])
+        # pv[j]=-np.log10(pv[j])
         # pv[j][pv[j]<minpval]=minpval
         label[j] = os.path.basename(myfiles[j]) + ", $\lambda$=%1.3f" % lambdas[j]
         if j == 0:
             idorder = rowids[j]
         else:
             if not all(idorder == idorder):
                 raise Exception("ids do not match up across file:" + label[j])
 
     import pylab as pl
 
     pl.ion()
     # these loops are to find out which are "notokany"
-    notokany = sp.zeros_like(pv[0], dtype=bool)
+    notokany = np.zeros_like(pv[0], dtype=bool)
     for j1 in indrange:
-        for j2 in sp.arange(j1 + 1, len(myfiles)):
+        for j2 in np.arange(j1 + 1, len(myfiles)):
             assert len(pv[j1]) == len(pv[j2]), "different # of pvals in each file"
             imag = (pv[j1] <= 0.0) | (pv[j2] <= 0.0)
             one = (pv[j1] > 1.0) | (pv[j2] > 1.0)
             iok = (~imag) & (~one)
             notokany = notokany | (~iok)
 
     # these are the standard plotting loops
     for j1 in indrange:
-        for j2 in sp.arange(j1 + 1, len(myfiles)):
+        for j2 in np.arange(j1 + 1, len(myfiles)):
             if fliporder:
                 tmp = j1
                 j1 = j2
                 j2 = tmp
             assert len(pv[j1]) == len(pv[j2]), "different # of pvals in each file"
             if newplot:
                 pl.figure()
@@ -284,59 +283,59 @@
             one = (pv[j1] > 1.0) | (pv[j2] > 1.0)
 
             # print pv[j1][imag]
             # print pv[j2][imag]
             iok = (~imag) & (~one)
 
             if not heatmap:
-                tmpj1 = sp.copy(pv[j1])
-                tmpj2 = sp.copy(pv[j2])
+                tmpj1 = np.copy(pv[j1])
+                tmpj2 = np.copy(pv[j2])
                 minpval1 = min(tmpj1[~imag1])
                 minpval2 = min(tmpj2[~imag2])
                 tmpj1[imag1] = minpval1
                 tmpj2[imag2] = minpval2
 
                 pl.plot(
-                    -sp.log10(tmpj1[iok]), -sp.log10(tmpj2[iok]), ".k", markersize=ms
+                    -np.log10(tmpj1[iok]), -np.log10(tmpj2[iok]), ".k", markersize=ms
                 )
-                # pl.plot(-sp.log10(tmpj1[notokany]),-sp.log10(tmpj2[notokany]),'b.',markersize=ms)
+                # pl.plot(-np.log10(tmpj1[notokany]),-np.log10(tmpj2[notokany]),'b.',markersize=ms)
                 # maxval=max(pl.xlim()[1],pl.ylim()[1])
                 pl.plot(
-                    -sp.log10(tmpj1[imag1]),
-                    -sp.log10(tmpj2[imag1]),
+                    -np.log10(tmpj1[imag1]),
+                    -np.log10(tmpj2[imag1]),
                     "g.",
                     markersize=ms,
                 )
                 pl.plot(
-                    -sp.log10(tmpj1[imag2]),
-                    -sp.log10(tmpj2[imag2]),
+                    -np.log10(tmpj1[imag2]),
+                    -np.log10(tmpj2[imag2]),
                     "r.",
                     markersize=ms,
                 )
 
-                # pl.plot(-sp.log10(pv[j1][~iok]),-sp.log10(pv[j2][~iok]),'g.')
+                # pl.plot(-np.log10(pv[j1][~iok]),-np.log10(pv[j2][~iok]),'g.')
                 maxval = max(pl.xlim()[1], pl.ylim()[1])
                 pl.plot([0, maxval + 1], [0, maxval + 1], "b--", linewidth=1)
                 # fix_axes()
                 pl.xlim([0, maxval + 1])
                 pl.ylim([0, maxval + 1])
                 pl.xlabel(label[j1], fontsize=fs)
                 pl.ylabel(label[j2], fontsize=fs)
             else:
                 heatmap, xedges, yedges = np.histogram2d(
-                    -sp.log10(pv[j1]), -sp.log10(pv[j2]), bins=100
+                    -np.log10(pv[j1]), -np.log10(pv[j2]), bins=100
                 )
                 if extent is None:
                     extent = [
                         xedges[0],
                         xedges[-1],
                         yedges[0],
                         yedges[-1],
                     ]  # heatmap=heatmap[-1:heatmap.shape[0]:-1,:]
-                pl.imshow(sp.log(heatmap + 1), extent=extent, cmap=pl.cm.Greys)
+                pl.imshow(np.log(heatmap + 1), extent=extent, cmap=pl.cm.Greys)
                 pl.colorbar()
     return pvorig
 
 
 def type1errdir_agg(
     dirin,
     filepattern=["*.txt"],
@@ -356,18 +355,18 @@
 ):
     """
     filepattern is a list of filepatterns, each of which is processed seperate as in type1errdir
     """
     assert dopower, "need to add in clause if false"
     S = len(filepattern)
     obs_count = [None for i in range(S)]
-    obs_count_tot = sp.zeros([len(threshlist())])
+    obs_count_tot = np.zeros([len(threshlist())])
     N_tot = 0
     Norig = None
-    for s in sp.arange(0, S):
+    for s in np.arange(0, S):
         if filepattern[s] is not None:
             (
                 thresh,
                 obs_error,
                 obs_count[s],
                 p_twot,
                 N,
@@ -405,15 +404,15 @@
     for f in filepattern:
         print(f)
     padl = 15
     strfm = "%1.2e"
 
     print("Threshold".ljust(padl, " ") + "\t" + "Obs. Count".ljust(padl, " "))
     print("--------------------------------------------------------")
-    for t in sp.arange(0, len(thresh)):
+    for t in np.arange(0, len(thresh)):
         print(
             str(strfm % thresh[t]).ljust(padl, " ")
             + "\t"
             + (str(int(obs_count_tot[t])) + "/" + str(N_tot)).ljust(padl, " ")
         )
 
     return thresh, obs_count_tot, N_tot
@@ -469,18 +468,18 @@
     duplicates = []
     extras = []
     auditind = None
 
     # put all p-values in to one qqplot, and also report the type 1 errors
     # for 1e-1 through to smallest order of magnitude
     pv = []
-    obs_count = -1 * sp.zeros([len(thresh)])
-    obs_error = -1 * sp.zeros([len(thresh)])
-    p_onet = sp.NaN * sp.zeros([len(thresh)])
-    p_twot = sp.NaN * sp.zeros([len(thresh)])
+    obs_count = -1 * np.zeros([len(thresh)])
+    obs_error = -1 * np.zeros([len(thresh)])
+    p_onet = np.NaN * np.zeros([len(thresh)])
+    p_twot = np.NaN * np.zeros([len(thresh)])
     ii = 0
     for f in myfiles:
         if "info.txt" not in f:
             import os
 
             shortf = os.path.split(f)[1]
             # if verbose: print str(ii) + ") " + shortf
@@ -514,19 +513,19 @@
                         obs_count[t] = obs_count[t] + ct
                         t = t + 1
                         if t >= len(thresh):
                             break
                 ii = ii + 1
     N = len(pv)
 
-    for t in sp.arange(0, len(thresh)):
-        p_onet[t] = 1 - sp.stats.binom.sf(
+    for t in np.arange(0, len(thresh)):
+        p_onet[t] = 1 - np.stats.binom.sf(
             obs_count[t] - 1, N, thresh[t]
         )  # -1 is there to include 51 as well ;-) (one-tailed test)
-        p_twot[t] = sp.stats.binom_test(obs_count[t], N, thresh[t])  # (two-tailed test)
+        p_twot[t] = np.stats.binom_test(obs_count[t], N, thresh[t])  # (two-tailed test)
 
     nfiles = ii
     missingind = []
     if verbose:
         if auditrange is not None:
             nummis = 0
             msg = "missinginds=["
@@ -581,29 +580,29 @@
                 + "\t"
                 + "Obs. Count".ljust(padl, " ")
                 + "\t"
                 + "two-tail P".ljust(padl, " ")
             )  # + "\t" + "one-tail P".ljust(padl," ")
             print("--------------------------------------------------------")
             strfm = "%1.2e"
-            for t in sp.arange(0, len(thresh)):
+            for t in np.arange(0, len(thresh)):
                 print(
                     str(strfm % thresh[t]).ljust(padl, " ")
                     + "\t"
                     + str(strfm % (obs_count[t] / float(N))).ljust(padl, " ")
                     + "\t"
                     + (str(int(obs_count[t])) + "/" + str(N)).ljust(padl, " ")
                     + "\t"
                     + str(strfm % (p_twot[t])).ljust(padl, " ")
                 )
         else:
             print("Threshold".ljust(padl, " ") + "\t" + "Obs. Count".ljust(padl, " "))
             print("--------------------------------------------------------")
             strfm = "%1.2e"
-            for t in sp.arange(0, len(thresh)):
+            for t in np.arange(0, len(thresh)):
                 print(
                     str(strfm % thresh[t]).ljust(padl, " ")
                     + "\t"
                     + (str(int(obs_count[t])) + "/" + str(N)).ljust(padl, " ")
                 )
     if plot:
         fileout = None
@@ -685,15 +684,15 @@
         else:
             pv, rowids, garb1, garb2 = extractpvals(f, pnames, rownames)
             # allp.append(pv) #this gives all seperate plots on one (makes several series)
             allp = allp + pv.tolist()  # this just makes one series
     if aggregate:
         title = "agg over " + filepatternorig + " (" + str(len(allp)) + " p-values)"
         qqplotp(
-            sp.array(allp),
+            np.array(allp),
             fileout=None,
             pnames=pnames,
             rownames=rownames,
             alphalevel=alphalevel,
             legend=None,
             title=title,
             dohist=dohist,
@@ -847,21 +846,20 @@
 
     h2 = pl.figure()
     [nn, bins, patches] = pl.hist(pv, numbins, normed=1)
     pl.plot([0, 1], [1, 1], linespec, linewidth=linewidth)
 
 
 def tmp():
-    import scipy as sp
     import fastlmm.util.stats.plotp as pt
 
     pall = []
-    for j in sp.arange(0, 100):
-        p = sp.rand(1, 1000)
-        p100 = sp.repeat(p, 100)
+    for j in np.arange(0, 100):
+        p = np.rand(1, 1000)
+        p100 = np.repeat(p, 100)
         pall.append(p100)
     qqplotavg(pall)
 
 
 def qqplotavg(
     pvallist,
     fileout=None,
@@ -872,20 +870,20 @@
     fixaxes=True,
 ):
     """
     Average the qqplots in pvallist (assumes qq theoretical is same for all, and averages qq empirical)
     """
     L = len(pvallist)
     qemp = None
-    for i in sp.arange(0, L):
+    for i in np.arange(0, L):
         pval = pvallist[i].flatten()
         M = pval.shape[0]
-        pnull = (0.5 + sp.arange(M)) / M
-        qnull = -sp.log10(pnull)
-        qemptmp = -sp.log10(sp.sort(pval))
+        pnull = (0.5 + np.arange(M)) / M
+        qnull = -np.log10(pnull)
+        qemptmp = -np.log10(np.sort(pval))
         if qemp is None:
             qemp = qemptmp
         else:
             qemp = qemp + qemptmp
     qavg = qemp / L
     qqplotfromq(qnull, qavg)
 
@@ -919,21 +917,21 @@
     if ylim is not None:
         pl.ylim(ylim)
     if alphalevel is not None:
         if distr == "log10":
             betaUp, betaDown, theoreticalPvals = _qqplot_bar(
                 M=M, alphalevel=alphalevel, distr=distr
             )
-            lower = -sp.log10(theoreticalPvals - betaDown)
-            upper = -sp.log10(theoreticalPvals + betaUp)
+            lower = -np.log10(theoreticalPvals - betaDown)
+            upper = -np.log10(theoreticalPvals + betaUp)
             pl.fill_between(
-                -sp.log10(theoreticalPvals), lower, upper, color="grey", alpha=0.5
+                -np.log10(theoreticalPvals), lower, upper, color="grey", alpha=0.5
             )
-            # pl.plot(-sp.log10(theoreticalPvals),lower,'g-.')
-            # pl.plot(-sp.log10(theoreticalPvals),upper,'g-.')
+            # pl.plot(-np.log10(theoreticalPvals),lower,'g-.')
+            # pl.plot(-np.log10(theoreticalPvals),upper,'g-.')
     if legendlist is not None:
         leg = pl.legend(legendlist, loc=4, numpoints=1)
         # set the markersize for the legend
         for lo in leg.legendHandles:
             lo.set_markersize(10)
 
     if fixaxes:
@@ -986,39 +984,39 @@
         legendlist = legend
     else:
         legendlist = [legend]
 
     if h1 is None:
         h1 = pl.figure(figsize=figsize)
 
-    pl.grid(b=grid, alpha=0.5)
+    pl.grid(which="both", alpha=0.5)
 
     maxval = 0
 
     for i in range(len(pvallist)):
         pval = pvallist[i].flatten()
         M = pval.shape[0]
-        pnull = (0.5 + sp.arange(M)) / M
+        pnull = (0.5 + np.arange(M)) / M
         # pnull = np.sort(np.random.uniform(size = tests))
 
         pval[pval < minpval] = minpval
         pval[pval >= 1] = 1
 
         if distr == "chi2":
             qnull = st.chi2.isf(pnull, 1)
-            qemp = st.chi2.isf(sp.sort(pval), 1)
+            qemp = st.chi2.isf(np.sort(pval), 1)
             xl = "LOD scores"
             yl = "$\chi^2$ quantiles"
 
         if distr == "log10":
-            qnull = -sp.log10(pnull)
-            qemp = -sp.log10(sp.sort(pval))  # sorts the object, returns nothing
+            qnull = -np.log10(pnull)
+            qemp = -np.log10(np.sort(pval))  # sorts the object, returns nothing
             xl = "-log10(P) observed"
             yl = "-log10(P) expected"
-        if not (sp.isreal(qemp)).all():
+        if not (np.isreal(qemp)).all():
             raise Exception("imaginary qemp found")
         if qnull.max() > maxval:
             maxval = qnull.max()
         pl.plot(qnull, qemp, ".", markersize=2)
         # pl.plot([0,qemp.max()], [0,qemp.max()],'r')
         if addlambda:
             lambda_gc = estimate_lambda(pval)
@@ -1060,10 +1058,10 @@
     estimate the lambda for a given array of P-values
     ------------------------------------------------------------------
     pv          numpy array containing the P-values
     ------------------------------------------------------------------
     L           lambda value
     ------------------------------------------------------------------
     """
-    LOD2 = sp.median(st.chi2.isf(pv, 1))
+    LOD2 = np.median(st.chi2.isf(pv, 1))
     L = LOD2 / 0.456
     return L
```

### Comparing `fastlmm-0.6.7/fastlmm/util/test.py` & `fastlmm-0.6.8b1/fastlmm/util/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,63 @@
-from __future__ import absolute_import
-from __future__ import print_function
 import numpy as np
-import scipy as sp
 import logging
 import doctest
 import sys
 
 import unittest
 import os.path
 import time
 
 
-   
-
 # We do it this way instead of using doctest.DocTestSuite because doctest.DocTestSuite requires modules to be pickled, which python doesn't allow.
 # We need tests to be pickleable so that they can be run on a cluster.
 class TestDocStrings(unittest.TestCase):
 
     def test_vertex_cut(self):
         import fastlmm.util.VertexCut
+
         old_dir = os.getcwd()
         os.chdir(os.path.dirname(os.path.realpath(__file__)))
         result = doctest.testmod(fastlmm.util.VertexCut)
         os.chdir(old_dir)
         assert result.failed == 0, "failed doc test: " + __file__
 
     def test_sample_util(self):
         import fastlmm.util.util
+
         old_dir = os.getcwd()
         os.chdir(os.path.dirname(os.path.realpath(__file__)))
 
         import matplotlib.pyplot as plt
+
         result = doctest.testmod(fastlmm.util.util)
         os.chdir(old_dir)
         assert result.failed == 0, "failed doc test: " + __file__
 
-    def test_compute_auto_pcs(self):
+    def deprecated_test_compute_auto_pcs(self):
         import fastlmm.util.compute_auto_pcs
+
         old_dir = os.getcwd()
         os.chdir(os.path.dirname(os.path.realpath(__file__)))
-        result = doctest.testmod(sys.modules['fastlmm.util.compute_auto_pcs'])
+        result = doctest.testmod(sys.modules["fastlmm.util.compute_auto_pcs"])
         os.chdir(old_dir)
         assert result.failed == 0, "failed doc test: " + __file__
 
 
-
 def getTestSuite():
     """
     set up composite test suite
     """
-    
+
     test_suite = unittest.TestSuite([])
     test_suite.addTests(unittest.TestLoader().loadTestsFromTestCase(TestDocStrings))
 
     return test_suite
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
 
     suites = getTestSuite()
     r = unittest.TextTestRunner(failfast=False)
     ret = r.run(suites)
     assert ret.wasSuccessful()
     print("done")
```

### Comparing `fastlmm-0.6.7/fastlmm/util/util.py` & `fastlmm-0.6.8b1/fastlmm/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import numpy as np
 import warnings
 import logging
 import sys
 import time
 import pysnptools.util as pstutil
-from six.moves import range
+
 from types import ModuleType
 
 
 def thin_results_file(myfile, dup_postfix="v2"):
     """
     Used in score vs lrt to remove any lines in the results
     ending with "v2", as these were replicate gene set entries.
@@ -558,15 +558,17 @@
     rle = list(_run_length_encode(array[:, 0]))
 
     if xaxis_unit_bp:  # compute and use cumulative basepair positions for x-axis
         if chromosome_starts is None:
             chromosome_starts = _compute_x_positions_chrom(array)
         chr_pos_list = _compute_x_positions_snps(array, chromosome_starts)
         plt.xlim([0, chromosome_starts[-1, 2] + 1])
-        plt.xticks(chromosome_starts[:, 1:3].mean(1), chromosome_starts[:, 0])
+        plt.xticks(
+            chromosome_starts[:, 1:3].mean(1), chromosome_starts[:, 0].astype(int)
+        )
     else:  # use rank indices for x-axis
         chr_pos_list = np.arange(array.shape[0])
         xTickMarks = [str(int(item)) for item, count in rle]
         plt.xlim([0, array.shape[0]])
         plt.xticks(list(_rel_to_midpoint(rle)), xTickMarks)
     y = -np.log10(array[:, 2])
     max_y = y.max()
@@ -604,23 +606,22 @@
     plt.ylim([-np.log10(plot_threshold), None])
     return chromosome_starts
 
 
 def _compute_x_positions_chrom(positions, offset=1e5):
     chromosomes = np.unique(positions[:, 0])
     chromosomes.sort()
-    chromosome_starts = np.zeros((chromosomes.shape[0], 3), dtype="object")
+    chromosome_starts = np.zeros((chromosomes.shape[0], 3), dtype="float")
     chr_start_next = 0
     for i, chromosome in enumerate(chromosomes):
-        pos_chr = positions[positions[:, 0] == chromosome]
+        pos_chr = positions[positions[:, 0] == chromosome, 1]
         chromosome_starts[i, 0] = chromosome  # the chromosome
         chromosome_starts[i, 1] = chr_start_next  # start of the chromosome
-        chromosome_starts[i, 2] = (
-            chr_start_next + pos_chr.max()
-        )  # end of the chromosome
+        # end of the chromosome
+        chromosome_starts[i, 2] = chr_start_next + np.nanmax(pos_chr)
         chr_start_next = chromosome_starts[i, 2] + offset
     return chromosome_starts
 
 
 def _compute_x_positions_snps(positions, chromosome_starts):
     cumulative_pos = np.zeros(positions.shape[0])
     for i, chromosome_start in enumerate(chromosome_starts):
```

### Comparing `fastlmm-0.6.7/fastlmm.egg-info/PKG-INFO` & `fastlmm-0.6.8b1/fastlmm.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlmm
-Version: 0.6.7
+Version: 0.6.8b1
 Summary: Fast GWAS
 Home-page: https://fastlmm.github.io/
 Author: FaST-LMM Team
 Author-email: fastlmm-dev@python.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/fastlmm/FaST-LMM/issues
 Project-URL: Documentation, http://fastlmm.github.io/FaST-LMM
@@ -15,52 +15,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS.txt
+Requires-Dist: pandas>=1.1.1
+Requires-Dist: matplotlib>=1.5.1
+Requires-Dist: scikit-learn>=0.19.1
+Requires-Dist: bed-reader>=1.0.4
+Requires-Dist: pysnptools>=0.5.11
+Requires-Dist: cloudpickle>=2.2.0
+Requires-Dist: statsmodels>=0.10.1
+Requires-Dist: psutil>=5.6.7
+Requires-Dist: fastlmmclib>=0.0.3
 
 FaST-LMM
 =================================
 
 FaST-LMM, which stands for Factored Spectrally Transformed Linear Mixed Models, is a program for performing 
 genome-wide association studies (GWAS) on datasets of all sizes, up to one millions samples.
 
 This release contains the following features, each illustrated with an IPython notebook.
 
-* Core FaST-LMM ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
+* Core FaST-LMM ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
 
 Improvements:
 
-* New features for single_snp (including effect size and multiple phenotype support) and epistasis (including reporting beta and using pre-computed eigenvalue decompositions) ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb))  -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
-* Ludicrous-Speed GWAS ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)) -- [Kadie and Heckerman, *bioRxiv* 2018](https://www.biorxiv.org/content/10.1101/154682v2)
-* Heritability with Spatial Correction ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)), [Heckerman *et al.*, *PNAS* 2016](http://www.pnas.org/content/113/27/7377.abstract)
-* Two Kernels ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Widmer *et al.*, *Scientific Reports* 2014](http://www.nature.com/srep/2014/141112/srep06874/full/srep06874.html)
-* Set Analysis ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Bioinformatics* 2014](http://bioinformatics.oxfordjournals.org/content/early/2014/09/07/bioinformatics.btu504)
-* Epistasis ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Scientific Reports,* 2013](http://www.nature.com/srep/2013/130122/srep01099/full/srep01099.html)
-* Prediction ([notebook](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
+* New features for single_snp (including effect size and multiple phenotype support) and epistasis (including reporting beta and using pre-computed eigenvalue decompositions) ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb))  -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
+* Ludicrous-Speed GWAS ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)) -- [Kadie and Heckerman, *bioRxiv* 2018](https://www.biorxiv.org/content/10.1101/154682v2)
+* Heritability with Spatial Correction ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)), [Heckerman *et al.*, *PNAS* 2016](http://www.pnas.org/content/113/27/7377.abstract)
+* Two Kernels ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Widmer *et al.*, *Scientific Reports* 2014](http://www.nature.com/srep/2014/141112/srep06874/full/srep06874.html)
+* Set Analysis ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Bioinformatics* 2014](http://bioinformatics.oxfordjournals.org/content/early/2014/09/07/bioinformatics.btu504)
+* Epistasis ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Scientific Reports,* 2013](http://www.nature.com/srep/2013/130122/srep01099/full/srep01099.html)
+* Prediction ([notebook](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)) -- [Lippert *et al.*, *Nature Methods* 2011](http://www.nature.com/nmeth/journal/v8/n10/abs/nmeth.1681.html)
 
 *A C++ version, which is generally less functional, is available. See http://fastlmm.github.io/.*
 
 Quick install:
 =================================
 
 `pip install fastlmm`
 
 For best performance, be sure your Python distribution includes a fast version of NumPy. We use Anaconda's [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
 
 Documentation
 =================================
 
 * IPython Notebooks:
-	* [Core, Epistasis, Set Analysis, Two Kernels](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)
-    * [Multiple-Phenotype GWAS and related features](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb)
-	* [Heritability with Spatial Correction](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)
-	* [Ludicrous-Speed GWAS](https://nbviewer.jupyter.org/github/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)
+	* [Core, Epistasis, Set Analysis, Two Kernels](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/FaST-LMM.ipynb)
+    * [Multiple-Phenotype GWAS and related features](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/fastlmm2021.ipynb)
+	* [Heritability with Spatial Correction](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/heritability_si.ipynb)
+	* [Ludicrous-Speed GWAS](https://github.com/fastlmm/FaST-LMM/blob/master/doc/ipynb/SingleSnpScale.ipynb)
 * [Main Documentation](http://fastlmm.github.io/FaST-LMM/)
 * [Project Home and Full Annotated Bibliography](https://fastlmm.github.io/)
 
 
 Code
 =================================
 * [PyPi](https://pypi.org/project/fastlmm/)
```

### Comparing `fastlmm-0.6.7/fastlmm.egg-info/SOURCES.txt` & `fastlmm-0.6.8b1/fastlmm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.7/setup.py` & `fastlmm-0.6.8b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Work around https://github.com/pypa/pip/issues/7953
 import site
 import sys
 
 site.ENABLE_USER_SITE = "--user" in sys.argv[1:]
 
 # Version number
-version = "0.6.7"
+version = "0.6.8b1"
 
 
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
@@ -88,14 +88,15 @@
         ],
         "fastlmm": ["util/fastlmm.hashdown.json"],
     },
     install_requires=[
         "pandas>=1.1.1",
         "matplotlib>=1.5.1",
         "scikit-learn>=0.19.1",
-        "pysnptools>=0.5.7",
+        "bed-reader>=1.0.4",
+        "pysnptools>=0.5.11",
         "cloudpickle>=2.2.0",
         "statsmodels>=0.10.1",
         "psutil>=5.6.7",
         "fastlmmclib>=0.0.3",
     ],
 )
```

### Comparing `fastlmm-0.6.7/tests/test.py` & `fastlmm-0.6.8b1/tests/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from __future__ import absolute_import
 import re
 import numpy as NP
-import scipy as SP
 import scipy.io as SIO
 import time
 import os
 import os.path
 import sys
 from fastlmm.association.FastLmmSet import FastLmmSet
 from fastlmm.association.FastLmmSet import Local
@@ -15,84 +13,94 @@
 import fastlmm.feature_selection.test
 import pysnptools.test
 import shutil
 import logging
 import fastlmm.util.util as ut
 from pysnptools.util.mapreduce1.distributabletest import DistributableTest
 from pysnptools.util.mapreduce1.runner import Local, LocalMultiProc, LocalInParts
-from fastlmm.pyplink.snpreader.Hdf5 import Hdf5 #Need by some *.py's that we eval
+from fastlmm.pyplink.snpreader.Hdf5 import Hdf5  # Need by some *.py's that we eval
 
 tolerance = 1e-4
 
-#def compare_files(afilename, bfilename):
+# def compare_files(afilename, bfilename):
 #    if not os.path.isfile(afilename) or not os.path.isfile(bfilename):
 #        return False
 #    if os.name == 'posix':
 #        call = 'wine CompareFiles/CompareFiles.exe'
 #    else:
 #        call = 'CompareFiles/CompareFiles.exe'
 #    out = subprocess.check_output(call+' -tol '+str(tolerance)+' '+afilename+' '
 #                                  +bfilename, shell=True)
 #    return out.find('Files are comparable.') != -1
 
 
-
 class WidgetTestCase(unittest.TestCase):
     def __init__(self, infile):
         unittest.TestCase.__init__(self)
 
         self._infile = infile
-        #if not self._existExpectedOutput():
+        # if not self._existExpectedOutput():
         #    self._generateExpectedOutput()
 
     def _tmpOutfile(self):
         outfile = os.path.splitext(self._infile)[0]
-        return 'tmp/'+outfile+'.txt'
-    
+        return "tmp/" + outfile + ".txt"
+
     def _referenceOutfile(self):
         #!!similar code elsewhere
-        import platform;
-        os_string=platform.platform()
+        import platform
+
+        os_string = platform.platform()
         outfile = os.path.splitext(self._infile)[0]
 
-        windows_fn = 'expected-Windows/'+outfile+'.txt'
+        windows_fn = "expected-Windows/" + outfile + ".txt"
         assert os.path.exists(windows_fn), "Can't find file '{0}'".format(windows_fn)
-        debian_fn = 'expected-debian/'+outfile  +'.txt'
-        if not os.path.exists(debian_fn): #If reference file is not in debian folder, look in windows folder
+        debian_fn = "expected-debian/" + outfile + ".txt"
+        if not os.path.exists(
+            debian_fn
+        ):  # If reference file is not in debian folder, look in windows folder
             debian_fn = windows_fn
 
         if "debian" in os_string or "Linux" in os_string:
             if "Linux" in os_string:
-                logging.warning("comparing to Debian output even though found: %s" % os_string)
+                logging.warning(
+                    "comparing to Debian output even though found: %s" % os_string
+                )
             return debian_fn
         else:
             if "Windows" not in os_string:
-                logging.warning("comparing to Windows output even though found: %s" % os_string)
-            return windows_fn 
-
+                logging.warning(
+                    "comparing to Windows output even though found: %s" % os_string
+                )
+            return windows_fn
 
     def runTest(self):
-        os.chdir( os.path.dirname( os.path.realpath(__file__) ) )
+        os.chdir(os.path.dirname(os.path.realpath(__file__)))
         tmpOutfile = self._tmpOutfile()
         referenceOutfile = self._referenceOutfile()
         logging.info(f"{'inputs/'+self._infile}")
-        with open('inputs/'+self._infile) as f:
+        with open("inputs/" + self._infile) as f:
             filecontent = f.read()
 
         runner = Local()
         try:
             distributable = eval(filecontent)
         except Exception as e:
-            raise Exception("Can't eval '{0}' because of '{1}'".format(self._infile,e.message))
-        runner.run(distributable)                               
-                
-        out,msg=ut.compare_files(tmpOutfile, referenceOutfile, tolerance)                
-        self.assertTrue(out, "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile))
+            raise Exception(
+                "Can't eval '{0}' because of '{1}'".format(self._infile, e.message)
+            )
+        runner.run(distributable)
+
+        out, msg = ut.compare_files(tmpOutfile, referenceOutfile, tolerance)
+        self.assertTrue(
+            out,
+            "msg='{0}', ref='{1}', tmp='{2}'".format(msg, referenceOutfile, tmpOutfile),
+        )
 
-    #def _generateExpectedOutput(self):
+    # def _generateExpectedOutput(self):
     #    tmpOutfile = self._tmpOutfile()
     #    referenceOutfile = self._referenceOutfile()
     #    with open('inputs/'+self._infile) as f:
     #        filecontent = f.read()
 
     #    runner = Local()
     #    exec(filecontent)
@@ -102,39 +110,40 @@
 
     def _existExpectedOutput(self):
         return os.path.isfile(self._referenceOutfile())
 
     def __str__(self):
         return self._infile
 
+
 ##for debuggingk
-#def getDebugTestSuite():
+# def getDebugTestSuite():
 #    suite = unittest.TestSuite()
 #    suite.addTest(WidgetTestCase('sc_davies_two_kernel_linear_qqfit.N300.needsReorder.py'))
 #    return suite
 
+
 def getTestSuiteX():
     suite = unittest.TestSuite()
-    for f in os.listdir( 'inputs' ):
-        if re.match(r'.*\.py$', f) is None:
+    for f in os.listdir("inputs"):
+        if re.match(r".*\.py$", f) is None:
             continue
         # from tests.test import WidgetTestCase
         suite.addTest(WidgetTestCase(f))
     return suite
 
+
 def removeTmpFiles():
     if os.path.exists("tmp"):
         shutil.rmtree("tmp")
-        #for f in os.listdir( 'tmp' ):
+        # for f in os.listdir( 'tmp' ):
         #    os.remove(os.path.join('tmp', f), )
 
 
-if __name__ == '__main__':
-
-
+if __name__ == "__main__":
     logging.basicConfig(level=logging.WARN)
     removeTmpFiles()
 
     import fastlmm.association.tests.testepistasis
     import fastlmm.association.tests.test_single_snp
     import fastlmm.association.tests.test_single_snp_linreg
     import fastlmm.association.tests.test_single_snp_select
@@ -145,47 +154,53 @@
     import fastlmm.association.tests.test_single_snp_scale
     import fastlmm.inference.tests.test_fastlmm_predictor
     import fastlmm.inference.tests.test_linear_regression
     import fastlmm.inference.tests.test
     import fastlmm.util.test
     import fastlmm.pyplink.test
 
-    suites = unittest.TestSuite([   # getDebugTestSuite(),
-
-                                    getTestSuiteX(),
-                                    fastlmm.inference.tests.test_linear_regression.getTestSuite(), 
-                                    fastlmm.association.tests.test_single_snp_scale.getTestSuite(), 
-                                    fastlmm.pyplink.test.getTestSuite(),
-                                    fastlmm.feature_selection.test.getTestSuite(),
-                                    fastlmm.association.tests.test_single_snp_select.getTestSuite(),
-                                    fastlmm.inference.tests.test_fastlmm_predictor.getTestSuite(),
-                                    fastlmm.association.tests.test_gwas.getTestSuite(),
-                                    fastlmm.association.tests.test_snp_set.getTestSuite(),
-                                    fastlmm.inference.tests.test.getTestSuite(),
-                                    fastlmm.association.tests.testepistasis.getTestSuite(),
-                                    fastlmm.association.tests.test_heritability_spatial_correction.getTestSuite(),
-                                    fastlmm.util.test.getTestSuite(),
-                                    fastlmm.association.tests.test_single_snp_all_plus_select.getTestSuite(),
-                                    fastlmm.inference.tests.test.getTestSuite(),
-                                    fastlmm.association.tests.test_single_snp.getTestSuite(),
-                                    fastlmm.association.tests.test_single_snp_linreg.getTestSuite(),
-                                    ])
+    suites = unittest.TestSuite(
+        [
+            # cmk
+            # for debugging getDebugTestSuite(),
+            getTestSuiteX(),
+            fastlmm.inference.tests.test_linear_regression.getTestSuite(),
+            fastlmm.association.tests.test_single_snp_scale.getTestSuite(),
+            fastlmm.pyplink.test.getTestSuite(),
+            fastlmm.feature_selection.test.getTestSuite(),
+            # this test is deprecated # fastlmm.association.tests.test_single_snp_select.getTestSuite(),
+            fastlmm.inference.tests.test_fastlmm_predictor.getTestSuite(),
+            fastlmm.association.tests.test_gwas.getTestSuite(),
+            fastlmm.association.tests.test_snp_set.getTestSuite(),
+            fastlmm.inference.tests.test.getTestSuite(),
+            fastlmm.association.tests.testepistasis.getTestSuite(),
+            fastlmm.association.tests.test_heritability_spatial_correction.getTestSuite(),
+            fastlmm.util.test.getTestSuite(),
+            fastlmm.association.tests.test_single_snp_all_plus_select.getTestSuite(),
+            fastlmm.inference.tests.test.getTestSuite(),
+            fastlmm.association.tests.test_single_snp.getTestSuite(),
+            fastlmm.association.tests.test_single_snp_linreg.getTestSuite(),
+        ]
+    )
 
     if True:  # Standard test run
-        r = unittest.TextTestRunner(failfast=False)
+        r = unittest.TextTestRunner(failfast=True)
         ret = r.run(suites)
         assert ret.wasSuccessful()
     else:  # Cluster test run
         # Because both pysnsptools and fastlmm contain a tests folder, to run on cluster must have fastlmm listed first in the PYTHONPATH
 
         runner = Local()
         runner = LocalMultiProc(taskcount=12, mkl_num_threads=5, just_one_process=False)
-        #runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
-        distributable_test = DistributableTest(suites,"temp_test")
+        # runner = LocalInParts(1,2,mkl_num_threads=1) # For debugging the cluster runs
+        distributable_test = DistributableTest(suites, "temp_test")
         runner.run(distributable_test)
 
-    debian_count = len(os.listdir('expected-debian'))
+    debian_count = len(os.listdir("expected-debian"))
     if debian_count > 0:
-        logging.warning("The tests contain {0} expected-results files that differ between Windows and Debian".format(debian_count))
-
+        logging.warning(
+            "The tests contain {0} expected-results files that differ between Windows and Debian".format(
+                debian_count
+            )
+        )
 
     logging.info("done with testing")
```

