# Comparing `tmp/cars-0.7.5.tar.gz` & `tmp/cars-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/work/CAMPUS/users/youssefd/Development/cars-master/dist/.tmp-cc8u5jzg/cars-0.7.5.tar", last modified: Thu Mar  7 17:01:21 2024, max compression
+gzip compressed data, was "/work/CAMPUS/users/youssefd/Development/cars-master/dist/.tmp-6es61qm_/cars-0.7.6.tar", last modified: Fri Apr 26 08:08:12 2024, max compression
```

## Comparing `cars-0.7.5.tar` & `cars-0.7.6.tar`

### file list

```diff
@@ -1,240 +1,244 @@
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:20.976757 cars-0.7.5/
--rw-------   0 youssefd  (7412) campus    (9585)       85 2021-09-29 14:51:03.000000 cars-0.7.5/.coveragerc
--rw-------   0 youssefd  (7412) campus    (9585)     1107 2022-10-07 19:31:52.000000 cars-0.7.5/.gitignore
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:00:56.147992 cars-0.7.5/.gitlab/
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:01.657170 cars-0.7.5/.gitlab/issue_templates/
--rw-------   0 youssefd  (7412) campus    (9585)     1009 2022-10-07 19:31:52.000000 cars-0.7.5/.gitlab/issue_templates/Bug.md
--rw-------   0 youssefd  (7412) campus    (9585)      442 2022-10-07 19:31:52.000000 cars-0.7.5/.gitlab/issue_templates/Proposal.md
--rw-------   0 youssefd  (7412) campus    (9585)     1821 2022-10-07 19:31:52.000000 cars-0.7.5/.gitlab/issue_templates/Refacto.md
--rw-------   0 youssefd  (7412) campus    (9585)      810 2022-10-07 19:31:52.000000 cars-0.7.5/.gitlab/issue_templates/Release.md
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:01.776262 cars-0.7.5/.gitlab/merge_request_templates/
--rw-------   0 youssefd  (7412) campus    (9585)     2345 2022-10-07 19:31:52.000000 cars-0.7.5/.gitlab/merge_request_templates/MR.md
--rw-------   0 youssefd  (7412) campus    (9585)      864 2023-06-02 19:05:31.000000 cars-0.7.5/.pre-commit-config.yaml
--rw-------   0 youssefd  (7412) campus    (9585)    16149 2023-06-05 15:54:23.000000 cars-0.7.5/.pylintrc
--rw-------   0 youssefd  (7412) campus    (9585)      547 2023-10-16 20:21:01.000000 cars-0.7.5/.readthedocs.yaml
--rw-------   0 youssefd  (7412) campus    (9585)     1719 2023-06-20 07:07:34.000000 cars-0.7.5/AUTHORS.md
--rw-------   0 youssefd  (7412) campus    (9585)    11577 2024-03-07 16:52:23.000000 cars-0.7.5/CHANGELOG.md
--rw-------   0 youssefd  (7412) campus    (9585)     4509 2023-03-10 14:58:43.000000 cars-0.7.5/CONTRIBUTING.md
--rw-------   0 youssefd  (7412) campus    (9585)      907 2023-01-02 09:39:32.000000 cars-0.7.5/Dockerfile
--rw-------   0 youssefd  (7412) campus    (9585)     3555 2024-02-15 14:48:18.000000 cars-0.7.5/Dockerfile.deps
--rw-------   0 youssefd  (7412) campus    (9585)      573 2023-08-16 11:31:21.000000 cars-0.7.5/Dockerfile.jupyter
--rw-------   0 youssefd  (7412) campus    (9585)    11358 2020-12-16 10:57:27.000000 cars-0.7.5/LICENSE
--rw-------   0 youssefd  (7412) campus    (9585)       38 2023-06-07 07:59:03.000000 cars-0.7.5/MANIFEST.in
--rw-------   0 youssefd  (7412) campus    (9585)    14375 2023-10-27 17:01:59.000000 cars-0.7.5/Makefile
--rw-------   0 youssefd  (7412) campus    (9585)     6950 2023-10-03 13:46:58.000000 cars-0.7.5/NOTICE
--rw-r--r--   0 youssefd  (7412) campus    (9585)     7990 2024-03-07 17:01:20.976391 cars-0.7.5/PKG-INFO
--rw-------   0 youssefd  (7412) campus    (9585)     4675 2023-10-27 17:01:59.000000 cars-0.7.5/README.md
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:02.171414 cars-0.7.5/cars/
--rw-------   0 youssefd  (7412) campus    (9585)     1670 2024-02-15 14:48:18.000000 cars-0.7.5/cars/__init__.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:03.213615 cars-0.7.5/cars/applications/
--rw-------   0 youssefd  (7412) campus    (9585)     1332 2023-10-03 13:46:58.000000 cars-0.7.5/cars/applications/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     2999 2022-11-30 10:16:57.000000 cars-0.7.5/cars/applications/application.py
--rw-------   0 youssefd  (7412) campus    (9585)      830 2022-10-07 19:31:52.000000 cars-0.7.5/cars/applications/application_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)     2726 2023-10-03 13:46:58.000000 cars-0.7.5/cars/applications/application_template.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:03.791704 cars-0.7.5/cars/applications/dem_generation/
--rw-------   0 youssefd  (7412) campus    (9585)      891 2023-10-03 13:46:58.000000 cars-0.7.5/cars/applications/dem_generation/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     3625 2024-02-01 07:18:04.000000 cars-0.7.5/cars/applications/dem_generation/dem_generation.py
--rw-------   0 youssefd  (7412) campus    (9585)      943 2024-02-01 07:18:04.000000 cars-0.7.5/cars/applications/dem_generation/dem_generation_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)     3461 2023-10-03 13:46:58.000000 cars-0.7.5/cars/applications/dem_generation/dem_generation_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)    17467 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/dem_generation/dichotomic_generation.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:04.475871 cars-0.7.5/cars/applications/dense_matches_filling/
--rw-------   0 youssefd  (7412) campus    (9585)      934 2023-10-03 13:46:58.000000 cars-0.7.5/cars/applications/dense_matches_filling/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     7744 2024-03-07 08:33:34.000000 cars-0.7.5/cars/applications/dense_matches_filling/dense_matches_filling.py
--rw-------   0 youssefd  (7412) campus    (9585)     1300 2023-02-22 08:13:12.000000 cars-0.7.5/cars/applications/dense_matches_filling/fill_disp_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    28779 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/dense_matches_filling/fill_disp_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)    18925 2024-03-07 08:33:34.000000 cars-0.7.5/cars/applications/dense_matches_filling/plane.py
--rw-------   0 youssefd  (7412) campus    (9585)     9094 2024-03-07 08:33:34.000000 cars-0.7.5/cars/applications/dense_matches_filling/zero_padding.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:05.132251 cars-0.7.5/cars/applications/dense_matching/
--rw-------   0 youssefd  (7412) campus    (9585)      898 2022-12-02 15:26:27.000000 cars-0.7.5/cars/applications/dense_matching/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    45278 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/dense_matching/census_mccnn_sgm.py
--rw-------   0 youssefd  (7412) campus    (9585)     8142 2023-12-06 08:28:57.000000 cars-0.7.5/cars/applications/dense_matching/dense_matching.py
--rw-------   0 youssefd  (7412) campus    (9585)     2688 2023-12-06 08:28:57.000000 cars-0.7.5/cars/applications/dense_matching/dense_matching_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    31588 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/dense_matching/dense_matching_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:05.474726 cars-0.7.5/cars/applications/dense_matching/loaders/
--rw-------   0 youssefd  (7412) campus    (9585)      770 2022-12-02 15:26:27.000000 cars-0.7.5/cars/applications/dense_matching/loaders/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)      901 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/dense_matching/loaders/config_census_sgm.json
--rw-------   0 youssefd  (7412) campus    (9585)      818 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/dense_matching/loaders/config_mccnn.json
--rw-------   0 youssefd  (7412) campus    (9585)     8502 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/dense_matching/loaders/pandora_loader.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:05.924359 cars-0.7.5/cars/applications/grid_generation/
--rw-------   0 youssefd  (7412) campus    (9585)      905 2022-12-02 15:26:27.000000 cars-0.7.5/cars/applications/grid_generation/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    10507 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/grid_generation/epipolar_grid_generation.py
--rw-------   0 youssefd  (7412) campus    (9585)     1503 2023-06-20 07:07:34.000000 cars-0.7.5/cars/applications/grid_generation/grid_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    17553 2023-12-06 08:28:57.000000 cars-0.7.5/cars/applications/grid_generation/grid_correction.py
--rw-------   0 youssefd  (7412) campus    (9585)     4010 2023-10-03 13:46:58.000000 cars-0.7.5/cars/applications/grid_generation/grid_generation.py
--rw-------   0 youssefd  (7412) campus    (9585)    10279 2023-12-06 08:28:57.000000 cars-0.7.5/cars/applications/grid_generation/grids.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:06.138947 cars-0.7.5/cars/applications/holes_detection/
--rw-------   0 youssefd  (7412) campus    (9585)      894 2022-12-02 15:26:27.000000 cars-0.7.5/cars/applications/holes_detection/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    11370 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/holes_detection/cloud_to_bbox.py
--rw-------   0 youssefd  (7412) campus    (9585)     4012 2023-10-03 13:46:58.000000 cars-0.7.5/cars/applications/holes_detection/holes_detection.py
--rw-------   0 youssefd  (7412) campus    (9585)     5512 2023-04-19 14:45:10.000000 cars-0.7.5/cars/applications/holes_detection/holes_detection_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:06.473548 cars-0.7.5/cars/applications/point_cloud_fusion/
--rw-------   0 youssefd  (7412) campus    (9585)      924 2022-12-02 15:26:27.000000 cars-0.7.5/cars/applications/point_cloud_fusion/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     1078 2022-12-02 15:26:27.000000 cars-0.7.5/cars/applications/point_cloud_fusion/cloud_fusion_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    20651 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/point_cloud_fusion/mapping_to_terrain_tiles.py
--rw-------   0 youssefd  (7412) campus    (9585)    38651 2024-02-01 07:18:04.000000 cars-0.7.5/cars/applications/point_cloud_fusion/pc_tif_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)     5058 2024-02-01 07:18:04.000000 cars-0.7.5/cars/applications/point_cloud_fusion/point_cloud_fusion.py
--rw-------   0 youssefd  (7412) campus    (9585)    30642 2024-02-01 07:18:04.000000 cars-0.7.5/cars/applications/point_cloud_fusion/point_cloud_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:07.110514 cars-0.7.5/cars/applications/point_cloud_outliers_removing/
--rw-------   0 youssefd  (7412) campus    (9585)      957 2022-12-02 15:26:27.000000 cars-0.7.5/cars/applications/point_cloud_outliers_removing/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    15683 2023-10-03 13:47:12.000000 cars-0.7.5/cars/applications/point_cloud_outliers_removing/outlier_removing_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)     6620 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/point_cloud_outliers_removing/pc_out_removing.py
--rw-------   0 youssefd  (7412) campus    (9585)     1298 2022-11-30 17:19:59.000000 cars-0.7.5/cars/applications/point_cloud_outliers_removing/points_removing_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    14299 2023-11-14 12:26:32.000000 cars-0.7.5/cars/applications/point_cloud_outliers_removing/small_components.py
--rw-------   0 youssefd  (7412) campus    (9585)    12864 2023-11-14 12:26:32.000000 cars-0.7.5/cars/applications/point_cloud_outliers_removing/statistical.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:07.630496 cars-0.7.5/cars/applications/rasterization/
--rw-------   0 youssefd  (7412) campus    (9585)      925 2022-12-02 15:26:27.000000 cars-0.7.5/cars/applications/rasterization/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     4817 2024-02-01 07:18:04.000000 cars-0.7.5/cars/applications/rasterization/point_cloud_rasterization.py
--rw-------   0 youssefd  (7412) campus    (9585)     1305 2023-03-21 16:35:08.000000 cars-0.7.5/cars/applications/rasterization/rasterization_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    25160 2024-03-07 08:33:34.000000 cars-0.7.5/cars/applications/rasterization/rasterization_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)    32723 2024-03-07 08:33:34.000000 cars-0.7.5/cars/applications/rasterization/simple_gaussian.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:08.129314 cars-0.7.5/cars/applications/resampling/
--rw-------   0 youssefd  (7412) campus    (9585)      885 2022-12-02 15:26:27.000000 cars-0.7.5/cars/applications/resampling/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    32660 2024-03-07 08:33:34.000000 cars-0.7.5/cars/applications/resampling/bicubic_resampling.py
--rw-------   0 youssefd  (7412) campus    (9585)     6272 2024-03-07 08:33:34.000000 cars-0.7.5/cars/applications/resampling/resampling.py
--rw-------   0 youssefd  (7412) campus    (9585)      906 2022-11-30 17:19:59.000000 cars-0.7.5/cars/applications/resampling/resampling_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    15096 2024-03-07 08:33:34.000000 cars-0.7.5/cars/applications/resampling/resampling_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:08.735423 cars-0.7.5/cars/applications/sparse_matching/
--rw-------   0 youssefd  (7412) campus    (9585)      883 2022-12-02 15:26:27.000000 cars-0.7.5/cars/applications/sparse_matching/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    30160 2024-03-07 08:33:34.000000 cars-0.7.5/cars/applications/sparse_matching/sift.py
--rw-------   0 youssefd  (7412) campus    (9585)     5413 2023-12-06 08:28:57.000000 cars-0.7.5/cars/applications/sparse_matching/sparse_matching.py
--rw-------   0 youssefd  (7412) campus    (9585)     2281 2023-06-20 07:07:34.000000 cars-0.7.5/cars/applications/sparse_matching/sparse_matching_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    15913 2024-03-07 08:33:34.000000 cars-0.7.5/cars/applications/sparse_matching/sparse_matching_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:09.332143 cars-0.7.5/cars/applications/triangulation/
--rw-------   0 youssefd  (7412) campus    (9585)      944 2022-10-07 19:31:52.000000 cars-0.7.5/cars/applications/triangulation/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    22291 2024-02-15 14:48:18.000000 cars-0.7.5/cars/applications/triangulation/line_of_sight_intersection.py
--rw-------   0 youssefd  (7412) campus    (9585)     7230 2024-02-01 07:18:04.000000 cars-0.7.5/cars/applications/triangulation/triangulation.py
--rw-------   0 youssefd  (7412) campus    (9585)     1017 2023-10-03 13:47:12.000000 cars-0.7.5/cars/applications/triangulation/triangulation_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    11910 2024-02-01 07:18:04.000000 cars-0.7.5/cars/applications/triangulation/triangulation_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)     5915 2024-02-15 14:48:18.000000 cars-0.7.5/cars/cars.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:09.700982 cars-0.7.5/cars/conf/
--rw-------   0 youssefd  (7412) campus    (9585)      754 2021-09-29 14:51:03.000000 cars-0.7.5/cars/conf/__init__.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:09.960307 cars-0.7.5/cars/conf/geoid/
--rw-------   0 youssefd  (7412) campus    (9585)  4155868 2021-09-29 14:51:03.000000 cars-0.7.5/cars/conf/geoid/egm96.grd
--rw-------   0 youssefd  (7412) campus    (9585)      454 2022-10-07 19:31:52.000000 cars-0.7.5/cars/conf/geoid/egm96.grd.hdr
--rw-------   0 youssefd  (7412) campus    (9585)     5042 2023-06-20 07:07:34.000000 cars-0.7.5/cars/conf/input_parameters.py
--rw-------   0 youssefd  (7412) campus    (9585)     1010 2023-02-22 08:13:12.000000 cars-0.7.5/cars/conf/mask_cst.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:11.840489 cars-0.7.5/cars/core/
--rw-------   0 youssefd  (7412) campus    (9585)      754 2021-09-29 14:51:03.000000 cars-0.7.5/cars/core/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     9894 2024-01-16 15:27:41.000000 cars-0.7.5/cars/core/cars_logging.py
--rw-------   0 youssefd  (7412) campus    (9585)     2918 2024-02-15 14:48:18.000000 cars-0.7.5/cars/core/constants.py
--rw-------   0 youssefd  (7412) campus    (9585)     1360 2023-12-06 08:28:57.000000 cars-0.7.5/cars/core/constants_disparity.py
--rw-------   0 youssefd  (7412) campus    (9585)     4204 2023-10-27 17:01:59.000000 cars-0.7.5/cars/core/datasets.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:12.482835 cars-0.7.5/cars/core/geometry/
--rw-------   0 youssefd  (7412) campus    (9585)      847 2023-10-03 13:46:58.000000 cars-0.7.5/cars/core/geometry/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    22386 2023-12-06 08:28:57.000000 cars-0.7.5/cars/core/geometry/abstract_geometry.py
--rw-------   0 youssefd  (7412) campus    (9585)    20965 2023-12-06 08:28:57.000000 cars-0.7.5/cars/core/geometry/otb_geometry.py
--rw-------   0 youssefd  (7412) campus    (9585)    16133 2024-02-15 14:48:18.000000 cars-0.7.5/cars/core/geometry/shareloc_geometry.py
--rw-------   0 youssefd  (7412) campus    (9585)    10275 2023-12-06 08:28:57.000000 cars-0.7.5/cars/core/inputs.py
--rw-------   0 youssefd  (7412) campus    (9585)     3476 2023-06-20 07:07:34.000000 cars-0.7.5/cars/core/otb_adapters.py
--rw-------   0 youssefd  (7412) campus    (9585)     5438 2024-03-07 08:33:34.000000 cars-0.7.5/cars/core/outputs.py
--rw-------   0 youssefd  (7412) campus    (9585)    20858 2024-02-01 07:18:04.000000 cars-0.7.5/cars/core/preprocessing.py
--rw-------   0 youssefd  (7412) campus    (9585)    25636 2024-01-11 08:25:08.000000 cars-0.7.5/cars/core/projection.py
--rw-------   0 youssefd  (7412) campus    (9585)     5693 2023-10-03 13:46:59.000000 cars-0.7.5/cars/core/roi_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)    24216 2024-03-07 08:33:34.000000 cars-0.7.5/cars/core/tiling.py
--rw-------   0 youssefd  (7412) campus    (9585)     4944 2022-11-22 10:23:47.000000 cars-0.7.5/cars/core/utils.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:13.094062 cars-0.7.5/cars/data_structures/
--rw-------   0 youssefd  (7412) campus    (9585)      765 2022-10-07 19:31:52.000000 cars-0.7.5/cars/data_structures/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    42218 2024-02-15 14:48:18.000000 cars-0.7.5/cars/data_structures/cars_dataset.py
--rw-------   0 youssefd  (7412) campus    (9585)     1857 2023-03-10 14:57:03.000000 cars-0.7.5/cars/data_structures/cars_dict.py
--rw-------   0 youssefd  (7412) campus    (9585)     9741 2024-02-15 14:48:18.000000 cars-0.7.5/cars/data_structures/corresponding_tiles_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)     6285 2023-12-06 08:28:57.000000 cars-0.7.5/cars/data_structures/dataframe_converter.py
--rw-------   0 youssefd  (7412) campus    (9585)     7442 2023-12-06 08:28:57.000000 cars-0.7.5/cars/data_structures/format_transformation.py
--rw-------   0 youssefd  (7412) campus    (9585)     3952 2024-02-01 07:18:04.000000 cars-0.7.5/cars/extractroi.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:13.662992 cars-0.7.5/cars/orchestrator/
--rw-------   0 youssefd  (7412) campus    (9585)      762 2022-10-07 19:31:52.000000 cars-0.7.5/cars/orchestrator/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     3122 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/achievement_tracker.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:14.705535 cars-0.7.5/cars/orchestrator/cluster/
--rw-------   0 youssefd  (7412) campus    (9585)     1045 2023-10-18 06:44:29.000000 cars-0.7.5/cars/orchestrator/cluster/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     6219 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/cluster/abstract_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)    10946 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/cluster/abstract_dask_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)     2919 2024-01-16 15:27:41.000000 cars-0.7.5/cars/orchestrator/cluster/dask_cluster_tools.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:14.930149 cars-0.7.5/cars/orchestrator/cluster/dask_config/
--rw-------   0 youssefd  (7412) campus    (9585)     7009 2023-01-02 09:39:32.000000 cars-0.7.5/cars/orchestrator/cluster/dask_config/README.md
--rw-------   0 youssefd  (7412) campus    (9585)     1016 2023-01-02 09:39:32.000000 cars-0.7.5/cars/orchestrator/cluster/dask_config/dask.yaml
--rw-------   0 youssefd  (7412) campus    (9585)     3120 2023-06-20 07:07:34.000000 cars-0.7.5/cars/orchestrator/cluster/dask_config/distributed.yaml
--rw-------   0 youssefd  (7412) campus    (9585)     1427 2023-01-02 09:39:32.000000 cars-0.7.5/cars/orchestrator/cluster/dask_config/jobqueue.yaml
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:15.228963 cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/
--rw-------   0 youssefd  (7412) campus    (9585)     4711 2023-01-02 09:39:32.000000 cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/dask-schema.yaml
--rw-------   0 youssefd  (7412) campus    (9585)      989 2023-01-02 09:39:32.000000 cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/dask.yaml
--rw-------   0 youssefd  (7412) campus    (9585)    38310 2023-01-02 09:39:32.000000 cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/distributed-schema.yaml
--rw-------   0 youssefd  (7412) campus    (9585)    11637 2023-02-22 08:13:13.000000 cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/distributed.yaml
--rw-------   0 youssefd  (7412) campus    (9585)     7566 2023-01-02 09:39:32.000000 cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/jobqueue.yaml
--rw-------   0 youssefd  (7412) campus    (9585)     6619 2023-10-03 13:46:59.000000 cars-0.7.5/cars/orchestrator/cluster/dask_jobqueue_utils.py
--rw-------   0 youssefd  (7412) campus    (9585)     3018 2023-10-18 06:44:29.000000 cars-0.7.5/cars/orchestrator/cluster/local_dask_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)    24392 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/cluster/log_wrapper.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:15.820969 cars-0.7.5/cars/orchestrator/cluster/mp_cluster/
--rw-------   0 youssefd  (7412) campus    (9585)      834 2023-03-21 16:35:08.000000 cars-0.7.5/cars/orchestrator/cluster/mp_cluster/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     6317 2023-10-03 13:47:12.000000 cars-0.7.5/cars/orchestrator/cluster/mp_cluster/mp_factorizer.py
--rw-------   0 youssefd  (7412) campus    (9585)    14531 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/cluster/mp_cluster/mp_objects.py
--rw-------   0 youssefd  (7412) campus    (9585)     3090 2023-10-03 13:47:12.000000 cars-0.7.5/cars/orchestrator/cluster/mp_cluster/mp_tools.py
--rw-------   0 youssefd  (7412) campus    (9585)    10298 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/cluster/mp_cluster/mp_wrapper.py
--rw-------   0 youssefd  (7412) campus    (9585)    25350 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/cluster/mp_cluster/multiprocessing_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)     5786 2023-10-18 06:44:29.000000 cars-0.7.5/cars/orchestrator/cluster/pbs_dask_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)     3386 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/cluster/sequential_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)     7033 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/cluster/slurm_dask_cluster.py
--rw-------   0 youssefd  (7412) campus    (9585)    17543 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/orchestrator.py
--rw-------   0 youssefd  (7412) campus    (9585)      894 2022-10-07 19:31:52.000000 cars-0.7.5/cars/orchestrator/orchestrator_constants.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:16.477510 cars-0.7.5/cars/orchestrator/registry/
--rw-------   0 youssefd  (7412) campus    (9585)      758 2022-10-07 19:31:52.000000 cars-0.7.5/cars/orchestrator/registry/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     4002 2024-02-15 14:48:18.000000 cars-0.7.5/cars/orchestrator/registry/abstract_registry.py
--rw-------   0 youssefd  (7412) campus    (9585)     3090 2022-10-07 19:31:52.000000 cars-0.7.5/cars/orchestrator/registry/id_generator.py
--rw-------   0 youssefd  (7412) campus    (9585)     6074 2024-03-07 08:33:34.000000 cars-0.7.5/cars/orchestrator/registry/replacer_registry.py
--rw-------   0 youssefd  (7412) campus    (9585)    12683 2024-02-15 14:48:18.000000 cars-0.7.5/cars/orchestrator/registry/saver_registry.py
--rw-------   0 youssefd  (7412) campus    (9585)     3234 2024-02-01 07:18:04.000000 cars-0.7.5/cars/orchestrator/registry/unseen_registry.py
--rw-------   0 youssefd  (7412) campus    (9585)     7600 2024-02-15 14:48:18.000000 cars-0.7.5/cars/orchestrator/tiles_profiler.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:16.991796 cars-0.7.5/cars/pipelines/
--rw-------   0 youssefd  (7412) campus    (9585)      973 2023-03-10 14:57:03.000000 cars-0.7.5/cars/pipelines/__init__.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:17.619010 cars-0.7.5/cars/pipelines/conf_pipeline/
--rw-------   0 youssefd  (7412) campus    (9585)      765 2022-11-02 08:44:18.000000 cars-0.7.5/cars/pipelines/conf_pipeline/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)        8 2023-03-10 14:57:03.000000 cars-0.7.5/cars/pipelines/conf_pipeline/point_clouds_to_dsm.json
--rw-------   0 youssefd  (7412) campus    (9585)       13 2023-03-10 14:57:03.000000 cars-0.7.5/cars/pipelines/conf_pipeline/sensor_to_dense_dsm.json
--rw-------   0 youssefd  (7412) campus    (9585)      158 2023-03-10 14:57:03.000000 cars-0.7.5/cars/pipelines/conf_pipeline/sensor_to_pc.json
--rw-------   0 youssefd  (7412) campus    (9585)      223 2023-06-05 15:54:23.000000 cars-0.7.5/cars/pipelines/conf_pipeline/sensor_to_sparse_dsm.json
--rw-------   0 youssefd  (7412) campus    (9585)     3445 2023-03-10 14:57:03.000000 cars-0.7.5/cars/pipelines/pipeline.py
--rw-------   0 youssefd  (7412) campus    (9585)      956 2023-10-03 13:46:59.000000 cars-0.7.5/cars/pipelines/pipeline_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)     4273 2023-10-03 13:46:59.000000 cars-0.7.5/cars/pipelines/pipeline_template.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:18.066642 cars-0.7.5/cars/pipelines/point_clouds_to_dsm/
--rw-------   0 youssefd  (7412) campus    (9585)      892 2023-03-10 14:57:03.000000 cars-0.7.5/cars/pipelines/point_clouds_to_dsm/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)      822 2023-03-10 14:57:03.000000 cars-0.7.5/cars/pipelines/point_clouds_to_dsm/pc_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    10299 2024-02-01 07:18:04.000000 cars-0.7.5/cars/pipelines/point_clouds_to_dsm/pc_inputs.py
--rw-------   0 youssefd  (7412) campus    (9585)    16404 2024-02-01 07:18:04.000000 cars-0.7.5/cars/pipelines/point_clouds_to_dsm/point_cloud_to_dsm_pipeline.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:18.828921 cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/
--rw-------   0 youssefd  (7412) campus    (9585)      893 2023-03-10 14:57:03.000000 cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)     2225 2023-03-10 14:57:03.000000 cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/dsm_output.py
--rw-------   0 youssefd  (7412) campus    (9585)     1711 2024-02-01 07:18:04.000000 cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/sensor_dense_dsm_constants.py
--rw-------   0 youssefd  (7412) campus    (9585)    56062 2024-03-07 08:33:34.000000 cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/sensor_to_dense_dsm_pipeline.py
--rw-------   0 youssefd  (7412) campus    (9585)    23728 2024-03-07 08:33:34.000000 cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/sensors_inputs.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:19.081313 cars-0.7.5/cars/pipelines/sensor_to_sparse_dsm/
--rw-------   0 youssefd  (7412) campus    (9585)      895 2023-03-10 14:57:03.000000 cars-0.7.5/cars/pipelines/sensor_to_sparse_dsm/__init__.py
--rw-------   0 youssefd  (7412) campus    (9585)    24316 2024-03-07 08:33:34.000000 cars-0.7.5/cars/pipelines/sensor_to_sparse_dsm/sensor_to_sparse_dsm_pipeline.py
--rw-------   0 youssefd  (7412) campus    (9585)     4437 2024-01-11 08:32:35.000000 cars-0.7.5/cars/starter.py
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:20.834020 cars-0.7.5/cars.egg-info/
--rw-r--r--   0 youssefd  (7412) campus    (9585)     7990 2024-03-07 17:00:53.000000 cars-0.7.5/cars.egg-info/PKG-INFO
--rw-------   0 youssefd  (7412) campus    (9585)     8448 2024-03-07 17:00:55.000000 cars-0.7.5/cars.egg-info/SOURCES.txt
--rw-------   0 youssefd  (7412) campus    (9585)        1 2024-03-07 17:00:53.000000 cars-0.7.5/cars.egg-info/dependency_links.txt
--rw-------   0 youssefd  (7412) campus    (9585)      167 2024-03-07 17:00:54.000000 cars-0.7.5/cars.egg-info/entry_points.txt
--rw-------   0 youssefd  (7412) campus    (9585)      854 2024-03-07 17:00:54.000000 cars-0.7.5/cars.egg-info/requires.txt
--rw-------   0 youssefd  (7412) campus    (9585)       11 2024-03-07 17:00:54.000000 cars-0.7.5/cars.egg-info/top_level.txt
--rwx------   0 youssefd  (7412) campus    (9585)     2254 2023-01-02 09:39:32.000000 cars-0.7.5/env_cars.sh
--rw-------   0 youssefd  (7412) campus    (9585)     2771 2023-07-05 16:15:54.000000 cars-0.7.5/gdal-config
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:19.270452 cars-0.7.5/otb_remote_module/
--rw-------   0 youssefd  (7412) campus    (9585)      374 2023-03-21 16:35:08.000000 cars-0.7.5/otb_remote_module/CMakeLists.txt
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:19.761033 cars-0.7.5/otb_remote_module/app/
--rw-------   0 youssefd  (7412) campus    (9585)      543 2023-12-06 08:28:57.000000 cars-0.7.5/otb_remote_module/app/CMakeLists.txt
--rw-------   0 youssefd  (7412) campus    (9585)     9637 2023-10-03 13:47:12.000000 cars-0.7.5/otb_remote_module/app/otbConvertSensorToGeoMultiPointFast.cxx
--rw-------   0 youssefd  (7412) campus    (9585)     7228 2023-02-27 10:57:22.000000 cars-0.7.5/otb_remote_module/app/otbEpipolarTriangulation.cxx
--rw-------   0 youssefd  (7412) campus    (9585)     8596 2023-12-06 08:28:57.000000 cars-0.7.5/otb_remote_module/app/otbLocalizeInverse.cxx
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:20.384785 cars-0.7.5/otb_remote_module/data/
--rw-------   0 youssefd  (7412) campus    (9585)   323046 2020-12-16 10:57:27.000000 cars-0.7.5/otb_remote_module/data/rectified_ref.tif
--rw-------   0 youssefd  (7412) campus    (9585)    81136 2020-12-16 10:57:27.000000 cars-0.7.5/otb_remote_module/data/rectified_ref_mask.tif
--rw-------   0 youssefd  (7412) campus    (9585)   322610 2020-12-16 10:57:27.000000 cars-0.7.5/otb_remote_module/data/rectified_sec.tif
--rw-------   0 youssefd  (7412) campus    (9585)    75835 2020-12-16 10:57:27.000000 cars-0.7.5/otb_remote_module/data/rectified_sec_mask.tif
-drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-03-07 17:01:20.726873 cars-0.7.5/otb_remote_module/include/
--rw-------   0 youssefd  (7412) campus    (9585)    13784 2023-02-27 10:57:22.000000 cars-0.7.5/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.h
--rw-------   0 youssefd  (7412) campus    (9585)    13094 2023-02-27 10:57:22.000000 cars-0.7.5/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.hxx
--rw-------   0 youssefd  (7412) campus    (9585)      506 2020-12-16 10:57:27.000000 cars-0.7.5/otb_remote_module/otb-module.cmake
--rw-------   0 youssefd  (7412) campus    (9585)      407 2022-10-07 19:31:52.000000 cars-0.7.5/pyproject.toml
--rw-------   0 youssefd  (7412) campus    (9585)      316 2023-08-16 11:31:21.000000 cars-0.7.5/pytest.ini
--rw-------   0 youssefd  (7412) campus    (9585)     3268 2024-03-07 17:01:20.977882 cars-0.7.5/setup.cfg
--rw-------   0 youssefd  (7412) campus    (9585)     1084 2023-06-07 07:59:04.000000 cars-0.7.5/setup.py
--rw-------   0 youssefd  (7412) campus    (9585)     1527 2024-02-01 07:18:04.000000 cars-0.7.5/sonar-project.properties
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.779028 cars-0.7.6/
+-rw-------   0 youssefd  (7412) campus    (9585)       85 2021-09-29 14:51:03.000000 cars-0.7.6/.coveragerc
+-rw-------   0 youssefd  (7412) campus    (9585)     1107 2022-10-07 19:31:52.000000 cars-0.7.6/.gitignore
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.558178 cars-0.7.6/.gitlab/
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.587892 cars-0.7.6/.gitlab/issue_templates/
+-rw-------   0 youssefd  (7412) campus    (9585)     1009 2022-10-07 19:31:52.000000 cars-0.7.6/.gitlab/issue_templates/Bug.md
+-rw-------   0 youssefd  (7412) campus    (9585)      442 2022-10-07 19:31:52.000000 cars-0.7.6/.gitlab/issue_templates/Proposal.md
+-rw-------   0 youssefd  (7412) campus    (9585)     1821 2022-10-07 19:31:52.000000 cars-0.7.6/.gitlab/issue_templates/Refacto.md
+-rw-------   0 youssefd  (7412) campus    (9585)      810 2022-10-07 19:31:52.000000 cars-0.7.6/.gitlab/issue_templates/Release.md
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.588533 cars-0.7.6/.gitlab/merge_request_templates/
+-rw-------   0 youssefd  (7412) campus    (9585)     2345 2022-10-07 19:31:52.000000 cars-0.7.6/.gitlab/merge_request_templates/MR.md
+-rw-------   0 youssefd  (7412) campus    (9585)      864 2023-06-02 19:05:31.000000 cars-0.7.6/.pre-commit-config.yaml
+-rw-------   0 youssefd  (7412) campus    (9585)    16149 2023-06-05 15:54:23.000000 cars-0.7.6/.pylintrc
+-rw-------   0 youssefd  (7412) campus    (9585)      547 2023-10-16 20:21:01.000000 cars-0.7.6/.readthedocs.yaml
+-rw-------   0 youssefd  (7412) campus    (9585)     1719 2023-06-20 07:07:34.000000 cars-0.7.6/AUTHORS.md
+-rw-------   0 youssefd  (7412) campus    (9585)    12515 2024-04-26 07:37:46.000000 cars-0.7.6/CHANGELOG.md
+-rw-------   0 youssefd  (7412) campus    (9585)     4509 2023-03-10 14:58:43.000000 cars-0.7.6/CONTRIBUTING.md
+-rw-------   0 youssefd  (7412) campus    (9585)      907 2023-01-02 09:39:32.000000 cars-0.7.6/Dockerfile
+-rw-------   0 youssefd  (7412) campus    (9585)     3555 2024-02-15 14:48:18.000000 cars-0.7.6/Dockerfile.deps
+-rw-------   0 youssefd  (7412) campus    (9585)      573 2023-08-16 11:31:21.000000 cars-0.7.6/Dockerfile.jupyter
+-rw-------   0 youssefd  (7412) campus    (9585)    11358 2020-12-16 10:57:27.000000 cars-0.7.6/LICENSE
+-rw-------   0 youssefd  (7412) campus    (9585)       38 2023-06-07 07:59:03.000000 cars-0.7.6/MANIFEST.in
+-rw-------   0 youssefd  (7412) campus    (9585)    14375 2023-10-27 17:01:59.000000 cars-0.7.6/Makefile
+-rw-------   0 youssefd  (7412) campus    (9585)     6950 2023-10-03 13:46:58.000000 cars-0.7.6/NOTICE
+-rw-r--r--   0 youssefd  (7412) campus    (9585)     8274 2024-04-26 08:08:12.778704 cars-0.7.6/PKG-INFO
+-rw-------   0 youssefd  (7412) campus    (9585)     4961 2024-03-19 07:37:31.000000 cars-0.7.6/README.md
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.590727 cars-0.7.6/cars/
+-rw-------   0 youssefd  (7412) campus    (9585)     1670 2024-02-15 14:48:18.000000 cars-0.7.6/cars/__init__.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.596693 cars-0.7.6/cars/applications/
+-rw-------   0 youssefd  (7412) campus    (9585)     1382 2024-04-26 07:37:46.000000 cars-0.7.6/cars/applications/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3023 2024-04-26 07:37:46.000000 cars-0.7.6/cars/applications/application.py
+-rw-------   0 youssefd  (7412) campus    (9585)      830 2022-10-07 19:31:52.000000 cars-0.7.6/cars/applications/application_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)     2726 2023-10-03 13:46:58.000000 cars-0.7.6/cars/applications/application_template.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.599534 cars-0.7.6/cars/applications/dem_generation/
+-rw-------   0 youssefd  (7412) campus    (9585)      891 2023-10-03 13:46:58.000000 cars-0.7.6/cars/applications/dem_generation/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3625 2024-02-01 07:18:04.000000 cars-0.7.6/cars/applications/dem_generation/dem_generation.py
+-rw-------   0 youssefd  (7412) campus    (9585)      943 2024-02-01 07:18:04.000000 cars-0.7.6/cars/applications/dem_generation/dem_generation_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3461 2023-10-03 13:46:58.000000 cars-0.7.6/cars/applications/dem_generation/dem_generation_tools.py
+-rw-------   0 youssefd  (7412) campus    (9585)    17967 2024-04-26 07:37:46.000000 cars-0.7.6/cars/applications/dem_generation/dichotomic_generation.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.603751 cars-0.7.6/cars/applications/dense_matches_filling/
+-rw-------   0 youssefd  (7412) campus    (9585)      934 2023-10-03 13:46:58.000000 cars-0.7.6/cars/applications/dense_matches_filling/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     7828 2024-03-27 10:20:35.000000 cars-0.7.6/cars/applications/dense_matches_filling/dense_matches_filling.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1300 2023-02-22 08:13:12.000000 cars-0.7.6/cars/applications/dense_matches_filling/fill_disp_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    28779 2024-03-19 07:37:31.000000 cars-0.7.6/cars/applications/dense_matches_filling/fill_disp_tools.py
+-rw-------   0 youssefd  (7412) campus    (9585)    18925 2024-03-07 08:33:34.000000 cars-0.7.6/cars/applications/dense_matches_filling/plane.py
+-rw-------   0 youssefd  (7412) campus    (9585)     9094 2024-03-07 08:33:34.000000 cars-0.7.6/cars/applications/dense_matches_filling/zero_padding.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.607173 cars-0.7.6/cars/applications/dense_matching/
+-rw-------   0 youssefd  (7412) campus    (9585)      898 2022-12-02 15:26:27.000000 cars-0.7.6/cars/applications/dense_matching/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)    45825 2024-04-26 07:37:46.000000 cars-0.7.6/cars/applications/dense_matching/census_mccnn_sgm.py
+-rw-------   0 youssefd  (7412) campus    (9585)     8142 2023-12-06 08:28:57.000000 cars-0.7.6/cars/applications/dense_matching/dense_matching.py
+-rw-------   0 youssefd  (7412) campus    (9585)     2738 2024-03-27 10:20:35.000000 cars-0.7.6/cars/applications/dense_matching/dense_matching_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    31588 2024-02-15 14:48:18.000000 cars-0.7.6/cars/applications/dense_matching/dense_matching_tools.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.609778 cars-0.7.6/cars/applications/dense_matching/loaders/
+-rw-------   0 youssefd  (7412) campus    (9585)      770 2022-12-02 15:26:27.000000 cars-0.7.6/cars/applications/dense_matching/loaders/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)      901 2024-02-15 14:48:18.000000 cars-0.7.6/cars/applications/dense_matching/loaders/config_census_sgm.json
+-rw-------   0 youssefd  (7412) campus    (9585)      818 2024-02-15 14:48:18.000000 cars-0.7.6/cars/applications/dense_matching/loaders/config_mccnn.json
+-rw-------   0 youssefd  (7412) campus    (9585)    11050 2024-04-26 07:37:46.000000 cars-0.7.6/cars/applications/dense_matching/loaders/pandora_loader.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.613899 cars-0.7.6/cars/applications/grid_generation/
+-rw-------   0 youssefd  (7412) campus    (9585)      905 2022-12-02 15:26:27.000000 cars-0.7.6/cars/applications/grid_generation/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)    10507 2024-02-15 14:48:18.000000 cars-0.7.6/cars/applications/grid_generation/epipolar_grid_generation.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1503 2023-06-20 07:07:34.000000 cars-0.7.6/cars/applications/grid_generation/grid_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    17553 2023-12-06 08:28:57.000000 cars-0.7.6/cars/applications/grid_generation/grid_correction.py
+-rw-------   0 youssefd  (7412) campus    (9585)     4010 2023-10-03 13:46:58.000000 cars-0.7.6/cars/applications/grid_generation/grid_generation.py
+-rw-------   0 youssefd  (7412) campus    (9585)    10279 2023-12-06 08:28:57.000000 cars-0.7.6/cars/applications/grid_generation/grids.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.616661 cars-0.7.6/cars/applications/holes_detection/
+-rw-------   0 youssefd  (7412) campus    (9585)      894 2022-12-02 15:26:27.000000 cars-0.7.6/cars/applications/holes_detection/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)    11370 2024-02-15 14:48:18.000000 cars-0.7.6/cars/applications/holes_detection/cloud_to_bbox.py
+-rw-------   0 youssefd  (7412) campus    (9585)     4012 2023-10-03 13:46:58.000000 cars-0.7.6/cars/applications/holes_detection/holes_detection.py
+-rw-------   0 youssefd  (7412) campus    (9585)     5512 2023-04-19 14:45:10.000000 cars-0.7.6/cars/applications/holes_detection/holes_detection_tools.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.617823 cars-0.7.6/cars/applications/point_cloud_denoising/
+-rw-------   0 youssefd  (7412) campus    (9585)      952 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/point_cloud_denoising/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     7794 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/point_cloud_denoising/point_cloud_denoising.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.621515 cars-0.7.6/cars/applications/point_cloud_fusion/
+-rw-------   0 youssefd  (7412) campus    (9585)      924 2022-12-02 15:26:27.000000 cars-0.7.6/cars/applications/point_cloud_fusion/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1078 2022-12-02 15:26:27.000000 cars-0.7.6/cars/applications/point_cloud_fusion/cloud_fusion_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    21687 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/point_cloud_fusion/mapping_to_terrain_tiles.py
+-rw-------   0 youssefd  (7412) campus    (9585)    38651 2024-02-01 07:18:04.000000 cars-0.7.6/cars/applications/point_cloud_fusion/pc_tif_tools.py
+-rw-------   0 youssefd  (7412) campus    (9585)     5093 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/point_cloud_fusion/point_cloud_fusion.py
+-rw-------   0 youssefd  (7412) campus    (9585)    31854 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/point_cloud_fusion/point_cloud_tools.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.625104 cars-0.7.6/cars/applications/point_cloud_outliers_removing/
+-rw-------   0 youssefd  (7412) campus    (9585)      957 2022-12-02 15:26:27.000000 cars-0.7.6/cars/applications/point_cloud_outliers_removing/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)    15683 2023-10-03 13:47:12.000000 cars-0.7.6/cars/applications/point_cloud_outliers_removing/outlier_removing_tools.py
+-rw-------   0 youssefd  (7412) campus    (9585)     6641 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/point_cloud_outliers_removing/pc_out_removing.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1298 2022-11-30 17:19:59.000000 cars-0.7.6/cars/applications/point_cloud_outliers_removing/points_removing_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    15095 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/point_cloud_outliers_removing/small_components.py
+-rw-------   0 youssefd  (7412) campus    (9585)    13660 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/point_cloud_outliers_removing/statistical.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.628222 cars-0.7.6/cars/applications/rasterization/
+-rw-------   0 youssefd  (7412) campus    (9585)      925 2022-12-02 15:26:27.000000 cars-0.7.6/cars/applications/rasterization/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     4817 2024-02-01 07:18:04.000000 cars-0.7.6/cars/applications/rasterization/point_cloud_rasterization.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1665 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/rasterization/rasterization_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    26195 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/rasterization/rasterization_tools.py
+-rw-------   0 youssefd  (7412) campus    (9585)    39290 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/rasterization/simple_gaussian.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.631632 cars-0.7.6/cars/applications/resampling/
+-rw-------   0 youssefd  (7412) campus    (9585)      885 2022-12-02 15:26:27.000000 cars-0.7.6/cars/applications/resampling/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)    33077 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/resampling/bicubic_resampling.py
+-rw-------   0 youssefd  (7412) campus    (9585)     6272 2024-03-07 08:33:34.000000 cars-0.7.6/cars/applications/resampling/resampling.py
+-rw-------   0 youssefd  (7412) campus    (9585)      906 2022-11-30 17:19:59.000000 cars-0.7.6/cars/applications/resampling/resampling_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    15096 2024-03-07 08:33:34.000000 cars-0.7.6/cars/applications/resampling/resampling_tools.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.635073 cars-0.7.6/cars/applications/sparse_matching/
+-rw-------   0 youssefd  (7412) campus    (9585)      883 2022-12-02 15:26:27.000000 cars-0.7.6/cars/applications/sparse_matching/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)    30160 2024-03-07 08:33:34.000000 cars-0.7.6/cars/applications/sparse_matching/sift.py
+-rw-------   0 youssefd  (7412) campus    (9585)     5413 2023-12-06 08:28:57.000000 cars-0.7.6/cars/applications/sparse_matching/sparse_matching.py
+-rw-------   0 youssefd  (7412) campus    (9585)     2281 2023-06-20 07:07:34.000000 cars-0.7.6/cars/applications/sparse_matching/sparse_matching_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    15913 2024-03-07 08:33:34.000000 cars-0.7.6/cars/applications/sparse_matching/sparse_matching_tools.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.638450 cars-0.7.6/cars/applications/triangulation/
+-rw-------   0 youssefd  (7412) campus    (9585)      944 2022-10-07 19:31:52.000000 cars-0.7.6/cars/applications/triangulation/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)    25892 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/triangulation/line_of_sight_intersection.py
+-rw-------   0 youssefd  (7412) campus    (9585)     7536 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/triangulation/triangulation.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1017 2023-10-03 13:47:12.000000 cars-0.7.6/cars/applications/triangulation/triangulation_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    12369 2024-04-26 07:37:47.000000 cars-0.7.6/cars/applications/triangulation/triangulation_tools.py
+-rw-------   0 youssefd  (7412) campus    (9585)     5915 2024-02-15 14:48:18.000000 cars-0.7.6/cars/cars.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.640414 cars-0.7.6/cars/conf/
+-rw-------   0 youssefd  (7412) campus    (9585)      754 2021-09-29 14:51:03.000000 cars-0.7.6/cars/conf/__init__.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.666516 cars-0.7.6/cars/conf/geoid/
+-rw-------   0 youssefd  (7412) campus    (9585)  4155868 2021-09-29 14:51:03.000000 cars-0.7.6/cars/conf/geoid/egm96.grd
+-rw-------   0 youssefd  (7412) campus    (9585)      454 2022-10-07 19:31:52.000000 cars-0.7.6/cars/conf/geoid/egm96.grd.hdr
+-rw-------   0 youssefd  (7412) campus    (9585)     5042 2023-06-20 07:07:34.000000 cars-0.7.6/cars/conf/input_parameters.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1010 2023-02-22 08:13:12.000000 cars-0.7.6/cars/conf/mask_cst.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.675251 cars-0.7.6/cars/core/
+-rw-------   0 youssefd  (7412) campus    (9585)      754 2021-09-29 14:51:03.000000 cars-0.7.6/cars/core/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     9894 2024-01-16 15:27:41.000000 cars-0.7.6/cars/core/cars_logging.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3268 2024-04-26 07:37:47.000000 cars-0.7.6/cars/core/constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1537 2024-04-26 07:37:47.000000 cars-0.7.6/cars/core/constants_disparity.py
+-rw-------   0 youssefd  (7412) campus    (9585)     4204 2023-10-27 17:01:59.000000 cars-0.7.6/cars/core/datasets.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.678011 cars-0.7.6/cars/core/geometry/
+-rw-------   0 youssefd  (7412) campus    (9585)      847 2023-10-03 13:46:58.000000 cars-0.7.6/cars/core/geometry/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)    24921 2024-04-26 07:37:47.000000 cars-0.7.6/cars/core/geometry/abstract_geometry.py
+-rw-------   0 youssefd  (7412) campus    (9585)    21240 2024-04-26 07:37:47.000000 cars-0.7.6/cars/core/geometry/otb_geometry.py
+-rw-------   0 youssefd  (7412) campus    (9585)    17044 2024-04-26 07:37:47.000000 cars-0.7.6/cars/core/geometry/shareloc_geometry.py
+-rw-------   0 youssefd  (7412) campus    (9585)    10723 2024-04-26 07:37:47.000000 cars-0.7.6/cars/core/inputs.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3476 2023-06-20 07:07:34.000000 cars-0.7.6/cars/core/otb_adapters.py
+-rw-------   0 youssefd  (7412) campus    (9585)     5438 2024-03-07 08:33:34.000000 cars-0.7.6/cars/core/outputs.py
+-rw-------   0 youssefd  (7412) campus    (9585)    20858 2024-02-01 07:18:04.000000 cars-0.7.6/cars/core/preprocessing.py
+-rw-------   0 youssefd  (7412) campus    (9585)    25636 2024-01-11 08:25:08.000000 cars-0.7.6/cars/core/projection.py
+-rw-------   0 youssefd  (7412) campus    (9585)     6110 2024-04-26 07:37:47.000000 cars-0.7.6/cars/core/roi_tools.py
+-rw-------   0 youssefd  (7412) campus    (9585)    24216 2024-03-07 08:33:34.000000 cars-0.7.6/cars/core/tiling.py
+-rw-------   0 youssefd  (7412) campus    (9585)     4944 2022-11-22 10:23:47.000000 cars-0.7.6/cars/core/utils.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.681474 cars-0.7.6/cars/data_structures/
+-rw-------   0 youssefd  (7412) campus    (9585)      765 2022-10-07 19:31:52.000000 cars-0.7.6/cars/data_structures/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)    42102 2024-04-26 07:37:47.000000 cars-0.7.6/cars/data_structures/cars_dataset.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1857 2023-03-10 14:57:03.000000 cars-0.7.6/cars/data_structures/cars_dict.py
+-rw-------   0 youssefd  (7412) campus    (9585)     9741 2024-02-15 14:48:18.000000 cars-0.7.6/cars/data_structures/corresponding_tiles_tools.py
+-rw-------   0 youssefd  (7412) campus    (9585)     6285 2023-12-06 08:28:57.000000 cars-0.7.6/cars/data_structures/dataframe_converter.py
+-rw-------   0 youssefd  (7412) campus    (9585)     7442 2023-12-06 08:28:57.000000 cars-0.7.6/cars/data_structures/format_transformation.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3952 2024-02-01 07:18:04.000000 cars-0.7.6/cars/extractroi.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.684644 cars-0.7.6/cars/orchestrator/
+-rw-------   0 youssefd  (7412) campus    (9585)      762 2022-10-07 19:31:52.000000 cars-0.7.6/cars/orchestrator/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3438 2024-04-26 07:37:47.000000 cars-0.7.6/cars/orchestrator/achievement_tracker.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.690736 cars-0.7.6/cars/orchestrator/cluster/
+-rw-------   0 youssefd  (7412) campus    (9585)     1045 2023-10-18 06:44:29.000000 cars-0.7.6/cars/orchestrator/cluster/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     6219 2024-03-07 08:33:34.000000 cars-0.7.6/cars/orchestrator/cluster/abstract_cluster.py
+-rw-------   0 youssefd  (7412) campus    (9585)    10946 2024-03-07 08:33:34.000000 cars-0.7.6/cars/orchestrator/cluster/abstract_dask_cluster.py
+-rw-------   0 youssefd  (7412) campus    (9585)     2919 2024-01-16 15:27:41.000000 cars-0.7.6/cars/orchestrator/cluster/dask_cluster_tools.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.694137 cars-0.7.6/cars/orchestrator/cluster/dask_config/
+-rw-------   0 youssefd  (7412) campus    (9585)     7009 2023-01-02 09:39:32.000000 cars-0.7.6/cars/orchestrator/cluster/dask_config/README.md
+-rw-------   0 youssefd  (7412) campus    (9585)     1016 2023-01-02 09:39:32.000000 cars-0.7.6/cars/orchestrator/cluster/dask_config/dask.yaml
+-rw-------   0 youssefd  (7412) campus    (9585)     3120 2023-06-20 07:07:34.000000 cars-0.7.6/cars/orchestrator/cluster/dask_config/distributed.yaml
+-rw-------   0 youssefd  (7412) campus    (9585)     1427 2023-01-02 09:39:32.000000 cars-0.7.6/cars/orchestrator/cluster/dask_config/jobqueue.yaml
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.699026 cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/
+-rw-------   0 youssefd  (7412) campus    (9585)     4711 2023-01-02 09:39:32.000000 cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/dask-schema.yaml
+-rw-------   0 youssefd  (7412) campus    (9585)      989 2023-01-02 09:39:32.000000 cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/dask.yaml
+-rw-------   0 youssefd  (7412) campus    (9585)    38310 2023-01-02 09:39:32.000000 cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/distributed-schema.yaml
+-rw-------   0 youssefd  (7412) campus    (9585)    11637 2023-02-22 08:13:13.000000 cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/distributed.yaml
+-rw-------   0 youssefd  (7412) campus    (9585)     7566 2023-01-02 09:39:32.000000 cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/jobqueue.yaml
+-rw-------   0 youssefd  (7412) campus    (9585)     6619 2023-10-03 13:46:59.000000 cars-0.7.6/cars/orchestrator/cluster/dask_jobqueue_utils.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3018 2023-10-18 06:44:29.000000 cars-0.7.6/cars/orchestrator/cluster/local_dask_cluster.py
+-rw-------   0 youssefd  (7412) campus    (9585)    24392 2024-03-07 08:33:34.000000 cars-0.7.6/cars/orchestrator/cluster/log_wrapper.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.703174 cars-0.7.6/cars/orchestrator/cluster/mp_cluster/
+-rw-------   0 youssefd  (7412) campus    (9585)      834 2023-03-21 16:35:08.000000 cars-0.7.6/cars/orchestrator/cluster/mp_cluster/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     6317 2023-10-03 13:47:12.000000 cars-0.7.6/cars/orchestrator/cluster/mp_cluster/mp_factorizer.py
+-rw-------   0 youssefd  (7412) campus    (9585)    14531 2024-03-07 08:33:34.000000 cars-0.7.6/cars/orchestrator/cluster/mp_cluster/mp_objects.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3090 2023-10-03 13:47:12.000000 cars-0.7.6/cars/orchestrator/cluster/mp_cluster/mp_tools.py
+-rw-------   0 youssefd  (7412) campus    (9585)    10298 2024-03-07 08:33:34.000000 cars-0.7.6/cars/orchestrator/cluster/mp_cluster/mp_wrapper.py
+-rw-------   0 youssefd  (7412) campus    (9585)    25350 2024-03-07 08:33:34.000000 cars-0.7.6/cars/orchestrator/cluster/mp_cluster/multiprocessing_cluster.py
+-rw-------   0 youssefd  (7412) campus    (9585)     5786 2023-10-18 06:44:29.000000 cars-0.7.6/cars/orchestrator/cluster/pbs_dask_cluster.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3386 2024-03-07 08:33:34.000000 cars-0.7.6/cars/orchestrator/cluster/sequential_cluster.py
+-rw-------   0 youssefd  (7412) campus    (9585)     7033 2024-03-07 08:33:34.000000 cars-0.7.6/cars/orchestrator/cluster/slurm_dask_cluster.py
+-rw-------   0 youssefd  (7412) campus    (9585)    18719 2024-04-26 07:37:47.000000 cars-0.7.6/cars/orchestrator/orchestrator.py
+-rw-------   0 youssefd  (7412) campus    (9585)      894 2022-10-07 19:31:52.000000 cars-0.7.6/cars/orchestrator/orchestrator_constants.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.707441 cars-0.7.6/cars/orchestrator/registry/
+-rw-------   0 youssefd  (7412) campus    (9585)      758 2022-10-07 19:31:52.000000 cars-0.7.6/cars/orchestrator/registry/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     4002 2024-02-15 14:48:18.000000 cars-0.7.6/cars/orchestrator/registry/abstract_registry.py
+-rw-------   0 youssefd  (7412) campus    (9585)     2962 2024-04-26 07:37:47.000000 cars-0.7.6/cars/orchestrator/registry/compute_registry.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3090 2022-10-07 19:31:52.000000 cars-0.7.6/cars/orchestrator/registry/id_generator.py
+-rw-------   0 youssefd  (7412) campus    (9585)     6074 2024-03-07 08:33:34.000000 cars-0.7.6/cars/orchestrator/registry/replacer_registry.py
+-rw-------   0 youssefd  (7412) campus    (9585)    12683 2024-02-15 14:48:18.000000 cars-0.7.6/cars/orchestrator/registry/saver_registry.py
+-rw-------   0 youssefd  (7412) campus    (9585)     3234 2024-02-01 07:18:04.000000 cars-0.7.6/cars/orchestrator/registry/unseen_registry.py
+-rw-------   0 youssefd  (7412) campus    (9585)     7925 2024-04-26 07:37:47.000000 cars-0.7.6/cars/orchestrator/tiles_profiler.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.709636 cars-0.7.6/cars/pipelines/
+-rw-------   0 youssefd  (7412) campus    (9585)      973 2023-03-10 14:57:03.000000 cars-0.7.6/cars/pipelines/__init__.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.712959 cars-0.7.6/cars/pipelines/conf_pipeline/
+-rw-------   0 youssefd  (7412) campus    (9585)      765 2022-11-02 08:44:18.000000 cars-0.7.6/cars/pipelines/conf_pipeline/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)        8 2023-03-10 14:57:03.000000 cars-0.7.6/cars/pipelines/conf_pipeline/point_clouds_to_dsm.json
+-rw-------   0 youssefd  (7412) campus    (9585)       13 2023-03-10 14:57:03.000000 cars-0.7.6/cars/pipelines/conf_pipeline/sensor_to_dense_dsm.json
+-rw-------   0 youssefd  (7412) campus    (9585)      158 2023-03-10 14:57:03.000000 cars-0.7.6/cars/pipelines/conf_pipeline/sensor_to_pc.json
+-rw-------   0 youssefd  (7412) campus    (9585)      223 2023-06-05 15:54:23.000000 cars-0.7.6/cars/pipelines/conf_pipeline/sensor_to_sparse_dsm.json
+-rw-------   0 youssefd  (7412) campus    (9585)     3445 2023-03-10 14:57:03.000000 cars-0.7.6/cars/pipelines/pipeline.py
+-rw-------   0 youssefd  (7412) campus    (9585)      956 2023-10-03 13:46:59.000000 cars-0.7.6/cars/pipelines/pipeline_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)     4273 2023-10-03 13:46:59.000000 cars-0.7.6/cars/pipelines/pipeline_template.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.715395 cars-0.7.6/cars/pipelines/point_clouds_to_dsm/
+-rw-------   0 youssefd  (7412) campus    (9585)      892 2023-03-10 14:57:03.000000 cars-0.7.6/cars/pipelines/point_clouds_to_dsm/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)      822 2023-03-10 14:57:03.000000 cars-0.7.6/cars/pipelines/point_clouds_to_dsm/pc_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    10299 2024-02-01 07:18:04.000000 cars-0.7.6/cars/pipelines/point_clouds_to_dsm/pc_inputs.py
+-rw-------   0 youssefd  (7412) campus    (9585)    16404 2024-02-01 07:18:04.000000 cars-0.7.6/cars/pipelines/point_clouds_to_dsm/point_cloud_to_dsm_pipeline.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.718355 cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/
+-rw-------   0 youssefd  (7412) campus    (9585)      893 2023-03-10 14:57:03.000000 cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)     2225 2023-03-10 14:57:03.000000 cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/dsm_output.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1765 2024-04-26 07:37:47.000000 cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/sensor_dense_dsm_constants.py
+-rw-------   0 youssefd  (7412) campus    (9585)    59251 2024-04-26 07:37:47.000000 cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/sensor_to_dense_dsm_pipeline.py
+-rw-------   0 youssefd  (7412) campus    (9585)    25885 2024-04-26 07:37:47.000000 cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/sensors_inputs.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.719731 cars-0.7.6/cars/pipelines/sensor_to_sparse_dsm/
+-rw-------   0 youssefd  (7412) campus    (9585)      895 2023-03-10 14:57:03.000000 cars-0.7.6/cars/pipelines/sensor_to_sparse_dsm/__init__.py
+-rw-------   0 youssefd  (7412) campus    (9585)    23929 2024-04-26 07:37:47.000000 cars-0.7.6/cars/pipelines/sensor_to_sparse_dsm/sensor_to_sparse_dsm_pipeline.py
+-rw-------   0 youssefd  (7412) campus    (9585)     4437 2024-01-11 08:32:35.000000 cars-0.7.6/cars/starter.py
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.594021 cars-0.7.6/cars.egg-info/
+-rw-r--r--   0 youssefd  (7412) campus    (9585)     8274 2024-04-26 08:08:02.000000 cars-0.7.6/cars.egg-info/PKG-INFO
+-rw-------   0 youssefd  (7412) campus    (9585)     8612 2024-04-26 08:08:12.592041 cars-0.7.6/cars.egg-info/SOURCES.txt
+-rw-------   0 youssefd  (7412) campus    (9585)        1 2024-04-26 08:08:02.000000 cars-0.7.6/cars.egg-info/dependency_links.txt
+-rw-------   0 youssefd  (7412) campus    (9585)      167 2024-04-26 08:08:02.000000 cars-0.7.6/cars.egg-info/entry_points.txt
+-rw-------   0 youssefd  (7412) campus    (9585)      852 2024-04-26 08:08:02.000000 cars-0.7.6/cars.egg-info/requires.txt
+-rw-------   0 youssefd  (7412) campus    (9585)       11 2024-04-26 08:08:02.000000 cars-0.7.6/cars.egg-info/top_level.txt
+-rwx------   0 youssefd  (7412) campus    (9585)     2254 2023-01-02 09:39:32.000000 cars-0.7.6/env_cars.sh
+-rw-------   0 youssefd  (7412) campus    (9585)     2771 2023-07-05 16:15:54.000000 cars-0.7.6/gdal-config
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.721134 cars-0.7.6/otb_remote_module/
+-rw-------   0 youssefd  (7412) campus    (9585)      374 2023-03-21 16:35:08.000000 cars-0.7.6/otb_remote_module/CMakeLists.txt
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.724203 cars-0.7.6/otb_remote_module/app/
+-rw-------   0 youssefd  (7412) campus    (9585)      543 2023-12-06 08:28:57.000000 cars-0.7.6/otb_remote_module/app/CMakeLists.txt
+-rw-------   0 youssefd  (7412) campus    (9585)     9637 2023-10-03 13:47:12.000000 cars-0.7.6/otb_remote_module/app/otbConvertSensorToGeoMultiPointFast.cxx
+-rw-------   0 youssefd  (7412) campus    (9585)     7228 2023-02-27 10:57:22.000000 cars-0.7.6/otb_remote_module/app/otbEpipolarTriangulation.cxx
+-rw-------   0 youssefd  (7412) campus    (9585)     8596 2023-12-06 08:28:57.000000 cars-0.7.6/otb_remote_module/app/otbLocalizeInverse.cxx
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.770864 cars-0.7.6/otb_remote_module/data/
+-rw-------   0 youssefd  (7412) campus    (9585)   323046 2020-12-16 10:57:27.000000 cars-0.7.6/otb_remote_module/data/rectified_ref.tif
+-rw-------   0 youssefd  (7412) campus    (9585)    81136 2020-12-16 10:57:27.000000 cars-0.7.6/otb_remote_module/data/rectified_ref_mask.tif
+-rw-------   0 youssefd  (7412) campus    (9585)   322610 2020-12-16 10:57:27.000000 cars-0.7.6/otb_remote_module/data/rectified_sec.tif
+-rw-------   0 youssefd  (7412) campus    (9585)    75835 2020-12-16 10:57:27.000000 cars-0.7.6/otb_remote_module/data/rectified_sec_mask.tif
+drwx--S---   0 youssefd  (7412) campus    (9585)        0 2024-04-26 08:08:12.773039 cars-0.7.6/otb_remote_module/include/
+-rw-------   0 youssefd  (7412) campus    (9585)    13784 2023-02-27 10:57:22.000000 cars-0.7.6/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.h
+-rw-------   0 youssefd  (7412) campus    (9585)    13094 2023-02-27 10:57:22.000000 cars-0.7.6/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.hxx
+-rw-------   0 youssefd  (7412) campus    (9585)      506 2020-12-16 10:57:27.000000 cars-0.7.6/otb_remote_module/otb-module.cmake
+-rw-------   0 youssefd  (7412) campus    (9585)      407 2022-10-07 19:31:52.000000 cars-0.7.6/pyproject.toml
+-rw-------   0 youssefd  (7412) campus    (9585)      316 2023-08-16 11:31:21.000000 cars-0.7.6/pytest.ini
+-rw-------   0 youssefd  (7412) campus    (9585)     3268 2024-04-26 08:08:12.780106 cars-0.7.6/setup.cfg
+-rw-------   0 youssefd  (7412) campus    (9585)     1084 2023-06-07 07:59:04.000000 cars-0.7.6/setup.py
+-rw-------   0 youssefd  (7412) campus    (9585)     1527 2024-02-01 07:18:04.000000 cars-0.7.6/sonar-project.properties
```

### Comparing `cars-0.7.5/.gitignore` & `cars-0.7.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/.gitlab/issue_templates/Bug.md` & `cars-0.7.6/.gitlab/issue_templates/Bug.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/.gitlab/issue_templates/Refacto.md` & `cars-0.7.6/.gitlab/issue_templates/Refacto.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/.gitlab/issue_templates/Release.md` & `cars-0.7.6/.gitlab/issue_templates/Release.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/.gitlab/merge_request_templates/MR.md` & `cars-0.7.6/.gitlab/merge_request_templates/MR.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/.pre-commit-config.yaml` & `cars-0.7.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/.pylintrc` & `cars-0.7.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/.readthedocs.yaml` & `cars-0.7.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/AUTHORS.md` & `cars-0.7.6/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/CHANGELOG.md` & `cars-0.7.6/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,35 @@
 # Changelog
 
 
 
+## 0.7.6  Confidence intervals (April 2024)
+
+### Added
+
+ - Integration of Pandora confidence intervals [#764]
+ - Option to choose endogenous or exogenous DEM to resample images [#790]
+ - Geomodel parameter is optional [#785]
+ - Path to JSON file is allowed for dense matching loader configuration [#552]
+ - Support for point cloud denoising plugin [#771]
+ - Check footprint of given initial elevation [#780]
+
+ ### Changed
+
+  - Version 0.2.0 of Shareloc is used : fast grid generation [#781]
+
+ ### Fixed
+
+  - Invert rows and columns for generation of disparity range grids with Shareloc [#804]
+  - Better typing of output files [#758]
+  - Faster LAZ point cloud saving [#795]
+  - Avoid computation of useless epipolar tiles when a ROI is given for no_merging pipelines [#791]
+  - Compute footprint of endogenous DEM according to images and epipolar footprint [#780]
+  - Broadcast delayed objects with dask to avoid memory overload [#796]
+
 ## 0.7.5  Pandora integration (March 2024)
 
 ### Added
 
  - New default pipeline sensors_to_dense_dsm_no_merging with cumulative rasterisation [#698]
  - Profiling report for multiprocessing mode [#745]
  - Dashboard showing tiles processing during a run [#765]
```

### Comparing `cars-0.7.5/CONTRIBUTING.md` & `cars-0.7.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/Dockerfile` & `cars-0.7.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/Dockerfile.deps` & `cars-0.7.6/Dockerfile.deps`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/Dockerfile.jupyter` & `cars-0.7.6/Dockerfile.jupyter`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/LICENSE` & `cars-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/Makefile` & `cars-0.7.6/Makefile`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/NOTICE` & `cars-0.7.6/NOTICE`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/PKG-INFO` & `cars-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cars
-Version: 0.7.5
+Version: 0.7.6
 Summary: A satellite multi view stereo pipeline
 Home-page: https://cars.readthedocs.io/
 Author: CNES
 Author-email: cars@cnes.fr
 License: Apache License 2.0
 Project-URL: Source, https://github.com/CNES/cars
 Project-URL: Documentation, https://cars.readthedocs.io/en/latest/
@@ -44,15 +44,15 @@
 Requires-Dist: laspy[laszip]
 Requires-Dist: tbb==2020.3.254
 Requires-Dist: numba
 Requires-Dist: pandora[sgm]==1.6.*
 Requires-Dist: cars-rasterize==0.2.*
 Requires-Dist: cars-resample==0.1.*
 Requires-Dist: vlsift==0.1.*
-Requires-Dist: shareloc==0.2.0a2
+Requires-Dist: shareloc==0.2.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: isort>=5.8.0; extra == "dev"
 Requires-Dist: black>=24.1a1; extra == "dev"
 Requires-Dist: flake8>=3.9.1; extra == "dev"
@@ -113,16 +113,17 @@
 <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/animation_sat.gif" alt="drawing" width="400"/> |  <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/overview_dsm_3d.gif" alt="drawing" width="400"/>
 
 
 **CARS** is an open source 3D tool dedicated to produce **Digital Surface Models** from satellite imaging by photogrammetry.
 This Multiview Stereo framework is intended for massive DSM production with a robust, performant and modular design.
 
 Be aware that the project is new and is evolving to maturity with CNES usage roadmaps and projects such as:
-- <a href="https://co3d.cnes.fr/en/co3d-0">CO3D project &nbsp;&nbsp;&nbsp;  <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo_co3D_cnes.jpg" width="20" height="20"/></a>
-- <a href="https://www.ai4geo.eu/">AI4GEO project &nbsp;&nbsp;&nbsp;  </a>
+- <a href="https://co3d.cnes.fr/en/co3d-0">CO3D project &nbsp;&nbsp;&nbsp;  <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo_co3D_cnes.jpg" height="20"/></a>
+- <a href="https://www.ai4geo.eu">AI4GEO project &nbsp;&nbsp;&nbsp; <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo-ai4geo.png" height="20"/> </a>
+- <a href="https://www.evo-land.eu">Evoland project &nbsp;&nbsp;&nbsp; <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo-evoland.png" height="20"/> </a>
 
 ## Quick start
 
 ### CARS Docker Image
 
 [![Docker Status](http://dockeri.co/image/cnes/cars)](https://hub.docker.com/r/cnes/cars)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cars Version: 0.7.5 Summary: A satellite multi view
+Metadata-Version: 2.1 Name: cars Version: 0.7.6 Summary: A satellite multi view
 stereo pipeline Home-page: https://cars.readthedocs.io/ Author: CNES Author-
 email: cars@cnes.fr License: Apache License 2.0 Project-URL: Source, https://
 github.com/CNES/cars Project-URL: Documentation, https://cars.readthedocs.io/
 en/latest/ Keywords: cars,3D,DEM,pandora,photogrammetry Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: End Users/Desktop Classifier:
 Intended Audience :: Science/Research Classifier: Environment :: Console
@@ -16,18 +16,18 @@
 dask>=2021.10.0 Requires-Dist: distributed>=2021.10.0 Requires-Dist: dask-
 jobqueue>=0.7.3 Requires-Dist: json-checker Requires-Dist: xarray Requires-
 Dist: tqdm Requires-Dist: netCDF4>=1.5.3 Requires-Dist: Shapely Requires-Dist:
 Fiona Requires-Dist: pyproj Requires-Dist: utm Requires-Dist: pandas Requires-
 Dist: urllib3<2.0,>=1.21.1 Requires-Dist: laspy[laszip] Requires-Dist:
 tbb==2020.3.254 Requires-Dist: numba Requires-Dist: pandora[sgm]==1.6.*
 Requires-Dist: cars-rasterize==0.2.* Requires-Dist: cars-resample==0.1.*
-Requires-Dist: vlsift==0.1.* Requires-Dist: shareloc==0.2.0a2 Provides-Extra:
-dev Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra ==
-"dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist: isort>=5.8.0;
-extra == "dev" Requires-Dist: black>=24.1a1; extra == "dev" Requires-Dist:
+Requires-Dist: vlsift==0.1.* Requires-Dist: shareloc==0.2.0 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev" Requires-Dist: isort>=5.8.0; extra ==
+"dev" Requires-Dist: black>=24.1a1; extra == "dev" Requires-Dist:
 flake8>=3.9.1; extra == "dev" Requires-Dist: flake8-comprehensions>=3.4.0;
 extra == "dev" Requires-Dist: flake8-bugbear<24.0.0,>=21.4.3; extra == "dev"
 Requires-Dist: jupyter_contrib_nbextensions; extra == "dev" Requires-Dist:
 pylint<3.0.0,>=2.8.12; extra == "dev" Requires-Dist: setuptools_scm; extra ==
 "dev" Requires-Dist: virtualenv; extra == "dev" Requires-Dist: configupdater;
 extra == "dev" Requires-Dist: twine; extra == "dev" Requires-Dist:
 notebook<7.0.0; extra == "dev" Requires-Dist: bokeh==2.4.3; extra == "dev"
@@ -56,39 +56,41 @@
 ------------------------:|:-------------------------: [drawing]|
 [drawing]**CARS** is an open source 3D tool dedicated to produce **Digital
 Surface Models** from satellite imaging by photogrammetry. This Multiview
 Stereo framework is intended for massive DSM production with a robust,
 performant and modular design. Be aware that the project is new and is evolving
 to maturity with CNES usage roadmaps and projects such as: - _C_O_3_D_ _p_r_o_j_e_c_t_ _ _ _ _ 
 _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_C_N_E_S_/_c_a_r_s_/_m_a_s_t_e_r_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/
-_l_o_g_o___c_o_3_D___c_n_e_s_._j_p_g_]- _A_I_4_G_E_O_ _p_r_o_j_e_c_t_ _ _ _ _ ## Quick start ### CARS Docker Image [!
-[Docker Status](http://dockeri.co/image/cnes/cars)](https://hub.docker.com/r/
-cnes/cars) CARS is available on Docker Hub and can be downloaded by: ``` bash
-docker pull cnes/cars ``` ### One main pipeline to generate DSM You only need
-to launch one command: ``` docker run -w /data -v "$(pwd)"/data_gizeh:/data
-cnes/cars /data/configfile.json ``` with one configuration input file
-("configfile.json") located in a "data" folder to be consistent with the
-previous command lines: ``` { "inputs": { "sensors" : { "one": { "image":
-"img1.tif", "geomodel": "img1.geom" }, "two": { "image": "img2.tif",
-"geomodel": "img2.geom" }, "three": { "image": "img3.tif", "geomodel":
-"img3.geom" } }, "pairing": [["one", "two"],["one", "three"]],
-"initial_elevation": "srtm_dir/N29E031_KHEOPS.tif" }, "output": { "out_dir":
-"outresults" } } ``` ### On the way to the Pyramids... You want to build the
-pyramids by yourself? Download our [open licence](https://www.etalab.gouv.fr/
-licence-ouverte-open-licence) Pleiades [data sample](https://
-raw.githubusercontent.com/CNES/cars/master/tutorials/data_gizeh.tar.bz2) to
-give CARS a try! ## Documentation Go to [CARS Main Documentation](https://
-cars.readthedocs.io/?badge=latest). ## Contribution To do a bug report or a
-contribution, see the [**Contribution Guide**](https://github.com/CNES/cars/
-blob/master/CONTRIBUTING.md). For project evolution, see [**Changelog**](https:
-//github.com/CNES/cars/blob/master/CHANGELOG.md). ## Credits See [Authors file]
-(https://github.com/CNES/cars/blob/master/AUTHORS.md) ## References - [Youssefi
-D., Michel, J., Sarrazin, E., Buffe, F., Cournet, M., Delvit, J., LâHelguen,
-C., Melet, O., Emilien, A., Bosman, J., 2020. Cars: A photogrammetry pipeline
-using dask graphs to construct a global 3d model. IGARSS - IEEE International
-Geoscience and Remote Sensing Symposium.](https://ieeexplore.ieee.org/document/
-9324020) - [Michel, J., Sarrazin, E., Youssefi, D., Cournet, M., Buffe, F.,
-Delvit, J., Emilien, A., Bosman, J., Melet, O., LâHelguen, C., 2020. A new
-satellite imagery stereo pipeline designed for scalability, robustness and
-performance. ISPRS - International Archives of the Photogrammetry, Remote
-Sensing and Spatial Information Sciences.](https://www.isprs-ann-photogramm-
-remote-sens-spatial-inf-sci.net/V-2-2020/171/2020/)
+_l_o_g_o___c_o_3_D___c_n_e_s_._j_p_g_]- _A_I_4_G_E_O_ _p_r_o_j_e_c_t_ _ _ _ _ _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/
+_C_N_E_S_/_c_a_r_s_/_m_a_s_t_e_r_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_l_o_g_o_-_a_i_4_g_e_o_._p_n_g_]- _E_v_o_l_a_n_d_ _p_r_o_j_e_c_t_ _ _ _ _ 
+_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_C_N_E_S_/_c_a_r_s_/_m_a_s_t_e_r_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_l_o_g_o_-
+_e_v_o_l_a_n_d_._p_n_g_]## Quick start ### CARS Docker Image [![Docker Status](http://
+dockeri.co/image/cnes/cars)](https://hub.docker.com/r/cnes/cars) CARS is
+available on Docker Hub and can be downloaded by: ``` bash docker pull cnes/
+cars ``` ### One main pipeline to generate DSM You only need to launch one
+command: ``` docker run -w /data -v "$(pwd)"/data_gizeh:/data cnes/cars /data/
+configfile.json ``` with one configuration input file ("configfile.json")
+located in a "data" folder to be consistent with the previous command lines:
+``` { "inputs": { "sensors" : { "one": { "image": "img1.tif", "geomodel":
+"img1.geom" }, "two": { "image": "img2.tif", "geomodel": "img2.geom" },
+"three": { "image": "img3.tif", "geomodel": "img3.geom" } }, "pairing": [
+["one", "two"],["one", "three"]], "initial_elevation": "srtm_dir/
+N29E031_KHEOPS.tif" }, "output": { "out_dir": "outresults" } } ``` ### On the
+way to the Pyramids... You want to build the pyramids by yourself? Download our
+[open licence](https://www.etalab.gouv.fr/licence-ouverte-open-licence)
+Pleiades [data sample](https://raw.githubusercontent.com/CNES/cars/master/
+tutorials/data_gizeh.tar.bz2) to give CARS a try! ## Documentation Go to [CARS
+Main Documentation](https://cars.readthedocs.io/?badge=latest). ## Contribution
+To do a bug report or a contribution, see the [**Contribution Guide**](https://
+github.com/CNES/cars/blob/master/CONTRIBUTING.md). For project evolution, see
+[**Changelog**](https://github.com/CNES/cars/blob/master/CHANGELOG.md). ##
+Credits See [Authors file](https://github.com/CNES/cars/blob/master/AUTHORS.md)
+## References - [Youssefi D., Michel, J., Sarrazin, E., Buffe, F., Cournet, M.,
+Delvit, J., LâHelguen, C., Melet, O., Emilien, A., Bosman, J., 2020. Cars: A
+photogrammetry pipeline using dask graphs to construct a global 3d model.
+IGARSS - IEEE International Geoscience and Remote Sensing Symposium.](https://
+ieeexplore.ieee.org/document/9324020) - [Michel, J., Sarrazin, E., Youssefi,
+D., Cournet, M., Buffe, F., Delvit, J., Emilien, A., Bosman, J., Melet, O.,
+LâHelguen, C., 2020. A new satellite imagery stereo pipeline designed for
+scalability, robustness and performance. ISPRS - International Archives of the
+Photogrammetry, Remote Sensing and Spatial Information Sciences.](https://
+www.isprs-ann-photogramm-remote-sens-spatial-inf-sci.net/V-2-2020/171/2020/)
```

### Comparing `cars-0.7.5/README.md` & `cars-0.7.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/animation_sat.gif" alt="drawing" width="400"/> |  <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/overview_dsm_3d.gif" alt="drawing" width="400"/>
 
 
 **CARS** is an open source 3D tool dedicated to produce **Digital Surface Models** from satellite imaging by photogrammetry.
 This Multiview Stereo framework is intended for massive DSM production with a robust, performant and modular design.
 
 Be aware that the project is new and is evolving to maturity with CNES usage roadmaps and projects such as:
-- <a href="https://co3d.cnes.fr/en/co3d-0">CO3D project &nbsp;&nbsp;&nbsp;  <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo_co3D_cnes.jpg" width="20" height="20"/></a>
-- <a href="https://www.ai4geo.eu/">AI4GEO project &nbsp;&nbsp;&nbsp;  </a>
+- <a href="https://co3d.cnes.fr/en/co3d-0">CO3D project &nbsp;&nbsp;&nbsp;  <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo_co3D_cnes.jpg" height="20"/></a>
+- <a href="https://www.ai4geo.eu">AI4GEO project &nbsp;&nbsp;&nbsp; <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo-ai4geo.png" height="20"/> </a>
+- <a href="https://www.evo-land.eu">Evoland project &nbsp;&nbsp;&nbsp; <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo-evoland.png" height="20"/> </a>
 
 ## Quick start
 
 ### CARS Docker Image
 
 [![Docker Status](http://dockeri.co/image/cnes/cars)](https://hub.docker.com/r/cnes/cars)
```

#### html2text {}

```diff
@@ -12,39 +12,41 @@
 ------------------------:|:-------------------------: [drawing]|
 [drawing]**CARS** is an open source 3D tool dedicated to produce **Digital
 Surface Models** from satellite imaging by photogrammetry. This Multiview
 Stereo framework is intended for massive DSM production with a robust,
 performant and modular design. Be aware that the project is new and is evolving
 to maturity with CNES usage roadmaps and projects such as: - _C_O_3_D_ _p_r_o_j_e_c_t_ _ _ _ _ 
 _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_C_N_E_S_/_c_a_r_s_/_m_a_s_t_e_r_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/
-_l_o_g_o___c_o_3_D___c_n_e_s_._j_p_g_]- _A_I_4_G_E_O_ _p_r_o_j_e_c_t_ _ _ _ _ ## Quick start ### CARS Docker Image [!
-[Docker Status](http://dockeri.co/image/cnes/cars)](https://hub.docker.com/r/
-cnes/cars) CARS is available on Docker Hub and can be downloaded by: ``` bash
-docker pull cnes/cars ``` ### One main pipeline to generate DSM You only need
-to launch one command: ``` docker run -w /data -v "$(pwd)"/data_gizeh:/data
-cnes/cars /data/configfile.json ``` with one configuration input file
-("configfile.json") located in a "data" folder to be consistent with the
-previous command lines: ``` { "inputs": { "sensors" : { "one": { "image":
-"img1.tif", "geomodel": "img1.geom" }, "two": { "image": "img2.tif",
-"geomodel": "img2.geom" }, "three": { "image": "img3.tif", "geomodel":
-"img3.geom" } }, "pairing": [["one", "two"],["one", "three"]],
-"initial_elevation": "srtm_dir/N29E031_KHEOPS.tif" }, "output": { "out_dir":
-"outresults" } } ``` ### On the way to the Pyramids... You want to build the
-pyramids by yourself? Download our [open licence](https://www.etalab.gouv.fr/
-licence-ouverte-open-licence) Pleiades [data sample](https://
-raw.githubusercontent.com/CNES/cars/master/tutorials/data_gizeh.tar.bz2) to
-give CARS a try! ## Documentation Go to [CARS Main Documentation](https://
-cars.readthedocs.io/?badge=latest). ## Contribution To do a bug report or a
-contribution, see the [**Contribution Guide**](https://github.com/CNES/cars/
-blob/master/CONTRIBUTING.md). For project evolution, see [**Changelog**](https:
-//github.com/CNES/cars/blob/master/CHANGELOG.md). ## Credits See [Authors file]
-(https://github.com/CNES/cars/blob/master/AUTHORS.md) ## References - [Youssefi
-D., Michel, J., Sarrazin, E., Buffe, F., Cournet, M., Delvit, J., LâHelguen,
-C., Melet, O., Emilien, A., Bosman, J., 2020. Cars: A photogrammetry pipeline
-using dask graphs to construct a global 3d model. IGARSS - IEEE International
-Geoscience and Remote Sensing Symposium.](https://ieeexplore.ieee.org/document/
-9324020) - [Michel, J., Sarrazin, E., Youssefi, D., Cournet, M., Buffe, F.,
-Delvit, J., Emilien, A., Bosman, J., Melet, O., LâHelguen, C., 2020. A new
-satellite imagery stereo pipeline designed for scalability, robustness and
-performance. ISPRS - International Archives of the Photogrammetry, Remote
-Sensing and Spatial Information Sciences.](https://www.isprs-ann-photogramm-
-remote-sens-spatial-inf-sci.net/V-2-2020/171/2020/)
+_l_o_g_o___c_o_3_D___c_n_e_s_._j_p_g_]- _A_I_4_G_E_O_ _p_r_o_j_e_c_t_ _ _ _ _ _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/
+_C_N_E_S_/_c_a_r_s_/_m_a_s_t_e_r_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_l_o_g_o_-_a_i_4_g_e_o_._p_n_g_]- _E_v_o_l_a_n_d_ _p_r_o_j_e_c_t_ _ _ _ _ 
+_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_C_N_E_S_/_c_a_r_s_/_m_a_s_t_e_r_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_l_o_g_o_-
+_e_v_o_l_a_n_d_._p_n_g_]## Quick start ### CARS Docker Image [![Docker Status](http://
+dockeri.co/image/cnes/cars)](https://hub.docker.com/r/cnes/cars) CARS is
+available on Docker Hub and can be downloaded by: ``` bash docker pull cnes/
+cars ``` ### One main pipeline to generate DSM You only need to launch one
+command: ``` docker run -w /data -v "$(pwd)"/data_gizeh:/data cnes/cars /data/
+configfile.json ``` with one configuration input file ("configfile.json")
+located in a "data" folder to be consistent with the previous command lines:
+``` { "inputs": { "sensors" : { "one": { "image": "img1.tif", "geomodel":
+"img1.geom" }, "two": { "image": "img2.tif", "geomodel": "img2.geom" },
+"three": { "image": "img3.tif", "geomodel": "img3.geom" } }, "pairing": [
+["one", "two"],["one", "three"]], "initial_elevation": "srtm_dir/
+N29E031_KHEOPS.tif" }, "output": { "out_dir": "outresults" } } ``` ### On the
+way to the Pyramids... You want to build the pyramids by yourself? Download our
+[open licence](https://www.etalab.gouv.fr/licence-ouverte-open-licence)
+Pleiades [data sample](https://raw.githubusercontent.com/CNES/cars/master/
+tutorials/data_gizeh.tar.bz2) to give CARS a try! ## Documentation Go to [CARS
+Main Documentation](https://cars.readthedocs.io/?badge=latest). ## Contribution
+To do a bug report or a contribution, see the [**Contribution Guide**](https://
+github.com/CNES/cars/blob/master/CONTRIBUTING.md). For project evolution, see
+[**Changelog**](https://github.com/CNES/cars/blob/master/CHANGELOG.md). ##
+Credits See [Authors file](https://github.com/CNES/cars/blob/master/AUTHORS.md)
+## References - [Youssefi D., Michel, J., Sarrazin, E., Buffe, F., Cournet, M.,
+Delvit, J., LâHelguen, C., Melet, O., Emilien, A., Bosman, J., 2020. Cars: A
+photogrammetry pipeline using dask graphs to construct a global 3d model.
+IGARSS - IEEE International Geoscience and Remote Sensing Symposium.](https://
+ieeexplore.ieee.org/document/9324020) - [Michel, J., Sarrazin, E., Youssefi,
+D., Cournet, M., Buffe, F., Delvit, J., Emilien, A., Bosman, J., Melet, O.,
+LâHelguen, C., 2020. A new satellite imagery stereo pipeline designed for
+scalability, robustness and performance. ISPRS - International Archives of the
+Photogrammetry, Remote Sensing and Spatial Information Sciences.](https://
+www.isprs-ann-photogramm-remote-sens-spatial-inf-sci.net/V-2-2020/171/2020/)
```

### Comparing `cars-0.7.5/cars/__init__.py` & `cars-0.7.6/cars/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/__init__.py` & `cars-0.7.6/cars/applications/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,13 +24,14 @@
 
 # Imports needed in order to register application for Application factory
 from . import dem_generation  # noqa: F401
 from . import dense_matches_filling  # noqa: F401
 from . import dense_matching  # noqa: F401
 from . import grid_generation  # noqa: F401
 from . import holes_detection  # noqa: F401
+from . import point_cloud_denoising  # noqa: F401
 from . import point_cloud_fusion  # noqa: F401
 from . import point_cloud_outliers_removing  # noqa: F401
 from . import rasterization  # noqa: F401
 from . import resampling  # noqa: F401
 from . import sparse_matching  # noqa: F401
 from . import triangulation  # noqa: F401
```

### Comparing `cars-0.7.5/cars/applications/application.py` & `cars-0.7.6/cars/applications/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 
         app = None
 
         try:
             app_class = cls.available_applications[name]
         except KeyError:
             logging.error("No application named {0} supported".format(name))
+            return None
 
         app = app_class(cfg)
         return app
 
     @classmethod
     def print_applications(cls):
         """
```

### Comparing `cars-0.7.5/cars/applications/application_constants.py` & `cars-0.7.6/cars/applications/application_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/application_template.py` & `cars-0.7.6/cars/applications/application_template.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dem_generation/__init__.py` & `cars-0.7.6/cars/applications/dem_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dem_generation/dem_generation.py` & `cars-0.7.6/cars/applications/dem_generation/dem_generation.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dem_generation/dem_generation_constants.py` & `cars-0.7.6/cars/applications/dem_generation/dem_generation_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dem_generation/dem_generation_tools.py` & `cars-0.7.6/cars/applications/dem_generation/dem_generation_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dem_generation/dichotomic_generation.py` & `cars-0.7.6/cars/applications/dem_generation/dichotomic_generation.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         # Overload conf
         overloaded_conf["method"] = conf.get("method", "dichotomic")
         overloaded_conf["resolution"] = conf.get("resolution", 200)
         # default margin: (z max - zmin) * tan(teta)
         # with z max = 9000, z min = 0, teta = 30 degrees
         overloaded_conf["margin"] = conf.get("margin", 6000)
         overloaded_conf["height_margin"] = conf.get("height_margin", 20)
-        overloaded_conf["percentile"] = conf.get("percentile", 5)
+        overloaded_conf["percentile"] = conf.get("percentile", 3)
         overloaded_conf["min_number_matches"] = conf.get(
             "min_number_matches", 100
         )
 
         overloaded_conf["fillnodata_max_search_distance"] = conf.get(
             "fillnodata_max_search_distance", 3
         )
@@ -135,24 +135,31 @@
         # Check conf
         checker = Checker(rectification_schema)
         checker.validate(overloaded_conf)
 
         return overloaded_conf
 
     @cars_profile(name="DEM Generation")
-    def run(self, triangulated_matches_list, output_dir, geoid_path):
+    def run(
+        self,
+        triangulated_matches_list,
+        output_dir,
+        geoid_path,
+        dem_roi_to_use=None,
+    ):
         """
         Run dichotomic dem generation using matches
 
         :param triangulated_matches_list: list of triangulated matches
             positions must be in a metric system
         :type triangulated_matches_list: list(pandas.Dataframe)
         :param output_dir: directory to save dem
         :type output_dir: str
         :param geoid_path: geoid path
+        :param dem_roi_to_use: dem roi polygon to use as roi
 
         :return: dem data computed with mean, min and max.
             dem is also saved in disk, and paths are available in attributes.
             (DEM_MEDIAN_PATH, DEM_MIN_PATH, DEM_MAX_PATH)
         :rtype: CarsDataset
         """
 
@@ -176,21 +183,30 @@
         merged_point_cloud = pandas.concat(
             triangulated_matches_list,
             ignore_index=True,
             sort=False,
         )
         merged_point_cloud.attrs["epsg"] = epsg
 
-        # Get min max with margin
-        mins = merged_point_cloud.min(skipna=True)
-        maxs = merged_point_cloud.max(skipna=True)
-        xmin = mins["x"]
-        ymin = mins["y"]
-        xmax = maxs["x"]
-        ymax = maxs["y"]
+        # Get bounds
+        if dem_roi_to_use is not None:
+            bounds_poly = dem_roi_to_use.bounds
+            xmin = min(bounds_poly[0], bounds_poly[2])
+            xmax = max(bounds_poly[0], bounds_poly[2])
+            ymin = min(bounds_poly[1], bounds_poly[3])
+            ymax = max(bounds_poly[1], bounds_poly[3])
+        else:
+            # Get min max with margin
+            mins = merged_point_cloud.min(skipna=True)
+            maxs = merged_point_cloud.max(skipna=True)
+            xmin = mins["x"]
+            ymin = mins["y"]
+            xmax = maxs["x"]
+            ymax = maxs["y"]
+
         bounds_cloud = [xmin, ymin, xmax, ymax]
 
         # Convert resolution and margin to degrees
         utm_epsg = preprocessing.get_utm_zone_as_epsg_code(xmin, ymin)
         conversion_factor = preprocessing.get_conversion_factor(
             bounds_cloud, epsg, utm_epsg
         )
```

### Comparing `cars-0.7.5/cars/applications/dense_matches_filling/__init__.py` & `cars-0.7.6/cars/applications/dense_matches_filling/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dense_matches_filling/dense_matches_filling.py` & `cars-0.7.6/cars/applications/dense_matches_filling/dense_matches_filling.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 this module contains the abstract dense matches filling application class.
 """
 import logging
 import os
 from abc import ABCMeta, abstractmethod
 from typing import Dict
 
+import numpy as np
+
 from cars.applications.application import Application
 from cars.applications.application_template import ApplicationTemplate
 from cars.core import constants as cst
 from cars.core import constants_disparity as cst_disp
 from cars.data_structures import cars_dataset
 
 
@@ -215,14 +217,15 @@
             self.orchestrator.add_to_save_lists(
                 os.path.join(
                     pair_folder,
                     "epi_disp_mask_" + app_name + "_filled.tif",
                 ),
                 cst_disp.VALID,
                 new_epipolar_disparity_map,
+                dtype=np.uint8,
                 cars_ds_name="epi_disp_mask_" + app_name + "_filled",
             )
 
             self.orchestrator.add_to_save_lists(
                 os.path.join(
                     pair_folder,
                     "epi_confidence_" + app_name + "_filled.tif",
@@ -235,11 +238,12 @@
             self.orchestrator.add_to_save_lists(
                 os.path.join(
                     pair_folder,
                     "epi_filling_" + app_name + ".tif",
                 ),
                 cst_disp.FILLING,
                 new_epipolar_disparity_map,
+                dtype=np.uint8,
                 cars_ds_name="epi_filling_" + app_name,
             )
 
         return new_epipolar_disparity_map
```

### Comparing `cars-0.7.5/cars/applications/dense_matches_filling/fill_disp_constants.py` & `cars-0.7.6/cars/applications/dense_matches_filling/fill_disp_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dense_matches_filling/fill_disp_tools.py` & `cars-0.7.6/cars/applications/dense_matches_filling/fill_disp_tools.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# pylint: disable=too-many-lines
 """
 This module is responsible for the filling disparity algorithms:
 thus it fills the disparity map with values estimated according to
 their neighbourhood.
 """
-# pylint: disable=too-many-lines
 
 
 import copy
 
 # Standard imports
 import logging
 import math
```

### Comparing `cars-0.7.5/cars/applications/dense_matches_filling/plane.py` & `cars-0.7.6/cars/applications/dense_matches_filling/plane.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dense_matches_filling/zero_padding.py` & `cars-0.7.6/cars/applications/dense_matches_filling/zero_padding.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dense_matching/__init__.py` & `cars-0.7.6/cars/applications/dense_matching/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dense_matching/census_mccnn_sgm.py` & `cars-0.7.6/cars/applications/dense_matching/census_mccnn_sgm.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,14 +159,17 @@
             "disp_max_threshold", None
         )
 
         # Permormance map parameters
         overloaded_conf["generate_performance_map"] = conf.get(
             "generate_performance_map", False
         )
+        overloaded_conf["generate_confidence_intervals"] = conf.get(
+            "generate_confidence_intervals", False
+        )
         overloaded_conf["perf_eta_max_ambiguity"] = conf.get(
             "perf_eta_max_ambiguity", 0.99
         )
         overloaded_conf["perf_eta_max_risk"] = conf.get(
             "perf_eta_max_risk", 0.25
         )
         overloaded_conf["perf_eta_step"] = conf.get("perf_eta_step", 0.04)
@@ -195,48 +198,50 @@
         # TODO modify, use loader directly
         pandora_loader = PandoraLoader(
             conf=loader_conf,
             method_name=overloaded_conf["method"],
             generate_performance_map=overloaded_conf[
                 "generate_performance_map"
             ],
+            generate_confidence_intervals=overloaded_conf[
+                "generate_confidence_intervals"
+            ],
             perf_eta_max_ambiguity=overloaded_conf["perf_eta_max_ambiguity"],
             perf_eta_max_risk=overloaded_conf["perf_eta_max_risk"],
             perf_eta_step=overloaded_conf["perf_eta_step"],
         )
         overloaded_conf["loader"] = loader
-        overloaded_conf["loader_conf"] = collections.OrderedDict(
-            pandora_loader.get_conf()
-        )
+        overloaded_conf["loader_conf"] = loader_conf
 
         # Get params from loader
         self.loader = pandora_loader
-        self.corr_config = overloaded_conf["loader_conf"]
+        self.corr_config = collections.OrderedDict(pandora_loader.get_conf())
 
         application_schema = {
             "method": str,
             "min_epi_tile_size": And(int, lambda x: x > 0),
             "max_epi_tile_size": And(int, lambda x: x > 0),
             "epipolar_tile_margin_in_percent": int,
             "min_elevation_offset": Or(None, int),
             "max_elevation_offset": Or(None, int),
             "disp_min_threshold": Or(None, int),
             "disp_max_threshold": Or(None, int),
             "save_disparity_map": bool,
             "generate_performance_map": bool,
+            "generate_confidence_intervals": bool,
             "perf_eta_max_ambiguity": float,
             "perf_eta_max_risk": float,
             "perf_eta_step": float,
             "perf_ambiguity_threshold": float,
             "use_global_disp_range": bool,
             "local_disp_grid_step": int,
             "disp_range_propagation_filter_size": And(
                 Or(int, float), lambda x: x >= 0
             ),
-            "loader_conf": dict,
+            "loader_conf": Or(dict, collections.OrderedDict, str, None),
             "loader": str,
         }
 
         # Check conf
         checker = Checker(application_schema)
         checker.validate(overloaded_conf)
 
@@ -274,19 +279,19 @@
                 "minimal disparity for dense matching"
             )
 
         return overloaded_conf
 
     def get_margins_fun(self, grid_left, disp_range_grid):
         """
-        Get Margins function  that generates margins needed by
+        Get Margins function that generates margins needed by
         matching method, to use during resampling
 
         :param grid_left: left epipolar grid
-        :param disp_min_grid: minimum and maximumdisparity grid
+        :param disp_min_grid: minimum and maximum disparity grid
         :return: function that generates margin for given roi
 
         """
 
         disp_min_grid_arr = disp_range_grid[0, 0]["disp_min_grid"].values
         disp_max_grid_arr = disp_range_grid[0, 0]["disp_max_grid"].values
         step_row = disp_range_grid.attributes["step_row"]
@@ -604,31 +609,27 @@
             # use local disparity
             if None not in (dmin, dmax):
                 raise RuntimeError("Mix between local and global mode")
 
             # dem mean, min max are the same shape
 
             # Get associated alti mean / min / max values
-            dem_min_shape = inputs.rasterio_get_size(dem_min)
-            dem_max_shape = inputs.rasterio_get_size(dem_max)
-
-            assert dem_min_shape == dem_max_shape
-            # dem mean can be different. Computation is based on dem min shape
+            dem_median_shape = inputs.rasterio_get_size(dem_median)
 
             # get epsg
-            terrain_epsg = inputs.rasterio_get_epsg(dem_min)
+            terrain_epsg = inputs.rasterio_get_epsg(dem_median)
 
             # Get epipolar position of all dem mean
-            transform = inputs.rasterio_get_transform(dem_min)
+            transform = inputs.rasterio_get_transform(dem_median)
             # index position to terrain position
             terrain_positions = np.empty(
-                (dem_min_shape[0] * dem_min_shape[1], 2)
+                (dem_median_shape[0] * dem_median_shape[1], 2)
             )
-            row_shape = dem_min_shape[0]
-            col_shape = dem_min_shape[1]
+            row_shape = dem_median_shape[0]
+            col_shape = dem_median_shape[1]
             for row in range(row_shape):
                 for col in range(col_shape):
                     col_geo, row_geo = transform * (row + 0.5, col + 0.5)
                     terrain_positions[row + row_shape * col, :] = (
                         row_geo,
                         col_geo,
                     )
@@ -978,22 +979,24 @@
                     cars_ds_name="epi_disp_color",
                 )
 
                 self.orchestrator.add_to_save_lists(
                     os.path.join(pair_folder, "epi_disp_mask.tif"),
                     cst_disp.VALID,
                     epipolar_disparity_map,
+                    dtype=np.uint8,
                     cars_ds_name="epi_disp_mask",
                     optional_data=True,
                 )
 
                 self.orchestrator.add_to_save_lists(
                     os.path.join(pair_folder, "epi_disp_classif.tif"),
                     cst.EPI_CLASSIFICATION,
                     epipolar_disparity_map,
+                    dtype=np.uint8,
                     cars_ds_name="epi_disp_classif",
                     optional_data=True,
                 )
 
                 self.orchestrator.add_to_save_lists(
                     os.path.join(
                         pair_folder,
@@ -1023,56 +1026,65 @@
                     cst_disp.EPI_DISP_MAX_GRID,
                     epipolar_disparity_map,
                     cars_ds_name="disp_max",
                 )
                 self.orchestrator.add_to_save_lists(
                     os.path.join(
                         pair_folder,
-                        "epi_filling_disp.tif",
+                        "epi_disp_filling.tif",
                     ),
                     cst_disp.FILLING,
                     epipolar_disparity_map,
-                    cars_ds_name="epi_filling_disp",
-                    nodata=-1,
+                    dtype=np.uint8,
+                    cars_ds_name="epi_disp_filling",
+                    nodata=255,
                 )
 
             # Get saving infos in order to save tiles when they are computed
             [saving_info] = self.orchestrator.get_saving_infos(
                 [epipolar_disparity_map]
             )
 
             # Add infos to orchestrator.out_json
             updating_dict = {
                 application_constants.APPLICATION_TAG: {
+                    dm_cst.DENSE_MATCHING_PARAM_TAG: {
+                        "pandora_config": self.corr_config
+                    },
                     pair_key: {
                         dm_cst.DENSE_MATCHING_RUN_TAG: {
                             "global_disp_min": np.nanmin(
                                 disp_range_grid[0, 0][
                                     dm_cst.DISP_MIN_GRID
                                 ].values
                             ),
                             "global_disp_max": np.nanmax(
                                 disp_range_grid[0, 0][
                                     dm_cst.DISP_MAX_GRID
                                 ].values
                             ),
                         },
-                    }
+                    },
                 }
             }
             self.orchestrator.update_out_info(updating_dict)
             logging.info(
                 "Compute disparity: number tiles: {}".format(
                     epipolar_disparity_map.shape[1]
                     * epipolar_disparity_map.shape[0]
                 )
             )
 
             nb_total_tiles_roi = 0
 
+            # broadcast grids
+            broadcasted_disp_range_grid = self.orchestrator.cluster.scatter(
+                disp_range_grid
+            )
+
             # Generate disparity maps
             for col in range(epipolar_disparity_map.shape[1]):
                 for row in range(epipolar_disparity_map.shape[0]):
                     use_tile = False
                     if type(None) not in (
                         type(epipolar_images_left[row, col]),
                         type(epipolar_images_right[row, col]),
@@ -1108,15 +1120,15 @@
                             epipolar_disparity_map[row, col]
                         ) = self.orchestrator.cluster.create_task(
                             compute_disparity_wrapper
                         )(
                             epipolar_images_left[row, col],
                             epipolar_images_right[row, col],
                             self.corr_config,
-                            disp_range_grid,
+                            broadcasted_disp_range_grid,
                             saving_info=full_saving_info,
                             compute_disparity_masks=compute_disparity_masks,
                             generate_performance_map=(
                                 self.generate_performance_map
                             ),
                             perf_ambiguity_threshold=(
                                 self.perf_ambiguity_threshold
```

### Comparing `cars-0.7.5/cars/applications/dense_matching/dense_matching.py` & `cars-0.7.6/cars/applications/dense_matching/dense_matching.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dense_matching/dense_matching_constants.py` & `cars-0.7.6/cars/applications/dense_matching/dense_matching_constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from cars.core import constants_disparity as disp_cst
 
 # USED VARIABLES
 
 
 DENSE_MATCHING_RUN_TAG = "dense_matching_run"
+DENSE_MATCHING_PARAM_TAG = "dense_matching_param"
 
 # grids disp
 DISP_MIN_GRID = "disp_min_grid"
 DISP_MAX_GRID = "disp_max_grid"
 
 
 # PARAMS
```

### Comparing `cars-0.7.5/cars/applications/dense_matching/dense_matching_tools.py` & `cars-0.7.6/cars/applications/dense_matching/dense_matching_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dense_matching/loaders/__init__.py` & `cars-0.7.6/cars/applications/dense_matching/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dense_matching/loaders/config_census_sgm.json` & `cars-0.7.6/cars/applications/dense_matching/loaders/config_census_sgm.json`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dense_matching/loaders/config_mccnn.json` & `cars-0.7.6/cars/applications/dense_matching/loaders/config_mccnn.json`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/dense_matching/loaders/pandora_loader.py` & `cars-0.7.6/cars/applications/dense_matching/loaders/pandora_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,26 +36,29 @@
     concat_conf,
     get_config_pipeline,
     update_conf,
 )
 from pandora.img_tools import get_metadata
 from pandora.state_machine import PandoraMachine
 
+from cars.core import constants_disparity as cst_disp
+
 
 class PandoraLoader:
     """
     PandoraLoader
 
     """
 
-    def __init__(
+    def __init__(  # noqa: C901
         self,
         conf=None,
         method_name=None,
         generate_performance_map=False,
+        generate_confidence_intervals=False,
         perf_eta_max_ambiguity=0.99,
         perf_eta_max_risk=0.25,
         perf_eta_step=0.04,
     ):
         """
         Init function of PandoraLoader
 
@@ -70,15 +73,20 @@
 
         """
 
         self.pandora_config = None
 
         uses_cars_pandora_conf = False
 
-        if conf is None:
+        if isinstance(conf, str):
+            # load file
+            with open(conf, "r", encoding="utf8") as fstream:
+                conf = json.load(fstream)
+
+        elif conf is None:
             uses_cars_pandora_conf = True
             package_path = os.path.dirname(__file__)
 
             if "mccnn" in method_name:
                 # Use mccn_conf
 
                 conf_file_path = os.path.join(package_path, "config_mccnn.json")
@@ -99,47 +107,107 @@
                 logging.error(
                     "No method named {} in pandora loader".format(method_name)
                 )
                 raise NameError(
                     "No method named {} in pandora loader".format(method_name)
                 )
 
-        # add performance map in configuration
-        if generate_performance_map:
-            perf_conf = {
-                "cost_volume_confidence.cars_1": {
-                    "confidence_method": "ambiguity",
-                    "eta_max": perf_eta_max_ambiguity,
-                    "eta_step": perf_eta_step,
-                },
-                "cost_volume_confidence.cars_2": {
-                    "confidence_method": "risk",
-                    "eta_max": perf_eta_max_risk,
-                    "eta_step": perf_eta_step,
-                },
+        # add required confidences
+        basic_ambiguity_conf = {
+            "cost_volume_confidence": {
+                "confidence_method": "ambiguity",
+                "eta_max": 0.7,
+                "eta_step": 0.01,
+            }
+        }
+
+        perf_ambiguity_conf = {
+            "cost_volume_confidence.cars_1": {
+                "confidence_method": "ambiguity",
+                "eta_max": perf_eta_max_ambiguity,
+                "eta_step": perf_eta_step,
             }
+        }
 
-            conf["pipeline"] = overload_pandora_conf_with_confidence(
-                conf["pipeline"], perf_conf
-            )
-
-        else:
-            # by default generate ambiguity user uses
-            # cars loaded configurations
+        perf_risk_conf = {
+            "cost_volume_confidence.cars_2": {
+                "confidence_method": "risk",
+                "eta_max": perf_eta_max_risk,
+                "eta_step": perf_eta_step,
+            }
+        }
+
+        intervals_conf = {
+            "cost_volume_confidence.cars_3": {
+                "confidence_method": "interval_bounds",
+            }
+        }
+
+        confidences = {}
+        if generate_performance_map:
+            confidences.update(perf_ambiguity_conf)
+            confidences.update(perf_risk_conf)
+        if generate_confidence_intervals:
             if uses_cars_pandora_conf:
-                ambi_conf = {
-                    "cost_volume_confidence": {
-                        "confidence_method": "ambiguity",
-                        "eta_max": 0.7,
-                        "eta_step": 0.01,
-                    },
+                confidences.update(perf_ambiguity_conf)
+                confidences.update(intervals_conf)
+            else:
+                flag_intervals = True
+                # Check consistency between generate_confidence_intervals
+                # and loader_conf
+                for key, item in conf["pipeline"].items():
+                    if cst_disp.CONFIDENCE_KEY in key:
+                        if item["confidence_method"] == cst_disp.INTERVAL:
+                            flag_intervals = False
+                if flag_intervals:
+                    raise KeyError(
+                        "Interval computation has been requested "
+                        "but no interval confidence is in the "
+                        "dense_matching_configuration loader_conf"
+                    )
+        if (
+            not generate_performance_map
+            and not generate_confidence_intervals
+            and uses_cars_pandora_conf
+        ):
+            confidences.update(basic_ambiguity_conf)
+
+        conf["pipeline"] = overload_pandora_conf_with_confidence(
+            conf["pipeline"], confidences
+        )
+
+        if generate_confidence_intervals:
+            # To ensure the consistency between the disparity map
+            # and the intervals, the median filter for intervals
+            # must be similar to the median filter. The filter is
+            # added at the end of the conf as it is applied during
+            # the disp_map state.
+            try:
+                filter_size = conf["pipeline"]["filter"]["filter_size"]
+            except KeyError:
+                filter_size = 3
+
+            conf_filter_interval = {
+                "filter.cars_3": {
+                    "filter_method": "median_for_intervals",
+                    "filter_size": filter_size,
+                    "interval_indicator": "cars_3",
+                    "regularization": True,
+                    "ambiguity_indicator": "cars_1",
                 }
-                conf["pipeline"] = overload_pandora_conf_with_confidence(
-                    conf["pipeline"], ambi_conf
-                )
+            }
+            pipeline_dict = OrderedDict()
+            pipeline_dict.update(conf["pipeline"])
+            # Filter is placed after validation in config
+            # and should be placed before.
+            # However it does not have any incidence on operation
+            if uses_cars_pandora_conf:
+                pipeline_dict.update(conf_filter_interval)
+
+            conf["pipeline"] = pipeline_dict
 
         # Check conf
         self.pandora_config = conf
 
     def get_conf(self):
         """
         Get pandora configuration used
@@ -287,12 +355,11 @@
 
     # get position of key "disparity"
     if "disparity" not in conf_keys:
         raise RuntimeError("disparity key not in pandora configuration")
     disp_index = conf_keys.index("disparity")
 
     # move to end every key from disparity
-
     for ind in range(disp_index, len(conf_keys)):
         out_dict.move_to_end(conf_keys[ind])
 
     return out_dict
```

### Comparing `cars-0.7.5/cars/applications/grid_generation/__init__.py` & `cars-0.7.6/cars/applications/grid_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/grid_generation/epipolar_grid_generation.py` & `cars-0.7.6/cars/applications/grid_generation/epipolar_grid_generation.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/grid_generation/grid_constants.py` & `cars-0.7.6/cars/applications/grid_generation/grid_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/grid_generation/grid_correction.py` & `cars-0.7.6/cars/applications/grid_generation/grid_correction.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/grid_generation/grid_generation.py` & `cars-0.7.6/cars/applications/grid_generation/grid_generation.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/grid_generation/grids.py` & `cars-0.7.6/cars/applications/grid_generation/grids.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/holes_detection/__init__.py` & `cars-0.7.6/cars/applications/holes_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/holes_detection/cloud_to_bbox.py` & `cars-0.7.6/cars/applications/holes_detection/cloud_to_bbox.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/holes_detection/holes_detection.py` & `cars-0.7.6/cars/applications/holes_detection/holes_detection.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/holes_detection/holes_detection_tools.py` & `cars-0.7.6/cars/applications/holes_detection/holes_detection_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/point_cloud_fusion/__init__.py` & `cars-0.7.6/cars/applications/point_cloud_fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/point_cloud_fusion/cloud_fusion_constants.py` & `cars-0.7.6/cars/applications/point_cloud_fusion/cloud_fusion_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/point_cloud_fusion/mapping_to_terrain_tiles.py` & `cars-0.7.6/cars/applications/point_cloud_fusion/mapping_to_terrain_tiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     pc_tif_tools,
     point_cloud_tools,
 )
 from cars.applications.point_cloud_fusion.point_cloud_fusion import (
     PointCloudFusion,
 )
 from cars.core import inputs, projection, tiling
+from cars.core.utils import safe_makedirs
 from cars.data_structures import cars_dataset
 
 
 class MappingToTerrainTiles(
     PointCloudFusion, short_name="mapping_to_terrain_tiles"
 ):
     """
@@ -317,26 +318,25 @@
                     "color"
                 ]
                 if color_file is not None:
                     color_type = inputs.rasterio_get_image_type(color_file)
                     merged_point_cloud.attributes["color_type"] = color_type
 
             # Save objects
+            pc_file_name = None
             if self.save_points_cloud_as_csv or self.save_points_cloud_as_laz:
                 # Points cloud file name
                 # TODO in input conf file
                 pc_file_name = os.path.join(
                     self.orchestrator.out_dir, "points_cloud"
                 )
-                self.orchestrator.add_to_save_lists(
-                    pc_file_name,
-                    None,
-                    merged_point_cloud,
-                    cars_ds_name="merged_points_cloud",
-                    save_points_cloud_by_pair=self.save_points_cloud_by_pair,
+                safe_makedirs(pc_file_name)
+                pc_file_name = os.path.join(pc_file_name, "pc")
+                self.orchestrator.add_to_compute_lists(
+                    merged_point_cloud, cars_ds_name="merged_points_cloud"
                 )
 
             # Get saving infos in order to save tiles when they are computed
             [saving_info] = self.orchestrator.get_saving_infos(
                 [merged_point_cloud]
             )
             for col in range(merged_point_cloud.shape[1]):
@@ -408,16 +408,24 @@
                             required_point_clouds,
                             epsg,
                             xmin=terrain_region[0],
                             ymin=terrain_region[1],
                             xmax=terrain_region[2],
                             ymax=terrain_region[3],
                             margins=margins,
-                            save_pc_as_laz=self.save_points_cloud_as_laz,
-                            save_pc_as_csv=self.save_points_cloud_as_csv,
+                            save_points_cloud_as_laz=(
+                                self.save_points_cloud_as_laz
+                            ),
+                            save_points_cloud_as_csv=(
+                                self.save_points_cloud_as_csv
+                            ),
+                            save_points_cloud_by_pair=(
+                                self.save_points_cloud_by_pair
+                            ),
+                            point_cloud_file_name=pc_file_name,
                             saving_info=full_saving_info,
                             source_pc_names=source_pc_names,
                         )
 
             # Sort tiles according to rank TODO remove or implement it ?
 
             # Raise an error if no tiles has been found
@@ -474,16 +482,18 @@
     point_clouds,
     epsg,
     xmin: float = None,
     ymin: float = None,
     xmax: float = None,
     ymax: float = None,
     margins: float = 0,
-    save_pc_as_laz: bool = False,
-    save_pc_as_csv: bool = False,
+    save_points_cloud_as_laz: bool = False,
+    save_points_cloud_as_csv: bool = False,
+    save_points_cloud_by_pair: bool = False,
+    point_cloud_file_name=None,
     saving_info=None,
     source_pc_names=None,
 ):
     """
     Wrapper for points clouds fusion step :
     - Convert a list of clouds to correct epsg
 
@@ -503,18 +513,22 @@
         (if None, will be estimated by the function)
     :param xmax: xmax of the rasterization grid
         (if None, will be estimated by the function)
     :param ymax: ymax of the rasterization grid
         (if None, will be estimated by the function)
     :param margins: margins needed for tiles, meter or degree
     :type margins: float
-    :param save_pc_as_laz: save point cloud as laz
-    :type save_pc_as_laz: bool
-    :param save_pc_as_csv: save point cloud as csv
-    :type save_pc_as_csv: bool
+    :param save_points_cloud_as_laz: save point cloud as laz
+    :type save_points_cloud_as_laz: bool
+    :param save_points_cloud_as_csv: save point cloud as csv
+    :type save_points_cloud_as_csv: bool
+    :param save_points_cloud_by_pair: save point cloud as pair
+    :type save_points_cloud_by_pair: bool
+    :param point_cloud_file_name: point cloud filename
+    :type point_cloud_file_name: str
     :param saving_info: informations about CarsDataset ID.
     :type saving_info: dict
     :param source_pc_names: source point cloud name (correspond to pair_key)
     :type source_pc_names: list str
 
     :return: merged points cloud dataframe with:
             - cst.X
@@ -577,17 +591,26 @@
     attributes = {
         "epsg": cloud_epsg,
         "xmin": xmin,
         "xmax": xmax,
         "ymin": ymin,
         "ymax": ymax,
         "color_type": color_type,
-        "save_points_cloud_as_laz": save_pc_as_laz,
-        "save_points_cloud_as_csv": save_pc_as_csv,
+        "save_points_cloud_as_laz": save_points_cloud_as_laz,
+        "save_points_cloud_as_csv": save_points_cloud_as_csv,
         "source_pc_names": source_pc_names,
         "number_of_pc": len(source_pc_names),
     }
     cars_dataset.fill_dataframe(
         pc_pandas, saving_info=saving_info, attributes=attributes
     )
 
+    # save point cloud in worker
+    if save_points_cloud_as_laz or save_points_cloud_as_csv:
+        cars_dataset.run_save_points(
+            pc_pandas,
+            point_cloud_file_name,
+            save_points_cloud_by_pair=save_points_cloud_by_pair,
+            overwrite=True,
+        )
+
     return pc_pandas
```

### Comparing `cars-0.7.5/cars/applications/point_cloud_fusion/pc_tif_tools.py` & `cars-0.7.6/cars/applications/point_cloud_fusion/pc_tif_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/point_cloud_fusion/point_cloud_fusion.py` & `cars-0.7.6/cars/applications/point_cloud_fusion/point_cloud_fusion.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         :param list_epipolar_points_cloud: list with points clouds\
             Each CarsDataset contains:
 
             - N x M Delayed tiles. \
                 Each tile will be a future xarray Dataset containing:
 
                 - data : with keys : "x", "y", "z", "corr_msk" \
-                    optional: "color", "msk",
+                    optional: "color", "msk", "z_inf", "z_sup"
                 - attrs with keys: "margins", "epi_full_size", "epsg"
             - attributes containing: "disp_lower_bound",  "disp_upper_bound" \
                 "elevation_delta_lower_bound", "elevation_delta_upper_bound"
         :type list_epipolar_points_cloud: list(CarsDataset) filled with
           xr.Dataset
         :param bounds: terrain bounds
         :type bounds: list
@@ -142,14 +142,14 @@
             CarsDataset contains:
 
             - Z x W Delayed tiles\
                 Each tile will be a future pandas DataFrame containing:
 
                 - data : with keys : "x", "y", "z", "corr_msk" \
                     optional: "clr", "msk", "data_valid","coord_epi_geom_i",\
-                     "coord_epi_geom_j","idx_im_epi"
+                     "coord_epi_geom_j","idx_im_epi", "z_inf", "z_sup"
                 - attrs with keys: "epsg"
             - attributes containing: "bounds", "epsg"
 
         :rtype: CarsDataset filled with pandas.DataFrame
 
         """
```

### Comparing `cars-0.7.5/cars/applications/point_cloud_fusion/point_cloud_tools.py` & `cars-0.7.6/cars/applications/point_cloud_fusion/point_cloud_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+# pylint: disable=too-many-lines
 """
 This module is responsible for the transition between triangulation and
 rasterization steps
 """
-# pylint: disable=too-many-lines
+
 
 # Standard imports
 import logging
 from typing import List, Tuple, Union
 
 # Third party imports
 import numpy as np
@@ -157,15 +158,15 @@
         cloud_indexes_with_types.update(
             {cst.POINTS_CLOUD_COORD_EPI_GEOM_I: "uint16"}
         )
 
     cloud_indexes = list(cloud_indexes_with_types.keys())
 
     # iterate through input clouds
-    combined_cloud = np.zeros((0, len(cloud_indexes)), dtype=np.float64)
+    combined_cloud = np.zeros((0, len(cloud_indexes)))
     nb_points = 0
     for cloud_global_id, points_cloud in zip(  # noqa: B905
         cloud_ids, cloud_list
     ):
         full_x = points_cloud[cst.X]
         full_y = points_cloud[cst.Y]
         full_z = points_cloud[cst.Z]
@@ -394,14 +395,16 @@
                      cst.POINTS_CLOUD_COORD_EPI_GEOM_I,\
                      cst.POINTS_CLOUD_COORD_EPI_GEOM_J,\
                      cst.POINTS_CLOUD_ID_IM_EPI]\
             The pixel position of the xyz point in the original epipolar\
             image (coord_epi_geom_i, coord_epi_geom_j) are added\
             to the dataframe along with the index of its original cloud\
             in the cloud_list input.
+        - if confidence intervals on Z in input, then\
+            [cst.Z_INF, cst.Z_SUP] are also added to the labels
 
 
     :param dsm_epsg: epsg code for the CRS of the final output raster
     :param xmin: xmin of the rasterization grid
         (if None, the whole clouds are combined)
     :param xmax: xmax of the rasterization grid
         (if None, the whole clouds are combined)
@@ -439,15 +442,15 @@
                 cst.POINTS_CLOUD_ID_IM_EPI: "uint16",
             }
         )
 
     cloud_indexes = list(cloud_indexes_with_types.keys())
 
     # Iterate through input clouds
-    combined_cloud = np.zeros((0, len(cloud_indexes)), dtype=np.float16)
+    combined_cloud = np.zeros((0, len(cloud_indexes)))
     nb_points = 0
     for cloud_global_id, (cloud_list_id, points_cloud) in zip(  # noqa: B905
         cloud_id, enumerate(cloud_list)
     ):
         full_x = points_cloud[cst.X].values
         full_y = points_cloud[cst.Y].values
         full_z = points_cloud[cst.Z].values
@@ -504,31 +507,53 @@
                 (bbox[2] - bbox[0] + 1) * (bbox[3] - bbox[1] + 1),
             )
         )
         flatten_cloud[cloud_indexes.index(cst.X), :] = np.ravel(crop_x)
         flatten_cloud[cloud_indexes.index(cst.Y), :] = np.ravel(crop_y)
         flatten_cloud[cloud_indexes.index(cst.Z), :] = np.ravel(crop_z)
 
+        if (cst.Z_INF in cloud_indexes) and (cst.Z_SUP in cloud_indexes):
+            full_z_inf = points_cloud[cst.Z_INF].values
+            full_z_sup = points_cloud[cst.Z_SUP].values
+            crop_z_inf = full_z_inf[
+                bbox[0] : bbox[2] + 1, bbox[1] : bbox[3] + 1
+            ]
+            crop_z_sup = full_z_sup[
+                bbox[0] : bbox[2] + 1, bbox[1] : bbox[3] + 1
+            ]
+            flatten_cloud[cloud_indexes.index(cst.Z_INF), :] = np.ravel(
+                crop_z_inf
+            )
+            flatten_cloud[cloud_indexes.index(cst.Z_SUP), :] = np.ravel(
+                crop_z_sup
+            )
+
         # add index of original point cloud
         flatten_cloud[cloud_indexes.index(cst.POINTS_CLOUD_GLOBAL_ID), :] = (
             cloud_global_id
         )
 
         # add additional information to point cloud
         arrays_to_add_to_points_cloud = [
             (cst.EPI_COLOR, cst.POINTS_CLOUD_CLR_KEY_ROOT),
             (cst.EPI_MSK, cst.POINTS_CLOUD_MSK),
             (cst.EPI_CLASSIFICATION, cst.POINTS_CLOUD_CLASSIF_KEY_ROOT),
             (cst.EPI_FILLING, cst.POINTS_CLOUD_FILLING_KEY_ROOT),
         ]
 
+        # add confidence layers
         for array_name in points_cloud:
             if cst.EPI_CONFIDENCE_KEY_ROOT in array_name:
                 arrays_to_add_to_points_cloud.append((array_name, array_name))
 
+        # add denoising info layers
+        for array_name in points_cloud:
+            if cst.EPI_DENOISING_INFO_KEY_ROOT in array_name:
+                arrays_to_add_to_points_cloud.append((array_name, array_name))
+
         for input_band, output_column in arrays_to_add_to_points_cloud:
             add_information_to_cloud(
                 points_cloud,
                 cloud_indexes,
                 bbox,
                 flatten_cloud,
                 input_band,
@@ -593,14 +618,19 @@
     cloud_indexes_with_types = {
         cst.POINTS_CLOUD_GLOBAL_ID: "uint16",
         cst.X: "float64",
         cst.Y: "float64",
         cst.Z: "float64",
     }
 
+    # Add Z_inf and Z_sup if intervals have been computed
+    if (cst.Z_INF in cloud_sample) and (cst.Z_SUP in cloud_sample):
+        cloud_indexes_with_types[cst.Z_INF] = "float64"
+        cloud_indexes_with_types[cst.Z_SUP] = "float64"
+
     # Add mask index
     if cst.EPI_MSK in cloud_sample:
         cloud_indexes_with_types[cst.POINTS_CLOUD_MSK] = "uint8"
 
     # Add color indexes
     if cst.EPI_COLOR in cloud_sample:
         band_color = list(cloud_sample.coords[cst.BAND_IM].to_numpy())
```

### Comparing `cars-0.7.5/cars/applications/point_cloud_outliers_removing/__init__.py` & `cars-0.7.6/cars/applications/point_cloud_outliers_removing/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/point_cloud_outliers_removing/outlier_removing_tools.py` & `cars-0.7.6/cars/applications/point_cloud_outliers_removing/outlier_removing_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/point_cloud_outliers_removing/pc_out_removing.py` & `cars-0.7.6/cars/applications/point_cloud_outliers_removing/pc_out_removing.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import logging
 import os
 from abc import ABCMeta, abstractmethod
 from typing import Dict
 
 from cars.applications.application import Application
 from cars.applications.application_template import ApplicationTemplate
+from cars.core.utils import safe_makedirs
 from cars.data_structures import cars_dataset
 
 
 @Application.register("point_cloud_outliers_removing")
 class PointCloudOutliersRemoving(ApplicationTemplate, metaclass=ABCMeta):
     """
     PointCloudOutliersRemoving
@@ -172,31 +173,30 @@
 
         # Get tiling grid
         filtered_point_cloud.tiling_grid = merged_points_cloud.tiling_grid
         filtered_point_cloud.generate_none_tiles()
         filtered_point_cloud.attributes = merged_points_cloud.attributes.copy()
 
         # Save objects
+        pc_file_name = None
         if save_points_cloud_as_laz or save_points_cloud_as_csv:
             # Points cloud file name
             # TODO in input conf file
             pc_file_name = os.path.join(
                 self.orchestrator.out_dir,
                 "points_cloud_post_" + app_name + "_removing",
             )
-            self.orchestrator.add_to_save_lists(
-                pc_file_name,
-                None,
+            safe_makedirs(pc_file_name)
+            pc_file_name = os.path.join(pc_file_name, "pc")
+            self.orchestrator.add_to_compute_lists(
                 filtered_point_cloud,
                 cars_ds_name="filtered_merged_pc_" + app_name,
-                # pylint: disable=E1101
-                save_points_cloud_by_pair=self.save_points_cloud_by_pair,
             )
 
-        return filtered_point_cloud
+        return filtered_point_cloud, pc_file_name
 
     @abstractmethod
     def run(
         self,
         merged_points_cloud,
         orchestrator=None,
     ):
```

### Comparing `cars-0.7.5/cars/applications/point_cloud_outliers_removing/points_removing_constants.py` & `cars-0.7.6/cars/applications/point_cloud_outliers_removing/points_removing_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/point_cloud_outliers_removing/small_components.py` & `cars-0.7.6/cars/applications/point_cloud_outliers_removing/small_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -291,15 +291,15 @@
             self.orchestrator = ocht.Orchestrator(
                 orchestrator_conf={"mode": "sequential"}
             )
         else:
             self.orchestrator = orchestrator
 
         if merged_points_cloud.dataset_type == "points":
-            (filtered_point_cloud) = self.__register_dataset__(
+            (filtered_point_cloud, pc_file_name) = self.__register_dataset__(
                 merged_points_cloud,
                 self.save_points_cloud_as_laz,
                 self.save_points_cloud_as_csv,
                 app_name="small_components",
             )
 
             # Get saving infos in order to save tiles when they are computed
@@ -331,14 +331,18 @@
                         )(
                             merged_points_cloud[row, col],
                             self.connection_distance,
                             self.nb_points_threshold,
                             self.clusters_distance_threshold,
                             self.save_points_cloud_as_laz,
                             self.save_points_cloud_as_csv,
+                            save_points_cloud_by_pair=(
+                                self.save_points_cloud_by_pair
+                            ),
+                            point_cloud_file_name=pc_file_name,
                             saving_info=full_saving_info,
                         )
 
         else:
             logging.error(
                 "PointCloudOutliersRemoving application doesn't support"
                 "this input data "
@@ -351,14 +355,16 @@
 def small_components_removing_wrapper(
     cloud,
     connection_distance,
     nb_points_threshold,
     clusters_distance_threshold,
     save_points_cloud_as_laz,
     save_points_cloud_as_csv,
+    save_points_cloud_by_pair: bool = False,
+    point_cloud_file_name=None,
     saving_info=None,
 ):
     """
     Statistical outlier removing
 
     :param cloud: cloud to filter
     :type cloud: pandas DataFrame
@@ -368,14 +374,18 @@
     :type nb_points_threshold: int
     :param clusters_distance_threshold:
     :type clusters_distance_threshold: float
     :param save_points_cloud_as_laz: activation of point cloud saving to laz
     :type save_points_cloud_as_laz: bool
     :param save_points_cloud_as_csv: activation of point cloud saving to csv
     :type save_points_cloud_as_csv: bool
+    :param save_points_cloud_by_pair: save point cloud as pair
+    :type save_points_cloud_by_pair: bool
+    :param point_cloud_file_name: point cloud filename
+    :type point_cloud_file_name: str
     :param saving_info: saving infos
     :type saving_info: dict
 
     :return: filtered cloud
     :rtype: pandas DataFrame
 
     """
@@ -430,8 +440,17 @@
     cloud_attributes["epsg"] = current_epsg
     cloud_attributes["save_points_cloud_as_laz"] = save_points_cloud_as_laz
     cloud_attributes["save_points_cloud_as_csv"] = save_points_cloud_as_csv
     cars_dataset.fill_dataframe(
         new_cloud, saving_info=saving_info, attributes=cloud_attributes
     )
 
+    # save point cloud in worker
+    if save_points_cloud_as_laz or save_points_cloud_as_csv:
+        cars_dataset.run_save_points(
+            new_cloud,
+            point_cloud_file_name,
+            save_points_cloud_by_pair=save_points_cloud_by_pair,
+            overwrite=True,
+        )
+
     return new_cloud
```

### Comparing `cars-0.7.5/cars/applications/point_cloud_outliers_removing/statistical.py` & `cars-0.7.6/cars/applications/point_cloud_outliers_removing/statistical.py`

 * *Files 11% similar despite different names*

```diff
@@ -262,15 +262,15 @@
             self.orchestrator = ocht.Orchestrator(
                 orchestrator_conf={"mode": "sequential"}
             )
         else:
             self.orchestrator = orchestrator
 
         if merged_points_cloud.dataset_type == "points":
-            (filtered_point_cloud) = self.__register_dataset__(
+            (filtered_point_cloud, pc_file_name) = self.__register_dataset__(
                 merged_points_cloud,
                 self.save_points_cloud_as_laz,
                 self.save_points_cloud_as_csv,
                 app_name="statistical",
             )
 
             # Get saving infos in order to save tiles when they are computed
@@ -307,14 +307,18 @@
                             statistical_removing_wrapper
                         )(
                             merged_points_cloud[row, col],
                             self.k,
                             self.std_dev_factor,
                             self.save_points_cloud_as_laz,
                             self.save_points_cloud_as_csv,
+                            save_points_cloud_by_pair=(
+                                self.save_points_cloud_by_pair
+                            ),
+                            point_cloud_file_name=pc_file_name,
                             saving_info=full_saving_info,
                         )
 
         else:
             logging.error(
                 "PointCloudOutliersRemoving application doesn't support"
                 "this input data "
@@ -326,14 +330,16 @@
 
 def statistical_removing_wrapper(
     cloud,
     statistical_k,
     std_dev_factor,
     save_points_cloud_as_laz,
     save_points_cloud_as_csv,
+    save_points_cloud_by_pair: bool = False,
+    point_cloud_file_name=None,
     saving_info=None,
 ):
     """
     Statistical outlier removing
 
     :param cloud: cloud to filter
     :type cloud: pandas DataFrame
@@ -341,14 +347,18 @@
     :type statistical_k: float
     :param std_dev_factor: std factor
     :type std_dev_factor: float
     :param save_points_cloud_as_laz: activation of point cloud saving to laz
     :type save_points_cloud_as_laz: bool
     :param save_points_cloud_as_csv: activation of point cloud saving to csv
     :type save_points_cloud_as_csv: bool
+    :param save_points_cloud_by_pair: save point cloud as pair
+    :type save_points_cloud_by_pair: bool
+    :param point_cloud_file_name: point cloud filename
+    :type point_cloud_file_name: str
     :param saving_info: saving infos
     :type saving_info: dict
 
     :return: filtered cloud
     :rtype: pandas DataFrame
 
     """
@@ -397,8 +407,17 @@
     cloud_attributes["save_points_cloud_as_laz"] = save_points_cloud_as_laz
     cloud_attributes["save_points_cloud_as_csv"] = save_points_cloud_as_csv
 
     cars_dataset.fill_dataframe(
         new_cloud, saving_info=saving_info, attributes=cloud_attributes
     )
 
+    # save point cloud in worker
+    if save_points_cloud_as_laz or save_points_cloud_as_csv:
+        cars_dataset.run_save_points(
+            new_cloud,
+            point_cloud_file_name,
+            save_points_cloud_by_pair=save_points_cloud_by_pair,
+            overwrite=True,
+        )
+
     return new_cloud
```

### Comparing `cars-0.7.5/cars/applications/rasterization/__init__.py` & `cars-0.7.6/cars/applications/rasterization/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/rasterization/point_cloud_rasterization.py` & `cars-0.7.6/cars/applications/rasterization/point_cloud_rasterization.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/rasterization/rasterization_constants.py` & `cars-0.7.6/cars/applications/sparse_matching/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+# !/usr/bin/env python
 # coding: utf8
 #
 # Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of CARS
 # (see https://github.com/CNES/cars).
 #
@@ -15,32 +15,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-file contains all the constants used in rasterization module
+CARS core matching module init file
 """
+# flake8: noqa: F401
 
-RASTERIZATION_RUN_TAG = "rasterization_run"
+from cars.applications.sparse_matching.sparse_matching import SparseMatching
 
-# Params
-METHOD = "method"
-DSM_RADIUS = "dsm_radius"
-SIGMA = "sigma"
-GRID_POINTS_DIVISION_FACTOR = "grid_points_division_factor"
-RESOLUTION = "resolution"
-
-
-# Run infos
-EPSG_TAG = "epsg"
-DSM_TAG = "dsm"
-COLOR_TAG = "color"
-MSK_TAG = "msk"
-CONFIDENCE_TAG = "disparity_confidence"
-DSM_MEAN_TAG = "dsm_mean"
-DSM_STD_TAG = "dsm_std"
-DSM_N_PTS_TAG = "dsm_n_pts"
-DSM_POINTS_IN_CELL_TAG = "dsm_points_in_cell"
-DSM_NO_DATA_TAG = "dsm_no_data"
-COLOR_NO_DATA_TAG = "color_no_data"
+from . import sift
```

### Comparing `cars-0.7.5/cars/applications/rasterization/rasterization_tools.py` & `cars-0.7.6/cars/applications/rasterization/rasterization_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+# pylint: disable=too-many-lines
+
 """
 This module is responsible for the rasterization step:
 - it contains all functions related to 3D representation on a 2D raster grid
 TODO: refactor in several files and remove too-many-lines
 """
-# pylint: disable=too-many-lines
+
 
 # Standard imports
 import logging
 from typing import List, Tuple, Union
 
 # Third party imports
 import numpy as np
@@ -85,15 +87,15 @@
     ystart: float = None,
     xsize: int = None,
     ysize: int = None,
     sigma: float = None,
     radius: int = 1,
     dsm_no_data: int = np.nan,
     color_no_data: int = np.nan,
-    msk_no_data: int = 65535,
+    msk_no_data: int = 255,
     list_computed_layers: List[str] = None,
     source_pc_names: List[str] = None,
 ) -> xr.Dataset:
     """
     Wrapper of simple_rasterization
     that has xarray.Dataset as inputs and outputs.
 
@@ -276,29 +278,36 @@
     # 2. confidences
     confidences_indexes = find_indexes_in_point_cloud(
         cloud, cst.POINTS_CLOUD_CONFIDENCE_KEY_ROOT, list_computed_layers
     )
     values_bands.extend(confidences_indexes)
     split_indexes.append(len(confidences_indexes))
 
-    # 3. mask
+    # 3. confidence interval
+    interval_indexes = find_indexes_in_point_cloud(
+        cloud, cst.POINTS_CLOUD_INTERVALS_KEY_ROOT, list_computed_layers
+    )
+    values_bands.extend(interval_indexes)
+    split_indexes.append(len(interval_indexes))
+
+    # 4. mask
     msk_indexes = find_indexes_in_point_cloud(
         cloud, cst.POINTS_CLOUD_MSK, list_computed_layers
     )
     values_bands.extend(msk_indexes)
     split_indexes.append(len(msk_indexes))
 
-    # 4. classification
+    # 5. classification
     classif_indexes = find_indexes_in_point_cloud(
         cloud, cst.POINTS_CLOUD_CLASSIF_KEY_ROOT, list_computed_layers
     )
     values_bands.extend(classif_indexes)
     split_indexes.append(len(classif_indexes))
 
-    # 5. source point cloud
+    # 6. source point cloud
     # Fill the dataframe with additional columns :
     # each column refers to a point cloud id
     number_of_pc = cars_dataset.get_attributes_dataframe(cloud)["number_of_pc"]
     if cst.POINTS_CLOUD_GLOBAL_ID in cloud.columns and (
         (list_computed_layers is None)
         or substring_in_list(
             list_computed_layers, cst.POINTS_CLOUD_SOURCE_KEY_ROOT
@@ -315,15 +324,15 @@
 
     source_pc_indexes = find_indexes_in_point_cloud(
         cloud, cst.POINTS_CLOUD_SOURCE_KEY_ROOT, list_computed_layers
     )
     values_bands.extend(source_pc_indexes)
     split_indexes.append(len(source_pc_indexes))
 
-    # 6. filling
+    # 7. filling
     filling_indexes = find_indexes_in_point_cloud(
         cloud, cst.POINTS_CLOUD_FILLING_KEY_ROOT, list_computed_layers
     )
     values_bands.extend(filling_indexes)
 
     values = (
         cloud.loc[:, values_bands].values.T
@@ -343,24 +352,28 @@
             resolution,
             radius,
             sigma,
         )
     )
 
     # pylint: disable=unbalanced-tuple-unpacking
-    out, confidences, msk, classif, source_pc, filling = np.split(
+    out, confidences, interval, msk, classif, source_pc, filling = np.split(
         out, np.cumsum(split_indexes), axis=-1
     )
 
     confidences_out = None
     if len(confidences_indexes) > 0:
         confidences_out = {}
         for k, key in enumerate(confidences_indexes):
             confidences_out[key] = confidences[..., k]
 
+    interval_out = None
+    if len(interval_indexes) > 0:
+        interval_out = interval
+
     msk_out = None
     if len(msk_indexes) > 0:
         msk_out = np.ceil(msk)
 
     classif_out = None
     if len(classif_indexes) > 0:
         classif_out = np.ceil(classif)
@@ -381,14 +394,15 @@
         nb_pts_in_disc,
         nb_pts_in_cell,
         msk_out,
         clr_indexes,
         classif_out,
         classif_indexes,
         confidences_out,
+        interval_out,
         source_pc_out,
         filling_out,
         filling_indexes,
     )
 
 
 def create_raster_dataset(
@@ -408,14 +422,15 @@
     n_pts: np.ndarray,
     n_in_cell: np.ndarray,
     msk: np.ndarray = None,
     band_im: List[str] = None,
     classif: np.ndarray = None,
     band_classif: List[str] = None,
     confidences: np.ndarray = None,
+    interval: np.ndarray = None,
     source_pc: np.ndarray = None,
     source_pc_names: List[str] = None,
     filling: np.ndarray = None,
     band_filling: List[str] = None,
 ) -> xr.Dataset:
     """
     Create final raster xarray dataset
@@ -486,19 +501,23 @@
     raster_out[cst.RASTER_HGT_STD_DEV] = xr.DataArray(
         stdev[..., 0], coords=raster_coords, dims=raster_dims
     )
 
     # add each band statistics
     for i_layer in range(1, n_layers):
         raster_out["{}{}".format(cst.RASTER_BAND_MEAN, i_layer)] = xr.DataArray(
-            mean[..., i_layer], coords=raster_coords, dims=raster_dims
+            mean[..., i_layer],
+            coords=raster_coords,
+            dims=raster_dims,
         )
         raster_out["{}{}".format(cst.RASTER_BAND_STD_DEV, i_layer)] = (
             xr.DataArray(
-                stdev[..., i_layer], coords=raster_coords, dims=raster_dims
+                stdev[..., i_layer],
+                coords=raster_coords,
+                dims=raster_dims,
             )
         )
 
     raster_out[cst.RASTER_NB_PTS] = xr.DataArray(n_pts, dims=raster_dims)
     raster_out[cst.RASTER_NB_PTS_IN_CELL] = xr.DataArray(
         n_in_cell, dims=raster_dims
     )
@@ -525,14 +544,24 @@
         # update raster output with classification data
         raster_out = xr.merge((raster_out, classif_out))
 
     if confidences is not None:  # rasterizer produced color output
         for key in confidences:
             raster_out[key] = xr.DataArray(confidences[key], dims=raster_dims)
 
+    if interval is not None:
+        hgt_inf = np.nan_to_num(interval[0], nan=hgt_no_data)
+        raster_out[cst.RASTER_HGT_INF] = xr.DataArray(
+            hgt_inf, coords=raster_coords, dims=raster_dims
+        )
+        hgt_sup = np.nan_to_num(interval[1], nan=hgt_no_data)
+        raster_out[cst.RASTER_HGT_SUP] = xr.DataArray(
+            hgt_sup, coords=raster_coords, dims=raster_dims
+        )
+
     if source_pc is not None and source_pc_names is not None:
         source_pc = np.nan_to_num(source_pc, nan=msk_no_data)
         source_pc_out = xr.Dataset(
             {
                 cst.RASTER_SOURCE_PC: (
                     [cst.BAND_SOURCE_PC, cst.Y, cst.X],
                     source_pc,
@@ -572,15 +601,15 @@
     y_start: float,
     x_size: int,
     y_size: int,
     sigma: float = None,
     radius: int = 1,
     hgt_no_data: int = -32768,
     color_no_data: int = 0,
-    msk_no_data: int = 65535,
+    msk_no_data: int = 255,
     list_computed_layers: List[str] = None,
     source_pc_names: List[str] = None,
 ) -> Union[xr.Dataset, None]:
     """
     Rasterize a point cloud with its color bands to a Dataset
     that also contains quality statistics.
 
@@ -624,14 +653,15 @@
         n_pts,
         n_in_cell,
         msk,
         clr_indexes,
         classif,
         classif_indexes,
         confidences,
+        interval,
         source_pc,
         filling,
         filling_indexes,
     ) = compute_vector_raster_and_stats(
         cloud,
         x_start,
         y_start,
@@ -663,14 +693,18 @@
     if msk is not None:
         msk = msk.reshape(shape_out)
 
     if confidences is not None:
         for key in confidences:
             confidences[key] = confidences[key].reshape(shape_out)
 
+    if interval is not None:
+        interval = interval.reshape(shape_out + (-1,))
+        interval = np.moveaxis(interval, 2, 0)
+
     if source_pc is not None:
         source_pc = source_pc.reshape(shape_out + (-1,))
         source_pc = np.moveaxis(source_pc, 2, 0)
 
     if filling is not None:
         filling = filling.reshape(shape_out + (-1,))
         filling = np.moveaxis(filling, 2, 0)
@@ -693,14 +727,15 @@
         n_pts,
         n_in_cell,
         msk,
         clr_indexes,
         classif,
         classif_indexes,
         confidences,
+        interval,
         source_pc,
         source_pc_names,
         filling,
         filling_indexes,
     )
 
     return raster_out
```

### Comparing `cars-0.7.5/cars/applications/rasterization/simple_gaussian.py` & `cars-0.7.6/cars/applications/rasterization/simple_gaussian.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,27 +14,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+# pylint: disable=too-many-lines
+
 """
 this module contains the dense_matching application class.
 """
-# pylint: disable=too-many-lines
 
 import collections
 
+# Third party imports
+import copy
+
 # Standard imports
 import logging
 import os
 from typing import List
 
-# Third party imports
 import numpy as np
 import rasterio as rio
 import xarray
 from affine import Affine
 from json_checker import Checker, Or
 
 # CARS imports
@@ -92,14 +95,15 @@
         self.msk_no_data = self.used_config["msk_no_data"]
         # Get if color, mask and stats are saved
         self.save_color = self.used_config["save_color"]
         self.save_stats = self.used_config["save_stats"]
         self.save_mask = self.used_config["save_mask"]
         self.save_classif = self.used_config["save_classif"]
         self.save_dsm = self.used_config["save_dsm"]
+        self.save_intervals = self.used_config["save_intervals"]
         self.save_confidence = self.used_config["save_confidence"]
         self.save_source_pc = self.used_config["save_source_pc"]
         self.save_filling = self.used_config["save_filling"]
 
         # Init orchestrator
         self.orchestrator = None
 
@@ -133,22 +137,23 @@
         )
         overloaded_conf["resolution"] = conf.get("resolution", 0.5)
 
         # get nodata values
         overloaded_conf["dsm_no_data"] = conf.get("dsm_no_data", -32768)
         overloaded_conf["color_no_data"] = conf.get("color_no_data", 0)
         overloaded_conf["color_dtype"] = conf.get("color_dtype", None)
-        overloaded_conf["msk_no_data"] = conf.get("msk_no_data", 65535)
+        overloaded_conf["msk_no_data"] = conf.get("msk_no_data", 255)
 
         # Get if color, mask and stats are saved
         overloaded_conf["save_color"] = conf.get("save_color", True)
         overloaded_conf["save_stats"] = conf.get("save_stats", False)
         overloaded_conf["save_mask"] = conf.get("save_mask", False)
         overloaded_conf["save_classif"] = conf.get("save_classif", False)
         overloaded_conf["save_dsm"] = conf.get("save_dsm", True)
+        overloaded_conf["save_intervals"] = conf.get("save_intervals", False)
         overloaded_conf["save_confidence"] = conf.get("save_confidence", False)
         overloaded_conf["save_source_pc"] = conf.get("save_source_pc", False)
         overloaded_conf["save_filling"] = conf.get("save_filling", False)
 
         overloaded_conf["compute_all"] = conf.get("compute_all", False)
         if overloaded_conf["compute_all"]:
             # all the layers will computed
@@ -171,14 +176,15 @@
             "color_no_data": int,
             "color_dtype": Or(None, str),
             "save_color": bool,
             "save_mask": bool,
             "save_classif": bool,
             "save_stats": bool,
             "save_dsm": bool,
+            "save_intervals": bool,
             "save_confidence": bool,
             "save_source_pc": bool,
             "save_filling": bool,
             "compute_all": bool,
         }
 
         # Check conf
@@ -260,27 +266,27 @@
 
             . CarsDataset contains:
 
             - Z x W Delayed tiles. \
                 Each tile will be a future pandas DataFrame containing:
 
                 - data with keys  "x", "y", "z", "corr_msk" \
-                    optional: "color", "mask", "data_valid",\
+                    optional: "color", "mask", "data_valid", "z_inf", "z_sup"\
                       "coord_epi_geom_i", "coord_epi_geom_j", "idx_im_epi"
                 - attrs with keys "epsg", "ysize", "xsize", "xstart", "ystart"
 
              - attributes containing "bounds", "ysize", "xsize", "epsg"
 
              OR
 
 
              Tuple(list of CarsDataset Arrays, bounds). With list of point
                 clouds:
                 list of CarsDataset of type array, with:
-                - data with keys x", "y", "z", "corr_msk" \
+                - data with keys x", "y", "z", "corr_msk", "z_inf", "z_sup"\
                     optional: "color", "mask", "data_valid",\
                       "coord_epi_geom_i", "coord_epi_geom_j", "idx_im_epi"
 
         :type points_clouds: CarsDataset filled with pandas.DataFrame
         :param epsg: epsg of raster data
         :type epsg: str
         :param orchestrator: orchestrator used
@@ -293,15 +299,16 @@
 
         :return: raster DSM. CarsDataset contains:
 
             - Z x W Delayed tiles. \
                 Each tile will be a future xarray Dataset containing:
 
                 - data : with keys : "hgt", "img", "raster_msk",optional : \
-                  "n_pts", "pts_in_cell", "hgt_mean", "hgt_stdev"
+                  "n_pts", "pts_in_cell", "hgt_mean", "hgt_stdev",\
+                  "hgt_inf", "hgt_sup"
                 - attrs with keys: "epsg"
             - attributes containing: None
 
         :rtype : CarsDataset filled with xr.Dataset
         """
 
         # Default orchestrator
@@ -315,15 +322,15 @@
         else:
             self.orchestrator = orchestrator
 
         # Check if input data is supported
         data_valid = True
         if isinstance(points_clouds, tuple):
             if isinstance(points_clouds[0][0], cars_dataset.CarsDataset):
-                if points_clouds[0][0].dataset_type != "arrays":
+                if points_clouds[0][0].dataset_type not in ("arrays", "points"):
                     data_valid = False
             else:
                 data_valid = False
         elif isinstance(points_clouds, cars_dataset.CarsDataset):
             if points_clouds.dataset_type != "points":
                 data_valid = False
         else:
@@ -372,22 +379,32 @@
         else:
             source_pc_names = points_clouds.attributes["source_pc_names"]
 
         # Save objects
         # Initialize files names
         # TODO get from config ?
         out_dsm_file_name = None
+        out_dsm_inf_file_name = None
+        out_dsm_sup_file_name = None
         out_weights_file_name = None
         out_clr_file_name = None
         out_msk_file_name = None
         out_confidence = None
         out_dsm_mean_file_name = None
         out_dsm_std_file_name = None
         out_dsm_n_pts_file_name = None
         out_dsm_points_in_cell_file_name = None
+        out_dsm_inf_mean_file_name = None
+        out_dsm_inf_std_file_name = None
+        out_dsm_inf_n_pts_file_name = None
+        out_dsm_inf_points_in_cell_file_name = None
+        out_dsm_sup_mean_file_name = None
+        out_dsm_sup_std_file_name = None
+        out_dsm_sup_n_pts_file_name = None
+        out_dsm_sup_points_in_cell_file_name = None
 
         if self.save_dsm:
             if dsm_file_name is not None:
                 out_dsm_file_name = dsm_file_name
             else:
                 out_dsm_file_name = os.path.join(
                     self.orchestrator.out_dir, "dsm.tif"
@@ -407,14 +424,40 @@
                 out_weights_file_name,
                 cst.RASTER_WEIGHTS_SUM,
                 terrain_raster,
                 dtype=np.float32,
                 nodata=0,
                 cars_ds_name="dsm_weights",
             )
+
+        # TODO Check that intervals indeed exist!
+        if self.save_intervals:
+            out_dsm_inf_file_name = os.path.join(
+                self.orchestrator.out_dir, "dsm_inf.tif"
+            )
+            self.orchestrator.add_to_save_lists(
+                out_dsm_inf_file_name,
+                cst.RASTER_HGT_INF,
+                terrain_raster,
+                dtype=np.float32,
+                nodata=self.dsm_no_data,
+                cars_ds_name="dsm_inf",
+            )
+            out_dsm_sup_file_name = os.path.join(
+                self.orchestrator.out_dir, "dsm_sup.tif"
+            )
+            self.orchestrator.add_to_save_lists(
+                out_dsm_sup_file_name,
+                cst.RASTER_HGT_SUP,
+                terrain_raster,
+                dtype=np.float32,
+                nodata=self.dsm_no_data,
+                cars_ds_name="dsm_sup",
+            )
+
         if self.save_color:
             if color_file_name is not None:
                 out_clr_file_name = color_file_name
             else:
                 out_clr_file_name = os.path.join(
                     self.orchestrator.out_dir, "clr.tif"
                 )
@@ -469,35 +512,124 @@
                 out_dsm_points_in_cell_file_name,
                 cst.RASTER_NB_PTS_IN_CELL,
                 terrain_raster,
                 dtype=np.uint16,
                 nodata=0,
                 cars_ds_name="dsm_pts_in_cells",
             )
+            if self.save_intervals:
+                out_dsm_inf_mean_file_name = os.path.join(
+                    self.orchestrator.out_dir, "dsm_inf_mean.tif"
+                )
+                out_dsm_inf_std_file_name = os.path.join(
+                    self.orchestrator.out_dir, "dsm_inf_std.tif"
+                )
+                out_dsm_inf_n_pts_file_name = os.path.join(
+                    self.orchestrator.out_dir, "dsm_inf_n_pts.tif"
+                )
+                out_dsm_inf_points_in_cell_file_name = os.path.join(
+                    self.orchestrator.out_dir, "dsm_inf_pts_in_cell.tif"
+                )
+                self.orchestrator.add_to_save_lists(
+                    out_dsm_inf_mean_file_name,
+                    cst.RASTER_HGT_INF_MEAN,
+                    terrain_raster,
+                    dtype=np.float32,
+                    nodata=self.dsm_no_data,
+                    cars_ds_name="dsm_inf_mean",
+                )
+                self.orchestrator.add_to_save_lists(
+                    out_dsm_inf_std_file_name,
+                    cst.RASTER_HGT_INF_STD_DEV,
+                    terrain_raster,
+                    dtype=np.float32,
+                    nodata=self.dsm_no_data,
+                    cars_ds_name="dsm_inf_std",
+                )
+                self.orchestrator.add_to_save_lists(
+                    out_dsm_inf_n_pts_file_name,
+                    cst.RASTER_NB_PTS,
+                    terrain_raster,
+                    dtype=np.uint16,
+                    nodata=0,
+                    cars_ds_name="dsm_inf_n_pts",
+                )
+                self.orchestrator.add_to_save_lists(
+                    out_dsm_inf_points_in_cell_file_name,
+                    cst.RASTER_NB_PTS_IN_CELL,
+                    terrain_raster,
+                    dtype=np.uint16,
+                    nodata=0,
+                    cars_ds_name="dsm_inf_pts_in_cells",
+                )
+                out_dsm_sup_mean_file_name = os.path.join(
+                    self.orchestrator.out_dir, "dsm_sup_mean.tif"
+                )
+                out_dsm_sup_std_file_name = os.path.join(
+                    self.orchestrator.out_dir, "dsm_sup_std.tif"
+                )
+                out_dsm_sup_n_pts_file_name = os.path.join(
+                    self.orchestrator.out_dir, "dsm_sup_n_pts.tif"
+                )
+                out_dsm_sup_points_in_cell_file_name = os.path.join(
+                    self.orchestrator.out_dir, "dsm_sup_pts_in_cell.tif"
+                )
+                self.orchestrator.add_to_save_lists(
+                    out_dsm_sup_mean_file_name,
+                    cst.RASTER_HGT_SUP_MEAN,
+                    terrain_raster,
+                    dtype=np.float32,
+                    nodata=self.dsm_no_data,
+                    cars_ds_name="dsm_sup_mean",
+                )
+                self.orchestrator.add_to_save_lists(
+                    out_dsm_sup_std_file_name,
+                    cst.RASTER_HGT_SUP_STD_DEV,
+                    terrain_raster,
+                    dtype=np.float32,
+                    nodata=self.dsm_no_data,
+                    cars_ds_name="dsm_sup_std",
+                )
+                self.orchestrator.add_to_save_lists(
+                    out_dsm_sup_n_pts_file_name,
+                    cst.RASTER_NB_PTS,
+                    terrain_raster,
+                    dtype=np.uint16,
+                    nodata=0,
+                    cars_ds_name="dsm_sup_n_pts",
+                )
+                self.orchestrator.add_to_save_lists(
+                    out_dsm_sup_points_in_cell_file_name,
+                    cst.RASTER_NB_PTS_IN_CELL,
+                    terrain_raster,
+                    dtype=np.uint16,
+                    nodata=0,
+                    cars_ds_name="dsm_sup_pts_in_cells",
+                )
         if self.save_classif:
             out_classif_file_name = os.path.join(
                 self.orchestrator.out_dir, "classif.tif"
             )
             self.orchestrator.add_to_save_lists(
                 out_classif_file_name,
                 cst.RASTER_CLASSIF,
                 terrain_raster,
-                dtype=np.float32,
+                dtype=np.uint8,
                 nodata=self.msk_no_data,
                 cars_ds_name="dsm_classif",
             )
         if self.save_mask:
             out_msk_file_name = os.path.join(
                 self.orchestrator.out_dir, "msk.tif"
             )
             self.orchestrator.add_to_save_lists(
                 out_msk_file_name,
                 cst.RASTER_MSK,
                 terrain_raster,
-                dtype=np.uint16,
+                dtype=np.uint8,
                 nodata=self.msk_no_data,
                 cars_ds_name="dsm_mask",
             )
 
         if self.save_confidence:
             out_confidence = os.path.join(
                 self.orchestrator.out_dir, "confidence.tif"
@@ -515,26 +647,26 @@
             out_source_pc = os.path.join(
                 self.orchestrator.out_dir, "source_pc.tif"
             )
             self.orchestrator.add_to_save_lists(
                 out_source_pc,
                 cst.RASTER_SOURCE_PC,
                 terrain_raster,
-                dtype=np.float32,
+                dtype=np.uint8,
                 nodata=self.msk_no_data,
                 cars_ds_name="source_pc",
             )
 
         if self.save_filling:
             out_filling = os.path.join(self.orchestrator.out_dir, "filling.tif")
             self.orchestrator.add_to_save_lists(
                 out_filling,
                 cst.RASTER_FILLING,
                 terrain_raster,
-                dtype=np.float32,
+                dtype=np.uint8,
                 nodata=self.msk_no_data,
                 cars_ds_name="filling",
             )
 
         # Get saving infos in order to save tiles when they are computed
         [saving_info] = self.orchestrator.get_saving_infos([terrain_raster])
 
@@ -573,25 +705,39 @@
 
         # Add infos to orchestrator.out_json
         updating_dict = {
             application_constants.APPLICATION_TAG: {
                 raster_cst.RASTERIZATION_RUN_TAG: {
                     raster_cst.EPSG_TAG: epsg,
                     raster_cst.DSM_TAG: out_dsm_file_name,
+                    raster_cst.DSM_INF_TAG: out_dsm_inf_file_name,
+                    raster_cst.DSM_SUP_TAG: out_dsm_sup_file_name,
                     raster_cst.DSM_NO_DATA_TAG: float(self.dsm_no_data),
                     raster_cst.COLOR_NO_DATA_TAG: float(self.color_no_data),
                     raster_cst.COLOR_TAG: out_clr_file_name,
                     raster_cst.MSK_TAG: out_msk_file_name,
                     raster_cst.CONFIDENCE_TAG: out_confidence,
                     raster_cst.DSM_MEAN_TAG: out_dsm_mean_file_name,
                     raster_cst.DSM_STD_TAG: out_dsm_std_file_name,
                     raster_cst.DSM_N_PTS_TAG: out_dsm_n_pts_file_name,
                     raster_cst.DSM_POINTS_IN_CELL_TAG: (
                         out_dsm_points_in_cell_file_name
                     ),
+                    raster_cst.DSM_INF_MEAN_TAG: out_dsm_inf_mean_file_name,
+                    raster_cst.DSM_INF_STD_TAG: out_dsm_inf_std_file_name,
+                    raster_cst.DSM_INF_N_PTS_TAG: out_dsm_inf_n_pts_file_name,
+                    raster_cst.DSM_INF_POINTS_IN_CELL_TAG: (
+                        out_dsm_inf_points_in_cell_file_name
+                    ),
+                    raster_cst.DSM_SUP_MEAN_TAG: out_dsm_sup_mean_file_name,
+                    raster_cst.DSM_SUP_STD_TAG: out_dsm_sup_std_file_name,
+                    raster_cst.DSM_SUP_N_PTS_TAG: out_dsm_sup_n_pts_file_name,
+                    raster_cst.DSM_SUP_POINTS_IN_CELL_TAG: (
+                        out_dsm_sup_points_in_cell_file_name
+                    ),
                 },
             }
         }
         self.orchestrator.update_out_info(updating_dict)
 
         # Generate rasters
         if not isinstance(points_clouds, tuple):
@@ -702,15 +848,15 @@
     terrain_full_roi=None,
     list_computed_layers: List[str] = None,
     saving_info=None,
     sigma: float = None,
     radius: int = 1,
     dsm_no_data: int = np.nan,
     color_no_data: int = np.nan,
-    msk_no_data: int = 65535,
+    msk_no_data: int = 255,
     source_pc_names=None,
 ):
     """
     Wrapper for rasterization step :
     - Convert a list of clouds to correct epsg
     - Rasterize it with associated colors
 
@@ -740,31 +886,41 @@
     :param color_no_data: no data value to use in the final colored raster
     :param msk_no_data: no data value to use in the final mask image
     :param source_pc_names: list of names of points cloud before merging :
         name of sensors pair or name of point cloud file
     :return: digital surface model + projected colors
     :rtype: xr.Dataset
     """
+    # update attributes
+    attributes = copy.deepcopy(cloud.attrs)
+    attributes.update(attributes.get("attributes", {}))
+    if "attributes" in attributes:
+        del attributes["attributes"]
+    if "saving_info" in attributes:
+        del attributes["saving_info"]
 
     # convert back to correct epsg
     # If the points cloud is not in the right epsg referential, it is converted
     if isinstance(cloud, xarray.Dataset):
         # Transform Dataset to Dataframe
-        attributes = cloud.attrs
         cloud, cloud_epsg = point_cloud_tools.create_combined_cloud(
             [cloud], [attributes["cloud_id"]], epsg
         )
-        if "number_of_pc" not in attributes and source_pc_names is not None:
-            attributes["number_of_pc"] = len(source_pc_names)
-        cars_dataset.fill_dataframe(cloud, attributes=attributes)
     elif cloud is None:
         logging.warning("Input cloud is None")
         return None
     else:
-        cloud_epsg = cars_dataset.get_attributes_dataframe(cloud)["epsg"]
+        cloud_epsg = attributes.get("epsg")
+
+    if "number_of_pc" not in attributes and source_pc_names is not None:
+        attributes["number_of_pc"] = len(source_pc_names)
+
+    # update attributes
+    cloud.attrs = {}
+    cars_dataset.fill_dataframe(cloud, attributes=attributes)
 
     if epsg != cloud_epsg:
         projection.points_cloud_conversion_dataframe(cloud, cloud_epsg, epsg)
 
     # filter cloud
     if "mask" in cloud:
         cloud = cloud[cloud["mask"] == 0]
```

### Comparing `cars-0.7.5/cars/applications/resampling/__init__.py` & `cars-0.7.6/cars/applications/resampling/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/resampling/bicubic_resampling.py` & `cars-0.7.6/cars/applications/resampling/bicubic_resampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,35 +414,39 @@
             )
 
             self.orchestrator.add_to_save_lists(
                 os.path.join(pair_folder, "epi_img_left_mask.tif"),
                 cst.EPI_MSK,
                 epipolar_images_left,
                 cars_ds_name="epi_img_left_mask",
+                dtype=np.uint8,
             )
 
             self.orchestrator.add_to_save_lists(
                 os.path.join(pair_folder, "epi_img_left_classif.tif"),
                 cst.EPI_CLASSIFICATION,
                 epipolar_images_left,
                 cars_ds_name="epi_img_left_classif",
+                dtype=np.uint8,
             )
 
             self.orchestrator.add_to_save_lists(
                 os.path.join(pair_folder, "epi_img_right_mask.tif"),
                 cst.EPI_MSK,
                 epipolar_images_right,
                 cars_ds_name="epi_img_right_mask",
+                dtype=np.uint8,
             )
 
             self.orchestrator.add_to_save_lists(
                 os.path.join(pair_folder, "epi_img_right_classif.tif"),
                 cst.EPI_CLASSIFICATION,
                 epipolar_images_right,
                 cars_ds_name="epi_img_right_classif",
+                dtype=np.uint8,
             )
 
         if self.save_epipolar_color:
             self.orchestrator.add_to_save_lists(
                 os.path.join(pair_folder, "epi_color.tif"),
                 cst.EPI_COLOR,
                 epipolar_images_left,
@@ -517,14 +521,18 @@
             sensor_image_left,
             sensor_image_right,
             epi_tilling_grid,
             grid_left,
             grid_right,
         )
 
+        # broadcast grids
+        broadcasted_grid1 = self.orchestrator.cluster.scatter(grid1)
+        broadcasted_grid2 = self.orchestrator.cluster.scatter(grid2)
+
         # Generate Image pair
         for col in range(epipolar_images_left.shape[1]):
             for row in range(epipolar_images_left.shape[0]):
                 # Create polygon corresponding to tile
                 tile = epi_tilling_grid[row, col]
                 tile_roi_poly = Polygon(
                     [
@@ -570,16 +578,16 @@
                         left_overlap,
                         right_overlap,
                         left_window,
                         epipolar_size_x,
                         epipolar_size_y,
                         img1,
                         img2,
-                        grid1,
-                        grid2,
+                        broadcasted_grid1,
+                        broadcasted_grid2,
                         self.step,
                         used_disp_min=used_disp_min[row, col],
                         used_disp_max=used_disp_max[row, col],
                         add_color=add_color,
                         color1=color1,
                         mask1=mask1,
                         mask2=mask2,
@@ -768,19 +776,23 @@
     :type sensor_image_right: dict
 
     :return: left image bounds, right image bounds
     :rtype: tuple(list, list)
     """
 
     left_sensor_bounds = list(
-        inputs.rasterio_get_bounds(sensor_image_left[sens_cst.INPUT_IMG])
+        inputs.rasterio_get_bounds(
+            sensor_image_left[sens_cst.INPUT_IMG], apply_resolution_sign=True
+        )
     )
 
     right_sensor_bounds = list(
-        inputs.rasterio_get_bounds(sensor_image_right[sens_cst.INPUT_IMG])
+        inputs.rasterio_get_bounds(
+            sensor_image_right[sens_cst.INPUT_IMG], apply_resolution_sign=True
+        )
     )
 
     return left_sensor_bounds, right_sensor_bounds
 
 
 def check_tiles_in_sensor(
     sensor_image_left,
```

### Comparing `cars-0.7.5/cars/applications/resampling/resampling.py` & `cars-0.7.6/cars/applications/resampling/resampling.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/resampling/resampling_constants.py` & `cars-0.7.6/cars/applications/resampling/resampling_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/resampling/resampling_tools.py` & `cars-0.7.6/cars/applications/resampling/resampling_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/sparse_matching/__init__.py` & `cars-0.7.6/cars/orchestrator/cluster/mp_cluster/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# !/usr/bin/env python
+#!/usr/bin/env python
 # coding: utf8
 #
 # Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of CARS
 # (see https://github.com/CNES/cars).
 #
@@ -15,14 +15,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-CARS core matching module init file
+CARS multiprocessing cluster module init file
 """
 # flake8: noqa: F401
 
-from cars.applications.sparse_matching.sparse_matching import SparseMatching
 
-from . import sift
+from . import multiprocessing_cluster
```

### Comparing `cars-0.7.5/cars/applications/sparse_matching/sift.py` & `cars-0.7.6/cars/applications/sparse_matching/sift.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/sparse_matching/sparse_matching.py` & `cars-0.7.6/cars/applications/sparse_matching/sparse_matching.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/sparse_matching/sparse_matching_constants.py` & `cars-0.7.6/cars/applications/sparse_matching/sparse_matching_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/sparse_matching/sparse_matching_tools.py` & `cars-0.7.6/cars/applications/sparse_matching/sparse_matching_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/triangulation/__init__.py` & `cars-0.7.6/cars/applications/triangulation/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/triangulation/line_of_sight_intersection.py` & `cars-0.7.6/cars/applications/triangulation/line_of_sight_intersection.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 # Standard imports
 import logging
 import os
 from typing import Dict, Tuple
 
 # Third party imports
+import numpy as np
 import pandas
 import xarray as xr
 from json_checker import Checker
 
 # CARS imports
 import cars.orchestrator.orchestrator as ocht
 from cars.applications import application_constants
@@ -133,21 +134,23 @@
         sensor_image_right,
         epipolar_image,
         grid_left,
         grid_right,
         epipolar_disparity_map,
         epsg,
         geometry_plugin,
+        denoising_overload_fun=None,
         source_pc_names=None,
         orchestrator=None,
         pair_folder=None,
         pair_key="PAIR_0",
         uncorrected_grid_right=None,
         geoid_path=None,
         cloud_id=None,
+        intervals=None,
     ):
         """
         Run Triangulation application.
 
         Created left and right CarsDataset filled with xarray.Dataset,
         corresponding to 3D points clouds, stored on epipolar geometry grid.
 
@@ -198,35 +201,39 @@
                     Each tile will be a future pandas DataFrame containing:
 
                     - data : (L, 4) shape matches
                 - attributes containing:"disp_lower_bound","disp_upper_bound",\
                     "elevation_delta_lower_bound","elevation_delta_upper_bound"
 
         :type epipolar_disparity_map: CarsDataset
+        :param denoising_overload_fun: function to overload dataset
+        :type denoising_overload_fun: fun
         :param source_pc_names: source pc names
         :type source_pc_names: list[str]
         :param orchestrator: orchestrator used
         :param pair_folder: folder used for current pair
         :type pair_folder: str
         :param pair_key: pair key id
         :type pair_key: str
         :param uncorrected_grid_right: not corrected right epipolar grid
                 used if self.snap_to_img1
         :type uncorrected_grid_right: CarsDataset
         :param geoid_path: geoid path
         :type geoid_path: str
+        :param intervals: Either None or a List of 2 intervals indicators
+        :type intervals: None or [str, str]
 
         :return: points cloud \
                 The CarsDataset contains:
 
             - N x M Delayed tiles \
                 Each tile will be a future xarray Dataset containing:
 
                 - data : with keys : "x", "y", "z", "corr_msk"\
-                    optional: "color", "msk",
+                    optional: "color", "msk", "z_inf", "z_sup"
                 - attrs with keys: "margins", "epi_full_size", "epsg"
             - attributes containing: "disp_lower_bound",  "disp_upper_bound", \
                 "elevation_delta_lower_bound","elevation_delta_upper_bound"
 
         :rtype: Tuple(CarsDataset, CarsDataset)
         """
 
@@ -370,30 +377,47 @@
                         )
 
                     self.orchestrator.add_to_save_lists(
                         os.path.join(pair_folder, "epi_pc_X.tif"),
                         cst.X,
                         epipolar_points_cloud,
                         cars_ds_name="epi_pc_x",
+                        dtype=np.float64,
                     )
 
                     self.orchestrator.add_to_save_lists(
                         os.path.join(pair_folder, "epi_pc_Y.tif"),
                         cst.Y,
                         epipolar_points_cloud,
                         cars_ds_name="epi_pc_y",
+                        dtype=np.float64,
                     )
 
                     self.orchestrator.add_to_save_lists(
                         os.path.join(pair_folder, "epi_pc_Z.tif"),
                         cst.Z,
                         epipolar_points_cloud,
                         cars_ds_name="epi_pc_z",
+                        dtype=np.float64,
                     )
 
+                    if intervals is not None:
+                        self.orchestrator.add_to_save_lists(
+                            os.path.join(pair_folder, "epi_pc_Z_inf.tif"),
+                            cst.Z_INF,
+                            epipolar_points_cloud,
+                            cars_ds_name="epi_pc_z_inf",
+                        )
+                        self.orchestrator.add_to_save_lists(
+                            os.path.join(pair_folder, "epi_pc_Z_sup.tif"),
+                            cst.Z_SUP,
+                            epipolar_points_cloud,
+                            cars_ds_name="epi_pc_z_sup",
+                        )
+
                     self.orchestrator.add_to_save_lists(
                         os.path.join(pair_folder, "epi_pc_corr_msk.tif"),
                         cst.POINTS_CLOUD_CORR_MSK,
                         epipolar_points_cloud,
                         cars_ds_name="epi_pc_corr_msk",
                         optional_data=True,
                     )
@@ -401,30 +425,34 @@
                     self.orchestrator.add_to_save_lists(
                         os.path.join(pair_folder, "epi_pc_msk.tif"),
                         cst.EPI_MSK,
                         epipolar_points_cloud,
                         cars_ds_name="epi_pc_msk",
                         nodata=mask_cst.NO_DATA_IN_EPIPOLAR_RECTIFICATION,
                         optional_data=True,
+                        dtype=np.uint8,
                     )
 
                     self.orchestrator.add_to_save_lists(
                         os.path.join(pair_folder, "epi_classification.tif"),
                         cst.EPI_CLASSIFICATION,
                         epipolar_points_cloud,
                         cars_ds_name="epi_classification",
                         optional_data=True,
+                        dtype=np.uint8,
                     )
 
                     self.orchestrator.add_to_save_lists(
                         os.path.join(pair_folder, "epi_filling.tif"),
                         cst.EPI_FILLING,
                         epipolar_points_cloud,
                         cars_ds_name="epi_filling",
                         optional_data=True,
+                        dtype=np.uint8,
+                        nodata=255,
                     )
 
                     self.orchestrator.add_to_save_lists(
                         os.path.join(pair_folder, "epi_pc_color.tif"),
                         cst.EPI_COLOR,
                         epipolar_points_cloud,
                         cars_ds_name="epi_pc_color",
@@ -461,14 +489,27 @@
 
             geoid_data = read_geoid_file(geoid_path)
             # Broadcast geoid data to all dask workers
             geoid_data_futures = self.orchestrator.cluster.scatter(
                 geoid_data, broadcast=True
             )
 
+        # Determining if a lower disparity inf corresponds to a lower or higher
+        # hgt. It depends on the image pairing and geometrical models.
+        if (
+            intervals is not None
+        ) and geometry_plugin.sensors_arrangement_left_right(
+            sensor1, sensor2, geomodel1, geomodel2, grid_left, grid_right
+        ):
+            intervals[0], intervals[1] = intervals[1], intervals[0]
+
+        # broadcast grids
+        broadcasted_grid_left = self.orchestrator.cluster.scatter(grid_left)
+        broadcasted_grid_right = self.orchestrator.cluster.scatter(grid_right)
+
         for col in range(epipolar_disparity_map.shape[1]):
             for row in range(epipolar_disparity_map.shape[0]):
                 if epipolar_disparity_map[row, col] is not None:
                     # update saving infos  for potential replacement
                     full_saving_info = ocht.update_saving_infos(
                         saving_info, row=row, col=col
                     )
@@ -479,20 +520,22 @@
                         triangulation_wrapper
                     )(
                         epipolar_disparity_map[row, col],
                         sensor1,
                         sensor2,
                         geomodel1,
                         geomodel2,
-                        grid_left,
-                        grid_right,
+                        broadcasted_grid_left,
+                        broadcasted_grid_right,
                         geometry_plugin,
                         epsg,
                         geoid_data=geoid_data_futures,
+                        denoising_overload_fun=denoising_overload_fun,
                         cloud_id=cloud_id,
+                        intervals=intervals,
                         saving_info=full_saving_info,
                     )
 
         return epipolar_points_cloud
 
 
 def triangulation_wrapper(
@@ -502,15 +545,17 @@
     geomodel1,
     geomodel2,
     grid1,
     grid2,
     geometry_plugin,
     epsg,
     geoid_data: xr.Dataset = None,
+    denoising_overload_fun=None,
     cloud_id=None,
+    intervals=None,
     saving_info=None,
 ) -> Dict[str, Tuple[xr.Dataset, xr.Dataset]]:
     """
     Compute points clouds from image objects and disparity objects.
 
     :param disparity_object: Left disparity map dataset with :
             - cst_disp.MAP
@@ -530,26 +575,29 @@
     :param grid2: dataset of the secondary image grid file
     :type grid2: CarsDataset
     :param geometry_plugin: geometry plugin to use
     :type geometry_plugin: AbstractGeometry
     :param geoid_data: Geoid used for altimetric reference. Defaults to None
         for using ellipsoid as altimetric reference.
     :type geoid_data: str
-    :param snap_to_img1: If True, Lines of Sight of img2 are moved so as to
-                         cross those of img1
-    :type snap_to_img1: bool
+    :param intervals: Either None or a List of 2 intervals indicators
+        :type intervals: None or [str, str]
+    :param denoising_overload_fun: function to overload dataset
+    :type denoising_overload_fun: fun
 
     :return: Left disparity object
 
     Returned object is composed of :
         - dataset with :
             - cst.X
             - cst.Y
             - cst.Z
             - cst.EPI_COLOR
+            - cst.Z_INF (optional)
+            - cst.Z_SUP (optional)
     """
 
     # Get disparity maps
     disp_ref = disparity_object
 
     # Triangulate
     if isinstance(disp_ref, xr.Dataset):
@@ -561,14 +609,46 @@
             geomodel1,
             geomodel2,
             grid1,
             grid2,
             disp_ref,
         )
 
+        if intervals is not None:
+            points_inf = triangulation_tools.triangulate(
+                geometry_plugin,
+                sensor1,
+                sensor2,
+                geomodel1,
+                geomodel2,
+                grid1,
+                grid2,
+                disp_ref,
+                disp_key=intervals[0],
+            )
+
+            points_sup = triangulation_tools.triangulate(
+                geometry_plugin,
+                sensor1,
+                sensor2,
+                geomodel1,
+                geomodel2,
+                grid1,
+                grid2,
+                disp_ref,
+                disp_key=intervals[1],
+            )
+
+            points[cst.STEREO_REF][cst.Z_INF] = points_inf[cst.STEREO_REF][
+                cst.Z
+            ]
+            points[cst.STEREO_REF][cst.Z_SUP] = points_sup[cst.STEREO_REF][
+                cst.Z
+            ]
+
     elif isinstance(disp_ref, pandas.DataFrame):
         # Triangulate epipolar sparse matches
         points = {}
         points[cst.STEREO_REF] = triangulation_tools.triangulate_matches(
             geometry_plugin,
             sensor1,
             sensor2,
@@ -582,22 +662,39 @@
         logging.error(
             "Disp ref is neither xarray Dataset  nor pandas DataFrame"
         )
         raise TypeError(
             "Disp ref is neither xarray Dataset  nor pandas DataFrame"
         )
 
-    if geoid_data is not None:  # if user pass a geoid, use it a alt reference
+    if geoid_data is not None:  # if user pass a geoid, use it as alt reference
         for key, point in points.items():
             points[key] = triangulation_tools.geoid_offset(point, geoid_data)
 
     # Fill datasets
     pc_dataset = points[cst.STEREO_REF]
     pc_dataset.attrs["cloud_id"] = cloud_id
 
+    # Overload dataset with denoising fun
+    if denoising_overload_fun is not None:
+        if isinstance(pc_dataset, xr.Dataset):
+            denoising_overload_fun(
+                pc_dataset,
+                sensor1,
+                sensor2,
+                geomodel1,
+                geomodel2,
+                grid1,
+                grid2,
+                geometry_plugin,
+                disp_ref,
+            )
+        else:
+            raise RuntimeError("wrong pc type for denoising func")
+
     attributes = None
     if isinstance(disp_ref, pandas.DataFrame):
         # Conversion to UTM
         projection.points_cloud_conversion_dataframe(
             points[cst.STEREO_REF], points[cst.STEREO_REF].attrs[cst.EPSG], epsg
         )
         cloud_epsg = epsg
```

### Comparing `cars-0.7.5/cars/applications/triangulation/triangulation.py` & `cars-0.7.6/cars/applications/triangulation/triangulation.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,21 +100,23 @@
         sensor_image_right,
         epipolar_image,
         grid_left,
         grid_right,
         epipolar_disparity_map,
         epsg,
         geometry_plugin,
+        denoising_overload_fun=None,
         source_pc_names=None,
         orchestrator=None,
         pair_folder=None,
         pair_key="PAIR_0",
         uncorrected_grid_right=None,
         geoid_path=None,
         cloud_id=None,
+        intervals=None,
     ):
         """
         Run Triangulation application.
 
         Created left and right CarsDataset filled with xarray.Dataset,
         corresponding to 3D points clouds, stored on epipolar geometry grid.
 
@@ -165,34 +167,38 @@
                     Each tile will be a future pandas DataFrame containing:
 
                     - data : (L, 4) shape matches
                 - attributes containing:"disp_lower_bound","disp_upper_bound",\
                     "elevation_delta_lower_bound","elevation_delta_upper_bound"
 
         :type epipolar_disparity_map: CarsDataset
+        :param denoising_overload_fun: function to overload dataset
+        :type denoising_overload_fun: fun
         :param source_pc_names: source pc names
         :type source_pc_names: list[str]
         :param orchestrator: orchestrator used
         :param pair_folder: folder used for current pair
         :type pair_folder: str
         :param pair_key: pair key id
         :type pair_key: str
         :param uncorrected_grid_right: not corrected right epipolar grid
                 used if self.snap_to_img1
         :type uncorrected_grid_right: CarsDataset
         :param geoid_path: geoid path
         :type geoid_path: str
+        :param intervals: Either None or a List of 2 intervals indicators
+        :type intervals: None or [str, str]
 
         :return: points cloud \
                 The CarsDataset contains:
 
             - N x M Delayed tiles \
                 Each tile will be a future xarray Dataset containing:
 
                 - data : with keys : "x", "y", "z", "corr_msk"\
-                    optional: "color", "msk",
+                    optional: "color", "msk", "z_inf", "z_sup"
                 - attrs with keys: "margins", "epi_full_size", "epsg"
             - attributes containing: "disp_lower_bound",  "disp_upper_bound", \
                 "elevation_delta_lower_bound","elevation_delta_upper_bound"
 
         :rtype: Tuple(CarsDataset, CarsDataset)
         """
```

### Comparing `cars-0.7.5/cars/applications/triangulation/triangulation_constants.py` & `cars-0.7.6/cars/applications/triangulation/triangulation_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/applications/triangulation/triangulation_tools.py` & `cars-0.7.6/cars/applications/triangulation/triangulation_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     sensor1,
     sensor2,
     geomodel1,
     geomodel2,
     grid1,
     grid2,
     disp_ref: xr.Dataset,
+    disp_key: str = cst_disp.MAP,
 ) -> Dict[str, xr.Dataset]:
     """
     This function will perform triangulation from a disparity map
 
     :param geometry_plugin: geometry plugin to use
     :type geometry_plugin: AbstractGeometry
     :param sensor1: path to left sensor image
@@ -65,28 +66,38 @@
     :param grid1: dataset of the reference image grid file
     :type grid1: CarsDataset
     :param grid2: dataset of the secondary image grid file
     :type grid2: CarsDataset
     :param disp_ref: left to right disparity map dataset
     :param im_ref_msk_ds: reference image dataset (image and
                           mask (if indicated by the user) in epipolar geometry)
+    :param disp_key: disparity key in the dataset\
+            usually set to cst_disp.MAP, but can be a disparity interval bound
     :returns: point_cloud as a dictionary of dataset containing:
 
         - Array with shape (roi_size_x,roi_size_y,3), with last dimension \
           corresponding to longitude, latitude and elevation
         - Array with shape (roi_size_x,roi_size_y) with output mask
         - Array for color (optional): only if color1 is not None
 
     The dictionary keys are :
 
         - 'ref' to retrieve the dataset built from the left to \
            right disparity map
         - 'sec' to retrieve the dataset built from the right to \
            left disparity map (if provided in input)
     """
+
+    if disp_key != cst_disp.MAP:
+        # Switching the variable names so the desired disparity is named 'disp'
+        # It does not modifies the dataset outside of this function
+        disp_ref = disp_ref.rename_vars(
+            {disp_key: cst_disp.MAP, cst_disp.MAP: disp_key}
+        )
+
     point_clouds = {}
     point_clouds[cst.STEREO_REF] = compute_points_cloud(
         geometry_plugin,
         sensor1,
         sensor2,
         geomodel1,
         geomodel2,
```

### Comparing `cars-0.7.5/cars/cars.py` & `cars-0.7.6/cars/cars.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/conf/__init__.py` & `cars-0.7.6/cars/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/conf/geoid/egm96.grd` & `cars-0.7.6/cars/conf/geoid/egm96.grd`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/conf/input_parameters.py` & `cars-0.7.6/cars/conf/input_parameters.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/conf/mask_cst.py` & `cars-0.7.6/cars/conf/mask_cst.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/core/__init__.py` & `cars-0.7.6/cars/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/core/cars_logging.py` & `cars-0.7.6/cars/core/cars_logging.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/core/constants_disparity.py` & `cars-0.7.6/cars/core/constants_disparity.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 """
 CARS Disparity Constants module
 """
 
 # disparity map
 MAP = "disp"
 CONFIDENCE = "confidence"
+CONFIDENCE_KEY = "cost_volume_confidence"
+INTERVAL = "interval_bounds"
+INTERVAL_INF = "confidence_from_interval_bounds_inf"
+INTERVAL_SUP = "confidence_from_interval_bounds_sup"
 EPI_DISP_MIN_GRID = "disp_min_grid"
 EPI_DISP_MAX_GRID = "disp_max_grid"
 
 # disparity mask
 VALID = "disp_msk"
 FILLING = "filling"
 INVALID_REF = "msk_invalid_ref"
```

### Comparing `cars-0.7.5/cars/core/datasets.py` & `cars-0.7.6/cars/core/datasets.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/core/geometry/__init__.py` & `cars-0.7.6/cars/core/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/core/geometry/abstract_geometry.py` & `cars-0.7.6/cars/core/geometry/abstract_geometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import rasterio as rio
 import xarray as xr
 from scipy import interpolate
 from scipy.interpolate import LinearNDInterpolator
 from shapely.geometry import Polygon
 
 from cars.core import constants as cst
+from cars.core import constants_disparity as cst_disp
 from cars.core import inputs, outputs
 from cars.data_structures import cars_dataset
 
 
 class AbstractGeometry(metaclass=ABCMeta):
     """
     AbstractGeometry
@@ -78,16 +79,19 @@
                 cls.available_plugins[geometry_plugin]
             )
         return super().__new__(cls)
 
     def __init__(
         self, geometry_plugin, dem=None, geoid=None, default_alt=None, **kwargs
     ):
+
         self.plugin_name = geometry_plugin
         self.dem = dem
+        self.dem_roi = None
+        self.dem_roi_epsg = None
         self.geoid = geoid
         self.default_alt = default_alt
         self.kwargs = kwargs
 
     @classmethod
     def register_subclass(cls, short_name: str):
         """
@@ -341,16 +345,16 @@
             grid_data = grid[0, 0]
             row_dep = grid_data[:, :, 1]
             col_dep = grid_data[:, :, 0]
 
             # Get step
             step_col = grid.attributes["grid_spacing"][1]
             step_row = grid.attributes["grid_spacing"][0]
-            ori_col = step_col / 2
-            ori_row = step_row / 2
+            ori_col = grid.attributes["grid_origin"][1]
+            ori_row = grid.attributes["grid_origin"][0]
             last_row = ori_row + step_row * grid_data.shape[0]
             last_col = ori_col + step_col * grid_data.shape[1]
 
         else:
             raise RuntimeError(
                 "Grid type {} not a path or CarsDataset".format(type(grid))
             )
@@ -530,14 +534,70 @@
         :param geomodel: path and attributes for geomodel
         :param lat_coord: latitute Coordinate list
         :param lon_coord: longitude Coordinates list
         :param z_coord: Z Altitude list
         :return: X  / Y / Z Coordinates list in input image as a numpy array
         """
 
+    def sensors_arrangement_left_right(
+        self, sensor1, sensor2, geomodel1, geomodel2, grid_left, grid_right
+    ):
+        """
+        Determine the arrangement of sensors, either:
+        (double slashes represent Lines Of Sight)
+        +---------------------+---------------------+
+        |    Arrangement 1    |    Arrangement 2    |
+        |  sensor1   sensor2  |   sensor2  sensor1  |
+        |   \\ \\    //       |       \\    // //   |
+        |    \\ \\  //        |        \\  // //    |
+        |     \\ \\// <-- z_2 | z_1 --> \\// //     |
+        |      \\ //          |          \\ //      |
+        |       \\/   <-- z_1 | z_2 -->   \\/       |
+        +---------------------+---------------------+
+        This allows to know if a lower disparity corresponds to a lower or
+        higher hgt. It depends on the image pairing and geometrical models.
+        A fake triangulation determines z_1 and z_2.
+        If z_1 < z_2 then the sensors are in arrangement 1
+        If z_2 < z_1 then the sensors are in arrangement 2
+
+        :param sensor1: path to left sensor image
+        :param sensor2: path to right sensor image
+        :param geomodel1: path and attributes for left geomodel
+        :param geomodel2: path and attributes for right geomodel
+        :param grid1: path or dataset for epipolar grid of sensor1
+        :param grid2: path or dataset for epipolar grid of sensor2
+
+        :return: boolean indicating if sensors are in arrangement 1 or not
+        """
+        # Create a fake disparity dataset, where the two LOS from
+        # sensor1 are associated with the same LOS from sensor2
+        fake_disp = xr.Dataset(
+            data_vars={
+                cst_disp.MAP: (
+                    [cst.ROW, cst.COL],
+                    np.array([[1, 0]], dtype=float),
+                )
+            },
+            coords={cst.ROW: [0], cst.COL: [0, 1]},
+            attrs={cst.ROI: [0, 0, 2, 1], cst.EPI_FULL_SIZE: [2, 1]},
+        )
+        fake_triangulation = self.triangulate(
+            sensor1,
+            sensor2,
+            geomodel1,
+            geomodel2,
+            cst.DISP_MODE,
+            fake_disp,
+            grid_left,
+            grid_right,
+            roi_key=cst.ROI,
+        )
+        # True if arrangement 1, False if arrangement 2
+        return fake_triangulation[0, 0, 2] < fake_triangulation[0, 1, 2]
+
     def image_envelope(self, sensor, geomodel, shp=None):
         """
         Export the image footprint to a shapefile
 
         :param sensor: path to sensor image
         :param geomodel: path and attributes for geometrical model
         :param shp: Path to the output shapefile
```

### Comparing `cars-0.7.5/cars/core/geometry/otb_geometry.py` & `cars-0.7.6/cars/core/geometry/otb_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,25 @@
     """
     OTB geometry class
     """
 
     # TODO: remove the hard-coded import in the steps/__init__.py if this class
     # is removed from CARS
 
+    def __init__(
+        self, geometry_plugin, dem=None, geoid=None, default_alt=None, **kwargs
+    ):
+        super().__init__(
+            geometry_plugin,
+            dem=dem,
+            geoid=geoid,
+            default_alt=default_alt,
+            **kwargs
+        )
+
     @property
     def conf_schema(self):
         """
         Returns the input configuration fields required by the geometry plugin
         as a json checker schema. The available fields are defined in the
         cars/conf/input_parameters.py file
```

### Comparing `cars-0.7.5/cars/core/geometry/shareloc_geometry.py` & `cars-0.7.6/cars/core/geometry/shareloc_geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 """
 Shareloc geometry sub class : CARS geometry wrappers functions to shareloc ones
 """
 
 import logging
 from typing import List, Tuple, Union
 
+import bindings_cpp
 import numpy as np
 import rasterio as rio
 import shareloc.geofunctions.rectification as rectif
 import xarray as xr
 from json_checker import Checker
 from shareloc.dtm_reader import dtm_reader
 from shareloc.geofunctions import localization
-from shareloc.geofunctions.dtm_intersection import DTMIntersection
 from shareloc.geofunctions.triangulation import epipolar_triangulation
 from shareloc.geomodels.geomodel import GeoModel
 from shareloc.geomodels.grid import Grid
 from shareloc.geomodels.rpc import RPC
 from shareloc.image import Image
 
 from cars.core import constants as cst
@@ -62,41 +62,57 @@
         dem=None,
         geoid=None,
         default_alt=None,
         pairs_for_roi=None,
     ):
         super().__init__(geometry_plugin)
 
-        roi = None
+        self.dem_roi = None
+        self.roi_shareloc = None
         self.elevation = None
 
-        if dem is not None:
-            # Get dem epsg
-            dem_epsg = inputs.rasterio_get_epsg(dem)
+        # compute roi only when generating geometry object with dem
+        # even if dem is None
+        if geoid is not None and pairs_for_roi is not None:
+            self.dem_roi_epsg = 4326
+            if dem is not None:
+                # Get dem epsg
+                self.dem_roi_epsg = inputs.rasterio_get_epsg(dem)
+
+            self.roi_shareloc = self.get_roi(
+                pairs_for_roi, self.dem_roi_epsg, margin=0.012
+            )
+            # change convention
+            self.dem_roi = [
+                self.roi_shareloc[1],
+                self.roi_shareloc[0],
+                self.roi_shareloc[3],
+                self.roi_shareloc[2],
+            ]
 
-            if pairs_for_roi is not None:
-                roi = self.get_roi(pairs_for_roi, dem_epsg)
+        if dem is not None:
 
             # fill_nodata option should be set when dealing with void in DTM
             # see shareloc DTM limitations in sphinx doc for further details
             dtm_image = dtm_reader(
                 dem,
                 geoid,
-                read_data=True,
-                roi=roi,
+                roi=self.roi_shareloc,
                 roi_is_in_physical_space=True,
                 fill_nodata="mean",
                 fill_value=0.0,
             )
-            self.elevation = DTMIntersection(
-                dtm_image.epsg,
-                dtm_image.alt_data,
-                dtm_image.nb_rows,
-                dtm_image.nb_columns,
-                dtm_image.transform,
+            self.elevation = (
+                bindings_cpp.DTMIntersection(  # pylint: disable=I1101
+                    dtm_image.epsg,
+                    dtm_image.alt_data,
+                    dtm_image.nb_rows,
+                    dtm_image.nb_columns,
+                    dtm_image.transform,
+                )
             )
         else:
             self.elevation = default_alt
 
     def get_roi(self, pairs_for_roi, epsg, margin=0.006):
         """
         Compute region of interest for intersection of DEM
@@ -111,15 +127,15 @@
         coords_list = []
         for image1, geomodel1, image2, geomodel2 in pairs_for_roi:
             # Footprint of left image
             coords_list.extend(self.image_envelope(image1, geomodel1))
             # Footprint of right image
             coords_list.extend(self.image_envelope(image2, geomodel2))
             # Epipolar extent
-            image1 = Image(image1)
+            image1 = SharelocGeometry.load_image(image1)
             geomodel1 = self.load_geom_model(geomodel1)
             geomodel2 = self.load_geom_model(geomodel2)
             epipolar_extent = rectif.get_epipolar_extent(
                 image1, geomodel1, geomodel2
             )
             lat_min, lon_min, lat_max, lon_max = list(epipolar_extent)
             coords_list.extend([(lon_min, lat_min), (lon_max, lat_max)])
@@ -160,14 +176,18 @@
         geomodel = model[GEO_MODEL_PATH_TAG]
         # Use RPC Type if none are used
         if model.get(GEO_MODEL_TYPE_TAG):
             geomodel_type = model[GEO_MODEL_TYPE_TAG]
         else:
             geomodel_type = RPC_TYPE
 
+        # Use RPCoptim class to use optimized C++ direct localizations
+        if geomodel_type == "RPC":
+            geomodel_type = "RPCoptim"
+
         shareloc_model = GeoModel(geomodel, geomodel_type)
 
         if shareloc_model is None:
             raise ValueError(f"Model {geomodel} could not be read by shareloc")
 
         return shareloc_model
 
@@ -176,15 +196,15 @@
         """
         Load the image using the Image class of Shareloc
 
         :param img: path to the image
         :return: The Image object
         """
         try:
-            shareloc_img = Image(img)
+            shareloc_img = Image(img, vertical_direction="north")
         except Exception as error:
             raise ValueError(f"Image type {img} is not supported") from error
 
         return shareloc_img
 
     @staticmethod
     def check_product_consistency(sensor: str, geomodel: dict) -> bool:
@@ -335,16 +355,16 @@
             - the disparity to altitude ratio as a float
 
         """
         # read inputs using shareloc
         shareloc_model1 = SharelocGeometry.load_geom_model(geomodel1)
         shareloc_model2 = SharelocGeometry.load_geom_model(geomodel2)
 
-        image1 = Image(sensor1)
-        image2 = Image(sensor2)
+        image1 = SharelocGeometry.load_image(sensor1)
+        image2 = SharelocGeometry.load_image(sensor2)
 
         # compute epipolar grids
         (
             grid1,
             grid2,
             [epipolar_size_y, epipolar_size_x],
             alt_to_disp_ratio,
@@ -406,15 +426,15 @@
         :param x_coord: X Coordinate in input image sensor
         :param y_coord: Y Coordinate in input image sensor
         :param z_coord: Z Altitude coordinate to take the image
         :return: Latitude, Longitude, Altitude coordinates as a numpy array
         """
         # load model and image with shareloc
         shareloc_model = SharelocGeometry.load_geom_model(geomodel)
-        shareloc_image = Image(sensor)
+        shareloc_image = SharelocGeometry.load_image(sensor)
 
         # perform direct localization operation
         loc = localization.Localization(
             shareloc_model,
             image=shareloc_image,
             elevation=self.elevation,
             epsg=4326,
@@ -453,24 +473,25 @@
         :param lon_coord: longitude Coordinates list
         :param z_coord: Z Altitude list
         :return: X  / Y / Z Coordinates list in input image as a numpy array
         """
 
         # load model and image with shareloc
         shareloc_model = SharelocGeometry.load_geom_model(geomodel)
-        shareloc_image = Image(sensor)
+        shareloc_image = SharelocGeometry.load_image(sensor)
 
         # perform inverse localization operation
         loc = localization.Localization(
             shareloc_model,
             image=shareloc_image,
             elevation=self.elevation,
             epsg=4326,
         )
-        row, col, alti = loc.inverse(
+        # Rows and columns order is inversed compared with OTB
+        col, row, alti = loc.inverse(
             lon_coord.astype(np.float64),
             lat_coord.astype(np.float64),
             h=z_coord.astype(np.float64),
             using_geotransform=True,
         )
 
         return row, col, alti
```

### Comparing `cars-0.7.5/cars/core/inputs.py` & `cars-0.7.6/cars/core/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,35 +175,55 @@
     :param raster_file: Image file
     :return: The size (width, height)
     """
     with rio.open(raster_file, "r") as descriptor:
         return (descriptor.width, descriptor.height)
 
 
-def rasterio_get_bounds(raster_file: str) -> Tuple[int, int]:
+def rasterio_get_bounds(
+    raster_file: str, apply_resolution_sign=False
+) -> Tuple[int, int]:
     """
     Get the bounds of an image (file)
 
     :param raster_file: Image file
     :return: The size (width, height)
     """
 
     # get sign of resolution
-    profile = rasterio_get_profile(raster_file)
-    transform = list(profile["transform"])
-    res_x = transform[0]
-    res_y = transform[4]
-    res_x /= abs(res_x)
-    res_y /= abs(res_y)
-    res_signs = np.array([res_x, res_y, res_x, res_y])
+    if apply_resolution_sign:
+        profile = rasterio_get_profile(raster_file)
+        transform = list(profile["transform"])
+        res_x = transform[0]
+        res_y = transform[4]
+        res_x /= abs(res_x)
+        res_y /= abs(res_y)
+        res_signs = np.array([res_x, res_y, res_x, res_y])
+    else:
+        res_signs = np.array([1, 1, 1, 1])
 
     with rio.open(raster_file, "r") as descriptor:
         return np.array(list(descriptor.bounds)) * res_signs
 
 
+def rasterio_get_epsg_code(
+    raster_file: str,
+) -> Tuple[int, int]:
+    """
+    Get the epsg code of an image (file)
+
+    :param raster_file: Image file
+    :return: epsg code
+    """
+
+    with rio.open(raster_file, "r") as descriptor:
+        epsg_code = descriptor.crs
+        return epsg_code
+
+
 def rasterio_get_list_min_max(raster_file: str) -> Tuple[int, int]:
     """
     Get the stats of an image (file)
 
     :param raster_file: Image file
     :return: The list min max
     """
```

### Comparing `cars-0.7.5/cars/core/otb_adapters.py` & `cars-0.7.6/cars/core/otb_adapters.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/core/outputs.py` & `cars-0.7.6/cars/core/outputs.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/core/preprocessing.py` & `cars-0.7.6/cars/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/core/projection.py` & `cars-0.7.6/cars/core/projection.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/core/roi_tools.py` & `cars-0.7.6/cars/core/roi_tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -187,7 +187,29 @@
                 "ROI file {} has an unsupported format".format(arg_roi_file)
             )
             raise AttributeError(
                 "ROI file {} has an unsupported format".format(arg_roi_file)
             )
 
     return roi_poly, roi_epsg
+
+
+def bounds_to_poly(bounds):
+    """
+    Convert bounds to polygon
+
+    :param bounds: bounds: [xmin, ymin, xmax, ymax]
+    :type: bounds: list
+
+    :return polygon
+    """
+
+    poly = Polygon(
+        [
+            [bounds[0], bounds[1]],
+            [bounds[0], bounds[3]],
+            [bounds[2], bounds[3]],
+            [bounds[2], bounds[1]],
+            [bounds[0], bounds[1]],
+        ]
+    )
+    return poly
```

### Comparing `cars-0.7.5/cars/core/tiling.py` & `cars-0.7.6/cars/core/tiling.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/core/utils.py` & `cars-0.7.6/cars/core/utils.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/data_structures/__init__.py` & `cars-0.7.6/cars/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/data_structures/cars_dataset.py` & `cars-0.7.6/cars/data_structures/cars_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+# pylint: disable=too-many-lines
 """
 cars_dataset module:
 
 """
-# pylint: disable=too-many-lines
+
 
 import copy
 import json
 import logging
 import math
 
 # Standard imports
@@ -588,24 +589,20 @@
     :param file_name: filename to save data to
     :type file_name: str
     :param overwrite: overwrite file
     :type overwrite: bool
 
     """
 
-    if overwrite:
-        # remove pickle file if already exists
-        if os.path.exists(file_name):
-            os.remove(file_name)
     # Save
     save_all_dataframe(
         future_result,
         file_name,
         save_points_cloud_by_pair=save_points_cloud_by_pair,
-        overwrite=False,
+        overwrite=overwrite,
     )
 
 
 def load_single_tile_array(tile_path_name: str) -> xr.Dataset:
     """
     Load a xarray tile
 
@@ -959,15 +956,14 @@
             file_name,
             (
                 str(dataframe.attrs["saving_info"]["cars_ds_col"])
                 + "_"
                 + str(dataframe.attrs["saving_info"]["cars_ds_row"])
             ),
         )
-
     if not save_points_cloud_by_pair:
         save_dataframe(dataframe, file_name, overwrite)
     else:
         pairing_indexes = set(np.array(dataframe["global_id"]).flat)
         source_pc_names = dataframe.attrs["attributes"]["source_pc_names"]
 
         for pair_index in pairing_indexes:
@@ -984,15 +980,15 @@
 
 def save_dataframe(dataframe, file_name, overwrite=True):
     """
     Save dataframe (csv, laz, attr file)
     """
     # Save attributes
     attributes_file_name = file_name + "_attrs.json"
-    save_dict(dataframe.attrs, attributes_file_name)
+    save_dict(dataframe.attrs, attributes_file_name, safe_save=True)
 
     # Save point cloud to laz format
     if (
         "attributes" in dataframe.attrs
         and "save_points_cloud_as_laz" in dataframe.attrs["attributes"]
     ):
         if dataframe.attrs["attributes"]["save_points_cloud_as_laz"]:
```

### Comparing `cars-0.7.5/cars/data_structures/cars_dict.py` & `cars-0.7.6/cars/data_structures/cars_dict.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/data_structures/corresponding_tiles_tools.py` & `cars-0.7.6/cars/data_structures/corresponding_tiles_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/data_structures/dataframe_converter.py` & `cars-0.7.6/cars/data_structures/dataframe_converter.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/data_structures/format_transformation.py` & `cars-0.7.6/cars/data_structures/format_transformation.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/extractroi.py` & `cars-0.7.6/cars/extractroi.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/__init__.py` & `cars-0.7.6/cars/orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/achievement_tracker.py` & `cars-0.7.6/cars/orchestrator/achievement_tracker.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,14 +64,27 @@
         """
         Add finished tile
 
         :param tile: finished tile
         :type tile: xarray Dataset or Pandas Dataframe
         """
 
+        try:
+            self._add_tile(tile)
+        except RuntimeError:
+            logging.error("Error getting id in Achiement Tracker")
+
+    def _add_tile(self, tile):
+        """
+        Add finished tile
+
+        :param tile: finished tile
+        :type tile: xarray Dataset or Pandas Dataframe
+        """
+
         # Get cars dataset id
         cars_ds_id = AbstractCarsDatasetRegistry.get_future_cars_dataset_id(
             tile
         )
         if cars_ds_id is None:
             raise RuntimeError("No id in data")
         if cars_ds_id not in self.cars_ds_ids:
```

### Comparing `cars-0.7.5/cars/orchestrator/cluster/__init__.py` & `cars-0.7.6/cars/orchestrator/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/abstract_cluster.py` & `cars-0.7.6/cars/orchestrator/cluster/abstract_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/abstract_dask_cluster.py` & `cars-0.7.6/cars/orchestrator/cluster/abstract_dask_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_cluster_tools.py` & `cars-0.7.6/cars/orchestrator/cluster/dask_cluster_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_config/README.md` & `cars-0.7.6/cars/orchestrator/cluster/dask_config/README.md`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_config/dask.yaml` & `cars-0.7.6/cars/orchestrator/cluster/dask_config/dask.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_config/distributed.yaml` & `cars-0.7.6/cars/orchestrator/cluster/dask_config/distributed.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_config/jobqueue.yaml` & `cars-0.7.6/cars/orchestrator/cluster/dask_config/jobqueue.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/dask-schema.yaml` & `cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/dask-schema.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/dask.yaml` & `cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/dask.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/distributed-schema.yaml` & `cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/distributed-schema.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/distributed.yaml` & `cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/distributed.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_config/reference_confs/jobqueue.yaml` & `cars-0.7.6/cars/orchestrator/cluster/dask_config/reference_confs/jobqueue.yaml`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/dask_jobqueue_utils.py` & `cars-0.7.6/cars/orchestrator/cluster/dask_jobqueue_utils.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/local_dask_cluster.py` & `cars-0.7.6/cars/orchestrator/cluster/local_dask_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/log_wrapper.py` & `cars-0.7.6/cars/orchestrator/cluster/log_wrapper.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/mp_cluster/__init__.py` & `cars-0.7.6/cars/orchestrator/registry/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,13 +15,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-CARS multiprocessing cluster module init file
+Cars registry module init file
 """
-# flake8: noqa: F401
-
-
-from . import multiprocessing_cluster
```

### Comparing `cars-0.7.5/cars/orchestrator/cluster/mp_cluster/mp_factorizer.py` & `cars-0.7.6/cars/orchestrator/cluster/mp_cluster/mp_factorizer.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/mp_cluster/mp_objects.py` & `cars-0.7.6/cars/orchestrator/cluster/mp_cluster/mp_objects.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/mp_cluster/mp_tools.py` & `cars-0.7.6/cars/orchestrator/cluster/mp_cluster/mp_tools.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/mp_cluster/mp_wrapper.py` & `cars-0.7.6/cars/orchestrator/cluster/mp_cluster/mp_wrapper.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/mp_cluster/multiprocessing_cluster.py` & `cars-0.7.6/cars/orchestrator/cluster/mp_cluster/multiprocessing_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/pbs_dask_cluster.py` & `cars-0.7.6/cars/orchestrator/cluster/pbs_dask_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/sequential_cluster.py` & `cars-0.7.6/cars/orchestrator/cluster/sequential_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/cluster/slurm_dask_cluster.py` & `cars-0.7.6/cars/orchestrator/cluster/slurm_dask_cluster.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/orchestrator.py` & `cars-0.7.6/cars/orchestrator/orchestrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from cars.orchestrator import achievement_tracker
 from cars.orchestrator.cluster.abstract_cluster import AbstractCluster
 from cars.orchestrator.orchestrator_constants import (
     CARS_DATASET_KEY,
     CARS_DS_COL,
     CARS_DS_ROW,
 )
+from cars.orchestrator.registry import compute_registry
 from cars.orchestrator.registry import id_generator as id_gen
 from cars.orchestrator.registry import replacer_registry, saver_registry
 from cars.orchestrator.tiles_profiler import TileProfiler
 
 
 class Orchestrator:
     """
@@ -109,14 +110,19 @@
         self.cars_ds_savers_registry = saver_registry.CarsDatasetsRegistrySaver(
             self.id_generator
         )
         # init CarsDataset replacement registry
         self.cars_ds_replacer_registry = (
             replacer_registry.CarsDatasetRegistryReplacer(self.id_generator)
         )
+        # init CarsDataset compute registry
+        self.cars_ds_compute_registry = (
+            compute_registry.CarsDatasetRegistryCompute(self.id_generator)
+        )
+
         # Achievement tracker
         self.achievement_tracker = achievement_tracker.AchievementTracker()
 
         # init tile profiler
         self.dir_tile_profiling = os.path.join(self.out_dir, "tile_processing")
         if not os.path.exists(self.dir_tile_profiling):
             os.makedirs(self.dir_tile_profiling)
@@ -208,14 +214,36 @@
             self.cars_ds_names_info.append(cars_ds_name)
 
         # add to tracking
         self.achievement_tracker.track(
             cars_ds, self.get_saving_infos([cars_ds])[0][CARS_DATASET_KEY]
         )
 
+    def add_to_compute_lists(self, cars_ds, cars_ds_name=None):
+        """
+        Add CarsDataset to compute Registry: computed, but not used
+        in main process
+
+        :param cars_ds: CarsDataset to comput
+        :type cars_ds: CarsDataset
+        :param cars_ds_name: name corresponding to CarsDataset,
+            for information during logging
+        """
+
+        self.cars_ds_compute_registry.add_cars_ds_to_compute(cars_ds)
+
+        # add name if exists
+        if cars_ds_name is not None:
+            self.cars_ds_names_info.append(cars_ds_name)
+
+        # add to tracking
+        self.achievement_tracker.track(
+            cars_ds, self.get_saving_infos([cars_ds])[0][CARS_DATASET_KEY]
+        )
+
     def save_out_json(self):
         """
         Check out_json and save it to file
         """
 
         # TODO check schema ?
 
@@ -332,15 +360,16 @@
 
             # run compute and save files
             logging.info("Compute delayed ...")
             # Flatten to list
             if only_remaining_delayed is None:
                 delayed_objects = flatten_object(
                     self.cars_ds_savers_registry.get_cars_datasets_list()
-                    + self.cars_ds_replacer_registry.get_cars_datasets_list(),
+                    + self.cars_ds_replacer_registry.get_cars_datasets_list()
+                    + self.cars_ds_compute_registry.get_cars_datasets_list(),
                     self.cluster.get_delayed_type(),
                 )
             else:
                 delayed_objects = only_remaining_delayed
 
             # Compute delayed
             future_objects = self.cluster.start_tasks(delayed_objects)
@@ -456,14 +485,18 @@
             self.id_generator
         )
 
         #  CarsDataset replacement registry
         self.cars_ds_replacer_registry = (
             replacer_registry.CarsDatasetRegistryReplacer(self.id_generator)
         )
+        # Compute registry
+        self.cars_ds_compute_registry = (
+            compute_registry.CarsDatasetRegistryCompute(self.id_generator)
+        )
 
         # tile profiler
         self.tile_profiler = TileProfiler(
             self.dir_tile_profiling,
             self.cars_ds_savers_registry,
             self.cars_ds_replacer_registry,
         )
```

### Comparing `cars-0.7.5/cars/orchestrator/orchestrator_constants.py` & `cars-0.7.6/cars/orchestrator/orchestrator_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/registry/__init__.py` & `cars-0.7.6/cars/pipelines/point_clouds_to_dsm/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,9 +15,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-Cars registry module init file
+CARS sensor_to_dense_dsm pipeline module init file
 """
+
+# Cars imports
+from cars.pipelines.point_clouds_to_dsm import (  # noqa: F401
+    point_cloud_to_dsm_pipeline,
+)
```

### Comparing `cars-0.7.5/cars/orchestrator/registry/abstract_registry.py` & `cars-0.7.6/cars/orchestrator/registry/abstract_registry.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/registry/id_generator.py` & `cars-0.7.6/cars/orchestrator/registry/id_generator.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/registry/replacer_registry.py` & `cars-0.7.6/cars/orchestrator/registry/replacer_registry.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/registry/saver_registry.py` & `cars-0.7.6/cars/orchestrator/registry/saver_registry.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/registry/unseen_registry.py` & `cars-0.7.6/cars/orchestrator/registry/unseen_registry.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/orchestrator/tiles_profiler.py` & `cars-0.7.6/cars/orchestrator/tiles_profiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,24 +57,36 @@
         self.arrays = []
 
     def add_tile(self, tile_object):
         """
         Add tile to profiling
         """
 
+        try:
+            self._add_tile(tile_object)
+        except Exception:
+            logging.debug("Error in TileProfiler.add_tile ")
+
+    def _add_tile(self, tile_object):
+        """
+        Add tile to profiling
+        """
+
         # Get Cars Dastaset id
         cars_ds_id = self.saver_registry.get_future_cars_dataset_id(tile_object)
 
         if cars_ds_id not in self.cars_ds_ids:
             self.cars_ds_ids.append(cars_ds_id)
 
             # Get cars_ds
             cars_ds = self.saver_registry.get_cars_ds(tile_object)
             if cars_ds is None:
                 cars_ds = self.replacer_registry.get_cars_ds(tile_object)
+            if cars_ds is None:
+                raise RuntimeError("CARS Dataset is None")
             self.monitored_cars_ds.append(cars_ds)
 
             # Create array
             new_arr = np.zeros((*cars_ds.shape, 3), dtype=int)
             # Update None tiles
             for tile_row in range(cars_ds.shape[0]):
                 for tile_col in range(cars_ds.shape[1]):
```

### Comparing `cars-0.7.5/cars/pipelines/__init__.py` & `cars-0.7.6/cars/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/pipelines/conf_pipeline/__init__.py` & `cars-0.7.6/cars/pipelines/conf_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/pipelines/pipeline.py` & `cars-0.7.6/cars/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/pipelines/pipeline_constants.py` & `cars-0.7.6/cars/pipelines/pipeline_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/pipelines/pipeline_template.py` & `cars-0.7.6/cars/pipelines/pipeline_template.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/pipelines/point_clouds_to_dsm/__init__.py` & `cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 # limitations under the License.
 #
 """
 CARS sensor_to_dense_dsm pipeline module init file
 """
 
 # Cars imports
-from cars.pipelines.point_clouds_to_dsm import (  # noqa: F401
-    point_cloud_to_dsm_pipeline,
+from cars.pipelines.sensor_to_dense_dsm import (  # noqa: F401
+    sensor_to_dense_dsm_pipeline,
 )
```

### Comparing `cars-0.7.5/cars/pipelines/point_clouds_to_dsm/pc_constants.py` & `cars-0.7.6/cars/pipelines/point_clouds_to_dsm/pc_constants.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/pipelines/point_clouds_to_dsm/pc_inputs.py` & `cars-0.7.6/cars/pipelines/point_clouds_to_dsm/pc_inputs.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/pipelines/point_clouds_to_dsm/point_cloud_to_dsm_pipeline.py` & `cars-0.7.6/cars/pipelines/point_clouds_to_dsm/point_cloud_to_dsm_pipeline.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/__init__.py` & `cars-0.7.6/cars/pipelines/sensor_to_sparse_dsm/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 # limitations under the License.
 #
 """
 CARS sensor_to_dense_dsm pipeline module init file
 """
 
 # Cars imports
-from cars.pipelines.sensor_to_dense_dsm import (  # noqa: F401
-    sensor_to_dense_dsm_pipeline,
+from cars.pipelines.sensor_to_sparse_dsm import (  # noqa: F401
+    sensor_to_sparse_dsm_pipeline,
 )
```

### Comparing `cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/dsm_output.py` & `cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/dsm_output.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/sensor_dense_dsm_constants.py` & `cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/sensor_dense_dsm_constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # Sensor input
 
 SENSORS = "sensors"
 PAIRING = "pairing"
 
 EPSG = "epsg"
 INITIAL_ELEVATION = "initial_elevation"
+USE_ENDOGENOUS_ELEVATION = "use_endogenous_elevation"
 
 CHECK_INPUTS = "check_inputs"
 DEFAULT_ALT = "default_alt"
 ROI = "roi"
 GEOID = "geoid"
 DEBUG_WITH_ROI = "debug_with_roi"
```

### Comparing `cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/sensor_to_dense_dsm_pipeline.py` & `cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/sensor_to_dense_dsm_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+# pylint: disable=too-many-lines
 """
 CARS sensors_to_dense_dsm pipeline class file
 """
-# pylint: disable=too-many-lines
 # Standard imports
 from __future__ import print_function
 
 import json
 import logging
 import os
 
@@ -39,14 +39,15 @@
     dem_generation_constants as dem_gen_cst,
 )
 from cars.applications.dem_generation import dem_generation_tools
 from cars.applications.grid_generation import grid_correction
 from cars.applications.sparse_matching import (
     sparse_matching_tools as sparse_mtch_tools,
 )
+from cars.core import constants_disparity as cst_disp
 from cars.core import preprocessing, roi_tools
 from cars.core.geometry.abstract_geometry import AbstractGeometry
 from cars.core.inputs import get_descriptions_bands
 from cars.core.utils import safe_makedirs
 from cars.data_structures import cars_dataset
 from cars.orchestrator import orchestrator
 from cars.orchestrator.cluster.log_wrapper import cars_profile
@@ -138,14 +139,15 @@
 
         # Check geometry plugin and overwrite geomodel in conf inputs
         (
             self.inputs,
             self.used_conf[GEOMETRY_PLUGIN],
             self.geom_plugin_without_dem_and_geoid,
             self.geom_plugin_with_dem_and_geoid,
+            self.dem_generation_roi,
         ) = sensors_inputs.check_geometry_plugin(
             self.inputs, self.conf.get(GEOMETRY_PLUGIN, None)
         )
         self.used_conf[INPUTS] = self.inputs
 
         # Get ROI
         (
@@ -230,14 +232,15 @@
             "resampling",
             "holes_detection",
             "dense_matches_filling.1",
             "dense_matches_filling.2",
             "sparse_matching",
             "dense_matching",
             "triangulation",
+            "pc_denoising",
             "dem_generation",
         ]
 
         terrain_applications = [
             "point_cloud_rasterization",
         ]
 
@@ -326,14 +329,18 @@
 
         # Triangulation
         self.triangulation_application = Application(
             "triangulation", cfg=conf.get("triangulation", {})
         )
         used_conf["triangulation"] = self.triangulation_application.get_conf()
 
+        self.pc_denoising_application = Application(
+            "pc_denoising", cfg=conf.get("pc_denoising", {"method": "none"})
+        )
+
         # MNT generation
         self.dem_generation_application = Application(
             "dem_generation", cfg=conf.get("dem_generation", {})
         )
         used_conf["dem_generation"] = self.dem_generation_application.get_conf()
 
         if generate_terrain_products:
@@ -778,25 +785,35 @@
             else:
                 # Use initial elevation if provided, and generate dems
                 # Generate MNT from matches
                 dem = self.dem_generation_application.run(
                     triangulated_matches_list,
                     cars_orchestrator.out_dir,
                     self.inputs[sens_cst.GEOID],
+                    dem_roi_to_use=self.dem_generation_roi,
                 )
+                # Same geometry plugin if we use exogenous dem
+                # as initial elevation always used before if provided
                 dem_median = dem.attributes[dem_gen_cst.DEM_MEDIAN_PATH]
-                # Generate geometry loader with dem and geoid
-                self.geom_plugin_with_dem_and_geoid = (
-                    sensors_inputs.generate_geometry_plugin_with_dem(
-                        self.used_conf[GEOMETRY_PLUGIN],
-                        self.inputs,
-                        dem=dem_median,
-                        crop_dem=False,
+                if (
+                    self.inputs[sens_cst.INITIAL_ELEVATION] is not None
+                    and not self.inputs[sens_cst.USE_ENDOGENOUS_ELEVATION]
+                ):
+                    dem_median = self.inputs[sens_cst.INITIAL_ELEVATION]
+
+                if dem_median != self.inputs[sens_cst.INITIAL_ELEVATION]:
+                    self.geom_plugin_with_dem_and_geoid = (
+                        sensors_inputs.generate_geometry_plugin_with_dem(
+                            self.used_conf[GEOMETRY_PLUGIN],
+                            self.inputs,
+                            dem=dem_median,
+                            crop_dem=False,
+                        )
                     )
-                )
+
                 dem_min = dem.attributes[dem_gen_cst.DEM_MIN_PATH]
                 dem_max = dem.attributes[dem_gen_cst.DEM_MAX_PATH]
 
             # update used configuration with terrain a priori
             sensors_inputs.update_conf(
                 self.used_conf,
                 dem_median=dem_median,
@@ -805,21 +822,32 @@
             )
 
             # Define param
             use_global_disp_range = (
                 self.dense_matching_app.use_global_disp_range
             )
 
+            if self.pc_denoising_application is not None:
+                denoising_overload_fun = (
+                    self.pc_denoising_application.get_triangulation_overload()
+                )
+            else:
+                denoising_overload_fun = None
+
             pairs_names = [pair_name for pair_name, _, _ in list_sensor_pairs]
 
             for cloud_id, (pair_key, _, _) in enumerate(list_sensor_pairs):
                 # Geometry plugin with dem will be used for the grid generation
                 geom_plugin = self.geom_plugin_with_dem_and_geoid
                 if self.used_conf[INPUTS]["use_epipolar_a_priori"] is False:
-                    if self.inputs[sens_cst.INITIAL_ELEVATION] is None:
+
+                    if not (
+                        self.inputs[sens_cst.INITIAL_ELEVATION] is not None
+                        and not self.inputs[sens_cst.USE_ENDOGENOUS_ELEVATION]
+                    ):
                         # Generate grids with new MNT
                         (
                             pairs[pair_key]["new_grid_left"],
                             pairs[pair_key]["new_grid_right"],
                         ) = self.epipolar_grid_generation_application.run(
                             pairs[pair_key]["sensor_image_left"],
                             pairs[pair_key]["sensor_image_right"],
@@ -870,44 +898,44 @@
                             )
                         )
 
                         pairs[pair_key]["corrected_grid_left"] = pairs[
                             pair_key
                         ]["new_grid_left"]
 
-                        # matches filter params
-                        matches_filter_knn = (
-                            self.sparse_mtch_app.get_matches_filter_knn()
-                        )
-                        matches_filter_dev_factor = (
-                            self.sparse_mtch_app.get_matches_filter_dev_factor()
-                        )
-                        if use_global_disp_range:
-                            # Triangulate new matches
-                            pairs[pair_key]["triangulated_matches"] = (
-                                dem_generation_tools.triangulate_sparse_matches(
-                                    pairs[pair_key]["sensor_image_left"],
-                                    pairs[pair_key]["sensor_image_right"],
-                                    pairs[pair_key]["corrected_grid_left"],
-                                    pairs[pair_key]["corrected_grid_right"],
-                                    pairs[pair_key]["corrected_matches_array"],
-                                    geometry_plugin=geom_plugin,
-                                )
+                    # matches filter params
+                    matches_filter_knn = (
+                        self.sparse_mtch_app.get_matches_filter_knn()
+                    )
+                    matches_filter_dev_factor = (
+                        self.sparse_mtch_app.get_matches_filter_dev_factor()
+                    )
+                    if use_global_disp_range:
+                        # Triangulate new matches
+                        pairs[pair_key]["triangulated_matches"] = (
+                            dem_generation_tools.triangulate_sparse_matches(
+                                pairs[pair_key]["sensor_image_left"],
+                                pairs[pair_key]["sensor_image_right"],
+                                pairs[pair_key]["corrected_grid_left"],
+                                pairs[pair_key]["corrected_grid_right"],
+                                pairs[pair_key]["corrected_matches_array"],
+                                geometry_plugin=geom_plugin,
                             )
-                            # filter triangulated_matches
-                            # Filter outliers
-                            pairs[pair_key]["filtered_triangulated_matches"] = (
-                                sparse_mtch_tools.filter_point_cloud_matches(
-                                    pairs[pair_key]["triangulated_matches"],
-                                    matches_filter_knn=matches_filter_knn,
-                                    matches_filter_dev_factor=(
-                                        matches_filter_dev_factor
-                                    ),
-                                )
+                        )
+                        # filter triangulated_matches
+                        # Filter outliers
+                        pairs[pair_key]["filtered_triangulated_matches"] = (
+                            sparse_mtch_tools.filter_point_cloud_matches(
+                                pairs[pair_key]["triangulated_matches"],
+                                matches_filter_knn=matches_filter_knn,
+                                matches_filter_dev_factor=(
+                                    matches_filter_dev_factor
+                                ),
                             )
+                        )
 
                     if use_global_disp_range:
                         # Compute disp_min and disp_max
                         (
                             dmin,
                             dmax,
                         ) = sparse_mtch_tools.compute_disp_min_disp_max(
@@ -1027,14 +1055,15 @@
                 )
 
                 # if sequential mode, apply roi
                 epipolar_roi = None
                 if (
                     cars_orchestrator.cluster.checked_conf_cluster["mode"]
                     == "sequential"
+                    or "no_merging" in self.used_conf[PIPELINE]
                 ):
                     # Generate roi
                     epipolar_roi = preprocessing.compute_epipolar_roi(
                         self.input_roi_poly,
                         self.input_roi_epsg,
                         self.geom_plugin_with_dem_and_geoid,
                         pairs[pair_key]["sensor_image_left"],
@@ -1173,33 +1202,64 @@
                         ),
                     )
                     # Compute roi polygon, in input EPSG
                     roi_poly = preprocessing.compute_roi_poly(
                         self.input_roi_poly, self.input_roi_epsg, epsg
                     )
 
+                # Checking disparity intervals indicators
+                if self.application_conf["dense_matching"][
+                    "generate_confidence_intervals"
+                ]:
+                    intervals = [cst_disp.INTERVAL_INF, cst_disp.INTERVAL_SUP]
+                    for key, item in self.dense_matching_app.corr_config[
+                        "pipeline"
+                    ].items():
+                        if cst_disp.CONFIDENCE_KEY in key:
+                            if item["confidence_method"] == cst_disp.INTERVAL:
+                                indicator = key.split(".")
+                                if len(indicator) > 1:
+                                    intervals[0] += "." + indicator[-1]
+                                    intervals[1] += "." + indicator[-1]
+                                # Only processing the first encountered interval
+                                break
+                else:
+                    intervals = None
+
                 # Run epipolar triangulation application
                 epipolar_points_cloud = self.triangulation_application.run(
                     pairs[pair_key]["sensor_image_left"],
                     pairs[pair_key]["sensor_image_right"],
                     new_epipolar_image_left,
                     pairs[pair_key]["corrected_grid_left"],
                     pairs[pair_key]["corrected_grid_right"],
                     filled_with_2_epipolar_disparity_map,
                     epsg,
                     self.geom_plugin_without_dem_and_geoid,
+                    denoising_overload_fun=denoising_overload_fun,
                     source_pc_names=pairs_names,
                     orchestrator=cars_orchestrator,
                     pair_folder=pairs[pair_key]["pair_folder"],
                     pair_key=pair_key,
                     uncorrected_grid_right=pairs[pair_key]["grid_right"],
                     geoid_path=self.inputs[sens_cst.GEOID],
                     cloud_id=cloud_id,
+                    intervals=intervals,
                 )
 
+                if "no_merging" in self.used_conf[PIPELINE]:
+                    denoised_epipolar_points_cloud = (
+                        self.pc_denoising_application.run(
+                            epipolar_points_cloud,
+                            orchestrator=cars_orchestrator,
+                            pair_folder=pairs[pair_key]["pair_folder"],
+                            pair_key=pair_key,
+                        )
+                    )
+
                 if self.generate_terrain_products:
                     # Compute terrain bounding box /roi related to
                     # current images
                     (current_terrain_roi_bbox) = (
                         preprocessing.compute_terrain_bbox(
                             pairs[pair_key]["sensor_image_left"],
                             pairs[pair_key]["sensor_image_right"],
@@ -1225,15 +1285,20 @@
                             pair_folder=pairs[pair_key]["pair_folder"],
                             check_inputs=self.inputs[sens_cst.CHECK_INPUTS],
                         )
                     )
                     list_terrain_roi.append(current_terrain_roi_bbox)
 
                 # add points cloud to list
-                list_epipolar_points_cloud.append(epipolar_points_cloud)
+                if "no_merging" in self.used_conf[PIPELINE]:
+                    list_epipolar_points_cloud.append(
+                        denoised_epipolar_points_cloud
+                    )
+                else:
+                    list_epipolar_points_cloud.append(epipolar_points_cloud)
 
             if self.generate_terrain_products:
                 # compute terrain bounds
                 (
                     terrain_bounds,
                     optimal_terrain_tile_width,
                 ) = preprocessing.compute_terrain_bounds(
@@ -1290,16 +1355,24 @@
                     filtered_2_merged_points_clouds = (
                         self.pc_outliers_removing_2_app.run(
                             filtered_1_merged_points_clouds,
                             orchestrator=cars_orchestrator,
                         )
                     )
 
+                    # denoise point cloud
+                    denoised_merged_points_clouds = (
+                        self.pc_denoising_application.run(
+                            filtered_2_merged_points_clouds,
+                            orchestrator=cars_orchestrator,
+                        )
+                    )
+
                     # Rasterize merged and filtered point cloud
-                    point_cloud_to_rasterize = filtered_2_merged_points_clouds
+                    point_cloud_to_rasterize = denoised_merged_points_clouds
 
                 # rasterize point cloud
                 _ = self.rasterization_application.run(
                     point_cloud_to_rasterize,
                     epsg,
                     orchestrator=cars_orchestrator,
                     dsm_file_name=os.path.join(
```

### Comparing `cars-0.7.5/cars/pipelines/sensor_to_dense_dsm/sensors_inputs.py` & `cars-0.7.6/cars/pipelines/sensor_to_dense_dsm/sensors_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import os
 
 import numpy as np
 import rasterio as rio
 from json_checker import Checker, Or
 
 # CARS imports
-from cars.core import inputs
+from cars.core import inputs, preprocessing, roi_tools
 from cars.core.geometry.abstract_geometry import AbstractGeometry
 from cars.core.utils import make_relative_path_absolute
 from cars.pipelines.pipeline_constants import INPUTS
 from cars.pipelines.sensor_to_dense_dsm import (
     sensor_dense_dsm_constants as sens_cst,
 )
 
@@ -58,14 +58,17 @@
     overloaded_conf = conf.copy()
 
     # Overload some optional parameters
     overloaded_conf[sens_cst.EPSG] = conf.get(sens_cst.EPSG, None)
     overloaded_conf[sens_cst.INITIAL_ELEVATION] = conf.get(
         sens_cst.INITIAL_ELEVATION, None
     )
+    overloaded_conf[sens_cst.USE_ENDOGENOUS_ELEVATION] = conf.get(
+        sens_cst.USE_ENDOGENOUS_ELEVATION, False
+    )
     overloaded_conf[sens_cst.DEFAULT_ALT] = conf.get(sens_cst.DEFAULT_ALT, 0)
     overloaded_conf[sens_cst.ROI] = conf.get(sens_cst.ROI, None)
     overloaded_conf[sens_cst.DEBUG_WITH_ROI] = conf.get(
         sens_cst.DEBUG_WITH_ROI, False
     )
     overloaded_conf[sens_cst.CHECK_INPUTS] = conf.get(
         sens_cst.CHECK_INPUTS, False
@@ -95,14 +98,15 @@
 
     # Validate inputs
     inputs_schema = {
         sens_cst.SENSORS: dict,
         sens_cst.PAIRING: [[str]],
         sens_cst.EPSG: Or(int, None),  # move to rasterization
         sens_cst.INITIAL_ELEVATION: Or(str, None),
+        sens_cst.USE_ENDOGENOUS_ELEVATION: bool,
         sens_cst.DEFAULT_ALT: int,
         sens_cst.ROI: Or(str, dict, None),
         sens_cst.DEBUG_WITH_ROI: bool,
         sens_cst.CHECK_INPUTS: bool,
         sens_cst.GEOID: Or(None, str),
     }
     if check_epipolar_a_priori:
@@ -154,14 +158,22 @@
         sens_cst.INPUT_MSK: Or(str, None),
         sens_cst.INPUT_CLASSIFICATION: Or(str, None),
     }
     checker_sensor = Checker(sensor_schema)
 
     for sensor_image_key in conf[sens_cst.SENSORS]:
         # Overload optional parameters
+        geomodel = conf[sens_cst.SENSORS][sensor_image_key].get(
+            "geomodel",
+            conf[sens_cst.SENSORS][sensor_image_key][sens_cst.INPUT_IMG],
+        )
+        overloaded_conf[sens_cst.SENSORS][sensor_image_key][
+            "geomodel"
+        ] = geomodel
+
         color = conf[sens_cst.SENSORS][sensor_image_key].get(
             "color",
             conf[sens_cst.SENSORS][sensor_image_key][sens_cst.INPUT_IMG],
         )
         overloaded_conf[sens_cst.SENSORS][sensor_image_key][
             sens_cst.INPUT_COLOR
         ] = color
@@ -348,19 +360,61 @@
             sens_cst.INPUT_GEO_MODEL
         ] = geomodel
 
     geom_plugin_with_dem_and_geoid = generate_geometry_plugin_with_dem(
         conf_geom_plugin, conf_inputs
     )
 
+    # Check dem is big enough
+    dem_generation_roi_poly = None
+    needed_dem_roi = geom_plugin_with_dem_and_geoid.dem_roi
+    needed_dem_roi_epsg = geom_plugin_with_dem_and_geoid.dem_roi_epsg
+    if needed_dem_roi is not None:
+        needed_dem_roi_poly = roi_tools.bounds_to_poly(needed_dem_roi)
+        # convert to 4326 roi
+        dem_generation_roi_poly = preprocessing.compute_roi_poly(
+            needed_dem_roi_poly, needed_dem_roi_epsg, 4326
+        )
+
+        if conf_inputs[sens_cst.INITIAL_ELEVATION] is not None:
+            # get dem total roi
+            total_input_roi_poly = roi_tools.bounds_to_poly(
+                inputs.rasterio_get_bounds(
+                    conf_inputs[sens_cst.INITIAL_ELEVATION]
+                )
+            )
+            total_input_roi_epsg = inputs.rasterio_get_epsg_code(
+                conf_inputs[sens_cst.INITIAL_ELEVATION]
+            )
+            total_input_roi_poly = preprocessing.compute_roi_poly(
+                total_input_roi_poly, total_input_roi_epsg, 4326
+            )
+
+            # if needed roi not inside dem, raise error
+            if not total_input_roi_poly.contains_properly(
+                dem_generation_roi_poly
+            ):
+                raise RuntimeError(
+                    "Given initial elevation ROI is not covering needed ROI: "
+                    " EPSG:4326, ROI: {}".format(dem_generation_roi_poly.bounds)
+                )
+
+    else:
+        logging.warning(
+            "Current geometry plugin doesnt compute dem roi needed "
+            "for later computations. Errors related to unsufficient "
+            "dem roi might occur."
+        )
+
     return (
         overloaded_conf_inputs,
         conf_geom_plugin,
         geom_plugin_without_dem_and_geoid,
         geom_plugin_with_dem_and_geoid,
+        dem_generation_roi_poly,
     )
 
 
 def generate_geometry_plugin_with_dem(
     conf_geom_plugin, conf_inputs, dem=None, crop_dem=True
 ):
     """
```

### Comparing `cars-0.7.5/cars/pipelines/sensor_to_sparse_dsm/__init__.py` & `cars-0.7.6/cars/applications/point_cloud_denoising/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+# !/usr/bin/env python
 # coding: utf8
 #
 # Copyright (c) 2020 Centre National d'Etudes Spatiales (CNES).
 #
 # This file is part of CARS
 # (see https://github.com/CNES/cars).
 #
@@ -15,14 +15,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
-CARS sensor_to_dense_dsm pipeline module init file
+CARS holes detection module init file
 """
+# flake8: noqa: F401
 
-# Cars imports
-from cars.pipelines.sensor_to_sparse_dsm import (  # noqa: F401
-    sensor_to_sparse_dsm_pipeline,
+import cars.applications.point_cloud_denoising.point_cloud_denoising
+from cars.applications.point_cloud_denoising.point_cloud_denoising import (
+    PCDenoising,
 )
```

### Comparing `cars-0.7.5/cars/pipelines/sensor_to_sparse_dsm/sensor_to_sparse_dsm_pipeline.py` & `cars-0.7.6/cars/pipelines/sensor_to_sparse_dsm/sensor_to_sparse_dsm_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
         # Check geometry plugin
         (
             self.inputs,
             self.used_conf[GEOMETRY_PLUGIN],
             self.geom_plugin_without_dem_and_geoid,
             self.geom_plugin_with_dem_and_geoid,
+            self.dem_generation_roi,
         ) = sensors_inputs.check_geometry_plugin(
             self.inputs, self.conf.get(GEOMETRY_PLUGIN, None)
         )
         self.used_conf[INPUTS] = self.inputs
 
         # Get ROI
         (
@@ -489,14 +490,15 @@
                 )
 
             # Generate MNT from matches
             dem = self.dem_generation_application.run(
                 triangulated_matches_list,
                 cars_orchestrator.out_dir,
                 self.inputs[sens_cst.GEOID],
+                dem_roi_to_use=self.dem_generation_roi,
             )
             dem_median = dem.attributes[dem_gen_cst.DEM_MEDIAN_PATH]
             # Generate geometry loader with dem and geoid
             self.geom_plugin_with_dem_and_geoid = (
                 sensors_inputs.generate_geometry_plugin_with_dem(
                     self.used_conf[GEOMETRY_PLUGIN],
                     self.inputs,
@@ -520,101 +522,96 @@
                 dem_median=dem_median,
                 dem_min=dem_min,
                 dem_max=dem_max,
             )
 
             for pair_key, _, _ in list_sensor_pairs:
                 geom_plugin = self.geom_plugin_with_dem_and_geoid
-                if self.inputs[sens_cst.INITIAL_ELEVATION] is None:
-                    # Generate grids with new MNT
-                    (
+                # Generate grids with new MNT
+                (
+                    pairs[pair_key]["new_grid_left"],
+                    pairs[pair_key]["new_grid_right"],
+                ) = self.epipolar_grid_generation_app.run(
+                    pairs[pair_key]["sensor_image_left"],
+                    pairs[pair_key]["sensor_image_right"],
+                    geom_plugin,
+                    orchestrator=cars_orchestrator,
+                    pair_folder=pairs[pair_key]["pair_folder"],
+                    pair_key=pair_key,
+                )
+
+                # Correct grids with former matches
+                # Transform matches to new grids
+
+                new_grid_matches_array = (
+                    AbstractGeometry.transform_matches_from_grids(
+                        pairs[pair_key]["corrected_matches_array"],
+                        pairs[pair_key]["corrected_grid_left"],
+                        pairs[pair_key]["corrected_grid_right"],
                         pairs[pair_key]["new_grid_left"],
                         pairs[pair_key]["new_grid_right"],
-                    ) = self.epipolar_grid_generation_app.run(
-                        pairs[pair_key]["sensor_image_left"],
-                        pairs[pair_key]["sensor_image_right"],
-                        geom_plugin,
-                        orchestrator=cars_orchestrator,
-                        pair_folder=pairs[pair_key]["pair_folder"],
-                        pair_key=pair_key,
                     )
+                )
 
-                    # Correct grids with former matches
-                    # Transform matches to new grids
-
-                    new_grid_matches_array = (
-                        AbstractGeometry.transform_matches_from_grids(
-                            pairs[pair_key]["corrected_matches_array"],
-                            pairs[pair_key]["corrected_grid_left"],
-                            pairs[pair_key]["corrected_grid_right"],
-                            pairs[pair_key]["new_grid_left"],
-                            pairs[pair_key]["new_grid_right"],
-                        )
-                    )
+                # Estimate grid_correction
+                (
+                    pairs[pair_key]["grid_correction_coef"],
+                    corrected_matches_array,
+                    pairs[pair_key]["corrected_matches_cars_ds"],
+                    _,
+                    _,
+                ) = grid_correction.estimate_right_grid_correction(
+                    new_grid_matches_array,
+                    pairs[pair_key]["new_grid_right"],
+                    initial_cars_ds=pairs[pair_key]["epipolar_matches_left"],
+                    save_matches=(self.sparse_matching_app.get_save_matches()),
+                    pair_folder=pairs[pair_key]["pair_folder"],
+                    pair_key=pair_key,
+                    orchestrator=cars_orchestrator,
+                )
 
-                    # Estimate grid_correction
-                    (
-                        pairs[pair_key]["grid_correction_coef"],
-                        corrected_matches_array,
-                        pairs[pair_key]["corrected_matches_cars_ds"],
-                        _,
-                        _,
-                    ) = grid_correction.estimate_right_grid_correction(
-                        new_grid_matches_array,
+                # Correct grid right
+                pairs[pair_key]["corrected_grid_right"] = (
+                    grid_correction.correct_grid(
                         pairs[pair_key]["new_grid_right"],
-                        initial_cars_ds=pairs[pair_key][
-                            "epipolar_matches_left"
-                        ],
-                        save_matches=(
-                            self.sparse_matching_app.get_save_matches()
-                        ),
-                        pair_folder=pairs[pair_key]["pair_folder"],
-                        pair_key=pair_key,
-                        orchestrator=cars_orchestrator,
-                    )
-
-                    # Correct grid right
-                    pairs[pair_key]["corrected_grid_right"] = (
-                        grid_correction.correct_grid(
-                            pairs[pair_key]["new_grid_right"],
-                            pairs[pair_key]["grid_correction_coef"],
-                            self.epipolar_grid_generation_app.save_grids,
-                            pairs[pair_key]["pair_folder"],
-                        )
+                        pairs[pair_key]["grid_correction_coef"],
+                        self.epipolar_grid_generation_app.save_grids,
+                        pairs[pair_key]["pair_folder"],
                     )
-                    pairs[pair_key]["corrected_grid_left"] = pairs[pair_key][
-                        "new_grid_left"
-                    ]
+                )
+                pairs[pair_key]["corrected_grid_left"] = pairs[pair_key][
+                    "new_grid_left"
+                ]
 
-                    # Triangulate new matches
-                    pairs[pair_key]["triangulated_matches"] = (
-                        dem_generation_tools.triangulate_sparse_matches(
-                            pairs[pair_key]["sensor_image_left"],
-                            pairs[pair_key]["sensor_image_right"],
-                            pairs[pair_key]["corrected_grid_left"],
-                            pairs[pair_key]["corrected_grid_right"],
-                            corrected_matches_array,
-                            geometry_plugin=geom_plugin,
-                        )
+                # Triangulate new matches
+                pairs[pair_key]["triangulated_matches"] = (
+                    dem_generation_tools.triangulate_sparse_matches(
+                        pairs[pair_key]["sensor_image_left"],
+                        pairs[pair_key]["sensor_image_right"],
+                        pairs[pair_key]["corrected_grid_left"],
+                        pairs[pair_key]["corrected_grid_right"],
+                        corrected_matches_array,
+                        geometry_plugin=geom_plugin,
                     )
+                )
 
-                    # filter triangulated_matches
-                    matches_filter_knn = (
-                        self.sparse_matching_app.get_matches_filter_knn()
-                    )
-                    matches_filter_dev_factor = (
-                        self.sparse_matching_app.get_matches_filter_dev_factor()
-                    )
-                    pairs[pair_key]["filtered_triangulated_matches"] = (
-                        sparse_matching_tools.filter_point_cloud_matches(
-                            pairs[pair_key]["triangulated_matches"],
-                            matches_filter_knn=matches_filter_knn,
-                            matches_filter_dev_factor=matches_filter_dev_factor,
-                        )
+                # filter triangulated_matches
+                matches_filter_knn = (
+                    self.sparse_matching_app.get_matches_filter_knn()
+                )
+                matches_filter_dev_factor = (
+                    self.sparse_matching_app.get_matches_filter_dev_factor()
+                )
+                pairs[pair_key]["filtered_triangulated_matches"] = (
+                    sparse_matching_tools.filter_point_cloud_matches(
+                        pairs[pair_key]["triangulated_matches"],
+                        matches_filter_knn=matches_filter_knn,
+                        matches_filter_dev_factor=matches_filter_dev_factor,
                     )
+                )
 
                 # Compute disp_min and disp_max
                 (dmin, dmax) = sparse_matching_tools.compute_disp_min_disp_max(
                     pairs[pair_key]["filtered_triangulated_matches"],
                     cars_orchestrator,
                     disp_margin=(
                         self.sparse_matching_app.get_disparity_margin()
```

### Comparing `cars-0.7.5/cars/starter.py` & `cars-0.7.6/cars/starter.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/cars.egg-info/PKG-INFO` & `cars-0.7.6/cars.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cars
-Version: 0.7.5
+Version: 0.7.6
 Summary: A satellite multi view stereo pipeline
 Home-page: https://cars.readthedocs.io/
 Author: CNES
 Author-email: cars@cnes.fr
 License: Apache License 2.0
 Project-URL: Source, https://github.com/CNES/cars
 Project-URL: Documentation, https://cars.readthedocs.io/en/latest/
@@ -44,15 +44,15 @@
 Requires-Dist: laspy[laszip]
 Requires-Dist: tbb==2020.3.254
 Requires-Dist: numba
 Requires-Dist: pandora[sgm]==1.6.*
 Requires-Dist: cars-rasterize==0.2.*
 Requires-Dist: cars-resample==0.1.*
 Requires-Dist: vlsift==0.1.*
-Requires-Dist: shareloc==0.2.0a2
+Requires-Dist: shareloc==0.2.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: isort>=5.8.0; extra == "dev"
 Requires-Dist: black>=24.1a1; extra == "dev"
 Requires-Dist: flake8>=3.9.1; extra == "dev"
@@ -113,16 +113,17 @@
 <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/animation_sat.gif" alt="drawing" width="400"/> |  <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/overview_dsm_3d.gif" alt="drawing" width="400"/>
 
 
 **CARS** is an open source 3D tool dedicated to produce **Digital Surface Models** from satellite imaging by photogrammetry.
 This Multiview Stereo framework is intended for massive DSM production with a robust, performant and modular design.
 
 Be aware that the project is new and is evolving to maturity with CNES usage roadmaps and projects such as:
-- <a href="https://co3d.cnes.fr/en/co3d-0">CO3D project &nbsp;&nbsp;&nbsp;  <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo_co3D_cnes.jpg" width="20" height="20"/></a>
-- <a href="https://www.ai4geo.eu/">AI4GEO project &nbsp;&nbsp;&nbsp;  </a>
+- <a href="https://co3d.cnes.fr/en/co3d-0">CO3D project &nbsp;&nbsp;&nbsp;  <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo_co3D_cnes.jpg" height="20"/></a>
+- <a href="https://www.ai4geo.eu">AI4GEO project &nbsp;&nbsp;&nbsp; <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo-ai4geo.png" height="20"/> </a>
+- <a href="https://www.evo-land.eu">Evoland project &nbsp;&nbsp;&nbsp; <img src="https://raw.githubusercontent.com/CNES/cars/master/docs/source/images/logo-evoland.png" height="20"/> </a>
 
 ## Quick start
 
 ### CARS Docker Image
 
 [![Docker Status](http://dockeri.co/image/cnes/cars)](https://hub.docker.com/r/cnes/cars)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cars Version: 0.7.5 Summary: A satellite multi view
+Metadata-Version: 2.1 Name: cars Version: 0.7.6 Summary: A satellite multi view
 stereo pipeline Home-page: https://cars.readthedocs.io/ Author: CNES Author-
 email: cars@cnes.fr License: Apache License 2.0 Project-URL: Source, https://
 github.com/CNES/cars Project-URL: Documentation, https://cars.readthedocs.io/
 en/latest/ Keywords: cars,3D,DEM,pandora,photogrammetry Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: End Users/Desktop Classifier:
 Intended Audience :: Science/Research Classifier: Environment :: Console
@@ -16,18 +16,18 @@
 dask>=2021.10.0 Requires-Dist: distributed>=2021.10.0 Requires-Dist: dask-
 jobqueue>=0.7.3 Requires-Dist: json-checker Requires-Dist: xarray Requires-
 Dist: tqdm Requires-Dist: netCDF4>=1.5.3 Requires-Dist: Shapely Requires-Dist:
 Fiona Requires-Dist: pyproj Requires-Dist: utm Requires-Dist: pandas Requires-
 Dist: urllib3<2.0,>=1.21.1 Requires-Dist: laspy[laszip] Requires-Dist:
 tbb==2020.3.254 Requires-Dist: numba Requires-Dist: pandora[sgm]==1.6.*
 Requires-Dist: cars-rasterize==0.2.* Requires-Dist: cars-resample==0.1.*
-Requires-Dist: vlsift==0.1.* Requires-Dist: shareloc==0.2.0a2 Provides-Extra:
-dev Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra ==
-"dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist: isort>=5.8.0;
-extra == "dev" Requires-Dist: black>=24.1a1; extra == "dev" Requires-Dist:
+Requires-Dist: vlsift==0.1.* Requires-Dist: shareloc==0.2.0 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev" Requires-Dist: isort>=5.8.0; extra ==
+"dev" Requires-Dist: black>=24.1a1; extra == "dev" Requires-Dist:
 flake8>=3.9.1; extra == "dev" Requires-Dist: flake8-comprehensions>=3.4.0;
 extra == "dev" Requires-Dist: flake8-bugbear<24.0.0,>=21.4.3; extra == "dev"
 Requires-Dist: jupyter_contrib_nbextensions; extra == "dev" Requires-Dist:
 pylint<3.0.0,>=2.8.12; extra == "dev" Requires-Dist: setuptools_scm; extra ==
 "dev" Requires-Dist: virtualenv; extra == "dev" Requires-Dist: configupdater;
 extra == "dev" Requires-Dist: twine; extra == "dev" Requires-Dist:
 notebook<7.0.0; extra == "dev" Requires-Dist: bokeh==2.4.3; extra == "dev"
@@ -56,39 +56,41 @@
 ------------------------:|:-------------------------: [drawing]|
 [drawing]**CARS** is an open source 3D tool dedicated to produce **Digital
 Surface Models** from satellite imaging by photogrammetry. This Multiview
 Stereo framework is intended for massive DSM production with a robust,
 performant and modular design. Be aware that the project is new and is evolving
 to maturity with CNES usage roadmaps and projects such as: - _C_O_3_D_ _p_r_o_j_e_c_t_ _ _ _ _ 
 _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_C_N_E_S_/_c_a_r_s_/_m_a_s_t_e_r_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/
-_l_o_g_o___c_o_3_D___c_n_e_s_._j_p_g_]- _A_I_4_G_E_O_ _p_r_o_j_e_c_t_ _ _ _ _ ## Quick start ### CARS Docker Image [!
-[Docker Status](http://dockeri.co/image/cnes/cars)](https://hub.docker.com/r/
-cnes/cars) CARS is available on Docker Hub and can be downloaded by: ``` bash
-docker pull cnes/cars ``` ### One main pipeline to generate DSM You only need
-to launch one command: ``` docker run -w /data -v "$(pwd)"/data_gizeh:/data
-cnes/cars /data/configfile.json ``` with one configuration input file
-("configfile.json") located in a "data" folder to be consistent with the
-previous command lines: ``` { "inputs": { "sensors" : { "one": { "image":
-"img1.tif", "geomodel": "img1.geom" }, "two": { "image": "img2.tif",
-"geomodel": "img2.geom" }, "three": { "image": "img3.tif", "geomodel":
-"img3.geom" } }, "pairing": [["one", "two"],["one", "three"]],
-"initial_elevation": "srtm_dir/N29E031_KHEOPS.tif" }, "output": { "out_dir":
-"outresults" } } ``` ### On the way to the Pyramids... You want to build the
-pyramids by yourself? Download our [open licence](https://www.etalab.gouv.fr/
-licence-ouverte-open-licence) Pleiades [data sample](https://
-raw.githubusercontent.com/CNES/cars/master/tutorials/data_gizeh.tar.bz2) to
-give CARS a try! ## Documentation Go to [CARS Main Documentation](https://
-cars.readthedocs.io/?badge=latest). ## Contribution To do a bug report or a
-contribution, see the [**Contribution Guide**](https://github.com/CNES/cars/
-blob/master/CONTRIBUTING.md). For project evolution, see [**Changelog**](https:
-//github.com/CNES/cars/blob/master/CHANGELOG.md). ## Credits See [Authors file]
-(https://github.com/CNES/cars/blob/master/AUTHORS.md) ## References - [Youssefi
-D., Michel, J., Sarrazin, E., Buffe, F., Cournet, M., Delvit, J., LâHelguen,
-C., Melet, O., Emilien, A., Bosman, J., 2020. Cars: A photogrammetry pipeline
-using dask graphs to construct a global 3d model. IGARSS - IEEE International
-Geoscience and Remote Sensing Symposium.](https://ieeexplore.ieee.org/document/
-9324020) - [Michel, J., Sarrazin, E., Youssefi, D., Cournet, M., Buffe, F.,
-Delvit, J., Emilien, A., Bosman, J., Melet, O., LâHelguen, C., 2020. A new
-satellite imagery stereo pipeline designed for scalability, robustness and
-performance. ISPRS - International Archives of the Photogrammetry, Remote
-Sensing and Spatial Information Sciences.](https://www.isprs-ann-photogramm-
-remote-sens-spatial-inf-sci.net/V-2-2020/171/2020/)
+_l_o_g_o___c_o_3_D___c_n_e_s_._j_p_g_]- _A_I_4_G_E_O_ _p_r_o_j_e_c_t_ _ _ _ _ _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/
+_C_N_E_S_/_c_a_r_s_/_m_a_s_t_e_r_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_l_o_g_o_-_a_i_4_g_e_o_._p_n_g_]- _E_v_o_l_a_n_d_ _p_r_o_j_e_c_t_ _ _ _ _ 
+_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_C_N_E_S_/_c_a_r_s_/_m_a_s_t_e_r_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_l_o_g_o_-
+_e_v_o_l_a_n_d_._p_n_g_]## Quick start ### CARS Docker Image [![Docker Status](http://
+dockeri.co/image/cnes/cars)](https://hub.docker.com/r/cnes/cars) CARS is
+available on Docker Hub and can be downloaded by: ``` bash docker pull cnes/
+cars ``` ### One main pipeline to generate DSM You only need to launch one
+command: ``` docker run -w /data -v "$(pwd)"/data_gizeh:/data cnes/cars /data/
+configfile.json ``` with one configuration input file ("configfile.json")
+located in a "data" folder to be consistent with the previous command lines:
+``` { "inputs": { "sensors" : { "one": { "image": "img1.tif", "geomodel":
+"img1.geom" }, "two": { "image": "img2.tif", "geomodel": "img2.geom" },
+"three": { "image": "img3.tif", "geomodel": "img3.geom" } }, "pairing": [
+["one", "two"],["one", "three"]], "initial_elevation": "srtm_dir/
+N29E031_KHEOPS.tif" }, "output": { "out_dir": "outresults" } } ``` ### On the
+way to the Pyramids... You want to build the pyramids by yourself? Download our
+[open licence](https://www.etalab.gouv.fr/licence-ouverte-open-licence)
+Pleiades [data sample](https://raw.githubusercontent.com/CNES/cars/master/
+tutorials/data_gizeh.tar.bz2) to give CARS a try! ## Documentation Go to [CARS
+Main Documentation](https://cars.readthedocs.io/?badge=latest). ## Contribution
+To do a bug report or a contribution, see the [**Contribution Guide**](https://
+github.com/CNES/cars/blob/master/CONTRIBUTING.md). For project evolution, see
+[**Changelog**](https://github.com/CNES/cars/blob/master/CHANGELOG.md). ##
+Credits See [Authors file](https://github.com/CNES/cars/blob/master/AUTHORS.md)
+## References - [Youssefi D., Michel, J., Sarrazin, E., Buffe, F., Cournet, M.,
+Delvit, J., LâHelguen, C., Melet, O., Emilien, A., Bosman, J., 2020. Cars: A
+photogrammetry pipeline using dask graphs to construct a global 3d model.
+IGARSS - IEEE International Geoscience and Remote Sensing Symposium.](https://
+ieeexplore.ieee.org/document/9324020) - [Michel, J., Sarrazin, E., Youssefi,
+D., Cournet, M., Buffe, F., Delvit, J., Emilien, A., Bosman, J., Melet, O.,
+LâHelguen, C., 2020. A new satellite imagery stereo pipeline designed for
+scalability, robustness and performance. ISPRS - International Archives of the
+Photogrammetry, Remote Sensing and Spatial Information Sciences.](https://
+www.isprs-ann-photogramm-remote-sens-spatial-inf-sci.net/V-2-2020/171/2020/)
```

### Comparing `cars-0.7.5/cars.egg-info/SOURCES.txt` & `cars-0.7.6/cars.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 cars/applications/grid_generation/grid_correction.py
 cars/applications/grid_generation/grid_generation.py
 cars/applications/grid_generation/grids.py
 cars/applications/holes_detection/__init__.py
 cars/applications/holes_detection/cloud_to_bbox.py
 cars/applications/holes_detection/holes_detection.py
 cars/applications/holes_detection/holes_detection_tools.py
+cars/applications/point_cloud_denoising/__init__.py
+cars/applications/point_cloud_denoising/point_cloud_denoising.py
 cars/applications/point_cloud_fusion/__init__.py
 cars/applications/point_cloud_fusion/cloud_fusion_constants.py
 cars/applications/point_cloud_fusion/mapping_to_terrain_tiles.py
 cars/applications/point_cloud_fusion/pc_tif_tools.py
 cars/applications/point_cloud_fusion/point_cloud_fusion.py
 cars/applications/point_cloud_fusion/point_cloud_tools.py
 cars/applications/point_cloud_outliers_removing/__init__.py
@@ -158,14 +160,15 @@
 cars/orchestrator/cluster/mp_cluster/mp_factorizer.py
 cars/orchestrator/cluster/mp_cluster/mp_objects.py
 cars/orchestrator/cluster/mp_cluster/mp_tools.py
 cars/orchestrator/cluster/mp_cluster/mp_wrapper.py
 cars/orchestrator/cluster/mp_cluster/multiprocessing_cluster.py
 cars/orchestrator/registry/__init__.py
 cars/orchestrator/registry/abstract_registry.py
+cars/orchestrator/registry/compute_registry.py
 cars/orchestrator/registry/id_generator.py
 cars/orchestrator/registry/replacer_registry.py
 cars/orchestrator/registry/saver_registry.py
 cars/orchestrator/registry/unseen_registry.py
 cars/pipelines/__init__.py
 cars/pipelines/pipeline.py
 cars/pipelines/pipeline_constants.py
```

### Comparing `cars-0.7.5/cars.egg-info/requires.txt` & `cars-0.7.6/cars.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 laspy[laszip]
 tbb==2020.3.254
 numba
 pandora[sgm]==1.6.*
 cars-rasterize==0.2.*
 cars-resample==0.1.*
 vlsift==0.1.*
-shareloc==0.2.0a2
+shareloc==0.2.0
 
 [dev]
 pytest
 pytest-cov
 pre-commit
 isort>=5.8.0
 black>=24.1a1
```

### Comparing `cars-0.7.5/env_cars.sh` & `cars-0.7.6/env_cars.sh`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/gdal-config` & `cars-0.7.6/gdal-config`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/otb_remote_module/app/CMakeLists.txt` & `cars-0.7.6/otb_remote_module/app/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/otb_remote_module/app/otbConvertSensorToGeoMultiPointFast.cxx` & `cars-0.7.6/otb_remote_module/app/otbConvertSensorToGeoMultiPointFast.cxx`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/otb_remote_module/app/otbEpipolarTriangulation.cxx` & `cars-0.7.6/otb_remote_module/app/otbEpipolarTriangulation.cxx`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/otb_remote_module/app/otbLocalizeInverse.cxx` & `cars-0.7.6/otb_remote_module/app/otbLocalizeInverse.cxx`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/otb_remote_module/data/rectified_ref.tif` & `cars-0.7.6/otb_remote_module/data/rectified_ref.tif`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/otb_remote_module/data/rectified_ref_mask.tif` & `cars-0.7.6/otb_remote_module/data/rectified_ref_mask.tif`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/otb_remote_module/data/rectified_sec.tif` & `cars-0.7.6/otb_remote_module/data/rectified_sec.tif`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/otb_remote_module/data/rectified_sec_mask.tif` & `cars-0.7.6/otb_remote_module/data/rectified_sec_mask.tif`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.h` & `cars-0.7.6/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.h`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.hxx` & `cars-0.7.6/otb_remote_module/include/otbOptiDisparityMapTo3DFilter.hxx`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/setup.cfg` & `cars-0.7.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 	laspy[laszip]
 	tbb==2020.3.254        # Intel optim for numba: KO for 2021 versions
 	numba
 	pandora[sgm]==1.6.*
 	cars-rasterize==0.2.*
 	cars-resample==0.1.*
 	vlsift==0.1.*
-	shareloc==0.2.0a2       # CARS geometry lib (optional but internal)
+	shareloc==0.2.0         # CARS geometry lib (optional but internal)
 package_dir = 
 	. = cars
 packages = find:
 scripts = 
 	env_cars.sh
 
 [options.extras_require]
```

### Comparing `cars-0.7.5/setup.py` & `cars-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `cars-0.7.5/sonar-project.properties` & `cars-0.7.6/sonar-project.properties`

 * *Files identical despite different names*

